# Comparing `tmp/auraboros-0.9.0a0.tar.gz` & `tmp/auraboros-1.0.0a0.tar.gz`

## Comparing `auraboros-0.9.0a0.tar` & `auraboros-1.0.0a0.tar`

### file list

```diff
@@ -1,86 +1,130 @@
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/Pipfile
--rw-r--r--   0        0        0    63551 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/Pipfile.lock
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/README.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/.vscode/settings.json
--rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/fonts/misaki_gothic.ttf
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/enemy_a.piskel
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/enemy_a.png
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/enemy_b.piskel
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/enemy_b.png
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/explosion_a.piskel
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/explosion_a.png
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/explosion_b.png
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/fighter_a.piskel
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/fighter_a.png
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/icon.ico
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/laser1.png
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/scoutdisk.piskel
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/scoutdisk.png
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot1.piskel
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot1.png
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot2.piskel
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot2.png
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot3.png
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot4.png
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot5.piskel
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot5.png
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot6.piskel
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot6.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot7.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/shot8.png
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/imgs/terrain_rock.png
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/level_data/debug1/level.json
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/level_data/debug1/patterns.json
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/level_data/stage1/level.json
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/level_data/stage1/patterns.json
--rw-r--r--   0        0        0    78688 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/deathse2.wav
--rw-r--r--   0        0        0   191648 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/deathse3.wav
--rw-r--r--   0        0        0    28264 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/deathse4.wav
--rw-r--r--   0        0        0    21586 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/explosion1.wav
--rw-r--r--   0        0        0   352960 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/explosion2.wav
--rw-r--r--   0        0        0   150572 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/laser.wav
--rw-r--r--   0        0        0   150610 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/laser2.wav
--rw-r--r--   0        0        0    21360 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/shot1.wav
--rw-r--r--   0        0        0  5177872 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/music/bgm1.wav
--rw-r--r--   0        0        0   789664 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/assets/sounds/music/gameover.wav
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/Makefile
--rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/make.bat
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/source/conf.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/source/index.rst
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/source/locale/de/LC_MESSAGES/index.po
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/docs/source/locale/ja/LC_MESSAGES/index.po
--rw-r--r--   0        0        0    43792 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/examples/eightrail.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/examples/example.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/examples/helloworld/engine.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/examples/helloworld/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/__init__.py
--rw-r--r--   0        0        0     5391 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/animation.py
--rw-r--r--   0        0        0     5196 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/animation2.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/engine.py
--rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/entity.py
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/gameinput.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/gameinput2.py
--rw-r--r--   0        0        0     9333 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/gamelevel.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/gamescene.py
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/gametext.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/global_.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/schedule.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/schedule2.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/sound.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/terrain.py
--rw-r--r--   0        0        0    15249 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/ui.py
--rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/auraboros/utilities.py
--rw-r--r--   0        0        0     6401 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/animation.py
--rw-r--r--   0        0        0     3569 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/gamemenu.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/init_for_dev.py
--rw-r--r--   0        0        0     5500 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/keyboard.py
--rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/assets/fonts/misaki_gothic.ttf
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/src/debugs/assets/imgs/testsprite.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/tests/__init__.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/tests/test_gameinput.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/tests/test_ui.py
--rw-r--r--   0        0        0     4254 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/LICENSE
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/pyproject.toml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 auraboros-0.9.0a0/PKG-INFO
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/Pipfile
+-rw-r--r--   0        0        0    82156 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/Pipfile.lock
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/README.jp.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/README.md
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/mkdocs.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/.vscode/settings.json
+-rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/fonts/misaki_gothic.ttf
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/enemy_a.piskel
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/enemy_a.png
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/enemy_b.piskel
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/enemy_b.png
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/explosion_a.piskel
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/explosion_a.png
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/explosion_b.png
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/fighter_a.piskel
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/fighter_a.png
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/icon.ico
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/laser1.png
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/scoutdisk.piskel
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/scoutdisk.png
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot1.piskel
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot1.png
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot2.piskel
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot2.png
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot3.png
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot4.png
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot5.piskel
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot5.png
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot6.piskel
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot6.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot7.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/shot8.png
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/imgs/terrain_rock.png
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/level_data/debug1/level.json
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/level_data/debug1/patterns.json
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/level_data/stage1/level.json
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/level_data/stage1/patterns.json
+-rw-r--r--   0        0        0    78688 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/sounds/deathse2.wav
+-rw-r--r--   0        0        0   191648 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/sounds/deathse3.wav
+-rw-r--r--   0        0        0    28264 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/sounds/deathse4.wav
+-rw-r--r--   0        0        0    21586 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/sounds/explosion1.wav
+-rw-r--r--   0        0        0   352960 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/sounds/explosion2.wav
+-rw-r--r--   0        0        0   150572 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/sounds/laser.wav
+-rw-r--r--   0        0        0   150610 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/sounds/laser2.wav
+-rw-r--r--   0        0        0    21360 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/sounds/shot1.wav
+-rw-r--r--   0        0        0  5177872 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/sounds/music/bgm1.wav
+-rw-r--r--   0        0        0   789664 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/assets/sounds/music/gameover.wav
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/__init__.py
+-rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/__main__.py
+-rw-r--r--   0        0        0    11150 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/animation.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/core.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/default.frag
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/default.vert
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/designpattern.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/engine.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/gamecamera.py
+-rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/gameinput.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/gamescene.py
+-rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/gametext.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/getasset_order.json
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/particle.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/schedule.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/shader.py
+-rw-r--r--   0        0        0    36537 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/ui.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/__pyinstaller/hook-auraboros.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/__pyinstaller/test_auraboros_packaging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/ecs/__init__.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/ecs/common.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/ecs/world.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/helloworld.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/setup_syspath.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/shooting_game.py
+-rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/ui_showcase.py
+-rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/assets/fonts/misaki_gothic.ttf
+-rw-r--r--   0        0        0  1133216 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/assets/fonts/PixelMplus/PixelMplus10-Regular.ttf
+-rw-r--r--   0        0        0  1274396 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/assets/fonts/PixelMplus/PixelMplus12-Regular.ttf
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/assets/fonts/PixelMplus/README.txt
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/LICENSE_E
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/LICENSE_J
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/README_E
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/README_J
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/assets/imgs/testsprite.png
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/animate_msgbox.py
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/animation.py
+-rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/animationimage.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/entity.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/gametext.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/helloworld.py
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/keyboard.py
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/keyframe_animation.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/menu_ui.py
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/mouse.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/msgbox.py
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/particle.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/scene_transition.py
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/schedule.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/shader.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/stopwatch.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/textinput.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/ui_example1.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/examples/deprecated/vignette.frag
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/utils/__init__.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/utils/coordinate.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/utils/misc.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/utils/path.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/utils/sequence.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/utils/string.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/src/auraboros/utils/surface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/__init__.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_animation.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_ecs.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_gameinput.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_gametext.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_particle.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_shader.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_ui.py
+-rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/assets/fonts/misaki_gothic.ttf
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/assets/imgs/testsprite.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_utils/test_path.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_utils/test_sequence.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/tests/test_utils/test_string.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/LICENSE
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/pyproject.toml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 auraboros-1.0.0a0/PKG-INFO
```

### Comparing `auraboros-0.9.0a0/Pipfile.lock` & `auraboros-1.0.0a0/Pipfile.lock`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7573302469135802%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'4eefea9475b87740d4d5dc0d44b0f2a27f9f8c5444a155bc56754c0e5c02525e'}, 'requires': "*

 * *            "{'python_version': '3.11'}}",*

 * * "'default'": "{'pygame': {'hashes': "*

 * *              "['sha256:00ecd4688ee25d5d4cf48eddab18749a9bb2b382772f7fa8a987e4d21026c603', "*

 * *              "'sha256:075c1282b1d307669c8ef29942564b91acb85623bedba3bfb841079d539ded31', "*

 * *              "'sha256:13511c7c29f0fc23636f3b95a96ab45f964e84073e7e27dc602a479cd274d89a', "*

 * *              "'sha256 […]*

