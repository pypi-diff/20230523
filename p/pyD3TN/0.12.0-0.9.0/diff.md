# Comparing `tmp/pyD3TN-0.12.0.tar.gz` & `tmp/pyD3TN-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyD3TN-0.12.0.tar", last modified: Tue May 23 11:21:20 2023, max compression
+gzip compressed data, was "dist/pyD3TN-0.9.0.tar", last modified: Thu Nov 19 17:44:30 2020, max compression
```

## Comparing `pyD3TN-0.12.0.tar` & `pyD3TN-0.9.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxr-xr-x   0 fw        (1000) users      (100)        0 2023-05-23 11:21:20.954142 pyD3TN-0.12.0/
--rw-r--r--   0 fw        (1000) users      (100)     1592 2022-01-22 13:20:17.000000 pyD3TN-0.12.0/LICENSE
--rw-r--r--   0 fw        (1000) users      (100)     1404 2023-05-23 11:21:20.954142 pyD3TN-0.12.0/PKG-INFO
--rw-r--r--   0 fw        (1000) users      (100)     1125 2022-01-22 13:20:17.000000 pyD3TN-0.12.0/README.md
-drwxr-xr-x   0 fw        (1000) users      (100)        0 2023-05-23 11:21:20.954142 pyD3TN-0.12.0/pyD3TN.egg-info/
--rw-r--r--   0 fw        (1000) users      (100)     1404 2023-05-23 11:21:20.000000 pyD3TN-0.12.0/pyD3TN.egg-info/PKG-INFO
--rw-r--r--   0 fw        (1000) users      (100)      322 2023-05-23 11:21:20.000000 pyD3TN-0.12.0/pyD3TN.egg-info/SOURCES.txt
--rw-r--r--   0 fw        (1000) users      (100)        1 2023-05-23 11:21:20.000000 pyD3TN-0.12.0/pyD3TN.egg-info/dependency_links.txt
--rw-r--r--   0 fw        (1000) users      (100)        5 2023-05-23 11:21:20.000000 pyD3TN-0.12.0/pyD3TN.egg-info/requires.txt
--rw-r--r--   0 fw        (1000) users      (100)        7 2023-05-23 11:21:20.000000 pyD3TN-0.12.0/pyD3TN.egg-info/top_level.txt
-drwxr-xr-x   0 fw        (1000) users      (100)        0 2023-05-23 11:21:20.954142 pyD3TN-0.12.0/pyd3tn/
--rw-r--r--   0 fw        (1000) users      (100)      217 2022-12-21 15:21:24.000000 pyD3TN-0.12.0/pyd3tn/__init__.py
--rw-r--r--   0 fw        (1000) users      (100)     4039 2022-12-21 15:21:24.000000 pyD3TN-0.12.0/pyd3tn/bundle6.py
--rw-r--r--   0 fw        (1000) users      (100)    31129 2023-05-11 15:05:22.000000 pyD3TN-0.12.0/pyd3tn/bundle7.py
--rw-r--r--   0 fw        (1000) users      (100)    11192 2022-12-21 15:21:24.000000 pyD3TN-0.12.0/pyd3tn/crc.py
--rw-r--r--   0 fw        (1000) users      (100)     1437 2022-12-21 15:21:24.000000 pyD3TN-0.12.0/pyd3tn/helpers.py
--rw-r--r--   0 fw        (1000) users      (100)     3218 2022-12-21 15:21:24.000000 pyD3TN-0.12.0/pyd3tn/mtcp.py
--rw-r--r--   0 fw        (1000) users      (100)     1859 2022-12-21 15:21:24.000000 pyD3TN-0.12.0/pyd3tn/sdnv.py
--rw-r--r--   0 fw        (1000) users      (100)    13610 2022-12-21 15:21:24.000000 pyD3TN-0.12.0/pyd3tn/spp.py
--rw-r--r--   0 fw        (1000) users      (100)    14154 2023-05-12 07:38:56.000000 pyD3TN-0.12.0/pyd3tn/tcpcl.py
--rw-r--r--   0 fw        (1000) users      (100)       38 2023-05-23 11:21:20.954142 pyD3TN-0.12.0/setup.cfg
--rw-r--r--   0 fw        (1000) users      (100)      569 2023-05-23 11:13:23.000000 pyD3TN-0.12.0/setup.py
+drwxr-xr-x   0 fw        (1000) users      (100)        0 2020-11-19 17:44:30.390563 pyD3TN-0.9.0/
+-rw-r--r--   0 fw        (1000) users      (100)     1741 2020-11-19 17:44:30.390563 pyD3TN-0.9.0/PKG-INFO
+-rw-r--r--   0 fw        (1000) users      (100)     1125 2020-11-19 12:00:37.000000 pyD3TN-0.9.0/README.md
+drwxr-xr-x   0 fw        (1000) users      (100)        0 2020-11-19 17:44:30.387230 pyD3TN-0.9.0/pyD3TN.egg-info/
+-rw-r--r--   0 fw        (1000) users      (100)     1741 2020-11-19 17:44:30.000000 pyD3TN-0.9.0/pyD3TN.egg-info/PKG-INFO
+-rw-r--r--   0 fw        (1000) users      (100)      314 2020-11-19 17:44:30.000000 pyD3TN-0.9.0/pyD3TN.egg-info/SOURCES.txt
+-rw-r--r--   0 fw        (1000) users      (100)        1 2020-11-19 17:44:30.000000 pyD3TN-0.9.0/pyD3TN.egg-info/dependency_links.txt
+-rw-r--r--   0 fw        (1000) users      (100)        5 2020-11-19 17:44:30.000000 pyD3TN-0.9.0/pyD3TN.egg-info/requires.txt
+-rw-r--r--   0 fw        (1000) users      (100)        7 2020-11-19 17:44:30.000000 pyD3TN-0.9.0/pyD3TN.egg-info/top_level.txt
+drwxr-xr-x   0 fw        (1000) users      (100)        0 2020-11-19 17:44:30.390563 pyD3TN-0.9.0/pyd3tn/
+-rw-r--r--   0 fw        (1000) users      (100)      163 2020-11-19 12:00:37.000000 pyD3TN-0.9.0/pyd3tn/__init__.py
+-rw-r--r--   0 fw        (1000) users      (100)     3964 2020-11-19 12:00:37.000000 pyD3TN-0.9.0/pyd3tn/bundle6.py
+-rw-r--r--   0 fw        (1000) users      (100)    27872 2020-11-19 12:00:37.000000 pyD3TN-0.9.0/pyd3tn/bundle7.py
+-rw-r--r--   0 fw        (1000) users      (100)    11138 2020-11-19 12:00:37.000000 pyD3TN-0.9.0/pyd3tn/crc.py
+-rw-r--r--   0 fw        (1000) users      (100)     2080 2020-11-19 12:00:37.000000 pyD3TN-0.9.0/pyd3tn/helpers.py
+-rw-r--r--   0 fw        (1000) users      (100)     3164 2020-11-19 12:00:37.000000 pyD3TN-0.9.0/pyd3tn/mtcp.py
+-rw-r--r--   0 fw        (1000) users      (100)     1805 2020-11-19 12:00:37.000000 pyD3TN-0.9.0/pyd3tn/sdnv.py
+-rw-r--r--   0 fw        (1000) users      (100)    13556 2020-11-19 12:00:37.000000 pyD3TN-0.9.0/pyd3tn/spp.py
+-rw-r--r--   0 fw        (1000) users      (100)    14542 2020-11-19 12:00:37.000000 pyD3TN-0.9.0/pyd3tn/tcpcl.py
+-rw-r--r--   0 fw        (1000) users      (100)       38 2020-11-19 17:44:30.390563 pyD3TN-0.9.0/setup.cfg
+-rw-r--r--   0 fw        (1000) users      (100)      514 2020-11-19 17:38:55.000000 pyD3TN-0.9.0/setup.py
```

### Comparing `pyD3TN-0.12.0/PKG-INFO` & `pyD3TN-0.9.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: pyD3TN
-Version: 0.12.0
-Summary: Collection of DTN protocol implementations
-Home-page: https://gitlab.com/d3tn/ud3tn
-Author: D3TN GmbH
-Author-email: contact@d3tn.com
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pyD3TN
 
 pyD3TN is a collection of protocol implementations of the *Delay-Tolerant
 Networking (DTN) Architecture* ([RFC4838][rfc4838]) for Python.
 
 Besides the *Bundle Protocol* implementations [BPv6][bpv6] and [BPv7][bpv7],
 implementations of the *Convergence Layer Adapters* (CLAs) for TCP
