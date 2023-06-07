# Comparing `tmp/apologies-0.1.8.tar.gz` & `tmp/apologies-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apologies-0.1.8.tar", last modified: Fri Mar 27 15:24:41 2020, max compression
+gzip compressed data, was "apologies-0.1.9.tar", last modified: Sun Mar 29 20:05:19 2020, max compression
```

## Comparing `apologies-0.1.8.tar` & `apologies-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11324 2020-03-18 13:23:51.584781 apologies-0.1.8/LICENSE
--rw-r--r--   0        0        0    11324 2020-03-18 13:23:51.584781 apologies-0.1.8/LICENSE
--rw-r--r--   0        0        0      791 2020-03-25 20:29:15.406519 apologies-0.1.8/PyPI.md
--rw-r--r--   0        0        0     1316 2020-03-27 15:24:24.016850 apologies-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       29 2020-03-18 19:22:37.786519 apologies-0.1.8/src/apologies/__init__.py
--rw-r--r--   0        0        0     2698 2020-03-26 17:05:30.034673 apologies-0.1.8/src/apologies/cli.py
--rw-r--r--   0        0        0     5011 2020-03-26 18:35:54.710822 apologies-0.1.8/src/apologies/demo.py
--rw-r--r--   0        0        0     6813 2020-03-27 15:18:23.048316 apologies-0.1.8/src/apologies/engine.py
--rw-r--r--   0        0        0    16811 2020-03-27 15:22:46.073030 apologies-0.1.8/src/apologies/game.py
--rw-r--r--   0        0        0    10358 2020-03-26 18:21:11.496354 apologies-0.1.8/src/apologies/render.py
--rw-r--r--   0        0        0    24778 2020-03-27 15:19:05.419612 apologies-0.1.8/src/apologies/rules.py
--rw-r--r--   0        0        0     3005 2020-03-27 15:18:23.062209 apologies-0.1.8/src/apologies/source.py
--rw-r--r--   0        0        0     1416 2020-03-26 18:02:22.590325 apologies-0.1.8/src/apologies/util.py
--rw-r--r--   0        0        0     1609 2020-03-27 15:24:41.102746 apologies-0.1.8/setup.py
--rw-r--r--   0        0        0     1802 2020-03-27 15:24:41.103073 apologies-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11324 2020-03-18 13:23:51.584781 apologies-0.1.9/LICENSE
+-rw-r--r--   0        0        0    11324 2020-03-18 13:23:51.584781 apologies-0.1.9/LICENSE
+-rw-r--r--   0        0        0      791 2020-03-25 20:29:15.406519 apologies-0.1.9/PyPI.md
+-rw-r--r--   0        0        0     1316 2020-03-29 20:05:03.831899 apologies-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       29 2020-03-18 19:22:37.786519 apologies-0.1.9/src/apologies/__init__.py
+-rw-r--r--   0        0        0     2698 2020-03-26 17:05:30.034673 apologies-0.1.9/src/apologies/cli.py
+-rw-r--r--   0        0        0     5011 2020-03-26 18:35:54.710822 apologies-0.1.9/src/apologies/demo.py
+-rw-r--r--   0        0        0     6813 2020-03-27 15:18:23.048316 apologies-0.1.9/src/apologies/engine.py
+-rw-r--r--   0        0        0    18386 2020-03-29 19:02:19.379870 apologies-0.1.9/src/apologies/game.py
+-rw-r--r--   0        0        0    10358 2020-03-26 18:21:11.496354 apologies-0.1.9/src/apologies/render.py
+-rw-r--r--   0        0        0    24582 2020-03-29 20:04:21.998636 apologies-0.1.9/src/apologies/rules.py
+-rw-r--r--   0        0        0     3005 2020-03-27 15:18:23.062209 apologies-0.1.9/src/apologies/source.py
+-rw-r--r--   0        0        0     1416 2020-03-26 18:02:22.590325 apologies-0.1.9/src/apologies/util.py
+-rw-r--r--   0        0        0     1609 2020-03-29 20:05:19.957817 apologies-0.1.9/setup.py
+-rw-r--r--   0        0        0     1802 2020-03-29 20:05:19.958140 apologies-0.1.9/PKG-INFO
```

### Comparing `apologies-0.1.8/LICENSE` & `apologies-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apologies-0.1.8/PyPI.md` & `apologies-0.1.9/PyPI.md`

 * *Files identical despite different names*

### Comparing `apologies-0.1.8/pyproject.toml` & `apologies-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apologies"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python code to play a game similar to Sorry"
 authors = ["Kenneth J. Pronovici <pronovic@ieee.org>"]
 license = "Apache-2.0"
 readme = "PyPI.md"
 homepage = "https://apologies.readthedocs.io"
 repository = "https://github.com/pronovic/apologies"
 include = ["LICENSE"]
