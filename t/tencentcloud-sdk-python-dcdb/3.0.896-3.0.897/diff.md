# Comparing `tmp/tencentcloud-sdk-python-dcdb-3.0.896.tar.gz` & `tmp/tencentcloud-sdk-python-dcdb-3.0.897.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.896.tar", last modified: Mon May 22 00:21:13 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.897.tar", last modified: Tue May 23 02:20:43 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dcdb-3.0.896.tar` & `tencentcloud-sdk-python-dcdb-3.0.897.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud_sdk_python_dcdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/dcdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/dcdb/v20180411/
--rw-r--r--   0 root         (0) root         (0)    13218 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/dcdb/v20180411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/dcdb/v20180411/__init__.py
--rw-r--r--   0 root         (0) root         (0)   223834 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/dcdb/v20180411/models.py
--rw-r--r--   0 root         (0) root         (0)    65206 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/dcdb/v20180411/dcdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/dcdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:21:13.000000 tencentcloud-sdk-python-dcdb-3.0.896/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud_sdk_python_dcdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-23 02:20:42.000000 tencentcloud-sdk-python-dcdb-3.0.897/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/dcdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/dcdb/v20180411/
+-rw-r--r--   0 root         (0) root         (0)    13507 2023-05-23 02:20:42.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/dcdb/v20180411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:20:42.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/dcdb/v20180411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   235272 2023-05-23 02:20:42.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/dcdb/v20180411/models.py
+-rw-r--r--   0 root         (0) root         (0)    68182 2023-05-23 02:20:42.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/dcdb/v20180411/dcdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-23 02:20:42.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/dcdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-23 02:20:42.000000 tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-23 02:20:42.000000 tencentcloud-sdk-python-dcdb-3.0.897/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-23 02:20:43.000000 tencentcloud-sdk-python-dcdb-3.0.897/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.896/README.rst` & `tencentcloud-sdk-python-dcdb-3.0.897/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/dcdb/v20180411/errorcodes.py` & `tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/dcdb/v20180411/errorcodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,17 @@
 
 # 安全组规则下发失败。
 FAILEDOPERATION_SETSVCLOCATIONFAILED = 'FailedOperation.SetSvcLocationFailed'
 
 # 标签键值校验或鉴权失败。
 FAILEDOPERATION_TAGDRYRUNERROR = 'FailedOperation.TagDryRunError'
 
+# 标签配额不足。
+FAILEDOPERATION_TAGQUOTAEXCEEDLIMIT = 'FailedOperation.TagQuotaExceedLimit'
+
 # 实例安全组信息更新失败。
 FAILEDOPERATION_UPDATEINSTANCEINFOFAILED = 'FailedOperation.UpdateInstanceInfoFailed'
 
 # 用户未实名认证。
 FAILEDOPERATION_USERNOTAUTHED = 'FailedOperation.UserNotAuthed'
 
 # VIP不能与之前一样。
@@ -328,14 +331,17 @@
 
 # 当前部署方式不允许设置此同步模式。
 INVALIDPARAMETERVALUE_SYNCMODENOTALLOWED = 'InvalidParameterValue.SyncModeNotAllowed'
 
 # 请求过于频繁。
 LIMITEXCEEDED_TOOFREQUENTLYCALLED = 'LimitExceeded.TooFrequentlyCalled'
 
+# 资源不足。
+RESOURCEINSUFFICIENT = 'ResourceInsufficient'
+
 # 指定的账号不存在。
 RESOURCENOTFOUND_ACCOUNTDOESNOTEXIST = 'ResourceNotFound.AccountDoesNotExist'
 
 # 实例不存在。
 RESOURCENOTFOUND_INSTANCENOTFOUND = 'ResourceNotFound.InstanceNotFound'
 
 # 找不到指定的数据库实例。
@@ -346,14 +352,17 @@
 
 # 实例状态错误，不能初始化。
 RESOURCEUNAVAILABLE_BADINSTANCESTATUS = 'ResourceUnavailable.BadInstanceStatus'
 
 # COS API调用错误。
 RESOURCEUNAVAILABLE_COSAPIFAILED = 'ResourceUnavailable.CosApiFailed'
 
+# 独享集群状态异常。
+RESOURCEUNAVAILABLE_EXCLUSTERSTATUSABNORMAL = 'ResourceUnavailable.ExclusterStatusAbnormal'
+
 # 数据库实例已被删除。
 RESOURCEUNAVAILABLE_INSTANCEALREADYDELETED = 'ResourceUnavailable.InstanceAlreadyDeleted'
 
 # 数据库实例已经被锁定，当前无法操作。
 RESOURCEUNAVAILABLE_INSTANCEHASBEENLOCKED = 'ResourceUnavailable.InstanceHasBeenLocked'
 
 # 数据库实例状态不正确，当前无法操作。
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/dcdb/v20180411/models.py` & `tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/dcdb/v20180411/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -731,14 +731,173 @@
 
     def _deserialize(self, params):
         self.DealName = params.get("DealName")
         self.InstanceIds = params.get("InstanceIds")
         self.RequestId = params.get("RequestId")
 
 
