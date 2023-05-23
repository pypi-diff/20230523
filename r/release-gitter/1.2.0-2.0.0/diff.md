# Comparing `tmp/release-gitter-1.2.0.tar.gz` & `tmp/release-gitter-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "release-gitter-1.2.0.tar", last modified: Tue Oct 11 19:54:52 2022, max compression
+gzip compressed data, was "release-gitter-2.0.0.tar", last modified: Tue May 23 00:27:11 2023, max compression
```

## Comparing `release-gitter-1.2.0.tar` & `release-gitter-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 19:54:52.025493 release-gitter-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     1096 2022-10-11 19:54:02.000000 release-gitter-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5045 2022-10-11 19:54:52.025493 release-gitter-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4445 2022-10-11 19:54:02.000000 release-gitter-1.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)     4691 2022-10-11 19:54:02.000000 release-gitter-1.2.0/pseudo_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-11 19:54:52.015493 release-gitter-1.2.0/release_gitter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5045 2022-10-11 19:54:51.000000 release-gitter-1.2.0/release_gitter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      292 2022-10-11 19:54:51.000000 release-gitter-1.2.0/release_gitter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-11 19:54:51.000000 release-gitter-1.2.0/release_gitter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2022-10-11 19:54:51.000000 release-gitter-1.2.0/release_gitter.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-10-11 19:54:51.000000 release-gitter-1.2.0/release_gitter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-10-11 19:54:51.000000 release-gitter-1.2.0/release_gitter.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)    17927 2022-10-11 19:54:02.000000 release-gitter-1.2.0/release_gitter.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-10-11 19:54:52.025493 release-gitter-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1204 2022-10-11 19:54:02.000000 release-gitter-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:27:11.423229 release-gitter-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-05-23 00:26:39.000000 release-gitter-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-23 00:27:11.423229 release-gitter-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4445 2023-05-23 00:26:39.000000 release-gitter-2.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-05-23 00:26:39.000000 release-gitter-2.0.0/pseudo_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 00:27:11.423229 release-gitter-2.0.0/release_gitter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5096 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-23 00:27:11.000000 release-gitter-2.0.0/release_gitter.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)    18254 2023-05-23 00:26:39.000000 release-gitter-2.0.0/release_gitter.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 00:27:11.423229 release-gitter-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-05-23 00:26:39.000000 release-gitter-2.0.0/setup.py
```

### Comparing `release-gitter-1.2.0/LICENSE` & `release-gitter-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `release-gitter-1.2.0/PKG-INFO` & `release-gitter-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: release-gitter
-Version: 1.2.0
-Summary: Easily download releases from sites like Github and Gitea
-Home-page: https://git.iamthefij.com/iamthefij/release-gitter.git
-Download-URL: https://git.iamthefij.com/iamthefij/release-gitter.git/archive/master.tar.gz
-Author: iamthefij
-Author-email: 
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: builder
-License-File: LICENSE
-
 # release-gitter
 
 Easily download releases from sites like Github and Gitea
 
 ## Original repo
 
 Originally hosted at https://git.iamthefij.com/iamthefij/release-gitter.git
```

### Comparing `release-gitter-1.2.0/README.md` & `release-gitter-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: release-gitter
+Version: 2.0.0
+Summary: Easily download releases from sites like Github and Gitea
+Home-page: https://git.iamthefij.com/iamthefij/release-gitter.git
+Download-URL: https://git.iamthefij.com/iamthefij/release-gitter.git/archive/master.tar.gz
+Author: iamthefij
+Author-email: 
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+Provides-Extra: builder
+License-File: LICENSE
+
 # release-gitter
 
 Easily download releases from sites like Github and Gitea
 
 ## Original repo
 
 Originally hosted at https://git.iamthefij.com/iamthefij/release-gitter.git
```

### Comparing `release-gitter-1.2.0/pseudo_builder.py` & `release-gitter-2.0.0/pseudo_builder.py`

 * *Files identical despite different names*

### Comparing `release-gitter-1.2.0/release_gitter.egg-info/PKG-INFO` & `release-gitter-2.0.0/release_gitter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: release-gitter
-Version: 1.2.0
+Version: 2.0.0
 Summary: Easily download releases from sites like Github and Gitea
 Home-page: https://git.iamthefij.com/iamthefij/release-gitter.git
 Download-URL: https://git.iamthefij.com/iamthefij/release-gitter.git/archive/master.tar.gz
 Author: iamthefij
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: builder
 License-File: LICENSE
 
 # release-gitter
 
 Easily download releases from sites like Github and Gitea
```

### Comparing `release-gitter-1.2.0/release_gitter.py` & `release-gitter-2.0.0/release_gitter.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,25 +9,20 @@
 from mimetypes import guess_type
 from pathlib import Path
 from subprocess import check_call
 from subprocess import check_output
 from tarfile import TarFile
 from tarfile import TarInfo
 from typing import Any
