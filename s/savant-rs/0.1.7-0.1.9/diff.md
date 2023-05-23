# Comparing `tmp/savant_rs-0.1.7.tar.gz` & `tmp/savant_rs-0.1.9.tar.gz`

## Comparing `savant_rs-0.1.7.tar` & `savant_rs-0.1.9.tar`

### file list

```diff
@@ -1,50 +1,60 @@
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 savant_rs-0.1.7/Cargo.toml
--rw-r--r--   0     1001      123     1614 2023-05-17 10:52:40.000000 savant_rs-0.1.7/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      466 2023-05-17 10:52:40.000000 savant_rs-0.1.7/.gitignore
--rw-r--r--   0     1001      123    11357 2023-05-17 10:52:40.000000 savant_rs-0.1.7/LICENSE
--rw-r--r--   0     1001      123      514 2023-05-17 10:52:40.000000 savant_rs-0.1.7/README.md
--rw-r--r--   0     1001      123      769 2023-05-17 10:52:40.000000 savant_rs-0.1.7/benches/batch_snapshot.rs
--rw-r--r--   0     1001      123     1197 2023-05-17 10:52:40.000000 savant_rs-0.1.7/benches/message_save_load.rs
--rw-r--r--   0     1001      123       71 2023-05-17 10:52:40.000000 savant_rs-0.1.7/build.rs
--rw-r--r--   0     1001      123      459 2023-05-17 10:52:40.000000 savant_rs-0.1.7/pyproject.toml
--rw-r--r--   0     1001      123     2351 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/primitives/bbox/ops.py
--rw-r--r--   0     1001      123     2531 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/primitives/bbox/savant_scale.py
--rw-r--r--   0     1001      123      783 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/primitives/buf_copy.py
--rw-r--r--   0     1001      123     3785 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/primitives/frame_ops.py
--rw-r--r--   0     1001      123     1116 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/primitives/polygon_match.py
--rw-r--r--   0     1001      123      200 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/test_pyo3_access/get_copy.py
--rw-r--r--   0     1001      123      184 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/test_pyo3_access/get_proxy.py
--rw-r--r--   0     1001      123      407 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/test_pyo3_access/get_pure.py
--rw-r--r--   0     1001      123      196 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/test_pyo3_access/get_py.py
--rw-r--r--   0     1001      123      213 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/test_pyo3_access/get_take.py
--rw-r--r--   0     1001      123      269 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/utils/fps_meter/rust_fps_meter.py
--rw-r--r--   0     1001      123     3515 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/utils/fps_meter/savant_fps_meter.py
--rw-r--r--   0     1001      123      627 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/utils/numpy_ops.py
--rw-r--r--   0     1001      123     3387 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/utils/symbol_mapper/rust_symbol_mapper.py
--rw-r--r--   0     1001      123     7231 2023-05-17 10:52:40.000000 savant_rs-0.1.7/python/utils/symbol_mapper/savant_symbol_mapper.py
--rw-r--r--   0     1001      123      997 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/lib.rs
--rw-r--r--   0     1001      123    14160 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/attribute.rs
--rw-r--r--   0     1001      123    16607 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/bbox.rs
--rw-r--r--   0     1001      123     1141 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/eos.rs
--rw-r--r--   0     1001      123     2807 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/loader.rs
--rw-r--r--   0     1001      123     2135 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/saver.rs
--rw-r--r--   0     1001      123     1932 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/video/batch.rs
--rw-r--r--   0     1001      123    28830 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/video/frame.rs
--rw-r--r--   0     1001      123    14359 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/video/object.rs
--rw-r--r--   0     1001      123       46 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message/video.rs
--rw-r--r--   0     1001      123     6736 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/message.rs
--rw-r--r--   0     1001      123      853 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/point.rs
--rw-r--r--   0     1001      123    14179 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/polygonal_area.rs
--rw-r--r--   0     1001      123     2558 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/segment.rs
--rw-r--r--   0     1001      123       87 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives/to_json_value.rs
--rw-r--r--   0     1001      123     1678 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/primitives.rs
--rw-r--r--   0     1001      123     5863 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/test.rs
--rw-r--r--   0     1001      123     2521 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/tests_pyo3_access.rs
--rw-r--r--   0     1001      123     6745 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils/bbox.rs
--rw-r--r--   0     1001      123      713 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils/conversions.rs
--rw-r--r--   0     1001      123     5961 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils/fps_meter.rs
--rw-r--r--   0     1001      123     8546 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils/numpy_utils.rs
--rw-r--r--   0     1001      123    21129 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils/symbol_mapper.rs
--rw-r--r--   0     1001      123     2719 2023-05-17 10:52:40.000000 savant_rs-0.1.7/src/utils.rs
--rw-r--r--   0     1001      123    38841 2023-05-17 10:54:16.000000 savant_rs-0.1.7/Cargo.lock
--rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 savant_rs-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      123     1614 2023-05-22 12:57:18.000000 savant_rs-0.1.9/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      466 2023-05-22 12:57:18.000000 savant_rs-0.1.9/.gitignore
+-rw-r--r--   0     1001      123    11357 2023-05-22 12:57:18.000000 savant_rs-0.1.9/LICENSE
+-rw-r--r--   0     1001      123      513 2023-05-22 12:57:18.000000 savant_rs-0.1.9/Makefile
+-rw-r--r--   0     1001      123      514 2023-05-22 12:57:18.000000 savant_rs-0.1.9/README.md
+-rw-r--r--   0     1001      123      769 2023-05-22 12:57:18.000000 savant_rs-0.1.9/benches/batch_snapshot.rs
+-rw-r--r--   0     1001      123     2389 2023-05-22 12:57:18.000000 savant_rs-0.1.9/benches/bench_object_filter.rs
+-rw-r--r--   0     1001      123     1197 2023-05-22 12:57:18.000000 savant_rs-0.1.9/benches/message_save_load.rs
+-rw-r--r--   0     1001      123       71 2023-05-22 12:57:18.000000 savant_rs-0.1.9/build.rs
+-rw-r--r--   0     1001      123      459 2023-05-22 12:57:18.000000 savant_rs-0.1.9/pyproject.toml
+-rw-r--r--   0     1001      123     2351 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/primitives/bbox/ops.py
+-rw-r--r--   0     1001      123     2531 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/primitives/bbox/savant_scale.py
+-rw-r--r--   0     1001      123      783 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/primitives/buf_copy.py
+-rw-r--r--   0     1001      123     3815 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/primitives/frame_ops.py
+-rw-r--r--   0     1001      123     1116 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/primitives/polygon_match.py
+-rw-r--r--   0     1001      123      200 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/test_pyo3_access/get_copy.py
+-rw-r--r--   0     1001      123      184 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/test_pyo3_access/get_proxy.py
+-rw-r--r--   0     1001      123      407 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/test_pyo3_access/get_pure.py
+-rw-r--r--   0     1001      123      196 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/test_pyo3_access/get_py.py
+-rw-r--r--   0     1001      123      213 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/test_pyo3_access/get_take.py
+-rw-r--r--   0     1001      123      269 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/utils/fps_meter/rust_fps_meter.py
+-rw-r--r--   0     1001      123     3515 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/utils/fps_meter/savant_fps_meter.py
+-rw-r--r--   0     1001      123     1263 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/utils/numpy_ops.py
+-rw-r--r--   0     1001      123     3387 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/utils/symbol_mapper/rust_symbol_mapper.py
+-rw-r--r--   0     1001      123     7231 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/utils/symbol_mapper/savant_symbol_mapper.py
+-rw-r--r--   0     1001      123     1078 2023-05-22 12:57:18.000000 savant_rs-0.1.9/python/video_object_query/query.py
+-rw-r--r--   0     1001      123     1241 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/lib.rs
+-rw-r--r--   0     1001      123    14160 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/attribute.rs
+-rw-r--r--   0     1001      123    16247 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/bbox.rs
+-rw-r--r--   0     1001      123     1141 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/eos.rs
+-rw-r--r--   0     1001      123     2798 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/loader.rs
+-rw-r--r--   0     1001      123     2126 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/saver.rs
+-rw-r--r--   0     1001      123     1892 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/video/batch.rs
+-rw-r--r--   0     1001      123    29114 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/video/frame.rs
+-rw-r--r--   0     1001      123     3705 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/video/object/query/functions.rs
+-rw-r--r--   0     1001      123      506 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/video/object/query/macros.rs
+-rw-r--r--   0     1001      123    12195 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/video/object/query/py.rs
+-rw-r--r--   0     1001      123    16212 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/video/object/query.rs
+-rw-r--r--   0     1001      123    15169 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/video/object.rs
+-rw-r--r--   0     1001      123       46 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message/video.rs
+-rw-r--r--   0     1001      123     6739 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/message.rs
+-rw-r--r--   0     1001      123      853 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/point.rs
+-rw-r--r--   0     1001      123    14075 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/polygonal_area.rs
+-rw-r--r--   0     1001      123     2558 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/segment.rs
+-rw-r--r--   0     1001      123       87 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives/to_json_value.rs
+-rw-r--r--   0     1001      123     1779 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/primitives.rs
+-rw-r--r--   0     1001      123     5970 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/test.rs
+-rw-r--r--   0     1001      123     2521 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/tests_pyo3_access.rs
+-rw-r--r--   0     1001      123     6749 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/utils/bbox.rs
+-rw-r--r--   0     1001      123      717 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/utils/conversions.rs
+-rw-r--r--   0     1001      123     5961 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/utils/fps_meter.rs
+-rw-r--r--   0     1001      123     8478 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/utils/np/np_nalgebra.rs
+-rw-r--r--   0     1001      123     5973 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/utils/np/np_ndarray.rs
+-rw-r--r--   0     1001      123      562 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/utils/np.rs
+-rw-r--r--   0     1001      123      197 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/utils/python.rs
+-rw-r--r--   0     1001      123    21625 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/utils/symbol_mapper.rs
+-rw-r--r--   0     1001      123     2982 2023-05-22 12:57:18.000000 savant_rs-0.1.9/src/utils.rs
+-rw-r--r--   0     1001      123    40517 2023-05-22 12:58:59.000000 savant_rs-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 savant_rs-0.1.9/PKG-INFO
```

### Comparing `savant_rs-0.1.7/Cargo.toml` & `savant_rs-0.1.9/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "savant_rs"
-version = "0.1.7"
+version = "0.1.9"
 edition = "2021"
 authors = ["Ivan Kudriavtsev <ivan.a.kudryavtsev@gmail.com>"]
 description = "Savant rust optimization library"
 homepage = "https://github.com/insight-platform/savant-rs"
 repository = "https://github.com/insight-platform/savant-rs"
 readme = "README.md"
 keywords = ["computer-vision", "video-processing"]
@@ -12,29 +12,34 @@
 license="Apache-2.0"
 rust-version = "1.66"
 
 [lib]
 crate-type = ["cdylib", "lib"]
 
 [dependencies]
+jmespath = { version = "0.3", features = ["sync"] }
+lru = "0.10"
 serde_json = "1.0"
+serde_yaml = "0.9"
+serde = { version = "1.0", features = ["derive"] }
 itertools = "0.10"
 anyhow = "1.0"
 thiserror = "1.0"
 geo = "0.24"
 rayon = "1.7"
 env_logger = "0.10"
 rkyv = { version = "0.7", features = ["validation", "archive_le"] }
 numpy = {version = "0.18", features = ["nalgebra"]}
 pyo3-log = "0.8"
 derive_builder = "0.12"
 num_cpus = "1.15"
 hashbrown = "0.13"
 lazy_static = "1.4"
 nalgebra = "0.32"
+ndarray = "0.15"
 num-traits = "0.2"
 
 [dependencies.pyo3]
 version = "0.18"
 
 [dev-dependencies]
 serial_test = "2.0"
