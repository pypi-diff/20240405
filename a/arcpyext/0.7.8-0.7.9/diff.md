# Comparing `tmp/arcpyext-0.7.8-py2.py3-none-any.whl.zip` & `tmp/arcpyext-0.7.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 64260 bytes, number of entries: 57
--rw-rw-rw-  2.0 fat      487 b- defN 19-Aug-05 23:42 arcpyext/__init__.py
+Zip file size: 65518 bytes, number of entries: 59
+-rw-rw-rw-  2.0 fat      507 b- defN 20-Jul-02 01:08 arcpyext/__init__.py
 -rw-rw-rw-  2.0 fat     1365 b- defN 19-Aug-05 23:42 arcpyext/_multiprocessing.py
 -rw-rw-rw-  2.0 fat     1846 b- defN 19-Aug-05 23:42 arcpyext/_patches.py
--rw-rw-rw-  2.0 fat      191 b- defN 20-Jan-30 00:38 arcpyext/_version.py
+-rw-rw-rw-  2.0 fat      191 b- defN 20-Jul-02 01:07 arcpyext/_version.py
 -rw-rw-rw-  2.0 fat       75 b- defN 19-Aug-05 23:42 arcpyext/_json/__init__.py
 -rw-rw-rw-  2.0 fat      805 b- defN 19-Aug-05 23:42 arcpyext/_json/json_enum.py
 -rw-rw-rw-  2.0 fat      823 b- defN 19-Aug-05 23:42 arcpyext/_json/to_json_encoder.py
 -rw-rw-rw-  2.0 fat      395 b- defN 19-Aug-05 23:42 arcpyext/_native/__init__.py
 -rw-rw-rw-  2.0 fat     4156 b- defN 19-Aug-05 23:42 arcpyext/_native/_dotnet.py
 -rw-rw-rw-  2.0 fat     2135 b- defN 19-Aug-05 23:42 arcpyext/_native/arcgispro.py
 -rw-rw-rw-  2.0 fat     2409 b- defN 19-Aug-05 23:42 arcpyext/_native/arcobjects.py
+-rw-rw-rw-  2.0 fat     1301 b- defN 20-Jul-02 03:11 arcpyext/_str/ExtendedFormatter.py
+-rw-rw-rw-  2.0 fat      104 b- defN 20-Jul-02 01:11 arcpyext/_str/__init__.py
 -rw-rw-rw-  2.0 fat     1799 b- defN 19-Nov-14 07:02 arcpyext/conversion/ToCsv.py
 -rw-rw-rw-  2.0 fat     3747 b- defN 19-Nov-15 05:40 arcpyext/conversion/ToGeoPackage.py
 -rw-rw-rw-  2.0 fat     1916 b- defN 19-Nov-14 07:02 arcpyext/conversion/ToKml.py
 -rw-rw-rw-  2.0 fat     2813 b- defN 19-Nov-15 04:05 arcpyext/conversion/ToMapInfoTab.py
 -rw-rw-rw-  2.0 fat     7848 b- defN 19-Nov-14 07:02 arcpyext/conversion/ToOfficeOpenXmlWorkbook.py
 -rw-rw-rw-  2.0 fat     2280 b- defN 19-Nov-14 07:02 arcpyext/conversion/ToShapefile.py
 -rw-rw-rw-  2.0 fat     5586 b- defN 19-Nov-15 04:59 arcpyext/conversion/_ConvertBase.py
@@ -29,31 +31,31 @@
 -rw-rw-rw-  2.0 fat      606 b- defN 19-Aug-05 23:42 arcpyext/exceptions/map_data_sources_broken_error.py
 -rw-rw-rw-  2.0 fat      851 b- defN 19-Aug-05 23:42 arcpyext/exceptions/map_layer_error.py
 -rw-rw-rw-  2.0 fat      598 b- defN 19-Aug-05 23:42 arcpyext/exceptions/serv_def_draft_create_error.py
 -rw-rw-rw-  2.0 fat      597 b- defN 19-Aug-05 23:42 arcpyext/exceptions/unmapped_data_source_error.py
 -rw-rw-rw-  2.0 fat      595 b- defN 19-Aug-05 23:42 arcpyext/exceptions/unsupported_layer_error.py
 -rw-rw-rw-  2.0 fat       23 b- defN 19-Aug-05 23:42 arcpyext/mapping/__init__.py
 -rw-rw-rw-  2.0 fat     2416 b- defN 19-Aug-05 23:42 arcpyext/mapping/_compare_helpers.py
