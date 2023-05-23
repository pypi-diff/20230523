# Comparing `tmp/CardGameBase-1.0.3.tar.gz` & `tmp/CardGameBase-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CardGameBase-1.0.3.tar", last modified: Mon May 22 14:04:58 2023, max compression
+gzip compressed data, was "CardGameBase-1.0.4.tar", last modified: Tue May 23 13:11:41 2023, max compression
```

## Comparing `CardGameBase-1.0.3.tar` & `CardGameBase-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:04:58.120648 CardGameBase-1.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:04:58.105009 CardGameBase-1.0.3/CardGameBase/
--rw-rw-rw-   0        0        0     3116 2023-05-16 09:08:46.000000 CardGameBase-1.0.3/CardGameBase/Card.py
--rw-rw-rw-   0        0        0     6242 2023-05-16 10:12:24.000000 CardGameBase-1.0.3/CardGameBase/Deck.py
--rw-rw-rw-   0        0        0       39 2023-04-13 10:08:54.000000 CardGameBase-1.0.3/CardGameBase/Exceptions.py
--rw-rw-rw-   0        0        0     7854 2023-05-22 13:37:46.000000 CardGameBase-1.0.3/CardGameBase/Hand.py
--rw-rw-rw-   0        0        0      970 2023-04-14 08:52:08.000000 CardGameBase-1.0.3/CardGameBase/Utility.py
--rw-rw-rw-   0        0        0      119 2023-04-13 10:09:58.000000 CardGameBase-1.0.3/CardGameBase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:04:58.120648 CardGameBase-1.0.3/CardGameBase.egg-info/
--rw-rw-rw-   0        0        0     1499 2023-05-22 14:04:57.000000 CardGameBase-1.0.3/CardGameBase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-05-22 14:04:58.000000 CardGameBase-1.0.3/CardGameBase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:04:57.000000 CardGameBase-1.0.3/CardGameBase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-22 14:04:57.000000 CardGameBase-1.0.3/CardGameBase.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1235 2023-05-16 07:57:54.000000 CardGameBase-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1499 2023-05-22 14:04:58.120648 CardGameBase-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      889 2023-05-16 11:03:15.000000 CardGameBase-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 14:04:58.120648 CardGameBase-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1171 2023-05-22 14:01:45.000000 CardGameBase-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:11:41.434572 CardGameBase-1.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-23 13:11:41.418939 CardGameBase-1.0.4/CardGameBase/
+-rw-rw-rw-   0        0        0     3156 2023-05-23 12:58:36.000000 CardGameBase-1.0.4/CardGameBase/Card.py
+-rw-rw-rw-   0        0        0     6293 2023-05-23 13:02:38.000000 CardGameBase-1.0.4/CardGameBase/Deck.py
+-rw-rw-rw-   0        0        0       39 2023-04-13 10:08:54.000000 CardGameBase-1.0.4/CardGameBase/Exceptions.py
+-rw-rw-rw-   0        0        0     7899 2023-05-23 12:57:36.000000 CardGameBase-1.0.4/CardGameBase/Hand.py
+-rw-rw-rw-   0        0        0      972 2023-05-23 12:54:04.000000 CardGameBase-1.0.4/CardGameBase/Utility.py
+-rw-rw-rw-   0        0        0      119 2023-04-13 10:09:58.000000 CardGameBase-1.0.4/CardGameBase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-23 13:11:41.418939 CardGameBase-1.0.4/CardGameBase.egg-info/
+-rw-rw-rw-   0        0        0     1500 2023-05-23 13:11:41.000000 CardGameBase-1.0.4/CardGameBase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-05-23 13:11:41.000000 CardGameBase-1.0.4/CardGameBase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-23 13:11:41.000000 CardGameBase-1.0.4/CardGameBase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-23 13:11:41.000000 CardGameBase-1.0.4/CardGameBase.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1235 2023-05-16 07:57:54.000000 CardGameBase-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1500 2023-05-23 13:11:41.434572 CardGameBase-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      889 2023-05-16 11:03:15.000000 CardGameBase-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-23 13:11:41.434572 CardGameBase-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1172 2023-05-23 13:11:23.000000 CardGameBase-1.0.4/setup.py
```

### Comparing `CardGameBase-1.0.3/CardGameBase/Card.py` & `CardGameBase-1.0.4/CardGameBase/Card.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 class Card:
     """
     Card Base Type with comparison features
     """
 
     def __init__(self,
-            symbol: str,
-            symbol_rank: int,
-            value: int,
-            _format: str = "{v}{s}",
-            special_value_format: str = None
-    ):
+                 symbol: str,
+                 symbol_rank: int,
+                 value: int,
+                 _format: str = "{v}{s}",
+                 special_value_format: str = None
+                 ):
         """
         Card Base Type with comparison features
 
         :param symbol: card symbol (like: spades, diamond, etc.)
         :param symbol_rank: symbol rank is required for comparing 2 cards
         :param value: card value
         :param _format: print format; {v} = value, {s} = symbol
@@ -24,15 +24,15 @@
         self.symbol_rank = symbol_rank
         self.value = value
         self._format = _format
         self.special_value_format = special_value_format
 
     def __add__(self, other) -> int:
         if isinstance(other, int):
-            return self.value*self.symbol_rank + other
+            return self.value * self.symbol_rank + other
 
         if not type(self) == type(other):
             raise TypeError(f"Cannot add type '{type(self)}' and '{type(other)}'")
 
         return self.value + other.value
 
     def __radd__(self, other):
```

### Comparing `CardGameBase-1.0.3/CardGameBase/Deck.py` & `CardGameBase-1.0.4/CardGameBase/Deck.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from typing import Iterable
-from random import shuffle
+from __future__ import annotations
+
+from typing import Iterable, List, Set
 from . import Card, EmptyDeck
+from random import shuffle
 import pickle
 
 
 class DeckConfig:
     """
     Deck config structure:
         __deck = {
             (symbol, symbol_rank): [
                 [value, special_value_format1],
                 ...
             ],
             ...
         }
     """
-    __deck_config: dict[tuple: list[list[int, str]]]
+    __deck_config: dict[tuple: List[List[int, str]]]
 
-    def __init__(self, deck_config: dict[tuple: list[list[int, str]]] = None):
+    def __init__(self, deck_config: dict[tuple: List[List[int, str]]] = None):
         if deck_config is None:
             deck_config = {}
-        self.__deck_config: dict[tuple: list[list[int, str]]] = deck_config
+        self.__deck_config: dict[tuple: List[List[int, str]]] = deck_config
 
     def add_card(self, symbol: str, symbol_rank: int, value: int, special_value_format: str = None) -> None:
         """
         Adds a card to the deck config
 
         :param symbol: Card symbol
         :param symbol_rank: symbol rank (for comparison when cards have the same value)
