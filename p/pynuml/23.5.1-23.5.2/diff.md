# Comparing `tmp/pynuml-23.5.1.tar.gz` & `tmp/pynuml-23.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynuml-23.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pynuml-23.5.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pynuml-23.5.1.tar` & `pynuml-23.5.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       17 2022-08-22 18:40:35.802435 pynuml-23.5.1/.gitignore
--rw-r--r--   0        0        0     1074 2023-05-19 17:54:50.911108 pynuml-23.5.1/LICENSE
--rw-r--r--   0        0        0     5647 2023-05-17 21:45:54.952303 pynuml-23.5.1/README.md
--rw-r--r--   0        0        0      170 2022-08-22 18:40:35.802435 pynuml-23.5.1/doc/README.md
--rw-r--r--   0        0        0     9267 2022-08-22 18:40:35.802435 pynuml-23.5.1/doc/graph_create.md
--rw-r--r--   0        0        0     2903 2022-08-22 18:40:35.802435 pynuml-23.5.1/doc/python_env.md
--rw-r--r--   0        0        0      638 2023-04-03 15:38:40.928784 pynuml-23.5.1/docs/Makefile
--rw-r--r--   0        0        0      804 2023-04-03 15:38:40.932784 pynuml-23.5.1/docs/make.bat
--rw-r--r--   0        0        0      916 2023-04-03 15:38:40.932784 pynuml-23.5.1/docs/source/conf.py
--rw-r--r--   0        0        0      671 2023-04-03 15:38:40.932784 pynuml-23.5.1/docs/source/index.rst
--rw-r--r--   0        0        0      581 2022-08-22 15:18:00.634737 pynuml-23.5.1/example/plot.py
--rwxr-xr-x   0        0        0     2089 2022-11-15 22:26:27.438225 pynuml-23.5.1/example/process.py
--rw-r--r--   0        0        0     1169 2022-08-22 18:40:35.802435 pynuml-23.5.1/h5merge.py
--rw-r--r--   0        0        0       38 2022-11-15 18:40:24.677584 pynuml-23.5.1/pynuml/.gitignore
--rw-r--r--   0        0        0      164 2023-05-19 19:12:57.703058 pynuml-23.5.1/pynuml/__init__.py
--rw-r--r--   0        0        0       97 2023-05-19 18:59:36.039498 pynuml-23.5.1/pynuml/io/__init__.py
--rw-r--r--   0        0        0    33686 2023-05-17 21:45:54.952303 pynuml-23.5.1/pynuml/io/file.py
--rw-r--r--   0        0        0     3290 2023-05-17 21:45:54.952303 pynuml-23.5.1/pynuml/io/h5interface.py
--rw-r--r--   0        0        0     4083 2023-05-17 21:45:54.952303 pynuml-23.5.1/pynuml/io/out.py
--rw-r--r--   0        0        0       69 2023-03-07 20:27:07.502862 pynuml-23.5.1/pynuml/labels/__init__.py
--rw-r--r--   0        0        0     1476 2022-11-15 18:40:24.677584 pynuml-23.5.1/pynuml/labels/ccqe.py
--rw-r--r--   0        0        0      779 2023-03-07 20:27:07.502862 pynuml-23.5.1/pynuml/labels/simple.py
--rw-r--r--   0        0        0    10532 2023-05-19 19:00:00.405738 pynuml-23.5.1/pynuml/labels/standard.py
--rw-r--r--   0        0        0       28 2023-03-15 20:32:17.479263 pynuml-23.5.1/pynuml/plot/__init__.py
--rw-r--r--   0        0        0     5246 2023-05-17 21:45:54.952303 pynuml-23.5.1/pynuml/plot/graph.py
--rw-r--r--   0        0        0       39 2023-02-28 00:57:35.995625 pynuml-23.5.1/pynuml/process/__init__.py
--rw-r--r--   0        0        0      463 2023-02-28 00:57:35.995625 pynuml-23.5.1/pynuml/process/base.py
--rw-r--r--   0        0        0     6095 2023-05-17 21:54:36.098985 pynuml-23.5.1/pynuml/process/hitgraph.py
--rw-r--r--   0        0        0     3780 2022-11-15 18:40:24.677584 pynuml-23.5.1/pynuml/process/spmap.py
--rw-r--r--   0        0        0      585 2023-05-19 19:08:37.474232 pynuml-23.5.1/pyproject.toml
--rw-r--r--   0        0        0     6181 1970-01-01 00:00:00.000000 pynuml-23.5.1/PKG-INFO
+-rw-r--r--   0        0        0       17 2022-08-22 18:40:35.802435 pynuml-23.5.2/.gitignore
+-rw-r--r--   0        0        0     1074 2023-05-22 19:32:38.886857 pynuml-23.5.2/LICENSE
+-rw-r--r--   0        0        0     5647 2023-05-22 19:32:38.886857 pynuml-23.5.2/README.md
+-rw-r--r--   0        0        0      170 2022-08-22 18:40:35.802435 pynuml-23.5.2/doc/README.md
+-rw-r--r--   0        0        0     9267 2022-08-22 18:40:35.802435 pynuml-23.5.2/doc/graph_create.md
+-rw-r--r--   0        0        0     2903 2022-08-22 18:40:35.802435 pynuml-23.5.2/doc/python_env.md
+-rw-r--r--   0        0        0      638 2023-05-22 19:32:38.886857 pynuml-23.5.2/docs/Makefile
+-rw-r--r--   0        0        0      804 2023-05-22 19:32:38.886857 pynuml-23.5.2/docs/make.bat
+-rw-r--r--   0        0        0      916 2023-05-22 19:32:38.886857 pynuml-23.5.2/docs/source/conf.py
+-rw-r--r--   0        0        0      671 2023-05-22 19:32:38.886857 pynuml-23.5.2/docs/source/index.rst
+-rw-r--r--   0        0        0      581 2022-08-22 15:18:00.634737 pynuml-23.5.2/example/plot.py
+-rwxr-xr-x   0        0        0     2089 2022-11-15 22:26:27.438225 pynuml-23.5.2/example/process.py
+-rw-r--r--   0        0        0     1169 2022-08-22 18:40:35.802435 pynuml-23.5.2/h5merge.py
+-rw-r--r--   0        0        0       38 2022-11-15 18:40:24.677584 pynuml-23.5.2/pynuml/.gitignore
+-rw-r--r--   0        0        0      164 2023-05-23 15:12:32.529985 pynuml-23.5.2/pynuml/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-19 18:59:36.039498 pynuml-23.5.2/pynuml/io/__init__.py
+-rw-r--r--   0        0        0    33647 2023-05-23 15:09:52.742521 pynuml-23.5.2/pynuml/io/file.py
+-rw-r--r--   0        0        0     3290 2023-05-22 19:32:38.886857 pynuml-23.5.2/pynuml/io/h5interface.py
+-rw-r--r--   0        0        0     4089 2023-05-23 15:09:52.742521 pynuml-23.5.2/pynuml/io/out.py
+-rw-r--r--   0        0        0       69 2023-05-22 19:32:38.890858 pynuml-23.5.2/pynuml/labels/__init__.py
+-rw-r--r--   0        0        0     1476 2022-11-15 18:40:24.677584 pynuml-23.5.2/pynuml/labels/ccqe.py
+-rw-r--r--   0        0        0      779 2023-05-22 19:32:38.890858 pynuml-23.5.2/pynuml/labels/simple.py
+-rw-r--r--   0        0        0    10392 2023-05-22 19:52:38.317160 pynuml-23.5.2/pynuml/labels/standard.py
+-rw-r--r--   0        0        0       28 2023-05-22 19:32:38.890858 pynuml-23.5.2/pynuml/plot/__init__.py
+-rw-r--r--   0        0        0     5246 2023-05-22 19:32:38.890858 pynuml-23.5.2/pynuml/plot/graph.py
+-rw-r--r--   0        0        0       39 2023-02-28 00:57:35.995625 pynuml-23.5.2/pynuml/process/__init__.py
+-rw-r--r--   0        0        0      463 2023-02-28 00:57:35.995625 pynuml-23.5.2/pynuml/process/base.py
+-rw-r--r--   0        0        0     6105 2023-05-23 15:09:52.742521 pynuml-23.5.2/pynuml/process/hitgraph.py
+-rw-r--r--   0        0        0     3780 2022-11-15 18:40:24.677584 pynuml-23.5.2/pynuml/process/spmap.py
+-rw-r--r--   0        0        0      585 2023-05-22 19:32:38.890858 pynuml-23.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6181 1970-01-01 00:00:00.000000 pynuml-23.5.2/PKG-INFO
```

### Comparing `pynuml-23.5.1/LICENSE` & `pynuml-23.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/README.md` & `pynuml-23.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/doc/graph_create.md` & `pynuml-23.5.2/doc/graph_create.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/doc/python_env.md` & `pynuml-23.5.2/doc/python_env.md`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/docs/Makefile` & `pynuml-23.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/docs/make.bat` & `pynuml-23.5.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/docs/source/conf.py` & `pynuml-23.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/docs/source/index.rst` & `pynuml-23.5.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/example/plot.py` & `pynuml-23.5.2/example/plot.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/example/process.py` & `pynuml-23.5.2/example/process.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/h5merge.py` & `pynuml-23.5.2/h5merge.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/pynuml/io/file.py` & `pynuml-23.5.2/pynuml/io/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,16 +250,16 @@
         # self._my_start: (== self._starts[rank]) this process's start
         # self._my_count: (== self._counts[rank]) this process's count
         # self._my_index: partitioned dataset i.e. assigned to this process
 
         comm = MPI.COMM_WORLD
         rank = comm.Get_rank()
         nprocs = comm.Get_size()
-        self._starts = np.zeros(nprocs, dtype=np.int)
-        self._counts = np.zeros(nprocs, dtype=np.int)
+        self._starts = np.zeros(nprocs, dtype=int)
+        self._counts = np.zeros(nprocs, dtype=int)
 
         if rank == 0:
             if self._use_seq_cnt:
                 self.read_seq_cnt()
             else:
                 self.read_seq()
 
@@ -279,15 +279,15 @@
 
             elif self._evt_part == 1:
                 # event amount based partitioning, which calculates event sizes
                 # across all groups. Note it is possible multiple consecutive rows
                 # a dataset have the same event ID. It is also possible some event
                 # IDs contain no data. First, we accumulate numbers of events
                 # across all groups
-                evt_size = np.zeros(num_events, dtype=np.int)
+                evt_size = np.zeros(num_events, dtype=int)
                 if self._use_seq_cnt:
                     for group, datasets in self._groups:
                         seq_cnt = self._whole_seq_cnt[group]
                         num_datasets = len(datasets)
                         for i in range(seq_cnt.shape[0]):
                             evt_size[seq_cnt[i, 0]] += seq_cnt[i, 1] * num_datasets
                 else:
@@ -357,18 +357,18 @@
                         acc_evt_num += seq_cnt[j, 1]
 
                 self._counts[nprocs-1] = num_events - self._starts[nprocs-1]
 
         # All processes participate the collective communication, scatter.
         # Root distributes start and count to all processes. Note only root process
         # uses self._starts and self._counts.
-        start_count = np.empty([nprocs, 2], dtype=np.int)
+        start_count = np.empty([nprocs, 2], dtype=int)
         start_count[:, 0] = self._starts[:]
         start_count[:, 1] = self._counts[:]
-        recvbuf = np.empty(2, dtype=np.int)
+        recvbuf = np.empty(2, dtype=int)
         comm.Scatter(start_count, recvbuf, root=0)
         self._my_start = recvbuf[0]
         self._my_count = recvbuf[1]
 
         # This process is assigned event IDs of range from self._my_start to
         # (self._my_start + self._my_count - 1)
         # print("my_start=",self._my_start," my_count=",self._my_count);
@@ -403,17 +403,17 @@
         # return the lower and upper array indices of subarray assigned to this
         # process, using the partition sequence dataset
 
         comm = MPI.COMM_WORLD
         rank = comm.Get_rank()
         nprocs = comm.Get_size()
 
-        displ  = np.zeros([nprocs], dtype=np.int)
-        count  = np.zeros([nprocs], dtype=np.int)
-        bounds = np.zeros([nprocs, 2], dtype=np.int)
+        displ  = np.zeros([nprocs], dtype=int)
+        count  = np.zeros([nprocs], dtype=int)
+        bounds = np.zeros([nprocs, 2], dtype=int)
 
         all_evt_seq = None
         if rank == 0:
             # root reads the entire dataset self._seq_name, if not already
             if not self._whole_seq: self.read_seq()
 
             all_evt_seq = self._whole_seq[group]
@@ -424,15 +424,15 @@
                 if self._counts[i] == 0: continue
                 end = self._starts[i] + self._counts[i] - 1
                 bounds[i, 0] = self.binary_search_min(self._starts[i], all_evt_seq, dim)
                 bounds[i, 1] = self.binary_search_max(end,             all_evt_seq, dim)
                 displ[i] = bounds[i, 0]
                 count[i] = bounds[i, 1] - bounds[i, 0] + 1
 
-        lower_upper = np.empty([2], dtype=np.int)
+        lower_upper = np.empty([2], dtype=int)
 
         # root distributes start and end indices to all processes
         comm.Scatter(bounds, lower_upper, root=0)
 
         # this process is assigned array indices from lower to upper
         # print("group=",group," lower=",lower," upper=",upper," count=",upper-lower)
 
@@ -452,17 +452,17 @@
         # return the lower and upper array indices of subarray assigned to this
         # process, using the partition sequence-count dataset
 
         comm   = MPI.COMM_WORLD
         rank   = comm.Get_rank()
         nprocs = comm.Get_size()
 
-        displ   = np.zeros([nprocs], dtype=np.int)
-        count   = np.zeros([nprocs], dtype=np.int)
-        seq_cnt = np.zeros([nprocs, 2], dtype=np.int)
+        displ   = np.zeros([nprocs], dtype=int)
+        count   = np.zeros([nprocs], dtype=int)
+        seq_cnt = np.zeros([nprocs, 2], dtype=int)
 
         all_seq_cnt = None
         if rank == 0:
             # root reads the entire dataset self._cnt_name, if not already
             if not self._whole_seq_cnt: self.read_seq_cnt()
 
             all_seq_cnt = self._whole_seq_cnt[group]
@@ -487,15 +487,15 @@
             seq_cnt[recv_rank, 1] = dim - displ[recv_rank]
 
             # print("starts=",self._starts," counts=",self._counts," displ=",displ," count=",count," seq_cnt=",seq_cnt )
             displ[:] *= 2
             count[:] = seq_cnt[:, 1] * 2
 
         # root distributes seq_cnt to all processes
-        my_seq_cnt = np.empty([2], dtype=np.int)
+        my_seq_cnt = np.empty([2], dtype=int)
         comm.Scatter(seq_cnt, my_seq_cnt, root=0)
 
         # self._seq_cnt[group][:, 0] is the event ID
         # self._seq_cnt[group][:, 1] is the number of elements
         self._seq_cnt[group] = np.empty([my_seq_cnt[1], 2], dtype=np.int64)
 
         # root scatters the subarray of evt_seq to all processes
```

