# Comparing `tmp/pyscomotif-0.9.29.tar.gz` & `tmp/pyscomotif-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscomotif-0.9.29.tar", last modified: Tue May 23 09:21:45 2023, max compression
+gzip compressed data, was "pyscomotif-0.9.9.tar", last modified: Mon Feb 20 09:32:55 2023, max compression
```

## Comparing `pyscomotif-0.9.29.tar` & `pyscomotif-0.9.9.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     8495 2023-05-23 09:21:12.266738 pyscomotif-0.9.29/README.md
--rw-r--r--   0        0        0      548 2023-05-23 09:21:08.894726 pyscomotif-0.9.29/pyproject.toml
--rw-r--r--   0        0        0     6901 2023-02-20 08:49:49.687463 pyscomotif-0.9.29/src/pyscomotif/RMSD_calculation.py
--rw-r--r--   0        0        0       88 2023-03-16 13:39:17.205069 pyscomotif-0.9.29/src/pyscomotif/__init__.py
--rw-r--r--   0        0        0     1251 2023-02-20 08:50:03.155529 pyscomotif-0.9.29/src/pyscomotif/constants.py
--rw-r--r--   0        0        0      857 2022-12-21 08:28:41.224270 pyscomotif-0.9.29/src/pyscomotif/data_containers.py
--rw-r--r--   0        0        0     1326 2023-01-27 13:49:21.652224 pyscomotif-0.9.29/src/pyscomotif/index_folders_and_files.py
--rw-r--r--   0        0        0    11830 2023-05-22 07:34:03.819862 pyscomotif-0.9.29/src/pyscomotif/indexing.py
--rw-r--r--   0        0        0    33394 2023-05-19 11:09:50.294910 pyscomotif-0.9.29/src/pyscomotif/motif_search.py
--rw-r--r--   0        0        0    36856 2023-02-20 08:49:49.687463 pyscomotif-0.9.29/src/pyscomotif/motif_search_with_ShareableList.py
--rw-r--r--   0        0        0    13395 2023-04-18 08:36:54.785589 pyscomotif-0.9.29/src/pyscomotif/pyscomotif.py
--rw-r--r--   0        0        0     7377 2023-02-27 14:14:03.695109 pyscomotif-0.9.29/src/pyscomotif/residue_data_dicts.py
--rw-r--r--   0        0        0     4320 2023-04-14 07:43:37.246808 pyscomotif-0.9.29/src/pyscomotif/utils.py
--rw-r--r--   0        0        0     9034 1970-01-01 00:00:00.000000 pyscomotif-0.9.29/PKG-INFO
+-rw-r--r--   0        0        0      526 2023-02-20 09:30:53.151507 pyscomotif-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     6901 2023-02-20 08:49:49.687463 pyscomotif-0.9.9/src/pyscomotif/RMSD_calculation.py
+-rw-r--r--   0        0        0      192 2022-12-05 14:40:26.045900 pyscomotif-0.9.9/src/pyscomotif/__init__.py
+-rw-r--r--   0        0        0     1251 2023-02-20 08:50:03.155529 pyscomotif-0.9.9/src/pyscomotif/constants.py
+-rw-r--r--   0        0        0      857 2022-12-21 08:28:41.224270 pyscomotif-0.9.9/src/pyscomotif/data_containers.py
+-rw-r--r--   0        0        0     1326 2023-01-27 13:49:21.652224 pyscomotif-0.9.9/src/pyscomotif/index_folders_and_files.py
+-rw-r--r--   0        0        0    11849 2023-02-20 08:49:49.691463 pyscomotif-0.9.9/src/pyscomotif/indexing.py
+-rw-r--r--   0        0        0    30206 2023-02-20 08:49:49.687463 pyscomotif-0.9.9/src/pyscomotif/motif_search.py
+-rw-r--r--   0        0        0    36856 2023-02-20 08:49:49.687463 pyscomotif-0.9.9/src/pyscomotif/motif_search_with_ShareableList.py
+-rw-r--r--   0        0        0    13398 2023-02-20 09:21:17.172691 pyscomotif-0.9.9/src/pyscomotif/pyscomotif.py
+-rw-r--r--   0        0        0     7375 2023-02-20 08:49:49.687463 pyscomotif-0.9.9/src/pyscomotif/residue_data_dicts.py
+-rw-r--r--   0        0        0     4195 2023-02-20 08:51:36.823987 pyscomotif-0.9.9/src/pyscomotif/utils.py
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 pyscomotif-0.9.9/PKG-INFO
```

### Comparing `pyscomotif-0.9.29/pyproject.toml` & `pyscomotif-0.9.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "pyscomotif"
 authors = [{name = "Gabriel Cia", email = "gabriel-_cia@hotmail.com"}]
-version = "0.9.29"
+version = "0.9.9"
 dependencies = ["numba", "click", "biopython <=1.79", "networkx", "scipy", "pandas", "numpy", "typing_extensions", "tqdm"]
 requires-python = ">=3.9"
-readme = "README.md"
 dynamic = ["description"]
 
 [project.urls]
 Home = "https://github.com/3BioCompBio/pyScoMotif"
 
 [project.scripts]
 pyscomotif = "pyscomotif.pyscomotif:command_line_interface"
```

### Comparing `pyscomotif-0.9.29/src/pyscomotif/RMSD_calculation.py` & `pyscomotif-0.9.9/src/pyscomotif/RMSD_calculation.py`

 * *Files identical despite different names*

### Comparing `pyscomotif-0.9.29/src/pyscomotif/constants.py` & `pyscomotif-0.9.9/src/pyscomotif/constants.py`

 * *Files identical despite different names*

### Comparing `pyscomotif-0.9.29/src/pyscomotif/data_containers.py` & `pyscomotif-0.9.9/src/pyscomotif/data_containers.py`

 * *Files identical despite different names*

### Comparing `pyscomotif-0.9.29/src/pyscomotif/index_folders_and_files.py` & `pyscomotif-0.9.9/src/pyscomotif/index_folders_and_files.py`

 * *Files identical despite different names*

### Comparing `pyscomotif-0.9.29/src/pyscomotif/indexing.py` & `pyscomotif-0.9.9/src/pyscomotif/indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     """Updates an existing index with new PDB files."""
     set_of_already_indexed_PDBs = get_set_of_already_indexed_PDBs(index_folder_path)
     PDB_files_to_index: List[Path] = []
     for PDB_file in database_path.rglob(pattern):
         PDB_ID = get_PDB_ID_from_file_path(PDB_file)
         if PDB_ID not in set_of_already_indexed_PDBs:
             PDB_files_to_index.append(PDB_file)
-    del set_of_already_indexed_PDBs
+    del set_of_already_indexed_PDBs # No longer needed
     
     if not PDB_files_to_index:
         raise ValueError(f"No new files were found that match the pattern {pattern}.")
 
     compression = detect_the_compression_algorithm_used_in_the_index(index_folder_path)
 
     index_PDB_files(PDB_files_to_index, index_folder_path, compression, n_cores)
```

### Comparing `pyscomotif-0.9.29/src/pyscomotif/motif_search.py` & `pyscomotif-0.9.9/src/pyscomotif/motif_search_with_ShareableList.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,37 @@
+# This version of the motif search code attemps to speed up the search when dealing with many mutated motifs. The idea is that when 
+# dealing with many mutated versions of a reference motif, the data of the same residue pairs is generally loaded over and over again, 
+# in particular the residue pair data of the reference motif. The optimization is to therefore load the data of those residue pairs
+# once and share it between the parallel process, which can be done using a ShareableList.
+# There are two problems with this implementation that need to be addresses before the code can be relased:
+# 1) There is a warning that says the shared_memory object is leaked and was not properly cleaned up, despite running shm.close() and shm.unlink() in the code
+# 2) The ShareableList documentation says that all items in the list must be < 10M bytes, so the code might crash if there is a residue pair that has a lot of data.
+
 import itertools
+import pickle
 from collections import defaultdict
 from concurrent.futures import Future, ProcessPoolExecutor, as_completed
+from multiprocessing.shared_memory import ShareableList
 from pathlib import Path
 from typing import Dict, Iterator, List, Set, Tuple, Union
 
 import networkx as nx
 import pandas as pd
