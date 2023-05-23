# Comparing `tmp/seakybox-0.1.tar.gz` & `tmp/seakybox-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seakybox-0.1.tar", last modified: Thu May 12 05:06:09 2022, max compression
+gzip compressed data, was "seakybox-0.2.tar", last modified: Tue May 23 15:53:55 2023, max compression
```

## Comparing `seakybox-0.1.tar` & `seakybox-0.2.tar`

### file list

```diff
@@ -1,46 +1,54 @@
-drwxrwxrwx   0        0        0        0 2022-05-12 05:06:09.273640 seakybox-0.1/
--rw-rw-rw-   0        0        0     1088 2021-01-19 06:57:43.000000 seakybox-0.1/LICENSE
--rw-rw-rw-   0        0        0      502 2022-05-12 05:06:09.270648 seakybox-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      100 2022-05-12 03:44:00.000000 seakybox-0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-05-12 05:06:09.225769 seakybox-0.1/seakybox/
--rw-rw-rw-   0        0        0      264 2022-05-12 03:47:20.000000 seakybox-0.1/seakybox/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-12 05:06:09.235742 seakybox-0.1/seakybox/data/
--rw-rw-rw-   0        0        0       96 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/data/__init__.py
--rw-rw-rw-   0        0        0    43134 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/data/mysql.py
--rw-rw-rw-   0        0        0     6928 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/data/pd.py
--rw-rw-rw-   0        0        0    16273 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/data/redis_func.py
-drwxrwxrwx   0        0        0        0 2022-05-12 05:06:09.249706 seakybox-0.1/seakybox/func/
--rw-rw-rw-   0        0        0       97 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/func/__init__.py
--rw-rw-rw-   0        0        0    17140 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/func/base.py
--rw-rw-rw-   0        0        0      577 2021-04-02 08:58:27.000000 seakybox-0.1/seakybox/func/interactive.py
--rw-rw-rw-   0        0        0     4266 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/func/log.py
--rw-rw-rw-   0        0        0      518 2022-05-12 02:32:11.000000 seakybox-0.1/seakybox/func/misc.py
--rw-rw-rw-   0        0        0    19453 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/func/mrun.py
--rw-rw-rw-   0        0        0     4034 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/func/parser.py
--rw-rw-rw-   0        0        0    12524 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/func/string.py
--rw-rw-rw-   0        0        0     2876 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/func/time.py
-drwxrwxrwx   0        0        0        0 2022-05-12 05:06:09.258682 seakybox-0.1/seakybox/net/
--rw-rw-rw-   0        0        0       97 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/net/__init__.py
--rw-rw-rw-   0        0        0     1631 2021-07-21 02:32:44.000000 seakybox-0.1/seakybox/net/connectivity.py
--rw-rw-rw-   0        0        0     9126 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/net/http.py
--rw-rw-rw-   0        0        0     3655 2021-06-25 06:25:11.000000 seakybox-0.1/seakybox/net/ip.py
--rw-rw-rw-   0        0        0     2716 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/net/proxy.py
--rw-rw-rw-   0        0        0     1707 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/net/sserver.py
-drwxrwxrwx   0        0        0        0 2022-05-12 05:06:09.262671 seakybox-0.1/seakybox/notify/
--rw-rw-rw-   0        0        0       94 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/notify/__init__.py
--rw-rw-rw-   0        0        0     1181 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/notify/im.py
--rw-rw-rw-   0        0        0     9469 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/notify/sendmail.py
-drwxrwxrwx   0        0        0        0 2022-05-12 05:06:09.268654 seakybox-0.1/seakybox/os/
--rw-rw-rw-   0        0        0       97 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/os/__init__.py
--rw-rw-rw-   0        0        0    15140 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/os/cmd.py
--rw-rw-rw-   0        0        0      566 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/os/compress.py
--rw-rw-rw-   0        0        0      873 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/os/info.py
--rw-rw-rw-   0        0        0     6450 2021-01-19 06:57:43.000000 seakybox-0.1/seakybox/os/oper.py
-drwxrwxrwx   0        0        0        0 2022-05-12 05:06:09.229759 seakybox-0.1/seakybox.egg-info/
--rw-rw-rw-   0        0        0      502 2022-05-12 05:06:08.000000 seakybox-0.1/seakybox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      840 2022-05-12 05:06:09.000000 seakybox-0.1/seakybox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-12 05:06:08.000000 seakybox-0.1/seakybox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      165 2022-05-12 05:06:09.000000 seakybox-0.1/seakybox.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-05-12 05:06:09.000000 seakybox-0.1/seakybox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-12 05:06:09.274638 seakybox-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1033 2022-05-12 03:47:40.000000 seakybox-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:53:55.430265 seakybox-0.2/
+-rw-rw-rw-   0        0        0     1088 2021-01-19 06:57:43.000000 seakybox-0.2/LICENSE
+-rw-rw-rw-   0        0        0     1032 2023-05-23 15:53:55.429281 seakybox-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2022-11-23 01:20:24.000000 seakybox-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 15:53:55.359453 seakybox-0.2/seakybox/
+-rw-rw-rw-   0        0        0      264 2023-05-23 15:52:59.000000 seakybox-0.2/seakybox/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:53:55.378402 seakybox-0.2/seakybox/data/
+-rw-rw-rw-   0        0        0       96 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/data/__init__.py
+-rw-rw-rw-   0        0        0    12807 2023-04-04 11:52:34.000000 seakybox-0.2/seakybox/data/mongo_func.py
+-rw-rw-rw-   0        0        0    43124 2022-06-27 16:36:20.000000 seakybox-0.2/seakybox/data/mysql.py
+-rw-rw-rw-   0        0        0      175 2022-05-15 02:34:09.000000 seakybox-0.2/seakybox/data/mysql_pd.py
+-rw-rw-rw-   0        0        0     6968 2022-06-21 01:20:46.000000 seakybox-0.2/seakybox/data/pd.py
+-rw-rw-rw-   0        0        0    16804 2022-05-29 02:25:20.000000 seakybox-0.2/seakybox/data/redis_func.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:53:55.396355 seakybox-0.2/seakybox/func/
+-rw-rw-rw-   0        0        0       97 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/func/__init__.py
+-rw-rw-rw-   0        0        0    17828 2023-03-25 04:04:44.000000 seakybox-0.2/seakybox/func/base.py
+-rw-rw-rw-   0        0        0      982 2022-08-05 09:08:28.000000 seakybox-0.2/seakybox/func/interactive.py
+-rw-rw-rw-   0        0        0     4546 2022-06-25 16:19:43.000000 seakybox-0.2/seakybox/func/log.py
+-rw-rw-rw-   0        0        0    19453 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/func/mrun.py
+-rw-rw-rw-   0        0        0     3482 2023-05-08 06:13:37.000000 seakybox-0.2/seakybox/func/number.py
+-rw-rw-rw-   0        0        0     4034 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/func/parser.py
+-rw-rw-rw-   0        0        0    10871 2022-05-26 15:48:30.000000 seakybox-0.2/seakybox/func/string.py
+-rw-rw-rw-   0        0        0     3857 2022-06-22 15:45:24.000000 seakybox-0.2/seakybox/func/time.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:53:55.401340 seakybox-0.2/seakybox/misc/
+-rw-rw-rw-   0        0        0       89 2022-06-26 01:49:37.000000 seakybox-0.2/seakybox/misc/__init__.py
+-rw-rw-rw-   0        0        0      518 2022-05-12 02:32:11.000000 seakybox-0.2/seakybox/misc/ctf.py
+-rw-rw-rw-   0        0        0     8077 2022-07-10 16:24:07.000000 seakybox-0.2/seakybox/misc/token.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:53:55.411314 seakybox-0.2/seakybox/net/
+-rw-rw-rw-   0        0        0       97 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/net/__init__.py
+-rw-rw-rw-   0        0        0     1631 2021-07-21 02:32:44.000000 seakybox-0.2/seakybox/net/connectivity.py
+-rw-rw-rw-   0        0        0     9047 2022-06-07 06:28:45.000000 seakybox-0.2/seakybox/net/http.py
+-rw-rw-rw-   0        0        0     3658 2022-06-10 10:43:17.000000 seakybox-0.2/seakybox/net/ip.py
+-rw-rw-rw-   0        0        0     2716 2022-05-21 08:40:13.000000 seakybox-0.2/seakybox/net/proxy.py
+-rw-rw-rw-   0        0        0     1707 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/net/sserver.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:53:55.420290 seakybox-0.2/seakybox/notify/
+-rw-rw-rw-   0        0        0       94 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/notify/__init__.py
+-rw-rw-rw-   0        0        0     1739 2022-12-04 07:46:13.000000 seakybox-0.2/seakybox/notify/dingding.py
+-rw-rw-rw-   0        0        0     1434 2022-11-03 08:00:24.000000 seakybox-0.2/seakybox/notify/ftqq.py
+-rw-rw-rw-   0        0        0     1187 2022-06-26 01:49:37.000000 seakybox-0.2/seakybox/notify/im.py
+-rw-rw-rw-   0        0        0     9469 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/notify/sendmail.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:53:55.427271 seakybox-0.2/seakybox/os/
+-rw-rw-rw-   0        0        0       97 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/os/__init__.py
+-rw-rw-rw-   0        0        0    15142 2023-01-04 13:34:55.000000 seakybox-0.2/seakybox/os/cmd.py
+-rw-rw-rw-   0        0        0      566 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/os/compress.py
+-rw-rw-rw-   0        0        0      873 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/os/info.py
+-rw-rw-rw-   0        0        0     6450 2021-01-19 06:57:43.000000 seakybox-0.2/seakybox/os/oper.py
+drwxrwxrwx   0        0        0        0 2023-05-23 15:53:55.368429 seakybox-0.2/seakybox.egg-info/
+-rw-rw-rw-   0        0        0     1032 2023-05-23 15:53:55.000000 seakybox-0.2/seakybox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1018 2023-05-23 15:53:55.000000 seakybox-0.2/seakybox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 15:53:55.000000 seakybox-0.2/seakybox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      161 2023-05-23 15:53:55.000000 seakybox-0.2/seakybox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-23 15:53:55.000000 seakybox-0.2/seakybox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 15:53:55.431260 seakybox-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1029 2022-11-22 07:31:58.000000 seakybox-0.2/setup.py
```

### Comparing `seakybox-0.1/LICENSE` & `seakybox-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox/data/mysql.py` & `seakybox-0.2/seakybox/data/mysql.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,23 @@
 
 import os
 import re
 import traceback
 from collections import OrderedDict
 from functools import wraps
 
