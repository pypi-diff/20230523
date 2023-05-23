# Comparing `tmp/cloudbender-0.9.8-py2.py3-none-any.whl.zip` & `tmp/cloudbender-0.9.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 35018 bytes, number of entries: 21
--rw-r--r--  2.0 unx      414 b- defN 21-Feb-22 18:36 cloudbender/__init__.py
--rw-r--r--  2.0 unx     8146 b- defN 20-Sep-22 11:30 cloudbender/cli.py
+Zip file size: 35314 bytes, number of entries: 21
+-rw-r--r--  2.0 unx      414 b- defN 21-Mar-11 18:18 cloudbender/__init__.py
+-rw-r--r--  2.0 unx     8194 b- defN 21-Mar-11 16:04 cloudbender/cli.py
 -rw-r--r--  2.0 unx     2468 b- defN 20-Sep-22 11:30 cloudbender/connection.py
 -rw-r--r--  2.0 unx     3712 b- defN 20-Sep-22 11:30 cloudbender/core.py
--rw-r--r--  2.0 unx      256 b- defN 20-Sep-22 11:30 cloudbender/exceptions.py
+-rw-r--r--  2.0 unx      317 b- defN 21-Mar-11 18:05 cloudbender/exceptions.py
 -rw-r--r--  2.0 unx     1216 b- defN 21-Feb-22 15:04 cloudbender/hooks.py
 -rw-r--r--  2.0 unx     8677 b- defN 20-Dec-28 17:11 cloudbender/jinja.py
--rw-r--r--  2.0 unx    31023 b- defN 21-Feb-22 18:31 cloudbender/stack.py
+-rw-r--r--  2.0 unx    32006 b- defN 21-Mar-11 18:18 cloudbender/stack.py
 -rw-r--r--  2.0 unx     3891 b- defN 20-Sep-22 11:30 cloudbender/stackgroup.py
 -rw-r--r--  2.0 unx     2776 b- defN 20-Sep-22 11:30 cloudbender/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Sep-22 11:30 cloudbender/templates/__init__.py
 -rw-r--r--  2.0 unx      127 b- defN 20-Sep-22 11:30 cloudbender/templates/outputs.yaml
 -rw-r--r--  2.0 unx     1192 b- defN 20-Sep-22 11:30 cloudbender/templates/stack-doc.md
 -rw-r--r--  2.0 unx        0 b- defN 19-Jul-14 19:50 tests/__init__.py
 -rw-r--r--  2.0 unx      375 b- defN 19-Jul-14 19:50 tests/test_utils.py
--rw-r--r--  2.0 unx    34354 b- defN 21-Feb-22 18:38 cloudbender-0.9.8.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     2488 b- defN 21-Feb-22 18:38 cloudbender-0.9.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 21-Feb-22 18:38 cloudbender-0.9.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 21-Feb-22 18:38 cloudbender-0.9.8.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       18 b- defN 21-Feb-22 18:38 cloudbender-0.9.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1708 b- defN 21-Feb-22 18:38 cloudbender-0.9.8.dist-info/RECORD
-21 files, 103004 bytes uncompressed, 32244 bytes compressed:  68.7%
+-rw-r--r--  2.0 unx    34354 b- defN 21-Mar-11 18:19 cloudbender-0.9.9.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     2488 b- defN 21-Mar-11 18:19 cloudbender-0.9.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 21-Mar-11 18:19 cloudbender-0.9.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       53 b- defN 21-Mar-11 18:19 cloudbender-0.9.9.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       18 b- defN 21-Mar-11 18:19 cloudbender-0.9.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1708 b- defN 21-Mar-11 18:19 cloudbender-0.9.9.dist-info/RECORD
+21 files, 104096 bytes uncompressed, 32540 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -39,26 +39,26 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_utils.py
 Comment: 
 
-Filename: cloudbender-0.9.8.dist-info/LICENSE.md
+Filename: cloudbender-0.9.9.dist-info/LICENSE.md
 Comment: 
 
