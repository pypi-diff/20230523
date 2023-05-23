# Comparing `tmp/pytest-alembic-0.9.0.tar.gz` & `tmp/pytest-alembic-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-alembic-0.9.0.tar", max compression
+gzip compressed data, was "pytest-alembic-0.9.1.tar", max compression
```

## Comparing `pytest-alembic-0.9.0.tar` & `pytest-alembic-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     4003 2022-11-01 16:07:26.492168 pytest-alembic-0.9.0/CHANGELOG.md
--rw-r--r--   0        0        0     1053 2022-09-15 11:48:01.006603 pytest-alembic-0.9.0/LICENSE
--rw-r--r--   0        0        0     5160 2022-09-15 11:48:01.007072 pytest-alembic-0.9.0/README.md
--rw-r--r--   0        0        0     2121 2022-11-01 16:07:28.328029 pytest-alembic-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      263 2022-09-15 11:48:01.060744 pytest-alembic-0.9.0/src/pytest_alembic/__init__.py
--rw-r--r--   0        0        0     5634 2022-09-15 11:48:01.060949 pytest-alembic-0.9.0/src/pytest_alembic/config.py
--rw-r--r--   0        0        0     4382 2022-09-15 11:48:01.061185 pytest-alembic-0.9.0/src/pytest_alembic/executor.py
--rw-r--r--   0        0        0     2885 2022-09-15 11:48:01.061347 pytest-alembic-0.9.0/src/pytest_alembic/history.py
--rw-r--r--   0        0        0      201 2022-11-01 16:07:28.328322 pytest-alembic-0.9.0/src/pytest_alembic/plugin/__init__.py
--rw-r--r--   0        0        0      900 2022-09-15 11:48:01.061982 pytest-alembic-0.9.0/src/pytest_alembic/plugin/error.py
--rw-r--r--   0        0        0     4379 2022-09-15 11:48:01.062177 pytest-alembic-0.9.0/src/pytest_alembic/plugin/fixtures.py
--rw-r--r--   0        0        0     2548 2022-11-01 16:07:28.335098 pytest-alembic-0.9.0/src/pytest_alembic/plugin/hooks.py
--rw-r--r--   0        0        0     6700 2022-11-01 16:07:28.336745 pytest-alembic-0.9.0/src/pytest_alembic/plugin/plugin.py
--rw-r--r--   0        0        0        0 2022-09-15 11:48:01.062689 pytest-alembic-0.9.0/src/pytest_alembic/py.typed
--rw-r--r--   0        0        0     2126 2022-09-15 11:48:01.062870 pytest-alembic-0.9.0/src/pytest_alembic/revision_data.py
--rw-r--r--   0        0        0     9461 2022-11-01 16:07:26.498686 pytest-alembic-0.9.0/src/pytest_alembic/runner.py
--rw-r--r--   0        0        0      302 2022-09-15 11:48:01.063286 pytest-alembic-0.9.0/src/pytest_alembic/tests/__init__.py
--rw-r--r--   0        0        0     5985 2022-11-01 16:07:26.498867 pytest-alembic-0.9.0/src/pytest_alembic/tests/default.py
--rw-r--r--   0        0        0      333 2022-09-15 11:48:01.063760 pytest-alembic-0.9.0/src/pytest_alembic/tests/experimental/__init__.py
--rw-r--r--   0        0        0     9007 2022-09-15 11:48:01.063989 pytest-alembic-0.9.0/src/pytest_alembic/tests/experimental/all_models_register_on_metadata.py
--rw-r--r--   0        0        0     3906 2022-09-15 11:48:01.064171 pytest-alembic-0.9.0/src/pytest_alembic/tests/experimental/collect_clean_alembic_environment.py
--rw-r--r--   0        0        0     6598 2022-09-15 11:48:01.064368 pytest-alembic-0.9.0/src/pytest_alembic/tests/experimental/downgrade_leaves_no_trace.py
--rw-r--r--   0        0        0     6264 1970-01-01 00:00:00.000000 pytest-alembic-0.9.0/setup.py
--rw-r--r--   0        0        0     6050 1970-01-01 00:00:00.000000 pytest-alembic-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     7604 2022-11-01 16:47:28.720654 pytest-alembic-0.9.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1053 2022-09-15 11:48:01.006603 pytest-alembic-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5160 2022-09-15 11:48:01.007072 pytest-alembic-0.9.1/README.md
+-rw-r--r--   0        0        0     2121 2022-11-01 16:47:28.729489 pytest-alembic-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      263 2022-09-15 11:48:01.060744 pytest-alembic-0.9.1/src/pytest_alembic/__init__.py
+-rw-r--r--   0        0        0     5634 2022-09-15 11:48:01.060949 pytest-alembic-0.9.1/src/pytest_alembic/config.py
+-rw-r--r--   0        0        0     4382 2022-09-15 11:48:01.061185 pytest-alembic-0.9.1/src/pytest_alembic/executor.py
+-rw-r--r--   0        0        0     2885 2022-09-15 11:48:01.061347 pytest-alembic-0.9.1/src/pytest_alembic/history.py
+-rw-r--r--   0        0        0      201 2022-11-01 16:07:28.328322 pytest-alembic-0.9.1/src/pytest_alembic/plugin/__init__.py
+-rw-r--r--   0        0        0      900 2022-09-15 11:48:01.061982 pytest-alembic-0.9.1/src/pytest_alembic/plugin/error.py
+-rw-r--r--   0        0        0     4379 2022-09-15 11:48:01.062177 pytest-alembic-0.9.1/src/pytest_alembic/plugin/fixtures.py
+-rw-r--r--   0        0        0     2548 2022-11-01 16:07:28.335098 pytest-alembic-0.9.1/src/pytest_alembic/plugin/hooks.py
+-rw-r--r--   0        0        0     6700 2022-11-01 16:07:28.336745 pytest-alembic-0.9.1/src/pytest_alembic/plugin/plugin.py
+-rw-r--r--   0        0        0        0 2022-09-15 11:48:01.062689 pytest-alembic-0.9.1/src/pytest_alembic/py.typed
+-rw-r--r--   0        0        0     2126 2022-09-15 11:48:01.062870 pytest-alembic-0.9.1/src/pytest_alembic/revision_data.py
+-rw-r--r--   0        0        0    10514 2022-11-01 16:47:28.729939 pytest-alembic-0.9.1/src/pytest_alembic/runner.py
+-rw-r--r--   0        0        0      302 2022-09-15 11:48:01.063286 pytest-alembic-0.9.1/src/pytest_alembic/tests/__init__.py
+-rw-r--r--   0        0        0     6023 2022-11-01 16:47:28.730319 pytest-alembic-0.9.1/src/pytest_alembic/tests/default.py
+-rw-r--r--   0        0        0      333 2022-09-15 11:48:01.063760 pytest-alembic-0.9.1/src/pytest_alembic/tests/experimental/__init__.py
+-rw-r--r--   0        0        0     9007 2022-09-15 11:48:01.063989 pytest-alembic-0.9.1/src/pytest_alembic/tests/experimental/all_models_register_on_metadata.py
+-rw-r--r--   0        0        0     3906 2022-09-15 11:48:01.064171 pytest-alembic-0.9.1/src/pytest_alembic/tests/experimental/collect_clean_alembic_environment.py
+-rw-r--r--   0        0        0     6598 2022-09-15 11:48:01.064368 pytest-alembic-0.9.1/src/pytest_alembic/tests/experimental/downgrade_leaves_no_trace.py
+-rw-r--r--   0        0        0     6264 1970-01-01 00:00:00.000000 pytest-alembic-0.9.1/setup.py
+-rw-r--r--   0        0        0     6050 1970-01-01 00:00:00.000000 pytest-alembic-0.9.1/PKG-INFO
```

### Comparing `pytest-alembic-0.9.0/LICENSE` & `pytest-alembic-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/README.md` & `pytest-alembic-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/pyproject.toml` & `pytest-alembic-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-alembic"
-version = "0.9.0"
+version = "0.9.1"
 description = "A pytest plugin for verifying alembic migrations."
 authors = [
     "Dan Cardin <ddcardin@gmail.com>",
 ]
 license = "MIT"
 keywords = [ "pytest", "sqlalchemy", "alembic", "migration", "revision" ]
 classifiers = [ "Framework :: Pytest" ]
