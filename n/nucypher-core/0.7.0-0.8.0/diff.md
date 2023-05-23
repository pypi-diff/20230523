# Comparing `tmp/nucypher_core-0.7.0.tar.gz` & `tmp/nucypher_core-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nucypher_core-0.7.0.tar", last modified: Tue May  2 04:30:01 2023, max compression
+gzip compressed data, was "nucypher_core-0.8.0.tar", last modified: Tue May 23 18:41:53 2023, max compression
```

## Comparing `nucypher_core-0.7.0.tar` & `nucypher_core-0.8.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:30:01.974393 nucypher_core-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-02 04:30:01.970394 nucypher_core-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:30:01.970394 nucypher_core-0.7.0/nucypher_core/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/nucypher_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/nucypher_core/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/nucypher_core/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/nucypher_core/umbral.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/nucypher_core/umbral.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:30:01.970394 nucypher_core-0.7.0/nucypher_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/nucypher_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/nucypher_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/nucypher_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/nucypher_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-02 04:30:01.000000 nucypher_core-0.7.0/nucypher_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 04:30:01.974393 nucypher_core-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 04:30:01.970394 nucypher_core-0.7.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    32681 2023-05-02 04:29:53.000000 nucypher_core-0.7.0/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-23 18:41:52.000000 nucypher_core-0.8.0/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/nucypher_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/nucypher_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9407 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/nucypher_core/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/nucypher_core/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/nucypher_core/umbral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/nucypher_core/umbral.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/nucypher_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-23 18:41:53.000000 nucypher_core-0.8.0/nucypher_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-23 18:41:53.000000 nucypher_core-0.8.0/nucypher_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:41:53.000000 nucypher_core-0.8.0/nucypher_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 18:41:53.000000 nucypher_core-0.8.0/nucypher_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 18:41:53.000000 nucypher_core-0.8.0/nucypher_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 18:41:53.343473 nucypher_core-0.8.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    35990 2023-05-23 18:41:49.000000 nucypher_core-0.8.0/src/lib.rs
```

### Comparing `nucypher_core-0.7.0/LICENSE` & `nucypher_core-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nucypher_core-0.7.0/PKG-INFO` & `nucypher_core-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucypher_core
-Version: 0.7.0
+Version: 0.8.0
 Summary: Protocol structures of Nucypher network
 Home-page: https://github.com/nucypher/nucypher-core/tree/main/nucypher-core-python
 Author: Bogdan Opanchuk
 Author-email: bogdan@opanchuk.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nucypher_core-0.7.0/README.md` & `nucypher_core-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `nucypher_core-0.7.0/nucypher_core/__init__.pyi` & `nucypher_core-0.8.0/nucypher_core/__init__.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -404,44 +404,91 @@
 
 
 class ThresholdDecryptionRequest:
 
     def __init__(self, ritual_id: int, variant: int, ciphertext: bytes, conditions: Optional[Conditions], context: Optional[Context]):
         ...
 
-    def id(self) -> int:
+    ritual_id: int
+
+    conditions: Optional[Conditions]
+
+    context: Optional[Context]
+
+    variant: int
+
+    ciphertext: bytes
+
+    def encrypt(self, request_encrypting_key: PublicKey, response_encrypting_key: PublicKey) -> EncryptedThresholdDecryptionRequest:
         ...
 
-    def conditions(self) -> Optional[Conditions]:
+    @staticmethod
+    def from_bytes(data: bytes) -> ThresholdDecryptionRequest:
         ...
 
-    def context(self) -> Optional[Context]:
+    def __bytes__(self) -> bytes:
+        ...
+
+
+class E2EThresholdDecryptionRequest:
+
+    decryption_request: ThresholdDecryptionRequest
+
+    response_encrypting_key: PublicKey
+
+    @staticmethod
+    def from_bytes(data: bytes) -> E2EThresholdDecryptionRequest:
         ...
 
-    def variant(self) -> int:
+    def __bytes__(self) -> bytes:
         ...
 
-    def ciphertext(self) -> bytes:
+
+class EncryptedThresholdDecryptionRequest:
+    ritual_id: int
+
+    def decrypt(
+        self,
+        sk: SecretKey
+    ) -> E2EThresholdDecryptionRequest:
         ...
 
     @staticmethod
-    def from_bytes(data: bytes) -> ThresholdDecryptionRequest:
+    def from_bytes(data: bytes) -> EncryptedThresholdDecryptionRequest:
         ...
 
     def __bytes__(self) -> bytes:
         ...
 
 
 class ThresholdDecryptionResponse:
 
     def __init__(self, decryption_share: bytes):
         ...
 
-    def decryption_share(self) -> bytes:
+    decryption_share: bytes
+
+    def encrypt(self, encrypting_key: PublicKey) -> EncryptedThresholdDecryptionResponse:
         ...
 
     @staticmethod
     def from_bytes(data: bytes) -> ThresholdDecryptionResponse:
         ...
 
     def __bytes__(self) -> bytes:
         ...
+
+
+class EncryptedThresholdDecryptionResponse:
+
+    def decrypt(
+        self,
+        sk: SecretKey
+    ) -> ThresholdDecryptionResponse:
+        ...
+
+    @staticmethod
+    def from_bytes(data: bytes) -> EncryptedThresholdDecryptionResponse:
+        ...
+
+    def __bytes__(self) -> bytes:
+        ...
```

