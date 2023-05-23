# Comparing `tmp/bmtool-0.3.4.tar.gz` & `tmp/bmtool-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmtool-0.3.4.tar", last modified: Sun Mar 19 05:10:05 2023, max compression
+gzip compressed data, was "bmtool-0.3.5.tar", last modified: Tue May 23 16:27:31 2023, max compression
```

## Comparing `bmtool-0.3.4.tar` & `bmtool-0.3.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-03-19 05:10:05.372911 bmtool-0.3.4/
--rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.4/LICENSE
--rw-rw-rw-   0        0        0    16777 2023-03-19 05:10:05.371912 bmtool-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    16032 2023-03-18 21:25:54.000000 bmtool-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-03-19 05:10:05.338437 bmtool-0.3.4/bmtool/
--rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.4/bmtool/__init__.py
--rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.4/bmtool/__main__.py
--rw-rw-rw-   0        0        0    25442 2023-03-17 15:40:34.000000 bmtool-0.3.4/bmtool/bmplot.py
-drwxrwxrwx   0        0        0        0 2023-03-19 05:10:05.359687 bmtool-0.3.4/bmtool/debug/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.4/bmtool/debug/__init__.py
--rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.4/bmtool/debug/commands.py
--rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.4/bmtool/debug/debug.py
--rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.4/bmtool/manage.py
--rw-rw-rw-   0        0        0    10440 2023-03-17 15:16:10.000000 bmtool-0.3.4/bmtool/plot_commands.py
--rw-rw-rw-   0        0        0    15251 2023-03-19 05:09:25.000000 bmtool-0.3.4/bmtool/singlecell.py
-drwxrwxrwx   0        0        0        0 2023-03-19 05:10:05.365913 bmtool-0.3.4/bmtool/util/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.4/bmtool/util/__init__.py
--rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.4/bmtool/util/commands.py
-drwxrwxrwx   0        0        0        0 2023-03-19 05:10:05.369913 bmtool-0.3.4/bmtool/util/neuron/
--rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.4/bmtool/util/neuron/__init__.py
--rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.4/bmtool/util/neuron/celltuner.py
--rw-rw-rw-   0        0        0    50448 2023-03-17 15:51:11.000000 bmtool-0.3.4/bmtool/util/util.py
-drwxrwxrwx   0        0        0        0 2023-03-19 05:10:05.354688 bmtool-0.3.4/bmtool.egg-info/
--rw-rw-rw-   0        0        0    16777 2023-03-19 05:10:04.000000 bmtool-0.3.4/bmtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-03-19 05:10:04.000000 bmtool-0.3.4/bmtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-19 05:10:04.000000 bmtool-0.3.4/bmtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-03-19 05:10:04.000000 bmtool-0.3.4/bmtool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2023-03-19 05:10:04.000000 bmtool-0.3.4/bmtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-19 05:10:04.000000 bmtool-0.3.4/bmtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-19 05:10:05.374076 bmtool-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1348 2023-03-19 05:09:43.000000 bmtool-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.053040 bmtool-0.3.5/
+-rw-rw-rw-   0        0        0     1089 2022-09-11 17:13:05.000000 bmtool-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0    16777 2023-05-23 16:27:31.050037 bmtool-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    16032 2023-03-18 21:25:54.000000 bmtool-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.005174 bmtool-0.3.5/bmtool/
+-rw-rw-rw-   0        0        0      141 2023-03-17 15:08:47.000000 bmtool-0.3.5/bmtool/__init__.py
+-rw-rw-rw-   0        0        0      676 2023-03-17 15:09:21.000000 bmtool-0.3.5/bmtool/__main__.py
+-rw-rw-rw-   0        0        0    25442 2023-03-17 15:40:34.000000 bmtool-0.3.5/bmtool/bmplot.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.033685 bmtool-0.3.5/bmtool/debug/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.5/bmtool/debug/__init__.py
+-rw-rw-rw-   0        0        0      602 2022-09-11 17:13:05.000000 bmtool-0.3.5/bmtool/debug/commands.py
+-rw-rw-rw-   0        0        0      218 2023-03-17 14:52:10.000000 bmtool-0.3.5/bmtool/debug/debug.py
+-rw-rw-rw-   0        0        0      688 2023-03-17 15:12:53.000000 bmtool-0.3.5/bmtool/manage.py
+-rw-rw-rw-   0        0        0    10440 2023-03-17 15:16:10.000000 bmtool-0.3.5/bmtool/plot_commands.py
+-rw-rw-rw-   0        0        0    14900 2023-05-23 16:25:45.000000 bmtool-0.3.5/bmtool/singlecell.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.042872 bmtool-0.3.5/bmtool/util/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.5/bmtool/util/__init__.py
+-rw-rw-rw-   0        0        0    65882 2023-03-17 15:09:19.000000 bmtool-0.3.5/bmtool/util/commands.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.047857 bmtool-0.3.5/bmtool/util/neuron/
+-rw-rw-rw-   0        0        0        0 2022-09-11 17:13:05.000000 bmtool-0.3.5/bmtool/util/neuron/__init__.py
+-rw-rw-rw-   0        0        0    89259 2023-03-17 14:53:16.000000 bmtool-0.3.5/bmtool/util/neuron/celltuner.py
+-rw-rw-rw-   0        0        0    51814 2023-05-23 16:25:45.000000 bmtool-0.3.5/bmtool/util/util.py
+drwxrwxrwx   0        0        0        0 2023-05-23 16:27:31.027584 bmtool-0.3.5/bmtool.egg-info/
+-rw-rw-rw-   0        0        0    16777 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-23 16:27:29.000000 bmtool-0.3.5/bmtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-23 16:27:31.053040 bmtool-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1348 2023-05-23 16:26:06.000000 bmtool-0.3.5/setup.py
```

### Comparing `bmtool-0.3.4/LICENSE` & `bmtool-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.4/PKG-INFO` & `bmtool-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.4
+Version: 0.3.5
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `bmtool-0.3.4/README.md` & `bmtool-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.4/bmtool/__main__.py` & `bmtool-0.3.5/bmtool/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.4/bmtool/bmplot.py` & `bmtool-0.3.5/bmtool/bmplot.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.4/bmtool/debug/commands.py` & `bmtool-0.3.5/bmtool/debug/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.4/bmtool/manage.py` & `bmtool-0.3.5/bmtool/manage.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.4/bmtool/plot_commands.py` & `bmtool-0.3.5/bmtool/plot_commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.4/bmtool/singlecell.py` & `bmtool-0.3.5/bmtool/singlecell.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,20 +71,17 @@
         h.tstop = int(self.tstop)
         h.stdinit()
         h.run()
 
         return (list(self.t_vec), list(self.cell_vec))
 
 class Passive(CurrentClamp):
-    def __init__(self, template_name, post_init_function=None, record_sec="soma", record_loc="0.5", tstop=1200,
-                 inj_sec="soma", inj_loc="0.5", inj_amp=-100,inj_delay=200, inj_dur=1000):
-        super(Passive, self).__init__(template_name=template_name,post_init_function=post_init_function,
-                                      record_sec=record_sec, record_loc=record_loc,
-                                      tstop=tstop, inj_sec=inj_sec, inj_loc=inj_loc,
-                                      inj_amp=inj_amp, inj_delay=inj_delay, inj_dur=inj_dur)
+    def __init__(self, template_name, tstop=1200, inj_amp=-100,inj_delay=200, inj_dur=1000, **kwargs):
+        super(Passive, self).__init__(template_name=template_name, tstop=tstop,
+                                      inj_amp=inj_amp, inj_delay=inj_delay, inj_dur=inj_dur, **kwargs)
 
         self.cell_v_final = 0
         self.v_t_const = 0
 
         self.v_rest_time = 0.0
         self.v_final_time = 0.0
 
@@ -150,18 +147,18 @@
         print(tau_calc4)
         print()  
 
         return (list(self.t_vec), list(self.cell_vec))
         #return (self.v_rest, self.r_in/1e6, self.tau)
 
 class FI():
-    def __init__(self,template_name, post_init_function=None, i_increment=100,i_start=0,i_stop=1050,tstart=50, tdur=1000,
-            record_sec="soma", record_loc="0.5", inj_sec="soma", inj_loc="0.5"):
-        """ Takes in values of pA
-        """
+    def __init__(self,template_name, post_init_function=None,
+                 i_increment=100, i_start=0, i_stop=1050, tstart=50, tdur=1000,
+                 record_sec="soma", record_loc="0.5", inj_sec="soma", inj_loc="0.5"):
+        """ Takes in values of pA """
         super(FI, self).__init__()
         self.template_name = template_name
         self.post_init_function = post_init_function
         self.i_increment = float(i_increment)/1e3
         self.i_start = float(i_start)/1e3
         self.i_stop = float(i_stop)/1e3
         self.tstart = tstart
@@ -288,15 +285,16 @@
             h_loaded = dir(h)
 
             self.templates = [x for x in h_loaded if x not in h_base]
 
         return self.templates
     
     def passive_properties(self, template_name:str, post_init_function:str=None, 
-                           record_sec:str='soma', inj_sec:str='soma', plot:bool=True) -> Tuple[float,float,float]:
+                           record_sec:str='soma', inj_sec:str='soma', plot:bool=True,
+                           **kwargs) -> Tuple[list,list]:
         """
         Calculates passive properties for the specified cell template_name
 
         Parameters
         ==========
         template_name:str
             name of the cell template located in hoc
@@ -304,52 +302,53 @@
             function of the cell to be called after the cell has been initialized (like insert_mechs(123))
         record_sec:str
             section of the cell you want to record spikes from (default: soma)
         inj_sec:str
             section of the cell you want to inject current (default: soma)
         plot:bool
             automatically plot the cell profile
-        
+        **kwargs:
+            extra key word arguments for Passive()
     """
-        passive = Passive(template_name, post_init_function=post_init_function, record_sec=record_sec, inj_sec=inj_sec)
+        passive = Passive(template_name, post_init_function=post_init_function,
+                          record_sec=record_sec, inj_sec=inj_sec, **kwargs)
         time_vec, amp_vec = passive.execute()
 
         if plot:
             plt.figure()
             plt.plot(time_vec, amp_vec)
             plt.title("Passive Cell Current Injection")
             plt.xlabel('Time (ms)')
             plt.ylabel('Membrane Potential (mV)')
             plt.show()
 
         return (time_vec, amp_vec)
     
-    def current_injection(self, template_name:str, post_init_function=None, plot=True, 
-                          record_sec="soma", record_loc="0.5",  tstop=1000,
-                          inj_sec="soma", inj_loc="0.5", inj_amp=100, inj_delay=100, inj_dur=1000) -> Tuple[list,list]:
+    def current_injection(self, template_name:str, post_init_function:str=None, 
+                          record_sec:str='soma', inj_sec:str='soma', plot:bool=True,
+                          **kwargs) -> Tuple[list,list]:
         
         ccl = CurrentClamp(template_name, post_init_function=post_init_function, 
-                                      record_sec=record_sec, record_loc=record_loc,
-                                      tstop=tstop, inj_sec=inj_sec, inj_loc=inj_loc,
-                                      inj_amp=inj_amp, inj_delay=inj_delay, inj_dur=inj_dur)
+                           record_sec=record_sec, inj_sec=inj_sec, **kwargs)
         time_vec, amp_vec = ccl.execute()
 
         if plot:
             plt.figure()
             plt.plot(time_vec, amp_vec)
             plt.title("Current Injection")
             plt.xlabel('Time (ms)')
             plt.ylabel('Membrane Potential (mV)')
             plt.show()
-        
+
         return (time_vec, amp_vec)
     
     
     def fi_curve(self, template_name:str, post_init_function=None, 
-                 record_sec:str='soma', inj_sec:str='soma', plot:bool=True) -> Tuple[list,list]:
+                 record_sec:str='soma', inj_sec:str='soma', plot:bool=True,
+                 **kwargs) -> Tuple[list,list]:
         """
         Calculates an FI curve for the specified cell template_name
 
         Parameters
         ==========
         template_name:str
             name of the cell template located in hoc
@@ -362,26 +361,27 @@
         plot:bool
             automatically plot an fi curve
 
         Returns the nA used, number of spikes per nA supplied
             list(amps), list(spikes)
 
         """
-        fi = FI(template_name, post_init_function=post_init_function, record_sec=record_sec, inj_sec=inj_sec)
+        fi = FI(template_name, post_init_function=post_init_function,
+                record_sec=record_sec, inj_sec=inj_sec, **kwargs)
         amp_vec, spike_vec = fi.execute()
 
         if plot:
             plt.figure()
             plt.plot(amp_vec, spike_vec)
             plt.title("FI Curve")
             plt.xlabel('Injection (nA)')
             plt.ylabel('# Spikes')
             plt.show()
 
         return (amp_vec, spike_vec)
-        
+
 
 #Example usage
 #profiler = Profiler('./temp/templates', './temp/mechanisms/modfiles')
 #profiler.passive_properties('Cell_Cf')
 #profiler.fi_curve('Cell_Cf')
 #profiler.current_injection('Cell_Cf', post_init_function="insert_mechs(123)", inj_amp=300, inj_delay=100)
```

