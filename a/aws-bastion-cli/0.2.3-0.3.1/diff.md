# Comparing `tmp/aws-bastion-cli-0.2.3.tar.gz` & `tmp/aws-bastion-cli-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-bastion-cli-0.2.3.tar", last modified: Tue May  9 06:40:16 2023, max compression
+gzip compressed data, was "aws-bastion-cli-0.3.1.tar", last modified: Tue May 23 07:34:28 2023, max compression
```

## Comparing `aws-bastion-cli-0.2.3.tar` & `aws-bastion-cli-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:40:16.655913 aws-bastion-cli-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 06:40:16.655913 aws-bastion-cli-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:40:16.651914 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 06:40:16.000000 aws-bastion-cli-0.2.3/aws_bastion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 06:40:16.655913 aws-bastion-cli-0.2.3/bastion_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/create_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/deploy_cfn.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/bastion_cli/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-09 06:40:16.655913 aws-bastion-cli-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-09 06:39:58.000000 aws-bastion-cli-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:28.789281 aws-bastion-cli-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 07:34:28.789281 aws-bastion-cli-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:28.789281 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-23 07:34:28.000000 aws-bastion-cli-0.3.1/aws_bastion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 07:34:28.789281 aws-bastion-cli-0.3.1/bastion_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11131 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/create_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/deploy_cfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/bastion_cli/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-23 07:34:28.789281 aws-bastion-cli-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-23 07:34:13.000000 aws-bastion-cli-0.3.1/setup.py
```

### Comparing `aws-bastion-cli-0.2.3/LICENSE` & `aws-bastion-cli-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.3/README.md` & `aws-bastion-cli-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.3/bastion_cli/command.py` & `aws-bastion-cli-0.3.1/bastion_cli/command.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.3/bastion_cli/create_yaml.py` & `aws-bastion-cli-0.3.1/bastion_cli/create_yaml.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,26 @@
             }
         }
 
     def create_instance(self, subnet, instance_name, instance_type, port, new_key_name, key_name, password):
         self.resources['Instance'] = {
             'Type': 'AWS::EC2::Instance',
             'Properties': {
+                'BlockDeviceMappings': [
+                    {
+                        'DeviceName': '/dev/xvda',
+                        'Ebs': {
+                            'Encrypted': True,
+                            'Iops': 3000,
+                            'VolumeSize': 50,
+                            'VolumeType': 'gp3',
+                            # 'Throughput': 125
+                        }
+                    }
+                ],
                 'IamInstanceProfile': self.instance_profile,
                 'ImageId': self.ami,
                 'SecurityGroupIds': [
                     {
                         'Fn::GetAtt': 'SG.GroupId'
                     }
                 ],
@@ -260,14 +272,19 @@
                         'IP': {
                             'Ref': 'EIP'
                         }
                     }
                 ]
             }
         }
+        self.outputs['InstanceId'] = {
+            'Value': {
+                'Ref': 'Instance'
+            }
+        }
         self.outputs['SSHPassword'] = {}
 
         if new_key_name:
             key_name = new_key_name
 
         if key_name:
             self.outputs['SSHCommand']['Value']['Fn::Sub'][0] = \
```

### Comparing `aws-bastion-cli-0.2.3/bastion_cli/deploy_cfn.py` & `aws-bastion-cli-0.3.1/bastion_cli/deploy_cfn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import os
 import boto3
 from botocore.config import Config
 from inquirer import prompt, Confirm, Text
 from datetime import datetime
 from dateutil import tz
 from prettytable import PrettyTable
 from cfn_visualizer import visualizer
 
 from bastion_cli.validators import stack_name_validator
-from bastion_cli.utils import bright_green, bright_red
+from bastion_cli.utils import bright_green, bright_red, modify_instance_attributes
 
 
 class DeployCfn:
     client = None
     deploy = False
     name = ''
     region = ''
@@ -75,14 +74,15 @@
                     print(f'\n{bright_red("Failed!")}\n')
                     print(f'{bright_red("Please check CloudFormation at here:")}\n')
                     print(
                         f'{bright_red(f"https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacks/stackinfo?stackId={stack_id}")}\n')
                     break
 
                 elif stack_status == 'CREATE_COMPLETE':  # create complete successful
+                    modify_instance_attributes(self.get_instance_id(), region)
                     self.print_table()
                     self.create_key_pair()
                     print(bright_green('Success!'))
 
                     break
 
                 else:
@@ -118,27 +118,31 @@
             rows.append([resource['LogicalResourceId'], resource['PhysicalResourceId'], resource['ResourceType']])
 
         rows = sorted(rows, key=lambda x: (x[2], x[0]))
         table.add_rows(rows)
         print(table)
 
     def create_key_pair(self):
-        home_dir = os.path.expanduser('~')
-        key_location = (home_dir + '/Desktop') if os.path.exists(home_dir + '/Desktop') else home_dir
-
         response = self.client.describe_stacks(StackName=self.name)
         key_id = [item.get('OutputValue') for item in response['Stacks'][0]['Outputs'] if item['OutputKey'] == 'KeyId']
         key_name = [item.get('OutputValue') for item in response['Stacks'][0]['Outputs'] if
                     item['OutputKey'] == 'KeyName']
 
         if len(key_id):
             response = boto3.client('ssm', config=Config(region_name=self.region)).get_parameter(
                 Name='/ec2/keypair/{}'.format(key_id[0]),
                 WithDecryption=True
             )
             key_body = response['Parameter']['Value']
 
-            with open(f'{key_location}/{key_name[0]}.pem', 'w') as f:
+            with open(f'{key_name[0]}.pem', 'w') as f:
                 f.write(key_body)
 
         else:
             pass
+
+    def get_instance_id(self):
+        response = self.client.describe_stacks(StackName=self.name)
+        instance_id = [item.get('OutputValue') for item in response['Stacks'][0]['Outputs'] if
+                       item['OutputKey'] == 'InstanceId'][0]
+
+        return instance_id
```

### Comparing `aws-bastion-cli-0.2.3/bastion_cli/main.py` & `aws-bastion-cli-0.3.1/bastion_cli/main.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.3/bastion_cli/validators.py` & `aws-bastion-cli-0.3.1/bastion_cli/validators.py`

 * *Files identical despite different names*

### Comparing `aws-bastion-cli-0.2.3/setup.py` & `aws-bastion-cli-0.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 from setuptools import setup, find_packages
 
 requires = [
     'ansicon>=1.89.0',
-    'aws-cloudformation-visualizer>=0.0.2',
+    'aws-cloudformation-visualizer>=0.0.3',
     'blessed>=1.20.0',
     'boto3>=1.26.104',
     'botocore>=1.29.104',
     'inquirer>=3.1.3',
     'jinxed>=1.2.0',
     'jmespath>=1.0.1',
     'prettytable>=3.6.0',
     'pyfiglet>=0.8.post1',
     'python-dateutil>=2.8.2',
     'python-editor>=1.0.4',
     'PyYAML>=6.0',
-    'readchar==4.0.3',
+    'readchar==4.0.5',
     's3transfer>=0.6.0',
     'six>=1.16.0',
     'urllib3>=1.26.14',
     'wcwidth>=0.2.6',
 ]
 
 setup(
     name='aws-bastion-cli',
-    version='0.2.3',
+    version='0.3.1',
     author='marcus16-kang',
     description='AWS Bastion EC2 Server Stack Generator',
     author_email='marcus16-kang@outlook.com',
     license='MIT',
     entry_points={
         'console_scripts': [
             'bastion-cli=bastion_cli.main:main'
```

