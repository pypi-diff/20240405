# Comparing `tmp/vbl_aquarium-0.0.8.tar.gz` & `tmp/vbl_aquarium-0.0.9.tar.gz`

## Comparing `vbl_aquarium-0.0.8.tar` & `vbl_aquarium-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/setup.cfg
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.github/workflows/autoformat-and-lint.yml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.github/workflows/build.yml
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.idea/vbl-json-schema.iml
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.idea/vcs.xml
--rw-r--r--   0        0        0    21723 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.idea/copilot/chatSessions/00000000000.xd
--rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.idea/copilot/chatSessions/xd.lck
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.idea/copilot/chatSessions/blobs/version
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/__init__.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/build.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/generate_cs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/models/__init__.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/models/dock.py
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/models/ephys_link.py
--rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/models/generic.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/models/logging.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/models/pinpoint.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/models/unity.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/models/urchin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/utils/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/utils/common.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/src/vbl_aquarium/utils/vbl_base_model.py
--rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/.gitignore
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/LICENSE
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/README.md
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/setup.cfg
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.github/workflows/autoformat-and-lint.yml
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.idea/.gitignore
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.idea/misc.xml
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.idea/modules.xml
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.idea/vbl-json-schema.iml
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.idea/vcs.xml
+-rw-r--r--   0        0        0    39235 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.idea/copilot/chatSessions/00000000000.xd
+-rw-r--r--   0        0        0     7571 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.idea/copilot/chatSessions/xd.lck
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.idea/copilot/chatSessions/blobs/version
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/__init__.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/build.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/generate_cs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/models/__init__.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/models/dock.py
+-rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/models/ephys_link.py
+-rw-r--r--   0        0        0     2824 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/models/generic.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/models/logging.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/models/pinpoint.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/models/unity.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/models/urchin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/utils/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/utils/common.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/src/vbl_aquarium/utils/vbl_base_model.py
+-rw-r--r--   0        0        0     7979 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/LICENSE
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/README.md
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 vbl_aquarium-0.0.9/PKG-INFO
```

### Comparing `vbl_aquarium-0.0.8/.github/dependabot.yml` & `vbl_aquarium-0.0.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/.github/workflows/autoformat-and-lint.yml` & `vbl_aquarium-0.0.9/.github/workflows/autoformat-and-lint.yml`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,26 @@
       - name: 📦 Install Hatch
         run: pip install hatch
 
       - name: 📝 Format Code
         run: hatch fmt -f
 
       - name: ✅ Commit code format changes
+        if: github.ref != 'refs/heads/main'
         uses: stefanzweifel/git-auto-commit-action@v5
         with:
-          commit_message: "Autoformat code"
+          commit_message: "chore: Autoformat code"
           skip_fetch: true
           skip_checkout: true
 
+      - name: 📤 PR code format changes
+        if: github.ref == 'refs/heads/main'
+        uses: peter-evans/create-pull-request@v6
+        with:
+          token: ${{ secrets.PR_TOKEN }}
+          commit-message: "Autoformat code"
+          title: "chore: Autoformat code"
+          branch: "autoformat-code"
+          delete-branch: true
+
       - name: 🔍 Lint
         run: hatch fmt --check
```

### Comparing `vbl_aquarium-0.0.8/.github/workflows/build.yml` & `vbl_aquarium-0.0.9/.github/workflows/build.yml`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 name: Build
 
 on:
+  pull_request: 
   push:
     branches:
       - main
+  merge_group:
 
 jobs:
   build:
     name: Build
     runs-on: ubuntu-latest
     
     steps:
@@ -23,14 +25,15 @@
       - name: 📦 Install dependencies
         run: pip install .
 
       - name: 🛠️ Build
         run: python src/vbl_aquarium/build.py
       
       - name: 📤 PR changes
+        if: github.ref == 'refs/heads/main'
         uses: peter-evans/create-pull-request@v6
         with:
           token: ${{ secrets.PR_TOKEN }}
           commit-message: "Build Models"
           title: "chore: Build Models"
           branch: "build-models"
           delete-branch: true
```

### Comparing `vbl_aquarium-0.0.8/.github/workflows/codeql-analysis.yml` & `vbl_aquarium-0.0.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/.idea/vbl-json-schema.iml` & `vbl_aquarium-0.0.9/.idea/vbl-json-schema.iml`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/.idea/copilot/chatSessions/xd.lck` & `vbl_aquarium-0.0.9/.idea/copilot/chatSessions/xd.lck`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/src/vbl_aquarium/build.py` & `vbl_aquarium-0.0.9/src/vbl_aquarium/build.py`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/src/vbl_aquarium/generate_cs.py` & `vbl_aquarium-0.0.9/src/vbl_aquarium/generate_cs.py`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/src/vbl_aquarium/models/ephys_link.py` & `vbl_aquarium-0.0.9/src/vbl_aquarium/models/ephys_link.py`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/src/vbl_aquarium/models/generic.py` & `vbl_aquarium-0.0.9/src/vbl_aquarium/models/generic.py`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/src/vbl_aquarium/models/urchin.py` & `vbl_aquarium-0.0.9/src/vbl_aquarium/models/urchin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
 from enum import Enum
 
+from pydantic import Field
+
 from vbl_aquarium.models.unity import Color, Vector2, Vector3
 from vbl_aquarium.utils.vbl_base_model import VBLBaseModel
 
 # CustomAtlas
 
 
 class CustomAtlasModel(VBLBaseModel):
@@ -14,22 +16,22 @@
     resolution: Vector3
 
 
 # CustomMesh
 
 
 class CustomMeshData(VBLBaseModel):
-    id: str
+    id: str = Field(alias="ID")
     vertices: list[Vector3]
     triangles: list[int]
     normals: list[Vector3] = None
 
 
 class CustomMeshModel(VBLBaseModel):
-    id: str
+    id: str = Field(alias="ID")
     position: Vector3
     use_reference: bool
     material: str
     scale: Vector3
     color: Color
 
 
@@ -62,28 +64,28 @@
     main: bool
 
 
 # Individual mesh neuron
 
 
 class MeshModel(VBLBaseModel):
-    id: str
+    id: str = Field(alias="ID")
     shape: str
     position: Vector3
     color: Color
     scale: Vector3
     material: str
     interactive: bool
 
 
 # Particle group
 
 
 class ParticleGroupModel(VBLBaseModel):
-    id: str
+    id: str = Field(alias="ID")
     scale: Vector3
     shape: str
     material: str
 
     xs: list[float]
     ys: list[float]
     zs: list[float]
```

### Comparing `vbl_aquarium-0.0.8/.gitignore` & `vbl_aquarium-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/LICENSE` & `vbl_aquarium-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/pyproject.toml` & `vbl_aquarium-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vbl_aquarium-0.0.8/PKG-INFO` & `vbl_aquarium-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: vbl-aquarium
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collection of Pydantic models describing data objects passed between Virtual Brain Lab projects.
 Project-URL: Documentation, https://github.com/VirtualBrainLab/vbl-aquarium/blob/main/README.md
 Project-URL: Issues, https://github.com/VirtualBrainLab/vbl-aquarium/issues
 Project-URL: Source, https://github.com/VirtualBrainLab/vbl-aquarium
 Author-email: Daniel Birman <dbirman@uw.edu>, Kenneth Yang <kjy5@uw.edu>
 License-Expression: MIT
 License-File: LICENSE
```

