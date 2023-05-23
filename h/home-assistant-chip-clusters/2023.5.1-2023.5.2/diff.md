# Comparing `tmp/home_assistant_chip_clusters-2023.5.1-py3-none-any.whl.zip` & `tmp/home_assistant_chip_clusters-2023.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,15 @@
-Zip file size: 102701 bytes, number of entries: 12
--rw-r--r--  2.0 unx     2154 b- defN 23-May-16 20:24 chip/ChipUtility.py
--rw-r--r--  2.0 unx   314619 b- defN 23-May-16 20:24 chip/clusters/CHIPClusters.py
--rw-r--r--  2.0 unx    12945 b- defN 23-May-16 20:24 chip/clusters/ClusterObjects.py
--rw-r--r--  2.0 unx  1300430 b- defN 23-May-16 20:24 chip/clusters/Objects.py
--rw-r--r--  2.0 unx     1947 b- defN 23-May-16 20:24 chip/clusters/TestObjects.py
--rw-r--r--  2.0 unx      973 b- defN 23-May-16 20:24 chip/clusters/Types.py
--rw-r--r--  2.0 unx    28802 b- defN 23-May-16 20:24 chip/tlv/__init__.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-16 20:24 home_assistant_chip_clusters-2023.5.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      527 b- defN 23-May-16 20:24 home_assistant_chip_clusters-2023.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-16 20:24 home_assistant_chip_clusters-2023.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-16 20:24 home_assistant_chip_clusters-2023.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1083 b- defN 23-May-16 20:24 home_assistant_chip_clusters-2023.5.1.dist-info/RECORD
-12 files, 1674934 bytes uncompressed, 100863 bytes compressed:  94.0%
+Zip file size: 103842 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     2154 b- defN 23-May-23 12:02 chip/ChipUtility.py
+-rw-r--r--  2.0 unx   314619 b- defN 23-May-23 12:02 chip/clusters/CHIPClusters.py
+-rw-r--r--  2.0 unx    12945 b- defN 23-May-23 12:02 chip/clusters/ClusterObjects.py
+-rw-r--r--  2.0 unx  1296745 b- defN 23-May-23 12:02 chip/clusters/Objects.py
+-rw-r--r--  2.0 unx     1947 b- defN 23-May-23 12:02 chip/clusters/TestObjects.py
+-rw-r--r--  2.0 unx     1014 b- defN 23-May-23 12:02 chip/clusters/Types.py
+-rw-r--r--  2.0 unx     2404 b- defN 23-May-23 12:02 chip/clusters/enum.py
+-rw-r--r--  2.0 unx    28802 b- defN 23-May-23 12:02 chip/tlv/__init__.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-23 12:02 home_assistant_chip_clusters-2023.5.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      548 b- defN 23-May-23 12:02 home_assistant_chip_clusters-2023.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-23 12:02 home_assistant_chip_clusters-2023.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-23 12:02 home_assistant_chip_clusters-2023.5.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1162 b- defN 23-May-23 12:02 home_assistant_chip_clusters-2023.5.2.dist-info/RECORD
+13 files, 1673794 bytes uncompressed, 101886 bytes compressed:  93.9%
```

## zipnote {}

```diff
@@ -12,26 +12,29 @@
 
 Filename: chip/clusters/TestObjects.py
 Comment: 
 
 Filename: chip/clusters/Types.py
 Comment: 
 
+Filename: chip/clusters/enum.py
+Comment: 
+
 Filename: chip/tlv/__init__.py
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.5.1.dist-info/LICENSE
+Filename: home_assistant_chip_clusters-2023.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.5.1.dist-info/METADATA
+Filename: home_assistant_chip_clusters-2023.5.2.dist-info/METADATA
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.5.1.dist-info/WHEEL
+Filename: home_assistant_chip_clusters-2023.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.5.1.dist-info/top_level.txt
+Filename: home_assistant_chip_clusters-2023.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: home_assistant_chip_clusters-2023.5.1.dist-info/RECORD
+Filename: home_assistant_chip_clusters-2023.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chip/clusters/Objects.py