```

### Comparing `pyD3TN-0.12.0/pyd3tn/bundle6.py` & `pyD3TN-0.9.0/pyd3tn/bundle6.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-# SPDX-License-Identifier: BSD-3-Clause OR Apache-2.0
 import enum
 import time
 import threading
 
-from .helpers import UNIX_TO_DTN_OFFSET
+from .helpers import unix2dtn
 from .sdnv import sdnv_encode
 
 
 class RFC5050Flag(enum.IntFlag):
     """Default BPv6 flags"""
     IS_FRAGMENT = 0x00001
     ADMINISTRATIVE_RECORD = 0x00002
@@ -94,15 +93,15 @@
         header_part2 += sdnv_encode(cur_dict_offset)
         cur_dict_offset += len(scheme) + 1
         dictionary += ssp + b"\0"
         header_part2 += sdnv_encode(cur_dict_offset)
         cur_dict_offset += len(ssp) + 1
 
     if creation_timestamp is None:
-        creation_timestamp = int(time.time() - UNIX_TO_DTN_OFFSET)
+        creation_timestamp = int(unix2dtn(time.time()))
     header_part2 += sdnv_encode(creation_timestamp)
 
     # If the sequence number is None, the last thread-local sequence number
     # will be used, incremented by one.
     if sequence_number is None:
         sequence_number = next_sequence_number()
     header_part2 += sdnv_encode(sequence_number)
