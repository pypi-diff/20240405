# Comparing `tmp/oras-0.1.28.tar.gz` & `tmp/oras-0.1.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oras-0.1.28.tar", last modified: Mon Mar 18 11:23:11 2024, max compression
+gzip compressed data, was "oras-0.1.29.tar", last modified: Fri Apr  5 17:27:10 2024, max compression
```

## Comparing `oras-0.1.28.tar` & `oras-0.1.29.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:23:11.002110 oras-0.1.28/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-03-18 11:22:55.000000 oras-0.1.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-18 11:22:55.000000 oras-0.1.28/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-03-18 11:23:11.002110 oras-0.1.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7647 2024-03-18 11:22:55.000000 oras-0.1.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:23:10.998110 oras-0.1.28/oras/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-18 11:22:55.000000 oras-0.1.28/oras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-18 11:22:55.000000 oras-0.1.28/oras/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-03-18 11:22:55.000000 oras-0.1.28/oras/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-03-18 11:22:55.000000 oras-0.1.28/oras/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-18 11:22:55.000000 oras-0.1.28/oras/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-03-18 11:22:55.000000 oras-0.1.28/oras/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-03-18 11:22:55.000000 oras-0.1.28/oras/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:23:10.998110 oras-0.1.28/oras/main/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 11:22:55.000000 oras-0.1.28/oras/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-18 11:22:55.000000 oras-0.1.28/oras/main/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-03-18 11:22:55.000000 oras-0.1.28/oras/oci.py
--rw-r--r--   0 runner    (1001) docker     (127)    37668 2024-03-18 11:22:55.000000 oras-0.1.28/oras/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-03-18 11:22:55.000000 oras-0.1.28/oras/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:23:10.998110 oras-0.1.28/oras/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 11:22:55.000000 oras-0.1.28/oras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-18 11:22:55.000000 oras-0.1.28/oras/tests/annotations.json
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-18 11:22:55.000000 oras-0.1.28/oras/tests/artifact.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-18 11:22:55.000000 oras-0.1.28/oras/tests/conftest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-03-18 11:22:55.000000 oras-0.1.28/oras/tests/run_registry.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-03-18 11:22:55.000000 oras-0.1.28/oras/tests/test_oras.py
--rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-03-18 11:22:55.000000 oras-0.1.28/oras/tests/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-03-18 11:22:55.000000 oras-0.1.28/oras/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:23:10.998110 oras-0.1.28/oras/tests/upload_data/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-18 11:22:55.000000 oras-0.1.28/oras/tests/upload_data/artifact.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:23:11.002110 oras-0.1.28/oras/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-18 11:22:55.000000 oras-0.1.28/oras/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-03-18 11:22:55.000000 oras-0.1.28/oras/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-18 11:22:55.000000 oras-0.1.28/oras/utils/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-18 11:22:55.000000 oras-0.1.28/oras/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 11:23:10.998110 oras-0.1.28/oras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-03-18 11:23:10.000000 oras-0.1.28/oras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-03-18 11:23:10.000000 oras-0.1.28/oras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 11:23:10.000000 oras-0.1.28/oras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 11:23:02.000000 oras-0.1.28/oras.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-18 11:23:10.000000 oras-0.1.28/oras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-18 11:23:10.000000 oras-0.1.28/oras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-03-18 11:22:55.000000 oras-0.1.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-03-18 11:23:11.002110 oras-0.1.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-03-18 11:22:55.000000 oras-0.1.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-04-05 17:27:00.000000 oras-0.1.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-05 17:27:00.000000 oras-0.1.29/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-05 17:27:10.293628 oras-0.1.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7981 2024-04-05 17:27:00.000000 oras-0.1.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-05 17:27:00.000000 oras-0.1.29/oras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-05 17:27:00.000000 oras-0.1.29/oras/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7686 2024-04-05 17:27:00.000000 oras-0.1.29/oras/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-05 17:27:00.000000 oras-0.1.29/oras/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-05 17:27:00.000000 oras-0.1.29/oras/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-05 17:27:00.000000 oras-0.1.29/oras/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8723 2024-04-05 17:27:00.000000 oras-0.1.29/oras/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras/main/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:00.000000 oras-0.1.29/oras/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-05 17:27:00.000000 oras-0.1.29/oras/main/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-04-05 17:27:00.000000 oras-0.1.29/oras/oci.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39049 2024-04-05 17:27:00.000000 oras-0.1.29/oras/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-05 17:27:00.000000 oras-0.1.29/oras/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/annotations.json
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/artifact.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/conftest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      185 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/run_registry.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/test_oras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras/tests/upload_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-05 17:27:00.000000 oras-0.1.29/oras/tests/upload_data/artifact.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-05 17:27:00.000000 oras-0.1.29/oras/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10737 2024-04-05 17:27:00.000000 oras-0.1.29/oras/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-05 17:27:00.000000 oras-0.1.29/oras/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-05 17:27:00.000000 oras-0.1.29/oras/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:27:10.293628 oras-0.1.29/oras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-04-05 17:27:10.000000 oras-0.1.29/oras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-05 17:27:10.000000 oras-0.1.29/oras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:27:10.000000 oras-0.1.29/oras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:27:02.000000 oras-0.1.29/oras.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 17:27:10.000000 oras-0.1.29/oras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-05 17:27:10.000000 oras-0.1.29/oras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-05 17:27:00.000000 oras-0.1.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-05 17:27:10.297628 oras-0.1.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-05 17:27:00.000000 oras-0.1.29/setup.py
```

### Comparing `oras-0.1.28/LICENSE` & `oras-0.1.29/LICENSE`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/PKG-INFO` & `oras-0.1.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.28
+Version: 0.1.29
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
@@ -22,15 +22,15 @@
 Provides-Extra: tests
 Provides-Extra: docker
 License-File: LICENSE
 
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-18-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-19-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -71,14 +71,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://terryhowe.wordpress.com/"><img src="https://avatars.githubusercontent.com/u/104113?v=4?s=100" width="100px;" alt="Terry Howe"/><br /><sub><b>Terry Howe</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=TerryHowe" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://saketjajoo.github.io"><img src="https://avatars.githubusercontent.com/u/23132557?v=4?s=100" width="100px;" alt="Saket Jajoo"/><br /><sub><b>Saket Jajoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=saketjajoo" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/miker985"><img src="https://avatars.githubusercontent.com/u/26555712?v=4?s=100" width="100px;" alt="Mike"/><br /><sub><b>Mike</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=miker985" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/linshokaku"><img src="https://avatars.githubusercontent.com/u/18627646?v=4?s=100" width="100px;" alt="deoxy"/><br /><sub><b>deoxy</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=linshokaku" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kavish-p"><img src="https://avatars.githubusercontent.com/u/29086148?v=4?s=100" width="100px;" alt="Kavish Punchoo"/><br /><sub><b>Kavish Punchoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=kavish-p" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/my5cents"><img src="https://avatars.githubusercontent.com/u/4820203?v=4?s=100" width="100px;" alt="my5cents"/><br /><sub><b>my5cents</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=my5cents" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.28 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.29 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests Provides-Extra: docker License-File:
 LICENSE # ORAS Python [![All Contributors](https://img.shields.io/badge/
-all_contributors-18-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
+all_contributors-19-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
 (https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
 foundation/blob/master/code-of-conduct.md). Please follow it in all your
 interactions with the project members and users. ## ðï¸ Contributors
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
-_[_V_a_n_e_s_s_a_s_a_u_r_u_s_] _[_L_a_c_h_l_a_n _[_S_t_e_v_e      _[_J_o_s_h     _[_B_r_i_d_g_e_t   _[_M_a_t_t      _[_W_o_l_f
- _VV_aa_nn_ee_ss_ss_aa_ss_aa_uu_rr_uu_ss  _E_v_e_n_s_o_n_] _L_a_s_k_e_r_]   _D_o_l_i_t_s_k_y_]   _K_r_o_m_h_o_u_t_] _W_a_r_n_e_r_]  _V_o_l_l_p_r_e_c_h_t_]
-     _ð___»       _LL_aa_cc_hh_ll_aa_nn   _SS_tt_ee_vv_ee  _JJ_oo_ss_hh_ _DD_oo_ll_ii_tt_ss_kk_yy  _BB_rr_ii_dd_gg_ee_tt    _MM_aa_tt_tt      _WW_oo_ll_ff
-                _EE_vv_ee_nn_ss_oo_nn  _LL_aa_ss_kk_ee_rr      _ð___»      _KK_rr_oo_mm_hh_oo_uu_tt   _WW_aa_rr_nn_ee_rr  _VV_oo_ll_ll_pp_rr_ee_cc_hh_tt
-                  _ð___»    _ð___»                   _ð___»      _ð___»      _ð___»
-_[_S_h_i_w_e_i_ _Z_h_a_n_g_]  _[_j_h_l_m_c_o_] _[_A_n_a_n_y_a _[_s_u_n_n_y_c_a_r_t_e_r_]  _[_M_a_r_i_u_s  _[_T_i_z_i_a_n_o   _[_T_e_r_r_y
- _SS_hh_ii_ww_ee_ii_ _ZZ_hh_aa_nn_gg    _jj_hh_ll_mm_cc_oo  _G_u_p_t_a_]   _ss_uu_nn_nn_yy_cc_aa_rr_tt_ee_rr  _B_e_r_t_r_a_m_]  _M_Ã_¼_l_l_e_r_]    _H_o_w_e_]
-     _ð___»         _ð___»   _AA_nn_aa_nn_yy_aa      _ð___»       _MM_aa_rr_ii_uu_ss   _TT_ii_zz_ii_aa_nn_oo  _TT_ee_rr_rr_yy_ _HH_oo_ww_ee
-                          _GG_uu_pp_tt_aa                 _BB_ee_rr_tt_rr_aa_mm  _MM_?Ã_?¼_ll_ll_ee_rr     _ð___»
-                          _ð___»                   _ð___»      _ð___»
- _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h
-  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]
-     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh
+_[_V_a_n_e_s_s_a_s_a_u_r_u_s_] _[_L_a_c_h_l_a_n _[_S_t_e_v_e      _[_J_o_s_h      _[_B_r_i_d_g_e_t   _[_M_a_t_t      _[_W_o_l_f
+ _VV_aa_nn_ee_ss_ss_aa_ss_aa_uu_rr_uu_ss  _E_v_e_n_s_o_n_] _L_a_s_k_e_r_]   _D_o_l_i_t_s_k_y_]   _K_r_o_m_h_o_u_t_]  _W_a_r_n_e_r_]  _V_o_l_l_p_r_e_c_h_t_]
+     _ð___»       _LL_aa_cc_hh_ll_aa_nn   _SS_tt_ee_vv_ee  _JJ_oo_ss_hh_ _DD_oo_ll_ii_tt_ss_kk_yy  _BB_rr_ii_dd_gg_ee_tt     _MM_aa_tt_tt      _WW_oo_ll_ff
+                _EE_vv_ee_nn_ss_oo_nn  _LL_aa_ss_kk_ee_rr      _ð___»       _KK_rr_oo_mm_hh_oo_uu_tt   _WW_aa_rr_nn_ee_rr  _VV_oo_ll_ll_pp_rr_ee_cc_hh_tt
+                  _ð___»    _ð___»                    _ð___»      _ð___»      _ð___»
+_[_S_h_i_w_e_i_ _Z_h_a_n_g_]  _[_j_h_l_m_c_o_] _[_A_n_a_n_y_a _[_s_u_n_n_y_c_a_r_t_e_r_]  _[_M_a_r_i_u_s   _[_T_i_z_i_a_n_o   _[_T_e_r_r_y
+ _SS_hh_ii_ww_ee_ii_ _ZZ_hh_aa_nn_gg    _jj_hh_ll_mm_cc_oo  _G_u_p_t_a_]   _ss_uu_nn_nn_yy_cc_aa_rr_tt_ee_rr   _B_e_r_t_r_a_m_]  _M_Ã_¼_l_l_e_r_]    _H_o_w_e_]
+     _ð___»         _ð___»   _AA_nn_aa_nn_yy_aa      _ð___»        _MM_aa_rr_ii_uu_ss   _TT_ii_zz_ii_aa_nn_oo  _TT_ee_rr_rr_yy_ _HH_oo_ww_ee
+                          _GG_uu_pp_tt_aa                 _BB_ee_rr_tt_rr_aa_mm   _MM_?Ã_?¼_ll_ll_ee_rr     _ð___»
+                          _ð___»                    _ð___»      _ð___»
+ _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h   _[_m_y_5_c_e_n_t_s_]
+  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]    _mm_yy_55_cc_ee_nn_tt_ss
+     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh       _ð___»
                                      _PP_uu_nn_cc_hh_oo_oo
                                       _ð___»
 ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.28/README.md` & `oras-0.1.29/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-18-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-19-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -46,14 +46,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://terryhowe.wordpress.com/"><img src="https://avatars.githubusercontent.com/u/104113?v=4?s=100" width="100px;" alt="Terry Howe"/><br /><sub><b>Terry Howe</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=TerryHowe" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://saketjajoo.github.io"><img src="https://avatars.githubusercontent.com/u/23132557?v=4?s=100" width="100px;" alt="Saket Jajoo"/><br /><sub><b>Saket Jajoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=saketjajoo" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/miker985"><img src="https://avatars.githubusercontent.com/u/26555712?v=4?s=100" width="100px;" alt="Mike"/><br /><sub><b>Mike</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=miker985" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/linshokaku"><img src="https://avatars.githubusercontent.com/u/18627646?v=4?s=100" width="100px;" alt="deoxy"/><br /><sub><b>deoxy</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=linshokaku" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kavish-p"><img src="https://avatars.githubusercontent.com/u/29086148?v=4?s=100" width="100px;" alt="Kavish Punchoo"/><br /><sub><b>Kavish Punchoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=kavish-p" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/my5cents"><img src="https://avatars.githubusercontent.com/u/4820203?v=4?s=100" width="100px;" alt="my5cents"/><br /><sub><b>my5cents</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=my5cents" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,29 +1,29 @@
 # ORAS Python [![All Contributors](https://img.shields.io/badge/
-all_contributors-18-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
+all_contributors-19-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
 (https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
 foundation/blob/master/code-of-conduct.md). Please follow it in all your
 interactions with the project members and users. ## ðï¸ Contributors
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
-_[_V_a_n_e_s_s_a_s_a_u_r_u_s_] _[_L_a_c_h_l_a_n _[_S_t_e_v_e      _[_J_o_s_h     _[_B_r_i_d_g_e_t   _[_M_a_t_t      _[_W_o_l_f
- _VV_aa_nn_ee_ss_ss_aa_ss_aa_uu_rr_uu_ss  _E_v_e_n_s_o_n_] _L_a_s_k_e_r_]   _D_o_l_i_t_s_k_y_]   _K_r_o_m_h_o_u_t_] _W_a_r_n_e_r_]  _V_o_l_l_p_r_e_c_h_t_]
-     _ð___»       _LL_aa_cc_hh_ll_aa_nn   _SS_tt_ee_vv_ee  _JJ_oo_ss_hh_ _DD_oo_ll_ii_tt_ss_kk_yy  _BB_rr_ii_dd_gg_ee_tt    _MM_aa_tt_tt      _WW_oo_ll_ff
-                _EE_vv_ee_nn_ss_oo_nn  _LL_aa_ss_kk_ee_rr      _ð___»      _KK_rr_oo_mm_hh_oo_uu_tt   _WW_aa_rr_nn_ee_rr  _VV_oo_ll_ll_pp_rr_ee_cc_hh_tt
-                  _ð___»    _ð___»                   _ð___»      _ð___»      _ð___»
-_[_S_h_i_w_e_i_ _Z_h_a_n_g_]  _[_j_h_l_m_c_o_] _[_A_n_a_n_y_a _[_s_u_n_n_y_c_a_r_t_e_r_]  _[_M_a_r_i_u_s  _[_T_i_z_i_a_n_o   _[_T_e_r_r_y
- _SS_hh_ii_ww_ee_ii_ _ZZ_hh_aa_nn_gg    _jj_hh_ll_mm_cc_oo  _G_u_p_t_a_]   _ss_uu_nn_nn_yy_cc_aa_rr_tt_ee_rr  _B_e_r_t_r_a_m_]  _M_Ã_¼_l_l_e_r_]    _H_o_w_e_]
-     _ð___»         _ð___»   _AA_nn_aa_nn_yy_aa      _ð___»       _MM_aa_rr_ii_uu_ss   _TT_ii_zz_ii_aa_nn_oo  _TT_ee_rr_rr_yy_ _HH_oo_ww_ee
-                          _GG_uu_pp_tt_aa                 _BB_ee_rr_tt_rr_aa_mm  _MM_?Ã_?¼_ll_ll_ee_rr     _ð___»
-                          _ð___»                   _ð___»      _ð___»
- _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h
-  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]
-     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh
+_[_V_a_n_e_s_s_a_s_a_u_r_u_s_] _[_L_a_c_h_l_a_n _[_S_t_e_v_e      _[_J_o_s_h      _[_B_r_i_d_g_e_t   _[_M_a_t_t      _[_W_o_l_f
+ _VV_aa_nn_ee_ss_ss_aa_ss_aa_uu_rr_uu_ss  _E_v_e_n_s_o_n_] _L_a_s_k_e_r_]   _D_o_l_i_t_s_k_y_]   _K_r_o_m_h_o_u_t_]  _W_a_r_n_e_r_]  _V_o_l_l_p_r_e_c_h_t_]
+     _ð___»       _LL_aa_cc_hh_ll_aa_nn   _SS_tt_ee_vv_ee  _JJ_oo_ss_hh_ _DD_oo_ll_ii_tt_ss_kk_yy  _BB_rr_ii_dd_gg_ee_tt     _MM_aa_tt_tt      _WW_oo_ll_ff
+                _EE_vv_ee_nn_ss_oo_nn  _LL_aa_ss_kk_ee_rr      _ð___»       _KK_rr_oo_mm_hh_oo_uu_tt   _WW_aa_rr_nn_ee_rr  _VV_oo_ll_ll_pp_rr_ee_cc_hh_tt
+                  _ð___»    _ð___»                    _ð___»      _ð___»      _ð___»
+_[_S_h_i_w_e_i_ _Z_h_a_n_g_]  _[_j_h_l_m_c_o_] _[_A_n_a_n_y_a _[_s_u_n_n_y_c_a_r_t_e_r_]  _[_M_a_r_i_u_s   _[_T_i_z_i_a_n_o   _[_T_e_r_r_y
+ _SS_hh_ii_ww_ee_ii_ _ZZ_hh_aa_nn_gg    _jj_hh_ll_mm_cc_oo  _G_u_p_t_a_]   _ss_uu_nn_nn_yy_cc_aa_rr_tt_ee_rr   _B_e_r_t_r_a_m_]  _M_Ã_¼_l_l_e_r_]    _H_o_w_e_]
+     _ð___»         _ð___»   _AA_nn_aa_nn_yy_aa      _ð___»        _MM_aa_rr_ii_uu_ss   _TT_ii_zz_ii_aa_nn_oo  _TT_ee_rr_rr_yy_ _HH_oo_ww_ee
+                          _GG_uu_pp_tt_aa                 _BB_ee_rr_tt_rr_aa_mm   _MM_?Ã_?¼_ll_ll_ee_rr     _ð___»
+                          _ð___»                    _ð___»      _ð___»
+ _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h   _[_m_y_5_c_e_n_t_s_]
+  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]    _mm_yy_55_cc_ee_nn_tt_ss
+     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh       _ð___»
                                      _PP_uu_nn_cc_hh_oo_oo
                                       _ð___»
 ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.28/oras/auth.py` & `oras-0.1.29/oras/auth.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/client.py` & `oras-0.1.29/oras/client.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/container.py` & `oras-0.1.29/oras/container.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/decorator.py` & `oras-0.1.29/oras/decorator.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/defaults.py` & `oras-0.1.29/oras/defaults.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/logger.py` & `oras-0.1.29/oras/logger.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/main/login.py` & `oras-0.1.29/oras/main/login.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/oci.py` & `oras-0.1.29/oras/oci.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/provider.py` & `oras-0.1.29/oras/provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -222,41 +222,48 @@
 
     def upload_blob(
         self,
         blob: str,
         container: container_type,
         layer: dict,
         do_chunked: bool = False,
+        refresh_headers: bool = True,
     ) -> requests.Response:
         """
         Prepare and upload a blob.
 
         Sizes > 1024 are uploaded via a chunked approach (post, patch+, put)
         and <= 1024 is a single post then put.
 
         :param blob: path to blob to upload
         :type blob: str
         :param container:  parsed container URI
         :type container: oras.container.Container or str
         :param layer: dict from oras.oci.NewLayer
         :type layer: dict
+        :param refresh_headers: if true, headers are refreshed
+        :type refresh_headers: bool
         """
         blob = os.path.abspath(blob)
         container = self.get_container(container)
 
         # Always reset headers between uploads
         self.reset_basic_auth()
 
         # Chunked for large, otherwise POST and PUT
         # This is currently disabled unless the user asks for it, as
         # it doesn't seem to work for all registries
         if not do_chunked:
-            response = self.put_upload(blob, container, layer)
+            response = self.put_upload(
+                blob, container, layer, refresh_headers=refresh_headers
+            )
         else:
-            response = self.chunked_upload(blob, container, layer)
+            response = self.chunked_upload(
+                blob, container, layer, refresh_headers=refresh_headers
+            )
 
         # If we have an empty layer digest and the registry didn't accept, just return dummy successful response
         if (
             response.status_code not in [200, 201, 202]
             and layer["digest"] == oras.defaults.blank_hash
         ):
             response = requests.Response()
@@ -470,28 +477,38 @@
         except Exception as e:
             if digest == oras.defaults.blank_hash:
                 return os.devnull
             raise e
         return outfile
 
     def put_upload(
-        self, blob: str, container: oras.container.Container, layer: dict
+        self,
+        blob: str,
+        container: oras.container.Container,
+        layer: dict,
+        refresh_headers: bool = True,
     ) -> requests.Response:
         """
         Upload to a registry via put.
 
         :param blob: path to blob to upload
         :type blob: str
         :param container:  parsed container URI
         :type container: oras.container.Container or str
         :param layer: dict from oras.oci.NewLayer
         :type layer: dict
+        :param refresh_headers: if true, headers are refreshed
+        :type refresh_headers: bool
         """
         # Start an upload session
         headers = {"Content-Type": "application/octet-stream"}
+
+        if not refresh_headers:
+            headers.update(self.headers)
+
         upload_url = f"{self.prefix}://{container.upload_blob_url()}"
         r = self.do_request(upload_url, "POST", headers=headers)
 
         # Location should be in the header
         session_url = self._get_location(r, container)
         if not session_url:
             raise ValueError(f"Issue retrieving session url: {r.json()}")
@@ -537,28 +554,37 @@
         prefix = f"{self.prefix}://{container.registry}"
 
         if not session_url.startswith("http"):
             session_url = f"{prefix}{session_url}"
         return session_url
 
     def chunked_upload(
-        self, blob: str, container: oras.container.Container, layer: dict
+        self,
+        blob: str,
+        container: oras.container.Container,
+        layer: dict,
+        refresh_headers: bool = True,
     ) -> requests.Response:
         """
         Upload via a chunked upload.
 
         :param blob: path to blob to upload
         :type blob: str
         :param container:  parsed container URI
         :type container: oras.container.Container or str
         :param layer: dict from oras.oci.NewLayer
         :type layer: dict
+        :param refresh_headers: if true, headers are refreshed
+        :type refresh_headers: bool
         """
         # Start an upload session
         headers = {"Content-Type": "application/octet-stream", "Content-Length": "0"}
+        if not refresh_headers:
+            headers.update(self.headers)
+
         upload_url = f"{self.prefix}://{container.upload_blob_url()}"
         r = self.do_request(upload_url, "POST", headers=headers)
 
         # Location should be in the header
         session_url = self._get_location(r, container)
         if not session_url:
             raise ValueError(f"Issue retrieving session url: {r.json()}")
@@ -614,30 +640,39 @@
             for error in msg.get("errors", []):
                 if isinstance(error, dict) and "message" in error:
                     logger.error(error["message"])
         except Exception:
             pass
 
     def upload_manifest(
-        self, manifest: dict, container: oras.container.Container
+        self,
+        manifest: dict,
+        container: oras.container.Container,
+        refresh_headers: bool = True,
     ) -> requests.Response:
         """
         Read a manifest file and upload it.
 
         :param manifest: manifest to upload
         :type manifest: dict
         :param container:  parsed container URI
         :type container: oras.container.Container or str
+        :param refresh_headers: if true, headers are refreshed
+        :type refresh_headers: bool
         """
         self.reset_basic_auth()
         jsonschema.validate(manifest, schema=oras.schemas.manifest)
         headers = {
             "Content-Type": oras.defaults.default_manifest_media_type,
             "Content-Length": str(len(manifest)),
         }
+
+        if not refresh_headers:
+            headers.update(self.headers)
+
         return self.do_request(
             f"{self.prefix}://{container.manifest_url()}",  # noqa
             "PUT",
             headers=headers,
             json=manifest,
         )
 
@@ -655,14 +690,16 @@
         :type insecure: bool
         :param annotation_file: manifest annotations file
         :type annotation_file: str
         :param manifest_annotations: manifest annotations
         :type manifest_annotations: dict
         :param target: target location to push to
         :type target: str
+        :param refresh_headers: if true or None, headers are refreshed
+        :type refresh_headers: bool
         :param subject: optional subject reference
         :type subject: Subject
         """
         container = self.get_container(kwargs["target"])
         self.load_configs(container, configs=kwargs.get("config_path"))
 
         # Hold state of request for http/https
@@ -671,14 +708,18 @@
         # Prepare a new manifest
         manifest = oras.oci.NewManifest()
 
         # A lookup of annotations we can add (to blobs or manifest)
         annotset = oras.oci.Annotations(kwargs.get("annotation_file"))
         media_type = None
 
+        refresh_headers = kwargs.get("refresh_headers")
+        if refresh_headers is None:
+            refresh_headers = True
+
         # Upload files as blobs
         for blob in kwargs.get("files", []):
             # You can provide a blob + content type
             path_content: PathAndOptionalContent = oras.utils.split_path_and_content(
                 str(blob)
             )
             blob = path_content.path
@@ -716,15 +757,17 @@
                 layer["annotations"].update(annotations)
 
             # update the manifest with the new layer
             manifest["layers"].append(layer)
             logger.debug(f"Preparing layer {layer}")
 
             # Upload the blob layer
-            response = self.upload_blob(blob, container, layer)
+            response = self.upload_blob(
+                blob, container, layer, refresh_headers=refresh_headers
+            )
             self._check_200_response(response)
 
             # Do we need to cleanup a temporary targz?
             if cleanup_blob and os.path.exists(blob):
                 os.remove(blob)
 
         # Add annotations to the manifest, if provided
@@ -758,21 +801,25 @@
         # Config is just another layer blob!
         logger.debug(f"Preparing config {conf}")
         with (
             temporary_empty_config()
             if config_file is None
             else nullcontext(config_file)
         ) as config_file:
-            response = self.upload_blob(config_file, container, conf)
+            response = self.upload_blob(
+                config_file, container, conf, refresh_headers=refresh_headers
+            )
 
         self._check_200_response(response)
 
         # Final upload of the manifest
         manifest["config"] = conf
-        self._check_200_response(self.upload_manifest(manifest, container))
+        self._check_200_response(
+            self.upload_manifest(manifest, container, refresh_headers=refresh_headers)
+        )
         print(f"Successfully pushed {container}")
         return response
 
     def pull(self, *args, **kwargs) -> List[str]:
         """
         Pull an artifact from a target
```

