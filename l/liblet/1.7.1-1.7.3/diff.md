# Comparing `tmp/liblet-1.7.1.tar.gz` & `tmp/liblet-1.7.3.tar.gz`

## Comparing `liblet-1.7.1.tar` & `liblet-1.7.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/api.rst
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/conf.py
--rw-r--r--   0        0        0   133561 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples.ipynb
--rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples.rst
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/index.rst
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/installation.rst
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/stg.svg
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/tree.svg
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/_static/custom.css
--rw-r--r--   0        0        0   710126 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/_static/logo.png
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/_templates/project.html
--rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples_files/examples_70_0.svg
--rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples_files/examples_71_0.svg
--rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples_files/examples_82_0.svg
--rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples_files/examples_83_0.svg
--rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 liblet-1.7.1/docs/examples_files/examples_8_0.svg
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liblet-1.7.1/src/scripts.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/__init__.py
--rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/antlr.py
--rw-r--r--   0        0        0    11718 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/automaton.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/const.py
--rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/decorators.py
--rw-r--r--   0        0        0    20296 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/display.py
--rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/grammar.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/llvm.py
--rw-r--r--   0        0        0     9757 2020-02-02 00:00:00.000000 liblet-1.7.1/src/liblet/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/__init__.py
--rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/antlr_test.py
--rw-r--r--   0        0        0    10107 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/automaton_test.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/decorators_test.py
--rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/grammar_test.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/run.py
--rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 liblet-1.7.1/src/tests/utils_test.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liblet-1.7.1/.gitignore
--rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 liblet-1.7.1/LICENSE-CC.txt
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 liblet-1.7.1/LICENSE-GPL.txt
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 liblet-1.7.1/README.md
--rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 liblet-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 liblet-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     8017 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/api.rst
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/conf.py
+-rw-r--r--   0        0        0   133561 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples.ipynb
+-rw-r--r--   0        0        0    57101 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples.rst
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/index.rst
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/installation.rst
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/stg.svg
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/tree.svg
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/_static/custom.css
+-rw-r--r--   0        0        0   710126 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/_static/logo.png
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/_templates/project.html
+-rw-r--r--   0        0        0    17662 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples_files/examples_70_0.svg
+-rw-r--r--   0        0        0    16784 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples_files/examples_71_0.svg
+-rw-r--r--   0        0        0    17775 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples_files/examples_82_0.svg
+-rw-r--r--   0        0        0    16940 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples_files/examples_83_0.svg
+-rw-r--r--   0        0        0    14143 2020-02-02 00:00:00.000000 liblet-1.7.3/docs/examples_files/examples_8_0.svg
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 liblet-1.7.3/src/scripts.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/__init__.py
+-rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/antlr.py
+-rw-r--r--   0        0        0    11772 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/automaton.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/const.py
+-rw-r--r--   0        0        0     3376 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/decorators.py
+-rw-r--r--   0        0        0    20499 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/display.py
+-rw-r--r--   0        0        0    21760 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/grammar.py
+-rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/llvm.py
+-rw-r--r--   0        0        0     9757 2020-02-02 00:00:00.000000 liblet-1.7.3/src/liblet/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/__init__.py
+-rw-r--r--   0        0        0     6878 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/antlr_test.py
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/automaton_test.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/decorators_test.py
+-rw-r--r--   0        0        0    12885 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/grammar_test.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/run.py
+-rw-r--r--   0        0        0     4271 2020-02-02 00:00:00.000000 liblet-1.7.3/src/tests/utils_test.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 liblet-1.7.3/.gitignore
+-rw-r--r--   0        0        0    20133 2020-02-02 00:00:00.000000 liblet-1.7.3/LICENSE-CC.txt
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 liblet-1.7.3/LICENSE-GPL.txt
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 liblet-1.7.3/README.md
+-rw-r--r--   0        0        0     2680 2020-02-02 00:00:00.000000 liblet-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 liblet-1.7.3/PKG-INFO
```

### Comparing `liblet-1.7.1/docs/api.rst` & `liblet-1.7.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/conf.py` & `liblet-1.7.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/examples.ipynb` & `liblet-1.7.3/docs/examples.ipynb`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/examples.rst` & `liblet-1.7.3/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/index.rst` & `liblet-1.7.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/installation.rst` & `liblet-1.7.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/stg.svg` & `liblet-1.7.3/docs/stg.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/tree.svg` & `liblet-1.7.3/docs/tree.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/_static/logo.png` & `liblet-1.7.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/_templates/project.html` & `liblet-1.7.3/docs/_templates/project.html`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/examples_files/examples_70_0.svg` & `liblet-1.7.3/docs/examples_files/examples_70_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/examples_files/examples_71_0.svg` & `liblet-1.7.3/docs/examples_files/examples_71_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/examples_files/examples_82_0.svg` & `liblet-1.7.3/docs/examples_files/examples_82_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/examples_files/examples_83_0.svg` & `liblet-1.7.3/docs/examples_files/examples_83_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/docs/examples_files/examples_8_0.svg` & `liblet-1.7.3/docs/examples_files/examples_8_0.svg`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/src/liblet/__init__.py` & `liblet-1.7.3/src/liblet/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.7.1'
+__version__ = '1.7.3'
 
 from liblet.antlr import ANTLR, AnnotatedTreeWalker
 from liblet.automaton import (
   Automaton,
   BottomUpInstantaneousDescription,
   InstantaneousDescription,
   TopDownInstantaneousDescription,
```

