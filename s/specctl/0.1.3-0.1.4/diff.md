# Comparing `tmp/specctl-0.1.3.tar.gz` & `tmp/specctl-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specctl-0.1.3.tar", max compression
+gzip compressed data, was "specctl-0.1.4.tar", max compression
```

## Comparing `specctl-0.1.3.tar` & `specctl-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0    10142 2023-05-09 01:54:35.901782 specctl-0.1.3/LICENSE
--rw-r--r--   0        0        0    12192 2023-05-19 00:46:47.759640 specctl-0.1.3/README.md
--rw-r--r--   0        0        0      441 2023-05-19 00:48:17.631594 specctl-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-19 00:47:05.045382 specctl-0.1.3/specctl/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 00:47:05.064218 specctl-0.1.3/specctl/ecs2k8s/__init__.py
--rw-r--r--   0        0        0    11015 2023-05-19 00:47:05.058566 specctl-0.1.3/specctl/ecs2k8s/ecs_parser.py
--rw-r--r--   0        0        0    11322 2023-05-19 00:47:05.070202 specctl-0.1.3/specctl/ecs2k8s/ecs_reader_writer.py
--rw-r--r--   0        0        0     2351 2023-05-19 00:47:05.062861 specctl-0.1.3/specctl/ecs2k8s/k8s_objects.py
--rw-r--r--   0        0        0     3444 2023-05-19 00:47:05.082926 specctl-0.1.3/specctl/k8s2ecs/README.md
--rw-r--r--   0        0        0        0 2023-05-19 00:47:05.074140 specctl-0.1.3/specctl/k8s2ecs/__init__.py
--rw-r--r--   0        0        0     1628 2023-05-19 00:47:05.083773 specctl-0.1.3/specctl/k8s2ecs/ecs_objects.py
--rw-r--r--   0        0        0     5175 2023-05-19 00:47:05.081450 specctl-0.1.3/specctl/k8s2ecs/ecs_output.py
--rw-r--r--   0        0        0    12173 2023-05-19 00:47:05.073674 specctl-0.1.3/specctl/k8s2ecs/ingress.py
--rw-r--r--   0        0        0    27795 2023-05-19 00:47:05.090036 specctl-0.1.3/specctl/k8s2ecs/k8s_parser.py
--rw-r--r--   0        0        0     6465 2023-05-19 00:47:05.088657 specctl-0.1.3/specctl/k8s2ecs/k8s_reader.py
--rw-r--r--   0        0        0     5453 2023-05-19 00:47:05.072663 specctl-0.1.3/specctl/k8s2ecs/tf_output.py
--rw-r--r--   0        0        0     1873 2023-05-19 00:47:05.092119 specctl-0.1.3/specctl/quantity.py
--rw-r--r--   0        0        0     5377 2023-05-19 00:47:05.091443 specctl-0.1.3/specctl/specctl.py
--rw-r--r--   0        0        0     1757 2023-05-19 00:47:05.071056 specctl-0.1.3/specctl/utils.py
--rw-r--r--   0        0        0    12943 1970-01-01 00:00:00.000000 specctl-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    10142 2023-05-09 01:54:35.901782 specctl-0.1.4/LICENSE
+-rw-r--r--   0        0        0    12312 2023-05-22 06:31:33.527898 specctl-0.1.4/README.md
+-rw-r--r--   0        0        0      441 2023-05-23 02:47:42.253843 specctl-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-19 00:47:05.045382 specctl-0.1.4/specctl/__init__.py
+-rw-r--r--   0        0        0     1936 2023-05-22 06:31:33.528528 specctl-0.1.4/specctl/ecs2k8s/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 00:47:05.064218 specctl-0.1.4/specctl/ecs2k8s/__init__.py
+-rw-r--r--   0        0        0    11027 2023-05-23 02:47:25.078738 specctl-0.1.4/specctl/ecs2k8s/ecs_parser.py
+-rw-r--r--   0        0        0    11874 2023-05-23 02:47:25.079390 specctl-0.1.4/specctl/ecs2k8s/ecs_reader_writer.py
+-rw-r--r--   0        0        0     2351 2023-05-19 00:47:05.062861 specctl-0.1.4/specctl/ecs2k8s/k8s_objects.py
+-rw-r--r--   0        0        0     4561 2023-05-22 06:31:33.529266 specctl-0.1.4/specctl/k8s2ecs/README.md
+-rw-r--r--   0        0        0        0 2023-05-19 00:47:05.074140 specctl-0.1.4/specctl/k8s2ecs/__init__.py
+-rw-r--r--   0        0        0     1628 2023-05-19 00:47:05.083773 specctl-0.1.4/specctl/k8s2ecs/ecs_objects.py
+-rw-r--r--   0        0        0     5176 2023-05-23 00:31:18.914322 specctl-0.1.4/specctl/k8s2ecs/ecs_output.py
+-rw-r--r--   0        0        0    12229 2023-05-23 00:31:18.915252 specctl-0.1.4/specctl/k8s2ecs/ingress.py
+-rw-r--r--   0        0        0    27795 2023-05-19 00:47:05.090036 specctl-0.1.4/specctl/k8s2ecs/k8s_parser.py
+-rw-r--r--   0        0        0     6465 2023-05-19 00:47:05.088657 specctl-0.1.4/specctl/k8s2ecs/k8s_reader.py
+-rw-r--r--   0        0        0     5453 2023-05-19 00:47:05.072663 specctl-0.1.4/specctl/k8s2ecs/tf_output.py
+-rw-r--r--   0        0        0     1873 2023-05-19 00:47:05.092119 specctl-0.1.4/specctl/quantity.py
+-rw-r--r--   0        0        0     5377 2023-05-19 00:47:05.091443 specctl-0.1.4/specctl/specctl.py
+-rw-r--r--   0        0        0     1757 2023-05-19 00:47:05.071056 specctl-0.1.4/specctl/utils.py
+-rw-r--r--   0        0        0    13063 1970-01-01 00:00:00.000000 specctl-0.1.4/PKG-INFO
```

### Comparing `specctl-0.1.3/LICENSE` & `specctl-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `specctl-0.1.3/README.md` & `specctl-0.1.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # specctl 
-`specctl` is a command-line based tool to extract and transform Kubernetes objects to ECS and vice versa. It has two modes, `-m k2e` (default) convert Kubernetes to ECS and `-m e2k` for ECS to Kubernetes. Currenly, only ECS Fargate is supported. 
-For Kubernetes to ECS converstion the tool uses [Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) to create all the necessary AWS resources needed to run services and tasks on ECS. For ECS to Kubernetes you can simply use `kubectl` on the generated spec. 
+The `specctl` is a command-line based tool to extract and transform Kubernetes objects to ECS and vice versa. It has two modes, `-m k2e` (default) convert Kubernetes to ECS and `-m e2k` for ECS to Kubernetes. Currently, only ECS Fargate is supported.
+
+For Kubernetes to ECS conversion, `specctl` can read and convert Kubernetes objects either from Kubernetes YAML specification files or from Kubernetes clusters. The tool uses [Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) to create all the necessary AWS resources needed to run services and tasks on ECS. 
+
+For ECS to Kubernetes, `specctl` can read and convert ECS and related AWS objects from an AWS account where the ECS cluster is running. Once the Kubernetes YAML specifications are generated, you can simply use `kubectl` on the generated spec. 
 
 ### Getting Started
 * Install [Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)
-* Install `mwinit` to get access to the Gitlab repo. 
 * I would recommend to use `virtualenv` to avoid any conflicts with preinstalled Python libraries. All testing done on Mac OS 13.2.1.
+* Fork the repo and clone
 
 ```bash
