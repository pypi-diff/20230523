# Comparing `tmp/pulumi_random-4.9.0a1673556316.tar.gz` & `tmp/pulumi_random-4.9.0a1674773801.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_random-4.9.0a1673556316.tar", last modified: Thu Jan 12 20:59:03 2023, max compression
+gzip compressed data, was "pulumi_random-4.9.0a1674773801.tar", last modified: Thu Jan 26 23:00:55 2023, max compression
```

## Comparing `pulumi_random-4.9.0a1673556316.tar` & `pulumi_random-4.9.0a1674773801.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:59:03.955911 pulumi_random-4.9.0a1673556316/
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-01-12 20:59:03.955911 pulumi_random-4.9.0a1673556316/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:59:03.955911 pulumi_random-4.9.0a1673556316/pulumi_random/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18668 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/random_id.py
--rw-r--r--   0 runner    (1001) docker     (123)    15761 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/random_integer.py
--rw-r--r--   0 runner    (1001) docker     (123)    31005 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/random_password.py
--rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/random_pet.py
--rw-r--r--   0 runner    (1001) docker     (123)    19028 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/random_shuffle.py
--rw-r--r--   0 runner    (1001) docker     (123)    31871 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/random_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     9486 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random/random_uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 20:59:03.955911 pulumi_random-4.9.0a1673556316/pulumi_random.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/pulumi_random.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 20:59:03.955911 pulumi_random-4.9.0a1673556316/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-01-12 20:59:03.000000 pulumi_random-4.9.0a1673556316/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 23:00:55.140885 pulumi_random-4.9.0a1674773801/
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-01-26 23:00:55.140885 pulumi_random-4.9.0a1674773801/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 23:00:55.136885 pulumi_random-4.9.0a1674773801/pulumi_random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18404 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/random_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/random_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37988 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/random_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/random_pet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16987 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/random_shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36985 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/random_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/pulumi_random/random_uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 23:00:55.136885 pulumi_random-4.9.0a1674773801/pulumi_random.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-01-26 23:00:55.000000 pulumi_random-4.9.0a1674773801/pulumi_random.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-01-26 23:00:55.000000 pulumi_random-4.9.0a1674773801/pulumi_random.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 23:00:55.000000 pulumi_random-4.9.0a1674773801/pulumi_random.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 23:00:55.000000 pulumi_random-4.9.0a1674773801/pulumi_random.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-01-26 23:00:55.000000 pulumi_random-4.9.0a1674773801/pulumi_random.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-01-26 23:00:55.000000 pulumi_random-4.9.0a1674773801/pulumi_random.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-26 23:00:55.140885 pulumi_random-4.9.0a1674773801/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-01-26 23:00:54.000000 pulumi_random-4.9.0a1674773801/setup.py
```

### Comparing `pulumi_random-4.9.0a1673556316/PKG-INFO` & `pulumi_random-4.9.0a1674773801/pulumi_random.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi_random
-Version: 4.9.0a1673556316
+Name: pulumi-random
+Version: 4.9.0a1674773801
 Summary: A Pulumi package to safely use randomness in Pulumi programs.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-random
 Keywords: pulumi random
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_random-4.9.0a1673556316/README.md` & `pulumi_random-4.9.0a1674773801/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random/__init__.py` & `pulumi_random-4.9.0a1674773801/pulumi_random/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random/_utilities.py` & `pulumi_random-4.9.0a1674773801/pulumi_random/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random/provider.py` & `pulumi_random-4.9.0a1674773801/pulumi_random/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random/random_id.py` & `pulumi_random-4.9.0a1674773801/pulumi_random/random_id.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,67 +11,57 @@
 
 __all__ = ['RandomIdArgs', 'RandomId']
 
 @pulumi.input_type
 class RandomIdArgs:
     def __init__(__self__, *,
                  byte_length: pulumi.Input[int],
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  prefix: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a RandomId resource.
-        :param pulumi.Input[int] byte_length: The number of random bytes to produce. The
-               minimum value is 1, which produces eight bits of randomness.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[str] prefix: Arbitrary string to prefix the output value with. This
-               string is supplied as-is, meaning it is not guaranteed to be URL-safe or
-               base64 encoded.
+        :param pulumi.Input[int] byte_length: The number of random bytes to produce. The minimum value is 1, which produces eight bits of randomness.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[str] prefix: Arbitrary string to prefix the output value with. This string is supplied as-is, meaning it is not guaranteed to be URL-safe or base64 encoded.
         """
         pulumi.set(__self__, "byte_length", byte_length)
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if prefix is not None:
             pulumi.set(__self__, "prefix", prefix)
 
     @property
     @pulumi.getter(name="byteLength")
     def byte_length(self) -> pulumi.Input[int]:
         """
-        The number of random bytes to produce. The
-        minimum value is 1, which produces eight bits of randomness.
+        The number of random bytes to produce. The minimum value is 1, which produces eight bits of randomness.
         """
         return pulumi.get(self, "byte_length")
 
     @byte_length.setter
     def byte_length(self, value: pulumi.Input[int]):
         pulumi.set(self, "byte_length", value)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        Arbitrary string to prefix the output value with. This
-        string is supplied as-is, meaning it is not guaranteed to be URL-safe or
-        base64 encoded.
+        Arbitrary string to prefix the output value with. This string is supplied as-is, meaning it is not guaranteed to be URL-safe or base64 encoded.
         """
         return pulumi.get(self, "prefix")
 
     @prefix.setter
     def prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "prefix", value)
 
@@ -80,30 +70,25 @@
 class _RandomIdState:
     def __init__(__self__, *,
                  b64_std: Optional[pulumi.Input[str]] = None,
                  b64_url: Optional[pulumi.Input[str]] = None,
                  byte_length: Optional[pulumi.Input[int]] = None,
                  dec: Optional[pulumi.Input[str]] = None,
                  hex: Optional[pulumi.Input[str]] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  prefix: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RandomId resources.
         :param pulumi.Input[str] b64_std: The generated id presented in base64 without additional transformations.
         :param pulumi.Input[str] b64_url: The generated id presented in base64, using the URL-friendly character set: case-sensitive letters, digits and the characters `_` and `-`.
-        :param pulumi.Input[int] byte_length: The number of random bytes to produce. The
-               minimum value is 1, which produces eight bits of randomness.
+        :param pulumi.Input[int] byte_length: The number of random bytes to produce. The minimum value is 1, which produces eight bits of randomness.
         :param pulumi.Input[str] dec: The generated id presented in non-padded decimal digits.
         :param pulumi.Input[str] hex: The generated id presented in padded hexadecimal digits. This result will always be twice as long as the requested byte length.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[str] prefix: Arbitrary string to prefix the output value with. This
-               string is supplied as-is, meaning it is not guaranteed to be URL-safe or
-               base64 encoded.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[str] prefix: Arbitrary string to prefix the output value with. This string is supplied as-is, meaning it is not guaranteed to be URL-safe or base64 encoded.
         """
         if b64_std is not None:
             pulumi.set(__self__, "b64_std", b64_std)
         if b64_url is not None:
             pulumi.set(__self__, "b64_url", b64_url)
         if byte_length is not None:
             pulumi.set(__self__, "byte_length", byte_length)
@@ -140,16 +125,15 @@
     def b64_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "b64_url", value)
 
     @property
     @pulumi.getter(name="byteLength")
     def byte_length(self) -> Optional[pulumi.Input[int]]:
         """
-        The number of random bytes to produce. The
-        minimum value is 1, which produces eight bits of randomness.
+        The number of random bytes to produce. The minimum value is 1, which produces eight bits of randomness.
         """
         return pulumi.get(self, "byte_length")
 
     @byte_length.setter
     def byte_length(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "byte_length", value)
 
@@ -175,48 +159,44 @@
 
     @hex.setter
     def hex(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "hex", value)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def prefix(self) -> Optional[pulumi.Input[str]]:
         """
-        Arbitrary string to prefix the output value with. This
-        string is supplied as-is, meaning it is not guaranteed to be URL-safe or
-        base64 encoded.
+        Arbitrary string to prefix the output value with. This string is supplied as-is, meaning it is not guaranteed to be URL-safe or base64 encoded.
         """
         return pulumi.get(self, "prefix")
 
     @prefix.setter
     def prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "prefix", value)
 
 
 class RandomId(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  byte_length: Optional[pulumi.Input[int]] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  prefix: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The resource `RandomId` generates random numbers that are intended to be
         used as unique identifiers for other resources.
 
         This resource *does* use a cryptographic random number generator in order
@@ -227,36 +207,31 @@
         This resource can be used in conjunction with resources that have
         the `create_before_destroy` lifecycle flag set to avoid conflicts with
         unique names during the brief period where both the old and new resources
         exist concurrently.
 
         ## Import
 
-        Random Ids can be imported using the `b64_url` with an optional `prefix`. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example with no prefix
+        Random IDs can be imported using the b64_url with an optional prefix. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example with no prefix
 
         ```sh
          $ pulumi import random:index/randomId:RandomId server p-9hUg
         ```
 
-         Example with prefix (prefix is separated by a `,`)
+         Example with prefix (prefix is separated by a ,)
 
         ```sh
          $ pulumi import random:index/randomId:RandomId server my-prefix-,p-9hUg
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[int] byte_length: The number of random bytes to produce. The
-               minimum value is 1, which produces eight bits of randomness.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[str] prefix: Arbitrary string to prefix the output value with. This
-               string is supplied as-is, meaning it is not guaranteed to be URL-safe or
-               base64 encoded.
+        :param pulumi.Input[int] byte_length: The number of random bytes to produce. The minimum value is 1, which produces eight bits of randomness.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[str] prefix: Arbitrary string to prefix the output value with. This string is supplied as-is, meaning it is not guaranteed to be URL-safe or base64 encoded.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RandomIdArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -272,21 +247,21 @@
         This resource can be used in conjunction with resources that have
         the `create_before_destroy` lifecycle flag set to avoid conflicts with
         unique names during the brief period where both the old and new resources
         exist concurrently.
 
         ## Import
 
-        Random Ids can be imported using the `b64_url` with an optional `prefix`. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example with no prefix
+        Random IDs can be imported using the b64_url with an optional prefix. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example with no prefix
 
         ```sh
          $ pulumi import random:index/randomId:RandomId server p-9hUg
         ```
 
-         Example with prefix (prefix is separated by a `,`)
+         Example with prefix (prefix is separated by a ,)
 
         ```sh
          $ pulumi import random:index/randomId:RandomId server my-prefix-,p-9hUg
         ```
 
         :param str resource_name: The name of the resource.
         :param RandomIdArgs args: The arguments to use to populate this resource's properties.
@@ -300,15 +275,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  byte_length: Optional[pulumi.Input[int]] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  prefix: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
@@ -335,35 +310,30 @@
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             b64_std: Optional[pulumi.Input[str]] = None,
             b64_url: Optional[pulumi.Input[str]] = None,
             byte_length: Optional[pulumi.Input[int]] = None,
             dec: Optional[pulumi.Input[str]] = None,
             hex: Optional[pulumi.Input[str]] = None,
-            keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+            keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             prefix: Optional[pulumi.Input[str]] = None) -> 'RandomId':
         """
         Get an existing RandomId resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] b64_std: The generated id presented in base64 without additional transformations.
         :param pulumi.Input[str] b64_url: The generated id presented in base64, using the URL-friendly character set: case-sensitive letters, digits and the characters `_` and `-`.
-        :param pulumi.Input[int] byte_length: The number of random bytes to produce. The
-               minimum value is 1, which produces eight bits of randomness.
+        :param pulumi.Input[int] byte_length: The number of random bytes to produce. The minimum value is 1, which produces eight bits of randomness.
         :param pulumi.Input[str] dec: The generated id presented in non-padded decimal digits.
         :param pulumi.Input[str] hex: The generated id presented in padded hexadecimal digits. This result will always be twice as long as the requested byte length.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[str] prefix: Arbitrary string to prefix the output value with. This
-               string is supplied as-is, meaning it is not guaranteed to be URL-safe or
-               base64 encoded.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[str] prefix: Arbitrary string to prefix the output value with. This string is supplied as-is, meaning it is not guaranteed to be URL-safe or base64 encoded.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RandomIdState.__new__(_RandomIdState)
 
         __props__.__dict__["b64_std"] = b64_std
         __props__.__dict__["b64_url"] = b64_url
