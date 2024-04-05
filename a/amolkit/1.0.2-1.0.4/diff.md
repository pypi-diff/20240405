# Comparing `tmp/amolkit-1.0.2.tar.gz` & `tmp/amolkit-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amolkit-1.0.2.tar", last modified: Fri Aug 11 15:14:22 2023, max compression
+gzip compressed data, was "amolkit-1.0.4.tar", last modified: Thu Apr  4 23:24:05 2024, max compression
```

## Comparing `amolkit-1.0.2.tar` & `amolkit-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 15:14:22.121336 amolkit-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-11 15:14:12.000000 amolkit-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-11 15:14:22.121336 amolkit-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-11 15:14:12.000000 amolkit-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 15:14:22.121336 amolkit-1.0.2/amolkit/
--rw-r--r--   0 runner    (1001) docker     (123)    32064 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/EleInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/genic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/getEleInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21189 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)    16183 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/molsystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/moltransform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/psf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/stringmanip.py
--rw-r--r--   0 runner    (1001) docker     (123)    15583 2023-08-11 15:14:12.000000 amolkit-1.0.2/amolkit/topology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 15:14:22.121336 amolkit-1.0.2/amolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-11 15:14:22.000000 amolkit-1.0.2/amolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-11 15:14:22.000000 amolkit-1.0.2/amolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-11 15:14:22.000000 amolkit-1.0.2/amolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-11 15:14:21.000000 amolkit-1.0.2/amolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-11 15:14:22.000000 amolkit-1.0.2/amolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-11 15:14:22.121336 amolkit-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-08-11 15:14:12.000000 amolkit-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-11 15:14:22.121336 amolkit-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-08-11 15:14:12.000000 amolkit-1.0.2/tests/test_amolkit.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-04 23:24:05.636194 amolkit-1.0.4/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.4/LICENSE
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-04-04 23:24:05.636194 amolkit-1.0.4/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.4/README.md
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-04 23:24:05.636194 amolkit-1.0.4/amolkit/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.4/amolkit/EleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.4/amolkit/__init__.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.4/amolkit/amolsystem.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3406 2024-04-03 21:23:50.000000 amolkit-1.0.4/amolkit/atom.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.4/amolkit/genic.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3309 2023-08-10 06:31:01.000000 amolkit-1.0.4/amolkit/getEleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.4/amolkit/getring.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      313 2023-08-10 20:56:51.000000 amolkit-1.0.4/amolkit/misc.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    22858 2024-04-03 22:23:43.000000 amolkit-1.0.4/amolkit/molecule.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.4/amolkit/moltransform.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8967 2023-08-19 01:39:50.000000 amolkit-1.0.4/amolkit/parameter.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.4/amolkit/psf.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3254 2023-08-16 19:17:38.000000 amolkit-1.0.4/amolkit/stringmanip.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    17660 2023-08-19 01:57:53.000000 amolkit-1.0.4/amolkit/topology.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-04-04 23:24:05.636194 amolkit-1.0.4/amolkit.egg-info/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-04-04 23:24:05.000000 amolkit-1.0.4/amolkit.egg-info/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      454 2024-04-04 23:24:05.000000 amolkit-1.0.4/amolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-04-04 23:24:05.000000 amolkit-1.0.4/amolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.4/amolkit.egg-info/not-zip-safe
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-04-04 23:24:05.000000 amolkit-1.0.4/amolkit.egg-info/top_level.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-04-04 23:24:05.636194 amolkit-1.0.4/setup.cfg
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2023-08-16 22:08:35.000000 amolkit-1.0.4/setup.py
```

### Comparing `amolkit-1.0.2/LICENSE` & `amolkit-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.2/amolkit/EleInfo.py` & `amolkit-1.0.4/amolkit/EleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.2/amolkit/genic.py` & `amolkit-1.0.4/amolkit/genic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import os, sys
 import numpy as np
 from operator import sub
 from collections import OrderedDict
 
-class GetBondAngleDihedral():
-    def __init__():
-        """Initialize"""
-
-    def GetBondDict(iatomname,bondlist,onlyatoms=True):
+class ICs():
+    """
+    Get Molecular Graph and Internal Coordinate List
+    """
+    @staticmethod
+    def getBondDict(iatomname,bondlist,onlyatoms=True):
         """
         Generate Dict with atomname as keys and bonded atoms as values
         Arguments:
             iatomname: Dictionary of atom indices containing atomnames
             bondlist: List of list of bonds obtained from reading mol2 format
             onlyatoms: If true, output dictionary will not have lone pair names as keys
         Returns:
@@ -72,49 +72,52 @@
         if alpbond_dict != None:
             abond_dict=patch_dict(anolpbond_dict,alpbond_dict)
             return({"aBond":abond_dict,"aNoLPBond":anolpbond_dict,"aLPBond":alpbond_dict})
         else:
             abond_dict=anolpbond_dict
             return({"aBond":abond_dict})
 
-    def GetBonds(aatomname,bond_dict):
+    @staticmethod
+    def getBonds(aatomname,bond_dict):
         """
         Make a list of list of bond pairs with atomnames and atomindices
         Arguments:
             aatomname: Dictionary of atom names containing atomindices
-            bond_dict: BondDict obtained from GetBondDict
+            bond_dict: BondDict obtained from getBondDict
         Returns:
             abondlist: list of list of bond pairs with atomnames
             ibondlist: list of list of bond pairs with atomindices
         """
         abondlist = []
         ibondlist = []
         for key,value in list(bond_dict.items()):
             for val in value:
                 if [val,key] not in abondlist:
                     abondlist.append([key,val])
                     ibondlist.append([int(aatomname[key]),int(aatomname[val])])
         return(abondlist,ibondlist)
 
-    def GetAngles(aatomname,bond_dict):
+    @staticmethod
+    def getAngles(aatomname,bond_dict):
         """Make a list of list of angle triplets with atomnames and atomindices"""
         aanglelist = []
         ianglelist = []
         for k0,v0 in list(bond_dict.items()):
             if len(v0) > 1:
                 for i in range(0,(len(v0)-1)):
                     ang2 = k0
                     ang1 = v0[i]
                     for j in range(i+1,len(v0)):
                         ang3 = v0[j]
                         aanglelist.append([ang1,ang2,ang3])
                         ianglelist.append([int(aatomname[ang1]),int(aatomname[ang2]),int(aatomname[ang3])])
         return(aanglelist,ianglelist)
 
-    def GetDihedrals(aatomname,bond_dict):
+    @staticmethod
+    def getDihedrals(aatomname,bond_dict):
         """Make a list of list of dihedral quads with atomnames and atomindices"""
         adihedrallist = []
         idihedrallist = []
         for k0,v0 in list(bond_dict.items()):
             dih0 = k0
             for k1 in v0:
                 if bond_dict.get(k1) and len(bond_dict[k1]) != 1:
@@ -126,15 +129,16 @@
                                 if k3 != dih1 and k3 != dih0:
                                     dih3 = k3
                                     if [dih3,dih2,dih1,dih0] not in adihedrallist:
                                         adihedrallist.append([dih0,dih1,dih2,dih3])
                                         idihedrallist.append([int(aatomname[dih0]),int(aatomname[dih1]),int(aatomname[dih2]),int(aatomname[dih3])])
         return(adihedrallist,idihedrallist)
 
-    def GetOnefives(aatomname,bond_dict):
+    @staticmethod
+    def getOnefives(aatomname,bond_dict):
         """Make a list of list of onefives 5 entries with atomnames and atomindices"""
         aonefivelist = []
         ionefivelist = []
         for k0,v0 in list(bond_dict.items()):
             skip=[k0,*v0]
             of0 = k0
             for k1 in v0:
@@ -149,100 +153,71 @@
                                     for k4 in bond_dict[k3]:
                                         if k4 != of2 and k4 != of1 and k4 != of0:
                                             of4 = k4
                                             if [of4,of3,of2,of1,of0] not in aonefivelist:
                                                 aonefivelist.append([of0,of1,of2,of3,of4])
                                                 ionefivelist.append([int(aatomname[of0]),int(aatomname[of1]),int(aatomname[of2]),int(aatomname[of3]),int(aatomname[of4])])
         return(aonefivelist,ionefivelist)
-
-    def GetImpropers(aatomname,bond_dict):
+    
+    @staticmethod
+    def getImpropers(aatomname,bond_dict):
         aimplist=[]
         iimplist=[]
         for key,val in list(bond_dict.items()):
             if len(val)==3:
                 aimplist.append([key,*val])
                 iimplist.append([int(aatomname[key]),int(aatomname[val[0]]),int(aatomname[val[1]]),int(aatomname[val[2]])])
         return (aimplist,iimplist)
 
-def generateBonds(elementnames=[],coordinates=[]):
+class ICValue():
     """
