# Comparing `tmp/sports2d-0.2.0.tar.gz` & `tmp/sports2d-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sports2d-0.2.0.tar", last modified: Sun May 21 00:04:39 2023, max compression
+gzip compressed data, was "sports2d-0.2.1.tar", last modified: Tue May 23 10:05:06 2023, max compression
```

## Comparing `sports2d-0.2.0.tar` & `sports2d-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:04:39.535256 sports2d-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-21 00:04:25.000000 sports2d-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-05-21 00:04:39.535256 sports2d-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12968 2023-05-21 00:04:25.000000 sports2d-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:04:39.531256 sports2d-0.2.0/Sports2D/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:04:39.531256 sports2d-0.2.0/Sports2D/Demo/
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/Demo/Config_demo.toml
--rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/Demo/demo.mp4
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/Sports2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:04:39.531256 sports2d-0.2.0/Sports2D/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/Utilities/Blazepose_runsave.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/Utilities/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/Utilities/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/Utilities/skeletons.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/Utilities/test_with_blazepose.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21766 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/compute_angles.py
--rw-r--r--   0 runner    (1001) docker     (123)    23921 2023-05-21 00:04:25.000000 sports2d-0.2.0/Sports2D/detect_pose.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-21 00:04:25.000000 sports2d-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-21 00:04:39.535256 sports2d-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-21 00:04:25.000000 sports2d-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 00:04:39.535256 sports2d-0.2.0/sports2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-05-21 00:04:39.000000 sports2d-0.2.0/sports2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-21 00:04:39.000000 sports2d-0.2.0/sports2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:04:39.000000 sports2d-0.2.0/sports2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 00:04:39.000000 sports2d-0.2.0/sports2d.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 00:04:39.000000 sports2d-0.2.0/sports2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 00:04:39.000000 sports2d-0.2.0/sports2d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:06.621564 sports2d-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-23 10:04:54.000000 sports2d-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-05-23 10:05:06.621564 sports2d-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12975 2023-05-23 10:04:54.000000 sports2d-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:06.617565 sports2d-0.2.1/Sports2D/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:06.617565 sports2d-0.2.1/Sports2D/Demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/Demo/Config_demo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)  2539508 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/Demo/demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/Sports2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:06.621564 sports2d-0.2.1/Sports2D/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/Utilities/Blazepose_runsave.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/Utilities/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4912 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/Utilities/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15305 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/Utilities/skeletons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/Utilities/test_with_blazepose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21895 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/compute_angles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24124 2023-05-23 10:04:54.000000 sports2d-0.2.1/Sports2D/detect_pose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 10:04:54.000000 sports2d-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-23 10:05:06.621564 sports2d-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-23 10:04:54.000000 sports2d-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:05:06.621564 sports2d-0.2.1/sports2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-05-23 10:05:06.000000 sports2d-0.2.1/sports2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-23 10:05:06.000000 sports2d-0.2.1/sports2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:05:06.000000 sports2d-0.2.1/sports2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:05:06.000000 sports2d-0.2.1/sports2d.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-23 10:05:06.000000 sports2d-0.2.1/sports2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 10:05:06.000000 sports2d-0.2.1/sports2d.egg-info/top_level.txt
```

### Comparing `sports2d-0.2.0/LICENSE` & `sports2d-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.0/PKG-INFO` & `sports2d-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.2.0
+Version: 0.2.1
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -48,14 +48,16 @@
 </br>
 
 **`Announcement:` \
 User-friendly Colab version released!\
 Works on any smartphone!**\
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
 