-import pandas
 import pandas as pd
 from sqlalchemy import Float
 from sqlalchemy import INTEGER as INTEGER1, FLOAT, create_engine, UniqueConstraint
 from sqlalchemy import event
 from sqlalchemy import exc
 from sqlalchemy.dialects.mysql import BIGINT, INTEGER, SMALLINT, TINYINT
 from sqlalchemy.orm import sessionmaker
 
-from ..data.pd import set_none
+from ..data.pd import df_set_none
 from ..func.string import change_type, add_quote
 from ..func.time import datetime_to_string
 
 
 # from ..func.log import make_logger
 
 
@@ -401,15 +400,15 @@
             items_skip = []
 
         changed_cols = df_diff.keys().tolist()
         items_need_update = []
         for x in list_diff:
             items_need_update.append((df_new_copy.loc[x].to_dict(), df_old_copy.loc[x].to_dict()))
         items_new = df_new_copy.loc[compare['left_only']]
-        items_new = set_none(items_new).to_dict(orient='index')
+        items_new = df_set_none(items_new).to_dict(orient='index')
         items_miss = df_new_copy.loc[compare['right_only']].to_dict(orient='index')
 
         # items_new = df_new_copy.loc[df_diff.index].to_dict(orient='index')
 
         return {'data_new': data_new, 'data_old': data_old,
                 'items_new': items_new, 'items_need_update': items_need_update,
                 'items_miss': items_miss, 'items_skip': items_skip,
@@ -467,15 +466,15 @@
             param_add = {}
         if not param_update:
             param_update = {}
         if key and key not in param_update:
             param_update['key'] = key
         if not param_delete:
             param_delete = {}
-        if not use_df and isinstance(data_new, pandas.core.frame.DataFrame):
+        if not use_df and isinstance(data_new, pd.core.frame.DataFrame):
             data_new = data_new.to_dict(orient='records')
         if isinstance(data_new, list):
             data_new = {x[key]: x for x in data_new}
         if isinstance(data_old, list):
             data_old = {x[key]: x for x in data_old}
         if use_df:
             d = self._update_compare_df(data_new, data_old, key, cols, func_skip, df_to_str)
@@ -929,15 +928,15 @@
         :param kwargs: read_sql_query的kwargs
             index_col=['device_id]
             parse_dates=['finance_pay_date']
         :return:
         如果列col是int，但有None，该col会被返回成float
         '''
         df = self._read_sql_query(sql, **kwargs)
-        df = set_none(df)
+        df = df_set_none(df)
         cols = df.columns.tolist()
         if ret_df:
             if apply_func:
                 df.index = df.apply(apply_func, axis=1)
             if key:
                 df.index = df.apply(lambda x: joint.join(x[k] for k in key) if isinstance(key, list) else x[key],
                                     axis=1)
```

### Comparing `seakybox-0.1/seakybox/data/pd.py` & `seakybox-0.2/seakybox/data/pd.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,25 @@
 import pandas as pd
 
 from ..func.string import change_type
 from ..net.ip import ip2int
 from ..os.oper import path_open
 
 
-def set_none(df, other=None, **kwargs):
+def df_set_none(df, other=None, **kwargs):
     '''将nan替换为None, 可以应用于series'''
     return df.where(pd.notnull(df), other=other, **kwargs)
 
 
-def drop_nan(df, col):
+def df_drop_nan(df, col):
     '''按某一列nan舍弃行'''
     return df[pd.notnull(df[col])]
 
 
-def select_row(df, func):
+def df_select_row(df, func):
     '''
     :param df:
     :param func: return True/False
     :return:
     '''
     df1 = df.apply(func, axis=1)
     return df1[df1]
@@ -87,15 +87,15 @@
                     _sort_by.append(key)
                 else:
                     _sort_by.append(co)
         else:
             _sort_by = sort_by
         df = df.sort_values(by=_sort_by, axis=0, ascending=not sort_desc, inplace=False)[origin_columns]
     if use_none:
-        df = set_none(df, other=none_str)
+        df = df_set_none(df, other=none_str)
     return df
 
 
 def array_to_df(lst, index=None, columns=None, **kwargs):
     if not index:
         index = range(int(len(lst) / len(columns)))
     if not columns:
@@ -103,15 +103,15 @@
     return pd.DataFrame(np.array(lst).reshape(len(index), len(columns)), index=index, columns=columns, **kwargs)
 
 
 def array_to_np(list, **kwargs):
     return np.array(list, **kwargs)
 
 
-def add_columns(df, col, value, axis=1):
+def df_add_columns(df, col, value, axis=1):
     '''
     :param df:
     :param col: str/list
     :param value:
         如果value是函数，如果如果col是list，则value需要是一个函数，返回list；如果col是str, value返回str。
         如果没有匹配，最好返回np.nan，可以后续dropna()
     :return:
@@ -192,19 +192,20 @@
     '''
     1、pd.to_numeric(series)
     2、df['x'].astype(str)
     3、df = df.infer_objects()'''
     pass
 
 
-def to_excel(data, fn, mode='w', engine=None):
+def df_to_excel(data, fn, mode='w', engine=None):
     '''
-    :param data:  (df, {'sheet_name': sheet_name, 'index': False})
+    :param data:  [(df, {'sheet_name': sheet_name, 'index': False})]
     :param fn:
     :param mode:  'a'模式，需要安装openpyxl
+    :param engine:
     :return:
     '''
     if mode == 'a':
         engine = 'openpyxl'
     writer = pd.ExcelWriter(fn, engine=engine, mode=mode)
     for df, kw in data:
         kw['index'] = kw.get('index')
```

### Comparing `seakybox-0.1/seakybox/data/redis_func.py` & `seakybox-0.2/seakybox/data/redis_func.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,37 +14,49 @@
 
 SCAN_COUNT = 10000
 PIPELINE_N = 10000
 
 
 class RedisC(Redis):
     def __init__(self, host=None, port=6379, db=0, password=None, sentinels=None, service_name=None,
-                 decode_responses=True, socket_timeout=None, log=None, *args, **kwargs):
+                 decode_responses=True, socket_timeout=None, log=None, health_check_interval=30, *args, **kwargs):
         if sentinels:
             sentinel = Sentinel(sentinels=sentinels)
             master = sentinel.discover_master(service_name=service_name)
             host, port = master
         self.server = {'host': host, 'port': port, 'db': db, 'password': password, 'decode_responses': decode_responses,
                        'socket_timeout': socket_timeout}
+        self.health_check_interval = health_check_interval
         self.log = log if log else SimpleLog()
         self.pool = ConnectionPool(*args, **self.server, **kwargs)
-        Redis.__init__(self, connection_pool=self.pool)
+        super().__init__(
+            connection_pool=self.pool, health_check_interval=self.health_check_interval, retry_on_timeout=True)
         # Redis.__init__(self, *args, **self.server, **kwargs)
         self.cache_result = {}
 
     def show_server(self):
         '''
         显示 redis server 信息
         :return:
         '''
-        msg = 'Redis: {host}:{port}/{db}'.format(**self.server)
-        if self.log:
-            self.log.info(msg)
-        else:
-            print(msg)
+        msg = 'Redis: {host}:{port}/{db}, Status: {}'.format(self.ping(), **self.server)
+        self.log.info(msg)
+
+    def get(self, name):
+        value = super(RedisC, self).get(name)
+        try:
+            return json.loads(value)
+        except Exception as e:
+            return value
+
+    def set(self, name, value, retry=2, **kwargs):
+        if not isinstance(value, str):
+            value = json.dumps(value)
+        resp = super(RedisC, self).set(name, value, **kwargs)
+        return resp
 
     def count_keys(self, prefix, count=SCAN_COUNT, ret_keys=False, limit=None, key_with_prefix=True):
         '''
         统计 keys 数量
         :param prefix:
         :param count:
         :param ret_keys:
```

### Comparing `seakybox-0.1/seakybox/func/base.py` & `seakybox-0.2/seakybox/func/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,19 +132,22 @@
 
 def is_instance(obj):
     '''对象是一个实例'''
     if hasattr(obj, '__dict__') and not callable(obj):
         return True
 
 
-def catch_exception(ignore=False, retry=0, prune_func=None):
+def catch_exception(ignore=False, retry=0, prune_func=None, interval=1, print_exception=1, raise_exp=False):
     '''
     :param ignore: 不记录错误, 尝试性的exception
     :param retry: 重试次数
     :param prune_func: 过滤一些不重要的log
+    :param interval: 重试等待时间
+    :param print_exception: 打印错误, 0-不打印，1-打印异常，2-打印trace
+    :param raise_exp: 是否要抛出异常
     :return:
     如果 kwargs中含有no_catch_exception，忽略本catch
     如果是普通函数，可以附加 _show_exception 参数控制是否显示具体异常，不会真正传入f；
         如果是in_class，还会被self.traceback影响
     '''
 
     def deco(f):
@@ -175,16 +178,23 @@
                 except AssertionError as e:
                     # e不能传递出try
                     excep_tp = 'assert'
                     excep, e1, trace = True, e, '{}'.format(traceback.format_exc())
                 except Exception as e:
                     excep, e1, trace = True, e, '{}'.format(traceback.format_exc())
                 i += 1
+                if print_exception & 1 == 1:
+                    print(e1)
+                elif print_exception & 2 == 2:
+                    print(trace)
+                time.sleep(interval)
             if not excep:
                 return result
+            elif raise_exp:
+                raise trace
             else:
                 d = {'function': real_func.__name__, 'message': '{}'.format(e1), 'except': e1,
                      'trace': trace, 'ignore': ignore}
                 msg = 'function: {function}, exception: {message}, ignore: {ignore}\ntrace: {trace}'.format(**d)
                 if instance and hasattr(instance, 'debug_info'):
                     # 过滤重复的异常
                     if len(instance.debug_info['exception']) == 0 or \
@@ -300,14 +310,20 @@
             if not log_params:
                 log_params = {}
             log_params.update(
                 {'debug': self.debug, 'console': not self.quite, 'name': self.__class__.__name__, 'simple_log': False})
             # 两个类建立默认log时，前者会没有输出？
             self.log = make_logger(**log_params)
 
+    def get_from_cache(self, key, func, func_kw=None):
+        func_kw = func_kw or {}
+        if self.cache.get(key) is None:
+            self.cache[key] = func(**func_kw)
+        return self.cache[key]
+
     def default(self, k):
         return self.control.get(k)
 
     def func_done(self, name=None, cache=None, flag=True):
         '''
         记录函数是否运行
         :param name:
```

### Comparing `seakybox-0.1/seakybox/func/log.py` & `seakybox-0.2/seakybox/func/log.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,28 +7,31 @@
 
 import logging
 import logging.config
 from copy import deepcopy
 from pathlib import Path
 
 from .time import datetime_to_string
-from ..os.info import get_pwd, get_caller
+from ..os.info import get_pwd, get_caller, get_hostname
 
 
-def make_logger(log=None, name=None, stem=None, log_dir='log', work_dir=None, console=True, write=False,
-                focus_error=True, multi_process=True,
+def make_logger(log=None, name=None, stem=None, add_hostname=False, log_dir='log', work_dir=None, filename=None,
+                console=True, write=False,
+                focus_error=True, multi_process=False,
                 level='INFO', debug=False, **kwargs):
     '''
     :param log:
     :param simple_log:   默认使用print
     :param name: logger name
     :param stem: file stem, default filename without type
+    :param add_hostname: add hostname to stem
     :param log_dir:
     :param work_dir:
     :param console:
+    :param filename:  不带后缀
     :param write:
     :param focus_error:     增加error日志
     :param multi_process:   支持多进程
     :param level:
     :param debug:   方便设置debug
     :param level:
         {'handlers': {...}}
@@ -38,26 +41,30 @@
         return log
     work_dir = work_dir or get_pwd()
     caller = get_caller()
     dpath = Path(work_dir) / log_dir
     dpath.mkdir(exist_ok=True)
     stem = stem or caller.stem
     name = name or caller.name
+    if add_hostname:
+        stem = '{}_{}'.format(stem, get_hostname())
+    if not filename:
+        filename = stem
 
     # concurrent_log_handler.ConcurrentRotatingFileHandler 支持多进程，但不能做时间分割
     # logging.handlers.RotatingFileHandler 只支持多线程
     file_handler = {
         'level': 'DEBUG',
         'class': 'concurrent_log_handler.ConcurrentRotatingFileHandler' if multi_process else 'logging.handlers.RotatingFileHandler',
         'maxBytes': 1024 * 1024 * 10,
         'backupCount': 10,
         # If delay is true,
         # then file opening is deferred until the first call to emit().
         'delay': True,
-        'filename': str(dpath / '{0}.log'.format(stem)),
+        'filename': str(dpath / '{0}.log'.format(filename)),
         'formatter': 'verbose'
     }
 
     d = {
         'version': 1,
         'disable_existing_loggers': True,
         'formatters': {
@@ -83,15 +90,15 @@
             'class': 'logging.StreamHandler',
             'formatter': 'verbose'
         }
     if write:
         d['handlers']['file'] = file_handler
         if focus_error:
             file_handler_error = deepcopy(file_handler)
-            file_handler_error.update({'level': 'WARN', 'filename': str(dpath / '{0}_error.log'.format(stem))})
+            file_handler_error.update({'level': 'WARN', 'filename': str(dpath / '{0}_error.log'.format(filename))})
             d['handlers']['file_error'] = file_handler_error
     if 'handlers' in kwargs:
         d['handlers'].update(kwargs['handlers'])
 
     d['loggers'] = {name: {'handlers': d['handlers'].keys(),
                            'level': 'DEBUG' if debug else level, }}
```

### Comparing `seakybox-0.1/seakybox/func/misc.py` & `seakybox-0.2/seakybox/misc/ctf.py`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox/func/mrun.py` & `seakybox-0.2/seakybox/func/mrun.py`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox/func/parser.py` & `seakybox-0.2/seakybox/func/parser.py`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox/func/string.py` & `seakybox-0.2/seakybox/func/string.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,21 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 # @Author: Seaky
 # @Date:   2019/8/20 14:57
 
 import re
-from decimal import Decimal
-
-
-def qround(n, digit=2, retf=False):
-    '''
-    比round更高的精度
-    :param n:
-    :param digit:
-    :param retf:
-    :return:
-    '''
-    r = Decimal(n).quantize(Decimal('0.{}'.format('0' * digit)))
-    if retf:
-        r = float(r)
-    return r
-
-
-def comma_digit(s, tp=int):
-    '''用逗号分割数字'''
-    if isinstance(s, int):
-        return '{,}'.format_map(s)
-    if str_is_number(s, tp, exp=True):
-        return '{:,}'.format(int(s))
-    return s
-
-
-def str_is_number(s, tp=None, exp=True):
-    '''
-
-    :param s:
-    :param tp: 指定int/float，None两者都行
-    :param exp: 扩展，如果s是int/float，也可以返回true
-    :return:
-    '''
-    if not isinstance(s, str):
-        if exp and isinstance(s, int) and tp in (None, int):
-            return True
-        if exp and isinstance(s, float) and tp in (None, float):
-            return True
-        return False
-    if tp == int:
-        return re.match('^\-{,1}\d+\.{0,0}\d+$', s)
-    elif tp == float:
-        return re.match('^\-{,1}\d+\.{1,1}\d+$', s)
-    else:
-        return re.match('^\-{,1}\d+\.{,1}\d+$', s)
+from .number import str_is_number
 
 
 def str_is_email_address(s):
     if isinstance(s, str):
         return re.search('^(?P<id>.+)@(?P<domain>[\w\d]+\.([\w\d]+\.){0,}\w+$)', s)
 
 
-def exact_number(s, base=1000):
-    '''
-    iptables中可以使用-x参数
-    :param s:
-    :param base:
-    :return:
-    '''
-    l = ['k', 'm', 'g', 't']
-    if s.isdigit():
-        return s
-    else:
-        for i, c in enumerate(l):
-            if s[-1].lower() == c:
-                return str(int(s[:-1]) * base ** (i + 1))
-
-
 def obj2list(obj, ret_str=False, sep=',', preserve_blank=False, preserve_none=False, wrapper='', ignore=None, sep2=','):
     '''
     合并 str2list, list2str, add_quote
     'a,b,c' -> ['a', 'b', 'c'] -> ['"a"', '"b"', '"c"'] -> "a","b","c"
     :param obj:
     :param ret_str:  返回str
     :param sep:  原字段分割符
@@ -118,15 +57,15 @@
                                         to_str=to_str, split=False, strip=strip, quote=quote))
     else:
         return '{0}{1}{0}'.format(quote, replace(v, pats=['(^"|"$)', "(^'|'$)"]))
 
 
 def str2list(s, sep=',', preserve_blank=False, wrapper='', filter=None):
     '''
-    分割字符串，添加引号
+    分割字符串，可添加引号
     :param s:
     :param preserve_blank:   是否保留空的item
     :param wrapper: '/"
     :param filter:  过滤回调函数，True过滤
     :return:
     '''
     if s is None:
@@ -143,31 +82,31 @@
         return l
     elif isinstance(s, list):
         return ['{0}{1}{0}'.format(wrapper, str(y)) for y in s]
     else:
         return [s]
 
 
-def list2str(l, sep=',', wrapper='', *args, **kwargs):
+def list2str(lst, sep=',', wrapper='', *args, **kwargs):
     '''
     list转成str，并加上wrapper
-    :param l:
+    :param lst:
     :param sep:
     :param wrapper:
     :param args:
     :param kwargs:
     :return:
     '''
-    if isinstance(l, (list, set)):
-        return sep.join(['{0}{1}{0}'.format(wrapper, x) for x in l])
-    elif isinstance(l, str):
-        l1 = str2list(l, sep=sep, *args, **kwargs)
+    if isinstance(lst, (list, set)):
+        return sep.join(['{0}{1}{0}'.format(wrapper, x) for x in lst])
+    elif isinstance(lst, str):
+        l1 = str2list(lst, sep=sep, *args, **kwargs)
         return list2str(l1, sep=sep, wrapper=wrapper)
     else:
-        return l
+        return lst
 
 
 def arg2list(obj):
     return str2list(obj)
 
 
 def bytes_decode(v, is_hex=False, enconding='utf-8', errors='strict', **kwargs):
