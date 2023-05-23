# Comparing `tmp/matcha_ml-0.2.2.tar.gz` & `tmp/matcha_ml-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matcha_ml-0.2.2.tar", max compression
+gzip compressed data, was "matcha_ml-0.2.3.tar", max compression
```

## Comparing `matcha_ml-0.2.2.tar` & `matcha_ml-0.2.3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
--rw-r--r--   0        0        0    11357 2023-05-16 13:30:52.718239 matcha_ml-0.2.2/LICENSE
--rw-r--r--   0        0        0     4177 2023-05-16 14:32:14.573403 matcha_ml-0.2.2/README.md
--rw-r--r--   0        0        0     3465 2023-05-16 14:35:21.950085 matcha_ml-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        6 2023-05-16 14:35:32.438541 matcha_ml-0.2.2/src/matcha_ml/VERSION
--rw-r--r--   0        0        0      220 2023-05-16 13:30:52.737917 matcha_ml-0.2.2/src/matcha_ml/__init__.py
--rw-r--r--   0        0        0       70 2023-05-16 13:30:52.738233 matcha_ml-0.2.2/src/matcha_ml/cli/__init__.py
--rw-r--r--   0        0        0     7645 2023-05-16 13:30:52.738457 matcha_ml-0.2.2/src/matcha_ml/cli/_validation.py
--rw-r--r--   0        0        0     3928 2023-05-16 13:30:52.738697 matcha_ml-0.2.2/src/matcha_ml/cli/cli.py
--rw-r--r--   0        0        0     1298 2023-05-16 13:30:52.738966 matcha_ml-0.2.2/src/matcha_ml/cli/destroy.py
--rw-r--r--   0        0        0     3571 2023-05-16 13:30:52.739356 matcha_ml-0.2.2/src/matcha_ml/cli/provision.py
--rw-r--r--   0        0        0      278 2023-05-16 13:30:52.739662 matcha_ml-0.2.2/src/matcha_ml/cli/ui/emojis.py
--rw-r--r--   0        0        0     1173 2023-05-16 13:30:52.739975 matcha_ml-0.2.2/src/matcha_ml/cli/ui/print_messages.py
--rw-r--r--   0        0        0     2549 2023-05-16 13:30:52.740225 matcha_ml-0.2.2/src/matcha_ml/cli/ui/resource_message_builders.py
--rw-r--r--   0        0        0     1249 2023-05-16 13:30:52.740423 matcha_ml-0.2.2/src/matcha_ml/cli/ui/spinner.py
--rw-r--r--   0        0        0     1703 2023-05-16 13:30:52.740612 matcha_ml-0.2.2/src/matcha_ml/cli/ui/status_message_builders.py
--rw-r--r--   0        0        0     1780 2023-05-16 13:30:52.740937 matcha_ml-0.2.2/src/matcha_ml/core/core.py
--rw-r--r--   0        0        0     2535 2023-05-16 13:30:52.741158 matcha_ml-0.2.2/src/matcha_ml/errors.py
--rw-r--r--   0        0        0      882 2023-05-16 13:30:52.741464 matcha_ml-0.2.2/src/matcha_ml/infrastructure/.gitignore
--rw-r--r--   0        0        0     9245 2023-05-16 13:30:52.741780 matcha_ml-0.2.2/src/matcha_ml/infrastructure/.terraform.lock.hcl
--rw-r--r--   0        0        0     4696 2023-05-16 13:30:52.741981 matcha_ml-0.2.2/src/matcha_ml/infrastructure/README.md
--rw-r--r--   0        0        0     2213 2023-05-16 13:30:52.742246 matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/README.md
--rw-r--r--   0        0        0      439 2023-05-16 13:30:52.742403 matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/main.tf
--rw-r--r--   0        0        0     1437 2023-05-16 13:30:52.742560 matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/output.tf
--rw-r--r--   0        0        0      386 2023-05-16 13:30:52.742727 matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/variables.tf
--rw-r--r--   0        0        0     1605 2023-05-16 13:30:52.743071 matcha_ml-0.2.2/src/matcha_ml/infrastructure/azure_container_registry/README.md
--rw-r--r--   0        0        0      484 2023-05-16 13:30:52.743315 matcha_ml-0.2.2/src/matcha_ml/infrastructure/azure_container_registry/main.tf
--rw-r--r--   0        0        0      327 2023-05-16 13:30:52.743521 matcha_ml-0.2.2/src/matcha_ml/infrastructure/azure_container_registry/output.tf
--rw-r--r--   0        0        0      462 2023-05-16 13:30:52.743734 matcha_ml-0.2.2/src/matcha_ml/infrastructure/azure_container_registry/variables.tf
--rw-r--r--   0        0        0      625 2023-05-16 13:30:52.743945 matcha_ml-0.2.2/src/matcha_ml/infrastructure/configure_kubectl.tf
--rw-r--r--   0        0        0      337 2023-05-16 13:30:52.744107 matcha_ml-0.2.2/src/matcha_ml/infrastructure/helm.tf
--rw-r--r--   0        0        0     1107 2023-05-16 13:30:52.744511 matcha_ml-0.2.2/src/matcha_ml/infrastructure/kubernetes.tf
--rw-r--r--   0        0        0     1912 2023-05-16 13:30:52.744677 matcha_ml-0.2.2/src/matcha_ml/infrastructure/main.tf
--rw-r--r--   0        0        0     2208 2023-05-16 13:30:52.744957 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/README.md
--rw-r--r--   0        0        0      308 2023-05-16 13:30:52.745228 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/getURI.tf
--rw-r--r--   0        0        0     1314 2023-05-16 13:30:52.745733 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/main.tf
--rw-r--r--   0        0        0      251 2023-05-16 13:30:52.745977 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/output.tf
--rw-r--r--   0        0        0      383 2023-05-16 13:30:52.746211 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/providers.tf
--rw-r--r--   0        0        0      803 2023-05-16 13:30:52.746415 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/variables.tf
--rw-r--r--   0        0        0       81 2023-05-16 13:30:52.746583 matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/zenml_namespace.tf
--rw-r--r--   0        0        0     1945 2023-05-16 13:30:52.746754 matcha_ml-0.2.2/src/matcha_ml/infrastructure/output.tf
--rw-r--r--   0        0        0       33 2023-05-16 13:30:52.747081 matcha_ml-0.2.2/src/matcha_ml/infrastructure/printf.cmd
--rw-r--r--   0        0        0      782 2023-05-16 13:30:52.747345 matcha_ml-0.2.2/src/matcha_ml/infrastructure/providers.tf
--rw-r--r--   0        0        0      892 2023-05-16 13:30:52.747629 matcha_ml-0.2.2/src/matcha_ml/infrastructure/resource_group/README.md
--rw-r--r--   0        0        0      110 2023-05-16 13:30:52.747966 matcha_ml-0.2.2/src/matcha_ml/infrastructure/resource_group/main.tf
--rw-r--r--   0        0        0      106 2023-05-16 13:30:52.748218 matcha_ml-0.2.2/src/matcha_ml/infrastructure/resource_group/output.tf
--rw-r--r--   0        0        0      224 2023-05-16 13:30:52.748422 matcha_ml-0.2.2/src/matcha_ml/infrastructure/resource_group/variables.tf
--rw-r--r--   0        0        0     3010 2023-05-16 13:30:52.748665 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/README.md
--rw-r--r--   0        0        0     1894 2023-05-16 13:30:52.748903 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/istio.tf
--rw-r--r--   0        0        0     1158 2023-05-16 13:30:52.749104 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/main.tf
--rw-r--r--   0        0        0      663 2023-05-16 13:30:52.749379 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/outputs.tf
--rw-r--r--   0        0        0      925 2023-05-16 13:30:52.749651 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/permissions.tf
--rw-r--r--   0        0        0      380 2023-05-16 13:30:52.749843 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/providers.tf
--rw-r--r--   0        0        0      453 2023-05-16 13:30:52.750059 matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/variables.tf
--rw-r--r--   0        0        0     2914 2023-05-16 13:30:52.750412 matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/README.md
--rw-r--r--   0        0        0      866 2023-05-16 13:30:52.750629 matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/main.tf
--rw-r--r--   0        0        0     1779 2023-05-16 13:30:52.750835 matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/output.tf
--rw-r--r--   0        0        0      124 2023-05-16 13:30:52.751031 matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/providers.tf
--rw-r--r--   0        0        0      454 2023-05-16 13:30:52.751271 matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/variables.tf
--rw-r--r--   0        0        0      754 2023-05-16 13:30:52.751482 matcha_ml-0.2.2/src/matcha_ml/infrastructure/variables.tf
--rw-r--r--   0        0        0     6080 2023-05-16 13:30:52.751745 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/README.md
--rw-r--r--   0        0        0      216 2023-05-16 13:30:52.751978 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/getURL.tf
--rw-r--r--   0        0        0      979 2023-05-16 13:30:52.752167 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/ingress.tf
--rw-r--r--   0        0        0     3026 2023-05-16 13:30:52.752460 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/main.tf
--rw-r--r--   0        0        0      704 2023-05-16 13:30:52.752657 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/outputs.tf
--rw-r--r--   0        0        0      292 2023-05-16 13:30:52.752818 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/providers.tf
--rw-r--r--   0        0        0     1943 2023-05-16 13:30:52.753089 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/sql.tf
--rw-r--r--   0        0        0     4701 2023-05-16 13:30:52.753426 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/variables.tf
--rw-r--r--   0        0        0      342 2023-05-16 13:30:52.753742 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/Chart.yaml
--rw-r--r--   0        0        0     1987 2023-05-16 13:30:52.754025 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/NOTES.txt
--rw-r--r--   0        0        0     2054 2023-05-16 13:30:52.754318 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/_helpers.tpl
--rw-r--r--   0        0        0     1565 2023-05-16 13:30:52.754544 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/cert-secret.yaml
--rw-r--r--   0        0        0      910 2023-05-16 13:30:52.754804 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/hpa.yaml
--rw-r--r--   0        0        0    10774 2023-05-16 13:30:52.755024 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-deployment.yaml
--rw-r--r--   0        0        0     2225 2023-05-16 13:30:52.755283 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-ingress.yaml
--rw-r--r--   0        0        0     3584 2023-05-16 13:30:52.755448 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-secret.yaml
--rw-r--r--   0        0        0      367 2023-05-16 13:30:52.755599 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-service.yaml
--rw-r--r--   0        0        0      316 2023-05-16 13:30:52.755785 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/serviceaccount.yaml
--rw-r--r--   0        0        0      379 2023-05-16 13:30:52.756101 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/tests/test-connection.yaml
--rw-r--r--   0        0        0    11587 2023-05-16 13:30:52.756349 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/values.yaml
--rw-r--r--   0        0        0     3453 2023-05-16 13:30:52.756631 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/README.md
--rw-r--r--   0        0        0     1102 2023-05-16 13:30:52.756856 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/main.tf
--rw-r--r--   0        0        0     1926 2023-05-16 13:30:52.757124 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/output.tf
--rw-r--r--   0        0        0      468 2023-05-16 13:30:52.757274 matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/variables.tf
--rw-r--r--   0        0        0      103 2023-05-16 13:30:52.757540 matcha_ml-0.2.2/src/matcha_ml/services/__init__.py
--rw-r--r--   0        0        0     7929 2023-05-16 13:30:52.757814 matcha_ml-0.2.2/src/matcha_ml/services/azure_service.py
--rw-r--r--   0        0        0     2652 2023-05-16 13:30:52.757983 matcha_ml-0.2.2/src/matcha_ml/services/matcha_state.py
--rw-r--r--   0        0        0     5503 2023-05-16 13:30:52.758191 matcha_ml-0.2.2/src/matcha_ml/services/terraform_service.py
--rw-r--r--   0        0        0       41 2023-05-16 13:30:52.758697 matcha_ml-0.2.2/src/matcha_ml/templates/__init__.py
--rw-r--r--   0        0        0     7396 2023-05-16 13:30:52.759121 matcha_ml-0.2.2/src/matcha_ml/templates/build_templates/azure_template.py
--rw-r--r--   0        0        0    10509 2023-05-16 13:30:52.759483 matcha_ml-0.2.2/src/matcha_ml/templates/run_template.py
--rw-r--r--   0        0        0     5978 1970-01-01 00:00:00.000000 matcha_ml-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 13:30:52.718239 matcha_ml-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4177 2023-05-18 15:36:43.261690 matcha_ml-0.2.3/README.md
+-rw-r--r--   0        0        0     3484 2023-05-18 15:41:44.588686 matcha_ml-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        6 2023-05-18 15:41:50.066694 matcha_ml-0.2.3/src/matcha_ml/VERSION
+-rw-r--r--   0        0        0      220 2023-05-16 13:30:52.737917 matcha_ml-0.2.3/src/matcha_ml/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-16 13:30:52.738233 matcha_ml-0.2.3/src/matcha_ml/cli/__init__.py
+-rw-r--r--   0        0        0     7645 2023-05-16 13:30:52.738457 matcha_ml-0.2.3/src/matcha_ml/cli/_validation.py
+-rw-r--r--   0        0        0     3928 2023-05-18 15:36:43.263898 matcha_ml-0.2.3/src/matcha_ml/cli/cli.py
+-rw-r--r--   0        0        0     1298 2023-05-16 13:30:52.738966 matcha_ml-0.2.3/src/matcha_ml/cli/destroy.py
+-rw-r--r--   0        0        0     3571 2023-05-18 09:13:20.950590 matcha_ml-0.2.3/src/matcha_ml/cli/provision.py
+-rw-r--r--   0        0        0      278 2023-05-16 13:30:52.739662 matcha_ml-0.2.3/src/matcha_ml/cli/ui/emojis.py
+-rw-r--r--   0        0        0     1173 2023-05-16 13:30:52.739975 matcha_ml-0.2.3/src/matcha_ml/cli/ui/print_messages.py
+-rw-r--r--   0        0        0     2549 2023-05-16 13:30:52.740225 matcha_ml-0.2.3/src/matcha_ml/cli/ui/resource_message_builders.py
+-rw-r--r--   0        0        0     1249 2023-05-16 13:30:52.740423 matcha_ml-0.2.3/src/matcha_ml/cli/ui/spinner.py
+-rw-r--r--   0        0        0     1703 2023-05-16 13:30:52.740612 matcha_ml-0.2.3/src/matcha_ml/cli/ui/status_message_builders.py
+-rw-r--r--   0        0        0     1780 2023-05-18 15:36:43.264193 matcha_ml-0.2.3/src/matcha_ml/core/core.py
+-rw-r--r--   0        0        0     2535 2023-05-16 13:30:52.741158 matcha_ml-0.2.3/src/matcha_ml/errors.py
+-rw-r--r--   0        0        0      882 2023-05-18 09:13:20.951530 matcha_ml-0.2.3/src/matcha_ml/infrastructure/.gitignore
+-rw-r--r--   0        0        0     9245 2023-05-18 09:13:20.951796 matcha_ml-0.2.3/src/matcha_ml/infrastructure/.terraform.lock.hcl
+-rw-r--r--   0        0        0     4696 2023-05-18 09:13:20.951974 matcha_ml-0.2.3/src/matcha_ml/infrastructure/README.md
+-rw-r--r--   0        0        0     2213 2023-05-18 09:13:20.952290 matcha_ml-0.2.3/src/matcha_ml/infrastructure/aks/README.md
+-rw-r--r--   0        0        0      439 2023-05-18 09:13:20.952517 matcha_ml-0.2.3/src/matcha_ml/infrastructure/aks/main.tf
+-rw-r--r--   0        0        0     1437 2023-05-18 09:13:20.952726 matcha_ml-0.2.3/src/matcha_ml/infrastructure/aks/output.tf
+-rw-r--r--   0        0        0      386 2023-05-18 09:13:20.952883 matcha_ml-0.2.3/src/matcha_ml/infrastructure/aks/variables.tf
+-rw-r--r--   0        0        0     1605 2023-05-18 09:13:20.953093 matcha_ml-0.2.3/src/matcha_ml/infrastructure/azure_container_registry/README.md
+-rw-r--r--   0        0        0      484 2023-05-18 09:13:20.953228 matcha_ml-0.2.3/src/matcha_ml/infrastructure/azure_container_registry/main.tf
+-rw-r--r--   0        0        0      327 2023-05-18 09:13:20.953351 matcha_ml-0.2.3/src/matcha_ml/infrastructure/azure_container_registry/output.tf
+-rw-r--r--   0        0        0      462 2023-05-18 09:13:20.953503 matcha_ml-0.2.3/src/matcha_ml/infrastructure/azure_container_registry/variables.tf
+-rw-r--r--   0        0        0      625 2023-05-18 09:13:20.953762 matcha_ml-0.2.3/src/matcha_ml/infrastructure/configure_kubectl.tf
+-rw-r--r--   0        0        0      337 2023-05-18 09:13:20.953902 matcha_ml-0.2.3/src/matcha_ml/infrastructure/helm.tf
+-rw-r--r--   0        0        0     1107 2023-05-18 09:13:20.954036 matcha_ml-0.2.3/src/matcha_ml/infrastructure/kubernetes.tf
+-rw-r--r--   0        0        0     1912 2023-05-18 09:13:20.954199 matcha_ml-0.2.3/src/matcha_ml/infrastructure/main.tf
+-rw-r--r--   0        0        0     2208 2023-05-18 09:13:20.954450 matcha_ml-0.2.3/src/matcha_ml/infrastructure/mlflow_module/README.md
+-rw-r--r--   0        0        0      308 2023-05-18 09:13:20.954586 matcha_ml-0.2.3/src/matcha_ml/infrastructure/mlflow_module/getURI.tf
+-rw-r--r--   0        0        0     1314 2023-05-18 09:13:20.954702 matcha_ml-0.2.3/src/matcha_ml/infrastructure/mlflow_module/main.tf
+-rw-r--r--   0        0        0      251 2023-05-18 09:13:20.954823 matcha_ml-0.2.3/src/matcha_ml/infrastructure/mlflow_module/output.tf
+-rw-r--r--   0        0        0      383 2023-05-18 09:13:20.955056 matcha_ml-0.2.3/src/matcha_ml/infrastructure/mlflow_module/providers.tf
+-rw-r--r--   0        0        0      803 2023-05-18 09:13:20.955222 matcha_ml-0.2.3/src/matcha_ml/infrastructure/mlflow_module/variables.tf
+-rw-r--r--   0        0        0       81 2023-05-18 09:13:20.955363 matcha_ml-0.2.3/src/matcha_ml/infrastructure/mlflow_module/zenml_namespace.tf
+-rw-r--r--   0        0        0     1945 2023-05-18 09:13:20.955497 matcha_ml-0.2.3/src/matcha_ml/infrastructure/output.tf
+-rw-r--r--   0        0        0       33 2023-05-18 09:13:20.955606 matcha_ml-0.2.3/src/matcha_ml/infrastructure/printf.cmd
+-rw-r--r--   0        0        0      782 2023-05-18 09:13:20.955749 matcha_ml-0.2.3/src/matcha_ml/infrastructure/providers.tf
+-rw-r--r--   0        0        0      892 2023-05-18 09:13:20.955951 matcha_ml-0.2.3/src/matcha_ml/infrastructure/resource_group/README.md
+-rw-r--r--   0        0        0      110 2023-05-18 09:13:20.956071 matcha_ml-0.2.3/src/matcha_ml/infrastructure/resource_group/main.tf
+-rw-r--r--   0        0        0      106 2023-05-18 09:13:20.956262 matcha_ml-0.2.3/src/matcha_ml/infrastructure/resource_group/output.tf
+-rw-r--r--   0        0        0      224 2023-05-18 09:13:20.956387 matcha_ml-0.2.3/src/matcha_ml/infrastructure/resource_group/variables.tf
+-rw-r--r--   0        0        0     3010 2023-05-18 09:13:20.956587 matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/README.md
+-rw-r--r--   0        0        0     1894 2023-05-18 09:13:20.956718 matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/istio.tf
+-rw-r--r--   0        0        0     1158 2023-05-18 09:13:20.956859 matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/main.tf
+-rw-r--r--   0        0        0      663 2023-05-18 09:13:20.956986 matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/outputs.tf
+-rw-r--r--   0        0        0      925 2023-05-18 09:13:20.957115 matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/permissions.tf
+-rw-r--r--   0        0        0      380 2023-05-18 09:13:20.957225 matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/providers.tf
+-rw-r--r--   0        0        0      453 2023-05-18 09:13:20.957488 matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/variables.tf
+-rw-r--r--   0        0        0     2914 2023-05-18 09:13:20.957700 matcha_ml-0.2.3/src/matcha_ml/infrastructure/storage/README.md
+-rw-r--r--   0        0        0      866 2023-05-18 09:13:20.957831 matcha_ml-0.2.3/src/matcha_ml/infrastructure/storage/main.tf
+-rw-r--r--   0        0        0     1779 2023-05-18 09:13:20.957950 matcha_ml-0.2.3/src/matcha_ml/infrastructure/storage/output.tf
+-rw-r--r--   0        0        0      124 2023-05-18 09:13:20.958051 matcha_ml-0.2.3/src/matcha_ml/infrastructure/storage/providers.tf
+-rw-r--r--   0        0        0      454 2023-05-18 09:13:20.958154 matcha_ml-0.2.3/src/matcha_ml/infrastructure/storage/variables.tf
+-rw-r--r--   0        0        0      754 2023-05-18 09:13:20.958358 matcha_ml-0.2.3/src/matcha_ml/infrastructure/variables.tf
+-rw-r--r--   0        0        0     6080 2023-05-18 09:13:20.958521 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/README.md
+-rw-r--r--   0        0        0      216 2023-05-18 09:13:20.958669 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/getURL.tf
+-rw-r--r--   0        0        0      979 2023-05-18 09:13:20.958777 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/ingress.tf
+-rw-r--r--   0        0        0     3026 2023-05-18 09:13:20.958884 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/main.tf
+-rw-r--r--   0        0        0      704 2023-05-18 09:13:20.958995 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/outputs.tf
+-rw-r--r--   0        0        0      292 2023-05-18 09:13:20.959095 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/providers.tf
+-rw-r--r--   0        0        0     1943 2023-05-18 09:13:20.959195 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/sql.tf
+-rw-r--r--   0        0        0     4701 2023-05-18 09:13:20.959359 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/variables.tf
+-rw-r--r--   0        0        0      342 2023-05-18 09:13:20.959519 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/Chart.yaml
+-rw-r--r--   0        0        0     1987 2023-05-18 09:13:20.959719 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/NOTES.txt
+-rw-r--r--   0        0        0     2054 2023-05-18 09:13:20.959838 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1565 2023-05-18 09:13:20.959946 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/cert-secret.yaml
+-rw-r--r--   0        0        0      910 2023-05-18 09:13:20.960059 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/hpa.yaml
+-rw-r--r--   0        0        0    10774 2023-05-18 09:13:20.960230 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-deployment.yaml
+-rw-r--r--   0        0        0     2225 2023-05-18 09:13:20.960357 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-ingress.yaml
+-rw-r--r--   0        0        0     3584 2023-05-18 09:13:20.960473 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-secret.yaml
+-rw-r--r--   0        0        0      367 2023-05-18 09:13:20.960590 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-service.yaml
+-rw-r--r--   0        0        0      316 2023-05-18 09:13:20.960702 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/serviceaccount.yaml
+-rw-r--r--   0        0        0      379 2023-05-18 09:13:20.960867 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/tests/test-connection.yaml
+-rw-r--r--   0        0        0    11587 2023-05-18 09:13:20.961025 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/values.yaml
+-rw-r--r--   0        0        0     3453 2023-05-18 09:13:20.961191 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zenml_storage/README.md
+-rw-r--r--   0        0        0     1102 2023-05-18 09:13:20.961298 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zenml_storage/main.tf
+-rw-r--r--   0        0        0     1926 2023-05-18 09:13:20.961416 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zenml_storage/output.tf
+-rw-r--r--   0        0        0      468 2023-05-18 09:13:20.961601 matcha_ml-0.2.3/src/matcha_ml/infrastructure/zenml_storage/variables.tf
+-rw-r--r--   0        0        0      103 2023-05-16 13:30:52.757540 matcha_ml-0.2.3/src/matcha_ml/services/__init__.py
+-rw-r--r--   0        0        0     7929 2023-05-18 15:32:21.444890 matcha_ml-0.2.3/src/matcha_ml/services/azure_service.py
+-rw-r--r--   0        0        0     2652 2023-05-18 15:36:43.264372 matcha_ml-0.2.3/src/matcha_ml/services/matcha_state.py
+-rw-r--r--   0        0        0     5503 2023-05-18 09:13:20.961965 matcha_ml-0.2.3/src/matcha_ml/services/terraform_service.py
+-rw-r--r--   0        0        0       41 2023-05-16 13:30:52.758697 matcha_ml-0.2.3/src/matcha_ml/templates/__init__.py
+-rw-r--r--   0        0        0     7396 2023-05-18 15:36:43.265011 matcha_ml-0.2.3/src/matcha_ml/templates/build_templates/azure_template.py
+-rw-r--r--   0        0        0    10509 2023-05-18 15:36:43.265485 matcha_ml-0.2.3/src/matcha_ml/templates/run_template.py
+-rw-r--r--   0        0        0     6012 1970-01-01 00:00:00.000000 matcha_ml-0.2.3/PKG-INFO
```

### Comparing `matcha_ml-0.2.2/LICENSE` & `matcha_ml-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/README.md` & `matcha_ml-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/pyproject.toml` & `matcha_ml-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "matcha-ml"
-version = "0.2.2"
+version = "0.2.3"
 description = "Matcha: A open source tool for provisioning MLOps environments to the cloud."
 authors = ["FuzzyLabs <info@fuzzylabs.ai>"]
 license = "Apache-2.0"
 homepage = "http://fuzzylabs.github.io/matcha"
 documentation = "http://fuzzylabs.github.io/matcha"
 repository = "https://github.com/fuzzylabs/matcha"
 readme = "README.md"
