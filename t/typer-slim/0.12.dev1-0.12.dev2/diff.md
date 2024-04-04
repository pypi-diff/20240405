# Comparing `tmp/typer_slim-0.12.dev1.tar.gz` & `tmp/typer_slim-0.12.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typer_slim-0.12.dev1.tar", last modified: Sat Mar 30 01:26:04 2024, max compression
+gzip compressed data, was "typer_slim-0.12.dev2.tar", last modified: Sat Mar 30 01:51:46 2024, max compression
```

## Comparing `typer_slim-0.12.dev1.tar` & `typer_slim-0.12.dev2.tar`

### file list

```diff
@@ -1,578 +1,578 @@
--rw-r--r--   0        0        0     1086 2024-03-30 01:26:02.451405 typer_slim-0.12.dev1/LICENSE
--rw-r--r--   0        0        0    13990 2024-03-30 01:26:02.451405 typer_slim-0.12.dev1/README.md
--rw-r--r--   0        0        0      310 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/app_dir/tutorial001.py
--rw-r--r--   0        0        0      144 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/default/tutorial001.py
--rw-r--r--   0        0        0      197 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/default/tutorial001_an.py
--rw-r--r--   0        0        0      252 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/default/tutorial002.py
--rw-r--r--   0        0        0      302 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/default/tutorial002_an.py
--rw-r--r--   0        0        0      165 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/envvar/tutorial001.py
--rw-r--r--   0        0        0      216 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/envvar/tutorial001_an.py
--rw-r--r--   0        0        0      179 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/envvar/tutorial002.py
--rw-r--r--   0        0        0      237 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/envvar/tutorial002_an.py
--rw-r--r--   0        0        0      184 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/envvar/tutorial003.py
--rw-r--r--   0        0        0      256 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/envvar/tutorial003_an.py
--rw-r--r--   0        0        0      172 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial001.py
--rw-r--r--   0        0        0      217 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial001_an.py
--rw-r--r--   0        0        0      231 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial002.py
--rw-r--r--   0        0        0      276 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial002_an.py
--rw-r--r--   0        0        0      218 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial003.py
--rw-r--r--   0        0        0      269 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial003_an.py
--rw-r--r--   0        0        0      238 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial004.py
--rw-r--r--   0        0        0      310 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial004_an.py
--rw-r--r--   0        0        0      232 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial005.py
--rw-r--r--   0        0        0      314 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial005_an.py
--rw-r--r--   0        0        0      164 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial006.py
--rw-r--r--   0        0        0      215 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial006_an.py
--rw-r--r--   0        0        0      447 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial007.py
--rw-r--r--   0        0        0      523 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial007_an.py
--rw-r--r--   0        0        0      210 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial008.py
--rw-r--r--   0        0        0      261 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/help/tutorial008_an.py
--rw-r--r--   0        0        0      131 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/optional/tutorial001.py
--rw-r--r--   0        0        0      181 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/optional/tutorial001_an.py
--rw-r--r--   0        0        0      247 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/optional/tutorial002.py
--rw-r--r--   0        0        0      292 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/optional/tutorial002_an.py
--rw-r--r--   0        0        0      142 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/arguments/optional/tutorial003.py
--rw-r--r--   0        0        0      241 2024-03-30 01:26:02.455405 typer_slim-0.12.dev1/docs_src/commands/arguments/tutorial001.py
--rw-r--r--   0        0        0      721 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/callback/tutorial001.py
--rw-r--r--   0        0        0      216 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/callback/tutorial002.py
--rw-r--r--   0        0        0      304 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/callback/tutorial003.py
--rw-r--r--   0        0        0      315 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/callback/tutorial004.py
--rw-r--r--   0        0        0      411 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/context/tutorial001.py
--rw-r--r--   0        0        0      390 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/context/tutorial002.py
--rw-r--r--   0        0        0      451 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/context/tutorial003.py
--rw-r--r--   0        0        0      277 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/context/tutorial004.py
--rw-r--r--   0        0        0     1197 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial001.py
--rw-r--r--   0        0        0     1301 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial001_an.py
--rw-r--r--   0        0        0      439 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial002.py
--rw-r--r--   0        0        0      386 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial003.py
--rw-r--r--   0        0        0      827 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial004.py
--rw-r--r--   0        0        0      903 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial004_an.py
--rw-r--r--   0        0        0      786 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial005.py
--rw-r--r--   0        0        0      855 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial005_an.py
--rw-r--r--   0        0        0     1143 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial006.py
--rw-r--r--   0        0        0     1044 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial007.py
--rw-r--r--   0        0        0     1200 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial007_an.py
--rw-r--r--   0        0        0      293 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/help/tutorial008.py
--rw-r--r--   0        0        0      138 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/index/tutorial001.py
--rw-r--r--   0        0        0      215 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/index/tutorial002.py
--rw-r--r--   0        0        0      235 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/index/tutorial003.py
--rw-r--r--   0        0        0      275 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/name/tutorial001.py
--rw-r--r--   0        0        0      187 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/one_or_multiple/tutorial001.py
--rw-r--r--   0        0        0      287 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/one_or_multiple/tutorial002.py
--rw-r--r--   0        0        0      708 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/options/tutorial001.py
--rw-r--r--   0        0        0      772 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/commands/options/tutorial001_an.py
--rw-r--r--   0        0        0      115 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/exceptions/tutorial001.py
--rw-r--r--   0        0        0      174 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/exceptions/tutorial002.py
--rw-r--r--   0        0        0      170 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/exceptions/tutorial003.py
--rw-r--r--   0        0        0      171 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/exceptions/tutorial004.py
--rw-r--r--   0        0        0      101 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/first_steps/tutorial001.py
--rw-r--r--   0        0        0      112 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/first_steps/tutorial002.py
--rw-r--r--   0        0        0      138 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/first_steps/tutorial003.py
--rw-r--r--   0        0        0      239 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/first_steps/tutorial004.py
--rw-r--r--   0        0        0      244 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/first_steps/tutorial005.py
--rw-r--r--   0        0        0      358 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/first_steps/tutorial006.py
--rw-r--r--   0        0        0      157 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/launch/tutorial001.py
--rw-r--r--   0        0        0      527 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/launch/tutorial002.py
--rw-r--r--   0        0        0      294 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/multiple_values/arguments_with_multiple_values/tutorial001.py
--rw-r--r--   0        0        0      292 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/multiple_values/arguments_with_multiple_values/tutorial002.py
--rw-r--r--   0        0        0      343 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/multiple_values/arguments_with_multiple_values/tutorial002_an.py
--rw-r--r--   0        0        0      317 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/multiple_values/multiple_options/tutorial001.py
--rw-r--r--   0        0        0      370 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/multiple_values/multiple_options/tutorial001_an.py
--rw-r--r--   0        0        0      178 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/multiple_values/multiple_options/tutorial002.py
--rw-r--r--   0        0        0      231 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/multiple_values/multiple_options/tutorial002_an.py
--rw-r--r--   0        0        0      403 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/multiple_values/options_with_multiple_values/tutorial001.py
--rw-r--r--   0        0        0      456 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/multiple_values/options_with_multiple_values/tutorial001_an.py
--rw-r--r--   0        0        0      339 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/callback/tutorial001.py
--rw-r--r--   0        0        0      382 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/callback/tutorial001_an.py
--rw-r--r--   0        0        0      368 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/callback/tutorial002.py
--rw-r--r--   0        0        0      411 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/callback/tutorial002_an.py
--rw-r--r--   0        0        0      433 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/callback/tutorial003.py
--rw-r--r--   0        0        0      476 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/callback/tutorial003_an.py
--rw-r--r--   0        0        0      477 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/callback/tutorial004.py
--rw-r--r--   0        0        0      520 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/callback/tutorial004_an.py
--rw-r--r--   0        0        0      464 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/help/tutorial001.py
--rw-r--r--   0        0        0      526 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/help/tutorial001_an.py
--rw-r--r--   0        0        0      643 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/help/tutorial002.py
--rw-r--r--   0        0        0      778 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/help/tutorial002_an.py
--rw-r--r--   0        0        0      170 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/help/tutorial003.py
--rw-r--r--   0        0        0      221 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/help/tutorial003_an.py
--rw-r--r--   0        0        0      217 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/help/tutorial004.py
--rw-r--r--   0        0        0      268 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/help/tutorial004_an.py
--rw-r--r--   0        0        0      152 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/name/tutorial001.py
--rw-r--r--   0        0        0      197 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/name/tutorial001_an.py
--rw-r--r--   0        0        0      158 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/name/tutorial002.py
--rw-r--r--   0        0        0      203 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/name/tutorial002_an.py
--rw-r--r--   0        0        0      148 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/name/tutorial003.py
--rw-r--r--   0        0        0      193 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/name/tutorial003_an.py
--rw-r--r--   0        0        0      163 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/name/tutorial004.py
--rw-r--r--   0        0        0      208 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/name/tutorial004_an.py
--rw-r--r--   0        0        0      281 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/name/tutorial005.py
--rw-r--r--   0        0        0      337 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/name/tutorial005_an.py
--rw-r--r--   0        0        0      212 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/password/tutorial001.py
--rw-r--r--   0        0        0      262 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/password/tutorial001_an.py
--rw-r--r--   0        0        0      341 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/password/tutorial002.py
--rw-r--r--   0        0        0      386 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/password/tutorial002_an.py
--rw-r--r--   0        0        0      171 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/prompt/tutorial001.py
--rw-r--r--   0        0        0      216 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/prompt/tutorial001_an.py
--rw-r--r--   0        0        0      204 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/prompt/tutorial002.py
--rw-r--r--   0        0        0      254 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/prompt/tutorial002_an.py
--rw-r--r--   0        0        0      198 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/prompt/tutorial003.py
--rw-r--r--   0        0        0      250 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/prompt/tutorial003_an.py
--rw-r--r--   0        0        0      155 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/required/tutorial001.py
--rw-r--r--   0        0        0      205 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/required/tutorial001_an.py
--rw-r--r--   0        0        0      166 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/required/tutorial002.py
--rw-r--r--   0        0        0      430 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/version/tutorial001.py
--rw-r--r--   0        0        0      494 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/version/tutorial001_an.py
--rw-r--r--   0        0        0      566 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/version/tutorial002.py
--rw-r--r--   0        0        0      622 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/version/tutorial002_an.py
--rw-r--r--   0        0        0      597 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/version/tutorial003.py
--rw-r--r--   0        0        0      662 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options/version/tutorial003_an.py
--rw-r--r--   0        0        0      193 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial001.py
--rw-r--r--   0        0        0      244 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial001_an.py
--rw-r--r--   0        0        0      313 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial002.py
--rw-r--r--   0        0        0      364 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial002_an.py
--rw-r--r--   0        0        0      479 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial003.py
--rw-r--r--   0        0        0      530 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial003_an.py
--rw-r--r--   0        0        0      665 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial004.py
--rw-r--r--   0        0        0      716 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial004_an.py
--rw-r--r--   0        0        0      564 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial005.py
--rw-r--r--   0        0        0      615 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial005_an.py
--rw-r--r--   0        0        0      262 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial006.py
--rw-r--r--   0        0        0      320 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial006_an.py
--rw-r--r--   0        0        0      700 2024-03-30 01:26:02.459405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial007.py
--rw-r--r--   0        0        0      760 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial007_an.py
--rw-r--r--   0        0        0      736 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial008.py
--rw-r--r--   0        0        0      796 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial008_an.py
--rw-r--r--   0        0        0      819 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial009.py
--rw-r--r--   0        0        0      879 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial009_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/bool/__init__.py
--rw-r--r--   0        0        0      208 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/bool/tutorial001.py
--rw-r--r--   0        0        0      259 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/bool/tutorial001_an.py
--rw-r--r--   0        0        0      323 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/bool/tutorial002.py
--rw-r--r--   0        0        0      374 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/bool/tutorial002_an.py
--rw-r--r--   0        0        0      228 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/bool/tutorial003.py
--rw-r--r--   0        0        0      279 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/bool/tutorial003_an.py
--rw-r--r--   0        0        0      225 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/bool/tutorial004.py
--rw-r--r--   0        0        0      276 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/bool/tutorial004_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/custom_types/__init__.py
--rw-r--r--   0        0        0      542 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/custom_types/tutorial001.py
--rw-r--r--   0        0        0      605 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/custom_types/tutorial001_an.py
--rw-r--r--   0        0        0      646 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/custom_types/tutorial002.py
--rw-r--r--   0        0        0      721 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/custom_types/tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/datetime/__init__.py
--rw-r--r--   0        0        0      211 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/datetime/tutorial001.py
--rw-r--r--   0        0        0      294 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/datetime/tutorial002.py
--rw-r--r--   0        0        0      370 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/datetime/tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/enum/__init__.py
--rw-r--r--   0        0        0      299 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/enum/tutorial001.py
--rw-r--r--   0        0        0      342 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/enum/tutorial002.py
--rw-r--r--   0        0        0      407 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/enum/tutorial002_an.py
--rw-r--r--   0        0        0      349 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/enum/tutorial003.py
--rw-r--r--   0        0        0      402 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/enum/tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/__init__.py
--rw-r--r--   0        0        0      180 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial001.py
--rw-r--r--   0        0        0      227 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial001_an.py
--rw-r--r--   0        0        0      202 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial002.py
--rw-r--r--   0        0        0      249 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial002_an.py
--rw-r--r--   0        0        0      321 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial003.py
--rw-r--r--   0        0        0      368 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial003_an.py
--rw-r--r--   0        0        0      547 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial004.py
--rw-r--r--   0        0        0      594 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial004_an.py
--rw-r--r--   0        0        0      205 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial005.py
--rw-r--r--   0        0        0      250 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial005_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/index/__init__.py
--rw-r--r--   0        0        0      394 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/index/tutorial001.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/number/__init__.py
--rw-r--r--   0        0        0      302 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/number/tutorial001.py
--rw-r--r--   0        0        0      369 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/number/tutorial001_an.py
--rw-r--r--   0        0        0      335 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/number/tutorial002.py
--rw-r--r--   0        0        0      402 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/number/tutorial002_an.py
--rw-r--r--   0        0        0      178 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/number/tutorial003.py
--rw-r--r--   0        0        0      229 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/number/tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/path/__init__.py
--rw-r--r--   0        0        0      530 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/path/tutorial001.py
--rw-r--r--   0        0        0      583 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/path/tutorial001_an.py
--rw-r--r--   0        0        0      372 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/path/tutorial002.py
--rw-r--r--   0        0        0      460 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/path/tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/uuid/__init__.py
--rw-r--r--   0        0        0      196 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/parameter_types/uuid/tutorial001.py
--rw-r--r--   0        0        0      296 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/printing/tutorial001.py
--rw-r--r--   0        0        0      183 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/printing/tutorial002.py
--rw-r--r--   0        0        0      296 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/printing/tutorial003.py
--rw-r--r--   0        0        0      214 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/printing/tutorial004.py
--rw-r--r--   0        0        0      365 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/printing/tutorial005.py
--rw-r--r--   0        0        0      150 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/printing/tutorial006.py
--rw-r--r--   0        0        0      315 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/progressbar/tutorial001.py
--rw-r--r--   0        0        0      476 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/progressbar/tutorial002.py
--rw-r--r--   0        0        0      313 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/progressbar/tutorial003.py
--rw-r--r--   0        0        0      455 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/progressbar/tutorial004.py
--rw-r--r--   0        0        0      333 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/progressbar/tutorial005.py
--rw-r--r--   0        0        0      336 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/progressbar/tutorial006.py
--rw-r--r--   0        0        0      162 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/prompt/tutorial001.py
--rw-r--r--   0        0        0      245 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/prompt/tutorial002.py
--rw-r--r--   0        0        0      180 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/prompt/tutorial003.py
--rw-r--r--   0        0        0      193 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/prompt/tutorial004.py
--rw-r--r--   0        0        0      304 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/callback_override/tutorial001.py
--rw-r--r--   0        0        0      306 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/callback_override/tutorial002.py
--rw-r--r--   0        0        0      409 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/callback_override/tutorial003.py
--rw-r--r--   0        0        0      533 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/callback_override/tutorial004.py
--rw-r--r--   0        0        0      254 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial001.py
--rw-r--r--   0        0        0      289 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial002.py
--rw-r--r--   0        0        0      282 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial003.py
--rw-r--r--   0        0        0      372 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial004.py
--rw-r--r--   0        0        0      473 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial005.py
--rw-r--r--   0        0        0      514 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial006.py
--rw-r--r--   0        0        0      564 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial007.py
--rw-r--r--   0        0        0      644 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial008.py
--rw-r--r--   0        0        0      298 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/tutorial001/items.py
--rw-r--r--   0        0        0      177 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/tutorial001/main.py
--rw-r--r--   0        0        0      245 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/tutorial001/users.py
--rw-r--r--   0        0        0      698 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/tutorial002/main.py
--rw-r--r--   0        0        0      298 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/tutorial003/items.py
--rw-r--r--   0        0        0      180 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/tutorial003/lands.py
--rw-r--r--   0        0        0      229 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/tutorial003/main.py
--rw-r--r--   0        0        0      233 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/tutorial003/reigns.py
--rw-r--r--   0        0        0      221 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/tutorial003/towns.py
--rw-r--r--   0        0        0      245 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/subcommands/tutorial003/users.py
--rw-r--r--   0        0        0      598 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/terminating/tutorial001.py
--rw-r--r--   0        0        0      235 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/terminating/tutorial002.py
--rw-r--r--   0        0        0      230 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/terminating/tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app01/__init__.py
--rw-r--r--   0        0        0      256 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app01/main.py
--rw-r--r--   0        0        0      299 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app01/test_main.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app02/__init__.py
--rw-r--r--   0        0        0      207 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app02/main.py
--rw-r--r--   0        0        0      284 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app02/test_main.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app02_an/__init__.py
--rw-r--r--   0        0        0      252 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app02_an/main.py
--rw-r--r--   0        0        0      284 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app02_an/test_main.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app03/__init__.py
--rw-r--r--   0        0        0      122 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app03/main.py
--rw-r--r--   0        0        0      284 2024-03-30 01:26:02.463405 typer_slim-0.12.dev1/docs_src/testing/app03/test_main.py
--rw-r--r--   0        0        0      371 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/docs_src/using_click/tutorial001.py
--rw-r--r--   0        0        0      287 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/docs_src/using_click/tutorial002.py
--rw-r--r--   0        0        0      626 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/docs_src/using_click/tutorial003.py
--rw-r--r--   0        0        0      511 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/docs_src/using_click/tutorial004.py
--rw-r--r--   0        0        0     4332 2024-03-30 01:26:04.903418 typer_slim-0.12.dev1/pyproject.toml
--rw-r--r--   0        0        0      438 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/requirements-docs.txt
--rw-r--r--   0        0        0      170 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/requirements-tests.txt
--rw-r--r--   0        0        0       90 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/requirements.txt
--rwxr-xr-x   0        0        0       76 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/build-docs.sh
--rwxr-xr-x   0        0        0       98 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/clean.sh
--rwxr-xr-x   0        0        0       68 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/docs-live.sh
--rwxr-xr-x   0        0        0      167 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/format-imports.sh
--rwxr-xr-x   0        0        0      109 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/format.sh
--rw-r--r--   0        0        0      112 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/get-pwsh-activate.sh
--rwxr-xr-x   0        0        0      114 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/lint.sh
--rwxr-xr-x   0        0        0       42 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/publish.sh
--rwxr-xr-x   0        0        0       80 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0      350 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/test-files.sh
--rwxr-xr-x   0        0        0      436 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/test.sh
--rw-r--r--   0        0        0      115 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/scripts/zip-docs.sh
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/cli/__init__.py
--rw-r--r--   0        0        0      134 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/cli/app_other_name.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/cli/empty_script.py
--rw-r--r--   0        0        0       67 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/cli/func_other_name.py
--rw-r--r--   0        0        0      622 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/cli/multi_app.py
--rw-r--r--   0        0        0      265 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/cli/multi_app_cli.py
--rw-r--r--   0        0        0      180 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/cli/multi_func.py
--rw-r--r--   0        0        0     1334 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/cli/multiapp-docs.md
--rw-r--r--   0        0        0       19 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/cli/not_python.txt
--rw-r--r--   0        0        0      412 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/cli/sample.py
--rw-r--r--   0        0        0      675 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/compat_click7_8.py
--rw-r--r--   0        0        0      542 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/completion_no_types.py
--rw-r--r--   0        0        0      542 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/completion_no_types_order.py
--rw-r--r--   0        0        0      160 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/prog_name.py
--rw-r--r--   0        0        0      157 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/type_error_no_rich.py
--rw-r--r--   0        0        0      213 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/type_error_no_rich_short_disable.py
--rw-r--r--   0        0        0      306 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/assets/type_error_normal_traceback.py
--rw-r--r--   0        0        0     6996 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_ambiguous_params.py
--rw-r--r--   0        0        0     2081 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_annotated.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/__init__.py
--rw-r--r--   0        0        0      838 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_app_other_name.py
--rw-r--r--   0        0        0      568 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_completion_run.py
--rw-r--r--   0        0        0     2592 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_doc.py
--rw-r--r--   0        0        0      402 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_empty_script.py
--rw-r--r--   0        0        0      446 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_func_other_name.py
--rw-r--r--   0        0        0      784 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_help.py
--rw-r--r--   0        0        0     2554 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_multi_app.py
--rw-r--r--   0        0        0     2110 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_multi_app_cli.py
--rw-r--r--   0        0        0      963 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_multi_app_sub.py
--rw-r--r--   0        0        0     2274 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_multi_func.py
--rw-r--r--   0        0        0      421 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_not_python.py
--rw-r--r--   0        0        0     2903 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_sub.py
--rw-r--r--   0        0        0      584 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_sub_completion.py
--rw-r--r--   0        0        0      522 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_sub_help.py
--rw-r--r--   0        0        0      269 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_cli/test_version.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_compat/__init__.py
--rw-r--r--   0        0        0     1495 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_compat/test_option_get_help.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_completion/__init__.py
--rw-r--r--   0        0        0     4979 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_completion/test_completion.py
--rw-r--r--   0        0        0     5432 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_completion/test_completion_complete.py
--rw-r--r--   0        0        0     2069 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_completion/test_completion_complete_no_help.py
--rw-r--r--   0        0        0     5650 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_completion/test_completion_install.py
--rw-r--r--   0        0        0     3966 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_completion/test_completion_show.py
--rw-r--r--   0        0        0      797 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_exit_errors.py
--rw-r--r--   0        0        0     7965 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_others.py
--rw-r--r--   0        0        0      375 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_prog_name.py
--rw-r--r--   0        0        0      849 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_rich_utils.py
--rw-r--r--   0        0        0     2031 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tracebacks.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_default/__init__.py
--rw-r--r--   0        0        0      945 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py
--rw-r--r--   0        0        0      963 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_default/test_tutorial001_an.py
--rw-r--r--   0        0        0     1071 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py
--rw-r--r--   0        0        0     1074 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_default/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/__init__.py
--rw-r--r--   0        0        0     1619 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py
--rw-r--r--   0        0        0     1622 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001_an.py
--rw-r--r--   0        0        0     1215 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py
--rw-r--r--   0        0        0     1218 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002_an.py
--rw-r--r--   0        0        0     1236 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py
--rw-r--r--   0        0        0     1239 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/__init__.py
--rw-r--r--   0        0        0     1308 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py
--rw-r--r--   0        0        0     1311 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial001_an.py
--rw-r--r--   0        0        0      953 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py
--rw-r--r--   0        0        0      956 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial002_an.py
--rw-r--r--   0        0        0      944 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py
--rw-r--r--   0        0        0      947 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial003_an.py
--rw-r--r--   0        0        0      948 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py
--rw-r--r--   0        0        0      951 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial004_an.py
--rw-r--r--   0        0        0      866 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py
--rw-r--r--   0        0        0      869 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial005_an.py
--rw-r--r--   0        0        0      850 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py
--rw-r--r--   0        0        0      853 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial006_an.py
--rw-r--r--   0        0        0      840 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py
--rw-r--r--   0        0        0      843 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial007_an.py
--rw-r--r--   0        0        0     1288 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py
--rw-r--r--   0        0        0     1291 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial008_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/__init__.py
--rw-r--r--   0        0        0     1153 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py
--rw-r--r--   0        0        0     1156 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/test_tutorial001_an.py
--rw-r--r--   0        0        0      848 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py
--rw-r--r--   0        0        0      851 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/test_tutorial002_an.py
--rw-r--r--   0        0        0     1153 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_arguments/__init__.py
--rw-r--r--   0        0        0     1043 2024-03-30 01:26:02.467405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_callback/__init__.py
--rw-r--r--   0        0        0     2167 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py
--rw-r--r--   0        0        0      589 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py
--rw-r--r--   0        0        0      706 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py
--rw-r--r--   0        0        0      829 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_context/__init__.py
--rw-r--r--   0        0        0      829 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_context/test_tutorial001.py
--rw-r--r--   0        0        0      947 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_context/test_tutorial002.py
--rw-r--r--   0        0        0      955 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_context/test_tutorial003.py
--rw-r--r--   0        0        0      714 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_context/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/__init__.py
--rw-r--r--   0        0        0     3570 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial001.py
--rw-r--r--   0        0        0     3573 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial001_an.py
--rw-r--r--   0        0        0     1644 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial002.py
--rw-r--r--   0        0        0     1103 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial003.py
--rw-r--r--   0        0        0     1804 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial004.py
--rw-r--r--   0        0        0     1809 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial004_an.py
--rw-r--r--   0        0        0     1871 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial005.py
--rw-r--r--   0        0        0     1876 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial005_an.py
--rw-r--r--   0        0        0     1575 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial006.py
--rw-r--r--   0        0        0     1672 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial007.py
--rw-r--r--   0        0        0     1675 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial007_an.py
--rw-r--r--   0        0        0      708 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial008.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_index/__init__.py
--rw-r--r--   0        0        0      660 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_index/test_tutorial001.py
--rw-r--r--   0        0        0      958 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_index/test_tutorial002.py
--rw-r--r--   0        0        0      948 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_index/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_name/__init__.py
--rw-r--r--   0        0        0      909 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_name/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_one_or_multiple/__init__.py
--rw-r--r--   0        0        0      719 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py
--rw-r--r--   0        0        0      863 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_options/__init__.py
--rw-r--r--   0        0        0     2240 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_options/test_tutorial001.py
--rw-r--r--   0        0        0     2243 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_options/test_tutorial001_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_exceptions/__init__.py
--rw-r--r--   0        0        0     1576 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_exceptions/test_tutorial001.py
--rw-r--r--   0        0        0     1588 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_exceptions/test_tutorial002.py
--rw-r--r--   0        0        0      989 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_exceptions/test_tutorial003.py
--rw-r--r--   0        0        0      935 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_exceptions/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/__init__.py
--rw-r--r--   0        0        0      526 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py
--rw-r--r--   0        0        0      696 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial002.py
--rw-r--r--   0        0        0      733 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial003.py
--rw-r--r--   0        0        0     1519 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial004.py
--rw-r--r--   0        0        0     1508 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial005.py
--rw-r--r--   0        0        0     1384 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial006.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/__init__.py
--rw-r--r--   0        0        0      722 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py
--rw-r--r--   0        0        0     1341 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py
--rw-r--r--   0        0        0     1353 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_multiple_options/__init__.py
--rw-r--r--   0        0        0     1138 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py
--rw-r--r--   0        0        0     1141 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001_an.py
--rw-r--r--   0        0        0      908 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py
--rw-r--r--   0        0        0      911 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/__init__.py
--rw-r--r--   0        0        0     1290 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py
--rw-r--r--   0        0        0     1293 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/__init__.py
--rw-r--r--   0        0        0      754 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial001.py
--rw-r--r--   0        0        0      757 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial001_an.py
--rw-r--r--   0        0        0     1265 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial003.py
--rw-r--r--   0        0        0     1274 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial003_an.py
--rw-r--r--   0        0        0     1272 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial004.py
--rw-r--r--   0        0        0     1281 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial004_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/__init__.py
--rw-r--r--   0        0        0     1299 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial001.py
--rw-r--r--   0        0        0     1302 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial001_an.py
--rw-r--r--   0        0        0     1068 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial002.py
--rw-r--r--   0        0        0     1071 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial002_an.py
--rw-r--r--   0        0        0      783 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial003.py
--rw-r--r--   0        0        0      786 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/__init__.py
--rw-r--r--   0        0        0      963 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial001.py
--rw-r--r--   0        0        0      966 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial001_an.py
--rw-r--r--   0        0        0      975 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial002.py
--rw-r--r--   0        0        0      978 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial002_an.py
--rw-r--r--   0        0        0      825 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial003.py
--rw-r--r--   0        0        0      828 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial003_an.py
--rw-r--r--   0        0        0      980 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial004.py
--rw-r--r--   0        0        0      983 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial004_an.py
--rw-r--r--   0        0        0     1309 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial005.py
--rw-r--r--   0        0        0     1312 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial005_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/__init__.py
--rw-r--r--   0        0        0     1055 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py
--rw-r--r--   0        0        0     1058 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial001_an.py
--rw-r--r--   0        0        0     1076 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py
--rw-r--r--   0        0        0     1079 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial002_an.py
--rw-r--r--   0        0        0     1353 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py
--rw-r--r--   0        0        0     1356 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_required/__init__.py
--rw-r--r--   0        0        0     1300 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_required/test_tutorial001.py
--rw-r--r--   0        0        0     1303 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_required/test_tutorial001_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_version/__init__.py
--rw-r--r--   0        0        0     1405 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_version/test_tutorial003.py
--rw-r--r--   0        0        0     1414 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_version/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/__init__.py
--rw-r--r--   0        0        0     1049 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py
--rw-r--r--   0        0        0     1058 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial002_an.py
--rw-r--r--   0        0        0     1060 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py
--rw-r--r--   0        0        0     1069 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial003_an.py
--rw-r--r--   0        0        0     1129 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py
--rw-r--r--   0        0        0     1138 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial004_an.py
--rw-r--r--   0        0        0     1215 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py
--rw-r--r--   0        0        0     1224 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial007_an.py
--rw-r--r--   0        0        0     1227 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py
--rw-r--r--   0        0        0     1236 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial008_an.py
--rw-r--r--   0        0        0     1248 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py
--rw-r--r--   0        0        0     1257 2024-03-30 01:26:02.471405 typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial009_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/__init__.py
--rw-r--r--   0        0        0     1054 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py
--rw-r--r--   0        0        0     1057 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001_an.py
--rw-r--r--   0        0        0     1576 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py
--rw-r--r--   0        0        0     1579 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002_an.py
--rw-r--r--   0        0        0      950 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py
--rw-r--r--   0        0        0      953 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003_an.py
--rw-r--r--   0        0        0     1012 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py
--rw-r--r--   0        0        0     1015 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_custom_types/__init__.py
--rw-r--r--   0        0        0      982 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001.py
--rw-r--r--   0        0        0      989 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001_an.py
--rw-r--r--   0        0        0      992 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002.py
--rw-r--r--   0        0        0      995 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_datetime/__init__.py
--rw-r--r--   0        0        0     1279 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py
--rw-r--r--   0        0        0      789 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py
--rw-r--r--   0        0        0      792 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/__init__.py
--rw-r--r--   0        0        0     1451 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py
--rw-r--r--   0        0        0      780 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py
--rw-r--r--   0        0        0      783 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002_an.py
--rw-r--r--   0        0        0     1203 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003.py
--rw-r--r--   0        0        0     1206 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/__init__.py
--rw-r--r--   0        0        0      831 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py
--rw-r--r--   0        0        0      834 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001_an.py
--rw-r--r--   0        0        0      858 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py
--rw-r--r--   0        0        0      861 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002_an.py
--rw-r--r--   0        0        0      776 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py
--rw-r--r--   0        0        0      779 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003_an.py
--rw-r--r--   0        0        0      892 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py
--rw-r--r--   0        0        0      895 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004_an.py
--rw-r--r--   0        0        0     1046 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py
--rw-r--r--   0        0        0     1049 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_index/__init__.py
--rw-r--r--   0        0        0     1338 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/__init__.py
--rw-r--r--   0        0        0     2219 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py
--rw-r--r--   0        0        0     2222 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001_an.py
--rw-r--r--   0        0        0      889 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py
--rw-r--r--   0        0        0      892 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002_an.py
--rw-r--r--   0        0        0     1377 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py
--rw-r--r--   0        0        0     1380 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_path/__init__.py
--rw-r--r--   0        0        0     1461 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py
--rw-r--r--   0        0        0     1464 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001_an.py
--rw-r--r--   0        0        0     1311 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py
--rw-r--r--   0        0        0     1314 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002_an.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_uuid/__init__.py
--rw-r--r--   0        0        0      929 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_prompt/__init__.py
--rw-r--r--   0        0        0      609 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_prompt/test_tutorial001.py
--rw-r--r--   0        0        0      885 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_prompt/test_tutorial002.py
--rw-r--r--   0        0        0      842 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_prompt/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/__init__.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_callback_override/__init__.py
--rw-r--r--   0        0        0      616 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py
--rw-r--r--   0        0        0      616 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py
--rw-r--r--   0        0        0      745 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py
--rw-r--r--   0        0        0      847 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/__init__.py
--rw-r--r--   0        0        0      952 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py
--rw-r--r--   0        0        0      952 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py
--rw-r--r--   0        0        0      952 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py
--rw-r--r--   0        0        0      952 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py
--rw-r--r--   0        0        0      994 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py
--rw-r--r--   0        0        0      944 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py
--rw-r--r--   0        0        0      977 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py
--rw-r--r--   0        0        0      990 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py
--rw-r--r--   0        0        0     2682 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_tutorial001.py
--rw-r--r--   0        0        0     2143 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_tutorial002.py
--rw-r--r--   0        0        0     5629 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_terminating/__init__.py
--rw-r--r--   0        0        0     1133 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_terminating/test_tutorial001.py
--rw-r--r--   0        0        0      721 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_terminating/test_tutorial002.py
--rw-r--r--   0        0        0     1238 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_terminating/test_tutorial003.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_testing/__init__.py
--rw-r--r--   0        0        0      388 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_testing/test_app01.py
--rw-r--r--   0        0        0      388 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_testing/test_app02.py
--rw-r--r--   0        0        0      397 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_testing/test_app02_an.py
--rw-r--r--   0        0        0      388 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_testing/test_app03.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_using_click/__init__.py
--rw-r--r--   0        0        0      996 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_using_click/test_tutorial003.py
--rw-r--r--   0        0        0      936 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_tutorial/test_using_click/test_tutorial004.py
--rw-r--r--   0        0        0     3318 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/test_type_conversion.py
--rw-r--r--   0        0        0      125 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/tests/utils.py
--rw-r--r--   0        0        0     1606 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/__init__.py
--rw-r--r--   0        0        0       30 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/__main__.py
--rw-r--r--   0        0        0     6689 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/_completion_classes.py
--rw-r--r--   0        0        0     8497 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/_completion_shared.py
--rw-r--r--   0        0        0    19727 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/_typing.py
--rw-r--r--   0        0        0     9149 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/cli.py
--rw-r--r--   0        0        0      430 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/colors.py
--rw-r--r--   0        0        0     4765 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/completion.py
--rw-r--r--   0        0        0    24283 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/core.py
--rw-r--r--   0        0        0    39496 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/main.py
--rw-r--r--   0        0        0    15908 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/models.py
--rw-r--r--   0        0        0    13787 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/params.py
--rw-r--r--   0        0        0        0 2024-03-30 01:26:02.475405 typer_slim-0.12.dev1/typer/py.typed
--rw-r--r--   0        0        0    23519 2024-03-30 01:26:02.479405 typer_slim-0.12.dev1/typer/rich_utils.py
--rw-r--r--   0        0        0      874 2024-03-30 01:26:02.479405 typer_slim-0.12.dev1/typer/testing.py
--rw-r--r--   0        0        0     7414 2024-03-30 01:26:02.479405 typer_slim-0.12.dev1/typer/utils.py
--rw-r--r--   0        0        0    15690 1970-01-01 00:00:00.000000 typer_slim-0.12.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-03-30 01:51:41.480208 typer_slim-0.12.dev2/LICENSE
+-rw-r--r--   0        0        0    13990 2024-03-30 01:51:41.480208 typer_slim-0.12.dev2/README.md
+-rw-r--r--   0        0        0      310 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/app_dir/tutorial001.py
+-rw-r--r--   0        0        0      144 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/default/tutorial001.py
+-rw-r--r--   0        0        0      197 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/default/tutorial001_an.py
+-rw-r--r--   0        0        0      252 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/default/tutorial002.py
+-rw-r--r--   0        0        0      302 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/default/tutorial002_an.py
+-rw-r--r--   0        0        0      165 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/envvar/tutorial001.py
+-rw-r--r--   0        0        0      216 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/envvar/tutorial001_an.py
+-rw-r--r--   0        0        0      179 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/envvar/tutorial002.py
+-rw-r--r--   0        0        0      237 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/envvar/tutorial002_an.py
+-rw-r--r--   0        0        0      184 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/envvar/tutorial003.py
+-rw-r--r--   0        0        0      256 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/envvar/tutorial003_an.py
+-rw-r--r--   0        0        0      172 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial001.py
+-rw-r--r--   0        0        0      217 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial001_an.py
+-rw-r--r--   0        0        0      231 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial002.py
+-rw-r--r--   0        0        0      276 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial002_an.py
+-rw-r--r--   0        0        0      218 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial003.py
+-rw-r--r--   0        0        0      269 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial003_an.py
+-rw-r--r--   0        0        0      238 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial004.py
+-rw-r--r--   0        0        0      310 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial004_an.py
+-rw-r--r--   0        0        0      232 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial005.py
+-rw-r--r--   0        0        0      314 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial005_an.py
+-rw-r--r--   0        0        0      164 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial006.py
+-rw-r--r--   0        0        0      215 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial006_an.py
+-rw-r--r--   0        0        0      447 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial007.py
+-rw-r--r--   0        0        0      523 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial007_an.py
+-rw-r--r--   0        0        0      210 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial008.py
+-rw-r--r--   0        0        0      261 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/help/tutorial008_an.py
+-rw-r--r--   0        0        0      131 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/optional/tutorial001.py
+-rw-r--r--   0        0        0      181 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/optional/tutorial001_an.py
+-rw-r--r--   0        0        0      247 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/optional/tutorial002.py
+-rw-r--r--   0        0        0      292 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/optional/tutorial002_an.py
+-rw-r--r--   0        0        0      142 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/arguments/optional/tutorial003.py
+-rw-r--r--   0        0        0      241 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/arguments/tutorial001.py
+-rw-r--r--   0        0        0      721 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/callback/tutorial001.py
+-rw-r--r--   0        0        0      216 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/callback/tutorial002.py
+-rw-r--r--   0        0        0      304 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/callback/tutorial003.py
+-rw-r--r--   0        0        0      315 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/callback/tutorial004.py
+-rw-r--r--   0        0        0      411 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/context/tutorial001.py
+-rw-r--r--   0        0        0      390 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/context/tutorial002.py
+-rw-r--r--   0        0        0      451 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/context/tutorial003.py
+-rw-r--r--   0        0        0      277 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/context/tutorial004.py
+-rw-r--r--   0        0        0     1197 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial001.py
+-rw-r--r--   0        0        0     1301 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial001_an.py
+-rw-r--r--   0        0        0      439 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial002.py
+-rw-r--r--   0        0        0      386 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial003.py
+-rw-r--r--   0        0        0      827 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial004.py
+-rw-r--r--   0        0        0      903 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial004_an.py
+-rw-r--r--   0        0        0      786 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial005.py
+-rw-r--r--   0        0        0      855 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial005_an.py
+-rw-r--r--   0        0        0     1143 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial006.py
+-rw-r--r--   0        0        0     1044 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial007.py
+-rw-r--r--   0        0        0     1200 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial007_an.py
+-rw-r--r--   0        0        0      293 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/help/tutorial008.py
+-rw-r--r--   0        0        0      138 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/index/tutorial001.py
+-rw-r--r--   0        0        0      215 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/index/tutorial002.py
+-rw-r--r--   0        0        0      235 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/index/tutorial003.py
+-rw-r--r--   0        0        0      275 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/name/tutorial001.py
+-rw-r--r--   0        0        0      187 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/one_or_multiple/tutorial001.py
+-rw-r--r--   0        0        0      287 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/one_or_multiple/tutorial002.py
+-rw-r--r--   0        0        0      708 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/options/tutorial001.py
+-rw-r--r--   0        0        0      772 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/commands/options/tutorial001_an.py
+-rw-r--r--   0        0        0      115 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/exceptions/tutorial001.py
+-rw-r--r--   0        0        0      174 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/exceptions/tutorial002.py
+-rw-r--r--   0        0        0      170 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/exceptions/tutorial003.py
+-rw-r--r--   0        0        0      171 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/exceptions/tutorial004.py
+-rw-r--r--   0        0        0      101 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/first_steps/tutorial001.py
+-rw-r--r--   0        0        0      112 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/first_steps/tutorial002.py
+-rw-r--r--   0        0        0      138 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/first_steps/tutorial003.py
+-rw-r--r--   0        0        0      239 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/first_steps/tutorial004.py
+-rw-r--r--   0        0        0      244 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/first_steps/tutorial005.py
+-rw-r--r--   0        0        0      358 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/first_steps/tutorial006.py
+-rw-r--r--   0        0        0      157 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/launch/tutorial001.py
+-rw-r--r--   0        0        0      527 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/launch/tutorial002.py
+-rw-r--r--   0        0        0      294 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/multiple_values/arguments_with_multiple_values/tutorial001.py
+-rw-r--r--   0        0        0      292 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/multiple_values/arguments_with_multiple_values/tutorial002.py
+-rw-r--r--   0        0        0      343 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/multiple_values/arguments_with_multiple_values/tutorial002_an.py
+-rw-r--r--   0        0        0      317 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/multiple_values/multiple_options/tutorial001.py
+-rw-r--r--   0        0        0      370 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/multiple_values/multiple_options/tutorial001_an.py
+-rw-r--r--   0        0        0      178 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/multiple_values/multiple_options/tutorial002.py
+-rw-r--r--   0        0        0      231 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/multiple_values/multiple_options/tutorial002_an.py
+-rw-r--r--   0        0        0      403 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/multiple_values/options_with_multiple_values/tutorial001.py
+-rw-r--r--   0        0        0      456 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/multiple_values/options_with_multiple_values/tutorial001_an.py
+-rw-r--r--   0        0        0      339 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/callback/tutorial001.py
+-rw-r--r--   0        0        0      382 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/callback/tutorial001_an.py
+-rw-r--r--   0        0        0      368 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/callback/tutorial002.py
+-rw-r--r--   0        0        0      411 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/callback/tutorial002_an.py
+-rw-r--r--   0        0        0      433 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/callback/tutorial003.py
+-rw-r--r--   0        0        0      476 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/callback/tutorial003_an.py
+-rw-r--r--   0        0        0      477 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/callback/tutorial004.py
+-rw-r--r--   0        0        0      520 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/callback/tutorial004_an.py
+-rw-r--r--   0        0        0      464 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/help/tutorial001.py
+-rw-r--r--   0        0        0      526 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/help/tutorial001_an.py
+-rw-r--r--   0        0        0      643 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/help/tutorial002.py
+-rw-r--r--   0        0        0      778 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/help/tutorial002_an.py
+-rw-r--r--   0        0        0      170 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/help/tutorial003.py
+-rw-r--r--   0        0        0      221 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/help/tutorial003_an.py
+-rw-r--r--   0        0        0      217 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/help/tutorial004.py
+-rw-r--r--   0        0        0      268 2024-03-30 01:51:41.488208 typer_slim-0.12.dev2/docs_src/options/help/tutorial004_an.py
+-rw-r--r--   0        0        0      152 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/name/tutorial001.py
+-rw-r--r--   0        0        0      197 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/name/tutorial001_an.py
+-rw-r--r--   0        0        0      158 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/name/tutorial002.py
+-rw-r--r--   0        0        0      203 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/name/tutorial002_an.py
+-rw-r--r--   0        0        0      148 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/name/tutorial003.py
+-rw-r--r--   0        0        0      193 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/name/tutorial003_an.py
+-rw-r--r--   0        0        0      163 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/name/tutorial004.py
+-rw-r--r--   0        0        0      208 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/name/tutorial004_an.py
+-rw-r--r--   0        0        0      281 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/name/tutorial005.py
+-rw-r--r--   0        0        0      337 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/name/tutorial005_an.py
+-rw-r--r--   0        0        0      212 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/password/tutorial001.py
+-rw-r--r--   0        0        0      262 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/password/tutorial001_an.py
+-rw-r--r--   0        0        0      341 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/password/tutorial002.py
+-rw-r--r--   0        0        0      386 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/password/tutorial002_an.py
+-rw-r--r--   0        0        0      171 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/prompt/tutorial001.py
+-rw-r--r--   0        0        0      216 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/prompt/tutorial001_an.py
+-rw-r--r--   0        0        0      204 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/prompt/tutorial002.py
+-rw-r--r--   0        0        0      254 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/prompt/tutorial002_an.py
+-rw-r--r--   0        0        0      198 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/prompt/tutorial003.py
+-rw-r--r--   0        0        0      250 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/prompt/tutorial003_an.py
+-rw-r--r--   0        0        0      155 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/required/tutorial001.py
+-rw-r--r--   0        0        0      205 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/required/tutorial001_an.py
+-rw-r--r--   0        0        0      166 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/required/tutorial002.py
+-rw-r--r--   0        0        0      430 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/version/tutorial001.py
+-rw-r--r--   0        0        0      494 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/version/tutorial001_an.py
+-rw-r--r--   0        0        0      566 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/version/tutorial002.py
+-rw-r--r--   0        0        0      622 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/version/tutorial002_an.py
+-rw-r--r--   0        0        0      597 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/version/tutorial003.py
+-rw-r--r--   0        0        0      662 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options/version/tutorial003_an.py
+-rw-r--r--   0        0        0      193 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial001.py
+-rw-r--r--   0        0        0      244 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial001_an.py
+-rw-r--r--   0        0        0      313 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial002.py
+-rw-r--r--   0        0        0      364 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial002_an.py
+-rw-r--r--   0        0        0      479 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial003.py
+-rw-r--r--   0        0        0      530 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial003_an.py
+-rw-r--r--   0        0        0      665 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial004.py
+-rw-r--r--   0        0        0      716 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial004_an.py
+-rw-r--r--   0        0        0      564 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial005.py
+-rw-r--r--   0        0        0      615 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial005_an.py
+-rw-r--r--   0        0        0      262 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial006.py
+-rw-r--r--   0        0        0      320 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial006_an.py
+-rw-r--r--   0        0        0      700 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial007.py
+-rw-r--r--   0        0        0      760 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial007_an.py
+-rw-r--r--   0        0        0      736 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial008.py
+-rw-r--r--   0        0        0      796 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial008_an.py
+-rw-r--r--   0        0        0      819 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial009.py
+-rw-r--r--   0        0        0      879 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial009_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/bool/__init__.py
+-rw-r--r--   0        0        0      208 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/bool/tutorial001.py
+-rw-r--r--   0        0        0      259 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/bool/tutorial001_an.py
+-rw-r--r--   0        0        0      323 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/bool/tutorial002.py
+-rw-r--r--   0        0        0      374 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/bool/tutorial002_an.py
+-rw-r--r--   0        0        0      228 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/bool/tutorial003.py
+-rw-r--r--   0        0        0      279 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/bool/tutorial003_an.py
+-rw-r--r--   0        0        0      225 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/bool/tutorial004.py
+-rw-r--r--   0        0        0      276 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/bool/tutorial004_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/custom_types/__init__.py
+-rw-r--r--   0        0        0      542 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/custom_types/tutorial001.py
+-rw-r--r--   0        0        0      605 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/custom_types/tutorial001_an.py
+-rw-r--r--   0        0        0      646 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/custom_types/tutorial002.py
+-rw-r--r--   0        0        0      721 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/custom_types/tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/datetime/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/datetime/tutorial001.py
+-rw-r--r--   0        0        0      294 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/datetime/tutorial002.py
+-rw-r--r--   0        0        0      370 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/datetime/tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/enum/__init__.py
+-rw-r--r--   0        0        0      299 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/enum/tutorial001.py
+-rw-r--r--   0        0        0      342 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/enum/tutorial002.py
+-rw-r--r--   0        0        0      407 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/enum/tutorial002_an.py
+-rw-r--r--   0        0        0      349 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/enum/tutorial003.py
+-rw-r--r--   0        0        0      402 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/enum/tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/__init__.py
+-rw-r--r--   0        0        0      180 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial001.py
+-rw-r--r--   0        0        0      227 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial001_an.py
+-rw-r--r--   0        0        0      202 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial002.py
+-rw-r--r--   0        0        0      249 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial002_an.py
+-rw-r--r--   0        0        0      321 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial003.py
+-rw-r--r--   0        0        0      368 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial003_an.py
+-rw-r--r--   0        0        0      547 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial004.py
+-rw-r--r--   0        0        0      594 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial004_an.py
+-rw-r--r--   0        0        0      205 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial005.py
+-rw-r--r--   0        0        0      250 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial005_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/index/__init__.py
+-rw-r--r--   0        0        0      394 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/index/tutorial001.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/number/__init__.py
+-rw-r--r--   0        0        0      302 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/number/tutorial001.py
+-rw-r--r--   0        0        0      369 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/number/tutorial001_an.py
+-rw-r--r--   0        0        0      335 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/number/tutorial002.py
+-rw-r--r--   0        0        0      402 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/number/tutorial002_an.py
+-rw-r--r--   0        0        0      178 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/number/tutorial003.py
+-rw-r--r--   0        0        0      229 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/number/tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/path/__init__.py
+-rw-r--r--   0        0        0      530 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/path/tutorial001.py
+-rw-r--r--   0        0        0      583 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/path/tutorial001_an.py
+-rw-r--r--   0        0        0      372 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/path/tutorial002.py
+-rw-r--r--   0        0        0      460 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/path/tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/uuid/__init__.py
+-rw-r--r--   0        0        0      196 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/parameter_types/uuid/tutorial001.py
+-rw-r--r--   0        0        0      296 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/printing/tutorial001.py
+-rw-r--r--   0        0        0      183 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/printing/tutorial002.py
+-rw-r--r--   0        0        0      296 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/printing/tutorial003.py
+-rw-r--r--   0        0        0      214 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/printing/tutorial004.py
+-rw-r--r--   0        0        0      365 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/printing/tutorial005.py
+-rw-r--r--   0        0        0      150 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/printing/tutorial006.py
+-rw-r--r--   0        0        0      315 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/progressbar/tutorial001.py
+-rw-r--r--   0        0        0      476 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/progressbar/tutorial002.py
+-rw-r--r--   0        0        0      313 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/progressbar/tutorial003.py
+-rw-r--r--   0        0        0      455 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/progressbar/tutorial004.py
+-rw-r--r--   0        0        0      333 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/progressbar/tutorial005.py
+-rw-r--r--   0        0        0      336 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/progressbar/tutorial006.py
+-rw-r--r--   0        0        0      162 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/prompt/tutorial001.py
+-rw-r--r--   0        0        0      245 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/prompt/tutorial002.py
+-rw-r--r--   0        0        0      180 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/prompt/tutorial003.py
+-rw-r--r--   0        0        0      193 2024-03-30 01:51:41.492208 typer_slim-0.12.dev2/docs_src/prompt/tutorial004.py
+-rw-r--r--   0        0        0      304 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/callback_override/tutorial001.py
+-rw-r--r--   0        0        0      306 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/callback_override/tutorial002.py
+-rw-r--r--   0        0        0      409 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/callback_override/tutorial003.py
+-rw-r--r--   0        0        0      533 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/callback_override/tutorial004.py
+-rw-r--r--   0        0        0      254 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial001.py
+-rw-r--r--   0        0        0      289 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial002.py
+-rw-r--r--   0        0        0      282 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial003.py
+-rw-r--r--   0        0        0      372 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial004.py
+-rw-r--r--   0        0        0      473 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial005.py
+-rw-r--r--   0        0        0      514 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial006.py
+-rw-r--r--   0        0        0      564 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial007.py
+-rw-r--r--   0        0        0      644 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial008.py
+-rw-r--r--   0        0        0      298 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/tutorial001/items.py
+-rw-r--r--   0        0        0      177 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/tutorial001/main.py
+-rw-r--r--   0        0        0      245 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/tutorial001/users.py
+-rw-r--r--   0        0        0      698 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/tutorial002/main.py
+-rw-r--r--   0        0        0      298 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/tutorial003/items.py
+-rw-r--r--   0        0        0      180 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/tutorial003/lands.py
+-rw-r--r--   0        0        0      229 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/tutorial003/main.py
+-rw-r--r--   0        0        0      233 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/tutorial003/reigns.py
+-rw-r--r--   0        0        0      221 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/tutorial003/towns.py
+-rw-r--r--   0        0        0      245 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/subcommands/tutorial003/users.py
+-rw-r--r--   0        0        0      598 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/terminating/tutorial001.py
+-rw-r--r--   0        0        0      235 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/terminating/tutorial002.py
+-rw-r--r--   0        0        0      230 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/terminating/tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app01/__init__.py
+-rw-r--r--   0        0        0      256 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app01/main.py
+-rw-r--r--   0        0        0      299 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app01/test_main.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app02/__init__.py
+-rw-r--r--   0        0        0      207 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app02/main.py
+-rw-r--r--   0        0        0      284 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app02/test_main.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app02_an/__init__.py
+-rw-r--r--   0        0        0      252 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app02_an/main.py
+-rw-r--r--   0        0        0      284 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app02_an/test_main.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app03/__init__.py
+-rw-r--r--   0        0        0      122 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app03/main.py
+-rw-r--r--   0        0        0      284 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/testing/app03/test_main.py
+-rw-r--r--   0        0        0      371 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/using_click/tutorial001.py
+-rw-r--r--   0        0        0      287 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/using_click/tutorial002.py
+-rw-r--r--   0        0        0      626 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/using_click/tutorial003.py
+-rw-r--r--   0        0        0      511 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/docs_src/using_click/tutorial004.py
+-rw-r--r--   0        0        0     4332 2024-03-30 01:51:46.336234 typer_slim-0.12.dev2/pyproject.toml
+-rw-r--r--   0        0        0      438 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/requirements-docs.txt
+-rw-r--r--   0        0        0      170 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/requirements-tests.txt
+-rw-r--r--   0        0        0       90 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/requirements.txt
+-rwxr-xr-x   0        0        0       76 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/build-docs.sh
+-rwxr-xr-x   0        0        0       98 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/clean.sh
+-rwxr-xr-x   0        0        0       68 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/docs-live.sh
+-rwxr-xr-x   0        0        0      167 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/format-imports.sh
+-rwxr-xr-x   0        0        0      109 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/format.sh
+-rw-r--r--   0        0        0      112 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/get-pwsh-activate.sh
+-rwxr-xr-x   0        0        0      114 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/lint.sh
+-rwxr-xr-x   0        0        0       42 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/publish.sh
+-rwxr-xr-x   0        0        0       80 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0      350 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/test-files.sh
+-rwxr-xr-x   0        0        0      436 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/test.sh
+-rw-r--r--   0        0        0      115 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/scripts/zip-docs.sh
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/cli/__init__.py
+-rw-r--r--   0        0        0      134 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/cli/app_other_name.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/cli/empty_script.py
+-rw-r--r--   0        0        0       67 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/cli/func_other_name.py
+-rw-r--r--   0        0        0      622 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/cli/multi_app.py
+-rw-r--r--   0        0        0      265 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/cli/multi_app_cli.py
+-rw-r--r--   0        0        0      180 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/cli/multi_func.py
+-rw-r--r--   0        0        0     1334 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/cli/multiapp-docs.md
+-rw-r--r--   0        0        0       19 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/cli/not_python.txt
+-rw-r--r--   0        0        0      412 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/cli/sample.py
+-rw-r--r--   0        0        0      675 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/compat_click7_8.py
+-rw-r--r--   0        0        0      542 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/completion_no_types.py
+-rw-r--r--   0        0        0      542 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/completion_no_types_order.py
+-rw-r--r--   0        0        0      160 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/prog_name.py
+-rw-r--r--   0        0        0      157 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/type_error_no_rich.py
+-rw-r--r--   0        0        0      213 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/type_error_no_rich_short_disable.py
+-rw-r--r--   0        0        0      306 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/assets/type_error_normal_traceback.py
+-rw-r--r--   0        0        0     6996 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_ambiguous_params.py
+-rw-r--r--   0        0        0     2081 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_annotated.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/__init__.py
+-rw-r--r--   0        0        0      838 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_app_other_name.py
+-rw-r--r--   0        0        0      521 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_completion_run.py
+-rw-r--r--   0        0        0     2592 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_doc.py
+-rw-r--r--   0        0        0      402 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_empty_script.py
+-rw-r--r--   0        0        0      446 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_func_other_name.py
+-rw-r--r--   0        0        0      784 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_help.py
+-rw-r--r--   0        0        0     2554 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_multi_app.py
+-rw-r--r--   0        0        0     2110 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_multi_app_cli.py
+-rw-r--r--   0        0        0      963 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_multi_app_sub.py
+-rw-r--r--   0        0        0     2274 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_multi_func.py
+-rw-r--r--   0        0        0      421 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_not_python.py
+-rw-r--r--   0        0        0     2903 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_sub.py
+-rw-r--r--   0        0        0      537 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_sub_completion.py
+-rw-r--r--   0        0        0      522 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_sub_help.py
+-rw-r--r--   0        0        0      269 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_cli/test_version.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_compat/__init__.py
+-rw-r--r--   0        0        0     1448 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_compat/test_option_get_help.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_completion/__init__.py
+-rw-r--r--   0        0        0     4603 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_completion/test_completion.py
+-rw-r--r--   0        0        0     4962 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_completion/test_completion_complete.py
+-rw-r--r--   0        0        0     1881 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_completion/test_completion_complete_no_help.py
+-rw-r--r--   0        0        0     5462 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_completion/test_completion_install.py
+-rw-r--r--   0        0        0     3684 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_completion/test_completion_show.py
+-rw-r--r--   0        0        0      797 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_exit_errors.py
+-rw-r--r--   0        0        0     7871 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_others.py
+-rw-r--r--   0        0        0      375 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_prog_name.py
+-rw-r--r--   0        0        0      849 2024-03-30 01:51:41.496209 typer_slim-0.12.dev2/tests/test_rich_utils.py
+-rw-r--r--   0        0        0     2031 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tracebacks.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_default/__init__.py
+-rw-r--r--   0        0        0      945 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py
+-rw-r--r--   0        0        0      963 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_default/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1071 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py
+-rw-r--r--   0        0        0     1074 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_default/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/__init__.py
+-rw-r--r--   0        0        0     1619 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py
+-rw-r--r--   0        0        0     1622 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1215 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py
+-rw-r--r--   0        0        0     1218 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1236 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py
+-rw-r--r--   0        0        0     1239 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/__init__.py
+-rw-r--r--   0        0        0     1308 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0     1311 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial001_an.py
+-rw-r--r--   0        0        0      953 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0      956 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial002_an.py
+-rw-r--r--   0        0        0      944 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0      947 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial003_an.py
+-rw-r--r--   0        0        0      948 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py
+-rw-r--r--   0        0        0      951 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial004_an.py
+-rw-r--r--   0        0        0      866 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py
+-rw-r--r--   0        0        0      869 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial005_an.py
+-rw-r--r--   0        0        0      850 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py
+-rw-r--r--   0        0        0      853 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial006_an.py
+-rw-r--r--   0        0        0      840 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py
+-rw-r--r--   0        0        0      843 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial007_an.py
+-rw-r--r--   0        0        0     1288 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py
+-rw-r--r--   0        0        0     1291 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial008_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/__init__.py
+-rw-r--r--   0        0        0     1153 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py
+-rw-r--r--   0        0        0     1156 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/test_tutorial001_an.py
+-rw-r--r--   0        0        0      848 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py
+-rw-r--r--   0        0        0      851 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1153 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_arguments/__init__.py
+-rw-r--r--   0        0        0     1043 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_callback/__init__.py
+-rw-r--r--   0        0        0     2167 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py
+-rw-r--r--   0        0        0      589 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py
+-rw-r--r--   0        0        0      706 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py
+-rw-r--r--   0        0        0      829 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_context/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_context/test_tutorial001.py
+-rw-r--r--   0        0        0      947 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_context/test_tutorial002.py
+-rw-r--r--   0        0        0      955 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_context/test_tutorial003.py
+-rw-r--r--   0        0        0      714 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_context/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/__init__.py
+-rw-r--r--   0        0        0     3570 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0     3573 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1644 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0     1103 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0     1804 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial004.py
+-rw-r--r--   0        0        0     1809 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial004_an.py
+-rw-r--r--   0        0        0     1871 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial005.py
+-rw-r--r--   0        0        0     1876 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial005_an.py
+-rw-r--r--   0        0        0     1575 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial006.py
+-rw-r--r--   0        0        0     1672 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial007.py
+-rw-r--r--   0        0        0     1675 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial007_an.py
+-rw-r--r--   0        0        0      708 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial008.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_index/__init__.py
+-rw-r--r--   0        0        0      660 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_index/test_tutorial001.py
+-rw-r--r--   0        0        0      958 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_index/test_tutorial002.py
+-rw-r--r--   0        0        0      948 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_index/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_name/__init__.py
+-rw-r--r--   0        0        0      909 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_name/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_one_or_multiple/__init__.py
+-rw-r--r--   0        0        0      719 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py
+-rw-r--r--   0        0        0      863 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_options/__init__.py
+-rw-r--r--   0        0        0     2240 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_options/test_tutorial001.py
+-rw-r--r--   0        0        0     2243 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_options/test_tutorial001_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_exceptions/__init__.py
+-rw-r--r--   0        0        0     1576 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_exceptions/test_tutorial001.py
+-rw-r--r--   0        0        0     1588 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_exceptions/test_tutorial002.py
+-rw-r--r--   0        0        0      989 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_exceptions/test_tutorial003.py
+-rw-r--r--   0        0        0      935 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_exceptions/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/__init__.py
+-rw-r--r--   0        0        0      526 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial001.py
+-rw-r--r--   0        0        0      696 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial002.py
+-rw-r--r--   0        0        0      733 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial003.py
+-rw-r--r--   0        0        0     1519 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial004.py
+-rw-r--r--   0        0        0     1508 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial005.py
+-rw-r--r--   0        0        0     1384 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial006.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/__init__.py
+-rw-r--r--   0        0        0      722 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py
+-rw-r--r--   0        0        0     1341 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py
+-rw-r--r--   0        0        0     1353 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_multiple_options/__init__.py
+-rw-r--r--   0        0        0     1138 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py
+-rw-r--r--   0        0        0     1141 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001_an.py
+-rw-r--r--   0        0        0      908 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py
+-rw-r--r--   0        0        0      911 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/__init__.py
+-rw-r--r--   0        0        0     1290 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py
+-rw-r--r--   0        0        0     1293 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/__init__.py
+-rw-r--r--   0        0        0      754 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial001.py
+-rw-r--r--   0        0        0      757 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1218 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial003.py
+-rw-r--r--   0        0        0     1227 2024-03-30 01:51:41.500208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial003_an.py
+-rw-r--r--   0        0        0     1225 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial004.py
+-rw-r--r--   0        0        0     1234 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial004_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/__init__.py
+-rw-r--r--   0        0        0     1299 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial001.py
+-rw-r--r--   0        0        0     1302 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1068 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial002.py
+-rw-r--r--   0        0        0     1071 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial002_an.py
+-rw-r--r--   0        0        0      783 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial003.py
+-rw-r--r--   0        0        0      786 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/__init__.py
+-rw-r--r--   0        0        0      963 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial001.py
+-rw-r--r--   0        0        0      966 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial001_an.py
+-rw-r--r--   0        0        0      975 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial002.py
+-rw-r--r--   0        0        0      978 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial002_an.py
+-rw-r--r--   0        0        0      825 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial003.py
+-rw-r--r--   0        0        0      828 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial003_an.py
+-rw-r--r--   0        0        0      980 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial004.py
+-rw-r--r--   0        0        0      983 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial004_an.py
+-rw-r--r--   0        0        0     1309 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial005.py
+-rw-r--r--   0        0        0     1312 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial005_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/__init__.py
+-rw-r--r--   0        0        0     1055 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py
+-rw-r--r--   0        0        0     1058 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1076 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py
+-rw-r--r--   0        0        0     1079 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1353 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py
+-rw-r--r--   0        0        0     1356 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_required/__init__.py
+-rw-r--r--   0        0        0     1300 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_required/test_tutorial001.py
+-rw-r--r--   0        0        0     1303 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_required/test_tutorial001_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_version/__init__.py
+-rw-r--r--   0        0        0     1358 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_version/test_tutorial003.py
+-rw-r--r--   0        0        0     1367 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_version/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/__init__.py
+-rw-r--r--   0        0        0     1002 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py
+-rw-r--r--   0        0        0     1011 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1013 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py
+-rw-r--r--   0        0        0     1022 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial003_an.py
+-rw-r--r--   0        0        0     1082 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py
+-rw-r--r--   0        0        0     1091 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial004_an.py
+-rw-r--r--   0        0        0     1168 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py
+-rw-r--r--   0        0        0     1177 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial007_an.py
+-rw-r--r--   0        0        0     1180 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py
+-rw-r--r--   0        0        0     1189 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial008_an.py
+-rw-r--r--   0        0        0     1201 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py
+-rw-r--r--   0        0        0     1210 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial009_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/__init__.py
+-rw-r--r--   0        0        0     1054 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py
+-rw-r--r--   0        0        0     1057 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1576 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py
+-rw-r--r--   0        0        0     1579 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002_an.py
+-rw-r--r--   0        0        0      950 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py
+-rw-r--r--   0        0        0      953 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003_an.py
+-rw-r--r--   0        0        0     1012 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py
+-rw-r--r--   0        0        0     1015 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_custom_types/__init__.py
+-rw-r--r--   0        0        0      982 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001.py
+-rw-r--r--   0        0        0      989 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001_an.py
+-rw-r--r--   0        0        0      992 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002.py
+-rw-r--r--   0        0        0      995 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_datetime/__init__.py
+-rw-r--r--   0        0        0     1279 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py
+-rw-r--r--   0        0        0      789 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py
+-rw-r--r--   0        0        0      792 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/__init__.py
+-rw-r--r--   0        0        0     1451 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py
+-rw-r--r--   0        0        0      780 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py
+-rw-r--r--   0        0        0      783 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1203 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003.py
+-rw-r--r--   0        0        0     1206 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/__init__.py
+-rw-r--r--   0        0        0      831 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py
+-rw-r--r--   0        0        0      834 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001_an.py
+-rw-r--r--   0        0        0      858 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py
+-rw-r--r--   0        0        0      861 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002_an.py
+-rw-r--r--   0        0        0      776 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py
+-rw-r--r--   0        0        0      779 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003_an.py
+-rw-r--r--   0        0        0      892 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py
+-rw-r--r--   0        0        0      895 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004_an.py
+-rw-r--r--   0        0        0     1046 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py
+-rw-r--r--   0        0        0     1049 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_index/__init__.py
+-rw-r--r--   0        0        0     1338 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/__init__.py
+-rw-r--r--   0        0        0     2219 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py
+-rw-r--r--   0        0        0     2222 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001_an.py
+-rw-r--r--   0        0        0      889 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py
+-rw-r--r--   0        0        0      892 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002_an.py
+-rw-r--r--   0        0        0     1377 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py
+-rw-r--r--   0        0        0     1380 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_path/__init__.py
+-rw-r--r--   0        0        0     1461 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py
+-rw-r--r--   0        0        0     1464 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001_an.py
+-rw-r--r--   0        0        0     1311 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py
+-rw-r--r--   0        0        0     1314 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002_an.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_uuid/__init__.py
+-rw-r--r--   0        0        0      929 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_prompt/__init__.py
+-rw-r--r--   0        0        0      609 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_prompt/test_tutorial001.py
+-rw-r--r--   0        0        0      885 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_prompt/test_tutorial002.py
+-rw-r--r--   0        0        0      842 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_prompt/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_callback_override/__init__.py
+-rw-r--r--   0        0        0      616 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py
+-rw-r--r--   0        0        0      616 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py
+-rw-r--r--   0        0        0      745 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py
+-rw-r--r--   0        0        0      847 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/__init__.py
+-rw-r--r--   0        0        0      952 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py
+-rw-r--r--   0        0        0      952 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py
+-rw-r--r--   0        0        0      952 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py
+-rw-r--r--   0        0        0      952 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py
+-rw-r--r--   0        0        0      994 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py
+-rw-r--r--   0        0        0      944 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py
+-rw-r--r--   0        0        0      977 2024-03-30 01:51:41.504208 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py
+-rw-r--r--   0        0        0      990 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py
+-rw-r--r--   0        0        0     2682 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_tutorial001.py
+-rw-r--r--   0        0        0     2143 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_tutorial002.py
+-rw-r--r--   0        0        0     5629 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_terminating/__init__.py
+-rw-r--r--   0        0        0     1133 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_terminating/test_tutorial001.py
+-rw-r--r--   0        0        0      721 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_terminating/test_tutorial002.py
+-rw-r--r--   0        0        0     1238 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_terminating/test_tutorial003.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_testing/__init__.py
+-rw-r--r--   0        0        0      388 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_testing/test_app01.py
+-rw-r--r--   0        0        0      388 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_testing/test_app02.py
+-rw-r--r--   0        0        0      397 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_testing/test_app02_an.py
+-rw-r--r--   0        0        0      388 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_testing/test_app03.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_using_click/__init__.py
+-rw-r--r--   0        0        0      996 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_using_click/test_tutorial003.py
+-rw-r--r--   0        0        0      936 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_tutorial/test_using_click/test_tutorial004.py
+-rw-r--r--   0        0        0     3318 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/test_type_conversion.py
+-rw-r--r--   0        0        0      125 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/tests/utils.py
+-rw-r--r--   0        0        0     1606 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/__init__.py
+-rw-r--r--   0        0        0       30 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/__main__.py
+-rw-r--r--   0        0        0     6689 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/_completion_classes.py
+-rw-r--r--   0        0        0     8497 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/_completion_shared.py
+-rw-r--r--   0        0        0    19727 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/_typing.py
+-rw-r--r--   0        0        0     9149 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/cli.py
+-rw-r--r--   0        0        0      430 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/colors.py
+-rw-r--r--   0        0        0     4765 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/completion.py
+-rw-r--r--   0        0        0    24283 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/core.py
+-rw-r--r--   0        0        0    39496 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/main.py
+-rw-r--r--   0        0        0    15908 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/models.py
+-rw-r--r--   0        0        0    13787 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/params.py
+-rw-r--r--   0        0        0        0 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/py.typed
+-rw-r--r--   0        0        0    23519 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/rich_utils.py
+-rw-r--r--   0        0        0      874 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/testing.py
+-rw-r--r--   0        0        0     7414 2024-03-30 01:51:41.508209 typer_slim-0.12.dev2/typer/utils.py
+-rw-r--r--   0        0        0    15690 1970-01-01 00:00:00.000000 typer_slim-0.12.dev2/PKG-INFO
```

### Comparing `typer_slim-0.12.dev1/LICENSE` & `typer_slim-0.12.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/README.md` & `typer_slim-0.12.dev2/README.md`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/arguments/help/tutorial007_an.py` & `typer_slim-0.12.dev2/docs_src/arguments/help/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/callback/tutorial001.py` & `typer_slim-0.12.dev2/docs_src/commands/callback/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/help/tutorial001.py` & `typer_slim-0.12.dev2/docs_src/commands/help/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/help/tutorial001_an.py` & `typer_slim-0.12.dev2/docs_src/commands/help/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/help/tutorial004.py` & `typer_slim-0.12.dev2/docs_src/commands/help/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/help/tutorial004_an.py` & `typer_slim-0.12.dev2/docs_src/commands/help/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/help/tutorial005.py` & `typer_slim-0.12.dev2/docs_src/commands/help/tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/help/tutorial005_an.py` & `typer_slim-0.12.dev2/docs_src/commands/help/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/help/tutorial006.py` & `typer_slim-0.12.dev2/docs_src/commands/help/tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/help/tutorial007.py` & `typer_slim-0.12.dev2/docs_src/commands/help/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/help/tutorial007_an.py` & `typer_slim-0.12.dev2/docs_src/commands/help/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/options/tutorial001.py` & `typer_slim-0.12.dev2/docs_src/commands/options/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/commands/options/tutorial001_an.py` & `typer_slim-0.12.dev2/docs_src/commands/options/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/launch/tutorial002.py` & `typer_slim-0.12.dev2/docs_src/launch/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options/callback/tutorial004_an.py` & `typer_slim-0.12.dev2/docs_src/options/callback/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options/help/tutorial001_an.py` & `typer_slim-0.12.dev2/docs_src/options/help/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options/help/tutorial002.py` & `typer_slim-0.12.dev2/docs_src/options/help/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options/help/tutorial002_an.py` & `typer_slim-0.12.dev2/docs_src/options/help/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options/version/tutorial002.py` & `typer_slim-0.12.dev2/docs_src/options/version/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options/version/tutorial002_an.py` & `typer_slim-0.12.dev2/docs_src/options/version/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options/version/tutorial003.py` & `typer_slim-0.12.dev2/docs_src/options/version/tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options/version/tutorial003_an.py` & `typer_slim-0.12.dev2/docs_src/options/version/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial003_an.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial004.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial004_an.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial005.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial005_an.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial007.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial007_an.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial008.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial008_an.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial009.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial009.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/options_autocompletion/tutorial009_an.py` & `typer_slim-0.12.dev2/docs_src/options_autocompletion/tutorial009_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/parameter_types/custom_types/tutorial001.py` & `typer_slim-0.12.dev2/docs_src/parameter_types/custom_types/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/parameter_types/custom_types/tutorial001_an.py` & `typer_slim-0.12.dev2/docs_src/parameter_types/custom_types/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/parameter_types/custom_types/tutorial002.py` & `typer_slim-0.12.dev2/docs_src/parameter_types/custom_types/tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/parameter_types/custom_types/tutorial002_an.py` & `typer_slim-0.12.dev2/docs_src/parameter_types/custom_types/tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial004.py` & `typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/parameter_types/file/tutorial004_an.py` & `typer_slim-0.12.dev2/docs_src/parameter_types/file/tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/parameter_types/path/tutorial001.py` & `typer_slim-0.12.dev2/docs_src/parameter_types/path/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/parameter_types/path/tutorial001_an.py` & `typer_slim-0.12.dev2/docs_src/parameter_types/path/tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/subcommands/callback_override/tutorial004.py` & `typer_slim-0.12.dev2/docs_src/subcommands/callback_override/tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial006.py` & `typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial007.py` & `typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/subcommands/name_help/tutorial008.py` & `typer_slim-0.12.dev2/docs_src/subcommands/name_help/tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/subcommands/tutorial002/main.py` & `typer_slim-0.12.dev2/docs_src/subcommands/tutorial002/main.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/terminating/tutorial001.py` & `typer_slim-0.12.dev2/docs_src/terminating/tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/docs_src/using_click/tutorial003.py` & `typer_slim-0.12.dev2/docs_src/using_click/tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/pyproject.toml` & `typer_slim-0.12.dev2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "click >= 8.0.0",
     "typing-extensions >= 3.7.4.3",
 ]
-version = "0.12.dev1"
+version = "0.12.dev2"
 
 [project.urls]
 Documentation = "https://typer.tiangolo.com/"
 homepage = "https://github.com/tiangolo/typer"
 
 [project.optional-dependencies]
 all = [
```

