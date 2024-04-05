# Comparing `tmp/sirji-messages-0.0.6.tar.gz` & `tmp/sirji-messages-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-messages-0.0.6.tar", last modified: Fri Apr  5 10:07:57 2024, max compression
+gzip compressed data, was "sirji-messages-0.0.7.tar", last modified: Fri Apr  5 12:36:42 2024, max compression
```

## Comparing `sirji-messages-0.0.6.tar` & `sirji-messages-0.0.7.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:57.119080 sirji-messages-0.0.6/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3916 2024-04-05 10:07:57.118447 sirji-messages-0.0.6/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3611 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 10:07:57.119697 sirji-messages-0.0.6/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      714 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:57.079034 sirji-messages-0.0.6/sirji_messages/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      591 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      610 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/action_enum.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      377 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/agent_enum.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      476 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/custom_exceptions.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:57.083958 sirji-messages-0.0.6/sirji_messages/messages/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:57.099146 sirji-messages-0.0.6/sirji_messages/messages/actions/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      654 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/acknowledge.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      723 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/answer.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1152 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      866 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/create_file.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/execute_command.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      724 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/feedback.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      744 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/generate_steps.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      798 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/infer.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      731 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/inform.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      747 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/install_package.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      706 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/output.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      809 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/problem_statement.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      775 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/question.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      811 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/read_dir.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/read_file.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      712 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/response.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      786 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/solution_complete.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      765 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/step_completed.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      738 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/step_started.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      783 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/steps.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      759 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/train_using_search_term.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      750 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/train_using_url.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      732 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/actions/training_output.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2852 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/messages/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3806 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/parser.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2394 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/permissions.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:57.099905 sirji-messages-0.0.6/sirji_messages/system_prompts/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/system_prompts/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:57.104568 sirji-messages-0.0.6/sirji_messages/system_prompts/agents/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/system_prompts/agents/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4447 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/system_prompts/agents/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2442 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/system_prompts/agents/coder.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      987 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/system_prompts/agents/executor.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1750 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/system_prompts/agents/planner.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      755 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/system_prompts/agents/researcher.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      883 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/system_prompts/agents/user.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1111 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/sirji_messages/system_prompts/factory.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:57.117371 sirji-messages-0.0.6/sirji_messages.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3916 2024-04-05 10:07:56.000000 sirji-messages-0.0.6/sirji_messages.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2329 2024-04-05 10:07:57.000000 sirji-messages-0.0.6/sirji_messages.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 10:07:56.000000 sirji-messages-0.0.6/sirji_messages.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       21 2024-04-05 10:07:56.000000 sirji-messages-0.0.6/sirji_messages.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:57.105474 sirji-messages-0.0.6/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:57.111134 sirji-messages-0.0.6/tests/integration/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/integration/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1454 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/integration/test_message_factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1806 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/integration/test_system_prompts.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      814 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/integration/test_system_prompts_base.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:57.116441 sirji-messages-0.0.6/tests/unit/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/unit/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      900 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/unit/test_actions_base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      633 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/unit/test_custom_exceptions.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1266 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/unit/test_enums.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2479 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/unit/test_parser.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1609 2024-04-05 10:07:39.000000 sirji-messages-0.0.6/tests/unit/test_permissions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:42.467895 sirji-messages-0.0.7/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3916 2024-04-05 12:36:42.467414 sirji-messages-0.0.7/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3611 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 12:36:42.467997 sirji-messages-0.0.7/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      714 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:42.446889 sirji-messages-0.0.7/sirji_messages/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      591 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      610 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/action_enum.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      377 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/agent_enum.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      476 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/custom_exceptions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:42.449116 sirji-messages-0.0.7/sirji_messages/messages/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:42.459066 sirji-messages-0.0.7/sirji_messages/messages/actions/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      654 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/acknowledge.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      723 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/answer.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1152 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      866 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/create_file.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/execute_command.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      724 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/feedback.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      744 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/generate_steps.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      798 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/infer.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      731 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/inform.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      747 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/install_package.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      706 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/output.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      809 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/problem_statement.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      775 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/question.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      811 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/read_dir.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/read_file.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      712 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/response.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      786 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/solution_complete.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      765 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/step_completed.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      738 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/step_started.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      783 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/steps.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      759 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/train_using_search_term.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      750 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/train_using_url.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      732 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/actions/training_output.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2852 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/messages/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4443 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/parser.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2394 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/permissions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:42.459759 sirji-messages-0.0.7/sirji_messages/system_prompts/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/system_prompts/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:42.462611 sirji-messages-0.0.7/sirji_messages/system_prompts/agents/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/system_prompts/agents/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4447 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/system_prompts/agents/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2442 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/system_prompts/agents/coder.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      987 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/system_prompts/agents/executor.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1750 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/system_prompts/agents/planner.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      755 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/system_prompts/agents/researcher.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      883 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/system_prompts/agents/user.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1111 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/sirji_messages/system_prompts/factory.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:42.466932 sirji-messages-0.0.7/sirji_messages.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3916 2024-04-05 12:36:42.000000 sirji-messages-0.0.7/sirji_messages.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2329 2024-04-05 12:36:42.000000 sirji-messages-0.0.7/sirji_messages.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 12:36:42.000000 sirji-messages-0.0.7/sirji_messages.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       21 2024-04-05 12:36:42.000000 sirji-messages-0.0.7/sirji_messages.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:42.462990 sirji-messages-0.0.7/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:42.464341 sirji-messages-0.0.7/tests/integration/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/integration/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1454 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/integration/test_message_factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1806 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/integration/test_system_prompts.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      814 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/integration/test_system_prompts_base.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:42.466473 sirji-messages-0.0.7/tests/unit/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/unit/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      900 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/unit/test_actions_base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      633 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/unit/test_custom_exceptions.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1266 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/unit/test_enums.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2479 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/unit/test_parser.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1609 2024-04-05 12:36:38.000000 sirji-messages-0.0.7/tests/unit/test_permissions.py
```

### Comparing `sirji-messages-0.0.6/LICENSE` & `sirji-messages-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/PKG-INFO` & `sirji-messages-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-messages
-Version: 0.0.6
+Version: 0.0.7
 Summary: Sirji messaging protocol implementation to create, validate and parse messages.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sirji-messages-0.0.6/README.md` & `sirji-messages-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/setup.py` & `sirji-messages-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-messages',
