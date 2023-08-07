# Comparing `tmp/pokerkit-0.0.0.tar.gz` & `tmp/pokerkit-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pokerkit-0.0.0.tar", last modified: Wed Aug  2 20:42:02 2023, max compression
+gzip compressed data, was "pokerkit-0.0.1.tar", last modified: Mon Aug  7 15:46:43 2023, max compression
```

## Comparing `pokerkit-0.0.0.tar` & `pokerkit-0.0.1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2023-08-02 20:42:02.191630 pokerkit-0.0.0/
--rw-rw-r--   0 juho      (1000) juho      (1000)     1108 2023-07-21 19:50:32.000000 pokerkit-0.0.0/LICENSE
--rw-rw-r--   0 juho      (1000) juho      (1000)    11881 2023-08-02 20:42:02.191630 pokerkit-0.0.0/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)    10553 2023-08-02 20:16:49.000000 pokerkit-0.0.0/README.rst
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2023-08-02 20:42:02.191630 pokerkit-0.0.0/pokerkit/
--rw-rw-r--   0 juho      (1000) juho      (1000)     2675 2023-08-02 20:14:24.000000 pokerkit-0.0.0/pokerkit/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    47584 2023-08-02 20:15:09.000000 pokerkit-0.0.0/pokerkit/games.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    21639 2023-08-02 20:13:36.000000 pokerkit-0.0.0/pokerkit/hands.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    15580 2023-08-02 20:12:59.000000 pokerkit-0.0.0/pokerkit/lookups.py
--rw-rw-r--   0 juho      (1000) juho      (1000)        0 2023-08-02 20:39:04.000000 pokerkit-0.0.0/pokerkit/py.typed
--rw-rw-r--   0 juho      (1000) juho      (1000)   117600 2023-08-02 20:08:52.000000 pokerkit-0.0.0/pokerkit/state.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2023-08-02 20:42:02.191630 pokerkit-0.0.0/pokerkit/tests/
--rw-rw-r--   0 juho      (1000) juho      (1000)       88 2023-07-21 19:50:32.000000 pokerkit-0.0.0/pokerkit/tests/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)      724 2023-08-01 10:21:47.000000 pokerkit-0.0.0/pokerkit/tests/test_games.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     3783 2023-08-02 20:12:30.000000 pokerkit-0.0.0/pokerkit/tests/test_lookups.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    15333 2023-08-02 20:10:51.000000 pokerkit-0.0.0/pokerkit/tests/test_state.py
--rw-rw-r--   0 juho      (1000) juho      (1000)     1875 2023-08-01 05:16:21.000000 pokerkit-0.0.0/pokerkit/tests/test_utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2023-08-02 20:42:02.191630 pokerkit-0.0.0/pokerkit/tests/test_wsop/
--rw-rw-r--   0 juho      (1000) juho      (1000)        0 2023-07-21 19:50:32.000000 pokerkit-0.0.0/pokerkit/tests/test_wsop/__init__.py
--rw-rw-r--   0 juho      (1000) juho      (1000)   152392 2023-08-02 20:11:32.000000 pokerkit-0.0.0/pokerkit/tests/test_wsop/test_2023_43.py
--rw-rw-r--   0 juho      (1000) juho      (1000)    14002 2023-08-02 20:15:33.000000 pokerkit-0.0.0/pokerkit/utilities.py
-drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2023-08-02 20:42:02.191630 pokerkit-0.0.0/pokerkit.egg-info/
--rw-rw-r--   0 juho      (1000) juho      (1000)    11881 2023-08-02 20:42:02.000000 pokerkit-0.0.0/pokerkit.egg-info/PKG-INFO
--rw-rw-r--   0 juho      (1000) juho      (1000)      517 2023-08-02 20:42:02.000000 pokerkit-0.0.0/pokerkit.egg-info/SOURCES.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        1 2023-08-02 20:42:02.000000 pokerkit-0.0.0/pokerkit.egg-info/dependency_links.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)        9 2023-08-02 20:42:02.000000 pokerkit-0.0.0/pokerkit.egg-info/top_level.txt
--rw-rw-r--   0 juho      (1000) juho      (1000)       38 2023-08-02 20:42:02.191630 pokerkit-0.0.0/setup.cfg
--rw-rw-r--   0 juho      (1000) juho      (1000)     1731 2023-08-02 20:41:57.000000 pokerkit-0.0.0/setup.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2023-08-07 15:46:43.131739 pokerkit-0.0.1/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     1108 2023-07-21 19:50:32.000000 pokerkit-0.0.1/LICENSE
+-rw-rw-r--   0 juho      (1000) juho      (1000)    12046 2023-08-07 15:46:43.131739 pokerkit-0.0.1/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)    10504 2023-08-07 15:19:06.000000 pokerkit-0.0.1/README.rst
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2023-08-07 15:46:43.131739 pokerkit-0.0.1/pokerkit/
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2713 2023-08-07 14:44:13.000000 pokerkit-0.0.1/pokerkit/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    46834 2023-08-07 14:44:04.000000 pokerkit-0.0.1/pokerkit/games.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    19701 2023-08-07 15:31:16.000000 pokerkit-0.0.1/pokerkit/hands.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15396 2023-08-07 14:12:14.000000 pokerkit-0.0.1/pokerkit/lookups.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)        0 2023-08-02 20:39:04.000000 pokerkit-0.0.1/pokerkit/py.typed
+-rw-rw-r--   0 juho      (1000) juho      (1000)   117070 2023-08-07 15:27:19.000000 pokerkit-0.0.1/pokerkit/state.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2023-08-07 15:46:43.131739 pokerkit-0.0.1/pokerkit/tests/
+-rw-rw-r--   0 juho      (1000) juho      (1000)       88 2023-07-21 19:50:32.000000 pokerkit-0.0.1/pokerkit/tests/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     3783 2023-08-02 20:12:30.000000 pokerkit-0.0.1/pokerkit/tests/test_lookups.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    15333 2023-08-02 20:10:51.000000 pokerkit-0.0.1/pokerkit/tests/test_state.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)     1875 2023-08-01 05:16:21.000000 pokerkit-0.0.1/pokerkit/tests/test_utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2023-08-07 15:46:43.131739 pokerkit-0.0.1/pokerkit/tests/test_wsop/
+-rw-rw-r--   0 juho      (1000) juho      (1000)        0 2023-07-21 19:50:32.000000 pokerkit-0.0.1/pokerkit/tests/test_wsop/__init__.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)   152299 2023-08-07 15:30:27.000000 pokerkit-0.0.1/pokerkit/tests/test_wsop/test_2023_43.py
+-rw-rw-r--   0 juho      (1000) juho      (1000)    16117 2023-08-07 15:27:34.000000 pokerkit-0.0.1/pokerkit/utilities.py
+drwxrwxr-x   0 juho      (1000) juho      (1000)        0 2023-08-07 15:46:43.131739 pokerkit-0.0.1/pokerkit.egg-info/
+-rw-rw-r--   0 juho      (1000) juho      (1000)    12046 2023-08-07 15:46:43.000000 pokerkit-0.0.1/pokerkit.egg-info/PKG-INFO
+-rw-rw-r--   0 juho      (1000) juho      (1000)      488 2023-08-07 15:46:43.000000 pokerkit-0.0.1/pokerkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        1 2023-08-07 15:46:43.000000 pokerkit-0.0.1/pokerkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)        9 2023-08-07 15:46:43.000000 pokerkit-0.0.1/pokerkit.egg-info/top_level.txt
+-rw-rw-r--   0 juho      (1000) juho      (1000)       38 2023-08-07 15:46:43.131739 pokerkit-0.0.1/setup.cfg
+-rw-rw-r--   0 juho      (1000) juho      (1000)     2077 2023-08-07 13:03:23.000000 pokerkit-0.0.1/setup.py
```

### Comparing `pokerkit-0.0.0/LICENSE` & `pokerkit-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pokerkit-0.0.0/PKG-INFO` & `pokerkit-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pokerkit
-Version: 0.0.0
+Version: 0.0.1
 Summary: A Python package for various poker tools
 Home-page: https://github.com/uoftcprg/pokerkit
 Author: University of Toronto Computer Poker Research Group
 Author-email: uoftcprg@outlook.com
 License: MIT
 Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pokerkit
 Project-URL: Tracker, https://github.com/uoftcprg/pokerkit/issues
-Keywords: poker,nlhe,ai,game,game theory,libratus,modicum
+Keywords: artificial-intelligence,deep-learning,game,game-development,game-theory,holdem-poker,imperfect-information-game,libratus,pluribus,poker,poker-engine,poker-evaluator,poker-game,poker-hands,poker-library,poker-strategies,python,reinforcement-learning,texas-holdem
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Scientific/Engineering
@@ -29,37 +29,37 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
 PokerKit
 ========
 
-``PokerKit`` is an open-source Python library for simulating poker games and
+PokerKit is an open-source Python library for simulating poker games and
 evaluating poker hands, developed by the University of Toronto Computer Poker
 Research Group. It provides extensive support for all major and minor poker
 variants, offers a high level of control over game states, and supports
 high-speed hand evaluations.
 
 **Installation**
 ----------------
 
-The ``PokerKit`` library can be installed using pip:
+The PokerKit library can be installed using pip:
 
 .. code-block:: bash
 
    pip install pokerkit
 
 **Features**
 ------------
 
 * Extensive poker game logic for major and minor poker variants
 * High-speed hand evaluations
 * Customizable game states and parameters
-* Robust implementation with extensive unit tests and doctests
-* Ability to simulate famous hands from poker history
+* Robust implementation with static type checking and extensive unit tests and
+  doctests
 
 **Usage**
 ---------
 
 Below shows the first televised million dollar pot between Tom Dwan and Phil
 Ivey.
 
@@ -73,16 +73,16 @@
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
            Automation.BLIND_OR_STRADDLE_POSTING,
            Automation.CARD_BURNING,
            Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
            Automation.HAND_KILLING,
-           Automation.CHIP_PUSHING,
-           Automation.CHIP_PULLING,
+           Automation.CHIPS_PUSHING,
+           Automation.CHIPS_PULLING,
        ),
        True,
        500,
        (1000, 2000),
        2000,
        (1125600, 2000000, 553500),
        3,
@@ -257,16 +257,16 @@
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
            Automation.BLIND_OR_STRADDLE_POSTING,
            Automation.CARD_BURNING,
            Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
            Automation.HAND_KILLING,
-           Automation.CHIP_PUSHING,
-           Automation.CHIP_PULLING,
+           Automation.CHIPS_PUSHING,
+           Automation.CHIPS_PULLING,
        ),
        True,
        None,
        (75000, 150000),
        150000,
        300000,
        (1180000, 4340000, 5910000, 10765000),
@@ -398,36 +398,36 @@
    # Below show the final stacks.
 
    print(state.stacks)  # [196, 220, 200, 184]
 
 **Testing and Validation**
 --------------------------
 
-``PokerKit`` has extensive test coverage, passes mypy static type checking with
+PokerKit has extensive test coverage, passes mypy static type checking with
 strict parameter, and has been validated through extensive use in real-life
 scenarios.
 
 **Contributing**
 ----------------
 
 Contributions are welcome! Please read our
 `Contributing Guide <CONTRIBUTING.rst>`_ for more information.
 
 **License**
 -----------
 
-``PokerKit`` is distributed under the MIT license. See `LICENSE <LICENSE>`_ for
+PokerKit is distributed under the MIT license. See `LICENSE <LICENSE>`_ for
 more information.
 
 **Citing**
 ----------
 
-If you use ``PokerKit`` in your research, please cite our library:
+If you use PokerKit in your research, please cite our library:
 
 .. code-block:: bibtex
 
    @misc{pokerkit,
      title={PokerKit: An Open-Source Python Library for Poker Simulations and Hand Evaluations},
-     author={Your name here},
+     author={Juho Kim},
      year={2023},
      url={https://github.com/uoftcprg/pokerkit}
    }
```

### Comparing `pokerkit-0.0.0/README.rst` & `pokerkit-0.0.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 ========
 PokerKit
 ========
 
-``PokerKit`` is an open-source Python library for simulating poker games and
+PokerKit is an open-source Python library for simulating poker games and
 evaluating poker hands, developed by the University of Toronto Computer Poker
 Research Group. It provides extensive support for all major and minor poker
 variants, offers a high level of control over game states, and supports
 high-speed hand evaluations.
 
 **Installation**
 ----------------
 
-The ``PokerKit`` library can be installed using pip:
+The PokerKit library can be installed using pip:
 
 .. code-block:: bash
 
    pip install pokerkit
 
 **Features**
 ------------
 
 * Extensive poker game logic for major and minor poker variants
 * High-speed hand evaluations
 * Customizable game states and parameters
-* Robust implementation with extensive unit tests and doctests
-* Ability to simulate famous hands from poker history
+* Robust implementation with static type checking and extensive unit tests and
+  doctests
 
 **Usage**
 ---------
 
 Below shows the first televised million dollar pot between Tom Dwan and Phil
 Ivey.
 
@@ -42,16 +42,16 @@
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
            Automation.BLIND_OR_STRADDLE_POSTING,
            Automation.CARD_BURNING,
            Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
            Automation.HAND_KILLING,
-           Automation.CHIP_PUSHING,
-           Automation.CHIP_PULLING,
+           Automation.CHIPS_PUSHING,
+           Automation.CHIPS_PULLING,
        ),
        True,
        500,
        (1000, 2000),
        2000,
        (1125600, 2000000, 553500),
        3,
@@ -226,16 +226,16 @@
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
            Automation.BLIND_OR_STRADDLE_POSTING,
            Automation.CARD_BURNING,
            Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
            Automation.HAND_KILLING,
-           Automation.CHIP_PUSHING,
-           Automation.CHIP_PULLING,
+           Automation.CHIPS_PUSHING,
+           Automation.CHIPS_PULLING,
        ),
        True,
        None,
        (75000, 150000),
        150000,
        300000,
        (1180000, 4340000, 5910000, 10765000),
@@ -367,36 +367,36 @@
    # Below show the final stacks.
 
    print(state.stacks)  # [196, 220, 200, 184]
 
 **Testing and Validation**
 --------------------------
 
-``PokerKit`` has extensive test coverage, passes mypy static type checking with
+PokerKit has extensive test coverage, passes mypy static type checking with
 strict parameter, and has been validated through extensive use in real-life
 scenarios.
 
 **Contributing**
 ----------------
 
 Contributions are welcome! Please read our
 `Contributing Guide <CONTRIBUTING.rst>`_ for more information.
 
 **License**
 -----------
 
-``PokerKit`` is distributed under the MIT license. See `LICENSE <LICENSE>`_ for
+PokerKit is distributed under the MIT license. See `LICENSE <LICENSE>`_ for
 more information.
 
 **Citing**
 ----------
 
-If you use ``PokerKit`` in your research, please cite our library:
+If you use PokerKit in your research, please cite our library:
 
 .. code-block:: bibtex
 
    @misc{pokerkit,
      title={PokerKit: An Open-Source Python Library for Poker Simulations and Hand Evaluations},
-     author={Your name here},
+     author={Juho Kim},
      year={2023},
      url={https://github.com/uoftcprg/pokerkit}
    }
```

### Comparing `pokerkit-0.0.0/pokerkit/__init__.py` & `pokerkit-0.0.1/pokerkit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     'StandardHighHand',
     'StandardLookup',
     'StandardLowHand',
     'State',
     'Street',
     'Suit',
     'TexasHoldem',
+    'clean_values',
     'filter_none',
     'max_or_none',
     'min_or_none',
 )
 
 from pokerkit.games import (
     DeuceToSevenLowball,
@@ -116,11 +117,12 @@
 )
 from pokerkit.utilities import (
     Card,
     Deck,
     Rank,
     RankOrder,
     Suit,
+    clean_values,
     filter_none,
     max_or_none,
     min_or_none,
 )