```diff
@@ -30,15 +30,15 @@
 
 from chip import ChipUtility
 from chip.clusters.enum import MatterIntEnum
 from chip.tlv import float32, uint
 
 from .ClusterObjects import (Cluster, ClusterAttributeDescriptor, ClusterCommand, ClusterEvent, ClusterObject,
                              ClusterObjectDescriptor, ClusterObjectFieldDescriptor)
-from .Types import Nullable
+from .Types import Nullable, NullValue
 
 
 @dataclass
 class Identify(Cluster):
     id: typing.ClassVar[int] = 0x0003
 
     @ChipUtility.classproperty
@@ -393,15 +393,15 @@
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="capacity", Tag=0, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="groupList", Tag=1, Type=typing.List[uint]),
                     ])
 
-            capacity: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            capacity: 'typing.Union[Nullable, uint]' = NullValue
             groupList: 'typing.List[uint]' = field(default_factory=lambda: [])
 
         @dataclass
         class RemoveGroup(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0004
             command_id: typing.ClassVar[int] = 0x00000003
             is_client: typing.ClassVar[bool] = True
@@ -897,15 +897,15 @@
                         ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=uint),
                         ClusterObjectFieldDescriptor(Label="capacity", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="groupID", Tag=2, Type=uint),
                         ClusterObjectFieldDescriptor(Label="sceneList", Tag=3, Type=typing.Optional[typing.List[uint]]),
                     ])
 
             status: 'uint' = 0
-            capacity: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            capacity: 'typing.Union[Nullable, uint]' = NullValue
             groupID: 'uint' = 0
             sceneList: 'typing.Optional[typing.List[uint]]' = None
 
         @dataclass
         class EnhancedAddScene(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0005
             command_id: typing.ClassVar[int] = 0x00000040
@@ -1830,15 +1830,15 @@
                         ClusterObjectFieldDescriptor(Label="level", Tag=0, Type=uint),
                         ClusterObjectFieldDescriptor(Label="transitionTime", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="optionsMask", Tag=2, Type=uint),
                         ClusterObjectFieldDescriptor(Label="optionsOverride", Tag=3, Type=uint),
                     ])
 
             level: 'uint' = 0
-            transitionTime: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            transitionTime: 'typing.Union[Nullable, uint]' = NullValue
             optionsMask: 'uint' = 0
             optionsOverride: 'uint' = 0
 
         @dataclass
         class Move(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0008
             command_id: typing.ClassVar[int] = 0x00000001
@@ -1852,15 +1852,15 @@
                         ClusterObjectFieldDescriptor(Label="moveMode", Tag=0, Type=LevelControl.Enums.MoveMode),
                         ClusterObjectFieldDescriptor(Label="rate", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="optionsMask", Tag=2, Type=uint),
                         ClusterObjectFieldDescriptor(Label="optionsOverride", Tag=3, Type=uint),
                     ])
 
             moveMode: 'LevelControl.Enums.MoveMode' = 0
-            rate: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            rate: 'typing.Union[Nullable, uint]' = NullValue
             optionsMask: 'uint' = 0
             optionsOverride: 'uint' = 0
 
         @dataclass
         class Step(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0008
             command_id: typing.ClassVar[int] = 0x00000002
@@ -1876,15 +1876,15 @@
                         ClusterObjectFieldDescriptor(Label="transitionTime", Tag=2, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="optionsMask", Tag=3, Type=uint),
                         ClusterObjectFieldDescriptor(Label="optionsOverride", Tag=4, Type=uint),
                     ])
 
             stepMode: 'LevelControl.Enums.StepMode' = 0
             stepSize: 'uint' = 0
-            transitionTime: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            transitionTime: 'typing.Union[Nullable, uint]' = NullValue
             optionsMask: 'uint' = 0
             optionsOverride: 'uint' = 0
 
         @dataclass
         class Stop(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0008
             command_id: typing.ClassVar[int] = 0x00000003
@@ -1916,15 +1916,15 @@
                         ClusterObjectFieldDescriptor(Label="level", Tag=0, Type=uint),
                         ClusterObjectFieldDescriptor(Label="transitionTime", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="optionsMask", Tag=2, Type=uint),
                         ClusterObjectFieldDescriptor(Label="optionsOverride", Tag=3, Type=uint),
                     ])
 
             level: 'uint' = 0
-            transitionTime: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            transitionTime: 'typing.Union[Nullable, uint]' = NullValue
             optionsMask: 'uint' = 0
             optionsOverride: 'uint' = 0
 
         @dataclass
         class MoveWithOnOff(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0008
             command_id: typing.ClassVar[int] = 0x00000005
@@ -1938,15 +1938,15 @@
                         ClusterObjectFieldDescriptor(Label="moveMode", Tag=0, Type=LevelControl.Enums.MoveMode),
                         ClusterObjectFieldDescriptor(Label="rate", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="optionsMask", Tag=2, Type=uint),
                         ClusterObjectFieldDescriptor(Label="optionsOverride", Tag=3, Type=uint),
                     ])
 
             moveMode: 'LevelControl.Enums.MoveMode' = 0
-            rate: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            rate: 'typing.Union[Nullable, uint]' = NullValue
             optionsMask: 'uint' = 0
             optionsOverride: 'uint' = 0
 
         @dataclass
         class StepWithOnOff(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0008
             command_id: typing.ClassVar[int] = 0x00000006
@@ -1962,15 +1962,15 @@
                         ClusterObjectFieldDescriptor(Label="transitionTime", Tag=2, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="optionsMask", Tag=3, Type=uint),
                         ClusterObjectFieldDescriptor(Label="optionsOverride", Tag=4, Type=uint),
                     ])
 
             stepMode: 'LevelControl.Enums.StepMode' = 0
             stepSize: 'uint' = 0
-            transitionTime: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            transitionTime: 'typing.Union[Nullable, uint]' = NullValue
             optionsMask: 'uint' = 0
             optionsOverride: 'uint' = 0
 
         @dataclass
         class StopWithOnOff(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0008
             command_id: typing.ClassVar[int] = 0x00000007
@@ -2015,15 +2015,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class RemainingTime(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0008
 
@@ -2159,15 +2159,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000011
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class OnTransitionTime(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0008
 
@@ -3170,17 +3170,17 @@
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="cluster", Tag=0, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="endpoint", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="deviceType", Tag=2, Type=typing.Union[Nullable, uint]),
                     ])
 
-            cluster: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            endpoint: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            deviceType: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            cluster: 'typing.Union[Nullable, uint]' = NullValue
+            endpoint: 'typing.Union[Nullable, uint]' = NullValue
+            deviceType: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class AccessControlEntryStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
                     Fields=[
@@ -3189,16 +3189,16 @@
                         ClusterObjectFieldDescriptor(Label="subjects", Tag=3, Type=typing.Union[Nullable, typing.List[uint]]),
                         ClusterObjectFieldDescriptor(Label="targets", Tag=4, Type=typing.Union[Nullable, typing.List[AccessControl.Structs.Target]]),
                         ClusterObjectFieldDescriptor(Label="fabricIndex", Tag=254, Type=uint),
                     ])
 
             privilege: 'AccessControl.Enums.AccessControlEntryPrivilegeEnum' = 0
             authMode: 'AccessControl.Enums.AccessControlEntryAuthModeEnum' = 0
-            subjects: 'typing.Union[Nullable, typing.List[uint]]' = field(default_factory=Nullable)
-            targets: 'typing.Union[Nullable, typing.List[AccessControl.Structs.Target]]' = field(default_factory=Nullable)
+            subjects: 'typing.Union[Nullable, typing.List[uint]]' = NullValue
+            targets: 'typing.Union[Nullable, typing.List[AccessControl.Structs.Target]]' = NullValue
             fabricIndex: 'uint' = 0
 
         @dataclass
         class AccessControlExtensionStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
                 return ClusterObjectDescriptor(
@@ -3405,18 +3405,18 @@
                         ClusterObjectFieldDescriptor(Label="adminNodeID", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="adminPasscodeID", Tag=2, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="changeType", Tag=3, Type=AccessControl.Enums.ChangeTypeEnum),
                         ClusterObjectFieldDescriptor(Label="latestValue", Tag=4, Type=typing.Union[Nullable, AccessControl.Structs.AccessControlEntryStruct]),
                         ClusterObjectFieldDescriptor(Label="fabricIndex", Tag=254, Type=uint),
                     ])
 
-            adminNodeID: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            adminPasscodeID: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            adminNodeID: 'typing.Union[Nullable, uint]' = NullValue
+            adminPasscodeID: 'typing.Union[Nullable, uint]' = NullValue
             changeType: 'AccessControl.Enums.ChangeTypeEnum' = 0
-            latestValue: 'typing.Union[Nullable, AccessControl.Structs.AccessControlEntryStruct]' = field(default_factory=Nullable)
+            latestValue: 'typing.Union[Nullable, AccessControl.Structs.AccessControlEntryStruct]' = NullValue
             fabricIndex: 'uint' = 0
 
         @dataclass
         class AccessControlExtensionChanged(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x001F
@@ -3432,18 +3432,18 @@
                         ClusterObjectFieldDescriptor(Label="adminNodeID", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="adminPasscodeID", Tag=2, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="changeType", Tag=3, Type=AccessControl.Enums.ChangeTypeEnum),
                         ClusterObjectFieldDescriptor(Label="latestValue", Tag=4, Type=typing.Union[Nullable, AccessControl.Structs.AccessControlExtensionStruct]),
                         ClusterObjectFieldDescriptor(Label="fabricIndex", Tag=254, Type=uint),
                     ])
 
-            adminNodeID: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            adminPasscodeID: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            adminNodeID: 'typing.Union[Nullable, uint]' = NullValue
+            adminPasscodeID: 'typing.Union[Nullable, uint]' = NullValue
             changeType: 'AccessControl.Enums.ChangeTypeEnum' = 0
-            latestValue: 'typing.Union[Nullable, AccessControl.Structs.AccessControlExtensionStruct]' = field(default_factory=Nullable)
+            latestValue: 'typing.Union[Nullable, AccessControl.Structs.AccessControlExtensionStruct]' = NullValue
             fabricIndex: 'uint' = 0
 
 
 @dataclass
 class Actions(Cluster):
     id: typing.ClassVar[int] = 0x0025
 
@@ -4121,15 +4121,15 @@
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="finish", Tag=0, Type=BasicInformation.Enums.ProductFinishEnum),
                         ClusterObjectFieldDescriptor(Label="primaryColor", Tag=1, Type=typing.Union[Nullable, BasicInformation.Enums.ColorEnum]),
                     ])
 
             finish: 'BasicInformation.Enums.ProductFinishEnum' = 0
-            primaryColor: 'typing.Union[Nullable, BasicInformation.Enums.ColorEnum]' = field(default_factory=Nullable)
+            primaryColor: 'typing.Union[Nullable, BasicInformation.Enums.ColorEnum]' = NullValue
 
     class Commands:
         @dataclass
         class MfgSpecificPing(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0028
             command_id: typing.ClassVar[int] = 0x10020000
             is_client: typing.ClassVar[bool] = True
@@ -5088,15 +5088,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x002A
 
@@ -5210,15 +5210,15 @@
                         ClusterObjectFieldDescriptor(Label="reason", Tag=2, Type=OtaSoftwareUpdateRequestor.Enums.OTAChangeReasonEnum),
                         ClusterObjectFieldDescriptor(Label="targetSoftwareVersion", Tag=3, Type=typing.Union[Nullable, uint]),
                     ])
 
             previousState: 'OtaSoftwareUpdateRequestor.Enums.OTAUpdateStateEnum' = 0
             newState: 'OtaSoftwareUpdateRequestor.Enums.OTAUpdateStateEnum' = 0
             reason: 'OtaSoftwareUpdateRequestor.Enums.OTAChangeReasonEnum' = 0
-            targetSoftwareVersion: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            targetSoftwareVersion: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class VersionApplied(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x002A
 
@@ -5255,16 +5255,16 @@
                         ClusterObjectFieldDescriptor(Label="bytesDownloaded", Tag=1, Type=uint),
                         ClusterObjectFieldDescriptor(Label="progressPercent", Tag=2, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="platformCode", Tag=3, Type=typing.Union[Nullable, int]),
                     ])
 
             softwareVersion: 'uint' = 0
             bytesDownloaded: 'uint' = 0
-            progressPercent: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            platformCode: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            progressPercent: 'typing.Union[Nullable, uint]' = NullValue
+            platformCode: 'typing.Union[Nullable, int]' = NullValue
 
 
 @dataclass
 class LocalizationConfiguration(Cluster):
     id: typing.ClassVar[int] = 0x002B
 
     @ChipUtility.classproperty
@@ -7574,15 +7574,15 @@
                         ClusterObjectFieldDescriptor(Label="networkingStatus", Tag=0, Type=NetworkCommissioning.Enums.NetworkCommissioningStatus),
                         ClusterObjectFieldDescriptor(Label="debugText", Tag=1, Type=typing.Optional[str]),
                         ClusterObjectFieldDescriptor(Label="errorValue", Tag=2, Type=typing.Union[Nullable, int]),
                     ])
 
             networkingStatus: 'NetworkCommissioning.Enums.NetworkCommissioningStatus' = 0
             debugText: 'typing.Optional[str]' = None
-            errorValue: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            errorValue: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class ReorderNetwork(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0031
             command_id: typing.ClassVar[int] = 0x00000008
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'NetworkConfigResponse'
@@ -7691,15 +7691,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000005
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, NetworkCommissioning.Enums.NetworkCommissioningStatus])
 
-            value: 'typing.Union[Nullable, NetworkCommissioning.Enums.NetworkCommissioningStatus]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, NetworkCommissioning.Enums.NetworkCommissioningStatus]' = NullValue
 
         @dataclass
         class LastNetworkID(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0031
 
@@ -7707,15 +7707,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000006
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, bytes])
 
-            value: 'typing.Union[Nullable, bytes]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, bytes]' = NullValue
 
         @dataclass
         class LastConnectErrorValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0031
 
@@ -7723,15 +7723,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000007
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0031
 
@@ -8148,16 +8148,16 @@
                         ClusterObjectFieldDescriptor(Label="IPv4Addresses", Tag=5, Type=typing.List[bytes]),
                         ClusterObjectFieldDescriptor(Label="IPv6Addresses", Tag=6, Type=typing.List[bytes]),
                         ClusterObjectFieldDescriptor(Label="type", Tag=7, Type=GeneralDiagnostics.Enums.InterfaceTypeEnum),
                     ])
 
             name: 'str' = ""
             isOperational: 'bool' = False
-            offPremiseServicesReachableIPv4: 'typing.Union[Nullable, bool]' = field(default_factory=Nullable)
-            offPremiseServicesReachableIPv6: 'typing.Union[Nullable, bool]' = field(default_factory=Nullable)
+            offPremiseServicesReachableIPv4: 'typing.Union[Nullable, bool]' = NullValue
+            offPremiseServicesReachableIPv6: 'typing.Union[Nullable, bool]' = NullValue
             hardwareAddress: 'bytes' = b""
             IPv4Addresses: 'typing.List[bytes]' = field(default_factory=lambda: [])
             IPv6Addresses: 'typing.List[bytes]' = field(default_factory=lambda: [])
             type: 'GeneralDiagnostics.Enums.InterfaceTypeEnum' = 0
 
     class Commands:
         @dataclass
@@ -8974,16 +8974,16 @@
 
             extAddress: 'uint' = 0
             age: 'uint' = 0
             rloc16: 'uint' = 0
             linkFrameCounter: 'uint' = 0
             mleFrameCounter: 'uint' = 0
             lqi: 'uint' = 0
-            averageRssi: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
-            lastRssi: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            averageRssi: 'typing.Union[Nullable, int]' = NullValue
+            lastRssi: 'typing.Union[Nullable, int]' = NullValue
             frameErrorRate: 'uint' = 0
             messageErrorRate: 'uint' = 0
             rxOnWhenIdle: 'bool' = False
             fullThreadDevice: 'bool' = False
             fullNetworkData: 'bool' = False
             isChild: 'bool' = False
 
@@ -9087,15 +9087,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class RoutingRole(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -9103,15 +9103,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, ThreadNetworkDiagnostics.Enums.RoutingRole])
 
-            value: 'typing.Union[Nullable, ThreadNetworkDiagnostics.Enums.RoutingRole]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, ThreadNetworkDiagnostics.Enums.RoutingRole]' = NullValue
 
         @dataclass
         class NetworkName(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -9119,15 +9119,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, str])
 
-            value: 'typing.Union[Nullable, str]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, str]' = NullValue
 
         @dataclass
         class PanId(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -9135,15 +9135,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class ExtendedPanId(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -9151,15 +9151,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000004
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class MeshLocalPrefix(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -9167,15 +9167,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000005
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, bytes])
 
-            value: 'typing.Union[Nullable, bytes]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, bytes]' = NullValue
 
         @dataclass
         class OverrunCount(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -9231,15 +9231,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000009
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class Weighting(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -9247,15 +9247,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000000A
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class DataVersion(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -9263,15 +9263,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000000B
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class StableDataVersion(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -9279,15 +9279,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000000C
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class LeaderRouterId(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -9295,15 +9295,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000000D
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class DetachedRoleCount(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -10031,15 +10031,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000003B
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, ThreadNetworkDiagnostics.Structs.SecurityPolicy])
 
-            value: 'typing.Union[Nullable, ThreadNetworkDiagnostics.Structs.SecurityPolicy]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, ThreadNetworkDiagnostics.Structs.SecurityPolicy]' = NullValue
 
         @dataclass
         class ChannelPage0Mask(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -10047,15 +10047,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000003C
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, bytes])
 
-            value: 'typing.Union[Nullable, bytes]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, bytes]' = NullValue
 
         @dataclass
         class OperationalDatasetComponents(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -10063,15 +10063,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000003D
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, ThreadNetworkDiagnostics.Structs.OperationalDatasetComponents])
 
-            value: 'typing.Union[Nullable, ThreadNetworkDiagnostics.Structs.OperationalDatasetComponents]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, ThreadNetworkDiagnostics.Structs.OperationalDatasetComponents]' = NullValue
 
         @dataclass
         class ActiveNetworkFaultsList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0035
 
@@ -10349,15 +10349,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, bytes])
 
-            value: 'typing.Union[Nullable, bytes]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, bytes]' = NullValue
 
         @dataclass
         class SecurityType(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0036
 
@@ -10365,15 +10365,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, WiFiNetworkDiagnostics.Enums.SecurityTypeEnum])
 
-            value: 'typing.Union[Nullable, WiFiNetworkDiagnostics.Enums.SecurityTypeEnum]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, WiFiNetworkDiagnostics.Enums.SecurityTypeEnum]' = NullValue
 
         @dataclass
         class WiFiVersion(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0036
 
@@ -10381,15 +10381,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, WiFiNetworkDiagnostics.Enums.WiFiVersionEnum])
 
-            value: 'typing.Union[Nullable, WiFiNetworkDiagnostics.Enums.WiFiVersionEnum]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, WiFiNetworkDiagnostics.Enums.WiFiVersionEnum]' = NullValue
 
         @dataclass
         class ChannelNumber(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0036
 
@@ -10397,15 +10397,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class Rssi(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0036
 
@@ -10413,15 +10413,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000004
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class BeaconLostCount(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0036
 
@@ -11167,15 +11167,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class Granularity(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0038
 
@@ -11215,15 +11215,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class DefaultNtp(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0038
 
@@ -11519,15 +11519,15 @@
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="finish", Tag=0, Type=BridgedDeviceBasicInformation.Enums.ProductFinishEnum),
                         ClusterObjectFieldDescriptor(Label="primaryColor", Tag=1, Type=typing.Union[Nullable, BridgedDeviceBasicInformation.Enums.ColorEnum]),
                     ])
 
             finish: 'BridgedDeviceBasicInformation.Enums.ProductFinishEnum' = 0
-            primaryColor: 'typing.Union[Nullable, BridgedDeviceBasicInformation.Enums.ColorEnum]' = field(default_factory=Nullable)
+            primaryColor: 'typing.Union[Nullable, BridgedDeviceBasicInformation.Enums.ColorEnum]' = NullValue
 
     class Attributes:
         @dataclass
         class VendorName(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0039
@@ -12414,15 +12414,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class AdminVendorId(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x003C
 
@@ -12430,15 +12430,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class GeneratedCommandList(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x003C
 
@@ -12625,15 +12625,15 @@
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="noc", Tag=1, Type=bytes),
                         ClusterObjectFieldDescriptor(Label="icac", Tag=2, Type=typing.Union[Nullable, bytes]),
                         ClusterObjectFieldDescriptor(Label="fabricIndex", Tag=254, Type=uint),
                     ])
 
             noc: 'bytes' = b""
-            icac: 'typing.Union[Nullable, bytes]' = field(default_factory=Nullable)
+            icac: 'typing.Union[Nullable, bytes]' = NullValue
             fabricIndex: 'uint' = 0
 
     class Commands:
         @dataclass
         class AttestationRequest(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x003E
             command_id: typing.ClassVar[int] = 0x00000000
@@ -13127,20 +13127,20 @@
                         ClusterObjectFieldDescriptor(Label="epochStartTime1", Tag=5, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="epochKey2", Tag=6, Type=typing.Union[Nullable, bytes]),
                         ClusterObjectFieldDescriptor(Label="epochStartTime2", Tag=7, Type=typing.Union[Nullable, uint]),
                     ])
 
             groupKeySetID: 'uint' = 0
             groupKeySecurityPolicy: 'GroupKeyManagement.Enums.GroupKeySecurityPolicyEnum' = 0
-            epochKey0: 'typing.Union[Nullable, bytes]' = field(default_factory=Nullable)
-            epochStartTime0: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            epochKey1: 'typing.Union[Nullable, bytes]' = field(default_factory=Nullable)
-            epochStartTime1: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            epochKey2: 'typing.Union[Nullable, bytes]' = field(default_factory=Nullable)
-            epochStartTime2: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            epochKey0: 'typing.Union[Nullable, bytes]' = NullValue
+            epochStartTime0: 'typing.Union[Nullable, uint]' = NullValue
+            epochKey1: 'typing.Union[Nullable, bytes]' = NullValue
+            epochStartTime1: 'typing.Union[Nullable, uint]' = NullValue
+            epochKey2: 'typing.Union[Nullable, bytes]' = NullValue
+            epochStartTime2: 'typing.Union[Nullable, uint]' = NullValue
 
     class Commands:
         @dataclass
         class KeySetWrite(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x003F
             command_id: typing.ClassVar[int] = 0x00000000
             is_client: typing.ClassVar[bool] = True
@@ -14337,15 +14337,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class SupportedModes(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0050
 
@@ -15350,19 +15350,19 @@
 
             @ChipUtility.classproperty
             def must_use_timed_invoke(cls) -> bool:
                 return True
 
             operationType: 'DoorLock.Enums.DataOperationTypeEnum' = 0
             userIndex: 'uint' = 0
-            userName: 'typing.Union[Nullable, str]' = field(default_factory=Nullable)
-            userUniqueID: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            userStatus: 'typing.Union[Nullable, DoorLock.Enums.UserStatusEnum]' = field(default_factory=Nullable)
-            userType: 'typing.Union[Nullable, DoorLock.Enums.UserTypeEnum]' = field(default_factory=Nullable)
-            credentialRule: 'typing.Union[Nullable, DoorLock.Enums.CredentialRuleEnum]' = field(default_factory=Nullable)
+            userName: 'typing.Union[Nullable, str]' = NullValue
+            userUniqueID: 'typing.Union[Nullable, uint]' = NullValue
+            userStatus: 'typing.Union[Nullable, DoorLock.Enums.UserStatusEnum]' = NullValue
+            userType: 'typing.Union[Nullable, DoorLock.Enums.UserTypeEnum]' = NullValue
+            credentialRule: 'typing.Union[Nullable, DoorLock.Enums.CredentialRuleEnum]' = NullValue
 
         @dataclass
         class GetUser(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0101
             command_id: typing.ClassVar[int] = 0x0000001B
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'GetUserResponse'
@@ -15396,23 +15396,23 @@
                         ClusterObjectFieldDescriptor(Label="credentials", Tag=6, Type=typing.Union[Nullable, typing.List[DoorLock.Structs.CredentialStruct]]),
                         ClusterObjectFieldDescriptor(Label="creatorFabricIndex", Tag=7, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="lastModifiedFabricIndex", Tag=8, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="nextUserIndex", Tag=9, Type=typing.Union[Nullable, uint]),
                     ])
 
             userIndex: 'uint' = 0
-            userName: 'typing.Union[Nullable, str]' = field(default_factory=Nullable)
-            userUniqueID: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            userStatus: 'typing.Union[Nullable, DoorLock.Enums.UserStatusEnum]' = field(default_factory=Nullable)
-            userType: 'typing.Union[Nullable, DoorLock.Enums.UserTypeEnum]' = field(default_factory=Nullable)
-            credentialRule: 'typing.Union[Nullable, DoorLock.Enums.CredentialRuleEnum]' = field(default_factory=Nullable)
-            credentials: 'typing.Union[Nullable, typing.List[DoorLock.Structs.CredentialStruct]]' = field(default_factory=Nullable)
-            creatorFabricIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            lastModifiedFabricIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            nextUserIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            userName: 'typing.Union[Nullable, str]' = NullValue
+            userUniqueID: 'typing.Union[Nullable, uint]' = NullValue
+            userStatus: 'typing.Union[Nullable, DoorLock.Enums.UserStatusEnum]' = NullValue
+            userType: 'typing.Union[Nullable, DoorLock.Enums.UserTypeEnum]' = NullValue
+            credentialRule: 'typing.Union[Nullable, DoorLock.Enums.CredentialRuleEnum]' = NullValue
+            credentials: 'typing.Union[Nullable, typing.List[DoorLock.Structs.CredentialStruct]]' = NullValue
+            creatorFabricIndex: 'typing.Union[Nullable, uint]' = NullValue
+            lastModifiedFabricIndex: 'typing.Union[Nullable, uint]' = NullValue
+            nextUserIndex: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class ClearUser(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0101
             command_id: typing.ClassVar[int] = 0x0000001D
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
@@ -15452,17 +15452,17 @@
             @ChipUtility.classproperty
             def must_use_timed_invoke(cls) -> bool:
                 return True
 
             operationType: 'DoorLock.Enums.DataOperationTypeEnum' = 0
             credential: 'DoorLock.Structs.CredentialStruct' = field(default_factory=lambda: DoorLock.Structs.CredentialStruct())
             credentialData: 'bytes' = b""
-            userIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            userStatus: 'typing.Union[Nullable, DoorLock.Enums.UserStatusEnum]' = field(default_factory=Nullable)
-            userType: 'typing.Union[Nullable, DoorLock.Enums.UserTypeEnum]' = field(default_factory=Nullable)
+            userIndex: 'typing.Union[Nullable, uint]' = NullValue
+            userStatus: 'typing.Union[Nullable, DoorLock.Enums.UserStatusEnum]' = NullValue
+            userType: 'typing.Union[Nullable, DoorLock.Enums.UserTypeEnum]' = NullValue
 
         @dataclass
         class SetCredentialResponse(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0101
             command_id: typing.ClassVar[int] = 0x00000023
             is_client: typing.ClassVar[bool] = False
             response_type: typing.ClassVar[str] = None
@@ -15473,16 +15473,16 @@
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="status", Tag=0, Type=DoorLock.Enums.DlStatus),
                         ClusterObjectFieldDescriptor(Label="userIndex", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="nextCredentialIndex", Tag=2, Type=typing.Union[Nullable, uint]),
                     ])
 
             status: 'DoorLock.Enums.DlStatus' = 0
-            userIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            nextCredentialIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            userIndex: 'typing.Union[Nullable, uint]' = NullValue
+            nextCredentialIndex: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class GetCredentialStatus(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0101
             command_id: typing.ClassVar[int] = 0x00000024
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = 'GetCredentialStatusResponse'
@@ -15511,18 +15511,18 @@
                         ClusterObjectFieldDescriptor(Label="userIndex", Tag=1, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="creatorFabricIndex", Tag=2, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="lastModifiedFabricIndex", Tag=3, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="nextCredentialIndex", Tag=4, Type=typing.Union[Nullable, uint]),
                     ])
 
             credentialExists: 'bool' = False
-            userIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            creatorFabricIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            lastModifiedFabricIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            nextCredentialIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            userIndex: 'typing.Union[Nullable, uint]' = NullValue
+            creatorFabricIndex: 'typing.Union[Nullable, uint]' = NullValue
+            lastModifiedFabricIndex: 'typing.Union[Nullable, uint]' = NullValue
+            nextCredentialIndex: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class ClearCredential(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0101
             command_id: typing.ClassVar[int] = 0x00000026
             is_client: typing.ClassVar[bool] = True
             response_type: typing.ClassVar[str] = None
@@ -15534,15 +15534,15 @@
                         ClusterObjectFieldDescriptor(Label="credential", Tag=0, Type=typing.Union[Nullable, DoorLock.Structs.CredentialStruct]),
                     ])
 
             @ChipUtility.classproperty
             def must_use_timed_invoke(cls) -> bool:
                 return True
 
-            credential: 'typing.Union[Nullable, DoorLock.Structs.CredentialStruct]' = field(default_factory=Nullable)
+            credential: 'typing.Union[Nullable, DoorLock.Structs.CredentialStruct]' = NullValue
 
     class Attributes:
         @dataclass
         class LockState(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0101
@@ -15551,15 +15551,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, DoorLock.Enums.DlLockState])
 
-            value: 'typing.Union[Nullable, DoorLock.Enums.DlLockState]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, DoorLock.Enums.DlLockState]' = NullValue
 
         @dataclass
         class LockType(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0101
 
@@ -16272,17 +16272,17 @@
                         ClusterObjectFieldDescriptor(Label="fabricIndex", Tag=3, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="sourceNode", Tag=4, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="credentials", Tag=5, Type=typing.Union[None, Nullable, typing.List[DoorLock.Structs.CredentialStruct]]),
                     ])
 
             lockOperationType: 'DoorLock.Enums.LockOperationTypeEnum' = 0
             operationSource: 'DoorLock.Enums.OperationSourceEnum' = 0
-            userIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            fabricIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            sourceNode: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            userIndex: 'typing.Union[Nullable, uint]' = NullValue
+            fabricIndex: 'typing.Union[Nullable, uint]' = NullValue
+            sourceNode: 'typing.Union[Nullable, uint]' = NullValue
             credentials: 'typing.Union[None, Nullable, typing.List[DoorLock.Structs.CredentialStruct]]' = None
 
         @dataclass
         class LockOperationError(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0101
@@ -16303,17 +16303,17 @@
                         ClusterObjectFieldDescriptor(Label="sourceNode", Tag=5, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="credentials", Tag=6, Type=typing.Union[None, Nullable, typing.List[DoorLock.Structs.CredentialStruct]]),
                     ])
 
             lockOperationType: 'DoorLock.Enums.LockOperationTypeEnum' = 0
             operationSource: 'DoorLock.Enums.OperationSourceEnum' = 0
             operationError: 'DoorLock.Enums.OperationErrorEnum' = 0
-            userIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            fabricIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            sourceNode: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            userIndex: 'typing.Union[Nullable, uint]' = NullValue
+            fabricIndex: 'typing.Union[Nullable, uint]' = NullValue
+            sourceNode: 'typing.Union[Nullable, uint]' = NullValue
             credentials: 'typing.Union[None, Nullable, typing.List[DoorLock.Structs.CredentialStruct]]' = None
 
         @dataclass
         class LockUserChange(ClusterEvent):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0101
@@ -16334,18 +16334,18 @@
                         ClusterObjectFieldDescriptor(Label="sourceNode", Tag=5, Type=typing.Union[Nullable, uint]),
                         ClusterObjectFieldDescriptor(Label="dataIndex", Tag=6, Type=typing.Union[Nullable, uint]),
                     ])
 
             lockDataType: 'DoorLock.Enums.LockDataTypeEnum' = 0
             dataOperationType: 'DoorLock.Enums.DataOperationTypeEnum' = 0
             operationSource: 'DoorLock.Enums.OperationSourceEnum' = 0
-            userIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            fabricIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            sourceNode: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
-            dataIndex: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            userIndex: 'typing.Union[Nullable, uint]' = NullValue
+            fabricIndex: 'typing.Union[Nullable, uint]' = NullValue
+            sourceNode: 'typing.Union[Nullable, uint]' = NullValue
+            dataIndex: 'typing.Union[Nullable, uint]' = NullValue
 
 
 @dataclass
 class WindowCovering(Cluster):
     id: typing.ClassVar[int] = 0x0102
 
     @ChipUtility.classproperty
@@ -17515,15 +17515,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class MaxSpeed(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0200
 
@@ -17531,15 +17531,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class MaxFlow(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0200
 
@@ -17547,15 +17547,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class MinConstPressure(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0200
 
@@ -17771,15 +17771,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000013
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class Speed(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0200
 
@@ -18446,16 +18446,16 @@
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="transitionTime", Tag=0, Type=uint),
                         ClusterObjectFieldDescriptor(Label="heatSetpoint", Tag=1, Type=typing.Union[Nullable, int]),
                         ClusterObjectFieldDescriptor(Label="coolSetpoint", Tag=2, Type=typing.Union[Nullable, int]),
                     ])
 
             transitionTime: 'uint' = 0
-            heatSetpoint: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
-            coolSetpoint: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            heatSetpoint: 'typing.Union[Nullable, int]' = NullValue
+            coolSetpoint: 'typing.Union[Nullable, int]' = NullValue
 
     class Commands:
         @dataclass
         class SetpointRaiseLower(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0201
             command_id: typing.ClassVar[int] = 0x00000000
             is_client: typing.ClassVar[bool] = True
@@ -18558,15 +18558,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class OutdoorTemperature(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0201
 
@@ -19565,15 +19565,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class PercentCurrent(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0202
 
@@ -20818,15 +20818,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000010
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class Primary1X(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0300
 
@@ -22004,15 +22004,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class MinMeasuredValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0400
 
@@ -22020,15 +22020,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class MaxMeasuredValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0400
 
@@ -22036,15 +22036,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class Tolerance(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0400
 
@@ -22213,15 +22213,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class MinMeasuredValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0402
 
@@ -22229,15 +22229,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class MaxMeasuredValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0402
 
@@ -22245,15 +22245,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class Tolerance(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0402
 
@@ -22420,15 +22420,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class MinMeasuredValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0403
 
@@ -22436,15 +22436,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class MaxMeasuredValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0403
 
@@ -22452,15 +22452,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class Tolerance(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0403
 
@@ -22693,15 +22693,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class MinMeasuredValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0404
 
@@ -22709,15 +22709,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class MaxMeasuredValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0404
 
@@ -22725,15 +22725,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class Tolerance(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0404
 
@@ -22886,15 +22886,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class MinMeasuredValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0405
 
@@ -22902,15 +22902,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class MaxMeasuredValue(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0405
 
@@ -22918,15 +22918,15 @@
             def attribute_id(cls) -> int:
                 return 0x00000002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class Tolerance(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0x0405
 
@@ -24133,15 +24133,15 @@
                 return ClusterObjectDescriptor(
                     Fields=[
                         ClusterObjectFieldDescriptor(Label="updatedAt", Tag=0, Type=uint),
                         ClusterObjectFieldDescriptor(Label="position", Tag=1, Type=typing.Union[Nullable, uint]),
                     ])
 
             updatedAt: 'uint' = 0
-            position: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            position: 'typing.Union[Nullable, uint]' = NullValue
 
     class Commands:
         @dataclass
         class Play(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0x0506
             command_id: typing.ClassVar[int] = 0x00000000
             is_client: typing.ClassVar[bool] = True
@@ -29553,15 +29553,15 @@
                         ClusterObjectFieldDescriptor(Label="fabricSensitiveStruct", Tag=6, Type=UnitTesting.Structs.SimpleStruct),
                         ClusterObjectFieldDescriptor(Label="fabricSensitiveInt8uList", Tag=7, Type=typing.List[uint]),
                         ClusterObjectFieldDescriptor(Label="fabricIndex", Tag=254, Type=uint),
                     ])
 
             fabricSensitiveInt8u: 'uint' = 0
             optionalFabricSensitiveInt8u: 'typing.Optional[uint]' = None
-            nullableFabricSensitiveInt8u: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            nullableFabricSensitiveInt8u: 'typing.Union[Nullable, uint]' = NullValue
             nullableOptionalFabricSensitiveInt8u: 'typing.Union[None, Nullable, uint]' = None
             fabricSensitiveCharString: 'str' = ""
             fabricSensitiveStruct: 'UnitTesting.Structs.SimpleStruct' = field(default_factory=lambda: UnitTesting.Structs.SimpleStruct())
             fabricSensitiveInt8uList: 'typing.List[uint]' = field(default_factory=lambda: [])
             fabricIndex: 'uint' = 0
 
         @dataclass
@@ -29580,24 +29580,24 @@
                         ClusterObjectFieldDescriptor(Label="optionalStruct", Tag=7, Type=typing.Optional[UnitTesting.Structs.SimpleStruct]),
                         ClusterObjectFieldDescriptor(Label="nullableOptionalStruct", Tag=8, Type=typing.Union[None, Nullable, UnitTesting.Structs.SimpleStruct]),
                         ClusterObjectFieldDescriptor(Label="nullableList", Tag=9, Type=typing.Union[Nullable, typing.List[UnitTesting.Enums.SimpleEnum]]),
                         ClusterObjectFieldDescriptor(Label="optionalList", Tag=10, Type=typing.Optional[typing.List[UnitTesting.Enums.SimpleEnum]]),
                         ClusterObjectFieldDescriptor(Label="nullableOptionalList", Tag=11, Type=typing.Union[None, Nullable, typing.List[UnitTesting.Enums.SimpleEnum]]),
                     ])
 
-            nullableInt: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            nullableInt: 'typing.Union[Nullable, uint]' = NullValue
             optionalInt: 'typing.Optional[uint]' = None
             nullableOptionalInt: 'typing.Union[None, Nullable, uint]' = None
-            nullableString: 'typing.Union[Nullable, str]' = field(default_factory=Nullable)
+            nullableString: 'typing.Union[Nullable, str]' = NullValue
             optionalString: 'typing.Optional[str]' = None
             nullableOptionalString: 'typing.Union[None, Nullable, str]' = None
-            nullableStruct: 'typing.Union[Nullable, UnitTesting.Structs.SimpleStruct]' = field(default_factory=Nullable)
+            nullableStruct: 'typing.Union[Nullable, UnitTesting.Structs.SimpleStruct]' = NullValue
             optionalStruct: 'typing.Optional[UnitTesting.Structs.SimpleStruct]' = None
             nullableOptionalStruct: 'typing.Union[None, Nullable, UnitTesting.Structs.SimpleStruct]' = None
-            nullableList: 'typing.Union[Nullable, typing.List[UnitTesting.Enums.SimpleEnum]]' = field(default_factory=Nullable)
+            nullableList: 'typing.Union[Nullable, typing.List[UnitTesting.Enums.SimpleEnum]]' = NullValue
             optionalList: 'typing.Optional[typing.List[UnitTesting.Enums.SimpleEnum]]' = None
             nullableOptionalList: 'typing.Union[None, Nullable, typing.List[UnitTesting.Enums.SimpleEnum]]' = None
 
         @dataclass
         class NestedStruct(ClusterObject):
             @ChipUtility.classproperty
             def descriptor(cls) -> ClusterObjectDescriptor:
@@ -30203,24 +30203,24 @@
                         ClusterObjectFieldDescriptor(Label="optionalStruct", Tag=7, Type=typing.Optional[UnitTesting.Structs.SimpleStruct]),
                         ClusterObjectFieldDescriptor(Label="nullableOptionalStruct", Tag=8, Type=typing.Union[None, Nullable, UnitTesting.Structs.SimpleStruct]),
                         ClusterObjectFieldDescriptor(Label="nullableList", Tag=9, Type=typing.Union[Nullable, typing.List[UnitTesting.Enums.SimpleEnum]]),
                         ClusterObjectFieldDescriptor(Label="optionalList", Tag=10, Type=typing.Optional[typing.List[UnitTesting.Enums.SimpleEnum]]),
                         ClusterObjectFieldDescriptor(Label="nullableOptionalList", Tag=11, Type=typing.Union[None, Nullable, typing.List[UnitTesting.Enums.SimpleEnum]]),
                     ])
 
-            nullableInt: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            nullableInt: 'typing.Union[Nullable, uint]' = NullValue
             optionalInt: 'typing.Optional[uint]' = None
             nullableOptionalInt: 'typing.Union[None, Nullable, uint]' = None
-            nullableString: 'typing.Union[Nullable, str]' = field(default_factory=Nullable)
+            nullableString: 'typing.Union[Nullable, str]' = NullValue
             optionalString: 'typing.Optional[str]' = None
             nullableOptionalString: 'typing.Union[None, Nullable, str]' = None
-            nullableStruct: 'typing.Union[Nullable, UnitTesting.Structs.SimpleStruct]' = field(default_factory=Nullable)
+            nullableStruct: 'typing.Union[Nullable, UnitTesting.Structs.SimpleStruct]' = NullValue
             optionalStruct: 'typing.Optional[UnitTesting.Structs.SimpleStruct]' = None
             nullableOptionalStruct: 'typing.Union[None, Nullable, UnitTesting.Structs.SimpleStruct]' = None
-            nullableList: 'typing.Union[Nullable, typing.List[UnitTesting.Enums.SimpleEnum]]' = field(default_factory=Nullable)
+            nullableList: 'typing.Union[Nullable, typing.List[UnitTesting.Enums.SimpleEnum]]' = NullValue
             optionalList: 'typing.Optional[typing.List[UnitTesting.Enums.SimpleEnum]]' = None
             nullableOptionalList: 'typing.Union[None, Nullable, typing.List[UnitTesting.Enums.SimpleEnum]]' = None
 
         @dataclass
         class SimpleStructEchoRequest(ClusterCommand):
             cluster_id: typing.ClassVar[int] = 0xFFF1FC05
             command_id: typing.ClassVar[int] = 0x00000011
@@ -31088,15 +31088,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004000
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, bool])
 
-            value: 'typing.Union[Nullable, bool]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, bool]' = NullValue
 
         @dataclass
         class NullableBitmap8(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31104,15 +31104,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004001
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableBitmap16(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31120,15 +31120,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004002
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableBitmap32(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31136,15 +31136,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004003
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableBitmap64(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31152,15 +31152,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004004
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableInt8u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31168,15 +31168,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004005
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableInt16u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31184,15 +31184,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004006
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableInt24u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31200,15 +31200,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004007
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableInt32u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31216,15 +31216,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004008
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableInt40u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31232,15 +31232,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004009
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableInt48u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31248,15 +31248,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000400A
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableInt56u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31264,15 +31264,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000400B
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableInt64u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31280,15 +31280,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000400C
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableInt8s(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31296,15 +31296,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000400D
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class NullableInt16s(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31312,15 +31312,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000400E
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class NullableInt24s(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31328,15 +31328,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000400F
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class NullableInt32s(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31344,15 +31344,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004010
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class NullableInt40s(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31360,15 +31360,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004011
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class NullableInt48s(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31376,15 +31376,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004012
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class NullableInt56s(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31392,15 +31392,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004013
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class NullableInt64s(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31408,15 +31408,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004014
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class NullableEnum8(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31424,15 +31424,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004015
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableEnum16(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31440,15 +31440,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004016
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableFloatSingle(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31456,15 +31456,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004017
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, float32])
 
-            value: 'typing.Union[Nullable, float32]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, float32]' = NullValue
 
         @dataclass
         class NullableFloatDouble(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31472,15 +31472,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004018
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, float])
 
-            value: 'typing.Union[Nullable, float]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, float]' = NullValue
 
         @dataclass
         class NullableOctetString(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31488,15 +31488,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004019
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, bytes])
 
-            value: 'typing.Union[Nullable, bytes]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, bytes]' = NullValue
 
         @dataclass
         class NullableCharString(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31504,15 +31504,15 @@
             def attribute_id(cls) -> int:
                 return 0x0000401E
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, str])
 
-            value: 'typing.Union[Nullable, str]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, str]' = NullValue
 
         @dataclass
         class NullableEnumAttr(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31520,15 +31520,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004024
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, UnitTesting.Enums.SimpleEnum])
 
-            value: 'typing.Union[Nullable, UnitTesting.Enums.SimpleEnum]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, UnitTesting.Enums.SimpleEnum]' = NullValue
 
         @dataclass
         class NullableStruct(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31536,15 +31536,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004025
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, UnitTesting.Structs.SimpleStruct])
 
-            value: 'typing.Union[Nullable, UnitTesting.Structs.SimpleStruct]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, UnitTesting.Structs.SimpleStruct]' = NullValue
 
         @dataclass
         class NullableRangeRestrictedInt8u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31552,15 +31552,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004026
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableRangeRestrictedInt8s(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31568,15 +31568,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004027
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class NullableRangeRestrictedInt16u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31584,15 +31584,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004028
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, uint])
 
-            value: 'typing.Union[Nullable, uint]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, uint]' = NullValue
 
         @dataclass
         class NullableRangeRestrictedInt16s(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
 
@@ -31600,15 +31600,15 @@
             def attribute_id(cls) -> int:
                 return 0x00004029
 
             @ChipUtility.classproperty
             def attribute_type(cls) -> ClusterObjectFieldDescriptor:
                 return ClusterObjectFieldDescriptor(Type=typing.Union[Nullable, int])
 
-            value: 'typing.Union[Nullable, int]' = field(default_factory=Nullable)
+            value: 'typing.Union[Nullable, int]' = NullValue
 
         @dataclass
         class WriteOnlyInt8u(ClusterAttributeDescriptor):
             @ChipUtility.classproperty
             def cluster_id(cls) -> int:
                 return 0xFFF1FC05
```

