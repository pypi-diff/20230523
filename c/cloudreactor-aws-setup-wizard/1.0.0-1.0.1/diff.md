# Comparing `tmp/cloudreactor_aws_setup_wizard-1.0.0.tar.gz` & `tmp/cloudreactor_aws_setup_wizard-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudreactor_aws_setup_wizard-1.0.0.tar", max compression
+gzip compressed data, was "cloudreactor_aws_setup_wizard-1.0.1.tar", max compression
```

## Comparing `cloudreactor_aws_setup_wizard-1.0.0.tar` & `cloudreactor_aws_setup_wizard-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1322 2020-09-13 22:46:39.873757 cloudreactor_aws_setup_wizard-1.0.0/LICENSE
--rw-r--r--   0        0        0     4272 2023-05-22 00:52:12.822697 cloudreactor_aws_setup_wizard-1.0.0/README.md
--rw-r--r--   0        0        0       64 2023-05-10 07:17:17.951124 cloudreactor_aws_setup_wizard-1.0.0/cloudreactor_aws_setup_wizard/__init__.py
--rw-r--r--   0        0        0     3248 2023-05-21 01:57:51.915251 cloudreactor_aws_setup_wizard-1.0.0/cloudreactor_aws_setup_wizard/__main__.py
--rw-r--r--   0        0        0     4831 2023-05-20 09:14:43.101924 cloudreactor_aws_setup_wizard-1.0.0/cloudreactor_aws_setup_wizard/cloudreactor_api_client.py
--rw-r--r--   0        0        0        0 2023-05-10 08:39:30.567796 cloudreactor_aws_setup_wizard-1.0.0/cloudreactor_aws_setup_wizard/py.typed
--rw-r--r--   0        0        0    15822 2023-05-21 01:27:20.119487 cloudreactor_aws_setup_wizard-1.0.0/cloudreactor_aws_setup_wizard/templates/vpc.yml.j2
--rw-r--r--   0        0        0    90595 2023-05-21 01:34:52.459046 cloudreactor_aws_setup_wizard-1.0.0/cloudreactor_aws_setup_wizard/wizard.py
--rw-r--r--   0        0        0     2283 2023-05-22 04:13:41.238072 cloudreactor_aws_setup_wizard-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5436 1970-01-01 00:00:00.000000 cloudreactor_aws_setup_wizard-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1322 2020-09-13 22:46:39.873757 cloudreactor_aws_setup_wizard-1.0.1/LICENSE
+-rw-r--r--   0        0        0     4327 2023-05-22 04:16:40.780255 cloudreactor_aws_setup_wizard-1.0.1/README.md
+-rw-r--r--   0        0        0       64 2023-05-23 08:03:53.789257 cloudreactor_aws_setup_wizard-1.0.1/cloudreactor_aws_setup_wizard/__init__.py
+-rw-r--r--   0        0        0     3248 2023-05-21 01:57:51.915251 cloudreactor_aws_setup_wizard-1.0.1/cloudreactor_aws_setup_wizard/__main__.py
+-rw-r--r--   0        0        0     4831 2023-05-20 09:14:43.101924 cloudreactor_aws_setup_wizard-1.0.1/cloudreactor_aws_setup_wizard/cloudreactor_api_client.py
+-rw-r--r--   0        0        0        0 2023-05-10 08:39:30.567796 cloudreactor_aws_setup_wizard-1.0.1/cloudreactor_aws_setup_wizard/py.typed
+-rw-r--r--   0        0        0    15822 2023-05-21 01:27:20.119487 cloudreactor_aws_setup_wizard-1.0.1/cloudreactor_aws_setup_wizard/templates/vpc.yml.j2
+-rw-r--r--   0        0        0    90606 2023-05-23 08:03:00.116756 cloudreactor_aws_setup_wizard-1.0.1/cloudreactor_aws_setup_wizard/wizard.py
+-rw-r--r--   0        0        0     2309 2023-05-23 08:03:53.789257 cloudreactor_aws_setup_wizard-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5491 1970-01-01 00:00:00.000000 cloudreactor_aws_setup_wizard-1.0.1/PKG-INFO
```

### Comparing `cloudreactor_aws_setup_wizard-1.0.0/LICENSE` & `cloudreactor_aws_setup_wizard-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudreactor_aws_setup_wizard-1.0.0/README.md` & `cloudreactor_aws_setup_wizard-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,18 @@
 
 First install native python 3.11.x or above. Then clone this repo.
 In a terminal window, navigate to the repo. Then:
 
     pip install -r requirements.txt
     python -m cloudreactor_aws_setup_wizard
 
