# Comparing `tmp/smartis_sdk-0.6.1.tar.gz` & `tmp/smartis_sdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartis_sdk-0.6.1.tar", max compression
+gzip compressed data, was "smartis_sdk-0.7.0.tar", max compression
```

## Comparing `smartis_sdk-0.6.1.tar` & `smartis_sdk-0.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1070 2023-05-11 10:40:57.750065 smartis_sdk-0.6.1/LICENSE
--rw-r--r--   0        0        0      155 2023-05-19 21:54:47.093789 smartis_sdk-0.6.1/README.md
--rw-r--r--   0        0        0     1190 2023-05-20 07:21:33.645432 smartis_sdk-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      385 2023-05-19 21:54:47.097123 smartis_sdk-0.6.1/src/smartis_sdk/__init__.py
--rw-r--r--   0        0        0     7299 2023-05-20 07:26:33.284017 smartis_sdk-0.6.1/src/smartis_sdk/client.py
--rw-r--r--   0        0        0     2389 2023-05-19 21:54:47.097123 smartis_sdk-0.6.1/src/smartis_sdk/common.py
--rw-r--r--   0        0        0     3899 2023-05-19 21:54:47.097123 smartis_sdk-0.6.1/src/smartis_sdk/entity.py
--rw-r--r--   0        0        0      279 2023-05-19 21:54:47.097123 smartis_sdk-0.6.1/src/smartis_sdk/errors.py
--rw-r--r--   0        0        0     1400 2023-05-20 06:41:12.014640 smartis_sdk-0.6.1/src/smartis_sdk/utils.py
--rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 smartis_sdk-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-21 17:18:33.271757 smartis_sdk-0.7.0/LICENSE
+-rw-r--r--   0        0        0      155 2023-05-21 17:18:33.271757 smartis_sdk-0.7.0/README.md
+-rw-r--r--   0        0        0     1213 2023-05-22 19:09:51.870572 smartis_sdk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      385 2023-05-21 17:18:33.275090 smartis_sdk-0.7.0/src/smartis_sdk/__init__.py
+-rw-r--r--   0        0        0     6998 2023-05-22 19:15:19.713410 smartis_sdk-0.7.0/src/smartis_sdk/client.py
+-rw-r--r--   0        0        0     2387 2023-05-22 18:45:25.962377 smartis_sdk-0.7.0/src/smartis_sdk/common.py
+-rw-r--r--   0        0        0     4323 2023-05-22 18:27:38.495638 smartis_sdk-0.7.0/src/smartis_sdk/entity.py
+-rw-r--r--   0        0        0      506 2023-05-22 07:06:09.674697 smartis_sdk-0.7.0/src/smartis_sdk/errors.py
+-rw-r--r--   0        0        0     1400 2023-05-21 17:18:33.275090 smartis_sdk-0.7.0/src/smartis_sdk/utils.py
+-rw-r--r--   0        0        0      672 1970-01-01 00:00:00.000000 smartis_sdk-0.7.0/PKG-INFO
```

### Comparing `smartis_sdk-0.6.1/LICENSE` & `smartis_sdk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.6.1/pyproject.toml` & `smartis_sdk-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartis_sdk"
-version = "0.6.1"
+version = "0.7.0"
 description = "SDK для Smartis API"
 license = "MIT"
 authors = ["viktor <vi.dave@yandex.ru>"]
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
@@ -21,15 +21,15 @@
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 120
 
 # Enable Pyflakes `E` and `F` codes by default.
-select = ["E", "F", "UP", "ANN", "B"]
+select = ["E", "F", "UP", "ANN", "B", "W","S", "BLE", "RUF"]
 ignore = ["E501", "ANN204", "ANN101"]
 
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
```

### Comparing `smartis_sdk-0.6.1/src/smartis_sdk/client.py` & `smartis_sdk-0.7.0/src/smartis_sdk/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,54 @@
-"""Дополнительные методы Smartis API"""
 import json
 import time
 from enum import Enum
 
 import requests