```

### Comparing `savant_rs-0.1.7/.github/workflows/CI.yml` & `savant_rs-0.1.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/LICENSE` & `savant_rs-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/README.md` & `savant_rs-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/benches/batch_snapshot.rs` & `savant_rs-0.1.9/benches/batch_snapshot.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/benches/message_save_load.rs` & `savant_rs-0.1.9/benches/message_save_load.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/python/primitives/bbox/ops.py` & `savant_rs-0.1.9/python/primitives/bbox/ops.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/python/primitives/bbox/savant_scale.py` & `savant_rs-0.1.9/python/primitives/bbox/savant_scale.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/python/primitives/buf_copy.py` & `savant_rs-0.1.9/python/primitives/buf_copy.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/python/primitives/frame_ops.py` & `savant_rs-0.1.9/python/primitives/frame_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 t = timer()
 
 frame_message = None
 for _ in range(1_000):
     bytes = save_message(message)
     frame_message = load_message(bytes)
 
-print(timer() - t)
+print("1K ser/des for frame took:", timer() - t)
 
 print(frame_message.is_video_frame)
 frame = frame_message.as_video_frame
 
 # print(frame)
```

### Comparing `savant_rs-0.1.7/python/primitives/polygon_match.py` & `savant_rs-0.1.9/python/primitives/polygon_match.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/python/utils/fps_meter/savant_fps_meter.py` & `savant_rs-0.1.9/python/utils/fps_meter/savant_fps_meter.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/python/utils/symbol_mapper/rust_symbol_mapper.py` & `savant_rs-0.1.9/python/utils/symbol_mapper/rust_symbol_mapper.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/python/utils/symbol_mapper/savant_symbol_mapper.py` & `savant_rs-0.1.9/python/utils/symbol_mapper/savant_symbol_mapper.py`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/src/lib.rs` & `savant_rs-0.1.9/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -7,30 +7,37 @@
     CopyWrapper, Internal, InternalMtx, InternalNoClone, ProxyWrapper, TakeWrapper, Wrapper,
 };
 
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 use pyo3::wrap_pymodule;
 
+use primitives::message::video::object::query::py::video_object_query;
+
 #[pymodule]
 fn savant_rs(py: Python, m: &PyModule) -> PyResult<()> {
     pyo3_log::init();
 
     m.add_class::<Internal>()?;
     m.add_class::<InternalNoClone>()?;
     m.add_class::<InternalMtx>()?;
     m.add_class::<Wrapper>()?;
     m.add_class::<CopyWrapper>()?;
     m.add_class::<TakeWrapper>()?;
     m.add_class::<ProxyWrapper>()?;
 
     m.add_wrapped(wrap_pymodule!(primitives::primitives))?;
     m.add_wrapped(wrap_pymodule!(utils::utils))?;
+    m.add_wrapped(wrap_pymodule!(video_object_query))?;
 
     let sys = PyModule::import(py, "sys")?;
     let sys_modules: &PyDict = sys.getattr("modules")?.downcast()?;
 
     sys_modules.set_item("savant_rs.primitives", m.getattr("primitives")?)?;
     sys_modules.set_item("savant_rs.utils", m.getattr("utils")?)?;
+    sys_modules.set_item(
+        "savant_rs.video_object_query",
+        m.getattr("video_object_query")?,
+    )?;
 
     Ok(())
 }
```

### Comparing `savant_rs-0.1.7/src/primitives/attribute.rs` & `savant_rs-0.1.9/src/primitives/attribute.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/src/primitives/bbox.rs` & `savant_rs-0.1.9/src/primitives/bbox.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use crate::primitives::to_json_value::ToSerdeJsonValue;
 use crate::primitives::{Point, PolygonalArea};
+use crate::utils::python::no_gil;
 use crate::utils::round_2_digits;
-use pyo3::{pyclass, pymethods, Py, PyAny, Python};
+use pyo3::{pyclass, pymethods, Py, PyAny};
 use rkyv::{Archive, Deserialize, Serialize};
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
 pub struct RBBox {
     #[pyo3(get, set)]
@@ -16,14 +17,26 @@
     pub width: f64,
     #[pyo3(get, set)]
     pub height: f64,
     #[pyo3(get, set)]
     pub angle: Option<f64>,
 }
 