### Comparing `oras-0.1.28/oras/schemas.py` & `oras-0.1.29/oras/schemas.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/tests/conftest.py` & `oras-0.1.29/oras/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/tests/test_oras.py` & `oras-0.1.29/oras/tests/test_oras.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/tests/test_provider.py` & `oras-0.1.29/oras/tests/test_provider.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/tests/test_utils.py` & `oras-0.1.29/oras/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/utils/fileio.py` & `oras-0.1.29/oras/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/utils/request.py` & `oras-0.1.29/oras/utils/request.py`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/oras/version.py` & `oras-0.1.29/oras/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Vanessa Sochat"
 __copyright__ = "Copyright The ORAS Authors."
 __license__ = "Apache-2.0"
 
-__version__ = "0.1.28"
+__version__ = "0.1.29"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "oras"
 PACKAGE_URL = "https://github.com/oras-project/oras-py"
 KEYWORDS = "oci, registry, storage"
 DESCRIPTION = "OCI Registry as Storage Python SDK"
 LICENSE = "LICENSE"
```

### Comparing `oras-0.1.28/oras.egg-info/PKG-INFO` & `oras-0.1.29/oras.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oras
-Version: 0.1.28
+Version: 0.1.29
 Summary: OCI Registry as Storage Python SDK
 Home-page: https://github.com/oras-project/oras-py
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: oci,registry,storage
@@ -22,15 +22,15 @@
 Provides-Extra: tests
 Provides-Extra: docker
 License-File: LICENSE
 
 # ORAS Python
 
 <!-- ALL-CONTRIBUTORS-BADGE:START - Do not remove or modify this section -->