```diff
@@ -1,491 +1,209 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "f1f28537dd6842fe8e7648402331b08a00640808dde68153ea572045ec6bdbb9"
+            "sha256": "4eefea9475b87740d4d5dc0d44b0f2a27f9f8c5444a155bc56754c0e5c02525e"
         },
         "pipfile-spec": 6,
         "requires": {
-            "python_version": "3.10.8"
+            "python_version": "3.11"
         },
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
-        "alabaster": {
-            "hashes": [
-                "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
-                "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==0.7.13"
-        },
-        "attrs": {
-            "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
-        },
-        "babel": {
-            "hashes": [
-                "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
-                "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.12.1"
-        },
-        "certifi": {
-            "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
-        },
-        "charset-normalizer": {
+        "glcontext": {
             "hashes": [
-                "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
-                "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
-                "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
-                "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
-                "sha256:0ca564606d2caafb0abe6d1b5311c2649e8071eb241b2d64e75a0d0065107e62",
-                "sha256:10c93628d7497c81686e8e5e557aafa78f230cd9e77dd0c40032ef90c18f2230",
-                "sha256:11d117e6c63e8f495412d37e7dc2e2fff09c34b2d09dbe2bee3c6229577818be",
-                "sha256:11d3bcb7be35e7b1bba2c23beedac81ee893ac9871d0ba79effc7fc01167db6c",
-                "sha256:12a2b561af122e3d94cdb97fe6fb2bb2b82cef0cdca131646fdb940a1eda04f0",
-                "sha256:12d1a39aa6b8c6f6248bb54550efcc1c38ce0d8096a146638fd4738e42284448",
-                "sha256:1435ae15108b1cb6fffbcea2af3d468683b7afed0169ad718451f8db5d1aff6f",
-                "sha256:1c60b9c202d00052183c9be85e5eaf18a4ada0a47d188a83c8f5c5b23252f649",
-                "sha256:1e8fcdd8f672a1c4fc8d0bd3a2b576b152d2a349782d1eb0f6b8e52e9954731d",
-                "sha256:20064ead0717cf9a73a6d1e779b23d149b53daf971169289ed2ed43a71e8d3b0",
-                "sha256:21fa558996782fc226b529fdd2ed7866c2c6ec91cee82735c98a197fae39f706",
-                "sha256:22908891a380d50738e1f978667536f6c6b526a2064156203d418f4856d6e86a",
-                "sha256:3160a0fd9754aab7d47f95a6b63ab355388d890163eb03b2d2b87ab0a30cfa59",
-                "sha256:322102cdf1ab682ecc7d9b1c5eed4ec59657a65e1c146a0da342b78f4112db23",
-                "sha256:34e0a2f9c370eb95597aae63bf85eb5e96826d81e3dcf88b8886012906f509b5",
-                "sha256:3573d376454d956553c356df45bb824262c397c6e26ce43e8203c4c540ee0acb",
-                "sha256:3747443b6a904001473370d7810aa19c3a180ccd52a7157aacc264a5ac79265e",
-                "sha256:38e812a197bf8e71a59fe55b757a84c1f946d0ac114acafaafaf21667a7e169e",
-                "sha256:3a06f32c9634a8705f4ca9946d667609f52cf130d5548881401f1eb2c39b1e2c",
-                "sha256:3a5fc78f9e3f501a1614a98f7c54d3969f3ad9bba8ba3d9b438c3bc5d047dd28",
-                "sha256:3d9098b479e78c85080c98e1e35ff40b4a31d8953102bb0fd7d1b6f8a2111a3d",
-                "sha256:3dc5b6a8ecfdc5748a7e429782598e4f17ef378e3e272eeb1340ea57c9109f41",
-                "sha256:4155b51ae05ed47199dc5b2a4e62abccb274cee6b01da5b895099b61b1982974",
-                "sha256:49919f8400b5e49e961f320c735388ee686a62327e773fa5b3ce6721f7e785ce",
-                "sha256:53d0a3fa5f8af98a1e261de6a3943ca631c526635eb5817a87a59d9a57ebf48f",
-                "sha256:5f008525e02908b20e04707a4f704cd286d94718f48bb33edddc7d7b584dddc1",
-                "sha256:628c985afb2c7d27a4800bfb609e03985aaecb42f955049957814e0491d4006d",
-                "sha256:65ed923f84a6844de5fd29726b888e58c62820e0769b76565480e1fdc3d062f8",
-                "sha256:6734e606355834f13445b6adc38b53c0fd45f1a56a9ba06c2058f86893ae8017",
-                "sha256:6baf0baf0d5d265fa7944feb9f7451cc316bfe30e8df1a61b1bb08577c554f31",
-                "sha256:6f4f4668e1831850ebcc2fd0b1cd11721947b6dc7c00bf1c6bd3c929ae14f2c7",
-                "sha256:6f5c2e7bc8a4bf7c426599765b1bd33217ec84023033672c1e9a8b35eaeaaaf8",
-                "sha256:6f6c7a8a57e9405cad7485f4c9d3172ae486cfef1344b5ddd8e5239582d7355e",
-                "sha256:7381c66e0561c5757ffe616af869b916c8b4e42b367ab29fedc98481d1e74e14",
-                "sha256:73dc03a6a7e30b7edc5b01b601e53e7fc924b04e1835e8e407c12c037e81adbd",
-                "sha256:74db0052d985cf37fa111828d0dd230776ac99c740e1a758ad99094be4f1803d",
-                "sha256:75f2568b4189dda1c567339b48cba4ac7384accb9c2a7ed655cd86b04055c795",
-                "sha256:78cacd03e79d009d95635e7d6ff12c21eb89b894c354bd2b2ed0b4763373693b",
-                "sha256:80d1543d58bd3d6c271b66abf454d437a438dff01c3e62fdbcd68f2a11310d4b",
-                "sha256:830d2948a5ec37c386d3170c483063798d7879037492540f10a475e3fd6f244b",
-                "sha256:891cf9b48776b5c61c700b55a598621fdb7b1e301a550365571e9624f270c203",
-                "sha256:8f25e17ab3039b05f762b0a55ae0b3632b2e073d9c8fc88e89aca31a6198e88f",
-                "sha256:9a3267620866c9d17b959a84dd0bd2d45719b817245e49371ead79ed4f710d19",
-                "sha256:a04f86f41a8916fe45ac5024ec477f41f886b3c435da2d4e3d2709b22ab02af1",
-                "sha256:aaf53a6cebad0eae578f062c7d462155eada9c172bd8c4d250b8c1d8eb7f916a",
-                "sha256:abc1185d79f47c0a7aaf7e2412a0eb2c03b724581139193d2d82b3ad8cbb00ac",
-                "sha256:ac0aa6cd53ab9a31d397f8303f92c42f534693528fafbdb997c82bae6e477ad9",
-                "sha256:ac3775e3311661d4adace3697a52ac0bab17edd166087d493b52d4f4f553f9f0",
-                "sha256:b06f0d3bf045158d2fb8837c5785fe9ff9b8c93358be64461a1089f5da983137",
-                "sha256:b116502087ce8a6b7a5f1814568ccbd0e9f6cfd99948aa59b0e241dc57cf739f",
-                "sha256:b82fab78e0b1329e183a65260581de4375f619167478dddab510c6c6fb04d9b6",
-                "sha256:bd7163182133c0c7701b25e604cf1611c0d87712e56e88e7ee5d72deab3e76b5",
-                "sha256:c36bcbc0d5174a80d6cccf43a0ecaca44e81d25be4b7f90f0ed7bcfbb5a00909",
-                "sha256:c3af8e0f07399d3176b179f2e2634c3ce9c1301379a6b8c9c9aeecd481da494f",
-                "sha256:c84132a54c750fda57729d1e2599bb598f5fa0344085dbde5003ba429a4798c0",
-                "sha256:cb7b2ab0188829593b9de646545175547a70d9a6e2b63bf2cd87a0a391599324",
-                "sha256:cca4def576f47a09a943666b8f829606bcb17e2bc2d5911a46c8f8da45f56755",
-                "sha256:cf6511efa4801b9b38dc5546d7547d5b5c6ef4b081c60b23e4d941d0eba9cbeb",
-                "sha256:d16fd5252f883eb074ca55cb622bc0bee49b979ae4e8639fff6ca3ff44f9f854",
-                "sha256:d2686f91611f9e17f4548dbf050e75b079bbc2a82be565832bc8ea9047b61c8c",
-                "sha256:d7fc3fca01da18fbabe4625d64bb612b533533ed10045a2ac3dd194bfa656b60",
-                "sha256:dd5653e67b149503c68c4018bf07e42eeed6b4e956b24c00ccdf93ac79cdff84",
-                "sha256:de5695a6f1d8340b12a5d6d4484290ee74d61e467c39ff03b39e30df62cf83a0",
-                "sha256:e0ac8959c929593fee38da1c2b64ee9778733cdf03c482c9ff1d508b6b593b2b",
-                "sha256:e1b25e3ad6c909f398df8921780d6a3d120d8c09466720226fc621605b6f92b1",
-                "sha256:e633940f28c1e913615fd624fcdd72fdba807bf53ea6925d6a588e84e1151531",
-                "sha256:e89df2958e5159b811af9ff0f92614dabf4ff617c03a4c1c6ff53bf1c399e0e1",
-                "sha256:ea9f9c6034ea2d93d9147818f17c2a0860d41b71c38b9ce4d55f21b6f9165a11",
-                "sha256:f645caaf0008bacf349875a974220f1f1da349c5dbe7c4ec93048cdc785a3326",
-                "sha256:f8303414c7b03f794347ad062c0516cee0e15f7a612abd0ce1e25caf6ceb47df",
-                "sha256:fca62a8301b605b954ad2e9c3666f9d97f63872aa4efcae5492baca2056b74ab"
-            ],
-            "markers": "python_full_version >= '3.7.0'",
-            "version": "==3.1.0"
-        },
-        "colorama": {
-            "hashes": [
-                "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
-                "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
-            "version": "==0.4.6"
-        },
-        "docutils": {
-            "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.19"
-        },
-        "exceptiongroup": {
-            "hashes": [
-                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
-                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
-            ],
-            "markers": "python_version < '3.11'",
-            "version": "==1.1.1"
-        },
-        "idna": {
-            "hashes": [
-                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
-                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
-            ],
-            "markers": "python_version >= '3.5'",
-            "version": "==3.4"
-        },
-        "imagesize": {
-            "hashes": [
-                "sha256:0d8d18d08f840c19d0ee7ca1fd82490fdc3729b7ac93f49870406ddde8ef8d8b",
-                "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.4.1"
-        },
-        "iniconfig": {
-            "hashes": [
-                "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
-                "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.0.0"
-        },
-        "jinja2": {
-            "hashes": [
-                "sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852",
-                "sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==3.1.2"
-        },
-        "livereload": {
-            "hashes": [
-                "sha256:776f2f865e59fde56490a56bcc6773b6917366bce0c267c60ee8aaf1a0959869",
-                "sha256:ad4ac6f53b2d62bb6ce1a5e6e96f1f00976a32348afedcb4b6d68df2a1d346e4"
-            ],
-            "version": "==2.6.3"
-        },
-        "markupsafe": {
-            "hashes": [
-                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
-                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
-                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
-                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
-                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
-                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
-                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
-                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
-                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
-                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
-                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
-                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
-                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
-                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
-                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
-                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
-                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
-                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
-                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
-                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
-                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
-                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
-                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
-                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
-                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
-                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
-                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
-                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
-                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
-                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
-                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
-                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
-                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
-                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
-                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
-                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
-                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
-                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
-                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
-                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
-                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
-                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
-                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
-                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
-                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
-                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
-                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
-                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
-                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
-                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.1.2"
-        },
-        "packaging": {
-            "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==23.0"
-        },
-        "pluggy": {
-            "hashes": [
-                "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
-                "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==1.0.0"
-        },
-        "pygame": {
-            "hashes": [
-                "sha256:033352321cc49d60fdc3c3ae4b3e10ecb6614846fb2eb3453c729aba48a2874d",
-                "sha256:0a664cd6c50870f6749c389a8844318afc8a2d02f8cb7b05d67930fdf99252bd",
-                "sha256:0ec8e691407b6c91525b2d7c8386fd6232b97d8f8c33d134ec0c0165b1d52c24",
-                "sha256:101c57141d705ca1930377c324d2c7acd3099f1b4ac676981bdf5d5b329842c8",
-                "sha256:17730a2ed1001e5876745702c92906ad31ecedc13825efba56a0cba92e273b7a",
-                "sha256:1dc89d825e0ccba5ba3605abbd83be1401e0a32de7ab64b9647a6bb1ecb0a4f7",
-                "sha256:1eda9f30d376d4205e8204e542ab1348dcbb31755c8ba38772e48a3b2f91b2fc",
-                "sha256:228514c0d034c840b8ee6bf99185df34ac15e6a6a99684b8a3900124417c8d8f",
-                "sha256:23bd3c3a6d4e8acddee2297d609dbc5953d6ba99b0f0cc5ccc2f567889db3785",
-                "sha256:246f75f67d2ad4c2dad21b1f35c6092d67c4c0db13b2fa0a42d794e6e2794f47",
-                "sha256:250b3ec3f90b05ad50cb0070d994a0a1f39fffe8181fc9508b8749884c313431",
-                "sha256:25c1b1819211aaa0f98264e6b670a496a9975079d5ae2dffd304b0aca6b1aa3c",
-                "sha256:32bdf1d5d9e0763779d0b915d4617253949a6c118c4c6b5ae1a77cf1df964e4c",
-                "sha256:35f5a9cc7a9a2ea3d048e418e79f30e1506cb47015939330903026c636761aab",
-                "sha256:385163fd1ed8809a72be68fddc9c76876c304e8712695aff2ea49adf3831caf9",
-                "sha256:38642c6cc6477db6ebddd52be39bad0a9e19cf097f83feaaf8e7573b9a9d2405",
-                "sha256:3d035ba196c258876a87451fa7de65b62c087d7016e51000e8d95bc67c8584f7",
-                "sha256:3e9535cf1af0c6ca38d94e0b492fc41057d7bf05e9bd64d3ed3e216d336d6d11",
-                "sha256:3ee86606c6c7f61176ed24b427fa230fe4fc9f552aa555b8db21ddb608b4ce88",
-                "sha256:43f238229b3a9e5692ba5a31638f1c148257b37a49ef21f03b23b34d7f00b2d9",
-                "sha256:4b334f6dd6c1412dd4b161a8562b7a422db957f67b7eb93e927606e2dd435882",
-                "sha256:4db1b103025fd4b451dfa409c0da16d2ff31714ae82bdf45b1434863cd69370b",
-                "sha256:4f79a3c5e7f24474d6e722d597ee03d2b0d17958c77d4307787147cf339b4ad9",
-                "sha256:525e11a2b9182ec84d690634016009e382ab8b488593c3f150a0b8aae28aa165",
-                "sha256:53e9418c457fa549294feee7947bc0b24b048b4eba133f0e757dd2348d15af3b",
-                "sha256:555234ed6b08242af95406fd3eb43255c3ce8e915e8c751f2d411bd40d574df4",
-                "sha256:57180b3aabbe17d8017aa724887019943d96ea69810f4315f5c1b7d4f64861f9",
-                "sha256:59a1e473c627acf369b30bb52fb5f39d1f68f8c204aa857578b72f07a23c952b",
-                "sha256:619eed2d97f28af9d4cdb217a5517fd6f59b873f2f1d31b4489ed852b9a175c3",
-                "sha256:653ec5102b9cb13a24e26663a81d7810790e56b88113b90aa5fdca681c01a5b9",
-                "sha256:6c5d33355dfb66382bcac1fcf3db64ba71bc9e97082db3ae45a7a0d335e73268",
-                "sha256:6ccde93b51d2393216f98e8f81cf5cc628513d837c89dcf5b588f52031659c09",
-                "sha256:703d5def9d4dbe9c358f63151bee4a55e328dd7737e692f52522bc44be7c7c8c",
-                "sha256:740b9f311c693b00d86a89cc6846afc1d1e013b006975eb8be0b18d5481c5b32",
-                "sha256:774233845099d632de676ad4d4dd08ba27ebce5bfa550b1dc9f6cce145e21c35",
-                "sha256:788717d0b9a0d0828a763381e1eb6a127ceef815f9a91ff52217ed4b78df62fc",
-                "sha256:82e5806fd797bd1b27fae705683f6822ae5276ec9cda42e6e21bba61985b763a",
-                "sha256:8308b21804d137a3b7cafbd020d2159eb5bcc18ffc9c3993b20311069c326a2c",
-                "sha256:84fad9538012f1d6b298dcf690c4336e0317fe97ac10993b4d847ff547e919dd",
-                "sha256:858d3968aebaca5015ef0ec82c513114a3c3fe64ce910222cfa852a39f03b135",
-                "sha256:884b92c9cbf0bfaf8b8dd0f75a746613c55447d307ddd1addf903709b3b9f89f",
-                "sha256:90931a210325274184860d898df4e87a0972654edbb2a6185afcdce32244dfb6",
-                "sha256:910678441d02c3b55ac59fcbc4220a824b094407de084734b5d84e0900d6448b",
-                "sha256:932034e1738873a55c4e2eb83b6e8c03f9a55feaa6a04a7da7b1e0e5a5050b4a",
-                "sha256:9ccac73a8c913809ba2c1408d750abf14e45666b3c83493370441c52e99222b4",
-                "sha256:a1d737db18f4c94b620613c6a047a3a1eecc0f36df7d5da4070de575930cc5f0",
-                "sha256:a5afd712bd7307d034e6940f3025c4b769656fd4cbb38fbdbd6af0f93d6c8386",
-                "sha256:a5e83bd89da26f8360e02d5de2d2575981b0ebad81ea6d48aba610dabf167b88",
-                "sha256:a7390815dad55a2db9f8daac6f2c2e593801daea2d674433a72b91ea1caee0d3",
-                "sha256:a8b315203925724f89a81a741682589ba1c36ec858d98e6accb7501ece9e99a3",
-                "sha256:ad8fa7a91fa8f2a4fa46366142763675a0a11b7c34b06dfc20b1095d116da820",
-                "sha256:b507df9ea606a87c29e5028b8de9f35066a15f6a5d7f3e5b47b3719e9403f924",
-                "sha256:bf236758429d9b9cdadd1fcf40901588818ee440178b932409c40157ab41e902",
-                "sha256:c2961d44593aaa99580971e4123db00d4ca72fb4b30fa56350b3f6792331a41e",
-                "sha256:c60be419d7cca1222895dfe9d520628b7346015208382a19fa678356a22664b3",
-                "sha256:cfff49dbb7fcc2a9a88e3f25fda7f181ee4957fd89df78c47fa64c689d19b8a9",
-                "sha256:d339f90cc30de4b013670de84abd46de4be602d5c52bbe4e569fa15d17b204ca",
-                "sha256:d628637d4f0c55613f258b84eef932faf89e683aa842f4fd483a676f44a38606",
-                "sha256:d949e93fbdaf5b43f69a484639104c07028f93686c8305afb0d8e382fde8ff5d",
-                "sha256:e13de2947c496fcb600fa4b5cd00a5fa33d4b3af9d13c169a5f79268268de0a8",
-                "sha256:e323b75abda43345aff5ab2f6b1c017135f937f8a114d7aac8d95a07d200e19f",
-                "sha256:e3948be800b5f251a0741ec3aab3ca508dfc391095726a69af7064fa4d3e0547",
-                "sha256:e516bc6bba5455817bbb0038f4c44d1914aac13c7f7954dee9213c9ae28bd9ac",
-                "sha256:e62607c86e02d29ba5cb00837f73b1dce7b325a1f1f6d93150a0f96fa68da1a1",
-                "sha256:f2acf958513bd1612960ec68aa5e388262218f7365db59e54e1ee68a55bc544b",
-                "sha256:f57b1ee40387e43ab5c3cf20437283477b5ef52ead4bb1d9bff254ef9ee70623",
-                "sha256:fa18acc2d6f0d09575802e1db11845fc0f83f9777cc385c51380125df92f3dc9",
-                "sha256:fab0457ab07e8abb99de2b83c0a71f98bdf79afb01ff611873e4333fd8649f02"
+                "sha256:03b3925472771607d13feb9a0de93b04408ae86c91eee3f5e09e43744f90b1af",
+                "sha256:03b505fc8ce2dfcf800feac0e20cbb7b1899a5ef7407fa0cccb3267a5b2abbdb",
+                "sha256:058bf839884b5d5d8488978ed804023be64fc9bafb674a0ede1ba26c05bd9146",
+                "sha256:088482e07aed6229a34fbb1d0c5fbe0ad9c413dbddb5eaaa8e5c83d933cbe8d6",
+                "sha256:0961811d85ac551b1ce1f197296a8e5f497b35a149cfc6e128f74dfaef5e592f",
+                "sha256:155154084bdedfc8904524d8bd212e5896cc5d5caf1d45c19d13dc34aee4b5ab",
+                "sha256:1716d21d423a1a2261cd717bc66714eeb5464d6a061b92678f356ca69cfd1255",
+                "sha256:1f1656e931c937f8bdce12c551fa0077db814b123e7f16b6db26e1e7c89dae16",
+                "sha256:2fae2d4bcb0564e0eb8e72c97e149faebfad369aeaef74ed7fd17f5f84a07428",
+                "sha256:376e12d230fd198a329dfe253b41480b0a015a2dabbac5eecf6b279fe3afb1b3",
+                "sha256:3dc6a6133bffc33cb75bbc79dc08bd1e206017ac69ec68f703227aaf5f5129bb",
+                "sha256:3ff822473d498d606424f92a341d01121562af35bf1d3d0e2ccd1f9c2f86859b",
+                "sha256:440ff5f59f318ce495c6bdddfa01a23dd64713fb960ceb87c3a9423745781d47",
+                "sha256:44f7dbf800e6f933a5c56e07b18ef70f44949f34bf57f5d5318e2199c12cbfbc",
+                "sha256:46ef33b616027a616dcceba33bc48e589ba24fa84ee43c5b8611c5b57d2dace3",
+                "sha256:4d18b3e9e9259595dd5c538c1fd9238f8b26c22d6351397e721ef8a89ad55f12",
+                "sha256:51e04b162529f99c7b764129e07aaa3ec8edfc63ca7a212b71e348319f8b821b",
+                "sha256:59580776fd7e520995b82a6134c8ca7152a7881e174077fc785f4cc69c476d69",
+                "sha256:5a4cc4fef74dcab0b428ef750fad3c05311657ffb4f1dd3d4afa75e664551588",
+                "sha256:65bf63b2068e13183e34a4beaf921f20cd144a25cebed0fa9a46f25e8b47577d",
+                "sha256:6df4cf354adb911a9ca58bc5c60fb1ae27544527878bc3ddf8f7ea56946c6fcc",
+                "sha256:755698083c6119e771ea3f5837143324636700e1e5b397885c05085a837d5876",
+                "sha256:79e561b67e606b6e13ba58e6ae3e688e3429dbb5d60e551ba40d649432044f37",
+                "sha256:7dc827f119ccc3ea55b7bec73573516117c55319edc93bc2bbcf389bf1e7acfe",
+                "sha256:82eff3e5664c5a17fc0cbb1dae2c32088cdd3c3bfbfe4b9c71012275c2a63e8e",
+                "sha256:84dc3b831af386cb20cae8fb10ac78d8007bb29118730db2e9f21c329a528028",
+                "sha256:867fe03c1c241d2416b719e23d1671537e34e03bab741dcc50d49298c1397073",
+                "sha256:87c90b525296c4930b1f74bf460b97af052c3cc9ba47d811f416ed82e1b16b03",
+                "sha256:891b56a3bbaf3470595c218e847e79448e95cecb412224c8585da640c61cf29a",
+                "sha256:89869925f4e1762878561fa1e3cbd1ee5ce73e5597275b5fc8bc054dd894fca4",
+                "sha256:8aa90a648f17bacacef95b09a5fab368e8feff3714fc4b81eb9374bd439850e6",
+                "sha256:8ece87d8616bf12e55a08a05159f4303c8b82d348c2c43c7297c85d8e95dfa3e",
+                "sha256:94e47dd8cf39cabe20b41dd0c4c6589f0c7a4de2a5bad8e51ab0fc0b4a26ae6b",
+                "sha256:a22a3fbb3abefd7a9f5a672af8fccb8d8d996b2eae2075ac9d8ca10f4a6f6653",
+                "sha256:a349317c9d634aa56e30aae9ad408bc1b9de281af0e4f87de682b454ebaf540e",
+                "sha256:ab8147607af85fc2ec2e02b4364ff36b636f63781295e74220dc5c5856794e07",
+                "sha256:ae930d226f9145ec580f3fe10fc23262b8c21a6a0cd6fbc081a6606e9000ce74",
+                "sha256:b5dcd68b23b1a549a3b0851d3621630e492ff9015a18f29f2512088b4e03e4d9",
+                "sha256:b85c873315741dbc208c199cbe449aa77d1831551dd78d9b3d67e0a6f9eb576d",
+                "sha256:bb2d0503f45ad85ca7319bd37fd983e374b3f824c38a450b5f72cfc974114156",
+                "sha256:bc906a19be96d2820dee8e681ca1d3129821eb6e5c4f1544db723edf0c0696bd",
+                "sha256:cc73099fa7525a20e2021a2f2befa61e9ef306364838c1859ba79f5bd8eda33a",
+                "sha256:d986976c9b758d60d966fbaf8bdff129d125e8b2c58889d2220ca96991f1071e",
+                "sha256:e48550269c3baff04cc46ca79bd9d2d5a62216665751b10aa86d95ebe182d319",
+                "sha256:ef0c7e534e53f14b7b09dc3fe1e207243c9bb3eb2543d9876ed253156ca7a8bf",
+                "sha256:f1444229f84a7aea48ce3f1143147acee92eee264826db4c41ea38c6b0a924a9",
+                "sha256:f17be52c99e3eaeefaaac780bde40bfa99be3ad32bbfed346bb347c9d0b01967",
+                "sha256:f234ebcc3355155811389c320974056ce20233770205fc7cb41d8653d6137efa",
+                "sha256:fa4595600a699ed13e854b87116a1519a25e47a10100df01650c1be3532bd629",
+                "sha256:fd03d6d8dbfdd9bab97ada98759e345b29d50f690cec95dd01d22d02f616bfea"
+            ],
+            "version": "==2.3.7"
+        },
+        "moderngl": {
+            "hashes": [
+                "sha256:1ce40fb73f80c1f09f4a095adda341fdaf1b3043f219fbfe44a9da81577dde7e",
+                "sha256:279486e143eb849fcab126e3ef3a1a0353bbbdb1d27a13c76335cf4ae14b2827",
+                "sha256:2d572b3e8243e63efbb85bb6a90dfffe84a8d57233ff7e03cad44023a414678f",
+                "sha256:2e2205402a8d0792efc380e68cb1a11218c09454e6d8d1d95fda0becb2d36a5a",
+                "sha256:3012c38b882985aa1140196ba157b8d5a625add0ee0761c3c2937505b1365675",
+                "sha256:310db1cc52dbcc211d957f27ca9d14f3e474657eb2d5670f03adf9221c9b1647",
+                "sha256:3366be15c5aaa841239091dfa2c86c6acb09b67fa2a86552f8b4f59c0e9dae55",
+                "sha256:3a850968d417fb62eb26922d2158a6748b90088db948c9499dc05cd616a845d9",
+                "sha256:3ebc9016a0849edc4654e4d1935748ca2dc72427ea678aa7fc166d449e0c1db2",
+                "sha256:4a16916facea2351b70db73226cef1545c43f3431d9861a7b467208898b82a0f",
+                "sha256:50313b30b744c59c07a01b63ecd4efd57488ad70ece4296d8669cac6ec1f634d",
+                "sha256:56b73042fb5593158b6935757c75c695673a46b74136c03c88c16af25628d998",
+                "sha256:5d3fd68011186a30ab4bbcdeb5348a5bce579cbef0e849944ca875d0be70f0c2",
+                "sha256:5d8ffeb7b30d001f8495f7efbcdf39a07185ad94e7f843133ce991b459d47ba6",
+                "sha256:60ad02423ecc434433aa63ec0d8adbef94432e88a87ebf0853336dc3677c645e",
+                "sha256:651f450ac4520cb24161096f0bcfaf10820743d48e231cf0a27a8ff4e036c450",
+                "sha256:670682ad734dacb501685c62d958a849a856d01ebb6cafb639d6549e7ca4d39a",
+                "sha256:67918bbc43b2f7aa37d72ba1ed2dd506d993aed8d62d9771caaf541607bd7402",
+                "sha256:7400876b5ef3eb12f0e0374c48b881dd44f8aef4b3d901ffe508213949d62d0a",
+                "sha256:7b9b6efe0cecb182e07f0424b9d33a969f85e39f9e6eff2d5fb05e8e9ff67750",
+                "sha256:7ff301371e91dd39486c8d52a27934cc04ca3da6da16613255d3a6b69e89e621",
+                "sha256:8094f14072e102272f31617b219b601dd15e5117047ba33508014f9a40b7188a",
+                "sha256:8227c2986e2ce9a76314fa6271d72749e37831fa3031d0db1eccb7fcfd027f08",
+                "sha256:841d8e056f188d03ab02268f96368f570c72a91ed01f8fa43e83ecbcaf80bf06",
+                "sha256:88e9500293f02220d9613beb852242507de34b29639427a3b113be38941458fe",
+                "sha256:96433f592a6a113a2cd236f00a306f43059580ec5109553e0f0044decd61fe0c",
+                "sha256:9f19b0c201c5c2739358a68c12f0502424ed76659edaba4ea20760fc9b71d2fa",
+                "sha256:9f5b909dd73a30235989685bf83e8a5b2dad435ce576669a6731bf6659076f4b",
+                "sha256:a135faa1be35346a258bd59daf5307b763e4f20e32ecdd69fc0d84e5bb48adfc",
+                "sha256:a37db97c20e942ec20281d320c50f8ea006d5ac4797998484a7f8fdfe9e0129b",
+                "sha256:a5e25f34e3b6916f6394b3a7f10fa443a901662ecfb01c623ed9c7f87a660ed9",
+                "sha256:a7e9220ce5447e050adaaea42abf2b48e3eae4cc4a2fc07a3827239c067c5c68",
+                "sha256:a994da9d8cf3f5d9f549b02f9b9bfaeb0ce20c17e5acaa8b9737795d1bf62a28",
+                "sha256:ab9d969cbed50d7f86c6da8252b4a7adc53d033a24a281cd4b00221b1b26faf2",
+                "sha256:affffa368aea60fd5df0edff10d6923f74cd3f9fd7893675fe7c7bfe73517b7b",
+                "sha256:b5e7d98c5bd5e840c9667cf1817c01809b83beb8f8b83c6e76bf85f10dc99b63",
+                "sha256:b66c18d7f4ab7a94be3f9eb9e4ca6836ead1da502d62e81b7f7a48150e2ed391",
+                "sha256:b8079fcf1a8e4df24ab2313165cc77721c7676a1c68b2e48a890d283525f6858",
+                "sha256:bbb23f67bd1bb0babd67246330137bd4b9fd49557fa5ae402305685a48df3d6d",
+                "sha256:bcd7de06efafa9e4cef63c942e886586fd25076867d46511aaf5aa478317c2f3",
+                "sha256:c5e92e1c8af12fdf3f5fb1923412632887aa3002bdb23d46a3ff564b93cc002c",
+                "sha256:cc3ed59322867afbc9edf4d96deb619e1e13bb7ef8bfc778b10adbd117f8af9b",
+                "sha256:d0d9fa90957c382ebbc7011ffc29807ae914e64f2d519d974b87e583d6c07188",
+                "sha256:d51c2d31decab2f3a534c04d2dfda631d9a2efc79ddb36d75e4b50747fc134f2",
+                "sha256:d7362808ab3ef32b95b534de6be20f09eee23f047954dd01d3d2433faf1f0725",
+                "sha256:df3c541ef9322fafebc113924a5034bb0fb3ac4afab9bd72cc6798795edbfd18",
+                "sha256:e2e6378212c18b82503c82555644a12bb9087215c8ae783b655a1f3ade403285",
+                "sha256:e4fc84269d26731832303c1904bd33e4692a648b26e97661c8455e4fdfc6bd17",
+                "sha256:f066d9b0e743bb60e3dfa540214b4fe19c5d25f3ab7dd4f61c36fb00854fa502",
+                "sha256:f140f9d9f5f11fc2a7b41324dd7bcf88c1fc9576d5b21f78b42707d835583be9"
             ],
             "index": "pypi",
-            "version": "==2.3.0"
+            "version": "==5.8.2"
         },
-        "pygments": {
-            "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
-        },
-        "pytest": {
-            "hashes": [
-                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
-                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
-            ],
-            "markers": "python_version >= '3.7'",
-            "version": "==7.2.2"
-        },
-        "pytest-ordering": {
-            "hashes": [
-                "sha256:27fba3fc265f5d0f8597e7557885662c1bdc1969497cd58aff6ed21c3b617de2",
-                "sha256:3f314a178dbeb6777509548727dc69edf22d6d9a2867bf2d310ab85c403380b6",
-                "sha256:561ad653626bb171da78e682f6d39ac33bb13b3e272d406cd555adb6b006bda6"
-            ],
-            "index": "pypi",
-            "version": "==0.6"
-        },
-        "requests": {
-            "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
-            ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
-        },
-        "six": {
-            "hashes": [
-                "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
-                "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.16.0"
-        },
-        "snowballstemmer": {
-            "hashes": [
-                "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
-                "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
-            ],
-            "version": "==2.2.0"
-        },
-        "sphinx": {
-            "hashes": [
-                "sha256:0dac3b698538ffef41716cf97ba26c1c7788dba73ce6f150c1ff5b4720786dd2",
-                "sha256:807d1cb3d6be87eb78a381c3e70ebd8d346b9a25f3753e9947e866b2786865fc"
-            ],
-            "markers": "python_version >= '3.8'",
-            "version": "==6.1.3"
-        },
-        "sphinx-autobuild": {
+        "pygame": {
             "hashes": [
-                "sha256:8fe8cbfdb75db04475232f05187c776f46f6e9e04cacf1e49ce81bdac649ccac",
-                "sha256:de1ca3b66e271d2b5b5140c35034c89e47f263f2cd5db302c9217065f7443f05"
+                "sha256:00ecd4688ee25d5d4cf48eddab18749a9bb2b382772f7fa8a987e4d21026c603",
+                "sha256:075c1282b1d307669c8ef29942564b91acb85623bedba3bfb841079d539ded31",
+                "sha256:13511c7c29f0fc23636f3b95a96ab45f964e84073e7e27dc602a479cd274d89a",
+                "sha256:1422673a2b485153cbc20dbbd37af791c9842ca98a1b7a89fe3ac115cce79805",
+                "sha256:14492d8c0eaad778bb10b6d53eaea4ef77f4d3431b6b7c857397dc6cf4397ac9",
+                "sha256:1b7201a44869eb420dd56c8e003251c9e7422c5304b3e78508e767a5634ab31b",
+                "sha256:23543e2d206d8de7d6db4f7b1c74e6fea6c01ead63caf7252e63341e1cdb09f6",
+                "sha256:2946c151691c80ffb9f3f39e1f294d7ed9edaae1814e528d2f5b4751e7e6d903",
+                "sha256:32ed4d4317bce8fe78592a7b5b4a07f2e0ff814e35c66cb5a3b398dae96c3f27",
+                "sha256:3ab14e06c302921f33d25180813711a920acef386d3992fc21731d2d5e8e86f0",
+                "sha256:418659c2d42f6a2356e2691006d79b6e07fd4992f9e904a2638c51c992f3e41b",
+                "sha256:43db3a6c9be3d94eececf7c86cde7584d2bb87f394ade40139c3b4e528fdff24",
+                "sha256:47be83060a9dbc79763fd230f04d53a29064b5f64d1b59425c432d3570b22623",
+                "sha256:47fd096ceb68d966681f8d0e820f7305bf05b30421ca562cfdb3c89a5aef26e5",
+                "sha256:4a98ed8c47e367b9233b5ca25c36c2b45ab61959ac543195f0b6349f0a599ec8",
+                "sha256:4b562cfdd8caa76ba47ca2a9211fee6b0a95ceb95c9da94cf60a3909b2300854",
+                "sha256:4ffec9661731fb674ccc88d1de92709219047af3d8198d0e6203c21f3f1b54a7",
+                "sha256:5210cb09ec31281e16fda008bf8dfe2e024eef58e075dd0c01935d0004fdfffd",
+                "sha256:53bfdc1aea619fa8d347be37b08de87089d543375948aacf8b163b0c5eb6d4e4",
+                "sha256:5a2aee4214e5efed2cb3650139010dd4d0b1c29a9760278ab259d0b46281b66a",
+                "sha256:5a93d368311d40827dc5f0cad2a0e9a8700c1b017346808cfdfd9ea98aee45df",
+                "sha256:6060d68d10fafd51c4cb3a7d687d741009881860dfd429c863e570877e2ce9de",
+                "sha256:627c8bb007a757da18d32c5d9b7ac50ab0356d9e922d570b0572765778080787",
+                "sha256:63591f381e5b28b90e115ac7a96f8ce5ecb917facb42d79d4f89714f89cc6d8e",
+                "sha256:65ee75e0e83e393fdc5c06e55e376c7511881a5ebee006ecca89cb1b3b41d6f1",
+                "sha256:6ba967d0e3fed8611f1face6695dc8fa554ee543d300681f8080f5de9cc7da73",
+                "sha256:6c0081546749c0b4341ce575622a4f8eee05f675d3a0872ab6aed6e5bd2ba5a8",
+                "sha256:6ec870a63295ebff737640c4ef39868312e206dcba655b4ad5c7d0e8c2488b73",
+                "sha256:751bc57e4c3b7cd92762344562dcbd405e2b54488de1d7a1e083a470bdbc5ae9",
+                "sha256:75ef535ebe541b74a160bb59c3e520f543250d19f69d5973350ec1b9706e1469",
+                "sha256:79b0962a8f09788ca735532cfcf2dd053424fe5eabbda564b74f8e5e2eb11f48",
+                "sha256:7e5d32def075e495b4802371fd8cda96ff4957aa39e215f83d87022dedf14cfb",
+                "sha256:7fa1e65fd559823997f39a592cb49d8c89dd31c8bbde8273fe3922e2c1f294f6",
+                "sha256:802b03f6c367359c94eb6a90169666efa1aa1d6e24fce37a0b21642ccdfe48cf",
+                "sha256:80502eb26483b0206d0508475ec7d67a86bc0afc5bb4aad3a6172a7a85a27554",
+                "sha256:867cf19f1c7aa6f187a0a31b702f5668e935e700b46d94bd58e94ec8581cf081",
+                "sha256:8b6e1493724d29e46a0e7e8125d9808c9957c652db67afe9497d385509fc5ac5",
+                "sha256:8f97c8be81b3262ad8dae982485c4a73c9f2374614dfc0db8eb0f754badb29d6",
+                "sha256:93bb1406125ae9bd7a9bb0d45f11b30f157ea8d2efee1ebe9d781b1d1a9fce6b",
+                "sha256:99c296ecb8ce6ea1f404f4d174fdb215c64515827778525301c29ddf6f8e6e07",
+                "sha256:9f6b7a604812f447495829751dfe7ab57cb31c2c9acdb07ba4b7157490411a12",
+                "sha256:a66b314f4a637784d5ca2970745bb2e6e554447dce8f4cfedd9b9fcef5e3ffc6",
+                "sha256:ab8115af26a9e95f39b08fff416f097803480f265500b218a5ca065d6e73124f",
+                "sha256:b04451e5addae3a078a7a4f494e6b217025f4813dfb364a49c250fc5dfd1d2e2",
+                "sha256:b4c75dd345707da622c78dbd6a63a025f7b89377ddc4e71ba40043929824f5d4",
+                "sha256:b6b94fc99487ce4a45ce00fa9145f4861f6e021254a005101d00bc17a4bb4f5c",
+                "sha256:bb5a39320d00fa781959d2d0151e6f0293dd1398c6dc9dc934112ecce7b4fb52",
+                "sha256:be7f948d33d0536c2922289e6f5983251cb0bd0d727db6ff692886c239f47a2c",
+                "sha256:c09323eeae9e0cb2ced0cb3635485ae17f4f1b2b6b908a494ce2d830c609d4be",
+                "sha256:c4241e1da3852a955d37a22157ed51b2d30a65f7987eac9d162bb302fb754d87",
+                "sha256:ca2ecc65126eaaa5b8e6a119913cfb2c2b1ed4c8ee1b980baf333aa9d379f227",
+                "sha256:cad74cbbefbdb81cb22a9ea22561614b8dc58fcd52cd54126bbb8ee9ee77a5d5",
+                "sha256:cff815181437add5f3d702e8c7f1d2aa4ed04ed04cde27ec809e7ac516ee6b5f",
+                "sha256:d9b1127f085d09c7c0a976d440e8fc2f7adc579d62abcfc20c23c2699bbe2dc1",
+                "sha256:de963a4b8787d93a9fba8f4052d9dde8b12adbeac5781e48035be1557dfadb20",
+                "sha256:e2a3176b33b97ebae397f951d254e3155a0afe730e1b76fb35126555c27dd3b5",
+                "sha256:e3603e70e96ee30af1954ce57d4922a059402f368013e7138e90f1c03d185267",
+                "sha256:e5f043751840a07ff0160abe46ed42a88bc29baee93656abb5a050beda176306",
+                "sha256:e70fd71e0321a805001192e08ae4af45b86c68f155670230c3f6f4dd25089e70",
+                "sha256:e75d8c2980d719045be366160568bf508cbbed21285efe32468c75abcd4cf8b3",
+                "sha256:ef14750fa60b47510cfe9c7c37e7abe67617f5d1f1a8ffa257a59d49836dadda",
+                "sha256:f3020fb98f27a6ea79418a5b332ca07be93884e4a455c8a0a31b2dcf39ee2d96",
+                "sha256:f576403c2b14f0eea694365b9018d5bacac70b1550261ffc7a54a92e18967541",
+                "sha256:f9c8bb7b77f97eb49dac900445fbf96a332d2072588949d6396581933843fb04",
+                "sha256:fa2531f83e7c5f6f7cc20a1b4e0f982bd608aad81ff6c385148e64256ab0419f",
+                "sha256:faa3b63b71d555e7a21cecc11c65e059d9cb1902158d863ac3592e1947bc521a",
+                "sha256:fb7bb86c4aedb4382d7f643ff7d21ab4731d59ddb9b448e78b9125ab1addc007",
+                "sha256:fbcba1b06f42338fecbd366227025f81729d9f4a577677fd3cd1ceff34d7286a"
             ],
             "index": "pypi",
-            "version": "==2021.3.14"
-        },
-        "sphinxcontrib-applehelp": {
-            "hashes": [
-                "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
-                "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
-            ],
-            "markers": "python_version >= '3.8'",
-            "version": "==1.0.4"
-        },
-        "sphinxcontrib-devhelp": {
-            "hashes": [
-                "sha256:8165223f9a335cc1af7ffe1ed31d2871f325254c0423bc0c4c7cd1c1e4734a2e",
-                "sha256:ff7f1afa7b9642e7060379360a67e9c41e8f3121f2ce9164266f61b9f4b338e4"
-            ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.2"
-        },
-        "sphinxcontrib-htmlhelp": {
-            "hashes": [
-                "sha256:0cbdd302815330058422b98a113195c9249825d681e18f11e8b1f78a2f11efff",
-                "sha256:c38cb46dccf316c79de6e5515e1770414b797162b23cd3d06e67020e1d2a6903"
-            ],
-            "markers": "python_version >= '3.8'",
-            "version": "==2.0.1"
-        },
-        "sphinxcontrib-jsmath": {
-            "hashes": [
-                "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
-                "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
-            ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.1"
-        },
-        "sphinxcontrib-qthelp": {
-            "hashes": [
-                "sha256:4c33767ee058b70dba89a6fc5c1892c0d57a54be67ddd3e7875a18d14cba5a72",
-                "sha256:bd9fc24bcb748a8d51fd4ecaade681350aa63009a347a8c14e637895444dfab6"
-            ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.0.3"
-        },
-        "sphinxcontrib-serializinghtml": {
-            "hashes": [
-                "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd",
-                "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
-            ],
-            "markers": "python_version >= '3.5'",
-            "version": "==1.1.5"
-        },
-        "tomli": {
-            "hashes": [
-                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
-                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
-            ],
-            "markers": "python_version < '3.11'",
-            "version": "==2.0.1"
-        },
-        "tornado": {
-            "hashes": [
-                "sha256:1d54d13ab8414ed44de07efecb97d4ef7c39f7438cf5e976ccd356bebb1b5fca",
-                "sha256:20f638fd8cc85f3cbae3c732326e96addff0a15e22d80f049e00121651e82e72",
-                "sha256:5c87076709343557ef8032934ce5f637dbb552efa7b21d08e89ae7619ed0eb23",
-                "sha256:5f8c52d219d4995388119af7ccaa0bcec289535747620116a58d830e7c25d8a8",
-                "sha256:6fdfabffd8dfcb6cf887428849d30cf19a3ea34c2c248461e1f7d718ad30b66b",
-                "sha256:87dcafae3e884462f90c90ecc200defe5e580a7fbbb4365eda7c7c1eb809ebc9",
-                "sha256:9b630419bde84ec666bfd7ea0a4cb2a8a651c2d5cccdbdd1972a0c859dfc3c13",
-                "sha256:b8150f721c101abdef99073bf66d3903e292d851bee51910839831caba341a75",
-                "sha256:ba09ef14ca9893954244fd872798b4ccb2367c165946ce2dd7376aebdde8e3ac",
-                "sha256:d3a2f5999215a3a06a4fc218026cd84c61b8b2b40ac5296a6db1f1451ef04c1e",
-                "sha256:e5f923aa6a47e133d1cf87d60700889d7eae68988704e20c75fb2d65677a8e4b"
-            ],
-            "markers": "python_version > '2.7'",
-            "version": "==6.2"
-        },
-        "urllib3": {
-            "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
-            ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "version": "==2.4.0"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
@@ -496,22 +214,14 @@
         "altgraph": {
             "hashes": [
                 "sha256:ad33358114df7c9416cdb8fa1eaa5852166c505118717021c6a8c7c7abbd03dd",
                 "sha256:c8ac1ca6772207179ed8003ce7687757c04b0b71536f81e2ac5755c6226458fe"
             ],
             "version": "==0.17.3"
         },
-        "attrs": {
-            "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
-        },
         "autopep8": {
             "hashes": [
                 "sha256:86e9303b5e5c8160872b2f5ef611161b2893e9bfe8ccc7e2f76385947d57a2f1",
                 "sha256:f9849cdd62108cb739dbcdbfb7fdcc9a30d1b63c4cc3e1c1f893b5360941b61c"
             ],
             "index": "pypi",
             "version": "==2.0.2"
@@ -528,21 +238,29 @@
             "hashes": [
                 "sha256:1a1a85c1595e07d8db14c5f09f09e6433502c51c595970edc090551f0db99414",
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
+        "build": {
+            "hashes": [
+                "sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171",
+                "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"
+            ],
+            "index": "pypi",
+            "version": "==0.10.0"
+        },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
                 "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
                 "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
                 "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
@@ -622,49 +340,131 @@
             "version": "==3.1.0"
         },
         "click": {
             "hashes": [
                 "sha256:7682dc8afb30297001674575ea00d1814d808d6a36af415a82bd481d37ba7b8e",
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
-            "markers": "python_version >= '3.7'",
+            "index": "pypi",
             "version": "==8.1.3"
         },
         "colorama": {
             "hashes": [
                 "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "markers": "os_name == 'nt'",
             "version": "==0.4.6"
         },
+        "coverage": {
+            "extras": [
+                "toml"
+            ],
+            "hashes": [
+                "sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f",
+                "sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2",
+                "sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a",
+                "sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a",
+                "sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01",
+                "sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6",
+                "sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7",
+                "sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f",
+                "sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02",
+                "sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c",
+                "sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063",
+                "sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a",
+                "sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5",
+                "sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959",
+                "sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97",
+                "sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6",
+                "sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f",
+                "sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9",
+                "sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5",
+                "sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f",
+                "sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562",
+                "sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe",
+                "sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9",
+                "sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f",
+                "sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb",
+                "sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb",
+                "sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1",
+                "sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb",
+                "sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250",
+                "sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e",
+                "sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511",
+                "sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5",
+                "sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59",
+                "sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2",
+                "sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d",
+                "sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3",
+                "sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4",
+                "sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de",
+                "sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9",
+                "sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833",
+                "sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0",
+                "sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9",
+                "sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d",
+                "sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050",
+                "sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d",
+                "sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6",
+                "sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353",
+                "sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb",
+                "sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e",
+                "sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8",
+                "sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495",
+                "sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2",
+                "sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd",
+                "sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27",
+                "sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1",
+                "sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818",
+                "sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4",
+                "sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e",
+                "sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850",
+                "sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==7.2.7"
+        },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:23010f129180089fbcd3bc08cfefccb3b890b0050e1ca00c867036e9d161b98c",
+                "sha256:679987caf361a7539d76e584cbeddc311e3aee937877c87346f31debc63e9d06"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
+            "version": "==0.18.1"
         },
-        "exceptiongroup": {
+        "easyprocess": {
             "hashes": [
-                "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
-                "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
+                "sha256:82eed523a0a5eb12a81fa4eacd9f342caeb3f900eb4b798740e6696ad07e63f9",
+                "sha256:885898302a57aab948973e8b5d32a4229392b9fb2d986ab1d4ffd590e5ba90ec"
             ],
-            "markers": "python_version < '3.11'",
-            "version": "==1.1.1"
+            "version": "==1.1"
+        },
+        "entrypoint2": {
+            "hashes": [
+                "sha256:eeb8c327bdb65cdd1668c023a6b110b7e3d1a046fb05e043861ebd9264b3a257",
+                "sha256:fc0b7fe7b21acdab47a585ab9407ca7e5c4f96cb6888575db6b0ceb91f0e105a"
+            ],
+            "version": "==1.1"
         },
         "flake8": {
             "hashes": [
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
             "version": "==6.0.0"
         },
+        "ghp-import": {
+            "hashes": [
+                "sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619",
+                "sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343"
+            ],
+            "version": "==2.1.0"
+        },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
@@ -675,19 +475,19 @@
                 "sha256:69150444affb9cb0d5cc5a92b3676f0b2fb7cd9ae39e947a5e11a36b4497cd4a"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.4.1"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:43ce9281e097583d758c2c708c4376371261a02c34682491a8e98352365aad20",
-                "sha256:ff80f3b5394912eb1b108fcfd444dc78b7f1f3e16b16188054bd01cb9cb86f09"
+                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
+                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==6.1.0"
+            "version": "==6.6.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -713,77 +513,99 @@
             "hashes": [
                 "sha256:771ed2a91909389ed6148631de678f82ddc73737d85a927f382a8a1b157898cd",
                 "sha256:ba2e15a9b35e21908d0aaf4e0a47acc52d6ae33444df0da2b49d41a46ef6d678"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.13.1"
         },
+        "logbook": {
+            "hashes": [
+                "sha256:0cf2cdbfb65a03b5987d19109dacad13417809dcf697f66e1a7084fb21744ea9",
+                "sha256:2dc85f1510533fddb481e97677bb7bca913560862734c0b3b289bfed04f78c92",
+                "sha256:56ee54c11df3377314cedcd6507638f015b4b88c0238c2e01b5eb44fd3a6ad1b",
+                "sha256:66f454ada0f56eae43066f604a222b09893f98c1adc18df169710761b8f32fe8",
+                "sha256:7c533eb728b3d220b1b5414ba4635292d149d79f74f6973b4aa744c850ca944a",
+                "sha256:8f76a2e7b1f72595f753228732f81ce342caf03babc3fed6bbdcf366f2f20f18",
+                "sha256:94e2e11ff3c2304b0d09a36c6208e5ae756eb948b210e5cbd63cd8d27f911542",
+                "sha256:97fee1bd9605f76335b169430ed65e15e457a844b2121bd1d90a08cf7e30aba0",
+                "sha256:e18f7422214b1cf0240c56f884fd9c9b4ff9d0da2eabca9abccba56df7222f66"
+            ],
+            "version": "==1.5.3"
+        },
+        "markdown": {
+            "hashes": [
+                "sha256:cbb516f16218e643d8e0a95b309f77eb118cb138d39a4f27851e6a63581db874",
+                "sha256:f5da449a6e1c989a4cea2631aa8ee67caa5a2ef855d551c88f9e309f4634c621"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==3.3.7"
+        },
         "markdown-it-py": {
             "hashes": [
                 "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
                 "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.2.0"
         },
         "markupsafe": {
             "hashes": [
-                "sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed",
-                "sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc",
-                "sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2",
-                "sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460",
-                "sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7",
-                "sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0",
-                "sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1",
-                "sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa",
-                "sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03",
-                "sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323",
-                "sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65",
-                "sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013",
-                "sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036",
-                "sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f",
-                "sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4",
-                "sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419",
-                "sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2",
-                "sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619",
-                "sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a",
-                "sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a",
-                "sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd",
-                "sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7",
-                "sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666",
-                "sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65",
-                "sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859",
-                "sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625",
-                "sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff",
-                "sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156",
-                "sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd",
-                "sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba",
-                "sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f",
-                "sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1",
-                "sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094",
-                "sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a",
-                "sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513",
-                "sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed",
-                "sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d",
-                "sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3",
-                "sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147",
-                "sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c",
-                "sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603",
-                "sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601",
-                "sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a",
-                "sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1",
-                "sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d",
-                "sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3",
-                "sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54",
-                "sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2",
-                "sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6",
-                "sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58"
+                "sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e",
+                "sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e",
+                "sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431",
+                "sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686",
+                "sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559",
+                "sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc",
+                "sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c",
+                "sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0",
+                "sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4",
+                "sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9",
+                "sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575",
+                "sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba",
+                "sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d",
+                "sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3",
+                "sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00",
+                "sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155",
+                "sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac",
+                "sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52",
+                "sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f",
+                "sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8",
+                "sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b",
+                "sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24",
+                "sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea",
+                "sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198",
+                "sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0",
+                "sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee",
+                "sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be",
+                "sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2",
+                "sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707",
+                "sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6",
+                "sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58",
+                "sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779",
+                "sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636",
+                "sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c",
+                "sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad",
+                "sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee",
+                "sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc",
+                "sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2",
+                "sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48",
+                "sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7",
+                "sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e",
+                "sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b",
+                "sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa",
+                "sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5",
+                "sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e",
+                "sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb",
+                "sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9",
+                "sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57",
+                "sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc",
+                "sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.1.2"
+            "version": "==2.1.3"
         },
         "mccabe": {
             "hashes": [
                 "sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325",
                 "sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e"
             ],
             "markers": "python_version >= '3.6'",
@@ -793,44 +615,156 @@
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
+        "mergedeep": {
+            "hashes": [
+                "sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8",
+                "sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==1.3.4"
+        },
+        "mkdocs": {
+            "hashes": [
+                "sha256:5955093bbd4dd2e9403c5afaf57324ad8b04f16886512a3ee6ef828956481c57",
+                "sha256:6ee46d309bda331aac915cd24aab882c179a933bd9e77b80ce7d2eaaa3f689dd"
+            ],
+            "index": "pypi",
+            "version": "==1.4.3"
+        },
+        "mkdocs-material": {
+            "hashes": [
+                "sha256:8513ab847c9a541ed3d11a3a7eed556caf72991ee786c31c5aac6691a121088a",
+                "sha256:b49e12869ab464558e2dd3c5792da5b748a7e0c48ee83b4d05715f98125a7a39"
+            ],
+            "index": "pypi",
+            "version": "==9.1.15"
+        },
+        "mkdocs-material-extensions": {
+            "hashes": [
+                "sha256:9c003da71e2cc2493d910237448c672e00cefc800d3d6ae93d2fc69979e3bd93",
+                "sha256:e41d9f38e4798b6617ad98ca8f7f1157b1e4385ac1459ca1e4ea219b556df945"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==1.1.1"
+        },
         "more-itertools": {
             "hashes": [
                 "sha256:cabaa341ad0389ea83c17a94566a53ae4c9d07349861ecb14dc6d0345cf9ac5d",
                 "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==9.1.0"
         },
         "mouseinfo": {
             "hashes": [
                 "sha256:2c62fb8885062b8e520a3cce0a297c657adcc08c60952eb05bc8256ef6f7f6e7"
             ],
             "version": "==0.1.3"
         },
+        "mss": {
+            "hashes": [
+                "sha256:6eb7b9008cf27428811fa33aeb35f3334db81e3f7cc2dd49ec7c6e5a94b39f12",
+                "sha256:7ee44db7ab14cbea6a3eb63813c57d677a109ca5979d3b76046e4bddd3ca1a0b"
+            ],
+            "markers": "python_version >= '3.5'",
+            "version": "==9.0.1"
+        },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pefile": {
             "hashes": [
                 "sha256:82e6114004b3d6911c77c3953e3838654b04511b8b66e8583db70c65998017dc",
                 "sha256:da185cd2af68c08a6cd4481f7325ed600a88f6a813bad9dea07ab3ef73d8d8d6"
             ],
             "markers": "sys_platform == 'win32'",
             "version": "==2023.2.7"
         },
+        "pillow": {
+            "hashes": [
+                "sha256:07999f5834bdc404c442146942a2ecadd1cb6292f5229f4ed3b31e0a108746b1",
+                "sha256:0852ddb76d85f127c135b6dd1f0bb88dbb9ee990d2cd9aa9e28526c93e794fba",
+                "sha256:1781a624c229cb35a2ac31cc4a77e28cafc8900733a864870c49bfeedacd106a",
+                "sha256:1e7723bd90ef94eda669a3c2c19d549874dd5badaeefabefd26053304abe5799",
+                "sha256:229e2c79c00e85989a34b5981a2b67aa079fd08c903f0aaead522a1d68d79e51",
+                "sha256:22baf0c3cf0c7f26e82d6e1adf118027afb325e703922c8dfc1d5d0156bb2eeb",
+                "sha256:252a03f1bdddce077eff2354c3861bf437c892fb1832f75ce813ee94347aa9b5",
+                "sha256:2dfaaf10b6172697b9bceb9a3bd7b951819d1ca339a5ef294d1f1ac6d7f63270",
+                "sha256:322724c0032af6692456cd6ed554bb85f8149214d97398bb80613b04e33769f6",
+                "sha256:35f6e77122a0c0762268216315bf239cf52b88865bba522999dc38f1c52b9b47",
+                "sha256:375f6e5ee9620a271acb6820b3d1e94ffa8e741c0601db4c0c4d3cb0a9c224bf",
+                "sha256:3ded42b9ad70e5f1754fb7c2e2d6465a9c842e41d178f262e08b8c85ed8a1d8e",
+                "sha256:432b975c009cf649420615388561c0ce7cc31ce9b2e374db659ee4f7d57a1f8b",
+                "sha256:482877592e927fd263028c105b36272398e3e1be3269efda09f6ba21fd83ec66",
+                "sha256:489f8389261e5ed43ac8ff7b453162af39c3e8abd730af8363587ba64bb2e865",
+                "sha256:54f7102ad31a3de5666827526e248c3530b3a33539dbda27c6843d19d72644ec",
+                "sha256:560737e70cb9c6255d6dcba3de6578a9e2ec4b573659943a5e7e4af13f298f5c",
+                "sha256:5671583eab84af046a397d6d0ba25343c00cd50bce03787948e0fff01d4fd9b1",
+                "sha256:5ba1b81ee69573fe7124881762bb4cd2e4b6ed9dd28c9c60a632902fe8db8b38",
+                "sha256:5d4ebf8e1db4441a55c509c4baa7a0587a0210f7cd25fcfe74dbbce7a4bd1906",
+                "sha256:60037a8db8750e474af7ffc9faa9b5859e6c6d0a50e55c45576bf28be7419705",
+                "sha256:608488bdcbdb4ba7837461442b90ea6f3079397ddc968c31265c1e056964f1ef",
+                "sha256:6608ff3bf781eee0cd14d0901a2b9cc3d3834516532e3bd673a0a204dc8615fc",
+                "sha256:662da1f3f89a302cc22faa9f14a262c2e3951f9dbc9617609a47521c69dd9f8f",
+                "sha256:7002d0797a3e4193c7cdee3198d7c14f92c0836d6b4a3f3046a64bd1ce8df2bf",
+                "sha256:763782b2e03e45e2c77d7779875f4432e25121ef002a41829d8868700d119392",
+                "sha256:77165c4a5e7d5a284f10a6efaa39a0ae8ba839da344f20b111d62cc932fa4e5d",
+                "sha256:7c9af5a3b406a50e313467e3565fc99929717f780164fe6fbb7704edba0cebbe",
+                "sha256:7ec6f6ce99dab90b52da21cf0dc519e21095e332ff3b399a357c187b1a5eee32",
+                "sha256:833b86a98e0ede388fa29363159c9b1a294b0905b5128baf01db683672f230f5",
+                "sha256:84a6f19ce086c1bf894644b43cd129702f781ba5751ca8572f08aa40ef0ab7b7",
+                "sha256:8507eda3cd0608a1f94f58c64817e83ec12fa93a9436938b191b80d9e4c0fc44",
+                "sha256:85ec677246533e27770b0de5cf0f9d6e4ec0c212a1f89dfc941b64b21226009d",
+                "sha256:8aca1152d93dcc27dc55395604dcfc55bed5f25ef4c98716a928bacba90d33a3",
+                "sha256:8d935f924bbab8f0a9a28404422da8af4904e36d5c33fc6f677e4c4485515625",
+                "sha256:8f36397bf3f7d7c6a3abdea815ecf6fd14e7fcd4418ab24bae01008d8d8ca15e",
+                "sha256:91ec6fe47b5eb5a9968c79ad9ed78c342b1f97a091677ba0e012701add857829",
+                "sha256:965e4a05ef364e7b973dd17fc765f42233415974d773e82144c9bbaaaea5d089",
+                "sha256:96e88745a55b88a7c64fa49bceff363a1a27d9a64e04019c2281049444a571e3",
+                "sha256:99eb6cafb6ba90e436684e08dad8be1637efb71c4f2180ee6b8f940739406e78",
+                "sha256:9adf58f5d64e474bed00d69bcd86ec4bcaa4123bfa70a65ce72e424bfb88ed96",
+                "sha256:9b1af95c3a967bf1da94f253e56b6286b50af23392a886720f563c547e48e964",
+                "sha256:a0aa9417994d91301056f3d0038af1199eb7adc86e646a36b9e050b06f526597",
+                "sha256:a0f9bb6c80e6efcde93ffc51256d5cfb2155ff8f78292f074f60f9e70b942d99",
+                "sha256:a127ae76092974abfbfa38ca2d12cbeddcdeac0fb71f9627cc1135bedaf9d51a",
+                "sha256:aaf305d6d40bd9632198c766fb64f0c1a83ca5b667f16c1e79e1661ab5060140",
+                "sha256:aca1c196f407ec7cf04dcbb15d19a43c507a81f7ffc45b690899d6a76ac9fda7",
+                "sha256:ace6ca218308447b9077c14ea4ef381ba0b67ee78d64046b3f19cf4e1139ad16",
+                "sha256:b416f03d37d27290cb93597335a2f85ed446731200705b22bb927405320de903",
+                "sha256:bf548479d336726d7a0eceb6e767e179fbde37833ae42794602631a070d630f1",
+                "sha256:c1170d6b195555644f0616fd6ed929dfcf6333b8675fcca044ae5ab110ded296",
+                "sha256:c380b27d041209b849ed246b111b7c166ba36d7933ec6e41175fd15ab9eb1572",
+                "sha256:c446d2245ba29820d405315083d55299a796695d747efceb5717a8b450324115",
+                "sha256:c830a02caeb789633863b466b9de10c015bded434deb3ec87c768e53752ad22a",
+                "sha256:cb841572862f629b99725ebaec3287fc6d275be9b14443ea746c1dd325053cbd",
+                "sha256:cfa4561277f677ecf651e2b22dc43e8f5368b74a25a8f7d1d4a3a243e573f2d4",
+                "sha256:cfcc2c53c06f2ccb8976fb5c71d448bdd0a07d26d8e07e321c103416444c7ad1",
+                "sha256:d3c6b54e304c60c4181da1c9dadf83e4a54fd266a99c70ba646a9baa626819eb",
+                "sha256:d3d403753c9d5adc04d4694d35cf0391f0f3d57c8e0030aac09d7678fa8030aa",
+                "sha256:d9c206c29b46cfd343ea7cdfe1232443072bbb270d6a46f59c259460db76779a",
+                "sha256:e49eb4e95ff6fd7c0c402508894b1ef0e01b99a44320ba7d8ecbabefddcc5569",
+                "sha256:f8286396b351785801a976b1e85ea88e937712ee2c3ac653710a4a57a8da5d9c",
+                "sha256:f8fc330c3370a81bbf3f88557097d1ea26cd8b019d6433aa59f71195f5ddebbf",
+                "sha256:fbd359831c1657d69bb81f0db962905ee05e5e9451913b18b831febfe0519082",
+                "sha256:fe7e1c262d3392afcf5071df9afa574544f28eac825284596ac6db56e6d11062",
+                "sha256:fed1e1cf6a42577953abbe8e6cf2fe2f566daebde7c34724ec8803c4c0cda579"
+            ],
+            "markers": "python_version == '3.11'",
+            "version": "==9.5.0"
+        },
         "pkginfo": {
             "hashes": [
                 "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
@@ -841,18 +775,18 @@
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
         "pyautogui": {
             "hashes": [
-                "sha256:d31de8f712218d90be7fc98091fce1a12a3e9196e0c814eb9afd73bb2ec97035"
+                "sha256:dd1d29e8fd118941cb193f74df57e5c6ff8e9253b99c7b04f39cfc69f3ae04b2"
             ],
             "index": "pypi",
-            "version": "==0.9.53"
+            "version": "==0.9.54"
         },
         "pycodestyle": {
             "hashes": [
                 "sha256:347187bdb476329d98f695c213d7295a846d1152ff4fe9bacb8a9590b8ee7053",
                 "sha256:8a4eaf0d0495c7395bdab3589ac2db602797d76207242c17d470186815706610"
             ],
             "markers": "python_version >= '3.6'",
@@ -870,139 +804,353 @@
             "hashes": [
                 "sha256:17894355e7d2b305cd832d717708384017c1698a90ce24f6f7fbf0242dd0a688"
             ],
             "version": "==0.0.9"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pyinstaller": {
             "hashes": [
-                "sha256:12ca6567be457826e14416637ea54485a185d0ce7a5a044df0d0daf588fff6d1",
-                "sha256:2ba42038b3bd83e1fba7c8eb9e7cde43bd5938e37ca542c89e8779355d213f52",
-                "sha256:2bde16a8d664e8eba9aa7b84f729f7ab005c1793be4fe1986b3c9cad6c486622",
-                "sha256:3b2c34c3c3ddf38f68d9f5afbed82abe0f89d53014c56892326fef10172ee652",
-                "sha256:4b21b0298db44f5f07fc04d8ff81ec31efa47b72798efaecc4e811c50a102111",
-                "sha256:6cf6c032c72ef78fd9aa5e47d8952e784db45b2c3f7862bd44a99df68c216f64",
-                "sha256:8476538aec8a0a3be4f74b93388bd6989b91cc437ff86d6f0d3a68961176dce6",
-                "sha256:93d7e8443a6b60745d42aa50f08730f6b419410832b4c616c4f1bb315f087661",
-                "sha256:c7dd156c2438f197c168b990bbce03c97d3fb758dd9bbc3ca93626c2f4473a47",
-                "sha256:d1ff94347183ae3755cfb8f02e64744eb7fe384469bd61e453c6ff59a81665d6",
-                "sha256:dcd348b174fd72c4df271790ac582969c9423cb099fe92db9ec131a8a9243d5a",
-                "sha256:e7a4c292810285c2466f3bdcb1e03ba2170177ebe3d7054ff1af3bb348bf61a4"
+                "sha256:036a062a228af41f6bb6370a4e87cef34858cc839200a07ace7f8738ef64ad86",
+                "sha256:049cdc3524aefb5ca015a63d2c81b6bf1567cc818ac066859fbfde702c6165d3",
+                "sha256:0af9d11a09ce217d32f95c79c984054457b310671387ff32bae1496876308556",
+                "sha256:2a1fe6d0da22f207cfa4b3221fe365503cba071c77aac19f76a75503f67d9ff9",
+                "sha256:42fdea67e4c2217cedd54d17d1d402736df3ba718db2b497df65df5a68ae4f93",
+                "sha256:8454bac8f3cb2219a3ce2227fd039bdaf943dcba60e8c55732958ea3a6d81263",
+                "sha256:a445a91b85c9a1ea3985268643a674900dd86f244cc4be4ff4ec4c6367ff99a9",
+                "sha256:b3c6299fd7526c6ca87ea5f9017fb1928d47046df0b9f983d6bbd893801010dc",
+                "sha256:b4cac0e7b0d63c6a869843113008f59fd5b38b2959ffa6059e7fac4bb05de92b",
+                "sha256:b8a4f6834e5c85150948e22c74dd3ab8b98aa4ccdf964d880ac14d2f78d9c1a4",
+                "sha256:cb87cee0b3c81ccd74d4bf3f4faf03b5e1e39bb91f1a894b2ce4cd22363bf779",
+                "sha256:e359571327bbef434fc61324891399f9117efbb685b5065234eebb01713650a8"
             ],
             "index": "pypi",
-            "version": "==5.9.0"
+            "version": "==5.11.0"
         },
         "pyinstaller-hooks-contrib": {
             "hashes": [
-                "sha256:ab56c192e7cd4472ff6b840cda4fc42bceccc7fb4234f064fc834a3248c0afdd",
-                "sha256:d2ea40a7105651aa525bfe5fe309aa264d4d9bb49f839b862243dcf0a56c34cd"
+                "sha256:062ad7a1746e1cfc24d3a8c4be4e606fced3b123bda7d419f14fcf7507804b07",
+                "sha256:bb39e1038e3e0972420455e0b39cd9dce73f3d80acaf4bf2b3615fea766ff370"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2023.3"
+        },
+        "pymdown-extensions": {
+            "hashes": [
+                "sha256:ae66d84013c5d027ce055693e09a4628b67e9dec5bce05727e45b0918e36f274",
+                "sha256:b44e1093a43b8a975eae17b03c3a77aad4681b3b56fce60ce746dbef1944c8cb"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2023.1"
+            "version": "==10.0.1"
         },
         "pymsgbox": {
             "hashes": [
                 "sha256:2194227de8bff7a3d6da541848705a155dcbb2a06ee120d9f280a1d7f51263ff"
             ],
             "version": "==1.0.9"
         },
         "pyperclip": {
             "hashes": [
                 "sha256:105254a8b04934f0bc84e9c24eb360a591aaf6535c9def5f29d92af107a9bf57"
             ],
             "version": "==1.8.2"
         },
+        "pyproject-hooks": {
+            "hashes": [
+                "sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8",
+                "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==1.0.0"
+        },
         "pyrect": {
             "hashes": [
                 "sha256:f65155f6df9b929b67caffbd57c0947c5ae5449d3b580d178074bffb47a09b78"
             ],
             "version": "==0.2.0"
         },
+        "pyscreenshot": {
+            "hashes": [
+                "sha256:73d406d41a0977125bdfd2f6488f0caf1394e84d1d4c1065d5e8b1400b307096",
+                "sha256:8c0e93f0aef66a6bfe55a86abfced6bd396ae4b4f6cc1e36f04a28ad2625594d"
+            ],
+            "markers": "python_version >= '3.4'",
+            "version": "==3.1"
+        },
         "pyscreeze": {
             "hashes": [
-                "sha256:4428600ed19b30cd3f4b5d83767d198fc1dbae7439eecf9bd795445c009b67ae"
+                "sha256:d074547795e128da176599a6d4470500e425d49b05cf22e9808a7984c3612836"
             ],
-            "version": "==0.1.28"
+            "version": "==0.1.29"
         },
         "pytest": {
             "hashes": [
-                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
-                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
+                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
+                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==7.2.2"
+            "index": "pypi",
+            "version": "==7.3.1"
+        },
+        "pytest-cov": {
+            "hashes": [
+                "sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6",
+                "sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a"
+            ],
+            "index": "pypi",
+            "version": "==4.1.0"
+        },
+        "pytest-logbook": {
+            "hashes": [
+                "sha256:9454453230989a3d5149689c3449445554808d429b651a3d89c4464054a4c2dc",
+                "sha256:e2e79cf188fdae3fc7c857a168a9f18a5d9cca6234f38795b3ff628d23e2be17"
+            ],
+            "index": "pypi",
+            "version": "==1.2.0"
+        },
+        "pytest-mock": {
+            "hashes": [
+                "sha256:f4c973eeae0282963eb293eb173ce91b091a79c1334455acfac9ddee8a1c784b",
+                "sha256:fbbdb085ef7c252a326fd8cdcac0aa3b1333d8811f131bdcc701002e1be7ed4f"
+            ],
+            "index": "pypi",
+            "version": "==3.10.0"
+        },
+        "pytest-ordering": {
+            "hashes": [
+                "sha256:27fba3fc265f5d0f8597e7557885662c1bdc1969497cd58aff6ed21c3b617de2",
+                "sha256:3f314a178dbeb6777509548727dc69edf22d6d9a2867bf2d310ab85c403380b6",
+                "sha256:561ad653626bb171da78e682f6d39ac33bb13b3e272d406cd555adb6b006bda6"
+            ],
+            "index": "pypi",
+            "version": "==0.6"
+        },
+        "python-dateutil": {
+            "hashes": [
+                "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
+                "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
+            ],
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
+            "version": "==2.8.2"
         },
         "pytweening": {
             "hashes": [
-                "sha256:8533282cf70b31de8a0499e1cf420930b0013c787118872b2ec899382792e2e6"
+                "sha256:767134f1bf57b76c1ce9f692dd1cfc776d9a279de6724e8d04854508fd7ededb"
             ],
-            "version": "==1.0.4"
+            "markers": "python_version >= '2.7'",
+            "version": "==1.0.7"
         },
         "pywin32-ctypes": {
             "hashes": [
                 "sha256:24ffc3b341d457d48e8922352130cf2644024a4ff09762a2261fd34c36ee5942",
                 "sha256:9dc2d991b3479cc2df15930958b674a48a227d5361d413827a4cfd0b5876fc98"
             ],
             "markers": "sys_platform == 'win32'",
             "version": "==0.2.0"
         },
+        "pyyaml": {
+            "hashes": [
+                "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
+                "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
+                "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
+                "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
+                "sha256:0b4624f379dab24d3725ffde76559cff63d9ec94e1736b556dacdfebe5ab6d4b",
+                "sha256:0ce82d761c532fe4ec3f87fc45688bdd3a4c1dc5e0b4a19814b9009a29baefd4",
+                "sha256:1e4747bc279b4f613a09eb64bba2ba602d8a6664c6ce6396a4d0cd413a50ce07",
+                "sha256:213c60cd50106436cc818accf5baa1aba61c0189ff610f64f4a3e8c6726218ba",
+                "sha256:231710d57adfd809ef5d34183b8ed1eeae3f76459c18fb4a0b373ad56bedcdd9",
+                "sha256:277a0ef2981ca40581a47093e9e2d13b3f1fbbeffae064c1d21bfceba2030287",
+                "sha256:2cd5df3de48857ed0544b34e2d40e9fac445930039f3cfe4bcc592a1f836d513",
+                "sha256:40527857252b61eacd1d9af500c3337ba8deb8fc298940291486c465c8b46ec0",
+                "sha256:432557aa2c09802be39460360ddffd48156e30721f5e8d917f01d31694216782",
+                "sha256:473f9edb243cb1935ab5a084eb238d842fb8f404ed2193a915d1784b5a6b5fc0",
+                "sha256:48c346915c114f5fdb3ead70312bd042a953a8ce5c7106d5bfb1a5254e47da92",
+                "sha256:50602afada6d6cbfad699b0c7bb50d5ccffa7e46a3d738092afddc1f9758427f",
+                "sha256:68fb519c14306fec9720a2a5b45bc9f0c8d1b9c72adf45c37baedfcd949c35a2",
+                "sha256:77f396e6ef4c73fdc33a9157446466f1cff553d979bd00ecb64385760c6babdc",
+                "sha256:81957921f441d50af23654aa6c5e5eaf9b06aba7f0a19c18a538dc7ef291c5a1",
+                "sha256:819b3830a1543db06c4d4b865e70ded25be52a2e0631ccd2f6a47a2822f2fd7c",
+                "sha256:897b80890765f037df3403d22bab41627ca8811ae55e9a722fd0392850ec4d86",
+                "sha256:98c4d36e99714e55cfbaaee6dd5badbc9a1ec339ebfc3b1f52e293aee6bb71a4",
+                "sha256:9df7ed3b3d2e0ecfe09e14741b857df43adb5a3ddadc919a2d94fbdf78fea53c",
+                "sha256:9fa600030013c4de8165339db93d182b9431076eb98eb40ee068700c9c813e34",
+                "sha256:a80a78046a72361de73f8f395f1f1e49f956c6be882eed58505a15f3e430962b",
+                "sha256:afa17f5bc4d1b10afd4466fd3a44dc0e245382deca5b3c353d8b757f9e3ecb8d",
+                "sha256:b3d267842bf12586ba6c734f89d1f5b871df0273157918b0ccefa29deb05c21c",
+                "sha256:b5b9eccad747aabaaffbc6064800670f0c297e52c12754eb1d976c57e4f74dcb",
+                "sha256:bfaef573a63ba8923503d27530362590ff4f576c626d86a9fed95822a8255fd7",
+                "sha256:c5687b8d43cf58545ade1fe3e055f70eac7a5a1a0bf42824308d868289a95737",
+                "sha256:cba8c411ef271aa037d7357a2bc8f9ee8b58b9965831d9e51baf703280dc73d3",
+                "sha256:d15a181d1ecd0d4270dc32edb46f7cb7733c7c508857278d3d378d14d606db2d",
+                "sha256:d4b0ba9512519522b118090257be113b9468d804b19d63c71dbcf4a48fa32358",
+                "sha256:d4db7c7aef085872ef65a8fd7d6d09a14ae91f691dec3e87ee5ee0539d516f53",
+                "sha256:d4eccecf9adf6fbcc6861a38015c2a64f38b9d94838ac1810a9023a0609e1b78",
+                "sha256:d67d839ede4ed1b28a4e8909735fc992a923cdb84e618544973d7dfc71540803",
+                "sha256:daf496c58a8c52083df09b80c860005194014c3698698d1a57cbcfa182142a3a",
+                "sha256:dbad0e9d368bb989f4515da330b88a057617d16b6a8245084f1b05400f24609f",
+                "sha256:e61ceaab6f49fb8bdfaa0f92c4b57bcfbea54c09277b1b4f7ac376bfb7a7c174",
+                "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==6.0"
+        },
+        "pyyaml-env-tag": {
+            "hashes": [
+                "sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb",
+                "sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==0.1"
+        },
         "readme-renderer": {
             "hashes": [
                 "sha256:cd653186dfc73055656f090f227f5cb22a046d7f71a841dfa305f55c9a513273",
                 "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==37.3"
         },
+        "regex": {
+            "hashes": [
+                "sha256:0385e73da22363778ef2324950e08b689abdf0b108a7d8decb403ad7f5191938",
+                "sha256:051da80e6eeb6e239e394ae60704d2b566aa6a7aed6f2890a7967307267a5dc6",
+                "sha256:05ed27acdf4465c95826962528f9e8d41dbf9b1aa8531a387dee6ed215a3e9ef",
+                "sha256:0654bca0cdf28a5956c83839162692725159f4cda8d63e0911a2c0dc76166525",
+                "sha256:09e4a1a6acc39294a36b7338819b10baceb227f7f7dbbea0506d419b5a1dd8af",
+                "sha256:0b49c764f88a79160fa64f9a7b425620e87c9f46095ef9c9920542ab2495c8bc",
+                "sha256:0b71e63226e393b534105fcbdd8740410dc6b0854c2bfa39bbda6b0d40e59a54",
+                "sha256:0c29ca1bd61b16b67be247be87390ef1d1ef702800f91fbd1991f5c4421ebae8",
+                "sha256:10590510780b7541969287512d1b43f19f965c2ece6c9b1c00fc367b29d8dce7",
+                "sha256:10cb847aeb1728412c666ab2e2000ba6f174f25b2bdc7292e7dd71b16db07568",
+                "sha256:12b74fbbf6cbbf9dbce20eb9b5879469e97aeeaa874145517563cca4029db65c",
+                "sha256:20326216cc2afe69b6e98528160b225d72f85ab080cbdf0b11528cbbaba2248f",
+                "sha256:2239d95d8e243658b8dbb36b12bd10c33ad6e6933a54d36ff053713f129aa536",
+                "sha256:25be746a8ec7bc7b082783216de8e9473803706723b3f6bef34b3d0ed03d57e2",
+                "sha256:271f0bdba3c70b58e6f500b205d10a36fb4b58bd06ac61381b68de66442efddb",
+                "sha256:29cdd471ebf9e0f2fb3cac165efedc3c58db841d83a518b082077e612d3ee5df",
+                "sha256:2d44dc13229905ae96dd2ae2dd7cebf824ee92bc52e8cf03dcead37d926da019",
+                "sha256:3676f1dd082be28b1266c93f618ee07741b704ab7b68501a173ce7d8d0d0ca18",
+                "sha256:36efeba71c6539d23c4643be88295ce8c82c88bbd7c65e8a24081d2ca123da3f",
+                "sha256:3e5219bf9e75993d73ab3d25985c857c77e614525fac9ae02b1bebd92f7cecac",
+                "sha256:43e1dd9d12df9004246bacb79a0e5886b3b6071b32e41f83b0acbf293f820ee8",
+                "sha256:457b6cce21bee41ac292d6753d5e94dcbc5c9e3e3a834da285b0bde7aa4a11e9",
+                "sha256:463b6a3ceb5ca952e66550a4532cef94c9a0c80dc156c4cc343041951aec1697",
+                "sha256:4959e8bcbfda5146477d21c3a8ad81b185cd252f3d0d6e4724a5ef11c012fb06",
+                "sha256:4d3850beab9f527f06ccc94b446c864059c57651b3f911fddb8d9d3ec1d1b25d",
+                "sha256:5708089ed5b40a7b2dc561e0c8baa9535b77771b64a8330b684823cfd5116036",
+                "sha256:5c6b48d0fa50d8f4df3daf451be7f9689c2bde1a52b1225c5926e3f54b6a9ed1",
+                "sha256:61474f0b41fe1a80e8dfa70f70ea1e047387b7cd01c85ec88fa44f5d7561d787",
+                "sha256:6343c6928282c1f6a9db41f5fd551662310e8774c0e5ebccb767002fcf663ca9",
+                "sha256:65ba8603753cec91c71de423a943ba506363b0e5c3fdb913ef8f9caa14b2c7e0",
+                "sha256:687ea9d78a4b1cf82f8479cab23678aff723108df3edeac098e5b2498879f4a7",
+                "sha256:6b2675068c8b56f6bfd5a2bda55b8accbb96c02fd563704732fd1c95e2083461",
+                "sha256:7117d10690c38a622e54c432dfbbd3cbd92f09401d622902c32f6d377e2300ee",
+                "sha256:7178bbc1b2ec40eaca599d13c092079bf529679bf0371c602edaa555e10b41c3",
+                "sha256:72d1a25bf36d2050ceb35b517afe13864865268dfb45910e2e17a84be6cbfeb0",
+                "sha256:742e19a90d9bb2f4a6cf2862b8b06dea5e09b96c9f2df1779e53432d7275331f",
+                "sha256:74390d18c75054947e4194019077e243c06fbb62e541d8817a0fa822ea310c14",
+                "sha256:74419d2b50ecb98360cfaa2974da8689cb3b45b9deff0dcf489c0d333bcc1477",
+                "sha256:824bf3ac11001849aec3fa1d69abcb67aac3e150a933963fb12bda5151fe1bfd",
+                "sha256:83320a09188e0e6c39088355d423aa9d056ad57a0b6c6381b300ec1a04ec3d16",
+                "sha256:837328d14cde912af625d5f303ec29f7e28cdab588674897baafaf505341f2fc",
+                "sha256:841d6e0e5663d4c7b4c8099c9997be748677d46cbf43f9f471150e560791f7ff",
+                "sha256:87b2a5bb5e78ee0ad1de71c664d6eb536dc3947a46a69182a90f4410f5e3f7dd",
+                "sha256:890e5a11c97cf0d0c550eb661b937a1e45431ffa79803b942a057c4fb12a2da2",
+                "sha256:8abbc5d54ea0ee80e37fef009e3cec5dafd722ed3c829126253d3e22f3846f1e",
+                "sha256:8e3f1316c2293e5469f8f09dc2d76efb6c3982d3da91ba95061a7e69489a14ef",
+                "sha256:8f56fcb7ff7bf7404becdfc60b1e81a6d0561807051fd2f1860b0d0348156a07",
+                "sha256:9427a399501818a7564f8c90eced1e9e20709ece36be701f394ada99890ea4b3",
+                "sha256:976d7a304b59ede34ca2921305b57356694f9e6879db323fd90a80f865d355a3",
+                "sha256:9a5bfb3004f2144a084a16ce19ca56b8ac46e6fd0651f54269fc9e230edb5e4a",
+                "sha256:9beb322958aaca059f34975b0df135181f2e5d7a13b84d3e0e45434749cb20f7",
+                "sha256:9edcbad1f8a407e450fbac88d89e04e0b99a08473f666a3f3de0fd292badb6aa",
+                "sha256:9edce5281f965cf135e19840f4d93d55b3835122aa76ccacfd389e880ba4cf82",
+                "sha256:a4c3b7fa4cdaa69268748665a1a6ff70c014d39bb69c50fda64b396c9116cf77",
+                "sha256:a8105e9af3b029f243ab11ad47c19b566482c150c754e4c717900a798806b222",
+                "sha256:a99b50300df5add73d307cf66abea093304a07eb017bce94f01e795090dea87c",
+                "sha256:aad51907d74fc183033ad796dd4c2e080d1adcc4fd3c0fd4fd499f30c03011cd",
+                "sha256:af4dd387354dc83a3bff67127a124c21116feb0d2ef536805c454721c5d7993d",
+                "sha256:b28f5024a3a041009eb4c333863d7894d191215b39576535c6734cd88b0fcb68",
+                "sha256:b4598b1897837067a57b08147a68ac026c1e73b31ef6e36deeeb1fa60b2933c9",
+                "sha256:b6192d5af2ccd2a38877bfef086d35e6659566a335b1492786ff254c168b1693",
+                "sha256:b862c2b9d5ae38a68b92e215b93f98d4c5e9454fa36aae4450f61dd33ff48487",
+                "sha256:b956231ebdc45f5b7a2e1f90f66a12be9610ce775fe1b1d50414aac1e9206c06",
+                "sha256:bb60b503ec8a6e4e3e03a681072fa3a5adcbfa5479fa2d898ae2b4a8e24c4591",
+                "sha256:bbb02fd4462f37060122e5acacec78e49c0fbb303c30dd49c7f493cf21fc5b27",
+                "sha256:bdff5eab10e59cf26bc479f565e25ed71a7d041d1ded04ccf9aee1d9f208487a",
+                "sha256:c123f662be8ec5ab4ea72ea300359023a5d1df095b7ead76fedcd8babbedf969",
+                "sha256:c2b867c17a7a7ae44c43ebbeb1b5ff406b3e8d5b3e14662683e5e66e6cc868d3",
+                "sha256:c5f8037000eb21e4823aa485149f2299eb589f8d1fe4b448036d230c3f4e68e0",
+                "sha256:c6a57b742133830eec44d9b2290daf5cbe0a2f1d6acee1b3c7b1c7b2f3606df7",
+                "sha256:ccf91346b7bd20c790310c4147eee6ed495a54ddb6737162a36ce9dbef3e4751",
+                "sha256:cf67ca618b4fd34aee78740bea954d7c69fdda419eb208c2c0c7060bb822d747",
+                "sha256:d2da3abc88711bce7557412310dfa50327d5769a31d1c894b58eb256459dc289",
+                "sha256:d4f03bb71d482f979bda92e1427f3ec9b220e62a7dd337af0aa6b47bf4498f72",
+                "sha256:d54af539295392611e7efbe94e827311eb8b29668e2b3f4cadcfe6f46df9c777",
+                "sha256:d77f09bc4b55d4bf7cc5eba785d87001d6757b7c9eec237fe2af57aba1a071d9",
+                "sha256:d831c2f8ff278179705ca59f7e8524069c1a989e716a1874d6d1aab6119d91d1",
+                "sha256:dbbbfce33cd98f97f6bffb17801b0576e653f4fdb1d399b2ea89638bc8d08ae1",
+                "sha256:dcba6dae7de533c876255317c11f3abe4907ba7d9aa15d13e3d9710d4315ec0e",
+                "sha256:e0bb18053dfcfed432cc3ac632b5e5e5c5b7e55fb3f8090e867bfd9b054dbcbf",
+                "sha256:e2fbd6236aae3b7f9d514312cdb58e6494ee1c76a9948adde6eba33eb1c4264f",
+                "sha256:e5087a3c59eef624a4591ef9eaa6e9a8d8a94c779dade95d27c0bc24650261cd",
+                "sha256:e8915cc96abeb8983cea1df3c939e3c6e1ac778340c17732eb63bb96247b91d2",
+                "sha256:ea353ecb6ab5f7e7d2f4372b1e779796ebd7b37352d290096978fea83c4dba0c",
+                "sha256:ee2d1a9a253b1729bb2de27d41f696ae893507c7db224436abe83ee25356f5c1",
+                "sha256:f415f802fbcafed5dcc694c13b1292f07fe0befdb94aa8a52905bd115ff41e88",
+                "sha256:fb5ec16523dc573a4b277663a2b5a364e2099902d3944c9419a40ebd56a118f9",
+                "sha256:fea75c3710d4f31389eed3c02f62d0b66a9da282521075061ce875eb5300cf23"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==2023.6.3"
+        },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f",
+                "sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.31.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
-                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
+                "sha256:76f6b65ea7e5c5d924ba80e322231d7cb5b5981aa60bfc1e694f1bc097fe6fe1",
+                "sha256:d204aadb50b936bf6b1a695385429d192bc1fdaf3e8b907e8e26f4c4e4b5bf75"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.3"
+            "version": "==13.4.1"
         },
         "setuptools": {
             "hashes": [
-                "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a",
-                "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"
+                "sha256:5df61bf30bb10c6f756eb19e7c9f3b473051f48db77fddbe06ff2ca307df9a6f",
+                "sha256:62642358adc77ffa87233bc4d2354c4b2682d214048f500964dbe760ccedf102"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.6.1"
+            "version": "==67.8.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
@@ -1013,35 +1161,35 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:0dac3b698538ffef41716cf97ba26c1c7788dba73ce6f150c1ff5b4720786dd2",
-                "sha256:807d1cb3d6be87eb78a381c3e70ebd8d346b9a25f3753e9947e866b2786865fc"
+                "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b",
+                "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"
             ],
-            "markers": "python_version >= '3.8'",
-            "version": "==6.1.3"
+            "index": "pypi",
+            "version": "==6.2.1"
         },
         "sphinx-intl": {
             "hashes": [
                 "sha256:9798946b995989de691387651d70c3fc191275b587e2e519655541edfd7bbd68",
                 "sha256:9d9849ae42515b39786824e99f1e30db0404c377b01bb022690fc932b0221c02"
             ],
             "index": "pypi",
             "version": "==2.1.0"
         },
         "sphinx-rtd-theme": {
             "hashes": [
-                "sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8",
-                "sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2"
+                "sha256:01c5c5a72e2d025bd23d1f06c59a4831b06e6ce6c01fdd5ebfe9986c0a880fc7",
+                "sha256:6a7e7d8af34eb8fc57d52a09c6b6b9c46ff44aea5951bc831eeb9245378f3689"
             ],
             "index": "pypi",
-            "version": "==1.2.0"
+            "version": "==1.2.2"
         },
         "sphinxcontrib-applehelp": {
             "hashes": [
                 "sha256:29d341f67fb0f6f586b23ad80e072c8e6ad0b48417db2bde114a4c9746feb228",
                 "sha256:828f867945bbe39817c210a1abfd1bc4895c8b73fcaade56d45357a348a07d7e"
             ],
             "markers": "python_version >= '3.8'",
@@ -1064,15 +1212,15 @@
             "version": "==2.0.1"
         },
         "sphinxcontrib-jquery": {
             "hashes": [
                 "sha256:1620739f04e36a2c779f1a131a2dfd49b2fd07351bf1968ced074365933abc7a",
                 "sha256:f936030d7d0147dd026a4f2b5a57343d233f1fc7b363f68b3d4f1cb0993878ae"
             ],
-            "markers": "python_version >= '3.1'",
+            "markers": "python_version >= '2.7'",
             "version": "==4.1"
         },
         "sphinxcontrib-jsmath": {
             "hashes": [
                 "sha256:2ec2eaebfb78f3f2078e73666b1415417a116cc848b72e5172e596c871103178",
                 "sha256:a9925e4a4587247ed2191a22df5f6970656cb8ca2bd6284309578f2153e0c4b8"
             ],
@@ -1091,37 +1239,62 @@
             "hashes": [
                 "sha256:352a9a00ae864471d3a7ead8d7d79f5fc0b57e8b3f95e9867eb9eb28999b92fd",
                 "sha256:aa5f6de5dfdf809ef505c4895e51ef5c9eac17d0f287933eb49ec495280b6952"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==1.1.5"
         },
-        "tomli": {
-            "hashes": [
-                "sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc",
-                "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
-            ],
-            "markers": "python_version < '3.11'",
-            "version": "==2.0.1"
-        },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
             "version": "==4.0.2"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.3"
+        },
+        "watchdog": {
+            "hashes": [
+                "sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a",
+                "sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100",
+                "sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8",
+                "sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc",
+                "sha256:2b57a1e730af3156d13b7fdddfc23dea6487fceca29fc75c5a868beed29177ae",
+                "sha256:336adfc6f5cc4e037d52db31194f7581ff744b67382eb6021c868322e32eef41",
+                "sha256:3aa7f6a12e831ddfe78cdd4f8996af9cf334fd6346531b16cec61c3b3c0d8da0",
+                "sha256:3ed7c71a9dccfe838c2f0b6314ed0d9b22e77d268c67e015450a29036a81f60f",
+                "sha256:4c9956d27be0bb08fc5f30d9d0179a855436e655f046d288e2bcc11adfae893c",
+                "sha256:4d98a320595da7a7c5a18fc48cb633c2e73cda78f93cac2ef42d42bf609a33f9",
+                "sha256:4f94069eb16657d2c6faada4624c39464f65c05606af50bb7902e036e3219be3",
+                "sha256:5113334cf8cf0ac8cd45e1f8309a603291b614191c9add34d33075727a967709",
+                "sha256:51f90f73b4697bac9c9a78394c3acbbd331ccd3655c11be1a15ae6fe289a8c83",
+                "sha256:5d9f3a10e02d7371cd929b5d8f11e87d4bad890212ed3901f9b4d68767bee759",
+                "sha256:7ade88d0d778b1b222adebcc0927428f883db07017618a5e684fd03b83342bd9",
+                "sha256:7c5f84b5194c24dd573fa6472685b2a27cc5a17fe5f7b6fd40345378ca6812e3",
+                "sha256:7e447d172af52ad204d19982739aa2346245cc5ba6f579d16dac4bfec226d2e7",
+                "sha256:8ae9cda41fa114e28faf86cb137d751a17ffd0316d1c34ccf2235e8a84365c7f",
+                "sha256:8f3ceecd20d71067c7fd4c9e832d4e22584318983cabc013dbf3f70ea95de346",
+                "sha256:9fac43a7466eb73e64a9940ac9ed6369baa39b3bf221ae23493a9ec4d0022674",
+                "sha256:a70a8dcde91be523c35b2bf96196edc5730edb347e374c7de7cd20c43ed95397",
+                "sha256:adfdeab2da79ea2f76f87eb42a3ab1966a5313e5a69a0213a3cc06ef692b0e96",
+                "sha256:ba07e92756c97e3aca0912b5cbc4e5ad802f4557212788e72a72a47ff376950d",
+                "sha256:c07253088265c363d1ddf4b3cdb808d59a0468ecd017770ed716991620b8f77a",
+                "sha256:c9d8c8ec7efb887333cf71e328e39cffbf771d8f8f95d308ea4125bf5f90ba64",
+                "sha256:d00e6be486affb5781468457b21a6cbe848c33ef43f9ea4a73b4882e5f188a44",
+                "sha256:d429c2430c93b7903914e4db9a966c7f2b068dd2ebdd2fa9b9ce094c7d459f33"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==3.0.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `auraboros-0.9.0a0/assets/fonts/misaki_gothic.ttf` & `auraboros-1.0.0a0/assets/fonts/misaki_gothic.ttf`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/enemy_a.piskel` & `auraboros-1.0.0a0/assets/imgs/enemy_a.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/enemy_a.png` & `auraboros-1.0.0a0/assets/imgs/enemy_a.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/enemy_b.piskel` & `auraboros-1.0.0a0/assets/imgs/enemy_b.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/enemy_b.png` & `auraboros-1.0.0a0/assets/imgs/enemy_b.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/explosion_a.piskel` & `auraboros-1.0.0a0/assets/imgs/explosion_a.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/explosion_a.png` & `auraboros-1.0.0a0/assets/imgs/explosion_a.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/explosion_b.png` & `auraboros-1.0.0a0/assets/imgs/explosion_b.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/fighter_a.piskel` & `auraboros-1.0.0a0/assets/imgs/fighter_a.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/fighter_a.png` & `auraboros-1.0.0a0/assets/imgs/fighter_a.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/icon.ico` & `auraboros-1.0.0a0/assets/imgs/icon.ico`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/scoutdisk.piskel` & `auraboros-1.0.0a0/assets/imgs/scoutdisk.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/scoutdisk.png` & `auraboros-1.0.0a0/assets/imgs/scoutdisk.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/shot6.piskel` & `auraboros-1.0.0a0/assets/imgs/shot6.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/imgs/terrain_rock.png` & `auraboros-1.0.0a0/assets/imgs/terrain_rock.png`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/level_data/debug1/patterns.json` & `auraboros-1.0.0a0/assets/level_data/debug1/patterns.json`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/level_data/stage1/patterns.json` & `auraboros-1.0.0a0/assets/level_data/stage1/patterns.json`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/sounds/deathse2.wav` & `auraboros-1.0.0a0/assets/sounds/deathse2.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/sounds/deathse3.wav` & `auraboros-1.0.0a0/assets/sounds/deathse3.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/sounds/deathse4.wav` & `auraboros-1.0.0a0/assets/sounds/deathse4.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/sounds/explosion1.wav` & `auraboros-1.0.0a0/assets/sounds/explosion1.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/sounds/explosion2.wav` & `auraboros-1.0.0a0/assets/sounds/explosion2.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/sounds/laser.wav` & `auraboros-1.0.0a0/assets/sounds/laser.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/sounds/laser2.wav` & `auraboros-1.0.0a0/assets/sounds/laser2.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/sounds/shot1.wav` & `auraboros-1.0.0a0/assets/sounds/shot1.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/sounds/music/bgm1.wav` & `auraboros-1.0.0a0/assets/sounds/music/bgm1.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/assets/sounds/music/gameover.wav` & `auraboros-1.0.0a0/assets/sounds/music/gameover.wav`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/src/auraboros/gamescene.py` & `auraboros-1.0.0a0/src/auraboros/gamescene.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,132 @@
-
 from dataclasses import dataclass