### Comparing `typer_slim-0.12.dev1/tests/assets/cli/multi_app.py` & `typer_slim-0.12.dev2/tests/assets/cli/multi_app.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/assets/cli/multiapp-docs.md` & `typer_slim-0.12.dev2/tests/assets/cli/multiapp-docs.md`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/assets/compat_click7_8.py` & `typer_slim-0.12.dev2/tests/assets/compat_click7_8.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/assets/completion_no_types.py` & `typer_slim-0.12.dev2/tests/assets/completion_no_types.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/assets/completion_no_types_order.py` & `typer_slim-0.12.dev2/tests/assets/completion_no_types_order.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_ambiguous_params.py` & `typer_slim-0.12.dev2/tests/test_ambiguous_params.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_annotated.py` & `typer_slim-0.12.dev2/tests/test_annotated.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_app_other_name.py` & `typer_slim-0.12.dev2/tests/test_cli/test_app_other_name.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_completion_run.py` & `typer_slim-0.12.dev2/tests/test_cli/test_completion_run.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,11 +10,10 @@
         encoding="utf-8",
         env={
             **os.environ,
             "___MAIN__.PY_COMPLETE": "complete_bash",
             "_PYTHON _M TYPER_COMPLETE": "complete_bash",
             "COMP_WORDS": "typer tests/assets/cli/sample.py",
             "COMP_CWORD": "2",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "run" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_doc.py` & `typer_slim-0.12.dev2/tests/test_cli/test_doc.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_help.py` & `typer_slim-0.12.dev2/tests/test_cli/test_help.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_multi_app.py` & `typer_slim-0.12.dev2/tests/test_cli/test_multi_app.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_multi_app_cli.py` & `typer_slim-0.12.dev2/tests/test_cli/test_multi_app_cli.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_multi_app_sub.py` & `typer_slim-0.12.dev2/tests/test_cli/test_multi_app_sub.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_multi_func.py` & `typer_slim-0.12.dev2/tests/test_cli/test_multi_func.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_sub.py` & `typer_slim-0.12.dev2/tests/test_cli/test_sub.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_sub_completion.py` & `typer_slim-0.12.dev2/tests/test_cli/test_sub_completion.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,11 +10,10 @@
         encoding="utf-8",
         env={
             **os.environ,
             "___MAIN__.PY_COMPLETE": "complete_bash",
             "_PYTHON _M TYPER_COMPLETE": "complete_bash",
             "COMP_WORDS": "typer tests/assets/cli/sample.py run hello --",
             "COMP_CWORD": "4",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "--name" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_cli/test_sub_help.py` & `typer_slim-0.12.dev2/tests/test_cli/test_sub_help.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_compat/test_option_get_help.py` & `typer_slim-0.12.dev2/tests/test_compat/test_option_get_help.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,11 +44,10 @@
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_COMPAT_CLICK7_8.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "compat_click7_8.py --nickname ",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "Jonny" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_completion/test_completion.py` & `typer_slim-0.12.dev2/tests/test_completion/test_completion.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,30 +47,28 @@
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "sourcebash",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert result.returncode != 0
     assert "Invalid completion instruction." in result.stderr
 
 
 def test_completion_source_bash():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_bash",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert (
         "complete -o default -F _tutorial001py_completion tutorial001.py"
         in result.stdout
     )
 
@@ -79,71 +77,66 @@
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_xxx",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "Shell xxx not supported." in result.stderr
 
 
 def test_completion_source_invalid_instruction():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "explode_bash",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert 'Completion instruction "explode" not supported.' in result.stderr
 
 
 def test_completion_source_zsh():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_zsh",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "compdef _tutorial001py_completion tutorial001.py" in result.stdout
 
 
 def test_completion_source_fish():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_fish",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "complete --command tutorial001.py --no-files" in result.stdout
 
 
 def test_completion_source_powershell():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_powershell",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert (
         "Register-ArgumentCompleter -Native -CommandName tutorial001.py -ScriptBlock $scriptblock"
         in result.stdout
     )
 
