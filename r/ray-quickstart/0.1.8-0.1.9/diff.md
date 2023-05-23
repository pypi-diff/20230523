# Comparing `tmp/ray-quickstart-0.1.8.tar.gz` & `tmp/ray-quickstart-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ray-quickstart-0.1.8.tar", last modified: Tue Feb  7 08:28:46 2023, max compression
+gzip compressed data, was "ray-quickstart-0.1.9.tar", last modified: Tue Feb  7 12:46:41 2023, max compression
```

## Comparing `ray-quickstart-0.1.8.tar` & `ray-quickstart-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,28 @@
-drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 08:28:46.259268 ray-quickstart-0.1.8/
--rw-r--r--   0 tuyen      (501) staff       (20)     1056 2023-02-02 01:41:04.000000 ray-quickstart-0.1.8/LICENSE.txt
--rw-r--r--   0 tuyen      (501) staff       (20)     5123 2023-02-07 08:28:46.259131 ray-quickstart-0.1.8/PKG-INFO
--rw-r--r--   0 tuyen      (501) staff       (20)     4377 2023-02-05 07:37:50.000000 ray-quickstart-0.1.8/README.md
--rw-r--r--   0 tuyen      (501) staff       (20)     1230 2023-02-07 07:25:51.000000 ray-quickstart-0.1.8/pyproject.toml
-drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 08:28:46.257606 ray-quickstart-0.1.8/scripts/
--rwxr-xr-x   0 tuyen      (501) staff       (20)      354 2023-02-03 11:13:35.000000 ray-quickstart-0.1.8/scripts/ray_start.bat
--rwxr-xr-x   0 tuyen      (501) staff       (20)      262 2023-02-02 23:36:40.000000 ray-quickstart-0.1.8/scripts/ray_start.sh
--rwxr-xr-x   0 tuyen      (501) staff       (20)       24 2023-02-03 11:13:35.000000 ray-quickstart-0.1.8/scripts/ray_stop.bat
--rwxr-xr-x   0 tuyen      (501) staff       (20)       22 2023-02-02 23:36:40.000000 ray-quickstart-0.1.8/scripts/ray_stop.sh
--rwxr-xr-x   0 tuyen      (501) staff       (20)     1281 2023-02-05 23:54:44.000000 ray-quickstart-0.1.8/scripts/ubuntu_start.bat
--rwxr-xr-x   0 tuyen      (501) staff       (20)       28 2023-02-02 23:36:40.000000 ray-quickstart-0.1.8/scripts/ubuntu_stop.bat
--rw-r--r--   0 tuyen      (501) staff       (20)       38 2023-02-07 08:28:46.259308 ray-quickstart-0.1.8/setup.cfg
--rwxr-xr-x   0 tuyen      (501) staff       (20)     2403 2023-02-07 08:28:17.000000 ray-quickstart-0.1.8/setup.py
-drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 08:28:46.256413 ray-quickstart-0.1.8/src/
-drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 08:28:46.258089 ray-quickstart-0.1.8/src/ray_quickstart/
--rw-r--r--   0 tuyen      (501) staff       (20)       82 2023-02-07 08:28:46.000000 ray-quickstart-0.1.8/src/ray_quickstart/__init__.py
--rw-r--r--   0 tuyen      (501) staff       (20)     6933 2023-02-07 06:52:21.000000 ray-quickstart-0.1.8/src/ray_quickstart/init.py
--rw-r--r--   0 tuyen      (501) staff       (20)     4237 2023-02-07 05:43:41.000000 ray-quickstart-0.1.8/src/ray_quickstart/monkey_patch.py
--rw-r--r--   0 tuyen      (501) staff       (20)     2406 2023-02-05 08:40:41.000000 ray-quickstart-0.1.8/src/ray_quickstart/rsync_syncer.py
-drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 08:28:46.258958 ray-quickstart-0.1.8/src/ray_quickstart/util/
--rw-r--r--   0 tuyen      (501) staff       (20)        0 2023-02-04 12:44:01.000000 ray-quickstart-0.1.8/src/ray_quickstart/util/__init__.py
--rw-r--r--   0 tuyen      (501) staff       (20)      478 2023-02-01 23:51:32.000000 ray-quickstart-0.1.8/src/ray_quickstart/util/debug.py
--rw-r--r--   0 tuyen      (501) staff       (20)     1004 2023-02-01 23:45:49.000000 ray-quickstart-0.1.8/src/ray_quickstart/util/platform.py
-drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 08:28:46.258661 ray-quickstart-0.1.8/src/ray_quickstart.egg-info/
--rw-r--r--   0 tuyen      (501) staff       (20)     5123 2023-02-07 08:28:46.000000 ray-quickstart-0.1.8/src/ray_quickstart.egg-info/PKG-INFO
--rw-r--r--   0 tuyen      (501) staff       (20)      620 2023-02-07 08:28:46.000000 ray-quickstart-0.1.8/src/ray_quickstart.egg-info/SOURCES.txt
--rw-r--r--   0 tuyen      (501) staff       (20)        1 2023-02-07 08:28:46.000000 ray-quickstart-0.1.8/src/ray_quickstart.egg-info/dependency_links.txt
--rw-r--r--   0 tuyen      (501) staff       (20)       19 2023-02-07 08:28:46.000000 ray-quickstart-0.1.8/src/ray_quickstart.egg-info/requires.txt
--rw-r--r--   0 tuyen      (501) staff       (20)       15 2023-02-07 08:28:46.000000 ray-quickstart-0.1.8/src/ray_quickstart.egg-info/top_level.txt
+drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 12:46:41.901476 ray-quickstart-0.1.9/
+-rw-r--r--   0 tuyen      (501) staff       (20)     1056 2023-02-02 01:41:04.000000 ray-quickstart-0.1.9/LICENSE.txt
+-rw-r--r--   0 tuyen      (501) staff       (20)     6401 2023-02-07 12:46:41.901346 ray-quickstart-0.1.9/PKG-INFO
+-rw-r--r--   0 tuyen      (501) staff       (20)     5655 2023-02-07 12:31:16.000000 ray-quickstart-0.1.9/README.md
+-rw-r--r--   0 tuyen      (501) staff       (20)     1167 2023-02-07 11:28:44.000000 ray-quickstart-0.1.9/pyproject.toml
+drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 12:46:41.899524 ray-quickstart-0.1.9/scripts/
+-rwxr-xr-x   0 tuyen      (501) staff       (20)      354 2023-02-03 11:13:35.000000 ray-quickstart-0.1.9/scripts/ray_start.bat
+-rwxr-xr-x   0 tuyen      (501) staff       (20)      262 2023-02-02 23:36:40.000000 ray-quickstart-0.1.9/scripts/ray_start.sh
+-rwxr-xr-x   0 tuyen      (501) staff       (20)       24 2023-02-03 11:13:35.000000 ray-quickstart-0.1.9/scripts/ray_stop.bat
+-rwxr-xr-x   0 tuyen      (501) staff       (20)       22 2023-02-02 23:36:40.000000 ray-quickstart-0.1.9/scripts/ray_stop.sh
+-rw-r--r--   0 tuyen      (501) staff       (20)       38 2023-02-07 12:46:41.901513 ray-quickstart-0.1.9/setup.cfg
+-rwxr-xr-x   0 tuyen      (501) staff       (20)     2403 2023-02-07 08:28:17.000000 ray-quickstart-0.1.9/setup.py
+drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 12:46:41.898140 ray-quickstart-0.1.9/src/
+drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 12:46:41.900065 ray-quickstart-0.1.9/src/ray_quickstart/
+-rw-r--r--   0 tuyen      (501) staff       (20)       83 2023-02-07 12:46:41.000000 ray-quickstart-0.1.9/src/ray_quickstart/__init__.py
+-rw-r--r--   0 tuyen      (501) staff       (20)     6691 2023-02-07 12:43:55.000000 ray-quickstart-0.1.9/src/ray_quickstart/init.py
+-rw-r--r--   0 tuyen      (501) staff       (20)     4170 2023-02-07 12:42:21.000000 ray-quickstart-0.1.9/src/ray_quickstart/monkey_patch.py
+-rw-r--r--   0 tuyen      (501) staff       (20)     2562 2023-02-07 12:43:31.000000 ray-quickstart-0.1.9/src/ray_quickstart/rsync_syncer.py
+drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 12:46:41.901075 ray-quickstart-0.1.9/src/ray_quickstart/util/
+-rw-r--r--   0 tuyen      (501) staff       (20)        0 2023-02-04 12:44:01.000000 ray-quickstart-0.1.9/src/ray_quickstart/util/__init__.py
+-rw-r--r--   0 tuyen      (501) staff       (20)      478 2023-02-01 23:51:32.000000 ray-quickstart-0.1.9/src/ray_quickstart/util/debug.py
+-rw-r--r--   0 tuyen      (501) staff       (20)     1004 2023-02-01 23:45:49.000000 ray-quickstart-0.1.9/src/ray_quickstart/util/platform.py
+drwxr-xr-x   0 tuyen      (501) staff       (20)        0 2023-02-07 12:46:41.900620 ray-quickstart-0.1.9/src/ray_quickstart.egg-info/
+-rw-r--r--   0 tuyen      (501) staff       (20)     6401 2023-02-07 12:46:41.000000 ray-quickstart-0.1.9/src/ray_quickstart.egg-info/PKG-INFO
+-rw-r--r--   0 tuyen      (501) staff       (20)      571 2023-02-07 12:46:41.000000 ray-quickstart-0.1.9/src/ray_quickstart.egg-info/SOURCES.txt
+-rw-r--r--   0 tuyen      (501) staff       (20)        1 2023-02-07 12:46:41.000000 ray-quickstart-0.1.9/src/ray_quickstart.egg-info/dependency_links.txt
+-rw-r--r--   0 tuyen      (501) staff       (20)       19 2023-02-07 12:46:41.000000 ray-quickstart-0.1.9/src/ray_quickstart.egg-info/requires.txt
+-rw-r--r--   0 tuyen      (501) staff       (20)       15 2023-02-07 12:46:41.000000 ray-quickstart-0.1.9/src/ray_quickstart.egg-info/top_level.txt
```

### Comparing `ray-quickstart-0.1.8/LICENSE.txt` & `ray-quickstart-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ray-quickstart-0.1.8/PKG-INFO` & `ray-quickstart-0.1.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,101 @@
-Metadata-Version: 2.1
-Name: ray-quickstart
-Version: 0.1.8
-Summary: Wrapper around the Ray library to make it easier for you to set up your ML project to use Ray to train/tune your models remotely on a GPU-enabled computer
-Author-email: Tuyen Truong <tuyen.truong@gmail.com>
-Project-URL: Homepage, https://github.com/tuyentruong/ray_quickstart
-Project-URL: Bug Tracker, https://github.com/tuyentruong/ray_quickstart/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-This project allows you to quickly set up your machine-learning project so that you can develop locally on your computer and 
-then train and tune your models remotely on a GPU-enabled computer. The remote training/tuning is implemented using 
-[Ray](https://github.com/ray-project/ray).
+Ray QuickStart allows you to quickly get started with remote training and tuning of your machine-learning
+project using Ray. You can develop locally using your computer and then train and tune your models remotely on a
+GPU-enabled computer. The remote training/tuning is implemented using the [Ray](https://github.com/ray-project/ray) library.
+
 
 ## Why Ray QuickStart?
 
-I think a lot of developers (like me) who are interested in getting started with ML learning are using Macs for their 
-development, but Macs don't have GPUs and MPS devices are still nowhere close to being as fast as GPUS. I ended up 
-buying a GPU card for my Windows computer, but found it cumbersome to develop on my Mac, commit my changes to GitHub, 
-push the changes to my Windows computer, and then run my training and tuning from my Windows computer. In addition, 
-I found myself having to manually save the trained models to the cloud and then download them to my Mac to use them for 
-inference afterwards.
-
-Ray was designed to address this inefficiency, but I didn't find it as easy as I would have liked to get it set up for 
-remote training and tuning on another computer. It's possible that they have the functionality already in place, so 
-please let me know if I am reinventing the wheel somewhere.
-
-The quickstart enable three main things:
-1. Sync your Python code to the remote computer.
-2. Uses Ray to perform the distributed training and tuning.
-3. Sync the trained model/checkpoints back to your computer.
-
-Over time, I hope to add additional functionality to allow you to train from a cluster in the cloud once your needs 
-exceed the capabilities of your GPU card.
-
-## Limitations Addressed By Ray QuickStart
-
-This project does the following to make it easier for you to get started with remote training and tuning:
-1. Help you create an Ubuntu 22.04 VM on your Windows computer using WSL2. I need Windows for some of my work and tried
-to run the Ray cluster directly from Windows, but it doesn't look like Ray supports it yet: I ran into issues trying to 
-sync the checkpoints from Windows to my Mac computer.
-2. Note that you will need to start the Ubuntu instanceYou will need to start your Ubuntu instance using wsl
-
-## Setup
-
-1. You can get started by either cloning this repository or by installing the ray-quickstart package from PyPI. The former
-is preferred if you want to try out the example project, but the latter is preferred if you want to use this package in
-your own project.
-
-2. If your GPU-enabled computer has Windows installed, you can run `setup\setup_windows.bat` to set up Ubuntu 22.04 
-on your computer. Some terminal windows will open during the setup process. You can close them once the setup is complete.
-
-If your GPU-enabled computer has Ubuntu installed, you can run `setup/setup_ubuntu.sh` to set it up.
-
-On your Mac, you will need to install grpcio using Conda and then copy it over to your pipenv's site-packages (see `setup/setup_mac.sh`).
-
-3. After Ubuntu has been installed, you will need to add your public SSH key to ~/.ssh/authorized_keys on your Ubuntu 
-instance so that your local computer will be able to connect to the Ubuntu instance for training/tuning.
-## Setup
-1. Create a YAML configuration file named `ray_config.yaml` in the root directory of your project.
-1. Ray QuickStart expects a configuration file named `ray_config.yaml` to be present in the root directory of your project.
+I recently got a GPU card for my Windows computer to allow me to train my ML models more quickly. I wanted to continue
+developing from my Mac computer, but the process of copying my code and data to my Windows computer, training my models, 
+and then copying the trained models back to my Mac computer was cumbersome. 
+
+I found the Ray library and decided to use it to train my models remotely on my Windows computer after developing it 
+locally on my Mac computer. I ran into some issues getting started with Ray, however, so I created this project to make 
+it easier for others to get started.
+
+Ray Quickstart is available as both a [PyPI package](https://pypi.org/project/ray-quickstart/) and as a 
+[GitHub repo](https://github.com/tuyentruong/ray-quickstart). You should install the PyPI package if you want to add 
+remote training and tuning to your own ML project. The GitHub repo includes an example project that you can run to see 
+the Ray QuickStart library in action.
+
+
+## What Does Ray QuickStart Do?
+
+Ray QuickStart will:
+1. Install the packages in your project's Pipfile on your remote computer without needing to set up an auto-scaling Ray cluster.
+2. Clean up your trials directories before training/tuning starts (optional).
+3. Use Ray to sync your Python project code to your remote computer and train/tune your model there.
+4. Sync the checkpoints from your training/tuning back to your computer.
+
+## Setting Up Your GPU-Enabled Computer
+
+My setup is as follows:
+1. I have a Mac computer that I use for development.
+2. I have a Windows 11 computer with a GPU card installed that I want to use for trainging/tuning.
+
+I decided to set up my Ray cluster on an Ubuntu instance on my Windows computer using WSL2. I originally tried to
+set up a Ray cluster on my Windows computer, but I ran into some path issues while trying to sync the checkpoints. 
+
+To set up Ubuntu on your Windows computer, you can run `setup\setup_windows.bat` found in GitHub repo. This will create 
+an Ubuntu 22.04 instance on your Windows computer and configure it with a Ray cluster. It will also open up the SSH port 
+and the ports used by Ray in your Windows firewall. A terminal window will open during the setup process. You can ignore 
+any errors that the window shows and close it once setup has completed.
+
+Once the Ubuntu instance has been set up, you will need to start it. It is recommended that you start the Ubuntu instance
+using the `scripts\ubuntu_start.bat` script. The script will ensure that port forwarding has been set up correctly so
+that you will be able to communicate with the Ray cluster on the Ubuntu instance from your local computer.
+
+Finally, you will need to add your public SSH key to ~/.ssh/authorized_keys on your Ubuntu instance so that your local
+computer will be able to connect to the Ubuntu instance to configure your runtime environment and sync the checkpoints
+using rsync.
+
+If your GPU-enabled computer has Linux installed, you can take a look at `setup\setup_ubuntu.sh` for the setup that needs
+to be done to install and configure Ray cluster. The setup script was written for Ubuntu, but hopefully it will be easy 
+to adapt for other distros.
+
+
+## Setting Up Your Local Computer
+
+1. Create a YAML configuration file named `ray_config.yaml` in your project. The file should contain the following
+   information:
+
+```yaml
+driver:
+  user: 'tuyen' # Your username on your local computer
+  private_key_file: '~/.ssh/id_rsa' # The private key file that will be used to connect to the remote computer
+
+ray_head:
+  hostname_or_ip_address: '192.168.2.4' # The hostname or IP address of the remote computer
+  client_server_port: 10001 # The port that will be used to communicate with the Ray cluster
+
+worker:
+  user: 'tuyen' # The user that will be used to connect to the remote computer using SSH
+  hostname_or_ip_address: '192.168.2.4' # The hostname or IP address of the remote computer
+  ssh_port: 22 # The port that will be used to connect to the remote computer using SSH
+  platform: 'linux' # The platform that the remote computer is running on (used for path conversion)
+```
+
+2. Add a call to `initialize_ray_with_syncer()` to your ML project code to initialize the connection with the Ray cluster.
+   The call will return a syncer object.
+
+3. Pass the syncer object to the `fit()` call in the subclass of `ray.train.base_trainer.BaseTrainer` that you are using 
+   to train your model. The syncer object will be used to sync your checkpoints back to your local computer after training.
+
 
 ## Troubleshooting
 
 **When I connect to the Ubuntu WSL instance, it says that the GPU is not available. What can I do to fix this?** 
    
-I got stumped on this issue for a while. From https://github.com/microsoft/WSL/issues/9185, I discovered the cause:
+I got stumped on this issue for a while. From https://github.com/microsoft/WSL/issues/9185, it seems to be user permission
+issue:
    
 > There is an issue when nvidia-smi doesn't work when one instance is launched as Administrator and another as a non-Administrator.
 
-When I started the Ubuntu WSL instance from the command line and passed in the `--user` flag with the same username as 
-in Windows, then it worked. It is recommended that you start the Ubuntu WSL instance using the `ubuntu_start.sh` script.
+It started working when I started the Ubuntu WSL instance from the command line and passed in the `--user` flag with the same username as 
+my Windows's username. It is recommended that you start the Ubuntu WSL instance using the `scripts\ubuntu_start.bat` script
+to avoid this issue.
+
 
-**I am getting ModuleNotFoundError: No module named '[module]' when I try to training remotely. How do I fix it?**
+## Future Directions
 
-You will need to install all your package dependencies to the ray-quickstart project because that is the project used 
-when starting the Ray cluster. Without those packages installed, Ray will fail when trying to export your code to the
-remote machine for training.
+1. Add support for training on a cluster in the cloud.
```

### Comparing `ray-quickstart-0.1.8/pyproject.toml` & `ray-quickstart-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 
 [tool.setuptools]
 script-files = [
     'scripts/ray_start.bat',
     'scripts/ray_start.sh',
     'scripts/ray_stop.bat',
     'scripts/ray_stop.sh',
-    'scripts/ubuntu_start.bat',
-    'scripts/ubuntu_stop.bat',
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "ray_quickstart.__version__"}
 
 [tool.setuptools.packages.find]
 where = ['src']
```

### Comparing `ray-quickstart-0.1.8/setup.py` & `ray-quickstart-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `ray-quickstart-0.1.8/src/ray_quickstart/init.py` & `ray-quickstart-0.1.9/src/ray_quickstart/init.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,61 +14,69 @@
 from ray_quickstart.rsync_syncer import RsyncSyncer
 from ray_quickstart.util import platform
 from ray_quickstart.util.platform import expand_user_home_path
 
 
 def initialize_ray_with_syncer(base_dir,
                                src_dir,
-                               config,
                                ray_config_file_path,
+                               trial_results_dir,
                                success_callback=None,
                                clean_trial_results_dir_at_start=True):
-    if ray.is_initialized():
-        return
+    """
+    :param base_dir: The base directory of your project.
+    :param src_dir: The base directory for your Python source code
+    :param ray_config_file_path: The path to the Ray config file.
+    :param trial_results_dir The directory where the Ray trial results are stored.
+    :param success_callback: Callback to call when Ray is successfully initialized.
+    :param clean_trial_results_dir_at_start: Whether to clean the trial results directory on your local computer and the remote computer at the start of the experiment.
+    :return: an RsyncSyncer object that needs to be called after training to sync the checkpoints from the remote computer to the local computer.
+    """
     ray_config = load_ray_config(ray_config_file_path)
     driver_user = ray_config['driver']['user']
-    driver_hostname_or_ip_address = ray_config['driver']['hostname_or_ip_address']
     driver_private_key_file = ray_config['driver']['private_key_file']
     worker_user = ray_config['worker']['user']
     worker_hostname_or_ip_address = ray_config['worker']['hostname_or_ip_address']
     worker_ssh_port = ray_config['worker']['ssh_port']
     worker_platform = ray_config['worker']['platform']
     syncer = RsyncSyncer(driver_user,
-                         driver_hostname_or_ip_address,
                          driver_private_key_file,
                          worker_user,
                          worker_hostname_or_ip_address,
                          worker_ssh_port,
-                         worker_platform)
+                         worker_platform,
+                         trial_results_dir)
+    if ray.is_initialized():
+        return syncer
     monkey_patch_base_trainer_to_enable_syncing_after_training()
     try:
         if clean_trial_results_dir_at_start:
             clean_trial_results_dir(syncer)
         configure_remote_ray_runtime_environment(base_dir,
                                                  driver_private_key_file,
                                                  worker_user,
                                                  worker_hostname_or_ip_address,
                                                  worker_ssh_port,
                                                  '~/git/ray-quickstart')
-        initialize_ray(src_dir, config, ray_config_file_path, ray_config, success_callback)
+        initialize_ray(src_dir, ray_config_file_path, ray_config, success_callback)
         return syncer
     except ConnectionError:
         if platform.is_windows():
             with subprocess.Popen(f'{base_dir}/scripts/ray_start.bat') as p:
                 p.wait()
-            initialize_ray(src_dir, config, ray_config_file_path, ray_config, success_callback)
+            initialize_ray(src_dir, ray_config_file_path, ray_config, success_callback)
             return syncer
         else:
             raise
 
 
-def initialize_ray(src_dir, config, ray_config_file_path, ray_config=None, success_callback=None):
+def initialize_ray(src_dir, ray_config_file_path, ray_config=None, success_callback=None):
     if ray.is_initialized():
         return
-    if config.run_on_ray_cluster and ray_config is None:
+    if ray_config is None:
         ray_config = load_ray_config(ray_config_file_path)
     # runtime_env is required for cloudpickle to be able to find modules
     runtime_env = {'working_dir': src_dir}
     ray_head_hostname_or_ip_address = ray_config['ray_head']['hostname_or_ip_address']
     ray_head_client_server_port = ray_config['ray_head']['client_server_port']
     ray.init(address=f'ray://{ray_head_hostname_or_ip_address}:{ray_head_client_server_port}', runtime_env=runtime_env)
     monkey_patch_trainable_util_to_fix_checkpoint_paths()
@@ -80,32 +88,24 @@
     if not os.path.exists(config_file_path):
         raise FileNotFoundError(f'config file not found at {config_file_path}')
     with open(config_file_path, 'r') as f:
         ray_config = yaml.safe_load(f)
     return ray_config
 
 
-def get_local_trial_results_dir():
-    return f'~/ray_results'
-
-
-def clean_trial_results_dir(syncer):
+def clean_trial_results_dir(syncer, trial_results_dir):
     logger.info('cleaning local trial results dir...')
-    local_trial_results_dir = os.path.expanduser(get_local_trial_results_dir())
-    if os.path.exists(local_trial_results_dir):
-        delete_dir_contents(local_trial_results_dir)
+    trial_results_dir = os.path.expanduser(trial_results_dir)
+    if os.path.exists(trial_results_dir):
+        delete_dir_contents(trial_results_dir)
     else:
-        os.makedirs(local_trial_results_dir, exist_ok=True)
+        os.makedirs(trial_results_dir, exist_ok=True)
     if syncer is not None:
         logger.info('cleaning ray worker trial results dir...')
-        trial_results_dir = get_local_trial_results_dir()
-        syncer.sync_from_driver_to_ray_worker(trial_results_dir,
-                                              expand_user_home_path(trial_results_dir,
-                                              syncer.worker_user,
-                                              syncer.worker_platform))
+        syncer.sync_from_driver_to_ray_worker()
 
 
 def configure_remote_ray_runtime_environment(base_dir,
                                              driver_private_key_file,
                                              worker_user,
                                              worker_hostname_or_ip_address,
                                              worker_ssh_port,
@@ -130,15 +130,7 @@
 def delete_dir_contents(dir_path):
     for filename in os.listdir(dir_path):
         file_path = os.path.join(dir_path, filename)
         if os.path.isfile(file_path) or os.path.islink(file_path):
             os.unlink(file_path)
         elif os.path.isdir(file_path):
             shutil.rmtree(file_path, ignore_errors=True)
-
-
-def sync_checkpoints_back_to_driver(syncer):
-    trial_results_dir = get_local_trial_results_dir()
-    syncer.sync_from_ray_worker_to_driver(expand_user_home_path(trial_results_dir,
-                                                                syncer.worker_user,
-                                                                syncer.worker_platform),
-                                          trial_results_dir)
```

### Comparing `ray-quickstart-0.1.8/src/ray_quickstart/monkey_patch.py` & `ray-quickstart-0.1.9/src/ray_quickstart/monkey_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 def monkey_patch_base_trainer_to_enable_syncing_after_training():
     """Monkey-patch ray.train.base_trainer.BaseTrainer so we can't sync the checkpoints before retrieving the grid results so that the checkpoints are available locally."""
 
     from ray.train.base_trainer import BaseTrainer
     from ray.air import Result
     from ray.train.base_trainer import TrainingFailedError
     from ray.util import PublicAPI
-    from ray_quickstart.init import sync_checkpoints_back_to_driver
 
     @PublicAPI(stability="beta")
     def fit(self, syncer=None) -> Result:
         """Runs training.
 
         Returns:
             A Result object containing the training result.
@@ -53,15 +52,15 @@
 
         trainable = self.as_trainable()
 
         tuner = Tuner(trainable=trainable, run_config=self.run_config)
         result_grid = tuner.fit()
         assert len(result_grid) == 1
         if syncer is not None:
-            sync_checkpoints_back_to_driver(syncer)
+            syncer.sync_checkpoints_back_to_driver()
         try:
             result = result_grid[0]
             if result.error:
                 raise result.error
         except TuneError as e:
             raise TrainingFailedError from e
         return result
```

### Comparing `ray-quickstart-0.1.8/src/ray_quickstart/rsync_syncer.py` & `ray-quickstart-0.1.9/src/ray_quickstart/rsync_syncer.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,44 +6,45 @@
 from util.platform import expand_user_home_path
 
 
 class RsyncSyncer:
 
     def __init__(self,
                  driver_user,
-                 driver_hostname,
                  driver_private_key_file,
                  worker_user,
                  worker_hostname,
                  worker_ssh_port,
-                 worker_platform):
+                 worker_platform,
+                 trial_results_dir):
         self.driver_user = driver_user
-        self.driver_hostname = driver_hostname
         self.driver_private_key_file = driver_private_key_file
         self.driver_platform = sys.platform
         self.worker_user = worker_user
         self.worker_hostname = worker_hostname
         self.worker_ssh_port = worker_ssh_port
         self.worker_platform = worker_platform
-        self.training_has_ended = False
+        self.trial_results_dir = trial_results_dir
 
-    def sync_from_driver_to_ray_worker(self, driver_dir, worker_dir):
+    def sync_from_driver_to_ray_worker(self):
         """Synchronize from the local computer (driver) to the Ray worker."""
-        driver_dir = expand_user_home_path(driver_dir, self.driver_user, self.driver_platform)
+        driver_dir = expand_user_home_path(self.trial_results_dir, self.driver_user, self.driver_platform)
+        worker_dir = expand_user_home_path(self.trial_results_dir, self.worker_user, self.worker_platform)
         sync_cmd = f'rsync -avz -e "ssh -i {self.driver_private_key_file} -o StrictHostKeyChecking=no -p {self.worker_ssh_port}" --delete --ignore-errors {driver_dir}/ {self.worker_user}@{self.worker_hostname}:{worker_dir}/'
         logger.info(f'syncing from local computer to ray worker: {sync_cmd}')
         try:
             output = str(subprocess.check_output(sync_cmd, shell=True)).replace('\\n', '\n')
             logger.info(output)
         except subprocess.CalledProcessError as e:
             logger.error(f'error syncing down: {e}')
 
-    def sync_from_ray_worker_to_driver(self, worker_dir, driver_dir):
+    def sync_from_ray_worker_to_driver(self):
         """Synchronize from the Ray worker to the local computer (driver)."""
-        driver_dir = expand_user_home_path(driver_dir, self.driver_user, self.driver_platform)
+        worker_dir = expand_user_home_path(self.trial_results_dir, self.worker_user, self.worker_platform)
+        driver_dir = expand_user_home_path(self.trial_results_dir, self.driver_user, self.driver_platform)
         sync_cmd = f'rsync -avz -e "ssh -i {self.driver_private_key_file} -o StrictHostKeyChecking=no -p {self.worker_ssh_port}" --delete --ignore-errors {self.worker_user}@{self.worker_hostname}:{worker_dir}/ {driver_dir}/'
         logger.info(f'syncing from ray worker to local computer: {sync_cmd}')
         try:
             output = str(subprocess.check_output(sync_cmd, shell=True)).replace('\\n', '\n')
             logger.info(output)
         except subprocess.CalledProcessError as e:
             logger.error(f'error syncing from ray worker to local computer: {e}')
```

### Comparing `ray-quickstart-0.1.8/src/ray_quickstart/util/platform.py` & `ray-quickstart-0.1.9/src/ray_quickstart/util/platform.py`

 * *Files identical despite different names*

### Comparing `ray-quickstart-0.1.8/src/ray_quickstart.egg-info/PKG-INFO` & `ray-quickstart-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,117 @@
 Metadata-Version: 2.1
 Name: ray-quickstart
-Version: 0.1.8
+Version: 0.1.9
 Summary: Wrapper around the Ray library to make it easier for you to set up your ML project to use Ray to train/tune your models remotely on a GPU-enabled computer
 Author-email: Tuyen Truong <tuyen.truong@gmail.com>
 Project-URL: Homepage, https://github.com/tuyentruong/ray_quickstart
 Project-URL: Bug Tracker, https://github.com/tuyentruong/ray_quickstart/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-This project allows you to quickly set up your machine-learning project so that you can develop locally on your computer and 
-then train and tune your models remotely on a GPU-enabled computer. The remote training/tuning is implemented using 
-[Ray](https://github.com/ray-project/ray).
+Ray QuickStart allows you to quickly get started with remote training and tuning of your machine-learning
+project using Ray. You can develop locally using your computer and then train and tune your models remotely on a
+GPU-enabled computer. The remote training/tuning is implemented using the [Ray](https://github.com/ray-project/ray) library.
+
 
 ## Why Ray QuickStart?
 
-I think a lot of developers (like me) who are interested in getting started with ML learning are using Macs for their 
-development, but Macs don't have GPUs and MPS devices are still nowhere close to being as fast as GPUS. I ended up 
-buying a GPU card for my Windows computer, but found it cumbersome to develop on my Mac, commit my changes to GitHub, 
-push the changes to my Windows computer, and then run my training and tuning from my Windows computer. In addition, 
-I found myself having to manually save the trained models to the cloud and then download them to my Mac to use them for 
-inference afterwards.
-
-Ray was designed to address this inefficiency, but I didn't find it as easy as I would have liked to get it set up for 
-remote training and tuning on another computer. It's possible that they have the functionality already in place, so 
-please let me know if I am reinventing the wheel somewhere.
-
-The quickstart enable three main things:
-1. Sync your Python code to the remote computer.
-2. Uses Ray to perform the distributed training and tuning.
-3. Sync the trained model/checkpoints back to your computer.
-
-Over time, I hope to add additional functionality to allow you to train from a cluster in the cloud once your needs 
-exceed the capabilities of your GPU card.
-
-## Limitations Addressed By Ray QuickStart
-
-This project does the following to make it easier for you to get started with remote training and tuning:
-1. Help you create an Ubuntu 22.04 VM on your Windows computer using WSL2. I need Windows for some of my work and tried
-to run the Ray cluster directly from Windows, but it doesn't look like Ray supports it yet: I ran into issues trying to 
-sync the checkpoints from Windows to my Mac computer.
-2. Note that you will need to start the Ubuntu instanceYou will need to start your Ubuntu instance using wsl
-
-## Setup
-
-1. You can get started by either cloning this repository or by installing the ray-quickstart package from PyPI. The former
-is preferred if you want to try out the example project, but the latter is preferred if you want to use this package in
-your own project.
-
-2. If your GPU-enabled computer has Windows installed, you can run `setup\setup_windows.bat` to set up Ubuntu 22.04 
-on your computer. Some terminal windows will open during the setup process. You can close them once the setup is complete.
-
-If your GPU-enabled computer has Ubuntu installed, you can run `setup/setup_ubuntu.sh` to set it up.
-
-On your Mac, you will need to install grpcio using Conda and then copy it over to your pipenv's site-packages (see `setup/setup_mac.sh`).
-
-3. After Ubuntu has been installed, you will need to add your public SSH key to ~/.ssh/authorized_keys on your Ubuntu 
-instance so that your local computer will be able to connect to the Ubuntu instance for training/tuning.
-## Setup
-1. Create a YAML configuration file named `ray_config.yaml` in the root directory of your project.
-1. Ray QuickStart expects a configuration file named `ray_config.yaml` to be present in the root directory of your project.
+I recently got a GPU card for my Windows computer to allow me to train my ML models more quickly. I wanted to continue
+developing from my Mac computer, but the process of copying my code and data to my Windows computer, training my models, 
+and then copying the trained models back to my Mac computer was cumbersome. 
+
+I found the Ray library and decided to use it to train my models remotely on my Windows computer after developing it 
+locally on my Mac computer. I ran into some issues getting started with Ray, however, so I created this project to make 
+it easier for others to get started.
+
+Ray Quickstart is available as both a [PyPI package](https://pypi.org/project/ray-quickstart/) and as a 
+[GitHub repo](https://github.com/tuyentruong/ray-quickstart). You should install the PyPI package if you want to add 
+remote training and tuning to your own ML project. The GitHub repo includes an example project that you can run to see 
+the Ray QuickStart library in action.
+
+
+## What Does Ray QuickStart Do?
+
+Ray QuickStart will:
+1. Install the packages in your project's Pipfile on your remote computer without needing to set up an auto-scaling Ray cluster.
+2. Clean up your trials directories before training/tuning starts (optional).
+3. Use Ray to sync your Python project code to your remote computer and train/tune your model there.
+4. Sync the checkpoints from your training/tuning back to your computer.
+
+## Setting Up Your GPU-Enabled Computer
+
+My setup is as follows:
+1. I have a Mac computer that I use for development.
+2. I have a Windows 11 computer with a GPU card installed that I want to use for trainging/tuning.
+
+I decided to set up my Ray cluster on an Ubuntu instance on my Windows computer using WSL2. I originally tried to
+set up a Ray cluster on my Windows computer, but I ran into some path issues while trying to sync the checkpoints. 
+
+To set up Ubuntu on your Windows computer, you can run `setup\setup_windows.bat` found in GitHub repo. This will create 
+an Ubuntu 22.04 instance on your Windows computer and configure it with a Ray cluster. It will also open up the SSH port 
+and the ports used by Ray in your Windows firewall. A terminal window will open during the setup process. You can ignore 
+any errors that the window shows and close it once setup has completed.
+
+Once the Ubuntu instance has been set up, you will need to start it. It is recommended that you start the Ubuntu instance
+using the `scripts\ubuntu_start.bat` script. The script will ensure that port forwarding has been set up correctly so
+that you will be able to communicate with the Ray cluster on the Ubuntu instance from your local computer.
+
+Finally, you will need to add your public SSH key to ~/.ssh/authorized_keys on your Ubuntu instance so that your local
+computer will be able to connect to the Ubuntu instance to configure your runtime environment and sync the checkpoints
+using rsync.
+
+If your GPU-enabled computer has Linux installed, you can take a look at `setup\setup_ubuntu.sh` for the setup that needs
+to be done to install and configure Ray cluster. The setup script was written for Ubuntu, but hopefully it will be easy 
+to adapt for other distros.
+
+
+## Setting Up Your Local Computer
+
+1. Create a YAML configuration file named `ray_config.yaml` in your project. The file should contain the following
+   information:
+
+```yaml
+driver:
+  user: 'tuyen' # Your username on your local computer
+  private_key_file: '~/.ssh/id_rsa' # The private key file that will be used to connect to the remote computer
+
+ray_head:
+  hostname_or_ip_address: '192.168.2.4' # The hostname or IP address of the remote computer
+  client_server_port: 10001 # The port that will be used to communicate with the Ray cluster
+
+worker:
+  user: 'tuyen' # The user that will be used to connect to the remote computer using SSH
+  hostname_or_ip_address: '192.168.2.4' # The hostname or IP address of the remote computer
+  ssh_port: 22 # The port that will be used to connect to the remote computer using SSH
+  platform: 'linux' # The platform that the remote computer is running on (used for path conversion)
+```
+
+2. Add a call to `initialize_ray_with_syncer()` to your ML project code to initialize the connection with the Ray cluster.
+   The call will return a syncer object.
+
+3. Pass the syncer object to the `fit()` call in the subclass of `ray.train.base_trainer.BaseTrainer` that you are using 
+   to train your model. The syncer object will be used to sync your checkpoints back to your local computer after training.
+
 
 ## Troubleshooting
 
 **When I connect to the Ubuntu WSL instance, it says that the GPU is not available. What can I do to fix this?** 
    
-I got stumped on this issue for a while. From https://github.com/microsoft/WSL/issues/9185, I discovered the cause:
+I got stumped on this issue for a while. From https://github.com/microsoft/WSL/issues/9185, it seems to be user permission
+issue:
    
 > There is an issue when nvidia-smi doesn't work when one instance is launched as Administrator and another as a non-Administrator.
 
-When I started the Ubuntu WSL instance from the command line and passed in the `--user` flag with the same username as 
-in Windows, then it worked. It is recommended that you start the Ubuntu WSL instance using the `ubuntu_start.sh` script.
+It started working when I started the Ubuntu WSL instance from the command line and passed in the `--user` flag with the same username as 
+my Windows's username. It is recommended that you start the Ubuntu WSL instance using the `scripts\ubuntu_start.bat` script
+to avoid this issue.
+
 
-**I am getting ModuleNotFoundError: No module named '[module]' when I try to training remotely. How do I fix it?**
+## Future Directions
 
-You will need to install all your package dependencies to the ray-quickstart project because that is the project used 
-when starting the Ray cluster. Without those packages installed, Ray will fail when trying to export your code to the
-remote machine for training.
+1. Add support for training on a cluster in the cloud.
```

### Comparing `ray-quickstart-0.1.8/src/ray_quickstart.egg-info/SOURCES.txt` & `ray-quickstart-0.1.9/src/ray_quickstart.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 README.md
 pyproject.toml
 setup.py
 scripts/ray_start.bat
 scripts/ray_start.sh
 scripts/ray_stop.bat
 scripts/ray_stop.sh
-scripts/ubuntu_start.bat
-scripts/ubuntu_stop.bat
 src/ray_quickstart/__init__.py
 src/ray_quickstart/init.py
 src/ray_quickstart/monkey_patch.py
 src/ray_quickstart/rsync_syncer.py
 src/ray_quickstart.egg-info/PKG-INFO
 src/ray_quickstart.egg-info/SOURCES.txt
 src/ray_quickstart.egg-info/dependency_links.txt
```