-    Expects names and coordinates 
+    Get Distance, Angle and Dihedral Value by provides a set of 2/3/4 coordinates
     """
-    from amolkit import getEleInfo as gei 
+    @staticmethod
+    def getBondValue(coord1,coord2):
+        coord1=np.array(coord1,dtype='float32')
+        coord2=np.array(coord2,dtype='float32')
+    
+        xyz = np.array(list(map(sub,coord1,coord2)))
+        distance = np.linalg.norm(xyz)
+        distance = round(distance,4)
+        return distance
+    
+    @staticmethod
+    def getAngleValue(coord1,coord2,coord3):
+        coord1=np.array(coord1,dtype='float32')
+        coord2=np.array(coord2,dtype='float32')
+        coord3=np.array(coord3,dtype='float32')
+    
+        bav = coord1 - coord2 
+        bcv = coord3 - coord2 
+        cosine_angle = np.dot(bav, bcv) / (np.linalg.norm(bav) * np.linalg.norm(bcv))
+        angle = np.arccos(cosine_angle)
+        angle = np.degrees(angle)
+        angle = round(angle,3)
+        return angle
+    
+    @staticmethod
+    def getDihedralValue(coord1,coord2,coord3,coord4):
+        coord1=np.array(coord1,dtype='float32')
+        coord2=np.array(coord2,dtype='float32')
+        coord3=np.array(coord3,dtype='float32')
+        coord4=np.array(coord4,dtype='float32')
+        b0 = -1.0*(coord2 - coord1)
+        b1 = coord3 - coord2 
+        b2 = coord4 - coord3 
+        b0xb1 = np.cross(b0, b1)
+        b1xb2 = np.cross(b2, b1)
+        b0xb1_x_b1xb2 = np.cross(b0xb1, b1xb2)
+        y = np.dot(b0xb1_x_b1xb2, b1)*(1.0/np.linalg.norm(b1))
+        x = np.dot(b0xb1, b1xb2)
+        dihedral = np.arctan2(y, x)
+        dihedral = np.degrees(dihedral)
+        dihedral = round(dihedral,3)
+        return dihedral
+    
+def getICValue(coord1=[],coord2=[],coord3=[],coord4=[]):
+    if coord1 and coord2 and not coord3 and not coord4: return ICValue.getBondValue(coord1,coord2)
+    if coord1 and coord2 and coord3 and not coord4: return ICValue.getAngleValue(coord1,coord2,coord3)
+    if coord1 and coord2 and coord3 and coord4: return ICValue.getDihedralValue(coord1,coord2,coord3,coord4)
+
 
-    if elementnames and coordinates and len(elementnames) != len(coordinates):
-        raise IndexError("names list and coordinate list don't match")
-     
-    coordinates = np.array(coordinates,dtype ='float32')
-
-    delta = [None]*3
-    for i in range(3):
-       coord = coordinates[:,i]
-       delta[i] = coord - coord.reshape((len(coord),1))
-
-    dist = delta[0]**2 + delta[1]**2 + delta[2]**2 + 10. * np.identity(len(coordinates))
-
-    radius = []
-    for el in elementnames:
-        radius.append(gei.covrad_by_atomsymbol(el)) 
-    radius = np.array(radius, dtype='float32')
-
-    radcov = (radius + radius.reshape((len(radius),1)))*2
-    bonded = np.array(np.where(dist - radcov<0.)).transpose()
-    distmat = np.sqrt(dist[bonded[:,0],bonded[:,1]])
-    
-    # amolkit indices for molecules starts from 1
-    bondindices=[]
-    for b in bonded:
-        bondindices.append(list(map(lambda x:x+1,b)))
-
-    bondinfo={}
-    bondinfo["radcov"]         = radcov
-    bondinfo["pybondindices"]  = bonded
-    bondinfo["distmat"]        = distmat
-    bondinfo["bondindices"]    = bondindices
-    return bondinfo 
-
-def getBondValue(coord1,coord2):
-    coord1=np.array(coord1,dtype='float32')
-    coord2=np.array(coord2,dtype='float32')
-
-    xyz = np.array(list(map(sub,coord1,coord2)))
-    distance = np.linalg.norm(xyz)
-    distance = round(distance,4)
-    return distance
-
-def getAngleValue(coord1,coord2,coord3):
-    coord1=np.array(coord1,dtype='float32')
-    coord2=np.array(coord2,dtype='float32')
-    coord3=np.array(coord3,dtype='float32')
-
-    bav = coord1 - coord2 
-    bcv = coord3 - coord2 
-    cosine_angle = np.dot(bav, bcv) / (np.linalg.norm(bav) * np.linalg.norm(bcv))
-    angle = np.arccos(cosine_angle)
-    angle = np.degrees(angle)
-    angle = round(angle,3)
-    return angle
-
-def getDihedralValue(coord1,coord2,coord3,coord4):
-    coord1=np.array(coord1,dtype='float32')
-    coord2=np.array(coord2,dtype='float32')
-    coord3=np.array(coord3,dtype='float32')
-    coord4=np.array(coord4,dtype='float32')
-    b0 = -1.0*(coord2 - coord1)
-    b1 = coord3 - coord2 
-    b2 = coord4 - coord3 
-    b0xb1 = np.cross(b0, b1)
-    b1xb2 = np.cross(b2, b1)
-    b0xb1_x_b1xb2 = np.cross(b0xb1, b1xb2)
-    y = np.dot(b0xb1_x_b1xb2, b1)*(1.0/np.linalg.norm(b1))
-    x = np.dot(b0xb1, b1xb2)
-    dihedral = np.arctan2(y, x)
-    dihedral = np.degrees(dihedral)
-    dihedral = round(dihedral,3)
-    return dihedral
-
-def getICvalue(coord1=[],coord2=[],coord3=[],coord4=[]):
-    if coord1 and coord2 and not coord3 and not coord4: return getBondValue(coord1,coord2)
-    if coord1 and coord2 and coord3 and not coord4: return getAngleValue(coord1,coord2,coord3)
-    if coord1 and coord2 and coord3 and coord4: return getDihedralValue(coord1,coord2,coord3,coord4)
```

### Comparing `amolkit-1.0.2/amolkit/getEleInfo.py` & `amolkit-1.0.4/amolkit/getEleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.2/amolkit/molecule.py` & `amolkit-1.0.4/amolkit/molecule.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import sys
 from os.path import join as opj
 from operator import sub
 from collections import OrderedDict
 from amolkit import getEleInfo as gei 
-from amolkit.stringmanip import updateAtomnames 
+from amolkit.stringmanip import updateAtomNames 
 from amolkit import misc
 
 def crdreadfmt(crdtype='extended'):
     if crdtype[0:3].lower() == 'ext':
         #fortran_format = '(2I10,2X,A8,2X,A8,3F20.10,2X,A8,2X,A8,F20.10)'
         indexdict={'srlno':[0,10],'resid':[10,20],'resn':[22,30],'aname':[32,40],
             'x':[40,60],'y':[60,80],'z':[80,100],'segn':[102,110],'segid':[112,120],'tfac':[120,140]}
@@ -61,15 +61,15 @@
         self.atommass_byId=OrderedDict()
         self.bondindices=[]
         self.energy=None
         self.natoms=None
         self.nmoltoms=None
         self.totalcharge=None
 
-    def readmol2(self,filename,istart=None,bio=True):
+    def readmol2(self,filename,istart=None,resid=None,bio=True):
         molblock = open(filename,"r").readlines()
         foundatm=False
         foundbnd=False
         if not istart: istart = 0
         ind=0
         for line in molblock:
             field = line.split()
@@ -224,15 +224,15 @@
         allnames = list(map(lambda x:x.upper(), self.atomname_byIdx.values())) 
         if len(allnames) ==  len(list(set(allnames))):
             self.atomindex_byId = {v: k for k, v in self.atomname_byIdx.items()}
 
         onlyatoms = [a for a in self.atomname_byIdx.values() if a[0:2].upper() != "LP" and a[0] != "D"]
         self.natoms = len(onlyatoms)
 
-    def readxyz(self,filename,istart=None,bio=True):
+    def readxyz(self,filename,istart=None,resid=None,bio=True):
         if not istart: istart = 0
         ind = 0
         molblock = open(filename,"r").readlines()
         for i,line in enumerate(molblock):
             field = line.split()
             if i == 0: self.nmolatoms = int(field[0]) 
             if i == 1: continue # Second line is comment
@@ -251,41 +251,65 @@
         allnames = list(map(lambda x:x.upper(), self.atomname_byIdx.values())) 
         if len(allnames) ==  len(list(set(allnames))):
             self.atomindex_byId = {v: k for k, v in self.atomname_byIdx.items()}
 
         onlyatoms = [a for a in self.atomname_byIdx.values() if a[0:2].upper() != "LP" and a[0] != "D"]
         self.natoms = len(onlyatoms)
  
-    def genMol(self,atomnames:list,atomcoords:list,**kwargs):
-        if not isinstance(atomnames,list) and not isinstance(atomcoords,list):
-            raise ValueError ("Provide list of atomnames and list of coords")
-        if len(atomnames) != len(atomcoords):
-            raise IndexError ("Length of atomnames and coords are not same.")
-        self.nmolatoms = len(atomname) 
+    @staticmethod
+    def generateBonds(elementnames=[],coordinates=[]):
+        """
+        Expects list of names and coordinates of same length 
+        """
+        import numpy as np
+        from amolkit import getEleInfo as gei 
+    
+        if elementnames and coordinates and len(elementnames) != len(coordinates):
+            raise IndexError("names list and coordinate list don't match")
+         
+        coordinates = np.array(coordinates,dtype ='float32')
+    
+        delta = [None]*3
+        for i in range(3):
+           coord = coordinates[:,i]
+           delta[i] = coord - coord.reshape((len(coord),1))
+    
+        dist = delta[0]**2 + delta[1]**2 + delta[2]**2 + 10. * np.identity(len(coordinates))
+    
+        radius = []
+        for el in elementnames:
+            radius.append(gei.covrad_by_atomsymbol(el)) 
+        radius = np.array(radius, dtype='float32')
+    
+        radcov = (radius + radius.reshape((len(radius),1)))*2
+        bonded = np.array(np.where(dist - radcov<0.)).transpose()
+        distmat = np.sqrt(dist[bonded[:,0],bonded[:,1]])
         
-        for i in range(len(atomnames)): 
-            ind = i + 1
-            self.atomcoord_byIdx[self.atomindex_byId[ind]]= atomcoords[i] 
-            self.atomserial_byIdx[self.atomindex_byId[ind]]= ind 
-            self.atomele_byIdx[self.atomindex_byId[ind]]=  gei.atomsymbol_by_anyatomname(atomnames[i]) 
-            self.atomresn_byIdx[self.atomindex_byId[ind]]= "RESN" 
-            self.atomresid_byIdx[self.atomindex_byId[ind]]= 1 
-            self.atomsegn_byIdx[self.atomindex_byId[ind]]= "SEGN" 
+        # amolkit indices for molecules starts from 1
+        bondindices=[]
+        for b in bonded:
+            bondindices.append(list(map(lambda x:x+1,b)))
+    
+        bondinfo={}
+        bondinfo["radcov"]         = radcov
+        bondinfo["pybondindices"]  = bonded
+        bondinfo["distmat"]        = distmat
+        bondinfo["bondindices"]    = bondindices
+        return bondinfo 
 
     def genBonds(self):
-        from amolkit.genic import generateBonds
-        self.bondindices=generateBonds(list(self.atomele_byIdx.values()),list(self.atomcoord_byIdx.values()))["bondindices"]
+        self.bondindices=self.generateBonds(list(self.atomele_byIdx.values()),list(self.atomcoord_byIdx.values()))["bondindices"]
 
-    def autoupdateMolAtomnames(self):
-        atomnames=updateAtomnames(list(self.atomname_byIdx.values()))
+    def autoupdateAtomNames(self):
+        atomnames=updateAtomNames(list(self.atomname_byIdx.values()))
         for i in range(len(atomnames)):
             ind = i + 1
             self.atomname_byIdx[ind] = atomnames[i]
 
-    def updateMolAtomnamesWith(self,atomnames):
+    def updateAtomNamesWith(self,atomnames):
         if not isinstance(atomnames,list) or len(atomnames) != len(list(self.atomname_byIdx.values())):
             raise IndexError ("Length of atomnames not same as molecule atoms.")
         for i in range(len(atomnames)):
             ind = i + 1
             self.atomname_byIdx[ind] = atomnames[i]
 
     def readMolecule(self,filename,istart=None,resid=None,bio=True):
@@ -293,16 +317,35 @@
         extension = misc.getExtension(filename)
         if not filestatus:
             raise RuntimeError ("Error reading file")
         if extension not in ["xyz","mol2","pdb","crd"]: 
             raise RuntimeError ("Cant read this file format")
         if extension == "pdb":  self.readpdb(filename,istart,resid,bio)
         if extension == "crd":  self.readcrd(filename,istart,resid,bio)
-        if extension == "mol2": self.readmol2(filename,istart,bio)
-        if extension == "xyz":  self.readxyz(filename,istart,bio)
+        if extension == "mol2": self.readmol2(filename,istart,resid,bio)
+        if extension == "xyz":  self.readxyz(filename,istart,resid,bio)
+
+def genMol(atomnames:list,atomcoords:list,**kwargs):
+    if not isinstance(atomnames,list) and not isinstance(atomcoords,list):
+        raise ValueError ("Provide list of atomnames and list of coords")
+    if len(atomnames) != len(atomcoords):
+        raise IndexError ("Length of atomnames and coords are not same.")
+    
+    mol = Molecule()
+    mol.nmolatoms = len(atomname) 
+    
+    for i in range(len(atomnames)): 
+        ind = i + 1
+        mol.atomcoord_byIdx[ind] = atomcoords[i] 
+        mol.atomserial_byIdx[ind]= ind 
+        mol.atomele_byIdx[ind]   = gei.atomsymbol_by_anyatomname(atomnames[i]) 
+        mol.atomresn_byIdx[ind]  = "RESN" 
+        mol.atomresid_byIdx[ind] = 1 
+        mol.atomsegn_byIdx[ind]  = "SEGN" 
+    return mol
 
 def coordline(molecule,ind,serialnum=None,resid=None):
     '''
     For index = ind in molinstance, this function assigns variables required 
     for writing coordinate line in crd/pdb/xyz/mol2
     Arguments:
         molinstance: instance of Molecule class with preloaded molecule information
@@ -363,17 +406,20 @@
 
     if molecule.atomcharge_byIdx and ind in molecule.atomcharge_byIdx.keys():
         cpvar["charge"] = molecule.atomcharge_byIdx[ind] 
     else:    
         cpvar["charge"] = 0.0 
     return cpvar 
  
-def writecrd(molecule,fileout=None,nolpd=False):
+def writecrd(molecule,fileout=None,nolpd=False,comment=None):
     ocrdfile = open(fileout,"w")
-    ocrdfile.write("* Generated by amolkit\n")
+    if comment:
+        ocrdfile.write("* %s\n"%(comment))
+    else:
+        ocrdfile.write("* Generated by amolkit\n")
     ocrdfile.write("* \n")
     if not nolpd:
         ocrdfile.write("%10i  EXT\n" %(molecule.nmolatoms))
         for i in range(molecule.nmolatoms):
             ind=i+1
             cdict = coordline(molecule,ind)
             ocrdfile.write(crdwrtfmt(cdict)+"\n")
@@ -390,18 +436,21 @@
                 serialnum = serialnum + 1
             cdict = coordline(molecule,ind,serialnum=serialnum)
             ocrdfile.write(crdwrtfmt(cdict)+"\n")
         ocrdfile.close()
     prntscr = " ".join((str(fileout),"created"))
     print(prntscr) 
 
-def writepdb(molecule,fileout=None,nolpd=False):
+def writepdb(molecule,fileout=None,nolpd=False,comment=None):
     #molecule = molecule()
     opdbfile = open(fileout,"w")
-    opdbfile.write("REMARK   1 Generated by amolkit\n")
+    if comment:
+        opdbfile.write("REMARK   %s\n"%(comment))
+    else:
+        opdbfile.write("REMARK   1 Generated by amolkit\n")
     if not nolpd:
         for i in range(molecule.nmolatoms):
             ind=i+1
             cdict = coordline(molecule,ind)
             opdbfile.write(pdbwrtfmt(cdict)+"\n")
     else:
         serialnum = 0
@@ -416,33 +465,39 @@
             opdbfile.write(pdbwrtfmt(pdict)+"\n")
     opdbfile.write("TER\n")
     opdbfile.write("END\n")
     opdbfile.close()
     prntscr = " ".join((str(fileout),"created"))
     print(prntscr) 
 
-def writexyz(molecule,fileout=None,nolpd=False):
+def writexyz(molecule,fileout=None,nolpd=False,comment=None):
     #molecule = molecule()
     if fileout == None:
        fileout = "molecule.xyz"
        print ("No output xyzfile name provided. Writing in molecule.xyz") 
 
     oxyzfile = open(fileout,"w")
     if not nolpd:
         oxyzfile.write("%10i \n" %(molecule.nmolatoms))
-        oxyzfile.write("Generated by amolkit\n")
+        if comment:
+            oxyzfile.write("%s\n"%(comment))
+        else:
+            oxyzfile.write("Generated by amolkit\n")
         for i in range(molecule.nmolatoms):
             ind=i+1
             xdict = coordline(molecule,ind)
             oxyzfile.write(xyzwrtfmt(xdict)+"\n")
         oxyzfile.close()
     else:
         serialnum = 0
         oxyzfile.write("%10i\n" %(molecule.natoms))
-        oxyzfile.write("Generated by amolkit\n")
+        if comment:
+            oxyzfile.write("%s\n"%(comment))
+        else:
+            oxyzfile.write("Generated by amolkit\n")
         for i in range(molecule.nmolatoms):
             ind=i+1
             checkatm = molecule.atomname_byIdx[ind]
             if checkatm[0:1] == "D" or checkatm[0:2] == "LP":
                 serialnum = serialnum
             else:    
                 serialnum = serialnum + 1
```

### Comparing `amolkit-1.0.2/amolkit/molsystem.py` & `amolkit-1.0.4/amolkit/amolsystem.py`

 * *Files 25% similar despite different names*

```diff
@@ -52,19 +52,19 @@
             print ("Charmm Parameters obtained, but not loaded on molecular ics. You should load topology prior to loading parameters")
             return
         
         # Get list of bond angle and dihedral
         bondindices=[]
         for ba,bb in self.bonds:
             bondindices.append([self.atomindex_byId[ba],self.atomindex_byId[bb]])
-        bondgraph = genic.GetBondAngleDihedral.GetBondDict(self.atomname_byIdx,bondindices)["aNoLPBond"]
-        bondnames,_ = genic.GetBondAngleDihedral.GetBonds(self.atomindex_byId,bondgraph)
+        bondgraph = genic.ICs.getBondDict(self.atomname_byIdx,bondindices)["aNoLPBond"]
+        bondnames,_ = genic.ICs.getBonds(self.atomindex_byId,bondgraph)
         if autogenangdih:
-            anglenames,_ = genic.GetBondAngleDihedral.GetAngles(self.atomindex_byId,bondgraph)
-            dihedralnames,_ = genic.GetBondAngleDihedral.GetDihedrals(self.atomindex_byId,bondgraph)
+            anglenames,_ = genic.ICs.getAngles(self.atomindex_byId,bondgraph)
+            dihedralnames,_ = genic.ICs.getDihedrals(self.atomindex_byId,bondgraph)
         else:
             anglenames = deepcopy(self.angles)
             dihedralnames = deepcopy(self.dihedrals)
             
         # Assign parameters to bond, angle and dihedral
         # Initialize parameter lists
         self.bondparam = deepcopy(bondnames)
@@ -93,49 +93,49 @@
                 self.superdihparam[nd].append(None) 
                 nd=nd+1
                 
         # Assign now
         for i,bl in enumerate(bondnames):
             parainq = [self.atomtype_byId[bl[0]], self.atomtype_byId[bl[1]]]
             for j, listele in enumerate(param.charmmParameter['BONDS']):
-               listf = listele[0:2]
-               listb = listele[0:2][::-1]
-               if parainq == listf or parainq == listb:
-                   self.bondparam[i][2] = listele[2] 
-                   self.bondparam[i][3] = listele[3]
-                   self.bondparam[i][4] = listele[4]
+                listf = listele[0:2]
+                listb = listele[0:2][::-1]
+                if parainq == listf or parainq == listb:
+                    self.bondparam[i][2] = listele[2] 
+                    self.bondparam[i][3] = listele[3]
+                    self.bondparam[i][4] = listele[4]
 
         for i,al in enumerate(anglenames):
             parainq = [self.atomtype_byId[al[0]], self.atomtype_byId[al[1]],self.atomtype_byId[al[2]]]
             for j, listele in enumerate(param.charmmParameter['ANGLES']):
-               listf = listele[0:3]
-               listb = listele[0:3][::-1]
-               if parainq == listf or parainq == listb:
-                   if len(listele) == 7:
-                       self.angleparam[i][3] = listele[3]
-                       self.angleparam[i][4] = listele[4]
-                       self.angleparam[i][5] = listele[5]
-                   elif len(listele) == 9:
-                       self.angleparam[i][3] = listele[3]
-                       self.angleparam[i][4] = listele[4]
-                       self.angleparam[i][5] = listele[5]
-                       self.angleparam[i].append(listele[6])
-                       self.angleparam[i].append(listele[7])
+                listf = listele[0:3]
+                listb = listele[0:3][::-1]
+                if parainq == listf or parainq == listb:
+                    if len(listele) == 7:
+                        self.angleparam[i][3] = listele[3]
+                        self.angleparam[i][4] = listele[4]
+                        self.angleparam[i][5] = listele[5]
+                    elif len(listele) == 9:
+                        self.angleparam[i][3] = listele[3]
+                        self.angleparam[i][4] = listele[4]
+                        self.angleparam[i][5] = listele[5]
+                        self.angleparam[i].append(listele[6])
+                        self.angleparam[i].append(listele[7])
 
         for i,dl in enumerate(dihedralnames):
             parainq = [self.atomtype_byId[dl[0]], self.atomtype_byId[dl[1]],self.atomtype_byId[dl[2]],self.atomtype_byId[dl[3]]]
             for j, listele in enumerate(param.charmmParameter['DIHEDRALS']):
-               listf = listele[0:4]
-               listb = listele[0:4][::-1]
-               if parainq == listf or parainq == listb:
-                   #listele[5] is multiplicity
-                   index = i*6 + (int(listele[5])-1)
-                   self.superdihparam[index][5] = listele[4] 
-                   self.superdihparam[index][6] = listele[6] 
-                   self.superdihparam[index][7] = listele[7] 
+                listf = listele[0:4]
+                listb = listele[0:4][::-1]
+                if parainq == listf or parainq == listb:
+                    #listele[5] is multiplicity
+                    index = i*6 + (int(listele[5])-1)
+                    self.superdihparam[index][5] = listele[4] 
+                    self.superdihparam[index][6] = listele[6] 
+                    self.superdihparam[index][7] = listele[7] 
         
         # Get dihedral IC with same multiplicities as obtained in charmm parameter files
         # ==> But this also removes those entries for which no parameter is found.
         self.dihedralparam=[]
         for ent in self.superdihparam:
             if ent[5] != None:
                 self.dihedralparam.append(ent)
@@ -253,106 +253,7 @@
         for key,value in self.atomcoord_byId.items(): 
             self.atomcoord_byIdx[self.atomindex_byId[key]]= value 
             self.atomserial_byIdx[self.atomindex_byId[key]]= self.atomindex_byId[key]
             self.atomele_byIdx[self.atomindex_byId[key]]= self.atomele_byId[key]
             self.atomresn_byIdx[self.atomindex_byId[key]]= self.resname 
             self.atomresid_byIdx[self.atomindex_byId[key]]= 1 
             self.atomsegn_byIdx[self.atomindex_byId[key]]=self.resname 
-
-class genRDMolSmiles():
-    '''
-    This class is to create an RDMol object from the topology file. To generate initial coordinates for the molecule, you can run coordinates_fromrdmol , after you initialize the class.
-    '''
-
-    import numpy as np
-    try:
-        from rdkit import Chem
-        from rdkit.Chem import AllChem
-    except ImportError:
-        logging.warning('RDKit not found!')
-
-    def __init__(self,resi='resn',bonds=[],atomnames=[],smiles=None):
-        self.resname=resi
-        if isinstance(smiles,str):
-            self.__rdmol_smiles(smiles)
-        else:
-            raise ValueError('Either provide a bonds and atomnames list&dictionary or pass a smiles string.')
-
-    def __rdmol_smiles(self,smiles):
-        m=Chem.MolFromSmiles(smiles)
-        try:
-            Chem.SanitizeMol(m)
-        except ValueError:
-            pass
-        self.mol=m
-        #coordinates_fromrdmol()
-
-    def coordinates_fromrdmol(self,outpath,cortype='crd'):
-        AllChem.EmbedMolecule(m,useExpTorsionAnglePrefs=True,useBasicKnowledge=True)
-        AllChem.MMFFOptimizeMolecule(m)
-
-        #names not used but it is returned from this function by default
-        names,positions=mr.Molecule.readpdb(Chem.rdmolfiles.MolToPDBBlock(m).split('\n'))
-        self.coor=positions
-        with open(fileout,'w') as f:
-            if otype == 'crd':
-                f.write("*Created by FFParam\n*\n")
-                f.write("%10i  EXT\n" %len(self.rdmolnrs))
-            for i in self.rdmolnrs:
-                name=self.rdmolnrs[i]
-                xyz=list(positions[i])
-                nr=i+1
-                line=cw.crdline([nr,name]+xyz,resname=self.resname,segname=self.resname,returntype=otype)
-                f.write(line+'\n')
-        return(fileout)
-
-        if otype == 'mol2':
-            mol2=self.rdmoltomol2(m)
-            with open(fileout,'w') as f:
-                f.write(mol2)
-            return(fileout)
-        else:
-            logging.error('Other types from rdkit are not yet supported.')
-            return(None)
-
-    def rdmoltomol2(self,m):
-       # #Create a moltomol2 function that assigns unique names to each atom and embeds the residue name
-        pMol2Block =""
-        Chem.Kekulize(m)
-        mH =Chem.AddHs(m)
-        if mH != m:
-            m=mH
-        m.SetProp("_Name",self.resname)
-        try:
-           AllChem.EmbedMolecule(m,useExpTorsionAnglePrefs=True,useBasicKnowledge=True)
-        except ValueError:
-           logging.error("Cant create coordinates, hypervalency exists")
-           return
-        AllChem.MMFFOptimizeMolecule(m)
-        natoms=m.GetNumAtoms()
-        nbonds=m.GetNumBonds()
-        names,positions=mr.Molecule.readpdb(Chem.rdmolfiles.MolToPDBBlock(m).split('\n'))
-        pMol2Block = "@<TRIPOS>MOLECULE\n"
-        pMol2Block += "%s\n"%(m.GetProp("_Name"))
-        pMol2Block += " %d %d %d %d %d\n"%(natoms,nbonds,0,0,0)
-        pMol2Block += "SMALL\n"
-        pMol2Block += "GASTEIGER\n"
-        pMol2Block += "\n"
-        pMol2Block += "@<TRIPOS>ATOM\n"
-        for i, atom in enumerate(m.GetAtoms()):
-            atname = atom.GetSymbol()+str(i+1)
-            attype = atom.GetSymbol()
-            parchar= round(float(0),4)
-            xyz=list(positions[i])
-            pMol2Block += "%7d %7s %10.4f%10.4f%10.4f %5s%4s  %8s%10.4f\n"%(i+1,atname,xyz[0],xyz[1],xyz[2],attype,"1",self.resname.upper(),parchar)
-        pMol2Block += "@<TRIPOS>BOND\n"
-        for i, bi in enumerate(m.GetBonds()):
-             i1 = int(bi.GetBeginAtomIdx())
-             i2 = int(bi.GetEndAtomIdx())
-             bint = bi.GetBondType()
-             btype = "1"
-             if(bint==1 or bint == 'SINGLE'): btype = "1"
-             if(bint==2 or bint == 'DOUBLE'): btype = "2"
-             if(bint==12 or bint == 'AROMATIC'): btype = "ar"
-             if(bint==3 or bint == 'TRIPLE'):  btype = "3"
-             pMol2Block += "%6d%6d%6d %s\n"%(i+1,i1+1,i2+1,btype)
-        return pMol2Block
```

### Comparing `amolkit-1.0.2/amolkit/moltransform.py` & `amolkit-1.0.4/amolkit/moltransform.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.2/amolkit/psf.py` & `amolkit-1.0.4/amolkit/psf.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,18 +30,17 @@
    k33 = kdrude*k33
    k33 = k33 - kdrude
    k11 = k11 - kdrude - k33
    k22 = k22 - kdrude - k33
    return ([k11,k22,k33])
 
 class Psf():
-    def __init__ (self,topology): 
+    def __init__ (self): 
         """
         Constructor for Psf class
