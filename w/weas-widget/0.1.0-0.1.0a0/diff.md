# Comparing `tmp/weas_widget-0.1.0.tar.gz` & `tmp/weas_widget-0.1.0a0.tar.gz`

## Comparing `weas_widget-0.1.0.tar` & `weas_widget-0.1.0a0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/__init__.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/atoms_viewer.py
--rw-r--r--   0        0        0     1933 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/base_class.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/base_widget.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/camera.py
--rw-r--r--   0        0        0     5937 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/utils.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/weas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/plugins/__init__.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/plugins/instanced_mesh_pritimive.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/plugins/isosurface.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/plugins/vector_field.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/static/widget.css
--rw-r--r--   0        0        0   699573 2020-02-02 00:00:00.000000 weas_widget-0.1.0/src/weas_widget/static/widget.js
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 weas_widget-0.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 weas_widget-0.1.0/LICENSE
--rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 weas_widget-0.1.0/README.md
--rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 weas_widget-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     8078 2020-02-02 00:00:00.000000 weas_widget-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/__init__.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/atoms_viewer.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/base_class.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/base_widget.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/camera.py
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/data.py
+-rw-r--r--   0        0        0     5111 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/utils.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/weas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/plugins/__init__.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/plugins/instanced_mesh_pritimive.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/plugins/isosurface.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/plugins/vector_field.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/static/widget.css
+-rw-r--r--   0        0        0   698930 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/src/weas_widget/static/widget.js
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/LICENSE
+-rw-r--r--   0        0        0     5099 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/README.md
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0     8080 2020-02-02 00:00:00.000000 weas_widget-0.1.0a0/PKG-INFO
```

### Comparing `weas_widget-0.1.0/src/weas_widget/atoms_viewer.py` & `weas_widget-0.1.0a0/src/weas_widget/atoms_viewer.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,21 +50,21 @@
         # separate spin up and down, add two vector fields
         if "moment" in atoms["attributes"]["atom"]:
             moment = atoms["attributes"]["atom"]["moment"]
             spin_up = [i for i, m in enumerate(moment) if m > 0]
             spin_down = [i for i, m in enumerate(moment) if m < 0]
             self.vf.settings = [
                 {
-                    "origins": [atoms["positions"][i] for i in spin_up],
-                    "vectors": [[0, 0, moment[i]] for i in spin_up],
+                    "origins": atoms["positions"][spin_up],
+                    "vectors": [[0, 0, m] for m in moment[spin_up]],
                     "color": "blue",
                 },
                 {
-                    "origins": [atoms["positions"][i] for i in spin_down],
-                    "vectors": [[0, 0, moment[i]] for i in spin_down],
+                    "origins": atoms["positions"][spin_down],
+                    "vectors": [[0, 0, m] for m in moment[spin_down]],
                     "color": "red",
                 },
             ]
 
     def draw(self):
         """Redraw the widget."""
         self._widget.send_js_task({"name": "avr.drawModels", "kwargs": {}})
```

### Comparing `weas_widget-0.1.0/src/weas_widget/base_widget.py` & `weas_widget-0.1.0a0/src/weas_widget/base_widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,16 +49,20 @@
     cameraRotation = tl.List().tag(sync=True)
     cameraLookAt = tl.List().tag(sync=True)
     # task
     js_task = tl.Dict({}).tag(sync=True)
     python_task = tl.Dict({}).tag(sync=True)
     debug = tl.Bool(False).tag(sync=True)
 
-    def __init__(self, **kwargs):
+    def __init__(self, from_ase=None, from_pymatgen=None, **kwargs):
         super().__init__(**kwargs)
+        if from_ase is not None:
+            self.from_ase(from_ase)
+        if from_pymatgen is not None:
+            self.from_pymatgen(from_pymatgen)
 
     def send_js_task(self, task):
         """Send a task to the javascript side.
         task is a dictionary with the following keys
         - name: the name of the task
         - kwargs: a dictionary of arguments
         """
```

### Comparing `weas_widget-0.1.0/src/weas_widget/utils.py` & `weas_widget-0.1.0a0/src/weas_widget/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-import numpy as np
-
-
-class ASEAdapter:
+class ASE_Adapter:
     def __init__(self):
         pass
 
     @classmethod
     def to_weas(cls, ase_atoms):
         """Convert an ASE Atoms object to the widget's format."""
         # if atoms is a list of atoms, check if they are the same species and number of atoms
@@ -33,15 +30,15 @@
         for key in ase_atoms.arrays.keys():
             if key not in ["positions", "numbers"]:
                 attributes["atom"][key] = ase_atoms.arrays[key]
 
         weas_atoms = {
             "species": species,
             "cell": cell,
-            "positions": positions.tolist(),
+            "positions": positions,
             "symbols": symbols,
             "attributes": attributes,
         }
         return weas_atoms
 
     @classmethod
     def to_ase(cls, weas_atoms):