--rw-rw-rw-  2.0 fat    17387 b- defN 20-Jan-30 00:38 arcpyext/mapping/_mapping.py
+-rw-rw-rw-  2.0 fat    17387 b- defN 20-Jan-30 00:52 arcpyext/mapping/_mapping.py
 -rw-rw-rw-  2.0 fat    25585 b- defN 20-Jan-14 20:43 arcpyext/mapping/_mapping2.py
--rw-rw-rw-  2.0 fat    11451 b- defN 20-Jan-30 00:37 arcpyext/mapping/_mapping3.py
--rw-rw-rw-  2.0 fat     2383 b- defN 20-Jan-29 21:13 arcpyext/mapping/_mapping_helpers.py
+-rw-rw-rw-  2.0 fat    13027 b- defN 20-Jul-02 03:11 arcpyext/mapping/_mapping3.py
+-rw-rw-rw-  2.0 fat     2383 b- defN 20-Jul-02 01:34 arcpyext/mapping/_mapping_helpers.py
 -rw-rw-rw-  2.0 fat     7850 b- defN 19-Aug-05 23:42 arcpyext/mapping/compare_types.py
 -rw-rw-rw-  2.0 fat       35 b- defN 19-Aug-05 23:42 arcpyext/mapping/_cim/__init__.py
 -rw-rw-rw-  2.0 fat     1117 b- defN 19-Nov-06 00:29 arcpyext/mapping/_cim/factories.py
 -rw-rw-rw-  2.0 fat     1479 b- defN 19-Aug-05 23:42 arcpyext/mapping/_cim/helpers.py
 -rw-rw-rw-  2.0 fat     2856 b- defN 19-Nov-06 00:29 arcpyext/mapping/_cim/layers.py
 -rw-rw-rw-  2.0 fat     3118 b- defN 19-Aug-05 23:42 arcpyext/mapping/_cim/pro_map.py
 -rw-rw-rw-  2.0 fat     2620 b- defN 19-Aug-05 23:42 arcpyext/mapping/_cim/pro_project.py
 -rw-rw-rw-  2.0 fat     2037 b- defN 19-Aug-05 23:42 arcpyext/mapping/_cim/tables.py
 -rw-rw-rw-  2.0 fat      369 b- defN 19-Oct-30 21:26 arcpyext/publishing/__init__.py
 -rw-rw-rw-  2.0 fat     5861 b- defN 19-Oct-11 00:51 arcpyext/publishing/_publishing.py
 -rw-rw-rw-  2.0 fat       53 b- defN 17-Nov-24 01:40 arcpyext/schematransform/__init__.py
 -rw-rw-rw-  2.0 fat    22822 b- defN 19-Aug-05 23:42 arcpyext/schematransform/_schematransform.py
 -rw-rw-rw-  2.0 fat     5155 b- defN 19-Aug-05 23:42 arcpyext/toolbox/PythonToolbox.py
 -rw-rw-rw-  2.0 fat       42 b- defN 17-Apr-07 05:23 arcpyext/toolbox/__init__.py
--rw-rw-rw-  2.0 fat     1520 b- defN 20-Jan-30 00:51 arcpyext-0.7.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13442 b- defN 20-Jan-30 00:51 arcpyext-0.7.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      116 b- defN 20-Jan-30 00:51 arcpyext-0.7.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 20-Jan-30 00:51 arcpyext-0.7.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     5067 b- defN 20-Jan-30 00:51 arcpyext-0.7.8.dist-info/RECORD
-57 files, 188558 bytes uncompressed, 56106 bytes compressed:  70.2%
+-rw-rw-rw-  2.0 fat     1520 b- defN 20-Jul-02 03:43 arcpyext-0.7.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13442 b- defN 20-Jul-02 03:43 arcpyext-0.7.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      116 b- defN 20-Jul-02 03:43 arcpyext-0.7.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 20-Jul-02 03:43 arcpyext-0.7.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     5239 b- defN 20-Jul-02 03:43 arcpyext-0.7.9.dist-info/RECORD
+59 files, 191731 bytes uncompressed, 57094 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -27,14 +27,20 @@
 
 Filename: arcpyext/_native/arcgispro.py
 Comment: 
 
 Filename: arcpyext/_native/arcobjects.py
 Comment: 
 
+Filename: arcpyext/_str/ExtendedFormatter.py
+Comment: 
+
+Filename: arcpyext/_str/__init__.py
+Comment: 
+
 Filename: arcpyext/conversion/ToCsv.py
 Comment: 
 
 Filename: arcpyext/conversion/ToGeoPackage.py
 Comment: 
 
 Filename: arcpyext/conversion/ToKml.py
@@ -150,23 +156,23 @@
 
 Filename: arcpyext/toolbox/PythonToolbox.py
 Comment: 
 
 Filename: arcpyext/toolbox/__init__.py
 Comment: 
 
