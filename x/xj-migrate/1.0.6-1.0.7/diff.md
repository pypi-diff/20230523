# Comparing `tmp/xj-migrate-1.0.6.tar.gz` & `tmp/xj-migrate-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\xj-migrate-1.0.6.tar", last modified: Tue Dec 13 06:38:43 2022, max compression
+gzip compressed data, was "dist\xj-migrate-1.0.7.tar", last modified: Wed Jan 11 06:00:35 2023, max compression
```

## Comparing `xj-migrate-1.0.6.tar` & `xj-migrate-1.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/
--rw-rw-rw-   0        0        0     1438 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      946 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/README.md
--rw-rw-rw-   0        0        0       42 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     2016 2022-12-13 06:38:29.000000 xj-migrate-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/xj_migrate/
--rw-rw-rw-   0        0        0        0 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/__init__.py
--rw-rw-rw-   0        0        0       83 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/admin.py
-drwxrwxrwx   0        0        0        0 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/xj_migrate/apis/
--rw-rw-rw-   0        0        0        0 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/apis/__init__.py
--rw-rw-rw-   0        0        0     1384 2022-12-13 06:16:46.000000 xj-migrate-1.0.6/xj_migrate/apis/data_excel.py
--rw-rw-rw-   0        0        0     3166 2022-12-13 06:16:46.000000 xj-migrate-1.0.6/xj_migrate/apis/data_migration.py
--rw-rw-rw-   0        0        0     2700 2022-12-13 06:06:27.000000 xj-migrate-1.0.6/xj_migrate/apis/export_api.py
--rw-rw-rw-   0        0        0     1017 2022-12-13 06:17:12.000000 xj-migrate-1.0.6/xj_migrate/apis/migrate_foreign_key_mapping.py
--rw-rw-rw-   0        0        0      964 2022-12-13 06:17:21.000000 xj-migrate-1.0.6/xj_migrate/apis/migrate_platfrom.py
--rw-rw-rw-   0        0        0      212 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/apps.py
--rw-rw-rw-   0        0        0     1675 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/common.py
--rw-rw-rw-   0        0        0     3010 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/models.py
-drwxrwxrwx   0        0        0        0 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/xj_migrate/services/
--rw-rw-rw-   0        0        0     4946 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/services/DataConsolidation.py
--rw-rw-rw-   0        0        0        0 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/services/__init__.py
--rw-rw-rw-   0        0        0     5306 2022-12-13 06:17:50.000000 xj-migrate-1.0.6/xj_migrate/services/data_execl_service.py
--rw-rw-rw-   0        0        0     3268 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/services/data_execl_service2.py
--rw-rw-rw-   0        0        0     1618 2022-12-13 06:15:11.000000 xj-migrate-1.0.6/xj_migrate/services/doc_export_service.py
--rw-rw-rw-   0        0        0    10525 2022-11-23 10:54:27.000000 xj-migrate-1.0.6/xj_migrate/services/excel_export_service.py
--rw-rw-rw-   0        0        0     4809 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/services/mapping_process.py
--rw-rw-rw-   0        0        0     1371 2022-12-13 06:18:48.000000 xj-migrate-1.0.6/xj_migrate/services/migrate_foregin_key_mapping_service.py
--rw-rw-rw-   0        0        0      785 2022-12-13 06:18:51.000000 xj-migrate-1.0.6/xj_migrate/services/migrate_platfrom_service.py
--rw-rw-rw-   0        0        0     1056 2022-11-23 10:49:43.000000 xj-migrate-1.0.6/xj_migrate/urls.py
-drwxrwxrwx   0        0        0        0 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/xj_migrate/utils/
--rw-rw-rw-   0        0        0        0 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/utils/__init__.py
--rw-rw-rw-   0        0        0     1661 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/utils/common.py
--rw-rw-rw-   0        0        0     1084 2022-12-13 01:22:36.000000 xj-migrate-1.0.6/xj_migrate/utils/custom_authorization.py
--rw-rw-rw-   0        0        0     1948 2022-11-23 10:48:23.000000 xj-migrate-1.0.6/xj_migrate/utils/custom_response.py
--rw-rw-rw-   0        0        0     7806 2022-10-31 08:53:23.000000 xj-migrate-1.0.6/xj_migrate/utils/custom_tool.py
--rw-rw-rw-   0        0        0     2075 2022-09-08 09:31:24.000000 xj-migrate-1.0.6/xj_migrate/utils/digit_algorithm.py
--rw-rw-rw-   0        0        0      981 2022-11-23 09:18:07.000000 xj-migrate-1.0.6/xj_migrate/utils/jconfig.py
--rw-rw-rw-   0        0        0     7314 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/utils/model_handle.py
--rw-rw-rw-   0        0        0     7599 2022-11-23 08:50:23.000000 xj-migrate-1.0.6/xj_migrate/utils/unionpay_utils.py
--rw-rw-rw-   0        0        0     4192 2022-12-13 01:22:36.000000 xj-migrate-1.0.6/xj_migrate/utils/user_wrapper.py
-drwxrwxrwx   0        0        0        0 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/xj_migrate.egg-info/
--rw-rw-rw-   0        0        0     1438 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/xj_migrate.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1235 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/xj_migrate.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/xj_migrate.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/xj_migrate.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-12-13 06:38:43.000000 xj-migrate-1.0.6/xj_migrate.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-01-11 06:00:35.000000 xj-migrate-1.0.7/
+-rw-rw-rw-   0        0        0     1438 2023-01-11 06:00:35.000000 xj-migrate-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      946 2022-09-19 09:25:05.000000 xj-migrate-1.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-01-11 06:00:35.000000 xj-migrate-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     2016 2023-01-11 05:35:12.000000 xj-migrate-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-01-11 06:00:34.000000 xj-migrate-1.0.7/xj_migrate/
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj-migrate-1.0.7/xj_migrate/__init__.py
+-rw-rw-rw-   0        0        0       83 2022-09-07 08:56:08.000000 xj-migrate-1.0.7/xj_migrate/admin.py
+drwxrwxrwx   0        0        0        0 2023-01-11 06:00:34.000000 xj-migrate-1.0.7/xj_migrate/apis/
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj-migrate-1.0.7/xj_migrate/apis/__init__.py
+-rw-rw-rw-   0        0        0     1913 2023-01-10 07:11:28.000000 xj-migrate-1.0.7/xj_migrate/apis/data_excel.py
+-rw-rw-rw-   0        0        0     3166 2022-12-16 01:37:09.000000 xj-migrate-1.0.7/xj_migrate/apis/data_migration.py
+-rw-rw-rw-   0        0        0     2701 2022-12-16 01:55:27.000000 xj-migrate-1.0.7/xj_migrate/apis/export_api.py
+-rw-rw-rw-   0        0        0     1017 2022-12-16 01:37:09.000000 xj-migrate-1.0.7/xj_migrate/apis/migrate_foreign_key_mapping.py
+-rw-rw-rw-   0        0        0      964 2022-12-16 01:37:09.000000 xj-migrate-1.0.7/xj_migrate/apis/migrate_platfrom.py
+-rw-rw-rw-   0        0        0      212 2022-09-09 02:14:57.000000 xj-migrate-1.0.7/xj_migrate/apps.py
+-rw-rw-rw-   0        0        0     1675 2022-08-29 03:39:13.000000 xj-migrate-1.0.7/xj_migrate/common.py
+-rw-rw-rw-   0        0        0     3010 2022-09-16 08:44:58.000000 xj-migrate-1.0.7/xj_migrate/models.py
+drwxrwxrwx   0        0        0        0 2023-01-11 06:00:34.000000 xj-migrate-1.0.7/xj_migrate/services/
+-rw-rw-rw-   0        0        0     4946 2022-09-07 08:51:41.000000 xj-migrate-1.0.7/xj_migrate/services/DataConsolidation.py
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj-migrate-1.0.7/xj_migrate/services/__init__.py
+-rw-rw-rw-   0        0        0     8257 2023-01-10 07:26:10.000000 xj-migrate-1.0.7/xj_migrate/services/data_execl_service.py
+-rw-rw-rw-   0        0        0     3268 2022-09-15 07:58:46.000000 xj-migrate-1.0.7/xj_migrate/services/data_execl_service2.py
+-rw-rw-rw-   0        0        0     1618 2022-12-16 01:37:09.000000 xj-migrate-1.0.7/xj_migrate/services/doc_export_service.py
+-rw-rw-rw-   0        0        0    10525 2022-12-08 07:39:45.000000 xj-migrate-1.0.7/xj_migrate/services/excel_export_service.py
+-rw-rw-rw-   0        0        0     4809 2022-09-19 02:59:53.000000 xj-migrate-1.0.7/xj_migrate/services/mapping_process.py
+-rw-rw-rw-   0        0        0     1371 2022-12-16 01:37:09.000000 xj-migrate-1.0.7/xj_migrate/services/migrate_foregin_key_mapping_service.py
+-rw-rw-rw-   0        0        0      785 2022-12-16 01:37:09.000000 xj-migrate-1.0.7/xj_migrate/services/migrate_platfrom_service.py
+-rw-rw-rw-   0        0        0     1122 2023-01-10 01:57:48.000000 xj-migrate-1.0.7/xj_migrate/urls.py
+drwxrwxrwx   0        0        0        0 2023-01-11 06:00:35.000000 xj-migrate-1.0.7/xj_migrate/utils/
+-rw-rw-rw-   0        0        0        0 2022-08-26 02:08:41.000000 xj-migrate-1.0.7/xj_migrate/utils/__init__.py
+-rw-rw-rw-   0        0        0     1661 2022-08-26 02:08:41.000000 xj-migrate-1.0.7/xj_migrate/utils/common.py
+-rw-rw-rw-   0        0        0     1084 2022-12-16 01:37:09.000000 xj-migrate-1.0.7/xj_migrate/utils/custom_authorization.py
+-rw-rw-rw-   0        0        0     1948 2022-12-08 07:39:45.000000 xj-migrate-1.0.7/xj_migrate/utils/custom_response.py
+-rw-rw-rw-   0        0        0     7806 2022-12-08 07:39:45.000000 xj-migrate-1.0.7/xj_migrate/utils/custom_tool.py
+-rw-rw-rw-   0        0        0     2075 2022-12-08 07:39:45.000000 xj-migrate-1.0.7/xj_migrate/utils/digit_algorithm.py
+-rw-rw-rw-   0        0        0      981 2022-12-08 07:39:45.000000 xj-migrate-1.0.7/xj_migrate/utils/jconfig.py
+-rw-rw-rw-   0        0        0     7314 2022-08-22 01:46:29.000000 xj-migrate-1.0.7/xj_migrate/utils/model_handle.py
+-rw-rw-rw-   0        0        0     7599 2022-09-05 06:52:36.000000 xj-migrate-1.0.7/xj_migrate/utils/unionpay_utils.py
+-rw-rw-rw-   0        0        0     4192 2022-12-16 01:37:09.000000 xj-migrate-1.0.7/xj_migrate/utils/user_wrapper.py
+drwxrwxrwx   0        0        0        0 2023-01-11 06:00:34.000000 xj-migrate-1.0.7/xj_migrate.egg-info/
+-rw-rw-rw-   0        0        0     1438 2023-01-11 06:00:34.000000 xj-migrate-1.0.7/xj_migrate.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1235 2023-01-11 06:00:34.000000 xj-migrate-1.0.7/xj_migrate.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-01-11 06:00:34.000000 xj-migrate-1.0.7/xj_migrate.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-01-11 06:00:34.000000 xj-migrate-1.0.7/xj_migrate.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-01-11 06:00:34.000000 xj-migrate-1.0.7/xj_migrate.egg-info/top_level.txt
```

### Comparing `xj-migrate-1.0.6/PKG-INFO` & `xj-migrate-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-migrate
-Version: 1.0.6
+Version: 1.0.7
 Summary: 迁移模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # xj_migrate
         
         #### 介绍
         迁移模块