+class CreateDedicatedClusterDCDBInstanceRequest(AbstractModel):
+    """CreateDedicatedClusterDCDBInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param GoodsNum: 分配实例个数
+        :type GoodsNum: int
+        :param ShardNum: 分片数量
+        :type ShardNum: int
+        :param ShardMemory: 分片內存大小, 单位GB
+        :type ShardMemory: int
+        :param ShardStorage: 分片磁盘大小, 单位GB
+        :type ShardStorage: int
+        :param ClusterId: 独享集群集群uuid
+        :type ClusterId: str
+        :param Zone: （废弃）可用区
+        :type Zone: str
+        :param ProjectId: 项目ID
+        :type ProjectId: int
+        :param Cpu: （废弃）cpu大小，单位：核
+        :type Cpu: int
+        :param VpcId: 网络ID
+        :type VpcId: str
+        :param SubnetId: 子网ID
+        :type SubnetId: str
+        :param ShardMachine: （废弃）分片机型
+        :type ShardMachine: str
+        :param ShardNodeNum: 分片的节点个数
+        :type ShardNodeNum: int
+        :param ShardNodeCpu: （废弃）节点cpu核数，单位：1/100核
+        :type ShardNodeCpu: int
+        :param ShardNodeMemory: （废弃）节点內存大小，单位：GB
+        :type ShardNodeMemory: int
+        :param ShardNodeStorage: （废弃）节点磁盘大小，单位：GB
+        :type ShardNodeStorage: int
+        :param DbVersionId: db版本
+        :type DbVersionId: str
+        :param SecurityGroupId: 安全组ID
+        :type SecurityGroupId: str
+        :param DcnInstanceId: DCN源实例ID
+        :type DcnInstanceId: str
+        :param DcnRegion: DCN源实例地域名
+        :type DcnRegion: str
+        :param InstanceName: 自定义实例名称
+        :type InstanceName: str
+        :param ResourceTags: 标签
+        :type ResourceTags: list of ResourceTag
+        :param Ipv6Flag: 支持IPv6标志：1 支持， 0 不支持
+        :type Ipv6Flag: int
+        :param Pid: （废弃）Pid，可通过获取独享集群售卖配置接口得到
+        :type Pid: int
+        :param InitParams: 参数列表。本接口的可选值为：character_set_server（字符集，必传），lower_case_table_names（表名大小写敏感，必传，0 - 敏感；1-不敏感），innodb_page_size（innodb数据页，默认16K），sync_mode（同步模式：0 - 异步； 1 - 强同步；2 - 强同步可退化。默认为强同步可退化）。
+        :type InitParams: list of DBParamValue
+        :param MasterHostId: 指定主节点uuid，不填随机分配
+        :type MasterHostId: str
+        :param SlaveHostIds: 指定从节点uuid，不填随机分配
+        :type SlaveHostIds: list of str
+        :param RollbackInstanceId: 需要回档的源实例ID
+        :type RollbackInstanceId: str
+        :param RollbackTime: 回档时间
+        :type RollbackTime: str
+        """
+        self.GoodsNum = None
+        self.ShardNum = None
+        self.ShardMemory = None
+        self.ShardStorage = None
+        self.ClusterId = None
+        self.Zone = None
+        self.ProjectId = None
+        self.Cpu = None
+        self.VpcId = None
+        self.SubnetId = None
+        self.ShardMachine = None
+        self.ShardNodeNum = None
+        self.ShardNodeCpu = None
+        self.ShardNodeMemory = None
+        self.ShardNodeStorage = None
+        self.DbVersionId = None
+        self.SecurityGroupId = None
+        self.DcnInstanceId = None
+        self.DcnRegion = None
+        self.InstanceName = None
+        self.ResourceTags = None
+        self.Ipv6Flag = None
+        self.Pid = None
+        self.InitParams = None
+        self.MasterHostId = None
+        self.SlaveHostIds = None
+        self.RollbackInstanceId = None
+        self.RollbackTime = None
+
+
+    def _deserialize(self, params):
+        self.GoodsNum = params.get("GoodsNum")
+        self.ShardNum = params.get("ShardNum")
+        self.ShardMemory = params.get("ShardMemory")
+        self.ShardStorage = params.get("ShardStorage")
+        self.ClusterId = params.get("ClusterId")
+        self.Zone = params.get("Zone")
+        self.ProjectId = params.get("ProjectId")
+        self.Cpu = params.get("Cpu")
+        self.VpcId = params.get("VpcId")
+        self.SubnetId = params.get("SubnetId")
+        self.ShardMachine = params.get("ShardMachine")
+        self.ShardNodeNum = params.get("ShardNodeNum")
+        self.ShardNodeCpu = params.get("ShardNodeCpu")
+        self.ShardNodeMemory = params.get("ShardNodeMemory")
+        self.ShardNodeStorage = params.get("ShardNodeStorage")
+        self.DbVersionId = params.get("DbVersionId")
+        self.SecurityGroupId = params.get("SecurityGroupId")
+        self.DcnInstanceId = params.get("DcnInstanceId")
+        self.DcnRegion = params.get("DcnRegion")
+        self.InstanceName = params.get("InstanceName")
+        if params.get("ResourceTags") is not None:
+            self.ResourceTags = []
+            for item in params.get("ResourceTags"):
+                obj = ResourceTag()
+                obj._deserialize(item)
+                self.ResourceTags.append(obj)
+        self.Ipv6Flag = params.get("Ipv6Flag")
+        self.Pid = params.get("Pid")
+        if params.get("InitParams") is not None:
+            self.InitParams = []
+            for item in params.get("InitParams"):
+                obj = DBParamValue()
+                obj._deserialize(item)
+                self.InitParams.append(obj)
+        self.MasterHostId = params.get("MasterHostId")
+        self.SlaveHostIds = params.get("SlaveHostIds")
+        self.RollbackInstanceId = params.get("RollbackInstanceId")
+        self.RollbackTime = params.get("RollbackTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateDedicatedClusterDCDBInstanceResponse(AbstractModel):
+    """CreateDedicatedClusterDCDBInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class CreateHourDCDBInstanceRequest(AbstractModel):
     """CreateHourDCDBInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -1885,14 +2044,67 @@
                 obj = InstanceBackupFileItem()
                 obj._deserialize(item)
                 self.Files.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
+class DescribeDBEncryptAttributesRequest(AbstractModel):
+    """DescribeDBEncryptAttributes请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例Id，形如：tdsqlshard-ow728lmc。
+        :type InstanceId: str
+        """
+        self.InstanceId = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDBEncryptAttributesResponse(AbstractModel):
+    """DescribeDBEncryptAttributes返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param EncryptStatus: 是否启用加密，1-已开启；0-未开启。
+        :type EncryptStatus: int
+        :param CipherText: DEK密钥
+        :type CipherText: str
+        :param ExpireDate: DEK密钥过期日期。
+        :type ExpireDate: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.EncryptStatus = None
+        self.CipherText = None
+        self.ExpireDate = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.EncryptStatus = params.get("EncryptStatus")
+        self.CipherText = params.get("CipherText")
+        self.ExpireDate = params.get("ExpireDate")
+        self.RequestId = params.get("RequestId")
+
+
 class DescribeDBLogFilesRequest(AbstractModel):
     """DescribeDBLogFiles请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -6246,14 +6458,93 @@
 
 
     def _deserialize(self, params):
         self.DealName = params.get("DealName")
         self.RequestId = params.get("RequestId")
 
 
+class UpgradeDedicatedDCDBInstanceRequest(AbstractModel):
+    """UpgradeDedicatedDCDBInstance请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UpgradeType: 升级类型，取值为ADD，SPLIT和EXPAND。ADD-添加分片；SPLIT-切分某个分片；EXPAND-垂直扩容某个分片
+        :type UpgradeType: str
+        :param InstanceId: 实例ID，形如 dcdbt-mlfjm74h
+        :type InstanceId: str
+        :param AddShardConfig: 当UpgradeType取值为ADD时，添加分片的配置参数
+        :type AddShardConfig: :class:`tencentcloud.dcdb.v20180411.models.AddShardConfig`
+        :param ExpandShardConfig: 当UpgradeType取值为EXPAND时，垂直扩容分片的配置参数
+        :type ExpandShardConfig: :class:`tencentcloud.dcdb.v20180411.models.ExpandShardConfig`
+        :param SplitShardConfig: 当UpgradeType取值为SPLIT时，切分分片的配置参数
+        :type SplitShardConfig: :class:`tencentcloud.dcdb.v20180411.models.SplitShardConfig`
+        :param SwitchAutoRetry: 错过切换时间窗口时，是否自动重试一次，0-否，1-是
+        :type SwitchAutoRetry: int
+        :param SwitchStartTime: 切换时间窗口开始时间
+        :type SwitchStartTime: str
+        :param SwitchEndTime: 切换时间窗口结束时间
+        :type SwitchEndTime: str
+        """
+        self.UpgradeType = None
+        self.InstanceId = None
+        self.AddShardConfig = None
+        self.ExpandShardConfig = None
+        self.SplitShardConfig = None
+        self.SwitchAutoRetry = None
+        self.SwitchStartTime = None
+        self.SwitchEndTime = None
+
+
+    def _deserialize(self, params):
+        self.UpgradeType = params.get("UpgradeType")
+        self.InstanceId = params.get("InstanceId")
+        if params.get("AddShardConfig") is not None:
+            self.AddShardConfig = AddShardConfig()
+            self.AddShardConfig._deserialize(params.get("AddShardConfig"))
+        if params.get("ExpandShardConfig") is not None:
+            self.ExpandShardConfig = ExpandShardConfig()
+            self.ExpandShardConfig._deserialize(params.get("ExpandShardConfig"))
+        if params.get("SplitShardConfig") is not None:
+            self.SplitShardConfig = SplitShardConfig()
+            self.SplitShardConfig._deserialize(params.get("SplitShardConfig"))
+        self.SwitchAutoRetry = params.get("SwitchAutoRetry")
+        self.SwitchStartTime = params.get("SwitchStartTime")
+        self.SwitchEndTime = params.get("SwitchEndTime")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UpgradeDedicatedDCDBInstanceResponse(AbstractModel):
+    """UpgradeDedicatedDCDBInstance返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param FlowId: 异步任务流程ID
+        :type FlowId: int
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.FlowId = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.FlowId = params.get("FlowId")
+        self.RequestId = params.get("RequestId")
+
+
 class UpgradeHourDCDBInstanceRequest(AbstractModel):
     """UpgradeHourDCDBInstance请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/dcdb/v20180411/dcdb_client.py` & `tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/dcdb/v20180411/dcdb_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,14 +207,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateDedicatedClusterDCDBInstance(self, request):
+        """创建独享集群DCDB实例
+
+        :param request: Request instance for CreateDedicatedClusterDCDBInstance.
+        :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateDedicatedClusterDCDBInstanceRequest`
+        :rtype: :class:`tencentcloud.dcdb.v20180411.models.CreateDedicatedClusterDCDBInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateDedicatedClusterDCDBInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateDedicatedClusterDCDBInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateHourDCDBInstance(self, request):
         """创建DCDB后付费实例
 
         :param request: Request instance for CreateHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.CreateHourDCDBInstanceRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.CreateHourDCDBInstanceResponse`
 
@@ -323,14 +346,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def DescribeDBEncryptAttributes(self, request):
+        """本接口(DescribeDBEncryptAttributes)用于查询实例数据加密状态。
+
+        :param request: Request instance for DescribeDBEncryptAttributes.
+        :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBEncryptAttributesRequest`
+        :rtype: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBEncryptAttributesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDBEncryptAttributes", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDBEncryptAttributesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def DescribeDBLogFiles(self, request):
         """本接口(DescribeDBLogFiles)用于获取数据库的各种日志列表，包括冷备、binlog、errlog和slowlog。
 
         :param request: Request instance for DescribeDBLogFiles.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBLogFilesRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.DescribeDBLogFilesResponse`
 
@@ -854,15 +900,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def DescribeSqlLogs(self, request):
-        """本接口（DescribeSqlLogs）用于获取实例SQL日志。
+        """已废弃接口
+
+        本接口（DescribeSqlLogs）用于获取实例SQL日志。
 
         :param request: Request instance for DescribeSqlLogs.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.DescribeSqlLogsRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.DescribeSqlLogsResponse`
 
         """
         try:
@@ -1531,14 +1579,37 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
+
+
+    def UpgradeDedicatedDCDBInstance(self, request):
+        """本接口（UpgradeDedicatedDCDBInstance）用于升级独享DCDB实例
+
+        :param request: Request instance for UpgradeDedicatedDCDBInstance.
+        :type request: :class:`tencentcloud.dcdb.v20180411.models.UpgradeDedicatedDCDBInstanceRequest`
+        :rtype: :class:`tencentcloud.dcdb.v20180411.models.UpgradeDedicatedDCDBInstanceResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("UpgradeDedicatedDCDBInstance", params, headers=headers)
+            response = json.loads(body)
+            model = models.UpgradeDedicatedDCDBInstanceResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
 
 
     def UpgradeHourDCDBInstance(self, request):
         """本接口（UpgradeHourDCDBInstance）用于升级后付费分布式数据库实例。
 
         :param request: Request instance for UpgradeHourDCDBInstance.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.UpgradeHourDCDBInstanceRequest`
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.896/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dcdb-3.0.897/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.896'
+__version__ = '3.0.897'
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.896/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.897/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.896
+Version: 3.0.897
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.896/setup.py` & `tencentcloud-sdk-python-dcdb-3.0.897/setup.py`

 * *Files identical despite different names*

