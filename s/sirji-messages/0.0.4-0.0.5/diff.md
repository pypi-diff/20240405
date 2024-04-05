# Comparing `tmp/sirji-messages-0.0.4.tar.gz` & `tmp/sirji-messages-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-messages-0.0.4.tar", last modified: Thu Apr  4 13:11:07 2024, max compression
+gzip compressed data, was "sirji-messages-0.0.5.tar", last modified: Fri Apr  5 09:36:16 2024, max compression
```

## Comparing `sirji-messages-0.0.4.tar` & `sirji-messages-0.0.5.tar`

### file list

```diff
@@ -1,70 +1,72 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.858721 sirji-messages-0.0.4/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3916 2024-04-04 13:11:07.858117 sirji-messages-0.0.4/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3611 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-04 13:11:07.858853 sirji-messages-0.0.4/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      714 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.825589 sirji-messages-0.0.4/sirji_messages/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      591 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      565 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/action_enum.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      377 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/agent_enum.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      476 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/custom_exceptions.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.828518 sirji-messages-0.0.4/sirji_messages/messages/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.843010 sirji-messages-0.0.4/sirji_messages/messages/actions/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      654 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/acknowledge.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      723 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/answer.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1152 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      866 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/create_file.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/execute_command.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      724 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/feedback.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      744 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/generate_steps.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      798 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/infer.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      731 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/inform.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      747 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/install_package.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      706 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/output.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      809 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/problem_statement.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      775 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/question.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      712 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/response.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      786 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/solution_complete.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      765 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/step_completed.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      738 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/step_started.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      783 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/steps.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      759 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/train_using_search_term.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      750 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/train_using_url.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      732 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/actions/training_output.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2668 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/messages/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3807 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/parser.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2335 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/permissions.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.844040 sirji-messages-0.0.4/sirji_messages/system_prompts/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.848342 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4447 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2469 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/coder.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      822 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/executor.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1676 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/planner.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      755 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/researcher.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      883 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/agents/user.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1111 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/sirji_messages/system_prompts/factory.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.857559 sirji-messages-0.0.4/sirji_messages.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3916 2024-04-04 13:11:07.000000 sirji-messages-0.0.4/sirji_messages.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2240 2024-04-04 13:11:07.000000 sirji-messages-0.0.4/sirji_messages.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-04 13:11:07.000000 sirji-messages-0.0.4/sirji_messages.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       21 2024-04-04 13:11:07.000000 sirji-messages-0.0.4/sirji_messages.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.849262 sirji-messages-0.0.4/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.852034 sirji-messages-0.0.4/tests/integration/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/integration/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1454 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/integration/test_message_factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1806 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/integration/test_system_prompts.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      814 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/integration/test_system_prompts_base.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:11:07.856639 sirji-messages-0.0.4/tests/unit/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      900 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/test_actions_base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      633 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/test_custom_exceptions.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1266 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/test_enums.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2479 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/test_parser.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1609 2024-04-04 13:10:51.000000 sirji-messages-0.0.4/tests/unit/test_permissions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:16.542063 sirji-messages-0.0.5/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       15 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3916 2024-04-05 09:36:16.541272 sirji-messages-0.0.5/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3611 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-05 09:36:16.542244 sirji-messages-0.0.5/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      714 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:16.513222 sirji-messages-0.0.5/sirji_messages/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      591 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      610 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/action_enum.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      377 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/agent_enum.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      476 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/custom_exceptions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:16.516229 sirji-messages-0.0.5/sirji_messages/messages/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:16.530308 sirji-messages-0.0.5/sirji_messages/messages/actions/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      654 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/acknowledge.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      723 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/answer.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1152 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      866 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/create_file.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/execute_command.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      724 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/feedback.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      744 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/generate_steps.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      798 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/infer.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      731 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/inform.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      747 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/install_package.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      706 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/output.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      809 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/problem_statement.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      775 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/question.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      811 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/read_dir.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/read_file.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      712 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/response.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      786 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/solution_complete.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      765 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/step_completed.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      738 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/step_started.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      783 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/steps.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      759 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/train_using_search_term.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      750 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/train_using_url.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      732 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/actions/training_output.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2852 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/messages/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3807 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/parser.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2394 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/permissions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:16.531190 sirji-messages-0.0.5/sirji_messages/system_prompts/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/system_prompts/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:16.535631 sirji-messages-0.0.5/sirji_messages/system_prompts/agents/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/system_prompts/agents/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4447 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/system_prompts/agents/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2476 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/system_prompts/agents/coder.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      987 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/system_prompts/agents/executor.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1750 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/system_prompts/agents/planner.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      755 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/system_prompts/agents/researcher.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      883 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/system_prompts/agents/user.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1111 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/sirji_messages/system_prompts/factory.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:16.540799 sirji-messages-0.0.5/sirji_messages.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3916 2024-04-05 09:36:16.000000 sirji-messages-0.0.5/sirji_messages.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2329 2024-04-05 09:36:16.000000 sirji-messages-0.0.5/sirji_messages.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-05 09:36:16.000000 sirji-messages-0.0.5/sirji_messages.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       21 2024-04-05 09:36:16.000000 sirji-messages-0.0.5/sirji_messages.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:16.536155 sirji-messages-0.0.5/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:16.537644 sirji-messages-0.0.5/tests/integration/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/integration/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1454 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/integration/test_message_factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1806 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/integration/test_system_prompts.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      814 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/integration/test_system_prompts_base.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:16.540349 sirji-messages-0.0.5/tests/unit/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/unit/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      900 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/unit/test_actions_base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      633 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/unit/test_custom_exceptions.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1266 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/unit/test_enums.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2479 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/unit/test_parser.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1609 2024-04-05 09:36:02.000000 sirji-messages-0.0.5/tests/unit/test_permissions.py
```

### Comparing `sirji-messages-0.0.4/LICENSE` & `sirji-messages-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/PKG-INFO` & `sirji-messages-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-messages
-Version: 0.0.4
+Version: 0.0.5
 Summary: Sirji messaging protocol implementation to create, validate and parse messages.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sirji-messages-0.0.4/README.md` & `sirji-messages-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/setup.py` & `sirji-messages-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-messages',