@@ -390,16 +360,15 @@
         """
         return pulumi.get(self, "b64_url")
 
     @property
     @pulumi.getter(name="byteLength")
     def byte_length(self) -> pulumi.Output[int]:
         """
-        The number of random bytes to produce. The
-        minimum value is 1, which produces eight bits of randomness.
+        The number of random bytes to produce. The minimum value is 1, which produces eight bits of randomness.
         """
         return pulumi.get(self, "byte_length")
 
     @property
     @pulumi.getter
     def dec(self) -> pulumi.Output[str]:
         """
@@ -413,25 +382,21 @@
         """
         The generated id presented in padded hexadecimal digits. This result will always be twice as long as the requested byte length.
         """
         return pulumi.get(self, "hex")
 
     @property
     @pulumi.getter
-    def keepers(self) -> pulumi.Output[Optional[Mapping[str, Any]]]:
+    def keepers(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @property
     @pulumi.getter
     def prefix(self) -> pulumi.Output[Optional[str]]:
         """
-        Arbitrary string to prefix the output value with. This
-        string is supplied as-is, meaning it is not guaranteed to be URL-safe or
-        base64 encoded.
+        Arbitrary string to prefix the output value with. This string is supplied as-is, meaning it is not guaranteed to be URL-safe or base64 encoded.
         """
         return pulumi.get(self, "prefix")
```

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random/random_integer.py` & `pulumi_random-4.9.0a1674773801/pulumi_random/random_integer.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,23 +12,21 @@
 __all__ = ['RandomIntegerArgs', 'RandomInteger']
 
 @pulumi.input_type
 class RandomIntegerArgs:
     def __init__(__self__, *,
                  max: pulumi.Input[int],
                  min: pulumi.Input[int],
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  seed: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a RandomInteger resource.
         :param pulumi.Input[int] max: The maximum inclusive value of the range.
         :param pulumi.Input[int] min: The minimum inclusive value of the range.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         :param pulumi.Input[str] seed: A custom seed to always produce the same value.
         """
         pulumi.set(__self__, "max", max)
         pulumi.set(__self__, "min", min)
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if seed is not None:
@@ -56,24 +54,22 @@
 
     @min.setter
     def min(self, value: pulumi.Input[int]):
         pulumi.set(self, "min", value)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def seed(self) -> Optional[pulumi.Input[str]]:
         """
         A custom seed to always produce the same value.
@@ -84,27 +80,25 @@
     def seed(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "seed", value)
 
 
 @pulumi.input_type
 class _RandomIntegerState:
     def __init__(__self__, *,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  max: Optional[pulumi.Input[int]] = None,
                  min: Optional[pulumi.Input[int]] = None,
                  result: Optional[pulumi.Input[int]] = None,
                  seed: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RandomInteger resources.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         :param pulumi.Input[int] max: The maximum inclusive value of the range.
         :param pulumi.Input[int] min: The minimum inclusive value of the range.
-        :param pulumi.Input[int] result: (int) The random Integer result.
+        :param pulumi.Input[int] result: The random integer result.
         :param pulumi.Input[str] seed: A custom seed to always produce the same value.
         """
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if max is not None:
             pulumi.set(__self__, "max", max)
         if min is not None:
@@ -112,24 +106,22 @@
         if result is not None:
             pulumi.set(__self__, "result", result)
         if seed is not None:
             pulumi.set(__self__, "seed", seed)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def max(self) -> Optional[pulumi.Input[int]]:
         """
         The maximum inclusive value of the range.
@@ -152,15 +144,15 @@
     def min(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min", value)
 
     @property
     @pulumi.getter
     def result(self) -> Optional[pulumi.Input[int]]:
         """
-        (int) The random Integer result.
+        The random integer result.
         """
         return pulumi.get(self, "result")
 
     @result.setter
     def result(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "result", value)
 
@@ -178,115 +170,53 @@
 
 
 class RandomInteger(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  max: Optional[pulumi.Input[int]] = None,
                  min: Optional[pulumi.Input[int]] = None,
                  seed: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The resource `RandomInteger` generates random values from a given range, described by the `min` and `max` attributes of a given resource.
 
-        This resource can be used in conjunction with resources that have
-        the `create_before_destroy` lifecycle flag set, to avoid conflicts with
-        unique names during the brief period where both the old and new resources
-        exist concurrently.
-
-        ## Example Usage
-
-        The following example shows how to generate a random priority between 1 and 50000 for
-        a `aws_alb_listener_rule` resource:
-
-        ```python
-        import pulumi
-        import pulumi_aws as aws
-        import pulumi_random as random
-
-        priority = random.RandomInteger("priority",
-            keepers={
-                "listener_arn": var["listener_arn"],
-            },
-            max=50000,
-            min=1)
-        main = aws.alb.ListenerRule("main",
-            actions=[aws.alb.ListenerRuleActionArgs(
-                target_group_arn=var["target_group_arn"],
-                type="forward",
-            )],
-            listener_arn=var["listener_arn"],
-            priority=priority.result)
-        ```
-
-        The result of the above will set a random priority.
+        This resource can be used in conjunction with resources that have the `create_before_destroy` lifecycle flag set, to avoid conflicts with unique names during the brief period where both the old and new resources exist concurrently.
 
         ## Import
 
-        Random integers can be imported using the `result`, `min`, and `max`, with an optional `seed`. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example (values are separated by a `,`)
+        Random integers can be imported using the result, min, and max, with an optional seed. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example (values are separated by a ,)
 
         ```sh
          $ pulumi import random:index/randomInteger:RandomInteger priority 15390,1,50000
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         :param pulumi.Input[int] max: The maximum inclusive value of the range.
         :param pulumi.Input[int] min: The minimum inclusive value of the range.
         :param pulumi.Input[str] seed: A custom seed to always produce the same value.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RandomIntegerArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The resource `RandomInteger` generates random values from a given range, described by the `min` and `max` attributes of a given resource.
 
-        This resource can be used in conjunction with resources that have
-        the `create_before_destroy` lifecycle flag set, to avoid conflicts with
-        unique names during the brief period where both the old and new resources
-        exist concurrently.
-
-        ## Example Usage
-
-        The following example shows how to generate a random priority between 1 and 50000 for
-        a `aws_alb_listener_rule` resource:
-
-        ```python
-        import pulumi
-        import pulumi_aws as aws
-        import pulumi_random as random
-
-        priority = random.RandomInteger("priority",
-            keepers={
-                "listener_arn": var["listener_arn"],
-            },
-            max=50000,
-            min=1)
-        main = aws.alb.ListenerRule("main",
-            actions=[aws.alb.ListenerRuleActionArgs(
-                target_group_arn=var["target_group_arn"],
-                type="forward",
-            )],
-            listener_arn=var["listener_arn"],
-            priority=priority.result)
-        ```
-
-        The result of the above will set a random priority.
+        This resource can be used in conjunction with resources that have the `create_before_destroy` lifecycle flag set, to avoid conflicts with unique names during the brief period where both the old and new resources exist concurrently.
 
         ## Import
 
-        Random integers can be imported using the `result`, `min`, and `max`, with an optional `seed`. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example (values are separated by a `,`)
+        Random integers can be imported using the result, min, and max, with an optional seed. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example (values are separated by a ,)
 
         ```sh
          $ pulumi import random:index/randomInteger:RandomInteger priority 15390,1,50000
         ```
 
         :param str resource_name: The name of the resource.
         :param RandomIntegerArgs args: The arguments to use to populate this resource's properties.
@@ -299,15 +229,15 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  max: Optional[pulumi.Input[int]] = None,
                  min: Optional[pulumi.Input[int]] = None,
                  seed: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -331,32 +261,30 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+            keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             max: Optional[pulumi.Input[int]] = None,
             min: Optional[pulumi.Input[int]] = None,
             result: Optional[pulumi.Input[int]] = None,
             seed: Optional[pulumi.Input[str]] = None) -> 'RandomInteger':
         """
         Get an existing RandomInteger resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         :param pulumi.Input[int] max: The maximum inclusive value of the range.
         :param pulumi.Input[int] min: The minimum inclusive value of the range.
-        :param pulumi.Input[int] result: (int) The random Integer result.
+        :param pulumi.Input[int] result: The random integer result.
         :param pulumi.Input[str] seed: A custom seed to always produce the same value.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RandomIntegerState.__new__(_RandomIntegerState)
 
         __props__.__dict__["keepers"] = keepers
@@ -364,19 +292,17 @@
         __props__.__dict__["min"] = min
         __props__.__dict__["result"] = result
         __props__.__dict__["seed"] = seed
         return RandomInteger(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def keepers(self) -> pulumi.Output[Optional[Mapping[str, Any]]]:
+    def keepers(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @property
     @pulumi.getter
     def max(self) -> pulumi.Output[int]:
         """
@@ -392,15 +318,15 @@
         """
         return pulumi.get(self, "min")
 
     @property
     @pulumi.getter
     def result(self) -> pulumi.Output[int]:
         """
-        (int) The random Integer result.
+        The random integer result.
         """
         return pulumi.get(self, "result")
 
     @property
     @pulumi.getter
     def seed(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random/random_password.py` & `pulumi_random-4.9.0a1674773801/pulumi_random/random_password.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,40 +11,39 @@
 
 __all__ = ['RandomPasswordArgs', 'RandomPassword']
 
 @pulumi.input_type
 class RandomPasswordArgs:
     def __init__(__self__, *,
                  length: pulumi.Input[int],
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  lower: Optional[pulumi.Input[bool]] = None,
                  min_lower: Optional[pulumi.Input[int]] = None,
                  min_numeric: Optional[pulumi.Input[int]] = None,
                  min_special: Optional[pulumi.Input[int]] = None,
                  min_upper: Optional[pulumi.Input[int]] = None,
                  number: Optional[pulumi.Input[bool]] = None,
+                 numeric: Optional[pulumi.Input[bool]] = None,
                  override_special: Optional[pulumi.Input[str]] = None,
                  special: Optional[pulumi.Input[bool]] = None,
                  upper: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a RandomPassword resource.
-        :param pulumi.Input[int] length: The length of the string desired.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See [the main provider
-               documentation](../index.html) for more information.
-        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result.
-        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result.
-        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result.
-        :param pulumi.Input[int] min_special: Minimum number of special characters in the result.
-        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result.
-        :param pulumi.Input[bool] number: Include numeric characters in the result.
-        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation. This overrides the default character list in
-               the special argument. The `special` argument must still be set to true for any overwritten characters to be used in
-               generation.
-        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`
-        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result.
+        :param pulumi.Input[int] length: The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result. Default value is `true`.
+        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_special: Minimum number of special characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[bool] number: Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
+        :param pulumi.Input[bool] numeric: Include numeric characters in the result. Default value is `true`.
+        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
+        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
+        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result. Default value is `true`.
         """
         pulumi.set(__self__, "length", length)
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if lower is not None:
             pulumi.set(__self__, "lower", lower)
         if min_lower is not None:
@@ -52,191 +51,208 @@
         if min_numeric is not None:
             pulumi.set(__self__, "min_numeric", min_numeric)
         if min_special is not None:
             pulumi.set(__self__, "min_special", min_special)
         if min_upper is not None:
             pulumi.set(__self__, "min_upper", min_upper)
         if number is not None:
+            warnings.warn("""**NOTE**: This is deprecated, use `numeric` instead.""", DeprecationWarning)
+            pulumi.log.warn("""number is deprecated: **NOTE**: This is deprecated, use `numeric` instead.""")
+        if number is not None:
             pulumi.set(__self__, "number", number)
+        if numeric is not None:
+            pulumi.set(__self__, "numeric", numeric)
         if override_special is not None:
             pulumi.set(__self__, "override_special", override_special)
         if special is not None:
             pulumi.set(__self__, "special", special)
         if upper is not None:
             pulumi.set(__self__, "upper", upper)
 
     @property
     @pulumi.getter
     def length(self) -> pulumi.Input[int]:
         """
-        The length of the string desired.
+        The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
         """
         return pulumi.get(self, "length")
 
     @length.setter
     def length(self, value: pulumi.Input[int]):
         pulumi.set(self, "length", value)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will trigger recreation of resource. See [the main provider
-        documentation](../index.html) for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def lower(self) -> Optional[pulumi.Input[bool]]:
         """
-        Include lowercase alphabet characters in the result.
+        Include lowercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "lower")
 
     @lower.setter
     def lower(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "lower", value)
 
     @property
     @pulumi.getter(name="minLower")
     def min_lower(self) -> Optional[pulumi.Input[int]]:
         """