```

### Comparing `pokerkit-0.0.0/pokerkit/games.py` & `pokerkit-0.0.1/pokerkit/games.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     OmahaHoldemHand,
     RegularLowHand,
     ShortDeckHoldemHand,
     StandardHighHand,
     StandardLowHand,
 )
 from pokerkit.state import BettingStructure, Opening, Automation, State, Street
-from pokerkit.utilities import Deck, RankOrder
+from pokerkit.utilities import Deck, RankOrder, clean_values
 
 
 class Poker(ABC):
     """The abstract base class for poker games."""
 
     max_down_card_count: int
     """The maximum number of down cards."""
@@ -29,41 +29,14 @@
     max_board_card_count: int
     """The maximum number of board cards."""
     rank_orders: tuple[RankOrder, ...]
     """The rank orders."""
     button_status: bool
     """The button status."""
 
-    @classmethod
-    def _clean_values(
-            cls,
-            values: int | Iterable[int] | Mapping[int, int] | None,
-            count: int,
-    ) -> tuple[int, ...]:
-        if values is None:
-            return (0,) * count
-        elif isinstance(values, Mapping):
-            parsed_values = [0] * count
-
-            for key, value in values.items():
-                parsed_values[key] = value
-
-            return tuple(parsed_values)
-        elif isinstance(values, Iterable):
-            parsed_values = list(values)
-
-            for i in range(len(parsed_values), count):
-                parsed_values.append(0)
-
-            return tuple(parsed_values)
-        elif isinstance(values, int):
-            return (values,) * count
-        else:
-            raise AssertionError
-
 
 class TexasHoldem(Poker, ABC):
     """The abstract base class for Texas hold'em games."""
 
     max_down_card_count = 2
     max_up_card_count = 0
     max_board_card_count = 5
@@ -108,18 +81,18 @@
         ...     4,
         ...     200,
         ...     2,
         ... )
 
         Below shows the pre-flop dealings and actions.
 
-        >>> state.deal_hole('AcAs')
-        State.HoleDealing(player_index=0, cards=(Ac, As), statuses=(False, False))
-        >>> state.deal_hole('7h6h')
-        State.HoleDealing(player_index=1, cards=(7h, 6h), statuses=(False, False))
+        >>> state.deal_hole('AcAs')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Ac, As), statuses=(False, F...
+        >>> state.deal_hole('7h6h')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(7h, 6h), statuses=(False, F...
 
         >>> state.complete_bet_or_raise_to()
         State.CompletionBettingOrRaisingTo(player_index=1, amount=4)
         >>> state.complete_bet_or_raise_to()
         State.CompletionBettingOrRaisingTo(player_index=0, amount=6)
         >>> state.fold()
         State.Folding(player_index=1)
@@ -177,18 +150,18 @@
                     big_bet,
                     4,
                 ),
             ),
             BettingStructure.FIXED_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(blinds_or_straddles, player_count),
+            clean_values(antes, player_count),
+            clean_values(blinds_or_straddles, player_count),
             0,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
 
 
 class NoLimitTexasHoldem(TexasHoldem):
     """The class for no-limit Texas hold'em games."""
 
     @classmethod
@@ -226,20 +199,20 @@
         ...     2000,
         ...     (1125600, 2000000, 553500),
         ...     3,
         ... )
 
         Below shows the pre-flop dealings and actions.
 
-        >>> state.deal_hole('Ac2d')  # Ivey
-        State.HoleDealing(player_index=0, cards=(Ac, 2d), statuses=(False, False))
-        >>> state.deal_hole('5h7s')  # Antonius*
-        State.HoleDealing(player_index=1, cards=(5h, 7s), statuses=(False, False))
-        >>> state.deal_hole('7h6h')  # Dwan
-        State.HoleDealing(player_index=2, cards=(7h, 6h), statuses=(False, False))
+        >>> state.deal_hole('Ac2d')  # Ivey  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Ac, 2d), statuses=(False, F...
+        >>> state.deal_hole('5h7s')  # Antonius*  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(5h, 7s), statuses=(False, F...
+        >>> state.deal_hole('7h6h')  # Dwan  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=2, cards=(7h, 6h), statuses=(False, F...
 
         >>> state.complete_bet_or_raise_to(7000)  # Dwan
         State.CompletionBettingOrRaisingTo(player_index=2, amount=7000)
         >>> state.complete_bet_or_raise_to(23000)  # Ivey
         State.CompletionBettingOrRaisingTo(player_index=0, amount=23000)
         >>> state.fold()  # Antonius
         State.Folding(player_index=1)
@@ -327,18 +300,18 @@
                     min_bet,
                     None,
                 ),
             ),
             BettingStructure.NO_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(blinds_or_straddles, player_count),
+            clean_values(antes, player_count),
+            clean_values(blinds_or_straddles, player_count),
             0,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
 
 
 class NoLimitShortDeckHoldem(TexasHoldem):
     """The class for no-limit short-deck hold'em games."""
 
     max_down_card_count = 2
@@ -381,26 +354,26 @@
         ...     3000,
         ...     (495000, 232000, 362000, 403000, 301000, 204000),
         ...     6,
         ... )
 
         Below shows the pre-flop dealings and actions.
 
-        >>> state.deal_hole('Th8h')  # Badziakouski
-        State.HoleDealing(player_index=0, cards=(Th, 8h), statuses=(False, False))
-        >>> state.deal_hole('QsJd')  # Zhong
-        State.HoleDealing(player_index=1, cards=(Qs, Jd), statuses=(False, False))
-        >>> state.deal_hole('QhQd')  # Xuan
-        State.HoleDealing(player_index=2, cards=(Qh, Qd), statuses=(False, False))
-        >>> state.deal_hole('8d7c')  # Jun
-        State.HoleDealing(player_index=3, cards=(8d, 7c), statuses=(False, False))
-        >>> state.deal_hole('KhKs')  # Phua
-        State.HoleDealing(player_index=4, cards=(Kh, Ks), statuses=(False, False))
-        >>> state.deal_hole('8c7h')  # Koon
-        State.HoleDealing(player_index=5, cards=(8c, 7h), statuses=(False, False))
+        >>> state.deal_hole('Th8h')  # Badziakouski  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Th, 8h), statuses=(False, F...
+        >>> state.deal_hole('QsJd')  # Zhong  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(Qs, Jd), statuses=(False, F...
+        >>> state.deal_hole('QhQd')  # Xuan  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=2, cards=(Qh, Qd), statuses=(False, F...
+        >>> state.deal_hole('8d7c')  # Jun  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=3, cards=(8d, 7c), statuses=(False, F...
+        >>> state.deal_hole('KhKs')  # Phua  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=4, cards=(Kh, Ks), statuses=(False, F...
+        >>> state.deal_hole('8c7h')  # Koon  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=5, cards=(8c, 7h), statuses=(False, F...
 
         >>> state.check_or_call()  # Badziakouski
         State.CheckingOrCalling(player_index=0, amount=3000)
         >>> state.check_or_call()  # Zhong
         State.CheckingOrCalling(player_index=1, amount=3000)
         >>> state.complete_bet_or_raise_to(35000)  # Xuan
         State.CompletionBettingOrRaisingTo(player_index=2, amount=35000)
@@ -484,18 +457,18 @@
                     min_bet,
                     None,
                 ),
             ),
             BettingStructure.NO_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(blinds_or_straddles, player_count),
+            clean_values(antes, player_count),
+            clean_values(blinds_or_straddles, player_count),
             0,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
 
 
 class OmahaHoldem(Poker, ABC):
     """The abstract base class for Omaha hold'em games."""
 
     max_down_card_count = 4
@@ -544,18 +517,18 @@
         ...     2000,
         ...     (125945025, 67847350),
         ...     2,
         ... )
 
         Below shows the pre-flop dealings and actions.
 
-        >>> state.deal_hole('Ah3sKsKh')  # Antonius
-        State.HoleDealing(player_index=0, cards=(Ah, 3s, Ks, Kh), statuses=(False, False, False, False))
-        >>> state.deal_hole('6d9s7d8h')  # Blom
-        State.HoleDealing(player_index=1, cards=(6d, 9s, 7d, 8h), statuses=(False, False, False, False))
+        >>> state.deal_hole('Ah3sKsKh')  # Antonius  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Ah, 3s, Ks, Kh), statuses=(...
+        >>> state.deal_hole('6d9s7d8h')  # Blom  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(6d, 9s, 7d, 8h), statuses=(...
 
         >>> state.complete_bet_or_raise_to(300000)  # Blom
         State.CompletionBettingOrRaisingTo(player_index=1, amount=300000)
         >>> state.complete_bet_or_raise_to(900000)  # Antonius
         State.CompletionBettingOrRaisingTo(player_index=0, amount=900000)
         >>> state.complete_bet_or_raise_to(2700000)  # Blom
         State.CompletionBettingOrRaisingTo(player_index=1, amount=2700000)
@@ -640,18 +613,18 @@
                     min_bet,
                     None,
                 ),
             ),
             BettingStructure.POT_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(blinds_or_straddles, player_count),
+            clean_values(antes, player_count),
+            clean_values(blinds_or_straddles, player_count),
             0,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
 
 
 class FixedLimitOmahaHoldemHighLowSplitEightOrBetter(OmahaHoldem):
     """The class for fixed-limit Omaha hold'em high/low-split eight or
     better low games.
     """
@@ -721,18 +694,18 @@
                     big_bet,
                     4,
                 ),
             ),
             BettingStructure.FIXED_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(blinds_or_straddles, player_count),
+            clean_values(antes, player_count),
+            clean_values(blinds_or_straddles, player_count),
             0,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
 
 
 class SevenCardStud(Poker, ABC):
     """The abstract base class for seven card stud games."""
 
     max_down_card_count = 3
@@ -816,18 +789,18 @@
                     big_bet,
                     4,
                 ),
             ),
             BettingStructure.FIXED_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(0, player_count),
+            clean_values(antes, player_count),
+            clean_values(0, player_count),
             bring_in,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
 
 
 class FixedLimitSevenCardStudHighLowSplitEightOrBetter(SevenCardStud):
     """The class for fixed-limit seven card stud high/low-split eight or
     better low games.
     """
@@ -906,18 +879,18 @@
                     big_bet,
                     4,
                 ),
             ),
             BettingStructure.FIXED_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(0, player_count),
+            clean_values(antes, player_count),
+            clean_values(0, player_count),
             bring_in,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
 
 
 class FixedLimitRazz(SevenCardStud):
     """The class for fixed-limit razz games."""
 
     rank_orders = (RankOrder.REGULAR,)
@@ -993,18 +966,18 @@
                     big_bet,
                     4,
                 ),
             ),
             BettingStructure.FIXED_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(0, player_count),
+            clean_values(antes, player_count),
+            clean_values(0, player_count),
             bring_in,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
 
 
 class DeuceToSevenLowball(Poker, ABC):
     """The abstract base class for deuce-to-seven lowball games."""
 
     max_down_card_count = 5
@@ -1060,18 +1033,18 @@
                     min_bet,
                     None,
                 ),
             ),
             BettingStructure.NO_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(blinds_or_straddles, player_count),
+            clean_values(antes, player_count),
+            clean_values(blinds_or_straddles, player_count),
             0,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
 
 
 class FixedLimitDeuceToSevenLowballTripleDraw(DeuceToSevenLowball):
     """The class for fixed-limit deuce-to-seven lowball triple draw
     games.
     """
@@ -1112,22 +1085,22 @@
         ...     300000,
         ...     (1180000, 4340000, 5910000, 10765000),
         ...     4,
         ... )
 
         Below shows the pre-flop dealings and actions.
 
-        >>> state.deal_hole('7h6c4c3d2c')  # Yockey
-        State.HoleDealing(player_index=0, cards=(7h, 6c, 4c, 3d, 2c), statuses=(False, False, False, False, False))
-        >>> state.deal_hole('JsJcJdJhTs')  # Hui*
-        State.HoleDealing(player_index=1, cards=(Js, Jc, Jd, Jh, Ts), statuses=(False, False, False, False, False))
-        >>> state.deal_hole('KsKcKdKhTh')  # Esposito*
-        State.HoleDealing(player_index=2, cards=(Ks, Kc, Kd, Kh, Th), statuses=(False, False, False, False, False))
-        >>> state.deal_hole('AsQs6s5c3c')  # Arieh
-        State.HoleDealing(player_index=3, cards=(As, Qs, 6s, 5c, 3c), statuses=(False, False, False, False, False))
+        >>> state.deal_hole('7h6c4c3d2c')  # Yockey  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(7h, 6c, 4c, 3d, 2c), status...
+        >>> state.deal_hole('JsJcJdJhTs')  # Hui*  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(Js, Jc, Jd, Jh, Ts), status...
+        >>> state.deal_hole('KsKcKdKhTh')  # Esposito*  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=2, cards=(Ks, Kc, Kd, Kh, Th), status...
+        >>> state.deal_hole('AsQs6s5c3c')  # Arieh  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=3, cards=(As, Qs, 6s, 5c, 3c), status...
 
         >>> state.fold()  # Esposito
         State.Folding(player_index=2)
         >>> state.complete_bet_or_raise_to()  # Arieh
         State.CompletionBettingOrRaisingTo(player_index=3, amount=300000)
         >>> state.complete_bet_or_raise_to()  # Yockey
         State.CompletionBettingOrRaisingTo(player_index=0, amount=450000)
@@ -1138,16 +1111,16 @@
 
         Below shows the first draw and actions.
 
         >>> state.stand_pat_or_discard()  # Yockey
         State.StandingPatOrDiscarding(player_index=0, cards=())
         >>> state.stand_pat_or_discard('AsQs')  # Arieh
         State.StandingPatOrDiscarding(player_index=3, cards=(As, Qs))
-        >>> state.deal_hole('2hQh')  # Arieh
-        State.HoleDealing(player_index=3, cards=(2h, Qh), statuses=(False, False))
+        >>> state.deal_hole('2hQh')  # Arieh  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=3, cards=(2h, Qh), statuses=(False, F...
 
         >>> state.complete_bet_or_raise_to()  # Yockey
         State.CompletionBettingOrRaisingTo(player_index=0, amount=150000)
         >>> state.check_or_call()  # Arieh
         State.CheckingOrCalling(player_index=3, amount=150000)
 
         Below shows the second draw and actions.
@@ -1231,18 +1204,18 @@
                     big_bet,
                     None,
                 ),
             ),
             BettingStructure.FIXED_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(blinds_or_straddles, player_count),
+            clean_values(antes, player_count),
+            clean_values(blinds_or_straddles, player_count),
             0,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
 
 
 class FixedLimitBadugi(Poker):
     """The class for fixed-limit badugi games."""
 
     max_down_card_count = 4
@@ -1287,22 +1260,22 @@
         ...     4,
         ...     200,
         ...     4,
         ... )
 
         Below shows the pre-flop dealings and actions.
 
