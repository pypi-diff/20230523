# Comparing `tmp/gmsofttest-0.0.4.tar.gz` & `tmp/gmsofttest-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gmsofttest-0.0.4.tar", last modified: Tue May 16 02:50:11 2023, max compression
+gzip compressed data, was "dist\gmsofttest-0.0.5.tar", last modified: Tue May 23 09:22:39 2023, max compression
```

## Comparing `gmsofttest-0.0.4.tar` & `gmsofttest-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      908 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      414 2023-05-16 02:49:52.000000 gmsofttest-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-05-16 02:49:57.000000 gmsofttest-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest/
--rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.4/src/gmsofttest/__init__.py
--rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.4/src/gmsofttest/china_address.py
--rw-rw-rw-   0        0        0      983 2023-05-16 01:57:10.000000 gmsofttest-0.0.4/src/gmsofttest/gm_parse_response.py
--rw-rw-rw-   0        0        0     2137 2023-05-16 01:35:08.000000 gmsofttest-0.0.4/src/gmsofttest/gm_randomdata.py
--rw-rw-rw-   0        0        0    12431 2023-05-16 01:35:08.000000 gmsofttest-0.0.4/src/gmsofttest/gm_sqlconn.py
--rw-rw-rw-   0        0        0     3127 2023-05-16 01:56:18.000000 gmsofttest-0.0.4/src/gmsofttest/gm_timestamp.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest.egg-info/
--rw-rw-rw-   0        0        0      908 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      365 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 02:50:11.000000 gmsofttest-0.0.4/src/gmsofttest.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-23 09:22:39.000000 gmsofttest-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-02-11 08:11:24.000000 gmsofttest-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1180 2023-05-23 09:22:39.000000 gmsofttest-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-05-23 09:14:29.000000 gmsofttest-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 09:22:39.000000 gmsofttest-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      803 2023-05-23 08:37:37.000000 gmsofttest-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:22:39.000000 gmsofttest-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-23 09:22:39.000000 gmsofttest-0.0.5/src/gmsofttest/
+-rw-rw-rw-   0        0        0      125 2023-02-11 07:45:36.000000 gmsofttest-0.0.5/src/gmsofttest/__init__.py
+-rw-rw-rw-   0        0        0    89848 2023-04-22 07:37:37.000000 gmsofttest-0.0.5/src/gmsofttest/china_address.py
+-rw-rw-rw-   0        0        0     2965 2023-05-23 08:08:28.000000 gmsofttest-0.0.5/src/gmsofttest/gm_assert_utils.py
+-rw-rw-rw-   0        0        0     4867 2023-05-23 08:36:05.000000 gmsofttest-0.0.5/src/gmsofttest/gm_excel_utils.py
+-rw-rw-rw-   0        0        0     2576 2023-05-20 08:22:39.000000 gmsofttest-0.0.5/src/gmsofttest/gm_parse_response_utils.py
+-rw-rw-rw-   0        0        0     2197 2023-05-20 08:15:01.000000 gmsofttest-0.0.5/src/gmsofttest/gm_randomdata_utils.py
+-rw-rw-rw-   0        0        0     1800 2023-05-20 08:15:01.000000 gmsofttest-0.0.5/src/gmsofttest/gm_request_utils.py
+-rw-rw-rw-   0        0        0    11797 2023-05-23 08:03:00.000000 gmsofttest-0.0.5/src/gmsofttest/gm_sqlconn_utils.py
+-rw-rw-rw-   0        0        0      877 2023-05-23 08:40:42.000000 gmsofttest-0.0.5/src/gmsofttest/gm_stock_enum.py
+-rw-rw-rw-   0        0        0     3109 2023-05-20 08:15:01.000000 gmsofttest-0.0.5/src/gmsofttest/gm_timestamp_utils.py
+-rw-rw-rw-   0        0        0     2196 2023-05-23 08:01:45.000000 gmsofttest-0.0.5/src/gmsofttest/gm_yaml_process_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-23 09:22:39.000000 gmsofttest-0.0.5/src/gmsofttest.egg-info/
+-rw-rw-rw-   0        0        0     1180 2023-05-23 09:22:38.000000 gmsofttest-0.0.5/src/gmsofttest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2023-05-23 09:22:38.000000 gmsofttest-0.0.5/src/gmsofttest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 09:22:38.000000 gmsofttest-0.0.5/src/gmsofttest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-23 09:22:38.000000 gmsofttest-0.0.5/src/gmsofttest.egg-info/top_level.txt
```

### Comparing `gmsofttest-0.0.4/LICENSE` & `gmsofttest-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.4/setup.py` & `gmsofttest-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="gmsofttest",
-    version="0.0.4",
+    version="0.0.5",
     author="ronaldsu",
     author_email="uph4rmt@dingtalk.com",
     description="大家软件内部测试技术线支撑工具",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.gec123.com",
     project_urls={
@@ -19,8 +19,8 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
-)
+)
```

### Comparing `gmsofttest-0.0.4/src/gmsofttest/china_address.py` & `gmsofttest-0.0.5/src/gmsofttest/china_address.py`

 * *Files identical despite different names*

### Comparing `gmsofttest-0.0.4/src/gmsofttest/gm_randomdata.py` & `gmsofttest-0.0.5/src/gmsofttest/gm_randomdata_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-Name : gm_randomdata.py
+Name : gm_randomdata_utils.py
 Author  : 写上自己的名字
 Contact : 邮箱地址
 Time    : 2023-02-13 10:11
-Desc:
+Desc: 生成随机数据，如手机号、身份证号、企业信息等
 """
 
 """