```

### Comparing `xj-migrate-1.0.6/README.md` & `xj-migrate-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/setup.py` & `xj-migrate-1.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf8') as fp:
     log_desc = fp.read()
 
 setup(
     name='xj-migrate',  # 模块名称
-    version='1.0.6',  # 模块版本
+    version='1.0.7',  # 模块版本
     description='迁移模块',  # 项目 摘要描述
     long_description=log_desc,  # 项目描述
     long_description_content_type="text/markdown",  # md文件，markdown格式
     packages=find_packages(),  # 系统自动从当前目录开始找包
     # packages=['xj_migrate'],  # 系指定安装模块
     license="apache 3.0",
     install_requires=[
```

### Comparing `xj-migrate-1.0.6/xj_migrate/apis/data_excel.py` & `xj-migrate-1.0.7/xj_migrate/apis/data_excel.py`

 * *Files 22% similar despite different names*

```diff
@@ -27,7 +27,18 @@
         old_table_id = self.POST.get('old_table_id')
         new_table_id = self.POST.get('new_table_id')
         data, err_txt = DataExeclService.data_migrate(filename, configure, export_field, old_table_id,
                                                       new_table_id)
         if not err_txt:
             return util_response(data=data)
         return util_response(err=47767, msg=err_txt)
+
+    def data_cover(self):
+        filename = self.POST.get('filename')  # 文件路径
+        table_name = self.POST.get('table_name')
+        configure = self.POST.get('configure')
+        cover_where = self.POST.get('cover_where')
+        cover_field = self.POST.get('cover_field')
+        data, err_txt = DataExeclService.data_cover(filename, configure, table_name, cover_where, cover_field)
+        if not err_txt:
+            return util_response(data=data)
+        return util_response(err=47767, msg=err_txt)
```

### Comparing `xj-migrate-1.0.6/xj_migrate/apis/data_migration.py` & `xj-migrate-1.0.7/xj_migrate/apis/data_migration.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/apis/export_api.py` & `xj-migrate-1.0.7/xj_migrate/apis/export_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         # print("request_params:", request_params)
         data, export_err = DocExportService.export(request_params, templet_path=TEMPLET_PATH_MAP.get(templet_path_name))
         if not export_err is None:
             return util_response(err=1003, msg=export_err)
         return doc_response(data)
 
     @request_params_wrapper
-    def excel_export(self, request_params, *args, **kwargs):
+    def  excel_export(self, request_params, *args, **kwargs):
         templet_path = MEDIA_ROOT + "/templet/test.xls"
         print(templet_path)
         print("request_params", request_params)
         export_instance = ExcelExport(excel_templet_path=templet_path)
         # 写入
         data, err = export_instance.additional_write(input_dict=[request_params])
         # 保存
```

### Comparing `xj-migrate-1.0.6/xj_migrate/apis/migrate_foreign_key_mapping.py` & `xj-migrate-1.0.7/xj_migrate/apis/migrate_foreign_key_mapping.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/apis/migrate_platfrom.py` & `xj-migrate-1.0.7/xj_migrate/apis/migrate_platfrom.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/common.py` & `xj-migrate-1.0.7/xj_migrate/common.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/models.py` & `xj-migrate-1.0.7/xj_migrate/models.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/services/DataConsolidation.py` & `xj-migrate-1.0.7/xj_migrate/services/DataConsolidation.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/services/data_execl_service.py` & `xj-migrate-1.0.7/xj_migrate/services/data_execl_service.py`

 * *Files 22% similar despite different names*

```diff
@@ -74,14 +74,15 @@
             return None, "目标数据库连接失败"
         conn = target_db.cursor()
         where = "id = " + new_table_id
         table_name_sql = "SELECT `table_name` FROM migrate_platform_table WHERE {};".format(where)
         conn.execute(table_name_sql)
         table_name = conn.fetchone()
         data = DataExeclService.excl_import(json.dumps(configure), table_name[0], file_path)
+        print(data)
         import_data = data[0]["list"]
         # 连接目标数据库
         try:
             num = 0
             for dict in import_data:
                 # row = tuple(i)
                 if "id" in dict.keys():
@@ -113,10 +114,78 @@
 
                 num = num + 1
         except Exception as e:
             return None, e
         target_db.commit()
         conn.close()
         data = {
-            # "rows": num
+            "rows": num
+        }
+        return data, None
+
+    @staticmethod
+    def data_cover(file_path, configure, table_name, cover_where, cover_field):
+        configure = json.loads(configure)  # 连接数据库配置
+        try:
+            target_db = pymysql.connect(
+                host=configure['localhost'],
+                port=int(configure['port']),
+                user=configure['username'],
+                password=configure['password'],
+                db=configure['database'],
+                charset="utf8",
+            )
+        except Exception as err:
+            return None, "目标数据库连接失败"
+        conn = target_db.cursor()
+        readboot = xlrd.open_workbook(file_path)
+        sheet = readboot.sheet_by_index(0)
+        # # 获取excel的行和列
+        nrows = sheet.nrows  # 行
+        ncols = sheet.ncols  # 列
+        first_row_values = sheet.row_values(0)  # 第一行数据
+        list = []
+        try:
+            num = 0
+            for row_num in range(1, nrows):
+                row_values = sheet.row_values(row_num)
+                if row_values:
+                    str_obj = {}
+                for i in range(len(first_row_values)):
+                    ctype = sheet.cell(num, i).ctype
+                    cell = sheet.cell_value(num, i)
+                    if ctype == 2 and cell % 1 == 0.0:  # ctype为2且为浮点
+                        cell = int(cell)  # 浮点转成整型
+                        cell = str(cell)  # 转成整型后再转成字符串，如果想要整型就去掉该行
+                    elif ctype == 3:
+                        date = datetime(*xldate_as_tuple(cell, 0))
+                        cell = date.strftime('%Y/%m/%d %H:%M:%S')
+                    elif ctype == 4:
+                        cell = True if cell == 1 else False
+                    str_obj[first_row_values[i]] = cell
+                list.append(str_obj)
+                num = num + 1
+            # print(list)
+
+            for dict in list:
+                where = cover_where + "=" + "'" + dict[cover_where] + "'"
+                li = []
+                for i in cover_field.split(","):
+                    if len(dict[i]) > 0:
+                        update = i + "=" + "'" + dict[i] + "'"
+                    else:
+                        update = i + "=" + "''"
+                    li.append(update)
+                str1 = ','.join(li)
+                sql = "UPDATE `{}` SET {} WHERE {};".format(table_name, str1, where)
+                sql = sql.replace("''", "NULL").replace("''", "NULL")  # 处理空数据
+                sql = sql.replace("'{}'", "NULL").replace("'{}'", "NULL")  # 处理空json
+                # print(sql)
+                conn.execute(sql)
+        except Exception as e:
+            return None, e
+        target_db.commit()
+        conn.close()
+        data = {
+            "rows": num
         }
         return data, None
```

### Comparing `xj-migrate-1.0.6/xj_migrate/services/data_execl_service2.py` & `xj-migrate-1.0.7/xj_migrate/services/data_execl_service2.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/services/doc_export_service.py` & `xj-migrate-1.0.7/xj_migrate/services/doc_export_service.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/services/excel_export_service.py` & `xj-migrate-1.0.7/xj_migrate/services/excel_export_service.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/services/mapping_process.py` & `xj-migrate-1.0.7/xj_migrate/services/mapping_process.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/services/migrate_foregin_key_mapping_service.py` & `xj-migrate-1.0.7/xj_migrate/services/migrate_foregin_key_mapping_service.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/services/migrate_platfrom_service.py` & `xj-migrate-1.0.7/xj_migrate/services/migrate_platfrom_service.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/urls.py` & `xj-migrate-1.0.7/xj_migrate/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 urlpatterns = [
 
     re_path(r'^list_table/?$', data_migration.DataMigration.list_table),
     re_path(r'^list_col/?$', data_migration.DataMigration.list_col),
     re_path(r'^consolidation/?$', data_migration.DataMigration.consolidation),
     re_path(r'^data_proving/?$', data_excel.DataExcel.data_proving),
     re_path(r'^data_match_write/?$', data_excel.DataExcel.data_match_write),
+    re_path(r'^data_cover/?$', data_excel.DataExcel.data_cover),
     re_path(r'^mapping_rocessing/?$', data_migration.DataMigration.mapping_rocessing),
     re_path(r'^platform/?$', migrate_platfrom.MigratePlatfrom.as_view()),  # 迁移平台
     re_path(r'^foreign_key_mapping/?$', migrate_foreign_key_mapping.MigrateForeignKeyMapping.as_view()),  # 外键映射
     re_path(r'^doc_export/?$', export_api.exportAPIView.doc_export),  # 外键映射
     re_path(r'^excel_export/?$', export_api.exportAPIView.excel_export),  # 外键映射
 
 ]
```

### Comparing `xj-migrate-1.0.6/xj_migrate/utils/common.py` & `xj-migrate-1.0.7/xj_migrate/utils/common.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/utils/custom_authorization.py` & `xj-migrate-1.0.7/xj_migrate/utils/custom_authorization.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/utils/custom_response.py` & `xj-migrate-1.0.7/xj_migrate/utils/custom_response.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/utils/custom_tool.py` & `xj-migrate-1.0.7/xj_migrate/utils/custom_tool.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/utils/digit_algorithm.py` & `xj-migrate-1.0.7/xj_migrate/utils/digit_algorithm.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/utils/jconfig.py` & `xj-migrate-1.0.7/xj_migrate/utils/jconfig.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/utils/model_handle.py` & `xj-migrate-1.0.7/xj_migrate/utils/model_handle.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/utils/unionpay_utils.py` & `xj-migrate-1.0.7/xj_migrate/utils/unionpay_utils.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate/utils/user_wrapper.py` & `xj-migrate-1.0.7/xj_migrate/utils/user_wrapper.py`

 * *Files identical despite different names*

### Comparing `xj-migrate-1.0.6/xj_migrate.egg-info/PKG-INFO` & `xj-migrate-1.0.7/xj_migrate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xj-migrate
-Version: 1.0.6
+Version: 1.0.7
 Summary: 迁移模块
 Home-page: UNKNOWN
 License: apache 3.0
 Description: # xj_migrate
         
         #### 介绍
         迁移模块
```

### Comparing `xj-migrate-1.0.6/xj_migrate.egg-info/SOURCES.txt` & `xj-migrate-1.0.7/xj_migrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