### Comparing `bmtool-0.3.4/bmtool/util/commands.py` & `bmtool-0.3.5/bmtool/util/commands.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.4/bmtool/util/neuron/celltuner.py` & `bmtool-0.3.5/bmtool/util/neuron/celltuner.py`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.4/bmtool/util/util.py` & `bmtool-0.3.5/bmtool/util/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -183,16 +183,16 @@
     config = load_config(fp)
     nodes = load_nodes_from_paths(config['networks']['nodes'])
     edges = load_edges_from_paths(config['networks']['edges'])
     return nodes, edges
 
 def load_nodes(nodes_file, node_types_file):
     nodes_arr = [{"nodes_file":nodes_file,"node_types_file":node_types_file}]
-    nodes = load_nodes_from_paths(nodes_arr)
-    return nodes
+    nodes = list(load_nodes_from_paths(nodes_arr).items())[0]  # single item
+    return nodes  # return (population, nodes_df)
 
 def load_nodes_from_config(config):
     if config is None:
         config = 'simulation_config.json'
     networks = load_config(config)['networks']
     return load_nodes_from_paths(networks['nodes'])
 
@@ -223,65 +223,70 @@
 
     #nodes_h5_fpaths = glob.glob(os.path.join(network_dir,'*'+nodes_regex))
     #node_types_fpaths = glob.glob(os.path.join(network_dir,'*'+node_types_regex))
 
     #regions = [re.findall('^[^_]+', os.path.basename(n))[0] for n in nodes_h5_fpaths]
     region_dict = {}
 
