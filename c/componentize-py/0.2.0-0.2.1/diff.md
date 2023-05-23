# Comparing `tmp/componentize_py-0.2.0.tar.gz` & `tmp/componentize_py-0.2.1.tar.gz`

## Comparing `componentize_py-0.2.0.tar` & `componentize_py-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      156 1970-01-01 00:00:00.000000 componentize_py-0.2.0/local_dependencies/test-generator/Cargo.toml
--rw-r--r--   0     1001      123    32490 2023-05-22 23:12:10.000000 componentize_py-0.2.0/local_dependencies/test-generator/src/lib.rs
--rw-r--r--   0        0        0      264 1970-01-01 00:00:00.000000 componentize_py-0.2.0/local_dependencies/componentize-py-shared/Cargo.toml
--rw-r--r--   0     1001      123     1071 2023-05-22 23:12:10.000000 componentize_py-0.2.0/local_dependencies/componentize-py-shared/src/lib.rs
--rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 componentize_py-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123      374 2023-05-22 23:12:10.000000 componentize_py-0.2.0/.github/workflows/lint.sh
--rw-r--r--   0     1001      123     9949 2023-05-22 23:12:10.000000 componentize_py-0.2.0/.github/workflows/release.yaml
--rw-r--r--   0     1001      123     1505 2023-05-22 23:12:10.000000 componentize_py-0.2.0/.github/workflows/test.yaml
--rw-r--r--   0     1001      123       41 2023-05-22 23:12:10.000000 componentize_py-0.2.0/.gitignore
--rw-r--r--   0     1001      123      192 2023-05-22 23:12:10.000000 componentize_py-0.2.0/.gitmodules
--rw-r--r--   0     1001      123    66305 2023-05-22 23:12:10.000000 componentize_py-0.2.0/Cargo.lock
--rw-r--r--   0     1001      123    11602 2023-05-22 23:12:10.000000 componentize_py-0.2.0/LICENSE
--rw-r--r--   0     1001      123     1275 2023-05-22 23:12:10.000000 componentize_py-0.2.0/README.md
--rw-r--r--   0     1001      123     7830 2023-05-22 23:12:10.000000 componentize_py-0.2.0/build.rs
--rw-r--r--   0     1001      123      149 2023-05-22 23:12:10.000000 componentize_py-0.2.0/pyo3-config.txt
--rw-r--r--   0     1001      123      665 2023-05-22 23:12:10.000000 componentize_py-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123     7357 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/abi.rs
--rw-r--r--   0     1001      123      111 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/bin/componentize-py.rs
--rw-r--r--   0     1001      123    87792 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/bindgen.rs
--rw-r--r--   0     1001      123     5208 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/command.rs
--rw-r--r--   0     1001      123    25711 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/componentize.rs
--rw-r--r--   0     1001      123    10003 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/convert.rs
--rw-r--r--   0     1001      123     5883 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     1641 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/python.rs
--rw-r--r--   0     1001      123    37547 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/summary.rs
--rw-r--r--   0     1001      123    17023 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/test/echoes.rs
--rw-r--r--   0     1001      123       80 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/test/echoes_generated.rs
--rw-r--r--   0     1001      123     2550 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/test/simple.rs
--rw-r--r--   0     1001      123     1826 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/test/wit/echoes.wit
--rw-r--r--   0     1001      123      103 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/test/wit/simple-export.wit
--rw-r--r--   0     1001      123      185 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/test/wit/simple-import-and-export.wit
--rw-r--r--   0     1001      123     4325 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/test.rs
--rw-r--r--   0     1001      123      991 2023-05-22 23:12:10.000000 componentize_py-0.2.0/src/util.rs
--rw-r--r--   0        0        0     1724 1970-01-01 00:00:00.000000 componentize_py-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      156 1970-01-01 00:00:00.000000 componentize_py-0.2.1/local_dependencies/test-generator/Cargo.toml
+-rw-r--r--   0     1001      123    32490 2023-05-23 15:07:26.000000 componentize_py-0.2.1/local_dependencies/test-generator/src/lib.rs
+-rw-r--r--   0        0        0      264 1970-01-01 00:00:00.000000 componentize_py-0.2.1/local_dependencies/componentize-py-shared/Cargo.toml
+-rw-r--r--   0     1001      123     1071 2023-05-23 15:07:26.000000 componentize_py-0.2.1/local_dependencies/componentize-py-shared/src/lib.rs
+-rw-r--r--   0        0        0      959 1970-01-01 00:00:00.000000 componentize_py-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123      374 2023-05-23 15:07:26.000000 componentize_py-0.2.1/.github/workflows/lint.sh
+-rw-r--r--   0     1001      123     9949 2023-05-23 15:07:26.000000 componentize_py-0.2.1/.github/workflows/release.yaml
+-rw-r--r--   0     1001      123     1505 2023-05-23 15:07:26.000000 componentize_py-0.2.1/.github/workflows/test.yaml
+-rw-r--r--   0     1001      123       41 2023-05-23 15:07:26.000000 componentize_py-0.2.1/.gitignore
+-rw-r--r--   0     1001      123      192 2023-05-23 15:07:26.000000 componentize_py-0.2.1/.gitmodules
+-rw-r--r--   0     1001      123    66305 2023-05-23 15:07:26.000000 componentize_py-0.2.1/Cargo.lock
+-rw-r--r--   0     1001      123    11602 2023-05-23 15:07:26.000000 componentize_py-0.2.1/LICENSE
+-rw-r--r--   0     1001      123     1325 2023-05-23 15:07:26.000000 componentize_py-0.2.1/README.md
+-rw-r--r--   0     1001      123     7830 2023-05-23 15:07:26.000000 componentize_py-0.2.1/build.rs
+-rw-r--r--   0     1001      123      149 2023-05-23 15:07:26.000000 componentize_py-0.2.1/pyo3-config.txt
+-rw-r--r--   0     1001      123      665 2023-05-23 15:07:26.000000 componentize_py-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123     7357 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/abi.rs
+-rw-r--r--   0     1001      123      111 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/bin/componentize-py.rs
+-rw-r--r--   0     1001      123    87792 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/bindgen.rs
+-rw-r--r--   0     1001      123     5203 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/command.rs
+-rw-r--r--   0     1001      123    25711 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/componentize.rs
+-rw-r--r--   0     1001      123    10003 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/convert.rs
+-rw-r--r--   0     1001      123     5883 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123     1641 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/python.rs
+-rw-r--r--   0     1001      123    37547 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/summary.rs
+-rw-r--r--   0     1001      123    17023 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/test/echoes.rs
+-rw-r--r--   0     1001      123       80 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/test/echoes_generated.rs
+-rw-r--r--   0     1001      123     2550 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/test/simple.rs
+-rw-r--r--   0     1001      123     1826 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/test/wit/echoes.wit
+-rw-r--r--   0     1001      123      103 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/test/wit/simple-export.wit
+-rw-r--r--   0     1001      123      185 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/test/wit/simple-import-and-export.wit
+-rw-r--r--   0     1001      123     4325 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/test.rs
+-rw-r--r--   0     1001      123      991 2023-05-23 15:07:26.000000 componentize_py-0.2.1/src/util.rs
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 componentize_py-0.2.1/PKG-INFO
```

### Comparing `componentize_py-0.2.0/local_dependencies/test-generator/src/lib.rs` & `componentize_py-0.2.1/local_dependencies/test-generator/src/lib.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/local_dependencies/componentize-py-shared/src/lib.rs` & `componentize_py-0.2.1/local_dependencies/componentize-py-shared/src/lib.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/Cargo.toml` & `componentize_py-0.2.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "componentize-py"
-version = "0.2.0"
+version = "0.2.1"
 edition = "2021"
 exclude = ["cpython"]
 
 [lib]
 name = "componentize_py"
 crate-type = ["cdylib", "rlib"]