@@ -152,14 +145,13 @@
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "source_pwsh",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert (
         "Register-ArgumentCompleter -Native -CommandName tutorial001.py -ScriptBlock $scriptblock"
         in result.stdout
     )
```

### Comparing `typer_slim-0.12.dev1/tests/test_completion/test_completion_complete.py` & `typer_slim-0.12.dev2/tests/test_completion/test_completion_complete.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,14 @@
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_bash",
             "COMP_WORDS": "tutorial001.py del",
             "COMP_CWORD": "1",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "delete\ndelete-all" in result.stdout
 
 
 def test_completion_complete_subcommand_bash_invalid():
     result = subprocess.run(
@@ -27,30 +26,28 @@
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_bash",
             "COMP_WORDS": "tutorial001.py del",
             "COMP_CWORD": "42",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "create\ndelete\ndelete-all\ninit" in result.stdout
 
 
 def test_completion_complete_subcommand_zsh():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert (
         """_arguments '*: :(("delete":"Delete a user with USERNAME."\n"""
         """\"delete-all":"Delete ALL users in the database."))'"""
     ) in result.stdout
 
@@ -60,15 +57,14 @@
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py delete ",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert ("_files") in result.stdout
 
 
 def test_completion_complete_subcommand_fish():
     result = subprocess.run(
@@ -76,15 +72,14 @@
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_fish",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
             "_TYPER_COMPLETE_FISH_ACTION": "get-args",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert (
         "delete\tDelete a user with USERNAME.\ndelete-all\tDelete ALL users in the database."
         in result.stdout
     )
 
@@ -95,15 +90,14 @@
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_fish",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
             "_TYPER_COMPLETE_FISH_ACTION": "is-args",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert result.returncode == 0
 
 
 def test_completion_complete_subcommand_fish_should_complete_no():
     result = subprocess.run(
@@ -111,30 +105,28 @@
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_fish",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py delete ",
             "_TYPER_COMPLETE_FISH_ACTION": "is-args",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert result.returncode != 0
 
 
 def test_completion_complete_subcommand_powershell():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_powershell",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert (
         "delete:::Delete a user with USERNAME.\ndelete-all:::Delete ALL users in the database."
     ) in result.stdout
 
 
@@ -143,15 +135,14 @@
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_pwsh",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert (
         "delete:::Delete a user with USERNAME.\ndelete-all:::Delete ALL users in the database."
     ) in result.stdout
 
 
@@ -160,11 +151,10 @@
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL001.PY_COMPLETE": "complete_noshell",
             "_TYPER_COMPLETE_ARGS": "tutorial001.py del",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert ("") in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_completion/test_completion_complete_no_help.py` & `typer_slim-0.12.dev2/tests/test_completion/test_completion_complete_no_help.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL002.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial002.py ",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "create" in result.stdout
     assert "delete" in result.stdout
 
 
 def test_completion_complete_subcommand_fish():
@@ -27,41 +26,38 @@
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL002.PY_COMPLETE": "complete_fish",
             "_TYPER_COMPLETE_ARGS": "tutorial002.py ",
             "_TYPER_COMPLETE_FISH_ACTION": "get-args",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "create\ndelete" in result.stdout
 
 
 def test_completion_complete_subcommand_powershell():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL002.PY_COMPLETE": "complete_powershell",
             "_TYPER_COMPLETE_ARGS": "tutorial002.py ",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert ("create::: \ndelete::: ") in result.stdout
 
 
 def test_completion_complete_subcommand_pwsh():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL002.PY_COMPLETE": "complete_pwsh",
             "_TYPER_COMPLETE_ARGS": "tutorial002.py ",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert ("create::: \ndelete::: ") in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_completion/test_completion_install.py` & `typer_slim-0.12.dev2/tests/test_completion/test_completion_install.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 def test_completion_install_no_shell():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, "--install-completion"],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     assert "Option '--install-completion' requires an argument" in result.stderr
 
 
 def test_completion_install_bash():