### Comparing `pynuml-23.5.1/pynuml/io/h5interface.py` & `pynuml-23.5.2/pynuml/io/h5interface.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/pynuml/io/out.py` & `pynuml-23.5.2/pynuml/io/out.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,13 +92,13 @@
                     field = (key, val.dtype, val.shape)
             fields.append(field)
         ctype = np.dtype(fields)
         # create a scalar dataset of compound data type
         ds = self.f.create_dataset(f"/{name}", shape=(), dtype=ctype, data=data)
         del ctype, fields, data, ds
 
-    def write_metadata(metadata: dict[str, Any]) -> None:
+    def write_metadata(self, metadata: dict[str, Any]) -> None:
         for key, val in metadata.items():
             self.f[key] = val
 
     def __del__(self):
         if self.f != None: self.f.close()
```

### Comparing `pynuml-23.5.1/pynuml/labels/ccqe.py` & `pynuml-23.5.2/pynuml/labels/ccqe.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/pynuml/labels/simple.py` & `pynuml-23.5.2/pynuml/labels/simple.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/pynuml/labels/standard.py` & `pynuml-23.5.2/pynuml/labels/standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,18 +108,14 @@
                         sl = self.shower
                         slc = self.shower
                     elif abs(parent_type) == 13 and (part.start_process == 'muMinusCaptureAtRest' \
                         or part.start_process == 'muPlusCaptureAtRest' or part.start_process == 'Decay'):
                         sl = self.michel
                         slc = self.michel
 