-from typing import Optional
-from typing import Union
 from urllib.parse import urlparse
 from zipfile import ZipFile
 
 import requests
 
 
-# Extract metadata from repo
-
-
 class UnsupportedContentTypeError(ValueError):
     pass
 
 
 class InvalidRemoteError(ValueError):
     pass
 
@@ -48,14 +43,16 @@
     except AttributeError:
         # Py < 3.9
         return s[: -len(suf)] if s and s.endswith(suf) else s
 
 
 @dataclass
 class GitRemoteInfo:
+    """Extracts information about a repository"""
+
     hostname: str
     owner: str
     repo: str
 
     def get_releases_url(self):
         """Gets API url for releases based on hostname and repo info
 
@@ -85,15 +82,15 @@
             )
 
         raise InvalidRemoteError(
             f"Could not find a valid API on host {self.hostname}. Only Github and Gitea APIs are supported"
         )
 
 
-def parse_git_remote(git_url: Optional[str] = None) -> GitRemoteInfo:
+def parse_git_remote(git_url: str | None = None) -> GitRemoteInfo:
     """Extract Github repo info from a git remote url"""
     if not git_url:
         git_url = (
             check_output(["git", "remote", "get-url", "origin"]).decode("UTF-8").strip()
         )
 
     # Normalize Github ssh url as a proper URL
@@ -124,26 +121,26 @@
         for line in f:
             if line.startswith("version"):
                 return line.partition(" = ")[2].strip()[1:-1]
 
     raise ValueError(f"No version found in {p}")
 
 
-def read_git_tag(fetch: bool = True) -> Optional[str]:
+def read_git_tag(fetch: bool = True) -> str | None:
     """Get local git tag for current repo
 
     fetch: optionally fetch tags with depth of 1 from remote"""
     if fetch:
         check_call(["git", "fetch", "--tags", "--depth", "1"])
 
     git_tag = check_output(["git", "describe", "--tags"]).decode("UTF-8").strip()
     return git_tag or None
 
 
-def read_version(from_tags: bool = False, fetch: bool = False) -> Optional[str]:
+def read_version(from_tags: bool = False, fetch: bool = False) -> str | None:
     """Read version information from file or from git"""
     if from_tags:
         return read_git_tag(fetch)
 
     matchers = {
         "Cargo.toml": parse_cargo_version,
     }
@@ -154,21 +151,18 @@
             return extractor(p)
 
     # TODO: Log this out to stderr
     # raise ValueError(f"Unknown project type. Didn't find any of {matchers.keys()}")
     return None
 
 
-# Fetch release and assets from Github
-
-
 def fetch_release(
     remote: GitRemoteInfo,
-    version: Optional[str] = None
-    # TODO: Accept an argument for pre-release
+    version: str | None = None,
+    pre_release=False,
 ) -> dict[Any, Any]:
     """Fetches a release object from a Github repo
 
     If a version number is provided, that version will be retrieved. Otherwise, the latest
     will be returned.
     """
     result = requests.get(
@@ -176,30 +170,37 @@
         # headers={"Accept": "application/vnd.github.v3+json"},
         headers={"Accept": "application/json"},
     )
     result.raise_for_status()
 
     # Return the latest if requested
     if version is None or version == "latest":
-        return result.json()[0]
+        for release in result.json():
+            if release["prerelease"] and not pre_release:
+                continue
+
+            return release
 
     # Return matching version
     for release in result.json():
         if release["tag_name"].endswith(version):
             return release
 
-    raise ValueError(f"Could not find release version ending in {version}")
+    raise ValueError(
+        f"Could not find release version ending in {version}."
+        f"{ ' Is it a pre-release?' if not pre_release else ''}"
+    )
 
 
 def match_asset(
     release: dict[Any, Any],
     format: str,
-    version: Optional[str] = None,
-    system_mapping: Optional[dict[str, str]] = None,
-    arch_mapping: Optional[dict[str, str]] = None,
+    version: str | None = None,
+    system_mapping: dict[str, str] | None = None,
+    arch_mapping: dict[str, str] | None = None,
 ) -> dict[Any, Any]:
     """Accepts a release and searches for an appropriate asset attached using
     a provided template and some alternative mappings for version, system, and machine info
 
     Args
         `release`: A dict release value from the Github API
         `format`: is a python format string allowing for "{version}", "{system}", and "{arch}"
@@ -269,15 +270,15 @@
     )
 
 
 class PackageAdapter:
     """Adapts the names and extractall methods from ZipFile and TarFile classes"""
 
     def __init__(self, content_type: str, response: requests.Response):
-        self._package: Union[TarFile, ZipFile]
+        self._package: TarFile | ZipFile
         if content_type in (
             "application/zip",
             "application/x-zip-compressed",
         ):
             self._package = ZipFile(BytesIO(response.content))
         elif content_type == "application/x-tar":
             self._package = TarFile(fileobj=response.raw)
