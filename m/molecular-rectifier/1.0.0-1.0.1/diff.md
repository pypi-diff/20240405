# Comparing `tmp/molecular_rectifier-1.0.0.tar.gz` & `tmp/molecular_rectifier-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecular_rectifier-1.0.0.tar", last modified: Wed Feb 21 13:35:14 2024, max compression
+gzip compressed data, was "molecular_rectifier-1.0.1.tar", last modified: Fri Apr  5 10:22:16 2024, max compression
```

## Comparing `molecular_rectifier-1.0.0.tar` & `molecular_rectifier-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-21 13:35:14.660146 molecular_rectifier-1.0.0/
--rw-r--r--   0 user       (502) staff       (20)     1069 2023-06-07 10:44:21.000000 molecular_rectifier-1.0.0/LICENSE
--rw-r--r--   0 user       (502) staff       (20)     2190 2024-02-21 13:35:14.657958 molecular_rectifier-1.0.0/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)     1783 2023-06-07 11:09:49.000000 molecular_rectifier-1.0.0/README.md
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-21 13:35:14.643481 molecular_rectifier-1.0.0/molecular_rectifier/
--rw-r--r--   0 user       (502) staff       (20)     5576 2024-02-21 13:33:22.000000 molecular_rectifier-1.0.0/molecular_rectifier/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     7998 2023-06-07 10:44:21.000000 molecular_rectifier-1.0.0/molecular_rectifier/_base.py
--rw-r--r--   0 user       (502) staff       (20)     2567 2023-06-07 10:44:21.000000 molecular_rectifier-1.0.0/molecular_rectifier/_odd.py
--rw-r--r--   0 user       (502) staff       (20)     2939 2023-06-07 10:44:21.000000 molecular_rectifier-1.0.0/molecular_rectifier/_overclose.py
--rw-r--r--   0 user       (502) staff       (20)    17724 2023-06-07 10:44:21.000000 molecular_rectifier-1.0.0/molecular_rectifier/_ring.py
--rw-r--r--   0 user       (502) staff       (20)    17244 2023-06-07 10:44:21.000000 molecular_rectifier-1.0.0/molecular_rectifier/_valence.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-02-21 13:35:14.656731 molecular_rectifier-1.0.0/molecular_rectifier.egg-info/
--rw-r--r--   0 user       (502) staff       (20)     2190 2024-02-21 13:35:14.000000 molecular_rectifier-1.0.0/molecular_rectifier.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      424 2024-02-21 13:35:14.000000 molecular_rectifier-1.0.0/molecular_rectifier.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2024-02-21 13:35:14.000000 molecular_rectifier-1.0.0/molecular_rectifier.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)        6 2024-02-21 13:35:14.000000 molecular_rectifier-1.0.0/molecular_rectifier.egg-info/requires.txt
--rw-r--r--   0 user       (502) staff       (20)       20 2024-02-21 13:35:14.000000 molecular_rectifier-1.0.0/molecular_rectifier.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)       38 2024-02-21 13:35:14.660229 molecular_rectifier-1.0.0/setup.cfg
--rw-r--r--   0 user       (502) staff       (20)     1122 2024-02-21 13:33:22.000000 molecular_rectifier-1.0.0/setup.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:16.882505 molecular_rectifier-1.0.1/
+-rw-r--r--   0 user       (502) staff       (20)     1069 2023-06-07 10:44:21.000000 molecular_rectifier-1.0.1/LICENSE
+-rw-r--r--   0 user       (502) staff       (20)     2190 2024-04-05 10:22:16.881114 molecular_rectifier-1.0.1/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)     1783 2023-06-07 11:09:49.000000 molecular_rectifier-1.0.1/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:16.853810 molecular_rectifier-1.0.1/molecular_rectifier/
+-rw-r--r--   0 user       (502) staff       (20)     5614 2024-04-04 15:20:28.000000 molecular_rectifier-1.0.1/molecular_rectifier/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     8056 2024-04-04 15:20:28.000000 molecular_rectifier-1.0.1/molecular_rectifier/_base.py
+-rw-r--r--   0 user       (502) staff       (20)     4156 2024-04-05 10:20:47.000000 molecular_rectifier-1.0.1/molecular_rectifier/_odd.py
+-rw-r--r--   0 user       (502) staff       (20)     2979 2024-04-04 15:20:28.000000 molecular_rectifier-1.0.1/molecular_rectifier/_overclose.py
+-rw-r--r--   0 user       (502) staff       (20)    17817 2024-04-04 15:20:28.000000 molecular_rectifier-1.0.1/molecular_rectifier/_ring.py
+-rw-r--r--   0 user       (502) staff       (20)    17357 2024-04-04 15:47:19.000000 molecular_rectifier-1.0.1/molecular_rectifier/_valence.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-04-05 10:22:16.879332 molecular_rectifier-1.0.1/molecular_rectifier.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)     2190 2024-04-05 10:22:16.000000 molecular_rectifier-1.0.1/molecular_rectifier.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      424 2024-04-05 10:22:16.000000 molecular_rectifier-1.0.1/molecular_rectifier.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2024-04-05 10:22:16.000000 molecular_rectifier-1.0.1/molecular_rectifier.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)        6 2024-04-05 10:22:16.000000 molecular_rectifier-1.0.1/molecular_rectifier.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)       20 2024-04-05 10:22:16.000000 molecular_rectifier-1.0.1/molecular_rectifier.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)       38 2024-04-05 10:22:16.882785 molecular_rectifier-1.0.1/setup.cfg
+-rw-r--r--   0 user       (502) staff       (20)     1122 2024-04-05 10:17:54.000000 molecular_rectifier-1.0.1/setup.py
```

### Comparing `molecular_rectifier-1.0.0/LICENSE` & `molecular_rectifier-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `molecular_rectifier-1.0.0/PKG-INFO` & `molecular_rectifier-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular_rectifier
-Version: 1.0.0
+Version: 1.0.1
 Summary: Given an RDKit molecule that does not sanitise, correct it until it does, regardless of the severity of the change.
 Home-page: https://github.com/matteoferla/molecular_rectifier
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
```