@@ -48,14 +48,15 @@
 
 azure-identity = "^1.12.0"
 azure-mgmt-resource = "^23.0.0"
 azure-mgmt-subscription = "^3.1.1"
 azure-mgmt-authorization = "^3.0.0"
 azure-mgmt-confluent = "^1.0.0"
 pyyaml = "^5.4.1"
+urllib3 = "1.26.6"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.1.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 mypy = "^1.1.1"
```

### Comparing `matcha_ml-0.2.2/src/matcha_ml/cli/_validation.py` & `matcha_ml-0.2.3/src/matcha_ml/cli/_validation.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/cli/cli.py` & `matcha_ml-0.2.3/src/matcha_ml/cli/cli.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/cli/destroy.py` & `matcha_ml-0.2.3/src/matcha_ml/cli/destroy.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/cli/provision.py` & `matcha_ml-0.2.3/src/matcha_ml/cli/provision.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/cli/ui/print_messages.py` & `matcha_ml-0.2.3/src/matcha_ml/cli/ui/print_messages.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/cli/ui/resource_message_builders.py` & `matcha_ml-0.2.3/src/matcha_ml/cli/ui/resource_message_builders.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/cli/ui/spinner.py` & `matcha_ml-0.2.3/src/matcha_ml/cli/ui/spinner.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/cli/ui/status_message_builders.py` & `matcha_ml-0.2.3/src/matcha_ml/cli/ui/status_message_builders.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/core/core.py` & `matcha_ml-0.2.3/src/matcha_ml/core/core.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/errors.py` & `matcha_ml-0.2.3/src/matcha_ml/errors.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/.gitignore` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/.gitignore`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/.terraform.lock.hcl` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/.terraform.lock.hcl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/README.md` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/README.md` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/aks/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/aks/output.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/aks/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/azure_container_registry/README.md` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/azure_container_registry/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/configure_kubectl.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/configure_kubectl.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/kubernetes.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/kubernetes.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/main.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/README.md` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/mlflow_module/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/main.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/mlflow_module/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/mlflow_module/variables.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/mlflow_module/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/output.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/providers.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/providers.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/resource_group/README.md` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/resource_group/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/README.md` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/istio.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/istio.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/main.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/outputs.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/outputs.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/seldon/permissions.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/seldon/permissions.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/README.md` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/storage/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/main.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/storage/output.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/variables.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/README.md` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/ingress.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/ingress.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/main.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/outputs.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/outputs.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/sql.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/sql.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/variables.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/variables.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/NOTES.txt` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/NOTES.txt`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/_helpers.tpl` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/cert-secret.yaml` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/cert-secret.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/hpa.yaml` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/hpa.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-deployment.yaml` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-deployment.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-ingress.yaml` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-ingress.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-secret.yaml` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/templates/server-secret.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zen_server/zenml_helm/values.yaml` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zen_server/zenml_helm/values.yaml`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/README.md` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zenml_storage/README.md`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/main.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zenml_storage/main.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/infrastructure/zenml_storage/output.tf` & `matcha_ml-0.2.3/src/matcha_ml/infrastructure/zenml_storage/output.tf`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/services/azure_service.py` & `matcha_ml-0.2.3/src/matcha_ml/services/azure_service.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/services/matcha_state.py` & `matcha_ml-0.2.3/src/matcha_ml/services/matcha_state.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/services/terraform_service.py` & `matcha_ml-0.2.3/src/matcha_ml/services/terraform_service.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/templates/build_templates/azure_template.py` & `matcha_ml-0.2.3/src/matcha_ml/templates/build_templates/azure_template.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/src/matcha_ml/templates/run_template.py` & `matcha_ml-0.2.3/src/matcha_ml/templates/run_template.py`

 * *Files identical despite different names*

### Comparing `matcha_ml-0.2.2/PKG-INFO` & `matcha_ml-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matcha-ml
-Version: 0.2.2
+Version: 0.2.3
 Summary: Matcha: A open source tool for provisioning MLOps environments to the cloud.
 Home-page: http://fuzzylabs.github.io/matcha
 License: Apache-2.0
 Keywords: production,mlops,devops,machine learning
 Author: FuzzyLabs
 Author-email: info@fuzzylabs.ai
 Requires-Python: >=3.8,<4.0