-    version='0.0.4',
+    version='0.0.5',
     author='Sirji',
     description='Sirji messaging protocol implementation to create, validate and parse messages.',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
```

### Comparing `sirji-messages-0.0.4/sirji_messages/__init__.py` & `sirji-messages-0.0.5/sirji_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/action_enum.py` & `sirji-messages-0.0.5/sirji_messages/action_enum.py`

 * *Files 23% similar despite different names*

```diff
@@ -18,7 +18,9 @@
     STEP_COMPLETED = auto()
     STEP_STARTED = auto()
     STEPS = auto()
     TRAIN_USING_SEARCH_TERM = auto()
     TRAIN_USING_URL = auto()
     FEEDBACK = auto()
     TRAINING_OUTPUT = auto()
+    READ_FILE = auto()
+    READ_DIR = auto()
```

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/acknowledge.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/acknowledge.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/answer.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/answer.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/base.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/create_file.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/create_file.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/execute_command.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/execute_command.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/feedback.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/feedback.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/generate_steps.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/generate_steps.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/infer.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/infer.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/inform.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/inform.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/install_package.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/install_package.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/output.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/output.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/problem_statement.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/problem_statement.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/question.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/question.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/response.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/response.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/solution_complete.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/solution_complete.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/step_completed.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/step_completed.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/step_started.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/step_started.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/steps.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/steps.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/train_using_search_term.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/train_using_search_term.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/train_using_url.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/train_using_url.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/actions/training_output.py` & `sirji-messages-0.0.5/sirji_messages/messages/actions/training_output.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/messages/factory.py` & `sirji-messages-0.0.5/sirji_messages/messages/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from .actions.step_completed import StepCompletedMessage
 from .actions.step_started import StepStartedMessage
 from .actions.steps import StepsMessage
 from .actions.train_using_search_term import TrainUsingSearchTermMessage
 from .actions.train_using_url import TrainUsingUrlMessage
 from .actions.feedback import FeedbackMessage
 from .actions.training_output import TrainingOutputMessage
+from .actions.read_dir import ReadDirMessage
+from .actions.read_file import ReadFileMessage
 
 
 class MetaMessageFactory(type):
     def __getitem__(cls, action):
         try:
             action_type = ActionEnum[action]
             return cls._message_map[action_type]
@@ -54,10 +56,12 @@
         ActionEnum.SOLUTION_COMPLETE: SolutionCompleteMessage,
         ActionEnum.STEP_COMPLETED: StepCompletedMessage,
         ActionEnum.STEP_STARTED: StepStartedMessage,
         ActionEnum.STEPS: StepsMessage,
         ActionEnum.TRAIN_USING_SEARCH_TERM: TrainUsingSearchTermMessage,
         ActionEnum.TRAIN_USING_URL: TrainUsingUrlMessage,
         ActionEnum.FEEDBACK: FeedbackMessage,
-        ActionEnum.TRAINING_OUTPUT: TrainingOutputMessage
+        ActionEnum.TRAINING_OUTPUT: TrainingOutputMessage,
+        ActionEnum.READ_DIR: ReadDirMessage,
+        ActionEnum.READ_FILE: ReadFileMessage
     }
```

