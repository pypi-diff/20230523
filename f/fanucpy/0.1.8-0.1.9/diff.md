# Comparing `tmp/fanucpy-0.1.8.tar.gz` & `tmp/fanucpy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fanucpy-0.1.8.tar", max compression
+gzip compressed data, was "fanucpy-0.1.9.tar", max compression
```

## Comparing `fanucpy-0.1.8.tar` & `fanucpy-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2022-12-21 12:47:59.697290 fanucpy-0.1.8/LICENSE
--rw-r--r--   0        0        0     2915 2022-12-21 12:47:59.697427 fanucpy-0.1.8/README.md
--rw-r--r--   0        0        0      561 2023-01-09 14:22:06.825834 fanucpy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     7484 2022-12-21 12:51:24.783633 fanucpy-0.1.8/src/fanucpy/Calibration.py
--rw-r--r--   0        0        0     7292 2022-12-21 12:55:47.150768 fanucpy-0.1.8/src/fanucpy/Robot.py
--rw-r--r--   0        0        0      946 2022-12-21 12:56:13.139343 fanucpy-0.1.8/src/fanucpy/RobotApp.py
--rw-r--r--   0        0        0      879 2022-12-21 12:47:59.700793 fanucpy-0.1.8/src/fanucpy/Transformations.py
--rw-r--r--   0        0        0       55 2022-12-21 12:47:59.700884 fanucpy-0.1.8/src/fanucpy/__init__.py
--rw-r--r--   0        0        0     3805 1970-01-01 00:00:00.000000 fanucpy-0.1.8/setup.py
--rw-r--r--   0        0        0     3712 1970-01-01 00:00:00.000000 fanucpy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-12-21 12:47:59.697290 fanucpy-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3239 2023-01-13 11:46:31.064813 fanucpy-0.1.9/README.md
+-rw-r--r--   0        0        0      561 2023-01-13 11:46:31.065000 fanucpy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     7484 2022-12-21 12:51:24.783633 fanucpy-0.1.9/src/fanucpy/Calibration.py
+-rw-r--r--   0        0        0     7967 2023-01-13 11:46:31.066117 fanucpy-0.1.9/src/fanucpy/Robot.py
+-rw-r--r--   0        0        0      946 2022-12-21 12:56:13.139343 fanucpy-0.1.9/src/fanucpy/RobotApp.py
+-rw-r--r--   0        0        0      879 2022-12-21 12:47:59.700793 fanucpy-0.1.9/src/fanucpy/Transformations.py
+-rw-r--r--   0        0        0       55 2022-12-21 12:47:59.700884 fanucpy-0.1.9/src/fanucpy/__init__.py
+-rw-r--r--   0        0        0     4147 1970-01-01 00:00:00.000000 fanucpy-0.1.9/setup.py
+-rw-r--r--   0        0        0     4036 1970-01-01 00:00:00.000000 fanucpy-0.1.9/PKG-INFO
```

### Comparing `fanucpy-0.1.8/LICENSE` & `fanucpy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fanucpy-0.1.8/README.md` & `fanucpy-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,32 @@
 # get robot state
 print(f"Current pose: {robot.get_curpos()}")
 print(f"Current joints: {robot.get_curjpos()}")
 print(f"Instantaneous power: {robot.get_ins_power()}")
 print(f"Get gripper state: {robot.get_rdo(7)}")
 ```
 
+### Calling external program
+```python
+robot.call_prog(prog_name)
+```
+
+### Get/Set RDO
+```python
+robot.get_rdo(rdo_num=7)
+robot.set_rdo(rdo_num=7, value=True)
+```
+
+## Contributions
+External contributions are welcome!
+
+- Agajan Torayev: Key developer
+- Fan Mo: Support with documentation
+- Michael Yiu: External contributor
+
 
 ## RobotApp
 We introduce an experimental feature: Robot Apps. This class facilitates modularity and plug-and-produce functionality. Check the following example apps:
 
 1. [Pick and Place App](examples/PickAndPlaceApp.py)
 1. [Aruco Tracking App](examples/ArucoTrackingApp.py)
```

