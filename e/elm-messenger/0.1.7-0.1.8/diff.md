# Comparing `tmp/elm-messenger-0.1.7.tar.gz` & `tmp/elm-messenger-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.1.7.tar", last modified: Sun May 21 09:28:54 2023, max compression
+gzip compressed data, was "elm-messenger-0.1.8.tar", last modified: Tue May 23 09:13:19 2023, max compression
```

## Comparing `elm-messenger-0.1.7.tar` & `elm-messenger-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-21 09:28:54.119096 elm-messenger-0.1.7/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.7/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-21 09:28:54.119096 elm-messenger-0.1.7/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.7/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-21 09:28:54.119096 elm-messenger-0.1.7/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-21 09:28:54.000000 elm-messenger-0.1.7/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-21 09:28:54.119096 elm-messenger-0.1.7/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.7/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.7/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)    16909 2023-05-21 09:26:59.000000 elm-messenger-0.1.7/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.1.7/messengercli/updater.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-21 09:28:54.119096 elm-messenger-0.1.7/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.7/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-23 09:13:19.499624 elm-messenger-0.1.8/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.8/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-23 09:13:19.499624 elm-messenger-0.1.8/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.8/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-23 09:13:19.499624 elm-messenger-0.1.8/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      368 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-23 09:13:19.000000 elm-messenger-0.1.8/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-23 09:13:19.499624 elm-messenger-0.1.8/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.8/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.8/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)    17530 2023-05-22 06:39:53.000000 elm-messenger-0.1.8/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)     1170 2023-05-12 14:41:01.000000 elm-messenger-0.1.8/messengercli/updater.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-23 09:13:19.499624 elm-messenger-0.1.8/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.8/setup.py
```

### Comparing `elm-messenger-0.1.7/messengercli/messenger.py` & `elm-messenger-0.1.8/messengercli/messenger.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import typer
 import os
 import shutil
 import json
 from .updater import Updater
 
 app = typer.Typer(add_completion=False, help="Messenger CLI")
-API_VERSION = "0.1.7"
+API_VERSION = "0.1.8"
 
 
 class Messenger:
     config = None
 
     def __init__(self) -> None:
         """
@@ -268,25 +268,28 @@
 
     def add_gamecomponent(self, sceneproto: str, gc: str):
         """
         Add a GameComponent to a SceneProto
         """
         if sceneproto not in self.config["sceneprotos"]:
             raise Exception("SceneProto doesn't exist.")
-        
+
         os.mkdir(f"src/SceneProtos/{sceneproto}/GameComponents/{gc}")
-        Updater([
-            ".messenger/sceneproto/gamecomponent/Sample/Base.elm",
-            ".messenger/sceneproto/gamecomponent/Sample/Export.elm",
-            ".messenger/sceneproto/gamecomponent/Sample/Model.elm",
-        ],[
-            f"src/SceneProtos/{sceneproto}/GameComponents/{gc}/Base.elm",
-            f"src/SceneProtos/{sceneproto}/GameComponents/{gc}/Export.elm",
-            f"src/SceneProtos/{sceneproto}/GameComponents/{gc}/Model.elm"
-        ]).rep(sceneproto).rep(gc)
+        Updater(
+            [
+                ".messenger/sceneproto/gamecomponent/Sample/Base.elm",
+                ".messenger/sceneproto/gamecomponent/Sample/Export.elm",
+                ".messenger/sceneproto/gamecomponent/Sample/Model.elm",
+            ],
+            [
+                f"src/SceneProtos/{sceneproto}/GameComponents/{gc}/Base.elm",
+                f"src/SceneProtos/{sceneproto}/GameComponents/{gc}/Export.elm",
+                f"src/SceneProtos/{sceneproto}/GameComponents/{gc}/Model.elm",
+            ],
+        ).rep(sceneproto).rep(gc)
 
         # Modify GameComponent
         with open(f"src/SceneProtos/{sceneproto}/GameComponent/Base.elm", "r") as f:
             scenebase = f.read()
         new_scenebase = scenebase.replace(
             "type GameComponentInitData\n    =",
             f"type GameComponentInitData\n    = GC{gc}InitData {gc}Init\n    |",
@@ -296,15 +299,15 @@
         )
         with open(f"src/SceneProtos/{sceneproto}/GameComponent/Base.elm", "w") as f:
             f.write(new_scenebase)
 
     def format(self):
         os.system("elm-format src/ --yes")
 
-    def add_layer(self, scene: str, layer: str):
+    def add_layer(self, scene: str, layer: str, has_component: bool):
         """
         Add a layer to a scene
         """
         if scene not in self.config["scenes"]:
             raise Exception("Scene doesn't exist.")
         if layer in self.config["scenes"][scene]:
             raise Exception("Layer already exists.")
@@ -322,14 +325,25 @@
             [
                 f"src/Scenes/{scene}/{layer}/Model.elm",
                 f"src/Scenes/{scene}/{layer}/Global.elm",
                 f"src/Scenes/{scene}/{layer}/Export.elm",
                 f"src/Scenes/{scene}/{layer}/Common.elm",
             ],
         ).rep(scene).rep(layer)
+        if has_component:
+            Updater(
+                [
+                    ".messenger/layer/Model_C.elm",
+                    ".messenger/layer/Common_C.elm",
+                ],
+                [
+                    f"src/Scenes/{scene}/{layer}/Model.elm",
+                    f"src/Scenes/{scene}/{layer}/Common.elm",
+                ],
+            ).rep(scene).rep(layer)
 
     def update_layers(self, scene: str):
         """
         Update layer settings.
         """
         layers = self.config["scenes"][scene]
 
@@ -423,20 +437,26 @@
     msg.add_scene(name)
     msg.update_scenes()
     msg.format()
     print("Done!")
 
 
 @app.command()
-def layer(scene: str, layer: str):
+def layer(
+    scene: str,
+    layer: str,
+    has_component: bool = typer.Option(
+        False, "--with-component", "-c", help="Use components in this layer"
+    ),
+):
     msg = Messenger()
     input(
         f"You are going to create a layer named {layer} under scene {scene}, continue?"
     )
-    msg.add_layer(scene, layer)
+    msg.add_layer(scene, layer, has_component)
     msg.update_layers(scene)
     msg.format()
     print("Done!")
 
 
 @app.command()
 def sceneproto(sceneproto: str):
@@ -466,19 +486,21 @@
         f"You are going to create a layer named {layer} under sceneproto {sceneproto}, continue?"
     )
     msg.add_sceneproto_layer(sceneproto, layer)
     msg.update_sceneproto_layers(sceneproto)
     msg.format()
     print("Done!")
 
+
 @app.command()
-def gamecomponent(sceneproto:str, gc:str):
+def gamecomponent(sceneproto: str, gc: str):
     msg = Messenger()
     input(
         f"You are going to create a game component named {gc} under sceneproto {sceneproto}, continue?"
     )
     msg.add_gamecomponent(sceneproto, gc)
     msg.format()
     print("Done!")
 
+
 if __name__ == "__main__":
     app()
```

### Comparing `elm-messenger-0.1.7/messengercli/updater.py` & `elm-messenger-0.1.8/messengercli/updater.py`

 * *Files identical despite different names*