-from tqdm import tqdm
 
 from pyscomotif.constants import (AMINO_ACID_ALPHABET,
-                                  AMINO_ACID_RELAXED_GROUPS_MAP,
-                                  INDEX_ANGLE_BIN_SIZE,
-                                  INDEX_DISTANCE_BIN_SIZE)
+                                    AMINO_ACID_RELAXED_GROUPS_MAP,
+                                    INDEX_ANGLE_BIN_SIZE,
+                                    INDEX_DISTANCE_BIN_SIZE)
 from pyscomotif.data_containers import Residue, Residue_pair_data
 from pyscomotif.index_folders_and_files import index_folder_exists
 from pyscomotif.residue_data_dicts import extract_residue_data
 from pyscomotif.utils import (
     angle_between_two_vectors,
-    detect_the_compression_algorithm_used_in_the_index, flatten_iterable,
-    get_bin_number, get_sorted_2_tuple, pairwise_euclidean_distance,
+    detect_the_compression_algorithm_used_in_the_index, get_bin_number,
+    get_sorted_2_tuple, pairwise_euclidean_distance,
     read_compressed_and_pickled_file, sort_and_join_2_strings)
 
 
 def extract_motif_residues_from_PDB_file(PDB_file: Path, motif: Tuple[str,...]) -> Dict[str, Residue]:
     """
     ...
     """
@@ -159,21 +168,18 @@
                     copy=True
                 )
                 
                 yield mutated_graph
     
 def get_all_pairs_of_residues_in_motif_MST(motif_MST: nx.Graph) -> Dict[Tuple[str,str], Residue_pair_data]:
     """
-    Returns all the residue pairs in motif_MST in an ordered manner such that, for all i, residue pairs between 0 and i form a connected graph. The order follows 
-    that of a Depth First Search (dfs). If the residue pairs were randomly ordered, we wouldn't be able to do the connectivity check 
-    in update_map_of_PDBs_with_all_residue_pairs, because the logic requires that new residue pairs are connected to already visited nodes.
     """
-    MST_edges: List[Tuple[str, str]] = list(nx.edge_dfs(motif_MST)) # Ex: [('A1G', 'A3K'), ('A3K', 'A8N'), ...]
-
     all_pairs_of_residues_in_motif_MST: Dict[Tuple[str,str], Residue_pair_data] = {}
+
+    MST_edges: List[Tuple[str, str]] = list(motif_MST.edges) # Ex: [('A1G', 'A3K'), ('A3K', 'A8N'), ...]
     for pair_of_full_residue_IDs in MST_edges:
         pair_of_full_residue_IDs = get_sorted_2_tuple(pair_of_full_residue_IDs) # Ordering is needed to make sure we only calculate each pair once, i.e avoid calculating the results of (A,B) and (B,A), as they are identical.
         
         all_pairs_of_residues_in_motif_MST[pair_of_full_residue_IDs] = motif_MST.edges[pair_of_full_residue_IDs]['residue_pair_data']
 
     return all_pairs_of_residues_in_motif_MST
 
@@ -274,138 +280,106 @@
     if full_residue_pair_df.empty:
         return {}
 
     PDBs_that_contain_the_residue_pair: Dict[str, List[Tuple[str,str]]] = defaultdict(list)
     res1_resname, res2_resname = pair_of_residues[0], pair_of_residues[1]
     res1_ID: str; res2_ID: str; PDB_ID: str
     for res1_ID, res2_ID, PDB_ID in zip(full_residue_pair_df.residue_1.values, full_residue_pair_df.residue_2.values, full_residue_pair_df.PDB_ID.values):
-        res1_ID, res2_ID = str(res1_ID), str(res2_ID) # Some PDBs such as 3PGA name their chains using numbers, which results in some dataframes where the residue_1 and residue_2 columns are not strings but ints.
-
         res1_full_ID = res1_ID + res1_resname # Ex: 'A1G', that is residue A1 which is a Glycine
         res2_full_ID = res2_ID + res2_resname
         pair_of_full_residue_IDs = get_sorted_2_tuple((res1_full_ID, res2_full_ID)) # Sorting is needed to be able to find PDBs with the residue pair in the correct geometric arrangement later
         
         PDBs_that_contain_the_residue_pair[PDB_ID].append(pair_of_full_residue_IDs)
         
     return PDBs_that_contain_the_residue_pair
 
-def residue_pair_is_connected_to_visited_nodes(residue_pair: Tuple[str, str], visited_nodes: Set[str]) -> bool:
-    return residue_pair[0] in visited_nodes or residue_pair[1] in visited_nodes
-
 def update_map_of_PDBs_with_all_residue_pairs(
-        map_of_PDBs_with_all_residue_pairs: Dict[str, List[Tuple[str,str]]], new_residue_pair_data: Dict[str, List[Tuple[str,str]]], visited_nodes_map: Dict[str, Set[str]]
+        map_of_PDBs_with_all_residue_pairs: Dict[str, List[Tuple[str,str]]], new_residue_pair_data: Dict[str, List[Tuple[str,str]]]
     ) -> None:
     """
     ...
     """
-    updated_set_of_PDBs_with_all_residue_pairs = map_of_PDBs_with_all_residue_pairs.keys() & new_residue_pair_data.keys() # & = set intersection
+    updated_set_of_PDBs_with_all_residue_pairs = map_of_PDBs_with_all_residue_pairs.keys() & new_residue_pair_data.keys() # & = set intersection 
     
     for PDB_ID in list(map_of_PDBs_with_all_residue_pairs.keys()):
-        # Drop PDBs that no longer have all the residue pairs
         if PDB_ID not in updated_set_of_PDBs_with_all_residue_pairs:
-            del map_of_PDBs_with_all_residue_pairs[PDB_ID]
-            del visited_nodes_map[PDB_ID]
-            continue
-        
-        # Connectivity check. New residue pairs that are not connected to already visited nodes can be dropped, and if all are droped then we can also drop the PDB
-        connectivity_checked_residue_pairs: List[Tuple[str,str]] = [
-            residue_pair
-            for residue_pair in new_residue_pair_data[PDB_ID]
-            if residue_pair_is_connected_to_visited_nodes(residue_pair, visited_nodes_map[PDB_ID])
-        ]
-        if not connectivity_checked_residue_pairs:
-            del map_of_PDBs_with_all_residue_pairs[PDB_ID]
-            del visited_nodes_map[PDB_ID]
-            continue
-
-        map_of_PDBs_with_all_residue_pairs[PDB_ID].extend(connectivity_checked_residue_pairs) # Update the list of residue pairs of the PDB
-        visited_nodes_map[PDB_ID].update(set(flatten_iterable(connectivity_checked_residue_pairs)))
+            del map_of_PDBs_with_all_residue_pairs[PDB_ID] # We remove PDBs that no longer have all the residue pairs
+        else:
+            map_of_PDBs_with_all_residue_pairs[PDB_ID].extend(new_residue_pair_data[PDB_ID]) # We update the set of residue pairs of the PDBs that have all the residue pairs
 
     return
 
 def find_PDBs_with_all_residue_pairs(
         motif_MST: nx.Graph, index_folder_path: Path, distance_delta_thr: float, angle_delta_thr: float, compression: str, 
         concurrent_executor: ProcessPoolExecutor
     ) -> Dict[str, List[Tuple[str,str]]]:
     """
     """
-    # The algorithm determines which PDBs contain all the residue pairs of a given motif MST by iterating over each residue pair and calculating the 
-    # intersection between the current map of PDBs with all residue pairs and the PDBs that contain the given residue pair that is being 
-    # checked (i.e iterative intersection). A connectivity check between the already determined residue pairs and the new ones is also performed to remove PDBs 
-    # that have the reside pairs but are not connected and therefore don't form a motif (see update_map_of_PDBs_with_all_residue_pairs).
+    # The algorithm determines which PDBs contain all the residue pairs of a given motif MST by simply iterating over each residue pair 
+    # and calculating the intersection between the current map of PDBs with all residue pairs and the PDBs that contain
+    # the given residue pair that is being checked (i.e iterative intersection).
     all_pairs_of_residues_to_check = get_all_pairs_of_residues_in_motif_MST(motif_MST)
-
+    
     submitted_futures: List[Future[Dict[str, List[Tuple[str,str]]]]] = [
         concurrent_executor.submit(get_PDBs_that_contain_the_residue_pair, pair_of_full_residue_IDs, residue_pair_data, distance_delta_thr, angle_delta_thr, index_folder_path, compression)
         for pair_of_full_residue_IDs, residue_pair_data in all_pairs_of_residues_to_check.items()
     ]
-    
+
     map_of_PDBs_with_all_residue_pairs: Dict[str, List[Tuple[str,str]]]
     map_of_PDBs_with_all_residue_pairs_initialized_flag: bool = False
-    visited_nodes_map: Dict[str, Set[str]] # Used for connectivity check
-    for future in submitted_futures:
+    for future in as_completed(submitted_futures):
         if future.exception():
             raise future.exception() # type: ignore
 
         PDBs_that_contain_the_residue_pair = future.result()
 
         # Iterative intersection code. map_of_PDBs_with_all_residue_pairs must be initialized with the PDBs of a 
         # residue pair in order to be able to do the iterative intersection, otherwise we would always get an empty set 
         # given it is initially empty.
         if map_of_PDBs_with_all_residue_pairs_initialized_flag == False:
             map_of_PDBs_with_all_residue_pairs = defaultdict(list, PDBs_that_contain_the_residue_pair)
             map_of_PDBs_with_all_residue_pairs_initialized_flag = True