### Comparing `fanucpy-0.1.8/pyproject.toml` & `fanucpy-0.1.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fanucpy"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python package for FANUC industrial robots"
 authors = ["Agajan Torayev <torayeff@gmail.com>"]
 repository = "https://github.com/torayeff/fanucpy"
 readme = 'README.md'
 keywords = ["fanuc", "industrial robot", "robotic apps"]
 license = "Apache License 2.0"
```

### Comparing `fanucpy-0.1.8/src/fanucpy/Calibration.py` & `fanucpy-0.1.9/src/fanucpy/Calibration.py`

 * *Files identical despite different names*

### Comparing `fanucpy-0.1.8/src/fanucpy/Robot.py` & `fanucpy-0.1.9/src/fanucpy/Robot.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self.sock_buff_sz = 1024
         self.socket_timeout = socket_timeout
         self.comm_sock = None
         self.SUCCESS_CODE = 0
         self.ERROR_CODE = 1
 
     def __version__(self):
-        print("MAPPDK Robot class v0.1.1")
+        print("MAPPDK Robot class v0.1.9")
 
     def handle_response(self, resp: str, verbose: bool = False):
         """Handles response from socket communication.
 
         Args:
             resp (str): Response string returned from socket.
             verbose (bool, optional): [description]. Defaults to False.
@@ -240,7 +240,35 @@
         Returns:
             rdo_value: RDO value.
         """
         cmd = f"getrdo:{rdo_num}"
         _, rdo_value = self.send_cmd(cmd)
         rdo_value = int(rdo_value)
         return rdo_value
