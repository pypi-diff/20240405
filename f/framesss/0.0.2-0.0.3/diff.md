# Comparing `tmp/framesss-0.0.2.tar.gz` & `tmp/framesss-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framesss-0.0.2.tar", max compression
+gzip compressed data, was "framesss-0.0.3.tar", max compression
```

## Comparing `framesss-0.0.2.tar` & `framesss-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1070 2024-02-15 11:42:49.815810 framesss-0.0.2/LICENSE
--rw-r--r--   0        0        0     1120 2024-02-15 11:42:49.815810 framesss-0.0.2/LICENSE.LESM
--rw-r--r--   0        0        0     3049 2024-02-15 11:42:49.815810 framesss-0.0.2/README.md
--rw-r--r--   0        0        0     4392 2024-02-15 11:42:59.851874 framesss-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       16 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/__init__.py
--rw-r--r--   0        0        0      207 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/__main__.py
--rw-r--r--   0        0        0     9938 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/enums.py
--rw-r--r--   0        0        0       16 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/__init__.py
--rw-r--r--   0        0        0       43 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/analysis/__init__.py
--rw-r--r--   0        0        0    19979 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/analysis/analysis.py
--rw-r--r--   0        0        0      305 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/analysis/frame_xyz_analysis.py
--rw-r--r--   0        0        0    24594 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/analysis/frame_xz_analysis.py
--rw-r--r--   0        0        0      300 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/analysis/grid_xy_analysis.py
--rw-r--r--   0        0        0      305 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/analysis/truss_xyz_analysis.py
--rw-r--r--   0        0        0      303 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/analysis/truss_xz_analysis.py
--rw-r--r--   0        0        0       46 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/boundary_conditions/__init__.py
--rw-r--r--   0        0        0    41007 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/boundary_conditions/element_load.py
--rw-r--r--   0        0        0      739 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/boundary_conditions/nodal_load.py
--rw-r--r--   0        0        0     1156 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/boundary_conditions/prescribed_displacement.py
--rw-r--r--   0        0        0    43385 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/element_1d.py
--rw-r--r--   0        0        0       33 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/models/__init__.py
--rw-r--r--   0        0        0      376 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/models/frame_xz.py
--rw-r--r--   0        0        0    12344 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/models/model.py
--rw-r--r--   0        0        0     9264 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/fea/node.py
--rw-r--r--   0        0        0       23 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/post/__init__.py
--rw-r--r--   0        0        0     2114 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/post/member_1d_results.py
--rw-r--r--   0        0        0     4606 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/post/node_results.py
--rw-r--r--   0        0        0       22 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/pre/__init__.py
--rw-r--r--   0        0        0     5182 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/pre/cases.py
--rw-r--r--   0        0        0     1682 2024-02-15 11:42:49.819810 framesss-0.0.2/src/framesss/pre/material.py
--rw-r--r--   0        0        0    29490 2024-02-15 11:42:49.823809 framesss-0.0.2/src/framesss/pre/member_1d.py
--rw-r--r--   0        0        0    20618 2024-02-15 11:42:49.823809 framesss-0.0.2/src/framesss/pre/member_load.py
--rw-r--r--   0        0        0     1786 2024-02-15 11:42:49.823809 framesss-0.0.2/src/framesss/pre/section.py
--rw-r--r--   0        0        0        0 2024-02-15 11:42:49.823809 framesss-0.0.2/src/framesss/py.typed
--rw-r--r--   0        0        0       15 2024-02-15 11:42:49.823809 framesss-0.0.2/src/framesss/solvers/__init__.py
--rw-r--r--   0        0        0     8646 2024-02-15 11:42:49.823809 framesss-0.0.2/src/framesss/solvers/linear_static.py
--rw-r--r--   0        0        0    12803 2024-02-15 11:42:49.823809 framesss-0.0.2/src/framesss/solvers/solver.py
--rw-r--r--   0        0        0     5174 2024-02-15 11:42:49.823809 framesss-0.0.2/src/framesss/utils.py
--rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 framesss-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-05 13:09:55.267582 framesss-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1120 2024-04-05 13:09:55.267582 framesss-0.0.3/LICENSE.LESM
+-rw-r--r--   0        0        0     3049 2024-04-05 13:09:55.267582 framesss-0.0.3/README.md
+-rw-r--r--   0        0        0     4392 2024-04-05 13:10:13.275652 framesss-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       16 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/__init__.py
+-rw-r--r--   0        0        0      207 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/__main__.py
+-rw-r--r--   0        0        0     9938 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/enums.py
+-rw-r--r--   0        0        0       16 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/analysis/__init__.py
+-rw-r--r--   0        0        0    19602 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/analysis/analysis.py
+-rw-r--r--   0        0        0      305 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/analysis/frame_xyz_analysis.py
+-rw-r--r--   0        0        0    25345 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/analysis/frame_xz_analysis.py
+-rw-r--r--   0        0        0      300 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/analysis/grid_xy_analysis.py
+-rw-r--r--   0        0        0      305 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/analysis/truss_xyz_analysis.py
+-rw-r--r--   0        0        0      303 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/analysis/truss_xz_analysis.py
+-rw-r--r--   0        0        0       46 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/boundary_conditions/__init__.py
+-rw-r--r--   0        0        0    42097 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/boundary_conditions/element_load.py
+-rw-r--r--   0        0        0      739 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/boundary_conditions/nodal_load.py
+-rw-r--r--   0        0        0     1156 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/boundary_conditions/prescribed_displacement.py
+-rw-r--r--   0        0        0    49467 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/element_1d.py
+-rw-r--r--   0        0        0       33 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/models/__init__.py
+-rw-r--r--   0        0        0      376 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/models/frame_xz.py
+-rw-r--r--   0        0        0    12870 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/models/model.py
+-rw-r--r--   0        0        0     9264 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/fea/node.py
+-rw-r--r--   0        0        0       23 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/post/__init__.py
+-rw-r--r--   0        0        0     2224 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/post/member_1d_results.py
+-rw-r--r--   0        0        0     4614 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/post/node_results.py
+-rw-r--r--   0        0        0       22 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/pre/__init__.py
+-rw-r--r--   0        0        0     6165 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/pre/cases.py
+-rw-r--r--   0        0        0     1682 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/pre/material.py
+-rw-r--r--   0        0        0    26757 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/pre/member_1d.py
+-rw-r--r--   0        0        0    18333 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/pre/member_load.py
+-rw-r--r--   0        0        0     5933 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/pre/section.py
+-rw-r--r--   0        0        0        0 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/py.typed
+-rw-r--r--   0        0        0       15 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/solvers/__init__.py
+-rw-r--r--   0        0        0     9479 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/solvers/linear_static.py
+-rw-r--r--   0        0        0    12451 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/solvers/solver.py
+-rw-r--r--   0        0        0     5174 2024-04-05 13:09:55.275582 framesss-0.0.3/src/framesss/utils.py
+-rw-r--r--   0        0        0     4015 1970-01-01 00:00:00.000000 framesss-0.0.3/PKG-INFO
```

### Comparing `framesss-0.0.2/LICENSE` & `framesss-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `framesss-0.0.2/LICENSE.LESM` & `framesss-0.0.3/LICENSE.LESM`

 * *Files identical despite different names*