-            visited_nodes_map = {
-                PDB_ID:set(flatten_iterable(list_of_residue_pairs))
-                for PDB_ID, list_of_residue_pairs in map_of_PDBs_with_all_residue_pairs.items()
-            }
 
         else:
             update_map_of_PDBs_with_all_residue_pairs(
                 map_of_PDBs_with_all_residue_pairs, 
-                PDBs_that_contain_the_residue_pair,
-                visited_nodes_map
+                PDBs_that_contain_the_residue_pair
             )
-
+        
     return map_of_PDBs_with_all_residue_pairs
 
 def add_resname_as_node_attribute(graph: nx.Graph) -> None:
     """
     """
     nx.set_node_attributes(graph, {node:{'resname':node[-1]} for node in graph.nodes}) # Each node is a residue_full_ID so [-1] returns the residue (ex: 'G', for Glycine)
     return
 
-def run_subgraph_monomorphism(motif_MST: nx.Graph, pairs_of_residues: List[Tuple[str,str]]) -> List[nx.Graph]:
+def run_subgraph_monomorphism(motif_MST: nx.Graph, pairs_of_residues: List[Tuple[str,str]]) -> Union[None, List[nx.Graph]]:
     """
     The returned list can be empty.
     """
     candidate_PDB_graph = nx.Graph(pairs_of_residues)
     add_resname_as_node_attribute(candidate_PDB_graph)
 
-    # NOTE: We don't need to use the edge_matcher functionality of the GraphMatcher because in the previous step we performed a connectivity check,
-    # which ensures that each residue pair of the candidate PDB is in the correct geometrical arrangement AND connected to a residue pair. 
-    # If the connectivity check had not been performed, candidate PDBs with residue pairs in the correct geometrical arrangement BUT connected in
-    # the wrong way would pass the monomorphism check given it does not check edge values, only the residue types. This kind of edge case can for example happen
-    # when an epitope has a chain of repeating residue pairs (i.e (S,T),(T,S),(S,T), ...).
     graph_matcher = nx.algorithms.isomorphism.GraphMatcher(
         G1 = candidate_PDB_graph, G2 = motif_MST, 
         node_match = lambda node1,node2: node1['resname'] == node2['resname'] # Match based on residue name
     )
-    
+
     monomorphism_checked_motifs: List[nx.Graph] = [] # Each PDB can have multiple motifs (i.e: homodimers) -> List[nx.Graph]
     residue_mapping_dict: Dict[str,str]
     for residue_mapping_dict in graph_matcher.subgraph_monomorphisms_iter():
         residues_of_the_similar_motif = list(residue_mapping_dict.keys())
         similar_motif_graph: nx.Graph = candidate_PDB_graph.subgraph(residues_of_the_similar_motif).copy()
         
         setattr(similar_motif_graph, 'residue_mapping_dict', residue_mapping_dict) # Used for RMSD calculation
 
         monomorphism_checked_motifs.append(similar_motif_graph)
 
-    return monomorphism_checked_motifs
+    return monomorphism_checked_motifs if monomorphism_checked_motifs else None
 
 def filter_out_PDBs_with_unconnected_residue_pairs(
         PDBs_with_all_residue_pairs: Dict[str, List[Tuple[str,str]]], motif_MST: nx.Graph, concurrent_executor: ProcessPoolExecutor, 
     ) -> Dict[str, List[nx.Graph]]:
     """
     """
     # To know if a PDB contains a set of connected residue pairs forming a similar motif, we use subgraph monomorphism to perform a matching between a reference 
@@ -418,143 +392,245 @@
     # the occurence of an additional AE edge between residue A32A and A35E, and that edge causes isomorphism to fail, unlike monomorphism which correctly finds the PDB.
     add_resname_as_node_attribute(motif_MST) # Needed for subgraph monomorphism, see run_subgraph_monomorphism().
 
     submited_futures: Dict[Future[Union[None, List[nx.Graph]]], str] = {
         concurrent_executor.submit(run_subgraph_monomorphism, motif_MST, pairs_of_residues):PDB_ID
         for PDB_ID, pairs_of_residues in PDBs_with_all_residue_pairs.items()
     }
-    PDBs_with_all_residue_pairs.clear() # Free some memory
 
     filtered_PDBs_with_all_residue_pairs: Dict[str, List[nx.Graph]] =  {}
     for future in as_completed(submited_futures):
         if future.exception():
             raise future.exception() # type: ignore
 
-        PDB_ID = submited_futures[future]
         monomorphism_checked_motifs = future.result()
-        if not monomorphism_checked_motifs: # These are the false positive PDBs, i.e PDBs that have all the residue pairs but where the monomorphism check doesn't find any similar motif 
+        if not monomorphism_checked_motifs: # These are the false positive PDBs, i.e PDBs that have all the residue pairs but where the monomorphism check doesn't find any similar motif as a result of unconnected pairs of residues 
             continue
 
+        PDB_ID = submited_futures[future]
         filtered_PDBs_with_all_residue_pairs[PDB_ID] = monomorphism_checked_motifs
 
     return filtered_PDBs_with_all_residue_pairs
 
+def residue_pair_level_parallelisation(
+        reference_motif_MST: nx.Graph, max_n_mutated_residues: int, residue_type_policy: Union[str, Dict[str,List[str]]],
+        reference_motif_residues_data: Dict[str, Residue], index_folder_path: Path, distance_delta_thr: float, 
+        angle_delta_thr: float, compression: str, concurrent_executor: ProcessPoolExecutor, 
+        motif_MST_filtered_PDBs_map: Dict[nx.Graph, Dict[str, List[nx.Graph]]]
+    ) -> None:
+    """
+    ...
+    """
+    for motif_MST in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, reference_motif_residues_data):
+        PDBs_with_all_residue_pairs = find_PDBs_with_all_residue_pairs(motif_MST, index_folder_path, distance_delta_thr, angle_delta_thr, compression, concurrent_executor)
+        filtered_PDBs_with_all_residue_pairs = filter_out_PDBs_with_unconnected_residue_pairs(PDBs_with_all_residue_pairs, motif_MST, concurrent_executor)
+        
+        if filtered_PDBs_with_all_residue_pairs:
+            motif_MST_filtered_PDBs_map[motif_MST] = filtered_PDBs_with_all_residue_pairs
+    
+    return
+
+def get_reference_motif_residue_pairs_data(
+        reference_motif_MST: nx.Graph, index_folder_path: Path, distance_delta_thr: float, angle_delta_thr: float, 
+        compression: str, concurrent_executor: ProcessPoolExecutor
+    ) -> Tuple[List[bytes], Dict[Tuple[str,str], int]]:
+    """
+    ...
+    """
+    # First load all the residue pair data of the reference_motif_MST
+    all_pairs_of_residues_to_check = get_all_pairs_of_residues_in_motif_MST(reference_motif_MST)
+    
+    submitted_futures: Dict[Future[Dict[str, List[Tuple[str,str]]]], Tuple[str,str]] = {
+        concurrent_executor.submit(get_PDBs_that_contain_the_residue_pair, pair_of_full_residue_IDs, residue_pair_data, distance_delta_thr, angle_delta_thr, index_folder_path, compression):pair_of_full_residue_IDs
+        for pair_of_full_residue_IDs, residue_pair_data in all_pairs_of_residues_to_check.items()
+    }
+
+    # The dictionary of each residue pair has to be turned into bytes in order to be shareable across multiple processes, raw 
+    # dictionaries are not accepted by ShareableList. Also, given we are sharing a list, we need to keep a mapping between each 
+    # residue pair data and it's index position in the list (e.g: the data of residue pair ('A1', 'A2') is at index position [1]).
+    reference_motif_residue_pairs_data: List[bytes] = []
+    shared_memory_residue_pair_mapping: Dict[Tuple[str,str], int] = {}
+    for i, future in enumerate(as_completed(submitted_futures)):
+        if future.exception():
+            raise future.exception() # type: ignore
+
+        PDBs_that_contain_the_residue_pair = future.result()
+        pair_of_full_residue_IDs = submitted_futures[future]
+
+        reference_motif_residue_pairs_data.append(pickle.dumps(PDBs_that_contain_the_residue_pair)) # Byte encode with pickle
+        shared_memory_residue_pair_mapping[pair_of_full_residue_IDs] = i
+
+    return reference_motif_residue_pairs_data, shared_memory_residue_pair_mapping
+
+def load_data_from_shared_memory(
+        pair_of_full_residue_IDs: Tuple[str,str], shared_memory_residue_pair_mapping:Dict[Tuple[str,str],int], 
+        shared_memory_list: ShareableList[bytes]
+    ) -> Dict[str, List[Tuple[str, str]]]:
+    """
+    ...
+    """
+    list_index_position = shared_memory_residue_pair_mapping[pair_of_full_residue_IDs]
+    bytes_data = shared_memory_list[list_index_position]
+    PDBs_that_contain_the_residue_pair: Dict[str, List[Tuple[str, str]]] = pickle.loads(bytes_data)
+    return PDBs_that_contain_the_residue_pair
+
 def solve_motif_MST(
         motif_MST: nx.Graph, index_folder_path: Path, distance_delta_thr: float, angle_delta_thr: float, compression: str, 
+        shared_memory_list_name: str, shared_memory_residue_pair_mapping: Dict[Tuple[str,str], int] 
     ) -> Dict[str, List[nx.Graph]]:
     """
     ...
     """
     # Non-parallel version of find_PDBs_with_all_residue_pairs
     map_of_PDBs_with_all_residue_pairs: Dict[str, List[Tuple[str,str]]]
     map_of_PDBs_with_all_residue_pairs_initialized_flag: bool = False