-git clone git@ssh.gitlab.aws.dev:arvsoni/specctl.git
+git clone https://github.com/awslabs/specctl.git
 cd specctl
-pip install --editable .
+pip install virtualenv
+virtualenv .venv
+source .venv/bin/activate
+pip install specctl
 specctl --help
 ```
 ### Kubernetes to ECS
 Let us first create an ECS cluster:
 ```bash
 cd terraform/core-infra
 terraform init
@@ -41,31 +47,29 @@
 ```
 Click on the URL and you should see the NGINX home page! **Congrats, you have converted Kubernetes simple spec to ECS!**
 
 #### OK, what did `specctl` do?
 The `specctl` will generate following artifacts in `./output` directory.
 * `namespaces` : contains (a) Kubernetes namespaces for creating CloudMap namespaces for service discovery, and (b) SSM parameters with both simple string obtained from ConfigMaps and secure strings obtained from Secrets. The Terraform code to create required AWS resources is also generated. The terraform init and apply commands created all the resources based on data extracted from Kubernetes namespaces, configmaps, and secrets.
 * `<namespace>/<service>` : a set of folders one for each Kubernetes namespace and inside that a service folder one for each Kubernetes service in the namespace. The Terraform code to create the service, task definition, and if applicable ALB resources, is auto-generated and available in the service folder. The terraform init and apply commands created all resources based on data extracted from Kubernetes service and deployments.
-
 To clean up, assuming you are in `specctl` directory
 ```bash
 cd output/default/nginx-svc
 terraform destroy --auto-approve
 cd ../../namespaces
 terraform destroy --auto-approve
 cd ../..
 rm -rf output
 ```
-
 ### Conversions at scale from a cluster
 `specctl` is built with scalable migration in mind. For the Kubernetes to ECS migration, for example, every service has its Terraform code and extracted settings in a seprate folder. By adding a CI/CD pipeline and S3 bucket (for Terraform state), the deployment of ECS services can be completely automated for all the services. The Terraform infra-as-code approach makes it easy to extend and customize to meet customer's application needs. 
 
-To test conversion at scale for Kubernetes to ECS, we can use the `tests/retail-store` example. Start by creating this application in Kubernetes. You can use `minikube`if you don't have a Kubernetes cluster handy. There is a convenience script `specctl/bin/migrate.sh` to recursively apply `terraform init` and `terraform apply --auto-approve` in each of the service directories. 
+To test conversion at scale for Kubernetes to ECS, we can use the `tests/retail-store` example. Start by creating this application in Kubernetes. You can use `minikube`if you don't have a Kubernetes cluster handy. 
 
-Assuming you are in `specctl` directory.
+Assuming you are in `specctl` directory and you have cleaned up the previous example `./output` directory.
 ```bash
 kubectl apply -f tests/retail-store
 ...
 ... (wait for apply to finish)
 ...
 ```
 ```bash