```

### Comparing `componentize_py-0.2.0/.github/workflows/release.yaml` & `componentize_py-0.2.1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/.github/workflows/test.yaml` & `componentize_py-0.2.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/Cargo.lock` & `componentize_py-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -325,15 +325,15 @@
 name = "clap_lex"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
 
 [[package]]
 name = "componentize-py"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "anyhow",
  "async-trait",
  "bincode",
  "cap-std 1.0.15",
  "clap",
  "componentize-py-shared",
```

### Comparing `componentize_py-0.2.0/LICENSE` & `componentize_py-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/README.md` & `componentize_py-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 # componentize-py
 
-This is a prototype of a tool to convert a Python application to a [WebAssembly
+This is a tool to convert a Python application to a [WebAssembly
 component](https://github.com/WebAssembly/component-model).  It takes the
 following as input:
 
 - a [WIT](https://github.com/WebAssembly/component-model/blob/main/design/mvp/WIT.md) file or directory
 - the name of a [WIT world](https://github.com/WebAssembly/component-model/blob/main/design/mvp/WIT.md#wit-worlds) defined in the above file or directory
 - the name of a Python module which targets said world
 - a list of directories in which to find the Python module and its dependencies
 
 The output is a component which may be run using
 e.g. [`wasmtime`](https://github.com/bytecodealliance/wasmtime).  See the
-[tests](tests) for examples.
+[tests](src/test) for examples.
+
+## Installing from PyPI
+
+```
+pip install componentize-py
+```
 
 ## Build Prerequisites
 
 - [WASI SDK](https://github.com/WebAssembly/wasi-sdk) v16 (later versions may work, but have not yet been tested)
     - Install this to `/opt/wasi-sdk`, or else specify an alternative location via the `WASI_SDK_PATH` environment variable
 - Tools needed to build [CPython](https://github.com/python/cpython) (e.g. Make, Clang, etc.)
 - [Rust](https://rustup.rs/) v1.68 or later, including the `wasm32-wasi` and `wasm32-unknown-unkown` targets
```

### Comparing `componentize_py-0.2.0/build.rs` & `componentize_py-0.2.1/build.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/pyproject.toml` & `componentize_py-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "maturin"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [project]
 name = "componentize-py"
-version = "0.2.0"
+version = "0.2.1"
 description = "Tool to package Python applications as WebAssembly components"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [ { name = "Fermyon Engineering", email = "engineering@fermyon.com" } ]
 maintainers = [ { name = "Fermyon Engineering", email = "engineering@fermyon.com" } ]
 keywords = [ "webassembly", "wasm", "component" ]
```

### Comparing `componentize_py-0.2.0/src/abi.rs` & `componentize_py-0.2.1/src/abi.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/bindgen.rs` & `componentize_py-0.2.1/src/bindgen.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/command.rs` & `componentize_py-0.2.1/src/command.rs`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     /// Directory to which bindings should be written.
     ///
     /// This will be created if it does not already exist.
     pub output_dir: PathBuf,
 }
 
 pub fn run<T: Into<OsString> + Clone, I: IntoIterator<Item = T>>(args: I) -> Result<()> {
-    let options = Options::try_parse_from(args)?;
+    let options = Options::parse_from(args);
     match options.command {
         Command::Componentize(opts) => componentize(options.common, opts),
         Command::Bindings(opts) => generate_bindings(options.common, opts),
     }
 }
 
 fn generate_bindings(common: Common, bindings: Bindings) -> Result<()> {
```

### Comparing `componentize_py-0.2.0/src/componentize.rs` & `componentize_py-0.2.1/src/componentize.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/convert.rs` & `componentize_py-0.2.1/src/convert.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/lib.rs` & `componentize_py-0.2.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/python.rs` & `componentize_py-0.2.1/src/python.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/summary.rs` & `componentize_py-0.2.1/src/summary.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/test/echoes.rs` & `componentize_py-0.2.1/src/test/echoes.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/test/simple.rs` & `componentize_py-0.2.1/src/test/simple.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/test/wit/echoes.wit` & `componentize_py-0.2.1/src/test/wit/echoes.wit`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/test.rs` & `componentize_py-0.2.1/src/test.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/src/util.rs` & `componentize_py-0.2.1/src/util.rs`

 * *Files identical despite different names*

### Comparing `componentize_py-0.2.0/PKG-INFO` & `componentize_py-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 Metadata-Version: 2.1
 Name: componentize-py
-Version: 0.2.0
+Version: 0.2.1
 License-File: LICENSE
 Summary: Tool to package Python applications as WebAssembly components
 Keywords: webassembly,wasm,component
 Author-email: Fermyon Engineering <engineering@fermyon.com>
 Maintainer-email: Fermyon Engineering <engineering@fermyon.com>
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: repository, https://github.com/dicej/componentize-py
 
 # componentize-py
 
-This is a prototype of a tool to convert a Python application to a [WebAssembly
+This is a tool to convert a Python application to a [WebAssembly
 component](https://github.com/WebAssembly/component-model).  It takes the
 following as input:
 
 - a [WIT](https://github.com/WebAssembly/component-model/blob/main/design/mvp/WIT.md) file or directory
 - the name of a [WIT world](https://github.com/WebAssembly/component-model/blob/main/design/mvp/WIT.md#wit-worlds) defined in the above file or directory
 - the name of a Python module which targets said world
 - a list of directories in which to find the Python module and its dependencies
 
 The output is a component which may be run using
 e.g. [`wasmtime`](https://github.com/bytecodealliance/wasmtime).  See the
-[tests](tests) for examples.
+[tests](src/test) for examples.
+
+## Installing from PyPI
+
+```
+pip install componentize-py
+```
 
 ## Build Prerequisites
 
 - [WASI SDK](https://github.com/WebAssembly/wasi-sdk) v16 (later versions may work, but have not yet been tested)
     - Install this to `/opt/wasi-sdk`, or else specify an alternative location via the `WASI_SDK_PATH` environment variable
 - Tools needed to build [CPython](https://github.com/python/cpython) (e.g. Make, Clang, etc.)
 - [Rust](https://rustup.rs/) v1.68 or later, including the `wasm32-wasi` and `wasm32-unknown-unkown` targets
```

