# Comparing `tmp/pokerkit-0.4.8.tar.gz` & `tmp/pokerkit-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerkit-0.4.8.tar", last modified: Mon Jan 22 17:56:30 2024, max compression
+gzip compressed data, was "pokerkit-0.4.9.tar", last modified: Sun Jan 28 07:40:22 2024, max compression
```

## Comparing `pokerkit-0.4.8.tar` & `pokerkit-0.4.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-22 17:56:30.922065 pokerkit-0.4.8/
--rw-rw-r--   0 juho      (1000) juho      (1000)     1108 2024-01-19 00:50:06.000000 pokerkit-0.4.8/LICENSE
--rw-r--r--   0 juho      (1000) juho      (1000)    13785 2024-01-22 17:56:30.922065 pokerkit-0.4.8/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)    12149 2024-01-19 00:50:06.000000 pokerkit-0.4.8/README.rst
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-22 17:56:30.922065 pokerkit-0.4.8/pokerkit/
--rw-rw-r--   0 juho      (1000) juho      (1000)     4030 2024-01-20 20:38:54.000000 pokerkit-0.4.8/pokerkit/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    55107 2024-01-20 21:50:46.000000 pokerkit-0.4.8/pokerkit/games.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    19496 2024-01-19 00:50:06.000000 pokerkit-0.4.8/pokerkit/hands.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    13677 2024-01-19 00:50:06.000000 pokerkit-0.4.8/pokerkit/lookups.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    17238 2024-01-22 17:41:39.000000 pokerkit-0.4.8/pokerkit/notation.py
--rw-rw-r--   0 juho      (1000) juho      (1000)        0 2024-01-19 00:50:06.000000 pokerkit-0.4.8/pokerkit/py.typed
--rw-rw-r--   0 juho      (1000) juho      (1000)   146217 2024-01-20 20:53:53.000000 pokerkit-0.4.8/pokerkit/state.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-22 17:56:30.922065 pokerkit-0.4.8/pokerkit/tests/
--rw-rw-r--   0 juho      (1000) juho      (1000)       88 2024-01-19 00:50:06.000000 pokerkit-0.4.8/pokerkit/tests/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     4368 2024-01-19 00:50:06.000000 pokerkit-0.4.8/pokerkit/tests/test_lookups.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    30011 2024-01-22 17:43:18.000000 pokerkit-0.4.8/pokerkit/tests/test_papers.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    26921 2024-01-20 21:00:02.000000 pokerkit-0.4.8/pokerkit/tests/test_state.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     2062 2024-01-19 00:50:06.000000 pokerkit-0.4.8/pokerkit/tests/test_utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-22 17:56:30.922065 pokerkit-0.4.8/pokerkit/tests/test_wsop/
--rw-rw-r--   0 juho      (1000) juho      (1000)      141 2024-01-19 00:50:06.000000 pokerkit-0.4.8/pokerkit/tests/test_wsop/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)   193280 2024-01-19 00:50:06.000000 pokerkit-0.4.8/pokerkit/tests/test_wsop/test_2023_43.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    18245 2024-01-20 20:48:35.000000 pokerkit-0.4.8/pokerkit/utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-22 17:56:30.922065 pokerkit-0.4.8/pokerkit.egg-info/
--rw-r--r--   0 juho      (1000) juho      (1000)    13785 2024-01-22 17:56:30.000000 pokerkit-0.4.8/pokerkit.egg-info/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)      539 2024-01-22 17:56:30.000000 pokerkit-0.4.8/pokerkit.egg-info/SOURCES.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        1 2024-01-22 17:56:30.000000 pokerkit-0.4.8/pokerkit.egg-info/dependency_links.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        9 2024-01-22 17:56:30.000000 pokerkit-0.4.8/pokerkit.egg-info/top_level.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)       38 2024-01-22 17:56:30.922065 pokerkit-0.4.8/setup.cfg
--rw-rw-r--   0 juho      (1000) juho      (1000)     2105 2024-01-22 17:53:20.000000 pokerkit-0.4.8/setup.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-28 07:40:22.247020 pokerkit-0.4.9/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     1108 2024-01-19 00:50:06.000000 pokerkit-0.4.9/LICENSE
+-rw-r--r--   0 juho      (1000) juho      (1000)    13777 2024-01-28 07:40:22.247020 pokerkit-0.4.9/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)    12141 2024-01-28 07:31:06.000000 pokerkit-0.4.9/README.rst
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-28 07:40:22.247020 pokerkit-0.4.9/pokerkit/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     4030 2024-01-20 20:38:54.000000 pokerkit-0.4.9/pokerkit/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    55107 2024-01-20 21:50:46.000000 pokerkit-0.4.9/pokerkit/games.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    19496 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/hands.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    13677 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/lookups.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    17624 2024-01-28 07:03:04.000000 pokerkit-0.4.9/pokerkit/notation.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)        0 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/py.typed
+-rw-rw-r--   0 juho      (1000) juho      (1000)   146217 2024-01-20 20:53:53.000000 pokerkit-0.4.9/pokerkit/state.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-28 07:40:22.247020 pokerkit-0.4.9/pokerkit/tests/
+-rw-rw-r--   0 juho      (1000) juho      (1000)       88 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/tests/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     4368 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/tests/test_lookups.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    30011 2024-01-22 17:43:18.000000 pokerkit-0.4.9/pokerkit/tests/test_papers.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    26921 2024-01-20 21:00:02.000000 pokerkit-0.4.9/pokerkit/tests/test_state.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2062 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/tests/test_utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-28 07:40:22.247020 pokerkit-0.4.9/pokerkit/tests/test_wsop/
+-rw-rw-r--   0 juho      (1000) juho      (1000)      141 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/tests/test_wsop/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)   193280 2024-01-19 00:50:06.000000 pokerkit-0.4.9/pokerkit/tests/test_wsop/test_2023_43.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    18245 2024-01-20 20:48:35.000000 pokerkit-0.4.9/pokerkit/utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2024-01-28 07:40:22.247020 pokerkit-0.4.9/pokerkit.egg-info/
+-rw-r--r--   0 juho      (1000) juho      (1000)    13777 2024-01-28 07:40:22.000000 pokerkit-0.4.9/pokerkit.egg-info/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)      539 2024-01-28 07:40:22.000000 pokerkit-0.4.9/pokerkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        1 2024-01-28 07:40:22.000000 pokerkit-0.4.9/pokerkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        9 2024-01-28 07:40:22.000000 pokerkit-0.4.9/pokerkit.egg-info/top_level.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)       38 2024-01-28 07:40:22.247020 pokerkit-0.4.9/setup.cfg
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2105 2024-01-28 07:29:41.000000 pokerkit-0.4.9/setup.py
```

### Comparing `pokerkit-0.4.8/LICENSE` & `pokerkit-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/PKG-INFO` & `pokerkit-0.4.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerkit
-Version: 0.4.8
+Version: 0.4.9
 Summary: An open-source Python library for poker simulations and hand evaluations
 Home-page: https://github.com/uoftcprg/pokerkit
 Author: University of Toronto Computer Poker Research Group
 Author-email: uoftcprg@studentorg.utoronto.ca
 License: MIT
 Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pokerkit