@@ -56,64 +53,47 @@
         symbols = [weas_atoms["species"][s] for s in weas_atoms["symbols"]]
         positions = weas_atoms["positions"]
         cell = np.array(weas_atoms["cell"]).reshape(3, 3)
         ase_atoms = Atoms(symbols=symbols, positions=positions, cell=cell)
         return ase_atoms
 
 
-class PymatgenAdapter:
+class Pymatgen_Adapter:
     def __init__(self):
         pass
 
     @classmethod
     def to_weas(cls, pymatgen_structure):
-        from pymatgen.core import Molecule
-
+        # Convert a Pymatgen Structure object to the widget's format
         species = {}
-        # structure is a Molecule, convert it to Structure
-        if isinstance(pymatgen_structure, Molecule):
-            cell = [[0, 0, 0], [0, 0, 0], [0, 0, 0]]
-        else:
-            cell = pymatgen_structure.lattice.matrix.flatten().tolist()
-        positions = [site.coords.tolist() for site in pymatgen_structure.sites]
+        cell = pymatgen_structure.lattice.matrix.flatten().tolist()
+        positions = [site.coords for site in pymatgen_structure.sites]
         symbols = [site.species_string for site in pymatgen_structure.sites]
         for i in range(len(symbols)):
             species[symbols[i]] = symbols[i]
-        # save other arrays to attributes
-        attributes = {"atom": {}, "species": {}}
-        # read pymatgen site properties
-        for key in pymatgen_structure.site_properties.keys():
-            attributes["atom"][key] = [
-                site.properties[key] for site in pymatgen_structure.sites
-            ]
         weas_atoms = {
             "species": species,
             "cell": cell,
             "positions": positions,
             "symbols": symbols,
-            "attributes": attributes,
         }
         return weas_atoms
 
     @classmethod
     def to_pymatgen(cls, weas_atoms):
         # Convert the widget's format to a Pymatgen Structure object
-        from pymatgen.core import Molecule, Structure, Lattice
+        from pymatgen.core import Structure, Lattice
 
         if isinstance(weas_atoms, list):
             return [cls.to_pymatgen(atom) for atom in weas_atoms]
+
+        lattice = Lattice(weas_atoms["cell"])
         species = weas_atoms["symbols"]
         sites = weas_atoms["positions"]