```

### Comparing `pyD3TN-0.12.0/pyd3tn/bundle7.py` & `pyD3TN-0.9.0/pyd3tn/bundle7.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause OR Apache-2.0
 """BPbis bundle Generator
 
 A simple Python package for generating and serialize BPbis bundles into CBOR.
 
 Dependencies:
     This module depends on the ``cbor`` package which can be installed via pip:
 
@@ -14,15 +13,15 @@
 import threading
 from enum import IntEnum, IntFlag
 from datetime import datetime, timezone, timedelta
 from binascii import hexlify
 import cbor  # type: ignore
 from cbor.cbor import CBOR_ARRAY  # type: ignore
 from .crc import crc16_x25, crc32_c
-from .helpers import DTN_EPOCH, UNIX_TO_DTN_OFFSET
+from .helpers import DTN_EPOCH, dtn2unix
 
 
 __all__ = [
     'BundleProcFlag',
     'CRCType',
     'BlockType',
     'BlockProcFlag',
@@ -77,16 +76,14 @@
     DISCARD_IF_UNPROC = 0x02
     REPORT_IF_UNPROC = 0x04
     DELETE_BUNDLE_IF_UNPROC = 0x10
 
 
 class RecordType(IntEnum):
     BUNDLE_STATUS_REPORT = 1
-    BIBE_PROTOCOL_DATA_UNIT = 3
-    BIBE_PROTOCOL_DATA_UNIT_COMPAT = 7
 
 
 class ReasonCode(IntEnum):
     """Bundle status report reason codes"""
     NO_INFO = 0
     LIFETIME_EXPIRDE = 1
     FORWARDED_UNIDIRECTIONAL = 2
@@ -175,72 +172,60 @@
     """BPbis creation timestamp tuple consisting of
 
         (<DTN timestamp>, <sequence number>)
 
     Args:
         time (None, int, datetime.datetime): Timestamp given as Unix timestamp
             (integer) or a Python timezone-aware datetime object. If the time
