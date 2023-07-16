# Comparing `tmp/mass_composition-0.1.8.tar.gz` & `tmp/mass_composition-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mass_composition-0.1.8.tar", max compression
+gzip compressed data, was "mass_composition-0.1.9.tar", max compression
```

## Comparing `mass_composition-0.1.8.tar` & `mass_composition-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,38 @@
--rw-r--r--   0        0        0       95 2023-03-30 23:02:48.765876 mass_composition-0.1.8/elphick/mass_composition/__init__.py
--rw-r--r--   0        0        0      378 2023-03-18 15:53:38.790312 mass_composition-0.1.8/elphick/mass_composition/config/mc_config.yml
--rw-r--r--   0        0        0    25114 2023-04-01 23:32:23.949257 mass_composition-0.1.8/elphick/mass_composition/mass_composition.py
--rw-r--r--   0        0        0    18226 2023-04-02 10:19:10.328941 mass_composition-0.1.8/elphick/mass_composition/mc_network.py
--rw-r--r--   0        0        0     3700 2023-04-01 12:05:20.820930 mass_composition-0.1.8/elphick/mass_composition/mc_node.py
--rw-r--r--   0        0        0    20074 2023-04-02 06:57:02.150313 mass_composition-0.1.8/elphick/mass_composition/mc_xarray.py
--rw-r--r--   0        0        0       43 2023-03-18 15:53:38.804742 mass_composition-0.1.8/elphick/mass_composition/utils/__init__.py
--rw-r--r--   0        0        0      214 2023-03-20 23:29:27.479355 mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3909 2023-03-20 23:29:27.526177 mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
--rw-r--r--   0        0        0     2197 2023-03-20 23:29:27.503110 mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
--rw-r--r--   0        0        0     1288 2023-04-02 09:40:10.491078 mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/partition.cpython-39.pyc
--rw-r--r--   0        0        0     1070 2023-04-02 04:19:49.351411 mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/size.cpython-39.pyc
--rw-r--r--   0        0        0     3122 2023-03-13 09:45:28.140963 mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/size_distribution.cpython-39.pyc
--rw-r--r--   0        0        0     1494 2023-03-20 23:29:27.885869 mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
--rw-r--r--   0        0        0     3036 2023-03-18 15:53:38.827788 mass_composition-0.1.8/elphick/mass_composition/utils/components.py
--rw-r--r--   0        0        0     2657 2023-03-18 15:53:38.832062 mass_composition-0.1.8/elphick/mass_composition/utils/moisture.py
--rw-r--r--   0        0        0     1078 2023-04-02 09:57:11.588006 mass_composition-0.1.8/elphick/mass_composition/utils/partition.py
--rw-r--r--   0        0        0      927 2023-04-02 04:14:35.940818 mass_composition-0.1.8/elphick/mass_composition/utils/size.py
--rw-r--r--   0        0        0     2730 2023-03-18 16:00:57.598605 mass_composition-0.1.8/elphick/mass_composition/utils/size_distribution.py
--rw-r--r--   0        0        0     1772 2023-03-18 15:53:38.841624 mass_composition-0.1.8/elphick/mass_composition/utils/viz.py
--rw-r--r--   0        0        0     1090 2023-03-18 16:00:57.535113 mass_composition-0.1.8/LICENSE
--rw-r--r--   0        0        0     1582 2023-04-02 10:19:54.350273 mass_composition-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1168 1970-01-01 00:00:00.000000 mass_composition-0.1.8/setup.py
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 mass_composition-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      133 2023-06-10 11:56:22.191053 mass_composition-0.1.9/elphick/mass_composition/__init__.py
+-rw-r--r--   0        0        0       36 2023-05-27 12:53:15.011676 mass_composition-0.1.9/elphick/mass_composition/config/__init__.py
+-rw-r--r--   0        0        0      208 2023-05-27 16:46:53.793999 mass_composition-0.1.9/elphick/mass_composition/config/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      618 2023-05-27 16:46:53.803978 mass_composition-0.1.9/elphick/mass_composition/config/__pycache__/config_read.cpython-39.pyc
+-rw-r--r--   0        0        0      410 2023-05-27 12:53:15.013670 mass_composition-0.1.9/elphick/mass_composition/config/config_read.py
+-rw-r--r--   0        0        0      757 2023-06-10 13:33:51.459046 mass_composition-0.1.9/elphick/mass_composition/config/mc_config.yml
+-rw-r--r--   0        0        0     3216 2023-05-21 11:48:53.697478 mass_composition-0.1.9/elphick/mass_composition/layout.py
+-rw-r--r--   0        0        0    36468 2023-06-11 08:27:02.589290 mass_composition-0.1.9/elphick/mass_composition/mass_composition.py
+-rw-r--r--   0        0        0    25883 2023-05-27 12:53:15.023643 mass_composition-0.1.9/elphick/mass_composition/mc_network.py
+-rw-r--r--   0        0        0     3814 2023-05-21 11:48:53.712222 mass_composition-0.1.9/elphick/mass_composition/mc_node.py
+-rw-r--r--   0        0        0      660 2023-05-27 12:53:15.024640 mass_composition-0.1.9/elphick/mass_composition/mc_status.py
+-rw-r--r--   0        0        0    19556 2023-05-21 11:48:54.150524 mass_composition-0.1.9/elphick/mass_composition/mc_xarray.py
+-rw-r--r--   0        0        0     2606 2023-05-27 12:53:15.026637 mass_composition-0.1.9/elphick/mass_composition/plot.py
+-rw-r--r--   0        0        0       43 2023-04-10 12:39:40.787145 mass_composition-0.1.9/elphick/mass_composition/utils/__init__.py
+-rw-r--r--   0        0        0      214 2023-05-27 16:46:53.824440 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3909 2023-05-27 16:46:53.869321 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc
+-rw-r--r--   0        0        0      326 2023-05-21 12:44:21.475008 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/geometry.cpython-39.pyc
+-rw-r--r--   0        0        0     3220 2023-05-21 12:44:20.456232 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/interp.cpython-39.pyc
+-rw-r--r--   0        0        0     2197 2023-05-27 16:46:53.837403 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc
+-rw-r--r--   0        0        0     1026 2023-05-21 12:44:21.482102 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/partition.cpython-39.pyc
+-rw-r--r--   0        0        0      430 2023-04-10 22:39:47.328179 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/random.cpython-39.pyc
+-rw-r--r--   0        0        0      440 2023-05-21 12:44:20.432193 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/sampling.cpython-39.pyc
+-rw-r--r--   0        0        0     1068 2023-05-27 16:46:53.846382 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/size.cpython-39.pyc
+-rw-r--r--   0        0        0     2898 2023-05-20 23:36:00.926218 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/size_distribution.cpython-39.pyc
+-rw-r--r--   0        0        0     1494 2023-05-27 16:46:53.857353 mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc
+-rw-r--r--   0        0        0     3036 2023-03-18 15:53:38.827788 mass_composition-0.1.9/elphick/mass_composition/utils/components.py
+-rw-r--r--   0        0        0       85 2023-05-21 11:48:53.725041 mass_composition-0.1.9/elphick/mass_composition/utils/geometry.py
+-rw-r--r--   0        0        0     3968 2023-05-21 11:48:53.727057 mass_composition-0.1.9/elphick/mass_composition/utils/interp.py
+-rw-r--r--   0        0        0     2657 2023-03-18 15:53:38.832062 mass_composition-0.1.9/elphick/mass_composition/utils/moisture.py
+-rw-r--r--   0        0        0     1078 2023-05-21 11:48:53.728597 mass_composition-0.1.9/elphick/mass_composition/utils/partition.py
+-rw-r--r--   0        0        0      321 2023-05-21 11:48:53.732855 mass_composition-0.1.9/elphick/mass_composition/utils/sampling.py
+-rw-r--r--   0        0        0      925 2023-05-27 12:53:15.029628 mass_composition-0.1.9/elphick/mass_composition/utils/size.py
+-rw-r--r--   0        0        0     2730 2023-03-18 16:00:57.598605 mass_composition-0.1.9/elphick/mass_composition/utils/size_distribution.py
+-rw-r--r--   0        0        0     1772 2023-03-18 15:53:38.841624 mass_composition-0.1.9/elphick/mass_composition/utils/viz.py
+-rw-r--r--   0        0        0     7912 2023-06-11 06:21:17.354868 mass_composition-0.1.9/elphick/mass_composition/variables.py
+-rw-r--r--   0        0        0     1090 2023-03-18 16:00:57.535113 mass_composition-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1648 2023-06-11 09:00:51.784644 mass_composition-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 mass_composition-0.1.9/PKG-INFO
```

### Comparing `mass_composition-0.1.8/elphick/mass_composition/mc_network.py` & `mass_composition-0.1.9/elphick/mass_composition/mc_network.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+from copy import deepcopy
 from typing import Dict, List, Optional, Tuple, Union
 
 import matplotlib
 import networkx as nx
+import numpy as np
 import pandas as pd
 import plotly.graph_objects as go
 from matplotlib import pyplot as plt
 from matplotlib.colors import ListedColormap, LinearSegmentedColormap
 import matplotlib.cm as cm
 import seaborn as sns
 
 from plotly.subplots import make_subplots
 
 from elphick.mass_composition import MassComposition
+from elphick.mass_composition.layout import digraph_linear_layout, linear_layout
 from elphick.mass_composition.mc_node import MCNode, NodeType
+from elphick.mass_composition.plot import parallel_plot
+from elphick.mass_composition.utils.geometry import midpoint
+from elphick.mass_composition.utils.size import mean_size
+from elphick.mass_composition.utils.viz import plot_parallel
 
 
 class MCNetwork(nx.DiGraph):
     def __init__(self, **attr):
         super().__init__(**attr)
 
     @classmethod
@@ -28,126 +35,202 @@
             name: name of the network
 
         Returns:
 
         """
         bunch_of_edges: List = []
         for stream in streams:
-            if stream.data.nodes is None:
+            if stream.nodes is None:
                 raise KeyError(f'Stream {stream.name} does not have the node property set')
-            nodes = stream.data.nodes
+            nodes = stream.nodes
 
             # add the objects to the edges
             bunch_of_edges.append((nodes[0], nodes[1], {'mc': stream}))
 
         graph = cls(name=name)
         graph.add_edges_from(bunch_of_edges)
         d_node_objects: Dict = {}
         for node in graph.nodes:
             d_node_objects[node] = MCNode(node_id=int(node))
-
         nx.set_node_attributes(graph, d_node_objects, 'mc')
 
         for node in graph.nodes:
             d_node_objects[node].inputs = [graph.get_edge_data(e[0], e[1])['mc'] for e in graph.in_edges(node)]
             d_node_objects[node].outputs = [graph.get_edge_data(e[0], e[1])['mc'] for e in graph.out_edges(node)]
 
-        # nx.set_node_attributes(graph, d_node_balance, 'data')
-        # bal_vals: List = [n['data'].balanced for n in graph.nodes if n is not None]
-        # graph['balanced'] = all(bal_vals)
+        graph = nx.convert_node_labels_to_integers(graph)
+        # update the temporary nodes on the mc object property to match the renumbered integers
+        for node1, node2, data in graph.edges(data=True):
+            data['mc'].nodes = [node1, node2]
+
         return graph
 
     @property
     def balanced(self) -> bool:
         bal_vals: List = [self.nodes[n]['mc'].balanced for n in self.nodes]
         bal_vals = [bv for bv in bal_vals if bv is not None]
         return all(bal_vals)
 
+    @property
+    def edge_status(self) -> Tuple:
+        d_edge_status_ok: Dict = {}
+        d_failing_edges: Dict = {}
+        for u, v, data in self.edges(data=True):
+            d_edge_status_ok[data['mc'].name] = data['mc'].status.ok
+            if not data['mc'].status.ok:
+                d_failing_edges[data['mc'].name] = data['mc'].status.failing_components
+        return all(d_edge_status_ok.values()), d_failing_edges
+
+    def get_edge_by_name(self, name: str) -> MassComposition:
+        """Get the MC object from the network by its name
+
+        Args:
+            name: The string name of the MassComposition object stored on an edge in the network.
+
+        Returns:
+
+        """
+
+        res: Optional[MassComposition] = None
+        for u, v, a in self.edges(data=True):
+            if a['mc'].name == name:
+                res = a['mc']
+
+        if not res:
+            raise ValueError(f"The specified name: {name} is not found on the network.")
+
+        return res
+
     def report(self) -> pd.DataFrame:
         """Summary Report
 
         Total Mass and weight averaged composition
         Returns:
 
         """
         chunks: List[pd.DataFrame] = []
         for n, nbrs in self.adj.items():
             for nbr, eattr in nbrs.items():
                 chunks.append(eattr['mc'].aggregate().assign(name=eattr['mc'].name))
         rpt: pd.DataFrame = pd.concat(chunks, axis='index').set_index('name')
         return rpt
 
+    def query(self, mc_name: str, queries: Dict) -> 'MCNetwork':
+        """Query/filter across the network
+
+        The queries provided will be applied to the MassComposition object in the network with the mc_name.
+        The indexes for that result are then used to filter the other edges of the network.
+
+        Args:
+            mc_name: The name of the MassComposition object in the network to which the first filter to be applied.
+            queries: The query or queries to apply to the object with mc_name.
+
+        Returns:
+
+        """
+
+        mc_obj_ref: MassComposition = self.get_edge_by_name(mc_name).query(queries=queries)
+        # TODO: This construct limits us to filtering along a single dimension only
+        coord: str = list(queries.keys())[0]
+        index = mc_obj_ref.data[coord]
+
+        # iterate through all other objects on the edges and filter them to the same indexes
+        mc_objects: List[MassComposition] = []
+        for u, v, a in self.edges(data=True):
+            if a['mc'].name == mc_name:
+                mc_objects.append(mc_obj_ref)
+            else:
+                mc_obj: MassComposition = deepcopy(self.get_edge_by_name(a['mc'].name))
+                mc_obj._data = mc_obj._data.sel({coord: index.values})
+                mc_objects.append(mc_obj)
+
+        res: MCNetwork = MCNetwork.from_streams(mc_objects)
+
+        return res
+
     def get_node_input_outputs(self, node) -> Tuple:
         in_edges = self.in_edges(node)
         in_mc = [self.get_edge_data(oe[0], oe[1])['mc'] for oe in in_edges]
         out_edges = self.out_edges(node)
         out_mc = [self.get_edge_data(oe[0], oe[1])['mc'] for oe in out_edges]
         return in_mc, out_mc
 
-    def plot(self) -> plt.Figure:
+    def plot(self, orientation: str = 'horizontal') -> plt.Figure:
         """Plot the network with matplotlib
 
+        Args:
+            orientation: 'horizontal'|'vertical' network layout
+
         Returns:
 
         """
 
         hf, ax = plt.subplots()
-        # TODO: add multi-partite layout to provide left to right layout
-        pos = nx.spring_layout(self, seed=1234)
+        # pos = nx.spring_layout(self, seed=1234)
+        pos = digraph_linear_layout(self, orientation=orientation)
 
         edge_labels: Dict = {}
         edge_colors: List = []
         node_colors: List = []
 
         for node1, node2, data in self.edges(data=True):
             edge_labels[(node1, node2)] = data['mc'].name
-            # TODO: add colors by edge balance status, once defined
-            edge_colors.append('gray')
+            if data['mc'].status.ok:
+                edge_colors.append('gray')
+            else:
+                edge_colors.append('red')
 
         for n in self.nodes:
             if self.nodes[n]['mc'].node_type == NodeType.BALANCE:
                 if self.nodes[n]['mc'].balanced:
                     node_colors.append('green')
                 else:
                     node_colors.append('red')
             else:
                 node_colors.append('gray')
 
         nx.draw(self, pos=pos, ax=ax, with_labels=True, font_weight='bold',
                 node_color=node_colors, edge_color=edge_colors)
 
         nx.draw_networkx_edge_labels(self, pos=pos, ax=ax, edge_labels=edge_labels, font_color='black')
+        ax.set_title(self._plot_title(html=False), fontsize=10)
 
-        ax.set_title(f"{self.name}\nBalanced: {self.balanced}")
         return hf
 
-    def plot_network(self) -> go.Figure:
+    def plot_network(self, orientation: str = 'horizontal') -> go.Figure:
         """Plot the network with plotly
 