-[![All Contributors](https://img.shields.io/badge/all_contributors-18-orange.svg?style=flat-square)](#contributors-)
+[![All Contributors](https://img.shields.io/badge/all_contributors-19-orange.svg?style=flat-square)](#contributors-)
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 ![ORAS Logo](https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/oras.png)
 
 OCI Registry as Storage enables libraries to push OCI Artifacts to [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries. This is a Python SDK for Python developers to empower them to do this in their applications.
 
 See our ⭐️ [Documentation](https://oras-project.github.io/oras-py/) ⭐️ to get started.
@@ -71,14 +71,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://terryhowe.wordpress.com/"><img src="https://avatars.githubusercontent.com/u/104113?v=4?s=100" width="100px;" alt="Terry Howe"/><br /><sub><b>Terry Howe</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=TerryHowe" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://saketjajoo.github.io"><img src="https://avatars.githubusercontent.com/u/23132557?v=4?s=100" width="100px;" alt="Saket Jajoo"/><br /><sub><b>Saket Jajoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=saketjajoo" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/miker985"><img src="https://avatars.githubusercontent.com/u/26555712?v=4?s=100" width="100px;" alt="Mike"/><br /><sub><b>Mike</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=miker985" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/linshokaku"><img src="https://avatars.githubusercontent.com/u/18627646?v=4?s=100" width="100px;" alt="deoxy"/><br /><sub><b>deoxy</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=linshokaku" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kavish-p"><img src="https://avatars.githubusercontent.com/u/29086148?v=4?s=100" width="100px;" alt="Kavish Punchoo"/><br /><sub><b>Kavish Punchoo</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=kavish-p" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/my5cents"><img src="https://avatars.githubusercontent.com/u/4820203?v=4?s=100" width="100px;" alt="my5cents"/><br /><sub><b>my5cents</b></sub></a><br /><a href="https://github.com/oras-project/oras-py/commits?author=my5cents" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

#### html2text {}

```diff
@@ -1,40 +1,40 @@
-Metadata-Version: 2.1 Name: oras Version: 0.1.28 Summary: OCI Registry as
+Metadata-Version: 2.1 Name: oras Version: 0.1.29 Summary: OCI Registry as
 Storage Python SDK Home-page: https://github.com/oras-project/oras-py Author:
 Vanessa Sochat Author-email: vsoch@users.noreply.github.com Maintainer: Vanessa
 Sochat License: LICENSE Keywords: oci,registry,storage Classifier: Intended
 Audience :: Science/Research Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering Classifier: Operating System ::
 Unix Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Description-Content-Type: text/markdown
 Provides-Extra: all Provides-Extra: tests Provides-Extra: docker License-File:
 LICENSE # ORAS Python [![All Contributors](https://img.shields.io/badge/
-all_contributors-18-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
+all_contributors-19-orange.svg?style=flat-square)](#contributors-) ![ORAS Logo]
 (https://raw.githubusercontent.com/oras-project/oras-www/main/static/img/
 oras.png) OCI Registry as Storage enables libraries to push OCI Artifacts to
 [OCI Conformant](https://github.com/opencontainers/oci-conformance) registries.
 This is a Python SDK for Python developers to empower them to do this in their
 applications. See our â­ï¸ [Documentation](https://oras-project.github.io/
 oras-py/) â­ï¸ to get started. ## Code of Conduct Please note that this
 project has adopted the [CNCF Code of Conduct](https://github.com/cncf/
 foundation/blob/master/code-of-conduct.md). Please follow it in all your
 interactions with the project members and users. ## ðï¸ Contributors
 ðï¸ We use the [all-contributors](https://github.com/all-contributors/all-
 contributors) tool to generate a contributors graphic below.
-_[_V_a_n_e_s_s_a_s_a_u_r_u_s_] _[_L_a_c_h_l_a_n _[_S_t_e_v_e      _[_J_o_s_h     _[_B_r_i_d_g_e_t   _[_M_a_t_t      _[_W_o_l_f
- _VV_aa_nn_ee_ss_ss_aa_ss_aa_uu_rr_uu_ss  _E_v_e_n_s_o_n_] _L_a_s_k_e_r_]   _D_o_l_i_t_s_k_y_]   _K_r_o_m_h_o_u_t_] _W_a_r_n_e_r_]  _V_o_l_l_p_r_e_c_h_t_]
-     _ð___»       _LL_aa_cc_hh_ll_aa_nn   _SS_tt_ee_vv_ee  _JJ_oo_ss_hh_ _DD_oo_ll_ii_tt_ss_kk_yy  _BB_rr_ii_dd_gg_ee_tt    _MM_aa_tt_tt      _WW_oo_ll_ff
-                _EE_vv_ee_nn_ss_oo_nn  _LL_aa_ss_kk_ee_rr      _ð___»      _KK_rr_oo_mm_hh_oo_uu_tt   _WW_aa_rr_nn_ee_rr  _VV_oo_ll_ll_pp_rr_ee_cc_hh_tt
-                  _ð___»    _ð___»                   _ð___»      _ð___»      _ð___»
-_[_S_h_i_w_e_i_ _Z_h_a_n_g_]  _[_j_h_l_m_c_o_] _[_A_n_a_n_y_a _[_s_u_n_n_y_c_a_r_t_e_r_]  _[_M_a_r_i_u_s  _[_T_i_z_i_a_n_o   _[_T_e_r_r_y
- _SS_hh_ii_ww_ee_ii_ _ZZ_hh_aa_nn_gg    _jj_hh_ll_mm_cc_oo  _G_u_p_t_a_]   _ss_uu_nn_nn_yy_cc_aa_rr_tt_ee_rr  _B_e_r_t_r_a_m_]  _M_Ã_¼_l_l_e_r_]    _H_o_w_e_]
-     _ð___»         _ð___»   _AA_nn_aa_nn_yy_aa      _ð___»       _MM_aa_rr_ii_uu_ss   _TT_ii_zz_ii_aa_nn_oo  _TT_ee_rr_rr_yy_ _HH_oo_ww_ee
-                          _GG_uu_pp_tt_aa                 _BB_ee_rr_tt_rr_aa_mm  _MM_?Ã_?¼_ll_ll_ee_rr     _ð___»
-                          _ð___»                   _ð___»      _ð___»
- _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h
-  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]
-     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh
+_[_V_a_n_e_s_s_a_s_a_u_r_u_s_] _[_L_a_c_h_l_a_n _[_S_t_e_v_e      _[_J_o_s_h      _[_B_r_i_d_g_e_t   _[_M_a_t_t      _[_W_o_l_f
+ _VV_aa_nn_ee_ss_ss_aa_ss_aa_uu_rr_uu_ss  _E_v_e_n_s_o_n_] _L_a_s_k_e_r_]   _D_o_l_i_t_s_k_y_]   _K_r_o_m_h_o_u_t_]  _W_a_r_n_e_r_]  _V_o_l_l_p_r_e_c_h_t_]
+     _ð___»       _LL_aa_cc_hh_ll_aa_nn   _SS_tt_ee_vv_ee  _JJ_oo_ss_hh_ _DD_oo_ll_ii_tt_ss_kk_yy  _BB_rr_ii_dd_gg_ee_tt     _MM_aa_tt_tt      _WW_oo_ll_ff
+                _EE_vv_ee_nn_ss_oo_nn  _LL_aa_ss_kk_ee_rr      _ð___»       _KK_rr_oo_mm_hh_oo_uu_tt   _WW_aa_rr_nn_ee_rr  _VV_oo_ll_ll_pp_rr_ee_cc_hh_tt
+                  _ð___»    _ð___»                    _ð___»      _ð___»      _ð___»
+_[_S_h_i_w_e_i_ _Z_h_a_n_g_]  _[_j_h_l_m_c_o_] _[_A_n_a_n_y_a _[_s_u_n_n_y_c_a_r_t_e_r_]  _[_M_a_r_i_u_s   _[_T_i_z_i_a_n_o   _[_T_e_r_r_y
+ _SS_hh_ii_ww_ee_ii_ _ZZ_hh_aa_nn_gg    _jj_hh_ll_mm_cc_oo  _G_u_p_t_a_]   _ss_uu_nn_nn_yy_cc_aa_rr_tt_ee_rr   _B_e_r_t_r_a_m_]  _M_Ã_¼_l_l_e_r_]    _H_o_w_e_]
+     _ð___»         _ð___»   _AA_nn_aa_nn_yy_aa      _ð___»        _MM_aa_rr_ii_uu_ss   _TT_ii_zz_ii_aa_nn_oo  _TT_ee_rr_rr_yy_ _HH_oo_ww_ee
+                          _GG_uu_pp_tt_aa                 _BB_ee_rr_tt_rr_aa_mm   _MM_?Ã_?¼_ll_ll_ee_rr     _ð___»
+                          _ð___»                    _ð___»      _ð___»
+ _[_S_a_k_e_t_ _J_a_j_o_o_]   _[_M_i_k_e_]  _[_d_e_o_x_y_]     _[_K_a_v_i_s_h   _[_m_y_5_c_e_n_t_s_]
+  _SS_aa_kk_ee_tt_ _JJ_aa_jj_oo_oo     _MM_ii_kk_ee    _dd_ee_oo_xx_yy     _P_u_n_c_h_o_o_]    _mm_yy_55_cc_ee_nn_tt_ss
+     _ð___»         _ð___»    _ð___»       _KK_aa_vv_ii_ss_hh       _ð___»
                                      _PP_uu_nn_cc_hh_oo_oo
                                       _ð___»
 ## License This code is licensed under the Apache 2.0 [LICENSE](LICENSE).
```

### Comparing `oras-0.1.28/oras.egg-info/SOURCES.txt` & `oras-0.1.29/oras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oras-0.1.28/setup.py` & `oras-0.1.29/setup.py`

 * *Files identical despite different names*