+impl Default for RBBox {
+    fn default() -> Self {
+        Self {
+            xc: 0.0,
+            yc: 0.0,
+            width: 0.0,
+            height: 0.0,
+            angle: None,
+        }
+    }
+}
+
 impl ToSerdeJsonValue for RBBox {
     fn to_serde_json_value(&self) -> serde_json::Value {
         serde_json::json!({
             "xc": self.xc,
             "yc": self.yc,
             "width": self.width,
             "height": self.height,
@@ -54,61 +67,57 @@
             height,
             angle,
         }
     }
 
     #[pyo3(name = "scale")]
     pub fn scale_py(&mut self, scale_x: f64, scale_y: f64) {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.scale(scale_x, scale_y);
-            })
-        });
+        no_gil(|| {
+            self.scale(scale_x, scale_y);
+        })
     }
 
     #[getter]
     #[pyo3(name = "vertices")]
     pub fn vertices_py(&self) -> Vec<(f64, f64)> {
-        Python::with_gil(|py| py.allow_threads(|| self.vertices()))
+        no_gil(|| self.vertices())
     }
 
     #[getter]
     #[pyo3(name = "vertices_rounded")]
     pub fn vertices_rounded_py(&self) -> Vec<(f64, f64)> {
-        Python::with_gil(|py| py.allow_threads(|| self.vertices_rounded()))
+        no_gil(|| self.vertices_rounded())
     }
 
     #[getter]
     #[pyo3(name = "vertices_int")]
     pub fn vertices_int_py(&self) -> Vec<(i64, i64)> {
-        Python::with_gil(|py| py.allow_threads(|| self.vertices_int()))
+        no_gil(|| self.vertices_int())
     }
 
     #[pyo3(name = "as_polygonal_area")]
     pub fn as_polygonal_area_py(&self) -> PolygonalArea {
-        Python::with_gil(|py| py.allow_threads(|| self.as_polygonal_area()))
+        no_gil(|| self.as_polygonal_area())
     }
 
     #[getter]
     #[pyo3(name = "wrapping_box")]
     pub fn wrapping_box_py(&self) -> BBox {
-        Python::with_gil(|py| py.allow_threads(|| self.wrapping_bbox()))
+        no_gil(|| self.wrapping_bbox())
     }
 
     #[pyo3(name = "as_graphical_wrapping_box")]
     pub fn as_graphical_wrapping_box_py(
         &self,
         padding: f64,
         border_width: f64,
         max_x: f64,
         max_y: f64,
     ) -> BBox {
-        Python::with_gil(|py| {
-            py.allow_threads(|| self.graphical_wrapping_bbox(padding, border_width, max_x, max_y))
-        })
+        no_gil(|| self.graphical_wrapping_bbox(padding, border_width, max_x, max_y))
     }
 }
 
 impl RBBox {
     pub fn scale(&mut self, scale_x: f64, scale_y: f64) {
         match self.angle {
             None => {
@@ -355,44 +364,42 @@
     #[getter]
     pub fn get_bottom(&self) -> f64 {
         self.rbbox.yc + self.rbbox.height / 2.0
     }
 
     #[getter]
     pub fn vertices(&self) -> Vec<(f64, f64)> {
-        Python::with_gil(|py| py.allow_threads(|| self.rbbox.vertices()))
+        no_gil(|| self.rbbox.vertices())
     }
 
     #[getter]
     pub fn vertices_rounded(&self) -> Vec<(f64, f64)> {
-        Python::with_gil(|py| py.allow_threads(|| self.rbbox.vertices_rounded()))
+        no_gil(|| self.rbbox.vertices_rounded())
     }
 
     #[getter]
     pub fn vertices_int(&self) -> Vec<(i64, i64)> {
-        Python::with_gil(|py| py.allow_threads(|| self.rbbox.vertices_int()))
+        no_gil(|| self.rbbox.vertices_int())
     }
 
     #[getter]
     pub fn wrapping_box(&self) -> BBox {
-        Python::with_gil(|py| py.allow_threads(|| self.rbbox.wrapping_bbox()))
+        no_gil(|| self.rbbox.wrapping_bbox())
     }
 
     pub fn as_graphical_wrapping_box(
         &self,
         padding: f64,
         border_width: f64,
         max_x: f64,
         max_y: f64,
     ) -> BBox {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.rbbox
-                    .graphical_wrapping_bbox(padding, border_width, max_x, max_y)
-            })
+        no_gil(|| {
+            self.rbbox
+                .graphical_wrapping_bbox(padding, border_width, max_x, max_y)
         })
     }
 
     pub fn as_ltrb(&self) -> (f64, f64, f64, f64) {
         let top = self.get_top();
         let left = self.get_left();
         let bottom = self.get_bottom();
@@ -441,23 +448,21 @@
     }
 
     pub fn as_rbbox(&self) -> RBBox {
         self.rbbox.clone()
     }
 
     pub fn scale(&mut self, scale_x: f64, scale_y: f64) {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.rbbox.scale(scale_x, scale_y);
-            })
-        });
+        no_gil(|| {
+            self.rbbox.scale(scale_x, scale_y);
+        })
     }
 
     pub fn as_polygonal_area(&self) -> PolygonalArea {
-        Python::with_gil(|py| py.allow_threads(|| self.rbbox.as_polygonal_area()))
+        no_gil(|| self.rbbox.as_polygonal_area())
     }
 }
 
 #[cfg(test)]
 mod tests {
     use crate::primitives::RBBox;
     use crate::utils::round_2_digits;
```

### Comparing `savant_rs-0.1.7/src/primitives/message/eos.rs` & `savant_rs-0.1.9/src/primitives/message/eos.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/src/primitives/message/loader.rs` & `savant_rs-0.1.9/src/primitives/message/loader.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 use crate::primitives::message::video::frame::InnerVideoFrame;
 use crate::primitives::message::{
     NativeMessageMarkerType, NativeMessageTypeConsts, NATIVE_MESSAGE_MARKER_LEN,
 };
 use crate::primitives::{EndOfStream, Message, VideoFrame, VideoFrameBatch};
-use pyo3::{pyfunction, Python};
+use crate::utils::python::no_gil;
+use pyo3::pyfunction;
 
 #[pyfunction]
 #[pyo3(name = "load_message")]
 pub fn load_message_py(bytes: Vec<u8>) -> Message {
-    Python::with_gil(|py| py.allow_threads(|| load_message(bytes)))
+    no_gil(|| load_message(bytes))
 }
 
 pub fn load_message(mut bytes: Vec<u8>) -> Message {
     if bytes.len() < NATIVE_MESSAGE_MARKER_LEN {
         return Message::unknown(format!(
             "Message is too short: {} < {}",
             bytes.len(),
```

### Comparing `savant_rs-0.1.7/src/primitives/message/saver.rs` & `savant_rs-0.1.9/src/primitives/message/saver.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-use pyo3::{pyfunction, Python};
+use pyo3::pyfunction;
 
 use crate::primitives::message::{NativeMessage, NativeMessageMarkerType, NativeMessageTypeConsts};
 use crate::primitives::Message;
+use crate::utils::python::no_gil;
 
 #[pyfunction]
 #[pyo3(name = "save_message")]
 pub fn save_message_py(frame: Message) -> Vec<u8> {
-    Python::with_gil(|py| py.allow_threads(|| save_message(frame)))
+    no_gil(|| save_message(frame))
 }
 
 pub fn save_message(m: Message) -> Vec<u8> {
     match m.payload {
         NativeMessage::EndOfStream(s) => {
             let mut buf = Vec::with_capacity(32);
             buf.extend_from_slice(
```

### Comparing `savant_rs-0.1.7/src/primitives/message/video/batch.rs` & `savant_rs-0.1.9/src/primitives/message/video/batch.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::primitives::message::video::frame::InnerVideoFrame;
 use crate::primitives::VideoFrame;
-use pyo3::{pyclass, pymethods, Python};
+use crate::utils::python::no_gil;
+use pyo3::{pyclass, pymethods};
 use rkyv::{with::Skip, Archive, Deserialize, Serialize};
 use std::collections::HashMap;
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, Clone, Default)]
 #[archive(check_bytes)]
 pub struct VideoFrameBatch {
@@ -56,15 +57,15 @@
 
     pub fn del(&mut self, id: i64) -> Option<VideoFrame> {
         self.frames.remove(&id)
     }
 
     #[pyo3(name = "snapshot")]
     pub fn snapshot_py(&mut self) {
-        Python::with_gil(|py| py.allow_threads(|| self.snapshot()))
+        no_gil(|| self.snapshot())
     }
 
     #[pyo3(name = "restore")]
     pub fn restore_py(&mut self) {
-        Python::with_gil(|py| py.allow_threads(|| self.restore()))
+        no_gil(|| self.restore())
     }
 }
```

### Comparing `savant_rs-0.1.7/src/primitives/message/video/frame.rs` & `savant_rs-0.1.9/src/primitives/message/video/frame.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 use crate::primitives::attribute::{Attributive, InnerAttributes};
+use crate::primitives::message::video::object::query::py::QueryWrapper;
+use crate::primitives::message::video::object::query::{ExecutableQuery, Query};
 use crate::primitives::message::video::object::InnerObject;
 use crate::primitives::to_json_value::ToSerdeJsonValue;
 use crate::primitives::{Attribute, Message, Object};
-use pyo3::{pyclass, pymethods, Py, PyAny, PyResult, Python};
+use crate::utils::python::no_gil;
+use pyo3::{pyclass, pymethods, Py, PyAny, PyResult};
 use rkyv::{with::Skip, Archive, Deserialize, Serialize};
 use serde_json::Value;
 use std::collections::HashMap;
+use std::ops::Deref;
 use std::sync::{Arc, Mutex};
 
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
 pub struct ExternalFrame {
     #[pyo3(get, set)]
@@ -153,36 +157,52 @@
             _ => Err(pyo3::exceptions::PyTypeError::new_err(
                 "Video data is not stored externally",
             )),
         }
     }
 }
 
+#[pyclass]
+#[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
+#[archive(check_bytes)]
+pub enum VideoTranscodingMethod {
+    Copy,
+    Encoded,
+}
+
+impl ToSerdeJsonValue for VideoTranscodingMethod {
+    fn to_serde_json_value(&self) -> Value {
+        serde_json::json!(format!("{:?}", self))
+    }
+}
+
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
 pub enum FrameTransformation {
     InitialSize(u64, u64),
     Scale(u64, u64),
     Padding(u64, u64, u64, u64),
-    None,
+    ResultingSize(u64, u64),
 }
 
 impl ToSerdeJsonValue for FrameTransformation {
     fn to_serde_json_value(&self) -> Value {
         match self {
             FrameTransformation::InitialSize(width, height) => {
                 serde_json::json!({"initial_size": [width, height]})
             }
             FrameTransformation::Scale(width, height) => {
                 serde_json::json!({"scale": [width, height]})
             }
             FrameTransformation::Padding(left, top, right, bottom) => {
                 serde_json::json!({"padding": [left, top, right, bottom]})
             }
-            FrameTransformation::None => serde_json::json!(null),
+            FrameTransformation::ResultingSize(width, height) => {
+                serde_json::json!({"resulting_size": [width, height]})
+            }
         }
     }
 }
 
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct PyFrameTransformation {
@@ -216,14 +236,25 @@
                 u64::try_from(width).unwrap(),
                 u64::try_from(height).unwrap(),
             ),
         }
     }
 
     #[staticmethod]
+    pub fn resulting_size(width: i64, height: i64) -> Self {
+        assert!(width > 0 && height > 0);
+        Self {
+            inner: FrameTransformation::ResultingSize(
+                u64::try_from(width).unwrap(),
+                u64::try_from(height).unwrap(),
+            ),
+        }
+    }
+
+    #[staticmethod]
     pub fn scale(width: i64, height: i64) -> Self {
         assert!(width > 0 && height > 0);
         Self {
             inner: FrameTransformation::Scale(
                 u64::try_from(width).unwrap(),
                 u64::try_from(height).unwrap(),
             ),
@@ -239,21 +270,14 @@
                 u64::try_from(top).unwrap(),
                 u64::try_from(right).unwrap(),
                 u64::try_from(bottom).unwrap(),
             ),
         }
     }
 
-    #[staticmethod]
-    pub fn none() -> Self {
-        Self {
-            inner: FrameTransformation::None,
-        }
-    }
-
     #[getter]
     pub fn is_initial_size(&self) -> bool {
         matches!(self.inner, FrameTransformation::InitialSize(_, _))
     }
 
     #[getter]
     pub fn is_scale(&self) -> bool {
@@ -262,27 +286,35 @@
 
     #[getter]
     pub fn is_padding(&self) -> bool {
         matches!(self.inner, FrameTransformation::Padding(_, _, _, _))
     }
 
     #[getter]
-    pub fn is_none(&self) -> bool {
-        matches!(self.inner, FrameTransformation::None)
+    pub fn is_resulting_size(&self) -> bool {
+        matches!(self.inner, FrameTransformation::ResultingSize(_, _))
     }
 
     #[getter]
     pub fn as_initial_size(&self) -> Option<(u64, u64)> {
         match &self.inner {
             FrameTransformation::InitialSize(w, h) => Some((*w, *h)),
             _ => None,
         }
     }
 
     #[getter]
+    pub fn as_resulting_size(&self) -> Option<(u64, u64)> {
+        match &self.inner {
+            FrameTransformation::ResultingSize(w, h) => Some((*w, *h)),
+            _ => None,
+        }
+    }
+
+    #[getter]
     pub fn as_scale(&self) -> Option<(u64, u64)> {
         match &self.inner {
             FrameTransformation::Scale(w, h) => Some((*w, *h)),
             _ => None,
         }
     }
 
@@ -298,14 +330,15 @@
 #[derive(Archive, Deserialize, Serialize, Debug, Clone, derive_builder::Builder)]
 #[archive(check_bytes)]
 pub struct InnerVideoFrame {
     pub source_id: String,
     pub framerate: String,
     pub width: i64,
     pub height: i64,
+    pub transcoding_method: VideoTranscodingMethod,
     pub codec: Option<String>,
     pub keyframe: Option<bool>,
     pub pts: i64,
     pub dts: Option<i64>,
     pub duration: Option<i64>,
     pub content: VideoFrameContent,
     pub transformations: Vec<FrameTransformation>,
@@ -320,14 +353,15 @@
         serde_json::json!(
             {
                 "type": "VideoFrame",
                 "source_id": self.source_id,
                 "framerate": self.framerate,
                 "width": self.width,
                 "height": self.height,
+                "transcoding_method": self.transcoding_method.to_serde_json_value(),
                 "codec": self.codec,
                 "keyframe": self.keyframe,
                 "pts": self.pts,
                 "dts": self.dts,
                 "duration": self.duration,
                 "content": self.content.to_serde_json_value(),
                 "transformations": self.transformations.iter().map(|t| t.to_serde_json_value()).collect::<Vec<_>>(),
@@ -380,14 +414,91 @@
 
 impl VideoFrame {
     pub(crate) fn from_inner(object: InnerVideoFrame) -> Self {
         VideoFrame {
             inner: Arc::new(Mutex::new(Box::new(object))),
         }
     }
+
+    pub fn access_objects(&self, q: &Query) -> Vec<Object> {
+        let frame = self.inner.lock().unwrap();
+        frame
+            .resident_objects
+            .iter()
+            .filter_map(|o| {
+                if q.execute(o.lock().unwrap().deref()) {
+                    Some(Object::from_arc_inner_object(o.clone()))
+                } else {
+                    None
+                }
+            })
+            .collect()
+    }
+
+    pub fn get_json(&self) -> String {
+        serde_json::to_string(&self.to_serde_json_value()).unwrap()
+    }
+
+    pub fn get_json_pretty(&self) -> String {
+        serde_json::to_string_pretty(&self.to_serde_json_value()).unwrap()
+    }
+
+    pub fn access_objects_by_id(&self, ids: &[i64]) -> Vec<Object> {
+        let frame = self.inner.lock().unwrap();
+        frame
+            .resident_objects
+            .iter()
+            .filter(|o| ids.contains(&o.lock().unwrap().id))
+            .map(|o| Object::from_arc_inner_object(o.clone()))
+            .collect()
+    }
+
+    pub fn delete_objects_by_ids(&mut self, ids: &[i64]) {
+        let mut frame = self.inner.lock().unwrap();
+        frame
+            .resident_objects
+            .retain(|o| !ids.contains(&o.lock().unwrap().id));
+    }
+
+    pub fn delete_objects(&mut self, q: &Query) {
+        let mut frame = self.inner.lock().unwrap();
+        frame
+            .resident_objects
+            .retain(|o| !q.execute(o.lock().unwrap().deref()));
+    }
+
+    pub fn get_object(&self, id: i64) -> Option<Object> {
+        let frame = self.inner.lock().unwrap();
+        frame
+            .resident_objects
+            .iter()
+            .find(|o| o.lock().unwrap().id == id)
+            .map(|o| Object::from_arc_inner_object(o.clone()))
+    }
+
+    pub fn make_snapshot(&mut self) {
+        let mut frame = self.inner.lock().unwrap();
+        frame.prepare_before_save();
+    }
+
+    pub fn restore_from_snapshot(&mut self) {
+        let mut frame = self.inner.lock().unwrap();
+        frame.resident_objects.clear();
+        frame.prepare_after_load();
+    }
+
+    pub fn get_modified_objects(&self) -> Vec<Object> {
+        let frame = self.inner.lock().unwrap();
+        frame
+            .resident_objects
+            .iter()
+            .filter(|o| !o.lock().unwrap().modifications.is_empty())
+            .map(|o| Object::from_arc_inner_object(o.clone()))
+            .collect()
+    }
 }
 
 impl ToSerdeJsonValue for VideoFrame {
     fn to_serde_json_value(&self) -> Value {
         self.inner.lock().unwrap().to_serde_json_value()
     }
 }
@@ -404,36 +515,38 @@
     fn __str__(&self) -> String {
         self.__repr__()
     }
 
     #[allow(clippy::too_many_arguments)]
     #[new]
     #[pyo3(
-        signature = (source_id, framerate, width, height, content, codec=None, keyframe=None, pts=0, dts=None, duration=None)
+        signature = (source_id, framerate, width, height, content, transcoding_method=VideoTranscodingMethod::Copy, codec=None, keyframe=None, pts=0, dts=None, duration=None)
     )]
     pub fn new(
         source_id: String,
         framerate: String,
         width: i64,
         height: i64,
         content: PyVideoFrameContent,
+        transcoding_method: VideoTranscodingMethod,
         codec: Option<String>,
         keyframe: Option<bool>,
         pts: i64,
         dts: Option<i64>,
         duration: Option<i64>,
     ) -> Self {
         VideoFrame::from_inner(InnerVideoFrame {
             source_id,
             pts,
             framerate,
             width,
             height,
             dts,
             duration,
+            transcoding_method,
             codec,
             keyframe,
             transformations: vec![],
             content: content.inner,
             attributes: HashMap::default(),
             offline_objects: vec![],
             resident_objects: vec![],
@@ -446,16 +559,23 @@
 
     #[getter]
     pub fn get_source_id(&self) -> String {
         self.inner.lock().unwrap().source_id.clone()
     }
 
     #[getter]
-    pub fn get_json(&self) -> String {
-        serde_json::to_string(&self.to_serde_json_value()).unwrap()
+    #[pyo3(name = "json")]
+    pub fn json_py(&self) -> String {
+        no_gil(|| serde_json::to_string(&self.to_serde_json_value()).unwrap())
+    }
+
+    #[getter]
+    #[pyo3(name = "json_pretty")]
+    fn json_pretty_py(&self) -> String {
+        no_gil(|| serde_json::to_string_pretty(&self.to_serde_json_value()).unwrap())
     }
 
     #[setter]
     pub fn set_source_id(&mut self, source_id: String) {
         let mut frame = self.inner.lock().unwrap();
         frame.source_id = source_id;
     }
@@ -536,14 +656,26 @@
             "duration must be greater than or equal to 0"
         );
         let mut frame = self.inner.lock().unwrap();
         frame.duration = duration;
     }
 
     #[getter]
+    pub fn get_transcoding_method(&self) -> VideoTranscodingMethod {
+        let frame = self.inner.lock().unwrap();
+        frame.transcoding_method.clone()
+    }
+
+    #[setter]
+    pub fn set_transcoding_method(&mut self, transcoding_method: VideoTranscodingMethod) {
+        let mut frame = self.inner.lock().unwrap();
+        frame.transcoding_method = transcoding_method;
+    }
+
+    #[getter]
     pub fn get_codec(&self) -> Option<String> {
         let frame = self.inner.lock().unwrap();
         frame.codec.clone()
     }
 
     #[setter]
     pub fn set_codec(&mut self, codec: Option<String>) {
@@ -593,45 +725,41 @@
     pub fn set_content(&mut self, content: PyVideoFrameContent) {
         let mut frame = self.inner.lock().unwrap();
         frame.content = content.inner;
     }
 
     #[getter]
     pub fn attributes(&self) -> Vec<(String, String)> {
-        Python::with_gil(move |py| py.allow_threads(move || self.get_attributes()))
+        no_gil(|| self.get_attributes())
     }
 
     #[pyo3(name = "find_attributes")]
     pub fn find_attributes_py(
         &self,
         creator: Option<String>,
         name: Option<String>,
         hint: Option<String>,
     ) -> Vec<(String, String)> {
-        Python::with_gil(move |py| {
-            py.allow_threads(move || self.find_attributes(creator, name, hint))
-        })
+        no_gil(|| self.find_attributes(creator, name, hint))
     }
 
     #[pyo3(name = "get_attribute")]
     pub fn get_attribute_py(&self, creator: String, name: String) -> Option<Attribute> {
-        self.get_attribute(creator, name)
+        no_gil(|| self.get_attribute(creator, name))
     }
 
     #[pyo3(signature = (negated=false, creator=None, names=vec![]))]
     #[pyo3(name = "delete_attributes")]
     pub fn delete_attributes_py(
         &mut self,
         negated: bool,
         creator: Option<String>,
         names: Vec<String>,
     ) {
-        Python::with_gil(move |py| {
-            py.allow_threads(move || self.delete_attributes(negated, creator, names))
-        })
+        no_gil(|| self.delete_attributes(negated, creator, names))
     }
 
     #[pyo3(name = "delete_attribute")]
     pub fn delete_attribute_py(&mut self, creator: String, name: String) -> Option<Attribute> {
         self.delete_attribute(creator, name)
     }
 
@@ -641,215 +769,132 @@
     }
 
     #[pyo3(name = "clear_attributes")]
     pub fn clear_attributes_py(&mut self) {
         self.clear_attributes()
     }
 
-    pub fn get_object(&self, id: i64) -> Option<Object> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                let frame = self.inner.lock().unwrap();
-                frame
-                    .resident_objects
-                    .iter()
-                    .find(|o| o.lock().unwrap().id == id)
-                    .map(|o| Object::from_arc_inner_object(o.clone()))
-            })
-        })
+    #[pyo3(name = "get_object")]
+    pub fn get_object_py(&self, id: i64) -> Option<Object> {
+        no_gil(|| self.get_object(id))
     }
 
-    pub fn access_objects(
-        &self,
-        negated: bool,
-        creator: Option<String>,
-        label: Option<String>,
-    ) -> Vec<Object> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                let frame = self.inner.lock().unwrap();
-                frame
-                    .resident_objects
-                    .iter()
-                    .filter(|o| {
-                        let o = o.lock().unwrap();
-                        let creator_match = match &creator {
-                            Some(creator) => o.creator == *creator,
-                            None => true,
-                        };
-                        let label_match = match &label {
-                            Some(label) => o.label == *label,
-                            None => true,
-                        };
-                        (creator_match && label_match) ^ negated
-                    })
-                    .map(|o| Object::from_arc_inner_object(o.clone()))
-                    .collect()
-            })
-        })
+    #[pyo3(name = "access_objects")]
+    pub fn access_objects_py(&self, q: QueryWrapper) -> Vec<Object> {
+        no_gil(|| self.access_objects(q.inner.deref()))
     }
 