-Filename: arcpyext-0.7.8.dist-info/LICENSE
+Filename: arcpyext-0.7.9.dist-info/LICENSE
 Comment: 
 
-Filename: arcpyext-0.7.8.dist-info/METADATA
+Filename: arcpyext-0.7.9.dist-info/METADATA
 Comment: 
 
-Filename: arcpyext-0.7.8.dist-info/WHEEL
+Filename: arcpyext-0.7.9.dist-info/WHEEL
 Comment: 
 
-Filename: arcpyext-0.7.8.dist-info/top_level.txt
+Filename: arcpyext-0.7.9.dist-info/top_level.txt
 Comment: 
 
-Filename: arcpyext-0.7.8.dist-info/RECORD
+Filename: arcpyext-0.7.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## arcpyext/__init__.py

```diff
@@ -9,13 +9,14 @@
 import logging
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 from . import _patches as _patches
 _patches.apply()
 
 from . import _native
+from . import _str
 from . import conversion
 from . import data
 from . import toolbox
 from . import schematransform
 from . import mapping
 from . import publishing
```

## arcpyext/_version.py

```diff
@@ -1,3 +1,3 @@
-__version__ = "0.7.8"
+__version__ = "0.7.9"
 __author__ = "David Whittingham; David Payne; Adam Kerz; Peter Reyne; Daniel Baternik; Chris Blanchfield"
 __copyright__ = "Copyright (C) 2019-2020 David Whittingham"
```

## arcpyext/mapping/_mapping3.py

```diff
@@ -19,14 +19,15 @@
 # Third-party imports
 import arcpy
 
 # Local imports
 from ._cim import ProProject
 from ._mapping_helpers import tokenise_table_name
 from .. import _native as _prosdk
+from .._str import eformat
 from ..exceptions import DataSourceUpdateError
 
 # Put the map document class here so we can access the per-version type in a consistent location across Python versions
 Document = arcpy.mp.ArcGISProject
 
 
 def open_document(project):
@@ -79,15 +80,42 @@
 
                         # process magic field updating
                         if k == "dataset":
                             # pass original value for parts
                             dataset_parts = tokenise_table_name(original[k])
 
                             # format new value, if necessary
-                            new_conn_props[k] = new_conn_props[k].format(**dataset_parts)
+                            new_conn_props[k] = eformat.format(new_conn_props[k], **dataset_parts)
+
+                elif k == "featureDataset":
+                    # won't be in original, have to drop into CIM to get the feature dataset (as of 2.5.2)
+                    layer_cim = layer.getDefinition("V2")
+                    data_connection = layer_cim.featureTable.dataConnection
+                    feature_dataset = ""
+                    if hasattr(data_connection, "featureDataset"):
+                        feature_dataset = data_connection.featureDataset
+
+                        # pass original value for parts
+                        feature_dataset_parts = tokenise_table_name(feature_dataset)
+
+                        # format new value, if necessary
+                        _get_logger().debug("k = %s", k)
+                        _get_logger().debug("new = %s", new)
+                        feature_dataset = eformat.format(new[k], **feature_dataset_parts)
+
+                    # easiest to apply here, rather than step through again on updateConnectionProperties
+                    # hopefully this code can be removed in some future ArcGIS Pro version
+                    if feature_dataset:
+                        #data_connection.featureDataset.replace(str(data_connection.featureDataset), newDatabase)
+                        data_connection.featureDataset = feature_dataset
+                    else:
+                        if hasattr(data_connection, "featureDataset"):
+                            del data_connection.featureDataset
+
+                    layer.setDefinition(layer_cim)
                 else:
                     new_conn_props[k] = new[k]
 
             return (matched_conn_props, new_conn_props)
 
         matched_conn_props, new_conn_props = get_paired_conn_props(layer.connectionProperties, new_props)
```

## Comparing `arcpyext-0.7.8.dist-info/LICENSE` & `arcpyext-0.7.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `arcpyext-0.7.8.dist-info/METADATA` & `arcpyext-0.7.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arcpyext
-Version: 0.7.8
+Version: 0.7.9
 Summary: Extended functionality for Esri's ArcPy site-package
 Home-page: https://github.com/DavidWhittingham/arcpyext
 Author: David Whittingham; David Payne; Adam Kerz; Peter Reyne; Daniel Baternik; Chris Blanchfield
 License: BSD 3-Clause
 Keywords: arcgis esri arcpy
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

