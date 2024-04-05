# Comparing `tmp/pyformlang-1.0.8.tar.gz` & `tmp/pyformlang-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyformlang-1.0.8.tar", last modified: Mon Mar 18 13:11:07 2024, max compression
+gzip compressed data, was "pyformlang-1.0.9.tar", last modified: Mon Mar 18 18:10:26 2024, max compression
```

## Comparing `pyformlang-1.0.8.tar` & `pyformlang-1.0.9.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.925637 pyformlang-1.0.8/
--rw-rw-r--   0 julien    (1000) julien    (1000)     1070 2022-06-03 08:50:00.000000 pyformlang-1.0.8/LICENSE
--rw-rw-r--   0 julien    (1000) julien    (1000)     2294 2024-03-18 13:11:07.925637 pyformlang-1.0.8/PKG-INFO
--rw-rw-r--   0 julien    (1000) julien    (1000)     1872 2022-06-03 14:50:28.000000 pyformlang-1.0.8/README.md
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.909636 pyformlang-1.0.8/pyformlang/
--rw-rw-r--   0 julien    (1000) julien    (1000)      814 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/__init__.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.909636 pyformlang-1.0.8/pyformlang/cfg/
--rw-rw-r--   0 julien    (1000) julien    (1000)      728 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/cfg/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    40695 2023-04-18 16:51:27.000000 pyformlang-1.0.8/pyformlang/cfg/cfg.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      608 2022-06-03 11:48:11.000000 pyformlang-1.0.8/pyformlang/cfg/cfg_object.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4501 2022-06-03 11:47:34.000000 pyformlang-1.0.8/pyformlang/cfg/cyk_table.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      281 2022-06-03 09:42:15.000000 pyformlang-1.0.8/pyformlang/cfg/epsilon.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     9297 2022-06-03 12:58:26.000000 pyformlang-1.0.8/pyformlang/cfg/llone_parser.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     3397 2023-04-18 19:05:13.000000 pyformlang-1.0.8/pyformlang/cfg/parse_tree.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1439 2022-06-03 11:47:26.000000 pyformlang-1.0.8/pyformlang/cfg/pda_object_creator.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1828 2023-04-18 17:27:00.000000 pyformlang-1.0.8/pyformlang/cfg/production.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4340 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/cfg/recursive_decent_parser.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      601 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/cfg/set_queue.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      718 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/cfg/terminal.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.913637 pyformlang-1.0.8/pyformlang/cfg/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/cfg/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    35520 2023-04-18 13:51:56.000000 pyformlang-1.0.8/pyformlang/cfg/tests/test_cfg.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    12656 2022-06-03 12:46:13.000000 pyformlang-1.0.8/pyformlang/cfg/tests/test_llone_parser.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1267 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/cfg/tests/test_production.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2579 2023-04-18 15:32:45.000000 pyformlang-1.0.8/pyformlang/cfg/tests/test_recursive_decent_parser.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      957 2023-04-18 15:33:47.000000 pyformlang-1.0.8/pyformlang/cfg/tests/test_terminal.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      804 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/cfg/tests/test_variable.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      394 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/cfg/utils.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1468 2022-06-03 11:47:38.000000 pyformlang-1.0.8/pyformlang/cfg/utils_cfg.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1062 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/cfg/variable.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.913637 pyformlang-1.0.8/pyformlang/fcfg/
--rw-rw-r--   0 julien    (1000) julien    (1000)      747 2023-04-18 19:10:47.000000 pyformlang-1.0.8/pyformlang/fcfg/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     9525 2023-04-18 19:06:00.000000 pyformlang-1.0.8/pyformlang/fcfg/fcfg.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1818 2023-04-18 17:28:34.000000 pyformlang-1.0.8/pyformlang/fcfg/feature_production.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    12463 2023-04-18 18:41:19.000000 pyformlang-1.0.8/pyformlang/fcfg/feature_structure.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2093 2023-04-18 18:55:29.000000 pyformlang-1.0.8/pyformlang/fcfg/state.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.913637 pyformlang-1.0.8/pyformlang/fcfg/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2023-04-17 10:32:24.000000 pyformlang-1.0.8/pyformlang/fcfg/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     9731 2023-04-18 19:07:03.000000 pyformlang-1.0.8/pyformlang/fcfg/tests/test_fcfg.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     8739 2023-04-18 18:40:38.000000 pyformlang-1.0.8/pyformlang/fcfg/tests/test_feature_structure.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.917636 pyformlang-1.0.8/pyformlang/finite_automaton/
--rw-rw-r--   0 julien    (1000) julien    (1000)     2388 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    16748 2022-06-03 11:33:21.000000 pyformlang-1.0.8/pyformlang/finite_automaton/deterministic_finite_automaton.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1320 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/doubly_linked_list.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1046 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/doubly_linked_node.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      473 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/epsilon.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    32753 2022-06-03 11:39:19.000000 pyformlang-1.0.8/pyformlang/finite_automaton/epsilon_nfa.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    18726 2022-06-07 15:07:04.000000 pyformlang-1.0.8/pyformlang/finite_automaton/finite_automaton.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      666 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/finite_automaton_object.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1206 2022-06-03 11:24:50.000000 pyformlang-1.0.8/pyformlang/finite_automaton/hopcroft_processing_list.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4238 2022-06-03 11:10:39.000000 pyformlang-1.0.8/pyformlang/finite_automaton/nondeterministic_finite_automaton.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     6084 2022-06-03 11:37:38.000000 pyformlang-1.0.8/pyformlang/finite_automaton/nondeterministic_transition_function.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1897 2022-06-03 11:10:33.000000 pyformlang-1.0.8/pyformlang/finite_automaton/partition.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2029 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/regexable.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      883 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/state.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      756 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/symbol.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.921637 pyformlang-1.0.8/pyformlang/finite_automaton/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    12636 2022-06-03 11:34:31.000000 pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_deterministic_finite_automaton.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      456 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_epsilon.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    28438 2022-06-03 11:34:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_epsilon_nfa.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4647 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_nondeterministic_finite_automaton.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4269 2022-06-03 12:48:58.000000 pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_nondeterministic_transition_function.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1272 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_state.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1282 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_symbol.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     3817 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_transition_function.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     7065 2022-06-03 11:09:17.000000 pyformlang-1.0.8/pyformlang/finite_automaton/transition_function.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.921637 pyformlang-1.0.8/pyformlang/fst/
--rw-rw-r--   0 julien    (1000) julien    (1000)      216 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/fst/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    21016 2022-06-07 15:07:10.000000 pyformlang-1.0.8/pyformlang/fst/fst.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.921637 pyformlang-1.0.8/pyformlang/fst/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/fst/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     8317 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/fst/tests/test_fst.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.921637 pyformlang-1.0.8/pyformlang/indexed_grammar/
--rw-rw-r--   0 julien    (1000) julien    (1000)      920 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2580 2022-06-03 11:46:36.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/consumption_rule.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2723 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/duplication_rule.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2303 2022-06-03 11:47:16.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/end_rule.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    18369 2022-06-03 14:06:05.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/indexed_grammar.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2803 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/production_rule.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2422 2022-06-03 11:45:37.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/reduced_rule.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     5610 2022-06-03 11:46:58.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/rule_ordering.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     5889 2023-04-18 17:39:15.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/rules.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.921637 pyformlang-1.0.8/pyformlang/indexed_grammar/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    14169 2022-06-03 12:32:54.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/tests/test_indexed_grammar.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2026 2022-06-03 12:47:16.000000 pyformlang-1.0.8/pyformlang/indexed_grammar/tests/test_rules.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.925637 pyformlang-1.0.8/pyformlang/pda/
--rw-rw-r--   0 julien    (1000) julien    (1000)      605 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/pda/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     4245 2022-06-03 12:18:27.000000 pyformlang-1.0.8/pyformlang/pda/cfg_variable_converter.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      215 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/pda/epsilon.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    27276 2022-06-07 15:07:16.000000 pyformlang-1.0.8/pyformlang/pda/pda.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      805 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/pda/stack_symbol.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      836 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/pda/state.py
--rw-rw-r--   0 julien    (1000) julien    (1000)      714 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/pda/symbol.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.925637 pyformlang-1.0.8/pyformlang/pda/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/pda/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    15278 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/pda/tests/test_pda.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     3359 2022-06-03 12:04:14.000000 pyformlang-1.0.8/pyformlang/pda/transition_function.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     1757 2022-06-03 12:18:35.000000 pyformlang-1.0.8/pyformlang/pda/utils.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.925637 pyformlang-1.0.8/pyformlang/regular_expression/
--rw-rw-r--   0 julien    (1000) julien    (1000)      771 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/regular_expression/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    14560 2024-03-18 13:04:48.000000 pyformlang-1.0.8/pyformlang/regular_expression/python_regex.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    16628 2022-06-03 11:57:40.000000 pyformlang-1.0.8/pyformlang/regular_expression/regex.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     5835 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/regular_expression/regex_objects.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     8908 2024-01-25 12:23:56.000000 pyformlang-1.0.8/pyformlang/regular_expression/regex_reader.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.925637 pyformlang-1.0.8/pyformlang/regular_expression/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/regular_expression/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    11700 2024-03-18 13:08:40.000000 pyformlang-1.0.8/pyformlang/regular_expression/tests/test_python_regex.py
--rw-rw-r--   0 julien    (1000) julien    (1000)    11742 2024-01-25 14:23:18.000000 pyformlang-1.0.8/pyformlang/regular_expression/tests/test_regex.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.925637 pyformlang-1.0.8/pyformlang/rsa/
--rw-rw-r--   0 julien    (1000) julien    (1000)      719 2022-06-03 09:44:06.000000 pyformlang-1.0.8/pyformlang/rsa/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     2529 2022-06-03 09:44:14.000000 pyformlang-1.0.8/pyformlang/rsa/box.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     6024 2022-06-03 11:58:43.000000 pyformlang-1.0.8/pyformlang/rsa/recursive_automaton.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.925637 pyformlang-1.0.8/pyformlang/rsa/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/rsa/tests/__init__.py
--rw-rw-r--   0 julien    (1000) julien    (1000)     3265 2022-06-03 12:01:10.000000 pyformlang-1.0.8/pyformlang/rsa/tests/test_rsa.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.925637 pyformlang-1.0.8/pyformlang/tests/
--rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.8/pyformlang/tests/__init__.py
-drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 13:11:07.909636 pyformlang-1.0.8/pyformlang.egg-info/
--rw-rw-r--   0 julien    (1000) julien    (1000)     2294 2024-03-18 13:11:07.000000 pyformlang-1.0.8/pyformlang.egg-info/PKG-INFO
--rw-rw-r--   0 julien    (1000) julien    (1000)     4051 2024-03-18 13:11:07.000000 pyformlang-1.0.8/pyformlang.egg-info/SOURCES.txt
--rw-rw-r--   0 julien    (1000) julien    (1000)        1 2024-03-18 13:11:07.000000 pyformlang-1.0.8/pyformlang.egg-info/dependency_links.txt
--rw-rw-r--   0 julien    (1000) julien    (1000)       21 2024-03-18 13:11:07.000000 pyformlang-1.0.8/pyformlang.egg-info/requires.txt
--rw-rw-r--   0 julien    (1000) julien    (1000)       11 2024-03-18 13:11:07.000000 pyformlang-1.0.8/pyformlang.egg-info/top_level.txt
--rw-rw-r--   0 julien    (1000) julien    (1000)       38 2024-03-18 13:11:07.925637 pyformlang-1.0.8/setup.cfg
--rw-rw-r--   0 julien    (1000) julien    (1000)      758 2024-03-18 13:11:05.000000 pyformlang-1.0.8/setup.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.249483 pyformlang-1.0.9/
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1070 2022-06-03 08:50:00.000000 pyformlang-1.0.9/LICENSE
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2294 2024-03-18 18:10:26.245483 pyformlang-1.0.9/PKG-INFO
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1872 2022-06-03 14:50:28.000000 pyformlang-1.0.9/README.md
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.237483 pyformlang-1.0.9/pyformlang/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      814 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/__init__.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.241483 pyformlang-1.0.9/pyformlang/cfg/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      728 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/cfg/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    40695 2023-04-18 16:51:27.000000 pyformlang-1.0.9/pyformlang/cfg/cfg.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      608 2022-06-03 11:48:11.000000 pyformlang-1.0.9/pyformlang/cfg/cfg_object.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4501 2022-06-03 11:47:34.000000 pyformlang-1.0.9/pyformlang/cfg/cyk_table.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      281 2022-06-03 09:42:15.000000 pyformlang-1.0.9/pyformlang/cfg/epsilon.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     9297 2022-06-03 12:58:26.000000 pyformlang-1.0.9/pyformlang/cfg/llone_parser.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     3397 2023-04-18 19:05:13.000000 pyformlang-1.0.9/pyformlang/cfg/parse_tree.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1439 2022-06-03 11:47:26.000000 pyformlang-1.0.9/pyformlang/cfg/pda_object_creator.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1828 2023-04-18 17:27:00.000000 pyformlang-1.0.9/pyformlang/cfg/production.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4340 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/cfg/recursive_decent_parser.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      601 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/cfg/set_queue.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      718 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/cfg/terminal.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.241483 pyformlang-1.0.9/pyformlang/cfg/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/cfg/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    35520 2023-04-18 13:51:56.000000 pyformlang-1.0.9/pyformlang/cfg/tests/test_cfg.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    12656 2022-06-03 12:46:13.000000 pyformlang-1.0.9/pyformlang/cfg/tests/test_llone_parser.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1267 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/cfg/tests/test_production.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2579 2023-04-18 15:32:45.000000 pyformlang-1.0.9/pyformlang/cfg/tests/test_recursive_decent_parser.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      957 2023-04-18 15:33:47.000000 pyformlang-1.0.9/pyformlang/cfg/tests/test_terminal.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      804 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/cfg/tests/test_variable.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      394 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/cfg/utils.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1468 2022-06-03 11:47:38.000000 pyformlang-1.0.9/pyformlang/cfg/utils_cfg.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1062 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/cfg/variable.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.241483 pyformlang-1.0.9/pyformlang/fcfg/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      747 2023-04-18 19:10:47.000000 pyformlang-1.0.9/pyformlang/fcfg/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     9525 2023-04-18 19:06:00.000000 pyformlang-1.0.9/pyformlang/fcfg/fcfg.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1818 2023-04-18 17:28:34.000000 pyformlang-1.0.9/pyformlang/fcfg/feature_production.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    12463 2023-04-18 18:41:19.000000 pyformlang-1.0.9/pyformlang/fcfg/feature_structure.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2093 2023-04-18 18:55:29.000000 pyformlang-1.0.9/pyformlang/fcfg/state.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.241483 pyformlang-1.0.9/pyformlang/fcfg/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2023-04-17 10:32:24.000000 pyformlang-1.0.9/pyformlang/fcfg/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     9731 2023-04-18 19:07:03.000000 pyformlang-1.0.9/pyformlang/fcfg/tests/test_fcfg.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     8739 2023-04-18 18:40:38.000000 pyformlang-1.0.9/pyformlang/fcfg/tests/test_feature_structure.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.241483 pyformlang-1.0.9/pyformlang/finite_automaton/
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2388 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    16748 2022-06-03 11:33:21.000000 pyformlang-1.0.9/pyformlang/finite_automaton/deterministic_finite_automaton.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1320 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/doubly_linked_list.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1046 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/doubly_linked_node.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      473 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/epsilon.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    32753 2022-06-03 11:39:19.000000 pyformlang-1.0.9/pyformlang/finite_automaton/epsilon_nfa.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    18726 2022-06-07 15:07:04.000000 pyformlang-1.0.9/pyformlang/finite_automaton/finite_automaton.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      666 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/finite_automaton_object.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1206 2022-06-03 11:24:50.000000 pyformlang-1.0.9/pyformlang/finite_automaton/hopcroft_processing_list.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4238 2022-06-03 11:10:39.000000 pyformlang-1.0.9/pyformlang/finite_automaton/nondeterministic_finite_automaton.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     6084 2022-06-03 11:37:38.000000 pyformlang-1.0.9/pyformlang/finite_automaton/nondeterministic_transition_function.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1897 2022-06-03 11:10:33.000000 pyformlang-1.0.9/pyformlang/finite_automaton/partition.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2029 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/regexable.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      883 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/state.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      756 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/symbol.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.241483 pyformlang-1.0.9/pyformlang/finite_automaton/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    12636 2022-06-03 11:34:31.000000 pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_deterministic_finite_automaton.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      456 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_epsilon.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    28438 2022-06-03 11:34:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_epsilon_nfa.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4647 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_nondeterministic_finite_automaton.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4269 2022-06-03 12:48:58.000000 pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_nondeterministic_transition_function.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1272 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_state.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1282 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_symbol.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     3817 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_transition_function.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     7065 2022-06-03 11:09:17.000000 pyformlang-1.0.9/pyformlang/finite_automaton/transition_function.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.241483 pyformlang-1.0.9/pyformlang/fst/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      216 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/fst/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    21016 2022-06-07 15:07:10.000000 pyformlang-1.0.9/pyformlang/fst/fst.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.245483 pyformlang-1.0.9/pyformlang/fst/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/fst/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     8317 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/fst/tests/test_fst.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.245483 pyformlang-1.0.9/pyformlang/indexed_grammar/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      920 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2580 2022-06-03 11:46:36.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/consumption_rule.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2723 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/duplication_rule.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2303 2022-06-03 11:47:16.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/end_rule.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    18369 2022-06-03 14:06:05.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/indexed_grammar.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2803 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/production_rule.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2422 2022-06-03 11:45:37.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/reduced_rule.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     5610 2022-06-03 11:46:58.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/rule_ordering.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     5889 2023-04-18 17:39:15.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/rules.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.245483 pyformlang-1.0.9/pyformlang/indexed_grammar/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    14169 2022-06-03 12:32:54.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/tests/test_indexed_grammar.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2026 2022-06-03 12:47:16.000000 pyformlang-1.0.9/pyformlang/indexed_grammar/tests/test_rules.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.245483 pyformlang-1.0.9/pyformlang/pda/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      605 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/pda/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4245 2022-06-03 12:18:27.000000 pyformlang-1.0.9/pyformlang/pda/cfg_variable_converter.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      215 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/pda/epsilon.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    27276 2022-06-07 15:07:16.000000 pyformlang-1.0.9/pyformlang/pda/pda.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      805 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/pda/stack_symbol.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      836 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/pda/state.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)      714 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/pda/symbol.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.245483 pyformlang-1.0.9/pyformlang/pda/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/pda/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    15278 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/pda/tests/test_pda.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     3359 2022-06-03 12:04:14.000000 pyformlang-1.0.9/pyformlang/pda/transition_function.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     1757 2022-06-03 12:18:35.000000 pyformlang-1.0.9/pyformlang/pda/utils.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.245483 pyformlang-1.0.9/pyformlang/regular_expression/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      771 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/regular_expression/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    14928 2024-03-18 15:58:12.000000 pyformlang-1.0.9/pyformlang/regular_expression/python_regex.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    16628 2022-06-03 11:57:40.000000 pyformlang-1.0.9/pyformlang/regular_expression/regex.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     5835 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/regular_expression/regex_objects.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     8908 2024-01-25 12:23:56.000000 pyformlang-1.0.9/pyformlang/regular_expression/regex_reader.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.245483 pyformlang-1.0.9/pyformlang/regular_expression/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/regular_expression/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    12451 2024-03-18 16:00:26.000000 pyformlang-1.0.9/pyformlang/regular_expression/tests/test_python_regex.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)    11742 2024-01-25 14:23:18.000000 pyformlang-1.0.9/pyformlang/regular_expression/tests/test_regex.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.245483 pyformlang-1.0.9/pyformlang/rsa/
+-rw-rw-r--   0 julien    (1000) julien    (1000)      719 2022-06-03 09:44:06.000000 pyformlang-1.0.9/pyformlang/rsa/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2529 2022-06-03 09:44:14.000000 pyformlang-1.0.9/pyformlang/rsa/box.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     6024 2022-06-03 11:58:43.000000 pyformlang-1.0.9/pyformlang/rsa/recursive_automaton.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.245483 pyformlang-1.0.9/pyformlang/rsa/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/rsa/tests/__init__.py
+-rw-rw-r--   0 julien    (1000) julien    (1000)     3265 2022-06-03 12:01:10.000000 pyformlang-1.0.9/pyformlang/rsa/tests/test_rsa.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.245483 pyformlang-1.0.9/pyformlang/tests/
+-rw-rw-r--   0 julien    (1000) julien    (1000)        0 2022-06-03 08:50:00.000000 pyformlang-1.0.9/pyformlang/tests/__init__.py
+drwxrwxr-x   0 julien    (1000) julien    (1000)        0 2024-03-18 18:10:26.237483 pyformlang-1.0.9/pyformlang.egg-info/
+-rw-rw-r--   0 julien    (1000) julien    (1000)     2294 2024-03-18 18:10:26.000000 pyformlang-1.0.9/pyformlang.egg-info/PKG-INFO
+-rw-rw-r--   0 julien    (1000) julien    (1000)     4051 2024-03-18 18:10:26.000000 pyformlang-1.0.9/pyformlang.egg-info/SOURCES.txt
+-rw-rw-r--   0 julien    (1000) julien    (1000)        1 2024-03-18 18:10:26.000000 pyformlang-1.0.9/pyformlang.egg-info/dependency_links.txt
+-rw-rw-r--   0 julien    (1000) julien    (1000)       21 2024-03-18 18:10:26.000000 pyformlang-1.0.9/pyformlang.egg-info/requires.txt
+-rw-rw-r--   0 julien    (1000) julien    (1000)       11 2024-03-18 18:10:26.000000 pyformlang-1.0.9/pyformlang.egg-info/top_level.txt
+-rw-rw-r--   0 julien    (1000) julien    (1000)       38 2024-03-18 18:10:26.249483 pyformlang-1.0.9/setup.cfg
+-rw-rw-r--   0 julien    (1000) julien    (1000)      758 2024-03-18 18:10:10.000000 pyformlang-1.0.9/setup.py
```

### Comparing `pyformlang-1.0.8/LICENSE` & `pyformlang-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/PKG-INFO` & `pyformlang-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyformlang
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python framework for formal grammars
 Home-page: https://github.com/Aunsiels/pyformlang
 Author: Julien Romero
 Author-email: romerojulien34@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyformlang-1.0.8/README.md` & `pyformlang-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/__init__.py` & `pyformlang-1.0.9/pyformlang/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/__init__.py` & `pyformlang-1.0.9/pyformlang/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/cfg.py` & `pyformlang-1.0.9/pyformlang/cfg/cfg.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/cfg_object.py` & `pyformlang-1.0.9/pyformlang/cfg/cfg_object.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/cyk_table.py` & `pyformlang-1.0.9/pyformlang/cfg/cyk_table.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/llone_parser.py` & `pyformlang-1.0.9/pyformlang/cfg/llone_parser.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/parse_tree.py` & `pyformlang-1.0.9/pyformlang/cfg/parse_tree.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/pda_object_creator.py` & `pyformlang-1.0.9/pyformlang/cfg/pda_object_creator.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/production.py` & `pyformlang-1.0.9/pyformlang/cfg/production.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/recursive_decent_parser.py` & `pyformlang-1.0.9/pyformlang/cfg/recursive_decent_parser.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/set_queue.py` & `pyformlang-1.0.9/pyformlang/cfg/set_queue.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/terminal.py` & `pyformlang-1.0.9/pyformlang/cfg/terminal.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/tests/test_cfg.py` & `pyformlang-1.0.9/pyformlang/cfg/tests/test_cfg.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/tests/test_llone_parser.py` & `pyformlang-1.0.9/pyformlang/cfg/tests/test_llone_parser.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/tests/test_production.py` & `pyformlang-1.0.9/pyformlang/cfg/tests/test_production.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/tests/test_recursive_decent_parser.py` & `pyformlang-1.0.9/pyformlang/cfg/tests/test_recursive_decent_parser.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/tests/test_terminal.py` & `pyformlang-1.0.9/pyformlang/cfg/tests/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/tests/test_variable.py` & `pyformlang-1.0.9/pyformlang/cfg/tests/test_variable.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/utils_cfg.py` & `pyformlang-1.0.9/pyformlang/cfg/utils_cfg.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/cfg/variable.py` & `pyformlang-1.0.9/pyformlang/cfg/variable.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/fcfg/__init__.py` & `pyformlang-1.0.9/pyformlang/fcfg/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/fcfg/fcfg.py` & `pyformlang-1.0.9/pyformlang/fcfg/fcfg.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/fcfg/feature_production.py` & `pyformlang-1.0.9/pyformlang/fcfg/feature_production.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/fcfg/feature_structure.py` & `pyformlang-1.0.9/pyformlang/fcfg/feature_structure.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/fcfg/state.py` & `pyformlang-1.0.9/pyformlang/fcfg/state.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/fcfg/tests/test_fcfg.py` & `pyformlang-1.0.9/pyformlang/fcfg/tests/test_fcfg.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/fcfg/tests/test_feature_structure.py` & `pyformlang-1.0.9/pyformlang/fcfg/tests/test_feature_structure.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/__init__.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/deterministic_finite_automaton.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/deterministic_finite_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/doubly_linked_list.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/doubly_linked_list.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/doubly_linked_node.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/doubly_linked_node.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/epsilon_nfa.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/epsilon_nfa.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/finite_automaton.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/finite_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/finite_automaton_object.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/finite_automaton_object.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/hopcroft_processing_list.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/hopcroft_processing_list.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/nondeterministic_finite_automaton.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/nondeterministic_finite_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/nondeterministic_transition_function.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/nondeterministic_transition_function.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/partition.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/partition.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/regexable.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/regexable.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/state.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/state.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/symbol.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/symbol.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_deterministic_finite_automaton.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_deterministic_finite_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_epsilon_nfa.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_epsilon_nfa.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_nondeterministic_finite_automaton.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_nondeterministic_finite_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_nondeterministic_transition_function.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_nondeterministic_transition_function.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_state.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_symbol.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_symbol.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/tests/test_transition_function.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/tests/test_transition_function.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/finite_automaton/transition_function.py` & `pyformlang-1.0.9/pyformlang/finite_automaton/transition_function.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/fst/fst.py` & `pyformlang-1.0.9/pyformlang/fst/fst.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/fst/tests/test_fst.py` & `pyformlang-1.0.9/pyformlang/fst/tests/test_fst.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/__init__.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/consumption_rule.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/consumption_rule.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/duplication_rule.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/duplication_rule.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/end_rule.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/end_rule.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/indexed_grammar.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/indexed_grammar.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/production_rule.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/production_rule.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/reduced_rule.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/reduced_rule.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/rule_ordering.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/rule_ordering.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/rules.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/rules.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/tests/test_indexed_grammar.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/tests/test_indexed_grammar.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/indexed_grammar/tests/test_rules.py` & `pyformlang-1.0.9/pyformlang/indexed_grammar/tests/test_rules.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/pda/__init__.py` & `pyformlang-1.0.9/pyformlang/pda/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/pda/cfg_variable_converter.py` & `pyformlang-1.0.9/pyformlang/pda/cfg_variable_converter.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/pda/pda.py` & `pyformlang-1.0.9/pyformlang/pda/pda.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/pda/stack_symbol.py` & `pyformlang-1.0.9/pyformlang/pda/stack_symbol.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/pda/state.py` & `pyformlang-1.0.9/pyformlang/pda/state.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/pda/symbol.py` & `pyformlang-1.0.9/pyformlang/pda/symbol.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/pda/tests/test_pda.py` & `pyformlang-1.0.9/pyformlang/pda/tests/test_pda.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/pda/transition_function.py` & `pyformlang-1.0.9/pyformlang/pda/transition_function.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/pda/utils.py` & `pyformlang-1.0.9/pyformlang/pda/utils.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/regular_expression/__init__.py` & `pyformlang-1.0.9/pyformlang/regular_expression/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/regular_expression/python_regex.py` & `pyformlang-1.0.9/pyformlang/regular_expression/python_regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     ")": "\\)",
     "*": "\\*",
     "+": "\\+",
     ".": "\\.",
     "$": "\\$",
     "\n": "",
     " ": "\\ ",
