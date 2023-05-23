# Comparing `tmp/musegan-0.1.3.tar.gz` & `tmp/musegan-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musegan-0.1.3.tar", last modified: Wed May 10 12:36:20 2023, max compression
+gzip compressed data, was "musegan-0.1.4.tar", last modified: Tue May 23 12:56:51 2023, max compression
```

## Comparing `musegan-0.1.3.tar` & `musegan-0.1.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 12:36:20.114116 musegan-0.1.3/
--rw-rw-rw-   0        0        0     1094 2023-04-25 05:46:28.000000 musegan-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2828 2023-05-10 12:36:20.114116 musegan-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2145 2023-05-10 06:38:22.000000 musegan-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 12:36:20.051663 musegan-0.1.3/musegan/
-drwxrwxrwx   0        0        0        0 2023-05-10 12:36:20.082906 musegan-0.1.3/musegan/musegan/
--rw-rw-rw-   0        0        0      420 2023-05-08 14:02:00.000000 musegan-0.1.3/musegan/musegan/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-09 08:17:02.000000 musegan-0.1.3/musegan/musegan/_version.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:36:20.098492 musegan-0.1.3/musegan/musegan/archs/
--rw-rw-rw-   0        0        0      376 2023-04-25 08:04:27.000000 musegan-0.1.3/musegan/musegan/archs/__init__.py
--rw-rw-rw-   0        0        0     3686 2023-04-25 08:06:16.000000 musegan-0.1.3/musegan/musegan/archs/bar_generator.py
--rw-rw-rw-   0        0        0     3590 2023-04-25 05:46:28.000000 musegan-0.1.3/musegan/musegan/archs/critic.py
--rw-rw-rw-   0        0        0     3659 2023-04-26 07:29:58.000000 musegan-0.1.3/musegan/musegan/archs/generator.py
--rw-rw-rw-   0        0        0     1909 2023-05-04 06:26:35.000000 musegan-0.1.3/musegan/musegan/archs/temp_network.py
--rw-rw-rw-   0        0        0     1342 2023-04-28 09:57:42.000000 musegan-0.1.3/musegan/musegan/archs/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:36:20.098492 musegan-0.1.3/musegan/musegan/dataset/
--rw-rw-rw-   0        0        0      174 2023-04-28 12:56:56.000000 musegan-0.1.3/musegan/musegan/dataset/__init__.py
--rw-rw-rw-   0        0        0     5443 2023-05-03 06:12:36.000000 musegan-0.1.3/musegan/musegan/dataset/data_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:36:20.098492 musegan-0.1.3/musegan/musegan/trainner/
--rw-rw-rw-   0        0        0      188 2023-04-26 07:13:54.000000 musegan-0.1.3/musegan/musegan/trainner/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-04-25 05:46:28.000000 musegan-0.1.3/musegan/musegan/trainner/criterion.py
--rw-rw-rw-   0        0        0    10398 2023-05-03 11:42:28.000000 musegan-0.1.3/musegan/musegan/trainner/trainer.py
-drwxrwxrwx   0        0        0        0 2023-05-10 12:36:20.082906 musegan-0.1.3/musegan/musegan.egg-info/
--rw-rw-rw-   0        0        0     2828 2023-05-10 12:36:20.000000 musegan-0.1.3/musegan/musegan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-05-10 12:36:20.000000 musegan-0.1.3/musegan/musegan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 12:36:20.000000 musegan-0.1.3/musegan/musegan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-10 12:36:20.000000 musegan-0.1.3/musegan/musegan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-10 12:36:20.000000 musegan-0.1.3/musegan/musegan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-09 06:31:55.000000 musegan-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      775 2023-05-10 12:36:20.114116 musegan-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 12:56:51.824084 musegan-0.1.4/
+-rw-rw-rw-   0        0        0     1094 2023-05-22 07:26:14.000000 musegan-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     2881 2023-05-23 12:56:51.824084 musegan-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2213 2023-05-22 07:26:14.000000 musegan-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 12:56:51.785965 musegan-0.1.4/musegan/
+drwxrwxrwx   0        0        0        0 2023-05-23 12:56:51.798533 musegan-0.1.4/musegan/musegan/
+-rw-rw-rw-   0        0        0      420 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:56:51.817031 musegan-0.1.4/musegan/musegan/archs/
+-rw-rw-rw-   0        0        0      376 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/archs/__init__.py
+-rw-rw-rw-   0        0        0     3686 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/archs/bar_generator.py
+-rw-rw-rw-   0        0        0     3590 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/archs/critic.py
+-rw-rw-rw-   0        0        0     3659 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/archs/generator.py
+-rw-rw-rw-   0        0        0     1909 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/archs/temp_network.py
+-rw-rw-rw-   0        0        0     1342 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/archs/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:56:51.820013 musegan-0.1.4/musegan/musegan/dataset/
+-rw-rw-rw-   0        0        0      174 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/dataset/__init__.py
+-rw-rw-rw-   0        0        0     5443 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/dataset/data_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:56:51.823023 musegan-0.1.4/musegan/musegan/trainner/
+-rw-rw-rw-   0        0        0      188 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/trainner/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-05-22 07:26:14.000000 musegan-0.1.4/musegan/musegan/trainner/criterion.py
+-rw-rw-rw-   0        0        0    10405 2023-05-23 12:41:03.000000 musegan-0.1.4/musegan/musegan/trainner/trainer.py
+drwxrwxrwx   0        0        0        0 2023-05-23 12:56:51.811616 musegan-0.1.4/musegan/musegan.egg-info/
+-rw-rw-rw-   0        0        0     2881 2023-05-23 12:56:51.000000 musegan-0.1.4/musegan/musegan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-05-23 12:56:51.000000 musegan-0.1.4/musegan/musegan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 12:56:51.000000 musegan-0.1.4/musegan/musegan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-23 12:56:51.000000 musegan-0.1.4/musegan/musegan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-23 12:56:51.000000 musegan-0.1.4/musegan/musegan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-22 07:26:14.000000 musegan-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      817 2023-05-23 12:56:51.825106 musegan-0.1.4/setup.cfg
```

### Comparing `musegan-0.1.3/LICENSE` & `musegan-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `musegan-0.1.3/PKG-INFO` & `musegan-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pytorch implementation of musegan
 Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
 Author: Clifford Njoroge
 Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 MuseGAN
 =========
 ![PyPI - License](https://img.shields.io/pypi/l/musegan)
 [![PyPI](https://img.shields.io/pypi/v/musegan)](https://pypi.org/project/musegan/)
```