-        >>> state.deal_hole('As4hJcKh')  # Bob*
-        State.HoleDealing(player_index=0, cards=(As, 4h, Jc, Kh), statuses=(False, False, False, False))
-        >>> state.deal_hole('3s5d7s8s')  # Carol*
-        State.HoleDealing(player_index=1, cards=(3s, 5d, 7s, 8s), statuses=(False, False, False, False))
-        >>> state.deal_hole('KsKdQsQd')  # Ted*
-        State.HoleDealing(player_index=2, cards=(Ks, Kd, Qs, Qd), statuses=(False, False, False, False))
-        >>> state.deal_hole('2s4c6dKc')  # Alice*
-        State.HoleDealing(player_index=3, cards=(2s, 4c, 6d, Kc), statuses=(False, False, False, False))
+        >>> state.deal_hole('As4hJcKh')  # Bob*  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(As, 4h, Jc, Kh), statuses=(...
+        >>> state.deal_hole('3s5d7s8s')  # Carol*  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(3s, 5d, 7s, 8s), statuses=(...
+        >>> state.deal_hole('KsKdQsQd')  # Ted*  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=2, cards=(Ks, Kd, Qs, Qd), statuses=(...
+        >>> state.deal_hole('2s4c6dKc')  # Alice*  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=3, cards=(2s, 4c, 6d, Kc), statuses=(...
 
         >>> state.fold()  # Ted
         State.Folding(player_index=2)
         >>> state.check_or_call()  # Alice
         State.CheckingOrCalling(player_index=3, amount=2)
         >>> state.check_or_call()  # Bob
         State.CheckingOrCalling(player_index=0, amount=1)
@@ -1313,18 +1286,18 @@
 
         >>> state.stand_pat_or_discard('JcKh')  # Bob*
         State.StandingPatOrDiscarding(player_index=0, cards=(Jc, Kh))
         >>> state.stand_pat_or_discard('7s8s')  # Carol*
         State.StandingPatOrDiscarding(player_index=1, cards=(7s, 8s))
         >>> state.stand_pat_or_discard('Kc')  # Alice*
         State.StandingPatOrDiscarding(player_index=3, cards=(Kc,))
-        >>> state.deal_hole('TcJs')  # Bob*
-        State.HoleDealing(player_index=0, cards=(Tc, Js), statuses=(False, False))
-        >>> state.deal_hole('7cTh')  # Carol*
-        State.HoleDealing(player_index=1, cards=(7c, Th), statuses=(False, False))
+        >>> state.deal_hole('TcJs')  # Bob*  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Tc, Js), statuses=(False, F...
+        >>> state.deal_hole('7cTh')  # Carol*  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(7c, Th), statuses=(False, F...
         >>> state.deal_hole('Qc')  # Alice*
         State.HoleDealing(player_index=3, cards=(Qc,), statuses=(False,))
 
         >>> state.check_or_call()  # Bob
         State.CheckingOrCalling(player_index=0, amount=0)
         >>> state.complete_bet_or_raise_to()  # Carol
         State.CompletionBettingOrRaisingTo(player_index=1, amount=2)
@@ -1426,12 +1399,12 @@
                     big_bet,
                     None,
                 ),
             ),
             BettingStructure.FIXED_LIMIT,
             automations,
             ante_trimming_status,
-            cls._clean_values(antes, player_count),
-            cls._clean_values(blinds_or_straddles, player_count),
+            clean_values(antes, player_count),
+            clean_values(blinds_or_straddles, player_count),
             0,
-            cls._clean_values(starting_stacks, player_count),
+            clean_values(starting_stacks, player_count),
         )