-    version='0.0.6',
+    version='0.0.7',
     author='Sirji',
     description='Sirji messaging protocol implementation to create, validate and parse messages.',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
```

### Comparing `sirji-messages-0.0.6/sirji_messages/__init__.py` & `sirji-messages-0.0.7/sirji_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/action_enum.py` & `sirji-messages-0.0.7/sirji_messages/action_enum.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/acknowledge.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/acknowledge.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/answer.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/answer.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/base.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/create_file.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/create_file.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/execute_command.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/execute_command.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/feedback.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/feedback.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/generate_steps.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/generate_steps.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/infer.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/infer.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/inform.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/inform.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/install_package.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/install_package.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/output.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/output.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/problem_statement.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/problem_statement.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/question.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/question.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/read_dir.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/read_dir.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/read_file.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/read_file.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/response.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/response.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/solution_complete.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/solution_complete.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/step_completed.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/step_completed.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/step_started.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/step_started.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/steps.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/steps.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/train_using_search_term.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/train_using_search_term.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/train_using_url.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/train_using_url.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/actions/training_output.py` & `sirji-messages-0.0.7/sirji_messages/messages/actions/training_output.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/messages/factory.py` & `sirji-messages-0.0.7/sirji_messages/messages/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/parser.py` & `sirji-messages-0.0.7/sirji_messages/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .messages.factory import MessageFactory
 from .custom_exceptions import MessageParsingError, MessageValidationError
 from .action_enum import ActionEnum
 from sirji_messages import validate_permission
 
 
 def parse(input_message):