@@ -36,15 +38,15 @@
         if not self.__deck_config.get(key):
             self.__deck_config[key] = [[value, special_value_format]]
         else:
             # if [value, special_value_format] in self.__deck[key]:
             #    raise KeyError(f"a card with '{symbol=}', '{symbol_rank=}', '{value=}'; already exists!")
             self.__deck_config[key].append([value, special_value_format])
 
-    def get(self) -> dict[tuple: list[list[int, str]]]:
+    def get(self) -> dict[tuple: List[List[int, str]]]:
         """
         :return: gives back a deck config copy
         """
         return self.__deck_config.copy()
 
     def load(self, file: str) -> None:
         """
@@ -57,15 +59,15 @@
         """
         save deck config to file
         """
         with open(file, "wb") as f:
             pickle.dump(self.__deck_config, f)
 
     def __add__(self, other):
-        if not type(self) == type(other): # hasattr(other, "_DeckConfig__deck_config"):
+        if not type(self) == type(other):  # hasattr(other, "_DeckConfig__deck_config"):
             raise TypeError(f"Cannot add type '{type(self)}' and '{type(other)}'")
 
         new_deck = self.__deck_config.copy()
         for symbol, symbol_rank in other.get().keys():
             if new_deck.get((symbol, symbol_rank)):
                 new_deck[(symbol, symbol_rank)].append(other.get()[(symbol, symbol_rank)])
             else:
@@ -77,26 +79,26 @@
     def __init__(self, deck_configuration: DeckConfig = None):
         """
         :param deck_configuration: Deck Configuration
         """
         if deck_configuration is None:
             deck_configuration = DeckConfig()
         self.deck_configuration = deck_configuration
-        self.cards: list[Card] = []
+        self.cards: List[Card] = []
         self.__iterator = 0
 
         self.__create(self.deck_configuration)
 
     def __create(self, deck_config: DeckConfig) -> None:
         """
         Creates cards with the deck configuration
         """
         deck = deck_config.get()
         for card_symbol, card_symbol_rank in deck:
-            #print(deck[(card_symbol, card_symbol_rank)])
+            # print(deck[(card_symbol, card_symbol_rank)])
             for card_value, special_value_format in deck[(card_symbol, card_symbol_rank)]:
                 self.cards.append(Card(
                     card_symbol,
                     card_symbol_rank,
                     card_value,
                     special_value_format=special_value_format
                 ))
@@ -109,15 +111,15 @@
         # Since random can also create the same deck as before
         # would be extremely rare, but it could happen.
         # And if the deck is smaller than or equal to 1 this would
         # create a infinite loop
         while self.cards == cards_before and len(self.cards) > 1:
             shuffle(self.cards)
 
-    def get_card(self, amount: int = 1, put_to_bottom: bool = False) -> Card | list[Card]:
+    def get_card(self, amount: int = 1, put_to_bottom: bool = False) -> Card | List[Card]:
         """
         Returns the top card of the deck and removes the card from the deck
 
         :param amount: Amount of cards to draw
         :param put_to_bottom: Don't remove card when taking one from top and put it at the bottom
         :return: {amount} amount of cards
         """
@@ -128,15 +130,15 @@
         for i in range(amount):
             cards.append(self.cards.pop(0))
             if put_to_bottom:
                 self.cards.append(cards[-1])
 
         return cards[0] if len(cards) == 1 else cards
 
-    def add_card(self, cards: Card | list[Card] | DeckConfig) -> None:
+    def add_card(self, cards: Card | List[Card] | DeckConfig) -> None:
         """
         Adds card(s) to bottom of the deck
 
         :param cards: The card(s) to add
         """
         if isinstance(cards, list):
             self.cards.extend(cards)
@@ -149,15 +151,15 @@
         """
         Resets the Deck to the deck_configuration
         """
         self.cards = []
         self.__iterator = 0
         self.__create(self.deck_configuration)
 
-    def get_all_symbols(self) -> set[str]:
+    def get_all_symbols(self) -> Set[str]:
         """
         Returns a set of card symbols
         :return: a set of all card symbols
         """
         symbols = set()
         for card in self.cards:
             symbols.add(card.symbol)
```

### Comparing `CardGameBase-1.0.3/CardGameBase/Hand.py` & `CardGameBase-1.0.4/CardGameBase/Hand.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-from typing import Iterable
+from __future__ import annotations
 
+from typing import Iterable, List
 from . import Deck, Card
 
+
 class Hand:
-    def __init__(self, deck: Deck, rules: list[str] | str = None, check_with_rank: bool = False):
+    def __init__(self, deck: Deck, rules: List[str] | str = None, check_with_rank: bool = False):
         """
         :param deck: Deck from which cards will be drawn
         :param rules: rules for the hand; Please see the documentation for more info!
         """
-        self.hand: list[Card] = []
+        self.hand: List[Card] = []
         self.deck = deck
         self.rules = rules
         self.__iterator = 0
         self.check_with_rank = check_with_rank
 
     def draw(self, amount: int = 1, dont_take_away: bool = False) -> None:
         """