```

### Comparing `pokerkit-0.0.0/pokerkit/hands.py` & `pokerkit-0.0.1/pokerkit/hands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """:mod:`pokerkit.hands` implements classes related to poker hands."""
 
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from collections.abc import Hashable, Iterable, Iterator
+from collections.abc import Hashable, Iterable
 from functools import total_ordering
 from itertools import chain, combinations
 from typing import Any
 
 from pokerkit.lookups import (
     BadugiLookup,
     EightOrBetterLookup,
@@ -23,68 +23,70 @@
 
 @total_ordering
 class Hand(Hashable, ABC):
     """The abstract base class for poker hands.
 
     Stronger hands are considered greater than weaker hands.
 
-    >>> h0 = ShortDeckHoldemHand(Card.parse('6s7s8s9sTs'))
-    >>> h1 = ShortDeckHoldemHand(Card.parse('7c8c9cTcJc'))
-    >>> h2 = ShortDeckHoldemHand(Card.parse('2c2d2h2s3h'))
+    >>> h0 = ShortDeckHoldemHand('6s7s8s9sTs')
+    >>> h1 = ShortDeckHoldemHand('7c8c9cTcJc')
+    >>> h2 = ShortDeckHoldemHand('2c2d2h2s3h')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand '2c2d2h2s3h'
     >>> h0
     6s7s8s9sTs
     >>> h1
     7c8c9cTcJc
     >>> print(h0)
     Straight flush (6s7s8s9sTs)
     >>> h0 < h1
     True
 
     It does not make sense to compare hands of different types.
 
-    >>> h = BadugiHand(Card.parse('6d7s8h9c'))
+    >>> h = BadugiHand('6d7s8h9c')
     >>> h < 500
     Traceback (most recent call last):
         ...
     TypeError: '<' not supported between instances of 'BadugiHand' and 'int'
 
     The hands are hashable.
 
-    >>> h0 = ShortDeckHoldemHand(Card.parse('6s7s8s9sTs'))
-    >>> h1 = ShortDeckHoldemHand(Card.parse('7c8c9cTcJc'))
+    >>> h0 = ShortDeckHoldemHand('6s7s8s9sTs')
+    >>> h1 = ShortDeckHoldemHand('7c8c9cTcJc')
     >>> hands = {h0, h1}
     """
 
-    _lookup: Lookup
-    _low: bool
+    lookup: Lookup
+    """The hand lookup."""
+    low: bool
+    """The low status."""
 
     @classmethod
     @abstractmethod
     def from_game(
             cls,
-            hole_cards: Iterable[Card],
-            board_cards: Iterable[Card] = (),
+            hole_cards: Iterable[Card] | str | Card | None,
+            board_cards: Iterable[Card] | str | Card | None = (),
     ) -> Hand:
         """Create a poker hand from a game setting.
 
         In a game setting, a player uses private cards from their hole
         and the public cards from the board to make their hand.
 
         :param hole_cards: The hole cards.
         :param board_cards: The optional board cards.
         :return: The strongest hand from possible card combinations.
         """
 
-    def __init__(self, cards: Iterable[Card]) -> None:
-        self.__cards = tuple(cards)
+    def __init__(self, cards: Iterable[Card] | str | Card | None) -> None:
+        self.__cards = Card.clean(cards)
 
-        if not self._lookup.has_entry(self.cards):
+        if not self.lookup.has_entry(self.cards):
             raise ValueError(f'invalid hand \'{repr(self)}\'')
 
     def __eq__(self, other: Any) -> bool:
         if type(self) != type(other):
             return NotImplemented
 
         assert isinstance(other, Hand)
@@ -96,147 +98,121 @@
 
     def __lt__(self, other: Hand) -> bool:
         if type(self) != type(other):
             return NotImplemented
 
         assert isinstance(other, Hand)
 
-        if self._low:
+        if self.low:
             return self.entry > other.entry
         else:
             return self.entry < other.entry
 
     def __repr__(self) -> str:
         return ''.join(map(repr, self.cards))
 
     def __str__(self) -> str:
         return f'{self.entry.label.value} ({repr(self)})'
 
     @property
     def cards(self) -> tuple[Card, ...]:
         """Return the cards that form this hand.
 
-        >>> hole = Card.parse('AsAc')
-        >>> board = Card.parse('Kh3sAdAh')
+        >>> hole = 'AsAc'
+        >>> board = 'Kh3sAdAh'
         >>> hand = StandardHighHand.from_game(hole, board)
         >>> hand.cards
         (As, Ac, Kh, Ad, Ah)
 
         :return: The cards that form this hand.
         """
         return self.__cards
 
     @property
     def entry(self) -> Entry:
         """Return the hand entry.
 
-        >>> hole = Card.parse('AsAc')
-        >>> board = Card.parse('Kh3sAdAh')
+        >>> hole = 'AsAc'
+        >>> board = 'Kh3sAdAh'
         >>> hand = StandardHighHand.from_game(hole, board)
         >>> hand.entry.label
         <Label.FOUR_OF_A_KIND: 'Four of a kind'>
 
         :return: The hand entry.
         """
-        return self._lookup.get_entry(self.cards)
+        return self.lookup.get_entry(self.cards)
 
 
 class CombinationHand(Hand, ABC):
     """The abstract base class for combination hands."""
 
-    _card_count: int
+    card_count: int
+    """The number of cards."""
 
     @classmethod
     def from_game(
             cls,
-            hole_cards: Iterable[Card],
-            board_cards: Iterable[Card] = (),
+            hole_cards: Iterable[Card] | str | Card | None,
+            board_cards: Iterable[Card] | str | Card | None = (),
     ) -> Hand:
         """Create a poker hand from a game setting.
 
         In a game setting, a player uses private cards from their hole
         and the public cards from the board to make their hand.
 
-        >>> h0 = StandardHighHand.from_game(
-        ...     Card.parse('AcAdAhAsKc'),
-        ...     Card.parse(''),
-        ... )
-        >>> h1 = StandardHighHand(Card.parse('AcAdAhAsKc'))
+        >>> h0 = StandardHighHand.from_game('AcAdAhAsKc')
+        >>> h1 = StandardHighHand('AcAdAhAsKc')
         >>> h0 == h1
         True
-        >>> h0 = StandardHighHand.from_game(
-        ...     Card.parse('Ac9c'),
-        ...     Card.parse('AhKhQhJhTh'),
-        ... )
-        >>> h1 = StandardHighHand(Card.parse('AhKhQhJhTh'))
+        >>> h0 = StandardHighHand.from_game('Ac9c', 'AhKhQhJhTh')
+        >>> h1 = StandardHighHand('AhKhQhJhTh')
         >>> h0 == h1
         True
 
-        >>> h0 = StandardLowHand.from_game(
-        ...     Card.parse('AcAdAhAsKc'),
-        ...     Card.parse(''),
-        ... )
-        >>> h1 = StandardLowHand(Card.parse('AcAdAhAsKc'))
+        >>> h0 = StandardLowHand.from_game('AcAdAhAsKc', '')
+        >>> h1 = StandardLowHand('AcAdAhAsKc')
         >>> h0 == h1
         True
-        >>> h0 = StandardLowHand.from_game(
-        ...     Card.parse('Ac9c'),
-        ...     Card.parse('AhKhQhJhTh'),
-        ... )
-        >>> h1 = StandardLowHand(Card.parse('AcQhJhTh9c'))
+        >>> h0 = StandardLowHand.from_game('Ac9c', 'AhKhQhJhTh')
+        >>> h1 = StandardLowHand('AcQhJhTh9c')
         >>> h0 == h1
         True
 
-        >>> h0 = ShortDeckHoldemHand.from_game(
-        ...     Card.parse('AcKs'),
-        ...     Card.parse('AhAsKcJsTs'),
-        ... )
-        >>> h1 = ShortDeckHoldemHand(Card.parse('AcAhAsKcKs'))
+        >>> h0 = ShortDeckHoldemHand.from_game('AcKs', 'AhAsKcJsTs')
+        >>> h1 = ShortDeckHoldemHand('AcAhAsKcKs')
         >>> h0 == h1
         True
-        >>> h0 = ShortDeckHoldemHand.from_game(
-        ...     Card.parse('AcAd'),
-        ...     Card.parse('6s7cKcKd'),
-        ... )
-        >>> h1 = ShortDeckHoldemHand(Card.parse('AcAdKcKd7c'))
+        >>> h0 = ShortDeckHoldemHand.from_game('AcAd', '6s7cKcKd')
+        >>> h1 = ShortDeckHoldemHand('AcAdKcKd7c')
         >>> h0 == h1
         True
 
-        >>> h0 = EightOrBetterLowHand.from_game(
-        ...     Card.parse('As2s'),
-        ...     Card.parse('2c3c4c5c6c'),
-        ... )
-        >>> h1 = EightOrBetterLowHand(Card.parse('Ad2d3d4d5d'))
+        >>> h0 = EightOrBetterLowHand.from_game('As2s', '2c3c4c5c6c')
+        >>> h1 = EightOrBetterLowHand('Ad2d3d4d5d')
         >>> h0 == h1
         True
 
-        >>> h0 = RegularLowHand.from_game(
-        ...     Card.parse('AcAd'),
-        ...     Card.parse('AhAsKcQdQh'),
-        ... )
-        >>> h1 = RegularLowHand(Card.parse('AcAsQdQhKc'))
+        >>> h0 = RegularLowHand.from_game('AcAd', 'AhAsKcQdQh')
+        >>> h1 = RegularLowHand('AcAsQdQhKc')
         >>> h0 == h1
         True
-        >>> h0 = RegularLowHand.from_game(
-        ...     Card.parse('AcAd'),
-        ...     Card.parse('AhAsKcQd'),
-        ... )
-        >>> h1 = RegularLowHand(Card.parse('AdAhAsKcQd'))
+        >>> h0 = RegularLowHand.from_game('AcAd', 'AhAsKcQd')
+        >>> h1 = RegularLowHand('AdAhAsKcQd')
         >>> h0 == h1
         True
 
         :param hole_cards: The hole cards.
         :param board_cards: The optional board cards.
         :return: The strongest hand from possible card combinations.
         """
         max_hand = None
 
         for combination in combinations(
-                chain(hole_cards, board_cards),
-                cls._card_count,
+                chain(Card.clean(hole_cards), Card.clean(board_cards)),
+                cls.card_count,
         ):
             try:
                 hand = cls(combination)
             except ValueError:
                 pass
             else:
                 if max_hand is None or hand > max_hand:
@@ -247,217 +223,208 @@
 
         return max_hand
 
 
 class StandardHand(CombinationHand, ABC):
     """The abstract base class for standard hands."""
 
-    _lookup = StandardLookup()
-    _card_count = 5
+    lookup = StandardLookup()
+    card_count = 5
 
 
 class StandardHighHand(StandardHand):
     """The class for standard high hands.
 
-    >>> h0 = StandardHighHand(Card.parse('7c5d4h3s2c'))
-    >>> h1 = StandardHighHand(Card.parse('7c6d4h3s2c'))
-    >>> h2 = StandardHighHand(Card.parse('8c7d6h4s2c'))
-    >>> h3 = StandardHighHand(Card.parse('AcAsAd2s4s'))
-    >>> h4 = StandardHighHand(Card.parse('TsJsQsKsAs'))
+    >>> h0 = StandardHighHand('7c5d4h3s2c')
+    >>> h1 = StandardHighHand('7c6d4h3s2c')
+    >>> h2 = StandardHighHand('8c7d6h4s2c')
+    >>> h3 = StandardHighHand('AcAsAd2s4s')
+    >>> h4 = StandardHighHand('TsJsQsKsAs')
     >>> h0 < h1 < h2 < h3 < h4
     True
 
-    >>> h = StandardHighHand(Card.parse('4c5dThJsAcKh2h'))
+    >>> h = StandardHighHand('4c5dThJsAcKh2h')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand '4c5dThJsAcKh2h'
-    >>> h = StandardHighHand(Card.parse('Ac2c3c4c'))
+    >>> h = StandardHighHand('Ac2c3c4c')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand 'Ac2c3c4c'
     >>> h = StandardHighHand(())
     Traceback (most recent call last):
         ...
     ValueError: invalid hand ''
     """
 
-    _low = False
+    low = False
 
 
 class StandardLowHand(StandardHand):
     """The class for standard low hands.
 
-    >>> h0 = StandardLowHand(Card.parse('TsJsQsKsAs'))
-    >>> h1 = StandardLowHand(Card.parse('AcAsAd2s4s'))
-    >>> h2 = StandardLowHand(Card.parse('8c7d6h4s2c'))
-    >>> h3 = StandardLowHand(Card.parse('7c6d4h3s2c'))
-    >>> h4 = StandardLowHand(Card.parse('7c5d4h3s2c'))
+    >>> h0 = StandardLowHand('TsJsQsKsAs')
+    >>> h1 = StandardLowHand('AcAsAd2s4s')
+    >>> h2 = StandardLowHand('8c7d6h4s2c')
+    >>> h3 = StandardLowHand('7c6d4h3s2c')
+    >>> h4 = StandardLowHand('7c5d4h3s2c')
     >>> h0 < h1 < h2 < h3 < h4
     True
 
-    >>> h = StandardLowHand(Card.parse('4c5dThJsAcKh2h'))
+    >>> h = StandardLowHand('4c5dThJsAcKh2h')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand '4c5dThJsAcKh2h'
-    >>> h = StandardLowHand(Card.parse('Ac2c3c4c'))
+    >>> h = StandardLowHand('Ac2c3c4c')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand 'Ac2c3c4c'
     >>> h = StandardLowHand(())
     Traceback (most recent call last):
         ...
     ValueError: invalid hand ''
     """
 
-    _low = True
+    low = True
 
 
 class ShortDeckHoldemHand(CombinationHand):
     """The class for short-deck hold'em hands.
 
     Here, flushes beat full houses.
 
-    >>> h0 = ShortDeckHoldemHand(Card.parse('6c7d8h9sJc'))
-    >>> h1 = ShortDeckHoldemHand(Card.parse('7c7d7hTsQc'))
-    >>> h2 = ShortDeckHoldemHand(Card.parse('As6c7h8h9h'))
-    >>> h3 = ShortDeckHoldemHand(Card.parse('AsAhKcKhKd'))
-    >>> h4 = ShortDeckHoldemHand(Card.parse('6s7s8sTsQs'))
+    >>> h0 = ShortDeckHoldemHand('6c7d8h9sJc')
+    >>> h1 = ShortDeckHoldemHand('7c7d7hTsQc')
+    >>> h2 = ShortDeckHoldemHand('As6c7h8h9h')
+    >>> h3 = ShortDeckHoldemHand('AsAhKcKhKd')
+    >>> h4 = ShortDeckHoldemHand('6s7s8sTsQs')
     >>> h0 < h1 < h2 < h3 < h4
     True
 
-    >>> h = ShortDeckHoldemHand(Card.parse('4c5dThJsAcKh2h'))
+    >>> h = ShortDeckHoldemHand('4c5dThJsAcKh2h')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand '4c5dThJsAcKh2h'
-    >>> h = ShortDeckHoldemHand(Card.parse('Ac2c3c4c5c'))
+    >>> h = ShortDeckHoldemHand('Ac2c3c4c5c')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand 'Ac2c3c4c5c'
     >>> h = ShortDeckHoldemHand(())
     Traceback (most recent call last):
         ...
     ValueError: invalid hand ''
     """
 
-    _lookup = ShortDeckHoldemLookup()
-    _low = False
-    _card_count = 5
+    lookup = ShortDeckHoldemLookup()
+    low = False
+    card_count = 5
 
 
 class EightOrBetterLowHand(CombinationHand):
     """The class for eight or better low hands.
 
-    >>> h0 = EightOrBetterLowHand(Card.parse('8c7d6h4s2c'))
-    >>> h1 = EightOrBetterLowHand(Card.parse('7c5d4h3s2c'))
-    >>> h2 = EightOrBetterLowHand(Card.parse('5d4h3s2dAd'))
+    >>> h0 = EightOrBetterLowHand('8c7d6h4s2c')
+    >>> h1 = EightOrBetterLowHand('7c5d4h3s2c')
+    >>> h2 = EightOrBetterLowHand('5d4h3s2dAd')
     >>> h0 < h1 < h2
     True
 
-    >>> h = EightOrBetterLowHand(Card.parse('AcAsAd2s4s'))
+    >>> h = EightOrBetterLowHand('AcAsAd2s4s')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand 'AcAsAd2s4s'
-    >>> h = EightOrBetterLowHand(Card.parse('TsJsQsKsAs'))
+    >>> h = EightOrBetterLowHand('TsJsQsKsAs')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand 'TsJsQsKsAs'
-    >>> h = EightOrBetterLowHand(Card.parse('4c5dThJsAcKh2h'))
+    >>> h = EightOrBetterLowHand('4c5dThJsAcKh2h')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand '4c5dThJsAcKh2h'
-    >>> h = EightOrBetterLowHand(Card.parse('Ac2c3c4c'))
+    >>> h = EightOrBetterLowHand('Ac2c3c4c')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand 'Ac2c3c4c'
     >>> h = EightOrBetterLowHand(())
     Traceback (most recent call last):
         ...
     ValueError: invalid hand ''
     """
 
-    _lookup = EightOrBetterLookup()
-    _low = True
-    _card_count = 5
+    lookup = EightOrBetterLookup()
+    low = True
+    card_count = 5
 
 
 class RegularLowHand(CombinationHand):
     """The class for low regular hands.
 
     Here, flushes are ignored.
 
-    >>> h0 = RegularLowHand(Card.parse('KhKsKcKdAc'))
-    >>> h1 = RegularLowHand(Card.parse('2s2c3s3cAh'))
-    >>> h2 = RegularLowHand(Card.parse('6c4d3h2sAc'))
-    >>> h3 = RegularLowHand(Card.parse('Ac2c3c4c5c'))
+    >>> h0 = RegularLowHand('KhKsKcKdAc')
+    >>> h1 = RegularLowHand('2s2c3s3cAh')
+    >>> h2 = RegularLowHand('6c4d3h2sAc')
+    >>> h3 = RegularLowHand('Ac2c3c4c5c')
     >>> h0 < h1 < h2 < h3
     True
 
-    >>> h = RegularLowHand(Card.parse('4c5dThJsAcKh2h'))
+    >>> h = RegularLowHand('4c5dThJsAcKh2h')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand '4c5dThJsAcKh2h'
     >>> h = RegularLowHand(())
     Traceback (most recent call last):
         ...
     ValueError: invalid hand ''
     """
 
-    _lookup = RegularLowLookup()
-    _low = True
-    _card_count = 5
+    lookup = RegularLowLookup()
+    low = True
+    card_count = 5
 
 
 class BoardCombinationHand(CombinationHand, ABC):
     """The abstract base class for board-combination hands."""
 
-    _board_card_count: int
+    board_card_count: int
+    """The number of board cards."""
 
     @classmethod
     def from_game(
             cls,
-            hole_cards: Iterable[Card],
-            board_cards: Iterable[Card] = (),
+            hole_cards: Iterable[Card] | str | Card | None,
+            board_cards: Iterable[Card] | str | Card | None = (),
     ) -> Hand:
         """Create a poker hand from a game setting.
 
         In a game setting, a player uses private cards from their hole
         and the public cards from the board to make their hand.
 
-        >>> h0 = GreekHoldemHand.from_game(
-        ...     Card.parse('Ac2d'),
-        ...     Card.parse('QdJdTh2sKs'),
-        ... )
-        >>> h1 = GreekHoldemHand(Card.parse('2s2dAcKsQd'))
-        >>> h0 == h1
-        True
-        >>> h0 = GreekHoldemHand.from_game(
-        ...     Card.parse('AsKs'),
-        ...     Card.parse('QdJdTh2s2d'),
-        ... )
-        >>> h1 = GreekHoldemHand(Card.parse('AsKsQdJdTh'))
-        >>> h0 == h1
-        True
-        >>> h0 = GreekHoldemHand.from_game(
-        ...     Card.parse('Ac9c'),
-        ...     Card.parse('AhKhQhJhTh'),
-        ... )
-        >>> h1 = GreekHoldemHand(Card.parse('AcAhKhQh9c'))
+        >>> h0 = GreekHoldemHand.from_game('Ac2d', 'QdJdTh2sKs')
+        >>> h1 = GreekHoldemHand('2s2dAcKsQd')
+        >>> h0 == h1
+        True
+        >>> h0 = GreekHoldemHand.from_game('AsKs', 'QdJdTh2s2d')
+        >>> h1 = GreekHoldemHand('AsKsQdJdTh')
+        >>> h0 == h1
+        True
+        >>> h0 = GreekHoldemHand.from_game('Ac9c', 'AhKhQhJhTh')
+        >>> h1 = GreekHoldemHand('AcAhKhQh9c')
         >>> h0 == h1
         True
 
         :param hole_cards: The hole cards.
         :param board_cards: The optional board cards.
         :return: The strongest hand from possible card combinations.
         """
-        if isinstance(hole_cards, Iterator):
-            hole_cards = tuple(hole_cards)
-
+        hole_cards = Card.clean(hole_cards)
+        board_cards = Card.clean(board_cards)
         max_hand = None
 
-        for combination in combinations(board_cards, cls._board_card_count):
+        for combination in combinations(board_cards, cls.board_card_count):
             try:
                 hand = super().from_game(hole_cards, combination)
             except ValueError:
                 pass
             else:
                 if max_hand is None or hand > max_hand:
                     max_hand = hand
@@ -470,99 +437,81 @@
 
 class GreekHoldemHand(BoardCombinationHand):
     """The class for Greek hold'em hands.
 
     In Greek hold'em, the player must use all of his or her hole cards
     to make a hand.
 
-    >>> h0 = GreekHoldemHand(Card.parse('7c5d4h3s2c'))
-    >>> h1 = GreekHoldemHand(Card.parse('7c6d4h3s2c'))
-    >>> h2 = GreekHoldemHand(Card.parse('8c7d6h4s2c'))
-    >>> h3 = GreekHoldemHand(Card.parse('AcAsAd2s4s'))
-    >>> h4 = GreekHoldemHand(Card.parse('TsJsQsKsAs'))
+    >>> h0 = GreekHoldemHand('7c5d4h3s2c')
+    >>> h1 = GreekHoldemHand('7c6d4h3s2c')
+    >>> h2 = GreekHoldemHand('8c7d6h4s2c')
+    >>> h3 = GreekHoldemHand('AcAsAd2s4s')
+    >>> h4 = GreekHoldemHand('TsJsQsKsAs')
     >>> h0 < h1 < h2 < h3 < h4
     True
     """
 
-    _lookup = StandardLookup()
-    _low = False
-    _card_count = 5
-    _board_card_count = 3
+    lookup = StandardLookup()
+    low = False
+    card_count = 5
+    board_card_count = 3
 
 
 class HoleBoardCombinationHand(BoardCombinationHand, ABC):
     """The abstract base class for hole-board-combination hands."""
 
-    _hole_card_count: int
+    hole_card_count: int
+    """The number of hole cards."""
 
     @classmethod
     def from_game(
             cls,
-            hole_cards: Iterable[Card],
-            board_cards: Iterable[Card] = (),
+            hole_cards: Iterable[Card] | str | Card | None,
+            board_cards: Iterable[Card] | str | Card | None = (),
     ) -> Hand:
         """Create a poker hand from a game setting.
 
         In a game setting, a player uses private cards from their hole
         and the public cards from the board to make their hand.
 
-        >>> h0 = OmahaHoldemHand.from_game(
-        ...     Card.parse('6c7c8c9c'),
-        ...     Card.parse('8s9sTc'),
-        ... )
-        >>> h1 = OmahaHoldemHand(Card.parse('6c7c8s9sTc'))
+        >>> h0 = OmahaHoldemHand.from_game('6c7c8c9c', '8s9sTc')
+        >>> h1 = OmahaHoldemHand('6c7c8s9sTc')
         >>> h0 == h1
         True
-        >>> h0 = OmahaHoldemHand.from_game(
-        ...     Card.parse('6c7c8s9s'),
-        ...     Card.parse('8c9cTc'),
-        ... )
-        >>> h1 = OmahaHoldemHand(Card.parse('6c7c8c9cTc'))
+        >>> h0 = OmahaHoldemHand.from_game('6c7c8s9s', '8c9cTc')
+        >>> h1 = OmahaHoldemHand('6c7c8c9cTc')
         >>> h0 == h1
         True
-        >>> h0 = OmahaHoldemHand.from_game(
-        ...     Card.parse('6c7c8c9c'),
-        ...     Card.parse('8s9sTc9hKs'),
-        ... )
-        >>> h1 = OmahaHoldemHand(Card.parse('8c8s9c9s9h'))
+        >>> h0 = OmahaHoldemHand.from_game('6c7c8c9c', '8s9sTc9hKs')
+        >>> h1 = OmahaHoldemHand('8c8s9c9s9h')
         >>> h0 == h1
         True
-        >>> h0 = OmahaHoldemHand.from_game(
-        ...     Card.parse('6c7c8sAh'),
-        ...     Card.parse('As9cTc2sKs'),
-        ... )
-        >>> h1 = OmahaHoldemHand(Card.parse('AhAsKsTc8s'))
+        >>> h0 = OmahaHoldemHand.from_game('6c7c8sAh', 'As9cTc2sKs')
+        >>> h1 = OmahaHoldemHand('AhAsKsTc8s')
         >>> h0 == h1
         True
 
-        >>> h0 = OmahaEightOrBetterLowHand.from_game(
-        ...     Card.parse('As2s3s4s'),
-        ...     Card.parse('2c3c4c5c6c'),
-        ... )
-        >>> h1 = OmahaEightOrBetterLowHand(Card.parse('Ad2d3d4d5d'))
+        >>> h0 = OmahaEightOrBetterLowHand.from_game('As2s3s4s', '2c3c4c5c6c')
+        >>> h1 = OmahaEightOrBetterLowHand('Ad2d3d4d5d')
         >>> h0 == h1
         True
-        >>> h0 = OmahaEightOrBetterLowHand.from_game(
-        ...     Card.parse('As6s7s8s'),
-        ...     Card.parse('2c3c4c5c6c'),
-        ... )
-        >>> h1 = OmahaEightOrBetterLowHand(Card.parse('Ad2d3d4d6d'))
+        >>> h0 = OmahaEightOrBetterLowHand.from_game('As6s7s8s', '2c3c4c5c6c')
+        >>> h1 = OmahaEightOrBetterLowHand('Ad2d3d4d6d')
         >>> h0 == h1
         True
 
         :param hole_cards: The hole cards.
         :param board_cards: The optional board cards.
         :return: The strongest hand from possible card combinations.
         """
-        if isinstance(board_cards, Iterator):
-            board_cards = tuple(board_cards)
-
+        hole_cards = Card.clean(hole_cards)
+        board_cards = Card.clean(board_cards)
         max_hand = None
 
-        for combination in combinations(hole_cards, cls._hole_card_count):
+        for combination in combinations(hole_cards, cls.hole_card_count):
             try:
                 hand = super().from_game(combination, board_cards)
             except ValueError:
                 pass
             else:
                 if max_hand is None or hand > max_hand:
                     max_hand = hand
@@ -575,165 +524,167 @@
 
 class OmahaHoldemHand(HoleBoardCombinationHand):
     """The class for Omaha hold'em hands.
 
     In Omaha hold'em, the player must use a fixed number of his or her
     hole cards to make a hand.
 
-    >>> h0 = OmahaHoldemHand(Card.parse('7c5d4h3s2c'))
-    >>> h1 = OmahaHoldemHand(Card.parse('7c6d4h3s2c'))
-    >>> h2 = OmahaHoldemHand(Card.parse('8c7d6h4s2c'))
-    >>> h3 = OmahaHoldemHand(Card.parse('AcAsAd2s4s'))
-    >>> h4 = OmahaHoldemHand(Card.parse('TsJsQsKsAs'))
+    >>> h0 = OmahaHoldemHand('7c5d4h3s2c')
+    >>> h1 = OmahaHoldemHand('7c6d4h3s2c')
+    >>> h2 = OmahaHoldemHand('8c7d6h4s2c')
+    >>> h3 = OmahaHoldemHand('AcAsAd2s4s')
+    >>> h4 = OmahaHoldemHand('TsJsQsKsAs')
     >>> h0 < h1 < h2 < h3 < h4
     True
     """
 
-    _lookup = StandardLookup()
-    _low = False
-    _card_count = 5
-    _board_card_count = 3
-    _hole_card_count = 2
+    lookup = StandardLookup()
+    low = False
+    card_count = 5
+    board_card_count = 3
+    hole_card_count = 2
 
 
 class OmahaEightOrBetterLowHand(HoleBoardCombinationHand):
     """The class for Omaha eight or better low hands.
 
-    >>> h0 = OmahaEightOrBetterLowHand(Card.parse('8c7d6h4s2c'))
-    >>> h1 = OmahaEightOrBetterLowHand(Card.parse('7c5d4h3s2c'))
-    >>> h2 = OmahaEightOrBetterLowHand(Card.parse('5d4h3s2dAd'))
+    >>> h0 = OmahaEightOrBetterLowHand('8c7d6h4s2c')
+    >>> h1 = OmahaEightOrBetterLowHand('7c5d4h3s2c')
+    >>> h2 = OmahaEightOrBetterLowHand('5d4h3s2dAd')
     >>> h0 < h1 < h2
     True
     """
 
-    _lookup = EightOrBetterLookup()
-    _low = True
-    _card_count = 5
-    _board_card_count = 3
-    _hole_card_count = 2
+    lookup = EightOrBetterLookup()
+    low = True
+    card_count = 5
+    board_card_count = 3
+    hole_card_count = 2
 
 
 class BadugiHand(Hand):
     """The class for badugi hands.
 
-    >>> h0 = BadugiHand(Card.parse('Kc'))
-    >>> h1 = BadugiHand(Card.parse('Ac'))
-    >>> h2 = BadugiHand(Card.parse('4c8dKh'))
-    >>> h3 = BadugiHand(Card.parse('Ac2d3h5s'))
-    >>> h4 = BadugiHand(Card.parse('Ac2d3h4s'))
+    >>> h0 = BadugiHand('Kc')
+    >>> h1 = BadugiHand('Ac')
+    >>> h2 = BadugiHand('4c8dKh')
+    >>> h3 = BadugiHand('Ac2d3h5s')
+    >>> h4 = BadugiHand('Ac2d3h4s')
     >>> h0 < h1 < h2 < h3 < h4
     True
 
-    >>> h = BadugiHand(Card.parse('Ac2d3c4s5c'))
+    >>> h = BadugiHand('Ac2d3c4s5c')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand 'Ac2d3c4s5c'
-    >>> h = BadugiHand(Card.parse('Ac2d3c4s'))
+    >>> h = BadugiHand('Ac2d3c4s')
     Traceback (most recent call last):
         ...
     ValueError: cards not rainbow
-    >>> h = BadugiHand(Card.parse('AcAd3h4s'))
+    >>> h = BadugiHand('AcAd3h4s')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand 'AcAd3h4s'
-    >>> h = BadugiHand(Card.parse('Ac2c'))
+    >>> h = BadugiHand('Ac2c')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand 'Ac2c'
     >>> h = BadugiHand(())
     Traceback (most recent call last):
         ...
     ValueError: invalid hand ''
     """
 
-    _lookup = BadugiLookup()
-    _low = True
+    lookup = BadugiLookup()
+    low = True
 
     @classmethod
     def from_game(
             cls,
-            hole_cards: Iterable[Card],
-            board_cards: Iterable[Card] = (),
+            hole_cards: Iterable[Card] | str | Card | None,
+            board_cards: Iterable[Card] | str | Card | None = (),
     ) -> Hand:
         """Create a poker hand from a game setting.
 
         In a game setting, a player uses private cards from their hole
         and the public cards from the board to make their hand.
 
-        >>> h0 = BadugiHand.from_game(Card.parse('2s4c5d6h'))
-        >>> h1 = BadugiHand(Card.parse('2s4c5d6h'))
+        >>> h0 = BadugiHand.from_game('2s4c5d6h')
+        >>> h1 = BadugiHand('2s4c5d6h')
         >>> h0 == h1
         True
-        >>> h0 = BadugiHand.from_game(Card.parse('2s3s4d7h'))
-        >>> h1 = BadugiHand(Card.parse('2s4d7h'))
+        >>> h0 = BadugiHand.from_game('2s3s4d7h')
+        >>> h1 = BadugiHand('2s4d7h')
         >>> h0 == h1
         True
-        >>> h0 = BadugiHand.from_game(Card.parse('KcKdKhKs'))
-        >>> h1 = BadugiHand(Card.parse('Ks'))
+        >>> h0 = BadugiHand.from_game('KcKdKhKs')
+        >>> h1 = BadugiHand('Ks')
         >>> h0 == h1
         True
 
         :param hole_cards: The hole cards.
         :param board_cards: The optional board cards.
         :return: The strongest hand from possible card combinations.
         """
         ranks = set()
         suits = set()
         cards = set()
 
         for card in sorted(
-                chain(hole_cards, board_cards),
+                chain(Card.clean(hole_cards), Card.clean(board_cards)),
                 key=lambda card: RankOrder.STANDARD.index(card.rank),
         ):
             if card.rank not in ranks and card.suit not in suits:
                 ranks.add(card.rank)
                 suits.add(card.suit)
                 cards.add(card)
 
         return cls(cards)
 
-    def __init__(self, cards: Iterable[Card]) -> None:
+    def __init__(self, cards: Iterable[Card] | str | Card | None) -> None:
         super().__init__(cards)
 
         if not Card.are_rainbow(self.cards):
             raise ValueError('cards not rainbow')
 
 
 class KuhnPokerHand(Hand):
     """The class for Kuhn poker hands.
 
-    >>> h0 = KuhnPokerHand(Card.parse('Js'))
-    >>> h1 = KuhnPokerHand(Card.parse('Qs'))
-    >>> h2 = KuhnPokerHand(Card.parse('Ks'))
+    >>> h0 = KuhnPokerHand('Js')
+    >>> h1 = KuhnPokerHand('Qs')
+    >>> h2 = KuhnPokerHand('Ks')
     >>> h0 < h1 < h2
     True
 
-    >>> h = KuhnPokerHand(Card.parse('As'))
+    >>> h = KuhnPokerHand('As')
     Traceback (most recent call last):
         ...
     ValueError: invalid hand 'As'
     """
 
-    _lookup = KuhnPokerLookup()
-    _low = False
+    lookup = KuhnPokerLookup()
+    low = False
 
     @classmethod
     def from_game(
             cls,
-            hole_cards: Iterable[Card],
-            board_cards: Iterable[Card] = (),
+            hole_cards: Iterable[Card] | str | Card | None,
+            board_cards: Iterable[Card] | str | Card | None = (),
     ) -> Hand:
         """Create a poker hand from a game setting.
 
         In a game setting, a player uses private cards from their hole
         and the public cards from the board to make their hand.
 
-        >>> h0 = BadugiHand.from_game(Card.parse('Ks'))
-        >>> h1 = BadugiHand(Card.parse('Ks'))
+        >>> h0 = BadugiHand.from_game('Ks')
+        >>> h1 = BadugiHand('Ks')
         >>> h0 == h1
         True
 
         :param hole_cards: The hole cards.
         :param board_cards: The optional board cards.
         :return: The strongest hand from possible card combinations.
         """
-        return max(map(cls, chain(hole_cards, board_cards)))
+        return max(
+            map(cls, chain(Card.clean(hole_cards), Card.clean(board_cards))),
+        )
```

### Comparing `pokerkit-0.0.0/pokerkit/lookups.py` & `pokerkit-0.0.1/pokerkit/lookups.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """:mod:`pokerkit.lookups` implements classes related to poker hand
 lookups.
 """
 
 from abc import ABC
 from collections import Counter
-from collections.abc import Iterable, Iterator, Reversible, Sequence
+from collections.abc import Iterable, Reversible, Sequence
 from dataclasses import dataclass, field
 from enum import StrEnum, unique
 from functools import partial
 from itertools import combinations, filterfalse
 from math import prod
 from operator import contains
 
@@ -87,16 +87,16 @@
 class Lookup(ABC):
     """The abstract base class for hand lookups.
 
     Lookups are used internally by hands. If you want to evaluate poker
     hands, please use one of the hand classes.
 
     >>> lookup = StandardLookup()
-    >>> e0 = lookup.get_entry(Card.parse('As3sQhJsJc'))
-    >>> e1 = lookup.get_entry(Card.parse('2s4sKhKsKc'))
+    >>> e0 = lookup.get_entry('As3sQhJsJc')
+    >>> e1 = lookup.get_entry('2s4sKhKsKc')
     >>> e0 < e1
     True
     >>> e0.label
     <Label.ONE_PAIR: 'One pair'>
     >>> e1.label
     <Label.THREE_OF_A_KIND: 'Three of a kind'>
     """
@@ -138,43 +138,43 @@
             ):
                 hashes.append(hash_ * partial_hash)
 
         counter[multiplicity] = count
 
         return hashes
 