@@ -30,51 +30,42 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
 PokerKit
 ========
 
-PokerKit is an open-source Python library for simulating poker games and
-evaluating poker hands, developed by the University of Toronto Computer Poker
-Research Group. PokerKit supports an extensive array of poker variants and it
-provides a flexible architecture for users to define their custom games. These
-facilities are exposed via an intuitive unified high-level programmatic API. The
-library can be used in a variety of use cases, from poker AI development, tool
-creation, to online poker casino implementation. PokerKit's reliability has been
-established through static type checking, extensive doctests, and unit tests,
-achieving 99% code coverage.
+PokerKit is an open-source Python library for simulating poker games and evaluating poker hands, developed by the University of Toronto Computer Poker Research Group. PokerKit supports an extensive array of poker variants and it provides a flexible architecture for users to define their custom games. These facilities are exposed via an intuitive unified high-level programmatic API. The library can be used in a variety of use cases, from poker AI development, and tool creation, to online poker casino implementation. PokerKit's reliability has been established through static type checking, extensive doctests, and unit tests, achieving 99% code coverage.
 
 Features
 --------
 
 * Extensive poker game logic for major and minor poker variants.
 * High-speed hand evaluations.
 * Customizable game states and parameters.
-* Robust implementation with static type checking and extensive unit tests and
-  doctests.
+* Robust implementation with static type checking and extensive unit tests and doctests.
+* Dataset of over 10,000 hand histories.
 
 Installation
 ------------
 
 The PokerKit library can be installed using pip:
 
 .. code-block:: bash
 
    pip install pokerkit
 
-Usage
------
+Usages
+------
 
-**The first televised million dollar pot between Tom Dwan and Phil
-Ivey.**
+**The first televised million-dollar pot between Tom Dwan and Phil Ivey.**
 
 Link: https://youtu.be/GnxFohpljqM
 
-Setup the game.
+Set up the game.
 
 .. code-block:: python
 
    from pokerkit import Automation, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
@@ -91,57 +82,57 @@
        500,  # Antes
        (1000, 2000),  # Blinds or straddles
        2000,  # Min-bet
        (1125600, 2000000, 553500),  # Starting stacks
        3,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('Ac2d')  # Ivey
    state.deal_hole('????')  # Antonius
    state.deal_hole('7h6h')  # Dwan
 
    state.complete_bet_or_raise_to(7000)  # Dwan
    state.complete_bet_or_raise_to(23000)  # Ivey
    state.fold()  # Antonius
    state.check_or_call()  # Dwan
 
-Below shows the flop dealing and actions.
+Below are the flop dealing and actions.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Jc3d5c')
 
    state.complete_bet_or_raise_to(35000)  # Ivey
    state.check_or_call()  # Dwan
 
-Below shows the turn dealing and actions.
+Below are the turn dealing and actions.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('4h')
 
    state.complete_bet_or_raise_to(90000)  # Ivey
    state.complete_bet_or_raise_to(232600)  # Dwan
    state.complete_bet_or_raise_to(1067100)  # Ivey
    state.check_or_call()  # Dwan
 
-Below shows the river dealing.
+Below is the river dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Jh')
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [572100, 1997500, 1109500]
 
 **An all-in hand between Xuan and Phua.**
 
@@ -166,15 +157,15 @@
        3000,  # Antes
        {-1: 3000},  # Blinds or straddles
        3000,  # Min-bet
        (495000, 232000, 362000, 403000, 301000, 204000),  # Starting stacks
        6,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('Th8h')  # Badziakouski
    state.deal_hole('QsJd')  # Zhong
    state.deal_hole('QhQd')  # Xuan
    state.deal_hole('8d7c')  # Jun
