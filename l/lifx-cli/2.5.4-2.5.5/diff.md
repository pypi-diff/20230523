# Comparing `tmp/lifx_cli-2.5.4.tar.gz` & `tmp/lifx_cli-2.5.5.tar.gz`

## Comparing `lifx_cli-2.5.4.tar` & `lifx_cli-2.5.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rwxr-xr-x   0        0        0     1617 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/increment_version.sh
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/requirements.txt
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/.github/workflows/python-publish.yml
--rwxr-xr-x   0        0        0     2898 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/auth.py
--rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/colors.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/effects.py
--rwxr-xr-x   0        0        0    13218 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/lifx.py
--rwxr-xr-x   0        0        0     3149 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/lights.py
--rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/scenes.py
--rwxr-xr-x   0        0        0     1644 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/tests/lifx_cli_test.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/tests/requirements.txt
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/LICENSE
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/README.md
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/pyproject.toml
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1617 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/increment_version.sh
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/requirements.txt
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0      254 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/.hooks/pre-commit
+-rwxr-xr-x   0        0        0     2898 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/src/lifx/auth.py
+-rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/src/lifx/colors.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/src/lifx/effects.py
+-rwxr-xr-x   0        0        0    12365 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/src/lifx/lifx.py
+-rwxr-xr-x   0        0        0     3572 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/src/lifx/lights.py
+-rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/src/lifx/scenes.py
+-rwxr-xr-x   0        0        0     2382 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/tests/lifx_cli_test.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/tests/requirements.txt
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/LICENSE
+-rw-r--r--   0        0        0     3023 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/README.md
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/pyproject.toml
+-rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 lifx_cli-2.5.5/PKG-INFO
```

### Comparing `lifx_cli-2.5.4/increment_version.sh` & `lifx_cli-2.5.5/increment_version.sh`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.4/.github/workflows/pylint.yml` & `lifx_cli-2.5.5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.4/.github/workflows/pytest.yml` & `lifx_cli-2.5.5/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.4/.github/workflows/python-publish.yml` & `lifx_cli-2.5.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.4/src/lifx/auth.py` & `lifx_cli-2.5.5/src/lifx/auth.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.4/src/lifx/colors.py` & `lifx_cli-2.5.5/src/lifx/colors.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.4/src/lifx/effects.py` & `lifx_cli-2.5.5/src/lifx/effects.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.4/src/lifx/lights.py` & `lifx_cli-2.5.5/src/lifx/lights.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
-"""Control LIFX lights and effects."""
+"""Control LIFX lights."""
 import sys
 import json
 from requests import get, post, put
 from tabulate import tabulate
 from src.lifx.auth import Auth
 
 API = 'https://api.lifx.com/v1'
 
 
 class Lights:
-    """Control LIFX lights and effects."""
+    """Control LIFX lights."""
 
     def __init__(self):
         self.auth = Auth()
         self.auth_headers = self.auth.auth()
 
     def get(self):
         """Print a list of all LIFX devices on this account."""
@@ -24,28 +24,39 @@
 
         if response.status_code != 200:
             print(f"HTTP request failed. State code: {response.status_code}")
             sys.exit(30)
 
         response = json.loads(response.content)
 
-        devices = []
+        lights = []
+        switches = []
 
         for _, value in enumerate(response):
-            label = value["label"]
-            ident = value["id"]
+            device = value["label"]
+            device_id = value["id"]
             power = value["power"]
             connected = value["connected"]
-            group = value["group"]["name"]
+            group_name = value["group"]["name"]
             group_id = value["group"]["id"]
 
-            devices += [[label, ident, power, connected, group, group_id]]
-
-        devices.sort()
-        print(tabulate(devices, headers=["Name", "ID", "State", "Connected", "Group", "Group ID"]))
+            if value["product"]["product_id"] == 116:
+                switches += [[device, device_id, power, connected, group_name, group_id]]
+            else:
+                lights += [[device, device_id, power, connected, group_name, group_id]]
+
+        lights.sort()
+        print(tabulate(lights,
+                       headers=["Light", "ID", "State", "Connected", "Group", "Group ID"]))
+
+        if len(switches) > 0:
+            switches.sort()
+            print("\n\n")
+            print(tabulate(switches,
+                           headers=["Switch", "ID", "State", "Connected", "Group", "Group ID"]))
 
     def toggle(self, light_id, group):
         """Toggles the power for the specified light. Requires the device ID."""
 
         if group:
             light_id = f'group_id:{light_id}'
```

