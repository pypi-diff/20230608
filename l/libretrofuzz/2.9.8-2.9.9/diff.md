# Comparing `tmp/libretrofuzz-2.9.8.tar.gz` & `tmp/libretrofuzz-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.9.8.tar", max compression
+gzip compressed data, was "libretrofuzz-2.9.9.tar", max compression
```

## Comparing `libretrofuzz-2.9.8.tar` & `libretrofuzz-2.9.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-08 01:21:18.143519 libretrofuzz-2.9.8/LICENSE
--rw-r--r--   0        0        0     7900 2023-06-08 01:21:18.143519 libretrofuzz-2.9.8/README.rst
--rw-r--r--   0        0        0       22 2023-06-08 01:21:18.143519 libretrofuzz-2.9.8/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    55172 2023-06-08 01:21:18.143519 libretrofuzz-2.9.8/libretrofuzz/__main__.py
--rw-r--r--   0        0        0     1275 2023-06-08 01:21:18.143519 libretrofuzz-2.9.8/pyproject.toml
--rw-r--r--   0        0        0     9078 2023-06-08 01:21:31.189565 libretrofuzz-2.9.8/setup.py
--rw-r--r--   0        0        0     9088 2023-06-08 01:21:31.190640 libretrofuzz-2.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-08 04:40:54.925718 libretrofuzz-2.9.9/LICENSE
+-rw-r--r--   0        0        0     7900 2023-06-08 04:40:54.925718 libretrofuzz-2.9.9/README.rst
+-rw-r--r--   0        0        0       22 2023-06-08 04:40:54.925718 libretrofuzz-2.9.9/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    55098 2023-06-08 04:40:54.925718 libretrofuzz-2.9.9/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0     1275 2023-06-08 04:40:54.925718 libretrofuzz-2.9.9/pyproject.toml
+-rw-r--r--   0        0        0     9078 2023-06-08 04:41:07.833858 libretrofuzz-2.9.9/setup.py
+-rw-r--r--   0        0        0     9088 2023-06-08 04:41:07.835004 libretrofuzz-2.9.9/PKG-INFO
```

### Comparing `libretrofuzz-2.9.8/LICENSE` & `libretrofuzz-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.8/README.rst` & `libretrofuzz-2.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.8/libretrofuzz/__main__.py` & `libretrofuzz-2.9.9/libretrofuzz/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,16 +310,17 @@
 
     def __call__(self, s1, s2, processor=None, score_cutoff=None):
         if (min(len(s1), len(s2)) / max(len(s1), len(s2))) < 0.2:
             # ideally this branch wouldn't exist, but since many games do not have
             # images, they get caught up on a short title being completely contained in another
             # token_set_ratio gives that 100. Skip if the smaller name length is less than 20%
             return 0
-        # names are whitespace and case normalized
-        if s1 == s2:
+        # names are whitespace and case normalized, but they keep spaces
+        # for token_set_ratio. But still test this case.
+        if s1 == s2 or "".join(s1.split()) == "".join(s2.split()):
             return MAX_SCORE
         prefix = len(os.path.commonprefix([s1, s2]))
         # score_cutoff needs to be 0 from a combination of 3 factors that create a bug:
         # 1. the caller of this, extract passes the 'current best score' as score_cutoff
         # 2. the token_set_ratio function returns 0 if the calculated score < score_cutoff
         # 3. 'current best score' includes the prefix, which this call can't include in 2.
         similarity = fuzz.token_set_ratio(s1, s2, processor=None, score_cutoff=0)
@@ -328,26 +329,26 @@
         # is prone because it sets score to 100 if one string words are completely on the other.
         return min(MAX_SCORE - 1, similarity + prefix)
 
 
 # -----------------------------------------------------------------------------------------------------------------------------
 # Normalization functions, part of the functions that change both local labels and remote names to be more similar to compare
 # -----------------------------------------------------------------------------------------------------------------------------
-camelcase_pattern = regex.compile(r"(\p{Lu}\p{Ll}+)")
+camelcase_pattern = regex.compile(r"(\p{Lu}[\p{Ll},'“”\"]+)")
 # number sequences in the middle (not start or end) of a string that start with 0
 zero_lead_pattern = regex.compile(r"([^\d])0+([1-9])")
 
 
 def normalizer(t, nometa, hack):
     if nometa:
         t = removeparenthesis(t, "(", ")")
     if not hack:
         t = removeparenthesis(t, "[", "]")
     # change all common ascci symbol characters we aren't going to use after this (, and ')
