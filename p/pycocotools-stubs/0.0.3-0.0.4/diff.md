# Comparing `tmp/pycocotools_stubs-0.0.3.tar.gz` & `tmp/pycocotools_stubs-0.0.4.tar.gz`

## Comparing `pycocotools_stubs-0.0.3.tar` & `pycocotools_stubs-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/requirements/README.md
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/requirements/requirements-build.txt
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/requirements/requirements-dev.txt
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/requirements/requirements.txt
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/src/pycocotools-stubs/__init__.pyi
--rw-r--r--   0        0        0     5222 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/src/pycocotools-stubs/coco.pyi
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/src/pycocotools-stubs/coco_types.pyi
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/src/pycocotools-stubs/cocoeval.pyi
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/src/pycocotools-stubs/mask.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/src/pycocotools-stubs/py.typed
--rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/LICENSE
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/README.md
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/requirements/README.md
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/requirements/requirements-build.txt
+-rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/requirements/requirements-dev.txt
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/requirements/requirements.txt
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/__init__.pyi
+-rw-r--r--   0        0        0     5215 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/coco.pyi
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/coco_types.pyi
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/cocoeval.pyi
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/mask.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/src/pycocotools-stubs/py.typed
+-rwxr-xr-x   0        0        0      342 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/README.md
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 pycocotools_stubs-0.0.4/PKG-INFO
```

### Comparing `pycocotools_stubs-0.0.3/.pre-commit-config.yaml` & `pycocotools_stubs-0.0.4/.pre-commit-config.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -3,29 +3,29 @@
   autofix_commit_msg: "ci: [pre-commit.ci] auto fixes [...]"
   autoupdate_commit_msg: "ci: [pre-commit.ci] autoupdate"
   autofix_prs: true
   autoupdate_branch: ''
   submodules: false
 
 default_language_version:
-  python: python3.10
+  python: python3.11
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
       - id: check-docstring-first
       - id: end-of-file-fixer
         exclude: typings
       - id: trailing-whitespace
         exclude: typings
       - id: mixed-line-ending
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.253"
+    rev: "v0.0.265"
     hooks:
       - id: ruff
 
   - repo: https://github.com/RobertCraigie/pyright-python
     rev: v1.1.300
     hooks:
     - id: pyright
