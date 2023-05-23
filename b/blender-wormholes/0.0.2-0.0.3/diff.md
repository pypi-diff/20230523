# Comparing `tmp/blender_wormholes-0.0.2.tar.gz` & `tmp/blender_wormholes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blender_wormholes-0.0.2.tar", last modified: Sun Aug 21 09:03:03 2022, max compression
+gzip compressed data, was "blender_wormholes-0.0.3.tar", last modified: Tue May 23 14:59:32 2023, max compression
```

## Comparing `blender_wormholes-0.0.2.tar` & `blender_wormholes-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 coreqode  (1000) coreqode  (1000)        0 2022-08-21 09:03:03.637084 blender_wormholes-0.0.2/
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)      435 2022-08-21 09:03:03.637084 blender_wormholes-0.0.2/PKG-INFO
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)       48 2022-08-21 08:34:42.000000 blender_wormholes-0.0.2/README.md
-drwxrwxr-x   0 coreqode  (1000) coreqode  (1000)        0 2022-08-21 09:03:03.637084 blender_wormholes-0.0.2/blender_wormholes/
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)       65 2022-08-21 08:34:53.000000 blender_wormholes-0.0.2/blender_wormholes/__init__.py
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)      224 2022-08-21 08:34:53.000000 blender_wormholes-0.0.2/blender_wormholes/constants.py
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)      925 2022-08-21 08:34:53.000000 blender_wormholes-0.0.2/blender_wormholes/constraints.py
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)    16214 2022-08-21 08:34:53.000000 blender_wormholes-0.0.2/blender_wormholes/core.py
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)     1472 2022-08-21 08:34:53.000000 blender_wormholes-0.0.2/blender_wormholes/utility.py
-drwxrwxr-x   0 coreqode  (1000) coreqode  (1000)        0 2022-08-21 09:03:03.637084 blender_wormholes-0.0.2/blender_wormholes.egg-info/
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)      435 2022-08-21 09:03:03.000000 blender_wormholes-0.0.2/blender_wormholes.egg-info/PKG-INFO
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)      415 2022-08-21 09:03:03.000000 blender_wormholes-0.0.2/blender_wormholes.egg-info/SOURCES.txt
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)        1 2022-08-21 09:03:03.000000 blender_wormholes-0.0.2/blender_wormholes.egg-info/dependency_links.txt
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)       55 2022-08-21 09:03:03.000000 blender_wormholes-0.0.2/blender_wormholes.egg-info/entry_points.txt
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)        1 2022-08-21 09:03:03.000000 blender_wormholes-0.0.2/blender_wormholes.egg-info/not-zip-safe
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)       18 2022-08-21 09:03:03.000000 blender_wormholes-0.0.2/blender_wormholes.egg-info/top_level.txt
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)       38 2022-08-21 09:03:03.637084 blender_wormholes-0.0.2/setup.cfg
--rw-rw-r--   0 coreqode  (1000) coreqode  (1000)      889 2022-08-21 09:01:18.000000 blender_wormholes-0.0.2/setup.py
+drwxr-xr-x   0 coreqode  (1001) coreqode  (1002)        0 2023-05-23 14:59:32.421213 blender_wormholes-0.0.3/
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)      423 2023-05-23 14:59:32.421213 blender_wormholes-0.0.3/PKG-INFO
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)       48 2023-05-23 10:07:48.000000 blender_wormholes-0.0.3/README.md
+drwxr-xr-x   0 coreqode  (1001) coreqode  (1002)        0 2023-05-23 14:59:32.421213 blender_wormholes-0.0.3/blender_wormholes/
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)       65 2023-05-23 10:07:48.000000 blender_wormholes-0.0.3/blender_wormholes/__init__.py
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)      224 2023-05-23 10:07:48.000000 blender_wormholes-0.0.3/blender_wormholes/constants.py
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)      925 2023-05-23 10:07:48.000000 blender_wormholes-0.0.3/blender_wormholes/constraints.py
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)    16544 2023-05-23 13:24:57.000000 blender_wormholes-0.0.3/blender_wormholes/core.py
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)     1472 2023-05-23 10:07:48.000000 blender_wormholes-0.0.3/blender_wormholes/utility.py
+drwxr-xr-x   0 coreqode  (1001) coreqode  (1002)        0 2023-05-23 14:59:32.421213 blender_wormholes-0.0.3/blender_wormholes.egg-info/
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)      423 2023-05-23 14:59:32.000000 blender_wormholes-0.0.3/blender_wormholes.egg-info/PKG-INFO
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)      415 2023-05-23 14:59:32.000000 blender_wormholes-0.0.3/blender_wormholes.egg-info/SOURCES.txt
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)        1 2023-05-23 14:59:32.000000 blender_wormholes-0.0.3/blender_wormholes.egg-info/dependency_links.txt
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)       55 2023-05-23 14:59:32.000000 blender_wormholes-0.0.3/blender_wormholes.egg-info/entry_points.txt
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)        1 2023-05-23 14:59:32.000000 blender_wormholes-0.0.3/blender_wormholes.egg-info/not-zip-safe
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)       18 2023-05-23 14:59:32.000000 blender_wormholes-0.0.3/blender_wormholes.egg-info/top_level.txt
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)       38 2023-05-23 14:59:32.421213 blender_wormholes-0.0.3/setup.cfg
+-rw-r--r--   0 coreqode  (1001) coreqode  (1002)      877 2023-05-23 14:59:30.000000 blender_wormholes-0.0.3/setup.py
```

### Comparing `blender_wormholes-0.0.2/blender_wormholes/constraints.py` & `blender_wormholes-0.0.3/blender_wormholes/constraints.py`

 * *Files identical despite different names*

### Comparing `blender_wormholes-0.0.2/blender_wormholes/core.py` & `blender_wormholes-0.0.3/blender_wormholes/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,42 +5,51 @@
 from mathutils import Matrix, Vector
 from .constants import SHADER_NODE_TYPE
 
 
 class Scene:
     def __init__(self):
         self.scene = bpy.context.scene