-    t = replacemany(t, '_()[]{}-.!?#"', " ")
+    t = replacemany(t, '_()[]{}-.!?#"', "")
     # strips just because the user may have made a mistake naming the source
     # (or the replacement above introduce boundary spaces)
     t = t.strip()
     # remove any number leading 0, except at the end or the start of the string
     # where it is likely a important part of the name, not a file manager sort workaround
     t = regex.sub(zero_lead_pattern, r"\1\2", t)
     # CamelCaseNames for local labels are common when there are no spaces,
@@ -385,18 +386,18 @@
     t = removefirst(t, ", as")
     t = removeprefix(t, "as ")
     t = removefirst(t, ", o")
     t = removeprefix(t, "o ")
     t = removefirst(t, ", a")
     t = removeprefix(t, "a ")
     # remove the symbols used in the definite article normalization
-    t = replacemany(t, ",'", "")
+    t = replacemany(t, ",'“”\"", "")
     # this makes sure that if a remote name has ' and ' instead of ' _ ' to replace ' & ' it works
     #': ' doesn't need this because ':' is a forbidden character and both '_' and '-' turn to ''
-    t = t.replace(" and ", "")
+    t = t.replace(" and ", " ")
     # Tries to make roman numerals in the range 1-20 equivalent to normal numbers.
     # If both sides are roman numerals there is no harm done if XXIV gets turned into 204 in both sides.
     t = t.replace("xviii", "18")
     t = t.replace("xvii", "17")
     t = t.replace("xvi", "16")
     t = t.replace("xiii", "13")
     t = t.replace("xii", "12")
@@ -1001,15 +1002,15 @@
         # it's a improvement because sometimes server thumbnail types have case letter typos
         result = process.extract(
             nameaux, remote_names, scorer=title_scorer, processor=None, limit=verbose or 2, score_cutoff=None
         )
         _, max_score, _ = (result and result[0]) or (None, -1, None)
         winners = [x for x in result if x[1] == max_score and x[1] >= score]
         show = result if verbose else winners
-        name_format = style(name + ": ", bold=True)
+        name_format = style(nameaux + ": ", bold=True) if verbose else style(name + ": ", bold=True)
 
         if winners:
             allow = True
             # these parent directories were created when reading the playlist
             # more efficient than doing it a playlist game loop
             real_thumb_dir = Path(thumbnails_dir, destination)
             down_thumb_dir = Path(tmpdir, destination)
@@ -1091,18 +1092,14 @@
                         for old, new in downloaded_dict.values():
                             if new.exists():
                                 shutil.move(new, old)
 
                         name_format = name_format + ", ".join((strfy_runtime(x, urls) for x in show))
                         success_format = f'{style("Success",   fg=GREEN, bold=True)}: {name_format}'
                         echo(success_format)
-                    else:
-                        name_format = name_format + ", ".join((strfy_runtime(x) for x in show))
-                        missing_format = f'{style("Missing",   fg=RED,   bold=True)}: {name_format}'
-                        echo(missing_format)
                 except StopProgram as e:
                     name_format = name_format + ", ".join((strfy_runtime(x) for x in show))
                     skipped_format = f'{style("Skipped",     fg=(135,135,135), bold=True)}: {name_format}'
                     echo(skipped_format)
                     raise e
                 except StopDownload:
                     name_format = name_format + ", ".join((strfy_runtime(x) for x in show))
```

### Comparing `libretrofuzz-2.9.8/pyproject.toml` & `libretrofuzz-2.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.9.8"
+version = "2.9.9"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.9.8/setup.py` & `libretrofuzz-2.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.9.8',
+    'version': '2.9.9',
     'description': 'Fuzzy Retroarch thumbnail downloader',
     'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (require exact matches after the standard heuristics). If you still want more thumbnails, using ``libretro-fuzz --min 100 --delay 5 --delay 5`` works (lowering ``--min`` increases fuzz), with some delays introduced before and after downloading to check if you want to keep the game selected for the thumbnails.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n\n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n\n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--min`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--min`` less than 100 without ``--filter`` to a specific game, or at least ``--delay/--delay-after`` to be able to cancel.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n\n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n\n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n\n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n\n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n\n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--min 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show length N list: score, mininame, emoji hyperlinks.\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
```

### Comparing `libretrofuzz-2.9.8/PKG-INFO` & `libretrofuzz-2.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.9.8
+Version: 2.9.9
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