@@ -76,15 +80,17 @@
 ...
 cd output
 cd namespaces
 terraform init && terraform apply --auto-approve
 ...
 ...
 ```
-The above will create all the shared resources in various namespaces that are extracted. Shared resources include SSM Parameters, ALBs, CloudMap namespaces. Now you can run the `migrate.sh` script from the `/output` folder to recursively create all the extracted services. Below is assuming your are in `namespaces` folder from above step.
+The above will create all the shared resources in various namespaces that are extracted. Shared resources include SSM Parameters, ALBs, CloudMap namespaces. 
+
+There is a convenience script `specctl/bin/migrate.sh` to recursively apply `terraform init` and `terraform apply --auto-approve` in each of the service directories. Below is assuming your are in `namespaces` folder from above step. 
 
 ```bash
 cd ..
 source ../bin/migrate.sh apply
 ```
 You should see a lot of services created in ECS - `ui`,`carts`, `catalog` ... The `ui` service is load balanced and if you access the ALB URL you will see the same home page as when you access the `ui` service in Kubernetes. Play around with the app and make sure all the inter-service communication is working in both ECS and Kubernetes!
 **Congrats, you have just migrated 7 services in matter of minutes!** And same approach can be adapted to do scalable migrations.
@@ -100,43 +106,44 @@
 mv ../namespaces .
 cd namespaces
 terraform destroy --auto-approve
 cd ../..
 rm -rf output
 ```
 #### What all K8s objects does specctl convert to ECS? 
-- [X] Deployment
+- [X] Deployment and ReplicaSets
 - [X] Service including ClusterIP, Load Balancer
-- [X] Ingress with HTTP 
+- [X] Ingress with HTTP and HTTPS (AWS ALB only)
 - [X] Pod IAM via Service Account
 - [X] ConfigMaps
 - [X] Secrets
-- [X] Container specs along with init-containers, and named ports handling
+- [X] Container specs along with init-containers, and named port handling
 - [X] Fargate size determination based on cpu and mem reservation and limit
-- [X] Ingress with HTTPS esp. certificate handling
 - [X] Pod Security Group
+- [ ] DaemonSets
 - [ ] Jobs
 - [ ] Container volumes
+- [ ] StatefulSets
 - [ ] ?
 
-**Note** K8s allows multiple variations for the service discovery, for example, `svc-name` or `svc-name.namespace` or `svc-name.namespace.svc.cluster.local`. But in ECS the service discovery name is `svc-name.namespace` (where namespace is in CloudMap). You may need to do some manual changes to the service endpoints configurations if they are not able to discover each other. This concern applies to both ECS to K8s and K8s to ECS conversions. 
+**Note:** Kubernetes allows multiple variations for the service discovery, for example, `svc-name` or `svc-name.namespace` or `svc-name.namespace.svc.cluster.local`. But in ECS the service discovery name is `svc-name.namespace` (where namespace is in CloudMap). You may need to do some manual changes to the service endpoints configurations if they are not able to discover each other. This concern applies to both ECS to K8s and K8s to ECS conversions. 
 
 ### ECS to Kubernetes 
 To do the reverse simply run the below command and it will generate the Kubernetes deployment, service, configmap, and secrets YAML specification files. Note to change the cluster name and/or region name if you created ECS cluster in a different region or are using your own ECS cluster in a different region. You can create Kubernetes namespace and deploy the generated artifacts to test. 
 
 ```bash
 specctl -m e2k --ecs_region_name us-west-2 --ecs_cluster_name core-infra
 ls output/core-infra
 ```
 #### What all ECS objects does specctl convert to Kubernetes?
 - [X] ECS Task to Pod
 - [X] ECS Service to K8s Service & K8s Deployment  
 - [X] ECS Load Balanced Service to K8s Ingress
-- [X] SSP Parameter Simple Strings to K8s ConfigMap 
-- [X] SSP Parameter SecureString to K8s Secrets
+- [X] SSM Parameter Simple Strings to K8s ConfigMap 
+- [X] SSM Parameter SecureString to K8s Secrets
 - [X] Secrets Manager to K8s Secrets
 - [X] Task IAM to IAM annotations on Service Account
 - [X] Task Security Group to EKS Security Group Policy 
 - [X] First "." delimiter of CloudMap namespace to K8s namespace 
 
 ### Features of `specctl`
 ```bash
@@ -167,24 +174,24 @@
   -o, --output_directory TEXT     Path to output directory
   --ecs_cluster_name TEXT         ECS cluster to extract services and tasks
   --ecs_region_name TEXT          Region name for ECS cluster
   --sgp                           Create EKS Security Group Policy from task
                                   security groups
   --help                          Show this message and exit.
 ```
-* `specctl` currenly reads and extracts information from Kubernetes `Deployment`,`Service`, `ConfigMap`, and `Secrets` objects. It can read these objects from a file/folder or directly from a Kubernetes cluster.
+* `specctl` can read Kubernetes objects from a file/folder or directly from a Kubernetes cluster.
 * If `-s` source path to the K8s YAML file or directory is provided, `specctl` will use those specification files to read and extract information to create `taskdefinition.json`, `servicedefinition.json`, and `terraform.tfvars` files.
 * If `-c`, cluster kubeconfig context is provided, then `specctl` will read the deployments, services, configmaps, secrets directly from K8s cluster and generate the output files.
 * If both `-s` and `-c` are provided then behavior is same as just `-s`, that is, to process file(s) at that source path.
 * If neither `-s` and `-c` are provided then `specctl` will load all the contexts from kubeconfig and prompt the user to pick one.
 * The `-l` option is to control logging. Default log level is `INFO`.
 * The `--td_file` refers to JSON file for task definition and is set to `taskdefinition.json`. The actual output file is of the format `<output_directory>/<service_namespace>/<service_name>/taskdefinition.json`
 * The `--sd_file` refers to JSON file for service definition and is set to `servicedefinition.json`. The actual output file is of the format `<output_directory>/<service_namespace>/<service_name>/taskdefinition.json`
