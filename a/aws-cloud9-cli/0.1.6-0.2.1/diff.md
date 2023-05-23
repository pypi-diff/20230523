# Comparing `tmp/aws-cloud9-cli-0.1.6.tar.gz` & `tmp/aws-cloud9-cli-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cloud9-cli-0.1.6.tar", last modified: Fri Apr  7 11:26:33 2023, max compression
+gzip compressed data, was "aws-cloud9-cli-0.2.1.tar", last modified: Tue May 23 08:14:17 2023, max compression
```

## Comparing `aws-cloud9-cli-0.1.6.tar` & `aws-cloud9-cli-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:26:33.533446 aws-cloud9-cli-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 11:26:15.000000 aws-cloud9-cli-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-07 11:26:33.533446 aws-cloud9-cli-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-07 11:26:15.000000 aws-cloud9-cli-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:26:33.529446 aws-cloud9-cli-0.1.6/aws_cloud9_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-07 11:26:33.000000 aws-cloud9-cli-0.1.6/aws_cloud9_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-07 11:26:33.000000 aws-cloud9-cli-0.1.6/aws_cloud9_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-07 11:26:33.000000 aws-cloud9-cli-0.1.6/aws_cloud9_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-07 11:26:33.000000 aws-cloud9-cli-0.1.6/aws_cloud9_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-07 11:26:33.000000 aws-cloud9-cli-0.1.6/aws_cloud9_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-07 11:26:33.000000 aws-cloud9-cli-0.1.6/aws_cloud9_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-07 11:26:33.533446 aws-cloud9-cli-0.1.6/cloud9_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-07 11:26:15.000000 aws-cloud9-cli-0.1.6/cloud9_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-04-07 11:26:15.000000 aws-cloud9-cli-0.1.6/cloud9_cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-04-07 11:26:15.000000 aws-cloud9-cli-0.1.6/cloud9_cli/create_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-07 11:26:15.000000 aws-cloud9-cli-0.1.6/cloud9_cli/deploy_cfn.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-07 11:26:15.000000 aws-cloud9-cli-0.1.6/cloud9_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-07 11:26:15.000000 aws-cloud9-cli-0.1.6/cloud9_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-07 11:26:15.000000 aws-cloud9-cli-0.1.6/cloud9_cli/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-07 11:26:33.533446 aws-cloud9-cli-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-07 11:26:15.000000 aws-cloud9-cli-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:14:17.825088 aws-cloud9-cli-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 08:13:58.000000 aws-cloud9-cli-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 08:14:17.825088 aws-cloud9-cli-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-23 08:13:58.000000 aws-cloud9-cli-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:14:17.825088 aws-cloud9-cli-0.2.1/aws_cloud9_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-23 08:14:17.000000 aws-cloud9-cli-0.2.1/aws_cloud9_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-23 08:14:17.000000 aws-cloud9-cli-0.2.1/aws_cloud9_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:14:17.000000 aws-cloud9-cli-0.2.1/aws_cloud9_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-23 08:14:17.000000 aws-cloud9-cli-0.2.1/aws_cloud9_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 08:14:17.000000 aws-cloud9-cli-0.2.1/aws_cloud9_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 08:14:17.000000 aws-cloud9-cli-0.2.1/aws_cloud9_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:14:17.825088 aws-cloud9-cli-0.2.1/cloud9_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 08:13:58.000000 aws-cloud9-cli-0.2.1/cloud9_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-05-23 08:13:58.000000 aws-cloud9-cli-0.2.1/cloud9_cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-05-23 08:13:58.000000 aws-cloud9-cli-0.2.1/cloud9_cli/create_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-05-23 08:13:58.000000 aws-cloud9-cli-0.2.1/cloud9_cli/deploy_cfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-23 08:13:58.000000 aws-cloud9-cli-0.2.1/cloud9_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-23 08:13:58.000000 aws-cloud9-cli-0.2.1/cloud9_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-23 08:13:58.000000 aws-cloud9-cli-0.2.1/cloud9_cli/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-23 08:14:17.825088 aws-cloud9-cli-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 08:13:58.000000 aws-cloud9-cli-0.2.1/setup.py
```

### Comparing `aws-cloud9-cli-0.1.6/LICENSE` & `aws-cloud9-cli-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cloud9-cli-0.1.6/README.md` & `aws-cloud9-cli-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aws-cloud9-cli-0.1.6/cloud9_cli/create_yaml.py` & `aws-cloud9-cli-0.2.1/cloud9_cli/create_yaml.py`

 * *Files identical despite different names*

### Comparing `aws-cloud9-cli-0.1.6/cloud9_cli/deploy_cfn.py` & `aws-cloud9-cli-0.2.1/cloud9_cli/deploy_cfn.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,37 @@
 import boto3
 from botocore.config import Config
 from inquirer import prompt, Confirm, Text
 from prettytable import PrettyTable
 from cfn_visualizer import visualizer
 
 from cloud9_cli.validators import stack_name_validator
+from cloud9_cli.utils import bright_cyan, bright_green, bright_red
 
 
 class DeployCfn:
     client = None
     deploy = False
     name = ''
     region = ''
     project = ''
 
     def __init__(
             self,
             region,
             project,
+            profile
     ):
         self.region = region
         self.project = project
+        self.profile = profile
         self.ask_deployment()
         self.input_stack_name()
         self.create_iam_roles()