+    input_message = _discard_format_deviations(input_message)
     lines = _validate_message(input_message)
     message_info = _extract_message_info(lines)
     payload = "\n".join(lines[3:])
     custom_properties = MessageFactory[message_info["ACTION"]].custom_properties()
 
     payload_dict = _parse_payload(payload, custom_properties)
 
@@ -17,14 +18,29 @@
 
     if parsed_message.get("ACTION") == ActionEnum.STEPS.name:
         parsed_message = {
             **parsed_message, "PARSED_STEPS": _parse_steps(parsed_message)}
 
     return parsed_message
 
+def _discard_format_deviations(input_message):
+    input_message = input_message.strip()
+
+    # Locate the positions of the first and last backticks (`).
+    start_index = input_message.find("```")
+    end_index = input_message.rfind("```")
+
+    # Extract the message prefix, message, and message suffix.
+    message_prefix = input_message[:start_index].strip()
+    # Including backticks as part of the message content.
+    message_content = input_message[start_index:end_index+3].strip()
+    message_suffix = input_message[end_index+3:].strip()
+
+    return message_content
+
 
 def _validate_message(message):
     message = message.strip()
     if not (message.startswith("```") and message.endswith("```")):
         raise MessageValidationError("Message must start and end with ```")
     message = message[3:-3].strip()
     lines = message.split("\n")
```

### Comparing `sirji-messages-0.0.6/sirji_messages/permissions.py` & `sirji-messages-0.0.7/sirji_messages/permissions.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/system_prompts/agents/base.py` & `sirji-messages-0.0.7/sirji_messages/system_prompts/agents/base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/system_prompts/agents/coder.py` & `sirji-messages-0.0.7/sirji_messages/system_prompts/agents/coder.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/system_prompts/agents/executor.py` & `sirji-messages-0.0.7/sirji_messages/system_prompts/agents/executor.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/system_prompts/agents/planner.py` & `sirji-messages-0.0.7/sirji_messages/system_prompts/agents/planner.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/system_prompts/agents/researcher.py` & `sirji-messages-0.0.7/sirji_messages/system_prompts/agents/researcher.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/system_prompts/agents/user.py` & `sirji-messages-0.0.7/sirji_messages/system_prompts/agents/user.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages/system_prompts/factory.py` & `sirji-messages-0.0.7/sirji_messages/system_prompts/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/sirji_messages.egg-info/PKG-INFO` & `sirji-messages-0.0.7/sirji_messages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-messages
-Version: 0.0.6
+Version: 0.0.7
 Summary: Sirji messaging protocol implementation to create, validate and parse messages.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sirji-messages-0.0.6/sirji_messages.egg-info/SOURCES.txt` & `sirji-messages-0.0.7/sirji_messages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/tests/integration/test_message_factory.py` & `sirji-messages-0.0.7/tests/integration/test_message_factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/tests/integration/test_system_prompts.py` & `sirji-messages-0.0.7/tests/integration/test_system_prompts.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/tests/integration/test_system_prompts_base.py` & `sirji-messages-0.0.7/tests/integration/test_system_prompts_base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/tests/unit/test_actions_base.py` & `sirji-messages-0.0.7/tests/unit/test_actions_base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/tests/unit/test_custom_exceptions.py` & `sirji-messages-0.0.7/tests/unit/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/tests/unit/test_enums.py` & `sirji-messages-0.0.7/tests/unit/test_enums.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/tests/unit/test_parser.py` & `sirji-messages-0.0.7/tests/unit/test_parser.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.6/tests/unit/test_permissions.py` & `sirji-messages-0.0.7/tests/unit/test_permissions.py`

 * *Files identical despite different names*

