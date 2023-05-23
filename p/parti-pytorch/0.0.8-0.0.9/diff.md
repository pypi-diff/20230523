# Comparing `tmp/parti-pytorch-0.0.8.tar.gz` & `tmp/parti-pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parti-pytorch-0.0.8.tar", last modified: Fri Jun 24 17:22:41 2022, max compression
+gzip compressed data, was "parti-pytorch-0.0.9.tar", last modified: Fri Jun 24 17:33:18 2022, max compression
```

## Comparing `parti-pytorch-0.0.8.tar` & `parti-pytorch-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:22:41.140573 parti-pytorch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-06-24 17:22:29.000000 parti-pytorch-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-06-24 17:22:41.140573 parti-pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4285 2022-06-24 17:22:29.000000 parti-pytorch-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:22:41.140573 parti-pytorch-0.0.8/parti_pytorch/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-24 17:22:29.000000 parti-pytorch-0.0.8/parti_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      943 2022-06-24 17:22:29.000000 parti-pytorch-0.0.8/parti_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (121)    13105 2022-06-24 17:22:29.000000 parti-pytorch-0.0.8/parti_pytorch/parti_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-06-24 17:22:29.000000 parti-pytorch-0.0.8/parti_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (121)    16937 2022-06-24 17:22:29.000000 parti-pytorch-0.0.8/parti_pytorch/vit_vqgan.py
--rw-r--r--   0 runner    (1001) docker     (121)     8330 2022-06-24 17:22:29.000000 parti-pytorch-0.0.8/parti_pytorch/vit_vqgan_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:22:41.140573 parti-pytorch-0.0.8/parti_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-06-24 17:22:40.000000 parti-pytorch-0.0.8/parti_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-06-24 17:22:41.000000 parti-pytorch-0.0.8/parti_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 17:22:40.000000 parti-pytorch-0.0.8/parti_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-24 17:22:40.000000 parti-pytorch-0.0.8/parti_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-24 17:22:41.000000 parti-pytorch-0.0.8/parti_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-24 17:22:41.140573 parti-pytorch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-06-24 17:22:29.000000 parti-pytorch-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:33:18.761191 parti-pytorch-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-06-24 17:33:06.000000 parti-pytorch-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2022-06-24 17:33:18.761191 parti-pytorch-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4462 2022-06-24 17:33:06.000000 parti-pytorch-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:33:18.761191 parti-pytorch-0.0.9/parti_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-06-24 17:33:06.000000 parti-pytorch-0.0.9/parti_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      943 2022-06-24 17:33:06.000000 parti-pytorch-0.0.9/parti_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13105 2022-06-24 17:33:06.000000 parti-pytorch-0.0.9/parti_pytorch/parti_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-06-24 17:33:06.000000 parti-pytorch-0.0.9/parti_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17106 2022-06-24 17:33:06.000000 parti-pytorch-0.0.9/parti_pytorch/vit_vqgan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8330 2022-06-24 17:33:06.000000 parti-pytorch-0.0.9/parti_pytorch/vit_vqgan_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:33:18.761191 parti-pytorch-0.0.9/parti_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2022-06-24 17:33:18.000000 parti-pytorch-0.0.9/parti_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-06-24 17:33:18.000000 parti-pytorch-0.0.9/parti_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 17:33:18.000000 parti-pytorch-0.0.9/parti_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-06-24 17:33:18.000000 parti-pytorch-0.0.9/parti_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-24 17:33:18.000000 parti-pytorch-0.0.9/parti_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-24 17:33:18.761191 parti-pytorch-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-06-24 17:33:06.000000 parti-pytorch-0.0.9/setup.py
```

### Comparing `parti-pytorch-0.0.8/LICENSE` & `parti-pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `parti-pytorch-0.0.8/PKG-INFO` & `parti-pytorch-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parti-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Parti - Pathways Autoregressive Text-to-Image Model - Pytorch
 Home-page: https://github.com/lucidrains/parti-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-image
 Classifier: Development Status :: 4 - Beta
```

### Comparing `parti-pytorch-0.0.8/README.md` & `parti-pytorch-0.0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 # first instantiate your ViT VQGan VAE
 # a VQGan VAE made of transformers
 
 vit_vae = VitVQGanVAE(
     dim = 512,               # dimensions
     image_size = 256,        # target image size
+    patch_size = 16,         # patch size in the image that attends to each other
     num_layers = 4           # number of layers
 ).cuda()
 
 images = torch.randn(4, 3, 256, 256).cuda()
 
 loss = vit_vae(images, return_loss = True)
 loss.backward()
@@ -94,14 +95,15 @@
 - [ ] get working vit vqgan-vae trainer code, as discriminator needs to be trained
 - [ ] preencoding of text with designated t5
 - [ ] training code for parti
 - [ ] inference caching
 - [ ] automatic filtering with Coca https://github.com/lucidrains/CoCa-pytorch
 - [ ] bring in the super-resoluting convolutional net mentioned in the paper, with training code
 - [ ] initialize 2d rel pos bias in conv-like pattern