@@ -44,15 +43,14 @@
             "--install-completion",
             "bash",
         ],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     new_text = bash_completion_path.read_text()
     bash_completion_path.write_text(text)
     install_source = ".bash_completions/tutorial001.py.sh"
     assert install_source not in text
@@ -86,15 +84,14 @@
             "--install-completion",
             "zsh",
         ],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     new_text = completion_path.read_text()
     completion_path.write_text(text)
     zfunc_fragment = "fpath+=~/.zfunc"
     assert zfunc_fragment in new_text
@@ -122,15 +119,14 @@
             "--install-completion",
             "fish",
         ],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     new_text = completion_path.read_text()
     completion_path.unlink()
     assert "complete --command tutorial001.py" in new_text
     assert "completion installed in" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_completion/test_completion_show.py` & `typer_slim-0.12.dev2/tests/test_completion/test_completion_show.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 def test_completion_show_no_shell():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, "--show-completion"],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     assert "Option '--show-completion' requires an argument" in result.stderr
 
 
 def test_completion_show_bash():
@@ -39,15 +38,14 @@
             "--show-completion",
             "bash",
         ],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     assert (
         "complete -o default -F _tutorial001py_completion tutorial001.py"
         in result.stdout
     )
@@ -64,15 +62,14 @@
             "--show-completion",
             "zsh",
         ],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     assert "compdef _tutorial001py_completion tutorial001.py" in result.stdout
 
 
 def test_completion_source_fish():