-# from typing import Optional, Union
+from typing import Any, Callable
 
 import pygame
 
-from .animation import AnimationImage
-from .gameinput2 import KeyboardManager
+from .core import Global
+# from .animation import AnimationImage
+# from .gameinput import KeyboardManager, Mouse
 
 
 @dataclass
-class Scene(object):
+class State:
+    script: Callable
+
+
+class StateMachine:
+    def __init__(self):
+        self.states: dict[str, State] = {}
+        self.current_state_name: str = ""
+
+    @property
+    def current_state(self) -> State:
+        return self.states[self.current_state_name]
+
+    def add_state(self, name: str, state: State):
+        self.states[name] = state
+
+    def is_state_exist(self, name: str) -> bool:
+        return name in self.states.keys()
+
+    def is_current_state(self, name: str) -> bool:
+        return self.current_state_name == name
+
+    def trans_to(self, state_name: str):
+        if self.is_state_exist(state_name):
+            self.current_state_name = state_name
+
+    def run_script_on_state(self) -> Any:
+        return self.current_state.script()
+
 
-    def __init__(self, manager):
-        from .gamelevel import Level
+class Scene:
+    """
+    Examples:
+        class ExampleScene(Scene):
+            def setup(self):
+                """"use instead of __init__""""
+
+            def event(self, event: pygame.event.Event):
+                pass
+
+            def update(self):
+                pass
+
+            def draw(self):
+                pass
+    """
+
+    def __init__(self, manager: "SceneManager"):
         self.manager = manager
