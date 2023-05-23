# Comparing `tmp/HawaData-0.5.0.tar.gz` & `tmp/HawaData-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.5.0.tar", last modified: Tue May 23 08:32:27 2023, max compression
+gzip compressed data, was "HawaData-0.5.1.tar", last modified: Tue May 23 08:48:32 2023, max compression
```

## Comparing `HawaData-0.5.0.tar` & `HawaData-0.5.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.695590 HawaData-0.5.0/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.678775 HawaData-0.5.0/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2334 2023-05-23 08:32:27.000000 HawaData-0.5.0/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      521 2023-05-23 08:32:27.000000 HawaData-0.5.0/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-23 08:32:27.000000 HawaData-0.5.0/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-23 08:32:27.000000 HawaData-0.5.0/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2334 2023-05-23 08:32:27.695157 HawaData-0.5.0/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.0/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.679340 HawaData-0.5.0/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.0/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.682910 HawaData-0.5.0/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.0/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.0/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.0/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.0/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.686054 HawaData-0.5.0/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.0/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     9282 2023-05-23 07:49:48.000000 HawaData-0.5.0/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.0/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.0/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.0/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.690276 HawaData-0.5.0/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.0/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.0/hawa/data/city.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.0/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     1995 2023-05-23 07:53:45.000000 HawaData-0.5.0/hawa/data/klass.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.0/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.692975 HawaData-0.5.0/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.0/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    23638 2023-05-22 12:07:32.000000 HawaData-0.5.0/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.0/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-23 08:32:27.695752 HawaData-0.5.0/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.0/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.694164 HawaData-0.5.0/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.0/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:48:32.817110 HawaData-0.5.1/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:48:32.807748 HawaData-0.5.1/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2358 2023-05-23 08:48:32.000000 HawaData-0.5.1/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      521 2023-05-23 08:48:32.000000 HawaData-0.5.1/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-23 08:48:32.000000 HawaData-0.5.1/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-23 08:48:32.000000 HawaData-0.5.1/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2358 2023-05-23 08:48:32.816830 HawaData-0.5.1/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.1/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:48:32.808309 HawaData-0.5.1/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.1/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:48:32.810299 HawaData-0.5.1/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.1/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.1/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.1/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.1/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:48:32.812009 HawaData-0.5.1/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.1/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9282 2023-05-23 07:49:48.000000 HawaData-0.5.1/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.1/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.1/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.1/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:48:32.814307 HawaData-0.5.1/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.1/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.1/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.1/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1592 2023-05-23 08:41:21.000000 HawaData-0.5.1/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.1/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:48:32.815558 HawaData-0.5.1/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.1/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    24126 2023-05-23 08:41:59.000000 HawaData-0.5.1/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.1/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-23 08:48:32.817187 HawaData-0.5.1/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.1/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:48:32.816195 HawaData-0.5.1/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.1/test/test_query.py
```

### Comparing `HawaData-0.5.0/HawaData.egg-info/PKG-INFO` & `HawaData-0.5.1/HawaData.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.0
+Version: 0.5.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -82,7 +82,8 @@
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
 - 0.3.7 update pandas to 2+
 - 0.3.8 fix loss data
 - 0.4.0 add case project_id
 - 0.4.1 fix miss grade data
 - 0.5.0 add health api data
+- 0.5.1 add grade param
```

### Comparing `HawaData-0.5.0/HawaData.egg-info/SOURCES.txt` & `HawaData-0.5.1/HawaData.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/PKG-INFO` & `HawaData-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.5.0
+Version: 0.5.1
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -82,7 +82,8 @@
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
 - 0.3.7 update pandas to 2+
 - 0.3.8 fix loss data
 - 0.4.0 add case project_id
 - 0.4.1 fix miss grade data
 - 0.5.0 add health api data