+Or with pipx:
+
+    pipx cloudreactor_aws_setup_wizard
+
 ## Permissions required / granting access
 
 So that this wizard can create AWS resources for you, it needs the following
 permissions:
 
 * Upload CloudFormation stacks
 * Create IAM Roles
```

#### html2text {}

```diff
@@ -12,18 +12,19 @@
 daemon. Next, create a directory somewhere that the wizard can use to save your
 settings, between runs. For example, mkdir -p saved_state Finally run the
 image: docker run --rm -it -v $PWD/saved_state:/usr/app/saved_state
 cloudreactor/aws-setup-wizard which will use the saved_state subdirectory of
 the current directory to save settings. ### Without Docker (native execution)
 First install native python 3.11.x or above. Then clone this repo. In a
 terminal window, navigate to the repo. Then: pip install -r requirements.txt
-python -m cloudreactor_aws_setup_wizard ## Permissions required / granting
-access So that this wizard can create AWS resources for you, it needs the
-following permissions: * Upload CloudFormation stacks * Create IAM Roles * List
-ECS clusters, VPCs, subnets, NAT gateways, Elastic IPs, and security groups *
+python -m cloudreactor_aws_setup_wizard Or with pipx: pipx
+cloudreactor_aws_setup_wizard ## Permissions required / granting access So that
+this wizard can create AWS resources for you, it needs the following
+permissions: * Upload CloudFormation stacks * Create IAM Roles * List ECS
+clusters, VPCs, subnets, NAT gateways, Elastic IPs, and security groups *
 Create ECS clusters (if using the wizard to create an ECS cluster) * Create
 VPCs, subnets, internet gateways, NAT gateways, route tables, route table
 associations, VPC endpoints, and security groups (if using the wizard to create
 a VPC) You can give the wizard these permissions in a few different ways: 1) An
 access key and access secret that you manually enter when prompted by the
 wizard 2) Passing the access key and the secret key in the environment
 variables `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` respectively when you
```

### Comparing `cloudreactor_aws_setup_wizard-1.0.0/cloudreactor_aws_setup_wizard/__main__.py` & `cloudreactor_aws_setup_wizard-1.0.1/cloudreactor_aws_setup_wizard/__main__.py`

 * *Files identical despite different names*

### Comparing `cloudreactor_aws_setup_wizard-1.0.0/cloudreactor_aws_setup_wizard/cloudreactor_api_client.py` & `cloudreactor_aws_setup_wizard-1.0.1/cloudreactor_aws_setup_wizard/cloudreactor_api_client.py`

 * *Files identical despite different names*

### Comparing `cloudreactor_aws_setup_wizard-1.0.0/cloudreactor_aws_setup_wizard/templates/vpc.yml.j2` & `cloudreactor_aws_setup_wizard-1.0.1/cloudreactor_aws_setup_wizard/templates/vpc.yml.j2`

 * *Files identical despite different names*

### Comparing `cloudreactor_aws_setup_wizard-1.0.0/cloudreactor_aws_setup_wizard/wizard.py` & `cloudreactor_aws_setup_wizard-1.0.1/cloudreactor_aws_setup_wizard/wizard.py`

 * *Files 0% similar despite different names*

```diff
@@ -2476,15 +2476,15 @@
         )
 
         for stack in existing_stacks:
             print(f"{stack['name']}: {stack['status']}")
 
         return existing_stacks
 
-    def list_vpcs(self, ec2_client) -> Optional[list[str]]:
+    def list_vpcs(self, ec2_client) -> Optional[list[dict[str, Any]]]:
         print(f"Looking for existing VPCs in region {self.aws_region} ...")
 
         resp = None
         try:
             resp = ec2_client.describe_vpcs(MaxResults=100)
         except Exception as ex:
             logging.warning(f"Failed to list VPCs: {ex}")
```

### Comparing `cloudreactor_aws_setup_wizard-1.0.0/pyproject.toml` & `cloudreactor_aws_setup_wizard-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cloudreactor-aws-setup-wizard"
-version = "1.0.0"
+version = "1.0.1"
 description = "A command-line wizard to setup customer environments for running tasks managed by CloudReactor"
 authors = [
     "Jeff Tsay <jeff@cloudreactor.io>"
 ]
 license = "BSD-2-Clause"
 readme = "README.md"
 repository = "https://github.com/CloudReactor/cloudreactor-aws-setup-wizard"
