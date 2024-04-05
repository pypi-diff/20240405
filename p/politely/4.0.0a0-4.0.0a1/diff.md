# Comparing `tmp/politely-4.0.0a0.tar.gz` & `tmp/politely-4.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "politely-4.0.0a0.tar", max compression
+gzip compressed data, was "politely-4.0.0a1.tar", max compression
```

## Comparing `politely-4.0.0a0.tar` & `politely-4.0.0a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10895 2024-04-05 04:59:46.503224 politely-4.0.0a0/README.md
--rw-r--r--   0        0        0      131 2024-04-02 08:15:05.754312 politely-4.0.0a0/politely/__init__.py
--rw-r--r--   0        0        0      846 2024-04-05 04:59:46.504517 politely-4.0.0a0/politely/errors.py
--rw-r--r--   0        0        0      676 2024-04-05 04:59:46.504948 politely-4.0.0a0/politely/fetchers.py
--rw-r--r--   0        0        0     2949 2024-04-05 04:59:46.505487 politely-4.0.0a0/politely/modeling_gpt2_scorer.py
--rw-r--r--   0        0        0     1202 2024-04-05 04:59:46.505881 politely-4.0.0a0/politely/modeling_heuristic_scorer.py
--rw-r--r--   0        0        0      715 2024-04-05 04:59:46.506199 politely-4.0.0a0/politely/modeling_sbg_scorer.py
--rw-r--r--   0        0        0      171 2024-04-05 04:59:46.506564 politely-4.0.0a0/politely/modeling_scorer.py
--rw-r--r--   0        0        0     5372 2024-04-05 04:59:46.507048 politely-4.0.0a0/politely/rules.py
--rw-r--r--   0        0        0     7024 2024-04-05 04:59:46.507502 politely-4.0.0a0/politely/styler.py
--rw-r--r--   0        0        0      424 2024-04-05 04:59:46.507879 politely-4.0.0a0/pyproject.toml
--rw-r--r--   0        0        0    11423 1970-01-01 00:00:00.000000 politely-4.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0    11290 2024-04-05 06:02:35.984691 politely-4.0.0a1/README.md
+-rw-r--r--   0        0        0      131 2024-04-02 08:15:05.754312 politely-4.0.0a1/politely/__init__.py
+-rw-r--r--   0        0        0      846 2024-04-05 04:59:46.504517 politely-4.0.0a1/politely/errors.py
+-rw-r--r--   0        0        0      676 2024-04-05 04:59:46.504948 politely-4.0.0a1/politely/fetchers.py
+-rw-r--r--   0        0        0     2957 2024-04-05 06:02:35.993400 politely-4.0.0a1/politely/modeling_gpt2_scorer.py
+-rw-r--r--   0        0        0     1202 2024-04-05 04:59:46.505881 politely-4.0.0a1/politely/modeling_heuristic_scorer.py
+-rw-r--r--   0        0        0      715 2024-04-05 06:02:35.993683 politely-4.0.0a1/politely/modeling_sbg_scorer.py
+-rw-r--r--   0        0        0      171 2024-04-05 05:55:13.336972 politely-4.0.0a1/politely/modeling_scorer.py
+-rw-r--r--   0        0        0     5190 2024-04-05 06:02:35.994439 politely-4.0.0a1/politely/rules.py
+-rw-r--r--   0        0        0     7331 2024-04-05 06:02:35.994836 politely-4.0.0a1/politely/styler.py
+-rw-r--r--   0        0        0      572 2024-04-05 06:02:35.995047 politely-4.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0    11913 1970-01-01 00:00:00.000000 politely-4.0.0a1/PKG-INFO
```

### Comparing `politely-4.0.0a0/README.md` & `politely-4.0.0a1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -145,33 +145,50 @@
 ```
 
 ```
 ##### lm을 쓰지 않는 경우 맥락 고려 X ######
 내일 나랑 같이 점심 먹어.
 ```
 
-But `gpt2` scorer is a bit slower, but does take context into account.
+`sbg` scorer (SkipBigram) is a bit slower, but does take context into account.
 
 ```shell
 # Pytorch is required to use GPT2 scorer. Install the version that fits your environment.
 pip3 install torch
 ```
 ```python
 from politely.modeling_gpt2_scorer import GPT2Scorer
