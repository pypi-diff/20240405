# Comparing `tmp/iso_standards-0.1.1.tar.gz` & `tmp/iso_standards-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso_standards-0.1.1.tar", max compression
+gzip compressed data, was "iso_standards-0.1.2.tar", max compression
```

## Comparing `iso_standards-0.1.1.tar` & `iso_standards-0.1.2.tar`

### file list

```diff
@@ -1,213 +1,213 @@
--rw-r--r--   0        0        0      109 2024-03-03 22:33:53.484457 iso_standards-0.1.1/README.md
--rw-r--r--   0        0        0      637 2024-03-03 22:33:53.484457 iso_standards-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/__init__.py
--rw-r--r--   0        0        0      696 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/base.py
--rw-r--r--   0        0        0      118 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/errors.py
--rw-r--r--   0        0        0        0 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/__init__.py
--rw-r--r--   0        0        0    20326 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_1.py
--rw-r--r--   0        0        0      853 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AD.py
--rw-r--r--   0        0        0      857 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AE.py
--rw-r--r--   0        0        0     5726 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AF.py
--rw-r--r--   0        0        0      917 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AG.py
--rw-r--r--   0        0        0     1155 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AL.py
--rw-r--r--   0        0        0     1096 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AM.py
--rw-r--r--   0        0        0     1645 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AO.py
--rw-r--r--   0        0        0     2038 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AR.py
--rw-r--r--   0        0        0      951 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AT.py
--rw-r--r--   0        0        0      959 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AU.py
--rw-r--r--   0        0        0     5886 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AZ.py
--rw-r--r--   0        0        0     1170 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BA.py
--rw-r--r--   0        0        0     1141 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BB.py
--rw-r--r--   0        0        0     5719 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BD.py
--rw-r--r--   0        0        0     1488 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BE.py
--rw-r--r--   0        0        0     4729 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BF.py
--rw-r--r--   0        0        0     2312 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BG.py
--rw-r--r--   0        0        0      663 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BH.py
--rw-r--r--   0        0        0     3134 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BI.py
--rw-r--r--   0        0        0     1200 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BJ.py
--rw-r--r--   0        0        0      972 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BN.py
--rw-r--r--   0        0        0      975 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BO.py
--rw-r--r--   0        0        0     1104 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BQ.py
--rw-r--r--   0        0        0     2238 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BR.py
--rw-r--r--   0        0        0     2748 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BS.py
--rw-r--r--   0        0        0     1766 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BT.py
--rw-r--r--   0        0        0     1461 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BW.py
--rw-r--r--   0        0        0     2543 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BY.py
--rw-r--r--   0        0        0      769 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BZ.py
--rw-r--r--   0        0        0     2503 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CA.py
--rw-r--r--   0        0        0     2206 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CD.py
--rw-r--r--   0        0        0     3197 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CF.py
--rw-r--r--   0        0        0     1211 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CG.py
--rw-r--r--   0        0        0     2540 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CH.py
--rw-r--r--   0        0        0     1382 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CI.py
--rw-r--r--   0        0        0     1576 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CL.py
--rw-r--r--   0        0        0     1840 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CM.py
--rw-r--r--   0        0        0     3404 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CN.py
--rw-r--r--   0        0        0     2844 2024-03-03 22:33:53.484457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CO.py
--rw-r--r--   0        0        0      828 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CR.py
--rw-r--r--   0        0        0     1540 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CU.py
--rw-r--r--   0        0        0     2361 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CV.py
--rw-r--r--   0        0        0     1266 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CY.py
--rw-r--r--   0        0        0     7498 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CZ.py
--rw-r--r--   0        0        0     1472 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DE.py
--rw-r--r--   0        0        0     1252 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DJ.py
--rw-r--r--   0        0        0      699 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DK.py
--rw-r--r--   0        0        0     1063 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DM.py
--rw-r--r--   0        0        0     3588 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DO.py
--rw-r--r--   0        0        0     4477 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DZ.py
--rw-r--r--   0        0        0     2034 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/EC.py
--rw-r--r--   0        0        0     8272 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/EE.py
--rw-r--r--   0        0        0     2472 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/EG.py
--rw-r--r--   0        0        0     1353 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ER.py
--rw-r--r--   0        0        0     6491 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ES.py
--rw-r--r--   0        0        0     2644 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ET.py
--rw-r--r--   0        0        0     3424 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/FI.py
--rw-r--r--   0        0        0     1713 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/FJ.py
--rw-r--r--   0        0        0      611 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/FM.py
--rw-r--r--   0        0        0    12439 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/FR.py
--rw-r--r--   0        0        0      990 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GA.py
--rw-r--r--   0        0        0    20353 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GB.py
--rw-r--r--   0        0        0      867 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GD.py
--rw-r--r--   0        0        0     1250 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GE.py
--rw-r--r--   0        0        0     1444 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GH.py
--rw-r--r--   0        0        0      769 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GL.py
--rw-r--r--   0        0        0      762 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GM.py
--rw-r--r--   0        0        0     3485 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GN.py
--rw-r--r--   0        0        0     2684 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GQ.py
--rw-r--r--   0        0        0     1598 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GR.py
--rw-r--r--   0        0        0     1989 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GT.py
--rw-r--r--   0        0        0     1194 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GW.py
--rw-r--r--   0        0        0     1145 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GY.py
--rw-r--r--   0        0        0     1682 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/HN.py
--rw-r--r--   0        0        0     2165 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/HR.py
--rw-r--r--   0        0        0     1910 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/HT.py
--rw-r--r--   0        0        0     3799 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/HU.py
--rw-r--r--   0        0        0     3970 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ID.py
--rw-r--r--   0        0        0     5123 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IE.py
--rw-r--r--   0        0        0     1280 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IL.py
--rw-r--r--   0        0        0     3037 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IN.py
--rw-r--r--   0        0        0     2164 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IQ.py
--rw-r--r--   0        0        0     2681 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IR.py
--rw-r--r--   0        0        0     6694 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IS.py
--rw-r--r--   0        0        0    10433 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IT.py
--rw-r--r--   0        0        0     1342 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/JM.py
--rw-r--r--   0        0        0     1251 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/JO.py
--rw-r--r--   0        0        0     5663 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/JP.py
--rw-r--r--   0        0        0     3550 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KE.py
--rw-r--r--   0        0        0     2386 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KG.py
--rw-r--r--   0        0        0     4414 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KH.py
--rw-r--r--   0        0        0      726 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KI.py
--rw-r--r--   0        0        0     1151 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KM.py
--rw-r--r--   0        0        0     1686 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KN.py
--rw-r--r--   0        0        0     2510 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KP.py
--rw-r--r--   0        0        0     1887 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KR.py
--rw-r--r--   0        0        0      819 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KW.py
--rw-r--r--   0        0        0     5216 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KZ.py
--rw-r--r--   0        0        0     1650 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LA.py
--rw-r--r--   0        0        0     1678 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LB.py
--rw-r--r--   0        0        0     1058 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LC.py
--rw-r--r--   0        0        0     1105 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LI.py
--rw-r--r--   0        0        0     8516 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LK.py
--rw-r--r--   0        0        0     1379 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LR.py
--rw-r--r--   0        0        0     1888 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LS.py
--rw-r--r--   0        0        0     6466 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LT.py
--rw-r--r--   0        0        0     2926 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LU.py
--rw-r--r--   0        0        0     3894 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LV.py
--rw-r--r--   0        0        0     2013 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LY.py
--rw-r--r--   0        0        0     7241 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MA.py
--rw-r--r--   0        0        0     1583 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MC.py
--rw-r--r--   0        0        0     3010 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MD.py
--rw-r--r--   0        0        0     2147 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ME.py
--rw-r--r--   0        0        0      768 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MG.py
--rw-r--r--   0        0        0     4854 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MH.py
--rw-r--r--   0        0        0     6593 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MK.py
--rw-r--r--   0        0        0     1072 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ML.py
--rw-r--r--   0        0        0     1356 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MM.py
--rw-r--r--   0        0        0     1957 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MN.py
--rw-r--r--   0        0        0     1722 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MR.py
--rw-r--r--   0        0        0    11572 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MT.py
--rw-r--r--   0        0        0     1252 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MU.py
--rw-r--r--   0        0        0     4436 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MV.py
--rw-r--r--   0        0        0     5342 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MW.py
--rw-r--r--   0        0        0     2677 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MX.py
--rw-r--r--   0        0        0     1545 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MY.py
--rw-r--r--   0        0        0     1088 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MZ.py
--rw-r--r--   0        0        0     1307 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NA.py
--rw-r--r--   0        0        0      873 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NE.py
--rw-r--r--   0        0        0     2826 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NG.py
--rw-r--r--   0        0        0     1611 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NI.py
--rw-r--r--   0        0        0     1677 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NL.py
--rw-r--r--   0        0        0     2602 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NO.py
--rw-r--r--   0        0        0     1442 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NP.py
--rw-r--r--   0        0        0     2452 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NR.py
--rw-r--r--   0        0        0     3048 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NZ.py
--rw-r--r--   0        0        0     1224 2024-03-03 22:33:53.488457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/OM.py
--rw-r--r--   0        0        0     1371 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PA.py
--rw-r--r--   0        0        0     5978 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PE.py
--rw-r--r--   0        0        0     2005 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PG.py
--rw-r--r--   0        0        0    17480 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PH.py
--rw-r--r--   0        0        0     1617 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PK.py
--rw-r--r--   0        0        0     1577 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PL.py
--rw-r--r--   0        0        0     3032 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PS.py
--rw-r--r--   0        0        0     1812 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PT.py
--rw-r--r--   0        0        0     2752 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PW.py
--rw-r--r--   0        0        0     1665 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PY.py
--rw-r--r--   0        0        0      992 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/QA.py
--rw-r--r--   0        0        0     3379 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/RO.py
--rw-r--r--   0        0        0     2954 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/RS.py
--rw-r--r--   0        0        0    16739 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/RU.py
--rw-r--r--   0        0        0     1443 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/RW.py
--rw-r--r--   0        0        0     1295 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SA.py
--rw-r--r--   0        0        0     1081 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SB.py
--rw-r--r--   0        0        0     6291 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SC.py
--rw-r--r--   0        0        0     3188 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SD.py
--rw-r--r--   0        0        0     1914 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SE.py
--rw-r--r--   0        0        0      714 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SG.py
--rw-r--r--   0        0        0      601 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SH.py
--rw-r--r--   0        0        0    17152 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SI.py
--rw-r--r--   0        0        0      960 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SK.py
--rw-r--r--   0        0        0      693 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SL.py
--rw-r--r--   0        0        0     1048 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SM.py
--rw-r--r--   0        0        0     1300 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SN.py
--rw-r--r--   0        0        0     1590 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SO.py
--rw-r--r--   0        0        0     1055 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SR.py
--rw-r--r--   0        0        0     1071 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SS.py
--rw-r--r--   0        0        0      847 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ST.py
--rw-r--r--   0        0        0     1387 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SV.py
--rw-r--r--   0        0        0     1359 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SY.py
--rw-r--r--   0        0        0      946 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SZ.py
--rw-r--r--   0        0        0     4113 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TD.py
--rw-r--r--   0        0        0      672 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TG.py
--rw-r--r--   0        0        0     6082 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TH.py
--rw-r--r--   0        0        0      884 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TJ.py
--rw-r--r--   0        0        0     2467 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TL.py
--rw-r--r--   0        0        0      729 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TM.py
--rw-r--r--   0        0        0     2099 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TN.py
--rw-r--r--   0        0        0     1104 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TO.py
--rw-r--r--   0        0        0     6024 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TR.py
--rw-r--r--   0        0        0     1468 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TT.py
--rw-r--r--   0        0        0      966 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TV.py
--rw-r--r--   0        0        0     1960 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TW.py
--rw-r--r--   0        0        0     3070 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TZ.py
--rw-r--r--   0        0        0     2432 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/UA.py
--rw-r--r--   0        0        0    10885 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/UG.py
--rw-r--r--   0        0        0     1188 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/UM.py
--rw-r--r--   0        0        0     4380 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/US.py
--rw-r--r--   0        0        0     1735 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/UY.py
--rw-r--r--   0        0        0     1331 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/UZ.py
--rw-r--r--   0        0        0      775 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/VC.py
--rw-r--r--   0        0        0     2032 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/VE.py
--rw-r--r--   0        0        0     5019 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/VN.py
--rw-r--r--   0        0        0     1272 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/VU.py
--rw-r--r--   0        0        0      589 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/WF.py
--rw-r--r--   0        0        0     2096 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/WS.py
--rw-r--r--   0        0        0     2014 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/YE.py
--rw-r--r--   0        0        0     6775 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ZA.py
--rw-r--r--   0        0        0     1053 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ZM.py
--rw-r--r--   0        0        0     1099 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ZW.py
--rw-r--r--   0        0        0      765 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/__init__.py
--rw-r--r--   0        0        0      797 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/iso3166/types.py
--rw-r--r--   0        0        0       91 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/utils/__init__.py
--rw-r--r--   0        0        0     1175 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/utils/country.py
--rw-r--r--   0        0        0      194 2024-03-03 22:33:53.492457 iso_standards-0.1.1/src/iso_standards/utils/types.py
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 iso_standards-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      109 2024-04-05 01:39:31.583528 iso_standards-0.1.2/README.md
+-rw-r--r--   0        0        0      636 2024-04-05 01:39:31.583528 iso_standards-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/base.py
+-rw-r--r--   0        0        0      118 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/errors.py
+-rw-r--r--   0        0        0        0 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/__init__.py
+-rw-r--r--   0        0        0    20394 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_1.py
+-rw-r--r--   0        0        0      853 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AD.py
+-rw-r--r--   0        0        0      857 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AE.py
+-rw-r--r--   0        0        0     5726 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AF.py
+-rw-r--r--   0        0        0      917 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AG.py
+-rw-r--r--   0        0        0     1155 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AL.py
+-rw-r--r--   0        0        0     1096 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AM.py
+-rw-r--r--   0        0        0     1645 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AO.py
+-rw-r--r--   0        0        0     2038 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AR.py
+-rw-r--r--   0        0        0      951 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AT.py
+-rw-r--r--   0        0        0      959 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AU.py
+-rw-r--r--   0        0        0     5886 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AZ.py
+-rw-r--r--   0        0        0     1170 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BA.py
+-rw-r--r--   0        0        0     1141 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BB.py
+-rw-r--r--   0        0        0     5719 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BD.py
+-rw-r--r--   0        0        0     1488 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BE.py
+-rw-r--r--   0        0        0     4729 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BF.py
+-rw-r--r--   0        0        0     2312 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BG.py
+-rw-r--r--   0        0        0      663 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BH.py
+-rw-r--r--   0        0        0     3134 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BI.py
+-rw-r--r--   0        0        0     1200 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BJ.py
+-rw-r--r--   0        0        0      972 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BN.py
+-rw-r--r--   0        0        0      975 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BO.py
+-rw-r--r--   0        0        0     1104 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BQ.py
+-rw-r--r--   0        0        0     2238 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BR.py
+-rw-r--r--   0        0        0     2748 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BS.py
+-rw-r--r--   0        0        0     1766 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BT.py
+-rw-r--r--   0        0        0     1461 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BW.py
+-rw-r--r--   0        0        0     2543 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BY.py
+-rw-r--r--   0        0        0      769 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BZ.py
+-rw-r--r--   0        0        0     2503 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CA.py
+-rw-r--r--   0        0        0     2206 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CD.py
+-rw-r--r--   0        0        0     3197 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CF.py
+-rw-r--r--   0        0        0     1211 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CG.py
+-rw-r--r--   0        0        0     2540 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CH.py
+-rw-r--r--   0        0        0     1382 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CI.py
+-rw-r--r--   0        0        0     1576 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CL.py
+-rw-r--r--   0        0        0     1840 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CM.py
+-rw-r--r--   0        0        0     3404 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CN.py
+-rw-r--r--   0        0        0     2844 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CO.py
+-rw-r--r--   0        0        0      828 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CR.py
+-rw-r--r--   0        0        0     1540 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CU.py
+-rw-r--r--   0        0        0     2361 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CV.py
+-rw-r--r--   0        0        0     1266 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CY.py
+-rw-r--r--   0        0        0     7498 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CZ.py
+-rw-r--r--   0        0        0     1472 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DE.py
+-rw-r--r--   0        0        0     1252 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DJ.py
+-rw-r--r--   0        0        0      699 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DK.py
+-rw-r--r--   0        0        0     1063 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DM.py
+-rw-r--r--   0        0        0     3588 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DO.py
+-rw-r--r--   0        0        0     4477 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DZ.py
+-rw-r--r--   0        0        0     2034 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/EC.py
+-rw-r--r--   0        0        0     8272 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/EE.py
+-rw-r--r--   0        0        0     2472 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/EG.py
+-rw-r--r--   0        0        0     1353 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ER.py
+-rw-r--r--   0        0        0     6491 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ES.py
+-rw-r--r--   0        0        0     2644 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ET.py
+-rw-r--r--   0        0        0     3424 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/FI.py
+-rw-r--r--   0        0        0     1713 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/FJ.py
+-rw-r--r--   0        0        0      611 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/FM.py
+-rw-r--r--   0        0        0    12439 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/FR.py
+-rw-r--r--   0        0        0      990 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GA.py
+-rw-r--r--   0        0        0    20353 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GB.py
+-rw-r--r--   0        0        0      867 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GD.py
+-rw-r--r--   0        0        0     1250 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GE.py
+-rw-r--r--   0        0        0     1444 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GH.py
+-rw-r--r--   0        0        0      769 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GL.py
+-rw-r--r--   0        0        0      762 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GM.py
+-rw-r--r--   0        0        0     3485 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GN.py
+-rw-r--r--   0        0        0     2684 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GQ.py
+-rw-r--r--   0        0        0     1598 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GR.py
+-rw-r--r--   0        0        0     1989 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GT.py
+-rw-r--r--   0        0        0     1194 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GW.py
+-rw-r--r--   0        0        0     1145 2024-04-05 01:39:31.583528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GY.py
+-rw-r--r--   0        0        0     1682 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/HN.py
+-rw-r--r--   0        0        0     2165 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/HR.py
+-rw-r--r--   0        0        0     1910 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/HT.py
+-rw-r--r--   0        0        0     3799 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/HU.py
+-rw-r--r--   0        0        0     3970 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ID.py
+-rw-r--r--   0        0        0     5123 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IE.py
+-rw-r--r--   0        0        0     1280 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IL.py
+-rw-r--r--   0        0        0     3037 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IN.py
+-rw-r--r--   0        0        0     2164 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IQ.py
+-rw-r--r--   0        0        0     2681 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IR.py
+-rw-r--r--   0        0        0     6694 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IS.py
+-rw-r--r--   0        0        0    10433 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IT.py
+-rw-r--r--   0        0        0     1342 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/JM.py
+-rw-r--r--   0        0        0     1251 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/JO.py
+-rw-r--r--   0        0        0     5663 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/JP.py
+-rw-r--r--   0        0        0     3550 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KE.py
+-rw-r--r--   0        0        0     2386 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KG.py
+-rw-r--r--   0        0        0     4414 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KH.py
+-rw-r--r--   0        0        0      726 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KI.py
+-rw-r--r--   0        0        0     1151 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KM.py
+-rw-r--r--   0        0        0     1686 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KN.py
+-rw-r--r--   0        0        0     2510 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KP.py
+-rw-r--r--   0        0        0     1887 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KR.py
+-rw-r--r--   0        0        0      819 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KW.py
+-rw-r--r--   0        0        0     5216 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KZ.py
+-rw-r--r--   0        0        0     1650 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LA.py
+-rw-r--r--   0        0        0     1678 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LB.py
+-rw-r--r--   0        0        0     1058 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LC.py
+-rw-r--r--   0        0        0     1105 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LI.py
+-rw-r--r--   0        0        0     8516 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LK.py
+-rw-r--r--   0        0        0     1379 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LR.py
+-rw-r--r--   0        0        0     1888 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LS.py
+-rw-r--r--   0        0        0     6466 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LT.py
+-rw-r--r--   0        0        0     2926 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LU.py
+-rw-r--r--   0        0        0     3894 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LV.py
+-rw-r--r--   0        0        0     2013 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LY.py
+-rw-r--r--   0        0        0     7241 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MA.py
+-rw-r--r--   0        0        0     1583 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MC.py
+-rw-r--r--   0        0        0     3010 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MD.py
+-rw-r--r--   0        0        0     2147 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ME.py
+-rw-r--r--   0        0        0      768 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MG.py
+-rw-r--r--   0        0        0     4854 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MH.py
+-rw-r--r--   0        0        0     6593 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MK.py
+-rw-r--r--   0        0        0     1072 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ML.py
+-rw-r--r--   0        0        0     1356 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MM.py
+-rw-r--r--   0        0        0     1957 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MN.py
+-rw-r--r--   0        0        0     1722 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MR.py
+-rw-r--r--   0        0        0    11572 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MT.py
+-rw-r--r--   0        0        0     1252 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MU.py
+-rw-r--r--   0        0        0     4436 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MV.py
+-rw-r--r--   0        0        0     5342 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MW.py
+-rw-r--r--   0        0        0     2677 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MX.py
+-rw-r--r--   0        0        0     1545 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MY.py
+-rw-r--r--   0        0        0     1088 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MZ.py
+-rw-r--r--   0        0        0     1307 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NA.py
+-rw-r--r--   0        0        0      873 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NE.py
+-rw-r--r--   0        0        0     2826 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NG.py
+-rw-r--r--   0        0        0     1611 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NI.py
+-rw-r--r--   0        0        0     1677 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NL.py
+-rw-r--r--   0        0        0     2602 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NO.py
+-rw-r--r--   0        0        0     1442 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NP.py
+-rw-r--r--   0        0        0     2452 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NR.py
+-rw-r--r--   0        0        0     3048 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NZ.py
+-rw-r--r--   0        0        0     1224 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/OM.py
+-rw-r--r--   0        0        0     1371 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PA.py
+-rw-r--r--   0        0        0     5978 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PE.py
+-rw-r--r--   0        0        0     2005 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PG.py
+-rw-r--r--   0        0        0    17480 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PH.py
+-rw-r--r--   0        0        0     1617 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PK.py
+-rw-r--r--   0        0        0     1577 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PL.py
+-rw-r--r--   0        0        0     3032 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PS.py
+-rw-r--r--   0        0        0     1812 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PT.py
+-rw-r--r--   0        0        0     2752 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PW.py
+-rw-r--r--   0        0        0     1665 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PY.py
+-rw-r--r--   0        0        0      992 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/QA.py
+-rw-r--r--   0        0        0     3379 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/RO.py
+-rw-r--r--   0        0        0     2954 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/RS.py
+-rw-r--r--   0        0        0    16739 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/RU.py
+-rw-r--r--   0        0        0     1443 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/RW.py
+-rw-r--r--   0        0        0     1295 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SA.py
+-rw-r--r--   0        0        0     1081 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SB.py
+-rw-r--r--   0        0        0     6291 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SC.py
+-rw-r--r--   0        0        0     3188 2024-04-05 01:39:31.587528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SD.py
+-rw-r--r--   0        0        0     1914 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SE.py
+-rw-r--r--   0        0        0      714 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SG.py
+-rw-r--r--   0        0        0      601 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SH.py
+-rw-r--r--   0        0        0    17152 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SI.py
+-rw-r--r--   0        0        0      960 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SK.py
+-rw-r--r--   0        0        0      693 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SL.py
+-rw-r--r--   0        0        0     1048 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SM.py
+-rw-r--r--   0        0        0     1300 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SN.py
+-rw-r--r--   0        0        0     1590 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SO.py
+-rw-r--r--   0        0        0     1055 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SR.py
+-rw-r--r--   0        0        0     1071 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SS.py
+-rw-r--r--   0        0        0      847 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ST.py
+-rw-r--r--   0        0        0     1387 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SV.py
+-rw-r--r--   0        0        0     1359 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SY.py
+-rw-r--r--   0        0        0      946 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SZ.py
+-rw-r--r--   0        0        0     4113 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TD.py
+-rw-r--r--   0        0        0      672 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TG.py
+-rw-r--r--   0        0        0     6082 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TH.py
+-rw-r--r--   0        0        0      884 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TJ.py
+-rw-r--r--   0        0        0     2467 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TL.py
+-rw-r--r--   0        0        0      729 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TM.py
+-rw-r--r--   0        0        0     2099 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TN.py
+-rw-r--r--   0        0        0     1104 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TO.py
+-rw-r--r--   0        0        0     6024 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TR.py
+-rw-r--r--   0        0        0     1468 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TT.py
+-rw-r--r--   0        0        0      966 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TV.py
+-rw-r--r--   0        0        0     1960 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TW.py
+-rw-r--r--   0        0        0     3070 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TZ.py
+-rw-r--r--   0        0        0     2432 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/UA.py
+-rw-r--r--   0        0        0    10885 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/UG.py
+-rw-r--r--   0        0        0     1188 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/UM.py
+-rw-r--r--   0        0        0     4380 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/US.py
+-rw-r--r--   0        0        0     1735 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/UY.py
+-rw-r--r--   0        0        0     1331 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/UZ.py
+-rw-r--r--   0        0        0      775 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/VC.py
+-rw-r--r--   0        0        0     2032 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/VE.py
+-rw-r--r--   0        0        0     5019 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/VN.py
+-rw-r--r--   0        0        0     1272 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/VU.py
+-rw-r--r--   0        0        0      589 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/WF.py
+-rw-r--r--   0        0        0     2096 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/WS.py
+-rw-r--r--   0        0        0     2014 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/YE.py
+-rw-r--r--   0        0        0     6775 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ZA.py
+-rw-r--r--   0        0        0     1053 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ZM.py
+-rw-r--r--   0        0        0     1099 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ZW.py
+-rw-r--r--   0        0        0      833 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/iso3166/types.py
+-rw-r--r--   0        0        0      117 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/utils/__init__.py
+-rw-r--r--   0        0        0     1273 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/utils/iso3166_based.py
+-rw-r--r--   0        0        0      212 2024-04-05 01:39:31.591528 iso_standards-0.1.2/src/iso_standards/utils/types.py
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 iso_standards-0.1.2/PKG-INFO
```

### Comparing `iso_standards-0.1.1/pyproject.toml` & `iso_standards-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "iso-standards"
-version = "0.1.1"
-description = "ISO Standards"
+version = "0.1.2"
+description = "ISO standards"
 authors = ["Arkadii Yakovets <ark@cho.red>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.2.0"
 pytest = "^8.0.0"
 requests = "^2.31.0"
 
-
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.2"
 
 [tool.isort]
 known_first_party = ["iso_standards", "tests"]
 line_length = 100
 multi_line_output = 3
```

### Comparing `iso_standards-0.1.1/src/iso_standards/base.py` & `iso_standards-0.1.2/src/iso_standards/base.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_1.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_1.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,7 +334,10 @@
         "WS": Entity("Samoa", "WS", "WSM", "882", "Samoa", ""),
         "YE": Entity("Yemen", "YE", "YEM", "887", "Yemen", ""),
         "YT": Entity("Mayotte", "YT", "MYT", "175", "Mayotte", "FR"),
         "ZA": Entity("South Africa", "ZA", "ZAF", "710", "South Africa", ""),
         "ZM": Entity("Zambia", "ZM", "ZMB", "894", "Zambia", ""),
         "ZW": Entity("Zimbabwe", "ZW", "ZWE", "716", "Zimbabwe", ""),
     }
