# Comparing `tmp/phiterm-1.6.8.tar.gz` & `tmp/phiterm-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.6.8.tar", last modified: Tue May 23 01:10:36 2023, max compression
+gzip compressed data, was "phiterm-1.6.9.tar", last modified: Tue May 23 01:46:30 2023, max compression
```

## Comparing `phiterm-1.6.8.tar` & `phiterm-1.6.9.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.849757 phiterm-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-23 01:10:17.000000 phiterm-1.6.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 01:10:36.845756 phiterm-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 01:10:17.000000 phiterm-1.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.821756 phiterm-1.6.8/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.821756 phiterm-1.6.8/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.821756 phiterm-1.6.8/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.825756 phiterm-1.6.8/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36902 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.829756 phiterm-1.6.8/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.829756 phiterm-1.6.8/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.829756 phiterm-1.6.8/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.829756 phiterm-1.6.8/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.833756 phiterm-1.6.8/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.833756 phiterm-1.6.8/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.833756 phiterm-1.6.8/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.833756 phiterm-1.6.8/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.817756 phiterm-1.6.8/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.837756 phiterm-1.6.8/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.837756 phiterm-1.6.8/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.837756 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.841756 phiterm-1.6.8/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.841756 phiterm-1.6.8/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.841756 phiterm-1.6.8/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.845756 phiterm-1.6.8/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.845756 phiterm-1.6.8/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    45502 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-23 01:10:17.000000 phiterm-1.6.8/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.821756 phiterm-1.6.8/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 01:10:36.000000 phiterm-1.6.8/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-23 01:10:17.000000 phiterm-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:10:36.849757 phiterm-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 01:10:17.000000 phiterm-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:10:36.845756 phiterm-1.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 01:10:17.000000 phiterm-1.6.8/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.912390 phiterm-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-23 01:46:07.000000 phiterm-1.6.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 01:46:30.912390 phiterm-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-23 01:46:07.000000 phiterm-1.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5436 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36902 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.900390 phiterm-1.6.9/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.892389 phiterm-1.6.9/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.904390 phiterm-1.6.9/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.908390 phiterm-1.6.9/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.908390 phiterm-1.6.9/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.908390 phiterm-1.6.9/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.908390 phiterm-1.6.9/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45502 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-23 01:46:07.000000 phiterm-1.6.9/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.896389 phiterm-1.6.9/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-23 01:46:30.000000 phiterm-1.6.9/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-23 01:46:07.000000 phiterm-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 01:46:30.912390 phiterm-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 01:46:07.000000 phiterm-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 01:46:30.908390 phiterm-1.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 01:46:07.000000 phiterm-1.6.9/tests/test_backend_api.py
```

### Comparing `phiterm-1.6.8/LICENSE.md` & `phiterm-1.6.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/api/client.py` & `phiterm-1.6.9/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/api/routes.py` & `phiterm-1.6.9/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/api/user.py` & `phiterm-1.6.9/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/api/workspace.py` & `phiterm-1.6.9/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/aws/aws_operator.py` & `phiterm-1.6.9/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/cli/cli_app.py` & `phiterm-1.6.9/phiterm/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/cli/cli_operator.py` & `phiterm-1.6.9/phiterm/cli/cli_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/cli/dx/dx_app.py` & `phiterm-1.6.9/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.6.9/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.6.9/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.6.9/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/cli/wf/wf_app.py` & `phiterm-1.6.9/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/cli/ws/ws_app.py` & `phiterm-1.6.9/phiterm/cli/ws/ws_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/conf/auth.py` & `phiterm-1.6.9/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/conf/constants.py` & `phiterm-1.6.9/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/conf/phi_conf.py` & `phiterm-1.6.9/phiterm/conf/phi_conf.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/databox/databox_operator.py` & `phiterm-1.6.9/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/docker/docker_operator.py` & `phiterm-1.6.9/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/enums/user.py` & `phiterm-1.6.9/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/k8s/k8s_operator.py` & `phiterm-1.6.9/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.6.9/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.6.9/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.6.9/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.6.9/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/local/local_operator.py` & `phiterm-1.6.9/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/release/release_schemas.py` & `phiterm-1.6.9/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/release/ws_releases.py` & `phiterm-1.6.9/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/schemas/user.py` & `phiterm-1.6.9/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/schemas/user_schemas.py` & `phiterm-1.6.9/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/schemas/workspace.py` & `phiterm-1.6.9/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.6.9/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.6.9/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.6.9/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.6.9/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.6.9/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.6.9/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.6.9/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.6.9/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.6.9/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.6.9/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/cli_auth_server.py` & `phiterm-1.6.9/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/cli_console.py` & `phiterm-1.6.9/phiterm/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/common.py` & `phiterm-1.6.9/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/dttm.py` & `phiterm-1.6.9/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/enums.py` & `phiterm-1.6.9/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/filesystem.py` & `phiterm-1.6.9/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/git.py` & `phiterm-1.6.9/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/load_env.py` & `phiterm-1.6.9/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/log.py` & `phiterm-1.6.9/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/pyproject.py` & `phiterm-1.6.9/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/utils/ws_filter.py` & `phiterm-1.6.9/phiterm/utils/ws_filter.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/workflow/wf_operator.py` & `phiterm-1.6.9/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/workflow/wf_utils.py` & `phiterm-1.6.9/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/workspace/phi_ws_data.py` & `phiterm-1.6.9/phiterm/workspace/phi_ws_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/workspace/ws_enums.py` & `phiterm-1.6.9/phiterm/workspace/ws_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/workspace/ws_loader.py` & `phiterm-1.6.9/phiterm/workspace/ws_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,35 +53,35 @@
         logger.debug(f"--^^-- Loading workspace from: {config_dir_path}")
         workspace_config_objects = {}
         config_files = config_dir_path.rglob("*.py")
         for _config_file in config_files:
             if _config_file.name == "__init__.py":
                 continue
             logger.debug(f"Reading file: {_config_file}")