-        self.gameworld: Level = None
-        self.keyboard: KeyboardManager = KeyboardManager()
-        # self._joystick: Joystick2 = None
-        self.visual_effects: list[AnimationImage] = []
-        attrs_of_class = set(dir(self.__class__)) - set(dir(Scene))
-        for attr_name in attrs_of_class:
-            attrs_of_object = set(
-                getattr(self, attr_name).__class__.__mro__) - {object, }
-            is_gameworld = Level in attrs_of_object
-            if is_gameworld:
-                getattr(self, attr_name).scene = self
-
-    # @property
-    # def joystick(self) -> Optional[Joystick2]:
-    #     return self._joystick
-
-    # @joystick.setter
-    # def joystick(self, value: Union[Joystick2, None]):
-    #     self._joystick = value
+        self.statemachine: StateMachine = StateMachine()
+        self._is_setup_finished = False  # turn True by SceneManager
+
+    def setup(self):
+        """
+        This method is called on scene transitions
+        or if this scene is the first scene.
+        """
+        pass
 
-    def event(self, event: pygame.event):
+    def event(self, event: pygame.event.Event):
         pass
 
     def draw(self, screen: pygame.surface.Surface):
         pass
 
-    def update(self, ):
+    def update(self, dt):
         pass
 
 
 class SceneManager:
     def __init__(self):
         self.scenes: list[Scene] = []