@@ -187,42 +178,42 @@
    state.fold()  # Jun
    state.complete_bet_or_raise_to(298000)  # Phua
    state.fold()  # Koon
    state.fold()  # Badziakouski
    state.fold()  # Zhong
    state.check_or_call()  # Xuan
 
-Below shows the flop dealing.
+Below is the flop dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('9h6cKc')
 
-Below shows the turn dealing.
+Below is the turn dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Jh')
 
-Below shows the river dealing.
+Below is the river dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Ts')
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [489000, 226000, 684000, 400000, 0, 198000]
 
-**The largest online poker pot every played between Patrik Antonius and Viktor
+**The largest online poker pot ever played between Patrik Antonius and Viktor
 Blom.**
 
 Link: https://youtu.be/UMBm66Id2AA
 
 .. code-block:: python
 
    from pokerkit import Automation, PotLimitOmahaHoldem
@@ -242,54 +233,54 @@
        0,  # Antes
        (500, 1000),  # Blinds or straddles
        1000,  # Min-bet
        (1259450.25, 678473.5),  # Starting stacks
        2,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('Ah3sKsKh')  # Antonius
    state.deal_hole('6d9s7d8h')  # Blom
 
    state.complete_bet_or_raise_to(3000)  # Blom
    state.complete_bet_or_raise_to(9000)  # Antonius
    state.complete_bet_or_raise_to(27000)  # Blom
    state.complete_bet_or_raise_to(81000)  # Antonius
    state.check_or_call()  # Blom
 
-Below shows the flop dealing and actions.
+Below are the flop dealing and actions.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('4s5c2h')
 
    state.complete_bet_or_raise_to(91000)  # Antonius
    state.complete_bet_or_raise_to(435000)  # Blom
    state.complete_bet_or_raise_to(779000)  # Antonius
    state.check_or_call()  # Blom
 
-Below shows the turn dealing.
+Below is the turn dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('5h')
 
-Below shows the river dealing.
+Below is the river dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('9c')
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [1937923.75, 0.0]
 
 **A bad beat between Yockey and Arieh.**
 
@@ -315,66 +306,66 @@
        (75000, 150000),  # Blinds or straddles
        150000,  # Small-bet
        300000,  # Big-bet
        (1180000, 4340000, 5910000, 10765000),  # Starting stacks
        4,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('7h6c4c3d2c')  # Yockey
    state.deal_hole('??????????')  # Hui
    state.deal_hole('??????????')  # Esposito
    state.deal_hole('AsQs6s5c3c')  # Arieh
 
    state.fold()  # Esposito
    state.complete_bet_or_raise_to()  # Arieh
    state.complete_bet_or_raise_to()  # Yockey
    state.fold()  # Hui
    state.check_or_call()  # Arieh
 
-Below shows the first draw and actions.
+Below are the first draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard()  # Yockey
    state.stand_pat_or_discard('AsQs')  # Arieh
    state.burn_card('??')
    state.deal_hole('2hQh')  # Arieh
 
    state.complete_bet_or_raise_to()  # Yockey
    state.check_or_call()  # Arieh
 
-Below shows the second draw and actions.
+Below are the second draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard()  # Yockey
    state.stand_pat_or_discard('Qh')  # Arieh
    state.burn_card('??')
    state.deal_hole('4d')  # Arieh
 
    state.complete_bet_or_raise_to()  # Yockey
    state.check_or_call()  # Arieh
 
-Below shows the third draw and actions.
+Below are the third draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard()  # Yockey
    state.stand_pat_or_discard('6s')  # Arieh
    state.burn_card('??')
    state.deal_hole('7c')  # Arieh
 
    state.complete_bet_or_raise_to()  # Yockey
    state.check_or_call()  # Arieh
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [0, 4190000, 5910000, 12095000]
 
 **An example badugi hand from Wikipedia.**
 
@@ -399,29 +390,29 @@
        (1, 2),  # Blinds or straddles
        2,  # Small-bet
        4,  # Big-bet
        200,  # Starting stacks
        4,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('????????')  # Bob
    state.deal_hole('????????')  # Carol
    state.deal_hole('????????')  # Ted
    state.deal_hole('????????')  # Alice
 
    state.fold()  # Ted
    state.check_or_call()  # Alice
    state.check_or_call()  # Bob
    state.check_or_call()  # Carol
 
-Below shows the first draw and actions.
+Below are the first draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard('????')  # Bob
    state.stand_pat_or_discard('????')  # Carol
    state.stand_pat_or_discard('??')  # Alice
    state.burn_card('??')
@@ -430,15 +421,15 @@
    state.deal_hole('??')  # Alice
 
    state.check_or_call()  # Bob
    state.complete_bet_or_raise_to()  # Carol
    state.check_or_call()  # Alice
    state.check_or_call()  # Bob
 
-Below shows the second draw and actions.
+Below are the second draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard('??')  # Bob
    state.stand_pat_or_discard()  # Carol
    state.stand_pat_or_discard('??')  # Alice
    state.burn_card('??')
@@ -447,52 +438,49 @@
 
    state.check_or_call()  # Bob
    state.complete_bet_or_raise_to()  # Carol
    state.complete_bet_or_raise_to()  # Alice
    state.fold()  # Bob
    state.check_or_call()  # Carol
 