-from pydantic import ValidationError, BaseModel
+from pydantic import ValidationError
 
-from .entity import Ads, Ad, Payload, CrmCustomFields, CrmCustomField, CrmCustomFieldGroups
+from .entity import Ads, Ad, Payload, CrmCustomFields, CrmCustomField, CrmCustomFieldGroups, Keyword
+from .entity import FieldsRootEntity, FieldsEntity, RootEntity, Entity
 from .entity import Campaigns, Campaign
 from .entity import Channels, Placements
-from .entity import Keywords, Keyword
+from .entity import Keywords
 from .common import Method
-from .errors import ApiLimitError
+from .errors import ApiLimitError, ApiInternalError
 import logging
 
 from .utils import clean_column_ids, ColumnType
 
 
 class ContentType(Enum):
     application = "application/json"
 
 
-def status_code_handler(response: requests.Response, retry: int) -> None:
-    """Обработка статус кодов"""
+def status_code_handler(response: requests.Response) -> None:
+    """Status code preprocessing"""
 
     match response.status_code:
         case 200:
             return
         case 400 | 403:
             resp_body: dict = response.json()
             message = resp_body.get("error")
             raise ConnectionError(f"{response.status_code}:{response.text}. details: {message}")
         case 429:
             if int(response.headers['X-Ratelimit-Remaining']) == 0:
                 logging.warning(f"Status code: {response.status_code}. "
-                                f"Причина: {response.reason}. "
-                                f"Пауза: {response.headers['Retry-After']} с.")
+                                f"Reason: {response.reason}. "
+                                f"Retry after: {response.headers['Retry-After']} sec.")
                 raise ApiLimitError(int(response.headers['Retry-After']), response.text)
         case 500 | 502:
             logging.warning(f"Status code: {response.status_code}. "
-                            f"Причина: {response.reason}. "
-                            f"Пауза: 60 с.")
-            time.sleep(60)
+                            f"Reason: {response.reason}")
+            raise ApiInternalError(response.text)
         case _:
-            logging.warning(f" Необработанное исключение. "
+            logging.warning(f" Unknown exception. "
                             f"Status code: {response.status_code}. "
-                            f"Причина: {response.reason}. ")
+                            f"Reason: {response.reason}. ")
             logging.info(response.headers)
             time.sleep(60)
 
 
 class Client:
     TRY_REQUEST = 10
     REQUEST_PAUSE = 1
@@ -62,111 +61,103 @@
         if dev:
             self.host = "https://dev.smartis.bi/api/"
         else:
             self.host = "https://my.smartis.bi/api/"
 
     def get_other(self, method: Method) -> []:
         response = self._prepare(method)
+        status_code_handler(response)
         return response.json()[method.value.location]
 
     def _prepare(self, method: Method, parameters: str | None = None) -> requests.Response:
         if parameters:
             resp = requests.post(f"{self.host}{method.value.method}", headers=self.header, data=parameters)
         else:
             resp = requests.post(f"{self.host}{method.value.method}", headers=self.header)
-
-        if resp.status_code != 200:
-            raise ConnectionError(f"{resp.status_code} {resp.reason}")
+        status_code_handler(resp)
 
         return resp
 
     def get_channels(self) -> Channels:
-        response = self._prepare(Method.get_channels)
+        response = self._prepare(Method.GET_CHANNELS)
         try:
             return Channels.model_validate(response.json())
         except ValidationError as e:
             raise ValueError from e
 
     def get_placements(self) -> Placements:
-        response = self._prepare(Method.get_placements)
+        response = self._prepare(Method.GET_PLACEMENTS)
         try:
             return Placements.model_validate(response.json())
         except ValidationError as e:
             raise ValueError from e
 
