# Comparing `tmp/TP_Generator-2024.3.3.tar.gz` & `tmp/TP_Generator-2024.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/TP_Generator-2024.3.3.tar", last modified: Sun Mar  3 15:52:31 2024, max compression
+gzip compressed data, was "dist/TP_Generator-2024.4.5.tar", last modified: Fri Apr  5 14:06:59 2024, max compression
```

## Comparing `TP_Generator-2024.3.3.tar` & `TP_Generator-2024.4.5.tar`

### file list

```diff
@@ -1,8 +1,18 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-03 15:52:30.000000 TP_Generator-2024.3.3/
--rwxrwxrwx   0 root         (0) root         (0)     3593 2024-03-03 15:52:31.000000 TP_Generator-2024.3.3/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-01 13:23:11.000000 TP_Generator-2024.3.3/requirements.txt
--rwxrwxrwx   0 root         (0) root         (0)      745 2024-03-03 08:28:39.000000 TP_Generator-2024.3.3/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-03 15:52:30.000000 TP_Generator-2024.3.3/TP_Generator/
--rwxrwxrwx   0 root         (0) root         (0)    11919 2024-03-03 07:58:03.000000 TP_Generator-2024.3.3/TP_Generator/AttackTypes.py
--rwxrwxrwx   0 root         (0) root         (0)      994 2024-03-01 17:10:42.000000 TP_Generator-2024.3.3/TP_Generator/MFA_Generator.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-01 13:56:31.000000 TP_Generator-2024.3.3/TP_Generator/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 14:06:59.000000 TP_Generator-2024.4.5/
+-rwxrwxrwx   0 root         (0) root         (0)     1093 2024-02-03 17:01:58.000000 TP_Generator-2024.4.5/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       24 2023-11-25 11:03:25.000000 TP_Generator-2024.4.5/MANIFEST.in
+-rwxrwxrwx   0 root         (0) root         (0)     3798 2024-04-05 14:06:59.000000 TP_Generator-2024.4.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2870 2024-04-05 13:55:55.000000 TP_Generator-2024.4.5/README.md
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-01 13:23:11.000000 TP_Generator-2024.4.5/requirements.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-05 14:06:59.000000 TP_Generator-2024.4.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      754 2024-04-05 13:49:58.000000 TP_Generator-2024.4.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 14:06:59.000000 TP_Generator-2024.4.5/TP_Generator/
+-rwxrwxrwx   0 root         (0) root         (0)    11919 2024-03-03 07:58:03.000000 TP_Generator-2024.4.5/TP_Generator/AttackTypes.py
+-rwxrwxrwx   0 root         (0) root         (0)     1986 2024-04-05 07:05:54.000000 TP_Generator-2024.4.5/TP_Generator/Bruteforcer_List.py
+-rwxrwxrwx   0 root         (0) root         (0)      994 2024-04-04 16:25:58.000000 TP_Generator-2024.4.5/TP_Generator/MFA_Generator.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-03-01 13:56:31.000000 TP_Generator-2024.4.5/TP_Generator/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-05 14:06:59.000000 TP_Generator-2024.4.5/TP_Generator.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-05 14:06:58.000000 TP_Generator-2024.4.5/TP_Generator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3798 2024-04-05 14:06:58.000000 TP_Generator-2024.4.5/TP_Generator.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      315 2024-04-05 14:06:58.000000 TP_Generator-2024.4.5/TP_Generator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)       13 2024-04-05 14:06:58.000000 TP_Generator-2024.4.5/TP_Generator.egg-info/top_level.txt
```

### Comparing `TP_Generator-2024.3.3/PKG-INFO` & `TP_Generator-2024.4.5/TP_Generator.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TP_Generator
-Version: 2024.3.3
+Name: TP-Generator
+Version: 2024.4.5
 Summary: UNKNOWN
 Home-page: https://github.com/truocphan/TP-Generator
 Author: TP Cyber Security
 Author-email: tpcybersec2023@gmail.com
 License: MIT
 Description: # TP-Generator
         
@@ -34,22 +34,26 @@
         cd TP-Generator
         python setup.py build
         python setup.py install
         ```
         
         ## Basic Usage
         ```