-styler = Styler(scorer="gpt2")  # uses GPT2Scorer by default
+styler = Styler(scorer="sbg")  # uses GPT2Scorer by default
 print("##### lm을 쓰는 경우 맥락 고려 O ######")
 print(styler("내일 저랑 같이 점심 먹어요.", 0))
 ```
 
 ```
 ##### lm을 쓰는 경우 맥락 고려 O ######
 내일 나랑 같이 점심 먹자.  # 권유가 아닌 청유이므로 이게 맞음
 ```
 
-More scoring options will be made available in the future. 
+`gpt2` scorer is the most accurate, but it is also the slowest. 
+
+```shell
+# need to install optional dependency
+pip3 install "politely[gpt2]"
+```
+
+```python
+styler = Styler(scorer="gpt2")
+print("##### lm을 쓰는 경우 맥락 고려 O ######")
+print(styler("내일 저랑 같이 점심 먹어요.", 0))
+```
+
+```
+##### lm을 쓰는 경우 맥락 고려 O ######
+내일 저랑 같이 점심 먹으러 가요.  # 권유이므로 이게 맞음
+```
+
 
 ## Hosting the interactive demo 
 
 You can either host the interactive demo locally (You have to setup your own `OPENAI_API_KEY`)
 ```shell
 export OPENAI_API_KEY = ...
 # host the demo via streamlit
```

### Comparing `politely-4.0.0a0/politely/errors.py` & `politely-4.0.0a1/politely/errors.py`

 * *Files identical despite different names*

### Comparing `politely-4.0.0a0/politely/fetchers.py` & `politely-4.0.0a1/politely/fetchers.py`

 * *Files identical despite different names*

### Comparing `politely-4.0.0a0/politely/modeling_gpt2_scorer.py` & `politely-4.0.0a1/politely/modeling_gpt2_scorer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 import random
 import numpy as np
 from kiwipiepy import Kiwi
-from transformers import AutoTokenizer, GPT2LMHeadModel
 from politely.modeling_scorer import Scorer
 from politely import TAG
 
 
 class GPT2Scorer(Scorer):
     """
     More accurate than heuristic scorer, but slower. Could be made faster with GPU support. 
     """
 
     def __init__(self, device: str = "cpu"):
         import torch
+        from transformers import AutoTokenizer, GPT2LMHeadModel
         self.gpt2 = GPT2LMHeadModel.from_pretrained(
             "beomi/kykim-gpt3-kor-small_based_on_gpt2"
         ).to(device)
         self.tokenizer = AutoTokenizer.from_pretrained(
             "beomi/kykim-gpt3-kor-small_based_on_gpt2"
         )
         self.device = device
```

### Comparing `politely-4.0.0a0/politely/modeling_heuristic_scorer.py` & `politely-4.0.0a1/politely/modeling_heuristic_scorer.py`

 * *Files identical despite different names*

### Comparing `politely-4.0.0a0/politely/modeling_sbg_scorer.py` & `politely-4.0.0a1/politely/modeling_sbg_scorer.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from politely.rules import TAG
-from .modeling_scorer import Scorer
 from kiwipiepy import Kiwi
+from .modeling_scorer import Scorer
 
 
 
 class SkipBigramScorer(Scorer):
     """
     This is better than heuristic scorer, but slightly less accurate than gpt2 scorer. 
     Good for most cases.
```

### Comparing `politely-4.0.0a0/politely/rules.py` & `politely-4.0.0a1/politely/rules.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-"""
-규칙:
-1.
-"""
-from typing import Set, Tuple, Dict
-
 # --- symbols --- #
 NULL = "❌"
 TAG = "🏷"
 SEP = "🔗"
 
 
 # --- all EF's of different styles they must be singular tokens --- #
@@ -67,15 +61,15 @@
 EFS = rf"(?P<MASK>({'|'.join([pair for pair in (CASUAL | POLITE | FORMAL)])}))"
 SELF = rf"\g<MASK>"
 WITH_JONG_SUNG = rf"[{''.join({chr(i) for i in range(44032, 55204)} - {chr(44032 + 28 * i) for i in range(399)})}]"
 NO_JONG_SUNG = rf"[^{''.join({chr(i) for i in range(44032, 55204)} - {chr(44032 + 28 * i) for i in range(399)})}]"
 
 
 # --- programmatically populated RULES --- #
-RULES: Dict[str, Tuple[Set[str], Set[str], Set[str]]] = dict()
+RULES: dict[str, tuple[set[str], set[str], set[str]]] = dict()
 
 # --- the overarching rule --- #
 RULES.update({
     EFS: (
         CASUAL,
         POLITE,
         FORMAL
@@ -199,15 +193,14 @@
 
 # --- 지 -> 지요 --- #
 RULES.update(
     {
         rf"(?P<MASK>(지|지요|ᆸ니다){TAG}EF)": (
             {f"지{TAG}EF"},
             {f"지요{TAG}EF"},
-            #  전부 가능함
             FORMAL
         )
     }
 )
 
 
 # --- 시 + ㄴ가요 -> 시 + 니 --- #
@@ -217,25 +210,16 @@
             {f"니{TAG}EF"},
             {f"ᆫ가요{TAG}EF"},
             {f"ᆸ니까{TAG}EF"}
         )
     }
 )
 
-# --- -어요 인 경우, 란다는 사용하지 않음 --- #
-RULES.update(
-    {
-        rf"(?P<MASK>어요{TAG}EF)": (
-            CASUAL - {f"란다{TAG}EF"},
-            {"어요{TAG}EF"},
-            FORMAL
-        )
-    }
-)
-
+# rule을 추가할 때 ... 교집합이 너무 금방 사라진다는 것이 문제.
+# 너무 많은 룰을 추가하면 안될듯함. 
 
 # ---- to be used for scoring -- #
 PREFERENCES = {
     f"어{TAG}EF",
     f"어요{TAG}EF",
     f"어요{TAG}EF",
     f"습니다{TAG}EF",
```

### Comparing `politely-4.0.0a0/politely/styler.py` & `politely-4.0.0a1/politely/styler.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,21 +38,27 @@
         #  --- object-owned attributes --- #
         if scorer == "heuristic":
             self.scorer: Scorer = HeuristicScorer()
         elif scorer == "sbg":
             self.scorer: Scorer = SkipBigramScorer()
         elif scorer == "gpt2":
             try:
+                import transformers
+            except ImportError:
+                raise ImportError(
+                    "`transformers` is required to use `GPT2Scorer`. Please install it via `pip3 install transformers`."
+                )
+            try:
                 import torch
             except ImportError:
                 raise ImportError(
                     "`torch` (Pytorch) is required to use `GPT2Scorer`. Please install it via `pip3 install torch`."
                 )
-            else:
-                self.scorer: Scorer = GPT2Scorer()
+
+            self.scorer: Scorer = GPT2Scorer()
         else:
             raise ValueError(
                 f"scorer should be either 'heuristic', `sbg` or 'gpt2', but got {scorer}"
             )
         self.strict = strict
         self.out: any = None
         self.kiwi = fetch_kiwi()
@@ -155,14 +161,15 @@
         candidates = [
             [pair.split(SEP) for pair in candidate if pair != NULL]
             for candidate in candidates
         ]
         # flatten pairs
         candidates = [list(itertools.chain(*candidate)) for candidate in candidates]
         # a list of candidates
+        assert len(candidates) > 0, "Candidates should not be empty"
         self.out = candidates
         return self
 
     @log
     def guess(self):
         """
         Guess the scores.
