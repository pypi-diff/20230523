# Comparing `tmp/algorithmadts-0.1.2.tar.gz` & `tmp/algorithmadts-0.1.4.tar.gz`

## Comparing `algorithmadts-0.1.2.tar` & `algorithmadts-0.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.DS_Store
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/.vscode/settings.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/src/AlgorithmADTs/.DS_Store
--rw-r--r--   0        0        0    12317 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/src/AlgorithmADTs/AbstractDataTypes.py
--rw-r--r--   0        0        0     7391 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/src/AlgorithmADTs/GraphAlgorithms.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/src/AlgorithmADTs/__init__.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/tests/experimenting.ipynb
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/tests/test_GraphAlgorithms.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/LICENSE
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/README.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4309 2020-02-02 00:00:00.000000 algorithmadts-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/.DS_Store
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/.vscode/settings.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/src/AlgorithmADTs/.DS_Store
+-rw-r--r--   0        0        0    12193 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/src/AlgorithmADTs/AbstractDataTypes.py
+-rw-r--r--   0        0        0     7358 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/src/AlgorithmADTs/GraphAlgorithms.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/src/AlgorithmADTs/__init__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/tests/experimenting.ipynb
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/tests/test_GraphAlgorithms.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/README.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 algorithmadts-0.1.4/PKG-INFO
```

### Comparing `algorithmadts-0.1.2/.DS_Store` & `algorithmadts-0.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.2/src/.DS_Store` & `algorithmadts-0.1.4/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.2/src/AlgorithmADTs/.DS_Store` & `algorithmadts-0.1.4/src/AlgorithmADTs/.DS_Store`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.2/src/AlgorithmADTs/AbstractDataTypes.py` & `algorithmadts-0.1.4/src/AlgorithmADTs/AbstractDataTypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any
 
-infinity = float('inf')
+infinity = float("inf")
+
 
 class Array:
     @classmethod
     def create(cls, length: int):
         return cls(length)
 
     def __init__(self, length: int):
@@ -36,22 +37,23 @@
         return f"Array({self.__repr__()})"
 
     def __repr__(self):
         return str(list(self._dictionary.values()))
 
     def __len__(self):
         return self._length
-    
+
     def __eq__(self, other):
-        if isinstance(other,Array):
+        if isinstance(other, Array):
             if len(self) == len(other) and self._dictionary == other._dictionary:
                 return True
         return False
 
-class Matrix():
+
+class Matrix:
     @classmethod
     def create(cls, rows: int, columns: int):
         return cls(rows, columns)
 
     def __init__(self, rows: int, columns: int):
         self._shape = (rows, columns)
         self._rows = rows
@@ -60,111 +62,111 @@
         self._values = Array(rows)
         for j in range(columns):
             self._values[j] = Array(columns)
 
     def get(self, row: int, column: int | None = None):
         if not (0 <= row < self._rows):
             raise ValueError(f"Incorrect index value {row}")
-        
+
         if column is None:
             return self._values[row]
-        
+
         if not (0 <= column < self._columns):
             raise ValueError(f"Incorrect index value {row}")
-        
+
         return self._values[row][column]
 
     def set(self, row: int, column: int, value: int | float | bool | None):
         if not (0 <= row < self._rows):
             raise ValueError(f"Incorrect index value {row}")
         if not (0 <= column < self._columns):
             raise ValueError(f"Incorrect index value {row}")
 
         self._values[row][column] = value
         return self
 
     def __getitem__(self, a: int | tuple):
         if isinstance(a, int):
             return self.get(a, None)
-        
+
         if not len(a) == 2:
             raise ValueError("Too many values. Only two dimensional")
-        
+
         return self.get(a[0], a[1])
 
     def __setitem__(self, a: int | tuple, value: int | float | bool | None):
         if isinstance(a, int):
             raise ValueError()
-        
+
         if not len(a) == 2:
             raise ValueError("Too many values. Only two dimensional")
-        
+
         return self.set(a[0], a[1], value)
 
     def __iter__(self):
         return self._values.__iter__()
 
     def __str__(self):
         return f"Matrix({self.__repr__()})"
 
     def __repr__(self):
         return str(self._values)
-    
+
     def __eq__(self, other):
-        if isinstance(other,Matrix):
+        if isinstance(other, Matrix):
             if self._shape == other._shape and self._values == other._values:
                 return True
         return False
-        
+
     def __add__(self, other):
         if not isinstance(other, Matrix):
             raise NotImplementedError()
-        
+
         if other._shape != self._shape:
             raise ValueError("Matrices must have identical shapes")
-        
+
         new = Matrix(self._shape[0], self._shape[1])
         for i in range(self._rows):
             for j in range(self._columns):
-                new[i,j] = self[i][j] + other[i][j]
+                new[i, j] = self[i][j] + other[i][j]
         return new
 
     def __sub__(self, other):
         if not isinstance(other, Matrix):
             raise NotImplementedError()
-        
+
         if other._shape != self._shape:
             raise ValueError("Matrices must have identical shapes")
-        
+
         new = Matrix(self._rows, self._columns)
         for i in range(self._rows):
             for j in range(self._columns):
-                new[i,j] = self[i][j] - other[i][j]
+                new[i, j] = self[i][j] - other[i][j]
         return new
 
     def __mul__(self, other):
         if isinstance(other, int) or isinstance(other, float):
             new = Matrix(self._rows, self._columns)
             for i in range(self._rows):
                 for j in range(self._columns):
-                    new[i,j] = other * self[i,j] 
+                    new[i, j] = other * self[i, j]
 
         if not isinstance(other, Matrix):
             raise NotImplementedError()
-        
+
         if not self._columns == other._rows:
             raise ValueError("column of first matrix must equal row of second")
-        
+
         new = Matrix(self._rows, other._columns)
         for i in range(self._rows):
             for j in range(self._columns):
-                new[i,j] = sum(self[i,k]*other[k,j] for k in range(self._columns))
+                new[i, j] = sum(self[i, k] * other[k, j] for k in range(self._columns))
 
         return new
-    
+
 
 class List:
     @classmethod
     def create(cls):
         return cls()
 
     def __init__(self):
@@ -207,20 +209,21 @@
         return f"List({self.__repr__()})"
 
     def __repr__(self):
         return str(self._list)
 
     def __len__(self):
         return len(self._list)
-    
+
     def __eq__(self, other):
         if isinstance(other, List):
             return self._list == other._list
         return False
 
+
 class Stack:
     @staticmethod
     def create():
         return Stack()
 
     def __init__(self):
         self._list: list[Any] = []
@@ -241,14 +244,15 @@
 
     def __str__(self):
         return f"Stack({self.__repr__()})"
 
     def __repr__(self):
         return f"Head: {self.head()}"
 
+
 class Queue:
     @staticmethod
     def create():
         return Queue()
 
     def __init__(self):
         self._list: list[Any] = []
@@ -269,14 +273,15 @@
 
     def __str__(self):
         return f"Queue({self.__repr__()})"
 
     def __repr__(self):
         return f"Head: {self.head()}"
 
+
 class PriorityQueue:
     @staticmethod
     def create():
         return PriorityQueue()
 
     def __init__(self):
         self._list: list[tuple[Any, int]] = []
@@ -298,14 +303,15 @@
 
     def __str__(self):
         return f"PriorityQueue({self.__repr__()})"
 
     def __repr__(self):
         return f"Head: {self.head()}"
 
+
 class Dictionary:
     @staticmethod
     def create():
         return Dictionary()
 
     def __init__(self):
         self._keys: list[Any] = []
@@ -356,20 +362,21 @@
         return self._keys.__iter__()
 
     def __str__(self):
         return f"Dictionary({self.__repr__()})"
 
     def __repr__(self):
         return f"keys: {str(self._keys)}"
-    
+
     def __eq__(self, other):
         if isinstance(other, Dictionary):
             return self._keys == other._keys and self._values == other._values
         return False
 
+
 class Graph:
     @staticmethod
     def create(*, directed=False):
         return Graph(directed=directed)
 
     def __init__(self, *, directed=False):
         self._nodes: list[Any] = []
@@ -392,15 +399,15 @@
     @property
     def edges(self):
         return self._edges
 
     def add_node(self, node: Any):
         self._nodes.append(node)
         return self
-    
+
     def add_edge(self, node1: Any, node2: Any):
         if not (node1 in self._nodes and node2 in self._nodes):
             raise ValueError("Nodes must already be in the graph")
 
         self._edges.append((node1, node2))
         if not self._directed:
             self._edges.append((node2, node1))
@@ -412,15 +419,15 @@
             self.add_node(node)
         return self
 
     def add_edges(self, edges: Any):
         for edge in edges:
             self.add_edge(*edge)
         return self
-    
+
     def adjacent(self, node1: Any, node2: Any):
         return (node1, node2) in self._edges
 
     def neighbours(self, node: Any):
         node_neighbours = List.create()
 
         for edge in self._edges:
@@ -434,14 +441,15 @@
 
     def has_edge(self, node1: Any, node2: Any):
         for edge in self._edges:
             if edge[0] == node1 and edge[1] == node2:
                 return True
         return False
 
+
 class WeightedGraph(Graph):
     def __init__(self, *, directed=False):
         self._nodes: list[Any] = []
         self._edges: list[tuple[Any, Any, int]] = []
 
         self._directed = directed
```