-        Minimum number of lowercase alphabet characters in the result.
+        Minimum number of lowercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_lower")
 
     @min_lower.setter
     def min_lower(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_lower", value)
 
     @property
     @pulumi.getter(name="minNumeric")
     def min_numeric(self) -> Optional[pulumi.Input[int]]:
         """
-        Minimum number of numeric characters in the result.
+        Minimum number of numeric characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_numeric")
 
     @min_numeric.setter
     def min_numeric(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_numeric", value)
 
     @property
     @pulumi.getter(name="minSpecial")
     def min_special(self) -> Optional[pulumi.Input[int]]:
         """
-        Minimum number of special characters in the result.
+        Minimum number of special characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_special")
 
     @min_special.setter
     def min_special(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_special", value)
 
     @property
     @pulumi.getter(name="minUpper")
     def min_upper(self) -> Optional[pulumi.Input[int]]:
         """
-        Minimum number of uppercase alphabet characters in the result.
+        Minimum number of uppercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_upper")
 
     @min_upper.setter
     def min_upper(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_upper", value)
 
     @property
     @pulumi.getter
     def number(self) -> Optional[pulumi.Input[bool]]:
         """
-        Include numeric characters in the result.
+        Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
         """
         return pulumi.get(self, "number")
 
     @number.setter
     def number(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "number", value)
 
     @property
+    @pulumi.getter
+    def numeric(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Include numeric characters in the result. Default value is `true`.
+        """
+        return pulumi.get(self, "numeric")
+
+    @numeric.setter
+    def numeric(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "numeric", value)
+
+    @property
     @pulumi.getter(name="overrideSpecial")
     def override_special(self) -> Optional[pulumi.Input[str]]:
         """
-        Supply your own list of special characters to use for string generation. This overrides the default character list in
-        the special argument. The `special` argument must still be set to true for any overwritten characters to be used in
-        generation.
+        Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
         """
         return pulumi.get(self, "override_special")
 
     @override_special.setter
     def override_special(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "override_special", value)
 
     @property
     @pulumi.getter
     def special(self) -> Optional[pulumi.Input[bool]]:
         """
-        Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`
+        Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
         """
         return pulumi.get(self, "special")
 
     @special.setter
     def special(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "special", value)
 
     @property
     @pulumi.getter
     def upper(self) -> Optional[pulumi.Input[bool]]:
         """
-        Include uppercase alphabet characters in the result.
+        Include uppercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "upper")
 
     @upper.setter
     def upper(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "upper", value)
 
 
 @pulumi.input_type
 class _RandomPasswordState:
     def __init__(__self__, *,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 bcrypt_hash: Optional[pulumi.Input[str]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  lower: Optional[pulumi.Input[bool]] = None,
                  min_lower: Optional[pulumi.Input[int]] = None,
                  min_numeric: Optional[pulumi.Input[int]] = None,
                  min_special: Optional[pulumi.Input[int]] = None,
                  min_upper: Optional[pulumi.Input[int]] = None,
                  number: Optional[pulumi.Input[bool]] = None,
+                 numeric: Optional[pulumi.Input[bool]] = None,
                  override_special: Optional[pulumi.Input[str]] = None,
                  result: Optional[pulumi.Input[str]] = None,
                  special: Optional[pulumi.Input[bool]] = None,
                  upper: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering RandomPassword resources.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See [the main provider
-               documentation](../index.html) for more information.
-        :param pulumi.Input[int] length: The length of the string desired.
-        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result.
-        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result.
-        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result.
-        :param pulumi.Input[int] min_special: Minimum number of special characters in the result.
-        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result.
-        :param pulumi.Input[bool] number: Include numeric characters in the result.
-        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation. This overrides the default character list in
-               the special argument. The `special` argument must still be set to true for any overwritten characters to be used in
-               generation.
+        :param pulumi.Input[str] bcrypt_hash: A bcrypt hash of the generated random string.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] length: The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
+        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result. Default value is `true`.
+        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_special: Minimum number of special characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[bool] number: Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
+        :param pulumi.Input[bool] numeric: Include numeric characters in the result. Default value is `true`.
+        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
         :param pulumi.Input[str] result: The generated random string.
-        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`
-        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result.
+        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
+        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result. Default value is `true`.
         """
+        if bcrypt_hash is not None:
+            pulumi.set(__self__, "bcrypt_hash", bcrypt_hash)
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if length is not None:
             pulumi.set(__self__, "length", length)
         if lower is not None:
             pulumi.set(__self__, "lower", lower)
         if min_lower is not None:
@@ -244,128 +260,154 @@
         if min_numeric is not None:
             pulumi.set(__self__, "min_numeric", min_numeric)
         if min_special is not None:
             pulumi.set(__self__, "min_special", min_special)
         if min_upper is not None:
             pulumi.set(__self__, "min_upper", min_upper)
         if number is not None:
+            warnings.warn("""**NOTE**: This is deprecated, use `numeric` instead.""", DeprecationWarning)
+            pulumi.log.warn("""number is deprecated: **NOTE**: This is deprecated, use `numeric` instead.""")
+        if number is not None:
             pulumi.set(__self__, "number", number)
+        if numeric is not None:
+            pulumi.set(__self__, "numeric", numeric)
         if override_special is not None:
             pulumi.set(__self__, "override_special", override_special)
         if result is not None:
             pulumi.set(__self__, "result", result)
         if special is not None:
             pulumi.set(__self__, "special", special)
         if upper is not None:
             pulumi.set(__self__, "upper", upper)
 
     @property
+    @pulumi.getter(name="bcryptHash")
+    def bcrypt_hash(self) -> Optional[pulumi.Input[str]]:
+        """
+        A bcrypt hash of the generated random string.
+        """
+        return pulumi.get(self, "bcrypt_hash")
+
+    @bcrypt_hash.setter
+    def bcrypt_hash(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "bcrypt_hash", value)
+
+    @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will trigger recreation of resource. See [the main provider
-        documentation](../index.html) for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def length(self) -> Optional[pulumi.Input[int]]:
         """
-        The length of the string desired.
+        The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
         """
         return pulumi.get(self, "length")
 
     @length.setter
     def length(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "length", value)
 
     @property
     @pulumi.getter
     def lower(self) -> Optional[pulumi.Input[bool]]:
         """
-        Include lowercase alphabet characters in the result.
+        Include lowercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "lower")
 
     @lower.setter
     def lower(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "lower", value)
 
     @property
     @pulumi.getter(name="minLower")
     def min_lower(self) -> Optional[pulumi.Input[int]]:
         """
-        Minimum number of lowercase alphabet characters in the result.
+        Minimum number of lowercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_lower")
 
     @min_lower.setter
     def min_lower(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_lower", value)
 
     @property
     @pulumi.getter(name="minNumeric")
     def min_numeric(self) -> Optional[pulumi.Input[int]]:
         """
-        Minimum number of numeric characters in the result.
+        Minimum number of numeric characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_numeric")
 
     @min_numeric.setter
     def min_numeric(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_numeric", value)
 
     @property
     @pulumi.getter(name="minSpecial")
     def min_special(self) -> Optional[pulumi.Input[int]]:
         """
-        Minimum number of special characters in the result.
+        Minimum number of special characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_special")
 
     @min_special.setter
     def min_special(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_special", value)
 
     @property
     @pulumi.getter(name="minUpper")
     def min_upper(self) -> Optional[pulumi.Input[int]]:
         """
-        Minimum number of uppercase alphabet characters in the result.
+        Minimum number of uppercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_upper")
 
     @min_upper.setter
     def min_upper(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_upper", value)
 
     @property
     @pulumi.getter
     def number(self) -> Optional[pulumi.Input[bool]]:
         """
-        Include numeric characters in the result.
+        Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
         """
         return pulumi.get(self, "number")
 
     @number.setter
     def number(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "number", value)
 
     @property
+    @pulumi.getter
+    def numeric(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Include numeric characters in the result. Default value is `true`.
+        """
+        return pulumi.get(self, "numeric")
+
+    @numeric.setter
+    def numeric(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "numeric", value)
+
+    @property
     @pulumi.getter(name="overrideSpecial")
     def override_special(self) -> Optional[pulumi.Input[str]]:
         """
-        Supply your own list of special characters to use for string generation. This overrides the default character list in
-        the special argument. The `special` argument must still be set to true for any overwritten characters to be used in
-        generation.
+        Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
         """
         return pulumi.get(self, "override_special")
 
     @override_special.setter
     def override_special(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "override_special", value)
 
@@ -381,153 +423,230 @@
     def result(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "result", value)
 
     @property
     @pulumi.getter
     def special(self) -> Optional[pulumi.Input[bool]]:
         """
-        Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`
+        Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
         """
         return pulumi.get(self, "special")
 
     @special.setter
     def special(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "special", value)
 
     @property
     @pulumi.getter
     def upper(self) -> Optional[pulumi.Input[bool]]:
         """
-        Include uppercase alphabet characters in the result.
+        Include uppercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "upper")
 
     @upper.setter
     def upper(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "upper", value)
 
 
 class RandomPassword(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  lower: Optional[pulumi.Input[bool]] = None,
                  min_lower: Optional[pulumi.Input[int]] = None,
                  min_numeric: Optional[pulumi.Input[int]] = None,
                  min_special: Optional[pulumi.Input[int]] = None,
                  min_upper: Optional[pulumi.Input[int]] = None,
                  number: Optional[pulumi.Input[bool]] = None,
+                 numeric: Optional[pulumi.Input[bool]] = None,
                  override_special: Optional[pulumi.Input[str]] = None,
                  special: Optional[pulumi.Input[bool]] = None,
                  upper: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        > **Note:** Requires random provider version >= 2.2.0
-
-        Identical to RandomString with the exception that the
-        result is treated as sensitive and, thus, _not_ displayed in console output.
-
-        > **Note:** All attributes including the generated password will be stored in
-        the raw state as plain-text. [Read more about sensitive data in
-        state](https://www.terraform.io/docs/state/sensitive-data.html).
-
-        This resource *does* use a cryptographic random number generator.
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aws as aws
         import pulumi_random as random
 
         password = random.RandomPassword("password",
             length=16,
             special=True,
-            override_special="_%@")
+            override_special="!#$%&*()-_=+[]{}<>:?")
         example = aws.rds.Instance("example",
             instance_class="db.t3.micro",
             allocated_storage=64,
             engine="mysql",
             username="someone",
             password=password.result)
         ```
 
         ## Import
 
-        Random Password can be imported by specifying the value of the string
+        ### Avoiding Replacement
 
         ```sh
-         $ pulumi import random:index/randomPassword:RandomPassword password securepassword
+         $ pulumi import random:index/randomPassword:RandomPassword If the resource were imported using `random_password.password securepassword`,
         ```
 
+         replacement could be avoided by using1. Attribute values that match the imported ID and defaults:
+
+         terraform
+
+         resource "random_password" "password" {
+
+         length = 14
+
+         lower
+
+        = true
+
+         } 2. Attribute values that match the imported ID and omit the attributes with defaults:
+
+         terraform
+
+         resource "random_password" "password" {
+
+         length = 14
+
+         } 3. `ignore_changes` specifying the attributes to ignore:
+
+         terraform
+
+         resource "random_password" "password" {
+
+         length = 16
+
+         lower
+
+        = false
+
+         lifecycle {
+
+         ignore_changes = [
+
+         length,
+
+         lower,
+
+         ]
+
+         }
+
+         }
+
+         **NOTE** `ignore_changes` is only required until the resource is recreated after import,
+
+         after which it will use the configuration values specified.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See [the main provider
-               documentation](../index.html) for more information.
-        :param pulumi.Input[int] length: The length of the string desired.
-        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result.
-        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result.
-        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result.
-        :param pulumi.Input[int] min_special: Minimum number of special characters in the result.
-        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result.
-        :param pulumi.Input[bool] number: Include numeric characters in the result.
-        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation. This overrides the default character list in
-               the special argument. The `special` argument must still be set to true for any overwritten characters to be used in
-               generation.
-        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`
-        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] length: The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
+        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result. Default value is `true`.
+        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_special: Minimum number of special characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[bool] number: Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
+        :param pulumi.Input[bool] numeric: Include numeric characters in the result. Default value is `true`.
+        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
+        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
+        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result. Default value is `true`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RandomPasswordArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        > **Note:** Requires random provider version >= 2.2.0
-
-        Identical to RandomString with the exception that the
-        result is treated as sensitive and, thus, _not_ displayed in console output.
-
-        > **Note:** All attributes including the generated password will be stored in
-        the raw state as plain-text. [Read more about sensitive data in
-        state](https://www.terraform.io/docs/state/sensitive-data.html).
-
-        This resource *does* use a cryptographic random number generator.
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aws as aws
         import pulumi_random as random
 
         password = random.RandomPassword("password",
             length=16,
             special=True,
-            override_special="_%@")
+            override_special="!#$%&*()-_=+[]{}<>:?")
         example = aws.rds.Instance("example",
             instance_class="db.t3.micro",
             allocated_storage=64,
             engine="mysql",
             username="someone",
             password=password.result)
         ```
 
         ## Import
 
-        Random Password can be imported by specifying the value of the string
+        ### Avoiding Replacement
 
         ```sh
-         $ pulumi import random:index/randomPassword:RandomPassword password securepassword
+         $ pulumi import random:index/randomPassword:RandomPassword If the resource were imported using `random_password.password securepassword`,
         ```
 
+         replacement could be avoided by using1. Attribute values that match the imported ID and defaults:
+
+         terraform
+
+         resource "random_password" "password" {
+
+         length = 14
+
+         lower
+
+        = true
+
+         } 2. Attribute values that match the imported ID and omit the attributes with defaults:
+
+         terraform
+
+         resource "random_password" "password" {
+
+         length = 14
+
+         } 3. `ignore_changes` specifying the attributes to ignore:
+
+         terraform
+
+         resource "random_password" "password" {
+
+         length = 16
+
+         lower
+
+        = false
+
+         lifecycle {
+
+         ignore_changes = [
+
+         length,
+
+         lower,
+
+         ]
+
+         }
+
+         }
+
+         **NOTE** `ignore_changes` is only required until the resource is recreated after import,
+
+         after which it will use the configuration values specified.
+
         :param str resource_name: The name of the resource.
         :param RandomPasswordArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(RandomPasswordArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -535,22 +654,23 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  lower: Optional[pulumi.Input[bool]] = None,
                  min_lower: Optional[pulumi.Input[int]] = None,
                  min_numeric: Optional[pulumi.Input[int]] = None,
                  min_special: Optional[pulumi.Input[int]] = None,
                  min_upper: Optional[pulumi.Input[int]] = None,
                  number: Optional[pulumi.Input[bool]] = None,
+                 numeric: Optional[pulumi.Input[bool]] = None,
                  override_special: Optional[pulumi.Input[str]] = None,
                  special: Optional[pulumi.Input[bool]] = None,
                  upper: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -564,176 +684,197 @@
                 raise TypeError("Missing required property 'length'")
             __props__.__dict__["length"] = length
             __props__.__dict__["lower"] = lower
             __props__.__dict__["min_lower"] = min_lower
             __props__.__dict__["min_numeric"] = min_numeric
             __props__.__dict__["min_special"] = min_special
             __props__.__dict__["min_upper"] = min_upper
+            if number is not None and not opts.urn:
+                warnings.warn("""**NOTE**: This is deprecated, use `numeric` instead.""", DeprecationWarning)
+                pulumi.log.warn("""number is deprecated: **NOTE**: This is deprecated, use `numeric` instead.""")
             __props__.__dict__["number"] = number
+            __props__.__dict__["numeric"] = numeric
             __props__.__dict__["override_special"] = override_special
             __props__.__dict__["special"] = special
             __props__.__dict__["upper"] = upper
+            __props__.__dict__["bcrypt_hash"] = None
             __props__.__dict__["result"] = None
-        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["result"])
+        secret_opts = pulumi.ResourceOptions(additional_secret_outputs=["bcryptHash", "result"])
         opts = pulumi.ResourceOptions.merge(opts, secret_opts)
         super(RandomPassword, __self__).__init__(
             'random:index/randomPassword:RandomPassword',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+            bcrypt_hash: Optional[pulumi.Input[str]] = None,
+            keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             length: Optional[pulumi.Input[int]] = None,
             lower: Optional[pulumi.Input[bool]] = None,
             min_lower: Optional[pulumi.Input[int]] = None,
             min_numeric: Optional[pulumi.Input[int]] = None,
             min_special: Optional[pulumi.Input[int]] = None,
             min_upper: Optional[pulumi.Input[int]] = None,
             number: Optional[pulumi.Input[bool]] = None,
+            numeric: Optional[pulumi.Input[bool]] = None,
             override_special: Optional[pulumi.Input[str]] = None,
             result: Optional[pulumi.Input[str]] = None,
             special: Optional[pulumi.Input[bool]] = None,
             upper: Optional[pulumi.Input[bool]] = None) -> 'RandomPassword':
         """
         Get an existing RandomPassword resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See [the main provider
-               documentation](../index.html) for more information.
-        :param pulumi.Input[int] length: The length of the string desired.
-        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result.
-        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result.
-        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result.
-        :param pulumi.Input[int] min_special: Minimum number of special characters in the result.
-        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result.
-        :param pulumi.Input[bool] number: Include numeric characters in the result.
-        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation. This overrides the default character list in
-               the special argument. The `special` argument must still be set to true for any overwritten characters to be used in
-               generation.
+        :param pulumi.Input[str] bcrypt_hash: A bcrypt hash of the generated random string.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] length: The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
+        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result. Default value is `true`.
+        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_special: Minimum number of special characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[bool] number: Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
+        :param pulumi.Input[bool] numeric: Include numeric characters in the result. Default value is `true`.
+        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
         :param pulumi.Input[str] result: The generated random string.
-        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`
-        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result.
+        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
+        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result. Default value is `true`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RandomPasswordState.__new__(_RandomPasswordState)
 
+        __props__.__dict__["bcrypt_hash"] = bcrypt_hash
         __props__.__dict__["keepers"] = keepers
         __props__.__dict__["length"] = length
         __props__.__dict__["lower"] = lower
         __props__.__dict__["min_lower"] = min_lower
         __props__.__dict__["min_numeric"] = min_numeric
         __props__.__dict__["min_special"] = min_special
         __props__.__dict__["min_upper"] = min_upper
         __props__.__dict__["number"] = number
+        __props__.__dict__["numeric"] = numeric
         __props__.__dict__["override_special"] = override_special
         __props__.__dict__["result"] = result
         __props__.__dict__["special"] = special
         __props__.__dict__["upper"] = upper
         return RandomPassword(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="bcryptHash")
+    def bcrypt_hash(self) -> pulumi.Output[str]:
+        """
+        A bcrypt hash of the generated random string.
+        """
+        return pulumi.get(self, "bcrypt_hash")
+
+    @property
     @pulumi.getter
-    def keepers(self) -> pulumi.Output[Optional[Mapping[str, Any]]]:
+    def keepers(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Arbitrary map of values that, when changed, will trigger recreation of resource. See [the main provider
-        documentation](../index.html) for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @property
     @pulumi.getter
     def length(self) -> pulumi.Output[int]:
         """
-        The length of the string desired.
+        The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
         """
         return pulumi.get(self, "length")
 
     @property
     @pulumi.getter
-    def lower(self) -> pulumi.Output[Optional[bool]]:
+    def lower(self) -> pulumi.Output[bool]:
         """
-        Include lowercase alphabet characters in the result.
+        Include lowercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "lower")
 
     @property
     @pulumi.getter(name="minLower")
-    def min_lower(self) -> pulumi.Output[Optional[int]]:
+    def min_lower(self) -> pulumi.Output[int]:
         """
-        Minimum number of lowercase alphabet characters in the result.
+        Minimum number of lowercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_lower")
 
     @property
     @pulumi.getter(name="minNumeric")
-    def min_numeric(self) -> pulumi.Output[Optional[int]]:
+    def min_numeric(self) -> pulumi.Output[int]:
         """
-        Minimum number of numeric characters in the result.
+        Minimum number of numeric characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_numeric")
 
     @property
     @pulumi.getter(name="minSpecial")
-    def min_special(self) -> pulumi.Output[Optional[int]]:
+    def min_special(self) -> pulumi.Output[int]:
         """
-        Minimum number of special characters in the result.
+        Minimum number of special characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_special")
 
     @property
     @pulumi.getter(name="minUpper")
-    def min_upper(self) -> pulumi.Output[Optional[int]]:
+    def min_upper(self) -> pulumi.Output[int]:
         """
-        Minimum number of uppercase alphabet characters in the result.
+        Minimum number of uppercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_upper")
 
     @property
     @pulumi.getter
-    def number(self) -> pulumi.Output[Optional[bool]]:
+    def number(self) -> pulumi.Output[bool]:
         """
-        Include numeric characters in the result.
+        Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
         """
         return pulumi.get(self, "number")
 
     @property
+    @pulumi.getter
+    def numeric(self) -> pulumi.Output[bool]:
+        """
+        Include numeric characters in the result. Default value is `true`.
+        """
+        return pulumi.get(self, "numeric")
+
+    @property
     @pulumi.getter(name="overrideSpecial")
     def override_special(self) -> pulumi.Output[Optional[str]]:
         """
-        Supply your own list of special characters to use for string generation. This overrides the default character list in
-        the special argument. The `special` argument must still be set to true for any overwritten characters to be used in
-        generation.
+        Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
         """
         return pulumi.get(self, "override_special")
 
     @property
     @pulumi.getter
     def result(self) -> pulumi.Output[str]:
         """
         The generated random string.
         """
         return pulumi.get(self, "result")
 
     @property
     @pulumi.getter
-    def special(self) -> pulumi.Output[Optional[bool]]:
+    def special(self) -> pulumi.Output[bool]:
         """
-        Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`
+        Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
         """
         return pulumi.get(self, "special")
 
     @property
     @pulumi.getter
-    def upper(self) -> pulumi.Output[Optional[bool]]:
+    def upper(self) -> pulumi.Output[bool]:
         """
-        Include uppercase alphabet characters in the result.
+        Include uppercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "upper")
```

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random/random_pet.py` & `pulumi_random-4.9.0a1674773801/pulumi_random/random_pet.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,55 +10,51 @@
 from . import _utilities
 
 __all__ = ['RandomPetArgs', 'RandomPet']
 
 @pulumi.input_type
 class RandomPetArgs:
     def __init__(__self__, *,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  prefix: Optional[pulumi.Input[str]] = None,
                  separator: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a RandomPet resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] length: The length (in words) of the pet name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] length: The length (in words) of the pet name. Defaults to 2
         :param pulumi.Input[str] prefix: A string to prefix the name with.
-        :param pulumi.Input[str] separator: The character to separate words in the pet name.
+        :param pulumi.Input[str] separator: The character to separate words in the pet name. Defaults to "-"
         """
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if length is not None:
             pulumi.set(__self__, "length", length)
         if prefix is not None:
             pulumi.set(__self__, "prefix", prefix)
         if separator is not None:
             pulumi.set(__self__, "separator", separator)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def length(self) -> Optional[pulumi.Input[int]]:
         """
-        The length (in words) of the pet name.
+        The length (in words) of the pet name. Defaults to 2
         """
         return pulumi.get(self, "length")
 
     @length.setter
     def length(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "length", value)
 
@@ -74,67 +70,63 @@
     def prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "prefix", value)
 
     @property
     @pulumi.getter
     def separator(self) -> Optional[pulumi.Input[str]]:
         """
-        The character to separate words in the pet name.
+        The character to separate words in the pet name. Defaults to "-"
         """
         return pulumi.get(self, "separator")
 
     @separator.setter
     def separator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "separator", value)
 
 
 @pulumi.input_type
 class _RandomPetState:
     def __init__(__self__, *,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  prefix: Optional[pulumi.Input[str]] = None,
                  separator: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RandomPet resources.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] length: The length (in words) of the pet name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] length: The length (in words) of the pet name. Defaults to 2
         :param pulumi.Input[str] prefix: A string to prefix the name with.
-        :param pulumi.Input[str] separator: The character to separate words in the pet name.
+        :param pulumi.Input[str] separator: The character to separate words in the pet name. Defaults to "-"
         """
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if length is not None:
             pulumi.set(__self__, "length", length)
         if prefix is not None:
             pulumi.set(__self__, "prefix", prefix)
         if separator is not None:
             pulumi.set(__self__, "separator", separator)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def length(self) -> Optional[pulumi.Input[int]]:
         """
-        The length (in words) of the pet name.
+        The length (in words) of the pet name. Defaults to 2
         """
         return pulumi.get(self, "length")
 
     @length.setter
     def length(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "length", value)
 
@@ -150,65 +142,55 @@
     def prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "prefix", value)
 
     @property
     @pulumi.getter
     def separator(self) -> Optional[pulumi.Input[str]]:
         """
-        The character to separate words in the pet name.
+        The character to separate words in the pet name. Defaults to "-"
         """
         return pulumi.get(self, "separator")
 
     @separator.setter
     def separator(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "separator", value)
 
 
 class RandomPet(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  prefix: Optional[pulumi.Input[str]] = None,
                  separator: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The resource `RandomPet` generates random pet names that are intended to be
-        used as unique identifiers for other resources.
+        The resource `RandomPet` generates random pet names that are intended to be used as unique identifiers for other resources.
 
-        This resource can be used in conjunction with resources that have
-        the `create_before_destroy` lifecycle flag set, to avoid conflicts with
-        unique names during the brief period where both the old and new resources
-        exist concurrently.
+        This resource can be used in conjunction with resources that have the `create_before_destroy` lifecycle flag set, to avoid conflicts with unique names during the brief period where both the old and new resources exist concurrently.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] length: The length (in words) of the pet name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] length: The length (in words) of the pet name. Defaults to 2
         :param pulumi.Input[str] prefix: A string to prefix the name with.
-        :param pulumi.Input[str] separator: The character to separate words in the pet name.
+        :param pulumi.Input[str] separator: The character to separate words in the pet name. Defaults to "-"
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[RandomPetArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The resource `RandomPet` generates random pet names that are intended to be
-        used as unique identifiers for other resources.
+        The resource `RandomPet` generates random pet names that are intended to be used as unique identifiers for other resources.
 
-        This resource can be used in conjunction with resources that have
-        the `create_before_destroy` lifecycle flag set, to avoid conflicts with
-        unique names during the brief period where both the old and new resources
-        exist concurrently.
+        This resource can be used in conjunction with resources that have the `create_before_destroy` lifecycle flag set, to avoid conflicts with unique names during the brief period where both the old and new resources exist concurrently.
 
         :param str resource_name: The name of the resource.
         :param RandomPetArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
@@ -217,15 +199,15 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  prefix: Optional[pulumi.Input[str]] = None,
                  separator: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -244,69 +226,65 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+            keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             length: Optional[pulumi.Input[int]] = None,
             prefix: Optional[pulumi.Input[str]] = None,
             separator: Optional[pulumi.Input[str]] = None) -> 'RandomPet':
         """
         Get an existing RandomPet resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] length: The length (in words) of the pet name.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] length: The length (in words) of the pet name. Defaults to 2
         :param pulumi.Input[str] prefix: A string to prefix the name with.
-        :param pulumi.Input[str] separator: The character to separate words in the pet name.
+        :param pulumi.Input[str] separator: The character to separate words in the pet name. Defaults to "-"
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RandomPetState.__new__(_RandomPetState)
 
         __props__.__dict__["keepers"] = keepers
         __props__.__dict__["length"] = length
         __props__.__dict__["prefix"] = prefix
         __props__.__dict__["separator"] = separator
         return RandomPet(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def keepers(self) -> pulumi.Output[Optional[Mapping[str, Any]]]:
+    def keepers(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @property
     @pulumi.getter
-    def length(self) -> pulumi.Output[Optional[int]]:
+    def length(self) -> pulumi.Output[int]:
         """
-        The length (in words) of the pet name.
+        The length (in words) of the pet name. Defaults to 2
         """
         return pulumi.get(self, "length")
 
     @property
     @pulumi.getter
     def prefix(self) -> pulumi.Output[Optional[str]]:
         """
         A string to prefix the name with.
         """
         return pulumi.get(self, "prefix")
 
     @property
     @pulumi.getter
-    def separator(self) -> pulumi.Output[Optional[str]]:
+    def separator(self) -> pulumi.Output[str]:
         """
-        The character to separate words in the pet name.
+        The character to separate words in the pet name. Defaults to "-"
         """
         return pulumi.get(self, "separator")
```

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random/random_shuffle.py` & `pulumi_random-4.9.0a1674773801/pulumi_random/random_shuffle.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,31 +11,23 @@
 
 __all__ = ['RandomShuffleArgs', 'RandomShuffle']
 
 @pulumi.input_type
 class RandomShuffleArgs:
     def __init__(__self__, *,
                  inputs: pulumi.Input[Sequence[pulumi.Input[str]]],
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  result_count: Optional[pulumi.Input[int]] = None,
                  seed: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a RandomShuffle resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] inputs: The list of strings to shuffle.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] result_count: The number of results to return. Defaults to
-               the number of items in the `input` list. If fewer items are requested,
-               some elements will be excluded from the result. If more items are requested,
-               items will be repeated in the result but not more frequently than the number
-               of items in the input list.
-        :param pulumi.Input[str] seed: Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the
-               list. **Important:** Even with an identical seed, it is not guaranteed that the same permutation will be produced across
-               different versions of Terraform. This argument causes the result to be *less volatile*, but not fixed for all time.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] result_count: The number of results to return. Defaults to the number of items in the `input` list. If fewer items are requested, some elements will be excluded from the result. If more items are requested, items will be repeated in the result but not more frequently than the number of items in the input list.
+        :param pulumi.Input[str] seed: Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the list.
         """
         pulumi.set(__self__, "inputs", inputs)
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if result_count is not None:
             pulumi.set(__self__, "result_count", result_count)
         if seed is not None:
@@ -51,80 +43,64 @@
 
     @inputs.setter
     def inputs(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "inputs", value)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter(name="resultCount")
     def result_count(self) -> Optional[pulumi.Input[int]]:
         """