### Comparing `liblet-1.7.1/src/liblet/antlr.py` & `liblet-1.7.3/src/liblet/antlr.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/src/liblet/automaton.py` & `liblet-1.7.3/src/liblet/automaton.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,21 +234,22 @@
     c = type(self)(self.G)
     c.tape = self.tape
     c.stack = copy(self.stack)
     c.steps = self.steps
     c.head_pos = self.head_pos
     return c
 
+  def _stack_str_(self):
+    return ''.join(reversed(list(map(str, self.stack))))
+
+  def _tape_str_(self):
+    return ''.join(self.tape[: self.head_pos :] + ('｜',) + self.tape[self.head_pos :])  # noqa: RUF001
+
   def __repr__(self):
-    return '{}, {}, \x1b[48;5;252m{}\x1b[0m{}'.format(  # https://en.wikipedia.org/wiki/ANSI_escape_code
-      self.steps,
-      ''.join(reversed(list(map(str, self.stack)))),
-      ''.join(self.tape[: self.head_pos :]),
-      ''.join(self.tape[self.head_pos :]),
-    )
+    return f'{self.steps}, {self._stack_str_()}, {self._tape_str_()}'
 
   def head(self):
     """Returns the symbol under the tape head."""
     return self.tape[self.head_pos]
 
   def top(self):
     """Returns the symbol at the (root of the :class:`~liblet.display.Tree` at the) top of the stack."""
@@ -334,13 +335,15 @@
 
   def reduce(self, P):
     """Attempts a reduce move, given the specified production, and returns the corresponding new instantaneous description."""
     if P not in self.G.P:
       raise ValueError('The production does not belong to the grammar.')
     c = copy(self)
     children = [c.stack.pop() for _ in P.rhs][::-1]
-    for X, T in zip(P.rhs, children, strict=True):
-      if T.root != X:
-        raise ValueError('The rhs does not correspond to the symbols on the stack.')
+    if tuple(t.root for t in children) != P.rhs:
+      raise ValueError('The rhs does not correspond to the symbols on the stack.')
     c.stack.push(Tree(P.lhs, children))
     c.steps = (P, *c.steps)
     return c
+
+  def _stack_str_(self):
+    return ''.join(map(str, self.stack))
```

### Comparing `liblet-1.7.1/src/liblet/decorators.py` & `liblet-1.7.3/src/liblet/decorators.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/src/liblet/display.py` & `liblet-1.7.3/src/liblet/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections import OrderedDict
 from collections.abc import Mapping, Set  # noqa: PYI025
 from functools import partial
 from html import escape
 from itertools import chain, pairwise
 from operator import itemgetter
 from re import sub
+from textwrap import indent
 from warnings import warn as wwarn
 
 import svgutils.transform as svg_ttransform
 from graphviz import Digraph
 from IPython.display import HTML, SVG, display
 from ipywidgets import IntSlider, interactive
 