@@ -28,14 +28,15 @@
 Requires-Dist: azure-mgmt-authorization (>=3.0.0,<4.0.0)
 Requires-Dist: azure-mgmt-confluent (>=1.0.0,<2.0.0)
 Requires-Dist: azure-mgmt-resource (>=23.0.0,<24.0.0)
 Requires-Dist: azure-mgmt-subscription (>=3.1.1,<4.0.0)
 Requires-Dist: python-terraform (>=0.10.1,<0.11.0)
 Requires-Dist: pyyaml (>=5.4.1,<6.0.0)
 Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
+Requires-Dist: urllib3 (==1.26.6)
 Project-URL: Bug Tracker, https://github.com/fuzzylabs/matcha/issues
 Project-URL: Documentation, http://fuzzylabs.github.io/matcha
 Project-URL: Repository, https://github.com/fuzzylabs/matcha
 Description-Content-Type: text/markdown
 
 <h1 align="center">
     <img src="docs/img/logo.png" width="200" style="max-width: 200px"></img>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: matcha-ml Version: 0.2.2 Summary: Matcha: A open
+Metadata-Version: 2.1 Name: matcha-ml Version: 0.2.3 Summary: Matcha: A open
 source tool for provisioning MLOps environments to the cloud. Home-page: http:/
 /fuzzylabs.github.io/matcha License: Apache-2.0 Keywords:
 production,mlops,devops,machine learning Author: FuzzyLabs Author-email:
 info@fuzzylabs.ai Requires-Python: >=3.8,<4.0 Classifier: Development Status ::
 3 - Alpha Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