-        cell = np.array(weas_atoms["cell"]).reshape(3, 3)
-        # if all cell are close to zeros, it is a molecule
-        if np.allclose(cell, np.zeros((3, 3))):
-            structure = Molecule(species, sites)
-        else:
-            lattice = Lattice(weas_atoms["cell"])
-            structure = Structure(lattice, species, sites, coords_are_cartesian=True)
+        structure = Structure(lattice, species, sites)
         return structure
 
 
 def generate_phonon_trajectory(
     atoms,
     eigenvectors,
     amplitude=1,
```

### Comparing `weas_widget-0.1.0/src/weas_widget/weas.py` & `weas_widget-0.1.0a0/src/weas_widget/weas.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 from .base_widget import BaseWidget
-from .utils import ASEAdapter, PymatgenAdapter, load_online_example
+from .utils import ASE_Adapter, Pymatgen_Adapter, load_online_example
+from .data import Data
 from .atoms_viewer import AtomsViewer
 from .camera import Camera
 from .plugins.instanced_mesh_pritimive import InstancedMeshPrimitive
 import time
 import threading
 
 
 class WeasWidget:
-    def __init__(self, from_ase=None, from_pymatgen=None, **kwargs):
+    def __init__(self, **kwargs):
         self._widget = BaseWidget(**kwargs)
         self.avr = AtomsViewer(self._widget)
+        self.data = Data(self._widget)
         self.camera = Camera(self._widget)
         self.imp = InstancedMeshPrimitive(self._widget)
-        if from_ase is not None:
-            self.from_ase(from_ase)
-        if from_pymatgen is not None:
-            self.from_pymatgen(from_pymatgen)
 
     def _repr_mimebundle_(self, *args, **kwargs):
-        # if ipywdigets > 8.0.0, use _repr_mimebundle_ instead of _ipython_display_
-        if hasattr(self._widget, "_repr_mimebundle_"):
-            return self._widget._repr_mimebundle_(*args, **kwargs)
-        else:
-            return self._widget._ipython_display_(*args, **kwargs)
+        return self._widget._repr_mimebundle_(*args, **kwargs)
 
     def from_ase(self, atoms):
-        self.avr.atoms = ASEAdapter.to_weas(atoms)
+        self.avr.atoms = ASE_Adapter.to_weas(atoms)
 
     def to_ase(self):
-        return ASEAdapter.to_ase(self.avr.atoms)
+        return ASE_Adapter.to_ase(self.avr.atoms)
 
     def from_pymatgen(self, structure):
-        self.avr.atoms = PymatgenAdapter.to_weas(structure)
+        self.avr.atoms = Pymatgen_Adapter.to_weas(structure)
 
     def to_pymatgen(self):
-        return PymatgenAdapter.to_pymatgen(self.avr.atoms)
+        return Pymatgen_Adapter.to_pymatgen(self.avr.atoms)
 
     def load_example(self, name="tio2.cif"):
         atoms = load_online_example(name)
-        self.avr.atoms = ASEAdapter.to_weas(atoms)
+        self.avr.atoms = ASE_Adapter.to_weas(atoms)
 
     def export_image(self, resolutionScale=5):
         self._widget.send_js_task(
             {
                 "name": "exportImage",
                 "kwargs": {"resolutionScale": resolutionScale},
             }
@@ -64,15 +58,15 @@
 
         # Display the image
         return display(Image(data=image_data))
 
     def download_image(self, filename="weas-model.png"):
         self._widget.send_js_task(
             {
-                "name": "tjs.downloadImage",
+                "name": "downloadImage",
                 "kwargs": {"filename": filename},
             }
         )
 
     def save_image(self, filename="weas-model.png", resolutionScale=5):
         import base64
```

### Comparing `weas_widget-0.1.0/src/weas_widget/static/widget.css` & `weas_widget-0.1.0a0/src/weas_widget/static/widget.css`

 * *Files identical despite different names*

### Comparing `weas_widget-0.1.0/src/weas_widget/static/widget.js` & `weas_widget-0.1.0a0/src/weas_widget/static/widget.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -16702,22 +16702,22 @@
     return r.position.copy(i), r
 }
 var yo = class extends no {
     constructor(e) {
         super(), this.tjs = e
     }
     add(e) {
-        super.add(e), this.dispatchObjectEvent({
+        console.log("add object", e), super.add(e), this.dispatchObjectEvent({
             data: e.toJSON(),
             action: "add",
             catalog: "object"
         })
     }
     remove(e) {
-        if (typeof e == "string" && (e = this.getObjectByProperty("uuid", e), !e)) {
+        if (console.log("remove object", e), typeof e == "string" && (e = this.getObjectByProperty("uuid", e), !e)) {
             console.warn("Object not found");
             return
         }
         super.remove(e), this.dispatchObjectEvent({
             data: e.toJSON(),
             action: "remove",
             catalog: "object"
@@ -16742,25 +16742,25 @@
             data: e,
             action: "zoom",
             catalog: "camera"
         }))
     }
     updatePosition(e, t, n) {
         let s = new y(e, t, n);
-        this.position.equals(s) || (this.position.copy(s), this.updateProjectionMatrix(), this.dispatchObjectEvent({
+        this.position.equals(s) || (this.position.copy(s), this.dispatchObjectEvent({
             data: [e, t, n],
             action: "position",
             catalog: "camera"
         }))
     }
     dispatchObjectEvent(e) {
         let t = new CustomEvent("weas", {
             detail: e
         });
-        this.tjs.containerElement.dispatchEvent(t), this.tjs.render()
+        this.tjs.containerElement.dispatchEvent(t)
     }
 };
 var Uc = class {
         constructor(e, t, n) {
             this.name = e, this.geometry = t, this.material = n, this.object3D = new Qe(t, n)
         }
     },
@@ -16798,15 +16798,15 @@
                 s = this.containerElement.clientWidth / this.containerElement.clientHeight,
                 r = n / 2,
                 a = r * s;
             this.camera = new vo(-a, a, r, -r, 1, 2e3, this), this.camera.position.set(0, -100, 0), this.camera.lookAt(0, 0, 0), this.camera.layers.enable(1), this.scene.add(this.camera);
             let o = new ao(16777215, 2);
             o.position.set(50, 50, 100), this.addLight("MainLight", o), this.camera.add(o);
             let c = new co(4210752, 20);
-            this.addLight("AmbientLight", c), this.controls = new mo(this.camera, e.domElement), this.viewerRect = this.containerElement.getBoundingClientRect(), window.addEventListener("resize", this.onWindowResize.bind(this), !1), this.containerElement.addEventListener("mousemove", this.render.bind(this)), this.containerElement.addEventListener("pointerup", this.render.bind(this)), this.containerElement.addEventListener("pointerdown", this.render.bind(this)), this.containerElement.addEventListener("click", this.render.bind(this)), this.containerElement.addEventListener("wheel", this.render.bind(this)), this.containerElement.addEventListener("atomsUpdated", this.render.bind(this))
+            this.addLight("AmbientLight", c), this.controls = new mo(this.camera, e.domElement), this.viewerRect = this.containerElement.getBoundingClientRect(), window.addEventListener("resize", this.onWindowResize.bind(this), !1)
         }
         addObject(e, t, n) {
             let s = new Uc(e, t, n);
             return this.objects[e] = s, this.scene.add(s.object3D), s
         }
         addMaterial(e, t) {
             let n = new Oc(e, t);
@@ -16829,15 +16829,15 @@
             if (this.camera.isOrthographicCamera) {
                 let e = this.containerElement.clientWidth / this.containerElement.clientHeight,
                     t = this.camera.top - this.camera.bottom;
                 this.camera.left = -t * e / 2, this.camera.right = t * e / 2
             } else this.camera.aspect = this.containerElement.clientWidth / this.containerElement.clientHeight;
             this.camera.updateProjectionMatrix(), Object.values(this.renderers).forEach(e => {
                 e.renderer.setSize(this.containerElement.clientWidth, this.containerElement.clientHeight)
-            }), this.viewerRect = this.containerElement.getBoundingClientRect(), this.render()
+            }), this.viewerRect = this.containerElement.getBoundingClientRect()
         }
         updateCameraAndControls({
             lookAt: e = null,
             direction: t = [0, 0, 1],
             distance: n = null,
             zoom: s = 1
         }) {
@@ -16848,15 +16848,15 @@
                 o;
             this.camera.isOrthographicCamera ? o = this.containerElement.clientWidth / this.containerElement.clientHeight : o = this.camera.aspect;
             let c = 10,
                 l = Math.max(a.x, a.y * o) + c,
                 h = l / o;
             this.camera.left = -l / 2, this.camera.right = l / 2, this.camera.top = h / 2, this.camera.bottom = -h / 2, n === null && (n = a.z + c);
             let u = e.clone().add(t.multiplyScalar(n));
-            this.camera.updatePosition(u.x, u.y, u.z), this.camera.lookAt(e), this.camera.updateZoom(s), this.camera.updateProjectionMatrix(), this.controls.target.set(e.x, e.y, e.z), this.render()
+            this.camera.updatePosition(u.x, u.y, u.z), this.camera.lookAt(e), this.camera.updateProjectionMatrix(), this.camera.updateZoom(s), this.controls.target.set(e.x, e.y, e.z)
         }
         getSceneBoundingBox() {
             let e = new Gt;
             return this.scene.traverse(function(t) {
                 if (t.isMesh || t.isLineSegments || t.isInstancedMesh) {
                     let n;
                     if (t.isInstancedMesh) {
@@ -16864,17 +16864,20 @@
                         t.computeBoundingBox(), n = t.boundingBox
                     } else t.geometry.computeBoundingBox(), n = t.geometry.boundingBox;
                     n = new Gt().copy(n).applyMatrix4(t.matrixWorld), e.union(n)
                 }
             }), e.isEmpty() && (e = new Gt(new y(-10, -10, -10), new y(10, 10, 10))), e
         }
         render() {
-            this.controls.update(), Object.values(this.renderers).forEach(e => {
-                e.renderer.render(this.scene, this.camera)
-            })
+            let e = () => {
+                requestAnimationFrame(e), this.controls.update(), Object.values(this.renderers).forEach(t => {
+                    t.renderer.render(this.scene, this.camera)
+                })
+            };
+            e()
         }
         exportImage(e = 5) {
             console.log("Exporting image");
             let t = this.renderers.MainRenderer.renderer,
                 n = t.getPixelRatio(),
                 s = e;
             t.setPixelRatio(s), t.render(this.scene, this.camera);
@@ -18726,15 +18729,15 @@
         if (this.guiConfig.buttons.measurement) {
             let s = this.createButton(`
             <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 512 512">
             <path d="M177.9 494.1c-18.7 18.7-49.1 18.7-67.9 0L17.9 401.9c-18.7-18.7-18.7-49.1 0-67.9l50.7-50.7 48 48c6.2 6.2 16.4 6.2 22.6 0s6.2-16.4 0-22.6l-48-48 41.4-41.4 48 48c6.2 6.2 16.4 6.2 22.6 0s6.2-16.4 0-22.6l-48-48 41.4-41.4 48 48c6.2 6.2 16.4 6.2 22.6 0s6.2-16.4 0-22.6l-48-48 41.4-41.4 48 48c6.2 6.2 16.4 6.2 22.6 0s6.2-16.4 0-22.6l-48-48 50.7-50.7c18.7-18.7 49.1-18.7 67.9 0l92.1 92.1c18.7 18.7 18.7 49.1 0 67.9L177.9 494.1z"/>
           </svg>
       `, "measurement");
             e.appendChild(s), s.addEventListener("click", () => {
-                this.weas.avr.Measurement.measure(this.weas.avr.selectedAtomsIndices)
+                this.weas.Measurement.measure(this.weas.avr.selectedAtomsIndices)
             })
         }
     }
     createButton(e, t = "button") {
         let n = document.createElement("button");
         return n.id = t, n.innerHTML = e, this.setStyle(n), n
     }
@@ -19262,15 +19265,15 @@
     init() {
         this.selectionBox = new Do(this.tjs.camera, this.tjs.scene), this.helper = new No(this.tjs.renderers.MainRenderer.renderer, "selectBox"), window.addEventListener("pointerdown", this.onMouseDown.bind(this), !1)
     }
     get selectedObjects() {
         return this._selectedObjects
     }
     set selectedObjects(e) {
-        e = e.filter(t => !t.userData.notSelectable), this._selectedObjects = e, this.highlightSelectedObjects()
+        console.log("Setting selected objects: ", e), e = e.filter(t => !t.userData.notSelectable), this._selectedObjects = e, this.highlightSelectedObjects()
     }
     onMouseDown(e) {
         let t = (e.clientX - this.tjs.viewerRect.left) / this.tjs.viewerRect.width * 2 - 1,
             n = -((e.clientY - this.tjs.viewerRect.top) / this.tjs.viewerRect.height) * 2 + 1;
         this.selectionBox.startPoint.set(t, n, .5), this.oldSelectedAtomsIndices = this.weas.avr.selectedAtomsIndices, this.oldSelectedObjects = this.selectedObjects
     }
     pickSelection(e) {
@@ -19319,15 +19322,18 @@
         this.selectedObjects.forEach(e => {
             Lo(e)
         }), this.selectedObjects = [], this.selectedInstances = {}, this.weas.avr.selectedAtomsIndices = [], this.highlightSelectedVertex()
     }
     highlightSelectedVertex() {
         Object.keys(this.selectedInstances).forEach(e => {
             let t = this.tjs.scene.getObjectByProperty("uuid", e);
-            if (!t || !t.userData.vertexPoints) return;
+            if (!t || !t.userData.vertexPoints) {
+                console.log("Object or vertex points not found");
+                return
+            }
             let n = t.userData.vertexPoints,
                 s = this.selectedInstances[e],
                 r = t.geometry.attributes.position.count,
                 a = new Float32Array(r * 3);
             for (let o = 0; o < r; o++) a[o * 3] = 0, a[o * 3 + 1] = 0, a[o * 3 + 2] = 0;
             s.forEach(o => {
                 a[o * 3] = 1, a[o * 3 + 1] = 0, a[o * 3 + 2] = 0
@@ -20569,84 +20575,84 @@
         JMOL: jx
     };
 var tr = class extends _t {
         static description = "Replace atoms";
         static category = "Edit";
         constructor({
             weas: e,
-            symbol: t = "C",
+            element: t = "C",
             indices: n = null
         }) {
-            super(e), this.indices = n || Array.from(this.weas.avr.selectedAtomsIndices), this.symbol = t, this.initialAtoms = e.avr.atoms.copy()
+            super(e), this.indices = n || Array.from(this.weas.avr.selectedAtomsIndices), this.element = t, this.initialAtoms = e.avr.atoms.copy()
         }
         execute() {
-            this.weas.avr.replaceSelectedAtoms(this.symbol, this.indices)
+            this.weas.avr.replaceSelectedAtoms(this.element, this.indices)
         }
         undo() {
             console.log("undo replace"), this.weas.avr.atoms = this.initialAtoms.copy()
         }
         adjust(e) {
-            (e in si || e in this.weas.avr.atoms.species) && (this.symbol = e, this.execute())
+            e in si && (this.element = e, this.execute())
         }
         setupGUI(e) {
-            _n(e, "Replace"), e.add(this, "symbol", "H").name("Symbol").onChange(t => {
-                this.adjust(this.symbol)
+            _n(e, "Replace"), e.add(this, "element", "H").name("Element").onChange(t => {
+                this.adjust(this.element)
             })
         }
     },
     nr = class extends _t {
         static description = "Add atom";
         static category = "Edit";
         constructor({
             weas: e,
-            symbol: t = "C",
+            element: t = "C",
             position: n = {
                 x: 0,
                 y: 0,
                 z: 0
             }
         }) {
-            super(e), this.position = n, this.symbol = t, this.initialAtoms = e.avr.atoms.copy()
+            super(e), this.position = n, this.element = t, this.initialAtoms = e.avr.atoms.copy()
         }
         execute() {
-            this.weas.avr.addAtom(this.symbol, this.position)
+            this.weas.avr.addAtom(this.element, this.position)
         }
         undo() {
             console.log("undo add atom"), this.weas.avr.atoms = this.initialAtoms.copy()
         }
         adjust(e, t) {
-            (e in si || e in this.weas.avr.atoms.species) && (this.weas.avr.atoms = this.initialAtoms.copy(), this.symbol = e, this.position = t, this.execute())
+            e in si && (this.weas.avr.atoms = this.initialAtoms.copy(), this.element = e, this.position = t, this.execute())
         }
         setupGUI(e) {
-            _n(e, "Add"), e.add(this, "symbol", "C").name("Symbol").onChange(t => {
+            _n(e, "Add"), e.add(this, "element", "C").name("Element").onChange(t => {
                 this.adjust(t, this.position)
             }), e.add(this.position, "x", -10, 10).name("X-axis").onChange(t => {
-                this.adjust(this.symbol, {
+                this.adjust(this.element, {
                     ...this.position,
                     x: t
                 })
             }), e.add(this.position, "y", -10, 10).name("Y-axis").onChange(t => {
-                this.adjust(this.symbol, {
+                this.adjust(this.element, {
                     ...this.position,
                     y: t
                 })
             }), e.add(this.position, "z", -10, 10).name("Z-axis").onChange(t => {
-                this.adjust(this.symbol, {
+                this.adjust(this.element, {
                     ...this.position,
                     z: t
                 })
             })
         }
     },
     ul = class extends _t {
         static description = "Color by attribute";
         static category = "Color";
         constructor({
             weas: e,
-            attribute: t = "Symbol",
+            attribute: t = "Element",
             color1: n = "#ff0000",
             color2: s = "#0000ff"
         }) {
             super(e), this.attribute = t, this.color1 = n, this.color2 = s, this.previousAttribute = e.colorBy, this.previousColorRamp = e.colorRamp, this.attributeKeys = Object.keys(this.weas.avr.atoms.attributes.atom).concat(Object.keys(Ws))
         }
         execute() {
             this.weas._colorRamp = [this.color1, this.color2], this.weas.colorBy = this.attribute, this.weas.drawModels()
@@ -22342,15 +22348,15 @@
                 if (e.origins.length > 1e3) {
                     console.warn("Too many labels, skipping...");
                     return
                 }
                 let t, n, s = e.selection || [...Array(this.viewer.atoms.getAtomsCount()).keys()];
                 typeof e.origins == "string" ? (t = this.viewer.atoms.getAttribute(e.origins), t = s.map(r => t[r])) : t = e.origins, typeof e.texts == "string" ? (n = this.viewer.atoms.getAttribute(e.texts), n = s.map(r => n[r])) : n = e.texts, this.labels = sy(t, n, e.fontSize, e.color, "Standard");
                 for (let r = 0; r < this.labels.length; r++) this.scene.add(this.labels[r])
-            }), this.viewer.tjs.render()
+            })
         }
         updateLabel(e = null, t = null) {}
     };
 
 function Fd(i, e) {
     e.forEach(t => {
         i.remove(t), t.remove()
@@ -22788,15 +22794,15 @@
                             transparent: !0,
                             opacity: .8,
                             side: Ot
                         });
                     var u = new Qe(g, _);
                     u.geometry.computeVertexNormals(), u.material.flatShading = !1, u.userData.type = "isosurface", u.userData.uuid = this.viewer.uuid, u.userData.notSelectable = !0, u.layers.set(1), this.scene.add(u), this.meshes.push(u)
                 }
-            }), this.viewer.tjs.render()
+            })
         }
     };
 
 function cy(i, e) {
     var t = new tt,
         n = [];
     return console.log("cells: ", e), i.forEach(function(s) {
@@ -22938,25 +22944,29 @@
         }
         reset() {
             this.settings = [], this.meshes.forEach(e => {
                 this.scene.remove(e)
             }), this.meshes = []
         }
         measure(e = null) {
-            e.length === 0 ? (this.meshes.forEach(t => {
-                this.scene.remove(t)
-            }), this.settings = [], this.meshes = []) : this.settings.push(new El({
+            if (e.length === 0) {
+                this.meshes.forEach(t => {
+                    this.scene.remove(t)
+                }), this.settings = [], this.meshes = [];
+                return
+            } else this.settings.push(new El({
                 indices: e
-            })), this.drawMeasurements()
+            }));
+            this.drawMeasurements()
         }
         drawMeasurements() {
             this.settings.forEach(e => {
                 let t = e.indices;
                 t.length === 1 ? this.showPosition(t) : t.length === 2 ? this.showDistance(t) : t.length === 3 ? this.showAngle(t) : t.length === 4 ? this.showDihedralAngle(t) : console.log("Invalid number of atoms for measurement")
-            }), this.viewer.tjs.render()
+            })
         }
         showPosition(e) {
             let t = e[0],
                 n = this.viewer.atoms.positions[t],
                 s = this.viewer.atoms.symbols[t];
             console.log(n, s);
             let r = `${s} [${n[0].toFixed(3)}, ${n[1].toFixed(3)}, ${n[2].toFixed(3)}]`,
@@ -23157,15 +23167,15 @@
         let e = document.createElement("div");
         e.id = "animation-controls", e.innerHTML = '<button id="play-pause-btn">Play</button><button id="reset-btn">Reset</button><input type="range" id="timeline" min="0" max="100" value="0"><span id="current-frame">0</span>', this.viewer.tjs.containerElement.appendChild(e);
         let t = document.getElementById("play-pause-btn"),
             n = document.getElementById("reset-btn");
         this.timeline = document.getElementById("timeline"), this.currentFrameDisplay = document.getElementById("current-frame"), this.isPlaying = !1;
         let s = 100;
         this.timeline.max = s, t.addEventListener("click", () => {
-            this.viewer.isPlaying = !this.viewer.isPlaying, t.textContent = this.viewer.isPlaying ? "Pause" : "Play", this.viewer.isPlaying && this.viewer.play()
+            this.isPlaying = !this.isPlaying, t.textContent = this.isPlaying ? "Pause" : "Play"
         }), n.addEventListener("click", () => {
             this.viewer.currentFrame = 0
         }), this.timeline.addEventListener("input", () => {
             this.viewer.currentFrame = parseInt(this.timeline.value, 10)
         })
     }
     removeTimeline() {
@@ -23205,41 +23215,35 @@
         viewerConfig: n = {}
     }) {
         this.uuid = Bt.generateUUID(), this.weas = e, this.tjs = e.tjs, console.log("weas: ", e);
         let s = {
             ...dd,
             ...n
         };
-        this._ready = !1, this._modelStyle = s._modelStyle, this._colorBy = s._colorBy, this._colorType = s._colorType, this._colorRamp = s._colorRamp, this._radiusType = s._radiusType, this._materialType = s._materialType, this._atomLabelType = s._atomLabelType, this._showBondedAtoms = s._showBondedAtoms, this._showCell = s._showCell, this._boundary = s._boundary, this.atomScale = s.atomScale, this.backgroundColor = s.backgroundColor, this._selectedAtomsIndices = new Array, this.debug = s.debug, this._currentFrame = 0, this.trajectory = [new wt], this.isPlaying = !1, this.frameDuration = 100, this.guiManager = new ia(this, this.weas.guiManager.gui), this.bondManager = new ko(this), this.polyhedraManager = new Zo(this), this.isosurfaceManager = new ea(this), this.ALManager = new Qo(this), this.Measurement = new na(this), this.VFManager = new ta(this), this.animate = this.animate.bind(this), this.init(t)
+        this._ready = !1, this._modelStyle = s._modelStyle, this._colorBy = s._colorBy, this._colorType = s._colorType, this._colorRamp = s._colorRamp, this._radiusType = s._radiusType, this._materialType = s._materialType, this._atomLabelType = s._atomLabelType, this._showBondedAtoms = s._showBondedAtoms, this._showCell = s._showCell, this._boundary = s._boundary, this.atomScale = s.atomScale, this.backgroundColor = s.backgroundColor, this._selectedAtomsIndices = new Array, this.debug = s.debug, this._currentFrame = 0, this.trajectory = [new wt], this.guiManager = new ia(this, this.weas.guiManager.gui), this.bondManager = new ko(this), this.polyhedraManager = new Zo(this), this.isosurfaceManager = new ea(this), this.ALManager = new Qo(this), this.Measurement = new na(this), this.VFManager = new ta(this), this.init(t)
     }
     init(e) {
         this.atomLabels = [], this.atomArrows = null, this.atomColors = new Array, this._atomScales = new Array, this._modelSticks = new Array, this._modelPolyhedras = new Array, this.lastFrameTime = Date.now(), this.boundaryList = null, this.bondRadius = .1, this.highlightAtomsMesh = null, this.selectedAtomsLabelElement = document.createElement("div"), this.selectedAtomsLabelElement.id = "selectedAtomSymbol", this.tjs.containerElement.appendChild(this.selectedAtomsLabelElement), this.showVectorField = !0, this.atoms = e, console.log("init AtomsViewer successfullly")
     }
-    play() {
-        this.isPlaying = !0, this.animate()
-    }
-    pause() {
-        this.isPlaying = !1
-    }
     animate() {
-        let e = Date.now();
-        this.isPlaying && this.trajectory.length > 0 && e - this.lastFrameTime > this.frameDuration && (this.currentFrame = (this.currentFrame + 1) % this.trajectory.length, this.lastFrameTime = e), this.isPlaying && requestAnimationFrame(this.animate)
+        let t = Date.now();
+        this.trajectory && this.trajectory.length > 0 && t - this.lastFrameTime > 100 && this.guiManager.isPlaying && (this.currentFrame = (this.currentFrame + 1) % this.trajectory.length)
     }
     updateFrame(e) {
         if (this.trajectory.length <= 1) return;
         let t = this.trajectory[e % this.trajectory.length];
         var n = new Te;
         for (let s = 0; s < t.positions.length; s++) this.atomsMesh.getMatrixAt(s, n), n.setPosition(new y(...t.positions[s])), this.atomsMesh.setMatrixAt(s, n);
         this.atomsMesh.instanceMatrix.needsUpdate = !0, this.guiManager.timeline.value = e, this.guiManager.currentFrameDisplay.textContent = e, this.bondManager.updateBondMesh(null, t), this.VFManager.updateArrowMesh(null, t)
     }
     get currentFrame() {
         return this._currentFrame
     }
     set currentFrame(e) {
-        this.currentFrame !== e && (this._currentFrame = e, this.lastFrameTime = Date.now(), this.updateFrame(e), this.tjs.render())
+        this.currentFrame !== e && (this._currentFrame = e, this.lastFrameTime = Date.now(), this.updateFrame(e))
     }
     get atoms() {
         let e = this.trajectory[this.currentFrame];
         return e.uuid = this.uuid, e
     }
     set atoms(e) {
         this.ready = !1, this.dispose(), console.log("set atoms: "), Array.isArray(e) && e.length > 1 ? this.trajectory = e : Array.isArray(e) && e.length === 1 ? this.trajectory = e : this.trajectory = [e], this._currentFrame = 0, this.bondManager.init(), this.polyhedraManager.init(), this.VFManager.init(), this.isosurfaceManager.reset(), this.Measurement.reset(), this.trajectory.length > 1 ? (this.guiManager.addTimeline(), this.guiManager.timeline.max = this.trajectory.length - 1) : this.guiManager.removeTimeline(), this.modelStyle = this._modelStyle, this.drawModels(), this.selectedAtomsIndices = [], this.tjs.updateCameraAndControls({
@@ -23391,15 +23395,15 @@
         }, this.debug && console.log("bondedAtoms: ", this.bondedAtoms), this.atomColors = Tl(this.atoms, this.colorBy, {
             colorType: this.colorType,
             colorRamp: this._colorRamp
         }), this.drawBalls();
         let n = this.bondManager.drawBonds();
         this.atomsMesh.add(n);
         let s = this.polyhedraManager.drawPolyhedras();
-        this.atomsMesh.add(s), this.isosurfaceManager.drawIsosurfaces(), this.showVectorField && this.VFManager.drawVectorFields(), this.drawHighlightAtoms(), this.ALManager.drawAtomLabels(), this.ready = !0, this.weas.tjs.render()
+        this.atomsMesh.add(s), this.isosurfaceManager.drawIsosurfaces(), this.showVectorField && this.VFManager.drawVectorFields(), this.drawHighlightAtoms(), this.ALManager.drawAtomLabels(), this.ready = !0
     }
     drawBalls() {
         if (this.atomsMesh = Vo({
                 scene: this.tjs.scene,
                 atoms: this.atoms,
                 atomScales: this.atomScales,
                 colors: this.atomColors,
@@ -23432,15 +23436,15 @@
             scene: this.tjs.scene,
             atoms: this.atoms,
             atomScales: e,
             colors: t,
             radiusType: this.radiusType,
             materialType: "Basic",
             data_type: "highlight"
-        }), this.atomsMesh.add(this.highlightAtomsMesh), this.highlightAtomsMesh.material.opacity = .6, this.highlightAtomsMesh.layers.set(1), this.updateHighlightAtomsMesh(this.selectedAtomsIndices)
+        }), this.atomsMesh.add(this.highlightAtomsMesh), this.highlightAtomsMesh.material.opacity = .6, this.updateHighlightAtomsMesh(this.selectedAtomsIndices)
     }
     clearHighlightAtoms() {
         this.highlightAtomsMesh && (console.log("clearHighlightAtoms: "), bt(this.tjs.scene, this.highlightAtomsMesh))
     }
     dispose() {
         this.atomsMesh && this.atomsMesh.dispose(), this.boundaryAtomsMesh && this.boundaryAtomsMesh.dispose(), xo(this.tjs.scene, this.uuid)
     }
@@ -23524,15 +23528,20 @@
             viewerConfig: n
         }), this.instancedMeshPrimitive = new zo(this), this.initialize()
     }
     initialize() {
         this.activeObject = null, this.render()
     }
     render() {
-        this.tjs.render()
+        let t = () => {
+            requestAnimationFrame(t), this.tjs.controls.update(), this.avr.animate(), Object.values(this.tjs.renderers).forEach(n => {
+                n.renderer.render(this.tjs.scene, this.tjs.camera)
+            })
+        };
+        t()
     }
     clear() {
         this.tjs.scene.clear()
     }
 };
 
 function hy(i) {
@@ -23815,15 +23824,15 @@
         let a = i.get("cameraZoom");
         t.tjs.camera.updateZoom(a)
     }), i.on("change:cameraPosition", () => {
         let a = i.get("cameraPosition");
         t.tjs.camera.updatePosition(a[0], a[1], a[2])
     }), i.on("change:cameraLookAt", () => {
         let a = i.get("cameraLookAt");
-        t.tjs.controls.target.set(a[0], a[1], a[2]), t.tjs.render()
+        t.tjs.controls.target.set(a[0], a[1], a[2])
     })
 }
 
 function zd(i, e = [
     [1, 0, 0],
     [0, 1, 0],
     [0, 0, 1]
```

### Comparing `weas_widget-0.1.0/.gitignore` & `weas_widget-0.1.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `weas_widget-0.1.0/LICENSE` & `weas_widget-0.1.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `weas_widget-0.1.0/README.md` & `weas_widget-0.1.0a0/README.md`

 * *Files identical despite different names*

### Comparing `weas_widget-0.1.0/pyproject.toml` & `weas_widget-0.1.0a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "weas_widget"
-version = "0.1.0"
+version = "0.1.0a"
 description = "A widget to visualize and interact with atomistic structures in Jupyter Notebook."
 authors = [{name = "Xing Wang", email = "xingwang1991@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `weas_widget-0.1.0/PKG-INFO` & `weas_widget-0.1.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: weas_widget
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: A widget to visualize and interact with atomistic structures in Jupyter Notebook.
 Project-URL: Documentation, https://weas-widget.readthedocs.io
 Project-URL: Source, https://github.com/superstart54/weas-widget
 Author-email: Xing Wang <xingwang1991@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Xing Wang
```

