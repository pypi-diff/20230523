# Comparing `tmp/solc-json-parser-0.1.5.tar.gz` & `tmp/solc-json-parser-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/solc-json-parser-0.1.5.tar", last modified: Wed Jan  4 07:28:22 2023, max compression
+gzip compressed data, was "dist/solc-json-parser-0.1.8.tar", last modified: Tue May 23 08:34:20 2023, max compression
```

## Comparing `solc-json-parser-0.1.5.tar` & `solc-json-parser-0.1.8.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 garfield  (1000) garfield  (1000)        0 2023-01-04 07:28:22.791193 solc-json-parser-0.1.5/
--rw-r--r--   0 garfield  (1000) garfield  (1000)      787 2023-01-04 07:28:22.791193 solc-json-parser-0.1.5/PKG-INFO
--rw-r--r--   0 garfield  (1000) garfield  (1000)      600 2022-12-27 06:23:59.000000 solc-json-parser-0.1.5/README.md
--rw-r--r--   0 garfield  (1000) garfield  (1000)      197 2023-01-04 07:28:22.792193 solc-json-parser-0.1.5/setup.cfg
--rw-r--r--   0 garfield  (1000) garfield  (1000)      723 2023-01-04 07:26:47.000000 solc-json-parser-0.1.5/setup.py
-drwxr-xr-x   0 garfield  (1000) garfield  (1000)        0 2023-01-04 07:28:22.790193 solc-json-parser-0.1.5/solc_json_parser/
--rw-r--r--   0 garfield  (1000) garfield  (1000)        0 2022-10-13 09:34:20.000000 solc-json-parser-0.1.5/solc_json_parser/__init__.py
--rw-r--r--   0 garfield  (1000) garfield  (1000)       33 2022-10-25 02:43:28.000000 solc-json-parser-0.1.5/solc_json_parser/consts.py
--rw-r--r--   0 garfield  (1000) garfield  (1000)     1031 2022-12-27 06:23:59.000000 solc-json-parser-0.1.5/solc_json_parser/fields.py
--rw-r--r--   0 garfield  (1000) garfield  (1000)     2229 2022-12-27 06:23:59.000000 solc-json-parser-0.1.5/solc_json_parser/fix_imports.py
--rw-r--r--   0 garfield  (1000) garfield  (1000)     7796 2023-01-04 07:25:35.000000 solc-json-parser-0.1.5/solc_json_parser/flatten.py
--rw-r--r--   0 garfield  (1000) garfield  (1000)    41910 2023-01-03 03:37:44.000000 solc-json-parser-0.1.5/solc_json_parser/parser.py
--rw-r--r--   0 garfield  (1000) garfield  (1000)      221 2022-10-13 09:34:11.000000 solc-json-parser-0.1.5/solc_json_parser/version_cfg.py
-drwxr-xr-x   0 garfield  (1000) garfield  (1000)        0 2023-01-04 07:28:22.791193 solc-json-parser-0.1.5/solc_json_parser.egg-info/
--rw-r--r--   0 garfield  (1000) garfield  (1000)      787 2023-01-04 07:28:22.000000 solc-json-parser-0.1.5/solc_json_parser.egg-info/PKG-INFO
--rw-r--r--   0 garfield  (1000) garfield  (1000)      429 2023-01-04 07:28:22.000000 solc-json-parser-0.1.5/solc_json_parser.egg-info/SOURCES.txt
--rw-r--r--   0 garfield  (1000) garfield  (1000)        1 2023-01-04 07:28:22.000000 solc-json-parser-0.1.5/solc_json_parser.egg-info/dependency_links.txt
--rw-r--r--   0 garfield  (1000) garfield  (1000)       89 2023-01-04 07:28:22.000000 solc-json-parser-0.1.5/solc_json_parser.egg-info/requires.txt
--rw-r--r--   0 garfield  (1000) garfield  (1000)       17 2023-01-04 07:28:22.000000 solc-json-parser-0.1.5/solc_json_parser.egg-info/top_level.txt
+drwxr-xr-x   0 garfield  (1000) garfield  (1000)        0 2023-05-23 08:34:20.484207 solc-json-parser-0.1.8/
+-rw-r--r--   0 garfield  (1000) garfield  (1000)     2112 2023-05-23 08:34:20.484207 solc-json-parser-0.1.8/PKG-INFO
+-rw-r--r--   0 garfield  (1000) garfield  (1000)     1945 2023-05-23 08:26:08.000000 solc-json-parser-0.1.8/README.md
+-rw-r--r--   0 garfield  (1000) garfield  (1000)      197 2023-05-23 08:34:20.484207 solc-json-parser-0.1.8/setup.cfg
+-rw-r--r--   0 garfield  (1000) garfield  (1000)      723 2023-05-23 08:28:56.000000 solc-json-parser-0.1.8/setup.py
+drwxr-xr-x   0 garfield  (1000) garfield  (1000)        0 2023-05-23 08:34:20.480874 solc-json-parser-0.1.8/solc_json_parser/
+-rw-r--r--   0 garfield  (1000) garfield  (1000)        0 2023-04-27 08:13:47.000000 solc-json-parser-0.1.8/solc_json_parser/__init__.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)     3827 2023-04-27 08:13:47.000000 solc-json-parser-0.1.8/solc_json_parser/abi.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)    10624 2023-05-23 08:26:08.000000 solc-json-parser-0.1.8/solc_json_parser/ast_shared.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)    22999 2023-05-23 08:26:08.000000 solc-json-parser-0.1.8/solc_json_parser/base_parser.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)    15925 2023-05-23 08:32:50.000000 solc-json-parser-0.1.8/solc_json_parser/combined_json_parser.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)       33 2023-04-27 08:13:47.000000 solc-json-parser-0.1.8/solc_json_parser/consts.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)     1418 2023-04-27 08:13:47.000000 solc-json-parser-0.1.8/solc_json_parser/fields.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)     2498 2023-04-27 08:13:47.000000 solc-json-parser-0.1.8/solc_json_parser/fix_imports.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)     7796 2023-04-27 08:13:47.000000 solc-json-parser-0.1.8/solc_json_parser/flatten.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)     3414 2023-04-27 08:13:47.000000 solc-json-parser-0.1.8/solc_json_parser/opcodes.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)    49761 2023-05-17 03:42:45.000000 solc-json-parser-0.1.8/solc_json_parser/parser.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)    12815 2023-05-23 08:26:08.000000 solc-json-parser-0.1.8/solc_json_parser/standard_json_parser.py
+-rw-r--r--   0 garfield  (1000) garfield  (1000)      221 2023-05-02 09:03:44.000000 solc-json-parser-0.1.8/solc_json_parser/version_cfg.py
+drwxr-xr-x   0 garfield  (1000) garfield  (1000)        0 2023-05-23 08:34:20.484207 solc-json-parser-0.1.8/solc_json_parser.egg-info/
+-rw-r--r--   0 garfield  (1000) garfield  (1000)     2112 2023-05-23 08:34:20.000000 solc-json-parser-0.1.8/solc_json_parser.egg-info/PKG-INFO
+-rw-r--r--   0 garfield  (1000) garfield  (1000)      626 2023-05-23 08:34:20.000000 solc-json-parser-0.1.8/solc_json_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 garfield  (1000) garfield  (1000)        1 2023-05-23 08:34:20.000000 solc-json-parser-0.1.8/solc_json_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 garfield  (1000) garfield  (1000)       89 2023-05-23 08:34:20.000000 solc-json-parser-0.1.8/solc_json_parser.egg-info/requires.txt
+-rw-r--r--   0 garfield  (1000) garfield  (1000)       17 2023-05-23 08:34:20.000000 solc-json-parser-0.1.8/solc_json_parser.egg-info/top_level.txt
```

### Comparing `solc-json-parser-0.1.5/setup.py` & `solc-json-parser-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='solc-json-parser',
     packages=find_packages(include=['solc_json_parser']),