-    def get_campaigns(self, campaigns_ids: list) -> list[Campaign]:
-        all_campaigns: list[Campaign] = []
-        items: Campaigns = self._get_entity(campaigns_ids, Method.get_campaigns, Campaigns)
-        all_campaigns.extend(items.items)
-        return all_campaigns
-
-    def get_ads(self, ads_ids: list) -> list[Ad]:
-        all_ads: list[Ad] = []
-        items: Ads = self._get_entity(ads_ids, Method.get_ads, Ads)
-        all_ads.extend(items.items)
-        return all_ads
-
-    def _get_entity(self, ids: list, method: Method, model: BaseModel) -> BaseModel:
+    def _get_entity(self, ids: list, method: Method,
+                    model: type[RootEntity] | type[FieldsRootEntity]) -> RootEntity | FieldsRootEntity:
         params = {"ids": ids}
-        if method in [Method.get_crm_custom_fields, Method.get_crm_custom_field_groups]:
+        if method in [Method.GET_CRM_CUSTOM_FIELDS, Method.GET_CRM_CUSTOM_FIELD_GROUPS]:
             params["smartis_crm_token"] = self.crm_token
         params_json = json.dumps(params)
         response = self._prepare(method, parameters=params_json)
-        if response.status_code != 200:
-            raise ConnectionError(f"status code: {str(response.status_code)}")
+        status_code_handler(response)
         try:
             return model.model_validate(response.json())
         except ValidationError as e:
             raise ValueError from e
 
+    def get_campaigns(self, campaigns_ids: list) -> list[Campaign]:
+        items: RootEntity = self._get_entity(campaigns_ids, Method.GET_CAMPAIGNS, Campaigns)
+        return items.items
+
+    def get_ads(self, ads_ids: list) -> list[Ad]:
+        items: RootEntity = self._get_entity(ads_ids, Method.GET_ADS, Ads)
+        return items.items
+
     def get_keywords(self, keywords_ids: list) -> list[Keyword]:
-        all_keywords: list[Keyword] = []
-        items: Keywords = self._get_entity(keywords_ids, Method.get_keywords, Keywords)
-        all_keywords.extend(items.items)
-        return all_keywords
+        items: RootEntity = self._get_entity(keywords_ids, Method.GET_KEYWORDS, Keywords)
+        return items.items
 
-    def get_crm_custom_fields(self, fields_ids: list) -> list[CrmCustomField]:
+    def _get_fields(self, method: Method, model: type[FieldsRootEntity], fields_ids: list) -> list[FieldsEntity]:
         if self.crm_token is None:
             raise ValueError("Not found crm token")
         fields_ids = clean_column_ids(fields_ids, ColumnType.CustomField)
-        all_fields: list[CrmCustomField] = []
-        items: CrmCustomFields = self._get_entity(fields_ids, Method.get_crm_custom_fields, CrmCustomFields)
-        all_fields.extend(items.items)
-        return all_fields
+        return self._get_entity(fields_ids, method, model).items
 
-    def get_crm_custom_field_groups(self, fields_ids: list) -> list[CrmCustomField]:
-        if self.crm_token is None:
-            raise ValueError("Not found crm token")
-        fields_ids = clean_column_ids(fields_ids, ColumnType.CustomFieldGroup)
-        all_fields: list[CrmCustomField] = []
-        items: CrmCustomFields = self._get_entity(fields_ids, Method.get_crm_custom_field_groups, CrmCustomFieldGroups)
-        all_fields.extend(items.items)
-        return all_fields
+    def get_crm_custom_fields(self, fields_ids: list) -> list[CrmCustomField]:
+        return self._get_fields(Method.GET_CRM_CUSTOM_FIELDS, CrmCustomFields, fields_ids)
+
+    def get_crm_custom_field_groups(self, fields_ids: list) -> list[CrmCustomFieldGroups]:
+        return self._get_fields(Method.GET_CRM_CUSTOM_FIELD_GROUPS, CrmCustomFieldGroups, fields_ids)
 
     def get_report(self, payload: Payload, retry: int = TRY_REQUEST) -> requests.Response:
-        """Выполнение запросов с обработкой ошибок"""
         payload_json = payload.to_json()
         try:
             time.sleep(self.REQUEST_PAUSE)
             answer = requests.post(f"{self.host}reports/getReport", headers=self.header, data=payload_json)
-            status_code_handler(answer, self.TRY_REQUEST)
-        except ApiLimitError as apiErr:
+            status_code_handler(answer)
+        except ApiLimitError as apiLimErr:
             if retry == 0:
                 return self.retry_get_report(payload)
-            logging.warning(f"error: {apiErr.message}")
+            logging.warning(f"error: {apiLimErr.message}")
+            logging.info(
+                f"Retry after {apiLimErr.retry_after} sec.: {self.TRY_REQUEST - retry + 1}/{self.TRY_REQUEST}")
+            time.sleep(apiLimErr.retry_after)
+            return self.get_report(payload, retry=retry - 1)
+        except ApiInternalError as apiIntErr:
+            if retry == 0:
+                return self.retry_get_report(payload)
+            logging.warning(f"error: {apiIntErr.message}")
             logging.info(f"Повтор запроса: {self.TRY_REQUEST - retry + 1}/{self.TRY_REQUEST}")
             return self.get_report(payload, retry=retry - 1)
         except Exception as er:
             if retry == 0:
                 return self.retry_get_report(payload)
-            logging.warning(f"Необработанное исключение. error: {er}")
+            logging.warning(f"Unknown exception. error: {er}")
             logging.info(f"Повтор запроса: {self.TRY_REQUEST - retry + 1}/{self.TRY_REQUEST}")
             return self.get_report(payload, retry=retry - 1)
         else:
             return answer
 
     def retry_get_report(self, payload: Payload) -> requests.Response:
-        logging.info("Количество ошибок больше заданного! Пауза 10 мин")
+        logging.warning("Количество ошибок больше заданного! Пауза 10 мин")
         time.sleep(self.FORCE_PAUSE)
         return self.get_report(payload)
-
-
```

### Comparing `smartis_sdk-0.6.1/src/smartis_sdk/common.py` & `smartis_sdk-0.7.0/src/smartis_sdk/common.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,25 +9,25 @@
     Placement = 1223
 
 
 MethodFields = namedtuple("MethodFields", "method location id")
 
 
 class Method(Enum):
-    get_projects = MethodFields("projects/get", "projects", "project")
-    get_metrics = MethodFields("metrics/get", "metrics", "code")
-    get_groupings = MethodFields("reports/getGroupings", "groupings", "code")
-    get_attributions = MethodFields("reports/getModelAttributions", "modelAttributions", "id")
-    get_channels = MethodFields("reports/getChannels", "", "")
-    get_placements = MethodFields("reports/getPlacements", "", "")
-    get_campaigns = MethodFields("reports/getCampaigns", "", "")
-    get_ads = MethodFields("reports/getAds", "", "")
-    get_keywords = MethodFields("reports/getKeywords", "", "")
-    get_crm_custom_fields = MethodFields("crm/crmCustomField/get", "crmCustomFields", "")
-    get_crm_custom_field_groups = MethodFields("crm/crmCustomFieldGroup/get", "crmCustomFieldGroups", "")
+    GET_PROJECTS = MethodFields("projects/get", "projects", "project")
+    GET_METRICS = MethodFields("metrics/get", "metrics", "code")
+    GET_GROUPINGS = MethodFields("reports/getGroupings", "groupings", "code")
+    GET_ATTRIBUTIONS = MethodFields("reports/getModelAttributions", "modelAttributions", "id")
+    GET_CHANNELS = MethodFields("reports/getChannels", "", "")
+    GET_PLACEMENTS = MethodFields("reports/getPlacements", "", "")
+    GET_CAMPAIGNS = MethodFields("reports/getCampaigns", "", "")
+    GET_ADS = MethodFields("reports/getAds", "", "")
+    GET_KEYWORDS = MethodFields("reports/getKeywords", "", "")
+    GET_CRM_CUSTOM_FIELDS = MethodFields("crm/crmCustomField/get", "crmCustomFields", "")
+    GET_CRM_CUSTOM_FIELD_GROUPS = MethodFields("crm/crmCustomFieldGroup/get", "crmCustomFieldGroups", "")
 
 
 class GroupBy(Enum):
     ADS = "ad_id"
     DAY = "day"
     PLACEMENT = "placement_id"
     CAMPAIGN = "campaigns"