-* The `--input_file` is to provide additional input to add or update the parsed input in task definition and service definition JSON output. See sample [input.json](./lb_service_input.json.example) files for content format.
+* The `--input_file` is to provide additional input to add or update the parsed input in task definition and service definition JSON output. 
 * The `--tfvars_file` is to provide the terraform tfvars output and set to `terraform.tfvars`. The actual output is of the form `<output_directory>/terraform.tfvars` and `<output_directory>/<service_namespace>/<service_name>/terraform.fvars`.
 * The `-d` options is to provide the path to Terraform modules directory. Default is "./terraform" from where the specctl command is launched.
 * The `--tf_modules_name_map` is to provide a map of what are the folder names for the `namespaces`, `ecs-lb-service`, and `ecs-backend-service` modules. Default is `"namespaces:namespaces,ecs-lb-service:ecs-lb-service,ecs-backend-service:ecs-backend-service"`. Keep the keys same and change module folder name as applicable. The module folders should be under the Terraform modules directory provided by `-d` option.
 * The `--tf_files` is to provide a comma separated string of Terraform files to copy from the modules. Default is `"main.tf,versions.tf,variables.tf,outputs.tf"`
 * The `-o` is the path to output directory. Default is `./output`.
-* The `--ecs_cluster_name` is to provide name of ECS cluster to extract services and tasks to conver to Kubernetes specifications
+* The `--ecs_cluster_name` is to provide name of ECS cluster to extract services and tasks to convert to Kubernetes specifications
 * The `--ecs_region_name` is to provide region name for ECS cluster
 * The `--sgp` flag is to control whether or not to create EKS security group policies based on ECS task security groups. By default specctl doesn't create the security group policies because pod networking can be quite different.
```

### Comparing `specctl-0.1.3/specctl/ecs2k8s/ecs_parser.py` & `specctl-0.1.4/specctl/ecs2k8s/ecs_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import re
 from ..utils import dict_check
 import logging
 
 logger = logging.getLogger(__name__)
 
 def k8s_conform(input_string):
-    return(re.sub("[^a-zA-Z0-9]+","-", input_string).lower())
+    return(re.sub("[^a-zA-Z0-9]+","-", input_string).lower().rstrip("-"))
 
 def get_pod_iam(task_def, k8s_svc_account):
     pod_iam = task_def.get("taskRoleArn")
     if pod_iam is not None and len(pod_iam) > 0 :
         k8s_svc_account["metadata"]["annotations"]["eks.amazonaws.com/role-arn"] = pod_iam
     return
```

### Comparing `specctl-0.1.3/specctl/ecs2k8s/ecs_reader_writer.py` & `specctl-0.1.4/specctl/ecs2k8s/ecs_reader_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import boto3
 import botocore
 import botocore.exceptions
 from botocore.config import Config
 from pick import pick
 from .ecs_parser import ecs_parser, ssm_secret_parser, ingress_parser, namespace_parser
 import os
+import re
+import json
 import yaml
 import base64
 import logging
 
 
 logger = logging.getLogger(__name__)
 
@@ -111,15 +113,15 @@
         secrets = cd.get("secrets",[])
         for item in secrets:
             valueFrom = item.get("valueFrom", None)
             if valueFrom is None or valueFrom in already_seen:
                 continue
             if "arn:aws:secretsmanager" in valueFrom:
                 try:
-                    response = secret_mgr_client.get_secret_value(SecretId=valueFrom)
+                    response = retrieve_secret_value(secret_mgr_client, valueFrom)
                 except botocore.exceptions.ClientError as error:
                     logger.error("Unable to get secret %s %s"%(valueFrom, error))
                 if response is None:
                     continue
                 name = response.get("Name","")
                 type = "SecureString"
                 value = base64.b64encode(response.get("SecretString","").encode("ascii")).decode("ascii")
@@ -136,14 +138,32 @@
                 value = base64.b64encode(parameter.get("Value","").encode("ascii")).decode("ascii")
             if len(name)<=0:
                 continue
             already_seen[valueFrom] = {"name":name, "value":value, "type":type}
             if type == "String":
                already_seen[valueFrom]["value"] = base64.b64decode(value.encode("ascii")).decode("ascii")
     return(already_seen)
+    
+
+def retrieve_secret_value(secrets_client, value_from):
+    if not value_from.endswith("::"):
+        return secrets_client.get_secret_value(SecretId=value_from)
+    match = re.match(r"^(.*):([^:]+)::?$", value_from)
+    arn = match.group(1)
+    key = match.group(2)
+    response = secrets_client.get_secret_value(SecretId=arn)
+    secret_json = json.loads(response['SecretString'])
+    if key not in secret_json:
+        return None
+    return {
+        'ARN': arn,
+        'Name': key,
+        'SecretString': secret_json[key],
+    }
+    
 
 def ecs_get_task_definition(client, task_definition):
     response = client.describe_task_definition(
         taskDefinition= task_definition,
         include=['TAGS']
     )
     return(response.get("taskDefinition", None))
@@ -224,15 +244,14 @@
                 logger.error("Skipping service %s that has no task definition"%(svc_name))
                 continue
             task_def = ecs_get_task_definition(client, task_def_arn) 
             k8s_secrets_and_configmaps = get_ssm_and_secrets(region_name, task_def)
             svc_lbs = svc_def.get("loadBalancers")
             if svc_lbs is not None and len(svc_lbs)>0:
                 get_lb_details(region_name, svc_lbs)
-            
             svc_namespace = ""
             svc_registries = svc_def.get("serviceRegistries")
             if svc_registries is not None and len(svc_registries) > 0:
                 svc_registry_arn = svc_registries[0].get("registryArn")
                 if svc_registry_arn is not None and len(svc_registry_arn)>0:
                     svc_namespace = get_cloudmap_namespace(region_name, svc_registry_arn)
