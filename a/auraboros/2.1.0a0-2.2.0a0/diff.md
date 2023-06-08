# Comparing `tmp/auraboros-2.1.0a0.tar.gz` & `tmp/auraboros-2.2.0a0.tar.gz`

## Comparing `auraboros-2.1.0a0.tar` & `auraboros-2.2.0a0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/Pipfile
--rw-r--r--   0        0        0    82156 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/Pipfile.lock
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/README.jp.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/README.md
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/mkdocs.yml
--rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/.vscode/launch.json
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/.vscode/settings.json
--rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/fonts/misaki_gothic.ttf
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/enemy_a.piskel
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/enemy_a.png
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/enemy_b.piskel
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/enemy_b.png
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/explosion_a.piskel
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/explosion_a.png
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/explosion_b.png
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/fighter_a.piskel
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/fighter_a.png
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/icon.ico
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/laser1.png
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/scoutdisk.piskel
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/scoutdisk.png
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot1.piskel
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot1.png
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot2.piskel
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot2.png
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot3.png
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot4.png
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot5.piskel
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot5.png
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot6.piskel
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot6.png
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot7.png
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/shot8.png
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/imgs/terrain_rock.png
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/level_data/debug1/level.json
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/level_data/debug1/patterns.json
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/level_data/stage1/level.json
--rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/level_data/stage1/patterns.json
--rw-r--r--   0        0        0    78688 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/sounds/deathse2.wav
--rw-r--r--   0        0        0   191648 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/sounds/deathse3.wav
--rw-r--r--   0        0        0    28264 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/sounds/deathse4.wav
--rw-r--r--   0        0        0    21586 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/sounds/explosion1.wav
--rw-r--r--   0        0        0   352960 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/sounds/explosion2.wav
--rw-r--r--   0        0        0   150572 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/sounds/laser.wav
--rw-r--r--   0        0        0   150610 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/sounds/laser2.wav
--rw-r--r--   0        0        0    21360 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/sounds/shot1.wav
--rw-r--r--   0        0        0  5177872 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/sounds/music/bgm1.wav
--rw-r--r--   0        0        0   789664 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/assets/sounds/music/gameover.wav
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/__init__.py
--rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/__main__.py
--rw-r--r--   0        0        0    11150 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/animation.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/core.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/default.frag
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/default.vert
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/designpattern.py
--rw-r--r--   0        0        0     2351 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/engine.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/gamecamera.py
--rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/gameinput.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/gamescene.py
--rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/gametext.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/getasset_order.json
--rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/particle.py
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/schedule.py
--rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/shader.py
--rw-r--r--   0        0        0    36537 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/ui.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/__pyinstaller/hook-auraboros.py
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/__pyinstaller/test_auraboros_packaging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/ecs/__init__.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/ecs/common.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/ecs/world.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/__init__.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/helloworld.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/setup_syspath.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/shooting_game.py
--rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/ui_showcase.py
--rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/misaki_gothic.ttf
--rw-r--r--   0        0        0  1133216 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/PixelMplus10-Regular.ttf
--rw-r--r--   0        0        0  1274396 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/PixelMplus12-Regular.ttf
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/README.txt
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/LICENSE_E
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/LICENSE_J
--rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/README_E
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/README_J
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/assets/imgs/testsprite.png
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/animate_msgbox.py
--rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/animation.py
--rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/animationimage.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/entity.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/gametext.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/helloworld.py
--rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/keyboard.py
--rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/keyframe_animation.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/menu_ui.py
--rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/mouse.py
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/msgbox.py
--rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/particle.py
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/scene_transition.py
--rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/schedule.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/shader.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/stopwatch.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/textinput.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/ui_example1.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/examples/deprecated/vignette.frag
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/utils/__init__.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/utils/coordinate.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/utils/misc.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/utils/path.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/utils/sequence.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/utils/string.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/src/auraboros/utils/surface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/__init__.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_animation.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_ecs.py
--rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_gameinput.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_gametext.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_particle.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_shader.py
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_ui.py
--rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/assets/fonts/misaki_gothic.ttf
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/assets/imgs/testsprite.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_utils/__init__.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_utils/test_path.py
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_utils/test_sequence.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/tests/test_utils/test_string.py
--rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/LICENSE
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/pyproject.toml
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 auraboros-2.1.0a0/PKG-INFO
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/Pipfile
+-rw-r--r--   0        0        0    82156 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/Pipfile.lock
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/README.jp.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/README.md
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/mkdocs.yml
+-rw-r--r--   0        0        0      934 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/.vscode/launch.json
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/.vscode/settings.json
+-rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/fonts/misaki_gothic.ttf
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/enemy_a.piskel
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/enemy_a.png
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/enemy_b.piskel
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/enemy_b.png
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/explosion_a.piskel
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/explosion_a.png
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/explosion_b.png
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/fighter_a.piskel
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/fighter_a.png
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/icon.ico
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/laser1.png
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/scoutdisk.piskel
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/scoutdisk.png
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot1.piskel
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot1.png
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot2.piskel
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot2.png
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot3.png
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot4.png
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot5.piskel
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot5.png
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot6.piskel
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot6.png
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot7.png
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/shot8.png
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/imgs/terrain_rock.png
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/level_data/debug1/level.json
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/level_data/debug1/patterns.json
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/level_data/stage1/level.json
+-rw-r--r--   0        0        0     3498 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/level_data/stage1/patterns.json
+-rw-r--r--   0        0        0    78688 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/sounds/deathse2.wav
+-rw-r--r--   0        0        0   191648 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/sounds/deathse3.wav
+-rw-r--r--   0        0        0    28264 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/sounds/deathse4.wav
+-rw-r--r--   0        0        0    21586 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/sounds/explosion1.wav
+-rw-r--r--   0        0        0   352960 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/sounds/explosion2.wav
+-rw-r--r--   0        0        0   150572 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/sounds/laser.wav
+-rw-r--r--   0        0        0   150610 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/sounds/laser2.wav
+-rw-r--r--   0        0        0    21360 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/sounds/shot1.wav
+-rw-r--r--   0        0        0  5177872 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/sounds/music/bgm1.wav
+-rw-r--r--   0        0        0   789664 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/assets/sounds/music/gameover.wav
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/__init__.py
+-rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/__main__.py
+-rw-r--r--   0        0        0    11150 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/animation.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/core.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/default.frag
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/default.vert
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/designpattern.py
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/engine.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/gamecamera.py
+-rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/gameinput.py
+-rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/gamescene.py
+-rw-r--r--   0        0        0    11687 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/gametext.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/getasset_order.json
+-rw-r--r--   0        0        0     4470 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/particle.py
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/schedule.py
+-rw-r--r--   0        0        0     4863 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/shader.py
+-rw-r--r--   0        0        0    36537 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/ui.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/__pyinstaller/hook-auraboros.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/__pyinstaller/test_auraboros_packaging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/ecs/__init__.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/ecs/common.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/ecs/world.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/__init__.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/helloworld.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/setup_syspath.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/shooting_game.py
+-rw-r--r--   0        0        0    10926 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/ui_showcase.py
+-rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/misaki_gothic.ttf
+-rw-r--r--   0        0        0  1133216 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/PixelMplus10-Regular.ttf
+-rw-r--r--   0        0        0  1274396 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/PixelMplus12-Regular.ttf
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/README.txt
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/LICENSE_E
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/LICENSE_J
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/README_E
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/README_J
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/assets/imgs/testsprite.png
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/animate_msgbox.py
+-rw-r--r--   0        0        0     6944 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/animation.py
+-rw-r--r--   0        0        0     7245 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/animationimage.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/entity.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/gametext.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/helloworld.py
+-rw-r--r--   0        0        0     6466 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/keyboard.py
+-rw-r--r--   0        0        0     7269 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/keyframe_animation.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/menu_ui.py
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/mouse.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/msgbox.py
+-rw-r--r--   0        0        0     4226 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/particle.py
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/scene_transition.py
+-rw-r--r--   0        0        0     6491 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/schedule.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/shader.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/stopwatch.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/textinput.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/ui_example1.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/examples/deprecated/vignette.frag
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/utils/__init__.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/utils/coordinate.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/utils/misc.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/utils/path.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/utils/sequence.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/utils/string.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/src/auraboros/utils/surface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/__init__.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_animation.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_ecs.py
+-rw-r--r--   0        0        0     2959 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_gameinput.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_gametext.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_particle.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_shader.py
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_ui.py
+-rw-r--r--   0        0        0  1171204 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/assets/fonts/misaki_gothic.ttf
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/assets/imgs/testsprite.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_utils/test_path.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_utils/test_sequence.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/tests/test_utils/test_string.py
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/LICENSE
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/pyproject.toml
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 auraboros-2.2.0a0/PKG-INFO
```

### Comparing `auraboros-2.1.0a0/Pipfile.lock` & `auraboros-2.2.0a0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/README.jp.md` & `auraboros-2.2.0a0/README.jp.md`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/README.md` & `auraboros-2.2.0a0/README.md`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/.github/workflows/test.yml` & `auraboros-2.2.0a0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/.vscode/launch.json` & `auraboros-2.2.0a0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/fonts/misaki_gothic.ttf` & `auraboros-2.2.0a0/assets/fonts/misaki_gothic.ttf`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/enemy_a.piskel` & `auraboros-2.2.0a0/assets/imgs/enemy_a.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/enemy_a.png` & `auraboros-2.2.0a0/assets/imgs/enemy_a.png`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/enemy_b.piskel` & `auraboros-2.2.0a0/assets/imgs/enemy_b.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/enemy_b.png` & `auraboros-2.2.0a0/assets/imgs/enemy_b.png`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/explosion_a.piskel` & `auraboros-2.2.0a0/assets/imgs/explosion_a.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/explosion_a.png` & `auraboros-2.2.0a0/assets/imgs/explosion_a.png`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/explosion_b.png` & `auraboros-2.2.0a0/assets/imgs/explosion_b.png`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/fighter_a.piskel` & `auraboros-2.2.0a0/assets/imgs/fighter_a.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/fighter_a.png` & `auraboros-2.2.0a0/assets/imgs/fighter_a.png`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/icon.ico` & `auraboros-2.2.0a0/assets/imgs/icon.ico`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/scoutdisk.piskel` & `auraboros-2.2.0a0/assets/imgs/scoutdisk.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/scoutdisk.png` & `auraboros-2.2.0a0/assets/imgs/scoutdisk.png`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/shot6.piskel` & `auraboros-2.2.0a0/assets/imgs/shot6.piskel`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/imgs/terrain_rock.png` & `auraboros-2.2.0a0/assets/imgs/terrain_rock.png`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/level_data/debug1/patterns.json` & `auraboros-2.2.0a0/assets/level_data/debug1/patterns.json`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/level_data/stage1/patterns.json` & `auraboros-2.2.0a0/assets/level_data/stage1/patterns.json`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/sounds/deathse2.wav` & `auraboros-2.2.0a0/assets/sounds/deathse2.wav`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/sounds/deathse3.wav` & `auraboros-2.2.0a0/assets/sounds/deathse3.wav`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/sounds/deathse4.wav` & `auraboros-2.2.0a0/assets/sounds/deathse4.wav`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/sounds/explosion1.wav` & `auraboros-2.2.0a0/assets/sounds/explosion1.wav`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/sounds/explosion2.wav` & `auraboros-2.2.0a0/assets/sounds/explosion2.wav`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/sounds/laser.wav` & `auraboros-2.2.0a0/assets/sounds/laser.wav`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/sounds/laser2.wav` & `auraboros-2.2.0a0/assets/sounds/laser2.wav`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/sounds/shot1.wav` & `auraboros-2.2.0a0/assets/sounds/shot1.wav`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/sounds/music/bgm1.wav` & `auraboros-2.2.0a0/assets/sounds/music/bgm1.wav`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/assets/sounds/music/gameover.wav` & `auraboros-2.2.0a0/assets/sounds/music/gameover.wav`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/__main__.py` & `auraboros-2.2.0a0/src/auraboros/__main__.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/animation.py` & `auraboros-2.2.0a0/src/auraboros/animation.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/core.py` & `auraboros-2.2.0a0/src/auraboros/core.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/engine.py` & `auraboros-2.2.0a0/src/auraboros/engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,26 @@
 
 DeltaTime = float
 PygameEvent = pygame.event.Event
 
 
 def run(
     scene_manager: SceneManager,
-    mod_for_mainloop: Callable[[DeltaTime]] = None,
-    mod_for_eventloop: Callable[[PygameEvent]] = None,
+    mod_for_mainloop: Callable = None,
+    mod_for_eventloop: Callable = None,
 ):
