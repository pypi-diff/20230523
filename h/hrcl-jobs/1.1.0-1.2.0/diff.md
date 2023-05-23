# Comparing `tmp/hrcl_jobs-1.1.0.tar.gz` & `tmp/hrcl_jobs-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hrcl_jobs-1.1.0.tar", last modified: Thu May 18 20:02:07 2023, max compression
+gzip compressed data, was "hrcl_jobs-1.2.0.tar", last modified: Tue May 23 15:42:36 2023, max compression
```

## Comparing `hrcl_jobs-1.1.0.tar` & `hrcl_jobs-1.2.0.tar`

### file list

```diff
@@ -1,35 +1,33 @@
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.095466 hrcl_jobs-1.1.0/
--rw-r--r--   0 austinwallace   (501) staff       (20)     1803 2023-02-02 20:22:41.000000 hrcl_jobs-1.1.0/.gitignore
--rw-r--r--   0 austinwallace   (501) staff       (20)     1074 2023-02-02 20:22:41.000000 hrcl_jobs-1.1.0/LICENSE
--rw-r--r--   0 austinwallace   (501) staff       (20)      962 2023-05-18 20:02:07.095976 hrcl_jobs-1.1.0/PKG-INFO
--rw-r--r--   0 austinwallace   (501) staff       (20)      342 2023-02-03 23:39:01.000000 hrcl_jobs-1.1.0/README.md
--rw-r--r--   0 austinwallace   (501) staff       (20)      116 2023-03-27 20:06:21.000000 hrcl_jobs-1.1.0/main.py
--rw-r--r--   0 austinwallace   (501) staff       (20)      665 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/pyproject.toml
--rw-r--r--   0 austinwallace   (501) staff       (20)      295 2023-05-18 20:02:07.097950 hrcl_jobs-1.1.0/setup.cfg
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.081689 hrcl_jobs-1.1.0/src/
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.088929 hrcl_jobs-1.1.0/src/hrcl_jobs/
--rw-r--r--   0 austinwallace   (501) staff       (20)      128 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/__init__.py
--rw-r--r--   0 austinwallace   (501) staff       (20)    14403 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/data.py
--rw-r--r--   0 austinwallace   (501) staff       (20)      968 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/examples.py
--rw-r--r--   0 austinwallace   (501) staff       (20)      893 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/jobspec.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     5861 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/parallel.py
--rw-r--r--   0 austinwallace   (501) staff       (20)    20138 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/s22.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     2093 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/serial.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     9082 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/setup.py
--rw-r--r--   0 austinwallace   (501) staff       (20)    19958 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/sqlt.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     2929 2023-03-27 20:06:21.000000 hrcl_jobs-1.1.0/src/hrcl_jobs/tools_og.py
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.091304 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/
--rw-r--r--   0 austinwallace   (501) staff       (20)      962 2023-05-18 20:02:07.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/PKG-INFO
--rw-r--r--   0 austinwallace   (501) staff       (20)      704 2023-05-18 20:02:07.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-05-18 20:02:07.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)       69 2023-05-18 20:02:07.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/requires.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)       40 2023-05-18 20:02:07.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/top_level.txt
--rw-r--r--   0 austinwallace   (501) staff       (20)        1 2023-02-02 20:26:18.000000 hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/zip-safe
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.093088 hrcl_jobs-1.1.0/src/hrcl_jobs_orca/
--rw-r--r--   0 austinwallace   (501) staff       (20)       24 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_orca/__init__.py
--rw-r--r--   0 austinwallace   (501) staff       (20)      629 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_orca/jobspec.py
--rw-r--r--   0 austinwallace   (501) staff       (20)     2463 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_orca/orca_inps.py
-drwxr-xr-x   0 austinwallace   (501) staff       (20)        0 2023-05-18 20:02:07.094719 hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/
--rw-r--r--   0 austinwallace   (501) staff       (20)       24 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/__init__.py
--rw-r--r--   0 austinwallace   (501) staff       (20)      842 2023-03-27 20:06:21.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/jobspec.py
--rw-r--r--   0 austinwallace   (501) staff       (20)    24621 2023-05-18 20:01:58.000000 hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/psi4_inps.py
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:42:36.691805 hrcl_jobs-1.2.0/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     1074 2023-01-18 19:26:42.000000 hrcl_jobs-1.2.0/LICENSE
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      962 2023-05-23 15:42:36.691805 hrcl_jobs-1.2.0/PKG-INFO
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      342 2023-02-03 23:37:54.000000 hrcl_jobs-1.2.0/README.md
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      665 2023-05-23 15:42:10.000000 hrcl_jobs-1.2.0/pyproject.toml
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      295 2023-05-23 15:42:36.693805 hrcl_jobs-1.2.0/setup.cfg
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:42:36.614805 hrcl_jobs-1.2.0/src/
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:42:36.653805 hrcl_jobs-1.2.0/src/hrcl_jobs/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      128 2023-05-17 19:18:08.000000 hrcl_jobs-1.2.0/src/hrcl_jobs/__init__.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)    14403 2023-04-04 18:52:12.000000 hrcl_jobs-1.2.0/src/hrcl_jobs/data.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      968 2023-05-17 19:44:14.000000 hrcl_jobs-1.2.0/src/hrcl_jobs/examples.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      893 2023-04-04 18:52:12.000000 hrcl_jobs-1.2.0/src/hrcl_jobs/jobspec.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)    11139 2023-05-23 04:01:41.000000 hrcl_jobs-1.2.0/src/hrcl_jobs/parallel.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)    20138 2023-04-04 18:52:12.000000 hrcl_jobs-1.2.0/src/hrcl_jobs/s22.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     2093 2023-04-04 18:52:12.000000 hrcl_jobs-1.2.0/src/hrcl_jobs/serial.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     9082 2023-04-04 18:52:12.000000 hrcl_jobs-1.2.0/src/hrcl_jobs/setup.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)    21146 2023-05-22 06:46:14.000000 hrcl_jobs-1.2.0/src/hrcl_jobs/sqlt.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     2929 2023-01-18 19:27:30.000000 hrcl_jobs-1.2.0/src/hrcl_jobs/tools_og.py
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:42:36.663805 hrcl_jobs-1.2.0/src/hrcl_jobs.egg-info/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      962 2023-05-23 15:42:36.000000 hrcl_jobs-1.2.0/src/hrcl_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      685 2023-05-23 15:42:36.000000 hrcl_jobs-1.2.0/src/hrcl_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-05-23 15:42:36.000000 hrcl_jobs-1.2.0/src/hrcl_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       69 2023-05-23 15:42:36.000000 hrcl_jobs-1.2.0/src/hrcl_jobs.egg-info/requires.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       40 2023-05-23 15:42:36.000000 hrcl_jobs-1.2.0/src/hrcl_jobs.egg-info/top_level.txt
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)        1 2023-01-18 19:35:58.000000 hrcl_jobs-1.2.0/src/hrcl_jobs.egg-info/zip-safe
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:42:36.685805 hrcl_jobs-1.2.0/src/hrcl_jobs_orca/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       24 2023-05-17 19:45:00.000000 hrcl_jobs-1.2.0/src/hrcl_jobs_orca/__init__.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      628 2023-05-22 17:53:47.000000 hrcl_jobs-1.2.0/src/hrcl_jobs_orca/jobspec.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)     5343 2023-05-23 15:40:29.000000 hrcl_jobs-1.2.0/src/hrcl_jobs_orca/orca_inps.py
+drwxr-xr-x   0 amwalla3  (1578) sherrill  (1500)        0 2023-05-23 15:42:36.689805 hrcl_jobs-1.2.0/src/hrcl_jobs_psi4/
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)       24 2023-05-05 05:19:00.000000 hrcl_jobs-1.2.0/src/hrcl_jobs_psi4/__init__.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)      842 2023-02-21 20:03:46.000000 hrcl_jobs-1.2.0/src/hrcl_jobs_psi4/jobspec.py
+-rw-r--r--   0 amwalla3  (1578) sherrill  (1500)    24621 2023-05-05 06:13:33.000000 hrcl_jobs-1.2.0/src/hrcl_jobs_psi4/psi4_inps.py
```

### Comparing `hrcl_jobs-1.1.0/LICENSE` & `hrcl_jobs-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.1.0/PKG-INFO` & `hrcl_jobs-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrcl_jobs
-Version: 1.1.0
+Version: 1.2.0
 Summary: Runs python functions on worker threads with main thread communicating with sql db
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/hierarchical_python_jobs
 Project-URL: Bug Tracker, https://github.com/Awallace3/hierarchical_python_jobs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hrcl_jobs-1.1.0/pyproject.toml` & `hrcl_jobs-1.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hrcl_jobs"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Austin M. Wallace", email="awallace43@gatech.edu" },
 ]
 description = "Runs python functions on worker threads with main thread communicating with sql db"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs/data.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs/data.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs/examples.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs/examples.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs/jobspec.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs/jobspec.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs/parallel.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs/parallel.py`

 * *Files 25% similar despite different names*

```diff
@@ -184,7 +184,172 @@
                 output = run_js_job(js)
                 output.append(js.id_label)
                 output.append(rank)
                 s = time.time()
                 comm.send(output, dest=0, tag=2)
         print(rank, "TERMINATING")
         return