+- 0.5.1 add grade param
```

### Comparing `HawaData-0.5.0/README.md` & `HawaData-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/hawa/base/db.py` & `HawaData-0.5.1/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/hawa/base/init.py` & `HawaData-0.5.1/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/hawa/common/data.py` & `HawaData-0.5.1/hawa/common/data.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/hawa/common/query.py` & `HawaData-0.5.1/hawa/common/query.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/hawa/common/utils.py` & `HawaData-0.5.1/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/hawa/config.py` & `HawaData-0.5.1/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/hawa/data/klass.py` & `HawaData-0.5.1/hawa/data/klass.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from collections import Counter
 from dataclasses import dataclass
 from typing import Optional
 
 import pandas as pd
 
 from hawa.common.query import MetaUnit
 from hawa.config import project
@@ -15,15 +14,14 @@
     meta_unit_type: str = 'class'
 
 
 @dataclass
 class ClassHealthApiData(ClassMixin, HealthApiData):
     """使用 school id 作为 meta_unit_id，额外增加班级的逻辑"""
     meta_class_id: Optional[int] = None  # 必填
-    grade: Optional[int] = None  # 必填
     class_id: Optional[int] = None
     class_name: Optional[str] = ''
 
     def _to_init_a0_meta(self):
         if not self.grade:
             raise ValueError("grade 必填")
         if not self.meta_class_id:
@@ -34,24 +32,16 @@
     def _to_init_a_meta_unit(self):
         super()._to_init_a_meta_unit()
         self.meta_unit = MetaUnit(
             id=self.meta_unit_id, name=f"{self.meta_unit.name}{self.class_name}",
             short_name=self.meta_unit.short_name
         )
 
-    def _to_init_d_cases(self):
-        super()._to_init_d_cases()
-        self.cases = self.cases.loc[self.cases['id'] % 100 == self.grade, :]
-        self.case_ids = self.cases['id'].tolist()
-        self.case_project_ids = Counter(self.cases['project_id'].tolist())
-        project.logger.debug(f'cases: {len(self.cases)}')
-
     def _to_init_e_answers(self):
         """筛选班级的答案"""
         super()._to_init_e_answers()
         records = []
         for _, row in self.answers.iterrows():
             if int(str(row['student_id'])[:15]) == self.meta_class_id:
                 records.append(row)
         self.answers = pd.DataFrame.from_records(records)
         project.logger.debug(f'class answers: {len(self.answers)}')
-
```

### Comparing `HawaData-0.5.0/hawa/data/school.py` & `HawaData-0.5.1/hawa/data/school.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/hawa/paper/health.py` & `HawaData-0.5.1/hawa/paper/health.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """健康测评数据"""
 import itertools
 import json
 import random
-from collections import defaultdict
+from collections import defaultdict, Counter
 from dataclasses import dataclass, field
-from typing import Union, Set
+from typing import Union, Set, Optional
 
 import pandas as pd
 from munch import Munch
 from pingouin import cronbach_alpha
 
 from hawa.common.data import CommonData
 from hawa.config import project
@@ -26,14 +26,24 @@
         else:
             return text.replace('还', '')
 
 
 @dataclass
 class HealthApiData(HealthData):
     """为 yingde api 项目提供基类"""
+    grade: Optional[int] = None  # 必填
+
+    def _to_init_d_cases(self):
+        """如果有年级参数，则筛选年级暑假"""
+        super()._to_init_d_cases()
+        if self.grade:
+            self.cases = self.cases.loc[self.cases['id'] % 100 == self.grade, :]
+            self.case_ids = self.cases['id'].tolist()
+            self.case_project_ids = Counter(self.cases['project_id'].tolist())
+            project.logger.debug(f'cases: {len(self.cases)}')
 
     def score_rank(self, grade: int):
         """某年级 健康素养水平各等级占比"""
         base = {'优秀': 0, '良好': 0, '中等': 0, '待提高': 0}
         final_scores = self.final_scores[self.final_scores['grade'] == grade]
         raw = dict(final_scores['level'].value_counts())
         data = base | raw
```

### Comparing `HawaData-0.5.0/hawa/paper/mht.py` & `HawaData-0.5.1/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/setup.py` & `HawaData-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.5.0/test/test_query.py` & `HawaData-0.5.1/test/test_query.py`

 * *Files identical despite different names*