### Comparing `molecular_rectifier-1.0.0/README.md` & `molecular_rectifier-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `molecular_rectifier-1.0.0/molecular_rectifier/__init__.py` & `molecular_rectifier-1.0.1/molecular_rectifier/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
-########################################################################################################################
 
+########################################################################################################################
 __doc__ = \
     """
 Fix issue in auto-merging.
     """
 
 __author__ = "Matteo Ferla. [Github](https://github.com/matteoferla)"
 __email__ = "matteo.ferla@gmail.com"
@@ -19,14 +19,15 @@
 from ._ring import _RectifierRing  # fixes rings
 from ._odd import _RectifierOdd  # fixes specific oddities
 from ._valence import _RectifierValence  # fixes valence
 from ._overclose import _RectifierOverclose  # fixes extreme overlaps
 from rdkit import Chem
 from rdkit.Chem import AllChem
 
+
 class Rectifier(_RectifierOverclose, _RectifierRing, _RectifierOdd, _RectifierValence):
     """
     Fixes the nastiness.
 
     Do note that the ``Chem.Mol`` does not get modified in place.
     ``.rwmol`` does and is a Chem.RWMol. The ``.mol`` is a Chem.Mol.
 
@@ -37,15 +38,15 @@
     New atoms with have the bool prop ``_Novel``.
 
     Does not link distant atoms. For that see joining methods in Monster.
 
     >>> Rectifier(mol).fix().mol
     """
 
-    def fix(self, catchErrors:bool=False, iteration:int=0) -> Rectifier:
+    def fix(self, catchErrors: bool = False, iteration: int = 0) -> Rectifier:
         """
         `CatchErrors` is the command in Sanitize, but it is not used there.
         """
         self.log.debug('============== Rectifier fix started =============')
         self.log.debug(self.mol_summary)
         self.absorb_overclose(distance_cutoff=0.8)  # from _RectifierOverclose
         self.log.debug(self.mol_summary)
@@ -106,18 +107,18 @@
         elif iteration == 4:
             problems = Chem.DetectChemistryProblems(self.rwmol)
             for p in problems:
                 if p.GetType() == 'KekulizeException':
                     for i in p.GetAtomIndices():
                         self.log.debug(f'KekulizeException downgrade_ring last resort: {i}')
                         self.downgrade_ring(self.rwmol.GetAtomWithIdx(i), hard=True)
