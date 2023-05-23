# Comparing `tmp/HawaData-0.4.1.tar.gz` & `tmp/HawaData-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HawaData-0.4.1.tar", last modified: Tue May 16 03:27:13 2023, max compression
+gzip compressed data, was "HawaData-0.5.0.tar", last modified: Tue May 23 08:32:27 2023, max compression
```

## Comparing `HawaData-0.4.1.tar` & `HawaData-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.575273 HawaData-0.4.1/
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.567239 HawaData-0.4.1/HawaData.egg-info/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2306 2023-05-16 03:27:13.000000 HawaData-0.4.1/HawaData.egg-info/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      484 2023-05-16 03:27:13.000000 HawaData-0.4.1/HawaData.egg-info/SOURCES.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-16 03:27:13.000000 HawaData-0.4.1/HawaData.egg-info/dependency_links.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-16 03:27:13.000000 HawaData-0.4.1/HawaData.egg-info/top_level.txt
--rw-r--r--   0 wangzhou   (501) staff       (20)     2306 2023-05-16 03:27:13.574974 HawaData-0.4.1/PKG-INFO
--rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.4.1/README.md
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.567784 HawaData-0.4.1/hawa/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.4.1/hawa/__init__.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.569529 HawaData-0.4.1/hawa/base/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.4.1/hawa/base/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.4.1/hawa/base/db.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.4.1/hawa/base/decos.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.4.1/hawa/base/init.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.570923 HawaData-0.4.1/hawa/common/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.4.1/hawa/common/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     8948 2023-05-16 03:27:04.000000 HawaData-0.4.1/hawa/common/data.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5320 2023-05-16 03:26:37.000000 HawaData-0.4.1/hawa/common/query.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.4.1/hawa/common/utils.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.4.1/hawa/config.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.572394 HawaData-0.4.1/hawa/data/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.4.1/hawa/data/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      336 2022-12-13 08:17:02.000000 HawaData-0.4.1/hawa/data/district.py
--rw-r--r--   0 wangzhou   (501) staff       (20)      472 2022-12-28 09:14:15.000000 HawaData-0.4.1/hawa/data/school.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.573514 HawaData-0.4.1/hawa/paper/
--rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.4.1/hawa/paper/__init__.py
--rw-r--r--   0 wangzhou   (501) staff       (20)    22995 2023-05-05 09:08:17.000000 HawaData-0.4.1/hawa/paper/health.py
--rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.4.1/hawa/paper/mht.py
--rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-16 03:27:13.575384 HawaData-0.4.1/setup.cfg
--rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.4.1/setup.py
-drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-16 03:27:13.574246 HawaData-0.4.1/test/
--rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.4.1/test/test_query.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.695590 HawaData-0.5.0/
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.678775 HawaData-0.5.0/HawaData.egg-info/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2334 2023-05-23 08:32:27.000000 HawaData-0.5.0/HawaData.egg-info/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      521 2023-05-23 08:32:27.000000 HawaData-0.5.0/HawaData.egg-info/SOURCES.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        1 2023-05-23 08:32:27.000000 HawaData-0.5.0/HawaData.egg-info/dependency_links.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)        5 2023-05-23 08:32:27.000000 HawaData-0.5.0/HawaData.egg-info/top_level.txt
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2334 2023-05-23 08:32:27.695157 HawaData-0.5.0/PKG-INFO
+-rw-r--r--   0 wangzhou   (501) staff       (20)      669 2022-12-02 07:10:45.000000 HawaData-0.5.0/README.md
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.679340 HawaData-0.5.0/hawa/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:39:05.000000 HawaData-0.5.0/hawa/__init__.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.682910 HawaData-0.5.0/hawa/base/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 05:35:03.000000 HawaData-0.5.0/hawa/base/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     3014 2023-05-05 08:28:22.000000 HawaData-0.5.0/hawa/base/db.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      173 2022-12-01 06:05:08.000000 HawaData-0.5.0/hawa/base/decos.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      845 2022-12-02 03:09:07.000000 HawaData-0.5.0/hawa/base/init.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.686054 HawaData-0.5.0/hawa/common/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-11-30 09:40:41.000000 HawaData-0.5.0/hawa/common/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     9282 2023-05-23 07:49:48.000000 HawaData-0.5.0/hawa/common/data.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5323 2023-05-23 06:47:14.000000 HawaData-0.5.0/hawa/common/query.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2784 2023-05-05 08:28:22.000000 HawaData-0.5.0/hawa/common/utils.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2551 2023-03-29 04:22:37.000000 HawaData-0.5.0/hawa/config.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.690276 HawaData-0.5.0/hawa/data/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 08:59:59.000000 HawaData-0.5.0/hawa/data/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      311 2023-05-22 06:36:14.000000 HawaData-0.5.0/hawa/data/city.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      432 2023-05-22 06:36:14.000000 HawaData-0.5.0/hawa/data/district.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     1995 2023-05-23 07:53:45.000000 HawaData-0.5.0/hawa/data/klass.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)      564 2023-05-22 09:15:45.000000 HawaData-0.5.0/hawa/data/school.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.692975 HawaData-0.5.0/hawa/paper/
+-rw-r--r--   0 wangzhou   (501) staff       (20)        0 2022-12-01 09:27:31.000000 HawaData-0.5.0/hawa/paper/__init__.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)    23638 2023-05-22 12:07:32.000000 HawaData-0.5.0/hawa/paper/health.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)     5273 2023-05-05 07:06:02.000000 HawaData-0.5.0/hawa/paper/mht.py
+-rw-r--r--   0 wangzhou   (501) staff       (20)       38 2023-05-23 08:32:27.695752 HawaData-0.5.0/setup.cfg
+-rw-r--r--   0 wangzhou   (501) staff       (20)      879 2023-05-05 08:13:11.000000 HawaData-0.5.0/setup.py
+drwxr-xr-x   0 wangzhou   (501) staff       (20)        0 2023-05-23 08:32:27.694164 HawaData-0.5.0/test/
+-rw-r--r--   0 wangzhou   (501) staff       (20)     2208 2022-12-08 07:17:34.000000 HawaData-0.5.0/test/test_query.py
```

### Comparing `HawaData-0.4.1/HawaData.egg-info/PKG-INFO` & `HawaData-0.5.0/HawaData.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.4.1
+Version: 0.5.0
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -81,7 +81,8 @@
 - 0.3.4 up to py3.11
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
 - 0.3.7 update pandas to 2+
 - 0.3.8 fix loss data
 - 0.4.0 add case project_id
 - 0.4.1 fix miss grade data