## Comparing `arcpyext-0.7.8.dist-info/RECORD` & `arcpyext-0.7.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-arcpyext/__init__.py,sha256=_9P6hLD22SZy68VeI51YgH0gL_uJT6MYgiybrKjtk6c,487
+arcpyext/__init__.py,sha256=n9BaouVgcRCVdz7u5J3_t4Pwj0l1MhuKs1tyM9oBcnQ,507
 arcpyext/_multiprocessing.py,sha256=zDqobM_wbOxGWNHRwLsk-KbzS77IUJoRl-BGF9ogzzY,1365
 arcpyext/_patches.py,sha256=A0h_jJzozIP6Jp_vct7ltgJTEHUjhReS1KhKVvzJHLE,1846
-arcpyext/_version.py,sha256=rTwgJ3uocAHs8Pt6NmZhiMrmvHQbwjyNh8Kfci1kVvs,191
+arcpyext/_version.py,sha256=ohKD_e-0-E-ejl89YZIOMpUG9QS31KEqFnzlCJjwjfQ,191
 arcpyext/_json/__init__.py,sha256=Mjzw6XfGzF0M67H9r7gA2ObtnYf7GvPw_UrtvGV1iDU,75
 arcpyext/_json/json_enum.py,sha256=YKZWw6KMcRVd5kAHXRRgPpQoMf7ddjpbWMU09Wbcj6U,805
 arcpyext/_json/to_json_encoder.py,sha256=q9UvUCgl2OD9K4OCBVPOoCpQQ6_GT7wXpEofVNOGlVg,823
 arcpyext/_native/__init__.py,sha256=FJh3H1znE_NK130TLtyDJR6teSlzW7OZAuDhR61y8JY,395
 arcpyext/_native/_dotnet.py,sha256=Rtu9EuPH_JV_nbyjHSoIAuW-OuXsHMRNuFcl04nOv30,4156
 arcpyext/_native/arcgispro.py,sha256=Ofq2k72l8-qWPP18sGknrLZX0o5WDzs252aocscS_f8,2135
 arcpyext/_native/arcobjects.py,sha256=cBh42iX3tfpcKbao_uMzMrRlMcqOBq-HhgxN_WWDA10,2409
+arcpyext/_str/ExtendedFormatter.py,sha256=6eOCkwVEtt1cpLisjY5vbAeJKGHp66O_HgQSBPDBDSk,1301
+arcpyext/_str/__init__.py,sha256=YB44fTvSfzI7m0OP5ZF77s0JiGDZoLRbH2rY9p4UWFQ,104
 arcpyext/conversion/ToCsv.py,sha256=OE_YodduTpAOfsuLMzkZpHD6V8kwnfeJtra8-KdIWB0,1799
 arcpyext/conversion/ToGeoPackage.py,sha256=LMg3bm2sCZtfRuI7mhsxxWBFrx2fV4u1-Yq1Funh7a4,3747
 arcpyext/conversion/ToKml.py,sha256=x-d1lfTKavKzKMY9IukyfBTpwVZOMunZlHQANKV33bA,1916
 arcpyext/conversion/ToMapInfoTab.py,sha256=OD8PYCZAvUEavzF6FcqueQySJ0zZGv5WHy3anIWiNw0,2813
 arcpyext/conversion/ToOfficeOpenXmlWorkbook.py,sha256=zJJYXso2j4knHcgCuaIjRWkhaFv32PfDUV5oID22dUw,7848
 arcpyext/conversion/ToShapefile.py,sha256=6EN1AkaXRU2uPuZpmhvBZiXXQ2zcXapbHl722GiZwbk,2280
 arcpyext/conversion/_ConvertBase.py,sha256=diEBSlobBdwpscTn01tqSNeY9577J3OO-LIvY2bvEno,5586
@@ -30,15 +32,15 @@
 arcpyext/exceptions/serv_def_draft_create_error.py,sha256=rlHjSuFDp6FoUYgGGz_vpyTL2J0-x1q4XVPNKBC09g0,598
 arcpyext/exceptions/unmapped_data_source_error.py,sha256=g9Pax-3bsJqoMur7AwCaKTJB2-KmPBo8Ksdqnp87L64,597
 arcpyext/exceptions/unsupported_layer_error.py,sha256=RRBH5Q9OD6IJcm3UMOh1tVLTmGNqCAqZ-uAP7PitxK0,595
 arcpyext/mapping/__init__.py,sha256=qWYpj_JEqUYFNM_X1cvzmXES3y70aPskoW7VLMtkBis,23
 arcpyext/mapping/_compare_helpers.py,sha256=7oZF8ZDsTaNLC1VIEDYPiFZv0mxvBpeIzhgJ8HpsMPg,2416
 arcpyext/mapping/_mapping.py,sha256=W2mWkc_NT9OZwvFnTNXHx24Ubq3FQXLWHsjDbNrD6po,17387
 arcpyext/mapping/_mapping2.py,sha256=cKtx-c_3FBP7OXhT9VZIng0uloL_IlPxrkjfQ0Pz09A,25585