-        Using topology to assign relevant attributes.
         """
 
         self.resname = None 
         self.segname = None
         self.first_byIdx=None
         self.last_byIdx=None
         self.npsfatoms=None
@@ -77,22 +76,30 @@
         self.acceptorindices=[]
         self.cmapindices=[]
         self.lpics=[]
         self.anisotropies=[]
         self.drudebondindices=[] 
         self.drudebonds=[] 
 
-        self.topology = topology 
-
-    def genpsf(self,istart=0,resid=1,dweight=0.4,segname=None,autogenangdih=True): 
+    def genPsf(self,topology,istart=0,resid=1,dweight=0.4,segname=None,autogenangdih=True): 
         '''
-        Load the features of the residue based on topology file.
-        TODO: read the topology file separately and get all features from there.
+        Using topology to assign relevant attributes.
+        Most attributes are based on index unlike topology class which is based on atomnames
+        Arguments:
+            topology: Topology class instance for a given residue
+            istart: Start value for indexing. 
+                    This helps when building sequential residues by calling this method again and again  
+            resid: User defined resid
+            dweight: Mass assigned to drude particle.
+            segname: Segname
+            autogenangdih: Whether or not angle and dihedral are autogenerated 
         '''
 
+        self.topology = topology 
+
         atomcharges=[]
 
         resname = self.topology.resname
         segname = segname if segname else resname
         self.fftype = self.topology.fftype
         self.atomsinring = self.topology.atomsinring 
         self.groups = self.topology.groups 
@@ -112,32 +119,38 @@
                 self.atomresn_byIdx[nat]   = resname
                 self.atomresid_byIdx[nat]  = resid 
                 self.atomsegn_byIdx[nat]   = segname 
                 atomcharges.append(self.atomcharge_byIdx[nat])
 
         elif self.fftype[0:4] == "drud":
             for key,value in self.topology.atomname_byIdx.items():
-                # Rethink: nat should be related to key # Although this would work because atomname_byIdx is ordereddict
+                # Rethink: nat should be related to key 
+                # Although this would work because atomname_byIdx is ordereddict
                 nat = nat + 1 
+
                 # Only has list of drude containing atoms
                 drud = self.topology.atomdrudetype_byId.get(value)
+
                 self.atomname_byIdx[nat]   = value
                 self.atomindex_byId[value] = nat
                 self.atomserial_byIdx[nat] = nat
                 self.atomtype_byIdx[nat]   = self.topology.atomtype_byId[value] 
                 self.atomqlp_byIdx[nat]    = -1 if self.atomtype_byIdx[nat][0:2].upper() == "LP" else 0            
                 self.atomcharge_byIdx[nat] = self.topology.atomcharge_byId[value] 
                 self.atomalpha_byIdx[nat]  = self.topology.atomalpha_byId[value] if drud else 0.0 
                 self.atomthole_byIdx[nat]  = self.topology.atomthole_byId[value] if drud else 0.0
                 self.atommass_byIdx[nat]   = self.topology.atommass_byId[value] 
                 self.atomresn_byIdx[nat]   = resname
                 self.atomresid_byIdx[nat]  = resid 
                 self.atomsegn_byIdx[nat]   = segname 
                 atomcharges.append(self.atomcharge_byIdx[nat])
-
+                
+                # If drud is True implies the atom contains Drude particle.
+                # Following assigns attributes to Drude particle
+                # And adjusts atomcharge_byIdx and atommass_byIdx of parent atom.
                 if drud:
                     nat = nat + 1
                     dvalue = "D"+value 
                     self.atomname_byIdx[nat]       = dvalue
                     self.atomindex_byId[dvalue]    = nat
                     self.atomserial_byIdx[nat]     = nat
                     self.atomtype_byIdx[nat]       = drud 
@@ -161,17 +174,17 @@
         for ba,bb in self.topology.lpbonds:
             self.lpbondindices.append([self.atomindex_byId[ba],self.atomindex_byId[bb]])
 
         if self.topology.first_byId: self.first_byIdx = self.atomindex_byId[self.topology.first_byId]
         if self.topology.last_byId: self.last_byIdx = self.atomindex_byId[self.topology.last_byId]
 
         if autogenangdih:
-            self.bondgraph = genic.GetBondAngleDihedral.GetBondDict(self.atomname_byIdx,self.bondindices)["aNoLPBond"]
-            _,self.angleindices = genic.GetBondAngleDihedral.GetAngles(self.atomindex_byId,self.bondgraph)
-            _,self.dihedralindices = genic.GetBondAngleDihedral.GetDihedrals(self.atomindex_byId,self.bondgraph)
+            self.bondgraph = genic.ICs.getBondDict(self.atomname_byIdx,self.bondindices)["aNoLPBond"]
+            _,self.angleindices = genic.ICs.getAngles(self.atomindex_byId,self.bondgraph)
+            _,self.dihedralindices = genic.ICs.getDihedrals(self.atomindex_byId,self.bondgraph)
 
             #Checks if there are any atoms not bonded to anything or any bonds with no defined atoms
             for atom in list(self.bondgraph.keys()):
                 if atom not in self.atomindex_byId.keys():
                      raise RuntimeError(('A bond is defined for atom %s but it is not in atom list of %s.' %(atom,resname)))
 
         else:
@@ -189,25 +202,25 @@
 
         for aa,ab in self.topology.acceptors:
             self.acceptorindices.append([self.atomindex_byId[aa],self.atomindex_byId[ab]])
 
         for ca,cb,cc,cd,ce,cf,cg,ch in self.topology.cmaps:
             self.cmapindices.append([self.atomindex_byId[ca],self.atomindex_byId[cb],self.atomindex_byId[cc],self.atomindex_byId[cd],self.atomindex_byId[ce],self.atomindex_byId[cf],self.atomindex_byId[cg],self.atomindex_byId[ch]])
 
-        #print(self.topology.lpics)
         for i in range(len(self.topology.lpics)):
             hlist = list(map(lambda x:self.atomindex_byId[x],self.topology.lpics[i][1])) 
             self.lpics.append([self.topology.lpics[i][0],hlist,self.topology.lpics[i][2]])   
 
         for i in range(len(self.topology.anisotropies)):
             hlist = list(map(lambda x:self.atomindex_byId[x],self.topology.anisotropies[i][0]))
             vlist = anisotropy(*self.topology.anisotropies[i][1])
             self.anisotropies.append([hlist,vlist])
 
         self.npsfatoms=len(self.atomindex_byId.keys())
+
         # Determine group types
         for i in range(len(self.groups)):
             if i+1 <= len(self.groups): 
                 gc = abs(sum(atomcharges[self.groups[i][0]:self.npsfatoms]))
                 natgrp = self.npsfatoms - self.groups[i][0]
             else:
                 gc = abs(sum(atomcharges[self.groups[i][0]:self.groups[i+1][0]]))
@@ -347,42 +360,112 @@
     fout.write('{:>10} !NCRTERM: cross-terms\n'.format(nallcmaps))
     psfFormat(fout,"cmap",psf.cmapindices) 
 
     fout.close()
     prntscr = " ".join((str(fileout),"created"))
     print(prntscr) 
 
-def buildPsf(resnames,resncount=None,resitopfiles=None,istart=0,resid=1,dweight=0.4,segname=None,autogenangdih=True,prevpsf=None): 
+def buildPsf(resnames,nresnames=None,resitopfiles=None,istart=0,resid=1,dweight=0.4,segname=None,autogenangdih=True,prevpsfs=None): 
     if not resitopfiles:
         raise FileNotFoundError("No resi toppar file is provided.")
 
-    if isinstance(resnames,str): resname=[resnames]
-    if isinstance(resitopfiles,str): resitopfiles=[resitopfiles]
-    
-    if not resncount: resncount=[1]*len(resnames)
-    psf=prevpsf
-    first_byIdx=[]
-    last_byIdx=[]
+    #if isinstance(resitopfiles,str): resitopfiles=[resitopfiles]
+
+    if isinstance(resnames,str): 
+        if not nresnames: 
+            resnames=[resnames]
+        elif isinstance(nresnames,list):
+            resnames=[resnames]*int(nresnames[0])
+        elif isinstance(nresnames,str) or isinstance(nresnames,int):
+            resnames=[resnames]*int(nresnames)
+        else:
+            raise ValueError("If you provide rescount list its length should be same as resname.") 
+
+    elif isinstance(resnames,list):
+        if not nresnames: 
+            pass 
+        elif not isinstance(nresnames,list): 
+            raise ValueError("If you provide resname as list either donot provide rescount \
+                    or if you do, the length of rescount list should be same as resname.") 
+        elif isinstance(nresnames,list) and len(nresnames) != len(resnames):
+            raise ValueError("If you provide rescount list its length should be same as resname.") 
+        elif isinstance(nresnames,list) and len(nresnames) == len(resnames):
+            tmpresn = []
+            for i,resn in enumerate(resnames):
+                tmpresn.append([resn]*int(nresnames[i]))
+            resnames = [item for resn in tmpresn for item in resn]
+
+    if not segname: segname = [resn for resn in resnames]
+    if isinstance(segname,str): segname = [segn for i in range(len(resnames))]
+    if not isinstance(segname,list) or len(segname) != len(resnames):
+        raise ValueError("Length of segname list should be same as resname. \
+                If you have single segname, provide it as string. \
+                It will be changed to list internally")
+
     restop=[]
-    if not psf:
-        t = Topology()
-        for i,resn in enumerate(resnames):
-            if i == 0: 
-                istart = 0 
-                resnwttopo = [resn]
-            else: 
-                if resn in resnwttopo:
-                    t=resnwttopo.index(resn)
-                else:
-                    t.loadTopology(resn,resitopfiles)
-                    restop.append(t)
-                    resnwttopo.append(resn)
-            p = Psf(t)
-            p.genpsf(istart,resid,dweight,segname,autogenangdih)
-            if p.first_byIdx: first_byIdx.append(p.first_byIdx)
-            if p.last_byIdx: last_byIdx.append(p.last_byIdx)
+    if prevpsfs:
+       istart = prevpsfs[i-1].npsfatoms
 
-            istart = istart + p.npsfatoms
-            resid = resid + 1
+    t = Topology()
+    for i,resn in enumerate(resnames):
+        if i == 0: 
+            t.loadCharmmTopology(resn,resitopfiles)
+            p = Psf()
+            p.genPsf(t,istart,resid,dweight,segname[i],autogenangdih)
+            #save
+            resns = [resn]
+            topos = [t]
+            psfs = [p]
+        else: 
+            if resn in resns:
+                ind = resns.index(resn)
+                t = topos[ind]
+                istart = istart+psfs[i-1].npsfatoms
+                resid = resid + 1
+                p = Psf()
+                p.genPsf(t,istart,resid,dweight,segname[i],autogenangdih)
+                psfs.append(p)
+            else:
+                t.loadCharmmTopology(resn,resitopfiles)
+                istart = istart+psfs[i-1].npsfatoms
+                resid = resid + 1
+                p = Psf()
+                p.genPsf(t,istart,resid,dweight,segname[i],autogenangdih)
+                resns.append(resn)
+                topos.append(t)
+                psfs.append(p)
+
+    return psfs
+
+def joinPsf(psfs):
+    combinedpsf=Psf()
+
+    combinedpsf.fftype = psfs[0].fftype
+    combinedpsf.npsfatoms  = 0 
+    #combinedpsf.npsfatoms = sum([ps.npsfatoms for ps in psfs])
+    for ps in psfs:    
+        combinedpsf.npsfatoms        = combinedpsf.npsfatoms        + ps.npsfatoms 
+        combinedpsf.bondindices      = combinedpsf.bondindices      + ps.bondindices 
+        combinedpsf.drudebondindices = combinedpsf.drudebondindices + ps.drudebondindices 
+        combinedpsf.angleindices     = combinedpsf.angleindices     + ps.angleindices 
+        combinedpsf.dihedralindices  = combinedpsf.dihedralindices  + ps.dihedralindices 
+        combinedpsf.improperindices  = combinedpsf.improperindices  + ps.improperindices 
+        combinedpsf.donorindices     = combinedpsf.donorindices     + ps.donorindices 
+        combinedpsf.acceptorindices  = combinedpsf.acceptorindices  + ps.acceptorindices 
+        combinedpsf.groups           = combinedpsf.groups           + ps.groups 
+        combinedpsf.lpics            = combinedpsf.lpics            + ps.lpics 
+        combinedpsf.anisotropies     = combinedpsf.anisotropies     + ps.anisotropies 
+        combinedpsf.cmapindices      = combinedpsf.cmapindices      + ps.cmapindices 
+
+        combinedpsf.atomserial_byIdx.update(ps.atomserial_byIdx)
+        combinedpsf.atomresn_byIdx.update(ps.atomresn_byIdx)
+        combinedpsf.atomresid_byIdx.update(ps.atomresid_byIdx)
+        combinedpsf.atomsegn_byIdx.update(ps.atomsegn_byIdx)
+        combinedpsf.atomname_byIdx.update(ps.atomname_byIdx)
+        combinedpsf.atomtype_byIdx.update(ps.atomtype_byIdx)
+        combinedpsf.atomcharge_byIdx.update(ps.atomcharge_byIdx)
+        combinedpsf.atommass_byIdx.update(ps.atommass_byIdx)
+        combinedpsf.atomqlp_byIdx.update(ps.atomqlp_byIdx)
+        combinedpsf.atomalpha_byIdx.update(ps.atomalpha_byIdx)
+        combinedpsf.atomthole_byIdx.update(ps.atomthole_byIdx)
 
-            #if first and last:
-            #    self.bondindices.append(istart,self.atomindex_byId[])
+    return combinedpsf
```

### Comparing `amolkit-1.0.2/amolkit/stringmanip.py` & `amolkit-1.0.4/amolkit/stringmanip.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,13 +84,13 @@
             newkey=key
         for v in value:
             i=i+1
             newname[v]=newkey+str(i)
                    
     return newname       
 
-def updateAtomnames(iatomnames):
+def updateAtomNames(iatomnames):
     update_names=renumber(list(iatomnames.values()))
     for i,nam in enumerate(update_names):
         iatomnames[i+1]=nam
     return iatomnames
```

### Comparing `amolkit-1.0.2/amolkit/topology.py` & `amolkit-1.0.4/amolkit/topology.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,329 +2,366 @@
 import math
 import argparse
 from collections import OrderedDict
 from amolkit import genic
 from amolkit import getEleInfo as gei 
 from amolkit.stringmanip import getPenaltyfromString
 
-def readCharmmTopology(resname,resitopfile,bio=True):
-    '''
-    Load the features of the residue based on topology file.
-
-    Note::
-    field[1] is atomname
-    field[2] is atomtype
-    if bio is True then utilize gei.atomicmass_by_anyatomname upon atomtype
-    to get atomicmass or symbol. This way I am not limited to predefined atomtypes in EleInfo.
-
-    atommass_byId[field[1]] = gei.atomicmass_by_anyatomname(field[2],bio)
-    atomele_byId[field[1]] = gei.atomsymbol_by_anyatomname(field[2],bio)
-
-    But if it false, then I should ideally get atomicmass by atomtype
-    and in case an atomtype is missing, I should allow user to supply new atomtype and its correspondence.
-
-    # Give some thought if bio is False. In that case, atomtype = MAG will not be converted to Mg
-    # Thus it would not find Mg
-    '''
-
-    topology = {}
-    topology["resname"]            = resname
-    topology["fftype"]             = 'additive' 
-    topology["rescharge"]          = None 
-    topology['ntopatoms']          = None
-    topology['natoms']             = None
-    topology['first_byId']         = None
-    topology['last_byId']          = None
-    topology['atomindex_byId']     = OrderedDict() 
-    topology['atomname_byIdx']     = OrderedDict()
-    topology['atomtype_byId']      = OrderedDict()
-    topology['atomcharge_byId']    = OrderedDict()
-    topology['atompenalty_byId']   = OrderedDict()
-    topology['atommass_byId']      = OrderedDict()
-    topology['atomele_byId']       = OrderedDict()
-    topology['atomalpha_byId']     = OrderedDict()
-    topology['atomthole_byId']     = OrderedDict()
-    topology['atomdrudetype_byId'] = OrderedDict()
-    topology['atomsinring']        = OrderedDict()
-    topology['groups']             = []  
-    topology['atomnames']          = []    
-    topology['bonds']              = []
-    topology['lpbonds']            = []
-    topology['angles']             = []
-    topology['dihedrals']          = []
-    topology['impropers']          = []
-    topology['lpics']              = []
-    topology['anisotropies']       = []
-    topology['donors']             = []
-    topology['acceptors']          = []
-    topology['cmaps']              = []
-    topology['atomcharges']        = []
-
-    try:
-        filein=open(resitopfile, "r")
-    except IOError:
-        raise IOError('Could not access the ' + resitopfile + ' topology file')
-
-    found=False
-    ring = 0
-    nat = 0
-
-    for nl,line in enumerate(filein):
-        #Strip the line, remove the comment lines, and split using whitespace
-        field = line.strip().split("!")[0].split()
-        
-        fieldup = list(map(lambda x:x.upper(),field))
-
-        comment = "!".join(line.strip().split("!")[1:]) 
-
-        if len(fieldup) >= 1:
-            ftype = fieldup[0][0:4]
-            if found and ftype == "END": break
-            if ftype in ["RESI","PRES"] and fieldup[1] !=  topology['resname'].upper():
-                if found:
-                    break
-                else:
-                   found = False
-            elif ftype in ["RESI","PRES"] and fieldup[1] ==  topology['resname'].upper():
-                found = True
-                try:
-                    topology["rescharge"]=round(float(field[2]),3)
-                except (ValueError,IndexError):
-                    raise ValueError('Beware:: Error in detecting residue charge of '+topology['resname']+'.')
-
-        if found and len(fieldup) > 0:
-            ftype = fieldup[0][0:4]
-            if ftype not in ["RING","GROU","ATOM","BOND","DOUB","TRIP","ANGL","DIHE","IMPR","DONO","ACCE","CMAP","LONE","ANIS"]: continue
-            if ftype == "RING":
-                ring=ring+1
-                #topology['atomsinring'][ring]=field[1:]
-                topology['atomsinring'][ring]=fieldup[1:]
-                continue
-            elif ftype == "GROU":
-                topology['groups'].append([nat,0,0])
-                continue
-            elif ftype == "ATOM" and len(fieldup) > 3: 
-                nat = nat + 1
-                topology['atomindex_byId'][fieldup[1]] = nat
-                topology['atomname_byIdx'][nat] = fieldup[1]    # Atomname stored as in str
-                topology['atomtype_byId'][fieldup[1]] = fieldup[2]  # Atomtype capitalized before storing
-                topology['atomcharge_byId'][fieldup[1]] = float(field[3])
-                # Using atomicmass_by_anyatomname, but supplying atomtype
-                # Because atomicmass_by_anyatomtype does a fixed conversion
-                topology['atommass_byId'][fieldup[1]] = gei.atomicmass_by_anyatomname(field[2],bio)
-                topology['atomele_byId'][fieldup[1]] = gei.atomsymbol_by_anyatomname(field[2],bio)
-                topology['atomcharges'].append(float(field[3]))
-                topology['atompenalty_byId'][fieldup[1]],_ = getPenaltyfromString(comment)
-
-                if topology['atomnames'] and fieldup[1] in topology['atomnames']:
-                    raise ValueError("Topology contains repeated atomname %s. Unable to load."%(field[1]))
-                else:
-                    topology['atomnames'].append(fieldup[1]) 
-                
-                if any(list(map(lambda x:x in fieldup, ["ALPHA","THOLE","TYPE"]))): 
-                    topology['atomalpha_byId'][fieldup[1]]=None
-                    topology['atomthole_byId'][fieldup[1]]=None
-                    topology['atomdrudetype_byId'][fieldup[1]]='DRUD'
-                    topology["fftype"] = "drude"
-
-                if "ALPHA" in fieldup:
-                    topology['atomalpha_byId'][fieldup[1]]=float(field[fieldup.index("ALPHA")+1])
-                if "THOLE" in fieldup:
-                    topology['atomthole_byId'][fieldup[1]]=float(field[fieldup.index("THOLE")+1])
-                if "TYPE" in fieldup:
-                    topology['atomdrudetype_byId'][fieldup[1]]=fieldup[fieldup.index("TYPE")+1]
-
-                continue
-
-            #Bond list dictionary of each atom is populated.
-            elif ftype in ["BOND","DOUB","TRIP"] and (len(fieldup)-1) % 2 == 0:
-                for i in range(1,len(fieldup),2):
-                    ba = fieldup[i].strip("+-")
-                    bb = fieldup[i+1].strip("+-")
-                    topology['bonds'].append([ba,bb])
-
-                    if ba.startswith('+'): topology['first_byId'] = ba
-                    if bb.startswith('+'): topology['first_byId'] = bb
-                    if ba.startswith('-'): topology['last_byId'] = ba
-                    if bb.startswith('-'): topology['last_byId'] = bb
-
-                    if 'LP' in [ba[0:2], bb[0:2]]:
-                        topology['lpbonds'].append([ba,bb])
-
-            elif ftype in ["BOND","DOUB","TRIP"] and (len(fieldup)-1) % 2 != 0:
-                 raise ValueError('Topology file BOND line has the wrong format. It should be multiples of two! BOND At1 At2 At2 At3 At1 At3 etc.')
-
-            #Angle list dictionary.
-            elif ftype == "ANGL" and (len(fieldup)-1) % 3 == 0:
-                for i in range(1,len(fieldup),3):
-                    aa = fieldup[i].strip("+-")
-                    ab = fieldup[i+1].strip("+-")
-                    ac = fieldup[i+2].strip("+-")
-                    topology['angles'].append([aa,ab,ac])
-                continue
-            elif ftype == "ANGL" and (len(fieldup)-1) % 3 != 0:
-                raise ValueError('Topology file ANGLE line has the wrong format. Ignored reading.')
-                continue
-
-            #Dihedral list dictionary.
-            elif ftype == "DIHE" and (len(fieldup)-1) % 4 == 0:
-                for i in range(1,len(fieldup),4):
-                    da = fieldup[i].strip("+-")
-                    db = fieldup[i+1].strip("+-")
-                    dc = fieldup[i+2].strip("+-")
-                    dd = fieldup[i+3].strip("+-")
-                    topology['dihedrals'].append([da,db,dc,dd])
-
-            elif ftype == "DIHE" and (len(fieldup)-1) % 4 != 0:
-                raise ValueError('Topology file DIHEDRAL line has the wrong format. Ignored reading.')
-
-            #Improper list dictionary.
-            elif ftype == "IMPR" and (len(fieldup)-1) % 4 == 0:
-                for i in range(1,len(fieldup),4):
-                    ima = fieldup[i].strip("+-")
-                    imb = fieldup[i+1].strip("+-")
-                    imc = fieldup[i+2].strip("+-")
-                    imd = fieldup[i+3].strip("+-")
-                    topology['impropers'].append([ima,imb,imc,imd])
-            elif ftype == "IMPR" and (len(fieldup)-1) % 4 != 0:
-                raise ValueError('Topology file IMPROPER line has the wrong format. Ignored reading.')
-
-            #Donor list dictionary.
-            elif ftype == "DONO" and (len(fieldup)-1) % 2 == 0:
-                for i in range(1,len(fieldup),2):
-                    topology['donors'].append([fieldup[i+1],fieldup[i]])
-
-            elif ftype == "DONO" and (len(fieldup)-1) % 2 != 0:
-                raise ValueError('Topology file DONOR line has the wrong format. Ignored reading.')
-
-            #Acceptor list dictionary.
-            elif ftype == "ACCE" and (len(fieldup)-1) % 2 == 0:
-                for i in range(1,len(fieldup),2):
-                    topology['acceptors'].append([fieldup[i],fieldup[i+1]])
-
-            elif ftype == "ACCE" and (len(fieldup)-1) == 1:
-                topology['acceptors'].append([fieldup[-1],""])
-
-            elif ftype == "ACCE" and (len(fieldup)-1) != 1 or ftype == "ACCE" and (len(fieldup)-1) % 2 != 0:
-                raise ValueError('Topology file ACCEPTOR line has the wrong format. Ignored reading.')
-
-            elif ftype == "CMAP" and (len(fieldup)-1) % 8 == 0:
-                for i in range(1,len(fieldup),8):
-                    ca = fieldup[i].strip("+-")
-                    cb = fieldup[i+1].strip("+-")
-                    cc = fieldup[i+2].strip("+-")
-                    cd = fieldup[i+3].strip("+-")
-                    ce = fieldup[i+4].strip("+-")
-                    cf = fieldup[i+5].strip("+-")
-                    cg = fieldup[i+6].strip("+-")
-                    ch = fieldup[i+7].strip("+-")
-                    topology['cmaps'].append([ca,cb,cc,cd,ce,cf,cg,ch])
-
-            elif ftype == "CMAP" and (len(fieldup)-1) % 8 != 0:
-                raise ValueError('Topology file CMAP line has the wrong format. Ignored reading.')
-            
-            # topology['atomindex_byId'] will change later according to inclusion of 
-            # Lone pair list dictionary
-            elif ftype == "LONE": 
-                if fieldup[1][0:4] in ["RELA","BISE"]:
-                    try:
-                        hlist = fieldup[2:6]
-                        vlist = []
-                        for ilp in range(len(fieldup)): 
-                            if fieldup[ilp][0:4] == "DIST" and fieldup[1][0:4] == "RELA":
-                                vlist.append(float(fieldup[ilp+1]))
-                            if fieldup[ilp][0:4] == "DIST" and fieldup[1][0:4] == "BISE":
-                                vlist.append(-(float(fieldup[ilp+1])))
-                            if fieldup[ilp][0:4] == "ANGL":
-                                vlist.append(float(fieldup[ilp+1]))
-                            if fieldup[ilp][0:4] == "DIHE":
-                                vlist.append(float(fieldup[ilp+1]))
-                        topology['lpics'].append([fieldup[1][0:4],hlist,vlist])
-                    except (IndexError, ValueError,KeyError):    
-                        raise ValueError('Topology file LONEPAIR line has the wrong format. Ignored reading.')
-                elif fieldup[1][0:4] == "COLI": 
-                    try:
-                        hlist =fieldup[2:5]
-                        vlist = []
-                        for ilp in range(len(fieldup)): 
-                            if fieldup[ilp][0:4] == "DIST":
-                                vlist.append(float(fieldup[ilp+1]))
-                            if fieldup[ilp][0:4] == "SCAL":
-                                vlist.append(float(fieldup[ilp+1]))
-                        vlist.append(float(0.0))
-                        topology['lpics'].append([fieldup[1][0:4],hlist,vlist])
-                    except (IndexError, ValueError):    
-                        raise ValueError('Topology file LONEPAIR line has the wrong format. Ignored reading.')
-                elif fieldup[1][0:4] == "FIXE":
-                    try:
-                        topology['lpics'].append([[fieldup[1][0:4]],[],list(map(float,fieldup[2:5]))]) 
-                    except (IndexError, ValueError):    
-                        raise ValueError('Topology file LONEPAIR line has the wrong format. Ignored reading.')
-                elif fieldup[1][0:4] == "CENT":
-                    try:
-                        topology['lpics'].append([fieldup[1][0:4],fieldup[2:],[]])
-                    except (IndexError, ValueError):    
-                        raise ValueError('Topology file LONEPAIR line has the wrong format. Ignored reading.')
-
-            # Anisotropy list dictionary
-            elif ftype == "ANIS": 
-                try:
-                    hlist = field[1:5]
-                    for ilp in range(len(fieldup)): 
-                        if fieldup[ilp][0:3] == "A11":
-                            a11 =  float(fieldup[ilp+1])
-                        if fieldup[ilp][0:3] == "A22":
-                            a22 =  float(fieldup[ilp+1])
-                    if a11 == 0.0 or a22 == 0.0:
-                       logging.error('0.0 is invalid force constant. Ignoring this anisotropy line.')
-                       continue
-                    vlist = [a11,a22] 
-                    topology['anisotropies'].append([hlist,vlist])
-                except (IndexError, ValueError,KeyError):    
-                    raise ValueError('Topology file Anisotropy line has the wrong format. Ignored reading.')
-    #### Reading done ###
-
-    if found:
-        onlyatomsnlps = [at for at in topology['atomindex_byId'].keys() if at[0].upper() != "D"]
-        onlyatoms     = [at for at in onlyatomsnlps if at[0:2].upper() != "LP" ]
-        topology['ntopatoms']     = len(topology['atomindex_byId'].keys())
-        topology['natoms']        = len(onlyatoms)
-
-        #Check for residue total charge
-        if abs( sum(topology['atomcharges']) - topology['rescharge'] ) > 0.00001:
-            print('Warning: Your total charge does not match the sum of partial charges.')
-
-    elif not found:
-        print ('Could not find the residue name: '+topology['resname']+' in the provided topology file.')
-
-    return topology
-
-
 class Topology():
     def __init__(self): 
         """
         Constructor for the Topology class.
         """
+    
+    @staticmethod
+    def readCharmmTopology(resname,resitopfile,bio=True):
+        '''
+        Load the features of the residue based on topology file.
+    
+        Note::
+        field[1] is atomname
+        field[2] is atomtype
+        if bio is True then utilize gei.atomicmass_by_anyatomname upon atomtype
+        to get atomicmass or symbol. This way I am not limited to predefined atomtypes in EleInfo.
+    
+        atommass_byId[field[1]] = gei.atomicmass_by_anyatomname(field[2],bio)
+        atomele_byId[field[1]] = gei.atomsymbol_by_anyatomname(field[2],bio)
+    
+        But if it false, then I should ideally get atomicmass by atomtype
+        and in case an atomtype is missing, I should allow user to supply new atomtype and its correspondence.
+    
+        # Give some thought if bio is False. In that case, atomtype = MAG will not be converted to Mg
+        # Thus it would not find Mg
+        '''
+    
+        topology = {}
+        topology["resname"]            = resname
+        topology["fftype"]             = 'additive' 
+        topology["rescharge"]          = None 
+        topology['ntopatoms']          = None
+        topology['natoms']             = None
+        topology['first_byId']         = None
+        topology['last_byId']          = None
+        topology['atomindex_byId']     = OrderedDict() 
+        topology['atomname_byIdx']     = OrderedDict()
+        topology['atomtype_byId']      = OrderedDict()
+        topology['atomcharge_byId']    = OrderedDict()
+        topology['atompenalty_byId']   = OrderedDict()
+        topology['atommass_byId']      = OrderedDict()
+        topology['atomele_byId']       = OrderedDict()
+        topology['atomalpha_byId']     = OrderedDict()
+        topology['atomthole_byId']     = OrderedDict()
+        topology['atomdrudetype_byId'] = OrderedDict()
+        topology['atomsinring']        = OrderedDict()
+        topology['groups']             = []  
+        topology['atomnames']          = []    
+        topology['bonds']              = []
+        topology['lpbonds']            = []
+        topology['angles']             = []
+        topology['dihedrals']          = []
+        topology['impropers']          = []
+        topology['lpics']              = []
+        topology['anisotropies']       = []
+        topology['donors']             = []
+        topology['acceptors']          = []
+        topology['cmaps']              = []
+        topology['atomcharges']        = []
+    
+        try:
+            filein=open(resitopfile, "r")
+        except IOError:
+            raise IOError('Could not access the ' + resitopfile + ' topology file')
+    
+        found=False
+        ring = 0
+        nat = 0
+    
+        for nl,line in enumerate(filein):
+            #Strip the line, remove the comment lines, and split using whitespace
+            field = line.strip().split("!")[0].split()
+            
+            fieldup = list(map(lambda x:x.upper(),field))
+    
+            comment = "!".join(line.strip().split("!")[1:]) 
+    
+            if len(fieldup) >= 1:
+                ftype = fieldup[0][0:4]
+                if found and ftype == "END": break
+                if ftype in ["RESI","PRES"] and fieldup[1] !=  topology['resname'].upper():
+                    if found:
+                        break
+                    else:
+                       found = False
+                elif ftype in ["RESI","PRES"] and fieldup[1] ==  topology['resname'].upper():
+                    found = True
+                    try:
+                        topology["rescharge"]=round(float(field[2]),3)
+                    except (ValueError,IndexError):
+                        raise ValueError('Beware:: Error in detecting residue charge of '+topology['resname']+'.')
+    
+            if found and len(fieldup) > 0:
+                ftype = fieldup[0][0:4]
+                if ftype not in ["RING","GROU","ATOM","BOND","DOUB","TRIP","ANGL","DIHE","IMPR","DONO","ACCE","CMAP","LONE","ANIS"]: continue
+                if ftype == "RING":
+                    ring=ring+1
+                    #topology['atomsinring'][ring]=field[1:]
+                    topology['atomsinring'][ring]=fieldup[1:]
+                    continue
+                elif ftype == "GROU":
+                    topology['groups'].append([nat,0,0])
+                    continue
+                elif ftype == "ATOM" and len(fieldup) > 3: 
+                    nat = nat + 1
+                    topology['atomindex_byId'][fieldup[1]] = nat
+                    topology['atomname_byIdx'][nat] = fieldup[1]    # Atomname stored as in str
+                    topology['atomtype_byId'][fieldup[1]] = fieldup[2]  # Atomtype capitalized before storing
+                    topology['atomcharge_byId'][fieldup[1]] = float(field[3])
+                    # Using atomicmass_by_anyatomname, but supplying atomtype
+                    # Because atomicmass_by_anyatomtype does a fixed conversion
+                    topology['atommass_byId'][fieldup[1]] = gei.atomicmass_by_anyatomname(field[2],bio)
+                    topology['atomele_byId'][fieldup[1]] = gei.atomsymbol_by_anyatomname(field[2],bio)
+                    topology['atomcharges'].append(float(field[3]))
+                    topology['atompenalty_byId'][fieldup[1]],_ = getPenaltyfromString(comment)
+    
+                    if topology['atomnames'] and fieldup[1] in topology['atomnames']:
+                        raise ValueError("Topology contains repeated atomname %s. Unable to load."%(field[1]))
+                    else:
+                        topology['atomnames'].append(fieldup[1]) 
+                    
+                    if any(list(map(lambda x:x in fieldup, ["ALPHA","THOLE","TYPE"]))): 
+                        topology['atomalpha_byId'][fieldup[1]]=None
+                        topology['atomthole_byId'][fieldup[1]]=None
+                        topology['atomdrudetype_byId'][fieldup[1]]='DRUD'
+                        topology["fftype"] = "drude"
+    
+                    if "ALPHA" in fieldup:
+                        topology['atomalpha_byId'][fieldup[1]]=float(field[fieldup.index("ALPHA")+1])
+                    if "THOLE" in fieldup:
+                        topology['atomthole_byId'][fieldup[1]]=float(field[fieldup.index("THOLE")+1])
+                    if "TYPE" in fieldup:
+                        topology['atomdrudetype_byId'][fieldup[1]]=fieldup[fieldup.index("TYPE")+1]
+    
+                    continue
+    
+                #Bond list dictionary of each atom is populated.
+                elif ftype in ["BOND","DOUB","TRIP"] and (len(fieldup)-1) % 2 == 0:
+                    for i in range(1,len(fieldup),2):
+                        ba = fieldup[i].strip("+-")
+                        bb = fieldup[i+1].strip("+-")
+                        topology['bonds'].append([ba,bb])
+    
+                        if ba.startswith('+'): topology['first_byId'] = ba
+                        if bb.startswith('+'): topology['first_byId'] = bb
+                        if ba.startswith('-'): topology['last_byId'] = ba
+                        if bb.startswith('-'): topology['last_byId'] = bb
+    
+                        if 'LP' in [ba[0:2], bb[0:2]]:
+                            topology['lpbonds'].append([ba,bb])
+    
+                elif ftype in ["BOND","DOUB","TRIP"] and (len(fieldup)-1) % 2 != 0:
+                     raise ValueError('Topology file BOND line has the wrong format. It should be multiples of two! BOND At1 At2 At2 At3 At1 At3 etc.')
+    
+                #Angle list dictionary.
+                elif ftype == "ANGL" and (len(fieldup)-1) % 3 == 0:
+                    for i in range(1,len(fieldup),3):
+                        aa = fieldup[i].strip("+-")
+                        ab = fieldup[i+1].strip("+-")
+                        ac = fieldup[i+2].strip("+-")
+                        topology['angles'].append([aa,ab,ac])
+                    continue
+                elif ftype == "ANGL" and (len(fieldup)-1) % 3 != 0:
+                    raise ValueError('Topology file ANGLE line has the wrong format. Ignored reading.')
+                    continue
+    
+                #Dihedral list dictionary.
+                elif ftype == "DIHE" and (len(fieldup)-1) % 4 == 0:
+                    for i in range(1,len(fieldup),4):
+                        da = fieldup[i].strip("+-")
+                        db = fieldup[i+1].strip("+-")
+                        dc = fieldup[i+2].strip("+-")
+                        dd = fieldup[i+3].strip("+-")
+                        topology['dihedrals'].append([da,db,dc,dd])
+    
+                elif ftype == "DIHE" and (len(fieldup)-1) % 4 != 0:
+                    raise ValueError('Topology file DIHEDRAL line has the wrong format. Ignored reading.')
+    
+                #Improper list dictionary.
+                elif ftype == "IMPR" and (len(fieldup)-1) % 4 == 0:
+                    for i in range(1,len(fieldup),4):
+                        ima = fieldup[i].strip("+-")
+                        imb = fieldup[i+1].strip("+-")
+                        imc = fieldup[i+2].strip("+-")
+                        imd = fieldup[i+3].strip("+-")
+                        topology['impropers'].append([ima,imb,imc,imd])
+                elif ftype == "IMPR" and (len(fieldup)-1) % 4 != 0:
+                    raise ValueError('Topology file IMPROPER line has the wrong format. Ignored reading.')
+    
+                #Donor list dictionary.
+                elif ftype == "DONO" and (len(fieldup)-1) % 2 == 0:
+                    for i in range(1,len(fieldup),2):
+                        topology['donors'].append([fieldup[i+1],fieldup[i]])
+    
+                elif ftype == "DONO" and (len(fieldup)-1) % 2 != 0:
+                    raise ValueError('Topology file DONOR line has the wrong format. Ignored reading.')
+    
+                #Acceptor list dictionary.
+                elif ftype == "ACCE" and (len(fieldup)-1) % 2 == 0:
+                    for i in range(1,len(fieldup),2):
+                        topology['acceptors'].append([fieldup[i],fieldup[i+1]])
+    
+                elif ftype == "ACCE" and (len(fieldup)-1) == 1:
+                    topology['acceptors'].append([fieldup[-1],""])
+    
+                elif ftype == "ACCE" and (len(fieldup)-1) != 1 or ftype == "ACCE" and (len(fieldup)-1) % 2 != 0:
+                    raise ValueError('Topology file ACCEPTOR line has the wrong format. Ignored reading.')
+    
+                elif ftype == "CMAP" and (len(fieldup)-1) % 8 == 0:
+                    for i in range(1,len(fieldup),8):
+                        ca = fieldup[i].strip("+-")
+                        cb = fieldup[i+1].strip("+-")
+                        cc = fieldup[i+2].strip("+-")
+                        cd = fieldup[i+3].strip("+-")
+                        ce = fieldup[i+4].strip("+-")
+                        cf = fieldup[i+5].strip("+-")
+                        cg = fieldup[i+6].strip("+-")
+                        ch = fieldup[i+7].strip("+-")
+                        topology['cmaps'].append([ca,cb,cc,cd,ce,cf,cg,ch])
+    
+                elif ftype == "CMAP" and (len(fieldup)-1) % 8 != 0:
+                    raise ValueError('Topology file CMAP line has the wrong format. Ignored reading.')
+                
+                # topology['atomindex_byId'] will change later according to inclusion of 
+                # Lone pair list dictionary
+                elif ftype == "LONE": 
+                    if fieldup[1][0:4] in ["RELA","BISE"]:
+                        try:
+                            hlist = fieldup[2:6]
+                            vlist = []
+                            for ilp in range(len(fieldup)): 
+                                if fieldup[ilp][0:4] == "DIST" and fieldup[1][0:4] == "RELA":
+                                    vlist.append(float(fieldup[ilp+1]))
+                                if fieldup[ilp][0:4] == "DIST" and fieldup[1][0:4] == "BISE":
+                                    vlist.append(-(float(fieldup[ilp+1])))
+                                if fieldup[ilp][0:4] == "ANGL":
+                                    vlist.append(float(fieldup[ilp+1]))
+                                if fieldup[ilp][0:4] == "DIHE":
+                                    vlist.append(float(fieldup[ilp+1]))
+                            topology['lpics'].append([fieldup[1][0:4],hlist,vlist])
+                        except (IndexError, ValueError,KeyError):    
+                            raise ValueError('Topology file LONEPAIR line has the wrong format. Ignored reading.')
+                    elif fieldup[1][0:4] == "COLI": 
+                        try:
+                            hlist =fieldup[2:5]
+                            vlist = []
+                            for ilp in range(len(fieldup)): 
+                                if fieldup[ilp][0:4] == "DIST":
+                                    vlist.append(float(fieldup[ilp+1]))
+                                if fieldup[ilp][0:4] == "SCAL":
+                                    vlist.append(float(fieldup[ilp+1]))
+                            vlist.append(float(0.0))
+                            topology['lpics'].append([fieldup[1][0:4],hlist,vlist])
+                        except (IndexError, ValueError):    
+                            raise ValueError('Topology file LONEPAIR line has the wrong format. Ignored reading.')
+                    elif fieldup[1][0:4] == "FIXE":
+                        try:
+                            topology['lpics'].append([[fieldup[1][0:4]],[],list(map(float,fieldup[2:5]))]) 
+                        except (IndexError, ValueError):    
+                            raise ValueError('Topology file LONEPAIR line has the wrong format. Ignored reading.')
+                    elif fieldup[1][0:4] == "CENT":
+                        try:
+                            topology['lpics'].append([fieldup[1][0:4],fieldup[2:],[]])
+                        except (IndexError, ValueError):    
+                            raise ValueError('Topology file LONEPAIR line has the wrong format. Ignored reading.')
+    
+                # Anisotropy list dictionary
+                elif ftype == "ANIS": 
+                    try:
+                        hlist = field[1:5]
+                        for ilp in range(len(fieldup)): 
+                            if fieldup[ilp][0:3] == "A11":
+                                a11 =  float(fieldup[ilp+1])
+                            if fieldup[ilp][0:3] == "A22":
+                                a22 =  float(fieldup[ilp+1])
+                        if a11 == 0.0 or a22 == 0.0:
+                            raise ValueError('0.0 is invalid force constant. Correct the anisotropy line.')
+                        vlist = [a11,a22] 
+                        topology['anisotropies'].append([hlist,vlist])
+                    except (IndexError, ValueError,KeyError):    
+                        raise ValueError('Topology file Anisotropy line has the wrong format. Ignored reading.')
+        #### Reading done ###
+    
+        if found:
+            onlyatomsnlps = [at for at in topology['atomindex_byId'].keys() if at[0].upper() != "D"]
+            onlyatoms     = [at for at in onlyatomsnlps if at[0:2].upper() != "LP" ]
+            topology['ntopatoms']     = len(topology['atomindex_byId'].keys())
+            topology['natoms']        = len(onlyatoms)
+    
+            #Check for residue total charge
+            if abs( sum(topology['atomcharges']) - topology['rescharge'] ) > 0.00001:
+                print('Warning: Your total charge does not match the sum of partial charges.')
+    
+        elif not found:
+            print ('Could not find the residue name: '+topology['resname']+' in the provided topology file.')
+        filein.close()
+        return topology
 
-    def loadCharmmTopology(self,resname,resitopfile): 
+    def loadCharmmTopology(self,resname,resitopfile,bio=True): 
         """
         Load topology information using CHARMM force field and store it as attributes.
         
         Args:
             resname (str): Name of the residue.
             resitopfile (str): Path to the CHARMM topology file.
         """
 
-        topology = readCharmmTopology(resname,resitopfile)
+        topology = self.readCharmmTopology(resname,resitopfile,bio)
         for key,value in topology.items():
             self._assignattr(key,value)
     
     def _assignattr(self, key, value):
         """
         Private method to assign attributes to the class instance.
 
         Args:
             key: The attribute name.
             value: The value to assign to the attribute.
         """
         setattr(self, key, value)  
 
+class WriteCharmmTopology():
+    @staticmethod
+    def rtf_header(header):
+        text="* %s\n* Written by: amolkit\n*\n"%(header)
+        return text
+    
+    @staticmethod
+    def rtf_ioformat(extended=True):
+        if extended: text="ioformat extended"
+        return text
+    
+    @staticmethod
+    def rtf_readinstruct(append=True):
+        if append:
+            text="read rtf card append"
+        else:
+            text="read rtf card"
+        return text
+    
+    @staticmethod
+    def rtf_version(version):
+        return str(version)
+    
+    @staticmethod
+    def rtf_autogenangdih(drude=True):
+        if drude: 
+            text = "AUTO ANGL DIHE DRUD"
+        else:    
+            text = "AUTO ANGL DIHE"
+        return text    
+    
+    @staticmethod
+    def rtf_comment(comment):
+        return comment
+    
+    @staticmethod
+    def rtf_end():
+        return "END\n\n"
```