-        The number of results to return. Defaults to
-        the number of items in the `input` list. If fewer items are requested,
-        some elements will be excluded from the result. If more items are requested,
-        items will be repeated in the result but not more frequently than the number
-        of items in the input list.
+        The number of results to return. Defaults to the number of items in the `input` list. If fewer items are requested, some elements will be excluded from the result. If more items are requested, items will be repeated in the result but not more frequently than the number of items in the input list.
         """
         return pulumi.get(self, "result_count")
 
     @result_count.setter
     def result_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "result_count", value)
 
     @property
     @pulumi.getter
     def seed(self) -> Optional[pulumi.Input[str]]:
         """
-        Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the
-        list. **Important:** Even with an identical seed, it is not guaranteed that the same permutation will be produced across
-        different versions of Terraform. This argument causes the result to be *less volatile*, but not fixed for all time.
+        Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the list.
         """
         return pulumi.get(self, "seed")
 
     @seed.setter
     def seed(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "seed", value)
 
 
 @pulumi.input_type
 class _RandomShuffleState:
     def __init__(__self__, *,
                  inputs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  result_count: Optional[pulumi.Input[int]] = None,
                  results: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  seed: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RandomShuffle resources.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] inputs: The list of strings to shuffle.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] result_count: The number of results to return. Defaults to
-               the number of items in the `input` list. If fewer items are requested,
-               some elements will be excluded from the result. If more items are requested,
-               items will be repeated in the result but not more frequently than the number
-               of items in the input list.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] result_count: The number of results to return. Defaults to the number of items in the `input` list. If fewer items are requested, some elements will be excluded from the result. If more items are requested, items will be repeated in the result but not more frequently than the number of items in the input list.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] results: Random permutation of the list of strings given in `input`.
-        :param pulumi.Input[str] seed: Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the
-               list. **Important:** Even with an identical seed, it is not guaranteed that the same permutation will be produced across
-               different versions of Terraform. This argument causes the result to be *less volatile*, but not fixed for all time.
+        :param pulumi.Input[str] seed: Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the list.
         """
         if inputs is not None:
             pulumi.set(__self__, "inputs", inputs)
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if result_count is not None:
             pulumi.set(__self__, "result_count", result_count)