@@ -22,15 +24,15 @@
         :param dont_take_away: Don't take the cards away from deck and put to the bottom of the deck
         """
         if amount > 1:
             self.hand.extend(self.deck.get_card(amount, dont_take_away))
         else:
             self.hand.append(self.deck.get_card(amount, dont_take_away))
 
-    def empty(self, put_back: bool=True) -> None:
+    def empty(self, put_back: bool = True) -> None:
         """
         Removes cards from hand
 
         :param put_back: when true puts cards back to the deck
         """
         if put_back:
             self.deck.add_card(self.hand)
@@ -63,28 +65,28 @@
         if isinstance(self.rules, list):
             for rule in self.rules:
                 if eval(rule.format(**special_vars)):
                     if not on_invalid:
                         return rule
 
                     fixed_hand = on_invalid(self.hand, rule)
-                    if not fixed_hand is None:
+                    if fixed_hand is not None:
                         self.hand = fixed_hand
                     return rule
         else:
             if eval(self.rules.format(**special_vars)):
                 if not on_invalid:
                     return self.rules
 
                 fixed_hand = on_invalid(self.hand, self.rules)
-                if not fixed_hand is None:
+                if fixed_hand is not None:
                     self.hand = fixed_hand
                 return self.rules
 
-    def get_total_value(self, symbol : str = None, with_rank: bool = False) -> int:
+    def get_total_value(self, symbol: str = None, with_rank: bool = False) -> int:
         """
         Get the value of all cards in hand
         :param symbol: if set only cards with the given symbol are counted
         :param with_rank: when set the value of the card is multiplied by the cards symbol_rank
         :return: The sum
         """
         _sum = 0
```

### Comparing `CardGameBase-1.0.3/CardGameBase/Utility.py` & `CardGameBase-1.0.4/CardGameBase/Utility.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from . import DeckConfig, Deck
 
+
 def create_classic_deck() -> Deck:
     """
     Creates a classic deck with 52 cards of clubs, spades, diamonds and hearts (2 - Ace)
 
     :return: The Deck
     """
     symbols = [['c', 1], ['d', 2], ['h', 3], ['s', 4]]
```

### Comparing `CardGameBase-1.0.3/CardGameBase.egg-info/PKG-INFO` & `CardGameBase-1.0.4/CardGameBase.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: CardGameBase
-Version: 1.0.3
+Version: 1.0.4
 Summary: Card Game Base with basic deck and card class
 Home-page: https://github.com/DerSchinken/CardGameBase/
 Author: DerSchinken
 Maintainer: DerSchinken
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >= 3.6
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Card Game Base
 Create Card Games with ease
 # How  to install:
 `pip install CardGameBase`
```

### Comparing `CardGameBase-1.0.3/LICENSE` & `CardGameBase-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.3/PKG-INFO` & `CardGameBase-1.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: CardGameBase
-Version: 1.0.3
+Version: 1.0.4
 Summary: Card Game Base with basic deck and card class
 Home-page: https://github.com/DerSchinken/CardGameBase/
 Author: DerSchinken
 Maintainer: DerSchinken
 Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >= 3.6
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Card Game Base
 Create Card Games with ease
 # How  to install:
 `pip install CardGameBase`
```

### Comparing `CardGameBase-1.0.3/README.md` & `CardGameBase-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `CardGameBase-1.0.3/setup.py` & `CardGameBase-1.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 
 # Get requirements
 with open("requirements.txt", "r") as reqs:
     requirements = reqs.read().splitlines()
 
 setup(
     name="CardGameBase",
-    version="1.0.3",
+    version="1.0.4",
     # Major version 1
     # Minor version 0
     # Maintenance version 0
 
     author="DerSchinken",
     maintainer="DerSchinken",
     description="Card Game Base with basic deck and card class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=requirements,
-    python_requires=">= 3.6",
+    python_requires=">= 3.7",
     url="https://github.com/DerSchinken/CardGameBase/",
     keyword=[
         "Card Game",
         "Game",
         "Cards"
     ],
     classifiers=[
         'Intended Audience :: Developers',
 
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
-        "Programming Language :: Python :: 3.10"
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11"
     ]
 )
```