### Comparing `framesss-0.0.2/README.md` & `framesss-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `framesss-0.0.2/pyproject.toml` & `framesss-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "framesss"
-version = "0.0.2"
+version = "0.0.3"
 description = "framesss"
 authors = ["Daniel Beranek <daniel.beraanek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/DanBeranek/framesss"
 repository = "https://github.com/DanBeranek/framesss"
 documentation = "https://DanBeranek.github.io/framesss"
```

### Comparing `framesss-0.0.2/src/framesss/enums.py` & `framesss-0.0.3/src/framesss/enums.py`

 * *Files identical despite different names*

### Comparing `framesss-0.0.2/src/framesss/fea/analysis/analysis.py` & `framesss-0.0.3/src/framesss/fea/analysis/analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 
     from framesss.enums import AnalysisModelType
     from framesss.enums import DoF
     from framesss.fea.boundary_conditions.element_load import ElementLoad
     from framesss.fea.element_1d import Element1D
     from framesss.fea.models.model import Model
     from framesss.fea.node import Node
+    from framesss.pre.cases import EnvelopeCombination
     from framesss.pre.cases import LoadCase
-    from framesss.pre.cases import LoadCombination
+    from framesss.pre.cases import LoadCaseCombination
     from framesss.pre.member_1d import Member1D
 
 
 class Analysis(ABC):
     """
     Abstract base class for defining a finite element analysis (FEA).
 
@@ -203,46 +204,39 @@
         :param element: A reference to an instance of the :class:`Element1D` class.
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         :return: Displacements from loads at the element sampling points.
         """
         pass
 
     @abstractmethod
-    def save_internal_stresses_on_member(
-        self, member: Member1D, load_case: LoadCase
+    def save_internal_stresses(
+        self, member: Member1D, case: LoadCase | LoadCaseCombination
     ) -> None:
         """
         Compute and save the internal stresses.
 
         Internal stresses are: axial forces, shear forces, and bending moments,
         for a member under a specified load case. This includes both detailed distributions
         along the member and extreme values for each stress component.
 
         This method aggregates internal stress data from each :class:`Element1D` of the :class:`Member1D`.
         :param member: A reference to an instance of the :class:`Member1D` class.
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
         """
         pass
 
     @abstractmethod
-    def save_internal_stresses_on_member_combination(
-        self, member: Member1D, load_combination: LoadCombination
+    def save_envelope_stresses(
+        self, member: Member1D, envelope: EnvelopeCombination
     ) -> None:
         """
-        Compute and save internal stresses.
-
-        Computes and saves the internal stresses (axial forces, shear forces, and bending moments)
-        for a member under a specified load case. This includes both detailed distributions
-        along the member and extreme values for each stress component.
-
-        This method aggregates internal stress data from each :class:`Element1D` of the :class:`Member1D`,
-        including axial forces, shear forces in the Z direction, and bending moments about the Y axis.
+        Compute and save the envelope of internal stresses.
 
         :param member: A reference to an instance of the :class:`Member1D` class.
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param envelope: A reference to an instance of the :class:`EnvelopeCombination`.
         """
         pass
 
     @abstractmethod
     def save_internal_displacements_on_member(
         self, member: Member1D, load_case: LoadCase
     ) -> None:
@@ -254,23 +248,23 @@
         :param member: A reference to an instance of the :class:`Member1D` class.
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         """
         pass
 
     @abstractmethod
     def save_internal_displacements_on_member_combination(
-        self, member: Member1D, load_combination: LoadCombination
+        self, member: Member1D, load_combination: LoadCaseCombination
     ) -> None:
         """
         Compute and save the internal displacements for a member under a specified load case.
 
         This method aggregates displacement data from each :class:`Element1D` of the :class:`Member1D`,
 
         :param member: A reference to an instance of the :class:`Member1D` class.
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
         """
         pass
 
     @abstractmethod
     def save_reactions(self, node: Node, load_case: LoadCase) -> None:
         """
         Save the reaction forces and moments for a specified node under a given load case.
@@ -287,24 +281,24 @@
         is None), this method will not attempt to save reactions in that direction.
         """
         pass
 
     # TODO: docstring
     @abstractmethod
     def save_reactions_combination(
-        self, node: Node, load_combination: LoadCombination
+        self, node: Node, load_combination: LoadCaseCombination
     ) -> None:
         """
         Save the reaction forces and moments for a specified node under a given load combination.
 
         This method extracts reaction forces and moments from the global force vector for the specified
         :class:`LoadCase` and assigns them to the corresponding node results.
 
         :param node: A reference to an instance of the :class:`Node` class.
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
 
         Note that the method operates directly on the `node.results` attribute, updating it with
         the calculated reactions for the specified load case. If `node.fixity` for a particular
         direction is not `SupportFixity.FIXED_DOF` (i.e. reaction storage for a particular direction
         is None), this method will not attempt to save reactions in that direction.
         """
         pass
@@ -321,24 +315,24 @@
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         """
         pass
 
     # TODO: docstring
     @abstractmethod
     def save_displacements_combination(
-        self, node: Node, load_combination: LoadCombination
+        self, node: Node, load_combination: LoadCaseCombination
     ) -> None:
         """
         Save the displacements for a specified node under a given load combination.
 
         This method extracts displacements from the global displacement vector for the
         specified :class:`LoadCase` and assigns them to the corresponding node results.
 
         :param node: A reference to an instance of the :class:`Node` class.
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
         """
 
     def setup_dof_numbers(self, model: Model) -> None:
         """
         Initialize the global DoF numbering matrix and counts the total number of equations.
 
         The `dof_connectivity_matrix` matrix is used to track the status of each DoF for every node in the model:
```

### Comparing `framesss-0.0.2/src/framesss/fea/analysis/frame_xz_analysis.py` & `framesss-0.0.3/src/framesss/fea/analysis/frame_xz_analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 
 import numpy as np
 import scipy as sp  # type: ignore[import-untyped]
 
 from framesss.enums import AnalysisModelType
 from framesss.enums import DoF
 from framesss.fea.analysis.analysis import Analysis
+from framesss.pre.cases import EnvelopeCombination
+from framesss.pre.cases import LoadCase
 from framesss.utils import assemble_subarray_at_indices
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
     from framesss.fea.boundary_conditions.element_load import ElementLoad
     from framesss.fea.element_1d import Element1D
     from framesss.fea.models.model import Model
     from framesss.fea.node import Node
-    from framesss.pre.cases import LoadCase
-    from framesss.pre.cases import LoadCombination
+    from framesss.pre.cases import LoadCaseCombination
     from framesss.pre.member_1d import Member1D
 
 
 class FrameXZAnalysis(Analysis):
     """
     Subclass of the :class:`Analysis` class for the implementation of the 2D Frame model in XZ-plane.
 
@@ -179,19 +180,19 @@
         """
         Assembles contribution of an internal force vector for a given element and load case.
 
         :param element: A reference to an instance of the :class:`Element1D` class.
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         :param fel: The internal force vector in local system for the element.
         """
-        element.axial_force[load_case] = fel[[0, 3]]
+        element.end_axial_forces[load_case] = fel[[0, 3]]
 
-        element.bending_moment_y[load_case] = fel[[1, 4]]
+        element.end_bending_moments_y[load_case] = fel[[1, 4]]
 
-        element.shear_force_z[load_case] = fel[[2, 5]]
+        element.end_shear_forces_z[load_case] = fel[[2, 5]]
 
     def get_displacement_shape_function_matrix(
         self, element: Element1D
     ) -> npt.NDArray[np.float64]:
         """
         Return displacement shape function matrix evaluated at sampling points of the element.
 
@@ -276,130 +277,170 @@
             )
             displacements[1, :] += thermla_load.get_flexural_xz_displacements(
                 element.sampling_points
             )
 
         return displacements
 
-    def save_internal_stresses_on_member(
-        self, member: Member1D, load_case: LoadCase
+    def save_internal_stresses(
+        self, member: Member1D, case: LoadCase | LoadCaseCombination
     ) -> None:
         """
         Compute and save internal stresses.
 
         Computes and saves the internal stresses (axial forces, shear forces, and bending moments)
         for a member under a specified load case. This includes both detailed distributions
         along the member and extreme values for each stress component.
 
         This method aggregates internal stress data from each :class:`Element1D` of the :class:`Member1D`,
         including axial forces, shear forces in the Z direction, and bending moments about the Y axis.
 
         :param member: A reference to an instance of the :class:`Member1D` class.
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
         """
+        # Save equation coefficients
+
+        if isinstance(case, LoadCase):
+            for element in member.generated_elements:
+                element.save_axial_equation_coefficients_for_load_case(case)
+                element.save_shear_force_xz_equation_coefficients_for_load_case(case)
+                element.save_bending_moment_xz_equation_coefficients_for_load_case(case)
+        else:
+            for element in member.generated_elements:
+                element.save_axial_equation_coefficients_for_load_combination(case)
+                element.save_shear_force_xz_equation_coefficients_for_load_combination(
+                    case
+                )
+                element.save_bending_moment_xz_equation_coefficients_for_load_combination(
+                    case
+                )
+
+        for element in member.generated_elements:
+            element.save_peak_points_for_axial_force_eqn(case)
+            element.save_peak_points_for_shear_force_xz_eqn(case)
+            element.save_peak_points_for_bending_moment_xz_eqn(case)
+
         # Initialize empty arrays
         axial_forces = np.array([])
         shear_forces_z = np.array([])
         bending_moments_y = np.array([])
 
-        extreme_axial_forces = np.empty((0, 2))
-        extreme_shear_forces_z = np.empty((0, 2))
-        extreme_bending_moments_y = np.empty((0, 2))
+        peak_x_local = np.array([])
+        peak_axial_forces = np.array([])
+        peak_shear_forces_z = np.array([])
+        peak_bending_moments_y = np.array([])
 
         # Loop through every element
         for element in member.generated_elements:
             x = element.sampling_points
+            x_peaks = element.peak_points[case]
+
+            peak_x_local = np.append(peak_x_local, x_peaks + element.x_start)
 
             # Get axial forces
-            axial_forces = np.append(
-                axial_forces, element.get_internal_axial_forces(load_case, x)
-            )
-            extreme_axial_forces = np.append(
-                extreme_axial_forces,
-                element.get_max_internal_axial_forces(load_case),
-                axis=0,
+            axial_forces = np.append(axial_forces, element.get_axial_force(case, x))
+            peak_axial_forces = np.append(
+                peak_axial_forces, element.get_axial_force(case, x_peaks)
             )
 
             # Get shear forces
             shear_forces_z = np.append(
-                shear_forces_z, element.get_internal_shear_forces_xz(load_case, x)
+                shear_forces_z, element.get_shear_force_xz(case, x)
             )
-            extreme_shear_forces_z = np.append(
-                extreme_shear_forces_z,
-                element.get_max_internal_shear_forces_xz(load_case),
-                axis=0,
+            peak_shear_forces_z = np.append(
+                peak_shear_forces_z, element.get_shear_force_xz(case, x_peaks)
             )
 
             # Get bending moments
             bending_moments_y = np.append(
-                bending_moments_y, element.get_internal_bending_moments_xz(load_case, x)
+                bending_moments_y, element.get_bending_moment_xz(case, x)
             )
-            extreme_bending_moments_y = np.append(
-                extreme_bending_moments_y,
-                element.get_max_internal_bending_moments_xz(load_case),
-                axis=0,
+            peak_bending_moments_y = np.append(
+                peak_bending_moments_y, element.get_bending_moment_xz(case, x_peaks)
             )
 
         # Save results
-        member.results.axial_forces[load_case] = axial_forces
-        member.results.extreme_axial_forces[load_case] = extreme_axial_forces
+        # Stack arrays and get only unique records for peak values
+        data = np.vstack(
+            [
+                peak_x_local,
+                peak_axial_forces,
+                peak_shear_forces_z,
+                peak_bending_moments_y,
+            ]
+        )
+        peak_x_local, peak_axial_forces, peak_shear_forces_z, peak_bending_moments_y = (
+            np.unique(data, axis=1)
+        )
+
+        member.results.peak_x_local[case] = peak_x_local
+
+        member.results.axial_forces[case] = axial_forces
+        member.results.peak_axial_forces[case] = peak_axial_forces
         min_max_axial_forces = np.array(
-            [np.min(extreme_axial_forces[:, 1]), np.max(extreme_axial_forces[:, 1])]
+            [np.min(peak_axial_forces), np.max(peak_axial_forces)]
         )
-        member.results.min_max_axial_forces[load_case] = min_max_axial_forces
+        member.results.min_max_axial_forces[case] = min_max_axial_forces
 
-        member.results.shear_forces_z[load_case] = shear_forces_z
-        member.results.extreme_shear_forces_z[load_case] = extreme_shear_forces_z
+        member.results.shear_forces_z[case] = shear_forces_z
+        member.results.peak_shear_forces_z[case] = peak_shear_forces_z
         min_max_shear_forces_z = np.array(
-            [np.min(extreme_shear_forces_z[:, 1]), np.max(extreme_shear_forces_z[:, 1])]
+            [np.min(peak_shear_forces_z), np.max(peak_shear_forces_z)]
         )
-        member.results.min_max_shear_forces_z[load_case] = min_max_shear_forces_z
+        member.results.min_max_shear_forces_z[case] = min_max_shear_forces_z
 
-        member.results.bending_moments_y[load_case] = bending_moments_y
-        member.results.extreme_bending_moments_y[load_case] = extreme_bending_moments_y
+        member.results.bending_moments_y[case] = bending_moments_y
+        member.results.peak_bending_moments_y[case] = peak_bending_moments_y
         min_max_bending_moments_y = np.array(
             [
-                np.min(extreme_bending_moments_y[:, 1]),
-                np.max(extreme_bending_moments_y[:, 1]),
+                np.min(peak_bending_moments_y),
+                np.max(peak_bending_moments_y),
             ]
         )
-        member.results.min_max_bending_moments_y[load_case] = min_max_bending_moments_y
+        member.results.min_max_bending_moments_y[case] = min_max_bending_moments_y
 
-    def save_internal_stresses_on_member_combination(
-        self, member: Member1D, load_combination: LoadCombination
+    def save_envelope_stresses(
+        self, member: Member1D, envelope: EnvelopeCombination
     ) -> None:
         """
-        Compute and save internal stresses.
-
-        Computes and saves the internal stresses (axial forces, shear forces, and bending moments)
-        for a member under a specified load case. This includes both detailed distributions
-        along the member and extreme values for each stress component.
-
-        This method aggregates internal stress data from each :class:`Element1D` of the :class:`Member1D`,
-        including axial forces, shear forces in the Z direction, and bending moments about the Y axis.
+        Filter and save the envelope of internal stresses.
 
         :param member: A reference to an instance of the :class:`Member1D` class.
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param envelope: A reference to an instance of the :class:`EnvelopeCombination`.
         """
-        member.results.axial_forces[load_combination] = np.zeros(member.x_local.shape)
-        member.results.shear_forces_z[load_combination] = np.zeros(member.x_local.shape)
-        member.results.bending_moments_y[load_combination] = np.zeros(
-            member.x_local.shape
+        axial_forces = np.vstack(
+            [member.results.axial_forces[case] for case in envelope.cases]
+        )
+        shear_forces_z = np.vstack(
+            [member.results.shear_forces_z[case] for case in envelope.cases]
+        )
+        bending_moments_y = np.vstack(
+            [member.results.bending_moments_y[case] for case in envelope.cases]
         )
 
-        for load_case, factor in load_combination.combinations.items():
-            member.results.axial_forces[load_combination] += (
-                factor * member.results.axial_forces[load_case]
-            )
-            member.results.shear_forces_z[load_combination] += (
-                factor * member.results.shear_forces_z[load_case]
-            )
-            member.results.bending_moments_y[load_combination] += (
-                factor * member.results.bending_moments_y[load_case]
-            )
+        member.results.axial_forces[envelope] = np.array(
+            [
+                np.min(axial_forces, axis=0),
+                np.max(axial_forces, axis=0),
+            ]
+        )
+
+        member.results.shear_forces_z[envelope] = np.array(
+            [
+                np.min(shear_forces_z, axis=0),
+                np.max(shear_forces_z, axis=0),
+            ]
+        )
+
+        member.results.bending_moments_y[envelope] = np.array(
+            [
+                np.min(bending_moments_y, axis=0),
+                np.max(bending_moments_y, axis=0),
+            ]
+        )
 
     def save_internal_displacements_on_member(
         self, member: Member1D, load_case: LoadCase
     ) -> None:
         """
         Compute and save the internal displacements for a member under a specified load case.
 
@@ -425,28 +466,28 @@
             translations_x = np.append(translations_x, u_local[0, :])
             translations_z = np.append(translations_z, u_local[1, :])
 
         member.results.translations_x[load_case] = translations_x
         member.results.translations_z[load_case] = translations_z
 
     def save_internal_displacements_on_member_combination(
-        self, member: Member1D, load_combination: LoadCombination
+        self, member: Member1D, load_combination: LoadCaseCombination
     ) -> None:
         """
         Compute and save the internal displacements for a member under a specified load case.
 
         This method aggregates displacement data from each :class:`Element1D` of the :class:`Member1D`,
 
         :param member: A reference to an instance of the :class:`Member1D` class.
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
         """
         member.results.translations_x[load_combination] = np.zeros(member.x_local.shape)
         member.results.translations_z[load_combination] = np.zeros(member.x_local.shape)
 
-        for load_case, factor in load_combination.combinations.items():
+        for load_case, factor in load_combination.load_cases.items():
             member.results.translations_x[load_combination] += (
                 factor * member.results.translations_x[load_case]
             )
             member.results.translations_z[load_combination] += (
                 factor * member.results.translations_z[load_case]
             )
 
@@ -471,60 +512,51 @@
         if (rmy := node.results.reaction_moment_y) is not None:
             rmy[load_case] = load_case.f_global[node.global_dofs[1]]
 
         if (rfz := node.results.reaction_force_z) is not None:
             rfz[load_case] = load_case.f_global[node.global_dofs[2]]
 
     def save_reactions_combination(
-        self, node: Node, load_combination: LoadCombination
+        self, node: Node, load_combination: LoadCaseCombination
     ) -> None:
         """
         Save the reaction forces and moments for a specified node under a given load combination.
 
         This method extracts reaction forces and moments from the global force vector for the specified
         :class:`LoadCase` and assigns them to the corresponding node results.
 
         :param node: A reference to an instance of the :class:`Node` class.
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
 
         Note that the method operates directly on the `node.results` attribute, updating it with
         the calculated reactions for the specified load case. If `node.fixity` for a particular
         direction is not `SupportFixity.FIXED_DOF` (i.e. reaction storage for a particular direction
         is None), this method will not attempt to save reactions in that direction.
         """
-        for load_case, factor in load_combination.combinations.items():
-            if node.results.reaction_force_x.get(load_case):
-                if node.results.reaction_force_x.get(load_combination):
-                    node.results.reaction_force_x[load_combination] += (
-                        factor * load_case.f_global[node.global_dofs[0]]
-                    )
-                else:
-                    node.results.reaction_force_x[load_combination] = (
-                        factor * load_case.f_global[node.global_dofs[0]]
-                    )
-
-            if node.results.reaction_moment_y.get(load_case):
-                if node.results.reaction_moment_y.get(load_combination):
-                    node.results.reaction_moment_y[load_combination] += (
-                        factor * load_case.f_global[node.global_dofs[1]]
-                    )
-                else:
-                    node.results.reaction_moment_y[load_combination] = (
-                        factor * load_case.f_global[node.global_dofs[1]]
-                    )
-
-            if node.results.reaction_force_z.get(load_case):
-                if node.results.reaction_force_z.get(load_combination):
-                    node.results.reaction_force_z[load_combination] += (
-                        factor * load_case.f_global[node.global_dofs[2]]
-                    )
-                else:
-                    node.results.reaction_force_z[load_combination] = (
-                        factor * load_case.f_global[node.global_dofs[2]]
-                    )
+        for load_case, factor in load_combination.load_cases.items():
+            if node.results.reaction_force_x.get(load_case) is not None:
+                if node.results.reaction_force_x.get(load_combination) is None:
+                    node.results.reaction_force_x[load_combination] = 0
+                node.results.reaction_force_x[load_combination] += (
+                    factor * load_case.f_global[node.global_dofs[0]]
+                )
+
+            if node.results.reaction_moment_y.get(load_case) is not None:
+                if node.results.reaction_moment_y.get(load_combination) is None:
+                    node.results.reaction_moment_y[load_combination] = 0
+                node.results.reaction_moment_y[load_combination] += (
+                    factor * load_case.f_global[node.global_dofs[1]]
+                )
+
+            if node.results.reaction_force_z.get(load_case) is not None:
+                if node.results.reaction_force_z.get(load_combination) is None:
+                    node.results.reaction_force_z[load_combination] = 0
+                node.results.reaction_force_z[load_combination] += (
+                    factor * load_case.f_global[node.global_dofs[2]]
+                )
 
     def save_displacements(self, node: Node, load_case: LoadCase) -> None:
         """
         Save the displacements for a specified node under a given load case.
 
         This method extracts displacements from the global displacement vector for the
         specified :class:`LoadCase` and assigns them to the corresponding node results.
@@ -536,28 +568,28 @@
 
         node.results.translation_x[load_case] = u_g[0]
         node.results.rotation_y[load_case] = u_g[1]
         node.results.translation_z[load_case] = u_g[2]
 
     # TODO: docstring
     def save_displacements_combination(
-        self, node: Node, load_combination: LoadCombination
+        self, node: Node, load_combination: LoadCaseCombination
     ) -> None:
         """
         Save the displacements for a specified node under a given load combination.
 
         This method extracts displacements from the global displacement vector for the
         specified :class:`LoadCase` and assigns them to the corresponding node results.
 
         :param node: A reference to an instance of the :class:`Node` class.
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
         """
         node.results.translation_x[load_combination] = 0.0
         node.results.rotation_y[load_combination] = 0.0
         node.results.translation_z[load_combination] = 0.0
 
-        for load_case, factor in load_combination.combinations.items():
+        for load_case, factor in load_combination.load_cases.items():
             u_g = load_case.u_global[node.global_dofs]
 
             node.results.translation_x[load_combination] += factor * u_g[0]
             node.results.rotation_y[load_combination] += factor * u_g[1]
             node.results.translation_z[load_combination] += factor * u_g[2]
```

### Comparing `framesss-0.0.2/src/framesss/fea/boundary_conditions/element_load.py` & `framesss-0.0.3/src/framesss/fea/boundary_conditions/element_load.py`

 * *Files 4% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         return (
             f"{self.__class__.__name__}(element={element_repr}, "
             f"components_local=[{components_str}])"
         )
 
     def get_axial_fixed_end_forces(self) -> npt.NDArray[np.float64]:
         """
-        Return axial fixed end force vector..
+        Return axial fixed end force vector.
 
         The forces are calculated and returned in the local coordinate system of the element.
 
         :return: A 1x2 array representing the axial fixed end forces at the start and end nodes.
         """
         # Initialize axial load values at end nodes
         fx_start = self.components_local[0]
@@ -165,20 +165,22 @@
             L2 = L**2
 
             # Timoshenko parameter
             if self.element.member.element_type == Element1DType.NAVIER:
                 Omega = 0.0
 
             elif self.element.member.element_type == Element1DType.TIMOSHENKO:
-                E = self.element.member.material.elastic_modulus
-                G = self.element.member.material.shear_modulus
-                As = self.element.member.section.area_y
-                I = self.element.member.section.inertia_z
+                EI = self.element.member.section.EIz
+                GA = self.element.member.section.GAy
 
-                Omega = E * I / (G * As * L2)
+                Omega = EI / (GA * L2)
+            else:
+                raise AttributeError(
+                    f"Wrong element type: {self.element.member.element_type}"
+                )
 
             # Auxiliary parameters
             mu = 1 + 12 * Omega
             lamb = 1 + 3 * Omega
             zeta = 1 + 40 * Omega / 3
             xi = 1 + 5 * Omega
             eta = 1 + 15 * Omega
@@ -258,14 +260,19 @@
                         -(fy_uniform * L / 2 + fy_linear * L / 6),
                         0,
                         -(fy_uniform * L / 2 + fy_linear * L / 3),
                         0,
                     ]
                 )
 
+            else:
+                raise AttributeError(
+                    f"Wrong hinge type: {self.element.hinge_start}, {self.element.hinge_end}"
+                )
+
         else:
             fef_flex = np.zeros([4])
 
         return fef_flex
 
     def get_flexural_xz_fixed_end_forces(self) -> npt.NDArray[np.float64]:
         """Return flexural fixed end force vector in local xz-plane.
@@ -283,20 +290,18 @@
             L2 = L**2
 
             # Timoshenko parameter
             if self.element.member.element_type == Element1DType.NAVIER:
                 Omega = 0.0
 
             elif self.element.member.element_type == Element1DType.TIMOSHENKO:
-                E = self.element.member.material.elastic_modulus
-                G = self.element.member.material.shear_modulus
-                As = self.element.member.section.area_z
-                I = self.element.member.section.inertia_y
+                EI = self.element.member.section.EIy
+                GA = self.element.member.section.GAz
 
-                Omega = E * I / (G * As * L2)
+                Omega = EI / (GA * L2)
 
             else:
                 raise ValueError(
                     f"Unknown member type: {self.element.member.element_type}."
                 )
 
             # Auxiliary parameters
@@ -379,14 +384,19 @@
                         -(fz_uniform * L / 2 + fz_linear * L / 6),
                         0,
                         -(fz_uniform * L / 2 + fz_linear * L / 3),
                         0,
                     ]
                 )
 
