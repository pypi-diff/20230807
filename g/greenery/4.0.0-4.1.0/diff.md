# Comparing `tmp/greenery-4.0.0.tar.gz` & `tmp/greenery-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\qntm\Documents\programming\GitHub\pypi\greenery\repo\dist\tmpn3uc5lqu\greenery-4.0.0.tar", last modified: Tue Nov  8 17:32:44 2022, max compression
+gzip compressed data, was "greenery-4.1.0.tar", last modified: Sun Aug  6 23:18:06 2023, max compression
```

## Comparing `greenery-4.0.0.tar` & `greenery-4.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2022-11-08 17:32:44.888613 greenery-4.0.0/
--rw-rw-rw-   0        0        0     1082 2022-05-22 15:44:09.000000 greenery-4.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0      498 2022-11-08 17:32:44.888180 greenery-4.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     9409 2022-11-08 17:30:30.000000 greenery-4.0.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-08 17:32:44.868945 greenery-4.0.0/greenery/
--rw-rw-rw-   0        0        0      644 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/__init__.py
--rw-rw-rw-   0        0        0     2232 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/bound.py
--rw-rw-rw-   0        0        0      254 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/bound_test.py
--rw-rw-rw-   0        0        0     8549 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/charclass.py
--rw-rw-rw-   0        0        0     2492 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/charclass_test.py
--rw-rw-rw-   0        0        0     2438 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/conc_test.py
--rw-rw-rw-   0        0        0    30719 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/fsm.py
--rw-rw-rw-   0        0        0    21291 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/fsm_test.py
--rw-rw-rw-   0        0        0     2508 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/mult_test.py
--rw-rw-rw-   0        0        0     6451 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/multiplier.py
--rw-rw-rw-   0        0        0     3873 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/multiplier_test.py
--rw-rw-rw-   0        0        0     9322 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/parse.py
--rw-rw-rw-   0        0        0     7172 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/parse_test.py
--rw-rw-rw-   0        0        0     3937 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/pattern_test.py
--rw-rw-rw-   0        0        0    34226 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/rxelems.py
--rw-rw-rw-   0        0        0    32961 2022-11-08 17:30:30.000000 greenery-4.0.0/greenery/rxelems_test.py
-drwxrwxrwx   0        0        0        0 2022-11-08 17:32:44.886667 greenery-4.0.0/greenery.egg-info/
--rw-rw-rw-   0        0        0      498 2022-11-08 17:32:44.000000 greenery-4.0.0/greenery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      512 2022-11-08 17:32:44.000000 greenery-4.0.0/greenery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-08 17:32:44.000000 greenery-4.0.0/greenery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-11-08 17:32:44.000000 greenery-4.0.0/greenery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-08 17:32:44.888726 greenery-4.0.0/setup.cfg
--rw-rw-rw-   0        0        0      769 2022-11-08 17:30:30.000000 greenery-4.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-06 23:18:06.811395 greenery-4.1.0/
+-rw-rw-rw-   0        0        0     1082 2022-05-22 15:44:09.000000 greenery-4.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      498 2023-08-06 23:18:06.811395 greenery-4.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9461 2023-08-03 20:40:33.000000 greenery-4.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-06 23:18:06.800358 greenery-4.1.0/greenery/
+-rw-rw-rw-   0        0        0      307 2023-04-14 17:46:24.000000 greenery-4.1.0/greenery/__init__.py
+-rw-rw-rw-   0        0        0     2570 2023-08-03 20:40:33.000000 greenery-4.1.0/greenery/bound.py
+-rw-rw-rw-   0        0        0     2841 2023-08-03 20:40:33.000000 greenery-4.1.0/greenery/bound_test.py
+-rw-rw-rw-   0        0        0    13684 2023-08-06 23:17:09.000000 greenery-4.1.0/greenery/charclass.py
+-rw-rw-rw-   0        0        0     9309 2023-08-06 23:17:09.000000 greenery-4.1.0/greenery/charclass_test.py
+-rw-rw-rw-   0        0        0     2518 2023-08-06 19:09:38.000000 greenery-4.1.0/greenery/conc_test.py
+-rw-rw-rw-   0        0        0    32594 2023-08-06 23:17:09.000000 greenery-4.1.0/greenery/fsm.py
+-rw-rw-rw-   0        0        0    36234 2023-08-06 23:17:09.000000 greenery-4.1.0/greenery/fsm_test.py
+-rw-rw-rw-   0        0        0     2413 2023-08-06 23:17:09.000000 greenery-4.1.0/greenery/mult_test.py
+-rw-rw-rw-   0        0        0     6601 2023-08-03 20:40:33.000000 greenery-4.1.0/greenery/multiplier.py
+-rw-rw-rw-   0        0        0     4342 2023-08-03 20:40:33.000000 greenery-4.1.0/greenery/multiplier_test.py
+-rw-rw-rw-   0        0        0     9968 2023-08-06 23:17:09.000000 greenery-4.1.0/greenery/parse.py
+-rw-rw-rw-   0        0        0     8003 2023-08-06 23:17:09.000000 greenery-4.1.0/greenery/parse_test.py
+-rw-rw-rw-   0        0        0     4579 2023-08-06 19:11:22.000000 greenery-4.1.0/greenery/pattern_test.py
+-rw-rw-rw-   0        0        0    32465 2023-08-06 23:17:09.000000 greenery-4.1.0/greenery/rxelems.py
+-rw-rw-rw-   0        0        0    44492 2023-08-06 23:17:09.000000 greenery-4.1.0/greenery/rxelems_test.py
+drwxrwxrwx   0        0        0        0 2023-08-06 23:18:06.809125 greenery-4.1.0/greenery.egg-info/
+-rw-rw-rw-   0        0        0      498 2023-08-06 23:18:06.000000 greenery-4.1.0/greenery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2023-08-06 23:18:06.000000 greenery-4.1.0/greenery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-06 23:18:06.000000 greenery-4.1.0/greenery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-06 23:18:06.000000 greenery-4.1.0/greenery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-06 23:18:06.811395 greenery-4.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-08-06 23:17:23.000000 greenery-4.1.0/setup.py
```

### Comparing `greenery-4.0.0/LICENSE.txt` & `greenery-4.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `greenery-4.0.0/README.md` & `greenery-4.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -56,22 +56,22 @@
 
 * This method is intentionally rigorously simple, and tolerates no ambiguity. For example, a hyphen must be escaped in a character class even if it appears first or last. `[-abc]` is a syntax error, write `[\-abc]`. Escaping something which doesn't need it is a syntax error too: `[\ab]` resolves to neither `[\\ab]` nor `[ab]`.
 
 * The `^` and `$` metacharacters are not supported. By default, `greenery` assumes that all regexes are anchored at the start and end of any input string. Carets and dollar signs will be parsed as themselves. If you want to *not* anchor at the start or end of the string, put `.*` at the start or end of your regex respectively.
 
   This is because computing the intersection between `.*a.*` and `.*b.*` (1) is largely pointless and (2) usually results in gibberish coming out of the program.
 
-* The greedy operators `*?`, `+?`, `??` and `{m,n}?` are not supported, since they do not alter the regular language.
+* The non-greedy operators `*?`, `+?`, `??` and `{m,n}?` are not supported, since they do not alter the regular language.
 
 * Parentheses are used to alternate between multiple possibilities e.g. `(a|bc)` only, not for capture grouping. Here's why:
 
-        ```python
-        print(parse("(ab)c") & parse("a(bc)"))
-        # "abc"
-        ```
+  ```python
+  print(parse("(ab)c") & parse("a(bc)"))
+  # "abc"
+  ```
 
 * The `(?:...)` syntax for non-capturing groups is permitted, but does nothing.
 
 * Other `(?...)` constructs are not supported (and most are not [regular in the computer science sense](http://en.wikipedia.org/wiki/Regular_language)).
 
 *  Back-references, such as `([aeiou])\1`, are not regular.
 
@@ -105,26 +105,27 @@
 #### pattern.reduce()
 
 Call this method to try to simplify the regular expression object. The follow simplification heuristics are supported:
 
 * `(ab|cd|ef|)g` to `(ab|cd|ef)?g`
 * `([ab])*` to `[ab]*`
 * `ab?b?c` to `ab{0,2}c`
+* `aa` to `a{2}`
 * `a(d(ab|a*c))` to `ad(ab|a*c)`
 * `0|[2-9]` to `[02-9]`
 * `abc|ade` to `a(bc|de)`
 * `xyz|stz` to `(xy|st)z`
 * `abc()def` to `abcdef`
 * `a{1,2}|a{3,4}` to `a{1,4}`
 
 The value returned is a new `Pattern` object.
 
 Note that in a few cases this did *not* result in a shorter regular expression.
 
-### Multiplier(Bound, Bound)
+### Multiplier
 
 A combination of a finite lower `Bound` (see below) and a possibly-infinite upper `Bound`.
 
 ```python
 from greenery import parse, Bound, INF, Multiplier
 
 print(parse("a") * Multiplier(Bound(3), INF)) # "a{3,}"
@@ -138,29 +139,34 @@
 
 Special `Multiplier`, equal to `Multiplier(Bound(0), Bound(1))`. When it appears in a regular expression, this is `{0,1}` or `?`.
 
 ### PLUS
 
 Special `Multiplier`, equal to `Multiplier(Bound(1), INF)`. When it appears in a regular expression, this is `{1,}` or `+`.
 
-### Bound(number)
+### Bound
 
 Represents a non-negative integer or infinity.
 
 ### INF
 
 Special `Bound` representing no limit. Can be used as an upper bound only.
 
 ## Development
 
 ### Running tests
 
 ```sh
-flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics
-flake8 . --count --exit-zero --max-complexity=10 --max-line-length=80 --statistics
+pip install -r requirements.dev.txt
+isort .
+black .
+mypy greenery
+flake8 --count --statistics --show-source --select=E9,F63,F7,F82 .
+flake8 --count --statistics --exit-zero --max-complexity=10 .
+pylint --recursive=true .
 pytest
 ```
 
 ### Building and publishing new versions
 
 * Update the version in `./setup.py`
 * Trash `./dist`
```

### Comparing `greenery-4.0.0/greenery/conc_test.py` & `greenery-4.1.0/greenery/conc_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import pytest
 
 from .bound import Bound
-from .multiplier import Multiplier, ZERO, QM, ONE, STAR, PLUS
 from .charclass import Charclass
-from .rxelems import Conc, Mult, EMPTYSTRING
+from .multiplier import ONE, PLUS, QM, STAR, ZERO, Multiplier
+from .rxelems import Conc, Mult
 
 
-def test_conc_equality():
+def test_conc_equality() -> None:
     a = Conc(Mult(Charclass("a"), ONE))
     assert a == Conc(Mult(Charclass("a"), ONE))
     assert a != Conc(Mult(Charclass("b"), ONE))
     assert a != Conc(Mult(Charclass("a"), QM))
-    assert a != Conc(Mult(
-        Charclass("a"),
-        Multiplier(Bound(1), Bound(2)))
-    )
-    assert a != EMPTYSTRING
+    assert a != Conc(Mult(Charclass("a"), Multiplier(Bound(1), Bound(2))))
+    assert a != Conc()
 
 
-def test_conc_str():
-    assert str(Conc(
-        Mult(Charclass("a"), ONE),
-        Mult(Charclass("b"), ONE),
-        Mult(Charclass("c"), ONE),
-        Mult(Charclass("d"), ONE),
-        Mult(Charclass("e"), ONE),
-        Mult(~Charclass("fg"), STAR),
-        Mult(Charclass("h"), Multiplier(Bound(5), Bound(5))),
-        Mult(Charclass("abcdefghijklmnopqrstuvwxyz"), PLUS),
-    )) == "abcde[^fg]*h{5}[a-z]+"
+def test_conc_str() -> None:
+    assert (
+        str(
+            Conc(
+                Mult(Charclass("a"), ONE),
+                Mult(Charclass("b"), ONE),
+                Mult(Charclass("c"), ONE),
+                Mult(Charclass("d"), ONE),
+                Mult(Charclass("e"), ONE),
+                Mult(~Charclass("fg"), STAR),
+                Mult(Charclass("h"), Multiplier(Bound(5), Bound(5))),
+                Mult(Charclass("abcdefghijklmnopqrstuvwxyz"), PLUS),
+            )
+        )
+        == "abcde[^fg]*h{5}[a-z]+"
+    )
 
 
-def test_conc_common():
+def test_conc_common() -> None:
     a = Mult(Charclass("A"), ONE)
     b = Mult(Charclass("B"), ONE)
     c = Mult(Charclass("C"), ONE)
     y = Mult(Charclass("y"), ONE)
     z = Mult(Charclass("Z"), ONE)
     zstar = Mult(Charclass("Z"), STAR)
 
@@ -43,34 +47,26 @@
     assert Conc(c, z).common(Conc(c, z), suffix=True) == Conc(c, z)
     assert Conc(c, y).common(Conc(c, z), suffix=True) == Conc()
     assert Conc(a, z).common(Conc(b, z), suffix=True) == Conc(z)
     assert Conc(a, zstar).common(Conc(b, z), suffix=True) == Conc()
     assert Conc(a).common(Conc(b), suffix=True) == Conc()
 
 
-def test_conc_dock():
+def test_conc_dock() -> None:
     a = Mult(Charclass("A"), ONE)
     b = Mult(Charclass("B"), ONE)
     x = Mult(Charclass("X"), ONE)
-    x2 = Mult(Charclass("X"), Multiplier(Bound(2), Bound(2)))
+    x_twice = Mult(Charclass("X"), Multiplier(Bound(2), Bound(2)))
     yplus = Mult(Charclass("y"), PLUS)
     z = Mult(Charclass("Z"), ONE)
 
     assert Conc(a, z).dock(Conc(z)) == Conc(a)
     assert Conc(a, b, x, yplus, z).dock(Conc(x, yplus, z)) == Conc(a, b)
     assert Conc(a, b, x, yplus, z).behead(Conc(a, b, x, yplus)) == Conc(z)
     assert Conc(a).dock(Conc()) == Conc(a)
 
-    try:
-        Conc(x2, yplus, z).behead(Conc(x, yplus))
-        assert False
-    except AssertionError:
-        assert False
-    except Exception:
-        pass
+    with pytest.raises(ArithmeticError, match="Can't subtract"):
+        Conc(x_twice, yplus, z).behead(Conc(x, yplus))
 
 
-def test_mult_reduction_easy():
-    assert Conc(Mult(
-        Charclass("a"),
-        ZERO
-    )).reduce() == Conc()
+def test_mult_reduction_easy() -> None:
+    assert Conc(Mult(Charclass("a"), ZERO)).reduce() == Conc()
```

### Comparing `greenery-4.0.0/greenery/fsm.py` & `greenery-4.1.0/greenery/fsm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,153 +1,206 @@
-# -*- coding: utf-8 -*-
+"""
+Finite state machine library, intended to be used by `greenery` only
+"""
+
+from __future__ import annotations
+
+__all__ = (
+    "Fsm",
+    "StateType",
+    "EPSILON",
+    "NULL",
+)
 
-'''
-    Finite state machine library, intended to be used by `greenery` only
-'''
-
-from typing import Optional, Union, Set, Dict
 from dataclasses import dataclass
+from typing import (
+    Callable,
+    ClassVar,
+    Collection,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Mapping,
+    TypeVar,
+)
+
+from .charclass import DOT, Charclass, repartition
+
+AlphaType = Charclass
+StateType = int
+M = TypeVar("M")
+"""Meta-state type for crawl(). Can be anything."""
+
+
+def unify_alphabets(fsms: Iterable[Fsm], /) -> List[Fsm]:
+    charclasses = set()
+    for fsm in fsms:
+        for charclass in fsm.alphabet:
+            charclasses.add(charclass)
 
-ANYTHING_ELSE = '9bd74361-04f9-4742-9d3a-1d14a6f0044c'
-
-
-def alphabet_key(symbol):
-    '''Ensure `ANYTHING_ELSE` always sorts last'''
-    return (symbol is ANYTHING_ELSE, symbol)
-
-
-class OblivionError(Exception):
-    '''
-        This exception is thrown while `crawl()`ing an FSM if we transition to
-        the oblivion state. For example while crawling two FSMs in parallel we
-        may transition to the oblivion state of both FSMs at once. This
-        warrants an out-of-band signal which will reduce the complexity of the
-        new FSM's map.
-    '''
-    pass
+    partition = repartition(charclasses)
+    # maps old Charclasses to collections of new Charclasses
 
+    return [fsm.replace_alphabet(partition) for fsm in fsms]
 
-state_type = Optional[Union[int, str]]
 
-
-@dataclass(frozen=True)
+# pylint: disable=too-many-public-methods,too-many-branches,fixme
+@dataclass(frozen=True, init=False)
 class Fsm:
-    '''
-        A Finite State Machine or FSM has an alphabet and a set of states. At
-        any given moment, the FSM is in one state. When passed a symbol from
-        the alphabet, the FSM jumps to another state (or possibly the same
-        state). A map (Python dictionary) indicates where to jump.
-        One state is nominated as a starting state. Zero or more states are
-        nominated as final states. If, after consuming a string of symbols,
-        the FSM is in a final state, then it is said to "accept" the string.
-        This class also has some pretty powerful methods which allow FSMs to
-        be concatenated, alternated between, multiplied, looped (Kleene star
-        closure), intersected, and simplified.
-        The majority of these methods are available using operator overloads.
-    '''
-    initial: state_type
-    finals: Set[state_type]
-    alphabet: Set[str]
-    states: Set[state_type]
-    map: Dict[state_type, Dict[str, state_type]]
-
-    def __post_init__(self):
-        '''
-            `alphabet` is an iterable of symbols the FSM can be fed.
-            `states` is the set of states for the FSM
-            `initial` is the initial state
-            `finals` is the set of accepting states
-            `map` may be sparse (i.e. it may omit transitions). In the case of
-            omitted transitions, a non-final "oblivion" state is simulated.
-        '''
+    """
+    A Finite State Machine or FSM has an alphabet and a set of states. At
+    any given moment, the FSM is in one state. When passed a symbol from
+    the alphabet, the FSM jumps to another state (or possibly the same
+    state). A map (Python dictionary) indicates where to jump.
+    One state is nominated as a starting state. Zero or more states are
+    nominated as final states. If, after consuming a string of symbols,
+    the FSM is in a final state, then it is said to "accept" the string.
+    This class also has some pretty powerful methods which allow FSMs to
+    be concatenated, alternated between, multiplied, looped (Kleene star
+    closure), intersected, and simplified.
+    The majority of these methods are available using operator overloads.
+    """
+
+    alphabet: frozenset[AlphaType]
+    states: frozenset[StateType]
+    initial: StateType
+    finals: frozenset[StateType]
+    map: Mapping[StateType, Mapping[AlphaType, StateType]]
+
+    # noinspection PyShadowingBuiltins
+    def __init__(
+        self,
+        /,
+        *,
+        alphabet: Iterable[AlphaType],
+        states: Iterable[StateType],
+        initial: StateType,
+        finals: Iterable[StateType],
+        # pylint: disable=redefined-builtin
+        map: Mapping[StateType, Mapping[AlphaType, StateType]],
+    ) -> None:
+        """
+        `alphabet` is an iterable of symbols the FSM can be fed.
+        `states` is the set of states for the FSM
+        `initial` is the initial state
+        `finals` is the set of accepting states
+        `map` may be sparse (i.e. it may omit transitions). In the case of
+        omitted transitions, a non-final "oblivion" state is simulated.
+        """
+        alphabet = frozenset(alphabet)
+        states = frozenset(states)
+        finals = frozenset(finals)
 
         # Validation. Thanks to immutability, this only needs to be carried out
         # once.