```

### Comparing `specctl-0.1.3/specctl/ecs2k8s/k8s_objects.py` & `specctl-0.1.4/specctl/ecs2k8s/k8s_objects.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.3/specctl/k8s2ecs/README.md` & `specctl-0.1.4/specctl/k8s2ecs/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,20 @@
-### K8s to ECS Fargate specification conversion details
-The `specctl` script parses Kubernetes objects and extracts attributes needed for related ECS objects. The `*_input.json` file is used to provide additional input that are necessary to run task and services on ECS. Remember when you run containers in ECS Fargate on AWS cloud you need to specify CPU, memory, subnet(s), and IAM. And also some optional but crucial elements such as log groups for container logs. All these additional input are not present in Kubernetes specification and require to be provided through the `*_input.json` file.
+### Kubernetes to ECS Fargate specification conversion details
+The `specctl` script parses Kubernetes objects and extracts attributes needed for related ECS objects. The tool can convert from either the Kubernetes YAML specification files, or from a Kubernetes cluster. If converting from Kubernetes cluster, your user role will need read access for the Kubernetes resources mentioned below.
 
-Below is a list of Kubernetes objects that are parsed along with details on what attributes are extracted and how those attributes are mapped to ECS objects.
-* Kubernetes Deployment object has some attributes that map to ECS service and some that map to ECS task definition object. The deployment related to replica set and settings associated with rolling deployment become part of ECS service definition. For example, `replicas` become `desiredCount`, rolling deployment settings `maxSurge`, `maxUnavailable`become part of ECS service `deploymentConfiguration` mapping to attributes `maximumPercent`, and `minimumHealthyPercent` respectively (with little bit of manipulation). The deployment template part which captures pod and associated container definitions become part of the ECS task definition.
+* Kubernetes Deployment object has some attributes that map to ECS service and some that map to ECS task definition object. The deployment related to replica set and settings associated with rolling deployment become part of ECS service definition. For example, `replicas` become `desiredCount`, rolling deployment settings `maxSurge`, `maxUnavailable` become part of ECS service `deploymentConfiguration` mapping to attributes `maximumPercent`, and `minimumHealthyPercent` respectively (with little bit of manipulation). The deployment template part which captures pod and associated container definitions becomes part of the ECS task definition.
 
-* Kubernetes Service object maps to ECS service. Currently, this script only handles ClusterIP and Load Balanced service type. The ClusterIP service is simply an ECS service with a CloudMap based DNS entry. For example, `my-service.namespace.cluster.local`, will remain same in ECS with `my-service` as the service name and `namespace.cluster.local` as the domain registry in CloudMap. The Kubernetes load balanced service maps to ECS service with an NLB. There one important challenge though. In ECS both the CloudMap registry and ALB/NLB have to be created beforehand and appropriate values have to be provided in ECS service definition. Another important aspect to note is that in Kubernetes pods and services are independent objects. Kubernetes services use label selectors to identify the pods for a specific service. In ECS service, tasks are creaetd as part of service creation. The tasks belong to service and are not independent, so there is no need for label selectors in ECS.
+* Kubernetes Service object maps to ECS service. Currently, this script only handles ClusterIP and Load Balanced service type. The ClusterIP service is simply an ECS service with a CloudMap based DNS entry. For example, `my-service.namespace.svc.cluster.local`, will remain same in ECS with `my-service` as the service name and `namespace.svc.cluster.local` as the domain registry in CloudMap. The Kubernetes load balanced service can maps to ECS service with an NLB or ALB. In practice AWS ALB is more commonly used for load balancing in ECS. So, currently, the Terraform code provisions only AWS ALB. In ECS both the CloudMap registry and ALB (or NLB) have to be created beforehand and appropriate values have to be provided in ECS service definition. That is why we use Terraform to create these resources and provide appropriate attributes to ECS service definition. Another important aspect to note is that in Kubernetes pods and services are independent objects. Kubernetes services use label selectors to identify the pods for a specific service. In ECS service, tasks are created as part of service creation. The tasks belong to service and are not independent, so there is no need for label selectors in ECS.
 
 * Kubernetes Pod object maps to ECS task and task definition. Container definitions form the bulk of pod specification. Kubernetes and ECS have equivalent attributes for most of the container definition needs such as volumes, environment variables, ports.
 
 * Kubernetes ConfigMap object maps to AWS SSM Parameter. Just like Kubernetes pods can access the ConfigMap parameters and values, ECS tasks can also access parameters from SSM Parameter Store. The important difference is that the SSM Parameters have to be created separately and the parameter name has to be supplied in ECS task container definitions.
 
-* Kubernetes Secrets object maps to AWS SSM Parameter Store or AWS Secrets Manager. Just like Kubernetes pods can access the secrets during runtime, ECS tasks can also access secrets from Parameter Store or Secrets Manager securely during runtime. Again the important difference is that secrets need to be stored in either SSM Parameter Store or Secrets Manager and the parameter name/ARN has to be made available in container definition.
+* Kubernetes Secrets object maps to AWS SSM Parameter Store or AWS Secrets Manager. Just like Kubernetes pods can access the secrets during runtime, ECS tasks can also access secrets from Parameter Store or Secrets Manager securely during runtime. Again the important difference is that secrets need to be stored in either SSM Parameter Store or Secrets Manager and the parameter name/ARN has to be made available in container definition. Currently, the script stores Kubernetes Secrets in SSM Parameter Store as SecureString. 
 