## chip/clusters/Types.py

```diff
@@ -28,9 +28,11 @@
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __lt__(self, other):
         return True
 
+    def __hash__(self):
+        return 0
 
 NullValue = Nullable()
```

## Comparing `home_assistant_chip_clusters-2023.5.1.dist-info/LICENSE` & `home_assistant_chip_clusters-2023.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `home_assistant_chip_clusters-2023.5.1.dist-info/METADATA` & `home_assistant_chip_clusters-2023.5.2.dist-info/METADATA`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: home-assistant-chip-clusters
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Python-base APIs and tools for CHIP.
 Home-page: https://github.com/project-chip/connectedhomeip
 License: Apache
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
+Requires-Dist: aenum
 Requires-Dist: dacite
 
 UNKNOWN
```

## Comparing `home_assistant_chip_clusters-2023.5.1.dist-info/RECORD` & `home_assistant_chip_clusters-2023.5.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 chip/ChipUtility.py,sha256=t3y8WWtYQc5NI8yBrIWeqPN8zPBUnLsxzg8Bm12aUYM,2154
 chip/clusters/CHIPClusters.py,sha256=rEIS3hnjd9nT3c_M3UGibQy_XnWIgI1F0XAz0_NSLW4,314619
 chip/clusters/ClusterObjects.py,sha256=S2Bc0oUe6Wo4OYnlFfT6BB3GaZculvTGVUxkJqq7JAc,12945
