# Comparing `tmp/norman_ai-0.0.5.tar.gz` & `tmp/norman_ai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "norman_ai-0.0.5.tar", last modified: Tue May 16 16:25:06 2023, max compression
+gzip compressed data, was "norman_ai-0.0.6.tar", last modified: Tue May 23 20:22:37 2023, max compression
```

## Comparing `norman_ai-0.0.5.tar` & `norman_ai-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 16:25:06.003969 norman_ai-0.0.5/
--rw-rw-rw-   0        0        0     7818 2023-05-16 12:28:05.000000 norman_ai-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0       43 2023-05-16 12:28:05.000000 norman_ai-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0    29930 2023-05-16 16:25:06.003969 norman_ai-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    29417 2023-05-16 15:33:11.000000 norman_ai-0.0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-05-16 12:28:09.000000 norman_ai-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      688 2023-05-16 16:25:06.006227 norman_ai-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 16:25:05.975639 norman_ai-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 16:25:05.996028 norman_ai-0.0.5/src/norman_ai/
--rw-rw-rw-   0        0        0        0 2023-05-16 12:28:09.000000 norman_ai-0.0.5/src/norman_ai/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 16:25:06.002678 norman_ai-0.0.5/src/norman_ai/data/
--rw-rw-rw-   0        0        0    31392 2023-05-16 12:28:09.000000 norman_ai-0.0.5/src/norman_ai/data/norman_model1.h5
--rw-rw-rw-   0        0        0    46167 2023-05-16 12:28:09.000000 norman_ai-0.0.5/src/norman_ai/norman_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-16 16:25:06.000673 norman_ai-0.0.5/src/norman_ai.egg-info/
--rw-rw-rw-   0        0        0    29930 2023-05-16 16:25:05.000000 norman_ai-0.0.5/src/norman_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-16 16:25:05.000000 norman_ai-0.0.5/src/norman_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 16:25:05.000000 norman_ai-0.0.5/src/norman_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-16 16:25:05.000000 norman_ai-0.0.5/src/norman_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 20:22:37.396718 norman_ai-0.0.6/
+-rw-rw-rw-   0        0        0     7818 2023-05-16 12:28:05.000000 norman_ai-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       43 2023-05-16 12:28:05.000000 norman_ai-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    31048 2023-05-23 20:22:37.397958 norman_ai-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    30535 2023-05-23 20:06:43.000000 norman_ai-0.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-16 12:28:09.000000 norman_ai-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      688 2023-05-23 20:22:37.397958 norman_ai-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-23 20:22:37.368092 norman_ai-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 20:22:37.387960 norman_ai-0.0.6/src/norman_ai/
+-rw-rw-rw-   0        0        0       28 2023-05-23 14:39:46.000000 norman_ai-0.0.6/src/norman_ai/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:22:37.395437 norman_ai-0.0.6/src/norman_ai/data/
+-rw-rw-rw-   0        0        0    31392 2023-05-16 12:28:09.000000 norman_ai-0.0.6/src/norman_ai/data/norman_model1.h5
+-rw-rw-rw-   0        0        0    48803 2023-05-23 20:22:08.000000 norman_ai-0.0.6/src/norman_ai/norman_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-23 20:22:37.393540 norman_ai-0.0.6/src/norman_ai.egg-info/
+-rw-rw-rw-   0        0        0    31048 2023-05-23 20:22:37.000000 norman_ai-0.0.6/src/norman_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-23 20:22:37.000000 norman_ai-0.0.6/src/norman_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 20:22:37.000000 norman_ai-0.0.6/src/norman_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-23 20:22:37.000000 norman_ai-0.0.6/src/norman_ai.egg-info/top_level.txt
```

### Comparing `norman_ai-0.0.5/LICENSE.txt` & `norman_ai-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `norman_ai-0.0.5/PKG-INFO` & `norman_ai-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: norman_ai
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for automation of the novel object recognition test.
 Home-page: https://github.com/Seyij/norman
 Author: seyij_p
 Author-email: seyi.ooj@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
@@ -108,15 +108,15 @@
 import norman_ai.norman_functions as nf
 nf.run_gui()
 #a user interface should appear
 ```
 
 ### Video to DI walkthrough
 