@@ -312,15 +251,15 @@
     if space:
         pats.append((' ', '_'))
     if not full:
         pats = [(x[0], '_') for x in pats]
     return replace(s, pats=pats)
 
 
-def sort_port(x, base=100):
+def sort_interface(x, base=100):
     '''排序端口 1/0/1 1/0/10'''
     m = re.findall('\d+', x)
     if m:
         return sum(int(n) * (base ** i) for i, n in enumerate(m[::-1]))
     else:
         return 0
 
@@ -376,17 +315,7 @@
                         _s.append(x[col])
                     else:
                         _s.append(default)
             s.append(sep.join(str(z) for z in _s))
         else:
             s.append(str(x))
     return '\n'.join(s)
-
-
-def confirm(prompt='确认？'):
-    '''
-    确认
-    :param prompt:
-    :return:
-    '''
-    c = input('{} (y|N)  '.format(prompt)).strip()
-    return c.lower() == 'y'
```

### Comparing `seakybox-0.1/seakybox/net/connectivity.py` & `seakybox-0.2/seakybox/net/connectivity.py`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox/net/http.py` & `seakybox-0.2/seakybox/net/http.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import re
 import warnings
 from functools import wraps
 from pathlib import Path
 from urllib import parse
 
 import requests
+from lxml import html
 from bs4 import BeautifulSoup
 
 from ..func.base import MyClass
 from ..func.mrun import MultiRun
 from ..func.parser import ArgParseClass
 
 warnings.filterwarnings("ignore")
@@ -63,77 +64,76 @@
             self.session.headers.update(http_headers)
         # self.status = {}  # for some vars preserve
         self.url_root = kwargs.get('url_root')
 
     def __getattr__(self, item):
         return self.__dict__.get(item, self.kwargs.get(item))
 
-    def fetch(self, url, ret_bs=True, method='GET', timeout=None,
-              retry=3, retry_code=None, retry_not_200=False,
-              ret_raw=False, ret_dic=False, ret_json=False, charset=None, **kwargs):
+    def fetch(self, url, method='GET', timeout=None,
+              retry=3, retry_code=None, retry_not_200=False, ret_dict=False, parse=True,
+              charset=None, **kwargs):
         '''
         :param url:
-        :param ret_bs: 返回bs4 obj
-        :param ret_raw: 返回原始数据
         :param method: GET、POST
         :param retry: 重试次数
         :param retry_code: 重试某些code
         :param retry_not_200: 重试非200
-        :param ret_dic: 返回url, args, result的字典
+        :param ret_dict: 返回url, args, result的字典
         :param charset:
+        :param timeout:
+        :param parse:
         :param kwargs:
             get-params, post-data
         :return:
         '''
         d = {'verify': self.default('ssl_verify'), 'timeout': timeout or self.default('http_timeout'),
              'proxies': self.default('http_proxy')}
         retries = retry or self.default('http_retry')
         d.update(kwargs)
         if not re.search(r'^http', url, re.I) and self.url_root:
             url = re.sub('/*$', '', self.url_root) + '/' + re.sub('^/*', '', url)
         flag = False
         retry_code = retry_code or []
         code_reason = ''
-        for i in range(retry):
+        for i in range(retries):
             try:
-                _raw = self.session.post(url, **d) if method == 'POST' else self.session.get(url, **d)
-                code = _raw.status_code
+                resp = self.session.post(url, **d) if method == 'POST' else self.session.get(url, **d)
+                code = resp.status_code
                 if retry_not_200 and code != 200:
                     code_reason = code
                     continue
                 elif code in retry_code:
                     code_reason = code
                     continue
                 else:
                     flag = True
-                    url = _raw.url
+                    url = resp.url
                     break
             except Exception as e:
                 error = e
         if not flag:
             if code_reason:
                 raise Exception('fetch {} fail, status_code={}. {}'.format(url, code_reason, d))
             else:
                 raise Exception('fetch {} error, {}. {}'.format(url, error, d))
-        if ret_raw:
-            self.fetch_after(_raw, None, None)
-            return {'result': _raw, 'url': url, 'kwargs': d} if ret_dic else _raw
-        if ret_json:
-            return _raw.json()
-        _raw = _raw.content
-        if not charset:
-            m = re.search('charset=\W*(?P<charset>\w+)', _raw[:200].decode(errors='ignore'))
-            charset = m.groupdict().get('charset', 'utf-8') if m else 'utf-8'
-        if charset == 'gb2312':
-            charset = 'cp936'
-        _content = _raw.decode(encoding=charset, errors='ignore')
-        bs = BeautifulSoup(_content, features=self.kwargs.get('features', 'html.parser'))
-        self.fetch_after(_raw, _content, bs)
-        ret = bs if ret_bs else _content
-        return {'result': ret, 'url': url, 'kwargs': d} if ret_dic else ret
+        ret = {'resp': resp, 'url': url, 'kwargs': d, 'method': method}
+        if parse:
+            content = resp.content
+            if not charset:
+                m = re.search('charset=\W*(?P<charset>\w+)', content[:200].decode(errors='ignore'))
+                charset = m.groupdict().get('charset', 'utf-8') if m else 'utf-8'
+            if charset == 'gb2312':
+                charset = 'cp936'
+            _content = content.decode(encoding=charset, errors='ignore')
+            ret['content'] = _content
+            tree = html.fromstring(_content)
+            ret['xpath'] = tree
+            ret['bs'] = BeautifulSoup(_content, features=self.kwargs.get('features', 'html.parser'))
+        self.fetch_after(ret)
+        return ret if ret_dict else resp
 
     def multi_job(self, *args, **kwargs):
         '''
         多进程的job
         :return:
         '''
         return True, self.fetch(*args, **kwargs)
```

