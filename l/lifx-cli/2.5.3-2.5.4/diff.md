# Comparing `tmp/lifx_cli-2.5.3.tar.gz` & `tmp/lifx_cli-2.5.4.tar.gz`

## Comparing `lifx_cli-2.5.3.tar` & `lifx_cli-2.5.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rwxr-xr-x   0        0        0     1519 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/increment_version.sh
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/requirements.txt
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/.github/workflows/python-publish.yml
--rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/auth.py
--rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/colors.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/effects.py
--rwxr-xr-x   0        0        0    12579 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/lifx.py
--rwxr-xr-x   0        0        0     3149 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/lights.py
--rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/src/lifx/scenes.py
--rwxr-xr-x   0        0        0     1262 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/tests/lifx_cli_test.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/tests/requirements.txt
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/LICENSE
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/README.md
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/pyproject.toml
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 lifx_cli-2.5.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1617 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/increment_version.sh
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/requirements.txt
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0     2898 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/auth.py
+-rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/colors.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/effects.py
+-rwxr-xr-x   0        0        0    13218 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/lifx.py
+-rwxr-xr-x   0        0        0     3149 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/lights.py
+-rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/src/lifx/scenes.py
+-rwxr-xr-x   0        0        0     1644 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/tests/lifx_cli_test.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/tests/requirements.txt
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/LICENSE
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/README.md
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 lifx_cli-2.5.4/PKG-INFO
```

### Comparing `lifx_cli-2.5.3/increment_version.sh` & `lifx_cli-2.5.4/increment_version.sh`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env bash
 # One stop shop for incrementing the lifx-cli version.
 
 declare -l ANSWER
 NEW_VERSION=$1
 CURRENT_VERSION=$(git describe --tags --abbrev=0)
 FILES=('pyproject.toml'
-       'src/lifx/lifx.py')
+       'src/lifx/lifx.py'
+       'tests/lifx_cli_test.py')
 
 function is_command {
     local FAILURE
   
     for program in $@; do
         hash ${program} > /dev/null 2>&1
         if [ $? != 0 ]; then
@@ -44,15 +45,16 @@
     git push origin main
     git tag v${NEW_VERSION}
     git push origin --tags
 }
 
 # Input validation.
 if [ -z ${NEW_VERSION} ]; then
-    err 5 "Must supply a new version number."
+    echo "Current Tagged Version: ${CURRENT_VERSION}"
+    err 5 "Must supply a new version number to continue."
 fi
 
 if ! echo ${NEW_VERSION} | grep -q "^[0-9]*\.[0-9]*\.[0-9]*$"; then
     err 6 "New version number is in the wrong format. Must be: <MAJOR>.<MINOR>.<PATCH>"
 fi
 
 is_command gawk
```

### Comparing `lifx_cli-2.5.3/.github/workflows/pylint.yml` & `lifx_cli-2.5.4/.github/workflows/pylint.yml`

 * *Files 17% similar despite different names*

```diff
@@ -19,8 +19,8 @@
         python -m pip install --upgrade pip
         pip install pylint
         pip install -r requirements.txt
         pip install -r tests/requirements.txt
         pip install -e .
     - name: Analysing the code with pylint
       run: |
-        pylint $(git ls-files '*.py') --fail-under=9.50
+        pylint $(git ls-files '*.py') --fail-under=10.00
```

### Comparing `lifx_cli-2.5.3/.github/workflows/pytest.yml` & `lifx_cli-2.5.4/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.3/.github/workflows/python-publish.yml` & `lifx_cli-2.5.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.3/src/lifx/colors.py` & `lifx_cli-2.5.4/src/lifx/colors.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.3/src/lifx/effects.py` & `lifx_cli-2.5.4/src/lifx/effects.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 
     @staticmethod
     def list_effects():
         """List effects currently supported by the CLI."""
         print(tabulate(EFFECTS, headers=["Name", "Description"]))
         print(f"\n{EFFECTS_NOTICE}")
 
-    def breathe_effect(self, light_id, group, color):
+    def breathe_effect(self, light_id, group, color, cycles):
         """Activates the breath effect (period: 2; cycles: 10).
         Requires the device ID and color."""
 
         if len(color) == 1:
             data = {
                 "period": 2,
-                "cycles": 10,
+                "cycles": {cycles},
                 "color": f"{color[0]}",
             }
         else:
             data = {
                 "period": 2,
-                "cycles": 10,
+                "cycles": {cycles},
                 "from_color": f"{color[0]}",
                 "color": f"{color[1]}",
             }
 
         if group:
             light_id = f'group_id:{light_id}'
 