@@ -143,35 +119,29 @@
 
     @inputs.setter
     def inputs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "inputs", value)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter(name="resultCount")
     def result_count(self) -> Optional[pulumi.Input[int]]:
         """
-        The number of results to return. Defaults to
-        the number of items in the `input` list. If fewer items are requested,
-        some elements will be excluded from the result. If more items are requested,
-        items will be repeated in the result but not more frequently than the number
-        of items in the input list.
+        The number of results to return. Defaults to the number of items in the `input` list. If fewer items are requested, some elements will be excluded from the result. If more items are requested, items will be repeated in the result but not more frequently than the number of items in the input list.
         """
         return pulumi.get(self, "result_count")
 
     @result_count.setter
     def result_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "result_count", value)
 
@@ -187,38 +157,35 @@
     def results(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "results", value)
 
     @property
     @pulumi.getter
     def seed(self) -> Optional[pulumi.Input[str]]:
         """
-        Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the
-        list. **Important:** Even with an identical seed, it is not guaranteed that the same permutation will be produced across
-        different versions of Terraform. This argument causes the result to be *less volatile*, but not fixed for all time.
+        Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the list.
         """
         return pulumi.get(self, "seed")
 
     @seed.setter
     def seed(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "seed", value)
 
 
 class RandomShuffle(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  inputs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  result_count: Optional[pulumi.Input[int]] = None,
                  seed: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The resource `RandomShuffle` generates a random permutation of a list
-        of strings given as an argument.
+        The resource `RandomShuffle` generates a random permutation of a list of strings given as an argument.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aws as aws
         import pulumi_random as random
@@ -227,41 +194,33 @@
             inputs=[
                 "us-west-1a",
                 "us-west-1c",
                 "us-west-1d",
                 "us-west-1e",
             ],
             result_count=2)
-        example = aws.elb.LoadBalancer("example", availability_zones=az.results)
+        example = aws.elb.LoadBalancer("example", availability_zones=[az.results])
+        # ... and other aws_elb arguments ...
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] inputs: The list of strings to shuffle.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] result_count: The number of results to return. Defaults to
-               the number of items in the `input` list. If fewer items are requested,
-               some elements will be excluded from the result. If more items are requested,
-               items will be repeated in the result but not more frequently than the number
-               of items in the input list.
-        :param pulumi.Input[str] seed: Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the
-               list. **Important:** Even with an identical seed, it is not guaranteed that the same permutation will be produced across
-               different versions of Terraform. This argument causes the result to be *less volatile*, but not fixed for all time.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] result_count: The number of results to return. Defaults to the number of items in the `input` list. If fewer items are requested, some elements will be excluded from the result. If more items are requested, items will be repeated in the result but not more frequently than the number of items in the input list.
+        :param pulumi.Input[str] seed: Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the list.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RandomShuffleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The resource `RandomShuffle` generates a random permutation of a list
-        of strings given as an argument.
+        The resource `RandomShuffle` generates a random permutation of a list of strings given as an argument.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_aws as aws
         import pulumi_random as random
@@ -270,15 +229,16 @@
             inputs=[
                 "us-west-1a",
                 "us-west-1c",
                 "us-west-1d",
                 "us-west-1e",
             ],
             result_count=2)