-        self._current: int = 0
+        self._current: int = 0  # -1 means exit app
+        self.__is_finished_setup_of_first_scene = False
 
     @property
     def current(self):
         return self._current
 
     @current.setter
     def current(self, value):
         self._current = value
 
-    def event(self, event: pygame.event):
-        """return False as a signal of quit app"""
+    def event(self, event: pygame.event.Event) -> bool:
+        """return False to notify whether quit event is fired"""
         if event.type == pygame.QUIT:
             return False
         if self.current == -1:
             return False
+        if self.scenes == []:
+            return True
+        if not self.scenes[self.current]._is_setup_finished:
+            return True
         self.scenes[self.current].event(event)
-        if self.scenes[self.current].keyboard.current_setup is not None:
-            self.scenes[self.current].keyboard.current_setup.event(event)
-        # if self.scenes[self.current].joystick is not None:
-        #     self.scenes[self.current].joystick.event(event)
         return True
 
-    def is_current_scene_has_gameworld(self) -> bool:
-        if self.scenes[self.current].gameworld is None:
-            return False
-        else:
-            return True
-
-    def update(self):
-        self.scenes[self.current].update()
-        if self.is_current_scene_has_gameworld():
-            if not self.scenes[self.current].gameworld.pause:
-                [entity.update()
-                 for entity in self.scenes[self.current].gameworld.entities]
-        [visual_effect.update()
-         for visual_effect in self.scenes[self.current].visual_effects]
+    def update(self, dt):
+        if self.scenes == []:
+            return
+        if not self.__is_finished_setup_of_first_scene:
+            if Global.is_initialized:
+                self.scenes[0].setup()
+                self.__is_finished_setup_of_first_scene = True
+                self.scenes[0]._is_setup_finished = True
+        self.scenes[self.current].update(dt)
 
     def draw(self, screen: pygame.surface.Surface):