```

### Comparing `apologies-0.1.8/src/apologies/cli.py` & `apologies-0.1.9/src/apologies/cli.py`

 * *Files identical despite different names*

### Comparing `apologies-0.1.8/src/apologies/demo.py` & `apologies-0.1.9/src/apologies/demo.py`

 * *Files identical despite different names*

### Comparing `apologies-0.1.8/src/apologies/engine.py` & `apologies-0.1.9/src/apologies/engine.py`

 * *Files identical despite different names*

### Comparing `apologies-0.1.8/src/apologies/game.py` & `apologies-0.1.9/src/apologies/game.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,16 +19,20 @@
 Attributes:
     MIN_PLAYERS(int): Minimum number of players in a game
     MAX_PLAYERS(int): Maximum number of players in a game
     PAWNS(int): Number of pawns per player
     SAFE_SQUARES(int): Number of safe squares for each color
     BOARD_SQUARES(int): Number of squares around the outside of the board
     ADULT_HAND(int): Number of cards in a player's hand for an adult mode game
-    DECK_COUNTS(dict): Dictionary from card name to number of cards in a standard deck
+    DECK_COUNTS(Dict[Card, int]): Dictionary from card name to number of cards in a standard deck
     DECK_SIZE(int): The total expected size of a complete deck
+    DRAW_AGAIN(Dict[Card, bool]): Whether each card results in a draw again action
+    CIRCLE(Dict[PlayerColor, Position]): The position of the start circle for each color
+    TURN(Dict[PlayerColor, Position()): The position of the turn square for each color, where forward movement turns into safe zone
+    SLIDE(Dict[PlayerColor, Tuple(int, int)): The slide start/end squares for each color
 """
 
 from __future__ import annotations  # see: https://stackoverflow.com/a/33533514/2907667
 
 import random
 from enum import Enum
 from typing import Dict, List, Optional
@@ -108,14 +112,29 @@
     CardType.CARD_10: 4,
     CardType.CARD_11: 4,
     CardType.CARD_12: 4,
     CardType.CARD_APOLOGIES: 4,
 }
 DECK_SIZE = sum(DECK_COUNTS.values())
 
+# Whether a card draws again
+DRAW_AGAIN = {
+    CardType.CARD_1: False,
+    CardType.CARD_2: True,
+    CardType.CARD_3: False,
+    CardType.CARD_4: False,
+    CardType.CARD_5: False,
+    CardType.CARD_7: False,
+    CardType.CARD_8: False,
+    CardType.CARD_10: False,
+    CardType.CARD_11: False,
+    CardType.CARD_12: False,
+    CardType.CARD_APOLOGIES: False,
+}
+
 
 @attr.s(frozen=True)
 class Card:
     """
     A card in a deck or in a player's hand.
 
     Attributes:
@@ -530,7 +549,32 @@
         self.history.append(History(action, player.color if player else None))
 
     def create_player_view(self, color: PlayerColor) -> PlayerView:
         """Return a player-specific view of the game, showing only the information a player would have available on their turn."""
         player = self.players[color].copy()
         opponents = {player.color: player.public_data() for player in self.players.values() if player.color != color}
         return PlayerView(player, opponents)
+
+
+# The start circles for each color
+CIRCLE = {
+    PlayerColor.RED: Position().move_to_square(4),
+    PlayerColor.BLUE: Position().move_to_square(19),
+    PlayerColor.YELLOW: Position().move_to_square(34),
+    PlayerColor.GREEN: Position().move_to_square(49),
+}
+
+# The turn squares for each color, where forward movement turns into the safe zone
+TURN = {
+    PlayerColor.RED: Position().move_to_square(2),
+    PlayerColor.BLUE: Position().move_to_square(17),
+    PlayerColor.YELLOW: Position().move_to_square(32),
+    PlayerColor.GREEN: Position().move_to_square(47),
+}
+
+# The slide start/end positions for each color
+SLIDE = {
+    PlayerColor.RED: ((1, 4), (9, 13)),
+    PlayerColor.BLUE: ((16, 19), (24, 28)),
+    PlayerColor.YELLOW: ((31, 34), (39, 43)),
+    PlayerColor.GREEN: ((46, 49), (54, 58)),
+}
```

### Comparing `apologies-0.1.8/src/apologies/render.py` & `apologies-0.1.9/src/apologies/render.py`

 * *Files identical despite different names*

### Comparing `apologies-0.1.8/src/apologies/rules.py` & `apologies-0.1.9/src/apologies/rules.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,65 +9,30 @@
 from typing import List, Optional
 
 import attr
 
 from .game import (
     ADULT_HAND,
     BOARD_SQUARES,
+    CIRCLE,
+    DRAW_AGAIN,
     SAFE_SQUARES,
+    SLIDE,
+    TURN,
     Card,
     CardType,
     Game,
     GameMode,
     Pawn,
     Player,
     PlayerColor,
     PlayerView,
     Position,
 )
 
-# The start circles for each color
-_CIRCLE = {
-    PlayerColor.RED: Position().move_to_square(4),
-    PlayerColor.BLUE: Position().move_to_square(19),
-    PlayerColor.YELLOW: Position().move_to_square(34),
-    PlayerColor.GREEN: Position().move_to_square(49),
-}
-
-# The turn squares for each color, where forward movement turns into the safe zone
-_TURN = {
-    PlayerColor.RED: Position().move_to_square(2),
-    PlayerColor.BLUE: Position().move_to_square(17),
-    PlayerColor.YELLOW: Position().move_to_square(32),
-    PlayerColor.GREEN: Position().move_to_square(47),
-}
-
-# The slide start/end positions for each color
-_SLIDE = {
-    PlayerColor.RED: ((1, 4), (9, 13)),
-    PlayerColor.BLUE: ((16, 19), (24, 28)),
-    PlayerColor.YELLOW: ((31, 34), (39, 43)),
-    PlayerColor.GREEN: ((46, 49), (54, 58)),
-}
-
-# Whether a card draws again
-_DRAW_AGAIN = {
-    CardType.CARD_1: False,
-    CardType.CARD_2: True,
-    CardType.CARD_3: False,
-    CardType.CARD_4: False,
-    CardType.CARD_5: False,
-    CardType.CARD_7: False,
-    CardType.CARD_8: False,
-    CardType.CARD_10: False,
-    CardType.CARD_11: False,
-    CardType.CARD_12: False,
-    CardType.CARD_APOLOGIES: False,
-}
-
 
 class ActionType(Enum):
     """Enumeration of all actions that a character can take."""
 
     MOVE_TO_START = "Move to start"  # Move a pawn back to its start area
     MOVE_TO_POSITION = "Move to position"  # Move a pawn to a specific position on the board
 
@@ -158,14 +123,38 @@
             elif card.cardtype == CardType.CARD_12:
                 moves += BoardRules._construct_legal_moves_12(color, card, pawn, all_pawns)
             elif card.cardtype == CardType.CARD_APOLOGIES:
                 moves += BoardRules._construct_legal_moves_apologies(color, card, pawn, all_pawns)
         BoardRules._augment_with_slides(all_pawns, moves)
         return moves
 
+    @staticmethod
+    def distance_to_home(pawn: Pawn) -> int:
+        """Return the distance to home for this pawn, a number of squares when moving forward."""
+        if pawn.position.home:
+            return 0
+        elif pawn.position.start:
+            return 65
+        elif pawn.position.safe is not None:
+            return SAFE_SQUARES - pawn.position.safe
+        else:
+            circle = CIRCLE[pawn.color].square
+            turn = TURN[pawn.color].square
+            square = pawn.position.square
+            square_to_corner = BOARD_SQUARES - square  # type: ignore
+            corner_to_turn = turn
+            turn_to_home = SAFE_SQUARES + 1
+            total = square_to_corner + corner_to_turn + turn_to_home  # type: ignore
+            if turn < square < circle:  # type: ignore
+                return total
+            if total < 65:
+                return total
+            else:
+                return total - 60
+
     # noinspection PyChainedComparisons
     # pylint: disable=too-many-branches,too-many-return-statements,line-too-long
     @staticmethod
     def _position(color: PlayerColor, position: Position, squares: int) -> Position:
         """
         Calculate the new position for a forward or backwards move, taking into account safe zone turns but disregarding slides.
         """
@@ -181,22 +170,22 @@
                     return position.copy().move_to_home()
                 else:
                     raise ValueError("Pawn cannot move past home.")
             else:  # squares < 0
                 if position.safe + squares >= 0:
                     return position.copy().move_to_safe(position.safe + squares)
                 else:  # handle moving back out of the safe area
-                    return BoardRules._position(color, position.copy().move_to_square(_TURN[color].square), squares + position.safe + 1)  # type: ignore
+                    return BoardRules._position(color, position.copy().move_to_square(TURN[color].square), squares + position.safe + 1)  # type: ignore
         elif position.square is not None:
             if squares == 0:
                 return position.copy()
             elif squares > 0:
                 if position.square + squares < BOARD_SQUARES:
-                    if position.square <= _TURN[color].square and position.square + squares > _TURN[color].square:  # type: ignore
-                        return BoardRules._position(color, position.copy().move_to_safe(0), squares - (_TURN[color].square - position.square) - 1)  # type: ignore
+                    if position.square <= TURN[color].square and position.square + squares > TURN[color].square:  # type: ignore
+                        return BoardRules._position(color, position.copy().move_to_safe(0), squares - (TURN[color].square - position.square) - 1)  # type: ignore
                     else:
                         return position.copy().move_to_square(position.square + squares)
                 else:  # handle turning the corner
                     return BoardRules._position(
                         color, position.copy().move_to_square(0), squares - (BOARD_SQUARES - position.square)
                     )
             else:  # squares < 0
@@ -289,22 +278,22 @@
 
     @staticmethod
     def _move_circle(color: PlayerColor, card: Card, pawn: Pawn, all_pawns: List[Pawn]) -> List[Move]:
         # For start-related cards, a pawn in the start area can move to the associated
         # circle position if that position is not occupied by another pawn of the same color.
         moves: List[Move] = []
         if pawn.position.start:
-            conflict = BoardRules._find_pawn(all_pawns, _CIRCLE[color])
+            conflict = BoardRules._find_pawn(all_pawns, CIRCLE[color])
             if not conflict:
-                moves.append(Move(card, actions=[Action(ActionType.MOVE_TO_POSITION, pawn, _CIRCLE[color].copy())]))
+                moves.append(Move(card, actions=[Action(ActionType.MOVE_TO_POSITION, pawn, CIRCLE[color].copy())]))
             elif conflict and conflict.color != color:
                 moves.append(
                     Move(
                         card,
-                        actions=[Action(ActionType.MOVE_TO_POSITION, pawn, _CIRCLE[color].copy())],
+                        actions=[Action(ActionType.MOVE_TO_POSITION, pawn, CIRCLE[color].copy())],
                         side_effects=[Action(ActionType.MOVE_TO_START, conflict)],
                     )
                 )
         return moves
 
     @staticmethod
     def _move_simple(color: PlayerColor, card: Card, pawn: Pawn, all_pawns: List[Pawn], squares: int) -> List[Move]:
@@ -395,15 +384,15 @@
     @staticmethod
     def _augment_with_slides(all_pawns: List[Pawn], moves: List[Move]) -> None:
         """Augument any legal moves with additional side-effects that occur as a result of slides."""
         for move in moves:
             for action in move.actions:
                 if action.actiontype == ActionType.MOVE_TO_POSITION:  # look at any move to a position on the board
                     for color in [color for color in PlayerColor if color != action.pawn.color]:  # any color other than the pawn's
-                        for (start, end) in _SLIDE[color]:  # look at all slides with this color
+                        for (start, end) in SLIDE[color]:  # look at all slides with this color
                             if action.position.square == start:  # if the pawn landed on the start of the slide
                                 action.position.move_to_square(end)  # move the pawn to the end of the slide
                                 for square in range(start + 1, end + 1):  # and then bump any pawns that were already on the slide
                                     # Note: in this one case, a pawn can bump another pawn of the same color
                                     pawn = BoardRules._find_pawn(all_pawns, Position().move_to_square(square))
                                     if pawn:
                                         bump = Action(ActionType.MOVE_TO_START, pawn)
@@ -428,15 +417,15 @@
     @_board_rules.default
     def _default_board_rules(self) -> BoardRules:
         return BoardRules()
 
     # noinspection PyMethodMayBeStatic
     def draw_again(self, card: Card) -> bool:
         """Whether the player gets to draw again based on the passed-in card."""
-        return _DRAW_AGAIN[card.cardtype]
+        return DRAW_AGAIN[card.cardtype]
 
     def start_game(self, game: Game) -> None:
         """
         Start the game.
 
         Args:
             game(Game): Game to operate on
@@ -523,11 +512,11 @@
                     pawn.position.move_to_position(action.position)
         return result
 
     @staticmethod
     def _setup_adult_mode(game: Game) -> None:
         """Setup adult mode at the start of the game, which moves some pieces and deals some cards."""
         for player in game.players.values():
-            player.pawns[0].position.move_to_position(_CIRCLE[player.color])
+            player.pawns[0].position.move_to_position(CIRCLE[player.color])
         for _ in range(ADULT_HAND):
             for player in game.players.values():
                 player.hand.append(game.deck.draw())
```

### Comparing `apologies-0.1.8/src/apologies/source.py` & `apologies-0.1.9/src/apologies/source.py`

 * *Files identical despite different names*

### Comparing `apologies-0.1.8/src/apologies/util.py` & `apologies-0.1.9/src/apologies/util.py`

 * *Files identical despite different names*

### Comparing `apologies-0.1.8/setup.py` & `apologies-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['attrs>=19.3.0,<20.0.0',
  'cattrs>=1.0.0,<2.0.0',
  'orjson>=2.6.1,<3.0.0',
  'pendulum>=2.1.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'apologies',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Python code to play a game similar to Sorry',
     'long_description': '# Apologies Python Library\n\n![](https://img.shields.io/pypi/l/apologies.svg)\n![](https://img.shields.io/pypi/wheel/apologies.svg)\n![](https://img.shields.io/pypi/pyversions/apologies.svg)\n![](https://github.com/pronovic/apologies/workflows/Test%20Suite/badge.svg)\n\n[Apologies](https://gitub.com/pronovic/apologies) is a Python library that\nimplements a game similar to the [Sorry](https://en.wikipedia.org/wiki/Sorry!_(game)) board \ngame.  It includes a console demo that plays the game with automated players,\nintended for use by developers and not by end users.\n\nIt also serves as a complete example of how to manage a modern (circa 2020)\nPython project, including style checks, code formatting, integration with\nIntelliJ, CI builds at GitHub, and integration with PyPI and Read the Docs.\n',
     'author': 'Kenneth J. Pronovici',
     'author_email': 'pronovic@ieee.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://apologies.readthedocs.io',
```

### Comparing `apologies-0.1.8/PKG-INFO` & `apologies-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apologies
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python code to play a game similar to Sorry
 Home-page: https://apologies.readthedocs.io
 License: Apache-2.0
 Author: Kenneth J. Pronovici
 Author-email: pronovic@ieee.org
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
```