-Below shows the third draw and actions.
+Below are the third draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard('??')  # Carol
    state.stand_pat_or_discard()  # Alice
    state.burn_card('??')
    state.deal_hole('??')  # Carol
 
    state.check_or_call()  # Carol
    state.complete_bet_or_raise_to()  # Alice
    state.check_or_call()  # Carol
 
-Below show the showdown.
+Below is the showdown.
 
 .. code-block:: python
 
    state.show_or_muck_hole_cards('2s4c6d9h')  # Alice
    state.show_or_muck_hole_cards('3s5d7c8h')  # Carol
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [196, 220, 200, 184]
 
 Testing and Validation
 ----------------------
 
-PokerKit has extensive test coverage, passes mypy static type checking with
-strict parameter, and has been validated through extensive use in real-life
-scenarios.
+PokerKit has extensive test coverage, passes mypy static type checking with strict parameter, and has been validated through extensive use in real-life scenarios.
 
 Contributing
 ------------
 
-Contributions are welcome! Please read our Contributing Guide for more
-information.
+Contributions are welcome! Please read our Contributing Guide for more information.
 
 License
 -------
 
 PokerKit is distributed under the MIT license.
 
 Citing
```

### Comparing `pokerkit-0.4.8/README.rst` & `pokerkit-0.4.9/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,39 @@
 ========
 PokerKit
 ========
 
-PokerKit is an open-source Python library for simulating poker games and
-evaluating poker hands, developed by the University of Toronto Computer Poker
-Research Group. PokerKit supports an extensive array of poker variants and it
-provides a flexible architecture for users to define their custom games. These
-facilities are exposed via an intuitive unified high-level programmatic API. The
-library can be used in a variety of use cases, from poker AI development, tool
-creation, to online poker casino implementation. PokerKit's reliability has been
-established through static type checking, extensive doctests, and unit tests,
-achieving 99% code coverage.
+PokerKit is an open-source Python library for simulating poker games and evaluating poker hands, developed by the University of Toronto Computer Poker Research Group. PokerKit supports an extensive array of poker variants and it provides a flexible architecture for users to define their custom games. These facilities are exposed via an intuitive unified high-level programmatic API. The library can be used in a variety of use cases, from poker AI development, and tool creation, to online poker casino implementation. PokerKit's reliability has been established through static type checking, extensive doctests, and unit tests, achieving 99% code coverage.
 
 Features
 --------
 
 * Extensive poker game logic for major and minor poker variants.
 * High-speed hand evaluations.
 * Customizable game states and parameters.
-* Robust implementation with static type checking and extensive unit tests and
-  doctests.
+* Robust implementation with static type checking and extensive unit tests and doctests.
+* Dataset of over 10,000 hand histories.
 
 Installation
 ------------
 
 The PokerKit library can be installed using pip:
 
 .. code-block:: bash
 
    pip install pokerkit
 
-Usage
------
+Usages
+------
 
-**The first televised million dollar pot between Tom Dwan and Phil
-Ivey.**
+**The first televised million-dollar pot between Tom Dwan and Phil Ivey.**
 
 Link: https://youtu.be/GnxFohpljqM
 
-Setup the game.
+Set up the game.
 
 .. code-block:: python
 
    from pokerkit import Automation, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
@@ -59,57 +50,57 @@
        500,  # Antes
        (1000, 2000),  # Blinds or straddles
        2000,  # Min-bet
        (1125600, 2000000, 553500),  # Starting stacks
        3,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('Ac2d')  # Ivey
    state.deal_hole('????')  # Antonius
    state.deal_hole('7h6h')  # Dwan
 
    state.complete_bet_or_raise_to(7000)  # Dwan
    state.complete_bet_or_raise_to(23000)  # Ivey
    state.fold()  # Antonius
    state.check_or_call()  # Dwan
 
-Below shows the flop dealing and actions.
+Below are the flop dealing and actions.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Jc3d5c')
 
    state.complete_bet_or_raise_to(35000)  # Ivey
    state.check_or_call()  # Dwan
 
-Below shows the turn dealing and actions.
+Below are the turn dealing and actions.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('4h')
 
    state.complete_bet_or_raise_to(90000)  # Ivey
    state.complete_bet_or_raise_to(232600)  # Dwan
    state.complete_bet_or_raise_to(1067100)  # Ivey
    state.check_or_call()  # Dwan
 
-Below shows the river dealing.
+Below is the river dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Jh')
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [572100, 1997500, 1109500]
 
 **An all-in hand between Xuan and Phua.**
 
@@ -134,15 +125,15 @@
        3000,  # Antes
        {-1: 3000},  # Blinds or straddles
        3000,  # Min-bet
        (495000, 232000, 362000, 403000, 301000, 204000),  # Starting stacks
        6,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('Th8h')  # Badziakouski
    state.deal_hole('QsJd')  # Zhong
    state.deal_hole('QhQd')  # Xuan
    state.deal_hole('8d7c')  # Jun
@@ -155,42 +146,42 @@
    state.fold()  # Jun
    state.complete_bet_or_raise_to(298000)  # Phua
    state.fold()  # Koon
    state.fold()  # Badziakouski
    state.fold()  # Zhong
    state.check_or_call()  # Xuan
 
-Below shows the flop dealing.
+Below is the flop dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('9h6cKc')
 
-Below shows the turn dealing.
+Below is the turn dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Jh')
 
-Below shows the river dealing.
+Below is the river dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Ts')
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [489000, 226000, 684000, 400000, 0, 198000]
 
