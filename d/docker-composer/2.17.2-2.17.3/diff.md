# Comparing `tmp/docker_composer-2.17.2.tar.gz` & `tmp/docker_composer-2.17.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_composer-2.17.2.tar", max compression
+gzip compressed data, was "docker_composer-2.17.3.tar", max compression
```

## Comparing `docker_composer-2.17.2.tar` & `docker_composer-2.17.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11358 2023-05-22 17:40:30.205463 docker_composer-2.17.2/LICENSE.txt
--rw-r--r--   0        0        0     1978 2023-05-22 17:40:30.205594 docker_composer-2.17.2/README.md
--rw-r--r--   0        0        0     1369 2023-05-23 04:08:51.031016 docker_composer-2.17.2/pyproject.toml
--rw-r--r--   0        0        0       60 2023-05-22 19:40:35.299994 docker_composer-2.17.2/src/docker_composer/__init__.py
--rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206343 docker_composer-2.17.2/src/docker_composer/_utils/__init__.py
--rw-r--r--   0        0        0     4557 2023-05-22 20:35:25.788589 docker_composer-2.17.2/src/docker_composer/_utils/argument.py
--rw-r--r--   0        0        0     7241 2023-05-22 20:35:25.789294 docker_composer-2.17.2/src/docker_composer/_utils/generate_class.py
--rw-r--r--   0        0        0     3238 2023-05-22 17:40:30.206770 docker_composer-2.17.2/src/docker_composer/base.py
--rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206821 docker_composer-2.17.2/src/docker_composer/py.typed
--rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206931 docker_composer-2.17.2/src/docker_composer/runner/__init__.py
--rw-r--r--   0        0        0     1227 2023-05-22 20:35:25.790242 docker_composer-2.17.2/src/docker_composer/runner/cmd/build.py
--rw-r--r--   0        0        0     1811 2023-05-22 20:35:25.790760 docker_composer-2.17.2/src/docker_composer/runner/cmd/config.py
--rw-r--r--   0        0        0      937 2023-05-22 20:35:25.791110 docker_composer-2.17.2/src/docker_composer/runner/cmd/cp.py
--rw-r--r--   0        0        0     1414 2023-05-22 20:35:25.791824 docker_composer-2.17.2/src/docker_composer/runner/cmd/create.py
--rw-r--r--   0        0        0     1029 2023-05-22 20:35:25.792441 docker_composer-2.17.2/src/docker_composer/runner/cmd/down.py
--rw-r--r--   0        0        0      608 2023-05-22 20:35:25.792940 docker_composer-2.17.2/src/docker_composer/runner/cmd/events.py
--rw-r--r--   0        0        0     1234 2023-05-22 20:35:25.793552 docker_composer-2.17.2/src/docker_composer/runner/cmd/exec.py
--rw-r--r--   0        0        0      690 2023-05-22 20:35:25.794073 docker_composer-2.17.2/src/docker_composer/runner/cmd/images.py
--rw-r--r--   0        0        0      729 2023-05-22 20:35:25.794481 docker_composer-2.17.2/src/docker_composer/runner/cmd/kill.py
--rw-r--r--   0        0        0     1250 2023-05-22 20:35:25.795147 docker_composer-2.17.2/src/docker_composer/runner/cmd/logs.py
--rw-r--r--   0        0        0      830 2023-05-22 20:35:25.795508 docker_composer-2.17.2/src/docker_composer/runner/cmd/ls.py
--rw-r--r--   0        0        0      463 2023-05-22 20:35:25.795972 docker_composer-2.17.2/src/docker_composer/runner/cmd/pause.py
--rw-r--r--   0        0        0      687 2023-05-22 20:35:25.796437 docker_composer-2.17.2/src/docker_composer/runner/cmd/port.py
--rw-r--r--   0        0        0     1112 2023-05-22 20:35:25.797054 docker_composer-2.17.2/src/docker_composer/runner/cmd/ps.py
--rw-r--r--   0        0        0      964 2023-05-22 20:35:25.797590 docker_composer-2.17.2/src/docker_composer/runner/cmd/pull.py
--rw-r--r--   0        0        0      856 2023-05-22 20:35:25.798080 docker_composer-2.17.2/src/docker_composer/runner/cmd/push.py
--rw-r--r--   0        0        0      689 2023-05-22 20:35:25.798685 docker_composer-2.17.2/src/docker_composer/runner/cmd/restart.py
--rw-r--r--   0        0        0     1012 2023-05-22 20:35:25.799207 docker_composer-2.17.2/src/docker_composer/runner/cmd/rm.py
--rw-r--r--   0        0        0     2329 2023-05-22 20:35:25.799746 docker_composer-2.17.2/src/docker_composer/runner/cmd/run.py
--rw-r--r--   0        0        0      463 2023-05-22 20:35:25.800293 docker_composer-2.17.2/src/docker_composer/runner/cmd/start.py
--rw-r--r--   0        0        0      564 2023-05-22 20:35:25.800735 docker_composer-2.17.2/src/docker_composer/runner/cmd/stop.py
--rw-r--r--   0        0        0      473 2023-05-22 20:35:25.801329 docker_composer-2.17.2/src/docker_composer/runner/cmd/top.py
--rw-r--r--   0        0        0      471 2023-05-22 20:35:25.801939 docker_composer-2.17.2/src/docker_composer/runner/cmd/unpause.py
--rw-r--r--   0        0        0     3410 2023-05-22 20:35:25.802415 docker_composer-2.17.2/src/docker_composer/runner/cmd/up.py
--rw-r--r--   0        0        0      702 2023-05-22 20:35:25.802883 docker_composer-2.17.2/src/docker_composer/runner/cmd/version.py
--rw-r--r--   0        0        0    27397 2023-05-22 20:35:25.803600 docker_composer-2.17.2/src/docker_composer/runner/root.py
--rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 docker_composer-2.17.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-22 17:40:30.205463 docker_composer-2.17.3/LICENSE.txt
+-rw-r--r--   0        0        0     1978 2023-05-22 17:40:30.205594 docker_composer-2.17.3/README.md
+-rw-r--r--   0        0        0     1369 2023-05-23 04:26:04.917641 docker_composer-2.17.3/pyproject.toml
+-rw-r--r--   0        0        0       60 2023-05-22 19:40:35.299994 docker_composer-2.17.3/src/docker_composer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206343 docker_composer-2.17.3/src/docker_composer/_utils/__init__.py
+-rw-r--r--   0        0        0     4557 2023-05-22 20:35:25.788589 docker_composer-2.17.3/src/docker_composer/_utils/argument.py
+-rw-r--r--   0        0        0     7241 2023-05-22 20:35:25.789294 docker_composer-2.17.3/src/docker_composer/_utils/generate_class.py
+-rw-r--r--   0        0        0     3238 2023-05-22 17:40:30.206770 docker_composer-2.17.3/src/docker_composer/base.py
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206821 docker_composer-2.17.3/src/docker_composer/py.typed
+-rw-r--r--   0        0        0        0 2023-05-22 17:40:30.206931 docker_composer-2.17.3/src/docker_composer/runner/__init__.py
+-rw-r--r--   0        0        0     1227 2023-05-23 04:26:04.918719 docker_composer-2.17.3/src/docker_composer/runner/cmd/build.py
+-rw-r--r--   0        0        0     1811 2023-05-23 04:26:04.920419 docker_composer-2.17.3/src/docker_composer/runner/cmd/config.py
+-rw-r--r--   0        0        0      937 2023-05-23 04:26:04.921067 docker_composer-2.17.3/src/docker_composer/runner/cmd/cp.py
+-rw-r--r--   0        0        0     1414 2023-05-23 04:26:04.923573 docker_composer-2.17.3/src/docker_composer/runner/cmd/create.py
+-rw-r--r--   0        0        0     1029 2023-05-23 04:26:04.924300 docker_composer-2.17.3/src/docker_composer/runner/cmd/down.py
+-rw-r--r--   0        0        0      608 2023-05-23 04:26:04.924787 docker_composer-2.17.3/src/docker_composer/runner/cmd/events.py
+-rw-r--r--   0        0        0     1234 2023-05-23 04:26:04.925252 docker_composer-2.17.3/src/docker_composer/runner/cmd/exec.py
+-rw-r--r--   0        0        0      690 2023-05-23 04:26:04.925715 docker_composer-2.17.3/src/docker_composer/runner/cmd/images.py
+-rw-r--r--   0        0        0      729 2023-05-23 04:26:04.926585 docker_composer-2.17.3/src/docker_composer/runner/cmd/kill.py
+-rw-r--r--   0        0        0     1250 2023-05-23 04:26:04.927212 docker_composer-2.17.3/src/docker_composer/runner/cmd/logs.py
+-rw-r--r--   0        0        0      830 2023-05-23 04:26:04.927781 docker_composer-2.17.3/src/docker_composer/runner/cmd/ls.py
+-rw-r--r--   0        0        0      463 2023-05-23 04:26:04.928480 docker_composer-2.17.3/src/docker_composer/runner/cmd/pause.py
+-rw-r--r--   0        0        0      687 2023-05-23 04:26:04.929044 docker_composer-2.17.3/src/docker_composer/runner/cmd/port.py
+-rw-r--r--   0        0        0     1112 2023-05-23 04:26:04.929585 docker_composer-2.17.3/src/docker_composer/runner/cmd/ps.py
+-rw-r--r--   0        0        0      964 2023-05-23 04:26:04.930252 docker_composer-2.17.3/src/docker_composer/runner/cmd/pull.py
+-rw-r--r--   0        0        0      856 2023-05-23 04:26:04.930719 docker_composer-2.17.3/src/docker_composer/runner/cmd/push.py
+-rw-r--r--   0        0        0      689 2023-05-23 04:26:04.931180 docker_composer-2.17.3/src/docker_composer/runner/cmd/restart.py
+-rw-r--r--   0        0        0     1012 2023-05-23 04:26:04.931614 docker_composer-2.17.3/src/docker_composer/runner/cmd/rm.py
+-rw-r--r--   0        0        0     2329 2023-05-23 04:26:04.932024 docker_composer-2.17.3/src/docker_composer/runner/cmd/run.py
+-rw-r--r--   0        0        0      463 2023-05-23 04:26:04.932460 docker_composer-2.17.3/src/docker_composer/runner/cmd/start.py
+-rw-r--r--   0        0        0      564 2023-05-23 04:26:04.932850 docker_composer-2.17.3/src/docker_composer/runner/cmd/stop.py
+-rw-r--r--   0        0        0      473 2023-05-23 04:26:04.933272 docker_composer-2.17.3/src/docker_composer/runner/cmd/top.py
+-rw-r--r--   0        0        0      471 2023-05-23 04:26:04.933590 docker_composer-2.17.3/src/docker_composer/runner/cmd/unpause.py
+-rw-r--r--   0        0        0     3402 2023-05-23 04:26:04.933916 docker_composer-2.17.3/src/docker_composer/runner/cmd/up.py
+-rw-r--r--   0        0        0      702 2023-05-23 04:26:04.934369 docker_composer-2.17.3/src/docker_composer/runner/cmd/version.py
+-rw-r--r--   0        0        0    27385 2023-05-23 04:26:04.935079 docker_composer-2.17.3/src/docker_composer/runner/root.py
+-rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 docker_composer-2.17.3/PKG-INFO
```

### Comparing `docker_composer-2.17.2/LICENSE.txt` & `docker_composer-2.17.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.2/README.md` & `docker_composer-2.17.3/README.md`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.2/pyproject.toml` & `docker_composer-2.17.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docker-composer"
-version = "2.17.2"
+version = "2.17.3"
 description = "Use docker-compose from within Python"
 authors = ["Micha <schollm-git@gmx.com>"]
 readme = "README.md"
 homepage = "https://github.com/schollm/docker-composer"
 repository = "https://github.com/schollm/docker-composer"
 license = "Apache-2.0"
 packages = [
```