-Filename: cloudbender-0.9.8.dist-info/METADATA
+Filename: cloudbender-0.9.9.dist-info/METADATA
 Comment: 
 
-Filename: cloudbender-0.9.8.dist-info/WHEEL
+Filename: cloudbender-0.9.9.dist-info/WHEEL
 Comment: 
 
-Filename: cloudbender-0.9.8.dist-info/entry_points.txt
+Filename: cloudbender-0.9.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: cloudbender-0.9.8.dist-info/top_level.txt
+Filename: cloudbender-0.9.9.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudbender-0.9.8.dist-info/RECORD
+Filename: cloudbender-0.9.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloudbender/__init__.py

```diff
@@ -1,12 +1,12 @@
 import logging
 
 __author__ = "Stefan Reimer"
 __email__ = "stefan@zero-downtimet.net"
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 
 # Set up logging to ``/dev/null`` like a library is supposed to.
 # http://docs.python.org/3.3/howto/logging.html#configuring-logging-for-a-library
 class NullHandler(logging.Handler):  # pragma: no cover
     def emit(self, record):
         pass
```

## cloudbender/cli.py

```diff
@@ -74,15 +74,17 @@
 @click.option("--multi", is_flag=True, help="Allow more than one stack to match")
 @click.pass_obj
 def validate(cb, stack_names, multi):
     """ Validates already rendered templates using cfn-lint """
     stacks = _find_stacks(cb, stack_names, multi)
 
     for s in stacks:
-        s.validate()
+        ret = s.validate()
+        if ret:
+            sys.exit(ret)
 
 
 @click.command()
 @click.argument("stack_names", nargs=-1)
 @click.option("--multi", is_flag=True, help="Allow more than one stack to match")
 @click.option("--include", default='.*', help="regex matching wanted outputs, default '.*'")
 @click.option("--values", is_flag=True, help="Only output values, most useful if only one outputs is returned")
```

## cloudbender/exceptions.py

```diff
@@ -8,7 +8,11 @@
 
 class InvalidProjectDir(Exception):
     """My documentation"""
 
 
 class InvalidHook(Exception):
     """My documentation"""
+
+
+class ChecksumError(Exception):
+    """My documentation"""
```

## cloudbender/stack.py

