# Comparing `tmp/zoomaker-0.4.0.tar.gz` & `tmp/zoomaker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoomaker-0.4.0.tar", max compression
+gzip compressed data, was "zoomaker-0.5.0.tar", max compression
```

## Comparing `zoomaker-0.4.0.tar` & `zoomaker-0.5.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     5402 2023-05-01 14:39:32.383238 zoomaker-0.4.0/README.md
--rw-r--r--   0        0        0      587 2023-05-06 08:07:46.152788 zoomaker-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6538 2023-05-06 08:07:37.811516 zoomaker-0.4.0/zoomaker.py
--rw-r--r--   0        0        0     6109 1970-01-01 00:00:00.000000 zoomaker-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     6424 2023-05-23 15:27:26.401882 zoomaker-0.5.0/README.md
+-rw-r--r--   0        0        0      587 2023-05-23 15:30:53.191905 zoomaker-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6855 2023-05-23 15:29:01.177122 zoomaker-0.5.0/zoomaker.py
+-rw-r--r--   0        0        0     7131 1970-01-01 00:00:00.000000 zoomaker-0.5.0/PKG-INFO
```

### Comparing `zoomaker-0.4.0/README.md` & `zoomaker-0.5.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+![zoomaker_social_keyvisual](https://github.com/hfg-gmuend/zoomaker/assets/480224/75d3d492-fe54-4711-afbf-02768bbb4033)
+
 Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 ========
 
 Zoomaker is a command-line tool that helps install AI models, git repositories and run scripts.
 
 - **single source of truth**: all resources are neatly definied in the `zoo.yaml` file
 - **freeze versions**: know exactly which revision of a resources is installed at any time
@@ -19,15 +21,15 @@
 
 ```bash
 pip install zoomaker
 ```
 
 ## 🦁 zoo.yaml Examples
 
-Example of the `zoo.yaml` of a Stable Diffsion project with the [Automatic1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui) image generator:
+Example of the `zoo.yaml` of a Stable Diffusion project with the [Automatic1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui) image generator:
 
 ```yaml
 name: my-automatic1111-model-zoo
 version: 1.0
 description: Lorem ipsum
 author: your name
 
@@ -146,18 +148,28 @@
 
 ## 🧞 Zoomaker Commands
 
 All commands are run from the root of the project, where also your `zoo.yaml` file is located.
 
 | Command                | Action                                           |
 | :--------------------- | :----------------------------------------------- |
-| `zoomaker install`          | Installs resources as defined in `zoo.yaml`                           |
+| `zoomaker install`          | Installs resources as defined in `zoo.yaml` |
 | `zoomaker run <script_name>`    | Run CLI scripts as defined in `zoo.yaml` |
 | `zoomaker --help` | Get help using the Zoomaker CLI                     |
 | `zoomaker --version` | Show current Zoomaker version                     |
+| `zoomaker --no-symlinks` | Do not use symlinks for installing resources  |
+
+## ⚠️ Limitations on Windows
+Symlinks are not widely supported on Windows, which limits the caching mechanism used by Zoomaker. To work around this limitation, you can disable symlinks by using the `--no-symlinks` flag with the install command:
+
+```bash
+zoomaker install --no-symlinks
+```
+
+This will still use the cache directory for checking if files are already cached, but if not, they will be downloaded and duplicated directly to the installation directory, saving bandwidth but increasing disk usage. Alternatively, you can use the [Windows Subsystem for Linux "WSL"](https://docs.microsoft.com/en-us/windows/wsl/install-win10) (don't forget to [enable developer mode](https://docs.microsoft.com/en-us/windows/apps/get-started/enable-your-device-for-development)) or run Zoomaker as an administrator to enable symlink support on Windows.
 
 ## 🤗 Hugging Face Access Token
 
 You might be asked for a [Hugging Face Access Token](https://huggingface.co/docs/hub/security-tokens) during `zoomaker install`. Some resources on Hugging Face require accepting the terms of use of the model. You can set your access token by running this command in a terminal. The command `huggingface-cli` is automatically shipped alongside zoomaker.
 
 ```bash
 huggingface-cli login
```

### Comparing `zoomaker-0.4.0/pyproject.toml` & `zoomaker-0.5.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zoomaker"
-version = "0.4.0"
+version = "0.5.0"
 description = "Zoomaker - Friendly house keeping for your AI model zoo and related resources."
 authors = ["Benedikt Groß"]
 readme = "README.md"
 homepage = "https://github.com/hfg-gmuend/zoomaker"
 documentation = "https://github.com/hfg-gmuend/zoomaker"
 repository = "https://github.com/hfg-gmuend/zoomaker"
```

### Comparing `zoomaker-0.4.0/zoomaker.py` & `zoomaker-0.5.0/zoomaker.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,18 +29,20 @@
                     raise Exception("❌ Resource must have 'type' attribute")
                 if "install_to" not in resource:
                     raise Exception("❌ Resource must have 'install_to' attribute")
                 type = resource["type"]
                 if type not in ["huggingface", "git", "download"]:
                     raise Exception(f"❌ Unknown resource type: {type}")
 
-    def install(self):
+    def install(self, no_symlinks: bool = False):
         print(f"👋 ===> {self.yaml_file} <===")
         print(f"name: {self.data.get('name', 'N/A')}")
         print(f"version: {self.data.get('version', 'N/A')}\n")
+        if no_symlinks:
+            print(f"⛔️ installing resources without symlinks ...")
         print(f"👇 installing resources ...")
         counter = 0;
         for group, resources in self.data["resources"].items():
             print(f"\n{group}:")
 
             for resource in resources:
                 name = resource["name"]
@@ -53,15 +55,15 @@
                 print(f"\t{counter}. {name} to {install_to}")
                 os.makedirs(install_to, exist_ok=True)
 
                 # Hugging Face Hub
                 if type == "huggingface":
                     repo_id = "/".join(src.split("/")[0:2])
                     repo_filepath = "/".join(src.split("/")[2:])
-                    downloaded = hf_hub_download(repo_id=repo_id, filename=repo_filepath, local_dir=install_to, revision=revision)
+                    downloaded = hf_hub_download(repo_id=repo_id, filename=repo_filepath, local_dir=install_to, revision=revision, local_dir_use_symlinks=False if no_symlinks else "auto")
                     if rename_to:
                         os.rename(downloaded, os.path.join(install_to, rename_to))
                 # Git
                 elif type == "git":
                     repo_path = os.path.join(install_to, self._get_repo_name(src))
                     if rename_to:
                         print(f"\trename_to is not supported for git repos. Ignoring rename_to: {rename_to}")
@@ -125,19 +127,20 @@
             return None
         return filename
 
 def main():
     parser = argparse.ArgumentParser(description="Install models, git repos and run scripts defined in the zoo.yaml file.")
     parser.add_argument("command", nargs="?", choices=["install", "run"], help="The command to execute.")
     parser.add_argument("script", nargs="?", help="The script name to execute.")
-    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.4.0")
+    parser.add_argument("--no-symlinks", action='store_true', help="Do not create symlinks for the installed resources.")
+    parser.add_argument("-v", "--version", action='version', help="The current version of the zoomaker.", version="0.5.0")
     args = parser.parse_args()
 
     if args.command == "install":
-        Zoomaker("zoo.yaml").install()
+        Zoomaker("zoo.yaml").install(args.no_symlinks)
     elif args.command == "run":
         Zoomaker("zoo.yaml").run(args.script)
     else:
         parser.print_help()
 
 if __name__ == "__main__":
     main()
```

### Comparing `zoomaker-0.4.0/PKG-INFO` & `zoomaker-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: zoomaker
-Version: 0.4.0
+Version: 0.5.0
 Summary: Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 Home-page: https://github.com/hfg-gmuend/zoomaker
 Author: Benedikt Groß
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: huggingface-hub (>=0.14.0,<0.15.0)
 Project-URL: Documentation, https://github.com/hfg-gmuend/zoomaker
 Project-URL: Repository, https://github.com/hfg-gmuend/zoomaker
 Description-Content-Type: text/markdown
 
+![zoomaker_social_keyvisual](https://github.com/hfg-gmuend/zoomaker/assets/480224/75d3d492-fe54-4711-afbf-02768bbb4033)
+
 Zoomaker - Friendly house keeping for your AI model zoo and related resources.
 ========
 
 Zoomaker is a command-line tool that helps install AI models, git repositories and run scripts.
 
 - **single source of truth**: all resources are neatly definied in the `zoo.yaml` file
 - **freeze versions**: know exactly which revision of a resources is installed at any time
@@ -36,15 +38,15 @@
 
 ```bash
 pip install zoomaker
 ```
 
 ## 🦁 zoo.yaml Examples
 
-Example of the `zoo.yaml` of a Stable Diffsion project with the [Automatic1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui) image generator:
+Example of the `zoo.yaml` of a Stable Diffusion project with the [Automatic1111](https://github.com/AUTOMATIC1111/stable-diffusion-webui) image generator:
 
 ```yaml
 name: my-automatic1111-model-zoo
 version: 1.0
 description: Lorem ipsum
 author: your name
 
@@ -163,18 +165,28 @@
 
 ## 🧞 Zoomaker Commands
 
 All commands are run from the root of the project, where also your `zoo.yaml` file is located.
 
 | Command                | Action                                           |
 | :--------------------- | :----------------------------------------------- |
-| `zoomaker install`          | Installs resources as defined in `zoo.yaml`                           |
+| `zoomaker install`          | Installs resources as defined in `zoo.yaml` |
 | `zoomaker run <script_name>`    | Run CLI scripts as defined in `zoo.yaml` |
 | `zoomaker --help` | Get help using the Zoomaker CLI                     |
 | `zoomaker --version` | Show current Zoomaker version                     |
+| `zoomaker --no-symlinks` | Do not use symlinks for installing resources  |
+
+## ⚠️ Limitations on Windows
+Symlinks are not widely supported on Windows, which limits the caching mechanism used by Zoomaker. To work around this limitation, you can disable symlinks by using the `--no-symlinks` flag with the install command:
+
+```bash
+zoomaker install --no-symlinks
+```
+
+This will still use the cache directory for checking if files are already cached, but if not, they will be downloaded and duplicated directly to the installation directory, saving bandwidth but increasing disk usage. Alternatively, you can use the [Windows Subsystem for Linux "WSL"](https://docs.microsoft.com/en-us/windows/wsl/install-win10) (don't forget to [enable developer mode](https://docs.microsoft.com/en-us/windows/apps/get-started/enable-your-device-for-development)) or run Zoomaker as an administrator to enable symlink support on Windows.
 
 ## 🤗 Hugging Face Access Token
 
 You might be asked for a [Hugging Face Access Token](https://huggingface.co/docs/hub/security-tokens) during `zoomaker install`. Some resources on Hugging Face require accepting the terms of use of the model. You can set your access token by running this command in a terminal. The command `huggingface-cli` is automatically shipped alongside zoomaker.
 
 ```bash
 huggingface-cli login
```