-        example = aws.elb.LoadBalancer("example", availability_zones=az.results)
+        example = aws.elb.LoadBalancer("example", availability_zones=[az.results])
+        # ... and other aws_elb arguments ...
         ```
 
         :param str resource_name: The name of the resource.
         :param RandomShuffleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -289,15 +249,15 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  inputs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  result_count: Optional[pulumi.Input[int]] = None,
                  seed: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
@@ -319,38 +279,30 @@
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             inputs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
-            keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+            keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             result_count: Optional[pulumi.Input[int]] = None,
             results: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             seed: Optional[pulumi.Input[str]] = None) -> 'RandomShuffle':
         """
         Get an existing RandomShuffle resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] inputs: The list of strings to shuffle.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] result_count: The number of results to return. Defaults to
-               the number of items in the `input` list. If fewer items are requested,
-               some elements will be excluded from the result. If more items are requested,
-               items will be repeated in the result but not more frequently than the number
-               of items in the input list.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] result_count: The number of results to return. Defaults to the number of items in the `input` list. If fewer items are requested, some elements will be excluded from the result. If more items are requested, items will be repeated in the result but not more frequently than the number of items in the input list.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] results: Random permutation of the list of strings given in `input`.
-        :param pulumi.Input[str] seed: Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the
-               list. **Important:** Even with an identical seed, it is not guaranteed that the same permutation will be produced across
-               different versions of Terraform. This argument causes the result to be *less volatile*, but not fixed for all time.
+        :param pulumi.Input[str] seed: Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the list.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RandomShuffleState.__new__(_RandomShuffleState)
 
         __props__.__dict__["inputs"] = inputs
         __props__.__dict__["keepers"] = keepers
@@ -365,31 +317,25 @@
         """
         The list of strings to shuffle.
         """
         return pulumi.get(self, "inputs")
 
     @property
     @pulumi.getter
-    def keepers(self) -> pulumi.Output[Optional[Mapping[str, Any]]]:
+    def keepers(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @property
     @pulumi.getter(name="resultCount")
     def result_count(self) -> pulumi.Output[Optional[int]]:
         """
-        The number of results to return. Defaults to
-        the number of items in the `input` list. If fewer items are requested,
-        some elements will be excluded from the result. If more items are requested,
-        items will be repeated in the result but not more frequently than the number
-        of items in the input list.
+        The number of results to return. Defaults to the number of items in the `input` list. If fewer items are requested, some elements will be excluded from the result. If more items are requested, items will be repeated in the result but not more frequently than the number of items in the input list.
         """
         return pulumi.get(self, "result_count")
 
     @property
     @pulumi.getter
     def results(self) -> pulumi.Output[Sequence[str]]:
         """
@@ -397,13 +343,11 @@
         """
         return pulumi.get(self, "results")
 
     @property
     @pulumi.getter
     def seed(self) -> pulumi.Output[Optional[str]]:
         """
-        Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the
-        list. **Important:** Even with an identical seed, it is not guaranteed that the same permutation will be produced across
-        different versions of Terraform. This argument causes the result to be *less volatile*, but not fixed for all time.
+        Arbitrary string with which to seed the random number generator, in order to produce less-volatile permutations of the list.
         """
         return pulumi.get(self, "seed")
```

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random/random_string.py` & `pulumi_random-4.9.0a1674773801/pulumi_random/random_string.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,50 +11,39 @@
 
 __all__ = ['RandomStringArgs', 'RandomString']
 
 @pulumi.input_type
 class RandomStringArgs:
     def __init__(__self__, *,
                  length: pulumi.Input[int],
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  lower: Optional[pulumi.Input[bool]] = None,
                  min_lower: Optional[pulumi.Input[int]] = None,
                  min_numeric: Optional[pulumi.Input[int]] = None,
                  min_special: Optional[pulumi.Input[int]] = None,
                  min_upper: Optional[pulumi.Input[int]] = None,
                  number: Optional[pulumi.Input[bool]] = None,
+                 numeric: Optional[pulumi.Input[bool]] = None,
                  override_special: Optional[pulumi.Input[str]] = None,
                  special: Optional[pulumi.Input[bool]] = None,
                  upper: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a RandomString resource.
-        :param pulumi.Input[int] length: The length of the string desired
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[bool] lower: (default true) Include lowercase alphabet characters
-               in random string.
-        :param pulumi.Input[int] min_lower: (default 0) Minimum number of lowercase alphabet
-               characters in random string.
-        :param pulumi.Input[int] min_numeric: (default 0) Minimum number of numeric characters
-               in random string.
-        :param pulumi.Input[int] min_special: (default 0) Minimum number of special characters
-               in random string.
-        :param pulumi.Input[int] min_upper: (default 0) Minimum number of uppercase alphabet
-               characters in random string.
-        :param pulumi.Input[bool] number: (default true) Include numeric characters in random
-               string.
-        :param pulumi.Input[str] override_special: Supply your own list of special characters to
-               use for string generation.  This overrides the default character list in the special
-               argument.  The special argument must still be set to true for any overwritten
-               characters to be used in generation.
-        :param pulumi.Input[bool] special: (default true) Include special characters in random
-               string. These are `!@#$%&*()-_=+[]{}<>:?`
-        :param pulumi.Input[bool] upper: (default true) Include uppercase alphabet characters
-               in random string.
+        :param pulumi.Input[int] length: The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result. Default value is `true`.
+        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_special: Minimum number of special characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[bool] number: Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
+        :param pulumi.Input[bool] numeric: Include numeric characters in the result. Default value is `true`.
+        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
+        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
+        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result. Default value is `true`.
         """
         pulumi.set(__self__, "length", length)
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if lower is not None:
             pulumi.set(__self__, "lower", lower)
         if min_lower is not None:
@@ -62,210 +51,203 @@
         if min_numeric is not None:
             pulumi.set(__self__, "min_numeric", min_numeric)
         if min_special is not None:
             pulumi.set(__self__, "min_special", min_special)
         if min_upper is not None:
             pulumi.set(__self__, "min_upper", min_upper)
         if number is not None:
+            warnings.warn("""**NOTE**: This is deprecated, use `numeric` instead.""", DeprecationWarning)
+            pulumi.log.warn("""number is deprecated: **NOTE**: This is deprecated, use `numeric` instead.""")
+        if number is not None:
             pulumi.set(__self__, "number", number)
+        if numeric is not None:
+            pulumi.set(__self__, "numeric", numeric)
         if override_special is not None:
             pulumi.set(__self__, "override_special", override_special)
         if special is not None:
             pulumi.set(__self__, "special", special)
         if upper is not None:
             pulumi.set(__self__, "upper", upper)
 
     @property
     @pulumi.getter
     def length(self) -> pulumi.Input[int]:
         """
-        The length of the string desired
+        The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
         """
         return pulumi.get(self, "length")
 
     @length.setter
     def length(self, value: pulumi.Input[int]):
         pulumi.set(self, "length", value)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def lower(self) -> Optional[pulumi.Input[bool]]:
         """
-        (default true) Include lowercase alphabet characters
-        in random string.
+        Include lowercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "lower")
 
     @lower.setter
     def lower(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "lower", value)
 
     @property
     @pulumi.getter(name="minLower")
     def min_lower(self) -> Optional[pulumi.Input[int]]:
         """
-        (default 0) Minimum number of lowercase alphabet
-        characters in random string.
+        Minimum number of lowercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_lower")
 
     @min_lower.setter
     def min_lower(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_lower", value)
 
     @property
     @pulumi.getter(name="minNumeric")
     def min_numeric(self) -> Optional[pulumi.Input[int]]:
         """
-        (default 0) Minimum number of numeric characters
-        in random string.
+        Minimum number of numeric characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_numeric")
 
     @min_numeric.setter
     def min_numeric(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_numeric", value)
 
     @property
     @pulumi.getter(name="minSpecial")
     def min_special(self) -> Optional[pulumi.Input[int]]:
         """
-        (default 0) Minimum number of special characters
-        in random string.
+        Minimum number of special characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_special")
 
     @min_special.setter
     def min_special(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_special", value)
 
     @property
     @pulumi.getter(name="minUpper")
     def min_upper(self) -> Optional[pulumi.Input[int]]:
         """
-        (default 0) Minimum number of uppercase alphabet
-        characters in random string.
+        Minimum number of uppercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_upper")
 
     @min_upper.setter
     def min_upper(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_upper", value)
 
     @property
     @pulumi.getter
     def number(self) -> Optional[pulumi.Input[bool]]:
         """
-        (default true) Include numeric characters in random
-        string.
+        Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
         """
         return pulumi.get(self, "number")
 
     @number.setter
     def number(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "number", value)
 
     @property
+    @pulumi.getter
+    def numeric(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Include numeric characters in the result. Default value is `true`.
+        """
+        return pulumi.get(self, "numeric")
+
+    @numeric.setter
+    def numeric(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "numeric", value)
+
+    @property
     @pulumi.getter(name="overrideSpecial")
     def override_special(self) -> Optional[pulumi.Input[str]]:
         """
-        Supply your own list of special characters to
-        use for string generation.  This overrides the default character list in the special
-        argument.  The special argument must still be set to true for any overwritten
-        characters to be used in generation.
+        Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
         """
         return pulumi.get(self, "override_special")
 
     @override_special.setter
     def override_special(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "override_special", value)
 
     @property
     @pulumi.getter
     def special(self) -> Optional[pulumi.Input[bool]]:
         """
-        (default true) Include special characters in random
-        string. These are `!@#$%&*()-_=+[]{}<>:?`
+        Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
         """
         return pulumi.get(self, "special")
 
     @special.setter
     def special(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "special", value)
 
     @property
     @pulumi.getter
     def upper(self) -> Optional[pulumi.Input[bool]]:
         """
-        (default true) Include uppercase alphabet characters
-        in random string.
+        Include uppercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "upper")
 
     @upper.setter
     def upper(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "upper", value)
 
 
 @pulumi.input_type
 class _RandomStringState:
     def __init__(__self__, *,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  lower: Optional[pulumi.Input[bool]] = None,
                  min_lower: Optional[pulumi.Input[int]] = None,
                  min_numeric: Optional[pulumi.Input[int]] = None,
                  min_special: Optional[pulumi.Input[int]] = None,
                  min_upper: Optional[pulumi.Input[int]] = None,
                  number: Optional[pulumi.Input[bool]] = None,
+                 numeric: Optional[pulumi.Input[bool]] = None,
                  override_special: Optional[pulumi.Input[str]] = None,
                  result: Optional[pulumi.Input[str]] = None,
                  special: Optional[pulumi.Input[bool]] = None,
                  upper: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering RandomString resources.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] length: The length of the string desired
-        :param pulumi.Input[bool] lower: (default true) Include lowercase alphabet characters
-               in random string.
-        :param pulumi.Input[int] min_lower: (default 0) Minimum number of lowercase alphabet
-               characters in random string.
-        :param pulumi.Input[int] min_numeric: (default 0) Minimum number of numeric characters
-               in random string.
-        :param pulumi.Input[int] min_special: (default 0) Minimum number of special characters
-               in random string.
-        :param pulumi.Input[int] min_upper: (default 0) Minimum number of uppercase alphabet
-               characters in random string.
-        :param pulumi.Input[bool] number: (default true) Include numeric characters in random
-               string.
-        :param pulumi.Input[str] override_special: Supply your own list of special characters to
-               use for string generation.  This overrides the default character list in the special
-               argument.  The special argument must still be set to true for any overwritten
-               characters to be used in generation.
-        :param pulumi.Input[str] result: Random string generated.
-        :param pulumi.Input[bool] special: (default true) Include special characters in random
-               string. These are `!@#$%&*()-_=+[]{}<>:?`
-        :param pulumi.Input[bool] upper: (default true) Include uppercase alphabet characters
-               in random string.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] length: The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
+        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result. Default value is `true`.
+        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_special: Minimum number of special characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[bool] number: Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
+        :param pulumi.Input[bool] numeric: Include numeric characters in the result. Default value is `true`.
+        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
+        :param pulumi.Input[str] result: The generated random string.
+        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
+        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result. Default value is `true`.
         """
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if length is not None:
             pulumi.set(__self__, "length", length)
         if lower is not None:
             pulumi.set(__self__, "lower", lower)
@@ -274,209 +256,210 @@
         if min_numeric is not None:
             pulumi.set(__self__, "min_numeric", min_numeric)
         if min_special is not None:
             pulumi.set(__self__, "min_special", min_special)
         if min_upper is not None:
             pulumi.set(__self__, "min_upper", min_upper)
         if number is not None:
+            warnings.warn("""**NOTE**: This is deprecated, use `numeric` instead.""", DeprecationWarning)
+            pulumi.log.warn("""number is deprecated: **NOTE**: This is deprecated, use `numeric` instead.""")
+        if number is not None:
             pulumi.set(__self__, "number", number)
+        if numeric is not None:
+            pulumi.set(__self__, "numeric", numeric)
         if override_special is not None:
             pulumi.set(__self__, "override_special", override_special)
         if result is not None:
             pulumi.set(__self__, "result", result)
         if special is not None:
             pulumi.set(__self__, "special", special)
         if upper is not None:
             pulumi.set(__self__, "upper", upper)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def length(self) -> Optional[pulumi.Input[int]]:
         """
-        The length of the string desired
+        The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
         """
         return pulumi.get(self, "length")
 
     @length.setter
     def length(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "length", value)
 
     @property
     @pulumi.getter
     def lower(self) -> Optional[pulumi.Input[bool]]:
         """
-        (default true) Include lowercase alphabet characters
-        in random string.
+        Include lowercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "lower")
 
     @lower.setter
     def lower(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "lower", value)
 
     @property
     @pulumi.getter(name="minLower")
     def min_lower(self) -> Optional[pulumi.Input[int]]:
         """
-        (default 0) Minimum number of lowercase alphabet
-        characters in random string.
+        Minimum number of lowercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_lower")
 
     @min_lower.setter
     def min_lower(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_lower", value)
 
     @property
     @pulumi.getter(name="minNumeric")
     def min_numeric(self) -> Optional[pulumi.Input[int]]:
         """
