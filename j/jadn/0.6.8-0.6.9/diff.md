# Comparing `tmp/jadn-0.6.8.tar.gz` & `tmp/jadn-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jadn-0.6.8.tar", last modified: Wed Jun  2 01:23:07 2021, max compression
+gzip compressed data, was "jadn-0.6.9.tar", last modified: Wed Jun  9 19:19:24 2021, max compression
```

## Comparing `jadn-0.6.8.tar` & `jadn-0.6.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2021-06-02 01:23:07.545202 jadn-0.6.8/
--rw-rw-rw-   0        0        0     3599 2021-06-02 01:23:07.545202 jadn-0.6.8/PKG-INFO
--rw-rw-rw-   0        0        0     3001 2021-03-16 13:58:46.000000 jadn-0.6.8/README.rst
--rw-rw-rw-   0        0        0      108 2021-02-19 15:41:53.000000 jadn-0.6.8/pyproject.toml
--rw-rw-rw-   0        0        0      928 2021-06-02 01:23:07.547202 jadn-0.6.8/setup.cfg
--rw-rw-rw-   0        0        0       41 2021-02-19 15:41:53.000000 jadn-0.6.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-02 01:23:07.389199 jadn-0.6.8/src/
-drwxrwxrwx   0        0        0        0 2021-06-02 01:23:07.414201 jadn-0.6.8/src/jadn/
--rw-rw-rw-   0        0        0      556 2021-05-24 03:56:44.000000 jadn-0.6.8/src/jadn/__init__.py
-drwxrwxrwx   0        0        0        0 2021-06-02 01:23:07.465199 jadn-0.6.8/src/jadn/codec/
--rw-rw-rw-   0        0        0     8457 2021-05-23 18:50:22.000000 jadn-0.6.8/src/jadn/codec/__init__.py
--rw-rw-rw-   0        0        0    15969 2021-06-01 14:04:03.000000 jadn-0.6.8/src/jadn/codec/codec.py
--rw-rw-rw-   0        0        0     5845 2021-02-11 15:52:37.000000 jadn-0.6.8/src/jadn/codec/format_serialize_json.py
--rw-rw-rw-   0        0        0     6014 2021-02-11 15:52:37.000000 jadn-0.6.8/src/jadn/codec/format_validate.py
-drwxrwxrwx   0        0        0        0 2021-06-02 01:23:07.517201 jadn-0.6.8/src/jadn/convert/
--rw-rw-rw-   0        0        0      378 2021-04-11 00:53:14.000000 jadn-0.6.8/src/jadn/convert/__init__.py
--rw-rw-rw-   0        0        0     4683 2021-03-30 00:35:43.000000 jadn-0.6.8/src/jadn/convert/dot_w.py
--rw-rw-rw-   0        0        0     7765 2021-02-11 15:52:37.000000 jadn-0.6.8/src/jadn/convert/html.py
--rw-rw-rw-   0        0        0     7286 2021-05-26 03:27:08.000000 jadn-0.6.8/src/jadn/convert/jas_w.py
--rw-rw-rw-   0        0        0     6423 2021-05-30 13:37:13.000000 jadn-0.6.8/src/jadn/convert/jidl.py
--rw-rw-rw-   0        0        0     6393 2021-04-11 00:53:14.000000 jadn-0.6.8/src/jadn/convert/proto.py
--rw-rw-rw-   0        0        0    10864 2021-03-08 13:19:23.000000 jadn-0.6.8/src/jadn/convert/table_w.py
--rw-rw-rw-   0        0        0     4004 2021-03-08 23:09:06.000000 jadn-0.6.8/src/jadn/convert/utils.py
--rw-rw-rw-   0        0        0     9579 2021-04-08 22:25:47.000000 jadn-0.6.8/src/jadn/core.py
-drwxrwxrwx   0        0        0        0 2021-06-02 01:23:07.521200 jadn-0.6.8/src/jadn/data/
--rw-rw-rw-   0        0        0     1484 2021-02-11 15:52:36.000000 jadn-0.6.8/src/jadn/data/dtheme.css
--rw-rw-rw-   0        0        0     4425 2021-05-30 13:54:27.000000 jadn-0.6.8/src/jadn/data/jadn_v1.0_schema.jadn
--rw-rw-rw-   0        0        0     3566 2021-05-30 13:37:13.000000 jadn-0.6.8/src/jadn/data/jadn_v1.0_schema.json
--rw-rw-rw-   0        0        0    14492 2021-05-27 17:57:48.000000 jadn-0.6.8/src/jadn/definitions.py
-drwxrwxrwx   0        0        0        0 2021-06-02 01:23:07.537203 jadn-0.6.8/src/jadn/transform/
--rw-rw-rw-   0        0        0      110 2021-05-23 18:49:24.000000 jadn-0.6.8/src/jadn/transform/__init__.py
--rw-rw-rw-   0        0        0     8327 2021-02-11 15:52:37.000000 jadn-0.6.8/src/jadn/transform/resolve.py
--rw-rw-rw-   0        0        0    10998 2021-06-02 01:04:14.000000 jadn-0.6.8/src/jadn/transform/transform.py
-drwxrwxrwx   0        0        0        0 2021-06-02 01:23:07.544200 jadn-0.6.8/src/jadn/translate/
--rw-rw-rw-   0        0        0       63 2021-02-11 15:52:37.000000 jadn-0.6.8/src/jadn/translate/__init__.py
--rw-rw-rw-   0        0        0    15773 2021-05-26 03:27:08.000000 jadn-0.6.8/src/jadn/translate/jsonschema_w.py
--rw-rw-rw-   0        0        0    17862 2021-06-01 23:26:43.000000 jadn-0.6.8/src/jadn/utils.py
-drwxrwxrwx   0        0        0        0 2021-06-02 01:23:07.439200 jadn-0.6.8/src/jadn.egg-info/
--rw-rw-rw-   0        0        0     3599 2021-06-02 01:23:07.000000 jadn-0.6.8/src/jadn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      875 2021-06-02 01:23:07.000000 jadn-0.6.8/src/jadn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-02 01:23:07.000000 jadn-0.6.8/src/jadn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2021-06-02 01:23:07.000000 jadn-0.6.8/src/jadn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2021-06-02 01:23:07.000000 jadn-0.6.8/src/jadn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-06-09 19:19:24.775730 jadn-0.6.9/
+-rw-rw-rw-   0        0        0     3599 2021-06-09 19:19:24.775730 jadn-0.6.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3001 2021-03-16 13:58:46.000000 jadn-0.6.9/README.rst
+-rw-rw-rw-   0        0        0      108 2021-02-19 15:41:53.000000 jadn-0.6.9/pyproject.toml
+-rw-rw-rw-   0        0        0      928 2021-06-09 19:19:24.785730 jadn-0.6.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2021-02-19 15:41:53.000000 jadn-0.6.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-09 19:19:24.575729 jadn-0.6.9/src/
+drwxrwxrwx   0        0        0        0 2021-06-09 19:19:24.609728 jadn-0.6.9/src/jadn/
+-rw-rw-rw-   0        0        0      556 2021-06-09 19:16:56.000000 jadn-0.6.9/src/jadn/__init__.py
+drwxrwxrwx   0        0        0        0 2021-06-09 19:19:24.677728 jadn-0.6.9/src/jadn/codec/
+-rw-rw-rw-   0        0        0     8457 2021-05-23 18:50:22.000000 jadn-0.6.9/src/jadn/codec/__init__.py
+-rw-rw-rw-   0        0        0    15969 2021-06-01 14:04:03.000000 jadn-0.6.9/src/jadn/codec/codec.py
+-rw-rw-rw-   0        0        0     5845 2021-02-11 15:52:37.000000 jadn-0.6.9/src/jadn/codec/format_serialize_json.py
+-rw-rw-rw-   0        0        0     6014 2021-02-11 15:52:37.000000 jadn-0.6.9/src/jadn/codec/format_validate.py
+drwxrwxrwx   0        0        0        0 2021-06-09 19:19:24.733728 jadn-0.6.9/src/jadn/convert/
+-rw-rw-rw-   0        0        0      378 2021-04-11 00:53:14.000000 jadn-0.6.9/src/jadn/convert/__init__.py
+-rw-rw-rw-   0        0        0     4759 2021-06-04 17:40:57.000000 jadn-0.6.9/src/jadn/convert/dot_w.py
+-rw-rw-rw-   0        0        0     7765 2021-02-11 15:52:37.000000 jadn-0.6.9/src/jadn/convert/html.py
+-rw-rw-rw-   0        0        0     7286 2021-05-26 03:27:08.000000 jadn-0.6.9/src/jadn/convert/jas_w.py
+-rw-rw-rw-   0        0        0     6423 2021-05-30 13:37:13.000000 jadn-0.6.9/src/jadn/convert/jidl.py
+-rw-rw-rw-   0        0        0     6393 2021-04-11 00:53:14.000000 jadn-0.6.9/src/jadn/convert/proto.py
+-rw-rw-rw-   0        0        0    10864 2021-03-08 13:19:23.000000 jadn-0.6.9/src/jadn/convert/table_w.py
+-rw-rw-rw-   0        0        0     4004 2021-03-08 23:09:06.000000 jadn-0.6.9/src/jadn/convert/utils.py
+-rw-rw-rw-   0        0        0     9579 2021-04-08 22:25:47.000000 jadn-0.6.9/src/jadn/core.py
+drwxrwxrwx   0        0        0        0 2021-06-09 19:19:24.737728 jadn-0.6.9/src/jadn/data/
+-rw-rw-rw-   0        0        0     1484 2021-02-11 15:52:36.000000 jadn-0.6.9/src/jadn/data/dtheme.css
+-rw-rw-rw-   0        0        0     4425 2021-06-06 23:47:58.000000 jadn-0.6.9/src/jadn/data/jadn_v1.0_schema.jadn
+-rw-rw-rw-   0        0        0     3566 2021-06-06 23:47:58.000000 jadn-0.6.9/src/jadn/data/jadn_v1.0_schema.json
+-rw-rw-rw-   0        0        0    14492 2021-05-27 17:57:48.000000 jadn-0.6.9/src/jadn/definitions.py
+drwxrwxrwx   0        0        0        0 2021-06-09 19:19:24.757728 jadn-0.6.9/src/jadn/transform/
+-rw-rw-rw-   0        0        0      110 2021-05-23 18:49:24.000000 jadn-0.6.9/src/jadn/transform/__init__.py
+-rw-rw-rw-   0        0        0     8327 2021-02-11 15:52:37.000000 jadn-0.6.9/src/jadn/transform/resolve.py
+-rw-rw-rw-   0        0        0    11186 2021-06-02 04:33:12.000000 jadn-0.6.9/src/jadn/transform/transform.py
+drwxrwxrwx   0        0        0        0 2021-06-09 19:19:24.773727 jadn-0.6.9/src/jadn/translate/
+-rw-rw-rw-   0        0        0       63 2021-02-11 15:52:37.000000 jadn-0.6.9/src/jadn/translate/__init__.py
+-rw-rw-rw-   0        0        0    15773 2021-05-26 03:27:08.000000 jadn-0.6.9/src/jadn/translate/jsonschema_w.py
+-rw-rw-rw-   0        0        0    17862 2021-06-01 23:26:43.000000 jadn-0.6.9/src/jadn/utils.py
+drwxrwxrwx   0        0        0        0 2021-06-09 19:19:24.639728 jadn-0.6.9/src/jadn.egg-info/
+-rw-rw-rw-   0        0        0     3599 2021-06-09 19:19:24.000000 jadn-0.6.9/src/jadn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      875 2021-06-09 19:19:24.000000 jadn-0.6.9/src/jadn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-09 19:19:24.000000 jadn-0.6.9/src/jadn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2021-06-09 19:19:24.000000 jadn-0.6.9/src/jadn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2021-06-09 19:19:24.000000 jadn-0.6.9/src/jadn.egg-info/top_level.txt
```

### Comparing `jadn-0.6.8/PKG-INFO` & `jadn-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jadn
-Version: 0.6.8
+Version: 0.6.9
 Summary: JADN schema tools
 Home-page: https://github.com/davaya/jadn-pypkg
 Author: David Kemp
 Author-email: dk190a@gmail.com
 License: Apache License 2.0
 Keywords: schema
 Platform: UNKNOWN