-            parent_dir = _config_file.parent.name
-            parent_parent_dir = _config_file.parent.parent.name
-            if parent_dir in ("resources", "tests") or parent_parent_dir in (
-                "resources",
-                "tests",
-            ):
-                logger.debug(f"Skipping file in {parent_dir}")
-                continue
             try:
                 python_objects = get_python_objects_from_module(_config_file)
                 for obj_name, obj in python_objects.items():
                     _type_name = obj.__class__.__name__
                     if _type_name in [
                         "WorkspaceSettings",
                         "DockerConfig",
                         "K8sConfig",
                         "AwsConfig",
                     ]:
                         workspace_config_objects[obj_name] = obj
             except Exception as e:
-                logger.warning(f"Error in {_config_file}: {e}")
+                parent_dir = _config_file.parent.name
+                parent_parent_dir = _config_file.parent.parent.name
+                if parent_dir in ("resources", "tests") or parent_parent_dir in (
+                    "resources",
+                    "tests",
+                ):
+                    pass
+                else:
+                    logger.warning(f"Error in {_config_file}: {e}")
                 pass
 
         # logger.debug(f"workspace_config_objects: {workspace_config_objects}")
         for obj_name, obj in workspace_config_objects.items():
             _obj_type = obj.__class__.__name__
             logger.debug(f"Adding {obj_name}: | Type: {_obj_type}")
             if _obj_type == "WorkspaceSettings":
```

### Comparing `phiterm-1.6.8/phiterm/workspace/ws_operator.py` & `phiterm-1.6.9/phiterm/workspace/ws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/workspace/ws_schemas.py` & `phiterm-1.6.9/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm/workspace/ws_utils.py` & `phiterm-1.6.9/phiterm/workspace/ws_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/phiterm.egg-info/SOURCES.txt` & `phiterm-1.6.9/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.8/pyproject.toml` & `phiterm-1.6.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.6.8"
+version = "1.6.9"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