+
+    def __str__(self) -> str:
+        return "ISO 3166-1 entities"
```

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AD.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AD.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AF.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AF.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AL.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AL.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AO.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AO.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AT.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AT.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AU.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AU.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/AZ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/AZ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BB.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BB.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BD.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BD.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BF.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BF.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BH.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BH.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BI.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BI.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BJ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BJ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BN.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BN.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BO.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BO.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BQ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BQ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BS.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BS.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BT.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BT.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BW.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BW.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BY.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BY.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/BZ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/BZ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CD.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CD.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CF.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CF.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CH.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CH.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CI.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CI.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CL.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CL.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CN.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CN.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CO.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CO.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CU.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CU.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CV.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CV.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CY.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CY.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/CZ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/CZ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DJ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DJ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DK.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DK.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DO.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DO.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/DZ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/DZ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/EC.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/EC.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/EE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/EE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/EG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/EG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ER.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ER.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ES.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ES.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ET.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ET.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/FI.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/FI.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/FJ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/FJ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/FM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/FM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/FR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/FR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GB.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GB.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GD.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GD.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GH.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GH.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GL.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GL.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GN.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GN.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GQ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GQ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GT.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GT.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GW.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GW.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/GY.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/GY.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/HN.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/HN.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/HR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/HR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/HT.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/HT.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/HU.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/HU.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ID.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ID.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IL.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IL.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IN.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IN.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IQ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IQ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IS.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IS.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/IT.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/IT.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/JM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/JM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/JO.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/JO.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/JP.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/JP.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KH.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KH.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KI.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KI.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KN.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KN.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KP.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KP.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KW.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KW.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/KZ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/KZ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LB.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LB.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LC.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LC.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LI.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LI.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LK.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LK.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LS.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LS.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LT.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LT.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LU.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LU.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LV.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LV.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/LY.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/LY.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MC.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MC.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MD.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MD.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ME.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ME.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MH.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MH.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MK.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MK.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ML.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ML.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MN.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MN.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MT.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MT.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MU.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MU.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MV.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MV.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MW.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MW.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MX.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MX.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MY.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MY.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/MZ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/MZ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NI.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NI.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NL.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NL.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NO.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NO.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NP.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NP.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/NZ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/NZ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/OM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/OM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PH.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PH.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PK.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PK.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PL.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PL.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PS.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PS.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PT.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PT.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PW.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PW.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/PY.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/PY.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/QA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/QA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/RO.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/RO.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/RS.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/RS.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/RU.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/RU.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/RW.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/RW.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SB.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SB.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SC.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SC.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SD.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SD.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SH.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SH.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SI.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SI.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SK.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SK.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SL.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SL.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SN.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SN.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SO.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SO.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SS.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SS.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ST.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ST.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SV.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SV.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SY.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SY.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/SZ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/SZ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TD.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TD.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TH.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TH.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TJ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TJ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TL.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TL.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TN.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TN.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TO.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TO.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TR.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TR.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TT.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TT.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TV.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TV.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TW.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TW.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/TZ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/TZ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/UA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/UA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/UG.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/UG.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/UM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/UM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/US.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/US.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/UY.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/UY.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/UZ.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/UZ.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/VC.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/VC.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/VE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/VE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/VN.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/VN.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/VU.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/VU.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/WF.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/WF.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/WS.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/WS.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/YE.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/YE.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ZA.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ZA.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ZM.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ZM.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/ZW.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/ZW.py`

 * *Files identical despite different names*

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/iso3166_2/__init__.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/iso3166_2/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,7 +23,10 @@
         for module_name in sorted(Path(__file__).parent.rglob("??.py")):
             self.entities.update(
                 getattr(
                     import_module(f"iso_standards.iso3166.iso3166_2.{module_name.stem}"),
                     "Iso3166_2",
                 ).entities
             )