```

### Comparing `jadn-0.6.8/README.rst` & `jadn-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/setup.cfg` & `jadn-0.6.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/__init__.py` & `jadn-0.6.9/src/jadn/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 )
 # TODO: migrate to local imports??
 import jadn.codec
 import jadn.convert
 import jadn.transform
 import jadn.translate
 
-__version__ = '0.6.8'
+__version__ = '0.6.9'
```

### Comparing `jadn-0.6.8/src/jadn/codec/__init__.py` & `jadn-0.6.9/src/jadn/codec/__init__.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/codec/codec.py` & `jadn-0.6.9/src/jadn/codec/codec.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/codec/format_serialize_json.py` & `jadn-0.6.9/src/jadn/codec/format_serialize_json.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/codec/format_validate.py` & `jadn-0.6.9/src/jadn/codec/format_validate.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/convert/dot_w.py` & `jadn-0.6.9/src/jadn/convert/dot_w.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Translate a JADN schema into a GraphViz (https://graphviz.org/) graph display file
 """
 
 import re
+from datetime import datetime
 from typing import NoReturn
 from ..definitions import (TypeName, BaseType, TypeDesc, Fields, FieldName, FieldType, FieldOptions, FieldDesc,
                            PRIMITIVE_TYPES)
 from ..utils import ftopts_s2d
 
 
 # Wrap typenames at word boundaries to minimize node width, using a max of "lines" lines.
 def wrapstr(ss: str, lines: int=3) -> str:
     p = 0
     bp = len(ss)/lines
     wrapped = ''
-    for w in re.findall(r'[A-Z][a-z0-9]+', ss): # TODO: update regex to support name formats other than PascalCase
+    for w in re.findall(r'[A-Z][a-z0-9]+', ss):     # TODO: update regex to support name formats other than PascalCase
         if p > 0 and p + len(w)/2 > bp:
             wrapped += '\\n'
             bp += len(ss)/lines
         wrapped += w
         p += len(w)
     return wrapped
 
@@ -77,24 +78,24 @@
     Convert JADN schema to GraphViz "dot" file
     """
     s = dot_style()
     if style:
         s.update(style)
 
     text = ''
-    for k, v in schema["info"].items():
+    for k, v in schema.get('info', {}).items():
         text += f'# {k}: {v}\n'
     text += f'\n{dot_header(s["dotfile"])}\n'
 
     atypes = (*PRIMITIVE_TYPES, 'Enumerated')
     nodes = {tdef[TypeName]: k for k, tdef in enumerate(schema['types']) if tdef[BaseType] not in atypes}
     for td in schema['types']:
         node_type = f', shape="ellipse", fillcolor="{s["attr_color"]}"' if td[BaseType] in atypes else ''
         if s['attributes'] or not node_type:
-            node_type = ', shape="hexagon"' if '<->' in td[TypeDesc] else node_type
+            node_type = ', shape="hexagon"' if '<->' in td[TypeDesc] else node_type     # TODO: replace SOSA hacks
             text += f'  n{nodes[td[TypeName]]} [label="{wrapstr(td[TypeName])}"{node_type}]\n'
             for fd in td[Fields]:
                 if fd[FieldType] in nodes:
                     fopts, topts = ftopts_s2d(fd[FieldOptions])
                     edge_attrs = ['style="dashed"'] if 'link' in fopts or '<=' in fd[FieldDesc] else []
                     if s['links'] or not edge_attrs:
                         edge_attrs += [f'label="{fd[FieldName]}"'] if s['edge_label'] else []
@@ -116,8 +117,8 @@
         f.write(dot_dumps(schema, style) + '\n')
 
 
 __all__ = [
     'dot_dump',
     'dot_dumps',
     'dot_style'
-]
+]
```

### Comparing `jadn-0.6.8/src/jadn/convert/html.py` & `jadn-0.6.9/src/jadn/convert/html.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/convert/jas_w.py` & `jadn-0.6.9/src/jadn/convert/jas_w.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/convert/jidl.py` & `jadn-0.6.9/src/jadn/convert/jidl.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/convert/proto.py` & `jadn-0.6.9/src/jadn/convert/proto.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/convert/table_w.py` & `jadn-0.6.9/src/jadn/convert/table_w.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/convert/utils.py` & `jadn-0.6.9/src/jadn/convert/utils.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/core.py` & `jadn-0.6.9/src/jadn/core.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/data/dtheme.css` & `jadn-0.6.9/src/jadn/data/dtheme.css`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/data/jadn_v1.0_schema.jadn` & `jadn-0.6.9/src/jadn/data/jadn_v1.0_schema.jadn`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989130434782608%*

 * *Differences: {"'types'": "{2: {2: {insert: [(1, '+NSID')], delete: [0]}}}"}*