@@ -19,57 +20,57 @@
 from liblet.utils import AttrDict, CYKTable, compose, letstr
 
 
 def _escape(label):
   return sub(r'\]', '&#93;', sub(r'\[', '&#91;', escape(str(label))))
 
 
-def make_mapping_aware_str(
-  other_str=letstr,  # in mapping_aware_str, how to represent non-mapping objects
-  key_str=str,  # in mapping_aware_str, how to represent keys
-  value_str=_escape,  # in mapping_aware_str, how to represent values
-  key_filter=lambda k: not k.startswith('_thread_'),  # in mapping_aware_str, which keys to show
+def make_mapping_aware_label(
+  other_str=letstr,  # in mapping_aware_label, how to represent non-mapping objects
+  key_str=str,  # in mapping_aware_label, how to represent keys
+  value_str=_escape,  # in mapping_aware_label, how to represent values
+  key_filter=lambda k: not k.startswith('_thread_'),  # in mapping_aware_label, which keys to show
 ):
-  def mapping_aware_str(obj):
+  def mapping_aware_label(obj):
     if obj is None:
       return None
     if isinstance(obj, Mapping):
       return ''.join(
         ['<<FONT POINT-SIZE="12"><TABLE BORDER="0" CELLBORDER="1" CELLSPACING="0">']
         + [f'<TR><TD>{key_str(k)}</TD><TD>{value_str(obj[k])}</TD></TR>' for k in filter(key_filter, obj)]
         + ['</TABLE></FONT>>']
       )
     return other_str(obj)
 
-  return mapping_aware_str
+  return mapping_aware_label
 
 
 def mapping_aware_gv_args(obj):
   return {'shape': 'none', 'margin': '0'} if isinstance(obj, Mapping) else {'margin': '.05'}
 
 
 def make_node_wrapper(
   node_label=None,  # how to produce the node label from the node object
   node_eq='obj',  # how to decide equality between nodes
   default_gv_args=None,  # how to produce the default gv args from the node object
 ):
   if node_label is None:
-    node_label = make_mapping_aware_str()
+    node_label = make_mapping_aware_label()
   elif not callable(node_label):
     raise ValueError('node_label must be either None or a callable')
 
   if node_eq == 'obj':
     node_eq = lambda x, y: x == y
-  elif node_eq == 'str':
+  elif node_eq == 'label':
     node_eq = lambda x, y: node_label(x) == node_label(y)
   elif not callable(node_eq):
-    raise ValueError('node_eq must be either "obj", "str" or a callable')
+    raise ValueError('node_eq must be either "obj", "label" or a callable')
 
   if default_gv_args is None:
-    default_gv_args = lambda x: mapping_aware_gv_args(x)
+    default_gv_args = mapping_aware_gv_args
   elif not callable(default_gv_args):
     raise ValueError('default_gv_args must be either None or a callable')
 
   class NodeWrapper:
     def __init__(self, obj):
       self.obj = obj
 
@@ -120,21 +121,24 @@
     return self.G.subgraph(**args)
 
   def node(self, obj, G=None, gv_args=None):
     if G is None:
       G = self.G
     wn, new = self._obj2wn(obj)
     if new:
-      G.node(wn.gid(), wn.label(), **(wn.default_gv_args() | (gv_args or {})))
+      G.node(wn.gid(), wn.label(), **({'fontname': 'Fira Code'} | wn.default_gv_args() | (gv_args or {})))
     return wn.gid()
 
   def edge(self, objsrc, objdst, G=None, gv_args=None):
     if G is None:
       G = self.G
-    G.edge(self.node(objsrc), self.node(objdst), **(gv_args or {}))
+    G.edge(self.node(objsrc), self.node(objdst), **({'fontname': 'Fira Code'} | (gv_args or {})))
+
+  def __repr__(self):
+    return 'GVWrapper[\n' + indent(str(self.G), '\t') + ']'
 
   def _repr_svg_(self):
     return self.G._repr_image_svg_xml()
 
 
 class BaseGraph(ABC):
   def __init__(self):
@@ -253,21 +257,22 @@
     G = GVWrapper(
       dict(  # noqa: C408
         graph_attr={'nodesep': '.25', 'ranksep': '.25'},
         node_attr={'shape': 'box', 'width': '0', 'height': '0', 'style': 'rounded, setlinewidth(.25)'},
         edge_attr={'dir': 'none'},
       ),
       make_node_wrapper(
-        node_label=compose(make_mapping_aware_str(), itemgetter(0)),
+        node_label=compose(make_mapping_aware_label(), itemgetter(0)),
         default_gv_args=compose(mapping_aware_gv_args, itemgetter(0)),
       ),
     )
 
     def walk(T):
       curr = (T.root, T)
+      G.node(curr)
       for child in T.children:
         G.edge(curr, (child.root, child))
       if len(T.children) > 1:
         with G.subgraph(edge_attr={'style': 'invis'}, graph_attr={'rank': 'same'}) as S:
           for f, t in pairwise(T.children):
             G.edge((f.root, f), (t.root, t), S)
       for child in T.children:
@@ -318,15 +323,15 @@
     return G
 
 
 class Graph:
   def __init__(self, arcs, sep=None):
     self.G = GVWrapper(
       dict(graph_attr={'size': '8', 'rankdir': 'LR'}, node_attr={'shape': 'oval'}),  # noqa: C408
-      make_node_wrapper(node_label=make_mapping_aware_str(other_str=partial(letstr, sep=sep))),
+      make_node_wrapper(node_label=make_mapping_aware_label(other_str=partial(letstr, sep=sep))),
     )
     self.adj = {}
     for src, dst in arcs:
       self.adj[src] = self.adj.get(src, set()) | {dst}
       self.adj[dst] = self.adj.get(dst, set())
       self.G.edge(src, dst)
 
@@ -378,15 +383,15 @@
           'margin': '.05',
           'width': '0',
           'height': '0',
           'style': 'rounded, setlinewidth(.25)',
         },
         edge_attr={'dir': 'none', 'penwidth': '.5', 'arrowsize': '.5'},
       ),