@@ -86,15 +83,14 @@
             "--show-completion",
             "fish",
         ],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     assert "complete --command tutorial001.py --no-files" in result.stdout
 
 
 def test_completion_source_powershell():
@@ -108,15 +104,14 @@
             "--show-completion",
             "powershell",
         ],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     assert (
         "Register-ArgumentCompleter -Native -CommandName tutorial001.py -ScriptBlock $scriptblock"
         in result.stdout
     )
@@ -133,15 +128,14 @@
             "--show-completion",
             "pwsh",
         ],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TYPER_COMPLETE_TESTING": "True",
             "_TYPER_COMPLETE_TEST_DISABLE_SHELL_DETECTION": "True",
         },
     )
     assert (
         "Register-ArgumentCompleter -Native -CommandName tutorial001.py -ScriptBlock $scriptblock"
         in result.stdout
     )
```

### Comparing `typer_slim-0.12.dev1/tests/test_exit_errors.py` & `typer_slim-0.12.dev2/tests/test_exit_errors.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_others.py` & `typer_slim-0.12.dev2/tests/test_others.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,14 @@
         [sys.executable, "-m", "coverage", "run", str(file_path)],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_COMPLETION_NO_TYPES.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "completion_no_types.py --name Sebastian --name Ca",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "info name is: completion_no_types.py" in result.stderr
     assert "args is: []" in result.stderr
     assert "incomplete is: Ca" in result.stderr
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
@@ -174,15 +173,14 @@
         [sys.executable, "-m", "coverage", "run", str(file_path)],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_COMPLETION_NO_TYPES_ORDER.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "completion_no_types_order.py --name Sebastian --name Ca",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "info name is: completion_no_types_order.py" in result.stderr
     assert "args is: []" in result.stderr
     assert "incomplete is: Ca" in result.stderr
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_rich_utils.py` & `typer_slim-0.12.dev2/tests/test_rich_utils.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tracebacks.py` & `typer_slim-0.12.dev2/tests/test_tracebacks.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_default/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_default/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_default/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_default/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_default/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_default/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_envvar/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial004_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial005_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial006_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial006_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial007_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_help/test_tutorial008_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_help/test_tutorial008_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_arguments/test_optional/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_arguments/test_optional/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_arguments/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_callback/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_callback/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_callback/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_callback/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_context/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_context/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_context/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_context/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_context/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_context/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_context/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_context/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial004_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial005.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial005_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial006.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial007.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial007_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial007_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_help/test_tutorial008.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_help/test_tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_index/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_index/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_index/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_index/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_index/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_index/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_name/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_name/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_one_or_multiple/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_options/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_options/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_commands/test_options/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_commands/test_options/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_exceptions/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_exceptions/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_exceptions/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_exceptions/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_exceptions/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_exceptions/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_exceptions/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_exceptions/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial005.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_first_steps/test_tutorial006.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_first_steps/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_arguments_with_multiple_values/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_multiple_options/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_multiple_values/test_options_with_multiple_values/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial003.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,11 +41,10 @@
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL003.PY_COMPLETE": "complete_bash",
             "COMP_WORDS": "tutorial003.py --",
             "COMP_CWORD": "1",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "--name" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial004.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 import subprocess
 import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.options.callback import tutorial003_an as mod