-    def has_entry(self, cards: Iterable[Card]) -> bool:
+    def has_entry(self, cards: Iterable[Card] | str | Card | None) -> bool:
         """Return whether the cards can be looked up.
 
         The cards can be looked up if the lookup contains an entry with
         the given cards.
 
         >>> lookup = ShortDeckHoldemLookup()
-        >>> lookup.has_entry(Card.parse('Ah6h7s8c9s'))
+        >>> lookup.has_entry('Ah6h7s8c9s')
         True
-        >>> lookup.has_entry(Card.parse('Ah6h7s8c2s'))
+        >>> lookup.has_entry('Ah6h7s8c2s')
         False
 
         :param cards: The cards to look up.
         :return: ``True`` if the cards can looked up, otherwise
                  ``False``.
         """
         return self.__get_key(cards) in self.__entries
 
-    def get_entry(self, cards: Iterable[Card]) -> Entry:
+    def get_entry(self, cards: Iterable[Card] | str | Card | None) -> Entry:
         """Return the corresponding lookup entry of the hand that the
         cards form.
 
         >>> lookup = ShortDeckHoldemLookup()
-        >>> entry = lookup.get_entry(Card.parse('Ah6h7s8c9s'))
+        >>> entry = lookup.get_entry('Ah6h7s8c9s')
         >>> entry.index
         1134
         >>> entry.label
         <Label.STRAIGHT: 'Straight'>
-        >>> entry = lookup.get_entry(Card.parse('Ah6h7s8c2s'))
+        >>> entry = lookup.get_entry('Ah6h7s8c2s')
         Traceback (most recent call last):
             ...
         ValueError: cards form an invalid hand
 
         :param cards: The cards to look up.
         :return: The corresponding lookup entry.
         :raises ValueError: If cards do not form a valid hand.
@@ -182,35 +182,39 @@
         key = self.__get_key(cards)
 
         if key not in self.__entries:
             raise ValueError('cards form an invalid hand')
 
         return self.__entries[key]
 
-    def get_entry_or_none(self, cards: Iterable[Card]) -> Entry | None:
+    def get_entry_or_none(
+            self,
+            cards: Iterable[Card] | str | Card | None,
+    ) -> Entry | None:
         """Return the corresponding lookup entry of the hand that the
         cards form if it exists. Otherwise, return ``None``.
 
         >>> lookup = ShortDeckHoldemLookup()
-        >>> lookup.get_entry(Card.parse('Ah6h7s8c2s'))
+        >>> lookup.get_entry('Ah6h7s8c2s')
         Traceback (most recent call last):
             ...
         ValueError: cards form an invalid hand
-        >>> lookup.get_entry_or_none(Card.parse('Ah6h7s8c2s')) is None
+        >>> lookup.get_entry_or_none('Ah6h7s8c2s') is None
         True
 
         :param cards: The cards to look up.
         :return: The optional corresponding lookup entry.
         """
         return self.__entries.get(self.__get_key(cards))
 
-    def __get_key(self, cards: Iterable[Card]) -> tuple[int, bool]:
-        if isinstance(cards, Iterator):
-            cards = tuple(cards)
-
+    def __get_key(
+            self,
+            cards: Iterable[Card] | str | Card | None,
+    ) -> tuple[int, bool]:
+        cards = Card.clean(cards)
         hash_ = self.__hash(Card.get_ranks(cards))
         suitedness = Card.are_suited(cards)
 
         return hash_, suitedness
 
     def _add_multisets(
             self,
@@ -262,17 +266,17 @@
     """The class for standard hand lookups.
 
     Lookups are used by evaluators. If you want to evaluate poker hands,
     please subclasses of :class:`pokerkit.hands.Hand` that use this
     lookup.
 
     >>> lookup = StandardLookup()
-    >>> e0 = lookup.get_entry(Card.parse('Ah6h7s8c9s'))
-    >>> e1 = lookup.get_entry(Card.parse('AhAc6s6hTd'))
-    >>> e2 = lookup.get_entry(Card.parse('AcAdAhAsAc'))
+    >>> e0 = lookup.get_entry('Ah6h7s8c9s')
+    >>> e1 = lookup.get_entry('AhAc6s6hTd')
+    >>> e2 = lookup.get_entry('AcAdAhAsAc')
     Traceback (most recent call last):
         ...
     ValueError: cards form an invalid hand
     >>> e0 < e1
     True
     >>> e0.label
     <Label.HIGH_CARD: 'High card'>
@@ -338,17 +342,17 @@
 
     Here, flushes beat full houses.
 
     Lookups are used by evaluators. If you want to evaluate poker hands,
     please use :class:`pokerkit.hands.ShortDeckHoldemHand`.
 
     >>> lookup = ShortDeckHoldemLookup()
-    >>> e0 = lookup.get_entry(Card.parse('AhAc6s6hTd'))
-    >>> e1 = lookup.get_entry(Card.parse('Ah6h7s8c9s'))
-    >>> e2 = lookup.get_entry(Card.parse('Ah2h3s4c5s'))
+    >>> e0 = lookup.get_entry('AhAc6s6hTd')
+    >>> e1 = lookup.get_entry('Ah6h7s8c9s')
+    >>> e2 = lookup.get_entry('Ah2h3s4c5s')
     Traceback (most recent call last):
         ...
     ValueError: cards form an invalid hand
     >>> e0 < e1
     True
     >>> e0.label
     <Label.TWO_PAIR: 'Two pair'>
@@ -436,17 +440,17 @@
 
     Here, flushes are ignored.
 
     Lookups are used by evaluators. If you want to evaluate poker hands,
     please use :class:`pokerkit.hands.RegularLowHand`.
 
     >>> lookup = RegularLowLookup()