### Comparing `nucypher_core-0.7.0/nucypher_core/umbral.py` & `nucypher_core-0.8.0/nucypher_core/umbral.py`

 * *Files identical despite different names*

### Comparing `nucypher_core-0.7.0/nucypher_core/umbral.pyi` & `nucypher_core-0.8.0/nucypher_core/umbral.pyi`

 * *Files identical despite different names*

### Comparing `nucypher_core-0.7.0/nucypher_core.egg-info/PKG-INFO` & `nucypher_core-0.8.0/nucypher_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucypher-core
-Version: 0.7.0
+Version: 0.8.0
 Summary: Protocol structures of Nucypher network
 Home-page: https://github.com/nucypher/nucypher-core/tree/main/nucypher-core-python
 Author: Bogdan Opanchuk
 Author-email: bogdan@opanchuk.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nucypher_core-0.7.0/setup.py` & `nucypher_core-0.8.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="nucypher_core",
     description="Protocol structures of Nucypher network",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.7.0",
+    version="0.8.0",
     author="Bogdan Opanchuk",
     author_email="bogdan@opanchuk.net",
     url="https://github.com/nucypher/nucypher-core/tree/main/nucypher-core-python",
     rust_extensions=[RustExtension("nucypher_core._nucypher_core", binding=Binding.PyO3, debug=False)],
     packages=["nucypher_core"],
     package_data = {
         'nucypher_core': ['py.typed', '__init__.pyi', 'umbral.pyi'],
```

### Comparing `nucypher_core-0.7.0/src/lib.rs` & `nucypher_core-0.8.0/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -641,15 +641,15 @@
     backend: nucypher_core::ThresholdDecryptionRequest,
 }
 
 #[pymethods]
 impl ThresholdDecryptionRequest {
     #[new]
     pub fn new(
-        id: u16,
+        ritual_id: u16,
         variant: u8,
         ciphertext: &[u8], // TODO use ferveo Ciphertext type
         conditions: Option<&Conditions>,
         context: Option<&Context>,
     ) -> PyResult<Self> {
         let ferveo_variant = match variant {
             0 => FerveoVariant::SIMPLE,
@@ -659,27 +659,27 @@
                     "Invalid ThresholdDecryptionRequest variant",
                 ))
             }
         };
 
         Ok(Self {
             backend: nucypher_core::ThresholdDecryptionRequest::new(
-                id,
+                ritual_id,
                 ciphertext,
                 conditions
                     .map(|conditions| conditions.backend.clone())
                     .as_ref(),
                 context.map(|context| context.backend.clone()).as_ref(),
                 ferveo_variant,
             ),
         })
     }
 
     #[getter]
-    pub fn id(&self) -> u16 {
+    pub fn ritual_id(&self) -> u16 {
         self.backend.ritual_id
     }
 
     #[getter]
     pub fn conditions(&self) -> Option<Conditions> {
         self.backend
             .conditions
@@ -706,25 +706,103 @@
     pub fn variant(&self) -> u8 {
         match self.backend.variant {
             FerveoVariant::SIMPLE => 0,
             FerveoVariant::PRECOMPUTED => 1,
         }
     }
 
+    pub fn encrypt(
+        &self,
+        request_encrypting_key: &PublicKey,
+        response_encrypting_key: &PublicKey,
+    ) -> EncryptedThresholdDecryptionRequest {
+        EncryptedThresholdDecryptionRequest {
+            backend: self.backend.encrypt(
+                request_encrypting_key.as_ref(),
+                response_encrypting_key.as_ref(),
+            ),
+        }
+    }
+
     #[staticmethod]
     pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
         from_bytes::<_, nucypher_core::ThresholdDecryptionRequest>(data)
     }
 
     fn __bytes__(&self) -> PyObject {
         to_bytes(self)
     }
 }
 
 //