+        Args:
+            orientation: 'horizontal'|'vertical' network layout
+
         Returns:
 
         """
-        pos = nx.spring_layout(self, seed=1234)
+        # pos = nx.spring_layout(self, seed=1234)
+        pos = digraph_linear_layout(self, orientation=orientation)
 
-        edge_trace, node_trace = self._get_scatter_node_edges(pos)
-        title = f"{self.name}<br>Balanced: {self.balanced}"
+        edge_traces, node_trace, edge_annotation_trace = self._get_scatter_node_edges(pos)
+        title = self._plot_title()
 
-        fig = go.Figure(data=[edge_trace, node_trace],
+        fig = go.Figure(data=[*edge_traces, node_trace, edge_annotation_trace],
                         layout=go.Layout(
                             title=title,
                             titlefont_size=16,
                             showlegend=False,
                             hovermode='closest',
                             margin=dict(b=20, l=5, r=5, t=40),
                             xaxis=dict(showgrid=False, zeroline=False, showticklabels=False),
                             yaxis=dict(showgrid=False, zeroline=False, showticklabels=False),
                             paper_bgcolor='rgba(0,0,0,0)',
                             plot_bgcolor='rgba(0,0,0,0)'
                         ),
                         )
+        # for k, d_args in edge_annotations.items():
+        #     fig.add_annotation(x=d_args['pos'][0], y=d_args['pos'][1], text=k, textangle=d_args['angle'])
+
         return fig
 
     def plot_sankey(self,
                     width_var: str = 'mass_wet',
                     color_var: Optional[str] = None,
                     edge_colormap: Optional[str] = 'copper_r',
                     vmin: Optional[float] = None,
@@ -164,45 +247,49 @@
 
         Returns:
 
         """
         d_sankey: Dict = self._generate_sankey_args(color_var, edge_colormap, width_var, vmin, vmax)
         node, link = self._get_sankey_node_link_dicts(d_sankey)
         fig = go.Figure(data=[go.Sankey(node=node, link=link)])
-        title = f"{self.name}<br>Balanced: {self.balanced}"
+        title = self._plot_title()
         fig.update_layout(title_text=title, font_size=10)
         return fig
 
     def table_plot(self,
                    plot_type: str = 'sankey',
+                   cols_exclude: Optional[List] = None,
                    table_pos: str = 'left',
                    table_area: float = 0.4,
                    table_header_color: str = 'cornflowerblue',
                    table_odd_color: str = 'whitesmoke',
                    table_even_color: str = 'lightgray',
                    sankey_width_var: str = 'mass_wet',
                    sankey_color_var: Optional[str] = None,
                    sankey_edge_colormap: Optional[str] = 'copper_r',
                    sankey_vmin: Optional[float] = None,
-                   sankey_vmax: Optional[float] = None
+                   sankey_vmax: Optional[float] = None,
+                   network_orientation: Optional[str] = 'horizontal'
                    ) -> go.Figure:
         """Plot with table of edge averages
 
         Args:
             plot_type: The type of plot ['sankey', 'network']
+            cols_exclude: List of columns to exclude from the table
             table_pos: Position of the table ['left', 'right', 'top', 'bottom']
             table_area: The proportion of width or height to allocate to the table [0, 1]
             table_header_color: Color of the table header
             table_odd_color: Color of the odd table rows
             table_even_color: Color of the even table rows
             sankey_width_var: If plot_type is sankey, the variable that determines the sankey width
             sankey_color_var: If plot_type is sankey, the optional variable that determines the sankey edge color
             sankey_edge_colormap: If plot_type is sankey, the optional colormap.  Used with sankey_color_var.
             sankey_vmin: The value that maps to the minimum color
             sankey_vmax: The value that maps to the maximum color
+            network_orientation: The orientation of the network layout 'vertical'|'horizontal'
 
         Returns:
 
         """
 
         valid_plot_types: List[str] = ['sankey', 'network']
         if plot_type not in valid_plot_types:
@@ -212,15 +299,17 @@
         if table_pos not in valid_table_pos:
             raise ValueError(f'The supplied table_pos is not in {valid_table_pos}')
 
         d_subplot, d_table, d_plot = self._get_position_kwargs(table_pos, table_area, plot_type)
 
         fig = make_subplots(**d_subplot, print_grid=False)
 