### Comparing `musegan-0.1.3/README.md` & `musegan-0.1.4/README.md`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-MuseGAN
-=========
-![PyPI - License](https://img.shields.io/pypi/l/musegan)
-[![PyPI](https://img.shields.io/pypi/v/musegan)](https://pypi.org/project/musegan/)
-![PyPI - Downloads](https://img.shields.io/pypi/dw/musegan)
-
-- A Pytorch implementation of MuseGAN
-- ***Note :*** Only linux BSD support due to SharedArray usage which is a linux only pip package
-
-
-
-
-[MuseGAN](https://arxiv.org/abs/1709.06298) is a generative model which allows to
-generate music.
-
-Usage
-=======
-The musegan package contains all the schema needed to train and generate your own music in MIDI format.
-There are two ways of using the musegan package;
-
-1. Using the PYPI package.
-   - To use it use the command: `pip install musegan` to install all the necessary packages
-
-2. Building from the source 
-   - First clone the repository to your local directory with `git`
-   - Open your local Terminal/Command Shell and run the following commands
-    ```shell
-    cd musegan-pytorch # change directory to the cloned repository
-    #use any of the following some will work dependent on your operating system
-    #try
-    python3 setup.py develop
-    #or
-    pip install .
-    #or
-    pip install -e
-    ```
-    - To test run the following in your python terminal;
-    ```py
-    >> import musegan
-    >> print(musegan__version__)
-    # which should return the latest musegan version according to the time you read this
-    0.0.9
-    ```
-    Now you should be able to use zthe musegan packages
-    
-## Table of content
-
-- [Training](https://github.com/cliffordkleinsr/musegan-pytorch/edit/dev/README.md#training)
-- [License](#license)
-- [Links](#links)
-
-## Training 
-
-See this [colab](https://colab.research.google.com/drive/1NF2t1dvqxeblZfd7BL4Gfn4SW-xEzgGg?authuser=3#scrollTo=9bj_FWvAArPI)  notebook for more details of training process.
-* The model components and utils are under `musegan/archs` folder.
-* The Midi `torch.utils.dataset` is under `musegan/dataset/data_utils.py`.
-* The training Functions and criterions can be found in the `musegan/trainner` folder
-
-
-
-
-## License
-
-This project is licensed under MIT.
-
-## Links
-
-* [MuseGAN](https://arxiv.org/abs/1709.06298)
+MuseGAN
+=========
+![PyPI - License](https://img.shields.io/pypi/l/musegan)
+[![PyPI](https://img.shields.io/pypi/v/musegan)](https://pypi.org/project/musegan/)
+![PyPI - Downloads](https://img.shields.io/pypi/dw/musegan)
+
+- A Pytorch implementation of MuseGAN
+- ***Note :*** Only linux BSD support due to SharedArray usage which is a linux only pip package
+
+
+
+
+[MuseGAN](https://arxiv.org/abs/1709.06298) is a generative model which allows to
+generate music.
+
+Usage
+=======
+The musegan package contains all the schema needed to train and generate your own music in MIDI format.
+There are two ways of using the musegan package;
+
+1. Using the PYPI package.
+   - To use it use the command: `pip install musegan` to install all the necessary packages
+
+2. Building from the source 
+   - First clone the repository to your local directory with `git`
+   - Open your local Terminal/Command Shell and run the following commands
+    ```shell
+    cd musegan-pytorch # change directory to the cloned repository
+    #use any of the following some will work dependent on your operating system
+    #try
+    python3 setup.py develop
+    #or
+    pip install .
+    #or
+    pip install -e
+    ```
+    - To test run the following in your python terminal;
+    ```py
+    >> import musegan
+    >> print(musegan__version__)
+    # which should return the latest musegan version according to the time you read this
+    0.0.9
+    ```
+    Now you should be able to use zthe musegan packages
+    
+## Table of content
+
+- [Training](https://github.com/cliffordkleinsr/musegan-pytorch/edit/dev/README.md#training)
+- [License](#license)
+- [Links](#links)
+
+## Training 
+
+See this [colab](https://colab.research.google.com/drive/1NF2t1dvqxeblZfd7BL4Gfn4SW-xEzgGg?authuser=3#scrollTo=9bj_FWvAArPI)  notebook for more details of training process.
+* The model components and utils are under `musegan/archs` folder.
+* The Midi `torch.utils.dataset` is under `musegan/dataset/data_utils.py`.
+* The training Functions and criterions can be found in the `musegan/trainner` folder
+
+
+
+
+## License
+
+This project is licensed under MIT.
+
+## Links
+
+* [MuseGAN](https://arxiv.org/abs/1709.06298)
```

### Comparing `musegan-0.1.3/musegan/musegan/archs/bar_generator.py` & `musegan-0.1.4/musegan/musegan/archs/bar_generator.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.3/musegan/musegan/archs/critic.py` & `musegan-0.1.4/musegan/musegan/archs/critic.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.3/musegan/musegan/archs/generator.py` & `musegan-0.1.4/musegan/musegan/archs/generator.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.3/musegan/musegan/archs/temp_network.py` & `musegan-0.1.4/musegan/musegan/archs/temp_network.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.3/musegan/musegan/archs/utils.py` & `musegan-0.1.4/musegan/musegan/archs/utils.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.3/musegan/musegan/dataset/data_utils.py` & `musegan-0.1.4/musegan/musegan/dataset/data_utils.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.3/musegan/musegan/trainner/criterion.py` & `musegan-0.1.4/musegan/musegan/trainner/criterion.py`

 * *Files identical despite different names*

### Comparing `musegan-0.1.3/musegan/musegan/trainner/trainer.py` & `musegan-0.1.4/musegan/musegan/trainner/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         start_epoch: int = 0,
         epochs: int = 500,
         batch_size: int = 64,
         repeat: int = 5,
         #(deprecated)display_step: int = 10,
         melody_groove: int = 4,
         save_checkpoint: bool = True,
-        model_name: str = "museGAN_netG"
+        model_name: str = "museGAN"
     ) -> None:
         os.makedirs(self.ckpt_path, exist_ok=True)
         """
         Why rand/randn?
                 - First, as you see from the documentation numpy.random.randn
                 generates samples from the normal distribution,
                 while numpy.random.rand from a uniform distribution (in the range [0,1)).
@@ -172,15 +172,15 @@
                     #SAVE DISC MODEL STATE DICT
                     if save_checkpoint:
                         checkpoint = {
                           'epoch': epoch+1,
                           'state_dict': self.critic.state_dict(),
                           'optimizer': self.c_optimizer.state_dict(),
                           }
-                        self.save_ckp(checkpoint, os.path.join(self.ckpt_path, '{}-{}.pth'.format(model_name, epoch)))
+                        self.save_ckp(checkpoint, os.path.join(self.ckpt_path, '{}_Net_G-{}.pth'.format(model_name, epoch)))
                     # Train Generator
                     self.g_optimizer.zero_grad()
                     # Very important note
                     # chords shape: (batch_size, z_dimension)
                     # style shape: (batch_size, z_dimension)
                     # melody shape: (batch_size, n_tracks, z_dimension)
                     # groove shape: (batch_size, n_tracks, z_dimension)
@@ -222,15 +222,15 @@
             #SAVE GEN MODEL STATE DICT
             if save_checkpoint:
                 checkpoint = {
                   'epoch': epoch+1,
                   'state_dict': self.generator.state_dict(),
                   'optimizer': self.g_optimizer.state_dict(),
                   }
-                self.save_ckp(checkpoint, os.path.join(self.ckpt_path, '{}-{}.pth'.format(model_name, epoch)))
+                self.save_ckp(checkpoint, os.path.join(self.ckpt_path, '{}_Net_D-{}.pth'.format(model_name, epoch)))
             """
                 Loss Statistics
             """
             torch.cuda.empty_cache()
             #(deprecated)if epoch % display_step == 0:
              #(deprecated)   print(f"Epoch {epoch}/{epochs} | Generator loss: {e_gloss:.3f} | Critic loss: {e_closs:.3f}")
               #(deprecated)  print(f"(fake: {e_cfloss:.3f}, real: {e_crloss:.3f}, penalty: {e_cploss:.3f})")
```

### Comparing `musegan-0.1.3/musegan/musegan.egg-info/PKG-INFO` & `musegan-0.1.4/musegan/musegan.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: musegan
-Version: 0.1.3
+Version: 0.1.4
 Summary: A pytorch implementation of musegan
 Home-page: https://github.com/cliffordkleinsr/musegan-pytorch
 Author: Clifford Njoroge
 Author-email: cnjoroge@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 MuseGAN
 =========
 ![PyPI - License](https://img.shields.io/pypi/l/musegan)
 [![PyPI](https://img.shields.io/pypi/v/musegan)](https://pypi.org/project/musegan/)
```

### Comparing `musegan-0.1.3/musegan/musegan.egg-info/SOURCES.txt` & `musegan-0.1.4/musegan/musegan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `musegan-0.1.3/setup.cfg` & `musegan-0.1.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 7573 6567 616e 0d0a 7665 7273   = musegan..vers
-00000020: 696f 6e20 3d20 302e 312e 330d 0a61 7574  ion = 0.1.3..aut
+00000020: 696f 6e20 3d20 302e 312e 340d 0a61 7574  ion = 0.1.4..aut
 00000030: 686f 7220 3d20 436c 6966 666f 7264 204e  hor = Clifford N
 00000040: 6a6f 726f 6765 0d0a 6175 7468 6f72 5f65  joroge..author_e
 00000050: 6d61 696c 203d 2063 6e6a 6f72 6f67 6540  mail = cnjoroge@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2041 2070 7974 6f72  iption = A pytor
 00000080: 6368 2069 6d70 6c65 6d65 6e74 6174 696f  ch implementatio
 00000090: 6e20 6f66 206d 7573 6567 616e 0d0a 6c6f  n of musegan..lo
@@ -24,26 +24,29 @@
 00000170: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 00000180: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
 00000190: 2033 2e37 0d0a 0950 726f 6772 616d 6d69   3.7...Programmi
 000001a0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 000001b0: 7974 686f 6e20 3a3a 2033 2e38 0d0a 0950  ython :: 3.8...P
 000001c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 000001d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000001e0: 2033 2e39 0d0a 094c 6963 656e 7365 203a   3.9...License :
-000001f0: 3a20 4f53 4920 4170 7072 6f76 6564 203a  : OSI Approved :
-00000200: 3a20 4d49 5420 4c69 6365 6e73 650d 0a09  : MIT License...
-00000210: 4f70 6572 6174 696e 6720 5379 7374 656d  Operating System
-00000220: 203a 3a20 4f53 2049 6e64 6570 656e 6465   :: OS Independe
-00000230: 6e74 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d  nt....[options].
-00000240: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
-00000250: 0a09 3d20 6d75 7365 6761 6e0d 0a70 6163  ..= musegan..pac
-00000260: 6b61 6765 7320 3d20 6669 6e64 3a0d 0a70  kages = find:..p
-00000270: 7974 686f 6e5f 7265 7175 6972 6573 203d  ython_requires =
-00000280: 203e 3d33 2e39 0d0a 696e 7374 616c 6c5f   >=3.9..install_
-00000290: 7265 7175 6972 6573 203d 200d 0a09 6d75  requires = ...mu
-000002a0: 7369 6332 310d 0a09 6e75 6d70 790d 0a0d  sic21...numpy...
-000002b0: 0a5b 6f70 7469 6f6e 732e 7061 636b 6167  .[options.packag
-000002c0: 6573 2e66 696e 645d 0d0a 7768 6572 6520  es.find]..where 
-000002d0: 3d20 6d75 7365 6761 6e0d 0a0d 0a5b 6567  = musegan....[eg
-000002e0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
-000002f0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
-00000300: 3d20 300d 0a0d 0a                        = 0....
+000001e0: 2033 2e39 0d0a 0950 726f 6772 616d 6d69   3.9...Programmi
+000001f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000200: 7974 686f 6e20 3a3a 2033 2e31 300d 0a09  ython :: 3.10...
+00000210: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
+00000220: 7070 726f 7665 6420 3a3a 204d 4954 204c  pproved :: MIT L
+00000230: 6963 656e 7365 0d0a 094f 7065 7261 7469  icense...Operati
+00000240: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
+00000250: 496e 6465 7065 6e64 656e 740d 0a0d 0a5b  Independent....[
+00000260: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
+00000270: 655f 6469 7220 3d20 0d0a 093d 206d 7573  e_dir = ...= mus
+00000280: 6567 616e 0d0a 7061 636b 6167 6573 203d  egan..packages =
+00000290: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
+000002a0: 6571 7569 7265 7320 3d20 3e3d 332e 3130  equires = >=3.10
+000002b0: 0d0a 696e 7374 616c 6c5f 7265 7175 6972  ..install_requir
+000002c0: 6573 203d 200d 0a09 6d75 7369 6332 310d  es = ...music21.
+000002d0: 0a09 6e75 6d70 790d 0a0d 0a5b 6f70 7469  ..numpy....[opti
+000002e0: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
+000002f0: 645d 0d0a 7768 6572 6520 3d20 6d75 7365  d]..where = muse
+00000300: 6761 6e0d 0a0d 0a5b 6567 675f 696e 666f  gan....[egg_info
+00000310: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000320: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000330: 0a                                       .
```