-    version='0.1.5',
+    version='0.1.8',
     description='AST parser from solc json file',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='SBIP',
     license='MIT',
     install_requires=['addict>=2.4.0',
                       'py_solc_x>=1.1.1',
                       'semantic_version>=2.9.0',
                       'pycryptodome>=3.16.0',
                       'utils>=1.0.1'],
     setup_requires=['pytest-runner'],
-    tests_require=['pytest>-4.4.1'],
+    tests_require=['pytest>=4.4.1'],
     test_suite='tests',
 )
```

### Comparing `solc-json-parser-0.1.5/solc_json_parser/flatten.py` & `solc-json-parser-0.1.8/solc_json_parser/flatten.py`

 * *Files identical despite different names*

### Comparing `solc-json-parser-0.1.5/solc_json_parser/parser.py` & `solc-json-parser-0.1.8/solc_json_parser/parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 import json
 import os
 import re
 from typing import Collection, Dict, Optional, List, Any, Tuple, Union
 from functools import cached_property, cache, reduce
 from Crypto.Hash import keccak
 
+from solc_json_parser.ast_shared import deprecated_class
+
 try:
-    from fields import Field, Function, ContractData, Modifier, Event
+    from fields import Field, Function, ContractData, Modifier, Event, Literal
     from version_cfg import v_keys
     import consts
 except:
-    from solc_json_parser.fields import Field, Function, ContractData, Modifier, Event
+    from solc_json_parser.fields import Field, Function, ContractData, Modifier, Event, Literal
     from solc_json_parser.version_cfg import v_keys
     import solc_json_parser.consts
 
 SOLC_JSON_AST_FOLDER = "./solc_json_ast"
 PARSED_JSON = "./parsed_json"
 
 INSTALLABLE_VERSION = []
@@ -70,52 +72,34 @@
         else:
             return None
     if len(nkeys) > 0 and nd:
         return get_in(nd, *nkeys)
     return nd
 
 
-def get_candidates():
+def get_all_installable_versions():
     '''
     Returns a cached list of solc versions available for install,
     version list is sorted in ascending order
     '''
     global INSTALLABLE_VERSION
     if INSTALLABLE_VERSION:
         return INSTALLABLE_VERSION
     else:
         INSTALLABLE_VERSION = sorted(solcx.get_installable_solc_versions())
         return INSTALLABLE_VERSION
 
-
-def select_available_version(version_str: str, install=False) -> Optional[str]:
-    '''Switch to current or the next semantic version available to use. Returns the version selected.'''
-    version = Version(version_str)
-    candidates = get_candidates()
-    try:
-        chosen = next(v for v in candidates if v >= version)
-    except StopIteration:
-        logging.error(f'No candidate version available for {version}')
-        return None
-    ver = str(chosen)
-
-    if ver and install:
-        solc_bin = f'{solcx.get_solcx_install_folder()}/solc-v{ver}'
-        if not os.path.exists(solc_bin):
-            solcx.install_solc(chosen)
-
-    return ver
-
-
 def version_str_from_line(line) -> Optional[str]:
     '''
     Extract solc version string from input line
     '''
     if line.strip().startswith('pragma') and 'solidity' in line:
         ver = line.strip().split(maxsplit=2)[-1].split(';', maxsplit=1)[0]
+        if 'solidity' in ver:
+            ver = ver.split('solidity', maxsplit=1)[-1]
         ver = re.sub(r'([\^>=<~]+)\s+', r'\1', ver)
         return re.sub(r'(\.0+)', '.0', ver)
     return None
 
 
 def version_str_from_source(source_or_source_file: str) -> Optional[str]:
     inputs = source_or_source_file.split('\n') if '\n' in source_or_source_file else open(source_or_source_file, 'r')
@@ -125,81 +109,95 @@
 
     if not versions:
         logging.warning('No pragma directive found in source code')
         return None
 
     return ' '.join(set(versions))
 
-def detect_solc_version(source_or_source_file: str) -> Optional[str]:
-    '''
-    Detect solc version from a flatten source. Input can be a single file or source code string
-    '''
+def get_solc_candidates(source_or_source_file: str) -> List[str]:
     merged_version = version_str_from_source(source_or_source_file)
 
     if not merged_version:
-        return None
-
+        return []
+    merged_version = " ".join(merged_version.split()) #remove extra spaces
     spec = semantic_version.NpmSpec(merged_version)
-    candidates = get_candidates()
+    return [str(v) for v in spec.filter(get_all_installable_versions())]
 
-    # if we want the best candidate, this normally means higher version
-    # ver = spec.select(candidates)
-
-    # if we want the lowest version, will throw if no version matches
-    return str(next(spec.filter(candidates)))
+def detect_solc_version(source_or_source_file: str) -> Optional[str]:
+    '''
+    Detect solc version from a flatten source. Input can be a single file or source code string
+    '''
+    versions = get_solc_candidates(source_or_source_file)
+    return versions[-1] if versions else None
 
 
 def symbols_to_ids_from_ast_v8(ast: Dict[Any, Any]) -> Dict[str, int]:
     syms = [c['ast']['exportedSymbols'] for c in ast.values()]
     return {k: v[0] for m in syms for k, v in m.items()}
 
 
 def symbols_to_ids_from_ast_v7(ast: Dict[Any, Any]) -> Dict[str, int]:
     syms = [c['ast']['attributes']['exportedSymbols'] for c in ast.values()]
     return {k: v[0] for m in syms for k, v in m.items()}
 
 