-        if self.initial not in self.states:
-            raise Exception(
-                f"Initial state {repr(self.initial)} "
-                f"must be one of {repr(self.states)}"
-            )
-        if not self.finals.issubset(self.states):
-            raise Exception(
-                f"Final states {repr(self.finals)} "
-                f"must be a subset of {repr(self.states)}"
-            )
-        for state, symbol in self.map.items():
-            for symbol in self.map[state]:
-                if not self.map[state][symbol] in self.states:
-                    raise Exception(
-                        f"Transition for state {repr(state)} "
-                        f"and symbol {repr(symbol)} "
-                        f"leads to {repr(self.map[state][symbol])}, "
-                        "which is not a state"
+        if initial not in states:
+            raise ValueError(f"Initial state {initial!r} must be one of {states!r}")
+        if not finals.issubset(states):
+            raise ValueError(f"Final states {finals!r} must be a subset of {states!r}")
+        for state, state_trans in map.items():
+            if state not in states:
+                raise ValueError(f"Transition from unknown state {state!r}")
+            for symbol, dest in state_trans.items():
+                if symbol not in alphabet:
+                    raise ValueError(
+                        f"Invalid symbol {symbol!r}"
+                        f" in transition from {state!r}"
+                        f" to {dest!r}"
+                    )
+                if dest not in states:
+                    raise ValueError(
+                        f"Transition for state {state!r}"
+                        f" and symbol {symbol!r}"
+                        f" leads to {dest!r},"
+                        " which is not a state"
                     )
+        for state in states:
+            if state not in map:
+                raise ValueError(f"State {state!r} missing from map")
+            for charclass in alphabet:
+                if charclass not in map[state]:
+                    raise ValueError(
+                        f"Symbol {charclass!r} missing from map[{state!r}]"
+                    )
+
+        # Check that the charclasses form a proper partition of all of Unicode
+        unified = Charclass()
+        for charclass in alphabet:
+            if unified & charclass != Charclass():
+                raise ValueError(f"Alphabet {alphabet!r} has overlaps")
+            unified |= charclass
+        if unified != DOT:
+            raise ValueError(f"Alphabet {alphabet!r} is not a proper partition")
 
         # Initialise the hard way due to immutability.
-        object.__setattr__(self, "alphabet", set(self.alphabet))
-        object.__setattr__(self, "states", set(self.states))
-        object.__setattr__(self, "finals", set(self.finals))
-
-    def accepts(self, input):
-        '''
-            Test whether the present FSM accepts the supplied string (iterable
-            of symbols). Equivalently, consider `self` as a possibly-infinite
-            set of strings and test whether `string` is a member of it. This is
-            actually mainly used for unit testing purposes. If `ANYTHING_ELSE`
-            is in your alphabet, then any symbol not in your alphabet will be
-            converted to `ANYTHING_ELSE`.
-        '''
+        object.__setattr__(self, "alphabet", alphabet)
+        object.__setattr__(self, "states", states)
+        object.__setattr__(self, "initial", initial)
+        object.__setattr__(self, "finals", finals)
+        object.__setattr__(self, "map", map)
+
+    def accepts(self, string: str, /) -> bool:
+        """
+        Test whether the present FSM accepts the supplied string (iterable
+        of symbols). Equivalently, consider `self` as a possibly-infinite
+        set of strings and test whether `string` is a member of it. This is
+        actually mainly used for unit testing purposes.
+        """
         state = self.initial
-        for symbol in input:
-            if ANYTHING_ELSE in self.alphabet and symbol not in self.alphabet:
-                symbol = ANYTHING_ELSE
-
-            # Missing transition = transition to dead state
-            if not (state in self.map and symbol in self.map[state]):
-                return False
-
-            state = self.map[state][symbol]
+        for char in string:
+            for charclass in self.map[state]:
+                if charclass.accepts(char):
+                    state = self.map[state][charclass]
+                    break
         return state in self.finals
 
-    def __contains__(self, string):
-        '''
-            This lets you use the syntax `"a" in fsm1` to see whether the
-            string "a" is in the set of strings accepted by `fsm1`.
-        '''
+    def __contains__(self, string: str, /) -> bool:
+        """
+        This lets you use the syntax `"a" in fsm1` to see whether the
+        string "a" is in the set of strings accepted by `fsm1`.
+        """
         return self.accepts(string)
 
-    def reduce(self):
-        '''
-            A result by Brzozowski (1963) shows that a minimal finite state
-            machine equivalent to the original can be obtained by reversing the
-            original twice.
-        '''
-        return reversed(reversed(self))
-
-    def __repr__(self):
-        args = ", ".join([
-            f"alphabet={repr(self.alphabet)}",
-            f"states={repr(self.states)}",
-            f"initial={repr(self.initial)}",
-            f"finals={repr(self.finals)}",
-            f"map={repr(self.map)}",
-        ])
+    def reduce(self, /) -> Fsm:
+        """
+        A result by Brzozowski (1963) shows that a minimal finite state
+        machine equivalent to the original can be obtained by reversing the
+        original twice.
+        """
+        return self.reversed().reversed()
+
+    def __repr__(self, /) -> str:
+        args = ", ".join(
+            [
+                f"alphabet={self.alphabet!r}",
+                f"states={self.states!r}",
+                f"initial={self.initial!r}",
+                f"finals={self.finals!r}",
+                f"map={self.map!r}",
+            ]
+        )
         return f"Fsm({args})"
 
-    def __str__(self):
+    # The Python `__eq__` + `__hash__` contract requires that value-equality
+    # implies hash-equality. `Fsm` `__eq__` implementation currently represents
+    # equality of the set of accepted strings, independent of specific state
+    # labels or unused members of the alphabet. This is not trivial to hash.
+    # Regarding the type suppression, see
+    # https://github.com/python/mypy/issues/4266
+    __hash__: ClassVar[None] = None  # type: ignore
+
+    def __str__(self, /) -> str:
         rows = []
 
-        sorted_alphabet = sorted(self.alphabet, key=alphabet_key)
+        sorted_alphabet = sorted(self.alphabet)
 
         # top row
         row = ["", "name", "final?"]
-        row.extend(
-          'ANYTHING_ELSE' if symbol is ANYTHING_ELSE else str(symbol)
-          for symbol in sorted_alphabet
-        )
+        row.extend(str(symbol) for symbol in sorted_alphabet)
         rows.append(row)
 
         # other rows
         for state in self.states:
             row = []
             if state == self.initial:
                 row.append("*")
@@ -155,697 +208,699 @@
                 row.append("")
             row.append(str(state))
             if state in self.finals:
                 row.append("True")
             else:
                 row.append("False")
             for symbol in sorted_alphabet:
-                if state in self.map and symbol in self.map[state]:
-                    row.append(str(self.map[state][symbol]))
-                else:
-                    row.append("")
+                row.append(str(self.map[state][symbol]))
             rows.append(row)
 
         # column widths
         colwidths = []
         for x in range(len(rows[0])):
-            colwidths.append(max(
-                len(str(rows[y][x])) for y in range(len(rows))
-            ) + 1)
+            colwidths.append(max(len(str(row[x])) for y, row in enumerate(rows)) + 1)
 
         # apply padding
-        for y in range(len(rows)):
-            for x in range(len(rows[y])):
-                rows[y][x] = rows[y][x].ljust(colwidths[x])
+        for y, row in enumerate(rows):
+            for x, col in enumerate(row):
+                rows[y][x] = col.ljust(colwidths[x])
 
         # horizontal line
         rows.insert(1, ["-" * colwidth for colwidth in colwidths])
 
         return "".join("".join(row) + "\n" for row in rows)
 
-    def concatenate(*fsms):
-        '''
-            Concatenate arbitrarily many finite state machines together.
-        '''
-        alphabet = set().union(*[fsm.alphabet for fsm in fsms])
-
-        def connect_all(i, substate):
-            '''
-                Take a state in the numbered FSM and return a set containing
-                it, plus (if it's final) the first state from the next FSM,
-                plus (if that's final) the first state from the next but one
-                FSM, plus...
-            '''
+    def concatenate(*fsms: Fsm) -> Fsm:
+        """
+        Concatenate arbitrarily many finite state machines together.
+        """
+        unified_fsms = unify_alphabets(fsms)
+
+        def connect_all(
+            i: int,
+            substate: StateType,
+        ) -> Iterable[tuple[int, StateType]]:
+            """
+            Take a state in the numbered FSM and return a set containing
+            it, plus (if it's final) the first state from the next FSM,
+            plus (if that's final) the first state from the next but one
+            FSM, plus...
+            """
             result = {(i, substate)}
-            while i < len(fsms) - 1 and substate in fsms[i].finals:
+            while i < len(unified_fsms) - 1 and substate in unified_fsms[i].finals:
                 i += 1
-                substate = fsms[i].initial
+                substate = unified_fsms[i].initial
                 result.add((i, substate))
             return result
 
         # Use a superset containing states from all FSMs at once.
         # We start at the start of the first FSM. If this state is final in the
         # first FSM, then we are also at the start of the second FSM. And so
         # on.
-        initial = set()
-        if len(fsms) > 0:
-            initial.update(connect_all(0, fsms[0].initial))
-        initial = frozenset(initial)
-
-        def final(state):
-            '''If you're in a final state of the final FSM, it's final'''
-            for (i, substate) in state:
-                if i == len(fsms) - 1 and substate in fsms[i].finals:
-                    return True
-            return False
-
-        def follow(current, symbol):
-            '''
-                Follow the collection of states through all FSMs at once,
-                jumping to the next FSM if we reach the end of the current one
-                TODO: improve all follow() implementations to allow for dead
-                metastates?
-            '''
-            next = set()
-            for (i, substate) in current:
-                fsm = fsms[i]
-                if substate in fsm.map:
-                    if symbol in fsm.map[substate]:
-                        next.update(connect_all(i, fsm.map[substate][symbol]))
-                    elif (
-                        ANYTHING_ELSE in fsm.map[substate]
-                        and symbol not in fsm.alphabet
-                    ):
-                        next.update(connect_all(
-                            i,
-                            fsm.map[substate][ANYTHING_ELSE]
-                        ))
-            if len(next) == 0:
-                raise OblivionError
-            return frozenset(next)
+        initial = frozenset(
+            connect_all(0, unified_fsms[0].initial) if unified_fsms else ()
+        )
+
+        def final(state: frozenset[tuple[int, StateType]]) -> bool:
+            """If you're in a final state of the final FSM, it's final"""
+            return any(
+                i == len(unified_fsms) - 1 and substate in unified_fsms[i].finals
+                for i, substate in state
+            )
+
+        def follow(
+            current: frozenset[tuple[int, StateType]],
+            symbol: AlphaType,
+        ) -> frozenset[tuple[int, StateType]]:
+            """
+            Follow the collection of states through all FSMs at once,
+            jumping to the next FSM if we reach the end of the current one
+            """
+            next_metastate: set[tuple[int, StateType]] = set()
+            for i, substate in current:
+                next_metastate.update(
+                    connect_all(i, unified_fsms[i].map[substate][symbol])
+                )
+
+            return frozenset(next_metastate)
+
+        alphabet = unified_fsms[0].alphabet if len(unified_fsms) > 0 else {~Charclass()}
 
         return crawl(alphabet, initial, final, follow).reduce()
 
-    def __add__(self, other):
-        '''
-            Concatenate two finite state machines together.
-            For example, if self accepts "0*" and other accepts "1+(0|1)",
-            will return a finite state machine accepting "0*1+(0|1)".
-            Accomplished by effectively following non-deterministically.
-            Call using "fsm3 = fsm1 + fsm2"
-        '''
+    def __add__(self, other: Fsm, /) -> Fsm:
+        """
+        Concatenate two finite state machines together.
+        For example, if self accepts "0*" and other accepts "1+(0|1)",
+        will return a finite state machine accepting "0*1+(0|1)".
+        Accomplished by effectively following non-deterministically.
+        Call using "fsm3 = fsm1 + fsm2"
+        """
         return self.concatenate(other)
 
-    def star(self):
-        '''
-            If the present FSM accepts X, returns an FSM accepting X* (i.e. 0
-            or more Xes). This is NOT as simple as naively connecting the final
-            states back to the initial state: see (b*ab)* for example.
-        '''
+    def star(self, /) -> Fsm:
+        """
+        If the present FSM accepts X, returns an FSM accepting X* (i.e. 0
+        or more Xes). This is NOT as simple as naively connecting the final
+        states back to the initial state: see (b*ab)* for example.
+        """
         alphabet = self.alphabet
 
-        initial = {self.initial}
+        initial: Collection[StateType] = {self.initial}
+
+        def follow(
+            state: Collection[StateType],
+            symbol: AlphaType,
+        ) -> Collection[StateType]:
+            next_states = set()
 
-        def follow(state, symbol):
-            next = set()
             for substate in state:
-                if substate in self.map and symbol in self.map[substate]:
-                    next.add(self.map[substate][symbol])
+                next_states.add(self.map[substate][symbol])
 
                 # If one of our substates is final, then we can also consider
                 # transitions from the initial state of the original FSM.
-                if substate in self.finals \
-                   and self.initial in self.map \
-                   and symbol in self.map[self.initial]:
-                    next.add(self.map[self.initial][symbol])
+                if substate in self.finals:
+                    next_states.add(self.map[self.initial][symbol])
 
-            if len(next) == 0:
-                raise OblivionError
+            return frozenset(next_states)
 
-            return frozenset(next)
-
-        def final(state):
+        def final(state: Collection[StateType]) -> bool:
             return any(substate in self.finals for substate in state)
 
-        return crawl(alphabet, initial, final, follow) | epsilon(alphabet)
+        return crawl(alphabet, initial, final, follow) | EPSILON
 
-    def times(self, multiplier):
-        '''
-            Given an FSM and a multiplier, return the multiplied FSM.
-        '''
+    def times(self, multiplier: int, /) -> Fsm:
+        """
+        Given an FSM and a multiplier, return the multiplied FSM.
+        """
         if multiplier < 0:
-            raise Exception(f"Can't multiply an FSM by {repr(multiplier)}")
+            raise ArithmeticError(f"Can't multiply an FSM by {multiplier!r}")
 
         alphabet = self.alphabet
 
         # metastate is a set of iterations+states
-        initial = {(self.initial, 0)}
+        initial: Collection[tuple[StateType, int]] = {(self.initial, 0)}
+
+        def final(state: Collection[tuple[StateType, int]]) -> bool:
+            """
+            If the initial state is final then multiplying doesn't alter
+            that
+            """
+            return any(
+                substate == self.initial
+                and (self.initial in self.finals or iteration == multiplier)
+                for substate, iteration in state
+            )
 
-        def final(state):
-            '''
-                If the initial state is final then multiplying doesn't alter
-                that
-            '''
-            for (substate, iteration) in state:
-                if substate == self.initial \
-                  and (
-                    self.initial in self.finals or
-                    iteration == multiplier
-                  ):
-                    return True
-            return False
-
-        def follow(current, symbol):
-            next = []
-            for (substate, iteration) in current:
-                if iteration < multiplier \
-                   and substate in self.map \
-                   and symbol in self.map[substate]:
-                    next.append((self.map[substate][symbol], iteration))
+        def follow(
+            current: Collection[tuple[StateType, int]],
+            symbol: AlphaType,
+        ) -> Collection[tuple[StateType, int]]:
+            next_metastate = []
+            for substate, iteration in current:
+                if iteration < multiplier:
+                    next_metastate.append((self.map[substate][symbol], iteration))
                     # final of self? merge with initial on next iteration
                     if self.map[substate][symbol] in self.finals:
-                        next.append((self.initial, iteration + 1))
-            if len(next) == 0:
-                raise OblivionError
-            return frozenset(next)
+                        next_metastate.append((self.initial, iteration + 1))
+            return frozenset(next_metastate)
 
         return crawl(alphabet, initial, final, follow).reduce()
 
-    def __mul__(self, multiplier):
-        '''
-            Given an FSM and a multiplier, return the multiplied FSM.
-        '''
+    def __mul__(self, multiplier: int, /) -> Fsm:
+        """
+        Given an FSM and a multiplier, return the multiplied FSM.
+        """
         return self.times(multiplier)
 
-    def union(*fsms):
-        '''
-            Treat `fsms` as a collection of arbitrary FSMs and return the union
-            FSM. Can be used as `fsm1.union(fsm2, ...)` or
-            `fsm.union(fsm1, ...)`. `fsms` may be empty.
-        '''
+    def union(*fsms: Fsm) -> Fsm:
+        """
+        Treat `fsms` as a collection of arbitrary FSMs and return the union
+        FSM. Can be used as `fsm1.union(fsm2, ...)` or
+        `fsm.union(fsm1, ...)`. `fsms` may be empty.
+        """
         return parallel(fsms, any)
 
-    def __or__(self, other):
-        '''
-            Alternation.
-            Return a finite state machine which accepts any sequence of symbols
-            that is accepted by either self or other. Note that the set of
-            strings recognised by the two FSMs undergoes a set union.
-            Call using "fsm3 = fsm1 | fsm2"
-        '''
+    def __or__(self, other: Fsm, /) -> Fsm:
+        """
+        Alternation.
+        Return a finite state machine which accepts any sequence of symbols
+        that is accepted by either self or other. Note that the set of
+        strings recognised by the two FSMs undergoes a set union.
+        Call using "fsm3 = fsm1 | fsm2"
+        """
         return self.union(other)
 
-    def intersection(*fsms):
-        '''
-            Intersection.
-            Take FSMs and AND them together. That is, return an FSM which
-            accepts any sequence of symbols that is accepted by both of the
-            original FSMs. Note that the set of strings recognised by the two
-            FSMs undergoes a set intersection operation.
-            Call using "fsm3 = fsm1 & fsm2"
-        '''
+    def intersection(*fsms: Fsm) -> Fsm:
+        """
+        Intersection.
+        Take FSMs and AND them together. That is, return an FSM which
+        accepts any sequence of symbols that is accepted by both of the
+        original FSMs. Note that the set of strings recognised by the two
+        FSMs undergoes a set intersection operation.
+        Call using "fsm3 = fsm1 & fsm2"
+        """
         return parallel(fsms, all)
 
-    def __and__(self, other):
-        '''
-            Treat the FSMs as sets of strings and return the intersection of
-            those sets in the form of a new FSM.
-        '''
+    def __and__(self, other: Fsm, /) -> Fsm:
+        """
+        Treat the FSMs as sets of strings and return the intersection of
+        those sets in the form of a new FSM.
+        """
         return self.intersection(other)
 
-    def symmetric_difference(*fsms):
-        '''
-            Treat `fsms` as a collection of sets of strings and compute the
-            symmetric difference of them all. The python set method only allows
-            two sets to be operated on at once, but we go the extra mile since
-            it's not too hard.
-        '''
+    def symmetric_difference(*fsms: Fsm) -> Fsm:
+        """
+        Treat `fsms` as a collection of sets of strings and compute the
+        symmetric difference of them all. The python set method only allows
+        two sets to be operated on at once, but we go the extra mile since
+        it's not too hard.
+        """
         return parallel(fsms, lambda accepts: (accepts.count(True) % 2) == 1)
 
-    def __xor__(self, other):
-        '''
-            Symmetric difference. Returns an FSM which recognises only the
-            strings recognised by `self` or `other` but not both.
-        '''
+    def __xor__(self, other: Fsm, /) -> Fsm:
+        """
+        Symmetric difference. Returns an FSM which recognises only the
+        strings recognised by `self` or `other` but not both.
+        """
         return self.symmetric_difference(other)
 
-    def everythingbut(self):
-        '''
-            Return a finite state machine which will accept any string NOT
-            accepted by self, and will not accept any string accepted by self.
-            This is more complicated if there are missing transitions, because
-            the missing "dead" state must now be reified.
-        '''
+    def everythingbut(self, /) -> Fsm:
+        """
+        Return a finite state machine which will accept any string NOT
+        accepted by self, and will not accept any string accepted by self.
+        """
         alphabet = self.alphabet
+        initial = self.initial
 
-        initial = {0: self.initial}
-
-        def follow(current, symbol):
-            next = {}
-            if 0 in current \
-               and current[0] in self.map \
-               and symbol in self.map[current[0]]:
-                next[0] = self.map[current[0]][symbol]
-            return next
+        def follow(
+            current: StateType,
+            symbol: AlphaType,
+        ) -> StateType:
+            return self.map[current][symbol]
 
         # state is final unless the original was
-        def final(state):
-            return not (0 in state and state[0] in self.finals)
+        def final(state: StateType) -> bool:
+            return state not in self.finals
 
         return crawl(alphabet, initial, final, follow).reduce()
 
-    def reversed(self):
-        '''
-            Return a new FSM such that for every string that self accepts (e.g.
-            "beer", the new FSM accepts the reversed string ("reeb").
-        '''
+    def reversed(self, /) -> Fsm:
+        """
+        Return a new FSM such that for every string that self accepts (e.g.
+        "beer", the new FSM accepts the reversed string ("reeb").
+        """
         alphabet = self.alphabet
 
         # Start from a composite "state-set" consisting of all final states.
         # If there are no final states, this set is empty and we'll find that
         # no other states get generated.
         initial = frozenset(self.finals)
 
         # Find every possible way to reach the current state-set
         # using this symbol.
-        def follow(current, symbol):
-            next = frozenset([
-                prev
-                for prev in self.map
-                for state in current
-                if symbol in self.map[prev] and self.map[prev][symbol] == state
-            ])
-            if len(next) == 0:
-                raise OblivionError
-            return next
+        def follow(
+            current: frozenset[StateType],
+            symbol: AlphaType,
+        ) -> frozenset[StateType]:
+            next_states = frozenset(
+                [
+                    prev
+                    for prev in self.map
+                    for state in current
+                    if self.map[prev][symbol] == state
+                ]
+            )
+            return next_states
 
         # A state-set is final if the initial state is in it.
-        def final(state):
+        def final(state: frozenset[StateType]) -> bool:
             return self.initial in state
 
         # Man, crawl() is the best!
         return crawl(alphabet, initial, final, follow)
         # Do not reduce() the result, since reduce() calls us in turn
 
-    def __reversed__(self):
-        '''
-            Return a new FSM such that for every string that self accepts (e.g.
-            "beer", the new FSM accepts the reversed string ("reeb").
-        '''
-        return self.reversed()
-
-    def islive(self, state):
-        '''A state is "live" if a final state can be reached from it.'''
+    def islive(self, /, state: StateType) -> bool:
+        """A state is "live" if a final state can be reached from it."""
         reachable = [state]
         i = 0
         while i < len(reachable):
             current = reachable[i]
             if current in self.finals:
                 return True
-            if current in self.map:
-                for symbol in self.map[current]:
-                    next = self.map[current][symbol]
-                    if next not in reachable:
-                        reachable.append(next)
+            for symbol in self.map[current]:
+                next_state = self.map[current][symbol]
+                if next_state not in reachable:
+                    reachable.append(next_state)
             i += 1
         return False
 
-    def empty(self):
-        '''
-            An FSM is empty if it recognises no strings. An FSM may be
-            arbitrarily complicated and have arbitrarily many final states
-            while still recognising no strings because those final states may
-            all be inaccessible from the initial state. Equally, an FSM may be
-            non-empty despite having an empty alphabet if the initial state is
-            final.
-        '''
+    def empty(self, /) -> bool:
+        """
+        An FSM is empty if it recognises no strings. An FSM may be
+        arbitrarily complicated and have arbitrarily many final states
+        while still recognising no strings because those final states may
+        all be inaccessible from the initial state. Equally, an FSM may be
+        non-empty despite having an empty alphabet if the initial state is
+        final.
+        """
         return not self.islive(self.initial)
 
-    def strings(self):
-        '''
-            Generate strings (lists of symbols) that this FSM accepts. Since
-            there may be infinitely many of these we use a generator instead of
-            constructing a static list. Strings will be sorted in order of
-            length and then lexically. This procedure uses arbitrary amounts of
-            memory but is very fast. There may be more efficient ways to do
-            this, that I haven't investigated yet. You can use this in list
-            comprehensions.
-        '''
+    def strings(self, otherchars: Iterable[str]) -> Iterator[str]:
+        """
+        Generate strings that this FSM accepts. Note that for our purposes a
+        string is a sequence of Unicode characters, NOT a list of Charclasses.
+
+        Since
+        there may be infinitely many of these we use a generator instead of
+        constructing a static list. Strings will be sorted in order of
+        length and then lexically. This procedure uses arbitrary amounts of
+        memory but is very fast. There may be more efficient ways to do
+        this, that I haven't investigated yet. You can use this in list
+        comprehensions.
+        """
 
-        # Many FSMs have "dead states". Once you reach a dead state, you can no
+        # Most FSMs have at least one "dead state".
+        # Once you reach a dead state, you can no
         # longer reach a final state. Since many strings may end up here, it's
         # advantageous to constrain our search to live states only.
         livestates = set(state for state in self.states if self.islive(state))
 
         # We store a list of tuples. Each tuple consists of an input string and
         # the state that this input string leads to. This means we don't have
         # to run the state machine from the very beginning every time we want
         # to check a new string.
-        strings = []
+        strings: list[tuple[str, StateType]] = []
 
         # Initial entry (or possibly not, in which case this is a short one)
-        cstate = self.initial
-        cstring = []
+        cstate: StateType = self.initial
+        cstring: str = ""
         if cstate in livestates:
             if cstate in self.finals:
                 yield cstring
             strings.append((cstring, cstate))
 
         # Fixed point calculation
         i = 0
         while i < len(strings):
-            (cstring, cstate) = strings[i]
-            if cstate in self.map:
-                for symbol in sorted(self.map[cstate], key=alphabet_key):
-                    nstate = self.map[cstate][symbol]
-                    nstring = cstring + [symbol]
+            cstring, cstate = strings[i]
+
+            for charclass in sorted(self.map[cstate]):
+                # TODO: scrap otherchars as a concept?
+                chars = otherchars if charclass.negated else charclass.get_chars()
+                for char in chars:
+                    nstate = self.map[cstate][charclass]
+                    nstring = cstring + char
                     if nstate in livestates:
                         if nstate in self.finals:
                             yield nstring
                         strings.append((nstring, nstate))
             i += 1
 
-    def __iter__(self):
-        '''
-            This allows you to do `for string in fsm1` as a list comprehension!
-        '''
-        return self.strings()
-
-    def equivalent(self, other):
-        '''
-            Two FSMs are considered equivalent if they recognise the same
-            strings. Or, to put it another way, if their symmetric difference
-            recognises no strings.
-        '''
+    def __iter__(self, /) -> Iterator[str]:
+        """
+        This allows you to do `for string in fsm1` as a list comprehension!
+        """
+        return self.strings([])
+
+    def equivalent(self, other: Fsm, /) -> bool:
+        """
+        Two FSMs are considered equivalent if they recognise the same
+        strings. Or, to put it another way, if their symmetric difference
+        recognises no strings.
+        """
         return (self ^ other).empty()
 
-    def __eq__(self, other):
-        '''
-            You can use `fsm1 == fsm2` to determine whether two FSMs recognise
-            the same strings.
-        '''
+    def __eq__(self, other: object, /) -> bool:
+        """
+        You can use `fsm1 == fsm2` to determine whether two FSMs recognise
+        the same strings.
+        """
+        if not isinstance(other, Fsm):
+            return NotImplemented
         return self.equivalent(other)
 
-    def different(self, other):
-        '''
-            Two FSMs are considered different if they have a non-empty
-            symmetric difference.
-        '''
+    def different(self, other: Fsm, /) -> bool:
+        """
+        Two FSMs are considered different if they have a non-empty
+        symmetric difference.
+        """
         return not (self ^ other).empty()
 
-    def __ne__(self, other):
-        '''
-            Use `fsm1 != fsm2` to determine whether two FSMs recognise
-            different strings.
-        '''
-        return self.different(other)
-
-    def difference(*fsms):
-        '''
-            Difference. Returns an FSM which recognises only the strings
-            recognised by the first FSM in the list, but none of the others.
-        '''
-        return parallel(
-            fsms,
-            lambda accepts: accepts[0] and not any(accepts[1:])
-        )
+    def __ne__(self, other: object, /) -> bool:
+        """
+        Use `fsm1 != fsm2` to determine whether two FSMs recognise
+        different strings.
+        """
+        return not self == other
+
+    def difference(*fsms: Fsm) -> Fsm:
+        """
+        Difference. Returns an FSM which recognises only the strings
+        recognised by the first FSM in the list, but none of the others.
+        """
+        return parallel(fsms, lambda accepts: accepts[0] and not any(accepts[1:]))
 
-    def __sub__(self, other):
+    def __sub__(self, other: Fsm, /) -> Fsm:
         return self.difference(other)
 
-    def cardinality(self):
-        '''
-            Consider the FSM as a set of strings and return the cardinality of
-            that set, or raise an OverflowError if there are infinitely many
-        '''
-        num_strings = {}
+    def cardinality(self, /) -> int:
+        """
+        Consider the FSM as a set of strings and return the cardinality of
+        that set, or raise an OverflowError if there are infinitely many
+        """
+        num_strings: dict[StateType, int | None] = {}
 
-        def get_num_strings(state):
-            # Many FSMs have at least one oblivion state
+        def get_num_strings(state: StateType) -> int:
+            # Most FSMs have at least one oblivion state
             if self.islive(state):
                 if state in num_strings:
                     if num_strings[state] is None:  # "computing..."
                         # Recursion! There are infinitely many strings
                         # recognised
                         raise OverflowError(state)
-                    return num_strings[state]
-                num_strings[state] = None  # i.e. "computing..."
+                    return num_strings[state]  # type: ignore
 
+                num_strings[state] = None  # i.e. "computing..."
                 n = 0
-                if state in self.finals:
-                    n += 1
-                if state in self.map:
-                    for symbol in self.map[state]:
-                        n += get_num_strings(self.map[state][symbol])
+                for charclass in self.map[state]:
+                    num_transitions = charclass.num_chars()
+                    nstate = self.map[state][charclass]
+                    if nstate in self.finals:
+                        n += num_transitions
+                    n += num_transitions * get_num_strings(nstate)
                 num_strings[state] = n
 
             else:
                 # Dead state
                 num_strings[state] = 0
 
-            return num_strings[state]
+            return num_strings[state]  # type: ignore
 
-        return get_num_strings(self.initial)
+        n = 1 if self.initial in self.finals else 0
+        return n + get_num_strings(self.initial)
 
-    def __len__(self):
-        '''
-            Consider the FSM as a set of strings and return the cardinality of
-            that set, or raise an OverflowError if there are infinitely many
-        '''
+    def __len__(self, /) -> int:
+        """
+        Consider the FSM as a set of strings and return the cardinality of
+        that set, or raise an OverflowError if there are infinitely many
+        """
         return self.cardinality()
 
-    def isdisjoint(self, other):
-        '''
-            Treat `self` and `other` as sets of strings and see if they are
-            disjoint
-        '''
+    def isdisjoint(self, other: Fsm, /) -> bool:
+        """
+        Treat `self` and `other` as sets of strings and see if they are
+        disjoint
+        """
         return (self & other).empty()
 
-    def issubset(self, other):
-        '''
-            Treat `self` and `other` as sets of strings and see if `self` is a
-            subset of `other`... `self` recognises no strings which `other`
-            doesn't.
-        '''
+    def issubset(self, other: Fsm, /) -> bool:
+        """
+        Treat `self` and `other` as sets of strings and see if `self` is a
+        subset of `other`... `self` recognises no strings which `other`
+        doesn't.
+        """
         return (self - other).empty()
 
-    def __le__(self, other):
-        '''
-            Treat `self` and `other` as sets of strings and see if `self` is a
-            subset of `other`... `self` recognises no strings which `other`
-            doesn't.
-        '''
+    def __le__(self, other: Fsm, /) -> bool:
+        """
+        Treat `self` and `other` as sets of strings and see if `self` is a
+        subset of `other`... `self` recognises no strings which `other`
+        doesn't.
+        """
         return self.issubset(other)
 
-    def ispropersubset(self, other):
-        '''
-            Treat `self` and `other` as sets of strings and see if `self` is a
-            proper subset of `other`.
-        '''
+    def ispropersubset(self, other: Fsm, /) -> bool:
+        """
+        Treat `self` and `other` as sets of strings and see if `self` is a
+        proper subset of `other`.
+        """
         return self <= other and self != other
 
-    def __lt__(self, other):
-        '''
-            Treat `self` and `other` as sets of strings and see if `self` is a
-            strict subset of `other`.
-        '''
+    def __lt__(self, other: Fsm, /) -> bool:
+        """
+        Treat `self` and `other` as sets of strings and see if `self` is a
+        strict subset of `other`.
+        """
         return self.ispropersubset(other)
 
-    def issuperset(self, other):
-        '''
-            Treat `self` and `other` as sets of strings and see if `self` is a
-            superset of `other`.
-        '''
+    def issuperset(self, other: Fsm, /) -> bool:
+        """
+        Treat `self` and `other` as sets of strings and see if `self` is a
+        superset of `other`.
+        """
         return (other - self).empty()
 
-    def __ge__(self, other):
-        '''
-            Treat `self` and `other` as sets of strings and see if `self` is a
-            superset of `other`.
-        '''
+    def __ge__(self, other: Fsm, /) -> bool:
+        """
+        Treat `self` and `other` as sets of strings and see if `self` is a
+        superset of `other`.
+        """
         return self.issuperset(other)
 
-    def ispropersuperset(self, other):
-        '''
-            Treat `self` and `other` as sets of strings and see if `self` is a
-            proper superset of `other`.
-        '''
+    def ispropersuperset(self, other: Fsm, /) -> bool:
+        """
+        Treat `self` and `other` as sets of strings and see if `self` is a
+        proper superset of `other`.
+        """
         return self >= other and self != other
 
-    def __gt__(self, other):
-        '''
-            Treat `self` and `other` as sets of strings and see if `self` is a
-            strict superset of `other`.
-        '''
+    def __gt__(self, other: Fsm, /) -> bool:
+        """
+        Treat `self` and `other` as sets of strings and see if `self` is a
+        strict superset of `other`.
+        """
         return self.ispropersuperset(other)
 
-    def copy(self):
-        '''
-            For completeness only, since `set.copy()` also exists. FSM objects
-            are immutable, so I can see only very odd reasons to need this.
-        '''
+    def copy(self, /) -> Fsm:
+        """
+        For completeness only, since `set.copy()` and `frozenset.copy()` exist.
+        FSM objects are immutable; like `frozenset`, this just returns `self`.
+        """
+        return self
+
+    __copy__ = copy
+
+    def derive(self, string: str, /) -> Fsm:
+        """
+        Compute the Brzozowski derivative of this FSM with respect to the
+        input string. Note that the FSM uses Charclasses as symbols internally,
+        but the input string is a sequence of Unicode characters
+        <https://en.wikipedia.org/wiki/Brzozowski_derivative>
+        """
+        # Consume the input string.
+        state = self.initial
+        for char in string:
+            for charclass in self.map[state]:
+                if charclass.accepts(char):
+                    state = self.map[state][charclass]
+                    break
+
+        # OK so now we have consumed that string, use the new location as
+        # the starting point.
         return Fsm(
             alphabet=self.alphabet,
             states=self.states,
-            initial=self.initial,
+            initial=state,
             finals=self.finals,
             map=self.map,
         )
 
-    def derive(self, input):
-        '''
-            Compute the Brzozowski derivative of this FSM with respect to the
-            input string of symbols.
-            <https://en.wikipedia.org/wiki/Brzozowski_derivative>
-            If any of the symbols are not members of the alphabet, that's a
-            `KeyError`. If you fall into oblivion, then the derivative is an
-            FSM accepting no strings.
-        '''
-        try:
-            # Consume the input string.
-            state = self.initial
-            for symbol in input:
-                if symbol not in self.alphabet:
-                    if ANYTHING_ELSE not in self.alphabet:
-                        raise KeyError(symbol)
-                    symbol = ANYTHING_ELSE
-
-                # Missing transition = transition to dead state
-                if not (state in self.map and symbol in self.map[state]):
-                    raise OblivionError
-
-                state = self.map[state][symbol]
-
-            # OK so now we have consumed that string, use the new location as
-            # the starting point.
-            return Fsm(
-                alphabet=self.alphabet,
-                states=self.states,
-                initial=state,
-                finals=self.finals,
-                map=self.map,
-            )
-
-        except OblivionError:
-            # Fell out of the FSM. The derivative of this FSM is the empty FSM.
-            return null(self.alphabet)
-
-
-def null(alphabet):
-    '''
-        An FSM accepting nothing (not even the empty string). This is
-        demonstrates that this is possible, and is also extremely useful
-        in some situations
-    '''
-    return Fsm(
-        alphabet=alphabet,
-        states={0},
-        initial=0,
-        finals=set(),
-        map={
-            0: dict([(symbol, 0) for symbol in alphabet]),
-        },
-    )
-
-
-def epsilon(alphabet):
-    '''
-        Return an FSM matching an empty string, "", only.
-        This is very useful in many situations
-    '''
-    return Fsm(
-        alphabet=alphabet,
-        states={0},
-        initial=0,
-        finals={0},
-        map={},
-    )
+    def replace_alphabet(
+        self, replacements: Mapping[AlphaType, Iterable[AlphaType]]
+    ) -> Fsm:
+        """
+        Returns a new FSM which uses a different alphabet. If one original
+        symbol converts to two new symbols, there will be multiple identical
+        transitions; if none, the transitions will be omitted.
+        """
+        new_alphabet = set()
+        for symbol in self.alphabet:
+            for replacement in replacements[symbol]:
+                new_alphabet.add(replacement)
+
+        new_map: Dict[StateType, Dict[AlphaType, StateType]] = {}
+        for state in self.map:
+            new_map[state] = {}
+            for symbol in self.alphabet:
+                for replacement in replacements[symbol]:
+                    new_map[state][replacement] = self.map[state][symbol]
 
+        return Fsm(
+            alphabet=new_alphabet,
+            states=self.states,
+            initial=self.initial,
+            finals=self.finals,
+            map=new_map,
+        )
 
-def parallel(fsms, test):
-    '''
-        Crawl several FSMs in parallel, mapping the states of a larger
-        meta-FSM. To determine whether a state in the larger FSM is final, pass
-        all of the finality statuses (e.g. [True, False, False] to `test`.
-    '''
-    alphabet = set().union(*[fsm.alphabet for fsm in fsms])
 
-    initial = dict([(i, fsm.initial) for (i, fsm) in enumerate(fsms)])
+NULL = Fsm(
+    alphabet={~Charclass()},
+    states={0},
+    initial=0,
+    finals=(),
+    map={
+        0: {~Charclass(): 0},
+    },
+)
+"""
+An FSM accepting nothing (not even the empty string). This is
+demonstrates that this is possible, and is also extremely useful
+in some situations
+"""
+
+EPSILON = Fsm(
+    alphabet={~Charclass()},
+    states={0, 1},
+    initial=0,
+    finals={0},
+    map={
+        0: {~Charclass(): 1},
+        1: {~Charclass(): 1},
+    },
+)
+"""
+An FSM matching an empty string, "", only.
+This is very useful in many situations
+"""
+
+
+def parallel(
+    fsms: tuple[Fsm, ...],
+    test: Callable[[list[bool]], bool],
+    /,
+) -> Fsm:
+    """
+    Crawl several FSMs in parallel, mapping the states of a larger
+    meta-FSM. To determine whether a state in the larger FSM is final, pass
+    all of the finality statuses (e.g. [True, False, False] to `test`.
+    """
+    unified_fsms = unify_alphabets(fsms)
+
+    initial: Mapping[int, StateType] = {
+        i: fsm.initial for i, fsm in enumerate(unified_fsms)
+    }
 
     # dedicated function accepts a "superset" and returns the next "superset"
     # obtained by following this transition in the new FSM
-    def follow(current, symbol):
-        next = {}
-        for i in range(len(fsms)):
-            if symbol not in fsms[i].alphabet \
-               and ANYTHING_ELSE in fsms[i].alphabet:
-                actual_symbol = ANYTHING_ELSE
-            else:
-                actual_symbol = symbol
-            if i in current \
-               and current[i] in fsms[i].map \
-               and actual_symbol in fsms[i].map[current[i]]:
-                next[i] = fsms[i].map[current[i]][actual_symbol]
-        if len(next.keys()) == 0:
-            raise OblivionError
-        return next
+    def follow(
+        current: Mapping[int, StateType],
+        symbol: AlphaType,
+    ) -> Mapping[int, StateType]:
+        return {i: fsm.map[current[i]][symbol] for i, fsm in enumerate(unified_fsms)}
 
     # Determine the "is final?" condition of each substate, then pass it to the
     # test to determine finality of the overall FSM.
-    def final(state):
-        accepts = [
-            i in state and state[i] in fsm.finals
-            for (i, fsm) in enumerate(fsms)
-        ]
-        return test(accepts)
+    def final(state: Mapping[int, StateType]) -> bool:
+        return test([state[i] in fsm.finals for i, fsm in enumerate(unified_fsms)])
+
+    alphabet = unified_fsms[0].alphabet if len(unified_fsms) > 0 else {~Charclass()}
 
     return crawl(alphabet, initial, final, follow).reduce()
 
 
-def crawl(alphabet, initial, final, follow):
-    '''
-        Given the above conditions and instructions, crawl a new unknown FSM,
-        mapping its states, final states and transitions. Return the new FSM.
-        This is a pretty powerful procedure which could potentially go on
-        forever if you supply an evil version of follow().
-    '''
-
-    states = [initial]
-    finals = set()
-    map = {}
+def crawl(
+    alphabet: Iterable[AlphaType],
+    initial: M,
+    final: Callable[[M], bool],
+    follow: Callable[[M, AlphaType], M],
+) -> Fsm:
+    """
+    Given the above conditions and instructions, crawl a new unknown FSM,
+    mapping its states, final states and transitions. Return the new FSM.
+    This is a pretty powerful procedure which could potentially go on
+    forever if you supply an evil version of follow().
+    """
+
+    states: list[M] = [initial]
+    finals: set[StateType] = set()
+    transitions: dict[StateType, dict[AlphaType, StateType]] = {}
 
     # iterate over a growing list
     i = 0
     while i < len(states):
         state = states[i]
 
         # add to finals
         if final(state):
             finals.add(i)
 
         # compute map for this state
-        map[i] = {}
-        for symbol in sorted(alphabet, key=alphabet_key):
-            try:
-                next = follow(state, symbol)
+        transitions[i] = {}
+        for symbol in sorted(alphabet):
+            next_state = follow(state, symbol)
 
-                try:
-                    j = states.index(next)
-                except ValueError:
-                    j = len(states)
-                    states.append(next)
-
-            except OblivionError:
-                # Reached an oblivion state. Don't list it.
-                continue
+            try:
+                j = states.index(next_state)
+            except ValueError:
+                j = len(states)
+                states.append(next_state)
 
-            map[i][symbol] = j
+            transitions[i][symbol] = j
 
         i += 1
 
     return Fsm(
         alphabet=alphabet,
         states=set(range(len(states))),
         initial=0,
         finals=finals,
-        map=map,
+        map=transitions,
+    )
+
+
+def from_charclass(charclass: Charclass) -> Fsm:
+    # 0 is initial, 1 is final, 2 is dead
+    return Fsm(
+        alphabet={charclass, ~charclass},
+        states={0, 1, 2},
+        initial=0,
+        finals={1},
+        map={
+            0: {charclass: 1, ~charclass: 2},
+            1: {charclass: 2, ~charclass: 2},
+            2: {charclass: 2, ~charclass: 2},
+        },
     )
```

### Comparing `greenery-4.0.0/greenery/mult_test.py` & `greenery-4.1.0/greenery/mult_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
-from .fsm import ANYTHING_ELSE
-from .charclass import Charclass, DIGIT
-from .bound import Bound, INF
-from .multiplier import Multiplier, ONE, QM, STAR, PLUS
+from .bound import INF, Bound
+from .charclass import DIGIT, Charclass
+from .multiplier import ONE, PLUS, QM, STAR, Multiplier
 from .rxelems import Mult
 
 
-def test_mult_equality():
+def test_mult_equality() -> None:
     a = Mult(Charclass("a"), ONE)
+    # pylint: disable=comparison-with-itself
     assert a == a
     assert a != Mult(Charclass("b"), ONE)
     assert a != Mult(Charclass("a"), QM)
-    assert a != Mult(
-        Charclass("a"),
-        Multiplier(Bound(1), Bound(2))
-    )
+    assert a != Mult(Charclass("a"), Multiplier(Bound(1), Bound(2)))
 
 
-def test_mult_str():
+def test_mult_str() -> None:
     a = Charclass("a")
     assert str(Mult(a, ONE)) == "a"
     assert str(Mult(a, Multiplier(Bound(2), Bound(2)))) == "a{2}"
     assert str(Mult(a, Multiplier(Bound(3), Bound(3)))) == "a{3}"
     assert str(Mult(a, Multiplier(Bound(4), Bound(4)))) == "a{4}"
     assert str(Mult(a, Multiplier(Bound(5), Bound(5)))) == "a{5}"
     assert str(Mult(a, QM)) == "a?"
@@ -32,46 +29,45 @@
     assert str(Mult(a, Multiplier(Bound(2), INF))) == "a{2,}"
 
     assert str(Mult(DIGIT, ONE)) == "\\d"
     assert str(Mult(DIGIT, Multiplier(Bound(2), Bound(2)))) == "\\d{2}"
     assert str(Mult(DIGIT, Multiplier(Bound(3), Bound(3)))) == "\\d{3}"
 
 
-def test_odd_bug():
+def test_odd_bug() -> None:
+    # pylint: disable=invalid-name
+
     # Odd bug with ([bc]*c)?[ab]*
     int5A = Mult(
         Charclass("bc"),
         STAR,
-    ).to_fsm({"a", "b", "c", ANYTHING_ELSE})
-    assert int5A.accepts([])
+    ).to_fsm()
     assert int5A.accepts("")
 
     int5B = Mult(
         Charclass("c"),
         ONE,
-    ).to_fsm({"a", "b", "c", ANYTHING_ELSE})
+    ).to_fsm()
     assert int5B.accepts("c")