@@ -39,22 +39,22 @@
     CHANNEL = 1222
     PLACEMENT = 1223
 
 
 class AttributionModel(Enum):
     LAST_CLICK = 1  # Последнее касание
     FIRST_CLICK = 2  # Первое касание
-    LINEAR = 3  # Линейное распределение
+    LINEAR = 3  # Линейное распределение
     BY_POSITION = 4  # На основе позиции
     FIRST_COMMUNICATION = 5  # Первое обращение
-    LINEAR_BY_COMMUNICATION = 6  # Линейное распределение на обращениях
-    LINEAR_WITH_POSTVIEW = 10  # Линейное распределение с учетом postview
-    LAST_CLICK_WITH_POSTVIEW = 15  # Последнее касание с учетом postview
-    FIRST_CLICK_WITH_POSTVIEW = 16  # Первое касание с учетом postview
+    LINEAR_BY_COMMUNICATION = 6  # Линейное распределение на обращениях
+    LINEAR_WITH_POSTVIEW = 10  # Линейное распределение с учетом post-view
+    LAST_CLICK_WITH_POSTVIEW = 15  # Последнее касание с учетом post-view
+    FIRST_CLICK_WITH_POSTVIEW = 16  # Первое касание с учетом post-view
     NOT_FIRST_NOT_LAST_CLICK = 17  # Не первое и не последнее
     LAST_COMMUNICATION = 22  # Последнее обращение
-    BY_POSITION_WITH_POSTVIEW = 23  # На основе позиции с учетом postview
+    BY_POSITION_WITH_POSTVIEW = 23  # На основе позиции с учетом post-view
 
 
 class TypeReport(Enum):
     RAW = "raw"
     AGGREGATED = "aggregated"
```

### Comparing `smartis_sdk-0.6.1/src/smartis_sdk/entity.py` & `smartis_sdk-0.7.0/src/smartis_sdk/entity.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 from datetime import datetime
+from typing import TypeVar
 
 from pydantic import BaseModel, Field
 
 from .common import AttributionModel, GroupBy, TypeReport, FilterCategory
 from .utils import normalize_date
 
 
@@ -97,14 +98,20 @@
     created_at: str
 
 
 class Ads(BaseModel):
     items: list[Ad] = Field(alias='ads')
 
 
+Entity = TypeVar('Entity', ChannelItem, Placement, Campaign, Keyword, CrmCustomField, CrmCustomFieldGroup, Ad)
+FieldsEntity = TypeVar('FieldsEntity', CrmCustomField, CrmCustomFieldGroup)
+RootEntity = TypeVar('RootEntity', Channels, Placements, Campaigns, Keywords, CrmCustomFields, CrmCustomFieldGroups, Ads)
+FieldsRootEntity = TypeVar('FieldsRootEntity', CrmCustomFields, CrmCustomFieldGroups)
+
+
 class Attribution:
 
     def __init__(self, model_id: AttributionModel, period: int, with_direct: bool):
         self.model_id = model_id.value
         self.period = period
         self.with_direct = with_direct
```

### Comparing `smartis_sdk-0.6.1/src/smartis_sdk/utils.py` & `smartis_sdk-0.7.0/src/smartis_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `smartis_sdk-0.6.1/PKG-INFO` & `smartis_sdk-0.7.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartis-sdk
-Version: 0.6.1
+Version: 0.7.0
 Summary: SDK для Smartis API
 License: MIT
 Author: viktor
 Author-email: vi.dave@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