### Comparing `algorithmadts-0.1.2/src/AlgorithmADTs/GraphAlgorithms.py` & `algorithmadts-0.1.4/src/AlgorithmADTs/GraphAlgorithms.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from AlgorithmADTs.AbstractDataTypes import *
 
+
 def Prims(G: WeightedGraph):
-    """ Finds the Minimal Spanning Tree of a weighted undirected graph
+    """Finds the Minimal Spanning Tree of a weighted undirected graph
     OUTPUT
     tree: WeightedGraph(directed=True)
         Contains every node in the input graph and every (weighted) edge in the MST
     """
-    
+
     if G._directed:
         raise ValueError("Prims Algorithm must be run on an undirected graph")
     N = len(G._nodes)
 
     tree = WeightedGraph(directed=True)
     tree.add_node(G._nodes[0])
 
@@ -25,22 +26,23 @@
             key=lambda e: G.get_weight(e[0], e[1]),
         )
         tree.add_node(min_edge[1])
         tree.add_edge(*min_edge, G.get_weight(*min_edge))
 
     return tree
 
+
 def Dijkstras(G: WeightedGraph, source: Any):
     """Finds the shortests path between source node and all others in a weighted graph with no negative edge weights
 
     OUTPUT
     dist: Dictionary[key: node, value: numeric]
         The distance for each node, calculated from the source
     prev: Dictionary[key: node, value: node]