### Comparing `lifx_cli-2.5.4/src/lifx/scenes.py` & `lifx_cli-2.5.5/src/lifx/scenes.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.4/tests/lifx_cli_test.py` & `lifx_cli-2.5.5/tests/lifx_cli_test.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,84 @@
 #!/usr/bin/env python3
 """Tests for lifx-cli."""
 import pytest
 import src.lifx.lifx
+from src.lifx.auth import Auth
+from src.lifx.colors import Colors
+from src.lifx.effects import Effects
+from src.lifx.lights import Lights
+from src.lifx.scenes import Scenes
+
+VERSION = "2.5.5"
+TEST_HELP = "Control LIFX devices via the CLI!"
+TEST_GROUP = "68931117c352834e0a8f70aebcbcdae1"
+TEST_COLORS = ["purple", "green"]
+TEST_CYCLES = 4
+TEST_LIGHT = "d073d568d053"
+TEST_SCENE = "9371a59c-6ee7-4ced-a3d3-b25d9fc08aad"
 
-VERSION = "2.5.4"
 
-
-def test_version(capsys):
+@pytest.mark.parametrize("option", ("-v", "--version"))
+def test_version(capsys, option):
     """Test the version output."""
     with pytest.raises(SystemExit) as pytest_wrapped_e:
-        src.lifx.lifx.get_version()
+        src.lifx.lifx.main([option])
     out, err = capsys.readouterr()
     assert f"Version: {VERSION}" in out
     assert err == ""
     assert pytest_wrapped_e.type == SystemExit
     assert pytest_wrapped_e.value.code == 0
 
 
+@pytest.mark.parametrize("option", ("-h", "--help"))
+def test_help(capsys, option):
+    """Test the help output."""
+    with pytest.raises(SystemExit) as pytest_wrapped_e:
+        src.lifx.lifx.main([option])
+    out, err = capsys.readouterr()
+    assert TEST_HELP in out
+    assert err == ""
+    assert pytest_wrapped_e.type == SystemExit
+    assert pytest_wrapped_e.value.code == 0
+
+
+def test_auth():
+    """Validate the API token."""
+    auth = Auth()
+    assert auth.validate_token()
+
+
 def test_colors(capsys):
-    """Test the colors sub-command."""
-    cli_args = [False, 'blue']
-    src.lifx.lifx.colors_sub_command(cli_args)
+    """Test the 'colors' module."""
+    colors = Colors()
+    colors.validate_color(color="blue")
     out, err = capsys.readouterr()
     assert "Saturation" in out
     assert err == ""
 
 
 def test_effects():
-    """Test the effects sub-command (lights will flash at Wes' home)."""
-    cli_args = [False, '68931117c352834e0a8f70aebcbcdae1', True,
-                ['purple', 'green'], 4, True, False, False]
+    """Test the 'effects' module (lights will flash at Wes' home)."""
+    effects = Effects()
     with pytest.raises(SystemExit) as pytest_wrapped_e:
-        src.lifx.lifx.effects_sub_command(cli_args)
+        effects.breathe_effect(light_id=TEST_GROUP, group=True,
+                               color=TEST_COLORS, cycles=TEST_CYCLES)
     assert pytest_wrapped_e.type == SystemExit
     assert pytest_wrapped_e.value.code == 0
 
 
 def test_lights(capsys):
-    """Test the lights sub-command."""
-    cli_args = [True, False, False, False, False, False, False, False, False, False, False]
-    src.lifx.lifx.lights_sub_command(cli_args)
+    """Test the 'lights' module."""
+    lights = Lights()
+    lights.get()
     out, err = capsys.readouterr()
-    assert "d073d568d053" in out
+    assert TEST_LIGHT in out
     assert err == ""
 
 
 def test_scenes(capsys):
-    """Test the scenes sub-command."""
-    cli_args = [True, False]
-    src.lifx.lifx.scenes_sub_command(cli_args)
+    """Test the 'scenes' module."""
+    scenes = Scenes()
+    scenes.get()
     out, err = capsys.readouterr()
-    assert "9371a59c-6ee7-4ced-a3d3-b25d9fc08aad" in out
+    assert TEST_SCENE in out
     assert err == ""
```

### Comparing `lifx_cli-2.5.4/.gitignore` & `lifx_cli-2.5.5/.gitignore`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.4/LICENSE` & `lifx_cli-2.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.4/pyproject.toml` & `lifx_cli-2.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lifx-cli"
-version = "2.5.4"
+version = "2.5.5"
 authors = [{name="Wes Henderson", email="info@necrux.com"}]
 description = "The Unofficial LIFX CLI"
 readme = "README.md"
 requires-python = ">=3.5"
 dependencies = [
   'requests',
   'tabulate',
```