-    pub fn access_objects_by_id(&self, ids: Vec<i64>) -> Vec<Object> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                let frame = self.inner.lock().unwrap();
-                frame
-                    .resident_objects
-                    .iter()
-                    .filter(|o| ids.contains(&o.lock().unwrap().id))
-                    .map(|o| Object::from_arc_inner_object(o.clone()))
-                    .collect()
-            })
-        })
+    #[pyo3(name = "access_objects_by_id")]
+    pub fn access_objects_by_id_py(&self, ids: Vec<i64>) -> Vec<Object> {
+        no_gil(|| self.access_objects_by_id(&ids))
     }
 
     pub fn add_object(&mut self, object: Object) {
         let mut frame = self.inner.lock().unwrap();
         frame.resident_objects.push(object.inner);
     }
 
-    pub fn delete_objects_by_ids(&mut self, ids: Vec<i64>) {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                let mut frame = self.inner.lock().unwrap();
-                frame
-                    .resident_objects
-                    .retain(|o| !ids.contains(&o.lock().unwrap().id));
-            })
-        })
+    #[pyo3(name = "delete_objects_by_ids")]
+    pub fn delete_objects_by_ids_py(&mut self, ids: Vec<i64>) {
+        no_gil(|| self.delete_objects_by_ids(&ids))
     }
 
-    pub fn delete_objects(
-        &mut self,
-        negated: bool,
-        creator: Option<String>,
-        label: Option<String>,
-    ) {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                let mut frame = self.inner.lock().unwrap();
-                frame.resident_objects.retain(|o| {
-                    let o = o.lock().unwrap();
-                    let creator_match = match &creator {
-                        Some(creator) => o.creator == *creator,
-                        None => true,
-                    };
-                    let label_match = match &label {
-                        Some(label) => o.label == *label,
-                        None => true,
-                    };
-                    !((creator_match && label_match) ^ negated)
-                });
-            })
-        })
+    #[pyo3(name = "delete_objects")]
+    pub fn delete_objects_py(&mut self, query: QueryWrapper) {
+        no_gil(|| self.delete_objects(&query.inner))
     }
 
     pub fn clear_objects(&mut self) {
         let mut frame = self.inner.lock().unwrap();
         frame.resident_objects.clear();
     }
 
-    pub fn snapshot(&mut self) {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                let mut frame = self.inner.lock().unwrap();
-                frame.prepare_before_save();
-            })
-        })
+    #[pyo3(name = "make_snapshot")]
+    pub fn make_snapshot_py(&mut self) {
+        no_gil(|| self.make_snapshot())
     }
 
-    pub fn restore(&mut self) {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                let mut frame = self.inner.lock().unwrap();
-                frame.resident_objects.clear();
-                frame.prepare_after_load();
-            })
-        })
+    #[pyo3(name = "restore_from_snapshot")]
+    pub fn restore_from_snapshot_py(&mut self) {
+        no_gil(|| self.restore_from_snapshot())
     }
 