+
+    def __str__(self) -> str:
+        return "ISO 3166-2 entities"
```

### Comparing `iso_standards-0.1.1/src/iso_standards/iso3166/types.py` & `iso_standards-0.1.2/src/iso_standards/iso3166/types.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""ISO 3166 related types."""
+
 from typing import NamedTuple
 
 
 class Iso3166_1(NamedTuple):
     """ISO 3166-1 lightweight immutable entity."""
 
     # Country name, short form.
@@ -18,14 +20,17 @@
 
     # Country name, long form .
     long_name: str
 
     # Sovereign country code.
     parent_code: str = ""
 
+    def __str__(self) -> str:
+        return f"ISO 3166-1 {self.alpha_2}"
+
     @property
     def is_independent(self):
         return self.parent_code == ""
 
 
 class Iso3166_2(NamedTuple):
     """ISO 3166-2 lightweight immutable entity."""
@@ -40,7 +45,10 @@
     category: str
 
     # Language code.
     language_code: str
 
     # Parent code.
     parent_code: str = ""
+
+    def __str__(self) -> str:
+        return f"ISO 3166-2 {self.code}"
```

### Comparing `iso_standards-0.1.1/src/iso_standards/utils/country.py` & `iso_standards-0.1.2/src/iso_standards/utils/iso3166_based.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-"""A consolidated country data.
+"""A consolidated ISO 3166 based entities data.
 
 It contains data from different ISO standards grouped by a specific entity.
 """
 
 from importlib import import_module
 
 from iso_standards.base import EntityCollection
 from iso_standards.iso3166.iso3166_1 import Iso3166_1