+- [ ] cite all techniques adopted from vision transformer literature in vit vqgan if they work
 
 ## Citations
 
 ```bibtex
 @inproceedings{Yu2022Pathways
     title   = {Pathways Autoregressive Text-to-Image Model},
     author  = {Jiahui Yu*, Yuanzhong Xu†, Jing Yu Koh†, Thang Luong†, Gunjan Baid†, Zirui Wang†, Vijay Vasudevan†, Alexander Ku†, Yinfei Yang, Burcu Karagol Ayan, Ben Hutchinson, Wei Han, Zarana Parekh, Xin Li, Han Zhang, Jason Baldridge†, Yonghui Wu*},
```

#### html2text {}

```diff
@@ -1,42 +1,44 @@
 [./parti.jpeg] ## Parti - Pytorch (wip) Implementation of Parti, Google's pure
 attention-based text-to-image neural network, in Pytorch Yannic_Kilcher Please
 join [Join_us_on_Discord] if you are interested in helping out with the
 replication with the LAION community ## Install ```bash $ pip install parti-
 pytorch ``` ## Usage ```python import torch from parti_pytorch import Parti,
 VitVQGanVAE # first instantiate your ViT VQGan VAE # a VQGan VAE made of
 transformers vit_vae = VitVQGanVAE( dim = 512, # dimensions image_size = 256, #
-target image size num_layers = 4 # number of layers ).cuda() images =
-torch.randn(4, 3, 256, 256).cuda() loss = vit_vae(images, return_loss = True)
-loss.backward() # do the above with as many images as possible # then you
-plugin the ViT VqGan VAE into your Parti parti = Parti( vae = vit_vae, # vit
-vqgan vae dim = 512, # model dimension depth = 8, # depth dim_head = 64, #
-attention head dimension heads = 8, # attention heads dropout = 0., # dropout
-cond_drop_prob = 0.25, # conditional dropout, for classifier free guidance
-ff_mult = 4, # feedforward expansion factor t5_name = 't5-large', # name of
-your T5 ) # ready your training text and images texts = [ 'a child screaming at
-finding a worm within a half-eaten apple', 'lizard running across the desert on
-two feet', 'waking up to a psychedelic landscape', 'seashells sparkling in the
-shallow waters' ] images = torch.randn(4, 3, 256, 256).cuda() # feed it into
-your parti instance, with return_loss set to True loss = parti( texts = texts,
-images = images, return_loss = True ) loss.backward() # do this for a long time
-on much data # then... images = parti.generate(texts = [ 'a whale breaching
-from afar', 'young girl blowing out candles on her birthday cake', 'fireworks
-with blue and green sparkles' ], cond_scale = 3., return_pil_images = True) #
-conditioning scale for classifier free guidance # List[PILImages] (256 x 256
-RGB) ``` ## Appreciation - StabilityAI for the sponsorship, as well as my other
-sponsors, for affording me the independence to open source artificial
-intelligence. - ð¤_Huggingface for the transformers library and the ease for
-encoding text with T5 language model ## Todo - [x] add 2d relative positional
-bias to parti autoregressive transformer - [ ] get working vit vqgan-vae
-trainer code, as discriminator needs to be trained - [ ] preencoding of text
-with designated t5 - [ ] training code for parti - [ ] inference caching - [ ]
-automatic filtering with Coca https://github.com/lucidrains/CoCa-pytorch - [ ]
-bring in the super-resoluting convolutional net mentioned in the paper, with
-training code - [ ] initialize 2d rel pos bias in conv-like pattern ##
+target image size patch_size = 16, # patch size in the image that attends to
+each other num_layers = 4 # number of layers ).cuda() images = torch.randn(4,
+3, 256, 256).cuda() loss = vit_vae(images, return_loss = True) loss.backward()
+# do the above with as many images as possible # then you plugin the ViT VqGan
+VAE into your Parti parti = Parti( vae = vit_vae, # vit vqgan vae dim = 512, #
+model dimension depth = 8, # depth dim_head = 64, # attention head dimension
+heads = 8, # attention heads dropout = 0., # dropout cond_drop_prob = 0.25, #
+conditional dropout, for classifier free guidance ff_mult = 4, # feedforward
+expansion factor t5_name = 't5-large', # name of your T5 ) # ready your
+training text and images texts = [ 'a child screaming at finding a worm within
+a half-eaten apple', 'lizard running across the desert on two feet', 'waking up
+to a psychedelic landscape', 'seashells sparkling in the shallow waters' ]
+images = torch.randn(4, 3, 256, 256).cuda() # feed it into your parti instance,
+with return_loss set to True loss = parti( texts = texts, images = images,
+return_loss = True ) loss.backward() # do this for a long time on much data #
+then... images = parti.generate(texts = [ 'a whale breaching from afar', 'young
+girl blowing out candles on her birthday cake', 'fireworks with blue and green
+sparkles' ], cond_scale = 3., return_pil_images = True) # conditioning scale
+for classifier free guidance # List[PILImages] (256 x 256 RGB) ``` ##
+Appreciation - StabilityAI for the sponsorship, as well as my other sponsors,
+for affording me the independence to open source artificial intelligence. -
+ð¤_Huggingface for the transformers library and the ease for encoding text
+with T5 language model ## Todo - [x] add 2d relative positional bias to parti
+autoregressive transformer - [ ] get working vit vqgan-vae trainer code, as
+discriminator needs to be trained - [ ] preencoding of text with designated t5
+- [ ] training code for parti - [ ] inference caching - [ ] automatic filtering
+with Coca https://github.com/lucidrains/CoCa-pytorch - [ ] bring in the super-
+resoluting convolutional net mentioned in the paper, with training code - [ ]
+initialize 2d rel pos bias in conv-like pattern - [ ] cite all techniques
+adopted from vision transformer literature in vit vqgan if they work ##
 Citations ```bibtex @inproceedings{Yu2022Pathways title = {Pathways
 Autoregressive Text-to-Image Model}, author = {Jiahui Yu*, Yuanzhong Xuâ ,
 Jing Yu Kohâ , Thang Luongâ , Gunjan Baidâ , Zirui Wangâ , Vijay
 Vasudevanâ , Alexander Kuâ , Yinfei Yang, Burcu Karagol Ayan, Ben Hutchinson,
 Wei Han, Zarana Parekh, Xin Li, Han Zhang, Jason Baldridgeâ , Yonghui Wu*},
 year = {2022} } ``` ```bibtex @article{Shleifer2021NormFormerIT, title =
 {NormFormer: Improved Transformer Pretraining with Extra Normalization}, author
```

