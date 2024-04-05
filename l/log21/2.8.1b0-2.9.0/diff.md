# Comparing `tmp/log21-2.8.1b0.tar.gz` & `tmp/log21-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log21-2.8.1b0.tar", last modified: Wed Mar 27 14:55:18 2024, max compression
+gzip compressed data, was "log21-2.9.0.tar", last modified: Fri Apr  5 21:16:03 2024, max compression
```

## Comparing `log21-2.8.1b0.tar` & `log21-2.9.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:55:18.930919 log21-2.8.1b0/
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2024-03-27 14:55:13.000000 log21-2.8.1b0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    16713 2024-03-27 14:55:18.930919 log21-2.8.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15413 2024-03-27 14:55:13.000000 log21-2.8.1b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-27 14:55:13.000000 log21-2.8.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 14:55:18.930919 log21-2.8.1b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:55:18.922919 log21-2.8.1b0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:55:18.926919 log21-2.8.1b0/src/log21/
--rw-r--r--   0 runner    (1001) docker     (127)    47574 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/Argparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    15229 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/Argumentify.py
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/Colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:55:18.930919 log21-2.8.1b0/src/log21/CrashReporter/
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/CrashReporter/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/CrashReporter/Reporters.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/CrashReporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/FileHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11632 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/Formatters.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/Levels.py
--rw-r--r--   0 runner    (1001) docker     (127)    11034 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/Logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    34385 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/LoggingWindow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/Manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    28854 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/PPrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15154 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/StreamHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9470 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/TreePrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    24135 2024-03-27 14:55:13.000000 log21-2.8.1b0/src/log21/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 14:55:18.930919 log21-2.8.1b0/src/log21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16713 2024-03-27 14:55:18.000000 log21-2.8.1b0/src/log21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-27 14:55:18.000000 log21-2.8.1b0/src/log21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 14:55:18.000000 log21-2.8.1b0/src/log21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-27 14:55:18.000000 log21-2.8.1b0/src/log21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-27 14:55:18.000000 log21-2.8.1b0/src/log21.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-05 21:16:03.811713 log21-2.9.0/
+-rw-rw-rw-   0        0        0    11552 2024-01-23 15:05:09.000000 log21-2.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     5103 2024-04-05 21:16:03.811713 log21-2.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3774 2024-04-05 21:07:28.000000 log21-2.9.0/README.md
+-rw-rw-rw-   0        0        0     1879 2024-04-05 21:07:28.000000 log21-2.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-05 21:16:03.812732 log21-2.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-05 21:16:03.627758 log21-2.9.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-05 21:16:03.752635 log21-2.9.0/src/log21/
+-rw-rw-rw-   0        0        0    48727 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/Argparse.py
+-rw-rw-rw-   0        0        0    15656 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/Argumentify.py
+-rw-rw-rw-   0        0        0    12155 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/Colors.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:16:03.808982 log21-2.9.0/src/log21/CrashReporter/
+-rw-rw-rw-   0        0        0     4140 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/CrashReporter/Formatters.py
+-rw-rw-rw-   0        0        0    15324 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/CrashReporter/Reporters.py
+-rw-rw-rw-   0        0        0      514 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/CrashReporter/__init__.py
+-rw-rw-rw-   0        0        0     1815 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/FileHandler.py
+-rw-rw-rw-   0        0        0    11925 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/Formatters.py
+-rw-rw-rw-   0        0        0      400 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/Levels.py
+-rw-rw-rw-   0        0        0    15374 2024-04-05 21:07:28.000000 log21-2.9.0/src/log21/Logger.py
+-rw-rw-rw-   0        0        0    35260 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/LoggingWindow.py
+-rw-rw-rw-   0        0        0     2138 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/Manager.py
+-rw-rw-rw-   0        0        0    29626 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/PPrint.py
+-rw-rw-rw-   0        0        0    15547 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/ProgressBar.py
+-rw-rw-rw-   0        0        0     8119 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/StreamHandler.py
+-rw-rw-rw-   0        0        0     9715 2024-01-23 15:05:09.000000 log21-2.9.0/src/log21/TreePrint.py
+-rw-rw-rw-   0        0        0    24662 2024-04-05 21:07:28.000000 log21-2.9.0/src/log21/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-05 21:16:03.810458 log21-2.9.0/src/log21.egg-info/
+-rw-rw-rw-   0        0        0     5103 2024-04-05 21:16:03.000000 log21-2.9.0/src/log21.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      632 2024-04-05 21:16:03.000000 log21-2.9.0/src/log21.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-05 21:16:03.000000 log21-2.9.0/src/log21.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2024-04-05 21:16:03.000000 log21-2.9.0/src/log21.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-05 21:16:03.000000 log21-2.9.0/src/log21.egg-info/top_level.txt
```

### Comparing `log21-2.8.1b0/LICENSE.txt` & `log21-2.9.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [2021-2024] [CodeWriter21]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [2021-2024] [CodeWriter21]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `log21-2.8.1b0/pyproject.toml` & `log21-2.9.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,71 @@
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "log21"
-authors = [
-  {name = "CodeWriter21(Mehrad Pooryoussof)", email = "CodeWriter21@gmail.com"}
-]
-description = "A simple logging package that helps you log colorized messages in Windows console."
-readme = {file = "README.md", content-type = "text/markdown"}
-requires-python = ">=3.8"
-keywords = ['python', 'log', 'colorize', 'color', 'logging', 'Python3', 'CodeWriter21']
-license = {text = "Apache License 2.0"}
-classifiers = [
-  "Intended Audience :: Developers",
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Operating System :: Unix",
-  "Operating System :: Microsoft :: Windows",
-  "Operating System :: MacOS :: MacOS X"
-]
-dependencies = [
-  "webcolors",
-  "docstring-parser"
-]
-version = "2.8.1b0"
-
-[tool.setuptools.packages.find]
-where = ["src"]
-
-[project.urls]
-Homepage = "https://github.com/MPCodeWriter21/log21"
-Donations = "https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md"
-Source = "https://github.com/MPCodeWriter21/log21"
-
-[project.optional-dependencies]
-dev = ["yapf", "isort", "docformatter", "pylint", "json5", "pytest"]
-
-[tool.pylint.messages_control]
-max-line-length = 88
-
-disable = [
-  "too-few-public-methods",
-  "too-many-arguments",
-  "protected-access",
-  "too-many-locals",
-  "fixme",
-]
-
-[tool.pylint.design]
-max-returns = 8
-
-[tool.yapf]
-column_limit = 88
-split_before_dot = true
-split_before_first_argument = true
-dedent_closing_brackets = true
-
-[tool.isort]
-line_length = 88
-combine_as_imports = true
-order_by_type = true
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "log21"
+authors = [
+  {name = "CodeWriter21(Mehrad Pooryoussof)", email = "CodeWriter21@gmail.com"}
+]
+description = "A simple logging package that helps you log colorized messages in Windows console."
+readme = {file = "README.md", content-type = "text/markdown"}
+requires-python = ">=3.8"
+keywords = ['python', 'log', 'colorize', 'color', 'logging', 'Python3', 'CodeWriter21']
+license = {text = "Apache License 2.0"}
+classifiers = [
+  "Intended Audience :: Developers",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.7",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Operating System :: Unix",
+  "Operating System :: Microsoft :: Windows",
+  "Operating System :: MacOS :: MacOS X"
+]
+dependencies = [
+  "webcolors",
+  "docstring-parser"
+]
+version = "2.9.0"
+
+[tool.setuptools.packages.find]
+where = ["src"]
+
+[project.urls]
+Homepage = "https://github.com/MPCodeWriter21/log21"
+Donations = "https://github.com/MPCodeWriter21/log21/blob/master/DONATE.md"
+Source = "https://github.com/MPCodeWriter21/log21"
+
+[project.optional-dependencies]
+dev = ["yapf", "isort", "docformatter", "pylint", "json5", "pytest"]
+
+[tool.pylint.messages_control]
+max-line-length = 88
+
+disable = [
+  "too-few-public-methods",
+  "too-many-arguments",
+  "protected-access",
+  "too-many-locals",
+  "fixme",
+]
+
+[tool.pylint.design]
+max-returns = 8
+
+[tool.yapf]
+column_limit = 88
+split_before_dot = true
+split_before_first_argument = true
+dedent_closing_brackets = true
+
+[tool.isort]
+line_length = 88
+combine_as_imports = true
+length_sort = true
+order_by_type = true
+
+[tool.docformatter]
+recursive = true
+wrap-summaries = 88
+wrap-descriptions = 88
```

### Comparing `log21-2.8.1b0/src/log21/Argparse.py` & `log21-2.9.0/src/log21/Argparse.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,1153 +1,1153 @@
-# log21.Argparse.py
-# CodeWriter21
-
-from __future__ import annotations
-
-import re as _re
-import sys as _sys
-import types as _types
-import typing as _typing
-import argparse as _argparse
-from enum import Enum as _Enum
-from typing import (Tuple as _Tuple, Mapping as _Mapping, Optional as _Optional,
-                    Sequence as _Sequence)
-from gettext import gettext as _gettext
-from textwrap import TextWrapper as _TextWrapper
-from collections import OrderedDict as _OrderedDict
-
-import log21 as _log21
-from log21.Colors import get_colors as _gc
-from log21.Formatters import DecolorizingFormatter as _Formatter
-
-__all__ = [
-    'ColorizingArgumentParser', 'ColorizingHelpFormatter', 'ColorizingTextWrapper',
-    'Literal'
-]
-
-
-class Literal:
-    """A class for representing literals in argparse arguments."""
-
-    def __init__(self, literal: _typing._LiteralGenericAlias):
-        self.literal = literal
-        # Only str arguments are allowed
-        if not all(map(lambda x: isinstance(x, str), self.literal.__args__)):
-            raise TypeError('Only str arguments are allowed for Literal.')
-
-    def __repr__(self):
-        return f'Literal[{", ".join(map(str, self.literal.__args__))}]'
-
-    def __str__(self):
-        return self.__repr__()
-
-    def __call__(self, value):
-        if value not in self.literal.__args__:
-            raise ValueError(
-                f'Value must be one of [{", ".join(map(str, self.literal.__args__))}]'
-            )
-        return value
-
-
-class ColorizingHelpFormatter(_argparse.HelpFormatter):
-    """A help formatter that supports colorizing help messages."""
-
-    def __init__(
-        self,
-        prog,
-        indent_increment=2,
-        max_help_position=24,
-        width=None,
-        colors: _Optional[_Mapping[str, str]] = None
-    ):
-        super().__init__(prog, indent_increment, max_help_position, width)
-
-        self.colors = {
-            'usage': 'Cyan',
-            'brackets': 'LightRed',
-            'switches': 'LightCyan',
-            'values': 'Green',
-            'colons': 'LightRed',
-            'commas': 'LightRed',
-            'section headers': 'LightGreen',
-            'help': 'LightWhite',
-            'choices': 'LightGreen'
-        }
-
-        if colors:
-            for key, value in colors.items():
-                if key in self.colors:
-                    self.colors[key] = value
-
-    class _Section(object):
-
-        def __init__(self, formatter, parent, heading=None):
-            self.formatter = formatter
-            self.parent = parent
-            self.heading = heading
-            self.items = []
-
-        def format_help(self):
-            # format the indented section
-            if self.parent is not None:
-                self.formatter._indent()
-            join = self.formatter._join_parts
-            item_help = join([func(*args) for func, args in self.items])
-            if self.parent is not None:
-                self.formatter._dedent()
-
-            # return nothing if the section was empty
-            if not item_help:
-                return ''
-
-            # add the heading if the section was non-empty
-            if self.heading is not _argparse.SUPPRESS and self.heading is not None:
-                current_indent = self.formatter._current_indent
-                heading = (
-                    '%*s%s' % (current_indent, '', self.heading) +
-                    _gc(self.formatter.colors['colons']) + ':\033[0m\n'
-                )
-            else:
-                heading = ''
-
-            # join the section-initial newline, the heading and the help
-            return join(
-                ['\n', heading,
-                 _gc(self.formatter.colors['help']), item_help, '\n']
-            )
-
-    def _add_item(self, func, args):
-        self._current_section.items.append((func, args))
-
-    def _fill_text(self, text, width, indent):
-        text = self._whitespace_matcher.sub(' ', text).strip()
-        return ColorizingTextWrapper(
-            width=width, initial_indent=indent, subsequent_indent=indent
-        ).fill(text)
-
-    def _split_lines(self, text, width):
-        text = self._whitespace_matcher.sub(' ', text).strip()
-        return ColorizingTextWrapper(width=width).wrap(text)
-
-    def start_section(self, heading):
-        self._indent()
-        section = self._Section(
-            self, self._current_section,
-            _gc(self.colors['section headers']) + str(heading) + '\033[0m'
-        )
-        self._add_item(section.format_help, [])
-        self._current_section = section
-
-    def _format_action(self, action):
-        # determine the required width and the entry label
-        help_position = min(self._action_max_length + 2, self._max_help_position)
-        help_width = max(self._width - help_position, 11)
-        action_width = help_position - self._current_indent - 2
-        action_header = _gc('rst') + self._format_action_invocation(action)
-
-        indent_first = 0
-        # no help; start on same line and add a final newline
-        if not action.help:
-            action_header = self._current_indent * ' ' + action_header + '\n'
-        # short action name; start on the same line and pad two spaces
-        elif len(action_header) <= action_width:
-            action_header = '%*s%-*s  ' % (
-                self._current_indent, '', action_width, action_header
-            )
-        # long action name; start on the next line
-        else:
-            action_header = self._current_indent * ' ' + action_header + '\n'
-            indent_first = help_position
-
-        # collect the pieces of the action help
-        parts = [action_header]
-
-        # if there was help for the action, add lines of help text
-        if action.help:
-            help_text = _gc(self.colors['help']) + self._expand_help(action)
-            help_lines = self._split_lines(help_text, help_width)
-            parts.append('%*s%s\n' % (indent_first, '', help_lines[0]))
-            for line in help_lines[1:]:
-                parts.append('%*s%s\n' % (help_position, '', line))
-
-        # or add a newline if the description doesn't end with one
-        elif not action_header.endswith('\n'):
-            parts.append('\n')
-
-        # if there are any sub-actions, add their help as well
-        for subaction in self._iter_indented_subactions(action):
-            parts.append(self._format_action(subaction))
-
-        # return a single string
-        return self._join_parts(parts)
-
-    # modified upstream code, not going to refactor for complexity.
-    def _format_usage(self, usage, actions, groups, prefix):  # noqa: C901
-        if prefix is None:
-            prefix = _gettext('usage: ')
-
-        # if usage is specified, use that
-        if usage is not None:
-            usage = usage % dict(prog=self._prog)
-
-        # if no optionals or positionals are available, usage is just prog
-        elif usage is None and not actions:
-            usage = '%(prog)s' % dict(prog=self._prog)
-
-        # if optionals and positionals are available, calculate usage
-        elif usage is None:
-            prog = '%(prog)s' % dict(prog=self._prog)
-
-            # split optionals from positionals
-            optionals = []
-            positionals = []
-            for action in actions:
-                if action.option_strings:
-                    optionals.append(action)
-                else:
-                    positionals.append(action)
-
-            # build full usage string
-            action_usage = self._format_actions_usage(optionals + positionals, groups)
-            usage = ' '.join([s for s in [prog, action_usage] if s])
-
-            # wrap the usage parts if it's too long
-            text_width = self._width - self._current_indent
-            if len(prefix) + len(_Formatter.decolorize(usage)) > text_width:
-
-                # break usage into wrappable parts
-                part_regexp = r'\(.*?\)+|\[.*?\]+|\S+'
-                opt_usage = self._format_actions_usage(optionals, groups)
-                pos_usage = self._format_actions_usage(positionals, groups)
-                opt_parts = _re.findall(part_regexp, opt_usage)
-                pos_parts = _re.findall(part_regexp, pos_usage)
-                assert ' '.join(opt_parts) == opt_usage
-                assert ' '.join(pos_parts) == pos_usage
-
-                # helper for wrapping lines
-                def get_lines(parts, indent, prefix=None):
-                    lines = []
-                    line = []
-                    if prefix is not None:
-                        line_len = len(prefix) - 1
-                    else:
-                        line_len = len(indent) - 1
-                    for part in parts:
-                        if line_len + 1 + len(_Formatter.decolorize(part)
-                                              ) > text_width and line:
-                            lines.append(indent + ' '.join(line))
-                            line = []
-                            line_len = len(indent) - 1
-                        line.append(part)
-                        line_len += len(_Formatter.decolorize(part)) + 1
-                    if line:
-                        lines.append(indent + ' '.join(line))
-                    if prefix is not None:
-                        lines[0] = lines[0][len(indent):]
-                    return lines
-
-                # if prog is short, follow it with optionals or positionals
-                len_prog = len(_Formatter.decolorize(prog))
-                if len(prefix) + len_prog <= 0.75 * text_width:
-                    indent = ' ' * (len(prefix) + len_prog + 1)
-                    if opt_parts:
-                        lines = get_lines([prog] + opt_parts, indent, prefix)
-                        lines.extend(get_lines(pos_parts, indent))
-                    elif pos_parts:
-                        lines = get_lines([prog] + pos_parts, indent, prefix)
-                    else:
-                        lines = [prog]
-
-                # if prog is long, put it on its own line
-                else:
-                    indent = ' ' * len(prefix)
-                    parts = opt_parts + pos_parts
-                    lines = get_lines(parts, indent)
-                    if len(lines) > 1:
-                        lines = []
-                        lines.extend(get_lines(opt_parts, indent))
-                        lines.extend(get_lines(pos_parts, indent))
-                    lines = [prog] + lines
-
-                # join lines into usage
-                usage = '\n'.join(lines)
-
-        # prefix with 'usage:'
-        return prefix + usage + '\n\n'
-
-    def _format_actions_usage(self, actions: list, groups):
-        # find group indices and identify actions in groups
-        group_actions = set()
-        inserts = {}
-        for group in groups:
-            try:
-                start = actions.index(group._group_actions[0])
-            except ValueError:
-                continue
-            else:
-                end = start + len(group._group_actions)
-                if actions[start:end] == group._group_actions:
-                    for action in group._group_actions:
-                        group_actions.add(action)
-                    if not group.required:
-                        if start in inserts:
-                            inserts[start] += ' ['
-                        else:
-                            inserts[start] = '['
-                        if end in inserts:
-                            inserts[end] += ']'
-                        else:
-                            inserts[end] = ']'
-                    else:
-                        if start in inserts:
-                            inserts[start] += ' ('
-                        else:
-                            inserts[start] = '('
-                        if end in inserts:
-                            inserts[end] += ')'
-                        else:
-                            inserts[end] = ')'
-                    for i in range(start + 1, end):
-                        inserts[i] = '|'
-
-        # collect all actions format strings
-        parts = []
-        for i, action in enumerate(actions):
-
-            # suppressed arguments are marked with None
-            # remove | separators for suppressed arguments
-            if action.help is _argparse.SUPPRESS:
-                parts.append(None)
-                if inserts.get(i) == '|':
-                    inserts.pop(i)
-                elif inserts.get(i + 1) == '|':
-                    inserts.pop(i + 1)
-
-            # produce all arg strings
-            elif not action.option_strings:
-                default = self._get_default_metavar_for_positional(action)
-                part = self._format_args(action, default)
-
-                # if it's in a group, strip the outer []
-                if action in group_actions:
-                    if part[0] == '[' and part[-1] == ']':
-                        part = part[1:-1]
-
-                # add the action string to the list
-                parts.append(part)
-
-            # produce the first way to invoke the option in brackets
-            else:
-                option_string = action.option_strings[0]
-
-                # if the Optional doesn't take a value, format is:
-                #    -s or --long
-                if action.nargs == 0:
-                    part = _gc(self.colors['switches']) + action.format_usage()
-
-                # if the Optional takes a value, format is:
-                #    -s ARGS or --long ARGS
-                else:
-                    default = self._get_default_metavar_for_optional(action)
-                    args_string = self._format_args(action, default)
-                    part = _gc(self.colors['switches']) + '%s %s%s' % (
-                        option_string, _gc(self.colors['values']), args_string
-                    )
-
-                # make it look optional if it's not required or in a group
-                if not action.required and action not in group_actions:
-                    part = _gc(self.colors['brackets']) + '[' + part + _gc(
-                        self.colors['brackets']
-                    ) + ']\033[0m'
-
-                # add the action string to the list
-                parts.append(part)
-
-        # insert things at the necessary indices
-        for i in sorted(inserts, reverse=True):
-            parts[i:i] = [inserts[i]]
-
-        # join all the action items with spaces
-        text = ' '.join([item for item in parts if item is not None])
-
-        # clean up separators for mutually exclusive groups
-        open = r'[\[(]'
-        close = r'[\])]'
-        text = _re.sub(r'(%s) ' % open, r'\1', text)
-        text = _re.sub(r' (%s)' % close, r'\1', text)
-        text = _re.sub(r'%s *%s' % (open, close), r'', text)
-        text = _re.sub(r'\(([^|]*)\)', r'\1', text)
-        text = text.strip()
-
-        # return the text
-        return text
-
-    def _format_action_invocation(self, action):
-        if not action.option_strings:
-            default = self._get_default_metavar_for_positional(action)
-            metavar, = self._metavar_formatter(action, default)(1)
-            return metavar
-
-        else:
-            parts = []
-
-            # if the Optional doesn't take a value, format is:
-            #    -s, --long
-            if action.nargs == 0:
-                for option_string in action.option_strings:
-                    parts.append(_gc(self.colors['switches']) + option_string)
-
-            # if the Optional takes a value, format is:
-            #    -s ARGS, --long ARGS
-            else:
-                default = self._get_default_metavar_for_optional(action)
-                args_string = self._format_args(action, default)
-                for option_string in action.option_strings:
-                    parts.append(
-                        _gc(self.colors['switches']) + '%s %s%s' %
-                        (option_string, _gc(self.colors['values']), args_string)
-                    )
-
-            return _gc(self.colors['commas']) + ', '.join(parts)
-
-    def _metavar_formatter(self, action, default_metavar):
-        if action.metavar is not None:
-            result = action.metavar
-        elif action.choices is not None:
-            choice_strs = [str(choice) for choice in action.choices]
-            result = (
-                _gc(self.colors['brackets']) + '{ ' +
-                (_gc(self.colors['commas']) + ', ').join(
-                    _gc(self.colors['choices']) + choice_str
-                    for choice_str in choice_strs
-                ) + _gc(self.colors['brackets']) + ' }'
-            )
-        else:
-            result = default_metavar
-
-        def format(tuple_size):
-            if isinstance(result, tuple):
-                return result
-            else:
-                return (result, ) * tuple_size
-
-        return format
-
-
-class ColorizingTextWrapper(_TextWrapper):
-    # modified upstream code, not going to refactor for complexity.
-    def _wrap_chunks(self, chunks):  # noqa: C901
-        """_wrap_chunks(chunks : [string]) -> [string]
-
-        Wrap a sequence of text chunks and return a list of lines of
-        length 'self.width' or less.  (If 'break_long_words' is false,
-        some lines may be longer than this.)  Chunks correspond roughly
-        to words and the whitespace between them: each chunk is
-        indivisible (modulo 'break_long_words'), but a line break can
-        come between any two chunks.  Chunks should not have internal
-        whitespace; i.e. a chunk is either all whitespace or a "word".
-        Whitespace chunks will be removed from the beginning and end of
-        lines, but apart from that whitespace is preserved.
-        """
-        lines = []
-        if self.width <= 0:
-            raise ValueError("invalid width %r (must be > 0)" % self.width)
-        if self.max_lines is not None:
-            if self.max_lines > 1:
-                indent = self.subsequent_indent
-            else:
-                indent = self.initial_indent
-            if len(indent) + len(self.placeholder.lstrip()) > self.width:
-                raise ValueError("placeholder too large for max width")
-
-        # Arrange in reverse order so items can be efficiently popped
-        # from a stack of chucks.
-        chunks.reverse()
-
-        while chunks:
-
-            # Start the list of chunks that will make up the current line.
-            # current_len is just the length of all the chunks in current_line.
-            current_line = []
-            current_len = 0
-
-            # Figure out which static string will prefix this line.
-            if lines:
-                indent = self.subsequent_indent
-            else:
-                indent = self.initial_indent
-
-            # Maximum width for this line.
-            width = self.width - len(indent)
-
-            # First chunk on the line is whitespace -- drop it, unless this
-            # is the very beginning of the text (i.e. no lines started yet).
-            if self.drop_whitespace and _Formatter.decolorize(chunks[-1]
-                                                              ).strip() == '' and lines:
-                del chunks[-1]
-
-            while chunks:
-                # modified upstream code, not going to refactor for ambiguous variable
-                # name.
-                length = len(_Formatter.decolorize(chunks[-1]))  # noqa: E741
-
-                # Can at least squeeze this chunk onto the current line.
-                # Modified upstream code, not going to refactor for ambiguous variable
-                # name.
-                if current_len + length <= width:  # noqa: E741
-                    current_line.append(chunks.pop())
-                    current_len += length
-                # Nope, this line is full.
-                else:
-                    break
-
-            # The current line is full, and the next chunk is too big to
-            # fit on *any* line (not just this one).
-            if chunks and len(_Formatter.decolorize(chunks[-1])) > width:
-                self._handle_long_word(chunks, current_line, current_len, width)
-                current_len = sum(map(len, current_line))
-
-            # If the last chunk on this line is all whitespace, drop it.
-            if self.drop_whitespace and current_line and _Formatter.decolorize(
-                    current_line[-1]).strip() == '':
-                current_len -= len(_Formatter.decolorize(current_line[-1]))
-                del current_line[-1]
-
-            if current_line:
-                if (self.max_lines is None or len(lines) + 1 < self.max_lines
-                        or (not chunks or self.drop_whitespace and len(chunks) == 1
-                            and not chunks[0].strip()) and current_len <= width):
-                    # Convert current line back to a string and store it in
-                    # list of all lines (return value).
-                    lines.append(indent + ''.join(current_line))
-                else:
-                    while current_line:
-                        if _Formatter.decolorize(
-                                current_line[-1]
-                        ).strip() and current_len + len(self.placeholder) <= width:
-                            current_line.append(self.placeholder)
-                            lines.append(indent + ''.join(current_line))
-                            break
-                        current_len -= len(_Formatter.decolorize(current_line[-1]))
-                        del current_line[-1]
-                    else:
-                        if lines:
-                            prev_line = lines[-1].rstrip()
-                            if len(_Formatter.decolorize(prev_line)) + len(
-                                    self.placeholder) <= self.width:
-                                lines[-1] = prev_line + self.placeholder
-                                break
-                        lines.append(indent + self.placeholder.lstrip())
-                    break
-
-        return lines
-
-
-class _ActionsContainer(_argparse._ActionsContainer):
-    """Container for the actions for a single command line option."""
-
-    # pylint: disable=too-many-branches
-    def _validate_func_type(self, action, func_type, kwargs, level: int = 0) -> _Tuple:
-        # raise an error if the action type is not callable
-        if (hasattr(_types, 'UnionType') and not callable(func_type)
-                and not isinstance(func_type, (_types.UnionType, tuple))):
-            raise ValueError(f'{func_type} is not callable; level={level}')
-
-        # Handle `UnionType` as a type (e.g. `int|str`)
-        if hasattr(_types, 'UnionType') and isinstance(func_type, _types.UnionType):
-            func_type = func_type.__args__  # type: ignore
-
-        # Handle `Literal` as a type (e.g. `Literal[1, 2, 3]`)
-        elif (hasattr(_typing, '_LiteralGenericAlias')
-              and isinstance(func_type, _typing._LiteralGenericAlias)):  # type: ignore
-            func_type = Literal(func_type)
-
-        # Handle `List` as a type (e.g. `List[int]`)
-        elif (hasattr(_typing, '_GenericAlias')
-              and isinstance(func_type, _typing._GenericAlias)  # type: ignore
-              and func_type.__origin__ is list):
-            func_type = func_type.__args__[0]
-            if kwargs.get('nargs') is None:
-                action.nargs = '+'
-
-        # Handle `Required` as a type (e.g. `Required[int]`)
-        elif (hasattr(_typing, 'Required') and hasattr(_typing, '_GenericAlias')
-              and isinstance(func_type, _typing._GenericAlias)  # type: ignore
-              and func_type.__origin__ is _typing.Required
-              ):
-            func_type = func_type.__args__[0]
-            action.required = True
-
-        # Handle `Union` and `Optional` as a type (e.g. `Union[int, str]` and
-        # `Optional[int]`)
-        elif (hasattr(_types, 'NoneType') and hasattr(_typing, '_UnionGenericAlias')
-              and isinstance(func_type, _typing._UnionGenericAlias)):  # type: ignore
-            # Optional[T] is just Union[T, NoneType]
-            # Optional
-            if (len(func_type.__args__) == 2
-                    and func_type.__args__[1] is _types.NoneType):
-                action.required = False
-                func_type = func_type.__args__[0]
-            # Union
-            else:
-                func_type = func_type.__args__  # type: ignore
-
-        # Handle Enum as a type
-        elif callable(func_type) and isinstance(func_type, type) and issubclass(
-                func_type, _Enum) and action.choices is None and level == 0:
-            action.choices = tuple(
-                map(lambda x: x.value, func_type.__members__.values())
-            )
-
-        # Handle SpecialForms
-        elif isinstance(func_type, _typing._SpecialForm):
-            if func_type is _typing.Any:
-                func_type = None
-            elif func_type is _typing.ClassVar:
-                func_type = None
-            elif func_type is _typing.Union:
-                func_type = None
-            elif func_type is _typing.Optional:
-                func_type = None
-                action.required = False
-            elif func_type is _typing.Type:
-                func_type = None
-            elif func_type is _typing.TypeVar:
-                func_type = None
-            else:
-                raise ValueError(f'Unknown special form {func_type}')
-
-        elif func_type is _argparse.FileType:
-            raise ValueError(
-                f'{func_type} is a FileType class object, instance of it must be passed'
-            )
-
-        if isinstance(func_type, _Sequence):
-            temp = []
-            for type_ in _OrderedDict(zip(func_type, [0] * len(func_type))):
-                temp.extend(self._validate_func_type(action, type_, kwargs, level + 1))
-            func_type = tuple(temp)
-        else:
-            if (hasattr(_types, 'UnionType') and hasattr(_typing, '_GenericAlias')
-                    and hasattr(_typing, '_UnionGenericAlias')
-                    and hasattr(_typing, '_LiteralGenericAlias') and isinstance(
-                        func_type,
-                        (
-                            _typing._GenericAlias,  # type: ignore
-                            _typing._UnionGenericAlias,  # type: ignore
-                            _typing._LiteralGenericAlias,  # type: ignore
-                            _types.UnionType,
-                        ))):
-                func_type = self._validate_func_type(
-                    action, func_type, kwargs, level + 1
-                )
-            else:
-                func_type = (func_type, )
-
-        return func_type
-
-    # Override the default add_argument method defined in argparse._ActionsContainer
-    # to add the support for different type annotations
-    def add_argument(self, *args, **kwargs):
-        """Add an argument to the parser.
-
-        Signature:
-            add_argument(dest, ..., name=value, ...)
-            add_argument(option_string, option_string, ..., name=value, ...)
-        """
-
-        # if no positional args are supplied or only one is supplied and
-        # it doesn't look like an option string, parse a positional
-        # argument
-        chars = self.prefix_chars
-        if not args or len(args) == 1 and args[0][0] not in chars:
-            if args and 'dest' in kwargs:
-                raise ValueError('dest supplied twice for positional argument')
-            kwargs = self._get_positional_kwargs(*args, **kwargs)
-
-        # otherwise, we're adding an optional argument
-        else:
-            kwargs = self._get_optional_kwargs(*args, **kwargs)
-
-        # if no default was supplied, use the parser-level default
-        if 'default' not in kwargs:
-            dest = kwargs['dest']
-            if dest in self._defaults:
-                kwargs['default'] = self._defaults[dest]
-            elif self.argument_default is not None:
-                kwargs['default'] = self.argument_default
-
-        # create the action object, and add it to the parser
-        action_class = self._pop_action_class(kwargs)
-        if not callable(action_class):
-            raise ValueError(f'unknown action "{action_class}"')
-        action = action_class(**kwargs)
-
-        func_type = self._registry_get('type', action.type, action.type)
-        action.type = self._validate_func_type(
-            action, func_type, kwargs
-        )  # type: ignore
-        if len(action.type) == 1:
-            action.type = action.type[0]
-        elif len(action.type) == 0:
-            action.type = None
-
-        # raise an error if the metavar does not match the type
-        if hasattr(self, "_get_formatter"):
-            try:
-                self._get_formatter()._format_args(action, None)
-            except TypeError:
-                raise ValueError(
-                    "length of metavar tuple does not match nargs"
-                ) from None
-
-        return self._add_action(action)
-
-    def add_argument_group(self, *args, **kwargs):
-        group = _ArgumentGroup(self, *args, **kwargs)
-        self._action_groups.append(group)
-        return group
-
-    def add_mutually_exclusive_group(self, **kwargs):
-        group = _MutuallyExclusiveGroup(self, **kwargs)
-        self._mutually_exclusive_groups.append(group)
-        return group
-
-
-class ColorizingArgumentParser(_argparse.ArgumentParser, _ActionsContainer):
-    """An ArgumentParser that colorizes its output and more."""
-
-    def __init__(
-        self,
-        formatter_class=ColorizingHelpFormatter,
-        colors: _Optional[_Mapping[str, str]] = None,
-        **kwargs
-    ):
-        self.logger = _log21.Logger('ArgumentParser')
-        self.colors = colors
-        super().__init__(formatter_class=formatter_class, **kwargs)
-
-    def _print_message(self, message, file=None):
-        if message:
-            self.logger.handlers.clear()
-            handler = _log21.ColorizingStreamHandler(stream=file)
-            self.logger.addHandler(handler)
-            self.logger.info(message + _gc('rst'))
-
-    def exit(self, status=0, message=None):
-        if message:
-            self._print_message(_gc('lr') + message + _gc('rst'), _sys.stderr)
-        _sys.exit(status)
-
-    def error(self, message):
-        self.print_usage(_sys.stderr)
-        args = {'prog': self.prog, 'message': message}
-        self.exit(
-            2,
-            _gettext(
-                f'%(prog)s: {_gc("r")}error{_gc("lr")}:{_gc("rst")} %(message)s\n'
-            ) % args
-        )
-
-    def _get_formatter(self):
-        if hasattr(self.formatter_class, 'colors'):
-            return self.formatter_class(prog=self.prog, colors=self.colors)
-        else:
-            return self.formatter_class(prog=self.prog)
-
-    def _get_value(self, action, arg_string):
-        """Override _get_value to add support for types such as Union and
-        Literal."""
-
-        func_type = self._registry_get('type', action.type, action.type)
-        if not callable(func_type) and not isinstance(func_type, tuple):
-            raise _argparse.ArgumentError(
-                action, _gettext(f'{func_type!r} is not callable')
-            )
-
-        name = getattr(action.type, '__name__', repr(action.type))
-
-        # convert the value to the appropriate type
-        try:
-            if callable(func_type):
-                result = func_type(arg_string)
-            else:
-                exception = ValueError()
-                for type_ in func_type:
-                    name = getattr(type_, '__name__', repr(type_))
-                    try:
-                        result = type_(arg_string)
-                        break
-                    except (ValueError, TypeError) as ex:
-                        exception = ex
-                else:
-                    raise exception
-
-        # ArgumentTypeErrors indicate errors
-        except _argparse.ArgumentTypeError as ex:
-            msg = str(ex)
-            raise _argparse.ArgumentError(action, msg)
-
-        # TypeErrors or ValueErrors also indicate errors
-        except (TypeError, ValueError):
-            raise _argparse.ArgumentError(
-                action, _gettext(f'invalid {name!s} value: {arg_string!r}')
-            ) from None
-
-        # return the converted value
-        return result
-
-    def __convert_type(self, func_type, arg_string):
-        result = None
-        if callable(func_type):
-            try:
-                result = func_type(arg_string)
-            except Exception:
-                pass
-        else:
-            for type_ in func_type:
-                try:
-                    result = type_(arg_string)
-                    break
-                except Exception:
-                    pass
-
-        return result
-
-    def _check_value(self, action, choice):
-        # converted value must be one of the choices (if specified)
-        if action.choices is not None:
-            choices = set(action.choices)
-
-            func_type = self._registry_get('type', action.type, action.type)
-            if not callable(func_type) and not isinstance(func_type, tuple):
-                raise _argparse.ArgumentError(
-                    action, _gettext(f'{func_type!r} is not callable')
-                )
-
-            for value in action.choices:
-                choices.add(self.__convert_type(func_type, value))
-
-            if choice not in choices:
-                raise _argparse.ArgumentError(
-                    action,
-                    _gettext(
-                        f'invalid choice: {choice!r} '
-                        f'(choose from {", ".join(map(repr, action.choices))})'
-                    )
-                )
-
-    def _read_args_from_files(self, arg_strings):
-        # expand arguments referencing files
-        new_arg_strings = []
-        for arg_string in arg_strings:
-
-            # for regular arguments, just add them back into the list
-            if not arg_string or arg_string[0] not in self.fromfile_prefix_chars:
-                new_arg_strings.append(arg_string)
-
-            # replace arguments referencing files with the file content
-            else:
-                try:
-                    with open(arg_string[1:]) as args_file:
-                        arg_strings = []
-                        for arg_line in args_file.read().splitlines():
-                            for arg in self.convert_arg_line_to_args(arg_line):
-                                arg_strings.append(arg)
-                        arg_strings = self._read_args_from_files(arg_strings)
-                        new_arg_strings.extend(arg_strings)
-                except OSError as err:
-                    self.error(str(err))
-
-        # return the modified argument list
-        return new_arg_strings
-
-    def _parse_known_args(self, arg_strings, namespace):
-        # replace arg strings that are file references
-        if self.fromfile_prefix_chars is not None:
-            arg_strings = self._read_args_from_files(arg_strings)
-
-        # map all mutually exclusive arguments to the other arguments
-        # they can't occur with
-        action_conflicts = {}
-        for mutex_group in self._mutually_exclusive_groups:
-            group_actions = mutex_group._group_actions
-            for i, mutex_action in enumerate(mutex_group._group_actions):
-                conflicts = action_conflicts.setdefault(mutex_action, [])
-                conflicts.extend(group_actions[:i])
-                conflicts.extend(group_actions[i + 1:])
-
-        # find all option indices, and determine the arg_string_pattern
-        # which has an 'O' if there is an option at an index,
-        # an 'A' if there is an argument, or a '-' if there is a '--'
-        option_string_indices = {}
-        arg_string_pattern_parts = []
-        arg_strings_iter = iter(arg_strings)
-        for i, arg_string in enumerate(arg_strings_iter):
-
-            # all args after -- are non-options
-            if arg_string == '--':
-                arg_string_pattern_parts.append('-')
-                for arg_string in arg_strings_iter:
-                    arg_string_pattern_parts.append('A')
-
-            # otherwise, add the arg to the arg strings
-            # and note the index if it was an option
-            else:
-                option_tuple = self._parse_optional(arg_string)
-                if option_tuple is None:
-                    pattern = 'A'
-                else:
-                    option_string_indices[i] = option_tuple
-                    pattern = 'O'
-                arg_string_pattern_parts.append(pattern)
-
-        # join the pieces together to form the pattern
-        arg_strings_pattern = ''.join(arg_string_pattern_parts)
-
-        # converts arg strings to the appropriate and then takes the action
-        seen_actions = set()
-        seen_non_default_actions = set()
-
-        def take_action(action, argument_strings, option_string=None):
-            seen_actions.add(action)
-            argument_values = self._get_values(action, argument_strings)
-
-            # error if this argument is not allowed with other previously
-            # seen arguments, assuming that actions that use the default
-            # value don't really count as "present"
-            if argument_values is not action.default:
-                seen_non_default_actions.add(action)
-                for conflict_action in action_conflicts.get(action, []):
-                    if conflict_action in seen_non_default_actions:
-                        action_name = _argparse._get_action_name(conflict_action)
-                        msg = _gettext(f'not allowed with argument {action_name}')
-                        raise _argparse.ArgumentError(action, msg)
-
-            # take the action if we didn't receive a SUPPRESS value
-            # (e.g. from a default)
-            if argument_values is not _argparse.SUPPRESS:
-                action(self, namespace, argument_values, option_string)
-
-        # function to convert arg_strings into an optional action
-        def consume_optional(start_index):
-
-            # get the optional identified at this index
-            option_tuple = option_string_indices[start_index]
-            action, option_string, explicit_arg = option_tuple
-
-            # identify additional optionals in the same arg string
-            # (e.g. -xyz is the same as -x -y -z if no args are required)
-            match_argument = self._match_argument
-            action_tuples = []
-            while True:
-
-                # if we found no optional action, skip it
-                if action is None:
-                    extras.append(arg_strings[start_index])
-                    return start_index + 1
-
-                # if there is an explicit argument, try to match the
-                # optional's string arguments to only this
-                if explicit_arg is not None:
-                    arg_count = match_argument(action, 'A')
-
-                    # if the action is a single-dash option and takes no
-                    # arguments, try to parse more single-dash options out
-                    # of the tail of the option string
-                    chars = self.prefix_chars
-                    if arg_count == 0 and option_string[1] not in chars:
-                        action_tuples.append((action, [], option_string))
-                        char = option_string[0]
-                        option_string = char + explicit_arg[0]
-                        new_explicit_arg = explicit_arg[1:] or None
-                        optionals_map = self._option_string_actions
-                        if option_string in optionals_map:
-                            action = optionals_map[option_string]
-                            explicit_arg = new_explicit_arg
-                        else:
-                            msg = _gettext(
-                                f'ignored explicit argument {explicit_arg!r}'
-                            )
-                            raise _argparse.ArgumentError(action, msg)
-
-                    # if the action expect exactly one argument, we've
-                    # successfully matched the option; exit the loop
-                    elif arg_count == 1:
-                        stop = start_index + 1
-                        args = [explicit_arg]
-                        action_tuples.append((action, args, option_string))
-                        break
-
-                    # error if a double-dash option did not use the
-                    # explicit argument
-                    else:
-                        msg = _gettext(f'ignored explicit argument {explicit_arg!r}')
-                        raise _argparse.ArgumentError(action, msg)
-
-                # if there is no explicit argument, try to match the
-                # optional's string arguments with the following strings
-                # if successful, exit the loop
-                else:
-                    start = start_index + 1
-                    selected_patterns = arg_strings_pattern[start:]
-                    arg_count = match_argument(action, selected_patterns)
-                    stop = start + arg_count
-                    args = arg_strings[start:stop]
-                    action_tuples.append((action, args, option_string))
-                    break
-
-            # add the Optional to the list and return the index at which
-            # the Optional's string args stopped
-            assert action_tuples
-            for action, args, option_string in action_tuples:
-                take_action(action, args, option_string)
-            return stop
-
-        # the list of Positionals left to be parsed; this is modified
-        # by consume_positionals()
-        positionals = self._get_positional_actions()
-
-        # function to convert arg_strings into positional actions
-        def consume_positionals(start_index):
-            # match as many Positionals as possible
-            match_partial = self._match_arguments_partial
-            selected_pattern = arg_strings_pattern[start_index:]
-            arg_counts = match_partial(positionals, selected_pattern)
-
-            # slice off the appropriate arg strings for each Positional
-            # and add the Positional and its args to the list
-            for action, arg_count in zip(positionals, arg_counts):
-                args = arg_strings[start_index:start_index + arg_count]
-                start_index += arg_count
-                take_action(action, args)
-
-            # slice off the Positionals that we just parsed and return the
-            # index at which the Positionals' string args stopped
-            positionals[:] = positionals[len(arg_counts):]
-            return start_index
-
-        # consume Positionals and Optionals alternately, until we have
-        # passed the last option string
-        extras = []
-        start_index = 0
-        if option_string_indices:
-            max_option_string_index = max(option_string_indices)
-        else:
-            max_option_string_index = -1
-        while start_index <= max_option_string_index:
-
-            # consume any Positionals preceding the next option
-            next_option_string_index = min(
-                [index for index in option_string_indices if index >= start_index]
-            )
-            if start_index != next_option_string_index:
-                positionals_end_index = consume_positionals(start_index)
-
-                # only try to parse the next optional if we didn't consume
-                # the option string during the positionals parsing
-                if positionals_end_index > start_index:
-                    start_index = positionals_end_index
-                    continue
-                else:
-                    start_index = positionals_end_index
-
-            # if we consumed all the positionals we could and we're not
-            # at the index of an option string, there were extra arguments
-            if start_index not in option_string_indices:
-                strings = arg_strings[start_index:next_option_string_index]
-                extras.extend(strings)
-                start_index = next_option_string_index
-
-            # consume the next optional and any arguments for it
-            start_index = consume_optional(start_index)
-
-        # consume any positionals following the last Optional
-        stop_index = consume_positionals(start_index)
-
-        # if we didn't consume all the argument strings, there were extras
-        extras.extend(arg_strings[stop_index:])
-
-        # make sure all required actions were present and also convert
-        # action defaults which were not given as arguments
-        required_actions = []
-        for action in self._actions:
-            if action not in seen_actions:
-                if action.required:
-                    required_actions.append(_argparse._get_action_name(action))
-                else:
-                    # Convert action default now instead of doing it before
-                    # parsing arguments to avoid calling convert functions
-                    # twice (which may fail) if the argument was given, but
-                    # only if it was defined already in the namespace
-                    if (action.default is not None and isinstance(action.default, str)
-                            and hasattr(namespace, action.dest)
-                            and action.default is getattr(namespace, action.dest)):
-                        setattr(
-                            namespace, action.dest,
-                            self._get_value(action, action.default)
-                        )
-
-        if required_actions:
-            self.error(
-                _gettext(
-                    'the following arguments are required: ' +
-                    ", ".join(required_actions)
-                )
-            )
-
-        # make sure all required groups had one option present
-        for group in self._mutually_exclusive_groups:
-            if group.required:
-                for action in group._group_actions:
-                    if action in seen_non_default_actions:
-                        break
-
-                # if no actions were used, report the error
-                else:
-                    names = [
-                        _argparse._get_action_name(action)
-                        for action in group._group_actions
-                        if action.help is not _argparse.SUPPRESS
-                    ]
-                    self.error(
-                        _gettext(f'one of the arguments {" ".join(names)} is required')
-                    )
-
-        for group in self._action_groups:
-            if isinstance(group, _ArgumentGroup) and group.required:
-                for action in group._group_actions:
-                    if action in seen_non_default_actions:
-                        break
-
-                # if no actions were used, report the error
-                else:
-                    names = [
-                        _argparse._get_action_name(action)
-                        for action in group._group_actions
-                        if action.help is not _argparse.SUPPRESS
-                    ]
-                    self.error(
-                        _gettext(f'one of the arguments {" ".join(names)} is required')
-                    )
-
-        # return the updated namespace and the extra arguments
-        return namespace, extras
-
-
-class _ArgumentGroup(_argparse._ArgumentGroup, _ActionsContainer):
-
-    def __init__(
-        self,
-        container,
-        title=None,
-        description=None,
-        required: bool = False,
-        **kwargs
-    ):
-        super().__init__(container, title=title, description=description, **kwargs)
-
-        self.required = required
-
-
-class _MutuallyExclusiveGroup(_argparse._MutuallyExclusiveGroup, _ArgumentGroup):
-    pass
+# log21.Argparse.py
+# CodeWriter21
+
+from __future__ import annotations
+
+import re as _re
+import sys as _sys
+import types as _types
+import typing as _typing
+import argparse as _argparse
+from enum import Enum as _Enum
+from typing import (Tuple as _Tuple, Mapping as _Mapping, Optional as _Optional,
+                    Sequence as _Sequence)
+from gettext import gettext as _gettext
+from textwrap import TextWrapper as _TextWrapper
+from collections import OrderedDict as _OrderedDict
+
+import log21 as _log21
+from log21.Colors import get_colors as _gc
+from log21.Formatters import DecolorizingFormatter as _Formatter
+
+__all__ = [
+    'ColorizingArgumentParser', 'ColorizingHelpFormatter', 'ColorizingTextWrapper',
+    'Literal'
+]
+
+
+class Literal:
+    """A class for representing literals in argparse arguments."""
+
+    def __init__(self, literal: _typing._LiteralGenericAlias):
+        self.literal = literal
+        # Only str arguments are allowed
+        if not all(map(lambda x: isinstance(x, str), self.literal.__args__)):
+            raise TypeError('Only str arguments are allowed for Literal.')
+
+    def __repr__(self):
+        return f'Literal[{", ".join(map(str, self.literal.__args__))}]'
+
+    def __str__(self):
+        return self.__repr__()
+
+    def __call__(self, value):
+        if value not in self.literal.__args__:
+            raise ValueError(
+                f'Value must be one of [{", ".join(map(str, self.literal.__args__))}]'
+            )
+        return value
+
+
+class ColorizingHelpFormatter(_argparse.HelpFormatter):
+    """A help formatter that supports colorizing help messages."""
+
+    def __init__(
+        self,
+        prog,
+        indent_increment=2,
+        max_help_position=24,
+        width=None,
+        colors: _Optional[_Mapping[str, str]] = None
+    ):
+        super().__init__(prog, indent_increment, max_help_position, width)
+
+        self.colors = {
+            'usage': 'Cyan',
+            'brackets': 'LightRed',
+            'switches': 'LightCyan',
+            'values': 'Green',
+            'colons': 'LightRed',
+            'commas': 'LightRed',
+            'section headers': 'LightGreen',
+            'help': 'LightWhite',
+            'choices': 'LightGreen'
+        }
+
+        if colors:
+            for key, value in colors.items():
+                if key in self.colors:
+                    self.colors[key] = value
+
+    class _Section(object):
+
+        def __init__(self, formatter, parent, heading=None):
+            self.formatter = formatter
+            self.parent = parent
+            self.heading = heading
+            self.items = []
+
+        def format_help(self):
+            # format the indented section
+            if self.parent is not None:
+                self.formatter._indent()
+            join = self.formatter._join_parts
+            item_help = join([func(*args) for func, args in self.items])
+            if self.parent is not None:
+                self.formatter._dedent()
+
+            # return nothing if the section was empty
+            if not item_help:
+                return ''
+
+            # add the heading if the section was non-empty
+            if self.heading is not _argparse.SUPPRESS and self.heading is not None:
+                current_indent = self.formatter._current_indent
+                heading = (
+                    '%*s%s' % (current_indent, '', self.heading) +
+                    _gc(self.formatter.colors['colons']) + ':\033[0m\n'
+                )
+            else:
+                heading = ''
+
+            # join the section-initial newline, the heading and the help
+            return join(
+                ['\n', heading,
+                 _gc(self.formatter.colors['help']), item_help, '\n']
+            )
+
+    def _add_item(self, func, args):
+        self._current_section.items.append((func, args))
+
+    def _fill_text(self, text, width, indent):
+        text = self._whitespace_matcher.sub(' ', text).strip()
+        return ColorizingTextWrapper(
+            width=width, initial_indent=indent, subsequent_indent=indent
+        ).fill(text)
+
+    def _split_lines(self, text, width):
+        text = self._whitespace_matcher.sub(' ', text).strip()
+        return ColorizingTextWrapper(width=width).wrap(text)
+
+    def start_section(self, heading):
+        self._indent()
+        section = self._Section(
+            self, self._current_section,
+            _gc(self.colors['section headers']) + str(heading) + '\033[0m'
+        )
+        self._add_item(section.format_help, [])
+        self._current_section = section
+
+    def _format_action(self, action):
+        # determine the required width and the entry label
+        help_position = min(self._action_max_length + 2, self._max_help_position)
+        help_width = max(self._width - help_position, 11)
+        action_width = help_position - self._current_indent - 2
+        action_header = _gc('rst') + self._format_action_invocation(action)
+
+        indent_first = 0
+        # no help; start on same line and add a final newline
+        if not action.help:
+            action_header = self._current_indent * ' ' + action_header + '\n'
+        # short action name; start on the same line and pad two spaces
+        elif len(action_header) <= action_width:
+            action_header = '%*s%-*s  ' % (
+                self._current_indent, '', action_width, action_header
+            )
+        # long action name; start on the next line
+        else:
+            action_header = self._current_indent * ' ' + action_header + '\n'
+            indent_first = help_position
+
+        # collect the pieces of the action help
+        parts = [action_header]
+
+        # if there was help for the action, add lines of help text
+        if action.help:
+            help_text = _gc(self.colors['help']) + self._expand_help(action)
+            help_lines = self._split_lines(help_text, help_width)
+            parts.append('%*s%s\n' % (indent_first, '', help_lines[0]))
+            for line in help_lines[1:]:
+                parts.append('%*s%s\n' % (help_position, '', line))
+
+        # or add a newline if the description doesn't end with one
+        elif not action_header.endswith('\n'):
+            parts.append('\n')
+
+        # if there are any sub-actions, add their help as well
+        for subaction in self._iter_indented_subactions(action):
+            parts.append(self._format_action(subaction))
+
+        # return a single string
+        return self._join_parts(parts)
+
+    # modified upstream code, not going to refactor for complexity.
+    def _format_usage(self, usage, actions, groups, prefix):  # noqa: C901
+        if prefix is None:
+            prefix = _gettext('usage: ')
+
+        # if usage is specified, use that
+        if usage is not None:
+            usage = usage % dict(prog=self._prog)
+
+        # if no optionals or positionals are available, usage is just prog
+        elif usage is None and not actions:
+            usage = '%(prog)s' % dict(prog=self._prog)
+
+        # if optionals and positionals are available, calculate usage
+        elif usage is None:
+            prog = '%(prog)s' % dict(prog=self._prog)
+
+            # split optionals from positionals
+            optionals = []
+            positionals = []
+            for action in actions:
+                if action.option_strings:
+                    optionals.append(action)
+                else:
+                    positionals.append(action)
+
+            # build full usage string
+            action_usage = self._format_actions_usage(optionals + positionals, groups)
+            usage = ' '.join([s for s in [prog, action_usage] if s])
+
+            # wrap the usage parts if it's too long
+            text_width = self._width - self._current_indent
+            if len(prefix) + len(_Formatter.decolorize(usage)) > text_width:
+
+                # break usage into wrappable parts
+                part_regexp = r'\(.*?\)+|\[.*?\]+|\S+'
+                opt_usage = self._format_actions_usage(optionals, groups)
+                pos_usage = self._format_actions_usage(positionals, groups)
+                opt_parts = _re.findall(part_regexp, opt_usage)
+                pos_parts = _re.findall(part_regexp, pos_usage)
+                assert ' '.join(opt_parts) == opt_usage
+                assert ' '.join(pos_parts) == pos_usage
+
+                # helper for wrapping lines
+                def get_lines(parts, indent, prefix=None):
+                    lines = []
+                    line = []
+                    if prefix is not None:
+                        line_len = len(prefix) - 1
+                    else:
+                        line_len = len(indent) - 1
+                    for part in parts:
+                        if line_len + 1 + len(_Formatter.decolorize(part)
+                                              ) > text_width and line:
+                            lines.append(indent + ' '.join(line))
+                            line = []
+                            line_len = len(indent) - 1
+                        line.append(part)
+                        line_len += len(_Formatter.decolorize(part)) + 1
+                    if line:
+                        lines.append(indent + ' '.join(line))
+                    if prefix is not None:
+                        lines[0] = lines[0][len(indent):]
+                    return lines
+
+                # if prog is short, follow it with optionals or positionals
+                len_prog = len(_Formatter.decolorize(prog))
+                if len(prefix) + len_prog <= 0.75 * text_width:
+                    indent = ' ' * (len(prefix) + len_prog + 1)
+                    if opt_parts:
+                        lines = get_lines([prog] + opt_parts, indent, prefix)
+                        lines.extend(get_lines(pos_parts, indent))
+                    elif pos_parts:
+                        lines = get_lines([prog] + pos_parts, indent, prefix)
+                    else:
+                        lines = [prog]
+
+                # if prog is long, put it on its own line
+                else:
+                    indent = ' ' * len(prefix)
+                    parts = opt_parts + pos_parts
+                    lines = get_lines(parts, indent)
+                    if len(lines) > 1:
+                        lines = []
+                        lines.extend(get_lines(opt_parts, indent))
+                        lines.extend(get_lines(pos_parts, indent))
+                    lines = [prog] + lines
+
+                # join lines into usage
+                usage = '\n'.join(lines)
+
+        # prefix with 'usage:'
+        return prefix + usage + '\n\n'
+
+    def _format_actions_usage(self, actions: list, groups):
+        # find group indices and identify actions in groups
+        group_actions = set()
+        inserts = {}
+        for group in groups:
+            try:
+                start = actions.index(group._group_actions[0])
+            except ValueError:
+                continue
+            else:
+                end = start + len(group._group_actions)
+                if actions[start:end] == group._group_actions:
+                    for action in group._group_actions:
+                        group_actions.add(action)
+                    if not group.required:
+                        if start in inserts:
+                            inserts[start] += ' ['
+                        else:
+                            inserts[start] = '['
+                        if end in inserts:
+                            inserts[end] += ']'
+                        else:
+                            inserts[end] = ']'
+                    else:
+                        if start in inserts:
+                            inserts[start] += ' ('
+                        else:
+                            inserts[start] = '('
+                        if end in inserts:
+                            inserts[end] += ')'
+                        else:
+                            inserts[end] = ')'
+                    for i in range(start + 1, end):
+                        inserts[i] = '|'
+
+        # collect all actions format strings
+        parts = []
+        for i, action in enumerate(actions):
+
+            # suppressed arguments are marked with None
+            # remove | separators for suppressed arguments
+            if action.help is _argparse.SUPPRESS:
+                parts.append(None)
+                if inserts.get(i) == '|':
+                    inserts.pop(i)
+                elif inserts.get(i + 1) == '|':
+                    inserts.pop(i + 1)
+
+            # produce all arg strings
+            elif not action.option_strings:
+                default = self._get_default_metavar_for_positional(action)
+                part = self._format_args(action, default)
+
+                # if it's in a group, strip the outer []
+                if action in group_actions:
+                    if part[0] == '[' and part[-1] == ']':
+                        part = part[1:-1]
+
+                # add the action string to the list
+                parts.append(part)
+
+            # produce the first way to invoke the option in brackets
+            else:
+                option_string = action.option_strings[0]
+
+                # if the Optional doesn't take a value, format is:
+                #    -s or --long
+                if action.nargs == 0:
+                    part = _gc(self.colors['switches']) + action.format_usage()
+
+                # if the Optional takes a value, format is:
+                #    -s ARGS or --long ARGS
+                else:
+                    default = self._get_default_metavar_for_optional(action)
+                    args_string = self._format_args(action, default)
+                    part = _gc(self.colors['switches']) + '%s %s%s' % (
+                        option_string, _gc(self.colors['values']), args_string
+                    )
+
+                # make it look optional if it's not required or in a group
+                if not action.required and action not in group_actions:
+                    part = _gc(self.colors['brackets']) + '[' + part + _gc(
+                        self.colors['brackets']
+                    ) + ']\033[0m'
+
+                # add the action string to the list
+                parts.append(part)
+
+        # insert things at the necessary indices
+        for i in sorted(inserts, reverse=True):
+            parts[i:i] = [inserts[i]]
+
+        # join all the action items with spaces
+        text = ' '.join([item for item in parts if item is not None])
+
+        # clean up separators for mutually exclusive groups
+        open = r'[\[(]'
+        close = r'[\])]'
+        text = _re.sub(r'(%s) ' % open, r'\1', text)
+        text = _re.sub(r' (%s)' % close, r'\1', text)
+        text = _re.sub(r'%s *%s' % (open, close), r'', text)
+        text = _re.sub(r'\(([^|]*)\)', r'\1', text)
+        text = text.strip()
+
+        # return the text
+        return text
+
+    def _format_action_invocation(self, action):
+        if not action.option_strings:
+            default = self._get_default_metavar_for_positional(action)
+            metavar, = self._metavar_formatter(action, default)(1)
+            return metavar
+
+        else:
+            parts = []
+
+            # if the Optional doesn't take a value, format is:
+            #    -s, --long
+            if action.nargs == 0:
+                for option_string in action.option_strings:
+                    parts.append(_gc(self.colors['switches']) + option_string)
+
+            # if the Optional takes a value, format is:
+            #    -s ARGS, --long ARGS
+            else:
+                default = self._get_default_metavar_for_optional(action)
+                args_string = self._format_args(action, default)
+                for option_string in action.option_strings:
+                    parts.append(
+                        _gc(self.colors['switches']) + '%s %s%s' %
+                        (option_string, _gc(self.colors['values']), args_string)
+                    )
+
+            return _gc(self.colors['commas']) + ', '.join(parts)
+
+    def _metavar_formatter(self, action, default_metavar):
+        if action.metavar is not None:
+            result = action.metavar
+        elif action.choices is not None:
+            choice_strs = [str(choice) for choice in action.choices]
+            result = (
+                _gc(self.colors['brackets']) + '{ ' +
+                (_gc(self.colors['commas']) + ', ').join(
+                    _gc(self.colors['choices']) + choice_str
+                    for choice_str in choice_strs
+                ) + _gc(self.colors['brackets']) + ' }'
+            )
+        else:
+            result = default_metavar
+
+        def format(tuple_size):
+            if isinstance(result, tuple):
+                return result
+            else:
+                return (result, ) * tuple_size
+
+        return format
+
+
+class ColorizingTextWrapper(_TextWrapper):
+    # modified upstream code, not going to refactor for complexity.
+    def _wrap_chunks(self, chunks):  # noqa: C901
+        """_wrap_chunks(chunks : [string]) -> [string]
+
+        Wrap a sequence of text chunks and return a list of lines of
+        length 'self.width' or less.  (If 'break_long_words' is false,
+        some lines may be longer than this.)  Chunks correspond roughly
+        to words and the whitespace between them: each chunk is
+        indivisible (modulo 'break_long_words'), but a line break can
+        come between any two chunks.  Chunks should not have internal
+        whitespace; i.e. a chunk is either all whitespace or a "word".
+        Whitespace chunks will be removed from the beginning and end of
+        lines, but apart from that whitespace is preserved.
+        """
+        lines = []
+        if self.width <= 0:
+            raise ValueError("invalid width %r (must be > 0)" % self.width)
+        if self.max_lines is not None:
+            if self.max_lines > 1:
+                indent = self.subsequent_indent
+            else:
+                indent = self.initial_indent
+            if len(indent) + len(self.placeholder.lstrip()) > self.width:
+                raise ValueError("placeholder too large for max width")
+
+        # Arrange in reverse order so items can be efficiently popped
+        # from a stack of chucks.
+        chunks.reverse()
+
+        while chunks:
+
+            # Start the list of chunks that will make up the current line.
+            # current_len is just the length of all the chunks in current_line.
+            current_line = []
+            current_len = 0
+
+            # Figure out which static string will prefix this line.
+            if lines:
+                indent = self.subsequent_indent
+            else:
+                indent = self.initial_indent
+
+            # Maximum width for this line.
+            width = self.width - len(indent)
+
+            # First chunk on the line is whitespace -- drop it, unless this
+            # is the very beginning of the text (i.e. no lines started yet).
+            if self.drop_whitespace and _Formatter.decolorize(chunks[-1]
+                                                              ).strip() == '' and lines:
+                del chunks[-1]
+
+            while chunks:
+                # modified upstream code, not going to refactor for ambiguous variable
+                # name.
+                length = len(_Formatter.decolorize(chunks[-1]))  # noqa: E741
+
+                # Can at least squeeze this chunk onto the current line.
+                # Modified upstream code, not going to refactor for ambiguous variable
+                # name.
+                if current_len + length <= width:  # noqa: E741
+                    current_line.append(chunks.pop())
+                    current_len += length
+                # Nope, this line is full.
+                else:
+                    break
+
+            # The current line is full, and the next chunk is too big to
+            # fit on *any* line (not just this one).
+            if chunks and len(_Formatter.decolorize(chunks[-1])) > width:
+                self._handle_long_word(chunks, current_line, current_len, width)
+                current_len = sum(map(len, current_line))
+
+            # If the last chunk on this line is all whitespace, drop it.
+            if self.drop_whitespace and current_line and _Formatter.decolorize(
+                    current_line[-1]).strip() == '':
+                current_len -= len(_Formatter.decolorize(current_line[-1]))
+                del current_line[-1]
+
+            if current_line:
+                if (self.max_lines is None or len(lines) + 1 < self.max_lines
+                        or (not chunks or self.drop_whitespace and len(chunks) == 1
+                            and not chunks[0].strip()) and current_len <= width):
+                    # Convert current line back to a string and store it in
+                    # list of all lines (return value).
+                    lines.append(indent + ''.join(current_line))
+                else:
+                    while current_line:
+                        if _Formatter.decolorize(
+                                current_line[-1]
+                        ).strip() and current_len + len(self.placeholder) <= width:
+                            current_line.append(self.placeholder)
+                            lines.append(indent + ''.join(current_line))
+                            break
+                        current_len -= len(_Formatter.decolorize(current_line[-1]))
+                        del current_line[-1]
+                    else:
+                        if lines:
+                            prev_line = lines[-1].rstrip()
+                            if len(_Formatter.decolorize(prev_line)) + len(
+                                    self.placeholder) <= self.width:
+                                lines[-1] = prev_line + self.placeholder
+                                break
+                        lines.append(indent + self.placeholder.lstrip())
+                    break
+
+        return lines
+
+
+class _ActionsContainer(_argparse._ActionsContainer):
+    """Container for the actions for a single command line option."""
+
+    # pylint: disable=too-many-branches
+    def _validate_func_type(self, action, func_type, kwargs, level: int = 0) -> _Tuple:
+        # raise an error if the action type is not callable
+        if (hasattr(_types, 'UnionType') and not callable(func_type)
+                and not isinstance(func_type, (_types.UnionType, tuple))):
+            raise ValueError(f'{func_type} is not callable; level={level}')
+
+        # Handle `UnionType` as a type (e.g. `int|str`)
+        if hasattr(_types, 'UnionType') and isinstance(func_type, _types.UnionType):
+            func_type = func_type.__args__  # type: ignore
+
+        # Handle `Literal` as a type (e.g. `Literal[1, 2, 3]`)
+        elif (hasattr(_typing, '_LiteralGenericAlias')
+              and isinstance(func_type, _typing._LiteralGenericAlias)):  # type: ignore
+            func_type = Literal(func_type)
+
+        # Handle `List` as a type (e.g. `List[int]`)
+        elif (hasattr(_typing, '_GenericAlias')
+              and isinstance(func_type, _typing._GenericAlias)  # type: ignore
+              and func_type.__origin__ is list):
+            func_type = func_type.__args__[0]
+            if kwargs.get('nargs') is None:
+                action.nargs = '+'
+
+        # Handle `Required` as a type (e.g. `Required[int]`)
+        elif (hasattr(_typing, 'Required') and hasattr(_typing, '_GenericAlias')
+              and isinstance(func_type, _typing._GenericAlias)  # type: ignore
+              and func_type.__origin__ is _typing.Required
+              ):
+            func_type = func_type.__args__[0]
+            action.required = True
+
+        # Handle `Union` and `Optional` as a type (e.g. `Union[int, str]` and
+        # `Optional[int]`)
+        elif (hasattr(_types, 'NoneType') and hasattr(_typing, '_UnionGenericAlias')
+              and isinstance(func_type, _typing._UnionGenericAlias)):  # type: ignore
+            # Optional[T] is just Union[T, NoneType]
+            # Optional
+            if (len(func_type.__args__) == 2
+                    and func_type.__args__[1] is _types.NoneType):
+                action.required = False
+                func_type = func_type.__args__[0]
+            # Union
+            else:
+                func_type = func_type.__args__  # type: ignore
+
+        # Handle Enum as a type
+        elif callable(func_type) and isinstance(func_type, type) and issubclass(
+                func_type, _Enum) and action.choices is None and level == 0:
+            action.choices = tuple(
+                map(lambda x: x.value, func_type.__members__.values())
+            )
+
+        # Handle SpecialForms
+        elif isinstance(func_type, _typing._SpecialForm):
+            if func_type is _typing.Any:
+                func_type = None
+            elif func_type is _typing.ClassVar:
+                func_type = None
+            elif func_type is _typing.Union:
+                func_type = None
+            elif func_type is _typing.Optional:
+                func_type = None
+                action.required = False
+            elif func_type is _typing.Type:
+                func_type = None
+            elif func_type is _typing.TypeVar:
+                func_type = None
+            else:
+                raise ValueError(f'Unknown special form {func_type}')
+
+        elif func_type is _argparse.FileType:
+            raise ValueError(
+                f'{func_type} is a FileType class object, instance of it must be passed'
+            )
+
+        if isinstance(func_type, _Sequence):
+            temp = []
+            for type_ in _OrderedDict(zip(func_type, [0] * len(func_type))):
+                temp.extend(self._validate_func_type(action, type_, kwargs, level + 1))
+            func_type = tuple(temp)
+        else:
+            if (hasattr(_types, 'UnionType') and hasattr(_typing, '_GenericAlias')
+                    and hasattr(_typing, '_UnionGenericAlias')
+                    and hasattr(_typing, '_LiteralGenericAlias') and isinstance(
+                        func_type,
+                        (
+                            _typing._GenericAlias,  # type: ignore
+                            _typing._UnionGenericAlias,  # type: ignore
+                            _typing._LiteralGenericAlias,  # type: ignore
+                            _types.UnionType,
+                        ))):
+                func_type = self._validate_func_type(
+                    action, func_type, kwargs, level + 1
+                )
+            else:
+                func_type = (func_type, )
+
+        return func_type
+
+    # Override the default add_argument method defined in argparse._ActionsContainer
+    # to add the support for different type annotations
+    def add_argument(self, *args, **kwargs):
+        """Add an argument to the parser.
+
+        Signature:
+            add_argument(dest, ..., name=value, ...)
+            add_argument(option_string, option_string, ..., name=value, ...)
+        """
+
+        # if no positional args are supplied or only one is supplied and
+        # it doesn't look like an option string, parse a positional
+        # argument
+        chars = self.prefix_chars
+        if not args or len(args) == 1 and args[0][0] not in chars:
+            if args and 'dest' in kwargs:
+                raise ValueError('dest supplied twice for positional argument')
+            kwargs = self._get_positional_kwargs(*args, **kwargs)
+
+        # otherwise, we're adding an optional argument
+        else:
+            kwargs = self._get_optional_kwargs(*args, **kwargs)
+
+        # if no default was supplied, use the parser-level default
+        if 'default' not in kwargs:
+            dest = kwargs['dest']
+            if dest in self._defaults:
+                kwargs['default'] = self._defaults[dest]
+            elif self.argument_default is not None:
+                kwargs['default'] = self.argument_default
+
+        # create the action object, and add it to the parser
+        action_class = self._pop_action_class(kwargs)
+        if not callable(action_class):
+            raise ValueError(f'unknown action "{action_class}"')
+        action = action_class(**kwargs)
+
+        func_type = self._registry_get('type', action.type, action.type)
+        action.type = self._validate_func_type(
+            action, func_type, kwargs
+        )  # type: ignore
+        if len(action.type) == 1:
+            action.type = action.type[0]
+        elif len(action.type) == 0:
+            action.type = None
+
+        # raise an error if the metavar does not match the type
+        if hasattr(self, "_get_formatter"):
+            try:
+                self._get_formatter()._format_args(action, None)
+            except TypeError:
+                raise ValueError(
+                    "length of metavar tuple does not match nargs"
+                ) from None
+
+        return self._add_action(action)
+
+    def add_argument_group(self, *args, **kwargs):
+        group = _ArgumentGroup(self, *args, **kwargs)
+        self._action_groups.append(group)
+        return group
+
+    def add_mutually_exclusive_group(self, **kwargs):
+        group = _MutuallyExclusiveGroup(self, **kwargs)
+        self._mutually_exclusive_groups.append(group)
+        return group
+
+
+class ColorizingArgumentParser(_argparse.ArgumentParser, _ActionsContainer):
+    """An ArgumentParser that colorizes its output and more."""
+
+    def __init__(
+        self,
+        formatter_class=ColorizingHelpFormatter,
+        colors: _Optional[_Mapping[str, str]] = None,
+        **kwargs
+    ):
+        self.logger = _log21.Logger('ArgumentParser')
+        self.colors = colors
+        super().__init__(formatter_class=formatter_class, **kwargs)
+
+    def _print_message(self, message, file=None):
+        if message:
+            self.logger.handlers.clear()
+            handler = _log21.ColorizingStreamHandler(stream=file)
+            self.logger.addHandler(handler)
+            self.logger.info(message + _gc('rst'))
+
+    def exit(self, status=0, message=None):
+        if message:
+            self._print_message(_gc('lr') + message + _gc('rst'), _sys.stderr)
+        _sys.exit(status)
+
+    def error(self, message):
+        self.print_usage(_sys.stderr)
+        args = {'prog': self.prog, 'message': message}
+        self.exit(
+            2,
+            _gettext(
+                f'%(prog)s: {_gc("r")}error{_gc("lr")}:{_gc("rst")} %(message)s\n'
+            ) % args
+        )
+
+    def _get_formatter(self):
+        if hasattr(self.formatter_class, 'colors'):
+            return self.formatter_class(prog=self.prog, colors=self.colors)
+        else:
+            return self.formatter_class(prog=self.prog)
+
+    def _get_value(self, action, arg_string):
+        """Override _get_value to add support for types such as Union and
+        Literal."""
+
+        func_type = self._registry_get('type', action.type, action.type)
+        if not callable(func_type) and not isinstance(func_type, tuple):
+            raise _argparse.ArgumentError(
+                action, _gettext(f'{func_type!r} is not callable')
+            )
+
+        name = getattr(action.type, '__name__', repr(action.type))
+
+        # convert the value to the appropriate type
+        try:
+            if callable(func_type):
+                result = func_type(arg_string)
+            else:
+                exception = ValueError()
+                for type_ in func_type:
+                    name = getattr(type_, '__name__', repr(type_))
+                    try:
+                        result = type_(arg_string)
+                        break
+                    except (ValueError, TypeError) as ex:
+                        exception = ex
+                else:
+                    raise exception
+
+        # ArgumentTypeErrors indicate errors
+        except _argparse.ArgumentTypeError as ex:
+            msg = str(ex)
+            raise _argparse.ArgumentError(action, msg)
+
+        # TypeErrors or ValueErrors also indicate errors
+        except (TypeError, ValueError):
+            raise _argparse.ArgumentError(
+                action, _gettext(f'invalid {name!s} value: {arg_string!r}')
+            ) from None
+
+        # return the converted value
+        return result
+
+    def __convert_type(self, func_type, arg_string):
+        result = None
+        if callable(func_type):
+            try:
+                result = func_type(arg_string)
+            except Exception:
+                pass
+        else:
+            for type_ in func_type:
+                try:
+                    result = type_(arg_string)
+                    break
+                except Exception:
+                    pass
+
+        return result
+
+    def _check_value(self, action, choice):
+        # converted value must be one of the choices (if specified)
+        if action.choices is not None:
+            choices = set(action.choices)
+
+            func_type = self._registry_get('type', action.type, action.type)
+            if not callable(func_type) and not isinstance(func_type, tuple):
+                raise _argparse.ArgumentError(
+                    action, _gettext(f'{func_type!r} is not callable')
+                )
+
+            for value in action.choices:
+                choices.add(self.__convert_type(func_type, value))
+
+            if choice not in choices:
+                raise _argparse.ArgumentError(
+                    action,
+                    _gettext(
+                        f'invalid choice: {choice!r} '
+                        f'(choose from {", ".join(map(repr, action.choices))})'
+                    )
+                )
+
+    def _read_args_from_files(self, arg_strings):
+        # expand arguments referencing files
+        new_arg_strings = []
+        for arg_string in arg_strings:
+
+            # for regular arguments, just add them back into the list
+            if not arg_string or arg_string[0] not in self.fromfile_prefix_chars:
+                new_arg_strings.append(arg_string)
+
+            # replace arguments referencing files with the file content
+            else:
+                try:
+                    with open(arg_string[1:]) as args_file:
+                        arg_strings = []
+                        for arg_line in args_file.read().splitlines():
+                            for arg in self.convert_arg_line_to_args(arg_line):
+                                arg_strings.append(arg)
+                        arg_strings = self._read_args_from_files(arg_strings)
+                        new_arg_strings.extend(arg_strings)
+                except OSError as err:
+                    self.error(str(err))
+
+        # return the modified argument list
+        return new_arg_strings
+
+    def _parse_known_args(self, arg_strings, namespace):
+        # replace arg strings that are file references
+        if self.fromfile_prefix_chars is not None:
+            arg_strings = self._read_args_from_files(arg_strings)
+
+        # map all mutually exclusive arguments to the other arguments
+        # they can't occur with
+        action_conflicts = {}
+        for mutex_group in self._mutually_exclusive_groups:
+            group_actions = mutex_group._group_actions
+            for i, mutex_action in enumerate(mutex_group._group_actions):
+                conflicts = action_conflicts.setdefault(mutex_action, [])
+                conflicts.extend(group_actions[:i])
+                conflicts.extend(group_actions[i + 1:])
+
+        # find all option indices, and determine the arg_string_pattern
+        # which has an 'O' if there is an option at an index,
+        # an 'A' if there is an argument, or a '-' if there is a '--'
+        option_string_indices = {}
+        arg_string_pattern_parts = []
+        arg_strings_iter = iter(arg_strings)
+        for i, arg_string in enumerate(arg_strings_iter):
+
+            # all args after -- are non-options
+            if arg_string == '--':
+                arg_string_pattern_parts.append('-')
+                for arg_string in arg_strings_iter:
+                    arg_string_pattern_parts.append('A')
+
+            # otherwise, add the arg to the arg strings
+            # and note the index if it was an option
+            else:
+                option_tuple = self._parse_optional(arg_string)
+                if option_tuple is None:
+                    pattern = 'A'
+                else:
+                    option_string_indices[i] = option_tuple
+                    pattern = 'O'
+                arg_string_pattern_parts.append(pattern)
+
+        # join the pieces together to form the pattern
+        arg_strings_pattern = ''.join(arg_string_pattern_parts)
+
+        # converts arg strings to the appropriate and then takes the action
+        seen_actions = set()
+        seen_non_default_actions = set()
+
+        def take_action(action, argument_strings, option_string=None):
+            seen_actions.add(action)
+            argument_values = self._get_values(action, argument_strings)
+
+            # error if this argument is not allowed with other previously
+            # seen arguments, assuming that actions that use the default
+            # value don't really count as "present"
+            if argument_values is not action.default:
+                seen_non_default_actions.add(action)
+                for conflict_action in action_conflicts.get(action, []):
+                    if conflict_action in seen_non_default_actions:
+                        action_name = _argparse._get_action_name(conflict_action)
+                        msg = _gettext(f'not allowed with argument {action_name}')
+                        raise _argparse.ArgumentError(action, msg)
+
+            # take the action if we didn't receive a SUPPRESS value
+            # (e.g. from a default)
+            if argument_values is not _argparse.SUPPRESS:
+                action(self, namespace, argument_values, option_string)
+
+        # function to convert arg_strings into an optional action
+        def consume_optional(start_index):
+
+            # get the optional identified at this index
+            option_tuple = option_string_indices[start_index]
+            action, option_string, explicit_arg = option_tuple
+
+            # identify additional optionals in the same arg string
+            # (e.g. -xyz is the same as -x -y -z if no args are required)
+            match_argument = self._match_argument
+            action_tuples = []
+            while True:
+
+                # if we found no optional action, skip it
+                if action is None:
+                    extras.append(arg_strings[start_index])
+                    return start_index + 1
+
+                # if there is an explicit argument, try to match the
+                # optional's string arguments to only this
+                if explicit_arg is not None:
+                    arg_count = match_argument(action, 'A')
+
+                    # if the action is a single-dash option and takes no
+                    # arguments, try to parse more single-dash options out
+                    # of the tail of the option string
+                    chars = self.prefix_chars
+                    if arg_count == 0 and option_string[1] not in chars:
+                        action_tuples.append((action, [], option_string))
+                        char = option_string[0]
+                        option_string = char + explicit_arg[0]
+                        new_explicit_arg = explicit_arg[1:] or None
+                        optionals_map = self._option_string_actions
+                        if option_string in optionals_map:
+                            action = optionals_map[option_string]
+                            explicit_arg = new_explicit_arg
+                        else:
+                            msg = _gettext(
+                                f'ignored explicit argument {explicit_arg!r}'
+                            )
+                            raise _argparse.ArgumentError(action, msg)
+
+                    # if the action expect exactly one argument, we've
+                    # successfully matched the option; exit the loop
+                    elif arg_count == 1:
+                        stop = start_index + 1
+                        args = [explicit_arg]
+                        action_tuples.append((action, args, option_string))
+                        break
+
+                    # error if a double-dash option did not use the
+                    # explicit argument
+                    else:
+                        msg = _gettext(f'ignored explicit argument {explicit_arg!r}')
+                        raise _argparse.ArgumentError(action, msg)
+
+                # if there is no explicit argument, try to match the
+                # optional's string arguments with the following strings
+                # if successful, exit the loop
+                else:
+                    start = start_index + 1
+                    selected_patterns = arg_strings_pattern[start:]
+                    arg_count = match_argument(action, selected_patterns)
+                    stop = start + arg_count
+                    args = arg_strings[start:stop]
+                    action_tuples.append((action, args, option_string))
+                    break
+
+            # add the Optional to the list and return the index at which
+            # the Optional's string args stopped
+            assert action_tuples
+            for action, args, option_string in action_tuples:
+                take_action(action, args, option_string)
+            return stop
+
+        # the list of Positionals left to be parsed; this is modified
+        # by consume_positionals()
+        positionals = self._get_positional_actions()
+
+        # function to convert arg_strings into positional actions
+        def consume_positionals(start_index):
+            # match as many Positionals as possible
+            match_partial = self._match_arguments_partial
+            selected_pattern = arg_strings_pattern[start_index:]
+            arg_counts = match_partial(positionals, selected_pattern)
+
+            # slice off the appropriate arg strings for each Positional
+            # and add the Positional and its args to the list
+            for action, arg_count in zip(positionals, arg_counts):
+                args = arg_strings[start_index:start_index + arg_count]
+                start_index += arg_count
+                take_action(action, args)
+
+            # slice off the Positionals that we just parsed and return the
+            # index at which the Positionals' string args stopped
+            positionals[:] = positionals[len(arg_counts):]
+            return start_index
+
+        # consume Positionals and Optionals alternately, until we have
+        # passed the last option string
+        extras = []
+        start_index = 0
+        if option_string_indices:
+            max_option_string_index = max(option_string_indices)
+        else:
+            max_option_string_index = -1
+        while start_index <= max_option_string_index:
+
+            # consume any Positionals preceding the next option
+            next_option_string_index = min(
+                [index for index in option_string_indices if index >= start_index]
+            )
+            if start_index != next_option_string_index:
+                positionals_end_index = consume_positionals(start_index)
+
+                # only try to parse the next optional if we didn't consume
+                # the option string during the positionals parsing
+                if positionals_end_index > start_index:
+                    start_index = positionals_end_index
+                    continue
+                else:
+                    start_index = positionals_end_index
+
+            # if we consumed all the positionals we could and we're not
+            # at the index of an option string, there were extra arguments
+            if start_index not in option_string_indices:
+                strings = arg_strings[start_index:next_option_string_index]
+                extras.extend(strings)
+                start_index = next_option_string_index
+
+            # consume the next optional and any arguments for it
+            start_index = consume_optional(start_index)
+
+        # consume any positionals following the last Optional
+        stop_index = consume_positionals(start_index)
+
+        # if we didn't consume all the argument strings, there were extras
+        extras.extend(arg_strings[stop_index:])
+
+        # make sure all required actions were present and also convert
+        # action defaults which were not given as arguments
+        required_actions = []
+        for action in self._actions:
+            if action not in seen_actions:
+                if action.required:
+                    required_actions.append(_argparse._get_action_name(action))
+                else:
+                    # Convert action default now instead of doing it before
+                    # parsing arguments to avoid calling convert functions
+                    # twice (which may fail) if the argument was given, but
+                    # only if it was defined already in the namespace
+                    if (action.default is not None and isinstance(action.default, str)
+                            and hasattr(namespace, action.dest)
+                            and action.default is getattr(namespace, action.dest)):
+                        setattr(
+                            namespace, action.dest,
+                            self._get_value(action, action.default)
+                        )
+
+        if required_actions:
+            self.error(
+                _gettext(
+                    'the following arguments are required: ' +
+                    ", ".join(required_actions)
+                )
+            )
+
+        # make sure all required groups had one option present
+        for group in self._mutually_exclusive_groups:
+            if group.required:
+                for action in group._group_actions:
+                    if action in seen_non_default_actions:
+                        break
+
+                # if no actions were used, report the error
+                else:
+                    names = [
+                        _argparse._get_action_name(action)
+                        for action in group._group_actions
+                        if action.help is not _argparse.SUPPRESS
+                    ]
+                    self.error(
+                        _gettext(f'one of the arguments {" ".join(names)} is required')
+                    )
+
+        for group in self._action_groups:
+            if isinstance(group, _ArgumentGroup) and group.required:
+                for action in group._group_actions:
+                    if action in seen_non_default_actions:
+                        break
+
+                # if no actions were used, report the error
+                else:
+                    names = [
+                        _argparse._get_action_name(action)
+                        for action in group._group_actions
+                        if action.help is not _argparse.SUPPRESS
+                    ]
+                    self.error(
+                        _gettext(f'one of the arguments {" ".join(names)} is required')
+                    )
+
+        # return the updated namespace and the extra arguments
+        return namespace, extras
+
+
+class _ArgumentGroup(_argparse._ArgumentGroup, _ActionsContainer):
+
+    def __init__(
+        self,
+        container,
+        title=None,
+        description=None,
+        required: bool = False,
+        **kwargs
+    ):
+        super().__init__(container, title=title, description=description, **kwargs)
+
+        self.required = required
+
+
+class _MutuallyExclusiveGroup(_argparse._MutuallyExclusiveGroup, _ArgumentGroup):
+    pass
```

### Comparing `log21-2.8.1b0/src/log21/Argumentify.py` & `log21-2.9.0/src/log21/Argumentify.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,427 +1,427 @@
-# log21.Argparse.py
-# CodeWriter21
-
-import re as _re
-import string as _string
-import asyncio as _asyncio
-import inspect as _inspect
-from typing import (Any as _Any, Set as _Set, Dict as _Dict, List as _List,
-                    Tuple as _Tuple, Union as _Union, Callable as _Callable,
-                    Optional as _Optional, Awaitable as _Awaitable,
-                    Coroutine as _Coroutine, OrderedDict as _OrderedDict)
-from dataclasses import field as _field, dataclass as _dataclass
-
-from docstring_parser import Docstring as _Docstring, parse as _parse
-
-import log21.Argparse as _Argparse
-
-__all__ = [
-    'argumentify', 'ArgumentifyError', 'ArgumentTypeError', 'FlagGenerationError',
-    'RESERVED_FLAGS', 'Callable', 'Argument', 'FunctionInfo', 'generate_flag',
-    'normalize_name', 'normalize_name_to_snake_case'
-]
-
-Callable = _Union[_Callable[..., _Any], _Callable[..., _Coroutine[_Any, _Any, _Any]]]
-RESERVED_FLAGS = {'--help', '-h'}
-
-
-class ArgumentifyError(Exception):
-    """Base class for exceptions in this module."""
-
-
-class ArgumentTypeError(ArgumentifyError, TypeError):
-    """Exception raised when a function has an unsupported type of argument.
-
-    e.g: a function has a VAR_KEYWORD argument.
-    """
-
-    def __init__(
-        self, message: _Optional[str] = None, unsupported_arg: _Optional[str] = None
-    ):
-        """Initialize the exception.
-
-        :param message: The message to display.
-        :param unsupported_arg: The name of the unsupported argument.
-        """
-        if message is None:
-            if unsupported_arg is None:
-                message = 'Unsupported argument type.'
-            else:
-                message = f'Unsupported argument type: {unsupported_arg}'
-        self.message = message
-        self.unsupported_arg = unsupported_arg
-
-
-class FlagGenerationError(ArgumentifyError, RuntimeError):
-    """Exception raised when an error occurs while generating a flag.
-
-    Most likely raised when there are arguments with the same name.
-    """
-
-    def __init__(self, message: _Optional[str] = None, arg_name: _Optional[str] = None):
-        """Initialize the exception.
-
-        :param message: The message to display.
-        :param arg_name: The name of the argument that caused the error.
-        """
-        if message is None:
-            if arg_name is None:
-                message = 'An error occurred while generating a flag.'
-            else:
-                message = (
-                    'An error occurred while generating a flag for argument: '
-                    f'{arg_name}'
-                )
-        self.message = message
-        self.arg_name = arg_name
-
-
-def normalize_name_to_snake_case(name: str, sep_char: str = '_') -> str:
-    """Returns the normalized name a class.
-
-    >>> normalize_name_to_snake_case('main')
-    'main'
-    >>> normalize_name_to_snake_case('MyClassName')
-    'my_class_name'
-    >>> normalize_name_to_snake_case('HelloWorld')
-    'hello_world'
-    >>> normalize_name_to_snake_case('myVar')
-    'my_var'
-    >>> normalize_name_to_snake_case("It's cool")
-    'it_s_cool'
-    >>> normalize_name_to_snake_case("test-name")
-    'test_name'
-
-    :param name: The name to normalize.
-    :param sep_char: The character that will replace space and separate words
-    :return: The normalized name.
-    """
-    for char in _string.punctuation:
-        name = name.replace(char, sep_char)
-    name = _re.sub(rf'([\s{sep_char}]+)|(([a-zA-z])([A-Z]))', rf'\3{sep_char}\4',
-                   name).lower()
-    return name
-
-
-def normalize_name(name: str, sep_char: str = '_') -> str:
-    """Returns the normalized name a class.
-
-    >>> normalize_name('main')
-    'main'
-    >>> normalize_name('MyFunction')
-    'MyFunction'
-    >>> normalize_name('HelloWorld')
-    'HelloWorld'
-    >>> normalize_name('myVar')
-    'myVar'
-    >>> normalize_name("It's cool")
-    'It_s_cool'
-    >>> normalize_name("test-name")
-    'test_name'
-
-    :param name: The name to normalize.
-    :param sep_char: The character that will replace space and separate words
-    :return: The normalized name.
-    """
-    for char in _string.punctuation:
-        name = name.replace(char, sep_char)
-    name = _re.sub(rf'([\s{sep_char}]+)', sep_char, name)
-    return name
-
-
-@_dataclass
-class Argument:
-    """Represents a function argument."""
-    name: str
-    kind: _inspect._ParameterKind
-    annotation: _Any = _inspect._empty
-    default: _Any = _inspect._empty
-    help: _Optional[str] = None
-
-    def __post_init__(self):
-        """Sets the some values to None if they are empty."""
-        if self.annotation == _inspect._empty:
-            self.annotation = None
-        if self.default == _inspect._empty:
-            self.default = None
-
-
-@_dataclass
-class FunctionInfo:
-    """Represents a function."""
-    function: Callable
-    name: str = _field(init=False)
-    arguments: _OrderedDict[str, Argument] = _field(init=False)
-    docstring: _Docstring = _field(init=False)
-    parser: _Argparse.ColorizingArgumentParser = _field(init=False)
-
-    def __post_init__(self):
-        self.name = normalize_name_to_snake_case(
-            self.function.__init__.__name__
-        ) if isinstance(self.function,
-                        type) else normalize_name(self.function.__name__)
-        self.function = self.function.__init__ if isinstance(
-            self.function, type
-        ) else self.function
-
-        self.arguments: _OrderedDict[str, Argument] = _OrderedDict()
-        for parameter in _inspect.signature(self.function).parameters.values():
-            self.arguments[parameter.name] = Argument(
-                name=parameter.name,
-                kind=parameter.kind,
-                default=parameter.default,
-                annotation=parameter.annotation,
-            )
-
-        self.docstring = _parse(self.function.__doc__ or '')
-        for parameter in self.docstring.params:
-            if parameter.arg_name in self.arguments:
-                self.arguments[parameter.arg_name].help = parameter.description
-
-
-def generate_flag(  # pylint: disable=too-many-branches
-    argument: Argument,
-    no_dash: bool = False,
-    reserved_flags: _Optional[_Set[str]] = None
-) -> _List[str]:
-    """Generates one or more flags for an argument based on its attributes.
-
-    :param argument: The argument to generate flags for.
-    :param no_dash: Whether to generate flags without dashes as
-        prefixes.
-    :param reserved_flags: A set of flags that are reserved. (Default: `RESERVED_FLAGS`)
-    :raises FlagGenerationError: If all the suitable flags are reserved.
-    :return: A list of flags for the argument.
-    """
-    if reserved_flags is None:
-        reserved_flags = RESERVED_FLAGS
-    flags: _List[str] = []
-    flag1_base = ('' if no_dash else '--')
-    flag1 = flag1_base + normalize_name_to_snake_case(argument.name, '-')
-    if flag1 in reserved_flags:
-        flag1 = flag1_base + normalize_name(argument.name, sep_char='-')
-    if flag1 in reserved_flags:
-        flag1 = flag1_base + argument.name
-    if flag1 in reserved_flags:
-        flag1 = flag1_base + normalize_name(
-            ' '.join(normalize_name_to_snake_case(argument.name, '-').split('-')
-                     ).capitalize(),
-            sep_char='-'
-        )
-    if flag1 in reserved_flags:
-        flag1 = flag1_base + normalize_name(argument.name, sep_char='-').upper()
-    if flag1 in reserved_flags:
-        if no_dash:
-            raise FlagGenerationError(
-                f"Failed to generate a flag for argument: {argument}"
-            )
-    else:
-        flags.append(flag1)
-
-    if not no_dash:
-        flag2 = '-' + argument.name[:1].lower()
-        if flag2 in reserved_flags:
-            flag2 = flag2.upper()
-        if flag2 in reserved_flags:
-            flag2 = '-' + ''.join(
-                part[:1]
-                for part in normalize_name_to_snake_case(argument.name).split('_')
-            )
-        if flag2 in reserved_flags:
-            flag2 = flag2.capitalize()
-        if flag2 in reserved_flags:
-            flag2 = flag2.upper()
-        if flag2 not in reserved_flags:
-            flags.append(flag2)
-
-    if not flags:
-        raise FlagGenerationError(f"Failed to generate a flag for argument: {argument}")
-
-    reserved_flags.update(flags)
-
-    return flags
-
-
-def _add_arguments(
-    parser: _Union[_Argparse.ColorizingArgumentParser, _Argparse._ArgumentGroup],
-    info: FunctionInfo,
-    reserved_flags: _Optional[_Set[str]] = None
-) -> None:
-    """Add the arguments to the parser.
-
-    :param parser: The parser to add the arguments to.
-    :param info: The function info.
-    :param reserved_flags: The reserved flags.
-    """
-    if reserved_flags is None:
-        reserved_flags = RESERVED_FLAGS.copy()
-    # Add the arguments
-    for argument in info.arguments.values():
-        config: _Dict[str, _Any] = {
-            'action': 'store',
-            'dest': argument.name,
-            'help': argument.help
-        }
-        if isinstance(argument.annotation, type):
-            config['type'] = argument.annotation
-        if argument.annotation == bool:
-            config['action'] = 'store_true'
-            config.pop('type')
-        if argument.kind == _inspect._ParameterKind.POSITIONAL_ONLY:
-            config['required'] = True
-        if argument.kind == _inspect._ParameterKind.VAR_POSITIONAL:
-            config['nargs'] = '*'
-        if argument.default:
-            config['default'] = argument.default
-        parser.add_argument(
-            *generate_flag(argument, reserved_flags=reserved_flags), **config
-        )
-
-
-def _argumentify_one(func: Callable):
-    """This function argumentifies one function as the entry point of the
-    script.
-
-    :param function: The function to argumentify.
-    """
-    info = FunctionInfo(func)
-
-    # Check if the function has a VAR_KEYWORD argument
-    # Raises a ArgumentTypeError if it does
-    for argument in info.arguments.values():
-        if argument.kind == _inspect._ParameterKind.VAR_KEYWORD:
-            raise ArgumentTypeError(
-                f"The function has a `**{argument.name}` argument, "
-                "which is not supported.",
-                unsupported_arg=argument.name
-            )
-
-    # Create the parser
-    parser = _Argparse.ColorizingArgumentParser(
-        description=info.docstring.short_description
-    )
-    # Add the arguments
-    _add_arguments(parser, info)
-    cli_args = parser.parse_args()
-    args = []
-    kwargs = {}
-    for argument in info.arguments.values():
-        if argument.kind in (_inspect._ParameterKind.POSITIONAL_ONLY,
-                             _inspect._ParameterKind.POSITIONAL_OR_KEYWORD):
-            args.append(getattr(cli_args, argument.name))
-        elif argument.kind == _inspect._ParameterKind.VAR_POSITIONAL:
-            args.extend(getattr(cli_args, argument.name) or [])
-        else:
-            kwargs[argument.name] = getattr(cli_args, argument.name)
-    result = func(*args, **kwargs)
-    # Check if the result is a coroutine
-    if isinstance(result, (_Coroutine, _Awaitable)):
-        _asyncio.run(result)
-
-
-def _argumentify(functions: _Dict[str, Callable]):
-    """This function argumentifies one or more functions as the entry point of
-    the script.
-
-    :param functions: A dictionary of functions to argumentify.
-    :raises RuntimeError:
-    """
-    functions_info: _Dict[str, _Tuple[Callable, FunctionInfo]] = {}
-    for name, function in functions.items():
-        functions_info[name] = (function, FunctionInfo(function))
-
-        # Check if the function has a VAR_KEYWORD argument
-        # Raises a ArgumentTypeError if it does
-        for argument in functions_info[name][1].arguments.values():
-            if argument.kind == _inspect._ParameterKind.VAR_KEYWORD:
-                raise ArgumentTypeError(
-                    f"Function {name} has `**{argument.name}` argument, "
-                    "which is not supported.",
-                    unsupported_arg=argument.name
-                )
-    parser = _Argparse.ColorizingArgumentParser()
-    subparsers = parser.add_subparsers(required=True)
-    for name, (_, info) in functions_info.items():
-        subparser = subparsers.add_parser(name, help=info.docstring.short_description)
-        _add_arguments(subparser, info)
-        subparser.set_defaults(func=info.function)
-    cli_args = parser.parse_args()
-    args = []
-    kwargs = {}
-    info = None
-    for name, (function, info) in functions_info.items():
-        if function == cli_args.func:
-            break
-    else:
-        raise RuntimeError('No function found for the given arguments.')
-    for argument in info.arguments.values():
-        if argument.kind in (_inspect._ParameterKind.POSITIONAL_ONLY,
-                             _inspect._ParameterKind.POSITIONAL_OR_KEYWORD):
-            args.append(getattr(cli_args, argument.name))
-        elif argument.kind == _inspect._ParameterKind.VAR_POSITIONAL:
-            args.extend(getattr(cli_args, argument.name) or [])
-        else:
-            kwargs[argument.name] = getattr(cli_args, argument.name)
-    result = function(*args, **kwargs)
-    # Check if the result is a coroutine
-    if isinstance(result, (_Coroutine, _Awaitable)):
-        _asyncio.run(result)
-
-
-def argumentify(entry_point: _Union[Callable, _List[Callable], _Dict[str, Callable]]):
-    """This function argumentifies one or more functions as the entry point of
-    the script.
-
-     1 #!/usr/bin/env python
-     2 # argumentified.py
-     3 from log21 import argumentify
-     4
-     5
-     6 def main(first_name: str, last_name: str, /, *, age: int = None) -> None:
-     7     if age is not None:
-     8         print(f'{first_name} {last_name} is {age} years old.')
-     9     else:
-    10         print(f'{first_name} {last_name} is not yet born.')
-    11
-    12 if __name__ == '__main__':
-    13     argumentify(main)
-
-    $ python argumentified.py Ahmad Ahmadi --age 20
-    Ahmad Ahmadi is 20 years old.
-    $ python argumentified.py Mehrad Pooryoussof
-    Mehrad Pooryoussof is not yet born.
-
-    :param entry_point: The function(s) to argumentify.
-    :raises TypeError: A function must be a function or a list of functions or a
-        dictionary of functions.
-    """
-
-    functions = {}
-    # Check the types
-    if callable(entry_point):
-        _argumentify_one(entry_point)
-        return entry_point
-    if isinstance(entry_point, _List):
-        for func in entry_point:
-            if not callable(func):
-                raise TypeError(
-                    "argumentify: func must be a function or a list of functions or a "
-                    "dictionary of functions."
-                )
-            functions[func.__name__] = func
-    elif isinstance(entry_point, _Dict):
-        for func in entry_point.values():
-            if not callable(func):
-                raise TypeError(
-                    "argumentify: func must be a function or a list of functions or a "
-                    "dictionary of functions."
-                )
-        functions = entry_point
-    else:
-        raise TypeError(
-            "argumentify: func must be a function or a list of functions or a "
-            "dictionary of functions."
-        )
-
-    _argumentify(functions)
-    return entry_point
+# log21.Argparse.py
+# CodeWriter21
+
+import re as _re
+import string as _string
+import asyncio as _asyncio
+import inspect as _inspect
+from typing import (Any as _Any, Set as _Set, Dict as _Dict, List as _List,
+                    Tuple as _Tuple, Union as _Union, Callable as _Callable,
+                    Optional as _Optional, Awaitable as _Awaitable,
+                    Coroutine as _Coroutine, OrderedDict as _OrderedDict)
+from dataclasses import field as _field, dataclass as _dataclass
+
+from docstring_parser import Docstring as _Docstring, parse as _parse
+
+import log21.Argparse as _Argparse
+
+__all__ = [
+    'argumentify', 'ArgumentifyError', 'ArgumentTypeError', 'FlagGenerationError',
+    'RESERVED_FLAGS', 'Callable', 'Argument', 'FunctionInfo', 'generate_flag',
+    'normalize_name', 'normalize_name_to_snake_case'
+]
+
+Callable = _Union[_Callable[..., _Any], _Callable[..., _Coroutine[_Any, _Any, _Any]]]
+RESERVED_FLAGS = {'--help', '-h'}
+
+
+class ArgumentifyError(Exception):
+    """Base class for exceptions in this module."""
+
+
+class ArgumentTypeError(ArgumentifyError, TypeError):
+    """Exception raised when a function has an unsupported type of argument.
+
+    e.g: a function has a VAR_KEYWORD argument.
+    """
+
+    def __init__(
+        self, message: _Optional[str] = None, unsupported_arg: _Optional[str] = None
+    ):
+        """Initialize the exception.
+
+        :param message: The message to display.
+        :param unsupported_arg: The name of the unsupported argument.
+        """
+        if message is None:
+            if unsupported_arg is None:
+                message = 'Unsupported argument type.'
+            else:
+                message = f'Unsupported argument type: {unsupported_arg}'
+        self.message = message
+        self.unsupported_arg = unsupported_arg
+
+
+class FlagGenerationError(ArgumentifyError, RuntimeError):
+    """Exception raised when an error occurs while generating a flag.
+
+    Most likely raised when there are arguments with the same name.
+    """
+
+    def __init__(self, message: _Optional[str] = None, arg_name: _Optional[str] = None):
+        """Initialize the exception.
+
+        :param message: The message to display.
+        :param arg_name: The name of the argument that caused the error.
+        """
+        if message is None:
+            if arg_name is None:
+                message = 'An error occurred while generating a flag.'
+            else:
+                message = (
+                    'An error occurred while generating a flag for argument: '
+                    f'{arg_name}'
+                )
+        self.message = message
+        self.arg_name = arg_name
+
+
+def normalize_name_to_snake_case(name: str, sep_char: str = '_') -> str:
+    """Returns the normalized name a class.
+
+    >>> normalize_name_to_snake_case('main')
+    'main'
+    >>> normalize_name_to_snake_case('MyClassName')
+    'my_class_name'
+    >>> normalize_name_to_snake_case('HelloWorld')
+    'hello_world'
+    >>> normalize_name_to_snake_case('myVar')
+    'my_var'
+    >>> normalize_name_to_snake_case("It's cool")
+    'it_s_cool'
+    >>> normalize_name_to_snake_case("test-name")
+    'test_name'
+
+    :param name: The name to normalize.
+    :param sep_char: The character that will replace space and separate words
+    :return: The normalized name.
+    """
+    for char in _string.punctuation:
+        name = name.replace(char, sep_char)
+    name = _re.sub(rf'([\s{sep_char}]+)|(([a-zA-z])([A-Z]))', rf'\3{sep_char}\4',
+                   name).lower()
+    return name
+
+
+def normalize_name(name: str, sep_char: str = '_') -> str:
+    """Returns the normalized name a class.
+
+    >>> normalize_name('main')
+    'main'
+    >>> normalize_name('MyFunction')
+    'MyFunction'
+    >>> normalize_name('HelloWorld')
+    'HelloWorld'
+    >>> normalize_name('myVar')
+    'myVar'
+    >>> normalize_name("It's cool")
+    'It_s_cool'
+    >>> normalize_name("test-name")
+    'test_name'
+
+    :param name: The name to normalize.
+    :param sep_char: The character that will replace space and separate words
+    :return: The normalized name.
+    """
+    for char in _string.punctuation:
+        name = name.replace(char, sep_char)
+    name = _re.sub(rf'([\s{sep_char}]+)', sep_char, name)
+    return name
+
+
+@_dataclass
+class Argument:
+    """Represents a function argument."""
+    name: str
+    kind: _inspect._ParameterKind
+    annotation: _Any = _inspect._empty
+    default: _Any = _inspect._empty
+    help: _Optional[str] = None
+
+    def __post_init__(self):
+        """Sets the some values to None if they are empty."""
+        if self.annotation == _inspect._empty:
+            self.annotation = None
+        if self.default == _inspect._empty:
+            self.default = None
+
+
+@_dataclass
+class FunctionInfo:
+    """Represents a function."""
+    function: Callable
+    name: str = _field(init=False)
+    arguments: _OrderedDict[str, Argument] = _field(init=False)
+    docstring: _Docstring = _field(init=False)
+    parser: _Argparse.ColorizingArgumentParser = _field(init=False)
+
+    def __post_init__(self):
+        self.name = normalize_name_to_snake_case(
+            self.function.__init__.__name__
+        ) if isinstance(self.function,
+                        type) else normalize_name(self.function.__name__)
+        self.function = self.function.__init__ if isinstance(
+            self.function, type
+        ) else self.function
+
+        self.arguments: _OrderedDict[str, Argument] = _OrderedDict()
+        for parameter in _inspect.signature(self.function).parameters.values():
+            self.arguments[parameter.name] = Argument(
+                name=parameter.name,
+                kind=parameter.kind,
+                default=parameter.default,
+                annotation=parameter.annotation,
+            )
+
+        self.docstring = _parse(self.function.__doc__ or '')
+        for parameter in self.docstring.params:
+            if parameter.arg_name in self.arguments:
+                self.arguments[parameter.arg_name].help = parameter.description
+
+
+def generate_flag(  # pylint: disable=too-many-branches
+    argument: Argument,
+    no_dash: bool = False,
+    reserved_flags: _Optional[_Set[str]] = None
+) -> _List[str]:
+    """Generates one or more flags for an argument based on its attributes.
+
+    :param argument: The argument to generate flags for.
+    :param no_dash: Whether to generate flags without dashes as
+        prefixes.
+    :param reserved_flags: A set of flags that are reserved. (Default: `RESERVED_FLAGS`)
+    :raises FlagGenerationError: If all the suitable flags are reserved.
+    :return: A list of flags for the argument.
+    """
+    if reserved_flags is None:
+        reserved_flags = RESERVED_FLAGS
+    flags: _List[str] = []
+    flag1_base = ('' if no_dash else '--')
+    flag1 = flag1_base + normalize_name_to_snake_case(argument.name, '-')
+    if flag1 in reserved_flags:
+        flag1 = flag1_base + normalize_name(argument.name, sep_char='-')
+    if flag1 in reserved_flags:
+        flag1 = flag1_base + argument.name
+    if flag1 in reserved_flags:
+        flag1 = flag1_base + normalize_name(
+            ' '.join(normalize_name_to_snake_case(argument.name, '-').split('-')
+                     ).capitalize(),
+            sep_char='-'
+        )
+    if flag1 in reserved_flags:
+        flag1 = flag1_base + normalize_name(argument.name, sep_char='-').upper()
+    if flag1 in reserved_flags:
+        if no_dash:
+            raise FlagGenerationError(
+                f"Failed to generate a flag for argument: {argument}"
+            )
+    else:
+        flags.append(flag1)
+
+    if not no_dash:
+        flag2 = '-' + argument.name[:1].lower()
+        if flag2 in reserved_flags:
+            flag2 = flag2.upper()
+        if flag2 in reserved_flags:
+            flag2 = '-' + ''.join(
+                part[:1]
+                for part in normalize_name_to_snake_case(argument.name).split('_')
+            )
+        if flag2 in reserved_flags:
+            flag2 = flag2.capitalize()
+        if flag2 in reserved_flags:
+            flag2 = flag2.upper()
+        if flag2 not in reserved_flags:
+            flags.append(flag2)
+
+    if not flags:
+        raise FlagGenerationError(f"Failed to generate a flag for argument: {argument}")
+
+    reserved_flags.update(flags)
+
+    return flags
+
+
+def _add_arguments(
+    parser: _Union[_Argparse.ColorizingArgumentParser, _Argparse._ArgumentGroup],
+    info: FunctionInfo,
+    reserved_flags: _Optional[_Set[str]] = None
+) -> None:
+    """Add the arguments to the parser.
+
+    :param parser: The parser to add the arguments to.
+    :param info: The function info.
+    :param reserved_flags: The reserved flags.
+    """
+    if reserved_flags is None:
+        reserved_flags = RESERVED_FLAGS.copy()
+    # Add the arguments
+    for argument in info.arguments.values():
+        config: _Dict[str, _Any] = {
+            'action': 'store',
+            'dest': argument.name,
+            'help': argument.help
+        }
+        if isinstance(argument.annotation, type):
+            config['type'] = argument.annotation
+        if argument.annotation == bool:
+            config['action'] = 'store_true'
+            config.pop('type')
+        if argument.kind == _inspect._ParameterKind.POSITIONAL_ONLY:
+            config['required'] = True
+        if argument.kind == _inspect._ParameterKind.VAR_POSITIONAL:
+            config['nargs'] = '*'
+        if argument.default:
+            config['default'] = argument.default
+        parser.add_argument(
+            *generate_flag(argument, reserved_flags=reserved_flags), **config
+        )
+
+
+def _argumentify_one(func: Callable):
+    """This function argumentifies one function as the entry point of the
+    script.
+
+    :param function: The function to argumentify.
+    """
+    info = FunctionInfo(func)
+
+    # Check if the function has a VAR_KEYWORD argument
+    # Raises a ArgumentTypeError if it does
+    for argument in info.arguments.values():
+        if argument.kind == _inspect._ParameterKind.VAR_KEYWORD:
+            raise ArgumentTypeError(
+                f"The function has a `**{argument.name}` argument, "
+                "which is not supported.",
+                unsupported_arg=argument.name
+            )
+
+    # Create the parser
+    parser = _Argparse.ColorizingArgumentParser(
+        description=info.docstring.short_description
+    )
+    # Add the arguments
+    _add_arguments(parser, info)
+    cli_args = parser.parse_args()
+    args = []
+    kwargs = {}
+    for argument in info.arguments.values():
+        if argument.kind in (_inspect._ParameterKind.POSITIONAL_ONLY,
+                             _inspect._ParameterKind.POSITIONAL_OR_KEYWORD):
+            args.append(getattr(cli_args, argument.name))
+        elif argument.kind == _inspect._ParameterKind.VAR_POSITIONAL:
+            args.extend(getattr(cli_args, argument.name) or [])
+        else:
+            kwargs[argument.name] = getattr(cli_args, argument.name)
+    result = func(*args, **kwargs)
+    # Check if the result is a coroutine
+    if isinstance(result, (_Coroutine, _Awaitable)):
+        _asyncio.run(result)
+
+
+def _argumentify(functions: _Dict[str, Callable]):
+    """This function argumentifies one or more functions as the entry point of
+    the script.
+
+    :param functions: A dictionary of functions to argumentify.
+    :raises RuntimeError:
+    """
+    functions_info: _Dict[str, _Tuple[Callable, FunctionInfo]] = {}
+    for name, function in functions.items():
+        functions_info[name] = (function, FunctionInfo(function))
+
+        # Check if the function has a VAR_KEYWORD argument
+        # Raises a ArgumentTypeError if it does
+        for argument in functions_info[name][1].arguments.values():
+            if argument.kind == _inspect._ParameterKind.VAR_KEYWORD:
+                raise ArgumentTypeError(
+                    f"Function {name} has `**{argument.name}` argument, "
+                    "which is not supported.",
+                    unsupported_arg=argument.name
+                )
+    parser = _Argparse.ColorizingArgumentParser()
+    subparsers = parser.add_subparsers(required=True)
+    for name, (_, info) in functions_info.items():
+        subparser = subparsers.add_parser(name, help=info.docstring.short_description)
+        _add_arguments(subparser, info)
+        subparser.set_defaults(func=info.function)
+    cli_args = parser.parse_args()
+    args = []
+    kwargs = {}
+    info = None
+    for name, (function, info) in functions_info.items():
+        if function == cli_args.func:
+            break
+    else:
+        raise RuntimeError('No function found for the given arguments.')
+    for argument in info.arguments.values():
+        if argument.kind in (_inspect._ParameterKind.POSITIONAL_ONLY,
+                             _inspect._ParameterKind.POSITIONAL_OR_KEYWORD):
+            args.append(getattr(cli_args, argument.name))
+        elif argument.kind == _inspect._ParameterKind.VAR_POSITIONAL:
+            args.extend(getattr(cli_args, argument.name) or [])
+        else:
+            kwargs[argument.name] = getattr(cli_args, argument.name)
+    result = function(*args, **kwargs)
+    # Check if the result is a coroutine
+    if isinstance(result, (_Coroutine, _Awaitable)):
+        _asyncio.run(result)
+
+
+def argumentify(entry_point: _Union[Callable, _List[Callable], _Dict[str, Callable]]):
+    """This function argumentifies one or more functions as the entry point of
+    the script.
+
+     1 #!/usr/bin/env python
+     2 # argumentified.py
+     3 from log21 import argumentify
+     4
+     5
+     6 def main(first_name: str, last_name: str, /, *, age: int = None) -> None:
+     7     if age is not None:
+     8         print(f'{first_name} {last_name} is {age} years old.')
+     9     else:
+    10         print(f'{first_name} {last_name} is not yet born.')
+    11
+    12 if __name__ == '__main__':
+    13     argumentify(main)
+
+    $ python argumentified.py Ahmad Ahmadi --age 20
+    Ahmad Ahmadi is 20 years old.
+    $ python argumentified.py Mehrad Pooryoussof
+    Mehrad Pooryoussof is not yet born.
+
+    :param entry_point: The function(s) to argumentify.
+    :raises TypeError: A function must be a function or a list of functions or a
+        dictionary of functions.
+    """
+
+    functions = {}
+    # Check the types
+    if callable(entry_point):
+        _argumentify_one(entry_point)
+        return entry_point
+    if isinstance(entry_point, _List):
+        for func in entry_point:
+            if not callable(func):
+                raise TypeError(
+                    "argumentify: func must be a function or a list of functions or a "
+                    "dictionary of functions."
+                )
+            functions[func.__name__] = func
+    elif isinstance(entry_point, _Dict):
+        for func in entry_point.values():
+            if not callable(func):
+                raise TypeError(
+                    "argumentify: func must be a function or a list of functions or a "
+                    "dictionary of functions."
+                )
+        functions = entry_point
+    else:
+        raise TypeError(
+            "argumentify: func must be a function or a list of functions or a "
+            "dictionary of functions."
+        )
+
+    _argumentify(functions)
+    return entry_point
```

### Comparing `log21-2.8.1b0/src/log21/Colors.py` & `log21-2.9.0/src/log21/Colors.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,359 +1,359 @@
-# log21.Colors.py
-# CodeWriter21
-
-import re as _re
-from typing import Union as _Union, Sequence as _Sequence
-
-import webcolors as _webcolors
-
-__all__ = [
-    'Colors', 'get_color', 'get_colors', 'ansi_escape', 'get_color_name',
-    'closest_color', 'hex_escape', 'RESET', 'BLACK', 'RED', 'GREEN', 'YELLOW',
-    'BLUE', 'MAGENTA', 'CYAN', 'WHITE', 'BACK_BLACK', 'BACK_RED', 'BACK_GREEN',
-    'BACK_YELLOW', 'BACK_BLUE', 'BACK_MAGENTA', 'BACK_CYAN', 'BACK_WHITE',
-    'GREY', 'LIGHT_RED', 'LIGHT_GREEN', 'LIGHT_YELLOW', 'LIGHT_BLUE',
-    'LIGHT_MAGENTA', 'LIGHT_CYAN', 'LIGHT_WHITE', 'BACK_GREY', 'BACK_LIGHT_RED',
-    'BACK_LIGHT_GREEN', 'BACK_LIGHT_YELLOW', 'BACK_LIGHT_BLUE',
-    'BACK_LIGHT_MAGENTA', 'BACK_LIGHT_CYAN', 'BACK_LIGHT_WHITE'
-]
-
-# Regex pattern to find ansi colors in message
-ansi_escape = _re.compile(r'\x1b\[((?:\d+)(?:;(?:\d+))*)m')
-hex_escape = _re.compile(r'\x1b(#[0-9a-fA-F]{6})h([f|b])')
-
-RESET = '\033[0m'
-BLACK = '\033[30m'
-RED = '\033[31m'
-GREEN = '\033[32m'
-YELLOW = '\033[33m'
-BLUE = '\033[34m'
-MAGENTA = '\033[35m'
-CYAN = '\033[36m'
-WHITE = '\033[37m'
-BACK_BLACK = '\033[40m'
-BACK_RED = '\033[41m'
-BACK_GREEN = '\033[42m'
-BACK_YELLOW = '\033[43m'
-BACK_BLUE = '\033[44m'
-BACK_MAGENTA = '\033[45m'
-BACK_CYAN = '\033[46m'
-BACK_WHITE = '\033[47m'
-GREY = '\033[90m'
-LIGHT_RED = '\033[91m'
-LIGHT_GREEN = '\033[92m'
-LIGHT_YELLOW = '\033[93m'
-LIGHT_BLUE = '\033[94m'
-LIGHT_MAGENTA = '\033[95m'
-LIGHT_CYAN = '\033[96m'
-LIGHT_WHITE = '\033[97m'
-BACK_GREY = '\033[100m'
-BACK_LIGHT_RED = '\033[101m'
-BACK_LIGHT_GREEN = '\033[102m'
-BACK_LIGHT_YELLOW = '\033[103m'
-BACK_LIGHT_BLUE = '\033[104m'
-BACK_LIGHT_MAGENTA = '\033[105m'
-BACK_LIGHT_CYAN = '\033[106m'
-BACK_LIGHT_WHITE = '\033[107m'
-
-
-class Colors:
-    """A class containing color-maps."""
-    color_map = {
-        'Reset': RESET,
-        'Black': BLACK,
-        'Red': RED,
-        'Green': GREEN,
-        'Yellow': YELLOW,
-        'Blue': BLUE,
-        'Magenta': MAGENTA,
-        'Cyan': CYAN,
-        'White': WHITE,
-        'BackBlack': BACK_BLACK,
-        'BackRed': BACK_RED,
-        'BackGreen': BACK_GREEN,
-        'BackYellow': BACK_YELLOW,
-        'BackBlue': BACK_BLUE,
-        'BackMagenta': BACK_MAGENTA,
-        'BackCyan': BACK_CYAN,
-        'BackWhite': BACK_WHITE,
-        'Grey': GREY,
-        'LightRed': LIGHT_RED,
-        'LightGreen': LIGHT_GREEN,
-        'LightYellow': LIGHT_YELLOW,
-        'LightBlue': LIGHT_BLUE,
-        'LightMagenta': LIGHT_MAGENTA,
-        'LightCyan': LIGHT_CYAN,
-        'LightWhite': LIGHT_WHITE,
-        'BackGrey': BACK_GREY,
-        'BackLightRed': BACK_LIGHT_RED,
-        'BackLightGreen': BACK_LIGHT_GREEN,
-        'BackLightYellow': BACK_LIGHT_YELLOW,
-        'BackLightBlue': BACK_LIGHT_BLUE,
-        'BackLightMagenta': BACK_LIGHT_MAGENTA,
-        'BackLightCyan': BACK_LIGHT_CYAN,
-        'BackLightWhite': BACK_LIGHT_WHITE,
-    }
-    color_map_ = {
-        'reset': RESET,
-        'black': BLACK,
-        'red': RED,
-        'green': GREEN,
-        'yellow': YELLOW,
-        'blue': BLUE,
-        'magenta': MAGENTA,
-        'cyan': CYAN,
-        'white': WHITE,
-        'backblack': BACK_BLACK,
-        'backred': BACK_RED,
-        'backgreen': BACK_GREEN,
-        'backyellow': BACK_YELLOW,
-        'backblue': BACK_BLUE,
-        'backmagenta': BACK_MAGENTA,
-        'backcyan': BACK_CYAN,
-        'backwhite': BACK_WHITE,
-        'grey': GREY,
-        'gray': GREY,
-        'lightred': LIGHT_RED,
-        'lightgreen': LIGHT_GREEN,
-        'lightyellow': LIGHT_YELLOW,
-        'lightblue': LIGHT_BLUE,
-        'lightmagenta': LIGHT_MAGENTA,
-        'lightcyan': LIGHT_CYAN,
-        'lightwhite': LIGHT_WHITE,
-        'backgrey': BACK_GREY,
-        'backlightred': BACK_LIGHT_RED,
-        'backlightgreen': BACK_LIGHT_GREEN,
-        'backlightyellow': BACK_LIGHT_YELLOW,
-        'backlightblue': BACK_LIGHT_BLUE,
-        'backlightmagenta': BACK_LIGHT_MAGENTA,
-        'backlightcyan': BACK_LIGHT_CYAN,
-        'backlightwhite': BACK_LIGHT_WHITE,
-        'brightblack': GREY,
-        'brightred': LIGHT_RED,
-        'brightgreen': LIGHT_GREEN,
-        'brightyellow': LIGHT_YELLOW,
-        'brightblue': LIGHT_BLUE,
-        'brightmagenta': LIGHT_MAGENTA,
-        'brightcyan': LIGHT_CYAN,
-        'brightwhite': LIGHT_WHITE,
-        'backbrightblack': BACK_GREY,
-        'backbrightred': BACK_LIGHT_RED,
-        'backbrightgreen': BACK_LIGHT_GREEN,
-        'backbrightyellow': BACK_LIGHT_YELLOW,
-        'backbrightblue': BACK_LIGHT_BLUE,
-        'backbrightmagenta': BACK_LIGHT_MAGENTA,
-        'backbrightcyan': BACK_LIGHT_CYAN,
-        'backbrightwhite': BACK_LIGHT_WHITE,
-        'rst': RESET,
-        'bk': BLACK,
-        'r': RED,
-        'g': GREEN,
-        'y': YELLOW,
-        'b': BLUE,
-        'm': MAGENTA,
-        'c': CYAN,
-        'w': WHITE,
-        'bbk': BACK_BLACK,
-        'br': BACK_RED,
-        'bg': BACK_GREEN,
-        'by': BACK_YELLOW,
-        'bb': BACK_BLUE,
-        'bm': BACK_MAGENTA,
-        'bc': BACK_CYAN,
-        'bw': BACK_WHITE,
-        'gr': GREY,
-        'lr': LIGHT_RED,
-        'lg': LIGHT_GREEN,
-        'ly': LIGHT_YELLOW,
-        'lb': LIGHT_BLUE,
-        'lm': LIGHT_MAGENTA,
-        'lc': LIGHT_CYAN,
-        'lw': LIGHT_WHITE,
-        'bgr': BACK_GREY,
-        'blr': BACK_LIGHT_RED,
-        'blg': BACK_LIGHT_GREEN,
-        'bly': BACK_LIGHT_YELLOW,
-        'blb': BACK_LIGHT_BLUE,
-        'blm': BACK_LIGHT_MAGENTA,
-        'blc': BACK_LIGHT_CYAN,
-        'blw': BACK_LIGHT_WHITE,
-    }
-    change_map = {
-        'aqua': 'LightCyan',
-        'blue': 'LightBlue',
-        'fuchsia': 'LightMagenta',
-        'lime': 'LightGreen',
-        'maroon': 'Red',
-        'navy': 'Blue',
-        'olive': 'Yellow',
-        'purple': 'Magenta',
-        'red': 'LightRed',
-        'silver': 'Grey',
-        'teal': 'Cyan',
-        'white': 'BrightWhite',
-        'yellow': 'LightYellow',
-    }
-
-
-def closest_color(requested_color: _Sequence[int]):
-    """
-    Takes a color in RGB and returns the name of the closest color to the value.
-    Uses the `webcolors.CSS2_HEX_TO_NAMES` dictionary to find the closest color.
-
-    :param requested_color: Sequence[int, int, int]: The input color in RGB.
-    :return: str: The name of the closest color.
-    """
-    min_colors = {}
-    for key, name in _webcolors.CSS2_HEX_TO_NAMES.items():
-        r_c, g_c, b_c = _webcolors.hex_to_rgb(key)
-        r_d = (r_c - requested_color[0])**2
-        g_d = (g_c - requested_color[1])**2
-        b_d = (b_c - requested_color[2])**2
-        min_colors[(r_d + g_d + b_d)] = name
-    return min_colors[min(min_colors.keys())]
-
-
-def get_color_name(
-    color: _Union[str, _Sequence[int], _webcolors.IntegerRGB,
-                  _webcolors.HTML5SimpleColor],
-    raise_exceptions: bool = False
-) -> str:
-    """
-    Takes a color in RGB format and returns a color name close to the RGB value.
-
-    >>>
-    >>> get_color_name('#00FF00')
-    'LightGreen'
-    >>>
-    >>> get_color_name((128, 0, 128))
-    'Magenta'
-    >>>
-
-    :param color: Union[str, Sequence[int]: The input color. Example: '#00FF00',
-        (128, 0, 128)
-    :param raise_exceptions: bool = False: Returns empty string when raise_exceptions is
-        False and an error occurs.
-    :raises TypeError
-    :return: str: The color name.
-    """
-    # Makes sure that the input parameters has valid values.
-    if not isinstance(color,
-                      (str, tuple, _webcolors.IntegerRGB, _webcolors.HTML5SimpleColor)):
-        if raise_exceptions:
-            raise TypeError(
-                'Input color must be a str or Tuple[int, int, int] or '
-                'webcolors.IntegerRGB or webcolors.HTML5SimpleColor'
-            )
-        return ''
-    if isinstance(color, str):
-        if color.startswith('#') and len(color) == 7:
-            color = _webcolors.hex_to_rgb(color)
-        elif color.isdigit() and len(color) == 9:
-            color = (int(color[:3]), int(color[3:6]), int(color[6:9]))
-        else:
-            if raise_exceptions:
-                raise TypeError('String color format must be `#0021ff` or `000033255`!')
-            return ''
-    if isinstance(color, _Sequence):
-        if len(color) == 3:
-            if not (isinstance(color[0], int) and isinstance(color[1], int)
-                    and isinstance(color[2], int)):
-                if raise_exceptions:
-                    raise TypeError('Color sequence format must be (int, int, int)!')
-                return ''
-        else:
-            if raise_exceptions:
-                raise TypeError('Color sequence format must be (int, int, int)!')
-            return ''
-
-    # Looks for the name of the input RGB color.
-    try:
-        closest_name = _webcolors.rgb_to_name(tuple(color))
-    except ValueError:
-        closest_name = closest_color(color)
-    if closest_name in Colors.change_map:
-        closest_name = Colors.change_map[closest_name]
-    return closest_name
-
-
-def get_color(color: _Union[str, _Sequence], raise_exceptions: bool = False) -> str:
-    """Gets a color name and returns it in ansi format
-
-    >>>
-    >>> get_color('LightRed')
-    '\x1b[91m'
-    >>>
-    >>> import log21
-    >>> log21.get_logger().info(log21.get_color('Blue') + 'Hello World!')
-    [21:21:21] [INFO] Hello World!
-    >>> # Note that you must run it yourself to see the colorful result ;D
-    >>>
-
-    :param color: color name(Example: Blue)
-    :param raise_exceptions: bool = False:
-        False: It will return '' instead of raising exceptions when an error occurs.
-        True: It may raise TypeError or KeyError
-    :raises TypeError: `color` must be str
-    :raises KeyError: `color` not found!
-    :return: str: an ansi color
-    """
-    if not isinstance(color, (str, _Sequence)):
-        if raise_exceptions:
-            raise TypeError('`color` must be str or Sequence!')
-        return ''
-    if isinstance(color, _Sequence) and not isinstance(color, str):
-        color = get_color_name(color)
-        return get_color(color)
-
-    color = color.lower()
-    color = color.replace(' ', '').replace('_', '').replace('-', '')
-    color = color.replace('foreground', '').replace('fore', '').replace('ground', '')
-    if (color.startswith('#') and len(color) == 7) or (color.isdigit()
-                                                       and len(color) == 9):
-        color = get_color_name(color)
-        return get_color(color)
-    if color in Colors.color_map_:
-        return Colors.color_map_[color]
-    if ansi_escape.match(color):
-        return ansi_escape.match(color).group()
-    if color in Colors.change_map:
-        return get_color(Colors.change_map[color])
-    if raise_exceptions:
-        raise KeyError(f'`{color}` not found!')
-    return ''
-
-
-def get_colors(*colors: str, raise_exceptions: bool = False) -> str:
-    """Gets a list of colors and combines them into one.
-
-    >>>
-    >>> get_colors('LightCyan')
-    '\x1b[96m'
-    >>>
-    >>> import log21
-    >>> log21.get_logger().info(log21.get_colors('Green', 'Background White') +
-    ... 'Hello World!')
-    [21:21:21] [INFO] Hello World!
-    >>> # Note that you must run it yourself to see the colorful result ;D
-    >>>
-
-    :param colors: Input colors
-    :param raise_exceptions: bool = False:
-        False: It will return '' instead of raising exceptions when an error occurs.
-        True: It may raise TypeError or KeyError
-    :raises TypeError: `color` must be str
-    :raises KeyError: `color` not found!
-    :return: str: a combined color
-    """
-    output = ''
-    for color in colors:
-        output += get_color(str(color), raise_exceptions=raise_exceptions)
-    parts = ansi_escape.split(output)
-    output = '\033['
-    for part in parts:
-        if part:
-            output += part + ';'
-    if output.endswith(';'):
-        output = output[:-1] + 'm'
-        return output
-    return ''
+# log21.Colors.py
+# CodeWriter21
+
+import re as _re
+from typing import Union as _Union, Sequence as _Sequence
+
+import webcolors as _webcolors
+
+__all__ = [
+    'Colors', 'get_color', 'get_colors', 'ansi_escape', 'get_color_name',
+    'closest_color', 'hex_escape', 'RESET', 'BLACK', 'RED', 'GREEN', 'YELLOW',
+    'BLUE', 'MAGENTA', 'CYAN', 'WHITE', 'BACK_BLACK', 'BACK_RED', 'BACK_GREEN',
+    'BACK_YELLOW', 'BACK_BLUE', 'BACK_MAGENTA', 'BACK_CYAN', 'BACK_WHITE',
+    'GREY', 'LIGHT_RED', 'LIGHT_GREEN', 'LIGHT_YELLOW', 'LIGHT_BLUE',
+    'LIGHT_MAGENTA', 'LIGHT_CYAN', 'LIGHT_WHITE', 'BACK_GREY', 'BACK_LIGHT_RED',
+    'BACK_LIGHT_GREEN', 'BACK_LIGHT_YELLOW', 'BACK_LIGHT_BLUE',
+    'BACK_LIGHT_MAGENTA', 'BACK_LIGHT_CYAN', 'BACK_LIGHT_WHITE'
+]
+
+# Regex pattern to find ansi colors in message
+ansi_escape = _re.compile(r'\x1b\[((?:\d+)(?:;(?:\d+))*)m')
+hex_escape = _re.compile(r'\x1b(#[0-9a-fA-F]{6})h([f|b])')
+
+RESET = '\033[0m'
+BLACK = '\033[30m'
+RED = '\033[31m'
+GREEN = '\033[32m'
+YELLOW = '\033[33m'
+BLUE = '\033[34m'
+MAGENTA = '\033[35m'
+CYAN = '\033[36m'
+WHITE = '\033[37m'
+BACK_BLACK = '\033[40m'
+BACK_RED = '\033[41m'
+BACK_GREEN = '\033[42m'
+BACK_YELLOW = '\033[43m'
+BACK_BLUE = '\033[44m'
+BACK_MAGENTA = '\033[45m'
+BACK_CYAN = '\033[46m'
+BACK_WHITE = '\033[47m'
+GREY = '\033[90m'
+LIGHT_RED = '\033[91m'
+LIGHT_GREEN = '\033[92m'
+LIGHT_YELLOW = '\033[93m'
+LIGHT_BLUE = '\033[94m'
+LIGHT_MAGENTA = '\033[95m'
+LIGHT_CYAN = '\033[96m'
+LIGHT_WHITE = '\033[97m'
+BACK_GREY = '\033[100m'
+BACK_LIGHT_RED = '\033[101m'
+BACK_LIGHT_GREEN = '\033[102m'
+BACK_LIGHT_YELLOW = '\033[103m'
+BACK_LIGHT_BLUE = '\033[104m'
+BACK_LIGHT_MAGENTA = '\033[105m'
+BACK_LIGHT_CYAN = '\033[106m'
+BACK_LIGHT_WHITE = '\033[107m'
+
+
+class Colors:
+    """A class containing color-maps."""
+    color_map = {
+        'Reset': RESET,
+        'Black': BLACK,
+        'Red': RED,
+        'Green': GREEN,
+        'Yellow': YELLOW,
+        'Blue': BLUE,
+        'Magenta': MAGENTA,
+        'Cyan': CYAN,
+        'White': WHITE,
+        'BackBlack': BACK_BLACK,
+        'BackRed': BACK_RED,
+        'BackGreen': BACK_GREEN,
+        'BackYellow': BACK_YELLOW,
+        'BackBlue': BACK_BLUE,
+        'BackMagenta': BACK_MAGENTA,
+        'BackCyan': BACK_CYAN,
+        'BackWhite': BACK_WHITE,
+        'Grey': GREY,
+        'LightRed': LIGHT_RED,
+        'LightGreen': LIGHT_GREEN,
+        'LightYellow': LIGHT_YELLOW,
+        'LightBlue': LIGHT_BLUE,
+        'LightMagenta': LIGHT_MAGENTA,
+        'LightCyan': LIGHT_CYAN,
+        'LightWhite': LIGHT_WHITE,
+        'BackGrey': BACK_GREY,
+        'BackLightRed': BACK_LIGHT_RED,
+        'BackLightGreen': BACK_LIGHT_GREEN,
+        'BackLightYellow': BACK_LIGHT_YELLOW,
+        'BackLightBlue': BACK_LIGHT_BLUE,
+        'BackLightMagenta': BACK_LIGHT_MAGENTA,
+        'BackLightCyan': BACK_LIGHT_CYAN,
+        'BackLightWhite': BACK_LIGHT_WHITE,
+    }
+    color_map_ = {
+        'reset': RESET,
+        'black': BLACK,
+        'red': RED,
+        'green': GREEN,
+        'yellow': YELLOW,
+        'blue': BLUE,
+        'magenta': MAGENTA,
+        'cyan': CYAN,
+        'white': WHITE,
+        'backblack': BACK_BLACK,
+        'backred': BACK_RED,
+        'backgreen': BACK_GREEN,
+        'backyellow': BACK_YELLOW,
+        'backblue': BACK_BLUE,
+        'backmagenta': BACK_MAGENTA,
+        'backcyan': BACK_CYAN,
+        'backwhite': BACK_WHITE,
+        'grey': GREY,
+        'gray': GREY,
+        'lightred': LIGHT_RED,
+        'lightgreen': LIGHT_GREEN,
+        'lightyellow': LIGHT_YELLOW,
+        'lightblue': LIGHT_BLUE,
+        'lightmagenta': LIGHT_MAGENTA,
+        'lightcyan': LIGHT_CYAN,
+        'lightwhite': LIGHT_WHITE,
+        'backgrey': BACK_GREY,
+        'backlightred': BACK_LIGHT_RED,
+        'backlightgreen': BACK_LIGHT_GREEN,
+        'backlightyellow': BACK_LIGHT_YELLOW,
+        'backlightblue': BACK_LIGHT_BLUE,
+        'backlightmagenta': BACK_LIGHT_MAGENTA,
+        'backlightcyan': BACK_LIGHT_CYAN,
+        'backlightwhite': BACK_LIGHT_WHITE,
+        'brightblack': GREY,
+        'brightred': LIGHT_RED,
+        'brightgreen': LIGHT_GREEN,
+        'brightyellow': LIGHT_YELLOW,
+        'brightblue': LIGHT_BLUE,
+        'brightmagenta': LIGHT_MAGENTA,
+        'brightcyan': LIGHT_CYAN,
+        'brightwhite': LIGHT_WHITE,
+        'backbrightblack': BACK_GREY,
+        'backbrightred': BACK_LIGHT_RED,
+        'backbrightgreen': BACK_LIGHT_GREEN,
+        'backbrightyellow': BACK_LIGHT_YELLOW,
+        'backbrightblue': BACK_LIGHT_BLUE,
+        'backbrightmagenta': BACK_LIGHT_MAGENTA,
+        'backbrightcyan': BACK_LIGHT_CYAN,
+        'backbrightwhite': BACK_LIGHT_WHITE,
+        'rst': RESET,
+        'bk': BLACK,
+        'r': RED,
+        'g': GREEN,
+        'y': YELLOW,
+        'b': BLUE,
+        'm': MAGENTA,
+        'c': CYAN,
+        'w': WHITE,
+        'bbk': BACK_BLACK,
+        'br': BACK_RED,
+        'bg': BACK_GREEN,
+        'by': BACK_YELLOW,
+        'bb': BACK_BLUE,
+        'bm': BACK_MAGENTA,
+        'bc': BACK_CYAN,
+        'bw': BACK_WHITE,
+        'gr': GREY,
+        'lr': LIGHT_RED,
+        'lg': LIGHT_GREEN,
+        'ly': LIGHT_YELLOW,
+        'lb': LIGHT_BLUE,
+        'lm': LIGHT_MAGENTA,
+        'lc': LIGHT_CYAN,
+        'lw': LIGHT_WHITE,
+        'bgr': BACK_GREY,
+        'blr': BACK_LIGHT_RED,
+        'blg': BACK_LIGHT_GREEN,
+        'bly': BACK_LIGHT_YELLOW,
+        'blb': BACK_LIGHT_BLUE,
+        'blm': BACK_LIGHT_MAGENTA,
+        'blc': BACK_LIGHT_CYAN,
+        'blw': BACK_LIGHT_WHITE,
+    }
+    change_map = {
+        'aqua': 'LightCyan',
+        'blue': 'LightBlue',
+        'fuchsia': 'LightMagenta',
+        'lime': 'LightGreen',
+        'maroon': 'Red',
+        'navy': 'Blue',
+        'olive': 'Yellow',
+        'purple': 'Magenta',
+        'red': 'LightRed',
+        'silver': 'Grey',
+        'teal': 'Cyan',
+        'white': 'BrightWhite',
+        'yellow': 'LightYellow',
+    }
+
+
+def closest_color(requested_color: _Sequence[int]):
+    """
+    Takes a color in RGB and returns the name of the closest color to the value.
+    Uses the `webcolors.CSS2_HEX_TO_NAMES` dictionary to find the closest color.
+
+    :param requested_color: Sequence[int, int, int]: The input color in RGB.
+    :return: str: The name of the closest color.
+    """
+    min_colors = {}
+    for key, name in _webcolors.CSS2_HEX_TO_NAMES.items():
+        r_c, g_c, b_c = _webcolors.hex_to_rgb(key)
+        r_d = (r_c - requested_color[0])**2
+        g_d = (g_c - requested_color[1])**2
+        b_d = (b_c - requested_color[2])**2
+        min_colors[(r_d + g_d + b_d)] = name
+    return min_colors[min(min_colors.keys())]
+
+
+def get_color_name(
+    color: _Union[str, _Sequence[int], _webcolors.IntegerRGB,
+                  _webcolors.HTML5SimpleColor],
+    raise_exceptions: bool = False
+) -> str:
+    """
+    Takes a color in RGB format and returns a color name close to the RGB value.
+
+    >>>
+    >>> get_color_name('#00FF00')
+    'LightGreen'
+    >>>
+    >>> get_color_name((128, 0, 128))
+    'Magenta'
+    >>>
+
+    :param color: Union[str, Sequence[int]: The input color. Example: '#00FF00',
+        (128, 0, 128)
+    :param raise_exceptions: bool = False: Returns empty string when raise_exceptions is
+        False and an error occurs.
+    :raises TypeError
+    :return: str: The color name.
+    """
+    # Makes sure that the input parameters has valid values.
+    if not isinstance(color,
+                      (str, tuple, _webcolors.IntegerRGB, _webcolors.HTML5SimpleColor)):
+        if raise_exceptions:
+            raise TypeError(
+                'Input color must be a str or Tuple[int, int, int] or '
+                'webcolors.IntegerRGB or webcolors.HTML5SimpleColor'
+            )
+        return ''
+    if isinstance(color, str):
+        if color.startswith('#') and len(color) == 7:
+            color = _webcolors.hex_to_rgb(color)
+        elif color.isdigit() and len(color) == 9:
+            color = (int(color[:3]), int(color[3:6]), int(color[6:9]))
+        else:
+            if raise_exceptions:
+                raise TypeError('String color format must be `#0021ff` or `000033255`!')
+            return ''
+    if isinstance(color, _Sequence):
+        if len(color) == 3:
+            if not (isinstance(color[0], int) and isinstance(color[1], int)
+                    and isinstance(color[2], int)):
+                if raise_exceptions:
+                    raise TypeError('Color sequence format must be (int, int, int)!')
+                return ''
+        else:
+            if raise_exceptions:
+                raise TypeError('Color sequence format must be (int, int, int)!')
+            return ''
+
+    # Looks for the name of the input RGB color.
+    try:
+        closest_name = _webcolors.rgb_to_name(tuple(color))
+    except ValueError:
+        closest_name = closest_color(color)
+    if closest_name in Colors.change_map:
+        closest_name = Colors.change_map[closest_name]
+    return closest_name
+
+
+def get_color(color: _Union[str, _Sequence], raise_exceptions: bool = False) -> str:
+    """Gets a color name and returns it in ansi format
+
+    >>>
+    >>> get_color('LightRed')
+    '\x1b[91m'
+    >>>
+    >>> import log21
+    >>> log21.get_logger().info(log21.get_color('Blue') + 'Hello World!')
+    [21:21:21] [INFO] Hello World!
+    >>> # Note that you must run it yourself to see the colorful result ;D
+    >>>
+
+    :param color: color name(Example: Blue)
+    :param raise_exceptions: bool = False:
+        False: It will return '' instead of raising exceptions when an error occurs.
+        True: It may raise TypeError or KeyError
+    :raises TypeError: `color` must be str
+    :raises KeyError: `color` not found!
+    :return: str: an ansi color
+    """
+    if not isinstance(color, (str, _Sequence)):
+        if raise_exceptions:
+            raise TypeError('`color` must be str or Sequence!')
+        return ''
+    if isinstance(color, _Sequence) and not isinstance(color, str):
+        color = get_color_name(color)
+        return get_color(color)
+
+    color = color.lower()
+    color = color.replace(' ', '').replace('_', '').replace('-', '')
+    color = color.replace('foreground', '').replace('fore', '').replace('ground', '')
+    if (color.startswith('#') and len(color) == 7) or (color.isdigit()
+                                                       and len(color) == 9):
+        color = get_color_name(color)
+        return get_color(color)
+    if color in Colors.color_map_:
+        return Colors.color_map_[color]
+    if ansi_escape.match(color):
+        return ansi_escape.match(color).group()
+    if color in Colors.change_map:
+        return get_color(Colors.change_map[color])
+    if raise_exceptions:
+        raise KeyError(f'`{color}` not found!')
+    return ''
+
+
+def get_colors(*colors: str, raise_exceptions: bool = False) -> str:
+    """Gets a list of colors and combines them into one.
+
+    >>>
+    >>> get_colors('LightCyan')
+    '\x1b[96m'
+    >>>
+    >>> import log21
+    >>> log21.get_logger().info(log21.get_colors('Green', 'Background White') +
+    ... 'Hello World!')
+    [21:21:21] [INFO] Hello World!
+    >>> # Note that you must run it yourself to see the colorful result ;D
+    >>>
+
+    :param colors: Input colors
+    :param raise_exceptions: bool = False:
+        False: It will return '' instead of raising exceptions when an error occurs.
+        True: It may raise TypeError or KeyError
+    :raises TypeError: `color` must be str
+    :raises KeyError: `color` not found!
+    :return: str: a combined color
+    """
+    output = ''
+    for color in colors:
+        output += get_color(str(color), raise_exceptions=raise_exceptions)
+    parts = ansi_escape.split(output)
+    output = '\033['
+    for part in parts:
+        if part:
+            output += part + ';'
+    if output.endswith(';'):
+        output = output[:-1] + 'm'
+        return output
+    return ''
```

### Comparing `log21-2.8.1b0/src/log21/CrashReporter/Formatters.py` & `log21-2.9.0/src/log21/CrashReporter/Formatters.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,121 +1,121 @@
-# log21.CrashReporter.Formatters.py
-# CodeWriter21
-
-import traceback
-from typing import (Any as _Any, Union as _Union, Mapping as _Mapping,
-                    Callable as _Callable, Optional as _Optional)
-from datetime import datetime as _datetime
-
-__all__ = [
-    'Formatter', 'CONSOLE_REPORTER_FORMAT', 'FILE_REPORTER_FORMAT',
-    'EMAIL_REPORTER_FORMAT'
-]
-
-RESERVED_KEYS = (
-    '__name__', 'type', 'message', 'traceback', 'name', 'file', 'lineno', 'function',
-    'asctime'
-)
-
-
-class Formatter:
-    """The base class for all CrashReporter formatters."""
-
-    def __init__(
-        self,
-        format_: str,
-        style: str = '%',
-        datefmt: str = '%Y-%m-%d %H:%M:%S',
-        extra_values: _Optional[_Mapping[str, _Union[str, _Callable, _Any]]] = None
-    ):
-        """Initialize the formatter.
-
-        :param format_: The format string.
-        :param style: The style of the format string. Valid styles: %, {
-        :param datefmt: The date format string.
-        :param extra_values: A mapping of extra values to be added to the log record.
-        """
-        self._format = format_
-
-        if style in ['%', '{']:
-            self.__style = style
-        else:
-            raise ValueError('Invalid style: "' + str(style) + '" Valid styles: %, {')
-
-        self.datefmt = datefmt
-        self.extra_values = {}
-        if extra_values:
-            for key in extra_values:
-                if key in RESERVED_KEYS:
-                    raise ValueError(
-                        f'`{key}` is a reserved-key and cannot be used in '
-                        '`extra_values`.'
-                    )
-                self.extra_values[key] = extra_values[key]
-
-    def format(self, exception: BaseException) -> str:
-        """Format the exception.
-
-        :param exception: The exception to format.
-        :raises ValueError: If the style is not either '%' or '{'.
-        :return: The formatted exception.
-        """
-        exception_dict = {
-            '__name__': __name__,
-            'type': type(exception),
-            'message': exception.args[0],
-            'traceback': traceback.format_tb(exception.__traceback__.tb_next),
-            'name': exception.__class__.__name__,
-            'file': exception.__traceback__.tb_next.tb_frame.f_code.co_filename,
-            'lineno': exception.__traceback__.tb_next.tb_lineno,
-            'function': exception.__traceback__.tb_next.tb_frame.f_code.co_name,
-            'asctime': _datetime.now().strftime(self.datefmt),
-        }
-        for key, value in self.extra_values.items():
-            if callable(value):
-                exception_dict[key] = value()
-            else:
-                exception_dict[key] = value
-
-        if self.__style == '%':
-            return self._format % exception_dict
-        if self.__style == '{':
-            return self._format.format(**exception_dict)
-        raise ValueError(
-            'Invalid style: "' + str(self.__style) + '" Valid styles: %, {'
-        )
-
-
-CONSOLE_REPORTER_FORMAT = {
-    'format_':
-    '\033[91m%(name)s: %(message)s\033[0m\n'  # Name and message of the exception.
-    '\tFile\033[91m:\033[0m "%(file)s"\n'  # The file that exception was raised in.
-    '\tLine\033[91m:\033[0m %(lineno)d',  # The line that exception was raised on.
-    'style':
-    '%'
-}
-
-FILE_REPORTER_FORMAT = {
-    'format_':
-    '[%(asctime)s] %(name)s: %(message)s'  # Name and message of the exception.
-    '; File: "%(file)s"'  # The file that exception was raised in.
-    '; Line: %(lineno)d\n',  # The line that exception was raised on.
-    'style':
-    '%'
-}
-
-EMAIL_REPORTER_FORMAT = {
-    'format_': """
-    <html>
-        <body>
-            <h1>Crash Report: %(__name__)s</h1>
-            <h2>%(name)s: %(message)s</h2>
-            <p>
-                <span style="bold">File:</span> "%(file)s"<br>
-                <span style="bold">Line:</span> %(lineno)d<br>
-                <span style="center">%(asctime)s</span><br>
-            </p>
-        <body>
-    </html>
-    """,
-    'style': '%'
-}
+# log21.CrashReporter.Formatters.py
+# CodeWriter21
+
+import traceback
+from typing import (Any as _Any, Union as _Union, Mapping as _Mapping,
+                    Callable as _Callable, Optional as _Optional)
+from datetime import datetime as _datetime
+
+__all__ = [
+    'Formatter', 'CONSOLE_REPORTER_FORMAT', 'FILE_REPORTER_FORMAT',
+    'EMAIL_REPORTER_FORMAT'
+]
+
+RESERVED_KEYS = (
+    '__name__', 'type', 'message', 'traceback', 'name', 'file', 'lineno', 'function',
+    'asctime'
+)
+
+
+class Formatter:
+    """The base class for all CrashReporter formatters."""
+
+    def __init__(
+        self,
+        format_: str,
+        style: str = '%',
+        datefmt: str = '%Y-%m-%d %H:%M:%S',
+        extra_values: _Optional[_Mapping[str, _Union[str, _Callable, _Any]]] = None
+    ):
+        """Initialize the formatter.
+
+        :param format_: The format string.
+        :param style: The style of the format string. Valid styles: %, {
+        :param datefmt: The date format string.
+        :param extra_values: A mapping of extra values to be added to the log record.
+        """
+        self._format = format_
+
+        if style in ['%', '{']:
+            self.__style = style
+        else:
+            raise ValueError('Invalid style: "' + str(style) + '" Valid styles: %, {')
+
+        self.datefmt = datefmt
+        self.extra_values = {}
+        if extra_values:
+            for key in extra_values:
+                if key in RESERVED_KEYS:
+                    raise ValueError(
+                        f'`{key}` is a reserved-key and cannot be used in '
+                        '`extra_values`.'
+                    )
+                self.extra_values[key] = extra_values[key]
+
+    def format(self, exception: BaseException) -> str:
+        """Format the exception.
+
+        :param exception: The exception to format.
+        :raises ValueError: If the style is not either '%' or '{'.
+        :return: The formatted exception.
+        """
+        exception_dict = {
+            '__name__': __name__,
+            'type': type(exception),
+            'message': exception.args[0],
+            'traceback': traceback.format_tb(exception.__traceback__.tb_next),
+            'name': exception.__class__.__name__,
+            'file': exception.__traceback__.tb_next.tb_frame.f_code.co_filename,
+            'lineno': exception.__traceback__.tb_next.tb_lineno,
+            'function': exception.__traceback__.tb_next.tb_frame.f_code.co_name,
+            'asctime': _datetime.now().strftime(self.datefmt),
+        }
+        for key, value in self.extra_values.items():
+            if callable(value):
+                exception_dict[key] = value()
+            else:
+                exception_dict[key] = value
+
+        if self.__style == '%':
+            return self._format % exception_dict
+        if self.__style == '{':
+            return self._format.format(**exception_dict)
+        raise ValueError(
+            'Invalid style: "' + str(self.__style) + '" Valid styles: %, {'
+        )
+
+
+CONSOLE_REPORTER_FORMAT = {
+    'format_':
+    '\033[91m%(name)s: %(message)s\033[0m\n'  # Name and message of the exception.
+    '\tFile\033[91m:\033[0m "%(file)s"\n'  # The file that exception was raised in.
+    '\tLine\033[91m:\033[0m %(lineno)d',  # The line that exception was raised on.
+    'style':
+    '%'
+}
+
+FILE_REPORTER_FORMAT = {
+    'format_':
+    '[%(asctime)s] %(name)s: %(message)s'  # Name and message of the exception.
+    '; File: "%(file)s"'  # The file that exception was raised in.
+    '; Line: %(lineno)d\n',  # The line that exception was raised on.
+    'style':
+    '%'
+}
+
+EMAIL_REPORTER_FORMAT = {
+    'format_': """
+    <html>
+        <body>
+            <h1>Crash Report: %(__name__)s</h1>
+            <h2>%(name)s: %(message)s</h2>
+            <p>
+                <span style="bold">File:</span> "%(file)s"<br>
+                <span style="bold">Line:</span> %(lineno)d<br>
+                <span style="center">%(asctime)s</span><br>
+            </p>
+        <body>
+    </html>
+    """,
+    'style': '%'
+}
```

### Comparing `log21-2.8.1b0/src/log21/FileHandler.py` & `log21-2.9.0/src/log21/FileHandler.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-# log21.FileHandler.py
-# CodeWriter21
-
-from logging import FileHandler as _FileHandler
-
-from log21.Formatters import DecolorizingFormatter as _DecolorizingFormatter
-
-
-class FileHandler(_FileHandler):
-    """A subclass of logging.FileHandler that allows you to specify a
-    formatter and a level when you initialize it."""
-
-    def __init__(
-        self,
-        filename,
-        mode='a',
-        encoding=None,
-        delay=False,
-        errors=None,
-        formatter=None,
-        level=None
-    ):
-        """Initialize the handler.
-
-        :param filename: The filename of the log file.
-        :param mode: The mode to open the file in.
-        :param encoding: The encoding to use when opening the file.
-        :param delay: Whether to delay opening the file.
-        :param errors: The error handling scheme to use.
-        :param formatter: The formatter to use.
-        :param level: The level to use.
-        """
-        super().__init__(filename, mode, encoding, delay, errors)
-        if formatter is not None:
-            self.setFormatter(formatter)
-        if level is not None:
-            self.setLevel(level)
-
-
-class DecolorizingFileHandler(FileHandler):
-    """A subclass of FileHandler that removes ANSI colors from the log messages before
-    writing them to the file."""
-    terminator = ''
-
-    def emit(self, record):
-        """Emit a record."""
-        if self.stream is None:
-            self.stream = self._open()
-        try:
-            msg = self.format(record)
-            msg = _DecolorizingFormatter.decolorize(msg)
-            stream = self.stream
-            stream.write(msg + self.terminator)
-            self.flush()
-        except Exception:  # pylint: disable=broad-except
-            self.handleError(record)
+# log21.FileHandler.py
+# CodeWriter21
+
+from logging import FileHandler as _FileHandler
+
+from log21.Formatters import DecolorizingFormatter as _DecolorizingFormatter
+
+
+class FileHandler(_FileHandler):
+    """A subclass of logging.FileHandler that allows you to specify a
+    formatter and a level when you initialize it."""
+
+    def __init__(
+        self,
+        filename,
+        mode='a',
+        encoding=None,
+        delay=False,
+        errors=None,
+        formatter=None,
+        level=None
+    ):
+        """Initialize the handler.
+
+        :param filename: The filename of the log file.
+        :param mode: The mode to open the file in.
+        :param encoding: The encoding to use when opening the file.
+        :param delay: Whether to delay opening the file.
+        :param errors: The error handling scheme to use.
+        :param formatter: The formatter to use.
+        :param level: The level to use.
+        """
+        super().__init__(filename, mode, encoding, delay, errors)
+        if formatter is not None:
+            self.setFormatter(formatter)
+        if level is not None:
+            self.setLevel(level)
+
+
+class DecolorizingFileHandler(FileHandler):
+    """A subclass of FileHandler that removes ANSI colors from the log messages before
+    writing them to the file."""
+    terminator = ''
+
+    def emit(self, record):
+        """Emit a record."""
+        if self.stream is None:
+            self.stream = self._open()
+        try:
+            msg = self.format(record)
+            msg = _DecolorizingFormatter.decolorize(msg)
+            stream = self.stream
+            stream.write(msg + self.terminator)
+            self.flush()
+        except Exception:  # pylint: disable=broad-except
+            self.handleError(record)
```

### Comparing `log21-2.8.1b0/src/log21/Formatters.py` & `log21-2.9.0/src/log21/Formatters.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,293 +1,293 @@
-# log21.Formatters.py
-# CodeWriter21
-
-import time as _time
-from typing import (Dict as _Dict, Tuple as _Tuple, Mapping as _Mapping,
-                    Optional as _Optional)
-from logging import Formatter as __Formatter
-
-from log21.Colors import get_colors as _gc, ansi_escape
-from log21.Levels import INFO, DEBUG, ERROR, INPUT, PRINT, WARNING, CRITICAL
-
-__all__ = ['ColorizingFormatter', 'DecolorizingFormatter']
-
-
-class _Formatter(__Formatter):
-
-    def __init__(
-        self,
-        fmt: _Optional[str] = None,
-        datefmt: _Optional[str] = None,
-        style: str = '%',
-        level_names: _Optional[_Mapping[int, str]] = None
-    ):
-        """
-        `level_names` usage:
-        >>> import log21
-        >>> logger = log21.Logger('MyLogger', log21.DEBUG)
-        >>> stream_handler = log21.ColorizingStreamHandler()
-        >>> formatter = log21.ColorizingFormatter(fmt='[%(levelname)s] %(message)s',
-        ...             level_names={log21.DEBUG: ' ', log21.INFO: '+',
-        ...                          log21.WARNING: '-', log21.ERROR: '!',
-        ...                          log21.CRITICAL: 'X'})
-        >>> stream_handler.setFormatter(formatter)
-        >>> logger.addHandler(stream_handler)
-        >>>
-        >>> logger.debug('Just wanna see if this works...')
-        [ ] Just wanna see if this works...
-        >>> logger.info("FYI: I'm glad somebody read this 8)")
-        [+] FYI: I'm glad somebody read this 8)
-        >>> logger.warning("Oh no! Something's gonna happen!")
-        [-] Oh no! something's gonna happen!
-        >>> logger.error('AN ERROR OCCURRED! (told ya ;))')
-        [!] AN ERROR OCCURRED! (told ya ;))
-        >>> logger.critical('Crashed....')
-        [X] Crashed....
-        >>>
-        >>> # Hope you've enjoyed
-        >>>
-
-        :param fmt: The format string to use.
-        :param datefmt: The date format string to use.
-        :param style: The style to use.
-        :param level_names: A dictionary mapping logging levels to their names.
-        """
-        super().__init__(fmt=fmt, datefmt=datefmt, style=style)
-
-        self._level_names: _Dict[int, str] = {
-            DEBUG: 'DEBUG',
-            INFO: 'INFO',
-            WARNING: 'WARNING',
-            ERROR: 'ERROR',
-            CRITICAL: 'CRITICAL',
-            PRINT: 'PRINT',
-            INPUT: 'INPUT'
-        }
-
-        if level_names:
-            for level, name in level_names.items():
-                self.level_names[level] = name
-
-    @property
-    def level_names(self):
-        """Get the level names mapping."""
-        return self._level_names
-
-    @level_names.setter
-    def level_names(self, level_names: _Mapping[int, str]):
-        if level_names:
-            if not isinstance(level_names, _Mapping):
-                raise TypeError(
-                    '`level_names` must be a Mapping, a dictionary like object!'
-                )
-            self._level_names = level_names
-        else:
-            self._level_names = {}
-
-    def format(self, record) -> str:
-        record.message = record.getMessage()
-        if self.usesTime():
-            record.asctime = self.formatTime(record, self.datefmt)
-
-        record.levelname = self.level_names.get(record.levelno, 'NOTSET')
-
-        s = self.formatMessage(record)  # pylint: disable=invalid-name
-        if record.exc_info:
-            if not record.exc_text:
-                record.exc_text = self.formatException(record.exc_info)
-        if record.exc_text:
-            if s[-1:] != "\n":
-                s = s + "\n"
-            s = s + record.exc_text
-        if record.stack_info:
-            if s[-1:] != "\n":
-                s = s + "\n"
-            s = s + self.formatStack(record.stack_info)
-        return s
-
-
-class ColorizingFormatter(_Formatter):  # pylint: disable=too-many-instance-attributes
-    """A formatter that helps adding colors to the log records."""
-    time_color: _Tuple[str, ...] = ('lightblue', )
-    name_color = pathname_color = filename_color = module_color = func_name_color = \
-        thread_name_color = message_color = tuple()
-
-    def __init__(
-        self,
-        fmt: _Optional[str] = None,
-        datefmt: _Optional[str] = None,
-        style: str = '%',
-        level_names: _Optional[_Mapping[int, str]] = None,
-        level_colors: _Optional[_Mapping[int, _Tuple[str]]] = None,
-        time_color: _Optional[_Tuple[str, ...]] = None,
-        name_color: _Optional[_Tuple[str, ...]] = None,
-        pathname_color: _Optional[_Tuple[str, ...]] = None,
-        filename_color: _Optional[_Tuple[str, ...]] = None,
-        module_color: _Optional[_Tuple[str, ...]] = None,
-        func_name_color: _Optional[_Tuple[str, ...]] = None,
-        thread_name_color: _Optional[_Tuple[str, ...]] = None,
-        message_color: _Optional[_Tuple[str, ...]] = None
-    ):  # pylint: disable=too-many-branches
-        """Initialize the formatter.
-
-        :param fmt: The format string to use for the message.
-        :param datefmt: The format string to use for the date/time
-            portion of the message.
-        :param style: The format style to use.
-        :param level_names: A mapping of level numbers to level names.
-        :param level_colors: A mapping of level numbers to level colors.
-        :param time_color: The color to use for the time portion of the
-            message.
-        :param name_color: The color to use for the logger name portion
-            of the message.
-        :param pathname_color: The color to use for the pathname portion
-            of the message.
-        :param filename_color: The color to use for the filename portion
-            of the message.
-        :param module_color: The color to use for the module portion of
-            the message.
-        :param func_name_color: The color to use for the function name
-            portion of the message.
-        :param thread_name_color: The color to use for the thread name
-            portion of the message.
-        :param message_color: The color to use for the message portion
-            of the message.
-        """
-        super().__init__(fmt=fmt, datefmt=datefmt, style=style, level_names=level_names)
-        self.level_colors: _Dict[int, _Tuple[str, ...]] = {
-            DEBUG: ('lightblue', ),
-            INFO: ('green', ),
-            WARNING: ('lightyellow', ),
-            ERROR: ('light red', ),
-            CRITICAL: ('background red', 'white'),
-            PRINT: ('Cyan', ),
-            INPUT: ('Magenta', )
-        }
-        # Checks and sets colors
-        if level_colors:
-            if not isinstance(level_colors, _Mapping):
-                raise TypeError('`level_colors` must be a dictionary like object!')
-            for level, color in level_colors.items():
-                self.level_colors[level] = (_gc(*color), )
-        if time_color:
-            if not isinstance(time_color, tuple):
-                raise TypeError('`time_color` must be a tuple!')
-            self.time_color = time_color
-        if name_color:
-            if not isinstance(name_color, tuple):
-                raise TypeError('`name_color` must be a tuple!')
-            self.name_color = name_color
-        if pathname_color:
-            if not isinstance(pathname_color, tuple):
-                raise TypeError('`pathname_color` must be a tuple!')
-            self.pathname_color = pathname_color
-        if filename_color:
-            if not isinstance(filename_color, tuple):
-                raise TypeError('`filename_color` must be a tuple!')
-            self.filename_color = filename_color
-        if module_color:
-            if not isinstance(module_color, tuple):
-                raise TypeError('`module_color` must be a tuple!')
-            self.module_color = module_color
-        if func_name_color:
-            if not isinstance(func_name_color, tuple):
-                raise TypeError('`func_name_color` must be a tuple!')
-            self.func_name_color = func_name_color
-        if thread_name_color:
-            if not isinstance(thread_name_color, tuple):
-                raise TypeError('`thread_name_color` must be a tuple!')
-            self.thread_name_color = thread_name_color
-        if message_color:
-            if not isinstance(message_color, tuple):
-                raise TypeError('`message_color` must be a tuple!')
-            self.message_color = message_color
-
-    def format(self, record) -> str:
-        """Colorizes the record and returns the formatted message."""
-        record.message = record.getMessage()
-        if self.usesTime():
-            record.asctime = self.formatTime(record, self.datefmt)
-
-        record.levelname = self.level_names.get(record.levelno, 'NOTSET')
-
-        record = self.colorize(record)
-
-        s = self.formatMessage(record)  # pylint: disable=invalid-name
-        if record.exc_info:
-            # Cache the traceback text to avoid converting it multiple times
-            # (it's constant anyway)
-            if not record.exc_text:
-                record.exc_text = self.formatException(record.exc_info)
-        if record.exc_text:
-            if s[-1:] != "\n":
-                s = s + "\n"
-            s = s + record.exc_text
-        if record.stack_info:
-            if s[-1:] != "\n":
-                s = s + "\n"
-            s = s + self.formatStack(record.stack_info)
-        return s
-
-    def colorize(self, record):
-        """Colorizes the record attributes.
-
-        :param record:
-        :return: colorized record
-        """
-        reset = '\033[0m'
-
-        if hasattr(record, 'asctime'):
-            record.asctime = _gc(*self.time_color) + record.asctime + reset
-        if hasattr(record, 'levelno'):
-            record.levelname = _gc(
-                *self.level_colors.get(int(record.levelno), ('lw', ))
-            ) + getattr(record, 'levelname', 'NOTSET') + reset
-        if hasattr(record, 'name'):
-            record.name = _gc(*self.name_color) + str(record.name) + reset
-        if hasattr(record, 'pathname'):
-            record.pathname = _gc(*self.pathname_color) + record.pathname + reset
-        if hasattr(record, 'filename'):
-            record.filename = _gc(*self.filename_color) + record.filename + reset
-        if hasattr(record, 'module'):
-            record.module = _gc(*self.module_color) + record.module + reset
-        if hasattr(record, 'funcName'):
-            record.funcName = _gc(*self.func_name_color) + record.funcName + reset
-        if hasattr(record, 'threadName'):
-            record.threadName = _gc(*self.thread_name_color) + record.threadName + reset
-        if hasattr(record, 'message'):
-            record.message = _gc(*self.message_color) + record.message
-
-        return record
-
-
-class DecolorizingFormatter(_Formatter):
-    """Formatter that removes color codes from the log records."""
-
-    def formatTime(self, record, datefmt=None):
-        """Returns the creation time of the specified LogRecord as formatted
-        text."""
-        ct = self.converter(int(record.created))
-        if datefmt:
-            s = _time.strftime(datefmt, ct)
-        else:
-            t = _time.strftime(self.default_time_format, ct)
-            s = self.default_msec_format % (t, record.msecs)
-        return s
-
-    def format(self, record) -> str:
-        """Decolorizes the record and returns the formatted message.
-
-        :param record:
-        :return: str
-        """
-        return self.decolorize(super().format(record))
-
-    @staticmethod
-    def decolorize(text: str):
-        """Removes all ansi colors in the text.
-
-        :param text: str: Input text
-        :return: str: decolorized text
-        """
-
-        return ansi_escape.sub('', text)
+# log21.Formatters.py
+# CodeWriter21
+
+import time as _time
+from typing import (Dict as _Dict, Tuple as _Tuple, Mapping as _Mapping,
+                    Optional as _Optional)
+from logging import Formatter as __Formatter
+
+from log21.Colors import get_colors as _gc, ansi_escape
+from log21.Levels import INFO, DEBUG, ERROR, INPUT, PRINT, WARNING, CRITICAL
+
+__all__ = ['ColorizingFormatter', 'DecolorizingFormatter']
+
+
+class _Formatter(__Formatter):
+
+    def __init__(
+        self,
+        fmt: _Optional[str] = None,
+        datefmt: _Optional[str] = None,
+        style: str = '%',
+        level_names: _Optional[_Mapping[int, str]] = None
+    ):
+        """
+        `level_names` usage:
+        >>> import log21
+        >>> logger = log21.Logger('MyLogger', log21.DEBUG)
+        >>> stream_handler = log21.ColorizingStreamHandler()
+        >>> formatter = log21.ColorizingFormatter(fmt='[%(levelname)s] %(message)s',
+        ...             level_names={log21.DEBUG: ' ', log21.INFO: '+',
+        ...                          log21.WARNING: '-', log21.ERROR: '!',
+        ...                          log21.CRITICAL: 'X'})
+        >>> stream_handler.setFormatter(formatter)
+        >>> logger.addHandler(stream_handler)
+        >>>
+        >>> logger.debug('Just wanna see if this works...')
+        [ ] Just wanna see if this works...
+        >>> logger.info("FYI: I'm glad somebody read this 8)")
+        [+] FYI: I'm glad somebody read this 8)
+        >>> logger.warning("Oh no! Something's gonna happen!")
+        [-] Oh no! something's gonna happen!
+        >>> logger.error('AN ERROR OCCURRED! (told ya ;))')
+        [!] AN ERROR OCCURRED! (told ya ;))
+        >>> logger.critical('Crashed....')
+        [X] Crashed....
+        >>>
+        >>> # Hope you've enjoyed
+        >>>
+
+        :param fmt: The format string to use.
+        :param datefmt: The date format string to use.
+        :param style: The style to use.
+        :param level_names: A dictionary mapping logging levels to their names.
+        """
+        super().__init__(fmt=fmt, datefmt=datefmt, style=style)
+
+        self._level_names: _Dict[int, str] = {
+            DEBUG: 'DEBUG',
+            INFO: 'INFO',
+            WARNING: 'WARNING',
+            ERROR: 'ERROR',
+            CRITICAL: 'CRITICAL',
+            PRINT: 'PRINT',
+            INPUT: 'INPUT'
+        }
+
+        if level_names:
+            for level, name in level_names.items():
+                self.level_names[level] = name
+
+    @property
+    def level_names(self):
+        """Get the level names mapping."""
+        return self._level_names
+
+    @level_names.setter
+    def level_names(self, level_names: _Mapping[int, str]):
+        if level_names:
+            if not isinstance(level_names, _Mapping):
+                raise TypeError(
+                    '`level_names` must be a Mapping, a dictionary like object!'
+                )
+            self._level_names = level_names
+        else:
+            self._level_names = {}
+
+    def format(self, record) -> str:
+        record.message = record.getMessage()
+        if self.usesTime():
+            record.asctime = self.formatTime(record, self.datefmt)
+
+        record.levelname = self.level_names.get(record.levelno, 'NOTSET')
+
+        s = self.formatMessage(record)  # pylint: disable=invalid-name
+        if record.exc_info:
+            if not record.exc_text:
+                record.exc_text = self.formatException(record.exc_info)
+        if record.exc_text:
+            if s[-1:] != "\n":
+                s = s + "\n"
+            s = s + record.exc_text
+        if record.stack_info:
+            if s[-1:] != "\n":
+                s = s + "\n"
+            s = s + self.formatStack(record.stack_info)
+        return s
+
+
+class ColorizingFormatter(_Formatter):  # pylint: disable=too-many-instance-attributes
+    """A formatter that helps adding colors to the log records."""
+    time_color: _Tuple[str, ...] = ('lightblue', )
+    name_color = pathname_color = filename_color = module_color = func_name_color = \
+        thread_name_color = message_color = tuple()
+
+    def __init__(
+        self,
+        fmt: _Optional[str] = None,
+        datefmt: _Optional[str] = None,
+        style: str = '%',
+        level_names: _Optional[_Mapping[int, str]] = None,
+        level_colors: _Optional[_Mapping[int, _Tuple[str]]] = None,
+        time_color: _Optional[_Tuple[str, ...]] = None,
+        name_color: _Optional[_Tuple[str, ...]] = None,
+        pathname_color: _Optional[_Tuple[str, ...]] = None,
+        filename_color: _Optional[_Tuple[str, ...]] = None,
+        module_color: _Optional[_Tuple[str, ...]] = None,
+        func_name_color: _Optional[_Tuple[str, ...]] = None,
+        thread_name_color: _Optional[_Tuple[str, ...]] = None,
+        message_color: _Optional[_Tuple[str, ...]] = None
+    ):  # pylint: disable=too-many-branches
+        """Initialize the formatter.
+
+        :param fmt: The format string to use for the message.
+        :param datefmt: The format string to use for the date/time
+            portion of the message.
+        :param style: The format style to use.
+        :param level_names: A mapping of level numbers to level names.
+        :param level_colors: A mapping of level numbers to level colors.
+        :param time_color: The color to use for the time portion of the
+            message.
+        :param name_color: The color to use for the logger name portion
+            of the message.
+        :param pathname_color: The color to use for the pathname portion
+            of the message.
+        :param filename_color: The color to use for the filename portion
+            of the message.
+        :param module_color: The color to use for the module portion of
+            the message.
+        :param func_name_color: The color to use for the function name
+            portion of the message.
+        :param thread_name_color: The color to use for the thread name
+            portion of the message.
+        :param message_color: The color to use for the message portion
+            of the message.
+        """
+        super().__init__(fmt=fmt, datefmt=datefmt, style=style, level_names=level_names)
+        self.level_colors: _Dict[int, _Tuple[str, ...]] = {
+            DEBUG: ('lightblue', ),
+            INFO: ('green', ),
+            WARNING: ('lightyellow', ),
+            ERROR: ('light red', ),
+            CRITICAL: ('background red', 'white'),
+            PRINT: ('Cyan', ),
+            INPUT: ('Magenta', )
+        }
+        # Checks and sets colors
+        if level_colors:
+            if not isinstance(level_colors, _Mapping):
+                raise TypeError('`level_colors` must be a dictionary like object!')
+            for level, color in level_colors.items():
+                self.level_colors[level] = (_gc(*color), )
+        if time_color:
+            if not isinstance(time_color, tuple):
+                raise TypeError('`time_color` must be a tuple!')
+            self.time_color = time_color
+        if name_color:
+            if not isinstance(name_color, tuple):
+                raise TypeError('`name_color` must be a tuple!')
+            self.name_color = name_color
+        if pathname_color:
+            if not isinstance(pathname_color, tuple):
+                raise TypeError('`pathname_color` must be a tuple!')
+            self.pathname_color = pathname_color
+        if filename_color:
+            if not isinstance(filename_color, tuple):
+                raise TypeError('`filename_color` must be a tuple!')
+            self.filename_color = filename_color
+        if module_color:
+            if not isinstance(module_color, tuple):
+                raise TypeError('`module_color` must be a tuple!')
+            self.module_color = module_color
+        if func_name_color:
+            if not isinstance(func_name_color, tuple):
+                raise TypeError('`func_name_color` must be a tuple!')
+            self.func_name_color = func_name_color
+        if thread_name_color:
+            if not isinstance(thread_name_color, tuple):
+                raise TypeError('`thread_name_color` must be a tuple!')
+            self.thread_name_color = thread_name_color
+        if message_color:
+            if not isinstance(message_color, tuple):
+                raise TypeError('`message_color` must be a tuple!')
+            self.message_color = message_color
+
+    def format(self, record) -> str:
+        """Colorizes the record and returns the formatted message."""
+        record.message = record.getMessage()
+        if self.usesTime():
+            record.asctime = self.formatTime(record, self.datefmt)
+
+        record.levelname = self.level_names.get(record.levelno, 'NOTSET')
+
+        record = self.colorize(record)
+
+        s = self.formatMessage(record)  # pylint: disable=invalid-name
+        if record.exc_info:
+            # Cache the traceback text to avoid converting it multiple times
+            # (it's constant anyway)
+            if not record.exc_text:
+                record.exc_text = self.formatException(record.exc_info)
+        if record.exc_text:
+            if s[-1:] != "\n":
+                s = s + "\n"
+            s = s + record.exc_text
+        if record.stack_info:
+            if s[-1:] != "\n":
+                s = s + "\n"
+            s = s + self.formatStack(record.stack_info)
+        return s
+
+    def colorize(self, record):
+        """Colorizes the record attributes.
+
+        :param record:
+        :return: colorized record
+        """
+        reset = '\033[0m'
+
+        if hasattr(record, 'asctime'):
+            record.asctime = _gc(*self.time_color) + record.asctime + reset
+        if hasattr(record, 'levelno'):
+            record.levelname = _gc(
+                *self.level_colors.get(int(record.levelno), ('lw', ))
+            ) + getattr(record, 'levelname', 'NOTSET') + reset
+        if hasattr(record, 'name'):
+            record.name = _gc(*self.name_color) + str(record.name) + reset
+        if hasattr(record, 'pathname'):
+            record.pathname = _gc(*self.pathname_color) + record.pathname + reset
+        if hasattr(record, 'filename'):
+            record.filename = _gc(*self.filename_color) + record.filename + reset
+        if hasattr(record, 'module'):
+            record.module = _gc(*self.module_color) + record.module + reset
+        if hasattr(record, 'funcName'):
+            record.funcName = _gc(*self.func_name_color) + record.funcName + reset
+        if hasattr(record, 'threadName'):
+            record.threadName = _gc(*self.thread_name_color) + record.threadName + reset
+        if hasattr(record, 'message'):
+            record.message = _gc(*self.message_color) + record.message
+
+        return record
+
+
+class DecolorizingFormatter(_Formatter):
+    """Formatter that removes color codes from the log records."""
+
+    def formatTime(self, record, datefmt=None):
+        """Returns the creation time of the specified LogRecord as formatted
+        text."""
+        ct = self.converter(int(record.created))
+        if datefmt:
+            s = _time.strftime(datefmt, ct)
+        else:
+            t = _time.strftime(self.default_time_format, ct)
+            s = self.default_msec_format % (t, record.msecs)
+        return s
+
+    def format(self, record) -> str:
+        """Decolorizes the record and returns the formatted message.
+
+        :param record:
+        :return: str
+        """
+        return self.decolorize(super().format(record))
+
+    @staticmethod
+    def decolorize(text: str):
+        """Removes all ansi colors in the text.
+
+        :param text: str: Input text
+        :return: str: decolorized text
+        """
+
+        return ansi_escape.sub('', text)
```

### Comparing `log21-2.8.1b0/src/log21/LoggingWindow.py` & `log21-2.9.0/src/log21/LoggingWindow.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,875 +1,875 @@
-# log21.LoggingWindow.py
-# CodeWriter2
-
-from __future__ import annotations
-
-import re as _re
-import threading as _threading
-import subprocess as _subprocess
-from enum import Enum as _Enum
-from time import sleep as _sleep
-from uuid import uuid4 as _uuid4
-from string import printable as _printable
-from typing import Union as _Union
-from logging import FileHandler as _FileHandler
-from argparse import Namespace as _Namespace
-
-from log21.Colors import hex_escape as _hex_escape, ansi_escape as _ansi_escape
-from log21.Levels import NOTSET as _NOTSET
-from log21.Logger import Logger as _Logger
-from log21.StreamHandler import StreamHandler as _StreamHandler
-
-__all__ = ['LoggingWindow', 'LoggingWindowHandler']
-
-try:
-    import tkinter as _tkinter
-except ImportError:
-    _tkinter = None
-
-ansi_to_hex_color_map = {
-    # https://chrisyeh96.github.io/2020/03/28/terminal-colors.html
-    '30': ('#000000', 'foreground'),  # Black foreground
-    '31': ('#cc0000', 'foreground'),  # Red foreground
-    '32': ('#4e9a06', 'foreground'),  # Green foreground
-    '33': ('#c4a000', 'foreground'),  # Yellow foreground
-    '34': ('#729fcf', 'foreground'),  # Blue foreground
-    '35': ('#75507b', 'foreground'),  # Magenta foreground
-    '36': ('#06989a', 'foreground'),  # Cyan foreground
-    '37': ('#d3d7cf', 'foreground'),  # White foreground
-    '90': ('#555753', 'foreground'),  # Bright black foreground
-    '91': ('#ef2929', 'foreground'),  # Bright red foreground
-    '92': ('#8ae234', 'foreground'),  # Bright green foreground
-    '93': ('#fce94f', 'foreground'),  # Bright yellow foreground
-    '94': ('#32afff', 'foreground'),  # Bright blue foreground
-    '95': ('#ad7fa8', 'foreground'),  # Bright magenta foreground
-    '96': ('#34e2e2', 'foreground'),  # Bright cyan foreground
-    '97': ('#ffffff', 'foreground'),  # Bright white foreground
-    '40': ('#000000', 'background'),  # Black background
-    '41': ('#cc0000', 'background'),  # Red background
-    '42': ('#4e9a06', 'background'),  # Green background
-    '43': ('#c4a000', 'background'),  # Yellow background
-    '44': ('#729fcf', 'background'),  # Blue background
-    '45': ('#75507b', 'background'),  # Magenta background
-    '46': ('#06989a', 'background'),  # Cyan background
-    '47': ('#d3d7cf', 'background'),  # White background
-    '100': ('#555753', 'background'),  # Bright black background
-    '101': ('#ef2929', 'background'),  # Bright red background
-    '102': ('#8ae234', 'background'),  # Bright green background
-    '103': ('#fce94f', 'background'),  # Bright yellow background
-    '104': ('#32afff', 'background'),  # Bright blue background
-    '105': ('#ad7fa8', 'background'),  # Bright magenta background
-    '106': ('#34e2e2', 'background'),  # Bright cyan background
-    '107': ('#ffffff', 'background'),  # Bright white background
-}
-
-_lock = _threading.RLock()
-
-
-class GettingInputStatus(_Enum):
-    """An enum for the status of getting input."""
-    NOT_GETTING_INPUT = 0
-    GETTING_INPUT = 1
-    CANCELLED = 2
-
-
-class CancelledInputError(InterruptedError, Exception):
-    """An exception raised when the input is cancelled."""
-
-
-class LoggingWindowHandler(_StreamHandler):
-    """A handler for logging to a LoggingWindow."""
-
-    def __init__(
-        self,
-        logging_window: LoggingWindow,
-        handle_carriage_return: bool = True,
-        handle_new_line: bool = True
-    ):
-        """Initialize the LoggingWindowHandler.
-
-        :param logging_window: The LoggingWindow to log to.
-        :param handle_carriage_return: Whether to handle carriage
-            returns.
-        :param handle_new_line: Whether to handle new lines.
-        """
-        self.HandleCR = handle_carriage_return
-        self.HandleNL = handle_new_line
-        self.__carriage_return: bool = False
-        self.LoggingWindow = logging_window  # pylint: disable=invalid-name
-        super().__init__(stream=None)
-
-    def emit(self, record):
-        try:
-            if self.HandleCR:
-                self.check_cr(record)
-            if self.HandleNL:
-                self.check_nl(record)
-            msg = self.format(record)
-            self.write(msg)
-            self.write(self.terminator)
-        except Exception:  # pylint: disable=broad-except
-            self.handleError(record)
-
-    def write(self, message):  # pylint: disable=too-many-branches
-        """Write a message to the LoggingWindow.
-
-        :param message: The message to write.
-        """
-        if self.LoggingWindow is not None:  # pylint: disable=too-many-nested-blocks
-            # Sets the element's state to normal so that it can be modified.
-            self.LoggingWindow.logs.config(state=_tkinter.NORMAL)
-
-            # Handles carriage return
-            parts = _re.split(r'(\r)', message)
-
-            while parts:
-                part = parts.pop(0)
-
-                if self.__carriage_return:
-                    # Checks if the part is printable
-                    if any((char in _printable[:-6])
-                           for char in _hex_escape.sub('', _ansi_escape.sub('', part))):
-                        # Removes the last line
-                        self.LoggingWindow.logs.delete('end - 1 lines', _tkinter.END)
-                        if self.LoggingWindow.logs.count('0.0', 'end')[0] != 1:
-                            self.LoggingWindow.logs.insert('end', '\n')
-                        self.__carriage_return = False
-
-                tags = []
-                # Handles ANSI color codes
-                ansi_parts = _ansi_escape.split(part)
-                while ansi_parts:
-                    ansi_text = ansi_parts.pop(0)
-
-                    if ansi_text:
-                        # Handles HEX color codes
-                        hex_parts = _hex_escape.split(ansi_text)
-                        while hex_parts:
-                            hex_text = hex_parts.pop(0)
-
-                            if hex_text:
-                                self.LoggingWindow.logs.insert(_tkinter.END, hex_text)
-
-                            if hex_parts:
-                                hex_color = hex_parts.pop(0)
-
-                                tag = str(_uuid4())
-                                # Foreground color
-                                if hex_parts.pop(0) == 'f':
-                                    tags.append(
-                                        {
-                                            'name': tag,
-                                            'start':
-                                            self.LoggingWindow.logs.index('end-1c'),
-                                            'config': {
-                                                'foreground': hex_color
-                                            }
-                                        }
-                                    )
-                                # Background color
-                                else:
-                                    tags.append(
-                                        {
-                                            'name': tag,
-                                            'start':
-                                            self.LoggingWindow.logs.index('end-1c'),
-                                            'config': {
-                                                'background': hex_color
-                                            }
-                                        }
-                                    )
-
-                    if ansi_parts:
-                        ansi_params = ansi_parts.pop(0).split(';')
-                        ansi_color = {'foreground': None, 'background': None}
-
-                        for part in ansi_params:
-                            if part in ansi_to_hex_color_map:
-                                color_ = ansi_to_hex_color_map[part]
-                                ansi_color[color_[1]] = color_[0]
-                            elif part == '0':
-                                ansi_color[
-                                    'foreground'
-                                ] = self.LoggingWindow.default_foreground_color
-                                ansi_color[
-                                    'background'
-                                ] = self.LoggingWindow.default_background_color
-                            else:
-                                pass  # error condition ignored
-                        if ansi_color['foreground'] or ansi_color['background']:
-                            tags.append(
-                                {
-                                    'name': str(_uuid4()),
-                                    'start': self.LoggingWindow.logs.index('end-1c'),
-                                    'config': ansi_color
-                                }
-                            )
-
-                # Applies the color tags
-                for tag in tags:
-                    self.LoggingWindow.logs.tag_add(tag['name'], tag['start'], 'end')
-                    self.LoggingWindow.logs.tag_config(tag['name'], **tag['config'])
-
-                if parts:
-                    parts.pop(0)
-                    self.__carriage_return = True
-
-            self.LoggingWindow.logs.config(state=_tkinter.DISABLED)
-            self.LoggingWindow.logs.see(_tkinter.END)
-
-
-class LoggingWindow(_Logger):  # pylint: disable=too-many-instance-attributes
-    """
-    Usage Example:
-        >>> # Manual creation
-        >>> # Imports the LoggingWindow and LoggingWindowHandler classes
-        >>> from log21 import LoggingWindow, LoggingWindowHandler
-        >>> # Creates a new LoggingWindow object
-        >>> window = LoggingWindow('Test Window', level='DEBUG')
-        >>> # Creates a new LoggingWindowHandler object and adds it to the LoggingWindow
-        >>> # we created earlier
-        >>> window.addHandler(LoggingWindowHandler(window))
-        >>> window.debug('A debug message')
-        >>> window.info('An info message')
-        >>> # Run these lines to see the messages in the window
-        >>>
-        >>> # Automatic creation
-        >>> # Imports log21 and time modules
-        >>> import log21, time
-        >>> # Creates a new LoggingWindow object
-        >>> window = log21.get_logging_window('Test Window')
-        >>> # Use it without any additional steps to add handlers and formatters
-        >>> window.info('This works properly!')
-        >>> # ANSI colors usage:
-        >>> window.info('This is a \033[91mred\033[0m message.')
-        >>> window.info('\033[102mThis is a message with green background.')
-        >>> # HEX colors usage:
-        >>> window.info('\033#00FFFFhfThis is a message with cyan foreground.')
-        >>> window.info('\033#0000FFhbThis is a message with blue background.')
-        >>> # Progressbar usage:
-        >>> for i in range(100):
-        ...     window.print_progress(i + 1, 100)
-        ...     time.sleep(0.1)
-        ...
-        >>> # Gettig input from the user:
-        >>> name: str = window.input('Enter your name: ')
-        >>> window.print('Hello, ' + name + '!')
-        >>> # Run these lines to see the messages in the window
-        >>>
-
-    """
-
-    def __init__(
-        self,
-        name,
-        level=_NOTSET,
-        width: int = 80,
-        height: int = 20,
-        default_foreground_color='white',
-        default_background_color='black',
-        font=('Courier', 10),
-        allow_python: bool = False,
-        allow_shell: bool = False,
-        command_history_buffer_size: int = 100
-    ):  # pylint: disable=too-many-statements
-        """Creates a new LoggingWindow object.
-
-        :param name: The name of the logger.
-        :param level: The level of the logger.
-        :param width: The width of the LoggingWindow.
-        :param height: The height of the LoggingWindow.
-        :param default_foreground_color: The default foreground color of
-            the LoggingWindow.
-        :param default_background_color: The default background color of
-            the LoggingWindow.
-        :param font: The font of the LoggingWindow.
-        """
-        super().__init__(name, level)
-        self.window = _tkinter.Tk()
-        self.window.title(name)
-        # Hides window instead of closing it
-        self.window.protocol("WM_DELETE_WINDOW", self.hide)
-
-        self.window.resizable(False, False)
-
-        self.logs = _tkinter.Text(self.window)
-        self.logs.grid(row=0, column=0, sticky='nsew')
-        self.logs.config(state=_tkinter.DISABLED)
-        self.logs.config(wrap=_tkinter.NONE)
-
-        # Commands entry
-        self.command_entry = _tkinter.Entry(self.window)
-        self.command_entry.grid(row=1, column=0, sticky='nsew')
-        self.command_entry.bind('<Return>', self.execute_command)
-        self.command_entry.bind('<Up>', self.history_up)
-        self.command_entry.bind('<Down>', self.history_down)
-        self.command_history = []
-        self.command_history_index = 0
-        if not isinstance(command_history_buffer_size, (int, float)):
-            raise TypeError('command_history_buffer_size must be a number')
-        self.command_history_buffer_size = (
-            command_history_buffer_size if command_history_buffer_size > 0 else 0
-        )
-        # Hides the command entry if allow_python and allow_shell are False
-        if not allow_python and not allow_shell:
-            self.command_entry.grid_remove()
-        if allow_python:
-            raise NotImplementedError('Python commands are not supported yet!')
-        self.__allow_python = False
-        self.__allow_shell = allow_shell
-
-        # Scroll bars
-        self.logs.config(
-            xscrollcommand=_tkinter.Scrollbar(self.window, orient=_tkinter.HORIZONTAL
-                                              ).set
-        )
-        self.logs.config(yscrollcommand=_tkinter.Scrollbar(self.window).set)
-
-        # Input related lines
-        self.getting_input_status: GettingInputStatus = (
-            GettingInputStatus.NOT_GETTING_INPUT
-        )
-        self.getting_pass = False
-        self.input_text = ''
-        # cursor counter is used for making a nice blinking cursor
-        self.__cursor_counter = 1
-        self._cursor_position = None
-        self.cursor_position = 0
-        # KeyPress event for self.logs
-        self.logs.bind('<KeyPress>', self.key_press)
-
-        self.font = font
-        self.width = width
-        self.height = height
-        self.default_foreground_color = default_foreground_color
-        self.default_background_color = default_background_color
-
-        # Events for multi-threading support
-        self.window.bind('<<hide>>', self.__hide)
-        self.window.bind('<<show>>', self.__show)
-        self.window.bind('<<clear>>', self.__clear)
-        self.window.bind('<<log>>', self.__log)
-        self.window.bind('<<input>>', self.__input)
-        self.window.bind('<<type input>>', self.__type_input)
-        self.window.bind('<<getpass>>', self.__getpass)
-        self.window.bind('<<SetAllowPython>>', self.__set_allow_python)
-        self.window.bind('<<SetAllowShell>>', self.__set_allow_shell)
-        self.window.bind('<<SetCursorPosition>>', self.__set_cursor_position)
-        self.window.bind(
-            '<<SetDefaultForegroundColor>>', self.__set_default_foreground_color
-        )
-        self.window.bind(
-            '<<SetDefaultBackgroundColor>>', self.__set_default_background_color
-        )
-        self.window.bind('<<SetFont>>', self.__set_font)
-        self.window.bind('<<SetWidth>>', self.__set_width)
-        self.window.bind('<<SetHeight>>', self.__set_height)
-
-    def addHandler(self, hdlr: _Union[_FileHandler, LoggingWindowHandler]):
-        if not isinstance(hdlr, LoggingWindowHandler, _FileHandler):
-            raise TypeError("Handler must be a FileHandler or LoggingWindowHandler")
-        super().addHandler(hdlr)
-
-    def __hide(self, _):
-        self.window.withdraw()
-
-    def __show(self, _):
-        self.window.deiconify()
-
-    def __clear(self, _):
-        self.logs.config(state=_tkinter.NORMAL)
-        self.logs.delete('1.0', _tkinter.END)
-        self.logs.config(state=_tkinter.DISABLED)
-
-    def __log(self, event):
-        data = event.data
-        if self.getting_input_status == GettingInputStatus.GETTING_INPUT:
-            raise RuntimeError(
-                'Cannot log while getting input from the user! '
-                'Please cancel the input first.'
-            )
-        super()._log(
-            data.level, data.msg, data.args, data.exc_info, data.extra, data.stack_info,
-            data.stacklevel
-        )
-
-    def __input(self, event):
-        data = event.data
-        msg = ' '.join([str(m) for m in data.msg]) + data.end
-        self._log(
-            self.level if self.level >= _NOTSET else _NOTSET, msg, data.args,
-            **data.kwargs
-        )
-        self.input_text = ''
-        self.getting_input_status = GettingInputStatus.GETTING_INPUT
-        self.cursor_position = 0
-        self.logs.focus()
-        try:
-            while self.getting_input_status == GettingInputStatus.GETTING_INPUT:
-                self.cursor_position = self.cursor_position
-                self.window.update()
-                self.window.after(10)
-        except KeyboardInterrupt:
-            self.input_text = ''
-            self.getting_input_status = GettingInputStatus.NOT_GETTING_INPUT
-
-        if self.getting_input_status == GettingInputStatus.NOT_GETTING_INPUT:
-            data.output = self.input_text
-        elif self.getting_input_status == GettingInputStatus.CANCELLED:
-            if data.raise_error:
-                raise CancelledInputError('Input cancelled!')
-            data.output = ''
-
-    def __type_input(self, event):
-        data = event.data
-        if (self.getting_input_status
-                != GettingInputStatus.GETTING_INPUT) and data.wait <= 0:
-            raise RuntimeError(
-                'The logger must be getting input for this method to work! '
-                'Use `input` method or set the `wait` argument to '
-                'a value greater than 0.'
-            )
-        while self.getting_input_status != GettingInputStatus.GETTING_INPUT:
-            _sleep(data.wait)
-        self.input_text += data.text
-        self.logs.config(state=_tkinter.NORMAL)
-        self.logs.delete(f'end-{len(self.input_text) + 1}c', 'end-1c')
-        self.logs.insert(_tkinter.END, self.input_text)
-        self.logs.config(state=_tkinter.DISABLED)
-        self.cursor_position = len(self.input_text) - 1
-
-    def __getpass(self, event):
-        data = event.data
-        msg = ' '.join([str(m) for m in data.msg]) + data.end
-        self._log(
-            self.level if self.level >= _NOTSET else _NOTSET, msg, data.args,
-            **data.kwargs
-        )
-        self.input_text = ''
-        self.getting_pass = True
-        self.cursor_position = 0
-        self.logs.focus()
-        try:
-            while self.getting_pass:
-                self.cursor_position = self.cursor_position
-                self.window.update()
-                self.window.after(10)
-        except KeyboardInterrupt:
-            self.input_text = ''
-            self.getting_pass = False
-        data.output = self.input_text
-
-    def hide(self):
-        """Hides the LoggingWindow.
-
-        :return:
-        """
-        self.window.event_generate('<<hide>>')
-
-    def show(self):
-        """Shows the LoggingWindow.
-
-        :return:
-        """
-        self.window.event_generate('<<show>>')
-
-    def clear(self):
-        """Clears the LoggingWindow.
-
-        :return:
-        """
-        self.window.event_generate('<<clear>>')
-
-    def _log(
-        self,
-        level,
-        msg,
-        args,
-        exc_info=None,
-        extra=None,
-        stack_info=False,
-        stacklevel=1
-    ):
-        _lock.acquire()
-        self.window.event_generate(
-            '<<log>>',
-            when='tail',
-            data=_Namespace(
-                level=level,
-                msg=msg,
-                args=args,
-                exc_info=exc_info,
-                extra=extra,
-                stack_info=stack_info,
-                stacklevel=stacklevel
-            )
-        )
-        _lock.release()
-
-    def input(
-        self,
-        *msg,
-        args: tuple = (),
-        end='',
-        raise_error: str = False,
-        **kwargs
-    ) -> str:
-        """Prints a message and waits for input.
-
-        :param msg: The message to print.
-        :param args: The arguments to pass to the message.
-        :param end: The end of the message.
-        :param raise_error: If True, raises an error instead of
-            returning an empty string.
-        :param kwargs:
-        :return: The input.
-        """
-        _lock.acquire()
-        data = _Namespace(
-            msg=msg, args=args, end=end, raise_error=raise_error, kwargs=kwargs
-        )
-        self.window.event_generate('<<input>>', when='tail', data=data)
-        _lock.release()
-        return data.output
-
-    def cancel_input(self) -> str:
-        """Cancels the input.
-
-        :return: Part of the input that the user has typed
-        """
-        if self.getting_input_status != GettingInputStatus.GETTING_INPUT:
-            raise RuntimeError(
-                'The logger must be getting input for this method to work! '
-                'Use `input` method.'
-            )
-        self.getting_input_status = GettingInputStatus.CANCELLED
-        return self.input_text
-
-    def type_input(self, text: str, wait: _Union[int, float, bool] = False):
-        """Types some text as a part of the input that the user can edit and
-        enter.
-
-        :param text: The text to type for the user
-        :param wait: Wait until the input function is called and then
-            type the text
-        :return:
-        """
-        self.window.event_generate(
-            '<<type input>>', when='tail', data=_Namespace(text=text, wait=wait)
-        )
-
-    def getpass(self, *msg, args: tuple = (), end='', **kwargs) -> str:
-        """Prints a message and waits for input.
-
-        :param msg: The message to print.
-        :param args: The arguments to pass to the message.
-        :param end: The end of the message.
-        :param kwargs:
-        :return: The input.
-        """
-        _lock.acquire()
-        data = _Namespace(msg=msg, args=args, end=end, kwargs=kwargs)
-        self.window.event_generate('<<getpass>>', when='tail', data=data)
-        _lock.release()
-        return data.output
-
-    def key_press(self, event):  # pylint: disable=too-many-branches
-        """KeyPress event callback for self.logs."""
-        if (self.getting_input_status == GettingInputStatus.GETTING_INPUT
-                or self.getting_pass):
-            # Handles Enter key
-            if event.keysym == 'Return':
-                self.getting_input_status = GettingInputStatus.NOT_GETTING_INPUT
-                self.getting_pass = False
-                self.cursor_position = 0
-                self.logs.config(state=_tkinter.NORMAL)
-                self.logs.insert(_tkinter.END, '\n')
-                self.logs.config(state=_tkinter.DISABLED)
-                self.logs.see(_tkinter.END)
-            # Handles Backspace key
-            elif event.keysym == 'BackSpace':
-                if self.input_text:
-                    self.logs.config(state=_tkinter.NORMAL)
-                    self.logs.delete(f'end-{len(self.input_text) + 1}c', 'end-1c')
-                    self.input_text = self.input_text[:self.cursor_position - 1] + \
-                                      self.input_text[self.cursor_position:]
-                    if self.getting_pass:
-                        self.logs.insert(_tkinter.END, '*' * len(self.input_text))
-                    else:
-                        self.logs.insert(_tkinter.END, self.input_text)
-                    self.logs.config(state=_tkinter.DISABLED)
-                    self.cursor_position -= 1
-            # Handles Right Arrow
-            elif event.keysym == 'Right':
-                if self.cursor_position < len(self.input_text
-                                              ) and not self.getting_pass:
-                    self.cursor_position += 1
-            # Handles Left Arrow
-            elif event.keysym == 'Left':
-                if self.cursor_position > 0 and not self.getting_pass:
-                    self.cursor_position -= 1
-            # Handles other keys
-            elif event.char:
-                self.logs.config(state=_tkinter.NORMAL)
-                self.logs.delete(f'end-{len(self.input_text) + 1}c', 'end-1c')
-                self.input_text = (
-                    self.input_text[:self.cursor_position] + event.char +
-                    self.input_text[self.cursor_position:]
-                )
-                if self.getting_pass:
-                    self.logs.insert(_tkinter.END, '*' * len(self.input_text))
-                else:
-                    self.logs.insert(_tkinter.END, self.input_text)
-                self.logs.config(state=_tkinter.DISABLED)
-                self.cursor_position += 1
-
-    def execute_command(self, _):
-        """Executes the command in self.command_entry."""
-        command = self.command_entry.get()
-        self.command_entry.delete(0, _tkinter.END)
-        self.command_history.append(command)
-        self.command_history = self.command_history[-self.command_history_buffer_size:]
-        # FIXME: It doesn't support multiline commands yet
-        # Shell commands:
-        if command.startswith('!'):
-            if self.allow_shell:
-                try:
-                    # TODO: Add the support of interactive programmes such as python
-                    # shell and bash
-                    output = _subprocess.check_output(command[1:].strip(), shell=False)
-                    self.print(output.decode('utf-8').strip('\r\n'))
-                except _subprocess.CalledProcessError as ex:
-                    self.error(
-                        'Error code:', ex.returncode,
-                        ex.output.decode('utf-8').strip('\r\n')
-                    )
-                except FileNotFoundError:
-                    self.error('File not found: Unrecognized command.')
-                except Exception as ex:  # pylint: disable=broad-except
-                    self.error(ex)
-            else:
-                self.error('Shell commands are not allowed!')
-        # Python commands:
-        else:
-            if self.allow_python:
-                try:
-                    # TODO: Add the support of python commands
-                    raise NotImplementedError
-                except Exception as ex:  # pylint: disable=broad-except
-                    self.error(ex)
-            else:
-                try:
-                    output = _subprocess.check_output(command.strip(), shell=False)
-                    self.print(output.decode('utf-8').strip('\r\n'))
-                except _subprocess.CalledProcessError as ex:
-                    self.error(
-                        'Error code:', ex.returncode,
-                        ex.output.decode('utf-8').strip('\r\n')
-                    )
-                except FileNotFoundError:
-                    self.error('File not found: Unrecognized command.')
-                except Exception as ex: # pylint: disable=broad-except
-                    self.error(ex)
-        self.command_history_index = len(self.command_history)
-
-    def history_up(self, _):
-        """Moves up the command history."""
-        _lock.acquire()
-        if self.command_history_index > 0:
-            self.command_history_index -= 1
-            self.command_entry.delete(0, _tkinter.END)
-            self.command_entry.insert(
-                0, self.command_history[self.command_history_index]
-            )
-        _lock.release()
-
-    def history_down(self, _):
-        """Moves down the command history."""
-        _lock.acquire()
-        if self.command_history_index < len(self.command_history) - 1:
-            self.command_history_index += 1
-            self.command_entry.delete(0, _tkinter.END)
-            self.command_entry.insert(
-                0, self.command_history[self.command_history_index]
-            )
-        else:
-            self.command_entry.delete(0, _tkinter.END)
-        _lock.release()
-
-    def __set_allow_python(self, event):
-        """Sets the allow_python attribute."""
-        self.__allow_python = event.data
-        # Hides the command entry if allow_python and allow_shell are False
-        if not self.__allow_python and not self.__allow_shell:
-            self.command_entry.grid_remove()
-        # Shows the command entry if allow_python or allow_shell are True
-        else:
-            self.command_entry.grid(row=1, column=0, sticky='nsew')
-
-    def __set_allow_shell(self, event):
-        """Sets the allow_shell attribute."""
-        self.__allow_shell = event.data
-        # Hides the command entry if allow_python and allow_shell are False
-        if not self.__allow_python and not self.__allow_shell:
-            self.command_entry.grid_remove()
-        # Shows the command entry if allow_python or allow_shell are True
-        else:
-            self.command_entry.grid(row=1, column=0, sticky='nsew')
-
-    def __set_cursor_position(self, event):
-        """Sets the cursor_position attribute."""
-        new_value = self.cursor_position != event.data
-
-        # Removes the cursor from the last position
-        if self.cursor_position is not None and (self.__cursor_counter % 50 == 0
-                                                 or new_value):
-            index = self.logs.index(
-                f'end-{len(self.input_text) - self.cursor_position + 2}c'
-            )
-            self.logs.tag_add(
-                index, index, f'end-{len(self.input_text) - self.cursor_position + 1}c'
-            )
-            self.logs.tag_config(
-                index,
-                background=self.default_background_color,
-                foreground=self.default_foreground_color
-            )
-        self._cursor_position = event.data
-
-        self.__cursor_counter += 1
-        # Places the new cursor
-        if self.getting_input_status == GettingInputStatus.GETTING_INPUT and (
-                self.__cursor_counter % 100 == 0 or new_value):
-            self.__cursor_counter = 1
-            index = self.logs.index(
-                f'end-{len(self.input_text) - self.cursor_position + 2}c'
-            )
-            self.logs.tag_add(
-                index, index, f'end-{len(self.input_text) - self.cursor_position + 1}c'
-            )
-            self.logs.tag_config(
-                index,
-                background=self.default_foreground_color,
-                foreground=self.default_background_color
-            )
-
-    def __set_default_foreground_color(self, event):
-        """Sets the default_foreground_color attribute."""
-        self._default_foreground_color = event.data
-        self.logs.config(foreground=event.data)
-
-    def __set_default_background_color(self, event):
-        """Sets the default_background_color attribute."""
-        self._default_background_color = event.data
-        self.logs.config(background=event.data)
-
-    def __set_font(self, event):
-        """Sets the font attribute."""
-        self.logs.config(font=event.data)
-
-    def __set_width(self, event):
-        """Sets the width attribute."""
-        self.logs.config(width=event.data)
-
-    def __set_height(self, event):
-        """Sets the height attribute."""
-        self.logs.config(height=event.data)
-
-    @property
-    def allow_python(self):
-        return self.__allow_python
-
-    @allow_python.setter
-    def allow_python(self, value):
-        raise NotImplementedError('Python commands are not supported yet!')
-        self.window.event_generate('<<SetAllowPython>>', when='tail', data=value)
-
-    @property
-    def allow_shell(self):
-        return self.__allow_shell
-
-    @allow_shell.setter
-    def allow_shell(self, value):
-        self.window.event_generate('<<SetAllowShell>>', when='tail', data=value)
-
-    @property
-    def cursor_position(self):
-        return self._cursor_position
-
-    @cursor_position.setter
-    def cursor_position(self, value):
-        self.window.event_generate('<<SetCursorPosition>>', when='tail', data=value)
-
-    @property
-    def default_foreground_color(self):
-        return self._default_foreground_color
-
-    @default_foreground_color.setter
-    def default_foreground_color(self, value):
-        self.window.event_generate(
-            '<<SetDefaultForegroundColor>>', when='tail', data=value
-        )
-
-    @property
-    def default_background_color(self):
-        return self._default_background_color
-
-    @default_background_color.setter
-    def default_background_color(self, value):
-        self.window.event_generate(
-            '<<SetDefaultBackgroundColor>>', when='tail', data=value
-        )
-
-    @property
-    def font(self):
-        return self.logs.config()['font']
-
-    @font.setter
-    def font(self, value):
-        self.window.event_generate('<<SetFont>>', when='tail', data=value)
-
-    @property
-    def width(self):
-        return self.logs.config()['width'][-1]
-
-    @width.setter
-    def width(self, value):
-        self.window.event_generate('<<SetWidth>>', when='tail', data=value)
-
-    @property
-    def height(self):
-        return self.logs.config()['height'][-1]
-
-    @height.setter
-    def height(self, value):
-        self.window.event_generate('<<SetHeight>>', when='tail', data=value)
-
-    @property
-    def progress_bar(self):
-        if not self._progress_bar:
-            # Import here to avoid circular import
-            # pylint: disable=import-outside-toplevel
-            from log21.ProgressBar import ProgressBar
-            self._progress_bar = ProgressBar(logger=self, width=self.width)
-        self.window.update()
-        return self._progress_bar
-
-    def __del__(self):
-        self.window.withdraw()
-        self.window.destroy()
-        del self.window
-
-
-if not _tkinter:
-
-    class LoggingWindow:  # pylint: disable=function-redefined
-        """LoggingWindow requires tkinter to be installed."""
-
-        def __init__(self, *args, **kwargs):
-            raise ImportError('LoggingWindow requires tkinter to be installed.')
-
-    class LoggingWindowHandler:  # pylint: disable=function-redefined
-        """LoggingWindow requires tkinter to be installed."""
-
-        def __init__(self, *args, **kwargs):
-            raise ImportError('LoggingWindow requires tkinter to be installed.')
+# log21.LoggingWindow.py
+# CodeWriter2
+
+from __future__ import annotations
+
+import re as _re
+import threading as _threading
+import subprocess as _subprocess
+from enum import Enum as _Enum
+from time import sleep as _sleep
+from uuid import uuid4 as _uuid4
+from string import printable as _printable
+from typing import Union as _Union
+from logging import FileHandler as _FileHandler
+from argparse import Namespace as _Namespace
+
+from log21.Colors import hex_escape as _hex_escape, ansi_escape as _ansi_escape
+from log21.Levels import NOTSET as _NOTSET
+from log21.Logger import Logger as _Logger
+from log21.StreamHandler import StreamHandler as _StreamHandler
+
+__all__ = ['LoggingWindow', 'LoggingWindowHandler']
+
+try:
+    import tkinter as _tkinter
+except ImportError:
+    _tkinter = None
+
+ansi_to_hex_color_map = {
+    # https://chrisyeh96.github.io/2020/03/28/terminal-colors.html
+    '30': ('#000000', 'foreground'),  # Black foreground
+    '31': ('#cc0000', 'foreground'),  # Red foreground
+    '32': ('#4e9a06', 'foreground'),  # Green foreground
+    '33': ('#c4a000', 'foreground'),  # Yellow foreground
+    '34': ('#729fcf', 'foreground'),  # Blue foreground
+    '35': ('#75507b', 'foreground'),  # Magenta foreground
+    '36': ('#06989a', 'foreground'),  # Cyan foreground
+    '37': ('#d3d7cf', 'foreground'),  # White foreground
+    '90': ('#555753', 'foreground'),  # Bright black foreground
+    '91': ('#ef2929', 'foreground'),  # Bright red foreground
+    '92': ('#8ae234', 'foreground'),  # Bright green foreground
+    '93': ('#fce94f', 'foreground'),  # Bright yellow foreground
+    '94': ('#32afff', 'foreground'),  # Bright blue foreground
+    '95': ('#ad7fa8', 'foreground'),  # Bright magenta foreground
+    '96': ('#34e2e2', 'foreground'),  # Bright cyan foreground
+    '97': ('#ffffff', 'foreground'),  # Bright white foreground
+    '40': ('#000000', 'background'),  # Black background
+    '41': ('#cc0000', 'background'),  # Red background
+    '42': ('#4e9a06', 'background'),  # Green background
+    '43': ('#c4a000', 'background'),  # Yellow background
+    '44': ('#729fcf', 'background'),  # Blue background
+    '45': ('#75507b', 'background'),  # Magenta background
+    '46': ('#06989a', 'background'),  # Cyan background
+    '47': ('#d3d7cf', 'background'),  # White background
+    '100': ('#555753', 'background'),  # Bright black background
+    '101': ('#ef2929', 'background'),  # Bright red background
+    '102': ('#8ae234', 'background'),  # Bright green background
+    '103': ('#fce94f', 'background'),  # Bright yellow background
+    '104': ('#32afff', 'background'),  # Bright blue background
+    '105': ('#ad7fa8', 'background'),  # Bright magenta background
+    '106': ('#34e2e2', 'background'),  # Bright cyan background
+    '107': ('#ffffff', 'background'),  # Bright white background
+}
+
+_lock = _threading.RLock()
+
+
+class GettingInputStatus(_Enum):
+    """An enum for the status of getting input."""
+    NOT_GETTING_INPUT = 0
+    GETTING_INPUT = 1
+    CANCELLED = 2
+
+
+class CancelledInputError(InterruptedError, Exception):
+    """An exception raised when the input is cancelled."""
+
+
+class LoggingWindowHandler(_StreamHandler):
+    """A handler for logging to a LoggingWindow."""
+
+    def __init__(
+        self,
+        logging_window: LoggingWindow,
+        handle_carriage_return: bool = True,
+        handle_new_line: bool = True
+    ):
+        """Initialize the LoggingWindowHandler.
+
+        :param logging_window: The LoggingWindow to log to.
+        :param handle_carriage_return: Whether to handle carriage
+            returns.
+        :param handle_new_line: Whether to handle new lines.
+        """
+        self.HandleCR = handle_carriage_return
+        self.HandleNL = handle_new_line
+        self.__carriage_return: bool = False
+        self.LoggingWindow = logging_window  # pylint: disable=invalid-name
+        super().__init__(stream=None)
+
+    def emit(self, record):
+        try:
+            if self.HandleCR:
+                self.check_cr(record)
+            if self.HandleNL:
+                self.check_nl(record)
+            msg = self.format(record)
+            self.write(msg)
+            self.write(self.terminator)
+        except Exception:  # pylint: disable=broad-except
+            self.handleError(record)
+
+    def write(self, message):  # pylint: disable=too-many-branches
+        """Write a message to the LoggingWindow.
+
+        :param message: The message to write.
+        """
+        if self.LoggingWindow is not None:  # pylint: disable=too-many-nested-blocks
+            # Sets the element's state to normal so that it can be modified.
+            self.LoggingWindow.logs.config(state=_tkinter.NORMAL)
+
+            # Handles carriage return
+            parts = _re.split(r'(\r)', message)
+
+            while parts:
+                part = parts.pop(0)
+
+                if self.__carriage_return:
+                    # Checks if the part is printable
+                    if any((char in _printable[:-6])
+                           for char in _hex_escape.sub('', _ansi_escape.sub('', part))):
+                        # Removes the last line
+                        self.LoggingWindow.logs.delete('end - 1 lines', _tkinter.END)
+                        if self.LoggingWindow.logs.count('0.0', 'end')[0] != 1:
+                            self.LoggingWindow.logs.insert('end', '\n')
+                        self.__carriage_return = False
+
+                tags = []
+                # Handles ANSI color codes
+                ansi_parts = _ansi_escape.split(part)
+                while ansi_parts:
+                    ansi_text = ansi_parts.pop(0)
+
+                    if ansi_text:
+                        # Handles HEX color codes
+                        hex_parts = _hex_escape.split(ansi_text)
+                        while hex_parts:
+                            hex_text = hex_parts.pop(0)
+
+                            if hex_text:
+                                self.LoggingWindow.logs.insert(_tkinter.END, hex_text)
+
+                            if hex_parts:
+                                hex_color = hex_parts.pop(0)
+
+                                tag = str(_uuid4())
+                                # Foreground color
+                                if hex_parts.pop(0) == 'f':
+                                    tags.append(
+                                        {
+                                            'name': tag,
+                                            'start':
+                                            self.LoggingWindow.logs.index('end-1c'),
+                                            'config': {
+                                                'foreground': hex_color
+                                            }
+                                        }
+                                    )
+                                # Background color
+                                else:
+                                    tags.append(
+                                        {
+                                            'name': tag,
+                                            'start':
+                                            self.LoggingWindow.logs.index('end-1c'),
+                                            'config': {
+                                                'background': hex_color
+                                            }
+                                        }
+                                    )
+
+                    if ansi_parts:
+                        ansi_params = ansi_parts.pop(0).split(';')
+                        ansi_color = {'foreground': None, 'background': None}
+
+                        for part in ansi_params:
+                            if part in ansi_to_hex_color_map:
+                                color_ = ansi_to_hex_color_map[part]
+                                ansi_color[color_[1]] = color_[0]
+                            elif part == '0':
+                                ansi_color[
+                                    'foreground'
+                                ] = self.LoggingWindow.default_foreground_color
+                                ansi_color[
+                                    'background'
+                                ] = self.LoggingWindow.default_background_color
+                            else:
+                                pass  # error condition ignored
+                        if ansi_color['foreground'] or ansi_color['background']:
+                            tags.append(
+                                {
+                                    'name': str(_uuid4()),
+                                    'start': self.LoggingWindow.logs.index('end-1c'),
+                                    'config': ansi_color
+                                }
+                            )
+
+                # Applies the color tags
+                for tag in tags:
+                    self.LoggingWindow.logs.tag_add(tag['name'], tag['start'], 'end')
+                    self.LoggingWindow.logs.tag_config(tag['name'], **tag['config'])
+
+                if parts:
+                    parts.pop(0)
+                    self.__carriage_return = True
+
+            self.LoggingWindow.logs.config(state=_tkinter.DISABLED)
+            self.LoggingWindow.logs.see(_tkinter.END)
+
+
+class LoggingWindow(_Logger):  # pylint: disable=too-many-instance-attributes
+    """
+    Usage Example:
+        >>> # Manual creation
+        >>> # Imports the LoggingWindow and LoggingWindowHandler classes
+        >>> from log21 import LoggingWindow, LoggingWindowHandler
+        >>> # Creates a new LoggingWindow object
+        >>> window = LoggingWindow('Test Window', level='DEBUG')
+        >>> # Creates a new LoggingWindowHandler object and adds it to the LoggingWindow
+        >>> # we created earlier
+        >>> window.addHandler(LoggingWindowHandler(window))
+        >>> window.debug('A debug message')
+        >>> window.info('An info message')
+        >>> # Run these lines to see the messages in the window
+        >>>
+        >>> # Automatic creation
+        >>> # Imports log21 and time modules
+        >>> import log21, time
+        >>> # Creates a new LoggingWindow object
+        >>> window = log21.get_logging_window('Test Window')
+        >>> # Use it without any additional steps to add handlers and formatters
+        >>> window.info('This works properly!')
+        >>> # ANSI colors usage:
+        >>> window.info('This is a \033[91mred\033[0m message.')
+        >>> window.info('\033[102mThis is a message with green background.')
+        >>> # HEX colors usage:
+        >>> window.info('\033#00FFFFhfThis is a message with cyan foreground.')
+        >>> window.info('\033#0000FFhbThis is a message with blue background.')
+        >>> # Progressbar usage:
+        >>> for i in range(100):
+        ...     window.print_progress(i + 1, 100)
+        ...     time.sleep(0.1)
+        ...
+        >>> # Gettig input from the user:
+        >>> name: str = window.input('Enter your name: ')
+        >>> window.print('Hello, ' + name + '!')
+        >>> # Run these lines to see the messages in the window
+        >>>
+
+    """
+
+    def __init__(
+        self,
+        name,
+        level=_NOTSET,
+        width: int = 80,
+        height: int = 20,
+        default_foreground_color='white',
+        default_background_color='black',
+        font=('Courier', 10),
+        allow_python: bool = False,
+        allow_shell: bool = False,
+        command_history_buffer_size: int = 100
+    ):  # pylint: disable=too-many-statements
+        """Creates a new LoggingWindow object.
+
+        :param name: The name of the logger.
+        :param level: The level of the logger.
+        :param width: The width of the LoggingWindow.
+        :param height: The height of the LoggingWindow.
+        :param default_foreground_color: The default foreground color of
+            the LoggingWindow.
+        :param default_background_color: The default background color of
+            the LoggingWindow.
+        :param font: The font of the LoggingWindow.
+        """
+        super().__init__(name, level)
+        self.window = _tkinter.Tk()
+        self.window.title(name)
+        # Hides window instead of closing it
+        self.window.protocol("WM_DELETE_WINDOW", self.hide)
+
+        self.window.resizable(False, False)
+
+        self.logs = _tkinter.Text(self.window)
+        self.logs.grid(row=0, column=0, sticky='nsew')
+        self.logs.config(state=_tkinter.DISABLED)
+        self.logs.config(wrap=_tkinter.NONE)
+
+        # Commands entry
+        self.command_entry = _tkinter.Entry(self.window)
+        self.command_entry.grid(row=1, column=0, sticky='nsew')
+        self.command_entry.bind('<Return>', self.execute_command)
+        self.command_entry.bind('<Up>', self.history_up)
+        self.command_entry.bind('<Down>', self.history_down)
+        self.command_history = []
+        self.command_history_index = 0
+        if not isinstance(command_history_buffer_size, (int, float)):
+            raise TypeError('command_history_buffer_size must be a number')
+        self.command_history_buffer_size = (
+            command_history_buffer_size if command_history_buffer_size > 0 else 0
+        )
+        # Hides the command entry if allow_python and allow_shell are False
+        if not allow_python and not allow_shell:
+            self.command_entry.grid_remove()
+        if allow_python:
+            raise NotImplementedError('Python commands are not supported yet!')
+        self.__allow_python = False
+        self.__allow_shell = allow_shell
+
+        # Scroll bars
+        self.logs.config(
+            xscrollcommand=_tkinter.Scrollbar(self.window, orient=_tkinter.HORIZONTAL
+                                              ).set
+        )
+        self.logs.config(yscrollcommand=_tkinter.Scrollbar(self.window).set)
+
+        # Input related lines
+        self.getting_input_status: GettingInputStatus = (
+            GettingInputStatus.NOT_GETTING_INPUT
+        )
+        self.getting_pass = False
+        self.input_text = ''
+        # cursor counter is used for making a nice blinking cursor
+        self.__cursor_counter = 1
+        self._cursor_position = None
+        self.cursor_position = 0
+        # KeyPress event for self.logs
+        self.logs.bind('<KeyPress>', self.key_press)
+
+        self.font = font
+        self.width = width
+        self.height = height
+        self.default_foreground_color = default_foreground_color
+        self.default_background_color = default_background_color
+
+        # Events for multi-threading support
+        self.window.bind('<<hide>>', self.__hide)
+        self.window.bind('<<show>>', self.__show)
+        self.window.bind('<<clear>>', self.__clear)
+        self.window.bind('<<log>>', self.__log)
+        self.window.bind('<<input>>', self.__input)
+        self.window.bind('<<type input>>', self.__type_input)
+        self.window.bind('<<getpass>>', self.__getpass)
+        self.window.bind('<<SetAllowPython>>', self.__set_allow_python)
+        self.window.bind('<<SetAllowShell>>', self.__set_allow_shell)
+        self.window.bind('<<SetCursorPosition>>', self.__set_cursor_position)
+        self.window.bind(
+            '<<SetDefaultForegroundColor>>', self.__set_default_foreground_color
+        )
+        self.window.bind(
+            '<<SetDefaultBackgroundColor>>', self.__set_default_background_color
+        )
+        self.window.bind('<<SetFont>>', self.__set_font)
+        self.window.bind('<<SetWidth>>', self.__set_width)
+        self.window.bind('<<SetHeight>>', self.__set_height)
+
+    def addHandler(self, hdlr: _Union[_FileHandler, LoggingWindowHandler]):
+        if not isinstance(hdlr, LoggingWindowHandler, _FileHandler):
+            raise TypeError("Handler must be a FileHandler or LoggingWindowHandler")
+        super().addHandler(hdlr)
+
+    def __hide(self, _):
+        self.window.withdraw()
+
+    def __show(self, _):
+        self.window.deiconify()
+
+    def __clear(self, _):
+        self.logs.config(state=_tkinter.NORMAL)
+        self.logs.delete('1.0', _tkinter.END)
+        self.logs.config(state=_tkinter.DISABLED)
+
+    def __log(self, event):
+        data = event.data
+        if self.getting_input_status == GettingInputStatus.GETTING_INPUT:
+            raise RuntimeError(
+                'Cannot log while getting input from the user! '
+                'Please cancel the input first.'
+            )
+        super()._log(
+            data.level, data.msg, data.args, data.exc_info, data.extra, data.stack_info,
+            data.stacklevel
+        )
+
+    def __input(self, event):
+        data = event.data
+        msg = ' '.join([str(m) for m in data.msg]) + data.end
+        self._log(
+            self.level if self.level >= _NOTSET else _NOTSET, msg, data.args,
+            **data.kwargs
+        )
+        self.input_text = ''
+        self.getting_input_status = GettingInputStatus.GETTING_INPUT
+        self.cursor_position = 0
+        self.logs.focus()
+        try:
+            while self.getting_input_status == GettingInputStatus.GETTING_INPUT:
+                self.cursor_position = self.cursor_position
+                self.window.update()
+                self.window.after(10)
+        except KeyboardInterrupt:
+            self.input_text = ''
+            self.getting_input_status = GettingInputStatus.NOT_GETTING_INPUT
+
+        if self.getting_input_status == GettingInputStatus.NOT_GETTING_INPUT:
+            data.output = self.input_text
+        elif self.getting_input_status == GettingInputStatus.CANCELLED:
+            if data.raise_error:
+                raise CancelledInputError('Input cancelled!')
+            data.output = ''
+
+    def __type_input(self, event):
+        data = event.data
+        if (self.getting_input_status
+                != GettingInputStatus.GETTING_INPUT) and data.wait <= 0:
+            raise RuntimeError(
+                'The logger must be getting input for this method to work! '
+                'Use `input` method or set the `wait` argument to '
+                'a value greater than 0.'
+            )
+        while self.getting_input_status != GettingInputStatus.GETTING_INPUT:
+            _sleep(data.wait)
+        self.input_text += data.text
+        self.logs.config(state=_tkinter.NORMAL)
+        self.logs.delete(f'end-{len(self.input_text) + 1}c', 'end-1c')
+        self.logs.insert(_tkinter.END, self.input_text)
+        self.logs.config(state=_tkinter.DISABLED)
+        self.cursor_position = len(self.input_text) - 1
+
+    def __getpass(self, event):
+        data = event.data
+        msg = ' '.join([str(m) for m in data.msg]) + data.end
+        self._log(
+            self.level if self.level >= _NOTSET else _NOTSET, msg, data.args,
+            **data.kwargs
+        )
+        self.input_text = ''
+        self.getting_pass = True
+        self.cursor_position = 0
+        self.logs.focus()
+        try:
+            while self.getting_pass:
+                self.cursor_position = self.cursor_position
+                self.window.update()
+                self.window.after(10)
+        except KeyboardInterrupt:
+            self.input_text = ''
+            self.getting_pass = False
+        data.output = self.input_text
+
+    def hide(self):
+        """Hides the LoggingWindow.
+
+        :return:
+        """
+        self.window.event_generate('<<hide>>')
+
+    def show(self):
+        """Shows the LoggingWindow.
+
+        :return:
+        """
+        self.window.event_generate('<<show>>')
+
+    def clear(self):
+        """Clears the LoggingWindow.
+
+        :return:
+        """
+        self.window.event_generate('<<clear>>')
+
+    def _log(
+        self,
+        level,
+        msg,
+        args,
+        exc_info=None,
+        extra=None,
+        stack_info=False,
+        stacklevel=1
+    ):
+        _lock.acquire()
+        self.window.event_generate(
+            '<<log>>',
+            when='tail',
+            data=_Namespace(
+                level=level,
+                msg=msg,
+                args=args,
+                exc_info=exc_info,
+                extra=extra,
+                stack_info=stack_info,
+                stacklevel=stacklevel
+            )
+        )
+        _lock.release()
+
+    def input(
+        self,
+        *msg,
+        args: tuple = (),
+        end='',
+        raise_error: str = False,
+        **kwargs
+    ) -> str:
+        """Prints a message and waits for input.
+
+        :param msg: The message to print.
+        :param args: The arguments to pass to the message.
+        :param end: The end of the message.
+        :param raise_error: If True, raises an error instead of
+            returning an empty string.
+        :param kwargs:
+        :return: The input.
+        """
+        _lock.acquire()
+        data = _Namespace(
+            msg=msg, args=args, end=end, raise_error=raise_error, kwargs=kwargs
+        )
+        self.window.event_generate('<<input>>', when='tail', data=data)
+        _lock.release()
+        return data.output
+
+    def cancel_input(self) -> str:
+        """Cancels the input.
+
+        :return: Part of the input that the user has typed
+        """
+        if self.getting_input_status != GettingInputStatus.GETTING_INPUT:
+            raise RuntimeError(
+                'The logger must be getting input for this method to work! '
+                'Use `input` method.'
+            )
+        self.getting_input_status = GettingInputStatus.CANCELLED
+        return self.input_text
+
+    def type_input(self, text: str, wait: _Union[int, float, bool] = False):
+        """Types some text as a part of the input that the user can edit and
+        enter.
+
+        :param text: The text to type for the user
+        :param wait: Wait until the input function is called and then
+            type the text
+        :return:
+        """
+        self.window.event_generate(
+            '<<type input>>', when='tail', data=_Namespace(text=text, wait=wait)
+        )
+
+    def getpass(self, *msg, args: tuple = (), end='', **kwargs) -> str:
+        """Prints a message and waits for input.
+
+        :param msg: The message to print.
+        :param args: The arguments to pass to the message.
+        :param end: The end of the message.
+        :param kwargs:
+        :return: The input.
+        """
+        _lock.acquire()
+        data = _Namespace(msg=msg, args=args, end=end, kwargs=kwargs)
+        self.window.event_generate('<<getpass>>', when='tail', data=data)
+        _lock.release()
+        return data.output
+
+    def key_press(self, event):  # pylint: disable=too-many-branches
+        """KeyPress event callback for self.logs."""
+        if (self.getting_input_status == GettingInputStatus.GETTING_INPUT
+                or self.getting_pass):
+            # Handles Enter key
+            if event.keysym == 'Return':
+                self.getting_input_status = GettingInputStatus.NOT_GETTING_INPUT
+                self.getting_pass = False
+                self.cursor_position = 0
+                self.logs.config(state=_tkinter.NORMAL)
+                self.logs.insert(_tkinter.END, '\n')
+                self.logs.config(state=_tkinter.DISABLED)
+                self.logs.see(_tkinter.END)
+            # Handles Backspace key
+            elif event.keysym == 'BackSpace':
+                if self.input_text:
+                    self.logs.config(state=_tkinter.NORMAL)
+                    self.logs.delete(f'end-{len(self.input_text) + 1}c', 'end-1c')
+                    self.input_text = self.input_text[:self.cursor_position - 1] + \
+                                      self.input_text[self.cursor_position:]
+                    if self.getting_pass:
+                        self.logs.insert(_tkinter.END, '*' * len(self.input_text))
+                    else:
+                        self.logs.insert(_tkinter.END, self.input_text)
+                    self.logs.config(state=_tkinter.DISABLED)
+                    self.cursor_position -= 1
+            # Handles Right Arrow
+            elif event.keysym == 'Right':
+                if self.cursor_position < len(self.input_text
+                                              ) and not self.getting_pass:
+                    self.cursor_position += 1
+            # Handles Left Arrow
+            elif event.keysym == 'Left':
+                if self.cursor_position > 0 and not self.getting_pass:
+                    self.cursor_position -= 1
+            # Handles other keys
+            elif event.char:
+                self.logs.config(state=_tkinter.NORMAL)
+                self.logs.delete(f'end-{len(self.input_text) + 1}c', 'end-1c')
+                self.input_text = (
+                    self.input_text[:self.cursor_position] + event.char +
+                    self.input_text[self.cursor_position:]
+                )
+                if self.getting_pass:
+                    self.logs.insert(_tkinter.END, '*' * len(self.input_text))
+                else:
+                    self.logs.insert(_tkinter.END, self.input_text)
+                self.logs.config(state=_tkinter.DISABLED)
+                self.cursor_position += 1
+
+    def execute_command(self, _):
+        """Executes the command in self.command_entry."""
+        command = self.command_entry.get()
+        self.command_entry.delete(0, _tkinter.END)
+        self.command_history.append(command)
+        self.command_history = self.command_history[-self.command_history_buffer_size:]
+        # FIXME: It doesn't support multiline commands yet
+        # Shell commands:
+        if command.startswith('!'):
+            if self.allow_shell:
+                try:
+                    # TODO: Add the support of interactive programmes such as python
+                    # shell and bash
+                    output = _subprocess.check_output(command[1:].strip(), shell=False)
+                    self.print(output.decode('utf-8').strip('\r\n'))
+                except _subprocess.CalledProcessError as ex:
+                    self.error(
+                        'Error code:', ex.returncode,
+                        ex.output.decode('utf-8').strip('\r\n')
+                    )
+                except FileNotFoundError:
+                    self.error('File not found: Unrecognized command.')
+                except Exception as ex:  # pylint: disable=broad-except
+                    self.error(ex)
+            else:
+                self.error('Shell commands are not allowed!')
+        # Python commands:
+        else:
+            if self.allow_python:
+                try:
+                    # TODO: Add the support of python commands
+                    raise NotImplementedError
+                except Exception as ex:  # pylint: disable=broad-except
+                    self.error(ex)
+            else:
+                try:
+                    output = _subprocess.check_output(command.strip(), shell=False)
+                    self.print(output.decode('utf-8').strip('\r\n'))
+                except _subprocess.CalledProcessError as ex:
+                    self.error(
+                        'Error code:', ex.returncode,
+                        ex.output.decode('utf-8').strip('\r\n')
+                    )
+                except FileNotFoundError:
+                    self.error('File not found: Unrecognized command.')
+                except Exception as ex: # pylint: disable=broad-except
+                    self.error(ex)
+        self.command_history_index = len(self.command_history)
+
+    def history_up(self, _):
+        """Moves up the command history."""
+        _lock.acquire()
+        if self.command_history_index > 0:
+            self.command_history_index -= 1
+            self.command_entry.delete(0, _tkinter.END)
+            self.command_entry.insert(
+                0, self.command_history[self.command_history_index]
+            )
+        _lock.release()
+
+    def history_down(self, _):
+        """Moves down the command history."""
+        _lock.acquire()
+        if self.command_history_index < len(self.command_history) - 1:
+            self.command_history_index += 1
+            self.command_entry.delete(0, _tkinter.END)
+            self.command_entry.insert(
+                0, self.command_history[self.command_history_index]
+            )
+        else:
+            self.command_entry.delete(0, _tkinter.END)
+        _lock.release()
+
+    def __set_allow_python(self, event):
+        """Sets the allow_python attribute."""
+        self.__allow_python = event.data
+        # Hides the command entry if allow_python and allow_shell are False
+        if not self.__allow_python and not self.__allow_shell:
+            self.command_entry.grid_remove()
+        # Shows the command entry if allow_python or allow_shell are True
+        else:
+            self.command_entry.grid(row=1, column=0, sticky='nsew')
+
+    def __set_allow_shell(self, event):
+        """Sets the allow_shell attribute."""
+        self.__allow_shell = event.data
+        # Hides the command entry if allow_python and allow_shell are False
+        if not self.__allow_python and not self.__allow_shell:
+            self.command_entry.grid_remove()
+        # Shows the command entry if allow_python or allow_shell are True
+        else:
+            self.command_entry.grid(row=1, column=0, sticky='nsew')
+
+    def __set_cursor_position(self, event):
+        """Sets the cursor_position attribute."""
+        new_value = self.cursor_position != event.data
+
+        # Removes the cursor from the last position
+        if self.cursor_position is not None and (self.__cursor_counter % 50 == 0
+                                                 or new_value):
+            index = self.logs.index(
+                f'end-{len(self.input_text) - self.cursor_position + 2}c'
+            )
+            self.logs.tag_add(
+                index, index, f'end-{len(self.input_text) - self.cursor_position + 1}c'
+            )
+            self.logs.tag_config(
+                index,
+                background=self.default_background_color,
+                foreground=self.default_foreground_color
+            )
+        self._cursor_position = event.data
+
+        self.__cursor_counter += 1
+        # Places the new cursor
+        if self.getting_input_status == GettingInputStatus.GETTING_INPUT and (
+                self.__cursor_counter % 100 == 0 or new_value):
+            self.__cursor_counter = 1
+            index = self.logs.index(
+                f'end-{len(self.input_text) - self.cursor_position + 2}c'
+            )
+            self.logs.tag_add(
+                index, index, f'end-{len(self.input_text) - self.cursor_position + 1}c'
+            )
+            self.logs.tag_config(
+                index,
+                background=self.default_foreground_color,
+                foreground=self.default_background_color
+            )
+
+    def __set_default_foreground_color(self, event):
+        """Sets the default_foreground_color attribute."""
+        self._default_foreground_color = event.data
+        self.logs.config(foreground=event.data)
+
+    def __set_default_background_color(self, event):
+        """Sets the default_background_color attribute."""
+        self._default_background_color = event.data
+        self.logs.config(background=event.data)
+
+    def __set_font(self, event):
+        """Sets the font attribute."""
+        self.logs.config(font=event.data)
+
+    def __set_width(self, event):
+        """Sets the width attribute."""
+        self.logs.config(width=event.data)
+
+    def __set_height(self, event):
+        """Sets the height attribute."""
+        self.logs.config(height=event.data)
+
+    @property
+    def allow_python(self):
+        return self.__allow_python
+
+    @allow_python.setter
+    def allow_python(self, value):
+        raise NotImplementedError('Python commands are not supported yet!')
+        self.window.event_generate('<<SetAllowPython>>', when='tail', data=value)
+
+    @property
+    def allow_shell(self):
+        return self.__allow_shell
+
+    @allow_shell.setter
+    def allow_shell(self, value):
+        self.window.event_generate('<<SetAllowShell>>', when='tail', data=value)
+
+    @property
+    def cursor_position(self):
+        return self._cursor_position
+
+    @cursor_position.setter
+    def cursor_position(self, value):
+        self.window.event_generate('<<SetCursorPosition>>', when='tail', data=value)
+
+    @property
+    def default_foreground_color(self):
+        return self._default_foreground_color
+
+    @default_foreground_color.setter
+    def default_foreground_color(self, value):
+        self.window.event_generate(
+            '<<SetDefaultForegroundColor>>', when='tail', data=value
+        )
+
+    @property
+    def default_background_color(self):
+        return self._default_background_color
+
+    @default_background_color.setter
+    def default_background_color(self, value):
+        self.window.event_generate(
+            '<<SetDefaultBackgroundColor>>', when='tail', data=value
+        )
+
+    @property
+    def font(self):
+        return self.logs.config()['font']
+
+    @font.setter
+    def font(self, value):
+        self.window.event_generate('<<SetFont>>', when='tail', data=value)
+
+    @property
+    def width(self):
+        return self.logs.config()['width'][-1]
+
+    @width.setter
+    def width(self, value):
+        self.window.event_generate('<<SetWidth>>', when='tail', data=value)
+
+    @property
+    def height(self):
+        return self.logs.config()['height'][-1]
+
+    @height.setter
+    def height(self, value):
+        self.window.event_generate('<<SetHeight>>', when='tail', data=value)
+
+    @property
+    def progress_bar(self):
+        if not self._progress_bar:
+            # Import here to avoid circular import
+            # pylint: disable=import-outside-toplevel
+            from log21.ProgressBar import ProgressBar
+            self._progress_bar = ProgressBar(logger=self, width=self.width)
+        self.window.update()
+        return self._progress_bar
+
+    def __del__(self):
+        self.window.withdraw()
+        self.window.destroy()
+        del self.window
+
+
+if not _tkinter:
+
+    class LoggingWindow:  # pylint: disable=function-redefined
+        """LoggingWindow requires tkinter to be installed."""
+
+        def __init__(self, *args, **kwargs):
+            raise ImportError('LoggingWindow requires tkinter to be installed.')
+
+    class LoggingWindowHandler:  # pylint: disable=function-redefined
+        """LoggingWindow requires tkinter to be installed."""
+
+        def __init__(self, *args, **kwargs):
+            raise ImportError('LoggingWindow requires tkinter to be installed.')
```

### Comparing `log21-2.8.1b0/src/log21/Manager.py` & `log21-2.9.0/src/log21/Manager.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# log21.Manager.py
-# CodeWriter21
-
-import logging as _logging
-from typing import Union as _Union
-
-from log21.Levels import INFO as _INFO
-from log21.Logger import Logger as _loggerClass
-
-root = _logging.RootLogger(_INFO)
-
-
-class Manager(_logging.Manager):
-    """The Manager class is a subclass of the logging.Manager class. It
-    overrides the getLogger method to make it more compatible with the
-    log21.Logger class. It also overrides the constructor."""
-
-    def __init__(self):
-        self.root = root
-        self.disable = 0
-        self.emittedNoHandlerWarning = False
-        self.loggerDict = {}
-        self.loggerClass = None
-        self.logRecordFactory = None
-
-    def getLogger(self, name: str) -> _Union[_logging.Logger, _loggerClass, None]:
-        """Takes the name of a logger and if there was a logger with that name
-        in the loggerDict it will return the logger otherwise it'll return
-        None.
-
-        :param name: The name of the logger.
-        :raises TypeError: A logger name must be a string
-        :return:
-        """
-        if not isinstance(name, str):
-            raise TypeError('A logger name must be a string')
-        try:
-            if name in self.loggerDict:
-                rv = self.loggerDict[name]
-                if isinstance(rv, _logging.PlaceHolder):
-                    rv = (self.loggerClass or _loggerClass)(name)
-                    rv.manager = self
-                    self.loggerDict[name] = rv
-            else:
-                return None
-        except Exception:  # pylint: disable=broad-except
-            return None
-        return rv
-
-    def addLogger(self, name: str, logger) -> None:  # pylint: disable=invalid-name
-        """Adds a logger to the loggerDict dictionary.
-
-        :param name: str: The name of the logger.
-        :param logger: The logger to save.
-        :raises TypeError: A logger name must be a string
-        :return: None
-        """
-        if not isinstance(name, str):
-            raise TypeError('A logger name must be a string')
-        self.loggerDict[name] = logger
+# log21.Manager.py
+# CodeWriter21
+
+import logging as _logging
+from typing import Union as _Union
+
+from log21.Levels import INFO as _INFO
+from log21.Logger import Logger as _loggerClass
+
+root = _logging.RootLogger(_INFO)
+
+
+class Manager(_logging.Manager):
+    """The Manager class is a subclass of the logging.Manager class. It
+    overrides the getLogger method to make it more compatible with the
+    log21.Logger class. It also overrides the constructor."""
+
+    def __init__(self):
+        self.root = root
+        self.disable = 0
+        self.emittedNoHandlerWarning = False
+        self.loggerDict = {}
+        self.loggerClass = None
+        self.logRecordFactory = None
+
+    def getLogger(self, name: str) -> _Union[_logging.Logger, _loggerClass, None]:
+        """Takes the name of a logger and if there was a logger with that name
+        in the loggerDict it will return the logger otherwise it'll return
+        None.
+
+        :param name: The name of the logger.
+        :raises TypeError: A logger name must be a string
+        :return:
+        """
+        if not isinstance(name, str):
+            raise TypeError('A logger name must be a string')
+        try:
+            if name in self.loggerDict:
+                rv = self.loggerDict[name]
+                if isinstance(rv, _logging.PlaceHolder):
+                    rv = (self.loggerClass or _loggerClass)(name)
+                    rv.manager = self
+                    self.loggerDict[name] = rv
+            else:
+                return None
+        except Exception:  # pylint: disable=broad-except
+            return None
+        return rv
+
+    def addLogger(self, name: str, logger) -> None:  # pylint: disable=invalid-name
+        """Adds a logger to the loggerDict dictionary.
+
+        :param name: str: The name of the logger.
+        :param logger: The logger to save.
+        :raises TypeError: A logger name must be a string
+        :return: None
+        """
+        if not isinstance(name, str):
+            raise TypeError('A logger name must be a string')
+        self.loggerDict[name] = logger
```

### Comparing `log21-2.8.1b0/src/log21/PPrint.py` & `log21-2.9.0/src/log21/PPrint.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,772 +1,772 @@
-# log21.PPrint.py
-# CodeWriter21
-
-import re as _re
-import sys as _sys
-import types as _types
-import collections as _collections
-import dataclasses as _dataclasses
-from pprint import PrettyPrinter as _PrettyPrinter
-from typing import Dict as _Dict, Mapping as _Mapping, Optional as _Optional
-
-from log21.Colors import get_colors as _gc
-
-_builtin_scalars = frozenset({str, bytes, bytearray, float, complex, bool, type(None)})
-
-
-def _recursion(obj):
-    return f"<Recursion on {type(obj).__name__} with id={id(obj)}>"
-
-
-def _safe_tuple(t):
-    """Helper function for comparing 2-tuples."""
-    return _SafeKey(t[0]), _SafeKey(t[1])
-
-
-def _wrap_bytes_repr(obj, width, allowance):
-    current = b''
-    last = len(obj) // 4 * 4
-    for i in range(0, len(obj), 4):
-        part = obj[i:i + 4]
-        candidate = current + part
-        if i == last:
-            width -= allowance
-        if len(repr(candidate)) > width:
-            if current:
-                yield repr(current)
-            current = part
-        else:
-            current = candidate
-    if current:
-        yield repr(current)
-
-
-class _SafeKey:
-    """Helper function for key functions when sorting unorderable objects.
-
-    The wrapped-object will fallback to a Py2.x style comparison for unorderable types
-    (sorting first comparing the type name and then by the obj ids).  Does not work
-    recursively, so dict.items() must have _safe_key applied to both the key and the
-    value.
-    """
-
-    __slots__ = ['obj']
-
-    def __init__(self, obj):
-        self.obj = obj
-
-    def __lt__(self, other):
-        try:
-            return self.obj < other.obj
-        except TypeError:
-            return (str(type(self.obj)), id(self.obj
-                                            )) < (str(type(other.obj)), id(other.obj))
-
-
-class PrettyPrinter(_PrettyPrinter):
-
-    def __init__(
-        self,
-        indent=1,
-        width=80,
-        depth=None,
-        stream=None,
-        sign_colors: _Optional[_Mapping[str, str]] = None,
-        *,
-        compact=False,
-        sort_dicts=True,
-        underscore_numbers=False,
-        **kwargs
-    ):
-        super().__init__(
-            indent=indent,
-            width=width,
-            depth=depth,
-            stream=stream,
-            compact=compact,
-            **kwargs
-        )
-        self._depth = depth
-        self._indent_per_level = indent
-        self._width = width
-        if stream is not None:
-            self._stream = stream
-        else:
-            self._stream = _sys.stdout
-        self._compact = bool(compact)
-        self._sort_dicts = sort_dicts
-        self._underscore_numbers = underscore_numbers
-
-        self.sign_colors: _Dict[str, str] = {
-            'square-brackets': _gc('LightCyan'),
-            'curly-braces': _gc('LightBlue'),
-            'parenthesis': _gc('LightGreen'),
-            'comma': _gc('LightRed'),
-            'colon': _gc('LightRed'),
-            '...': _gc('LightMagenta'),
-            'data': _gc('Green')
-        }
-        if sign_colors:
-            for sign, color in sign_colors.items():
-                self.sign_colors[sign.lower()] = _gc(color)
-
-    def _format(self, obj, stream, indent, allowance, context, level):
-        objid = id(obj)
-        if objid in context:
-            stream.write(_recursion(obj))
-            self._recursive = True
-            self._readable = False
-            return
-        rep = self._repr(obj, context, level)
-        max_width = self._width - indent - allowance
-        if len(rep) > max_width:
-            p = self._dispatch.get(type(obj).__repr__, None)
-            if p is not None:
-                context[objid] = 1
-                p(self, obj, stream, indent, allowance, context, level + 1)
-                del context[objid]
-                return
-            elif (_dataclasses.is_dataclass(obj) and not isinstance(obj, type)
-                  and obj.__dataclass_params__.repr
-                  and  # Check dataclass has generated repr method.
-                  hasattr(obj.__repr__, "__wrapped__") and "__create_fn__"
-                  in obj.__repr__.__wrapped__.__qualname__):
-                context[objid] = 1
-                self._pprint_dataclass(
-                    obj, stream, indent, allowance, context, level + 1
-                )
-                del context[objid]
-                return
-        stream.write(rep)
-
-    def _pprint_dataclass(self, obj, stream, indent, allowance, context, level):
-        cls_name = obj.__class__.__name__
-        indent += len(cls_name) + 1
-        items = [
-            (f.name, getattr(obj, f.name)) for f in _dataclasses.fields(obj) if f.repr
-        ]
-        stream.write(cls_name + '(')
-        self._format_namespace_items(items, stream, indent, allowance, context, level)
-        stream.write(')')
-
-    def _repr(self, obj, context, level):
-        repr, readable, recursive = self.format(obj, context.copy(), self._depth, level)
-        if not readable:
-            self._readable = False
-        if recursive:
-            self._recursive = True
-        return repr
-
-    def _safe_repr(self, object_, context, max_levels, level):
-        # Return triple (repr_string, isreadable, isrecursive).
-        type_ = type(object_)
-        if type_ in _builtin_scalars:
-            return repr(object_), True, False
-
-        representation = getattr(type_, "__repr__", None)
-
-        if issubclass(type_, int) and representation is int.__repr__:
-            if self._underscore_numbers:
-                return f"{object_:_d}", True, False
-            else:
-                return repr(object_), True, False
-
-        if issubclass(type_, dict) and representation is dict.__repr__:
-            if not object_:
-                return self.sign_colors.get(
-                    'curly-braces', ''
-                ) + "{}" + self.sign_colors.get('data', ''), True, False
-            object_id = id(object_)
-            if max_levels and level >= max_levels:
-                return (
-                    self.sign_colors.get('curly-braces', '') + "{" +
-                    self.sign_colors.get('...', '') + "..." +
-                    self.sign_colors.get('curly-braces', '') + "}" +
-                    self.sign_colors.get('data', ''), False, object_id in context
-                )
-            if object_id in context:
-                return _recursion(object_), False, True
-            context[object_id] = 1
-            readable = True
-            recursive = False
-            components = []
-            append = components.append
-            level += 1
-            if self._sort_dicts:
-                items = sorted(object_.items(), key=_safe_tuple)
-            else:
-                items = object_.items()
-            for k, v in items:
-                krepr, kreadable, krecur = self.format(k, context, max_levels, level)
-                vrepr, vreadable, vrecur = self.format(v, context, max_levels, level)
-                append(
-                    f"{krepr}{self.sign_colors.get('colon')}:"
-                    f"{self.sign_colors.get('data')} {vrepr}"
-                )
-                readable = readable and kreadable and vreadable
-                if krecur or vrecur:
-                    recursive = True
-            del context[object_id]
-            return (
-                self.sign_colors.get('curly-braces', '') + "{" +
-                self.sign_colors.get('data', '') + (
-                    self.sign_colors.get('comma', '') + ", " +
-                    self.sign_colors.get('data', '')
-                ).join(components) + self.sign_colors.get('curly-braces', '') + "}",
-                readable, recursive
-            )
-
-        if (issubclass(type_, list) and representation is list.__repr__) or \
-                (issubclass(type_, tuple) and representation is tuple.__repr__):
-            if issubclass(type_, list):
-                if not object_:
-                    return self.sign_colors.get(
-                        'square-brackets', ''
-                    ) + "[]" + self.sign_colors.get('data', ''), True, False
-                format_ = (
-                    self.sign_colors.get('square-brackets', '') + "[" +
-                    self.sign_colors.get('data', '') + "%s" +
-                    self.sign_colors.get('square-brackets', '') + "]" +
-                    self.sign_colors.get('data', '')
-                )
-            elif len(object_) == 1:
-                format_ = (
-                    self.sign_colors.get('parenthesis', '') + "(" +
-                    self.sign_colors.get('data', '') + "%s" +
-                    self.sign_colors.get('comma', '') + "," +
-                    self.sign_colors.get('parenthesis', '') + ")" +
-                    self.sign_colors.get('data', '')
-                )
-            else:
-                if not object_:
-                    return self.sign_colors.get(
-                        'parenthesis', ''
-                    ) + "()" + self.sign_colors.get('data', ''), True, False
-                format_ = (
-                    self.sign_colors.get('parenthesis', '') + "(" +
-                    self.sign_colors.get('data', '') + "%s" +
-                    self.sign_colors.get('parenthesis', '') + ")" +
-                    self.sign_colors.get('data', '')
-                )
-            object_id = id(object_)
-            if max_levels and level >= max_levels:
-                return format_ % self.sign_colors.get(
-                    '...'
-                ) + "...", False, object_id in context
-            if object_id in context:
-                return _recursion(object_), False, True
-            context[object_id] = 1
-            readable = True
-            recursive = False
-            components = []
-            append = components.append
-            level += 1
-            for o in object_:
-                orepr, oreadable, orecur = self.format(o, context, max_levels, level)
-                append(orepr)
-                if not oreadable:
-                    readable = False
-                if orecur:
-                    recursive = True
-            del context[object_id]
-            return (
-                format_ % (
-                    self.sign_colors.get('comma', '') + ", " +
-                    self.sign_colors.get('data', '')
-                ).join(components), readable, recursive
-            )
-
-        rep = repr(object_)
-        return rep, (rep and not rep.startswith('<')), False
-
-    _dispatch = {}
-
-    def _pprint_dict(self, obj, stream, indent, allowance, context, level):
-        write = stream.write
-        write(
-            self.sign_colors.get('curly-braces', '') + '{' +
-            self.sign_colors.get('data', '')
-        )
-        if self._indent_per_level > 1:
-            write((self._indent_per_level - 1) * ' ')
-        length = len(obj)
-        if length:
-            if self._sort_dicts:
-                items = sorted(obj.items(), key=_safe_tuple)
-            else:
-                items = obj.items()
-            self._format_dict_items(
-                items, stream, indent, allowance + 1, context, level
-            )
-        write(
-            self.sign_colors.get('curly-braces', '') + '}' +
-            self.sign_colors.get('data', '')
-        )
-
-    _dispatch[dict.__repr__] = _pprint_dict
-
-    def _pprint_ordered_dict(self, obj, stream, indent, allowance, context, level):
-        if not len(obj):
-            stream.write(repr(obj))
-            return
-        cls = obj.__class__
-        stream.write(
-            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
-            self.sign_colors.get('data')
-        )
-        self._format(
-            list(obj.items()), stream, indent + len(cls.__name__) + 1, allowance + 1,
-            context, level
-        )
-        stream.write(
-            self.sign_colors.get('parenthesis', '') + ')' +
-            self.sign_colors.get('data', '')
-        )
-
-    _dispatch[_collections.OrderedDict.__repr__] = _pprint_ordered_dict
-
-    def _pprint_list(self, obj, stream, indent, allowance, context, level):
-        stream.write(
-            self.sign_colors.get('square-brackets', '') + '[' +
-            self.sign_colors.get('data', '')
-        )
-        self._format_items(obj, stream, indent, allowance + 1, context, level)
-        stream.write(
-            self.sign_colors.get('square-brackets', '') + ']' +
-            self.sign_colors.get('data', '')
-        )
-
-    _dispatch[list.__repr__] = _pprint_list
-
-    def _pprint_tuple(self, obj, stream, indent, allowance, context, level):
-        stream.write(
-            self.sign_colors.get('parenthesis', '') + '(' +
-            self.sign_colors.get('data', '')
-        )
-        endchar = (
-            self.sign_colors.get('comma', '') + ',' +
-            self.sign_colors.get('parenthesis', '') + ')' +
-            self.sign_colors.get('data', '')
-            if len(obj) == 1 else self.sign_colors.get('parenthesis', '') + ')' +
-            self.sign_colors.get('data', '')
-        )
-        self._format_items(
-            obj, stream, indent, allowance + len(endchar), context, level
-        )
-        stream.write(endchar)
-
-    _dispatch[tuple.__repr__] = _pprint_tuple
-
-    def _pprint_set(self, obj, stream, indent, allowance, context, level):
-        if not len(obj):
-            stream.write(repr(obj))
-            return
-        typ = obj.__class__
-        if typ is set:
-            stream.write(
-                self.sign_colors.get('curly-braces', '') + '{' +
-                self.sign_colors.get('data', '')
-            )
-            endchar = self.sign_colors.get('curly-braces',
-                                           '') + '}' + self.sign_colors.get('data', '')
-        else:
-            stream.write(
-                typ.__name__ + self.sign_colors.get('parenthesis', '') + '(' +
-                self.sign_colors.get('curly-braces', '') + '{' +
-                self.sign_colors.get('data', '')
-            )
-            endchar = (
-                self.sign_colors.get('curly-braces', '') + '}' +
-                self.sign_colors.get('parenthesis', '') + ')' +
-                self.sign_colors.get('data', '')
-            )
-            indent += len(typ.__name__) + 1
-        obj = sorted(obj, key=_SafeKey)
-        self._format_items(
-            obj, stream, indent, allowance + len(endchar), context, level
-        )
-        stream.write(endchar)
-
-    _dispatch[set.__repr__] = _pprint_set
-    _dispatch[frozenset.__repr__] = _pprint_set
-
-    def _pprint_str(self, object_, stream, indent, allowance, context, level):
-        write = stream.write
-        if not len(object_):
-            write(repr(object_))
-            return
-        chunks = []
-        lines = object_.splitlines(True)
-        if level == 1:
-            indent += 1
-            allowance += 1
-        max_width1 = max_width = self._width - indent
-        representation = ''
-        for i, line in enumerate(lines):
-            representation = repr(line)
-            if i == len(lines) - 1:
-                max_width1 -= allowance
-            if len(representation) <= max_width1:
-                chunks.append(representation)
-            else:
-                # A list of alternating (non-space, space) strings
-                parts = _re.findall(r'\S*\s*', line)
-                assert parts
-                assert not parts[-1]
-                parts.pop()  # drop empty last part
-                max_width2 = max_width
-                current = ''
-                for j, part in enumerate(parts):
-                    candidate = current + part
-                    if j == len(parts) - 1 and i == len(lines) - 1:
-                        max_width2 -= allowance
-                    if len(repr(candidate)) > max_width2:
-                        if current:
-                            chunks.append(repr(current))
-                        current = part
-                    else:
-                        current = candidate
-                if current:
-                    chunks.append(repr(current))
-        if len(chunks) == 1:
-            write(representation)
-            return
-        if level == 1:
-            write(
-                self.sign_colors.get('parenthesis', '') + '(' +
-                self.sign_colors.get('data', '')
-            )
-        for i, representation in enumerate(chunks):
-            if i > 0:
-                write('\n' + ' ' * indent)
-            write(representation)
-        if level == 1:
-            write(
-                self.sign_colors.get('parenthesis', '') + ')' +
-                self.sign_colors.get('data', '')
-            )
-
-    _dispatch[str.__repr__] = _pprint_str
-
-    def _pprint_bytes(self, obj, stream, indent, allowance, context, level):
-        write = stream.write
-        if len(obj) <= 4:
-            write(repr(obj))
-            return
-        parens = level == 1
-        if parens:
-            indent += 1
-            allowance += 1
-            write(
-                self.sign_colors.get('parenthesis', '') + '(' +
-                self.sign_colors.get('data', '')
-            )
-        delim = ''
-        for rep in _wrap_bytes_repr(obj, self._width - indent, allowance):
-            write(delim)
-            write(rep)
-            if not delim:
-                delim = '\n' + ' ' * indent
-        if parens:
-            write(
-                self.sign_colors.get('parenthesis', '') + ')' +
-                self.sign_colors.get('data', '')
-            )
-
-    _dispatch[bytes.__repr__] = _pprint_bytes
-
-    def _pprint_bytearray(self, obj, stream, indent, allowance, context, level):
-        write = stream.write
-        write(
-            'bytearray' + self.sign_colors.get('parenthesis', '') + '(' +
-            self.sign_colors.get('data', '')
-        )
-        self._pprint_bytes(
-            bytes(obj), stream, indent + 10, allowance + 1, context, level + 1
-        )
-        write(
-            self.sign_colors.get('parenthesis', '') + ')' +
-            self.sign_colors.get('data', '')
-        )
-
-    _dispatch[bytearray.__repr__] = _pprint_bytearray
-
-    def _pprint_mappingproxy(self, obj, stream, indent, allowance, context, level):
-        stream.write(
-            'mappingproxy' + self.sign_colors.get('parenthesis', '') + '(' +
-            self.sign_colors.get('data', '')
-        )
-        self._format(obj.copy(), stream, indent + 13, allowance + 1, context, level)
-        stream.write(
-            self.sign_colors.get('parenthesis', '') + ')' +
-            self.sign_colors.get('data', '')
-        )
-
-    _dispatch[_types.MappingProxyType.__repr__] = _pprint_mappingproxy
-
-    def _pprint_simplenamespace(self, obj, stream, indent, allowance, context, level):
-        if isinstance(obj, _types.SimpleNamespace):
-            # The SimpleNamespace repr is "namespace" instead of the class
-            # name, so we do the same here. For subclasses; use the class name.
-            cls_name = 'namespace'
-        else:
-            cls_name = obj.__class__.__name__
-        indent += len(cls_name) + 1
-        items = obj.__dict__.items()
-        stream.write(
-            cls_name + self.sign_colors.get('parenthesis', '') + '(' +
-            self.sign_colors.get('data', '')
-        )
-        self._format_namespace_items(items, stream, indent, allowance, context, level)
-        stream.write(
-            self.sign_colors.get('parenthesis', '') + ')' +
-            self.sign_colors.get('data', '')
-        )
-
-    _dispatch[_types.SimpleNamespace.__repr__] = _pprint_simplenamespace
-
-    def _format_dict_items(self, items, stream, indent, allowance, context, level):
-        write = stream.write
-        indent += self._indent_per_level
-        delimnl = self.sign_colors.get('comma', '') + ',\n' + self.sign_colors.get(
-            'data', ''
-        ) + ' ' * indent
-        last_index = len(items) - 1
-        for i, (key, ent) in enumerate(items):
-            last = i == last_index
-            rep = self._repr(key, context, level)
-            write(rep)
-            write(
-                self.sign_colors.get('colon', '') + ': ' +
-                self.sign_colors.get('data', '')
-            )
-            self._format(
-                ent, stream, indent + len(rep) + 2, allowance if last else 1, context,
-                level
-            )
-            if not last:
-                write(delimnl)
-
-    def _format_namespace_items(self, items, stream, indent, allowance, context, level):
-        write = stream.write
-        delimnl = self.sign_colors.get('comma', '') + ',\n' + self.sign_colors.get(
-            'data', ''
-        ) + ' ' * indent
-        last_index = len(items) - 1
-        for i, (key, ent) in enumerate(items):
-            last = i == last_index
-            write(key)
-            write('=')
-            if id(ent) in context:
-                # Special-case representation of recursion to match standard
-                # recursive dataclass repr.
-                write(
-                    self.sign_colors.get('...', '') + "..." +
-                    self.sign_colors.get('data', '')
-                )
-            else:
-                self._format(
-                    ent, stream, indent + len(key) + 1, allowance if last else 1,
-                    context, level
-                )
-            if not last:
-                write(delimnl)
-
-    def _format_items(self, items, stream, indent, allowance, context, level):
-        write = stream.write
-        indent += self._indent_per_level
-        if self._indent_per_level > 1:
-            write((self._indent_per_level - 1) * ' ')
-        delimnl = self.sign_colors.get('comma', '') + ',\n' + self.sign_colors.get(
-            'data', ''
-        ) + ' ' * indent
-        delim = ''
-        width = max_width = self._width - indent + 1
-        it = iter(items)
-        try:
-            next_ent = next(it)
-        except StopIteration:
-            return
-        last = False
-        while not last:
-            ent = next_ent
-            try:
-                next_ent = next(it)
-            except StopIteration:
-                last = True
-                max_width -= allowance
-                width -= allowance
-            if self._compact:
-                rep = self._repr(ent, context, level)
-                w = len(rep) + 2
-                if width < w:
-                    width = max_width
-                    if delim:
-                        delim = delimnl
-                if width >= w:
-                    width -= w
-                    write(delim)
-                    delim = self.sign_colors.get(
-                        'comma', ''
-                    ) + ', ' + self.sign_colors.get('data', '')
-                    write(rep)
-                    continue
-            write(delim)
-            delim = delimnl
-            self._format(ent, stream, indent, allowance if last else 1, context, level)
-
-    def _pprint_default_dict(self, obj, stream, indent, allowance, context, level):
-        if not len(obj):
-            stream.write(repr(obj))
-            return
-        rdf = self._repr(obj.default_factory, context, level)
-        cls = obj.__class__
-        indent += len(cls.__name__) + 1
-        stream.write(
-            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
-            self.sign_colors.get('data') + rdf + self.sign_colors.get('comma') + ',\n' +
-            self.sign_colors.get('data') + (' ' * indent)
-        )
-        self._pprint_dict(obj, stream, indent, allowance + 1, context, level)
-        stream.write(
-            self.sign_colors.get('parenthesis', '') + ')' +
-            self.sign_colors.get('data', '')
-        )
-
-    _dispatch[_collections.defaultdict.__repr__] = _pprint_default_dict
-
-    def _pprint_counter(self, obj, stream, indent, allowance, context, level):
-        if not len(obj):
-            stream.write(repr(obj))
-            return
-        cls = obj.__class__
-        stream.write(
-            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
-            self.sign_colors.get('curly-braces') + '{' + self.sign_colors.get('data')
-        )
-        if self._indent_per_level > 1:
-            stream.write((self._indent_per_level - 1) * ' ')
-        items = obj.most_common()
-        self._format_dict_items(
-            items, stream, indent + len(cls.__name__) + 1, allowance + 2, context, level
-        )
-        stream.write(
-            self.sign_colors.get('curly-braces', '') + '}' +
-            self.sign_colors.get('parenthesis', '') + ')' +
-            self.sign_colors.get('data', '')
-        )
-
-    _dispatch[_collections.Counter.__repr__] = _pprint_counter
-
-    def _pprint_chain_map(self, obj, stream, indent, allowance, context, level):
-        if not len(obj.maps):
-            stream.write(repr(obj))
-            return
-        cls = obj.__class__
-        stream.write(
-            cls.__name__ + self.sign_colors.get('parenthesis', '') + '(' +
-            self.sign_colors.get('data', '')
-        )
-        indent += len(cls.__name__) + 1
-        for i, m in enumerate(obj.maps):
-            if i == len(obj.maps) - 1:
-                self._format(m, stream, indent, allowance + 1, context, level)
-                stream.write(
-                    self.sign_colors.get('parenthesis', '') + ')' +
-                    self.sign_colors.get('data', '')
-                )
-            else:
-                self._format(m, stream, indent, 1, context, level)
-                stream.write(
-                    self.sign_colors.get('comma', '') + ',\n' +
-                    self.sign_colors.get('data', '') + ' ' * indent
-                )
-
-    _dispatch[_collections.ChainMap.__repr__] = _pprint_chain_map
-
-    def _pprint_deque(self, obj, stream, indent, allowance, context, level):
-        if not len(obj):
-            stream.write(repr(obj))
-            return
-        cls = obj.__class__
-        stream.write(
-            cls.__name__ + self.sign_colors.get('parenthesis', '') + '(' +
-            self.sign_colors.get('data', '')
-        )
-        indent += len(cls.__name__) + 1
-        stream.write(
-            self.sign_colors.get('square-brackets', '') + '[' +
-            self.sign_colors.get('data', '')
-        )
-        if obj.maxlen is None:
-            self._format_items(obj, stream, indent, allowance + 2, context, level)
-            stream.write(
-                self.sign_colors.get('square-brackets', '') + ']' +
-                self.sign_colors.get('parenthesis', '') + ')' +
-                self.sign_colors.get('data', '')
-            )
-        else:
-            self._format_items(obj, stream, indent, 2, context, level)
-            rml = self._repr(obj.maxlen, context, level)
-            stream.write(
-                self.sign_colors.get('square-brackets', '') + ']' +
-                self.sign_colors.get('comma', '') + ',' +
-                self.sign_colors.get('data', '') + '\n' + (' ' * indent) + 'maxlen=' +
-                rml + self.sign_colors.get('parenthesis', '') + ')'
-            )
-
-    _dispatch[_collections.deque.__repr__] = _pprint_deque
-
-    def _pprint_user_dict(self, obj, stream, indent, allowance, context, level):
-        self._format(obj.data, stream, indent, allowance, context, level - 1)
-
-    _dispatch[_collections.UserDict.__repr__] = _pprint_user_dict
-
-    def _pprint_user_list(self, obj, stream, indent, allowance, context, level):
-        self._format(obj.data, stream, indent, allowance, context, level - 1)
-
-    _dispatch[_collections.UserList.__repr__] = _pprint_user_list
-
-    def _pprint_user_string(self, obj, stream, indent, allowance, context, level):
-        self._format(obj.data, stream, indent, allowance, context, level - 1)
-
-    _dispatch[_collections.UserString.__repr__] = _pprint_user_string
-
-
-def pformat(
-    obj,
-    indent=1,
-    width=80,
-    depth=None,
-    signs_colors: _Optional[_Mapping[str, str]] = None,
-    *,
-    compact=False,
-    sort_dicts=True,
-    underscore_numbers=False,
-    **kwargs
-):
-    """Format a Python object into a pretty-printed representation.
-
-    :param obj: the object to format.
-    :param indent: the number of spaces to indent for each level of nesting.
-    :param width: the maximum width of the formatted representation.
-    :param depth: the maximum depth to print out nested structures.
-    :param signs_colors: a mapping of signs and colors.
-    :param compact: if `True`, several items will be combined in one line.
-    :param sort_dicts: if `True`, dictionaries will be sorted by key. (py38+)
-    :param underscore_numbers: if `True`, numbers will be represented with an
-        underscore between every digit. (py310+)
-    :param kwargs: additional keyword arguments to pass to the underlying pretty
-        printer.
-    :return: the formatted representation.
-    """
-    return PrettyPrinter(
-        indent=indent,
-        width=width,
-        depth=depth,
-        compact=compact,
-        sign_colors=signs_colors,
-        sort_dicts=sort_dicts,
-        underscore_numbers=underscore_numbers,
-        **kwargs
-    ).pformat(obj)
+# log21.PPrint.py
+# CodeWriter21
+
+import re as _re
+import sys as _sys
+import types as _types
+import collections as _collections
+import dataclasses as _dataclasses
+from pprint import PrettyPrinter as _PrettyPrinter
+from typing import Dict as _Dict, Mapping as _Mapping, Optional as _Optional
+
+from log21.Colors import get_colors as _gc
+
+_builtin_scalars = frozenset({str, bytes, bytearray, float, complex, bool, type(None)})
+
+
+def _recursion(obj):
+    return f"<Recursion on {type(obj).__name__} with id={id(obj)}>"
+
+
+def _safe_tuple(t):
+    """Helper function for comparing 2-tuples."""
+    return _SafeKey(t[0]), _SafeKey(t[1])
+
+
+def _wrap_bytes_repr(obj, width, allowance):
+    current = b''
+    last = len(obj) // 4 * 4
+    for i in range(0, len(obj), 4):
+        part = obj[i:i + 4]
+        candidate = current + part
+        if i == last:
+            width -= allowance
+        if len(repr(candidate)) > width:
+            if current:
+                yield repr(current)
+            current = part
+        else:
+            current = candidate
+    if current:
+        yield repr(current)
+
+
+class _SafeKey:
+    """Helper function for key functions when sorting unorderable objects.
+
+    The wrapped-object will fallback to a Py2.x style comparison for unorderable types
+    (sorting first comparing the type name and then by the obj ids).  Does not work
+    recursively, so dict.items() must have _safe_key applied to both the key and the
+    value.
+    """
+
+    __slots__ = ['obj']
+
+    def __init__(self, obj):
+        self.obj = obj
+
+    def __lt__(self, other):
+        try:
+            return self.obj < other.obj
+        except TypeError:
+            return (str(type(self.obj)), id(self.obj
+                                            )) < (str(type(other.obj)), id(other.obj))
+
+
+class PrettyPrinter(_PrettyPrinter):
+
+    def __init__(
+        self,
+        indent=1,
+        width=80,
+        depth=None,
+        stream=None,
+        sign_colors: _Optional[_Mapping[str, str]] = None,
+        *,
+        compact=False,
+        sort_dicts=True,
+        underscore_numbers=False,
+        **kwargs
+    ):
+        super().__init__(
+            indent=indent,
+            width=width,
+            depth=depth,
+            stream=stream,
+            compact=compact,
+            **kwargs
+        )
+        self._depth = depth
+        self._indent_per_level = indent
+        self._width = width
+        if stream is not None:
+            self._stream = stream
+        else:
+            self._stream = _sys.stdout
+        self._compact = bool(compact)
+        self._sort_dicts = sort_dicts
+        self._underscore_numbers = underscore_numbers
+
+        self.sign_colors: _Dict[str, str] = {
+            'square-brackets': _gc('LightCyan'),
+            'curly-braces': _gc('LightBlue'),
+            'parenthesis': _gc('LightGreen'),
+            'comma': _gc('LightRed'),
+            'colon': _gc('LightRed'),
+            '...': _gc('LightMagenta'),
+            'data': _gc('Green')
+        }
+        if sign_colors:
+            for sign, color in sign_colors.items():
+                self.sign_colors[sign.lower()] = _gc(color)
+
+    def _format(self, obj, stream, indent, allowance, context, level):
+        objid = id(obj)
+        if objid in context:
+            stream.write(_recursion(obj))
+            self._recursive = True
+            self._readable = False
+            return
+        rep = self._repr(obj, context, level)
+        max_width = self._width - indent - allowance
+        if len(rep) > max_width:
+            p = self._dispatch.get(type(obj).__repr__, None)
+            if p is not None:
+                context[objid] = 1
+                p(self, obj, stream, indent, allowance, context, level + 1)
+                del context[objid]
+                return
+            elif (_dataclasses.is_dataclass(obj) and not isinstance(obj, type)
+                  and obj.__dataclass_params__.repr
+                  and  # Check dataclass has generated repr method.
+                  hasattr(obj.__repr__, "__wrapped__") and "__create_fn__"
+                  in obj.__repr__.__wrapped__.__qualname__):
+                context[objid] = 1
+                self._pprint_dataclass(
+                    obj, stream, indent, allowance, context, level + 1
+                )
+                del context[objid]
+                return
+        stream.write(rep)
+
+    def _pprint_dataclass(self, obj, stream, indent, allowance, context, level):
+        cls_name = obj.__class__.__name__
+        indent += len(cls_name) + 1
+        items = [
+            (f.name, getattr(obj, f.name)) for f in _dataclasses.fields(obj) if f.repr
+        ]
+        stream.write(cls_name + '(')
+        self._format_namespace_items(items, stream, indent, allowance, context, level)
+        stream.write(')')
+
+    def _repr(self, obj, context, level):
+        repr, readable, recursive = self.format(obj, context.copy(), self._depth, level)
+        if not readable:
+            self._readable = False
+        if recursive:
+            self._recursive = True
+        return repr
+
+    def _safe_repr(self, object_, context, max_levels, level):
+        # Return triple (repr_string, isreadable, isrecursive).
+        type_ = type(object_)
+        if type_ in _builtin_scalars:
+            return repr(object_), True, False
+
+        representation = getattr(type_, "__repr__", None)
+
+        if issubclass(type_, int) and representation is int.__repr__:
+            if self._underscore_numbers:
+                return f"{object_:_d}", True, False
+            else:
+                return repr(object_), True, False
+
+        if issubclass(type_, dict) and representation is dict.__repr__:
+            if not object_:
+                return self.sign_colors.get(
+                    'curly-braces', ''
+                ) + "{}" + self.sign_colors.get('data', ''), True, False
+            object_id = id(object_)
+            if max_levels and level >= max_levels:
+                return (
+                    self.sign_colors.get('curly-braces', '') + "{" +
+                    self.sign_colors.get('...', '') + "..." +
+                    self.sign_colors.get('curly-braces', '') + "}" +
+                    self.sign_colors.get('data', ''), False, object_id in context
+                )
+            if object_id in context:
+                return _recursion(object_), False, True
+            context[object_id] = 1
+            readable = True
+            recursive = False
+            components = []
+            append = components.append
+            level += 1
+            if self._sort_dicts:
+                items = sorted(object_.items(), key=_safe_tuple)
+            else:
+                items = object_.items()
+            for k, v in items:
+                krepr, kreadable, krecur = self.format(k, context, max_levels, level)
+                vrepr, vreadable, vrecur = self.format(v, context, max_levels, level)
+                append(
+                    f"{krepr}{self.sign_colors.get('colon')}:"
+                    f"{self.sign_colors.get('data')} {vrepr}"
+                )
+                readable = readable and kreadable and vreadable
+                if krecur or vrecur:
+                    recursive = True
+            del context[object_id]
+            return (
+                self.sign_colors.get('curly-braces', '') + "{" +
+                self.sign_colors.get('data', '') + (
+                    self.sign_colors.get('comma', '') + ", " +
+                    self.sign_colors.get('data', '')
+                ).join(components) + self.sign_colors.get('curly-braces', '') + "}",
+                readable, recursive
+            )
+
+        if (issubclass(type_, list) and representation is list.__repr__) or \
+                (issubclass(type_, tuple) and representation is tuple.__repr__):
+            if issubclass(type_, list):
+                if not object_:
+                    return self.sign_colors.get(
+                        'square-brackets', ''
+                    ) + "[]" + self.sign_colors.get('data', ''), True, False
+                format_ = (
+                    self.sign_colors.get('square-brackets', '') + "[" +
+                    self.sign_colors.get('data', '') + "%s" +
+                    self.sign_colors.get('square-brackets', '') + "]" +
+                    self.sign_colors.get('data', '')
+                )
+            elif len(object_) == 1:
+                format_ = (
+                    self.sign_colors.get('parenthesis', '') + "(" +
+                    self.sign_colors.get('data', '') + "%s" +
+                    self.sign_colors.get('comma', '') + "," +
+                    self.sign_colors.get('parenthesis', '') + ")" +
+                    self.sign_colors.get('data', '')
+                )
+            else:
+                if not object_:
+                    return self.sign_colors.get(
+                        'parenthesis', ''
+                    ) + "()" + self.sign_colors.get('data', ''), True, False
+                format_ = (
+                    self.sign_colors.get('parenthesis', '') + "(" +
+                    self.sign_colors.get('data', '') + "%s" +
+                    self.sign_colors.get('parenthesis', '') + ")" +
+                    self.sign_colors.get('data', '')
+                )
+            object_id = id(object_)
+            if max_levels and level >= max_levels:
+                return format_ % self.sign_colors.get(
+                    '...'
+                ) + "...", False, object_id in context
+            if object_id in context:
+                return _recursion(object_), False, True
+            context[object_id] = 1
+            readable = True
+            recursive = False
+            components = []
+            append = components.append
+            level += 1
+            for o in object_:
+                orepr, oreadable, orecur = self.format(o, context, max_levels, level)
+                append(orepr)
+                if not oreadable:
+                    readable = False
+                if orecur:
+                    recursive = True
+            del context[object_id]
+            return (
+                format_ % (
+                    self.sign_colors.get('comma', '') + ", " +
+                    self.sign_colors.get('data', '')
+                ).join(components), readable, recursive
+            )
+
+        rep = repr(object_)
+        return rep, (rep and not rep.startswith('<')), False
+
+    _dispatch = {}
+
+    def _pprint_dict(self, obj, stream, indent, allowance, context, level):
+        write = stream.write
+        write(
+            self.sign_colors.get('curly-braces', '') + '{' +
+            self.sign_colors.get('data', '')
+        )
+        if self._indent_per_level > 1:
+            write((self._indent_per_level - 1) * ' ')
+        length = len(obj)
+        if length:
+            if self._sort_dicts:
+                items = sorted(obj.items(), key=_safe_tuple)
+            else:
+                items = obj.items()
+            self._format_dict_items(
+                items, stream, indent, allowance + 1, context, level
+            )
+        write(
+            self.sign_colors.get('curly-braces', '') + '}' +
+            self.sign_colors.get('data', '')
+        )
+
+    _dispatch[dict.__repr__] = _pprint_dict
+
+    def _pprint_ordered_dict(self, obj, stream, indent, allowance, context, level):
+        if not len(obj):
+            stream.write(repr(obj))
+            return
+        cls = obj.__class__
+        stream.write(
+            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('data')
+        )
+        self._format(
+            list(obj.items()), stream, indent + len(cls.__name__) + 1, allowance + 1,
+            context, level
+        )
+        stream.write(
+            self.sign_colors.get('parenthesis', '') + ')' +
+            self.sign_colors.get('data', '')
+        )
+
+    _dispatch[_collections.OrderedDict.__repr__] = _pprint_ordered_dict
+
+    def _pprint_list(self, obj, stream, indent, allowance, context, level):
+        stream.write(
+            self.sign_colors.get('square-brackets', '') + '[' +
+            self.sign_colors.get('data', '')
+        )
+        self._format_items(obj, stream, indent, allowance + 1, context, level)
+        stream.write(
+            self.sign_colors.get('square-brackets', '') + ']' +
+            self.sign_colors.get('data', '')
+        )
+
+    _dispatch[list.__repr__] = _pprint_list
+
+    def _pprint_tuple(self, obj, stream, indent, allowance, context, level):
+        stream.write(
+            self.sign_colors.get('parenthesis', '') + '(' +
+            self.sign_colors.get('data', '')
+        )
+        endchar = (
+            self.sign_colors.get('comma', '') + ',' +
+            self.sign_colors.get('parenthesis', '') + ')' +
+            self.sign_colors.get('data', '')
+            if len(obj) == 1 else self.sign_colors.get('parenthesis', '') + ')' +
+            self.sign_colors.get('data', '')
+        )
+        self._format_items(
+            obj, stream, indent, allowance + len(endchar), context, level
+        )
+        stream.write(endchar)
+
+    _dispatch[tuple.__repr__] = _pprint_tuple
+
+    def _pprint_set(self, obj, stream, indent, allowance, context, level):
+        if not len(obj):
+            stream.write(repr(obj))
+            return
+        typ = obj.__class__
+        if typ is set:
+            stream.write(
+                self.sign_colors.get('curly-braces', '') + '{' +
+                self.sign_colors.get('data', '')
+            )
+            endchar = self.sign_colors.get('curly-braces',
+                                           '') + '}' + self.sign_colors.get('data', '')
+        else:
+            stream.write(
+                typ.__name__ + self.sign_colors.get('parenthesis', '') + '(' +
+                self.sign_colors.get('curly-braces', '') + '{' +
+                self.sign_colors.get('data', '')
+            )
+            endchar = (
+                self.sign_colors.get('curly-braces', '') + '}' +
+                self.sign_colors.get('parenthesis', '') + ')' +
+                self.sign_colors.get('data', '')
+            )
+            indent += len(typ.__name__) + 1
+        obj = sorted(obj, key=_SafeKey)
+        self._format_items(
+            obj, stream, indent, allowance + len(endchar), context, level
+        )
+        stream.write(endchar)
+
+    _dispatch[set.__repr__] = _pprint_set
+    _dispatch[frozenset.__repr__] = _pprint_set
+
+    def _pprint_str(self, object_, stream, indent, allowance, context, level):
+        write = stream.write
+        if not len(object_):
+            write(repr(object_))
+            return
+        chunks = []
+        lines = object_.splitlines(True)
+        if level == 1:
+            indent += 1
+            allowance += 1
+        max_width1 = max_width = self._width - indent
+        representation = ''
+        for i, line in enumerate(lines):
+            representation = repr(line)
+            if i == len(lines) - 1:
+                max_width1 -= allowance
+            if len(representation) <= max_width1:
+                chunks.append(representation)
+            else:
+                # A list of alternating (non-space, space) strings
+                parts = _re.findall(r'\S*\s*', line)
+                assert parts
+                assert not parts[-1]
+                parts.pop()  # drop empty last part
+                max_width2 = max_width
+                current = ''
+                for j, part in enumerate(parts):
+                    candidate = current + part
+                    if j == len(parts) - 1 and i == len(lines) - 1:
+                        max_width2 -= allowance
+                    if len(repr(candidate)) > max_width2:
+                        if current:
+                            chunks.append(repr(current))
+                        current = part
+                    else:
+                        current = candidate
+                if current:
+                    chunks.append(repr(current))
+        if len(chunks) == 1:
+            write(representation)
+            return
+        if level == 1:
+            write(
+                self.sign_colors.get('parenthesis', '') + '(' +
+                self.sign_colors.get('data', '')
+            )
+        for i, representation in enumerate(chunks):
+            if i > 0:
+                write('\n' + ' ' * indent)
+            write(representation)
+        if level == 1:
+            write(
+                self.sign_colors.get('parenthesis', '') + ')' +
+                self.sign_colors.get('data', '')
+            )
+
+    _dispatch[str.__repr__] = _pprint_str
+
+    def _pprint_bytes(self, obj, stream, indent, allowance, context, level):
+        write = stream.write
+        if len(obj) <= 4:
+            write(repr(obj))
+            return
+        parens = level == 1
+        if parens:
+            indent += 1
+            allowance += 1
+            write(
+                self.sign_colors.get('parenthesis', '') + '(' +
+                self.sign_colors.get('data', '')
+            )
+        delim = ''
+        for rep in _wrap_bytes_repr(obj, self._width - indent, allowance):
+            write(delim)
+            write(rep)
+            if not delim:
+                delim = '\n' + ' ' * indent
+        if parens:
+            write(
+                self.sign_colors.get('parenthesis', '') + ')' +
+                self.sign_colors.get('data', '')
+            )
+
+    _dispatch[bytes.__repr__] = _pprint_bytes
+
+    def _pprint_bytearray(self, obj, stream, indent, allowance, context, level):
+        write = stream.write
+        write(
+            'bytearray' + self.sign_colors.get('parenthesis', '') + '(' +
+            self.sign_colors.get('data', '')
+        )
+        self._pprint_bytes(
+            bytes(obj), stream, indent + 10, allowance + 1, context, level + 1
+        )
+        write(
+            self.sign_colors.get('parenthesis', '') + ')' +
+            self.sign_colors.get('data', '')
+        )
+
+    _dispatch[bytearray.__repr__] = _pprint_bytearray
+
+    def _pprint_mappingproxy(self, obj, stream, indent, allowance, context, level):
+        stream.write(
+            'mappingproxy' + self.sign_colors.get('parenthesis', '') + '(' +
+            self.sign_colors.get('data', '')
+        )
+        self._format(obj.copy(), stream, indent + 13, allowance + 1, context, level)
+        stream.write(
+            self.sign_colors.get('parenthesis', '') + ')' +
+            self.sign_colors.get('data', '')
+        )
+
+    _dispatch[_types.MappingProxyType.__repr__] = _pprint_mappingproxy
+
+    def _pprint_simplenamespace(self, obj, stream, indent, allowance, context, level):
+        if isinstance(obj, _types.SimpleNamespace):
+            # The SimpleNamespace repr is "namespace" instead of the class
+            # name, so we do the same here. For subclasses; use the class name.
+            cls_name = 'namespace'
+        else:
+            cls_name = obj.__class__.__name__
+        indent += len(cls_name) + 1
+        items = obj.__dict__.items()
+        stream.write(
+            cls_name + self.sign_colors.get('parenthesis', '') + '(' +
+            self.sign_colors.get('data', '')
+        )
+        self._format_namespace_items(items, stream, indent, allowance, context, level)
+        stream.write(
+            self.sign_colors.get('parenthesis', '') + ')' +
+            self.sign_colors.get('data', '')
+        )
+
+    _dispatch[_types.SimpleNamespace.__repr__] = _pprint_simplenamespace
+
+    def _format_dict_items(self, items, stream, indent, allowance, context, level):
+        write = stream.write
+        indent += self._indent_per_level
+        delimnl = self.sign_colors.get('comma', '') + ',\n' + self.sign_colors.get(
+            'data', ''
+        ) + ' ' * indent
+        last_index = len(items) - 1
+        for i, (key, ent) in enumerate(items):
+            last = i == last_index
+            rep = self._repr(key, context, level)
+            write(rep)
+            write(
+                self.sign_colors.get('colon', '') + ': ' +
+                self.sign_colors.get('data', '')
+            )
+            self._format(
+                ent, stream, indent + len(rep) + 2, allowance if last else 1, context,
+                level
+            )
+            if not last:
+                write(delimnl)
+
+    def _format_namespace_items(self, items, stream, indent, allowance, context, level):
+        write = stream.write
+        delimnl = self.sign_colors.get('comma', '') + ',\n' + self.sign_colors.get(
+            'data', ''
+        ) + ' ' * indent
+        last_index = len(items) - 1
+        for i, (key, ent) in enumerate(items):
+            last = i == last_index
+            write(key)
+            write('=')
+            if id(ent) in context:
+                # Special-case representation of recursion to match standard
+                # recursive dataclass repr.
+                write(
+                    self.sign_colors.get('...', '') + "..." +
+                    self.sign_colors.get('data', '')
+                )
+            else:
+                self._format(
+                    ent, stream, indent + len(key) + 1, allowance if last else 1,
+                    context, level
+                )
+            if not last:
+                write(delimnl)
+
+    def _format_items(self, items, stream, indent, allowance, context, level):
+        write = stream.write
+        indent += self._indent_per_level
+        if self._indent_per_level > 1:
+            write((self._indent_per_level - 1) * ' ')
+        delimnl = self.sign_colors.get('comma', '') + ',\n' + self.sign_colors.get(
+            'data', ''
+        ) + ' ' * indent
+        delim = ''
+        width = max_width = self._width - indent + 1
+        it = iter(items)
+        try:
+            next_ent = next(it)
+        except StopIteration:
+            return
+        last = False
+        while not last:
+            ent = next_ent
+            try:
+                next_ent = next(it)
+            except StopIteration:
+                last = True
+                max_width -= allowance
+                width -= allowance
+            if self._compact:
+                rep = self._repr(ent, context, level)
+                w = len(rep) + 2
+                if width < w:
+                    width = max_width
+                    if delim:
+                        delim = delimnl
+                if width >= w:
+                    width -= w
+                    write(delim)
+                    delim = self.sign_colors.get(
+                        'comma', ''
+                    ) + ', ' + self.sign_colors.get('data', '')
+                    write(rep)
+                    continue
+            write(delim)
+            delim = delimnl
+            self._format(ent, stream, indent, allowance if last else 1, context, level)
+
+    def _pprint_default_dict(self, obj, stream, indent, allowance, context, level):
+        if not len(obj):
+            stream.write(repr(obj))
+            return
+        rdf = self._repr(obj.default_factory, context, level)
+        cls = obj.__class__
+        indent += len(cls.__name__) + 1
+        stream.write(
+            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('data') + rdf + self.sign_colors.get('comma') + ',\n' +
+            self.sign_colors.get('data') + (' ' * indent)
+        )
+        self._pprint_dict(obj, stream, indent, allowance + 1, context, level)
+        stream.write(
+            self.sign_colors.get('parenthesis', '') + ')' +
+            self.sign_colors.get('data', '')
+        )
+
+    _dispatch[_collections.defaultdict.__repr__] = _pprint_default_dict
+
+    def _pprint_counter(self, obj, stream, indent, allowance, context, level):
+        if not len(obj):
+            stream.write(repr(obj))
+            return
+        cls = obj.__class__
+        stream.write(
+            cls.__name__ + self.sign_colors.get('parenthesis') + '(' +
+            self.sign_colors.get('curly-braces') + '{' + self.sign_colors.get('data')
+        )
+        if self._indent_per_level > 1:
+            stream.write((self._indent_per_level - 1) * ' ')
+        items = obj.most_common()
+        self._format_dict_items(
+            items, stream, indent + len(cls.__name__) + 1, allowance + 2, context, level
+        )
+        stream.write(
+            self.sign_colors.get('curly-braces', '') + '}' +
+            self.sign_colors.get('parenthesis', '') + ')' +
+            self.sign_colors.get('data', '')
+        )
+
+    _dispatch[_collections.Counter.__repr__] = _pprint_counter
+
+    def _pprint_chain_map(self, obj, stream, indent, allowance, context, level):
+        if not len(obj.maps):
+            stream.write(repr(obj))
+            return
+        cls = obj.__class__
+        stream.write(
+            cls.__name__ + self.sign_colors.get('parenthesis', '') + '(' +
+            self.sign_colors.get('data', '')
+        )
+        indent += len(cls.__name__) + 1
+        for i, m in enumerate(obj.maps):
+            if i == len(obj.maps) - 1:
+                self._format(m, stream, indent, allowance + 1, context, level)
+                stream.write(
+                    self.sign_colors.get('parenthesis', '') + ')' +
+                    self.sign_colors.get('data', '')
+                )
+            else:
+                self._format(m, stream, indent, 1, context, level)
+                stream.write(
+                    self.sign_colors.get('comma', '') + ',\n' +
+                    self.sign_colors.get('data', '') + ' ' * indent
+                )
+
+    _dispatch[_collections.ChainMap.__repr__] = _pprint_chain_map
+
+    def _pprint_deque(self, obj, stream, indent, allowance, context, level):
+        if not len(obj):
+            stream.write(repr(obj))
+            return
+        cls = obj.__class__
+        stream.write(
+            cls.__name__ + self.sign_colors.get('parenthesis', '') + '(' +
+            self.sign_colors.get('data', '')
+        )
+        indent += len(cls.__name__) + 1
+        stream.write(
+            self.sign_colors.get('square-brackets', '') + '[' +
+            self.sign_colors.get('data', '')
+        )
+        if obj.maxlen is None:
+            self._format_items(obj, stream, indent, allowance + 2, context, level)
+            stream.write(
+                self.sign_colors.get('square-brackets', '') + ']' +
+                self.sign_colors.get('parenthesis', '') + ')' +
+                self.sign_colors.get('data', '')
+            )
+        else:
+            self._format_items(obj, stream, indent, 2, context, level)
+            rml = self._repr(obj.maxlen, context, level)
+            stream.write(
+                self.sign_colors.get('square-brackets', '') + ']' +
+                self.sign_colors.get('comma', '') + ',' +
+                self.sign_colors.get('data', '') + '\n' + (' ' * indent) + 'maxlen=' +
+                rml + self.sign_colors.get('parenthesis', '') + ')'
+            )
+
+    _dispatch[_collections.deque.__repr__] = _pprint_deque
+
+    def _pprint_user_dict(self, obj, stream, indent, allowance, context, level):
+        self._format(obj.data, stream, indent, allowance, context, level - 1)
+
+    _dispatch[_collections.UserDict.__repr__] = _pprint_user_dict
+
+    def _pprint_user_list(self, obj, stream, indent, allowance, context, level):
+        self._format(obj.data, stream, indent, allowance, context, level - 1)
+
+    _dispatch[_collections.UserList.__repr__] = _pprint_user_list
+
+    def _pprint_user_string(self, obj, stream, indent, allowance, context, level):
+        self._format(obj.data, stream, indent, allowance, context, level - 1)
+
+    _dispatch[_collections.UserString.__repr__] = _pprint_user_string
+
+
+def pformat(
+    obj,
+    indent=1,
+    width=80,
+    depth=None,
+    signs_colors: _Optional[_Mapping[str, str]] = None,
+    *,
+    compact=False,
+    sort_dicts=True,
+    underscore_numbers=False,
+    **kwargs
+):
+    """Format a Python object into a pretty-printed representation.
+
+    :param obj: the object to format.
+    :param indent: the number of spaces to indent for each level of nesting.
+    :param width: the maximum width of the formatted representation.
+    :param depth: the maximum depth to print out nested structures.
+    :param signs_colors: a mapping of signs and colors.
+    :param compact: if `True`, several items will be combined in one line.
+    :param sort_dicts: if `True`, dictionaries will be sorted by key. (py38+)
+    :param underscore_numbers: if `True`, numbers will be represented with an
+        underscore between every digit. (py310+)
+    :param kwargs: additional keyword arguments to pass to the underlying pretty
+        printer.
+    :return: the formatted representation.
+    """
+    return PrettyPrinter(
+        indent=indent,
+        width=width,
+        depth=depth,
+        compact=compact,
+        sign_colors=signs_colors,
+        sort_dicts=sort_dicts,
+        underscore_numbers=underscore_numbers,
+        **kwargs
+    ).pformat(obj)
```

### Comparing `log21-2.8.1b0/src/log21/ProgressBar.py` & `log21-2.9.0/src/log21/ProgressBar.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,393 +1,393 @@
-# log21.ProgressBar.py
-# CodeWriter21
-
-from __future__ import annotations
-
-import shutil as _shutil
-from typing import Any as _Any, Mapping as _Mapping, Optional as _Optional
-
-import log21 as _log21
-from log21.Colors import get_colors as _gc
-from log21.Logger import Logger as _Logger
-from log21.StreamHandler import ColorizingStreamHandler as _ColorizingStreamHandler
-
-_logger = _Logger('ProgressBar')
-_logger.addHandler(_ColorizingStreamHandler())
-
-__all__ = ['ProgressBar']
-
-
-class ProgressBar:  # pylint: disable=too-many-instance-attributes, line-too-long
-    """
-    Usage Example:
-        >>> pb = ProgressBar(width=20, show_percentage=False, prefix='[', suffix=']',
-        ... fill='=', empty='-')
-        >>> pb(0, 10)
-        [/-----------------]
-        >>> pb(1, 10)
-        [==----------------]
-        >>> pb(2, 10)
-        [====\\-------------]
-        >>>
-        >>> # A better example
-        >>> import time
-        >>> pb = ProgressBar()
-        >>> for i in range(500):
-        ...     pb(i + 1, 500)
-        ...     time.sleep(0.01)
-        ...
-        |███████████████████████████████████████████████████████████████████| 100%
-        >>> # Of course, You should try it yourself to see the progress! XD
-        >>>
-    """
-
-    def __init__(
-        self,
-        *,
-        width: _Optional[int] = None,
-        show_percentage: bool = True,
-        prefix: str = '|',
-        suffix: str = '|',
-        fill: str = '█',
-        empty: str = ' ',
-        format_: _Optional[str] = None,
-        style: str = '%',
-        new_line_when_complete: bool = True,
-        colors: _Optional[_Mapping[str, str]] = None,
-        no_color: bool = False,
-        logger: _log21.Logger = _logger,
-        additional_variables: _Optional[_Mapping[str, _Any]] = None
-    ):  # pylint: disable=too-many-branches, too-many-statements
-        """
-        :param args: Prevents the use of positional arguments
-        :param width: The width of the progress bar
-        :param show_percentage: Whether to show the percentage of the progress
-        :param prefix: The prefix of the progress bar
-        :param suffix: The suffix of the progress bar
-        :param fill: The fill character of the progress bar
-        :param empty: The empty character of the progress bar
-        :param format_: The format of the progress bar
-        :param style: The style that is used to format the progress bar
-        :param new_line_when_complete: Whether to print a new line when the progress is
-            complete or failed
-        :param colors: The colors of the progress bar
-        :param no_color: If True, removes the colors of the progress bar
-        :param logger: The logger to use
-        :param additional_variables: Additional variables to use in the format and their
-            default values
-        """
-        # Sets a default value for the width
-        if width is None:
-            try:
-                width = _shutil.get_terminal_size().columns - 1
-            except OSError:
-                width = 50
-            if width < 1:
-                width = 50
-        self.width = width
-        if self.width < 3:
-            raise ValueError('`width` must be greater than 1')
-        if not isinstance(fill, str):
-            raise TypeError('`fill` must be a string')
-        if not isinstance(empty, str):
-            raise TypeError('`empty` must be a string')
-        if not isinstance(prefix, str):
-            raise TypeError('`prefix` must be a string')
-        if not isinstance(suffix, str):
-            raise TypeError('`suffix` must be a string')
-        if len(fill) != 1:
-            raise ValueError('`fill` must be a single character')
-        if len(empty) != 1:
-            raise ValueError('`empty` must be a single character')
-        if style not in ['%', '{']:
-            raise ValueError('`style` must be either `%` or `{`')
-        if colors and no_color:
-            raise PermissionError(
-                'You cannot use `no_color` and `colors` parameters together!'
-            )
-        if additional_variables:
-            if not isinstance(additional_variables, _Mapping):
-                raise TypeError(
-                    '`additional_variables` must be a dictionary like object.'
-                )
-            for key, value in additional_variables.items():
-                if not isinstance(key, str):
-                    raise TypeError('`additional_variables` keys must be strings')
-                if not isinstance(value, str):
-                    additional_variables[key] = str(value)
-        else:
-            additional_variables = {}
-
-        self.colors = {
-            'progress in-progress': _gc('LightYellow'),
-            'progress complete': _gc('LightGreen'),
-            'progress failed': _gc('LightRed'),
-            'percentage in-progress': _gc('LightBlue'),
-            'percentage complete': _gc('LightCyan'),
-            'percentage failed': _gc('LightRed'),
-            'prefix-color in-progress': _gc('Yellow'),
-            'prefix-color complete': _gc('Green'),
-            'prefix-color failed': _gc('Red'),
-            'suffix-color in-progress': _gc('Yellow'),
-            'suffix-color complete': _gc('Green'),
-            'suffix-color failed': _gc('Red'),
-            'reset-color': _gc('Reset'),
-        }
-        self.spinner = ['|', '/', '-', '\\']
-
-        self.fill = fill
-        self.empty = empty
-        self.prefix = prefix
-        self.suffix = suffix
-        if format_:
-            self.format = format_
-        else:
-            self.format = (
-                '%(prefix)s%(bar)s%(suffix)s %(percentage)s%%'
-                if show_percentage else '%(prefix)s%(bar)s%(suffix)s'
-            )
-            style = '%'
-        self.style = style
-        self.new_line_when_complete = new_line_when_complete
-        if colors:
-            for key, value in colors.items():
-                self.colors[key] = value
-        if no_color:
-            self.colors = {name: '' for name in self.colors}
-        self.logger = logger
-        self.additional_variables = additional_variables
-        self.i = 0
-
-    def get_bar(self, progress: float, total: float, **kwargs) -> str:
-        """Return the progress bar as a string.
-
-        :param progress: The current progress. (e.g. 21)
-        :param total: The total progress. (e.g. 100)
-        :param kwargs: Additional variables to be used in the format
-            string.
-        :raises ValueError: If the style is not supported.
-            Set the style to one of the following:
-            + '%'
-            + '{'
-            e.g. bar = ProgressBar(style='{')
-        :return: The progress bar as a string.
-        """
-        if progress == total:
-            return self.progress_complete(**kwargs)
-        if progress > total or progress < 0:
-            return self.progress_failed(progress, total, **kwargs)
-        return self.progress_in_progress(progress, total, **kwargs)
-
-    def progress_in_progress(self, progress: float, total: float, **kwargs) -> str:
-        """Return the progress bar as a string when the progress is in progress.
-
-        :param progress: The current progress. (e.g. 21)
-        :param total: The total progress. (e.g. 100)
-        :param kwargs: Additional variables to be used in the format
-            string.
-        :raises ValueError: If the style is not supported. (supported
-            styles: '%', '{')
-        :return: The progress bar as a string.
-        """
-        percentage = str(round(progress / total * 100, 2))
-        progress_dict = {
-            'prefix': self.prefix,
-            'bar': '',
-            'suffix': self.suffix,
-            'percentage': percentage,
-            **self.additional_variables
-        }
-        for key, value in kwargs.items():
-            if key in ['prefix', 'bar', 'suffix', 'percentage']:
-                raise ValueError(f'`{key}` is a reserved keyword')
-            progress_dict[key] = value
-
-        if self.style == '%':
-            used_characters = len(self.format % progress_dict)
-        elif self.style == '{':
-            used_characters = len(self.format.format(**progress_dict))
-        else:
-            raise ValueError('`style` must be either `%` or `{`')
-
-        fill_length = round(progress / total * (self.width - used_characters))
-        empty_length = (self.width - (fill_length + used_characters)) - 1
-
-        if self.i >= 3:
-            self.i = 0
-        else:
-            self.i += 1
-        spinner_char = self.spinner[self.i] if empty_length > 0 else ''
-
-        progress_dict = {
-            'prefix':
-            self.colors['prefix-color in-progress'] + self.prefix +
-            self.colors['reset-color'],
-            'bar':
-            self.colors['progress in-progress'] +
-            (self.fill * fill_length + spinner_char + self.empty * empty_length) +
-            self.colors['reset-color'],
-            'suffix':
-            self.colors['suffix-color in-progress'] + self.suffix +
-            self.colors['reset-color'],
-            'percentage':
-            self.colors["percentage in-progress"] + str(percentage) +
-            self.colors['reset-color'],
-            **self.additional_variables
-        }
-        for key, value in kwargs.items():
-            progress_dict[key] = value
-
-        if self.style == '%':
-            return '\r' + self.format % progress_dict + self.colors['reset-color']
-        if self.style == '{':
-            return '\r' + self.format.format(**progress_dict
-                                             ) + self.colors['reset-color']
-        raise ValueError('`style` must be either `%` or `{`')
-
-    def progress_complete(self, **kwargs) -> str:
-        """Prints the progress bar as complete.
-
-        :param kwargs: Additional variables to be passed to the format string.
-        :raises ValueError: If the style is not either `%` or `{`.
-        :return: The formatted progress bar.
-        """
-        progress_dict = {
-            'prefix': self.prefix,
-            'bar': '',
-            'suffix': self.suffix,
-            'percentage': '100',
-            **self.additional_variables
-        }
-        for key, value in kwargs.items():
-            if key in ['prefix', 'bar', 'suffix', 'percentage']:
-                raise ValueError(f'`{key}` is a reserved keyword')
-            progress_dict[key] = value
-
-        if self.style == '%':
-            bar_length = self.width - len(self.format % progress_dict)
-        elif self.style == '{':
-            bar_length = self.width - len(self.format.format(**progress_dict))
-        else:
-            raise ValueError('`style` must be either `%` or `{`')
-
-        progress_dict = {
-            'prefix':
-            self.colors['prefix-color complete'] + self.prefix +
-            self.colors['reset-color'],
-            'bar':
-            self.colors['progress complete'] + (self.fill * bar_length) +
-            self.colors['reset-color'],
-            'suffix':
-            self.colors['suffix-color complete'] + self.suffix +
-            self.colors['reset-color'],
-            'percentage':
-            self.colors["percentage complete"] + '100' + self.colors['reset-color'],
-            **self.additional_variables
-        }
-        for key, value in kwargs.items():
-            progress_dict[key] = value
-
-        if self.style == '%':
-            return (
-                '\r' + self.format % progress_dict + self.colors['reset-color'] +
-                ('\n' if self.new_line_when_complete else '')
-            )
-        if self.style == '{':
-            return (
-                '\r' + self.format.format(**progress_dict) +
-                self.colors['reset-color'] +
-                ('\n' if self.new_line_when_complete else '')
-            )
-        raise ValueError('`style` must be either `%` or `{`')
-
-    def progress_failed(self, progress: float, total: float, **kwargs):
-        """Returns a progress bar with a failed state.
-
-        :param progress: The current progress.
-        :param total: The total progress.
-        :param kwargs: Additional variables to be passed to the format string.
-        :raises ValueError: If the style is not `%` or `{`.
-        :return: A progress bar with a failed state.
-        """
-        progress_dict = {
-            'prefix': self.prefix,
-            'bar': '',
-            'suffix': self.suffix,
-            'percentage': str(round(progress / total * 100, 2)),
-            **self.additional_variables
-        }
-        for key, value in kwargs.items():
-            if key in ['prefix', 'bar', 'suffix', 'percentage']:
-                raise ValueError(f'`{key}` is a reserved keyword')
-            progress_dict[key] = value
-
-        if self.style == '%':
-            bar_length = self.width - len(self.format % progress_dict)
-        elif self.style == '{':
-            bar_length = self.width - len(self.format.format(**progress_dict))
-        else:
-            raise ValueError('`style` must be either `%` or `{`')
-
-        if progress > total:
-            bar_char = self.fill
-        else:
-            bar_char = self.empty
-
-        progress_dict = {
-            'prefix':
-            self.colors['prefix-color failed'] + self.prefix +
-            self.colors['reset-color'],
-            'bar':
-            self.colors['progress failed'] + (bar_char * bar_length) +
-            self.colors['reset-color'],
-            'suffix':
-            self.colors['suffix-color failed'] + self.suffix +
-            self.colors['reset-color'],
-            'percentage':
-            self.colors["percentage failed"] + progress_dict['percentage'] +
-            self.colors['reset-color'],
-            **self.additional_variables
-        }
-        for key, value in kwargs.items():
-            progress_dict[key] = value
-
-        if self.style == '%':
-            progress_bar = self.format % progress_dict
-        elif self.style == '{':
-            progress_bar = self.format.format(**progress_dict)
-        else:
-            raise ValueError('`style` must be either `%` or `{`')
-
-        return '\r' + progress_bar + self.colors['reset-color'] + (
-            '\n' if self.new_line_when_complete else ''
-        )
-
-    def __call__(
-        self,
-        progress: float,
-        total: float,
-        logger: _Optional[_log21.Logger] = None,
-        **kwargs
-    ):
-        if not logger:
-            logger = self.logger
-
-        logger.print(self.get_bar(progress, total, **kwargs), end='')
-
-    def update(
-        self,
-        progress: float,
-        total: float,
-        logger: _Optional[_log21.Logger] = None,
-        **kwargs
-    ):
-        """Update the progress bar.
-
-        :param progress: The current progress.
-        :param total: The total progress.
-        :param logger: The logger to use. If not specified, the logger specified in the
-            constructor will be used.
-        :param kwargs: Additional variables to be used in the format string.
-        :raises ValueError: If the style is not `%` or `{`.
-        """
-        self(progress, total, logger, **kwargs)
+# log21.ProgressBar.py
+# CodeWriter21
+
+from __future__ import annotations
+
+import shutil as _shutil
+from typing import Any as _Any, Mapping as _Mapping, Optional as _Optional
+
+import log21 as _log21
+from log21.Colors import get_colors as _gc
+from log21.Logger import Logger as _Logger
+from log21.StreamHandler import ColorizingStreamHandler as _ColorizingStreamHandler
+
+_logger = _Logger('ProgressBar')
+_logger.addHandler(_ColorizingStreamHandler())
+
+__all__ = ['ProgressBar']
+
+
+class ProgressBar:  # pylint: disable=too-many-instance-attributes, line-too-long
+    """
+    Usage Example:
+        >>> pb = ProgressBar(width=20, show_percentage=False, prefix='[', suffix=']',
+        ... fill='=', empty='-')
+        >>> pb(0, 10)
+        [/-----------------]
+        >>> pb(1, 10)
+        [==----------------]
+        >>> pb(2, 10)
+        [====\\-------------]
+        >>>
+        >>> # A better example
+        >>> import time
+        >>> pb = ProgressBar()
+        >>> for i in range(500):
+        ...     pb(i + 1, 500)
+        ...     time.sleep(0.01)
+        ...
+        |███████████████████████████████████████████████████████████████████| 100%
+        >>> # Of course, You should try it yourself to see the progress! XD
+        >>>
+    """
+
+    def __init__(
+        self,
+        *,
+        width: _Optional[int] = None,
+        show_percentage: bool = True,
+        prefix: str = '|',
+        suffix: str = '|',
+        fill: str = '█',
+        empty: str = ' ',
+        format_: _Optional[str] = None,
+        style: str = '%',
+        new_line_when_complete: bool = True,
+        colors: _Optional[_Mapping[str, str]] = None,
+        no_color: bool = False,
+        logger: _log21.Logger = _logger,
+        additional_variables: _Optional[_Mapping[str, _Any]] = None
+    ):  # pylint: disable=too-many-branches, too-many-statements
+        """
+        :param args: Prevents the use of positional arguments
+        :param width: The width of the progress bar
+        :param show_percentage: Whether to show the percentage of the progress
+        :param prefix: The prefix of the progress bar
+        :param suffix: The suffix of the progress bar
+        :param fill: The fill character of the progress bar
+        :param empty: The empty character of the progress bar
+        :param format_: The format of the progress bar
+        :param style: The style that is used to format the progress bar
+        :param new_line_when_complete: Whether to print a new line when the progress is
+            complete or failed
+        :param colors: The colors of the progress bar
+        :param no_color: If True, removes the colors of the progress bar
+        :param logger: The logger to use
+        :param additional_variables: Additional variables to use in the format and their
+            default values
+        """
+        # Sets a default value for the width
+        if width is None:
+            try:
+                width = _shutil.get_terminal_size().columns - 1
+            except OSError:
+                width = 50
+            if width < 1:
+                width = 50
+        self.width = width
+        if self.width < 3:
+            raise ValueError('`width` must be greater than 1')
+        if not isinstance(fill, str):
+            raise TypeError('`fill` must be a string')
+        if not isinstance(empty, str):
+            raise TypeError('`empty` must be a string')
+        if not isinstance(prefix, str):
+            raise TypeError('`prefix` must be a string')
+        if not isinstance(suffix, str):
+            raise TypeError('`suffix` must be a string')
+        if len(fill) != 1:
+            raise ValueError('`fill` must be a single character')
+        if len(empty) != 1:
+            raise ValueError('`empty` must be a single character')
+        if style not in ['%', '{']:
+            raise ValueError('`style` must be either `%` or `{`')
+        if colors and no_color:
+            raise PermissionError(
+                'You cannot use `no_color` and `colors` parameters together!'
+            )
+        if additional_variables:
+            if not isinstance(additional_variables, _Mapping):
+                raise TypeError(
+                    '`additional_variables` must be a dictionary like object.'
+                )
+            for key, value in additional_variables.items():
+                if not isinstance(key, str):
+                    raise TypeError('`additional_variables` keys must be strings')
+                if not isinstance(value, str):
+                    additional_variables[key] = str(value)
+        else:
+            additional_variables = {}
+
+        self.colors = {
+            'progress in-progress': _gc('LightYellow'),
+            'progress complete': _gc('LightGreen'),
+            'progress failed': _gc('LightRed'),
+            'percentage in-progress': _gc('LightBlue'),
+            'percentage complete': _gc('LightCyan'),
+            'percentage failed': _gc('LightRed'),
+            'prefix-color in-progress': _gc('Yellow'),
+            'prefix-color complete': _gc('Green'),
+            'prefix-color failed': _gc('Red'),
+            'suffix-color in-progress': _gc('Yellow'),
+            'suffix-color complete': _gc('Green'),
+            'suffix-color failed': _gc('Red'),
+            'reset-color': _gc('Reset'),
+        }
+        self.spinner = ['|', '/', '-', '\\']
+
+        self.fill = fill
+        self.empty = empty
+        self.prefix = prefix
+        self.suffix = suffix
+        if format_:
+            self.format = format_
+        else:
+            self.format = (
+                '%(prefix)s%(bar)s%(suffix)s %(percentage)s%%'
+                if show_percentage else '%(prefix)s%(bar)s%(suffix)s'
+            )
+            style = '%'
+        self.style = style
+        self.new_line_when_complete = new_line_when_complete
+        if colors:
+            for key, value in colors.items():
+                self.colors[key] = value
+        if no_color:
+            self.colors = {name: '' for name in self.colors}
+        self.logger = logger
+        self.additional_variables = additional_variables
+        self.i = 0
+
+    def get_bar(self, progress: float, total: float, **kwargs) -> str:
+        """Return the progress bar as a string.
+
+        :param progress: The current progress. (e.g. 21)
+        :param total: The total progress. (e.g. 100)
+        :param kwargs: Additional variables to be used in the format
+            string.
+        :raises ValueError: If the style is not supported.
+            Set the style to one of the following:
+            + '%'
+            + '{'
+            e.g. bar = ProgressBar(style='{')
+        :return: The progress bar as a string.
+        """
+        if progress == total:
+            return self.progress_complete(**kwargs)
+        if progress > total or progress < 0:
+            return self.progress_failed(progress, total, **kwargs)
+        return self.progress_in_progress(progress, total, **kwargs)
+
+    def progress_in_progress(self, progress: float, total: float, **kwargs) -> str:
+        """Return the progress bar as a string when the progress is in progress.
+
+        :param progress: The current progress. (e.g. 21)
+        :param total: The total progress. (e.g. 100)
+        :param kwargs: Additional variables to be used in the format
+            string.
+        :raises ValueError: If the style is not supported. (supported
+            styles: '%', '{')
+        :return: The progress bar as a string.
+        """
+        percentage = str(round(progress / total * 100, 2))
+        progress_dict = {
+            'prefix': self.prefix,
+            'bar': '',
+            'suffix': self.suffix,
+            'percentage': percentage,
+            **self.additional_variables
+        }
+        for key, value in kwargs.items():
+            if key in ['prefix', 'bar', 'suffix', 'percentage']:
+                raise ValueError(f'`{key}` is a reserved keyword')
+            progress_dict[key] = value
+
+        if self.style == '%':
+            used_characters = len(self.format % progress_dict)
+        elif self.style == '{':
+            used_characters = len(self.format.format(**progress_dict))
+        else:
+            raise ValueError('`style` must be either `%` or `{`')
+
+        fill_length = round(progress / total * (self.width - used_characters))
+        empty_length = (self.width - (fill_length + used_characters)) - 1
+
+        if self.i >= 3:
+            self.i = 0
+        else:
+            self.i += 1
+        spinner_char = self.spinner[self.i] if empty_length > 0 else ''
+
+        progress_dict = {
+            'prefix':
+            self.colors['prefix-color in-progress'] + self.prefix +
+            self.colors['reset-color'],
+            'bar':
+            self.colors['progress in-progress'] +
+            (self.fill * fill_length + spinner_char + self.empty * empty_length) +
+            self.colors['reset-color'],
+            'suffix':
+            self.colors['suffix-color in-progress'] + self.suffix +
+            self.colors['reset-color'],
+            'percentage':
+            self.colors["percentage in-progress"] + str(percentage) +
+            self.colors['reset-color'],
+            **self.additional_variables
+        }
+        for key, value in kwargs.items():
+            progress_dict[key] = value
+
+        if self.style == '%':
+            return '\r' + self.format % progress_dict + self.colors['reset-color']
+        if self.style == '{':
+            return '\r' + self.format.format(**progress_dict
+                                             ) + self.colors['reset-color']
+        raise ValueError('`style` must be either `%` or `{`')
+
+    def progress_complete(self, **kwargs) -> str:
+        """Prints the progress bar as complete.
+
+        :param kwargs: Additional variables to be passed to the format string.
+        :raises ValueError: If the style is not either `%` or `{`.
+        :return: The formatted progress bar.
+        """
+        progress_dict = {
+            'prefix': self.prefix,
+            'bar': '',
+            'suffix': self.suffix,
+            'percentage': '100',
+            **self.additional_variables
+        }
+        for key, value in kwargs.items():
+            if key in ['prefix', 'bar', 'suffix', 'percentage']:
+                raise ValueError(f'`{key}` is a reserved keyword')
+            progress_dict[key] = value
+
+        if self.style == '%':
+            bar_length = self.width - len(self.format % progress_dict)
+        elif self.style == '{':
+            bar_length = self.width - len(self.format.format(**progress_dict))
+        else:
+            raise ValueError('`style` must be either `%` or `{`')
+
+        progress_dict = {
+            'prefix':
+            self.colors['prefix-color complete'] + self.prefix +
+            self.colors['reset-color'],
+            'bar':
+            self.colors['progress complete'] + (self.fill * bar_length) +
+            self.colors['reset-color'],
+            'suffix':
+            self.colors['suffix-color complete'] + self.suffix +
+            self.colors['reset-color'],
+            'percentage':
+            self.colors["percentage complete"] + '100' + self.colors['reset-color'],
+            **self.additional_variables
+        }
+        for key, value in kwargs.items():
+            progress_dict[key] = value
+
+        if self.style == '%':
+            return (
+                '\r' + self.format % progress_dict + self.colors['reset-color'] +
+                ('\n' if self.new_line_when_complete else '')
+            )
+        if self.style == '{':
+            return (
+                '\r' + self.format.format(**progress_dict) +
+                self.colors['reset-color'] +
+                ('\n' if self.new_line_when_complete else '')
+            )
+        raise ValueError('`style` must be either `%` or `{`')
+
+    def progress_failed(self, progress: float, total: float, **kwargs):
+        """Returns a progress bar with a failed state.
+
+        :param progress: The current progress.
+        :param total: The total progress.
+        :param kwargs: Additional variables to be passed to the format string.
+        :raises ValueError: If the style is not `%` or `{`.
+        :return: A progress bar with a failed state.
+        """
+        progress_dict = {
+            'prefix': self.prefix,
+            'bar': '',
+            'suffix': self.suffix,
+            'percentage': str(round(progress / total * 100, 2)),
+            **self.additional_variables
+        }
+        for key, value in kwargs.items():
+            if key in ['prefix', 'bar', 'suffix', 'percentage']:
+                raise ValueError(f'`{key}` is a reserved keyword')
+            progress_dict[key] = value
+
+        if self.style == '%':
+            bar_length = self.width - len(self.format % progress_dict)
+        elif self.style == '{':
+            bar_length = self.width - len(self.format.format(**progress_dict))
+        else:
+            raise ValueError('`style` must be either `%` or `{`')
+
+        if progress > total:
+            bar_char = self.fill
+        else:
+            bar_char = self.empty
+
+        progress_dict = {
+            'prefix':
+            self.colors['prefix-color failed'] + self.prefix +
+            self.colors['reset-color'],
+            'bar':
+            self.colors['progress failed'] + (bar_char * bar_length) +
+            self.colors['reset-color'],
+            'suffix':
+            self.colors['suffix-color failed'] + self.suffix +
+            self.colors['reset-color'],
+            'percentage':
+            self.colors["percentage failed"] + progress_dict['percentage'] +
+            self.colors['reset-color'],
+            **self.additional_variables
+        }
+        for key, value in kwargs.items():
+            progress_dict[key] = value
+
+        if self.style == '%':
+            progress_bar = self.format % progress_dict
+        elif self.style == '{':
+            progress_bar = self.format.format(**progress_dict)
+        else:
+            raise ValueError('`style` must be either `%` or `{`')
+
+        return '\r' + progress_bar + self.colors['reset-color'] + (
+            '\n' if self.new_line_when_complete else ''
+        )
+
+    def __call__(
+        self,
+        progress: float,
+        total: float,
+        logger: _Optional[_log21.Logger] = None,
+        **kwargs
+    ):
+        if not logger:
+            logger = self.logger
+
+        logger.print(self.get_bar(progress, total, **kwargs), end='')
+
+    def update(
+        self,
+        progress: float,
+        total: float,
+        logger: _Optional[_log21.Logger] = None,
+        **kwargs
+    ):
+        """Update the progress bar.
+
+        :param progress: The current progress.
+        :param total: The total progress.
+        :param logger: The logger to use. If not specified, the logger specified in the
+            constructor will be used.
+        :param kwargs: Additional variables to be used in the format string.
+        :raises ValueError: If the style is not `%` or `{`.
+        """
+        self(progress, total, logger, **kwargs)
```

### Comparing `log21-2.8.1b0/src/log21/StreamHandler.py` & `log21-2.9.0/src/log21/StreamHandler.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,203 +1,203 @@
-# log21.StreamHandler.py
-# CodeWriter21
-
-import os as _os
-import re as _re
-import shutil as _shutil
-from typing import Optional as _Optional
-from logging import StreamHandler as _StreamHandler
-
-from log21.Colors import (get_colors as _gc, hex_escape as _hex_escape,
-                          ansi_escape as _ansi_escape)
-
-__all__ = ['IS_WINDOWS', 'ColorizingStreamHandler', 'StreamHandler']
-
-IS_WINDOWS = _os.name == 'nt'
-
-if IS_WINDOWS:
-    import ctypes
-
-
-class StreamHandler(_StreamHandler):
-    """A StreamHandler that can handle carriage returns and new lines."""
-    terminator = ''
-
-    def __init__(
-        self,
-        handle_carriage_return: bool = True,
-        handle_new_line: bool = True,
-        stream=None,
-        formatter=None,
-        level=None
-    ):
-        """Initialize the StreamHandler.
-
-        :param handle_carriage_return: Whether to handle carriage
-            returns.
-        :param handle_new_line: Whether to handle new lines.
-        :param stream: The stream to write to.
-        :param formatter: The formatter to use.
-        :param level: The level to log at.
-        """
-        self.HandleCR = handle_carriage_return
-        self.HandleNL = handle_new_line
-        super().__init__(stream=stream)
-        if formatter is not None:
-            self.setFormatter(formatter)
-        if level is not None:
-            self.setLevel(level)
-
-    def check_cr(self, record):
-        """Check if the record contains a carriage return and handle it."""
-        if record.msg:
-            msg = _hex_escape.sub(
-                '', _ansi_escape.sub('', record.msg.strip(' \t\n\x0b\x0c'))
-            )
-            if '\r' == msg[:1]:
-                file_descriptor = getattr(self.stream, 'fileno', None)
-                if file_descriptor:
-                    file_descriptor = file_descriptor()
-                    if file_descriptor in (1, 2):  # stdout or stderr
-                        self.stream.write(
-                            '\r' + (
-                                ' ' * (
-                                    _shutil.get_terminal_size(file_descriptor).columns -
-                                    1
-                                )
-                            ) + '\r'
-                        )
-                        index = record.msg.rfind('\r')
-                        find = _re.compile(r'(\x1b\[(?:\d+(?:;(?:\d+))*)m)')
-                        record.msg = _gc(*find.split(record.msg[:index])
-                                         ) + record.msg[index + 1:]
-
-    def check_nl(self, record):
-        """Check if the record contains a newline and handle it."""
-        while record.msg and record.msg[0] == '\n':
-            file_descriptor = getattr(self.stream, 'fileno', None)
-            if file_descriptor:
-                file_descriptor = file_descriptor()
-                if file_descriptor in (1, 2):  # stdout or stderr
-                    self.stream.write('\n')
-                    record.msg = record.msg[1:]
-
-    def emit(self, record):
-        if self.HandleCR:
-            self.check_cr(record)
-        if self.HandleNL:
-            self.check_nl(record)
-        super().emit(record)
-
-    def clear_line(self, length: _Optional[int] = None):
-        """Clear the current line.
-
-        :param length: The length of the line to clear.
-        :return:
-        """
-        file_descriptor = getattr(self.stream, 'fileno', None)
-        if file_descriptor:
-            file_descriptor = file_descriptor()
-            if file_descriptor in (1, 2):
-                if length is None:
-                    length = _shutil.get_terminal_size(file_descriptor).columns
-                self.stream.write('\r' + (' ' * (length - 1)) + '\r')
-
-
-# A stream handler that supports colorizing.
-class ColorizingStreamHandler(StreamHandler):
-    """A stream handler that supports colorizing even in Windows."""
-
-    def emit(self, record):
-        try:
-            if self.HandleCR:
-                self.check_cr(record)
-            if self.HandleNL:
-                self.check_nl(record)
-            msg = self.format(record)
-            if IS_WINDOWS:
-                self.convert_and_write(msg)
-                self.convert_and_write(self.terminator)
-            else:
-                self.write(msg)
-                self.write(self.terminator)
-            self.flush()
-        except Exception:  # pylint: disable=broad-except
-            self.handleError(record)
-
-    # Writes colorized text to the Windows console.
-    def convert_and_write(self, message):
-        """Convert the message to a Windows console colorized message and write
-        it to the stream."""
-        nt_color_map = {
-            30: 0,  # foreground: black   - 0b00000000
-            31: 4,  # foreground: red     - 0b00000100
-            32: 2,  # foreground: green   - 0b00000010
-            33: 6,  # foreground: yellow  - 0b00000110
-            34: 1,  # foreground: blue    - 0b00000001
-            35: 5,  # foreground: magenta - 0b00000101
-            36: 3,  # foreground: cyan    - 0b00000011
-            37: 7,  # foreground: white   - 0b00000111
-            40: 0,  # background: black   - 0b00000000 = 0 << 4
-            41: 64,  # background: red     - 0b01000000 = 4 << 4
-            42: 32,  # background: green   - 0b00100000 = 2 << 4
-            43: 96,  # background: yellow  - 0b01100000 = 6 << 4
-            44: 16,  # background: blue    - 0b00010000 = 1 << 4
-            45: 80,  # background: magenta - 0b01010000 = 5 << 4
-            46: 48,  # background: cyan    - 0b00110000 = 3 << 4
-            47: 112,  # background: white   - 0b01110000 = 7 << 4
-            90: 8,  # foreground: gray          - 0b00001000
-            91: 12,  # foreground: light red     - 0b00001100
-            92: 10,  # foreground: light green   - 0b00001010
-            93: 14,  # foreground: light yellow  - 0b00001110
-            94: 9,  # foreground: light blue    - 0b00001001
-            95: 13,  # foreground: light magenta - 0b00001101
-            96: 11,  # foreground: light cyan    - 0b00001011
-            97: 15,  # foreground: light white   - 0b00001111
-            100: 128,  # background: gray          - 0b10000000 = 8  << 4
-            101: 192,  # background: light red     - 0b11000000 = 12 << 4
-            102: 160,  # background: light green   - 0b10100000 = 10 << 4
-            103: 224,  # background: light yellow  - 0b11100000 = 14 << 4
-            104: 144,  # background: light blue    - 0b10010000 = 9  << 4
-            105: 208,  # background: light magenta - 0b11010000 = 13 << 4
-            106: 176,  # background: light cyan    - 0b10110000 = 11 << 4
-            107: 240,  # background: light white   - 0b11110000 = 15 << 4
-            2: 8,
-            0: 7
-        }
-
-        parts = _ansi_escape.split(message)
-        win_handle = None
-        file_descriptor = getattr(self.stream, 'fileno', None)
-
-        if file_descriptor:
-            file_descriptor = file_descriptor()
-
-            if file_descriptor in (1, 2):  # stdout or stderr
-                win_handle = ctypes.windll.kernel32.GetStdHandle(-10 - file_descriptor)
-
-        while parts:
-            text = parts.pop(0)
-
-            if text:
-                self.write(text)
-
-            if parts:
-                params = parts.pop(0)
-
-                if win_handle is not None:
-                    params = [int(p) for p in params.split(';')]
-                    color = 0
-
-                    for param in params:
-                        if param in nt_color_map:
-                            color |= nt_color_map[param]
-                        else:
-                            pass  # error condition ignored
-
-                    ctypes.windll.kernel32.SetConsoleTextAttribute(win_handle, color)
-
-    # Writes the message to the console.
-    def write(self, message):
-        """Write the message to the stream."""
-        self.stream.write(message)
-        self.flush()
+# log21.StreamHandler.py
+# CodeWriter21
+
+import os as _os
+import re as _re
+import shutil as _shutil
+from typing import Optional as _Optional
+from logging import StreamHandler as _StreamHandler
+
+from log21.Colors import (get_colors as _gc, hex_escape as _hex_escape,
+                          ansi_escape as _ansi_escape)
+
+__all__ = ['IS_WINDOWS', 'ColorizingStreamHandler', 'StreamHandler']
+
+IS_WINDOWS = _os.name == 'nt'
+
+if IS_WINDOWS:
+    import ctypes
+
+
+class StreamHandler(_StreamHandler):
+    """A StreamHandler that can handle carriage returns and new lines."""
+    terminator = ''
+
+    def __init__(
+        self,
+        handle_carriage_return: bool = True,
+        handle_new_line: bool = True,
+        stream=None,
+        formatter=None,
+        level=None
+    ):
+        """Initialize the StreamHandler.
+
+        :param handle_carriage_return: Whether to handle carriage
+            returns.
+        :param handle_new_line: Whether to handle new lines.
+        :param stream: The stream to write to.
+        :param formatter: The formatter to use.
+        :param level: The level to log at.
+        """
+        self.HandleCR = handle_carriage_return
+        self.HandleNL = handle_new_line
+        super().__init__(stream=stream)
+        if formatter is not None:
+            self.setFormatter(formatter)
+        if level is not None:
+            self.setLevel(level)
+
+    def check_cr(self, record):
+        """Check if the record contains a carriage return and handle it."""
+        if record.msg:
+            msg = _hex_escape.sub(
+                '', _ansi_escape.sub('', record.msg.strip(' \t\n\x0b\x0c'))
+            )
+            if '\r' == msg[:1]:
+                file_descriptor = getattr(self.stream, 'fileno', None)
+                if file_descriptor:
+                    file_descriptor = file_descriptor()
+                    if file_descriptor in (1, 2):  # stdout or stderr
+                        self.stream.write(
+                            '\r' + (
+                                ' ' * (
+                                    _shutil.get_terminal_size(file_descriptor).columns -
+                                    1
+                                )
+                            ) + '\r'
+                        )
+                        index = record.msg.rfind('\r')
+                        find = _re.compile(r'(\x1b\[(?:\d+(?:;(?:\d+))*)m)')
+                        record.msg = _gc(*find.split(record.msg[:index])
+                                         ) + record.msg[index + 1:]
+
+    def check_nl(self, record):
+        """Check if the record contains a newline and handle it."""
+        while record.msg and record.msg[0] == '\n':
+            file_descriptor = getattr(self.stream, 'fileno', None)
+            if file_descriptor:
+                file_descriptor = file_descriptor()
+                if file_descriptor in (1, 2):  # stdout or stderr
+                    self.stream.write('\n')
+                    record.msg = record.msg[1:]
+
+    def emit(self, record):
+        if self.HandleCR:
+            self.check_cr(record)
+        if self.HandleNL:
+            self.check_nl(record)
+        super().emit(record)
+
+    def clear_line(self, length: _Optional[int] = None):
+        """Clear the current line.
+
+        :param length: The length of the line to clear.
+        :return:
+        """
+        file_descriptor = getattr(self.stream, 'fileno', None)
+        if file_descriptor:
+            file_descriptor = file_descriptor()
+            if file_descriptor in (1, 2):
+                if length is None:
+                    length = _shutil.get_terminal_size(file_descriptor).columns
+                self.stream.write('\r' + (' ' * (length - 1)) + '\r')
+
+
+# A stream handler that supports colorizing.
+class ColorizingStreamHandler(StreamHandler):
+    """A stream handler that supports colorizing even in Windows."""
+
+    def emit(self, record):
+        try:
+            if self.HandleCR:
+                self.check_cr(record)
+            if self.HandleNL:
+                self.check_nl(record)
+            msg = self.format(record)
+            if IS_WINDOWS:
+                self.convert_and_write(msg)
+                self.convert_and_write(self.terminator)
+            else:
+                self.write(msg)
+                self.write(self.terminator)
+            self.flush()
+        except Exception:  # pylint: disable=broad-except
+            self.handleError(record)
+
+    # Writes colorized text to the Windows console.
+    def convert_and_write(self, message):
+        """Convert the message to a Windows console colorized message and write
+        it to the stream."""
+        nt_color_map = {
+            30: 0,  # foreground: black   - 0b00000000
+            31: 4,  # foreground: red     - 0b00000100
+            32: 2,  # foreground: green   - 0b00000010
+            33: 6,  # foreground: yellow  - 0b00000110
+            34: 1,  # foreground: blue    - 0b00000001
+            35: 5,  # foreground: magenta - 0b00000101
+            36: 3,  # foreground: cyan    - 0b00000011
+            37: 7,  # foreground: white   - 0b00000111
+            40: 0,  # background: black   - 0b00000000 = 0 << 4
+            41: 64,  # background: red     - 0b01000000 = 4 << 4
+            42: 32,  # background: green   - 0b00100000 = 2 << 4
+            43: 96,  # background: yellow  - 0b01100000 = 6 << 4
+            44: 16,  # background: blue    - 0b00010000 = 1 << 4
+            45: 80,  # background: magenta - 0b01010000 = 5 << 4
+            46: 48,  # background: cyan    - 0b00110000 = 3 << 4
+            47: 112,  # background: white   - 0b01110000 = 7 << 4
+            90: 8,  # foreground: gray          - 0b00001000
+            91: 12,  # foreground: light red     - 0b00001100
+            92: 10,  # foreground: light green   - 0b00001010
+            93: 14,  # foreground: light yellow  - 0b00001110
+            94: 9,  # foreground: light blue    - 0b00001001
+            95: 13,  # foreground: light magenta - 0b00001101
+            96: 11,  # foreground: light cyan    - 0b00001011
+            97: 15,  # foreground: light white   - 0b00001111
+            100: 128,  # background: gray          - 0b10000000 = 8  << 4
+            101: 192,  # background: light red     - 0b11000000 = 12 << 4
+            102: 160,  # background: light green   - 0b10100000 = 10 << 4
+            103: 224,  # background: light yellow  - 0b11100000 = 14 << 4
+            104: 144,  # background: light blue    - 0b10010000 = 9  << 4
+            105: 208,  # background: light magenta - 0b11010000 = 13 << 4
+            106: 176,  # background: light cyan    - 0b10110000 = 11 << 4
+            107: 240,  # background: light white   - 0b11110000 = 15 << 4
+            2: 8,
+            0: 7
+        }
+
+        parts = _ansi_escape.split(message)
+        win_handle = None
+        file_descriptor = getattr(self.stream, 'fileno', None)
+
+        if file_descriptor:
+            file_descriptor = file_descriptor()
+
+            if file_descriptor in (1, 2):  # stdout or stderr
+                win_handle = ctypes.windll.kernel32.GetStdHandle(-10 - file_descriptor)
+
+        while parts:
+            text = parts.pop(0)
+
+            if text:
+                self.write(text)
+
+            if parts:
+                params = parts.pop(0)
+
+                if win_handle is not None:
+                    params = [int(p) for p in params.split(';')]
+                    color = 0
+
+                    for param in params:
+                        if param in nt_color_map:
+                            color |= nt_color_map[param]
+                        else:
+                            pass  # error condition ignored
+
+                    ctypes.windll.kernel32.SetConsoleTextAttribute(win_handle, color)
+
+    # Writes the message to the console.
+    def write(self, message):
+        """Write the message to the stream."""
+        self.stream.write(message)
+        self.flush()
```

### Comparing `log21-2.8.1b0/src/log21/__init__.py` & `log21-2.9.0/src/log21/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,632 +1,633 @@
-# log21.__init__.py
-# CodeWriter21
-
-import os as _os
-import logging as _logging
-from typing import (Type as _Type, Tuple as _Tuple, Union as _Union,
-                    Mapping as _Mapping, Optional as _Optional)
-
-from log21 import CrashReporter
-from log21.Colors import (Colors, get_color, get_colors, ansi_escape, closest_color,
-                          get_color_name)
-from log21.Levels import (INFO, WARN, DEBUG, ERROR, FATAL, INPUT, NOTSET, WARNING,
-                          CRITICAL)
-from log21.Logger import Logger
-from log21.PPrint import PrettyPrinter, pformat
-from log21.Manager import Manager
-from log21.Argparse import ColorizingArgumentParser
-from log21.TreePrint import TreePrint, tree_format
-from log21.Formatters import ColorizingFormatter, DecolorizingFormatter, _Formatter
-from log21.Argumentify import argumentify
-from log21.FileHandler import FileHandler, DecolorizingFileHandler
-from log21.ProgressBar import ProgressBar
-from log21.LoggingWindow import LoggingWindow, LoggingWindowHandler
-from log21.StreamHandler import StreamHandler, ColorizingStreamHandler
-
-__version__ = "2.8.1b0"
-__author__ = "CodeWriter21 (Mehrad Pooryoussof)"
-__github__ = "Https://GitHub.com/MPCodeWriter21/log21"
-__all__ = [
-    'ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter',
-    'DecolorizingFormatter', 'get_logger', 'Logger', 'Colors', 'get_color',
-    'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN', 'INFO', 'DEBUG',
-    'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter',
-    'pformat', 'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager',
-    'get_color_name', 'closest_color', 'ansi_escape', '__version__', '__author__',
-    '__github__', 'debug', 'info', 'warning', 'warn', 'error', 'critical', 'fatal',
-    'exception', 'log', 'basic_config', 'basicConfig', 'ProgressBar', 'progress_bar',
-    'LoggingWindow', 'LoggingWindowHandler', 'get_logging_window', 'CrashReporter',
-    'console_reporter', 'file_reporter', 'argumentify'
-]
-
-_manager = Manager()
-_logging.setLoggerClass(Logger)
-
-
-def _prepare_formatter(
-    fmt: _Optional[str] = None,
-    style: str = '%',
-    datefmt: str = "%H:%M:%S",
-    show_level: bool = True,
-    show_time: bool = True,
-    colorize_time_and_level: bool = True,
-    level_names: _Optional[_Mapping[int, str]] = None,
-    level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
-    formatter_class: _Type[_logging.Formatter] = ColorizingFormatter
-):
-    # Prepares a formatting if the fmt was None
-    if not fmt:
-        style = '%'
-        fmt = "%(message)s"
-        if show_level:
-            fmt = "[%(levelname)s] " + fmt
-        if show_time:
-            fmt = "[%(asctime)s] " + fmt
-        fmt = '\r' + fmt
-
-    if level_colors and not issubclass(formatter_class, ColorizingFormatter):
-        warning(
-            '`formatter_class` should be a subclass of ColorizingFormatter when used '
-            'with level_colors.'
-        )
-        warning(
-            f'Using `{formatter_class.__name__}` might lead to unexpected behaviour!'
-        )
-
-    # Defines the formatter
-    if level_colors:
-        formatter = formatter_class(
-            fmt,
-            datefmt,
-            style=style,
-            level_colors=level_colors  # type: ignore
-        )
-    else:
-        formatter = formatter_class(fmt, datefmt, style=style)  # type: ignore
-
-    if isinstance(formatter, _Formatter) and level_names:
-        formatter.level_names = level_names
-    if not colorize_time_and_level and isinstance(formatter, ColorizingFormatter):
-        for key in formatter.level_colors:
-            formatter.level_colors[key] = tuple()
-        formatter.time_color = tuple()
-
-    return formatter
-
-
-def get_logger(
-    name: str = '',
-    level: _Union[int, str] = NOTSET,
-    show_time: bool = True,
-    show_level: bool = True,
-    colorize_time_and_level: bool = True,
-    fmt: _Optional[str] = None,
-    datefmt: str = "%H:%M:%S",
-    style: str = '%',
-    handle_carriage_return: bool = True,
-    handle_new_line: bool = True,
-    override=False,
-    level_names: _Optional[_Mapping[int, str]] = None,
-    level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
-    file: _Optional[_Union[_os.PathLike, str]] = None
-) -> Logger:
-    """Returns a logging.Logger with colorizing support. >>> >>> import log21 >>> >>> l
-    = log21.get_logger() >>> l.warning('Pretty basic, huh?') [14:49:41] [WARNING] Pretty
-    basic, huh? >>> l.critical('CONTINUE READING!! please...') [14:50:08] [CRITICAL]
-    CONTINUE READING!! please... >>> >>> my_logger =
-    log21.get_logger(name='CodeWriter21', level=log21.INFO, ... fmt='{asctime} ->
-    [{levelname}]: {message}', style='{', override=True) >>> >>> my_logger.info('FYI: My
-    name is Mehrad.') 14:56:12 -> [INFO]: FYI: My name is Mehrad. >>>
-    my_logger.error(log21.get_color('LightRed') + 'Oh no! Something went wrong D:')
-    14:56:29 -> [ERROR]: Oh no! Something went wrong D: >>> >>> my_logger.debug(1 ,2 ,3)
-    >>> # It prints Nothing because our logger level is INFO and DEBUG level is lower
-    >>> # than INFO. >>> # So let's modify the my_logger's level >>>
-    my_logger.setLevel(log21.DEBUG) >>> # Now we try again... >>> my_logger.debug(1, 2,
-    3) 14:57:34 -> [DEBUG]: 1 2 3 >>> # Well Done. Right? >>> # Let's see more >>>
-    my_logger.debug('I like %s number!', args=('21', ), end='\033[0m\n\n\n') 15:01:43 ->
-    [DEBUG]: I like 21 number!
-
-    >>> # Well, I've got a question...
-    >>> # Do you know the name of this color?
-    >>> # #888888
-    >>> # Oh ya! I can use get_color_name
-    >>> log21.get_color_name('#888888')
-    'gray'
-    >>> # Oh thank you dear!
-    >>> # Yes I knew that was grey -_- But I wanted to introduce my little friend ☺
-    >>> # See you soon!
-    >>>
-
-    :param name: Optional[str]: The name of the logger
-    :param level: Union[int, str] = logging.NOTSET: The logging level of the logger
-    :param show_time: bool = True: Show the time in the log
-    :param show_level: bool = True: Show the level of logging in the log
-    :param fmt: Optional[str]: Custom formatting for the logger - overrides the default
-        (show_time & show_level)
-    :param datefmt: str = "%H:%M:%S": Custom date-time formatting for the logger
-    :param style: str = '%': Use a style parameter of '%', '{' or '$' to specify that
-        you want to use one of %-formatting, :meth:`str.format` (``{}``) formatting or
-        :class:`string.Template` formatting in your format string.
-    :param colorize_time_and_level: bool = True: Colorizes the time and level using the
-        default colors
-    :param handle_carriage_return: bool = True: Adds a line of space characters to
-        remove any text before the CR
-    :param handle_new_line: bool = True: Places the NewLine characters at the beginning
-        of the text before everything else
-    :param override: bool = True: Overrides the logger attributes even if it already
-        exists.
-    :param level_names: Mapping[int, str] = None: You can specify custom level names.
-    :param level_colors: Mapping[int, Tuple[str, ...]] = None: You can specify custom
-        level colors.
-    :param file: Union[os.PathLike, str] = None: The file to log to
-    :return: log21.Logger
-    """
-    if not isinstance(name, str):
-        raise TypeError('A logger name must be a string')
-    logger = None
-    if name:
-        logger = _manager.getLogger(name)
-    if (not logger) or override:
-        logger = Logger(name, level)
-        formatter = _prepare_formatter(
-            fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
-            level_names, level_colors
-        )
-
-        # Defines the handler
-        handler = ColorizingStreamHandler(
-            handle_carriage_return=handle_carriage_return,
-            handle_new_line=handle_new_line
-        )
-        handler.setFormatter(formatter)
-        logger.addHandler(handler)
-        if level_names:
-            logger.add_levels(level_names, errors='ignore')
-        _manager.addLogger(name, logger)
-
-        if file:
-            file_handler = FileHandler(file)
-            file_formatter = _prepare_formatter(
-                fmt,
-                style,
-                datefmt,
-                show_level,
-                show_time,
-                False,
-                level_names,
-                formatter_class=DecolorizingFormatter
-            )
-            file_handler.setFormatter(file_formatter)
-            logger.addHandler(file_handler)
-
-    return logger
-
-
-def get_logging_window(
-    name: str = '',
-    level: _Union[int, str] = NOTSET,
-    show_time: bool = True,
-    show_level: bool = True,
-    colorize_time_and_level: bool = True,
-    fmt: _Optional[str] = None,
-    datefmt: str = "%H:%M:%S",
-    style: str = '%',
-    handle_carriage_return: bool = True,
-    handle_new_line: bool = True,
-    override=False,
-    level_names: _Optional[_Mapping[int, str]] = None,
-    width: int = 80,
-    height: int = 20,
-    allow_shell: bool = False
-) -> LoggingWindow:
-    """Returns a logging window.
-
-    >>> # Let's see how it works
-    >>> # Imports log21 and time modules
-    >>> import log21, time
-    >>> # Creates a new LoggingWindow object
-    >>> window = log21.get_logging_window('Test Window')
-    >>> # Now use it without any additional steps to add handlers and formatters!
-    >>> # It works just like a normal logger but with some extra features
-    >>>
-    >>> window.info('This works properly!')
-    >>>
-    >>> # You can use HEX colors as well as the ANSI colors which are supported by
-    >>> # normal loggers
-    >>> # ANSI colors usage:
-    >>> window.info('This is a \033[91mred\033[0m message.')
-    >>> window.info('\033[102mThis is a message with green background.')
-    >>> # HEX colors usage:
-    >>> window.info('\033#00FFFFhfThis is a message with cyan foreground.')
-    >>> window.info('\033#0000FFhbThis is a message with blue background.')
-    >>>
-    >>> # Progressbar usage:
-    >>> for i in range(100):
-    ...     window.print_progress(i + 1, 100)
-    ...     time.sleep(0.1)
-    ...
-    >>>
-    >>> # Gettig input from the user:
-    >>> name: str = window.input('Enter your name: ')
-    >>> window.print('Hello, ' + name + '!')
-    >>> # Run these lines to see the messages in the window
-    >>>
-
-    :param name: Optional[str]: The name of the logger
-    :param level: Union[int, str] = logging.NOTSET: The logging level of the logger
-    :param show_time: bool = True: Show the time in the log
-    :param show_level: bool = True: Show the level of logging in the log
-    :param fmt: Optional[str]: Custom formatting for the logger - overrides the default
-        (show_time & show_level)
-    :param datefmt: str = "%H:%M:%S": Custom date-time formatting for the logger
-    :param style: str = '%': Use a style parameter of '%', '{' or '$' to specify that
-        you want to use one of %-formatting, :meth:`str.format` (``{}``) formatting or
-        :class:`string.Template` formatting in your format string.
-    :param colorize_time_and_level: bool = True: Colorizes the time and level using the
-        default colors
-    :param handle_carriage_return: bool = True: Adds a line of space characters to
-        remove any text before the CR
-    :param handle_new_line: bool = True: Places the NewLine characters at the beginning
-        of the text before everything else
-    :param override: bool = True: Overrides the logger attributes even if it already
-        exists
-    :param level_names: Mapping[int, str] = None: You can specify custom level names.
-    :param width: int = 80: The width of the window
-    :param height: int = 20: The height of the window
-    :param allow_shell: bool = False: Allow the user to use the shell
-    :return: log21.LoggingWindow
-    """
-    if not isinstance(name, str):
-        raise TypeError('A logger name must be a string')
-    logging_window = None
-    if name:
-        logging_window = _manager.getLogger(name)
-    if (not logging_window) or override:
-        logging_window = LoggingWindow(
-            name, level=level, width=width, height=height, allow_shell=allow_shell
-        )
-        formatter = _prepare_formatter(
-            fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
-            level_names
-        )
-
-        # Defines the handler
-        handler = LoggingWindowHandler(
-            logging_window,
-            handle_carriage_return=handle_carriage_return,
-            handle_new_line=handle_new_line
-        )
-        handler.setFormatter(formatter)
-        logging_window.addHandler(handler)
-        _manager.addLogger(name, logging_window)
-    return logging_window
-
-
-getLogger = get_logger
-
-
-def print(  # pylint: disable=redefined-builtin
-    *msg,
-    args: tuple = (),
-    end='\033[0m\n',
-    **kwargs
-):
-    """Works like the print function but ANSI colors are supported (even on Windows) and
-    it ends with a new line and a reset color by default."""
-    logger = get_logger('log21.print', level=DEBUG, show_time=False, show_level=False)
-    logger.print(*msg, args=args, end=end, **kwargs)
-
-
-def input(  # pylint: disable=redefined-builtin
-    *msg,
-    args: tuple = (),
-    end='',
-    **kwargs
-):
-    """Works like the input function but ANSI colors are supported (even on Windows)."""
-    logger = get_logger('log21.input', level=DEBUG, show_time=False, show_level=False)
-    return logger.input(*msg, args=args, end=end, **kwargs)
-
-
-def getpass(*msg, args: tuple = (), end='', **kwargs):
-    """Works like the getpass.getpass function but ANSI colors are supported (even on
-    Windows)."""
-    logger = get_logger('log21.getpass', level=DEBUG, show_time=False, show_level=False)
-    return logger.getpass(*msg, args=args, end=end, **kwargs)
-
-
-def pprint(
-    obj,
-    indent=1,
-    width=80,
-    depth=None,
-    signs_colors: _Optional[_Mapping[str, str]] = None,
-    *,
-    sort_dicts=True,
-    underscore_numbers=False,
-    compact=False,
-    end='\033[0m\n',
-    **kwargs
-):
-    """A colorful version of the pprint.pprint function.
-
-    :param obj: The object to print.
-    :param indent: The amount of indentation to use.
-    :param width: The maximum width in characters of the output.
-    :param depth: The maximum depth to print nested structures. None means unlimited.
-    :param signs_colors: A mapping that lets you specify the colors of the supported
-        signs.
-    :param sort_dicts: If True, dictionaries are sorted by key.
-    :param underscore_numbers: If True, numbers are printed with an underscore between
-        each group of three digits.
-    :param compact: If True, lists and tuples are displayed on a single line.
-    :param end: The string to append at the end of the output.
-    :param kwargs: Additional keyword arguments passed to the Logger.print function.
-    """
-    logger = get_logger('log21.pprint', level=DEBUG, show_time=False, show_level=False)
-    logger.print(
-        pformat(
-            obj=obj,
-            indent=indent,
-            width=width,
-            depth=depth,
-            signs_colors=signs_colors,
-            compact=compact,
-            sort_dicts=sort_dicts,
-            underscore_numbers=underscore_numbers
-        ),
-        end=end,
-        **kwargs
-    )
-
-
-pretty_print = pprint
-
-
-def tree_print(
-    obj,
-    indent: int = 4,
-    mode='-',
-    colors: _Optional[_Mapping[str, str]] = None,
-    end='\033[0m\n',
-    **kwargs
-):
-    """Prints a tree representation of the given object. (e.g. a dictionary)
-
-    :param obj: The object to print.
-    :param indent: The number of spaces to indent each level.
-    :param mode: The mode to use for the tree. Can be '-' or '='.
-    :param colors: A mapping that lets you customize the colors of branches and fruits.
-    :param end: The string to append at the end of the output.
-    :param kwargs: Additional keyword arguments passed to the Logger.print function.
-    """
-    logger = get_logger(
-        'log21.tree_print', level=DEBUG, show_time=False, show_level=False
-    )
-    logger.print(
-        tree_format(obj, indent=indent, mode=mode, colors=colors), end=end, **kwargs
-    )
-
-
-tprint = tree_print
-
-root = Logger('root-logger', INFO)
-
-
-def basic_config(
-    force: bool = False,
-    encoding: _Optional[str] = None,
-    errors: _Optional[str] = 'backslashreplace',
-    handlers=None,
-    stream=None,
-    filename=None,
-    filemode: str = 'a',
-    date_format: str = "%H:%M:%S",
-    style: str = '%',
-    format_: _Optional[str] = None,
-    level: _Optional[_Union[int, str]] = None
-):  # pylint: disable=too-many-branches
-    """Do basic configuration for the logging system.
-
-    This function does nothing if the root logger already has handlers
-    configured, unless the keyword argument *force* is set to ``True``.
-    It is a convenience method intended for use by simple scripts
-    to do one-shot configuration of the logging package.
-
-    The default behaviour is to create a ColorizingStreamHandler which writes to
-    sys.stderr, set a formatter using the BASIC_FORMAT format string, and
-    add the handler to the root logger.
-
-    A number of optional keyword arguments may be specified, which can alter
-    the default behaviour.
-
-    filename  Specifies that a FileHandler be created, using the specified
-              filename, rather than a StreamHandler.
-    filemode  Specifies the mode to open the file, if filename is specified
-              (if filemode is unspecified, it defaults to 'a').
-    format    Use the specified format string for the handler.
-    datefmt   Use the specified date/time format.
-    style     If a format string is specified, use this to specify the
-              type of format string (possible values '%', '{', '$', for
-              %-formatting, :meth:`str.format` and :class:`string.Template`
-              - defaults to '%').
-    level     Set the root logger level to the specified level.
-    stream    Use the specified stream to initialize the StreamHandler. Note
-              that this argument is incompatible with 'filename' - if both
-              are present, 'stream' is ignored.
-    handlers  If specified, this should be an iterable of already created
-              handlers, which will be added to the root handler. Any handler
-              in the list which does not have a formatter assigned will be
-              assigned the formatter created in this function.
-    force     If this keyword  is specified as true, any existing handlers
-              attached to the root logger are removed and closed, before
-              carrying out the configuration as specified by the other
-              arguments.
-    encoding  If specified together with a filename, this encoding is passed to
-              the created FileHandler, causing it to be used when the file is
-              opened.
-    errors    If specified together with a filename, this value is passed to the
-              created FileHandler, causing it to be used when the file is
-              opened in text mode. If not specified, the default value is
-              `backslashreplace`.
-
-    Note that you could specify a stream created using open(filename, mode)
-    rather than passing the filename and mode in. However, it should be
-    remembered that StreamHandler does not close its stream (since it may be
-    using sys.stdout or sys.stderr), whereas FileHandler closes its stream
-    when the handler is closed.
-    """
-    if force:
-        for handler in root.handlers[:]:
-            root.removeHandler(handler)
-            handler.close()
-    if len(root.handlers) == 0:
-        if handlers is None:
-            if stream and filename:
-                raise ValueError(
-                    "'stream' and 'filename' should not be specified together"
-                )
-        else:
-            if stream or filename:
-                raise ValueError(
-                    "'stream' or 'filename' should not be specified together with "
-                    "'handlers'"
-                )
-        if handlers is None:
-            if filename:
-                if 'b' in filemode:
-                    errors = None
-                else:
-                    encoding = encoding or 'utf-8'
-                handler = DecolorizingFileHandler(
-                    filename, filemode, encoding=encoding, errors=errors
-                )
-            else:
-                handler = ColorizingStreamHandler(stream=stream)
-            handlers = [handler]
-        if style not in '%{$':
-            raise ValueError('Style must be one of: %, {, $')
-        if not format_:
-            format_ = {
-                '%': '[%(asctime)s] [%(levelname)s] %(message)s',
-                '{': '[{asctime}] [{levelname}] {message}',
-                '$': '[${asctime}] [${levelname}] ${message}'
-            }[style]
-        formatter = ColorizingFormatter(format_, date_format, style=style)
-        for handler in handlers:
-            if handler.formatter is None:
-                handler.setFormatter(formatter)
-            root.addHandler(handler)
-    if level is not None:
-        root.setLevel(level)
-
-
-basicConfig = basic_config
-
-
-def critical(*msg, args=(), **kwargs):
-    """Log a message with severity 'CRITICAL' on the root logger.
-
-    If the logger has no handlers, call basicConfig() to add a console handler with a
-    pre-defined format.
-    """
-    if len(root.handlers) == 0:
-        basic_config()
-    root.critical(*msg, args=args, **kwargs)
-
-
-def fatal(*msg, args=(), **kwargs):
-    """Don't use this function, use critical() instead."""
-    critical(*msg, args=args, **kwargs)
-
-
-def error(*msg, args=(), **kwargs):
-    """Log a message with severity 'ERROR' on the root logger.
-
-    If the logger has no handlers, call basicConfig() to add a console handler with a
-    pre-defined format.
-    """
-    if len(root.handlers) == 0:
-        basic_config()
-    root.error(*msg, args=args, **kwargs)
-
-
-def exception(*msg, args=(), exc_info=True, **kwargs):
-    """Log a message with severity 'ERROR' on the root logger, with exception
-    information.
-
-    If the logger has no handlers, basicConfig() is called to add a console handler with
-    a pre-defined format.
-    """
-    error(*msg, args=args, exc_info=exc_info, **kwargs)
-
-
-def warning(*msg, args=(), **kwargs):
-    """Log a message with severity 'WARNING' on the root logger.
-
-    If the logger has no handlers, call basicConfig() to add a console handler with a
-    pre-defined format.
-    """
-    if len(root.handlers) == 0:
-        basic_config()
-    root.warning(*msg, args=args, **kwargs)
-
-
-def warn(*msg, args=(), **kwargs):
-    """An alias of warning()"""
-    warning(*msg, args=args, **kwargs)
-
-
-def info(*msg, args=(), **kwargs):
-    """Log a message with severity 'INFO' on the root logger.
-
-    If the logger has no handlers, call basicConfig() to add a console handler with a
-    pre-defined format.
-    """
-    if len(root.handlers) == 0:
-        basic_config()
-    root.info(*msg, args=args, **kwargs)
-
-
-def debug(*msg, args=(), **kwargs):
-    """Log a message with severity 'DEBUG' on the root logger.
-
-    If the logger has no handlers, call basicConfig() to add a console handler with a
-    pre-defined format.
-    """
-    if len(root.handlers) == 0:
-        basic_config()
-    root.debug(*msg, args=args, **kwargs)
-
-
-def log(level, *msg, args=(), **kwargs):
-    """Log 'msg % args' with the integer severity 'level' on the root logger.
-
-    If the logger has no handlers, call basicConfig() to add a console handler with a
-    pre-defined format.
-    """
-    if len(root.handlers) == 0:
-        basic_config()
-    root.log(level, *msg, args=args, **kwargs)
-
-
-def progress_bar(
-    progress: float,
-    total: float,
-    width: _Optional[int] = None,
-    prefix: str = '|',
-    suffix: str = '|',
-    show_percentage: bool = True
-):
-    """Print a progress bar to the console."""
-
-    progress_bar_ = ProgressBar(
-        width=width, prefix=prefix, suffix=suffix, show_percentage=show_percentage
-    )
-
-    print(progress_bar_.get_bar(progress, total))
-
-
-console_reporter = CrashReporter.ConsoleReporter()
-
-file_reporter = CrashReporter.FileReporter(file='.crash_report.log')
+# log21.__init__.py
+# CodeWriter21
+
+import os as _os
+import logging as _logging
+from typing import (Type as _Type, Tuple as _Tuple, Union as _Union,
+                    Mapping as _Mapping, Optional as _Optional)
+
+from . import CrashReporter
+from .Colors import (Colors, get_color, get_colors, ansi_escape, closest_color,
+                     get_color_name)
+from .Levels import INFO, WARN, DEBUG, ERROR, FATAL, INPUT, NOTSET, WARNING, CRITICAL
+from .Logger import Logger
+from .PPrint import PrettyPrinter, pformat
+from .Manager import Manager
+from .Argparse import ColorizingArgumentParser
+from .TreePrint import TreePrint, tree_format
+from .Formatters import ColorizingFormatter, DecolorizingFormatter, _Formatter
+from .Argumentify import argumentify
+from .FileHandler import FileHandler, DecolorizingFileHandler
+from .ProgressBar import ProgressBar
+from .LoggingWindow import LoggingWindow, LoggingWindowHandler
+from .StreamHandler import StreamHandler, ColorizingStreamHandler
+
+__author__ = 'CodeWriter21 (Mehrad Pooryoussof)'
+__version__ = '2.9.0'
+__github__ = 'Https://GitHub.com/MPCodeWriter21/log21'
+__all__ = [
+    'ColorizingStreamHandler', 'DecolorizingFileHandler', 'ColorizingFormatter',
+    'DecolorizingFormatter', 'get_logger', 'Logger', 'Colors', 'get_color',
+    'get_colors', 'CRITICAL', 'FATAL', 'ERROR', 'WARNING', 'WARN', 'INFO', 'DEBUG',
+    'NOTSET', 'INPUT', 'StreamHandler', 'ColorizingArgumentParser', 'PrettyPrinter',
+    'pformat', 'pprint', 'pretty_print', 'tree_format', 'TreePrint', 'Manager',
+    'get_color_name', 'closest_color', 'ansi_escape', '__author__', '__github__',
+    'debug', 'info', 'warning', 'warn', 'error', 'critical', 'fatal', 'exception',
+    'log', 'basic_config', 'basicConfig', 'ProgressBar', 'progress_bar',
+    'LoggingWindow', 'LoggingWindowHandler', 'get_logging_window', 'CrashReporter',
+    'console_reporter', 'file_reporter', 'argumentify'
+]
+
+_manager = Manager()
+_logging.setLoggerClass(Logger)
+
+
+def _prepare_formatter(
+    fmt: _Optional[str] = None,
+    style: str = '%',
+    datefmt: str = '%H:%M:%S',
+    show_level: bool = True,
+    show_time: bool = True,
+    colorize_time_and_level: bool = True,
+    level_names: _Optional[_Mapping[int, str]] = None,
+    level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
+    formatter_class: _Type[_logging.Formatter] = ColorizingFormatter
+):
+    # Prepares a formatting if the fmt was None
+    if not fmt:
+        style = '%'
+        fmt = '%(message)s'
+        if show_level:
+            fmt = '[%(levelname)s] ' + fmt
+        if show_time:
+            fmt = '[%(asctime)s] ' + fmt
+        fmt = '\r' + fmt
+
+    if level_colors and not issubclass(formatter_class, ColorizingFormatter):
+        warning(
+            '`formatter_class` should be a subclass of ColorizingFormatter when used '
+            'with level_colors.'
+        )
+        warning(
+            f'Using `{formatter_class.__name__}` might lead to unexpected behaviour!'
+        )
+
+    # Defines the formatter
+    if level_colors:
+        formatter = formatter_class(
+            fmt,
+            datefmt,
+            style=style,
+            level_colors=level_colors  # type: ignore
+        )
+    else:
+        formatter = formatter_class(fmt, datefmt, style=style)  # type: ignore
+
+    if isinstance(formatter, _Formatter) and level_names:
+        formatter.level_names = level_names
+    if not colorize_time_and_level and isinstance(formatter, ColorizingFormatter):
+        for key in formatter.level_colors:
+            formatter.level_colors[key] = tuple()
+        formatter.time_color = tuple()
+
+    return formatter
+
+
+def get_logger(
+    name: str = '',
+    level: _Union[int, str] = NOTSET,
+    show_time: bool = True,
+    show_level: bool = True,
+    colorize_time_and_level: bool = True,
+    fmt: _Optional[str] = None,
+    datefmt: str = '%H:%M:%S',
+    style: str = '%',
+    handle_carriage_return: bool = True,
+    handle_new_line: bool = True,
+    override=False,
+    level_names: _Optional[_Mapping[int, str]] = None,
+    level_colors: _Optional[_Mapping[int, _Tuple[str, ...]]] = None,
+    file: _Optional[_Union[_os.PathLike, str]] = None
+) -> Logger:
+    """Returns a logging.Logger with colorizing support. >>> >>> import log21 >>> >>> l
+    = log21.get_logger() >>> l.warning('Pretty basic, huh?') [14:49:41] [WARNING] Pretty
+    basic, huh? >>> l.critical('CONTINUE READING!! please...') [14:50:08] [CRITICAL]
+    CONTINUE READING!! please... >>> >>> my_logger =
+    log21.get_logger(name='CodeWriter21', level=log21.INFO, ... fmt='{asctime} ->
+    [{levelname}]: {message}', style='{', override=True) >>> >>> my_logger.info('FYI: My
+    name is Mehrad.') 14:56:12 -> [INFO]: FYI: My name is Mehrad. >>>
+    my_logger.error(log21.get_color('LightRed') + 'Oh no! Something went wrong D:')
+    14:56:29 -> [ERROR]: Oh no! Something went wrong D: >>> >>> my_logger.debug(1 ,2 ,3)
+    >>> # It prints Nothing because our logger level is INFO and DEBUG level is lower
+    >>> # than INFO. >>> # So let's modify the my_logger's level >>>
+    my_logger.setLevel(log21.DEBUG) >>> # Now we try again... >>> my_logger.debug(1, 2,
+    3) 14:57:34 -> [DEBUG]: 1 2 3 >>> # Well Done. Right? >>> # Let's see more >>>
+    my_logger.debug('I like %s number!', args=('21', ), end='\033[0m\n\n\n') 15:01:43 ->
+    [DEBUG]: I like 21 number!
+
+    >>> # Well, I've got a question...
+    >>> # Do you know the name of this color?
+    >>> # #888888
+    >>> # Oh ya! I can use get_color_name
+    >>> log21.get_color_name('#888888')
+    'gray'
+    >>> # Oh thank you dear!
+    >>> # Yes I knew that was grey -_- But I wanted to introduce my little friend ☺
+    >>> # See you soon!
+    >>>
+
+    :param name: Optional[str]: The name of the logger
+    :param level: Union[int, str] = logging.NOTSET: The logging level of the logger
+    :param show_time: bool = True: Show the time in the log
+    :param show_level: bool = True: Show the level of logging in the log
+    :param fmt: Optional[str]: Custom formatting for the logger - overrides the default
+        (show_time & show_level)
+    :param datefmt: str = "%H:%M:%S": Custom date-time formatting for the logger
+    :param style: str = '%': Use a style parameter of '%', '{' or '$' to specify that
+        you want to use one of %-formatting, :meth:`str.format` (``{}``) formatting or
+        :class:`string.Template` formatting in your format string.
+    :param colorize_time_and_level: bool = True: Colorizes the time and level using the
+        default colors
+    :param handle_carriage_return: bool = True: Adds a line of space characters to
+        remove any text before the CR
+    :param handle_new_line: bool = True: Places the NewLine characters at the beginning
+        of the text before everything else
+    :param override: bool = True: Overrides the logger attributes even if it already
+        exists.
+    :param level_names: Mapping[int, str] = None: You can specify custom level names.
+    :param level_colors: Mapping[int, Tuple[str, ...]] = None: You can specify custom
+        level colors.
+    :param file: Union[os.PathLike, str] = None: The file to log to
+    :return: log21.Logger
+    """
+    if not isinstance(name, str):
+        raise TypeError('A logger name must be a string')
+    logger = None
+    if name:
+        logger = _manager.getLogger(name)
+    if (not logger) or override:
+        logger = Logger(name, level)
+        formatter = _prepare_formatter(
+            fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
+            level_names, level_colors
+        )
+
+        # Defines the handler
+        handler = ColorizingStreamHandler(
+            handle_carriage_return=handle_carriage_return,
+            handle_new_line=handle_new_line
+        )
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
+        if level_names:
+            logger.add_levels(level_names, errors='ignore')
+        _manager.addLogger(name, logger)
+
+        if file:
+            file_handler = FileHandler(file)
+            file_formatter = _prepare_formatter(
+                fmt,
+                style,
+                datefmt,
+                show_level,
+                show_time,
+                False,
+                level_names,
+                formatter_class=DecolorizingFormatter
+            )
+            file_handler.setFormatter(file_formatter)
+            logger.addHandler(file_handler)
+
+    return logger
+
+
+def get_logging_window(
+    name: str = '',
+    level: _Union[int, str] = NOTSET,
+    show_time: bool = True,
+    show_level: bool = True,
+    colorize_time_and_level: bool = True,
+    fmt: _Optional[str] = None,
+    datefmt: str = '%H:%M:%S',
+    style: str = '%',
+    handle_carriage_return: bool = True,
+    handle_new_line: bool = True,
+    override=False,
+    level_names: _Optional[_Mapping[int, str]] = None,
+    width: int = 80,
+    height: int = 20,
+    allow_shell: bool = False
+) -> LoggingWindow:
+    """Returns a logging window.
+
+    >>> # Let's see how it works
+    >>> # Imports log21 and time modules
+    >>> import log21, time
+    >>> # Creates a new LoggingWindow object
+    >>> window = log21.get_logging_window('Test Window')
+    >>> # Now use it without any additional steps to add handlers and formatters!
+    >>> # It works just like a normal logger but with some extra features
+    >>>
+    >>> window.info('This works properly!')
+    >>>
+    >>> # You can use HEX colors as well as the ANSI colors which are supported by
+    >>> # normal loggers
+    >>> # ANSI colors usage:
+    >>> window.info('This is a \033[91mred\033[0m message.')
+    >>> window.info('\033[102mThis is a message with green background.')
+    >>> # HEX colors usage:
+    >>> window.info('\033#00FFFFhfThis is a message with cyan foreground.')
+    >>> window.info('\033#0000FFhbThis is a message with blue background.')
+    >>>
+    >>> # Progressbar usage:
+    >>> for i in range(100):
+    ...     window.print_progress(i + 1, 100)
+    ...     time.sleep(0.1)
+    ...
+    >>>
+    >>> # Gettig input from the user:
+    >>> name: str = window.input('Enter your name: ')
+    >>> window.print('Hello, ' + name + '!')
+    >>> # Run these lines to see the messages in the window
+    >>>
+
+    :param name: Optional[str]: The name of the logger
+    :param level: Union[int, str] = logging.NOTSET: The logging level of the logger
+    :param show_time: bool = True: Show the time in the log
+    :param show_level: bool = True: Show the level of logging in the log
+    :param fmt: Optional[str]: Custom formatting for the logger - overrides the default
+        (show_time & show_level)
+    :param datefmt: str = "%H:%M:%S": Custom date-time formatting for the logger
+    :param style: str = '%': Use a style parameter of '%', '{' or '$' to specify that
+        you want to use one of %-formatting, :meth:`str.format` (``{}``) formatting or
+        :class:`string.Template` formatting in your format string.
+    :param colorize_time_and_level: bool = True: Colorizes the time and level using the
+        default colors
+    :param handle_carriage_return: bool = True: Adds a line of space characters to
+        remove any text before the CR
+    :param handle_new_line: bool = True: Places the NewLine characters at the beginning
+        of the text before everything else
+    :param override: bool = True: Overrides the logger attributes even if it already
+        exists
+    :param level_names: Mapping[int, str] = None: You can specify custom level names.
+    :param width: int = 80: The width of the window
+    :param height: int = 20: The height of the window
+    :param allow_shell: bool = False: Allow the user to use the shell
+    :return: log21.LoggingWindow
+    """
+    if not isinstance(name, str):
+        raise TypeError('A logger name must be a string')
+    logging_window = None
+    if name:
+        logging_window = _manager.getLogger(name)
+    if (not logging_window) or override:
+        logging_window = LoggingWindow(
+            name, level=level, width=width, height=height, allow_shell=allow_shell
+        )
+        formatter = _prepare_formatter(
+            fmt, style, datefmt, show_level, show_time, colorize_time_and_level,
+            level_names
+        )
+
+        # Defines the handler
+        handler = LoggingWindowHandler(
+            logging_window,
+            handle_carriage_return=handle_carriage_return,
+            handle_new_line=handle_new_line
+        )
+        handler.setFormatter(formatter)
+        logging_window.addHandler(handler)
+        _manager.addLogger(name, logging_window)
+    return logging_window
+
+
+getLogger = get_logger
+
+
+def print(  # pylint: disable=redefined-builtin
+    *msg,
+    args: tuple = (),
+    end='\033[0m\n',
+    **kwargs
+):
+    """Works like the print function but ANSI colors are supported (even on Windows) and
+    it ends with a new line and a reset color by default."""
+    logger = get_logger('log21.print', level=DEBUG, show_time=False, show_level=False)
+    logger.print(*msg, args=args, end=end, **kwargs)
+
+
+def input(  # pylint: disable=redefined-builtin
+    *msg,
+    args: tuple = (),
+    end='',
+    **kwargs
+):
+    """Works like the input function but ANSI colors are supported (even on Windows)."""
+    logger = get_logger('log21.input', level=DEBUG, show_time=False, show_level=False)
+    return logger.input(*msg, args=args, end=end, **kwargs)
+
+
+def getpass(*msg, args: tuple = (), end='', **kwargs):
+    """Works like the getpass.getpass function but ANSI colors are supported (even on
+    Windows)."""
+    logger = get_logger('log21.getpass', level=DEBUG, show_time=False, show_level=False)
+    return logger.getpass(*msg, args=args, end=end, **kwargs)
+
+
+def pprint(
+    obj,
+    indent=1,
+    width=80,
+    depth=None,
+    signs_colors: _Optional[_Mapping[str, str]] = None,
+    *,
+    sort_dicts=True,
+    underscore_numbers=False,
+    compact=False,
+    end='\033[0m\n',
+    **kwargs
+):
+    """A colorful version of the pprint.pprint function.
+
+    :param obj: The object to print.
+    :param indent: The amount of indentation to use.
+    :param width: The maximum width in characters of the output.
+    :param depth: The maximum depth to print nested structures. None means unlimited.
+    :param signs_colors: A mapping that lets you specify the colors of the supported
+        signs.
+    :param sort_dicts: If True, dictionaries are sorted by key.
+    :param underscore_numbers: If True, numbers are printed with an underscore between
+        each group of three digits.
+    :param compact: If True, lists and tuples are displayed on a single line.
+    :param end: The string to append at the end of the output.
+    :param kwargs: Additional keyword arguments passed to the Logger.print function.
+    """
+    logger = get_logger('log21.pprint', level=DEBUG, show_time=False, show_level=False)
+    logger.print(
+        pformat(
+            obj=obj,
+            indent=indent,
+            width=width,
+            depth=depth,
+            signs_colors=signs_colors,
+            compact=compact,
+            sort_dicts=sort_dicts,
+            underscore_numbers=underscore_numbers
+        ),
+        end=end,
+        **kwargs
+    )
+
+
+pretty_print = pprint
+
+
+def tree_print(
+    obj,
+    indent: int = 4,
+    mode='-',
+    colors: _Optional[_Mapping[str, str]] = None,
+    end='\033[0m\n',
+    **kwargs
+):
+    """Prints a tree representation of the given object. (e.g. a dictionary)
+
+    :param obj: The object to print.
+    :param indent: The number of spaces to indent each level.
+    :param mode: The mode to use for the tree. Can be '-' or '='.
+    :param colors: A mapping that lets you customize the colors of branches and fruits.
+    :param end: The string to append at the end of the output.
+    :param kwargs: Additional keyword arguments passed to the Logger.print function.
+    """
+    logger = get_logger(
+        'log21.tree_print', level=DEBUG, show_time=False, show_level=False
+    )
+    logger.print(
+        tree_format(obj, indent=indent, mode=mode, colors=colors), end=end, **kwargs
+    )
+
+
+tprint = tree_print
+
+root = Logger('root-logger', INFO)
+
+
+def basic_config(
+    force: bool = False,
+    encoding: _Optional[str] = None,
+    errors: _Optional[str] = 'backslashreplace',
+    handlers=None,
+    stream=None,
+    filename=None,
+    filemode: str = 'a',
+    date_format: str = '%H:%M:%S',
+    style: str = '%',
+    format_: _Optional[str] = None,
+    level: _Optional[_Union[int, str]] = None
+):  # pylint: disable=too-many-branches
+    """Do basic configuration for the logging system.
+
+    This function does nothing if the root logger already has handlers
+    configured, unless the keyword argument *force* is set to ``True``.
+    It is a convenience method intended for use by simple scripts
+    to do one-shot configuration of the logging package.
+
+    The default behaviour is to create a ColorizingStreamHandler which writes to
+    sys.stderr, set a formatter using the BASIC_FORMAT format string, and
+    add the handler to the root logger.
+
+    A number of optional keyword arguments may be specified, which can alter
+    the default behaviour.
+
+    filename  Specifies that a FileHandler be created, using the specified
+              filename, rather than a StreamHandler.
+    filemode  Specifies the mode to open the file, if filename is specified
+              (if filemode is unspecified, it defaults to 'a').
+    format    Use the specified format string for the handler.
+    datefmt   Use the specified date/time format.
+    style     If a format string is specified, use this to specify the
+              type of format string (possible values '%', '{', '$', for
+              %-formatting, :meth:`str.format` and :class:`string.Template`
+              - defaults to '%').
+    level     Set the root logger level to the specified level.
+    stream    Use the specified stream to initialize the StreamHandler. Note
+              that this argument is incompatible with 'filename' - if both
+              are present, 'stream' is ignored.
+    handlers  If specified, this should be an iterable of already created
+              handlers, which will be added to the root handler. Any handler
+              in the list which does not have a formatter assigned will be
+              assigned the formatter created in this function.
+    force     If this keyword  is specified as true, any existing handlers
+              attached to the root logger are removed and closed, before
+              carrying out the configuration as specified by the other
+              arguments.
+    encoding  If specified together with a filename, this encoding is passed to
+              the created FileHandler, causing it to be used when the file is
+              opened.
+    errors    If specified together with a filename, this value is passed to the
+              created FileHandler, causing it to be used when the file is
+              opened in text mode. If not specified, the default value is
+              `backslashreplace`.
+
+    Note that you could specify a stream created using open(filename, mode)
+    rather than passing the filename and mode in. However, it should be
+    remembered that StreamHandler does not close its stream (since it may be
+    using sys.stdout or sys.stderr), whereas FileHandler closes its stream
+    when the handler is closed.
+    """
+    if force:
+        for handler in root.handlers[:]:
+            root.removeHandler(handler)
+            handler.close()
+    if len(root.handlers) == 0:
+        if handlers is None:
+            if stream and filename:
+                raise ValueError(
+                    "'stream' and 'filename' should not be specified together"
+                )
+        else:
+            if stream or filename:
+                raise ValueError(
+                    "'stream' or 'filename' should not be specified together with "
+                    "'handlers'"
+                )
+        if handlers is None:
+            if filename:
+                if 'b' in filemode:
+                    errors = None
+                else:
+                    encoding = encoding or 'utf-8'
+                handler = DecolorizingFileHandler(
+                    filename, filemode, encoding=encoding, errors=errors
+                )
+            else:
+                handler = ColorizingStreamHandler(stream=stream)
+            handlers = [handler]
+        if style not in '%{$':
+            raise ValueError('Style must be one of: %, {, $')
+        if not format_:
+            format_ = {
+                '%': '[%(asctime)s] [%(levelname)s] %(message)s',
+                '{': '[{asctime}] [{levelname}] {message}',
+                '$': '[${asctime}] [${levelname}] ${message}'
+            }[style]
+        formatter = ColorizingFormatter(format_, date_format, style=style)
+        for handler in handlers:
+            if handler.formatter is None:
+                handler.setFormatter(formatter)
+            root.addHandler(handler)
+    if level is not None:
+        root.setLevel(level)
+
+
+basicConfig = basic_config
+
+
+def critical(*msg, args=(), **kwargs):
+    """Log a message with severity 'CRITICAL' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console handler with a
+    pre-defined format.
+    """
+    if len(root.handlers) == 0:
+        basic_config()
+    root.critical(*msg, args=args, **kwargs)
+
+
+def fatal(*msg, args=(), **kwargs):
+    """Don't use this function, use critical() instead."""
+    critical(*msg, args=args, **kwargs)
+
+
+def error(*msg, args=(), **kwargs):
+    """Log a message with severity 'ERROR' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console handler with a
+    pre-defined format.
+    """
+    if len(root.handlers) == 0:
+        basic_config()
+    root.error(*msg, args=args, **kwargs)
+
+
+def exception(*msg, args=(), exc_info=True, **kwargs):
+    """Log a message with severity 'ERROR' on the root logger, with exception
+    information.
+
+    If the logger has no handlers, basicConfig() is called to add a console handler with
+    a pre-defined format.
+    """
+    error(*msg, args=args, exc_info=exc_info, **kwargs)
+
+
+def warning(*msg, args=(), **kwargs):
+    """Log a message with severity 'WARNING' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console handler with a
+    pre-defined format.
+    """
+    if len(root.handlers) == 0:
+        basic_config()
+    root.warning(*msg, args=args, **kwargs)
+
+
+def warn(*msg, args=(), **kwargs):
+    """An alias of warning()"""
+    warning(*msg, args=args, **kwargs)
+
+
+def info(*msg, args=(), **kwargs):
+    """Log a message with severity 'INFO' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console handler with a
+    pre-defined format.
+    """
+    if len(root.handlers) == 0:
+        basic_config()
+    root.info(*msg, args=args, **kwargs)
+
+
+def debug(*msg, args=(), **kwargs):
+    """Log a message with severity 'DEBUG' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console handler with a
+    pre-defined format.
+    """
+    if len(root.handlers) == 0:
+        basic_config()
+    root.debug(*msg, args=args, **kwargs)
+
+
+def log(level, *msg, args=(), **kwargs):
+    """Log 'msg % args' with the integer severity 'level' on the root logger.
+
+    If the logger has no handlers, call basicConfig() to add a console handler with a
+    pre-defined format.
+    """
+    if len(root.handlers) == 0:
+        basic_config()
+    root.log(level, *msg, args=args, **kwargs)
+
+
+def progress_bar(
+    progress: float,
+    total: float,
+    width: _Optional[int] = None,
+    prefix: str = '|',
+    suffix: str = '|',
+    show_percentage: bool = True
+):
+    """Print a progress bar to the console."""
+
+    progress_bar_ = ProgressBar(
+        width=width, prefix=prefix, suffix=suffix, show_percentage=show_percentage
+    )
+
+    print(progress_bar_.get_bar(progress, total))
+
+
+endl = '\n'
+
+console_reporter = CrashReporter.ConsoleReporter()
+
+file_reporter = CrashReporter.FileReporter(file='.crash_report.log')
```

### Comparing `log21-2.8.1b0/src/log21.egg-info/SOURCES.txt` & `log21-2.9.0/src/log21.egg-info/SOURCES.txt`

 * *Files identical despite different names*

