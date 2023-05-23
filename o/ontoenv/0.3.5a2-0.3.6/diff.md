# Comparing `tmp/ontoenv-0.3.5a2.tar.gz` & `tmp/ontoenv-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontoenv-0.3.5a2.tar", max compression
+gzip compressed data, was "ontoenv-0.3.6.tar", max compression
```

## Comparing `ontoenv-0.3.5a2.tar` & `ontoenv-0.3.6.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1519 2021-06-05 05:57:22.610687 ontoenv-0.3.5a2/LICENSE
--rw-r--r--   0        0        0    11453 2023-02-14 01:45:19.905094 ontoenv-0.3.5a2/ontoenv/__init__.py
--rw-r--r--   0        0        0     1910 2023-02-14 01:39:47.981943 ontoenv-0.3.5a2/ontoenv/cli.py
--rw-r--r--   0        0        0      529 2023-02-14 01:45:38.025266 ontoenv-0.3.5a2/pyproject.toml
--rw-r--r--   0        0        0      881 1970-01-01 00:00:00.000000 ontoenv-0.3.5a2/setup.py
--rw-r--r--   0        0        0      813 1970-01-01 00:00:00.000000 ontoenv-0.3.5a2/PKG-INFO
+-rw-r--r--   0        0        0     1519 2023-04-20 23:37:22.604572 ontoenv-0.3.6/LICENSE
+-rw-r--r--   0        0        0    11493 2023-05-23 00:33:34.327522 ontoenv-0.3.6/ontoenv/__init__.py
+-rw-r--r--   0        0        0     2065 2023-04-20 23:37:22.605017 ontoenv-0.3.6/ontoenv/cli.py
+-rw-r--r--   0        0        0      527 2023-05-23 00:38:28.702655 ontoenv-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      811 1970-01-01 00:00:00.000000 ontoenv-0.3.6/PKG-INFO
```

### Comparing `ontoenv-0.3.5a2/LICENSE` & `ontoenv-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ontoenv-0.3.5a2/ontoenv/__init__.py` & `ontoenv-0.3.6/ontoenv/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,16 @@
         logging.info(f"Searching for RDF files in {self.oedir.parent}")
         for filename in find_ontology_files(self.oedir.parent):
             self._get_ontology_definition(filename)
         for filename in find_ontology_files(self.oedir.parent):
             self._resolve_imports_from_uri(filename)
 
         # remove old imports/files that are no longer in the mapping
-        for uri, filename in self.mapping.items():
+        mapping_tmp = list(self.mapping.items())
+        for uri, filename in mapping_tmp:
             if not os.path.exists(filename):
                 del self.mapping[uri]
                 self._dependencies.remove_node(uri)
                 logging.info(f"Removed {uri} from mapping")
 
     def _refresh_cache_contents(self):
         self.cache_contents = set()
```

### Comparing `ontoenv-0.3.5a2/ontoenv/cli.py` & `ontoenv-0.3.6/ontoenv/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import sys
 import click
 import logging
 from ontoenv import OntoEnv
 import networkx as nx
-import matplotlib.pyplot as plt
 
 
 @click.group(help="Manage ontology definition mappings")
 @click.option("-v", is_flag=True)
 def i(v):
     if v:
         logging.basicConfig(level=logging.INFO)
@@ -41,22 +41,27 @@
     for ontology, filename in oe.mapping.items():
         print(f"{ontology} => {filename}")
 
 
 @i.command(help="Output dependency graph")
 @click.argument("output_filename", default="dependencies.pdf")
 def output(output_filename):
+    try:
+        import matplotlib.pyplot as plt
+    except ImportError:
+        logging.error("Could not import matplotlib; please install and try again")
+        sys.exit(1)
     oe = OntoEnv(initialize=False)
     pos = nx.spring_layout(oe._dependencies, 2)
     nx.draw_networkx(oe._dependencies, pos=pos, with_labels=True)
     plt.savefig(output_filename)
 
 
 @i.command(help="Print dependency graph")
 @click.argument("root_uri", default="")
 def deps(root_uri):
     oe = OntoEnv(initialize=False)
     oe.print_dependency_graph(root_uri)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     i()
```

### Comparing `ontoenv-0.3.5a2/pyproject.toml` & `ontoenv-0.3.6/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ontoenv"
-version = "0.3.5a2"
+version = "0.3.6"
 description = "Manages owl:imports statements for multi-file development"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD 3-Clause"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 rdflib = "^6.0.0"
```

### Comparing `ontoenv-0.3.5a2/PKG-INFO` & `ontoenv-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontoenv
-Version: 0.3.5a2
+Version: 0.3.6
 Summary: Manages owl:imports statements for multi-file development
 License: BSD 3-Clause
 Author: Gabe Fierro
 Author-email: gtfierro@mines.edu
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