-    assert int5B.accepts(["c"])
 
-    int5C = int5A + int5B
+    int5C = int5A.concatenate(int5B)
     assert int5C.accepts("c")
-    assert int5C.accepts(["c"])
 
 
-def test_mult_common():
+def test_mult_common() -> None:
     a = Charclass("a")
-    assert Mult(a, Multiplier(Bound(3), Bound(4))) \
-        .common(Mult(a, Multiplier(Bound(2), Bound(5)))) == \
-        Mult(a, Multiplier(Bound(2), Bound(3)))
-    assert Mult(a, Multiplier(Bound(2), INF)) \
-        .common(Mult(a, Multiplier(Bound(1), Bound(5)))) == \
+    assert Mult(a, Multiplier(Bound(3), Bound(4))).common(
+        Mult(a, Multiplier(Bound(2), Bound(5)))
+    ) == Mult(a, Multiplier(Bound(2), Bound(3)))
+    assert Mult(a, Multiplier(Bound(2), INF)).common(
         Mult(a, Multiplier(Bound(1), Bound(5)))
-    assert Mult(a, Multiplier(Bound(3), INF)) \
-        .common(Mult(a, Multiplier(Bound(2), INF))) == \
+    ) == Mult(a, Multiplier(Bound(1), Bound(5)))
+    assert Mult(a, Multiplier(Bound(3), INF)).common(
         Mult(a, Multiplier(Bound(2), INF))
+    ) == Mult(a, Multiplier(Bound(2), INF))
 
 
-def test_mult_dock():
+def test_mult_dock() -> None:
     a = Charclass("a")