+</br>
+
 <img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
 
 `Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
 `Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
 If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.\
 `Warning:` Google Colab does not follow the European GDPR requirements regarding data privacy. [Install locally](#installation) if this matters.
```

### Comparing `sports2d-0.2.0/README.md` & `sports2d-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 </br>
 
 **`Announcement:` \
 User-friendly Colab version released!\
 Works on any smartphone!**\
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
 
+</br>
+
 <img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
 
 `Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
 `Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
 If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.\
 `Warning:` Google Colab does not follow the European GDPR requirements regarding data privacy. [Install locally](#installation) if this matters.
```

### Comparing `sports2d-0.2.0/Sports2D/Demo/Config_demo.toml` & `sports2d-0.2.1/Sports2D/Demo/Config_demo.toml`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.0/Sports2D/Demo/demo.mp4` & `sports2d-0.2.1/Sports2D/Demo/demo.mp4`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.0/Sports2D/Sports2D.py` & `sports2d-0.2.1/Sports2D/Sports2D.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
     if result_dir == '': result_dir = os.getcwd()
     
     video = cv2.VideoCapture(str(video_dir / video_file))
     frame_rate = video.get(cv2.CAP_PROP_FPS)
     try:
         1/frame_rate
     except ZeroDivisionError:
-        print(f'Frame rate of {str(video_dir / video_file)} could not be retrieved: check that it exists at the correct path')
+        print('Frame rate could not be retrieved: check that your video exists at the correct path')
         raise
     video.release()
 
     return video_dir, video_file, result_dir, frame_rate
 
 
 def detect_pose(config='Config_demo.toml'):
```

### Comparing `sports2d-0.2.0/Sports2D/Utilities/Blazepose_runsave.py` & `sports2d-0.2.1/Sports2D/Utilities/Blazepose_runsave.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 __version__ = "0.1"
 __maintainer__ = "David Pagnon"
 __email__ = "contact@david-pagnon.com"
 __status__ = "Development"
 
 
 ## FUNCTIONS
-def save_to_csv_or_h5(kpt_list, output_folder, video_name, to_csv, to_h5):
+def save_to_csv_or_h5(kpt_list, fps, output_folder, video_name, to_csv, to_h5):
     '''
     Saves blazepose keypoint coordinates to csv or h5 file, 
     in the DeepLabCut format.
 
     INPUTS:
     - kpt_list: List of lists of keypoints X and Y coordinates and likelihood, for each frame
     - output_folder: Folder where to save the csv or h5 file
@@ -62,23 +62,24 @@
     - to_h5: Boolean, whether to save to h5
 
     OUTPUTS:
     - Creation of csv or h5 file in output_folder
     '''
     
     # Prepare dataframe file
-    scorer = ['DavidPagnon']*len(mp_pose.PoseLandmark)*3
-    individuals = ['person']*len(mp_pose.PoseLandmark)*3
+    scorer = ['DavidPagnon']*(len(mp_pose.PoseLandmark)*3+1)
+    individuals = ['person']*(len(mp_pose.PoseLandmark)*3+1)
     bodyparts = [[p]*3 for p in ['Nose', 'LEyeInner', 'LEye', 'LEyeOuter', 'REyeInner', 'REye', 'REyeOuter', 'LEar', 'REar', 'LMouth', 'RMouth', 'LShoulder', 'RShoulder', 'LElbow', 'RElbow', 'LWrist', 'RWrist', 'LPinky', 'RPinky', 'LIndex', 'RIndex', 'LThumb', 'RThumb', 'LHip', 'RHip', 'LKnee', 'RKnee', 'LAnkle', 'RAnkle', 'LHeel', 'RHeel', 'LBigToe', 'RBigToe']]
-    bodyparts = [item for sublist in bodyparts for item in sublist]
-    coords = ['x', 'y', 'likelihood']*len(mp_pose.PoseLandmark)
-
+    bodyparts = ['Times'] + [item for sublist in bodyparts for item in sublist]
+    coords = ['seconds'] + ['x', 'y', 'likelihood']*len(mp_pose.PoseLandmark)
     tuples = list(zip(scorer, individuals, bodyparts, coords))
     index_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'bodyparts', 'coords'])
-    df = pd.DataFrame(np.array(kpt_list).T, index=index_csv).T
+    
+    time = np.expand_dims( np.arange(0,len(kpt_list)/fps, 1/fps), axis=0 )
+    df = pd.DataFrame(np.concatenate(( time, np.array(kpt_list).T)), index=index_csv).T
 
     if to_csv:
         csv_file = os.path.join(output_folder, video_name+'_BLAZEPOSE_points.csv')
         logging.info(f'Saving csv file in {csv_file}.')
         df.to_csv(csv_file, sep=',', index=True, lineterminator='\n')
 
     if to_h5:
@@ -225,15 +226,15 @@
         cap.release()
         if save_video:
             writer.release()    
         cv2.destroyAllWindows()
 
     # Save coordinates
     if to_csv or to_h5:
-        save_to_csv_or_h5(kpt_list, output_folder, video_name, to_csv, to_h5)
+        save_to_csv_or_h5(kpt_list, fps, output_folder, video_name, to_csv, to_h5)
    
     if to_json:
         save_to_json(kpt_list, output_folder, video_name)
     
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
```

### Comparing `sports2d-0.2.0/Sports2D/Utilities/common.py` & `sports2d-0.2.1/Sports2D/Utilities/common.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.0/Sports2D/Utilities/filter.py` & `sports2d-0.2.1/Sports2D/Utilities/filter.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.0/Sports2D/Utilities/skeletons.py` & `sports2d-0.2.1/Sports2D/Utilities/skeletons.py`

 * *Files identical despite different names*

### Comparing `sports2d-0.2.0/Sports2D/compute_angles.py` & `sports2d-0.2.1/Sports2D/compute_angles.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,23 +119,25 @@
     INPUTS:
     - df_list: list of dataframes of angles
 
     OUTPUT:
     - matplotlib window with tabbed figures for each angle
     '''
     
-    angle_names = df_list[0].columns.get_level_values(2)
+    angle_names = df_list[0].iloc[:,1:].columns.get_level_values(2)
+    time = df_list[0].iloc[:,0]
     
     pw = common.plotWindow()
     for id, angle in enumerate(angle_names): # angles
         f = plt.figure()
         
         plt.plot()
-        [plt.plot(df_list[0].index, df.iloc[:,id], label=['unfiltered' if i==0 else 'filtered' if i==1 else ''][0]) for i,df in enumerate(df_list)]
-        plt.ylabel(angle) # nom angle
+        [plt.plot(time, df.iloc[:,id+1], label=['unfiltered' if i==0 else 'filtered' if i==1 else ''][0]) for i,df in enumerate(df_list)]
+        plt.xlabel('Time (seconds)')
+        plt.ylabel(angle)
         plt.legend()
 
         pw.addPlot(angle, f)
     
     pw.show()
     
     
@@ -183,15 +185,15 @@
     OUTPUT:
     - df_points: dataframe of pose detection with flipped X coordinates
     '''
     
     righ_orientation = df_points.iloc[:,df_points.columns.get_level_values(2)=='RBigToe'].iloc[:,0] - df_points.iloc[:,df_points.columns.get_level_values(2)=='RHeel'].iloc[:,0]
     left_orientation = df_points.iloc[:,df_points.columns.get_level_values(2)=='LBigToe'].iloc[:,0] - df_points.iloc[:,df_points.columns.get_level_values(2)=='LHeel'].iloc[:,0]
     orientation = righ_orientation + left_orientation
-    df_points.iloc[:,1::3] = df_points.iloc[:,1::3] * np.where(orientation>=0, 1, -1).reshape(-1,1)
+    df_points.iloc[:,2::3] = df_points.iloc[:,2::3] * np.where(orientation>=0, 1, -1).reshape(-1,1)
     
     return df_points
             
 
 def joint_angles_series_from_points(df_points, angle_params):
     '''
     Obtain joint angle series from point series.
@@ -213,15 +215,14 @@
     points_list = [k.values.T for k in keypt_series]
     ang_series = points2D_to_angles(points_list)
     ang_series += angle_params[2]
     ang_series *= angle_params[3]
     ang_series = np.where(ang_series>180,ang_series-360,ang_series)
     ang_series = np.where((ang_series==0) | (ang_series==90) | (ang_series==180), +0, ang_series)
 
-    
     return ang_series
 
 
 def segment_angles_series_from_points(df_points, angle_params, segment):
     '''
     Obtain segment angle series w/r horizontal from point series.
     For trunk segment: mean of the angles between RHip-RShoulder and LHip-LShoulder
@@ -383,25 +384,26 @@
     csv_paths = list(result_dir.glob(f'*{video_file.stem}_{pose_model}_*points*.csv'))
     logging.info(f'{len(csv_paths)} persons found.')
 
     # Compute angles
     df_angles_list = []
     for i, c in enumerate(csv_paths):
         # Prepare angle csv header