-        The previous node in the shortest path for each node, from the source node. 
+        The previous node in the shortest path for each node, from the source node.
         Used for path reconstruction
     """
 
     if not G.has_node(source):
         raise ValueError("Starting_node must be in G")
 
     dist = Dictionary()
@@ -63,23 +65,24 @@
                 continue
             alt = dist[closest_node] + G.get_weight(closest_node, neighbour)
             if alt < dist[neighbour]:
                 dist[neighbour] = alt
                 prev[neighbour] = closest_node
     return dist, prev
 
+
 def BellmanFord(G: WeightedGraph, source: Any):
     """Finds the shortest path between source node and all others in a weighted graph. Negative weights are allowed
     Inclues error checking for negative cycles
 
     OUTPUT
     dist: Dictionary[key: node, value: numeric]
         The distance for each node, calculated from the source
     prev: Dictionary[key: node, value: node]
-        The previous node in the shortest path for each node, from the source node. 
+        The previous node in the shortest path for each node, from the source node.
         Used for path reconstruction
     """
     if not G.has_node(source):
         raise ValueError("Starting_node must be in G")
 
     dist = Dictionary()
     prev = Dictionary()
@@ -99,14 +102,15 @@
     # Check for negative cycles
     for u, v, weight in G._edges:
         if dist[u] + weight < dist[v]:
             raise ValueError("Graph contains a negative cycle")
 
     return dist, prev
 
+
 def FloydWarshall(G: WeightedGraph):
     """Finds the shortest path between all nodes in a weighted graph. Negative weights are allowed.
     No negative cycle checking
 
     OUTPUT
     dist: Matrix[numeric] (G.V x G.V)
         The distance between each pair of nodes, indexed according to G.nodes
@@ -118,108 +122,116 @@
     """
     dist = Matrix(G.V, G.V)
     prev = Matrix(G.V, G.V)
 
     for i, node1 in enumerate(G._nodes):
         for j, node2 in enumerate(G._nodes):
             if i == j:
-                dist[i][j] = 0 
-                prev[i][j] = i 
+                dist[i][j] = 0
+                prev[i][j] = i
 
             elif G.has_edge(node1, node2):
                 dist[i][j] = G.get_weight(node1, node2)
                 prev[i][j] = i
-            
+
             else:
                 dist[i][j] = infinity
                 prev[i][j] = None
 
     for k in range(G.V):
         for i in range(G.V):
             for j in range(G.V):
                 if dist[i][j] > dist[i][k] + dist[k][j]:
                     dist[i][j] = dist[i][k] + dist[k][j]
                     prev[i][j] = prev[k][j]
-            
+
     return dist, prev
 
-def FloydWarshalTC(G: Graph):
+
+def FloydWarshallTC(G: Graph):
     """Calculates transitive closure between all nodes in an unweighted graph.
 