-    pub fn get_modified_objects(&self) -> Vec<Object> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                let frame = self.inner.lock().unwrap();
-                frame
-                    .resident_objects
-                    .iter()
-                    .filter(|o| !o.lock().unwrap().modifications.is_empty())
-                    .map(|o| Object::from_arc_inner_object(o.clone()))
-                    .collect()
-            })
-        })
+    #[pyo3(name = "get_modified_objects")]
+    pub fn get_modified_objects_py(&self) -> Vec<Object> {
+        no_gil(|| self.get_modified_objects())
     }
 }
 
 #[cfg(test)]
 mod tests {
     use crate::primitives::attribute::Attributive;
+    use crate::primitives::message::video::object::query::Query;
     use crate::primitives::Modification;
     use crate::test::utils::gen_frame;
 
     #[test]
     fn test_access_objects_by_id() {
         pyo3::prepare_freethreaded_python();
         let t = gen_frame();
-        let objects = t.access_objects_by_id(vec![0, 1]);
+        let objects = t.access_objects_by_id_py(vec![0, 1]);
         assert_eq!(objects.len(), 2);
         assert_eq!(objects[0].get_id(), 0);
         assert_eq!(objects[1].get_id(), 1);
     }
 
     #[test]
     fn test_access_objects() {
         pyo3::prepare_freethreaded_python();
 
-        let t = gen_frame();
-        let objects = t.access_objects(false, None, None);
-        assert_eq!(objects.len(), 3);
-
-        let t = gen_frame();
-        let objects = t.access_objects(true, None, None);
-        assert!(objects.is_empty());
-
-        let t = gen_frame();
-        let objects = t.access_objects(false, Some("abc".to_string()), None);
-        assert!(objects.is_empty());
-
-        let t = gen_frame();
-        let objects = t.access_objects(true, Some("abc".to_string()), None);
-        assert_eq!(objects.len(), 3);
-
-        let t = gen_frame();
-        let objects = t.access_objects(false, Some("test2".to_string()), None);
-        assert_eq!(objects.len(), 2);
-        assert_eq!(objects[0].get_id(), 1);
-        assert_eq!(objects[1].get_id(), 2);
-
-        let t = gen_frame();
-        let objects = t.access_objects(true, Some("test2".to_string()), None);
-        assert_eq!(objects.len(), 1);
-        assert_eq!(objects[0].get_id(), 0);
-
-        let t = gen_frame();
-        let objects = t.access_objects(false, Some("test2".to_string()), Some("test2".to_string()));
-        assert_eq!(objects.len(), 1);
-        assert_eq!(objects[0].get_id(), 2);
-
-        let t = gen_frame();
-        let objects = t.access_objects(true, Some("test2".to_string()), Some("test2".to_string()));
-        assert_eq!(objects.len(), 2);
-        assert_eq!(objects[0].get_id(), 0);
-        assert_eq!(objects[1].get_id(), 1);
+        // let t = gen_frame();
+        // let objects = t.access_objects_py(false, None, None);
+        // assert_eq!(objects.len(), 3);
+        //
+        // let t = gen_frame();
+        // let objects = t.access_objects_py(true, None, None);
+        // assert!(objects.is_empty());
+        //
+        // let t = gen_frame();
+        // let objects = t.access_objects_py(false, Some("abc".to_string()), None);
+        // assert!(objects.is_empty());
+        //
+        // let t = gen_frame();
+        // let objects = t.access_objects_py(true, Some("abc".to_string()), None);
+        // assert_eq!(objects.len(), 3);
+        //
+        // let t = gen_frame();
+        // let objects = t.access_objects_py(false, Some("test2".to_string()), None);
+        // assert_eq!(objects.len(), 2);
+        // assert_eq!(objects[0].get_id(), 1);
+        // assert_eq!(objects[1].get_id(), 2);
+
+        // let t = gen_frame();
+        // let objects = t.access_objects_py(true, Some("test2".to_string()), None);
+        // assert_eq!(objects.len(), 1);
+        // assert_eq!(objects[0].get_id(), 0);
+        //
+        // let t = gen_frame();
+        // let objects =
+        //     t.access_objects_py(false, Some("test2".to_string()), Some("test2".to_string()));
+        // assert_eq!(objects.len(), 1);
+        // assert_eq!(objects[0].get_id(), 2);
+        //
+        // let t = gen_frame();
+        // let objects =
+        //     t.access_objects_py(true, Some("test2".to_string()), Some("test2".to_string()));
+        // assert_eq!(objects.len(), 2);
+        // assert_eq!(objects[0].get_id(), 0);
+        // assert_eq!(objects[1].get_id(), 1);
     }
 
     #[test]
     fn test_objects_by_id() {
         pyo3::prepare_freethreaded_python();
         let t = gen_frame();
-        let objects = t.access_objects_by_id(vec![0, 1]);
+        let objects = t.access_objects_by_id_py(vec![0, 1]);
         assert_eq!(objects.len(), 2);
         assert_eq!(objects[0].get_id(), 0);
         assert_eq!(objects[1].get_id(), 1);
     }
 
     #[test]
     fn test_get_attribute() {
@@ -893,75 +938,44 @@
         assert_eq!(attributes[1], ("system".to_string(), "test2".to_string()));
     }
 
     #[test]
     fn test_delete_objects_by_ids() {
         pyo3::prepare_freethreaded_python();
         let mut t = gen_frame();
-        t.delete_objects_by_ids(vec![0, 1]);
-        let objects = t.access_objects(false, None, None);
+        t.delete_objects_by_ids(&[0, 1]);
+        let objects = t.access_objects(&Query::Idle);
         assert_eq!(objects.len(), 1);
         assert_eq!(objects[0].get_id(), 2);
     }
 
     #[test]
-    fn test_delete_objects() {
+    fn test_delete_all_objects() {
         pyo3::prepare_freethreaded_python();
         let mut t = gen_frame();
-        t.delete_objects(false, None, None);
-        let objects = t.access_objects(false, None, None);
+        t.delete_objects(&Query::Idle);
+        let objects = t.access_objects(&Query::Idle);
         assert!(objects.is_empty());
-
-        let mut t = gen_frame();
-        t.delete_objects(true, None, None);
-        let objects = t.access_objects(false, None, None);
-        assert_eq!(objects.len(), 3);
-
-        let mut t = gen_frame();
-        t.delete_objects(false, Some("test2".to_string()), None);
-        let objects = t.access_objects(false, None, None);
-        assert_eq!(objects.len(), 1);
-        assert_eq!(objects[0].get_id(), 0);
-
-        let mut t = gen_frame();
-        t.delete_objects(true, Some("test2".to_string()), None);
-        let objects = t.access_objects(false, None, None);
-        assert_eq!(objects.len(), 2);
-        assert_eq!(objects[0].get_id(), 1);
-        assert_eq!(objects[1].get_id(), 2);
-
-        let mut t = gen_frame();
-        t.delete_objects(false, Some("test2".to_string()), Some("test2".to_string()));
-        let objects = t.access_objects(false, None, None);
-        assert_eq!(objects.len(), 2);
-        assert_eq!(objects[0].get_id(), 0);
-        assert_eq!(objects[1].get_id(), 1);
-
-        let mut t = gen_frame();
-        t.delete_objects(true, Some("test2".to_string()), Some("test2".to_string()));
-        let objects = t.access_objects(false, None, None);
-        assert_eq!(objects.len(), 1);
-        assert_eq!(objects[0].get_id(), 2);
     }
 
     #[test]
     fn test_snapshotting() {
         let mut t = gen_frame();
-        t.snapshot();
-        let mut o = t.access_objects_by_id(vec![0]).pop().unwrap();
+        t.make_snapshot_py();
+        let mut o = t.access_objects_by_id_py(vec![0]).pop().unwrap();
         o.set_id(12);
-        assert!(matches!(t.access_objects_by_id(vec![0]).pop(), None));
-        t.restore();
-        t.access_objects_by_id(vec![0]).pop().unwrap();
+        assert!(matches!(t.access_objects_by_id_py(vec![0]).pop(), None));
+        t.restore_from_snapshot_py();
+        t.access_objects_by_id_py(vec![0]).pop().unwrap();
     }
 
     #[test]
     fn test_modified_objects() {
         let t = gen_frame();
-        let mut o = t.access_objects_by_id(vec![0]).pop().unwrap();
+        let mut o = t.access_objects_by_id_py(vec![0]).pop().unwrap();
         o.set_id(12);
         let mut modified = t.get_modified_objects();
         assert_eq!(modified.len(), 1);
         let modified = modified.pop().unwrap();
         assert_eq!(modified.get_id(), 12);
 
         let mods = modified.take_modifications();
```

### Comparing `savant_rs-0.1.7/src/primitives/message/video/object.rs` & `savant_rs-0.1.9/src/primitives/message/video/object.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 use crate::primitives::attribute::{Attributive, InnerAttributes};
 use crate::primitives::to_json_value::ToSerdeJsonValue;
 use crate::primitives::{Attribute, RBBox};
-use pyo3::{pyclass, pymethods, Py, PyAny, Python};
+use crate::utils::python::no_gil;
+use crate::utils::symbol_mapper::get_object_id;
+use pyo3::{pyclass, pymethods, Py, PyAny};
 use rkyv::{with::Skip, Archive, Deserialize, Serialize};
 use std::collections::HashMap;
 use std::sync::{Arc, Mutex};
 
+pub mod query;
+
 #[pyclass]
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone)]
 #[archive(check_bytes)]
 pub struct ParentObject {
     #[pyo3(get, set)]
     pub id: i64,
     #[pyo3(get, set)]
@@ -69,20 +73,49 @@
 #[derive(Archive, Deserialize, Serialize, Debug, PartialEq, Clone, derive_builder::Builder)]
 #[archive(check_bytes)]
 pub struct InnerObject {
     pub id: i64,
     pub creator: String,
     pub label: String,
     pub bbox: RBBox,
+    #[builder(default)]
     pub attributes: HashMap<(String, String), Attribute>,
+    #[builder(default)]
     pub confidence: Option<f64>,
+    #[builder(default)]
     pub parent: Option<ParentObject>,
+    #[builder(default)]
     pub track_id: Option<i64>,
     #[with(Skip)]
+    #[builder(default)]
     pub modifications: Vec<Modification>,
+    #[with(Skip)]
+    #[builder(default)]
+    pub creator_id: Option<i64>,
+    #[with(Skip)]
+    #[builder(default)]
+    pub label_id: Option<i64>,
+}
+
+impl Default for InnerObject {
+    fn default() -> Self {
+        Self {
+            id: 0,
+            creator: "".to_string(),
+            label: "".to_string(),
+            bbox: RBBox::default(),
+            attributes: HashMap::new(),
+            confidence: None,
+            parent: None,
+            track_id: None,
+            modifications: Vec::new(),
+            creator_id: None,
+            label_id: None,
+        }
+    }
 }
 
 impl ToSerdeJsonValue for InnerObject {
     fn to_serde_json_value(&self) -> serde_json::Value {
         serde_json::json!({
             "id": self.id,
             "creator": self.creator,
@@ -159,24 +192,29 @@
         label: String,
         bbox: RBBox,
         attributes: HashMap<(String, String), Attribute>,
         confidence: Option<f64>,
         parent: Option<ParentObject>,
         track_id: Option<i64>,
     ) -> Self {
+        let (creator_id, label_id) =
+            get_object_id(&creator, &label).map_or((None, None), |(c, o)| (Some(c), Some(o)));
+
         let object = InnerObject {
             id,
             creator,
             label,
             bbox,
             attributes,
             confidence,
             parent,
             track_id,
             modifications: Vec::default(),
+            creator_id,
+            label_id,
         };
         Self {
             inner: Arc::new(Mutex::new(object)),
         }
     }
 
     #[getter]
@@ -264,15 +302,15 @@
         let mut object = self.inner.lock().unwrap();
         object.parent = parent;
         object.modifications.push(Modification::Parent);
     }
 
     #[getter]
     pub fn attributes(&self) -> Vec<(String, String)> {
-        Python::with_gil(move |py| py.allow_threads(move || self.get_attributes()))
+        no_gil(|| self.get_attributes())
     }
 
     #[pyo3(name = "get_attribute")]
     pub fn get_attribute_py(&self, creator: String, name: String) -> Option<Attribute> {
         self.get_attribute(creator, name)
     }
 
@@ -310,33 +348,31 @@
     #[pyo3(name = "delete_attributes")]
     pub fn delete_attributes_py(
         &mut self,
         negated: bool,
         creator: Option<String>,
         names: Vec<String>,
     ) {
-        Python::with_gil(move |py| {
-            py.allow_threads(move || {
-                {
-                    let mut object = self.inner.lock().unwrap();
-                    object.modifications.push(Modification::Attributes);
-                }
-                self.delete_attributes(negated, creator, names)
-            })
+        no_gil(move || {
+            {
+                let mut object = self.inner.lock().unwrap();
+                object.modifications.push(Modification::Attributes);
+            }
+            self.delete_attributes(negated, creator, names)
         })
     }
 
     #[pyo3(name = "find_attributes")]
     pub fn find_attributes_py(
         &self,
         creator: Option<String>,
         name: Option<String>,
         hint: Option<String>,
     ) -> Vec<(String, String)> {
-        Python::with_gil(move |py| py.allow_threads(|| self.find_attributes(creator, name, hint)))
+        no_gil(|| self.find_attributes(creator, name, hint))
     }
 
     pub fn take_modifications(&self) -> Vec<Modification> {
         let mut object = self.inner.lock().unwrap();
         std::mem::take(&mut object.modifications)
     }
 }
```

### Comparing `savant_rs-0.1.7/src/primitives/message.rs` & `savant_rs-0.1.9/src/primitives/message.rs`

 * *Files 0% similar despite different names*

```diff
@@ -229,10 +229,10 @@
                 ("system".into(), "test".into()),
                 ("system".into(), "test2".into()),
                 ("system2".into(), "test2".into()),
                 ("test".into(), "test".into()),
             ]
         );
 
-        let _ = f.access_objects_by_id(vec![0]).pop().unwrap();
+        let _ = f.access_objects_by_id_py(vec![0]).pop().unwrap();
     }
 }
```

### Comparing `savant_rs-0.1.7/src/primitives/point.rs` & `savant_rs-0.1.9/src/primitives/point.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/src/primitives/polygonal_area.rs` & `savant_rs-0.1.9/src/primitives/polygonal_area.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use crate::primitives::point::Point;
 use crate::primitives::to_json_value::ToSerdeJsonValue;
 use crate::primitives::{Intersection, IntersectionKind, Segment};
+use crate::utils::python::no_gil;
 use geo::{Contains, Intersects, Line, LineString};
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use rayon::prelude::*;
 use rkyv::{with::Skip, Archive, Deserialize, Serialize};
 use serde_json::Value;
 use std::sync::Arc;
@@ -71,78 +72,74 @@
                 }
             }
         }
     }
 
     #[pyo3(name = "crossed_by_segment")]
     pub fn crossed_by_segment_py(&mut self, seg: &Segment) -> Intersection {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.build_polygon();
-                self.crossed_by_segment(seg)
-            })
+        no_gil(|| {
+            self.build_polygon();
+            self.crossed_by_segment(seg)
         })
     }
 
     pub fn crossed_by_segments(&mut self, segs: Vec<Segment>) -> Vec<Intersection> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.build_polygon();