+* Aspects such as `envFrom`, `configMapKeyRef`, and `secretKeyRef` are handled appropriately to ensure the containers in tasks are able to refer and fetch resources from SSM Parameter Store.
+
+* Kubernetes Ingress object maps to AWS ALB. Most of the conversion logic for ingress objects is to create ALB, listeners, listener rules, and target groups. Once all the ALB related resources are created from parsing Kubernetes ingress, all we need to do is pass the target group(s) to ECS service definition.
+
+* Kubernetes Service Account can be used to associate AWS IAM roles for pods. In ECS, task IAM roles can be specified in task definition. So the Service Account and any associated IAM roles are added to the ECS task definition.
+
+* When using Kubernetes on AWS, you may also be using Pod Security Groups through `vpcresources.k8s.aws/v1beta1/securitygrouppolicies` resource. The tool will extract these and associate with ECS tasks. However, most likely, your ECS Fargate networking environment will be different from Kubernetes environment. It is best to handle the security groups in the Terraform module associated with ECS Fargate service definitions.
```

### Comparing `specctl-0.1.3/specctl/k8s2ecs/ecs_objects.py` & `specctl-0.1.4/specctl/k8s2ecs/ecs_objects.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.3/specctl/k8s2ecs/ecs_output.py` & `specctl-0.1.4/specctl/k8s2ecs/ecs_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     return task_def
 
 
 
 
 # options needs task definition file td_file ;
 # service definition file sd_file ;
-# additiona input file input_file
+# additional input file input_file
 # The first two are to write the json output
 # The last input_file is to read additional json parameters for task/container/service
 def ecs_print(output_dict, options):
     input_file = options.get("input_file")
     additional_input = []
     if len(input_file) > 0:
         with open(input_file,'r') as ipf:
```

### Comparing `specctl-0.1.3/specctl/k8s2ecs/ingress.py` & `specctl-0.1.4/specctl/k8s2ecs/ingress.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,28 +243,29 @@
                 if svc_name != backend_service_name:
                     continue
                 svc_lb_ports_list = svc.get("lb_ports",{})
                 for svc_lb_ports in svc_lb_ports_list:
                     if dict_check(svc_lb_ports) is None: continue
                     svc_port_number = svc_lb_ports.get("service_port")
                     svc_port_name = svc_lb_ports.get("service_port_name")
+                    svc_protocol = svc_lb_ports.get("listener_protocol","HTTP")
                     if svc_port_number is None: continue
                     if (backend_service_port_number is not None \
                         and svc_port_number == backend_service_port_number) or \
                         (backend_service_port_name is not None and svc_port_name is not None\
                         and backend_service_port_name == svc_port_name):
                         target_port = svc_lb_ports.get("listener_port")
                         target_group_key = ingress_alb_name+"-"+svc_name+"-"+svc_namespace+"-"+str(target_port)
                         target_group_name = svc_name+"-"+svc_namespace+"-"+str(target_port)
                         svc_lb_health_check = svc.get("lb_health_check_path")
                         if svc_lb_health_check is not None: ingress["health_check"]["path"]=svc_lb_health_check 
                         ingress["target_groups"][target_group_key] = {
                             "name": target_group_name,
                             "port": target_port,
-                            "protocol": listener_rule.get("protocol","HTTP"),
+                            "protocol": svc_protocol,
                             "tags":{"key":target_group_key},
                             "health_check":ingress.get("health_check",{})
                         }
                         listener_rule["target_group_key"]=target_group_key
                         svc_target_groups = svc.get("ingress_target_groups")
                         if svc_target_groups is None:
                             svc["ingress_target_groups"] = []