-        OUTPUT
-        dist: Matrix[bool] (G.V x G.V)
-            Transitive closure between every pair of nodes, indexed according to G.nodes
-            dist[i, j] is the boolen of whether j can be reached from i
-        prev: Matrix[node] (G.V x G.V)
-            The previous node in the shortest path between each node
-            Used for path reconstruction
-            prev[i, j] is the node immediately before j
-        """
+    OUTPUT
+    dist: Matrix[bool] (G.V x G.V)
+        Transitive closure between every pair of nodes, indexed according to G.nodes
+        dist[i, j] is the boolen of whether j can be reached from i
+    prev: Matrix[node] (G.V x G.V)
+        The previous node in the shortest path between each node
+        Used for path reconstruction
+        prev[i, j] is the node immediately before j
+    """
 
     dist = Matrix(G.V, G.V)
     prev = Matrix(G.V, G.V)
-  
+
     for i, node1 in enumerate(G._nodes):
         for j, node2 in enumerate(G._nodes):
             if i == j:
                 dist[i][j] = True
-                prev[i][j] = i 
+                prev[i][j] = i
 
             elif G.has_edge(node1, node2):
                 dist[i][j] = True
                 prev[i][j] = i
-            
+
             else:
                 dist[i][j] = False
                 prev[i][j] = None
 
     for k in range(G.V):
         for i in range(G.V):
             for j in range(G.V):
                 if (not dist[i][j]) and (dist[i][k] and dist[k][j]):
                     dist[i][j] = True
                     prev[i][j] = prev[k][j]
-            
+
     return dist, prev
 
-def PageRank(_G: Graph, d=0.85, num_iterations = 1_000):
+
+def PageRank(_G: Graph, d=0.85, num_iterations=1_000):
     """Calculates the PageRank value in an unweighted graph.
-        INPUT
-        d: float
-            The damping factor, the probability that a surfer will continue choosing links
-        num_iterations: int
-            The number of times the values are updated
-
-        OUTPUT
-        Pr: Dictionary[key: node, value: float]
-            The PageRank value for every node
+    INPUT
+    d: float
+        The damping factor, the probability that a surfer will continue choosing links
+    num_iterations: int
+        The number of times the values are updated
+
+    OUTPUT
+    Pr: Dictionary[key: node, value: float]
+        The PageRank value for every node
     """
     Pr = Dictionary()
 
-    G = Graph(directed=_G._directed) #Create a filtered copy of the graph to run the algorithm on
+    G = Graph(
+        directed=_G._directed
+    )  # Create a filtered copy of the graph to run the algorithm on
     for node in _G._nodes:
         G.add_node(node)
 
     for edge in _G._edges:
-        if not edge[0] == edge[1]:#links from a page to itself are ignored
+        if not edge[0] == edge[1]:  # links from a page to itself are ignored
             G.add_edge(*edge)
 
-    #Initialise values and check for sink nodes
+    # Initialise values and check for sink nodes
     for node in G._nodes:
-        if len(G.neighbours(node)) == 0: #redistribute sink nodes
+        if len(G.neighbours(node)) == 0:  # redistribute sink nodes
             for other_node in G._nodes:
                 if other_node != node:
                     G.add_edge(node, other_node)
 
-        Pr.add(node, 1/G.V) 
-    
-    #Calculate PageRank values
-    for _ in range(num_iterations): #Run for a set number of iterations
+        Pr.add(node, 1 / G.V)
+
+    # Calculate PageRank values
+    for _ in range(num_iterations):  # Run for a set number of iterations
         temp = Array(G.V)
         for i, node in enumerate(G._nodes):
-            incoming_links = (node2 for node2 in G._nodes if node in G.neighbours(node2))
-            temp[i] = (1-d)/G.V + d*sum(Pr[node2]/len(G.neighbours(node2)) for node2 in incoming_links)
+            incoming_links = (
+                node2 for node2 in G._nodes if node in G.neighbours(node2)
+            )
+            temp[i] = (1 - d) / G.V + d * sum(
+                Pr[node2] / len(G.neighbours(node2)) for node2 in incoming_links
+            )
 
         for i, node in enumerate(G._nodes):
             Pr[node] = temp[i]
 
     return Pr
```

### Comparing `algorithmadts-0.1.2/tests/experimenting.ipynb` & `algorithmadts-0.1.4/tests/experimenting.ipynb`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.2/tests/test_GraphAlgorithms.py` & `algorithmadts-0.1.4/tests/test_GraphAlgorithms.py`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.2/LICENSE` & `algorithmadts-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `algorithmadts-0.1.2/README.md` & `algorithmadts-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -64,24 +64,25 @@
 Graph
     create: None -> Graph
     add_node: Graph x Element -> Graph
     add_edge: Graph x Element x Element -> Graph
     adjacent: Graph x Element x Element -> Boolean
     neighbours: Graph x Element -> List
 ```