+        if self.scenes == []:
+            return
         self.scenes[self.current].draw(screen)
-        if self.is_current_scene_has_gameworld():
-            if not self.scenes[self.current].gameworld.pause:
-                [entity.draw(screen)
-                 for entity in self.scenes[self.current].gameworld.entities]
-        [visual_effect.draw(screen)
-         for visual_effect in self.scenes[self.current].visual_effects]
-        # Delete finished animations
-        [self.scenes[self.current].visual_effects.pop(i)
-         for i, visual_effect in enumerate(
-            self.scenes[self.current].visual_effects)
-         if visual_effect.was_played_once]
 
-    def push(self, scene: Scene):
+    def add(self, scene: Scene):
         self.scenes.append(scene)
 
     def pop(self):
         self.scenes.pop()
 
-    def transition_to(self, index):
-        if self.scenes[self.current].keyboard.current_setup is not None:
-            self.scenes[
-                self.current].keyboard.current_setup.release_all_of_keys()
+    def transition_to(self, index: int):
         self.current = index
+        self.scenes[self.current].setup()
+        self.scenes[self.current]._is_setup_finished = True
```

### Comparing `auraboros-0.9.0a0/src/debugs/animation.py` & `auraboros-1.0.0a0/src/auraboros/examples/deprecated/animationimage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,150 +1,189 @@
-
 # from collections import deque
 from pathlib import Path
 import sys