-      make_node_wrapper(node_label=compose(make_mapping_aware_str(), itemgetter(0))),
+      make_node_wrapper(node_label=compose(make_mapping_aware_label(), itemgetter(0))),
     )
 
     def remove_ε(sentence):
       return tuple(_ for _ in sentence if _[0] != ε)
 
     sentence = ((derivation.start, 0, 0),)
     for step, (rule, pos) in enumerate(derivation.steps(), 1):
@@ -507,15 +512,15 @@
     G = GVWrapper(
       dict(  # noqa: C408
         graph_attr={'rankdir': 'LR', 'size': '32'},
         node_attr={'margin': '.05'} if self.large_labels else {},
         engine='dot',
       ),
       make_node_wrapper(
-        node_label=make_mapping_aware_str(other_str=partial(letstr, sep=sep)),
+        node_label=make_mapping_aware_label(other_str=partial(letstr, sep=sep)),
         default_gv_args=lambda X: {'peripheries': '2' if X in self.F else '1'},
       ),
     )
     if self.S is not None:
       (G.node('', gv_args={'shape': 'point'}),)
       G.edge('', self.S)
     for X, x, Y in self.transitions:
```

### Comparing `liblet-1.7.1/src/liblet/grammar.py` & `liblet-1.7.3/src/liblet/grammar.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/src/liblet/llvm.py` & `liblet-1.7.3/src/liblet/llvm.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/src/liblet/utils.py` & `liblet-1.7.3/src/liblet/utils.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/src/tests/antlr_test.py` & `liblet-1.7.3/src/tests/antlr_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/src/tests/automaton_test.py` & `liblet-1.7.3/src/tests/automaton_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,26 +203,26 @@
       """
       S -> a B C
       B -> a B | b
       C -> a
     """
     )
     i = TopDownInstantaneousDescription(G, 'aaba')
-    self.assertEqual('(), S♯, \x1b[48;5;252m\x1b[0maaba♯', str(i))
+    self.assertEqual('(), S♯, ｜aaba♯', str(i))
 
   def test_BUID_init(self):
     G = Grammar.from_string(
       """
       S -> A C
       A -> a b
       C -> c
     """
     )
     i = BottomUpInstantaneousDescription(G, 'abc')