### Comparing `docker_composer-2.17.2/src/docker_composer/_utils/argument.py` & `docker_composer-2.17.3/src/docker_composer/_utils/argument.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.2/src/docker_composer/_utils/generate_class.py` & `docker_composer-2.17.3/src/docker_composer/_utils/generate_class.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.2/src/docker_composer/base.py` & `docker_composer-2.17.3/src/docker_composer/base.py`

 * *Files identical despite different names*

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/build.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/config.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/cp.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/cp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/create.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/create.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/down.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/down.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/events.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/exec.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/images.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/images.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/kill.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/kill.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/logs.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/ls.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/ls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/port.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/port.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/ps.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/ps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/pull.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/pull.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/push.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/push.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/restart.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/restart.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/rm.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/rm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/run.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/stop.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/stop.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/up.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/up.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
 
@@ -51,22 +51,22 @@
     """Pull without printing progress information."""
     remove_orphans: Optional[bool] = None
     """Remove containers for services not defined in the Compose file."""
     renew_anon_volumes: Optional[bool] = None
     """Recreate anonymous volumes instead of retrieving data from the previous containers."""
     scale: Optional[str] = None
     """Scale SERVICE to NUM instances. Overrides the scale setting in the Compose file if present."""
+    timeout: Optional[int] = None
+    """Use this timeout in seconds for container shutdown when attached or when containers are already running. (default 10)"""
     timestamps: Optional[bool] = None
     """Show timestamps."""
     wait: Optional[bool] = None
     """Wait for services to be running|healthy. Implies detached mode."""
     wait_timeout: Optional[int] = None
     """timeout waiting for application to be running|healthy."""