-        scorer = ['DavidPagnon']*angle_nb
-        individuals = [f'person{i}']*angle_nb
-        angs = joint_angles + segment_angles
-        coords = [joint_angle_dict.get(j)[1] for j in joint_angles] + [segment_angle_dict.get(s)[1] for s in segment_angles]
+        scorer = ['DavidPagnon']*(angle_nb+1)
+        individuals = [f'person{i}']*(angle_nb+1)
+        angs = ['Time'] + joint_angles + segment_angles
+        coords = ['seconds'] + [joint_angle_dict.get(j)[1] for j in joint_angles] + [segment_angle_dict.get(s)[1] for s in segment_angles]
         tuples = list(zip(scorer, individuals, angs, coords))
-        index_angs_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'joints', 'angles'])    
+        index_angs_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'angs', 'coords'])    
 
         # Compute angles for each person, for each angle, with each required keypoint position
         logging.info(f'Person {i}: Computing 2D joint and segment angles.')
         with open(c) as c_f:
             df_points = pd.read_csv(c_f, header=[0,1,2,3])
+            time = [np.array(df_points.iloc[:,1])]
             
             # Flip along x when feet oriented to the left
             df_points = flip_left_right_direction(df_points)
             
             # Joint angles
             joint_angle_series = []
             for j in joint_angles: 
@@ -412,15 +414,15 @@
             # Segment angles
             segment_angle_series = []
             for s in segment_angles:
                 angle_params = segment_angle_dict.get(s)
                 s_ang_series = segment_angles_series_from_points(df_points, angle_params, s)
                 segment_angle_series += [s_ang_series]
             
-            angle_series = joint_angle_series + segment_angle_series
+            angle_series = time + joint_angle_series + segment_angle_series
             df_angles = []
             df_angles += [pd.DataFrame(angle_series, index=index_angs_csv).T]
             
             # Filter
             if filter_options[0]:
                 filter_type = filter_options[1]
                 if filter_type == 'butterworth':
@@ -460,15 +462,15 @@
             cap = [cv2.VideoCapture(str(video_pose)) if Path.exists(video_pose) else cv2.VideoCapture(str(video_base))][0]
             fps = cap.get(cv2.CAP_PROP_FPS)
             W, H = cap.get(cv2.CAP_PROP_FRAME_WIDTH), cap.get(cv2.CAP_PROP_FRAME_HEIGHT)
             fourcc = cv2.VideoWriter_fourcc(*'mp4v')
             writer = cv2.VideoWriter(str(video_pose2), fourcc, fps, (int(W), int(H)))
         
         # Preferentially from pose image files
-        frames_img = sorted(list(img_pose.glob('*.png')))
+        frames_img = list(img_pose.glob('*'))
         if len(frames_img)>0:
             for frame_nb in range(df_angles_list[0].shape[0]):
                 df_angles_list_frame = [df_angles_list[n].iloc[frame_nb,:] for n in range(len(df_angles_list))]
                 frame = cv2.imread(str(frames_img[frame_nb]))
                 frame = overlay_angles(frame, df_angles_list_frame)
                 if show_angles_img:
                     cv2.imwrite(str(frames_img[frame_nb]), frame)
@@ -496,8 +498,8 @@
         cap.release()
         writer.release()
         if show_angles_vid:
             if Path.exists(video_pose): os.remove(video_pose)
             os.rename(video_pose2,video_pose)
             if Path.exists(video_pose2): os.remove(video_pose2)
 
-    logging.info(f'Done.')
+    logging.info(f'Done.')
```

### Comparing `sports2d-0.2.0/Sports2D/detect_pose.py` & `sports2d-0.2.1/Sports2D/detect_pose.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,22 +87,22 @@
     keypoints_names = df_list[0].columns.get_level_values(2)[1::3]
     
     pw = common.plotWindow()
     for id, keypoint in enumerate(keypoints_names):
         f = plt.figure()
         
         axX = plt.subplot(211)