-    visited_nodes_map: Dict[str, Set[str]] # Used for connectivity check
+    shared_memory_list: ShareableList[bytes] = ShareableList(name=shared_memory_list_name) # 'Connect' to the shared memory block
     for pair_of_full_residue_IDs, residue_pair_data in get_all_pairs_of_residues_in_motif_MST(motif_MST).items():
-        PDBs_that_contain_the_residue_pair = get_PDBs_that_contain_the_residue_pair(pair_of_full_residue_IDs, residue_pair_data, distance_delta_thr, angle_delta_thr, index_folder_path, compression)
+        if pair_of_full_residue_IDs in shared_memory_residue_pair_mapping:
+            PDBs_that_contain_the_residue_pair = load_data_from_shared_memory(pair_of_full_residue_IDs, shared_memory_residue_pair_mapping, shared_memory_list)
+        else:
+            PDBs_that_contain_the_residue_pair = get_PDBs_that_contain_the_residue_pair(pair_of_full_residue_IDs, residue_pair_data, distance_delta_thr, angle_delta_thr, index_folder_path, compression)
         
+
         if map_of_PDBs_with_all_residue_pairs_initialized_flag == False:
             map_of_PDBs_with_all_residue_pairs = defaultdict(list, PDBs_that_contain_the_residue_pair)
             map_of_PDBs_with_all_residue_pairs_initialized_flag = True
-            visited_nodes_map = {
-                PDB_ID:set(flatten_iterable(list_of_residue_pairs))
-                for PDB_ID, list_of_residue_pairs in map_of_PDBs_with_all_residue_pairs.items()
-            }
-
         else:
             update_map_of_PDBs_with_all_residue_pairs(
                 map_of_PDBs_with_all_residue_pairs, 
-                PDBs_that_contain_the_residue_pair,
-                visited_nodes_map
+                PDBs_that_contain_the_residue_pair
             )
+    # Clean up
+    shared_memory_list.shm.close() # 'Disconnect'
+    del shared_memory_residue_pair_mapping, shared_memory_list
 
-    # Non-parallel version of filter_out_PDBs_with_unconnected_residue_pairs. Using while loop + popitem()
-    # instead of a for loop to limit RAM usage.
+    # Non-parallel version of filter_out_PDBs_with_unconnected_residue_pairs
     add_resname_as_node_attribute(motif_MST) # Needed for subgraph monomorphism, see run_subgraph_monomorphism().
     filtered_PDBs_with_all_residue_pairs: Dict[str, List[nx.Graph]] =  {}
-    while map_of_PDBs_with_all_residue_pairs:
-        PDB_ID, pairs_of_residues = map_of_PDBs_with_all_residue_pairs.popitem()
+    for PDB_ID, pairs_of_residues in map_of_PDBs_with_all_residue_pairs.items():
         monomorphism_checked_motifs = run_subgraph_monomorphism(motif_MST, pairs_of_residues)
-        
-        if not monomorphism_checked_motifs: # These are the false positive PDBs, i.e PDBs that have all the residue pairs but where the monomorphism check doesn't find any similar motif
+
+        if not monomorphism_checked_motifs: # These are the false positive PDBs, i.e PDBs that have all the residue pairs but where the monomorphism check doesn't find any similar motif as a result of unconnected pairs of residues 
             continue
 
         filtered_PDBs_with_all_residue_pairs[PDB_ID] = monomorphism_checked_motifs
 
     return filtered_PDBs_with_all_residue_pairs
+    
+def motif_level_parallelisation(        
+        reference_motif_MST: nx.Graph, max_n_mutated_residues: int, residue_type_policy: Union[str, Dict[str,List[str]]],
+        reference_motif_residues_data: Dict[str, Residue], index_folder_path: Path, distance_delta_thr: float, 
+        angle_delta_thr: float, compression: str, concurrent_executor: ProcessPoolExecutor, 
+        motif_MST_filtered_PDBs_map: Dict[nx.Graph, Dict[str, List[nx.Graph]]]) -> None:
+    """
+    ...
+    """
+    # When dealing with many mutated versions of a reference motif, the data of the same residue pairs is often loaded over
+    # and over again, in particular the residue pair data of the reference motif. Given IO is one of the main speed 
+    # bottlenecks of the search procedure, loading this data once and sharing it between the parallel processes can speed 
+    # up the search. For that we use ShareableList, which enables different processes to access the same data directly from RAM.
+    reference_motif_residue_pairs_data, shared_memory_residue_pair_mapping = get_reference_motif_residue_pairs_data(
+        reference_motif_MST,
+        index_folder_path,
+        distance_delta_thr, angle_delta_thr,
+        compression,
+        concurrent_executor
+    )
+    shared_memory_list = ShareableList(reference_motif_residue_pairs_data)
+    shared_memory_list_name: str = shared_memory_list.shm.name
+    
+    # Motif level parallelisation code
+    try:
+        submitted_futures = {
+            concurrent_executor.submit(solve_motif_MST, motif_MST, index_folder_path, distance_delta_thr, angle_delta_thr, compression, shared_memory_list_name, shared_memory_residue_pair_mapping):motif_MST
+            for motif_MST in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, reference_motif_residues_data)
+        }
+
+        for future in as_completed(submitted_futures):
+            if future.exception():
+                raise future.exception() # type: ignore
+
+            filtered_PDBs_with_all_residue_pairs = future.result()
+            if filtered_PDBs_with_all_residue_pairs:
+                motif_MST = submitted_futures[future]
+                motif_MST_filtered_PDBs_map[motif_MST] = filtered_PDBs_with_all_residue_pairs
+    
+    except Exception as exception:
+        raise exception
+
+    finally:
+        # Clean up the shared memory
+        shared_memory_list.shm.close()
+        shared_memory_list.shm.unlink()
 
-def get_tqdm_progress_bar(total: int, desc: str) -> tqdm:
-    return tqdm(total=total, desc=desc, position=0, leave=True, smoothing=0, bar_format='{l_bar}{bar} | {n_fmt}/{total_fmt} | Ellapsed={elapsed}; Remaining={remaining} |')
+    return
 
 def get_PDBs_with_similar_motifs(
-        reference_motif_MST: nx.Graph, motif_residues_data: Dict[str, Residue], index_folder_path: Path, max_n_mutated_residues: int, 
+        reference_motif_MST: nx.Graph, reference_motif_residues_data: Dict[str, Residue], index_folder_path: Path, max_n_mutated_residues: int, 
         residue_type_policy: Union[str, Dict[str,List[str]]], distance_delta_thr: float, angle_delta_thr: float, compression: str, n_cores: int
     ) -> Dict[nx.Graph, Dict[str, List[nx.Graph]]]:
     """
     ...
     """
     motif_MST_filtered_PDBs_map: Dict[nx.Graph, Dict[str, List[nx.Graph]]] = {}
-    n_motifs_to_solve = sum(1 for _ in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, motif_residues_data))
-
+    n_motifs_to_solve = sum(1 for _ in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, reference_motif_residues_data))
     with ProcessPoolExecutor(max_workers=n_cores) as concurrent_executor:
-        # Residue-pair level parallelisation
-        if n_motifs_to_solve <= n_cores:
-            for motif_MST in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, motif_residues_data):
-                PDBs_with_all_residue_pairs = find_PDBs_with_all_residue_pairs(motif_MST, index_folder_path, distance_delta_thr, angle_delta_thr, compression, concurrent_executor)
-                filtered_PDBs_with_all_residue_pairs = filter_out_PDBs_with_unconnected_residue_pairs(PDBs_with_all_residue_pairs, motif_MST, concurrent_executor)
+        if n_motifs_to_solve < n_cores:
+            residue_pair_level_parallelisation(
+                reference_motif_MST, 
+                max_n_mutated_residues, residue_type_policy, 
+                reference_motif_residues_data, 
+                index_folder_path, 
+                distance_delta_thr, angle_delta_thr, 
+                compression, 
+                concurrent_executor,
+                motif_MST_filtered_PDBs_map
+            )
 
-                if filtered_PDBs_with_all_residue_pairs:
-                    motif_MST_filtered_PDBs_map[motif_MST] = filtered_PDBs_with_all_residue_pairs
-        
-        # Motif level parallelisation. When having to check a large number of motifs as a result of mutated residues provided 
-        # by the user, motif level parallelisation is ~35% faster than residue-pair level parallelisation.
+        # When having to check a large number of motifs as a result of mutated residues provided by the user, 
+        # motif level parallelisation is ~35% faster than residue-pair level parallelisation.
         else:
-            submitted_futures = {
-                concurrent_executor.submit(solve_motif_MST, motif_MST, index_folder_path, distance_delta_thr, angle_delta_thr, compression):motif_MST
-                for motif_MST in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, motif_residues_data)
-            }
-
-            tqdm_progress_bar = get_tqdm_progress_bar(total=n_motifs_to_solve, desc='Searched motifs')
-            for future in as_completed(submitted_futures):
-                if future.exception():
-                    raise future.exception() # type: ignore
-
-                filtered_PDBs_with_all_residue_pairs = future.result()
-                if filtered_PDBs_with_all_residue_pairs:
-                    motif_MST = submitted_futures[future]
-                    motif_MST_filtered_PDBs_map[motif_MST] = filtered_PDBs_with_all_residue_pairs
-
-                tqdm_progress_bar.update()
-
+            motif_level_parallelisation(
+                reference_motif_MST, 
+                max_n_mutated_residues, residue_type_policy, 
+                reference_motif_residues_data, 
+                index_folder_path, 
+                distance_delta_thr, angle_delta_thr, 
+                compression, 
+                concurrent_executor,
+                motif_MST_filtered_PDBs_map
+            )
+            
     return motif_MST_filtered_PDBs_map
 
 def search_index_for_PDBs_with_similar_motifs(
         index_folder_path: Path, PDB_file: Path, motif: Tuple[str,...], residue_type_policy: Union[str, Dict[str,List[str]]], max_n_mutated_residues: int, 
         distance_delta_thr: float, angle_delta_thr: float, n_cores: int
     ) -> Tuple[nx.Graph, Dict[nx.Graph, Dict[str, List[nx.Graph]]]]:
     """
     ...
     """
     if not index_folder_exists(index_folder_path):
         raise ValueError("Could not find all the index folders and files. Did you previously create the index with the 'create-index' command ? Does the index path point towards a pyScoMotif_index folder ?")
     
-    motif_residues_data = extract_motif_residues_from_PDB_file(PDB_file, motif)
-    data_of_all_pairs_of_residues_in_motif = get_data_of_all_pairs_of_residues_in_motif(motif_residues_data)
+    reference_motif_residues_data = extract_motif_residues_from_PDB_file(PDB_file, motif)
+    data_of_all_pairs_of_residues_in_motif = get_data_of_all_pairs_of_residues_in_motif(reference_motif_residues_data)
 
     # It would be inefficient to search the index for every single pair of residues in the motif in order to find PDBs that have a similar 
     # motif. Instead we can determine the Minimum Spanning Tree (MST) of the motif to limit the search to a subset of pairs that covers all the residues.
-    motif_MST = get_minimum_spanning_tree(data_of_all_pairs_of_residues_in_motif)
+    reference_motif_MST = get_minimum_spanning_tree(data_of_all_pairs_of_residues_in_motif)
 
     compression = detect_the_compression_algorithm_used_in_the_index(index_folder_path)
     
     PDBs_with_similar_motifs = get_PDBs_with_similar_motifs(
-        motif_MST, 
-        motif_residues_data, 
+        reference_motif_MST, 
+        reference_motif_residues_data, 
         index_folder_path,
         max_n_mutated_residues, 
         residue_type_policy,
         distance_delta_thr, 
         angle_delta_thr,
         compression,
         n_cores
     )
 
-    return motif_MST, PDBs_with_similar_motifs
+    return reference_motif_MST, PDBs_with_similar_motifs
```

### Comparing `pyscomotif-0.9.29/src/pyscomotif/motif_search_with_ShareableList.py` & `pyscomotif-0.9.9/src/pyscomotif/motif_search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,16 @@
-# This version of the motif search code attemps to speed up the search when dealing with many mutated motifs. The idea is that when 
-# dealing with many mutated versions of a reference motif, the data of the same residue pairs is generally loaded over and over again, 
-# in particular the residue pair data of the reference motif. The optimization is to therefore load the data of those residue pairs
-# once and share it between the parallel process, which can be done using a ShareableList.
-# There are two problems with this implementation that need to be addresses before the code can be relased:
-# 1) There is a warning that says the shared_memory object is leaked and was not properly cleaned up, despite running shm.close() and shm.unlink() in the code
-# 2) The ShareableList documentation says that all items in the list must be < 10M bytes, so the code might crash if there is a residue pair that has a lot of data.
-
 import itertools
-import pickle
 from collections import defaultdict
 from concurrent.futures import Future, ProcessPoolExecutor, as_completed
-from multiprocessing.shared_memory import ShareableList
 from pathlib import Path
 from typing import Dict, Iterator, List, Set, Tuple, Union
 
 import networkx as nx
 import pandas as pd
+from tqdm import tqdm
 
 from pyscomotif.constants import (AMINO_ACID_ALPHABET,
                                     AMINO_ACID_RELAXED_GROUPS_MAP,
                                     INDEX_ANGLE_BIN_SIZE,
                                     INDEX_DISTANCE_BIN_SIZE)
 from pyscomotif.data_containers import Residue, Residue_pair_data
 from pyscomotif.index_folders_and_files import index_folder_exists
@@ -349,37 +340,37 @@
 
 def add_resname_as_node_attribute(graph: nx.Graph) -> None:
     """
     """
     nx.set_node_attributes(graph, {node:{'resname':node[-1]} for node in graph.nodes}) # Each node is a residue_full_ID so [-1] returns the residue (ex: 'G', for Glycine)
     return
 
-def run_subgraph_monomorphism(motif_MST: nx.Graph, pairs_of_residues: List[Tuple[str,str]]) -> Union[None, List[nx.Graph]]:
+def run_subgraph_monomorphism(motif_MST: nx.Graph, pairs_of_residues: List[Tuple[str,str]]) -> List[nx.Graph]:
     """
     The returned list can be empty.
     """
     candidate_PDB_graph = nx.Graph(pairs_of_residues)
     add_resname_as_node_attribute(candidate_PDB_graph)
 
     graph_matcher = nx.algorithms.isomorphism.GraphMatcher(
         G1 = candidate_PDB_graph, G2 = motif_MST, 
         node_match = lambda node1,node2: node1['resname'] == node2['resname'] # Match based on residue name
     )
-
+    
     monomorphism_checked_motifs: List[nx.Graph] = [] # Each PDB can have multiple motifs (i.e: homodimers) -> List[nx.Graph]
     residue_mapping_dict: Dict[str,str]
     for residue_mapping_dict in graph_matcher.subgraph_monomorphisms_iter():
         residues_of_the_similar_motif = list(residue_mapping_dict.keys())
         similar_motif_graph: nx.Graph = candidate_PDB_graph.subgraph(residues_of_the_similar_motif).copy()
         
         setattr(similar_motif_graph, 'residue_mapping_dict', residue_mapping_dict) # Used for RMSD calculation
 
         monomorphism_checked_motifs.append(similar_motif_graph)
 
-    return monomorphism_checked_motifs if monomorphism_checked_motifs else None
+    return monomorphism_checked_motifs
 
 def filter_out_PDBs_with_unconnected_residue_pairs(
         PDBs_with_all_residue_pairs: Dict[str, List[Tuple[str,str]]], motif_MST: nx.Graph, concurrent_executor: ProcessPoolExecutor, 
     ) -> Dict[str, List[nx.Graph]]:
     """
     """
     # To know if a PDB contains a set of connected residue pairs forming a similar motif, we use subgraph monomorphism to perform a matching between a reference 
@@ -407,230 +398,119 @@
             continue
 
         PDB_ID = submited_futures[future]
         filtered_PDBs_with_all_residue_pairs[PDB_ID] = monomorphism_checked_motifs
 
     return filtered_PDBs_with_all_residue_pairs
 