-def get_increased_version(current_version: str) -> str:
-    """
-    :param current_version:
-    :return: next solc valid version, e.g. 0.5.10 -> 0.5.11
-    """
-    # convert current version str to Version object
-    current_version_obj = Version(current_version)
-    next_version = select_available_version(str(current_version_obj.next_patch()), install=True)
-    if not next_version:
-        raise SolidityAstError(f'No next version available for {current_version}')
-    return str(next_version)
+def find_next_version_in_candidates(current_version: str, solc_candidates: List[str]) -> Tuple[str, List[str]]:
+    """Try to get the next version"""
+    ver = Version(current_version)
+    try_next_version = Version(major=ver.major, minor= ver.minor - 1, patch=0)
+    print(f'try_next_version: {try_next_version} solc_candidates: {solc_candidates}')
+    version = None
+    # print(f'try_next_version: {try_next_version} solc_candidates: {solc_candidates}')
+    if str(try_next_version) in solc_candidates:
+        version = str(try_next_version)
+        solc_candidates = [v for v in solc_candidates if Version(v) < try_next_version]
+
+    elif solc_candidates:
+        version = str(solc_candidates[-1])
+        solc_candidates = solc_candidates[:-1]
+    if not version:
+        raise ValueError(f'No next solc version available for {current_version}')
+    return version, solc_candidates
+
 
 
 class SolidityAstError(ValueError):
     pass
 
 
+DEFAULT_OPTIMIZER = {'enabled': True, 'runs': 200}
+
+@deprecated_class
 class SolidityAst():
 
     FIELD_VISIBILITY_ALL = frozenset(('default', 'internal', 'public', 'private'))
     FIELD_VISIBILITY_NON_PRIVATE = frozenset(('default', 'internal', 'public'))
 
     FUNC_VISIBILITY_ALL = frozenset(('external', 'private', 'internal', 'public'))
     FUNC_VISIBILITY_NON_PRIVATE = frozenset(('external', 'internal', 'public'))
 