-        [plt.plot(df_list[0].index, df.iloc[:,id*3], label=['unfiltered' if i==0 else 'filtered' if i==1 else ''][0]) for i,df in enumerate(df_list)]
+        [plt.plot(df.iloc[:,0], df.iloc[:,id*3+1], label=['unfiltered' if i==0 else 'filtered' if i==1 else ''][0]) for i,df in enumerate(df_list)]
         plt.setp(axX.get_xticklabels(), visible=False)
         axX.set_ylabel(keypoint+' X')
         plt.legend()
 
         axY = plt.subplot(212)
-        [plt.plot(df_list[0].index, df.iloc[:,id*3+1]) for df in df_list]
-        plt.setp(axY.get_xticklabels(), visible=False)
+        [plt.plot(df.iloc[:,0], df.iloc[:,id*3+2]) for df in df_list]
+        axY.set_xlabel('Time (seconds)')
         axY.set_ylabel(keypoint+' Y')
 
         pw.addPlot(keypoint, f)
     
     pw.show()
     
 
@@ -259,15 +259,15 @@
     personsIDs_sorted = np.array(personsIDs_comb)[index_best_comb][:,1]
     # rearrange persons
     keypt = np.array(keypt)[personsIDs_sorted]
     
     return keypt
 
 
-def json_to_csv(json_path, pose_model, interp_gap_smaller_than, filter_options, show_plots):
+def json_to_csv(json_path, frame_rate, pose_model, interp_gap_smaller_than, filter_options, show_plots):
     '''
     Converts frame-by-frame json coordinate files 
     to one csv files per detected person
 
     INPUTS:
     - json_path: directory path of json files
     - pose_model: string, to get tree from skeletons.py
@@ -284,15 +284,15 @@
     keypoints_ids = [node.id for _, _, node in RenderTree(model) if node.id!=None]
     keypoints_names = [node.name for _, _, node in RenderTree(model) if node.id!=None]
     keypoints_names_rearranged = [y for x,y in sorted(zip(keypoints_ids,keypoints_names))]
     keypoints_nb = len(keypoints_ids)
 
     # Retrieve coordinates
     logging.info('Sorting people across frames.')
-    json_fnames = sorted(list(json_path.glob('*.json')))
+    json_fnames = list(json_path.glob('*.json'))
     nb_persons_to_detect = max([len(json.load(open(json_fname))['people']) for json_fname in json_fnames])
     Coords = [np.array([]).reshape(0,keypoints_nb*3)] * nb_persons_to_detect
     for json_fname in json_fnames:    # for each frame
         with open(json_fname) as json_f:
             json_file = json.load(json_f)
             keypt = []
             # Retrieve coords for this frame 
@@ -312,26 +312,30 @@
                 Coords[i] = np.vstack([Coords[i], keypt[i].reshape(-1)])
             keyptpre = keypt
     logging.info(f'{nb_persons_to_detect} persons found.')
     
     # Inject coordinates in dataframes and save
     for i in range(nb_persons_to_detect): 
         # Prepare csv header
-        scorer = ['DavidPagnon']*keypoints_nb*3
-        individuals = [f'person{i}']*keypoints_nb*3
+        scorer = ['DavidPagnon']*(keypoints_nb*3+1)
+        individuals = [f'person{i}']*(keypoints_nb*3+1)
         bodyparts = [[p]*3 for p in keypoints_names_rearranged]
-        bodyparts = [item for sublist in bodyparts for item in sublist]
-        coords = ['x', 'y', 'likelihood']*keypoints_nb
+        bodyparts = ['Time']+[item for sublist in bodyparts for item in sublist]
+        coords = ['seconds']+['x', 'y', 'likelihood']*keypoints_nb
         tuples = list(zip(scorer, individuals, bodyparts, coords))
         index_csv = pd.MultiIndex.from_tuples(tuples, names=['scorer', 'individuals', 'bodyparts', 'coords'])
-    
+
+        # Create dataframe
+        df_list=[]
+        time = np.expand_dims( np.arange(0,len(Coords[i])/frame_rate, 1/frame_rate), axis=0 )
+        time_coords = np.concatenate(( time, Coords[i].T ))
+        df_list += [pd.DataFrame(time_coords, index=index_csv).T]
+
         # Interpolate
         logging.info(f'Person {i}: Interpolating missing sequences if they are smaller than {interp_gap_smaller_than} frames.')
-        df_list=[]
-        df_list += [pd.DataFrame(Coords[i].T, index=index_csv).T]
         df_list[0] = df_list[0].apply(common.interpolate_zeros_nans, axis=0, args = [interp_gap_smaller_than, 'linear'])
         
         # Filter
         if filter_options[0]:
             filter_type = filter_options[1]
             if filter_type == 'butterworth':
                 args = f'Butterworth filter, {filter_options[2]}th order, {filter_options[3]} Hz.'
@@ -479,17 +483,17 @@
         img_pose_path = video_result_path.parent / (video_result_path.stem + '_' + pose_model + '_img')
         img_pose_path.mkdir(parents=True, exist_ok=True)  
         
     f = 0
     while(cap.isOpened()):
         ret, frame = cap.read()
         if ret == True:
-            X = [np.array(coord.iloc[f,1::3]) for coord in coords]
+            X = [np.array(coord.iloc[f,2::3]) for coord in coords]
             X = [np.where(x==0., np.nan, x) for x in X]
-            Y = [np.array(coord.iloc[f,2::3]) for coord in coords]
+            Y = [np.array(coord.iloc[f,3::3]) for coord in coords]
             Y = [np.where(y==0., np.nan, y) for y in Y]
 
             # Draw bounding box
             frame = draw_bounding_box(X, Y, frame)
 
             # Draw keypoints and skeleton
             frame = draw_keypts_skel(X, Y, frame, pose_model)
@@ -580,15 +584,15 @@
             elif platform == "darwin":
                 run_openpose_mac(video_path, json_path, pose_model)
             elif platform == "linux" or platform=="linux2":
                 run_openpose_linux(video_path, json_path, pose_model)
             os.chdir(root_dir)
         
     # Sort people and save to csv, optionally display plot
-        json_to_csv(json_path, pose_model, interp_gap_smaller_than, filter_options, show_plots)
+        json_to_csv(json_path, frame_rate, pose_model, interp_gap_smaller_than, filter_options, show_plots)
         
     # Save images and files after reindentification
         if save_img and save_vid:
             logging.info(f'Saving images and video in {result_dir}.')
         if save_img and not save_vid:
             logging.info(f'Saving images in {result_dir}.')
         if not save_img and save_vid:
```

### Comparing `sports2d-0.2.0/setup.cfg` & `sports2d-0.2.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sports2d
-version = 0.2.0
+version = 0.2.1
 author = David Pagnon
 author_email = contact@david-pagnon.com
 description = Detect pose and compute 2D joint angles from a video.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/davidpagnon/Sports2D
 keywords = markerless, kinematics, OpenPose, BlazePose, joint angles, 2D, biomechanics, sports, sports-analytics
```

### Comparing `sports2d-0.2.0/sports2d.egg-info/PKG-INFO` & `sports2d-0.2.1/sports2d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sports2d
-Version: 0.2.0
+Version: 0.2.1
 Summary: Detect pose and compute 2D joint angles from a video.
 Home-page: https://github.com/davidpagnon/Sports2D
 Author: David Pagnon
 Author-email: contact@david-pagnon.com
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/davidpagnon/Sports2D/issues
 Keywords: markerless,kinematics,OpenPose,BlazePose,joint angles,2D,biomechanics,sports,sports-analytics
@@ -48,14 +48,16 @@
 </br>
 
 **`Announcement:` \
 User-friendly Colab version released!\
 Works on any smartphone!**\
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://bit.ly/Sports2D_Colab)
 
+</br>
+
 <img src='Content/demo_gif.gif' title='Demonstration of Sports2D with OpenPose.'  width="760">
 
 `Warning:` Angle estimation is only as good as the pose estimation algorithm, i.e., it is not perfect.\
 `Warning:` Results are acceptable only if the persons move in the 2D plane, from right to left or from left to right.\
 If you need research-grade markerless joint kinematics, consider using several cameras, and constraining angles to a biomechanically accurate model. See [Pose2Sim](https://github.com/perfanalytics/pose2sim) for example.\
 `Warning:` Google Colab does not follow the European GDPR requirements regarding data privacy. [Install locally](#installation) if this matters.
```

### Comparing `sports2d-0.2.0/sports2d.egg-info/SOURCES.txt` & `sports2d-0.2.1/sports2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