-**The largest online poker pot every played between Patrik Antonius and Viktor
+**The largest online poker pot ever played between Patrik Antonius and Viktor
 Blom.**
 
 Link: https://youtu.be/UMBm66Id2AA
 
 .. code-block:: python
 
    from pokerkit import Automation, PotLimitOmahaHoldem
@@ -210,54 +201,54 @@
        0,  # Antes
        (500, 1000),  # Blinds or straddles
        1000,  # Min-bet
        (1259450.25, 678473.5),  # Starting stacks
        2,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('Ah3sKsKh')  # Antonius
    state.deal_hole('6d9s7d8h')  # Blom
 
    state.complete_bet_or_raise_to(3000)  # Blom
    state.complete_bet_or_raise_to(9000)  # Antonius
    state.complete_bet_or_raise_to(27000)  # Blom
    state.complete_bet_or_raise_to(81000)  # Antonius
    state.check_or_call()  # Blom
 
-Below shows the flop dealing and actions.
+Below are the flop dealing and actions.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('4s5c2h')
 
    state.complete_bet_or_raise_to(91000)  # Antonius
    state.complete_bet_or_raise_to(435000)  # Blom
    state.complete_bet_or_raise_to(779000)  # Antonius
    state.check_or_call()  # Blom
 
-Below shows the turn dealing.
+Below is the turn dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('5h')
 
-Below shows the river dealing.
+Below is the river dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('9c')
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [1937923.75, 0.0]
 
 **A bad beat between Yockey and Arieh.**
 
@@ -283,66 +274,66 @@
        (75000, 150000),  # Blinds or straddles
        150000,  # Small-bet
        300000,  # Big-bet
        (1180000, 4340000, 5910000, 10765000),  # Starting stacks
        4,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('7h6c4c3d2c')  # Yockey
    state.deal_hole('??????????')  # Hui
    state.deal_hole('??????????')  # Esposito
    state.deal_hole('AsQs6s5c3c')  # Arieh
 
    state.fold()  # Esposito
    state.complete_bet_or_raise_to()  # Arieh
    state.complete_bet_or_raise_to()  # Yockey
    state.fold()  # Hui
    state.check_or_call()  # Arieh
 
-Below shows the first draw and actions.
+Below are the first draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard()  # Yockey
    state.stand_pat_or_discard('AsQs')  # Arieh
    state.burn_card('??')
    state.deal_hole('2hQh')  # Arieh
 
    state.complete_bet_or_raise_to()  # Yockey
    state.check_or_call()  # Arieh
 
-Below shows the second draw and actions.
+Below are the second draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard()  # Yockey
    state.stand_pat_or_discard('Qh')  # Arieh
    state.burn_card('??')
    state.deal_hole('4d')  # Arieh
 
    state.complete_bet_or_raise_to()  # Yockey
    state.check_or_call()  # Arieh
 
-Below shows the third draw and actions.
+Below are the third draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard()  # Yockey
    state.stand_pat_or_discard('6s')  # Arieh
    state.burn_card('??')
    state.deal_hole('7c')  # Arieh
 
    state.complete_bet_or_raise_to()  # Yockey
    state.check_or_call()  # Arieh
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [0, 4190000, 5910000, 12095000]
 
 **An example badugi hand from Wikipedia.**
 
@@ -367,29 +358,29 @@
        (1, 2),  # Blinds or straddles
        2,  # Small-bet
        4,  # Big-bet
        200,  # Starting stacks
        4,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('????????')  # Bob
    state.deal_hole('????????')  # Carol
    state.deal_hole('????????')  # Ted
    state.deal_hole('????????')  # Alice
 
    state.fold()  # Ted
    state.check_or_call()  # Alice
    state.check_or_call()  # Bob
    state.check_or_call()  # Carol
 
-Below shows the first draw and actions.
+Below are the first draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard('????')  # Bob
    state.stand_pat_or_discard('????')  # Carol
    state.stand_pat_or_discard('??')  # Alice
    state.burn_card('??')
@@ -398,15 +389,15 @@
    state.deal_hole('??')  # Alice
 
    state.check_or_call()  # Bob
    state.complete_bet_or_raise_to()  # Carol
    state.check_or_call()  # Alice
    state.check_or_call()  # Bob
 
-Below shows the second draw and actions.
+Below are the second draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard('??')  # Bob
    state.stand_pat_or_discard()  # Carol
    state.stand_pat_or_discard('??')  # Alice
    state.burn_card('??')
@@ -415,52 +406,49 @@
 
    state.check_or_call()  # Bob
    state.complete_bet_or_raise_to()  # Carol
    state.complete_bet_or_raise_to()  # Alice
    state.fold()  # Bob
    state.check_or_call()  # Carol
 
-Below shows the third draw and actions.
+Below are the third draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard('??')  # Carol
    state.stand_pat_or_discard()  # Alice
    state.burn_card('??')
    state.deal_hole('??')  # Carol
 
    state.check_or_call()  # Carol
    state.complete_bet_or_raise_to()  # Alice
    state.check_or_call()  # Carol
 
-Below show the showdown.
+Below is the showdown.
 
 .. code-block:: python
 
    state.show_or_muck_hole_cards('2s4c6d9h')  # Alice
    state.show_or_muck_hole_cards('3s5d7c8h')  # Carol
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [196, 220, 200, 184]
 
 Testing and Validation
 ----------------------
 
