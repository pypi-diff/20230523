# Comparing `tmp/lnschema_lamin1-0.16.2.tar.gz` & `tmp/lnschema_lamin1-0.16.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lnschema_lamin1-0.16.2.tar", last modified: Mon May 15 15:03:10 2023, max compression
+gzip compressed data, was "lnschema_lamin1-0.16.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lnschema_lamin1-0.16.2.tar` & `lnschema_lamin1-0.16.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     3577 2023-05-08 08:17:58.718695 lnschema_lamin1-0.16.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-08 08:17:58.718802 lnschema_lamin1-0.16.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-08 08:17:58.718895 lnschema_lamin1-0.16.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1416 2023-05-08 08:17:58.718998 lnschema_lamin1-0.16.2/.gitignore
--rw-r--r--   0        0        0     1795 2023-05-08 08:17:58.719108 lnschema_lamin1-0.16.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      145 2023-05-08 08:17:58.719211 lnschema_lamin1-0.16.2/README.md
--rw-r--r--   0        0        0      740 2023-05-15 15:02:40.305835 lnschema_lamin1-0.16.2/docs/changelog.md
--rw-r--r--   0        0        0     5015 2023-05-08 08:17:58.719651 lnschema_lamin1-0.16.2/docs/guide/01-get-started.ipynb
--rw-r--r--   0        0        0     2190 2023-05-08 08:17:58.719754 lnschema_lamin1-0.16.2/docs/guide/02-orms.ipynb
--rw-r--r--   0        0        0     5397 2023-05-15 14:35:07.531917 lnschema_lamin1-0.16.2/docs/guide/10-migrate.ipynb
--rw-r--r--   0        0        0       65 2023-05-08 08:17:58.719916 lnschema_lamin1-0.16.2/docs/guide/index.md
--rw-r--r--   0        0        0      122 2023-05-08 08:17:58.719983 lnschema_lamin1-0.16.2/docs/index.md
--rw-r--r--   0        0        0       63 2023-05-08 08:17:58.720072 lnschema_lamin1-0.16.2/docs/reference.md
--rw-r--r--   0        0        0      163 2023-05-08 08:17:58.720149 lnschema_lamin1-0.16.2/lamin-project.yaml
--rw-r--r--   0        0        0      641 2023-05-15 15:02:23.794592 lnschema_lamin1-0.16.2/lnschema_lamin1/__init__.py
--rw-r--r--   0        0        0     3800 2023-05-15 15:00:39.484732 lnschema_lamin1-0.16.2/lnschema_lamin1/_core.py
--rw-r--r--   0        0        0     2406 2023-05-15 13:03:26.641667 lnschema_lamin1-0.16.2/lnschema_lamin1/_link.py
--rw-r--r--   0        0        0      259 2023-05-15 13:03:26.641873 lnschema_lamin1-0.16.2/lnschema_lamin1/dev/__init__.py
--rw-r--r--   0        0        0      119 2023-05-08 08:17:58.720546 lnschema_lamin1-0.16.2/lnschema_lamin1/dev/_id.py
--rw-r--r--   0        0        0      346 2023-05-15 13:03:26.642051 lnschema_lamin1-0.16.2/lnschema_lamin1/dev/_type.py
--rw-r--r--   0        0        0     1145 2023-05-08 08:17:58.720606 lnschema_lamin1-0.16.2/lnschema_lamin1/dev/_versions.py
--rw-r--r--   0        0        0       31 2023-05-08 08:17:58.720661 lnschema_lamin1-0.16.2/lnschema_lamin1/dev/id.py
--rw-r--r--   0        0        0      156 2023-05-15 13:03:26.642233 lnschema_lamin1-0.16.2/lnschema_lamin1/dev/type.py
--rw-r--r--   0        0        0      366 2023-05-15 13:03:26.642393 lnschema_lamin1-0.16.2/lnschema_lamin1/link.py
--rw-r--r--   0        0        0     1063 2023-05-08 08:17:58.720890 lnschema_lamin1-0.16.2/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
--rw-r--r--   0        0        0     4097 2023-05-15 15:02:57.367902 lnschema_lamin1-0.16.2/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py
--rw-r--r--   0        0        0      776 2023-05-08 08:17:58.720978 lnschema_lamin1-0.16.2/noxfile.py
--rw-r--r--   0        0        0      655 2023-05-15 09:56:43.981463 lnschema_lamin1-0.16.2/pyproject.toml
--rw-r--r--   0        0        0      811 2023-05-08 08:17:58.721159 lnschema_lamin1-0.16.2/tests/test_migrations.py
--rw-r--r--   0        0        0      481 2023-05-08 08:17:58.721222 lnschema_lamin1-0.16.2/tests/test_notebooks.py
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 lnschema_lamin1-0.16.2/PKG-INFO
+-rw-r--r--   0        0        0     3577 2023-05-08 08:17:58.718695 lnschema_lamin1-0.16.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-08 08:17:58.718802 lnschema_lamin1-0.16.3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-08 08:17:58.718895 lnschema_lamin1-0.16.3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1416 2023-05-08 08:17:58.718998 lnschema_lamin1-0.16.3/.gitignore
+-rw-r--r--   0        0        0     1795 2023-05-08 08:17:58.719108 lnschema_lamin1-0.16.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      154 2023-05-15 15:05:43.656555 lnschema_lamin1-0.16.3/README.md
+-rw-r--r--   0        0        0      904 2023-05-23 10:11:29.066166 lnschema_lamin1-0.16.3/docs/changelog.md
+-rw-r--r--   0        0        0     5015 2023-05-08 08:17:58.719651 lnschema_lamin1-0.16.3/docs/guide/01-get-started.ipynb
+-rw-r--r--   0        0        0     2190 2023-05-08 08:17:58.719754 lnschema_lamin1-0.16.3/docs/guide/02-orms.ipynb
+-rw-r--r--   0        0        0     5397 2023-05-15 14:35:07.531917 lnschema_lamin1-0.16.3/docs/guide/10-migrate.ipynb
+-rw-r--r--   0        0        0       65 2023-05-08 08:17:58.719916 lnschema_lamin1-0.16.3/docs/guide/index.md
+-rw-r--r--   0        0        0      122 2023-05-08 08:17:58.719983 lnschema_lamin1-0.16.3/docs/index.md
+-rw-r--r--   0        0        0       63 2023-05-08 08:17:58.720072 lnschema_lamin1-0.16.3/docs/reference.md
+-rw-r--r--   0        0        0      163 2023-05-08 08:17:58.720149 lnschema_lamin1-0.16.3/lamin-project.yaml
+-rw-r--r--   0        0        0      641 2023-05-23 10:10:40.628983 lnschema_lamin1-0.16.3/lnschema_lamin1/__init__.py
+-rw-r--r--   0        0        0     4300 2023-05-23 10:09:49.269416 lnschema_lamin1-0.16.3/lnschema_lamin1/_core.py
+-rw-r--r--   0        0        0     3232 2023-05-23 10:09:49.269675 lnschema_lamin1-0.16.3/lnschema_lamin1/_link.py
+-rw-r--r--   0        0        0      259 2023-05-15 13:03:26.641873 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/__init__.py
+-rw-r--r--   0        0        0      119 2023-05-08 08:17:58.720546 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/_id.py
+-rw-r--r--   0        0        0      346 2023-05-15 13:03:26.642051 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/_type.py
+-rw-r--r--   0        0        0     1145 2023-05-08 08:17:58.720606 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/_versions.py
+-rw-r--r--   0        0        0       31 2023-05-08 08:17:58.720661 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/id.py
+-rw-r--r--   0        0        0      156 2023-05-15 13:03:26.642233 lnschema_lamin1-0.16.3/lnschema_lamin1/dev/type.py
+-rw-r--r--   0        0        0      426 2023-05-23 10:09:49.269914 lnschema_lamin1-0.16.3/lnschema_lamin1/link.py
+-rw-r--r--   0        0        0     1063 2023-05-08 08:17:58.720890 lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py
+-rw-r--r--   0        0        0     4097 2023-05-15 15:02:57.367902 lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py
+-rw-r--r--   0        0        0     2251 2023-05-23 10:12:25.006468 lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-05-23-f9f58cf3ab38-v0_16_3.py
+-rw-r--r--   0        0        0      776 2023-05-08 08:17:58.720978 lnschema_lamin1-0.16.3/noxfile.py
+-rw-r--r--   0        0        0      655 2023-05-15 09:56:43.981463 lnschema_lamin1-0.16.3/pyproject.toml
+-rw-r--r--   0        0        0      811 2023-05-08 08:17:58.721159 lnschema_lamin1-0.16.3/tests/test_migrations.py
+-rw-r--r--   0        0        0      481 2023-05-08 08:17:58.721222 lnschema_lamin1-0.16.3/tests/test_notebooks.py
+-rw-r--r--   0        0        0      716 1970-01-01 00:00:00.000000 lnschema_lamin1-0.16.3/PKG-INFO
```

### Comparing `lnschema_lamin1-0.16.2/.github/workflows/build.yml` & `lnschema_lamin1-0.16.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/.github/workflows/latest-changes.yml` & `lnschema_lamin1-0.16.3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/.gitignore` & `lnschema_lamin1-0.16.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/.pre-commit-config.yaml` & `lnschema_lamin1-0.16.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/docs/changelog.md` & `lnschema_lamin1-0.16.3/docs/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🎨 Add `Well` table, File.cell_lines | [8](https://github.com/laminlabs/lnschema-lamin1/pull/8) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-23 | 0.16.3
 💚 Removed treatment relationships | [4](https://github.com/laminlabs/lnschema-lamin1/pull/4) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 | 0.16.2
 ✨ Added `Treatment` table | [3](https://github.com/laminlabs/lnschema-lamin1/pull/3) | [sunnyosun](https://github.com/sunnyosun) | 2023-05-15 |
 🚚 Link `CellType` to `File` | [2](https://github.com/laminlabs/lnschema-lamin1/pull/2) | [falexwolf](https://github.com/falexwolf) | 2023-04-24 | 0.16.1
 🎉 Move content from `lnschema-wetlab` here | [1](https://github.com/laminlabs/lnschema-lamin1/pull/1) | [falexwolf](https://github.com/falexwolf) | 2023-04-22 | 0.15.1
```

### Comparing `lnschema_lamin1-0.16.2/docs/guide/01-get-started.ipynb` & `lnschema_lamin1-0.16.3/docs/guide/01-get-started.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/docs/guide/02-orms.ipynb` & `lnschema_lamin1-0.16.3/docs/guide/02-orms.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/docs/guide/10-migrate.ipynb` & `lnschema_lamin1-0.16.3/docs/guide/10-migrate.ipynb`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/lnschema_lamin1/__init__.py` & `lnschema_lamin1-0.16.3/lnschema_lamin1/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,16 +23,16 @@
    dev
    link
 
 """
 
 _schema_id = "tvhn"
 _name = "lamin1"
-_migration = "a0867fc8d6e5"
-__version__ = "0.16.2"
+_migration = "f9f58cf3ab38"
+__version__ = "0.16.3"
 
 # prints warning of python versions
 from lamin_logger import py_version_warning
 
 py_version_warning("3.8", "3.10")
```

### Comparing `lnschema_lamin1-0.16.2/lnschema_lamin1/_core.py` & `lnschema_lamin1-0.16.3/lnschema_lamin1/_core.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,33 +3,35 @@
 from lnbase_biolab import (
     BiosampleBase,
     ExperimentBase,
     ExperimentTypeBase,
     TechsampleBase,
     TreatmentBase,
 )
-from lnschema_bionty import CellType, Disease, Species, Tissue
+from lnschema_bionty import CellLine, CellType, Disease, Species, Tissue
 from lnschema_core import File
 from lnschema_core.dev.sqlmodel import add_relationship_keys, schema_sqlmodel
 from sqlalchemy.orm import relationship
 from sqlmodel import Field, Relationship
 
 from lnschema_lamin1.dev import type as tp
 
 from . import _name as schema_name
 from .link import (
     BiosampleTechsample,
     BiosampleTreatment,
     FileBiosample,
+    FileCellLine,
     FileCellType,
     FileExperiment,
     FileTreatment,
+    FileWell,
 )
 
-_, prefix, schema_arg = schema_sqlmodel(schema_name)
+SQLModel, prefix, schema_arg = schema_sqlmodel(schema_name)
 
 
 class Experiment(ExperimentBase, table=True):  # type: ignore
     """Experiments."""
 
     experiment_type_id: str = Field(default=None, foreign_key="lamin1.experiment_type.id", index=True)
     files: File = Relationship(
@@ -64,14 +66,29 @@
         sa_relationship_kwargs=dict(secondary=FileBiosample.__table__),
     )
 
 
 File.biosamples = relationship(Biosample, back_populates="files", secondary=FileBiosample.__table__)
 
 
+class Well(SQLModel, table=True):  # type: ignore
+    """Wells in a experimental plate."""
+
+    row: str = Field(primary_key=True)
+    column: int = Field(primary_key=True)
+
+    files: File = Relationship(
+        back_populates="wells",
+        sa_relationship_kwargs=dict(secondary=FileWell.__table__),
+    )
+
+
+File.wells = relationship(Well, secondary=FileWell.__table__)
+
+
 class Treatment(TreatmentBase, table=True):  # type: ignore
     type: tp.treatment_type = Field(nullable=False, index=True)
     system: tp.treatment_system = Field(default=None, index=True)
     target: Optional[str] = Field(default=None, index=True)
     sequence: Optional[str] = Field(default=None, index=True)
     on_target_score: Optional[float] = Field(default=None, index=True)
     off_target_score: Optional[float] = Field(default=None, index=True)
@@ -81,14 +98,15 @@
         back_populates="treatments",
         sa_relationship_kwargs=dict(secondary=FileTreatment.__table__),
     )
 
 
 File.treatments = relationship(Treatment, back_populates="files", secondary=FileTreatment.__table__)
 File.cell_types = relationship(CellType, secondary=FileCellType.__table__)
+File.cell_line = relationship(CellLine, secondary=FileCellLine.__table__)
 add_relationship_keys(File)
 
 
 class Techsample(TechsampleBase, table=True):  # type: ignore
     biosamples: Biosample = Relationship(
         back_populates="techsamples",
         sa_relationship_kwargs=dict(secondary=BiosampleTechsample.__table__),
```

### Comparing `lnschema_lamin1-0.16.2/lnschema_lamin1/dev/_versions.py` & `lnschema_lamin1-0.16.3/lnschema_lamin1/dev/_versions.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py` & `lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-04-24-652443621d5a-v0_16_0.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py` & `lnschema_lamin1-0.16.3/lnschema_lamin1/migrations/versions/2023-05-15-a0867fc8d6e5-v0_16_2.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/noxfile.py` & `lnschema_lamin1-0.16.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/pyproject.toml` & `lnschema_lamin1-0.16.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/tests/test_migrations.py` & `lnschema_lamin1-0.16.3/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `lnschema_lamin1-0.16.2/PKG-INFO` & `lnschema_lamin1-0.16.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: lnschema_lamin1
-Version: 0.16.2
+Version: 0.16.3
 Summary: Lamin's `lamin1` lab schema (`tvhn`).
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamindb[bionty,biolab]
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: nbproject_test>=0.4.1 ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lnschema-lamin1
 Provides-Extra: dev
 Provides-Extra: test
 
-# lnschema-lamin1: Customized schema of Lamin
+# lnschema-lamin1: Customized schema of Lamin (`tvhn`)
 
 Latest developer docs: [netlify](https://lnschema-lamin1-tvhn.netlify.app/docs/lnschema-lamin1/).
```