@@ -15,17 +15,18 @@
 Classifier: Topic :: Software Development Classifier: Topic :: Software
 Development :: Libraries :: Python Modules Requires-Dist: azure-identity
 (>=1.12.0,<2.0.0) Requires-Dist: azure-mgmt-authorization (>=3.0.0,<4.0.0)
 Requires-Dist: azure-mgmt-confluent (>=1.0.0,<2.0.0) Requires-Dist: azure-mgmt-
 resource (>=23.0.0,<24.0.0) Requires-Dist: azure-mgmt-subscription
 (>=3.1.1,<4.0.0) Requires-Dist: python-terraform (>=0.10.1,<0.11.0) Requires-
 Dist: pyyaml (>=5.4.1,<6.0.0) Requires-Dist: typer[all] (>=0.7.0,<0.8.0)
-Project-URL: Bug Tracker, https://github.com/fuzzylabs/matcha/issues Project-
-URL: Documentation, http://fuzzylabs.github.io/matcha Project-URL: Repository,
-https://github.com/fuzzylabs/matcha Description-Content-Type: text/markdown
+Requires-Dist: urllib3 (==1.26.6) Project-URL: Bug Tracker, https://github.com/
+fuzzylabs/matcha/issues Project-URL: Documentation, http://fuzzylabs.github.io/
+matcha Project-URL: Repository, https://github.com/fuzzylabs/matcha
+Description-Content-Type: text/markdown
                        ****** [docs/img/logo.png] ******
                     [Build] [License] [Release] [Downloads]
                **** Open source MLOps on Azure in one step ****
 If you train machine learning models, then you know the challenge of going from
 _experiment_ to _production_. There's a vast range of tools that promise to
 help, from experiment tracking through to model deployment, but setting these
 up requires a lot of time and cloud engineering knowledge. **Matcha removes the
```