```

### Comparing `pycocotools_stubs-0.0.3/requirements/requirements-build.txt` & `pycocotools_stubs-0.0.4/requirements/requirements-build.txt`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.3/requirements/requirements-dev.txt` & `pycocotools_stubs-0.0.4/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.3/requirements/requirements.txt` & `pycocotools_stubs-0.0.4/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.3/src/pycocotools-stubs/coco.pyi` & `pycocotools_stubs-0.0.4/src/pycocotools-stubs/coco.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -12,102 +12,102 @@
     dataset: _Dataset
     anns: dict[int, _AnnotationAny]
     cats: dict[int, _Category]
     imgs: dict[int, _Image]
     imgToAnns: dict[int, list[_AnnotationAny]]
     catToImgs: dict[int, list[int]]
 
-    def __init__(self: Self, annotation_file: str | Path | None = ...) -> None:
+    def __init__(self: Self, annotation_file: str | Path | None = None) -> None:
         """Constructor of Microsoft COCO helper class for reading and visualizing annotations.
 
         Args:
             annotation_file: Location of annotation file
         """
         ...
 
     def createIndex(self: Self) -> None:
         ...
 
     def info(self: Self) -> None:
         """Print information about the annotation file."""
         ...
 
-    def getAnnIds(self: Self, imgIds: Collection[int] | int = ..., catIds: Collection[int] | int = ..., areaRng: Sequence[float] = ..., iscrowd: bool | None = ...) -> list[int]:
+    def getAnnIds(self: Self, imgIds: Collection[int] | int = [], catIds: Collection[int] | int = [], areaRng: Sequence[float] = [], iscrowd: bool | None = None) -> list[int]:
         """Get ann ids that satisfy given filter conditions. default skips that filter.
 
         Args:
             imgIds: Get anns for given imgs.
             catIds: Get anns for given cats.
             areaRng: Get anns for given area range (e.g. [0 inf]).
             iscrowd: Get anns for given crowd label (False or True).
 
         Returns:
             Integer array of ann ids.
         """
         ...
 
-    def getCatIds(self: Self, catNms: Collection[str] | str = ..., supNms: Collection[str] | str = ..., catIds: Sequence[int] | int = ...) -> list[int]:
+    def getCatIds(self: Self, catNms: Collection[str] | str = [], supNms: Collection[str] | str = [], catIds: Sequence[int] | int = []) -> list[int]:
         """Get cat ids that satisfy given filter conditions. default skips that filter.
 
         Args:
             catNms: get cats for given cat names
             supNms get cats for given supercategory names
             catIds: get cats for given cat ids
 
         Returns:
             ids: integer array of cat ids
         """
         ...
 
-    def getImgIds(self: Self, imgIds: Collection[int] | int = ..., catIds: list[int] | int = ...) -> list[int]:
+    def getImgIds(self: Self, imgIds: Collection[int] | int = [], catIds: list[int] | int = []) -> list[int]:
         """Get img ids that satisfy given filter conditions.
 
         Args:
             imgIds: get imgs for given ids
             catIds : get imgs with all given cats
 
         Returns:
             ids: integer array of img ids
         """
         ...
 
-    def loadAnns(self: Self, ids: Collection[int] | int = ...) -> list[_AnnotationAny]:
+    def loadAnns(self: Self, ids: Collection[int] | int = []) -> list[_AnnotationAny]:
         """Load anns with the specified ids.
 
         Args:
             ids: Integer ids specifying anns.
 
         Returns:
             anns: loaded ann objects
         """
         ...
 
-    def loadCats(self: Self, ids: Collection[int] | int = ...) -> list[_Category]:
+    def loadCats(self: Self, ids: Collection[int] | int = []) -> list[_Category]:
         """Load cats with the specified ids.
 
         Args:
             ids: integer ids specifying cats.
 
         Returns:
             cats: loaded cat objects.
         """
         ...
 
-    def loadImgs(self: Self, ids: Collection[int] | int = ...) -> list[_Image]:
+    def loadImgs(self: Self, ids: Collection[int] | int = []) -> list[_Image]:
         """Load anns with the specified ids.
 
         Args:
             ids: integer ids specifying img
 
         Returns:
             imgs: loaded img objects
         """
         ...
 
-    def showAnns(self: Self, anns: Sequence[_AnnotationAny], draw_bbox: bool = ...) -> None:
+    def showAnns(self: Self, anns: Sequence[_AnnotationAny], draw_bbox: bool = False) -> None:
         """Display the specified annotations.
 
         Args:
             anns: Annotations to display.
             draw_bbox: Wether to draw the bounding boxes or not.
         """
         ...
@@ -119,15 +119,15 @@
             resFile: file name of result file
 
         Returns:
             res: result api object
         """
         ...
 
-    def download(self: Self, tarDir: str | None = ..., imgIds: Collection[int] = ...) -> Literal[-1] | None:
+    def download(self: Self, tarDir: str | None = None, imgIds: Collection[int] = []) -> Literal[-1] | None:
         """Download COCO images from mscoco.org server.
 
         Args:
             tarDir: COCO results directory name
             imgIds: images to be downloaded
         """
         ...
```

### Comparing `pycocotools_stubs-0.0.3/src/pycocotools-stubs/coco_types.pyi` & `pycocotools_stubs-0.0.4/src/pycocotools-stubs/coco_types.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 class _Category(TypedDict):
     id: int
     name: str
     supercategory: str
 
 
-class _EvaluationResult(TypedDict):
+class _ImageEvaluationResult(TypedDict):
     image_id: int
     category_id: int
     aRng: list[int]
     maxDet: int
     dtIds: list[int]
     gtIds: list[int]
     dtMatches: npt.NDArray[np.float64]
```

### Comparing `pycocotools_stubs-0.0.3/src/pycocotools-stubs/cocoeval.pyi` & `pycocotools_stubs-0.0.4/src/pycocotools-stubs/cocoeval.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import Literal, TypeAlias
+from typing import Literal, TypeAlias, TypedDict
 
 import numpy as np
 import numpy.typing as npt
 from typing_extensions import Self
 
 from .coco import COCO
-from .coco_types import _EvaluationResult
+from .coco_types import _ImageEvaluationResult
 
 _T_IOU: TypeAlias = Literal["segm", "bbox", "keypoints"]
 
 
 class COCOeval:
     cocoGt: COCO
     cocoDt: COCO