```diff
@@ -11,15 +11,15 @@
 
 from botocore.exceptions import ClientError
 
 from .utils import dict_merge, search_refs, ensure_dir, get_s3_url
 from .connection import BotoConnection
 from .jinja import JinjaEnv, read_config_file
 from . import __version__
-from .exceptions import ParameterNotFound, ParameterIllegalValue
+from .exceptions import ParameterNotFound, ParameterIllegalValue, ChecksumError
 from .hooks import exec_hooks
 
 import cfnlint.core
 import cfnlint.template
 import cfnlint.graph
 
 try:
@@ -105,15 +105,15 @@
         # Inject Artifact if not explicitly set
         if 'Artifact' not in self.tags:
             self.tags['Artifact'] = self.provides
 
         if 'options' in _config:
             self.options = dict_merge(self.options, _config['options'])
 
-        if 'Mode' in self.options:
+        if 'Mode' in self.options and self.options['Mode'] == 'Piped':
             self.mode = self.options['Mode']
 
         if 'StoreOutputs' in self.options and self.options['StoreOutputs']:
             self.store_outputs = True
 
         if 'dependencies' in _config:
             for dep in _config['dependencies']:
@@ -203,14 +203,28 @@
         # Extract dependencies
         try:
             for dep in self.cfn_data['Metadata']['CloudBender']['Dependencies']:
                 self.dependencies.add(dep)
         except KeyError:
             pass
 
+        # Get checksum
+        if not self.md5:
+            try:
+                self.md5 = self.cfn_data['Metadata']['Template']['Hash']
+
+                # Verify embedded md5 hash
+                source_cfn = re.sub('Hash: [0-9a-f]{32}', 'Hash: __HASH__', self.cfn_template)
+                our_md5 = hashlib.md5(source_cfn.encode('utf-8')).hexdigest()
+                if (our_md5 != self.md5):
+                    raise ChecksumError("Template hash checksum mismatch! Expected: {} Got: {}".format(self.md5, our_md5)) from None
+
+            except KeyError:
+                raise ChecksumError("Template missing Hash checksum!") from None
+
         # Add CloudBender dependencies
         include = []
         search_refs(self.cfn_data, include, self.mode)
         for ref in include:
             if self.mode != "Piped":
                 self.dependencies.add(ref.split('.')[0])
             else:
@@ -311,14 +325,15 @@
                         logger.debug('Read cfn template %s.', yaml_file)
                 except FileNotFoundError as e:
                     logger.warn("Could not find template file: {}".format(yaml_file))
                     raise e
 
             self.cfn_data = yaml.load(self.cfn_template, Loader=SafeLoaderIgnoreUnknown)
             self._parse_metadata()
+
         else:
             logger.debug('Using cached cfn template %s.', self.stackname)
 
     def validate(self):
         """Validates the rendered template via cfn-lint"""
         self.read_template_file()
 
@@ -342,21 +357,28 @@
         if ignore_checks:
             lint_args.append('--ignore-checks')
             lint_args = lint_args + ignore_checks
             logger.info('Ignoring checks: {}'.format(','.join(ignore_checks)))
 
         (args, filenames, formatter) = cfnlint.core.get_args_filenames(lint_args)
         (template, rules, matches) = cfnlint.core.get_template_rules(filename, args)
+
+        region = self.region
+        if region == 'global':
+            region = 'us-east-1'
+
         if not matches:
-            matches.extend(cfnlint.core.run_checks(filename, template, rules, [self.region]))
+            matches.extend(cfnlint.core.run_checks(filename, template, rules, [region]))
         if len(matches):
             for match in matches:
                 logger.error(formatter._format(match))
+            return 1
         else:
             logger.info("Passed.")
+            return 0
 
     def get_outputs(self, include='.*', values=False):
         """ gets outputs of the stack """
 
         self.read_template_file()
         try:
             stacks = self.connection_manager.call(
@@ -757,12 +779,16 @@
 
     def _add_template_arg(self, kwargs):
         if self.template_bucket_url:
             # https://bucket-name.s3.Region.amazonaws.com/key name
             # so we need the region, AWS as usual
             (bucket, path) = get_s3_url(self.template_bucket_url, self.rel_path, self.stackname + ".yaml")
             bucket_region = self.connection_manager.call('s3', 'get_bucket_location', {'Bucket': bucket}, profile=self.profile, region=self.region)['LocationConstraint']
+            # If bucket is in us-east-1 AWS returns 'none' cause reasons grrr
+            if not bucket_region:
+                bucket_region = 'us-east-1'
+
             kwargs['TemplateURL'] = 'https://{}.s3.{}.amazonaws.com/{}'.format(bucket, bucket_region, path)
         else:
             kwargs['TemplateBody'] = self.cfn_template
 
         return kwargs
```

## Comparing `cloudbender-0.9.8.dist-info/LICENSE.md` & `cloudbender-0.9.9.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `cloudbender-0.9.8.dist-info/METADATA` & `cloudbender-0.9.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudbender
-Version: 0.9.8
+Version: 0.9.9
 Summary: Toolset to render and manage AWS Cloudformation
 Home-page: https://git.zero-downtime.net/ZeroDownTime/CloudBender
 Author: Stefan Reimer
 Author-email: stefan@zero-downtime.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

