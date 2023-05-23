# Comparing `tmp/bento_mdf-0.4.5.tar.gz` & `tmp/bento_mdf-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bento_mdf-0.4.5.tar", max compression
+gzip compressed data, was "bento_mdf-0.7.2.tar", max compression
```

## Comparing `bento_mdf-0.4.5.tar` & `bento_mdf-0.7.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4774 2023-02-13 17:09:07.264076 bento_mdf-0.4.5/README.md
--rwxr-xr-x   0        0        0     2553 2023-02-13 17:09:07.265118 bento_mdf-0.4.5/bin/load-mdf.py
--rwxr-xr-x   0        0        0     1918 2023-02-13 17:09:07.266171 bento_mdf-0.4.5/bin/test-mdf.py
--rw-r--r--   0        0        0     1769 2023-02-13 17:27:16.746139 bento_mdf-0.4.5/pyproject.toml
--rw-r--r--   0        0        0       48 2023-02-13 17:09:07.277553 bento_mdf-0.4.5/src/bento_mdf/__init__.py
--rw-r--r--   0        0        0     9145 2023-02-13 17:09:07.278684 bento_mdf-0.4.5/src/bento_mdf/diff.py
--rw-r--r--   0        0        0    27398 2023-02-13 17:09:07.280008 bento_mdf-0.4.5/src/bento_mdf/mdf.py
--rw-r--r--   0        0        0     8110 2023-02-13 17:09:07.281324 bento_mdf-0.4.5/src/bento_mdf/validator.py
--rw-r--r--   0        0        0     5900 1970-01-01 00:00:00.000000 bento_mdf-0.4.5/setup.py
--rw-r--r--   0        0        0     5578 1970-01-01 00:00:00.000000 bento_mdf-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     4774 2023-02-13 22:09:03.146259 bento_mdf-0.7.2/README.md
+-rwxr-xr-x   0        0        0     2936 2023-05-23 17:21:20.349476 bento_mdf-0.7.2/bin/load-mdf.py
+-rwxr-xr-x   0        0        0     1918 2023-02-13 22:09:03.147706 bento_mdf-0.7.2/bin/test-mdf.py
+-rw-r--r--   0        0        0     1848 2023-05-23 21:47:12.034021 bento_mdf-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-02-13 22:09:03.157582 bento_mdf-0.7.2/src/bento_mdf/__init__.py
+-rw-r--r--   0        0        0     9129 2023-02-13 22:09:03.158593 bento_mdf-0.7.2/src/bento_mdf/diff.py
+-rw-r--r--   0        0        0    29005 2023-05-23 21:45:45.813530 bento_mdf-0.7.2/src/bento_mdf/mdf.py
+-rw-r--r--   0        0        0     8110 2023-02-13 22:09:03.160193 bento_mdf-0.7.2/src/bento_mdf/validator.py
+-rw-r--r--   0        0        0     5899 1970-01-01 00:00:00.000000 bento_mdf-0.7.2/setup.py
+-rw-r--r--   0        0        0     5577 1970-01-01 00:00:00.000000 bento_mdf-0.7.2/PKG-INFO
```

### Comparing `bento_mdf-0.4.5/README.md` & `bento_mdf-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `bento_mdf-0.4.5/bin/load-mdf.py` & `bento_mdf-0.7.2/bin/load-mdf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 #!/usr/bin/env python
 import sys
 sys.path.insert(0, '..')
 import os
 import getpass
 import argparse
 from bento_mdf.mdf import MDF
-from bento_meta.mdb import WriteableMDB, make_nanoid, load_mdf
+from bento_meta.mdb import (
+    WriteableMDB, make_nanoid, load_mdf, load_model_statements
+    )
+from sys import stderr
 
 parser = argparse.ArgumentParser(description="Load model in MDF into an MDB")
 parser.add_argument('files', nargs="*",
                     metavar="MDF-FILE", help="MDF file(s)/url(s)")
 parser.add_argument('--commit', default='',
                     help="commit SHA1 for MDF instance (if any)",
                     required=True)
 parser.add_argument('--handle', help="model handle")
 parser.add_argument('--user', help="MDB username")
 parser.add_argument('--passw', help="MDB password")
-parser.add_argument('--bolt', metavar="BoltURL", help="MDB Bolt url endpoint (specify as 'bolt://...')")
-parser.add_argument('--put', action='store_true', help="Load model to database")
-parser.add_argument('--make-nanoids', action='store_true', help="Add new nanoids to graph nodes")
+parser.add_argument('--bolt', metavar="BoltURL",
+                    help="MDB Bolt url endpoint (specify as 'bolt://...')")
+parser.add_argument('--put', action='store_true',
+                    help="Load model to database")
+parser.add_argument('--make-nanoids', action='store_true',
+                    help="Add new nanoids to graph nodes")
 # example:
 # args = parser.parse_args([
 #     "https://raw.githubusercontent.com/CBIIT/icdc-model-tool/master/model-desc/icdc-model.yml",
 #     "https://raw.githubusercontent.com/CBIIT/icdc-model-tool/master/model-desc/icdc-model-props.yml",
 #     "--commit",
 #     "a4aa9a43b9ad2087638ceaeef50d4a22a4b9b959",
 #     "--handle",
@@ -34,37 +40,45 @@
 #     "--passw",
 #     getpass.getpass()
 #     ])
 
 args = parser.parse_args()
 
 if not args.files:
-    parser.print_help()
+    parser.print_help(file=stderr)
     parser.exit(1)
 
+if args.put and not args.bolt:
+    print("error: --bolt and --user args required to put to database",file=stderr)
+    parser.exit(2)
+    
 if args.put and not args.passw:
     args.passw = getpass.getpass()
 
-print("load model from MDFs")
-mdf = MDF(*args.files, handle=args.handle, _commit=args.commit, raiseError=True)
+print("load model from MDFs", file=stderr)
+mdf = MDF(*args.files, handle=args.handle,
+          _commit=args.commit, raiseError=True)
 model = mdf.model
-if (args.bolt):
-    mdb = WriteableMDB(uri=args.bolt, user=args.user, password=args.passw)
-    model.mdb = mdb
 
 if args.put:
-    print("Put model to DB")
-    load_mdf(mdf,model.mdb)
+    print("Put model to DB",file=stderr)
+    mdb = WriteableMDB(uri=args.bolt, user=args.user, password=args.passw)
+    model.mdb = mdb
+    load_mdf(mdf, model.mdb)
     if args.make_nanoids:
-        print("Add nanoids to nodes")
+        print("Add nanoids to nodes",file=stderr)
         with mdb.driver.session() as s:
             result = s.run(
                 "match (n {_commit:$commit}) where not exists(n.nanoid) "
                 "with n limit 1 set n.nanoid=$nanoid return n",
-                {"commit":args.commit, "nanoid":make_nanoid()}
+                {"commit": args.commit, "nanoid": make_nanoid()}
             )
             while (result.peek()):
                 result = s.run(
                     "match (n {_commit:$commit}) where not exists(n.nanoid) "
                     "with n limit 1 set n.nanoid=$nanoid return n",
-                    {"commit":args.commit, "nanoid":make_nanoid()}
+                    {"commit": args.commit, "nanoid": make_nanoid()}
                     )
+else:
+    for s in load_model_statements(model, args.commit):
+        print(s)
+
```