-def residue_pair_level_parallelisation(
-        reference_motif_MST: nx.Graph, max_n_mutated_residues: int, residue_type_policy: Union[str, Dict[str,List[str]]],
-        reference_motif_residues_data: Dict[str, Residue], index_folder_path: Path, distance_delta_thr: float, 
-        angle_delta_thr: float, compression: str, concurrent_executor: ProcessPoolExecutor, 
-        motif_MST_filtered_PDBs_map: Dict[nx.Graph, Dict[str, List[nx.Graph]]]
-    ) -> None:
-    """
-    ...
-    """
-    for motif_MST in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, reference_motif_residues_data):
-        PDBs_with_all_residue_pairs = find_PDBs_with_all_residue_pairs(motif_MST, index_folder_path, distance_delta_thr, angle_delta_thr, compression, concurrent_executor)
-        filtered_PDBs_with_all_residue_pairs = filter_out_PDBs_with_unconnected_residue_pairs(PDBs_with_all_residue_pairs, motif_MST, concurrent_executor)
-        
-        if filtered_PDBs_with_all_residue_pairs:
-            motif_MST_filtered_PDBs_map[motif_MST] = filtered_PDBs_with_all_residue_pairs
-    
-    return
-
-def get_reference_motif_residue_pairs_data(
-        reference_motif_MST: nx.Graph, index_folder_path: Path, distance_delta_thr: float, angle_delta_thr: float, 
-        compression: str, concurrent_executor: ProcessPoolExecutor
-    ) -> Tuple[List[bytes], Dict[Tuple[str,str], int]]:
-    """
-    ...
-    """
-    # First load all the residue pair data of the reference_motif_MST
-    all_pairs_of_residues_to_check = get_all_pairs_of_residues_in_motif_MST(reference_motif_MST)
-    
-    submitted_futures: Dict[Future[Dict[str, List[Tuple[str,str]]]], Tuple[str,str]] = {
-        concurrent_executor.submit(get_PDBs_that_contain_the_residue_pair, pair_of_full_residue_IDs, residue_pair_data, distance_delta_thr, angle_delta_thr, index_folder_path, compression):pair_of_full_residue_IDs
-        for pair_of_full_residue_IDs, residue_pair_data in all_pairs_of_residues_to_check.items()
-    }
-
-    # The dictionary of each residue pair has to be turned into bytes in order to be shareable across multiple processes, raw 
-    # dictionaries are not accepted by ShareableList. Also, given we are sharing a list, we need to keep a mapping between each 
-    # residue pair data and it's index position in the list (e.g: the data of residue pair ('A1', 'A2') is at index position [1]).
-    reference_motif_residue_pairs_data: List[bytes] = []
-    shared_memory_residue_pair_mapping: Dict[Tuple[str,str], int] = {}
-    for i, future in enumerate(as_completed(submitted_futures)):
-        if future.exception():
-            raise future.exception() # type: ignore
-
-        PDBs_that_contain_the_residue_pair = future.result()
-        pair_of_full_residue_IDs = submitted_futures[future]
-
-        reference_motif_residue_pairs_data.append(pickle.dumps(PDBs_that_contain_the_residue_pair)) # Byte encode with pickle
-        shared_memory_residue_pair_mapping[pair_of_full_residue_IDs] = i
-
-    return reference_motif_residue_pairs_data, shared_memory_residue_pair_mapping
-
-def load_data_from_shared_memory(
-        pair_of_full_residue_IDs: Tuple[str,str], shared_memory_residue_pair_mapping:Dict[Tuple[str,str],int], 
-        shared_memory_list: ShareableList[bytes]
-    ) -> Dict[str, List[Tuple[str, str]]]:
-    """
-    ...
-    """
-    list_index_position = shared_memory_residue_pair_mapping[pair_of_full_residue_IDs]
-    bytes_data = shared_memory_list[list_index_position]
-    PDBs_that_contain_the_residue_pair: Dict[str, List[Tuple[str, str]]] = pickle.loads(bytes_data)
-    return PDBs_that_contain_the_residue_pair
-
 def solve_motif_MST(
         motif_MST: nx.Graph, index_folder_path: Path, distance_delta_thr: float, angle_delta_thr: float, compression: str, 
-        shared_memory_list_name: str, shared_memory_residue_pair_mapping: Dict[Tuple[str,str], int] 
     ) -> Dict[str, List[nx.Graph]]:
     """
     ...
     """
     # Non-parallel version of find_PDBs_with_all_residue_pairs
     map_of_PDBs_with_all_residue_pairs: Dict[str, List[Tuple[str,str]]]
     map_of_PDBs_with_all_residue_pairs_initialized_flag: bool = False
-    shared_memory_list: ShareableList[bytes] = ShareableList(name=shared_memory_list_name) # 'Connect' to the shared memory block
     for pair_of_full_residue_IDs, residue_pair_data in get_all_pairs_of_residues_in_motif_MST(motif_MST).items():
-        if pair_of_full_residue_IDs in shared_memory_residue_pair_mapping:
-            PDBs_that_contain_the_residue_pair = load_data_from_shared_memory(pair_of_full_residue_IDs, shared_memory_residue_pair_mapping, shared_memory_list)
-        else:
-            PDBs_that_contain_the_residue_pair = get_PDBs_that_contain_the_residue_pair(pair_of_full_residue_IDs, residue_pair_data, distance_delta_thr, angle_delta_thr, index_folder_path, compression)
+        PDBs_that_contain_the_residue_pair = get_PDBs_that_contain_the_residue_pair(pair_of_full_residue_IDs, residue_pair_data, distance_delta_thr, angle_delta_thr, index_folder_path, compression)
         
-
         if map_of_PDBs_with_all_residue_pairs_initialized_flag == False:
             map_of_PDBs_with_all_residue_pairs = defaultdict(list, PDBs_that_contain_the_residue_pair)
             map_of_PDBs_with_all_residue_pairs_initialized_flag = True
+
         else:
             update_map_of_PDBs_with_all_residue_pairs(
                 map_of_PDBs_with_all_residue_pairs, 
                 PDBs_that_contain_the_residue_pair
             )
-    # Clean up
-    shared_memory_list.shm.close() # 'Disconnect'
-    del shared_memory_residue_pair_mapping, shared_memory_list
 
     # Non-parallel version of filter_out_PDBs_with_unconnected_residue_pairs
+    #print(f'Filtering {len(map_of_PDBs_with_all_residue_pairs)} target motifs.')
     add_resname_as_node_attribute(motif_MST) # Needed for subgraph monomorphism, see run_subgraph_monomorphism().
     filtered_PDBs_with_all_residue_pairs: Dict[str, List[nx.Graph]] =  {}
     for PDB_ID, pairs_of_residues in map_of_PDBs_with_all_residue_pairs.items():
         monomorphism_checked_motifs = run_subgraph_monomorphism(motif_MST, pairs_of_residues)
 
         if not monomorphism_checked_motifs: # These are the false positive PDBs, i.e PDBs that have all the residue pairs but where the monomorphism check doesn't find any similar motif as a result of unconnected pairs of residues 
             continue
 
         filtered_PDBs_with_all_residue_pairs[PDB_ID] = monomorphism_checked_motifs
 
     return filtered_PDBs_with_all_residue_pairs
-    
-def motif_level_parallelisation(        
-        reference_motif_MST: nx.Graph, max_n_mutated_residues: int, residue_type_policy: Union[str, Dict[str,List[str]]],
-        reference_motif_residues_data: Dict[str, Residue], index_folder_path: Path, distance_delta_thr: float, 
-        angle_delta_thr: float, compression: str, concurrent_executor: ProcessPoolExecutor, 
-        motif_MST_filtered_PDBs_map: Dict[nx.Graph, Dict[str, List[nx.Graph]]]) -> None:
-    """
-    ...
-    """
-    # When dealing with many mutated versions of a reference motif, the data of the same residue pairs is often loaded over
-    # and over again, in particular the residue pair data of the reference motif. Given IO is one of the main speed 
-    # bottlenecks of the search procedure, loading this data once and sharing it between the parallel processes can speed 
-    # up the search. For that we use ShareableList, which enables different processes to access the same data directly from RAM.
-    reference_motif_residue_pairs_data, shared_memory_residue_pair_mapping = get_reference_motif_residue_pairs_data(
-        reference_motif_MST,
-        index_folder_path,
-        distance_delta_thr, angle_delta_thr,
-        compression,
-        concurrent_executor
-    )
-    shared_memory_list = ShareableList(reference_motif_residue_pairs_data)
-    shared_memory_list_name: str = shared_memory_list.shm.name
-    
-    # Motif level parallelisation code
-    try:
-        submitted_futures = {
-            concurrent_executor.submit(solve_motif_MST, motif_MST, index_folder_path, distance_delta_thr, angle_delta_thr, compression, shared_memory_list_name, shared_memory_residue_pair_mapping):motif_MST
-            for motif_MST in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, reference_motif_residues_data)
-        }
-
-        for future in as_completed(submitted_futures):
-            if future.exception():
-                raise future.exception() # type: ignore
-
-            filtered_PDBs_with_all_residue_pairs = future.result()
-            if filtered_PDBs_with_all_residue_pairs:
-                motif_MST = submitted_futures[future]
-                motif_MST_filtered_PDBs_map[motif_MST] = filtered_PDBs_with_all_residue_pairs
-    
-    except Exception as exception:
-        raise exception
-
-    finally:
-        # Clean up the shared memory
-        shared_memory_list.shm.close()
-        shared_memory_list.shm.unlink()
 