```diff
@@ -138,16 +138,16 @@
                 ]
             ]
         ],
         [
             "Namespaces",
             "MapOf",
             [
-                "+NSID",
                 "*Namespace",
+                "+NSID",
                 "{1"
             ],
             "Packages with referenced type defs",
             []
         ],
         [
             "Exports",
```

### Comparing `jadn-0.6.8/src/jadn/data/jadn_v1.0_schema.json` & `jadn-0.6.9/src/jadn/data/jadn_v1.0_schema.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.99951171875%*

 * *Differences: {"'properties'": "{'types': {'items': {'minItems': 2}}}"}*

```diff
@@ -208,15 +208,15 @@
                         "$ref": "#/definitions/Description"
                     },
                     {
                         "$ref": "#/definitions/Fields"
                     }
                 ],
                 "maxItems": 5,
-                "minItems": 1,
+                "minItems": 2,
                 "type": "array"
             },
             "type": "array"
         }
     },
     "required": [
         "types"
```

### Comparing `jadn-0.6.8/src/jadn/definitions.py` & `jadn-0.6.9/src/jadn/definitions.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/transform/resolve.py` & `jadn-0.6.9/src/jadn/transform/resolve.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/transform/transform.py` & `jadn-0.6.9/src/jadn/transform/transform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 
 from typing import Generator, List, NoReturn, Set, Union
 from ..definitions import (
     TypeName, BaseType, TypeDesc, Fields, ItemID, ItemValue, ItemDesc, FieldName, FieldOptions, FieldDesc, OPTION_ID,
-    EXTENSIONS, OPTION_TYPES, is_builtin, has_fields, TypeDefinition, EnumFieldDefinition, GenFieldDefinition
-)
-from ..utils import del_opt, ftopts_s2d, get_optx, list_type_schema, opts_d2s, object_type_schema, topts_s2d, etrunc
+    EXTENSIONS, OPTION_TYPES, is_builtin, has_fields, TypeDefinition, EnumFieldDefinition, GenFieldDefinition)
+from ..utils import (
+    del_opt, ftopts_s2d, get_optx, list_type_schema, opts_d2s, object_type_schema, topts_s2d, etrunc, raise_error)
 
 
 def strip_comments(schema: dict, width=0) -> dict:  # Strip or truncate comments from schema
     sc = copy.deepcopy(schema)
     for tdef in sc['types']:
         tdef[TypeDesc] = etrunc(tdef[TypeDesc], width)
         if len(tdef) > Fields:
@@ -41,15 +41,18 @@
                 elif 'link' in fo and tdef not in ltypes:
                     ltypes.append(tdef)
     for tdef in ltypes:
         for fdef in tdef.Fields:
             fo, fto = ftopts_s2d(fdef.FieldOptions)
             if 'link' in fo:
                 del_opt(fdef.FieldOptions, 'link')
-                fdef.FieldType = keys[fdef.FieldType]
+                try:
+                    fdef.FieldType = keys[fdef.FieldType]
+                except KeyError:
+                    raise_error(f'{tdef.TypeName}/{fdef.FieldName}: "{fdef.FieldType}" has no primary key')
 
 
 # Return option array index of enum or pointer option
 def epx(topts: List[OPTION_TYPES]) -> Union[int, float, str, None]:
     ex = get_optx(topts, 'enum')
     return ex if ex is not None else get_optx(topts, 'pointer')
```

### Comparing `jadn-0.6.8/src/jadn/translate/jsonschema_w.py` & `jadn-0.6.9/src/jadn/translate/jsonschema_w.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn/utils.py` & `jadn-0.6.9/src/jadn/utils.py`

 * *Files identical despite different names*

### Comparing `jadn-0.6.8/src/jadn.egg-info/PKG-INFO` & `jadn-0.6.9/src/jadn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jadn
-Version: 0.6.8
+Version: 0.6.9
 Summary: JADN schema tools
 Home-page: https://github.com/davaya/jadn-pypkg
 Author: David Kemp
 Author-email: dk190a@gmail.com
 License: Apache License 2.0
 Keywords: schema
 Platform: UNKNOWN
```

### Comparing `jadn-0.6.8/src/jadn.egg-info/SOURCES.txt` & `jadn-0.6.9/src/jadn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