+
 # from string import ascii_lowercase
 
 import pygame
 
-import init_for_dev  # noqa
+import setup_syspath  # noqa
 from auraboros import engine
-from auraboros.utilities import AssetFilePath, draw_grid_background
+from auraboros.animation import AnimationImage, SpriteSheet
 from auraboros.gametext import TextSurfaceFactory
 from auraboros.gamescene import Scene, SceneManager
-from auraboros.gameinput2 import Keyboard
-from auraboros.ui import GameMenuSystem, GameMenuUI, MsgWindow
-from auraboros.animation2 import AnimationImage, SpriteSheet
+from auraboros.gameinput import Keyboard
+from auraboros.oldold_ui import GameMenuSystem, GameMenuUI, MsgWindow
+from auraboros.utils import AssetFilePath, draw_grid, pos_on_pixel_scale
+from auraboros.schedule import Stopwatch
 from auraboros import global_
 
-engine.init(caption="Test Animation System")
+engine.init(caption="Test AnimationImage System")
 
 AssetFilePath.set_asset_root(Path(sys.argv[0]).parent / "assets")
 
 textfactory = TextSurfaceFactory()
 textfactory.register_font(
-    "misaki_gothic",
-    pygame.font.Font(AssetFilePath.font("misaki_gothic.ttf"), 16))
+    "misaki_gothic", pygame.font.Font(AssetFilePath.font("misaki_gothic.ttf"), 16)
+)
 
 
 class TestAnimImg(AnimationImage):
     def __init__(self):
         super().__init__()
         self.sprite_sheet = SpriteSheet(AssetFilePath.img("testsprite.png"))
         self.anim_frames: list[pygame.surface.Surface] = [
             self.sprite_sheet.image_by_area(0, 0, 32, 32),
             self.sprite_sheet.image_by_area(0, 32, 32, 32),
-            self.sprite_sheet.image_by_area(0, 32*2, 32, 32),
-            self.sprite_sheet.image_by_area(0, 32*3, 32, 32),
-            self.sprite_sheet.image_by_area(0, 32*4, 32, 32),
-            self.sprite_sheet.image_by_area(0, 32*3, 32, 32),
-            self.sprite_sheet.image_by_area(0, 32*2, 32, 32),
-            self.sprite_sheet.image_by_area(0, 32, 32, 32)]
-        self.anim_interval = 500
-        self.loop_count = 2
+            self.sprite_sheet.image_by_area(0, 32 * 2, 32, 32),
+            self.sprite_sheet.image_by_area(0, 32 * 3, 32, 32),
+            self.sprite_sheet.image_by_area(0, 32 * 4, 32, 32),
+            self.sprite_sheet.image_by_area(0, 32 * 3, 32, 32),
+            self.sprite_sheet.image_by_area(0, 32 * 2, 32, 32),
+            self.sprite_sheet.image_by_area(0, 32, 32, 32),
+        ]
+        self.anim_interval = 1000
+        self.loop_count = 1
 
 
-class GameMenuDebugScene(Scene):
+class DebugScene(Scene):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         textfactory.set_current_font("misaki_gothic")
         self.test_anim_img = TestAnimImg()
         self.keyboard["menu"] = Keyboard()
         self.keyboard.set_current_setup("menu")
         self.menusystem = GameMenuSystem()
         self.keyboard["menu"].register_keyaction(
-            pygame.K_UP, 0, 122, self.menusystem.menu_cursor_up)
+            pygame.K_UP, 0, 122, 122, self.menusystem.menu_cursor_up
+        )
         self.keyboard["menu"].register_keyaction(
-            pygame.K_DOWN, 0, 122, self.menusystem.menu_cursor_down)
+            pygame.K_DOWN, 0, 122, 122, self.menusystem.menu_cursor_down
+        )
         self.keyboard["menu"].register_keyaction(
-            pygame.K_z, 0, 0, self.menusystem.do_selected_action)
-        self.menusystem.add_menu_item(
-            "play", self.play_animation, text="Play")
-        self.menusystem.add_menu_item(
-            "stop", self.stop_animation, text="STOP")
-        self.menusystem.add_menu_item(
-            "reset", self.reset_animation, text="RESET")
+            pygame.K_z, 0, 0, 0, self.menusystem.do_selected_action
+        )
+        self.menusystem.add_menu_item("play", self.play_animation, text="Play")
+        self.menusystem.add_menu_item("stop", self.stop_animation, text="STOP")
+        self.menusystem.add_menu_item("reset", self.reset_animation, text="RESET")
         self.menuui = GameMenuUI(self.menusystem, textfactory, "filled_box")
         self.menuui.padding = 4
         self.msgbox = MsgWindow(textfactory.font())
         self.msgbox.padding = 4
         self.msgbox.text = "Press 'Z'"
