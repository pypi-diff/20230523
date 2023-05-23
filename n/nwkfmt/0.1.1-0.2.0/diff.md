# Comparing `tmp/nwkfmt-0.1.1.tar.gz` & `tmp/nwkfmt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwkfmt-0.1.1.tar", max compression
+gzip compressed data, was "nwkfmt-0.2.0.tar", max compression
```

## Comparing `nwkfmt-0.1.1.tar` & `nwkfmt-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1073 2022-09-19 16:56:12.057972 nwkfmt-0.1.1/LICENSE
--rw-r--r--   0        0        0      499 2022-11-11 11:42:58.678644 nwkfmt-0.1.1/README.md
--rwxr-xr-x   0        0        0     3651 2022-11-11 14:51:50.308189 nwkfmt-0.1.1/nwkfmt/cli.py
--rw-r--r--   0        0        0      462 2022-11-11 15:12:37.927747 nwkfmt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1293 2022-11-11 15:12:52.047529 nwkfmt-0.1.1/setup.py
--rw-r--r--   0        0        0     1008 2022-11-11 15:12:52.047688 nwkfmt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-09-19 16:56:12.057972 nwkfmt-0.2.0/LICENSE
+-rw-r--r--   0        0        0      660 2023-05-23 14:03:09.250940 nwkfmt-0.2.0/README.md
+-rwxr-xr-x   0        0        0     4010 2023-05-23 14:01:53.260339 nwkfmt-0.2.0/nwkfmt/cli.py
+-rw-r--r--   0        0        0      459 2023-05-23 14:03:55.298995 nwkfmt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1217 1970-01-01 00:00:00.000000 nwkfmt-0.2.0/PKG-INFO
```

### Comparing `nwkfmt-0.1.1/LICENSE` & `nwkfmt-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nwkfmt-0.1.1/nwkfmt/cli.py` & `nwkfmt-0.2.0/nwkfmt/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #! /usr/bin/env python
 from pathlib import Path
+from typing import List
 
 import typer
 
 app = typer.Typer(context_settings={"help_option_names": ["-h", "--help"]})
 
 @app.command()
 def test( 
@@ -15,20 +16,22 @@
         dir_okay=False,
         writable=True,
         readable=True,
         resolve_path=True,
     ),
     outfile: Path = typer.Option(None, help="Output file"),
     inplace: bool = typer.Option(False, help="Overwrite input file"),
-    terminals=typer.Option(None, help="Output path for list of tips"),
+    terminals=typer.Option(None, help="Output path for list of tip names"),
+    internals=typer.Option(None, help="Output path for list of internal node names"),
 ):
     import re
     from uuid import uuid4
 
     from Bio import Phylo
+    from Bio.Phylo import BaseTree
 
     def recursive_print(
         clade: Phylo.BaseTree.Clade,
         string: list = [],
         indent: int = 0,
         last=True,
     ) -> str:
@@ -46,15 +49,15 @@
                 )
             string.append(
                 "  " * indent
                 + ")"
                 + (
                     clade.name
                     if clade.name
-                    else f"internal_{str(uuid4())[0:4]}"
+                    else f"internal_{str(uuid4())[0:8]}"
                 )
                 + ("," if not last else "")
             )
         return string
 
     with open(file, "r") as f:
         # Check if regex matches
@@ -78,15 +81,15 @@
                         print(f"Line {line_number+2}: {lines[line_number+1]}")
                         break
             print(
                 "\nERROR: Invalid input Newick, clade name(s) contain(s) whitespace"
             )
             raise typer.Exit(1)
 
-    trees = list(Phylo.parse(file, "newick"))
+    trees: List[BaseTree.Tree] = list(Phylo.parse(file, "newick"))
     for tree in trees:
         clade_names = []
         for clade in tree.find_clades():
             if clade.name is not None:
                 if clade.name in clade_names:
                     raise Exception(f"Duplicate name {clade.name} detected")
                 clade_names.append(clade.name)
@@ -98,17 +101,20 @@
             outfile = file
         if outfile:
             with open(outfile, "w") as f:
                 for line in recursive_print(tree.root):
                     f.write(line + "\n")
                 f.write(";")
         if terminals:
-            with open(terminals):
+            with open(terminals, "w") as f:
                 for clade in tree.get_terminals():
                     f.write(clade.name + "\n")
-
+        if internals:
+            with open(internals, "w") as f:
+                for nonterminal in tree.get_nonterminals():
+                    f.write(nonterminal.name + "\n")
 
 def entry_point() -> None:
     app()
 
 if __name__ == "__main__":
     entry_point()
```

### Comparing `nwkfmt-0.1.1/PKG-INFO` & `nwkfmt-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: nwkfmt
-Version: 0.1.1
+Version: 0.2.0
 Summary: Simple Newick tree validator and formatter
 Author: Cornelius Roemer
 Author-email: cornelius.roemer@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: biopython (>=1.73,<2.0)
 Requires-Dist: typer (>=0.6,<1)
 Description-Content-Type: text/markdown
 
 # Newick Tree Validator and Formatter
 
 Simple utility to validate and format Newick trees.
@@ -45,7 +46,17 @@
 
 ## Requirements
 
 - Python
 - Typer
 - BioPython
 
+## Release
+
+This project uses [Poetry](https://python-poetry.org/) for dependency management and packaging.
+
+To build a release, run:
+
+```bash
+poetry build
+```
+
```