-This section will take you through the basic steps required to get a DI from a video and to visualise NORMAN'S labelling, both using the provided user interface and with code. Make sure you are in the "norman_dlc" environment before proceeding.
+This section will take you through the basic steps required to get a DI from a video and to visualise NORMAN'S labelling, both using the provided user interface and with code. Make sure you are in the conda environment with norman and deeplabcut installed before proceeding. Please note that the user interface is primarily for demonstration purposes. To fully take advantage of NORMAN and process in batches for your own application, the code method is what you should use.
 
 ##### __*User interface method*__
 
 This uses the video file, a premade deeplabcut tracking file and an option norman model file in the demo folder of the project repository.
 
 ```bash
 #open the ipython program
@@ -175,26 +175,47 @@
 
 ```python
 
 #get path to pose document
 poses = r"test_79DLC_resnet_50_nort_demoSep26shuffle1_50000_filtered.csv"
 
 #create norkid python object
-# stating the novel object is the left object in the experiment
+# stating the novel object is the left object in the experiment, if the right object is novel state "right"
 x = nf.norkid(video, poses, "left")
 
 #show the discrimination index, the time spent with left object, time spent with right object
 print("DI:"+str(x.di)+", Time left:"+str(x.tl)+ ", Time right:"+ str(x.tr))
 
 #make an video visualisation of norman labelling the mouse video
 #this is optional as not every video result will need visualisation
 x.draw_vid()
 
 ```
-If you have trouble with this demo, please see the function details, which contain code examples and guidance on other functions in the NORMAN package. When attempting this with your own data, the most common error is related to the find_objects() function, as not all NORT mouse chambers are compatible with the object detection algorithm. If this is the case with your data I am happy to work on variant object detectors.
+If you have trouble with this demo, please see the function details, which contain code examples and guidance on other functions in the NORMAN package. 
+
+When using NORMAN with your own data, the most common problem is related to the find_objects() function, as not all NORT mouse chambers are compatible with the object detection algorithm. If this is the case you can use a conditional argument to draw the location of the experimental objects, and all the other parts of analysis will still be done automatically.
+![draw](https://github.com/Seyij/norman/blob/master/media/draw_objects.png)
+
+Hold the "r" key to reset the drawing and hold the escape key to exit once the drawing is complete.
+
+```python
+#if you wish to mark object locations yourself use draw_objects as true
+#hold r to reset the drawing
+#press escape to exit the window once the drawing is complete
+x = nf.norkid(video, poses, "left", draw_objects=True)
+
+#show the discrimination index, the time spent with left object, time spent with right object
+print("DI:"+str(x.di)+", Time left:"+str(x.tl)+ ", Time right:"+ str(x.tr))
+
+#make an video visualisation of norman labelling the mouse video
+#this is optional as not every video result will need visualisation
+x.draw_vid()
+
+
+```
 
 ### Function details
 
 
 Though very few NORMAN functions are needed to extract a discrimination index from a video, the NORMAN system has more functions for working with NORT images and videos. In this section I will explain how to use various functions in the library, with their use-cases and code examples. Where relevant I will also include information on how/why I made the function for context. Code examples below were done in the “demo” folder of the NORMAN project repository, using the “test_79.mp4” video as the source data. The top of each code example with show the arguments of the function and their defaults when applicable. For the full code of each function see the norman_functions.py file, and for the help doc strings use the python default function help().
 
 ```python
