# Comparing `tmp/sca_rhythm-0.4.9.tar.gz` & `tmp/sca_rhythm-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sca_rhythm-0.4.9.tar", max compression
+gzip compressed data, was "sca_rhythm-0.5.0.tar", max compression
```

## Comparing `sca_rhythm-0.4.9.tar` & `sca_rhythm-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.4.9/LICENSE.md
--rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.4.9/README.md
--rw-r--r--   0        0        0      357 2023-05-18 18:52:15.885999 sca_rhythm-0.4.9/pyproject.toml
--rw-r--r--   0        0        0    16425 2023-05-18 18:52:01.877993 sca_rhythm-0.4.9/sca_rhythm/__init__.py
--rw-r--r--   0        0        0     6872 2023-05-18 08:56:42.945290 sca_rhythm-0.4.9/sca_rhythm/progress.py
--rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 sca_rhythm-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0      586 2023-03-23 23:01:50.128697 sca_rhythm-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0     2384 2023-03-24 04:09:44.600188 sca_rhythm-0.5.0/README.md
+-rw-r--r--   0        0        0      357 2023-05-23 18:55:30.668198 sca_rhythm-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    16487 2023-05-19 15:25:47.040793 sca_rhythm-0.5.0/sca_rhythm/__init__.py
+-rw-r--r--   0        0        0     6872 2023-05-18 08:56:42.945290 sca_rhythm-0.5.0/sca_rhythm/progress.py
+-rw-r--r--   0        0        0     2904 1970-01-01 00:00:00.000000 sca_rhythm-0.5.0/PKG-INFO
```

### Comparing `sca_rhythm-0.4.9/LICENSE.md` & `sca_rhythm-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.9/README.md` & `sca_rhythm-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.9/sca_rhythm/__init__.py` & `sca_rhythm-0.5.0/sca_rhythm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,23 @@
 class NonRetryableException(Exception):
     pass
 
 
 def _validate_args(steps, name, app_id):
     assert len(steps) > 0, 'steps is empty'
     for i, step in enumerate(steps):
-        assert 'name' in step, f'step - {i} does not have "name" key'
-        assert len(step['name']) > 0, f'step - {i} name is empty'
-        assert 'task' in step, f'step - {i} does not have "task" key'
+        attrs = ['name', 'task']
+        for attr in attrs:
+            assert attr in step, f'step[{i}] does not have "{attr}" key'
+            assert isinstance(attr, str), f'step[{i}]["{attr}"] is not a string'
+            assert len(step[attr]) > 0, f'step[{i}]["{attr}"] is an empty string'
+        if 'queue' in step:
+            attr = 'queue'
+            assert isinstance(attr, str), f'step[{i}]["{attr}"] is not a string'
+            assert len(step[attr]) > 0, f'step[{i}]["{attr}"] is an empty string'
         # assert step['task'] in self.app.tasks, \
         #     f' step - {i} Task {step["task"]} is not registered in the celery application'
     names = [step['name'] for step in steps]
     duplicate_names = duplicates(names)
     assert len(duplicate_names) == 0, f'Steps with duplicate names: {duplicate_names}'
 
     assert name, 'name cannot be empty'
@@ -63,31 +69,35 @@
                 'steps': steps,
                 'name': name,
                 'app_id': app_id,
                 'description': description
             }
             self.wf_col.insert_one(self.workflow)
 
+    def wf_send_task(self, step: dict, task_args: list | tuple = None, task_kwargs: dict = None, **kwargs):
+        task_name = step['task']
+        task_queue = step.get('queue', None)
+
+        task_kwargs = task_kwargs or {}
+        task_kwargs['workflow_id'] = self.workflow['_id']
+        task_kwargs['step'] = step['name']
+
+        self.app.send_task(name=task_name, args=task_args, kwargs=task_kwargs, queue=task_queue, **kwargs)
+
     def start(self, *args, **kwargs):
         """
         Launches the task of the first step in this workflow.
 
         The task is called with given args and kwargs
         along with additional keyword args "workflow_id" and "step"
 
         :return: None
         """
         first_step = self.workflow['steps'][0]
-        # task = self.app.tasks[first_step['task']]
-
-        kwargs['workflow_id'] = self.workflow['_id']
-        kwargs['step'] = first_step['name']
-        # task.apply_async(args, kwargs)
-
-        self.app.send_task(first_step['task'], args, kwargs)
+        self.wf_send_task(first_step, args, kwargs)
 
     def pause(self):
         """
         Revoke the current running task.
 
         :return: status of the pause operation and the revoked step if successful
         - dict { "paused": bool, "revoked_step": dict }
@@ -140,20 +150,15 @@
                 # task = self.app.tasks[step['task']]
 
                 # failed / revoked task instance
                 task_inst = self.get_last_run_task_instance(step)
                 assert not (task_inst is None and args is None), 'no args are provided and there is no last run task'
                 task_args = task_inst['args'] if task_inst is not None else args
 
-                kwargs = {
-                    'workflow_id': self.workflow['_id'],
-                    'step': step['name']
-                }
-                # task.apply_async(task_args, kwargs)
-                self.app.send_task(step['task'], task_args, kwargs)
+                self.wf_send_task(step, task_args)
                 # print(f' resuming step {step["name"]}')
                 return {
                     'resumed': True,
                     'restarted_step': {
                         'name': step['name'],
                         'task': step['task']
                     }
@@ -197,22 +202,15 @@
         :return:
         """
         # self.update_step_end_time(step_name)
         next_step = self.get_next_step(step_name)
 
         # apply next task with retval
         if next_step:
-            # next_task = self.app.tasks[next_step['task']]
-
-            kwargs = {
-                'workflow_id': self.workflow['_id'],
-                'step': next_step['name']
-            }
-            # next_task.apply_async((retval[0],), kwargs)
-            self.app.send_task(next_step['task'], (retval[0],), kwargs)
+            self.wf_send_task(next_step, (retval[0],))
             # print(f' starting next step {next_step["name"]}')
 
     def update(self):
         """
         Update the workflow object in mongo db
         :return: None
         """
```

### Comparing `sca_rhythm-0.4.9/sca_rhythm/progress.py` & `sca_rhythm-0.5.0/sca_rhythm/progress.py`

 * *Files identical despite different names*

### Comparing `sca_rhythm-0.4.9/PKG-INFO` & `sca_rhythm-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sca-rhythm
-Version: 0.4.9
+Version: 0.5.0
 Summary: Create and manage workflows using Celery tasks
 Author: Deepak Duggirala
 Author-email: deepakduggi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

