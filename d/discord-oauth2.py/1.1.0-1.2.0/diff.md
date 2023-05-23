# Comparing `tmp/discord-oauth2.py-1.1.0.tar.gz` & `tmp/discord-oauth2.py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-oauth2.py-1.1.0.tar", last modified: Sun Feb  5 16:48:49 2023, max compression
+gzip compressed data, was "discord-oauth2.py-1.2.0.tar", last modified: Tue May 23 13:21:14 2023, max compression
```

## Comparing `discord-oauth2.py-1.1.0.tar` & `discord-oauth2.py-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 16:48:49.178296 discord-oauth2.py-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-05 16:48:38.000000 discord-oauth2.py-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-02-05 16:48:49.178296 discord-oauth2.py-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-02-05 16:48:38.000000 discord-oauth2.py-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 16:48:49.178296 discord-oauth2.py-1.1.0/discord_oauth2.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-02-05 16:48:49.000000 discord-oauth2.py-1.1.0/discord_oauth2.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-02-05 16:48:49.000000 discord-oauth2.py-1.1.0/discord_oauth2.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-05 16:48:49.000000 discord-oauth2.py-1.1.0/discord_oauth2.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-05 16:48:49.000000 discord-oauth2.py-1.1.0/discord_oauth2.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-05 16:48:49.000000 discord-oauth2.py-1.1.0/discord_oauth2.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-05 16:48:49.178296 discord-oauth2.py-1.1.0/discordoauth2/
--rw-r--r--   0 runner    (1001) docker     (123)    10104 2023-02-05 16:48:38.000000 discord-oauth2.py-1.1.0/discordoauth2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-05 16:48:49.178296 discord-oauth2.py-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-02-05 16:48:38.000000 discord-oauth2.py-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:21:14.158206 discord-oauth2.py-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 13:21:03.000000 discord-oauth2.py-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-23 13:21:14.158206 discord-oauth2.py-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-23 13:21:03.000000 discord-oauth2.py-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:21:14.158206 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-23 13:21:14.000000 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-23 13:21:14.000000 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 13:21:14.000000 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 13:21:14.000000 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 13:21:14.000000 discord-oauth2.py-1.2.0/discord_oauth2.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 13:21:14.158206 discord-oauth2.py-1.2.0/discordoauth2/
+-rw-r--r--   0 runner    (1001) docker     (123)    17451 2023-05-23 13:21:03.000000 discord-oauth2.py-1.2.0/discordoauth2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 13:21:14.158206 discord-oauth2.py-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-23 13:21:03.000000 discord-oauth2.py-1.2.0/setup.py
```

### Comparing `discord-oauth2.py-1.1.0/LICENSE` & `discord-oauth2.py-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-oauth2.py-1.1.0/PKG-INFO` & `discord-oauth2.py-1.2.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: discord-oauth2.py
-Version: 1.1.0
-Summary: Use Discord's OAuth2 effortlessly! Turns the auth code to a access token and the access token into scope infomation. 
-Home-page: https://github.com/TreeBen77/discordoauth2
-Author: TreeBen77
-License: MIT
-Keywords: flask,oauth2,discord,discord-api
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # DiscordOAuth2.py
 Use Discord's OAuth2 effortlessly! Turns the auth code to a access token and the access token into scope infomation.
 
 ### Useful Links
 Discord Server: https://discord.gg/DJ9xbbZAP5
 
 Documentation is coming soon, don't worry.
@@ -45,14 +33,18 @@
         "type": 7,
         "key": "supporter",
         "name": "Supporter",
         "description": "Spent money to help the game"
     }
 ])
 
+@app.route('/')
+def main():
+  return redirect(client.generate_uri(scope=["identify", "connections", "guilds", "role_connections.write"]))
+
 @app.route("/oauth2")
 def oauth2():
     code = request.args.get("code")
 
     access = client.exchange_code(code)
 
     access.update_metadata("Platform Name", "Username",  level=69, supporter=True)
@@ -60,8 +52,8 @@
     identify = access.fetch_identify()
     connections = access.fetch_connections()
     guilds = access.fetch_guilds()
 
     return f"""{identify}<br><br>{connections}<br><br>{guilds}"""
 
 app.run("0.0.0.0", 8080)
-```
+```
```

### Comparing `discord-oauth2.py-1.1.0/discord_oauth2.py.egg-info/PKG-INFO` & `discord-oauth2.py-1.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-oauth2.py
-Version: 1.1.0
+Version: 1.2.0
 Summary: Use Discord's OAuth2 effortlessly! Turns the auth code to a access token and the access token into scope infomation. 
 Home-page: https://github.com/TreeBen77/discordoauth2
 Author: TreeBen77
 License: MIT
 Keywords: flask,oauth2,discord,discord-api
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -45,14 +45,18 @@
         "type": 7,
         "key": "supporter",
         "name": "Supporter",
         "description": "Spent money to help the game"
     }
 ])
 
+@app.route('/')
+def main():
+  return redirect(client.generate_uri(scope=["identify", "connections", "guilds", "role_connections.write"]))
+
 @app.route("/oauth2")
 def oauth2():
     code = request.args.get("code")
 
     access = client.exchange_code(code)
 
     access.update_metadata("Platform Name", "Username",  level=69, supporter=True)
```

### Comparing `discord-oauth2.py-1.1.0/setup.py` & `discord-oauth2.py-1.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 setup(
     name='discord-oauth2.py',
     description='Use Discord\'s OAuth2 effortlessly! Turns the auth code to a access token and the access token into scope infomation. ',
-    version="1.1.0",
+    version="1.2.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     python_requires='>=3.8',
     author="TreeBen77",
     packages=[
         'discordoauth2'
```