-    return
+def get_tqdm_progress_bar(total: int, desc: str) -> tqdm:
+    return tqdm(total=total, desc=desc, position=0, leave=True, smoothing=0, bar_format='{l_bar}{bar} | {n_fmt}/{total_fmt} | Ellapsed={elapsed}; Remaining={remaining} |')
 
 def get_PDBs_with_similar_motifs(
-        reference_motif_MST: nx.Graph, reference_motif_residues_data: Dict[str, Residue], index_folder_path: Path, max_n_mutated_residues: int, 
+        reference_motif_MST: nx.Graph, motif_residues_data: Dict[str, Residue], index_folder_path: Path, max_n_mutated_residues: int, 
         residue_type_policy: Union[str, Dict[str,List[str]]], distance_delta_thr: float, angle_delta_thr: float, compression: str, n_cores: int
     ) -> Dict[nx.Graph, Dict[str, List[nx.Graph]]]:
     """
     ...
     """
     motif_MST_filtered_PDBs_map: Dict[nx.Graph, Dict[str, List[nx.Graph]]] = {}
-    n_motifs_to_solve = sum(1 for _ in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, reference_motif_residues_data))
+    n_motifs_to_solve = sum(1 for _ in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, motif_residues_data))
     with ProcessPoolExecutor(max_workers=n_cores) as concurrent_executor:
+        # Residue-pair level parallelisation
         if n_motifs_to_solve < n_cores:
-            residue_pair_level_parallelisation(
-                reference_motif_MST, 
-                max_n_mutated_residues, residue_type_policy, 
-                reference_motif_residues_data, 
-                index_folder_path, 
-                distance_delta_thr, angle_delta_thr, 
-                compression, 
-                concurrent_executor,
-                motif_MST_filtered_PDBs_map
-            )
-
-        # When having to check a large number of motifs as a result of mutated residues provided by the user, 
-        # motif level parallelisation is ~35% faster than residue-pair level parallelisation.
+            for motif_MST in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, motif_residues_data):
+                PDBs_with_all_residue_pairs = find_PDBs_with_all_residue_pairs(motif_MST, index_folder_path, distance_delta_thr, angle_delta_thr, compression, concurrent_executor)
+                filtered_PDBs_with_all_residue_pairs = filter_out_PDBs_with_unconnected_residue_pairs(PDBs_with_all_residue_pairs, motif_MST, concurrent_executor)
+                
+                if filtered_PDBs_with_all_residue_pairs:
+                    motif_MST_filtered_PDBs_map[motif_MST] = filtered_PDBs_with_all_residue_pairs
+        
+        # Motif level parallelisation. When having to check a large number of motifs as a result of mutated residues provided 
+        # by the user, motif level parallelisation is ~35% faster than residue-pair level parallelisation.
         else:
-            motif_level_parallelisation(
-                reference_motif_MST, 
-                max_n_mutated_residues, residue_type_policy, 
-                reference_motif_residues_data, 
-                index_folder_path, 
-                distance_delta_thr, angle_delta_thr, 
-                compression, 
-                concurrent_executor,
-                motif_MST_filtered_PDBs_map
-            )
-            
+            submitted_futures = {
+                concurrent_executor.submit(solve_motif_MST, motif_MST, index_folder_path, distance_delta_thr, angle_delta_thr, compression):motif_MST
+                for motif_MST in get_all_motif_MSTs_generator(reference_motif_MST, max_n_mutated_residues, residue_type_policy, motif_residues_data)
+            }
+
+            tqdm_progress_bar = get_tqdm_progress_bar(total=n_motifs_to_solve, desc='Searched motifs')
+            for future in as_completed(submitted_futures):
+                if future.exception():
+                    raise future.exception() # type: ignore
+
+                filtered_PDBs_with_all_residue_pairs = future.result()
+                if filtered_PDBs_with_all_residue_pairs:
+                    motif_MST = submitted_futures[future]
+                    motif_MST_filtered_PDBs_map[motif_MST] = filtered_PDBs_with_all_residue_pairs
+
+                tqdm_progress_bar.update()
+
     return motif_MST_filtered_PDBs_map
 
 def search_index_for_PDBs_with_similar_motifs(
         index_folder_path: Path, PDB_file: Path, motif: Tuple[str,...], residue_type_policy: Union[str, Dict[str,List[str]]], max_n_mutated_residues: int, 
         distance_delta_thr: float, angle_delta_thr: float, n_cores: int
     ) -> Tuple[nx.Graph, Dict[nx.Graph, Dict[str, List[nx.Graph]]]]:
     """
     ...
     """
     if not index_folder_exists(index_folder_path):
         raise ValueError("Could not find all the index folders and files. Did you previously create the index with the 'create-index' command ? Does the index path point towards a pyScoMotif_index folder ?")
     
-    reference_motif_residues_data = extract_motif_residues_from_PDB_file(PDB_file, motif)
-    data_of_all_pairs_of_residues_in_motif = get_data_of_all_pairs_of_residues_in_motif(reference_motif_residues_data)
+    motif_residues_data = extract_motif_residues_from_PDB_file(PDB_file, motif)
+    data_of_all_pairs_of_residues_in_motif = get_data_of_all_pairs_of_residues_in_motif(motif_residues_data)
 
     # It would be inefficient to search the index for every single pair of residues in the motif in order to find PDBs that have a similar 
     # motif. Instead we can determine the Minimum Spanning Tree (MST) of the motif to limit the search to a subset of pairs that covers all the residues.
-    reference_motif_MST = get_minimum_spanning_tree(data_of_all_pairs_of_residues_in_motif)
+    motif_MST = get_minimum_spanning_tree(data_of_all_pairs_of_residues_in_motif)
 
     compression = detect_the_compression_algorithm_used_in_the_index(index_folder_path)
     
     PDBs_with_similar_motifs = get_PDBs_with_similar_motifs(
-        reference_motif_MST, 
-        reference_motif_residues_data, 
+        motif_MST, 
+        motif_residues_data, 
         index_folder_path,
         max_n_mutated_residues, 
         residue_type_policy,
         distance_delta_thr, 
         angle_delta_thr,
         compression,
         n_cores
     )
 
-    return reference_motif_MST, PDBs_with_similar_motifs
+    return motif_MST, PDBs_with_similar_motifs
```

### Comparing `pyscomotif-0.9.29/src/pyscomotif/pyscomotif.py` & `pyscomotif-0.9.9/src/pyscomotif/pyscomotif.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,40 +11,31 @@
 
 from pyscomotif.constants import (INDEX_MAX_ANGLE_VALUE,
                                     INDEX_MAX_DISTANCE_VALUE)
 from pyscomotif.indexing import create_index_folder, update_index_folder
 from pyscomotif.motif_search import search_index_for_PDBs_with_similar_motifs
 from pyscomotif.RMSD_calculation import calculate_RMSD_between_motif_and_similar_motifs
 
-DISCLAIMER = """
-\n
-DISCLAIMER: pyScoMotif is free to use for non-commercial purposes. To use pyScoMotif for commercial purposes, please contact us.
-pyScoMotif is developed by the 3BioInfo group from the ULB, Belgium.
-Reference paper: 'pyScoMotif: Discovery of similar 3D structural motifs across proteins'.
-Main developer: Gabriel Cia.
-\n
-"""
 
-@click.group(help='pyScoMotif: a tool for the discovery of similar 3D structural motifs across proteins.', context_settings={'max_content_width':2000}, epilog=DISCLAIMER)
+@click.group(help='pyScoMotif: a tool for the discovery of similar 3D structural motifs across proteins.', context_settings={'max_content_width':2000})
 def command_line_interface() -> None:
     pass
 
 
 def check_index_path_option(ctx: Any, param: Any, value: Union[None, Path]) -> Path:
     if value:
         return value