-    """_summary_
-
+    """
     Args:
         scene_manager (SceneManager): _description_
-        mod_for_mainloop (Callable[[DeltaTime]], optional):
+        mod_for_mainloop (Callable, optional):
             Append and do given func for mainloop.
             this is useful to provide the engine mainloop section for thirdparty
             pygame package.
-        mod_for_eventloop (Callable[[PygameEvent]], optional):
-            Append and do given func for mainloop.
+        mod_for_eventloop (Callable, optional):
+            Append and do given func for eventloop.
             this is useful to provide the engine eventloop section for thirdparty
             pygame package.
     """
     clock = pygame.time.Clock()
 
     if Global.use_opengl_display:
         shader2d = Shader2D()
```

### Comparing `auraboros-2.1.0a0/src/auraboros/gamecamera.py` & `auraboros-2.2.0a0/src/auraboros/gamecamera.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/gameinput.py` & `auraboros-2.2.0a0/src/auraboros/gameinput.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/gamescene.py` & `auraboros-2.2.0a0/src/auraboros/gamescene.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/gametext.py` & `auraboros-2.2.0a0/src/auraboros/gametext.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/getasset_order.json` & `auraboros-2.2.0a0/src/auraboros/getasset_order.json`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/particle.py` & `auraboros-2.2.0a0/src/auraboros/particle.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/schedule.py` & `auraboros-2.2.0a0/src/auraboros/schedule.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/shader.py` & `auraboros-2.2.0a0/src/auraboros/shader.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/ui.py` & `auraboros-2.2.0a0/src/auraboros/ui.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/__pyinstaller/test_auraboros_packaging.py` & `auraboros-2.2.0a0/src/auraboros/__pyinstaller/test_auraboros_packaging.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/ecs/common.py` & `auraboros-2.2.0a0/src/auraboros/ecs/common.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/ecs/world.py` & `auraboros-2.2.0a0/src/auraboros/ecs/world.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/helloworld.py` & `auraboros-2.2.0a0/src/auraboros/examples/helloworld.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/shooting_game.py` & `auraboros-2.2.0a0/src/auraboros/examples/shooting_game.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/ui_showcase.py` & `auraboros-2.2.0a0/src/auraboros/examples/ui_showcase.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/misaki_gothic.ttf` & `auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/misaki_gothic.ttf`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/PixelMplus10-Regular.ttf` & `auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/PixelMplus10-Regular.ttf`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/PixelMplus12-Regular.ttf` & `auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/PixelMplus12-Regular.ttf`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/README.txt` & `auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/README.txt`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/README_E` & `auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/README_E`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/README_J` & `auraboros-2.2.0a0/src/auraboros/examples/assets/fonts/PixelMplus/mplus_bitmap_fonts/README_J`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/animate_msgbox.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/animate_msgbox.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/animation.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/animation.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/animationimage.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/animationimage.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/entity.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/entity.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/gametext.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/gametext.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/keyboard.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/keyboard.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/keyframe_animation.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/keyframe_animation.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/menu_ui.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/menu_ui.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/mouse.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/mouse.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/msgbox.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/msgbox.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/particle.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/particle.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/scene_transition.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/scene_transition.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/schedule.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/schedule.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/shader.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/shader.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/stopwatch.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/stopwatch.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/textinput.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/textinput.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/examples/deprecated/ui_example1.py` & `auraboros-2.2.0a0/src/auraboros/examples/deprecated/ui_example1.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/utils/coordinate.py` & `auraboros-2.2.0a0/src/auraboros/utils/coordinate.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/utils/misc.py` & `auraboros-2.2.0a0/src/auraboros/utils/misc.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/utils/path.py` & `auraboros-2.2.0a0/src/auraboros/utils/path.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/utils/sequence.py` & `auraboros-2.2.0a0/src/auraboros/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/utils/string.py` & `auraboros-2.2.0a0/src/auraboros/utils/string.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/src/auraboros/utils/surface.py` & `auraboros-2.2.0a0/src/auraboros/utils/surface.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/tests/test_animation.py` & `auraboros-2.2.0a0/tests/test_animation.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/tests/test_ecs.py` & `auraboros-2.2.0a0/tests/test_ecs.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/tests/test_gameinput.py` & `auraboros-2.2.0a0/tests/test_gameinput.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/tests/test_gametext.py` & `auraboros-2.2.0a0/tests/test_gametext.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/tests/test_particle.py` & `auraboros-2.2.0a0/tests/test_particle.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/tests/test_ui.py` & `auraboros-2.2.0a0/tests/test_ui.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/tests/assets/fonts/misaki_gothic.ttf` & `auraboros-2.2.0a0/tests/assets/fonts/misaki_gothic.ttf`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/tests/test_utils/test_sequence.py` & `auraboros-2.2.0a0/tests/test_utils/test_sequence.py`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/.gitignore` & `auraboros-2.2.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `auraboros-2.1.0a0/LICENSE` & `auraboros-2.2.0a0/LICENSE`

 * *Files identical despite different names*

