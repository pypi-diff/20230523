# Comparing `tmp/foxplot-0.0.2.tar.gz` & `tmp/foxplot-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foxplot-0.0.2.tar", last modified: Wed May  3 10:10:49 2023, max compression
+gzip compressed data, was "foxplot-0.1.0.tar", last modified: Tue May 23 17:58:24 2023, max compression
```

## Comparing `foxplot-0.0.2.tar` & `foxplot-0.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     2700 2023-05-03 10:05:19.625704 foxplot-0.0.2/.github/workflows/CI.yml
--rw-r--r--   0        0        0     1270 2023-05-03 10:05:32.381708 foxplot-0.0.2/.github/workflows/docs.yml
--rw-r--r--   0        0        0       62 2023-05-03 10:05:19.625704 foxplot-0.0.2/.gitignore
--rw-r--r--   0        0        0      373 2023-05-03 09:37:34.286589 foxplot-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-01-26 08:59:41.542467 foxplot-0.0.2/LICENSE
--rw-r--r--   0        0        0       30 2023-01-26 08:59:41.542467 foxplot-0.0.2/MANIFEST.in
--rw-r--r--   0        0        0     2262 2023-05-03 10:05:19.625704 foxplot-0.0.2/README.md
--rw-r--r--   0        0        0       51 2023-05-03 10:05:19.625704 foxplot-0.0.2/docs/api.rst
--rw-r--r--   0        0        0     9358 2023-05-03 10:05:19.625704 foxplot-0.0.2/docs/conf.py
--rw-r--r--   0        0        0      204 2023-05-03 10:05:19.625704 foxplot-0.0.2/docs/environment.yml
--rw-r--r--   0        0        0      253 2023-05-03 10:05:19.629704 foxplot-0.0.2/docs/index.rst
--rw-r--r--   0        0        0      202 2023-05-03 10:05:19.629704 foxplot-0.0.2/docs/installation.rst
--rw-r--r--   0        0        0     1003 2023-05-03 10:05:19.629704 foxplot-0.0.2/docs/usage.rst
--rw-r--r--   0        0        0     1073 2023-04-25 14:58:06.539529 foxplot-0.0.2/examples/plot_robot_data.py
--rw-r--r--   0        0        0   128378 2023-04-25 14:37:52.909959 foxplot-0.0.2/examples/robot_data.json
--rw-r--r--   0        0        0      747 2023-05-03 09:37:39.262562 foxplot-0.0.2/foxplot/__init__.py
--rw-r--r--   0        0        0     2971 2023-05-03 09:37:04.506756 foxplot-0.0.2/foxplot/cli.py
--rw-r--r--   0        0        0     1442 2023-05-02 15:36:42.759188 foxplot-0.0.2/foxplot/color_picker.py
--rw-r--r--   0        0        0      777 2023-05-03 09:37:04.506756 foxplot-0.0.2/foxplot/decoders/__init__.py
--rw-r--r--   0        0        0     1469 2023-05-02 15:36:46.319031 foxplot-0.0.2/foxplot/decoders/json.py
--rw-r--r--   0        0        0     1302 2023-05-03 09:37:04.506756 foxplot-0.0.2/foxplot/decoders/msgpack.py
--rw-r--r--   0        0        0      736 2023-05-02 15:36:38.119141 foxplot-0.0.2/foxplot/exceptions.py
--rw-r--r--   0        0        0     5667 2023-05-03 09:37:04.510756 foxplot-0.0.2/foxplot/fox.py
--rw-r--r--   0        0        0     8177 2023-05-02 15:36:35.263076 foxplot-0.0.2/foxplot/generate_html.py
--rw-r--r--   0        0        0     1597 2023-04-25 14:56:10.622539 foxplot-0.0.2/foxplot/indexed_series.py
--rw-r--r--   0        0        0     3231 2023-04-25 14:56:38.401779 foxplot-0.0.2/foxplot/node.py
--rw-r--r--   0        0        0   120184 2023-05-02 15:36:29.614947 foxplot-0.0.2/foxplot/uPlot/uPlot.iife.js
--rw-r--r--   0        0        0     1839 2023-05-02 15:36:29.614947 foxplot-0.0.2/foxplot/uPlot/uPlot.min.css
--rw-r--r--   0        0        0     4543 2023-05-02 15:36:29.614947 foxplot-0.0.2/foxplot/uPlot/uPlot.mousewheel.js
--rw-r--r--   0        0        0     1205 2023-04-25 14:19:33.129645 foxplot-0.0.2/foxplot/write_tmpfile.py
--rw-r--r--   0        0        0     1529 2023-04-24 12:26:58.318170 foxplot-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       70 2023-01-26 08:59:41.542467 foxplot-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1057 2023-04-04 12:24:42.147920 foxplot-0.0.2/tests/test_color_picker.py
--rw-r--r--   0        0        0     1739 2023-05-03 09:37:04.510756 foxplot-0.0.2/tests/test_decoders.py
--rw-r--r--   0        0        0     6603 2023-04-24 12:24:53.005389 foxplot-0.0.2/tests/test_fox.py
--rw-r--r--   0        0        0     1074 2023-04-24 11:57:18.540637 foxplot-0.0.2/tests/test_generate_html.py
--rw-r--r--   0        0        0      739 2023-05-03 09:37:04.510756 foxplot-0.0.2/tox.ini
--rw-r--r--   0        0        0     3321 1970-01-01 00:00:00.000000 foxplot-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2700 2023-05-03 10:05:19.625704 foxplot-0.1.0/.github/workflows/CI.yml
+-rw-r--r--   0        0        0     1268 2023-05-03 10:16:36.797927 foxplot-0.1.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0       62 2023-05-03 10:05:19.625704 foxplot-0.1.0/.gitignore
+-rw-r--r--   0        0        0      728 2023-05-23 17:57:57.262019 foxplot-0.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-01-26 08:59:41.542467 foxplot-0.1.0/LICENSE
+-rw-r--r--   0        0        0       30 2023-01-26 08:59:41.542467 foxplot-0.1.0/MANIFEST.in
+-rw-r--r--   0        0        0     2248 2023-05-23 17:57:22.370680 foxplot-0.1.0/README.md
+-rw-r--r--   0        0        0       51 2023-05-03 10:05:19.625704 foxplot-0.1.0/docs/api.rst
+-rw-r--r--   0        0        0     9358 2023-05-03 10:05:19.625704 foxplot-0.1.0/docs/conf.py
+-rw-r--r--   0        0        0      204 2023-05-03 10:05:19.625704 foxplot-0.1.0/docs/environment.yml
+-rw-r--r--   0        0        0      253 2023-05-03 10:05:19.629704 foxplot-0.1.0/docs/index.rst
+-rw-r--r--   0        0        0      202 2023-05-03 10:05:19.629704 foxplot-0.1.0/docs/installation.rst
+-rw-r--r--   0        0        0      983 2023-05-16 17:17:17.695690 foxplot-0.1.0/docs/usage.rst
+-rw-r--r--   0        0        0     1073 2023-04-25 14:58:06.539529 foxplot-0.1.0/examples/plot_robot_data.py
+-rw-r--r--   0        0        0   128378 2023-04-25 14:37:52.909959 foxplot-0.1.0/examples/robot_data.json
+-rw-r--r--   0        0        0      747 2023-05-23 17:58:03.477903 foxplot-0.1.0/foxplot/__init__.py
+-rw-r--r--   0        0        0     3682 2023-05-23 17:57:22.374680 foxplot-0.1.0/foxplot/cli.py
+-rw-r--r--   0        0        0     1442 2023-05-16 17:17:52.315117 foxplot-0.1.0/foxplot/color_picker.py
+-rw-r--r--   0        0        0      777 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/decoders/__init__.py
+-rw-r--r--   0        0        0     1469 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/decoders/json.py
+-rw-r--r--   0        0        0     1302 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/decoders/msgpack.py
+-rw-r--r--   0        0        0      736 2023-05-16 17:17:52.315117 foxplot-0.1.0/foxplot/exceptions.py
+-rw-r--r--   0        0        0     6137 2023-05-23 17:57:22.374680 foxplot-0.1.0/foxplot/fox.py
+-rw-r--r--   0        0        0     8177 2023-05-16 17:17:52.315117 foxplot-0.1.0/foxplot/generate_html.py
+-rw-r--r--   0        0        0     1597 2023-05-16 17:17:52.315117 foxplot-0.1.0/foxplot/indexed_series.py
+-rw-r--r--   0        0        0     3231 2023-05-16 17:17:52.315117 foxplot-0.1.0/foxplot/node.py
+-rw-r--r--   0        0        0   120184 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/uPlot/uPlot.iife.js
+-rw-r--r--   0        0        0     1839 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/uPlot/uPlot.min.css
+-rw-r--r--   0        0        0     4543 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/uPlot/uPlot.mousewheel.js
+-rw-r--r--   0        0        0     1217 2023-05-16 17:17:52.319117 foxplot-0.1.0/foxplot/write_tmpfile.py
+-rw-r--r--   0        0        0     1544 2023-05-16 17:17:17.695690 foxplot-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-01-26 08:59:41.542467 foxplot-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-04-04 12:24:42.147920 foxplot-0.1.0/tests/test_color_picker.py
+-rw-r--r--   0        0        0     1739 2023-05-03 09:37:04.510756 foxplot-0.1.0/tests/test_decoders.py
+-rw-r--r--   0        0        0     6603 2023-04-24 12:24:53.005389 foxplot-0.1.0/tests/test_fox.py
+-rw-r--r--   0        0        0     1074 2023-04-24 11:57:18.540637 foxplot-0.1.0/tests/test_generate_html.py
+-rw-r--r--   0        0        0      739 2023-05-03 09:37:04.510756 foxplot-0.1.0/tox.ini
+-rw-r--r--   0        0        0     3330 1970-01-01 00:00:00.000000 foxplot-0.1.0/PKG-INFO
```

### Comparing `foxplot-0.0.2/.github/workflows/CI.yml` & `foxplot-0.1.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/.github/workflows/docs.yml` & `foxplot-0.1.0/.github/workflows/docs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -31,13 +31,13 @@
 
             - name: "Build documentation"
               run: |
                   sphinx-build docs _build -W
 
             - name: "Deploy to GitHub Pages"
               uses: peaceiris/actions-gh-pages@v3
