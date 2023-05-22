# Comparing `tmp/pulumi_terraform-5.8.0a1675048832.tar.gz` & `tmp/pulumi_terraform-5.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pulumi_terraform-5.8.0a1675048832.tar", last modified: Mon Jan 30 03:24:42 2023, max compression
+gzip compressed data, was "dist/pulumi_terraform-5.9.0.tar", last modified: Fri Mar  3 20:13:38 2023, max compression
```

## Comparing `pulumi_terraform-5.8.0a1675048832.tar` & `pulumi_terraform-5.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform/state/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform/state/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44832 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform/state/remote_state_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/pulumi_terraform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-01-30 03:24:42.000000 pulumi_terraform-5.8.0a1675048832/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-03-03 20:13:37.000000 pulumi_terraform-5.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/pulumi_terraform/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-03 20:13:37.000000 pulumi_terraform-5.9.0/pulumi_terraform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/pulumi_terraform/state/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-03 20:13:37.000000 pulumi_terraform-5.9.0/pulumi_terraform/state/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44832 2023-03-03 20:13:37.000000 pulumi_terraform-5.9.0/pulumi_terraform/state/remote_state_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/pulumi_terraform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/pulumi_terraform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/pulumi_terraform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/pulumi_terraform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/pulumi_terraform.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/pulumi_terraform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/pulumi_terraform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-03 20:13:38.000000 pulumi_terraform-5.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-03 20:13:37.000000 pulumi_terraform-5.9.0/setup.py
```

### Comparing `pulumi_terraform-5.8.0a1675048832/PKG-INFO` & `pulumi_terraform-5.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_terraform
-Version: 5.8.0a1675048832
+Version: 5.9.0
 Summary: A Pulumi package for consuming Terraform Remote State resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-terraform
 Description: # Pulumi Terraform Provider
         
         The Terraform resource provider for Pulumi lets you consume the outputs
```

### Comparing `pulumi_terraform-5.8.0a1675048832/README.md` & `pulumi_terraform-5.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_terraform-5.8.0a1675048832/pulumi_terraform/state/remote_state_reference.py` & `pulumi_terraform-5.9.0/pulumi_terraform/state/remote_state_reference.py`

 * *Files identical despite different names*

### Comparing `pulumi_terraform-5.8.0a1675048832/pulumi_terraform.egg-info/PKG-INFO` & `pulumi_terraform-5.9.0/pulumi_terraform.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-terraform
-Version: 5.8.0a1675048832
+Version: 5.9.0
 Summary: A Pulumi package for consuming Terraform Remote State resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-terraform
 Description: # Pulumi Terraform Provider
         
         The Terraform resource provider for Pulumi lets you consume the outputs
```

### Comparing `pulumi_terraform-5.8.0a1675048832/setup.py` & `pulumi_terraform-5.9.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 import errno
 
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'terraform', '5.8.0-alpha.1675048832+792ae89c'])
+            check_call(['pulumi', 'plugin', 'install', 'resource', 'terraform', '5.9.0'])
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print("""
                 There was an error installing the terraform resource provider plugin. It looks
                 like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com to install the Pulumi CLI.
                 You may try manually installin the plugin by running:
-                `pulumi plugin install resource terraform 5.8.0-alpha.1675048832+792ae89c`
+                `pulumi plugin install resource terraform 5.9.0`
                 """)
 
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(name='pulumi_terraform',
-      version='5.8.0a1675048832',
+      version='5.9.0',
       description='A Pulumi package for consuming Terraform Remote State resources.',
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
       keywords='pulumi terraform',
```