-        from TP_Generator import AttackTypes
+        from TP_Generator import AttackTypes, MFA_Generator, Bruteforcer_List
+        
         ```
         
         ## CHANGELOG
+        #### [TP-Generator v2024.4.5](https://github.com/truocphan/TP-Generator/tree/2024.4.5)
+        - **New**: _Bruteforcer_List_: **UUID1**
+        
         #### [TP-Generator v2024.3.3](https://github.com/truocphan/TP-Generator/tree/2024.3.3)
         - **New**: _MFA_Generator_: **TOTP** (Time-based One-Time Password) and **HOTP** (HMAC-based One-Time Password)
         
         #### [TP-Generator v2024.3.1](https://github.com/truocphan/TP-Generator/tree/2024.3.1)
         - **New**: Generate test cases for attack types: **_Sniper_**, **_Battering Ram_**, **_Pitchfork_**, **_Cluster Bomb_**
-Keywords: TPCyberSec,TP-Generator,Sniper Attack,Batteringram Attack,Pitchfork Attack,Clusterbomb Attack,TOTP/ HOTP Generate
+Keywords: TPCyberSec,TP-Generator,Sniper Attack,Batteringram Attack,Pitchfork Attack,Clusterbomb Attack,TOTP/ HOTP Generate,UUID1
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TP_Generator Version: 2024.3.3 Summary: UNKNOWN
+Metadata-Version: 2.1 Name: TP-Generator Version: 2024.4.5 Summary: UNKNOWN
 Home-page: https://github.com/truocphan/TP-Generator Author: TP Cyber Security
 Author-email: tpcybersec2023@gmail.com License: MIT Description: # TP-Generator
     _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_r_e_l_e_a_s_e_/_t_r_u_o_c_p_h_a_n_/_T_P_-_G_e_n_e_r_a_t_o_r_]_[_h_t_t_p_s_:_/_/
     _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_d_o_w_n_l_o_a_d_s_/_t_r_u_o_c_p_h_a_n_/_T_P_-_G_e_n_e_r_a_t_o_r_/_t_o_t_a_l_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_t_r_u_o_c_p_h_a_n_/_T_P_-_G_e_n_e_r_a_t_o_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
   _g_i_t_h_u_b_/_f_o_r_k_s_/_t_r_u_o_c_p_h_a_n_/_T_P_-_G_e_n_e_r_a_t_o_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_/
 _t_r_u_o_c_p_h_a_n_/_T_P_-_G_e_n_e_r_a_t_o_r_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_i_s_s_u_e_s_-_c_l_o_s_e_d_/_t_r_u_o_c_p_h_a_n_/
@@ -15,18 +15,20 @@
   _b_a_d_g_e_/_G_m_a_i_l_-_D_1_4_8_3_6_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_g_m_a_i_l_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_B_u_y___M_e___A___C_o_f_f_e_e_-_F_F_D_D_0_0_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_=_b_u_y_-_m_e_-_a_-
                             _c_o_f_f_e_e_&_l_o_g_o_C_o_l_o_r_=_b_l_a_c_k_]
 ## Installation #### From PyPI: ```console pip install TP-Generator ``` ####
 From Source: ```console git clone https://github.com/truocphan/TP-Generator.git
 --branch
 ag> cd TP-Generator python setup.py build python setup.py install ``` ## Basic
-Usage ``` from TP_Generator import AttackTypes ``` ## CHANGELOG #### [TP-
+Usage ``` from TP_Generator import AttackTypes, MFA_Generator, Bruteforcer_List
+``` ## CHANGELOG #### [TP-Generator v2024.4.5](https://github.com/truocphan/TP-
+Generator/tree/2024.4.5) - **New**: _Bruteforcer_List_: **UUID1** #### [TP-
 Generator v2024.3.3](https://github.com/truocphan/TP-Generator/tree/2024.3.3) -
 **New**: _MFA_Generator_: **TOTP** (Time-based One-Time Password) and **HOTP**
 (HMAC-based One-Time Password) #### [TP-Generator v2024.3.1](https://
 github.com/truocphan/TP-Generator/tree/2024.3.1) - **New**: Generate test cases
 for attack types: **_Sniper_**, **_Battering Ram_**, **_Pitchfork_**,
 **_Cluster Bomb_** Keywords: TPCyberSec,TP-Generator,Sniper Attack,Batteringram
-Attack,Pitchfork Attack,Clusterbomb Attack,TOTP/ HOTP Generate Platform:
+Attack,Pitchfork Attack,Clusterbomb Attack,TOTP/ HOTP Generate,UUID1 Platform:
 UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 2 Classifier: Programming Language :: Python ::
 Implementation :: Jython Description-Content-Type: text/markdown
```

### Comparing `TP_Generator-2024.3.3/setup.py` & `TP_Generator-2024.4.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 setuptools.setup(
 	name="TP_Generator",
-	version="2024.3.3",
+	version="2024.4.5",
 	author="TP Cyber Security",
 	license="MIT",
 	author_email="tpcybersec2023@gmail.com",
 	description="",
 	long_description=open("README.md").read(),
 	long_description_content_type="text/markdown",
 	install_requires=open("requirements.txt").read().split(),
 	url="https://github.com/truocphan/TP-Generator",
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"Programming Language :: Python :: 2",
 		"Programming Language :: Python :: Implementation :: Jython"
 	],
-	keywords=["TPCyberSec", "TP-Generator", "Sniper Attack", "Batteringram Attack", "Pitchfork Attack", "Clusterbomb Attack", "TOTP/ HOTP Generate"],
+	keywords=["TPCyberSec", "TP-Generator", "Sniper Attack", "Batteringram Attack", "Pitchfork Attack", "Clusterbomb Attack", "TOTP/ HOTP Generate", "UUID1"],
 	packages=["TP_Generator"],
 )
```

### Comparing `TP_Generator-2024.3.3/TP_Generator/AttackTypes.py` & `TP_Generator-2024.4.5/TP_Generator/AttackTypes.py`

 * *Files identical despite different names*

### Comparing `TP_Generator-2024.3.3/TP_Generator/MFA_Generator.py` & `TP_Generator-2024.4.5/TP_Generator/MFA_Generator.py`

 * *Files identical despite different names*