+    pos_labels = ('pos_x', 'pos_y', 'pos_z')
+
     #Need to get all cell groups for each region
     def get_node_table(cell_models_file, cells_file, population=None):
         cm_df = pd.read_csv(cells_file, sep=' ')
         cm_df.set_index('node_type_id', inplace=True)
 
         cells_h5 = h5py.File(cell_models_file, 'r')
         if population is None:
             if len(cells_h5['/nodes']) > 1:
                 raise Exception('Multiple populations in nodes file. Not currently supported. Should be easy to implement when needed. Let Tyler know.')
             else:
                 population = list(cells_h5['/nodes'])[0]
 
         nodes_grp = cells_h5['/nodes'][population]
-        c_df = pd.DataFrame({'node_id': nodes_grp['node_id'], 'node_type_id': nodes_grp['node_type_id']})
+        c_df = pd.DataFrame({key: nodes_grp[key] for key in ('node_id', 'node_type_id')})
         c_df.set_index('node_id', inplace=True)
 
-        nodes_df = pd.merge(left=c_df,
-                            right=cm_df,
-                            how='left',
-                            left_on='node_type_id',
-                            right_index=True)  # use 'model_id' key to merge, for right table the "model_id" is an index
-        
-        if 'positions' in list(nodes_grp['0']):
-            #cpos = pd.DataFrame({'node_id': nodes_grp['node_id'],"pos_x":nodes_grp['0']['positions'][:,0],"pos_y":nodes_grp['0']['positions'][:,1],"pos_z":nodes_grp['0']['positions'][:,2]})
-
-            #Possibly a problem when not all nodes have positions. Those without positions 
-            #should be placed at the end of your simulation (point processes)
-            di = pd.DataFrame({'node_id': nodes_grp['node_id']})
-            dx = pd.DataFrame({"pos_x":nodes_grp['0']['positions'][:,0]})
-            dy = pd.DataFrame({"pos_y":nodes_grp['0']['positions'][:,1]})
-            dz = pd.DataFrame({"pos_z":nodes_grp['0']['positions'][:,2]})
-            cpos = pd.concat([di,dx,dy,dz],ignore_index=True,axis=1)
-            cpos.rename(index=str,columns={0:di.columns[0],1:dx.columns[0],2:dy.columns[0],3:dz.columns[0]},inplace=True)
-            #End
-
-            cpos.set_index('node_id', inplace=True)            
-            
-            nodes_df = pd.merge(left=nodes_df,
-                                right=cpos,
-                                how='left',
-                                left_index=True,
-                                right_index=True)
+        nodes_df = pd.merge(left=c_df, right=cm_df, how='left',
+                            left_on='node_type_id', right_index=True)  # use 'model_id' key to merge, for right table the "model_id" is an index
+
+        # extra properties of individual nodes (see SONATA Data format)
+        if nodes_grp.get('0'):
+            node_id = nodes_grp['node_id'][()]
+            node_group_id = nodes_grp['node_group_id'][()]
+            node_group_index = nodes_grp['node_group_index'][()]
+            n_group = node_group_id.max() + 1
+            prop_dtype = {}
+            for group_id in range(n_group):
+                group = nodes_grp[str(group_id)]
+                idx = node_group_id == group_id
+                for prop in group:
+                    if prop == 'positions':
+                        positions = group[prop][node_group_index[idx]]
+                        for i in range(positions.shape[1]):
+                            if pos_labels[i] not in nodes_df:
+                                nodes_df[pos_labels[i]] = np.nan
+                            nodes_df.loc[node_id, pos_labels[i]] = positions[:, i]
+                    else:
+                        # create new column with NaN if property does not exist
+                        if prop not in nodes_df: 
+                            nodes_df[prop] = np.nan
+                        nodes_df.loc[idx, prop] = tuple(group[prop][node_group_index[idx]])
+                        prop_dtype[prop] = group[prop].dtype
+            # convert to original data type if possible
+            for prop, dtype in prop_dtype.items():
+                nodes_df[prop] = nodes_df[prop].astype(dtype, errors='ignore')
+
+        return population, nodes_df
 