-chip/clusters/Objects.py,sha256=u5RSUiFByWuwQx_rnSVxUA7l6V7LJ0c4sGu4wtLzXgM,1300430
+chip/clusters/Objects.py,sha256=yYKeyip-F-PcJUjAaOB41Co2yAtvG9NWr2ik3akFIbM,1296745
 chip/clusters/TestObjects.py,sha256=Az2iQd-H0sN9tXOjLQkzd8nMA5STRFTMButw-8ro5GQ,1947
-chip/clusters/Types.py,sha256=T3ltNCmQox3Z4LafesNkmV0aEfZpmyXANB_EJ9Ac5AE,973
+chip/clusters/Types.py,sha256=sRRy-_Bec3EaXIs1XNXr6qFRqXckn2YAgwvoD4ISjC4,1014
+chip/clusters/enum.py,sha256=zw06GH82ONj3CIHKNI4sr7QnBXEr7vBB6zQnYFVAvYg,2404
 chip/tlv/__init__.py,sha256=SeIN82CcAqgyte0dcbNQwqUJULlUHRmqRMG_0HYowc0,28802
-home_assistant_chip_clusters-2023.5.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-home_assistant_chip_clusters-2023.5.1.dist-info/METADATA,sha256=e5fxqng6ON2SzV_i4tdDn4hKBI3hmbHsDdnlUqX2O0Q,527
-home_assistant_chip_clusters-2023.5.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-home_assistant_chip_clusters-2023.5.1.dist-info/top_level.txt,sha256=5pBsfKK6BMqu66YKYb0-uQqOgrqirLFfcBFAxXDNme0,5
-home_assistant_chip_clusters-2023.5.1.dist-info/RECORD,,
+home_assistant_chip_clusters-2023.5.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+home_assistant_chip_clusters-2023.5.2.dist-info/METADATA,sha256=r6D-z67K6sKCeUbDFk1iHaHQ_KBFZTx2GmXXy-R3MlY,548
+home_assistant_chip_clusters-2023.5.2.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+home_assistant_chip_clusters-2023.5.2.dist-info/top_level.txt,sha256=5pBsfKK6BMqu66YKYb0-uQqOgrqirLFfcBFAxXDNme0,5
+home_assistant_chip_clusters-2023.5.2.dist-info/RECORD,,
```