+- 0.5.0 add health api data
```

### Comparing `HawaData-0.4.1/PKG-INFO` & `HawaData-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HawaData
-Version: 0.4.1
+Version: 0.5.0
 Summary: Use For Unified Hawa Data.
 Home-page: https://github.com/StevenLianaL/HawaData
 Author: Steven Wang
 Author-email: brightstar8284@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
@@ -81,7 +81,8 @@
 - 0.3.4 up to py3.11
 - 0.3.5 fix engine encoding
 - 0.3.6 update sqlarchemy to 2+
 - 0.3.7 update pandas to 2+
 - 0.3.8 fix loss data
 - 0.4.0 add case project_id
 - 0.4.1 fix miss grade data
+- 0.5.0 add health api data
```

### Comparing `HawaData-0.4.1/README.md` & `HawaData-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.1/hawa/base/db.py` & `HawaData-0.5.0/hawa/base/db.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.1/hawa/base/init.py` & `HawaData-0.5.0/hawa/base/init.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.1/hawa/common/data.py` & `HawaData-0.5.0/hawa/common/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         attrs['query'] = DataQuery()
         return super().__new__(cls, name, bases, attrs)
 
 
 @dataclass
 class CommonData(metaclass=MetaCommomData):
     # 构造单位
-    meta_unit_type: Optional[str] = ''  # school/district/city/province/country
+    meta_unit_type: Optional[str] = ''  # class/school/district/city/province/country
     meta_unit_id: Optional[int] = None
     meta_unit: Optional[Any] = None
 
     # 时间目标
     target_year: Optional[int] = None
     last_year_num: Optional[int] = None
     is_load_last: bool = True  # 仅计算往年数据时 为 False
