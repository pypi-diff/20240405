# Comparing `tmp/hyperx-2024.1.8-py3-none-any.whl.zip` & `tmp/hyperx-2024.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 47643 bytes, number of entries: 12
+Zip file size: 47634 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat      742 b- defN 24-Jan-17 19:54 hyperx/__init__.py
--rw-rw-rw-  2.0 fat   292609 b- defN 24-Mar-12 21:02 hyperx/api/__init__.py
--rw-rw-rw-  2.0 fat    32628 b- defN 24-Mar-12 21:02 hyperx/api/types/__init__.py
+-rw-rw-rw-  2.0 fat   292632 b- defN 24-Mar-28 17:41 hyperx/api/__init__.py
+-rw-rw-rw-  2.0 fat    32628 b- defN 24-Mar-28 17:41 hyperx/api/types/__init__.py
 -rw-rw-rw-  2.0 fat      125 b- defN 23-Oct-16 20:54 hyperx/library/__init__.py
 -rw-rw-rw-  2.0 fat     1621 b- defN 24-Jan-17 19:54 hyperx/library/find.py
 -rw-rw-rw-  2.0 fat     1502 b- defN 24-Jan-17 19:54 hyperx/library/library.py
 -rw-rw-rw-  2.0 fat       71 b- defN 23-Oct-16 20:54 hyperx/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2787 b- defN 23-Oct-16 20:54 hyperx/utils/utils.py
--rw-rw-rw-  2.0 fat      629 b- defN 24-Mar-12 21:05 hyperx-2024.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-12 21:05 hyperx-2024.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 24-Mar-12 21:05 hyperx-2024.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      945 b- defN 24-Mar-12 21:05 hyperx-2024.1.8.dist-info/RECORD
-12 files, 333758 bytes uncompressed, 46065 bytes compressed:  86.2%
+-rw-rw-rw-  2.0 fat      629 b- defN 24-Mar-28 17:45 hyperx-2024.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-28 17:45 hyperx-2024.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Mar-28 17:45 hyperx-2024.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      945 b- defN 24-Mar-28 17:45 hyperx-2024.1.9.dist-info/RECORD
+12 files, 333781 bytes uncompressed, 46056 bytes compressed:  86.2%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: hyperx/utils/__init__.py
 Comment: 
 
 Filename: hyperx/utils/utils.py
 Comment: 
 
-Filename: hyperx-2024.1.8.dist-info/METADATA
+Filename: hyperx-2024.1.9.dist-info/METADATA
 Comment: 
 
-Filename: hyperx-2024.1.8.dist-info/WHEEL
+Filename: hyperx-2024.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: hyperx-2024.1.8.dist-info/top_level.txt
+Filename: hyperx-2024.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: hyperx-2024.1.8.dist-info/RECORD
+Filename: hyperx-2024.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hyperx/api/__init__.py

```diff
@@ -421,15 +421,15 @@
 		for subclass in IdEntity.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
 		return tuple([givenClass(idEntityCol) for idEntityCol in self._Entity])
 
 	@property
 	def Ids(self) -> tuple[int]:
-		return tuple([int(int32) for int32 in self._Entity.Ids])
+		return tuple([int32 for int32 in self._Entity.Ids])
 
 	def Contains(self, id: int) -> bool:
 		return self._Entity.Contains(id)
 
 	def Count(self) -> int:
 		return self._Entity.Count()
 
@@ -460,15 +460,15 @@
 		for subclass in T.__subclasses__():
 			if subclass.__name__ == thisClass:
 				givenClass = subclass
 		return tuple([givenClass(idNameEntityCol) for idNameEntityCol in self._Entity])
 
 	@property
 	def Names(self) -> tuple[str]:
-		return tuple([str(string) for string in self._Entity.Names])
+		return tuple([string for string in self._Entity.Names])
 
 	@overload
 	def Get(self, name: str) -> T: ...
 
 	@overload
 	def Get(self, id: int) -> T: ...
 
@@ -1739,19 +1739,19 @@
 		for kvp in self._Entity.ElementsByObjectOrSkin:
 			elementsByObjectOrSkinDict[types.DiscreteDefinitionType[kvp.Key.ToString()]] = ElementCol(kvp.Value)
 
 		return elementsByObjectOrSkinDict
 
 	@property
 	def Skins(self) -> tuple[types.DiscreteDefinitionType]:
-		return tuple([types.DiscreteDefinitionType(discreteDefinitionType) for discreteDefinitionType in self._Entity.Skins])
+		return tuple([types.DiscreteDefinitionType[discreteDefinitionType.ToString()] for discreteDefinitionType in self._Entity.Skins])
 
 	@property
 	def Objects(self) -> tuple[types.DiscreteDefinitionType]:
-		return tuple([types.DiscreteDefinitionType(discreteDefinitionType) for discreteDefinitionType in self._Entity.Objects])
+		return tuple([types.DiscreteDefinitionType[discreteDefinitionType.ToString()] for discreteDefinitionType in self._Entity.Objects])
 
 	@property
 	def DiscreteTechnique(self) -> types.DiscreteTechnique:
 		return types.DiscreteTechnique[self._Entity.DiscreteTechnique.ToString()]
 
 	@property
 	def LeftSkinZoneId(self) -> int:
@@ -4306,15 +4306,15 @@
 		for kvp in self._Entity.CorrectionFactorRows:
 			correctionFactorRowsDict[int(kvp.Key)] = TabularCorrectionFactorRow(kvp.Value)
 
 		return correctionFactorRowsDict
 
 	@property
 	def CorrectionIndependentDefinitions(self) -> set[types.CorrectionIndependentDefinition]:
-		return {types.CorrectionIndependentDefinition(correctionIndependentDefinition) for correctionIndependentDefinition in self._Entity.CorrectionIndependentDefinitions}
+		return {types.CorrectionIndependentDefinition[correctionIndependentDefinition.ToString()] for correctionIndependentDefinition in self._Entity.CorrectionIndependentDefinitions}
 
 	@overload
 	def SetIndependentValue(self, correctionPointId: int, cid: types.CorrectionIndependentDefinition, value: float) -> None: ...
 
 	@overload
 	def SetIndependentValue(self, correctionPointId: int, cid: types.CorrectionIndependentDefinition, value: bool) -> None: ...
```

## Comparing `hyperx-2024.1.8.dist-info/METADATA` & `hyperx-2024.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 2024.1.8
+Version: 2024.1.9
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