### Comparing `seakybox-0.1/seakybox/net/ip.py` & `seakybox-0.2/seakybox/net/ip.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # @Date:   2019/8/20 14:56
 
 import ipaddress
 import re
 
 import IPy
 
-Pattern_IP = '(?P<ip>((25[0-5]|2[0-4]\d|[01]?\d\d?)\.){3}(25[0-5]|2[0-4]\d|[01]?\d\d?))'    # 老版本
+Pattern_IPv4 = '(?P<ip4>((25[0-5]|2[0-4]\d|[01]?\d\d?)\.){3}(25[0-5]|2[0-4]\d|[01]?\d\d?))'    # 老版本
 
 Pattern_IPv4Seg = '(25[0-5]|(2[0-4]|1{0,1}[0-9]){0,1}[0-9])'
 Pattern_IPv4Address = '(?P<ip4>{})'.format('({0}\.){{3,3}}{0}'.format(Pattern_IPv4Seg))
 Pattern_IPv6Seg = '[0-9a-fA-F]{1,4}'
 Pattern_IPv6Address = '(?P<ip6>{})'.format('|'.join([
     '({0}:){{7,7}}{0}'.format(Pattern_IPv6Seg),  # 1:2:3:4:5:6:7:8
     '({0}:){{1,7}}:'.format(Pattern_IPv6Seg),  # 1::                                 1:2:3:4:5:6:7::
```

### Comparing `seakybox-0.1/seakybox/net/proxy.py` & `seakybox-0.2/seakybox/net/proxy.py`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox/net/sserver.py` & `seakybox-0.2/seakybox/net/sserver.py`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox/notify/im.py` & `seakybox-0.2/seakybox/notify/im.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import base64
 import hashlib
 import time
 from functools import partial
 
 import requests
 
-from ..func.misc import fence
+from seakybox.misc.ctf import fence
 
 
 def im(content, url, auth, mode, to, add_time=False, log=None):
     '''
     :param s:
     :param url:
     :param auth:
```

### Comparing `seakybox-0.1/seakybox/notify/sendmail.py` & `seakybox-0.2/seakybox/notify/sendmail.py`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox/os/cmd.py` & `seakybox-0.2/seakybox/os/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,17 +162,17 @@
         if print_error:
             print(p.stdout)
     return parse_execute_sql_result(p, columns_func=columns_func)
 
 
 def parse_execute_sql_result(p, columns_func=None):
     if p.returncode == 0:
-        p.result = []
+        p.account = []
         if p.stdout:
-            p.result.extend(parse_sql_result(p.stdout, columns_func=columns_func))
+            p.account.extend(parse_sql_result(p.stdout, columns_func=columns_func))
     return p
 
 
 def parse_sql_result(s, columns_func=None):
     '''
     解析命令行的sql结果，也可以从文件读取
     :param s:
```

### Comparing `seakybox-0.1/seakybox/os/compress.py` & `seakybox-0.2/seakybox/os/compress.py`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox/os/info.py` & `seakybox-0.2/seakybox/os/info.py`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox/os/oper.py` & `seakybox-0.2/seakybox/os/oper.py`

 * *Files identical despite different names*

### Comparing `seakybox-0.1/seakybox.egg-info/SOURCES.txt` & `seakybox-0.2/seakybox.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,33 +4,40 @@
 seakybox/__init__.py
 seakybox.egg-info/PKG-INFO
 seakybox.egg-info/SOURCES.txt
 seakybox.egg-info/dependency_links.txt
 seakybox.egg-info/requires.txt
 seakybox.egg-info/top_level.txt
 seakybox/data/__init__.py
+seakybox/data/mongo_func.py
 seakybox/data/mysql.py
+seakybox/data/mysql_pd.py
 seakybox/data/pd.py
 seakybox/data/redis_func.py
 seakybox/func/__init__.py
 seakybox/func/base.py
 seakybox/func/interactive.py
 seakybox/func/log.py
-seakybox/func/misc.py
 seakybox/func/mrun.py
+seakybox/func/number.py
 seakybox/func/parser.py
 seakybox/func/string.py
 seakybox/func/time.py
+seakybox/misc/__init__.py
+seakybox/misc/ctf.py
+seakybox/misc/token.py
 seakybox/net/__init__.py
 seakybox/net/connectivity.py
 seakybox/net/http.py
 seakybox/net/ip.py
 seakybox/net/proxy.py
 seakybox/net/sserver.py
 seakybox/notify/__init__.py
+seakybox/notify/dingding.py
+seakybox/notify/ftqq.py
 seakybox/notify/im.py
 seakybox/notify/sendmail.py
 seakybox/os/__init__.py
 seakybox/os/cmd.py
 seakybox/os/compress.py
 seakybox/os/info.py
 seakybox/os/oper.py
```

### Comparing `seakybox-0.1/setup.py` & `seakybox-0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     author_email='seaky.cn@gmail.com',
     description=seakybox.__description__,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sseaky',
     packages=setuptools.find_packages(),
     install_requires=['beautifulsoup4', 'IPy', 'numpy', 'pandas',
-                      'psutil', 'puresnmp', 'PyMySQL', 'requests',
+                      'psutil', 'PyMySQL', 'requests',
                       'SocksiPy-branch', 'sqlacodegen', 'SQLAlchemy', 'sshtunnel',
-                      'urllib3', 'concurrent-log-handler', 'xlrd', 'openpyxl', 'redis'],
+                      'urllib3', 'concurrent-log-handler', 'xlrd', 'openpyxl', 'redis', 'lxml'],
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