+from docs_src.options.callback import tutorial004 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_1():
     result = runner.invoke(app, ["--name", "Camila"])
     assert result.exit_code == 0
-    assert "Validating name" in result.output
+    assert "Validating param: name" in result.output
     assert "Hello Camila" in result.output
 
 
 def test_2():
     result = runner.invoke(app, ["--name", "rick"])
     assert result.exit_code != 0
     assert "Invalid value for '--name': Only Camila is allowed" in result.output
@@ -38,14 +38,13 @@
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL003_AN.PY_COMPLETE": "complete_bash",
-            "COMP_WORDS": "tutorial003_an.py --",
+            "_TUTORIAL004.PY_COMPLETE": "complete_bash",
+            "COMP_WORDS": "tutorial004.py --",
             "COMP_CWORD": "1",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "--name" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial003_an.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import os
 import subprocess
 import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.options.callback import tutorial004 as mod
+from docs_src.options.callback import tutorial003_an as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
 def test_1():
     result = runner.invoke(app, ["--name", "Camila"])
     assert result.exit_code == 0
-    assert "Validating param: name" in result.output
+    assert "Validating name" in result.output
     assert "Hello Camila" in result.output
 
 
 def test_2():
     result = runner.invoke(app, ["--name", "rick"])
     assert result.exit_code != 0
     assert "Invalid value for '--name': Only Camila is allowed" in result.output