-              if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/master' }}
+              if: ${{ github.event_name == 'push' && github.ref == 'refs/heads/main' }}
               with:
                   publish_branch: gh-pages
                   github_token: ${{ secrets.GITHUB_TOKEN }}
                   publish_dir: _build/
                   force_orphan: true
```

### Comparing `foxplot-0.0.2/LICENSE` & `foxplot-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/README.md` & `foxplot-0.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 # foxplot
 
 [![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/foxplot/CI.yml?branch=main)](https://github.com/stephane-caron/foxplot/actions)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/stephane-caron/foxplot/docs.yml?branch=main&label=docs)](https://stephane-caron.github.io/foxplot/)
 
-Plot time-series data from [line-delimited JSON](https://en.wikipedia.org/wiki/JSON_streaming#Line-delimited_JSON).
+Plot time-series data from [newline-delimited JSON](https://en.wikipedia.org/wiki/JSON_streaming#Newline-delimited-JSON).
 
 Foxplot stands for "Frequent Observation diXionary plots". Frequent observations arise from the project's initial use case (robotic control loops). Dictionaries are the observation format used in [Vulp](https://github.com/tasts-robots/vulp). Plots are plots :wink:
 
 ## Installation
 
 ```console
 $ pip install foxplot
 ```
 
 ## Usage
 
 ### Interactive mode
 
-In interactive mode, you can explore the data in ``fox.data`` (tab completion works) and plot it using the ``fox.plot`` function:
+In interactive mode, you can explore the data in ``data`` (tab completion works) and plot it using the ``fox.plot`` function:
 
 ```python
 $ foxplot -i upkie_2023-05-03-103245.mpack
 Python 3.8.10 (default, Mar 13 2023, 10:26:41)
 Type 'copyright', 'credits' or 'license' for more information
 IPython 8.0.1 -- An enhanced Interactive Python. Type '?' for help.
 
 In [1]: fox.plot(
    ...:     [
-   ...:         fox.data.observation.servo.left_knee.torque,
-   ...:         fox.data.observation.servo.left_wheel.torque,
+   ...:         data.observation.servo.left_knee.torque,
+   ...:         data.observation.servo.left_wheel.torque,
    ...:     ],
    ...:     right=[
-   ...:         fox.data.observation.servo.left_knee.velocity,
-   ...:         fox.data.observation.servo.left_wheel.velocity,
+   ...:         data.observation.servo.left_knee.velocity,
+   ...:         data.observation.servo.left_wheel.velocity,
    ...:     ],
    ...: )
 New tab opened in your web browser! The command line is to produce it directly is:
 
 foxplot upkie_2023-05-03-103245.mpack -l /observation/servo/left_knee/torque /observation/servo/left_wheel/torque -r /observation/servo/left_knee/velocity /observation/servo/left_wheel/velocity
 ```
```

### Comparing `foxplot-0.0.2/docs/conf.py` & `foxplot-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/docs/usage.rst` & `foxplot-0.1.0/docs/usage.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 *****
 Usage
 *****
 
 Interactive mode
 ================
 
-In interactive mode, you can explore the data in ``fox.data`` (tab completion works) and plot it using the ``fox.plot`` function:
+In interactive mode, you can explore the data in ``data`` (tab completion works) and plot it using the ``fox.plot`` function:
 
 .. code:: console
 
     $ foxplot -i upkie_2023-05-03-103245.mpack
     Python 3.8.10 (default, Mar 13 2023, 10:26:41)
     Type 'copyright', 'credits' or 'license' for more information
     IPython 8.0.1 -- An enhanced Interactive Python. Type '?' for help.
 
     In [1]: fox.plot(
        ...:     [
-       ...:         fox.data.observation.servo.left_knee.torque,
-       ...:         fox.data.observation.servo.left_wheel.torque,
+       ...:         data.observation.servo.left_knee.torque,
+       ...:         data.observation.servo.left_wheel.torque,
        ...:     ],
        ...:     right=[
-       ...:         fox.data.observation.servo.left_knee.velocity,
-       ...:         fox.data.observation.servo.left_wheel.velocity,
+       ...:         data.observation.servo.left_knee.velocity,
+       ...:         data.observation.servo.left_wheel.velocity,
        ...:     ],
        ...: )
 
 Plotting from files
 ===================
 
 - JSON: ``foxplot my_data.json -l /observation/cpu_temperature``
```

### Comparing `foxplot-0.0.2/examples/plot_robot_data.py` & `foxplot-0.1.0/examples/plot_robot_data.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/examples/robot_data.json` & `foxplot-0.1.0/examples/robot_data.json`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/__init__.py` & `foxplot-0.1.0/foxplot/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Plot time-series data from line-delimited JSON."""
+"""Custom exceptions."""
 
-__version__ = "0.0.2"
 
-from .fox import Fox
-
-__all__ = ["Fox"]
+class FoxplotException(Exception):
+    """Base class for Foxplot exceptions."""
```

### Comparing `foxplot-0.0.2/foxplot/cli.py` & `foxplot-0.1.0/foxplot/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -84,16 +84,35 @@
     """Entry point for command-line execution."""
     args = parse_command_line_arguments()
 
     fox = Fox(from_file=args.file, time=args.time)
     if args.file is None:
         fox.read_from_json(sys.stdin)
 
-    if args.interactive:
-        __import__("IPython").embed()
+    nothing_to_plot = not args.left and not args.right
+    if args.interactive or nothing_to_plot:
+        usage = (
+            "-" * 68 + "\n\n\n"
+            "Welcome to foxplot!\n\n"
+            "Explore your time series in ``data`` (tab completion works).\n"
+            "When you know what you want, plot time series with:\n\n"
+            "    fox.plot(\n"
+            "        left=[data.foo.bar, data.other.bar],\n"
+            "        right=[data.something.else],\n"
+            "        time=data.timestamp,\n"
+            '        title="My awesome plot",\n'
+            "    )"
+        )
+        __import__("IPython").embed(
+            header=usage,
+            user_ns={
+                "data": fox.data,
+                "fox": fox,
+            },
+        )
     else:  # not args.interactive
         left_labels = args.left if args.left else []
         right_labels = args.right if args.right else []
         left_series = [fox.get_series(label) for label in left_labels]
         right_series = [fox.get_series(label) for label in right_labels]
         fox.plot(
             left_series,
```

### Comparing `foxplot-0.0.2/foxplot/color_picker.py` & `foxplot-0.1.0/foxplot/color_picker.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/decoders/__init__.py` & `foxplot-0.1.0/foxplot/decoders/__init__.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/decoders/json.py` & `foxplot-0.1.0/foxplot/decoders/json.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/decoders/msgpack.py` & `foxplot-0.1.0/foxplot/decoders/msgpack.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/exceptions.py` & `foxplot-0.1.0/foxplot/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -11,12 +11,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Custom exceptions."""
+"""Plot time-series data from line-delimited JSON."""
 
+__version__ = "0.1.0"
 
-class FoxplotException(Exception):
-    """Base class for Foxplot exceptions."""
+from .fox import Fox
+
+__all__ = ["Fox"]
```

### Comparing `foxplot-0.0.2/foxplot/fox.py` & `foxplot-0.1.0/foxplot/fox.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Main class to manipulate dictionary-series data."""
 
 import sys
 import webbrowser
-from typing import BinaryIO, List, Optional, TextIO
+from typing import BinaryIO, List, Optional, TextIO, Union
 
 from .decoders.json import decode_json
 from .decoders.msgpack import decode_msgpack
 from .generate_html import generate_html
 from .indexed_series import IndexedSeries
 from .node import Node
 from .write_tmpfile import write_tmpfile
@@ -32,31 +32,37 @@
 class Fox:
     """Frequent Observation diXionaries, our main class.
 
     Our main class to read, access and manipulate series of dictionary data.
     """
 
     __file: Optional[str]
-    __time: str
+    __time: Optional[str]
     data: Node
     length: int
 
-    def __init__(self, from_file: Optional[str] = None, time: str = ""):
+    def __init__(
+        self,
+        from_file: Optional[str] = None,
+        time: Union[None, str, IndexedSeries] = None,
+    ):
         """Initialize series.
 
         Args:
             from_file: If set, read data from this path.
             time: Label of time index in input dictionaries.
         """
         self.__file = from_file
-        self.__time = time
+        self.__time = None
         self.data = Node("/")
         self.length = 0
         if from_file:
             self.read_from_file(from_file)
+        if time is not None:
+            self.set_time(time)
 
     def get_series(self, label: str) -> IndexedSeries:
         """Get time-series data from a given label.
 
         Args:
             label: Label to the data in input dictionaries, for example
                 ``/observation/cpu_temperature``.
@@ -72,29 +78,33 @@
         """List of all labels present in the data."""
         return self.data._list_labels()
 
     def plot(
         self,
         left: List[IndexedSeries],
         right: Optional[List[IndexedSeries]] = None,
+        time: Union[str, IndexedSeries, None] = None,
         title: str = "",
         left_axis_unit: str = "",
         right_axis_unit: str = "",
         open_new_tab: bool = True,
     ) -> None:
         """Plot a set of indexed series.
 
         Args:
             left: Series to plot on the left axis.
             right: Series to plot on the right axis.
+            time: Time index as a series or its label in input dictionaries.
             title: Plot title.
             left_axis_unit: Unit label for the left axis.
             right_axis_unit: Unit label for the right axis.
             open_new_tab: If true (default), open plot in a new browser tab.
         """
+        if time is not None:
+            self.set_time(time)
         times = (
             self.get_series(self.__time)._get(self.length)
             if self.__time is not None
             else [float(x) for x in range(self.length)]
         )
         left_series = {
             series.label: series._get(self.length) for series in left
@@ -106,30 +116,30 @@
         html = generate_html(
             times,
             left_series,
             right_series,
             title,
             left_axis_unit,
             right_axis_unit,
-            timestamped=self.__time != "",
+            timestamped=self.__time is not None,
         )
 
         if open_new_tab:
             filename = write_tmpfile(html)
             webbrowser.open_new_tab(filename)
             print("New tab opened in your web browser! ", end="")
 
         print("The command line is to produce it directly is:\n")
         left_args = " ".join(left_series.keys())
         right_args = ("-r " if right_series else "") + " ".join(
             right_series.keys()
         )
         file = f"{self.__file} " if self.__file is not None else ""
-        time = f"-t {self.__time} " if self.__time else ""
-        print(f"foxplot {file}{time}-l {left_args} {right_args}")
+        timestamp = f"-t {self.__time} " if self.__time is not None else ""
+        print(f"foxplot {file}{timestamp}-l {left_args} {right_args}")
 
     def read_from_file(self, filename: str) -> None:
         """Process time series data.
 
         Args:
             filename: Name of a file to read time series from.
         """
@@ -156,21 +166,22 @@
 
         Args:
             file: MessagePack stream to read time series from.
         """
         for unpacked in decode_msgpack(file=file):
             self.unpack(unpacked)
 
-    def set_time(self, time: str):
+    def set_time(self, time: Union[str, IndexedSeries]):
         """Set label of time index in input dictionaries.
 
         Args:
-            time: Label of time index in input dictionaries.
+            time: Time index as a series or its label in input dictionaries.
         """
-        self.__time = time
+        label = time.label if isinstance(time, IndexedSeries) else time
+        self.__time = label
 
     def unpack(self, unpacked: dict) -> None:
         """Append data from an unpacked dictionary.
 
         Args:
             unpacked: Unpacked dictionary.
         """
```

### Comparing `foxplot-0.0.2/foxplot/generate_html.py` & `foxplot-0.1.0/foxplot/generate_html.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/indexed_series.py` & `foxplot-0.1.0/foxplot/indexed_series.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/node.py` & `foxplot-0.1.0/foxplot/node.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/uPlot/uPlot.iife.js` & `foxplot-0.1.0/foxplot/uPlot/uPlot.iife.js`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/uPlot/uPlot.min.css` & `foxplot-0.1.0/foxplot/uPlot/uPlot.min.css`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/uPlot/uPlot.mousewheel.js` & `foxplot-0.1.0/foxplot/uPlot/uPlot.mousewheel.js`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/foxplot/write_tmpfile.py` & `foxplot-0.1.0/foxplot/write_tmpfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,9 +35,9 @@
     with tempfile.NamedTemporaryFile(
         mode="w+",
         prefix=f"plot-{datetime.now().strftime('%Y%m%d-%H%M%S')}-",
         suffix=".html",
         delete=False,
     ) as output_file:
         output_file.write(html)
-        filename = output_file.name
+        filename = f"file://{output_file.name}"
     return filename
```

### Comparing `foxplot-0.0.2/pyproject.toml` & `foxplot-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 dependencies = [
+    "ipython",
     "msgpack",
 ]
 keywords = ["json", "time", "series", "plot"]
 
 [project.scripts]
 foxplot = "foxplot.cli:main"
```

### Comparing `foxplot-0.0.2/tests/test_color_picker.py` & `foxplot-0.1.0/tests/test_color_picker.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/tests/test_decoders.py` & `foxplot-0.1.0/tests/test_decoders.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/tests/test_fox.py` & `foxplot-0.1.0/tests/test_fox.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/tests/test_generate_html.py` & `foxplot-0.1.0/tests/test_generate_html.py`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/tox.ini` & `foxplot-0.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `foxplot-0.0.2/PKG-INFO` & `foxplot-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxplot
-Version: 0.0.2
+Version: 0.1.0
 Summary: Plot time-series data from line-delimited JSON.
 Keywords: json,time,series,plot
 Author-email: Stéphane Caron <stephane.caron@normalesup.org>
 Maintainer-email: Stéphane Caron <stephane.caron@normalesup.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
@@ -12,54 +12,55 @@
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Dist: ipython
 Requires-Dist: msgpack
 Project-URL: Changelog, https://github.com/stephane-caron/foxplot/blob/master/CHANGELOG.md
 Project-URL: Source, https://github.com/stephane-caron/foxplot
 Project-URL: Tracker, https://github.com/stephane-caron/foxplot/issues
 
 # foxplot
 
 [![Build](https://img.shields.io/github/actions/workflow/status/stephane-caron/foxplot/CI.yml?branch=main)](https://github.com/stephane-caron/foxplot/actions)
 [![Documentation](https://img.shields.io/github/actions/workflow/status/stephane-caron/foxplot/docs.yml?branch=main&label=docs)](https://stephane-caron.github.io/foxplot/)
 
-Plot time-series data from [line-delimited JSON](https://en.wikipedia.org/wiki/JSON_streaming#Line-delimited_JSON).
+Plot time-series data from [newline-delimited JSON](https://en.wikipedia.org/wiki/JSON_streaming#Newline-delimited-JSON).
 
 Foxplot stands for "Frequent Observation diXionary plots". Frequent observations arise from the project's initial use case (robotic control loops). Dictionaries are the observation format used in [Vulp](https://github.com/tasts-robots/vulp). Plots are plots :wink:
 
 ## Installation
 
 ```console
 $ pip install foxplot
 ```
 
 ## Usage
 
 ### Interactive mode
 
-In interactive mode, you can explore the data in ``fox.data`` (tab completion works) and plot it using the ``fox.plot`` function:
+In interactive mode, you can explore the data in ``data`` (tab completion works) and plot it using the ``fox.plot`` function:
 
 ```python
 $ foxplot -i upkie_2023-05-03-103245.mpack
 Python 3.8.10 (default, Mar 13 2023, 10:26:41)
 Type 'copyright', 'credits' or 'license' for more information
 IPython 8.0.1 -- An enhanced Interactive Python. Type '?' for help.
 
 In [1]: fox.plot(
    ...:     [
-   ...:         fox.data.observation.servo.left_knee.torque,
-   ...:         fox.data.observation.servo.left_wheel.torque,
+   ...:         data.observation.servo.left_knee.torque,
+   ...:         data.observation.servo.left_wheel.torque,
    ...:     ],
    ...:     right=[
-   ...:         fox.data.observation.servo.left_knee.velocity,
-   ...:         fox.data.observation.servo.left_wheel.velocity,
+   ...:         data.observation.servo.left_knee.velocity,
+   ...:         data.observation.servo.left_wheel.velocity,
    ...:     ],
    ...: )
 New tab opened in your web browser! The command line is to produce it directly is:
 
 foxplot upkie_2023-05-03-103245.mpack -l /observation/servo/left_knee/torque /observation/servo/left_wheel/torque -r /observation/servo/left_knee/velocity /observation/servo/left_wheel/velocity
 ```
```