-    def __init__(self, contract_source_path: str, version=None, retry_num=None, solc_options={}):
+    def __init__(self, contract_source_path: Optional[str], version=None, retry_num=None, standard_json: Optional[Dict]=None, standard_json_str: Optional[str]=None,
+                 solc_options={}, lazy=False, solc_outputs=None, try_install_solc=True):
         '''
     Compile the input contract and create a SolidityAst object.
 
     Parameters:
     contract_source_path: str, required
         a path to the solidity source file or source code as string.
     version:  str, optional
         solc version to use for compile the contract. If not provided will use auto detected solc version.
         Note that SolidityAst will try to compile the contract starting from the lowest detected solc version first, increase the solc version each time when compilation fails.
     retry_num: int, optional
         Maximum number of solc versions to try to compile the contract
-
+    lazy: bool, optional
+        When true, you need to call `build()` explicitly to compile and parse the contract.
+    solc_outputs: List, optional
+        When non empty, only the specified outputs will be returned by the solc compiler.
+    no_install: bool, optional
+        When true, will not check and install the solc
 
     solc_options: Dict, optional
     The optionsl passed to the solc compiler, the following options are supports:
     overwrite : bool, optional
         Overwrite existing files (used in combination with `output_dir`)
     evm_version: str, optional
         Select the desired EVM version. Valid options depend on the `solc` version.
@@ -237,29 +235,36 @@
             self.file_path = contract_source_path
             self.file_path = os.path.abspath(contract_source_path)
             self.root_path = os.path.dirname(contract_source_path)
             with open(contract_source_path, 'r') as f:
                 self.source = f.read()
 
         self.original_compilation_output :Optional[Dict] = None
+        self.try_install_solc = try_install_solc
+        self.solc_outputs = solc_outputs
         self.solc_options = solc_options
         self.import_remappings = solc_options.get('import_remappings')
         base_path = solc_options.get('base_path')
         self.base_path = os.path.abspath(base_path) if base_path else None
         self.allow_paths = solc_options.get('allow_paths')
         self.retry_num = retry_num or 0
-        self.exact_version: str   = version or detect_solc_version(self.source) or consts.DEFAULT_SOLC_VERSION
-        self.version_key: str     = self._get_version_key()
-        self.keys: addict.Dict    = v_keys[self.version_key]
+        self.allowed_solc_versions = get_solc_candidates(self.source) or get_all_installable_versions()
+        self.solc_candidates = list(self.allowed_solc_versions)
+        self.exact_version: str   = version or self.solc_candidates[-1] or consts.DEFAULT_SOLC_VERSION
         self.exported_symbols: Dict[str, int] = {} # contract name -> id mapping, to be determined in _parse()
         self.id_to_symbols: Dict[int, str] = {} # reverse mapping of exported_symbols
-        self.solc_compile_outputs = ['abi', 'bin', 'bin-runtime', 'srcmap', 'srcmap-runtime', 'asm', 'opcodes', 'ast']
-        if self.v8:
-            self.solc_compile_outputs += ['generated-sources-runtime', 'generated-sources']
 
+        self.version_key: str     = self._get_version_key()
+        self.keys: addict.Dict    = v_keys[self.version_key]
+        self.prepare_by_version()
+
+        if not lazy:
+            self.build()
+
+    def build(self):
         self.compile()
         self.contracts_dict: Dict = self._parse()
 
     @cached_property
     def raw_version(self):
         return version_str_from_source(self.source)
 
@@ -281,15 +286,15 @@
         line_number_range_raw = list(map(int, node.get('src').split(':')))
         start, offset, source_file_idx = line_number_range_raw
         line_number_range, source = self.get_line_number_range_and_source(line_number_range_raw)
         raw = source.encode()[start: start+offset].decode()
         return raw, line_number_range
 
     def get_signature(self, function_name, parameters, kind='function') -> str:
-        if kind in ['function', 'constructor']:
+        if kind in ['constructor']:
             return ''
 
         signature = "" + function_name + "("
         param_type_str = ""
         if self.v8:
             for param in parameters['parameters']:
                 param_type_str += param['typeDescriptions']['typeString'] + ", "
@@ -452,15 +457,15 @@
         contract_id, contract_kind, is_abstract, contract_name, base_contracts, line_number_range = contract_meta_data
 
         functions = []
         fields = []
         modifiers = []
         events = []
         keys = self.keys
-        for node in node.get(keys.children):
+        for node in node.get(keys.children, []):
             if node[keys.name] == "FunctionDefinition":
                 functions.append(self._process_function(node))
             elif node[keys.name] == "VariableDeclaration":
                 fields.append(self._process_field(node))
             elif node[keys.name] == "ModifierDefinition":
                 modifiers.append(self._process_modifier(node))
             elif node[keys.name] == "EventDefinition":
@@ -483,15 +488,15 @@
                             new_field.inherited_from = base_contract_name
                             contract.fields.append(new_field)
                         for function in base_contract.functions:
                             new_function = copy.deepcopy(function)
                             new_function.inherited_from = base_contract_name
                             contract.functions.append(new_function)
 
-        # self.save_solc_ast_json("multi_file5.0")
+        # self.save_solc_ast_json("test_literal")
         # if there are n contracts in the same file, there will be n keys in the json,
         # but we only need the first one[0], because it contains all the contracts, and the rest are the same
         # ast = self.solc_json_ast.get(list(self.solc_json_ast.keys())[0]).get('ast')
         data_dict = {}
         # use version key to get the correct version cfg
         keys = self.keys
         unique_file = set()
@@ -526,39 +531,62 @@
         if 'pragma solidity' in source_code:
             return source_code.split("pragma solidity")[1]\
                               .split(";")[0].strip()\
                                             .replace('^', '').replace('=', '').replace('>', '').replace('<', '')
         else:
             return None
 
+    def prepare_by_version(self):
+        """Prepare compilation outputs, etc by the current `exact_version`"""
+        ver = Version(self.exact_version)
+        outputs = ['abi', 'bin', 'bin-runtime', 'srcmap', 'srcmap-runtime', 'asm', 'opcodes', 'ast']
+
+        self.version_key: str     = self._get_version_key()
+        self.keys: addict.Dict    = v_keys[self.version_key]
+        # clear cache
+        try: del self.v8
+        except AttributeError: pass
+
+        if ver >= Version("0.6.5"):
+            outputs.append('storage-layout')
+
+        if self.v8:
+            outputs += ['generated-sources-runtime', 'generated-sources', ]
+
+        self.solc_compile_outputs = outputs
+
+
     def compile(self):
         current_working_dir = os.getcwd()
         try:
-            solcx.install_solc(self.exact_version)
+            if self.try_install_solc:
+                solcx.install_solc(self.exact_version)
             solcx.set_solc_version(self.exact_version)
             if self.root_path:
                 os.chdir(self.root_path)
                 self.root_path = os.getcwd()
 
             compiler_options = dict(self.solc_options)
             overwritten_options = dict(base_path=self.base_path,
                                        import_remappings=self.import_remappings,
-                                       output_values=self.solc_compile_outputs,
+                                       output_values=self.solc_outputs or self.solc_compile_outputs,
                                        solc_version=self.exact_version)
             compiler_options.update(overwritten_options)
             if self.compile_type == "file":
                 out = solcx.compile_files(self.file_path, **compiler_options)
             else:
                 out = solcx.compile_source(self.source, **compiler_options)
             self.original_compilation_output = out
             self.solc_json_ast = {k.split(':')[-1]: v for k, v in out.items()}
         except Exception as e:
             if self.retry_num > 0:
                 self.retry_num -= 1
-                self.exact_version = get_increased_version(self.exact_version)
+                # self.exact_version = get_increased_version(self.exact_version, install=self.try_install_solc)
+                self.exact_version, self.solc_candidates = find_next_version_in_candidates(self.exact_version, self.solc_candidates)
+                self.prepare_by_version()
                 self.compile()
             else:
                 raise SolidityAstError(f"Compile failed with solc version {self.exact_version}, err msg: {e}")
         finally:
             os.chdir(current_working_dir)
 
     def save_solc_ast_json(self, name: str):
@@ -749,15 +777,20 @@
         combined_json = self.solc_json_ast
         contract = combined_json.get(contract_name)
         if contract is None:
             raise SolidityAstError(f'Contract {contract_name} not found in compiled json')
         asm_data = contract.get('asm').get('.code') if deploy else contract.get('asm').get('.data')
         # deploys = contract.get('asm').get('.code')
         opcodes = contract.get('opcodes').split()
-        source_list = self.get_source_list()
+
+        # contract.get('asm').get('sourceList') is introduced in 0.8.15, it is not put in get_source_list() for 2 reasons
+        # 1. it is quite a new feature, get_source_list() is to support more common cases.
+        # 2. contract.get('asm').get('sourceList') requires you to know the contract name first, get_source_list() is
+        #    independent of contract names.
+        source_list = contract.get('asm').get('sourceList') if contract.get('asm').get('sourceList') else self.get_source_list()
 
         if not deploy:
             opcodes = SolidityAst.__skip_deploys(opcodes)
 
         if not (opcodes or asm_data):
             raise(SolidityAstError('Missing required params!'))
 
@@ -808,33 +841,49 @@
             op_idx += 1
 
         pc2idx = {v: k for k, v in idx2pc.items()}
         return dict(code=code, pc2idx=pc2idx, source_list=source_list, seen_targets=seen_targets)
 
     @cache
     def get_source_list(self):
+        """
+        explanation on `yul_support_flag`:
+        contract.get('asm').get('sourceList') is introduced very lately in 0.8.15. In this sourceList we get from the
+        output, "#utility.yul" is at last. For example, if there are two files, a.sol and b.sol, the sourceList will
+        look like: ["a.sol", "b.sol", "#utility.yul"]. But in the earlier version, we get the sourceList by analyzing
+        the AST. Yul is introduced in solidity in 0.7.2. So between 0.7.2 and 0.8.15, we want to get a same output
+        from self.get_source_list(). So we check if there are generated-sources and generated-sources-runtime in it
+        by using the yul_support_flag then we append "#utility.yul" to the list accordingly.
+        """
         source_list = []
         idx2path = {}
+        yul_support_flag = False
         for contract_name in self.solc_json_ast.keys():
             absolute_path = self.source_path_by_contract(contract_name)
             idx = get_in(self.solc_json_ast, contract_name, 'ast', 'src').split(':')[-1]
             idx2path[int(idx)] = absolute_path
+            if self.solc_json_ast.get(contract_name).get('generated-sources') and \
+                    self.solc_json_ast.get(contract_name).get('generated-sources-runtime'):
+                yul_support_flag = True
         sort_keys = sorted(idx2path.keys())
         for idx in sort_keys:
             source_list.append(idx2path[idx])
+
+        if yul_support_flag:
+            source_list.append("#utility.yul")
         return source_list
 
     def get_line_number_range_and_source(self, line_number_range_raw: list):
         start_index, offset, source_file_idx = line_number_range_raw
         source_list = self.get_source_list()
         source_path = self.__source_path_from_source_list(source_list, source_file_idx)
-        source_code = self.__source_code_from_source_path(source_path)
-        start_line = source_code[:start_index].count('\n') + 1
-        end_line = start_line + source_code[start_index:start_index + offset].count('\n')
-        return (start_line, end_line), source_code
+        source_code_bytes = self.__source_code_from_source_path(source_path).encode()
+        start_line = source_code_bytes[:start_index].decode().count('\n') + 1
+        end_line = start_line + source_code_bytes[start_index:start_index + offset].decode().count('\n')
+        return (start_line, end_line), source_code_bytes.decode()
 
     def source_path_by_contract(self, contract_name) -> Optional[str]:
         path = None
         if self.v8:
             path = get_in(self.solc_json_ast, contract_name, 'ast', 'absolutePath')
         else:
             path = get_in(self.solc_json_ast, contract_name, 'ast', 'attributes', 'absolutePath')
@@ -909,50 +958,52 @@
                 t.append(l + [None] * (3 - len(l)))
         parsed = [{'s': s if s != "" else None, 'l': l, 'f': f} for s, l, f in t]
         parsed = reduce(_reduce_fn, parsed, [{}])
         parsed = list(reversed(parsed[:-1]))
         return parsed
 
     def source_by_pc(self, contract_name: str, pc: int, deploy=False) -> Dict[str, Any]:
-        '''
+        """
         Get source code by program counter:
         - `pc`: program counter
         - `deploy`: set to true to search in deploy opcodes
-        '''
+        """
         code, pc2idx, source_list = itemgetter('code', 'pc2idx', 'source_list')(self.__parse_asm_data(contract_name, deploy=deploy))
         pc_idx = pc2idx.get(pc)
         part = code[pc_idx]
         if part.get('source') is not None:
             source_idx = part['source']
         else:
             src_mapping = self.solc_json_ast[contract_name]['srcmap-runtime']
             parsed_mapping = self.parse_src_mapping(src_mapping)
             mapping_idx = list(pc2idx.values()).index(pc_idx)
             source_idx = parsed_mapping[mapping_idx].get('f')
 
         begin, end = itemgetter('begin', 'end')(part)
         source_idx = source_idx if source_idx is not None else list(self.solc_json_ast.keys()).index(contract_name)
         source_path = self.__source_path_from_source_list(source_list, source_idx)