-
+        
     def initialize_image_settings(self, settings):
         self.scene.render.resolution_x = settings['resolution'][0]
         self.scene.render.resolution_y = settings['resolution'][1]
         self.scene.render.filepath = settings['output_path']
+        self.scene.render.image_settings.file_format = settings['file_format']
+        self.scene.render.film_transparent = settings['film_transparent'] 
 
     def initialize_rendering_settings(self, settings):
         self.scene.render.engine = settings['engine']
         self.scene.cycles.progressive = settings['engine_type']
         self.scene.cycles.use_adaptive_sampling = settings['use_adaptive_sampling']
         self.scene.cycles.max_bounces = settings['max_bounces']
         self.scene.cycles.samples = settings['sample_size']
 
     def add_objects(self, filepath):
-        bpy.ops.import_scene.obj(filepath=filepath, split_mode='OFF')
+        old_objs = set(self.scene.objects)
+        if '.obj' in filepath:
+                bpy.ops.import_scene.obj(filepath=filepath, split_mode='OFF')
+        elif '.ply' in filepath:
+                bpy.ops.import_mesh.ply(filepath = filepath)
         bpy.ops.object.origin_set(type='ORIGIN_GEOMETRY')
-        name = filepath.split('/')[-1].split('.')[0]
-        return Object(name)
+        imported_objs = set(self.scene.objects) - old_objs
+        name = list(imported_objs)[0].name
+        return Object(obj_name = name)
 
     def delete_objects(self, obj_name):
         self.deselect_all()
         self.select_object(obj_name)
         bpy.ops.object.delete()
 
     def set_camera(self):
         pass
 
-    def render(self, animation=False):
+    def render(self, path = None, animation=False):
+        if path is not None:
+            self.scene.render.filepath = path
         bpy.ops.render.render(write_still=True, animation=animation)
 
     def current_mode(self):
         return self.obj.mode
 
     def toggle_mode_to(self, mode):
         bpy.ops.object.mode_set(mode=mode)
@@ -58,23 +67,14 @@
         self.toggle_mode_to('POSE')
         self.armature.bones[bone].select = True
 
     def deselect_all(self):
         bpy.ops.object.select_all(action='DESELECT')
         bpy.context.view_layer.objects.active = None
 