-                        AllChem.AddHs(self.rwmol)
+                        AllChem.AddHs(self.rwmol, addCoords=self.has_conformer)
             self.fix(catchErrors=catchErrors, iteration=iteration)
         else:
-            pass # burn...
+            pass  # burn...
         # check:
         CaughtError = Exception if catchErrors else ()  # noqa Uppercase as its a class
         try:
             self._update_cache(sanitize=False)  # catchErrors is true...
             Chem.SanitizeMol(self.rwmol, catchErrors=False)
         except CaughtError as error:
             self.log.info(f'{error.__class__.__name__}: {error}')
```

### Comparing `molecular_rectifier-1.0.0/molecular_rectifier/_base.py` & `molecular_rectifier-1.0.1/molecular_rectifier/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,19 @@
         if not isinstance(mol, Chem.Mol):
             # anything that is not Chem.Mol or Chem.RWMol
             # isinstance(Chem.RWMol(), Chem.Mol) == True
             raise TypeError('not a molecule')
         # an unsanitised mol has no `.updatePropertyCache`
         # mol.updatePropertyCache(strict=False)
         self.rwmol = Chem.RWMol(mol)
-        self.modifications = []  # keeping track of steps
+        self.modifications = {}  # keeping track of steps
         self._valence_mode = 'max'
         self._iterations_done = 0
         self._subiterations_done = 0
+        self.has_conformer = bool(mol.GetNumConformers())
 
     @property
     def mol(self) -> Chem.Mol:
         return self.rwmol.GetMol()
 
     @property
     def name(self) -> str:
```

### Comparing `molecular_rectifier-1.0.0/molecular_rectifier/_overclose.py` & `molecular_rectifier-1.0.1/molecular_rectifier/_overclose.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,9 +56,9 @@
             for atom in self.rwmol.GetAtoms():
                 if atom.HasProp('DELETE'):
                     self.rwmol.RemoveAtom(atom.GetIdx())
                     break
             else:
                 break
         # store copy (self.mol is property <= .rwmol
-        self.modifications.append(self.mol)
+        self.modifications[f'no_overclose-inter{self._iterations_done}'] = self.mol
```

### Comparing `molecular_rectifier-1.0.0/molecular_rectifier/_ring.py` & `molecular_rectifier-1.0.1/molecular_rectifier/_ring.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,16 @@
         rank = sorted(pairs, key=lambda x: c[x[0]] + c[x[1]], reverse=True)
         if len(rank) > 0:
             idx_a, idx_b = rank[0]
             self.rwmol.RemoveBond(idx_a, idx_b)  # SetBoolProp('_IsRingBond') is not important
             self.log.info(f'Zero-atom bridged ring issue: bond between {idx_a}-{idx_b} removed')
             # re-run:
             self._prevent_conjoined_ring()
-        self.modifications.append(self.mol)  # not self.rwmol as I want a snapshot
+        # not self.rwmol as I want a snapshot:
+        self.modifications[f'no_bridged_rings-inter{self._iterations_done}'] = self.mol
 
     def _get_bridges(self) -> List[Dict[str, Union[Tuple[int]]]]:
         """
         The output includes not only the bridgeheads but the middle ones too
         list of dict shared, ring_atom_A_idxs, ring_atom_A_idxs
         """
         bridge_info = []
@@ -192,15 +193,15 @@
                 self.log.warning(f'This molecule ({self.name}) has a bridge that will be removed')
                 self._prevent_bridge_ring(ring_A)
                 # start from scratch.
                 if iteration < 3:
                     self._prevent_weird_rings(iteration=iteration+1)
                 else:
                     self.log.warning(f'Too many trials to remove bridge.')
-        self.modifications.append(self.mol)  # not self.rwmol as I want a snapshot
+        self.modifications[f'no_weird_rings-inter{self._iterations_done}'] = self.mol # not self.rwmol as I want a snapshot
 
     # ===== Dependencies of prevent weird rings =================================================================================
 
     def _place_between(self, a: int, b: int, aromatic: Optional[bool] = None, atomic_number: int = 6) -> None:
         """
         Places an C atom, possibly of type aromatic, between atom of index a, and of b.
```

### Comparing `molecular_rectifier-1.0.0/molecular_rectifier/_valence.py` & `molecular_rectifier-1.0.1/molecular_rectifier/_valence.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         :return: None
         """
         for bond in self.rwmol.GetBonds():
             if bond.GetBondType().name == 'UNSPECIFIED':
                 self.log.debug(f'Fixing unspecified bond {bond.GetIdx()}')
                 bond.SetBondType(Chem.BondType.SINGLE)
                 # debug:
-                self.modifications.append(self.mol)
+                self.modifications[f'no_unspecificied-inter{self._iterations_done}'] = self.mol
         self._update_cache()
 
     def triage_rings(self) -> None:
         """
         This get run during instantiation. It is the second one run.
         It is also run again by `fix_issues` the third step after a weird valence change.
         Deals with rings.
@@ -72,26 +72,26 @@
             if self._is_aromatic_ring(ring, rings):  # the nonaromatic rings will be done first.
                 for i in ring:
                     self.rwmol.GetAtomWithIdx(i).SetIsAromatic(True)
             else:
                 for i in ring:
                     self.rwmol.GetAtomWithIdx(i).SetIsAromatic(False)
         self._update_cache()
-        self.modifications.append(self.mol)  # may not have changed.
+        self.modifications[f'no_cyclopropane-inter{self._iterations_done}'] = self.mol  # may not have changed.
 
     def fix_issues(self, _previous=None) -> None:
         """
         This get run during instantiation. It is the third and final one run before sanitization.
         Deals with a variety of problems.
         It calls itself until no problems according to `Chem.DetectChemistryProblems` exits.
         It is a bit shoddy and any oddity likely steps from here. TODO
 
         :return: None
         """
-        self.modifications.append(self.mol)  # may not have changed.
+        self.modifications[f'issue-inter{self._iterations_done}'] = self.mol  # may not have changed.
         problems = Chem.DetectChemistryProblems(self.rwmol)
         if self._iterations_done > 100:
             self.log.error(f'Iterations maxed out!')
             return None
         elif self._subiterations_done > 5:
             self.log.error(f'Unfixable')
             return None
@@ -368,20 +368,20 @@
         else:
             return self.fix_valence(i)
 
     def _adjust_Hs(self):
         for atom in self.rwmol.GetAtoms():
             atom.SetNumRadicalElectrons(0)
         self._update_cache(sanitize=False)
-        idxs = [i for ring in self._get_ring_info('atom') for i in ring]
-        for i in idxs:
-            # atom: Chem.Atom = self.rwmol.GetAtomWithIdx(i)
-            # self.fix_valence(i)
-            pass
-        mol = AllChem.AddHs(self.rwmol, addCoords=bool(self.rwmol.GetNumConformers()))
+        # idxs = [i for ring in self._get_ring_info('atom') for i in ring]
+        # for i in idxs:
+        #     # atom: Chem.Atom = self.rwmol.GetAtomWithIdx(i)
+        #     # self.fix_valence(i)
+        #     pass
+        mol = AllChem.AddHs(self.rwmol, addCoords=self.has_conformer)
         self.rwmol = Chem.RWMol(mol)
 
     def _preemptive_protonate(self):
         """
         This is a debug test in essence as it's a bad idea
         """
         for atom in self.rwmol.GetAtoms():
```

### Comparing `molecular_rectifier-1.0.0/molecular_rectifier.egg-info/PKG-INFO` & `molecular_rectifier-1.0.1/molecular_rectifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molecular-rectifier
-Version: 1.0.0
+Version: 1.0.1
 Summary: Given an RDKit molecule that does not sanitise, correct it until it does, regardless of the severity of the change.
 Home-page: https://github.com/matteoferla/molecular_rectifier
 Author: Matteo Ferla
 Author-email: matteo.ferla@gmail.com
 License: MIT
 Requires-Python: >3.6
 Description-Content-Type: text/markdown
```

### Comparing `molecular_rectifier-1.0.0/setup.py` & `molecular_rectifier-1.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     __doc__ = f.read()
 descr = __doc__.split('\n')[1] # non-title line.
 
 # ------------ Setup ---------------------------------------------------------------------------------------------------
 
 setup(
     name='molecular_rectifier',
-    version='1.0.0',
+    version='1.0.1',
     python_requires='>3.6',
     packages=find_packages(),
     install_requires=['rdkit'],
     url='https://github.com/matteoferla/molecular_rectifier',
     license='MIT',
     author='Matteo Ferla',
     author_email='matteo.ferla@gmail.com',
```