-        (default 0) Minimum number of numeric characters
-        in random string.
+        Minimum number of numeric characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_numeric")
 
     @min_numeric.setter
     def min_numeric(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_numeric", value)
 
     @property
     @pulumi.getter(name="minSpecial")
     def min_special(self) -> Optional[pulumi.Input[int]]:
         """
-        (default 0) Minimum number of special characters
-        in random string.
+        Minimum number of special characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_special")
 
     @min_special.setter
     def min_special(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_special", value)
 
     @property
     @pulumi.getter(name="minUpper")
     def min_upper(self) -> Optional[pulumi.Input[int]]:
         """
-        (default 0) Minimum number of uppercase alphabet
-        characters in random string.
+        Minimum number of uppercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_upper")
 
     @min_upper.setter
     def min_upper(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "min_upper", value)
 
     @property
     @pulumi.getter
     def number(self) -> Optional[pulumi.Input[bool]]:
         """
-        (default true) Include numeric characters in random
-        string.
+        Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
         """
         return pulumi.get(self, "number")
 
     @number.setter
     def number(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "number", value)
 
     @property
+    @pulumi.getter
+    def numeric(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Include numeric characters in the result. Default value is `true`.
+        """
+        return pulumi.get(self, "numeric")
+
+    @numeric.setter
+    def numeric(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "numeric", value)
+
+    @property
     @pulumi.getter(name="overrideSpecial")
     def override_special(self) -> Optional[pulumi.Input[str]]:
         """
-        Supply your own list of special characters to
-        use for string generation.  This overrides the default character list in the special
-        argument.  The special argument must still be set to true for any overwritten
-        characters to be used in generation.
+        Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
         """
         return pulumi.get(self, "override_special")
 
     @override_special.setter
     def override_special(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "override_special", value)
 
     @property
     @pulumi.getter
     def result(self) -> Optional[pulumi.Input[str]]:
         """
-        Random string generated.
+        The generated random string.
         """
         return pulumi.get(self, "result")
 
     @result.setter
     def result(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "result", value)
 
     @property
     @pulumi.getter
     def special(self) -> Optional[pulumi.Input[bool]]:
         """
-        (default true) Include special characters in random
-        string. These are `!@#$%&*()-_=+[]{}<>:?`
+        Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
         """
         return pulumi.get(self, "special")
 
     @special.setter
     def special(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "special", value)
 
     @property
     @pulumi.getter
     def upper(self) -> Optional[pulumi.Input[bool]]:
         """
-        (default true) Include uppercase alphabet characters
-        in random string.
+        Include uppercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "upper")
 
     @upper.setter
     def upper(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "upper", value)
 
 
 class RandomString(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  lower: Optional[pulumi.Input[bool]] = None,
                  min_lower: Optional[pulumi.Input[int]] = None,
                  min_numeric: Optional[pulumi.Input[int]] = None,
                  min_special: Optional[pulumi.Input[int]] = None,
                  min_upper: Optional[pulumi.Input[int]] = None,
                  number: Optional[pulumi.Input[bool]] = None,
+                 numeric: Optional[pulumi.Input[bool]] = None,
                  override_special: Optional[pulumi.Input[str]] = None,
                  special: Optional[pulumi.Input[bool]] = None,
                  upper: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         """
-        The resource `RandomString` generates a random permutation of alphanumeric
-        characters and optionally special characters.
+        The resource `RandomString` generates a random permutation of alphanumeric characters and optionally special characters.
 
         This resource *does* use a cryptographic random number generator.
 
-        Historically this resource's intended usage has been ambiguous as the original example
-        used it in a password. For backwards compatibility it will
-        continue to exist. For unique ids please use random_id, for sensitive
-        random values please use random_password.
+        Historically this resource's intended usage has been ambiguous as the original example used it in a password. For backwards compatibility it will continue to exist. For unique ids please use random_id, for sensitive random values please use random_password.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_random as random
 
@@ -484,63 +467,97 @@
             length=16,
             override_special="/@£$",
             special=True)
         ```
 
         ## Import
 
-        Strings can be imported by just specifying the value of the string
+        ### Avoiding Replacement
 
         ```sh
-         $ pulumi import random:index/randomString:RandomString test test
+         $ pulumi import random:index/randomString:RandomString If the resource were imported using `random_string.test test`,
         ```
 
+         replacement can be avoided by using1. Attribute values that match the imported ID and defaults:
+
+         terraform
+
+         resource "random_string" "test" {
+
+         length = 4
+
+         lower
+
+        = true
+
+         } 2. Attribute values that match the imported ID and omit the attributes with defaults:
+
+         terraform
+
+         resource "random_string" "test" {
+
+         length = 4
+
+         } 3. `ignore_changes` specifying the attributes to ignore:
+
+         terraform
+
+         resource "random_string" "test" {
+
+         length = 16
+
+         lower
+
+        = false
+
+         lifecycle {
+
+         ignore_changes = [
+
+         length,
+
+         lower,
+
+         ]
+
+         }
+
+         }
+
+         **NOTE** `ignore_changes` is only required until the resource is recreated after import,
+
+         after which it will use the configuration values specified.
+
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] length: The length of the string desired
-        :param pulumi.Input[bool] lower: (default true) Include lowercase alphabet characters
-               in random string.
-        :param pulumi.Input[int] min_lower: (default 0) Minimum number of lowercase alphabet
-               characters in random string.
-        :param pulumi.Input[int] min_numeric: (default 0) Minimum number of numeric characters
-               in random string.
-        :param pulumi.Input[int] min_special: (default 0) Minimum number of special characters
-               in random string.
-        :param pulumi.Input[int] min_upper: (default 0) Minimum number of uppercase alphabet
-               characters in random string.
-        :param pulumi.Input[bool] number: (default true) Include numeric characters in random
-               string.
-        :param pulumi.Input[str] override_special: Supply your own list of special characters to
-               use for string generation.  This overrides the default character list in the special
-               argument.  The special argument must still be set to true for any overwritten
-               characters to be used in generation.
-        :param pulumi.Input[bool] special: (default true) Include special characters in random
-               string. These are `!@#$%&*()-_=+[]{}<>:?`
-        :param pulumi.Input[bool] upper: (default true) Include uppercase alphabet characters
-               in random string.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] length: The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
+        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result. Default value is `true`.
+        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_special: Minimum number of special characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[bool] number: Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
+        :param pulumi.Input[bool] numeric: Include numeric characters in the result. Default value is `true`.
+        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
+        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
+        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result. Default value is `true`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: RandomStringArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The resource `RandomString` generates a random permutation of alphanumeric
-        characters and optionally special characters.
+        The resource `RandomString` generates a random permutation of alphanumeric characters and optionally special characters.
 
         This resource *does* use a cryptographic random number generator.
 
-        Historically this resource's intended usage has been ambiguous as the original example
-        used it in a password. For backwards compatibility it will
-        continue to exist. For unique ids please use random_id, for sensitive
-        random values please use random_password.
+        Historically this resource's intended usage has been ambiguous as the original example used it in a password. For backwards compatibility it will continue to exist. For unique ids please use random_id, for sensitive random values please use random_password.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_random as random
 
@@ -548,20 +565,70 @@
             length=16,
             override_special="/@£$",
             special=True)
         ```
 
         ## Import
 
-        Strings can be imported by just specifying the value of the string
+        ### Avoiding Replacement
 
         ```sh
-         $ pulumi import random:index/randomString:RandomString test test
+         $ pulumi import random:index/randomString:RandomString If the resource were imported using `random_string.test test`,
         ```
 
+         replacement can be avoided by using1. Attribute values that match the imported ID and defaults:
+
+         terraform
+
+         resource "random_string" "test" {
+
+         length = 4
+
+         lower
+
+        = true
+
+         } 2. Attribute values that match the imported ID and omit the attributes with defaults:
+
+         terraform
+
+         resource "random_string" "test" {
+
+         length = 4
+
+         } 3. `ignore_changes` specifying the attributes to ignore:
+
+         terraform
+
+         resource "random_string" "test" {
+
+         length = 16
+
+         lower
+
+        = false
+
+         lifecycle {
+
+         ignore_changes = [
+
+         length,
+
+         lower,
+
+         ]
+
+         }
+
+         }
+
+         **NOTE** `ignore_changes` is only required until the resource is recreated after import,
+
+         after which it will use the configuration values specified.
+
         :param str resource_name: The name of the resource.
         :param RandomStringArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(RandomStringArgs, pulumi.ResourceOptions, *args, **kwargs)
@@ -569,22 +636,23 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  length: Optional[pulumi.Input[int]] = None,
                  lower: Optional[pulumi.Input[bool]] = None,
                  min_lower: Optional[pulumi.Input[int]] = None,
                  min_numeric: Optional[pulumi.Input[int]] = None,
                  min_special: Optional[pulumi.Input[int]] = None,
                  min_upper: Optional[pulumi.Input[int]] = None,
                  number: Optional[pulumi.Input[bool]] = None,
+                 numeric: Optional[pulumi.Input[bool]] = None,
                  override_special: Optional[pulumi.Input[str]] = None,
                  special: Optional[pulumi.Input[bool]] = None,
                  upper: Optional[pulumi.Input[bool]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -598,194 +666,183 @@
                 raise TypeError("Missing required property 'length'")
             __props__.__dict__["length"] = length
             __props__.__dict__["lower"] = lower
             __props__.__dict__["min_lower"] = min_lower
             __props__.__dict__["min_numeric"] = min_numeric
             __props__.__dict__["min_special"] = min_special
             __props__.__dict__["min_upper"] = min_upper
+            if number is not None and not opts.urn:
+                warnings.warn("""**NOTE**: This is deprecated, use `numeric` instead.""", DeprecationWarning)
+                pulumi.log.warn("""number is deprecated: **NOTE**: This is deprecated, use `numeric` instead.""")
             __props__.__dict__["number"] = number
+            __props__.__dict__["numeric"] = numeric
             __props__.__dict__["override_special"] = override_special
             __props__.__dict__["special"] = special
             __props__.__dict__["upper"] = upper
             __props__.__dict__["result"] = None
         super(RandomString, __self__).__init__(
             'random:index/randomString:RandomString',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+            keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             length: Optional[pulumi.Input[int]] = None,
             lower: Optional[pulumi.Input[bool]] = None,
             min_lower: Optional[pulumi.Input[int]] = None,
             min_numeric: Optional[pulumi.Input[int]] = None,
             min_special: Optional[pulumi.Input[int]] = None,
             min_upper: Optional[pulumi.Input[int]] = None,
             number: Optional[pulumi.Input[bool]] = None,
+            numeric: Optional[pulumi.Input[bool]] = None,
             override_special: Optional[pulumi.Input[str]] = None,
             result: Optional[pulumi.Input[str]] = None,
             special: Optional[pulumi.Input[bool]] = None,
             upper: Optional[pulumi.Input[bool]] = None) -> 'RandomString':
         """
         Get an existing RandomString resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new id to be generated. See
-               the main provider documentation for more information.
-        :param pulumi.Input[int] length: The length of the string desired
-        :param pulumi.Input[bool] lower: (default true) Include lowercase alphabet characters
-               in random string.
-        :param pulumi.Input[int] min_lower: (default 0) Minimum number of lowercase alphabet
-               characters in random string.
-        :param pulumi.Input[int] min_numeric: (default 0) Minimum number of numeric characters
-               in random string.
-        :param pulumi.Input[int] min_special: (default 0) Minimum number of special characters
-               in random string.
-        :param pulumi.Input[int] min_upper: (default 0) Minimum number of uppercase alphabet
-               characters in random string.
-        :param pulumi.Input[bool] number: (default true) Include numeric characters in random
-               string.
-        :param pulumi.Input[str] override_special: Supply your own list of special characters to
-               use for string generation.  This overrides the default character list in the special
-               argument.  The special argument must still be set to true for any overwritten
-               characters to be used in generation.
-        :param pulumi.Input[str] result: Random string generated.
-        :param pulumi.Input[bool] special: (default true) Include special characters in random
-               string. These are `!@#$%&*()-_=+[]{}<>:?`
-        :param pulumi.Input[bool] upper: (default true) Include uppercase alphabet characters
-               in random string.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
+        :param pulumi.Input[int] length: The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
+        :param pulumi.Input[bool] lower: Include lowercase alphabet characters in the result. Default value is `true`.
+        :param pulumi.Input[int] min_lower: Minimum number of lowercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_numeric: Minimum number of numeric characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_special: Minimum number of special characters in the result. Default value is `0`.
+        :param pulumi.Input[int] min_upper: Minimum number of uppercase alphabet characters in the result. Default value is `0`.
+        :param pulumi.Input[bool] number: Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
+        :param pulumi.Input[bool] numeric: Include numeric characters in the result. Default value is `true`.
+        :param pulumi.Input[str] override_special: Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
+        :param pulumi.Input[str] result: The generated random string.
+        :param pulumi.Input[bool] special: Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
+        :param pulumi.Input[bool] upper: Include uppercase alphabet characters in the result. Default value is `true`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RandomStringState.__new__(_RandomStringState)
 
         __props__.__dict__["keepers"] = keepers
         __props__.__dict__["length"] = length
         __props__.__dict__["lower"] = lower
         __props__.__dict__["min_lower"] = min_lower
         __props__.__dict__["min_numeric"] = min_numeric
         __props__.__dict__["min_special"] = min_special
         __props__.__dict__["min_upper"] = min_upper
         __props__.__dict__["number"] = number
+        __props__.__dict__["numeric"] = numeric
         __props__.__dict__["override_special"] = override_special
         __props__.__dict__["result"] = result
         __props__.__dict__["special"] = special
         __props__.__dict__["upper"] = upper
         return RandomString(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def keepers(self) -> pulumi.Output[Optional[Mapping[str, Any]]]:
+    def keepers(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new id to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @property
     @pulumi.getter
     def length(self) -> pulumi.Output[int]:
         """
-        The length of the string desired
+        The length of the string desired. The minimum value for length is 1 and, length must also be >= (`min_upper` + `min_lower` + `min_numeric` + `min_special`).
         """
         return pulumi.get(self, "length")
 
     @property
     @pulumi.getter
-    def lower(self) -> pulumi.Output[Optional[bool]]:
+    def lower(self) -> pulumi.Output[bool]:
         """
-        (default true) Include lowercase alphabet characters
-        in random string.
+        Include lowercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "lower")
 
     @property
     @pulumi.getter(name="minLower")
-    def min_lower(self) -> pulumi.Output[Optional[int]]:
+    def min_lower(self) -> pulumi.Output[int]:
         """
-        (default 0) Minimum number of lowercase alphabet
-        characters in random string.
+        Minimum number of lowercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_lower")
 
     @property
     @pulumi.getter(name="minNumeric")
-    def min_numeric(self) -> pulumi.Output[Optional[int]]:
+    def min_numeric(self) -> pulumi.Output[int]:
         """
-        (default 0) Minimum number of numeric characters
-        in random string.
+        Minimum number of numeric characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_numeric")
 
     @property
     @pulumi.getter(name="minSpecial")
-    def min_special(self) -> pulumi.Output[Optional[int]]:
+    def min_special(self) -> pulumi.Output[int]:
         """
-        (default 0) Minimum number of special characters
-        in random string.
+        Minimum number of special characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_special")
 
     @property
     @pulumi.getter(name="minUpper")
-    def min_upper(self) -> pulumi.Output[Optional[int]]:
+    def min_upper(self) -> pulumi.Output[int]:
         """
-        (default 0) Minimum number of uppercase alphabet
-        characters in random string.
+        Minimum number of uppercase alphabet characters in the result. Default value is `0`.
         """
         return pulumi.get(self, "min_upper")
 
     @property
     @pulumi.getter
-    def number(self) -> pulumi.Output[Optional[bool]]:
+    def number(self) -> pulumi.Output[bool]:
         """
-        (default true) Include numeric characters in random
-        string.
+        Include numeric characters in the result. Default value is `true`. **NOTE**: This is deprecated, use `numeric` instead.
         """
         return pulumi.get(self, "number")
 
     @property
+    @pulumi.getter
+    def numeric(self) -> pulumi.Output[bool]:
+        """
+        Include numeric characters in the result. Default value is `true`.
+        """
+        return pulumi.get(self, "numeric")
+
+    @property
     @pulumi.getter(name="overrideSpecial")
     def override_special(self) -> pulumi.Output[Optional[str]]:
         """
-        Supply your own list of special characters to
-        use for string generation.  This overrides the default character list in the special
-        argument.  The special argument must still be set to true for any overwritten
-        characters to be used in generation.
+        Supply your own list of special characters to use for string generation.  This overrides the default character list in the special argument.  The `special` argument must still be set to true for any overwritten characters to be used in generation.
         """
         return pulumi.get(self, "override_special")
 
     @property
     @pulumi.getter
     def result(self) -> pulumi.Output[str]:
         """
-        Random string generated.
+        The generated random string.
         """
         return pulumi.get(self, "result")
 
     @property
     @pulumi.getter
-    def special(self) -> pulumi.Output[Optional[bool]]:
+    def special(self) -> pulumi.Output[bool]:
         """
-        (default true) Include special characters in random
-        string. These are `!@#$%&*()-_=+[]{}<>:?`
+        Include special characters in the result. These are `!@#$%&*()-_=+[]{}<>:?`. Default value is `true`.
         """
         return pulumi.get(self, "special")
 
     @property
     @pulumi.getter
-    def upper(self) -> pulumi.Output[Optional[bool]]:
+    def upper(self) -> pulumi.Output[bool]:
         """
-        (default true) Include uppercase alphabet characters
-        in random string.
+        Include uppercase alphabet characters in the result. Default value is `true`.
         """
         return pulumi.get(self, "upper")
```

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random/random_uuid.py` & `pulumi_random-4.9.0a1674773801/pulumi_random/random_uuid.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,68 +10,60 @@
 from . import _utilities
 
 __all__ = ['RandomUuidArgs', 'RandomUuid']
 
 @pulumi.input_type
 class RandomUuidArgs:
     def __init__(__self__, *,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None):
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a RandomUuid resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new uuid to be generated. See
-               the main provider documentation for more information.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new uuid to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
 
 @pulumi.input_type
 class _RandomUuidState:
     def __init__(__self__, *,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  result: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering RandomUuid resources.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new uuid to be generated. See
-               the main provider documentation for more information.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         :param pulumi.Input[str] result: The generated uuid presented in string format.
         """
         if keepers is not None:
             pulumi.set(__self__, "keepers", keepers)
         if result is not None:
             pulumi.set(__self__, "result", result)
 
     @property
     @pulumi.getter
-    def keepers(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
+    def keepers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new uuid to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @keepers.setter
-    def keepers(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
+    def keepers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "keepers", value)
 
     @property
     @pulumi.getter
     def result(self) -> Optional[pulumi.Input[str]]:
         """
         The generated uuid presented in string format.
@@ -84,79 +76,69 @@
 
 
 class RandomUuid(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         """
-        The resource `RandomUuid` generates random uuid string that is intended to be
-        used as unique identifiers for other resources.
+        The resource `RandomUuid` generates random uuid string that is intended to be used as unique identifiers for other resources.
 
-        This resource uses the `hashicorp/go-uuid` to generate a UUID-formatted string
-        for use with services needed a unique string identifier.
+        This resource uses [hashicorp/go-uuid](https://github.com/hashicorp/go-uuid) to generate a UUID-formatted string for use with services needed a unique string identifier.
 
         ## Example Usage
 
-        The following example shows how to generate a unique name for an Azure Resource Group.
-
         ```python
         import pulumi
         import pulumi_azure as azure
         import pulumi_random as random
 
         test_random_uuid = random.RandomUuid("testRandomUuid")
         test_resource_group = azure.core.ResourceGroup("testResourceGroup", location="Central US")
         ```
 
         ## Import
 
-        Random UUID's can be imported. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example
+        Random UUID's can be imported. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs.
 
         ```sh
          $ pulumi import random:index/randomUuid:RandomUuid main aabbccdd-eeff-0011-2233-445566778899
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new uuid to be generated. See
-               the main provider documentation for more information.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[RandomUuidArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The resource `RandomUuid` generates random uuid string that is intended to be
-        used as unique identifiers for other resources.
+        The resource `RandomUuid` generates random uuid string that is intended to be used as unique identifiers for other resources.
 
-        This resource uses the `hashicorp/go-uuid` to generate a UUID-formatted string
-        for use with services needed a unique string identifier.
+        This resource uses [hashicorp/go-uuid](https://github.com/hashicorp/go-uuid) to generate a UUID-formatted string for use with services needed a unique string identifier.
 
         ## Example Usage
 
-        The following example shows how to generate a unique name for an Azure Resource Group.
-
         ```python
         import pulumi
         import pulumi_azure as azure
         import pulumi_random as random
 
         test_random_uuid = random.RandomUuid("testRandomUuid")
         test_resource_group = azure.core.ResourceGroup("testResourceGroup", location="Central US")
         ```
 
         ## Import
 
-        Random UUID's can be imported. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs. Example
+        Random UUID's can be imported. This can be used to replace a config value with a value interpolated from the random provider without experiencing diffs.
 
         ```sh
          $ pulumi import random:index/randomUuid:RandomUuid main aabbccdd-eeff-0011-2233-445566778899
         ```
 
         :param str resource_name: The name of the resource.
         :param RandomUuidArgs args: The arguments to use to populate this resource's properties.
@@ -169,15 +151,15 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+                 keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
@@ -191,43 +173,39 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            keepers: Optional[pulumi.Input[Mapping[str, Any]]] = None,
+            keepers: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
             result: Optional[pulumi.Input[str]] = None) -> 'RandomUuid':
         """
         Get an existing RandomUuid resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[Mapping[str, Any]] keepers: Arbitrary map of values that, when changed, will
-               trigger a new uuid to be generated. See
-               the main provider documentation for more information.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] keepers: Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         :param pulumi.Input[str] result: The generated uuid presented in string format.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _RandomUuidState.__new__(_RandomUuidState)
 
         __props__.__dict__["keepers"] = keepers
         __props__.__dict__["result"] = result
         return RandomUuid(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def keepers(self) -> pulumi.Output[Optional[Mapping[str, Any]]]:
+    def keepers(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
-        Arbitrary map of values that, when changed, will
-        trigger a new uuid to be generated. See
-        the main provider documentation for more information.
+        Arbitrary map of values that, when changed, will trigger recreation of resource. See the main provider documentation for more information.
         """
         return pulumi.get(self, "keepers")
 
     @property
     @pulumi.getter
     def result(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random.egg-info/PKG-INFO` & `pulumi_random-4.9.0a1674773801/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pulumi-random
-Version: 4.9.0a1673556316
+Name: pulumi_random
+Version: 4.9.0a1674773801
 Summary: A Pulumi package to safely use randomness in Pulumi programs.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-random
 Keywords: pulumi random
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_random-4.9.0a1673556316/pulumi_random.egg-info/SOURCES.txt` & `pulumi_random-4.9.0a1674773801/pulumi_random.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_random-4.9.0a1673556316/setup.py` & `pulumi_random-4.9.0a1674773801/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.9.0a1673556316"
-PLUGIN_VERSION = "4.9.0-alpha.1673556316+20991696"
+VERSION = "4.9.0a1674773801"
+PLUGIN_VERSION = "4.9.0-alpha.1674773801+6bcc9089"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'random', PLUGIN_VERSION])
         except OSError as error:
```

