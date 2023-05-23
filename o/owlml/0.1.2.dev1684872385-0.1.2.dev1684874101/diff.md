# Comparing `tmp/owlml-0.1.2.dev1684872385.tar.gz` & `tmp/owlml-0.1.2.dev1684874101.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlml-0.1.2.dev1684872385.tar", last modified: Tue May 23 20:06:37 2023, max compression
+gzip compressed data, was "owlml-0.1.2.dev1684874101.tar", last modified: Tue May 23 20:35:12 2023, max compression
```

## Comparing `owlml-0.1.2.dev1684872385.tar` & `owlml-0.1.2.dev1684874101.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:37.054124 owlml-0.1.2.dev1684872385/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 20:05:52.000000 owlml-0.1.2.dev1684872385/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 20:06:37.054124 owlml-0.1.2.dev1684872385/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-23 20:05:52.000000 owlml-0.1.2.dev1684872385/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:37.054124 owlml-0.1.2.dev1684872385/owlml/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-23 20:05:52.000000 owlml-0.1.2.dev1684872385/owlml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-23 20:05:52.000000 owlml-0.1.2.dev1684872385/owlml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-23 20:05:52.000000 owlml-0.1.2.dev1684872385/owlml/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 20:05:52.000000 owlml-0.1.2.dev1684872385/owlml/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-23 20:05:52.000000 owlml-0.1.2.dev1684872385/owlml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-23 20:05:52.000000 owlml-0.1.2.dev1684872385/owlml/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:06:37.054124 owlml-0.1.2.dev1684872385/owlml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 20:06:37.000000 owlml-0.1.2.dev1684872385/owlml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 20:06:37.000000 owlml-0.1.2.dev1684872385/owlml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:06:37.000000 owlml-0.1.2.dev1684872385/owlml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 20:06:37.000000 owlml-0.1.2.dev1684872385/owlml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 20:06:37.000000 owlml-0.1.2.dev1684872385/owlml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:06:37.000000 owlml-0.1.2.dev1684872385/owlml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 20:06:37.054124 owlml-0.1.2.dev1684872385/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:05:52.000000 owlml-0.1.2.dev1684872385/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:35:12.970708 owlml-0.1.2.dev1684874101/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 20:35:12.970708 owlml-0.1.2.dev1684874101/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:35:12.966708 owlml-0.1.2.dev1684874101/owlml/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:35:12.970708 owlml-0.1.2.dev1684874101/owlml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 20:35:12.970708 owlml-0.1.2.dev1684874101/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/setup.py
```

### Comparing `owlml-0.1.2.dev1684872385/LICENSE` & `owlml-0.1.2.dev1684874101/LICENSE`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684872385/README.md` & `owlml-0.1.2.dev1684874101/README.md`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684872385/owlml/__main__.py` & `owlml-0.1.2.dev1684874101/owlml/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """Main entry point for OwlML CLI."""
 import fire
 
 from .auth import assign_batch, create_org, create_user, invite_user
-from .datasets import create_dataset
+from .datasets import create_dataset, version_dataset
 from .images import upload_images
 
 
 def main() -> None:
     """Expose CLI commands."""
     fire.Fire(
         {
             "assign-batch": assign_batch,
             "create-dataset": create_dataset,
             "create-org": create_org,
             "create-user": create_user,
             "invite-user": invite_user,
             "upload-images": upload_images,
+            "version-dataset": version_dataset,
         }
     )
```

### Comparing `owlml-0.1.2.dev1684872385/owlml/api.py` & `owlml-0.1.2.dev1684874101/owlml/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,19 @@
     base_url: str = _get_required_env_var("OWLML_API")
 
     @classmethod
     def get(cls, route: str) -> dict[str, Any]:
         """Make a GET request to the OwlML API."""
         response = requests.get(os.path.join(cls.base_url, route))
         raise_for_status(response)
+        if response.status_code == 204:
+            return {}
         return response.json()
 
     @classmethod
     def post(cls, route: str, payload: dict[str, Any] = dict()) -> dict[str, Any]:
         """Make a POST request to the OwlML API."""
         response = requests.post(os.path.join(cls.base_url, route), json=payload)
         raise_for_status(response)
+        if response.status_code == 204:
+            return {}
         return response.json()
```

### Comparing `owlml-0.1.2.dev1684872385/owlml/auth.py` & `owlml-0.1.2.dev1684874101/owlml/auth.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684872385/owlml/images.py` & `owlml-0.1.2.dev1684874101/owlml/images.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 
 def _complete_image(image_id: str) -> dict[str, Any]:
     """Complete an image."""
     return OwlMLAPI.post(f"images/{image_id}/complete", dict())
 
 
 def upload_images(
-    dataset: str, image_directory: Union[str, Path], batch: Optional[str] = None
+    dataset: str, image_directory: Union[str, Path], batch_slug: Optional[str] = None
 ) -> dict[str, Any]:
     """Upload images to a dataset."""
-    batch = _create_batch(dataset)
+    batch = _create_batch(dataset, batch_slug)
     images = list(Path(image_directory).glob("*"))
     for image_path in tqdm(images):
         image_response = _create_image(dataset, batch["slug"], image_path)
         _upload_image(image_response["presigned_post"], image_path)
         _complete_image(image_response["id"])
     return _complete_batch(batch["slug"])
```