+// E2EThresholdDecryptionRequest
+//
+#[pyclass(module = "nucypher_core")]
+#[derive(derive_more::From, derive_more::AsRef)]
+pub struct E2EThresholdDecryptionRequest {
+    backend: nucypher_core::E2EThresholdDecryptionRequest,
+}
+
+#[pymethods]
+impl E2EThresholdDecryptionRequest {
+    #[getter]
+    pub fn decryption_request(&self) -> ThresholdDecryptionRequest {
+        self.backend.decryption_request.clone().into()
+    }
+
+    #[getter]
+    pub fn response_encrypting_key(&self) -> PublicKey {
+        self.backend.response_encrypting_key.into()
+    }
+
+    #[staticmethod]
+    pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
+        from_bytes::<_, nucypher_core::E2EThresholdDecryptionRequest>(data)
+    }
+
+    fn __bytes__(&self) -> PyObject {
+        to_bytes(self)
+    }
+}
+
+//
+// EncryptedThresholdDecryptionRequest
+//
+
+#[pyclass(module = "nucypher_core")]
+#[derive(derive_more::From, derive_more::AsRef)]
+pub struct EncryptedThresholdDecryptionRequest {
+    backend: nucypher_core::EncryptedThresholdDecryptionRequest,
+}
+
+#[pymethods]
+impl EncryptedThresholdDecryptionRequest {
+    #[getter]
+    pub fn ritual_id(&self) -> u16 {
+        self.backend.ritual_id
+    }
+
+    pub fn decrypt(&self, sk: &SecretKey) -> PyResult<E2EThresholdDecryptionRequest> {
+        self.backend
+            .decrypt(sk.as_ref())
+            .map(E2EThresholdDecryptionRequest::from)
+            .map_err(|err| PyValueError::new_err(format!("{}", err)))
+    }
+
+    #[staticmethod]
+    pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
+        from_bytes::<_, nucypher_core::EncryptedThresholdDecryptionRequest>(data)
+    }
+
+    fn __bytes__(&self) -> PyObject {
+        to_bytes(self)
+    }
+}
+
+//
 // Threshold Decryption Response
 //
 
 #[pyclass(module = "nucypher_core")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct ThresholdDecryptionResponse {
     backend: nucypher_core::ThresholdDecryptionResponse,
@@ -740,25 +818,60 @@
     }
 
     #[getter]
     pub fn decryption_share(&self) -> &[u8] {
         self.backend.decryption_share.as_ref()
     }
 
+    pub fn encrypt(&self, encrypting_key: &PublicKey) -> EncryptedThresholdDecryptionResponse {
+        EncryptedThresholdDecryptionResponse {
+            backend: self.backend.encrypt(encrypting_key.as_ref()),
+        }
+    }
+
     #[staticmethod]
     pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
         from_bytes::<_, nucypher_core::ThresholdDecryptionResponse>(data)
     }
 
     fn __bytes__(&self) -> PyObject {
         to_bytes(self)
     }
 }
 
 //
+// EncryptedThresholdDecryptionResponse
+//
+
+#[pyclass(module = "nucypher_core")]
+#[derive(derive_more::From, derive_more::AsRef)]
+pub struct EncryptedThresholdDecryptionResponse {
+    backend: nucypher_core::EncryptedThresholdDecryptionResponse,
+}
+
+#[pymethods]
+impl EncryptedThresholdDecryptionResponse {
+    pub fn decrypt(&self, sk: &SecretKey) -> PyResult<ThresholdDecryptionResponse> {
+        self.backend
+            .decrypt(sk.as_ref())
+            .map(ThresholdDecryptionResponse::from)
+            .map_err(|err| PyValueError::new_err(format!("{}", err)))
+    }
+
+    #[staticmethod]
+    pub fn from_bytes(data: &[u8]) -> PyResult<Self> {
+        from_bytes::<_, nucypher_core::EncryptedThresholdDecryptionResponse>(data)
+    }
+
+    fn __bytes__(&self) -> PyObject {
+        to_bytes(self)
+    }
+}
+
+//
 // RetrievalKit
 //
 
 #[pyclass(module = "nucypher_core")]
 #[derive(derive_more::From, derive_more::AsRef)]
 pub struct RetrievalKit {
     backend: nucypher_core::RetrievalKit,
@@ -1216,15 +1329,18 @@
     m.add_class::<NodeMetadata>()?;
     m.add_class::<NodeMetadataPayload>()?;
     m.add_class::<FleetStateChecksum>()?;
     m.add_class::<MetadataRequest>()?;
     m.add_class::<MetadataResponsePayload>()?;
     m.add_class::<MetadataResponse>()?;
     m.add_class::<ThresholdDecryptionRequest>()?;
+    m.add_class::<E2EThresholdDecryptionRequest>()?;
     m.add_class::<ThresholdDecryptionResponse>()?;
+    m.add_class::<EncryptedThresholdDecryptionRequest>()?;
+    m.add_class::<EncryptedThresholdDecryptionResponse>()?;
 
     let umbral_module = PyModule::new(py, "umbral")?;
 
     umbral_module.add_class::<umbral_pre::bindings_python::SecretKey>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::SecretKeyFactory>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::PublicKey>()?;
     umbral_module.add_class::<umbral_pre::bindings_python::Capsule>()?;
```