```

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/config.py` & `pytest-alembic-0.9.1/src/pytest_alembic/config.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/executor.py` & `pytest-alembic-0.9.1/src/pytest_alembic/executor.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/history.py` & `pytest-alembic-0.9.1/src/pytest_alembic/history.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/plugin/error.py` & `pytest-alembic-0.9.1/src/pytest_alembic/plugin/error.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/plugin/fixtures.py` & `pytest-alembic-0.9.1/src/pytest_alembic/plugin/fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/plugin/hooks.py` & `pytest-alembic-0.9.1/src/pytest_alembic/plugin/hooks.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/plugin/plugin.py` & `pytest-alembic-0.9.1/src/pytest_alembic/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/revision_data.py` & `pytest-alembic-0.9.1/src/pytest_alembic/revision_data.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/runner.py` & `pytest-alembic-0.9.1/src/pytest_alembic/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import contextlib
 import functools
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Union
 
 import alembic.command
 import alembic.migration
+from alembic.script.revision import RevisionMap
 from sqlalchemy.engine import Engine
 
 from pytest_alembic.config import Config
 from pytest_alembic.executor import CommandExecutor, ConnectionExecutor
 from pytest_alembic.history import AlembicHistory
 from pytest_alembic.revision_data import RevisionData
 
@@ -32,35 +33,34 @@
 @dataclass
 class MigrationContext:
     """Within a given environment/execution context, executes alembic commands."""
 
     command_executor: CommandExecutor
     revision_data: RevisionData
     connection_executor: ConnectionExecutor
-    config: Config
     history: AlembicHistory
+    config: Config
     connection: Engine = None
 
     @classmethod
     def from_config(
         cls,
         config: Config,
         command_executor: CommandExecutor,
         connection_executor: ConnectionExecutor,
         connection: Engine,
     ):
-        raw_history = command_executor.script.revision_map
-        history = AlembicHistory.parse(raw_history)
+        history = AlembicHistory.parse(command_executor.script.revision_map)
 
         return cls(
             command_executor=command_executor,
             revision_data=RevisionData.from_config(config),
             connection_executor=connection_executor,
-            config=config,
             history=history,
+            config=config,
             connection=connection,
         )
 
     @property
     def heads(self) -> List[str]:
         """Get the list of revision heads.
 
@@ -80,30 +80,61 @@
             return None
 
         current = run_connection_task(self.connection, get_current)
         if current:
             return current
         return "base"
 
-    def generate_revision(self, process_revision_directives=None, **kwargs):
+    def refresh_history(self) -> AlembicHistory:
+        """Refresh the context's version of the alembic history.
+
+        Note this is not done automatically to avoid the expensive reevaluation
+        step which can make long histories take seconds longer to evaluate for
+        each test.
+        """
+        script = self.command_executor.script
+        script.revision_map = RevisionMap(script._load_revisions)
+        self.history = AlembicHistory.parse(self.command_executor.script.revision_map)
+        return self.history
+
+    def generate_revision(
+        self,
+        process_revision_directives=None,
+        prevent_file_generation=True,
+        autogenerate=False,
+        **kwargs
+    ):
         """Generate a test revision.
 
-        The final act of this process raises a `RevisionSuccess`, which is used as a sentinal
-        to indicate the revision was generated successfully, while not actually finishing the
-        generation of the revision file.
+        If `prevent_file_generation` is `True`, the final act of this process raises a
+        `RevisionSuccess`, which is used as a sentinal to indicate the revision was
+        generated successfully, while not actually finishing the generation of the
+        revision file on disk.
         """
         alembic_config = self.command_executor.alembic_config
         config_directive = alembic_config.attributes["process_revision_directives"]
-        fn = RevisionSuccess.process_revision_directives(
-            _sequence_directives(config_directive, process_revision_directives)
-        )
+
+        directive = _sequence_directives(config_directive, process_revision_directives)
+
+        if prevent_file_generation:
+            directive = RevisionSuccess.process_revision_directives(directive)
+
         try:
-            return self.command_executor.run_command(
-                "revision", process_revision_directives=fn, **kwargs
+            result = self.command_executor.run_command(
+                "revision",
+                process_revision_directives=directive,
+                autogenerate=autogenerate,
+                **kwargs,
             )
+
+            # The history will only have changed if we didn't aritifically prevent it from failing.
+            if not prevent_file_generation:
+                self.refresh_history()
+
+            return result
         except RevisionSuccess:
             pass
 
     def raw_command(self, *args, **kwargs):
         """Execute a raw alembic command."""
         return self.command_executor.run_command(*args, **kwargs)
```

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/tests/default.py` & `pytest-alembic-0.9.1/src/pytest_alembic/tests/default.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,14 +81,15 @@
                     ],
                 )
 
     test_upgrade(alembic_runner)
     alembic_runner.generate_revision(
         message="test revision",
         autogenerate=True,
+        prevent_file_generation=True,
         process_revision_directives=verify_is_empty_revision,
     )
 
 
 @pytest.mark.alembic
 def test_up_down_consistency(alembic_runner):
     """Assert that all downgrades succeed.
```

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/tests/experimental/all_models_register_on_metadata.py` & `pytest-alembic-0.9.1/src/pytest_alembic/tests/experimental/all_models_register_on_metadata.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/tests/experimental/collect_clean_alembic_environment.py` & `pytest-alembic-0.9.1/src/pytest_alembic/tests/experimental/collect_clean_alembic_environment.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/src/pytest_alembic/tests/experimental/downgrade_leaves_no_trace.py` & `pytest-alembic-0.9.1/src/pytest_alembic/tests/experimental/downgrade_leaves_no_trace.py`

 * *Files identical despite different names*

### Comparing `pytest-alembic-0.9.0/setup.py` & `pytest-alembic-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ['alembic', 'pytest>=6.0', 'sqlalchemy']
 
 entry_points = \
 {'pytest11': ['pytest_alembic = pytest_alembic.plugin']}
 
 setup_kwargs = {
     'name': 'pytest-alembic',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'A pytest plugin for verifying alembic migrations.',
     'long_description': '![CircleCI](https://img.shields.io/circleci/build/gh/schireson/pytest-alembic/main)\n[![codecov](https://codecov.io/gh/schireson/pytest-alembic/branch/master/graph/badge.svg)](https://codecov.io/gh/schireson/pytest-alembic)\n[![Documentation Status](https://readthedocs.org/projects/pytest-alembic/badge/?version=latest)](https://pytest-alembic.readthedocs.io/en/latest/?badge=latest)\n\n## Introduction\n\nA pytest plugin to test alembic migrations (with default tests) and\nwhich enables you to write tests specific to your migrations.\n\n```bash\n$ pip install pytest-alembic\n$ pytest --test-alembic\n\n...\n::pytest_alembic/tests/model_definitions_match_ddl <- . PASSED           [ 25%]\n::pytest_alembic/tests/single_head_revision <- . PASSED                  [ 50%]\n::pytest_alembic/tests/up_down_consistency <- . PASSED                   [ 75%]\n::pytest_alembic/tests/upgrade <- . PASSED                               [100%]\n\n============================== 4 passed in 2.32s ===============================\n```\n\n## The pitch\n\nHave you ever merged a change to your models and you forgot to generate\na migration?\n\nHave you ever written a migration only to realize that it fails when\nthere’s data in the table?\n\nHave you ever written a **perfect** migration only to merge it and later\nfind out that someone else merged also merged a migration and your CD is\nnow broken!?\n\n`pytest-alembic` is meant to (with a little help) solve all these\nproblems and more. Note, due to a few different factors, there **may**\nbe some [minimal required\nsetup](http://pytest-alembic.readthedocs.io/en/latest/setup.html);\nhowever most of it is boilerplate akin to the setup required for alembic\nitself.\n\n### Built-in Tests\n\n- **test_single_head_revision**\n\n  Assert that there only exists one head revision.\n\n  We’re not sure what realistic scenario involves a diverging history to\n  be desirable. We have only seen it be the result of uncaught merge\n  conflicts resulting in a diverged history, which lazily breaks during\n  deployment.\n\n- **test_upgrade**\n\n  Assert that the revision history can be run through from base to head.\n\n- **test_model_definitions_match_ddl**\n\n  Assert that the state of the migrations matches the state of the\n  models describing the DDL.\n\n  In general, the set of migrations in the history should coalesce into\n  DDL which is described by the current set of models. Therefore, a call\n  to `revision --autogenerate` should always generate an empty migration\n  (e.g.\xa0find no difference between your database (i.e.\xa0migrations\n  history) and your models).\n\n- **test_up_down_consistency**\n\n  Assert that all downgrades succeed.\n\n  While downgrading may not be lossless operation data-wise, there’s a\n  theory of database migrations that says that the revisions in\n  existence for a database should be able to go from an entirely blank\n  schema to the finished product, and back again.\n\n- [Experimental\n  tests](http://pytest-alembic.readthedocs.io/en/latest/experimental_tests.html)\n\n  - all_models_register_on_metadata\n\n    Assert that all defined models are imported statically.\n\n    Prevents scenarios in which the minimal import of your models in your `env.py`\n    does not import all extant models, leading alembic to not autogenerate all\n    your models, or (worse!) suggest the deletion of tables which should still exist.\n\n  - downgrade_leaves_no_trace\n\n    Assert that there is no difference between the state of the database pre/post downgrade.\n\n    In essence this is a much more strict version of `test_up_down_consistency`,\n    where the state of a MetaData before and after a downgrade are identical as\n    far as alembic (autogenerate) is concerned.\n\n  These tests will need to be enabled manually because their semantics or API are\n  not yet guaranteed to stay the same. See the linked docs for more details!\n\nLet us know if you have any ideas for more built-in tests which would be\ngenerally useful for most alembic histories!\n\n### Custom Tests\n\nFor more information, see the docs for [custom\ntests](http://pytest-alembic.readthedocs.io/en/latest/custom_tests.html)\n(example below) or [custom static\ndata](http://pytest-alembic.readthedocs.io/en/latest/custom_data.html)\n(to be inserted automatically before a given revision).\n\nSometimes when writing a particularly gnarly data migration, it helps to\nbe able to practice a little timely TDD, since there’s always the\npotential you’ll trash your actual production data.\n\nWith `pytest-alembic`, you can write tests directly, in the same way\nthat you would normally, through the use of the `alembic_runner`\nfixture.\n\n```python\ndef test_gnarly_migration_xyz123(alembic_engine, alembic_runner):\n    # Migrate up to, but not including this new migration\n    alembic_runner.migrate_up_before(\'xyz123\')\n\n    # Perform some very specific data setup, because this migration is sooooo complex.\n    # ...\n    alembic_engine.execute(table.insert(id=1, name=\'foo\'))\n\n    alembic_runner.migrate_up_one()\n```\n\n`alembic_runner` has a number of methods designed to make it convenient\nto change the state of your database up, down, and all around.\n\n## Installing\n\n```bash\npip install "pytest-alembic"\n```\n',
     'author': 'Dan Cardin',
     'author_email': 'ddcardin@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/schireson/pytest-alembic',
```

### Comparing `pytest-alembic-0.9.0/PKG-INFO` & `pytest-alembic-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-alembic
-Version: 0.9.0
+Version: 0.9.1
 Summary: A pytest plugin for verifying alembic migrations.
 Home-page: https://github.com/schireson/pytest-alembic
 License: MIT
 Keywords: pytest,sqlalchemy,alembic,migration,revision
 Author: Dan Cardin
 Author-email: ddcardin@gmail.com
 Requires-Python: >=3.6,<4
```

