# Comparing `tmp/politely-4.0.0a1.tar.gz` & `tmp/politely-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "politely-4.0.0a1.tar", max compression
+gzip compressed data, was "politely-4.0.1.tar", max compression
```

## Comparing `politely-4.0.0a1.tar` & `politely-4.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11290 2024-04-05 06:02:35.984691 politely-4.0.0a1/README.md
--rw-r--r--   0        0        0      131 2024-04-02 08:15:05.754312 politely-4.0.0a1/politely/__init__.py
--rw-r--r--   0        0        0      846 2024-04-05 04:59:46.504517 politely-4.0.0a1/politely/errors.py
--rw-r--r--   0        0        0      676 2024-04-05 04:59:46.504948 politely-4.0.0a1/politely/fetchers.py
--rw-r--r--   0        0        0     2957 2024-04-05 06:02:35.993400 politely-4.0.0a1/politely/modeling_gpt2_scorer.py
--rw-r--r--   0        0        0     1202 2024-04-05 04:59:46.505881 politely-4.0.0a1/politely/modeling_heuristic_scorer.py
--rw-r--r--   0        0        0      715 2024-04-05 06:02:35.993683 politely-4.0.0a1/politely/modeling_sbg_scorer.py
--rw-r--r--   0        0        0      171 2024-04-05 05:55:13.336972 politely-4.0.0a1/politely/modeling_scorer.py
--rw-r--r--   0        0        0     5190 2024-04-05 06:02:35.994439 politely-4.0.0a1/politely/rules.py
--rw-r--r--   0        0        0     7331 2024-04-05 06:02:35.994836 politely-4.0.0a1/politely/styler.py
--rw-r--r--   0        0        0      572 2024-04-05 06:02:35.995047 politely-4.0.0a1/pyproject.toml
--rw-r--r--   0        0        0    11913 1970-01-01 00:00:00.000000 politely-4.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11290 2024-04-05 06:02:35.984691 politely-4.0.1/README.md
+-rw-r--r--   0        0        0      131 2024-04-02 08:15:05.754312 politely-4.0.1/politely/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-05 04:59:46.504517 politely-4.0.1/politely/errors.py
+-rw-r--r--   0        0        0      676 2024-04-05 04:59:46.504948 politely-4.0.1/politely/fetchers.py
+-rw-r--r--   0        0        0     2957 2024-04-05 06:02:35.993400 politely-4.0.1/politely/modeling_gpt2_scorer.py
+-rw-r--r--   0        0        0     1202 2024-04-05 04:59:46.505881 politely-4.0.1/politely/modeling_heuristic_scorer.py
+-rw-r--r--   0        0        0      715 2024-04-05 06:02:35.993683 politely-4.0.1/politely/modeling_sbg_scorer.py
+-rw-r--r--   0        0        0      171 2024-04-05 05:55:13.336972 politely-4.0.1/politely/modeling_scorer.py
+-rw-r--r--   0        0        0     6675 2024-04-05 06:57:39.149962 politely-4.0.1/politely/rules.py
+-rw-r--r--   0        0        0     7331 2024-04-05 06:02:35.994836 politely-4.0.1/politely/styler.py
+-rw-r--r--   0        0        0      588 2024-04-05 07:00:36.494030 politely-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11911 1970-01-01 00:00:00.000000 politely-4.0.1/PKG-INFO
```

### Comparing `politely-4.0.0a1/README.md` & `politely-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `politely-4.0.0a1/politely/errors.py` & `politely-4.0.1/politely/errors.py`

 * *Files identical despite different names*

### Comparing `politely-4.0.0a1/politely/fetchers.py` & `politely-4.0.1/politely/fetchers.py`

 * *Files identical despite different names*

### Comparing `politely-4.0.0a1/politely/modeling_gpt2_scorer.py` & `politely-4.0.1/politely/modeling_gpt2_scorer.py`

 * *Files identical despite different names*

### Comparing `politely-4.0.0a1/politely/modeling_heuristic_scorer.py` & `politely-4.0.1/politely/modeling_heuristic_scorer.py`

 * *Files identical despite different names*

### Comparing `politely-4.0.0a1/politely/modeling_sbg_scorer.py` & `politely-4.0.1/politely/modeling_sbg_scorer.py`

 * *Files identical despite different names*

### Comparing `politely-4.0.0a1/politely/rules.py` & `politely-4.0.1/politely/rules.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,43 +10,91 @@
     f"다{TAG}EF",
     f"니{TAG}EF",
     f"라{TAG}EF",
     f"어라{TAG}EF",
     f"자{TAG}EF",
     f"대{TAG}EF",
     f"는다{TAG}EF",
+    f"는데{TAG}EF",
     f"마{TAG}EF",
     f"야{TAG}EF",
     f"군{TAG}EF",
+    f"구나{TAG}EF",
     f"네{TAG}EF",
     f"냐{TAG}EF",
     f"ᆫ다{TAG}EF",
     f"란다{TAG}EF",
     f"ᆯ게{TAG}EF",
+    f"ᆯ래{TAG}EF",
+    f"ᆯ까{TAG}EF",
     f"ᆫ대{TAG}EF",
+    f"ᆫ데{TAG}EF",
     f"ᆫ가{TAG}EF",
