# Comparing `tmp/owlml-0.1.2.dev1684874101.tar.gz` & `tmp/owlml-0.1.2.dev1684875369.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owlml-0.1.2.dev1684874101.tar", last modified: Tue May 23 20:35:12 2023, max compression
+gzip compressed data, was "owlml-0.1.2.dev1684875369.tar", last modified: Tue May 23 20:56:21 2023, max compression
```

## Comparing `owlml-0.1.2.dev1684874101.tar` & `owlml-0.1.2.dev1684875369.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:35:12.970708 owlml-0.1.2.dev1684874101/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 20:35:12.970708 owlml-0.1.2.dev1684874101/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:35:12.966708 owlml-0.1.2.dev1684874101/owlml/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/owlml/images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:35:12.970708 owlml-0.1.2.dev1684874101/owlml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:35:12.000000 owlml-0.1.2.dev1684874101/owlml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 20:35:12.970708 owlml-0.1.2.dev1684874101/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:34:30.000000 owlml-0.1.2.dev1684874101/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:56:21.625930 owlml-0.1.2.dev1684875369/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 20:56:21.625930 owlml-0.1.2.dev1684875369/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:56:21.625930 owlml-0.1.2.dev1684875369/owlml/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/owlml/images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 20:56:21.625930 owlml-0.1.2.dev1684875369/owlml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 20:56:21.000000 owlml-0.1.2.dev1684875369/owlml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-23 20:56:21.625930 owlml-0.1.2.dev1684875369/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 20:55:38.000000 owlml-0.1.2.dev1684875369/setup.py
```

### Comparing `owlml-0.1.2.dev1684874101/LICENSE` & `owlml-0.1.2.dev1684875369/LICENSE`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684874101/README.md` & `owlml-0.1.2.dev1684875369/README.md`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684874101/owlml/__main__.py` & `owlml-0.1.2.dev1684875369/owlml/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Main entry point for OwlML CLI."""
 import fire
 
 from .auth import assign_batch, create_org, create_user, invite_user
-from .datasets import create_dataset, version_dataset
+from .datasets import create_dataset, download_dataset, version_dataset
 from .images import upload_images
 
 
 def main() -> None:
     """Expose CLI commands."""
     fire.Fire(
         {
             "assign-batch": assign_batch,
             "create-dataset": create_dataset,
             "create-org": create_org,
             "create-user": create_user,
+            "download-dataset": download_dataset,
             "invite-user": invite_user,
             "upload-images": upload_images,
             "version-dataset": version_dataset,
         }
     )
```

### Comparing `owlml-0.1.2.dev1684874101/owlml/api.py` & `owlml-0.1.2.dev1684875369/owlml/api.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684874101/owlml/auth.py` & `owlml-0.1.2.dev1684875369/owlml/auth.py`

 * *Files identical despite different names*

### Comparing `owlml-0.1.2.dev1684874101/owlml/images.py` & `owlml-0.1.2.dev1684875369/owlml/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         presigned_post["url"], data=presigned_post["fields"], files=files
     )
     raise_for_status(response)
 
 
 def _complete_image(image_id: str) -> dict[str, Any]:
     """Complete an image."""
-    return OwlMLAPI.post(f"images/{image_id}/complete", dict())
+    return OwlMLAPI.post(f"images/{image_id}/complete")
 
 
 def upload_images(
     dataset: str, image_directory: Union[str, Path], batch_slug: Optional[str] = None
 ) -> dict[str, Any]:
     """Upload images to a dataset."""
     batch = _create_batch(dataset, batch_slug)
```