-        df = self.report().reset_index()
+        df: pd.DataFrame = self.report().reset_index()
+        if cols_exclude:
+            df = df[[col for col in df.columns if col not in cols_exclude]]
         fmt: List[str] = ["%s"] + [".1f", ".1f"] + [".2f"] * (len(df.columns) - 3)
         column_widths = [2] + [1] * (len(df.columns) - 1)
 
         fig.add_table(
             header=dict(values=list(df.columns),
                         fill_color=table_header_color,
                         align='center',
@@ -238,31 +327,81 @@
                                                         sankey_width_var,
                                                         sankey_vmin,
                                                         sankey_vmax)
             node, link = self._get_sankey_node_link_dicts(d_sankey)
             fig.add_trace(go.Sankey(node=node, link=link), **d_plot)
 
         elif plot_type == 'network':
-            pos = nx.spring_layout(self, seed=1234)
+            # pos = nx.spring_layout(self, seed=1234)
+            pos = digraph_linear_layout(self, orientation=network_orientation)
 
-            edge_trace, node_trace = self._get_scatter_node_edges(pos)
-            fig.add_traces(data=[edge_trace, node_trace], **d_plot)
+            edge_traces, node_trace, edge_annotation_trace = self._get_scatter_node_edges(pos)
+            fig.add_traces(data=[*edge_traces, node_trace, edge_annotation_trace], **d_plot)
 
             fig.update_layout(showlegend=False, hovermode='closest',
                               xaxis=dict(showgrid=False, zeroline=False, showticklabels=False),
                               yaxis=dict(showgrid=False, zeroline=False, showticklabels=False),
                               paper_bgcolor='rgba(0,0,0,0)',
                               plot_bgcolor='rgba(0,0,0,0)'
                               )
 
-        title = f"{self.name}<br>Balanced: {self.balanced}"
+        title = self._plot_title(compact=True)
         fig.update_layout(title_text=title, font_size=12)
 
         return fig
 
+    def to_dataframe(self,
+                     names: Optional[str] = None):
+        """Return a tidy dataframe
+
+        Args:
+            names: Optional List of names of MassComposition objects (network edges) for export
+
+        Returns:
+
+        """
+        chunks: List[pd.DataFrame] = []
+        for u, v, data in self.edges(data=True):
+            if (names is None) or ((names is not None) and (data['mc'].name in names)):
+                chunks.append(data['mc'].data.mc.to_dataframe().assign(name=data['mc'].name))
+        return pd.concat(chunks, axis='index')
+
+    def plot_parallel(self,
+                      names: Optional[str] = None,
+                      color: Optional[str] = None,
+                      vars_include: Optional[List[str]] = None,
+                      vars_exclude: Optional[List[str]] = None,
+                      title: Optional[str] = None,
+                      include_dims: Optional[Union[bool, List[str]]] = True,
+                      plot_interval_edges: bool = False) -> go.Figure:
+        """Create an interactive parallel plot
+
+        Useful to explore multidimensional data like mass-composition data
+
+        Args:
+            names: Optional List of Names to plot
+            color: Optional color variable
+            vars_include: Optional List of variables to include in the plot
+            vars_exclude: Optional List of variables to exclude in the plot
+            title: Optional plot title
+            include_dims: Optional boolean or list of dimension to include in the plot.  True will show all dims.
+            plot_interval_edges: If True, interval edges will be plotted instead of interval mid
+
+        Returns:
+
+        """
+        df: pd.DataFrame = self.to_dataframe(names=names)
+
+        if not title and hasattr(self, 'name'):
+            title = self.name
+
+        fig = parallel_plot(data=df, color=color, vars_include=vars_include, vars_exclude=vars_exclude, title=title,
+                            include_dims=include_dims, plot_interval_edges=plot_interval_edges)
+        return fig
+
     @staticmethod
     def _get_position_kwargs(table_pos, table_area, plot_type):
         """Helper to manage location dependencies
 
         Args:
             table_pos: position of the table: left|right|top|bottom
             table_width: fraction of the plot to assign to the table [0, 1]
@@ -308,17 +447,17 @@
 
     def _generate_sankey_args(self, color_var, edge_colormap, width_var, v_min, v_max):
         rpt: pd.DataFrame = self.report()
         if color_var is not None:
             cmap = sns.color_palette(edge_colormap, as_cmap=True)
             rpt: pd.DataFrame = self.report()
             if not v_min:
-                v_min = float(rpt[color_var].min())
+                v_min = np.floor(rpt[color_var].min())
             if not v_max:
-                v_max = float(rpt[color_var].max())
+                v_max = np.ceil(rpt[color_var].max())
         if isinstance(list(self.nodes)[0], int):
             labels = [str(n) for n in list(self.nodes)]
         else:
             labels = list(self.nodes)
         # run the report for the hover data
         d_custom_data: Dict = self._rpt_to_html(df=rpt)
         source: List = []
@@ -382,45 +521,67 @@
             customdata=d_sankey['edge_custom_data'],
             hovertemplate='<b><i>%{label}</i></b><br />Source: %{source.customdata}<br />'
                           'Target: %{target.customdata}<br />%{customdata}'
         )
         return node, link
 
     def _get_scatter_node_edges(self, pos):
-        edge_x = []
-        edge_y = []
-        for edge in self.edges():
-            x0, y0 = pos[edge[0]]
-            x1, y1 = pos[edge[1]]
-            edge_x.append(x0)
-            edge_x.append(x1)
-            edge_x.append(None)
-            edge_y.append(y0)
-            edge_y.append(y1)
-            edge_y.append(None)
-        edge_trace = go.Scatter(
-            x=edge_x, y=edge_y,
-            line=dict(width=2, color='#888'),
-            hoverinfo='none',
-            mode='lines')
+        # edges
+        edge_color_map: Dict = {True: 'grey', False: 'red'}
+        edge_annotations: Dict = {}
+
+        edge_traces = []
+        for u, v, data in self.edges(data=True):
+            x0, y0 = pos[u]
+            x1, y1 = pos[v]
+            edge_annotations[data['mc'].name] = {'pos': midpoint(pos[u], pos[v])}
+            edge_traces.append(go.Scatter(x=[x0, x1], y=[y0, y1],
+                                          line=dict(width=2, color=edge_color_map[data['mc'].status.ok]),
+                                          hoverinfo='text',
+                                          mode='lines',
+                                          text=data['mc'].name))
+
+        # nodes
+        node_color_map: Dict = {None: 'grey', True: 'green', False: 'red'}
         node_x = []
         node_y = []
+        node_color = []
+        node_text = []
         for node in self.nodes():
             x, y = pos[node]
             node_x.append(x)
             node_y.append(y)
+            node_color.append(node_color_map[self.nodes[node]['mc'].balanced])
+            node_text.append(node)
         node_trace = go.Scatter(
             x=node_x, y=node_y,
+            mode='markers+text',
+            hoverinfo='none',
+            marker=dict(
+                color=node_color,
+                size=30,
+                line_width=2),
+            text=node_text)
+
+        # edge annotations
+        edge_labels = list(edge_annotations.keys())
+        edge_label_x = [edge_annotations[k]['pos'][0] for k, v in edge_annotations.items()]
+        edge_label_y = [edge_annotations[k]['pos'][1] for k, v in edge_annotations.items()]
+
+        edge_annotation_trace = go.Scatter(
+            x=edge_label_x, y=edge_label_y,
             mode='markers',
             hoverinfo='text',
             marker=dict(
-                color=[],
-                size=20,
-                line_width=2))
-        return edge_trace, node_trace
+                color='grey',
+                size=3,
+                line_width=1),
+            text=edge_labels)
+
+        return edge_traces, node_trace, edge_annotation_trace
 
     @staticmethod
     def _rpt_to_html(df: pd.DataFrame) -> Dict:
         custom_data: Dict = {}
         for i, row in df.iterrows():
             str_data: str = '<br />'
             for k, v in dict(row).items():
@@ -440,7 +601,17 @@
             m = cm.ScalarMappable(norm=norm, cmap=cmap)
             r, g, b, a = m.to_rgba(val, bytes=True)
             color_rgba = int(r), int(g), int(b), int(a)
         else:
             NotImplementedError("Unrecognised colormap type")
 
         return color_rgba
+
+    def _plot_title(self, html: bool = True, compact: bool = False):
+        title = f"{self.name}<br><br><sup>Balanced: {self.balanced}<br>Edge Status OK: {self.edge_status[0]}</sup>"
+        if compact:
+            title = title.replace("<br><br>", "<br>").replace("<br>Edge", ", Edge")
+        if not self.edge_status[0]:
+            title = title.replace("</sup>", "") + f", {self.edge_status[1]}</sup>"
+        if not html:
+            title = title.replace('<br><br>', '\n').replace('<br>', '\n').replace('<sup>', '').replace('</sup>', '')
+        return title
```

### Comparing `mass_composition-0.1.8/elphick/mass_composition/mc_node.py` & `mass_composition-0.1.9/elphick/mass_composition/mc_node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from enum import Enum
-from typing import List, Optional, Dict, Tuple
+from typing import List, Optional, Dict
 
 import numpy as np
 import pandas as pd
-
+import xarray as xr
 from elphick.mass_composition import MassComposition
 # noinspection PyUnresolvedReferences
 import elphick.mass_composition.mc_xarray  # keep this "unused" import - it helps
 
 
 class NodeType(Enum):
     SOURCE = 'input'
@@ -16,18 +16,20 @@
     BALANCE = 'degree 2+'
 
 
 class MCNode:
     def __init__(self,
                  node_id: int = 0,
                  node_name: str = 'Node',
+                 node_subset: int = 0,
                  ):
 
         self.node_id: int = node_id
         self.node_name: str = node_name
+        self.node_subset: int = node_subset
         self._tolerance: float = np.finfo('float32').eps
 
         self._inputs: Optional[List[MassComposition]] = None
         self._outputs: Optional[List[MassComposition]] = None
         self._balanced: Optional[bool] = None
         self._balance_errors: Optional[pd.DataFrame] = None
 
@@ -101,19 +103,18 @@
         obj_list = []
         if direction == 'in':
             obj_list = self.inputs
         elif direction == 'out':
             obj_list = self.outputs
 
         if obj_list:
-            obj_sum: MassComposition = obj_list[0]
+            cols = obj_list[0].data.mc.mc_vars_mass + ['H2O'] + obj_list[0].data.mc.mc_vars_chem
+            res: pd.DataFrame = obj_list[0].data.mc.composition_to_mass().to_dataframe()[cols]
             for obj_mc in obj_list[1:]:
-                obj_sum = obj_sum + obj_mc
-            cols = obj_sum.data.mc.mc_vars_mass + ['H2O'] + obj_sum.data.mc.mc_vars_chem
-            res = obj_sum.data.mc.composition_to_mass().to_dataframe()[cols]
+                res = res + obj_mc.data.mc.composition_to_mass().to_dataframe()[cols]
         return res
 
     def node_balance(self) -> Optional[pd.DataFrame]:
         if self.node_type == NodeType.BALANCE:
             res = self.mass_sum('in') - self.mass_sum('out')
         else:
             res = None
```

### Comparing `mass_composition-0.1.8/elphick/mass_composition/mc_xarray.py` & `mass_composition-0.1.9/elphick/mass_composition/mc_xarray.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Dict, Optional, Union, Iterable, List, Tuple, Callable
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 
 from elphick.mass_composition.utils import solve_mass_moisture
+from elphick.mass_composition.utils.interp import interp_monotonic
 from elphick.mass_composition.utils.size import mean_size
 
 
 class CompositionContext(Enum):
     ABSOLUTE = 'mass'
     RELATIVE = "percent"
 
@@ -35,26 +36,14 @@
         self._chem: xr.Dataset = self._obj[self.mc_vars_chem]
         self._mass: xr.Dataset = self._obj[self.mc_vars_mass]
 
     @property
     def name(self):
         return self._obj.attrs['mc_name']
 
-    @property
-    def nodes(self):
-        return self._obj.attrs['nodes']
-
-    @nodes.setter
-    def nodes(self, values):
-        self._obj.attrs['nodes'] = values
-
-    @property
-    def history(self):
-        return self._obj.attrs['mc_history']
-
     def data(self):
 
         moisture: xr.DataArray = xr.DataArray((self._obj['mass_wet'] - self._obj['mass_dry']) /
                                               self._obj['mass_wet'] * 100, name='H2O',
                                               attrs={'units': '%',
                                                      'standard_name': 'H2O',
                                                      'mc_type': 'moisture',
@@ -79,19 +68,14 @@
                 raise KeyError("Chemistry units do not conform")
         else:
             raise KeyError("Chemistry units are inconsistent")
         return res
 
     def rename(self, new_name: str):
         self._obj.attrs['mc_name'] = new_name
-        self.log_to_history(f'Renamed to {new_name}')
-
-    def log_to_history(self, msg: str):
-        self._logger.info(msg)
-        self._obj.attrs['mc_history'].append(msg)
 
     def aggregate(self, group_var: Optional[str] = None,
                   group_bins: Optional[Union[int, Iterable]] = None,
                   as_dataframe: bool = False,
                   original_column_names: bool = False) -> Union[xr.Dataset, pd.DataFrame]:
         """Calculate the weight average of this dataset.
 
@@ -146,45 +130,57 @@
                 res.index = pd.Index([self.name], name='name')
 
         return res
 
     def cumulate(self, direction: str) -> xr.Dataset:
         """Cumulate along the dims
 
-        Expected use case in only for Datasets that have been reduced to 1D.
+        Expected use case is only for Datasets that have been reduced to 1D.
 
         Args:
             direction: 'ascending'|'descending'
 
         Returns:
 
         """
 
         valid_dirs: List[str] = ['ascending', 'descending']
         if direction not in valid_dirs:
             raise KeyError(f'Invalid direction provided.  Valid arguments are: {valid_dirs}')
 
+        d_dir: Dict = {'ascending': True, 'descending': False}
+
         if len(self._obj.dims) > 1:
             raise NotImplementedError('Datasets > 1D have not been tested.')
 
+        index_var: str = str(list(self._obj.dims.keys())[0])
+        if not isinstance(self._obj[index_var].data[0], pd.Interval):
+            self._logger.warning("Unexpected use of the cumulate method on non-fractional data.  "
+                                 "Consider setting the index (dim) as intervals.")
+
+        interval_index = pd.Index(self._obj[index_var])
+        if not (interval_index.is_monotonic_increasing or interval_index.is_monotonic_decreasing):
+            raise ValueError('Index is not monotonically increasing or decreasing')
+
+        in_data_ascending: bool = True
+        if interval_index.is_monotonic_decreasing:
+            in_data_ascending = False
+
         # convert to mass, then cumsum, then convert back to relative composition (grade)
         mass: xr.Dataset = self.composition_to_mass()
 
-        index_var = list(mass.indexes)[0]
-        if direction == 'descending':
-            mass = mass.sortby(variables=index_var, ascending=False)
+        mass = mass.sortby(variables=index_var, ascending=d_dir[direction])
 
         mass_cum: xr.Dataset = mass.cumsum(keep_attrs=True)
         # put the coords back
         mass_cum = mass_cum.assign_coords(**mass.coords)
         res: xr.Dataset = mass_cum.mc.mass_to_composition()
 
-        if direction == 'descending':
-            # put back to ascending order
-            res = res.sortby(variables=index_var, ascending=True)
+        # put back to original order
+        res = res.sortby(variables=index_var, ascending=in_data_ascending)
 
         return res
 
     def composition_to_mass(self) -> xr.Dataset:
         """Transform composition to mass
 
         :return:
@@ -193,22 +189,22 @@
         if self.composition_context == CompositionContext.ABSOLUTE:
             raise AssertionError('The dataset composition context is already absolute (mass units)')
 
         xr.set_options(keep_attrs=True)
 
         dsm: xr.Dataset = self._obj.copy()
 
-        dsm[self._obj.mc_vars_chem] = (dsm[self._obj.mc_vars_chem] * self._obj['mass_dry'] / 100)
+        dsm[self._obj.mc_vars_chem] = dsm[self._obj.mc_vars_chem] * self._obj['mass_dry'] / 100
+        if 'H2O' in dsm.variables:
+            dsm['H2O'] = self._obj['mass_wet'] - self._obj['mass_dry']
 
         for da in dsm.values():
             if da.attrs['mc_type'] == 'chemistry':
                 da.attrs['units'] = dsm['mass_wet'].attrs['units']
 
-        self.log_to_history(f'Converted to {self.composition_context}, dropped attr variables')
-
         xr.set_options(keep_attrs='default')
 
         return dsm
 
     def mass_to_composition(self) -> xr.Dataset:
         """Transform mass to composition.
 
@@ -217,22 +213,22 @@
 
         if self.composition_context == CompositionContext.RELATIVE:
             raise AssertionError('The dataset composition context is already relative (% units)')
 
         xr.set_options(keep_attrs=True)
 
         dsc: xr.Dataset = self._obj.copy()
-        dsc[self._obj.mc_vars_chem] = (dsc[self._obj.mc_vars_chem] / self._obj['mass_dry'] * 100)
+        dsc[self._obj.mc_vars_chem] = dsc[self._obj.mc_vars_chem] / self._obj['mass_dry'] * 100
+        if 'H2O' in dsc.variables:
+            dsc['H2O'] = (self._obj['mass_wet'] - self._obj['mass_dry']) / self._obj['mass_wet'] * 100
 
         for da in dsc.values():
             if da.attrs['mc_type'] == 'chemistry':
                 da.attrs['units'] = '%'
 
-        self.log_to_history(f'Converted to {self.composition_context}')
-
         xr.set_options(keep_attrs='default')
 
         return dsc
 
     def split(self, fraction: float) -> Tuple[xr.Dataset, xr.Dataset]:
         """Split the object by mass
 
@@ -254,25 +250,19 @@
             raise ValueError("The fraction provided must be between [0.0, 1.0] - mass cannot be created nor destroyed.")
 
         out = deepcopy(self)
         comp = deepcopy(self)
 
         # split by mass
         out._obj[self._obj.mc_vars_mass] = out._obj[self._obj.mc_vars_mass] * fraction
-        out.log_to_history(f'Split from object [{self.name}] @ fraction: {fraction}')
         out.rename(f'({fraction} * {self.name})')
 
         comp._obj[self._obj.mc_vars_mass] = comp._obj[self._obj.mc_vars_mass] * (1 - fraction)
-        comp.log_to_history(f'Split from object [{self.name}] @ 1 - fraction {fraction}: {1 - fraction}')
         comp.rename(f'({1 - fraction} * {self.name})')
 
-        # set the start and end nodes to the attributes
-        out._obj.attrs['nodes'] = [self._obj.attrs['nodes'][1], self._obj.attrs['nodes'][1] + 1]
-        comp._obj.attrs['nodes'] = [self._obj.attrs['nodes'][1], self._obj.attrs['nodes'][1] + 2]
-
         xr.set_options(keep_attrs='default')
 
         return out._obj, comp._obj
 
     def partition(self, definition: Callable) -> Tuple[xr.Dataset, xr.Dataset]:
         """Partition the object along a given dimension.
 
@@ -315,18 +305,14 @@
             # TODO: Set the dim to match the partition if it does not already
             # obj_mass = obj_mass.swap_dims(dim=)
             pass
 
         out._obj = out.mul(pn / 100)
         comp._obj = self.sub(out._obj)
 
-        # set the start and end nodes to the attributes
-        out._obj.attrs['nodes'] = [self._obj.attrs['nodes'][1], self._obj.attrs['nodes'][1] + 1]
-        comp._obj.attrs['nodes'] = [self._obj.attrs['nodes'][1], self._obj.attrs['nodes'][1] + 2]
-
         xr.set_options(keep_attrs='default')
 
         return out._obj, comp._obj
 
     def add(self, other: xr.Dataset) -> xr.Dataset:
         """Add two objects
 
@@ -345,20 +331,14 @@
         xr_self: xr.Dataset = self.composition_to_mass()[self.mc_vars]
         xr_other: xr.Dataset = other.mc.composition_to_mass()[self.mc_vars]
 
         res: xr.Dataset = xr_self + xr_other
 
         res = self._math_post_process(other, res, xr_self, 'added')
 
-        # when two objects (edges) are added, their to-nodes must be set to the same value (merged)
-        # then the nodes for the summed object will be from that merged node to the next, new node.
-        # add the start and end nodes to the attributes
-        # xr_other.attrs['nodes'][1] = xr_self.attrs['nodes'][1]
-        res.attrs['nodes'] = [self._obj.attrs['nodes'][1], self._obj.attrs['nodes'][1] + 1]
-
         xr.set_options(keep_attrs='default')
 
         return res
 
     def sub(self, other: xr.Dataset) -> xr.Dataset:
         """Subtract the supplied object from self
 
@@ -457,27 +437,23 @@
         res.attrs.update(self._obj.attrs)
         da: xr.DataArray
         for new_da, da in zip(res.values(), xr_self.values()):
             new_da.attrs.update(da.attrs)
         # merge in the attr vars
         res = xr.merge([res, self._obj[self._obj.mc_vars_attrs]])
         if operator_string == 'added':
-            res.mc.log_to_history(f'Object called {other.mc.name} has been {operator_string}.')
             res.mc.rename(f'({self.name} + {other.mc.name})')
             res = res.mc.mass_to_composition()
         elif operator_string == 'subtracted':
-            res.mc.log_to_history(f'Object called {other.mc.name} has been {operator_string}.')
             res.mc.rename(f'({self.name} - {other.mc.name})')
             res = res.mc.mass_to_composition()
         elif operator_string == 'divided':
-            res.mc.log_to_history(f'Object has been {operator_string} by {other.mc.name}.')
             res.mc.rename(f'({self.name} / {other.mc.name})')
             # division returns relative, not absolute - do not convert back to relative composition
         elif operator_string == 'multiplied':
-            res.mc.log_to_history(f'Object has been {operator_string} by one or more values.')
             res.mc.rename(f'({self.name} partitioned)')
             res = res.mc.mass_to_composition()
         else:
             raise NotImplementedError('Unexpected operator string')
 
         # protect grades from nans and infs - push them to zero
         res[res.mc_vars_chem] = res[res.mc_vars_chem].where(res[res.mc_vars_chem].map(np.isfinite), 0.0)
@@ -499,14 +475,24 @@
         col_order: List[str] = self.mc_vars_mass + ['H2O'] + self.mc_vars_chem + self.mc_vars_attrs
         df = df[[col for col in col_order if col in df.columns]]
 
         if original_column_names:
             df.rename(columns=self.column_map(), inplace=True)
         return df
 
+    def resample(self, dim: str, num_intervals: int = 50, edge_precision: int = 8) -> xr.Dataset:
+        if len(self._obj.dims) > 1:
+            raise NotImplementedError("Not yet tested on datasets > 1D")
+
+        # define the new coordinates
+        right_edges = pd.arrays.IntervalArray(self._obj[dim].data).right
+        new_coords = np.round(np.geomspace(right_edges.min(), right_edges.max(), num_intervals), edge_precision)
+        xr_upsampled: xr.Dataset = interp_monotonic(self._obj, coords={'size': new_coords},
+                                                    include_original_coords=True)
+        return xr_upsampled
 
 def mc_aggregate(xr_ds: xr.Dataset) -> xr.Dataset:
     """A standalone function to aggregate
 
     Sum the mass vars and weight average the chem vars by the mass_dry.
 
     Args:
```

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc` & `mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/components.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sat Mar 18 15:53:38 2023 UTC, .py size: 3036 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -23,86 +23,86 @@
 00000160: 8405 5a12 641f 6502 650a 1900 650f 6504  ..Z.d.e.e...e.e.
 00000170: 6502 650a 1900 6503 650a 650a 6602 1900  e.e...e.e.e.f...
 00000180: 6602 1900 6414 9c03 641b 641c 8405 5a13  f...d...d.d...Z.
 00000190: 6403 5300 2920 7a21 0a4d 616e 6167 696e  d.S.) z!.Managin
 000001a0: 6720 636f 6d70 6f6e 656e 7473 2f63 6f6d  g components/com
 000001b0: 706f 7369 7469 6f6e 0ae9 0000 0000 2903  position......).
 000001c0: da04 4c69 7374 da04 4469 6374 da05 556e  ..List..Dict..Un
-000001d0: 696f 6e4e 2901 da07 466f 726d 756c 61da  ionN)...Formula.
+000001d0: 696f 6e4e 2901 da07 466f 726d 756c 615a  ionN)...FormulaZ
 000001e0: 034c 4f49 da11 6375 7374 6f6d 5f63 6f6d  .LOI..custom_com
 000001f0: 706f 6e65 6e74 73e9 0100 0000 e903 0000  ponents.........
 00000200: 00e9 0400 0000 e9fe ffff ffe9 ffff ffff  ................
 00000210: e902 0000 00e9 0500 0000 2935 da01 485a  ..........)5..HZ
 00000220: 024c 695a 0242 65da 0142 da01 43da 014f  .LiZ.Be..B..C..O
 00000230: da01 46da 024e 615a 024d 675a 0241 6c5a  ..F..NaZ.MgZ.AlZ
 00000240: 0253 69da 0150 5a02 436c da01 4b5a 0243  .Si..PZ.Cl..KZ.C
-00000250: 615a 0253 635a 0254 69da 0156 da02 4372  aZ.ScZ.Ti..V..Cr
-00000260: da02 4d6e da02 4665 5a02 436f 5a02 4e69  ..Mn..FeZ.CoZ.Ni
+00000250: 61da 0253 635a 0254 69da 0156 da02 4372  a..ScZ.Ti..V..Cr
+00000260: da02 4d6e 5a02 4665 da02 436f 5a02 4e69  ..MnZ.Fe..CoZ.Ni
 00000270: 5a02 4375 5a02 5a6e 5a02 4272 5a02 5262  Z.CuZ.ZnZ.BrZ.Rb
 00000280: 5a02 5372 da01 595a 025a 725a 024e 625a  Z.Sr..YZ.ZrZ.NbZ
-00000290: 0253 6eda 0149 5a02 4373 5a02 4261 da02  .Sn..IZ.CsZ.Ba..
-000002a0: 4c61 5a02 4365 5a02 5072 5a02 4e64 5a02  LaZ.CeZ.PrZ.NdZ.
-000002b0: 536d 5a02 4575 5a02 4764 5a02 5462 5a02  SmZ.EuZ.GdZ.TbZ.
+00000290: 0253 6eda 0149 da02 4373 5a02 4261 da02  .Sn..I..CsZ.Ba..
+000002a0: 4c61 da02 4365 da02 5072 da02 4e64 da02  La..Ce..Pr..Nd..
+000002b0: 536d 5a02 4575 5a02 4764 da02 5462 5a02  SmZ.EuZ.Gd..TbZ.
 000002c0: 4479 5a02 486f 5a02 4572 5a02 546d 5a02  DyZ.HoZ.ErZ.TmZ.
-000002d0: 5962 5a02 4c75 da02 4866 5a02 5062 5a02  YbZ.Lu..HfZ.PbZ.
+000002d0: 5962 da02 4c75 da02 4866 5a02 5062 5a02  Yb..Lu..HfZ.PbZ.
 000002e0: 5468 da01 55da 0f44 4546 4155 4c54 5f43  Th..U..DEFAULT_C
 000002f0: 4841 5247 4553 2901 da06 7265 7475 726e  HARGES)...return
 00000300: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
 00000310: 0002 0000 0043 0000 0073 1400 0000 6401  .....C...s....d.
 00000320: 6402 8400 7400 6a01 4400 8301 7d00 7c00  d...t.j.D...}.|.
 00000330: 5300 2903 4e63 0100 0000 0000 0000 0000  S.).Nc..........
 00000340: 0000 0200 0000 0300 0000 5300 0000 7312  ..........S...s.
 00000350: 0000 0067 007c 005d 0a7d 017c 016a 0091  ...g.|.].}.|.j..
 00000360: 0271 0453 00a9 0029 01da 0673 796d 626f  .q.S...)...symbo
-00000370: 6ca9 02da 022e 30da 0265 6c72 2200 0000  l.....0..elr"...
-00000380: 7222 0000 00fa 4943 3a5c 7072 6f6a 6563  r"....IC:\projec
+00000370: 6ca9 02da 022e 30da 0265 6c72 2900 0000  l.....0..elr)...
+00000380: 7229 0000 00fa 4943 3a5c 7072 6f6a 6563  r)....IC:\projec
 00000390: 7473 5c6d 6173 732d 636f 6d70 6f73 6974  ts\mass-composit
 000003a0: 696f 6e5c 656c 7068 6963 6b5c 6d61 7373  ion\elphick\mass
 000003b0: 5f63 6f6d 706f 7369 7469 6f6e 5c75 7469  _composition\uti
 000003c0: 6c73 5c63 6f6d 706f 6e65 6e74 732e 7079  ls\components.py
 000003d0: da0a 3c6c 6973 7463 6f6d 703e 4700 0000  ..<listcomp>G...
 000003e0: f300 0000 007a 1c65 6c65 6d65 6e74 732e  .....z.elements.
 000003f0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
 00000400: 6d70 3e29 02da 0270 74da 0865 6c65 6d65  mp>)...pt..eleme
-00000410: 6e74 7329 01da 0372 6573 7222 0000 0072  nts)...resr"...r
-00000420: 2200 0000 7227 0000 0072 2b00 0000 4600  "...r'...r+...F.
-00000430: 0000 7304 0000 0000 0110 0172 2b00 0000  ..s........r+...
+00000410: 6e74 7329 01da 0372 6573 7229 0000 0072  nts)...resr)...r
+00000420: 2900 0000 722e 0000 0072 3200 0000 4600  )...r....r2...F.
+00000430: 0000 7304 0000 0000 0110 0172 3200 0000  ..s........r2...
 00000440: 5429 03da 0a63 616e 6469 6461 7465 73da  T)...candidates.
-00000450: 0673 7472 6963 7472 2100 0000 6302 0000  .strictr!...c...
+00000450: 0673 7472 6963 7472 2800 0000 6302 0000  .strictr(...c...
 00000460: 0000 0000 0000 0000 0003 0000 0004 0000  ................
 00000470: 0003 0000 0073 4000 0000 7c01 721a 7400  .....s@...|.r.t.
 00000480: 7401 7c00 8301 a002 7403 8300 a101 8301  t.|.....t.......
 00000490: 7d02 6e22 6401 6402 8400 7404 6a03 4400  }.n"d.d...t.j.D.
 000004a0: 8301 8900 8700 6601 6403 6402 8408 7c00  ......f.d.d...|.
 000004b0: 4400 8301 7d02 7c02 5300 2904 4e63 0100  D...}.|.S.).Nc..
 000004c0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
 000004d0: 0000 5300 0000 731a 0000 0069 007c 005d  ..S...s....i.|.]
 000004e0: 127d 017c 016a 00a0 01a1 007c 016a 0093  .}.|.j.....|.j..
-000004f0: 0271 0453 0072 2200 0000 2902 7223 0000  .q.S.r"...).r#..
-00000500: 00da 056c 6f77 6572 2902 7225 0000 00da  ...lower).r%....
-00000510: 0165 7222 0000 0072 2200 0000 7227 0000  .er"...r"...r'..
+000004f0: 0271 0453 0072 2900 0000 2902 722a 0000  .q.S.r)...).r*..
+00000500: 00da 056c 6f77 6572 2902 722c 0000 00da  ...lower).r,....
+00000510: 0165 7229 0000 0072 2900 0000 722e 0000  .er)...r)...r...
 00000520: 00da 0a3c 6469 6374 636f 6d70 3e4f 0000  ...<dictcomp>O..
-00000530: 0072 2900 0000 7a1e 6973 5f65 6c65 6d65  .r)...z.is_eleme
+00000530: 0072 3000 0000 7a1e 6973 5f65 6c65 6d65  .r0...z.is_eleme
 00000540: 6e74 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  nt.<locals>.<dic
 00000550: 7463 6f6d 703e 6301 0000 0000 0000 0000  tcomp>c.........
 00000560: 0000 0002 0000 0006 0000 0013 0000 0073  ...............s
 00000570: 2a00 0000 6900 7c00 5d22 7d01 7c01 a000  *...i.|.]"}.|...
 00000580: a100 8800 a001 a100 7600 7204 7c01 8800  ........v.r.|...
-00000590: 7c01 a000 a100 1900 9302 7104 5300 7222  |.........q.S.r"
-000005a0: 0000 00a9 0272 2f00 0000 da04 6b65 7973  .....r/.....keys
-000005b0: a902 7225 0000 00da 0163 a901 5a05 655f  ..r%.....c..Z.e_
-000005c0: 6d61 7072 2200 0000 7227 0000 0072 3100  mapr"...r'...r1.
-000005d0: 0000 5000 0000 7229 0000 0029 05da 046c  ..P...r)...)...l
+00000590: 7c01 a000 a100 1900 9302 7104 5300 7229  |.........q.S.r)
+000005a0: 0000 00a9 0272 3600 0000 da04 6b65 7973  .....r6.....keys
+000005b0: a902 722c 0000 00da 0163 a901 5a05 655f  ..r,.....c..Z.e_
+000005c0: 6d61 7072 2900 0000 722e 0000 0072 3800  mapr)...r....r8.
+000005d0: 0000 5000 0000 7230 0000 0029 05da 046c  ..P...r0...)...l
 000005e0: 6973 74da 0373 6574 da0c 696e 7465 7273  ist..set..inters
-000005f0: 6563 7469 6f6e 722b 0000 0072 2a00 0000  ectionr+...r*...
-00000600: 2903 722d 0000 0072 2e00 0000 da07 6d61  ).r-...r......ma
-00000610: 7463 6865 7372 2200 0000 7236 0000 0072  tchesr"...r6...r
-00000620: 2700 0000 da0a 6973 5f65 6c65 6d65 6e74  '.....is_element
+000005f0: 6563 7469 6f6e 7232 0000 0072 3100 0000  ectionr2...r1...
+00000600: 2903 7234 0000 0072 3500 0000 da07 6d61  ).r4...r5.....ma
+00000610: 7463 6865 7372 2900 0000 723d 0000 0072  tchesr)...r=...r
+00000620: 2e00 0000 da0a 6973 5f65 6c65 6d65 6e74  ......is_element
 00000630: 4b00 0000 730a 0000 0000 0104 0116 0210  K...s...........
-00000640: 0112 0272 3b00 0000 6300 0000 0000 0000  ...r;...c.......
+00000640: 0112 0272 4200 0000 6300 0000 0000 0000  ...rB...c.......
 00000650: 0000 0000 0004 0000 0009 0000 0043 0000  .............C..
 00000660: 0073 9000 0000 6401 6402 8400 7400 6a01  .s....d.d...t.j.
 00000670: 4400 8301 7d00 6700 7d01 7c00 4400 5d72  D...}.g.}.|.D.]r
 00000680: 7d02 7402 7403 7c02 8301 1900 7d03 7c03  }.t.t.|.....}.|.
 00000690: 6403 1600 6404 6b02 7262 7c01 a004 7400  d...d.k.rb|...t.
 000006a0: a005 7403 7c02 8301 7403 6405 8301 1700  ..t.|...t.d.....
 000006b0: 6406 1700 7403 7c03 6403 1a00 8301 1700  d...t.|.d.......
@@ -111,132 +111,132 @@
 000006e0: 1700 7403 7c03 8301 1700 a101 a101 0100  ..t.|...........
 000006f0: 7118 7c01 5300 2907 4e63 0100 0000 0000  q.|.S.).Nc......
 00000700: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
 00000710: 0000 7330 0000 0068 007c 005d 287d 0174  ..s0...h.|.](}.t
 00000720: 007c 0183 0174 01a0 02a1 0076 0072 0474  .|...t.....v.r.t
 00000730: 0174 007c 0183 0119 0064 006b 0472 047c  .t.|.....d.k.r.|
 00000740: 0192 0271 0453 0029 0172 0100 0000 2903  ...q.S.).r....).
-00000750: da03 7374 7272 2000 0000 7233 0000 0072  ..strr ...r3...r
-00000760: 2400 0000 7222 0000 0072 2200 0000 7227  $...r"...r"...r'
+00000750: da03 7374 7272 2700 0000 723a 0000 0072  ..strr'...r:...r
+00000760: 2b00 0000 7229 0000 0072 2900 0000 722e  +...r)...r)...r.
 00000770: 0000 00da 093c 7365 7463 6f6d 703e 5700  .....<setcomp>W.
-00000780: 0000 7229 0000 007a 196f 7869 6465 732e  ..r)...z.oxides.
+00000780: 0000 7230 0000 007a 196f 7869 6465 732e  ..r0...z.oxides.
 00000790: 3c6c 6f63 616c 733e 2e3c 7365 7463 6f6d  <locals>.<setcom
-000007a0: 703e 720d 0000 0072 0100 0000 7208 0000  p>r....r....r...
-000007b0: 0072 1200 0000 2906 722a 0000 0072 2b00  .r....).r*...r+.
-000007c0: 0000 7220 0000 0072 3c00 0000 da06 6170  ..r ...r<.....ap
-000007d0: 7065 6e64 5a07 666f 726d 756c 6129 04da  pendZ.formula)..
-000007e0: 0463 6174 7372 2c00 0000 7235 0000 005a  .catsr,...r5...Z
-000007f0: 0663 6861 7267 6572 2200 0000 7222 0000  .charger"...r"..
-00000800: 0072 2700 0000 da06 6f78 6964 6573 5500  .r'.....oxidesU.
+000007a0: 703e 720c 0000 0072 0100 0000 7207 0000  p>r....r....r...
+000007b0: 0072 1100 0000 2906 7231 0000 0072 3200  .r....).r1...r2.
+000007c0: 0000 7227 0000 0072 4300 0000 da06 6170  ..r'...rC.....ap
+000007d0: 7065 6e64 da07 666f 726d 756c 6129 04da  pend..formula)..
+000007e0: 0463 6174 7372 3300 0000 723c 0000 005a  .catsr3...r<...Z
+000007f0: 0663 6861 7267 6572 2900 0000 7229 0000  .charger)...r)..
+00000800: 0072 2e00 0000 da06 6f78 6964 6573 5500  .r......oxidesU.
 00000810: 0000 7310 0000 0000 0210 0204 0108 010c  ..s.............
-00000820: 010c 012e 022a 0272 4000 0000 6302 0000  .....*.r@...c...
+00000820: 010c 012e 022a 0272 4800 0000 6302 0000  .....*.rH...c...
 00000830: 0000 0000 0000 0000 0004 0000 0004 0000  ................
 00000840: 0003 0000 0073 4e00 0000 7c01 7228 6401  .....sN...|.r(d.
 00000850: 6402 8400 7400 8300 4400 8301 7d02 7401  d...t...D...}.t.
 00000860: 7402 7c00 8301 a003 7c02 a101 8301 7d03  t.|.....|.....}.
 00000870: 6e22 6403 6404 8400 7400 8300 4400 8301  n"d.d...t...D...
 00000880: 8900 8700 6601 6405 6404 8408 7c00 4400  ....f.d.d...|.D.
 00000890: 8301 7d03 7c03 5300 2906 4e63 0100 0000  ..}.|.S.).Nc....
 000008a0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
 000008b0: 5300 0000 7314 0000 0068 007c 005d 0c7d  S...s....h.|.].}
-000008c0: 0174 007c 0183 0192 0271 0453 0072 2200  .t.|.....q.S.r".
-000008d0: 0000 a901 723c 0000 00a9 0272 2500 0000  ....r<.....r%...
-000008e0: da01 6f72 2200 0000 7222 0000 0072 2700  ..or"...r"...r'.
-000008f0: 0000 723d 0000 0066 0000 0072 2900 0000  ..r=...f...r)...
+000008c0: 0174 007c 0183 0192 0271 0453 0072 2900  .t.|.....q.S.r).
+000008d0: 0000 a901 7243 0000 00a9 0272 2c00 0000  ....rC.....r,...
+000008e0: da01 6f72 2900 0000 7229 0000 0072 2e00  ..or)...r)...r..
+000008f0: 0000 7244 0000 0066 0000 0072 3000 0000  ..rD...f...r0...
 00000900: 7a1b 6973 5f6f 7869 6465 2e3c 6c6f 6361  z.is_oxide.<loca
 00000910: 6c73 3e2e 3c73 6574 636f 6d70 3e63 0100  ls>.<setcomp>c..
 00000920: 0000 0000 0000 0000 0000 0200 0000 0500  ................
 00000930: 0000 5300 0000 731e 0000 0069 007c 005d  ..S...s....i.|.]
 00000940: 167d 0174 007c 0183 01a0 01a1 0074 007c  .}.t.|.......t.|
-00000950: 0183 0193 0271 0453 0072 2200 0000 a902  .....q.S.r".....
-00000960: 723c 0000 0072 2f00 0000 7242 0000 0072  r<...r/...rB...r
-00000970: 2200 0000 7222 0000 0072 2700 0000 7231  "...r"...r'...r1
-00000980: 0000 0069 0000 0072 2900 0000 7a1c 6973  ...i...r)...z.is
+00000950: 0183 0193 0271 0453 0072 2900 0000 a902  .....q.S.r).....
+00000960: 7243 0000 0072 3600 0000 724a 0000 0072  rC...r6...rJ...r
+00000970: 2900 0000 7229 0000 0072 2e00 0000 7238  )...r)...r....r8
+00000980: 0000 0069 0000 0072 3000 0000 7a1c 6973  ...i...r0...z.is
 00000990: 5f6f 7869 6465 2e3c 6c6f 6361 6c73 3e2e  _oxide.<locals>.
 000009a0: 3c64 6963 7463 6f6d 703e 6301 0000 0000  <dictcomp>c.....
 000009b0: 0000 0000 0000 0002 0000 0006 0000 0013  ................
 000009c0: 0000 0073 2a00 0000 6900 7c00 5d22 7d01  ...s*...i.|.]"}.
 000009d0: 7c01 a000 a100 8800 a001 a100 7600 7204  |...........v.r.
 000009e0: 7c01 8800 7c01 a000 a100 1900 9302 7104  |...|.........q.
-000009f0: 5300 7222 0000 0072 3200 0000 7234 0000  S.r"...r2...r4..
-00000a00: 00a9 015a 056f 5f6d 6170 7222 0000 0072  ...Z.o_mapr"...r
-00000a10: 2700 0000 7231 0000 006a 0000 0072 2900  '...r1...j...r).
-00000a20: 0000 2904 7240 0000 0072 3700 0000 7238  ..).r@...r7...r8
-00000a30: 0000 0072 3900 0000 2904 722d 0000 0072  ...r9...).r-...r
-00000a40: 2e00 0000 5a03 6f78 7372 3a00 0000 7222  ....Z.oxsr:...r"
-00000a50: 0000 0072 4500 0000 7227 0000 00da 0869  ...rE...r'.....i
+000009f0: 5300 7229 0000 0072 3900 0000 723b 0000  S.r)...r9...r;..
+00000a00: 00a9 015a 056f 5f6d 6170 7229 0000 0072  ...Z.o_mapr)...r
+00000a10: 2e00 0000 7238 0000 006a 0000 0072 3000  ....r8...j...r0.
+00000a20: 0000 2904 7248 0000 0072 3e00 0000 723f  ..).rH...r>...r?
+00000a30: 0000 0072 4000 0000 2904 7234 0000 0072  ...r@...).r4...r
+00000a40: 3500 0000 5a03 6f78 7372 4100 0000 7229  5...Z.oxsrA...r)
+00000a50: 0000 0072 4d00 0000 722e 0000 00da 0869  ...rM...r......i
 00000a60: 735f 6f78 6964 6564 0000 0073 0c00 0000  s_oxided...s....
-00000a70: 0001 0401 1001 1402 1001 1202 7246 0000  ............rF..
+00000a70: 0001 0401 1001 1402 1001 1202 724e 0000  ............rN..
 00000a80: 0063 0200 0000 0000 0000 0000 0000 0400  .c..............
 00000a90: 0000 0400 0000 0300 0000 7386 0000 007c  ..........s....|
 00000aa0: 0172 3e64 0164 0284 0074 0083 0044 0083  .r>d.d...t...D..
 00000ab0: 01a0 0174 0274 0383 0083 01a1 01a0 0174  ...t.t.........t
 00000ac0: 0274 0483 01a1 017d 0274 0574 027c 0083  .t.....}.t.t.|..
 00000ad0: 01a0 067c 02a1 0183 017d 036e 4469 0064  ...|.....}.nDi.d
 00000ae0: 0364 0484 0074 0083 0044 0083 01a5 0164  .d...t...D.....d
 00000af0: 0564 0484 0074 0383 0044 0083 01a5 0164  .d...t...D.....d
 00000b00: 0664 0484 0074 0444 0083 01a5 0189 0087  .d...t.D........
 00000b10: 0066 0164 0764 0484 087c 0044 0083 017d  .f.d.d...|.D...}
 00000b20: 037c 0353 0029 084e 6301 0000 0000 0000  .|.S.).Nc.......
 00000b30: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
 00000b40: 0073 1400 0000 6800 7c00 5d0c 7d01 7400  .s....h.|.].}.t.
-00000b50: 7c01 8301 9202 7104 5300 7222 0000 0072  |.....q.S.r"...r
-00000b60: 4100 0000 7242 0000 0072 2200 0000 7222  A...rB...r"...r"
-00000b70: 0000 0072 2700 0000 723d 0000 0071 0000  ...r'...r=...q..
-00000b80: 0072 2900 0000 7a23 6973 5f63 6f6d 706f  .r)...z#is_compo
+00000b50: 7c01 8301 9202 7104 5300 7229 0000 0072  |.....q.S.r)...r
+00000b60: 4900 0000 724a 0000 0072 2900 0000 7229  I...rJ...r)...r)
+00000b70: 0000 0072 2e00 0000 7244 0000 0071 0000  ...r....rD...q..
+00000b80: 0072 3000 0000 7a23 6973 5f63 6f6d 706f  .r0...z#is_compo
 00000b90: 7369 7469 6f6e 616c 2e3c 6c6f 6361 6c73  sitional.<locals
 00000ba0: 3e2e 3c73 6574 636f 6d70 3e63 0100 0000  >.<setcomp>c....
 00000bb0: 0000 0000 0000 0000 0200 0000 0500 0000  ................
 00000bc0: 5300 0000 731e 0000 0069 007c 005d 167d  S...s....i.|.].}
 00000bd0: 0174 007c 0183 01a0 01a1 0074 007c 0183  .t.|.......t.|..
-00000be0: 0193 0271 0453 0072 2200 0000 7244 0000  ...q.S.r"...rD..
-00000bf0: 0072 4200 0000 7222 0000 0072 2200 0000  .rB...r"...r"...
-00000c00: 7227 0000 0072 3100 0000 7400 0000 7229  r'...r1...t...r)
+00000be0: 0193 0271 0453 0072 2900 0000 724c 0000  ...q.S.r)...rL..
+00000bf0: 0072 4a00 0000 7229 0000 0072 2900 0000  .rJ...r)...r)...
+00000c00: 722e 0000 0072 3800 0000 7400 0000 7230  r....r8...t...r0
 00000c10: 0000 007a 2469 735f 636f 6d70 6f73 6974  ...z$is_composit
 00000c20: 696f 6e61 6c2e 3c6c 6f63 616c 733e 2e3c  ional.<locals>.<
 00000c30: 6469 6374 636f 6d70 3e63 0100 0000 0000  dictcomp>c......
 00000c40: 0000 0000 0000 0200 0000 0400 0000 5300  ..............S.
 00000c50: 0000 7316 0000 0069 007c 005d 0e7d 017c  ..s....i.|.].}.|
-00000c60: 01a0 00a1 007c 0193 0271 0453 0072 2200  .....|...q.S.r".
-00000c70: 0000 a901 722f 0000 0029 0272 2500 0000  ....r/...).r%...
-00000c80: da01 6172 2200 0000 7222 0000 0072 2700  ..ar"...r"...r'.
-00000c90: 0000 7231 0000 0075 0000 0072 2900 0000  ..r1...u...r)...
+00000c60: 01a0 00a1 007c 0193 0271 0453 0072 2900  .....|...q.S.r).
+00000c70: 0000 a901 7236 0000 0029 0272 2c00 0000  ....r6...).r,...
+00000c80: da01 6172 2900 0000 7229 0000 0072 2e00  ..ar)...r)...r..
+00000c90: 0000 7238 0000 0075 0000 0072 3000 0000  ..r8...u...r0...
 00000ca0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
 00000cb0: 0004 0000 0053 0000 0073 1600 0000 6900  .....S...s....i.
 00000cc0: 7c00 5d0e 7d01 7c01 a000 a100 7c01 9302  |.].}.|.....|...
-00000cd0: 7104 5300 7222 0000 0072 4700 0000 7234  q.S.r"...rG...r4
-00000ce0: 0000 0072 2200 0000 7222 0000 0072 2700  ...r"...r"...r'.
-00000cf0: 0000 7231 0000 0076 0000 0072 2900 0000  ..r1...v...r)...
+00000cd0: 7104 5300 7229 0000 0072 4f00 0000 723b  q.S.r)...rO...r;
+00000ce0: 0000 0072 2900 0000 7229 0000 0072 2e00  ...r)...r)...r..
+00000cf0: 0000 7238 0000 0076 0000 0072 3000 0000  ..r8...v...r0...
 00000d00: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
 00000d10: 0006 0000 0013 0000 0073 2a00 0000 6900  .........s*...i.
 00000d20: 7c00 5d22 7d01 7c01 a000 a100 8800 a001  |.]"}.|.........
 00000d30: a100 7600 7204 7c01 8800 7c01 a000 a100  ..v.r.|...|.....
-00000d40: 1900 9302 7104 5300 7222 0000 0072 3200  ....q.S.r"...r2.
-00000d50: 0000 7234 0000 00a9 015a 0863 6f6d 705f  ..r4.....Z.comp_
-00000d60: 6d61 7072 2200 0000 7227 0000 0072 3100  mapr"...r'...r1.
-00000d70: 0000 7700 0000 7229 0000 0029 0772 4000  ..w...r)...).r@.
-00000d80: 0000 da05 756e 696f 6e72 3800 0000 722b  ....unionr8...r+
-00000d90: 0000 0072 0700 0000 7237 0000 0072 3900  ...r....r7...r9.
-00000da0: 0000 2904 722d 0000 0072 2e00 0000 da05  ..).r-...r......
-00000db0: 636f 6d70 7372 3a00 0000 7222 0000 0072  compsr:...r"...r
-00000dc0: 4900 0000 7227 0000 00da 1069 735f 636f  I...r'.....is_co
+00000d40: 1900 9302 7104 5300 7229 0000 0072 3900  ....q.S.r)...r9.
+00000d50: 0000 723b 0000 00a9 015a 0863 6f6d 705f  ..r;.....Z.comp_
+00000d60: 6d61 7072 2900 0000 722e 0000 0072 3800  mapr)...r....r8.
+00000d70: 0000 7700 0000 7230 0000 0029 0772 4800  ..w...r0...).rH.
+00000d80: 0000 da05 756e 696f 6e72 3f00 0000 7232  ....unionr?...r2
+00000d90: 0000 0072 0600 0000 723e 0000 0072 4000  ...r....r>...r@.
+00000da0: 0000 2904 7234 0000 0072 3500 0000 da05  ..).r4...r5.....
+00000db0: 636f 6d70 7372 4100 0000 7229 0000 0072  compsrA...r)...r
+00000dc0: 5100 0000 722e 0000 00da 1069 735f 636f  Q...r......is_co
 00000dd0: 6d70 6f73 6974 696f 6e61 6c6f 0000 0073  mpositionalo...s
 00000de0: 1400 0000 0001 0401 2601 1402 1201 0eff  ........&.......
-00000df0: 0202 0cfe 0403 1202 724c 0000 0029 0154  ........rL...).T
+00000df0: 0202 0cfe 0403 1202 7254 0000 0029 0154  ........rT...).T
 00000e00: 2901 5429 0154 2914 da07 5f5f 646f 635f  ).T).T)...__doc_
 00000e10: 5fda 0674 7970 696e 6772 0200 0000 7203  _..typingr....r.
 00000e20: 0000 0072 0400 0000 5a0d 7065 7269 6f64  ...r....Z.period
-00000e30: 6963 7461 626c 6572 2a00 0000 5a16 7065  ictabler*...Z.pe
+00000e30: 6963 7461 626c 6572 3100 0000 5a16 7065  ictabler1...Z.pe
 00000e40: 7269 6f64 6963 7461 626c 652e 666f 726d  riodictable.form
-00000e50: 756c 6173 7205 0000 0072 0700 0000 723c  ulasr....r....r<
+00000e50: 756c 6173 7205 0000 0072 0600 0000 7243  ulasr....r....rC
 00000e60: 0000 00da 0f5f 5f61 6e6e 6f74 6174 696f  .....__annotatio
-00000e70: 6e73 5f5f da04 6469 6374 7220 0000 0072  ns__..dictr ...r
-00000e80: 2b00 0000 da04 626f 6f6c 723b 0000 0072  +.....boolr;...r
-00000e90: 4000 0000 7246 0000 0072 4c00 0000 7222  @...rF...rL...r"
-00000ea0: 0000 0072 2200 0000 7222 0000 0072 2700  ...r"...r"...r'.
+00000e70: 6e73 5f5f da04 6469 6374 7227 0000 0072  ns__..dictr'...r
+00000e80: 3200 0000 da04 626f 6f6c 7242 0000 0072  2.....boolrB...r
+00000e90: 4800 0000 724e 0000 0072 5400 0000 7229  H...rN...rT...r)
+00000ea0: 0000 0072 2900 0000 7229 0000 0072 2e00  ...r)...r)...r..
 00000eb0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
 00000ec0: 7380 0000 0006 0414 0208 010c 0212 0302  s...............
 00000ed0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 00000ee0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 00000ef0: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 00000f00: 0102 0102 0102 0102 0102 0102 0102 0102  ................
 00000f10: 0102 0102 0102 0102 0102 0102 0102 0102  ................
```

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc` & `mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/moisture.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/size.cpython-39.pyc` & `mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/size.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Apr  2 04:14:35 2023 UTC, .py size: 927 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 2b01 2964 9f03 0000  a.......+.)d....
+00000000: 610d 0d0a 0000 0000 3bfd 7164 9d03 0000  a.......;.qd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2a00 0000 6400  .....@...s*...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6503 6501 6a04 6403 9c02 6404 6405  ..e.e.j.d...d.d.
 00000050: 8404 5a05 6401 5300 2906 e900 0000 004e  ..Z.d.S.)......N
 00000060: 2901 da0d 496e 7465 7276 616c 4172 7261  )...IntervalArra
 00000070: 7929 02da 0e73 697a 655f 696e 7465 7276  y)...size_interv
@@ -11,57 +11,57 @@
 000000a0: 4300 0000 736a 0000 007c 00a0 00a1 007d  C...sj...|.....}
 000000b0: 0174 01a0 027c 016a 037c 016a 0414 0064  .t...|.j.|.j...d
 000000c0: 0113 00a1 017d 0274 0574 01a0 067c 0264  .....}.t.t...|.d
 000000d0: 0264 0385 0219 007c 016a 0764 0264 0385  .d.....|.j.d.d..
 000000e0: 0219 001b 00a1 0183 017d 0374 01a0 087c  .........}.t...|
 000000f0: 00a0 09a1 006a 0364 04a1 0272 667c 00a0  .....j.d...rf|..
 00000100: 09a1 006a 077c 0314 007c 0264 033c 007c  ...j.|...|.d.<.|
-00000110: 0253 0029 0561 c101 0000 4765 6f6d 6574  .S.).a....Geomet
+00000110: 0253 0029 0561 bf01 0000 4765 6f6d 6574  .S.).a....Geomet
 00000120: 7269 6320 6d65 616e 2073 697a 650a 0a20  ric mean size.. 
 00000130: 2020 2053 697a 6520 6361 6c63 756c 6174     Size calculat
 00000140: 696f 6e73 2061 7265 2070 6572 666f 726d  ions are perform
 00000150: 6564 2075 7369 6e67 2074 6865 2067 656f  ed using the geo
 00000160: 6d65 7472 6963 206d 6561 6e2c 206e 6f74  metric mean, not
 00000170: 2074 6865 2061 7269 7468 6d65 7469 6320   the arithmetic 
 00000180: 6d65 616e 0a0a 2020 2020 4e4f 5445 3a20  mean..    NOTE: 
 00000190: 4966 2067 656f 6d65 7472 6963 206d 6561  If geometric mea
 000001a0: 6e20 6973 2075 7365 6420 666f 7220 7468  n is used for th
 000001b0: 6520 7061 6e20 6672 6163 7469 6f6e 2028  e pan fraction (
 000001c0: 302e 306d 6d20 7265 7461 696e 6564 2920  0.0mm retained) 
 000001d0: 6974 2077 696c 6c20 7265 7475 726e 207a  it will return z
 000001e0: 6572 6f2c 2077 6869 6368 2069 7320 616e  ero, which is an
-000001f0: 640a 2020 2020 6564 6765 2073 697a 6520  d.    edge size 
-00000200: 6e6f 7420 6d65 616e 2073 697a 652e 2020  not mean size.  
-00000210: 536f 2074 6865 206d 6561 6e20 7261 7469  So the mean rati
-00000220: 6f20 6f66 2074 6865 2067 656f 6d65 7472  o of the geometr
-00000230: 6963 206d 6561 6e20 746f 2074 6865 2061  ic mean to the a
-00000240: 7269 7468 6d65 7469 6320 6d65 616e 2066  rithmetic mean f
-00000250: 6f72 2061 6c6c 206f 7468 6572 0a20 2020  or all other.   
-00000260: 2020 6672 6163 7469 6f6e 7320 6973 2075    fractions is u
-00000270: 7365 6420 666f 7220 7468 6520 626f 7474  sed for the bott
-00000280: 6f6d 2066 7261 6374 696f 6e2e 0a0a 0a20  om fraction.... 
-00000290: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-000002a0: 2073 697a 655f 696e 7465 7276 616c 733a   size_intervals:
-000002b0: 2041 2070 616e 6461 7320 496e 7465 7276   A pandas Interv
-000002c0: 616c 4172 7261 790a 0a20 2020 2052 6574  alArray..    Ret
-000002d0: 7572 6e73 3a0a 0a20 2020 2067 0000 0000  urns:..    g....
-000002e0: 0000 e03f 7201 0000 00e9 ffff ffff 6700  ...?r.........g.
-000002f0: 0000 0000 0000 0029 0ada 0463 6f70 79da  .......)...copy.
-00000300: 026e 70da 0561 7272 6179 da04 6c65 6674  .np..array..left
-00000310: da05 7269 6768 74da 0566 6c6f 6174 da04  ..right..float..
-00000320: 6d65 616e da03 6d69 64da 0769 7363 6c6f  mean..mid..isclo
-00000330: 7365 da03 6d69 6e29 0472 0300 0000 da09  se..min).r......
-00000340: 696e 7465 7276 616c 73da 0372 6573 5a12  intervals..resZ.
-00000350: 6765 6f6d 6561 6e5f 6d65 616e 5f72 6174  geomean_mean_rat
-00000360: 696f a900 7212 0000 00fa 4343 3a5c 7072  io..r.....CC:\pr
-00000370: 6f6a 6563 7473 5c6d 6173 732d 636f 6d70  ojects\mass-comp
-00000380: 6f73 6974 696f 6e5c 656c 7068 6963 6b5c  osition\elphick\
-00000390: 6d61 7373 5f63 6f6d 706f 7369 7469 6f6e  mass_composition
-000003a0: 5c75 7469 6c73 5c73 697a 652e 7079 da09  \utils\size.py..
-000003b0: 6d65 616e 5f73 697a 6505 0000 0073 0c00  mean_size....s..
-000003c0: 0000 0011 0801 1602 2402 1201 1202 7214  ........$.....r.
-000003d0: 0000 0029 06da 056e 756d 7079 7207 0000  ...)...numpyr...
-000003e0: 00da 0d70 616e 6461 732e 6172 7261 7973  ...pandas.arrays
-000003f0: 7202 0000 00da 076e 6461 7272 6179 7214  r......ndarrayr.
-00000400: 0000 0072 1200 0000 7212 0000 0072 1200  ...r....r....r..
-00000410: 0000 7213 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000420: 3e01 0000 0073 0400 0000 0801 0c03       >....s........
+000001f0: 0a20 2020 2065 6467 6520 7369 7a65 206e  .    edge size n
+00000200: 6f74 206d 6561 6e20 7369 7a65 2e20 2053  ot mean size.  S
+00000210: 6f20 7468 6520 6d65 616e 2072 6174 696f  o the mean ratio
+00000220: 206f 6620 7468 6520 6765 6f6d 6574 7269   of the geometri
+00000230: 6320 6d65 616e 2074 6f20 7468 6520 6172  c mean to the ar
+00000240: 6974 686d 6574 6963 206d 6561 6e20 666f  ithmetic mean fo
+00000250: 7220 616c 6c20 6f74 6865 720a 2020 2020  r all other.    
+00000260: 6672 6163 7469 6f6e 7320 6973 2075 7365  fractions is use
+00000270: 6420 666f 7220 7468 6520 626f 7474 6f6d  d for the bottom
+00000280: 2066 7261 6374 696f 6e2e 0a0a 0a20 2020   fraction....   
+00000290: 2041 7267 733a 0a20 2020 2020 2020 2073   Args:.        s
+000002a0: 697a 655f 696e 7465 7276 616c 733a 2041  ize_intervals: A
+000002b0: 2070 616e 6461 7320 496e 7465 7276 616c   pandas Interval
+000002c0: 4172 7261 790a 0a20 2020 2052 6574 7572  Array..    Retur
+000002d0: 6e73 3a0a 0a20 2020 2067 0000 0000 0000  ns:..    g......
+000002e0: e03f 7201 0000 00e9 ffff ffff 6700 0000  .?r.........g...
+000002f0: 0000 0000 0029 0ada 0463 6f70 79da 026e  .....)...copy..n
+00000300: 70da 0561 7272 6179 da04 6c65 6674 da05  p..array..left..
+00000310: 7269 6768 74da 0566 6c6f 6174 da04 6d65  right..float..me
+00000320: 616e da03 6d69 64da 0769 7363 6c6f 7365  an..mid..isclose
+00000330: da03 6d69 6e29 0472 0300 0000 da09 696e  ..min).r......in
+00000340: 7465 7276 616c 73da 0372 6573 5a12 6765  tervals..resZ.ge
+00000350: 6f6d 6561 6e5f 6d65 616e 5f72 6174 696f  omean_mean_ratio
+00000360: a900 7212 0000 00fa 4343 3a5c 7072 6f6a  ..r.....CC:\proj
+00000370: 6563 7473 5c6d 6173 732d 636f 6d70 6f73  ects\mass-compos
+00000380: 6974 696f 6e5c 656c 7068 6963 6b5c 6d61  ition\elphick\ma
+00000390: 7373 5f63 6f6d 706f 7369 7469 6f6e 5c75  ss_composition\u
+000003a0: 7469 6c73 5c73 697a 652e 7079 da09 6d65  tils\size.py..me
+000003b0: 616e 5f73 697a 6505 0000 0073 0c00 0000  an_size....s....
+000003c0: 0011 0801 1602 2402 1201 1202 7214 0000  ......$.....r...
+000003d0: 0029 06da 056e 756d 7079 7207 0000 00da  .)...numpyr.....
+000003e0: 0d70 616e 6461 732e 6172 7261 7973 7202  .pandas.arraysr.
+000003f0: 0000 00da 076e 6461 7272 6179 7214 0000  .....ndarrayr...
+00000400: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00000410: 7213 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000420: 0000 0073 0400 0000 0801 0c03            ...s........
```

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/size_distribution.cpython-39.pyc` & `mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/size_distribution.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Mar 13 09:45:20 2023 UTC, .py size: 2941 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,196 +1,182 @@
-00000000: 610d 0d0a 0000 0000 b0f0 0e64 7d0b 0000  a..........d}...
+00000000: 610d 0d0a 0000 0000 39e0 1564 aa0a 0000  a.......9..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0007 0000 0040 0000 0073 e400 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 5a03 6400 6402 6c04 5a05 6503 a006 6700  Z.d.d.l.Z.e...g.
-00000050: 6403 a201 a101 6404 6405 6603 6503 6a07  d.....d.d.f.e.j.
-00000060: 6508 1900 6508 6508 6406 9c03 6407 6408  e...e.e.d...d.d.
-00000070: 8405 5a09 6503 a006 6700 6403 a201 a101  ..Z.e...g.d.....
-00000080: 6404 6405 6603 6501 6503 6a07 6508 1900  d.d.f.e.e.j.e...
-00000090: 6505 6a0a 6602 1900 6508 6508 6501 6503  e.j.f...e.e.e.e.
-000000a0: 6a07 6508 1900 6505 6a0a 6602 1900 6409  j.e...e.j.f...d.
-000000b0: 9c04 640a 640b 8405 5a0b 6503 a006 6700  ..d.d...Z.e...g.
-000000c0: 6403 a201 a101 640c 640d 6603 6503 6a07  d.....d.d.f.e.j.
-000000d0: 6508 1900 6508 6508 640e 9c03 640f 6410  e...e.e.d...d.d.
-000000e0: 8405 5a0c 6503 a006 6700 6403 a201 a101  ..Z.e...g.d.....
-000000f0: 6411 6405 6603 6503 6a07 6508 1900 6508  d.d.f.e.j.e...e.
-00000100: 6508 6412 9c03 6413 6414 8405 5a0d 6402  e.d...d.d...Z.d.
-00000110: 5300 2915 e900 0000 0029 01da 0555 6e69  S.)......)...Uni
-00000120: 6f6e 4e29 0567 6666 6666 66e6 4a40 67cd  onN).gfffff.J@g.
-00000130: cccc cccc 0c43 4067 3333 3333 33b3 3a40  .....C@g33333.:@
-00000140: 67cd cccc cccc cc32 4067 9a99 9999 9999  g......2@g......
-00000150: 2a40 e90a 0000 0067 b81e 85eb 51b8 f63f  *@.....g....Q..?
-00000160: 2903 da01 64da 0161 da01 6263 0300 0000  )...d..a..bc....
-00000170: 0000 0000 0000 0000 0400 0000 0600 0000  ................
-00000180: 4300 0000 7320 0000 0064 0164 0274 00a0  C...s ...d.d.t..
-00000190: 017c 007c 011b 007c 0213 000b 00a1 0118  .|.|...|........
-000001a0: 0014 007d 037c 0353 0029 0361 ba01 0000  ...}.|.S.).a....
-000001b0: 5468 6520 526f 7369 6e2d 5261 6d6d 6c65  The Rosin-Rammle
-000001c0: 7220 6571 7561 7469 6f6e 0a0a 2020 2020  r equation..    
-000001d0: 5468 6520 526f 7369 6e2d 5261 6d6d 6c65  The Rosin-Rammle
-000001e0: 7220 6571 7561 7469 6f6e 2075 7365 6420  r equation used 
-000001f0: 746f 2064 6574 6572 6d69 6e65 2074 6865  to determine the
-00000200: 2073 697a 6520 6469 7374 7269 6275 7469   size distributi
-00000210: 6f6e 2069 7320 6173 2066 6f6c 6c6f 7773  on is as follows
-00000220: 3a0a 0a20 2020 206d 7020 3d20 3130 3020  :..    mp = 100 
-00000230: 2a20 2831 202d 2065 7870 202a 2028 2d28  * (1 - exp * (-(
-00000240: 642f 6129 2a2a 6229 290a 0a20 2020 2077  d/a)**b))..    w
-00000250: 6865 7265 3a0a 2020 2020 6d70 203d 206d  here:.    mp = m
-00000260: 6173 7320 6672 6163 7469 6f6e 2070 6173  ass fraction pas
-00000270: 7369 6e67 2028 2529 0a20 2020 2064 203d  sing (%).    d =
-00000280: 2070 6172 7469 636c 6520 6469 616d 6574   particle diamet
-00000290: 6572 0a20 2020 2061 203d 2073 697a 6520  er.    a = size 
-000002a0: 6174 2077 6869 6368 2028 3130 302f 6529  at which (100/e)
-000002b0: 203d 2033 362e 3825 206f 6620 7061 7274   = 36.8% of part
-000002c0: 6963 6c65 7320 7265 7461 696e 6564 0a20  icles retained. 
-000002d0: 2020 2062 203d 2063 6f6e 7374 616e 7420     b = constant 
-000002e0: 3d20 736c 6f70 6520 6f66 2074 6865 2070  = slope of the p
-000002f0: 6c6f 7420 6f66 206c 6e28 3130 302f 7770  lot of ln(100/wp
-00000300: 2920 7673 206c 6e20 780a 0a20 2020 2052  ) vs ln x..    R
-00000310: 4546 3a20 6874 7470 733a 2f2f 6865 6c70  EF: https://help
-00000320: 2e73 7973 6361 642e 6e65 742f 5369 7a65  .syscad.net/Size
-00000330: 5f44 6973 7472 6962 7574 696f 6e5f 4465  _Distribution_De
-00000340: 6669 6e69 7469 6f6e 2352 6f73 696e 2d52  finition#Rosin-R
-00000350: 616d 6d6c 6572 0a0a 2020 2020 5265 7475  ammler..    Retu
-00000360: 726e 733a 0a0a 2020 2020 e964 0000 00e9  rns:..    .d....
-00000370: 0100 0000 a902 da02 6e70 da03 6578 7029  ........np..exp)
-00000380: 0472 0400 0000 7205 0000 0072 0600 0000  .r....r....r....
-00000390: da02 6d70 a900 720d 0000 00fa 5043 3a5c  ..mp..r.....PC:\
-000003a0: 7072 6f6a 6563 7473 5c6d 6173 732d 636f  projects\mass-co
-000003b0: 6d70 6f73 6974 696f 6e5c 656c 7068 6963  mposition\elphic
-000003c0: 6b5c 6d61 7373 5f63 6f6d 706f 7369 7469  k\mass_compositi
-000003d0: 6f6e 5c75 7469 6c73 5c73 697a 655f 6469  on\utils\size_di
-000003e0: 7374 7269 6275 7469 6f6e 2e70 79da 0d72  stribution.py..r
-000003f0: 6f73 696e 5f72 616d 6d6c 6572 0700 0000  osin_rammler....
-00000400: 7304 0000 0000 151c 0172 0f00 0000 2904  s........r....).
-00000410: 7204 0000 00da 0364 3530 da01 6dda 0672  r......d50..m..r
-00000420: 6574 7572 6e63 0300 0000 0000 0000 0000  eturnc..........
-00000430: 0000 0400 0000 0700 0000 4300 0000 7340  ..........C...s@
-00000440: 0000 0064 0164 0274 00a0 0164 037c 007c  ...d.d.t...d.|.|
-00000450: 011b 007c 0213 0014 00a1 0118 0014 007d  ...|...........}
-00000460: 0374 027c 0074 036a 0483 0272 3c74 036a  .t.|.t.j...r<t.j
-00000470: 047c 037c 006a 0564 0464 058d 037d 037c  .|.|.j.d.d...}.|
-00000480: 0353 0029 0661 ac01 0000 5468 6520 4d6f  .S.).a....The Mo
-00000490: 6469 6669 6564 2052 6f73 696e 2d52 616d  dified Rosin-Ram
-000004a0: 6d6c 6572 2065 7175 6174 696f 6e0a 0a20  mler equation.. 
-000004b0: 2020 2054 6865 2052 6f73 696e 2d52 616d     The Rosin-Ram
-000004c0: 6d6c 6572 2065 7175 6174 696f 6e20 7573  mler equation us
-000004d0: 6564 2074 6f20 6465 7465 726d 696e 6520  ed to determine 
-000004e0: 7468 6520 7369 7a65 2064 6973 7472 6962  the size distrib
-000004f0: 7574 696f 6e20 6973 2061 7320 666f 6c6c  ution is as foll
-00000500: 6f77 733a 0a0a 2020 2020 6d70 203d 2031  ows:..    mp = 1
-00000510: 3030 202a 2028 3120 2d20 6578 7020 2a20  00 * (1 - exp * 
-00000520: 282d 2d30 2e36 3933 3134 3728 642f 6435  (--0.693147(d/d5
-00000530: 3029 2a2a 6d29 290a 0a20 2020 2077 6865  0)**m))..    whe
-00000540: 7265 3a0a 2020 2020 6d70 203d 206d 6173  re:.    mp = mas
-00000550: 7320 6672 6163 7469 6f6e 2070 6173 7369  s fraction passi
-00000560: 6e67 2028 2529 0a20 2020 2064 203d 2070  ng (%).    d = p
-00000570: 6172 7469 636c 6520 6469 616d 6574 6572  article diameter
-00000580: 0a20 2020 2064 3530 203d 2073 697a 6520  .    d50 = size 
-00000590: 6174 2077 6869 6368 2035 3025 206f 6620  at which 50% of 
-000005a0: 7061 7274 6963 6c65 7320 7265 7461 696e  particles retain
-000005b0: 6564 2062 7920 6d61 7373 0a20 2020 206d  ed by mass.    m
-000005c0: 203d 2073 6861 7270 6e65 7373 2063 6f6e   = sharpness con
-000005d0: 7374 616e 740a 0a20 2020 2052 4546 3a20  stant..    REF: 
-000005e0: 6874 7470 733a 2f2f 6865 6c70 2e73 7973  https://help.sys
-000005f0: 6361 642e 6e65 742f 5369 7a65 5f44 6973  cad.net/Size_Dis
-00000600: 7472 6962 7574 696f 6e5f 4465 6669 6e69  tribution_Defini
-00000610: 7469 6f6e 2352 6f73 696e 2d52 616d 6d6c  tion#Rosin-Ramml
-00000620: 6572 0a0a 2020 2020 5265 7475 726e 733a  er..    Returns:
-00000630: 0a0a 2020 2020 7207 0000 0072 0800 0000  ..    r....r....
-00000640: 67a2 410a 9e42 2ee6 bf5a 0e77 745f 7063  g.A..B...Z.wt_pc
-00000650: 745f 7061 7373 696e 6729 03da 0464 6174  t_passing)...dat
-00000660: 61da 0569 6e64 6578 da04 6e61 6d65 2906  a..index..name).
-00000670: 720a 0000 0072 0b00 0000 da0a 6973 696e  r....r......isin
-00000680: 7374 616e 6365 da02 7064 da06 5365 7269  stance..pd..Seri
-00000690: 6573 7214 0000 0029 0472 0400 0000 7210  esr....).r....r.
-000006a0: 0000 0072 1100 0000 720c 0000 0072 0d00  ...r....r....r..
-000006b0: 0000 720d 0000 0072 0e00 0000 da16 6d6f  ..r....r......mo
-000006c0: 6469 6669 6564 5f72 6f73 696e 5f72 616d  dified_rosin_ram
-000006d0: 6d6c 6572 2000 0000 7308 0000 0000 151e  mler ...s.......
-000006e0: 010c 0112 0172 1900 0000 695e 0100 0067  .....r....i^...g
-000006f0: b81e 85eb 51b8 e63f 2903 7204 0000 00da  ....Q..?).r.....
-00000700: 016b 7211 0000 0063 0300 0000 0000 0000  .kr....c........
-00000710: 0000 0000 0400 0000 0300 0000 4300 0000  ............C...
-00000720: 7314 0000 0064 017c 007c 011b 007c 0213  s....d.|.|...|..
-00000730: 0014 007d 037c 0353 0029 0261 8b01 0000  ...}.|.S.).a....
-00000740: 5468 6520 4761 7564 696e 2d53 6368 7568  The Gaudin-Schuh
-00000750: 6d61 6e6e 2065 7175 6174 696f 6e0a 0a20  mann equation.. 
-00000760: 2020 2054 6865 2047 6175 6469 6e2d 5363     The Gaudin-Sc
-00000770: 6875 686d 616e 6e20 6571 7561 7469 6f6e  huhmann equation
-00000780: 2075 7365 6420 746f 2064 6574 6572 6d69   used to determi
-00000790: 6e65 2074 6865 2073 697a 6520 6469 7374  ne the size dist
-000007a0: 7269 6275 7469 6f6e 2069 7320 6173 2066  ribution is as f
-000007b0: 6f6c 6c6f 7773 3a0a 0a20 2020 206d 7020  ollows:..    mp 
-000007c0: 3d20 3130 3020 2a20 2864 2f6b 292a 2a6d  = 100 * (d/k)**m
-000007d0: 0a0a 2020 2020 7768 6572 653a 0a20 2020  ..    where:.   
-000007e0: 206d 7020 3d20 6d61 7373 2066 7261 6374   mp = mass fract
-000007f0: 696f 6e20 7061 7373 696e 6720 2825 290a  ion passing (%).
-00000800: 2020 2020 6b20 3d20 7369 7a65 206d 6f64      k = size mod
-00000810: 756c 7573 202d 2073 697a 6520 7768 656e  ulus - size when
-00000820: 2057 7020 3d20 3130 300a 2020 2020 6d20   Wp = 100.    m 
-00000830: 3d20 6469 7374 7269 6275 7469 6f6e 206d  = distribution m
-00000840: 6f64 756c 7573 203d 2073 6c6f 7065 206f  odulus = slope o
-00000850: 6620 7468 6520 6c6f 672d 6c6f 6720 706c  f the log-log pl
-00000860: 6f74 2057 7020 7673 2078 0a0a 2020 2020  ot Wp vs x..    
-00000870: 5245 463a 2068 7474 7073 3a2f 2f68 656c  REF: https://hel
-00000880: 702e 7379 7363 6164 2e6e 6574 2f53 697a  p.syscad.net/Siz
-00000890: 655f 4469 7374 7269 6275 7469 6f6e 5f44  e_Distribution_D
-000008a0: 6566 696e 6974 696f 6e23 526f 7369 6e2d  efinition#Rosin-
-000008b0: 5261 6d6d 6c65 720a 0a20 2020 2052 6574  Rammler..    Ret
-000008c0: 7572 6e73 3a0a 0a20 2020 2072 0700 0000  urns:..    r....
-000008d0: 720d 0000 0029 0472 0400 0000 721a 0000  r....).r....r...
-000008e0: 0072 1100 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000008f0: 720d 0000 0072 0e00 0000 da10 6761 7564  r....r......gaud
-00000900: 696e 5f73 6368 7568 6d61 6e6e 3b00 0000  in_schuhmann;...
-00000910: 7304 0000 0000 1410 0172 1b00 0000 6700  s........r....g.
-00000920: 0000 0000 0024 4029 0372 0400 0000 7210  .....$@).r....r.
-00000930: 0000 0072 1100 0000 6303 0000 0000 0000  ...r....c.......
-00000940: 0000 0000 0005 0000 0007 0000 0043 0000  .............C..
-00000950: 0073 4600 0000 6401 7c02 1400 6402 1800  .sF...d.|...d...
-00000960: 7d03 6403 6403 7400 a001 7c03 a101 6404  }.d.d.t...|...d.
-00000970: 1800 7400 a001 7c03 7c00 1400 7c01 1b00  ..t...|.|...|...
-00000980: a101 7400 a001 7c03 a101 1700 6405 1800  ..t...|.....d...
-00000990: 1b00 1400 1800 7d04 7c04 5300 2906 6167  ......}.|.S.).ag
-000009a0: 0100 0054 6865 204c 796e 6368 2065 7175  ...The Lynch equ
-000009b0: 6174 696f 6e0a 0a20 2020 2054 6865 204c  ation..    The L
-000009c0: 796e 6368 2065 7175 6174 696f 6e20 7573  ynch equation us
-000009d0: 6564 2074 6f20 6465 7465 726d 696e 6520  ed to determine 
-000009e0: 7468 6520 7369 7a65 2064 6973 7472 6962  the size distrib
-000009f0: 7574 696f 6e20 6973 2061 7320 666f 6c6c  ution is as foll
-00000a00: 6f77 733a 0a0a 2020 2020 6d70 203d 2031  ows:..    mp = 1
-00000a10: 3030 202d 2028 3130 3020 2a20 2864 2f6b  00 - (100 * (d/k
-00000a20: 292a 2a6d 290a 0a20 2020 2077 6865 7265  )**m)..    where
-00000a30: 3a0a 2020 2020 6d70 203d 206d 6173 7320  :.    mp = mass 
-00000a40: 6672 6163 7469 6f6e 2070 6173 7369 6e67  fraction passing
-00000a50: 2028 2529 0a20 2020 2064 3530 203d 2073   (%).    d50 = s
-00000a60: 697a 6520 6174 2077 6869 6368 2035 3025  ize at which 50%
-00000a70: 206f 6620 7061 7274 6963 6c65 7320 7265   of particles re
-00000a80: 7461 696e 6564 2062 7920 6d61 7373 0a20  tained by mass. 
-00000a90: 2020 206d 203d 2073 6861 7270 6e65 7373     m = sharpness
-00000aa0: 2063 6f6e 7374 616e 740a 0a20 2020 2052   constant..    R
-00000ab0: 4546 3a20 6874 7470 733a 2f2f 6865 6c70  EF: https://help
-00000ac0: 2e73 7973 6361 642e 6e65 742f 5369 7a65  .syscad.net/Size
-00000ad0: 5f44 6973 7472 6962 7574 696f 6e5f 4465  _Distribution_De
-00000ae0: 6669 6e69 7469 6f6e 2352 6f73 696e 2d52  finition#Rosin-R
-00000af0: 616d 6d6c 6572 0a0a 2020 2020 5265 7475  ammler..    Retu
-00000b00: 726e 733a 0a0a 2020 2020 67a4 703d 0ad7  rns:..    g.p=..
-00000b10: a3f8 3f67 14ae 47e1 7a14 de3f 7207 0000  ..?g..G.z..?r...
-00000b20: 0072 0800 0000 e902 0000 0072 0900 0000  .r.........r....
-00000b30: 2905 7204 0000 0072 1000 0000 7211 0000  ).r....r....r...
-00000b40: 00da 0561 6c70 6861 720c 0000 0072 0d00  ...alphar....r..
-00000b50: 0000 720d 0000 0072 0e00 0000 da05 6c79  ..r....r......ly
-00000b60: 6e63 6853 0000 0073 0600 0000 0014 0c01  nchS...s........
-00000b70: 3601 721e 0000 0029 0eda 0674 7970 696e  6.r....)...typin
-00000b80: 6772 0200 0000 da05 6e75 6d70 7972 0a00  gr......numpyr..
-00000b90: 0000 da06 7061 6e64 6173 7217 0000 00da  ....pandasr.....
-00000ba0: 0561 7272 6179 da07 6e64 6172 7261 79da  .array..ndarray.
-00000bb0: 0566 6c6f 6174 720f 0000 0072 1800 0000  .floatr....r....
-00000bc0: 7219 0000 0072 1b00 0000 721e 0000 0072  r....r....r....r
-00000bd0: 0d00 0000 720d 0000 0072 0d00 0000 720e  ....r....r....r.
-00000be0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000bf0: 0073 3c00 0000 0c02 0801 0803 0c01 0201  .s<.............
-00000c00: 02fe 0a01 0201 02fe 0c19 0c01 0201 02fe  ................
-00000c10: 1401 0201 14fe 0c1b 0c01 0201 02fe 0a01  ................
-00000c20: 0201 02fe 0c18 0c01 0201 02fe 0a01 0201  ................
-00000c30: 02fe                                     ..
+00000020: 0005 0000 0040 0000 0073 b400 0000 6400  .....@...s....d.
+00000030: 6401 6c00 5a01 6501 a002 6700 6402 a201  d.l.Z.e...g.d...
+00000040: a101 6403 6404 6603 6501 6a03 6504 1900  ..d.d.f.e.j.e...
+00000050: 6504 6504 6405 9c03 6406 6407 8405 5a05  e.e.d...d.d...Z.
+00000060: 6501 a002 6700 6402 a201 a101 6403 6404  e...g.d.....d.d.
+00000070: 6603 6501 6a03 6504 1900 6504 6504 6408  f.e.j.e...e.e.d.
+00000080: 9c03 6409 640a 8405 5a06 6501 a002 6700  ..d.d...Z.e...g.
+00000090: 6402 a201 a101 640b 640c 6603 6501 6a03  d.....d.d.f.e.j.
+000000a0: 6504 1900 6504 6504 640d 9c03 640e 640f  e...e.e.d...d.d.
+000000b0: 8405 5a07 6501 a002 6700 6402 a201 a101  ..Z.e...g.d.....
+000000c0: 6410 6404 6603 6501 6a03 6504 1900 6504  d.d.f.e.j.e...e.
+000000d0: 6504 6408 9c03 6411 6412 8405 5a08 6401  e.d...d.d...Z.d.
+000000e0: 5300 2913 e900 0000 004e 2905 6766 6666  S.)......N).gfff
+000000f0: 6666 e64a 4067 cdcc cccc cc0c 4340 6733  ff.J@g......C@g3
+00000100: 3333 3333 b33a 4067 cdcc cccc cccc 3240  3333.:@g......2@
+00000110: 679a 9999 9999 992a 40e9 0a00 0000 67b8  g......*@.....g.
+00000120: 1e85 eb51 b8f6 3f29 03da 0164 da01 61da  ...Q..?)...d..a.
+00000130: 0162 6303 0000 0000 0000 0000 0000 0004  .bc.............
+00000140: 0000 0006 0000 0043 0000 0073 2000 0000  .......C...s ...
+00000150: 6401 6402 7400 a001 7c00 7c01 1b00 7c02  d.d.t...|.|...|.
+00000160: 1300 0b00 a101 1800 1400 7d03 7c03 5300  ..........}.|.S.
+00000170: 2903 61ba 0100 0054 6865 2052 6f73 696e  ).a....The Rosin
+00000180: 2d52 616d 6d6c 6572 2065 7175 6174 696f  -Rammler equatio
+00000190: 6e0a 0a20 2020 2054 6865 2052 6f73 696e  n..    The Rosin
+000001a0: 2d52 616d 6d6c 6572 2065 7175 6174 696f  -Rammler equatio
+000001b0: 6e20 7573 6564 2074 6f20 6465 7465 726d  n used to determ
+000001c0: 696e 6520 7468 6520 7369 7a65 2064 6973  ine the size dis
+000001d0: 7472 6962 7574 696f 6e20 6973 2061 7320  tribution is as 
+000001e0: 666f 6c6c 6f77 733a 0a0a 2020 2020 6d70  follows:..    mp
+000001f0: 203d 2031 3030 202a 2028 3120 2d20 6578   = 100 * (1 - ex
+00000200: 7020 2a20 282d 2864 2f61 292a 2a62 2929  p * (-(d/a)**b))
+00000210: 0a0a 2020 2020 7768 6572 653a 0a20 2020  ..    where:.   
+00000220: 206d 7020 3d20 6d61 7373 2066 7261 6374   mp = mass fract
+00000230: 696f 6e20 7061 7373 696e 6720 2825 290a  ion passing (%).
+00000240: 2020 2020 6420 3d20 7061 7274 6963 6c65      d = particle
+00000250: 2064 6961 6d65 7465 720a 2020 2020 6120   diameter.    a 
+00000260: 3d20 7369 7a65 2061 7420 7768 6963 6820  = size at which 
+00000270: 2831 3030 2f65 2920 3d20 3336 2e38 2520  (100/e) = 36.8% 
+00000280: 6f66 2070 6172 7469 636c 6573 2072 6574  of particles ret
+00000290: 6169 6e65 640a 2020 2020 6220 3d20 636f  ained.    b = co
+000002a0: 6e73 7461 6e74 203d 2073 6c6f 7065 206f  nstant = slope o
+000002b0: 6620 7468 6520 706c 6f74 206f 6620 6c6e  f the plot of ln
+000002c0: 2831 3030 2f77 7029 2076 7320 6c6e 2078  (100/wp) vs ln x
+000002d0: 0a0a 2020 2020 5245 463a 2068 7474 7073  ..    REF: https
+000002e0: 3a2f 2f68 656c 702e 7379 7363 6164 2e6e  ://help.syscad.n
+000002f0: 6574 2f53 697a 655f 4469 7374 7269 6275  et/Size_Distribu
+00000300: 7469 6f6e 5f44 6566 696e 6974 696f 6e23  tion_Definition#
+00000310: 526f 7369 6e2d 5261 6d6d 6c65 720a 0a20  Rosin-Rammler.. 
+00000320: 2020 2052 6574 7572 6e73 3a0a 0a20 2020     Returns:..   
+00000330: 20e9 6400 0000 e901 0000 00a9 02da 026e   .d............n
+00000340: 70da 0365 7870 2904 7203 0000 0072 0400  p..exp).r....r..
+00000350: 0000 7205 0000 00da 026d 70a9 0072 0c00  ..r......mp..r..
+00000360: 0000 fa50 433a 5c70 726f 6a65 6374 735c  ...PC:\projects\
+00000370: 6d61 7373 2d63 6f6d 706f 7369 7469 6f6e  mass-composition
+00000380: 5c65 6c70 6869 636b 5c6d 6173 735f 636f  \elphick\mass_co
+00000390: 6d70 6f73 6974 696f 6e5c 7574 696c 735c  mposition\utils\
+000003a0: 7369 7a65 5f64 6973 7472 6962 7574 696f  size_distributio
+000003b0: 6e2e 7079 da0d 726f 7369 6e5f 7261 6d6d  n.py..rosin_ramm
+000003c0: 6c65 7204 0000 0073 0400 0000 0015 1c01  ler....s........
+000003d0: 720e 0000 0029 0372 0300 0000 da03 6435  r....).r......d5
+000003e0: 30da 016d 6303 0000 0000 0000 0000 0000  0..mc...........
+000003f0: 0004 0000 0007 0000 0043 0000 0073 2200  .........C...s".
+00000400: 0000 6401 6402 7400 a001 6403 7c00 7c01  ..d.d.t...d.|.|.
+00000410: 1b00 7c02 1300 1400 a101 1800 1400 7d03  ..|...........}.
+00000420: 7c03 5300 2904 61ac 0100 0054 6865 204d  |.S.).a....The M
+00000430: 6f64 6966 6965 6420 526f 7369 6e2d 5261  odified Rosin-Ra
+00000440: 6d6d 6c65 7220 6571 7561 7469 6f6e 0a0a  mmler equation..
+00000450: 2020 2020 5468 6520 526f 7369 6e2d 5261      The Rosin-Ra
+00000460: 6d6d 6c65 7220 6571 7561 7469 6f6e 2075  mmler equation u
+00000470: 7365 6420 746f 2064 6574 6572 6d69 6e65  sed to determine
+00000480: 2074 6865 2073 697a 6520 6469 7374 7269   the size distri
+00000490: 6275 7469 6f6e 2069 7320 6173 2066 6f6c  bution is as fol
+000004a0: 6c6f 7773 3a0a 0a20 2020 206d 7020 3d20  lows:..    mp = 
+000004b0: 3130 3020 2a20 2831 202d 2065 7870 202a  100 * (1 - exp *
+000004c0: 2028 2d2d 302e 3639 3331 3437 2864 2f64   (--0.693147(d/d
+000004d0: 3530 292a 2a6d 2929 0a0a 2020 2020 7768  50)**m))..    wh
+000004e0: 6572 653a 0a20 2020 206d 7020 3d20 6d61  ere:.    mp = ma
+000004f0: 7373 2066 7261 6374 696f 6e20 7061 7373  ss fraction pass
+00000500: 696e 6720 2825 290a 2020 2020 6420 3d20  ing (%).    d = 
+00000510: 7061 7274 6963 6c65 2064 6961 6d65 7465  particle diamete
+00000520: 720a 2020 2020 6435 3020 3d20 7369 7a65  r.    d50 = size
+00000530: 2061 7420 7768 6963 6820 3530 2520 6f66   at which 50% of
+00000540: 2070 6172 7469 636c 6573 2072 6574 6169   particles retai
+00000550: 6e65 6420 6279 206d 6173 730a 2020 2020  ned by mass.    
+00000560: 6d20 3d20 7368 6172 706e 6573 7320 636f  m = sharpness co
+00000570: 6e73 7461 6e74 0a0a 2020 2020 5245 463a  nstant..    REF:
+00000580: 2068 7474 7073 3a2f 2f68 656c 702e 7379   https://help.sy
+00000590: 7363 6164 2e6e 6574 2f53 697a 655f 4469  scad.net/Size_Di
+000005a0: 7374 7269 6275 7469 6f6e 5f44 6566 696e  stribution_Defin
+000005b0: 6974 696f 6e23 526f 7369 6e2d 5261 6d6d  ition#Rosin-Ramm
+000005c0: 6c65 720a 0a20 2020 2052 6574 7572 6e73  ler..    Returns
+000005d0: 3a0a 0a20 2020 2072 0600 0000 7207 0000  :..    r....r...
+000005e0: 0067 a241 0a9e 422e e6bf 7208 0000 0029  .g.A..B...r....)
+000005f0: 0472 0300 0000 720f 0000 0072 1000 0000  .r....r....r....
+00000600: 720b 0000 0072 0c00 0000 720c 0000 0072  r....r....r....r
+00000610: 0d00 0000 da16 6d6f 6469 6669 6564 5f72  ......modified_r
+00000620: 6f73 696e 5f72 616d 6d6c 6572 1d00 0000  osin_rammler....
+00000630: 7304 0000 0000 151e 0172 1100 0000 695e  s........r....i^
+00000640: 0100 0067 b81e 85eb 51b8 e63f 2903 7203  ...g....Q..?).r.
+00000650: 0000 00da 016b 7210 0000 0063 0300 0000  .....kr....c....
+00000660: 0000 0000 0000 0000 0400 0000 0300 0000  ................
+00000670: 4300 0000 7314 0000 0064 017c 007c 011b  C...s....d.|.|..
+00000680: 007c 0213 0014 007d 037c 0353 0029 0261  .|.....}.|.S.).a
+00000690: 8b01 0000 5468 6520 4761 7564 696e 2d53  ....The Gaudin-S
+000006a0: 6368 7568 6d61 6e6e 2065 7175 6174 696f  chuhmann equatio
+000006b0: 6e0a 0a20 2020 2054 6865 2047 6175 6469  n..    The Gaudi
+000006c0: 6e2d 5363 6875 686d 616e 6e20 6571 7561  n-Schuhmann equa
+000006d0: 7469 6f6e 2075 7365 6420 746f 2064 6574  tion used to det
+000006e0: 6572 6d69 6e65 2074 6865 2073 697a 6520  ermine the size 
+000006f0: 6469 7374 7269 6275 7469 6f6e 2069 7320  distribution is 
+00000700: 6173 2066 6f6c 6c6f 7773 3a0a 0a20 2020  as follows:..   
+00000710: 206d 7020 3d20 3130 3020 2a20 2864 2f6b   mp = 100 * (d/k
+00000720: 292a 2a6d 0a0a 2020 2020 7768 6572 653a  )**m..    where:
+00000730: 0a20 2020 206d 7020 3d20 6d61 7373 2066  .    mp = mass f
+00000740: 7261 6374 696f 6e20 7061 7373 696e 6720  raction passing 
+00000750: 2825 290a 2020 2020 6b20 3d20 7369 7a65  (%).    k = size
+00000760: 206d 6f64 756c 7573 202d 2073 697a 6520   modulus - size 
+00000770: 7768 656e 2057 7020 3d20 3130 300a 2020  when Wp = 100.  
+00000780: 2020 6d20 3d20 6469 7374 7269 6275 7469    m = distributi
+00000790: 6f6e 206d 6f64 756c 7573 203d 2073 6c6f  on modulus = slo
+000007a0: 7065 206f 6620 7468 6520 6c6f 672d 6c6f  pe of the log-lo
+000007b0: 6720 706c 6f74 2057 7020 7673 2078 0a0a  g plot Wp vs x..
+000007c0: 2020 2020 5245 463a 2068 7474 7073 3a2f      REF: https:/
+000007d0: 2f68 656c 702e 7379 7363 6164 2e6e 6574  /help.syscad.net
+000007e0: 2f53 697a 655f 4469 7374 7269 6275 7469  /Size_Distributi
+000007f0: 6f6e 5f44 6566 696e 6974 696f 6e23 526f  on_Definition#Ro
+00000800: 7369 6e2d 5261 6d6d 6c65 720a 0a20 2020  sin-Rammler..   
+00000810: 2052 6574 7572 6e73 3a0a 0a20 2020 2072   Returns:..    r
+00000820: 0600 0000 720c 0000 0029 0472 0300 0000  ....r....).r....
+00000830: 7212 0000 0072 1000 0000 720b 0000 0072  r....r....r....r
+00000840: 0c00 0000 720c 0000 0072 0d00 0000 da10  ....r....r......
+00000850: 6761 7564 696e 5f73 6368 7568 6d61 6e6e  gaudin_schuhmann
+00000860: 3600 0000 7304 0000 0000 1410 0172 1300  6...s........r..
+00000870: 0000 6700 0000 0000 0024 4063 0300 0000  ..g......$@c....
+00000880: 0000 0000 0000 0000 0500 0000 0700 0000  ................
+00000890: 4300 0000 7346 0000 0064 017c 0214 0064  C...sF...d.|...d
+000008a0: 0218 007d 0364 0364 0374 00a0 017c 03a1  ...}.d.d.t...|..
+000008b0: 0164 0418 0074 00a0 017c 037c 0014 007c  .d...t...|.|...|
+000008c0: 011b 00a1 0174 00a0 017c 03a1 0117 0064  .....t...|.....d
+000008d0: 0518 001b 0014 0018 007d 047c 0453 0029  .........}.|.S.)
+000008e0: 0661 6701 0000 5468 6520 4c79 6e63 6820  .ag...The Lynch 
+000008f0: 6571 7561 7469 6f6e 0a0a 2020 2020 5468  equation..    Th
+00000900: 6520 4c79 6e63 6820 6571 7561 7469 6f6e  e Lynch equation
+00000910: 2075 7365 6420 746f 2064 6574 6572 6d69   used to determi
+00000920: 6e65 2074 6865 2073 697a 6520 6469 7374  ne the size dist
+00000930: 7269 6275 7469 6f6e 2069 7320 6173 2066  ribution is as f
+00000940: 6f6c 6c6f 7773 3a0a 0a20 2020 206d 7020  ollows:..    mp 
+00000950: 3d20 3130 3020 2d20 2831 3030 202a 2028  = 100 - (100 * (
+00000960: 642f 6b29 2a2a 6d29 0a0a 2020 2020 7768  d/k)**m)..    wh
+00000970: 6572 653a 0a20 2020 206d 7020 3d20 6d61  ere:.    mp = ma
+00000980: 7373 2066 7261 6374 696f 6e20 7061 7373  ss fraction pass
+00000990: 696e 6720 2825 290a 2020 2020 6435 3020  ing (%).    d50 
+000009a0: 3d20 7369 7a65 2061 7420 7768 6963 6820  = size at which 
+000009b0: 3530 2520 6f66 2070 6172 7469 636c 6573  50% of particles
+000009c0: 2072 6574 6169 6e65 6420 6279 206d 6173   retained by mas
+000009d0: 730a 2020 2020 6d20 3d20 7368 6172 706e  s.    m = sharpn
+000009e0: 6573 7320 636f 6e73 7461 6e74 0a0a 2020  ess constant..  
+000009f0: 2020 5245 463a 2068 7474 7073 3a2f 2f68    REF: https://h
+00000a00: 656c 702e 7379 7363 6164 2e6e 6574 2f53  elp.syscad.net/S
+00000a10: 697a 655f 4469 7374 7269 6275 7469 6f6e  ize_Distribution
+00000a20: 5f44 6566 696e 6974 696f 6e23 526f 7369  _Definition#Rosi
+00000a30: 6e2d 5261 6d6d 6c65 720a 0a20 2020 2052  n-Rammler..    R
+00000a40: 6574 7572 6e73 3a0a 0a20 2020 2067 a470  eturns:..    g.p
+00000a50: 3d0a d7a3 f83f 6714 ae47 e17a 14de 3f72  =....?g..G.z..?r
+00000a60: 0600 0000 7207 0000 00e9 0200 0000 7208  ....r.........r.
+00000a70: 0000 0029 0572 0300 0000 720f 0000 0072  ...).r....r....r
+00000a80: 1000 0000 da05 616c 7068 6172 0b00 0000  ......alphar....
+00000a90: 720c 0000 0072 0c00 0000 720d 0000 00da  r....r....r.....
+00000aa0: 056c 796e 6368 4e00 0000 7306 0000 0000  .lynchN...s.....
+00000ab0: 140c 0136 0172 1600 0000 2909 da05 6e75  ...6.r....)...nu
+00000ac0: 6d70 7972 0900 0000 da05 6172 7261 79da  mpyr......array.
+00000ad0: 076e 6461 7272 6179 da05 666c 6f61 7472  .ndarray..floatr
+00000ae0: 0e00 0000 7211 0000 0072 1300 0000 7216  ....r....r....r.
+00000af0: 0000 0072 0c00 0000 720c 0000 0072 0c00  ...r....r....r..
+00000b00: 0000 720d 0000 00da 083c 6d6f 6475 6c65  ..r......<module
+00000b10: 3e01 0000 0073 3800 0000 0803 0c01 0201  >....s8.........
+00000b20: 02fe 0a01 0201 02fe 0c19 0c01 0201 02fe  ................
+00000b30: 0a01 0201 02fe 0c19 0c01 0201 02fe 0a01  ................
+00000b40: 0201 02fe 0c18 0c01 0201 02fe 0a01 0201  ................
+00000b50: 02fe                                     ..
```

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc` & `mass_composition-0.1.9/elphick/mass_composition/utils/__pycache__/viz.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/components.py` & `mass_composition-0.1.9/elphick/mass_composition/utils/components.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/moisture.py` & `mass_composition-0.1.9/elphick/mass_composition/utils/moisture.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/partition.py` & `mass_composition-0.1.9/elphick/mass_composition/utils/partition.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/size.py` & `mass_composition-0.1.9/elphick/mass_composition/utils/size.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 
 def mean_size(size_intervals: IntervalArray) -> np.ndarray:
     """Geometric mean size
 
     Size calculations are performed using the geometric mean, not the arithmetic mean
 
-    NOTE: If geometric mean is used for the pan fraction (0.0mm retained) it will return zero, which is and
+    NOTE: If geometric mean is used for the pan fraction (0.0mm retained) it will return zero, which is an
     edge size not mean size.  So the mean ratio of the geometric mean to the arithmetic mean for all other
-     fractions is used for the bottom fraction.
+    fractions is used for the bottom fraction.
 
 
     Args:
         size_intervals: A pandas IntervalArray
 
     Returns:
```

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/size_distribution.py` & `mass_composition-0.1.9/elphick/mass_composition/utils/size_distribution.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.1.8/elphick/mass_composition/utils/viz.py` & `mass_composition-0.1.9/elphick/mass_composition/utils/viz.py`

 * *Files identical despite different names*

### Comparing `mass_composition-0.1.8/LICENSE` & `mass_composition-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mass_composition-0.1.8/pyproject.toml` & `mass_composition-0.1.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 [tool.poetry]
 name = "mass-composition"
-version = "0.1.8"
+version = "0.1.9"
 description = "For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation."
 authors = ["Greg <greg@elphick.com.au>"]
 packages = [{ include = "elphick/mass_composition" }]
 
+#[[tool.poetry.source]]
+#name = "pypi_"
+#url = "https://pypi.org/mass-composition"
+#priority = "primary"
+
 [[tool.poetry.source]]
-name = "pypi_"
-url = "https://pypi.org/mass-composition"
-secondary = false
-
-#[tool.semantic_release]
-#version_variable = "pyproject.toml:version"
-#version_source = "tag"
+name = "PyPI"
+priority = "primary"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 xarray = "^2022.6.0"
 periodictable = "^1.6.1"
 pyyaml = "^6.0"
 scipy = "^1.9.0"
 pyvista = { version = "^0.37.0", optional = true }
 pyvista-xarray = { version = "^0.1.2", optional = true }
 matplotlib = { version = "^3.6.2", optional = true }
 plotly = { version = "^5.13.0", optional = true }
 kaleido = { version = "0.2.1", optional = true }
 seaborn = { version = "^0.12.2", optional = true }
 networkx = { version = "^3.0", optional = true }
+omfvista = {version = "^0.2.5", optional = true}
 
 [tool.poetry.extras]
 viz = ["matplotlib", "seaborn", "plotly", "kaleido", "pyvista", "pyvista-xarray"]
 network = ["networkx"]
+omf = ["omfvista"]
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^7.0.5"
 notebook = "^6.5.2"
 pytest = "^7.1.3"
 Sphinx = "^5.0.2"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-gallery = "^0.11.1"
 sphinx-autodoc-typehints = "^1.18.3"
 myst-parser = "^0.18.0"
 orca = "^1.8"  # for plotly thumbnails in docs
 #python-semantic-release = "^7.33.2"
 #ydata-profiling = "^4.1.1"
+#setuptools = "^67.8.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mass_composition-0.1.8/PKG-INFO` & `mass_composition-0.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: mass-composition
-Version: 0.1.8
+Version: 0.1.9
 Summary: For managing multi-dimensional mass-composition datasets, supporting weighted mathematical operations and visualisation.
 Author: Greg
 Author-email: greg@elphick.com.au
 Requires-Python: >=3.8,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: network
+Provides-Extra: omf
 Provides-Extra: viz
-Requires-Dist: kaleido (==0.2.1); extra == "viz"
-Requires-Dist: matplotlib (>=3.6.2,<4.0.0); extra == "viz"
-Requires-Dist: networkx (>=3.0,<4.0); extra == "network"
+Requires-Dist: kaleido (==0.2.1) ; extra == "viz"
+Requires-Dist: matplotlib (>=3.6.2,<4.0.0) ; extra == "viz"
+Requires-Dist: networkx (>=3.0,<4.0) ; extra == "network"
+Requires-Dist: omfvista (>=0.2.5,<0.3.0) ; extra == "omf"
 Requires-Dist: periodictable (>=1.6.1,<2.0.0)
-Requires-Dist: plotly (>=5.13.0,<6.0.0); extra == "viz"
-Requires-Dist: pyvista (>=0.37.0,<0.38.0); extra == "viz"
-Requires-Dist: pyvista-xarray (>=0.1.2,<0.2.0); extra == "viz"
+Requires-Dist: plotly (>=5.13.0,<6.0.0) ; extra == "viz"
+Requires-Dist: pyvista (>=0.37.0,<0.38.0) ; extra == "viz"
+Requires-Dist: pyvista-xarray (>=0.1.2,<0.2.0) ; extra == "viz"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
-Requires-Dist: seaborn (>=0.12.2,<0.13.0); extra == "viz"
+Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "viz"
 Requires-Dist: xarray (>=2022.6.0,<2023.0.0)
```