```

### Comparing `norman_ai-0.0.5/README.md` & `norman_ai-0.0.6/src/norman_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: norman-ai
+Version: 0.0.6
+Summary: A package for automation of the novel object recognition test.
+Home-page: https://github.com/Seyij/norman
+Author: seyij_p
+Author-email: seyi.ooj@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # The NORMAN System
 
 The Novel Object Recognition Mouse Analysis Network (NORMAN) system is a package for automation of the novel object recognition behavioural assay in neuroscience studies.
 
 PyPi link: https://pypi.org/project/norman-ai/
 
 This is part of work that will be presented as a poster at the [BNA Festival 2021](https://meetings.bna.org.uk/bna2021/) which runs from the 12-15th of April. It was developed as part of an MSci degree at the University of Dundee. The package and repository will be updated with video outlines and other details shortly, in the run up to the BNA festival.
@@ -94,15 +108,15 @@
 import norman_ai.norman_functions as nf
 nf.run_gui()
 #a user interface should appear
 ```
 
 ### Video to DI walkthrough
 
-This section will take you through the basic steps required to get a DI from a video and to visualise NORMAN'S labelling, both using the provided user interface and with code. Make sure you are in the "norman_dlc" environment before proceeding.
+This section will take you through the basic steps required to get a DI from a video and to visualise NORMAN'S labelling, both using the provided user interface and with code. Make sure you are in the conda environment with norman and deeplabcut installed before proceeding. Please note that the user interface is primarily for demonstration purposes. To fully take advantage of NORMAN and process in batches for your own application, the code method is what you should use.
 
 ##### __*User interface method*__
 
 This uses the video file, a premade deeplabcut tracking file and an option norman model file in the demo folder of the project repository.
 
 ```bash
 #open the ipython program
@@ -161,26 +175,47 @@
 
 ```python
 
 #get path to pose document
 poses = r"test_79DLC_resnet_50_nort_demoSep26shuffle1_50000_filtered.csv"
 
 #create norkid python object
-# stating the novel object is the left object in the experiment
+# stating the novel object is the left object in the experiment, if the right object is novel state "right"
 x = nf.norkid(video, poses, "left")
 
 #show the discrimination index, the time spent with left object, time spent with right object
 print("DI:"+str(x.di)+", Time left:"+str(x.tl)+ ", Time right:"+ str(x.tr))
 
 #make an video visualisation of norman labelling the mouse video
 #this is optional as not every video result will need visualisation
 x.draw_vid()
 
 ```
-If you have trouble with this demo, please see the function details, which contain code examples and guidance on other functions in the NORMAN package. When attempting this with your own data, the most common error is related to the find_objects() function, as not all NORT mouse chambers are compatible with the object detection algorithm. If this is the case with your data I am happy to work on variant object detectors.
+If you have trouble with this demo, please see the function details, which contain code examples and guidance on other functions in the NORMAN package. 
+
+When using NORMAN with your own data, the most common problem is related to the find_objects() function, as not all NORT mouse chambers are compatible with the object detection algorithm. If this is the case you can use a conditional argument to draw the location of the experimental objects, and all the other parts of analysis will still be done automatically.
+![draw](https://github.com/Seyij/norman/blob/master/media/draw_objects.png)
+
+Hold the "r" key to reset the drawing and hold the escape key to exit once the drawing is complete.
+
+```python
+#if you wish to mark object locations yourself use draw_objects as true
+#hold r to reset the drawing
+#press escape to exit the window once the drawing is complete
+x = nf.norkid(video, poses, "left", draw_objects=True)
+
+#show the discrimination index, the time spent with left object, time spent with right object
+print("DI:"+str(x.di)+", Time left:"+str(x.tl)+ ", Time right:"+ str(x.tr))
+
+#make an video visualisation of norman labelling the mouse video
+#this is optional as not every video result will need visualisation
+x.draw_vid()
+
+
+```
 
 ### Function details
 
 
 Though very few NORMAN functions are needed to extract a discrimination index from a video, the NORMAN system has more functions for working with NORT images and videos. In this section I will explain how to use various functions in the library, with their use-cases and code examples. Where relevant I will also include information on how/why I made the function for context. Code examples below were done in the “demo” folder of the NORMAN project repository, using the “test_79.mp4” video as the source data. The top of each code example with show the arguments of the function and their defaults when applicable. For the full code of each function see the norman_functions.py file, and for the help doc strings use the python default function help().
 
 ```python
```

### Comparing `norman_ai-0.0.5/setup.cfg` & `norman_ai-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 6f72 6d61 6e5f 6169 0d0a 7665   = norman_ai..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 350d 0a61  rsion = 0.0.5..a
+00000020: 7273 696f 6e20 3d20 302e 302e 360d 0a61  rsion = 0.0.6..a
 00000030: 7574 686f 7220 3d20 7365 7969 6a5f 700d  uthor = seyij_p.
 00000040: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000050: 7365 7969 2e6f 6f6a 4067 6d61 696c 2e63  seyi.ooj@gmail.c
 00000060: 6f6d 0d0a 6465 7363 7269 7074 696f 6e20  om..description 
 00000070: 3d20 4120 7061 636b 6167 6520 666f 7220  = A package for 
 00000080: 6175 746f 6d61 7469 6f6e 206f 6620 7468  automation of th
 00000090: 6520 6e6f 7665 6c20 6f62 6a65 6374 2072  e novel object r
```

### Comparing `norman_ai-0.0.5/src/norman_ai/data/norman_model1.h5` & `norman_ai-0.0.6/src/norman_ai/data/norman_model1.h5`

 * *Files identical despite different names*

### Comparing `norman_ai-0.0.5/src/norman_ai/norman_functions.py` & `norman_ai-0.0.6/src/norman_ai/norman_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,86 @@
         ret, frame = vid.read()
         if ret == False:
             break
         sm_frame = cv2.resize(frame, res)
         out.write(sm_frame)
     vid.release()
     out.release()
+#%%
+def draw_objects(image_or_path):
+    """
+    Use this function to draw where the objects are in your image of the experiment box.
+    
+    Parameters
+    ----------
+    source_path : TYPE
+        Path to image showing objects.
+        Or image array of images showing objects.
+
+    Returns
+    -------
+    blank_img : TYPE
+        Image to be sent to find_objects function for object identification.
+
+    """
+    drawing = False # true if mouse is pressed
+    
+    # define mouse callback function to draw circle
+    def draw_curve(event, x, y, flags, param):
+        global pt1_x,pt1_y,drawing
+    
+        if event==cv2.EVENT_LBUTTONDOWN:
+            drawing=True
+            pt1_x,pt1_y=x,y
+    
+        elif event==cv2.EVENT_MOUSEMOVE:
+            if drawing==True:
+                cv2.line(source_img,(pt1_x,pt1_y),(x,y),color=(255,255,255),thickness=2)
+                cv2.line(blank_img,(pt1_x,pt1_y),(x,y),color=(255,255,255),thickness=2)
+                pt1_x,pt1_y=x,y
+        elif event==cv2.EVENT_LBUTTONUP:
+            drawing=False
+            cv2.line(source_img,(pt1_x,pt1_y),(x,y),color=(255,255,255),thickness=2)
+            cv2.line(blank_img,(pt1_x,pt1_y),(x,y),color=(255,255,255),thickness=2)
+    
+    
+    if type(image_or_path) == str:
+        source_img = cv2.imread(image_or_path)
+        
+    #if loaded image array just use that
+    else:
+        source_img = image_or_path
+    
+    
+    # Create a black image the same size as input image
+    blank_img = np.zeros((source_img.shape[0],source_img.shape[1],3), np.uint8)
+    
+    # Create a window and bind the function to window
+    cv2.namedWindow("Draw objects Window")
+    
+    # Connect the mouse button to our callback function
+    cv2.setMouseCallback("Draw objects Window", draw_curve)
+    
+    # display the window
+    while True:
+       cv2.imshow("Draw objects Window", source_img)
+       #if r key is pressed, reset
+       if cv2.waitKey(1) == ord("r"):
+           if type(image_or_path) == str:
+               source_img = cv2.imread(image_or_path)
+           #if loaded image array just use that
+           else:
+               source_img = image_or_path
+           blank_img = np.zeros((source_img.shape[0],source_img.shape[1],3), np.uint8)
+    #if escape key is pressed
+       if cv2.waitKey(1) == 27:
+          break
+    cv2.destroyAllWindows()
+    return blank_img
+
 
 #%% add image, threshold and find contours. use TREE for hierarchy
 def find_objects(image_or_path, show=False, img_out=False, im_write=False):
     """ Finds object locations images where no animal is present.
     
     Arguments:
         image_or_path -- input image variable or path to input image file
@@ -938,21 +1010,25 @@
         fps -- fps of input video
     
     Methods:
         draw_vid -- makes a video with an overlay of norman predictions
     
     """
     #the class takes in a video and the associated deeplabcut pose file for it
-    def __init__(self, video, pose_file, no_loc, model_path="normal"):
+    def __init__(self, video, pose_file, no_loc, draw_obj=False, model_path="normal"):
         #have the name of the video as a string
         self.video_name = video
         #the median image is a frame from the video without the mouse 
         self.median_img = median_filt_video(video)
         # object locations are the output of the find objects funtion
-        self.object_locs, self.fo_img = find_objects(self.median_img, img_out = True)
+        if draw_obj=True:
+            self.object_locs, self.fo_img = find_objects(self.median_img, img_out = True)
+        if draw_obj=False:
+            x = draw_objects(self.median_img)
+            self.object_locs, self.fo_img = find_objects(x, img_out = True)
         # use relative position
         self.relative_pos = rel_pos(pose_file, self.object_locs)
         #get labels produced by the classification by norman
         self.labels = label_vid(self.relative_pos, model_path)  
         #get the discrimination index, seconds spent with left or right, and fps
         self.di, self.tl, self.tr, self.fps = calc_di(video, self.labels, no_loc)
```

### Comparing `norman_ai-0.0.5/src/norman_ai.egg-info/PKG-INFO` & `norman_ai-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: norman-ai
-Version: 0.0.5
-Summary: A package for automation of the novel object recognition test.
-Home-page: https://github.com/Seyij/norman
-Author: seyij_p
-Author-email: seyi.ooj@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # The NORMAN System
 
 The Novel Object Recognition Mouse Analysis Network (NORMAN) system is a package for automation of the novel object recognition behavioural assay in neuroscience studies.
 
 PyPi link: https://pypi.org/project/norman-ai/
 
 This is part of work that will be presented as a poster at the [BNA Festival 2021](https://meetings.bna.org.uk/bna2021/) which runs from the 12-15th of April. It was developed as part of an MSci degree at the University of Dundee. The package and repository will be updated with video outlines and other details shortly, in the run up to the BNA festival.
@@ -108,15 +94,15 @@
 import norman_ai.norman_functions as nf
 nf.run_gui()
 #a user interface should appear
 ```
 
 ### Video to DI walkthrough
 
-This section will take you through the basic steps required to get a DI from a video and to visualise NORMAN'S labelling, both using the provided user interface and with code. Make sure you are in the "norman_dlc" environment before proceeding.
+This section will take you through the basic steps required to get a DI from a video and to visualise NORMAN'S labelling, both using the provided user interface and with code. Make sure you are in the conda environment with norman and deeplabcut installed before proceeding. Please note that the user interface is primarily for demonstration purposes. To fully take advantage of NORMAN and process in batches for your own application, the code method is what you should use.
 
 ##### __*User interface method*__
 
 This uses the video file, a premade deeplabcut tracking file and an option norman model file in the demo folder of the project repository.
 
 ```bash
 #open the ipython program
@@ -175,26 +161,47 @@
 
 ```python
 
 #get path to pose document
 poses = r"test_79DLC_resnet_50_nort_demoSep26shuffle1_50000_filtered.csv"
 
 #create norkid python object
-# stating the novel object is the left object in the experiment
+# stating the novel object is the left object in the experiment, if the right object is novel state "right"
 x = nf.norkid(video, poses, "left")
 
 #show the discrimination index, the time spent with left object, time spent with right object
 print("DI:"+str(x.di)+", Time left:"+str(x.tl)+ ", Time right:"+ str(x.tr))
 
 #make an video visualisation of norman labelling the mouse video
 #this is optional as not every video result will need visualisation
 x.draw_vid()
 
 ```
-If you have trouble with this demo, please see the function details, which contain code examples and guidance on other functions in the NORMAN package. When attempting this with your own data, the most common error is related to the find_objects() function, as not all NORT mouse chambers are compatible with the object detection algorithm. If this is the case with your data I am happy to work on variant object detectors.
+If you have trouble with this demo, please see the function details, which contain code examples and guidance on other functions in the NORMAN package. 
+
+When using NORMAN with your own data, the most common problem is related to the find_objects() function, as not all NORT mouse chambers are compatible with the object detection algorithm. If this is the case you can use a conditional argument to draw the location of the experimental objects, and all the other parts of analysis will still be done automatically.
+![draw](https://github.com/Seyij/norman/blob/master/media/draw_objects.png)
+
+Hold the "r" key to reset the drawing and hold the escape key to exit once the drawing is complete.
+
+```python
+#if you wish to mark object locations yourself use draw_objects as true
+#hold r to reset the drawing
+#press escape to exit the window once the drawing is complete
+x = nf.norkid(video, poses, "left", draw_objects=True)
+
+#show the discrimination index, the time spent with left object, time spent with right object
+print("DI:"+str(x.di)+", Time left:"+str(x.tl)+ ", Time right:"+ str(x.tr))
+
+#make an video visualisation of norman labelling the mouse video
+#this is optional as not every video result will need visualisation
+x.draw_vid()
+
+
+```
 
 ### Function details
 
 
 Though very few NORMAN functions are needed to extract a discrimination index from a video, the NORMAN system has more functions for working with NORT images and videos. In this section I will explain how to use various functions in the library, with their use-cases and code examples. Where relevant I will also include information on how/why I made the function for context. Code examples below were done in the “demo” folder of the NORMAN project repository, using the “test_79.mp4” video as the source data. The top of each code example with show the arguments of the function and their defaults when applicable. For the full code of each function see the norman_functions.py file, and for the help doc strings use the python default function help().
 
 ```python
```