+
+    def set_rdo(self, rdo_num: int, val: bool):
+        """Sets RDO value.
+
+        Args:
+            rdo_num (int): RDO number.
+            val (bool): Value.
+        """
+        if val:
+            val = "true"
+        else:
+            val = "false"
+        cmd = f"setrdo:{rdo_num}:{val}"
+        self.send_cmd(cmd)
+
+    def set_sys_var(self, sys_var: str, val: bool):
+        """Sets system variable to True or False.
+
+        Args:
+            sys_var (str): System variable name.
+            val (bool): Value.
+        """
+        if val:
+            val = "T"
+        else:
+            val = "F"
+        cmd = f"setsysvar:{sys_var}:{val}"
+        self.send_cmd(cmd)
```

### Comparing `fanucpy-0.1.8/src/fanucpy/RobotApp.py` & `fanucpy-0.1.9/src/fanucpy/RobotApp.py`

 * *Files identical despite different names*

### Comparing `fanucpy-0.1.8/src/fanucpy/Transformations.py` & `fanucpy-0.1.9/src/fanucpy/Transformations.py`

 * *Files identical despite different names*

### Comparing `fanucpy-0.1.8/setup.py` & `fanucpy-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 install_requires = \
 ['numpy>=1.22.3,<2.0.0',
  'opencv-contrib-python>=4.5.5,<5.0.0',
  'scipy>=1.8.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'fanucpy',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Python package for FANUC industrial robots',
-    'long_description': '# fanucpy: Python package for FANUC industrial robots\n\n## Acknowledgements\nThis work was developed at the [Institute for Advanced Manufacturing at the University of Nottingham](https://www.nottingham.ac.uk/ifam/index.aspx) as a part of the [Digital Manufacturing and Design Training Network](https://dimanditn.eu/).\n\nThis project has received funding from the European Union’s Horizon 2020 research and innovation programme under the Marie Skłodowska-Curie grant agreement No 814078.\n\n## Software contents\nThe package consists of two parts: \n1. Robot interface code written in Python programming language\n2. FANUC robot controller driver (tested with R-30iB Mate Plus Controller) written in KAREL and FANUC teach pendant languages\n\nThe communication protocol between the Python package and the FANUC robot controller is depicted below:\n![Communication Protocol](https://github.com/torayeff/fanucpy/raw/main/media/CommProtocol.png)\n\n## Python package installation\n```bash\npip install fanucpy\n```\n\n## Driver installation\nFollow these [steps](https://github.com/torayeff/fanucpy/blob/main/fanuc.md) to install FANUC driver.\n\n## Usage\n### Connect to a robot:\n```python\nfrom fanucpy import Robot\n\nrobot = Robot(\n    robot_model="Fanuc",\n    host="192.168.1.100",\n    port=18735,\n    ee_DO_type="RDO",\n    ee_DO_num=7,\n)\n\nrobot.connect()\n```\n\n### Moving\n```python\n# move in joint space\nrobot.move(\n    "joint",\n    vals=[19.0, 66.0, -33.0, 18.0, -30.0, -33.0],\n    velocity=100,\n    acceleration=100,\n    cnt_val=0,\n    linear=False\n)\n\n# move in cartesian space\nrobot.move(\n    "pose",\n    vals=[0.0, -28.0, -35.0, 0.0, -55.0, 0.0],\n    velocity=50,\n    acceleration=50,\n    cnt_val=0,\n    linear=False\n)\n```\n\n### Opening/closing gripper\n```Python\n# open gripper\nrobot.gripper(True)\n\n# close gripper\nrobot.gripper(False)\n```\n\n### Querying robot state\n```python\n# get robot state\nprint(f"Current pose: {robot.get_curpos()}")\nprint(f"Current joints: {robot.get_curjpos()}")\nprint(f"Instantaneous power: {robot.get_ins_power()}")\nprint(f"Get gripper state: {robot.get_rdo(7)}")\n```\n\n\n## RobotApp\nWe introduce an experimental feature: Robot Apps. This class facilitates modularity and plug-and-produce functionality. Check the following example apps:\n\n1. [Pick and Place App](examples/PickAndPlaceApp.py)\n1. [Aruco Tracking App](examples/ArucoTrackingApp.py)\n\n## Citation\nPlease use the following to cite if you are using this library in academic publications [Towards Modular and Plug-and-Produce Manufacturing Apps](https://www.sciencedirect.com/science/article/pii/S2212827122004255)\n```\n@article{torayev2022towards,\n  title={Towards Modular and Plug-and-Produce Manufacturing Apps},\n  author={Torayev, Agajan and Mart{\\\'\\i}nez-Arellano, Giovanna and Chaplin, Jack C and Sanderson, David and Ratchev, Svetan},\n  journal={Procedia CIRP},\n  volume={107},\n  pages={1257--1262},\n  year={2022},\n  publisher={Elsevier}\n}\n```\n',
+    'long_description': '# fanucpy: Python package for FANUC industrial robots\n\n## Acknowledgements\nThis work was developed at the [Institute for Advanced Manufacturing at the University of Nottingham](https://www.nottingham.ac.uk/ifam/index.aspx) as a part of the [Digital Manufacturing and Design Training Network](https://dimanditn.eu/).\n\nThis project has received funding from the European Union’s Horizon 2020 research and innovation programme under the Marie Skłodowska-Curie grant agreement No 814078.\n\n## Software contents\nThe package consists of two parts: \n1. Robot interface code written in Python programming language\n2. FANUC robot controller driver (tested with R-30iB Mate Plus Controller) written in KAREL and FANUC teach pendant languages\n\nThe communication protocol between the Python package and the FANUC robot controller is depicted below:\n![Communication Protocol](https://github.com/torayeff/fanucpy/raw/main/media/CommProtocol.png)\n\n## Python package installation\n```bash\npip install fanucpy\n```\n\n## Driver installation\nFollow these [steps](https://github.com/torayeff/fanucpy/blob/main/fanuc.md) to install FANUC driver.\n\n## Usage\n### Connect to a robot:\n```python\nfrom fanucpy import Robot\n\nrobot = Robot(\n    robot_model="Fanuc",\n    host="192.168.1.100",\n    port=18735,\n    ee_DO_type="RDO",\n    ee_DO_num=7,\n)\n\nrobot.connect()\n```\n\n### Moving\n```python\n# move in joint space\nrobot.move(\n    "joint",\n    vals=[19.0, 66.0, -33.0, 18.0, -30.0, -33.0],\n    velocity=100,\n    acceleration=100,\n    cnt_val=0,\n    linear=False\n)\n\n# move in cartesian space\nrobot.move(\n    "pose",\n    vals=[0.0, -28.0, -35.0, 0.0, -55.0, 0.0],\n    velocity=50,\n    acceleration=50,\n    cnt_val=0,\n    linear=False\n)\n```\n\n### Opening/closing gripper\n```Python\n# open gripper\nrobot.gripper(True)\n\n# close gripper\nrobot.gripper(False)\n```\n\n### Querying robot state\n```python\n# get robot state\nprint(f"Current pose: {robot.get_curpos()}")\nprint(f"Current joints: {robot.get_curjpos()}")\nprint(f"Instantaneous power: {robot.get_ins_power()}")\nprint(f"Get gripper state: {robot.get_rdo(7)}")\n```\n\n### Calling external program\n```python\nrobot.call_prog(prog_name)\n```\n\n### Get/Set RDO\n```python\nrobot.get_rdo(rdo_num=7)\nrobot.set_rdo(rdo_num=7, value=True)\n```\n\n## Contributions\nExternal contributions are welcome!\n\n- Agajan Torayev: Key developer\n- Fan Mo: Support with documentation\n- Michael Yiu: External contributor\n\n\n## RobotApp\nWe introduce an experimental feature: Robot Apps. This class facilitates modularity and plug-and-produce functionality. Check the following example apps:\n\n1. [Pick and Place App](examples/PickAndPlaceApp.py)\n1. [Aruco Tracking App](examples/ArucoTrackingApp.py)\n\n## Citation\nPlease use the following to cite if you are using this library in academic publications [Towards Modular and Plug-and-Produce Manufacturing Apps](https://www.sciencedirect.com/science/article/pii/S2212827122004255)\n```\n@article{torayev2022towards,\n  title={Towards Modular and Plug-and-Produce Manufacturing Apps},\n  author={Torayev, Agajan and Mart{\\\'\\i}nez-Arellano, Giovanna and Chaplin, Jack C and Sanderson, David and Ratchev, Svetan},\n  journal={Procedia CIRP},\n  volume={107},\n  pages={1257--1262},\n  year={2022},\n  publisher={Elsevier}\n}\n```\n',
     'author': 'Agajan Torayev',
     'author_email': 'torayeff@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/torayeff/fanucpy',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `fanucpy-0.1.8/PKG-INFO` & `fanucpy-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fanucpy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package for FANUC industrial robots
 Home-page: https://github.com/torayeff/fanucpy
 License: Apache-2.0
 Keywords: fanuc,industrial robot,robotic apps
 Author: Agajan Torayev
 Author-email: torayeff@gmail.com
 Requires-Python: >=3.8,<3.11
@@ -95,14 +95,32 @@
 # get robot state
 print(f"Current pose: {robot.get_curpos()}")
 print(f"Current joints: {robot.get_curjpos()}")
 print(f"Instantaneous power: {robot.get_ins_power()}")
 print(f"Get gripper state: {robot.get_rdo(7)}")
 ```
 
+### Calling external program
+```python
+robot.call_prog(prog_name)
+```
+
+### Get/Set RDO
+```python
+robot.get_rdo(rdo_num=7)
+robot.set_rdo(rdo_num=7, value=True)
+```
+
+## Contributions
+External contributions are welcome!
+
+- Agajan Torayev: Key developer
+- Fan Mo: Support with documentation
+- Michael Yiu: External contributor
+
 
 ## RobotApp
 We introduce an experimental feature: Robot Apps. This class facilitates modularity and plug-and-produce functionality. Check the following example apps:
 
 1. [Pick and Place App](examples/PickAndPlaceApp.py)
 1. [Aruco Tracking App](examples/ArucoTrackingApp.py)
```