+            else:
+                raise AttributeError(
+                    f"Wrong hinge type: {self.element.hinge_start}, {self.element.hinge_end}"
+                )
+
         else:
             fef_flex = np.zeros([4])
 
         return fef_flex
 
     def get_axial_displacements(
         self, x: npt.NDArray[np.float64]
@@ -400,20 +410,17 @@
         """
         # Initialize axial load values at end nodes
         fx_start = self.components_local[0]
         fx_end = self.components_local[3]
 
         # Check if transversal load is not null over member
         if fx_start or fx_end:
-            E = self.element.member.material.elastic_modulus
-            A = self.element.member.section.area_x
+            EA = self.element.member.section.EA
             L = self.element.length
 
-            EA = E * A
-
             # Separate uniform portion from linear partition of axial load
             fx_uniform = fx_start
             fx_linear = fx_end - fx_start
 
             # Calculate axial displacements from uniform and from linear axial load portion
             u_uniform = fx_uniform / EA * (L * x / 2 - x**2 / 2)
             u_linear = fx_linear / EA * (L * x / 6 - x**3 / (6 * L))
@@ -438,31 +445,33 @@
         # Initialize transversal load value at end nodes
         fy_start = self.components_local[1]
         fy_end = self.components_local[4]
 
         # Check if transversal load is not null over the member
         if fy_start or fy_end:
             # Basic member properties
-            E = self.element.member.material.elastic_modulus
-            I = self.element.member.section.inertia_z
+            EI = self.element.member.section.EIz
             L = self.element.length
 
-            EI = E * I
             L2 = L * L
             L3 = L2 * L
 
             # Timoshenko parameter
             if self.element.member.element_type == Element1DType.NAVIER:
                 Omega = 0.0
 
             elif self.element.member.element_type == Element1DType.TIMOSHENKO:
-                G = self.element.member.material.shear_modulus
-                As = self.element.member.section.area_y
+                GA = self.element.member.section.GAy
+
+                Omega = EI / (GA * L2)
 
-                Omega = EI / (G * As * L2)
+            else:
+                raise AttributeError(
+                    f"Wrong element type: {self.element.member.element_type}"
+                )
 
             # Auxiliary parameters
             mu = 1 + 12 * Omega
             lamb = 1 + 3 * Omega
             zeta = 1 + 40 * Omega / 3
             xi = 1 + 5 * Omega
             eta = 1 + 15 * Omega
@@ -570,14 +579,19 @@
                     * (
                         (7 * L3 / 360 + L3 * Omega / 6) * x
                         - (L / 36 + L * Omega / 6) * x**3
                         + x**5 / (120 * L)
                     )
                 )
 
+            else:
+                raise AttributeError(
+                    f"Wrong hinge type: {self.element.hinge_start}, {self.element.hinge_end}"
+                )
+
             v = v_uniform + v_linear
 
         else:
             v = np.zeros(x.shape)
 
         return v  # type: ignore[no-any-return]
 
@@ -594,31 +608,33 @@
         # Initialize transversal load value at end nodes
         fz_start = self.components_local[2]
         fz_end = self.components_local[5]
 
         # Check if transversal load is not null over the member
         if fz_start or fz_end:
             # Basic member properties
-            E = self.element.member.material.elastic_modulus
-            I = self.element.member.section.inertia_y
+            EI = self.element.member.section.EIy
             L = self.element.length
 
-            EI = E * I
             L2 = L * L
             L3 = L2 * L
 
             # Timoshenko parameter
             if self.element.member.element_type == Element1DType.NAVIER:
                 Omega = 0.0
 
             elif self.element.member.element_type == Element1DType.TIMOSHENKO:
-                G = self.element.member.material.shear_modulus
-                As = self.element.member.section.area_z
+                GA = self.element.member.section.GAz
+
+                Omega = EI / (GA * L2)
 
-                Omega = EI / (G * As * L2)
+            else:
+                raise AttributeError(
+                    f"Wrong element type: {self.element.member.element_type}"
+                )
 
             # Auxiliary parameters
             mu = 1 + 12 * Omega
             lamb = 1 + 3 * Omega
             zeta = 1 + 40 * Omega / 3
             xi = 1 + 5 * Omega
             eta = 1 + 15 * Omega
@@ -726,14 +742,19 @@
                     * (
                         (7 * L3 / 360 + L3 * Omega / 6) * x
                         - (L / 36 + L * Omega / 6) * x**3
                         + x**5 / (120 * L)
                     )
                 )
 
+            else:
+                raise AttributeError(
+                    f"Wrong hinge type: {self.element.hinge_start}, {self.element.hinge_end}"
+                )
+
             w = w_uniform + w_linear
 
         else:
             w = np.zeros(x.shape)
 
         return w  # type: ignore[no-any-return]
 
@@ -772,23 +793,22 @@
 
         :return: A 1x2 array representing the axial fixed end forces at the start and end nodes.
         """
         # Get temperature variation on member center of gravity
         dtx = self.temperature_gradients[0]
 
         if dtx:
-            E = self.element.member.material.elastic_modulus
-            alpha = self.element.member.material.thermal_expansion_coefficient
-            A = self.element.member.section.area_x
+            EA = self.element.member.section.EA
+            alpha = self.element.member.section.material.thermal_expansion_coefficient
 
             # Calculate fixed end forces
             fef_axial = np.array(
                 [
-                    E * A * alpha * dtx,
-                    -E * A * alpha * dtx,
+                    EA * alpha * dtx,
+                    -EA * alpha * dtx,
                 ]
             )
 
         else:
             return np.zeros(2)
 
         return fef_axial
@@ -800,30 +820,32 @@
         :return: A 4x1 array representing the flexural fixed end forces at the start and end nodes.
         """
         # Get temperature gradient relative to member local y-axis
         dty = self.temperature_gradients[1]
 
         if dty:
             # Basic member properties
-            E = self.element.member.material.elastic_modulus
-            alpha = self.element.member.material.thermal_expansion_coefficient
-            I = self.element.member.section.inertia_z
+            alpha = self.element.member.section.material.thermal_expansion_coefficient
             h = self.element.member.section.height_y
             L = self.element.length
-            EI = E * I
+            EI = self.element.member.section.EIz
 
             # Timoshenko parameter
             if self.element.member.element_type == Element1DType.NAVIER:
                 Omega = 0.0
 
             elif self.element.member.element_type == Element1DType.TIMOSHENKO:
-                G = self.element.member.material.shear_modulus
-                As = self.element.member.section.area_y
+                GA = self.element.member.section.GAy
 
-                Omega = E * I / (G * As * L * L)
+                Omega = EI / (GA * L * L)
+
+            else:
+                raise AttributeError(
+                    f"Wrong element type: {self.element.member.element_type}"
+                )
 
             # Auxiliary parameter
             lamb = 1 + 3 * Omega
 
             # Compute unitary dimensionless temperature gradient
             tg = (alpha * dty) / h
 
@@ -862,14 +884,19 @@
 
             elif (
                 self.element.hinge_start == BeamConnection.HINGED_END
                 and self.element.hinge_end == BeamConnection.HINGED_END
             ):
                 fef_flex = np.zeros(4)
 
+            else:
+                raise AttributeError(
+                    f"Wrong hinge type: {self.element.hinge_start}, {self.element.hinge_end}"
+                )
+
         else:
             fef_flex = np.zeros(4)
 
         return fef_flex
 
     def get_flexural_xz_fixed_end_forces(self) -> npt.NDArray[np.float64]:
         """
@@ -878,30 +905,33 @@
         :return: A 4x1 array representing the flexural fixed end forces at the start and end nodes.
         """
         # Get temperature gradient relative to member local y-axis
         dtz = self.temperature_gradients[2]
 
         if dtz:
             # Basic member properties
-            E = self.element.member.material.elastic_modulus
-            alpha = self.element.member.material.thermal_expansion_coefficient
-            I = self.element.member.section.inertia_y
+            alpha = self.element.member.section.material.thermal_expansion_coefficient
             h = self.element.member.section.height_z
             L = self.element.length
-            EI = E * I
+            EI = self.element.member.section.EIy
 
             # Timoshenko parameter
             if self.element.member.element_type == Element1DType.NAVIER:
                 Omega = 0.0
 
             elif self.element.member.element_type == Element1DType.TIMOSHENKO:
-                G = self.element.member.material.shear_modulus
-                As = self.element.member.section.area_z
 
-                Omega = E * I / (G * As * L * L)
+                GA = self.element.member.section.GAz
+
+                Omega = EI / (GA * L * L)
+
+            else:
+                raise AttributeError(
+                    f"Wrong element type: {self.element.member.element_type}"
+                )
 
             # Auxiliary parameter
             lamb = 1 + 3 * Omega
 
             # Compute unitary dimensionless temperature gradient
             tg = (alpha * dtz) / h
 
@@ -940,14 +970,19 @@
 
             elif (
                 self.element.hinge_start == BeamConnection.HINGED_END
                 and self.element.hinge_end == BeamConnection.HINGED_END
             ):
                 fef_flex = np.zeros(4)
 
+            else:
+                raise AttributeError(
+                    f"Wrong hinge type: {self.element.hinge_start}, {self.element.hinge_end}"
+                )
+
         else:
             fef_flex = np.zeros(4)
 
         return fef_flex
 
     def get_axial_displacements(
         self, x: npt.NDArray[np.float64]
@@ -976,29 +1011,32 @@
         """
         # Get temperature gradient relative to member local y-axis
         dty = self.temperature_gradients[1]
 
         # Check if temperature gradient is not null
         if dty:
             # Basic member properties
-            alpha = self.element.member.material.thermal_expansion_coefficient
+            alpha = self.element.member.section.material.thermal_expansion_coefficient
             h = self.element.member.section.height_y
             L = self.element.length
 
             # Timoshenko parameter
             if self.element.member.element_type == Element1DType.NAVIER:
                 Omega = 0.0
 
             elif self.element.member.element_type == Element1DType.TIMOSHENKO:
-                E = self.element.member.material.elastic_modulus
-                G = self.element.member.material.shear_modulus
-                As = self.element.member.section.area_y
-                I = self.element.member.section.inertia_z
+                EI = self.element.member.section.EIz
+                GA = self.element.member.section.GAy
 
-                Omega = E * I / (G * As * L * L)
+                Omega = EI / (GA * L * L)
+
+            else:
+                raise AttributeError(
+                    f"Wrong element type: {self.element.member.element_type}"
+                )
 
             # Auxiliary parameters
             mu = 1 + 12 * Omega
             lamb = 1 + 3 * Omega
             gamma = 1 - 6 * Omega
 
             # Unitary dimensionless temperature gradient
@@ -1033,14 +1071,19 @@
 
             elif (
                 self.element.hinge_start == BeamConnection.HINGED_END
                 and self.element.hinge_end == BeamConnection.HINGED_END
             ):
                 v = tg * (-L * x / 2 + x**2 / 2)
 
+            else:
+                raise AttributeError(
+                    f"Wrong hinge type: {self.element.hinge_start}, {self.element.hinge_end}"
+                )
+
         else:
             v = np.zeros(x.shape)
 
         return v
 
     def get_flexural_xz_displacements(
         self, x: npt.NDArray[np.float64]
@@ -1054,29 +1097,32 @@
         """
         # Get temperature gradient relative to member local y-axis
         dtz = self.temperature_gradients[2]
 
         # Check if temperature gradient is not null
         if dtz:
             # Basic member properties
-            alpha = self.element.member.material.thermal_expansion_coefficient
+            alpha = self.element.member.section.material.thermal_expansion_coefficient
             h = self.element.member.section.height_z
             L = self.element.length
 
             # Timoshenko parameter
             if self.element.member.element_type == Element1DType.NAVIER:
                 Omega = 0.0
 
             elif self.element.member.element_type == Element1DType.TIMOSHENKO:
-                E = self.element.member.material.elastic_modulus
-                G = self.element.member.material.shear_modulus
-                As = self.element.member.section.area_z
-                I = self.element.member.section.inertia_y
+                EI = self.element.member.section.EIy
+                GA = self.element.member.section.GAz
 
-                Omega = E * I / (G * As * L * L)
+                Omega = EI / (GA * L * L)
+
+            else:
+                raise AttributeError(
+                    f"Wrong element type: {self.element.member.element_type}"
+                )
 
             # Auxiliary parameters
             mu = 1 + 12 * Omega
             lamb = 1 + 3 * Omega
             gamma = 1 - 6 * Omega
 
             # Unitary dimensionless temperature gradient
@@ -1111,11 +1157,16 @@
 
             elif (
                 self.element.hinge_start == BeamConnection.HINGED_END
                 and self.element.hinge_end == BeamConnection.HINGED_END
             ):
                 w = tg * (-L * x / 2 + x**2 / 2)
 
+            else:
+                raise AttributeError(
+                    f"Wrong hinge type: {self.element.hinge_start}, {self.element.hinge_end}"
+                )
+
         else:
             w = np.zeros(x.shape)
 
         return w
```

### Comparing `framesss-0.0.2/src/framesss/fea/boundary_conditions/nodal_load.py` & `framesss-0.0.3/src/framesss/fea/boundary_conditions/nodal_load.py`

 * *Files identical despite different names*

### Comparing `framesss-0.0.2/src/framesss/fea/boundary_conditions/prescribed_displacement.py` & `framesss-0.0.3/src/framesss/fea/boundary_conditions/prescribed_displacement.py`

 * *Files identical despite different names*

### Comparing `framesss-0.0.2/src/framesss/fea/element_1d.py` & `framesss-0.0.3/src/framesss/fea/element_1d.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from framesss.enums import Element1DType
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
     from framesss.fea.node import Node
     from framesss.pre.cases import LoadCase
+    from framesss.pre.cases import LoadCaseCombination
     from framesss.pre.member_1d import Member1D
 
-MAX_DISTANCE_BETWEEN_SAMPLING_POINTS = 0.1  # (m)
+MAX_DISTANCE_BETWEEN_SAMPLING_POINTS = 0.25  # (m)
 NUMERIC_GARBAGE = 1.0e-12
 
 
 class Element1D:
     """
     Class representing a one-dimensional (1D) element in a structural analysis model.
 
@@ -53,18 +54,20 @@
     :ivar number_of_sampling_points: The number of points along the element used for detailed analysis.
     :ivar sampling_points: The local x coordinates of the sampling points along the element's length.
     :ivar internal_coords: Coordinates for a set number of points along the element, used for
                            internal analysis and visualization purposes.
     :ivar stiffness_matrix_local: The element's stiffness matrix in the local coordinate system,
                                   initially None until computed.
     :ivar global_dofs: Global degrees of freedom indices for the element, initially None until set.
-    :ivar axial_force, shear_force_y, shear_force_z: Dictionaries mapping each LoadCase to the respective internal
-                                                     force at the start of the element.
-    :ivar torsional_moment, bending_moment_y, bending_moment_z: Dictionaries mapping each LoadCase to the respective
-                                                                internal moment at the start of the element.
+    :ivar end_axial_forces, end_shear_forces_y, end_shear_forces_z: Dictionaries mapping each LoadCase to the
+                            respective internal force at the start of the element.
+    :ivar end_torsional_moments, end_bending_moments_y, end_bending_moments_z: Dictionaries mapping each
+                            LoadCase to the respective internal moment at the start of the element.
+    :ivar peak_points: Dictionary mapping each LoadCase and LoadCaseCombination to the local x coordinate
+                       of potential critical points along the element's length.
     """
 
     def __init__(
         self,
         member: Member1D,
         nodes: list[Node],
         x_start: float,
@@ -100,15 +103,15 @@
         cx = dx / length
         cy = dy / length
         cz = dz / length
 
         # Calculate deformed configuration coordinates of 50 cross-sections
         # along the member local x-axis
         number_of_sampling_points = max(
-            int(np.ceil(length / MAX_DISTANCE_BETWEEN_SAMPLING_POINTS)) + 1, 11
+            int(np.ceil(length / MAX_DISTANCE_BETWEEN_SAMPLING_POINTS)) + 1, 9
         )
         internal_coords = np.ones([3, number_of_sampling_points])
         i = np.linspace(0, length, number_of_sampling_points)
         internal_coords[0, :] = internal_coords[0, :] * xi + i * cx
         internal_coords[1, :] = internal_coords[1, :] * yi + i * cy
         internal_coords[2, :] = internal_coords[2, :] * zi + i * cz
 
@@ -117,20 +120,46 @@
         self.sampling_points = np.linspace(0, self.length, number_of_sampling_points)
 
         self.stiffness_matrix_local: npt.NDArray[np.float64] = np.empty(
             0, dtype=np.float64
         )
         self.global_dofs: npt.NDArray[np.int64] = np.empty(0, dtype=np.int64)
 
-        self.axial_force: dict[LoadCase, npt.NDArray[np.float64]] = {}
-        self.shear_force_y: dict[LoadCase, npt.NDArray[np.float64]] = {}
-        self.shear_force_z: dict[LoadCase, npt.NDArray[np.float64]] = {}
-        self.torsional_moment: dict[LoadCase, npt.NDArray[np.float64]] = {}
-        self.bending_moment_y: dict[LoadCase, npt.NDArray[np.float64]] = {}
-        self.bending_moment_z: dict[LoadCase, npt.NDArray[np.float64]] = {}
+        self.end_axial_forces: dict[LoadCase, npt.NDArray[np.float64]] = {}
+        self.end_shear_forces_y: dict[LoadCase, npt.NDArray[np.float64]] = {}
+        self.end_shear_forces_z: dict[LoadCase, npt.NDArray[np.float64]] = {}
+        self.end_torsional_moments: dict[LoadCase, npt.NDArray[np.float64]] = {}
+        self.end_bending_moments_y: dict[LoadCase, npt.NDArray[np.float64]] = {}
+        self.end_bending_moments_z: dict[LoadCase, npt.NDArray[np.float64]] = {}
+
+        # [a, b, c]
+        self.axial_force_eqn_coefficients: dict[
+            LoadCase | LoadCaseCombination, npt.NDArray[np.float64]
+        ] = {}
+        self.shear_force_y_eqn_coefficients: dict[
+            LoadCase | LoadCaseCombination, npt.NDArray[np.float64]
+        ] = {}
+        self.shear_force_z_eqn_coefficients: dict[
+            LoadCase | LoadCaseCombination, npt.NDArray[np.float64]
+        ] = {}
+        self.torsional_moment_eqn_coefficients: dict[
+            LoadCase | LoadCaseCombination, npt.NDArray[np.float64]
+        ] = {}
+
+        # [a, b, c, d]
+        self.bending_moment_y_eqn_coefficients: dict[
+            LoadCase | LoadCaseCombination, npt.NDArray[np.float64]
+        ] = {}
+        self.bending_moment_z_eqn_coefficients: dict[
+            LoadCase | LoadCaseCombination, npt.NDArray[np.float64]
+        ] = {}
+
+        self.peak_points: dict[
+            LoadCase | LoadCaseCombination, npt.NDArray[np.float64]
+        ] = {}
 
     def __repr__(self) -> str:
         """Return a string representation of the element."""
         node_labels = [node.label for node in self.nodes]
         hinge_descriptions = [hinge for hinge in [self.hinge_start, self.hinge_end]]
         return (
             f"{self.__class__.__name__}("
@@ -165,15 +194,15 @@
         self, load_case: LoadCase
     ) -> npt.NDArray[np.float64]:
         """
         Return element internal actions related to the :class:`LoadCase`.
 
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         :return: Internal force vector.
-        :raise ValueError: If 'u_global' is None for the load_case.
+        :raise ValueError: If 'u_global' is None for the case.
         """
         # Get nodal displacements and rotations at member end nodes in global system
         if (u := load_case.u_global) is not None:
             u_g = u[self.global_dofs]
         else:
             raise ValueError("'u_global' is not initialized.")
 
@@ -185,64 +214,59 @@
 
     def get_axial_stiffness_coefficients(self) -> npt.NDArray[np.float64]:
         """
         Return axial stiffness coefficient matrix.
 
         :return kea: A 2x2 matrix with axial stiffness coefficients.
         """
-        E = self.member.material.elastic_modulus
-        A = self.member.section.area_x
+        EA = self.member.section.EA
         L = self.length
 
-        k11 = E * A / L
+        k11 = EA / L
 
         kea = k11 * np.array([[+1, -1], [-1, +1]])
 
         return kea
 
     def get_torsion_stiffness_coefficients(self) -> npt.NDArray[np.float64]:
         """
         Return torsion stiffness coefficient matrix.
 
         :return ket: A 2x2 matrix with torsion stiffness coefficients.
         """
-        G = self.member.material.shear_modulus
-        Jt = self.member.section.inertia_x
+        GJ = self.member.section.GJt
         L = self.length
 
         if (self.hinge_start == BeamConnection.CONTINUOUS_END) and (
             self.hinge_end == BeamConnection.CONTINUOUS_END
         ):
-            k11 = G * Jt / L
+            k11 = GJ / L
 
             ket = k11 * np.array([[+1, -1], [-1, +1]])
 
         else:
             ket = np.zeros([2, 2])
 
         return ket
 
     def get_flexural_xy_stiffness_coefficients(self) -> npt.NDArray[np.float64]:
         """
         Return flexural stiffness coefficient matrix in local xy-plane.
 
         :return kef: A 4x4 matrix with flexural stiffness coefficients.
         """
-        E = self.member.material.elastic_modulus
-        I = self.member.section.inertia_z  # noqa: E741
+        EI = self.member.section.EIz
         L = self.length
-        EI = E * I
 
         if self.member.element_type == Element1DType.NAVIER:
             Omega = 0.0
         elif self.member.element_type == Element1DType.TIMOSHENKO:
-            G = self.member.material.shear_modulus
-            As = self.member.section.area_y
+            GA = self.member.section.GAy
 
-            Omega = EI / (G * As * L * L)
+            Omega = EI / (GA * L * L)
         else:
             raise ValueError(f"Unknown member type: {self.member.element_type}.")
 
         lamb = 1 + 3 * Omega
         mu = 1 + 12 * Omega
         gamma = 1 - 6 * Omega
 
@@ -318,26 +342,23 @@
 
     def get_flexural_xz_stiffness_coefficients(self) -> npt.NDArray[np.float64]:
         """
         Return flexural stiffness coefficient matrix in local xz-plane.
 
         :return kef: A 4x4 matrix with flexural stiffness coefficients.
         """
-        E = self.member.material.elastic_modulus
-        I = self.member.section.inertia_y  # noqa: E741
+        EI = self.member.section.EIy
         L = self.length
-        EI = E * I
 
         if self.member.element_type == Element1DType.NAVIER:
             Omega = 0.0
         elif self.member.element_type == Element1DType.TIMOSHENKO:
-            G = self.member.material.shear_modulus
-            As = self.member.section.area_z
+            GA = self.member.section.GAz
 
-            Omega = EI / (G * As * L * L)
+            Omega = EI / (GA * L * L)
         else:
             raise ValueError(f"Unknown member type: {self.member.element_type}.")
 
         lamb = 1 + 3 * Omega
         mu = 1 + 12 * Omega
         gamma = 1 - 6 * Omega
 
@@ -421,15 +442,15 @@
         displacement(s) of an element.
 
         :param x: The position(s) along the element's local x-axis.
         :return: A 2x*n* matrix with the evaluated axial displacement
                  shape functions at the specified position(s).
         """
         L = self.length
-        # TODO: Transpose the solution?
+
         return np.array([1 - x / L, x / L])
 
     def get_flexural_xy_displacement_shape_functions(
         self, x: npt.NDArray[np.float64]
     ) -> npt.NDArray[np.float64]:
         """
         Return the flexural displacement shape functions in local xy-plane at a given position(s).
@@ -446,20 +467,18 @@
         L = self.length
         L2 = L * L
         L3 = L2 * L
 
         if self.member.element_type == Element1DType.NAVIER:
             Omega = 0.0
         elif self.member.element_type == Element1DType.TIMOSHENKO:
-            E = self.member.material.elastic_modulus
-            G = self.member.material.shear_modulus
-            As = self.member.section.area_y
-            I = self.member.section.inertia_z  # noqa: E741
+            EI = self.member.section.EIz
+            GA = self.member.section.GAy
 
-            Omega = E * I / (G * As * L * L)
+            Omega = EI / (GA * L * L)
         else:
             raise ValueError(f"Unknown member type: {self.member.element_type}.")
 
         lamb = 1 + 3 * Omega
         mu = 1 + 12 * Omega
         gamma = 1 - 6 * Omega
 
@@ -553,20 +572,18 @@
         L = self.length
         L2 = L * L
         L3 = L2 * L
 
         if self.member.element_type == Element1DType.NAVIER:
             Omega = 0.0
         elif self.member.element_type == Element1DType.TIMOSHENKO:
-            E = self.member.material.elastic_modulus
-            G = self.member.material.shear_modulus
-            As = self.member.section.area_z
-            I = self.member.section.inertia_y  # noqa: E741
+            EI = self.member.section.EIy
+            GA = self.member.section.GAz
 
-            Omega = E * I / (G * As * L * L)
+            Omega = EI / (GA * L * L)
         else:
             raise ValueError(f"Unknown member type: {self.member.element_type}.")
 
         lamb = 1 + 3 * Omega
         mu = 1 + 12 * Omega
         gamma = 1 - 6 * Omega
 
@@ -668,357 +685,478 @@
         N = self.member.analysis.get_displacement_shape_function_matrix(self)
 
         # Compute internal displacements matrix from global fea
         return self.member.analysis.get_internal_displacements_from_global_analysis(
             N, u_local
         )
 
-    def get_axial_equation_coefficients(
+    def save_axial_equation_coefficients_for_load_case(
         self, load_case: LoadCase
-    ) -> tuple[float, float, float]:
+    ) -> None:
         """
         Calculate axial force coefficients for an element under given load case.
 
         For linear distributed load, the axial force equation
         is defined as: N(x) = (a / 2) * x^2 + b * x + c.
 
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         :return: A tuple of three floats representing the coefficients of the axial force equation.
         """
-        n_start = -self.axial_force[load_case][0]
+        n_start = -self.end_axial_forces[load_case][0]
 
         if abs(n_start) < NUMERIC_GARBAGE:
             n_start = 0.0
 
         if load := load_case.element_distributed_loads.get(self):
             f_start = +load.components_local[0]
             f_end = +load.components_local[3]
         else:
             # There is no load on element => axial force is constant
-            return 0.0, 0.0, n_start
+            self.axial_force_eqn_coefficients[load_case] = np.array([0.0, 0.0, n_start])
+            return
 
         # Linear load equation coefficients: fx(x) = ax + b
         a, b = get_load_equation_coefficients(f_start, f_end, self.length)
 
         # Normal force equation coefficients: N(x) = (a / 2) * x^2 + b * x + c
         a, b, c = get_internal_force_coefficients(a, b, n_start)
 
-        return -a, -b, c
+        self.axial_force_eqn_coefficients[load_case] = np.array([-a, -b, c])
 
-    def get_internal_axial_forces(
-        self, load_case: LoadCase, x: npt.NDArray[np.float64]
-    ) -> npt.NDArray[np.float64]:
+    def save_axial_equation_coefficients_for_load_combination(
+        self, load_combination: LoadCaseCombination
+    ) -> None:
         """
-        Calculate axial forces along the element for given load case.
+        Calculate axial force coefficients for an element under given load combination.
 
-        This method computes the axial force distribution along the element for a specific load
-        case. For truss structures, the axial force is considered constant. For other types of
-        structures, the axial force is calculated using the coefficients from the axial force equation.
+        For linear distributed load, the axial force equation
+        is defined as: N(x) = (a / 2) * x^2 + b * x + c.
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
-        :param x: An array of positions along the element's x-axis where the internal axial forces are to be computed.
-        :return: The calculated axial forces at the specified positions.
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
+        :return: A tuple of three floats representing the coefficients of the axial force equation.
         """
-        # TODO: Probably don't support truss structures.
-        # # Axial force is constant for truss structures
-        # if (self.member.analysis.analysis_type == AnalysisModelType.TRUSS_XZ) or (
-        #     self.member.analysis.analysis_type == AnalysisModelType.TRUSS_XYZ
-        # ):
-        #     return -self.axial_force[load_case][0]
+        coefficients = np.zeros(3, dtype=np.float64)
 
-        a, b, c = self.get_axial_equation_coefficients(load_case)
+        for load_case, factor in load_combination.load_cases.items():
+            coefficients += self.axial_force_eqn_coefficients[load_case] * factor
 
-        normal_forces = a * x**2 + b * x + c
+        self.axial_force_eqn_coefficients[load_combination] = coefficients
 
-        return normal_forces
+    def save_peak_points_for_axial_force_eqn(
+        self, case: LoadCase | LoadCaseCombination
+    ) -> None:
+        """
+        Calculate positions of local extreme axial forces for given load case or load combination.
 
-    def get_max_internal_axial_forces(
-        self, load_case: LoadCase
-    ) -> npt.NDArray[np.float64]:
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
+        :return: An array of points where local extremes can occur.
         """
-        Calculate local extreme axial forces for given load case.
+        a, b, c = self.axial_force_eqn_coefficients[case]
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
-        :return: An array where each row contains a pair [position, axial force] for each critical point.
+        x_peaks = get_suspicious_points([b, 2 * a], self.length)
+
+        if case in self.peak_points:
+            peak_points = self.peak_points[case]
+            peak_points = np.append(peak_points, x_peaks)
+        else:
+            peak_points = np.array(x_peaks)
+
+        peak_points = np.unique(peak_points)
+
+        self.peak_points[case] = peak_points
+
+    def get_axial_force(
+        self, case: LoadCase | LoadCaseCombination, x: npt.NDArray[np.float64] | float
+    ) -> npt.NDArray[np.float64]:
         """
-        a, b, c = self.get_axial_equation_coefficients(load_case)
+        Calculate axial forces along the element for given load case.
 
-        x_max = get_suspicious_points([b, 2 * a], self.length)
+        This method computes the axial force distribution along the element for a specific load
+        case. For truss structures, the axial force is considered constant. For other types of
+        structures, the axial force is calculated using the coefficients from the axial force equation.
 
-        max_normal_forces = self.get_internal_axial_forces(load_case, x_max)
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
+        :param x: An array of positions along the element's x-axis where the internal axial forces are to be computed.
+        :return: The calculated axial forces at the specified positions.
+        """
+        a, b, c = self.axial_force_eqn_coefficients[case]
 
-        return np.vstack((self.x_start + x_max, max_normal_forces)).T
+        return a * x**2 + b * x + c  # type: ignore[no-any-return]
 
-    def get_shear_force_xy_equation_coefficients(
+    def save_shear_force_xy_equation_coefficients_for_load_case(
         self, load_case: LoadCase
-    ) -> tuple[float, float, float]:
+    ) -> None:
         """
         Calculate shear force coefficients in local xy plane for an element under given load case.
 
         For linear distributed load, the shear force equation
         is defined as: V(x) = (a / 2) * x^2 + b * x + c.
 
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         :return: A tuple of three floats representing the coefficients of the shear force equation.
         """
-        shear_start = +self.shear_force_y[load_case][0]
+        shear_start = +self.end_shear_forces_y[load_case][0]
 
         if abs(shear_start) < NUMERIC_GARBAGE:
             shear_start = 0.0
 
         if load := load_case.element_distributed_loads.get(self):
             f_start = +load.components_local[1]
             f_end = +load.components_local[4]
         else:
             # There is no load on element => shear force is constant
-            return 0.0, 0.0, shear_start
+            self.shear_force_y_eqn_coefficients[load_case] = np.array(
+                [0.0, 0.0, shear_start]
+            )
+            return
 
         # Linear load equation coefficients: fx(x) = ax + b
         a, b = get_load_equation_coefficients(f_start, f_end, self.length)
 
         # Normal force equation coefficients: N(x) = (a / 2) * x^2 + b * x + c
         a, b, c = get_internal_force_coefficients(a, b, shear_start)
 
-        return a, b, c
+        self.shear_force_y_eqn_coefficients[load_case] = np.array([a, b, c])
 
-    def get_internal_shear_forces_xy(
-        self, load_case: LoadCase, x: npt.NDArray[np.float64]
-    ) -> npt.NDArray[np.float64]:
+    def save_shear_force_xy_equation_coefficients_for_load_combination(
+        self, load_combination: LoadCaseCombination
+    ) -> None:
         """
-        Calculate shear forces in local xy plane along the element for given load case.
+        Calculate shear force coefficients in local xy plane for an element under given load case.
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
-        :param x: An array of positions along the element's x-axis where the internal axial forces are to be computed.
-        :return: The calculated shear forces in local xy plane at the specified positions.
+        For linear distributed load, the shear force equation
+        is defined as: V(x) = (a / 2) * x^2 + b * x + c.
+
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
+        :return: A tuple of three floats representing the coefficients of the shear force equation.
         """
-        a, b, c = self.get_shear_force_xy_equation_coefficients(load_case)
+        coefficients = np.zeros(3, dtype=np.float64)
 
-        shear_forces_xy = a * x**2 + b * x + c
+        for load_case, factor in load_combination.load_cases.items():
+            coefficients += self.shear_force_y_eqn_coefficients[load_case] * factor
 
-        return shear_forces_xy
+        self.shear_force_y_eqn_coefficients[load_combination] = coefficients
 
-    def get_max_internal_shear_forces_xy(
-        self, load_case: LoadCase
-    ) -> npt.NDArray[np.float64]:
+    def save_peak_points_for_shear_force_xy_eqn(
+        self, case: LoadCase | LoadCaseCombination
+    ) -> None:
         """
-        Calculate local extreme shear forces in local xy plane for given load case.
+        Calculate positions of local extreme shear forces for given load case or load combination.
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
-        :return: An array where each row contains a pair [position, shear force] for each critical point.
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
+        :return: An array of points where local extremes can occur.
         """
-        a, b, c = self.get_shear_force_xy_equation_coefficients(load_case)
+        a, b, c = self.shear_force_y_eqn_coefficients[case]
 
-        x_max = get_suspicious_points([b, 2 * a], self.length)
+        x_peaks = get_suspicious_points([b, 2 * a], self.length)
+
+        if case in self.peak_points:
+            peak_points = self.peak_points[case]
+            peak_points = np.append(peak_points, x_peaks)
+        else:
+            peak_points = np.array(x_peaks)
+
+        peak_points = np.unique(peak_points)
+
+        self.peak_points[case] = peak_points
+
+    def get_shear_force_xy(
+        self, case: LoadCase | LoadCaseCombination, x: npt.NDArray[np.float64] | float
+    ) -> npt.NDArray[np.float64]:
+        """
+        Calculate shear forces in local xy plane along the element for given load case.
 
-        max_shear_forces_xy = self.get_internal_shear_forces_xy(load_case, x_max)
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
+        :param x: An array of positions along the element's x-axis where the internal axial forces are to be computed.
+        :return: The calculated shear forces in local xy plane at the specified positions.
+        """
+        a, b, c = self.shear_force_y_eqn_coefficients[case]
 
-        return np.vstack((self.x_start + x_max, max_shear_forces_xy)).T
+        return a * x**2 + b * x + c  # type: ignore[no-any-return]
 
-    def get_shear_force_xz_equation_coefficients(
+    def save_shear_force_xz_equation_coefficients_for_load_case(
         self, load_case: LoadCase
-    ) -> tuple[float, float, float]:
+    ) -> None:
         """
         Calculate shear force coefficients in local xz plane for an element under given load case.
 
         For linear distributed load, the shear force equation
         is defined as: V(x) = (a / 2) * x^2 + b * x + c.
 
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         :return: A tuple of three floats representing the coefficients of the shear force equation.
         """
-        shear_start = +self.shear_force_z[load_case][0]
+        shear_start = +self.end_shear_forces_z[load_case][0]
 
         if abs(shear_start) < NUMERIC_GARBAGE:
             shear_start = 0.0
 
         if load := load_case.element_distributed_loads.get(self):
             f_start = +load.components_local[2]
             f_end = +load.components_local[5]
         else:
             # There is no load on element => shear force is constant
-            return 0.0, 0.0, shear_start
+            self.shear_force_z_eqn_coefficients[load_case] = np.array(
+                [0.0, 0.0, shear_start]
+            )
+            return
 
         # Linear load equation coefficients: fx(x) = ax + b
         a, b = get_load_equation_coefficients(f_start, f_end, self.length)
 
         # Normal force equation coefficients: N(x) = (a / 2) * x^2 + b * x + c
         a, b, c = get_internal_force_coefficients(a, b, shear_start)
 
-        return a, b, c
+        self.shear_force_z_eqn_coefficients[load_case] = np.array([a, b, c])
 
-    def get_internal_shear_forces_xz(
-        self, load_case: LoadCase, x: npt.NDArray[np.float64]
-    ) -> npt.NDArray[np.float64]:
+    def save_shear_force_xz_equation_coefficients_for_load_combination(
+        self, load_combination: LoadCaseCombination
+    ) -> None:
         """
-        Calculate shear forces in local xz plane along the element for given load case.
+        Calculate shear force coefficients in local xz plane for an element under given load combination.
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
-        :param x: An array of positions along the element's x-axis where the internal shear forces are to be computed.
-        :return: The calculated shear forces in local xz plane at the specified positions.
+        For linear distributed load, the shear force equation
+        is defined as: V(x) = (a / 2) * x^2 + b * x + c.
+
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
+        :return: A tuple of three floats representing the coefficients of the shear force equation.
         """
-        a, b, c = self.get_shear_force_xz_equation_coefficients(load_case)
+        coefficients = np.zeros(3, dtype=np.float64)
 
-        shear_forces_xz = a * x**2 + b * x + c
+        for load_case, factor in load_combination.load_cases.items():
+            coefficients += self.shear_force_z_eqn_coefficients[load_case] * factor
 
-        return shear_forces_xz
+        self.shear_force_z_eqn_coefficients[load_combination] = coefficients
 
-    def get_max_internal_shear_forces_xz(
-        self, load_case: LoadCase
-    ) -> npt.NDArray[np.float64]:
+    def save_peak_points_for_shear_force_xz_eqn(
+        self, case: LoadCase | LoadCaseCombination
+    ) -> None:
         """
-        Calculate local extreme shear forces in local xz plane for given load case.
+        Calculate positions of local extreme shear forces for given load case or load combination.
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
-        :return: An array where each row contains a pair [position, shear force] for each critical point.
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
+        :return: An array of points where local extremes can occur.
         """
-        a, b, c = self.get_shear_force_xz_equation_coefficients(load_case)
+        a, b, c = self.shear_force_z_eqn_coefficients[case]
+
+        x_peaks = get_suspicious_points([b, 2 * a], self.length)
+
+        if case in self.peak_points:
+            peak_points = self.peak_points[case]
+            peak_points = np.append(peak_points, x_peaks)
+        else:
+            peak_points = np.array(x_peaks)
 
-        x_max = get_suspicious_points([b, 2 * a], self.length)
+        peak_points = np.unique(peak_points)
 
-        max_shear_forces_xz = self.get_internal_shear_forces_xz(load_case, x_max)
+        self.peak_points[case] = peak_points
 
-        return np.vstack((self.x_start + x_max, max_shear_forces_xz)).T
+    def get_shear_force_xz(
+        self, case: LoadCase | LoadCaseCombination, x: npt.NDArray[np.float64] | float
+    ) -> npt.NDArray[np.float64]:
+        """
+        Calculate shear forces in local xz plane along the element for given load case.
 
-    def get_bending_moment_xy_equation_coefficients(
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
+        :param x: An array of positions along the element's x-axis where the internal shear forces are to be computed.
+        :return: The calculated shear forces in local xz plane at the specified positions.
+        """
+        a, b, c = self.shear_force_z_eqn_coefficients[case]
+
+        return a * x**2 + b * x + c  # type: ignore[no-any-return]
+
+    def save_bending_moment_xy_equation_coefficients_for_load_case(
         self, load_case: LoadCase
-    ) -> tuple[float, float, float, float]:
+    ) -> None:
         """
         Calculate bending moment coefficients about local z-axis for an element under given load case.
 
         For linear distributed load, the bending moment equation
         is defined as: M(x) = (a / 6) * x^3 + (b / 2)* x^2 + c * x + d.
 
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         :return: A tuple of four floats representing the coefficients of the bending moment equation.
         """
-        moment_start = float(-self.bending_moment_z[load_case][0])
-        shear_start = float(+self.shear_force_y[load_case][0])
+        moment_start = float(-self.end_bending_moments_z[load_case][0])
+        shear_start = float(+self.end_shear_forces_y[load_case][0])
 
         if abs(moment_start) < NUMERIC_GARBAGE:
             moment_start = 0.0
         if abs(shear_start) < NUMERIC_GARBAGE:
             shear_start = 0.0
 
         if load := load_case.element_distributed_loads.get(self):
             f_start = float(+load.components_local[1])
             f_end = float(+load.components_local[4])
         else:
             # There is no load on element => bending moment is linear
-            return 0.0, 0.0, shear_start, moment_start
+            self.bending_moment_z_eqn_coefficients[load_case] = np.array(
+                [0.0, 0.0, shear_start, moment_start]
+            )
+            return
 
         # Linear load equation coefficients: fx(x) = ax + b
         a, b = get_load_equation_coefficients(f_start, f_end, self.length)
 
         # Bending moment equation coefficients: M(x) = (a / 6) * x^3 + (b / 2)* x^2 + c * x + d
         a, b, c, d = get_internal_moment_coefficients(a, b, shear_start, moment_start)
 
-        return a, b, c, d
+        self.bending_moment_z_eqn_coefficients[load_case] = np.array([a, b, c, d])
 
-    def get_internal_bending_moments_xy(
-        self, load_case: LoadCase, x: npt.NDArray[np.float64]
-    ) -> npt.NDArray[np.float64]:
+    def save_bending_moment_xy_equation_coefficients_for_load_combination(
+        self, load_combination: LoadCaseCombination
+    ) -> None:
         """
-        Calculate bending moment about local z-axis along the element for given load case.
+        Calculate bending moment coefficients about local z-axis for an element under given load combination.
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
-        :param x: An array of positions along the element's x-axis where the internal bending
-                  moments are to be computed.
-        :return: The calculated bending moments about local z-axis at the specified positions.
+        For linear distributed load, the bending moment equation
+        is defined as: M(x) = (a / 6) * x^3 + (b / 2)* x^2 + c * x + d.
+
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
+        :return: A tuple of four floats representing the coefficients of the bending moment equation.
         """
-        a, b, c, d = self.get_bending_moment_xy_equation_coefficients(load_case)
+        coefficients = np.zeros(4, dtype=np.float64)
 
-        bending_moments_xy = a * x**3 + b * x**2 + c * x + d
+        for load_case, factor in load_combination.load_cases.items():
+            coefficients += self.bending_moment_z_eqn_coefficients[load_case] * factor
 
-        return bending_moments_xy  # type: ignore[no-any-return]
+        self.bending_moment_z_eqn_coefficients[load_combination] = coefficients
 
-    def get_max_internal_bending_moments_xy(
-        self, load_case: LoadCase
-    ) -> npt.NDArray[np.float64]:
+    def save_peak_points_for_bending_moment_xy_eqn(
+        self, case: LoadCase | LoadCaseCombination
+    ) -> None:
         """
         Calculate local extreme bending moments about z-axis for given load case.
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
         :return: An array where each row contains a pair [position, bending moment] for each critical point.
         """
-        a, b, c, d = self.get_bending_moment_xy_equation_coefficients(load_case)
+        a, b, c, d = self.bending_moment_z_eqn_coefficients[case]
 
-        x_max = get_suspicious_points([c, 2 * b, 3 * a], self.length)
+        x_peaks = get_suspicious_points([c, 2 * b, 3 * a], self.length)
+
+        if case in self.peak_points:
+            peak_points = self.peak_points[case]
+            peak_points = np.append(peak_points, x_peaks)
+        else:
+            peak_points = np.array(x_peaks)
 
-        max_bending_moment_xy = self.get_internal_bending_moments_xy(load_case, x_max)
+        peak_points = np.unique(peak_points)
 
-        return np.vstack((self.x_start + x_max, max_bending_moment_xy)).T
+        self.peak_points[case] = peak_points
+
+    def get_bending_moment_xy(
+        self, case: LoadCase | LoadCaseCombination, x: npt.NDArray[np.float64] | float
+    ) -> npt.NDArray[np.float64]:
+        """
+        Calculate bending moment about local z-axis along the element for given load case.
 
-    def get_bending_moment_xz_equation_coefficients(
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
+        :param x: An array of positions along the element's x-axis where the internal bending
+                  moments are to be computed.
+        :return: The calculated bending moments about local z-axis at the specified positions.
+        """
+        a, b, c, d = self.bending_moment_z_eqn_coefficients[case]
+
+        return a * x**3 + b * x**2 + c * x + d  # type: ignore[no-any-return]
+
+    def save_bending_moment_xz_equation_coefficients_for_load_case(
         self, load_case: LoadCase
-    ) -> tuple[float, float, float, float]:
+    ) -> None:
         """
         Calculate bending moment coefficients about local y-axis for an element under given load case.
 
         For linear distributed load, the bending moment equation
         is defined as: M(x) = (a / 6) * x^3 + (b / 2)* x^2 + c * x + d.
 
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         :return: A tuple of four floats representing the coefficients of the bending moment equation.
         """
-        moment_start = float(+self.bending_moment_y[load_case][0])
-        shear_start = float(+self.shear_force_z[load_case][0])
+        moment_start = float(+self.end_bending_moments_y[load_case][0])
+        shear_start = float(+self.end_shear_forces_z[load_case][0])
 
         if abs(moment_start) < NUMERIC_GARBAGE:
             moment_start = 0.0
         if abs(shear_start) < NUMERIC_GARBAGE:
             shear_start = 0.0
 
         if load := load_case.element_distributed_loads.get(self):
             f_start = float(+load.components_local[2])
             f_end = float(+load.components_local[5])
         else:
             # There is no load on element => bending moment is linear
-            return 0.0, 0.0, shear_start, moment_start
+            self.bending_moment_y_eqn_coefficients[load_case] = np.array(
+                [0.0, 0.0, shear_start, moment_start]
+            )
+            return
 
         # Linear load equation coefficients: fx(x) = ax + b
         a, b = get_load_equation_coefficients(f_start, f_end, self.length)
 
         # Bending moment equation coefficients: M(x) = (a / 6) * x^3 + (b / 2)* x^2 + c * x + d
         a, b, c, d = get_internal_moment_coefficients(a, b, shear_start, moment_start)
 
-        return a, b, c, d
+        self.bending_moment_y_eqn_coefficients[load_case] = np.array([a, b, c, d])
 
-    def get_internal_bending_moments_xz(
-        self, load_case: LoadCase, x: npt.NDArray[np.float64]
-    ) -> npt.NDArray[np.float64]:
+    def save_bending_moment_xz_equation_coefficients_for_load_combination(
+        self, load_combination: LoadCaseCombination
+    ) -> None:
         """
-        Calculate bending moment about local y-axis along the element for given load case.
+        Calculate bending moment coefficients about local y-axis for an element under given load combination.
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
-        :param x: An array of positions along the element's x-axis where the internal bending moments
-                  are to be computed.
-        :return: The calculated bending moments about local y-axis at the specified positions.
+        For linear distributed load, the bending moment equation
+        is defined as: M(x) = (a / 6) * x^3 + (b / 2)* x^2 + c * x + d.
+
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
+        :return: A tuple of four floats representing the coefficients of the bending moment equation.
         """
-        a, b, c, d = self.get_bending_moment_xz_equation_coefficients(load_case)
+        coefficients = np.zeros(4, dtype=np.float64)
 
-        bending_moments_xz = a * x**3 + b * x**2 + c * x + d
+        for load_case, factor in load_combination.load_cases.items():
+            coefficients += self.bending_moment_y_eqn_coefficients[load_case] * factor
 
-        return bending_moments_xz  # type: ignore[no-any-return]
+        self.bending_moment_y_eqn_coefficients[load_combination] = coefficients
 
-    def get_max_internal_bending_moments_xz(
-        self, load_case: LoadCase
-    ) -> npt.NDArray[np.float64]:
+    def save_peak_points_for_bending_moment_xz_eqn(
+        self, case: LoadCase | LoadCaseCombination
+    ) -> None:
         """
-        Calculate local extreme bending moments about z-axis for given load case.
+        Calculate local extreme bending moments about y-axis for given load case.
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
         :return: An array where each row contains a pair [position, bending moment] for each critical point.
         """
-        a, b, c, d = self.get_bending_moment_xz_equation_coefficients(load_case)
+        a, b, c, d = self.bending_moment_y_eqn_coefficients[case]
+
+        x_peaks = get_suspicious_points([c, 2 * b, 3 * a], self.length)
+
+        if case in self.peak_points:
+            peak_points = self.peak_points[case]
+            peak_points = np.append(peak_points, x_peaks)
+        else:
+            peak_points = np.array(x_peaks)
 
-        x_max = get_suspicious_points([c, 2 * b, 3 * a], self.length)
+        peak_points = np.unique(peak_points)
 
-        max_bending_moment_xz = self.get_internal_bending_moments_xz(load_case, x_max)
+        self.peak_points[case] = peak_points
+
+    def get_bending_moment_xz(
+        self, case: LoadCase | LoadCaseCombination, x: npt.NDArray[np.float64] | float
+    ) -> npt.NDArray[np.float64]:
+        """
+        Calculate bending moment about local y-axis along the element for given load case.
+
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
+        :param x: An array of positions along the element's x-axis where the internal bending moments
+                  are to be computed.
+        :return: The calculated bending moments about local y-axis at the specified positions.
+        """
+        a, b, c, d = self.bending_moment_y_eqn_coefficients[case]
 
-        return np.vstack((self.x_start + x_max, max_bending_moment_xz)).T
+        return a * x**3 + b * x**2 + c * x + d  # type: ignore[no-any-return]
 
 
 def get_load_equation_coefficients(
     f_start: float, f_end: float, length: float
 ) -> tuple[float, float]:
     """
     Calculate the coefficients of the linear load equation 'f(x) = a * x + b'.
```

### Comparing `framesss-0.0.2/src/framesss/fea/models/model.py` & `framesss-0.0.3/src/framesss/fea/models/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 import numpy as np
 
 from framesss.enums import BeamConnection
 from framesss.enums import Element1DType
 from framesss.enums import SupportFixity
 from framesss.fea.node import Node
+from framesss.pre.cases import EnvelopeCombination
 from framesss.pre.cases import LoadCase
-from framesss.pre.cases import LoadCombination
+from framesss.pre.cases import LoadCaseCombination
 from framesss.pre.member_1d import Member1D
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
     from framesss.fea.analysis.analysis import Analysis
     from framesss.fea.element_1d import Element1D
@@ -35,16 +36,16 @@
     :ivar sections: A set of :class:`Section` instances, detailing the cross-sectional properties of members.
     :ivar nodes: A set of :class:`Node` instances, defining the points of interest within the model
                  where members connect or loads are applied.
     :ivar members: A set of :class:`Member1D` instances, representing the one-dimensional structural
                    members (e.g., beams, columns) in the model.
     :ivar load_cases: A set of :class:`LoadCase` instances, each defining a unique set
                       of loading conditions to be analyzed.
-    :ivar load_combinations: A set of :class:`LoadCombination` instances, defining
-                             combinations of load cases for analysis.
+    :ivar load_combinations: A set of :class:`LoadCaseCombination` instances, defining
+                             load_cases of load cases for analysis.
     :ivar elements: A set of :class:`Element1D` instances.
     :ivar neq_free: Number of equations corresponding to free DoFs.
     :ivar neq_fixed: Number of equations corresponding to fixed DoFs.
     :ivar neq_spring: Number of equations corresponding to spring DoFs.
     :ivar k_global: Global stiffness matrix for the entire model.
     :ivar spring_stiffness_global: List containing global spring stiffness coefficients.
     :ivar dof_connectivity_matrix: Matrix defining the global numbering of DoFs for each node.
@@ -57,15 +58,16 @@
         """Init the Model object."""
         self.analysis = analysis
         self.materials: set[Material] = set()
         self.sections: set[Section] = set()
         self.nodes: set[Node] = set()
         self.members: set[Member1D] = set()
         self.load_cases: set[LoadCase] = set()
-        self.load_combinations: set[LoadCombination] = set()
+        self.load_combinations: set[LoadCaseCombination] = set()
+        self.envelopes: set[EnvelopeCombination] = set()
         self.elements: set[Element1D] = set()
 
         self.neq_free: int = 0
         self.neq_fixed: int = 0
         self.neq_spring: int = 0
 
         self.k_global: npt.NDArray[np.float64] = np.empty(0, dtype=np.float64)
@@ -125,38 +127,35 @@
         return new_node
 
     def add_member(
         self,
         label: str,
         element_type: str,
         nodes: list[Node],
-        material: Material,
         section: Section,
         hinges: list[str] | tuple[str, str] = (BeamConnection.CONTINUOUS_END,) * 2,
     ) -> Member1D:
         """
         Create and return new :class:`Member1D` instance.
 
         :param label: A user-defined label for the member.
         :param element_type: Specifies the type of the element ('navier', 'timoshenko').
         :param nodes: A list of nodes at the start and the end of the member.
-        :param material: The material of the member.
         :param section: The cross-section of the member.
         :param hinges: Defines the type of connections at the start and the end of the  member
                        (e.g., fixed, hinged, or semirigid) to model the rotational stiffness accurately.
         """
         elem_type = Element1DType(element_type)
         hngs = [BeamConnection(hng) for hng in hinges]
 
         aux = self.analysis.get_auxiliary_vector_in_local_xy_plane(nodes)
         new_member = Member1D(
             label,
             elem_type,
             nodes,
-            material,
             section,
             hngs,
             aux,
             self.analysis,
         )
         self.members.add(new_member)
         return new_member
@@ -167,28 +166,41 @@
 
         :param label: Unique user-defined label of the load case.
         """
         new_case = LoadCase(label)
         self.load_cases.add(new_case)
         return new_case
 
-    def add_load_combination(
+    def add_load_case_combination(
         self, label: str, combination: dict[LoadCase, float]
-    ) -> LoadCombination:
+    ) -> LoadCaseCombination:
         """
-        Add and return new :class:`LoadCombination` instance.
+        Add and return new :class:`LoadCaseCombination` instance.
 
         :param label: Unique user-defined label of the load combination.
         :param combination: Dictionary mapping :class:`LoadCase` instances
                             to their scaling factors.
         """
-        new_combination = LoadCombination(label, combination)
+        new_combination = LoadCaseCombination(label, combination)
         self.load_combinations.add(new_combination)
         return new_combination
 
+    def add_envelope(
+        self, label: str, cases: list[LoadCase | LoadCaseCombination]
+    ) -> EnvelopeCombination:
+        """
+        Add and return new :class:`EnvelopeCombination` instance.
+
+        :param label: Unique user-defined label of the load combination.
+        :param cases:  A list of :class:`LoadCase` and :class:`LoadCombination`.
+        """
+        new_envelope = EnvelopeCombination(label, cases)
+        self.envelopes.add(new_envelope)
+        return new_envelope
+
     def discretize_members(self) -> None:
         """
         Discretize all members in model and assign IDs to nodes and elements.
 
         This method iterates over each member in the model, calling its `discretize`
         method to divide it into finite elements. After discretization, it assigns
         a unique ID to each node and element in the model.
```

### Comparing `framesss-0.0.2/src/framesss/fea/node.py` & `framesss-0.0.3/src/framesss/fea/node.py`

 * *Files identical despite different names*

### Comparing `framesss-0.0.2/src/framesss/post/node_results.py` & `framesss-0.0.3/src/framesss/post/node_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from framesss.utils import DictProxy
 
 if TYPE_CHECKING:
     from typing_extensions import TypeAlias
 
     from framesss.fea.node import Node
     from framesss.pre.cases import LoadCase
-    from framesss.pre.cases import LoadCombination
+    from framesss.pre.cases import LoadCaseCombination
 
-    LoadType: TypeAlias = Union[LoadCase, LoadCombination]
+    LoadType: TypeAlias = Union[LoadCase, LoadCaseCombination]
     ResultDict: TypeAlias = dict[LoadType, float]
 
 FIXITIES_WITH_REACTION = [SupportFixity.FIXED_DOF, SupportFixity.SPRING_DOF]
 
 
 class NodeResults:
     """Class for storing results from finite element analysis."""
```

### Comparing `framesss-0.0.2/src/framesss/pre/cases.py` & `framesss-0.0.3/src/framesss/pre/cases.py`

 * *Files 16% similar despite different names*

```diff
@@ -82,33 +82,61 @@
             dofs = elem.global_dofs
             # get member equivalent nodal loads
             feg = thermal_load.get_equivalent_nodal_actions()
             # assemble equivalent nodal loads to global force vector
             self.f_global[dofs] += feg
 
 
-class LoadCombination:
+class LoadCaseCombination:
     """
     Represent a combination of load cases.
 
     :param label: A unique identifier for the load combination.
-    :ivar combinations: A dictionary mapping :class:`LoadCase` instances
+    :ivar load_cases: A dictionary mapping :class:`LoadCase` instances
                         to their scaling factors.
     """
 
-    def __init__(self, label: str, combinations: dict[LoadCase, float]) -> None:
-        """Init the LoadCombination class."""
+    def __init__(self, label: str, load_cases: dict[LoadCase, float]) -> None:
+        """Init the LoadCaseCombination class."""
         self.label = label
-        self.combinations = combinations
+        self.load_cases = load_cases
 
     def __repr__(self) -> str:
-        """Return a string representation of LoadCombination object."""
+        """Return a string representation of LoadCaseCombination object."""
         return f"{self.__class__.__name__}({self.label})"
 
     def add_load_case(self, load_case: LoadCase, factor: float) -> None:
         """
         Add load case to load combination.
 
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         :param factor: The factor for a given load case.
         """
-        self.combinations[load_case] = factor
+        self.load_cases[load_case] = factor
+
+
+class EnvelopeCombination:
+    """
+    Represent an envelope of load cases and (or) load combinations.
+
+    This class is designed to create an envelope of internal forces.
+
+    :param label: A unique identifier for the envelope combination.
+    :ivar cases: A list of :class:`LoadCase` and :class:`LoadCombination`.
+    """
+
+    def __init__(self, label: str, cases: list[LoadCase | LoadCaseCombination]) -> None:
+        """Init the LoadCaseCombination class."""
+        self.label = label
+        self.cases = cases
+
+    def __repr__(self) -> str:
+        """Return a string representation of EnvelopeCombination object."""
+        return f"{self.__class__.__name__}({self.label})"
+
+    def add_case(self, case: LoadCase | LoadCaseCombination) -> None:
+        """
+        Add load case or load combination to load combination.
+
+        :param case: A reference to an instance of the :class:`LoadCase` and :class:`LoadCombination`.
+        """
+        self.cases.append(case)
```

### Comparing `framesss-0.0.2/src/framesss/pre/material.py` & `framesss-0.0.3/src/framesss/pre/material.py`

 * *Files identical despite different names*

### Comparing `framesss-0.0.2/src/framesss/pre/member_1d.py` & `framesss-0.0.3/src/framesss/pre/member_1d.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,25 +13,23 @@
 from framesss.fea.boundary_conditions.element_load import DistributedLoad
 from framesss.fea.boundary_conditions.element_load import ThermalLoad
 from framesss.fea.boundary_conditions.nodal_load import NodalLoad
 from framesss.fea.element_1d import Element1D
 from framesss.fea.node import Node
 from framesss.post.member_1d_results import Member1DResults
 from framesss.pre.member_load import DistributedLoadOnMember
-from framesss.pre.member_load import PointForceOnMember
-from framesss.pre.member_load import PointMomentOnMember
+from framesss.pre.member_load import PointLoadOnMember
 from framesss.pre.member_load import ThermalLoadOnMember
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
     from framesss.fea.analysis.analysis import Analysis
     from framesss.fea.models.model import Model
     from framesss.pre.cases import LoadCase
-    from framesss.pre.material import Material
     from framesss.pre.section import Section
 
 MAX_DISTANCE_BETWEEN_SAMPLING_POINTS = 0.1  # (m)
 NUMERIC_GARBAGE = 1.0e-12
 
 
 def cross(
@@ -54,15 +52,14 @@
     the member's physical and mechanical properties, as well as its loading conditions.
 
     The member is discretized into unique elements at points where discontinuities in the loading occur.
 
     :param label: A user-defined identifier for the member.
     :param element_type: Specifies the type of the element ('navier', 'timoshenko').
     :param nodes: The nodes at the ends of the member.
-    :param material: The material of the member.
     :param section: The cross-section of the member.
     :param hinges: Defines the type of connections at the start and the end of the  member
                    (e.g., fixed, hinged, or semirigid) to model the rotational stiffness accurately.
     :param auxiliary_vector_xy_plane: An auxiliary vector in local xy-plane that defines the local
                                       coordinate system of the member.
     :param analysis: The :class:`Analysis` object.
 
@@ -82,26 +79,24 @@
     """
 
     def __init__(
         self,
         label: str,
         element_type: str,
         nodes: list[Node],
-        material: Material,
         section: Section,
         hinges: list[str] | list[BeamConnection],
         auxiliary_vector_xy_plane: npt.NDArray[np.float64],
         analysis: Analysis,
     ) -> None:
         """Init the Member1D object."""
         self.id: None | int = None
         self.label = label
         self.element_type = Element1DType(element_type)
         self.analysis = analysis
-        self.material = material
         self.section = section
         self.nodes = nodes
         self.hinge_start, self.hinge_end = (BeamConnection(hng) for hng in hinges)
         self.auxiliary_vector_xy_plane = auxiliary_vector_xy_plane
 
         xi, yi, zi = nodes[0].coords
         xf, yf, zf = nodes[1].coords
@@ -123,15 +118,15 @@
         self.cosine_z = cz
 
         self.direction_cosine_matrix = self.get_direction_cosine_matrix()
         self.transformation_matrix = analysis.get_transformation_matrix(self)
 
         self.distributed_loads: list[DistributedLoadOnMember] = []
         self.thermal_loads: list[ThermalLoadOnMember] = []
-        self.point_loads: list[PointForceOnMember | PointMomentOnMember] = []
+        self.point_loads: list[PointLoadOnMember] = []
 
         self.generated_nodes: list[Node] = []
         self.generated_elements: list[Element1D] = []
 
         self.x_user_defined_nodes: npt.NDArray[np.float64] = np.array(
             [0.0, self.length]
         )
@@ -147,15 +142,14 @@
             f"{component:.2f}" for component in self.auxiliary_vector_xy_plane
         )
         return (
             f"{self.__class__.__name__}("
             f"label='{self.label}', "
             f"element_type='{self.element_type}', "
             f"nodes={node_labels}, "
-            f"material='{self.material.label}', "
             f"section='{self.section.label}', "
             f"length={self.length:.2f}, "
             f"hinges={hinge_descriptions}, "
             f"auxiliary_vector_xy_plane=[{aux_vector}])"
         )
 
     @property
@@ -254,98 +248,62 @@
 
         idx = np.where(x == self.x_user_defined_nodes)[0][0]
 
         self.nodes.insert(idx, new_node)
 
         return new_node
 
-    def add_point_force(
+    def add_point_load(
         self,
-        load_components: list[float],
+        load_components: list[float] | npt.NDArray[np.float64],
         load_case: LoadCase,
         x: float,
         coordinate_system: str | LoadCoordinateSystem = LoadCoordinateSystem.GLOBAL,
         coordinate_definition: (
             str | CoordinateDefinition
         ) = CoordinateDefinition.RELATIVE,
     ) -> None:
         """
-        Add a point force to the member at a specified location.
+        Add a point load to the member at a specified location.
 
-        This method creates and adds a :class:`PointForceOnMember` object representing a point force
-        applied to the :class:`Member1D`. The force is specified by its components, the position along
+        This method creates and adds a :class:`PointLoadOnMember` object representing a point load
+        applied to the :class:`Member1D`. The load is specified by its components, the position along
         the member where it is applied, the :class:`LoadCase` it belongs to, and its coordinate system.
 
         The position of the force can be defined relative to the member's length or as an
         absolute value, based on the ``coordinate_definition`` parameter. The method also records
         the position of the force as a discontinuity in the member's load distribution.
 
-        :param load_components: The components of the point force in the format [Fx, Fy, Fz],
+        :param load_components: The components of the point force in the format [Fx, Fy, Fz, Mx, My, Mz],
                                 representing the force in the x, y, and z directions.
         :param load_case: The :class:`LoadCase` to which this point force belongs.
         :param x: The position along the member's length where the force is applied.
                   This can be a relative value (0 to 1) or an absolute value.
         :param coordinate_system: The coordinate system in which the force components are
                                   defined. Can be 'global' or 'local', or an instance
                                   of :class:`LoadCoordinateSystem`. Default to ``GLOBAL``.
         :param coordinate_definition: Defines how the position 'x' is interpreted, either
                                       as 'relative' to the member's length or as an 'absolute'
                                       value. Can be an instance of :class:`CoordinateDefinition`.
                                       Default to ``RELATIVE``.
         """
-        new_force = PointForceOnMember(
+        new_load = PointLoadOnMember(
             self,
             load_components,
             x,
             load_case,
             coordinate_system,
             coordinate_definition,
         )
-        self.x_discontinuities = np.append(self.x_discontinuities, new_force.x)
-        self.point_loads.append(new_force)
-
-    def add_point_moment(
-        self,
-        load_components: list[float],
-        load_case: LoadCase,
-        x: float,
-        coordinate_definition: (
-            str | CoordinateDefinition
-        ) = CoordinateDefinition.RELATIVE,
-    ) -> None:
-        """
-        Add a point moment to the structural member at a specified location.
-
-        This method creates and adds a :class:`PointMomentOnMember` object representing a point moment
-        applied to the :class:`Member1D`. The moment is specified by its components, the position along
-        the member where it is applied and the :class:`LoadCase` it belongs to.
-
-        The position of the moment can be defined relative to the member's length or as an
-        absolute value, based on the ``coordinate_definition`` parameter. The method also records
-        the position of the moment as a discontinuity in the member's load distribution.
-
-        :param load_components: The components of the point force in the format [Fx, Fy, Fz],
-                                representing the force in the x, y, and z directions.
-        :param load_case: The :class:`LoadCase` to which this point force belongs.
-        :param x: The position along the member's length where the force is applied.
-                  This can be a relative value (0 to 1) or an absolute value.
-        :param coordinate_definition: Defines how the position 'x' is interpreted, either
-                                      as 'relative' to the member's length or as an 'absolute'
-                                      value. Can be an instance of :class:`CoordinateDefinition`.
-                                      Default to ``RELATIVE``.
-        """
-        new_moment = PointMomentOnMember(
-            self, load_components, x, load_case, coordinate_definition
-        )
-        self.x_discontinuities = np.append(self.x_discontinuities, new_moment.x)
-        self.point_loads.append(new_moment)
+        self.x_discontinuities = np.append(self.x_discontinuities, new_load.x)
+        self.point_loads.append(new_load)
 
     def add_distributed_load(
         self,
-        load_components: list[float],
+        load_components: list[float] | npt.NDArray[np.float64],
         load_case: LoadCase,
         x_start: float = 0.0,
         x_end: float = 1.0,
         coordinate_system: str | LoadCoordinateSystem = LoadCoordinateSystem.GLOBAL,
         location: str | DistributedLoadLocation = DistributedLoadLocation.LENGTH,
         coordinate_definition: (
             str | CoordinateDefinition
@@ -390,15 +348,15 @@
         )
         self.x_discontinuities = np.append(self.x_discontinuities, new_udl.x_start)
         self.x_discontinuities = np.append(self.x_discontinuities, new_udl.x_end)
         self.distributed_loads.append(new_udl)
 
     def add_thermal_load(
         self,
-        temperature_gradients: list[float],
+        temperature_gradients: list[float] | npt.NDArray[np.float64],
         load_case: LoadCase,
         x_start: float = 0.0,
         x_end: float = 1.0,
         coordinate_definition: (
             str | CoordinateDefinition
         ) = CoordinateDefinition.RELATIVE,
     ) -> None:
@@ -524,17 +482,14 @@
 
         This method iterates through each point load defined for the member and assigns
         it to the appropriate generated node based on the load's position.
 
         The method checks if a nodal load already exists for each node in the relevant load
         case. If not, it initializes a new :class:`NodalLoad` object. It then adds the load
         components from the point load to this nodal load.
-
-        :raises TypeError: If the point load type is not recognized (not a PointForceOnMember
-                             or PointMomentOnMember).
         """
         # assign point loads (forces and moments) to generated nodes
         for point_load in self.point_loads:
             idx = np.where(self.x_discontinuities == point_load.x)[0][0]
 
             node = self.generated_nodes[idx]
 
@@ -542,23 +497,16 @@
             if not point_load.load_case.nodal_loads.get(node):
                 # If not, create a new NodalLoad instance for this node
                 point_load.load_case.nodal_loads[node] = NodalLoad()
 
             nodal_load = point_load.load_case.nodal_loads[node]
 
             # Update the NodalLoad components for this node in the given LoadCase
-            if isinstance(point_load, PointForceOnMember):
-                nodal_load.load_components[:3] += point_load.components_global
-            elif isinstance(point_load, PointMomentOnMember):
-                nodal_load.load_components[3:] += point_load.load_components
-            else:
-                raise TypeError(
-                    f"Unrecognized point load type: {type(point_load).__name__}. "
-                    f"Expected PointForceOnMember or PointMomentOnMember."
-                )
+
+            nodal_load.load_components += point_load.components_global
 
     def assign_distributed_loads(self) -> None:
         """
         Assign distributed loads to the appropriate elements generated along the member.
 
         This method iterates over each distributed load defined for the member. For each
         distributed load, it identifies the elements that fall within
```

### Comparing `framesss-0.0.2/src/framesss/pre/member_load.py` & `framesss-0.0.3/src/framesss/pre/member_load.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,47 +16,47 @@
     from framesss.pre.member_1d import Member1D
 
 
 COORDINATE_DEFINITIONS = [CoordinateDefinition.ABSOLUTE, CoordinateDefinition.RELATIVE]
 LOAD_COORDINATE_SYSTEMS = [LoadCoordinateSystem.LOCAL, LoadCoordinateSystem.GLOBAL]
 
 
-class PointForceOnMember:
+class PointLoadOnMember:
     """
-    Represents a point force acting on a member.
+    Represents a point load (forces and moments) acting on a member.
 
-    This class represents a point force applied to a member, allowing specification of the
-    force's magnitude and direction, its position along the member, and the coordinate
+    This class represents a point load applied to a member, allowing specification of the
+    load's magnitude and direction, its position along the member, and the coordinate
     system in which the force components are defined.
 
     :param member: A reference to an instance of the :class:`Member1D` class, representing
                    the member on which the force is acting.
-    :param load_components: A list of force components [Fx, Fy, Fz].
+    :param load_components: A list of force components [Fx, Fy, Fz, Mx, My, Mz].
     :param x: The position along the member's local x-axis where the force is applied,
               measured from start node. This value should be within the member's length.
     :param load_case: A reference to an instance of the :class:`LoadCase` class, representing
                       the load case to which this force belongs.
     :param coordinate_system: The coordinate system in which the provided load
                               components are defined. Should be either 'global' or 'local',
                               as defined in :class:`LoadCoordinateSystem`.
     :param coordinate_definition: Specifies the definition of the position. Should be either
                                   'absolute' or 'relative' as defined in :class:`CoordinateDefinition`.
     """
 
     def __init__(
         self,
         member: Member1D,
-        load_components: list[float],
+        load_components: list[float] | npt.NDArray[np.float64],
         x: float,
         load_case: LoadCase,
         coordinate_system: str | LoadCoordinateSystem,
         coordinate_definition: str | CoordinateDefinition,
     ) -> None:
         """
-        Init the PointForceOnMember class.
+        Init the PointLoadOnMember class.
 
         :raises ValueError: If the position 'x' is outside the interval of the member's length.
         """
         self.member = member
 
         if coordinate_definition == CoordinateDefinition.RELATIVE:
             x *= member.length
@@ -77,15 +77,15 @@
 
         self.components_global, self.components_local = self.set_load_components(
             np.array(load_components), coordinate_system
         )
         self.load_case = load_case
 
     def __repr__(self) -> str:
-        """Return a string representation of PointForceOnMember class."""
+        """Return a string representation of PointLoadOnMember class."""
         local_components_str = ", ".join(
             f"{comp:.2f}" for comp in self.components_local
         )
         global_components_str = ", ".join(
             f"{comp:.2f}" for comp in self.components_global
         )
         return (
@@ -101,29 +101,33 @@
         self,
         load_components: npt.NDArray[np.float64],
         coordinate_system: str | LoadCoordinateSystem,
     ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
         """
         Transform the load components based on the specified coordinate system.
 
-        This method takes the components of a point force and transforms them between the
+        This method takes the components of a point load and transforms them between the
         global coordinate system and local coordinate system of the member.
 
-        :param load_components: Array of the force components [Fx, Fy, Fz].
+        :param load_components: Array of the force components [Fx, Fy, Fz, Mx, My, Mz].
         :param coordinate_system: The coordinate system in which the provided load
                                   components are defined. Should be either 'global' or 'local',
                                   as defined in LoadCoordinateSystem. Defaults to 'global'.
 
-        :return: A tuple containing two np.ndarray objects: the first array is the force
+        :return: A tuple containing two np.ndarray objects: the first array is the load
                  components in the global coordinate system, and the second is in the local
                  coordinate system.
 
         :raises ValueError: If the specified coordinate system is neither 'global' nor 'local'.
         """
-        transformation_matrix = self.member.direction_cosine_matrix
+        load_components = np.array(load_components)
+
+        transformation_matrix = sp.linalg.block_diag(
+            self.member.direction_cosine_matrix, self.member.direction_cosine_matrix
+        )
 
         if coordinate_system == LoadCoordinateSystem.GLOBAL:
             components_global = load_components
             components_local = transformation_matrix @ load_components
 
         elif coordinate_system == LoadCoordinateSystem.LOCAL:
             components_global = transformation_matrix.T @ load_components
@@ -134,77 +138,14 @@
                 f"Invalid load coordinate system: '{coordinate_system}'.\n"
                 f"Valid options are: {LOAD_COORDINATE_SYSTEMS}"
             )
 
         return components_global, components_local
 
 
-class PointMomentOnMember:
-    """
-    Represents a point moment acting on a member.
-
-    This class represents a point moment applied to a member, allowing specification of the
-    moment's magnitude and its position along the member.
-
-    :param member: A reference to an instance of the :class:`Member1D` class, representing
-                   the member on which the moment is acting.
-    :param load_components: A list of moment components [Mx, My, Mz].
-    :param x: The position along the member's local x-axis where the moment is applied,
-              measured from start node. This value should be within the member's length.
-    :param load_case: A reference to an instance of the :class:`LoadCase` class, representing
-                      the load case to which this moment belongs.
-    :param coordinate_definition: Specifies the definition of the position. Should be either
-                                  'absolute' or 'relative' as defined in :class:`CoordinateDefinition`.
-
-    :raises ValueError: If the position 'x' is outside the interval of the member's length.
-    """
-
-    def __init__(
-        self,
-        member: Member1D,
-        load_components: list[float],
-        x: float,
-        load_case: LoadCase,
-        coordinate_definition: str | CoordinateDefinition,
-    ) -> None:
-        """Init the PointMomentOnMember class."""
-        self.member = member
-
-        if coordinate_definition == CoordinateDefinition.RELATIVE:
-            x *= member.length
-        elif coordinate_definition == CoordinateDefinition.ABSOLUTE:
-            pass
-        else:
-            raise ValueError(
-                f"Unknown coordinate definition: '{coordinate_definition}.'"
-                f"Valid options are: {COORDINATE_DEFINITIONS}."
-            )
-
-        if 0 <= x <= member.length:
-            self.x = x
-        else:
-            raise ValueError(
-                f"Position of the moment is outside the beam interval [{0, member.length}], x: '{x}'."
-            )
-
-        self.load_components = np.array(load_components)
-        self.load_case = load_case
-
-    def __repr__(self) -> str:
-        """Return a string representation of the PointMomentOnMember class."""
-        components_str = ", ".join(f"{comp:.2f}" for comp in self.load_components)
-        return (
-            f"{self.__class__.__name__}("
-            f"member='{self.member.label}', "
-            f"load_components=[{components_str}], "
-            f"x={self.x:.2f}, "
-            f"load_case='{self.load_case.label}'"
-        )
-
-
 class DistributedLoadOnMember:
     """
     Represents a distributed uniform or trapezoidal load acting on a member.
 
     This class represents a distributed load applied to a member, allowing specification of the
     force's magnitude and direction, its position along the member, and the coordinate
     system in which the force components are defined.
@@ -230,15 +171,15 @@
                      For 'local' coordinate_system, the only option is 'length'.
                      For 'global' coordinate_system, the options are 'length' and 'projection'.
     """
 
     def __init__(
         self,
         member: Member1D,
-        load_components: list[float],
+        load_components: list[float] | npt.NDArray[np.float64],
         x_start: float,
         x_end: float,
         load_case: LoadCase,
         coordinate_system: str | LoadCoordinateSystem,
         location: str | DistributedLoadLocation,
         coordinate_definition: str | CoordinateDefinition,
     ) -> None:
@@ -422,15 +363,15 @@
     :param coordinate_definition: Specifies the definition of the position. Should be either
                                   'absolute' or 'relative' as defined in :class:`CoordinateDefinition`.
     """
 
     def __init__(
         self,
         member: Member1D,
-        temperature_gradients: list[float],
+        temperature_gradients: list[float] | npt.NDArray[np.float64],
         x_start: float,
         x_end: float,
         load_case: LoadCase,
         coordinate_definition: str | CoordinateDefinition,
     ) -> None:
         """
         Init the ThermalLoadOnMember class.
```

### Comparing `framesss-0.0.2/src/framesss/solvers/linear_static.py` & `framesss-0.0.3/src/framesss/solvers/linear_static.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,30 +95,33 @@
 
         This method systematically processes the structural model, performing steps from discretization
         of members to the calculation of internal forces and displacements for each load case.
         It supports verbose output to monitor the progress through these steps.
 
         :param verbose: If True, detailed progress of each analysis step is printed to the console.
         """
+        steps_init = 6
         steps_cases = len(self.model.load_cases) * 7
-        steps_combs = len(self.model.load_combinations) * 4
-        n_steps = 7 + steps_cases + steps_combs
+        steps_combs = len(self.model.load_combinations) * 3
+        steps_envelopes = len(self.model.envelopes) * 1
+        n_steps = steps_init + steps_cases + steps_combs + steps_envelopes
 
         if verbose:
             print(f"1/{n_steps} : Preparing fea data...")
 
         self.model.discretize_members()
         self.model.setup_fictitious_rotation_constraints(True)
 
         if verbose:
             print(f"2/{n_steps} : Number of equations: {self.model.neq}...")
 
         if verbose:
             print(
-                f"3/{n_steps} : Initialization of global stiffness matrix and force vectors..."
+                f"3/{n_steps}"
+                f" : Initialization of global stiffness matrix and force vectors..."
             )
         self.init_global_matrices_vectors()
 
         if verbose:
             print(f"4/{n_steps} : Generating global DoFs numbering matrix...")
         self.model.analysis.setup_dof_numbers(self.model)
 
@@ -131,76 +134,94 @@
             print(f"6/{n_steps} : Assembling global stiffness matrix...")
         self.assemble_global_stiffness_matrix()
         self.model.analysis.assemble_spring_stiffness(self.model)
 
         for i, load_case in enumerate(self.model.load_cases):
             if verbose:
                 print(
-                    f"{i*7 + 7}/{n_steps} : Applying prescribed displacements for load case: '{load_case.label}..."
+                    f"{i*7 + steps_init + 1}/{n_steps}"
+                    f" : Applying prescribed displacements for load case: '{load_case.label}..."
                 )
             self.model.analysis.apply_prescribed_displacements(self.model, load_case)
 
             if verbose:
                 print(
-                    f"{i*7 + 8}/{n_steps} : Applying nodal forces for load case: '{load_case.label}'..."
+                    f"{i*7 + steps_init + 2}/{n_steps}"
+                    f" : Applying nodal forces for load case: '{load_case.label}'..."
                 )
             self.model.analysis.assemble_nodal_loads(self.model, load_case)
 
             if verbose:
                 print(
-                    f"{i*7 + 9}/{n_steps} : Applying member forces for load case: '{load_case.label}'..."
+                    f"{i*7 + steps_init + 3}/{n_steps}"
+                    f" : Applying member forces for load case: '{load_case.label}'..."
                 )
             load_case.assemble_equivalent_nodal_loads()
 
             if verbose:
                 print(
-                    f"{i*7 + 10}/{n_steps} : Solving load case: '{load_case.label}'..."
+                    f"{i*7 + steps_init + 3}/{n_steps}"
+                    f" : Solving load case: '{load_case.label}'..."
                 )
             self.solve_load_case(load_case)
 
             if verbose:
                 print(
-                    f"{i*7 + 11}/{n_steps} : Computing reactions for load case: '{load_case.label}'..."
+                    f"{i*7 + steps_init + 4}/{n_steps}"
+                    f" : Computing reactions for load case: '{load_case.label}'..."
                 )
             self.save_displacements(load_case)
             self.save_reactions(load_case)
 
             if verbose:
                 print(
-                    f"{i*7 + 12}/{n_steps} : Computing internal forces for load case: '{load_case.label}'..."
+                    f"{i*7 + steps_init + 5}/{n_steps}"
+                    f" : Computing internal forces for load case: '{load_case.label}'..."
                 )
             self.save_element_internal_forces(load_case)
             self.save_member_internal_forces(load_case)
 
             if verbose:
                 print(
-                    f"{i*7 + 13}/{n_steps} : Computing internal displacements for load case: '{load_case.label}'..."
+                    f"{i*7 + steps_init + 6}/{n_steps}"
+                    f" : Computing internal displacements for load case: '{load_case.label}'..."
                 )
             self.save_member_internal_displacements(load_case)
 
             load_case.is_solved = True
 
         for i, load_combination in enumerate(self.model.load_combinations):
             if verbose:
                 print(
-                    f"{i*7 + steps_cases + 1}/{n_steps} : Computing internal forces for load combination: "
+                    f"{i*3 + steps_init + steps_cases + 1}/{n_steps}"
+                    f" : Computing internal forces for load combination: "
                     f"'{load_combination.label}'..."
                 )
             self.save_displacements_combination(load_combination)
             self.save_reactions_combination(load_combination)
 
             if verbose:
                 print(
-                    f"{i*7 + steps_cases + 2}/{n_steps} : Computing internal forces for load combination: "
+                    f"{i*3 + steps_init + steps_cases + 2}/{n_steps}"
+                    f" : Computing internal forces for load combination: "
                     f"'{load_combination.label}'..."
                 )
-            self.save_member_internal_forces_combination(load_combination)
+            self.save_member_internal_forces(load_combination)
 
             if verbose:
                 print(
-                    f"{i*7 + steps_cases + 3}/{n_steps} : Computing internal displacements for load combination: "
+                    f"{i*3 + steps_init + steps_cases + 3}/{n_steps}"
+                    f" : Computing internal displacements for load combination: "
                     f"'{load_combination.label}'..."
                 )
             self.save_member_internal_displacements_combination(load_combination)
 
+        for i, envelope in enumerate(self.model.envelopes):
+            if verbose:
+                print(
+                    f"{i*1 + steps_init + steps_cases + steps_combs + 1}/{n_steps}"
+                    f" : Computing internal forces for envelope: {envelope.label}..."
+                )
+            self.save_envelope_internal_forces(envelope)
+
         if verbose:
             print(f"{n_steps}/{n_steps} : Analysis successfully finished.")
```

### Comparing `framesss-0.0.2/src/framesss/solvers/solver.py` & `framesss-0.0.3/src/framesss/solvers/solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import numpy as np
 import scipy as sp  # type: ignore[import-untyped]
 
 if TYPE_CHECKING:
     import numpy.typing as npt
 
     from framesss.fea.models.model import Model
+    from framesss.pre.cases import EnvelopeCombination
     from framesss.pre.cases import LoadCase
-    from framesss.pre.cases import LoadCombination
+    from framesss.pre.cases import LoadCaseCombination
 
 
 class Solver(ABC):
     """
     Class for a finite element solver.
 
     An abstract base class that outlines the structure and requirements of solver
@@ -117,48 +118,39 @@
 
             if thermal_load := load_case.element_thermal_loads.get(elem):
                 fel += self.model.analysis.get_fixed_end_forces(thermal_load)
 
             # Assemble member internal force arrays
             self.model.analysis.assemble_internal_forces(elem, load_case, fel)
 
-    def save_member_internal_forces(self, load_case: LoadCase) -> None:
+    def save_member_internal_forces(self, case: LoadCase | LoadCaseCombination) -> None:
         """
         Save the internal forces for each member in the model under a specified load case.
 
         This method iterates over all members in the model and invokes a process to calculate and store
         the internal stresses (forces and moments) experienced by each member due to the applied loads
         in the given load case. The calculation is performed by the `save_internal_stresses_on_member`
         method of the analysis model, which takes into account both global and local effects to
         accurately determine the stresses along each member.
 
-        :param load_case: A reference to an instance of the :class:`LoadCase` class.
+        :param case: A reference to an instance of the :class:`LoadCase` or :class:`LoadCaseCombination` class.
         """
         for member in self.model.members:
-            self.model.analysis.save_internal_stresses_on_member(member, load_case)
+            self.model.analysis.save_internal_stresses(member, case)
 
-    # TODO: docstring
-    def save_member_internal_forces_combination(
-        self, load_combination: LoadCombination
-    ) -> None:
+    def save_envelope_internal_forces(self, envelope: EnvelopeCombination) -> None:
         """
-        Save the internal forces for each member in the model under a specified load case.
+        Save the envelope of internal forces for each member.
 
         This method iterates over all members in the model and invokes a process to calculate and store
-        the internal stresses (forces and moments) experienced by each member due to the applied loads
-        in the given load case. The calculation is performed by the `save_internal_stresses_on_member`
-        method of the analysis model, which takes into account both global and local effects to
-        accurately determine the stresses along each member.
-
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        the envelope of internal stresses (forces and moments) experienced by each member due to the applied
+        loads.
         """
         for member in self.model.members:
-            self.model.analysis.save_internal_stresses_on_member_combination(
-                member, load_combination
-            )
+            self.model.analysis.save_envelope_stresses(member, envelope)
 
     def save_member_internal_displacements(self, load_case: LoadCase) -> None:
         """
         Save the displacements for each member in the model under a specified load case.
 
         This method iterates over all members in the model and invokes a process to calculate and store
         the displacements (translations and rotations) experienced by each member due to the applied loads
@@ -168,26 +160,26 @@
 
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         """
         for member in self.model.members:
             self.model.analysis.save_internal_displacements_on_member(member, load_case)
 
     def save_member_internal_displacements_combination(
-        self, load_combination: LoadCombination
+        self, load_combination: LoadCaseCombination
     ) -> None:
         """
         Save the displacements for each member in the model under a specified load case.
 
         This method iterates over all members in the model and invokes a process to calculate and store
         the displacements (translations and rotations) experienced by each member due to the applied loads
         in the given load case. The calculation is performed by the `save_internal_displacements_on_member`
         method of the analysis model, which takes into account both global and local effects to
         accurately determine the stresses along each member.
 
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
         """
         for member in self.model.members:
             self.model.analysis.save_internal_displacements_on_member_combination(
                 member, load_combination
             )
 
     def save_reactions(self, load_case: LoadCase) -> None:
@@ -199,22 +191,22 @@
 
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         """
         for node in self.model.nodes:
             self.model.analysis.save_reactions(node, load_case)
 
     # TODO: docstring
-    def save_reactions_combination(self, load_combination: LoadCombination) -> None:
+    def save_reactions_combination(self, load_combination: LoadCaseCombination) -> None:
         """
         Save the reaction forces and moments for each node in the model under a specified load case.
 
         This method iterates over all nodes in the model, retrieving and storing the reaction forces
         and moments resulting from the applied loads and constraints defined by the load case.
 
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
         """
         for node in self.model.nodes:
             self.model.analysis.save_reactions_combination(node, load_combination)
 
     def save_displacements(self, load_case: LoadCase) -> None:
         """
         Save the displacements for each node in the model under a specified load case.
@@ -224,22 +216,24 @@
 
         :param load_case: A reference to an instance of the :class:`LoadCase` class.
         """
         for node in self.model.nodes:
             self.model.analysis.save_displacements(node, load_case)
 
     # TODO: docstring
-    def save_displacements_combination(self, load_combination: LoadCombination) -> None:
+    def save_displacements_combination(
+        self, load_combination: LoadCaseCombination
+    ) -> None:
         """
         Save the displacements for each node in the model under a specified load case.
 
         This method iterates over all nodes in the model, retrieving and storing the displacements
         (translations and rotations) resulting from the applied loads and constraints defined by the load case.
 
-        :param load_combination: A reference to an instance of the :class:`LoadCombination` class.
+        :param load_combination: A reference to an instance of the :class:`LoadCaseCombination` class.
         """
         for node in self.model.nodes:
             self.model.analysis.save_displacements_combination(node, load_combination)
 
     @abstractmethod
     def solve_load_case(self, load_case: LoadCase) -> None:
         """Solve the system of equilibrium equations for a specific load case."""
```

### Comparing `framesss-0.0.2/src/framesss/utils.py` & `framesss-0.0.3/src/framesss/utils.py`

 * *Files identical despite different names*

### Comparing `framesss-0.0.2/PKG-INFO` & `framesss-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: framesss
-Version: 0.0.2
+Version: 0.0.3
 Summary: framesss
 Home-page: https://github.com/DanBeranek/framesss
 License: MIT
 Author: Daniel Beranek
 Author-email: daniel.beraanek@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