-arcpyext/mapping/_mapping3.py,sha256=9mWzlo04OmjBy5GkBokpYp6YzRU5gv2veB7J7PhTqP4,11451
+arcpyext/mapping/_mapping3.py,sha256=xrUBwf1lzV2Utde3E0wiXMgPYEkhnTS4ofdZGO6TwSY,13027
 arcpyext/mapping/_mapping_helpers.py,sha256=aP6-nTatW4TqachYGt-7jU_-U2n069D69_onoes96dw,2383
 arcpyext/mapping/compare_types.py,sha256=IGA1H4GAUgjOwOy830E-39WClKOXu6flRWNFtNxffsw,7850
 arcpyext/mapping/_cim/__init__.py,sha256=feqUuTem8LHfYtXu4dBi3Q36Njg9kW1Mk-qGTKBGEN4,35
 arcpyext/mapping/_cim/factories.py,sha256=r6prCb5hoElQ2PzAEFndmxwho3WlZp2bREz8bcPm5Xc,1117
 arcpyext/mapping/_cim/helpers.py,sha256=2EIjNkUmjtYMkABqJfXgA-rC1g-m7A6u4g762O4Cg9U,1479
 arcpyext/mapping/_cim/layers.py,sha256=t5fDPwaBap72xCz31FrxuYwfjGFC_QhVEx-PI7GZGuo,2856
 arcpyext/mapping/_cim/pro_map.py,sha256=l_V2_n8h2tvmrTeY7XwFQuizzQm8n3vmCJQRkbq62Y8,3118
@@ -46,12 +48,12 @@
 arcpyext/mapping/_cim/tables.py,sha256=ahR8-CA5LM385EwdJxmeee8S2122d_Hht8vdE_5bfus,2037
 arcpyext/publishing/__init__.py,sha256=25z0Ft2YbAAeTKkwQ8f9niFYisdy3gTa7mODkTESp5I,369
 arcpyext/publishing/_publishing.py,sha256=8IIMpE_CQM9-SCHxB_hsmNHdpE-YC_pq0AdU0H18lvc,5861
 arcpyext/schematransform/__init__.py,sha256=ELUkW8ADD1afaS-3rEq9kdlNHuKWZRV8XYzQYfAe2U8,53
 arcpyext/schematransform/_schematransform.py,sha256=46-asLRDt0cAbarWumpdu_5yTwuBel-8cLY4SfF5cnY,22822
 arcpyext/toolbox/PythonToolbox.py,sha256=iSrfnlqdKle-LHiUhVILrlrpCZbXY_bv4CH_Mbd_MnA,5155
 arcpyext/toolbox/__init__.py,sha256=T-MUfdRjBKG3noQh7IAjBoDwDLrPwPa6L2Q7yvgmy1g,42
-arcpyext-0.7.8.dist-info/LICENSE,sha256=jRVcUafc5g93kZT8M_seqpfjvTnyqaTF9_KjXZZdg4I,1520
-arcpyext-0.7.8.dist-info/METADATA,sha256=rLmVX0nWNaWifoVe1wfSR72rqs5ZJhSyz8_95QRPEaA,13442
-arcpyext-0.7.8.dist-info/WHEEL,sha256=JZXtYepZFsf4IoivNpnSgKIc4qTHan08DRd56koo_DM,116
-arcpyext-0.7.8.dist-info/top_level.txt,sha256=otv9ExFe2-U4B2Mg32CJQqaRVrKr5P9pmk6GREwc4CY,9
-arcpyext-0.7.8.dist-info/RECORD,,
+arcpyext-0.7.9.dist-info/LICENSE,sha256=jRVcUafc5g93kZT8M_seqpfjvTnyqaTF9_KjXZZdg4I,1520
+arcpyext-0.7.9.dist-info/METADATA,sha256=JiohR-VA9QRqD7Bh-2aFz0rleNPKuTre6UgHX6ns31k,13442
+arcpyext-0.7.9.dist-info/WHEEL,sha256=JZXtYepZFsf4IoivNpnSgKIc4qTHan08DRd56koo_DM,116
+arcpyext-0.7.9.dist-info/top_level.txt,sha256=otv9ExFe2-U4B2Mg32CJQqaRVrKr5P9pmk6GREwc4CY,9
+arcpyext-0.7.9.dist-info/RECORD,,
```