-from iso_standards.utils.types import Country
+from iso_standards.utils.types import Iso3166BasedEntity
 
 
-class CountryCollection(EntityCollection):
+class Iso3166BasedEntities(EntityCollection):
     __slots__ = ()
 
     entities = {}
 
     def __init__(self):
         super().__init__()
 
@@ -24,19 +24,22 @@
                 subdivisions = getattr(
                     import_module(f"iso_standards.iso3166.iso3166_2.{iso3166_1.alpha_2}"),
                     "Iso3166_2",
                 )()
             except ModuleNotFoundError:
                 pass
 
-            country = Country(
+            country = Iso3166BasedEntity(
                 iso3166_1.short_name,
                 iso3166_1.alpha_2,
                 iso3166_1.alpha_3,
                 iso3166_1.num_3,
                 iso3166_1.long_name,
                 iso3166_1.parent_code,
             )
             # Add additional attributes.
             country.subdivisions = subdivisions
 
             self.entities[iso3166_1.alpha_2] = country
+
+    def __str__(self) -> str:
+        return "ISO 3166"
```

### Comparing `iso_standards-0.1.1/PKG-INFO` & `iso_standards-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: iso-standards
-Version: 0.1.1
-Summary: ISO Standards
+Version: 0.1.2
+Summary: ISO standards
 License: MIT
 Author: Arkadii Yakovets
 Author-email: ark@cho.red
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

