# Comparing `tmp/langful-0.25-py2.py3-none-any.whl.zip` & `tmp/langful-0.26-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 7937 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     1549 b- defN 23-May-10 08:22 langful/__init__.py
 -rw-rw-rw-  2.0 fat      611 b- defN 23-Apr-26 14:01 langful/define.py
--rw-rw-rw-  2.0 fat     2453 b- defN 23-May-10 08:11 langful/function.py
+-rw-rw-rw-  2.0 fat     2461 b- defN 23-May-23 04:47 langful/function.py
 -rw-rw-rw-  2.0 fat    13089 b- defN 23-May-10 08:07 langful/lang.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-May-10 08:29 langful-0.25.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2641 b- defN 23-May-10 08:29 langful-0.25.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-May-10 08:29 langful-0.25.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-10 08:29 langful-0.25.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      679 b- defN 23-May-10 08:29 langful-0.25.dist-info/RECORD
-9 files, 22204 bytes uncompressed, 6783 bytes compressed:  69.5%
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-May-23 04:50 langful-0.26.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2641 b- defN 23-May-23 04:50 langful-0.26.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-May-23 04:50 langful-0.26.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-23 04:50 langful-0.26.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      679 b- defN 23-May-23 04:50 langful-0.26.dist-info/RECORD
+9 files, 22212 bytes uncompressed, 6783 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: langful/function.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.25.dist-info/LICENSE
+Filename: langful-0.26.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.25.dist-info/METADATA
+Filename: langful-0.26.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.25.dist-info/WHEEL
+Filename: langful-0.26.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.25.dist-info/top_level.txt
+Filename: langful-0.26.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.25.dist-info/RECORD
+Filename: langful-0.26.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/function.py

```diff
@@ -66,15 +66,15 @@
 
     把lang文件转换为json文件
     """
     ret={}
     lang = lang.split("\n")
     for i in lang :
         I=i.split("#")[0]#移除注释
-        I=I.split("=")
+        I=I.split( "=" , 1 )
         if len(I) == 2 :
             key , value = I
             if value[0] == " " :
                 value = value[1:]
             if key[-1] == " " :
                 key = key[:-1]
             ret[key]=value
@@ -91,8 +91,8 @@
     """
     ret = ""
     for key , value in dict.items() :
         if isinstance( value , str ) :
             ret += f"{key} = {value}\n"
         else :
             raise TypeError( "" )
-    return ret
+    return ret
```

## Comparing `langful-0.25.dist-info/LICENSE` & `langful-0.26.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.25.dist-info/METADATA` & `langful-0.26.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.25
+Version: 0.26
 Home-page: https://github.com/cueavyqwp/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: > 3.6
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langful Version: 0.25 Home-page: https://
+Metadata-Version: 2.1 Name: langful Version: 0.26 Home-page: https://
 github.com/cueavyqwp/langful Author: cueavyqwp Author-email:
 cueavyqwp@outlook.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: > 3.6 Description-Content-Type: text/
 markdown License-File: LICENSE # langful
    [PyPI_version] [Python_version] [license] [Github_stars] [Github_issues]
 # install Use `pip` to install `pip install langful` or `pip3 install langful`
```