-Name : generate_basedata.py
-Author  : 写上自己的名字
+Name : gm_randomdata_utils.py
+Author  : 粟飞
 Contact : 邮箱地址
 Time    : 2022-09-01 13:46
 Desc: 生成各种测试数据
 """
 
 from faker import Factory
 import time
```

### Comparing `gmsofttest-0.0.4/src/gmsofttest/gm_sqlconn.py` & `gmsofttest-0.0.5/src/gmsofttest/gm_sqlconn_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Name : gm_sqlconn.py
+Name : gm_sqlconn_utils.py
 Author  : 写上自己的名字
 Contact : 邮箱地址
 Time    : 2021/3/22 15:52
 Desc: 操作MYSQL数据库
 """
 
 
@@ -124,15 +124,14 @@
             print("已创建xcj数据库连接,链接信息{}:{}".format(self.env, self.xcj_port))
             print("已创建内网数据库连接,链接信息{}:{}".format(self.env, self.inner_port))
             print("已创建私有化数据库连接,链接信息{}:{}".format(self.env, self.syh_port))
 
         else:
             print("未获取到env或host参数")
 
-
     def select_first_data(self, sql):
         """
         查询第一条数据
         """
         try:
             # 执行 sql 语句
             if self.host == 'zcj':
@@ -165,15 +164,14 @@
                 self.jydw_cursor = self.jydw_conn.cursor(pymysql.cursors.DictCursor)
                 self.jydw_cursor.execute(sql)
                 first_data = self.jydw_cursor.fetchone()
                 return first_data
         except TypeError as first_data:
             print("SQL执行时类型错误！请检查：{}".format(first_data))
 
-
     def select_all_data(self, sql):
         """
         查询所有数据
         :param sql:
         :return:
         """
         try:
@@ -208,34 +206,14 @@
                 self.jydw_cursor = self.jydw_conn.cursor(pymysql.cursors.DictCursor)
                 self.jydw_cursor.execute(sql)
                 first_data = self.jydw_cursor.fetchall()
                 return first_data
         except TypeError as first_data:
             print("SQL执行时类型错误！请检查：{}".format(first_data))
 
-
-    def select_random_one_data(self, host, sql):
-        """
-        查询第一条数据
-        """
-        try:
-            # 执行 sql 语句
-            if host == 'zcj':
-                self.zcj_cursor.execute(sql)
-                first_data = self.zcj_cursor.fetchone()
-                return first_data
-            elif host == 'xcj':
-                self.xcj_cursor.execute(sql)
-                first_data = self.xcj_cursor.fetchone()
-                return first_data
-        except TypeError as e:
-            print("SQL执行时类型错误！请检查,{}".format(e))
-        except Exception as e:
-            print("执行sql异常:%s" % e)
-
     def delete_data(self, host, sql):
         """
         查询所有数据
         :param host:  zcj、xcj
         :param sql: SQL查询
         :return:
         """
@@ -245,20 +223,20 @@
                 self.zcj_cursor.commit()
             elif host == 'xcj':
                 self.xcj_cursor.execute(sql)
                 self.xcj_cursor.commit()
 
         except TypeError as e1:
             print("SQL执行时类型错误！请检查" % e1)
-            self.zcj_cursor.rollback()
-            self.xcj_cursor.rollback()
+            self.zcj_cursor.rollback()  # 回滚操作
+            self.xcj_cursor.rollback()  # 回滚操作
         except Exception as e2:
             print("执行sql异常:%s" % e2)
-            self.zcj_cursor.rollback()
-            self.xcj_cursor.rollback()
+            self.zcj_cursor.rollback()  # 回滚操作
+            self.xcj_cursor.rollback()  # 回滚操作
 
     def conn_close(self):
         # 关闭数据库连接
         try:
             self.xcj_conn.close()
             self.zcj_conn.close()
             self.jydn_conn.close()
@@ -269,19 +247,19 @@
             self.xcj_cursor.close()
             self.zcj_cursor.close()
             self.jydn_cursor.close()
             self.jydw_cursor.close()
             self.syh_cursor.close()
             self.inner_cursor.close()
         except AttributeError as e:
-            print("数据库连接已关闭, {} ".format(e))
+            print("数据库连接已关闭!!!")
 
 
 if __name__ == "__main__":
-    # ()类的实例化
+    # 生成类实例对象
     om = OperateMysql('show', 'zcj')
-    # # 查询征集服务的所有已提交申请
-    #
+    # 执行sql
     a = om.select_all_data("SELECT count(*) FROM `zcj_openbid`.`e_openbid_package` where anoteno like '%CQS%'")
     #
     print(a)
+    # 关闭数据库连接
     om.conn_close()
```

### Comparing `gmsofttest-0.0.4/src/gmsofttest/gm_timestamp.py` & `gmsofttest-0.0.5/src/gmsofttest/gm_timestamp_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-Name : gm_timestamp.py
+Name : gm_timestamp_utils.py
 Author  : 写上自己的名字
 Contact : 邮箱地址
 Time    : 2023-05-16 9:45
 Desc:
 """
 
 """
 Name : timestamphandler.py
 Author  : 写上自己的名字
 Contact : 邮箱地址
 Time    : 2021/3/25 10:27
-Desc: 根据调用时间，生成时间戳，精确到毫秒，用于生成文件名
+Desc: 根据调用时间，生成时间戳，精确到毫秒
 """
 
 # 年-月-日 时:分:秒
 import datetime
 import time
 
 nowTime = datetime.datetime.now().strftime('%Y-%m-%d %H:%M:%S')
```