+
+
+def ms_sl_extra_info(
+    id_list=[0, 50],
+    db_path="db/dimers_all.db",
+    collect_ids_into_js_ls=collect_ids_into_js_ls,
+    collect_id_into_js=collect_id_into_js,
+    run_js_job=example_run_js_job,
+    update_func=update_by_id,
+    extra_info=[],
+    headers_sql=["main_id", "id", "RA", "RB", "ZA", "ZB", "TQA", "TQB"],
+    js_obj=example_js,
+    ppm="4gb",
+    table="main",
+    id_label="main_id",
+    output_columns=[
+        "env_multipole_A",
+        "env_multipole_B",
+        "vac_widths_A",
+        "vac_widths_B",
+        "vac_vol_rat_A",
+        "vac_vol_rat_B",
+    ],
+):
+    """
+    To use ms_sl properly, write your own run_js_job function along with an
+    appropriate js_obj dataclass.
+
+    This was designed to work with psi4 jobs using the python api; however,
+    any user defined function for workers will work.
+
+    To run with multiple procs, use following example
+    ```bash
+    mpiexec -n 2 python3 -u main.py
+    ```
+    """
+
+    comm = MPI.COMM_WORLD
+    rank = comm.Get_rank()
+    n_procs = comm.Get_size()
+    print("rank", rank)
+    if rank == 0:
+        jobs = len(id_list)
+        start = time.time()
+        first = True
+        con, cur = establish_connection(db_p=db_path)
+        cur_rows = []
+        id_list_first = id_list[: n_procs - 1]
+        if len(id_list) == 1 or n_procs == 2:
+            js = collect_id_into_js(
+                cur,
+                mem=ppm,
+                headers=headers_sql,
+                extra_info=extra_info,
+                dataclass_obj=js_obj,
+                id_value=id_list[0],
+                id_label=id_label,
+                table=table,
+            )
+            r = [js]
+
+        else:
+            r = collect_ids_into_js_ls(
+                cur,
+                mem=ppm,
+                headers=headers_sql,
+                extra_info=extra_info,
+                dataclass_obj=js_obj,
+                id_list=id_list_first,
+                id_label=id_label,
+                table=table,
+            )
+        for n, js in enumerate(r):
+            n = n + 1
+            req = comm.isend(js, dest=n, tag=2)
+            req.wait()
+            print(f"{n} / {jobs}")
+        id_list_extra = id_list[len(r) :]
+        # active_ind = jobs + n_procs - 1
+        # while active_ind <= jobs:
+        for n, active_ind in enumerate(id_list_extra):
+            output = comm.recv(source=MPI.ANY_SOURCE, tag=2)
+            target_proc = output.pop()
+            id_value = output.pop()
+            js = collect_id_into_js(
+                cur,
+                mem=ppm,
+                headers=headers_sql,
+                extra_info=extra_info,
+                dataclass_obj=js_obj,
+                id_value=active_ind,
+                id_label=id_label,
+                table=table,
+            )
+            comm.send(js, dest=target_proc, tag=2)
+            i1 = time.time()
+            print(f"MAIN: {n + n_procs - 1} / {jobs}")
+            p = glob("psi.*.clean")
+            for i in p:
+                if os.path.exists(i):
+                    try:
+                        os.remove(i)
+                    except FileNotFoundError:
+                        continue
+            update_func(
+                con,
+                cur,
+                output,
+                id_label=id_label,
+                id_value=id_value,
+                table=table,
+                output_columns=output_columns,
+            )
+            i2 = time.time() - i1
+            print(f"\nMAIN: id {id_value} inserted\n")
+        print("\nMAIN CLEANING UP PROCESSES\n")
+        for n in range(n_procs - 1):
+            output = comm.recv(source=MPI.ANY_SOURCE, tag=2)
+            p = glob("psi.*.clean")
+            target_proc = output.pop()
+            for i in p:
+                if os.path.exists(i):
+                    try:
+                        os.remove(i)
+                    except FileNotFoundError:
+                        continue
+            id_value = output.pop()
+            update_func(
+                con,
+                cur,
+                output,
+                id_label=id_label,
+                id_value=id_value,
+                table=table,
+                output_columns=output_columns,
+            )
+            comm.send(0, dest=target_proc, tag=2)
+        print("\nCOMPLETED MAIN\n")
+        # read_output(db_path, id_list=[id_list[0]], id_label=id_label)
+
+    else:
+        start = True
+        js = 1
+        req = comm.irecv(source=0, tag=2)
+        js = req.wait()
+        print(f"rank: {rank}, js.main_id: {js.id_label}")
+        s = time.time()
+        output = run_js_job(js)
+        output.append(js.id_label)
+        output.append(rank)
+        comm.send(output, dest=0, tag=2)
+        print(f"rank: {rank} TOOK {time.time() - s} seconds")
+        while js != 0:
+            # print(f"rank: {rank} is BLOCKED")
+            s = time.time()
+            js = comm.recv(source=0, tag=2)
+            if js != 0:
+                print(f"rank: {rank}, js.main_id: {js.id_label}")
+                output = run_js_job(js)
+                output.append(js.id_label)
+                output.append(rank)
+                comm.send(output, dest=0, tag=2)
+                print(f"rank: {rank} TOOK {time.time() - s} seconds")
+        print(rank, "TERMINATING")
+        return
```

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs/s22.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs/s22.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs/serial.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs/serial.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs/setup.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs/setup.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs/sqlt.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs/sqlt.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,31 @@
     except sql.OperationalError as e:
         # print("TABLE ALREADY EXISTS. SKIPPING GENERATION\n")
         print(e)
         return False
     return True
 
 
+def table_add_columns(con: sql.Connection, table_name:str, table_dict: dict,) -> bool:
+    """
+    table_add_columns insert columns into a table.
+    """
+    cur = con.execute(f"PRAGMA table_info({table_name});")
+    desc = cur.fetchall()
+    existing_table = {}
+    for i in desc:
+        existing_table[i[1]] = i[2]
+    for k, v in table_dict.items():
+        if k not in existing_table.keys():
+            print(f"Adding column {k} to {table_name}")
+            con.execute(f"ALTER TABLE {table_name} ADD COLUMN {k} {v};")
+    return True
+
+
+
 def create_new_db(
     db_name="db/main.db",
     table_name="main",
     table={
         "Dimer": "TEXT",
         "R": "FLOAT",
         "CBS": "FLOAT",
@@ -513,15 +530,18 @@
     else:
         id_name = ", ".join(id_names)
     if len(matches) > 0:
         where_match = []
         for k, v in matches.items():
             v = query_clean_match(v)
             if len(v) == 1:
-                m = f'{k}=={v[0]}'
+                if v[0] == '"NULL"':
+                    m = f"{k} IS NULL"
+                else:
+                    m = f'{k}=={v[0]}'
             else:
                 m = f"{k} IN {tuple(v)}"
             where_match.append(m)
         wm = " AND ".join(where_match)
         sql_cmd = f"""SELECT {id_name} FROM {table_name} WHERE {wm};"""
     else:
         sql_cmd = f"""SELECT {id_name} FROM {table_name};"""
@@ -711,14 +731,38 @@
         df = pd.read_sql_query(f"SELECT * from {table};", con)
     print(df)
     df.to_pickle(df_p)
     print(df.columns)
     return
 
 
+def table_to_df_csv(
+    db_p="db/dimers_all.db",
+    table="main",
+    df_csv="data/dimers_10k.csv",
+    id_list=[],
+    id_label="main_id",
+) -> None:
+    """
+    table_to_df_csv
+    """
+    con, cur = establish_connection(db_p)
+    if id_list:
+        cmd = f"""SELECT * FROM {table} WHERE {table}.{id_label} IN {tuple(id_list)};"""
+        print(cmd)
+        df = pd.read_sql_query(cmd, con)
+    else:
+        df = pd.read_sql_query(f"SELECT * from {table};", con)
+    print(df)
+    df.to_csv(df_csv)
+    print(df.columns)
+    return
+
+
+
 def read_example_output(db_path="db/dimers.db", row_range=[0, 1]) -> None:
     """
     read_example_output reads sql row by rowid to verify update
     """
     con, cur = establish_connection(db_path)
     rows = collect_rows_index_range(cur, row_range)
     for n, i in enumerate(rows):
```

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs/tools_og.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs/tools_og.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/PKG-INFO` & `hrcl_jobs-1.2.0/src/hrcl_jobs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hrcl-jobs
-Version: 1.1.0
+Version: 1.2.0
 Summary: Runs python functions on worker threads with main thread communicating with sql db
 Author-email: "Austin M. Wallace" <awallace43@gatech.edu>
 Project-URL: Homepage, https://github.com/Awallace3/hierarchical_python_jobs
 Project-URL: Bug Tracker, https://github.com/Awallace3/hierarchical_python_jobs/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs.egg-info/SOURCES.txt` & `hrcl_jobs-1.2.0/src/hrcl_jobs.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-.gitignore
 LICENSE
 README.md
-main.py
 pyproject.toml
 setup.cfg
 src/hrcl_jobs/__init__.py
 src/hrcl_jobs/data.py
 src/hrcl_jobs/examples.py
 src/hrcl_jobs/jobspec.py
 src/hrcl_jobs/parallel.py
```

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs_orca/jobspec.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs_orca/jobspec.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     DB: str
     sys_ind: int
     RA: np.array
     RB: np.array
     ZA: np.array
     ZB: np.array
     charges: np.array
-    level_theory: str
+    extra_info: dict
     mem: str
 
 def dlpno_ie_sql_headers() -> []:
         return [
             "id",
             "DB",
             "sys_ind",
```

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/jobspec.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs_psi4/jobspec.py`

 * *Files identical despite different names*

### Comparing `hrcl_jobs-1.1.0/src/hrcl_jobs_psi4/psi4_inps.py` & `hrcl_jobs-1.2.0/src/hrcl_jobs_psi4/psi4_inps.py`

 * *Files identical despite different names*

