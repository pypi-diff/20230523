# Comparing `tmp/tailraiders-0.0.3.tar.gz` & `tmp/tailraiders-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tailraiders-0.0.3.tar", last modified: Fri May 19 18:33:11 2023, max compression
+gzip compressed data, was "tailraiders-0.0.4.tar", last modified: Tue May 23 09:37:35 2023, max compression
```

## Comparing `tailraiders-0.0.3.tar` & `tailraiders-0.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.429534 tailraiders-0.0.3/
--rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 tailraiders-0.0.3/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      695 2023-05-19 18:33:11.429534 tailraiders-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      370 2023-05-19 18:28:04.000000 tailraiders-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 18:33:11.430805 tailraiders-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      646 2023-05-18 20:40:04.000000 tailraiders-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.366356 tailraiders-0.0.3/tailraiders/
--rw-rw-rw-   0        0        0      841 2023-05-19 18:27:22.000000 tailraiders-0.0.3/tailraiders/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.404021 tailraiders-0.0.3/tailraiders/boaboa/
--rw-rw-rw-   0        0        0       44 2023-05-19 18:26:14.000000 tailraiders-0.0.3/tailraiders/boaboa/__init__.py
--rw-rw-rw-   0        0        0     1149 2023-05-17 11:17:42.000000 tailraiders-0.0.3/tailraiders/boaboa/doc.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.411009 tailraiders-0.0.3/tailraiders/bugtrapper/
--rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 tailraiders-0.0.3/tailraiders/bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.422440 tailraiders-0.0.3/tailraiders/gajalaka/
--rw-rw-rw-   0        0        0      163 2023-05-19 18:25:51.000000 tailraiders-0.0.3/tailraiders/gajalaka/__init__.py
--rw-rw-rw-   0        0        0     2644 2023-05-19 17:19:07.000000 tailraiders-0.0.3/tailraiders/gajalaka/nan.py
--rw-rw-rw-   0        0        0     2337 2023-05-16 21:59:03.000000 tailraiders-0.0.3/tailraiders/gajalaka/plots.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.424439 tailraiders-0.0.3/tailraiders/plunderer/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 tailraiders-0.0.3/tailraiders/plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.425439 tailraiders-0.0.3/tailraiders/protector/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 tailraiders-0.0.3/tailraiders/protector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.426883 tailraiders-0.0.3/tailraiders/trouper/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 tailraiders-0.0.3/tailraiders/trouper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-19 18:33:11.399680 tailraiders-0.0.3/tailraiders.egg-info/
--rw-rw-rw-   0        0        0      695 2023-05-19 18:33:10.000000 tailraiders-0.0.3/tailraiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2023-05-19 18:33:11.000000 tailraiders-0.0.3/tailraiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 18:33:10.000000 tailraiders-0.0.3/tailraiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-19 18:33:10.000000 tailraiders-0.0.3/tailraiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-19 18:33:10.000000 tailraiders-0.0.3/tailraiders.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 09:37:35.638664 tailraiders-0.0.4/
+-rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 tailraiders-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 tailraiders-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1012 2023-05-23 09:37:35.637411 tailraiders-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      687 2023-05-23 09:33:42.000000 tailraiders-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:37:35.638664 tailraiders-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      646 2023-05-22 11:23:45.000000 tailraiders-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:37:35.509834 tailraiders-0.0.4/tailraiders/
+-rw-rw-rw-   0        0        0      919 2023-05-23 09:32:42.000000 tailraiders-0.0.4/tailraiders/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:37:35.603472 tailraiders-0.0.4/tailraiders/boaboa/
+-rw-rw-rw-   0        0        0      141 2023-05-23 09:34:49.000000 tailraiders-0.0.4/tailraiders/boaboa/__init__.py
+-rw-rw-rw-   0        0        0     2521 2023-05-23 09:27:58.000000 tailraiders-0.0.4/tailraiders/boaboa/doc.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:37:35.605500 tailraiders-0.0.4/tailraiders/bugtrapper/
+-rw-rw-rw-   0        0        0      110 2023-05-23 09:36:01.000000 tailraiders-0.0.4/tailraiders/bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:37:35.624828 tailraiders-0.0.4/tailraiders/gajalaka/
+-rw-rw-rw-   0        0        0      132 2023-05-23 09:35:13.000000 tailraiders-0.0.4/tailraiders/gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     6178 2023-05-23 09:20:00.000000 tailraiders-0.0.4/tailraiders/gajalaka/plots.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:37:35.628165 tailraiders-0.0.4/tailraiders/plunderer/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 tailraiders-0.0.4/tailraiders/plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:37:35.632822 tailraiders-0.0.4/tailraiders/protector/
+-rw-rw-rw-   0        0        0      135 2023-05-23 09:35:05.000000 tailraiders-0.0.4/tailraiders/protector/__init__.py
+-rw-rw-rw-   0        0        0     3635 2023-05-23 09:24:23.000000 tailraiders-0.0.4/tailraiders/protector/nan.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:37:35.634914 tailraiders-0.0.4/tailraiders/trouper/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 tailraiders-0.0.4/tailraiders/trouper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:37:35.597384 tailraiders-0.0.4/tailraiders.egg-info/
+-rw-rw-rw-   0        0        0     1012 2023-05-23 09:37:33.000000 tailraiders-0.0.4/tailraiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2023-05-23 09:37:35.000000 tailraiders-0.0.4/tailraiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:37:33.000000 tailraiders-0.0.4/tailraiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-23 09:37:34.000000 tailraiders-0.0.4/tailraiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-23 09:37:34.000000 tailraiders-0.0.4/tailraiders.egg-info/top_level.txt
```

### Comparing `tailraiders-0.0.3/LICENSE` & `tailraiders-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tailraiders-0.0.3/setup.py` & `tailraiders-0.0.4/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 setup(
     author = 'Busse Heemskerk',
     description = 'A package for making Data Science easier, versions with 0.0.x are trials and tests',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     name = 'tailraiders',
-    version = '0.0.3',
+    version = '0.0.4',
     packages = find_packages(include = ['tailraiders', 'tailraiders.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
                         'seaborn>=0.9.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
     )
```

### Comparing `tailraiders-0.0.3/tailraiders/__init__.py` & `tailraiders-0.0.4/tailraiders/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,9 +16,11 @@
     #Try to import modules
     try:
         __import__(module)
     #Raise an error when it fails, telling them to install the failed module
     except ImportError:
         raise ImportError(f"The required package {module} was not found. Please install it.")
     
-#Making it so you can use from tailraiders import module as well (hopefully)
-from tailraiders import boaboa, gajalaka
+#Making it so you can, for certain parts, just import tailraiders
+from tailraiders.boaboa import docstring
+from tailraiders.gajalaka import Plots, MeltPlot
+from tailraiders.protector import Nan
```

### Comparing `tailraiders-0.0.3/tailraiders/gajalaka/nan.py` & `tailraiders-0.0.4/tailraiders/protector/nan.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,17 +25,22 @@
 
         Returns:
         ----------------
         None :
             It makes it so that self.df is now edited to no longer has the dropped columns
         """
 
-        self.nan_df = self.check[self.check['perc nan'] > th]
+        #making a temp df to see what columns go over the threshold
+        self.nan_df = self.dfnan[self.dfnan['perc nan'] > th]
+        
+        #making a list from the index to use for drop
         dropcols = list(self.nan_df.index)
         print(f'The columns {dropcols} are being dropped')
+
+        #dropping the columns in the list
         self.df = self.df.drop(dropcols, axis = 1)
         self.__init__(self.df)
     
     def fill_na(self, col, group, stat = 'mean'):
         """
         Fills dataframe columns based on a given group and method
 
@@ -44,25 +49,26 @@
         self :
             The given name of the class
         
         col : str
             The column name that will be filled
         
         group : str
-            Column name that will be used to group
+            Column name that will be used to group by
         
         stat : str (default = 'mean')
             The stat on how people will be grouped
             
         Returns:
         ----------------
         None :
             It makes it so that self.df is now edited to no longer have the dropped columns
         """
 
+        #using fillna to fill the given column with given groupby column using the given method
         self.df[col] = self.df[col].fillna(self.df.groupby(group)[col].transform(stat))
         self.__init__(self.df)
         
     def drop_na(self, axis = 0):
         """
         Drops columns based on the given axis
 
@@ -73,12 +79,35 @@
 
         axis : int (default = 0)
             Bool value, either 0 or 1. 0 is for rows and 1 is for columns
 
         Returns:
         ----------------
         None :
-            It makes it so that self.df is now edited to no longer have the dropped columns
+            It makes it so that self.df is now edited to no longer have the dropped rows or columns
         """
 
+        #dropna to drop rows or columns, based on given axis
         self.df = self.df.dropna(axis = axis)
-        self.__init__(self.df)
+        self.__init__(self.df)
+
+    @classmethod
+    def df_from_file(cls, file_path):
+        """
+        A function to immediately convert files to be used for Nan
+
+        Parameters
+        --------------------
+        cls : 
+            The class it is in (will not be filled in when using the function)
+        
+        file_path : str
+            The file_path to the file containing the data you want to use
+
+        returns:
+        --------------------
+        cls(df) : pandas.Dataframe
+            A pandas dataframe that is immediately used for Nan.__init__
+        """
+        
+        df = pd.read_csv(file_path)
+        return cls(df)
```

### Comparing `tailraiders-0.0.3/tailraiders.egg-info/SOURCES.txt` & `tailraiders-0.0.4/tailraiders.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 tailraiders.egg-info/dependency_links.txt
 tailraiders.egg-info/requires.txt
 tailraiders.egg-info/top_level.txt
 tailraiders/boaboa/__init__.py
 tailraiders/boaboa/doc.py
 tailraiders/bugtrapper/__init__.py
 tailraiders/gajalaka/__init__.py
-tailraiders/gajalaka/nan.py
 tailraiders/gajalaka/plots.py
 tailraiders/plunderer/__init__.py
 tailraiders/protector/__init__.py
+tailraiders/protector/nan.py
 tailraiders/trouper/__init__.py
```