-    assert Mult(a, Multiplier(Bound(4), Bound(5))) \
-        .dock(Mult(a, Multiplier(Bound(3), Bound(3)))) == \
-        Mult(a, Multiplier(Bound(1), Bound(2)))
+    assert Mult(a, Multiplier(Bound(4), Bound(5))).dock(
+        Mult(a, Multiplier(Bound(3), Bound(3)))
+    ) == Mult(a, Multiplier(Bound(1), Bound(2)))
```

### Comparing `greenery-4.0.0/greenery/multiplier.py` & `greenery-4.1.0/greenery/multiplier.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,183 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+__all__ = (
+    "Multiplier",
+    "ONE",
+    "PLUS",
+    "QM",
+    "STAR",
+    "ZERO",
+    "symbolic",
+)
 
 from dataclasses import dataclass, field
+from typing import Mapping
 
-from .bound import Bound, INF
+from .bound import INF, Bound
 
 
 @dataclass(frozen=True)
 class Multiplier:
-    '''
-        A min and a max. The vast majority of characters in regular expressions
-        occur without a specific multiplier, which is implicitly equivalent to
-        a min of 1 and a max of 1, but many more have explicit multipliers like
-        "*" (min = 0, max = inf) and so on.
-
-        Although it seems odd and can lead to some confusing edge cases, we do
-        also permit a max of 0 (iff min is 0 too). This allows the multiplier
-        `ZERO` to exist, which actually are quite useful in their own special
-        way.
-    '''
+    """
+    A min and a max. The vast majority of characters in regular expressions
+    occur without a specific multiplier, which is implicitly equivalent to
+    a min of 1 and a max of 1, but many more have explicit multipliers like
+    "*" (min = 0, max = inf) and so on.
+
+    Although it seems odd and can lead to some confusing edge cases, we do
+    also permit a max of 0 (iff min is 0 too). This allows the multiplier
+    `ZERO` to exist, which actually are quite useful in their own special
+    way.
+    """
+
     min: Bound
     max: Bound
     mandatory: Bound = field(init=False)
     optional: Bound = field(init=False)
 
-    def __post_init__(self):
+    def __post_init__(self, /) -> None:
         if self.min == INF:
-            raise Exception(
-                f"Minimum bound of a multiplier can't be {repr(INF)}"
-            )
+            raise ValueError(f"Minimum bound of a multiplier can't be {INF!r}")
         if self.min > self.max:
-            raise Exception(
-                "Invalid multiplier bounds: "
-                f"{repr(self.min)} and {repr(self.max)}"
+            raise ValueError(
+                f"Invalid multiplier bounds: {self.min!r} and {self.max!r}"
             )
 
         # More useful than "min" and "max" in many situations
         # are "mandatory" and "optional".
         object.__setattr__(self, "mandatory", self.min)
         object.__setattr__(self, "optional", self.max - self.min)
 
-    def __eq__(self, other):
+    def __eq__(self, other: object, /) -> bool:
+        if not isinstance(other, type(self)):
+            return NotImplemented
         return self.min == other.min and self.max == other.max
 
-    def __hash__(self):
+    def __hash__(self, /) -> int:
         return hash((self.min, self.max))
 
-    def __repr__(self):
-        return f"Multiplier({repr(self.min)}, {repr(self.max)})"
+    def __repr__(self, /) -> str:
+        return f"Multiplier({self.min!r}, {self.max!r})"
 
-    def __str__(self):
-        if self.max == Bound(0):
-            raise Exception(
-                f"Can't serialise a multiplier with bound {repr(self.max)}"
-            )
-        if self in symbolic.keys():
+    def __str__(self, /) -> str:
+        try:
             return symbolic[self]
+        except LookupError:
+            pass
+
         if self.min == self.max:
             return "{" + str(self.min) + "}"
         return "{" + str(self.min) + "," + str(self.max) + "}"
 
-    def canmultiplyby(self, other):
-        '''
-            Multiplication is not well-defined for all pairs of multipliers
-            because the resulting possibilities do not necessarily form a
-            continuous range.
-
-            For example:
-                {0,x} * {0,y} = {0,x*y}
-                {2} * {3} = {6}
-                {2} * {1,2} = ERROR
-
-            The proof isn't simple but suffice it to say that {p,p+q} * {r,r+s}
-            is equal to {pr, (p+q)(r+s)} only if s=0 or qr+1 >= p. If not, then
-            at least one gap appears in the range. The first inaccessible
-            number is (p+q)r+1. And no, multiplication is not commutative
-        '''
-        return other.optional == Bound(0) or \
-            self.optional * other.mandatory + Bound(1) >= self.mandatory
+    def canmultiplyby(self, other: Multiplier, /) -> bool:
+        """
+        Multiplication is not well-defined for all pairs of multipliers
+        because the resulting possibilities do not necessarily form a
+        continuous range.
+
+        For example:
+            {0,x} * {0,y} = {0,x*y}
+            {2} * {3} = {6}
+            {2} * {1,2} = ERROR
+
+        The proof isn't simple but suffice it to say that {p,p+q} * {r,r+s}
+        is equal to {pr, (p+q)(r+s)} only if s=0 or qr+1 >= p. If not, then
+        at least one gap appears in the range. The first inaccessible
+        number is (p+q)r+1. And no, multiplication is not commutative
+        """
+        return (
+            other.optional == Bound(0)
+            or self.optional * other.mandatory + Bound(1) >= self.mandatory
+        )
 
-    def __mul__(self, other):
-        '''Multiply this multiplier by another'''
+    def __mul__(self, other: Multiplier, /) -> Multiplier:
+        """Multiply this multiplier by another"""
         if not self.canmultiplyby(other):
-            raise Exception(
-                f"Can't multiply {repr(self)} by {repr(other)}"
-            )
+            raise ArithmeticError(f"Can't multiply {self!r} by {other!r}")
         return Multiplier(self.min * other.min, self.max * other.max)
 
-    def __add__(self, other):
-        '''Add two multipliers together'''
+    def __add__(self, other: Multiplier, /) -> Multiplier:
+        """Add two multipliers together"""
         return Multiplier(self.min + other.min, self.max + other.max)
 
-    def __sub__(self, other):
-        '''
-            Subtract another multiplier from this one.
-            Caution: multipliers are not totally ordered.
-            This operation is not meaningful for all pairs of multipliers.
-        '''
+    def __sub__(self, other: Multiplier, /) -> Multiplier:
+        """
+        Subtract another multiplier from this one.
+        Caution: multipliers are not totally ordered.
+        This operation is not meaningful for all pairs of multipliers.
+        """
         mandatory = self.mandatory - other.mandatory
         optional = self.optional - other.optional
         return Multiplier(mandatory, mandatory + optional)
 
-    def canintersect(self, other):
-        '''
-            Intersection is not well-defined for all pairs of multipliers.
-            For example:
-                {2,3} & {3,4} = {3}
-                {2,} & {1,7} = {2,7}
-                {2} & {5} = ERROR
-        '''
+    def canintersect(self, other: Multiplier, /) -> bool:
+        """
+        Intersection is not well-defined for all pairs of multipliers.
+        For example:
+            {2,3} & {3,4} = {3}
+            {2,} & {1,7} = {2,7}
+            {2} & {5} = ERROR
+        """
         return not (self.max < other.min or other.max < self.min)
 
-    def __and__(self, other):
-        '''
-            Find the intersection of two multipliers: that is, a third
-            multiplier expressing the range covered by both of the originals.
-            This is not defined for all multipliers since they may not overlap.
-        '''
+    def __and__(self, other: Multiplier, /) -> Multiplier:
+        """
+        Find the intersection of two multipliers: that is, a third
+        multiplier expressing the range covered by both of the originals.
+        This is not defined for all multipliers since they may not overlap.
+        """
         if not self.canintersect(other):
-            raise Exception(
-                f"Can't compute intersection of {repr(self)} and {repr(other)}"
+            raise ArithmeticError(
+                f"Can't compute intersection of {self!r} and {other!r}"
             )
         a = max(self.min, other.min)
         b = min(self.max, other.max)
         return Multiplier(a, b)
 
-    def canunion(self, other):
-        '''
-            Union is not defined for all pairs of multipliers.
-            E.g. {0,1} | {3,4} -> nope
-        '''
-        return not (
-            self.max + Bound(1) < other.min or
-            other.max + Bound(1) < self.min
-        )
-
-    def __or__(self, other):
-        '''
-            Find the union of two multipliers: that is, a third multiplier
-            expressing the range covered by either of the originals. This is
-            not defined for all multipliers since they may not intersect.
-        '''
+    def canunion(self, other: Multiplier, /) -> bool:
+        """
+        Union is not defined for all pairs of multipliers.
+        E.g. {0,1} | {3,4} -> nope
+        """
+        return not (self.max + Bound(1) < other.min or other.max + Bound(1) < self.min)
+
+    def __or__(self, other: Multiplier, /) -> Multiplier:
+        """
+        Find the union of two multipliers: that is, a third multiplier
+        expressing the range covered by either of the originals. This is
+        not defined for all multipliers since they may not intersect.
+        """
         if not self.canunion(other):
-            raise Exception(
-                f"Can't compute the union of {repr(self)} and {repr(other)}"
-            )
+            raise ArithmeticError(f"Can't compute the union of {self!r} and {other!r}")
         a = min(self.min, other.min)
         b = max(self.max, other.max)
         return Multiplier(a, b)
 
-    def common(self, other):
-        '''
-            Find the shared part of two multipliers. This is the largest
-            multiplier which can be safely subtracted from both the originals.
-            This may return the `ZERO` multiplier.
-        '''
+    def common(self, other: Multiplier, /) -> Multiplier:
+        """
+        Find the shared part of two multipliers. This is the largest
+        multiplier which can be safely subtracted from both the originals.
+        This may return the `ZERO` multiplier.
+        """
         mandatory = min(self.mandatory, other.mandatory)
         optional = min(self.optional, other.optional)
         return Multiplier(mandatory, mandatory + optional)
 
-    def copy(self):
+    def copy(self, /) -> Multiplier:
         return Multiplier(self.min.copy(), self.max.copy())
 
 
 # Preset multipliers. These get used ALL THE TIME in unit tests
 ZERO = Multiplier(Bound(0), Bound(0))  # has some occasional uses
 QM = Multiplier(Bound(0), Bound(1))
 ONE = Multiplier(Bound(1), Bound(1))
 STAR = Multiplier(Bound(0), INF)
 PLUS = Multiplier(Bound(1), INF)
 
 # Symbol lookup table for preset multipliers.
-symbolic = {
+symbolic: Mapping[Multiplier, str] = {
     QM: "?",
     ONE: "",
     STAR: "*",
     PLUS: "+",
 }
```

### Comparing `greenery-4.0.0/greenery/multiplier_test.py` & `greenery-4.1.0/greenery/multiplier_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,42 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
-from .bound import Bound, INF
-from .multiplier import Multiplier, ZERO, ONE, QM, STAR, PLUS
+import pytest
 
+from .bound import INF, Bound
+from .multiplier import ONE, PLUS, QM, STAR, ZERO, Multiplier
 
-def test_multiplier_str():
+
+def test_multiplier_str() -> None:
     assert str(Multiplier(Bound(2), INF)) == "{2,}"
+    assert str(Multiplier(Bound(0), Bound(0))) == "{0}"
+    assert str(Multiplier(Bound(2), Bound(2))) == "{2}"
+    assert str(Multiplier(Bound(2), Bound(5))) == "{2,5}"
 
 
-def test_bound_qm():
+def test_bound_qm() -> None:
     assert QM.mandatory == Bound(0)
     assert QM.optional == Bound(1)
 
 
-def test_multiplier_common():
+def test_eq() -> None:
+    assert ZERO == Multiplier(Bound(0), Bound(0))
+    assert ONE == Multiplier(Bound(1), Bound(1))
+    assert STAR == Multiplier(Bound(0), INF)
+    assert Multiplier(Bound(1), Bound(2)) == Multiplier(Bound(1), Bound(2))
+
+    assert ZERO != ONE
+    assert STAR != QM
+
+
+def test_eq_het() -> None:
+    assert ZERO != "goldfish"
+
+
+def test_multiplier_common() -> None:
     assert ZERO.common(ZERO) == ZERO
     assert ZERO.common(QM) == ZERO
     assert ZERO.common(ONE) == ZERO
     assert ZERO.common(STAR) == ZERO
     assert ZERO.common(PLUS) == ZERO
     assert QM.common(ZERO) == ZERO
     assert QM.common(QM) == QM
@@ -37,45 +56,46 @@
     assert PLUS.common(ZERO) == ZERO
     assert PLUS.common(QM) == QM
     assert PLUS.common(ONE) == ONE
     assert PLUS.common(STAR) == STAR
     assert PLUS.common(PLUS) == PLUS
 
 
-def test_multiplier_subtraction():
+def test_multiplier_subtraction() -> None:
     # a{3,4}, a{2,5} -> a{2,3} (with a{1,1}, a{0,2} left over)
-    assert Multiplier(Bound(3), Bound(4)) \
-        .common(Multiplier(Bound(2), Bound(5))) \
-        == Multiplier(Bound(2), Bound(3))
-    assert Multiplier(Bound(3), Bound(4)) - Multiplier(Bound(2), Bound(3)) \
-        == ONE
-    assert Multiplier(Bound(2), Bound(5)) - Multiplier(Bound(2), Bound(3)) \
-        == Multiplier(Bound(0), Bound(2))
+    assert Multiplier(Bound(3), Bound(4)).common(
+        Multiplier(Bound(2), Bound(5))
+    ) == Multiplier(Bound(2), Bound(3))
+    assert Multiplier(Bound(3), Bound(4)) - Multiplier(Bound(2), Bound(3)) == ONE
+    assert Multiplier(Bound(2), Bound(5)) - Multiplier(
+        Bound(2), Bound(3)
+    ) == Multiplier(Bound(0), Bound(2))
 
     # a{2,}, a{1,5} -> a{1,5} (with a{1,}, a{0,0} left over)
-    assert Multiplier(Bound(2), INF).common(Multiplier(Bound(1), Bound(5))) \
-        == Multiplier(Bound(1), Bound(5))
-    assert Multiplier(Bound(2), INF) - Multiplier(Bound(1), Bound(5)) \
-        == PLUS
-    assert Multiplier(Bound(1), Bound(5)) - Multiplier(Bound(1), Bound(5)) \
-        == ZERO
+    assert Multiplier(Bound(2), INF).common(
+        Multiplier(Bound(1), Bound(5))
+    ) == Multiplier(Bound(1), Bound(5))
+    assert Multiplier(Bound(2), INF) - Multiplier(Bound(1), Bound(5)) == PLUS
+    assert Multiplier(Bound(1), Bound(5)) - Multiplier(Bound(1), Bound(5)) == ZERO
 
     # a{3,}, a{2,} -> a{2,} (with a, epsilon left over)
-    assert Multiplier(Bound(3), INF).common(Multiplier(Bound(2), INF)) \
-        == Multiplier(Bound(2), INF)
+    assert Multiplier(Bound(3), INF).common(Multiplier(Bound(2), INF)) == Multiplier(
+        Bound(2), INF
+    )
     assert Multiplier(Bound(3), INF) - Multiplier(Bound(2), INF) == ONE
     assert Multiplier(Bound(2), INF) - Multiplier(Bound(2), INF) == ZERO
 
     # a{3,}, a{3,} -> a{3,} (with ZERO, ZERO left over)
-    assert Multiplier(Bound(3), INF).common(Multiplier(Bound(3), INF)) \
-        == Multiplier(Bound(3), INF)
+    assert Multiplier(Bound(3), INF).common(Multiplier(Bound(3), INF)) == Multiplier(
+        Bound(3), INF
+    )
     assert Multiplier(Bound(3), INF) - Multiplier(Bound(3), INF) == ZERO
 
 
-def test_multiplier_union():
+def test_multiplier_union() -> None:
     assert ZERO | ZERO == ZERO
     assert ZERO | QM == QM
     assert ZERO | ONE == QM
     assert ZERO | STAR == STAR
     assert ZERO | PLUS == STAR
     assert QM | ZERO == QM
     assert QM | QM == QM
@@ -95,23 +115,11 @@
     assert PLUS | ZERO == STAR
     assert PLUS | QM == STAR
     assert PLUS | ONE == PLUS
     assert PLUS | STAR == STAR
     assert PLUS | PLUS == PLUS
     assert not ZERO.canunion(Multiplier(Bound(2), INF))
     assert not ONE.canunion(Multiplier(Bound(3), Bound(4)))
-    assert not Multiplier(
-        Bound(8),
-        INF
-    ).canunion(
-        Multiplier(
-            Bound(3),
-            Bound(4)
-        )
-    )
-    try:
-        ZERO | Multiplier(Bound(7), Bound(8))
-        assert False
-    except AssertionError:
-        assert False
-    except Exception:
-        pass
+    assert not Multiplier(Bound(8), INF).canunion(Multiplier(Bound(3), Bound(4)))
+
+    with pytest.raises(ArithmeticError, match="Can't compute the union"):
+        _ = ZERO | Multiplier(Bound(7), Bound(8))
```

### Comparing `greenery-4.0.0/greenery/parse.py` & `greenery-4.1.0/greenery/parse.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,77 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
-from typing import Tuple
-
-from .bound import Bound, INF
-from .charclass import Charclass, shorthand, escapes
+__all__ = (
+    "parse",
+    "NoMatch",
+)
+
+from typing import Collection, Tuple, TypeVar
+
+from .bound import INF, Bound
+from .charclass import (
+    DIGIT,
+    NONDIGITCHAR,
+    NONSPACECHAR,
+    NONWORDCHAR,
+    SPACECHAR,
+    WORDCHAR,
+    Charclass,
+    escapes,
+    shorthand,
+)
 from .multiplier import Multiplier, symbolic
-from .rxelems import Pattern, Conc, Mult
+from .rxelems import Conc, Mult, Pattern
+
+# Currently many statements are grouped by `try/except NoMatch` in order to try
+# multiple matching functions in sequence. They can be refactored into smaller
+# functions to remove this suppression.
+# pylint: disable=too-many-try-statements
+
+T_co = TypeVar("T_co", covariant=True)
 
 
 class NoMatch(Exception):
-    '''
-        Thrown when parsing fails.
-        Almost always caught and almost never fatal
-    '''
-    pass
+    """
+    Thrown when parsing fails.
+    Almost always caught and almost never fatal
+    """
+
 
+MatchResult = Tuple[T_co, int]
 
-def read_until(string: str, i: int, stop_char: str) -> Tuple[int, str]:
+
+def read_until(string: str, i: int, stop_char: str) -> MatchResult[str]:
     start = i
     while True:
         if i >= len(string):
             raise NoMatch
         if string[i] == stop_char:
             break
         i += 1
-    return i + 1, string[start:i]
+    return string[start:i], i + 1
 
 
-def static(string, i, static):
-    j = i + len(static)
-    if string[i:j] == static:
+def static(haystack: str, i: int, needle: str) -> int:
+    j = i + len(needle)
+    if haystack[i:j] == needle:
         return j
     raise NoMatch
 
 
-def select_static(string, i, *statics):
-    for st in statics:
-        j = i + len(st)
-        if string[i:j] == st:
-            return j, st
+def select_static(haystack: str, i: int, *needles: str) -> MatchResult[str]:
+    for needle in needles:
+        j = i + len(needle)
+        if haystack[i:j] == needle:
+            return needle, j
     raise NoMatch
 
 
-def unescape_hex(string, i):
-    '''Turn e.g. "\\x40" into "@". Exactly two hex digits'''
+def unescape_hex(string: str, i: int) -> MatchResult[str]:
+    """Turn e.g. "\\x40" into "@". Exactly two hex digits"""
     hex_digits = "0123456789AaBbCcDdEeFf"
 
     j = static(string, i, "\\x")
 
     hex1 = string[j]  # e.g. "4"
     if hex1 not in hex_digits:
         raise NoMatch
@@ -59,19 +83,19 @@
     j += len(hex2)
 
     codepoint = int(hex1 + hex2, 16)  # e.g. 64
     char = chr(codepoint)  # "@"
     return char, j
 
 
-def match_internal_char(string, i):
+def match_internal_char(string: str, i: int) -> MatchResult[str]:
     # e.g. if we see "\\t", return "\t"
-    for key in escapes.keys():
+    for char, escaped_mnemonic in escapes.items():
         try:
-            return key, static(string, i, escapes[key])
+            return char, static(string, i, escaped_mnemonic)
         except NoMatch:
             pass
 
     # special chars e.g. "\\-" returns "-"
     for char in Charclass.classSpecial:
         try:
             return char, static(string, i, "\\" + char)
@@ -82,149 +106,144 @@
     try:
         return unescape_hex(string, i)
     except NoMatch:
         pass
 
     # single non-special character, not contained
     # inside square brackets
-    char, j = string[i], i+1
+    char, j = string[i], i + 1
     if char in Charclass.classSpecial:
         raise NoMatch
 
     return char, j
 
 
-def match_class_interior_1(string, i):
-    # Attempt 1: shorthand e.g. "\w"
-    for frozenset, cc_shorthand in Charclass.shorthand.items():
-        try:
-            return frozenset, False, static(string, i, cc_shorthand)
-        except NoMatch:
-            pass
+def match_inner_charclass(
+    string: str,
+    i: int,
+) -> MatchResult[Charclass]:
+    """
+    We have to return several ranges, because of \\\\w etc.
+    """
+    # Attempt 1: shorthand
+    inner_shorthand = {
+        "\\w": WORDCHAR,
+        "\\d": DIGIT,
+        "\\s": SPACECHAR,
+        "\\W": NONWORDCHAR,
+        "\\D": NONDIGITCHAR,
+        "\\S": NONSPACECHAR,
+        # no ".": DOT,
+    }
 
-    # Attempt 1B: shorthand e.g. "\W"
-    for frozenset, cc_shorthand in Charclass.negated_shorthand.items():
+    for cc_shorthand, charclass in inner_shorthand.items():
         try:
-            return frozenset, True, static(string, i, cc_shorthand)
+            return charclass, static(string, i, cc_shorthand)
         except NoMatch:
             pass
 
     # Attempt 2: a range e.g. "d-h"
     try:
         first, j = match_internal_char(string, i)  # `first` is "d"
         k = static(string, j, "-")
         last, k = match_internal_char(string, k)  # `last` is "h"
-
-        firstIndex = ord(first)  # 100
-        lastIndex = ord(last)  # 104
-
-        # Be strict here, "d-d" is not allowed
-        if firstIndex >= lastIndex:
-            raise NoMatch(f"Range '{first}' to '{last}' not allowed")
-
-        chars = set([
-            chr(i) for i in range(firstIndex, lastIndex + 1)
-        ])
-        return chars, False, k
+        return Charclass(((first, last),)), k
     except NoMatch:
         pass
 
     # Attempt 3: just a character on its own
-    (char, j) = match_internal_char(string, i)
-    return set(char), False, j
+    char, j = match_internal_char(string, i)
+    return Charclass(((char, char),)), j
 
 
-def match_class_interior(string, i):
-    internals = set()
-    internals_negated = False
+def match_class_interior(string: str, i: int) -> MatchResult[Charclass]:
+    inner_charclasses = []
     try:
         while True:
-            internal, internal_negated, i = match_class_interior_1(string, i)
-            if internal_negated:
-                if internals_negated:
-                    # E.g. [a1\D\W]
-                    internals |= internal
-                else:
-                    internals_negated = True
-                    internals = internal - internals
-            else:
-                if internals_negated:
-                    internals = internals - internal
-                else:
-                    internals |= internal
+            # Match an internal character, range, or other charclass predicate.
+            inner_charclass, i = match_inner_charclass(string, i)
+            inner_charclasses.append(inner_charclass)
     except NoMatch:
         pass
-    return internals, internals_negated, i
 
+    # Use the existing Charclass union functionality
+    charclass = Charclass()
+    for inner_charclass in inner_charclasses:
+        charclass |= inner_charclass
+
+    return charclass, i
+
+
+def match_charclass(string: str, i: int) -> MatchResult[Charclass]:
+    # pylint: disable=too-many-return-statements
 
-def match_charclass(string: str, i):
     if i >= len(string):
         raise NoMatch
 
     # wildcard ".", "\\w", "\\d", etc.
-    for key in shorthand.keys():
+    for shorthand_charclass, shorthand_abbrev in shorthand.items():
         try:
-            return key, static(string, i, shorthand[key])
+            return shorthand_charclass, static(string, i, shorthand_abbrev)
         except NoMatch:
             pass
 
     # "[^dsgsdg]"
     try:
         j = static(string, i, "[^")
-        chars, negated, j = match_class_interior(string, j)
+        result, j = match_class_interior(string, j)
         j = static(string, j, "]")
-        return Charclass(chars, not negated), j
+        return ~result, j
     except NoMatch:
         pass
 
     # "[sdfsf]"
     try:
         j = static(string, i, "[")
-        chars, negated, j = match_class_interior(string, j)
+        result, j = match_class_interior(string, j)
         j = static(string, j, "]")
-        return Charclass(chars, negated), j
+        return result, j
     except NoMatch:
         pass
 
     # e.g. if seeing "\\t", return "\t"
-    for key in escapes.keys():
+    for char, escaped_mnemonic in escapes.items():
         try:
-            return Charclass(key), static(string, i, escapes[key])
+            return Charclass(((char, char),)), static(string, i, escaped_mnemonic)
         except NoMatch:
             pass
 
     # e.g. if seeing "\\{", return "{"
     for char in Charclass.allSpecial:
         try:
-            return Charclass(char), static(string, i, "\\" + char)
+            return Charclass(((char, char),)), static(string, i, "\\" + char)
         except NoMatch:
             pass
 
     # e.g. if seeing "\\x40", return "@"
     try:
         char, j = unescape_hex(string, i)
-        return Charclass(char), j
+        return Charclass(((char, char),)), j
     except NoMatch:
         pass
 
     # single non-special character, not contained inside square brackets
-    char, i = string[i], i+1
+    char, i = string[i], i + 1
     if char in Charclass.allSpecial:
         raise NoMatch
 
-    return Charclass(char), i
+    return Charclass(((char, char),)), i
 
 
-def match_multiplicand(string, i):
+def match_multiplicand(string: str, i: int) -> MatchResult[Pattern | Charclass]:
     # explicitly non-capturing "(?:...)" syntax. No special significance
     try:
         j = static(string, i, "(?")
-        j, st = select_static(string, j, ':', 'P<')
-        if st == 'P<':
-            j, group_name = read_until(string, j, '>')
+        opts, j = select_static(string, j, ":", "P<")
+        if opts == "P<":
+            _group_name, j = read_until(string, j, ">")
         pattern, j = match_pattern(string, j)
         j = static(string, j, ")")
         return pattern, j
     except NoMatch:
         pass
 
     # normal "(...)" syntax
@@ -237,24 +256,24 @@
         pass
 
     # Just a `Charclass` on its own
     charclass, j = match_charclass(string, i)
     return charclass, j
 
 
-def match_any_of(string, i, collection):
+def match_any_of(string: str, i: int, collection: Collection[str]) -> MatchResult[str]:
     for char in collection:
         try:
             return char, static(string, i, char)
         except NoMatch:
             pass
     raise NoMatch
 
 
-def match_bound(string: str, i):
+def match_bound(string: str, i: int) -> MatchResult[Bound]:
     # "0"
     try:
         return Bound(0), static(string, i, "0")
     except NoMatch:
         pass
 
     # "1", etc.
@@ -271,66 +290,66 @@
     except NoMatch:
         pass
 
     # "" empty string = infinite bound as in "{4,}"
     return INF, i
 
 
-def match_multiplier(string: str, i):
+def match_multiplier(string: str, i: int) -> MatchResult[Multiplier]:
     # {2,3} or {2,}
     try:
         j = static(string, i, "{")
-        min, j = match_bound(string, j)
+        min_, j = match_bound(string, j)
         j = static(string, j, ",")
-        max, j = match_bound(string, j)
+        max_, j = match_bound(string, j)
         j = static(string, j, "}")
-        return Multiplier(min, max), j
+        return Multiplier(min_, max_), j
     except NoMatch:
         pass
 
     # {2}
     try:
         j = static(string, i, "{")
-        min, j = match_bound(string, j)
+        min_, j = match_bound(string, j)
         j = static(string, j, "}")
-        return Multiplier(min, min), j
+        return Multiplier(min_, min_), j
     except NoMatch:
         pass
 
     # "?"/"*"/"+"/""
     # we do these in reverse order of symbol length, because
     # that forces "" to be done last
-    for key in sorted(symbolic, key=lambda key: -len(symbolic[key])):
+    for mult, symbol in sorted(symbolic.items(), key=lambda kv: -len(kv[1])):
         try:
-            return key, static(string, i, symbolic[key])
+            return mult, static(string, i, symbol)
         except NoMatch:
             pass
 
     raise NoMatch
 
 
-def match_mult(string: str, i):
+def match_mult(string: str, i: int) -> MatchResult[Mult]:
     multiplicand, j = match_multiplicand(string, i)
     multiplier, j = match_multiplier(string, j)
     return Mult(multiplicand, multiplier), j
 
 
-def match_conc(string: str, i):
-    mults = list()
+def match_conc(string: str, i: int) -> MatchResult[Conc]:
+    mults = []
     try:
         while True:
             m, i = match_mult(string, i)
             mults.append(m)
     except NoMatch:
         pass
     return Conc(*mults), i
 
 
-def match_pattern(string: str, i):
-    concs = list()
+def match_pattern(string: str, i: int) -> MatchResult[Pattern]:
+    concs = []
 
     # first one
     c, i = match_conc(string, i)
     concs.append(c)
 
     # the rest
     while True:
@@ -338,18 +357,16 @@
             i = static(string, i, "|")
             c, i = match_conc(string, i)
             concs.append(c)
         except NoMatch:
             return Pattern(*concs), i
 
 
-def parse(string: str):
-    '''
-        Parse a full string and return a `Pattern` object. Fail if
-        the whole string wasn't parsed
-    '''
+def parse(string: str) -> Pattern:
+    """
+    Parse a full string and return a `Pattern` object. Fail if
+    the whole string wasn't parsed
+    """
     obj, i = match_pattern(string, 0)
     if i != len(string):
-        raise Exception(
-            f"Could not parse '{string}' beyond index {str(i)}"
-        )
+        raise NoMatch(f"Could not parse {string!r} beyond index {i}")
     return obj
```

### Comparing `greenery-4.0.0/greenery/parse_test.py` & `greenery-4.1.0/greenery/parse_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,143 +1,140 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
+
+import pytest
+
+from .bound import INF, Bound
+from .charclass import DIGIT, DOT, NULLCHARCLASS, Charclass
+from .multiplier import ONE, PLUS, STAR, Multiplier
+
+# noinspection PyProtectedMember
+from .parse import NoMatch, match_charclass, match_mult, parse
+from .rxelems import Conc, Mult, Pattern
 
 if __name__ == "__main__":
-    raise Exception(
+    raise RuntimeError(
         "Test files can't be run directly. Use `python -m pytest greenery`"
     )
 
-from .bound import Bound, INF
-from .charclass import Charclass, DOT, NULLCHARCLASS, DIGIT
-from .multiplier import Multiplier, ONE, STAR, PLUS
-from .rxelems import Mult, Conc, Pattern
-from .parse import NoMatch, match_charclass, parse, match_mult
 
-
-def test_charclass_matching():
+def test_charclass_matching() -> None:
     assert match_charclass("a", 0) == (Charclass("a"), 1)
     assert match_charclass("aa", 1) == (Charclass("a"), 2)
     assert match_charclass("a$", 1) == (Charclass("$"), 2)
     assert match_charclass(".", 0) == (DOT, 1)
-    try:
+
+    with pytest.raises(IndexError):
         match_charclass("[", 0)
-        assert False
-    except IndexError:
-        pass
-    try:
+
+    with pytest.raises(NoMatch):
         match_charclass("a", 1)
-        assert False
-    except NoMatch:
-        pass
+
     assert match_charclass("[\\d]", 0) == (DIGIT, 4)
 
 
-def test_negatives_inside_charclasses():
+def test_negatives_inside_charclasses() -> None:
     assert match_charclass("[\\D]", 0) == (~DIGIT, 4)
     assert match_charclass("[a\\D]", 0) == (~DIGIT, 5)
     assert match_charclass("[a1\\D]", 0) == (~Charclass("023456789"), 6)
     assert match_charclass("[1a\\D]", 0) == (~Charclass("023456789"), 6)
     assert match_charclass("[1\\D]", 0) == (~Charclass("023456789"), 5)
     assert match_charclass("[\\Da]", 0) == (~DIGIT, 5)
     assert match_charclass("[\\D1]", 0) == (~Charclass("023456789"), 5)
     assert match_charclass("[\\D1a]", 0) == (~Charclass("023456789"), 6)
     assert match_charclass("[\\D\\d]", 0) == (DOT, 6)
     assert match_charclass("[\\D\\D]", 0) == (~DIGIT, 6)
-    assert match_charclass("[\\S\\D]", 0) == \
-        (~Charclass("\t\n\v\f\r 0123456789"), 6)
-    assert match_charclass("[\\S \\D]", 0) == \
-        (~Charclass("\t\n\v\f\r0123456789"), 7)
 
+    # "Either non-whitespace or a non-digit" matches _anything_.
+    assert match_charclass("[\\S\\D]", 0) == (DOT, 6)
+    assert match_charclass("[\\S \\D]", 0) == (DOT, 7)
 
-def test_negated_negatives_inside_charclasses():
+
+def test_negated_negatives_inside_charclasses() -> None:
     assert match_charclass("[^\\D]", 0) == (DIGIT, 5)
     assert match_charclass("[^a\\D]", 0) == (DIGIT, 6)
     assert match_charclass("[^a1\\D]", 0) == (Charclass("023456789"), 7)
     assert match_charclass("[^1a\\D]", 0) == (Charclass("023456789"), 7)
     assert match_charclass("[^1\\D]", 0) == (Charclass("023456789"), 6)
     assert match_charclass("[^\\Da]", 0) == (DIGIT, 6)
     assert match_charclass("[^\\D1]", 0) == (Charclass("023456789"), 6)
     assert match_charclass("[^\\D1a]", 0) == (Charclass("023456789"), 7)
     assert match_charclass("[^\\D\\d]", 0) == (NULLCHARCLASS, 7)
     assert match_charclass("[^\\D\\D]", 0) == (DIGIT, 7)
-    assert match_charclass("[^\\S\\D]", 0) == \
-        (Charclass("\t\n\v\f\r 0123456789"), 7)
-    assert match_charclass("[^\\S \\D]", 0) == \
-        (Charclass("\t\n\v\f\r0123456789"), 8)
+
+    # "Anything but non-whitespace and non-digit" matches _nothing_.
+    assert match_charclass("[^\\S\\D]", 0) == (NULLCHARCLASS, 7)
+    assert match_charclass("[^\\S \\D]", 0) == (NULLCHARCLASS, 8)
 
 
-def test_mult_matching():
-    assert match_mult("abcde[^fg]*", 5) == (
-        Mult(~Charclass("fg"), STAR),
-        11
+def test_match_nightmare_charclass() -> None:
+    assert match_charclass("[\t\n\r -\uD7FF\uE000-\uFFFD\U00010000-\U0010FFFF]", 0) == (
+        Charclass(
+            (
+                ("\t", "\t"),
+                ("\n", "\n"),
+                ("\r", "\r"),
+                (" ", "\uD7FF"),
+                ("\uE000", "\uFFFD"),
+                ("\U00010000", "\U0010FFFF"),
+            )
+        ),
+        14,
     )
+
+
+def test_mult_matching() -> None:
+    assert match_mult("abcde[^fg]*", 5) == (Mult(~Charclass("fg"), STAR), 11)
     assert match_mult("abcde[^fg]*h{5}[a-z]+", 11) == (
         Mult(Charclass("h"), Multiplier(Bound(5), Bound(5))),
-        15
+        15,
     )
     assert match_mult("abcde[^fg]*h{5}[a-z]+T{1,}", 15) == (
         Mult(Charclass("abcdefghijklmnopqrstuvwxyz"), PLUS),
-        21
+        21,
     )
     assert match_mult("abcde[^fg]*h{5}[a-z]+T{2,}", 21) == (
         Mult(Charclass("T"), Multiplier(Bound(2), INF)),
-        26
+        26,
     )
 
 
-def test_charclass_ranges():
+def test_charclass_ranges() -> None:
     # Should accept arbitrary ranges of characters in charclasses. No longer
     # limited to alphanumerics. (User beware...)
     assert parse("[z{|}~]") == parse("[z-~]")
     assert parse("[\\w:;<=>?@\\[\\\\\\]\\^`]") == parse("[0-z]")
 
 
-def test_hex_escapes():
+def test_hex_escapes() -> None:
     # Should be able to parse e.g. "\\x40"
     assert parse("\\x00") == parse("\x00")
     assert parse("\\x40") == parse("@")
     assert parse("[\\x40]") == parse("[@]")
     assert parse("[\\x41-\\x5a]") == parse("[A-Z]")
 
 
-def test_w_d_s():
+def test_w_d_s() -> None:
     # Allow "\w", "\d" and "\s" in charclasses
     assert parse("\\w") == parse("[0-9A-Z_a-z]")
     assert parse("[\\w~]") == parse("[0-9A-Z_a-z~]")
     assert parse("[\\da]") == parse("[0123456789a]")
     assert parse("[\\s]") == parse("[\t\n\r\f\v ]")
 
 
-def test_mult_parsing():
-    assert parse("[a-g]+") == Pattern(
-        Conc(
-            Mult(
-                Charclass("abcdefg"),
-                PLUS
-            )
-        )
-    )
+def test_mult_parsing() -> None:
+    assert parse("[a-g]+") == Pattern(Conc(Mult(Charclass("abcdefg"), PLUS)))
     assert parse("[a-g0-8$%]+") == Pattern(
-        Conc(
-            Mult(
-                Charclass("abcdefg012345678$%"),
-                PLUS
-            )
-        )
+        Conc(Mult(Charclass("abcdefg012345678$%"), PLUS))
     )
     assert parse("[a-g0-8$%\\^]+") == Pattern(
-        Conc(
-            Mult(
-                Charclass("abcdefg012345678$%^"),
-                PLUS
-            )
-        )
+        Conc(Mult(Charclass("abcdefg012345678$%^"), PLUS))
     )
 
 
-def test_conc_parsing():
+def test_conc_parsing() -> None:
     assert parse("abcde[^fg]*h{5}[a-z]+") == Pattern(
         Conc(
             Mult(Charclass("a"), ONE),
             Mult(Charclass("b"), ONE),
             Mult(Charclass("c"), ONE),
             Mult(Charclass("d"), ONE),
             Mult(Charclass("e"), ONE),
@@ -169,15 +166,15 @@
             Mult(DIGIT, Multiplier(Bound(2), Bound(2))),
             Mult(Charclass("-"), ONE),
             Mult(DIGIT, Multiplier(Bound(2), Bound(2))),
         )
     )
 
 
-def test_pattern_parsing():
+def test_pattern_parsing() -> None:
     assert parse("abc|def(ghi|jkl)") == Pattern(
         Conc(
             Mult(Charclass("a"), ONE),
             Mult(Charclass("b"), ONE),
             Mult(Charclass("c"), ONE),
         ),
         Conc(
@@ -206,7 +203,27 @@
     # special significance
     assert parse("(?:)") == parse("()")
     assert parse("(?:abc|def)") == parse("(abc|def)")
     parse("(:abc)")  # should give no problems
 
     # Named groups
     assert parse("(?P<ng1>abc)") == parse("(abc)")
+
+
+def test_nightmare_pattern() -> None:
+    assert parse("[\t\n\r -\uD7FF\uE000-\uFFFD\U00010000-\U0010FFFF]*") == Pattern(
+        Conc(
+            Mult(
+                Charclass(
+                    (
+                        ("\t", "\t"),
+                        ("\n", "\n"),
+                        ("\r", "\r"),
+                        (" ", "\uD7FF"),
+                        ("\uE000", "\uFFFD"),
+                        ("\U00010000", "\U0010FFFF"),
+                    )
+                ),
+                STAR,
+            )
+        )
+    )
```

### Comparing `greenery-4.0.0/greenery/pattern_test.py` & `greenery-4.1.0/greenery/pattern_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# -*- coding: utf-8 -*-
+from __future__ import annotations
 
 from .charclass import Charclass
 from .multiplier import ONE, ZERO
-from .rxelems import Pattern, Conc, Mult
 from .parse import parse
+from .rxelems import Conc, Mult, Pattern
 
 
-def test_pattern_equality():
+def test_pattern_equality() -> None:
     assert Pattern(
         Conc(Mult(Charclass("a"), ONE)),
         Conc(Mult(Charclass("b"), ONE)),
     ) == Pattern(
         Conc(Mult(Charclass("b"), ONE)),
         Conc(Mult(Charclass("a"), ONE)),
     )
@@ -18,108 +18,129 @@
         Conc(Mult(Charclass("a"), ONE)),
         Conc(Mult(Charclass("a"), ONE)),
     ) == Pattern(
         Conc(Mult(Charclass("a"), ONE)),
     )
 
 
-def test_pattern_str():
-    assert str(Pattern(
-        Conc(Mult(Charclass("a"), ONE)),
-        Conc(Mult(Charclass("b"), ONE)),
-    )) == "a|b"
-    assert str(Pattern(
-        Conc(Mult(Charclass("a"), ONE)),
-        Conc(Mult(Charclass("a"), ONE)),
-    )) == "a"
-    assert str(Pattern(
-        Conc(
-            Mult(Charclass("a"), ONE),
-            Mult(Charclass("b"), ONE),
-            Mult(Charclass("c"), ONE),
-        ),
-        Conc(
-            Mult(Charclass("d"), ONE),
-            Mult(Charclass("e"), ONE),
-            Mult(Charclass("f"), ONE),
-            Mult(
-                Pattern(
-                    Conc(
-                        Mult(Charclass("g"), ONE),
-                        Mult(Charclass("h"), ONE),
-                        Mult(Charclass("i"), ONE),
-                    ),
-                    Conc(
-                        Mult(Charclass("j"), ONE),
-                        Mult(Charclass("k"), ONE),
-                        Mult(Charclass("l"), ONE),
+def test_pattern_str() -> None:
+    assert (
+        str(
+            Pattern(
+                Conc(Mult(Charclass("a"), ONE)),
+                Conc(Mult(Charclass("b"), ONE)),
+            )
+        )
+        == "a|b"
+    )
+    assert (
+        str(
+            Pattern(
+                Conc(Mult(Charclass("a"), ONE)),
+                Conc(Mult(Charclass("a"), ONE)),
+            )
+        )
+        == "a"
+    )
+    assert (
+        str(
+            Pattern(
+                Conc(
+                    Mult(Charclass("a"), ONE),
+                    Mult(Charclass("b"), ONE),
+                    Mult(Charclass("c"), ONE),
+                ),
+                Conc(
+                    Mult(Charclass("d"), ONE),
+                    Mult(Charclass("e"), ONE),
+                    Mult(Charclass("f"), ONE),
+                    Mult(
+                        Pattern(
+                            Conc(
+                                Mult(Charclass("g"), ONE),
+                                Mult(Charclass("h"), ONE),
+                                Mult(Charclass("i"), ONE),
+                            ),
+                            Conc(
+                                Mult(Charclass("j"), ONE),
+                                Mult(Charclass("k"), ONE),
+                                Mult(Charclass("l"), ONE),
+                            ),
+                        ),
+                        ONE,
                     ),
                 ),
-                ONE,
-            ),
-        ),
-    )) == "abc|def(ghi|jkl)"
+            )
+        )
+        == "abc|def(ghi|jkl)"
+    )
 
 
-def test_empty():
+def test_empty() -> None:
     assert Pattern().empty()
 
 
-def test_mult_reduction_easy():
+def test_mult_reduction_easy() -> None:
     assert Pattern(Conc()).reduce() == Pattern(Conc())
     assert Pattern(
         Conc(
             Mult(
                 Charclass("a"),
                 ZERO,
             )
         )
-    ).reduce() == Pattern(
-        Conc()
-    )
+    ).reduce() == Pattern(Conc())
+
     assert str(
+        # pylint: disable-next=compare-to-empty-string
         Pattern(
             Conc(
                 Mult(
                     Charclass("a"),
                     ZERO,
                 )
-            )
-        ).reduce()
-    ) == ""
+            ).reduce()
+        )
+        == ""
+    )
 
 
-def test_empty_pattern_reduction():
+def test_empty_pattern_reduction() -> None:
     assert str(Pattern().reduce()) == "[]"
 
 
-def test_empty_conc_suppression():
-    assert str(Pattern(
-        Conc(
-            # this `Mult` can never actually match anything
-            Mult(Pattern(), ONE),
-            Mult(Charclass("0"), ONE),
-            Mult(Charclass("0123456789"), ONE),
-        )  # so neither can this `Conc`
-    ).reduce()) == "[]"
+def test_empty_conc_suppression() -> None:
+    assert (
+        str(
+            Pattern(
+                Conc(
+                    # this `Mult` can never actually match anything
+                    Mult(Pattern(), ONE),
+                    Mult(Charclass("0"), ONE),
+                    Mult(Charclass("0123456789"), ONE),
+                )  # so neither can this `Conc`
+            ).reduce()
+        )
+        == "[]"
+    )
 
 
-def test_pattern_dock():
+def test_pattern_dock() -> None:
     a = Mult(Charclass("a"), ONE)
     c = Mult(Charclass("c"), ONE)
     f = Mult(Charclass("f"), ONE)
 
     assert parse("a|bc").dock(Conc()) == parse("a|bc")
     assert parse("aa|bca").dock(Conc(a)) == parse("a|bc")
     assert parse("xyza|abca|a").dock(Conc(a)) == parse("xyz|abc|")
     assert parse("f{2,3}c|fc").dock(Conc(f, c)) == parse("f{1,2}|")
     assert parse("aa").dock(Conc(a, a)) == parse("")
 
 
-def test_pattern_beheading():
+def test_pattern_beheading() -> None:
     a = Mult(Charclass("a"), ONE)
     c = Mult(Charclass("c"), ONE)
     f = Mult(Charclass("f"), ONE)
     z = Mult(Charclass("Z"), ONE)
 
     assert parse("aa").behead(Conc(a)) == parse("a")
     assert parse("abc|aa").behead(Conc(a)) == parse("a|bc")
```

### Comparing `greenery-4.0.0/greenery/rxelems.py` & `greenery-4.1.0/greenery/rxelems.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,62 @@
-# -*- coding: utf-8 -*-
-
-'''
-    Because of the circularity between `Pattern`, `Conc` and `Mult`, all three
-    need to be in the same source file?
-'''
+"""
+Because of the circularity between `Pattern`, `Conc` and `Mult`, all three
+need to be in the same source file?
+"""
+
+from __future__ import annotations
+
+__all__ = (
+    "Conc",
+    "Mult",
+    "Pattern",
+    "from_fsm",
+)
 
 from dataclasses import dataclass
-from typing import Union
-
-from .fsm import Fsm, ANYTHING_ELSE, null, epsilon, alphabet_key
-from .multiplier import Multiplier, ZERO, QM, ONE, STAR
-from .charclass import Charclass, NULLCHARCLASS
-from .bound import Bound, INF
+from enum import Enum, auto
+from functools import reduce
+from typing import Iterator
+
+from .bound import INF, Bound
+from .charclass import NULLCHARCLASS, Charclass
+from .fsm import EPSILON, NULL, Fsm, StateType, from_charclass
+from .multiplier import ONE, QM, STAR, ZERO, Multiplier
 
 
 @dataclass(frozen=True)
-class Conc():
-    '''
-        A `Conc` (short for "concatenation") is a tuple of `Mult`s i.e. an
-        unbroken string of mults occurring one after the other.
-        e.g. abcde[^fg]*h{4}[a-z]+(subpattern)(subpattern2)
-        To express the empty string, use an empty `Conc`, Conc().
-    '''
-    def __init__(self, *mults):
+class Conc:
+    """
+    A `Conc` (short for "concatenation") is a tuple of `Mult`s i.e. an
+    unbroken string of mults occurring one after the other.
+    e.g. abcde[^fg]*h{4}[a-z]+(subpattern)(subpattern2)
+    To express the empty string, use an empty `Conc`, Conc().
+    """
+
+    mults: tuple[Mult, ...]
+
+    def __init__(self, /, *mults: Mult):
         object.__setattr__(self, "mults", tuple(mults))
 
-    def __eq__(self, other):
+    def __eq__(self, other: object, /) -> bool:
+        if not isinstance(other, type(self)):
+            return NotImplemented
         return self.mults == other.mults
 
-    def __hash__(self):
+    def __hash__(self, /) -> int:
         return hash(self.mults)
 
-    def __repr__(self):
+    def __repr__(self, /) -> str:
         args = ", ".join(repr(mult) for mult in self.mults)
         return f"Conc({args})"
 
-    def reduce(self):
+    def reduce(self) -> Conc:
+        # pylint: disable=too-many-branches
+        # pylint: disable=too-many-return-statements
+
         if self == NULLCONC:
             return self
 
         if self.empty():
             return NULLCONC
 
         # Try recursively reducing our mults
@@ -49,148 +66,124 @@
 
         # strip out mults which can only match the empty string
         for i, mult in enumerate(self.mults):
             if (
                 # Conc contains "()" (i.e. a `Mult` containing only a `Pattern`
                 # containing the empty string)? That can be removed
                 # e.g. "a()b" -> "ab"
-                (
-                    mult.multiplicand == Pattern(EMPTYSTRING)
-                ) \
-
+                mult.multiplicand == Pattern(EMPTYSTRING)
                 # If a `Mult` has an empty multiplicand, we can only match it
                 # zero times => empty string => remove it entirely
                 # e.g. "a[]{0,3}b" -> "ab"
-                or (
-                    mult.multiplicand.empty()
-                    and mult.multiplier.min == Bound(0)
-                ) \
-
+                or (mult.multiplicand.empty() and mult.multiplier.min == Bound(0))
                 # Failing that, we have a positive multiplicand which we
                 # intend to match zero times. In this case the only possible
                 # match is the empty string => remove it
                 # e.g. "a[XYZ]{0}b" -> "ab"
                 or mult.multiplier == ZERO
             ):
-                new = self.mults[:i] + self.mults[i + 1:]
+                new = self.mults[:i] + self.mults[i + 1 :]
                 return Conc(*new).reduce()
 
         # We might be able to combine some mults together or at least simplify
         # the multiplier on one of them.
         if len(self.mults) > 1:
             for i in range(len(self.mults) - 1):
                 r = self.mults[i]
                 s = self.mults[i + 1]
 
-                def to_pattern(multiplicand):
+                def to_pattern(multiplicand: Pattern | Charclass, /) -> Pattern:
                     if isinstance(multiplicand, Pattern):
                         return multiplicand
                     return Pattern(Conc(Mult(multiplicand, ONE)))
 
                 # so we can do intersection
                 rm_pattern = to_pattern(r.multiplicand)
                 sm_pattern = to_pattern(s.multiplicand)
                 rm_sm_intersection = None
 
                 # If R = S, then we can squish the multipliers together
                 # e.g. ab?b?c -> ab{0,2}c
                 if rm_pattern == sm_pattern:
-                    squished = Mult(
-                        rm_pattern,
-                        r.multiplier + s.multiplier
-                    )
-                    new = self.mults[:i] + (squished,) + self.mults[i + 2:]
+                    squished = Mult(rm_pattern, r.multiplier + s.multiplier)
+                    new = self.mults[:i] + (squished,) + self.mults[i + 2 :]
                     return Conc(*new).reduce()
 
                 # If R's language is a subset of S's, then R{a,b}S{c,} reduces
                 # to R{a}S{c,}...
                 # e.g. \d+\w+ -> \d\w+
                 # Do the cheapest checks first
-                if r.multiplier.min < r.multiplier.max \
-                   and s.multiplier.max == INF:
+                if r.multiplier.min < r.multiplier.max and s.multiplier.max == INF:
                     rm_sm_intersection = rm_pattern & sm_pattern
                     if rm_sm_intersection.equivalent(rm_pattern):
                         trimmed = Mult(
                             rm_pattern,
-                            Multiplier(r.multiplier.min, r.multiplier.min)
+                            Multiplier(r.multiplier.min, r.multiplier.min),
                         )
-                        new = self.mults[:i] + \
-                            (trimmed, s) + \
-                            self.mults[i + 2:]
+                        new = self.mults[:i] + (trimmed, s) + self.mults[i + 2 :]
                         return Conc(*new).reduce()
 
                 # Conversely, if R is superset of S, then R{c,}S{a,b} reduces
                 # to R{c,}S{a}.
                 # e.g. [ab]+a? -> [ab]+
                 # Do the cheapest checks first
-                if r.multiplier.max == INF \
-                   and s.multiplier.min < s.multiplier.max:
+                if r.multiplier.max == INF and s.multiplier.min < s.multiplier.max:
                     if rm_sm_intersection is None:
                         rm_sm_intersection = rm_pattern & sm_pattern
                     if rm_sm_intersection.equivalent(sm_pattern):
                         trimmed = Mult(
                             sm_pattern,
-                            Multiplier(s.multiplier.min, s.multiplier.min)
+                            Multiplier(s.multiplier.min, s.multiplier.min),
                         )
-                        new = self.mults[:i] + \
-                            (r, trimmed) + \
-                            self.mults[i + 2:]
+                        new = self.mults[:i] + (r, trimmed) + self.mults[i + 2 :]
                         return Conc(*new).reduce()
 
         # Conc contains (among other things) a *singleton* `Mult` containing
         # `Pattern` with only one internal `Conc`? Flatten out.
         # e.g. "a(d(ab|a*c))" -> "ad(ab|a*c)"
         # BUT NOT "a(d(ab|a*c)){2,}"
         # AND NOT "a(d(ab|a*c)|y)"
         for i, mult in enumerate(self.mults):
-            if mult.multiplier == ONE \
-               and isinstance(mult.multiplicand, Pattern) \
-               and len(mult.multiplicand.concs) == 1:
+            if (
+                mult.multiplier == ONE
+                and isinstance(mult.multiplicand, Pattern)
+                and len(mult.multiplicand.concs) == 1
+            ):
                 (conc,) = mult.multiplicand.concs
-                new = self.mults[:i] + conc.mults + self.mults[i + 1:]
+                new = self.mults[:i] + conc.mults + self.mults[i + 1 :]
                 return Conc(*new).reduce()
 
         return self
 
-    def to_fsm(self, alphabet=None):
-        if alphabet is None:
-            alphabet = self.alphabet()
-
-        # start with a component accepting only the empty string
-        fsm1 = epsilon(alphabet)
-        for mult in self.mults:
-            fsm1 += mult.to_fsm(alphabet)
-        return fsm1
+    def to_fsm(self, /) -> Fsm:
+        return Fsm.concatenate(EPSILON, *(mult.to_fsm() for mult in self.mults))
 
-    def alphabet(self):
-        return {ANYTHING_ELSE}.union(*[mult.alphabet() for mult in self.mults])
-
-    def empty(self):
+    def empty(self, /) -> bool:
         return any(mult.empty() for mult in self.mults)
 
-    def __str__(self):
+    def __str__(self, /) -> str:
         return "".join(str(m) for m in self.mults)
 
-    def common(self, other, suffix=False):
-        '''
-            Return the common prefix of these two `Conc`s; that is, the largest
-            `Conc` which can be safely beheaded() from the front of both. The
-            result could be `EMPTYSTRING`.
-            "ZYAA, ZYBB" -> "ZY"
-            "CZ, CZ" -> "CZ"
-            "YC, ZC" -> ""
-
-            With the "suffix" flag set, works from the end. E.g.:
-            "AAZY, BBZY" -> "ZY"
-            "CZ, CZ" -> "CZ"
-            "CY, CZ" -> ""
-        '''
+    def common(self, other: Conc, /, suffix: bool = False) -> Conc:
+        """
+        Return the common prefix of these two `Conc`s; that is, the largest
+        `Conc` which can be safely beheaded() from the front of both. The
+        result could be `EMPTYSTRING`.
+        "ZYAA, ZYBB" -> "ZY"
+        "CZ, CZ" -> "CZ"
+        "YC, ZC" -> ""
+
+        With the "suffix" flag set, works from the end. E.g.:
+        "AAZY, BBZY" -> "ZY"
+        "CZ, CZ" -> "CZ"
+        "CY, CZ" -> ""
+        """
         mults = []
 
-        indices = range(min(len(self.mults), len(other.mults)))
+        indices = list(range(min(len(self.mults), len(other.mults))))
         # e.g. [0, 1, 2, 3]
 
         # Work backwards from the end of both `Conc`s instead.
         if suffix:
             indices = [-i - 1 for i in indices]  # e.g. [-1, -2, -3, -4]
 
         for i in indices:
@@ -208,25 +201,25 @@
 
             # If we did not remove the entirety of both mults, we cannot
             # continue.
             if common != x or common != y:
                 break
 
         if suffix:
-            mults = reversed(mults)
+            mults = mults[::-1]
 
         return Conc(*mults)
 
-    def dock(self, other):
-        '''
-            Subtract another `Conc` from this one.
-            This is the opposite of concatenation.
-            For example, if ABC + DEF = ABCDEF,
-            then logically ABCDEF - DEF = ABC.
-        '''
+    def dock(self, other: Conc, /) -> Conc:
+        """
+        Subtract another `Conc` from this one.
+        This is the opposite of concatenation.
+        For example, if ABC + DEF = ABCDEF,
+        then logically ABCDEF - DEF = ABC.
+        """
 
         # e.g. self has mults at indices [0, 1, 2, 3, 4, 5, 6] len=7
         # e.g. other has mults at indices [0, 1, 2] len=3
         new = list(self.mults)
         for i in reversed(range(len(other.mults))):  # [2, 1, 0]
             # e.g. i = 1, j = 7 - 3 + 1 = 5
             j = len(self.mults) - len(other.mults) + i
@@ -236,52 +229,46 @@
                 # omit that `Mult` entirely since it has been factored out
                 del new[j]
 
             # If the subtraction is incomplete but there is more to
             # other.mults, then we have a problem. For example, "ABC{2} - BC"
             # subtracts the C successfully but leaves something behind,
             # then tries to subtract the B too, which isn't possible
-            else:
-                if i != 0:
-                    raise Exception(
-                        f"Can't subtract {repr(other)} from {repr(self)}"
-                    )
+            elif i:
+                raise ArithmeticError(f"Can't subtract {other!r} from {self!r}")
 
         return Conc(*new)
 
-    def behead(self, other):
-        '''
-            As with dock() but the other way around. For example, if
-            ABC + DEF = ABCDEF, then ABCDEF.behead(AB) = CDEF.
-        '''
+    def behead(self, other: Conc, /) -> Conc:
+        """
+        As with dock() but the other way around. For example, if
+        ABC + DEF = ABCDEF, then ABCDEF.behead(AB) = CDEF.
+        """
         # Observe that FEDCBA - BA = FEDC.
         return self.reversed().dock(other.reversed()).reversed()
 
-    def reversed(self):
-        return Conc(*reversed([mult.reversed() for mult in self.mults]))
+    def reversed(self, /) -> Conc:
+        return Conc(*[mult.reversed() for mult in reversed(self.mults)])
 
 
-def from_fsm(f: Fsm):
-    '''
-        Turn the supplied finite state machine into a `Pattern`. This is
-        accomplished using the Brzozowski algebraic method.
-    '''
-    # Make sure the supplied alphabet is kosher. It must contain only single-
-    # character strings or `ANYTHING_ELSE`.
-    for symbol in f.alphabet:
-        if symbol == ANYTHING_ELSE:
-            continue
-        if isinstance(symbol, str) and len(symbol) == 1:
-            continue
-        raise Exception(
-            f"Symbol {repr(symbol)} cannot be used in a regular expression"
-        )
+# We need a new state not already used.
+class _Outside(Enum):
+    """Marker state for use in `from_fsm`."""
+
+    TOKEN = auto()
+
 
-    # We need a new state not already used
-    outside = object()
+def from_fsm(f: Fsm) -> Pattern:
+    """
+    Turn the supplied finite state machine into a `Pattern`. This is
+    accomplished using the Brzozowski algebraic method.
+    """
+    # pylint: disable=too-many-branches
+
+    outside = _Outside.TOKEN
 
     # The set of strings that would be accepted by this FSM if you started
     # at state i is represented by the regex R_i.
     # If state i has a sole transition "a" to state j, then we know
     # R_i = a R_j.
     # If state i is final, then the empty string is also accepted by this
     # regex.
@@ -295,64 +282,52 @@
     # so that when we perform our back-substitutions, we can start with the
     # last (deepest) state and therefore finish with R_a.
     states = [f.initial]
     i = 0
     while i < len(states):
         current = states[i]
         if current in f.map:
-            for symbol in sorted(f.map[current], key=alphabet_key):
-                next = f.map[current][symbol]
-                if next not in states:
-                    states.append(next)
+            for symbol in sorted(f.map[current]):
+                next_state = f.map[current][symbol]
+                if next_state not in states:
+                    states.append(next_state)
         i += 1
 
     # Our system of equations is represented like so:
-    brz = {}
+    brz: dict[StateType, dict[StateType | _Outside, Pattern]] = {}
+
     for a in f.states:
         brz[a] = {}
         for b in f.states:
             brz[a][b] = NULLPATTERN
 
         if a in f.finals:
             brz[a][outside] = Pattern(EMPTYSTRING)
         else:
             brz[a][outside] = NULLPATTERN
 
     # Populate it with some initial data.
     for a in f.map:
-        for symbol in f.map[a]:
-            b = f.map[a][symbol]
-            if symbol == ANYTHING_ELSE:
-                charclass = ~Charclass(f.alphabet - {ANYTHING_ELSE})
-            else:
-                charclass = Charclass({symbol})
-
-            brz[a][b] = Pattern(
-                *brz[a][b].concs,
-                Conc(Mult(charclass, ONE))
-            ).reduce()
+        for charclass in f.map[a]:
+            b = f.map[a][charclass]
+            brz[a][b] = Pattern(*brz[a][b].concs, Conc(Mult(charclass, ONE))).reduce()
 
     # Now perform our back-substitution
     for i in reversed(range(len(states))):
         a = states[i]
 
         # Before the equation for R_a can be substituted into the other
         # equations, we need to resolve the self-transition (if any).
         # e.g.    R_a = 0 R_a |   1 R_b |   2 R_c
         # becomes R_a =         0*1 R_b | 0*2 R_c
         loop = Mult(brz[a][a], STAR)  # i.e. "0*"
         del brz[a][a]
 
         for right in brz[a]:
-            brz[a][right] = Pattern(
-                Conc(
-                    loop,
-                    Mult(brz[a][right], ONE)
-                )
-            ).reduce()
+            brz[a][right] = Pattern(Conc(loop, Mult(brz[a][right], ONE))).reduce()
 
         # Note: even if we're down to our final equation, the above step still
         # needs to be performed before anything is returned.
 
         # Now we can substitute this equation into all of the previous ones.
         for j in range(i):
             b = states[j]
@@ -362,109 +337,91 @@
             # yields            R_b = 30*1 R_b | (30*2|4) R_c | 5 R_d
             univ = brz[b][a]  # i.e. "3"
             del brz[b][a]
 
             for right in brz[a]:
                 brz[b][right] = Pattern(
                     *brz[b][right].concs,
-                    Conc(
-                        Mult(univ, ONE),
-                        Mult(brz[a][right], ONE)
-                    )
+                    Conc(Mult(univ, ONE), Mult(brz[a][right], ONE)),
                 ).reduce()
 
     return brz[f.initial][outside].reduce()
 
 
-def call_fsm(method):
-    '''
-        Take a method which acts on 0 or more regular expression objects...
-        return a new method which simply converts them all to FSMs, calls the
-        FSM method on them instead, then converts the result back to a regular
-        expression. We do this for several of the more annoying operations.
-    '''
-    fsm_method = getattr(Fsm, method.__name__)
-
-    def new_method(*elems):
-        alphabet = set().union(*[elem.alphabet() for elem in elems])
-        return from_fsm(fsm_method(*[elem.to_fsm(alphabet) for elem in elems]))
-    return new_method
-
-
 @dataclass(frozen=True)
 class Pattern:
-    '''
-        A `Pattern` (also known as an "alt", short for "alternation") is a
-        set of `Conc`s. A `Pattern` expresses multiple alternate possibilities.
-        When written out as a regex, these would separated by pipes. A
-        `Pattern` containing no possibilities is possible and represents a
-        regular expression matching no strings whatsoever (there is no
-        conventional string form for this).
-
-        e.g. "abc|def(ghi|jkl)" is an alt containing two `Conc`s: "abc" and
-        "def(ghi|jkl)". The latter is a `Conc` containing four `Mult`s: "d",
-        "e", "f" and "(ghi|jkl)". The latter in turn is a `Mult` consisting of
-        an upper bound 1, a lower bound 1, and a multiplicand which is a new
-        subpattern, "ghi|jkl". This new subpattern again consists of two
-        `Conc`s: "ghi" and "jkl".
-    '''
-    def __init__(self, *concs):
+    """
+    A `Pattern` (also known as an "alt", short for "alternation") is a
+    set of `Conc`s. A `Pattern` expresses multiple alternate possibilities.
+    When written out as a regex, these would separated by pipes. A
+    `Pattern` containing no possibilities is possible and represents a
+    regular expression matching no strings whatsoever (there is no
+    conventional string form for this).
+
+    e.g. "abc|def(ghi|jkl)" is an alt containing two `Conc`s: "abc" and
+    "def(ghi|jkl)". The latter is a `Conc` containing four `Mult`s: "d",
+    "e", "f" and "(ghi|jkl)". The latter in turn is a `Mult` consisting of
+    an upper bound 1, a lower bound 1, and a multiplicand which is a new
+    subpattern, "ghi|jkl". This new subpattern again consists of two
+    `Conc`s: "ghi" and "jkl".
+    """
+
+    concs: frozenset[Conc]
+
+    def __init__(self, /, *concs: Conc):
         object.__setattr__(self, "concs", frozenset(concs))
 
-    def __eq__(self, other):
-        return isinstance(other, Pattern) and self.concs == other.concs
+    def __eq__(self, other: object, /) -> bool:
+        if not isinstance(other, type(self)):
+            return NotImplemented
+        return self.concs == other.concs
 
-    def __hash__(self):
+    def __hash__(self, /) -> int:
         return hash(self.concs)
 
-    def __repr__(self):
+    def __repr__(self, /) -> str:
         args = ", ".join(repr(conc) for conc in self.concs)
         return f"Pattern({args})"
 
-    def alphabet(self):
-        return {ANYTHING_ELSE}.union(*[c.alphabet() for c in self.concs])
-
-    def empty(self):
+    def empty(self, /) -> bool:
         return all(conc.empty() for conc in self.concs)
 
-    def intersection(self, other):
-        # A deceptively simple method for an astoundingly difficult operation
-        alphabet = self.alphabet() | other.alphabet()
-
-        # Which means that we can build finite state machines sharing that
-        # alphabet
-        combined = self.to_fsm(alphabet) & other.to_fsm(alphabet)
+    def intersection(self, other: Pattern, /) -> Pattern:
+        combined = self.to_fsm() & other.to_fsm()
         return from_fsm(combined)
 
-    def __and__(self, other):
+    def __and__(self, other: Pattern, /) -> Pattern:
         return self.intersection(other)
 
-    @call_fsm
-    def difference(*elems):
-        '''
-            Return a regular expression which matches any string which `self`
-            matches but none of the strings which `other` matches.
-        '''
-        pass
+    def difference(*elems: Pattern) -> Pattern:
+        """
+        Return a regular expression which matches any string which `self`
+        matches but none of the strings which `other` matches.
+        """
+        return from_fsm(Fsm.difference(*(elem.to_fsm() for elem in elems)))
 
-    def __sub__(self, other):
+    def __sub__(self, other: Pattern, /) -> Pattern:
         return self.difference(other)
 
-    def union(self, other):
+    def union(self, other: Pattern, /) -> Pattern:
         return Pattern(*(self.concs | other.concs))
 
-    def __or__(self, other):
+    def __or__(self, other: Pattern, /) -> Pattern:
         return self.union(other)
 
-    def __str__(self):
-        if len(self.concs) == 0:
-            raise Exception(f"Can't serialise {repr(self)}")
+    def __str__(self, /) -> str:
+        if not self.concs:
+            raise ValueError(f"Can't serialise {self!r}")
         return "|".join(sorted(str(conc) for conc in self.concs))
 
-    def reduce(self):
+    def reduce(self, /) -> Pattern:
+        # pylint: disable=too-many-branches
+        # pylint: disable=too-many-locals
+        # pylint: disable=too-many-return-statements
+
         if self == NULLPATTERN:
             return self
 
         if self.empty():
             return NULLPATTERN
 
         # Try recursively reducing our internal `Conc`s.
@@ -478,26 +435,27 @@
                 new = self.concs - {conc}
                 return Pattern(*new).reduce()
 
         # If we have just one `Conc` with just one `Mult` with a multiplier of
         # 1, and the multiplicand is a `Pattern`, pull that up
         if len(self.concs) == 1:
             (conc,) = self.concs
-            if len(conc.mults) == 1 \
-               and conc.mults[0].multiplier == ONE \
-               and isinstance(conc.mults[0].multiplicand, Pattern):
+            if (
+                len(conc.mults) == 1
+                and conc.mults[0].multiplier == ONE
+                and isinstance(conc.mults[0].multiplicand, Pattern)
+            ):
                 return conc.mults[0].multiplicand.reduce()
 
         # If this `Pattern` contains several `Conc`s each containing just 1
         # `Mult` and their multiplicands agree, we may be able to merge the
         # multipliers.
         # e.g. "a{1,2}|a{3,4}|bc" -> "a{1,4}|bc"
         oldconcs = list(self.concs)  # so we can index the things
-        for i in range(len(oldconcs)):
-            conc1 = oldconcs[i]
+        for i, conc1 in enumerate(oldconcs):
             if len(conc1.mults) != 1:
                 continue
             multiplicand1 = conc1.mults[0].multiplicand
             for j in range(i + 1, len(oldconcs)):
                 conc2 = oldconcs[j]
                 if len(conc2.mults) != 1:
                     continue
@@ -506,67 +464,65 @@
                     continue
                 multiplicand = multiplicand1
                 multiplier1 = conc1.mults[0].multiplier
                 multiplier2 = conc2.mults[0].multiplier
                 if not multiplier1.canunion(multiplier2):
                     continue
                 multiplier = multiplier1 | multiplier2
-                newconcs = \
-                    oldconcs[:i] + \
-                    oldconcs[i + 1:j] + \
-                    oldconcs[j + 1:] + \
-                    [Conc(Mult(multiplicand, multiplier))]
+                newconcs = (
+                    oldconcs[:i]
+                    + oldconcs[i + 1 : j]
+                    + oldconcs[j + 1 :]
+                    + [Conc(Mult(multiplicand, multiplier))]
+                )
                 return Pattern(*newconcs).reduce()
 
         # If this `Pattern` contains several `Conc`s each containing just 1
         # `Mult` each containing just a `Charclass`, with a multiplier of 1,
         # then we can merge those `Charclass`es together.
         # e.g. "0|[1-9]|ab" -> "[0-9]|ab"
         merged_charclass = NULLCHARCLASS
         num_merged = 0
         rest = []
         for conc in self.concs:
-            if len(conc.mults) == 1 \
-               and conc.mults[0].multiplier == ONE \
-               and isinstance(conc.mults[0].multiplicand, Charclass):
+            if (
+                len(conc.mults) == 1
+                and conc.mults[0].multiplier == ONE
+                and isinstance(conc.mults[0].multiplicand, Charclass)
+            ):
                 merged_charclass |= conc.mults[0].multiplicand
                 num_merged += 1
             else:
                 rest.append(conc)
         if num_merged >= 2:
             rest.append(Conc(Mult(merged_charclass, ONE)))
             return Pattern(*rest).reduce()
 
         # If one of the present `Pattern`'s `Conc`s is the empty string...
         if EMPTYSTRING in self.concs:
             for conc in self.concs:
                 # ...and there is another `Conc`
                 # with a single `Mult` whose lower bound is 0...
-                if len(conc.mults) == 1 \
-                   and conc.mults[0].multiplier.min == Bound(0):
+                if len(conc.mults) == 1 and conc.mults[0].multiplier.min == Bound(0):
                     # Then we can omit the empty string.
                     # E.g. "|(ab)*|def" => "(ab)*|def".
-                    rest = self.concs - {EMPTYSTRING}
-                    return Pattern(*rest).reduce()
+                    return Pattern(*(self.concs - {EMPTYSTRING})).reduce()
 
             for conc in self.concs:
                 # ...and there is another `Conc`
                 # with a single `Mult` whose lower bound is 1...
-                if len(conc.mults) == 1 \
-                   and conc.mults[0].multiplier.min == Bound(1):
+                if len(conc.mults) == 1 and conc.mults[0].multiplier.min == Bound(1):
                     # Then we can merge the empty string into that.
                     # E.g. "|(ab)+|def" => "(ab)*|def".
                     merged_conc = Conc(
-                        Mult(
-                            conc.mults[0].multiplicand,
-                            conc.mults[0].multiplier * QM
-                        )
+                        Mult(conc.mults[0].multiplicand, conc.mults[0].multiplier * QM)
                     )
-                    rest = self.concs - {EMPTYSTRING, conc} | {merged_conc}
-                    return Pattern(*rest).reduce()
+                    return Pattern(
+                        *(self.concs - {EMPTYSTRING, conc} | {merged_conc})
+                    ).reduce()
 
         # If the present `Pattern`'s `Conc`s all have a common prefix, split
         # that out. This increases the depth of the object
         # but it is still arguably simpler/ripe for further reduction
         # e.g. "abc|ade" -> a(bc|de)"
         if len(self.concs) > 1:
             prefix = self._commonconc()
@@ -581,246 +537,216 @@
             if suffix != EMPTYSTRING:
                 leftovers = self.dock(suffix)
                 mults = (Mult(leftovers, ONE),) + suffix.mults
                 return Pattern(Conc(*mults)).reduce()
 
         return self
 
-    @call_fsm
-    def symmetric_difference(*elems):
-        '''
-            Return a regular expression matching only the strings recognised by
-            `self` or `other` but not both.
-        '''
-        pass
+    def symmetric_difference(*elems: Pattern) -> Pattern:
+        """
+        Return a regular expression matching only the strings recognised by
+        `self` or `other` but not both.
+        """
+        return from_fsm(Fsm.symmetric_difference(*(elem.to_fsm() for elem in elems)))
 
-    def __xor__(self, other):
+    def __xor__(self, other: Pattern, /) -> Pattern:
         return self.symmetric_difference(other)
 
-    def dock(self, other):
-        '''
-            The opposite of concatenation. Remove a common suffix from the
-            present `Pattern`; that is, from each of its constituent concs.
+    def dock(self, other: Conc, /) -> Pattern:
+        """
+        The opposite of concatenation. Remove a common suffix from the
+        present `Pattern`; that is, from each of its constituent concs.
 
-            AYZ|BYZ|CYZ - YZ -> A|B|C.
-        '''
+        AYZ|BYZ|CYZ - YZ -> A|B|C.
+        """
         return Pattern(*[conc.dock(other) for conc in self.concs])
 
-    def behead(self, other):
-        '''
-            Like dock() but the other way around. Remove a common prefix from
-            the present `Pattern`; that is, from each of its constituent concs.
+    def behead(self, other: Conc, /) -> Pattern:
+        """
+        Like dock() but the other way around. Remove a common prefix from
+        the present `Pattern`; that is, from each of its constituent concs.
 
-            ZA|ZB|ZC.behead(Z) -> A|B|C
-        '''
+        ZA|ZB|ZC.behead(Z) -> A|B|C
+        """
         return Pattern(*[conc.behead(other) for conc in self.concs])
 
-    def _commonconc(self, suffix=False):
-        '''
-            Find the longest `Conc` which acts as prefix to every `Conc` in
-            this `Pattern`. This could be `EMPTYSTRING`. Return the common
-            prefix along with all the leftovers after truncating that common
-            prefix from each `Conc`.
-
-            "ZA|ZB|ZC" -> "Z", "(A|B|C)"
-            "ZA|ZB|ZC|Z" -> "Z", "(A|B|C|)"
-            "CZ|CZ" -> "CZ", "()"
-
-            If "suffix" is True, the same result but for suffixes.
-        '''
-        if len(self.concs) == 0:
-            raise Exception(f"Can't call _commonconc on {repr(self)}")
-
-        from functools import reduce
-        return reduce(
-            lambda x, y: x.common(y, suffix=suffix),
-            self.concs
-        )
+    def _commonconc(self, /, suffix: bool = False) -> Conc:
+        """
+        Find the longest `Conc` which acts as prefix to every `Conc` in
+        this `Pattern`. This could be `EMPTYSTRING`. Return the common
+        prefix along with all the leftovers after truncating that common
+        prefix from each `Conc`.
+
+        "ZA|ZB|ZC" -> "Z", "(A|B|C)"
+        "ZA|ZB|ZC|Z" -> "Z", "(A|B|C|)"
+        "CZ|CZ" -> "CZ", "()"
+
+        If "suffix" is True, the same result but for suffixes.
+        """
+        if not self.concs:
+            raise ValueError(f"Can't call _commonconc on {self!r}")
 
-    def to_fsm(self, alphabet=None):
-        if alphabet is None:
-            alphabet = self.alphabet()
+        return reduce(lambda x, y: x.common(y, suffix=suffix), self.concs)
 
-        fsm1 = null(alphabet)
-        for conc in self.concs:
-            fsm1 |= conc.to_fsm(alphabet)
-        return fsm1
+    def to_fsm(self, /) -> Fsm:
+        return Fsm.union(NULL, *(conc.to_fsm() for conc in self.concs))
 
-    def reversed(self):
+    def reversed(self, /) -> Pattern:
         return Pattern(*(c.reversed() for c in self.concs))
 
-    def copy(self):
-        '''
-            For completeness only, since `set.copy()` also exists. `Pattern`s
-            are immutable, so I can see only very odd reasons to need this
-        '''
+    def copy(self, /) -> Pattern:
+        """
+        For completeness only, since `set.copy()` also exists. `Pattern`s
+        are immutable, so I can see only very odd reasons to need this
+        """
         return Pattern(*self.concs)
 
-    def equivalent(self, other):
-        '''
-            Two `Pattern`s are equivalent if they recognise the same strings.
-            Note that in the general case this is actually quite an intensive
-            calculation, but far from unsolvable, as we demonstrate here:
-        '''
+    def equivalent(self, other: Pattern, /) -> bool:
+        """
+        Two `Pattern`s are equivalent if they recognise the same strings.
+        Note that in the general case this is actually quite an intensive
+        calculation, but far from unsolvable, as we demonstrate here:
+        """
         return self.to_fsm().equivalent(other.to_fsm())
 
-    def times(self, multiplier):
-        '''
-            Equivalent to repeated concatenation. Multiplier consists of a
-            minimum and a maximum; maximum may be infinite (for Kleene star
-            closure). Call using "a = b * qm"
-        '''
+    def times(self, multiplier: Multiplier, /) -> Pattern:
+        """
+        Equivalent to repeated concatenation. Multiplier consists of a
+        minimum and a maximum; maximum may be infinite (for Kleene star
+        closure). Call using "a = b * qm"
+        """
         return Pattern(Conc(Mult(self, multiplier)))
 
-    def __mul__(self, multiplier):
+    def __mul__(self, multiplier: Multiplier, /) -> Pattern:
         return self.times(multiplier)
 
-    @call_fsm
-    def everythingbut(self):
-        '''
-            Return a `Pattern` which will match any string not matched by
-            `self`, and which will not match any string matched by `self`.
-            Another task which is very difficult in general (and typically
-            returns utter garbage when actually printed), but becomes trivial
-            to code thanks to FSM routines.
-        '''
-        pass
+    def everythingbut(self, /) -> Pattern:
+        """
+        Return a `Pattern` which will match any string not matched by
+        `self`, and which will not match any string matched by `self`.
+        Another task which is very difficult in general (and typically
+        returns utter garbage when actually printed), but becomes trivial
+        to code thanks to FSM routines.
+        """
+        return from_fsm(self.to_fsm().everythingbut())
 
-    def derive(self, string):
+    def derive(self, string: str, /) -> Pattern:
         return from_fsm(self.to_fsm().derive(string))
 
-    @call_fsm
-    def isdisjoint(self, other):
-        '''
-            Treat `self` and `other` as sets of strings and see if they are
-            disjoint
-        '''
-        pass
+    def isdisjoint(self, other: Pattern, /) -> bool:
+        """
+        Treat `self` and `other` as sets of strings and see if they are
+        disjoint
+        """
+        return self.to_fsm().isdisjoint(other.to_fsm())
 
-    def matches(self, string):
+    def matches(self, string: str, /) -> bool:
         return self.to_fsm().accepts(string)
 
-    def __contains__(self, string):
-        '''
-            This lets you use the syntax `"a" in pattern` to see whether the
-            string "a" is in the set of strings matched by `pattern`.
-        '''
+    def __contains__(self, string: str, /) -> bool:
+        """
+        This lets you use the syntax `"a" in pattern` to see whether the
+        string "a" is in the set of strings matched by `pattern`.
+        """
         return self.matches(string)
 
-    def __reversed__(self):
+    # pylint: disable=fixme
+    # TODO: this is a misuse of __reversed__
+    # and should be removed next major version
+    def __reversed__(self, /) -> Pattern:
         return self.reversed()
 
-    def cardinality(self):
-        '''
-            Consider the regular expression as a set of strings and return the
-            cardinality of that set, or raise an OverflowError if there are
-            infinitely many.
-        '''
+    def cardinality(self, /) -> int:
+        """
+        Consider the regular expression as a set of strings and return the
+        cardinality of that set, or raise an OverflowError if there are
+        infinitely many.
+        """
         # There is no way to do this other than converting to an FSM, because
         # the `Pattern` may allow duplicate routes, such as "a|a".
         return self.to_fsm().cardinality()
 
-    def __len__(self):
+    def __len__(self, /) -> int:
         return self.cardinality()
 
-    def strings(self, otherchar=None):
-        '''
-            Each time next() is called on this iterator, a new string is
-            returned which this `Pattern` can match. `StopIteration`
-            is raised once all such strings have been returned, although a
-            regex with a * in may match infinitely many strings.
-        '''
-
-        # In the case of a regex like "[^abc]", there are infinitely many
-        # (well, a very large finite number of) single characters which will
-        # match. It's not productive to iterate over all of these giving every
-        # single example. You must supply your own "otherchar" to stand in for
-        # all of these possibilities.
-        for string in self.to_fsm().strings():
-
-            # Have to represent `ANYTHING_ELSE` somehow.
-            if ANYTHING_ELSE in string:
-                if otherchar is None:
-                    raise Exception("Please choose an `otherchar`")
-                string = [
-                    otherchar if char == ANYTHING_ELSE else char
-                    for char in string
-                ]
-
-            yield "".join(string)
-
-    def __iter__(self):
-        '''
-            This allows you to do `for string in pattern` as a list
-            comprehension!
-        '''
+    def strings(self, /, *, otherchar: str | None = None) -> Iterator[str]:
+        """
+        Each time next() is called on this iterator, a new string is
+        returned which this `Pattern` can match. `StopIteration`
+        is raised once all such strings have been returned, although a
+        regex with a * in may match infinitely many strings.
+        """
+        otherchars = [] if otherchar is None else [otherchar]
+        return self.to_fsm().strings(otherchars)
+
+    def __iter__(self, /) -> Iterator[str]:
+        """
+        This allows you to do `for string in pattern` as a list
+        comprehension!
+        """
         return self.strings()
 
 
 @dataclass(frozen=True)
 class Mult:
-    '''
-        A `Mult` is a combination of a multiplicand with a multiplier (a min
-        and a max). The vast majority of characters in regular expressions
-        occur without a specific multiplier, which is implicitly equivalent to
-        a min of 1 and a max of 1, but many more have explicit multipliers like
-        "*" (min = 0, max = INF) and so on.
-
-        e.g. a, b{2}, c?, d*, [efg]{2,5}, f{2,}, (anysubpattern)+, .*, ...
-    '''
-    multiplicand: Union[Charclass, Pattern]
+    """
+    A `Mult` is a combination of a multiplicand with a multiplier (a min
+    and a max). The vast majority of characters in regular expressions
+    occur without a specific multiplier, which is implicitly equivalent to
+    a min of 1 and a max of 1, but many more have explicit multipliers like
+    "*" (min = 0, max = INF) and so on.
+
+    e.g. a, b{2}, c?, d*, [efg]{2,5}, f{2,}, (anysubpattern)+, .*, ...
+    """
+
+    multiplicand: Charclass | Pattern
     multiplier: Multiplier
 
-    def __eq__(self, other):
-        return isinstance(other.multiplicand, type(self.multiplicand)) \
-               and self.multiplicand == other.multiplicand \
-               and self.multiplier == other.multiplier
+    def __eq__(self, other: object, /) -> bool:
+        if not isinstance(other, type(self)):
+            return NotImplemented
+        return (
+            self.multiplicand == other.multiplicand
+            and self.multiplier == other.multiplier
+        )
 
-    def __hash__(self):
+    def __hash__(self, /) -> int:
         return hash((self.multiplicand, self.multiplier))
 
-    def __repr__(self):
-        return f"Mult({repr(self.multiplicand)}, {repr(self.multiplier)})"
+    def __repr__(self, /) -> str:
+        return f"Mult({self.multiplicand!r}, {self.multiplier!r})"
 
-    def dock(self, other):
-        '''
-            "Dock" another `Mult` from this one (i.e. remove part of the tail)
-            and return the result. The reverse of concatenation. This is a lot
-            trickier.
-            e.g. a{4,5} - a{3} = a{1,2}
-        '''
+    def dock(self, other: Mult, /) -> Mult:
+        """
+        "Dock" another `Mult` from this one (i.e. remove part of the tail)
+        and return the result. The reverse of concatenation. This is a lot
+        trickier.
+        e.g. a{4,5} - a{3} = a{1,2}
+        """
         if other.multiplicand != self.multiplicand:
-            raise Exception(
-                f"Can't subtract {repr(other)} from {repr(self)}"
-            )
+            raise ArithmeticError(f"Can't subtract {other!r} from {self!r}")
         return Mult(self.multiplicand, self.multiplier - other.multiplier)
 
-    def common(self, other):
-        '''
-            Return the common part of these two mults. This is the largest
-            `Mult` which can be safely subtracted from both the originals. The
-            multiplier on this `Mult` could be `ZERO`: this is the case if, for
-            example, the multiplicands disagree.
-        '''
+    def common(self, other: Mult, /) -> Mult:
+        """
+        Return the common part of these two mults. This is the largest
+        `Mult` which can be safely subtracted from both the originals. The
+        multiplier on this `Mult` could be `ZERO`: this is the case if, for
+        example, the multiplicands disagree.
+        """
         if self.multiplicand == other.multiplicand:
-            return Mult(
-                self.multiplicand,
-                self.multiplier.common(other.multiplier)
-            )
+            return Mult(self.multiplicand, self.multiplier.common(other.multiplier))
 
         # Multiplicands disagree, no common part at all.
         return Mult(NULLCHARCLASS, ZERO)
 
-    def alphabet(self):
-        return {ANYTHING_ELSE} | self.multiplicand.alphabet()
-
-    def empty(self):
+    def empty(self, /) -> bool:
         return self.multiplicand.empty() and self.multiplier.min > Bound(0)
 
-    def reduce(self):
+    def reduce(self, /) -> Mult:
         if self == NULLMULT:
             return self
 
         # Can't match anything: reduce to empty `Mult`
         if self.empty():
             return NULLMULT
 
@@ -830,82 +756,87 @@
             return Mult(reduced, self.multiplier).reduce()
 
         # If our multiplicand is a `Pattern` containing an empty `Conc`
         # we can pull that "optional" bit out into our own multiplier
         # instead.
         # e.g. (A|B|C|) -> (A|B|C)?
         # e.g. (A|B|C|){2} -> (A|B|C){0,2}
-        if isinstance(self.multiplicand, Pattern) \
-           and EMPTYSTRING in self.multiplicand.concs \
-           and self.multiplier.canmultiplyby(QM):
+        if (
+            isinstance(self.multiplicand, Pattern)
+            and EMPTYSTRING in self.multiplicand.concs
+            and self.multiplier.canmultiplyby(QM)
+        ):
             return Mult(
-                Pattern(
-                    *filter(
-                        lambda conc: len(conc.mults) != 0,
-                        self.multiplicand.concs
-                    )
-                ),
+                Pattern(*(conc for conc in self.multiplicand.concs if conc.mults)),
                 self.multiplier * QM,
             ).reduce()
 
         # If our multiplicand is a `Pattern` containing a single `Conc`
         # containing a single `Mult`, we can scrap the `Pattern` in favour of
         # that `Mult`'s multiplicand
         # e.g. ([ab])* -> [ab]*
         # e.g. ((a))* -> (a)* -> a*
         # NOTE: this logic lives here at the `Mult` level, NOT in
         # `Pattern.reduce` because we want to return another `Mult` (same type)
-        if isinstance(self.multiplicand, Pattern) \
-           and len(self.multiplicand.concs) == 1:
+        if isinstance(self.multiplicand, Pattern) and len(self.multiplicand.concs) == 1:
             (conc,) = self.multiplicand.concs
-            if len(conc.mults) == 1 \
-               and conc.mults[0].multiplier.canmultiplyby(self.multiplier):
+            if len(conc.mults) == 1 and conc.mults[0].multiplier.canmultiplyby(
+                self.multiplier
+            ):
                 return Mult(
                     conc.mults[0].multiplicand,
-                    conc.mults[0].multiplier * self.multiplier
+                    conc.mults[0].multiplier * self.multiplier,
                 ).reduce()
 
         # no reduction possible
         return self
 
-    def __str__(self):
+    def __str__(self, /) -> str:
         if isinstance(self.multiplicand, Pattern):
-            return f"({str(self.multiplicand)}){str(self.multiplier)}"
+            return f"({self.multiplicand}){self.multiplier}"
         if isinstance(self.multiplicand, Charclass):
-            return f"{str(self.multiplicand)}{str(self.multiplier)}"
-        raise Exception(f"Unknown type {str(type(self.inner))}")
-
-    def to_fsm(self, alphabet=None):
-        if alphabet is None:
-            alphabet = self.alphabet()
+            return f"{self.multiplicand}{self.multiplier}"
+        raise TypeError(f"Unknown type {type(self.multiplicand)}")
 
+    def to_fsm(self, /) -> Fsm:
         # worked example: (min, max) = (5, 7) or (5, INF)
         # (mandatory, optional) = (5, 2) or (5, INF)
 
-        unit = self.multiplicand.to_fsm(alphabet)
+        unit = (
+            from_charclass(self.multiplicand)
+            if isinstance(self.multiplicand, Charclass)
+            else self.multiplicand.to_fsm()
+        )
         # accepts e.g. "ab"
 
+        # Yuck. `mandatory` cannot be infinite: it's just a natural number.
+        # However, it uses `Bound`, which describes co-naturals.
+        assert self.multiplier.mandatory.v is not None
+
         # accepts "ababababab"
-        mandatory = unit * self.multiplier.mandatory.v
+        mandatory = unit.times(self.multiplier.mandatory.v)
 
         # unlimited additional copies
         if self.multiplier.optional == INF:
             optional = unit.star()
             # accepts "(ab)*"
 
         else:
-            optional = epsilon(alphabet) | unit
+            optional = EPSILON | unit
             # accepts "(ab)?"
 
-            optional *= self.multiplier.optional.v
+            # Implied by `!= INF`.
+            assert self.multiplier.optional.v is not None
+
+            optional = optional.times(self.multiplier.optional.v)
             # accepts "(ab)?(ab)?"
 
-        return mandatory + optional
+        return mandatory.concatenate(optional)
 
-    def reversed(self):
+    def reversed(self, /) -> Mult:
         return Mult(self.multiplicand.reversed(), self.multiplier)
 
 
 NULLMULT = Mult(NULLCHARCLASS, ONE)
 NULLCONC = Conc(NULLMULT)
 EMPTYSTRING = Conc()
 NULLPATTERN = Pattern(NULLCONC)
```

### Comparing `greenery-4.0.0/greenery.egg-info/SOURCES.txt` & `greenery-4.1.0/greenery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `greenery-4.0.0/setup.py` & `greenery-4.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,39 @@
+from __future__ import annotations
+
 from setuptools import setup
 
 setup(
     name="greenery",
-    version="4.0.0",
+    version="4.1.0",
     tests_require=["pytest"],
     packages=["greenery"],
-    package_dir={
-        "greenery": "greenery"
-    },
+    package_dir={"greenery": "greenery"},
     author="qntm",
     author_email="qntm <qntm@users.noreply.github.com>",
     description="Greenery allows manipulation of regular expressions",
     license="MIT License",
-    keywords=" ".join([
-        "re", "regex", "regexp", "regular", "expression", "deterministic",
-        "finite", "state", "machine", "automaton", "fsm", "dfsm", "fsa",
-        "dfsa", "greenery",
-    ]),
+    keywords=" ".join(
+        [
+            "re",
+            "regex",
+            "regexp",
+            "regular",
+            "expression",
+            "deterministic",
+            "finite",
+            "state",
+            "machine",
+            "automaton",
+            "fsm",
+            "dfsm",
+            "fsa",
+            "dfsa",
+            "greenery",
+        ]
+    ),
     url="https://github.com/qntm/greenery",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
     ],
 )
```