-    >>> e0 = lookup.get_entry(Card.parse('Ah6h7s8c9s'))
-    >>> e1 = lookup.get_entry(Card.parse('AhAc6s6hTd'))
-    >>> e2 = lookup.get_entry(Card.parse('3s4sQhTc'))
+    >>> e0 = lookup.get_entry('Ah6h7s8c9s')
+    >>> e1 = lookup.get_entry('AhAc6s6hTd')
+    >>> e2 = lookup.get_entry('3s4sQhTc')
     Traceback (most recent call last):
         ...
     ValueError: cards form an invalid hand
     >>> e0 < e1
     True
     >>> e0.label
     <Label.HIGH_CARD: 'High card'>
@@ -497,17 +501,17 @@
 class BadugiLookup(Lookup):
     """The class for badugi hand lookups.
 
     Lookups are used by evaluators. If you want to evaluate poker hands,
     please use :class:`pokerkit.hands.BadugiHand`.
 
     >>> lookup = BadugiLookup()
-    >>> e0 = lookup.get_entry(Card.parse('2s'))
-    >>> e1 = lookup.get_entry(Card.parse('KhQc'))
-    >>> e2 = lookup.get_entry(Card.parse('AcAdAhAs'))
+    >>> e0 = lookup.get_entry('2s')
+    >>> e1 = lookup.get_entry('KhQc')
+    >>> e2 = lookup.get_entry('AcAdAhAs')
     Traceback (most recent call last):
         ...
     ValueError: cards form an invalid hand
     >>> e0 > e1
     True
     >>> e0.label
     <Label.HIGH_CARD: 'High card'>
@@ -529,17 +533,17 @@
 class KuhnPokerLookup(Lookup):
     """The class for Kuhn poker hand lookups.
 
     Lookups are used by evaluators. If you want to evaluate poker hands,
     please use :class:`pokerkit.hands.KuhnPokerHand`.
 
     >>> lookup = KuhnPokerLookup()
-    >>> e0 = lookup.get_entry(Card.parse('Js'))
-    >>> e1 = lookup.get_entry(Card.parse('Qs'))
-    >>> e2 = lookup.get_entry(Card.parse('2c'))
+    >>> e0 = lookup.get_entry('Js')
+    >>> e1 = lookup.get_entry('Qs')
+    >>> e2 = lookup.get_entry('2c')
     Traceback (most recent call last):
         ...
     ValueError: cards form an invalid hand
     >>> e0 < e1
     True
     >>> e0.label
     <Label.HIGH_CARD: 'High card'>
```

### Comparing `pokerkit-0.0.0/pokerkit/state.py` & `pokerkit-0.0.1/pokerkit/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -807,23 +807,25 @@
         ...     (1, 2),
         ...     2,
         ...     200,
         ...     2,
         ... )
         >>> state.hand_type_count
         1
-        >>> state = FixedLimitOmahaHoldemHighLowSplitEightOrBetter.create_state(
-        ...     (),
-        ...     True,
-        ...     1,
-        ...     (1, 2),
-        ...     2,
-        ...     4,
-        ...     100,
-        ...     3,
+        >>> state = (
+        ...     FixedLimitOmahaHoldemHighLowSplitEightOrBetter.create_state(
+        ...         (),
+        ...         True,
+        ...         1,
+        ...         (1, 2),
+        ...         2,
+        ...         4,
+        ...         100,
+        ...         3,
+        ...     )
         ... )
         >>> state.hand_type_count
         2
 
         :return: The number of hand types.
         """
         return len(self.hand_types)
@@ -843,23 +845,25 @@
         ...     (1, 2),
         ...     2,
         ...     200,
         ...     2,
         ... )
         >>> state.hand_type_indices
         range(0, 1)
-        >>> state = FixedLimitOmahaHoldemHighLowSplitEightOrBetter.create_state(
-        ...     (),
-        ...     True,
-        ...     1,
-        ...     (1, 2),
-        ...     2,
-        ...     4,
-        ...     100,
-        ...     3,
+        >>> state = (
+        ...     FixedLimitOmahaHoldemHighLowSplitEightOrBetter.create_state(
+        ...         (),
+        ...         True,
+        ...         1,
+        ...         (1, 2),
+        ...         2,
+        ...         4,
+        ...         100,
+        ...         3,
+        ...     )
         ... )
         >>> state.hand_type_indices
         range(0, 2)
 
         :return: The hand type indices.
         """
         return range(self.hand_type_count)
@@ -1387,18 +1391,18 @@
         ...     None,
         ...     1,
         ...     2,
         ...     4,
         ...     (50, 100),
         ...     2,
         ... )