### Comparing `sirji-messages-0.0.4/sirji_messages/parser.py` & `sirji-messages-0.0.5/sirji_messages/parser.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/permissions.py` & `sirji-messages-0.0.5/sirji_messages/permissions.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 # Defining permissions_dict
 # Key: (from_agent, to_agent)
 # Value: set of allowed actions between the agents
 permissions_dict = {
     (AgentEnum.CODER, AgentEnum.EXECUTOR): {
         ActionEnum.CREATE_FILE,
         ActionEnum.EXECUTE_COMMAND,
-        ActionEnum.INSTALL_PACKAGE
+        ActionEnum.INSTALL_PACKAGE,
+        ActionEnum.READ_FILE,
+        ActionEnum.READ_DIR
     },
     (AgentEnum.CODER, AgentEnum.PLANNER): (
         ActionEnum.GENERATE_STEPS
     ),
     (AgentEnum.CODER, AgentEnum.RESEARCHER): (
         ActionEnum.TRAIN_USING_URL,
         ActionEnum.INFER
```

### Comparing `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/base.py` & `sirji-messages-0.0.5/sirji_messages/system_prompts/agents/base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/coder.py` & `sirji-messages-0.0.5/sirji_messages/system_prompts/agents/coder.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             - Identify URLs (Excluding GitHub) present in the PS, on which you have no knowledge and want to be trained on or researched. After training, infer from the trained content/knowledge. If the response of the inference has new URLs (Excluding GitHub), on which you have no knowledge, you can get trained on them too.
             - Get the list of non-technical steps generated before you start solving the problem statement (PS).
             - Follow the generated non-technical steps sequentially to solve the PS.
             - Ask questions, if essential.                             
             - Always notify about the step started before you start working on it. Similarly, notify about the step completed before you move to the next step.
             - Follow secure software development practices while generating code.
             - Ensure that you don't create any file/folder outside of current directory, i.e. './'
-            - Read the GitHub files by first cloning the repository and then reading the files. 
+            - Read the GitHub files by first cloning the repository and then reading the files at once.
             - Ensure that every code and command execution output is always written in a log file using packages like "tee" and execute in background using "nohup". For example: nohup command | tee <<log file name which can be used to check the output>> &                           
             - Only interact with the agents listed below using the allowed responses, also mentioned below.
             - Ensure the response is also enclosed inside 3 backticks (```).
             - End the conversation if you find that the PS cannot be solved programmatically or your solution is complete.
             """)
 
     def capabilities(self):
```

### Comparing `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/executor.py` & `sirji-messages-0.0.5/sirji_messages/system_prompts/agents/executor.py`

 * *Files 24% similar despite different names*

```diff
@@ -21,13 +21,15 @@
     def responsibilities(self):
         return ""  # This will never be called.
 
     def capabilities(self):
         return textwrap.dedent("""
           - Interact with macOS terminal.
           - Create or update files on macOS.
+          - Read content from a single file.
+          - Read the content from all files in a directory and all its subdirectories at once (separated by a divider).
           - Install required dependencies/packages/libraries on macOS.
           - Execute code on macOS.
           """)
 
     def ending_prompt(self):
         return ""  # This will never be called.
```

### Comparing `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/planner.py` & `sirji-messages-0.0.5/sirji_messages/system_prompts/agents/planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     def responsibilities(self):
         return textwrap.dedent(f"""
           - Pay close attention to PS while generating non-technical steps to solve the problem programmatically.
           - Use Python, if the programming language cannot be inferred from PS.
           - Ensure that each step in the list of steps should start with 'Step #: ....'                    
           - Don't explain the steps further using sub-steps.
           - Generate concise steps enough to solve the problem statement.
-          - Ensure that all the steps should be about either create file or install package or execute command or execute code to debug or git clone or read files.
+          - Ensure that all the steps are about either create file or install package or execute command or execute code to debug or git clone or read single file or read all files in a directory (including those in its subdirectories).
           - Always add a step to execute the code and evaluate the response output. If the response has errors, solve them before moving ahead.                   
-          - Focus on particular data points given in the PS and not solve the problem in a over-generalized manner.
+          - Focus on particular data points given in the PS and not solve the problem in an over-generalized manner.
           """)
 
     def capabilities(self):
         return textwrap.dedent("""
           - Generate non-technical steps to solve the problem programmatically.
           """)
```

### Comparing `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/researcher.py` & `sirji-messages-0.0.5/sirji_messages/system_prompts/agents/researcher.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/system_prompts/agents/user.py` & `sirji-messages-0.0.5/sirji_messages/system_prompts/agents/user.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages/system_prompts/factory.py` & `sirji-messages-0.0.5/sirji_messages/system_prompts/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/sirji_messages.egg-info/PKG-INFO` & `sirji-messages-0.0.5/sirji_messages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirji-messages
-Version: 0.0.4
+Version: 0.0.5
 Summary: Sirji messaging protocol implementation to create, validate and parse messages.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sirji-messages-0.0.4/sirji_messages.egg-info/SOURCES.txt` & `sirji-messages-0.0.5/sirji_messages.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,16 @@
 sirji_messages/messages/actions/generate_steps.py
 sirji_messages/messages/actions/infer.py
 sirji_messages/messages/actions/inform.py
 sirji_messages/messages/actions/install_package.py
 sirji_messages/messages/actions/output.py
 sirji_messages/messages/actions/problem_statement.py
 sirji_messages/messages/actions/question.py
+sirji_messages/messages/actions/read_dir.py
+sirji_messages/messages/actions/read_file.py
 sirji_messages/messages/actions/response.py
 sirji_messages/messages/actions/solution_complete.py
 sirji_messages/messages/actions/step_completed.py
 sirji_messages/messages/actions/step_started.py
 sirji_messages/messages/actions/steps.py
 sirji_messages/messages/actions/train_using_search_term.py
 sirji_messages/messages/actions/train_using_url.py
```

### Comparing `sirji-messages-0.0.4/tests/integration/test_message_factory.py` & `sirji-messages-0.0.5/tests/integration/test_message_factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/tests/integration/test_system_prompts.py` & `sirji-messages-0.0.5/tests/integration/test_system_prompts.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/tests/integration/test_system_prompts_base.py` & `sirji-messages-0.0.5/tests/integration/test_system_prompts_base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/tests/unit/test_actions_base.py` & `sirji-messages-0.0.5/tests/unit/test_actions_base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/tests/unit/test_custom_exceptions.py` & `sirji-messages-0.0.5/tests/unit/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/tests/unit/test_enums.py` & `sirji-messages-0.0.5/tests/unit/test_enums.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/tests/unit/test_parser.py` & `sirji-messages-0.0.5/tests/unit/test_parser.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.4/tests/unit/test_permissions.py` & `sirji-messages-0.0.5/tests/unit/test_permissions.py`

 * *Files identical despite different names*