```

### Comparing `specctl-0.1.3/specctl/k8s2ecs/k8s_parser.py` & `specctl-0.1.4/specctl/k8s2ecs/k8s_parser.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.3/specctl/k8s2ecs/k8s_reader.py` & `specctl-0.1.4/specctl/k8s2ecs/k8s_reader.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.3/specctl/k8s2ecs/tf_output.py` & `specctl-0.1.4/specctl/k8s2ecs/tf_output.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.3/specctl/quantity.py` & `specctl-0.1.4/specctl/quantity.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.3/specctl/specctl.py` & `specctl-0.1.4/specctl/specctl.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.3/specctl/utils.py` & `specctl-0.1.4/specctl/utils.py`

 * *Files identical despite different names*

### Comparing `specctl-0.1.3/PKG-INFO` & `specctl-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specctl
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: Apache 2.0
 Author: Arvind Soni
 Author-email: arvindsoni@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -17,26 +17,32 @@
 Requires-Dist: boto3 (>=1.26.130,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: kubernetes (>=26.1.0,<27.0.0)
 Requires-Dist: pick (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # specctl 
-`specctl` is a command-line based tool to extract and transform Kubernetes objects to ECS and vice versa. It has two modes, `-m k2e` (default) convert Kubernetes to ECS and `-m e2k` for ECS to Kubernetes. Currenly, only ECS Fargate is supported. 
-For Kubernetes to ECS converstion the tool uses [Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) to create all the necessary AWS resources needed to run services and tasks on ECS. For ECS to Kubernetes you can simply use `kubectl` on the generated spec. 
+The `specctl` is a command-line based tool to extract and transform Kubernetes objects to ECS and vice versa. It has two modes, `-m k2e` (default) convert Kubernetes to ECS and `-m e2k` for ECS to Kubernetes. Currently, only ECS Fargate is supported.
+
+For Kubernetes to ECS conversion, `specctl` can read and convert Kubernetes objects either from Kubernetes YAML specification files or from Kubernetes clusters. The tool uses [Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli) to create all the necessary AWS resources needed to run services and tasks on ECS. 
+
+For ECS to Kubernetes, `specctl` can read and convert ECS and related AWS objects from an AWS account where the ECS cluster is running. Once the Kubernetes YAML specifications are generated, you can simply use `kubectl` on the generated spec. 
 
 ### Getting Started
 * Install [Terraform](https://developer.hashicorp.com/terraform/tutorials/aws-get-started/install-cli)
-* Install `mwinit` to get access to the Gitlab repo. 
 * I would recommend to use `virtualenv` to avoid any conflicts with preinstalled Python libraries. All testing done on Mac OS 13.2.1.
+* Fork the repo and clone
 
 ```bash
-git clone git@ssh.gitlab.aws.dev:arvsoni/specctl.git
+git clone https://github.com/awslabs/specctl.git
 cd specctl
-pip install --editable .
+pip install virtualenv
+virtualenv .venv
+source .venv/bin/activate
+pip install specctl
 specctl --help
 ```
 ### Kubernetes to ECS
 Let us first create an ECS cluster:
 ```bash
 cd terraform/core-infra
 terraform init
@@ -63,31 +69,29 @@
 ```
 Click on the URL and you should see the NGINX home page! **Congrats, you have converted Kubernetes simple spec to ECS!**
 
 #### OK, what did `specctl` do?
 The `specctl` will generate following artifacts in `./output` directory.
 * `namespaces` : contains (a) Kubernetes namespaces for creating CloudMap namespaces for service discovery, and (b) SSM parameters with both simple string obtained from ConfigMaps and secure strings obtained from Secrets. The Terraform code to create required AWS resources is also generated. The terraform init and apply commands created all the resources based on data extracted from Kubernetes namespaces, configmaps, and secrets.
 * `<namespace>/<service>` : a set of folders one for each Kubernetes namespace and inside that a service folder one for each Kubernetes service in the namespace. The Terraform code to create the service, task definition, and if applicable ALB resources, is auto-generated and available in the service folder. The terraform init and apply commands created all resources based on data extracted from Kubernetes service and deployments.
-
 To clean up, assuming you are in `specctl` directory
 ```bash
 cd output/default/nginx-svc
 terraform destroy --auto-approve
 cd ../../namespaces
 terraform destroy --auto-approve
 cd ../..
 rm -rf output
 ```
-
 ### Conversions at scale from a cluster
 `specctl` is built with scalable migration in mind. For the Kubernetes to ECS migration, for example, every service has its Terraform code and extracted settings in a seprate folder. By adding a CI/CD pipeline and S3 bucket (for Terraform state), the deployment of ECS services can be completely automated for all the services. The Terraform infra-as-code approach makes it easy to extend and customize to meet customer's application needs. 
 
-To test conversion at scale for Kubernetes to ECS, we can use the `tests/retail-store` example. Start by creating this application in Kubernetes. You can use `minikube`if you don't have a Kubernetes cluster handy. There is a convenience script `specctl/bin/migrate.sh` to recursively apply `terraform init` and `terraform apply --auto-approve` in each of the service directories. 
+To test conversion at scale for Kubernetes to ECS, we can use the `tests/retail-store` example. Start by creating this application in Kubernetes. You can use `minikube`if you don't have a Kubernetes cluster handy. 
 
-Assuming you are in `specctl` directory.
+Assuming you are in `specctl` directory and you have cleaned up the previous example `./output` directory.
 ```bash
 kubectl apply -f tests/retail-store
 ...
 ... (wait for apply to finish)
 ...
 ```
 ```bash
@@ -98,15 +102,17 @@
 ...
 cd output
 cd namespaces
 terraform init && terraform apply --auto-approve
 ...
 ...
 ```
-The above will create all the shared resources in various namespaces that are extracted. Shared resources include SSM Parameters, ALBs, CloudMap namespaces. Now you can run the `migrate.sh` script from the `/output` folder to recursively create all the extracted services. Below is assuming your are in `namespaces` folder from above step.
+The above will create all the shared resources in various namespaces that are extracted. Shared resources include SSM Parameters, ALBs, CloudMap namespaces. 
+
+There is a convenience script `specctl/bin/migrate.sh` to recursively apply `terraform init` and `terraform apply --auto-approve` in each of the service directories. Below is assuming your are in `namespaces` folder from above step. 
 
 ```bash
 cd ..
 source ../bin/migrate.sh apply
 ```
 You should see a lot of services created in ECS - `ui`,`carts`, `catalog` ... The `ui` service is load balanced and if you access the ALB URL you will see the same home page as when you access the `ui` service in Kubernetes. Play around with the app and make sure all the inter-service communication is working in both ECS and Kubernetes!
 **Congrats, you have just migrated 7 services in matter of minutes!** And same approach can be adapted to do scalable migrations.
@@ -122,43 +128,44 @@
 mv ../namespaces .
 cd namespaces
 terraform destroy --auto-approve
 cd ../..
 rm -rf output
 ```
 #### What all K8s objects does specctl convert to ECS? 
-- [X] Deployment
+- [X] Deployment and ReplicaSets
 - [X] Service including ClusterIP, Load Balancer
-- [X] Ingress with HTTP 
+- [X] Ingress with HTTP and HTTPS (AWS ALB only)
 - [X] Pod IAM via Service Account
 - [X] ConfigMaps
 - [X] Secrets
-- [X] Container specs along with init-containers, and named ports handling
+- [X] Container specs along with init-containers, and named port handling
 - [X] Fargate size determination based on cpu and mem reservation and limit
-- [X] Ingress with HTTPS esp. certificate handling
 - [X] Pod Security Group
+- [ ] DaemonSets
 - [ ] Jobs
 - [ ] Container volumes
+- [ ] StatefulSets
 - [ ] ?
 
-**Note** K8s allows multiple variations for the service discovery, for example, `svc-name` or `svc-name.namespace` or `svc-name.namespace.svc.cluster.local`. But in ECS the service discovery name is `svc-name.namespace` (where namespace is in CloudMap). You may need to do some manual changes to the service endpoints configurations if they are not able to discover each other. This concern applies to both ECS to K8s and K8s to ECS conversions. 
+**Note:** Kubernetes allows multiple variations for the service discovery, for example, `svc-name` or `svc-name.namespace` or `svc-name.namespace.svc.cluster.local`. But in ECS the service discovery name is `svc-name.namespace` (where namespace is in CloudMap). You may need to do some manual changes to the service endpoints configurations if they are not able to discover each other. This concern applies to both ECS to K8s and K8s to ECS conversions. 
 
 ### ECS to Kubernetes 
 To do the reverse simply run the below command and it will generate the Kubernetes deployment, service, configmap, and secrets YAML specification files. Note to change the cluster name and/or region name if you created ECS cluster in a different region or are using your own ECS cluster in a different region. You can create Kubernetes namespace and deploy the generated artifacts to test. 
 
 ```bash
 specctl -m e2k --ecs_region_name us-west-2 --ecs_cluster_name core-infra
 ls output/core-infra
 ```
 #### What all ECS objects does specctl convert to Kubernetes?
 - [X] ECS Task to Pod
 - [X] ECS Service to K8s Service & K8s Deployment  
 - [X] ECS Load Balanced Service to K8s Ingress
-- [X] SSP Parameter Simple Strings to K8s ConfigMap 
-- [X] SSP Parameter SecureString to K8s Secrets
+- [X] SSM Parameter Simple Strings to K8s ConfigMap 
+- [X] SSM Parameter SecureString to K8s Secrets
 - [X] Secrets Manager to K8s Secrets
 - [X] Task IAM to IAM annotations on Service Account
 - [X] Task Security Group to EKS Security Group Policy 
 - [X] First "." delimiter of CloudMap namespace to K8s namespace 
 
 ### Features of `specctl`
 ```bash
@@ -189,25 +196,25 @@
   -o, --output_directory TEXT     Path to output directory
   --ecs_cluster_name TEXT         ECS cluster to extract services and tasks
   --ecs_region_name TEXT          Region name for ECS cluster
   --sgp                           Create EKS Security Group Policy from task
                                   security groups
   --help                          Show this message and exit.
 ```
-* `specctl` currenly reads and extracts information from Kubernetes `Deployment`,`Service`, `ConfigMap`, and `Secrets` objects. It can read these objects from a file/folder or directly from a Kubernetes cluster.
+* `specctl` can read Kubernetes objects from a file/folder or directly from a Kubernetes cluster.
 * If `-s` source path to the K8s YAML file or directory is provided, `specctl` will use those specification files to read and extract information to create `taskdefinition.json`, `servicedefinition.json`, and `terraform.tfvars` files.
 * If `-c`, cluster kubeconfig context is provided, then `specctl` will read the deployments, services, configmaps, secrets directly from K8s cluster and generate the output files.
 * If both `-s` and `-c` are provided then behavior is same as just `-s`, that is, to process file(s) at that source path.
 * If neither `-s` and `-c` are provided then `specctl` will load all the contexts from kubeconfig and prompt the user to pick one.
 * The `-l` option is to control logging. Default log level is `INFO`.
 * The `--td_file` refers to JSON file for task definition and is set to `taskdefinition.json`. The actual output file is of the format `<output_directory>/<service_namespace>/<service_name>/taskdefinition.json`
 * The `--sd_file` refers to JSON file for service definition and is set to `servicedefinition.json`. The actual output file is of the format `<output_directory>/<service_namespace>/<service_name>/taskdefinition.json`
-* The `--input_file` is to provide additional input to add or update the parsed input in task definition and service definition JSON output. See sample [input.json](./lb_service_input.json.example) files for content format.
+* The `--input_file` is to provide additional input to add or update the parsed input in task definition and service definition JSON output. 
 * The `--tfvars_file` is to provide the terraform tfvars output and set to `terraform.tfvars`. The actual output is of the form `<output_directory>/terraform.tfvars` and `<output_directory>/<service_namespace>/<service_name>/terraform.fvars`.
 * The `-d` options is to provide the path to Terraform modules directory. Default is "./terraform" from where the specctl command is launched.
 * The `--tf_modules_name_map` is to provide a map of what are the folder names for the `namespaces`, `ecs-lb-service`, and `ecs-backend-service` modules. Default is `"namespaces:namespaces,ecs-lb-service:ecs-lb-service,ecs-backend-service:ecs-backend-service"`. Keep the keys same and change module folder name as applicable. The module folders should be under the Terraform modules directory provided by `-d` option.
 * The `--tf_files` is to provide a comma separated string of Terraform files to copy from the modules. Default is `"main.tf,versions.tf,variables.tf,outputs.tf"`
 * The `-o` is the path to output directory. Default is `./output`.
-* The `--ecs_cluster_name` is to provide name of ECS cluster to extract services and tasks to conver to Kubernetes specifications
+* The `--ecs_cluster_name` is to provide name of ECS cluster to extract services and tasks to convert to Kubernetes specifications
 * The `--ecs_region_name` is to provide region name for ECS cluster
 * The `--sgp` flag is to control whether or not to create EKS security group policies based on ECS task security groups. By default specctl doesn't create the security group policies because pod networking can be quite different.
```