-        >>> state.deal_hole('AcAdAh')
-        State.HoleDealing(player_index=0, cards=(Ac, Ad, Ah), statuses=(False, False, True))
-        >>> state.deal_hole('KcKdKh')
-        State.HoleDealing(player_index=1, cards=(Kc, Kd, Kh), statuses=(False, False, True))
+        >>> state.deal_hole('AcAdAh')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Ac, Ad, Ah), statuses=(Fals...
+        >>> state.deal_hole('KcKdKh')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(Kc, Kd, Kh), statuses=(Fals...
         >>> state.get_down_cards(0)  # doctest: +ELLIPSIS
         <generator object State.get_down_cards at 0x...>
         >>> tuple(state.get_down_cards(0))
         (Ac, Ad)
         >>> tuple(state.get_down_cards(1))
         (Kc, Kd)
         >>> state.post_bring_in()
@@ -1439,18 +1443,18 @@
         ...     None,
         ...     1,
         ...     2,
         ...     4,
         ...     (50, 100),
         ...     2,
         ... )
-        >>> state.deal_hole('AcAdAh')
-        State.HoleDealing(player_index=0, cards=(Ac, Ad, Ah), statuses=(False, False, True))
-        >>> state.deal_hole('KcKdKh')
-        State.HoleDealing(player_index=1, cards=(Kc, Kd, Kh), statuses=(False, False, True))
+        >>> state.deal_hole('AcAdAh')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Ac, Ad, Ah), statuses=(Fals...
+        >>> state.deal_hole('KcKdKh')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(Kc, Kd, Kh), statuses=(Fals...
         >>> state.get_down_cards(0)  # doctest: +ELLIPSIS
         <generator object State.get_down_cards at 0x...>
         >>> tuple(state.get_up_cards(0))
         (Ah,)
         >>> tuple(state.get_up_cards(1))
         (Kh,)
         >>> state.post_bring_in()
@@ -1494,18 +1498,18 @@
         ...     (50, 100),
         ...     2,
         ... )
         >>> state.get_hand(0, 0) is None
         True
         >>> state.get_hand(1, 0) is None
         True
-        >>> state.deal_hole('AcAd')
-        State.HoleDealing(player_index=0, cards=(Ac, Ad), statuses=(False, False))
-        >>> state.deal_hole('KsQs')
-        State.HoleDealing(player_index=1, cards=(Ks, Qs), statuses=(False, False))
+        >>> state.deal_hole('AcAd')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Ac, Ad), statuses=(False, F...
+        >>> state.deal_hole('KsQs')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(Ks, Qs), statuses=(False, F...
         >>> state.get_hand(0, 0) is None
         True
         >>> state.get_hand(1, 0) is None
         True
         >>> state.check_or_call()
         State.CheckingOrCalling(player_index=1, amount=1)
         >>> state.check_or_call()
@@ -1591,18 +1595,18 @@
         ...     (50, 100),
         ...     2,
         ... )
         >>> state.get_up_hand(0, 0) is None
         True
         >>> state.get_up_hand(1, 0) is None
         True
-        >>> state.deal_hole('AcAd')
-        State.HoleDealing(player_index=0, cards=(Ac, Ad), statuses=(False, False))
-        >>> state.deal_hole('KsQs')
-        State.HoleDealing(player_index=1, cards=(Ks, Qs), statuses=(False, False))
+        >>> state.deal_hole('AcAd')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Ac, Ad), statuses=(False, F...
+        >>> state.deal_hole('KsQs')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(Ks, Qs), statuses=(False, F...
         >>> state.get_up_hand(0, 0) is None
         True
         >>> state.get_up_hand(1, 0) is None
         True
         >>> state.check_or_call()
         State.CheckingOrCalling(player_index=1, amount=1)
         >>> state.check_or_call()
@@ -1681,18 +1685,18 @@
         ...     (50, 100),
         ...     2,
         ... )
         >>> state.get_up_hands(0)  # doctest: +ELLIPSIS
         <generator object State.get_up_hands at 0x...>
         >>> tuple(state.get_up_hands(0))
         (None, None)
-        >>> state.deal_hole('AcAd')
-        State.HoleDealing(player_index=0, cards=(Ac, Ad), statuses=(False, False))
-        >>> state.deal_hole('KsQs')
-        State.HoleDealing(player_index=1, cards=(Ks, Qs), statuses=(False, False))
+        >>> state.deal_hole('AcAd')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Ac, Ad), statuses=(False, F...
+        >>> state.deal_hole('KsQs')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(Ks, Qs), statuses=(False, F...
         >>> state.check_or_call()
         State.CheckingOrCalling(player_index=1, amount=1)
         >>> state.check_or_call()
         State.CheckingOrCalling(player_index=0, amount=0)
         >>> state.deal_board('JsTs2c')
         State.BoardDealing(cards=(Js, Ts, 2c))
         >>> state.check_or_call()
@@ -1742,18 +1746,18 @@
         ...     True,
         ...     None,
         ...     (1, 2),
         ...     2,
         ...     (50, 100),
         ...     2,
         ... )
-        >>> state.deal_hole('KhQh')
-        State.HoleDealing(player_index=0, cards=(Kh, Qh), statuses=(False, False))
-        >>> state.deal_hole('AcKc')
-        State.HoleDealing(player_index=1, cards=(Ac, Kc), statuses=(False, False))
+        >>> state.deal_hole('KhQh')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=0, cards=(Kh, Qh), statuses=(False, F...
+        >>> state.deal_hole('AcKc')  # doctest: +ELLIPSIS
+        State.HoleDealing(player_index=1, cards=(Ac, Kc), statuses=(False, F...
         >>> state.check_or_call()
         State.CheckingOrCalling(player_index=1, amount=1)
         >>> state.check_or_call()
         State.CheckingOrCalling(player_index=0, amount=0)
         >>> state.deal_board('JsTs2c')
         State.BoardDealing(cards=(Js, Ts, 2c))
         >>> state.check_or_call()
@@ -2271,49 +2275,15 @@
         assert not self.card_burning_status
         assert not any(self.hole_dealing_statuses)
         assert not self.board_dealing_count
         assert not any(self.standing_pat_or_discarding_statuses)
 
         self._begin_betting()
 
-    def _clean_cards(
-            self,
-            cards: Iterable[Card] | str | Card | int | None,
-    ) -> tuple[Card, ...]:
-        if cards is None:
-            card_count = 0
-        elif isinstance(cards, int):
-            card_count = cards
-        elif isinstance(cards, Card):
-            card_count = 1
-        elif isinstance(cards, str):
-            cards = tuple(Card.parse(cards))
-            card_count = len(cards)
-        elif isinstance(cards, tuple):
-            card_count = len(cards)
-        else:
-            cards = tuple(cards)
-            card_count = len(cards)
-
-        if isinstance(cards, int):
-            if len(self.deck_cards) < card_count:
-                raise ValueError('too many cards')
-
-            cards = tuple(self.deck_cards)[:cards]
-        elif isinstance(cards, Card):
-            cards = (cards,)
-        elif cards is None:
-            cards = ()
-
-        if len(set(cards)) != len(cards):
-            raise ValueError('duplicate cards')
-
-        return cards
-
-    def _make_available(self, cards: tuple[Card, ...]) -> None:
+    def _make_card_available(self, cards: tuple[Card, ...]) -> None:
         assert len(self.deck_cards) >= len(cards)
 
         for card in cards:
             assert card in self.burned_cards or card in self.deck_cards
 
             if card in self.burned_cards:
                 self.burned_cards[self.burned_cards.index(card)] = (
@@ -2330,31 +2300,34 @@
         :return: The available cards.
         """
         if (
                 self.card_burning_status
                 or any(self.hole_dealing_statuses)
                 or self.board_dealing_count
         ):
-            yield from chain(self.burned_cards, self.deck_cards)
+            yield from chain(self.deck_cards, self.burned_cards)
 
     def verify_card_availabilities(
             self,
             cards: Iterable[Card] | str | Card | int | None,
     ) -> tuple[Card, ...]:
         """Verify the card availability.
 
         :param cards: The optional cards.
         :return: The available cards.
         :raises ValueError: If the card is unavailable.
         """
-        cards = self._clean_cards(cards)
+        if isinstance(cards, int):
+            cards = tuple(islice(self.available_cards, cards))
+        else:
+            cards = Card.clean(cards)
 
-        for card in cards:
-            if card not in tuple(self.available_cards):
-                raise ValueError('unavailable card')
+            for card in cards:
+                if card not in tuple(self.available_cards):
+                    raise ValueError('unavailable card')
 
         return cards
 
     @dataclass
     class CardBurning:
         """The card burning."""
 
@@ -2410,15 +2383,15 @@
         assert self.street is not None
         assert (
             any(self.hole_dealing_statuses)
             or self.board_dealing_count
             or self.street.draw_status
         )
 
-        self._make_available((card,))
+        self._make_card_available((card,))
 
         self.card_burning_status = False
         self.burned_cards.append(card)
 
         if (
                 not any(self.hole_dealing_statuses)
                 and not self.board_dealing_count
@@ -2525,15 +2498,15 @@
         cards = self.verify_hole_dealing(cards)
         player_index = self.hole_dealee_index
         statuses = []
 
         assert player_index is not None
         assert self.hole_dealing_statuses[player_index]
 
-        self._make_available(cards)
+        self._make_card_available(cards)
 
         for card in cards:
             status = self.hole_dealing_statuses[player_index].popleft()
 
             statuses.append(status)
             self.hole_cards[player_index].append(card)
             self.hole_card_statuses[player_index].append(status)
@@ -2605,15 +2578,15 @@
         :return: The board dealing.
         :raises ValueError: If the board dealing cannot be done.
         """
         cards = self.verify_board_dealing(cards)
 
         assert self.board_dealing_count
 
-        self._make_available(cards)
+        self._make_card_available(cards)
 
         self.board_dealing_count -= len(cards)
         self.board_cards.extend(cards)
 
         if (
                 not any(self.hole_dealing_statuses)
                 and not self.board_dealing_count
@@ -2658,15 +2631,15 @@
 
         :param cards: The optional discarded cards.
         :return: The discarded cards.
         :raises ValueError: If the discard cannot be done.
         """
         self._verify_standing_pat_or_discarding()
 
-        cards = self._clean_cards(cards)
+        cards = Card.clean(cards)
         player_index = self.stander_pat_or_discarder_index
 
         assert player_index is not None
 
         if not set(cards) <= set(self.hole_cards[player_index]):
             raise ValueError('discarded cards not a subset of hole cards')
 
@@ -3683,15 +3656,18 @@
 
         self._end_chips_pushing()
 
         return self.ChipsPushing(tuple(self.bets))
 
     # chips pulling
 
-    chips_pulling_statuses: list[bool] = field(default_factory=list, init=False)
+    chips_pulling_statuses: list[bool] = field(
+        default_factory=list,
+        init=False,
+    )
     """The chips pulling statuses."""
 
     def _setup_chips_pulling(self) -> None:
         assert not self.chips_pulling_statuses
 
         for _ in range(self.player_count):
             self.chips_pulling_statuses.append(False)
```

### Comparing `pokerkit-0.0.0/pokerkit/tests/test_lookups.py` & `pokerkit-0.0.1/pokerkit/tests/test_lookups.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.0.0/pokerkit/tests/test_state.py` & `pokerkit-0.0.1/pokerkit/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.0.0/pokerkit/tests/test_utilities.py` & `pokerkit-0.0.1/pokerkit/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `pokerkit-0.0.0/pokerkit/tests/test_wsop/test_2023_43.py` & `pokerkit-0.0.1/pokerkit/tests/test_wsop/test_2023_43.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [7340000, 3775000, 5110000, 8935000, 4545000],
         )
 
     def test_00_08_38(self) -> None:
@@ -153,15 +153,15 @@
         state.fold()
         state.complete_bet_or_raise_to(4990000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 6195000)
 
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [3735000, 4115000, 8765000, 4545000, 8545000],
         )
 
     def test_00_15_36(self) -> None:
@@ -228,15 +228,15 @@
         state.complete_bet_or_raise_to(225000)
         state.complete_bet_or_raise_to(700000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1875000)
 
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4050000, 8025000, 4550000, 8525000, 4550000],
         )
 
     def test_00_18_39(self) -> None:
@@ -295,15 +295,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to(300000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1000000)
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [7750000, 4825000, 8525000, 4550000, 4050000],
         )
 
     def test_00_22_43(self) -> None:
@@ -368,15 +368,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1050000)
 
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4000000, 7700000, 4775000, 8275000, 4950000],
         )
 
     def test_00_25_05(self) -> None:
@@ -477,15 +477,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2150000, 9750000, 4675000, 8225000, 4900000],
         )
 
     def test_00_29_03(self) -> None:
@@ -524,15 +524,15 @@
         state.complete_bet_or_raise_to()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 500000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2400000, 9700000, 4575000, 8175000, 4850000],
         )
 
     def test_00_30_52(self) -> None:
@@ -571,15 +571,15 @@
         state.fold()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 500000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2650000, 9600000, 4525000, 8125000, 4800000],
         )
 
     def test_00_32_02(self) -> None:
@@ -677,15 +677,15 @@
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2600000, 11250000, 4475000, 6675000, 4700000],
         )
 
     def test_00_34_43(self) -> None:
@@ -724,15 +724,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 500000)
 
         state.push_chips()
-        state.pull_chips(3)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2550000, 11150000, 4425000, 6925000, 4650000],
         )
 
     def test_00_35_59(self) -> None:
@@ -833,15 +833,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4750000, 9500000, 4175000, 6675000, 4600000],
         )
 
     def test_00_41_13(self) -> None:
@@ -916,15 +916,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4075000, 5275000, 6100000, 4750000, 9500000],
         )
 
     def test_00_43_47(self) -> None:
@@ -997,15 +997,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [7075000, 5900000, 4750000, 7900000, 4075000],
         )
 
     def test_00_46_43(self) -> None:
@@ -1053,15 +1053,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1100000)
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [5800000, 4350000, 8400000, 4075000, 7075000],
         )
 
     def test_00_48_29(self) -> None:
@@ -1136,16 +1136,16 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(1)
-        state.pull_chips(3)
+        state.pull_chips()
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4250000, 9375000, 4075000, 6200000, 5800000],
         )
 
     def test_00_51_22(self) -> None:
@@ -1219,15 +1219,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [7975000, 3875000, 7800000, 5800000, 4250000],
         )
 
     def test_00_55_24(self) -> None:
@@ -1300,15 +1300,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(3)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [3775000, 7600000, 5400000, 6550000, 6375000],
         )
 
     def test_00_58_03(self) -> None:
@@ -1381,16 +1381,16 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(1)
-        state.pull_chips(3)
+        state.pull_chips()
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [7500000, 5450000, 6550000, 6425000, 3775000],
         )
 
     def test_01_00_21(self) -> None:
@@ -1468,15 +1468,15 @@
 
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2300000)
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [6450000, 5575000, 4825000, 7450000, 5400000],
         )
 
     def test_01_02_14(self) -> None:
@@ -1528,15 +1528,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 550000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [6700000, 5525000, 4775000, 7350000, 5350000],
         )
 
     def test_01_03_57(self) -> None:
@@ -1589,15 +1589,15 @@
 
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 900000)
 
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [6650000, 5475000, 4675000, 7100000, 5800000],
         )
 
     def test_01_06_16(self) -> None:
@@ -1636,15 +1636,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 500000)
 
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [6600000, 5425000, 4575000, 7050000, 6050000],
         )
 
     def test_01_07_20(self) -> None:
@@ -1742,15 +1742,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [6500000, 3575000, 6625000, 7000000, 6000000],
         )
 
     def test_01_10_31(self) -> None:
@@ -1832,15 +1832,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2500000)
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [5650000, 3525000, 7875000, 6900000, 5750000],
         )
 
     def test_01_13_57(self) -> None:
@@ -1940,15 +1940,15 @@
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [5550000, 3075000, 10125000, 6850000, 4100000],
         )
 
     def test_01_18_22(self) -> None:
@@ -1988,15 +1988,15 @@
         state.complete_bet_or_raise_to(1100000)
         state.complete_bet_or_raise_to(3350000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 4600000)
 
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4050000, 4350000, 3075000, 10125000, 8100000],
         )
 
     def test_01_22_35(self) -> None:
@@ -2034,15 +2034,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 525000)
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4300000, 2875000, 10375000, 8100000, 4050000],
         )
 
     def test_01_25_08(self) -> None:
@@ -2080,15 +2080,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 600000)
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2825000, 10175000, 8350000, 4050000, 4300000],
         )
 
     def test_01_26_14(self) -> None:
@@ -2160,15 +2160,15 @@
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [10125000, 7700000, 4050000, 4300000, 3525000],
         )
 
     def test_01_29_49(self) -> None:
@@ -2238,16 +2238,16 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(0)
-        state.pull_chips(1)
+        state.pull_chips()
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [7750000, 4000000, 4300000, 3525000, 10125000],
         )
 
     def test_01_32_58(self) -> None:
@@ -2296,15 +2296,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to(800000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1650000)
 
         state.push_chips()
-        state.pull_chips(3)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [3950000, 3850000, 3525000, 10625000, 7750000],
         )
 
     def test_01_37_39(self) -> None:
@@ -2353,15 +2353,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to(375000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1025000)
 
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [3800000, 3175000, 10625000, 7750000, 4350000],
         )
 
     def test_01_39_18(self) -> None:
@@ -2432,15 +2432,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [3075000, 11925000, 7750000, 3150000, 3800000],
         )
 
     def test_01_42_31(self) -> None:
@@ -2511,15 +2511,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [13725000, 7550000, 3150000, 3800000, 1475000],
         )
 
     def test_01_44_49(self) -> None:
@@ -2554,15 +2554,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 700000)
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [7450000, 2950000, 4100000, 1475000, 13725000],
         )
 
     def test_01_45_43(self) -> None:
@@ -2596,15 +2596,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 300000)
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2850000, 4200000, 1475000, 13725000, 7450000],
         )
 
     def test_01_46_42(self) -> None:
@@ -2638,15 +2638,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 300000)
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4100000, 1575000, 13725000, 7450000, 2850000],
         )
 
     def test_01_47_38(self) -> None:
@@ -2701,15 +2701,15 @@
         state.deal_board()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1700000)
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [1475000, 14425000, 7450000, 2850000, 3500000],
         )
 
     def test_01_51_27(self) -> None:
@@ -2767,15 +2767,15 @@
         state.deal_board()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2700000)
 
         state.push_chips()
-        state.pull_chips(3)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [14325000, 7250000, 2850000, 4800000, 475000],
         )
 
     def test_01_53_52(self) -> None:
@@ -2814,15 +2814,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 500000)
 
         state.push_chips()
-        state.pull_chips(3)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [7200000, 2600000, 4800000, 775000, 14325000],
         )
 
     def test_01_56_25(self) -> None:
@@ -2861,15 +2861,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1225000)
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2525000, 4425000, 1225000, 14325000, 7200000],
         )
 
     def test_01_59_02(self) -> None:
@@ -2908,15 +2908,15 @@
         state.fold()
         state.complete_bet_or_raise_to(1000000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1375000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4800000, 850000, 14325000, 7200000, 2525000],
         )
 
     def test_02_00_25(self) -> None:
@@ -2955,15 +2955,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 825000)
 
         state.push_chips()
-        state.pull_chips(3)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [775000, 13950000, 7200000, 2975000, 4800000],
         )
 
     def test_02_01_50(self) -> None:
@@ -3016,15 +3016,15 @@
         state.deal_hole()
         state.deal_hole()
         state.deal_hole()
         self.assertEqual(state.total_pot_amount, 1850000)
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [13875000, 6200000, 2975000, 4800000, 1850000],
         )
 
     def test_02_04_37(self) -> None:
@@ -3084,15 +3084,15 @@
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [6125000, 2400000, 4800000, 1850000, 14525000],
         )
 
     def test_02_07_21(self) -> None:
@@ -3134,15 +3134,15 @@
         state.fold()
         state.complete_bet_or_raise_to(2400000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2775000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2775000, 4425000, 1850000, 14525000, 6125000],
         )
 
     def test_02_09_20(self) -> None:
@@ -3241,16 +3241,16 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(0)
-        state.pull_chips(4)
+        state.pull_chips()
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4537500, 1800000, 14400000, 6075000, 2887500],
         )
 
     def test_02_13_08(self) -> None:
@@ -3289,15 +3289,15 @@
         state.fold()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 575000)
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4500000, 1750000, 14675000, 5950000, 2825000],
         )
 
     def test_02_14_32(self) -> None:
@@ -3395,16 +3395,16 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(0)
-        state.pull_chips(2)
+        state.pull_chips()
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4575000, 1700000, 14750000, 5900000, 2775000],
         )
 
     def test_02_18_42(self) -> None:
@@ -3503,16 +3503,16 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(3)
-        state.pull_chips(4)
+        state.pull_chips()
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4525000, 1650000, 14700000, 5975000, 2850000],
         )
 
     def test_02_22_35(self) -> None:
@@ -3564,15 +3564,15 @@
 
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1000000)
 
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4475000, 1600000, 14650000, 5675000, 3300000],
         )
 
     def test_02_25_11(self) -> None:
@@ -3651,15 +3651,15 @@
 
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2750000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [5675000, 1550000, 14600000, 4625000, 3250000],
         )
 
     def test_02_28_14(self) -> None:
@@ -3713,15 +3713,15 @@
 
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1000000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [6125000, 1500000, 14550000, 4575000, 2950000],
         )
 
     def test_02_29_59(self) -> None:
@@ -3805,15 +3805,15 @@
         state.stand_pat_or_discard()
         state.burn_card()
         state.deal_hole()
         self.assertEqual(state.total_pot_amount, 3000000)
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4625000, 3000000, 14550000, 4575000, 2950000],
         )
 
     def test_02_34_51(self) -> None:
@@ -3851,15 +3851,15 @@
         state.complete_bet_or_raise_to()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 875000)
 
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2875000, 14300000, 4575000, 2950000, 5000000],
         )
 
     def test_02_36_12(self) -> None:
@@ -3953,15 +3953,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [14175000, 2325000, 2950000, 5000000, 5250000],
         )
 
     def test_02_40_27(self) -> None:
@@ -3999,15 +3999,15 @@
         state.fold()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 750000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2575000, 2700000, 5000000, 5250000, 14175000],
         )
 
     def test_02_41_31(self) -> None:
@@ -4045,15 +4045,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 875000)
 
         state.push_chips()
-        state.pull_chips(3)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2575000, 4750000, 5250000, 14550000, 2575000],
         )
 
     def test_02_42_44(self) -> None:
@@ -4141,15 +4141,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4625000, 2500000, 17425000, 2575000, 2575000],
         )
 
     def test_02_46_42(self) -> None:
@@ -4233,15 +4233,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2375000, 19050000, 2575000, 2575000, 3125000],
         )
 
     def test_02_51_10(self) -> None:
@@ -4277,15 +4277,15 @@
         state.fold()
         state.complete_bet_or_raise_to(2350000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2725000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [19425000, 2200000, 2575000, 3125000, 2375000],
         )
 
     def test_02_53_09(self) -> None:
@@ -4321,15 +4321,15 @@
         state.fold()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2825000)
 
         state.push_chips()
-        state.pull_chips(3)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2125000, 2200000, 3125000, 2825000, 19425000],
         )
 
     def test_02_54_12(self) -> None:
@@ -4366,15 +4366,15 @@
         state.complete_bet_or_raise_to(2200000)
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2875000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2875000, 2750000, 2825000, 19125000, 2125000],
         )
 
     def test_02_56_12(self) -> None:
@@ -4411,15 +4411,15 @@
         state.fold()
         state.complete_bet_or_raise_to(2600000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 3200000)
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2675000, 3200000, 18825000, 2125000, 2875000],
         )
 
     def test_02_57_27(self) -> None:
@@ -4466,15 +4466,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to(350000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1450000)
 
         state.push_chips()
-        state.pull_chips(3)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [3125000, 18200000, 2125000, 3575000, 2675000],
         )
 
     def test_03_00_32(self) -> None:
@@ -4511,15 +4511,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to(1900000)
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2275000)
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [18050000, 2275000, 3575000, 2675000, 3125000],
         )
 
     def test_03_02_41(self) -> None:
@@ -4578,15 +4578,15 @@
 
         state.burn_card()
         state.deal_board()
         self.assertEqual(state.total_pot_amount, 7000000)
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(4)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2200000, 0, 2675000, 3125000, 21700000],
         )
 
     def test_03_05_55(self) -> None:
@@ -4682,15 +4682,15 @@
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(3)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2550000, 1825000, 21650000, 3675000],
         )
 
     def test_03_11_08(self) -> None:
@@ -4729,15 +4729,15 @@
         state.complete_bet_or_raise_to()
         state.fold()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1025000)
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2375000, 2525000, 21475000, 3325000],
         )
 
     def test_03_12_55(self) -> None:
@@ -4791,15 +4791,15 @@
         state.complete_bet_or_raise_to()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2025000)
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2325000, 3500000, 20675000, 3200000],
         )
 
     def test_03_14_40(self) -> None:
@@ -4896,15 +4896,15 @@
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2275000, 5650000, 18625000, 3150000],
         )
 
     def test_03_17_31(self) -> None:
@@ -4956,15 +4956,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1025000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2750000, 5525000, 18325000, 3100000],
         )
 
     def test_03_19_14(self) -> None:
@@ -5041,15 +5041,15 @@
         state.check_or_call()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 1775000)
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2625000, 6250000, 18275000, 2550000],
         )
 
     def test_03_22_08(self) -> None:
@@ -5121,16 +5121,16 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(1)
-        state.pull_chips(2)
+        state.pull_chips()
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2375000, 6375000, 18400000, 2550000],
         )
 
     def test_03_25_05(self) -> None:
@@ -5205,15 +5205,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(2)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [125000, 6125000, 22150000, 1300000],
         )
 
     def test_03_32_24(self) -> None:
@@ -5279,15 +5279,15 @@
         state.check_or_call()
         state.check_or_call()
         self.assertEqual(state.total_pot_amount, 1625000)
 
         state.kill_hand()
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [5375000, 23025000, 1300000, 0],
         )
 
     def test_03_36_22(self) -> None:
@@ -5358,16 +5358,16 @@
         state.complete_bet_or_raise_to()
         state.check_or_call()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 5900000)
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(0)
-        state.pull_chips(2)
+        state.pull_chips()
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [25150000, 0, 4550000],
         )
 
     def test_03_42_38(self) -> None:
@@ -5437,16 +5437,16 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(0)
-        state.pull_chips(1)
+        state.pull_chips()
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [4550000, 25150000],
         )
 
     def test_03_44_38(self) -> None:
@@ -5519,16 +5519,16 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(0)
-        state.pull_chips(1)
+        state.pull_chips()
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [25150000, 4550000],
         )
 
     def test_03_46_32(self) -> None:
@@ -5599,15 +5599,15 @@
 
         # Showdown
 
         state.show_or_muck_hole_cards()
         state.show_or_muck_hole_cards()
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2150000, 27550000],
         )
 
     def test_03_48_33(self) -> None:
@@ -5643,15 +5643,15 @@
         state.post_bring_in()
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 600000)
 
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [1950000, 27750000],
         )
 
     def test_03_49_18(self) -> None:
@@ -5713,15 +5713,15 @@
 
         state.complete_bet_or_raise_to()
         state.fold()
         state.collect_bets()
         self.assertEqual(state.total_pot_amount, 2000000)
 
         state.push_chips()
-        state.pull_chips(0)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [2650000, 27050000],
         )
 
     def test_03_50_24(self) -> None:
@@ -5810,13 +5810,13 @@
         for _ in range(2):
             state.deal_hole()
 
         self.assertEqual(state.total_pot_amount, 5300000)
 
         state.kill_hand()
         state.push_chips()
-        state.pull_chips(1)
+        state.pull_chips()
         self.assertEqual(state.total_pot_amount, 0)
         self.assertEqual(
             state.stacks,
             [0, 29700000],
         )
```

### Comparing `pokerkit-0.0.0/pokerkit/utilities.py` & `pokerkit-0.0.1/pokerkit/utilities.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """:mod:`pokerkit.utilities` implements classes related to poker
 utilities.
 """
 
 from __future__ import annotations
 
-from collections.abc import Iterable, Iterator
+from collections.abc import Iterable, Iterator, Mapping
 from dataclasses import dataclass
 from enum import Enum, StrEnum, unique
 from functools import partial
 from itertools import product, starmap
 from operator import is_not
 from typing import Any
 
@@ -224,109 +224,147 @@
 
     rank: Rank
     """The rank."""
     suit: Suit
     """The suit."""
 
     @classmethod
-    def get_ranks(cls, cards: Iterable[Card]) -> Iterator[Rank]:
+    def get_ranks(
+            cls,
+            cards: Iterable[Card] | str | Card | None,
+    ) -> Iterator[Rank]:
         """Return an iterator of the ranks of each card.
 
-        >>> Card.get_ranks(Card.parse('2sKh'))  # doctest: +ELLIPSIS
+        >>> Card.get_ranks('2sKh')  # doctest: +ELLIPSIS
         <generator object Card.get_ranks at 0x...>
-        >>> list(Card.get_ranks(Card.parse('2sKh')))
+        >>> list(Card.get_ranks('2sKh'))
         [<Rank.DEUCE: '2'>, <Rank.KING: 'K'>]
 
         :param cards: The cards to get ranks from.
         :return: The iterator of the ranks of each card.
         """
-        for card in cards:
+        for card in cls.clean(cards):
             yield card.rank
 
     @classmethod
-    def get_suits(cls, cards: Iterable[Card]) -> Iterator[Suit]:
+    def get_suits(
+            cls,
+            cards: Iterable[Card] | str | Card | None,
+    ) -> Iterator[Suit]:
         """Return an iterator of the suits of each card.
 
-        >>> Card.get_suits(Card.parse('2sKh'))  # doctest: +ELLIPSIS
+        >>> Card.get_suits('2sKh')  # doctest: +ELLIPSIS
         <generator object Card.get_suits at 0x...>
-        >>> list(Card.get_suits(Card.parse('2sKh')))
+        >>> list(Card.get_suits('2sKh'))
         [<Suit.SPADE: 's'>, <Suit.HEART: 'h'>]
 
         :param cards: The cards to get suits from.
         :return: The iterator of the suits of each card.
         """
-        for card in cards:
+        for card in cls.clean(cards):
             yield card.suit
 
     @classmethod
-    def are_paired(cls, cards: Iterable[Card]) -> bool:
+    def are_paired(cls, cards: Iterable[Card] | str | Card | None) -> bool:
         """Return the pairedness of the given cards.
 
         The cards are paired if at least two of the cards share a
         common rank.
 
         >>> Card.are_paired(())
         False
-        >>> Card.are_paired(Card.parse('2sKh'))
+        >>> Card.are_paired('2sKh')
         False
-        >>> Card.are_paired(Card.parse('2sKh2h'))
+        >>> Card.are_paired('2sKh2h')
         True
-        >>> Card.are_paired(Card.parse('2s2c2h'))
+        >>> Card.are_paired('2s2c2h')
         True
 
         :param cards: The cards to determine the pairedness from.
         :return: The pairedness of the cards.
         """
         ranks = tuple(cls.get_ranks(cards))
 
         return len(set(ranks)) != len(ranks)
 
     @classmethod
-    def are_suited(cls, cards: Iterable[Card]) -> bool:
+    def are_suited(cls, cards: Iterable[Card] | str | Card | None) -> bool:
         """Return the suitedness of the given cards.
 
         The cards are suited if all of the cards share a common suit.
 
         >>> Card.are_suited(())
         True
-        >>> Card.are_suited(Card.parse('2s'))
+        >>> Card.are_suited('2s')
         True
-        >>> Card.are_suited(Card.parse('2sKh3s'))
+        >>> Card.are_suited('2sKh3s')
         False
-        >>> Card.are_suited(Card.parse('2hKh3h'))
+        >>> Card.are_suited('2hKh3h')
         True
 
         :param cards: The cards to determine the suitedness from.
         :return: The suitedness of the cards.
         """
         return len(set(cls.get_suits(cards))) <= 1
 
     @classmethod
-    def are_rainbow(cls, cards: Iterable[Card]) -> bool:
+    def are_rainbow(cls, cards: Iterable[Card] | str | Card | None) -> bool:
         """Return whether the cards are rainbow.
 
         The cards are rainbow if no two cards share a common suit.
 
         >>> Card.are_rainbow(())
         True
-        >>> Card.are_rainbow(Card.parse('2s'))
+        >>> Card.are_rainbow('2s')
         True
-        >>> Card.are_rainbow(Card.parse('2sKh3c'))
+        >>> Card.are_rainbow('2sKh3c')
         True
-        >>> Card.are_rainbow(Card.parse('2hKh3c'))
+        >>> Card.are_rainbow('2hKh3c')
         False
 
         :param cards: The cards to determine whether they are rainbow.
         :return: ``True`` if the cards are rainbow, otherwise ``False``.
         """
         suits = tuple(cls.get_suits(cards))
 
         return len(set(suits)) == len(suits)
 
     @classmethod
+    def clean(
+            cls,
+            values: Iterable[Card] | str | Card | None,
+    ) -> tuple[Card, ...]:
+        """Clean the cards.
+
+        >>> Card.clean('AsKs')
+        (As, Ks)
+        >>> Card.clean('AsKs')
+        (As, Ks)
+        >>> Card.clean(Card(Rank.ACE, Suit.SPADE))
+        (As,)
+        >>> Card.clean(None)
+        ()
+
+        :param values: The cards.
+        :return: The cleaned cards.
+        """
+        if values is None:
+            values = ()
+        elif isinstance(values, Card):
+            values = (values,)
+        elif isinstance(values, str):
+            values = tuple(Card.parse(values))
+        elif not isinstance(values, tuple) and isinstance(values, Iterable):
+            assert not isinstance(values, str)
+
+            values = tuple(values)
+
+        return values
+
+    @classmethod
     def parse(cls, *raw_cards: str) -> Iterator[Card]:
         """Parse the string of the card representations.
 
         >>> Card.parse('AsKsQsJsTs')  # doctest: +ELLIPSIS
         <generator object Card.parse at 0x...>
         >>> list(Card.parse('2c8d5sKh'))
         [2c, 8d, 5s, Kh]
@@ -509,7 +547,56 @@
     :param key: The optional key function.
     :return: The maximum value if any, otherwise ``None``.
     """
     try:
         return max(filter_none(values), key=key)
     except ValueError:
         return None
+
+
+def clean_values(
+        values: Iterable[int] | Mapping[int, int] | int | None,
+        count: int,
+) -> tuple[int, ...]:
+    """Clean the integers.
+
+    >>> clean_values([1, 2, 3, 4], 4)
+    (1, 2, 3, 4)
+    >>> clean_values([1, 2, 3, 4], 6)
+    (1, 2, 3, 4, 0, 0)
+    >>> clean_values({0: 1, -1: 2}, 4)
+    (1, 0, 0, 2)
+    >>> clean_values(4, 4)
+    (4, 4, 4, 4)
+    >>> clean_values(None, 4)
+    (0, 0, 0, 0)
+
+    :param values: The values.
+    :param count: The number of values.
+    :return: The cleaned integers.
+    """
+    if values is None:
+        values = (0,) * count
+    elif isinstance(values, int):
+        values = (values,) * count
+    elif isinstance(values, Mapping):
+        parsed_values = [0] * count
+
+        for key, value in values.items():
+            parsed_values[key] = value
+
+        values = tuple(parsed_values)
+    elif (
+            not (isinstance(values, tuple) and len(values) == count)
+            and isinstance(values, Iterable)
+    ):
+        parsed_values = list(values)
+
+        if len(parsed_values) > count:
+            raise ValueError('too many values')
+
+        while len(parsed_values) < count:
+            parsed_values.append(0)
+
+        values = tuple(parsed_values)
+
+    return values
```

### Comparing `pokerkit-0.0.0/pokerkit.egg-info/PKG-INFO` & `pokerkit-0.0.1/pokerkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pokerkit
-Version: 0.0.0
+Version: 0.0.1
 Summary: A Python package for various poker tools
 Home-page: https://github.com/uoftcprg/pokerkit
 Author: University of Toronto Computer Poker Research Group
 Author-email: uoftcprg@outlook.com
 License: MIT
 Project-URL: Documentation, https://pokerkit.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/uoftcprg/pokerkit
 Project-URL: Tracker, https://github.com/uoftcprg/pokerkit/issues
-Keywords: poker,nlhe,ai,game,game theory,libratus,modicum
+Keywords: artificial-intelligence,deep-learning,game,game-development,game-theory,holdem-poker,imperfect-information-game,libratus,pluribus,poker,poker-engine,poker-evaluator,poker-game,poker-hands,poker-library,poker-strategies,python,reinforcement-learning,texas-holdem
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Education
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Scientific/Engineering
@@ -29,37 +29,37 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ========
 PokerKit
 ========
 
-``PokerKit`` is an open-source Python library for simulating poker games and
+PokerKit is an open-source Python library for simulating poker games and
 evaluating poker hands, developed by the University of Toronto Computer Poker
 Research Group. It provides extensive support for all major and minor poker
 variants, offers a high level of control over game states, and supports
 high-speed hand evaluations.
 
 **Installation**
 ----------------
 
-The ``PokerKit`` library can be installed using pip:
+The PokerKit library can be installed using pip:
 
 .. code-block:: bash
 
    pip install pokerkit
 
 **Features**
 ------------
 
 * Extensive poker game logic for major and minor poker variants
 * High-speed hand evaluations
 * Customizable game states and parameters
-* Robust implementation with extensive unit tests and doctests
-* Ability to simulate famous hands from poker history
+* Robust implementation with static type checking and extensive unit tests and
+  doctests
 
 **Usage**
 ---------
 
 Below shows the first televised million dollar pot between Tom Dwan and Phil
 Ivey.
 
@@ -73,16 +73,16 @@
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
            Automation.BLIND_OR_STRADDLE_POSTING,
            Automation.CARD_BURNING,
            Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
            Automation.HAND_KILLING,
-           Automation.CHIP_PUSHING,
-           Automation.CHIP_PULLING,
+           Automation.CHIPS_PUSHING,
+           Automation.CHIPS_PULLING,
        ),
        True,
        500,
        (1000, 2000),
        2000,
        (1125600, 2000000, 553500),
        3,
@@ -257,16 +257,16 @@
        (
            Automation.ANTE_POSTING,
            Automation.BET_COLLECTION,
            Automation.BLIND_OR_STRADDLE_POSTING,
            Automation.CARD_BURNING,
            Automation.HOLE_CARDS_SHOWING_OR_MUCKING,
            Automation.HAND_KILLING,
-           Automation.CHIP_PUSHING,
-           Automation.CHIP_PULLING,
+           Automation.CHIPS_PUSHING,
+           Automation.CHIPS_PULLING,
        ),
        True,
        None,
        (75000, 150000),
        150000,
        300000,
        (1180000, 4340000, 5910000, 10765000),
@@ -398,36 +398,36 @@
    # Below show the final stacks.
 
    print(state.stacks)  # [196, 220, 200, 184]
 
 **Testing and Validation**
 --------------------------
 
-``PokerKit`` has extensive test coverage, passes mypy static type checking with
+PokerKit has extensive test coverage, passes mypy static type checking with
 strict parameter, and has been validated through extensive use in real-life
 scenarios.
 
 **Contributing**
 ----------------
 
 Contributions are welcome! Please read our
 `Contributing Guide <CONTRIBUTING.rst>`_ for more information.
 
 **License**
 -----------
 
-``PokerKit`` is distributed under the MIT license. See `LICENSE <LICENSE>`_ for
+PokerKit is distributed under the MIT license. See `LICENSE <LICENSE>`_ for
 more information.
 
 **Citing**
 ----------
 
-If you use ``PokerKit`` in your research, please cite our library:
+If you use PokerKit in your research, please cite our library:
 
 .. code-block:: bibtex
 
    @misc{pokerkit,
      title={PokerKit: An Open-Source Python Library for Poker Simulations and Hand Evaluations},
-     author={Your name here},
+     author={Juho Kim},
      year={2023},
      url={https://github.com/uoftcprg/pokerkit}
    }
```

### Comparing `pokerkit-0.0.0/setup.py` & `pokerkit-0.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 
 with open('README.rst', 'r') as file:
     long_description = file.read()
 
 setup(
     name='pokerkit',
-    version='0.0.0',
+    version='0.0.1',
     description='A Python package for various poker tools',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     url='https://github.com/uoftcprg/pokerkit',
     author='University of Toronto Computer Poker Research Group',
     author_email='uoftcprg@outlook.com',
     license='MIT',
@@ -29,21 +29,33 @@
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     keywords=[
-        'poker',
-        'nlhe',
-        'ai',
+        'artificial-intelligence',
+        'deep-learning',
         'game',
-        'game theory',
+        'game-development',
+        'game-theory',
+        'holdem-poker',
+        'imperfect-information-game',
         'libratus',
-        'modicum',
+        'pluribus',
+        'poker',
+        'poker-engine',
+        'poker-evaluator',
+        'poker-game',
+        'poker-hands',
+        'poker-library',
+        'poker-strategies',
+        'python',
+        'reinforcement-learning',
+        'texas-holdem',
     ],
     project_urls={
         'Documentation': 'https://pokerkit.readthedocs.io/en/latest/',
         'Source': 'https://github.com/uoftcprg/pokerkit',
         'Tracker': 'https://github.com/uoftcprg/pokerkit/issues',
     },
     package_data={'pokerkit': ['py.typed']},
```