-    self.assertEqual('(), , \x1b[48;5;252m\x1b[0mabc', str(i))
+    self.assertEqual('(), , ｜abc', str(i))
 
   def test_TDID_init_exception(self):
     G = Grammar.from_string('S -> ♯')
     with self.assertRaisesRegex(ValueError, r'.*♯.*belong to terminal'):
       TopDownInstantaneousDescription(G, 'aaba')
 
   def test_TDID_predict(self):
@@ -231,15 +231,15 @@
       S -> a B C
       B -> a B | b
       C -> a
     """
     )
     i = TopDownInstantaneousDescription(G, 'aaba')
     i = i.predict(G.P[0])
-    self.assertEqual('(S -> a\u200aB\u200aC,), aBC♯, \x1b[48;5;252m\x1b[0maaba♯', str(i))
+    self.assertEqual('(S -> a\u200aB\u200aC,), aBC♯, ｜aaba♯', str(i))
 
   def test_TDID_predict_exception0(self):
     G = Grammar.from_string(
       """
       S -> a B C
       B -> a B | b
       C -> a
@@ -267,15 +267,15 @@
       S -> A C
       A -> a b
       C -> c
     """
     )
     i = BottomUpInstantaneousDescription(G, 'abc')
     i = i.shift().shift().reduce(G.P[1])
-    self.assertEqual('(A -> a\u200ab,), (A: (a), (b)), \x1b[48;5;252mab\x1b[0mc', str(i))
+    self.assertEqual('(A -> a\u200ab,), (A: (a), (b)), ab｜c', str(i))
 
   def test_BUID_reduce_exception0(self):
     G = Grammar.from_string(
       """
       S -> A C
       A -> a b
       C -> c
@@ -303,15 +303,15 @@
       S -> a B C
       B -> a B | b
       C -> a
     """
     )
     i = TopDownInstantaneousDescription(G, 'aaba')
     i = i.predict(G.P[0]).match()
-    self.assertEqual('(S -> a\u200aB\u200aC,), BC♯, \x1b[48;5;252ma\x1b[0maba♯', str(i))
+    self.assertEqual('(S -> a\u200aB\u200aC,), BC♯, a｜aba♯', str(i))
 
   def test_TDID_match_exception(self):
     G = Grammar.from_string(
       """
       S -> a B C
       B -> a B | b
       C -> a
@@ -327,15 +327,15 @@
       S -> A C
       A -> a b
       C -> c
     """
     )
     i = BottomUpInstantaneousDescription(G, 'abc')
     i = i.shift()
-    self.assertEqual('(), (a), \x1b[48;5;252ma\x1b[0mbc', str(i))
+    self.assertEqual('(), (a), a｜bc', str(i))
 
   def test_TDID_done(self):
     G = Grammar.from_string(
       """
       S -> a B C
       B -> a B | b
       C -> a
```

### Comparing `liblet-1.7.1/src/tests/decorators_test.py` & `liblet-1.7.3/src/tests/decorators_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/src/tests/grammar_test.py` & `liblet-1.7.3/src/tests/grammar_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/src/tests/utils_test.py` & `liblet-1.7.3/src/tests/utils_test.py`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/LICENSE-CC.txt` & `liblet-1.7.3/LICENSE-CC.txt`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/LICENSE-GPL.txt` & `liblet-1.7.3/LICENSE-GPL.txt`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/README.md` & `liblet-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/pyproject.toml` & `liblet-1.7.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `liblet-1.7.1/PKG-INFO` & `liblet-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: liblet
-Version: 1.7.1
+Version: 1.7.3
 Summary: A teaching aid library for formal languages and compiler courses.
 Project-URL: Documentation, https://liblet.readthedocs.io/
 Project-URL: Source code, https://github.com/let-unimi/liblet
 Project-URL: Changelog, https://github.com/let-unimi/liblet/blob/master/CHANGELOG.txt
 Project-URL: Bug Tracker, https://github.com/let-unimi/liblet/issues
 Author-email: Massimo Santini <massimo.santini@unimi.it>
 License-File: LICENSE-CC.txt
```