-                    elif part.end_process == 'eIoni':
-                        sl = self.diffuse
-                        slc = self.diffuse
-
                     elif part.start_process == 'conv' or part.end_process == 'conv' \
                         or part.start_process == 'compt' or part.end_process == 'compt':
                         if part.momentum >= self._gamma_threshold:
                             sl = self.shower
                             slc = self.shower
                         else:
                             sl = self.diffuse
```

### Comparing `pynuml-23.5.1/pynuml/plot/graph.py` & `pynuml-23.5.2/pynuml/plot/graph.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/pynuml/process/hitgraph.py` & `pynuml-23.5.2/pynuml/process/hitgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             groups['particle_table'] = ['g4_id','parent_id','type','momentum','start_process','end_process']
             groups['edep_table'] = []
         return groups
 
     @property
     def metadata(self):
         metadata = { 'planes': self.planes }
-        if laleller is not None:
-            metadata['classes'] = labeller.labels[:-1]
+        if self.labeller is not None:
+            metadata['classes'] = self.labeller.labels[:-1]
         return metadata
 
     def __call__(self, evt: 'pynuml.io.Event') -> tuple[str, Any]:
 
         event_id = evt.event_id
         name = f'r{event_id[0]}_sr{event_id[1]}_evt{event_id[2]}'
```

### Comparing `pynuml-23.5.1/pynuml/process/spmap.py` & `pynuml-23.5.2/pynuml/process/spmap.py`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/pyproject.toml` & `pynuml-23.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynuml-23.5.1/PKG-INFO` & `pynuml-23.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynuml
-Version: 23.5.1
+Version: 23.5.2
 Summary: Standardised ML input processing for particle physics
 Author-email: v hewes <vhewes@fnal.gov>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: h5py>=3.7.0
```