-        self.loop_count_msgbox = MsgWindow(textfactory.font())
-        self.loop_count_msgbox.padding = 4
-        self.anim_interval_msgbox = MsgWindow(textfactory.font())
-        self.anim_interval_msgbox.padding = 4
-        self.anim_frame_id_msgbox = MsgWindow(textfactory.font())
-        self.anim_frame_id_msgbox.padding = 4
-        self.is_playing_msgbox = MsgWindow(textfactory.font())
-        self.is_playing_msgbox.padding = 4
-        self.loop_counter_msgbox = MsgWindow(textfactory.font())
-        self.loop_counter_msgbox.padding = 4
+        self.msgbox2 = MsgWindow(textfactory.font())
+        self.msgbox2.padding = 4
+        self.msgbox3 = MsgWindow(textfactory.font())
+        self.msgbox3.padding = 4
+        self.msgbox4 = MsgWindow(textfactory.font())
+        self.msgbox4.padding = 4
+        self.msgbox5 = MsgWindow(textfactory.font())
+        self.msgbox5.padding = 4
+        self.msgbox6 = MsgWindow(textfactory.font())
+        self.msgbox6.padding = 4
+        self.msgbox7 = MsgWindow(textfactory.font())
+        self.msgbox7.padding = 4
+        self.msgbox8 = MsgWindow(textfactory.font())
+        self.msgbox8.padding = 4
+        self.stopwatch = Stopwatch()
+        self.mouse.register_mouseaction(
+            "down",
+            on_left=lambda: self.menuui.do_option_if_givenpos_on_ui(
+                pos_on_pixel_scale(pygame.mouse.get_pos())
+            ),
+        )
 
     def play_animation(self):
         self.test_anim_img.let_play()
+        self.stopwatch.start()
 
     def stop_animation(self):
         self.test_anim_img.let_stop()
+        self.stopwatch.stop()
 
     def reset_animation(self):
         self.test_anim_img.reset_animation()
-        pass
+        self.stopwatch.reset()
 
-    def update(self, ):
-        self.keyboard.current_setup.do_action_by_keyinput(pygame.K_UP)
-        self.keyboard.current_setup.do_action_by_keyinput(pygame.K_DOWN)
-        self.keyboard.current_setup.do_action_by_keyinput(pygame.K_z)
+    def update(self, dt):
+        if self.test_anim_img.is_all_loop_finished():
+            self.stopwatch.stop()
+        self.keyboard.current_setup.do_action_on_keyinput(pygame.K_UP)
+        self.keyboard.current_setup.do_action_on_keyinput(pygame.K_DOWN)
+        self.keyboard.current_setup.do_action_on_keyinput(pygame.K_z)
         self.menuui.set_pos_to_center()
         self.menusystem.update()
-        # self.test_anim_img
-        self.loop_count_msgbox.text = \
-            f"loop_count:{self.test_anim_img.loop_count}"
-        self.anim_interval_msgbox.text = \
+        self.menuui.highlight_option_on_givenpos(
+            pos_on_pixel_scale(pygame.mouse.get_pos())
+        )
+        self.msgbox2.text = f"loop_count:{self.test_anim_img.loop_count}"
+        self.msgbox3.text = (
             f"anim_interval:{self.test_anim_img.anim_interval} milliseconds"
-        self.anim_frame_id_msgbox.text = \
-            f"anim_frame_id:{self.test_anim_img.anim_frame_id}"
-        self.is_playing_msgbox.text = \
-            f"is_playing:{self.test_anim_img.is_playing}"
-        self.loop_counter_msgbox.text = \
-            f"loop_counter:{self.test_anim_img.loop_counter}"    
-        self.loop_count_msgbox.pos[1] = \
-            self.msgbox.calculate_ultimate_size()[1]
-        self.anim_interval_msgbox.pos[1] = \
-            self.msgbox.calculate_ultimate_size()[1] +\
-            self.loop_count_msgbox.calculate_ultimate_size()[1]
-        self.anim_frame_id_msgbox.pos[1] = \
-            self.msgbox.calculate_ultimate_size()[1] +\
-            self.loop_count_msgbox.calculate_ultimate_size()[1] +\
-            self.anim_interval_msgbox.calculate_ultimate_size()[1]
-        self.is_playing_msgbox.pos[1] = \
-            self.msgbox.calculate_ultimate_size()[1] +\
-            self.loop_count_msgbox.calculate_ultimate_size()[1] +\
-            self.anim_interval_msgbox.calculate_ultimate_size()[1] +\
-            self.is_playing_msgbox.calculate_ultimate_size()[1]
-        self.loop_counter_msgbox.pos[1] = \
-            self.msgbox.calculate_ultimate_size()[1] +\
-            self.loop_count_msgbox.calculate_ultimate_size()[1] +\
-            self.anim_interval_msgbox.calculate_ultimate_size()[1] +\
-            self.is_playing_msgbox.calculate_ultimate_size()[1] +\
-            self.is_playing_msgbox.calculate_ultimate_size()[1]
+        )
+        self.msgbox4.text = f"anim_frame_id:{self.test_anim_img.anim_frame_id}"
+        self.msgbox5.text = f"is_playing:{self.test_anim_img.is_playing}"
+        self.msgbox6.text = f"loop_counter:{self.test_anim_img.loop_counter}"
+        self.msgbox7.text = f"elapsed time:{self.stopwatch.read()/1000}"
+        self.msgbox8.text = f"pausing time:{self.stopwatch.read_pausing()/1000}"
+        self.msgbox2.pos[1] = self.msgbox.real_size[1]
+        self.msgbox3.pos[1] = self.msgbox.real_size[1] + self.msgbox2.real_size[1]
+        self.msgbox4.pos[1] = (
+            self.msgbox.real_size[1]
+            + self.msgbox2.real_size[1]
+            + self.msgbox3.real_size[1]
+        )
+        self.msgbox5.pos[1] = (
+            self.msgbox.real_size[1]
+            + self.msgbox2.real_size[1]
+            + self.msgbox3.real_size[1]
+            + self.msgbox4.real_size[1]
+        )
+        self.msgbox6.pos[1] = (
+            self.msgbox.real_size[1]
+            + self.msgbox2.real_size[1]
+            + self.msgbox3.real_size[1]
+            + self.msgbox4.real_size[1]
+            + self.msgbox5.real_size[1]
+        )
+        self.msgbox7.pos[1] = (
+            self.msgbox.real_size[1]
+            + self.msgbox2.real_size[1]
+            + self.msgbox3.real_size[1]
+            + self.msgbox4.real_size[1]
+            + self.msgbox5.real_size[1]
+            + self.msgbox6.real_size[1]
+        )
+        self.msgbox8.pos[1] = (
+            self.msgbox.real_size[1]
+            + self.msgbox2.real_size[1]
+            + self.msgbox3.real_size[1]
+            + self.msgbox4.real_size[1]
+            + self.msgbox5.real_size[1]
+            + self.msgbox6.real_size[1]
+            + self.msgbox7.real_size[1]
+        )
 
     def draw(self, screen):
-        draw_grid_background(screen, 16, (78, 78, 78))
-        # self.test_anim_img.draw(screen)
+        draw_grid(screen, 16, (78, 78, 78))
         screen.blit(
             self.test_anim_img.image,
-            (global_.w_size[0]//2-self.test_anim_img.image.get_width()//2,
-             self.menuui.pos[1]-self.test_anim_img.image.get_height()))
+            (
+                global_.w_size[0] // 2 - self.test_anim_img.image.get_width() // 2,
+                self.menuui.pos[1] - self.test_anim_img.image.get_height(),
+            ),
+        )
         self.menuui.draw(screen)
         self.msgbox.draw(screen)
-        self.loop_count_msgbox.draw(screen)
-        self.anim_interval_msgbox.draw(screen)
-        self.anim_frame_id_msgbox.draw(screen)
-        self.is_playing_msgbox.draw(screen)
-        self.loop_counter_msgbox.draw(screen)
+        self.msgbox2.draw(screen)
+        self.msgbox3.draw(screen)
+        self.msgbox4.draw(screen)
+        self.msgbox5.draw(screen)
+        self.msgbox6.draw(screen)
+        self.msgbox7.draw(screen)
+        self.msgbox8.draw(screen)
 
 
 scene_manager = SceneManager()
-scene_manager.push(GameMenuDebugScene(scene_manager))
+scene_manager.push(DebugScene(scene_manager))
 
 if __name__ == "__main__":
-    engine.run(scene_manager=scene_manager, fps_num=60)
+    engine.run(scene_manager=scene_manager, fps=60)
```

### Comparing `auraboros-0.9.0a0/src/debugs/assets/fonts/misaki_gothic.ttf` & `auraboros-1.0.0a0/src/auraboros/examples/assets/fonts/misaki_gothic.ttf`

 * *Files identical despite different names*

### Comparing `auraboros-0.9.0a0/.gitignore` & `auraboros-1.0.0a0/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,25 @@
 # File created using '.gitignore Generator' for Visual Studio Code: https://bit.ly/vscode-gig
-# Created by https://www.toptal.com/developers/gitignore/api/windows,visualstudiocode,python
-# Edit at https://www.toptal.com/developers/gitignore?templates=windows,visualstudiocode,python
+# Created by https://www.toptal.com/developers/gitignore/api/windows,visualstudiocode,python,git
+# Edit at https://www.toptal.com/developers/gitignore?templates=windows,visualstudiocode,python,git
+
+### Git ###
+# Created by git for backups. To disable backups in Git:
+# $ git config --global mergetool.keepBackup false
+*.orig
+
+# Created by git when using merge tools for conflicts
+*.BACKUP.*
+*.BASE.*
+*.LOCAL.*
+*.REMOTE.*
+*_BACKUP_*.txt
+*_BASE_*.txt
+*_LOCAL_*.txt
+*_REMOTE_*.txt
 
 ### Python ###
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
@@ -160,14 +175,24 @@
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
+### Python Patch ###
+# Poetry local configuration file - https://python-poetry.org/docs/configuration/#local-configuration
+poetry.toml
+
+# ruff
+.ruff_cache/
+
+# LSP config files
+pyrightconfig.json
+
 ### VisualStudioCode ###
 .vscode/*
 !.vscode/settings.json
 !.vscode/tasks.json
 !.vscode/launch.json
 !.vscode/extensions.json
 !.vscode/*.code-snippets
@@ -205,12 +230,13 @@
 *.msix
 *.msm
 *.msp
 
 # Windows shortcuts
 *.lnk
 
-# End of https://www.toptal.com/developers/gitignore/api/windows,visualstudiocode,python
+# End of https://www.toptal.com/developers/gitignore/api/windows,visualstudiocode,python,git
 
 # Custom rules (everything added below won't be overriden by 'Generate .gitignore File' if you use 'Update' option)
 
 beginning_of_history_cover.wav
+sandbox.py
```

### Comparing `auraboros-0.9.0a0/LICENSE` & `auraboros-1.0.0a0/LICENSE`

 * *Files identical despite different names*