+Multiple nodes and edges can now be added at one time with `add_nodes` and `add_edges`, using an iterable
 ```
 WeightedGraph (inherits from Graph)
     create: None -> Graph
     add_node: Graph x Element -> Graph
     add_edge: Graph x Element x Element -> Graph
     adjacent: Graph x Element x Element -> Boolean
     neighbours: Graph x Element -> List
     get_weight: Graph x Element x Element -> integer
 ```
-Multiple nodes and edges can now be added at one time with `add_nodes` and `add_edges`, using an iterable
+
 
 Note that there is no restriction in these classes that elements be hashable, unlike some Python data types
 e.g. a Python `dict` requires keys to be hashable.
 
 It also defines a variable `infinity`, set equal to `float('inf')`
 
 The following magic methods are supported:
@@ -90,15 +91,15 @@
 - `__iter__` for Array and List, which operates as expected. Dictionary iter returns an iterable of keys.
     This enables iterating through a class like `for elem in instance`
 - `__str__` and `__repr__` are defined for all classes except graphs and allow for classes to be easily viewed through printing
     Note that only the head element is visible for a stack or queue, so it is the only information that can be returned by these methods
 - Numerical magic methods (e.g. `__add__`) are defined for matrices
 
 ## Graph Algorithms
-Currently, only the following graph algorithms are defined:
+Currently, the following graph algorithms are defined:
 - Prim's algorithm for computing the Minimal Spanning Tree of a weighted, undirected graph
 - Dijkstra's algorithm for finding the single source shortest path in a weighted graph 
 - The Bellman-Ford algorithm which extends the functionality of Dijkstra's algorithm to allow for negative weights
 - The two variants of the Floyd-Warshall algorithm to calculate shortest path between all nodes and transitive closure of an unweighted graph
 - The PageRank algorithm for determining the relative importance of nodes in an unweighted graph
 
 ## Version things
```

### Comparing `algorithmadts-0.1.2/PKG-INFO` & `algorithmadts-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlgorithmADTs
-Version: 0.1.2
+Version: 0.1.4
 Summary: General purpose Abstract Data Types for Algorithmics
 Author-email: Finlay <finlay3.141@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -76,24 +76,25 @@
 Graph
     create: None -> Graph
     add_node: Graph x Element -> Graph
     add_edge: Graph x Element x Element -> Graph
     adjacent: Graph x Element x Element -> Boolean
     neighbours: Graph x Element -> List
 ```
+Multiple nodes and edges can now be added at one time with `add_nodes` and `add_edges`, using an iterable
 ```
 WeightedGraph (inherits from Graph)
     create: None -> Graph
     add_node: Graph x Element -> Graph
     add_edge: Graph x Element x Element -> Graph
     adjacent: Graph x Element x Element -> Boolean
     neighbours: Graph x Element -> List
     get_weight: Graph x Element x Element -> integer
 ```
-Multiple nodes and edges can now be added at one time with `add_nodes` and `add_edges`, using an iterable
+
 
 Note that there is no restriction in these classes that elements be hashable, unlike some Python data types
 e.g. a Python `dict` requires keys to be hashable.
 
 It also defines a variable `infinity`, set equal to `float('inf')`
 
 The following magic methods are supported:
@@ -102,15 +103,15 @@
 - `__iter__` for Array and List, which operates as expected. Dictionary iter returns an iterable of keys.
     This enables iterating through a class like `for elem in instance`
 - `__str__` and `__repr__` are defined for all classes except graphs and allow for classes to be easily viewed through printing
     Note that only the head element is visible for a stack or queue, so it is the only information that can be returned by these methods
 - Numerical magic methods (e.g. `__add__`) are defined for matrices
 
 ## Graph Algorithms
-Currently, only the following graph algorithms are defined:
+Currently, the following graph algorithms are defined:
 - Prim's algorithm for computing the Minimal Spanning Tree of a weighted, undirected graph
 - Dijkstra's algorithm for finding the single source shortest path in a weighted graph 
 - The Bellman-Ford algorithm which extends the functionality of Dijkstra's algorithm to allow for negative weights
 - The two variants of the Floyd-Warshall algorithm to calculate shortest path between all nodes and transitive closure of an unweighted graph
 - The PageRank algorithm for determining the relative importance of nodes in an unweighted graph
 
 ## Version things
```