-        source_code = self.__source_code_from_source_path(source_path)
 
-        source = source_idx # WARN: assuming yul source is has index 1, not true for multi-source file contract
-        yul_index = len(source_list) - 1
-        if source == yul_index and self.v8 and not deploy:
+        # NOTE: assuming yul file is at the last in the generated source list
+        # e.g. [a.sol, util/b.sol, #utility.yul]
+        has_yul = len(source_list) > 1
+        yul_index = len(source_list) - 1 if has_yul else -1
+
+        if source_idx == yul_index and self.v8 and not deploy:
             combined_source = self.solc_json_ast[contract_name]['generated-sources-runtime'][0]['contents']
-        elif source == yul_index and self.v8 and deploy:
+        elif source_idx == yul_index and self.v8 and deploy:
             combined_source = self.solc_json_ast[contract_name]['generated-sources'][0]['contents']
         else:
-            combined_source = source_code
+            combined_source = self.__source_code_from_source_path(source_path)
         # assumes utf8 encoding here
         source_as_bytes = combined_source.encode()
         fragment = source_as_bytes[begin:end].decode()
         # print ("fragment ", fragment)
         linenums = (source_as_bytes[:begin].decode().count('\n') + 1,
                     source_as_bytes[:end].decode().count('\n') + 1)