### Comparing `parti-pytorch-0.0.8/parti_pytorch/optimizer.py` & `parti-pytorch-0.0.9/parti_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `parti-pytorch-0.0.8/parti_pytorch/parti_pytorch.py` & `parti-pytorch-0.0.9/parti_pytorch/parti_pytorch.py`

 * *Files identical despite different names*

### Comparing `parti-pytorch-0.0.8/parti_pytorch/t5.py` & `parti-pytorch-0.0.9/parti_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `parti-pytorch-0.0.8/parti_pytorch/vit_vqgan.py` & `parti-pytorch-0.0.9/parti_pytorch/vit_vqgan.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,28 +241,32 @@
         super().__init__()
         self.norm = ChanLayerNorm(dim)
         self.heads = heads
         self.scale = dim_head ** -0.5
         inner_dim = dim_head * heads
 
         self.to_qkv = nn.Conv2d(dim, inner_dim * 3, 1, bias = False)
+        self.primer_ds_convs = nn.ModuleList([PEG(inner_dim) for _ in range(3)])
+
         self.to_out = nn.Conv2d(inner_dim, dim, 1, bias = False)
 
         self.rel_pos_bias = None
         if rel_pos_bias:
             assert exists(fmap_size)
             self.rel_pos_bias = RelPosBias2d(fmap_size, heads)
 
     def forward(self, x):
         fmap_size = x.shape[-1]
         h = self.heads
 
         x = self.norm(x)
 
         q, k, v = self.to_qkv(x).chunk(3, dim = 1)
+
+        q, k, v = [ds_conv(t) for ds_conv, t in zip(self.primer_ds_convs, (q, k, v))]
         q, k, v = rearrange_many((q, k, v), 'b (h d) x y -> b h (x y) d', h = h)
 
         q = q * self.scale
         sim = einsum('b h i d, b h j d -> b h i j', q, k)
 
         if exists(self.rel_pos_bias):
             sim = sim + self.rel_pos_bias(sim)
```

### Comparing `parti-pytorch-0.0.8/parti_pytorch/vit_vqgan_trainer.py` & `parti-pytorch-0.0.9/parti_pytorch/vit_vqgan_trainer.py`

 * *Files identical despite different names*

### Comparing `parti-pytorch-0.0.8/parti_pytorch.egg-info/PKG-INFO` & `parti-pytorch-0.0.9/parti_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parti-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Parti - Pathways Autoregressive Text-to-Image Model - Pytorch
 Home-page: https://github.com/lucidrains/parti-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-image
 Classifier: Development Status :: 4 - Beta
```

### Comparing `parti-pytorch-0.0.8/setup.py` & `parti-pytorch-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'parti-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'Parti - Pathways Autoregressive Text-to-Image Model - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/parti-pytorch',
   keywords = [
```