### Comparing `bento_mdf-0.4.5/bin/test-mdf.py` & `bento_mdf-0.7.2/bin/test-mdf.py`

 * *Files identical despite different names*

### Comparing `bento_mdf-0.4.5/pyproject.toml` & `bento_mdf-0.7.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bento-mdf"
-version = "0.4.5"
+version = "0.7.2"
 description = "Python driver/validator for Bento Model Description Format"
 authors = [
     { name="Mark A. Jensen", email = "mark.jensen@nih.gov"}
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
@@ -14,30 +14,30 @@
 
 [project.urls]
 "Homepage" = "https://github.com/CBIIT/bento-mdf"
 "Bug Tracker" = "https://github.com/CBIIT/bento-mdf/issues"
 
 [tool.poetry]
 name = "bento-mdf"
-version = "0.4.5"
+version = "0.7.2"
 description = "Python driver/validator for Bento Model Description Format"
 authors = [
     "Mark A. Jensen <mark.jensen@nih.gov>"
 ]
 license = "Apache 2.0"
 readme = "README.md"
 include = ["logs/log.ini"]
 
 [tool.poetry.scripts]
 "test-mdf.py" = { reference = "bin/test-mdf.py", type = "file" }
 "load-mdf" = { reference = "bin/load-mdf.py", type = "file" }
 
 [tool.poetry.dependencies]
 python = "^3.8"
-bento-meta = ">=0.0.54"
+bento-meta = ">=0.1.3"
 jsonschema = "^4.17.3"
 pyyaml = ">=6"
 delfick-project = "^0.7.9"
 requests = "^2.28.2"
 tqdm = "^4.64.1"
 
 [tool.poetry.group.dev.dependencies]
@@ -64,7 +64,13 @@
 dist_path = "dist/"
 upload_to_release = true
 upload_to_pypi = false
 remove_dist = false
 patch_without_tag = true
 major_on_zero = false # while major version on 0.y.z, won't bump to 1.0.0
 version_source = "tag" # temp?
+
+[tool.pytest.ini_options]
+filterwarnings = [
+   "ignore::UserWarning",
+   ]
+
```

### Comparing `bento_mdf-0.4.5/src/bento_mdf/diff.py` & `bento_mdf-0.7.2/src/bento_mdf/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             for att in obj_atts:
                 a_att = getattr(a_ent, att)
                 b_att = getattr(b_ent, att)
 
                 if a_att == b_att:  # only if both 'None' *or* is same object
                     continue
                 if not a_att or not b_att:  # one is 'None'
-                    diff_.update_result(thing, entk, att, sorted(a_att), sorted(b_att))
+                    diff_.update_result(thing, entk, att, a_att, b_att)
                     continue
 
                 if type(a_att) == type(b_att):
                     if type(a_att) == ValueSet:  # kludge for ValueSet+Terms
                         if diff_.valuesets_are_different(a_att, b_att):
                             diff_.update_result(
                                 thing,
```

### Comparing `bento_mdf-0.4.5/src/bento_mdf/mdf.py` & `bento_mdf-0.7.2/src/bento_mdf/mdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 bento_mdf.mdf
 ==============
 
 This module contains :class:`MDF`, a class for reading a graph data model in
-Model Description Format into a :class:`bento_meta.model.Model` object, and 
+Model Description Format into a :class:`bento_meta.model.Model` object, and
 writing the opposite way.
 
 """
 import sys
 import yaml
 import logging
 from tqdm import tqdm
@@ -49,16 +49,14 @@
         :param str|file|url *yaml_files: MDF filenames or file objects, 
         in desired merge order
         :param str handle: Handle (name) for the resulting Model
         :param :class:`Model` model: Model to convert to MDF
         :param boolean raiseError: raise on error if True
         :param :class:`logging.Logger` logger: Python logger (suitable default)
         :attribute model: the :class:`bento_meta.model.Model` created"""
-        if not model and (not handle or not isinstance(handle, str)):
-            raise ArgError("arg handle= must be a str - name for model")
         if model and not isinstance(model,Model):
             raise ArgError("arg model= must be a Model instance")
             
         self.files = yaml_files
         self.schema = {}
         self.mdf_schema = mdf_schema
         self._model = model
@@ -237,16 +235,18 @@
                 (hdl, src, dst) = ent.triplet
                 ends = [
                     e
                     for e in yedges[hdl]["Ends"]
                     if e["Src"] == src and e["Dst"] == dst
                 ]
                 if len(ends) > 1:
-                    self.logger.warning("edge '{ename}' has more than one Ends pair Src:'{src}',"
-                                        "Dst:'{dst}'".format(ename=hdl, src=src, dst=dst))
+                    self.logger.warning(
+                        "edge '{ename}' has more than one Ends pair Src:'{src}',"
+                        "Dst:'{dst}'".format(ename=hdl, src=src, dst=dst)
+                    )
                 end = ends[0]
             
                 # note the end-specified props _replace_ the edge-specified props,
                 # they are not merged:
                 pnames = end.get("Props") or yedges[hdl].get("Props")
                 if yurps:  # universal relationship props
                     pnames.extend(yurps["mayHave"] if yurps.get("mayHave") else [])
@@ -305,42 +305,45 @@
     def create_or_merge_prop_from_mdf(self, ypdef, p_hdl,force_create):
         init = {"handle": p_hdl,
                 "model": self.handle,
                 "_commit": self._commit}
         if not force_create and (init["model"], init["handle"]) in self._props:
             pass  # merge property
         else:
+            prop = Property(init)
             if 'Desc' in ypdef and ypdef['Desc']:
-                init['desc'] = ypdef['Desc']
+                prop.desc = ypdef['Desc']
             if 'NanoID' in ypdef and ypdef['NanoID']:
-                init['nanoid'] = ypdef['NanoID']
+                prop.nanoid = ypdef['NanoID']
             if 'Type' in ypdef:
-                init.update(self.calc_value_domain(ypdef["Type"], p_hdl))
+                self.calc_value_domain(ypdef["Type"], prop)
             elif 'Enum' in ypdef:
-                init.update(self.calc_value_domain(ypdef["Enum"], p_hdl))
+                self.calc_value_domain(ypdef["Enum"], prop)
             else:
                 self.logger.warning(
                     "property '{p_hdl}' does not "
                     "specify a data type".format(p_hdl=p_hdl)
                 )
                 init["value_domain"] = Property.default("value_domain")
-            # handle union type
-            u_types = None
-            if init["value_domain"] == "union":
-                u_types = init["types"]
-                del init["types"]
-                # reduce to the first value set present in type list
-                specs = [x for x in u_types if x["value_domain"] == "value_set"]
-                if specs:
-                    init.update(specs[0])
-                else:
-                    init["value_domain"] = "union"
-            prop = Property(init)
-            if u_types:
-                prop.value_types.extend(u_types)
+
+            # TODO: handle union type
+            # removing this kludge by commenting:
+            # u_types = None
+            # if init["value_domain"] == "union":
+            #     u_types = init["types"]
+            #     del init["types"]
+            #     # reduce to the first value set present in type list
+            #     specs = [x for x in u_types if x["value_domain"] == "value_set"]
+            #     if specs:
+            #         init.update(specs[0])
+            #     else:
+            #         init["value_domain"] = "union"
+
+            # if u_types:
+            #     prop.value_types.extend(u_types)
             if "Tags" in ypdef:
                 for t in ypdef["Tags"]:
                     prop.tags[t] = Tag({"key": t,
                                         "value": ypdef["Tags"][t],
                                         "_commit": self._commit})
             if "Term" in ypdef:
                 self.annotate_entity_from_mdf(prop, ypdef["Term"])
@@ -361,123 +364,158 @@
             tm["origin_name"] = ytm["Origin"]
         else:
             self.logger.warning(
                 "No Origin provided for term '{term}'".format(term=t_hdl)
             )
             tm["origin_name"] = self.handle
         tm["value"] = ytm["Value"]
-        if (tm["value"],tm["origin_name"]) in self._terms:
+        tm_key = t_hdl if t_hdl else tm["value"]
+        if (tm_key,tm["origin_name"]) in self._terms:
             pass  # merge term
         else:
+            tm["handle"] = ytm["Handle"] if 'Handle' in ytm else t_hdl
             if 'Definition' in ytm and ytm['Definition']:
                 tm["origin_definition"] = unquote(ytm["Definition"])
             if 'Code' in ytm:
                 tm["origin_id"] = ytm["Code"]
             if 'Version' in ytm:
                 tm["origin_version"] = ytm["Version"]
-            if 'Handle' in ytm:
-                tm["handle"] = ytm["Handle"]
             if 'NanoID' in ytm:
                 tm["nanoid"] = ytm["NanoID"]
-            self._terms[(tm["value"],tm["origin_name"])] = Term(tm)
-        return self._terms[(tm["value"],tm["origin_name"])]
+            self._terms[(tm_key, tm["origin_name"])] = Term(tm)
+        return self._terms[(tm_key, tm["origin_name"])]
 
     def annotate_entity_from_mdf(self, ent, yterm_list):
         for yterm in yterm_list:
             tm = self.create_or_merge_term_from_mdf(yterm)
             self._model.annotate(ent, tm)
             if self._commit:
                 if not ent.concept._commit:
                     ent.concept._commit = self._commit
 
-    def calc_value_domain(self, typedef, pname=None):
+    def calc_value_domain(self, typedef, prop=None):
+        pname = prop.handle if prop else '(none)';
         if isinstance(typedef, dict):
             if typedef.get("pattern"):
+                prop.value_domain = "regexp"
+                prop.pattern = typedef["pattern"]
                 return {"value_domain": "regexp",
                         "pattern": typedef["pattern"]}
             elif typedef.get("units"):
+                prop.value_domain = typedef.get("value_type")
+                prop.units = ";".join(typedef.get("units"))
                 return {
                     "value_domain": typedef.get("value_type"),
                     "units": ";".join(typedef.get("units")),
                 }
             elif typedef.get("item_type"):
                 if (typedef["value_type"] == 'list'):
                     i_domain = self.calc_value_domain(typedef["item_type"])
+                    prop.value_domain = "list"
+                    prop.item_domain = i_domain["value_domain"]
                     ret = {"value_domain": "list",
                            "item_domain": i_domain["value_domain"]}
                     if i_domain.get("pattern"):
+                        prop.pattern = i_domain["pattern"]
                         ret["pattern"] = i_domain["pattern"]
                     if i_domain.get("units"):
+                        prop.units = i_domain["units"]
                         ret["units"] = i_domain["units"]
                     if i_domain.get("value_set"):
                         ret["value_set"] = i_domain["value_set"]
                     return ret
                 else:
                     self.logger.warning(
                         "MDF type descriptor defines item_type, but value_type"
                         " is {}, not 'list' (property '{}')".format(typedef["value_type"],pname))
             elif not typedef:
                 self.logger.warning("MDF type descriptor is null for property '{}'".format(pname))
             else:
                 # punt
                 self.logger.warning(
                     "MDF type descriptor unrecognized: json looks like {} (property '{}')".
-                    format(json.dumps(typedef),pname)
+                    format(json.dumps(typedef), pname)
                     )
+                if prop:
+                    prop.value_domain = json.dumps(typedef)
                 return {"value_domain": json.dumps(typedef)}
         elif isinstance(typedef, list):  # a valueset: create value set and term objs
             # could be either a Union or an Enum...
             if (not isinstance(typedef[0], str) or
                 typedef[0] in self.mdf_schema["defs"]["simpleType"]["enum"]):
                 # guess is a union type
                 ret = []
                 for t in typedef:
                     ret.append(self.calc_value_domain(t))
-                return {"value_domain": "union", "types":ret}
+                if prop:
+                    prop.value_domain = "union"
+                    prop.value_types = ret
+                return {"value_domain": "union", "types": ret}
             else:
-                vs = ValueSet({"nanoid": make_nano(), "_commit": self._commit})
-                vs.handle = self.handle + vs.nanoid
-                # interpret boolean values as strings
+                vs_terms = []
                 if (isinstance(typedef[0], str) and
-                    re.match("^(?:https?|bolt)://", typedef[0])):  # looks like url
+                        re.match("^(?:https?|bolt)://", typedef[0])):  # looks like url
+                    # here create a ValueSet for the purpose of storing the url
+                    if prop:
+                        prop.value_domain = 'value_set'
+                    vs = ValueSet({"nanoid": make_nano(), "_commit": self._commit})
+                    vs.handle = self.handle + vs.nanoid
                     vs.url = typedef[0]
-                else:  # an enum
+                else:  # an enum, use model machinery to add terms
+                    if prop:
+                        prop.value_domain = 'value_set'
                     for t in typedef:
                         if isinstance(t, bool):  # stringify booleans in term context
                             t = "True" if t else "False"
-                        if t not in self._terms:
-                            self._terms[t] = Term({
+                        # here is where we 'merge' terms
+                        # look for this term value/handle among the Terms
+                        keys = [k for k in self._terms if k[0] == t]
+                        tm = None
+                        if keys:
+                            tm = self._terms[keys[0]]
+                        else:
+                            # create a stub term
+                            tm = Term({
                                 "value": t,
                                 "origin_name": self.handle,
                                 "_commit": self._commit
                             })
-                        vs.terms[self._terms[t].value] = self._terms[t]
-                return {"value_domain": "value_set", "value_set": vs}
+                            self._terms[(t, self.handle)] = tm
+                        vs_terms.append(tm)
+                        if prop:
+                            self.model.add_terms(prop, tm)
+                return {"value_domain": "value_set", "value_set": vs_terms}
         elif isinstance(typedef, str):
             if typedef not in self.mdf_schema["defs"]["simpleType"]["enum"]:
                 self.logger.warning(
-                    "Type descriptor '{}' not present in MDF schema simpleType definition"
+                    "Type descriptor '{}' not present in MDF schema "
+                    "simpleType definition"
                     .format(typedef))
+            if prop:
+                prop.value_domain = typedef
             return {"value_domain": typedef}
         else:
-            self.logger.warning("Applying default value domain to property '{}'".format(pname))
+            self.logger.warning(
+                "Applying default value domain to property '{}'".format(pname))
+            if prop:
+                prop.value_domain = Property.default("value_domain")
             return {"value_domain": Property.default("value_domain")}
 
     def write_mdf(self, model=None, file=None):
         """Write a :class:`Model` to a model description file (MDF)
         :param :class:`Model` model: Model to convert (if None, use the model attribute of the MDF object)
         :param str|file file: File name or object to write to (default is None; just return the MDF as dict)
         :returns: MDF as dict"""
         if not model:
             model = self.model
-        mdf = {"Nodes":{},
-               "Relationships":{},
-               "PropDefinitions":{},
-               "Terms":{},
-               "Handle":model.handle}
+        mdf = {"Nodes": {},
+               "Relationships": {},
+               "PropDefinitions": {},
+               "Terms": {},
+               "Handle": model.handle}
         for nd in sorted(model.nodes):
             node = model.nodes[nd]
             mdf_node = {}
             mdf["Nodes"][nd] = mdf_node
             if node.tags:
                 mdf_node["Tags"] = {}
                 for t in node.tags:
@@ -514,15 +552,15 @@
                 mdf["Relationships"][edge.handle] = mdf_edge
             ends = {"Src": edge.src.handle,
                     "Dst": edge.dst.handle}
             if "Ends" in mdf_edge:
                 mdf_edge["Ends"].append(ends)
             else:
                 mdf_edge["Ends"] = [ends]
-            if not "Mul" in mdf_edge:
+            if "Mul" not in mdf_edge:
                 mdf_edge["Mul"] = edge.multiplicity or Edge.default("multiplicity")
             else:
                 if mdf_edge["Mul"] != edge.multiplicity:
                     ends["Mul"] = edge.multiplicity
             if edge.tags:
                 mdf_edge["Tags"] = {}
                 for t in edge.tags:
@@ -569,15 +607,15 @@
                 for t in prop.tags:
                     mdf_prop["Tags"][t] = prop.tags[t].value
             if prop.value_domain == "value_set":
                 mdf_prop["Enum"] = self.calc_prop_type(prop)
                 for t in prop.terms:
                     # if t in mdf["Terms"]:
                     #    self.logger.warning("Term collision at {} (property {})".format(t, prop.handle))
-                    if not t in mdf["Terms"]:
+                    if t not in mdf["Terms"]:
                         mdf["Terms"][t] = {
                             "Value": prop.terms[t].value,
                             "Definition": prop.terms[t].origin_definition,
                             "Origin": prop.terms[t].origin,
                             "Code": prop.terms[t].origin_id,
                         }
             else:
@@ -608,19 +646,19 @@
 
     def calc_prop_type(self,prop):
         if not prop.value_domain:
             return Property.default("value_domain")
         if prop.value_domain == "regexp":
             if not prop.pattern:
                 self.logger.warning("Property {} has 'regexp' value domain, but no pattern specified".format(prop.handle))
-                return {"pattern":"^.*$"}
+                return {"pattern": "^.*$"}
             else:
-                return {"pattern":prop.pattern}
+                return {"pattern": prop.pattern}
         if prop.units:
-            return {"value_type":prop.value_domain, "units":prop.units.split(';')}
+            return {"value_type": prop.value_domain, "units": prop.units.split(';')}
         if prop.value_domain == "value_set":
             if not prop.value_set:
                 self.logger.warning("Property {} has 'value_set' value domain, but value_set attribute is None".format(prop.handle))
                 return "string"
             values = []
             for trm in sorted(prop.terms):
                 values.append(trm)
```

### Comparing `bento_mdf-0.4.5/src/bento_mdf/validator.py` & `bento_mdf-0.7.2/src/bento_mdf/validator.py`

 * *Files identical despite different names*

### Comparing `bento_mdf-0.4.5/setup.py` & `bento_mdf-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 packages = \
 ['bento_mdf']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bento-meta>=0.0.54',
+['bento-meta>=0.1.3',
  'delfick-project>=0.7.9,<0.8.0',
  'jsonschema>=4.17.3,<5.0.0',
  'pyyaml>=6',
  'requests>=2.28.2,<3.0.0',
  'tqdm>=4.64.1,<5.0.0']
 
 scripts = \
 ['bin/test-mdf.py', 'bin/load-mdf.py']
 
 setup_kwargs = {
     'name': 'bento-mdf',
-    'version': '0.4.5',
+    'version': '0.7.2',
     'description': 'Python driver/validator for Bento Model Description Format',
     'long_description': 'bento_mdf\n=======\n\nPython 3 drivers for the graph [Model Description Format](https://github.com/CBIIT/bento-mdf)\n\nThis directory provides ``test-mdf.py``, a standalone command line MDF validator.\n\n## Installation\n\nInstall the latest version (including scripts below) from GitHub using\nan up-to-date pip:\n\n\tpip install bento_mdf@git+https://github.com/CBIIT/bento-mdf.git#egg=subdir\\&subdirectory=drivers/python\n\n## Scripts\n\nScripts [`test-mdf.py`](./test-mdf.py) and\n[`load-mdf.py`](./load-mdf.py) are included in the\ndistribution. `test-mdf` is a verbose validator that can be used to\nfind issues in a set of local MDFs using the [MDF\nJSONSchema](../../schema/mdf-schema.yaml). `load-mdf` will load a\nvalid set of MDFs into an existing [Neo4j](https://neo4j.com) [Metamodel Database](https://github.com/CBIIT/bento-meta).\n\n\n## `test-mdf` Usage\n\n    $ test-mdf.py -h\n    usage: test-mdf.py [-h] [--schema SCHEMA] [--quiet] [--log-file LOG_FILE]\n                       mdf-file [mdf-file ...]\n\n    Validate MDF against JSONSchema\n\n    positional arguments:\n      mdf-file             MDF yaml files for validation\n\n    optional arguments:\n      -h, --help           show this help message and exit\n      --schema SCHEMA      MDF JSONschema file\n      --quiet              Suppress output; return only exit value\n      --log-file LOG_FILE  Log file name\n\nSee "Validator Notes" below.\n\n## `load-mdf` Usage\n\n    $ ./load-mdf.py -h\n    usage: load-mdf.py [-h] --commit COMMIT [--handle HANDLE] [--user USER] [--passw PASSW]\n                       [--bolt BoltURL] [--put]\n                       [MDF-FILE ...]\n\n    Load model in MDF into an MDB\n\n    positional arguments:\n      MDF-FILE         MDF file(s)/url(s)\n\n    optional arguments:\n      -h, --help       show this help message and exit\n      --commit COMMIT  commit SHA1 for MDF instance (if any)\n      --handle HANDLE  model handle\n      --user USER      MDB username\n      --passw PASSW    MDB password\n      --bolt BoltURL   MDB Bolt url endpoint (specify as \'bolt://...\')\n      --put            Load model to database\n\n## Validator `test-mdf.py`Notes\n\nThe ``--schema`` argument is optional. ``test-mdf.py`` will automatically retrieve the latest [mdf-schema.yaml](../../schema/mdf-schema.yaml) in the master branch of [this repo](https://github.com/CBIIT/bento-mdf).\n\nThe script tests both the syntax of the YAML (for both schema and MDF files), and the validity of the files with respect to the JSONSchema (for both schema and MDF files).\n\nThe errors are as emitted from the [PyYaml](https://pyyaml.org/wiki/PyYAMLDocumentation) and [jsonschema](https://python-jsonschema.readthedocs.io/en/stable/) packages, and can be rather obscure.\n\n* Successful test\n\n        $ test-mdf.py samples/ctdc_model_file.yaml samples/ctdc_model_properties_file.yaml \n        Checking schema YAML =====\n        Checking as a JSON schema =====\n        Checking instance YAML =====\n        Checking instance against schema =====\n\n* Bad YAML syntax\n\n        $ test-mdf.py samples/ctdc_model_bad.yaml samples/ctdc_model_properties_file.yaml \n        Checking schema YAML =====\n        Checking as a JSON schema =====\n        Checking instance YAML =====\n        YAML error in \'samples/ctdc_model_bad.yaml\':\n        while parsing a block mapping\n          in "samples/ctdc_model_bad.yaml", line 1, column 1\n        expected <block end>, but found \'<block mapping start>\'\n          in "samples/ctdc_model_bad.yaml", line 3, column 3\n\n* Schema-invalid YAML\n\n        $ test-mdf.py samples/ctdc_model_file_invalid.yaml samples/ctdc_model_properties_file.yaml \n        Checking schema YAML =====\n        Checking as a JSON schema =====\n        Checking instance YAML =====\n        Checking instance against schema =====\n        [\'show_node\', \'specimen_id\', \'biopsy_sequence_number\', \'specimen_type\'] is not of type \'object\'\n        \n        Failed validating \'type\' in schema[\'properties\'][\'Nodes\'][\'additionalProperties\']:\n            {\'$id\': \'#nodeSpec\',\n             \'properties\': {\'Category\': {\'$ref\': \'#/defs/snake_case_id\'},\n                            \'Props\': {\'oneOf\': [{\'items\': {\'$ref\': \'#/defs/snake_case_id\'},\n                                                 \'type\': \'array\',\n                                                 \'uniqueItems\': True},\n                                                {\'type\': \'null\'}]},\n                            \'Tags\': {\'$ref\': \'#/defs/tagsSpec\'}},\n             \'required\': [\'Props\'],\n             \'type\': \'object\'}\n        \n        On instance[\'Nodes\'][\'specimen\']:\n            [\'show_node\', \'specimen_id\', \'biopsy_sequence_number\', \'specimen_type\']\n\n## Testing the tester\n\nThe validator code itself can be tested as follows:\n\n    pip install tox\n    cd bento-mdf/validators/mdf-validate\n    tox\n\n\n\n\n',
     'author': 'Mark A. Jensen',
     'author_email': 'mark.jensen@nih.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `bento_mdf-0.4.5/PKG-INFO` & `bento_mdf-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: bento-mdf
-Version: 0.4.5
+Version: 0.7.2
 Summary: Python driver/validator for Bento Model Description Format
 License: Apache 2.0
 Author: Mark A. Jensen
 Author-email: mark.jensen@nih.gov
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bento-meta (>=0.0.54)
+Requires-Dist: bento-meta (>=0.1.3)
 Requires-Dist: delfick-project (>=0.7.9,<0.8.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: pyyaml (>=6)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Description-Content-Type: text/markdown
```