-    evalImgs: list[_EvaluationResult]
+    evalImgs: list[_ImageEvaluationResult]
     eval: _EvaluationResult
     params: Params
     stats: npt.NDArray[np.float64]
     ious: dict[tuple[int, int],  list[float]]
 
-    def __init__(self: Self, cocoGt: COCO | None = ..., cocoDt: COCO | None = ..., iouType: _T_IOU = ...) -> None:
+    def __init__(self: Self, cocoGt: COCO | None = None, cocoDt: COCO | None = None, iouType: _T_IOU = "segm") -> None:
         """Initialize CocoEval using coco APIs for gt and dt
 
         Args:
             cocoGt: coco object with ground truth annotations
             cocoDt: coco object with detection results
         """
         ...
@@ -34,23 +34,23 @@
 
     def computeIoU(self: Self, imgId: int, catId: int) -> list[float]:
         ...
 
     def computeOks(self: Self, imgId: int, catId: int) -> npt.NDArray[np.float64]:
         ...
 
-    def evaluateImg(self: Self, imgId: int, catId: int, aRng: list[int], maxDet: int) -> _EvaluationResult:
+    def evaluateImg(self: Self, imgId: int, catId: int, aRng: list[int], maxDet: int) -> _ImageEvaluationResult:
         """Perform evaluation for single category and image.
 
         Returns:
             dict (single image results)
         """
         ...
 
-    def accumulate(self: Self, p: Params | None = ...) -> None:
+    def accumulate(self: Self, p: Params | None = None) -> None:
         """Accumulate per image evaluation results and store the result in self.eval
 
         Args:
             p: input params for evaluation
         """
         ...
 
@@ -68,22 +68,31 @@
 class Params:
     """Params for coco evaluation api"""
     imgIds: list[int]
     catIds: list[int]
     iouThrs: npt.NDArray[np.float64]
     recThrs: npt.NDArray[np.float64]
     maxDets: list[int]
-    areaRng: list[int]
+    areaRng: list[float]
     areaRngLbl: list[str]
     useCats: int
     kpt_oks_sigmas: npt.NDArray[np.float64]
     iouType: _T_IOU
     useSegm: int | None
 
-    def __init__(self: Self, iouType: _T_IOU = ...) -> None:
+    def __init__(self: Self, iouType: _T_IOU = "segm") -> None:
         ...
 
     def setDetParams(self: Self) -> None:
         ...
 
     def setKpParams(self: Self) -> None:
         ...
+
+
+class _EvaluationResult(TypedDict):
+    params: Params
+    counts: list[int]
+    date: str
+    precision: npt.NDArray[np.float64]
+    recall: npt.NDArray[np.float64]
+    scores: npt.NDArray[np.float64]
```

### Comparing `pycocotools_stubs-0.0.3/src/pycocotools-stubs/mask.pyi` & `pycocotools_stubs-0.0.4/src/pycocotools-stubs/mask.pyi`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.3/LICENSE` & `pycocotools_stubs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycocotools_stubs-0.0.3/README.md` & `pycocotools_stubs-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/pycocotools-stubs?style=flat)](https://pypi.org/project/pycocotools-stubs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pycocotools-stubs?style=flat)](https://pypi.org/project/pycocotools-stubs)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pycocotools-stubs?style=flat-square)](https://pypistats.org/packages/pycocotools-stubs)
 [![License](https://img.shields.io/pypi/l/pycocotools-stubs?style=flat)](https://opensource.org/licenses/MIT)
 ![Linting](https://github.com/hoel-bagard/pycocotools-stubs/actions/workflows/pre-commit.yaml/badge.svg)
 
 
-Unofficial python stubs for the pycocotools package.
+Unofficial python stubs for the [pycocotools package](https://pypi.org/project/pycocotools/).
 
-An equivalents stubs is available on [typeshed](https://github.com/python/typeshed/tree/main/stubs/pycocotools) (and therefore [pypi](https://pypi.org/project/pycocotools/)).\
+An equivalents stubs is available on [typeshed](https://github.com/python/typeshed/tree/main/stubs/pycocotools).
 This stubs are different on two points:
 - They include the docstrings as they are otherwise not available in the IDE (as far as I know).
 - They include numpy typing (not possible to do in typeshed).
 
 ## Installation
 
-The package is available on pypi [here](https://pypi.org/project/pycocotools-stubs/) you can install it with:
+The package is available on pypi [here](https://pypi.org/project/pycocotools-stubs/), you can install it with:
 
 ```
 pip install pycocotools-stubs
 ```
```