-            is None, the current time will be used. If the time is 0, no
-            conversion is performed and the DTN timestamp is set to 0.
+            is None, the current time will be used.
         sequence_number (int): Sequence number of the bundle if the device is
             lacking a precise clock
     """
     def __new__(cls, time, sequence_number):
-        if time == 0:
-            return super().__new__(cls, [0, int(sequence_number)])
-
         # Use current datetime
         if time is None:
             time = datetime.now(timezone.utc)
         # Convert Unix timestamp into UTC datetime object
         elif isinstance(time, int) or isinstance(time, float):
             time = datetime.fromtimestamp(time, timezone.utc)
 
         return super().__new__(cls, [
-            int(round((time - DTN_EPOCH).total_seconds() * 1000)),
+            int(round((time - DTN_EPOCH).total_seconds())),
             int(sequence_number),
         ])
 
     @property
     def time(self):
-        """Returns the DTN timestamp value of the CreationTimestamp tuple as
-        datetime object or None if it's 0.
-        """
-        return (
-            None if self[0] == 0
-            else DTN_EPOCH + timedelta(milliseconds=self[0])
-        )
+        return DTN_EPOCH + timedelta(seconds=self[0])
 
     @property
     def sequence_number(self):
         return self[1]
 
     def __repr__(self):
         return "<CreationTimestamp time={} sequence={}>".format(
                     self.time, self.sequence_number)
 
     @staticmethod
     def from_cbor(cbor_data):
         assert len(cbor_data) == 2
-        return CreationTimestamp(
-            cbor_data[0] / 1000 + UNIX_TO_DTN_OFFSET, cbor_data[1]
-        )
+        return CreationTimestamp(dtn2unix(cbor_data[0]), cbor_data[1])
 
 
 class PrimaryBlock(object):
     """The primary bundle block contains the basic information needed to
     forward bundles to their destination.
     """
     def __init__(self, bundle_proc_flags=BundleProcFlag.NONE,
                  crc_type=CRCType.CRC16,
                  destination=None,
                  source=None,
                  report_to=None,
                  creation_time=None,
-                 lifetime=24 * 60 * 60 * 1000,
+                 lifetime=24 * 60 * 60,
                  fragment_offset=None,
                  total_payload_length=None,
                  crc_provided=None):
         self.version = 7
         self.bundle_proc_flags = bundle_proc_flags
         self.crc_type = crc_type
         self.destination = EID(destination)
@@ -275,15 +260,15 @@
             self.version,
             self.bundle_proc_flags,
             self.crc_type,
             self.destination,
             self.source,
             self.report_to,
             self.creation_time,
-            self.lifetime,
+            int(self.lifetime * 1000000),
         ]
 
         # Fragmentation
         if self.has_flag(BundleProcFlag.IS_FRAGMENT):
 
             assert self.fragment_offset is not None, (
                 "Fragment offset must be present for fragmented bundles"
@@ -383,15 +368,15 @@
             crc_type=crc_type,
             destination=EID.from_cbor(cbor_data[3]),
             source=EID.from_cbor(cbor_data[4]),
             report_to=EID.from_cbor(cbor_data[5]),
             creation_time=CreationTimestamp.from_cbor(cbor_data[6]),
             fragment_offset=fragment_offset,
             total_payload_length=total_payload_length,
-            lifetime=(cbor_data[7]),
+            lifetime=(cbor_data[7] / 1000000),
             crc_provided=crc,
         )
 
 
 class CanonicalBlock(object):
     """Canonical bundle block structure"""
     def __init__(self, block_type, data,
@@ -511,20 +496,29 @@
 # ----------------------
 # Administrative Records
 # ----------------------
 
 class AdministrativeRecord(PayloadBlock):
 
     def __init__(self, bundle, record_type_code, record_data):
+        record_data.extend([
+            bundle.primary_block.source,
+            bundle.primary_block.creation_time
+        ])
+
+        if bundle.is_fragmented:
+            record_data.extend([
+                bundle.primary_block.fragment_offset,
+                bundle.primary_block.total_payload_length
+            ])
+
         super().__init__(data=cbor.dumps([
             record_type_code,
             record_data
         ]))
-        self.record_type_code = record_type_code
-        self.record_data = record_data
 
 
 class BundleStatusReport(AdministrativeRecord):
 
     def __init__(self, infos, reason, bundle, time=None):
         status_info = [
             [infos & StatusCode.RECEIVED_BUNDLE != 0],
@@ -539,99 +533,44 @@
             for info in status_info:
                 if info[0]:
                     info.append(int(round((time - DTN_EPOCH).total_seconds())))
 
         record_data = [
             status_info,
             reason,
-            bundle.primary_block.source,
-            bundle.primary_block.creation_time,
         ]
 
-        if bundle.is_fragmented:
-            record_data.extend([
-                bundle.primary_block.fragment_offset,
-                bundle.primary_block.total_payload_length
-            ])
-
         super().__init__(
             bundle,
             record_type_code=RecordType.BUNDLE_STATUS_REPORT,
             record_data=record_data
         )
 
     @property
     def status_info(self):
         return self.data[1][0]
 
     def __repr__(self):
         return "<BundleStatusReport {!r}>".format(self.status_info)
 
 
-class BibeProtocolDataUnit(AdministrativeRecord):
-
-    def __init__(self, bundle, transmission_id=0,
-                 retransmission_time=0, compatibility=False):
-        """Initializes a new BIBE Protocol Data Unit
-
-        Args:
-            bundle (Bundle): The bundle which will be encapsulated in the BPDU.
-            transmission_id (int): If custody is requested the current value of
-                the local node's custodial transmission count, plus 1. Else 0.
-            retransmission_time (DtnTime): If custody is requested the time by
-                which custody disposition for this BPDU is expected. Else 0.
-            compatibility (Bool): Flag for switching the administrative record
-                type code used to 7 for compatibility with older BIBE
-                implementations.
-        """
-        record_data = [transmission_id, retransmission_time, bytes(bundle)]
-        typecode = RecordType.BIBE_PROTOCOL_DATA_UNIT if not compatibility \
-            else RecordType.BIBE_PROTOCOL_DATA_UNIT_COMPAT
-        super().__init__(
-            bundle,
-            record_type_code=typecode,
-            record_data=record_data)
-
-    @staticmethod
-    def parse_bibe_pdu(data):
-        # BIBE PDU has 3 fields
-        assert len(data) == 3
-
-        # Return types:
-        # transmission_id:      int
-        # retransmission_time:  int
-        # encapsulated_bundle:  byte-string
-        return {
-            "transmission_id": data[0],
-            "retransmission_time": data[1],
-            "encapsulated_bundle": data[2]
-        }
-
 # ----------------
 # Extension Blocks
 # ----------------
 
-
 class PreviousNodeBlock(CBORBlock):
 
     def __init__(self, eid, **kwargs):
         super().__init__(BlockType.PREVIOUS_NODE, EID(eid), **kwargs)
 
 
 class BundleAgeBlock(CBORBlock):
-    """The Bundle Age block, block type 7, contains the number of milliseconds
-    that have elapsed between the time the bundle was created and time at which
-    it was most recently forwarded.
-
-    Args:
-        age (int): Age value in seconds
-    """
 
     def __init__(self, age, **kwargs):
-        super().__init__(BlockType.BUNDLE_AGE, int(age * 1000), **kwargs)
+        super().__init__(BlockType.BUNDLE_AGE, int(age * 1000000), **kwargs)
 
 
 class HopCountBlock(CBORBlock):
 
     def __init__(self, hop_limit, hop_count, **kwargs):
         super().__init__(BlockType.HOP_COUNT, (hop_limit, hop_count), **kwargs)
 
@@ -698,20 +637,14 @@
     ..code:: python
 
         for i, block in enumerate(bundle):
             if i == 0:
                 assert isinstance(block, PrimaryBlock)
     """
     def __init__(self, primary_block, payload_block, blocks=None):