-PokerKit has extensive test coverage, passes mypy static type checking with
-strict parameter, and has been validated through extensive use in real-life
-scenarios.
+PokerKit has extensive test coverage, passes mypy static type checking with strict parameter, and has been validated through extensive use in real-life scenarios.
 
 Contributing
 ------------
 
-Contributions are welcome! Please read our Contributing Guide for more
-information.
+Contributions are welcome! Please read our Contributing Guide for more information.
 
 License
 -------
 
 PokerKit is distributed under the MIT license.
 
 Citing
```

### Comparing `pokerkit-0.4.8/pokerkit/__init__.py` & `pokerkit-0.4.9/pokerkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit/games.py` & `pokerkit-0.4.9/pokerkit/games.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit/hands.py` & `pokerkit-0.4.9/pokerkit/hands.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit/lookups.py` & `pokerkit-0.4.9/pokerkit/lookups.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit/notation.py` & `pokerkit-0.4.9/pokerkit/notation.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from __future__ import annotations
 
 from collections.abc import Callable, Iterable, Iterator
 from collections import defaultdict, deque
 from dataclasses import asdict, dataclass, fields, KW_ONLY
+from functools import partial
 from operator import itemgetter
 from tomllib import loads as loads_toml
 from typing import Any, ClassVar, BinaryIO
 from warnings import warn
 import datetime
 
 from pokerkit.state import (
@@ -35,15 +36,15 @@
     FixedLimitTexasHoldem,
     NoLimitDeuceToSevenLowballSingleDraw,
     NoLimitShortDeckHoldem,
     NoLimitTexasHoldem,
     Poker,
     PotLimitOmahaHoldem,
 )
-from pokerkit.utilities import Card, divmod, parse_value
+from pokerkit.utilities import Card, divmod, parse_value, rake
 
 
 @dataclass
 class HandHistory(Iterable[State]):
     game_types: ClassVar[dict[str, type[Poker]]] = {
         'FT': FixedLimitTexasHoldem,
         'NT': NoLimitTexasHoldem,
@@ -262,14 +263,16 @@
         Automation.HAND_KILLING,
         Automation.CHIPS_PUSHING,
         Automation.CHIPS_PULLING,
     )
     """The automations."""
     divmod: Callable[[int, int], tuple[int, int]] = divmod
     """The divmod function."""
+    rake: Callable[[int], tuple[int, int]] = partial(rake, rake=0)
+    """The rake function."""
     parse_value: Callable[[str], int] = parse_value
     """The value parsing function."""
 
     @classmethod
     def _filter_non_fields(cls, **kwargs: Any) -> dict[str, Any]:
         field_names = {field.name for field in fields(cls)}
 
@@ -277,22 +280,33 @@
             if key not in field_names and not key.startswith('_'):
                 warn(f'unexpected field \'{key}\'')
                 kwargs.pop(key)
 
         return kwargs
 
     @classmethod
-    def loads(cls, s: str, **kwargs: Any) -> HandHistory:
+    def loads(
+            cls,
+            s: str,
+            *,
+            parse_value: Callable[[str], int] = parse_value,
+            **kwargs: Any,
+    ) -> HandHistory:
         """Load PHH from ``str`` object.
 
         :param s: The ``str`` object.
+        :param parse_value: The value parsing function.
         :param kwargs: The metadata.
         :return: The hand history object.
         """