-        return dict(pc=pc, fragment=fragment, begin=begin, end=end, linenums=linenums, source_idx=source, source_path=(source_path or self.file_path))
+        return dict(pc=pc, fragment=fragment, begin=begin, end=end, linenums=linenums, source_idx=source_idx, source_path=(source_path or self.file_path))
 
     def get_any(self, *keys) -> Any:
         '''Get any value by keys from the original compiled ast data'''
         return get_in(self.original_compilation_output, *keys)
 
     def get_deploy_bin_by_contract_name(self, contract_name: str) -> Optional[str]:
         return get_in(self.solc_json_ast, contract_name, 'bin')
@@ -961,14 +1012,116 @@
         '''Get fully qualified contract name from 34 character hash'''
         return next(full_name for full_name in self.original_compilation_output.keys() if keccak256(full_name)[:34] == hsh)
 
     def get_deploy_bin_by_hash(self, hsh: str) -> Optional[str]:
         '''Get deployment binary by hash of fully qualified contract / library name'''
         return self.get_any(self.qualified_name_from_hash(hsh), 'bin')
 
+    @staticmethod
+    def _process_literal_node(literals_nodes, only_value):
+        def _process_other_literal_node(literal_node, literals, only_value):
+            try:
+                if only_value:
+                    literals['other'].add(literal_node.str_value)
+                else:
+                    literals['other'].add(literal_node)
+            except AttributeError:
+                pass
+
+        literals = dict(number=set(), string=set(), address=set(), other=set())
+        for literal in literals_nodes:
+            try:
+                if literal.sub_type is None and literal.token_type == 'number':
+                    if only_value and literal.str_value.isdecimal():
+                        literals['number'].add(int(literal.str_value))
+                    else:
+                        literals['number'].add(literal)
+                elif literal.sub_type.startswith("address"):
+                    if only_value:
+                        literals['address'].add(literal.str_value)
+                    else:
+                        literals['address'].add(literal)
+                elif literal.sub_type.startswith("int"):
+                    if only_value:
+                        if literal.str_value.startswith('0x'):
+                            literals['number'].add(int(literal.str_value, 16))
+                        elif literal.sub_type.split()[1].isdecimal():
+                            literals['number'].add(int(literal.sub_type.split()[1]))
+                        else:
+                            literals['number'].add(int(literal.str_value))
+                    else:
+                        literals['number'].add(literal)
+                # check if string in token_type, ignore case
+                elif literal.sub_type.startswith("literal_string"):
+                    if only_value:
+                        literals['string'].add(literal.str_value)
+                    else:
+                        literals['string'].add(literal)
+                elif literal.sub_type.startswith("bool"):
+                    continue
+                else:
+                    _process_other_literal_node(literal, literals, only_value)
+            except Exception as e:
+                _process_other_literal_node(literal, literals, only_value)
+
+        return literals
+
+    def _traverse_nodes(self, node, literals_nodes):
+        if not isinstance(node, dict):
+            return
+
+        if node.get(self.keys.name) == 'Literal':
+            if self.v8 and node.get('typeDescriptions'):
+                literals_nodes.add(Literal(
+                    hex_value=node.get('hexValue'),
+                    str_value=node.get('value'),
+                    sub_type=node.get('typeDescriptions').get('typeString'),
+                    token_type=node.get('kind', ),
+                ))
+            elif not self.v8 and node.get('attributes'):
+                literals_nodes.add(Literal(
+                    hex_value=node.get('attributes').get('hexvalue'),
+                    str_value=node.get('attributes').get('value'),
+                    sub_type=node.get('attributes').get('type'),
+                    token_type=node.get('attributes').get('token'),
+                ))
+        else:
+            for k, v in node.items():
+                if isinstance(v, dict):
+                    self._traverse_nodes(v, literals_nodes)
+                if isinstance(v, list):
+                    for c in v:
+                        if isinstance(c, dict):
+                            self._traverse_nodes(c, literals_nodes)
+
+    def get_literals(self, contract_name: str, only_value=False) -> dict:
+        """
+        Get all literals(number, address, string, other) in the contract.
+        for 'other' type, if only_value is True, return the string value
+        - `contract_name`: contract_name in string
+        - `only_value`: set to true to get only values, otherwise get all literal objects
+        """
+
+        literals_nodes = set() # save data here
+        root_node = self.solc_json_ast[contract_name]['ast']
+        contract_node = None
+        for i, node in enumerate(root_node[self.keys.children]):
+            if node[self.keys.name] == "ContractDefinition":
+                info_node = node if self.v8 else node.get('attributes')
+                if info_node['name'] == contract_name:
+                    contract_node = node
+                    break
+
+        # traverse the dictionary and get all the literals recursively
+        self._traverse_nodes(contract_node, literals_nodes)
+
+        literals = self._process_literal_node(literals_nodes, only_value)
+
+        return literals
+
 
 if __name__ == '__main__':
     import argparse
     import glob
     import traceback
 
     parser = argparse.ArgumentParser()
```