@@ -302,16 +303,16 @@
 
         raise ValueError(
             f"Unknown package type, cannot extract from {type(self._package)}"
         )
 
     def extractall(
         self,
-        path: Optional[Path],
-        members: Optional[list[str]],
+        path: Path | None,
+        members: list[str] | None,
     ) -> list[str]:
         """Extract all or a subset of files from the package
 
         If the `file_names` list is empty, all files will be extracted"""
         if path is None:
             path = Path.cwd()
         if not members:
@@ -347,16 +348,16 @@
         raise UnsupportedContentTypeError(
             "Cannot extract files from archive because we don't recognize the content type"
         )
 
 
 def download_asset(
     asset: dict[Any, Any],
-    extract_files: Optional[list[str]] = None,
-    destination: Optional[Path] = None,
+    extract_files: list[str] | None = None,
+    destination: Path | None = None,
 ) -> list[Path]:
     """Download asset from entity passed in
 
     Extracts files from archives if provided. Any empty list will extract all files
 
     Args
         `asset`: asset dictionary as returned from API
@@ -384,16 +385,16 @@
 
 
 class MapAddAction(argparse.Action):
     def __call__(
         self,
         _: argparse.ArgumentParser,
         namespace: argparse.Namespace,
-        values: Union[str, Sequence[Any], None],
-        option_string: Optional[str] = None,
+        values: str | Sequence[Any] | None,
+        option_string: str | None = None,
     ):
         # Validate that required value has something
         if self.required and not values:
             raise argparse.ArgumentError(
                 self, f"Did not provide required argument {option_string}"
             )
 
@@ -415,15 +416,15 @@
                 parts = value.partition("=")
                 dest[parts[0]] = parts[2]
 
         # Set dest value
         setattr(namespace, self.dest, dest)
 
 
-def _parse_args(args: Optional[list[str]] = None) -> argparse.Namespace:
+def _parse_args(args: list[str] | None = None) -> argparse.Namespace:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "format",
         help="Format template to match assets. Eg. `foo-{version}-{system}-{arch}.zip`",
     )
     parser.add_argument(
         "destination",
@@ -450,14 +451,19 @@
         help="Git repository URL. Overrides `git remote` detection, but not command line options for hostname, owner, and repo",
     )
     parser.add_argument(
         "--version",
         help="Release version to download. If not provied, it will look for project metadata",
     )
     parser.add_argument(
+        "--prerelease",
+        action="store_true",
+        help="Include pre-release versions in search",
+    )
+    parser.add_argument(
         "--version-git-tag",
         "-t",
         action="store_true",
         help="Get the release version from a git tag",
     )
     parser.add_argument(
         "--version-git-no-fetch",
@@ -525,21 +531,26 @@
     return parsed_args
 
 
 def download_release(
     remote_info: GitRemoteInfo,
     destination: Path,
     format: str,
-    version: Optional[str] = None,
-    system_mapping: Optional[dict[str, str]] = None,
-    arch_mapping: Optional[dict[str, str]] = None,
-    extract_files: Optional[list[str]] = None,
+    version: str | None = None,
+    system_mapping: dict[str, str] | None = None,
+    arch_mapping: dict[str, str] | None = None,
+    extract_files: list[str] | None = None,
+    pre_release=False,
 ) -> list[Path]:
     """Convenience method for fetching, downloading and extracting a release"""
-    release = fetch_release(remote_info)
+    release = fetch_release(
+        remote_info,
+        version=version,
+        pre_release=pre_release,
+    )
     asset = match_asset(
         release,
         format,
         version=version,
         system_mapping=system_mapping,
         arch_mapping=arch_mapping,
     )
@@ -552,15 +563,17 @@
     return files
 
 
 def main():
     args = _parse_args()
 
     release = fetch_release(
-        GitRemoteInfo(args.hostname, args.owner, args.repo), args.version
+        GitRemoteInfo(args.hostname, args.owner, args.repo),
+        version=args.version,
+        pre_release=args.prerelease,
     )
     asset = match_asset(
         release,
         args.format,
         version=args.version,
         system_mapping=args.map_system,
         arch_mapping=args.map_arch,
```

### Comparing `release-gitter-1.2.0/setup.py` & `release-gitter-2.0.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="release-gitter",
-    version="1.2.0",
+    version="2.0.0",
     description="Easily download releases from sites like Github and Gitea",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.iamthefij.com/iamthefij/release-gitter.git",
     download_url=(
         "https://git.iamthefij.com/iamthefij/release-gitter.git/archive/master.tar.gz"
     ),
     author="iamthefij",
     author_email="",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     keywords="",
     py_modules=["release_gitter", "pseudo_builder"],
     install_requires=["requests"],
     extras_require={"builder": ["toml", "wheel"]},
     entry_points={
         "console_scripts": [
```