-    # def add_lights_to_scene(self):
-    #     mat = self.smplx_indices['lights_matrix_world']['light_1']
-    #     bpy.ops.object.light_add(type='POINT', radius=1, align='WORLD')
-    #     light_1 = bpy.data.objects['Point']
-    #     light_1.matrix_world = Matrix(mat)
-    #     light_1.name = 'light_1'
-    #     light_1.data.energy = 20
-    #     light_1.data.color = (1, 0.701487, 0.278857)
-
     def apply_hdri(self, image_path):
         self.env_texture_node.image = bpy.data.images.load(image_path)
         self.mapping_node.inputs[2].default_value[2] = random.randint(
             -180, 180)
         bpy.context.view_layer.update()
 
     def create_world_shader_nodes(self):
@@ -242,37 +242,43 @@
                     a = ((c_x - x) / f_x)
                     z[y][x] = val / np.linalg.norm([1, a, b])
         os.remove(tmp_file_path)
         return z
 
 
 class Object:
-    def __init__(self, obj_name):
+    def __init__(self, obj_name = None, obj_path = None):
         self.name = obj_name
         self.obj = bpy.data.objects[self.name]
         self.mode = self.obj.mode
 
     def select_object(self):
         bpy.context.view_layer.objects.active = self.obj
 
     def visibility(self, hide=True):
         if hide:
             self.obj.hide_render = True
         else:
             self.obj.hide_render = False
 
     def link_material(self, mat):
-        self.obj.data.materials[0] = mat
+        if self.obj.data.materials:
+            self.obj.data.materials[0] = mat
+        else:
+            self.obj.data.materials.append(mat)
 
     def rotate(self, angle, axis):
         self.obj.rotation_euler[axis] = angle
 
     def scale(self, value):
         self.obj.scale = (value[0], value[1], value[2])
 
+    def translate(self, value):
+        self.obj.location = (value[0], value[1], value[2])
+
     def add_keyframe(self, data_path, frame):
         self.obj.keyframe_insert(data_path=data_path, frame=frame)
 
     def remove_keyframe(self, data_path, frame):
         self.obj.keyframe_delete(data_path=data_path, frame=frame)
 
     def uv_parameterize(self, type):
@@ -331,17 +337,17 @@
         self.node_names.append(tar_name)
 
 
 class Camera:
     def __init__(self, name=None):
         if name:
             self.name = name
+            self.camera = bpy.data.objects[self.name]
         else:
-            self.name = 'camera'
-        self.camera = None
+            self.add_camera()
 
     def add_camera(self,  matrix=None, lens=None):
         bpy.ops.object.camera_add(enter_editmode=False, align="WORLD")
 
         if lens:
             bpy.context.object.data.lens = lens
 
@@ -416,8 +422,8 @@
         return RT_blender, extr
 
     def get_camera_parameters(self, scene):
         bpy.context.view_layer.update()
         K = self.get_intrinsic_camera_parameters(scene)
         RT_blender, RT_cv = self.get_extrinsic_camera_parameters(scene)
         P = np.matmul(K, RT_cv)
-        return P, K, RT_cv, RT_blender
+        return P, K, RT_cv, RT_blender
```

### Comparing `blender_wormholes-0.0.2/blender_wormholes/utility.py` & `blender_wormholes-0.0.3/blender_wormholes/utility.py`

 * *Files identical despite different names*

### Comparing `blender_wormholes-0.0.2/setup.py` & `blender_wormholes-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
 	requirements = f.readlines()
 
-long_description = 'High-Level API for Blender'
+long_description = 'helper library'
 
 setup(
 		name ='blender_wormholes',
-		version ='0.0.2',
+		version ='0.0.3',
 		author ='Chandradeep Pokhariya',
 		author_email ='cdpokhariya@gmail.com',
 		url ='https://github.com/coreqode/blender_wormholes',
 		description ='helper library',
 		long_description = long_description,
 		long_description_content_type ="text/markdown",
 		license ='MIT',
```