-        return nodes_df, population
-    
     #for region, cell_models_file, cells_file in zip(regions, node_types_fpaths, nodes_h5_fpaths):
     #    region_dict[region] = get_node_table(cell_models_file,cells_file,population=region)
     for nodes in node_paths:
         cell_models_file = nodes["nodes_file"]
         cells_file = nodes["node_types_file"]
-        region, region_name = get_node_table(cell_models_file,cells_file)
+        region_name, region = get_node_table(cell_models_file, cells_file)
         region_dict[region_name] = region
 
     #cell_num = 2
     #print(region_dict["hippocampus"].iloc[cell_num]["node_type_id"])
     #print(list(set(region_dict["hippocampus"]["node_type_id"]))) #Unique
 
     return region_dict
@@ -290,16 +295,16 @@
     if config is None:
         config = 'simulation_config.json'
     networks = load_config(config)['networks']
     return load_edges_from_paths(networks['edges'])
 
 def load_edges(edges_file, edge_types_file):
     edges_arr = [{"edges_file":edges_file,"edge_types_file":edge_types_file}]
-    edges = load_edges_from_paths(edges_arr)
-    return edges
+    edges = list(load_edges_from_paths(edges_arr).items())[0]  # single item
+    return edges  # return (population, edges_df)
 
 def load_edges_from_paths(edge_paths):#network_dir='network'):
     """
     Returns: A dictionary of connections with filenames (minus _edges.h5) as keys
 
     edge_paths must be in the format in a circuit config file:
         [
@@ -316,51 +321,68 @@
     #edge_types_regex = "_edge_types.csv"
 
     #edges_h5_fpaths = glob.glob(os.path.join(network_dir,'*'+edges_regex))
     #edge_types_fpaths = glob.glob(os.path.join(network_dir,'*'+edge_types_regex))
 
     #connections = [re.findall('^[A-Za-z0-9]+_[A-Za-z0-9][^_]+', os.path.basename(n))[0] for n in edges_h5_fpaths]
     edges_dict = {}
-    def get_edge_table(edges_file, edge_types_file,population=None):
-        
+    def get_edge_table(edges_file, edge_types_file, population=None):
+
+        # dataframe where each row is an edge type
         cm_df = pd.read_csv(edge_types_file, sep=' ')
         cm_df.set_index('edge_type_id', inplace=True)
 
-        connections_h5 = h5py.File(edges_file, 'r')
-
-        if population is None:
-            if len(connections_h5['/edges']) > 1:
-                raise Exception('Multiple populations in edges file. Not currently implemented, should not be hard to do, contact Tyler')
-            else:
-                population = list(connections_h5['/edges'])[0]
+        with h5py.File(edges_file, 'r') as connections_h5:
+            if population is None:
+                if len(connections_h5['/edges']) > 1:
+                    raise Exception('Multiple populations in edges file. Not currently implemented, should not be hard to do, contact Tyler')
+                else:
+                    population = list(connections_h5['/edges'])[0]
+            conn_grp = connections_h5['/edges'][population]
+
+            # dataframe where each row is an edge
+            c_df = pd.DataFrame({key: conn_grp[key] for key in (
+                'edge_type_id', 'source_node_id', 'target_node_id')})
+
+            c_df.reset_index(inplace=True)
+            c_df.rename(columns={'index': 'edge_id'}, inplace=True)
+            c_df.set_index('edge_type_id', inplace=True)
+
+            # add edge type properties to df of edges
+            edges_df = pd.merge(left=c_df, right=cm_df, how='left',
+                                left_index=True, right_index=True)
+
+            # extra properties of individual edges (see SONATA Data format)
+            if conn_grp.get('0'):
+                edge_group_id = conn_grp['edge_group_id'][()]
+                edge_group_index = conn_grp['edge_group_index'][()]
+                n_group = edge_group_id.max() + 1
+                prop_dtype = {}
+                for group_id in range(n_group):
+                    group = conn_grp[str(group_id)]
+                    idx = edge_group_id == group_id
+                    for prop in group:
+                        # create new column with NaN if property does not exist
+                        if prop not in edges_df: 
+                            edges_df[prop] = np.nan
+                        edges_df.loc[idx, prop] = tuple(group[prop][edge_group_index[idx]])
+                        prop_dtype[prop] = group[prop].dtype
+                # convert to original data type if possible
+                for prop, dtype in prop_dtype.items():
+                    edges_df[prop] = edges_df[prop].astype(dtype, errors='ignore')
 
-        conn_grp = connections_h5['/edges'][population]
-        c_df = pd.DataFrame({'edge_type_id': conn_grp['edge_type_id'], 'source_node_id': conn_grp['source_node_id'],
-                                'target_node_id': conn_grp['target_node_id']})
-        if conn_grp.get('0'):
-            custom_props = conn_grp['0']
-            for prop in custom_props:
-                c_df[prop] = list(conn_grp['0'][prop])
-
-        c_df.set_index('edge_type_id', inplace=True)
-
-        nodes_df = pd.merge(left=c_df,
-                            right=cm_df,
-                            how='left',
-                            left_index=True,
-                            right_index=True) 
-        return nodes_df, population
+        return population, edges_df
 
     #for edges_dict, conn_models_file, conns_file in zip(connections, edge_types_fpaths, edges_h5_fpaths):
     #    connections_dict[connection] = get_connection_table(conn_models_file,conns_file)
     try:
         for nodes in edge_paths:
             edges_file = nodes["edges_file"]
             edge_types_file = nodes["edge_types_file"]
-            region, region_name = get_edge_table(edges_file,edge_types_file)
+            region_name, region = get_edge_table(edges_file, edge_types_file)
             edges_dict[region_name] = region
     except Exception as e:
         print(repr(e))
         print("Hint: Are you loading the correct simulation config file?")
         print("Command Line: bmtool plot --config yourconfig.json <rest of command>")
         print("Python: bmplot.connection_matrix(config='yourconfig.json')")
```

### Comparing `bmtool-0.3.4/bmtool.egg-info/PKG-INFO` & `bmtool-0.3.5/bmtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmtool
-Version: 0.3.4
+Version: 0.3.5
 Summary: BMTool
 Home-page: https://github.com/tjbanks/bmtool
 Download-URL: 
 Author: Tyler Banks
 Author-email: tbanks@mail.missouri.edu
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `bmtool-0.3.4/bmtool.egg-info/SOURCES.txt` & `bmtool-0.3.5/bmtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bmtool-0.3.4/setup.py` & `bmtool-0.3.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="bmtool",
-    version="0.3.4",
+    version="0.3.5",
     author="Tyler Banks",
     author_email="tbanks@mail.missouri.edu",
     description="BMTool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tjbanks/bmtool",
     download_url='',
```