-        return cls(**cls._filter_non_fields(**kwargs | loads_toml(s)))
+        return cls(
+            **cls._filter_non_fields(
+                **kwargs | loads_toml(s, parse_float=parse_value),
+            ),
+        )
 
     @classmethod
     def load(cls, fp: BinaryIO, **kwargs: Any) -> HandHistory:
         """Load PHH from a file pointer.
 
         :param fp: The file pointer.
         :param kwargs: The metadata.
```

### Comparing `pokerkit-0.4.8/pokerkit/state.py` & `pokerkit-0.4.9/pokerkit/state.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit/tests/test_lookups.py` & `pokerkit-0.4.9/pokerkit/tests/test_lookups.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit/tests/test_papers.py` & `pokerkit-0.4.9/pokerkit/tests/test_papers.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit/tests/test_state.py` & `pokerkit-0.4.9/pokerkit/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit/tests/test_utilities.py` & `pokerkit-0.4.9/pokerkit/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit/tests/test_wsop/test_2023_43.py` & `pokerkit-0.4.9/pokerkit/tests/test_wsop/test_2023_43.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit/utilities.py` & `pokerkit-0.4.9/pokerkit/utilities.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/pokerkit.egg-info/PKG-INFO` & `pokerkit-0.4.9/pokerkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pokerkit
-Version: 0.4.8
+Version: 0.4.9
 Summary: An open-source Python library for poker simulations and hand evaluations
 Home-page: https://github.com/uoftcprg/pokerkit
 Author: University of Toronto Computer Poker Research Group
 Author-email: uoftcprg@studentorg.utoronto.ca
 License: MIT
 Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pokerkit
@@ -30,51 +30,42 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
 PokerKit
 ========
 
-PokerKit is an open-source Python library for simulating poker games and
-evaluating poker hands, developed by the University of Toronto Computer Poker
-Research Group. PokerKit supports an extensive array of poker variants and it
-provides a flexible architecture for users to define their custom games. These
-facilities are exposed via an intuitive unified high-level programmatic API. The
-library can be used in a variety of use cases, from poker AI development, tool
-creation, to online poker casino implementation. PokerKit's reliability has been
-established through static type checking, extensive doctests, and unit tests,
-achieving 99% code coverage.
+PokerKit is an open-source Python library for simulating poker games and evaluating poker hands, developed by the University of Toronto Computer Poker Research Group. PokerKit supports an extensive array of poker variants and it provides a flexible architecture for users to define their custom games. These facilities are exposed via an intuitive unified high-level programmatic API. The library can be used in a variety of use cases, from poker AI development, and tool creation, to online poker casino implementation. PokerKit's reliability has been established through static type checking, extensive doctests, and unit tests, achieving 99% code coverage.
 
 Features
 --------
 
 * Extensive poker game logic for major and minor poker variants.
 * High-speed hand evaluations.
 * Customizable game states and parameters.
-* Robust implementation with static type checking and extensive unit tests and
-  doctests.
+* Robust implementation with static type checking and extensive unit tests and doctests.
+* Dataset of over 10,000 hand histories.
 
 Installation
 ------------
 
 The PokerKit library can be installed using pip:
 
 .. code-block:: bash
 
    pip install pokerkit
 
-Usage
------
+Usages
+------
 
-**The first televised million dollar pot between Tom Dwan and Phil
-Ivey.**
+**The first televised million-dollar pot between Tom Dwan and Phil Ivey.**
 
 Link: https://youtu.be/GnxFohpljqM
 
-Setup the game.
+Set up the game.
 
 .. code-block:: python
 
    from pokerkit import Automation, NoLimitTexasHoldem
 
    state = NoLimitTexasHoldem.create_state(
        # Automations
@@ -91,57 +82,57 @@
        500,  # Antes
        (1000, 2000),  # Blinds or straddles
        2000,  # Min-bet
        (1125600, 2000000, 553500),  # Starting stacks
        3,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('Ac2d')  # Ivey
    state.deal_hole('????')  # Antonius
    state.deal_hole('7h6h')  # Dwan
 
    state.complete_bet_or_raise_to(7000)  # Dwan
    state.complete_bet_or_raise_to(23000)  # Ivey
    state.fold()  # Antonius
    state.check_or_call()  # Dwan
 
-Below shows the flop dealing and actions.
+Below are the flop dealing and actions.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Jc3d5c')
 
    state.complete_bet_or_raise_to(35000)  # Ivey
    state.check_or_call()  # Dwan
 
-Below shows the turn dealing and actions.
+Below are the turn dealing and actions.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('4h')
 
    state.complete_bet_or_raise_to(90000)  # Ivey
    state.complete_bet_or_raise_to(232600)  # Dwan
    state.complete_bet_or_raise_to(1067100)  # Ivey
    state.check_or_call()  # Dwan
 
-Below shows the river dealing.
+Below is the river dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Jh')
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [572100, 1997500, 1109500]
 
 **An all-in hand between Xuan and Phua.**
 
@@ -166,15 +157,15 @@
        3000,  # Antes
        {-1: 3000},  # Blinds or straddles
        3000,  # Min-bet
        (495000, 232000, 362000, 403000, 301000, 204000),  # Starting stacks
        6,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('Th8h')  # Badziakouski
    state.deal_hole('QsJd')  # Zhong
    state.deal_hole('QhQd')  # Xuan
    state.deal_hole('8d7c')  # Jun
@@ -187,42 +178,42 @@
    state.fold()  # Jun
    state.complete_bet_or_raise_to(298000)  # Phua
    state.fold()  # Koon
    state.fold()  # Badziakouski
    state.fold()  # Zhong
    state.check_or_call()  # Xuan
 
-Below shows the flop dealing.
+Below is the flop dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('9h6cKc')
 
-Below shows the turn dealing.
+Below is the turn dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Jh')
 
-Below shows the river dealing.
+Below is the river dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('Ts')
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [489000, 226000, 684000, 400000, 0, 198000]
 
-**The largest online poker pot every played between Patrik Antonius and Viktor
+**The largest online poker pot ever played between Patrik Antonius and Viktor
 Blom.**
 
 Link: https://youtu.be/UMBm66Id2AA
 
 .. code-block:: python
 
    from pokerkit import Automation, PotLimitOmahaHoldem
@@ -242,54 +233,54 @@
        0,  # Antes
        (500, 1000),  # Blinds or straddles
        1000,  # Min-bet
        (1259450.25, 678473.5),  # Starting stacks
        2,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('Ah3sKsKh')  # Antonius
    state.deal_hole('6d9s7d8h')  # Blom
 
    state.complete_bet_or_raise_to(3000)  # Blom
    state.complete_bet_or_raise_to(9000)  # Antonius
    state.complete_bet_or_raise_to(27000)  # Blom
    state.complete_bet_or_raise_to(81000)  # Antonius
    state.check_or_call()  # Blom
 
-Below shows the flop dealing and actions.
+Below are the flop dealing and actions.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('4s5c2h')
 
    state.complete_bet_or_raise_to(91000)  # Antonius
    state.complete_bet_or_raise_to(435000)  # Blom
    state.complete_bet_or_raise_to(779000)  # Antonius
    state.check_or_call()  # Blom
 
-Below shows the turn dealing.
+Below is the turn dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('5h')
 
-Below shows the river dealing.
+Below is the river dealing.
 
 .. code-block:: python
 
    state.burn_card('??')
    state.deal_board('9c')
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [1937923.75, 0.0]
 
 **A bad beat between Yockey and Arieh.**
 
@@ -315,66 +306,66 @@
        (75000, 150000),  # Blinds or straddles
        150000,  # Small-bet
        300000,  # Big-bet
        (1180000, 4340000, 5910000, 10765000),  # Starting stacks
        4,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('7h6c4c3d2c')  # Yockey
    state.deal_hole('??????????')  # Hui
    state.deal_hole('??????????')  # Esposito
    state.deal_hole('AsQs6s5c3c')  # Arieh
 
    state.fold()  # Esposito
    state.complete_bet_or_raise_to()  # Arieh
    state.complete_bet_or_raise_to()  # Yockey
    state.fold()  # Hui
    state.check_or_call()  # Arieh
 
-Below shows the first draw and actions.
+Below are the first draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard()  # Yockey
    state.stand_pat_or_discard('AsQs')  # Arieh
    state.burn_card('??')
    state.deal_hole('2hQh')  # Arieh
 
    state.complete_bet_or_raise_to()  # Yockey
    state.check_or_call()  # Arieh
 
-Below shows the second draw and actions.
+Below are the second draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard()  # Yockey
    state.stand_pat_or_discard('Qh')  # Arieh
    state.burn_card('??')
    state.deal_hole('4d')  # Arieh
 
    state.complete_bet_or_raise_to()  # Yockey
    state.check_or_call()  # Arieh
 
-Below shows the third draw and actions.
+Below are the third draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard()  # Yockey
    state.stand_pat_or_discard('6s')  # Arieh
    state.burn_card('??')
    state.deal_hole('7c')  # Arieh
 
    state.complete_bet_or_raise_to()  # Yockey
    state.check_or_call()  # Arieh
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [0, 4190000, 5910000, 12095000]
 
 **An example badugi hand from Wikipedia.**
 
@@ -399,29 +390,29 @@
        (1, 2),  # Blinds or straddles
        2,  # Small-bet
        4,  # Big-bet
        200,  # Starting stacks
        4,  # Number of players
    )
 
-Below shows the pre-flop dealings and actions.
+Below are the pre-flop dealings and actions.
 
 .. code-block:: python
 
    state.deal_hole('????????')  # Bob
    state.deal_hole('????????')  # Carol
    state.deal_hole('????????')  # Ted
    state.deal_hole('????????')  # Alice
 
    state.fold()  # Ted
    state.check_or_call()  # Alice
    state.check_or_call()  # Bob
    state.check_or_call()  # Carol
 
-Below shows the first draw and actions.
+Below are the first draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard('????')  # Bob
    state.stand_pat_or_discard('????')  # Carol
    state.stand_pat_or_discard('??')  # Alice
    state.burn_card('??')
@@ -430,15 +421,15 @@
    state.deal_hole('??')  # Alice
 
    state.check_or_call()  # Bob
    state.complete_bet_or_raise_to()  # Carol
    state.check_or_call()  # Alice
    state.check_or_call()  # Bob
 
-Below shows the second draw and actions.
+Below are the second draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard('??')  # Bob
    state.stand_pat_or_discard()  # Carol
    state.stand_pat_or_discard('??')  # Alice
    state.burn_card('??')
@@ -447,52 +438,49 @@
 
    state.check_or_call()  # Bob
    state.complete_bet_or_raise_to()  # Carol
    state.complete_bet_or_raise_to()  # Alice
    state.fold()  # Bob
    state.check_or_call()  # Carol
 
-Below shows the third draw and actions.
+Below are the third draw and actions.
 
 .. code-block:: python
 
    state.stand_pat_or_discard('??')  # Carol
    state.stand_pat_or_discard()  # Alice
    state.burn_card('??')
    state.deal_hole('??')  # Carol
 
    state.check_or_call()  # Carol
    state.complete_bet_or_raise_to()  # Alice
    state.check_or_call()  # Carol
 
-Below show the showdown.
+Below is the showdown.
 
 .. code-block:: python
 
    state.show_or_muck_hole_cards('2s4c6d9h')  # Alice
    state.show_or_muck_hole_cards('3s5d7c8h')  # Carol
 
-Below show the final stacks.
+Below are the final stacks.
 
 .. code-block:: python
 
    print(state.stacks)  # [196, 220, 200, 184]
 
 Testing and Validation
 ----------------------
 
-PokerKit has extensive test coverage, passes mypy static type checking with
-strict parameter, and has been validated through extensive use in real-life
-scenarios.
+PokerKit has extensive test coverage, passes mypy static type checking with strict parameter, and has been validated through extensive use in real-life scenarios.
 
 Contributing
 ------------
 
-Contributions are welcome! Please read our Contributing Guide for more
-information.
+Contributions are welcome! Please read our Contributing Guide for more information.
 
 License
 -------
 
 PokerKit is distributed under the MIT license.
 
 Citing
```

### Comparing `pokerkit-0.4.8/pokerkit.egg-info/SOURCES.txt` & `pokerkit-0.4.9/pokerkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pokerkit-0.4.8/setup.py` & `pokerkit-0.4.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 from setuptools import find_packages, setup
 
 setup(
     name='pokerkit',
-    version='0.4.8',
+    version='0.4.9',
     description='An open-source Python library for poker simulations and hand evaluations',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
     url='https://github.com/uoftcprg/pokerkit',
     author='University of Toronto Computer Poker Research Group',
     author_email='uoftcprg@studentorg.utoronto.ca',
     license='MIT',
```