-                segs.iter().map(|s| self.crossed_by_segment(s)).collect()
-            })
+        no_gil(|| {
+            self.build_polygon();
+            segs.iter().map(|s| self.crossed_by_segment(s)).collect()
         })
     }
 
     #[pyo3(name = "contains")]
     pub fn contains_py(&mut self, p: &Point) -> bool {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.build_polygon();
-                self.contains(p)
-            })
+        no_gil(|| {
+            self.build_polygon();
+            self.contains(p)
         })
     }
 
     pub fn contains_many_points(&mut self, points: Vec<Point>) -> Vec<bool> {
-        Python::with_gil(|py| {
-            py.allow_threads(|| {
-                self.build_polygon();
-                points.iter().map(|p| self.contains(p)).collect()
-            })
+        no_gil(|| {
+            self.build_polygon();
+            points.iter().map(|p| self.contains(p)).collect()
         })
     }
 
     #[staticmethod]
     pub fn points_positions(polys: Vec<Self>, points: Vec<Point>) -> Vec<Vec<bool>> {
-        let pts = &points;
-        polys
-            .into_par_iter()
-            .map(|mut p| {
-                p.build_polygon();
-                pts.iter().map(|pt| p.contains(pt)).collect()
-            })
-            .collect()
+        no_gil(|| {
+            let pts = &points;
+            polys
+                .into_par_iter()
+                .map(|mut p| {
+                    p.build_polygon();
+                    pts.iter().map(|pt| p.contains(pt)).collect()
+                })
+                .collect()
+        })
     }
 
     #[staticmethod]
     pub fn segments_intersections(
         polys: Vec<Self>,
         segments: Vec<Segment>,
     ) -> Vec<Vec<Intersection>> {
-        let segments = &segments;
-        polys
-            .into_par_iter()
-            .map(|mut p| {
-                p.build_polygon();
-                segments
-                    .iter()
-                    .map(|seg| p.crossed_by_segment_py(seg))
-                    .collect()
-            })
-            .collect()
+        no_gil(|| {
+            let segments = &segments;
+            polys
+                .into_par_iter()
+                .map(|mut p| {
+                    p.build_polygon();
+                    segments
+                        .iter()
+                        .map(|seg| p.crossed_by_segment_py(seg))
+                        .collect()
+                })
+                .collect()
+        })
     }
 }
 
 impl PolygonalArea {
     pub fn crossed_by_segment(&mut self, seg: &Segment) -> Intersection {
         let seg = Line::from([(seg.begin.x, seg.begin.y), (seg.end.x, seg.end.y)]);
         let poly = self.polygon.as_ref().unwrap();
```

### Comparing `savant_rs-0.1.7/src/primitives/segment.rs` & `savant_rs-0.1.9/src/primitives/segment.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/src/primitives.rs` & `savant_rs-0.1.9/src/primitives.rs`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 pub use bbox::RBBox;
 pub use message::eos::EndOfStream;
 pub use message::loader::load_message;
 pub use message::saver::save_message;
 pub use message::video::batch::VideoFrameBatch;
 pub use message::video::frame::PyVideoFrameContent;
 pub use message::video::frame::VideoFrame;
+pub use message::video::frame::VideoTranscodingMethod;
 pub use message::video::object::Modification;
 pub use message::video::object::Object;
 pub use message::video::object::ParentObject;
 pub use message::Message;
 pub use point::Point;
 pub use polygonal_area::PolygonalArea;
 use pyo3::prelude::PyModule;
@@ -43,12 +44,13 @@
     m.add_class::<Value>()?;
     m.add_class::<Object>()?;
     m.add_class::<ParentObject>()?;
     m.add_class::<VideoFrame>()?;
     m.add_class::<VideoFrameBatch>()?;
     m.add_class::<EndOfStream>()?;
     m.add_class::<Message>()?;
+    m.add_class::<VideoTranscodingMethod>()?;
     m.add_class::<PyVideoFrameContent>()?;
     m.add_class::<PyFrameTransformation>()?;
     m.add_class::<Modification>()?;
     Ok(())
 }
```

### Comparing `savant_rs-0.1.7/src/test.rs` & `savant_rs-0.1.9/src/test.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 pub mod utils {
-    use crate::primitives::message::video::frame::InnerVideoFrameBuilder;
+    use crate::primitives::message::video::frame::{
+        InnerVideoFrameBuilder, VideoTranscodingMethod,
+    };
     use crate::primitives::message::video::object::InnerObjectBuilder;
     use crate::primitives::{
         AttributeBuilder, Intersection, IntersectionKind, Point, PyVideoFrameContent, Value,
     };
     use crate::primitives::{RBBox, VideoFrame};
     use pyo3::pyfunction;
     use std::collections::HashMap;
@@ -18,14 +20,15 @@
                 .framerate("test".to_string())
                 .width(0)
                 .height(0)
                 .content(PyVideoFrameContent::none().inner)
                 .dts(None)
                 .transformations(Vec::default())
                 .duration(None)
+                .transcoding_method(VideoTranscodingMethod::Copy)
                 .codec(None)
                 .keyframe(None)
                 .attributes(HashMap::default())
                 .offline_objects(Default::default())
                 .resident_objects(vec![
                     Arc::new(Mutex::new(
                         InnerObjectBuilder::default()
```

### Comparing `savant_rs-0.1.7/src/tests_pyo3_access.rs` & `savant_rs-0.1.9/src/tests_pyo3_access.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/src/utils/bbox.rs` & `savant_rs-0.1.9/src/utils/bbox.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use crate::primitives::{BBox, RBBox};
-use crate::utils::{ConvF64, ElementType, RConvF64};
+use crate::utils::np::{ConvF64, ElementType, RConvF64};
 use numpy::ndarray::ArrayD;
 use numpy::{IxDyn, PyArray, PyReadonlyArrayDyn};
 use pyo3::prelude::*;
 
 #[pyclass]
 #[derive(Debug, Clone)]
 pub enum BBoxFormat {
```

### Comparing `savant_rs-0.1.7/src/utils/conversions.rs` & `savant_rs-0.1.9/src/utils/conversions.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::utils::{ConvF64, RConvF64};
+use crate::utils::np::{ConvF64, RConvF64};
 
 impl ConvF64 for f32 {
     fn conv_f64(self) -> f64 {
         self as f64
     }
 }
```

### Comparing `savant_rs-0.1.7/src/utils/fps_meter.rs` & `savant_rs-0.1.9/src/utils/fps_meter.rs`

 * *Files identical despite different names*

### Comparing `savant_rs-0.1.7/src/utils/numpy_utils.rs` & `savant_rs-0.1.9/src/utils/np/np_nalgebra.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-use nalgebra::{DMatrix, Scalar};
+use crate::utils::np::ElementType;
+use nalgebra::DMatrix;
 use numpy::ndarray::ArrayD;
 use numpy::{IxDyn, PyArray, PyReadonlyArrayDyn};
 use pyo3::exceptions::PyValueError;
 use pyo3::prelude::*;
 use std::fmt::Debug;
 use std::ops::Deref;
-use std::sync::{Arc, Mutex};
+use std::sync::Arc;
 
 macro_rules! pretty_print {
     ($arr:expr) => {{
         let indent = 4;
         let prefix = String::from_utf8(vec![b' '; indent]).unwrap();
         let mut result_els = vec!["".to_string()];
         for i in 0..$arr.nrows() {
@@ -21,174 +22,152 @@
             let row_str = format!("{}{}", prefix, row_str);
             result_els.push(row_str);
         }
         result_els.into_iter().collect::<Vec<_>>().join("\n")
     }};
 }
 
-pub trait ConvF64 {
-    fn conv_f64(self) -> f64;
-}
-
-pub trait RConvF64 {
-    fn conv_from_f64(f: f64) -> Self;
-}
-
-pub trait ElementType: numpy::Element + Scalar + Copy + Clone + Debug {}
-
-impl ElementType for f32 {}
-impl ElementType for f64 {}
-impl ElementType for i8 {}
-impl ElementType for i16 {}
-impl ElementType for i32 {}
-impl ElementType for i64 {}
-impl ElementType for u8 {}
-impl ElementType for u16 {}
-impl ElementType for u32 {}
-impl ElementType for u64 {}
-
 #[derive(Debug, Clone)]
-pub enum MatrixVariant {
+pub enum NalgebraDMatrixVariant {
     Float64(DMatrix<f64>),
     Float32(DMatrix<f32>),
     Int64(DMatrix<i64>),
     Int32(DMatrix<i32>),
     Int16(DMatrix<i16>),
     Int8(DMatrix<i8>),
     UnsignedInt64(DMatrix<u64>),
     UnsignedInt32(DMatrix<u32>),
     UnsignedInt16(DMatrix<u16>),
     UnsignedInt8(DMatrix<u8>),
 }
 
 #[pyclass]
 #[derive(Debug, Clone)]
-pub struct Matrix {
-    inner: Arc<Mutex<MatrixVariant>>,
+pub struct NalgebraDMatrix {
+    inner: Arc<NalgebraDMatrixVariant>,
 }
 
-impl Matrix {
+impl NalgebraDMatrix {
     pub fn from_fp64(m: DMatrix<f64>) -> Self {
         Self {
-            inner: Arc::new(Mutex::new(MatrixVariant::Float64(m))),
+            inner: Arc::new(NalgebraDMatrixVariant::Float64(m)),
         }
     }
     pub fn from_fp32(m: DMatrix<f32>) -> Self {
         Self {
-            inner: Arc::new(Mutex::new(MatrixVariant::Float32(m))),
+            inner: Arc::new(NalgebraDMatrixVariant::Float32(m)),
         }
     }
 
     pub fn from_i64(m: DMatrix<i64>) -> Self {
         Self {
-            inner: Arc::new(Mutex::new(MatrixVariant::Int64(m))),
+            inner: Arc::new(NalgebraDMatrixVariant::Int64(m)),
         }
     }
 
     pub fn from_i32(m: DMatrix<i32>) -> Self {
         Self {
-            inner: Arc::new(Mutex::new(MatrixVariant::Int32(m))),
+            inner: Arc::new(NalgebraDMatrixVariant::Int32(m)),
         }
     }
 
     pub fn from_i16(m: DMatrix<i16>) -> Self {
         Self {
-            inner: Arc::new(Mutex::new(MatrixVariant::Int16(m))),
+            inner: Arc::new(NalgebraDMatrixVariant::Int16(m)),
         }
     }
 
     pub fn from_i8(m: DMatrix<i8>) -> Self {
         Self {
-            inner: Arc::new(Mutex::new(MatrixVariant::Int8(m))),
+            inner: Arc::new(NalgebraDMatrixVariant::Int8(m)),
         }
     }
 
     pub fn from_u64(m: DMatrix<u64>) -> Self {
         Self {
-            inner: Arc::new(Mutex::new(MatrixVariant::UnsignedInt64(m))),
+            inner: Arc::new(NalgebraDMatrixVariant::UnsignedInt64(m)),
         }
     }
 
     pub fn from_u32(m: DMatrix<u32>) -> Self {
         Self {
-            inner: Arc::new(Mutex::new(MatrixVariant::UnsignedInt32(m))),
+            inner: Arc::new(NalgebraDMatrixVariant::UnsignedInt32(m)),
         }
     }
 
     pub fn from_u16(m: DMatrix<u16>) -> Self {
         Self {
-            inner: Arc::new(Mutex::new(MatrixVariant::UnsignedInt16(m))),
+            inner: Arc::new(NalgebraDMatrixVariant::UnsignedInt16(m)),
         }
     }
 
     pub fn from_u8(m: DMatrix<u8>) -> Self {
         Self {
-            inner: Arc::new(Mutex::new(MatrixVariant::UnsignedInt8(m))),
+            inner: Arc::new(NalgebraDMatrixVariant::UnsignedInt8(m)),
         }
     }
 }
 
 #[pymethods]
-impl Matrix {
+impl NalgebraDMatrix {
     #[classattr]
     const __hash__: Option<Py<PyAny>> = None;
 
     fn __repr__(&self) -> String {
-        let m = self.inner.lock().unwrap();
-        match m.deref() {
-            MatrixVariant::Float64(m) => {
+        match self.inner.deref() {
+            NalgebraDMatrixVariant::Float64(m) => {
                 pretty_print!(m)
             }
-            MatrixVariant::Float32(m) => {
+            NalgebraDMatrixVariant::Float32(m) => {
                 pretty_print!(m)
             }
-            MatrixVariant::Int64(m) => {
+            NalgebraDMatrixVariant::Int64(m) => {
                 pretty_print!(m)
             }
-            MatrixVariant::Int32(m) => {
+            NalgebraDMatrixVariant::Int32(m) => {
                 pretty_print!(m)
             }
 
-            MatrixVariant::Int16(m) => {
+            NalgebraDMatrixVariant::Int16(m) => {
                 pretty_print!(m)
             }
-            MatrixVariant::Int8(m) => {
+            NalgebraDMatrixVariant::Int8(m) => {
                 pretty_print!(m)
             }
-            MatrixVariant::UnsignedInt64(m) => {
+            NalgebraDMatrixVariant::UnsignedInt64(m) => {
                 pretty_print!(m)
             }
-            MatrixVariant::UnsignedInt32(m) => {
+            NalgebraDMatrixVariant::UnsignedInt32(m) => {
                 pretty_print!(m)
             }
-            MatrixVariant::UnsignedInt16(m) => {
+            NalgebraDMatrixVariant::UnsignedInt16(m) => {
                 pretty_print!(m)
             }
-            MatrixVariant::UnsignedInt8(m) => {
+            NalgebraDMatrixVariant::UnsignedInt8(m) => {
                 pretty_print!(m)
             }
         }
     }
 
     fn __str__(&self) -> String {
         self.__repr__()
     }
 }
 
-pub fn matrix_to_ndarray<T: ElementType>(m: &DMatrix<T>) -> PyObject {
+pub fn matrix_to_np<T: ElementType>(m: &DMatrix<T>) -> PyObject {
     let arr =
         ArrayD::<T>::from_shape_vec(IxDyn(&[m.nrows(), m.ncols()]), m.as_slice().to_vec()).unwrap();
 
     Python::with_gil(|py| {
         let arr = PyArray::from_array(py, &arr);
         arr.into_py(py)
     })
 }
 
-pub fn ndarray_to_matrix<T: ElementType>(arr: PyReadonlyArrayDyn<T>) -> PyResult<DMatrix<T>> {
+pub fn np_to_matrix<T: ElementType>(arr: PyReadonlyArrayDyn<T>) -> PyResult<DMatrix<T>> {
     let shape = arr.shape().to_vec();
     let slice = arr.as_slice();
     let slice = match slice {
         Ok(slice) => slice,
         Err(_) => {
             return Err(PyValueError::new_err(
                 "Non-contiguous array cannot be converted to DMatrix",
@@ -199,87 +178,98 @@
 
     Python::with_gil(|py| {
         py.allow_threads(|| Ok(nalgebra::DMatrix::from_vec(shape[0], shape[1], slice)))
     })
 }
 
 #[pyfunction]
-#[pyo3(name = "ndarray_to_matrix")]
-pub fn ndarray_to_matrix_py(arr: &PyAny) -> PyResult<PyObject> {
+#[pyo3(name = "np_to_matrix")]
+pub fn np_to_matrix_py(arr: &PyAny) -> PyResult<PyObject> {
     if let Ok(arr) = arr.downcast::<PyArray<f32, IxDyn>>() {
-        let m = ndarray_to_matrix(arr.readonly()).map(Matrix::from_fp32)?;
+        let m = np_to_matrix(arr.readonly()).map(NalgebraDMatrix::from_fp32)?;
         return Python::with_gil(|py| Ok(m.into_py(py)));
     }
 
     if let Ok(arr) = arr.downcast::<PyArray<f64, IxDyn>>() {
-        let m = ndarray_to_matrix(arr.readonly()).map(Matrix::from_fp64)?;
+        let m = np_to_matrix(arr.readonly()).map(NalgebraDMatrix::from_fp64)?;
         return Python::with_gil(|py| Ok(m.into_py(py)));
     }
 
     if let Ok(arr) = arr.downcast::<PyArray<i8, IxDyn>>() {
-        let m = ndarray_to_matrix(arr.readonly()).map(Matrix::from_i8)?;
+        let m = np_to_matrix(arr.readonly()).map(NalgebraDMatrix::from_i8)?;
         return Python::with_gil(|py| Ok(m.into_py(py)));
     }
 
     if let Ok(arr) = arr.downcast::<PyArray<i16, IxDyn>>() {
-        let m = ndarray_to_matrix(arr.readonly()).map(Matrix::from_i16)?;
+        let m = np_to_matrix(arr.readonly()).map(NalgebraDMatrix::from_i16)?;
         return Python::with_gil(|py| Ok(m.into_py(py)));
     }
 
     if let Ok(arr) = arr.downcast::<PyArray<i32, IxDyn>>() {
-        let m = ndarray_to_matrix(arr.readonly()).map(Matrix::from_i32)?;
+        let m = np_to_matrix(arr.readonly()).map(NalgebraDMatrix::from_i32)?;
         return Python::with_gil(|py| Ok(m.into_py(py)));
     }
 
     if let Ok(arr) = arr.downcast::<PyArray<i64, IxDyn>>() {
-        let m = ndarray_to_matrix(arr.readonly()).map(Matrix::from_i64)?;
+        let m = np_to_matrix(arr.readonly()).map(NalgebraDMatrix::from_i64)?;
         return Python::with_gil(|py| Ok(m.into_py(py)));
     }
 
     if let Ok(arr) = arr.downcast::<PyArray<u8, IxDyn>>() {
-        let m = ndarray_to_matrix(arr.readonly()).map(Matrix::from_u8)?;
+        let m = np_to_matrix(arr.readonly()).map(NalgebraDMatrix::from_u8)?;
         return Python::with_gil(|py| Ok(m.into_py(py)));
     }
 
     if let Ok(arr) = arr.downcast::<PyArray<u16, IxDyn>>() {
-        let m = ndarray_to_matrix(arr.readonly()).map(Matrix::from_u16)?;
+        let m = np_to_matrix(arr.readonly()).map(NalgebraDMatrix::from_u16)?;
         return Python::with_gil(|py| Ok(m.into_py(py)));
     }
 
     if let Ok(arr) = arr.downcast::<PyArray<u32, IxDyn>>() {
-        let m = ndarray_to_matrix(arr.readonly()).map(Matrix::from_u32)?;
+        let m = np_to_matrix(arr.readonly()).map(NalgebraDMatrix::from_u32)?;
         return Python::with_gil(|py| Ok(m.into_py(py)));
     }
 
     if let Ok(arr) = arr.downcast::<PyArray<u64, IxDyn>>() {
-        let m = ndarray_to_matrix(arr.readonly()).map(Matrix::from_u64)?;
+        let m = np_to_matrix(arr.readonly()).map(NalgebraDMatrix::from_u64)?;
         return Python::with_gil(|py| Ok(m.into_py(py)));
     }
 
     Err(pyo3::exceptions::PyTypeError::new_err(
         "Expected ndarray of type f32/64, i8/16/32/64, or u8/16/32/64",
     ))
 }
 
 #[pyfunction]
-#[pyo3(name = "matrix_to_ndarray")]
-pub fn matrix_to_ndarray_py(m: &PyAny) -> PyResult<PyObject> {
-    if let Ok(m) = m.extract::<Matrix>() {
-        let m = match m.inner.lock().unwrap().deref() {
-            MatrixVariant::Float64(m) => matrix_to_ndarray(m),
-            MatrixVariant::Float32(m) => matrix_to_ndarray(m),
-            MatrixVariant::Int64(m) => matrix_to_ndarray(m),
-            MatrixVariant::Int32(m) => matrix_to_ndarray(m),
-            MatrixVariant::Int16(m) => matrix_to_ndarray(m),
-            MatrixVariant::Int8(m) => matrix_to_ndarray(m),
-            MatrixVariant::UnsignedInt64(m) => matrix_to_ndarray(m),
-            MatrixVariant::UnsignedInt32(m) => matrix_to_ndarray(m),
-            MatrixVariant::UnsignedInt16(m) => matrix_to_ndarray(m),
-            MatrixVariant::UnsignedInt8(m) => matrix_to_ndarray(m),
+#[pyo3(name = "matrix_to_np")]
+pub fn matrix_to_np_py(m: &PyAny) -> PyResult<PyObject> {
+    if let Ok(m) = m.extract::<NalgebraDMatrix>() {
+        let m = match m.inner.deref() {
+            NalgebraDMatrixVariant::Float64(m) => matrix_to_np(m),
+            NalgebraDMatrixVariant::Float32(m) => matrix_to_np(m),
+            NalgebraDMatrixVariant::Int64(m) => matrix_to_np(m),
+            NalgebraDMatrixVariant::Int32(m) => matrix_to_np(m),
+            NalgebraDMatrixVariant::Int16(m) => matrix_to_np(m),
+            NalgebraDMatrixVariant::Int8(m) => matrix_to_np(m),
+            NalgebraDMatrixVariant::UnsignedInt64(m) => matrix_to_np(m),
+            NalgebraDMatrixVariant::UnsignedInt32(m) => matrix_to_np(m),
+            NalgebraDMatrixVariant::UnsignedInt16(m) => matrix_to_np(m),
+            NalgebraDMatrixVariant::UnsignedInt8(m) => matrix_to_np(m),
         };
         return Ok(m);
     }
 
     Err(pyo3::exceptions::PyTypeError::new_err(
-        "Expected ndarray of type f32, f64, i32 or i64",
+        "Expected ndarray of type f32/64, i8/16/32/64, or u8/16/32/64",
     ))
 }
+
+#[cfg(test)]
+mod tests {
+    #[test]
+    fn test_cast() {
+        let m = nalgebra::DMatrix::<i8>::from_row_slice(2, 2, &[1, 2, 3, 4]);
+        let _n = m.clone().cast::<f64>();
+        let _n = m.clone().cast::<f32>();
+        let _n = m.cast::<i64>();
+    }
+}
```

### Comparing `savant_rs-0.1.7/src/utils/symbol_mapper.rs` & `savant_rs-0.1.9/src/utils/symbol_mapper.rs`

 * *Files 2% similar despite different names*

```diff
@@ -30,37 +30,49 @@
     #[error("The key `{0}` is expected to be a base name of the form `some-thing_name` without `.` symbols.")]
     BaseNameParseError(String),
     #[error("For model `{0}({1})` the `{2}({3})` object already exists and policy is set to `ErrorIfNonUnique`.")]
     DuplicateId(String, i64, String, i64),
 }
 
 #[pyfunction]
-pub fn get_model_id(model_name: String) -> PyResult<i64> {
+#[pyo3(name = "get_model_id")]
+pub fn get_model_id_py(model_name: String) -> PyResult<i64> {
     Python::with_gil(|py| {
         py.allow_threads(|| {
             let mut mapper = SYMBOL_MAPPER.lock().unwrap();
             mapper
                 .get_model_id(&model_name)
                 .map_err(|e| PyValueError::new_err(e.to_string()))
         })
     })
 }
 
+pub fn get_model_id(model_name: &String) -> anyhow::Result<i64> {
+    let mut mapper = SYMBOL_MAPPER.lock().unwrap();
+    mapper.get_model_id(model_name)
+}
+
 #[pyfunction]
-pub fn get_object_id(model_name: String, object_label: String) -> PyResult<(i64, i64)> {
+#[pyo3(name = "get_object_id")]
+pub fn get_object_id_py(model_name: String, object_label: String) -> PyResult<(i64, i64)> {
     Python::with_gil(|py| {
         py.allow_threads(|| {
             let mut mapper = SYMBOL_MAPPER.lock().unwrap();
             mapper
                 .get_object_id(&model_name, &object_label)
                 .map_err(|e| PyValueError::new_err(e.to_string()))
         })
     })
 }
 
+pub fn get_object_id(model_name: &String, object_label: &String) -> anyhow::Result<(i64, i64)> {
+    let mut mapper = SYMBOL_MAPPER.lock().unwrap();
+    mapper.get_object_id(model_name, object_label)
+}
+
 #[pyfunction]
 pub fn register_model_objects(
     model_name: String,
     elements: StdHashMap<i64, String>,
     policy: RegistrationPolicy,
 ) -> PyResult<i64> {
     Python::with_gil(|py| {
@@ -456,15 +468,15 @@
 }
 
 #[cfg(test)]
 mod tests {
     use super::SymbolMapper;
     use crate::test::utils::s;
     use crate::utils::symbol_mapper::{
-        clear_symbol_maps, get_model_id, get_model_name, get_object_id, get_object_label,
+        clear_symbol_maps, get_model_id_py, get_model_name, get_object_id_py, get_object_label,
         register_model_objects, RegistrationPolicy,
     };
     use serial_test::serial;
 
     #[test]
     fn test_validate_base_key() {
         assert!(matches!(SymbolMapper::validate_base_key(&s("")), Err(_)));
@@ -594,15 +606,18 @@
                 s("model"),
                 [(2, s("object"))].into_iter().collect(),
                 RegistrationPolicy::Override,
             ),
             Ok(0)
         ));
 
-        assert!(matches!(get_object_id(s("model"), s("object")), Ok((0, 2))));
+        assert!(matches!(
+            get_object_id_py(s("model"), s("object")),
+            Ok((0, 2))
+        ));
 
         let label = get_object_label(0, 2).unwrap();
         assert_eq!(label, s("object"));
 
         clear_symbol_maps();
 
         register_model_objects(
@@ -626,78 +641,78 @@
         Ok(())
     }
 
     #[test]
     #[serial]
     fn test_get_model_id() {
         clear_symbol_maps();
-        let model_id = get_model_id(s("model")).unwrap();
+        let model_id = get_model_id_py(s("model")).unwrap();
         assert_eq!(model_id, 0);
     }
 
     #[test]
     #[serial]
     fn test_get_model_name() {
         clear_symbol_maps();
-        let model_id = get_model_id(s("model")).unwrap();
+        let model_id = get_model_id_py(s("model")).unwrap();
         assert_eq!(model_id, 0);
 
         let model_name = get_model_name(model_id).unwrap();
         assert_eq!(model_name, s("model"));
 
         let nonexistent_model_name = get_model_name(1);
         assert!(matches!(nonexistent_model_name, None));
     }
 
     #[test]
     #[serial]
     fn test_get_object_label() {
         clear_symbol_maps();
-        let (model_id, object_id) = get_object_id(s("model"), s("object")).unwrap();
+        let (model_id, object_id) = get_object_id_py(s("model"), s("object")).unwrap();
         assert_eq!(model_id, 0);
         assert_eq!(object_id, 0);
 
         let object_label = get_object_label(model_id, object_id).unwrap();
         assert_eq!(object_label, s("object"));
 
         let nonexistent_object_label = get_object_label(0, 1);
         assert!(matches!(nonexistent_object_label, None));
     }
 
     #[test]
     #[serial]
     fn get_model_object_ids() {
         clear_symbol_maps();
-        let (model_id, object_id) = get_object_id(s("model"), s("object0")).unwrap();
+        let (model_id, object_id) = get_object_id_py(s("model"), s("object0")).unwrap();
         assert_eq!(model_id, 0);
         assert_eq!(object_id, 0);
 
-        let (model_id, object_id) = get_object_id(s("model"), s("object1")).unwrap();
+        let (model_id, object_id) = get_object_id_py(s("model"), s("object1")).unwrap();
         assert_eq!(model_id, 0);
         assert_eq!(object_id, 1);
 
-        let (model_id, object_id) = get_object_id(s("model2"), s("object0")).unwrap();
+        let (model_id, object_id) = get_object_id_py(s("model2"), s("object0")).unwrap();
         assert_eq!(model_id, 1);
         assert_eq!(object_id, 0);
     }
 
     #[test]
     #[serial]
     fn register_and_get_model_object_ids() -> anyhow::Result<()> {
         clear_symbol_maps();
         register_model_objects(
             s("model"),
             [(2, s("object0"))].into_iter().collect(),
             RegistrationPolicy::Override,
         )?;
 
-        let (model_id, object_id) = get_object_id(s("model"), s("object0")).unwrap();
+        let (model_id, object_id) = get_object_id_py(s("model"), s("object0")).unwrap();
         assert_eq!(model_id, 0);
         assert_eq!(object_id, 2);
 
-        let (model_id, object_id) = get_object_id(s("model"), s("object1")).unwrap();
+        let (model_id, object_id) = get_object_id_py(s("model"), s("object1")).unwrap();
         assert_eq!(model_id, 0);
         assert_eq!(object_id, 3);
 
         Ok(())
     }
 }
```

### Comparing `savant_rs-0.1.7/src/utils.rs` & `savant_rs-0.1.9/src/utils.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 pub mod bbox;
 pub mod conversions;
 pub mod fps_meter;
-pub mod numpy_utils;
+pub mod np;
+pub mod python;
 pub mod symbol_mapper;
 
 use pyo3::prelude::*;
 
 use crate::primitives::message::loader::load_message_py;
 use crate::primitives::message::saver::save_message_py;
 use crate::test::utils::gen_frame;
+use crate::utils::np::np_nalgebra;
+use crate::utils::np::np_ndarray;
 use crate::utils::symbol_mapper::RegistrationPolicy;
 use crate::utils::symbol_mapper::SymbolMapper;
 use crate::utils::symbol_mapper::{
-    build_model_object_key, clear_symbol_maps, dump_registry, get_model_id, get_model_name,
-    get_object_id, get_object_ids, get_object_label, get_object_labels, is_model_registered,
+    build_model_object_key, clear_symbol_maps, dump_registry, get_model_id_py, get_model_name,
+    get_object_id_py, get_object_ids, get_object_label, get_object_labels, is_model_registered,
     is_object_registered, parse_compound_key, register_model_objects, validate_base_key,
 };
 
 pub use bbox::*;
 pub use fps_meter::FpsMeter;
-pub use numpy_utils::*;
+pub use np_nalgebra::*;
+pub use np_ndarray::*;
 
 #[pyfunction]
 #[inline]
 pub fn round_2_digits(v: f64) -> f64 {
     (v * 100.0).round() / 100.0
 }
 
@@ -39,34 +43,37 @@
     // bbox batch ops
     m.add_function(wrap_pyfunction!(rotated_bboxes_to_ndarray_py, m)?)?;
     m.add_function(wrap_pyfunction!(bboxes_to_ndarray_py, m)?)?;
     m.add_function(wrap_pyfunction!(ndarray_to_bboxes_py, m)?)?;
     m.add_function(wrap_pyfunction!(ndarray_to_rotated_bboxes_py, m)?)?;
 
     // numpy utils
-    m.add_function(wrap_pyfunction!(ndarray_to_matrix_py, m)?)?;
-    m.add_function(wrap_pyfunction!(matrix_to_ndarray_py, m)?)?;
+    m.add_function(wrap_pyfunction!(np_to_matrix_py, m)?)?;
+    m.add_function(wrap_pyfunction!(matrix_to_np_py, m)?)?;
+    m.add_function(wrap_pyfunction!(np_to_ndarray_py, m)?)?;
+    m.add_function(wrap_pyfunction!(ndarray_to_np_py, m)?)?;
 
     // model object registry
     m.add_function(wrap_pyfunction!(build_model_object_key, m)?)?;
     m.add_function(wrap_pyfunction!(clear_symbol_maps, m)?)?;
     m.add_function(wrap_pyfunction!(dump_registry, m)?)?;
-    m.add_function(wrap_pyfunction!(get_model_id, m)?)?;
+    m.add_function(wrap_pyfunction!(get_model_id_py, m)?)?;
     m.add_function(wrap_pyfunction!(get_model_name, m)?)?;
-    m.add_function(wrap_pyfunction!(get_object_id, m)?)?;
+    m.add_function(wrap_pyfunction!(get_object_id_py, m)?)?;
     m.add_function(wrap_pyfunction!(get_object_ids, m)?)?;
     m.add_function(wrap_pyfunction!(get_object_label, m)?)?;
     m.add_function(wrap_pyfunction!(get_object_labels, m)?)?;
     m.add_function(wrap_pyfunction!(is_model_registered, m)?)?;
     m.add_function(wrap_pyfunction!(is_object_registered, m)?)?;
     m.add_function(wrap_pyfunction!(parse_compound_key, m)?)?;
     m.add_function(wrap_pyfunction!(register_model_objects, m)?)?;
     m.add_function(wrap_pyfunction!(validate_base_key, m)?)?;
 
     m.add_class::<FpsMeter>()?;
     m.add_class::<SymbolMapper>()?;
     m.add_class::<RegistrationPolicy>()?;
     m.add_class::<BBoxFormat>()?;
-    m.add_class::<Matrix>()?;
+    m.add_class::<NalgebraDMatrix>()?;
+    m.add_class::<NDarray>()?;
 
     Ok(())
 }
```

### Comparing `savant_rs-0.1.7/Cargo.lock` & `savant_rs-0.1.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -258,14 +258,20 @@
 checksum = "ebcda35c7a396850a55ffeac740804b40ffec779b98fffbb1738f4033f0ee79e"
 dependencies = [
  "derive_builder_core",
  "syn 1.0.109",
 ]
 
 [[package]]
+name = "deunicode"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "850878694b7933ca4c9569d30a34b55031b9b139ee1fc7b94a527c4ef960d690"
+
+[[package]]
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "env_logger"
@@ -507,14 +513,24 @@
 [[package]]
 name = "ident_case"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9e0384b61958566e926dc50660321d12159025e767c18e043daf26b70104c39"
 
 [[package]]
+name = "indexmap"
+version = "1.9.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
+dependencies = [
+ "autocfg",
+ "hashbrown 0.12.3",
+]
+
+[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "io-lifetimes"
@@ -551,14 +567,26 @@
 [[package]]
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
+name = "jmespath"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "017f8f53dd3b8ada762acb1f850da2a742d0ef3f921c60849a644380de1d683a"
+dependencies = [
+ "lazy_static",
+ "serde",
+ "serde_json",
+ "slug",
+]
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
@@ -570,17 +598,17 @@
 name = "libm"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.7"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ece97ea872ece730aed82664c424eb4c8291e1ff2480247ccf7409044bc6479f"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -594,14 +622,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "lru"
+version = "0.10.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "03f1160296536f10c833a82dca22267d5486734230d47bf00bf435885814ba1e"
+dependencies = [
+ "hashbrown 0.13.2",
+]
+
+[[package]]
 name = "matrixmultiply"
 version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
  "autocfg",
  "rawpointer",
@@ -773,17 +810,17 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.57"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4ec6d5fe0b140acb27c9a0444118cf55bfbb4e0b259739429abb4521dd67c16"
+checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.1.4"
@@ -1040,33 +1077,38 @@
 checksum = "794821e4ccb0d9f979512f9c1973480123f9bd62a90d74ab0f9426fcf8f4a529"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "savant_rs"
-version = "0.1.7"
+version = "0.1.9"
 dependencies = [
  "anyhow",
  "derive_builder",
  "env_logger",
  "geo",
  "hashbrown 0.13.2",
  "itertools",
+ "jmespath",
  "lazy_static",
+ "lru",
  "nalgebra",
+ "ndarray",
  "num-traits",
  "num_cpus",
  "numpy",
  "pyo3",
  "pyo3-build-config",
  "pyo3-log",
  "rayon",
  "rkyv",
+ "serde",
  "serde_json",
+ "serde_yaml",
  "serial_test",
  "thiserror",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
@@ -1113,14 +1155,27 @@
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "serde_yaml"
+version = "0.9.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d9d684e3ec7de3bf5466b32bd75303ac16f0736426e5a4e0d6e489559ce1249c"
+dependencies = [
+ "indexmap",
+ "itoa",
+ "ryu",
+ "serde",
+ "unsafe-libyaml",
+]
+
+[[package]]
 name = "serial_test"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e56dd856803e253c8f298af3f4d7eb0ae5e23a737252cd90bb4f3b435033b2d"
 dependencies = [
  "dashmap",
  "futures",
@@ -1166,14 +1221,23 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "slug"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b3bc762e6a4b6c6fcaade73e77f9ebc6991b676f88bb2358bddb56560f073373"
+dependencies = [
+ "deunicode",
+]
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "spin"
@@ -1289,14 +1353,20 @@
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "unsafe-libyaml"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1865806a559042e51ab5414598446a5871b561d21b6764f2eabb0dd481d880a6"
+
+[[package]]
 name = "uuid"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 
 [[package]]
 name = "version_check"
@@ -1308,17 +1378,17 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wide"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b689b6c49d6549434bf944e6b0f39238cf63693cb7a147e9d887507fffa3b223"
+checksum = "5cd0496a71f3cc6bc4bf0ed91346426a5099e93d89807e663162dc5a1069ff65"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
```

### Comparing `savant_rs-0.1.7/PKG-INFO` & `savant_rs-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: savant_rs
-Version: 0.1.7
+Version: 0.1.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Savant rust optimization library
 Keywords: computer-vision,video-processing
 Home-Page: https://github.com/insight-platform/savant-rs
```