-        assert (
-            primary_block.creation_time.time or
-            blocks and
-            any(b.block_type == BlockType.BUNDLE_AGE for b in blocks)
-        ), "There must be a 'Bundle Age' block if the creation time is 0"
-
         self.primary_block = primary_block
         self.payload_block = payload_block
         self.blocks = []
 
         if blocks:
             for block in blocks:
                 self.add(block)
@@ -744,17 +677,23 @@
                 # Hop Count
                 elif block.block_type == BlockType.HOP_COUNT:
                     raise ValueError(
                         "There must be only one 'Hop Count' block"
                     )
                 # Bundle Age
                 elif block.block_type == BlockType.BUNDLE_AGE:
-                    raise ValueError(
-                        "There must be only one 'Bundle Age' block"
+                    creation_time, _ = self.primary_block.creation_time
+                    creation_time_dtn = int(
+                        round((creation_time - DTN_EPOCH).total_seconds())
                     )
+                    if creation_time_dtn == 0:
+                        raise ValueError(
+                            "There must be only one 'Bundle Age' block "
+                            "if the bundle creation time is 0"
+                        )
 
         if new_block.block_number is None:
             new_block.block_number = num + 1
 
         # Previous Node blocks must be the first blocks after the primary block
         if new_block.block_type == BlockType.PREVIOUS_NODE:
             self.blocks.insert(0, new_block)
@@ -795,37 +734,14 @@
         # At least a primary and a payload block are required
         assert len(cbor_data) >= 2
         primary_block = PrimaryBlock.from_cbor(cbor_data[0])
         payload_block = PayloadBlock.from_cbor(cbor_data[-1])
         blocks = [CanonicalBlock.from_cbor(e) for e in cbor_data[1:-1]]
         return Bundle(primary_block, payload_block, blocks)
 
-    @staticmethod
-    def parse_administrative_record(data):
-        """Function for parsing administrative records of different types
-
-        Args:
-            data (CBOR bytestring): The encoded bundle
-
-        Returns:
-           dict: If the type of the AR is known, a dict containing the fields
-           record_type and record_data is returned. Else returns an empty dict.
-        """
-        record_data = cbor.loads(data)
-        record_type = record_data[0]
-
-        if record_type == RecordType.BUNDLE_STATUS_REPORT:
-            pass
-        elif (record_type == RecordType.BIBE_PROTOCOL_DATA_UNIT or
-              record_type == RecordType.BIBE_PROTOCOL_DATA_UNIT_COMPAT):
-            bpdu = BibeProtocolDataUnit.parse_bibe_pdu(record_data[1])
-            return {"record_type": record_type, "record_data": bpdu}
-
-        return {}
-
 
 _th_local = threading.local()
 
 
 def next_sequence_number():
     seqnum = _th_local.__dict__.get("seqnum", 0)
     _th_local.__dict__["seqnum"] = seqnum + 1
@@ -837,15 +753,15 @@
 
 
 def create_bundle7(source_eid, destination_eid, payload,
                    report_to_eid=None, crc_type_primary=CRCType.CRC32,
                    creation_timestamp=None, sequence_number=None,
                    lifetime=300, flags=BlockProcFlag.NONE,
                    fragment_offset=None, total_adu_length=None,
-                   hop_limit=None, hop_count=0, bundle_age=None,
+                   hop_limit=30, hop_count=0, bundle_age=0,
                    previous_node_eid=None,
                    crc_type_canonical=CRCType.CRC16):
     """All-in-one function to encode a payload from a source EID
     to a destination EID as BPbis bundle.
 
     Args:
         source_eid (EID, str): Source endpoint address
@@ -877,62 +793,64 @@
         bundle_age (int, optional): Age of the bundle in seconds
         previous_node_eid (EID, str, optional): Address of the previous
             endpoint the bundle was received from Returns: bytes: CBOR encoded
             BPbis bundle
         crc_type_canonical (CRCType, optional): The kind of CRC used for the
             canonical blocks.
     """
-    blocks = []
-
-    if hop_limit is not None and hop_count is not None:
-        blocks.append(
-            HopCountBlock(hop_limit, hop_count, crc_type=crc_type_canonical)
-        )
-    if previous_node_eid is not None:
-        blocks.append(
-            PreviousNodeBlock(previous_node_eid, crc_type=crc_type_canonical)
-        )
-    if bundle_age is not None:
-        blocks.append(
-            BundleAgeBlock(bundle_age, crc_type=crc_type_canonical)
-        )
-
-    return Bundle(
+    bundle = Bundle(
         PrimaryBlock(
             bundle_proc_flags=flags,
             crc_type=crc_type_primary,
             destination=destination_eid,
             source=source_eid,
             report_to=report_to_eid,
             creation_time=CreationTimestamp(
                 creation_timestamp,
                 (
                     sequence_number
                     if sequence_number is not None
                     else next_sequence_number()
                 ),
             ),
-            lifetime=lifetime * 1000,
+            lifetime=lifetime,
             fragment_offset=fragment_offset,
             total_payload_length=total_adu_length,
         ),
         PayloadBlock(
             payload,
             crc_type=crc_type_canonical,
         ),
-        blocks,
     )
 
+    if previous_node_eid is not None:
+        bundle.add(PreviousNodeBlock(
+            previous_node_eid,
+            crc_type=crc_type_canonical,
+        ))
+
+    bundle.add(HopCountBlock(
+        hop_limit,
+        hop_count,
+        crc_type=crc_type_canonical,
+    ))
+    bundle.add(BundleAgeBlock(
+        bundle_age,
+        crc_type=crc_type_canonical,
+    ))
+
+    return bundle
+
 
 def serialize_bundle7(source_eid, destination_eid, payload,
                       report_to_eid=None, crc_type_primary=CRCType.CRC32,
                       creation_timestamp=None, sequence_number=None,
                       lifetime=300, flags=BlockProcFlag.NONE,
                       fragment_offset=None, total_adu_length=None,
-                      hop_limit=None, hop_count=0, bundle_age=None,
+                      hop_limit=30, hop_count=0, bundle_age=0,
                       previous_node_eid=None,
                       crc_type_canonical=CRCType.CRC16):
     """All-in-one function to encode a payload from a source EID
     to a destination EID as BPbis bundle.
     See create_bundle7 for a description of options."""
     return bytes(create_bundle7(
         source_eid, destination_eid, payload,
```

### Comparing `pyD3TN-0.12.0/pyd3tn/crc.py` & `pyD3TN-0.9.0/pyd3tn/crc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause OR Apache-2.0
 """Generic CRC implementation with many pre-defined CRC models.
 
 This module is the adopted Python implementation of the JavaScript CRC
 implementation by Bastian Molkenthin:
 
     http://www.sunshine2k.de/coding/javascript/crc/crc_js.html
```

### Comparing `pyD3TN-0.12.0/pyd3tn/mtcp.py` & `pyD3TN-0.9.0/pyd3tn/mtcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause OR Apache-2.0
 import socket
 import logging
 
 import cbor
 
 from .helpers import sock_recv_raw
```

### Comparing `pyD3TN-0.12.0/pyd3tn/sdnv.py` & `pyD3TN-0.9.0/pyd3tn/sdnv.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause OR Apache-2.0
 """Self-Delimiting Numeric Values (RFC 6256)"""
 
 
 def sdnv_encode(value):
     """Returns the SDNV-encoded byte string representing value
 
     Args:
```

### Comparing `pyD3TN-0.12.0/pyd3tn/spp.py` & `pyD3TN-0.9.0/pyd3tn/spp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause OR Apache-2.0
 import enum
 import struct
 import socket
 import logging
 from datetime import datetime, timedelta, timezone
 
 from .crc import crc16_ccitt_false
```

### Comparing `pyD3TN-0.12.0/pyd3tn/tcpcl.py` & `pyD3TN-0.9.0/pyd3tn/tcpcl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# SPDX-License-Identifier: BSD-3-Clause OR Apache-2.0
 import enum
 import struct
 import socket
 import logging
 import asyncio
 
 from .sdnv import sdnv_encode, sdnv_decode
@@ -77,15 +76,15 @@
     The connection supports the context manager protocol to ensure a proper
     shutdown of the connection in case of any error:
 
     .. code:: python
 
         from pyd3tn.tcpcl import TCPCLConnection
 
-        with TCPCLConnection('dtn://my-eid.dtn/', '127.0.0.1', 4223) as conn:
+        with TCPCLConnection('dtn://my-eid.dtn', '127.0.0.1', 4223) as conn:
             conn.send(bundle)
 
     Args:
         eid (str): Endpoint identifier for this DTN node
         host (str): Host to connect to
         port (int): TCP port to connect to
         timeout (float): Timeout for receiving bundles (None for infinite)
@@ -180,19 +179,23 @@
         async with AsyncTCPCLConnection(me) as conn:
             conn.bind('127.0.0.1', 42421)
             await conn.connect()
             await conn.send(bundle)
 
     Args:
         eid (str): Endpoint identifier for this DTN node
+        loop (asyncio.AbstractEventLoop, optional): Event loop that should be
+            used. If not given the default :func:`asyncio.get_event_loop` will
+            be used.
     """
 
-    def __init__(self, eid):
+    def __init__(self, eid, loop=None):
         super().__init__(eid)
 
+        self.loop = loop or asyncio.get_event_loop()
         self.reader = None
         self.writer = None
 
     async def __aenter__(self):
         self.__enter__()
         self.sock.setblocking(False)
         return self
@@ -201,22 +204,21 @@
         """Async variant of :meth:`TCPCLConnection.connect`. The interface is
         identical, except that this function is a coroutine and has the be
         awaited.
         """
         if not self.sock:
             return
 
-        loop = asyncio.get_event_loop()
         # Establish TCP connection
-        await loop.sock_connect(
+        await self.loop.sock_connect(
             self.sock, (host, port)
         )
         # Create stream reader and writer pair
         self.reader, self.writer = await asyncio.open_connection(
-            sock=self.sock
+            sock=self.sock, loop=self.loop
         )
         logger.debug("TCPCL: Connected to %s:%d", host, port)
 
         # Send TCPCL contact header with own EID
         logger.debug("TCPCL: Send header for %r", self.eid)
         self.writer.write(serialize_tcpcl_contact_header(self.eid))
         await self.writer.drain()
@@ -267,45 +269,49 @@
 
     .. code:: python
 
         import asyncio
         from pyd3tn.tcpcl import TCPCLServer
 
         async def listen():
-            async with TCPCLServer('dtn://me/', '127.0.0.1', 42420) as server:
+            async with TCPCLServer('dtn:me', '127.0.0.1', 42420) as server:
                 # do some other cool stuff here while the server is running in
                 # the background ... or just wait for the server to finish
                 await server.wait_closed()
 
         loop = asyncio.get_event_loop()
         loop.run_until_complete(listen())
 
     Args:
         eid (str): The endpoint identifier (EID) that is used for this DTN node
         host (str): Hostname / IP address the server should listening on
         port (int): TCP port number the server should listenin on
         backlog (int, optional): Number of concurrent TCP connections
+        loop (asyncio.AbstractEventLoop, optional): Event loop that should be
+            used. If not given the default :func:`asyncio.get_event_loop` will
+            be used.
     """
 
-    def __init__(self, eid, host, port, backlog=100):
+    def __init__(self, eid, host, port, backlog=100, loop=None):
         self.eid = eid
         self.host = host
         self.port = port
         self.backlog = backlog
         self.server = None
         self.handlers = []
+        self.loop = loop or asyncio.get_event_loop()
 
     async def start(self):
         """Start listening on the specified host and port"""
         if self.server:
             return
 
         self.server = await asyncio.start_server(
             self.client_connected, host=self.host, port=self.port,
-            backlog=self.backlog
+            backlog=self.backlog, loop=self.loop
         )
         logger.debug("TCPCLServer: Listening on %s:%d", self.host, self.port)
 
     def close(self):
         """Terminate all open connections and close the listening socket"""
         if not self.server:
             return
@@ -339,16 +345,15 @@
             writer (asyncio.StreamWriter): Writer for the underlying TCP
                 connection
         """
         # We create an extra task for handling the connection because we want
         # to be able to cancel them. A call to "self.server.close()" would stop
         # this coroutine without any exception. Hence we have no possibility to
         # shutdown the TCPCL connection properly in this coroutine.
-        loop = asyncio.get_event_loop()
-        task = loop.create_task(self.handle_connection(reader, writer))
+        task = self.loop.create_task(self.handle_connection(reader, writer))
         task.add_done_callback(lambda task: self.handlers.remove(task))
         self.handlers.append(task)
 
     async def handle_connection(self, reader, writer):
         """This method is executed for each new connection is a separate
         asyncio task. It sends and receives the TCPCL contact header and then
         receives messages and forwards them to the :meth:`received_message`
```

### Comparing `pyD3TN-0.12.0/setup.py` & `pyD3TN-0.9.0/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python
-# SPDX-License-Identifier: BSD-3-Clause OR Apache-2.0
 
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name='pyD3TN',
-    version='0.12.0',
+    version='0.9.0',
     author='D3TN GmbH',
     author_email='contact@d3tn.com',
     description='Collection of DTN protocol implementations',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://gitlab.com/d3tn/ud3tn',
     packages=['pyd3tn'],
```