-    waitTimeout: Optional[int] = None
-    """Use this waitTimeout in seconds for container shutdown when attached or when containers are already running. (default 10)"""
     _cmd: str = "up"
     _options: List[str] = [
         "abort_on_container_exit",
         "always_recreate_deps",
         "attach_dependencies",
         "build",
         "detach",
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/cmd/version.py` & `docker_composer-2.17.3/src/docker_composer/runner/cmd/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 from docker_composer.base import DockerBaseRunner
```

### Comparing `docker_composer-2.17.2/src/docker_composer/runner/root.py` & `docker_composer-2.17.3/src/docker_composer/runner/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # DO NOT EDIT: Autogenerated by /Users/micha/dev/external/docker-composer/src/docker_composer/_utils/generate_class.py
-# for Docker Compose version v2.17.2
+# for Docker Compose version v2.17.3
 
 from typing import List, Optional
 
 import attr
 
 import docker_composer.runner.cmd.build
 import docker_composer.runner.cmd.config
@@ -591,18 +591,18 @@
         no_recreate: Optional[bool] = None,
         no_start: Optional[bool] = None,
         pull: Optional[str] = None,
         quiet_pull: Optional[bool] = None,
         remove_orphans: Optional[bool] = None,
         renew_anon_volumes: Optional[bool] = None,
         scale: Optional[str] = None,
+        timeout: Optional[int] = None,
         timestamps: Optional[bool] = None,
         wait: Optional[bool] = None,
         wait_timeout: Optional[int] = None,
-        waitTimeout: Optional[int] = None,
     ) -> docker_composer.runner.cmd.up.DockerComposeUp:
         """
         Usage:  docker compose up [OPTIONS] [SERVICE...]
         Create and start containers
 
         :param abort_on_container_exit: Stops all containers if any container was stopped. Incompatible with -d
         :param always_recreate_deps: Recreate dependent containers. Incompatible with --no-recreate.
@@ -620,18 +620,18 @@
         :param no_recreate: If containers already exist, don't recreate them. Incompatible with --force-recreate.
         :param no_start: Don't start the services after creating them.
         :param pull: Pull image before running ("always"|"missing"|"never") (default "missing")
         :param quiet_pull: Pull without printing progress information.
         :param remove_orphans: Remove containers for services not defined in the Compose file.
         :param renew_anon_volumes: Recreate anonymous volumes instead of retrieving data from the previous containers.
         :param scale: Scale SERVICE to NUM instances. Overrides the scale setting in the Compose file if present.
+        :param timeout: Use this timeout in seconds for container shutdown when attached or when containers are already running. (default 10)
         :param timestamps: Show timestamps.
         :param wait: Wait for services to be running|healthy. Implies detached mode.
         :param wait_timeout: timeout waiting for application to be running|healthy.
-        :param waitTimeout: Use this waitTimeout in seconds for container shutdown when attached or when containers are already running. (default 10)
         """
         runner = docker_composer.runner.cmd.up.DockerComposeUp(
             **{k: v for k, v in locals().items() if k != "self"}
         )
         runner._parent_cmd = self._call_cmd()
         return runner
```

### Comparing `docker_composer-2.17.2/PKG-INFO` & `docker_composer-2.17.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-composer
-Version: 2.17.2
+Version: 2.17.3
 Summary: Use docker-compose from within Python
 Home-page: https://github.com/schollm/docker-composer
 License: Apache-2.0
 Author: Micha
 Author-email: schollm-git@gmx.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