-    f"지{TAG}EF"
+    f"지{TAG}EF", 
+    f"던데{TAG}EF",
+    f"는데{TAG}EF",
+    f"은데{TAG}EF",
+    f"데{TAG}EF",
+    f"잖아{TAG}EF",
+    f"을까{TAG}EF",
+    f"을까나{TAG}EF",
+    f"을래{TAG}EF",
+    f"을게{TAG}EF",
+    f"라고{TAG}EF",
+    f"고{TAG}EF",
+    f"니까{TAG}EF",
+    f"으니까{TAG}EF",
+    f"니깐{TAG}EF",
+    f"더라{TAG}EF",
+    f"는다고{TAG}EF",
+    f"다고{TAG}EF",
+    f"거든{TAG}EF", 
+    f"는군{TAG}EF",
+    f"어야지{TAG}EF"
 }
 
 POLITE = {
     f"요{TAG}EF",
+    f"군요{TAG}EF",
     f"어요{TAG}EF",
     f"에요{TAG}EF",
+    f"예요{TAG}EF",
     f"ᆫ가요{TAG}EF",
     f"지요{TAG}EF",
     f"래요{TAG}EF",
     f"죠{TAG}EF",
     f"래요{TAG}EF",
     f"네요{TAG}EF",
     f"나요{TAG}EF",
     f"대요{TAG}EF",
+    f"데요{TAG}EF",
+    f"은데요{TAG}EF",
     f"ᆯ게요{TAG}EF",
+    f"ᆯ까요{TAG}EF",
     f"ᆫ대요{TAG}EF",
     f"ᆫ가요{TAG}EF",
-    f"세요{TAG}EF"
+    f"으세요{TAG}EF",
+    f"세요{TAG}EF",
+    f"던데요{TAG}EF",
+    f"잖아요{TAG}EF",
+    f"을까요{TAG}EF",
+    f"ᆯ래요{TAG}EF",
+    f"라고요{TAG}EF",
+    f"니까요{TAG}EF",
+    f"니깐요{TAG}EF",
+    f"더라고요{TAG}EF",
+    f"더군요{TAG}EF",
+    f"는다고요{TAG}EF",
+    f"다고요{TAG}EF",
+    f"거든요{TAG}EF",
+    f"는데요{TAG}EF",
+    f"는군요{TAG}EF",
+    f"어서요{TAG}EF",
+    f"어야지요{TAG}EF",
+    f"어야죠{TAG}EF"
 }
 
 FORMAL = {
     f"습니다{TAG}EF",
     f"습니까{TAG}EF",
     f"랍니다{TAG}EF",
     f"ᆸ니까{TAG}EF",
@@ -83,14 +131,26 @@
             {NULL},  # you don't use them
             {SELF},  # just repeat yourself
             {SELF},  # just repeat yourself
         )
     }
 )
 
+# --- 계시/VX: 반말을 쓰는 경우 제거 --- #
+RULES.update(
+    {
+        rf"(?P<MASK>계시{TAG}VX)": (
+            {f"있{TAG}VX"},  # replace it with this.
+            {SELF},  # just repeat yourself
+            {SELF},  # just repeat yourself
+        )
+    }
+)
+
+
 
 # --- 종성이 있는 경우, 종성으로 시작하는 EF는 사용하지 않음 --- #
 RULES.update(
     {
         rf"{WITH_JONG_SUNG}{TAG}[A-Z\-]+?{SEP}{EFS}": (
             CASUAL - {f"ᆫ다{TAG}EF", f"ᆯ게{TAG}EF", f"ᆫ대{TAG}EF"},
             POLITE - {f"ᆯ게요{TAG}EF", f"ᆫ대요{TAG}EF", f"ᆫ가요{TAG}EF"},
@@ -99,26 +159,26 @@
     }
 )
 
 # --- 종성이 없는 경우, 어/EF, f"어라{TAG}EF", 어요/EF는 사용하지 않음 --- #
 RULES.update(
     {
         rf"{NO_JONG_SUNG}{TAG}[A-Z\-]+?{SEP}{EFS}": (
-            CASUAL - {f"어{TAG}EF", f"어라{TAG}EF"},
+            CASUAL - {f"어{TAG}EF", f"어라{TAG}EF", f"마{TAG}EF"},
             POLITE - {f"어요{TAG}EF"},
             FORMAL
         )
     }
 )
 
-# --- 의문형인 경우, formal은 -니까만 가능 --- #
+# --- 의문형인 경우, CASUAL에서 -다는 불가. formal은 -니까만 가능 --- #
 RULES.update(
     {
         rf"{EFS}{SEP}\?{TAG}SF": (
-            CASUAL,
+            CASUAL - {f"다{TAG}EF", f"데{TAG}EF"},
             POLITE,
             {f"습니까{TAG}EF", f"ᆸ니까{TAG}EF", f"시{TAG}EP{SEP}ᆸ니까{TAG}EF"}
         )
     }
 )
 
 # --- 나/저 --- #
```

### Comparing `politely-4.0.0a1/politely/styler.py` & `politely-4.0.1/politely/styler.py`

 * *Files identical despite different names*

### Comparing `politely-4.0.0a1/pyproject.toml` & `politely-4.0.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "politely"
-version = "4.0.0a1"
+version = "4.0.1"
 description = "An explainable styler for the Korean language"
 authors = ["Eu-Bin KIM <tlrndk123@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.12"
 kiwipiepy = "^0.17.0"
@@ -13,11 +13,12 @@
 
 [tool.poetry.extras]
 gpt2 = ["transformers", "torch"]
 
 [tool.poetry.group.dev.dependencies]
 python-dotenv = "^1.0.1"
 pytest = "^8.1.1"
+pandas = "^2.2.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `politely-4.0.0a1/PKG-INFO` & `politely-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: politely
-Version: 4.0.0a1
+Version: 4.0.1
 Summary: An explainable styler for the Korean language
 Author: Eu-Bin KIM
 Author-email: tlrndk123@gmail.com
 Requires-Python: >=3.9.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