-    '\\': '\\\\'
+    '\\': '\\\\',
+    "?": "\\?"
 }
 
 RECOMBINE = {
     "\\b": "\b",
     "\\n": "\n",
     "\\r": "\r",
     "\\t": "\t",
@@ -128,22 +129,19 @@
         self._python_regex = " ".join(regex_temp_dot)
 
     def _preprocess_brackets(self):
         regex_temp = []
         in_brackets = 0
         in_brackets_temp = []
         for symbol in self._python_regex:
-            if symbol == "[" and (not regex_temp or regex_temp[-1] != "\\") and \
-                    (in_brackets == 0 or not in_brackets_temp[-1] or in_brackets_temp[-1][-1] != "\\"):
+            if symbol == "[" and not self._should_escape_next_symbol(regex_temp) and \
+                    (in_brackets == 0 or not self._should_escape_next_symbol(in_brackets_temp[-1])):
                 in_brackets += 1
                 in_brackets_temp.append([])
-            elif symbol == "]" and (not regex_temp or regex_temp[-1] != "\\") and \
-                    (in_brackets == 0 or not in_brackets_temp[-1] or
-                     (in_brackets_temp[-1][-1] != "\\" or
-                      (len(in_brackets_temp[-1]) > 1 and in_brackets_temp[-1][-2] == "\\"))):
+            elif symbol == "]" and in_brackets >= 1 and not self._should_escape_next_symbol(in_brackets_temp[-1]):
                 if len(in_brackets_temp) == 1:
                     regex_temp.append("(")
                     regex_temp += self._preprocess_brackets_content(
                         in_brackets_temp[-1])
                     regex_temp.append(")")
                 else:
                     in_brackets_temp[-2].append(
@@ -217,21 +215,22 @@
                 res.append(x)
         return res
 
     def _preprocess_brackets_content(self, bracket_content):
         bracket_content_temp = []
         previous_is_valid_for_range = False
         for i, symbol in enumerate(bracket_content):
-            if (symbol == "-" and not self._should_escape_next_symbol(
-                    bracket_content_temp)):
-                if (not previous_is_valid_for_range
-                        or i == len(bracket_content) - 1):
+            # We have a range
+            if symbol == "-" and not self._should_escape_next_symbol(bracket_content_temp):
+                if not previous_is_valid_for_range or i == len(bracket_content) - 1:
+                    # False alarm, no range
                     bracket_content_temp.append("-")
                     previous_is_valid_for_range = True
                 else:
+                    # We insert all the characters in the range
                     bracket_content[i - 1] = self._recombine(bracket_content[i - 1])
                     for j in range(ord(bracket_content[i - 1][-1]) + 1,
                                    ord(bracket_content[i + 1][-1])):
                         next_char = chr(j)
                         if next_char in TRANSFORMATIONS:
                             bracket_content_temp.append(TRANSFORMATIONS[next_char])
                         else:
@@ -243,19 +242,27 @@
                 else:
                     bracket_content_temp.append(symbol)
                 if (i != 0 and bracket_content[i - 1] == "-"
                         and not previous_is_valid_for_range):
                     previous_is_valid_for_range = False
                 else:
                     previous_is_valid_for_range = True
+        bracket_content_temp = self._preprocess_negation(bracket_content_temp)
         bracket_content_temp = self._insert_or(bracket_content_temp)
         bracket_content_temp = self._recombine(bracket_content_temp)
         return bracket_content_temp
 
     @staticmethod
+    def _preprocess_negation(bracket_content):
+        if not bracket_content or bracket_content[0] != "^":
+            return bracket_content
+        # We inverse everything
+        return [x for x in ESCAPED_PRINTABLES if x not in bracket_content]
+
+    @staticmethod
     def _insert_or(l_to_modify):
         res = []
         for x in l_to_modify:
             res.append(x)
             res.append("|")
         if res:
             return res[:-1]
@@ -387,14 +394,16 @@
             elif (symbol == "]"
                   and not self._should_escape_next_symbol(regex_temp)):
                 in_brackets = False
             if (in_brackets
                     and not self._should_escape_next_symbol(regex_temp)
                     and symbol in TO_ESCAPE_IN_BRACKETS):
                 regex_temp.append("\\" + symbol)
+            elif self._should_escape_next_symbol(regex_temp):
+                regex_temp[-1] += symbol
             else:
                 regex_temp.append(symbol)
         self._python_regex = "".join(regex_temp)
 
     def _replace_shortcuts(self):
         for to_replace, replacement in SHORTCUTS.items():
             self._python_regex = self._python_regex.replace(to_replace,
```

### Comparing `pyformlang-1.0.8/pyformlang/regular_expression/regex.py` & `pyformlang-1.0.9/pyformlang/regular_expression/regex.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/regular_expression/regex_objects.py` & `pyformlang-1.0.9/pyformlang/regular_expression/regex_objects.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/regular_expression/regex_reader.py` & `pyformlang-1.0.9/pyformlang/regular_expression/regex_reader.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/regular_expression/tests/test_python_regex.py` & `pyformlang-1.0.9/pyformlang/regular_expression/tests/test_python_regex.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,7 +304,27 @@
         self._test_compare(r"ab{2,5}", "abbbbb")
         self._test_compare(r"ab{2,5}", "abbbbbbbbb")
         self._test_compare(r"[a-z]{1,3}", "")
         self._test_compare(r"[a-z]{1,3}", "d")
         self._test_compare(r"[a-z]{1,3}", "do")
         self._test_compare(r"[a-z]{1,3}", "dpo")
         self._test_compare(r"[a-z]{1,3}", "dpoz")
+
+    def test_error_backslash(self):
+        self._test_compare(r"[a\\\\\\]]", "\\]")
+        self._test_compare(r"\"([d\"\\\\]|\\\\.)*\"", '"d\\"')
+        self._test_compare(r"[a\\\\]", "a")
+
+    def test_negation_brackets(self):
+        self._test_compare(r"[^abc]*", "")
+        self._test_compare(r"[^abc]*", "a")
+        self._test_compare(r"[^abc]*", "b")
+        self._test_compare(r"[^abc]*", "c")
+        self._test_compare(r"[^abc]*", "d")
+        self._test_compare(r"[^abc]*", "dga")
+        self._test_compare(r"[^abc]*", "dgh")
+        self._test_compare(r"[^?]*", "dgh")
+
+    def test_question_mark(self):
+        self._test_compare(r".", "?")
+        self._test_compare(r"a(a|b)?", "a")
+        self._test_compare(r"a(a|b)\?", "ab?")
```

### Comparing `pyformlang-1.0.8/pyformlang/regular_expression/tests/test_regex.py` & `pyformlang-1.0.9/pyformlang/regular_expression/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/rsa/__init__.py` & `pyformlang-1.0.9/pyformlang/rsa/__init__.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/rsa/box.py` & `pyformlang-1.0.9/pyformlang/rsa/box.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/rsa/recursive_automaton.py` & `pyformlang-1.0.9/pyformlang/rsa/recursive_automaton.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang/rsa/tests/test_rsa.py` & `pyformlang-1.0.9/pyformlang/rsa/tests/test_rsa.py`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/pyformlang.egg-info/PKG-INFO` & `pyformlang-1.0.9/pyformlang.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyformlang
-Version: 1.0.8
+Version: 1.0.9
 Summary: A python framework for formal grammars
 Home-page: https://github.com/Aunsiels/pyformlang
 Author: Julien Romero
 Author-email: romerojulien34@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyformlang-1.0.8/pyformlang.egg-info/SOURCES.txt` & `pyformlang-1.0.9/pyformlang.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyformlang-1.0.8/setup.py` & `pyformlang-1.0.9/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     "networkx",
     "numpy",
     "pydot"
 ]
 
 setuptools.setup(
     name='pyformlang',
-    version='1.0.8',
+    version='1.0.9',
     #scripts=['pyformlang'] ,
     author="Julien Romero",
     author_email="romerojulien34@gmail.com",
     description="A python framework for formal grammars",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Aunsiels/pyformlang",
```