## Comparing `cloudbender-0.9.8.dist-info/RECORD` & `cloudbender-0.9.9.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-cloudbender/__init__.py,sha256=e-bBSzUYT4_otfc9ARXoPBujsUwXqWPR_bgBsH9ejTo,414
-cloudbender/cli.py,sha256=fwUw0Nvp_azcZIc65UpWNJ4p3Gj3Hb7jo_l-JvbdDfM,8146
+cloudbender/__init__.py,sha256=-oFl_jkNM9YgMZwL3JPzg7BY3VxlhUYHSlULr-YhZG4,414
+cloudbender/cli.py,sha256=FaKZ7XjWGYhcULw4S3KAGrmhwF6uAl5QCxMh6feNd5g,8194
 cloudbender/connection.py,sha256=p1zDMPH7TpzbWFixY3aRnZ0sCOxAsk7pFgogNsVoVw8,2468
 cloudbender/core.py,sha256=NdhAsW3Wdewyx5E_w35uwyBq_DrgwooiV7ITYoQtamY,3712
-cloudbender/exceptions.py,sha256=MpYGTMjI6ZrnYfYrDR7nyrO3liYfgNjBPYAwiaNvm6k,256
+cloudbender/exceptions.py,sha256=cA1sWhy6PRBDJfu5Xu5sX2DV5gtQ6KOZzffPxkdBLnA,317
 cloudbender/hooks.py,sha256=UcWDLMnWccoi7ed_AslpbRFJV5ZSa-y8R8RMdtAI0Ys,1216
 cloudbender/jinja.py,sha256=ANQqemqQ4Q5IAAE8FDh7BSeadoBJ699szk-IieLCQN8,8677
-cloudbender/stack.py,sha256=Ir3Hbl-du24rXFsUCgUQKAOtJTixUO03LytcGtYX3Lw,31023
+cloudbender/stack.py,sha256=MfjOXJFaGp8l3WtosMiPcu5PfbsbUkyp7Pq0N9Wl05Y,32006
 cloudbender/stackgroup.py,sha256=OPIUGtUt-XaRNpztZ7xamQqOF427eg6fVEQLPfMEiqI,3891
 cloudbender/utils.py,sha256=WEZu4utTWU2hT0MKmRRLpTN6LuH8ZPnadnVl1makHik,2776
 cloudbender/templates/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cloudbender/templates/outputs.yaml,sha256=p2QyMuo7k47Ewq0Tg5w2rhYj9YGXineemuj71IpfB7E,127
 cloudbender/templates/stack-doc.md,sha256=S_qLQrZ1xm-YrzAjiV8qPWYVDXDfSuawhW4HjL6N120,1192
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/test_utils.py,sha256=DzqMZsjYdRxxZGRFY9OTGmNkaoOJMqno8F7KniMYtpI,375
-cloudbender-0.9.8.dist-info/LICENSE.md,sha256=MqCnOBu8uXsEOzRZWh9EBVfVz-kE9NkXcLCrtGXo2yU,34354
-cloudbender-0.9.8.dist-info/METADATA,sha256=qdtra4ykeAYzVUjCYG4g6vn7ycsaSjVzztxpq0PGRuQ,2488
-cloudbender-0.9.8.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
-cloudbender-0.9.8.dist-info/entry_points.txt,sha256=HDaDyBlBs1XZne6sPX8NWcavEJPhhGE290rgtJM9aWI,53
-cloudbender-0.9.8.dist-info/top_level.txt,sha256=UuhoCNBJMpxTUaWhVS6EhC9dmaylPdJeDpIIHvaukdE,18
-cloudbender-0.9.8.dist-info/RECORD,,
+cloudbender-0.9.9.dist-info/LICENSE.md,sha256=MqCnOBu8uXsEOzRZWh9EBVfVz-kE9NkXcLCrtGXo2yU,34354
+cloudbender-0.9.9.dist-info/METADATA,sha256=P0Ht_ECMe-J26EFCI8syocPEVwWQxBAWcPrAQa-G7FE,2488
+cloudbender-0.9.9.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
+cloudbender-0.9.9.dist-info/entry_points.txt,sha256=HDaDyBlBs1XZne6sPX8NWcavEJPhhGE290rgtJM9aWI,53
+cloudbender-0.9.9.dist-info/top_level.txt,sha256=UuhoCNBJMpxTUaWhVS6EhC9dmaylPdJeDpIIHvaukdE,18
+cloudbender-0.9.9.dist-info/RECORD,,
```