@@ -98,18 +98,23 @@
         self.last_year_num = self.target_year - 1
         project.logger.info(f'target_year: {self.target_year}')
 
     def _to_init_c_schools(self):
         if self.school_ids:
             self.schools = self.query.query_schools_by_ids(self.school_ids)
         else:
-            if self.meta_unit_type == 'country':
-                self.schools = self.query.query_schools_all()
-            else:
-                self.schools = self.query.query_schools_by_startwith(self.meta_unit_id)
+            match self.meta_unit_type:
+                case 'country':
+                    self.schools = self.query.query_schools_all()
+                case 'province':
+                    self.schools = self.query.query_schools_by_startwith(self.meta_unit_id // 10000)
+                case 'city':
+                    self.schools = self.query.query_schools_by_startwith(self.meta_unit_id // 100)
+                case 'district' | 'school' | 'class':
+                    self.schools = self.query.query_schools_by_startwith(self.meta_unit_id)
             self.school_ids = self.schools['id'].tolist()
         project.logger.debug(f'schools: {len(self.schools)}')
 
     def _to_init_d_cases(self):
         start_stamp = pendulum.datetime(self.target_year, 1, 1)
         end_stamp = pendulum.datetime(self.target_year + 1, 1, 1)
         start_stamp_str = start_stamp.format(project.format)
```

### Comparing `HawaData-0.4.1/hawa/common/query.py` & `HawaData-0.5.0/hawa/common/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 import pandas as pd
 from sqlalchemy import text
 
 from hawa.base.db import DbUtil
 from hawa.base.decos import singleton
 
+MetaUnit = namedtuple("MetaUnit", ["id", "name", "short_name"])
+
 
 @singleton
 class DataQuery:
     db = DbUtil()
 
     def query_unit(self, meta_unit_type: str, meta_unit_id: str):
-        MetaUnit = namedtuple("MetaUnit", ["id", "name", "short_name"])
         match meta_unit_type:
-            case 'school':
+            case 'school' | 'class':
                 sql = f"select id,name,short_name from schools where id={meta_unit_id};"
                 data = self.db.query_by_sql(sql=sql, mode='one')
                 meta_unit = MetaUnit(**data)
             case 'district' | 'city' | 'province':
                 sql = f"select id,name from locations where id={meta_unit_id};"
                 data = self.db.query_by_sql(sql=sql, mode='one')
                 meta_unit = MetaUnit(**data, short_name=data['name'])
```

### Comparing `HawaData-0.4.1/hawa/common/utils.py` & `HawaData-0.5.0/hawa/common/utils.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.1/hawa/config.py` & `HawaData-0.5.0/hawa/config.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.1/hawa/paper/health.py` & `HawaData-0.5.0/hawa/paper/health.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,31 @@
         if condition:
             return text
         else:
             return text.replace('还', '')
 
 
 @dataclass
+class HealthApiData(HealthData):
+    """为 yingde api 项目提供基类"""
+
+    def score_rank(self, grade: int):
+        """某年级 健康素养水平各等级占比"""
+        base = {'优秀': 0, '良好': 0, '中等': 0, '待提高': 0}
+        final_scores = self.final_scores[self.final_scores['grade'] == grade]
+        raw = dict(final_scores['level'].value_counts())
+        data = base | raw
+        sum_data = sum(data.values())
+        if not sum_data:
+            raise ValueError(f'grade {grade} score rank is empty')
+        percent = {k: round(v / sum_data, 2) for k, v in data.items()}
+        return percent
+
+
+@dataclass
 class HealthReportData(HealthData):
     # 计算数据
     code_scores: pd.DataFrame = field(default_factory=pd.DataFrame)
     summary_scores: dict = field(default_factory=dict)
     grade_good_bad = None  # 优势 优先关注点
 
     grade_rank_dis = None  # 年级、性别、水平学生分布占比
```

### Comparing `HawaData-0.4.1/hawa/paper/mht.py` & `HawaData-0.5.0/hawa/paper/mht.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.1/setup.py` & `HawaData-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `HawaData-0.4.1/test/test_query.py` & `HawaData-0.5.0/test/test_query.py`

 * *Files identical despite different names*