@@ -51,28 +51,28 @@
 
         if response.status_code != 207:
             print(f"HTTP request failed. State code: {response.status_code}")
             sys.exit(20)
         else:
             sys.exit(0)
 
-    def pulse_effect(self, light_id, group, color):
+    def pulse_effect(self, light_id, group, color, cycles):
         """Activates the pulse effect (period: 2; cycles: 10).
         Requires the device ID and color."""
 
         if len(color) == 1:
             data = {
                 "period": 2,
-                "cycles": 10,
+                "cycles": {cycles},
                 "color": f"{color[0]}",
             }
         else:
             data = {
                 "period": 2,
-                "cycles": 10,
+                "cycles": {cycles},
                 "from_color": f"{color[0]}",
                 "color": f"{color[1]}",
             }
 
         if group:
             light_id = f'group_id:{light_id}'
```

### Comparing `lifx_cli-2.5.3/src/lifx/lifx.py` & `lifx_cli-2.5.4/src/lifx/lifx.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,21 @@
 ██      ██ ███████ ██   ██      ██████ ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ██      ██ █████     ███       ██      ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ███████ ██ ██      ██   ██      ██████ ███████ ██
 
 """
-VERSION = "2.5.3"
+VERSION = "2.5.4"
+
+
+def get_version():
+    """Print the version and exit."""
+    print(f"Version: {VERSION}")
+    sys.exit(0)
 
 
 def colors_sub_command(args):
     """Control the actions for the 'colors' sub-command."""
     colors = Colors()
 
     if isinstance(args, list):
@@ -47,35 +53,41 @@
     effects = Effects()
 
     if isinstance(args, list):
         list_effects = args[0]
         light_id = args[1]
         group = args[2]
         color = args[3]
-        breathe = args[4]
-        pulse = args[5]
-        stop = args[6]
+        cycles = args[4]
+        breathe = args[5]
+        pulse = args[6]
+        stop = args[7]
     else:
         list_effects = args.list_effects
         light_id = args.light_id
         group = args.group
         color = args.color
+        cycles = args.cycles
         breathe = args.breathe
         pulse = args.pulse
         stop = args.stop
 
     if list_effects:
         effects.list_effects()
     elif not light_id:
         print("Must specify a light/group ID.")
         sys.exit(4)
+    elif light_id and not color:
+        print("Must specify at least 1 color.")
+        sys.exit(5)
+
     if breathe:
-        effects.breathe_effect(light_id, group, color)
+        effects.breathe_effect(light_id, group, color, cycles)
     elif pulse:
-        effects.pulse_effect(light_id, group, color)
+        effects.pulse_effect(light_id, group, color, cycles)
     elif stop:
         effects.stop_effect(light_id, group)
 
 
 def lights_sub_command(args):
     """Control the actions for the 'lights' sub-command."""
     light = Lights()
@@ -149,15 +161,16 @@
 def main():
     """Main entrypoint for the LIFX CLI."""
     auth = Auth()
     print(LOGO)
     # Create the parser
     description = 'Control LIFX devices via the CLI!'
     epilog = 'Run `lifx --configure` to setup authentication.'
-    job_options = argparse.ArgumentParser(description=description, epilog=epilog)
+    job_options = argparse.ArgumentParser(description=description,
+                                          epilog=epilog)
 
     # Add the arguments
     job_options.add_argument('-c',
                              '--configure',
                              default=False,
                              action='store_true',
                              help='Add your LIFX token to the local authentication file: ~/.keys')
@@ -165,15 +178,16 @@
                              '--version',
                              default=False,
                              action='store_true',
                              help='Print the version and exit.')
 
     # Add the 'lights' sub-command.
     light_job_options = job_options.add_subparsers(dest='command')
-    light_command = light_job_options.add_parser('lights', help='Light specific functions.')
+    light_command = light_job_options.add_parser('lights',
+                                                 help='Light specific functions.')
     light_command.add_argument('-l',
                                '--list',
                                default=False,
                                dest='list_devices',
                                action='store_true',
                                help='List LIFX devices.')
     light_command.add_argument('-i',
@@ -229,15 +243,16 @@
     light_command.add_argument('-u',
                                '--duration',
                                default=1,
                                action='store',
                                help='State: How many seconds should the action take. [Default: 1]')
 
     # Add the 'scenes' sub-command.
-    scene_command = light_job_options.add_parser('scenes', help='Scene specific functions.')
+    scene_command = light_job_options.add_parser('scenes',
+                                                 help='Scene specific functions.')
     scene_command.add_argument('-l',
                                '--list',
                                default=False,
                                dest='list_scenes',
                                action='store_true',
                                help='List LIFX scenes.')
     scene_command.add_argument('-i',
@@ -245,19 +260,19 @@
                                default=False,
                                dest='scene_id',
                                action='store',
                                metavar='ID',
                                help='Activate scene.')
 
     # Add the 'effects' sub-command.
-    effects_description = 'Control lighting effects.'
     effects_epilog = "Note: The CLI can only control effects stored on your light's firmware."
-    effects_help = 'Effects specific functions.'
-    effect_command = light_job_options.add_parser('effects', description=effects_description,
-                                                  epilog=effects_epilog, help=effects_help)
+    effect_command = light_job_options.add_parser('effects',
+                                                  description='Control lighting effects.',
+                                                  epilog=effects_epilog,
+                                                  help='Effects specific functions.')
     effect_command.add_argument('-l',
                                 '--list',
                                 default=False,
                                 dest='list_effects',
                                 action='store_true',
                                 help='List effects supported by the LIFX CLI.')
     effect_command.add_argument('-i',
@@ -273,32 +288,36 @@
                                 action='store_true',
                                 help='Specify whether or not the target is a group.')
     effect_command.add_argument('-c',
                                 '--color',
                                 default=[],
                                 action='append',
                                 help='Set the color; add multiple -c options to alternate colors.')
+    effect_command.add_argument('-y',
+                                '--cycles',
+                                default=10,
+                                action='store',
+                                help='Number of cycles to perform the effect. [Default: 10]')
     effect_command.add_argument('--breathe',
                                 default=False,
                                 action='store_true',
                                 help='Effects: Breathe')
     effect_command.add_argument('--pulse',
                                 default=False,
                                 action='store_true',
                                 help='Effects: Pulse')
     effect_command.add_argument('--stop',
                                 default=False,
                                 action='store_true',
                                 help='Effects: Stop')
 
     # Add the 'Colors' sub-command.
-    colors_description = 'Explore all of the color-related options!'
-    colors_help = 'Learn how to provide colors to the CLI.'
-    color_command = light_job_options.add_parser('colors', description=colors_description,
-                                                 help=colors_help)
+    color_command = light_job_options.add_parser('colors',
+                                                 description='Explore color-related options!',
+                                                 help='Learn how to provide colors to the CLI.')
     color_command.add_argument('-l',
                                '--list',
                                default=False,
                                dest='list_colors',
                                action='store_true',
                                help='List color options supported by the LIFX CLI.')
     color_command.add_argument('-c',
@@ -307,16 +326,15 @@
                                dest='colors',
                                action='store',
                                help='Validate a color using the LIFX API.')
 
     args = job_options.parse_args()
 
     if args.version:
-        print(f"Version: {VERSION}")
-        sys.exit(0)
+        get_version()
 
     # Configure authentication.
     if args.configure:
         auth.configure()
 
     # The 'colors' sub-command.
     if args.command == 'colors':
```

### Comparing `lifx_cli-2.5.3/src/lifx/lights.py` & `lifx_cli-2.5.4/src/lifx/lights.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.3/src/lifx/scenes.py` & `lifx_cli-2.5.4/src/lifx/scenes.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.3/.gitignore` & `lifx_cli-2.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.3/LICENSE` & `lifx_cli-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.3/README.md` & `lifx_cli-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.3/pyproject.toml` & `lifx_cli-2.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lifx-cli"
-version = "2.5.3"
+version = "2.5.4"
 authors = [{name="Wes Henderson", email="info@necrux.com"}]
 description = "The Unofficial LIFX CLI"
 readme = "README.md"
 requires-python = ">=3.5"
 dependencies = [
   'requests',
   'tabulate',
```

### Comparing `lifx_cli-2.5.3/PKG-INFO` & `lifx_cli-2.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifx-cli
-Version: 2.5.3
+Version: 2.5.4
 Summary: The Unofficial LIFX CLI
 Project-URL: Homepage, https://github.com/necrux/lifx-cli
 Project-URL: Bug Tracker, https://github.com/necrux/lifx-cli/issues
 Author-email: Wes Henderson <info@necrux.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