@@ -38,14 +38,13 @@
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL004.PY_COMPLETE": "complete_bash",
-            "COMP_WORDS": "tutorial004.py --",
+            "_TUTORIAL003_AN.PY_COMPLETE": "complete_bash",
+            "COMP_WORDS": "tutorial003_an.py --",
             "COMP_CWORD": "1",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "--name" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_callback/test_tutorial004_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_callback/test_tutorial004_an.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,11 +41,10 @@
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL004_AN.PY_COMPLETE": "complete_bash",
             "COMP_WORDS": "tutorial004_an.py --",
             "COMP_CWORD": "1",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "--name" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_help/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_help/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial004_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial005.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_name/test_tutorial005_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_name/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_prompt/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_prompt/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_required/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_required/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_required/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_required/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_version/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_version/test_tutorial003_an.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import subprocess
 import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.options.version import tutorial003 as mod
+from docs_src.options.version import tutorial003_an as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
@@ -43,14 +43,13 @@
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL003.PY_COMPLETE": "complete_bash",
-            "COMP_WORDS": "tutorial003.py --name Rick --v",
+            "_TUTORIAL003_AN.PY_COMPLETE": "complete_bash",
+            "COMP_WORDS": "tutorial003_an.py --name Rick --v",
             "COMP_CWORD": "3",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "--version" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options/test_version/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options/test_version/test_tutorial003.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import subprocess
 import sys
 
 import typer
 from typer.testing import CliRunner
 