### Comparing `pycocotools_stubs-0.0.3/pyproject.toml` & `pycocotools_stubs-0.0.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -52,32 +52,39 @@
 
 [tool.hatch.envs.pypi.scripts]
 # hatch run pypi:publish_test
 publish_test = "hatch build --clean && hatch publish -r test"
 publish = "hatch build --clean && hatch publish"
 
 [tool.ruff]
-select = ["A", "B", "C4", "E", "I", "Q", "UP", "ANN", "S", "BLE", "COM", "DTZ", "PIE", "PT", "RSE", "SIM","PTH", "TRY", "NPY", "RUF"]
-ignore = ["D1", "D401", "D204", "D203", "D213", "S101", "PLR2004", "A002", "A003"]
+select = ["ALL"]
+# A003 Class attribute `X` is shadowing a python builtin
+# B006: Do not use mutable data structures for argument defaults
+# PYI021: Docstrings should not be included in stubs
+ignore = ["A003", "B006", "D", "FBT", "N", "PYI021"]
 line-length = 10000
 
+[tool.ruff.per-file-ignores]
+"__init__.pyi" = ["F401"]
+
 [tool.ruff.isort]
 order-by-type = false
 
 [tool.ruff.flake8-quotes]
 docstring-quotes = "double"
 
 [tool.pyright]
+pythonVersion = "3.11"
+pythonPlatform = "Linux"
 include = ["src/pycocotools-stubs"]
 ignore = ["src/pycocotools-stubs/__init__.pyi"]
 
 strictListInference = true
 strictDictionaryInference = true
 strictSetInference = true
-
 reportMissingModuleSource = false
 reportMissingImports = true
 reportMissingTypeStubs = false
 reportUnusedImport = true
 reportUnusedClass = "warning"
 reportUnusedFunction = "warning"
 reportUnusedVariable = "warning"
@@ -97,10 +104,7 @@
 reportUnnecessaryCast = "warning"
 reportUnnecessaryComparison = "warning"
 reportImplicitStringConcatenation = false
 reportUnusedCallResult = false
 reportUnusedExpression = "warning"
 reportUnnecessaryTypeIgnoreComment = "warning"
 reportMatchNotExhaustive = "warning"
-
-pythonVersion = "3.10"
-pythonPlatform = "Linux"
```

### Comparing `pycocotools_stubs-0.0.3/PKG-INFO` & `pycocotools_stubs-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycocotools-stubs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unofficial stubs for the pycocotools package.
 Project-URL: Homepage, https://github.com/hoel-bagard/pycocotools-stubs
 Project-URL: Bug Tracker, https://github.com/hoel-bagard/pycocotools-stubs/issues
 Author: Bagard Hoel
 License: MIT
 License-File: LICENSE
 Keywords: pycocotools,stubs
@@ -34,21 +34,21 @@
 [![PyPI - Implementation](https://img.shields.io/pypi/implementation/pycocotools-stubs?style=flat)](https://pypi.org/project/pycocotools-stubs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pycocotools-stubs?style=flat)](https://pypi.org/project/pycocotools-stubs)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/pycocotools-stubs?style=flat-square)](https://pypistats.org/packages/pycocotools-stubs)
 [![License](https://img.shields.io/pypi/l/pycocotools-stubs?style=flat)](https://opensource.org/licenses/MIT)
 ![Linting](https://github.com/hoel-bagard/pycocotools-stubs/actions/workflows/pre-commit.yaml/badge.svg)
 
 
-Unofficial python stubs for the pycocotools package.
+Unofficial python stubs for the [pycocotools package](https://pypi.org/project/pycocotools/).
 
-An equivalents stubs is available on [typeshed](https://github.com/python/typeshed/tree/main/stubs/pycocotools) (and therefore [pypi](https://pypi.org/project/pycocotools/)).\
+An equivalents stubs is available on [typeshed](https://github.com/python/typeshed/tree/main/stubs/pycocotools).
 This stubs are different on two points:
 - They include the docstrings as they are otherwise not available in the IDE (as far as I know).
 - They include numpy typing (not possible to do in typeshed).
 
 ## Installation
 
-The package is available on pypi [here](https://pypi.org/project/pycocotools-stubs/) you can install it with:
+The package is available on pypi [here](https://pypi.org/project/pycocotools-stubs/), you can install it with:
 
 ```
 pip install pycocotools-stubs
 ```
```