```

### Comparing `politely-4.0.0a0/PKG-INFO` & `politely-4.0.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: politely
-Version: 4.0.0a0
+Version: 4.0.0a1
 Summary: An explainable styler for the Korean language
 Author: Eu-Bin KIM
 Author-email: tlrndk123@gmail.com
 Requires-Python: >=3.9.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: gpt2
 Requires-Dist: kiwipiepy (>=0.17.0,<0.18.0)
-Requires-Dist: transformers (>=4.39.3,<5.0.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0) ; extra == "gpt2"
+Requires-Dist: transformers (>=4.39.3,<5.0.0) ; extra == "gpt2"
 Description-Content-Type: text/markdown
 
 # Politely
 
 [![PyPI version](https://badge.fury.io/py/politely.svg)](https://badge.fury.io/py/politely)
 [![Open in Streamlit](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://politely.streamlit.app)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1tpx_wrMmzD_pWeEibeenlU4q8TuKK1j7?usp=sharing)
@@ -160,33 +162,50 @@
 ```
 
 ```
 ##### lm을 쓰지 않는 경우 맥락 고려 X ######
 내일 나랑 같이 점심 먹어.
 ```
 
-But `gpt2` scorer is a bit slower, but does take context into account.
+`sbg` scorer (SkipBigram) is a bit slower, but does take context into account.
 
 ```shell
 # Pytorch is required to use GPT2 scorer. Install the version that fits your environment.
 pip3 install torch
 ```
 ```python
 from politely.modeling_gpt2_scorer import GPT2Scorer
-styler = Styler(scorer="gpt2")  # uses GPT2Scorer by default
+styler = Styler(scorer="sbg")  # uses GPT2Scorer by default
 print("##### lm을 쓰는 경우 맥락 고려 O ######")
 print(styler("내일 저랑 같이 점심 먹어요.", 0))
 ```
 
 ```
 ##### lm을 쓰는 경우 맥락 고려 O ######
 내일 나랑 같이 점심 먹자.  # 권유가 아닌 청유이므로 이게 맞음
 ```
 
-More scoring options will be made available in the future. 
+`gpt2` scorer is the most accurate, but it is also the slowest. 
+
+```shell
+# need to install optional dependency
+pip3 install "politely[gpt2]"
+```
+
+```python
+styler = Styler(scorer="gpt2")
+print("##### lm을 쓰는 경우 맥락 고려 O ######")
+print(styler("내일 저랑 같이 점심 먹어요.", 0))
+```
+
+```
+##### lm을 쓰는 경우 맥락 고려 O ######
+내일 저랑 같이 점심 먹으러 가요.  # 권유이므로 이게 맞음
+```
+
 
 ## Hosting the interactive demo 
 
 You can either host the interactive demo locally (You have to setup your own `OPENAI_API_KEY`)
 ```shell
 export OPENAI_API_KEY = ...
 # host the demo via streamlit
```