@@ -32,38 +32,38 @@
 boto3 = "^1.26.137"
 questionary = "^1.10.0"
 jsonpickle = "^1.5.2"
 urllib3 = "^1.26.15"
 jinja2 = "^3.1.2"
 pyyaml = "^6.0"
 
-[tool.poetry.scripts]
-wizard = "cloudreactor_aws_setup_wizard.wizard:run"
-
 # Documentation Dependencies
 #Sphinx = {version = "^3.5.4", optional = true}
 #sphinx-rtd-theme = {version = "^1.0.0", optional = true}
 #myst-parser = {version = "^0.17.2", optional = true}
 # Jinja 3.1.0 breaks this version of Sphinx
 # https://github.com/apache/flink/pull/19238
 #Jinja2 = {version = "3.0.3"}
-types-PyYAML = "6.0.12.9"
+
+[tool.poetry.scripts]
+cloudreactor_aws_setup_wizard = "cloudreactor_aws_setup_wizard.__main__:run"
 
 #[tool.poetry.extras]
 #docs = [
 #    "myst-parser",
 #    "sphinx",
 #    "sphinx-rtd-theme",
 #]
 
 [tool.poetry.dev-dependencies]
 flake8 = "^4.0.1"
 isort = "^5.10.1"
-mypy = "^0.982"
+mypy = "^1.3.0"
 pip-audit = "^2.5.5"
+types-PyYAML = "6.0.12.10"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 branch = "main"
```

### Comparing `cloudreactor_aws_setup_wizard-1.0.0/PKG-INFO` & `cloudreactor_aws_setup_wizard-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudreactor-aws-setup-wizard
-Version: 1.0.0
+Version: 1.0.1
 Summary: A command-line wizard to setup customer environments for running tasks managed by CloudReactor
 Home-page: https://cloudreactor.io
 License: BSD-2-Clause
 Author: Jeff Tsay
 Author-email: jeff@cloudreactor.io
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -76,14 +76,18 @@
 
 First install native python 3.11.x or above. Then clone this repo.
 In a terminal window, navigate to the repo. Then:
 
     pip install -r requirements.txt
     python -m cloudreactor_aws_setup_wizard
 
+Or with pipx:
+
+    pipx cloudreactor_aws_setup_wizard
+
 ## Permissions required / granting access
 
 So that this wizard can create AWS resources for you, it needs the following
 permissions:
 
 * Upload CloudFormation stacks
 * Create IAM Roles
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cloudreactor-aws-setup-wizard Version: 1.0.0
+Metadata-Version: 2.1 Name: cloudreactor-aws-setup-wizard Version: 1.0.1
 Summary: A command-line wizard to setup customer environments for running tasks
 managed by CloudReactor Home-page: https://cloudreactor.io License: BSD-2-
 Clause Author: Jeff Tsay Author-email: jeff@cloudreactor.io Requires-Python:
 >=3.11,<4.0 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
@@ -27,18 +27,19 @@
 daemon. Next, create a directory somewhere that the wizard can use to save your
 settings, between runs. For example, mkdir -p saved_state Finally run the
 image: docker run --rm -it -v $PWD/saved_state:/usr/app/saved_state
 cloudreactor/aws-setup-wizard which will use the saved_state subdirectory of
 the current directory to save settings. ### Without Docker (native execution)
 First install native python 3.11.x or above. Then clone this repo. In a
 terminal window, navigate to the repo. Then: pip install -r requirements.txt
-python -m cloudreactor_aws_setup_wizard ## Permissions required / granting
-access So that this wizard can create AWS resources for you, it needs the
-following permissions: * Upload CloudFormation stacks * Create IAM Roles * List
-ECS clusters, VPCs, subnets, NAT gateways, Elastic IPs, and security groups *
+python -m cloudreactor_aws_setup_wizard Or with pipx: pipx
+cloudreactor_aws_setup_wizard ## Permissions required / granting access So that
+this wizard can create AWS resources for you, it needs the following
+permissions: * Upload CloudFormation stacks * Create IAM Roles * List ECS
+clusters, VPCs, subnets, NAT gateways, Elastic IPs, and security groups *
 Create ECS clusters (if using the wizard to create an ECS cluster) * Create
 VPCs, subnets, internet gateways, NAT gateways, route tables, route table
 associations, VPC endpoints, and security groups (if using the wizard to create
 a VPC) You can give the wizard these permissions in a few different ways: 1) An
 access key and access secret that you manually enter when prompted by the
 wizard 2) Passing the access key and the secret key in the environment
 variables `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` respectively when you
```