-from docs_src.options.version import tutorial003_an as mod
+from docs_src.options.version import tutorial003 as mod
 
 runner = CliRunner()
 
 app = typer.Typer()
 app.command()(mod.main)
 
 
@@ -43,14 +43,13 @@
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL003_AN.PY_COMPLETE": "complete_bash",
-            "COMP_WORDS": "tutorial003_an.py --name Rick --v",
+            "_TUTORIAL003.PY_COMPLETE": "complete_bash",
+            "COMP_WORDS": "tutorial003.py --name Rick --v",
             "COMP_CWORD": "3",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "--version" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial002.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL002.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial002.py --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "Camila" in result.stdout
     assert "Carlos" in result.stdout
     assert "Sebastian" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial002_an.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL002_AN.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial002_an.py --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "Camila" in result.stdout
     assert "Carlos" in result.stdout
     assert "Sebastian" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial003.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,14 @@
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
             "_TUTORIAL003.PY_COMPLETE": "complete_zsh",
             "_TYPER_COMPLETE_ARGS": "tutorial003.py --name Seb",
-            "_TYPER_COMPLETE_TESTING": "True",
         },
     )
     assert "Camila" not in result.stdout
     assert "Carlos" not in result.stdout
     assert "Sebastian" in result.stdout
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import os
 import subprocess
 import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial003_an as mod
+from docs_src.options_autocompletion import tutorial008 as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL003_AN.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial003_an.py --name Seb",
-            "_TYPER_COMPLETE_TESTING": "True",
+            "_TUTORIAL008.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial008.py --name ",
         },
     )
-    assert "Camila" not in result.stdout
-    assert "Carlos" not in result.stdout
-    assert "Sebastian" in result.stdout
+    assert '"Camila":"The reader of books."' in result.stdout
+    assert '"Carlos":"The writer of scripts."' in result.stdout
+    assert '"Sebastian":"The type hints guy."' in result.stdout
+    assert "[]" in result.stderr
 
 
 def test_1():
-    result = runner.invoke(mod.app, ["--name", "Camila"])
+    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
+    assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         capture_output=True,
         encoding="utf-8",
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial008_an.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import os
 import subprocess
 import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial004 as mod
+from docs_src.options_autocompletion import tutorial008_an as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL004.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial004_aux.py --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
+            "_TUTORIAL008_AN.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial008_an.py --name ",
         },
     )
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' in result.stdout
+    assert "[]" in result.stderr
 
 
 def test_1():
-    result = runner.invoke(mod.app, ["--name", "Camila"])
+    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
+    assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         capture_output=True,
         encoding="utf-8",
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial004_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import os
 import subprocess
 import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial004_an as mod
+from docs_src.options_autocompletion import tutorial007 as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL004_AN.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial004_an_aux.py --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
+            "_TUTORIAL007.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial007.py --name Sebastian --name ",
         },
     )
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
-    assert '"Sebastian":"The type hints guy."' in result.stdout
+    assert '"Sebastian":"The type hints guy."' not in result.stdout
 
 
 def test_1():
-    result = runner.invoke(mod.app, ["--name", "Camila"])
+    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
+    assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         capture_output=True,
         encoding="utf-8",
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial007.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial009_an.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
 import subprocess
 import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial007 as mod
+from docs_src.options_autocompletion import tutorial009_an as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL007.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial007.py --name Sebastian --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
+            "_TUTORIAL009_AN.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial009_an.py --name Sebastian --name ",
         },
     )
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' not in result.stdout
+    assert "[]" in result.stderr
 
 
 def test_1():
     result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
     assert "Hello Sebastian" in result.output
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial007_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 import os
 import subprocess
 import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial007_an as mod
+from docs_src.options_autocompletion import tutorial009 as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL007_AN.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial007_an.py --name Sebastian --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
+            "_TUTORIAL009.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial009.py --name Sebastian --name ",
         },
     )
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' not in result.stdout
+    assert "[]" in result.stderr
 
 
 def test_1():
     result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
     assert "Hello Sebastian" in result.output
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial008.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial004.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import os
 import subprocess
 import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial008 as mod
+from docs_src.options_autocompletion import tutorial004 as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL008.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial008.py --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
+            "_TUTORIAL004.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial004_aux.py --name ",
         },
     )
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' in result.stdout
-    assert "[]" in result.stderr
 
 
 def test_1():
-    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
+    result = runner.invoke(mod.app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
-    assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         capture_output=True,
         encoding="utf-8",
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial008_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial004_an.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import os
 import subprocess
 import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial008_an as mod
+from docs_src.options_autocompletion import tutorial004_an as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL008_AN.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial008_an.py --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
+            "_TUTORIAL004_AN.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial004_an_aux.py --name ",
         },
     )
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' in result.stdout
-    assert "[]" in result.stderr
 
 
 def test_1():
-    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
+    result = runner.invoke(mod.app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
-    assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         capture_output=True,
         encoding="utf-8",
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial009.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial007_an.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 import os
 import subprocess
 import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial009 as mod
+from docs_src.options_autocompletion import tutorial007_an as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL009.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial009.py --name Sebastian --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
+            "_TUTORIAL007_AN.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial007_an.py --name Sebastian --name ",
         },
     )
     assert '"Camila":"The reader of books."' in result.stdout
     assert '"Carlos":"The writer of scripts."' in result.stdout
     assert '"Sebastian":"The type hints guy."' not in result.stdout
-    assert "[]" in result.stderr
 
 
 def test_1():
     result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
     assert "Hello Sebastian" in result.output
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_options_autocompletion/test_tutorial009_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_options_autocompletion/test_tutorial003_an.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 import os
 import subprocess
 import sys
 
 from typer.testing import CliRunner
 
-from docs_src.options_autocompletion import tutorial009_an as mod
+from docs_src.options_autocompletion import tutorial003_an as mod
 
 runner = CliRunner()
 
 
 def test_completion():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, " "],
         capture_output=True,
         encoding="utf-8",
         env={
             **os.environ,
-            "_TUTORIAL009_AN.PY_COMPLETE": "complete_zsh",
-            "_TYPER_COMPLETE_ARGS": "tutorial009_an.py --name Sebastian --name ",
-            "_TYPER_COMPLETE_TESTING": "True",
+            "_TUTORIAL003_AN.PY_COMPLETE": "complete_zsh",
+            "_TYPER_COMPLETE_ARGS": "tutorial003_an.py --name Seb",
         },
     )
-    assert '"Camila":"The reader of books."' in result.stdout
-    assert '"Carlos":"The writer of scripts."' in result.stdout
-    assert '"Sebastian":"The type hints guy."' not in result.stdout
-    assert "[]" in result.stderr
+    assert "Camila" not in result.stdout
+    assert "Carlos" not in result.stdout
+    assert "Sebastian" in result.stdout
 
 
 def test_1():
-    result = runner.invoke(mod.app, ["--name", "Camila", "--name", "Sebastian"])
+    result = runner.invoke(mod.app, ["--name", "Camila"])
     assert result.exit_code == 0
     assert "Hello Camila" in result.output
-    assert "Hello Sebastian" in result.output
 
 
 def test_script():
     result = subprocess.run(
         [sys.executable, "-m", "coverage", "run", mod.__file__, "--help"],
         capture_output=True,
         encoding="utf-8",
```

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_bool/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_custom_types/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_datetime/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_enum/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial004_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_file/test_tutorial005_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_index/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_number/test_tutorial003_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_path/test_tutorial001_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002_an.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_path/test_tutorial002_an.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_parameter_types/test_uuid/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_prompt/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_prompt/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_prompt/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_prompt/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_prompt/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_prompt/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_callback_override/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial005.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial006.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial007.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_name_help/test_tutorial008.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_subcommands/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_subcommands/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_terminating/test_tutorial001.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_terminating/test_tutorial001.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_terminating/test_tutorial002.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_terminating/test_tutorial002.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_terminating/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_terminating/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_using_click/test_tutorial003.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_using_click/test_tutorial003.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_tutorial/test_using_click/test_tutorial004.py` & `typer_slim-0.12.dev2/tests/test_tutorial/test_using_click/test_tutorial004.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/tests/test_type_conversion.py` & `typer_slim-0.12.dev2/tests/test_type_conversion.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/__init__.py` & `typer_slim-0.12.dev2/typer/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Typer, build great CLIs. Easy to code. Based on Python type hints."""
 
-__version__ = "0.12.dev1"
+__version__ = "0.12.dev2"
 
 from shutil import get_terminal_size as get_terminal_size
 
 from click.exceptions import Abort as Abort
 from click.exceptions import BadParameter as BadParameter
 from click.exceptions import Exit as Exit
 from click.termui import clear as clear
```

### Comparing `typer_slim-0.12.dev1/typer/_completion_classes.py` & `typer_slim-0.12.dev2/typer/_completion_classes.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/_completion_shared.py` & `typer_slim-0.12.dev2/typer/_completion_shared.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/_typing.py` & `typer_slim-0.12.dev2/typer/_typing.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/cli.py` & `typer_slim-0.12.dev2/typer/cli.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/completion.py` & `typer_slim-0.12.dev2/typer/completion.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/core.py` & `typer_slim-0.12.dev2/typer/core.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/main.py` & `typer_slim-0.12.dev2/typer/main.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/models.py` & `typer_slim-0.12.dev2/typer/models.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/params.py` & `typer_slim-0.12.dev2/typer/params.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/rich_utils.py` & `typer_slim-0.12.dev2/typer/rich_utils.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/testing.py` & `typer_slim-0.12.dev2/typer/testing.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/typer/utils.py` & `typer_slim-0.12.dev2/typer/utils.py`

 * *Files identical despite different names*

### Comparing `typer_slim-0.12.dev1/PKG-INFO` & `typer_slim-0.12.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typer-slim
-Version: 0.12.dev1
+Version: 0.12.dev2
 Summary: Typer, build great CLIs. Easy to code. Based on Python type hints.
 Home-page: https://github.com/tiangolo/typer
 Author-Email: Sebastián Ramírez <tiangolo@gmail.com>
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: typer-slim Version: 0.12.dev1 Summary: Typer, build
+Metadata-Version: 2.1 Name: typer-slim Version: 0.12.dev2 Summary: Typer, build
 great CLIs. Easy to code. Based on Python type hints. Home-page: https://
 github.com/tiangolo/typer Author-Email: SebastiÃ¡n RamÃ­rez
 gmail.com> Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Topic :: Software Development
```