-        self.deployment(self.name, region)
+        self.deployment(self.name, region, profile)
 
     def ask_deployment(self):
         questions = [
             Confirm(
                 name='required',
                 message='Do you want to deploy using CloudFormation in here?',
                 default=True
@@ -39,15 +42,15 @@
         self.deploy = prompt(questions=questions, raise_keyboard_interrupt=True)['required']
 
     def input_stack_name(self):
         questions = [
             Text(
                 name='name',
                 message='Type CloudFormation Stack name',
-                validate=lambda _, x: stack_name_validator(x, self.region),
+                validate=lambda _, x: stack_name_validator(x, self.region, self.profile),
             )
         ]
 
         self.name = prompt(questions=questions, raise_keyboard_interrupt=True)['name']
 
     def create_iam_roles(self):
         print('Create the Cloud9 SSM role...')
@@ -104,17 +107,17 @@
             client.add_role_to_instance_profile(
                 InstanceProfileName='AWSCloud9SSMInstanceProfile',
                 RoleName='AWSCloud9SSMAccessRole',
             )
         except client.exceptions.LimitExceededException:
             pass
 
-    def deployment(self, name, region):
+    def deployment(self, name, region, profile='default'):
         if self.deploy:  # deploy using cloudformation
-            self.client = boto3.client('cloudformation', config=Config(region_name=region))
+            self.client = boto3.session.Session(profile_name=profile, region_name=region).client('cloudformation')
             response = self.client.create_stack(
                 StackName=name,
                 TemplateBody=self.get_template(),
                 TimeoutInMinutes=15,
                 Capabilities=['CAPABILITY_NAMED_IAM'],
                 Tags=[{'Key': 'Name', 'Value': name}, {'Key': 'project', 'Value': self.project}],
             )
@@ -126,37 +129,35 @@
                     StackName=name
                 )
                 stack_status = response['Stacks'][0]['StackStatus']
 
                 if stack_status in ['CREATE_FAILED', 'ROLLBACK_FAILED',
                                     'ROLLBACK_COMPLETE']:  # create failed
                     print()
-                    print('\x1b[31m' + 'Failed!' + '\x1b[0m')
+                    print(f'{bright_red("Failed!")}')
                     print()
-                    print('\x1b[31m' + 'Please check CloudFormation at here:' + '\x1b[0m')
+                    print(f'{bright_red("Please check CloudFormation at here:")}')
                     print()
                     print(
-                        '\x1b[31m' +
-                        'https://{0}.console.aws.amazon.com/cloudformation/home?region={0}#/stacks/stackinfo?stackId={1}'.format(
-                            region, stack_id) +
-                        '\x1b[0m')
+                        f'{bright_red(f"https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacks/stackinfo?stackId={stack_id}")}')
+
                     break
 
                 elif stack_status == 'CREATE_COMPLETE':  # create complete successful
                     print()
                     self.print_table()
-                    print('\x1b[32m' + 'Success!' + '\x1b[0m')
+                    print(f'{bright_green("Success!")}')
                     print()
-                    print('\x1b[32m' + 'You can access IDE in here:' + '\x1b[0m')
+                    print(f'{bright_green("You can access IDE in here:")}')
                     print()
                     url = next((item['OutputValue'] for item in
                                 boto3.client('cloudformation', config=Config(region_name=region)).describe_stacks(
                                     StackName=name)['Stacks'][0]['Outputs'] if item['OutputKey'] == 'EnvironmentUrl'),
                                False)
-                    print('\x1b[32m' + url + '\x1b[0m')
+                    print(f'{bright_green(url)}')
 
                     break
 
                 else:
                     visualizer(self.client, self.name)
 
         else:
```

### Comparing `aws-cloud9-cli-0.1.6/setup.py` & `aws-cloud9-cli-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup, find_packages
 
 requires = [
-    'ansicon==1.89.0',
-    'aws-cloudformation-visualizer==0.0.2',
-    'blessed==1.20.0',
-    'boto3==1.26.104',
-    'botocore==1.29.104',
-    'inquirer==3.1.3',
-    'jinxed==1.2.0',
-    'jmespath==1.0.1',
-    'prettytable==3.6.0',
-    'pyfiglet==0.8.post1',
-    'python-dateutil==2.8.2',
-    'python-editor==1.0.4',
-    'PyYAML==6.0',
-    'readchar==4.0.3',
-    's3transfer==0.6.0',
-    'six==1.16.0',
-    'urllib3==1.26.14',
-    'wcwidth==0.2.6',
+    'ansicon>=1.89.0',
+    'aws-cloudformation-visualizer>=0.0.4',
+    'blessed>=1.20.0',
+    'boto3>=1.26.104',
+    'botocore>=1.29.104',
+    'inquirer>=3.1.3',
+    'jinxed>=1.2.0',
+    'jmespath>=1.0.1',
+    'prettytable>=3.6.0',
+    'pyfiglet>=0.8.post1',
+    'python-dateutil>=2.8.2',
+    'python-editor>=1.0.4',
+    'PyYAML>=6.0',
+    'readchar==4.0.5',
+    's3transfer>=0.6.0',
+    'six>=1.16.0',
+    'urllib3>=1.26.14',
+    'wcwidth>=0.2.6',
 ]
 
 setup(
     name='aws-cloud9-cli',
-    version='0.1.6',
+    version='0.2.1',
     author='marcus16-kang',
     description='AWS Cloud9 Environment Stack Generator',
     author_email='marcus16-kang@outlook.com',
     license='MIT',
     entry_points={
         'console_scripts': [
             'c9-cli=cloud9_cli.main:main'
```