-    
+
     default_index_folder_path: Path = ctx.params['database_path'] / 'pyScoMotif_index'
     # In Click, callbacks run AFTER type casting and its associated validation, so we have to re-run the validations.
-    default_index_folder_path = click.Path(file_okay=False, dir_okay=True, readable=True, writable=True, path_type=Path).convert(default_index_folder_path, ctx=ctx, param=param)
-    
+    click.Path(file_okay=False, dir_okay=True, readable=True, writable=True, path_type=Path).convert(default_index_folder_path, ctx=ctx, param=param)
+ 
     return default_index_folder_path
 
-
-@command_line_interface.command(epilog=DISCLAIMER)
+@command_line_interface.command()
 @click.argument('database_path', type=click.Path(exists=True, file_okay=False, dir_okay=True, readable=True, path_type=Path))
 @click.option('--index_path', default=None, show_default=False, type=click.Path(file_okay=False, dir_okay=True, readable=True, writable=True, path_type=Path), 
               callback=check_index_path_option, help="Full path of the directory that will contain the index files. Defaults to <database_path>/pyScoMotif_index.")
 @click.option('--pattern', type=str, default='*.pdb', show_default=True,
                help="File extension pattern of the PDB files in the database that the file detection algorithm should match, including compression. Examples: *.pdb, *.pdb.gz, *.ent , etcetc . Note the use of the '*' wildcard. Also note that only simple unix style patterns are accepted, complex regex patterns will fail. To know if your pattern works, test it with pathlib.Path.rglob.")
 @click.option('--compression', type=click.Choice(('bz2', 'gz')), default='bz2', show_default=True,
                help="Compression algorithm to use to compress the index files. This has nothing to do with the compression of the PDB files, for that use the '--pattern' option.")
@@ -63,19 +54,18 @@
     ---------
     DATABASE_PATH  Full path of the directory containing the PDB files to index (e.g: /home/user/Downloads/PDB). The file detection algorithm is recursive, 
     so PDB files in subfolders will also be indexed.
     """
     create_index_folder(database_path, pattern, index_path, compression, n_cores)
     return
 
-
-@command_line_interface.command(epilog=DISCLAIMER)
+@command_line_interface.command()
 @click.argument('database_path', type=click.Path(exists=True, file_okay=False, dir_okay=True, readable=True, path_type=Path))
 @click.argument('index_path', type=click.Path(exists=True, file_okay=False, dir_okay=True, writable=True, readable=True, path_type=Path))
-@click.option('--pattern', type=str, default='*.pdb', show_default=True,
+@click.option('--pattern', type=str, default='*.pdb',
                help="File extension pattern of the PDB files in the database that the file detection algorithm should match. Examples: *.pdb, *.pdb.gz, *.ent , etcetc . Note the use of the '*' wildcard. Also note that only simple unix style patterns are accepted, complex regex patterns will fail. To know if your pattern works, test it with pathlib.Path.rglob.")
 @click.option('--n_cores', default=1, show_default=True,
                help='Number of cores to use.')
 def update_index(database_path: Path, pattern: str, index_path: Path, n_cores: int) -> None:
     """
     Command to update an existing pyScoMotif index with new PDB files. The new PDB files are determined by comparing the name 
     of the PDB files with those that have already been indexed, which are stored in the 'indexed_PDB_files.txt' file.
@@ -116,15 +106,15 @@
         loaded_json: Dict[str,str] = json.loads(value) # loads = load string
         position_specific_exchange: Dict[str, List[str]] = {key:list(value) for key, value in loaded_json.items()} # Ex: {'A43':'KRH'} -> {'A43':['K', 'R', 'H']}
     except JSONDecodeError as exception:
         raise exception
 
     return position_specific_exchange
 
-@command_line_interface.command(epilog=DISCLAIMER)
+@command_line_interface.command()
 @click.argument('index_path', type=click.Path(exists=True, path_type=Path))
 @click.argument('PDB_file', type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True, path_type=Path))
 @click.argument('motif', nargs=-1, callback=check_motif_argument) # -1 => Unlimited number of arguments
 @click.option('--results_output_path', type=click.Path(path_type=Path), default=None, callback=check_results_output_path_option,
               help='Full path of the csv file where the results will be saved (e.g: /home/user/Downloads/similar_motifs.csv). If not given, the results will be saved in the current working directory in a file named with the current timestamp (e.g: pyScoMotif_result_14230214102022.csv)')
 @click.option('--residue_type_policy', default='strict', callback=check_residue_type_policy_option,
                help='''Option to control whether mutated versions of the query motif should also be tested. There are 4 possible values: 1) strict (DEFAULT): only similar motifs with strictly identical residues to the query motif are searched. 2) relaxed: finds PDBs with motifs that are similar but with potential mutated residues by allowing residues to mutate according to the residue group they are part of, such as polar, positively charged, aromatic, etcetc (see our Github for the exact grouping of the residues). 3) fully_relaxed: similar to the relaxed mode, but residues can be mutated to any of the 20 possible residues. 4) custom position specific exchange: specify possible residue mutations for the desired positions in your motif using a JSON formated string (e.g: '{"A1":"KL", "A2":"YW", "A5":"E"}'. Note the use of single and double quotes).\n To control the maximum number of simultaneous mutations, see the max_n_mutated_residues option.''')
@@ -181,8 +171,14 @@
         print('No PDB structure with a similar motif was found.')
 
     return
 
 if __name__ == '__main__':
     #scalene_profiler.start()
     command_line_interface(max_content_width=2000) # max_content_width=2000 allows help texts to span the entire width of the terminal
-    #scalene_profiler.stop()
+    #scalene_profiler.stop()
+    
+
+# What if the distance is outside of the available distances, say C_alpha_distance of 25 angstroom in an index made with max 20 angstroom ???
+# Could stop the solve_motif function earlier by checking if the current list of PDBs with all the pairs is empty, in which case we can stop computing the remaining pairs.
+# Currently we don't recalculate the sidechain CMR coordinates of mutated residues in the reference motif, although in theory we should probably do it
+
```

### Comparing `pyscomotif-0.9.29/src/pyscomotif/residue_data_dicts.py` & `pyscomotif-0.9.9/src/pyscomotif/residue_data_dicts.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,17 +139,17 @@
     }
 
     add_C_alpha_attribute(residue_data)
     add_sidechain_CMR_attribute(residue_data)
     add_C_alpha_sidechain_CMR_vector_attribute(residue_data)
 
     # The Biopython Residue objects contain a lot of data we are not interested in, so we replace them with our own Residue object 
-    # that only contains the data we actually care about. 
-    # We also want to have access to the PDB's header description/title, which is why we use a UserDict which allows us to add that 
-    # string as an attribute to the UserDict object instead of a key in the dictionary, which would be confusing as it's not a Residue object.
+    # that only contains the data we actually care about. We also want to have access to the PDB's header description/title, which
+    # is why we use a UserDict which allows us to add that string as an attribute to the UserDict object instead of a key in the dictionary,
+    # which would be confusing as it's not a Residue object.
     customized_residue_data = UserDict({
         residue_id:Residue(resname=protein_letters_3to1_extended[residue.resname], C_alpha=residue.C_alpha, sidechain_CMR=residue.sidechain_CMR, vector=residue.vector)
         for residue_id, residue in residue_data.items()
         if residue.resname in protein_letters_3to1_extended
     })
     add_PDB_header_description_as_dict_attribute(customized_residue_data, parsed_PDB_file)
```

### Comparing `pyscomotif-0.9.29/src/pyscomotif/utils.py` & `pyscomotif-0.9.9/src/pyscomotif/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import bz2
 import gzip
 import itertools
 import pickle
 from pathlib import Path
-from typing import Any, List, Tuple, Union, Iterable
+from typing import Any, List, Tuple, Union
 
 import numba
 import numpy as np
 import numpy.typing as npt
 
 from pyscomotif.constants import AMINO_ACID_ALPHABET
 from pyscomotif.data_containers import Residue
@@ -18,16 +18,14 @@
 
 def get_sorted_2_tuple(tuple_: Tuple[Any, Any]) -> Tuple[Any, Any]:
     return tuple_ if tuple_[0] <= tuple_[1] else (tuple_[1], tuple_[0])
 
 def sort_and_join_2_strings(str1: str, str2: str) -> str:
     return str1+str2 if str1 <= str2 else str2+str1
 
-def flatten_iterable(iterable: Iterable[Any]) -> Iterable[Any]:
-    return itertools.chain.from_iterable(iterable)
 
 def pickle_and_compress_python_object(python_object: Any, output_file_path: Path) -> None:
     """
     ...
     """
     if output_file_path.suffix == '.bz2':
         with bz2.open(output_file_path, 'wb') as file_handle:
```

