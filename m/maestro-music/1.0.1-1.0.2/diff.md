# Comparing `tmp/maestro-music-1.0.1.tar.gz` & `tmp/maestro-music-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maestro-music-1.0.1.tar", last modified: Tue Mar 28 03:43:10 2023, max compression
+gzip compressed data, was "maestro-music-1.0.2.tar", last modified: Thu Jun  8 00:37:58 2023, max compression
```

## Comparing `maestro-music-1.0.1.tar` & `maestro-music-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-03-28 03:43:10.708698 maestro-music-1.0.1/
--rw-r--r--   0 sysadmin   (501) staff       (20)     1067 2023-03-25 20:23:16.000000 maestro-music-1.0.1/LICENSE
--rw-r--r--   0 sysadmin   (501) staff       (20)    11090 2023-03-28 03:43:10.708498 maestro-music-1.0.1/PKG-INFO
--rw-r--r--   0 sysadmin   (501) staff       (20)    37884 2023-03-28 02:35:39.000000 maestro-music-1.0.1/helpers.py
--rw-r--r--   0 sysadmin   (501) staff       (20)   146639 2023-03-25 20:23:16.000000 maestro-music-1.0.1/icon.py
--rw-r--r--   0 sysadmin   (501) staff       (20)     8837 2023-03-28 02:40:12.000000 maestro-music-1.0.1/mac_presence.py
--rw-r--r--   0 sysadmin   (501) staff       (20)   100445 2023-03-28 03:43:07.000000 maestro-music-1.0.1/maestro.py
-drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-03-28 03:43:10.707450 maestro-music-1.0.1/maestro_music.egg-info/
--rw-r--r--   0 sysadmin   (501) staff       (20)    11090 2023-03-28 03:43:10.000000 maestro-music-1.0.1/maestro_music.egg-info/PKG-INFO
--rw-r--r--   0 sysadmin   (501) staff       (20)      286 2023-03-28 03:43:10.000000 maestro-music-1.0.1/maestro_music.egg-info/SOURCES.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)        1 2023-03-28 03:43:10.000000 maestro-music-1.0.1/maestro_music.egg-info/dependency_links.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       41 2023-03-28 03:43:10.000000 maestro-music-1.0.1/maestro_music.egg-info/entry_points.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)      367 2023-03-28 03:43:10.000000 maestro-music-1.0.1/maestro_music.egg-info/requires.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       34 2023-03-28 03:43:10.000000 maestro-music-1.0.1/maestro_music.egg-info/top_level.txt
--rw-r--r--   0 sysadmin   (501) staff       (20)       38 2023-03-28 03:43:10.708760 maestro-music-1.0.1/setup.cfg
--rw-r--r--   0 sysadmin   (501) staff       (20)     1646 2023-03-28 02:25:36.000000 maestro-music-1.0.1/setup.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-08 00:37:58.164713 maestro-music-1.0.2/
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1067 2023-06-06 05:56:48.000000 maestro-music-1.0.2/LICENSE
+-rw-r--r--   0 sysadmin   (501) staff       (20)    10863 2023-06-08 00:37:58.164313 maestro-music-1.0.2/PKG-INFO
+-rw-r--r--   0 sysadmin   (501) staff       (20)    40364 2023-06-08 00:37:56.000000 maestro-music-1.0.2/helpers.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)   146639 2023-03-25 20:23:16.000000 maestro-music-1.0.2/icon.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)     8837 2023-05-06 22:47:50.000000 maestro-music-1.0.2/mac_presence.py
+-rw-r--r--   0 sysadmin   (501) staff       (20)   111741 2023-06-07 21:45:08.000000 maestro-music-1.0.2/maestro.py
+drwxr-xr-x   0 sysadmin   (501) staff       (20)        0 2023-06-08 00:37:58.163214 maestro-music-1.0.2/maestro_music.egg-info/
+-rw-r--r--   0 sysadmin   (501) staff       (20)    10863 2023-06-08 00:37:58.000000 maestro-music-1.0.2/maestro_music.egg-info/PKG-INFO
+-rw-r--r--   0 sysadmin   (501) staff       (20)      286 2023-06-08 00:37:58.000000 maestro-music-1.0.2/maestro_music.egg-info/SOURCES.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)        1 2023-06-08 00:37:58.000000 maestro-music-1.0.2/maestro_music.egg-info/dependency_links.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       40 2023-06-08 00:37:58.000000 maestro-music-1.0.2/maestro_music.egg-info/entry_points.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)      367 2023-06-08 00:37:58.000000 maestro-music-1.0.2/maestro_music.egg-info/requires.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       34 2023-06-08 00:37:58.000000 maestro-music-1.0.2/maestro_music.egg-info/top_level.txt
+-rw-r--r--   0 sysadmin   (501) staff       (20)       38 2023-06-08 00:37:58.164781 maestro-music-1.0.2/setup.cfg
+-rw-r--r--   0 sysadmin   (501) staff       (20)     1646 2023-06-06 01:02:22.000000 maestro-music-1.0.2/setup.py
```

### Comparing `maestro-music-1.0.1/LICENSE` & `maestro-music-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.1/PKG-INFO` & `maestro-music-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: maestro-music
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple command line tool to play songs (or any audio files, really).
 Home-page: https://github.com/PrajwalVandana/maestro-cli
 Author: Prajwal Vandana
 License: MIT
 Keywords: music,sound,audio,music-player,cli,ogg,flac,mp3,wav,spotify,youtube,audio-visualization,audio-visualizer
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # maestro
 `maestro` is a command-line tool to play songs (or any audio, really) in the terminal.
 
 ## Features
 
 - cross-platform!
 - add songs directly from YouTube, YouTube Music, or Spotify!
 - audio visualization directly in the terminal!
 - Discord integration!
 - [clips!](#maestro-clip)
-- shuffle! (along with precise control over the behavior of shuffling when looping)
+- shuffle! (along with precise control over the behavior of shuffling when repeating)
 - filter by [tags](#usage)!
 
 ## Installation
 
 Make sure you have Python 3 and `pip` installed.
 
 First, run
@@ -91,54 +90,57 @@
 ```
 pip install PATH_TO_DOWNLOADED_WIN64_WHEEL
 ```
 and *now* installing `maestro` should work. Another option (especially if you're on a 32-bit Windows) is to just get Visual C++ Build Tools.
 
 #### Linux
 
-If you have issues, try:
+If you have issues (especially if you get `Illegal instruction (core dumped)` when running `maestro play`, even after installing succesfully), try:
  * upgrading pip: `pip install --upgrade pip`
  * uninstalling `just_playback`: `pip uninstall just_playback`
  * reinstalling `just_playback` with the `--no-binary` flag: `pip install just_playback --no-binary just_playback --force-reinstall --upgrade`
 
-Check this out: [https://github.com/cheofusi/just_playback/issues/21](https://github.com/cheofusi/just_playback/issues/21) ... and good luck 💀.
+Also check this out: [https://github.com/cheofusi/just_playback/issues/21](https://github.com/cheofusi/just_playback/issues/21) ... and good luck 💀.
+
+
+#### If all else fails ...
+You could uninstall and reinstall.
+```pip uninstall maestro-music```
+and also remove the `~/.maestro-files` folder.
+
+WARNING: this will delete all your songs! You should probably back up your `~/.maestro-files/songs/` folder first.
 
 ## Platforms
 
 Tested heavily on macOS Monterey, barely at all on Windows and Linux. `maestro` was coded to be cross-platform, but if there are any problems, please open an issue (or PR if you know how to fix it!).
 
 Supports `.mp3`, `.wav`, `.flac`, and `.ogg` (Ogg Vorbis).
 
 ## Usage
 
 Run `maestro -h` to get a list of commands. Run `maestro <some command> -h` to get comprehensive help for that command—the below is just an overview.
 
 `maestro` uses the concept of a positive integer **song ID** to uniquely refer to each song.
 
-Also, playlists don't exist—`maestro` uses **tags**. For example, let's say you want to be able to listen to all your Jon Bellion songs together. Instead of adding them all to a playlist, run `maestro -t jon-bellion <song IDs for each Jon Bellion song>`. Then `maestro play jon-bellion`. If song `s` has tag `t`, then you can think of song `s` as belonging to the playlist defined by tag `t`.
+Also, playlists don't exist—`maestro` uses **tags**. For example, let's say you want to be able to listen to all your Jon Bellion songs together. Instead of adding them all to a playlist, run `maestro tag <song IDs for each Jon Bellion song> -t jon-bellion `. Then `maestro play jon-bellion`. If song `s` has tag `t`, then you can think of song `s` as belonging to the playlist defined by tag `t`.
 
-`maestro` also tracks your listen time—total and by year. You can see this with `maestro list` and/or `maestro entry`. For example, to see your top 10 listened songs (by number of times listened; note that this is NOT the number of times the song was played but rather the total listen time for that song divided by the duration), run `maestro list -s times_listened -T 10 -y cur`—replace 'cur' with e.g. '2020' to get the listen times for 2020 instead.
+`maestro` also tracks your listen time—total and by year. You can see this with `maestro list` and/or `maestro entry`. For example, to see your top 10 listened songs (by average number of times listened; note that this is NOT the number of times the song was played but rather the total listen time for that song divided by the duration), run `maestro list -s times_listened -T 10 -y cur`—replace 'cur' with e.g. '2020' to get the listen times for 2020 instead.
 
 ### `maestro add`
 
 Add a song (can be a folder of songs too!) given a file path.
 
 Pass the `-Y` or `--youtube` flag to download from a YouTube or YouTube Music URL instead of a file path. This requires installing [FFmpeg](https://github.com/FFmpeg/FFmpeg). Passing a YouTube Music **song** URL (not "Video") is recommended, as passing "Video"s (i.e. just normal YouTube videos) can sometimes mess up the artist/album data.
 
 Pass the `-S` or `--spotify` flag to download from a Spotify URL instead of a file path. This also requires installing FFmpeg.
 
 Pass the `-P` or `--playlist` flag to download an entire YT playlist from a song URL with a playlist component, e.g. https://www.youtube.com/watch?v=V1Z586zoeeE&list=PLfSdF_HSSu55q-5p-maISZyr19erpZsTo. The `-p` flag is unnecessary if the URL points directly to a playlist, e.g. https://www.youtube.com/playlist?list=PLfSdF_HSSu55q-5p-maISZyr19erpZsTo.
 
 By default, `maestro add` copies the file to its internal database (`~/.maestro-files`), but you can pass the `-M` or `--move` flag to move the file instead.
 
-### `maestro cache`
-Calculate (or recalculate with the `-F/--force` flag) visualization frequency data (see [`maestro play`](#maestro-play)) for songs passed by ID (or all songs with the `-A/--all` flag.
-
-If you ever go into the song database (located at `~/.maestro-files`) and manually edit a song, e.g. trimming (not recommended but should be fine as long as you don't mess with the name of the file), you should run `maestro cache --recache <SONG_ID>` to readjust the visualization.
-
 ### `maestro clip`
 
 Ever been listening to music, and you're skipping every song because you keep getting bored of them? You like the songs, you're just not in the mood to listen to all of them entirely.
 
 Introducing clips, something I've always wished the big companies like Spotify, YT Music would do. Use `maestro clip ID START END` to define a clip for any song with a start and end timestamp (or use the clip editor for fine-grained control with `maestro clip ID`), then `maestro play -c` to play in "clip mode" (can also be toggled while playing a normal mode session with the `c` key)—this will play the clips for each song (or the entire song if there's no clip). Now you can listen to only the best parts of your music!
 
 ### `maestro entry`
@@ -149,24 +151,23 @@
 
 List songs (or tags) and details. Use `maestro list -h` to see full options (e.g. sort, list only songs with a certain tag, etc.).
 
 ### `maestro play`
 
 Play songs. Use `maestro play -h` to see full options. Has lots of features:
 - pass tag(s) as arguments to play songs with any of those tag(s) (or songs with all of those tag(s) if you pass the `-M` or `--match-all` flag)
-- shuffle playlist with the `-s` or `--shuffle option (shuffle once, shuffle every loop, or shuffle every loop except the first)
+- shuffle playlist with the `-s` or `--shuffle option (shuffle once, shuffle everytime the playlist repeats, or shuffle everytime the playlist repeats except the first)
 - play songs in reverse order with the `-R` or `--reverse` flag
 - loop playlist with the `-L` or `--loop` flag
 - show an audio visualization with the `-V` or `--visualize` flag
-  - you may notice some wait time for the visualization to properly load the first time a song is visualized (~7 seconds), but after that the visualization is cached and should load quickly
 - works with headphone buttons (and the Touch Bar and Siri!) on Mac using the Now Playing Center!
 - works with Discord status! (pass the `-D` or `--discord` flag)
 
 While playing:
-- like a song and want to play *that specific song* on loop? click `l` while playing to toggle loop mode (not the same as passing `-L` to `maestro play`!)
+- like a song and want to play it on loop? click `l` while playing to replay it once, and click it one more time to replay it infinitely (click it a third time to stop replaying it)
 - seek with left/right arrow keys
 - volume up/down with `[` and `]`
 - remove selected song (not necessarily the currently playing song) from current playlist with `backspace/delete`
 - scroll with mouse or up/down arrow keys to scroll the selected song
 - `c` to toggle clip mode
 - `v` to toggle visualization mode
 - `d` to toggle Discord status
@@ -211,9 +212,7 @@
 ### `maestro untag`
 
 Remove tags from a song, e.g. `maestro untag -t harry-styles 87` (removes the tag 'harry-styles' from the song with ID 87).
 
 ## Thanks
 
 Big thanks to the creators of [just_playback](https://github.com/cheofusi/just_playback), no doubt the best Python module for playing sound!
-
-
```

### Comparing `maestro-music-1.0.1/helpers.py` & `maestro-music-1.0.2/helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,61 @@
 # region imports
 import curses
+import importlib
 import logging
 import multiprocessing
 import os
-import sys
 import threading
 import warnings
 
 logging.disable(logging.CRITICAL)
 
 import click
+import music_tag
 import numpy as np
 
 from datetime import date
 from shutil import copy, move
+from time import sleep
 
 from just_playback import Playback
 from numba import jit  # NOTE: I think I'm in love with this decorator
 from numba.core.errors import NumbaWarning
 
 warnings.simplefilter("ignore", category=NumbaWarning)
+
+try:
+    LIBROSA = importlib.import_module("librosa")
+    if not (
+        "load" in dir(LIBROSA)
+        and "amplitude_to_db" in dir(LIBROSA)
+        and "stft" in dir(LIBROSA)
+    ):
+        raise ImportError
+except ImportError:
+    LIBROSA = None
+
 # endregion
 
 # region constants
 
 DISCORD_ID = 1039038199881810040
 
 CUR_YEAR = date.today().year
 EXTS = (".mp3", ".wav", ".flac", ".ogg")
+PROMPT_MODES = {
+    "insert": 0,
+    "add": 1,
+    "tag": 2,
+}
+LOOP_MODES = {
+    "none": 0,
+    "one": 1,
+    "inf": 2,
+}
 
 METADATA_KEYS = (
     "album",
     "albumartist",
     "artist",
     "artwork",
     "comment",
@@ -60,17 +84,14 @@
 SONGS_DIR = os.path.join(MAESTRO_DIR, "songs/")
 
 SONGS_INFO_PATH = os.path.join(MAESTRO_DIR, "songs.txt")
 
 STATS_DIR = os.path.join(MAESTRO_DIR, "stats/")
 CUR_YEAR_STATS_PATH = os.path.join(STATS_DIR, f"{CUR_YEAR}.txt")
 TOTAL_STATS_PATH = os.path.join(STATS_DIR, "total.txt")
-
-FREQ_CACHE_DIR = os.path.join(MAESTRO_DIR, "cache/freqs/")
-DATA_CACHE_DIR = os.path.join(MAESTRO_DIR, "cache/data")
 # endregion
 
 # region player
 HORIZONTAL_BLOCKS = {
     1: "▏",
     2: "▎",
     3: "▍",
@@ -135,16 +156,17 @@
                 self.top -= 1
             self.pos -= 1
 
     @property
     def halfway(self):
         return self.top + self.win_size // 2
 
-    def resize(self, win_size):
-        self.win_size = win_size
+    def resize(self, win_size=None):
+        if win_size is not None:
+            self.win_size = win_size
         self.top = max(0, self.pos - self.win_size // 2)
         self.top = max(0, min(self.num_lines - self.win_size, self.top))
 
 
 def fit_string_to_width(string, width, length_so_far):
     if length_so_far + len(string) > width:
         remaining_width = width - length_so_far
@@ -184,15 +206,15 @@
             arr[:, -remainder:].reshape(arr.shape[0], -1, remainder), axis=1
         )
         return np.concatenate((avg_head, avg_tail), axis=1)
 
     return avg_head
 
 
-@jit
+# @jit
 def render(
     num_bins,
     freqs,
     t,
     visualizer_height,
     mono=None,
     include_remainder=None,
@@ -258,131 +280,104 @@
             for b in range(num_bins):
                 s += VERTICAL_BLOCKS[arr[1, h, b]]
         res.append(s)
 
     return res
 
 
-class AudioData:
-    def __init__(self, song_path=None, freqs=True, data=True):
-        if song_path is None:
-            self.data = self.freqs = None
-            self.loaded_song = ""
-            self.loading = False
-            return
-
-        try:
-            self.loading = True
-
-            if data:
-                self.load_data(song_path)
-
-            if freqs:
-                self.load_freqs(song_path)
-                self.freqs = (
-                    80 * (self.freqs / 80) ** VIS_FLATTEN_FACTOR
-                )  # flatten
-
-            self.loaded_song = song_path
-            self.loading = False
-        except:  # pylint: disable=bare-except
-            self.data = self.freqs = self.loaded_song = self.loading = None
-
-    def load_data(self, song_path):
-        data_cache_path = os.path.join(
-            DATA_CACHE_DIR,
-            os.path.splitext(os.path.basename(song_path))[0] + ".npy",
-        )
-
-        if not os.path.exists(data_cache_path):
-            from librosa import load
-
-            self.data = load(song_path, mono=False, sr=SAMPLE_RATE)[0]
-
-            if len(self.data.shape) == 1:  # mono -> stereo
-                self.data = np.repeat([self.data], 2, axis=0)
-            elif self.data.shape[0] == 1:  # mono -> stereo
-                self.data = np.repeat(self.data, 2, axis=0)
-            elif self.data.shape[0] == 6:  # 5.1 surround -> stereo
-                self.data = np.delete(self.data, (1, 3, 4, 5), axis=0)
-            np.save(data_cache_path, self.data)
-        else:
-            self.data = np.load(data_cache_path)
-
-    def load_freqs(self, song_path):
-        freq_cache_path = os.path.join(
-            FREQ_CACHE_DIR,
-            os.path.splitext(os.path.basename(song_path))[0] + ".npy",
-        )
-
-        if not os.path.exists(freq_cache_path):
-            from librosa import stft, amplitude_to_db
-
-            self.load_data(song_path)
-
-            self.freqs = (
-                amplitude_to_db(np.abs(stft(self.data)), ref=np.max) + 80
-            )  # [-80, 0] -> [0, 80]
-            np.save(freq_cache_path, self.freqs)
-        else:
-            self.freqs = np.load(freq_cache_path)
-
-
 class PlayerOutput:
     def __init__(
         self, stdscr, playlist, volume, clip_mode, update_discord, visualize
     ):
         self.stdscr = stdscr
         self.scroller = Scroller(
             len(playlist), stdscr.getmaxyx()[0] - 2  # -2 for status bar
         )
         self.playlist = playlist
+        self.i = 0
         self.volume = volume
         self.clip_mode = clip_mode
         self.update_discord = update_discord
-        self.can_visualize = self.visualize = visualize
+        self.visualize = visualize  # want to visualize
+        self.can_visualize = LIBROSA is not None  # can generate visualization
+        # space to show visualization
+        self.can_show_visualization = (
+            self.can_visualize
+            and self.stdscr.getmaxyx()[0] > VISUALIZER_HEIGHT + 5
+        )
+        if self.visualize and self.can_visualize:
+            t = threading.Thread(
+                target=self.load_visualizer_data,
+                daemon=True,
+            )
+            self.visualizer_data = {}
+            t.start()
 
-        self.i = 0
-        self.looping_current_song = False
+        self.looping_current_song = LOOP_MODES["none"]
         self.duration = 0
         self.paused = False
         self.ending = False
-        self.adding_song: None | tuple = None
+        self.prompting: None | tuple = None
         self.clip = (0, 0)
         self.discord_connected = multiprocessing.Value("i", 2)
-        self.visualizer_data = AudioData()
+
+    def load_visualizer_data(self):
+        while True:
+            cur_song_ids = set(
+                map(lambda x: x[0], self.playlist[self.i : self.i + 5])
+            )
+            keys_to_delete = []
+            for k in self.visualizer_data:
+                if k not in cur_song_ids:
+                    keys_to_delete.append(k)
+            for k in keys_to_delete:
+                del self.visualizer_data[k]
+
+            for i in range(self.i, self.i + 5):
+                if self.playlist[i][0] in self.visualizer_data:
+                    continue
+                song_path = os.path.join(SONGS_DIR, self.playlist[i][1])
+                cur_song_data = LIBROSA.load(
+                    song_path, mono=False, sr=SAMPLE_RATE
+                )[0]
+
+                if len(cur_song_data.shape) == 1:  # mono -> stereo
+                    cur_song_data = np.repeat([cur_song_data], 2, axis=0)
+                elif cur_song_data.shape[0] == 1:  # mono -> stereo
+                    cur_song_data = np.repeat(cur_song_data, 2, axis=0)
+                elif cur_song_data.shape[0] == 6:  # 5.1 surround -> stereo
+                    cur_song_data = np.delete(
+                        cur_song_data, (1, 3, 4, 5), axis=0
+                    )
+
+                self.visualizer_data[self.playlist[i][0]] = (
+                    LIBROSA.amplitude_to_db(
+                        np.abs(LIBROSA.stft(cur_song_data)), ref=np.max
+                    )
+                    + 80
+                )
+            sleep(1)
 
     @property
     def song_path(self):
         return os.path.join(SONGS_DIR, self.playlist[self.i][1])
 
     def output(self, pos):
-        self.can_visualize = (
-            self.visualize and self.stdscr.getmaxyx()[0] > VISUALIZER_HEIGHT + 3
+        self.can_show_visualization = (
+            self.visualize
+            and self.can_visualize
+            and self.stdscr.getmaxyx()[0] > VISUALIZER_HEIGHT + 5
         )
-
-        if self.can_visualize:
-            if self.visualizer_data.loaded_song != self.song_path:
-                if self.visualizer_data.loaded_song is None:
-                    self.can_visualize = False
-                elif not self.visualizer_data.loading:
-                    t = threading.Thread(
-                        target=lambda: self.visualizer_data.__init__(
-                            self.song_path
-                        ),
-                        daemon=True,
-                    )
-                    t.start()
-
         self.scroller.resize(
             self.stdscr.getmaxyx()[0]
             - 3  # -3 for status bar
             - 1  # -1 for header
-            - (self.adding_song != None)  # - add mode
-            - (VISUALIZER_HEIGHT if self.can_visualize else 0)  # - visualizer
+            - (self.prompting != None)  # - add mode
+            # - visualizer
+            - (VISUALIZER_HEIGHT if self.can_show_visualization else 0)
         )
 
         if self.clip_mode:
             pos -= self.clip[0]
 
         self.stdscr.erase()
 
@@ -414,23 +409,23 @@
                     length_so_far,
                     curses.color_pair(14),
                 )
 
         visualize_message = ""
         visualize_color = 12
         if self.visualize:
-            if self.can_visualize:
-                if self.visualizer_data.loading:
-                    visualize_message = "Loading visualization..."
-            else:
-                if self.stdscr.getmaxyx()[0] <= VISUALIZER_HEIGHT + 3:
-                    visualize_message = "Window too small for visualization."
-                else:
-                    visualize_message = "Failed to load visualization."
+            if not self.can_visualize:
+                visualize_message = "Librosa is required for visualization."
+                visualize_color = 14
+            elif not self.can_show_visualization:
+                visualize_message = "Window too small for visualization."
                 visualize_color = 14
+            elif self.playlist[self.i][0] not in self.visualizer_data:
+                visualize_message = "Loading visualization..."
+                visualize_color = 12
         length_so_far = addstr_fit_to_width(
             self.stdscr,
             " " * (screen_width - length_so_far - len(visualize_message))
             + visualize_message,
             screen_width,
             length_so_far,
             curses.color_pair(visualize_color),
@@ -484,25 +479,41 @@
                     f"{', '.join(self.playlist[j][2].split(','))}",
                     screen_width,
                     length_so_far,
                     curses.color_pair(2),
                 )
             self.stdscr.move((j - self.scroller.top) + 2, 0)
 
-        if self.adding_song is not None:
+        if self.prompting is not None:
             # pylint: disable=unsubscriptable-object
-            adding_song_length = addstr_fit_to_width(
-                self.stdscr,
-                ("Insert" if self.adding_song[2] else "Append")
-                + " song (by ID): "
-                + self.adding_song[0],
-                screen_width,
-                0,
-                curses.color_pair(1),
-            )
+            if (
+                self.prompting[2] == PROMPT_MODES["add"]
+                or self.prompting[2] == PROMPT_MODES["insert"]
+            ):
+                adding_song_length = addstr_fit_to_width(
+                    self.stdscr,
+                    (
+                        "Insert"
+                        if self.prompting[2] == PROMPT_MODES["insert"]
+                        else "Append"
+                    )
+                    + " song (by ID): "
+                    + self.prompting[0],
+                    screen_width,
+                    0,
+                    curses.color_pair(1),
+                )
+            else:
+                adding_song_length = addstr_fit_to_width(
+                    self.stdscr,
+                    "Add tag to songs: " + self.prompting[0],
+                    screen_width,
+                    0,
+                    curses.color_pair(1),
+                )
             self.stdscr.move(self.stdscr.getyx()[0] + 1, 0)
 
         length_so_far = 0
 
         length_so_far = addstr_fit_to_width(
             self.stdscr,
             ("| " if self.paused else "> ") + f"({self.playlist[self.i][0]}) ",
@@ -527,17 +538,23 @@
         length_so_far = addstr_fit_to_width(
             self.stdscr,
             f"{'c' if self.clip_mode else ' '}",
             screen_width,
             length_so_far,
             curses.color_pair(17) | curses.A_BOLD,
         )
+        loop_char = " "
+        if self.looping_current_song == LOOP_MODES["one"]:
+            loop_char = "l"
+        elif self.looping_current_song == LOOP_MODES["inf"]:
+            loop_char = "L"
+        # print_to_logfile(self.looping_current_song)
         length_so_far = addstr_fit_to_width(
             self.stdscr,
-            f"{'l' if self.looping_current_song else ' '}",
+            loop_char,
             screen_width,
             length_so_far,
             curses.color_pair(15) | curses.A_BOLD,
         )
         volume_line_length_so_far = addstr_fit_to_width(
             self.stdscr,
             f"{'e' if self.ending else ' '}  ",
@@ -555,15 +572,15 @@
         self.stdscr.insstr(  # hacky fix for curses bug
             " ",
             curses.color_pair(16),
         )
         self.stdscr.move(
             self.stdscr.getmaxyx()[0]
             - 2
-            - (VISUALIZER_HEIGHT if self.can_visualize else 0),
+            - (VISUALIZER_HEIGHT if self.can_show_visualization else 0),
             0,
         )
 
         addstr_fit_to_width(
             self.stdscr,
             " " * (screen_width - 1),
             screen_width,
@@ -583,27 +600,23 @@
             self.stdscr,
             self.playlist[self.i][-3] + " - ",
             screen_width,
             0,
             curses.color_pair(12),
         )
 
-        if (
-            curses.ncurses_version >= (6, 1)
-            and sys.version_info >= (3, 7)
-            and "A_ITALIC" in dir(curses)
-        ):
+        try:
             song_data_length_so_far = addstr_fit_to_width(
                 self.stdscr,
                 self.playlist[self.i][-2],
                 screen_width,
                 song_data_length_so_far,
                 curses.color_pair(12) | curses.A_ITALIC,
             )
-        else:
+        except:  # pylint: disable=bare-except
             song_data_length_so_far = addstr_fit_to_width(
                 self.stdscr,
                 self.playlist[self.i][-2],
                 screen_width,
                 song_data_length_so_far,
                 curses.color_pair(12),
             )
@@ -613,15 +626,17 @@
             f" ({self.playlist[self.i][-1]})",
             screen_width,
             song_data_length_so_far,
             curses.color_pair(12),
         )
 
         self.stdscr.move(
-            self.stdscr.getmaxyx()[0] - VISUALIZER_HEIGHT - 1,
+            self.stdscr.getmaxyx()[0]
+            - (VISUALIZER_HEIGHT if self.can_show_visualization else 0)
+            - 1,
             0,
         )
 
         length_so_far = 0
         secs = int(pos)
         length_so_far = addstr_fit_to_width(
             self.stdscr,
@@ -663,15 +678,15 @@
                 )
 
         # right align volume bar
         if not volume_line_length_so_far >= screen_width:
             self.stdscr.move(
                 self.stdscr.getmaxyx()[0]
                 - 3
-                - (VISUALIZER_HEIGHT if self.can_visualize else 0),
+                - (VISUALIZER_HEIGHT if self.can_show_visualization else 0),
                 volume_line_length_so_far,
             )
             if (
                 screen_width - volume_line_length_so_far
                 >= MIN_VOLUME_BAR_WIDTH + 10
             ):
                 bar = f"{str(int(self.volume*100)).rjust(3)}/100 |"
@@ -697,54 +712,54 @@
                 self.stdscr.addstr(
                     f"{str(int(self.volume*100)).rjust(3)}/100".rjust(
                         screen_width - volume_line_length_so_far
                     ),
                     curses.color_pair(16),
                 )
 
-        if self.can_visualize:
+        if self.can_show_visualization:
             if self.clip_mode:
                 pos += self.clip[0]
 
             self.stdscr.move(
                 self.stdscr.getmaxyx()[0]
-                - (VISUALIZER_HEIGHT if self.can_visualize else 0),
+                - (VISUALIZER_HEIGHT if self.can_show_visualization else 0),
                 0,
             )
-            if self.visualizer_data.loading in (True, None):
+            if self.playlist[self.i][0] not in self.visualizer_data:
                 self.stdscr.addstr(
                     (
                         (" " * (self.stdscr.getmaxyx()[1] - 1) + "\n")
                         * VISUALIZER_HEIGHT
                     ).rstrip()
                 )
             else:
                 rendered_lines = render(
                     self.stdscr.getmaxyx()[1],
-                    self.visualizer_data.freqs,
+                    self.visualizer_data[self.playlist[self.i][0]],
                     min(
                         round(pos * FPS),
-                        self.visualizer_data.freqs.shape[2] - 1,
+                        self.visualizer_data[self.playlist[self.i][0]].shape[2] - 1,
                     ),
                     VISUALIZER_HEIGHT,
                 )
                 for i in range(len(rendered_lines)):
                     self.stdscr.addstr(rendered_lines[i][:-1])
                     self.stdscr.insstr(rendered_lines[i][-1])
                     if i < len(rendered_lines) - 1:
                         self.stdscr.move(self.stdscr.getyx()[0] + 1, 0)
 
-        if self.adding_song is not None:
+        if self.prompting is not None:
             # pylint: disable=unsubscriptable-object
             self.stdscr.move(
                 self.stdscr.getmaxyx()[0]
-                - (VISUALIZER_HEIGHT if self.can_visualize else 0)
+                - (VISUALIZER_HEIGHT if self.can_show_visualization else 0)
                 - 4,  # 4 lines for status bar + adding entry
                 adding_song_length
-                + (self.adding_song[1] - len(self.adding_song[0])),
+                + (self.prompting[1] - len(self.prompting[0])),
             )
 
         self.stdscr.refresh()
 
 
 def init_curses(stdscr):
     curses.start_color()
@@ -766,28 +781,30 @@
     curses.init_pair(15, curses.COLOR_YELLOW, curses.COLOR_BLACK)
     curses.init_pair(16, curses.COLOR_GREEN, curses.COLOR_BLACK)
     curses.init_pair(17, curses.COLOR_MAGENTA, curses.COLOR_BLACK)
     # endregion
 
     curses.curs_set(False)
     stdscr.nodelay(True)
-    curses.set_escdelay(25)  # 25 ms
+    try:
+        curses.set_escdelay(25)  # 25 ms
+    except:  # pylint: disable=bare-except
+        pass
 
 
 def add_song(
     path,
     tags,
     move_,
     songs_file,
     lines,
     song_id,
     prepend_newline,
     clip_start,
     clip_end,
-    gen_vis_cache,
 ):
     song_name = os.path.split(path)[1]
     if "|" in song_name:
         song_name = song_name.replace("|", "-")
         click.secho(
             f"The song \"{song_name}\" contains one or more '|' character(s), which is not allowed—all ocurrences have been replaced with '-'.",
             fg="yellow",
@@ -839,63 +856,61 @@
         tags_string = f" and tags {', '.join([repr(tag) for tag in tags])}"
 
     if clip_start is not None:
         clip_string = f" and clip [{format_seconds(clip_start, show_decimal=True)}, {format_seconds(clip_end, show_decimal=True)}]"
     else:
         clip_string = ""
 
-    if gen_vis_cache:
-        data = AudioData(os.path.join(SONGS_DIR, song_name), data=False)
-        if data.loaded_song is None:
-            data = None
-    else:
-        data = None
-
+    song_metadata = music_tag.load_file(dest_path)
     click.secho(
-        f"Added{' and cached visualization frequencies for' if data is not None else ''} song '{song_name}' with ID {song_id}"
+        f"Added song '{song_name}' with ID {song_id}"
         + tags_string
         + clip_string
-        + ".",
+        + f" and metadata (artist: {song_metadata['artist'] if song_metadata['artist'] else '<None>'}, album: {song_metadata['album'] if song_metadata['album'] else '<None>'}, albumartist: {song_metadata['albumartist'] if song_metadata['albumartist'] else '<None>'}).",
         fg="green",
     )
 
 
 def clip_editor(stdscr, details):
     song_name = details[1]
     song_path = os.path.join(SONGS_DIR, song_name)
 
     show_waveform = True
-    audio_data = AudioData(song_path, freqs=False)
-    if audio_data.loaded_song is None:
+    if LIBROSA is None:
         show_waveform = False
+    else:
+        audio_data = LIBROSA.load(song_path, sr=SAMPLE_RATE)[0]
 
-    init_curses(stdscr)
+        if len(audio_data.shape) == 1:  # mono -> stereo
+            audio_data = np.repeat([audio_data], 2, axis=0)
+        elif audio_data.shape[0] == 1:  # mono -> stereo
+            audio_data = np.repeat(audio_data, 2, axis=0)
+        elif audio_data.shape[0] == 6:  # 5.1 surround -> stereo
+            audio_data = np.delete(audio_data, (1, 3, 4, 5), axis=0)
 
-    if show_waveform:
-        audio_data.data /= np.max(np.abs(audio_data.data))
-        audio_data.data = (
+        audio_data /= np.max(np.abs(audio_data))
+        audio_data = (
             80
-            * (
-                (np.reshape(audio_data.data, audio_data.data.shape + (1,)) + 1)
-                / 2
-            )
-            ** WAVEFORM_FLATTEN_FACTOR
+            * ((np.reshape(audio_data, audio_data.shape + (1,)) + 1) / 2) ** 80
         )
 
     playback = Playback()
     playback.load_file(song_path)
 
+    init_curses(stdscr)
+
     if details[3]:
         clip_start, clip_end = [float(x) for x in details[3].split()]
     else:
         clip_start, clip_end = 0, playback.duration
     editing_start = True
     change_output = True
     playback.play()
     playback.pause()
+    playback.seek(clip_start)
     last_timestamp = playback.curr_pos
     while True:
         if playback.curr_pos >= clip_end:
             playback.pause()
 
         change_output = change_output or (
             (playback.curr_pos - last_timestamp)
@@ -1032,15 +1047,15 @@
 
     show_waveform = (
         show_waveform and stdscr.getmaxyx()[0] >= 4 + WAVEFORM_HEIGHT
     )
     if show_waveform:
         rendered_lines = render(
             screen_width - 2,
-            audio_data.data,
+            audio_data,
             0,
             WAVEFORM_HEIGHT,
             mono=True,
             include_remainder=True,
             func=np.max,
         )
 
@@ -1148,31 +1163,52 @@
 def format_seconds(secs, show_decimal=False):
     """Format seconds into a string."""
     return f"{int(secs//60):02}:{int(secs%60):02}" + (
         f".{secs%1:0.2f}"[2:] if show_decimal else ""
     )
 
 
-def print_entry(entry_list):
+def print_entry(entry_list, highlight=None, show_song_info=None):
     """
     tuple or iterable of strings
 
     0: song ID
     1: song name
     2: tags
     3: clip
 
     optional:
     4: seconds listened
-    5: total duration (must be passed if 3 is passed)
+    5: total duration (must be passed if 4 is passed)
 
-    Pretty prints '<song ID> <song name> [<total duration> <seconds
-    listened> <times listened>] <clip> <tags>'"""
+    Pretty prints ([] means optional)
+        <song ID> <song name> [<total duration> <seconds listened> <times listened>] <clip> <tags>
+            [<artist> - <album> (<album artist>)]
+    """
     click.secho(entry_list[0] + " ", fg="bright_black", nl=False)
-    click.secho(entry_list[1] + " ", fg="blue", nl=False)
+    if highlight is None:
+        click.secho(entry_list[1] + " ", fg="blue", nl=False, bold=True)
+    else:
+        highlight_loc = entry_list[1].lower().find(highlight.lower())
+        click.secho(
+            entry_list[1][:highlight_loc],
+            fg="white",
+            nl=False,
+        )
+        click.secho(
+            entry_list[1][highlight_loc : highlight_loc + len(highlight)],
+            fg="blue",
+            nl=False,
+            bold=True,
+        )
+        click.secho(
+            entry_list[1][highlight_loc + len(highlight) :] + " ",
+            fg="white",
+            nl=False,
+        )
 
     if len(entry_list) > 4:  # len should == 6
         secs_listened = float(entry_list[4])
         total_duration = float(entry_list[5])
         click.secho(
             format_seconds(total_duration, show_decimal=True) + " ",
             nl=False,
@@ -1198,12 +1234,41 @@
         )
 
     if entry_list[2]:
         click.secho(", ".join(entry_list[2].split(",")), fg="bright_black")
     else:
         click.echo()  # newline
 
+    if show_song_info:
+        song_data = music_tag.load_file(os.path.join(SONGS_DIR, entry_list[1]))
+        artist, album, album_artist = (
+            song_data["artist"].value,
+            song_data["album"].value,
+            song_data["albumartist"].value,
+        )
+        click.secho(
+            f"{(len(entry_list[0])+1)*' '}{artist if artist else 'Unknown Artist'} - ",
+            fg="bright_black",
+            nl=False,
+        )
+        click.secho(
+            (album if album else "Unknown Album"),
+            italic=True,
+            fg="bright_black",
+            nl=False,
+        )
+        click.secho(
+            f" ({album_artist if album_artist else 'Unknown Album Artist'})",
+            fg="bright_black",
+        )
+
 
 def print_to_logfile(*args, **kwargs):
     if "file" in kwargs:
-        raise ValueError("file kwarg is not allowed for 'print_to_logfile'")
+        raise ValueError("file kwargs not allowed for 'print_to_logfile'")
     print(*args, **kwargs, file=open("log.txt", "a", encoding="utf-8"))
+
+
+def multiprocessing_put_word(q, word):
+    for c in word:
+        q.put(c)
+    q.put("\n")
```

### Comparing `maestro-music-1.0.1/icon.py` & `maestro-music-1.0.2/icon.py`

 * *Files identical despite different names*

### Comparing `maestro-music-1.0.1/mac_presence.py` & `maestro-music-1.0.2/mac_presence.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,22 +129,22 @@
 
         return 0
 
     def next_handler(self, _event):
         """
         Handle an external 'nextTrackCommand' event.
         """
-        self.q.put("s")
+        self.q.put("n")
         return 0
 
     def prev_handler(self, _event):
         """
         Handle an external 'previousTrackCommand' event.
         """
-        self.q.put("p")
+        self.q.put("b")
         return 0
 
     def seek_backward_handler(self, _event):
         """
         Handle an external 'seekBackwardCommand' event.
         """
         self.pos -= 10
```

### Comparing `maestro-music-1.0.1/maestro.py` & `maestro-music-1.0.2/maestro.py`

 * *Files 4% similar despite different names*

```diff
@@ -172,6107 +172,6813 @@
 00000ab0: 2073 6f6e 675f 6e61 6d65 5f71 7565 7565   song_name_queue
 00000ac0: 2e67 6574 2829 0a0a 2020 2020 2020 2020  .get()..        
 00000ad0: 2020 2020 6172 7469 7374 5f6e 616d 6520      artist_name 
 00000ae0: 3d20 2222 0a20 2020 2020 2020 2020 2020  = "".           
 00000af0: 2077 6869 6c65 206e 6f74 2061 7274 6973   while not artis
 00000b00: 745f 7175 6575 652e 656d 7074 7928 293a  t_queue.empty():
 00000b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b20: 2063 203d 2061 7274 6973 745f 7175 6575   c = artist_queu
-00000b30: 652e 6765 7428 290a 2020 2020 2020 2020  e.get().        
-00000b40: 2020 2020 2020 2020 7768 696c 6520 6320          while c 
-00000b50: 213d 2022 5c6e 223a 0a20 2020 2020 2020  != "\n":.       
-00000b60: 2020 2020 2020 2020 2020 2020 2061 7274               art
-00000b70: 6973 745f 6e61 6d65 202b 3d20 630a 2020  ist_name += c.  
-00000b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b90: 2020 6320 3d20 6172 7469 7374 5f71 7565    c = artist_que
-00000ba0: 7565 2e67 6574 2829 0a0a 2020 2020 2020  ue.get()..      
-00000bb0: 2020 2020 2020 6172 7469 7374 5f6e 616d        artist_nam
-00000bc0: 6520 3d20 2262 7920 2220 2b20 6172 7469  e = "by " + arti
-00000bd0: 7374 5f6e 616d 650a 0a20 2020 2020 2020  st_name..       
-00000be0: 2020 2020 2069 6620 6469 7363 6f72 645f       if discord_
-00000bf0: 636f 6e6e 6563 7465 642e 7661 6c75 653a  connected.value:
-00000c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000c10: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00000c20: 2020 2020 2020 2020 2020 6469 7363 6f72            discor
-00000c30: 645f 7270 632e 7570 6461 7465 280a 2020  d_rpc.update(.  
-00000c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c50: 2020 2020 2020 6465 7461 696c 733d 736f        details=so
-00000c60: 6e67 5f6e 616d 652c 0a20 2020 2020 2020  ng_name,.       
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2073 7461 7465 3d61 7274 6973 745f 6e61   state=artist_na
-00000c90: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
-00000ca0: 2020 2020 2020 2020 2020 2020 6c61 7267              larg
-00000cb0: 655f 696d 6167 653d 226d 6165 7374 726f  e_image="maestro
-00000cc0: 2d69 636f 6e22 2c0a 2020 2020 2020 2020  -icon",.        
-00000cd0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cf0: 2020 736f 6e67 5f6e 616d 6520 3d20 2222    song_name = ""
-00000d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000d10: 2020 2020 2061 7274 6973 745f 6e61 6d65       artist_name
-00000d20: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
-00000d30: 2020 2020 2020 2020 2020 736c 6565 7028            sleep(
-00000d40: 3135 290a 2020 2020 2020 2020 2020 2020  15).            
-00000d50: 2020 2020 6578 6365 7074 3a20 2023 2070      except:  # p
-00000d60: 796c 696e 743a 2064 6973 6162 6c65 3d62  ylint: disable=b
-00000d70: 6172 652d 6578 6365 7074 0a20 2020 2020  are-except.     
-00000d80: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00000d90: 6973 636f 7264 5f63 6f6e 6e65 6374 6564  iscord_connected
-00000da0: 2e76 616c 7565 203d 2030 0a20 2020 2020  .value = 0.     
-00000db0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00000dc0: 2020 2020 2020 2020 2020 2020 2074 7279               try
-00000dd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000de0: 2020 2020 2020 6469 7363 6f72 645f 7270        discord_rp
-00000df0: 6320 3d20 7079 7072 6573 656e 6365 2e50  c = pypresence.P
-00000e00: 7265 7365 6e63 6528 636c 6965 6e74 5f69  resence(client_i
-00000e10: 643d 4449 5343 4f52 445f 4944 290a 2020  d=DISCORD_ID).  
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 6469 7363 6f72 645f 7270 632e 636f    discord_rpc.co
-00000e40: 6e6e 6563 7428 290a 2020 2020 2020 2020  nnect().        
-00000e50: 2020 2020 2020 2020 2020 2020 6469 7363              disc
-00000e60: 6f72 645f 636f 6e6e 6563 7465 642e 7661  ord_connected.va
-00000e70: 6c75 6520 3d20 310a 2020 2020 2020 2020  lue = 1.        
-00000e80: 2020 2020 2020 2020 6578 6365 7074 3a20          except: 
-00000e90: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-00000ea0: 6c65 3d62 6172 652d 6578 6365 7074 0a20  le=bare-except. 
-00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ec0: 2020 2070 6173 730a 0a20 2020 2020 2020     pass..       
-00000ed0: 2020 2020 2020 2020 2069 6620 6469 7363           if disc
-00000ee0: 6f72 645f 636f 6e6e 6563 7465 642e 7661  ord_connected.va
-00000ef0: 6c75 653a 0a20 2020 2020 2020 2020 2020  lue:.           
-00000f00: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f20: 2020 2020 2020 6469 7363 6f72 645f 7270        discord_rp
-00000f30: 632e 7570 6461 7465 280a 2020 2020 2020  c.update(.      
-00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f50: 2020 2020 2020 6465 7461 696c 733d 736f        details=so
-00000f60: 6e67 5f6e 616d 652c 0a20 2020 2020 2020  ng_name,.       
-00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f80: 2020 2020 2073 7461 7465 3d61 7274 6973       state=artis
-00000f90: 745f 6e61 6d65 2c0a 2020 2020 2020 2020  t_name,.        
-00000fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fb0: 2020 2020 6c61 7267 655f 696d 6167 653d      large_image=
-00000fc0: 226d 6165 7374 726f 2d69 636f 6e22 2c0a  "maestro-icon",.
-00000fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fe0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00000ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001000: 2020 736f 6e67 5f6e 616d 6520 3d20 2222    song_name = ""
-00001010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001020: 2020 2020 2020 2020 2061 7274 6973 745f           artist_
-00001030: 6e61 6d65 203d 2022 220a 2020 2020 2020  name = "".      
-00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 2020 736c 6565 7028 3135 290a 2020 2020    sleep(15).    
+00000b20: 2061 7274 6973 745f 6e61 6d65 203d 2022   artist_name = "
+00000b30: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000b40: 2020 6320 3d20 6172 7469 7374 5f71 7565    c = artist_que
+00000b50: 7565 2e67 6574 2829 0a20 2020 2020 2020  ue.get().       
+00000b60: 2020 2020 2020 2020 2077 6869 6c65 2063           while c
+00000b70: 2021 3d20 225c 6e22 3a0a 2020 2020 2020   != "\n":.      
+00000b80: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+00000b90: 7469 7374 5f6e 616d 6520 2b3d 2063 0a20  tist_name += c. 
+00000ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000bb0: 2020 2063 203d 2061 7274 6973 745f 7175     c = artist_qu
+00000bc0: 6575 652e 6765 7428 290a 0a20 2020 2020  eue.get()..     
+00000bd0: 2020 2020 2020 2061 7274 6973 745f 6e61         artist_na
+00000be0: 6d65 203d 2022 6279 2022 202b 2061 7274  me = "by " + art
+00000bf0: 6973 745f 6e61 6d65 0a0a 2020 2020 2020  ist_name..      
+00000c00: 2020 2020 2020 6966 2064 6973 636f 7264        if discord
+00000c10: 5f63 6f6e 6e65 6374 6564 2e76 616c 7565  _connected.value
+00000c20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00000c30: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00000c40: 2020 2020 2020 2020 2020 2064 6973 636f             disco
+00000c50: 7264 5f72 7063 2e75 7064 6174 6528 0a20  rd_rpc.update(. 
+00000c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000c70: 2020 2020 2020 2064 6574 6169 6c73 3d73         details=s
+00000c80: 6f6e 675f 6e61 6d65 2c0a 2020 2020 2020  ong_name,.      
+00000c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ca0: 2020 7374 6174 653d 6172 7469 7374 5f6e    state=artist_n
+00000cb0: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
+00000cc0: 2020 2020 2020 2020 2020 2020 206c 6172               lar
+00000cd0: 6765 5f69 6d61 6765 3d22 6d61 6573 7472  ge_image="maestr
+00000ce0: 6f2d 6963 6f6e 222c 0a20 2020 2020 2020  o-icon",.       
+00000cf0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00000d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d10: 2020 2073 6f6e 675f 6e61 6d65 203d 2022     song_name = "
+00000d20: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00000d30: 2020 2020 2020 6172 7469 7374 5f6e 616d        artist_nam
+00000d40: 6520 3d20 2222 0a20 2020 2020 2020 2020  e = "".         
+00000d50: 2020 2020 2020 2020 2020 2073 6c65 6570             sleep
+00000d60: 2831 3529 0a20 2020 2020 2020 2020 2020  (15).           
+00000d70: 2020 2020 2065 7863 6570 743a 2020 2320       except:  # 
+00000d80: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+00000d90: 6261 7265 2d65 7863 6570 740a 2020 2020  bare-except.    
+00000da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000db0: 6469 7363 6f72 645f 636f 6e6e 6563 7465  discord_connecte
+00000dc0: 642e 7661 6c75 6520 3d20 300a 2020 2020  d.value = 0.    
+00000dd0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00000de0: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+00000df0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+00000e00: 2020 2020 2020 2064 6973 636f 7264 5f72         discord_r
+00000e10: 7063 203d 2070 7970 7265 7365 6e63 652e  pc = pypresence.
+00000e20: 5072 6573 656e 6365 2863 6c69 656e 745f  Presence(client_
+00000e30: 6964 3d44 4953 434f 5244 5f49 4429 0a20  id=DISCORD_ID). 
+00000e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e50: 2020 2064 6973 636f 7264 5f72 7063 2e63     discord_rpc.c
+00000e60: 6f6e 6e65 6374 2829 0a20 2020 2020 2020  onnect().       
+00000e70: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00000e80: 636f 7264 5f63 6f6e 6e65 6374 6564 2e76  cord_connected.v
+00000e90: 616c 7565 203d 2031 0a20 2020 2020 2020  alue = 1.       
+00000ea0: 2020 2020 2020 2020 2065 7863 6570 743a           except:
+00000eb0: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+00000ec0: 626c 653d 6261 7265 2d65 7863 6570 740a  ble=bare-except.
+00000ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ee0: 2020 2020 7061 7373 0a0a 2020 2020 2020      pass..      
+00000ef0: 2020 2020 2020 2020 2020 6966 2064 6973            if dis
+00000f00: 636f 7264 5f63 6f6e 6e65 6374 6564 2e76  cord_connected.v
+00000f10: 616c 7565 3a0a 2020 2020 2020 2020 2020  alue:.          
+00000f20: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00000f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f40: 2020 2020 2020 2064 6973 636f 7264 5f72         discord_r
+00000f50: 7063 2e75 7064 6174 6528 0a20 2020 2020  pc.update(.     
+00000f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f70: 2020 2020 2020 2064 6574 6169 6c73 3d73         details=s
+00000f80: 6f6e 675f 6e61 6d65 2c0a 2020 2020 2020  ong_name,.      
+00000f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fa0: 2020 2020 2020 7374 6174 653d 6172 7469        state=arti
+00000fb0: 7374 5f6e 616d 652c 0a20 2020 2020 2020  st_name,.       
+00000fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000fd0: 2020 2020 206c 6172 6765 5f69 6d61 6765       large_image
+00000fe0: 3d22 6d61 6573 7472 6f2d 6963 6f6e 222c  ="maestro-icon",
+00000ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001000: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00001010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001020: 2020 2073 6f6e 675f 6e61 6d65 203d 2022     song_name = "
+00001030: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00001040: 2020 2020 2020 2020 2020 6172 7469 7374            artist
+00001050: 5f6e 616d 6520 3d20 2222 0a20 2020 2020  _name = "".     
 00001060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001070: 6578 6365 7074 3a20 2023 2070 796c 696e  except:  # pylin
-00001080: 743a 2064 6973 6162 6c65 3d62 6172 652d  t: disable=bare-
-00001090: 6578 6365 7074 0a20 2020 2020 2020 2020  except.         
-000010a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000010b0: 6973 636f 7264 5f63 6f6e 6e65 6374 6564  iscord_connected
-000010c0: 2e76 616c 7565 203d 2030 0a20 2020 2020  .value = 0.     
-000010d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000010e0: 2020 2020 2069 6620 6e6f 7420 6469 7363       if not disc
-000010f0: 6f72 645f 636f 6e6e 6563 7465 642e 7661  ord_connected.va
-00001100: 6c75 653a 0a20 2020 2020 2020 2020 2020  lue:.           
-00001110: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00001120: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00001130: 7363 6f72 645f 7270 6320 3d20 7079 7072  scord_rpc = pypr
-00001140: 6573 656e 6365 2e50 7265 7365 6e63 6528  esence.Presence(
-00001150: 636c 6965 6e74 5f69 643d 4449 5343 4f52  client_id=DISCOR
-00001160: 445f 4944 290a 2020 2020 2020 2020 2020  D_ID).          
-00001170: 2020 2020 2020 2020 2020 6469 7363 6f72            discor
-00001180: 645f 7270 632e 636f 6e6e 6563 7428 290a  d_rpc.connect().
-00001190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011a0: 2020 2020 6469 7363 6f72 645f 636f 6e6e      discord_conn
-000011b0: 6563 7465 642e 7661 6c75 6520 3d20 310a  ected.value = 1.
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011d0: 6578 6365 7074 3a20 2023 2070 796c 696e  except:  # pylin
-000011e0: 743a 2064 6973 6162 6c65 3d62 6172 652d  t: disable=bare-
-000011f0: 6578 6365 7074 0a20 2020 2020 2020 2020  except.         
-00001200: 2020 2020 2020 2020 2020 2070 6173 730a             pass.
-00001210: 0a0a 6465 6620 5f70 6c61 7928 0a20 2020  ..def _play(.   
-00001220: 2073 7464 7363 722c 0a20 2020 2070 6c61   stdscr,.    pla
-00001230: 796c 6973 742c 0a20 2020 2076 6f6c 756d  ylist,.    volum
-00001240: 652c 0a20 2020 206c 6f6f 702c 0a20 2020  e,.    loop,.   
-00001250: 2063 6c69 705f 6d6f 6465 2c0a 2020 2020   clip_mode,.    
-00001260: 7265 7368 7566 666c 652c 0a20 2020 2075  reshuffle,.    u
-00001270: 7064 6174 655f 6469 7363 6f72 642c 0a20  pdate_discord,. 
-00001280: 2020 2076 6973 7561 6c69 7a65 2c0a 293a     visualize,.):
-00001290: 0a20 2020 2067 6c6f 6261 6c20 6361 6e5f  .    global can_
-000012a0: 6d61 635f 6e6f 775f 706c 6179 696e 6720  mac_now_playing 
-000012b0: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
-000012c0: 6c65 3d67 6c6f 6261 6c2d 7374 6174 656d  le=global-statem
-000012d0: 656e 740a 0a20 2020 2069 6e69 745f 6375  ent..    init_cu
-000012e0: 7273 6573 2873 7464 7363 7229 0a0a 2020  rses(stdscr)..  
-000012f0: 2020 6966 206c 6f6f 703a 0a20 2020 2020    if loop:.     
-00001300: 2020 206e 6578 745f 706c 6179 6c69 7374     next_playlist
-00001310: 203d 2070 6c61 796c 6973 745b 3a5d 0a20   = playlist[:]. 
-00001320: 2020 2020 2020 2069 6620 7265 7368 7566         if reshuf
-00001330: 666c 653a 0a20 2020 2020 2020 2020 2020  fle:.           
-00001340: 2073 6875 6666 6c65 286e 6578 745f 706c   shuffle(next_pl
-00001350: 6179 6c69 7374 290a 2020 2020 656c 7365  aylist).    else
-00001360: 3a0a 2020 2020 2020 2020 6e65 7874 5f70  :.        next_p
-00001370: 6c61 796c 6973 7420 3d20 4e6f 6e65 0a0a  laylist = None..
-00001380: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00001390: 7420 3d20 506c 6179 6572 4f75 7470 7574  t = PlayerOutput
-000013a0: 280a 2020 2020 2020 2020 7374 6473 6372  (.        stdscr
-000013b0: 2c20 706c 6179 6c69 7374 2c20 766f 6c75  , playlist, volu
-000013c0: 6d65 2c20 636c 6970 5f6d 6f64 652c 2075  me, clip_mode, u
-000013d0: 7064 6174 655f 6469 7363 6f72 642c 2076  pdate_discord, v
-000013e0: 6973 7561 6c69 7a65 0a20 2020 2029 0a0a  isualize.    )..
-000013f0: 2020 2020 6966 2070 6c61 7965 725f 6f75      if player_ou
-00001400: 7470 7574 2e75 7064 6174 655f 6469 7363  tput.update_disc
-00001410: 6f72 643a 0a20 2020 2020 2020 2064 6973  ord:.        dis
-00001420: 636f 7264 5f73 6f6e 675f 6e61 6d65 5f71  cord_song_name_q
-00001430: 7565 7565 203d 206d 756c 7469 7072 6f63  ueue = multiproc
-00001440: 6573 7369 6e67 2e53 696d 706c 6551 7565  essing.SimpleQue
-00001450: 7565 2829 0a20 2020 2020 2020 2064 6973  ue().        dis
-00001460: 636f 7264 5f61 7274 6973 745f 7175 6575  cord_artist_queu
-00001470: 6520 3d20 6d75 6c74 6970 726f 6365 7373  e = multiprocess
-00001480: 696e 672e 5369 6d70 6c65 5175 6575 6528  ing.SimpleQueue(
-00001490: 290a 2020 2020 2020 2020 6469 7363 6f72  ).        discor
-000014a0: 645f 7072 6573 656e 6365 5f70 726f 6365  d_presence_proce
-000014b0: 7373 203d 206d 756c 7469 7072 6f63 6573  ss = multiproces
-000014c0: 7369 6e67 2e50 726f 6365 7373 280a 2020  sing.Process(.  
-000014d0: 2020 2020 2020 2020 2020 6461 656d 6f6e            daemon
-000014e0: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
-000014f0: 2020 2074 6172 6765 743d 6469 7363 6f72     target=discor
-00001500: 645f 7072 6573 656e 6365 5f6c 6f6f 702c  d_presence_loop,
-00001510: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
-00001520: 733d 280a 2020 2020 2020 2020 2020 2020  s=(.            
-00001530: 2020 2020 6469 7363 6f72 645f 736f 6e67      discord_song
-00001540: 5f6e 616d 655f 7175 6575 652c 0a20 2020  _name_queue,.   
-00001550: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-00001560: 636f 7264 5f61 7274 6973 745f 7175 6575  cord_artist_queu
-00001570: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001580: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00001590: 2e64 6973 636f 7264 5f63 6f6e 6e65 6374  .discord_connect
-000015a0: 6564 2c0a 2020 2020 2020 2020 2020 2020  ed,.            
-000015b0: 292c 0a20 2020 2020 2020 2029 0a20 2020  ),.        ).   
-000015c0: 2020 2020 2064 6973 636f 7264 5f70 7265       discord_pre
-000015d0: 7365 6e63 655f 7072 6f63 6573 732e 7374  sence_process.st
-000015e0: 6172 7428 290a 0a20 2020 2069 6620 7379  art()..    if sy
-000015f0: 732e 706c 6174 666f 726d 203d 3d20 2264  s.platform == "d
-00001600: 6172 7769 6e22 2061 6e64 2063 616e 5f6d  arwin" and can_m
-00001610: 6163 5f6e 6f77 5f70 6c61 7969 6e67 3a0a  ac_now_playing:.
-00001620: 2020 2020 2020 2020 6d61 635f 6e6f 775f          mac_now_
-00001630: 706c 6179 696e 672e 7469 746c 655f 7175  playing.title_qu
-00001640: 6575 6520 3d20 5175 6575 6528 290a 2020  eue = Queue().  
-00001650: 2020 2020 2020 6d61 635f 6e6f 775f 706c        mac_now_pl
-00001660: 6179 696e 672e 6172 7469 7374 5f71 7565  aying.artist_que
-00001670: 7565 203d 2051 7565 7565 2829 0a20 2020  ue = Queue().   
-00001680: 2020 2020 206d 6163 5f6e 6f77 5f70 6c61       mac_now_pla
-00001690: 7969 6e67 2e71 203d 2051 7565 7565 2829  ying.q = Queue()
-000016a0: 0a20 2020 2020 2020 206d 6163 5f6e 6f77  .        mac_now
-000016b0: 5f70 6c61 7969 6e67 2e63 6f76 6572 203d  _playing.cover =
-000016c0: 2063 6f76 6572 5f69 6d67 0a0a 2020 2020   cover_img..    
-000016d0: 2020 2020 6e73 5f61 7070 6c69 6361 7469      ns_applicati
-000016e0: 6f6e 203d 204e 5341 7070 6c69 6361 7469  on = NSApplicati
-000016f0: 6f6e 2e73 6861 7265 6441 7070 6c69 6361  on.sharedApplica
-00001700: 7469 6f6e 2829 0a20 2020 2020 2020 2023  tion().        #
-00001710: 206c 6f67 6f5f 6e73 5f69 6d61 6765 203d   logo_ns_image =
-00001720: 204e 5349 6d61 6765 2e61 6c6c 6f63 2829   NSImage.alloc()
-00001730: 2e69 6e69 7442 7952 6566 6572 656e 6369  .initByReferenci
-00001740: 6e67 4669 6c65 5f28 0a20 2020 2020 2020  ngFile_(.       
-00001750: 2023 2020 2020 2022 2e2f 6d61 6573 7472   #     "./maestr
-00001760: 6f5f 6963 6f6e 2e70 6e67 220a 2020 2020  o_icon.png".    
-00001770: 2020 2020 2320 290a 2020 2020 2020 2020      # ).        
-00001780: 2320 6e73 5f61 7070 6c69 6361 7469 6f6e  # ns_application
-00001790: 2e73 6574 4170 706c 6963 6174 696f 6e49  .setApplicationI
-000017a0: 636f 6e49 6d61 6765 5f28 6c6f 676f 5f6e  conImage_(logo_n
-000017b0: 735f 696d 6167 6529 0a20 2020 2020 2020  s_image).       
-000017c0: 206e 735f 6170 706c 6963 6174 696f 6e2e   ns_application.
-000017d0: 7365 7441 6374 6976 6174 696f 6e50 6f6c  setActivationPol
-000017e0: 6963 795f 280a 2020 2020 2020 2020 2020  icy_(.          
-000017f0: 2020 4e53 4170 706c 6963 6174 696f 6e41    NSApplicationA
-00001800: 6374 6976 6174 696f 6e50 6f6c 6963 7950  ctivationPolicyP
-00001810: 726f 6869 6269 7465 640a 2020 2020 2020  rohibited.      
-00001820: 2020 290a 0a20 2020 2020 2020 2023 204e    )..        # N
-00001830: 4f54 453a 206b 6565 7020 7265 6620 746f  OTE: keep ref to
-00001840: 2064 656c 6567 6174 6520 6f62 6a65 6374   delegate object
-00001850: 2c20 7365 7444 656c 6567 6174 655f 2064  , setDelegate_ d
-00001860: 6f65 736e 2774 2072 6574 6169 6e0a 2020  oesn't retain.  
-00001870: 2020 2020 2020 6465 6c65 6761 7465 203d        delegate =
-00001880: 2041 7070 4465 6c65 6761 7465 2e61 6c6c   AppDelegate.all
-00001890: 6f63 2829 2e69 6e69 7428 290a 2020 2020  oc().init().    
-000018a0: 2020 2020 4e53 4170 7028 292e 7365 7444      NSApp().setD
-000018b0: 656c 6567 6174 655f 2864 656c 6567 6174  elegate_(delegat
-000018c0: 6529 0a0a 2020 2020 2020 2020 6170 705f  e)..        app_
-000018d0: 6865 6c70 6572 5f70 726f 6365 7373 203d  helper_process =
-000018e0: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
-000018f0: 2e50 726f 6365 7373 280a 2020 2020 2020  .Process(.      
-00001900: 2020 2020 2020 6461 656d 6f6e 3d54 7275        daemon=Tru
-00001910: 652c 0a20 2020 2020 2020 2020 2020 2074  e,.            t
-00001920: 6172 6765 743d 6170 705f 6865 6c70 6572  arget=app_helper
-00001930: 5f6c 6f6f 702c 0a20 2020 2020 2020 2029  _loop,.        )
-00001940: 0a20 2020 2020 2020 2061 7070 5f68 656c  .        app_hel
-00001950: 7065 725f 7072 6f63 6573 732e 7374 6172  per_process.star
-00001960: 7428 290a 0a20 2020 2070 7265 765f 766f  t()..    prev_vo
-00001970: 6c75 6d65 203d 2076 6f6c 756d 650a 2020  lume = volume.  
-00001980: 2020 7768 696c 6520 706c 6179 6572 5f6f    while player_o
-00001990: 7574 7075 742e 6920 696e 2072 616e 6765  utput.i in range
-000019a0: 286c 656e 2870 6c61 7965 725f 6f75 7470  (len(player_outp
-000019b0: 7574 2e70 6c61 796c 6973 7429 293a 0a20  ut.playlist)):. 
-000019c0: 2020 2020 2020 2073 6f6e 675f 7061 7468         song_path
-000019d0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-000019e0: 0a20 2020 2020 2020 2020 2020 2053 4f4e  .            SON
-000019f0: 4753 5f44 4952 2c20 706c 6179 6572 5f6f  GS_DIR, player_o
-00001a00: 7574 7075 742e 706c 6179 6c69 7374 5b70  utput.playlist[p
-00001a10: 6c61 7965 725f 6f75 7470 7574 2e69 5d5b  layer_output.i][
-00001a20: 315d 0a20 2020 2020 2020 2029 0a0a 2020  1].        )..  
-00001a30: 2020 2020 2020 706c 6179 6261 636b 203d        playback =
-00001a40: 2050 6c61 7962 6163 6b28 290a 2020 2020   Playback().    
-00001a50: 2020 2020 706c 6179 6261 636b 2e6c 6f61      playback.loa
-00001a60: 645f 6669 6c65 2873 6f6e 675f 7061 7468  d_file(song_path
-00001a70: 290a 0a20 2020 2020 2020 2063 6c69 705f  )..        clip_
-00001a80: 7374 7269 6e67 203d 2070 6c61 7965 725f  string = player_
-00001a90: 6f75 7470 7574 2e70 6c61 796c 6973 745b  output.playlist[
-00001aa0: 706c 6179 6572 5f6f 7574 7075 742e 695d  player_output.i]
-00001ab0: 5b33 5d0a 2020 2020 2020 2020 6966 2063  [3].        if c
-00001ac0: 6c69 705f 7374 7269 6e67 3a0a 2020 2020  lip_string:.    
-00001ad0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00001ae0: 7574 7075 742e 636c 6970 203d 2074 7570  utput.clip = tup
-00001af0: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-00001b00: 2020 2020 6d61 7028 666c 6f61 742c 2070      map(float, p
-00001b10: 6c61 7965 725f 6f75 7470 7574 2e70 6c61  layer_output.pla
-00001b20: 796c 6973 745b 706c 6179 6572 5f6f 7574  ylist[player_out
-00001b30: 7075 742e 695d 5b33 5d2e 7370 6c69 7428  put.i][3].split(
-00001b40: 2929 0a20 2020 2020 2020 2020 2020 2029  )).            )
-00001b50: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00001b60: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00001b70: 725f 6f75 7470 7574 2e63 6c69 7020 3d20  r_output.clip = 
-00001b80: 302c 2070 6c61 7962 6163 6b2e 6475 7261  0, playback.dura
-00001b90: 7469 6f6e 0a0a 2020 2020 2020 2020 706c  tion..        pl
-00001ba0: 6179 6572 5f6f 7574 7075 742e 7061 7573  ayer_output.paus
-00001bb0: 6564 203d 2046 616c 7365 0a20 2020 2020  ed = False.     
-00001bc0: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00001bd0: 2e64 7572 6174 696f 6e20 3d20 6675 6c6c  .duration = full
-00001be0: 5f64 7572 6174 696f 6e20 3d20 706c 6179  _duration = play
-00001bf0: 6261 636b 2e64 7572 6174 696f 6e0a 0a20  back.duration.. 
-00001c00: 2020 2020 2020 2069 6620 7379 732e 706c         if sys.pl
-00001c10: 6174 666f 726d 203d 3d20 2264 6172 7769  atform == "darwi
-00001c20: 6e22 2061 6e64 2063 616e 5f6d 6163 5f6e  n" and can_mac_n
-00001c30: 6f77 5f70 6c61 7969 6e67 3a0a 2020 2020  ow_playing:.    
-00001c40: 2020 2020 2020 2020 6d61 635f 6e6f 775f          mac_now_
-00001c50: 706c 6179 696e 672e 7061 7573 6564 203d  playing.paused =
-00001c60: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-00001c70: 2020 206d 6163 5f6e 6f77 5f70 6c61 7969     mac_now_playi
-00001c80: 6e67 2e70 6f73 203d 2030 0a20 2020 2020  ng.pos = 0.     
-00001c90: 2020 2020 2020 206d 6163 5f6e 6f77 5f70         mac_now_p
-00001ca0: 6c61 7969 6e67 2e6c 656e 6774 6820 3d20  laying.length = 
-00001cb0: 706c 6179 6572 5f6f 7574 7075 742e 6475  player_output.du
-00001cc0: 7261 7469 6f6e 0a0a 2020 2020 2020 2020  ration..        
-00001cd0: 2020 2020 666f 7220 6320 696e 2070 6c61      for c in pla
-00001ce0: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
-00001cf0: 6973 745b 706c 6179 6572 5f6f 7574 7075  ist[player_outpu
-00001d00: 742e 695d 5b31 5d3a 0a20 2020 2020 2020  t.i][1]:.       
-00001d10: 2020 2020 2020 2020 206d 6163 5f6e 6f77           mac_now
-00001d20: 5f70 6c61 7969 6e67 2e74 6974 6c65 5f71  _playing.title_q
-00001d30: 7565 7565 2e70 7574 2863 290a 2020 2020  ueue.put(c).    
-00001d40: 2020 2020 2020 2020 6d61 635f 6e6f 775f          mac_now_
-00001d50: 706c 6179 696e 672e 7469 746c 655f 7175  playing.title_qu
-00001d60: 6575 652e 7075 7428 225c 6e22 290a 0a20  eue.put("\n").. 
-00001d70: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-00001d80: 2069 6e20 706c 6179 6572 5f6f 7574 7075   in player_outpu
-00001d90: 742e 706c 6179 6c69 7374 5b70 6c61 7965  t.playlist[playe
-00001da0: 725f 6f75 7470 7574 2e69 5d5b 2d33 5d3a  r_output.i][-3]:
-00001db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001dc0: 206d 6163 5f6e 6f77 5f70 6c61 7969 6e67   mac_now_playing
-00001dd0: 2e61 7274 6973 745f 7175 6575 652e 7075  .artist_queue.pu
-00001de0: 7428 6329 0a20 2020 2020 2020 2020 2020  t(c).           
-00001df0: 206d 6163 5f6e 6f77 5f70 6c61 7969 6e67   mac_now_playing
-00001e00: 2e61 7274 6973 745f 7175 6575 652e 7075  .artist_queue.pu
-00001e10: 7428 225c 6e22 290a 0a20 2020 2020 2020  t("\n")..       
-00001e20: 2020 2020 2075 7064 6174 655f 6e6f 775f       update_now_
-00001e30: 706c 6179 696e 6720 3d20 5472 7565 0a0a  playing = True..
-00001e40: 2020 2020 2020 2020 6966 2070 6c61 7965          if playe
-00001e50: 725f 6f75 7470 7574 2e75 7064 6174 655f  r_output.update_
-00001e60: 6469 7363 6f72 643a 0a20 2020 2020 2020  discord:.       
-00001e70: 2020 2020 2066 6f72 2063 2069 6e20 706c       for c in pl
-00001e80: 6179 6572 5f6f 7574 7075 742e 706c 6179  ayer_output.play
-00001e90: 6c69 7374 5b70 6c61 7965 725f 6f75 7470  list[player_outp
-00001ea0: 7574 2e69 5d5b 315d 3a0a 2020 2020 2020  ut.i][1]:.      
-00001eb0: 2020 2020 2020 2020 2020 6469 7363 6f72            discor
-00001ec0: 645f 736f 6e67 5f6e 616d 655f 7175 6575  d_song_name_queu
-00001ed0: 652e 7075 7428 6329 0a20 2020 2020 2020  e.put(c).       
-00001ee0: 2020 2020 2064 6973 636f 7264 5f73 6f6e       discord_son
-00001ef0: 675f 6e61 6d65 5f71 7565 7565 2e70 7574  g_name_queue.put
-00001f00: 2822 5c6e 2229 0a0a 2020 2020 2020 2020  ("\n")..        
-00001f10: 2020 2020 666f 7220 6320 696e 2070 6c61      for c in pla
-00001f20: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
-00001f30: 6973 745b 706c 6179 6572 5f6f 7574 7075  ist[player_outpu
-00001f40: 742e 695d 5b2d 335d 3a0a 2020 2020 2020  t.i][-3]:.      
-00001f50: 2020 2020 2020 2020 2020 6469 7363 6f72            discor
-00001f60: 645f 6172 7469 7374 5f71 7565 7565 2e70  d_artist_queue.p
-00001f70: 7574 2863 290a 2020 2020 2020 2020 2020  ut(c).          
-00001f80: 2020 6469 7363 6f72 645f 6172 7469 7374    discord_artist
-00001f90: 5f71 7565 7565 2e70 7574 2822 5c6e 2229  _queue.put("\n")
-00001fa0: 0a0a 2020 2020 2020 2020 706c 6179 6261  ..        playba
-00001fb0: 636b 2e70 6c61 7928 290a 0a20 2020 2020  ck.play()..     
-00001fc0: 2020 2069 6620 706c 6179 6572 5f6f 7574     if player_out
-00001fd0: 7075 742e 636c 6970 5f6d 6f64 653a 0a20  put.clip_mode:. 
-00001fe0: 2020 2020 2020 2020 2020 2063 6c69 705f             clip_
-00001ff0: 7374 6172 742c 2063 6c69 705f 656e 6420  start, clip_end 
-00002000: 3d20 706c 6179 6572 5f6f 7574 7075 742e  = player_output.
-00002010: 636c 6970 0a20 2020 2020 2020 2020 2020  clip.           
-00002020: 2070 6c61 7965 725f 6f75 7470 7574 2e64   player_output.d
-00002030: 7572 6174 696f 6e20 3d20 636c 6970 5f65  uration = clip_e
-00002040: 6e64 202d 2063 6c69 705f 7374 6172 740a  nd - clip_start.
-00002050: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00002060: 6261 636b 2e73 6565 6b28 636c 6970 5f73  back.seek(clip_s
-00002070: 7461 7274 290a 2020 2020 2020 2020 2020  tart).          
-00002080: 2020 6966 2073 7973 2e70 6c61 7466 6f72    if sys.platfor
-00002090: 6d20 3d3d 2022 6461 7277 696e 2220 616e  m == "darwin" an
-000020a0: 6420 6361 6e5f 6d61 635f 6e6f 775f 706c  d can_mac_now_pl
-000020b0: 6179 696e 673a 0a20 2020 2020 2020 2020  aying:.         
-000020c0: 2020 2020 2020 206d 6163 5f6e 6f77 5f70         mac_now_p
-000020d0: 6c61 7969 6e67 2e70 6f73 203d 2072 6f75  laying.pos = rou
-000020e0: 6e64 2870 6c61 7962 6163 6b2e 6375 7272  nd(playback.curr
-000020f0: 5f70 6f73 290a 2020 2020 2020 2020 2020  _pos).          
-00002100: 2020 6c61 7374 5f74 696d 6573 7461 6d70    last_timestamp
-00002110: 203d 2070 6c61 7962 6163 6b2e 6375 7272   = playback.curr
-00002120: 5f70 6f73 0a0a 2020 2020 2020 2020 7374  _pos..        st
-00002130: 6172 745f 7469 6d65 203d 2070 6175 7365  art_time = pause
-00002140: 5f73 7461 7274 203d 2074 696d 6528 290a  _start = time().
-00002150: 2020 2020 2020 2020 706c 6179 6261 636b          playback
-00002160: 2e73 6574 5f76 6f6c 756d 6528 706c 6179  .set_volume(play
-00002170: 6572 5f6f 7574 7075 742e 766f 6c75 6d65  er_output.volume
-00002180: 290a 0a20 2020 2020 2020 206c 6173 745f  )..        last_
-00002190: 7469 6d65 7374 616d 7020 3d20 706c 6179  timestamp = play
-000021a0: 6261 636b 2e63 7572 725f 706f 730a 2020  back.curr_pos.  
-000021b0: 2020 2020 2020 6e65 7874 5f73 6f6e 6720        next_song 
-000021c0: 3d20 3120 2023 202d 3120 6966 2067 6f69  = 1  # -1 if goi
-000021d0: 6e67 2062 6163 6b2c 2030 2069 6620 7265  ng back, 0 if re
-000021e0: 7374 6172 7469 6e67 2c20 2b31 2069 6620  starting, +1 if 
-000021f0: 6e65 7874 2073 6f6e 670a 2020 2020 2020  next song.      
-00002200: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00002210: 656e 6469 6e67 203d 2046 616c 7365 0a20  ending = False. 
-00002220: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
-00002230: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-00002240: 6620 6e6f 7420 706c 6179 6261 636b 2e61  f not playback.a
-00002250: 6374 6976 6520 6f72 2028 0a20 2020 2020  ctive or (.     
-00002260: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00002270: 725f 6f75 7470 7574 2e63 6c69 705f 6d6f  r_output.clip_mo
-00002280: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
-00002290: 2020 2061 6e64 2070 6c61 7962 6163 6b2e     and playback.
-000022a0: 6375 7272 5f70 6f73 203e 2070 6c61 7965  curr_pos > playe
-000022b0: 725f 6f75 7470 7574 2e63 6c69 705b 315d  r_output.clip[1]
-000022c0: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
-000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022e0: 6e65 7874 5f73 6f6e 6720 3d20 6e6f 7420  next_song = not 
-000022f0: 706c 6179 6572 5f6f 7574 7075 742e 6c6f  player_output.lo
-00002300: 6f70 696e 675f 6375 7272 656e 745f 736f  oping_current_so
-00002310: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-00002320: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
-00002330: 2020 2020 2020 2320 6661 6465 2069 6e20        # fade in 
-00002340: 6669 7273 7420 3220 7365 636f 6e64 7320  first 2 seconds 
-00002350: 6f66 2063 6c69 700a 2020 2020 2020 2020  of clip.        
-00002360: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-00002370: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00002380: 6f75 7470 7574 2e63 6c69 705f 6d6f 6465  output.clip_mode
-00002390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000023a0: 2061 6e64 2063 6c69 705f 7374 6172 7420   and clip_start 
-000023b0: 213d 2030 2020 2320 6966 2063 6c69 7020  != 0  # if clip 
-000023c0: 646f 6573 6e27 7420 7374 6172 7420 6174  doesn't start at
-000023d0: 2062 6567 696e 6e69 6e67 0a20 2020 2020   beginning.     
-000023e0: 2020 2020 2020 2020 2020 2061 6e64 2063             and c
-000023f0: 6c69 705f 656e 6420 2d20 636c 6970 5f73  lip_end - clip_s
-00002400: 7461 7274 203e 2035 2020 2320 6966 2063  tart > 5  # if c
-00002410: 6c69 7020 6973 206c 6f6e 6765 7220 7468  lip is longer th
-00002420: 616e 2035 2073 6563 730a 2020 2020 2020  an 5 secs.      
-00002430: 2020 2020 2020 2020 2020 616e 6420 706c            and pl
-00002440: 6179 6261 636b 2e63 7572 725f 706f 7320  ayback.curr_pos 
-00002450: 3c20 636c 6970 5f73 7461 7274 202b 2032  < clip_start + 2
-00002460: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
-00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002480: 706c 6179 6261 636b 2e73 6574 5f76 6f6c  playback.set_vol
-00002490: 756d 6528 0a20 2020 2020 2020 2020 2020  ume(.           
-000024a0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-000024b0: 6f75 7470 7574 2e76 6f6c 756d 6520 2a20  output.volume * 
-000024c0: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
-000024d0: 6f73 202d 2063 6c69 705f 7374 6172 7429  os - clip_start)
-000024e0: 202f 2032 0a20 2020 2020 2020 2020 2020   / 2.           
-000024f0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00002500: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00002510: 2020 2020 2020 2020 2070 6c61 7962 6163           playbac
-00002520: 6b2e 7365 745f 766f 6c75 6d65 2870 6c61  k.set_volume(pla
-00002530: 7965 725f 6f75 7470 7574 2e76 6f6c 756d  yer_output.volum
-00002540: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
-00002550: 6966 2073 7973 2e70 6c61 7466 6f72 6d20  if sys.platform 
-00002560: 3d3d 2022 6461 7277 696e 2220 616e 6420  == "darwin" and 
-00002570: 6361 6e5f 6d61 635f 6e6f 775f 706c 6179  can_mac_now_play
-00002580: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-00002590: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000025a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000025b0: 2075 7064 6174 655f 6e6f 775f 706c 6179   update_now_play
-000025c0: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
-000025d0: 2020 2020 2020 2020 2020 2020 206d 6163               mac
-000025e0: 5f6e 6f77 5f70 6c61 7969 6e67 2e75 7064  _now_playing.upd
-000025f0: 6174 6528 290a 2020 2020 2020 2020 2020  ate().          
-00002600: 2020 2020 2020 2020 2020 2020 2020 7570                up
-00002610: 6461 7465 5f6e 6f77 5f70 6c61 7969 6e67  date_now_playing
-00002620: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00002630: 2020 2020 2020 2020 2020 2020 204e 5352               NSR
-00002640: 756e 4c6f 6f70 2e63 7572 7265 6e74 5275  unLoop.currentRu
-00002650: 6e4c 6f6f 7028 292e 7275 6e55 6e74 696c  nLoop().runUntil
-00002660: 4461 7465 5f28 0a20 2020 2020 2020 2020  Date_(.         
-00002670: 2020 2020 2020 2020 2020 2020 2020 204e                 N
-00002680: 5344 6174 652e 6461 7465 5769 7468 5469  SDate.dateWithTi
-00002690: 6d65 496e 7465 7276 616c 5369 6e63 654e  meIntervalSinceN
-000026a0: 6f77 5f28 302e 3035 290a 2020 2020 2020  ow_(0.05).      
-000026b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-000026c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026d0: 6578 6365 7074 3a20 2023 2070 796c 696e  except:  # pylin
-000026e0: 743a 2064 6973 6162 6c65 3d62 6172 652d  t: disable=bare-
-000026f0: 6578 6365 7074 0a20 2020 2020 2020 2020  except.         
-00002700: 2020 2020 2020 2020 2020 2063 616e 5f6d             can_m
-00002710: 6163 5f6e 6f77 5f70 6c61 7969 6e67 203d  ac_now_playing =
-00002720: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
-00002730: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-00002740: 2020 2020 2020 2020 2073 7973 2e70 6c61           sys.pla
-00002750: 7466 6f72 6d20 3d3d 2022 6461 7277 696e  tform == "darwin
-00002760: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00002770: 2020 616e 6420 6361 6e5f 6d61 635f 6e6f    and can_mac_no
-00002780: 775f 706c 6179 696e 670a 2020 2020 2020  w_playing.      
-00002790: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
-000027a0: 7420 6d61 635f 6e6f 775f 706c 6179 696e  t mac_now_playin
-000027b0: 672e 712e 656d 7074 7928 290a 2020 2020  g.q.empty().    
-000027c0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-000027d0: 2020 2020 2020 2020 2020 2063 203d 206d             c = m
-000027e0: 6163 5f6e 6f77 5f70 6c61 7969 6e67 2e71  ac_now_playing.q
-000027f0: 2e67 6574 2829 0a20 2020 2020 2020 2020  .get().         
-00002800: 2020 2020 2020 2069 6620 6320 696e 2022         if c in "
-00002810: 6e4e 7353 223a 0a20 2020 2020 2020 2020  nNsS":.         
-00002820: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00002850: 7574 7075 742e 6920 3d3d 206c 656e 2870  utput.i == len(p
-00002860: 6c61 7965 725f 6f75 7470 7574 2e70 6c61  layer_output.pla
-00002870: 796c 6973 7429 202d 2031 0a20 2020 2020  ylist) - 1.     
-00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002890: 2020 2061 6e64 206e 6f74 206c 6f6f 700a     and not loop.
-000028a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028b0: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
-000028c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000028d0: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-000028e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 2020 2020 2020 6e65 7874 5f73 6f6e 6720        next_song 
-00002910: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00002920: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00002930: 6261 636b 2e73 746f 7028 290a 2020 2020  back.stop().    
-00002940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002950: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00002960: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
-00002970: 2069 6e20 2262 4270 5022 3a0a 2020 2020   in "bBpP":.    
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 6966 2070 6c61 7965 725f 6f75 7470 7574  if player_output
-000029a0: 2e69 203d 3d20 303a 0a20 2020 2020 2020  .i == 0:.       
-000029b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029c0: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
-000029d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 2020 2020 2020 6e65 7874 5f73 6f6e          next_son
-00002a00: 6720 3d20 2d31 0a20 2020 2020 2020 2020  g = -1.         
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00002a20: 6c61 7962 6163 6b2e 7374 6f70 2829 0a20  layback.stop(). 
-00002a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a40: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00002a50: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00002a60: 6620 6320 696e 2022 7252 223a 0a20 2020  f c in "rR":.   
-00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 2070 6c61 7962 6163 6b2e 7374 6f70 2829   playback.stop()
-00002a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002aa0: 2020 2020 206e 6578 745f 736f 6e67 203d       next_song =
-00002ab0: 2030 0a20 2020 2020 2020 2020 2020 2020   0.             
-00002ac0: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00002ad0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00002ae0: 6620 6320 696e 2022 6545 7151 223a 0a20  f c in "eEqQ":. 
-00002af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b00: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00002b10: 2e65 6e64 696e 6720 3d20 6e6f 7420 706c  .ending = not pl
-00002b20: 6179 6572 5f6f 7574 7075 742e 656e 6469  ayer_output.endi
-00002b30: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-00002b40: 2020 2065 6c69 6620 6320 3d3d 2022 2022     elif c == " "
-00002b50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002b60: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00002b70: 7075 742e 7061 7573 6564 203d 206e 6f74  put.paused = not
-00002b80: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
-00002b90: 6175 7365 640a 0a20 2020 2020 2020 2020  aused..         
-00002ba0: 2020 2020 2020 2020 2020 2069 6620 706c             if pl
-00002bb0: 6179 6572 5f6f 7574 7075 742e 7061 7573  ayer_output.paus
-00002bc0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-00002bd0: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00002be0: 6261 636b 2e70 6175 7365 2829 0a20 2020  back.pause().   
-00002bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c00: 2020 2020 2070 6175 7365 5f73 7461 7274       pause_start
-00002c10: 203d 2074 696d 6528 290a 2020 2020 2020   = time().      
-00002c20: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00002c30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00002c40: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00002c50: 6261 636b 2e72 6573 756d 6528 290a 2020  back.resume().  
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
-00002c80: 202b 3d20 7469 6d65 2829 202d 2070 6175   += time() - pau
-00002c90: 7365 5f73 7461 7274 0a0a 2020 2020 2020  se_start..      
-00002ca0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002cb0: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
-00002cc0: 2022 6461 7277 696e 2220 616e 6420 6361   "darwin" and ca
-00002cd0: 6e5f 6d61 635f 6e6f 775f 706c 6179 696e  n_mac_now_playin
-00002ce0: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-00002cf0: 2020 2020 2020 2020 2020 206d 6163 5f6e             mac_n
-00002d00: 6f77 5f70 6c61 7969 6e67 2e70 6175 7365  ow_playing.pause
-00002d10: 6420 3d20 706c 6179 6572 5f6f 7574 7075  d = player_outpu
-00002d20: 742e 7061 7573 6564 0a20 2020 2020 2020  t.paused.       
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d40: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
-00002d50: 742e 7061 7573 6564 3a0a 2020 2020 2020  t.paused:.      
-00002d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d70: 2020 2020 2020 6d61 635f 6e6f 775f 706c        mac_now_pl
-00002d80: 6179 696e 672e 7061 7573 6528 290a 2020  aying.pause().  
-00002d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002da0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00002db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002dc0: 2020 2020 2020 2020 6d61 635f 6e6f 775f          mac_now_
-00002dd0: 706c 6179 696e 672e 7265 7375 6d65 2829  playing.resume()
-00002de0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002df0: 2020 2020 2020 2020 2075 7064 6174 655f           update_
-00002e00: 6e6f 775f 706c 6179 696e 6720 3d20 5472  now_playing = Tr
-00002e10: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
-00002e20: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00002e30: 7574 7075 742e 6f75 7470 7574 2870 6c61  utput.output(pla
-00002e40: 7962 6163 6b2e 6375 7272 5f70 6f73 290a  yback.curr_pos).
-00002e50: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00002e60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002e70: 2020 6320 3d20 7374 6473 6372 2e67 6574    c = stdscr.get
-00002e80: 6368 2829 0a20 2020 2020 2020 2020 2020  ch().           
-00002e90: 2020 2020 206e 6578 745f 6320 3d20 7374       next_c = st
-00002ea0: 6473 6372 2e67 6574 6368 2829 0a20 2020  dscr.getch().   
-00002eb0: 2020 2020 2020 2020 2020 2020 2077 6869               whi
-00002ec0: 6c65 206e 6578 745f 6320 213d 202d 313a  le next_c != -1:
-00002ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ee0: 2020 2020 2063 2c20 6e65 7874 5f63 203d       c, next_c =
-00002ef0: 206e 6578 745f 632c 2073 7464 7363 722e   next_c, stdscr.
-00002f00: 6765 7463 6828 290a 0a20 2020 2020 2020  getch()..       
-00002f10: 2020 2020 2020 2020 2069 6620 6320 213d           if c !=
-00002f20: 202d 313a 0a20 2020 2020 2020 2020 2020   -1:.           
-00002f30: 2020 2020 2020 2020 2069 6620 706c 6179           if play
-00002f40: 6572 5f6f 7574 7075 742e 6164 6469 6e67  er_output.adding
-00002f50: 5f73 6f6e 6720 6973 204e 6f6e 653a 0a20  _song is None:. 
-00002f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f70: 2020 2020 2020 2069 6620 6320 3d3d 2063         if c == c
-00002f80: 7572 7365 732e 4b45 595f 4c45 4654 3a0a  urses.KEY_LEFT:.
-00002f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fa0: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00002fb0: 6261 636b 2e73 6565 6b28 706c 6179 6261  back.seek(playba
-00002fc0: 636b 2e63 7572 725f 706f 7320 2d20 5343  ck.curr_pos - SC
-00002fd0: 5255 425f 5449 4d45 290a 2020 2020 2020  RUB_TIME).      
-00002fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ff0: 2020 2020 2020 6966 2073 7973 2e70 6c61        if sys.pla
-00003000: 7466 6f72 6d20 3d3d 2022 6461 7277 696e  tform == "darwin
-00003010: 2220 616e 6420 6361 6e5f 6d61 635f 6e6f  " and can_mac_no
-00003020: 775f 706c 6179 696e 673a 0a20 2020 2020  w_playing:.     
-00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003040: 2020 2020 2020 2020 2020 206d 6163 5f6e             mac_n
-00003050: 6f77 5f70 6c61 7969 6e67 2e70 6f73 203d  ow_playing.pos =
-00003060: 2072 6f75 6e64 2870 6c61 7962 6163 6b2e   round(playback.
-00003070: 6375 7272 5f70 6f73 290a 2020 2020 2020  curr_pos).      
-00003080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003090: 2020 2020 2020 2020 2020 7570 6461 7465            update
-000030a0: 5f6e 6f77 5f70 6c61 7969 6e67 203d 2054  _now_playing = T
-000030b0: 7275 650a 0a20 2020 2020 2020 2020 2020  rue..           
-000030c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030d0: 206c 6173 745f 7469 6d65 7374 616d 7020   last_timestamp 
-000030e0: 3d20 706c 6179 6261 636b 2e63 7572 725f  = playback.curr_
-000030f0: 706f 730a 2020 2020 2020 2020 2020 2020  pos.            
-00003100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003110: 706c 6179 6572 5f6f 7574 7075 742e 6f75  player_output.ou
-00003120: 7470 7574 2870 6c61 7962 6163 6b2e 6375  tput(playback.cu
-00003130: 7272 5f70 6f73 290a 2020 2020 2020 2020  rr_pos).        
-00003140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003150: 656c 6966 2063 203d 3d20 6375 7273 6573  elif c == curses
-00003160: 2e4b 4559 5f52 4947 4854 3a0a 2020 2020  .KEY_RIGHT:.    
-00003170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003180: 2020 2020 2020 2020 706c 6179 6261 636b          playback
-00003190: 2e73 6565 6b28 706c 6179 6261 636b 2e63  .seek(playback.c
-000031a0: 7572 725f 706f 7320 2b20 5343 5255 425f  urr_pos + SCRUB_
-000031b0: 5449 4d45 290a 2020 2020 2020 2020 2020  TIME).          
-000031c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031d0: 2020 6966 2073 7973 2e70 6c61 7466 6f72    if sys.platfor
-000031e0: 6d20 3d3d 2022 6461 7277 696e 2220 616e  m == "darwin" an
-000031f0: 6420 6361 6e5f 6d61 635f 6e6f 775f 706c  d can_mac_now_pl
-00003200: 6179 696e 673a 0a20 2020 2020 2020 2020  aying:.         
-00003210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003220: 2020 2020 2020 206d 6163 5f6e 6f77 5f70         mac_now_p
-00003230: 6c61 7969 6e67 2e70 6f73 203d 2072 6f75  laying.pos = rou
-00003240: 6e64 2870 6c61 7962 6163 6b2e 6375 7272  nd(playback.curr
-00003250: 5f70 6f73 290a 2020 2020 2020 2020 2020  _pos).          
-00003260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003270: 2020 2020 2020 7570 6461 7465 5f6e 6f77        update_now
-00003280: 5f70 6c61 7969 6e67 203d 2054 7275 650a  _playing = True.
-00003290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000032a0: 2020 2020 2020 2020 2020 2020 206c 6173               las
-000032b0: 745f 7469 6d65 7374 616d 7020 3d20 706c  t_timestamp = pl
-000032c0: 6179 6261 636b 2e63 7572 725f 706f 730a  ayback.curr_pos.
-000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032e0: 2020 2020 2020 2020 2020 2020 706c 6179              play
-000032f0: 6572 5f6f 7574 7075 742e 6f75 7470 7574  er_output.output
-00003300: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
-00003310: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
-00003320: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00003330: 2063 203d 3d20 6375 7273 6573 2e4b 4559   c == curses.KEY
-00003340: 5f55 503a 0a20 2020 2020 2020 2020 2020  _UP:.           
-00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003360: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
-00003370: 742e 7363 726f 6c6c 6572 2e70 6f73 2021  t.scroller.pos !
-00003380: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033a0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-000033b0: 7574 2e73 6372 6f6c 6c65 722e 7363 726f  ut.scroller.scro
-000033c0: 6c6c 5f62 6163 6b77 6172 6428 290a 2020  ll_backward().  
-000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033e0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-000033f0: 6179 6572 5f6f 7574 7075 742e 6f75 7470  ayer_output.outp
-00003400: 7574 2870 6c61 7962 6163 6b2e 6375 7272  ut(playback.curr
-00003410: 5f70 6f73 290a 2020 2020 2020 2020 2020  _pos).          
-00003420: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00003430: 6966 2063 203d 3d20 6375 7273 6573 2e4b  if c == curses.K
-00003440: 4559 5f44 4f57 4e3a 0a20 2020 2020 2020  EY_DOWN:.       
-00003450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003460: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-00003470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003480: 2020 2020 2020 2020 2020 706c 6179 6572            player
-00003490: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
-000034a0: 2e70 6f73 0a20 2020 2020 2020 2020 2020  .pos.           
+00001070: 2020 2073 6c65 6570 2831 3529 0a20 2020     sleep(15).   
+00001080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001090: 2065 7863 6570 743a 2020 2320 7079 6c69   except:  # pyli
+000010a0: 6e74 3a20 6469 7361 626c 653d 6261 7265  nt: disable=bare
+000010b0: 2d65 7863 6570 740a 2020 2020 2020 2020  -except.        
+000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010d0: 6469 7363 6f72 645f 636f 6e6e 6563 7465  discord_connecte
+000010e0: 642e 7661 6c75 6520 3d20 300a 2020 2020  d.value = 0.    
+000010f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00001100: 2020 2020 2020 6966 206e 6f74 2064 6973        if not dis
+00001110: 636f 7264 5f63 6f6e 6e65 6374 6564 2e76  cord_connected.v
+00001120: 616c 7565 3a0a 2020 2020 2020 2020 2020  alue:.          
+00001130: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00001140: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00001150: 6973 636f 7264 5f72 7063 203d 2070 7970  iscord_rpc = pyp
+00001160: 7265 7365 6e63 652e 5072 6573 656e 6365  resence.Presence
+00001170: 2863 6c69 656e 745f 6964 3d44 4953 434f  (client_id=DISCO
+00001180: 5244 5f49 4429 0a20 2020 2020 2020 2020  RD_ID).         
+00001190: 2020 2020 2020 2020 2020 2064 6973 636f             disco
+000011a0: 7264 5f72 7063 2e63 6f6e 6e65 6374 2829  rd_rpc.connect()
+000011b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000011c0: 2020 2020 2064 6973 636f 7264 5f63 6f6e       discord_con
+000011d0: 6e65 6374 6564 2e76 616c 7565 203d 2031  nected.value = 1
+000011e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000011f0: 2065 7863 6570 743a 2020 2320 7079 6c69   except:  # pyli
+00001200: 6e74 3a20 6469 7361 626c 653d 6261 7265  nt: disable=bare
+00001210: 2d65 7863 6570 740a 2020 2020 2020 2020  -except.        
+00001220: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00001230: 0a0a 0a64 6566 205f 706c 6179 280a 2020  ...def _play(.  
+00001240: 2020 7374 6473 6372 2c0a 2020 2020 706c    stdscr,.    pl
+00001250: 6179 6c69 7374 2c0a 2020 2020 766f 6c75  aylist,.    volu
+00001260: 6d65 2c0a 2020 2020 6c6f 6f70 2c0a 2020  me,.    loop,.  
+00001270: 2020 636c 6970 5f6d 6f64 652c 0a20 2020    clip_mode,.   
+00001280: 2072 6573 6875 6666 6c65 2c0a 2020 2020   reshuffle,.    
+00001290: 7570 6461 7465 5f64 6973 636f 7264 2c0a  update_discord,.
+000012a0: 2020 2020 7669 7375 616c 697a 652c 0a29      visualize,.)
+000012b0: 3a0a 2020 2020 676c 6f62 616c 2063 616e  :.    global can
+000012c0: 5f6d 6163 5f6e 6f77 5f70 6c61 7969 6e67  _mac_now_playing
+000012d0: 2020 2320 7079 6c69 6e74 3a20 6469 7361    # pylint: disa
+000012e0: 626c 653d 676c 6f62 616c 2d73 7461 7465  ble=global-state
+000012f0: 6d65 6e74 0a0a 2020 2020 696e 6974 5f63  ment..    init_c
+00001300: 7572 7365 7328 7374 6473 6372 290a 0a20  urses(stdscr).. 
+00001310: 2020 2069 6620 6c6f 6f70 3a0a 2020 2020     if loop:.    
+00001320: 2020 2020 6e65 7874 5f70 6c61 796c 6973      next_playlis
+00001330: 7420 3d20 706c 6179 6c69 7374 5b3a 5d0a  t = playlist[:].
+00001340: 2020 2020 2020 2020 6966 2072 6573 6875          if reshu
+00001350: 6666 6c65 3a0a 2020 2020 2020 2020 2020  ffle:.          
+00001360: 2020 7368 7566 666c 6528 6e65 7874 5f70    shuffle(next_p
+00001370: 6c61 796c 6973 7429 0a20 2020 2065 6c73  laylist).    els
+00001380: 653a 0a20 2020 2020 2020 206e 6578 745f  e:.        next_
+00001390: 706c 6179 6c69 7374 203d 204e 6f6e 650a  playlist = None.
+000013a0: 0a20 2020 2070 6c61 7965 725f 6f75 7470  .    player_outp
+000013b0: 7574 203d 2050 6c61 7965 724f 7574 7075  ut = PlayerOutpu
+000013c0: 7428 0a20 2020 2020 2020 2073 7464 7363  t(.        stdsc
+000013d0: 722c 2070 6c61 796c 6973 742c 2076 6f6c  r, playlist, vol
+000013e0: 756d 652c 2063 6c69 705f 6d6f 6465 2c20  ume, clip_mode, 
+000013f0: 7570 6461 7465 5f64 6973 636f 7264 2c20  update_discord, 
+00001400: 7669 7375 616c 697a 650a 2020 2020 290a  visualize.    ).
+00001410: 0a20 2020 2069 6620 706c 6179 6572 5f6f  .    if player_o
+00001420: 7574 7075 742e 7570 6461 7465 5f64 6973  utput.update_dis
+00001430: 636f 7264 3a0a 2020 2020 2020 2020 6469  cord:.        di
+00001440: 7363 6f72 645f 736f 6e67 5f6e 616d 655f  scord_song_name_
+00001450: 7175 6575 6520 3d20 6d75 6c74 6970 726f  queue = multipro
+00001460: 6365 7373 696e 672e 5369 6d70 6c65 5175  cessing.SimpleQu
+00001470: 6575 6528 290a 2020 2020 2020 2020 6469  eue().        di
+00001480: 7363 6f72 645f 6172 7469 7374 5f71 7565  scord_artist_que
+00001490: 7565 203d 206d 756c 7469 7072 6f63 6573  ue = multiproces
+000014a0: 7369 6e67 2e53 696d 706c 6551 7565 7565  sing.SimpleQueue
+000014b0: 2829 0a20 2020 2020 2020 2064 6973 636f  ().        disco
+000014c0: 7264 5f70 7265 7365 6e63 655f 7072 6f63  rd_presence_proc
+000014d0: 6573 7320 3d20 6d75 6c74 6970 726f 6365  ess = multiproce
+000014e0: 7373 696e 672e 5072 6f63 6573 7328 0a20  ssing.Process(. 
+000014f0: 2020 2020 2020 2020 2020 2064 6165 6d6f             daemo
+00001500: 6e3d 5472 7565 2c0a 2020 2020 2020 2020  n=True,.        
+00001510: 2020 2020 7461 7267 6574 3d64 6973 636f      target=disco
+00001520: 7264 5f70 7265 7365 6e63 655f 6c6f 6f70  rd_presence_loop
+00001530: 2c0a 2020 2020 2020 2020 2020 2020 6172  ,.            ar
+00001540: 6773 3d28 0a20 2020 2020 2020 2020 2020  gs=(.           
+00001550: 2020 2020 2064 6973 636f 7264 5f73 6f6e       discord_son
+00001560: 675f 6e61 6d65 5f71 7565 7565 2c0a 2020  g_name_queue,.  
+00001570: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00001580: 7363 6f72 645f 6172 7469 7374 5f71 7565  scord_artist_que
+00001590: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+000015a0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+000015b0: 742e 6469 7363 6f72 645f 636f 6e6e 6563  t.discord_connec
+000015c0: 7465 642c 0a20 2020 2020 2020 2020 2020  ted,.           
+000015d0: 2029 2c0a 2020 2020 2020 2020 290a 2020   ),.        ).  
+000015e0: 2020 2020 2020 6469 7363 6f72 645f 7072        discord_pr
+000015f0: 6573 656e 6365 5f70 726f 6365 7373 2e73  esence_process.s
+00001600: 7461 7274 2829 0a0a 2020 2020 6966 2073  tart()..    if s
+00001610: 7973 2e70 6c61 7466 6f72 6d20 3d3d 2022  ys.platform == "
+00001620: 6461 7277 696e 2220 616e 6420 6361 6e5f  darwin" and can_
+00001630: 6d61 635f 6e6f 775f 706c 6179 696e 673a  mac_now_playing:
+00001640: 0a20 2020 2020 2020 206d 6163 5f6e 6f77  .        mac_now
+00001650: 5f70 6c61 7969 6e67 2e74 6974 6c65 5f71  _playing.title_q
+00001660: 7565 7565 203d 2051 7565 7565 2829 0a20  ueue = Queue(). 
+00001670: 2020 2020 2020 206d 6163 5f6e 6f77 5f70         mac_now_p
+00001680: 6c61 7969 6e67 2e61 7274 6973 745f 7175  laying.artist_qu
+00001690: 6575 6520 3d20 5175 6575 6528 290a 2020  eue = Queue().  
+000016a0: 2020 2020 2020 6d61 635f 6e6f 775f 706c        mac_now_pl
+000016b0: 6179 696e 672e 7120 3d20 5175 6575 6528  aying.q = Queue(
+000016c0: 290a 2020 2020 2020 2020 6d61 635f 6e6f  ).        mac_no
+000016d0: 775f 706c 6179 696e 672e 636f 7665 7220  w_playing.cover 
+000016e0: 3d20 636f 7665 725f 696d 670a 0a20 2020  = cover_img..   
+000016f0: 2020 2020 206e 735f 6170 706c 6963 6174       ns_applicat
+00001700: 696f 6e20 3d20 4e53 4170 706c 6963 6174  ion = NSApplicat
+00001710: 696f 6e2e 7368 6172 6564 4170 706c 6963  ion.sharedApplic
+00001720: 6174 696f 6e28 290a 2020 2020 2020 2020  ation().        
+00001730: 2320 6c6f 676f 5f6e 735f 696d 6167 6520  # logo_ns_image 
+00001740: 3d20 4e53 496d 6167 652e 616c 6c6f 6328  = NSImage.alloc(
+00001750: 292e 696e 6974 4279 5265 6665 7265 6e63  ).initByReferenc
+00001760: 696e 6746 696c 655f 280a 2020 2020 2020  ingFile_(.      
+00001770: 2020 2320 2020 2020 222e 2f6d 6165 7374    #     "./maest
+00001780: 726f 5f69 636f 6e2e 706e 6722 0a20 2020  ro_icon.png".   
+00001790: 2020 2020 2023 2029 0a20 2020 2020 2020       # ).       
+000017a0: 2023 206e 735f 6170 706c 6963 6174 696f   # ns_applicatio
+000017b0: 6e2e 7365 7441 7070 6c69 6361 7469 6f6e  n.setApplication
+000017c0: 4963 6f6e 496d 6167 655f 286c 6f67 6f5f  IconImage_(logo_
+000017d0: 6e73 5f69 6d61 6765 290a 2020 2020 2020  ns_image).      
+000017e0: 2020 6e73 5f61 7070 6c69 6361 7469 6f6e    ns_application
+000017f0: 2e73 6574 4163 7469 7661 7469 6f6e 506f  .setActivationPo
+00001800: 6c69 6379 5f28 0a20 2020 2020 2020 2020  licy_(.         
+00001810: 2020 204e 5341 7070 6c69 6361 7469 6f6e     NSApplication
+00001820: 4163 7469 7661 7469 6f6e 506f 6c69 6379  ActivationPolicy
+00001830: 5072 6f68 6962 6974 6564 0a20 2020 2020  Prohibited.     
+00001840: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
+00001850: 4e4f 5445 3a20 6b65 6570 2072 6566 2074  NOTE: keep ref t
+00001860: 6f20 6465 6c65 6761 7465 206f 626a 6563  o delegate objec
+00001870: 742c 2073 6574 4465 6c65 6761 7465 5f20  t, setDelegate_ 
+00001880: 646f 6573 6e27 7420 7265 7461 696e 0a20  doesn't retain. 
+00001890: 2020 2020 2020 2064 656c 6567 6174 6520         delegate 
+000018a0: 3d20 4170 7044 656c 6567 6174 652e 616c  = AppDelegate.al
+000018b0: 6c6f 6328 292e 696e 6974 2829 0a20 2020  loc().init().   
+000018c0: 2020 2020 204e 5341 7070 2829 2e73 6574       NSApp().set
+000018d0: 4465 6c65 6761 7465 5f28 6465 6c65 6761  Delegate_(delega
+000018e0: 7465 290a 0a20 2020 2020 2020 2061 7070  te)..        app
+000018f0: 5f68 656c 7065 725f 7072 6f63 6573 7320  _helper_process 
+00001900: 3d20 6d75 6c74 6970 726f 6365 7373 696e  = multiprocessin
+00001910: 672e 5072 6f63 6573 7328 0a20 2020 2020  g.Process(.     
+00001920: 2020 2020 2020 2064 6165 6d6f 6e3d 5472         daemon=Tr
+00001930: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00001940: 7461 7267 6574 3d61 7070 5f68 656c 7065  target=app_helpe
+00001950: 725f 6c6f 6f70 2c0a 2020 2020 2020 2020  r_loop,.        
+00001960: 290a 2020 2020 2020 2020 6170 705f 6865  ).        app_he
+00001970: 6c70 6572 5f70 726f 6365 7373 2e73 7461  lper_process.sta
+00001980: 7274 2829 0a0a 2020 2020 7072 6576 5f76  rt()..    prev_v
+00001990: 6f6c 756d 6520 3d20 766f 6c75 6d65 0a20  olume = volume. 
+000019a0: 2020 2077 6869 6c65 2070 6c61 7965 725f     while player_
+000019b0: 6f75 7470 7574 2e69 2069 6e20 7261 6e67  output.i in rang
+000019c0: 6528 6c65 6e28 706c 6179 6572 5f6f 7574  e(len(player_out
+000019d0: 7075 742e 706c 6179 6c69 7374 2929 3a0a  put.playlist)):.
+000019e0: 2020 2020 2020 2020 736f 6e67 5f70 6174          song_pat
+000019f0: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+00001a00: 280a 2020 2020 2020 2020 2020 2020 534f  (.            SO
+00001a10: 4e47 535f 4449 522c 2070 6c61 7965 725f  NGS_DIR, player_
+00001a20: 6f75 7470 7574 2e70 6c61 796c 6973 745b  output.playlist[
+00001a30: 706c 6179 6572 5f6f 7574 7075 742e 695d  player_output.i]
+00001a40: 5b31 5d0a 2020 2020 2020 2020 290a 0a20  [1].        ).. 
+00001a50: 2020 2020 2020 2070 6c61 7962 6163 6b20         playback 
+00001a60: 3d20 506c 6179 6261 636b 2829 0a20 2020  = Playback().   
+00001a70: 2020 2020 2070 6c61 7962 6163 6b2e 6c6f       playback.lo
+00001a80: 6164 5f66 696c 6528 736f 6e67 5f70 6174  ad_file(song_pat
+00001a90: 6829 0a0a 2020 2020 2020 2020 636c 6970  h)..        clip
+00001aa0: 5f73 7472 696e 6720 3d20 706c 6179 6572  _string = player
+00001ab0: 5f6f 7574 7075 742e 706c 6179 6c69 7374  _output.playlist
+00001ac0: 5b70 6c61 7965 725f 6f75 7470 7574 2e69  [player_output.i
+00001ad0: 5d5b 335d 0a20 2020 2020 2020 2069 6620  ][3].        if 
+00001ae0: 636c 6970 5f73 7472 696e 673a 0a20 2020  clip_string:.   
+00001af0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+00001b00: 6f75 7470 7574 2e63 6c69 7020 3d20 7475  output.clip = tu
+00001b10: 706c 6528 0a20 2020 2020 2020 2020 2020  ple(.           
+00001b20: 2020 2020 206d 6170 2866 6c6f 6174 2c20       map(float, 
+00001b30: 706c 6179 6572 5f6f 7574 7075 742e 706c  player_output.pl
+00001b40: 6179 6c69 7374 5b70 6c61 7965 725f 6f75  aylist[player_ou
+00001b50: 7470 7574 2e69 5d5b 335d 2e73 706c 6974  tput.i][3].split
+00001b60: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+00001b70: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00001b80: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00001b90: 6572 5f6f 7574 7075 742e 636c 6970 203d  er_output.clip =
+00001ba0: 2030 2c20 706c 6179 6261 636b 2e64 7572   0, playback.dur
+00001bb0: 6174 696f 6e0a 0a20 2020 2020 2020 2070  ation..        p
+00001bc0: 6c61 7965 725f 6f75 7470 7574 2e70 6175  layer_output.pau
+00001bd0: 7365 6420 3d20 4661 6c73 650a 2020 2020  sed = False.    
+00001be0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+00001bf0: 742e 6475 7261 7469 6f6e 203d 2066 756c  t.duration = ful
+00001c00: 6c5f 6475 7261 7469 6f6e 203d 2070 6c61  l_duration = pla
+00001c10: 7962 6163 6b2e 6475 7261 7469 6f6e 0a0a  yback.duration..
+00001c20: 2020 2020 2020 2020 6966 2073 7973 2e70          if sys.p
+00001c30: 6c61 7466 6f72 6d20 3d3d 2022 6461 7277  latform == "darw
+00001c40: 696e 2220 616e 6420 6361 6e5f 6d61 635f  in" and can_mac_
+00001c50: 6e6f 775f 706c 6179 696e 673a 0a20 2020  now_playing:.   
+00001c60: 2020 2020 2020 2020 206d 6163 5f6e 6f77           mac_now
+00001c70: 5f70 6c61 7969 6e67 2e70 6175 7365 6420  _playing.paused 
+00001c80: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00001c90: 2020 2020 6d61 635f 6e6f 775f 706c 6179      mac_now_play
+00001ca0: 696e 672e 706f 7320 3d20 300a 2020 2020  ing.pos = 0.    
+00001cb0: 2020 2020 2020 2020 6d61 635f 6e6f 775f          mac_now_
+00001cc0: 706c 6179 696e 672e 6c65 6e67 7468 203d  playing.length =
+00001cd0: 2070 6c61 7965 725f 6f75 7470 7574 2e64   player_output.d
+00001ce0: 7572 6174 696f 6e0a 0a20 2020 2020 2020  uration..       
+00001cf0: 2020 2020 206d 756c 7469 7072 6f63 6573       multiproces
+00001d00: 7369 6e67 5f70 7574 5f77 6f72 6428 0a20  sing_put_word(. 
+00001d10: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00001d20: 6163 5f6e 6f77 5f70 6c61 7969 6e67 2e74  ac_now_playing.t
+00001d30: 6974 6c65 5f71 7565 7565 2c0a 2020 2020  itle_queue,.    
+00001d40: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00001d50: 6572 5f6f 7574 7075 742e 706c 6179 6c69  er_output.playli
+00001d60: 7374 5b70 6c61 7965 725f 6f75 7470 7574  st[player_output
+00001d70: 2e69 5d5b 315d 2c0a 2020 2020 2020 2020  .i][1],.        
+00001d80: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00001d90: 2020 6d75 6c74 6970 726f 6365 7373 696e    multiprocessin
+00001da0: 675f 7075 745f 776f 7264 280a 2020 2020  g_put_word(.    
+00001db0: 2020 2020 2020 2020 2020 2020 6d61 635f              mac_
+00001dc0: 6e6f 775f 706c 6179 696e 672e 7469 746c  now_playing.titl
+00001dd0: 655f 7175 6575 652c 0a20 2020 2020 2020  e_queue,.       
+00001de0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+00001df0: 6f75 7470 7574 2e70 6c61 796c 6973 745b  output.playlist[
+00001e00: 706c 6179 6572 5f6f 7574 7075 742e 695d  player_output.i]
+00001e10: 5b2d 335d 2c0a 2020 2020 2020 2020 2020  [-3],.          
+00001e20: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00001e30: 2075 7064 6174 655f 6e6f 775f 706c 6179   update_now_play
+00001e40: 696e 6720 3d20 5472 7565 0a0a 2020 2020  ing = True..    
+00001e50: 2020 2020 6966 2070 6c61 7965 725f 6f75      if player_ou
+00001e60: 7470 7574 2e75 7064 6174 655f 6469 7363  tput.update_disc
+00001e70: 6f72 643a 0a20 2020 2020 2020 2020 2020  ord:.           
+00001e80: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
+00001e90: 5f70 7574 5f77 6f72 6428 0a20 2020 2020  _put_word(.     
+00001ea0: 2020 2020 2020 2020 2020 2064 6973 636f             disco
+00001eb0: 7264 5f61 7274 6973 745f 7175 6575 652c  rd_artist_queue,
+00001ec0: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+00001ed0: 6c61 796c 6973 745b 706c 6179 6572 5f6f  laylist[player_o
+00001ee0: 7574 7075 742e 695d 5b31 5d0a 2020 2020  utput.i][1].    
+00001ef0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00001f00: 2020 2020 2020 6d75 6c74 6970 726f 6365        multiproce
+00001f10: 7373 696e 675f 7075 745f 776f 7264 280a  ssing_put_word(.
+00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001f30: 6469 7363 6f72 645f 6172 7469 7374 5f71  discord_artist_q
+00001f40: 7565 7565 2c0a 2020 2020 2020 2020 2020  ueue,.          
+00001f50: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00001f60: 7075 742e 706c 6179 6c69 7374 5b70 6c61  put.playlist[pla
+00001f70: 7965 725f 6f75 7470 7574 2e69 5d5b 2d33  yer_output.i][-3
+00001f80: 5d2c 0a20 2020 2020 2020 2020 2020 2029  ],.            )
+00001f90: 0a0a 2020 2020 2020 2020 706c 6179 6261  ..        playba
+00001fa0: 636b 2e70 6c61 7928 290a 0a20 2020 2020  ck.play()..     
+00001fb0: 2020 2069 6620 706c 6179 6572 5f6f 7574     if player_out
+00001fc0: 7075 742e 636c 6970 5f6d 6f64 653a 0a20  put.clip_mode:. 
+00001fd0: 2020 2020 2020 2020 2020 2063 6c69 705f             clip_
+00001fe0: 7374 6172 742c 2063 6c69 705f 656e 6420  start, clip_end 
+00001ff0: 3d20 706c 6179 6572 5f6f 7574 7075 742e  = player_output.
+00002000: 636c 6970 0a20 2020 2020 2020 2020 2020  clip.           
+00002010: 2070 6c61 7965 725f 6f75 7470 7574 2e64   player_output.d
+00002020: 7572 6174 696f 6e20 3d20 636c 6970 5f65  uration = clip_e
+00002030: 6e64 202d 2063 6c69 705f 7374 6172 740a  nd - clip_start.
+00002040: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00002050: 6261 636b 2e73 6565 6b28 636c 6970 5f73  back.seek(clip_s
+00002060: 7461 7274 290a 2020 2020 2020 2020 2020  tart).          
+00002070: 2020 6966 2073 7973 2e70 6c61 7466 6f72    if sys.platfor
+00002080: 6d20 3d3d 2022 6461 7277 696e 2220 616e  m == "darwin" an
+00002090: 6420 6361 6e5f 6d61 635f 6e6f 775f 706c  d can_mac_now_pl
+000020a0: 6179 696e 673a 0a20 2020 2020 2020 2020  aying:.         
+000020b0: 2020 2020 2020 206d 6163 5f6e 6f77 5f70         mac_now_p
+000020c0: 6c61 7969 6e67 2e70 6f73 203d 2072 6f75  laying.pos = rou
+000020d0: 6e64 2870 6c61 7962 6163 6b2e 6375 7272  nd(playback.curr
+000020e0: 5f70 6f73 290a 2020 2020 2020 2020 2020  _pos).          
+000020f0: 2020 6c61 7374 5f74 696d 6573 7461 6d70    last_timestamp
+00002100: 203d 2070 6c61 7962 6163 6b2e 6375 7272   = playback.curr
+00002110: 5f70 6f73 0a0a 2020 2020 2020 2020 7374  _pos..        st
+00002120: 6172 745f 7469 6d65 203d 2070 6175 7365  art_time = pause
+00002130: 5f73 7461 7274 203d 2074 696d 6528 290a  _start = time().
+00002140: 2020 2020 2020 2020 706c 6179 6261 636b          playback
+00002150: 2e73 6574 5f76 6f6c 756d 6528 706c 6179  .set_volume(play
+00002160: 6572 5f6f 7574 7075 742e 766f 6c75 6d65  er_output.volume
+00002170: 290a 0a20 2020 2020 2020 206c 6173 745f  )..        last_
+00002180: 7469 6d65 7374 616d 7020 3d20 706c 6179  timestamp = play
+00002190: 6261 636b 2e63 7572 725f 706f 730a 2020  back.curr_pos.  
+000021a0: 2020 2020 2020 6e65 7874 5f73 6f6e 6720        next_song 
+000021b0: 3d20 3120 2023 202d 3120 6966 2067 6f69  = 1  # -1 if goi
+000021c0: 6e67 2062 6163 6b2c 2030 2069 6620 7265  ng back, 0 if re
+000021d0: 7374 6172 7469 6e67 2c20 2b31 2069 6620  starting, +1 if 
+000021e0: 6e65 7874 2073 6f6e 670a 2020 2020 2020  next song.      
+000021f0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+00002200: 656e 6469 6e67 203d 2046 616c 7365 0a20  ending = False. 
+00002210: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
+00002220: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
+00002230: 6620 6e6f 7420 706c 6179 6261 636b 2e61  f not playback.a
+00002240: 6374 6976 6520 6f72 2028 0a20 2020 2020  ctive or (.     
+00002250: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+00002260: 725f 6f75 7470 7574 2e63 6c69 705f 6d6f  r_output.clip_mo
+00002270: 6465 0a20 2020 2020 2020 2020 2020 2020  de.             
+00002280: 2020 2061 6e64 2070 6c61 7962 6163 6b2e     and playback.
+00002290: 6375 7272 5f70 6f73 203e 2070 6c61 7965  curr_pos > playe
+000022a0: 725f 6f75 7470 7574 2e63 6c69 705b 315d  r_output.clip[1]
+000022b0: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
+000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000022d0: 6e65 7874 5f73 6f6e 6720 3d20 6e6f 7420  next_song = not 
+000022e0: 706c 6179 6572 5f6f 7574 7075 742e 6c6f  player_output.lo
+000022f0: 6f70 696e 675f 6375 7272 656e 745f 736f  oping_current_so
+00002300: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+00002310: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
+00002320: 2020 2020 2020 2320 6661 6465 2069 6e20        # fade in 
+00002330: 6669 7273 7420 3220 7365 636f 6e64 7320  first 2 seconds 
+00002340: 6f66 2063 6c69 700a 2020 2020 2020 2020  of clip.        
+00002350: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+00002360: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+00002370: 6f75 7470 7574 2e63 6c69 705f 6d6f 6465  output.clip_mode
+00002380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002390: 2061 6e64 2063 6c69 705f 7374 6172 7420   and clip_start 
+000023a0: 213d 2030 2020 2320 6966 2063 6c69 7020  != 0  # if clip 
+000023b0: 646f 6573 6e27 7420 7374 6172 7420 6174  doesn't start at
+000023c0: 2062 6567 696e 6e69 6e67 0a20 2020 2020   beginning.     
+000023d0: 2020 2020 2020 2020 2020 2061 6e64 2063             and c
+000023e0: 6c69 705f 656e 6420 2d20 636c 6970 5f73  lip_end - clip_s
+000023f0: 7461 7274 203e 2035 2020 2320 6966 2063  tart > 5  # if c
+00002400: 6c69 7020 6973 206c 6f6e 6765 7220 7468  lip is longer th
+00002410: 616e 2035 2073 6563 730a 2020 2020 2020  an 5 secs.      
+00002420: 2020 2020 2020 2020 2020 616e 6420 706c            and pl
+00002430: 6179 6261 636b 2e63 7572 725f 706f 7320  ayback.curr_pos 
+00002440: 3c20 636c 6970 5f73 7461 7274 202b 2032  < clip_start + 2
+00002450: 0a20 2020 2020 2020 2020 2020 2029 3a0a  .            ):.
+00002460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002470: 706c 6179 6261 636b 2e73 6574 5f76 6f6c  playback.set_vol
+00002480: 756d 6528 0a20 2020 2020 2020 2020 2020  ume(.           
+00002490: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+000024a0: 6f75 7470 7574 2e76 6f6c 756d 6520 2a20  output.volume * 
+000024b0: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
+000024c0: 6f73 202d 2063 6c69 705f 7374 6172 7429  os - clip_start)
+000024d0: 202f 2032 0a20 2020 2020 2020 2020 2020   / 2.           
+000024e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000024f0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00002500: 2020 2020 2020 2020 2070 6c61 7962 6163           playbac
+00002510: 6b2e 7365 745f 766f 6c75 6d65 2870 6c61  k.set_volume(pla
+00002520: 7965 725f 6f75 7470 7574 2e76 6f6c 756d  yer_output.volum
+00002530: 6529 0a0a 2020 2020 2020 2020 2020 2020  e)..            
+00002540: 6966 2073 7973 2e70 6c61 7466 6f72 6d20  if sys.platform 
+00002550: 3d3d 2022 6461 7277 696e 2220 616e 6420  == "darwin" and 
+00002560: 6361 6e5f 6d61 635f 6e6f 775f 706c 6179  can_mac_now_play
+00002570: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00002580: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00002590: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000025a0: 2075 7064 6174 655f 6e6f 775f 706c 6179   update_now_play
+000025b0: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+000025c0: 2020 2020 2020 2020 2020 2020 206d 6163               mac
+000025d0: 5f6e 6f77 5f70 6c61 7969 6e67 2e75 7064  _now_playing.upd
+000025e0: 6174 6528 290a 2020 2020 2020 2020 2020  ate().          
+000025f0: 2020 2020 2020 2020 2020 2020 2020 7570                up
+00002600: 6461 7465 5f6e 6f77 5f70 6c61 7969 6e67  date_now_playing
+00002610: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00002620: 2020 2020 2020 2020 2020 2020 204e 5352               NSR
+00002630: 756e 4c6f 6f70 2e63 7572 7265 6e74 5275  unLoop.currentRu
+00002640: 6e4c 6f6f 7028 292e 7275 6e55 6e74 696c  nLoop().runUntil
+00002650: 4461 7465 5f28 0a20 2020 2020 2020 2020  Date_(.         
+00002660: 2020 2020 2020 2020 2020 2020 2020 204e                 N
+00002670: 5344 6174 652e 6461 7465 5769 7468 5469  SDate.dateWithTi
+00002680: 6d65 496e 7465 7276 616c 5369 6e63 654e  meIntervalSinceN
+00002690: 6f77 5f28 302e 3035 290a 2020 2020 2020  ow_(0.05).      
+000026a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 6578 6365 7074 3a20 2023 2070 796c 696e  except:  # pylin
+000026d0: 743a 2064 6973 6162 6c65 3d62 6172 652d  t: disable=bare-
+000026e0: 6578 6365 7074 0a20 2020 2020 2020 2020  except.         
+000026f0: 2020 2020 2020 2020 2020 2063 616e 5f6d             can_m
+00002700: 6163 5f6e 6f77 5f70 6c61 7969 6e67 203d  ac_now_playing =
+00002710: 2046 616c 7365 0a0a 2020 2020 2020 2020   False..        
+00002720: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+00002730: 2020 2020 2020 2020 2073 7973 2e70 6c61           sys.pla
+00002740: 7466 6f72 6d20 3d3d 2022 6461 7277 696e  tform == "darwin
+00002750: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00002760: 2020 616e 6420 6361 6e5f 6d61 635f 6e6f    and can_mac_no
+00002770: 775f 706c 6179 696e 670a 2020 2020 2020  w_playing.      
+00002780: 2020 2020 2020 2020 2020 616e 6420 6e6f            and no
+00002790: 7420 6d61 635f 6e6f 775f 706c 6179 696e  t mac_now_playin
+000027a0: 672e 712e 656d 7074 7928 290a 2020 2020  g.q.empty().    
+000027b0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+000027c0: 2020 2020 2020 2020 2020 2063 203d 206d             c = m
+000027d0: 6163 5f6e 6f77 5f70 6c61 7969 6e67 2e71  ac_now_playing.q
+000027e0: 2e67 6574 2829 0a20 2020 2020 2020 2020  .get().         
+000027f0: 2020 2020 2020 2069 6620 6320 696e 2022         if c in "
+00002800: 6e4e 223a 0a20 2020 2020 2020 2020 2020  nN":.           
+00002810: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
+00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002830: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00002840: 7075 742e 6920 3d3d 206c 656e 2870 6c61  put.i == len(pla
+00002850: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
+00002860: 6973 7429 202d 2031 0a20 2020 2020 2020  ist) - 1.       
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2061 6e64 206e 6f74 206c 6f6f 700a 2020   and not loop.  
+00002890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028a0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+000028b0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+000028c0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000028d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000028f0: 2020 2020 6e65 7874 5f73 6f6e 6720 3d20      next_song = 
+00002900: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00002910: 2020 2020 2020 2020 2020 706c 6179 6261            playba
+00002920: 636b 2e73 746f 7028 290a 2020 2020 2020  ck.stop().      
+00002930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002940: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
+00002950: 2020 2020 2020 2020 656c 6966 2063 2069          elif c i
+00002960: 6e20 2262 4222 3a0a 2020 2020 2020 2020  n "bB":.        
+00002970: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+00002980: 6c61 7965 725f 6f75 7470 7574 2e69 203d  layer_output.i =
+00002990: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+000029a0: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+000029b0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000029c0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000029d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029e0: 2020 2020 6e65 7874 5f73 6f6e 6720 3d20      next_song = 
+000029f0: 2d31 0a20 2020 2020 2020 2020 2020 2020  -1.             
+00002a00: 2020 2020 2020 2020 2020 2070 6c61 7962             playb
+00002a10: 6163 6b2e 7374 6f70 2829 0a20 2020 2020  ack.stop().     
+00002a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a30: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00002a40: 2020 2020 2020 2020 2065 6c69 6620 6320           elif c 
+00002a50: 696e 2022 7252 223a 0a20 2020 2020 2020  in "rR":.       
+00002a60: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00002a70: 7962 6163 6b2e 7374 6f70 2829 0a20 2020  yback.stop().   
+00002a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a90: 206e 6578 745f 736f 6e67 203d 2030 0a20   next_song = 0. 
+00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ab0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00002ac0: 2020 2020 2020 2020 2065 6c69 6620 6320           elif c 
+00002ad0: 696e 2022 7151 223a 0a20 2020 2020 2020  in "qQ":.       
+00002ae0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00002af0: 7965 725f 6f75 7470 7574 2e65 6e64 696e  yer_output.endin
+00002b00: 6720 3d20 5472 7565 0a20 2020 2020 2020  g = True.       
+00002b10: 2020 2020 2020 2020 2020 2020 2062 7265               bre
+00002b20: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
+00002b30: 2020 2065 6c69 6620 6320 3d3d 2022 2022     elif c == " "
+00002b40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002b50: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00002b60: 7075 742e 7061 7573 6564 203d 206e 6f74  put.paused = not
+00002b70: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+00002b80: 6175 7365 640a 0a20 2020 2020 2020 2020  aused..         
+00002b90: 2020 2020 2020 2020 2020 2069 6620 706c             if pl
+00002ba0: 6179 6572 5f6f 7574 7075 742e 7061 7573  ayer_output.paus
+00002bb0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
+00002bc0: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00002bd0: 6261 636b 2e70 6175 7365 2829 0a20 2020  back.pause().   
+00002be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002bf0: 2020 2020 2070 6175 7365 5f73 7461 7274       pause_start
+00002c00: 203d 2074 696d 6528 290a 2020 2020 2020   = time().      
+00002c10: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00002c20: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00002c30: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00002c40: 6261 636b 2e72 6573 756d 6528 290a 2020  back.resume().  
+00002c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c60: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
+00002c70: 202b 3d20 7469 6d65 2829 202d 2070 6175   += time() - pau
+00002c80: 7365 5f73 7461 7274 0a0a 2020 2020 2020  se_start..      
+00002c90: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00002ca0: 2073 7973 2e70 6c61 7466 6f72 6d20 3d3d   sys.platform ==
+00002cb0: 2022 6461 7277 696e 2220 616e 6420 6361   "darwin" and ca
+00002cc0: 6e5f 6d61 635f 6e6f 775f 706c 6179 696e  n_mac_now_playin
+00002cd0: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
+00002ce0: 2020 2020 2020 2020 2020 206d 6163 5f6e             mac_n
+00002cf0: 6f77 5f70 6c61 7969 6e67 2e70 6175 7365  ow_playing.pause
+00002d00: 6420 3d20 706c 6179 6572 5f6f 7574 7075  d = player_outpu
+00002d10: 742e 7061 7573 6564 0a20 2020 2020 2020  t.paused.       
+00002d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d30: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
+00002d40: 742e 7061 7573 6564 3a0a 2020 2020 2020  t.paused:.      
+00002d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d60: 2020 2020 2020 6d61 635f 6e6f 775f 706c        mac_now_pl
+00002d70: 6179 696e 672e 7061 7573 6528 290a 2020  aying.pause().  
+00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002d90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00002da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002db0: 2020 2020 2020 2020 6d61 635f 6e6f 775f          mac_now_
+00002dc0: 706c 6179 696e 672e 7265 7375 6d65 2829  playing.resume()
+00002dd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002de0: 2020 2020 2020 2020 2075 7064 6174 655f           update_
+00002df0: 6e6f 775f 706c 6179 696e 6720 3d20 5472  now_playing = Tr
+00002e00: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+00002e10: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+00002e20: 7574 7075 742e 6f75 7470 7574 2870 6c61  utput.output(pla
+00002e30: 7962 6163 6b2e 6375 7272 5f70 6f73 290a  yback.curr_pos).
+00002e40: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00002e50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002e60: 2020 6320 3d20 7374 6473 6372 2e67 6574    c = stdscr.get
+00002e70: 6368 2829 0a20 2020 2020 2020 2020 2020  ch().           
+00002e80: 2020 2020 206e 6578 745f 6320 3d20 7374       next_c = st
+00002e90: 6473 6372 2e67 6574 6368 2829 0a20 2020  dscr.getch().   
+00002ea0: 2020 2020 2020 2020 2020 2020 2077 6869               whi
+00002eb0: 6c65 206e 6578 745f 6320 213d 202d 313a  le next_c != -1:
+00002ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ed0: 2020 2020 2063 2c20 6e65 7874 5f63 203d       c, next_c =
+00002ee0: 206e 6578 745f 632c 2073 7464 7363 722e   next_c, stdscr.
+00002ef0: 6765 7463 6828 290a 0a20 2020 2020 2020  getch()..       
+00002f00: 2020 2020 2020 2020 2069 6620 6320 213d           if c !=
+00002f10: 202d 313a 0a20 2020 2020 2020 2020 2020   -1:.           
+00002f20: 2020 2020 2020 2020 2069 6620 706c 6179           if play
+00002f30: 6572 5f6f 7574 7075 742e 7072 6f6d 7074  er_output.prompt
+00002f40: 696e 6720 6973 204e 6f6e 653a 0a20 2020  ing is None:.   
+00002f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f60: 2020 2020 2069 6620 6320 3d3d 2063 7572       if c == cur
+00002f70: 7365 732e 4b45 595f 4c45 4654 3a0a 2020  ses.KEY_LEFT:.  
+00002f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f90: 2020 2020 2020 2020 2020 706c 6179 6261            playba
+00002fa0: 636b 2e73 6565 6b28 706c 6179 6261 636b  ck.seek(playback
+00002fb0: 2e63 7572 725f 706f 7320 2d20 5343 5255  .curr_pos - SCRU
+00002fc0: 425f 5449 4d45 290a 2020 2020 2020 2020  B_TIME).        
+00002fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002fe0: 2020 2020 6966 2073 7973 2e70 6c61 7466      if sys.platf
+00002ff0: 6f72 6d20 3d3d 2022 6461 7277 696e 2220  orm == "darwin" 
+00003000: 616e 6420 6361 6e5f 6d61 635f 6e6f 775f  and can_mac_now_
+00003010: 706c 6179 696e 673a 0a20 2020 2020 2020  playing:.       
+00003020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003030: 2020 2020 2020 2020 206d 6163 5f6e 6f77           mac_now
+00003040: 5f70 6c61 7969 6e67 2e70 6f73 203d 2072  _playing.pos = r
+00003050: 6f75 6e64 2870 6c61 7962 6163 6b2e 6375  ound(playback.cu
+00003060: 7272 5f70 6f73 290a 2020 2020 2020 2020  rr_pos).        
+00003070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003080: 2020 2020 2020 2020 7570 6461 7465 5f6e          update_n
+00003090: 6f77 5f70 6c61 7969 6e67 203d 2054 7275  ow_playing = Tru
+000030a0: 650a 0a20 2020 2020 2020 2020 2020 2020  e..             
+000030b0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000030c0: 6173 745f 7469 6d65 7374 616d 7020 3d20  ast_timestamp = 
+000030d0: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+000030e0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000030f0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00003100: 6179 6572 5f6f 7574 7075 742e 6f75 7470  ayer_output.outp
+00003110: 7574 2870 6c61 7962 6163 6b2e 6375 7272  ut(playback.curr
+00003120: 5f70 6f73 290a 2020 2020 2020 2020 2020  _pos).          
+00003130: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00003140: 6966 2063 203d 3d20 6375 7273 6573 2e4b  if c == curses.K
+00003150: 4559 5f52 4947 4854 3a0a 2020 2020 2020  EY_RIGHT:.      
+00003160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003170: 2020 2020 2020 706c 6179 6261 636b 2e73        playback.s
+00003180: 6565 6b28 706c 6179 6261 636b 2e63 7572  eek(playback.cur
+00003190: 725f 706f 7320 2b20 5343 5255 425f 5449  r_pos + SCRUB_TI
+000031a0: 4d45 290a 2020 2020 2020 2020 2020 2020  ME).            
+000031b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000031c0: 6966 2073 7973 2e70 6c61 7466 6f72 6d20  if sys.platform 
+000031d0: 3d3d 2022 6461 7277 696e 2220 616e 6420  == "darwin" and 
+000031e0: 6361 6e5f 6d61 635f 6e6f 775f 706c 6179  can_mac_now_play
+000031f0: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003210: 2020 2020 206d 6163 5f6e 6f77 5f70 6c61       mac_now_pla
+00003220: 7969 6e67 2e70 6f73 203d 2072 6f75 6e64  ying.pos = round
+00003230: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
+00003240: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
+00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003260: 2020 2020 7570 6461 7465 5f6e 6f77 5f70      update_now_p
+00003270: 6c61 7969 6e67 203d 2054 7275 650a 0a20  laying = True.. 
+00003280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003290: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+000032a0: 7469 6d65 7374 616d 7020 3d20 706c 6179  timestamp = play
+000032b0: 6261 636b 2e63 7572 725f 706f 730a 2020  back.curr_pos.  
+000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000032d0: 2020 2020 2020 2020 2020 706c 6179 6572            player
+000032e0: 5f6f 7574 7075 742e 6f75 7470 7574 2870  _output.output(p
+000032f0: 6c61 7962 6163 6b2e 6375 7272 5f70 6f73  layback.curr_pos
+00003300: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00003310: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
+00003320: 203d 3d20 6375 7273 6573 2e4b 4559 5f55   == curses.KEY_U
+00003330: 503a 0a20 2020 2020 2020 2020 2020 2020  P:.             
+00003340: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003350: 6c61 7965 725f 6f75 7470 7574 2e73 6372  layer_output.scr
+00003360: 6f6c 6c65 722e 7363 726f 6c6c 5f62 6163  oller.scroll_bac
+00003370: 6b77 6172 6428 290a 2020 2020 2020 2020  kward().        
+00003380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003390: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+000033a0: 742e 6f75 7470 7574 2870 6c61 7962 6163  t.output(playbac
+000033b0: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
+000033c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000033d0: 2020 2020 656c 6966 2063 203d 3d20 6375      elif c == cu
+000033e0: 7273 6573 2e4b 4559 5f44 4f57 4e3a 0a20  rses.KEY_DOWN:. 
+000033f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003400: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+00003410: 725f 6f75 7470 7574 2e73 6372 6f6c 6c65  r_output.scrolle
+00003420: 722e 7363 726f 6c6c 5f66 6f72 7761 7264  r.scroll_forward
+00003430: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00003440: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003450: 6c61 7965 725f 6f75 7470 7574 2e6f 7574  layer_output.out
+00003460: 7075 7428 706c 6179 6261 636b 2e63 7572  put(playback.cur
+00003470: 725f 706f 7329 0a20 2020 2020 2020 2020  r_pos).         
+00003480: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00003490: 6c69 6620 6320 3d3d 2063 7572 7365 732e  lif c == curses.
+000034a0: 4b45 595f 454e 5445 523a 0a20 2020 2020  KEY_ENTER:.     
 000034b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034c0: 2020 2020 2021 3d20 706c 6179 6572 5f6f       != player_o
-000034d0: 7574 7075 742e 7363 726f 6c6c 6572 2e6e  utput.scroller.n
-000034e0: 756d 5f6c 696e 6573 202d 2031 0a20 2020  um_lines - 1.   
-000034f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003500: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
-00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003520: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00003530: 6572 5f6f 7574 7075 742e 7363 726f 6c6c  er_output.scroll
-00003540: 6572 2e73 6372 6f6c 6c5f 666f 7277 6172  er.scroll_forwar
-00003550: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
-00003560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003570: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00003580: 742e 6f75 7470 7574 2870 6c61 7962 6163  t.output(playbac
-00003590: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
-000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035b0: 2020 2020 656c 6966 2063 203d 3d20 6375      elif c == cu
-000035c0: 7273 6573 2e4b 4559 5f45 4e54 4552 3a0a  rses.KEY_ENTER:.
-000035d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035e0: 2020 2020 2020 2020 2020 2020 706c 6179              play
-000035f0: 6572 5f6f 7574 7075 742e 6920 3d20 706c  er_output.i = pl
-00003600: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
-00003610: 6c6c 6572 2e70 6f73 202d 2031 0a20 2020  ller.pos - 1.   
-00003620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003630: 2020 2020 2020 2020 206e 6578 745f 736f           next_so
-00003640: 6e67 203d 2031 0a20 2020 2020 2020 2020  ng = 1.         
-00003650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003660: 2020 2070 6c61 7962 6163 6b2e 7374 6f70     playback.stop
-00003670: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00003680: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00003690: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-000036a0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-000036b0: 6620 6320 3d3d 2063 7572 7365 732e 4b45  f c == curses.KE
-000036c0: 595f 4443 3a0a 2020 2020 2020 2020 2020  Y_DC:.          
+000034c0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+000034d0: 7470 7574 2e69 203d 2070 6c61 7965 725f  tput.i = player_
+000034e0: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
+000034f0: 706f 7320 2d20 310a 2020 2020 2020 2020  pos - 1.        
+00003500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003510: 2020 2020 6e65 7874 5f73 6f6e 6720 3d20      next_song = 
+00003520: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00003530: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00003540: 6179 6261 636b 2e73 746f 7028 290a 2020  ayback.stop().  
+00003550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003560: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00003570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003580: 2020 2020 2020 2020 656c 6966 2063 203d          elif c =
+00003590: 3d20 6375 7273 6573 2e4b 4559 5f44 433a  = curses.KEY_DC:
+000035a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000035b0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+000035c0: 6563 7465 645f 736f 6e67 203d 2070 6c61  ected_song = pla
+000035d0: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
+000035e0: 6c65 722e 706f 730a 2020 2020 2020 2020  ler.pos.        
+000035f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003600: 2020 2020 6465 6c20 706c 6179 6572 5f6f      del player_o
+00003610: 7574 7075 742e 706c 6179 6c69 7374 5b73  utput.playlist[s
+00003620: 656c 6563 7465 645f 736f 6e67 5d0a 0a20  elected_song].. 
+00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003640: 2020 2020 2020 2020 2020 2069 6620 6c6f             if lo
+00003650: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
+00003660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003670: 2020 2020 6966 2072 6573 6875 6666 6c65      if reshuffle
+00003680: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036a0: 2020 2020 2020 6e65 7874 5f70 6c61 796c        next_playl
+000036b0: 6973 7420 3d20 706c 6179 6c69 7374 5b3a  ist = playlist[:
+000036c0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
 000036d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000036e0: 2020 7365 6c65 6374 6564 5f73 6f6e 6720    selected_song 
-000036f0: 3d20 706c 6179 6572 5f6f 7574 7075 742e  = player_output.
-00003700: 7363 726f 6c6c 6572 2e70 6f73 0a20 2020  scroller.pos.   
-00003710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003720: 2020 2020 2020 2020 2064 656c 2070 6c61           del pla
-00003730: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
-00003740: 6973 745b 7365 6c65 6374 6564 5f73 6f6e  ist[selected_son
-00003750: 675d 0a0a 2020 2020 2020 2020 2020 2020  g]..            
-00003760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003770: 6966 206c 6f6f 703a 0a20 2020 2020 2020  if loop:.       
-00003780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003790: 2020 2020 2020 2020 2069 6620 7265 7368           if resh
-000037a0: 7566 666c 653a 0a20 2020 2020 2020 2020  uffle:.         
+000036e0: 2020 2020 2020 7368 7566 666c 6528 6e65        shuffle(ne
+000036f0: 7874 5f70 6c61 796c 6973 7429 0a20 2020  xt_playlist).   
+00003700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003710: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00003720: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00003730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003740: 2020 2020 2020 2064 656c 206e 6578 745f         del next_
+00003750: 706c 6179 6c69 7374 5b73 656c 6563 7465  playlist[selecte
+00003760: 645f 736f 6e67 5d0a 0a20 2020 2020 2020  d_song]..       
+00003770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003780: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+00003790: 7574 2e73 6372 6f6c 6c65 722e 6e75 6d5f  ut.scroller.num_
+000037a0: 6c69 6e65 7320 2d3d 2031 0a20 2020 2020  lines -= 1.     
 000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037c0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-000037d0: 706c 6179 6c69 7374 203d 2070 6c61 796c  playlist = playl
-000037e0: 6973 745b 3a5d 0a20 2020 2020 2020 2020  ist[:].         
-000037f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003800: 2020 2020 2020 2020 2020 2073 6875 6666             shuff
-00003810: 6c65 286e 6578 745f 706c 6179 6c69 7374  le(next_playlist
-00003820: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00003830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003840: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000037c0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
+000037d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000037e0: 2020 2020 2020 2020 2020 2020 7365 6c65              sele
+000037f0: 6374 6564 5f73 6f6e 6720 3d3d 2070 6c61  cted_song == pla
+00003800: 7965 725f 6f75 7470 7574 2e69 0a20 2020  yer_output.i.   
+00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003820: 2020 2020 2020 2020 2029 3a20 2023 2064           ):  # d
+00003830: 656c 6574 6564 2063 7572 7265 6e74 2073  eleted current s
+00003840: 6f6e 670a 2020 2020 2020 2020 2020 2020  ong.            
 00003850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003860: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-00003870: 6e65 7874 5f70 6c61 796c 6973 745b 7365  next_playlist[se
-00003880: 6c65 6374 6564 5f73 6f6e 675d 0a0a 2020  lected_song]..  
-00003890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038a0: 2020 2020 2020 2020 2020 706c 6179 6572            player
-000038b0: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
-000038c0: 2e6e 756d 5f6c 696e 6573 202d 3d20 310a  .num_lines -= 1.
-000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000038e0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-000038f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003860: 2020 2020 6e65 7874 5f73 6f6e 6720 3d20      next_song = 
+00003870: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
+00003880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003890: 2020 2320 7769 6c6c 2062 6520 696e 6372    # will be incr
+000038a0: 656d 656e 7465 6420 746f 2069 0a20 2020  emented to i.   
+000038b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038c0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+000038d0: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
+000038e0: 6c65 722e 706f 7320 3d20 706c 6179 6572  ler.pos = player
+000038f0: 5f6f 7574 7075 742e 6920 2d20 310a 2020  _output.i - 1.  
 00003900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003910: 2073 656c 6563 7465 645f 736f 6e67 203d   selected_song =
-00003920: 3d20 706c 6179 6572 5f6f 7574 7075 742e  = player_output.
-00003930: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
-00003940: 2020 2020 2020 2020 2020 2020 2020 293a                ):
-00003950: 2020 2320 6465 6c65 7465 6420 6375 7272    # deleted curr
-00003960: 656e 7420 736f 6e67 0a20 2020 2020 2020  ent song.       
+00003910: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00003920: 6179 6572 5f6f 7574 7075 742e 6920 2d3d  ayer_output.i -=
+00003930: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+00003940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003950: 2020 2070 6c61 7962 6163 6b2e 7374 6f70     playback.stop
+00003960: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
 00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003980: 2020 2020 2020 2020 206e 6578 745f 736f           next_so
-00003990: 6e67 203d 2031 0a20 2020 2020 2020 2020  ng = 1.         
-000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039b0: 2020 2020 2020 2023 2077 696c 6c20 6265         # will be
-000039c0: 2069 6e63 7265 6d65 6e74 6564 2074 6f20   incremented to 
-000039d0: 690a 2020 2020 2020 2020 2020 2020 2020  i.              
-000039e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000039f0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00003a00: 7363 726f 6c6c 6572 2e70 6f73 203d 2070  scroller.pos = p
-00003a10: 6c61 7965 725f 6f75 7470 7574 2e69 202d  layer_output.i -
-00003a20: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
-00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a40: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00003a50: 2e69 202d 3d20 310a 2020 2020 2020 2020  .i -= 1.        
+00003980: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00003990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039a0: 2020 2020 2023 2064 656c 6574 6564 2073       # deleted s
+000039b0: 6f6e 6720 6265 666f 7265 2063 7572 7265  ong before curre
+000039c0: 6e74 0a20 2020 2020 2020 2020 2020 2020  nt.             
+000039d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000039e0: 6620 7365 6c65 6374 6564 5f73 6f6e 6720  f selected_song 
+000039f0: 3c20 706c 6179 6572 5f6f 7574 7075 742e  < player_output.
+00003a00: 693a 0a20 2020 2020 2020 2020 2020 2020  i:.             
+00003a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a20: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00003a30: 2e69 202d 3d20 310a 2020 2020 2020 2020  .i -= 1.        
+00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
 00003a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a70: 2020 2020 2020 2020 706c 6179 6261 636b          playback
-00003a80: 2e73 746f 7028 290a 2020 2020 2020 2020  .stop().        
-00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003aa0: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
+00003a70: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a90: 2020 2020 2020 2063 203d 2063 6872 2863         c = chr(c
+00003aa0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
 00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ac0: 2020 2020 2020 2020 2020 2320 6465 6c65            # dele
-00003ad0: 7465 6420 736f 6e67 2062 6566 6f72 6520  ted song before 
-00003ae0: 6375 7272 656e 740a 2020 2020 2020 2020  current.        
-00003af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b00: 2020 2020 6966 2073 656c 6563 7465 645f      if selected_
-00003b10: 736f 6e67 203c 2070 6c61 7965 725f 6f75  song < player_ou
-00003b20: 7470 7574 2e69 3a0a 2020 2020 2020 2020  tput.i:.        
-00003b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b40: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00003b50: 7574 7075 742e 6920 2d3d 2031 0a20 2020  utput.i -= 1.   
-00003b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b70: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00003ac0: 2020 6966 2063 2069 6e20 226e 4e22 3a0a    if c in "nN":.
+00003ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003af0: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2070 6c61 7965 725f 6f75 7470 7574 2e69   player_output.i
+00003b30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b50: 2020 2020 2020 2020 203d 3d20 6c65 6e28           == len(
+00003b60: 706c 6179 6572 5f6f 7574 7075 742e 706c  player_output.pl
+00003b70: 6179 6c69 7374 2920 2d20 310a 2020 2020  aylist) - 1.    
 00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003b90: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
-00003ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003bb0: 2020 2020 2020 2020 2020 2020 6320 3d20              c = 
-00003bc0: 6368 7228 6329 0a20 2020 2020 2020 2020  chr(c).         
-00003bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003be0: 2020 2020 2020 2069 6620 6320 696e 2022         if c in "
-00003bf0: 6e4e 7353 223a 0a20 2020 2020 2020 2020  nNsS":.         
-00003c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c10: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
-00003c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ba0: 2020 2020 616e 6420 6e6f 7420 6c6f 6f70      and not loop
+00003bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bd0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
+00003be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c00: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+00003c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c20: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 00003c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c40: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00003c50: 7574 7075 742e 690a 2020 2020 2020 2020  utput.i.        
-00003c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c50: 2020 2020 2020 206e 6578 745f 736f 6e67         next_song
+00003c60: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
 00003c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003c80: 3d3d 206c 656e 2870 6c61 7965 725f 6f75  == len(player_ou
-00003c90: 7470 7574 2e70 6c61 796c 6973 7429 202d  tput.playlist) -
-00003ca0: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+00003c80: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00003c90: 7962 6163 6b2e 7374 6f70 2829 0a20 2020  yback.stop().   
+00003ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cc0: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
-00003cd0: 6f74 206c 6f6f 700a 2020 2020 2020 2020  ot loop.        
-00003ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003cf0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
+00003cc0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
+00003cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ce0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00003cf0: 6320 696e 2022 6242 223a 0a20 2020 2020  c in "bB":.     
 00003d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d20: 2020 2020 2020 2070 6173 730a 2020 2020         pass.    
-00003d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00003d20: 6620 706c 6179 6572 5f6f 7574 7075 742e  f player_output.
+00003d30: 6920 3d3d 2030 3a0a 2020 2020 2020 2020  i == 0:.        
 00003d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00003d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003d70: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-00003d80: 7874 5f73 6f6e 6720 3d20 310a 2020 2020  xt_song = 1.    
+00003d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d60: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+00003d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003d80: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 00003d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003db0: 2020 2020 706c 6179 6261 636b 2e73 746f      playback.sto
-00003dc0: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
+00003db0: 2020 2020 2020 206e 6578 745f 736f 6e67         next_song
+00003dc0: 203d 202d 310a 2020 2020 2020 2020 2020   = -1.          
 00003dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003de0: 2020 2020 2020 2020 2020 2020 6272 6561              brea
-00003df0: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+00003de0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00003df0: 6179 6261 636b 2e73 746f 7028 290a 2020  ayback.stop().  
 00003e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e10: 2020 656c 6966 2063 2069 6e20 2262 4270    elif c in "bBp
-00003e20: 5022 3a0a 2020 2020 2020 2020 2020 2020  P":.            
+00003e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e20: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
 00003e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e40: 2020 2020 2020 2020 6966 2070 6c61 7965          if playe
-00003e50: 725f 6f75 7470 7574 2e69 203d 3d20 303a  r_output.i == 0:
-00003e60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003e40: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00003e50: 2063 2069 6e20 2272 5222 3a0a 2020 2020   c in "rR":.    
+00003e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003e80: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+00003e80: 706c 6179 6261 636b 2e73 746f 7028 290a  playback.stop().
 00003e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003eb0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00003ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003eb0: 2020 2020 6e65 7874 5f73 6f6e 6720 3d20      next_song = 
+00003ec0: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
 00003ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003ee0: 6e65 7874 5f73 6f6e 6720 3d20 2d31 0a20  next_song = -1. 
+00003ee0: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
 00003ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f10: 2020 2020 2020 2070 6c61 7962 6163 6b2e         playback.
-00003f20: 7374 6f70 2829 0a20 2020 2020 2020 2020  stop().         
+00003f00: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00003f10: 2063 2069 6e20 226c 4c22 3a0a 2020 2020   c in "lL":.    
+00003f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00003f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f40: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00003f50: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-00003f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003f70: 2020 2020 2065 6c69 6620 6320 696e 2022       elif c in "
-00003f80: 7252 223a 0a20 2020 2020 2020 2020 2020  rR":.           
-00003f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fa0: 2020 2020 2020 2020 2070 6c61 7962 6163           playbac
-00003fb0: 6b2e 7374 6f70 2829 0a20 2020 2020 2020  k.stop().       
+00003f40: 706c 6179 6572 5f6f 7574 7075 742e 6c6f  player_output.lo
+00003f50: 6f70 696e 675f 6375 7272 656e 745f 736f  oping_current_so
+00003f60: 6e67 203d 2028 0a20 2020 2020 2020 2020  ng = (.         
+00003f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003f80: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003f90: 6c61 7965 725f 6f75 7470 7574 2e6c 6f6f  layer_output.loo
+00003fa0: 7069 6e67 5f63 7572 7265 6e74 5f73 6f6e  ping_current_son
+00003fb0: 6720 2b20 310a 2020 2020 2020 2020 2020  g + 1.          
 00003fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003fd0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-00003fe0: 745f 736f 6e67 203d 2030 0a20 2020 2020  t_song = 0.     
+00003fd0: 2020 2020 2020 2020 2020 2920 2520 6c65            ) % le
+00003fe0: 6e28 4c4f 4f50 5f4d 4f44 4553 290a 2020  n(LOOP_MODES).  
 00003ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004000: 2020 2020 2020 2020 2020 2020 2020 2062                 b
-00004010: 7265 616b 0a20 2020 2020 2020 2020 2020  reak.           
-00004020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004030: 2020 2020 2065 6c69 6620 6320 696e 2022       elif c in "
-00004040: 6c4c 223a 0a20 2020 2020 2020 2020 2020  lL":.           
-00004050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004060: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00004070: 6f75 7470 7574 2e6c 6f6f 7069 6e67 5f63  output.looping_c
-00004080: 7572 7265 6e74 5f73 6f6e 6720 3d20 280a  urrent_song = (.
-00004090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000040b0: 2020 2020 2020 2020 6e6f 7420 706c 6179          not play
-000040c0: 6572 5f6f 7574 7075 742e 6c6f 6f70 696e  er_output.loopin
-000040d0: 675f 6375 7272 656e 745f 736f 6e67 0a20  g_current_song. 
-000040e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004010: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+00004020: 6f75 7470 7574 2870 6c61 7962 6163 6b2e  output(playback.
+00004030: 6375 7272 5f70 6f73 290a 2020 2020 2020  curr_pos).      
+00004040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004050: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
+00004060: 2069 6e20 2263 4322 3a0a 2020 2020 2020   in "cC":.      
+00004070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004080: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00004090: 6179 6572 5f6f 7574 7075 742e 636c 6970  ayer_output.clip
+000040a0: 5f6d 6f64 6520 3d20 280a 2020 2020 2020  _mode = (.      
+000040b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000040d0: 2020 6e6f 7420 706c 6179 6572 5f6f 7574    not player_out
+000040e0: 7075 742e 636c 6970 5f6d 6f64 650a 2020  put.clip_mode.  
 000040f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004100: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004120: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00004130: 6f75 7470 7574 2e6f 7574 7075 7428 706c  output.output(pl
-00004140: 6179 6261 636b 2e63 7572 725f 706f 7329  ayback.curr_pos)
-00004150: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004110: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00004120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004130: 2020 2020 2020 2020 6966 2070 6c61 7965          if playe
+00004140: 725f 6f75 7470 7574 2e63 6c69 705f 6d6f  r_output.clip_mo
+00004150: 6465 3a0a 2020 2020 2020 2020 2020 2020  de:.            
 00004160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004170: 2065 6c69 6620 6320 696e 2022 6343 223a   elif c in "cC":
-00004180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004170: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
+00004180: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041a0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-000041b0: 7574 2e63 6c69 705f 6d6f 6465 203d 2028  ut.clip_mode = (
-000041c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000041a0: 2020 2020 2020 2020 2020 636c 6970 5f73            clip_s
+000041b0: 7461 7274 2c0a 2020 2020 2020 2020 2020  tart,.          
+000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000041d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041e0: 2020 2020 2020 2020 206e 6f74 2070 6c61           not pla
-000041f0: 7965 725f 6f75 7470 7574 2e63 6c69 705f  yer_output.clip_
-00004200: 6d6f 6465 0a20 2020 2020 2020 2020 2020  mode.           
-00004210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004220: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000041e0: 2020 636c 6970 5f65 6e64 2c0a 2020 2020    clip_end,.    
+000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004210: 2020 2020 2920 3d20 706c 6179 6572 5f6f      ) = player_o
+00004220: 7574 7075 742e 636c 6970 0a20 2020 2020  utput.clip.     
 00004230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004240: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00004250: 6620 706c 6179 6572 5f6f 7574 7075 742e  f player_output.
-00004260: 636c 6970 5f6d 6f64 653a 0a20 2020 2020  clip_mode:.     
+00004240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004250: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00004260: 2e64 7572 6174 696f 6e20 3d20 280a 2020  .duration = (.  
 00004270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004290: 2020 2028 0a20 2020 2020 2020 2020 2020     (.           
-000042a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004290: 2020 2020 2020 2020 2020 636c 6970 5f65            clip_e
+000042a0: 6e64 202d 2063 6c69 705f 7374 6172 740a  nd - clip_start.
 000042b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042c0: 2063 6c69 705f 7374 6172 742c 0a20 2020   clip_start,.   
-000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
 000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042f0: 2020 2020 2020 2020 2063 6c69 705f 656e           clip_en
-00004300: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
+000042f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004300: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
 00004310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004320: 2020 2020 2020 2020 2020 2029 203d 2070             ) = p
-00004330: 6c61 7965 725f 6f75 7470 7574 2e63 6c69  layer_output.cli
-00004340: 700a 2020 2020 2020 2020 2020 2020 2020  p.              
-00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004360: 2020 2020 2020 2020 2020 706c 6179 6572            player
-00004370: 5f6f 7574 7075 742e 6475 7261 7469 6f6e  _output.duration
-00004380: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00004390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004330: 2020 2070 6c61 7962 6163 6b2e 6375 7272     playback.curr
+00004340: 5f70 6f73 203c 2063 6c69 705f 7374 6172  _pos < clip_star
+00004350: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004370: 2020 2020 2020 2020 2020 2020 2020 6f72                or
+00004380: 2070 6c61 7962 6163 6b2e 6375 7272 5f70   playback.curr_p
+00004390: 6f73 203e 2063 6c69 705f 656e 640a 2020  os > clip_end.  
 000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043b0: 2063 6c69 705f 656e 6420 2d20 636c 6970   clip_end - clip
-000043c0: 5f73 7461 7274 0a20 2020 2020 2020 2020  _start.         
+000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043c0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
 000043d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000043f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004410: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
+000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043f0: 2020 2020 2070 6c61 7962 6163 6b2e 7365       playback.se
+00004400: 656b 2863 6c69 705f 7374 6172 7429 0a20  ek(clip_start). 
+00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004440: 2020 2020 2020 2020 2020 706c 6179 6261            playba
-00004450: 636b 2e63 7572 725f 706f 7320 3c20 636c  ck.curr_pos < cl
-00004460: 6970 5f73 7461 7274 0a20 2020 2020 2020  ip_start.       
-00004470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004490: 2020 2020 206f 7220 706c 6179 6261 636b       or playback
-000044a0: 2e63 7572 725f 706f 7320 3e20 636c 6970  .curr_pos > clip
-000044b0: 5f65 6e64 0a20 2020 2020 2020 2020 2020  _end.           
-000044c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044d0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
+00004430: 2020 2020 2020 2020 2020 2069 6620 280a             if (.
+00004440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 7379 732e 706c 6174 666f 726d 203d 3d20  sys.platform == 
+00004480: 2264 6172 7769 6e22 0a20 2020 2020 2020  "darwin".       
+00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000044b0: 2020 2020 2020 2020 2061 6e64 2063 616e           and can
+000044c0: 5f6d 6163 5f6e 6f77 5f70 6c61 7969 6e67  _mac_now_playing
+000044d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000044e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004500: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00004510: 6261 636b 2e73 6565 6b28 636c 6970 5f73  back.seek(clip_s
-00004520: 7461 7274 290a 2020 2020 2020 2020 2020  tart).          
-00004530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004550: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
+000044f0: 2020 2020 2020 2020 2020 2020 2029 3a0a               ):.
+00004500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004530: 6d61 635f 6e6f 775f 706c 6179 696e 672e  mac_now_playing.
+00004540: 706f 7320 3d20 726f 756e 6428 0a20 2020  pos = round(.   
+00004550: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004580: 2020 2020 2020 2073 7973 2e70 6c61 7466         sys.platf
-00004590: 6f72 6d20 3d3d 2022 6461 7277 696e 220a  orm == "darwin".
+00004580: 2070 6c61 7962 6163 6b2e 6375 7272 5f70   playback.curr_p
+00004590: 6f73 0a20 2020 2020 2020 2020 2020 2020  os.             
 000045a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000045b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045d0: 616e 6420 6361 6e5f 6d61 635f 6e6f 775f  and can_mac_now_
-000045e0: 706c 6179 696e 670a 2020 2020 2020 2020  playing.        
-000045f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004610: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+000045c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000045d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000045f0: 2020 2020 2075 7064 6174 655f 6e6f 775f       update_now_
+00004600: 706c 6179 696e 6720 3d20 5472 7565 0a20  playing = True. 
+00004610: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004640: 2020 2020 2020 206d 6163 5f6e 6f77 5f70         mac_now_p
-00004650: 6c61 7969 6e67 2e70 6f73 203d 2072 6f75  laying.pos = rou
-00004660: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
+00004630: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+00004640: 7469 6d65 7374 616d 7020 3d20 706c 6179  timestamp = play
+00004650: 6261 636b 2e63 7572 725f 706f 730a 2020  back.curr_pos.  
+00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004690: 2020 2020 2020 2020 706c 6179 6261 636b          playback
-000046a0: 2e63 7572 725f 706f 730a 2020 2020 2020  .curr_pos.      
-000046b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046d0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00004680: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046b0: 706c 6179 6572 5f6f 7574 7075 742e 6475  player_output.du
+000046c0: 7261 7469 6f6e 203d 2066 756c 6c5f 6475  ration = full_du
+000046d0: 7261 7469 6f6e 0a20 2020 2020 2020 2020  ration.         
 000046e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000046f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004700: 2020 2020 2020 2020 2020 2020 7570 6461              upda
-00004710: 7465 5f6e 6f77 5f70 6c61 7969 6e67 203d  te_now_playing =
-00004720: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+000046f0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+00004700: 725f 6f75 7470 7574 2e6f 7574 7075 7428  r_output.output(
+00004710: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+00004720: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
 00004730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004750: 2020 6c61 7374 5f74 696d 6573 7461 6d70    last_timestamp
-00004760: 203d 2070 6c61 7962 6163 6b2e 6375 7272   = playback.curr
-00004770: 5f70 6f73 0a20 2020 2020 2020 2020 2020  _pos.           
-00004780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004790: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-000047a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004740: 2020 2065 6c69 6620 6320 696e 2022 7050     elif c in "pP
+00004750: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00004760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004770: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00004780: 7470 7574 2e73 6372 6f6c 6c65 722e 706f  tput.scroller.po
+00004790: 7320 3d20 706c 6179 6572 5f6f 7574 7075  s = player_outpu
+000047a0: 742e 690a 2020 2020 2020 2020 2020 2020  t.i.            
 000047b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000047c0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-000047d0: 7470 7574 2e64 7572 6174 696f 6e20 3d20  tput.duration = 
-000047e0: 6675 6c6c 5f64 7572 6174 696f 6e0a 2020  full_duration.  
+000047c0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+000047d0: 7574 7075 742e 7363 726f 6c6c 6572 2e72  utput.scroller.r
+000047e0: 6573 697a 6528 290a 2020 2020 2020 2020  esize().        
 000047f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004810: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00004820: 6f75 7470 7574 2870 6c61 7962 6163 6b2e  output(playback.
-00004830: 6375 7272 5f70 6f73 290a 2020 2020 2020  curr_pos).      
+00004800: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00004810: 6572 5f6f 7574 7075 742e 6f75 7470 7574  er_output.output
+00004820: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
+00004830: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
 00004840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004850: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
-00004860: 2069 6e20 2265 4522 3a0a 2020 2020 2020   in "eE":.      
+00004850: 2020 2020 656c 6966 2063 2069 6e20 2267      elif c in "g
+00004860: 4722 3a0a 2020 2020 2020 2020 2020 2020  G":.            
 00004870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004880: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00004890: 6179 6572 5f6f 7574 7075 742e 656e 6469  ayer_output.endi
-000048a0: 6e67 203d 2028 0a20 2020 2020 2020 2020  ng = (.         
-000048b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048c0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000048d0: 6f74 2070 6c61 7965 725f 6f75 7470 7574  ot player_output
-000048e0: 2e65 6e64 696e 670a 2020 2020 2020 2020  .ending.        
-000048f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004900: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00004880: 2020 2020 2020 2020 6966 206c 6f6f 703a          if loop:
+00004890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000048a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048b0: 2020 2020 2020 2020 2070 6c61 7962 6163           playbac
+000048c0: 6b2e 7374 6f70 2829 0a20 2020 2020 2020  k.stop().       
+000048d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000048f0: 2070 6c61 7965 725f 6f75 7470 7574 2e69   player_output.i
+00004900: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
 00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004930: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00004940: 6f75 7470 7574 2870 6c61 7962 6163 6b2e  output(playback.
-00004950: 6375 7272 5f70 6f73 290a 2020 2020 2020  curr_pos).      
+00004930: 206c 656e 2870 6c61 7965 725f 6f75 7470   len(player_outp
+00004940: 7574 2e70 6c61 796c 6973 7429 202d 2031  ut.playlist) - 1
+00004950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00004960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004970: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
-00004980: 2069 6e20 2271 5122 3a0a 2020 2020 2020   in "qQ":.      
+00004970: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049a0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-000049b0: 6179 6572 5f6f 7574 7075 742e 656e 6469  ayer_output.endi
-000049c0: 6e67 203d 2054 7275 650a 2020 2020 2020  ng = True.      
-000049d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049e0: 2020 2020 2020 2020 2020 2020 2020 6272                br
-000049f0: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
-00004a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a10: 2020 2020 656c 6966 2063 2069 6e20 2264      elif c in "d
-00004a20: 4422 3a0a 2020 2020 2020 2020 2020 2020  D":.            
-00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a40: 2020 2020 2020 2020 6966 2070 6c61 7965          if playe
-00004a50: 725f 6f75 7470 7574 2e75 7064 6174 655f  r_output.update_
-00004a60: 6469 7363 6f72 643a 0a20 2020 2020 2020  discord:.       
-00004a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 2070 6c61 7965 725f 6f75 7470 7574 2e75   player_output.u
-00004aa0: 7064 6174 655f 6469 7363 6f72 6420 3d20  pdate_discord = 
-00004ab0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+000049a0: 2020 206e 6578 745f 736f 6e67 203d 2031     next_song = 1
+000049b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000049c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049d0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+000049e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049f0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00004a00: 6c69 6620 6320 696e 2022 6545 223a 0a20  lif c in "eE":. 
+00004a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a30: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00004a40: 2e65 6e64 696e 6720 3d20 280a 2020 2020  .ending = (.    
+00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a70: 2020 2020 6e6f 7420 706c 6179 6572 5f6f      not player_o
+00004a80: 7574 7075 742e 656e 6469 6e67 0a20 2020  utput.ending.   
+00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ab0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
 00004ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ad0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00004ae0: 7363 6f72 645f 7072 6573 656e 6365 5f70  scord_presence_p
-00004af0: 726f 6365 7373 2e74 6572 6d69 6e61 7465  rocess.terminate
-00004b00: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-00004b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b20: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00004ad0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00004ae0: 7470 7574 2e6f 7574 7075 7428 706c 6179  tput.output(play
+00004af0: 6261 636b 2e63 7572 725f 706f 7329 0a20  back.curr_pos). 
+00004b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b10: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00004b20: 6c69 6620 6320 696e 2022 7151 223a 0a20  lif c in "qQ":. 
 00004b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b50: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00004b60: 7574 2e75 7064 6174 655f 6469 7363 6f72  ut.update_discor
-00004b70: 6420 3d20 5472 7565 0a0a 2020 2020 2020  d = True..      
+00004b50: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00004b60: 2e65 6e64 696e 6720 3d20 5472 7565 0a20  .ending = True. 
+00004b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ba0: 2020 6469 7363 6f72 645f 736f 6e67 5f6e    discord_song_n
-00004bb0: 616d 655f 7175 6575 6520 3d20 280a 2020  ame_queue = (.  
-00004bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004b90: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00004ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bb0: 2020 2020 2020 2020 2065 6c69 6620 6320           elif c 
+00004bc0: 696e 2022 6444 223a 0a20 2020 2020 2020  in "dD":.       
 00004bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004be0: 2020 2020 2020 2020 2020 6d75 6c74 6970            multip
-00004bf0: 726f 6365 7373 696e 672e 5369 6d70 6c65  rocessing.Simple
-00004c00: 5175 6575 6528 290a 2020 2020 2020 2020  Queue().        
+00004be0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004bf0: 706c 6179 6572 5f6f 7574 7075 742e 7570  player_output.up
+00004c00: 6461 7465 5f64 6973 636f 7264 3a0a 2020  date_discord:.  
 00004c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c50: 2020 2020 2020 2020 2020 666f 7220 6320            for c 
-00004c60: 696e 2070 6c61 7965 725f 6f75 7470 7574  in player_output
-00004c70: 2e70 6c61 796c 6973 745b 0a20 2020 2020  .playlist[.     
-00004c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ca0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-00004cb0: 7470 7574 2e69 0a20 2020 2020 2020 2020  tput.i.         
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
-00004ce0: 5b31 5d3a 0a20 2020 2020 2020 2020 2020  [1]:.           
-00004cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d10: 2064 6973 636f 7264 5f73 6f6e 675f 6e61   discord_song_na
-00004d20: 6d65 5f71 7565 7565 2e70 7574 2863 290a  me_queue.put(c).
+00004c30: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00004c40: 7075 742e 7570 6461 7465 5f64 6973 636f  put.update_disco
+00004c50: 7264 203d 2046 616c 7365 0a20 2020 2020  rd = False.     
+00004c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c80: 2020 2064 6973 636f 7264 5f70 7265 7365     discord_prese
+00004c90: 6e63 655f 7072 6f63 6573 732e 7465 726d  nce_process.term
+00004ca0: 696e 6174 6528 290a 2020 2020 2020 2020  inate().        
+00004cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cc0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00004cd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cf0: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00004d00: 5f6f 7574 7075 742e 7570 6461 7465 5f64  _output.update_d
+00004d10: 6973 636f 7264 203d 2054 7275 650a 0a20  iscord = True.. 
+00004d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d50: 2020 2020 2020 2020 6469 7363 6f72 645f          discord_
-00004d60: 736f 6e67 5f6e 616d 655f 7175 6575 652e  song_name_queue.
-00004d70: 7075 7428 225c 6e22 290a 0a20 2020 2020  put("\n")..     
-00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004da0: 2020 2064 6973 636f 7264 5f61 7274 6973     discord_artis
-00004db0: 745f 7175 6575 6520 3d20 280a 2020 2020  t_queue = (.    
+00004d40: 2020 2020 2020 2064 6973 636f 7264 5f73         discord_s
+00004d50: 6f6e 675f 6e61 6d65 5f71 7565 7565 203d  ong_name_queue =
+00004d60: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00004d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d80: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00004d90: 756c 7469 7072 6f63 6573 7369 6e67 2e53  ultiprocessing.S
+00004da0: 696d 706c 6551 7565 7565 2829 0a20 2020  impleQueue().   
+00004db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004de0: 2020 2020 2020 2020 6d75 6c74 6970 726f          multipro
-00004df0: 6365 7373 696e 672e 5369 6d70 6c65 5175  cessing.SimpleQu
-00004e00: 6575 6528 290a 2020 2020 2020 2020 2020  eue().          
-00004e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e20: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00004dd0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00004de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004df0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00004e00: 6f72 2063 2069 6e20 706c 6179 6572 5f6f  or c in player_o
+00004e10: 7574 7075 742e 706c 6179 6c69 7374 5b0a  utput.playlist[.
+00004e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e50: 2020 2020 2020 2020 666f 7220 6320 696e          for c in
-00004e60: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
-00004e70: 6c61 796c 6973 745b 0a20 2020 2020 2020  laylist[.       
-00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e40: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00004e50: 6572 5f6f 7574 7075 742e 690a 2020 2020  er_output.i.    
+00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e80: 2020 2020 5d5b 315d 3a0a 2020 2020 2020      ][1]:.      
 00004e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ea0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00004eb0: 7574 2e69 0a20 2020 2020 2020 2020 2020  ut.i.           
-00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ed0: 2020 2020 2020 2020 2020 2020 205d 5b2d               ][-
-00004ee0: 335d 3a0a 2020 2020 2020 2020 2020 2020  3]:.            
-00004ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f10: 6469 7363 6f72 645f 6172 7469 7374 5f71  discord_artist_q
-00004f20: 7565 7565 2e70 7574 2863 290a 2020 2020  ueue.put(c).    
+00004ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004eb0: 2020 2020 2020 6469 7363 6f72 645f 736f        discord_so
+00004ec0: 6e67 5f6e 616d 655f 7175 6575 652e 7075  ng_name_queue.pu
+00004ed0: 7428 6329 0a20 2020 2020 2020 2020 2020  t(c).           
+00004ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ef0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
+00004f00: 636f 7264 5f73 6f6e 675f 6e61 6d65 5f71  cord_song_name_q
+00004f10: 7565 7565 2e70 7574 2822 5c6e 2229 0a0a  ueue.put("\n")..
+00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f50: 2020 2020 6469 7363 6f72 645f 6172 7469      discord_arti
-00004f60: 7374 5f71 7565 7565 2e70 7574 2822 5c6e  st_queue.put("\n
-00004f70: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
-00004f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f90: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00004fa0: 6572 5f6f 7574 7075 742e 6469 7363 6f72  er_output.discor
-00004fb0: 645f 636f 6e6e 6563 7465 6420 3d20 280a  d_connected = (.
+00004f40: 2020 2020 2020 2020 6469 7363 6f72 645f          discord_
+00004f50: 6172 7469 7374 5f71 7565 7565 203d 2028  artist_queue = (
+00004f60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f80: 2020 2020 2020 2020 2020 2020 206d 756c               mul
+00004f90: 7469 7072 6f63 6573 7369 6e67 2e53 696d  tiprocessing.Sim
+00004fa0: 706c 6551 7565 7565 2829 0a20 2020 2020  pleQueue().     
+00004fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00004fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fe0: 2020 2020 2020 2020 2020 2020 6d75 6c74              mult
-00004ff0: 6970 726f 6365 7373 696e 672e 5661 6c75  iprocessing.Valu
-00005000: 6528 2269 222c 2032 290a 2020 2020 2020  e("i", 2).      
-00005010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004fd0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ff0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00005000: 2063 2069 6e20 706c 6179 6572 5f6f 7574   c in player_out
+00005010: 7075 742e 706c 6179 6c69 7374 5b0a 2020  put.playlist[.  
 00005020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005030: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-00005040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005050: 2020 2020 2020 2020 2020 2020 2023 2073               # s
-00005060: 7461 7274 206e 6577 2070 726f 6365 7373  tart new process
-00005070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005090: 2020 2020 2020 2020 2064 6973 636f 7264           discord
-000050a0: 5f70 7265 7365 6e63 655f 7072 6f63 6573  _presence_proces
-000050b0: 7320 3d20 6d75 6c74 6970 726f 6365 7373  s = multiprocess
-000050c0: 696e 672e 5072 6f63 6573 7328 0a20 2020  ing.Process(.   
-000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005040: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00005050: 5f6f 7574 7075 742e 690a 2020 2020 2020  _output.i.      
+00005060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005080: 2020 5d5b 2d33 5d3a 0a20 2020 2020 2020    ][-3]:.       
+00005090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050b0: 2020 2020 2064 6973 636f 7264 5f61 7274       discord_art
+000050c0: 6973 745f 7175 6575 652e 7075 7428 6329  ist_queue.put(c)
+000050d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000050e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050f0: 2020 2020 2020 2020 2064 6165 6d6f 6e3d           daemon=
-00005100: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050f0: 2020 2020 2020 2020 2064 6973 636f 7264           discord
+00005100: 5f61 7274 6973 745f 7175 6575 652e 7075  _artist_queue.pu
+00005110: 7428 225c 6e22 290a 0a20 2020 2020 2020  t("\n")..       
 00005120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005130: 2020 7461 7267 6574 3d64 6973 636f 7264    target=discord
-00005140: 5f70 7265 7365 6e63 655f 6c6f 6f70 2c0a  _presence_loop,.
-00005150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005170: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00005180: 3d28 0a20 2020 2020 2020 2020 2020 2020  =(.             
-00005190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051b0: 2020 2064 6973 636f 7264 5f73 6f6e 675f     discord_song_
-000051c0: 6e61 6d65 5f71 7565 7565 2c0a 2020 2020  name_queue,.    
-000051d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005140: 2070 6c61 7965 725f 6f75 7470 7574 2e64   player_output.d
+00005150: 6973 636f 7264 5f63 6f6e 6e65 6374 6564  iscord_connected
+00005160: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00005170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005190: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
+000051a0: 2e56 616c 7565 2822 6922 2c20 3229 0a20  .Value("i", 2). 
+000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000051d0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
 000051e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051f0: 2020 2020 2020 2020 2020 2020 6469 7363              disc
-00005200: 6f72 645f 6172 7469 7374 5f71 7565 7565  ord_artist_queue
-00005210: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000051f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005200: 2020 2320 7374 6172 7420 6e65 7720 7072    # start new pr
+00005210: 6f63 6573 730a 2020 2020 2020 2020 2020  ocess.          
 00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005240: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-00005250: 6469 7363 6f72 645f 636f 6e6e 6563 7465  discord_connecte
-00005260: 642c 0a20 2020 2020 2020 2020 2020 2020  d,.             
-00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005280: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00005290: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052b0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00005230: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00005240: 7363 6f72 645f 7072 6573 656e 6365 5f70  scord_presence_p
+00005250: 726f 6365 7373 203d 206d 756c 7469 7072  rocess = multipr
+00005260: 6f63 6573 7369 6e67 2e50 726f 6365 7373  ocessing.Process
+00005270: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005290: 2020 2020 2020 2020 2020 2020 2020 6461                da
+000052a0: 656d 6f6e 3d54 7275 652c 0a20 2020 2020  emon=True,.     
+000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000052c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052e0: 2020 2020 6469 7363 6f72 645f 7072 6573      discord_pres
-000052f0: 656e 6365 5f70 726f 6365 7373 2e73 7461  ence_process.sta
-00005300: 7274 2829 0a20 2020 2020 2020 2020 2020  rt().           
+000052d0: 2020 2020 2020 2074 6172 6765 743d 6469         target=di
+000052e0: 7363 6f72 645f 7072 6573 656e 6365 5f6c  scord_presence_l
+000052f0: 6f6f 702c 0a20 2020 2020 2020 2020 2020  oop,.           
+00005300: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005320: 2020 2020 2065 6c69 6620 6320 696e 2022       elif c in "
-00005330: 6949 223a 0a20 2020 2020 2020 2020 2020  iI":.           
+00005320: 2061 7267 733d 280a 2020 2020 2020 2020   args=(.        
+00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005350: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00005360: 6f75 7470 7574 2e61 6464 696e 675f 736f  output.adding_so
-00005370: 6e67 203d 2022 222c 2030 2c20 5472 7565  ng = "", 0, True
-00005380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005350: 2020 2020 2020 2020 6469 7363 6f72 645f          discord_
+00005360: 736f 6e67 5f6e 616d 655f 7175 6575 652c  song_name_queue,
+00005370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005380: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053a0: 2020 2020 2063 7572 7365 732e 6375 7273       curses.curs
-000053b0: 5f73 6574 2854 7275 6529 0a20 2020 2020  _set(True).     
+000053a0: 2064 6973 636f 7264 5f61 7274 6973 745f   discord_artist_
+000053b0: 7175 6575 652c 0a20 2020 2020 2020 2020  queue,.         
 000053c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000053d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000053e0: 6372 6565 6e5f 7369 7a65 203d 2073 7464  creen_size = std
-000053f0: 7363 722e 6765 746d 6178 7978 2829 0a20  scr.getmaxyx(). 
-00005400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053e0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+000053f0: 7470 7574 2e64 6973 636f 7264 5f63 6f6e  tput.discord_con
+00005400: 6e65 6374 6564 2c0a 2020 2020 2020 2020  nected,.        
 00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005420: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00005430: 2e73 6372 6f6c 6c65 722e 7265 7369 7a65  .scroller.resize
-00005440: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005460: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-00005470: 5f73 697a 655b 305d 202d 2033 0a20 2020  _size[0] - 3.   
-00005480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054a0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00005420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005430: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005450: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00005460: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005480: 2020 2020 2020 2020 2064 6973 636f 7264           discord
+00005490: 5f70 7265 7365 6e63 655f 7072 6f63 6573  _presence_proces
+000054a0: 732e 7374 6172 7428 290a 2020 2020 2020  s.start().      
 000054b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000054c0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-000054d0: 7470 7574 2e6f 7574 7075 7428 706c 6179  tput.output(play
-000054e0: 6261 636b 2e63 7572 725f 706f 7329 0a20  back.curr_pos). 
-000054f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005500: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00005510: 6c69 6620 6320 696e 2022 6141 223a 0a20  lif c in "aA":. 
+000054c0: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
+000054d0: 2069 6e20 2269 4922 3a0a 2020 2020 2020   in "iI":.      
+000054e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000054f0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00005500: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
+00005510: 7074 696e 6720 3d20 280a 2020 2020 2020  pting = (.      
 00005520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005540: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00005550: 2e61 6464 696e 675f 736f 6e67 203d 2022  .adding_song = "
-00005560: 222c 2030 2c20 4661 6c73 650a 2020 2020  ", 0, False.    
-00005570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005540: 2020 2222 2c0a 2020 2020 2020 2020 2020    "",.          
+00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005560: 2020 2020 2020 2020 2020 2020 2020 302c                0,
+00005570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00005580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005590: 6375 7273 6573 2e63 7572 735f 7365 7428  curses.curs_set(
-000055a0: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-000055b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000055c0: 2020 2020 2020 2020 2020 7363 7265 656e            screen
-000055d0: 5f73 697a 6520 3d20 7374 6473 6372 2e67  _size = stdscr.g
-000055e0: 6574 6d61 7879 7828 290a 2020 2020 2020  etmaxyx().      
-000055f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005600: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00005610: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
-00005620: 6c6c 6572 2e72 6573 697a 6528 0a20 2020  ller.resize(.   
-00005630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005650: 2020 2020 2073 6372 6565 6e5f 7369 7a65       screen_size
-00005660: 5b30 5d20 2d20 330a 2020 2020 2020 2020  [0] - 3.        
-00005670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005680: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00005690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005590: 2020 2020 2020 2020 2050 524f 4d50 545f           PROMPT_
+000055a0: 4d4f 4445 535b 2269 6e73 6572 7422 5d2c  MODES["insert"],
+000055b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000055c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055d0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000055e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000055f0: 2020 2020 2020 2020 2020 2063 7572 7365             curse
+00005600: 732e 6375 7273 5f73 6574 2854 7275 6529  s.curs_set(True)
+00005610: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005630: 2020 2020 2073 6372 6565 6e5f 7369 7a65       screen_size
+00005640: 203d 2073 7464 7363 722e 6765 746d 6178   = stdscr.getmax
+00005650: 7978 2829 0a20 2020 2020 2020 2020 2020  yx().           
+00005660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005670: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+00005680: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
+00005690: 7265 7369 7a65 280a 2020 2020 2020 2020  resize(.        
 000056a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056b0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-000056c0: 6f75 7470 7574 2870 6c61 7962 6163 6b2e  output(playback.
-000056d0: 6375 7272 5f70 6f73 290a 2020 2020 2020  curr_pos).      
+000056b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000056c0: 7363 7265 656e 5f73 697a 655b 305d 202d  screen_size[0] -
+000056d0: 2033 0a20 2020 2020 2020 2020 2020 2020   3.             
 000056e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000056f0: 2020 2020 2020 2020 2020 656c 6966 2063            elif c
-00005700: 2069 6e20 226d 4d22 3a0a 2020 2020 2020   in "mM":.      
-00005710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005720: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005730: 2070 6c61 7965 725f 6f75 7470 7574 2e76   player_output.v
-00005740: 6f6c 756d 6520 3d3d 2030 3a0a 2020 2020  olume == 0:.    
+000056f0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005710: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00005720: 7965 725f 6f75 7470 7574 2e6f 7574 7075  yer_output.outpu
+00005730: 7428 706c 6179 6261 636b 2e63 7572 725f  t(playback.curr_
+00005740: 706f 7329 0a20 2020 2020 2020 2020 2020  pos).           
 00005750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005770: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00005780: 742e 766f 6c75 6d65 203d 2070 7265 765f  t.volume = prev_
-00005790: 766f 6c75 6d65 0a20 2020 2020 2020 2020  volume.         
-000057a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000057c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000057d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000057e0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-000057f0: 6f75 7470 7574 2e76 6f6c 756d 6520 3d20  output.volume = 
-00005800: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+00005760: 2020 2020 2065 6c69 6620 6320 696e 2022       elif c in "
+00005770: 6141 223a 0a20 2020 2020 2020 2020 2020  aA":.           
+00005780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005790: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+000057a0: 6f75 7470 7574 2e70 726f 6d70 7469 6e67  output.prompting
+000057b0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+000057c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000057d0: 2020 2020 2020 2020 2020 2020 2022 222c               "",
+000057e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000057f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005800: 2020 2020 2020 2020 2030 2c0a 2020 2020           0,.    
 00005810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005820: 2020 2020 2020 706c 6179 6261 636b 2e73        playback.s
-00005830: 6574 5f76 6f6c 756d 6528 706c 6179 6572  et_volume(player
-00005840: 5f6f 7574 7075 742e 766f 6c75 6d65 290a  _output.volume).
-00005850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005870: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00005880: 7574 2e6f 7574 7075 7428 706c 6179 6261  ut.output(playba
-00005890: 636b 2e63 7572 725f 706f 7329 0a20 2020  ck.curr_pos).   
-000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058b0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-000058c0: 6620 6320 696e 2022 7656 223a 0a20 2020  f c in "vV":.   
-000058d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058f0: 2070 6c61 7965 725f 6f75 7470 7574 2e76   player_output.v
-00005900: 6973 7561 6c69 7a65 203d 2028 0a20 2020  isualize = (.   
-00005910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005930: 2020 2020 206e 6f74 2070 6c61 7965 725f       not player_
-00005940: 6f75 7470 7574 2e76 6973 7561 6c69 7a65  output.visualize
-00005950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005970: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00005980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005990: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-000059a0: 725f 6f75 7470 7574 2e6f 7574 7075 7428  r_output.output(
-000059b0: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
-000059c0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-000059d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000059e0: 2020 2065 6c69 6620 6320 3d3d 2022 2022     elif c == " "
-000059f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00005a20: 7075 742e 7061 7573 6564 203d 2028 0a20  put.paused = (. 
-00005a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2020 2020 2020 206e 6f74 2070 6c61 7965         not playe
-00005a60: 725f 6f75 7470 7574 2e70 6175 7365 640a  r_output.paused.
-00005a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005830: 2020 2020 5052 4f4d 5054 5f4d 4f44 4553      PROMPT_MODES
+00005840: 5b22 6164 6422 5d2c 0a20 2020 2020 2020  ["add"],.       
+00005850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005860: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005890: 2020 2063 7572 7365 732e 6375 7273 5f73     curses.curs_s
+000058a0: 6574 2854 7275 6529 0a20 2020 2020 2020  et(True).       
+000058b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000058c0: 2020 2020 2020 2020 2020 2020 2073 6372               scr
+000058d0: 6565 6e5f 7369 7a65 203d 2073 7464 7363  een_size = stdsc
+000058e0: 722e 6765 746d 6178 7978 2829 0a20 2020  r.getmaxyx().   
+000058f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005910: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
+00005920: 6372 6f6c 6c65 722e 7265 7369 7a65 280a  croller.resize(.
+00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005950: 2020 2020 2020 2020 7363 7265 656e 5f73          screen_s
+00005960: 697a 655b 305d 202d 2033 0a20 2020 2020  ize[0] - 3.     
+00005970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005980: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00005990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000059a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059b0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+000059c0: 7574 2e6f 7574 7075 7428 706c 6179 6261  ut.output(playba
+000059d0: 636b 2e63 7572 725f 706f 7329 0a20 2020  ck.curr_pos).   
+000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059f0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00005a00: 6620 6320 696e 2022 7454 223a 0a20 2020  f c in "tT":.   
+00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a30: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+00005a40: 726f 6d70 7469 6e67 203d 2028 0a20 2020  rompting = (.   
+00005a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a70: 2020 2020 2022 222c 0a20 2020 2020 2020       "",.       
 00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a90: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00005aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ab0: 2020 2020 2020 2020 2020 2069 6620 706c             if pl
-00005ac0: 6179 6572 5f6f 7574 7075 742e 7061 7573  ayer_output.paus
-00005ad0: 6564 3a0a 2020 2020 2020 2020 2020 2020  ed:.            
-00005ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005af0: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00005b00: 6261 636b 2e70 6175 7365 2829 0a20 2020  back.pause().   
+00005a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005aa0: 2030 2c0a 2020 2020 2020 2020 2020 2020   0,.            
+00005ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ac0: 2020 2020 2020 2020 2020 2020 5052 4f4d              PROM
+00005ad0: 5054 5f4d 4f44 4553 5b22 7461 6722 5d2c  PT_MODES["tag"],
+00005ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005b00: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
 00005b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b30: 2020 2020 2070 6175 7365 5f73 7461 7274       pause_start
-00005b40: 203d 2074 696d 6528 290a 2020 2020 2020   = time().      
+00005b20: 2020 2020 2020 2020 2020 2063 7572 7365             curse
+00005b30: 732e 6375 7273 5f73 6574 2854 7275 6529  s.curs_set(True)
+00005b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00005b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b60: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00005b70: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00005b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005b90: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00005ba0: 6261 636b 2e72 6573 756d 6528 290a 2020  back.resume().  
-00005bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005bd0: 2020 2020 2020 7374 6172 745f 7469 6d65        start_time
-00005be0: 202b 3d20 7469 6d65 2829 202d 2070 6175   += time() - pau
-00005bf0: 7365 5f73 7461 7274 0a0a 2020 2020 2020  se_start..      
-00005c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c10: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00005c20: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00005b60: 2020 2020 2073 6372 6565 6e5f 7369 7a65       screen_size
+00005b70: 203d 2073 7464 7363 722e 6765 746d 6178   = stdscr.getmax
+00005b80: 7978 2829 0a20 2020 2020 2020 2020 2020  yx().           
+00005b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ba0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+00005bb0: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
+00005bc0: 7265 7369 7a65 280a 2020 2020 2020 2020  resize(.        
+00005bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005bf0: 7363 7265 656e 5f73 697a 655b 305d 202d  screen_size[0] -
+00005c00: 2033 0a20 2020 2020 2020 2020 2020 2020   3.             
+00005c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c20: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 00005c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c40: 2020 2020 2020 2020 2020 2073 7973 2e70             sys.p
-00005c50: 6c61 7466 6f72 6d20 3d3d 2022 6461 7277  latform == "darw
-00005c60: 696e 220a 2020 2020 2020 2020 2020 2020  in".            
-00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00005c90: 6361 6e5f 6d61 635f 6e6f 775f 706c 6179  can_mac_now_play
-00005ca0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00005c40: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00005c50: 7965 725f 6f75 7470 7574 2e6f 7574 7075  yer_output.outpu
+00005c60: 7428 706c 6179 6261 636b 2e63 7572 725f  t(playback.curr_
+00005c70: 706f 7329 0a20 2020 2020 2020 2020 2020  pos).           
+00005c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005c90: 2020 2020 2065 6c69 6620 6320 696e 2022       elif c in "
+00005ca0: 6d4d 223a 0a20 2020 2020 2020 2020 2020  mM":.           
 00005cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cc0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00005cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005cf0: 2020 206d 6163 5f6e 6f77 5f70 6c61 7969     mac_now_playi
-00005d00: 6e67 2e70 6175 7365 6420 3d20 280a 2020  ng.paused = (.  
-00005d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d30: 2020 2020 2020 2020 2020 706c 6179 6572            player
-00005d40: 5f6f 7574 7075 742e 7061 7573 6564 0a20  _output.paused. 
-00005d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005cc0: 2020 2020 2020 2020 2069 6620 706c 6179           if play
+00005cd0: 6572 5f6f 7574 7075 742e 766f 6c75 6d65  er_output.volume
+00005ce0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
+00005cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d00: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00005d10: 6c61 7965 725f 6f75 7470 7574 2e76 6f6c  layer_output.vol
+00005d20: 756d 6520 3d20 7072 6576 5f76 6f6c 756d  ume = prev_volum
+00005d30: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00005d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d50: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 00005d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d70: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00005d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005da0: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
-00005db0: 742e 7061 7573 6564 3a0a 2020 2020 2020  t.paused:.      
-00005dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005de0: 2020 2020 2020 6d61 635f 6e6f 775f 706c        mac_now_pl
-00005df0: 6179 696e 672e 7061 7573 6528 290a 2020  aying.pause().  
+00005d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d80: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+00005d90: 742e 766f 6c75 6d65 203d 2030 0a20 2020  t.volume = 0.   
+00005da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005dc0: 2070 6c61 7962 6163 6b2e 7365 745f 766f   playback.set_vo
+00005dd0: 6c75 6d65 2870 6c61 7965 725f 6f75 7470  lume(player_outp
+00005de0: 7574 2e76 6f6c 756d 6529 0a0a 2020 2020  ut.volume)..    
+00005df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e20: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00005e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e10: 706c 6179 6572 5f6f 7574 7075 742e 6f75  player_output.ou
+00005e20: 7470 7574 2870 6c61 7962 6163 6b2e 6375  tput(playback.cu
+00005e30: 7272 5f70 6f73 290a 2020 2020 2020 2020  rr_pos).        
 00005e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e50: 2020 2020 2020 2020 6d61 635f 6e6f 775f          mac_now_
-00005e60: 706c 6179 696e 672e 7265 7375 6d65 2829  playing.resume()
-00005e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005e90: 2020 2020 2020 2020 2075 7064 6174 655f           update_
-00005ea0: 6e6f 775f 706c 6179 696e 6720 3d20 5472  now_playing = Tr
-00005eb0: 7565 0a0a 2020 2020 2020 2020 2020 2020  ue..            
+00005e50: 2020 2020 2020 2020 656c 6966 2063 2069          elif c i
+00005e60: 6e20 2276 5622 3a0a 2020 2020 2020 2020  n "vV":.        
+00005e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005e80: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00005e90: 6572 5f6f 7574 7075 742e 7669 7375 616c  er_output.visual
+00005ea0: 697a 6520 3d20 280a 2020 2020 2020 2020  ize = (.        
+00005eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005ed0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00005ee0: 7574 7075 742e 6f75 7470 7574 2870 6c61  utput.output(pla
-00005ef0: 7962 6163 6b2e 6375 7272 5f70 6f73 290a  yback.curr_pos).
+00005ed0: 6e6f 7420 706c 6179 6572 5f6f 7574 7075  not player_outpu
+00005ee0: 742e 7669 7375 616c 697a 650a 2020 2020  t.visualize.    
+00005ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f20: 656c 6966 2063 203d 3d20 225b 223a 0a20  elif c == "[":. 
-00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f50: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00005f60: 2e76 6f6c 756d 6520 3d20 6d61 7828 0a20  .volume = max(. 
-00005f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f90: 2020 2020 2020 2030 2c20 706c 6179 6572         0, player
-00005fa0: 5f6f 7574 7075 742e 766f 6c75 6d65 202d  _output.volume -
-00005fb0: 2056 4f4c 554d 455f 5354 4550 0a20 2020   VOLUME_STEP.   
-00005fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00005f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f30: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00005f40: 7075 742e 6f75 7470 7574 2870 6c61 7962  put.output(playb
+00005f50: 6163 6b2e 6375 7272 5f70 6f73 290a 2020  ack.curr_pos).  
+00005f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005f70: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00005f80: 6966 2063 203d 3d20 2220 223a 0a20 2020  if c == " ":.   
+00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fb0: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+00005fc0: 6175 7365 6420 3d20 280a 2020 2020 2020  aused = (.      
 00005fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005fe0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00005ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006000: 2020 2020 2020 2070 6c61 7962 6163 6b2e         playback.
-00006010: 7365 745f 766f 6c75 6d65 2870 6c61 7965  set_volume(playe
-00006020: 725f 6f75 7470 7574 2e76 6f6c 756d 6529  r_output.volume)
+00005fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ff0: 2020 6e6f 7420 706c 6179 6572 5f6f 7574    not player_out
+00006000: 7075 742e 7061 7573 6564 0a20 2020 2020  put.paused.     
+00006010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006020: 2020 2020 2020 2020 2020 2020 2020 2029                 )
 00006030: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
 00006040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006050: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00006060: 7075 742e 6f75 7470 7574 2870 6c61 7962  put.output(playb
-00006070: 6163 6b2e 6375 7272 5f70 6f73 290a 0a20  ack.curr_pos).. 
+00006050: 2020 2020 2020 6966 2070 6c61 7965 725f        if player_
+00006060: 6f75 7470 7574 2e70 6175 7365 643a 0a20  output.paused:. 
+00006070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060a0: 2020 2070 7265 765f 766f 6c75 6d65 203d     prev_volume =
-000060b0: 2070 6c61 7965 725f 6f75 7470 7574 2e76   player_output.v
-000060c0: 6f6c 756d 650a 2020 2020 2020 2020 2020  olume.          
-000060d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000060e0: 2020 2020 2020 656c 6966 2063 203d 3d20        elif c == 
-000060f0: 225d 223a 0a20 2020 2020 2020 2020 2020  "]":.           
-00006100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006110: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00006120: 6f75 7470 7574 2e76 6f6c 756d 6520 3d20  output.volume = 
-00006130: 6d69 6e28 0a20 2020 2020 2020 2020 2020  min(.           
-00006140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006150: 2020 2020 2020 2020 2020 2020 2031 2c20               1, 
-00006160: 706c 6179 6572 5f6f 7574 7075 742e 766f  player_output.vo
-00006170: 6c75 6d65 202b 2056 4f4c 554d 455f 5354  lume + VOLUME_ST
-00006180: 4550 0a20 2020 2020 2020 2020 2020 2020  EP.             
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000061b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061c0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-000061d0: 7962 6163 6b2e 7365 745f 766f 6c75 6d65  yback.set_volume
-000061e0: 2870 6c61 7965 725f 6f75 7470 7574 2e76  (player_output.v
-000061f0: 6f6c 756d 6529 0a0a 2020 2020 2020 2020  olume)..        
+00006090: 2020 2020 2020 2070 6c61 7962 6163 6b2e         playback.
+000060a0: 7061 7573 6528 290a 2020 2020 2020 2020  pause().        
+000060b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060d0: 7061 7573 655f 7374 6172 7420 3d20 7469  pause_start = ti
+000060e0: 6d65 2829 0a20 2020 2020 2020 2020 2020  me().           
+000060f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006100: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00006110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006130: 2020 2020 2020 2070 6c61 7962 6163 6b2e         playback.
+00006140: 7265 7375 6d65 2829 0a20 2020 2020 2020  resume().       
+00006150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006170: 2073 7461 7274 5f74 696d 6520 2b3d 2074   start_time += t
+00006180: 696d 6528 2920 2d20 7061 7573 655f 7374  ime() - pause_st
+00006190: 6172 740a 0a20 2020 2020 2020 2020 2020  art..           
+000061a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061b0: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
+000061c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000061e0: 2020 2020 2020 7379 732e 706c 6174 666f        sys.platfo
+000061f0: 726d 203d 3d20 2264 6172 7769 6e22 0a20  rm == "darwin". 
 00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006210: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00006220: 6572 5f6f 7574 7075 742e 6f75 7470 7574  er_output.output
-00006230: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
-00006240: 6f73 290a 0a20 2020 2020 2020 2020 2020  os)..           
+00006210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006220: 2020 2020 2020 2061 6e64 2063 616e 5f6d         and can_m
+00006230: 6163 5f6e 6f77 5f70 6c61 7969 6e67 0a20  ac_now_playing. 
+00006240: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006260: 2020 2020 2020 2020 2070 7265 765f 766f           prev_vo
-00006270: 6c75 6d65 203d 2070 6c61 7965 725f 6f75  lume = player_ou
-00006280: 7470 7574 2e76 6f6c 756d 650a 2020 2020  tput.volume.    
-00006290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062a0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000062b0: 2063 2069 6e20 225c 725c 6e22 3a0a 2020   c in "\r\n":.  
+00006260: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00006270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006280: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00006290: 635f 6e6f 775f 706c 6179 696e 672e 7061  c_now_playing.pa
+000062a0: 7573 6564 203d 2028 0a20 2020 2020 2020  used = (.       
+000062b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062e0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-000062f0: 6920 3d20 280a 2020 2020 2020 2020 2020  i = (.          
+000062d0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+000062e0: 7574 2e70 6175 7365 640a 2020 2020 2020  ut.paused.      
+000062f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006310: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00006320: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
-00006330: 6c6c 6572 2e70 6f73 202d 2031 0a20 2020  ller.pos - 1.   
-00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006360: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00006310: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00006320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006330: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+00006340: 6c61 7965 725f 6f75 7470 7574 2e70 6175  layer_output.pau
+00006350: 7365 643a 0a20 2020 2020 2020 2020 2020  sed:.           
+00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006380: 2020 2020 2020 206e 6578 745f 736f 6e67         next_song
-00006390: 203d 2031 0a20 2020 2020 2020 2020 2020   = 1.           
+00006380: 206d 6163 5f6e 6f77 5f70 6c61 7969 6e67   mac_now_playing
+00006390: 2e70 6175 7365 2829 0a20 2020 2020 2020  .pause().       
 000063a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063b0: 2020 2020 2020 2020 2070 6c61 7962 6163           playbac
-000063c0: 6b2e 7374 6f70 2829 0a20 2020 2020 2020  k.stop().       
+000063b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
 000063d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000063e0: 2020 2020 2020 2020 2020 2020 2062 7265               bre
-000063f0: 616b 0a20 2020 2020 2020 2020 2020 2020  ak.             
-00006400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006410: 2020 2065 6c69 6620 6320 696e 2022 5c62     elif c in "\b
-00006420: 5c78 3766 223a 0a20 2020 2020 2020 2020  \x7f":.         
-00006430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006440: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-00006450: 7465 645f 736f 6e67 203d 2070 6c61 7965  ted_song = playe
-00006460: 725f 6f75 7470 7574 2e73 6372 6f6c 6c65  r_output.scrolle
-00006470: 722e 706f 730a 2020 2020 2020 2020 2020  r.pos.          
-00006480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006490: 2020 2020 2020 2020 2020 6465 6c20 706c            del pl
-000064a0: 6179 6572 5f6f 7574 7075 742e 706c 6179  ayer_output.play
-000064b0: 6c69 7374 5b73 656c 6563 7465 645f 736f  list[selected_so
-000064c0: 6e67 5d0a 0a20 2020 2020 2020 2020 2020  ng]..           
+000063e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000063f0: 2020 206d 6163 5f6e 6f77 5f70 6c61 7969     mac_now_playi
+00006400: 6e67 2e72 6573 756d 6528 290a 2020 2020  ng.resume().    
+00006410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006430: 2020 2020 7570 6461 7465 5f6e 6f77 5f70      update_now_p
+00006440: 6c61 7969 6e67 203d 2054 7275 650a 0a20  laying = True.. 
+00006450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006470: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00006480: 2e6f 7574 7075 7428 706c 6179 6261 636b  .output(playback
+00006490: 2e63 7572 725f 706f 7329 0a20 2020 2020  .curr_pos).     
+000064a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064b0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+000064c0: 6320 3d3d 2022 5b22 3a0a 2020 2020 2020  c == "[":.      
 000064d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000064e0: 2020 2020 2020 2020 2069 6620 6c6f 6f70           if loop
-000064f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006510: 2020 2020 2020 2020 2020 6966 2072 6573            if res
-00006520: 6875 6666 6c65 3a0a 2020 2020 2020 2020  huffle:.        
-00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006550: 2020 2020 6e65 7874 5f70 6c61 796c 6973      next_playlis
-00006560: 7420 3d20 706c 6179 6c69 7374 5b3a 5d0a  t = playlist[:].
-00006570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000064e0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+000064f0: 6179 6572 5f6f 7574 7075 742e 766f 6c75  ayer_output.volu
+00006500: 6d65 203d 206d 6178 280a 2020 2020 2020  me = max(.      
+00006510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006530: 2020 302c 2070 6c61 7965 725f 6f75 7470    0, player_outp
+00006540: 7574 2e76 6f6c 756d 6520 2d20 564f 4c55  ut.volume - VOLU
+00006550: 4d45 5f53 5445 500a 2020 2020 2020 2020  ME_STEP.        
+00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006570: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
 00006580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006590: 2020 2020 2020 2020 2020 2020 7368 7566              shuf
-000065a0: 666c 6528 6e65 7874 5f70 6c61 796c 6973  fle(next_playlis
-000065b0: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
-000065c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000065d0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000065e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000065f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006600: 2020 2020 2020 2020 2020 2020 2064 656c               del
-00006610: 206e 6578 745f 706c 6179 6c69 7374 5b73   next_playlist[s
-00006620: 656c 6563 7465 645f 736f 6e67 5d0a 0a20  elected_song].. 
-00006630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006650: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00006660: 2e73 6372 6f6c 6c65 722e 6e75 6d5f 6c69  .scroller.num_li
-00006670: 6e65 7320 2d3d 2031 0a20 2020 2020 2020  nes -= 1.       
-00006680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006690: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000066a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000066b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000066c0: 2020 2020 2020 2020 2020 7365 6c65 6374            select
-000066d0: 6564 5f73 6f6e 6720 3d3d 2070 6c61 7965  ed_song == playe
-000066e0: 725f 6f75 7470 7574 2e69 0a20 2020 2020  r_output.i.     
-000066f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006700: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00006710: 3a20 2023 2064 656c 6574 6564 2063 7572  :  # deleted cur
-00006720: 7265 6e74 2073 6f6e 670a 2020 2020 2020  rent song.      
+00006590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065a0: 2020 706c 6179 6261 636b 2e73 6574 5f76    playback.set_v
+000065b0: 6f6c 756d 6528 706c 6179 6572 5f6f 7574  olume(player_out
+000065c0: 7075 742e 766f 6c75 6d65 290a 0a20 2020  put.volume)..   
+000065d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000065f0: 2070 6c61 7965 725f 6f75 7470 7574 2e6f   player_output.o
+00006600: 7574 7075 7428 706c 6179 6261 636b 2e63  utput(playback.c
+00006610: 7572 725f 706f 7329 0a0a 2020 2020 2020  urr_pos)..      
+00006620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006630: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00006640: 6576 5f76 6f6c 756d 6520 3d20 706c 6179  ev_volume = play
+00006650: 6572 5f6f 7574 7075 742e 766f 6c75 6d65  er_output.volume
+00006660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006680: 2065 6c69 6620 6320 3d3d 2022 5d22 3a0a   elif c == "]":.
+00006690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066b0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+000066c0: 742e 766f 6c75 6d65 203d 206d 696e 280a  t.volume = min(.
+000066d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000066f0: 2020 2020 2020 2020 312c 2070 6c61 7965          1, playe
+00006700: 725f 6f75 7470 7574 2e76 6f6c 756d 6520  r_output.volume 
+00006710: 2b20 564f 4c55 4d45 5f53 5445 500a 2020  + VOLUME_STEP.  
+00006720: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006750: 2020 6e65 7874 5f73 6f6e 6720 3d20 310a    next_song = 1.
-00006760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006780: 2020 2020 2020 2020 2320 7769 6c6c 2062          # will b
-00006790: 6520 696e 6372 656d 656e 7465 6420 746f  e incremented to
-000067a0: 2069 0a20 2020 2020 2020 2020 2020 2020   i.             
-000067b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067c0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-000067d0: 725f 6f75 7470 7574 2e73 6372 6f6c 6c65  r_output.scrolle
-000067e0: 722e 706f 7320 3d20 280a 2020 2020 2020  r.pos = (.      
+00006740: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00006750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006760: 2020 2020 2020 2020 706c 6179 6261 636b          playback
+00006770: 2e73 6574 5f76 6f6c 756d 6528 706c 6179  .set_volume(play
+00006780: 6572 5f6f 7574 7075 742e 766f 6c75 6d65  er_output.volume
+00006790: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067b0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+000067c0: 7470 7574 2e6f 7574 7075 7428 706c 6179  tput.output(play
+000067d0: 6261 636b 2e63 7572 725f 706f 7329 0a0a  back.curr_pos)..
+000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000067f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006810: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00006820: 7075 742e 6920 2d20 310a 2020 2020 2020  put.i - 1.      
+00006800: 2020 2020 7072 6576 5f76 6f6c 756d 6520      prev_volume 
+00006810: 3d20 706c 6179 6572 5f6f 7574 7075 742e  = player_output.
+00006820: 766f 6c75 6d65 0a20 2020 2020 2020 2020  volume.         
 00006830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006850: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00006840: 2020 2020 2020 2065 6c69 6620 6320 696e         elif c in
+00006850: 2022 5c72 5c6e 223a 0a20 2020 2020 2020   "\r\n":.       
 00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006870: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00006880: 6572 5f6f 7574 7075 742e 6920 2d3d 2031  er_output.i -= 1
+00006870: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00006880: 7965 725f 6f75 7470 7574 2e69 203d 2028  yer_output.i = (
 00006890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 000068a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068b0: 2020 2020 2020 2020 2070 6c61 7962 6163           playbac
-000068c0: 6b2e 7374 6f70 2829 0a20 2020 2020 2020  k.stop().       
-000068d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000068b0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+000068c0: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
+000068d0: 706f 7320 2d20 310a 2020 2020 2020 2020  pos - 1.        
 000068e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000068f0: 2062 7265 616b 0a20 2020 2020 2020 2020   break.         
+000068f0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
 00006900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006910: 2020 2020 2020 2020 2020 2023 2064 656c             # del
-00006920: 6574 6564 2073 6f6e 6720 6265 666f 7265  eted song before
-00006930: 2063 7572 7265 6e74 0a20 2020 2020 2020   current.       
+00006910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006920: 2020 6e65 7874 5f73 6f6e 6720 3d20 310a    next_song = 1.
+00006930: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006950: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00006960: 7365 6c65 6374 6564 5f73 6f6e 6720 3c20  selected_song < 
-00006970: 706c 6179 6572 5f6f 7574 7075 742e 693a  player_output.i:
-00006980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006950: 2020 2020 706c 6179 6261 636b 2e73 746f      playback.sto
+00006960: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
+00006970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006980: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
 00006990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069a0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-000069b0: 6f75 7470 7574 2e69 202d 3d20 310a 2020  output.i -= 1.  
-000069c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000069d0: 2020 2020 2020 2020 2020 6578 6365 7074            except
-000069e0: 2028 5661 6c75 6545 7272 6f72 2c20 4f76   (ValueError, Ov
-000069f0: 6572 666c 6f77 4572 726f 7229 3a0a 2020  erflowError):.  
-00006a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a10: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00006a20: 7373 0a20 2020 2020 2020 2020 2020 2020  ss.             
-00006a30: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00006a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a50: 2020 2020 2069 6620 6320 3d3d 2063 7572       if c == cur
-00006a60: 7365 732e 4b45 595f 4c45 4654 3a0a 2020  ses.KEY_LEFT:.  
+000069a0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+000069b0: 6966 2063 2069 6e20 225c 625c 7837 6622  if c in "\b\x7f"
+000069c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000069d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000069e0: 2020 2020 2020 7365 6c65 6374 6564 5f73        selected_s
+000069f0: 6f6e 6720 3d20 706c 6179 6572 5f6f 7574  ong = player_out
+00006a00: 7075 742e 7363 726f 6c6c 6572 2e70 6f73  put.scroller.pos
+00006a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006a30: 2020 2020 2064 656c 2070 6c61 7965 725f       del player_
+00006a40: 6f75 7470 7574 2e70 6c61 796c 6973 745b  output.playlist[
+00006a50: 7365 6c65 6374 6564 5f73 6f6e 675d 0a0a  selected_song]..
+00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a80: 2020 2020 2020 2020 2020 2320 7079 6c69            # pyli
-00006a90: 6e74 3a20 6469 7361 626c 653d 756e 7375  nt: disable=unsu
-00006aa0: 6273 6372 6970 7461 626c 652d 6f62 6a65  bscriptable-obje
-00006ab0: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
-00006ac0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00006ad0: 6c61 7965 725f 6f75 7470 7574 2e61 6464  layer_output.add
-00006ae0: 696e 675f 736f 6e67 203d 2028 0a20 2020  ing_song = (.   
-00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b00: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-00006b10: 7965 725f 6f75 7470 7574 2e61 6464 696e  yer_output.addin
-00006b20: 675f 736f 6e67 5b30 5d2c 0a20 2020 2020  g_song[0],.     
-00006b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b40: 2020 2020 2020 2020 2020 206d 6178 2870             max(p
-00006b50: 6c61 7965 725f 6f75 7470 7574 2e61 6464  layer_output.add
-00006b60: 696e 675f 736f 6e67 5b31 5d20 2d20 312c  ing_song[1] - 1,
-00006b70: 2030 292c 0a20 2020 2020 2020 2020 2020   0),.           
+00006a80: 2020 2020 6966 206c 6f6f 703a 0a20 2020      if loop:.   
+00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ab0: 2020 2020 2069 6620 7265 7368 7566 666c       if reshuffl
+00006ac0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00006ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ae0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00006af0: 6578 745f 706c 6179 6c69 7374 203d 2070  ext_playlist = p
+00006b00: 6c61 796c 6973 745b 3a5d 0a20 2020 2020  laylist[:].     
+00006b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b30: 2020 2020 2020 2073 6875 6666 6c65 286e         shuffle(n
+00006b40: 6578 745f 706c 6179 6c69 7374 290a 2020  ext_playlist).  
+00006b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006b70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 00006b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b90: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00006ba0: 7574 2e61 6464 696e 675f 736f 6e67 5b32  ut.adding_song[2
-00006bb0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-00006bc0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00006bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006be0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-00006bf0: 7965 725f 6f75 7470 7574 2e6f 7574 7075  yer_output.outpu
-00006c00: 7428 706c 6179 6261 636b 2e63 7572 725f  t(playback.curr_
-00006c10: 706f 7329 0a20 2020 2020 2020 2020 2020  pos).           
-00006c20: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00006c30: 6620 6320 3d3d 2063 7572 7365 732e 4b45  f c == curses.KE
-00006c40: 595f 5249 4748 543a 0a20 2020 2020 2020  Y_RIGHT:.       
+00006b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ba0: 2020 2020 2020 2020 6465 6c20 6e65 7874          del next
+00006bb0: 5f70 6c61 796c 6973 745b 7365 6c65 6374  _playlist[select
+00006bc0: 6564 5f73 6f6e 675d 0a0a 2020 2020 2020  ed_song]..      
+00006bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006be0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00006bf0: 6179 6572 5f6f 7574 7075 742e 7363 726f  ayer_output.scro
+00006c00: 6c6c 6572 2e6e 756d 5f6c 696e 6573 202d  ller.num_lines -
+00006c10: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
+00006c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006c30: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
+00006c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006c60: 2020 2020 2023 2070 796c 696e 743a 2064       # pylint: d
-00006c70: 6973 6162 6c65 3d75 6e73 7562 7363 7269  isable=unsubscri
-00006c80: 7074 6162 6c65 2d6f 626a 6563 740a 2020  ptable-object.  
+00006c60: 2020 2020 2073 656c 6563 7465 645f 736f       selected_so
+00006c70: 6e67 203d 3d20 706c 6179 6572 5f6f 7574  ng == player_out
+00006c80: 7075 742e 690a 2020 2020 2020 2020 2020  put.i.          
 00006c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ca0: 2020 2020 2020 2020 2020 706c 6179 6572            player
-00006cb0: 5f6f 7574 7075 742e 6164 6469 6e67 5f73  _output.adding_s
-00006cc0: 6f6e 6720 3d20 280a 2020 2020 2020 2020  ong = (.        
+00006ca0: 2020 2020 2020 2020 2020 293a 2020 2320            ):  # 
+00006cb0: 6465 6c65 7465 6420 6375 7272 656e 7420  deleted current 
+00006cc0: 736f 6e67 0a20 2020 2020 2020 2020 2020  song.           
 00006cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ce0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00006cf0: 7574 7075 742e 6164 6469 6e67 5f73 6f6e  utput.adding_son
-00006d00: 675b 305d 2c0a 2020 2020 2020 2020 2020  g[0],.          
+00006ce0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00006cf0: 745f 736f 6e67 203d 2031 0a20 2020 2020  t_song = 1.     
+00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d20: 2020 2020 2020 6d69 6e28 0a20 2020 2020        min(.     
-00006d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d40: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00006d50: 6c61 7965 725f 6f75 7470 7574 2e61 6464  layer_output.add
-00006d60: 696e 675f 736f 6e67 5b31 5d20 2b20 312c  ing_song[1] + 1,
-00006d70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d90: 2020 2020 206c 656e 2870 6c61 7965 725f       len(player_
-00006da0: 6f75 7470 7574 2e61 6464 696e 675f 736f  output.adding_so
-00006db0: 6e67 5b30 5d29 2c0a 2020 2020 2020 2020  ng[0]),.        
-00006dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006dd0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00006de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006df0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00006e00: 725f 6f75 7470 7574 2e61 6464 696e 675f  r_output.adding_
-00006e10: 736f 6e67 5b32 5d2c 0a20 2020 2020 2020  song[2],.       
-00006e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e30: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00006d20: 2020 2023 2077 696c 6c20 6265 2069 6e63     # will be inc
+00006d30: 7265 6d65 6e74 6564 2074 6f20 690a 2020  remented to i.  
+00006d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006d60: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00006d70: 7075 742e 7363 726f 6c6c 6572 2e70 6f73  put.scroller.pos
+00006d80: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00006d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006db0: 2070 6c61 7965 725f 6f75 7470 7574 2e69   player_output.i
+00006dc0: 202d 2031 0a20 2020 2020 2020 2020 2020   - 1.           
+00006dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006de0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e10: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00006e20: 7470 7574 2e69 202d 3d20 310a 2020 2020  tput.i -= 1.    
+00006e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e50: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00006e60: 2e6f 7574 7075 7428 706c 6179 6261 636b  .output(playback
-00006e70: 2e63 7572 725f 706f 7329 0a20 2020 2020  .curr_pos).     
-00006e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e90: 2020 2065 6c69 6620 6320 3d3d 2063 7572     elif c == cur
-00006ea0: 7365 732e 4b45 595f 5550 3a0a 2020 2020  ses.KEY_UP:.    
-00006eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ec0: 2020 2020 2020 2020 6966 2070 6c61 7965          if playe
-00006ed0: 725f 6f75 7470 7574 2e73 6372 6f6c 6c65  r_output.scrolle
-00006ee0: 722e 706f 7320 213d 2030 3a0a 2020 2020  r.pos != 0:.    
-00006ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f00: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00006f10: 6572 5f6f 7574 7075 742e 7363 726f 6c6c  er_output.scroll
-00006f20: 6572 2e73 6372 6f6c 6c5f 6261 636b 7761  er.scroll_backwa
-00006f30: 7264 2829 0a20 2020 2020 2020 2020 2020  rd().           
-00006f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f50: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00006f60: 7574 2e6f 7574 7075 7428 706c 6179 6261  ut.output(playba
-00006f70: 636b 2e63 7572 725f 706f 7329 0a20 2020  ck.curr_pos).   
-00006f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f90: 2020 2020 2065 6c69 6620 6320 3d3d 2063       elif c == c
-00006fa0: 7572 7365 732e 4b45 595f 444f 574e 3a0a  urses.KEY_DOWN:.
-00006fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006fc0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00006fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006e50: 2020 2020 706c 6179 6261 636b 2e73 746f      playback.sto
+00006e60: 7028 290a 2020 2020 2020 2020 2020 2020  p().            
+00006e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e80: 2020 2020 2020 2020 2020 2020 6272 6561              brea
+00006e90: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
+00006ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006eb0: 2020 2020 2020 2320 6465 6c65 7465 6420        # deleted 
+00006ec0: 736f 6e67 2062 6566 6f72 6520 6375 7272  song before curr
+00006ed0: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
+00006ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006ef0: 2020 2020 2020 2020 6966 2073 656c 6563          if selec
+00006f00: 7465 645f 736f 6e67 203c 2070 6c61 7965  ted_song < playe
+00006f10: 725f 6f75 7470 7574 2e69 3a0a 2020 2020  r_output.i:.    
+00006f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f40: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+00006f50: 742e 6920 2d3d 2031 0a20 2020 2020 2020  t.i -= 1.       
+00006f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006f70: 2020 2020 2065 7863 6570 7420 2856 616c       except (Val
+00006f80: 7565 4572 726f 722c 204f 7665 7266 6c6f  ueError, Overflo
+00006f90: 7745 7272 6f72 293a 0a20 2020 2020 2020  wError):.       
+00006fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fb0: 2020 2020 2020 2020 2070 6173 730a 2020           pass.  
+00006fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006fd0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
 00006fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ff0: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
-00007000: 6372 6f6c 6c65 722e 706f 730a 2020 2020  croller.pos.    
+00006ff0: 6966 2063 203d 3d20 6375 7273 6573 2e4b  if c == curses.K
+00007000: 4559 5f4c 4546 543a 0a20 2020 2020 2020  EY_LEFT:.       
 00007010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007020: 2020 2020 2020 2020 2020 2020 213d 2070              != p
-00007030: 6c61 7965 725f 6f75 7470 7574 2e73 6372  layer_output.scr
-00007040: 6f6c 6c65 722e 6e75 6d5f 6c69 6e65 7320  oller.num_lines 
-00007050: 2d20 310a 2020 2020 2020 2020 2020 2020  - 1.            
-00007060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007070: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00007080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007090: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-000070a0: 2e73 6372 6f6c 6c65 722e 7363 726f 6c6c  .scroller.scroll
-000070b0: 5f66 6f72 7761 7264 2829 0a20 2020 2020  _forward().     
-000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000070d0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-000070e0: 725f 6f75 7470 7574 2e6f 7574 7075 7428  r_output.output(
-000070f0: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
-00007100: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-00007110: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00007120: 6320 3d3d 2063 7572 7365 732e 4b45 595f  c == curses.KEY_
-00007130: 4443 3a0a 2020 2020 2020 2020 2020 2020  DC:.            
-00007140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007150: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
-00007160: 653d 756e 7375 6273 6372 6970 7461 626c  e=unsubscriptabl
-00007170: 652d 6f62 6a65 6374 0a20 2020 2020 2020  e-object.       
-00007180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007190: 2020 2020 2069 6620 706c 6179 6572 5f6f       if player_o
-000071a0: 7574 7075 742e 6164 6469 6e67 5f73 6f6e  utput.adding_son
-000071b0: 675b 315d 203e 2030 3a0a 2020 2020 2020  g[1] > 0:.      
-000071c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071d0: 2020 2020 2020 2020 2020 706c 6179 6572            player
-000071e0: 5f6f 7574 7075 742e 6164 6469 6e67 5f73  _output.adding_s
-000071f0: 6f6e 6720 3d20 280a 2020 2020 2020 2020  ong = (.        
-00007200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007210: 2020 2020 2020 2020 2020 2020 706c 6179              play
-00007220: 6572 5f6f 7574 7075 742e 6164 6469 6e67  er_output.adding
-00007230: 5f73 6f6e 675b 305d 5b0a 2020 2020 2020  _song[0][.      
-00007240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007260: 2020 3a20 706c 6179 6572 5f6f 7574 7075    : player_outpu
-00007270: 742e 6164 6469 6e67 5f73 6f6e 675b 315d  t.adding_song[1]
-00007280: 202d 2031 0a20 2020 2020 2020 2020 2020   - 1.           
-00007290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072a0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-000072b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072c0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
-000072d0: 2070 6c61 7965 725f 6f75 7470 7574 2e61   player_output.a
-000072e0: 6464 696e 675f 736f 6e67 5b30 5d5b 0a20  dding_song[0][. 
-000072f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007020: 2020 2020 2023 2070 796c 696e 743a 2064       # pylint: d
+00007030: 6973 6162 6c65 3d75 6e73 7562 7363 7269  isable=unsubscri
+00007040: 7074 6162 6c65 2d6f 626a 6563 740a 2020  ptable-object.  
+00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007060: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00007070: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+00007080: 6720 3d20 280a 2020 2020 2020 2020 2020  g = (.          
+00007090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070a0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+000070b0: 7075 742e 7072 6f6d 7074 696e 675b 305d  put.prompting[0]
+000070c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000070d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070e0: 2020 6d61 7828 706c 6179 6572 5f6f 7574    max(player_out
+000070f0: 7075 742e 7072 6f6d 7074 696e 675b 315d  put.prompting[1]
+00007100: 202d 2031 2c20 3029 2c0a 2020 2020 2020   - 1, 0),.      
+00007110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007120: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00007130: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+00007140: 675b 325d 2c0a 2020 2020 2020 2020 2020  g[2],.          
+00007150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007160: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007180: 706c 6179 6572 5f6f 7574 7075 742e 6f75  player_output.ou
+00007190: 7470 7574 2870 6c61 7962 6163 6b2e 6375  tput(playback.cu
+000071a0: 7272 5f70 6f73 290a 2020 2020 2020 2020  rr_pos).        
+000071b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071c0: 656c 6966 2063 203d 3d20 6375 7273 6573  elif c == curses
+000071d0: 2e4b 4559 5f52 4947 4854 3a0a 2020 2020  .KEY_RIGHT:.    
+000071e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071f0: 2020 2020 2020 2020 2320 7079 6c69 6e74          # pylint
+00007200: 3a20 6469 7361 626c 653d 756e 7375 6273  : disable=unsubs
+00007210: 6372 6970 7461 626c 652d 6f62 6a65 6374  criptable-object
+00007220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007230: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00007240: 7965 725f 6f75 7470 7574 2e70 726f 6d70  yer_output.promp
+00007250: 7469 6e67 203d 2028 0a20 2020 2020 2020  ting = (.       
+00007260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007270: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+00007280: 6f75 7470 7574 2e70 726f 6d70 7469 6e67  output.prompting
+00007290: 5b30 5d2c 0a20 2020 2020 2020 2020 2020  [0],.           
+000072a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072b0: 2020 2020 206d 696e 280a 2020 2020 2020       min(.      
+000072c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072d0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+000072e0: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
+000072f0: 7074 696e 675b 315d 202b 2031 2c0a 2020  pting[1] + 1,.  
 00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007310: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-00007320: 7470 7574 2e61 6464 696e 675f 736f 6e67  tput.adding_song
-00007330: 5b31 5d20 3a0a 2020 2020 2020 2020 2020  [1] :.          
-00007340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007350: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007320: 2020 6c65 6e28 706c 6179 6572 5f6f 7574    len(player_out
+00007330: 7075 742e 7072 6f6d 7074 696e 675b 305d  put.prompting[0]
+00007340: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00007350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007360: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
 00007370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007380: 2070 6c61 7965 725f 6f75 7470 7574 2e61   player_output.a
-00007390: 6464 696e 675f 736f 6e67 5b31 5d20 2d20  dding_song[1] - 
-000073a0: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
-000073b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073c0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-000073d0: 7470 7574 2e61 6464 696e 675f 736f 6e67  tput.adding_song
-000073e0: 5b32 5d2c 0a20 2020 2020 2020 2020 2020  [2],.           
-000073f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007400: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00007410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007420: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00007430: 2e6f 7574 7075 7428 706c 6179 6261 636b  .output(playback
-00007440: 2e63 7572 725f 706f 7329 0a20 2020 2020  .curr_pos).     
-00007450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007460: 2020 2065 6c69 6620 6320 3d3d 2063 7572     elif c == cur
-00007470: 7365 732e 4b45 595f 454e 5445 523a 0a20  ses.KEY_ENTER:. 
+00007380: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+00007390: 7075 742e 7072 6f6d 7074 696e 675b 325d  put.prompting[2]
+000073a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000073b0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000073c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073d0: 2020 2020 2020 2020 2020 2020 706c 6179              play
+000073e0: 6572 5f6f 7574 7075 742e 6f75 7470 7574  er_output.output
+000073f0: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
+00007400: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
+00007410: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00007420: 2063 203d 3d20 6375 7273 6573 2e4b 4559   c == curses.KEY
+00007430: 5f55 503a 0a20 2020 2020 2020 2020 2020  _UP:.           
+00007440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007450: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
+00007460: 742e 7363 726f 6c6c 6572 2e70 6f73 2021  t.scroller.pos !
+00007470: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
 00007480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007490: 2020 2020 2020 2020 2020 2023 2070 796c             # pyl
-000074a0: 696e 743a 2064 6973 6162 6c65 3d75 6e73  int: disable=uns
-000074b0: 7562 7363 7269 7074 6162 6c65 2d6f 626a  ubscriptable-obj
-000074c0: 6563 740a 2020 2020 2020 2020 2020 2020  ect.            
-000074d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000074e0: 6966 2070 6c61 7965 725f 6f75 7470 7574  if player_output
-000074f0: 2e61 6464 696e 675f 736f 6e67 5b30 5d2e  .adding_song[0].
-00007500: 6973 6e75 6d65 7269 6328 293a 0a20 2020  isnumeric():.   
-00007510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007520: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00007530: 2064 6574 6169 6c73 2069 6e20 706c 6179   details in play
-00007540: 6572 5f6f 7574 7075 742e 706c 6179 6c69  er_output.playli
-00007550: 7374 3a0a 2020 2020 2020 2020 2020 2020  st:.            
+00007490: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+000074a0: 7574 2e73 6372 6f6c 6c65 722e 7363 726f  ut.scroller.scro
+000074b0: 6c6c 5f62 6163 6b77 6172 6428 290a 2020  ll_backward().  
+000074c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000074d0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+000074e0: 6179 6572 5f6f 7574 7075 742e 6f75 7470  ayer_output.outp
+000074f0: 7574 2870 6c61 7962 6163 6b2e 6375 7272  ut(playback.curr
+00007500: 5f70 6f73 290a 2020 2020 2020 2020 2020  _pos).          
+00007510: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00007520: 6966 2063 203d 3d20 6375 7273 6573 2e4b  if c == curses.K
+00007530: 4559 5f44 4f57 4e3a 0a20 2020 2020 2020  EY_DOWN:.       
+00007540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007550: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
 00007560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007570: 2020 2020 2020 2020 6966 2069 6e74 2864          if int(d
-00007580: 6574 6169 6c73 5b30 5d29 203d 3d20 696e  etails[0]) == in
-00007590: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00007570: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00007580: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
+00007590: 2e70 6f73 0a20 2020 2020 2020 2020 2020  .pos.           
 000075a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075b0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-000075c0: 725f 6f75 7470 7574 2e61 6464 696e 675f  r_output.adding_
-000075d0: 736f 6e67 5b30 5d0a 2020 2020 2020 2020  song[0].        
+000075b0: 2020 2020 2021 3d20 706c 6179 6572 5f6f       != player_o
+000075c0: 7574 7075 742e 7363 726f 6c6c 6572 2e6e  utput.scroller.n
+000075d0: 756d 5f6c 696e 6573 202d 2031 0a20 2020  um_lines - 1.   
 000075e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000075f0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
+000075f0: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
 00007600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007620: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
-00007630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007640: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00007650: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00007660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007670: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
-00007680: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00007610: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00007620: 6572 5f6f 7574 7075 742e 7363 726f 6c6c  er_output.scroll
+00007630: 6572 2e73 6372 6f6c 6c5f 666f 7277 6172  er.scroll_forwar
+00007640: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
+00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+00007670: 742e 6f75 7470 7574 2870 6c61 7962 6163  t.output(playbac
+00007680: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
 00007690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076a0: 2020 2020 2020 2020 2020 534f 4e47 535f            SONGS_
-000076b0: 494e 464f 5f50 4154 482c 0a20 2020 2020  INFO_PATH,.     
+000076a0: 2020 2020 656c 6966 2063 203d 3d20 6375      elif c == cu
+000076b0: 7273 6573 2e4b 4559 5f44 433a 0a20 2020  rses.KEY_DC:.   
 000076c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000076e0: 2020 2022 7222 2c0a 2020 2020 2020 2020     "r",.        
-000076f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007710: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
-00007720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007740: 2020 2020 2020 2920 6173 2073 6f6e 6773        ) as songs
-00007750: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
-00007760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007770: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00007780: 6f72 206c 696e 6520 696e 2073 6f6e 6773  or line in songs
-00007790: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
-000077a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000077c0: 2020 2064 6574 6169 6c73 203d 206c 696e     details = lin
-000077d0: 652e 7374 7269 7028 292e 7370 6c69 7428  e.strip().split(
-000077e0: 227c 2229 0a20 2020 2020 2020 2020 2020  "|").           
-000077f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007810: 2073 6f6e 675f 6964 203d 2069 6e74 2864   song_id = int(d
-00007820: 6574 6169 6c73 5b30 5d29 0a20 2020 2020  etails[0]).     
+000076d0: 2020 2020 2020 2020 2023 2070 796c 696e           # pylin
+000076e0: 743a 2064 6973 6162 6c65 3d75 6e73 7562  t: disable=unsub
+000076f0: 7363 7269 7074 6162 6c65 2d6f 626a 6563  scriptable-objec
+00007700: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00007710: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00007720: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+00007730: 726f 6d70 7469 6e67 5b31 5d20 3e20 303a  rompting[1] > 0:
+00007740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007760: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+00007770: 726f 6d70 7469 6e67 203d 2028 0a20 2020  rompting = (.   
+00007780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077a0: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+000077b0: 726f 6d70 7469 6e67 5b30 5d5b 0a20 2020  rompting[0][.   
+000077c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000077e0: 2020 2020 203a 2070 6c61 7965 725f 6f75       : player_ou
+000077f0: 7470 7574 2e70 726f 6d70 7469 6e67 5b31  tput.prompting[1
+00007800: 5d20 2d20 310a 2020 2020 2020 2020 2020  ] - 1.          
+00007810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007820: 2020 2020 2020 2020 2020 5d0a 2020 2020            ].    
 00007830: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007850: 2020 2020 2020 2069 6620 736f 6e67 5f69         if song_i
-00007860: 6420 3d3d 2069 6e74 280a 2020 2020 2020  d == int(.      
+00007850: 2b20 706c 6179 6572 5f6f 7574 7075 742e  + player_output.
+00007860: 7072 6f6d 7074 696e 675b 305d 5b0a 2020  prompting[0][.  
 00007870: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007890: 2020 2020 2020 2020 2020 706c 6179 6572            player
-000078a0: 5f6f 7574 7075 742e 6164 6469 6e67 5f73  _output.adding_s
-000078b0: 6f6e 675b 305d 0a20 2020 2020 2020 2020  ong[0].         
+00007890: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+000078a0: 7075 742e 7072 6f6d 7074 696e 675b 315d  put.prompting[1]
+000078b0: 203a 0a20 2020 2020 2020 2020 2020 2020   :.             
 000078c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078e0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-000078f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007910: 2020 2020 2020 6966 2070 6c61 7965 725f        if player_
-00007920: 6f75 7470 7574 2e61 6464 696e 675f 736f  output.adding_so
-00007930: 6e67 5b32 5d3a 0a20 2020 2020 2020 2020  ng[2]:.         
-00007940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00007970: 725f 6f75 7470 7574 2e70 6c61 796c 6973  r_output.playlis
-00007980: 742e 696e 7365 7274 280a 2020 2020 2020  t.insert(.      
-00007990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079c0: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-000079d0: 6920 2b20 312c 0a20 2020 2020 2020 2020  i + 1,.         
-000079e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000079f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a00: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00007a10: 6574 6169 6c73 2c0a 2020 2020 2020 2020  etails,.        
-00007a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a40: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a70: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00007a80: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00007a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078d0: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000078f0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00007900: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
+00007910: 7074 696e 675b 315d 202d 2031 2c0a 2020  pting[1] - 1,.  
+00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007940: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+00007950: 7072 6f6d 7074 696e 675b 325d 2c0a 2020  prompting[2],.  
+00007960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007970: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00007980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007990: 2020 2020 2020 2020 2020 2020 706c 6179              play
+000079a0: 6572 5f6f 7574 7075 742e 6f75 7470 7574  er_output.output
+000079b0: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
+000079c0: 6f73 290a 2020 2020 2020 2020 2020 2020  os).            
+000079d0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+000079e0: 2063 203d 3d20 6375 7273 6573 2e4b 4559   c == curses.KEY
+000079f0: 5f45 4e54 4552 3a0a 2020 2020 2020 2020  _ENTER:.        
+00007a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a10: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
+00007a20: 7361 626c 653d 756e 7375 6273 6372 6970  sable=unsubscrip
+00007a30: 7461 626c 652d 6f62 6a65 6374 0a20 2020  table-object.   
+00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a50: 2020 2020 2020 2020 2069 6620 706c 6179           if play
+00007a60: 6572 5f6f 7574 7075 742e 7072 6f6d 7074  er_output.prompt
+00007a70: 696e 675b 0a20 2020 2020 2020 2020 2020  ing[.           
+00007a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a90: 2020 2020 2030 0a20 2020 2020 2020 2020       0.         
 00007aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ab0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00007ac0: 7574 7075 742e 706c 6179 6c69 7374 2e61  utput.playlist.a
-00007ad0: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
-00007ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ab0: 2020 205d 2e69 736e 756d 6572 6963 2829     ].isnumeric()
+00007ac0: 2061 6e64 2070 6c61 7965 725f 6f75 7470   and player_outp
+00007ad0: 7574 2e70 726f 6d70 7469 6e67 5b32 5d20  ut.prompting[2] 
+00007ae0: 696e 2028 0a20 2020 2020 2020 2020 2020  in (.           
 00007af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b00: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00007b10: 6574 6169 6c73 0a20 2020 2020 2020 2020  etails.         
+00007b00: 2020 2020 2050 524f 4d50 545f 4d4f 4445       PROMPT_MODE
+00007b10: 535b 2261 6464 225d 2c0a 2020 2020 2020  S["add"],.      
 00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00007b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00007b80: 6c6f 6f70 3a0a 2020 2020 2020 2020 2020  loop:.          
-00007b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bb0: 2020 2020 2020 2020 2020 6966 2072 6573            if res
-00007bc0: 6875 6666 6c65 3a0a 2020 2020 2020 2020  huffle:.        
-00007bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c00: 6e65 7874 5f70 6c61 796c 6973 742e 696e  next_playlist.in
-00007c10: 7365 7274 280a 2020 2020 2020 2020 2020  sert(.          
-00007c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b30: 2020 2020 2020 2020 2020 5052 4f4d 5054            PROMPT
+00007b40: 5f4d 4f44 4553 5b22 696e 7365 7274 225d  _MODES["insert"]
+00007b50: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007b60: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+00007b70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007b90: 2066 6f72 2064 6574 6169 6c73 2069 6e20   for details in 
+00007ba0: 706c 6179 6572 5f6f 7574 7075 742e 706c  player_output.pl
+00007bb0: 6179 6c69 7374 3a0a 2020 2020 2020 2020  aylist:.        
+00007bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bd0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00007be0: 6e74 2864 6574 6169 6c73 5b30 5d29 203d  nt(details[0]) =
+00007bf0: 3d20 696e 7428 0a20 2020 2020 2020 2020  = int(.         
+00007c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00007c20: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
+00007c30: 6d70 7469 6e67 5b30 5d0a 2020 2020 2020  mpting[0].      
 00007c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c50: 2020 7261 6e64 696e 7428 0a20 2020 2020    randint(.     
-00007c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c50: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+00007c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00007c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007c90: 2020 2020 2020 2020 2020 2030 2c0a 2020             0,.  
-00007ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007c80: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+00007c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ca0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00007cb0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
 00007cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007cd0: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00007ce0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00007cd0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
+00007ce0: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
 00007cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d20: 2020 2020 2020 206e 6578 745f 706c 6179         next_play
-00007d30: 6c69 7374 0a20 2020 2020 2020 2020 2020  list.           
-00007d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d00: 2020 2020 2020 2020 2020 2020 534f 4e47              SONG
+00007d10: 535f 494e 464f 5f50 4154 482c 0a20 2020  S_INFO_PATH,.   
+00007d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d40: 2020 2020 2022 7222 2c0a 2020 2020 2020       "r",.      
 00007d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007d70: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00007d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d70: 2020 656e 636f 6469 6e67 3d22 7574 662d    encoding="utf-
+00007d80: 3822 2c0a 2020 2020 2020 2020 2020 2020  8",.            
 00007d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007db0: 2020 2020 2020 202d 2031 2c0a 2020 2020         - 1,.    
+00007da0: 2020 2020 2020 2020 2920 6173 2073 6f6e          ) as son
+00007db0: 6773 5f66 696c 653a 0a20 2020 2020 2020  gs_file:.       
 00007dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007df0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00007de0: 2066 6f72 206c 696e 6520 696e 2073 6f6e   for line in son
+00007df0: 6773 5f66 696c 653a 0a20 2020 2020 2020  gs_file:.       
 00007e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e30: 2020 2020 2020 2064 6574 6169 6c73 2c0a         details,.
-00007e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e20: 2020 2020 2064 6574 6169 6c73 203d 206c       details = l
+00007e30: 696e 652e 7374 7269 7028 292e 7370 6c69  ine.strip().spli
+00007e40: 7428 227c 2229 0a20 2020 2020 2020 2020  t("|").         
 00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e70: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00007e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007e70: 2020 2073 6f6e 675f 6964 203d 2069 6e74     song_id = int
+00007e80: 2864 6574 6169 6c73 5b30 5d29 0a20 2020  (details[0]).   
 00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00007eb0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007eb0: 2020 2020 2020 2020 2069 6620 736f 6e67           if song
+00007ec0: 5f69 6420 3d3d 2069 6e74 280a 2020 2020  _id == int(.    
 00007ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ee0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-00007ef0: 6c61 7965 725f 6f75 7470 7574 2e61 6464  layer_output.add
-00007f00: 696e 675f 736f 6e67 5b0a 2020 2020 2020  ing_song[.      
-00007f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ef0: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00007f00: 6572 5f6f 7574 7075 742e 7072 6f6d 7074  er_output.prompt
+00007f10: 696e 675b 305d 0a20 2020 2020 2020 2020  ing[0].         
 00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 2020 2020 320a 2020 2020 2020 2020        2.        
+00007f40: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
 00007f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f80: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00007f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f70: 2020 2020 2020 736f 6e67 5f64 6174 6120        song_data 
+00007f80: 3d20 6d75 7369 635f 7461 672e 6c6f 6164  = music_tag.load
+00007f90: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
 00007fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007fb0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00007fc0: 6578 745f 706c 6179 6c69 7374 2e69 6e73  ext_playlist.ins
-00007fd0: 6572 7428 0a20 2020 2020 2020 2020 2020  ert(.           
+00007fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007fc0: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
+00007fd0: 7468 2e6a 6f69 6e28 0a20 2020 2020 2020  th.join(.       
 00007fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00007ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008010: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00008020: 7574 2e69 0a20 2020 2020 2020 2020 2020  ut.i.           
+00008010: 2053 4f4e 4753 5f44 4952 2c20 6465 7461   SONGS_DIR, deta
+00008020: 696c 735b 315d 0a20 2020 2020 2020 2020  ils[1].         
 00008030: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008060: 2020 2020 202b 2031 2c0a 2020 2020 2020       + 1,.      
+00008050: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00008060: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008080: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
 00008090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080a0: 2020 2020 2020 2020 2020 6465 7461 696c            detail
-000080b0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000080c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080b0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000080c0: 6574 6169 6c73 202b 3d20 5b0a 2020 2020  etails += [.    
 000080d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000080f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000080f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008100: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
 00008110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008120: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00008130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008130: 2020 2020 2020 2020 2020 736f 6e67 5f64            song_d
+00008140: 6174 615b 0a20 2020 2020 2020 2020 2020  ata[.           
 00008150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008160: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00008170: 706c 6179 6c69 7374 2e61 7070 656e 6428  playlist.append(
-00008180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008180: 2022 6172 7469 7374 220a 2020 2020 2020   "artist".      
 00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000081b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081c0: 2064 6574 6169 6c73 0a20 2020 2020 2020   details.       
+000081c0: 2020 5d2e 7661 6c75 650a 2020 2020 2020    ].value.      
 000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000081e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008200: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00008210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008200: 2020 6f72 2022 556e 6b6e 6f77 6e20 4172    or "Unknown Ar
+00008210: 7469 7374 220a 2020 2020 2020 2020 2020  tist".          
 00008220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008230: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-00008240: 7470 7574 2e73 6372 6f6c 6c65 722e 6e75  tput.scroller.nu
-00008250: 6d5f 6c69 6e65 7320 2b3d 2028 0a20 2020  m_lines += (.   
+00008230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008240: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00008250: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008260: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008290: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+00008280: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00008290: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000082a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082c0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-000082d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000082b0: 2020 2020 2020 2020 2020 2073 6f6e 675f             song_
+000082c0: 6461 7461 5b22 616c 6275 6d22 5d2e 7661  data["album"].va
+000082d0: 6c75 650a 2020 2020 2020 2020 2020 2020  lue.            
 000082e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000082f0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00008300: 7574 2e61 6464 696e 675f 736f 6e67 203d  ut.adding_song =
-00008310: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+000082f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008300: 2020 2020 2020 2020 2020 2020 6f72 2022              or "
+00008310: 556e 6b6e 6f77 6e20 416c 6275 6d22 0a20  Unknown Album". 
 00008320: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008340: 2020 2020 2020 6375 7273 6573 2e63 7572        curses.cur
-00008350: 735f 7365 7428 4661 6c73 6529 0a20 2020  s_set(False).   
+00008340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008350: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
 00008360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008380: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-00008390: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
-000083a0: 6c65 722e 7265 7369 7a65 280a 2020 2020  ler.resize(.    
+00008380: 2020 2020 2020 2020 2020 280a 2020 2020            (.    
+00008390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000083b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083c0: 2020 2020 736f 6e67 5f64 6174 615b 0a20      song_data[. 
 000083d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000083e0: 7363 7265 656e 5f73 697a 655b 305d 202d  screen_size[0] -
-000083f0: 2032 0a20 2020 2020 2020 2020 2020 2020   2.             
-00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008420: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000083e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000083f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008400: 2020 2020 2020 2020 2020 2022 616c 6275             "albu
+00008410: 6d61 7274 6973 7422 0a20 2020 2020 2020  martist".       
+00008420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008450: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00008460: 7574 2e6f 7574 7075 7428 0a20 2020 2020  ut.output(.     
+00008450: 205d 2e76 616c 7565 0a20 2020 2020 2020   ].value.       
+00008460: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008490: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000084a0: 6c61 7962 6163 6b2e 6375 7272 5f70 6f73  layback.curr_pos
-000084b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008490: 206f 7220 2255 6e6b 6e6f 776e 2041 6c62   or "Unknown Alb
+000084a0: 756d 2041 7274 6973 7422 0a20 2020 2020  um Artist".     
+000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000084c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084e0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+000084d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000084e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 000084f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008510: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00008510: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
 00008520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008530: 2065 6c69 6620 6320 3d3d 2032 373a 2020   elif c == 27:  
-00008540: 2320 4553 4320 6b65 790a 2020 2020 2020  # ESC key.      
+00008530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008540: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
 00008550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008560: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00008570: 7075 742e 6164 6469 6e67 5f73 6f6e 6720  put.adding_song 
-00008580: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
-00008590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085a0: 2020 2063 7572 7365 732e 6375 7273 5f73     curses.curs_s
-000085b0: 6574 2846 616c 7365 290a 2020 2020 2020  et(False).      
-000085c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000085d0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-000085e0: 7075 742e 7363 726f 6c6c 6572 2e72 6573  put.scroller.res
-000085f0: 697a 6528 7363 7265 656e 5f73 697a 655b  ize(screen_size[
-00008600: 305d 202d 2032 290a 2020 2020 2020 2020  0] - 2).        
-00008610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008620: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-00008630: 742e 6f75 7470 7574 2870 6c61 7962 6163  t.output(playbac
-00008640: 6b2e 6375 7272 5f70 6f73 290a 2020 2020  k.curr_pos).    
-00008650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008660: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008570: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00008580: 7965 725f 6f75 7470 7574 2e70 726f 6d70  yer_output.promp
+00008590: 7469 6e67 5b32 5d0a 2020 2020 2020 2020  ting[2].        
+000085a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000085c0: 2020 2020 2020 2020 2020 2020 3d3d 2050              == P
+000085d0: 524f 4d50 545f 4d4f 4445 535b 2269 6e73  ROMPT_MODES["ins
+000085e0: 6572 7422 5d0a 2020 2020 2020 2020 2020  ert"].          
+000085f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008610: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+00008620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008640: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00008650: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
+00008660: 6973 742e 696e 7365 7274 280a 2020 2020  ist.insert(.    
 00008670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008680: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00008680: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086a0: 2020 2020 2020 2020 2020 2063 203d 2063             c = c
-000086b0: 6872 2863 290a 2020 2020 2020 2020 2020  hr(c).          
+000086a0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+000086b0: 742e 7363 726f 6c6c 6572 2e70 6f73 0a20  t.scroller.pos. 
 000086c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000086d0: 2020 2020 2020 6966 2063 2069 6e20 225c        if c in "\
-000086e0: 725c 6e22 3a0a 2020 2020 2020 2020 2020  r\n":.          
-000086f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008700: 2020 2020 2020 2020 2020 2320 7079 6c69            # pyli
-00008710: 6e74 3a20 6469 7361 626c 653d 756e 7375  nt: disable=unsu
-00008720: 6273 6372 6970 7461 626c 652d 6f62 6a65  bscriptable-obje
-00008730: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
+000086d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000086f0: 2020 2020 2020 202b 2031 2c0a 2020 2020         + 1,.    
+00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008730: 2020 2020 6465 7461 696c 732c 0a20 2020      details,.   
 00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008750: 2020 2020 2020 2069 6620 706c 6179 6572         if player
-00008760: 5f6f 7574 7075 742e 6164 6469 6e67 5f73  _output.adding_s
-00008770: 6f6e 675b 305d 2e69 736e 756d 6572 6963  ong[0].isnumeric
-00008780: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00008750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008770: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00008780: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087a0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000087b0: 6465 7461 696c 7320 696e 2070 6c61 7965  details in playe
-000087c0: 725f 6f75 7470 7574 2e70 6c61 796c 6973  r_output.playlis
-000087d0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-000087e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00008800: 6620 696e 7428 6465 7461 696c 735b 305d  f int(details[0]
-00008810: 2920 3d3d 2069 6e74 280a 2020 2020 2020  ) == int(.      
+000087a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000087b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000087d0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+000087e0: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
+000087f0: 6973 742e 6170 7065 6e64 280a 2020 2020  ist.append(.    
+00008800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008840: 2020 2020 2020 2020 2020 706c 6179 6572            player
-00008850: 5f6f 7574 7075 742e 6164 6469 6e67 5f73  _output.adding_s
-00008860: 6f6e 675b 305d 0a20 2020 2020 2020 2020  ong[0].         
-00008870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008830: 2020 2020 6465 7461 696c 730a 2020 2020      details.    
+00008840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008870: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
 00008880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008890: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-000088a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088a0: 2020 6966 206c 6f6f 703a 0a20 2020 2020    if loop:.     
 000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088c0: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000088c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000088d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000088e0: 6620 7265 7368 7566 666c 653a 0a20 2020  f reshuffle:.   
+000088f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008920: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
-00008930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008920: 2020 2020 206e 6578 745f 706c 6179 6c69       next_playli
+00008930: 7374 2e69 6e73 6572 7428 0a20 2020 2020  st.insert(.     
 00008940: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008960: 2053 4f4e 4753 5f49 4e46 4f5f 5041 5448   SONGS_INFO_PATH
-00008970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008970: 2020 2020 2020 2072 616e 6469 6e74 280a         randint(.
 00008980: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089a0: 2020 2272 222c 0a20 2020 2020 2020 2020    "r",.         
+000089a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000089b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089d0: 2020 2020 2020 2065 6e63 6f64 696e 673d         encoding=
-000089e0: 2275 7466 2d38 222c 0a20 2020 2020 2020  "utf-8",.       
+000089c0: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
+000089d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000089f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a10: 2020 2020 2029 2061 7320 736f 6e67 735f       ) as songs_
-00008a20: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+00008a00: 2020 206c 656e 280a 2020 2020 2020 2020     len(.        
+00008a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a50: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
-00008a60: 6e20 736f 6e67 735f 6669 6c65 3a0a 2020  n songs_file:.  
+00008a40: 2020 2020 2020 2020 2020 2020 6e65 7874              next
+00008a50: 5f70 6c61 796c 6973 740a 2020 2020 2020  _playlist.      
+00008a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008aa0: 2020 6465 7461 696c 7320 3d20 280a 2020    details = (.  
+00008a90: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ae0: 2020 2020 2020 6c69 6e65 2e73 7472 6970        line.strip
-00008af0: 2829 2e73 706c 6974 2822 7c22 290a 2020  ().split("|").  
+00008ad0: 2020 2020 2020 2020 2020 2020 2d20 312c              - 1,
+00008ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b10: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
 00008b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b30: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00008b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b60: 2020 2020 2020 2020 736f 6e67 5f69 6420          song_id 
-00008b70: 3d20 696e 7428 6465 7461 696c 735b 305d  = int(details[0]
-00008b80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00008b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b50: 2020 2020 2020 2020 2020 2020 6465 7461              deta
+00008b60: 696c 732c 0a20 2020 2020 2020 2020 2020  ils,.           
+00008b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b90: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
 00008ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008bb0: 2020 2020 2020 6966 2073 6f6e 675f 6964        if song_id
-00008bc0: 203d 3d20 696e 7428 0a20 2020 2020 2020   == int(.       
-00008bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bd0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
 00008be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c00: 2070 6c61 7965 725f 6f75 7470 7574 2e61   player_output.a
-00008c10: 6464 696e 675f 736f 6e67 5b0a 2020 2020  dding_song[.    
+00008c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c10: 2069 6620 280a 2020 2020 2020 2020 2020   if (.          
 00008c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c50: 2020 2020 2020 2020 300a 2020 2020 2020          0.      
-00008c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c50: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+00008c60: 7072 6f6d 7074 696e 675b 0a20 2020 2020  prompting[.     
 00008c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008c90: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
-00008ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ca0: 2020 2020 2020 2020 2020 2032 0a20 2020             2.   
 00008cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008cc0: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
+00008cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ce0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
 00008cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d00: 2020 2069 6620 706c 6179 6572 5f6f 7574     if player_out
-00008d10: 7075 742e 6164 6469 6e67 5f73 6f6e 675b  put.adding_song[
-00008d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008d20: 2020 2020 2020 203d 3d20 5052 4f4d 5054         == PROMPT
+00008d30: 5f4d 4f44 4553 5b0a 2020 2020 2020 2020  _MODES[.        
 00008d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d50: 2020 2020 2020 2020 2020 2020 2032 0a20               2. 
+00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d90: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
+00008d70: 2020 2020 2020 2020 2269 6e73 6572 7422          "insert"
+00008d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008db0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
 00008dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dd0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
-00008de0: 7075 742e 706c 6179 6c69 7374 2e69 6e73  put.playlist.ins
-00008df0: 6572 7428 0a20 2020 2020 2020 2020 2020  ert(.           
+00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008df0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
 00008e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e30: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-00008e40: 7574 2e69 0a20 2020 2020 2020 2020 2020  ut.i.           
+00008e30: 2020 2020 2020 6e65 7874 5f70 6c61 796c        next_playl
+00008e40: 6973 742e 696e 7365 7274 280a 2020 2020  ist.insert(.    
 00008e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e80: 2020 2020 202b 2031 2c0a 2020 2020 2020       + 1,.      
-00008e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008e80: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00008e90: 6572 5f6f 7574 7075 742e 7363 726f 6c6c  er_output.scroll
+00008ea0: 6572 2e70 6f73 0a20 2020 2020 2020 2020  er.pos.         
 00008eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008ec0: 2020 2020 2020 2020 2020 6465 7461 696c            detail
-00008ed0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00008ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ee0: 2020 2020 2020 202b 2031 2c0a 2020 2020         + 1,.    
 00008ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f00: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00008f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f40: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00008f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f20: 2020 2020 2020 2020 2020 2020 6465 7461              deta
+00008f30: 696c 732c 0a20 2020 2020 2020 2020 2020  ils,.           
+00008f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f80: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00008f90: 725f 6f75 7470 7574 2e70 6c61 796c 6973  r_output.playlis
-00008fa0: 742e 6170 7065 6e64 280a 2020 2020 2020  t.append(.      
-00008fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f70: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fa0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00008fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00008fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00008fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008fe0: 2020 2020 2020 2020 2020 6465 7461 696c            detail
-00008ff0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-00009000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008fe0: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+00008ff0: 745f 706c 6179 6c69 7374 2e61 7070 656e  t_playlist.appen
+00009000: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
 00009010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009020: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00009020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009040: 2020 2064 6574 6169 6c73 0a20 2020 2020     details.     
 00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009060: 2020 2020 2020 2020 6966 206c 6f6f 703a          if loop:
-00009070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009080: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
 00009090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000090b0: 7265 7368 7566 666c 653a 0a20 2020 2020  reshuffle:.     
-000090c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000090b0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+000090c0: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
+000090d0: 6e75 6d5f 6c69 6e65 7320 2b3d 2028 0a20  num_lines += (. 
 000090e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000090f0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-00009100: 706c 6179 6c69 7374 2e69 6e73 6572 7428  playlist.insert(
-00009110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000090f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009110: 2020 2031 0a20 2020 2020 2020 2020 2020     1.           
 00009120: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009150: 2020 2020 2072 616e 6469 6e74 280a 2020       randint(.  
+00009140: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091a0: 2020 2020 2020 302c 0a20 2020 2020 2020        0,.       
+00009170: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00009180: 7470 7574 2e70 726f 6d70 7469 6e67 203d  tput.prompting =
+00009190: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+000091a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000091b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091c0: 2020 2020 2020 6375 7273 6573 2e63 7572        curses.cur
+000091d0: 735f 7365 7428 4661 6c73 6529 0a20 2020  s_set(False).   
 000091e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091f0: 206c 656e 280a 2020 2020 2020 2020 2020   len(.          
-00009200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009200: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+00009210: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
+00009220: 6c65 722e 7265 7369 7a65 280a 2020 2020  ler.resize(.    
 00009230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009240: 2020 6e65 7874 5f70 6c61 796c 6973 740a    next_playlist.
+00009240: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009260: 7363 7265 656e 5f73 697a 655b 305d 202d  screen_size[0] -
+00009270: 2032 0a20 2020 2020 2020 2020 2020 2020   2.             
 00009280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009290: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000092a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000092a0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
 000092b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000092c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000092e0: 2020 2d20 312c 0a20 2020 2020 2020 2020    - 1,.         
+000092d0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+000092e0: 7574 2e6f 7574 7075 7428 0a20 2020 2020  ut.output(.     
 000092f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009320: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00009330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009310: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00009320: 6c61 7962 6163 6b2e 6375 7272 5f70 6f73  layback.curr_pos
+00009330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00009340: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009370: 2020 6465 7461 696c 732c 0a20 2020 2020    details,.     
+00009360: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00009370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009390: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
 000093a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000093b0: 2020 2020 2065 6c69 6620 280a 2020 2020       elif (.    
 000093c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000093f0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00009400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093d0: 2020 2020 2020 2020 2020 2020 227c 2220              "|" 
+000093e0: 6e6f 7420 696e 2070 6c61 7965 725f 6f75  not in player_ou
+000093f0: 7470 7574 2e70 726f 6d70 7469 6e67 5b30  tput.prompting[0
+00009400: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
 00009410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009430: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00009440: 6620 706c 6179 6572 5f6f 7574 7075 742e  f player_output.
-00009450: 6164 6469 6e67 5f73 6f6e 675b 0a20 2020  adding_song[.   
-00009460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009420: 2020 616e 6420 706c 6179 6572 5f6f 7574    and player_out
+00009430: 7075 742e 7072 6f6d 7074 696e 675b 325d  put.prompting[2]
+00009440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009460: 203d 3d20 5052 4f4d 5054 5f4d 4f44 4553   == PROMPT_MODES
+00009470: 5b22 7461 6722 5d0a 2020 2020 2020 2020  ["tag"].        
 00009480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094a0: 2032 0a20 2020 2020 2020 2020 2020 2020   2.             
-000094b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094e0: 2020 205d 3a0a 2020 2020 2020 2020 2020     ]:.          
+00009490: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+000094a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000094b0: 2020 2020 2020 2074 6167 7320 3d20 706c         tags = pl
+000094c0: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
+000094d0: 7074 696e 675b 305d 2e73 706c 6974 2822  pting[0].split("
+000094e0: 2c22 290a 0a20 2020 2020 2020 2020 2020  ,")..           
 000094f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009520: 2020 2020 2020 2020 2020 6e65 7874 5f70            next_p
-00009530: 6c61 796c 6973 742e 696e 7365 7274 280a  laylist.insert(.
-00009540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009500: 2020 2020 2074 6167 6769 6e67 5f69 6473       tagging_ids
+00009510: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
+00009520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009530: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00009540: 616e 6765 286c 656e 2870 6c61 7965 725f  ange(len(player_
+00009550: 6f75 7470 7574 2e70 6c61 796c 6973 7429  output.playlist)
+00009560: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
 00009570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009580: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00009590: 7574 7075 742e 690a 2020 2020 2020 2020  utput.i.        
+00009580: 2020 2020 2020 2074 6167 6769 6e67 5f69         tagging_i
+00009590: 6473 5b0a 2020 2020 2020 2020 2020 2020  ds[.            
 000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095e0: 2b20 312c 0a20 2020 2020 2020 2020 2020  + 1,.           
+000095b0: 2020 2020 2020 2020 2020 2020 696e 7428              int(
+000095c0: 706c 6179 6572 5f6f 7574 7075 742e 706c  player_output.pl
+000095d0: 6179 6c69 7374 5b69 5d5b 305d 290a 2020  aylist[i][0]).  
+000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000095f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009600: 2020 5d20 3d20 690a 0a20 2020 2020 2020    ] = i..       
 00009610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009620: 2020 2020 2020 2020 2020 2020 2064 6574               det
-00009630: 6169 6c73 2c0a 2020 2020 2020 2020 2020  ails,.          
+00009620: 2020 2020 2020 2020 2073 6f6e 6773 5f66           songs_f
+00009630: 696c 6520 3d20 6f70 656e 280a 2020 2020  ile = open(.    
 00009640: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009670: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00009680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009660: 534f 4e47 535f 494e 464f 5f50 4154 482c  SONGS_INFO_PATH,
+00009670: 2022 7222 2c20 656e 636f 6469 6e67 3d22   "r", encoding="
+00009680: 7574 662d 3822 0a20 2020 2020 2020 2020  utf-8".         
 00009690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096b0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000096c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000096d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000096b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096c0: 2020 2020 2020 2020 206c 696e 6573 203d           lines =
+000096d0: 2073 6f6e 6773 5f66 696c 652e 7265 6164   songs_file.read
+000096e0: 2829 2e73 706c 6974 6c69 6e65 7328 290a  ().splitlines().
 000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009700: 2020 2020 2020 6e65 7874 5f70 6c61 796c        next_playl
-00009710: 6973 742e 6170 7065 6e64 280a 2020 2020  ist.append(.    
-00009720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009710: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
+00009720: 656e 286c 696e 6573 2929 3a0a 2020 2020  en(lines)):.    
 00009730: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009760: 2020 2020 6465 7461 696c 730a 2020 2020      details.    
-00009770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009750: 6465 7461 696c 7320 3d20 6c69 6e65 735b  details = lines[
+00009760: 695d 2e73 7472 6970 2829 2e73 706c 6974  i].strip().split
+00009770: 2822 7c22 290a 2020 2020 2020 2020 2020  ("|").          
 00009780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009790: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
+000097a0: 6420 3d20 696e 7428 6465 7461 696c 735b  d = int(details[
+000097b0: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
 000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097e0: 2020 2020 2020 2020 2020 706c 6179 6572            player
-000097f0: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
-00009800: 2e6e 756d 5f6c 696e 6573 202b 3d20 280a  .num_lines += (.
-00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097d0: 2020 2020 2020 2020 6966 2073 6f6e 675f          if song_
+000097e0: 6964 2069 6e20 7461 6767 696e 675f 6964  id in tagging_id
+000097f0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00009800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009810: 2020 2020 2020 2020 2020 2069 6620 6465             if de
+00009820: 7461 696c 735b 325d 3a0a 2020 2020 2020  tails[2]:.      
 00009830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009840: 2020 2020 2020 2020 2020 2020 310a 2020              1.  
-00009850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009880: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00009890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009850: 2020 2020 2020 6e65 775f 7461 6773 203d        new_tags =
+00009860: 2064 6574 6169 6c73 5b32 5d2e 7370 6c69   details[2].spli
+00009870: 7428 222c 2229 0a20 2020 2020 2020 2020  t(",").         
+00009880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009890: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+000098a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
 000098b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000098c0: 706c 6179 6572 5f6f 7574 7075 742e 6164  player_output.ad
-000098d0: 6469 6e67 5f73 6f6e 6720 3d20 280a 2020  ding_song = (.  
+000098c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000098d0: 206e 6577 5f74 6167 7320 3d20 5b5d 0a20   new_tags = []. 
 000098e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000098f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009910: 2020 2020 2020 2020 2020 4e6f 6e65 0a20            None. 
+00009900: 2020 2020 2020 206e 6577 5f74 6167 7320         new_tags 
+00009910: 2b3d 205b 0a20 2020 2020 2020 2020 2020  += [.           
 00009920: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009950: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00009940: 2074 6167 0a20 2020 2020 2020 2020 2020   tag.           
+00009950: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009990: 2063 7572 7365 732e 6375 7273 5f73 6574   curses.curs_set
-000099a0: 2846 616c 7365 290a 2020 2020 2020 2020  (False).        
-000099b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009970: 2066 6f72 2074 6167 2069 6e20 7461 6773   for tag in tags
+00009980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000099a0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000099b0: 7461 6720 6e6f 7420 696e 206e 6577 5f74  tag not in new_t
+000099c0: 6167 730a 2020 2020 2020 2020 2020 2020  ags.            
 000099d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000099e0: 706c 6179 6572 5f6f 7574 7075 742e 7363  player_output.sc
-000099f0: 726f 6c6c 6572 2e72 6573 697a 6528 0a20  roller.resize(. 
+000099e0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+000099f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a30: 2020 2020 2020 2020 2020 2073 6372 6565             scree
-00009a40: 6e5f 7369 7a65 5b30 5d20 2d20 320a 2020  n_size[0] - 2.  
-00009a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009a80: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00009a10: 2020 2020 2020 6465 7461 696c 735b 325d        details[2]
+00009a20: 203d 2022 2c22 2e6a 6f69 6e28 6e65 775f   = ",".join(new_
+00009a30: 7461 6773 290a 2020 2020 2020 2020 2020  tags).          
+00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a50: 2020 2020 2020 2020 2020 2020 2020 6c69                li
+00009a60: 6e65 735b 695d 203d 2022 7c22 2e6a 6f69  nes[i] = "|".joi
+00009a70: 6e28 6465 7461 696c 7329 0a20 2020 2020  n(details).     
+00009a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00009a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ac0: 706c 6179 6572 5f6f 7574 7075 742e 6f75  player_output.ou
-00009ad0: 7470 7574 280a 2020 2020 2020 2020 2020  tput(.          
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009aa0: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+00009ab0: 2e70 6c61 796c 6973 745b 0a20 2020 2020  .playlist[.     
+00009ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ae0: 2020 2020 2020 2074 6167 6769 6e67 5f69         tagging_i
+00009af0: 6473 5b73 6f6e 675f 6964 5d0a 2020 2020  ds[song_id].    
 00009b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b10: 2020 706c 6179 6261 636b 2e63 7572 725f    playback.curr_
-00009b20: 706f 730a 2020 2020 2020 2020 2020 2020  pos.            
-00009b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b20: 2020 2020 5d5b 325d 203d 2064 6574 6169      ][2] = detai
+00009b30: 6c73 5b32 5d0a 2020 2020 2020 2020 2020  ls[2].          
 00009b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b50: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00009b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b50: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
+00009b60: 2e63 6c6f 7365 2829 0a0a 2020 2020 2020  .close()..      
 00009b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009b90: 2020 2020 2020 6272 6561 6b0a 2020 2020        break.    
+00009b80: 2020 2020 2020 2020 2020 736f 6e67 735f            songs_
+00009b90: 6669 6c65 203d 206f 7065 6e28 0a20 2020  file = open(.   
 00009ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bb0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00009bc0: 2063 2069 6e20 225c 625c 7837 6622 3a0a   c in "\b\x7f":.
-00009bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bf0: 2020 2020 2320 7079 6c69 6e74 3a20 6469      # pylint: di
-00009c00: 7361 626c 653d 756e 7375 6273 6372 6970  sable=unsubscrip
-00009c10: 7461 626c 652d 6f62 6a65 6374 0a20 2020  table-object.   
-00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c40: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
-00009c50: 742e 6164 6469 6e67 5f73 6f6e 675b 315d  t.adding_song[1]
-00009c60: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c80: 2020 2020 2020 2020 2020 2020 2020 706c                pl
-00009c90: 6179 6572 5f6f 7574 7075 742e 6164 6469  ayer_output.addi
-00009ca0: 6e67 5f73 6f6e 6720 3d20 280a 2020 2020  ng_song = (.    
-00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bc0: 2053 4f4e 4753 5f49 4e46 4f5f 5041 5448   SONGS_INFO_PATH
+00009bd0: 2c20 2277 222c 2065 6e63 6f64 696e 673d  , "w", encoding=
+00009be0: 2275 7466 2d38 220a 2020 2020 2020 2020  "utf-8".        
+00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c20: 2020 2020 2020 2020 2020 736f 6e67 735f            songs_
+00009c30: 6669 6c65 2e77 7269 7465 2822 5c6e 222e  file.write("\n".
+00009c40: 6a6f 696e 286c 696e 6573 2929 0a20 2020  join(lines)).   
+00009c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c60: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
+00009c70: 6773 5f66 696c 652e 636c 6f73 6528 290a  gs_file.close().
+00009c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ca0: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+00009cb0: 726f 6d70 7469 6e67 203d 204e 6f6e 650a  rompting = None.
 00009cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009cd0: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
-00009ce0: 7574 7075 742e 6164 6469 6e67 5f73 6f6e  utput.adding_son
-00009cf0: 675b 305d 5b0a 2020 2020 2020 2020 2020  g[0][.          
+00009cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ce0: 6375 7273 6573 2e63 7572 735f 7365 7428  curses.curs_set(
+00009cf0: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
 00009d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d20: 2020 2020 2020 3a20 706c 6179 6572 5f6f        : player_o
-00009d30: 7574 7075 742e 6164 6469 6e67 5f73 6f6e  utput.adding_son
-00009d40: 675b 315d 0a20 2020 2020 2020 2020 2020  g[1].           
-00009d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d70: 2020 2020 202d 2031 0a20 2020 2020 2020       - 1.       
-00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009da0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+00009d10: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
+00009d20: 7470 7574 2e6f 7574 7075 7428 706c 6179  tput.output(play
+00009d30: 6261 636b 2e63 7572 725f 706f 7329 0a20  back.curr_pos). 
+00009d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d50: 2020 2020 2020 2065 6c69 6620 6320 3d3d         elif c ==
+00009d60: 2032 373a 2020 2320 4553 4320 6b65 790a   27:  # ESC key.
+00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d80: 2020 2020 2020 2020 2020 2020 706c 6179              play
+00009d90: 6572 5f6f 7574 7075 742e 7072 6f6d 7074  er_output.prompt
+00009da0: 696e 6720 3d20 4e6f 6e65 0a20 2020 2020  ing = None.     
 00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dd0: 2020 202b 2070 6c61 7965 725f 6f75 7470     + player_outp
-00009de0: 7574 2e61 6464 696e 675f 736f 6e67 5b30  ut.adding_song[0
-00009df0: 5d5b 0a20 2020 2020 2020 2020 2020 2020  ][.             
-00009e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e20: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-00009e30: 2e61 6464 696e 675f 736f 6e67 5b31 5d20  .adding_song[1] 
-00009e40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e60: 2020 2020 2020 2020 2020 2020 2020 5d2c                ],
-00009e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e90: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-00009ea0: 7965 725f 6f75 7470 7574 2e61 6464 696e  yer_output.addin
-00009eb0: 675f 736f 6e67 5b31 5d20 2d20 312c 0a20  g_song[1] - 1,. 
-00009ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ee0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-00009ef0: 725f 6f75 7470 7574 2e61 6464 696e 675f  r_output.adding_
-00009f00: 736f 6e67 5b32 5d2c 0a20 2020 2020 2020  song[2],.       
+00009dc0: 2020 2020 2020 2063 7572 7365 732e 6375         curses.cu
+00009dd0: 7273 5f73 6574 2846 616c 7365 290a 2020  rs_set(False).  
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009df0: 2020 2020 2020 2020 2020 706c 6179 6572            player
+00009e00: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
+00009e10: 2e72 6573 697a 6528 7363 7265 656e 5f73  .resize(screen_s
+00009e20: 697a 655b 305d 202d 2032 290a 2020 2020  ize[0] - 2).    
+00009e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e40: 2020 2020 2020 2020 706c 6179 6572 5f6f          player_o
+00009e50: 7574 7075 742e 6f75 7470 7574 2870 6c61  utput.output(pla
+00009e60: 7962 6163 6b2e 6375 7272 5f70 6f73 290a  yback.curr_pos).
+00009e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e80: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00009e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ea0: 2020 2020 2020 2020 2020 7472 793a 0a20            try:. 
+00009eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ec0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00009ed0: 203d 2063 6872 2863 290a 2020 2020 2020   = chr(c).      
+00009ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ef0: 2020 2020 2020 2020 2020 6966 2063 2069            if c i
+00009f00: 6e20 225c 725c 6e22 3a0a 2020 2020 2020  n "\r\n":.      
 00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f30: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-00009f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f50: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-00009f60: 7470 7574 2e6f 7574 7075 7428 706c 6179  tput.output(play
-00009f70: 6261 636b 2e63 7572 725f 706f 7329 0a20  back.curr_pos). 
-00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00009fa0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00009fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009fc0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-00009fd0: 6f75 7470 7574 2e61 6464 696e 675f 736f  output.adding_so
-00009fe0: 6e67 203d 2028 0a20 2020 2020 2020 2020  ng = (.         
-00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a000: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000a010: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
-0000a020: 3d75 6e73 7562 7363 7269 7074 6162 6c65  =unsubscriptable
-0000a030: 2d6f 626a 6563 740a 2020 2020 2020 2020  -object.        
+00009f20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00009f30: 7079 6c69 6e74 3a20 6469 7361 626c 653d  pylint: disable=
+00009f40: 756e 7375 6273 6372 6970 7461 626c 652d  unsubscriptable-
+00009f50: 6f62 6a65 6374 0a20 2020 2020 2020 2020  object.         
+00009f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f70: 2020 2020 2020 2020 2020 2069 6620 706c             if pl
+00009f80: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
+00009f90: 7074 696e 675b 0a20 2020 2020 2020 2020  pting[.         
+00009fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fb0: 2020 2020 2020 2020 2020 2020 2020 2030                 0
+00009fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009fe0: 2020 2020 205d 2e69 736e 756d 6572 6963       ].isnumeric
+00009ff0: 2829 2061 6e64 2070 6c61 7965 725f 6f75  () and player_ou
+0000a000: 7470 7574 2e70 726f 6d70 7469 6e67 5b0a  tput.prompting[.
+0000a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a030: 2020 2020 2020 2020 320a 2020 2020 2020          2.      
 0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a060: 706c 6179 6572 5f6f 7574 7075 742e 6164  player_output.ad
-0000a070: 6469 6e67 5f73 6f6e 675b 305d 5b0a 2020  ding_song[0][.  
-0000a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0a0: 2020 2020 2020 2020 2020 3a20 706c 6179            : play
-0000a0b0: 6572 5f6f 7574 7075 742e 6164 6469 6e67  er_output.adding
-0000a0c0: 5f73 6f6e 675b 315d 0a20 2020 2020 2020  _song[1].       
-0000a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0f0: 205d 0a20 2020 2020 2020 2020 2020 2020   ].             
-0000a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a110: 2020 2020 2020 2020 2020 202b 2063 0a20             + c. 
+0000a050: 2020 2020 2020 2020 2020 2020 2020 5d20                ] 
+0000a060: 696e 2028 0a20 2020 2020 2020 2020 2020  in (.           
+0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a080: 2020 2020 2020 2020 2020 2020 2050 524f               PRO
+0000a090: 4d50 545f 4d4f 4445 535b 2261 6464 225d  MPT_MODES["add"]
+0000a0a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0c0: 2020 2020 2020 2020 2020 5052 4f4d 5054            PROMPT
+0000a0d0: 5f4d 4f44 4553 5b22 696e 7365 7274 225d  _MODES["insert"]
+0000a0e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a100: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+0000a110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a140: 2020 2020 2020 202b 2070 6c61 7965 725f         + player_
-0000a150: 6f75 7470 7574 2e61 6464 696e 675f 736f  output.adding_so
-0000a160: 6e67 5b30 5d5b 0a20 2020 2020 2020 2020  ng[0][.         
+0000a130: 2066 6f72 2064 6574 6169 6c73 2069 6e20   for details in 
+0000a140: 706c 6179 6572 5f6f 7574 7075 742e 706c  player_output.pl
+0000a150: 6179 6c69 7374 3a0a 2020 2020 2020 2020  aylist:.        
+0000a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a190: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-0000a1a0: 2e61 6464 696e 675f 736f 6e67 5b31 5d20  .adding_song[1] 
-0000a1b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a1d0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
-0000a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a180: 2020 2020 6966 2069 6e74 2864 6574 6169      if int(detai
+0000a190: 6c73 5b30 5d29 203d 3d20 696e 7428 0a20  ls[0]) == int(. 
+0000a1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a1c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000a1d0: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
+0000a1e0: 6d70 7469 6e67 5b30 5d0a 2020 2020 2020  mpting[0].      
 0000a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a200: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
-0000a210: 7574 2e61 6464 696e 675f 736f 6e67 5b31  ut.adding_song[1
-0000a220: 5d20 2b20 312c 0a20 2020 2020 2020 2020  ] + 1,.         
+0000a200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a210: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+0000a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a240: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000a250: 6c61 7965 725f 6f75 7470 7574 2e61 6464  layer_output.add
-0000a260: 696e 675f 736f 6e67 5b32 5d2c 0a20 2020  ing_song[2],.   
-0000a270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a240: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+0000a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a270: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
 0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a290: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2b0: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-0000a2c0: 7470 7574 2e6f 7574 7075 7428 706c 6179  tput.output(play
-0000a2d0: 6261 636b 2e63 7572 725f 706f 7329 0a20  back.curr_pos). 
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2f0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-0000a300: 7420 2856 616c 7565 4572 726f 722c 204f  t (ValueError, O
-0000a310: 7665 7266 6c6f 7745 7272 6f72 293a 0a20  verflowError):. 
-0000a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a330: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000a340: 6173 730a 0a20 2020 2020 2020 2020 2020  ass..           
-0000a350: 2069 6620 7379 732e 706c 6174 666f 726d   if sys.platform
-0000a360: 203d 3d20 2264 6172 7769 6e22 2061 6e64   == "darwin" and
-0000a370: 2063 616e 5f6d 6163 5f6e 6f77 5f70 6c61   can_mac_now_pla
-0000a380: 7969 6e67 3a0a 2020 2020 2020 2020 2020  ying:.          
-0000a390: 2020 2020 2020 6966 2061 6273 286d 6163        if abs(mac
-0000a3a0: 5f6e 6f77 5f70 6c61 7969 6e67 2e70 6f73  _now_playing.pos
-0000a3b0: 202d 2070 6c61 7962 6163 6b2e 6375 7272   - playback.curr
-0000a3c0: 5f70 6f73 2920 3e20 323a 0a20 2020 2020  _pos) > 2:.     
-0000a3d0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000a3e0: 6c61 7962 6163 6b2e 7365 656b 286d 6163  layback.seek(mac
-0000a3f0: 5f6e 6f77 5f70 6c61 7969 6e67 2e70 6f73  _now_playing.pos
-0000a400: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a410: 2020 2020 2020 6c61 7374 5f74 696d 6573        last_times
-0000a420: 7461 6d70 203d 206d 6163 5f6e 6f77 5f70  tamp = mac_now_p
-0000a430: 6c61 7969 6e67 2e70 6f73 0a20 2020 2020  laying.pos.     
-0000a440: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0000a450: 7064 6174 655f 6e6f 775f 706c 6179 696e  pdate_now_playin
-0000a460: 6720 3d20 5472 7565 0a20 2020 2020 2020  g = True.       
-0000a470: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
-0000a480: 7965 725f 6f75 7470 7574 2e6f 7574 7075  yer_output.outpu
-0000a490: 7428 706c 6179 6261 636b 2e63 7572 725f  t(playback.curr_
-0000a4a0: 706f 7329 0a20 2020 2020 2020 2020 2020  pos).           
-0000a4b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000a4d0: 6163 5f6e 6f77 5f70 6c61 7969 6e67 2e70  ac_now_playing.p
-0000a4e0: 6f73 203d 2072 6f75 6e64 2870 6c61 7962  os = round(playb
-0000a4f0: 6163 6b2e 6375 7272 5f70 6f73 290a 0a20  ack.curr_pos).. 
-0000a500: 2020 2020 2020 2020 2020 2070 726f 6772             progr
-0000a510: 6573 735f 6261 725f 7769 6474 6820 3d20  ess_bar_width = 
-0000a520: 7374 6473 6372 2e67 6574 6d61 7879 7828  stdscr.getmaxyx(
-0000a530: 295b 315d 202d 2031 380a 2020 2020 2020  )[1] - 18.      
-0000a540: 2020 2020 2020 6672 616d 655f 6475 7261        frame_dura
-0000a550: 7469 6f6e 203d 206d 696e 280a 2020 2020  tion = min(.    
-0000a560: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
+0000a290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2a0: 2020 2020 2020 2020 2077 6974 6820 6f70           with op
+0000a2b0: 656e 280a 2020 2020 2020 2020 2020 2020  en(.            
+0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2e0: 2020 2020 534f 4e47 535f 494e 464f 5f50      SONGS_INFO_P
+0000a2f0: 4154 482c 0a20 2020 2020 2020 2020 2020  ATH,.           
+0000a300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a320: 2020 2020 2022 7222 2c0a 2020 2020 2020       "r",.      
+0000a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a350: 2020 2020 2020 2020 2020 656e 636f 6469            encodi
+0000a360: 6e67 3d22 7574 662d 3822 2c0a 2020 2020  ng="utf-8",.    
+0000a370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a390: 2020 2020 2020 2020 2920 6173 2073 6f6e          ) as son
+0000a3a0: 6773 5f66 696c 653a 0a20 2020 2020 2020  gs_file:.       
+0000a3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a3d0: 2020 2020 2020 2020 2066 6f72 206c 696e           for lin
+0000a3e0: 6520 696e 2073 6f6e 6773 5f66 696c 653a  e in songs_file:
+0000a3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a420: 2020 2020 2064 6574 6169 6c73 203d 2028       details = (
+0000a430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a460: 2020 2020 2020 2020 206c 696e 652e 7374           line.st
+0000a470: 7269 7028 292e 7370 6c69 7428 227c 2229  rip().split("|")
+0000a480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4b0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4e0: 2020 2020 2020 2020 2020 2073 6f6e 675f             song_
+0000a4f0: 6964 203d 2069 6e74 2864 6574 6169 6c73  id = int(details
+0000a500: 5b30 5d29 0a20 2020 2020 2020 2020 2020  [0]).           
+0000a510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a530: 2020 2020 2020 2020 2069 6620 736f 6e67           if song
+0000a540: 5f69 6420 3d3d 2069 6e74 280a 2020 2020  _id == int(.    
+0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a580: 2020 310a 2020 2020 2020 2020 2020 2020    1.            
-0000a590: 2020 2020 2020 2020 6966 2070 726f 6772          if progr
-0000a5a0: 6573 735f 6261 725f 7769 6474 6820 3c20  ess_bar_width < 
-0000a5b0: 4d49 4e5f 5052 4f47 5245 5353 5f42 4152  MIN_PROGRESS_BAR
-0000a5c0: 5f57 4944 5448 0a20 2020 2020 2020 2020  _WIDTH.         
-0000a5d0: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-0000a5e0: 706c 6179 6572 5f6f 7574 7075 742e 6475  player_output.du
-0000a5f0: 7261 7469 6f6e 202f 2028 7072 6f67 7265  ration / (progre
-0000a600: 7373 5f62 6172 5f77 6964 7468 202a 2038  ss_bar_width * 8
-0000a610: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a620: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-0000a630: 2020 2020 2031 202f 2046 5053 2069 6620       1 / FPS if 
-0000a640: 706c 6179 6572 5f6f 7574 7075 742e 7669  player_output.vi
-0000a650: 7375 616c 697a 6520 656c 7365 2031 2c0a  sualize else 1,.
-0000a660: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000a670: 2020 2020 2020 2020 2020 6966 2061 6273            if abs
-0000a680: 2870 6c61 7962 6163 6b2e 6375 7272 5f70  (playback.curr_p
-0000a690: 6f73 202d 206c 6173 745f 7469 6d65 7374  os - last_timest
-0000a6a0: 616d 7029 203e 2066 7261 6d65 5f64 7572  amp) > frame_dur
-0000a6b0: 6174 696f 6e3a 0a20 2020 2020 2020 2020  ation:.         
-0000a6c0: 2020 2020 2020 206c 6173 745f 7469 6d65         last_time
-0000a6d0: 7374 616d 7020 3d20 706c 6179 6261 636b  stamp = playback
-0000a6e0: 2e63 7572 725f 706f 730a 2020 2020 2020  .curr_pos.      
-0000a6f0: 2020 2020 2020 2020 2020 706c 6179 6572            player
-0000a700: 5f6f 7574 7075 742e 6f75 7470 7574 2870  _output.output(p
-0000a710: 6c61 7962 6163 6b2e 6375 7272 5f70 6f73  layback.curr_pos
-0000a720: 290a 0a20 2020 2020 2020 2023 2072 6567  )..        # reg
-0000a730: 696f 6e20 7374 6174 730a 2020 2020 2020  ion stats.      
-0000a740: 2020 7469 6d65 5f6c 6973 7465 6e65 6420    time_listened 
-0000a750: 3d20 7469 6d65 2829 202d 2073 7461 7274  = time() - start
-0000a760: 5f74 696d 650a 2020 2020 2020 2020 6966  _time.        if
-0000a770: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
-0000a780: 6175 7365 643a 0a20 2020 2020 2020 2020  aused:.         
-0000a790: 2020 2074 696d 655f 6c69 7374 656e 6564     time_listened
-0000a7a0: 202d 3d20 7469 6d65 2829 202d 2070 6175   -= time() - pau
-0000a7b0: 7365 5f73 7461 7274 0a0a 2020 2020 2020  se_start..      
-0000a7c0: 2020 7769 7468 206f 7065 6e28 544f 5441    with open(TOTA
-0000a7d0: 4c5f 5354 4154 535f 5041 5448 2c20 2272  L_STATS_PATH, "r
-0000a7e0: 2b22 2c20 656e 636f 6469 6e67 3d22 7574  +", encoding="ut
-0000a7f0: 662d 3822 2920 6173 2073 7461 7473 5f66  f-8") as stats_f
-0000a800: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
-0000a810: 206c 696e 6573 203d 2073 7461 7473 5f66   lines = stats_f
-0000a820: 696c 652e 7265 6164 6c69 6e65 7328 290a  ile.readlines().
-0000a830: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000a840: 6a20 696e 2072 616e 6765 286c 656e 286c  j in range(len(l
-0000a850: 696e 6573 2929 3a0a 2020 2020 2020 2020  ines)):.        
-0000a860: 2020 2020 2020 2020 736f 6e67 5f69 642c          song_id,
-0000a870: 206c 6973 7465 6e65 6420 3d20 6c69 6e65   listened = line
-0000a880: 735b 6a5d 2e73 7472 6970 2829 2e73 706c  s[j].strip().spl
-0000a890: 6974 2822 7c22 290a 2020 2020 2020 2020  it("|").        
-0000a8a0: 2020 2020 2020 2020 6966 2073 6f6e 675f          if song_
-0000a8b0: 6964 203d 3d20 706c 6179 6572 5f6f 7574  id == player_out
-0000a8c0: 7075 742e 706c 6179 6c69 7374 5b70 6c61  put.playlist[pla
-0000a8d0: 7965 725f 6f75 7470 7574 2e69 5d5b 305d  yer_output.i][0]
-0000a8e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000a8f0: 2020 2020 2020 6c69 7374 656e 6564 203d        listened =
-0000a900: 2066 6c6f 6174 286c 6973 7465 6e65 6429   float(listened)
-0000a910: 202b 2074 696d 655f 6c69 7374 656e 6564   + time_listened
-0000a920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a930: 2020 2020 206c 696e 6573 5b6a 5d20 3d20       lines[j] = 
-0000a940: 6622 7b73 6f6e 675f 6964 7d7c 7b6c 6973  f"{song_id}|{lis
-0000a950: 7465 6e65 647d 5c6e 220a 2020 2020 2020  tened}\n".      
-0000a960: 2020 2020 2020 2020 2020 2020 2020 6272                br
-0000a970: 6561 6b0a 0a20 2020 2020 2020 2020 2020  eak..           
-0000a980: 2023 2077 7269 7465 206f 7574 0a20 2020   # write out.   
-0000a990: 2020 2020 2020 2020 2073 7461 7473 5f66           stats_f
-0000a9a0: 696c 652e 7365 656b 2830 290a 2020 2020  ile.seek(0).    
-0000a9b0: 2020 2020 2020 2020 7374 6174 735f 6669          stats_fi
-0000a9c0: 6c65 2e77 7269 7465 2822 222e 6a6f 696e  le.write("".join
-0000a9d0: 286c 696e 6573 2929 0a20 2020 2020 2020  (lines)).       
-0000a9e0: 2020 2020 2073 7461 7473 5f66 696c 652e       stats_file.
-0000a9f0: 7472 756e 6361 7465 2829 0a0a 2020 2020  truncate()..    
-0000aa00: 2020 2020 7769 7468 206f 7065 6e28 4355      with open(CU
-0000aa10: 525f 5945 4152 5f53 5441 5453 5f50 4154  R_YEAR_STATS_PAT
-0000aa20: 482c 2022 722b 222c 2065 6e63 6f64 696e  H, "r+", encodin
-0000aa30: 673d 2275 7466 2d38 2229 2061 7320 7374  g="utf-8") as st
-0000aa40: 6174 735f 6669 6c65 3a0a 2020 2020 2020  ats_file:.      
-0000aa50: 2020 2020 2020 6c69 6e65 7320 3d20 7374        lines = st
-0000aa60: 6174 735f 6669 6c65 2e72 6561 646c 696e  ats_file.readlin
-0000aa70: 6573 2829 0a20 2020 2020 2020 2020 2020  es().           
-0000aa80: 2066 6f72 206a 2069 6e20 7261 6e67 6528   for j in range(
-0000aa90: 6c65 6e28 6c69 6e65 7329 293a 0a20 2020  len(lines)):.   
-0000aaa0: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
-0000aab0: 675f 6964 2c20 6c69 7374 656e 6564 203d  g_id, listened =
-0000aac0: 206c 696e 6573 5b6a 5d2e 7374 7269 7028   lines[j].strip(
-0000aad0: 292e 7370 6c69 7428 227c 2229 0a20 2020  ).split("|").   
-0000aae0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000aaf0: 736f 6e67 5f69 6420 3d3d 2070 6c61 7965  song_id == playe
-0000ab00: 725f 6f75 7470 7574 2e70 6c61 796c 6973  r_output.playlis
-0000ab10: 745b 706c 6179 6572 5f6f 7574 7075 742e  t[player_output.
-0000ab20: 695d 5b30 5d3a 0a20 2020 2020 2020 2020  i][0]:.         
-0000ab30: 2020 2020 2020 2020 2020 206c 6973 7465             liste
-0000ab40: 6e65 6420 3d20 666c 6f61 7428 6c69 7374  ned = float(list
-0000ab50: 656e 6564 2920 2b20 7469 6d65 5f6c 6973  ened) + time_lis
-0000ab60: 7465 6e65 640a 2020 2020 2020 2020 2020  tened.          
-0000ab70: 2020 2020 2020 2020 2020 6c69 6e65 735b            lines[
-0000ab80: 6a5d 203d 2066 227b 736f 6e67 5f69 647d  j] = f"{song_id}
-0000ab90: 7c7b 6c69 7374 656e 6564 7d5c 6e22 0a20  |{listened}\n". 
+0000a580: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+0000a590: 742e 7072 6f6d 7074 696e 675b 0a20 2020  t.prompting[.   
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5d0: 2020 2020 2020 2020 2030 0a20 2020 2020           0.     
+0000a5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a610: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+0000a620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a640: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+0000a650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a680: 2020 2020 736f 6e67 5f64 6174 6120 3d20      song_data = 
+0000a690: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6c0: 2020 2020 2020 2020 2020 2020 2020 6d75                mu
+0000a6d0: 7369 635f 7461 672e 6c6f 6164 5f66 696c  sic_tag.load_fil
+0000a6e0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+0000a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a720: 2020 206f 732e 7061 7468 2e6a 6f69 6e28     os.path.join(
+0000a730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a770: 2020 2020 2053 4f4e 4753 5f44 4952 2c0a       SONGS_DIR,.
+0000a780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7c0: 2020 2020 6465 7461 696c 735b 315d 2c0a      details[1],.
+0000a7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a810: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000a820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a840: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000a850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a880: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000a890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8c0: 2020 6465 7461 696c 7320 2b3d 205b 0a20    details += [. 
+0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a900: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
+0000a910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a940: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
+0000a950: 675f 6461 7461 5b0a 2020 2020 2020 2020  g_data[.        
+0000a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a990: 2020 2020 2020 2020 2020 2020 2261 7274              "art
+0000a9a0: 6973 7422 0a20 2020 2020 2020 2020 2020  ist".           
+0000a9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9e0: 2020 2020 205d 2e76 616c 7565 0a20 2020       ].value.   
+0000a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa20: 2020 2020 2020 2020 2020 2020 206f 7220               or 
+0000aa30: 2255 6e6b 6e6f 776e 2041 7274 6973 7422  "Unknown Artist"
+0000aa40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000aa50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa70: 2020 2020 2020 2020 2020 2020 2029 2c0a               ),.
+0000aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aab0: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
+0000aac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aaf0: 2020 2020 2020 2020 2020 2020 2020 736f                so
+0000ab00: 6e67 5f64 6174 615b 0a20 2020 2020 2020  ng_data[.       
+0000ab10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab40: 2020 2020 2020 2020 2020 2020 2022 616c               "al
+0000ab50: 6275 6d22 0a20 2020 2020 2020 2020 2020  bum".           
+0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab90: 2020 2020 205d 2e76 616c 7565 0a20 2020       ].value.   
 0000aba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abb0: 2020 2062 7265 616b 0a0a 2020 2020 2020     break..      
-0000abc0: 2020 2020 2020 2320 7772 6974 6520 6f75        # write ou
-0000abd0: 740a 2020 2020 2020 2020 2020 2020 7374  t.            st
-0000abe0: 6174 735f 6669 6c65 2e73 6565 6b28 3029  ats_file.seek(0)
-0000abf0: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
-0000ac00: 7473 5f66 696c 652e 7772 6974 6528 2222  ts_file.write(""
-0000ac10: 2e6a 6f69 6e28 6c69 6e65 7329 290a 2020  .join(lines)).  
-0000ac20: 2020 2020 2020 2020 2020 7374 6174 735f            stats_
-0000ac30: 6669 6c65 2e74 7275 6e63 6174 6528 290a  file.truncate().
-0000ac40: 2020 2020 2020 2020 2320 656e 6472 6567          # endreg
-0000ac50: 696f 6e0a 0a20 2020 2020 2020 2069 6620  ion..        if 
-0000ac60: 706c 6179 6572 5f6f 7574 7075 742e 656e  player_output.en
-0000ac70: 6469 6e67 3a0a 2020 2020 2020 2020 2020  ding:.          
-0000ac80: 2020 7265 7475 726e 0a0a 2020 2020 2020    return..      
-0000ac90: 2020 6966 206e 6578 745f 736f 6e67 203d    if next_song =
-0000aca0: 3d20 2d31 3a0a 2020 2020 2020 2020 2020  = -1:.          
-0000acb0: 2020 6966 2070 6c61 7965 725f 6f75 7470    if player_outp
-0000acc0: 7574 2e69 203d 3d20 706c 6179 6572 5f6f  ut.i == player_o
-0000acd0: 7574 7075 742e 7363 726f 6c6c 6572 2e70  utput.scroller.p
-0000ace0: 6f73 3a0a 2020 2020 2020 2020 2020 2020  os:.            
-0000acf0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
-0000ad00: 742e 7363 726f 6c6c 6572 2e73 6372 6f6c  t.scroller.scrol
-0000ad10: 6c5f 6261 636b 7761 7264 2829 0a20 2020  l_backward().   
-0000ad20: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
-0000ad30: 6f75 7470 7574 2e69 202d 3d20 310a 2020  output.i -= 1.  
-0000ad40: 2020 2020 2020 656c 6966 206e 6578 745f        elif next_
-0000ad50: 736f 6e67 203d 3d20 313a 0a20 2020 2020  song == 1:.     
-0000ad60: 2020 2020 2020 2069 6620 706c 6179 6572         if player
-0000ad70: 5f6f 7574 7075 742e 6920 3d3d 206c 656e  _output.i == len
-0000ad80: 2870 6c61 7965 725f 6f75 7470 7574 2e70  (player_output.p
-0000ad90: 6c61 796c 6973 7429 202d 2031 3a0a 2020  laylist) - 1:.  
-0000ada0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000adb0: 206c 6f6f 703a 0a20 2020 2020 2020 2020   loop:.         
-0000adc0: 2020 2020 2020 2020 2020 206e 6578 745f             next_
-0000add0: 6e65 7874 5f70 6c61 796c 6973 7420 3d20  next_playlist = 
-0000ade0: 6e65 7874 5f70 6c61 796c 6973 745b 3a5d  next_playlist[:]
-0000adf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ae00: 2020 2020 2069 6620 7265 7368 7566 666c       if reshuffl
-0000ae10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000ae20: 2020 2020 2020 2020 2020 2073 6875 6666             shuff
-0000ae30: 6c65 286e 6578 745f 6e65 7874 5f70 6c61  le(next_next_pla
-0000ae40: 796c 6973 7429 0a20 2020 2020 2020 2020  ylist).         
-0000ae50: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-0000ae60: 725f 6f75 7470 7574 2e70 6c61 796c 6973  r_output.playlis
-0000ae70: 742c 206e 6578 745f 706c 6179 6c69 7374  t, next_playlist
-0000ae80: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-0000ae90: 2020 2020 2020 2020 2020 2020 206e 6578               nex
-0000aea0: 745f 706c 6179 6c69 7374 2c0a 2020 2020  t_playlist,.    
-0000aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aec0: 2020 2020 6e65 7874 5f6e 6578 745f 706c      next_next_pl
-0000aed0: 6179 6c69 7374 2c0a 2020 2020 2020 2020  aylist,.        
-0000aee0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af00: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
-0000af10: 6920 3d20 2d31 0a20 2020 2020 2020 2020  i = -1.         
-0000af20: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
-0000af30: 725f 6f75 7470 7574 2e73 6372 6f6c 6c65  r_output.scrolle
-0000af40: 722e 706f 7320 3d20 300a 2020 2020 2020  r.pos = 0.      
-0000af50: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abd0: 2020 2020 2020 2020 2020 2020 206f 7220               or 
+0000abe0: 2255 6e6b 6e6f 776e 2041 6c62 756d 220a  "Unknown Album".
+0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac20: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+0000ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac60: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
+0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aca0: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
+0000acb0: 675f 6461 7461 5b0a 2020 2020 2020 2020  g_data[.        
+0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acf0: 2020 2020 2020 2020 2020 2020 2261 6c62              "alb
+0000ad00: 756d 6172 7469 7374 220a 2020 2020 2020  umartist".      
+0000ad10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad40: 2020 2020 2020 2020 2020 5d2e 7661 6c75            ].valu
+0000ad50: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad90: 2020 6f72 2022 556e 6b6e 6f77 6e20 416c    or "Unknown Al
+0000ada0: 6275 6d20 4172 7469 7374 220a 2020 2020  bum Artist".    
+0000adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ade0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+0000adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae20: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+0000ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000ae60: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000ae70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ae90: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+0000aea0: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
+0000aeb0: 7074 696e 675b 0a20 2020 2020 2020 2020  pting[.         
+0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aef0: 2020 2020 2020 2032 0a20 2020 2020 2020         2.       
+0000af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af30: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+0000af40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af70: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-0000af80: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000af90: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000afa0: 706c 6179 6572 5f6f 7574 7075 742e 6920  player_output.i 
-0000afb0: 3d3d 2070 6c61 7965 725f 6f75 7470 7574  == player_output
-0000afc0: 2e73 6372 6f6c 6c65 722e 706f 733a 0a20  .scroller.pos:. 
+0000af70: 2020 203d 3d20 5052 4f4d 5054 5f4d 4f44     == PROMPT_MOD
+0000af80: 4553 5b0a 2020 2020 2020 2020 2020 2020  ES[.            
+0000af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afc0: 2020 2020 2269 6e73 6572 7422 0a20 2020      "insert".   
 0000afd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afe0: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
-0000aff0: 2e73 6372 6f6c 6c65 722e 7363 726f 6c6c  .scroller.scroll
-0000b000: 5f66 6f72 7761 7264 2829 0a20 2020 2020  _forward().     
-0000b010: 2020 2020 2020 2070 6c61 7965 725f 6f75         player_ou
-0000b020: 7470 7574 2e69 202b 3d20 310a 0a0a 2320  tput.i += 1...# 
-0000b030: 656e 6472 6567 696f 6e0a 0a0a 4063 6c69  endregion...@cli
-0000b040: 636b 2e67 726f 7570 2863 6f6e 7465 7874  ck.group(context
-0000b050: 5f73 6574 7469 6e67 733d 6469 6374 2868  _settings=dict(h
-0000b060: 656c 705f 6f70 7469 6f6e 5f6e 616d 6573  elp_option_names
-0000b070: 3d5b 222d 6822 2c20 222d 2d68 656c 7022  =["-h", "--help"
-0000b080: 5d29 290a 6465 6620 636c 6928 293a 0a20  ])).def cli():. 
-0000b090: 2020 2022 2222 4120 636f 6d6d 616e 6420     """A command 
-0000b0a0: 6c69 6e65 2069 6e74 6572 6661 6365 2066  line interface f
-0000b0b0: 6f72 2070 6c61 7969 6e67 206d 7573 6963  or playing music
-0000b0c0: 2e22 2222 0a20 2020 2069 6620 6e6f 7420  .""".    if not 
-0000b0d0: 6f73 2e70 6174 682e 6578 6973 7473 2853  os.path.exists(S
-0000b0e0: 4f4e 4753 5f44 4952 293a 0a20 2020 2020  ONGS_DIR):.     
-0000b0f0: 2020 206f 732e 6d61 6b65 6469 7273 2853     os.makedirs(S
-0000b100: 4f4e 4753 5f44 4952 290a 0a20 2020 2069  ONGS_DIR)..    i
-0000b110: 6620 6e6f 7420 6f73 2e70 6174 682e 6578  f not os.path.ex
-0000b120: 6973 7473 2853 4f4e 4753 5f49 4e46 4f5f  ists(SONGS_INFO_
-0000b130: 5041 5448 293a 0a20 2020 2020 2020 2077  PATH):.        w
-0000b140: 6974 6820 6f70 656e 2853 4f4e 4753 5f49  ith open(SONGS_I
-0000b150: 4e46 4f5f 5041 5448 2c20 2278 222c 2065  NFO_PATH, "x", e
-0000b160: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
-0000b170: 2061 7320 5f3a 0a20 2020 2020 2020 2020   as _:.         
-0000b180: 2020 2070 6173 730a 0a20 2020 2069 6620     pass..    if 
-0000b190: 6e6f 7420 6f73 2e70 6174 682e 6578 6973  not os.path.exis
-0000b1a0: 7473 2853 5441 5453 5f44 4952 293a 0a20  ts(STATS_DIR):. 
-0000b1b0: 2020 2020 2020 206f 732e 6d61 6b65 6469         os.makedi
-0000b1c0: 7273 2853 5441 5453 5f44 4952 290a 2020  rs(STATS_DIR).  
-0000b1d0: 2020 6966 206e 6f74 206f 732e 7061 7468    if not os.path
-0000b1e0: 2e65 7869 7374 7328 544f 5441 4c5f 5354  .exists(TOTAL_ST
-0000b1f0: 4154 535f 5041 5448 293a 0a20 2020 2020  ATS_PATH):.     
-0000b200: 2020 2077 6974 6820 280a 2020 2020 2020     with (.      
-0000b210: 2020 2020 2020 6f70 656e 2854 4f54 414c        open(TOTAL
-0000b220: 5f53 5441 5453 5f50 4154 482c 2022 7722  _STATS_PATH, "w"
-0000b230: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-0000b240: 3822 2920 6173 2066 2c0a 2020 2020 2020  8") as f,.      
-0000b250: 2020 2020 2020 6f70 656e 2853 4f4e 4753        open(SONGS
-0000b260: 5f49 4e46 4f5f 5041 5448 2c20 2272 222c  _INFO_PATH, "r",
-0000b270: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
-0000b280: 2229 2061 7320 672c 0a20 2020 2020 2020  ") as g,.       
-0000b290: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000b2a0: 666f 7220 6c69 6e65 2069 6e20 673a 0a20  for line in g:. 
-0000b2b0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000b2c0: 2e77 7269 7465 2866 227b 6c69 6e65 2e73  .write(f"{line.s
-0000b2d0: 7472 6970 2829 2e73 706c 6974 2827 7c27  trip().split('|'
-0000b2e0: 295b 305d 7d7c 305c 6e22 290a 2020 2020  )[0]}|0\n").    
-0000b2f0: 6966 206e 6f74 206f 732e 7061 7468 2e65  if not os.path.e
-0000b300: 7869 7374 7328 4355 525f 5945 4152 5f53  xists(CUR_YEAR_S
-0000b310: 5441 5453 5f50 4154 4829 3a0a 2020 2020  TATS_PATH):.    
-0000b320: 2020 2020 7769 7468 2028 0a20 2020 2020      with (.     
-0000b330: 2020 2020 2020 206f 7065 6e28 4355 525f         open(CUR_
-0000b340: 5945 4152 5f53 5441 5453 5f50 4154 482c  YEAR_STATS_PATH,
-0000b350: 2022 7722 2c20 656e 636f 6469 6e67 3d22   "w", encoding="
-0000b360: 7574 662d 3822 2920 6173 2066 2c0a 2020  utf-8") as f,.  
-0000b370: 2020 2020 2020 2020 2020 6f70 656e 2853            open(S
-0000b380: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
-0000b390: 2272 222c 2065 6e63 6f64 696e 673d 2275  "r", encoding="u
-0000b3a0: 7466 2d38 2229 2061 7320 672c 0a20 2020  tf-8") as g,.   
-0000b3b0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-0000b3c0: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-0000b3d0: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-0000b3e0: 2020 2066 2e77 7269 7465 2866 227b 6c69     f.write(f"{li
-0000b3f0: 6e65 2e73 7472 6970 2829 2e73 706c 6974  ne.strip().split
-0000b400: 2827 7c27 295b 305d 7d7c 305c 6e22 290a  ('|')[0]}|0\n").
-0000b410: 0a20 2020 2069 6620 6e6f 7420 6f73 2e70  .    if not os.p
-0000b420: 6174 682e 6578 6973 7473 2846 5245 515f  ath.exists(FREQ_
-0000b430: 4341 4348 455f 4449 5229 3a0a 2020 2020  CACHE_DIR):.    
-0000b440: 2020 2020 6f73 2e6d 616b 6564 6972 7328      os.makedirs(
-0000b450: 4652 4551 5f43 4143 4845 5f44 4952 290a  FREQ_CACHE_DIR).
-0000b460: 2020 2020 6966 206e 6f74 206f 732e 7061      if not os.pa
-0000b470: 7468 2e65 7869 7374 7328 4441 5441 5f43  th.exists(DATA_C
-0000b480: 4143 4845 5f44 4952 293a 0a20 2020 2020  ACHE_DIR):.     
-0000b490: 2020 206f 732e 6d61 6b65 6469 7273 2844     os.makedirs(D
-0000b4a0: 4154 415f 4341 4348 455f 4449 5229 0a0a  ATA_CACHE_DIR)..
-0000b4b0: 0a40 636c 692e 636f 6d6d 616e 6428 290a  .@cli.command().
-0000b4c0: 4063 6c69 636b 2e61 7267 756d 656e 7428  @click.argument(
-0000b4d0: 2270 6174 685f 222c 206d 6574 6176 6172  "path_", metavar
-0000b4e0: 3d22 5041 5448 5f4f 525f 5552 4c22 290a  ="PATH_OR_URL").
-0000b4f0: 4063 6c69 636b 2e61 7267 756d 656e 7428  @click.argument(
-0000b500: 2274 6167 7322 2c20 6e61 7267 733d 2d31  "tags", nargs=-1
-0000b510: 290a 4063 6c69 636b 2e6f 7074 696f 6e28  ).@click.option(
-0000b520: 0a20 2020 2022 2d4d 2f2d 6e4d 222c 0a20  .    "-M/-nM",. 
-0000b530: 2020 2022 2d2d 6d6f 7665 2f2d 2d6e 6f2d     "--move/--no-
-0000b540: 6d6f 7665 222c 0a20 2020 2022 6d6f 7665  move",.    "move
-0000b550: 5f22 2c0a 2020 2020 6465 6661 756c 743d  _",.    default=
-0000b560: 4661 6c73 652c 0a20 2020 2068 656c 703d  False,.    help=
-0000b570: 224d 6f76 6520 6669 6c65 2066 726f 6d20  "Move file from 
-0000b580: 5041 5448 2074 6f20 6d61 6573 7472 6f27  PATH to maestro'
-0000b590: 7320 696e 7465 726e 616c 2073 6f6e 6720  s internal song 
-0000b5a0: 6461 7461 6261 7365 2069 6e73 7465 6164  database instead
-0000b5b0: 206f 6620 636f 7079 696e 672e 222c 0a29   of copying.",.)
-0000b5c0: 0a40 636c 6963 6b2e 6f70 7469 6f6e 280a  .@click.option(.
-0000b5d0: 2020 2020 222d 6e22 2c0a 2020 2020 222d      "-n",.    "-
-0000b5e0: 2d6e 616d 6522 2c0a 2020 2020 7479 7065  -name",.    type
-0000b5f0: 3d73 7472 2c0a 2020 2020 6865 6c70 3d22  =str,.    help="
-0000b600: 5768 6174 2074 6f20 6e61 6d65 2074 6865  What to name the
-0000b610: 2073 6f6e 672c 2069 6620 796f 7520 646f   song, if you do
-0000b620: 6e27 7420 7761 6e74 2074 6f20 7573 6520  n't want to use 
-0000b630: 7468 6520 7469 746c 6520 6672 6f6d 2059  the title from Y
-0000b640: 6f75 7475 6265 2f53 706f 7469 6679 206f  outube/Spotify o
-0000b650: 7220 6669 6c65 6e61 6d65 2e20 446f 206e  r filename. Do n
-0000b660: 6f74 2069 6e63 6c75 6465 2061 6e20 6578  ot include an ex
-0000b670: 7465 6e73 696f 6e20 2865 2e67 2e20 272e  tension (e.g. '.
-0000b680: 7761 7627 292e 2049 676e 6f72 6564 2069  wav'). Ignored i
-0000b690: 6620 6164 6469 6e67 206d 756c 7469 706c  f adding multipl
-0000b6a0: 6520 736f 6e67 732e 222c 0a29 0a40 636c  e songs.",.).@cl
-0000b6b0: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
-0000b6c0: 222d 522c 202d 6e52 222c 0a20 2020 2022  "-R, -nR",.    "
-0000b6d0: 2d2d 7265 6375 7273 6976 652f 2d2d 6e6f  --recursive/--no
-0000b6e0: 2d72 6563 7572 7369 7665 222c 0a20 2020  -recursive",.   
-0000b6f0: 2022 7265 6375 7273 6522 2c0a 2020 2020   "recurse",.    
-0000b700: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
-0000b710: 2020 2068 656c 703d 2249 6620 5041 5448     help="If PATH
-0000b720: 2069 7320 6120 666f 6c64 6572 2c20 6164   is a folder, ad
-0000b730: 6420 736f 6e67 7320 696e 2073 7562 666f  d songs in subfo
-0000b740: 6c64 6572 732e 222c 0a29 0a40 636c 6963  lders.",.).@clic
-0000b750: 6b2e 6f70 7469 6f6e 280a 2020 2020 222d  k.option(.    "-
-0000b760: 592f 2d6e 5922 2c0a 2020 2020 222d 2d79  Y/-nY",.    "--y
-0000b770: 6f75 7475 6265 2f2d 2d6e 6f2d 796f 7574  outube/--no-yout
-0000b780: 7562 6522 2c0a 2020 2020 6465 6661 756c  ube",.    defaul
-0000b790: 743d 4661 6c73 652c 0a20 2020 2068 656c  t=False,.    hel
-0000b7a0: 703d 2241 6464 2061 2073 6f6e 6720 6672  p="Add a song fr
-0000b7b0: 6f6d 2061 2059 6f75 5475 6265 206f 7220  om a YouTube or 
-0000b7c0: 596f 7554 7562 6520 4d75 7369 6320 5552  YouTube Music UR
-0000b7d0: 4c2e 222c 0a29 0a40 636c 6963 6b2e 6f70  L.",.).@click.op
-0000b7e0: 7469 6f6e 280a 2020 2020 222d 532f 2d6e  tion(.    "-S/-n
-0000b7f0: 5322 2c0a 2020 2020 222d 2d73 706f 7469  S",.    "--spoti
-0000b800: 6679 2f2d 2d6e 6f2d 7370 6f74 6966 7922  fy/--no-spotify"
-0000b810: 2c0a 2020 2020 6465 6661 756c 743d 4661  ,.    default=Fa
-0000b820: 6c73 652c 0a20 2020 2068 656c 703d 2241  lse,.    help="A
-0000b830: 6464 2061 2073 6f6e 6720 6672 6f6d 2053  dd a song from S
-0000b840: 706f 7469 6679 2028 7472 6163 6b20 5552  potify (track UR
-0000b850: 4c2c 2061 6c62 756d 2055 524c 2c20 706c  L, album URL, pl
-0000b860: 6179 6c69 7374 2055 524c 2c20 6172 7469  aylist URL, arti
-0000b870: 7374 2055 524c 2c20 6f72 2073 6561 7263  st URL, or searc
-0000b880: 6820 7175 6572 7929 2e22 2c0a 290a 4063  h query).",.).@c
-0000b890: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
-0000b8a0: 2022 2d66 222c 0a20 2020 2022 2d2d 666f   "-f",.    "--fo
-0000b8b0: 726d 6174 222c 0a20 2020 2022 666f 726d  rmat",.    "form
-0000b8c0: 6174 5f22 2c0a 2020 2020 7479 7065 3d63  at_",.    type=c
-0000b8d0: 6c69 636b 2e43 686f 6963 6528 5b22 7761  lick.Choice(["wa
-0000b8e0: 7622 2c20 226d 7033 222c 2022 666c 6163  v", "mp3", "flac
-0000b8f0: 222c 2022 6f67 6722 5d29 2c0a 2020 2020  ", "ogg"]),.    
-0000b900: 6865 6c70 3d22 5370 6563 6966 7920 7468  help="Specify th
-0000b910: 6520 666f 726d 6174 206f 6620 7468 6520  e format of the 
-0000b920: 736f 6e67 2069 6620 646f 776e 6c6f 6164  song if download
-0000b930: 696e 6720 6672 6f6d 2061 2059 6f75 5475  ing from a YouTu
-0000b940: 6265 206f 7220 596f 7554 7562 6520 4d75  be or YouTube Mu
-0000b950: 7369 6320 5552 4c2e 222c 0a20 2020 2064  sic URL.",.    d
-0000b960: 6566 6175 6c74 3d22 666c 6163 222c 0a20  efault="flac",. 
-0000b970: 2020 2073 686f 775f 6465 6661 756c 743d     show_default=
-0000b980: 5472 7565 2c0a 290a 4063 6c69 636b 2e6f  True,.).@click.o
-0000b990: 7074 696f 6e28 0a20 2020 2022 2d63 222c  ption(.    "-c",
-0000b9a0: 0a20 2020 2022 2d2d 636c 6970 222c 0a20  .    "--clip",. 
-0000b9b0: 2020 206e 6172 6773 3d32 2c0a 2020 2020     nargs=2,.    
-0000b9c0: 7479 7065 3d66 6c6f 6174 2c0a 2020 2020  type=float,.    
-0000b9d0: 6865 6c70 3d22 4164 6420 6120 636c 6970  help="Add a clip
-0000b9e0: 2e20 4967 6e6f 7265 6420 6966 2061 6464  . Ignored if add
-0000b9f0: 696e 6720 6d75 6c74 6970 6c65 2073 6f6e  ing multiple son
-0000ba00: 6773 2e22 2c0a 290a 4063 6c69 636b 2e6f  gs.",.).@click.o
-0000ba10: 7074 696f 6e28 0a20 2020 2022 2d50 2f2d  ption(.    "-P/-
-0000ba20: 6e50 222c 0a20 2020 2022 2d2d 706c 6179  nP",.    "--play
-0000ba30: 6c69 7374 2f2d 2d6e 6f2d 706c 6179 6c69  list/--no-playli
-0000ba40: 7374 222c 0a20 2020 2022 706c 6179 6c69  st",.    "playli
-0000ba50: 7374 5f22 2c0a 2020 2020 6465 6661 756c  st_",.    defaul
-0000ba60: 743d 4661 6c73 652c 0a20 2020 2068 656c  t=False,.    hel
-0000ba70: 703d 2249 6620 736f 6e67 2055 524c 2070  p="If song URL p
-0000ba80: 6173 7365 6420 6973 2066 726f 6d20 6120  assed is from a 
-0000ba90: 596f 7554 7562 6520 706c 6179 6c69 7374  YouTube playlist
-0000baa0: 2c20 646f 776e 6c6f 6164 2061 6c6c 2074  , download all t
-0000bab0: 6865 2073 6f6e 6773 2e20 4966 2074 6865  he songs. If the
-0000bac0: 2055 524c 2070 6f69 6e74 7320 6469 7265   URL points dire
-0000bad0: 6374 6c79 2074 6f20 6120 706c 6179 6c69  ctly to a playli
-0000bae0: 7374 2c20 7468 6973 2066 6c61 6720 6973  st, this flag is
-0000baf0: 2075 6e6e 6365 7373 6172 792e 222c 0a29   unncessary.",.)
-0000bb00: 0a40 636c 6963 6b2e 6f70 7469 6f6e 280a  .@click.option(.
-0000bb10: 2020 2020 222d 562f 2d6e 5622 2c0a 2020      "-V/-nV",.  
-0000bb20: 2020 222d 2d76 6973 7561 6c69 7a65 2f2d    "--visualize/-
-0000bb30: 2d6e 6f2d 7669 7375 616c 697a 6522 2c0a  -no-visualize",.
-0000bb40: 2020 2020 6465 6661 756c 743d 4661 6c73      default=Fals
-0000bb50: 652c 0a20 2020 2068 656c 703d 2243 616c  e,.    help="Cal
-0000bb60: 6375 6c61 7465 2061 6e64 2063 6163 6865  culate and cache
-0000bb70: 2076 6973 7561 6c69 7a61 7469 6f6e 2066   visualization f
-0000bb80: 7265 7175 656e 6369 6573 2066 6f72 2074  requencies for t
-0000bb90: 6865 2073 6f6e 672e 2049 676e 6f72 6564  he song. Ignored
-0000bba0: 2069 6620 7468 6520 7265 7175 6972 6564   if the required
-0000bbb0: 2064 6570 656e 6465 6e63 6965 7320 6172   dependencies ar
-0000bbc0: 6520 6e6f 7420 696e 7374 616c 6c65 642e  e not installed.
-0000bbd0: 222c 0a29 0a40 636c 6963 6b2e 6f70 7469  ",.).@click.opti
-0000bbe0: 6f6e 280a 2020 2020 222d 6d22 2c0a 2020  on(.    "-m",.  
-0000bbf0: 2020 222d 2d6d 6574 6164 6174 6122 2c0a    "--metadata",.
-0000bc00: 2020 2020 226d 6574 6164 6174 615f 7061      "metadata_pa
-0000bc10: 6972 7322 2c0a 2020 2020 6465 6661 756c  irs",.    defaul
-0000bc20: 743d 4e6f 6e65 2c0a 2020 2020 6865 6c70  t=None,.    help
-0000bc30: 3d22 4164 6420 6d65 7461 6461 7461 2074  ="Add metadata t
-0000bc40: 6f20 7468 6520 736f 6e67 2e20 4967 6e6f  o the song. Igno
-0000bc50: 7265 6420 6966 2061 6464 696e 6720 6d75  red if adding mu
-0000bc60: 6c74 6970 6c65 2073 6f6e 6773 2e20 5468  ltiple songs. Th
-0000bc70: 6520 666f 726d 6174 2069 7320 276b 6579  e format is 'key
-0000bc80: 313a 7661 6c75 6531 7c6b 6579 323a 7661  1:value1|key2:va
-0000bc90: 6c75 6532 7c2e 2e2e 272e 222c 0a29 0a64  lue2|...'.",.).d
-0000bca0: 6566 2061 6464 280a 2020 2020 7061 7468  ef add(.    path
-0000bcb0: 5f2c 0a20 2020 2074 6167 732c 0a20 2020  _,.    tags,.   
-0000bcc0: 206d 6f76 655f 2c0a 2020 2020 6e61 6d65   move_,.    name
-0000bcd0: 2c0a 2020 2020 7265 6375 7273 652c 0a20  ,.    recurse,. 
-0000bce0: 2020 2079 6f75 7475 6265 2c0a 2020 2020     youtube,.    
-0000bcf0: 7370 6f74 6966 792c 0a20 2020 2066 6f72  spotify,.    for
-0000bd00: 6d61 745f 2c0a 2020 2020 636c 6970 2c0a  mat_,.    clip,.
-0000bd10: 2020 2020 706c 6179 6c69 7374 5f2c 0a20      playlist_,. 
-0000bd20: 2020 2076 6973 7561 6c69 7a65 2c0a 2020     visualize,.  
-0000bd30: 2020 6d65 7461 6461 7461 5f70 6169 7273    metadata_pairs
-0000bd40: 2c0a 293a 0a20 2020 2022 2222 4164 6420  ,.):.    """Add 
-0000bd50: 6120 6e65 7720 736f 6e67 2c20 6c6f 6361  a new song, loca
-0000bd60: 7465 6420 6174 2050 4154 482e 2049 6620  ted at PATH. If 
-0000bd70: 5041 5448 2069 7320 6120 666f 6c64 6572  PATH is a folder
-0000bd80: 2c20 6164 6473 2061 6c6c 2066 696c 6573  , adds all files
-0000bd90: 0a20 2020 2069 6e20 5041 5448 2028 696e  .    in PATH (in
-0000bda0: 636c 7564 696e 6720 6669 6c65 7320 696e  cluding files in
-0000bdb0: 2073 7562 666f 6c64 6572 7320 6966 2027   subfolders if '
-0000bdc0: 2d72 2720 6973 2070 6173 7365 6429 2e20  -r' is passed). 
-0000bdd0: 5468 6520 6e61 6d65 206f 6620 6561 6368  The name of each
-0000bde0: 0a20 2020 2073 6f6e 6720 7769 6c6c 2062  .    song will b
-0000bdf0: 6520 7468 6520 6669 6c65 6e61 6d65 2028  e the filename (
-0000be00: 756e 6c65 7373 2027 2d6e 2720 6973 2070  unless '-n' is p
-0000be10: 6173 7365 6429 2e20 4669 6c65 6e61 6d65  assed). Filename
-0000be20: 7320 616e 6420 7461 6773 2063 616e 6e6f  s and tags canno
-0000be30: 740a 2020 2020 636f 6e74 6169 6e20 7468  t.    contain th
-0000be40: 6520 6368 6172 6163 7465 7220 277c 272c  e character '|',
-0000be50: 2061 6e64 2074 6167 7320 6361 6e6e 6f74   and tags cannot
-0000be60: 2063 6f6e 7461 696e 2027 2c27 2e0a 0a20   contain ','... 
-0000be70: 2020 2049 6620 7468 6520 272d 5927 206f     If the '-Y' o
-0000be80: 7220 272d 2d79 6f75 7475 6265 2720 666c  r '--youtube' fl
-0000be90: 6167 2069 7320 7061 7373 6564 2c20 5041  ag is passed, PA
-0000bea0: 5448 2069 7320 7472 6561 7465 6420 6173  TH is treated as
-0000beb0: 2061 2059 6f75 5475 6265 206f 720a 2020   a YouTube or.  
-0000bec0: 2020 596f 7554 7562 6520 4d75 7369 6320    YouTube Music 
-0000bed0: 5552 4c20 696e 7374 6561 6420 6f66 2061  URL instead of a
-0000bee0: 2066 696c 6520 7061 7468 2e0a 0a20 2020   file path...   
-0000bef0: 2049 6620 7468 6520 272d 5327 206f 7220   If the '-S' or 
-0000bf00: 272d 2d73 706f 7469 6679 2720 666c 6167  '--spotify' flag
-0000bf10: 2069 7320 7061 7373 6564 2c20 5041 5448   is passed, PATH
-0000bf20: 2069 7320 7472 6561 7465 6420 6173 2061   is treated as a
-0000bf30: 2053 706f 7469 6679 0a20 2020 2074 7261   Spotify.    tra
-0000bf40: 636b 2055 524c 2c20 616c 6275 6d20 5552  ck URL, album UR
-0000bf50: 4c2c 2070 6c61 796c 6973 7420 5552 4c2c  L, playlist URL,
-0000bf60: 2061 7274 6973 7420 5552 4c2c 206f 7220   artist URL, or 
-0000bf70: 7365 6172 6368 2071 7565 7279 2069 6e73  search query ins
-0000bf80: 7465 6164 206f 660a 2020 2020 6120 6669  tead of.    a fi
-0000bf90: 6c65 2070 6174 682e 0a0a 2020 2020 5468  le path...    Th
-0000bfa0: 6520 272d 632f 2d2d 636c 6970 2720 6f70  e '-c/--clip' op
-0000bfb0: 7469 6f6e 2063 616e 2062 6520 7573 6564  tion can be used
-0000bfc0: 2074 6f20 6164 6420 6120 636c 6970 2066   to add a clip f
-0000bfd0: 6f72 2074 6865 2073 6f6e 672e 2049 7420  or the song. It 
-0000bfe0: 7461 6b65 7320 7477 6f0a 2020 2020 6172  takes two.    ar
-0000bff0: 6775 6d65 6e74 732c 2062 7574 2075 6e6c  guments, but unl
-0000c000: 696b 6520 276d 6165 7374 726f 2063 6c69  ike 'maestro cli
-0000c010: 7027 2c20 796f 7520 6361 6e6e 6f74 2070  p', you cannot p
-0000c020: 6173 7320 6f6e 6c79 2074 6865 2073 7461  ass only the sta
-0000c030: 7274 2074 696d 650a 2020 2020 616e 6420  rt time.    and 
-0000c040: 6e6f 7420 7468 6520 656e 642e 2054 6f20  not the end. To 
-0000c050: 6765 7420 6172 6f75 6e64 2074 6869 732c  get around this,
-0000c060: 2079 6f75 2063 616e 2070 6173 7320 2d31   you can pass -1
-0000c070: 2061 7320 7468 6520 656e 6420 7469 6d65   as the end time
-0000c080: 2c20 652e 672e 0a20 2020 2027 6d61 6573  , e.g..    'maes
-0000c090: 7472 6f20 6164 6420 2d63 2033 3020 2d31  tro add -c 30 -1
-0000c0a0: 2068 7474 7073 3a2f 2f77 7777 2e79 6f75   https://www.you
-0000c0b0: 7475 6265 2e63 6f6d 2f77 6174 6368 3f76  tube.com/watch?v
-0000c0c0: 3d33 5678 754d 4572 4364 2d45 202d 7927  =3VxuMErCd-E -y'
-0000c0d0: 2e20 4966 0a20 2020 2061 6464 696e 6720  . If.    adding 
-0000c0e0: 6d75 6c74 6970 6c65 2073 6f6e 6773 2c20  multiple songs, 
-0000c0f0: 7468 6973 206f 7074 696f 6e20 6361 6e6e  this option cann
-0000c100: 6f74 2062 6520 7573 6564 2e0a 0a20 2020  ot be used...   
-0000c110: 2054 6865 2027 2d6d 2f2d 2d6d 6574 6164   The '-m/--metad
-0000c120: 6174 6127 206f 7074 696f 6e20 6361 6e20  ata' option can 
-0000c130: 6265 2075 7365 6420 746f 2061 6464 206d  be used to add m
-0000c140: 6574 6164 6174 6120 746f 2074 6865 2073  etadata to the s
-0000c150: 6f6e 672e 2049 7420 7461 6b65 730a 2020  ong. It takes.  
-0000c160: 2020 6120 7374 7269 6e67 206f 6620 7468    a string of th
-0000c170: 6520 666f 726d 6174 2027 6b65 7931 3a76  e format 'key1:v
-0000c180: 616c 7565 317c 6b65 7932 3a76 616c 7565  alue1|key2:value
-0000c190: 327c 2e2e 2e27 2e20 4966 2061 6464 696e  2|...'. If addin
-0000c1a0: 6720 6d75 6c74 6970 6c65 0a20 2020 2073  g multiple.    s
-0000c1b0: 6f6e 6773 2c20 7468 6973 206f 7074 696f  ongs, this optio
-0000c1c0: 6e20 6361 6e6e 6f74 2062 6520 7573 6564  n cannot be used
-0000c1d0: 2e0a 0a20 2020 2050 6f73 7369 626c 6520  ...    Possible 
-0000c1e0: 6564 6974 6162 6c65 206d 6574 6164 6174  editable metadat
-0000c1f0: 6120 6b65 7973 2061 7265 3a20 616c 6275  a keys are: albu
-0000c200: 6d2c 2061 6c62 756d 6172 7469 7374 2c20  m, albumartist, 
-0000c210: 6172 7469 7374 2c20 6172 7477 6f72 6b2c  artist, artwork,
-0000c220: 0a20 2020 2063 6f6d 6d65 6e74 2c20 636f  .    comment, co
-0000c230: 6d70 696c 6174 696f 6e2c 2063 6f6d 706f  mpilation, compo
-0000c240: 7365 722c 2064 6973 636e 756d 6265 722c  ser, discnumber,
-0000c250: 2067 656e 7265 2c20 6c79 7269 6373 2c20   genre, lyrics, 
-0000c260: 746f 7461 6c64 6973 6373 2c0a 2020 2020  totaldiscs,.    
-0000c270: 746f 7461 6c74 7261 636b 732c 2074 7261  totaltracks, tra
-0000c280: 636b 6e75 6d62 6572 2c20 7472 6163 6b74  cknumber, trackt
-0000c290: 6974 6c65 2c20 7965 6172 2c20 6973 7263  itle, year, isrc
-0000c2a0: 0a0a 2020 2020 4b65 7973 2061 7265 206e  ..    Keys are n
-0000c2b0: 6f74 2063 6173 6520 7365 6e73 6974 6976  ot case sensitiv
-0000c2c0: 6520 616e 6420 6361 6e20 636f 6e74 6169  e and can contai
-0000c2d0: 6e20 6172 6269 7472 6172 7920 7768 6974  n arbitrary whit
-0000c2e0: 6573 7061 6365 2c20 272d 272c 2061 6e64  espace, '-', and
-0000c2f0: 0a20 2020 2027 5f27 2063 6861 7261 6374  .    '_' charact
-0000c300: 6572 732e 2049 6e20 6f74 6865 7220 776f  ers. In other wo
-0000c310: 7264 732c 2027 416c 6275 6d20 4172 7469  rds, 'Album Arti
-0000c320: 7374 272c 2027 616c 6275 6d2d 6172 7469  st', 'album-arti
-0000c330: 7374 272c 2061 6e64 0a20 2020 2027 616c  st', and.    'al
-0000c340: 6275 6d5f 6172 7469 7374 2720 6172 6520  bum_artist' are 
-0000c350: 616c 6c20 7379 6e6f 6e79 6d73 2066 6f72  all synonyms for
-0000c360: 2027 616c 6275 6d61 7274 6973 7427 2e20   'albumartist'. 
-0000c370: 416c 736f 2c20 2764 6973 6b27 2069 730a  Also, 'disk' is.
-0000c380: 2020 2020 7379 6e6f 6e79 6d6f 7573 2077      synonymous w
-0000c390: 6974 6820 2764 6973 6327 2e0a 2020 2020  ith 'disc'..    
-0000c3a0: 2222 220a 0a20 2020 2070 6174 6873 203d  """..    paths =
-0000c3b0: 204e 6f6e 650a 2020 2020 6966 206e 6f74   None.    if not
-0000c3c0: 2028 796f 7574 7562 6520 6f72 2073 706f   (youtube or spo
-0000c3d0: 7469 6679 2920 616e 6420 6e6f 7420 6f73  tify) and not os
-0000c3e0: 2e70 6174 682e 6578 6973 7473 2870 6174  .path.exists(pat
-0000c3f0: 685f 293a 0a20 2020 2020 2020 2063 6c69  h_):.        cli
-0000c400: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
-0000c410: 2020 2020 2020 6622 5468 6520 7061 7468        f"The path
-0000c420: 2027 7b70 6174 685f 7d27 2064 6f65 7320   '{path_}' does 
-0000c430: 6e6f 7420 6578 6973 742e 2054 6f20 646f  not exist. To do
-0000c440: 776e 6c6f 6164 2066 726f 6d20 6120 596f  wnload from a Yo
-0000c450: 7554 7562 6520 6f72 2059 6f75 5475 6265  uTube or YouTube
-0000c460: 204d 7573 6963 2055 526c 2c20 7061 7373   Music URl, pass
-0000c470: 2074 6865 2027 2d59 2f2d 2d79 6f75 7475   the '-Y/--youtu
-0000c480: 6265 2720 666c 6167 2e20 546f 2064 6f77  be' flag. To dow
-0000c490: 6e6c 6f61 6420 6672 6f6d 2061 2053 706f  nload from a Spo
-0000c4a0: 7469 6679 2055 526c 2c20 7061 7373 2074  tify URl, pass t
-0000c4b0: 6865 2027 2d53 2f2d 2d73 706f 7469 6679  he '-S/--spotify
-0000c4c0: 2720 666c 6167 2e22 2c0a 2020 2020 2020  ' flag.",.      
-0000c4d0: 2020 2020 2020 6667 3d22 7265 6422 2c0a        fg="red",.
-0000c4e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000c4f0: 2020 7265 7475 726e 0a20 2020 2065 6c69    return.    eli
-0000c500: 6620 796f 7574 7562 6520 6f72 2073 706f  f youtube or spo
-0000c510: 7469 6679 3a0a 2020 2020 2020 2020 6966  tify:.        if
-0000c520: 2079 6f75 7475 6265 2061 6e64 2073 706f   youtube and spo
-0000c530: 7469 6679 3a0a 2020 2020 2020 2020 2020  tify:.          
-0000c540: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
-0000c550: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000c560: 4361 6e6e 6f74 2070 6173 7320 626f 7468  Cannot pass both
-0000c570: 2027 2d79 2f2d 2d79 6f75 7475 6265 2720   '-y/--youtube' 
-0000c580: 616e 6420 272d 732f 2d2d 7370 6f74 6966  and '-s/--spotif
-0000c590: 7927 2066 6c61 6773 2e22 2c0a 2020 2020  y' flags.",.    
-0000c5a0: 2020 2020 2020 2020 2020 2020 6667 3d22              fg="
-0000c5b0: 7265 6422 2c0a 2020 2020 2020 2020 2020  red",.          
-0000c5c0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-0000c5d0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
-0000c5e0: 6966 2079 6f75 7475 6265 3a0a 2020 2020  if youtube:.    
-0000c5f0: 2020 2020 2020 2020 6966 2066 6f72 6d61          if forma
-0000c600: 745f 203d 3d20 226f 6767 223a 0a20 2020  t_ == "ogg":.   
-0000c610: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
-0000c620: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
-0000c630: 2020 2020 2020 2020 2020 2020 2020 2243                "C
-0000c640: 616e 6e6f 7420 646f 776e 6c6f 6164 2073  annot download s
-0000c650: 6f6e 6773 2066 726f 6d20 596f 7554 7562  ongs from YouTub
-0000c660: 6520 6173 2027 2e6f 6767 272e 2050 6c65  e as '.ogg'. Ple
-0000c670: 6173 6520 6368 6f6f 7365 2061 2064 6966  ase choose a dif
-0000c680: 6665 7265 6e74 2066 6f72 6d61 742e 222c  ferent format.",
-0000c690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c6a0: 2020 2020 2066 673d 2272 6564 222c 0a20       fg="red",. 
-0000c6b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000c6c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c6d0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000c6e0: 2020 2020 7375 6270 726f 6365 7373 2e72      subprocess.r
-0000c6f0: 756e 280a 2020 2020 2020 2020 2020 2020  un(.            
-0000c700: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-0000c710: 2020 2020 2020 2020 2020 2279 742d 646c            "yt-dl
-0000c720: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-0000c730: 2020 2020 2020 2020 7061 7468 5f2c 0a20          path_,. 
+0000afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b000: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
+0000b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b040: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b080: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+0000b090: 706c 6179 6c69 7374 2e69 6e73 6572 7428  playlist.insert(
+0000b0a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b0e0: 2070 6c61 7965 725f 6f75 7470 7574 2e73   player_output.s
+0000b0f0: 6372 6f6c 6c65 722e 706f 730a 2020 2020  croller.pos.    
+0000b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b130: 2020 2020 2020 2020 2020 2020 2b20 312c              + 1,
+0000b140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b180: 2064 6574 6169 6c73 2c0a 2020 2020 2020   details,.      
+0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b200: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b240: 2020 706c 6179 6572 5f6f 7574 7075 742e    player_output.
+0000b250: 706c 6179 6c69 7374 2e61 7070 656e 6428  playlist.append(
+0000b260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2a0: 2064 6574 6169 6c73 0a20 2020 2020 2020   details.       
+0000b2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b310: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000b320: 6620 6c6f 6f70 3a0a 2020 2020 2020 2020  f loop:.        
+0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b360: 2020 2020 6966 2072 6573 6875 6666 6c65      if reshuffle
+0000b370: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3b0: 2020 6e65 7874 5f70 6c61 796c 6973 742e    next_playlist.
+0000b3c0: 696e 7365 7274 280a 2020 2020 2020 2020  insert(.        
+0000b3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b400: 2020 2020 2020 2020 2020 2020 7261 6e64              rand
+0000b410: 696e 7428 0a20 2020 2020 2020 2020 2020  int(.           
+0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b450: 2020 2020 2020 2020 2020 2020 2030 2c0a               0,.
+0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4a0: 2020 2020 2020 2020 6c65 6e28 0a20 2020          len(.   
+0000b4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4f0: 2020 2020 2020 2020 206e 6578 745f 706c           next_pl
+0000b500: 6179 6c69 7374 0a20 2020 2020 2020 2020  aylist.         
+0000b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b540: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000b550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b590: 2020 2020 2020 2020 202d 2031 2c0a 2020           - 1,.  
+0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b5e0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b620: 2020 2020 2020 2020 2064 6574 6169 6c73           details
+0000b630: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b670: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000b680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6b0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6f0: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
+0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b730: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000b740: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
+0000b750: 6d70 7469 6e67 5b0a 2020 2020 2020 2020  mpting[.        
+0000b760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7a0: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
+0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7e0: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
+0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b820: 2020 2020 2020 2020 2020 2020 3d3d 2050              == P
+0000b830: 524f 4d50 545f 4d4f 4445 535b 0a20 2020  ROMPT_MODES[.   
+0000b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b880: 2020 2020 2022 696e 7365 7274 220a 2020       "insert".  
+0000b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8d0: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+0000b8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b910: 2020 2020 293a 0a20 2020 2020 2020 2020      ):.         
+0000b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b950: 2020 2020 2020 2020 2020 206e 6578 745f             next_
+0000b960: 706c 6179 6c69 7374 2e69 6e73 6572 7428  playlist.insert(
+0000b970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9b0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+0000b9c0: 6f75 7470 7574 2e73 6372 6f6c 6c65 722e  output.scroller.
+0000b9d0: 706f 730a 2020 2020 2020 2020 2020 2020  pos.            
+0000b9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba10: 2020 2020 2020 2020 2020 2020 2b20 312c              + 1,
+0000ba20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba60: 2020 2020 2020 2020 2064 6574 6169 6c73           details
+0000ba70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000ba80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bab0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000bac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000baf0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb40: 2020 6e65 7874 5f70 6c61 796c 6973 742e    next_playlist.
+0000bb50: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
+0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bba0: 6465 7461 696c 730a 2020 2020 2020 2020  details.        
+0000bbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bbe0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc20: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+0000bc30: 7075 742e 7363 726f 6c6c 6572 2e6e 756d  put.scroller.num
+0000bc40: 5f6c 696e 6573 202b 3d20 280a 2020 2020  _lines += (.    
+0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc80: 2020 2020 2020 2020 310a 2020 2020 2020          1.      
+0000bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcc0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcf0: 2020 2020 2020 2020 2020 2020 706c 6179              play
+0000bd00: 6572 5f6f 7574 7075 742e 7072 6f6d 7074  er_output.prompt
+0000bd10: 696e 6720 3d20 280a 2020 2020 2020 2020  ing = (.        
+0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd50: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
+0000bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd90: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+0000bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdc0: 2020 2020 2020 2020 2020 2063 7572 7365             curse
+0000bdd0: 732e 6375 7273 5f73 6574 2846 616c 7365  s.curs_set(False
+0000bde0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be10: 2020 2020 2020 2020 2020 706c 6179 6572            player
+0000be20: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
+0000be30: 2e72 6573 697a 6528 0a20 2020 2020 2020  .resize(.       
+0000be40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be70: 2020 2020 2073 6372 6565 6e5f 7369 7a65       screen_size
+0000be80: 5b30 5d20 2d20 320a 2020 2020 2020 2020  [0] - 2.        
+0000be90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bec0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000bed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bef0: 2020 2020 2020 2020 2020 706c 6179 6572            player
+0000bf00: 5f6f 7574 7075 742e 6f75 7470 7574 280a  _output.output(.
+0000bf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf40: 2020 2020 2020 2020 2020 2020 706c 6179              play
+0000bf50: 6261 636b 2e63 7572 725f 706f 730a 2020  back.curr_pos.  
+0000bf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf90: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bfd0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
+0000bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bff0: 2020 2020 2020 2020 2020 656c 6966 2028            elif (
+0000c000: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c020: 2020 2020 2020 2020 2022 7c22 206e 6f74           "|" not
+0000c030: 2069 6e20 706c 6179 6572 5f6f 7574 7075   in player_outpu
+0000c040: 742e 7072 6f6d 7074 696e 675b 305d 0a20  t.prompting[0]. 
+0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c070: 2020 2020 2020 2061 6e64 2070 6c61 7965         and playe
+0000c080: 725f 6f75 7470 7574 2e70 726f 6d70 7469  r_output.prompti
+0000c090: 6e67 5b32 5d0a 2020 2020 2020 2020 2020  ng[2].          
+0000c0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0b0: 2020 2020 2020 2020 2020 2020 2020 3d3d                ==
+0000c0c0: 2050 524f 4d50 545f 4d4f 4445 535b 2274   PROMPT_MODES["t
+0000c0d0: 6167 225d 0a20 2020 2020 2020 2020 2020  ag"].           
+0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0f0: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+0000c100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c120: 2020 2020 7461 6773 203d 2070 6c61 7965      tags = playe
+0000c130: 725f 6f75 7470 7574 2e70 726f 6d70 7469  r_output.prompti
+0000c140: 6e67 5b30 5d2e 7370 6c69 7428 0a20 2020  ng[0].split(.   
+0000c150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c170: 2020 2020 2020 2020 2022 2c22 0a20 2020           ",".   
+0000c180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1a0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1d0: 7461 6767 696e 675f 6964 7320 3d20 7b7d  tagging_ids = {}
+0000c1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c200: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+0000c210: 6e20 7261 6e67 6528 0a20 2020 2020 2020  n range(.       
+0000c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c240: 2020 2020 206c 656e 2870 6c61 7965 725f       len(player_
+0000c250: 6f75 7470 7574 2e70 6c61 796c 6973 7429  output.playlist)
+0000c260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c280: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+0000c290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2b0: 2020 2020 2020 2020 7461 6767 696e 675f          tagging_
+0000c2c0: 6964 735b 0a20 2020 2020 2020 2020 2020  ids[.           
+0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2f0: 2020 2020 2069 6e74 280a 2020 2020 2020       int(.      
+0000c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c320: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+0000c330: 6179 6572 5f6f 7574 7075 742e 706c 6179  ayer_output.play
+0000c340: 6c69 7374 5b69 5d5b 305d 0a20 2020 2020  list[i][0].     
+0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c370: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3a0: 2020 2020 2020 2020 205d 203d 2069 0a0a           ] = i..
+0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3d0: 2020 2020 2020 2020 736f 6e67 735f 6669          songs_fi
+0000c3e0: 6c65 203d 206f 7065 6e28 0a20 2020 2020  le = open(.     
+0000c3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c410: 2020 2020 2020 2053 4f4e 4753 5f49 4e46         SONGS_INF
+0000c420: 4f5f 5041 5448 2c0a 2020 2020 2020 2020  O_PATH,.        
+0000c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c450: 2020 2020 2272 222c 0a20 2020 2020 2020      "r",.       
+0000c460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c480: 2020 2020 2065 6e63 6f64 696e 673d 2275       encoding="u
+0000c490: 7466 2d38 222c 0a20 2020 2020 2020 2020  tf-8",.         
+0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000c4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4e0: 2020 2020 2020 2020 206c 696e 6573 203d           lines =
+0000c4f0: 2073 6f6e 6773 5f66 696c 652e 7265 6164   songs_file.read
+0000c500: 2829 2e73 706c 6974 6c69 6e65 7328 290a  ().splitlines().
+0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c530: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+0000c540: 2072 616e 6765 286c 656e 286c 696e 6573   range(len(lines
+0000c550: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c580: 6465 7461 696c 7320 3d20 280a 2020 2020  details = (.    
+0000c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5b0: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+0000c5c0: 735b 695d 2e73 7472 6970 2829 2e73 706c  s[i].strip().spl
+0000c5d0: 6974 2822 7c22 290a 2020 2020 2020 2020  it("|").        
+0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c600: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c630: 2020 736f 6e67 5f69 6420 3d20 696e 7428    song_id = int(
+0000c640: 6465 7461 696c 735b 305d 290a 2020 2020  details[0]).    
+0000c650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c670: 2020 2020 2020 2020 6966 2073 6f6e 675f          if song_
+0000c680: 6964 2069 6e20 7461 6767 696e 675f 6964  id in tagging_id
+0000c690: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+0000c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6c0: 2020 2069 6620 6465 7461 696c 735b 325d     if details[2]
+0000c6d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c700: 2020 2020 2020 6e65 775f 7461 6773 203d        new_tags =
+0000c710: 2064 6574 6169 6c73 5b32 5d2e 7370 6c69   details[2].spli
+0000c720: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+0000c730: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000c740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c750: 2020 2022 2d78 222c 2020 2320 6578 7472     "-x",  # extr
-0000c760: 6163 7420 6175 6469 6f20 286e 6563 6573  act audio (neces
-0000c770: 7361 7279 2c20 6e65 6564 7320 6666 6d70  sary, needs ffmp
-0000c780: 6567 290a 2020 2020 2020 2020 2020 2020  eg).            
-0000c790: 2020 2020 2020 2020 222d 2d61 7564 696f          "--audio
-0000c7a0: 2d66 6f72 6d61 7422 2c0a 2020 2020 2020  -format",.      
-0000c7b0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000c7c0: 726d 6174 5f2c 0a20 2020 2020 2020 2020  rmat_,.         
-0000c7d0: 2020 2020 2020 2020 2020 2022 2d2d 6e6f             "--no
-0000c7e0: 2d70 6c61 796c 6973 7422 2069 6620 6e6f  -playlist" if no
-0000c7f0: 7420 706c 6179 6c69 7374 5f20 656c 7365  t playlist_ else
-0000c800: 2022 222c 0a20 2020 2020 2020 2020 2020   "",.           
-0000c810: 2020 2020 2020 2020 2022 2d2d 656d 6265           "--embe
-0000c820: 642d 6d65 7461 6461 7461 222c 0a20 2020  d-metadata",.   
-0000c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c840: 2022 2d6f 222c 0a20 2020 2020 2020 2020   "-o",.         
-0000c850: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
-0000c860: 7468 2e6a 6f69 6e28 4d41 4553 5452 4f5f  th.join(MAESTRO_
-0000c870: 4449 522c 2022 2528 7469 746c 6529 732e  DIR, "%(title)s.
-0000c880: 2528 6578 7429 7322 292c 0a20 2020 2020  %(ext)s"),.     
-0000c890: 2020 2020 2020 2020 2020 205d 2c0a 2020             ],.  
-0000c8a0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-0000c8b0: 6563 6b3d 5472 7565 2c0a 2020 2020 2020  eck=True,.      
-0000c8c0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000c8d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000c8e0: 2020 6966 2066 6f72 6d61 745f 203d 3d20    if format_ == 
-0000c8f0: 2277 6176 223a 0a20 2020 2020 2020 2020  "wav":.         
-0000c900: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
-0000c910: 686f 280a 2020 2020 2020 2020 2020 2020  ho(.            
-0000c920: 2020 2020 2020 2020 2243 616e 6e6f 7420          "Cannot 
-0000c930: 646f 776e 6c6f 6164 2073 6f6e 6773 2066  download songs f
-0000c940: 726f 6d20 5370 6f74 6966 7920 6173 2027  rom Spotify as '
-0000c950: 2e77 6176 272e 2050 6c65 6173 6520 6368  .wav'. Please ch
-0000c960: 6f6f 7365 2061 2064 6966 6665 7265 6e74  oose a different
-0000c970: 2066 6f72 6d61 742e 222c 0a20 2020 2020   format.",.     
-0000c980: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000c990: 673d 2272 6564 222c 0a20 2020 2020 2020  g="red",.       
-0000c9a0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000c9b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000c9c0: 6e0a 0a20 2020 2020 2020 2020 2020 2063  n..            c
-0000c9d0: 7764 203d 206f 732e 6765 7463 7764 2829  wd = os.getcwd()
-0000c9e0: 0a20 2020 2020 2020 2020 2020 206f 732e  .            os.
-0000c9f0: 6368 6469 7228 4d41 4553 5452 4f5f 4449  chdir(MAESTRO_DI
-0000ca00: 5229 0a20 2020 2020 2020 2020 2020 2074  R).            t
-0000ca10: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000ca20: 2020 2020 7375 6270 726f 6365 7373 2e72      subprocess.r
-0000ca30: 756e 280a 2020 2020 2020 2020 2020 2020  un(.            
-0000ca40: 2020 2020 2020 2020 5b0a 2020 2020 2020          [.      
-0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca60: 2020 2273 706f 7464 6c22 2c0a 2020 2020    "spotdl",.    
-0000ca70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca80: 2020 2020 2264 6f77 6e6c 6f61 6422 2c0a      "download",.
+0000c750: 2020 2020 2020 2020 2020 2022 2c22 0a20             ",". 
+0000c760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c790: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7c0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c7f0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000c800: 6577 5f74 6167 7320 3d20 5b5d 0a20 2020  ew_tags = [].   
+0000c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c830: 2020 2020 2020 2020 2020 2020 206e 6577               new
+0000c840: 5f74 6167 7320 2b3d 205b 0a20 2020 2020  _tags += [.     
+0000c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c870: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000c880: 6167 0a20 2020 2020 2020 2020 2020 2020  ag.             
+0000c890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8b0: 2020 2020 2020 2066 6f72 2074 6167 2069         for tag i
+0000c8c0: 6e20 7461 6773 0a20 2020 2020 2020 2020  n tags.         
+0000c8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c8f0: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
+0000c900: 6720 6e6f 7420 696e 206e 6577 5f74 6167  g not in new_tag
+0000c910: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000c920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c940: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+0000c950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c970: 2020 2020 6465 7461 696c 735b 325d 203d      details[2] =
+0000c980: 2022 2c22 2e6a 6f69 6e28 6e65 775f 7461   ",".join(new_ta
+0000c990: 6773 290a 2020 2020 2020 2020 2020 2020  gs).            
+0000c9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9c0: 2020 2020 6c69 6e65 735b 695d 203d 2022      lines[i] = "
+0000c9d0: 7c22 2e6a 6f69 6e28 6465 7461 696c 7329  |".join(details)
+0000c9e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca10: 2070 6c61 7965 725f 6f75 7470 7574 2e70   player_output.p
+0000ca20: 6c61 796c 6973 745b 0a20 2020 2020 2020  laylist[.       
+0000ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca50: 2020 2020 2020 2020 2020 2020 2074 6167               tag
+0000ca60: 6769 6e67 5f69 6473 5b73 6f6e 675f 6964  ging_ids[song_id
+0000ca70: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000caa0: 2020 2020 2020 2020 7061 7468 5f2c 0a20          path_,. 
-0000cab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cac0: 2020 2020 2020 2022 2d2d 6f75 7470 7574         "--output
-0000cad0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000cae0: 2020 2020 2020 2020 2020 2022 7b74 6974             "{tit
-0000caf0: 6c65 7d2e 7b6f 7574 7075 742d 6578 747d  le}.{output-ext}
-0000cb00: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000cb10: 2020 2020 2020 2020 2020 2022 2d2d 666f             "--fo
-0000cb20: 726d 6174 222c 0a20 2020 2020 2020 2020  rmat",.         
-0000cb30: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000cb40: 6f72 6d61 745f 2c0a 2020 2020 2020 2020  ormat_,.        
-0000cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb60: 222d 2d68 6561 646c 6573 7322 2c0a 2020  "--headless",.  
+0000caa0: 2020 5d5b 325d 203d 2064 6574 6169 6c73    ][2] = details
+0000cab0: 5b32 5d0a 2020 2020 2020 2020 2020 2020  [2].            
+0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cad0: 2020 2020 2020 2020 2020 2020 736f 6e67              song
+0000cae0: 735f 6669 6c65 2e63 6c6f 7365 2829 0a0a  s_file.close()..
+0000caf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb10: 2020 2020 2020 2020 736f 6e67 735f 6669          songs_fi
+0000cb20: 6c65 203d 206f 7065 6e28 0a20 2020 2020  le = open(.     
+0000cb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb50: 2020 2020 2020 2053 4f4e 4753 5f49 4e46         SONGS_INF
+0000cb60: 4f5f 5041 5448 2c0a 2020 2020 2020 2020  O_PATH,.        
 0000cb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cb80: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
-0000cb90: 2020 2020 2020 2020 2063 6865 636b 3d54           check=T
-0000cba0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
-0000cbb0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-0000cbc0: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
-0000cbd0: 696f 6e20 6173 2065 7272 3a0a 2020 2020  ion as err:.    
-0000cbe0: 2020 2020 2020 2020 2020 2020 6f73 2e63              os.c
-0000cbf0: 6864 6972 2863 7764 290a 2020 2020 2020  hdir(cwd).      
-0000cc00: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000cc10: 6572 720a 0a20 2020 2020 2020 2070 6174  err..        pat
-0000cc20: 6873 203d 205b 5d0a 2020 2020 2020 2020  hs = [].        
-0000cc30: 666f 7220 666e 616d 6520 696e 206f 732e  for fname in os.
-0000cc40: 6c69 7374 6469 7228 4d41 4553 5452 4f5f  listdir(MAESTRO_
-0000cc50: 4449 5229 3a0a 2020 2020 2020 2020 2020  DIR):.          
-0000cc60: 2020 666f 7220 6620 696e 205b 222e 7761    for f in [".wa
-0000cc70: 7622 2c20 222e 6d70 3322 2c20 222e 666c  v", ".mp3", ".fl
-0000cc80: 6163 222c 2022 2e6f 6767 225d 3a0a 2020  ac", ".ogg"]:.  
-0000cc90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000cca0: 2066 6e61 6d65 2e65 6e64 7377 6974 6828   fname.endswith(
-0000ccb0: 6629 3a0a 2020 2020 2020 2020 2020 2020  f):.            
-0000ccc0: 2020 2020 2020 2020 7261 775f 7061 7468          raw_path
-0000ccd0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-0000cce0: 4d41 4553 5452 4f5f 4449 522c 2066 6e61  MAESTRO_DIR, fna
-0000ccf0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0000cd00: 2020 2020 2020 2020 7361 6e69 7469 7a65          sanitize
-0000cd10: 645f 7061 7468 203d 2072 6177 5f70 6174  d_path = raw_pat
-0000cd20: 682e 7265 706c 6163 6528 227c 222c 2022  h.replace("|", "
-0000cd30: 2d22 290a 0a20 2020 2020 2020 2020 2020  -")..           
-0000cd40: 2020 2020 2020 2020 206f 732e 7265 6e61           os.rena
-0000cd50: 6d65 2872 6177 5f70 6174 682c 2073 616e  me(raw_path, san
-0000cd60: 6974 697a 6564 5f70 6174 6829 0a0a 2020  itized_path)..  
-0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd80: 2020 7061 7468 732e 6170 7065 6e64 2873    paths.append(s
-0000cd90: 616e 6974 697a 6564 5f70 6174 6829 0a20  anitized_path). 
-0000cda0: 2020 2020 2020 2020 2020 2069 6620 666e             if fn
-0000cdb0: 616d 652e 656e 6473 7769 7468 2822 2e70  ame.endswith(".p
-0000cdc0: 6172 7422 293a 2020 2320 6465 6c65 7465  art"):  # delete
-0000cdd0: 2069 6e63 6f6d 706c 6574 6520 646f 776e   incomplete down
-0000cde0: 6c6f 6164 730a 2020 2020 2020 2020 2020  loads.          
-0000cdf0: 2020 2020 2020 6f73 2e72 656d 6f76 6528        os.remove(
-0000ce00: 6f73 2e70 6174 682e 6a6f 696e 284d 4145  os.path.join(MAE
-0000ce10: 5354 524f 5f44 4952 2c20 666e 616d 6529  STRO_DIR, fname)
-0000ce20: 290a 0a20 2020 2020 2020 206d 6f76 655f  )..        move_
-0000ce30: 203d 2054 7275 650a 0a20 2020 2069 6620   = True..    if 
-0000ce40: 7061 7468 7320 6973 204e 6f6e 653a 0a20  paths is None:. 
-0000ce50: 2020 2020 2020 2069 6620 6f73 2e70 6174         if os.pat
-0000ce60: 682e 6973 6469 7228 7061 7468 5f29 3a0a  h.isdir(path_):.
-0000ce70: 2020 2020 2020 2020 2020 2020 7061 7468              path
-0000ce80: 7320 3d20 5b5d 0a20 2020 2020 2020 2020  s = [].         
-0000ce90: 2020 2069 6620 7265 6375 7273 653a 0a20     if recurse:. 
-0000cea0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ceb0: 6f72 2064 6972 7061 7468 2c20 5f2c 2066  or dirpath, _, f
-0000cec0: 6e61 6d65 7320 696e 206f 732e 7761 6c6b  names in os.walk
-0000ced0: 2870 6174 685f 293a 0a20 2020 2020 2020  (path_):.       
-0000cee0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000cef0: 2066 6e61 6d65 2069 6e20 666e 616d 6573   fname in fnames
-0000cf00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000cf10: 2020 2020 2020 2020 2020 6966 206f 732e            if os.
-0000cf20: 7061 7468 2e73 706c 6974 6578 7428 666e  path.splitext(fn
-0000cf30: 616d 6529 5b31 5d20 696e 2045 5854 533a  ame)[1] in EXTS:
-0000cf40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cf50: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-0000cf60: 6873 2e61 7070 656e 6428 6f73 2e70 6174  hs.append(os.pat
-0000cf70: 682e 6a6f 696e 2864 6972 7061 7468 2c20  h.join(dirpath, 
-0000cf80: 666e 616d 6529 290a 2020 2020 2020 2020  fname)).        
-0000cf90: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000cfa0: 2020 2020 2020 2020 2020 666f 7220 666e            for fn
-0000cfb0: 616d 6520 696e 206f 732e 6c69 7374 6469  ame in os.listdi
-0000cfc0: 7228 7061 7468 5f29 3a0a 2020 2020 2020  r(path_):.      
-0000cfd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000cfe0: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
-0000cff0: 7428 666e 616d 6529 5b31 5d20 696e 2045  t(fname)[1] in E
-0000d000: 5854 533a 0a20 2020 2020 2020 2020 2020  XTS:.           
-0000d010: 2020 2020 2020 2020 2020 2020 2066 756c               ful
-0000d020: 6c5f 7061 7468 203d 206f 732e 7061 7468  l_path = os.path
-0000d030: 2e6a 6f69 6e28 7061 7468 5f2c 2066 6e61  .join(path_, fna
-0000d040: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
-0000d050: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-0000d060: 732e 7061 7468 2e69 7366 696c 6528 6675  s.path.isfile(fu
-0000d070: 6c6c 5f70 6174 6829 3a0a 2020 2020 2020  ll_path):.      
-0000d080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d090: 2020 2020 2020 7061 7468 732e 6170 7065        paths.appe
-0000d0a0: 6e64 2866 756c 6c5f 7061 7468 290a 2020  nd(full_path).  
-0000d0b0: 2020 2020 2020 2020 2020 6966 206c 656e            if len
-0000d0c0: 2870 6174 6873 2920 3d3d 2030 3a0a 2020  (paths) == 0:.  
-0000d0d0: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-0000d0e0: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
-0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000d100: 224e 6f20 736f 6e67 7320 666f 756e 6420  "No songs found 
-0000d110: 696e 2027 7b70 6174 685f 7d27 2e22 2c0a  in '{path_}'.",.
-0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d130: 2020 2020 6667 3d22 7265 6422 2c0a 2020      fg="red",.  
-0000d140: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d160: 7265 7475 726e 0a20 2020 2020 2020 2065  return.        e
-0000d170: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000d180: 2070 6174 6873 203d 205b 7061 7468 5f5d   paths = [path_]
-0000d190: 0a0a 2020 2020 6966 206c 656e 2870 6174  ..    if len(pat
-0000d1a0: 6873 2920 3e20 313a 0a20 2020 2020 2020  hs) > 1:.       
-0000d1b0: 2069 6620 636c 6970 2069 7320 6e6f 7420   if clip is not 
-0000d1c0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000d1d0: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
-0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000d1f0: 4361 6e6e 6f74 2070 6173 7320 272d 632f  Cannot pass '-c/
-0000d200: 2d2d 636c 6970 2720 6f70 7469 6f6e 2077  --clip' option w
-0000d210: 6865 6e20 6164 6469 6e67 206d 756c 7469  hen adding multi
-0000d220: 706c 6520 736f 6e67 732e 222c 0a20 2020  ple songs.",.   
-0000d230: 2020 2020 2020 2020 2020 2020 2066 673d               fg=
-0000d240: 2272 6564 222c 0a20 2020 2020 2020 2020  "red",.         
-0000d250: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000d260: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-0000d270: 2069 6620 6e61 6d65 2069 7320 6e6f 7420   if name is not 
-0000d280: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000d290: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
-0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000d2b0: 4361 6e6e 6f74 2070 6173 7320 272d 6e2f  Cannot pass '-n/
-0000d2c0: 2d2d 6e61 6d65 2720 6f70 7469 6f6e 2077  --name' option w
-0000d2d0: 6865 6e20 6164 6469 6e67 206d 756c 7469  hen adding multi
-0000d2e0: 706c 6520 736f 6e67 732e 222c 0a20 2020  ple songs.",.   
-0000d2f0: 2020 2020 2020 2020 2020 2020 2066 673d               fg=
-0000d300: 2272 6564 222c 0a20 2020 2020 2020 2020  "red",.         
-0000d310: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000d320: 2072 6574 7572 6e0a 0a20 2020 2069 6620   return..    if 
-0000d330: 6c65 6e28 7061 7468 7329 203d 3d20 3120  len(paths) == 1 
-0000d340: 616e 6420 6e61 6d65 2069 7320 6e6f 7420  and name is not 
-0000d350: 4e6f 6e65 3a0a 2020 2020 2020 2020 6e65  None:.        ne
-0000d360: 775f 7061 7468 203d 206f 732e 7061 7468  w_path = os.path
-0000d370: 2e6a 6f69 6e28 0a20 2020 2020 2020 2020  .join(.         
-0000d380: 2020 204d 4145 5354 524f 5f44 4952 2c20     MAESTRO_DIR, 
-0000d390: 6e61 6d65 202b 206f 732e 7061 7468 2e73  name + os.path.s
-0000d3a0: 706c 6974 6578 7428 7061 7468 735b 305d  plitext(paths[0]
-0000d3b0: 295b 315d 0a20 2020 2020 2020 2029 0a20  )[1].        ). 
-0000d3c0: 2020 2020 2020 206d 6f76 6528 7061 7468         move(path
-0000d3d0: 735b 305d 2c20 6e65 775f 7061 7468 290a  s[0], new_path).
-0000d3e0: 2020 2020 2020 2020 7061 7468 7320 3d20          paths = 
-0000d3f0: 5b6e 6577 5f70 6174 685d 0a0a 2020 2020  [new_path]..    
-0000d400: 6966 2063 6c69 7020 6973 206e 6f74 204e  if clip is not N
-0000d410: 6f6e 6520 616e 6420 6c65 6e28 7061 7468  one and len(path
-0000d420: 7329 203d 3d20 313a 0a20 2020 2020 2020  s) == 1:.       
-0000d430: 2073 6f6e 675f 6475 7261 7469 6f6e 203d   song_duration =
-0000d440: 206d 7573 6963 5f74 6167 2e6c 6f61 645f   music_tag.load_
-0000d450: 6669 6c65 2870 6174 6873 5b30 5d29 5b22  file(paths[0])["
-0000d460: 236c 656e 6774 6822 5d2e 7661 6c75 650a  #length"].value.
-0000d470: 0a20 2020 2020 2020 2073 7461 7274 2c20  .        start, 
-0000d480: 656e 6420 3d20 636c 6970 0a20 2020 2020  end = clip.     
-0000d490: 2020 2069 6620 7374 6172 7420 3c20 303a     if start < 0:
-0000d4a0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-0000d4b0: 636b 2e73 6563 686f 2822 436c 6970 2073  ck.secho("Clip s
-0000d4c0: 7461 7274 2074 696d 6520 6361 6e6e 6f74  tart time cannot
-0000d4d0: 2062 6520 6e65 6761 7469 7665 2e22 2c20   be negative.", 
-0000d4e0: 6667 3d22 7265 6422 290a 2020 2020 2020  fg="red").      
-0000d4f0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000d500: 2020 2020 2065 6c69 6620 7374 6172 7420       elif start 
-0000d510: 3e20 736f 6e67 5f64 7572 6174 696f 6e3a  > song_duration:
-0000d520: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-0000d530: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
-0000d540: 2020 2020 2020 2020 2020 2243 6c69 7020            "Clip 
-0000d550: 7374 6172 7420 7469 6d65 2063 616e 6e6f  start time canno
-0000d560: 7420 6265 2067 7265 6174 6572 2074 6861  t be greater tha
-0000d570: 6e20 7468 6520 736f 6e67 2064 7572 6174  n the song durat
-0000d580: 696f 6e2e 222c 0a20 2020 2020 2020 2020  ion.",.         
-0000d590: 2020 2020 2020 2066 673d 2272 6564 222c         fg="red",
-0000d5a0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000d5b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000d5c0: 6e0a 0a20 2020 2020 2020 2069 6620 656e  n..        if en
-0000d5d0: 6420 3d3d 202d 313a 0a20 2020 2020 2020  d == -1:.       
-0000d5e0: 2020 2020 2065 6e64 203d 2073 6f6e 675f       end = song_
-0000d5f0: 6475 7261 7469 6f6e 0a20 2020 2020 2020  duration.       
-0000d600: 2065 6c69 6620 656e 6420 3c20 7374 6172   elif end < star
-0000d610: 743a 0a20 2020 2020 2020 2020 2020 2063  t:.            c
-0000d620: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
-0000d630: 2020 2020 2020 2020 2020 2020 2243 6c69              "Cli
-0000d640: 7020 656e 6420 7469 6d65 2063 616e 6e6f  p end time canno
-0000d650: 7420 6265 206c 6573 7320 7468 616e 2074  t be less than t
-0000d660: 6865 2063 6c69 7020 7374 6172 7420 7469  he clip start ti
-0000d670: 6d65 2e22 2c0a 2020 2020 2020 2020 2020  me.",.          
-0000d680: 2020 2020 2020 6667 3d22 7265 6422 2c0a        fg="red",.
-0000d690: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000d6a0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d6b0: 0a20 2020 2020 2020 2065 6c69 6620 656e  .        elif en
-0000d6c0: 6420 3e20 736f 6e67 5f64 7572 6174 696f  d > song_duratio
-0000d6d0: 6e3a 0a20 2020 2020 2020 2020 2020 2063  n:.            c
-0000d6e0: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
-0000d6f0: 2020 2020 2020 2020 2020 2020 2243 6c69              "Cli
-0000d700: 7020 656e 6420 7469 6d65 2063 616e 6e6f  p end time canno
-0000d710: 7420 6265 2067 7265 6174 6572 2074 6861  t be greater tha
-0000d720: 6e20 7468 6520 736f 6e67 2064 7572 6174  n the song durat
-0000d730: 696f 6e2e 222c 0a20 2020 2020 2020 2020  ion.",.         
-0000d740: 2020 2020 2020 2066 673d 2272 6564 222c         fg="red",
-0000d750: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000d760: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000d770: 6e0a 2020 2020 656c 7365 3a0a 2020 2020  n.    else:.    
-0000d780: 2020 2020 7374 6172 7420 3d20 656e 6420      start = end 
-0000d790: 3d20 4e6f 6e65 0a0a 2020 2020 6966 206d  = None..    if m
-0000d7a0: 6574 6164 6174 615f 7061 6972 7320 6973  etadata_pairs is
-0000d7b0: 206e 6f74 204e 6f6e 6520 616e 6420 6c65   not None and le
-0000d7c0: 6e28 7061 7468 7329 203d 3d20 313a 0a20  n(paths) == 1:. 
-0000d7d0: 2020 2020 2020 2023 2063 6f6e 7665 7274         # convert
-0000d7e0: 2066 726f 6d20 226b 6579 3a76 616c 7565   from "key:value
-0000d7f0: 2c6b 6579 3a76 616c 7565 2220 746f 205b  ,key:value" to [
-0000d800: 2822 6b65 7922 2c20 2276 616c 7565 2229  ("key", "value")
-0000d810: 5d0a 2020 2020 2020 2020 6d65 7461 6461  ].        metada
-0000d820: 7461 5f70 6169 7273 203d 205b 0a20 2020  ta_pairs = [.   
-0000d830: 2020 2020 2020 2020 2074 7570 6c65 2870           tuple(p
-0000d840: 6169 722e 7374 7269 7028 292e 7370 6c69  air.strip().spli
-0000d850: 7428 223a 2229 2920 666f 7220 7061 6972  t(":")) for pair
-0000d860: 2069 6e20 6d65 7461 6461 7461 5f70 6169   in metadata_pai
-0000d870: 7273 2e73 706c 6974 2822 7c22 290a 2020  rs.split("|").  
-0000d880: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-0000d890: 736f 6e67 5f64 6174 6120 3d20 6d75 7369  song_data = musi
-0000d8a0: 635f 7461 672e 6c6f 6164 5f66 696c 6528  c_tag.load_file(
-0000d8b0: 7061 7468 735b 305d 290a 2020 2020 2020  paths[0]).      
-0000d8c0: 2020 666f 7220 6b65 792c 2076 616c 7565    for key, value
-0000d8d0: 2069 6e20 6d65 7461 6461 7461 5f70 6169   in metadata_pai
-0000d8e0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-0000d8f0: 6966 206b 6579 206e 6f74 2069 6e20 4d45  if key not in ME
-0000d900: 5441 4441 5441 5f4b 4559 5320 6f72 206b  TADATA_KEYS or k
-0000d910: 6579 2e73 7461 7274 7377 6974 6828 2223  ey.startswith("#
-0000d920: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-0000d930: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-0000d940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d950: 2020 2020 2066 2227 7b6b 6579 7d27 2069       f"'{key}' i
-0000d960: 7320 6e6f 7420 6120 7661 6c69 6420 6564  s not a valid ed
-0000d970: 6974 6162 6c65 206d 6574 6164 6174 6120  itable metadata 
-0000d980: 6b65 792e 222c 2066 673d 2272 6564 220a  key.", fg="red".
-0000d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000d9b0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-0000d9c0: 2020 2020 2020 2073 6f6e 675f 6461 7461         song_data
-0000d9d0: 5b6b 6579 5d20 3d20 7661 6c75 650a 2020  [key] = value.  
-0000d9e0: 2020 2020 2020 736f 6e67 5f64 6174 612e        song_data.
-0000d9f0: 7361 7665 2829 0a0a 2020 2020 666f 7220  save()..    for 
-0000da00: 7061 7468 2069 6e20 7061 7468 733a 0a20  path in paths:. 
-0000da10: 2020 2020 2020 2065 7874 203d 206f 732e         ext = os.
-0000da20: 7061 7468 2e73 706c 6974 6578 7428 7061  path.splitext(pa
-0000da30: 7468 295b 315d 0a20 2020 2020 2020 2069  th)[1].        i
-0000da40: 6620 6e6f 7420 6f73 2e70 6174 682e 6973  f not os.path.is
-0000da50: 6469 7228 7061 7468 2920 616e 6420 6578  dir(path) and ex
-0000da60: 7420 6e6f 7420 696e 2045 5854 533a 0a20  t not in EXTS:. 
-0000da70: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-0000da80: 2e73 6563 686f 2866 2227 7b65 7874 7d27  .secho(f"'{ext}'
-0000da90: 2069 7320 6e6f 7420 7375 7070 6f72 7465   is not supporte
-0000daa0: 642e 222c 2066 673d 2272 6564 2229 0a20  d.", fg="red"). 
-0000dab0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000dac0: 6e0a 0a20 2020 2020 2020 2066 6f72 2074  n..        for t
-0000dad0: 6167 2069 6e20 7461 6773 3a0a 2020 2020  ag in tags:.    
-0000dae0: 2020 2020 2020 2020 6966 2022 2c22 2069          if "," i
-0000daf0: 6e20 7461 6720 6f72 2022 7c22 2069 6e20  n tag or "|" in 
-0000db00: 7461 673a 0a20 2020 2020 2020 2020 2020  tag:.           
-0000db10: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
-0000db20: 2822 5461 6773 2063 616e 6e6f 7420 636f  ("Tags cannot co
-0000db30: 6e74 6169 6e20 272c 2720 6f72 2027 7c27  ntain ',' or '|'
-0000db40: 2e22 2c20 6667 3d22 7265 6422 290a 2020  .", fg="red").  
-0000db50: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000db60: 7475 726e 0a0a 2020 2020 2020 2020 7769  turn..        wi
-0000db70: 7468 206f 7065 6e28 534f 4e47 535f 494e  th open(SONGS_IN
-0000db80: 464f 5f50 4154 482c 2022 612b 222c 2065  FO_PATH, "a+", e
-0000db90: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
-0000dba0: 2061 7320 736f 6e67 735f 6669 6c65 3a0a   as songs_file:.
-0000dbb0: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-0000dbc0: 735f 6669 6c65 2e73 6565 6b28 3029 2020  s_file.seek(0)  
-0000dbd0: 2320 7374 6172 7420 7265 6164 696e 6720  # start reading 
-0000dbe0: 6672 6f6d 2062 6567 696e 6e69 6e67 0a0a  from beginning..
-0000dbf0: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-0000dc00: 7320 3d20 736f 6e67 735f 6669 6c65 2e72  s = songs_file.r
-0000dc10: 6561 646c 696e 6573 2829 0a0a 2020 2020  eadlines()..    
-0000dc20: 2020 2020 2020 2020 736f 6e67 5f69 6420          song_id 
-0000dc30: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-0000dc40: 666f 7220 6c69 6e65 2069 6e20 6c69 6e65  for line in line
-0000dc50: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000dc60: 2020 2073 6f6e 675f 6964 203d 206d 6178     song_id = max
-0000dc70: 2873 6f6e 675f 6964 2c20 696e 7428 6c69  (song_id, int(li
-0000dc80: 6e65 2e73 706c 6974 2822 7c22 295b 305d  ne.split("|")[0]
-0000dc90: 2920 2b20 3129 0a0a 2020 2020 2020 2020  ) + 1)..        
-0000dca0: 2020 2020 7072 6570 656e 645f 6e65 776c      prepend_newl
-0000dcb0: 696e 6520 3d20 6c69 6e65 7320 616e 6420  ine = lines and 
-0000dcc0: 6c69 6e65 735b 2d31 5d5b 2d31 5d20 213d  lines[-1][-1] !=
-0000dcd0: 2022 5c6e 220a 0a20 2020 2020 2020 2020   "\n"..         
-0000dce0: 2020 2061 6464 5f73 6f6e 6728 0a20 2020     add_song(.   
-0000dcf0: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-0000dd00: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
-0000dd10: 2020 2074 6167 732c 0a20 2020 2020 2020     tags,.       
-0000dd20: 2020 2020 2020 2020 206d 6f76 655f 2c0a           move_,.
-0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd40: 736f 6e67 735f 6669 6c65 2c0a 2020 2020  songs_file,.    
-0000dd50: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-0000dd60: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-0000dd70: 2020 2073 6f6e 675f 6964 2c0a 2020 2020     song_id,.    
-0000dd80: 2020 2020 2020 2020 2020 2020 7072 6570              prep
-0000dd90: 656e 645f 6e65 776c 696e 652c 0a20 2020  end_newline,.   
-0000dda0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
-0000ddb0: 7274 2c0a 2020 2020 2020 2020 2020 2020  rt,.            
-0000ddc0: 2020 2020 656e 642c 0a20 2020 2020 2020      end,.       
-0000ddd0: 2020 2020 2020 2020 2076 6973 7561 6c69           visuali
-0000dde0: 7a65 2c0a 2020 2020 2020 2020 2020 2020  ze,.            
-0000ddf0: 290a 0a0a 4063 6c69 2e63 6f6d 6d61 6e64  )...@cli.command
-0000de00: 2829 0a40 636c 6963 6b2e 6172 6775 6d65  ().@click.argume
-0000de10: 6e74 2822 4152 4753 222c 2072 6571 7569  nt("ARGS", requi
-0000de20: 7265 643d 5472 7565 2c20 6e61 7267 733d  red=True, nargs=
-0000de30: 2d31 290a 4063 6c69 636b 2e6f 7074 696f  -1).@click.optio
-0000de40: 6e28 0a20 2020 2022 2d46 2f2d 6e46 222c  n(.    "-F/-nF",
-0000de50: 2022 2d2d 666f 7263 652f 2d2d 6e6f 2d66   "--force/--no-f
-0000de60: 6f72 6365 222c 2064 6566 6175 6c74 3d46  orce", default=F
-0000de70: 616c 7365 2c20 6865 6c70 3d22 466f 7263  alse, help="Forc
-0000de80: 6520 6465 6c65 7469 6f6e 2e22 0a29 0a40  e deletion.".).@
-0000de90: 636c 6963 6b2e 6f70 7469 6f6e 280a 2020  click.option(.  
-0000dea0: 2020 222d 542f 2d6e 5422 2c0a 2020 2020    "-T/-nT",.    
-0000deb0: 222d 2d74 6167 2f2d 2d6e 6f2d 7461 6722  "--tag/--no-tag"
-0000dec0: 2c0a 2020 2020 6465 6661 756c 743d 4661  ,.    default=Fa
-0000ded0: 6c73 652c 0a20 2020 2068 656c 703d 2249  lse,.    help="I
-0000dee0: 6620 7061 7373 6564 2c20 7472 6561 7420  f passed, treat 
-0000def0: 616c 6c20 6172 6775 6d65 6e74 7320 6173  all arguments as
-0000df00: 2074 6167 732c 2064 656c 6574 696e 6720   tags, deleting 
-0000df10: 6576 6572 7920 6f63 7572 7265 6e63 6520  every ocurrence 
-0000df20: 6f66 2065 6163 6820 7461 672e 222c 0a29  of each tag.",.)
-0000df30: 0a64 6566 2072 656d 6f76 6528 6172 6773  .def remove(args
-0000df40: 2c20 666f 7263 652c 2074 6167 293a 0a20  , force, tag):. 
-0000df50: 2020 2022 2222 5265 6d6f 7665 2065 6974     """Remove eit
-0000df60: 6865 7220 7461 6728 7329 206f 7220 736f  her tag(s) or so
-0000df70: 6e67 2873 2920 7061 7373 6564 2061 7320  ng(s) passed as 
-0000df80: 4944 2873 292e 2222 220a 2020 2020 6966  ID(s).""".    if
-0000df90: 206e 6f74 2074 6167 3a0a 2020 2020 2020   not tag:.      
-0000dfa0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0000dfb0: 2020 2073 6f6e 675f 6964 7320 3d20 7b69     song_ids = {i
-0000dfc0: 6e74 2873 6f6e 675f 6964 2920 666f 7220  nt(song_id) for 
-0000dfd0: 736f 6e67 5f69 6420 696e 2061 7267 737d  song_id in args}
-0000dfe0: 0a20 2020 2020 2020 2020 2020 2072 656d  .            rem
-0000dff0: 6169 6e69 6e67 5f73 6f6e 675f 6964 7320  aining_song_ids 
-0000e000: 3d20 7b6e 2066 6f72 206e 2069 6e20 736f  = {n for n in so
-0000e010: 6e67 5f69 6473 7d0a 2020 2020 2020 2020  ng_ids}.        
-0000e020: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
-0000e030: 723a 0a20 2020 2020 2020 2020 2020 2063  r:.            c
-0000e040: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
-0000e050: 2020 2020 2020 2020 2020 2020 2253 6f6e              "Son
-0000e060: 6720 4944 7320 6d75 7374 2062 6520 696e  g IDs must be in
-0000e070: 7465 6765 7273 2e20 546f 2064 656c 6574  tegers. To delet
-0000e080: 6520 7461 6773 2c20 7061 7373 2074 6865  e tags, pass the
-0000e090: 2027 2d54 2f2d 2d74 6167 2720 666c 6167   '-T/--tag' flag
-0000e0a0: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-0000e0b0: 2020 2020 6667 3d22 7265 6422 2c0a 2020      fg="red",.  
-0000e0c0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000e0d0: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-0000e0e0: 2020 2020 2020 2020 6966 206e 6f74 2066          if not f
-0000e0f0: 6f72 6365 3a0a 2020 2020 2020 2020 2020  orce:.          
-0000e100: 2020 6368 6172 203d 2069 6e70 7574 280a    char = input(.
-0000e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e120: 6622 4172 6520 796f 7520 7375 7265 2079  f"Are you sure y
-0000e130: 6f75 2077 616e 7420 746f 2064 656c 6574  ou want to delet
-0000e140: 6520 7b6c 656e 2873 6f6e 675f 6964 7329  e {len(song_ids)
-0000e150: 7d20 736f 6e67 2873 293f 205b 792f 6e5d  } song(s)? [y/n]
-0000e160: 2022 0a20 2020 2020 2020 2020 2020 2029   ".            )
-0000e170: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0000e180: 2063 6861 722e 6c6f 7765 7228 2920 213d   char.lower() !=
-0000e190: 2022 7922 3a0a 2020 2020 2020 2020 2020   "y":.          
-0000e1a0: 2020 2020 2020 7072 696e 7428 2244 6964        print("Did
-0000e1b0: 206e 6f74 2064 656c 6574 652e 2229 0a20   not delete."). 
-0000e1c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000e1d0: 6574 7572 6e0a 0a20 2020 2020 2020 2077  eturn..        w
-0000e1e0: 6974 6820 6f70 656e 2853 4f4e 4753 5f49  ith open(SONGS_I
-0000e1f0: 4e46 4f5f 5041 5448 2c20 2272 222c 2065  NFO_PATH, "r", e
-0000e200: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
-0000e210: 2061 7320 736f 6e67 735f 6669 6c65 3a0a   as songs_file:.
-0000e220: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
-0000e230: 7320 3d20 736f 6e67 735f 6669 6c65 2e72  s = songs_file.r
-0000e240: 6561 6428 292e 7370 6c69 746c 696e 6573  ead().splitlines
-0000e250: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-0000e260: 746f 5f62 655f 6465 6c65 7465 6420 3d20  to_be_deleted = 
-0000e270: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
-0000e280: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-0000e290: 6e28 6c69 6e65 7329 293a 0a20 2020 2020  n(lines)):.     
-0000e2a0: 2020 2020 2020 2020 2020 2064 6574 6169             detai
-0000e2b0: 6c73 203d 206c 696e 6573 5b69 5d2e 7374  ls = lines[i].st
-0000e2c0: 7269 7028 292e 7370 6c69 7428 227c 2229  rip().split("|")
+0000cb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb90: 2020 2020 2277 222c 0a20 2020 2020 2020      "w",.       
+0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbc0: 2020 2020 2065 6e63 6f64 696e 673d 2275       encoding="u
+0000cbd0: 7466 2d38 222c 0a20 2020 2020 2020 2020  tf-8",.         
+0000cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cbf0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000cc00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc20: 2020 2020 2020 2020 2073 6f6e 6773 5f66           songs_f
+0000cc30: 696c 652e 7772 6974 6528 225c 6e22 2e6a  ile.write("\n".j
+0000cc40: 6f69 6e28 6c69 6e65 7329 290a 2020 2020  oin(lines)).    
+0000cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc70: 2020 2020 736f 6e67 735f 6669 6c65 2e63      songs_file.c
+0000cc80: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
+0000cc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccb0: 706c 6179 6572 5f6f 7574 7075 742e 7072  player_output.pr
+0000ccc0: 6f6d 7074 696e 6720 3d20 4e6f 6e65 0a20  ompting = None. 
+0000ccd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ccf0: 2020 2020 2020 2063 7572 7365 732e 6375         curses.cu
+0000cd00: 7273 5f73 6574 2846 616c 7365 290a 2020  rs_set(False).  
+0000cd10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd30: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+0000cd40: 7075 742e 6f75 7470 7574 2870 6c61 7962  put.output(playb
+0000cd50: 6163 6b2e 6375 7272 5f70 6f73 290a 2020  ack.curr_pos).  
+0000cd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd70: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000cd80: 6966 2063 2069 6e20 225c 625c 7837 6622  if c in "\b\x7f"
+0000cd90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdb0: 2020 2020 2020 2320 7079 6c69 6e74 3a20        # pylint: 
+0000cdc0: 6469 7361 626c 653d 756e 7375 6273 6372  disable=unsubscr
+0000cdd0: 6970 7461 626c 652d 6f62 6a65 6374 0a20  iptable-object. 
+0000cde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce00: 2020 2069 6620 706c 6179 6572 5f6f 7574     if player_out
+0000ce10: 7075 742e 7072 6f6d 7074 696e 675b 315d  put.prompting[1]
+0000ce20: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
+0000ce30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce40: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+0000ce50: 6179 6572 5f6f 7574 7075 742e 7072 6f6d  ayer_output.prom
+0000ce60: 7074 696e 6720 3d20 280a 2020 2020 2020  pting = (.      
+0000ce70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce90: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+0000cea0: 7075 742e 7072 6f6d 7074 696e 675b 305d  put.prompting[0]
+0000ceb0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
+0000cec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cee0: 2020 3a20 706c 6179 6572 5f6f 7574 7075    : player_outpu
+0000cef0: 742e 7072 6f6d 7074 696e 675b 315d 202d  t.prompting[1] -
+0000cf00: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+0000cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf20: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0000cf30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf50: 2020 2020 2020 2020 2020 2020 202b 2070               + p
+0000cf60: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
+0000cf70: 6d70 7469 6e67 5b30 5d5b 0a20 2020 2020  mpting[0][.     
+0000cf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfa0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+0000cfb0: 725f 6f75 7470 7574 2e70 726f 6d70 7469  r_output.prompti
+0000cfc0: 6e67 5b31 5d20 3a0a 2020 2020 2020 2020  ng[1] :.        
+0000cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cff0: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d020: 2020 2070 6c61 7965 725f 6f75 7470 7574     player_output
+0000d030: 2e70 726f 6d70 7469 6e67 5b31 5d20 2d20  .prompting[1] - 
+0000d040: 312c 0a20 2020 2020 2020 2020 2020 2020  1,.             
+0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d060: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000d070: 6c61 7965 725f 6f75 7470 7574 2e70 726f  layer_output.pro
+0000d080: 6d70 7469 6e67 5b32 5d2c 0a20 2020 2020  mpting[2],.     
+0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0b0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000d0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0d0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+0000d0e0: 6f75 7470 7574 2e6f 7574 7075 7428 706c  output.output(pl
+0000d0f0: 6179 6261 636b 2e63 7572 725f 706f 7329  ayback.curr_pos)
+0000d100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d120: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d140: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+0000d150: 725f 6f75 7470 7574 2e70 726f 6d70 7469  r_output.prompti
+0000d160: 6e67 203d 2028 0a20 2020 2020 2020 2020  ng = (.         
+0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d180: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000d190: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
+0000d1a0: 3d75 6e73 7562 7363 7269 7074 6162 6c65  =unsubscriptable
+0000d1b0: 2d6f 626a 6563 740a 2020 2020 2020 2020  -object.        
+0000d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1e0: 706c 6179 6572 5f6f 7574 7075 742e 7072  player_output.pr
+0000d1f0: 6f6d 7074 696e 675b 305d 5b0a 2020 2020  ompting[0][.    
+0000d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d220: 2020 2020 2020 2020 3a20 706c 6179 6572          : player
+0000d230: 5f6f 7574 7075 742e 7072 6f6d 7074 696e  _output.promptin
+0000d240: 675b 315d 0a20 2020 2020 2020 2020 2020  g[1].           
+0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d260: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d290: 2020 2020 2020 202b 2063 0a20 2020 2020         + c.     
+0000d2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2c0: 2020 202b 2070 6c61 7965 725f 6f75 7470     + player_outp
+0000d2d0: 7574 2e70 726f 6d70 7469 6e67 5b30 5d5b  ut.prompting[0][
+0000d2e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d300: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+0000d310: 7965 725f 6f75 7470 7574 2e70 726f 6d70  yer_output.promp
+0000d320: 7469 6e67 5b31 5d20 3a0a 2020 2020 2020  ting[1] :.      
+0000d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d350: 2020 5d2c 0a20 2020 2020 2020 2020 2020    ],.           
+0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d370: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+0000d380: 7965 725f 6f75 7470 7574 2e70 726f 6d70  yer_output.promp
+0000d390: 7469 6e67 5b31 5d20 2b20 312c 0a20 2020  ting[1] + 1,.   
+0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d3c0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+0000d3d0: 7574 2e70 726f 6d70 7469 6e67 5b32 5d2c  ut.prompting[2],
+0000d3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d400: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d420: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+0000d430: 725f 6f75 7470 7574 2e6f 7574 7075 7428  r_output.output(
+0000d440: 706c 6179 6261 636b 2e63 7572 725f 706f  playback.curr_po
+0000d450: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+0000d460: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000d470: 7863 6570 7420 2856 616c 7565 4572 726f  xcept (ValueErro
+0000d480: 722c 204f 7665 7266 6c6f 7745 7272 6f72  r, OverflowError
+0000d490: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d4b0: 2020 2070 6173 730a 0a20 2020 2020 2020     pass..       
+0000d4c0: 2020 2020 2069 6620 7379 732e 706c 6174       if sys.plat
+0000d4d0: 666f 726d 203d 3d20 2264 6172 7769 6e22  form == "darwin"
+0000d4e0: 2061 6e64 2063 616e 5f6d 6163 5f6e 6f77   and can_mac_now
+0000d4f0: 5f70 6c61 7969 6e67 3a0a 2020 2020 2020  _playing:.      
+0000d500: 2020 2020 2020 2020 2020 6966 2061 6273            if abs
+0000d510: 286d 6163 5f6e 6f77 5f70 6c61 7969 6e67  (mac_now_playing
+0000d520: 2e70 6f73 202d 2070 6c61 7962 6163 6b2e  .pos - playback.
+0000d530: 6375 7272 5f70 6f73 2920 3e20 323a 0a20  curr_pos) > 2:. 
+0000d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d550: 2020 2070 6c61 7962 6163 6b2e 7365 656b     playback.seek
+0000d560: 286d 6163 5f6e 6f77 5f70 6c61 7969 6e67  (mac_now_playing
+0000d570: 2e70 6f73 290a 2020 2020 2020 2020 2020  .pos).          
+0000d580: 2020 2020 2020 2020 2020 6c61 7374 5f74            last_t
+0000d590: 696d 6573 7461 6d70 203d 206d 6163 5f6e  imestamp = mac_n
+0000d5a0: 6f77 5f70 6c61 7969 6e67 2e70 6f73 0a20  ow_playing.pos. 
+0000d5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5c0: 2020 2075 7064 6174 655f 6e6f 775f 706c     update_now_pl
+0000d5d0: 6179 696e 6720 3d20 5472 7565 0a20 2020  aying = True.   
+0000d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d5f0: 2070 6c61 7965 725f 6f75 7470 7574 2e6f   player_output.o
+0000d600: 7574 7075 7428 706c 6179 6261 636b 2e63  utput(playback.c
+0000d610: 7572 725f 706f 7329 0a20 2020 2020 2020  urr_pos).       
+0000d620: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d640: 2020 206d 6163 5f6e 6f77 5f70 6c61 7969     mac_now_playi
+0000d650: 6e67 2e70 6f73 203d 2072 6f75 6e64 2870  ng.pos = round(p
+0000d660: 6c61 7962 6163 6b2e 6375 7272 5f70 6f73  layback.curr_pos
+0000d670: 290a 0a20 2020 2020 2020 2020 2020 2070  )..            p
+0000d680: 726f 6772 6573 735f 6261 725f 7769 6474  rogress_bar_widt
+0000d690: 6820 3d20 7374 6473 6372 2e67 6574 6d61  h = stdscr.getma
+0000d6a0: 7879 7828 295b 315d 202d 2031 380a 2020  xyx()[1] - 18.  
+0000d6b0: 2020 2020 2020 2020 2020 6672 616d 655f            frame_
+0000d6c0: 6475 7261 7469 6f6e 203d 206d 696e 280a  duration = min(.
+0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000d6f0: 2020 2020 2020 310a 2020 2020 2020 2020        1.        
+0000d700: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+0000d710: 726f 6772 6573 735f 6261 725f 7769 6474  rogress_bar_widt
+0000d720: 6820 3c20 4d49 4e5f 5052 4f47 5245 5353  h < MIN_PROGRESS
+0000d730: 5f42 4152 5f57 4944 5448 0a20 2020 2020  _BAR_WIDTH.     
+0000d740: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000d750: 6c73 6520 706c 6179 6572 5f6f 7574 7075  lse player_outpu
+0000d760: 742e 6475 7261 7469 6f6e 202f 2028 7072  t.duration / (pr
+0000d770: 6f67 7265 7373 5f62 6172 5f77 6964 7468  ogress_bar_width
+0000d780: 202a 2038 290a 2020 2020 2020 2020 2020   * 8).          
+0000d790: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+0000d7a0: 2020 2020 2020 2020 2031 202f 2046 5053           1 / FPS
+0000d7b0: 2069 6620 706c 6179 6572 5f6f 7574 7075   if player_outpu
+0000d7c0: 742e 7669 7375 616c 697a 6520 656c 7365  t.visualize else
+0000d7d0: 2031 2c0a 2020 2020 2020 2020 2020 2020   1,.            
+0000d7e0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000d7f0: 2061 6273 2870 6c61 7962 6163 6b2e 6375   abs(playback.cu
+0000d800: 7272 5f70 6f73 202d 206c 6173 745f 7469  rr_pos - last_ti
+0000d810: 6d65 7374 616d 7029 203e 2066 7261 6d65  mestamp) > frame
+0000d820: 5f64 7572 6174 696f 6e3a 0a20 2020 2020  _duration:.     
+0000d830: 2020 2020 2020 2020 2020 206c 6173 745f             last_
+0000d840: 7469 6d65 7374 616d 7020 3d20 706c 6179  timestamp = play
+0000d850: 6261 636b 2e63 7572 725f 706f 730a 2020  back.curr_pos.  
+0000d860: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+0000d870: 6179 6572 5f6f 7574 7075 742e 6f75 7470  ayer_output.outp
+0000d880: 7574 2870 6c61 7962 6163 6b2e 6375 7272  ut(playback.curr
+0000d890: 5f70 6f73 290a 0a20 2020 2020 2020 2020  _pos)..         
+0000d8a0: 2020 2023 2073 6c65 6570 2830 2e30 3129     # sleep(0.01)
+0000d8b0: 2020 2320 4e4f 5445 3a20 736f 2043 5055    # NOTE: so CPU
+0000d8c0: 2075 7361 6765 2064 6f65 736e 2774 2066   usage doesn't f
+0000d8d0: 6c79 2074 6872 6f75 6768 2074 6865 2072  ly through the r
+0000d8e0: 6f6f 660a 0a20 2020 2020 2020 2023 2072  oof..        # r
+0000d8f0: 6567 696f 6e20 7374 6174 730a 2020 2020  egion stats.    
+0000d900: 2020 2020 7469 6d65 5f6c 6973 7465 6e65      time_listene
+0000d910: 6420 3d20 7469 6d65 2829 202d 2073 7461  d = time() - sta
+0000d920: 7274 5f74 696d 650a 2020 2020 2020 2020  rt_time.        
+0000d930: 6966 2070 6c61 7965 725f 6f75 7470 7574  if player_output
+0000d940: 2e70 6175 7365 643a 0a20 2020 2020 2020  .paused:.       
+0000d950: 2020 2020 2074 696d 655f 6c69 7374 656e       time_listen
+0000d960: 6564 202d 3d20 7469 6d65 2829 202d 2070  ed -= time() - p
+0000d970: 6175 7365 5f73 7461 7274 0a0a 2020 2020  ause_start..    
+0000d980: 2020 2020 7769 7468 206f 7065 6e28 544f      with open(TO
+0000d990: 5441 4c5f 5354 4154 535f 5041 5448 2c20  TAL_STATS_PATH, 
+0000d9a0: 2272 2b22 2c20 656e 636f 6469 6e67 3d22  "r+", encoding="
+0000d9b0: 7574 662d 3822 2920 6173 2073 7461 7473  utf-8") as stats
+0000d9c0: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
+0000d9d0: 2020 206c 696e 6573 203d 2073 7461 7473     lines = stats
+0000d9e0: 5f66 696c 652e 7265 6164 6c69 6e65 7328  _file.readlines(
+0000d9f0: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000da00: 7220 6a20 696e 2072 616e 6765 286c 656e  r j in range(len
+0000da10: 286c 696e 6573 2929 3a0a 2020 2020 2020  (lines)):.      
+0000da20: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
+0000da30: 642c 206c 6973 7465 6e65 6420 3d20 6c69  d, listened = li
+0000da40: 6e65 735b 6a5d 2e73 7472 6970 2829 2e73  nes[j].strip().s
+0000da50: 706c 6974 2822 7c22 290a 2020 2020 2020  plit("|").      
+0000da60: 2020 2020 2020 2020 2020 6966 2073 6f6e            if son
+0000da70: 675f 6964 203d 3d20 706c 6179 6572 5f6f  g_id == player_o
+0000da80: 7574 7075 742e 706c 6179 6c69 7374 5b70  utput.playlist[p
+0000da90: 6c61 7965 725f 6f75 7470 7574 2e69 5d5b  layer_output.i][
+0000daa0: 305d 3a0a 2020 2020 2020 2020 2020 2020  0]:.            
+0000dab0: 2020 2020 2020 2020 6c69 7374 656e 6564          listened
+0000dac0: 203d 2066 6c6f 6174 286c 6973 7465 6e65   = float(listene
+0000dad0: 6429 202b 2074 696d 655f 6c69 7374 656e  d) + time_listen
+0000dae0: 6564 0a20 2020 2020 2020 2020 2020 2020  ed.             
+0000daf0: 2020 2020 2020 206c 696e 6573 5b6a 5d20         lines[j] 
+0000db00: 3d20 6622 7b73 6f6e 675f 6964 7d7c 7b6c  = f"{song_id}|{l
+0000db10: 6973 7465 6e65 647d 5c6e 220a 2020 2020  istened}\n".    
+0000db20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db30: 6272 6561 6b0a 0a20 2020 2020 2020 2020  break..         
+0000db40: 2020 2023 2077 7269 7465 206f 7574 0a20     # write out. 
+0000db50: 2020 2020 2020 2020 2020 2073 7461 7473             stats
+0000db60: 5f66 696c 652e 7365 656b 2830 290a 2020  _file.seek(0).  
+0000db70: 2020 2020 2020 2020 2020 7374 6174 735f            stats_
+0000db80: 6669 6c65 2e77 7269 7465 2822 222e 6a6f  file.write("".jo
+0000db90: 696e 286c 696e 6573 2929 0a20 2020 2020  in(lines)).     
+0000dba0: 2020 2020 2020 2073 7461 7473 5f66 696c         stats_fil
+0000dbb0: 652e 7472 756e 6361 7465 2829 0a0a 2020  e.truncate()..  
+0000dbc0: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+0000dbd0: 4355 525f 5945 4152 5f53 5441 5453 5f50  CUR_YEAR_STATS_P
+0000dbe0: 4154 482c 2022 722b 222c 2065 6e63 6f64  ATH, "r+", encod
+0000dbf0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+0000dc00: 7374 6174 735f 6669 6c65 3a0a 2020 2020  stats_file:.    
+0000dc10: 2020 2020 2020 2020 6c69 6e65 7320 3d20          lines = 
+0000dc20: 7374 6174 735f 6669 6c65 2e72 6561 646c  stats_file.readl
+0000dc30: 696e 6573 2829 0a20 2020 2020 2020 2020  ines().         
+0000dc40: 2020 2066 6f72 206a 2069 6e20 7261 6e67     for j in rang
+0000dc50: 6528 6c65 6e28 6c69 6e65 7329 293a 0a20  e(len(lines)):. 
+0000dc60: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000dc70: 6f6e 675f 6964 2c20 6c69 7374 656e 6564  ong_id, listened
+0000dc80: 203d 206c 696e 6573 5b6a 5d2e 7374 7269   = lines[j].stri
+0000dc90: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
+0000dca0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000dcb0: 6620 736f 6e67 5f69 6420 3d3d 2070 6c61  f song_id == pla
+0000dcc0: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
+0000dcd0: 6973 745b 706c 6179 6572 5f6f 7574 7075  ist[player_outpu
+0000dce0: 742e 695d 5b30 5d3a 0a20 2020 2020 2020  t.i][0]:.       
+0000dcf0: 2020 2020 2020 2020 2020 2020 206c 6973               lis
+0000dd00: 7465 6e65 6420 3d20 666c 6f61 7428 6c69  tened = float(li
+0000dd10: 7374 656e 6564 2920 2b20 7469 6d65 5f6c  stened) + time_l
+0000dd20: 6973 7465 6e65 640a 2020 2020 2020 2020  istened.        
+0000dd30: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+0000dd40: 735b 6a5d 203d 2066 227b 736f 6e67 5f69  s[j] = f"{song_i
+0000dd50: 647d 7c7b 6c69 7374 656e 6564 7d5c 6e22  d}|{listened}\n"
+0000dd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dd70: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
+0000dd80: 2020 2020 2020 2020 2320 7772 6974 6520          # write 
+0000dd90: 6f75 740a 2020 2020 2020 2020 2020 2020  out.            
+0000dda0: 7374 6174 735f 6669 6c65 2e73 6565 6b28  stats_file.seek(
+0000ddb0: 3029 0a20 2020 2020 2020 2020 2020 2073  0).            s
+0000ddc0: 7461 7473 5f66 696c 652e 7772 6974 6528  tats_file.write(
+0000ddd0: 2222 2e6a 6f69 6e28 6c69 6e65 7329 290a  "".join(lines)).
+0000dde0: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+0000ddf0: 735f 6669 6c65 2e74 7275 6e63 6174 6528  s_file.truncate(
+0000de00: 290a 2020 2020 2020 2020 2320 656e 6472  ).        # endr
+0000de10: 6567 696f 6e0a 0a20 2020 2020 2020 2069  egion..        i
+0000de20: 6620 706c 6179 6572 5f6f 7574 7075 742e  f player_output.
+0000de30: 656e 6469 6e67 3a0a 2020 2020 2020 2020  ending:.        
+0000de40: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
+0000de50: 2020 2020 6966 206e 6578 745f 736f 6e67      if next_song
+0000de60: 203d 3d20 2d31 3a0a 2020 2020 2020 2020   == -1:.        
+0000de70: 2020 2020 6966 2070 6c61 7965 725f 6f75      if player_ou
+0000de80: 7470 7574 2e69 203d 3d20 706c 6179 6572  tput.i == player
+0000de90: 5f6f 7574 7075 742e 7363 726f 6c6c 6572  _output.scroller
+0000dea0: 2e70 6f73 3a0a 2020 2020 2020 2020 2020  .pos:.          
+0000deb0: 2020 2020 2020 706c 6179 6572 5f6f 7574        player_out
+0000dec0: 7075 742e 7363 726f 6c6c 6572 2e73 6372  put.scroller.scr
+0000ded0: 6f6c 6c5f 6261 636b 7761 7264 2829 0a20  oll_backward(). 
+0000dee0: 2020 2020 2020 2020 2020 2070 6c61 7965             playe
+0000def0: 725f 6f75 7470 7574 2e69 202d 3d20 310a  r_output.i -= 1.
+0000df00: 2020 2020 2020 2020 656c 6966 206e 6578          elif nex
+0000df10: 745f 736f 6e67 203d 3d20 313a 0a20 2020  t_song == 1:.   
+0000df20: 2020 2020 2020 2020 2069 6620 706c 6179           if play
+0000df30: 6572 5f6f 7574 7075 742e 6920 3d3d 206c  er_output.i == l
+0000df40: 656e 2870 6c61 7965 725f 6f75 7470 7574  en(player_output
+0000df50: 2e70 6c61 796c 6973 7429 202d 2031 3a0a  .playlist) - 1:.
+0000df60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df70: 6966 206c 6f6f 703a 0a20 2020 2020 2020  if loop:.       
+0000df80: 2020 2020 2020 2020 2020 2020 206e 6578               nex
+0000df90: 745f 6e65 7874 5f70 6c61 796c 6973 7420  t_next_playlist 
+0000dfa0: 3d20 6e65 7874 5f70 6c61 796c 6973 745b  = next_playlist[
+0000dfb0: 3a5d 0a20 2020 2020 2020 2020 2020 2020  :].             
+0000dfc0: 2020 2020 2020 2069 6620 7265 7368 7566         if reshuf
+0000dfd0: 666c 653a 0a20 2020 2020 2020 2020 2020  fle:.           
+0000dfe0: 2020 2020 2020 2020 2020 2020 2073 6875               shu
+0000dff0: 6666 6c65 286e 6578 745f 6e65 7874 5f70  ffle(next_next_p
+0000e000: 6c61 796c 6973 7429 0a20 2020 2020 2020  laylist).       
+0000e010: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+0000e020: 7965 725f 6f75 7470 7574 2e70 6c61 796c  yer_output.playl
+0000e030: 6973 742c 206e 6578 745f 706c 6179 6c69  ist, next_playli
+0000e040: 7374 203d 2028 0a20 2020 2020 2020 2020  st = (.         
+0000e050: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+0000e060: 6578 745f 706c 6179 6c69 7374 2c0a 2020  ext_playlist,.  
+0000e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e080: 2020 2020 2020 6e65 7874 5f6e 6578 745f        next_next_
+0000e090: 706c 6179 6c69 7374 2c0a 2020 2020 2020  playlist,.      
+0000e0a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000e0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e0c0: 2020 2020 706c 6179 6572 5f6f 7574 7075      player_outpu
+0000e0d0: 742e 6920 3d20 2d31 0a20 2020 2020 2020  t.i = -1.       
+0000e0e0: 2020 2020 2020 2020 2020 2020 2070 6c61               pla
+0000e0f0: 7965 725f 6f75 7470 7574 2e73 6372 6f6c  yer_output.scrol
+0000e100: 6c65 722e 706f 7320 3d20 300a 2020 2020  ler.pos = 0.    
+0000e110: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000e120: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000e130: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+0000e140: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000e150: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000e160: 6620 706c 6179 6572 5f6f 7574 7075 742e  f player_output.
+0000e170: 6920 3d3d 2070 6c61 7965 725f 6f75 7470  i == player_outp
+0000e180: 7574 2e73 6372 6f6c 6c65 722e 706f 733a  ut.scroller.pos:
+0000e190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e1a0: 2020 2020 2070 6c61 7965 725f 6f75 7470       player_outp
+0000e1b0: 7574 2e73 6372 6f6c 6c65 722e 7363 726f  ut.scroller.scro
+0000e1c0: 6c6c 5f66 6f72 7761 7264 2829 0a20 2020  ll_forward().   
+0000e1d0: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+0000e1e0: 6f75 7470 7574 2e69 202b 3d20 310a 2020  output.i += 1.  
+0000e1f0: 2020 2020 2020 656c 6966 206e 6578 745f        elif next_
+0000e200: 736f 6e67 203d 3d20 303a 0a20 2020 2020  song == 0:.     
+0000e210: 2020 2020 2020 2069 6620 706c 6179 6572         if player
+0000e220: 5f6f 7574 7075 742e 6c6f 6f70 696e 675f  _output.looping_
+0000e230: 6375 7272 656e 745f 736f 6e67 203d 3d20  current_song == 
+0000e240: 4c4f 4f50 5f4d 4f44 4553 5b22 6f6e 6522  LOOP_MODES["one"
+0000e250: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0000e260: 2020 2070 7269 6e74 5f74 6f5f 6c6f 6766     print_to_logf
+0000e270: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+0000e280: 2020 2020 2020 2020 2070 6c61 7965 725f           player_
+0000e290: 6f75 7470 7574 2e6c 6f6f 7069 6e67 5f63  output.looping_c
+0000e2a0: 7572 7265 6e74 5f73 6f6e 672c 204c 4f4f  urrent_song, LOO
+0000e2b0: 505f 4d4f 4445 535b 226f 6e65 225d 0a20  P_MODES["one"]. 
+0000e2c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
 0000e2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e2e0: 2073 6f6e 675f 6964 203d 2069 6e74 2864   song_id = int(d
-0000e2f0: 6574 6169 6c73 5b30 5d29 0a20 2020 2020  etails[0]).     
-0000e300: 2020 2020 2020 2020 2020 2069 6620 736f             if so
-0000e310: 6e67 5f69 6420 696e 2072 656d 6169 6e69  ng_id in remaini
-0000e320: 6e67 5f73 6f6e 675f 6964 733a 0a20 2020  ng_song_ids:.   
-0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e340: 2072 656d 6169 6e69 6e67 5f73 6f6e 675f   remaining_song_
-0000e350: 6964 732e 7265 6d6f 7665 2873 6f6e 675f  ids.remove(song_
-0000e360: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
-0000e370: 2020 2020 2020 2020 746f 5f62 655f 6465          to_be_de
-0000e380: 6c65 7465 642e 6170 7065 6e64 2869 290a  leted.append(i).
-0000e390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e3a0: 2020 2020 2073 6f6e 675f 6e61 6d65 203d       song_name =
-0000e3b0: 2064 6574 6169 6c73 5b31 5d0a 2020 2020   details[1].    
-0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3d0: 6f73 2e72 656d 6f76 6528 2020 2320 7265  os.remove(  # re
-0000e3e0: 6d6f 7665 2061 6374 7561 6c20 736f 6e67  move actual song
-0000e3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e400: 2020 2020 2020 2020 206f 732e 7061 7468           os.path
-0000e410: 2e6a 6f69 6e28 534f 4e47 535f 4449 522c  .join(SONGS_DIR,
-0000e420: 2073 6f6e 675f 6e61 6d65 290a 2020 2020   song_name).    
-0000e430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e440: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000e450: 2020 2020 2020 2023 2072 656d 6f76 6520         # remove 
-0000e460: 6361 6368 6564 2076 6973 7561 6c69 7a61  cached visualiza
-0000e470: 7469 6f6e 2066 7265 7175 656e 6369 6573  tion frequencies
-0000e480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e490: 2020 2020 2066 7265 715f 6361 6368 655f       freq_cache_
-0000e4a0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-0000e4b0: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
-0000e4c0: 2020 2020 2020 2020 2020 2020 2046 5245               FRE
-0000e4d0: 515f 4341 4348 455f 4449 522c 206f 732e  Q_CACHE_DIR, os.
-0000e4e0: 7061 7468 2e73 706c 6974 6578 7428 736f  path.splitext(so
-0000e4f0: 6e67 5f6e 616d 6529 5b30 5d20 2b20 222e  ng_name)[0] + ".
-0000e500: 6e70 7922 0a20 2020 2020 2020 2020 2020  npy".           
-0000e510: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000e520: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e530: 6620 6f73 2e70 6174 682e 6578 6973 7473  f os.path.exists
-0000e540: 2866 7265 715f 6361 6368 655f 7061 7468  (freq_cache_path
-0000e550: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000e560: 2020 2020 2020 2020 2020 206f 732e 7265             os.re
-0000e570: 6d6f 7665 2866 7265 715f 6361 6368 655f  move(freq_cache_
-0000e580: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
-0000e590: 2020 2020 2020 2020 2020 6461 7461 5f63            data_c
-0000e5a0: 6163 6865 5f70 6174 6820 3d20 6f73 2e70  ache_path = os.p
-0000e5b0: 6174 682e 6a6f 696e 280a 2020 2020 2020  ath.join(.      
-0000e5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5d0: 2020 4441 5441 5f43 4143 4845 5f44 4952    DATA_CACHE_DIR
-0000e5e0: 2c20 6f73 2e70 6174 682e 7370 6c69 7465  , os.path.splite
-0000e5f0: 7874 2873 6f6e 675f 6e61 6d65 295b 305d  xt(song_name)[0]
-0000e600: 202b 2022 2e6e 7079 220a 2020 2020 2020   + ".npy".      
-0000e610: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e630: 2020 2020 6966 206f 732e 7061 7468 2e65      if os.path.e
-0000e640: 7869 7374 7328 6461 7461 5f63 6163 6865  xists(data_cache
-0000e650: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
-0000e660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e670: 6f73 2e72 656d 6f76 6528 6461 7461 5f63  os.remove(data_c
-0000e680: 6163 6865 5f70 6174 6829 0a0a 2020 2020  ache_path)..    
-0000e690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6a0: 636c 6963 6b2e 7365 6368 6f28 0a20 2020  click.secho(.   
-0000e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6c0: 2020 2020 2066 2252 656d 6f76 6564 2073       f"Removed s
-0000e6d0: 6f6e 6720 277b 736f 6e67 5f6e 616d 657d  ong '{song_name}
-0000e6e0: 2720 7769 7468 2049 4420 7b73 6f6e 675f  ' with ID {song_
-0000e6f0: 6964 7d2e 222c 0a20 2020 2020 2020 2020  id}.",.         
-0000e700: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000e710: 673d 2267 7265 656e 222c 0a20 2020 2020  g="green",.     
-0000e720: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000e730: 0a0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
-0000e740: 696e 2072 6576 6572 7365 6428 746f 5f62  in reversed(to_b
-0000e750: 655f 6465 6c65 7465 6429 3a0a 2020 2020  e_deleted):.    
-0000e760: 2020 2020 2020 2020 6465 6c20 6c69 6e65          del line
-0000e770: 735b 695d 0a0a 2020 2020 2020 2020 7769  s[i]..        wi
-0000e780: 7468 206f 7065 6e28 534f 4e47 535f 494e  th open(SONGS_IN
-0000e790: 464f 5f50 4154 482c 2022 7722 2c20 656e  FO_PATH, "w", en
-0000e7a0: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-0000e7b0: 6173 2073 6f6e 6773 5f66 696c 653a 0a20  as songs_file:. 
-0000e7c0: 2020 2020 2020 2020 2020 2073 6f6e 6773             songs
-0000e7d0: 5f66 696c 652e 7772 6974 6528 225c 6e22  _file.write("\n"
-0000e7e0: 2e6a 6f69 6e28 6c69 6e65 7329 290a 0a20  .join(lines)).. 
-0000e7f0: 2020 2020 2020 2066 6f72 2073 7461 7473         for stats
-0000e800: 5f66 696c 6520 696e 206f 732e 6c69 7374  _file in os.list
-0000e810: 6469 7228 5354 4154 535f 4449 5229 3a0a  dir(STATS_DIR):.
-0000e820: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000e830: 6f74 2073 7461 7473 5f66 696c 652e 656e  ot stats_file.en
-0000e840: 6473 7769 7468 2822 2e74 7874 2229 3a0a  dswith(".txt"):.
-0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e860: 636f 6e74 696e 7565 0a0a 2020 2020 2020  continue..      
-0000e870: 2020 2020 2020 7374 6174 735f 7061 7468        stats_path
-0000e880: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-0000e890: 5354 4154 535f 4449 522c 2073 7461 7473  STATS_DIR, stats
-0000e8a0: 5f66 696c 6529 0a20 2020 2020 2020 2020  _file).         
-0000e8b0: 2020 2077 6974 6820 6f70 656e 2873 7461     with open(sta
-0000e8c0: 7473 5f70 6174 682c 2022 7222 2c20 656e  ts_path, "r", en
-0000e8d0: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-0000e8e0: 6173 2073 7461 7473 5f66 696c 653a 0a20  as stats_file:. 
-0000e8f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e900: 7461 7473 5f6c 696e 6573 203d 2073 7461  tats_lines = sta
-0000e910: 7473 5f66 696c 652e 7265 6164 2829 2e73  ts_file.read().s
-0000e920: 706c 6974 6c69 6e65 7328 290a 0a20 2020  plitlines()..   
-0000e930: 2020 2020 2020 2020 2020 2020 2074 6f5f               to_
-0000e940: 6265 5f64 656c 6574 6564 203d 205b 5d0a  be_deleted = [].
-0000e950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e960: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-0000e970: 656e 2873 7461 7473 5f6c 696e 6573 2929  en(stats_lines))
-0000e980: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e990: 2020 2020 2020 6465 7461 696c 7320 3d20        details = 
-0000e9a0: 7374 6174 735f 6c69 6e65 735b 695d 2e73  stats_lines[i].s
-0000e9b0: 7472 6970 2829 2e73 706c 6974 2822 7c22  trip().split("|"
-0000e9c0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e9d0: 2020 2020 2020 736f 6e67 5f69 6420 3d20        song_id = 
-0000e9e0: 696e 7428 6465 7461 696c 735b 305d 290a  int(details[0]).
-0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea00: 2020 2020 6966 2073 6f6e 675f 6964 2069      if song_id i
-0000ea10: 6e20 736f 6e67 5f69 6473 3a0a 2020 2020  n song_ids:.    
-0000ea20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea30: 2020 2020 746f 5f62 655f 6465 6c65 7465      to_be_delete
-0000ea40: 642e 6170 7065 6e64 2869 290a 0a20 2020  d.append(i)..   
-0000ea50: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
-0000ea60: 6e20 7265 7665 7273 6564 2874 6f5f 6265  n reversed(to_be
-0000ea70: 5f64 656c 6574 6564 293a 0a20 2020 2020  _deleted):.     
-0000ea80: 2020 2020 2020 2020 2020 2064 656c 2073             del s
-0000ea90: 7461 7473 5f6c 696e 6573 5b69 5d0a 0a20  tats_lines[i].. 
-0000eaa0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-0000eab0: 6f70 656e 2873 7461 7473 5f70 6174 682c  open(stats_path,
-0000eac0: 2022 7722 2c20 656e 636f 6469 6e67 3d22   "w", encoding="
-0000ead0: 7574 662d 3822 2920 6173 2073 7461 7473  utf-8") as stats
-0000eae0: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
-0000eaf0: 2020 2020 2020 2073 7461 7473 5f66 696c         stats_fil
-0000eb00: 652e 7772 6974 6528 225c 6e22 2e6a 6f69  e.write("\n".joi
-0000eb10: 6e28 7374 6174 735f 6c69 6e65 7329 290a  n(stats_lines)).
-0000eb20: 0a20 2020 2020 2020 2069 6620 7265 6d61  .        if rema
-0000eb30: 696e 696e 675f 736f 6e67 5f69 6473 3a0a  ining_song_ids:.
-0000eb40: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-0000eb50: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
-0000eb60: 2020 2020 2020 2020 2066 2243 6f75 6c64           f"Could
-0000eb70: 206e 6f74 2066 696e 6420 7468 6520 666f   not find the fo
-0000eb80: 6c6c 6f77 696e 6720 736f 6e67 2049 4473  llowing song IDs
-0000eb90: 3a20 7b27 2c20 272e 6a6f 696e 286d 6170  : {', '.join(map
-0000eba0: 2873 7472 2c20 7265 6d61 696e 696e 675f  (str, remaining_
-0000ebb0: 736f 6e67 5f69 6473 2929 7d2e 222c 0a20  song_ids))}.",. 
-0000ebc0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000ebd0: 673d 2272 6564 222c 0a20 2020 2020 2020  g="red",.       
-0000ebe0: 2020 2020 2029 0a20 2020 2065 6c73 653a       ).    else:
-0000ebf0: 0a20 2020 2020 2020 2074 6167 735f 746f  .        tags_to
-0000ec00: 5f72 656d 6f76 6520 3d20 7365 7428 6172  _remove = set(ar
-0000ec10: 6773 290a 2020 2020 2020 2020 6966 206e  gs).        if n
-0000ec20: 6f74 2066 6f72 6365 3a0a 2020 2020 2020  ot force:.      
-0000ec30: 2020 2020 2020 6368 6172 203d 2069 6e70        char = inp
-0000ec40: 7574 280a 2020 2020 2020 2020 2020 2020  ut(.            
-0000ec50: 2020 2020 6622 4172 6520 796f 7520 7375      f"Are you su
-0000ec60: 7265 2079 6f75 2077 616e 7420 746f 2064  re you want to d
-0000ec70: 656c 6574 6520 7b6c 656e 2874 6167 735f  elete {len(tags_
-0000ec80: 746f 5f72 656d 6f76 6529 7d20 7461 6728  to_remove)} tag(
-0000ec90: 7329 3f20 5b79 2f6e 5d20 220a 2020 2020  s)? [y/n] ".    
-0000eca0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000ecb0: 2020 2020 2020 2069 6620 6368 6172 2e6c         if char.l
-0000ecc0: 6f77 6572 2829 2021 3d20 2279 223a 0a20  ower() != "y":. 
-0000ecd0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0000ece0: 7269 6e74 2822 4469 6420 6e6f 7420 6465  rint("Did not de
-0000ecf0: 6c65 7465 2e22 290a 2020 2020 2020 2020  lete.").        
-0000ed00: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-0000ed10: 2020 2020 2020 2020 7769 7468 206f 7065          with ope
-0000ed20: 6e28 534f 4e47 535f 494e 464f 5f50 4154  n(SONGS_INFO_PAT
-0000ed30: 482c 2022 7222 2c20 656e 636f 6469 6e67  H, "r", encoding
-0000ed40: 3d22 7574 662d 3822 2920 6173 2073 6f6e  ="utf-8") as son
-0000ed50: 6773 5f66 696c 653a 0a20 2020 2020 2020  gs_file:.       
-0000ed60: 2020 2020 206c 696e 6573 203d 2073 6f6e       lines = son
-0000ed70: 6773 5f66 696c 652e 7265 6164 2829 2e73  gs_file.read().s
-0000ed80: 706c 6974 6c69 6e65 7328 290a 2020 2020  plitlines().    
-0000ed90: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-0000eda0: 2072 616e 6765 286c 656e 286c 696e 6573   range(len(lines
-0000edb0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-0000edc0: 2020 2020 6465 7461 696c 7320 3d20 6c69      details = li
-0000edd0: 6e65 735b 695d 2e73 7472 6970 2829 2e73  nes[i].strip().s
-0000ede0: 706c 6974 2822 7c22 290a 2020 2020 2020  plit("|").      
-0000edf0: 2020 2020 2020 2020 2020 7461 6773 203d            tags =
-0000ee00: 2064 6574 6169 6c73 5b32 5d2e 7370 6c69   details[2].spli
-0000ee10: 7428 222c 2229 0a20 2020 2020 2020 2020  t(",").         
-0000ee20: 2020 2020 2020 2066 6f72 206a 2069 6e20         for j in 
-0000ee30: 7261 6e67 6528 6c65 6e28 7461 6773 2929  range(len(tags))
-0000ee40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ee50: 2020 2020 2020 6966 2074 6167 735b 6a5d        if tags[j]
-0000ee60: 2069 6e20 7461 6773 5f74 6f5f 7265 6d6f   in tags_to_remo
-0000ee70: 7665 3a0a 2020 2020 2020 2020 2020 2020  ve:.            
-0000ee80: 2020 2020 2020 2020 2020 2020 6465 6c20              del 
-0000ee90: 7461 6773 5b6a 5d0a 2020 2020 2020 2020  tags[j].        
-0000eea0: 2020 2020 2020 2020 6465 7461 696c 735b          details[
-0000eeb0: 325d 203d 2022 2c22 2e6a 6f69 6e28 7461  2] = ",".join(ta
-0000eec0: 6773 290a 2020 2020 2020 2020 2020 2020  gs).            
-0000eed0: 2020 2020 6c69 6e65 735b 695d 203d 2022      lines[i] = "
-0000eee0: 7c22 2e6a 6f69 6e28 6465 7461 696c 7329  |".join(details)
-0000eef0: 0a0a 2020 2020 2020 2020 7769 7468 206f  ..        with o
-0000ef00: 7065 6e28 534f 4e47 535f 494e 464f 5f50  pen(SONGS_INFO_P
-0000ef10: 4154 482c 2022 7722 2c20 656e 636f 6469  ATH, "w", encodi
-0000ef20: 6e67 3d22 7574 662d 3822 2920 6173 2073  ng="utf-8") as s
-0000ef30: 6f6e 6773 5f66 696c 653a 0a20 2020 2020  ongs_file:.     
-0000ef40: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
-0000ef50: 652e 7772 6974 6528 225c 6e22 2e6a 6f69  e.write("\n".joi
-0000ef60: 6e28 6c69 6e65 7329 290a 0a20 2020 2020  n(lines))..     
-0000ef70: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
-0000ef80: 2020 2020 2020 2020 2020 2020 6622 4465              f"De
-0000ef90: 6c65 7465 6420 616c 6c20 6f63 6375 7272  leted all occurr
-0000efa0: 656e 6365 7320 6f66 207b 6c65 6e28 7461  ences of {len(ta
-0000efb0: 6773 5f74 6f5f 7265 6d6f 7665 297d 2074  gs_to_remove)} t
-0000efc0: 6167 2873 292e 222c 0a20 2020 2020 2020  ag(s).",.       
-0000efd0: 2020 2020 2066 673d 2267 7265 656e 222c       fg="green",
-0000efe0: 0a20 2020 2020 2020 2029 0a0a 0a40 636c  .        )...@cl
-0000eff0: 692e 636f 6d6d 616e 6428 6e61 6d65 3d22  i.command(name="
-0000f000: 7461 6722 290a 4063 6c69 636b 2e61 7267  tag").@click.arg
-0000f010: 756d 656e 7428 2273 6f6e 675f 6964 7322  ument("song_ids"
-0000f020: 2c20 7479 7065 3d63 6c69 636b 2e49 4e54  , type=click.INT
-0000f030: 2c20 7265 7175 6972 6564 3d54 7275 652c  , required=True,
-0000f040: 206e 6172 6773 3d2d 3129 0a40 636c 6963   nargs=-1).@clic
-0000f050: 6b2e 6f70 7469 6f6e 280a 2020 2020 222d  k.option(.    "-
-0000f060: 7422 2c0a 2020 2020 222d 2d74 6167 222c  t",.    "--tag",
-0000f070: 0a20 2020 2022 7461 6773 222c 0a20 2020  .    "tags",.   
-0000f080: 2068 656c 703d 2254 6167 7320 746f 2061   help="Tags to a
-0000f090: 6464 2e22 2c0a 2020 2020 6d75 6c74 6970  dd.",.    multip
-0000f0a0: 6c65 3d54 7275 652c 0a29 0a64 6566 2074  le=True,.).def t
-0000f0b0: 6167 5f28 736f 6e67 5f69 6473 2c20 7461  ag_(song_ids, ta
-0000f0c0: 6773 293a 0a20 2020 2022 2222 4164 6420  gs):.    """Add 
-0000f0d0: 7461 6773 2074 6f20 6120 736f 6e67 2028  tags to a song (
-0000f0e0: 7061 7373 6564 2061 7320 4944 292e 2054  passed as ID). T
-0000f0f0: 6167 7320 6361 6e6e 6f74 2063 6f6e 7461  ags cannot conta
-0000f100: 696e 2074 6865 2063 6861 7261 6374 6572  in the character
-0000f110: 730a 2020 2020 272c 2720 6f72 2027 7c27  s.    ',' or '|'
-0000f120: 2e22 2222 0a20 2020 2073 6f6e 675f 6964  .""".    song_id
-0000f130: 7320 3d20 7365 7428 736f 6e67 5f69 6473  s = set(song_ids
-0000f140: 290a 2020 2020 6e75 6d5f 736f 6e67 7320  ).    num_songs 
-0000f150: 3d20 6c65 6e28 736f 6e67 5f69 6473 290a  = len(song_ids).
-0000f160: 2020 2020 7461 6773 203d 2073 6574 2874      tags = set(t
-0000f170: 6167 7329 0a20 2020 2066 6f72 2074 6167  ags).    for tag
-0000f180: 2069 6e20 7461 6773 3a0a 2020 2020 2020   in tags:.      
-0000f190: 2020 6966 2022 2c22 2069 6e20 7461 6720    if "," in tag 
-0000f1a0: 6f72 2022 7c22 2069 6e20 7461 673a 0a20  or "|" in tag:. 
-0000f1b0: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-0000f1c0: 2e73 6563 686f 2822 5461 6773 2063 616e  .secho("Tags can
-0000f1d0: 6e6f 7420 636f 6e74 6169 6e20 272c 2720  not contain ',' 
-0000f1e0: 6f72 2027 7c27 2e22 2c20 6667 3d22 7265  or '|'.", fg="re
-0000f1f0: 6422 290a 2020 2020 2020 2020 2020 2020  d").            
-0000f200: 7265 7475 726e 0a20 2020 2069 6620 7461  return.    if ta
-0000f210: 6773 3a0a 2020 2020 2020 2020 736f 6e67  gs:.        song
-0000f220: 735f 6669 6c65 203d 206f 7065 6e28 534f  s_file = open(SO
-0000f230: 4e47 535f 494e 464f 5f50 4154 482c 2022  NGS_INFO_PATH, "
-0000f240: 7222 2c20 656e 636f 6469 6e67 3d22 7574  r", encoding="ut
-0000f250: 662d 3822 290a 2020 2020 2020 2020 6c69  f-8").        li
-0000f260: 6e65 7320 3d20 736f 6e67 735f 6669 6c65  nes = songs_file
-0000f270: 2e72 6561 6428 292e 7370 6c69 746c 696e  .read().splitlin
-0000f280: 6573 2829 0a20 2020 2020 2020 2066 6f72  es().        for
-0000f290: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-0000f2a0: 6c69 6e65 7329 293a 0a20 2020 2020 2020  lines)):.       
-0000f2b0: 2020 2020 2064 6574 6169 6c73 203d 206c       details = l
-0000f2c0: 696e 6573 5b69 5d2e 7374 7269 7028 292e  ines[i].strip().
-0000f2d0: 7370 6c69 7428 227c 2229 0a20 2020 2020  split("|").     
-0000f2e0: 2020 2020 2020 2073 6f6e 675f 6964 203d         song_id =
-0000f2f0: 2069 6e74 2864 6574 6169 6c73 5b30 5d29   int(details[0])
-0000f300: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000f310: 736f 6e67 5f69 6420 696e 2073 6f6e 675f  song_id in song_
-0000f320: 6964 733a 0a20 2020 2020 2020 2020 2020  ids:.           
-0000f330: 2020 2020 2073 6f6e 675f 6964 732e 7265       song_ids.re
-0000f340: 6d6f 7665 2873 6f6e 675f 6964 290a 0a20  move(song_id).. 
-0000f350: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f360: 6620 6465 7461 696c 735b 325d 3a0a 2020  f details[2]:.  
-0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f380: 2020 6e65 775f 7461 6773 203d 2064 6574    new_tags = det
-0000f390: 6169 6c73 5b32 5d2e 7370 6c69 7428 222c  ails[2].split(",
-0000f3a0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000f3b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000f3c0: 2020 2020 2020 2020 2020 2020 206e 6577               new
-0000f3d0: 5f74 6167 7320 3d20 5b5d 0a20 2020 2020  _tags = [].     
-0000f3e0: 2020 2020 2020 2020 2020 206e 6577 5f74             new_t
-0000f3f0: 6167 7320 2b3d 205b 7461 6720 666f 7220  ags += [tag for 
-0000f400: 7461 6720 696e 2074 6167 7320 6966 2074  tag in tags if t
-0000f410: 6167 206e 6f74 2069 6e20 6e65 775f 7461  ag not in new_ta
-0000f420: 6773 5d0a 2020 2020 2020 2020 2020 2020  gs].            
-0000f430: 2020 2020 6465 7461 696c 735b 325d 203d      details[2] =
-0000f440: 2022 2c22 2e6a 6f69 6e28 6e65 775f 7461   ",".join(new_ta
-0000f450: 6773 290a 2020 2020 2020 2020 2020 2020  gs).            
-0000f460: 2020 2020 6c69 6e65 735b 695d 203d 2022      lines[i] = "
-0000f470: 7c22 2e6a 6f69 6e28 6465 7461 696c 7329  |".join(details)
-0000f480: 0a20 2020 2020 2020 2073 6f6e 6773 5f66  .        songs_f
-0000f490: 696c 652e 636c 6f73 6528 290a 0a20 2020  ile.close()..   
-0000f4a0: 2020 2020 2073 6f6e 6773 5f66 696c 6520       songs_file 
-0000f4b0: 3d20 6f70 656e 2853 4f4e 4753 5f49 4e46  = open(SONGS_INF
-0000f4c0: 4f5f 5041 5448 2c20 2277 222c 2065 6e63  O_PATH, "w", enc
-0000f4d0: 6f64 696e 673d 2275 7466 2d38 2229 0a20  oding="utf-8"). 
-0000f4e0: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
-0000f4f0: 652e 7772 6974 6528 225c 6e22 2e6a 6f69  e.write("\n".joi
-0000f500: 6e28 6c69 6e65 7329 290a 2020 2020 2020  n(lines)).      
-0000f510: 2020 736f 6e67 735f 6669 6c65 2e63 6c6f    songs_file.clo
-0000f520: 7365 2829 0a0a 2020 2020 2020 2020 6966  se()..        if
-0000f530: 2073 6f6e 675f 6964 733a 0a20 2020 2020   song_ids:.     
-0000f540: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
-0000f550: 686f 280a 2020 2020 2020 2020 2020 2020  ho(.            
-0000f560: 2020 2020 6622 436f 756c 6420 6e6f 7420      f"Could not 
-0000f570: 6669 6e64 2073 6f6e 6728 7329 2077 6974  find song(s) wit
-0000f580: 6820 4944 2873 2920 7b27 2c20 272e 6a6f  h ID(s) {', '.jo
-0000f590: 696e 286d 6170 2873 7472 2c20 736f 6e67  in(map(str, song
-0000f5a0: 5f69 6473 2929 7d2e 222c 0a20 2020 2020  _ids))}.",.     
-0000f5b0: 2020 2020 2020 2020 2020 2066 673d 2272             fg="r
-0000f5c0: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
-0000f5d0: 2029 0a20 2020 2020 2020 2020 2020 2069   ).            i
-0000f5e0: 6620 6c65 6e28 736f 6e67 5f69 6473 2920  f len(song_ids) 
-0000f5f0: 3d3d 206e 756d 5f73 6f6e 6773 3a0a 2020  == num_songs:.  
-0000f600: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000f610: 7475 726e 0a20 2020 2020 2020 2063 6c69  turn.        cli
-0000f620: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
-0000f630: 2020 2020 2020 6622 4164 6465 6420 7b6c        f"Added {l
-0000f640: 656e 2874 6167 7329 7d20 7461 6728 7329  en(tags)} tag(s)
-0000f650: 2074 6f20 7b6e 756d 5f73 6f6e 6773 202d   to {num_songs -
-0000f660: 206c 656e 2873 6f6e 675f 6964 7329 7d20   len(song_ids)} 
-0000f670: 736f 6e67 2873 292e 222c 0a20 2020 2020  song(s).",.     
-0000f680: 2020 2020 2020 2066 673d 2267 7265 656e         fg="green
-0000f690: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
-0000f6a0: 2065 6c73 653a 0a20 2020 2020 2020 2063   else:.        c
-0000f6b0: 6c69 636b 2e73 6563 686f 2822 4e6f 2074  lick.secho("No t
-0000f6c0: 6167 7320 7061 7373 6564 2e22 2c20 6667  ags passed.", fg
-0000f6d0: 3d22 7265 6422 290a 0a0a 4063 6c69 2e63  ="red")...@cli.c
-0000f6e0: 6f6d 6d61 6e64 2829 0a40 636c 6963 6b2e  ommand().@click.
-0000f6f0: 6172 6775 6d65 6e74 2822 736f 6e67 5f69  argument("song_i
-0000f700: 6473 222c 2074 7970 653d 636c 6963 6b2e  ds", type=click.
-0000f710: 494e 542c 2072 6571 7569 7265 643d 5472  INT, required=Tr
-0000f720: 7565 2c20 6e61 7267 733d 2d31 290a 4063  ue, nargs=-1).@c
-0000f730: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
-0000f740: 2022 2d74 222c 0a20 2020 2022 2d2d 7461   "-t",.    "--ta
-0000f750: 6722 2c0a 2020 2020 2274 6167 7322 2c0a  g",.    "tags",.
-0000f760: 2020 2020 6865 6c70 3d22 5461 6773 2074      help="Tags t
-0000f770: 6f20 7265 6d6f 7665 2e22 2c0a 2020 2020  o remove.",.    
-0000f780: 6d75 6c74 6970 6c65 3d54 7275 652c 0a29  multiple=True,.)
-0000f790: 0a40 636c 6963 6b2e 6f70 7469 6f6e 2822  .@click.option("
-0000f7a0: 2d41 2f2d 6e41 222c 2022 2d2d 616c 6c2f  -A/-nA", "--all/
-0000f7b0: 2d2d 6e6f 2d61 6c6c 222c 2022 616c 6c5f  --no-all", "all_
-0000f7c0: 222c 2064 6566 6175 6c74 3d46 616c 7365  ", default=False
-0000f7d0: 290a 6465 6620 756e 7461 6728 736f 6e67  ).def untag(song
-0000f7e0: 5f69 6473 2c20 7461 6773 2c20 616c 6c5f  _ids, tags, all_
-0000f7f0: 293a 0a20 2020 2022 2222 5265 6d6f 7665  ):.    """Remove
-0000f800: 2074 6167 7320 6672 6f6d 2061 2073 7065   tags from a spe
-0000f810: 6369 6669 6320 736f 6e67 2028 7061 7373  cific song (pass
-0000f820: 6564 2061 7320 4944 292e 2054 6167 7320  ed as ID). Tags 
-0000f830: 7468 6174 2074 6865 2073 6f6e 670a 2020  that the song.  
-0000f840: 2020 646f 6573 6e27 7420 6861 7665 2077    doesn't have w
-0000f850: 696c 6c20 6265 2069 676e 6f72 6564 2e0a  ill be ignored..
-0000f860: 0a20 2020 2050 6173 7369 6e67 2074 6865  .    Passing the
-0000f870: 2027 2d41 2f2d 2d61 6c6c 2720 666c 6167   '-A/--all' flag
-0000f880: 2077 696c 6c20 7265 6d6f 7665 2061 6c6c   will remove all
-0000f890: 2074 6167 7320 6672 6f6d 2074 6865 2073   tags from the s
-0000f8a0: 6f6e 672c 2075 6e6c 6573 7320 5441 4753  ong, unless TAGS
-0000f8b0: 0a20 2020 2069 7320 7061 7373 6564 2028  .    is passed (
-0000f8c0: 696e 2077 6869 6368 2063 6173 6520 7468  in which case th
-0000f8d0: 6520 666c 6167 2069 7320 6967 6e6f 7265  e flag is ignore
-0000f8e0: 6429 2e22 2222 0a20 2020 2073 6f6e 675f  d).""".    song_
-0000f8f0: 6964 7320 3d20 7365 7428 736f 6e67 5f69  ids = set(song_i
-0000f900: 6473 290a 2020 2020 6e75 6d5f 736f 6e67  ds).    num_song
-0000f910: 7320 3d20 6c65 6e28 736f 6e67 5f69 6473  s = len(song_ids
-0000f920: 290a 2020 2020 7461 6773 203d 2073 6574  ).    tags = set
-0000f930: 2874 6167 7329 0a20 2020 2069 6620 7461  (tags).    if ta
-0000f940: 6773 3a0a 2020 2020 2020 2020 736f 6e67  gs:.        song
-0000f950: 735f 6669 6c65 203d 206f 7065 6e28 534f  s_file = open(SO
-0000f960: 4e47 535f 494e 464f 5f50 4154 482c 2022  NGS_INFO_PATH, "
-0000f970: 7222 2c20 656e 636f 6469 6e67 3d22 7574  r", encoding="ut
-0000f980: 662d 3822 290a 2020 2020 2020 2020 6c69  f-8").        li
-0000f990: 6e65 7320 3d20 736f 6e67 735f 6669 6c65  nes = songs_file
-0000f9a0: 2e72 6561 6428 292e 7370 6c69 746c 696e  .read().splitlin
-0000f9b0: 6573 2829 0a20 2020 2020 2020 2066 6f72  es().        for
-0000f9c0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-0000f9d0: 6c69 6e65 7329 293a 0a20 2020 2020 2020  lines)):.       
-0000f9e0: 2020 2020 2064 6574 6169 6c73 203d 206c       details = l
-0000f9f0: 696e 6573 5b69 5d2e 7374 7269 7028 292e  ines[i].strip().
-0000fa00: 7370 6c69 7428 227c 2229 0a20 2020 2020  split("|").     
-0000fa10: 2020 2020 2020 2073 6f6e 675f 6964 203d         song_id =
-0000fa20: 2069 6e74 2864 6574 6169 6c73 5b30 5d29   int(details[0])
-0000fa30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000fa40: 736f 6e67 5f69 6420 696e 2073 6f6e 675f  song_id in song_
-0000fa50: 6964 733a 0a20 2020 2020 2020 2020 2020  ids:.           
-0000fa60: 2020 2020 2073 6f6e 675f 6964 732e 7265       song_ids.re
-0000fa70: 6d6f 7665 2873 6f6e 675f 6964 290a 0a20  move(song_id).. 
-0000fa80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000fa90: 6167 735f 746f 5f6b 6565 7020 3d20 5b0a  ags_to_keep = [.
-0000faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fab0: 2020 2020 7461 6720 666f 7220 7461 6720      tag for tag 
-0000fac0: 696e 2064 6574 6169 6c73 5b32 5d2e 7370  in details[2].sp
-0000fad0: 6c69 7428 222c 2229 2069 6620 7461 6720  lit(",") if tag 
-0000fae0: 6e6f 7420 696e 2074 6167 730a 2020 2020  not in tags.    
-0000faf0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
-0000fb00: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000fb10: 6e65 735b 695d 203d 2022 7c22 2e6a 6f69  nes[i] = "|".joi
-0000fb20: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-0000fb30: 2020 2020 2020 2064 6574 6169 6c73 5b3a         details[:
-0000fb40: 325d 202b 205b 222c 222e 6a6f 696e 2874  2] + [",".join(t
-0000fb50: 6167 735f 746f 5f6b 6565 7029 5d20 2b20  ags_to_keep)] + 
-0000fb60: 6465 7461 696c 735b 333a 5d0a 2020 2020  details[3:].    
-0000fb70: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000fb80: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
-0000fb90: 2e63 6c6f 7365 2829 0a0a 2020 2020 2020  .close()..      
-0000fba0: 2020 736f 6e67 735f 6669 6c65 203d 206f    songs_file = o
-0000fbb0: 7065 6e28 534f 4e47 535f 494e 464f 5f50  pen(SONGS_INFO_P
-0000fbc0: 4154 482c 2022 7722 2c20 656e 636f 6469  ATH, "w", encodi
-0000fbd0: 6e67 3d22 7574 662d 3822 290a 2020 2020  ng="utf-8").    
-0000fbe0: 2020 2020 736f 6e67 735f 6669 6c65 2e77      songs_file.w
-0000fbf0: 7269 7465 2822 5c6e 222e 6a6f 696e 286c  rite("\n".join(l
-0000fc00: 696e 6573 2929 0a20 2020 2020 2020 2073  ines)).        s
-0000fc10: 6f6e 6773 5f66 696c 652e 636c 6f73 6528  ongs_file.close(
-0000fc20: 290a 0a20 2020 2020 2020 2069 6620 736f  )..        if so
-0000fc30: 6e67 5f69 6473 3a0a 2020 2020 2020 2020  ng_ids:.        
-0000fc40: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-0000fc50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc60: 2066 2243 6f75 6c64 206e 6f74 2066 696e   f"Could not fin
-0000fc70: 6420 736f 6e67 2873 2920 7769 7468 2049  d song(s) with I
-0000fc80: 4428 7329 207b 272c 2027 2e6a 6f69 6e28  D(s) {', '.join(
-0000fc90: 6d61 7028 7374 722c 2073 6f6e 675f 6964  map(str, song_id
-0000fca0: 7329 297d 2e22 2c0a 2020 2020 2020 2020  s))}.",.        
-0000fcb0: 2020 2020 2020 2020 6667 3d22 7265 6422          fg="red"
-0000fcc0: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000fcd0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-0000fce0: 656e 2873 6f6e 675f 6964 7329 203d 3d20  en(song_ids) == 
-0000fcf0: 6e75 6d5f 736f 6e67 733a 0a20 2020 2020  num_songs:.     
-0000fd00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000fd10: 6e0a 2020 2020 2020 2020 636c 6963 6b2e  n.        click.
-0000fd20: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
-0000fd30: 2020 2066 2252 656d 6f76 6564 2061 6e79     f"Removed any
-0000fd40: 206f 6363 7572 7265 6e63 6573 206f 6620   occurrences of 
-0000fd50: 7b6c 656e 2874 6167 7329 7d20 7461 6728  {len(tags)} tag(
-0000fd60: 7329 2066 726f 6d20 7b6e 756d 5f73 6f6e  s) from {num_son
-0000fd70: 6773 202d 206c 656e 2873 6f6e 675f 6964  gs - len(song_id
-0000fd80: 7329 7d20 736f 6e67 2873 292e 222c 0a20  s)} song(s).",. 
-0000fd90: 2020 2020 2020 2020 2020 2066 673d 2267             fg="g
-0000fda0: 7265 656e 222c 0a20 2020 2020 2020 2029  reen",.        )
-0000fdb0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0000fdc0: 2020 2069 6620 6e6f 7420 616c 6c5f 3a0a     if not all_:.
-0000fdd0: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-0000fde0: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
-0000fdf0: 2020 2020 2020 2020 2022 4e6f 2074 6167           "No tag
-0000fe00: 7320 7061 7373 6564 e280 9474 6f20 7265  s passed...to re
-0000fe10: 6d6f 7665 2061 6c6c 2074 6167 732c 2070  move all tags, p
-0000fe20: 6173 7320 7468 6520 272d 412f 2d2d 616c  ass the '-A/--al
-0000fe30: 6c27 2066 6c61 672e 222c 0a20 2020 2020  l' flag.",.     
-0000fe40: 2020 2020 2020 2020 2020 2066 673d 2272             fg="r
-0000fe50: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
-0000fe60: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
-0000fe70: 0a20 2020 2020 2020 2020 2020 2073 6f6e  .            son
-0000fe80: 6773 5f66 696c 6520 3d20 6f70 656e 2853  gs_file = open(S
-0000fe90: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
-0000fea0: 2272 222c 2065 6e63 6f64 696e 673d 2275  "r", encoding="u
-0000feb0: 7466 2d38 2229 0a20 2020 2020 2020 2020  tf-8").         
-0000fec0: 2020 206c 696e 6573 203d 2073 6f6e 6773     lines = songs
-0000fed0: 5f66 696c 652e 7265 6164 2829 2e73 706c  _file.read().spl
-0000fee0: 6974 6c69 6e65 7328 290a 2020 2020 2020  itlines().      
-0000fef0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-0000ff00: 616e 6765 286c 656e 286c 696e 6573 2929  ange(len(lines))
-0000ff10: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ff20: 2020 6c69 6e65 203d 206c 696e 6573 5b69    line = lines[i
-0000ff30: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000ff40: 2020 6465 7461 696c 7320 3d20 6c69 6e65    details = line
-0000ff50: 2e73 7472 6970 2829 2e73 706c 6974 2822  .strip().split("
-0000ff60: 7c22 290a 2020 2020 2020 2020 2020 2020  |").            
-0000ff70: 2020 2020 6966 2069 6e74 2864 6574 6169      if int(detai
-0000ff80: 6c73 5b30 5d29 2069 6e20 736f 6e67 5f69  ls[0]) in song_i
-0000ff90: 6473 3a0a 2020 2020 2020 2020 2020 2020  ds:.            
-0000ffa0: 2020 2020 2020 2020 6c69 6e65 735b 695d          lines[i]
-0000ffb0: 203d 2022 7c22 2e6a 6f69 6e28 6465 7461   = "|".join(deta
-0000ffc0: 696c 735b 3a32 5d20 2b20 5b22 225d 202b  ils[:2] + [""] +
-0000ffd0: 2064 6574 6169 6c73 5b33 3a5d 290a 2020   details[3:]).  
-0000ffe0: 2020 2020 2020 2020 2020 736f 6e67 735f            songs_
-0000fff0: 6669 6c65 2e63 6c6f 7365 2829 0a0a 2020  file.close()..  
-00010000: 2020 2020 2020 2020 2020 736f 6e67 735f            songs_
-00010010: 6669 6c65 203d 206f 7065 6e28 534f 4e47  file = open(SONG
-00010020: 535f 494e 464f 5f50 4154 482c 2022 7722  S_INFO_PATH, "w"
-00010030: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-00010040: 3822 290a 2020 2020 2020 2020 2020 2020  8").            
-00010050: 736f 6e67 735f 6669 6c65 2e77 7269 7465  songs_file.write
-00010060: 2822 5c6e 222e 6a6f 696e 286c 696e 6573  ("\n".join(lines
-00010070: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
-00010080: 6f6e 6773 5f66 696c 652e 636c 6f73 6528  ongs_file.close(
-00010090: 290a 0a20 2020 2020 2020 2020 2020 2063  )..            c
-000100a0: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
-000100b0: 2020 2020 2020 2020 2020 2020 6622 5265              f"Re
-000100c0: 6d6f 7665 6420 7b6c 656e 2874 6167 7329  moved {len(tags)
-000100d0: 7d20 7461 6728 7329 2066 726f 6d20 7b6c  } tag(s) from {l
-000100e0: 656e 2873 6f6e 675f 6964 7329 7d20 736f  en(song_ids)} so
-000100f0: 6e67 2873 292e 222c 0a20 2020 2020 2020  ng(s).",.       
-00010100: 2020 2020 2020 2020 2066 673d 2267 7265           fg="gre
-00010110: 656e 222c 0a20 2020 2020 2020 2020 2020  en",.           
-00010120: 2029 0a0a 0a40 636c 692e 636f 6d6d 616e   )...@cli.comman
-00010130: 6428 290a 4063 6c69 636b 2e61 7267 756d  d().@click.argum
-00010140: 656e 7428 2274 6167 7322 2c20 6e61 7267  ent("tags", narg
-00010150: 733d 2d31 290a 4063 6c69 636b 2e6f 7074  s=-1).@click.opt
-00010160: 696f 6e28 0a20 2020 2022 2d73 222c 0a20  ion(.    "-s",. 
-00010170: 2020 2022 2d2d 7368 7566 666c 6522 2c0a     "--shuffle",.
-00010180: 2020 2020 2273 6875 6666 6c65 5f22 2c0a      "shuffle_",.
-00010190: 2020 2020 7479 7065 3d63 6c69 636b 2e49      type=click.I
-000101a0: 6e74 5261 6e67 6528 302c 2032 292c 0a20  ntRange(0, 2),. 
-000101b0: 2020 2068 656c 703d 2230 3a20 7368 7566     help="0: shuf
-000101c0: 666c 6520 6f6e 6365 2c20 313a 2073 6875  fle once, 1: shu
-000101d0: 6666 6c65 2065 7665 7279 206c 6f6f 702c  ffle every loop,
-000101e0: 2032 3a20 7368 7566 666c 6520 6576 6572   2: shuffle ever
-000101f0: 7920 6c6f 6f70 2065 7863 6570 7420 666f  y loop except fo
-00010200: 7220 7468 6520 6669 7273 7420 6f6e 652e  r the first one.
-00010210: 222c 0a29 0a40 636c 6963 6b2e 6f70 7469  ",.).@click.opti
-00010220: 6f6e 280a 2020 2020 222d 522f 2d6e 5222  on(.    "-R/-nR"
-00010230: 2c0a 2020 2020 222d 2d72 6576 6572 7365  ,.    "--reverse
-00010240: 2f2d 2d6e 6f2d 7265 7665 7273 6522 2c0a  /--no-reverse",.
-00010250: 2020 2020 2272 6576 6572 7365 222c 0a20      "reverse",. 
-00010260: 2020 2064 6566 6175 6c74 3d46 616c 7365     default=False
-00010270: 2c0a 2020 2020 6865 6c70 3d22 506c 6179  ,.    help="Play
-00010280: 2073 6f6e 6773 2069 6e20 7265 7665 7273   songs in revers
-00010290: 6520 286d 6f73 7420 7265 6365 6e74 6c79  e (most recently
-000102a0: 2061 6464 6564 2066 6972 7374 292e 222c   added first).",
-000102b0: 0a29 0a40 636c 6963 6b2e 6f70 7469 6f6e  .).@click.option
-000102c0: 280a 2020 2020 222d 6f22 2c0a 2020 2020  (.    "-o",.    
-000102d0: 222d 2d6f 6e6c 7922 2c0a 2020 2020 226f  "--only",.    "o
-000102e0: 6e6c 7922 2c0a 2020 2020 7479 7065 3d63  nly",.    type=c
-000102f0: 6c69 636b 2e49 4e54 2c0a 2020 2020 6d75  lick.INT,.    mu
-00010300: 6c74 6970 6c65 3d54 7275 652c 0a20 2020  ltiple=True,.   
-00010310: 2068 656c 703d 2250 6c61 7920 6f6e 6c79   help="Play only
-00010320: 2074 6869 732f 7468 6573 6520 736f 6e67   this/these song
-00010330: 2873 2920 2863 616e 2062 6520 7061 7373  (s) (can be pass
-00010340: 6564 206d 756c 7469 706c 6520 7469 6d65  ed multiple time
-00010350: 732c 2065 2e67 2e20 276d 6165 7374 726f  s, e.g. 'maestro
-00010360: 2070 6c61 7920 2d6f 2031 202d 6f20 3137   play -o 1 -o 17
-00010370: 2729 2e22 2c0a 290a 4063 6c69 636b 2e6f  ').",.).@click.o
-00010380: 7074 696f 6e28 0a20 2020 2022 2d76 222c  ption(.    "-v",
-00010390: 0a20 2020 2022 2d2d 766f 6c75 6d65 222c  .    "--volume",
-000103a0: 0a20 2020 2022 766f 6c75 6d65 222c 0a20  .    "volume",. 
-000103b0: 2020 2074 7970 653d 636c 6963 6b2e 496e     type=click.In
-000103c0: 7452 616e 6765 2830 2c20 3130 3029 2c0a  tRange(0, 100),.
-000103d0: 2020 2020 6465 6661 756c 743d 3130 302c      default=100,
-000103e0: 0a20 2020 2073 686f 775f 6465 6661 756c  .    show_defaul
-000103f0: 743d 5472 7565 2c0a 290a 4063 6c69 636b  t=True,.).@click
-00010400: 2e6f 7074 696f 6e28 0a20 2020 2022 2d4c  .option(.    "-L
-00010410: 2f2d 6e4c 222c 0a20 2020 2022 2d2d 6c6f  /-nL",.    "--lo
-00010420: 6f70 2f2d 2d6e 6f2d 6c6f 6f70 222c 0a20  op/--no-loop",. 
-00010430: 2020 2022 6c6f 6f70 222c 0a20 2020 2064     "loop",.    d
-00010440: 6566 6175 6c74 3d46 616c 7365 2c0a 2020  efault=False,.  
-00010450: 2020 6865 6c70 3d22 4c6f 6f70 2074 6865    help="Loop the
-00010460: 2070 6c61 796c 6973 742e 2043 616e 2062   playlist. Can b
-00010470: 6520 746f 6767 6c65 6420 7769 7468 2027  e toggled with '
-00010480: 6c27 2e22 2c0a 290a 4063 6c69 636b 2e6f  l'.",.).@click.o
-00010490: 7074 696f 6e28 0a20 2020 2022 2d43 2f2d  ption(.    "-C/-
-000104a0: 6e43 222c 0a20 2020 2022 2d2d 636c 6970  nC",.    "--clip
-000104b0: 732f 2d2d 6e6f 2d63 6c69 7073 222c 0a20  s/--no-clips",. 
-000104c0: 2020 2022 636c 6970 7322 2c0a 2020 2020     "clips",.    
-000104d0: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
-000104e0: 2020 2068 656c 703d 2253 7461 7274 2069     help="Start i
-000104f0: 6e20 636c 6970 206d 6f64 652e 2043 616e  n clip mode. Can
-00010500: 2062 6520 746f 6767 6c65 6420 7769 7468   be toggled with
-00010510: 2027 6327 2e22 2c0a 290a 4063 6c69 636b   'c'.",.).@click
-00010520: 2e6f 7074 696f 6e28 0a20 2020 2022 2d44  .option(.    "-D
-00010530: 2f2d 6e44 222c 0a20 2020 2022 2d2d 6469  /-nD",.    "--di
-00010540: 7363 6f72 642f 2d2d 6e6f 2d64 6973 636f  scord/--no-disco
-00010550: 7264 222c 0a20 2020 2022 6469 7363 6f72  rd",.    "discor
-00010560: 6422 2c0a 2020 2020 6465 6661 756c 743d  d",.    default=
-00010570: 4661 6c73 652c 0a20 2020 2068 656c 703d  False,.    help=
-00010580: 2244 6973 636f 7264 2072 6963 6820 7072  "Discord rich pr
-00010590: 6573 656e 6365 2e20 4967 6e6f 7265 6420  esence. Ignored 
-000105a0: 6966 2072 6571 7569 7265 6420 6465 7065  if required depe
-000105b0: 6e64 656e 6369 6573 2061 7265 206e 6f74  ndencies are not
-000105c0: 2069 6e73 7461 6c6c 6564 2e20 5769 6c6c   installed. Will
-000105d0: 2066 6169 6c20 7369 6c65 6e74 6c79 2061   fail silently a
-000105e0: 6e64 2072 6574 7279 2065 7665 7279 2074  nd retry every t
-000105f0: 696d 6520 7468 6520 736f 6e67 2063 6861  ime the song cha
-00010600: 6e67 6573 2069 6620 4469 7363 6f72 6420  nges if Discord 
-00010610: 636f 6e6e 6563 7469 6f6e 2066 6169 6c73  connection fails
-00010620: 2028 652e 672e 2044 6973 636f 7264 206e   (e.g. Discord n
-00010630: 6f74 206f 7065 6e29 2e22 2c0a 290a 4063  ot open).",.).@c
-00010640: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
-00010650: 2022 2d4d 2f2d 6e4d 222c 0a20 2020 2022   "-M/-nM",.    "
-00010660: 2d2d 6d61 7463 682d 616c 6c2f 2d2d 6e6f  --match-all/--no
-00010670: 2d6d 6174 6368 2d61 6c6c 222c 0a20 2020  -match-all",.   
-00010680: 2022 6d61 7463 685f 616c 6c22 2c0a 2020   "match_all",.  
-00010690: 2020 6465 6661 756c 743d 4661 6c73 652c    default=False,
-000106a0: 0a20 2020 2068 656c 703d 2250 6c61 7920  .    help="Play 
-000106b0: 736f 6e67 7320 7468 6174 206d 6174 6368  songs that match
-000106c0: 2061 6c6c 2074 6167 732c 206e 6f74 2061   all tags, not a
-000106d0: 6e79 2e22 2c0a 290a 4063 6c69 636b 2e6f  ny.",.).@click.o
-000106e0: 7074 696f 6e28 0a20 2020 2022 2d56 2f2d  ption(.    "-V/-
-000106f0: 6e56 222c 0a20 2020 2022 2d2d 7669 7375  nV",.    "--visu
-00010700: 616c 697a 652f 2d2d 6e6f 2d76 6973 7561  alize/--no-visua
-00010710: 6c69 7a65 222c 0a20 2020 2022 7669 7375  lize",.    "visu
-00010720: 616c 697a 6522 2c0a 2020 2020 6465 6661  alize",.    defa
-00010730: 756c 743d 4661 6c73 652c 0a20 2020 2068  ult=False,.    h
-00010740: 656c 703d 2256 6973 7561 6c69 7a65 2074  elp="Visualize t
-00010750: 6865 2073 6f6e 6720 6265 696e 6720 706c  he song being pl
-00010760: 6179 6564 2e20 4967 6e6f 7265 6420 6966  ayed. Ignored if
-00010770: 2072 6571 7569 7265 6420 6465 7065 6e64   required depend
-00010780: 656e 6369 6573 2061 7265 206e 6f74 2069  encies are not i
-00010790: 6e73 7461 6c6c 6564 2e22 2c0a 290a 6465  nstalled.",.).de
-000107a0: 6620 706c 6179 280a 2020 2020 7461 6773  f play(.    tags
-000107b0: 2c0a 2020 2020 7368 7566 666c 655f 2c0a  ,.    shuffle_,.
-000107c0: 2020 2020 7265 7665 7273 652c 0a20 2020      reverse,.   
-000107d0: 206f 6e6c 792c 0a20 2020 2076 6f6c 756d   only,.    volum
-000107e0: 652c 0a20 2020 206c 6f6f 702c 0a20 2020  e,.    loop,.   
-000107f0: 2063 6c69 7073 2c0a 2020 2020 6469 7363   clips,.    disc
-00010800: 6f72 642c 0a20 2020 206d 6174 6368 5f61  ord,.    match_a
-00010810: 6c6c 2c0a 2020 2020 7669 7375 616c 697a  ll,.    visualiz
-00010820: 652c 0a29 3a0a 2020 2020 2222 2250 6c61  e,.):.    """Pla
-00010830: 7920 796f 7572 2073 6f6e 6773 2e20 4966  y your songs. If
-00010840: 2074 6167 7320 6172 6520 7061 7373 6564   tags are passed
-00010850: 2c20 616e 7920 736f 6e67 206d 6174 6368  , any song match
-00010860: 696e 6720 616e 7920 7461 6720 7769 6c6c  ing any tag will
-00010870: 2062 6520 696e 0a20 2020 2079 6f75 7220   be in.    your 
-00010880: 706c 6179 6c69 7374 2c20 756e 6c65 7373  playlist, unless
-00010890: 2074 6865 2027 2d4d 2f2d 2d6d 6174 6368   the '-M/--match
-000108a0: 2d61 6c6c 2720 666c 6167 2069 7320 7061  -all' flag is pa
-000108b0: 7373 6564 2c20 696e 2077 6869 6368 2063  ssed, in which c
-000108c0: 6173 650a 2020 2020 6576 6572 7920 7461  ase.    every ta
-000108d0: 6720 6d75 7374 2062 6520 6d61 7463 6865  g must be matche
-000108e0: 642e 0a0a 2020 2020 5c62 0a20 2020 205c  d...    \b.    \
-000108f0: 7831 625b 316d 5350 4143 455c 7831 625b  x1b[1mSPACE\x1b[
-00010900: 306d 2020 746f 2070 6175 7365 2f70 6c61  0m  to pause/pla
-00010910: 790a 2020 2020 5c78 3162 5b31 6d62 2f70  y.    \x1b[1mb/p
-00010920: 5c78 3162 5b30 6d20 2074 6f20 676f 205b  \x1b[0m  to go [
-00010930: 625d 6163 6b20 746f 205b 705d 7265 7669  b]ack to [p]revi
-00010940: 6f75 7320 736f 6e67 0a20 2020 205c 7831  ous song.    \x1
-00010950: 625b 316d 725c 7831 625b 306d 2020 746f  b[1mr\x1b[0m  to
-00010960: 205b 725d 6570 6c61 7920 736f 6e67 0a20   [r]eplay song. 
-00010970: 2020 205c 7831 625b 316d 732f 6e5c 7831     \x1b[1ms/n\x1
-00010980: 625b 306d 2020 746f 205b 735d 6b69 7020  b[0m  to [s]kip 
-00010990: 746f 205b 6e5d 6578 7420 736f 6e67 0a20  to [n]ext song. 
-000109a0: 2020 205c 7831 625b 316d 6c5c 7831 625b     \x1b[1ml\x1b[
-000109b0: 306d 2020 746f 205b 6c5d 6f6f 7020 7468  0m  to [l]oop th
-000109c0: 6520 6375 7272 656e 7420 736f 6e67 0a20  e current song. 
-000109d0: 2020 205c 7831 625b 316d 635c 7831 625b     \x1b[1mc\x1b[
-000109e0: 306d 2020 746f 2074 6f67 676c 6520 5b63  0m  to toggle [c
-000109f0: 5d6c 6970 206d 6f64 650a 2020 2020 5c78  ]lip mode.    \x
-00010a00: 3162 5b31 6d76 5c78 3162 5b30 6d20 2074  1b[1mv\x1b[0m  t
-00010a10: 6f20 746f 6767 6c65 205b 765d 6973 7561  o toggle [v]isua
-00010a20: 6c69 7a61 7469 6f6e 0a20 2020 205c 7831  lization.    \x1
-00010a30: 625b 316d 4c45 4654 5c78 3162 5b30 6d20  b[1mLEFT\x1b[0m 
-00010a40: 2074 6f20 7265 7769 6e64 2035 730a 2020   to rewind 5s.  
-00010a50: 2020 5c78 3162 5b31 6d52 4947 4854 5c78    \x1b[1mRIGHT\x
-00010a60: 3162 5b30 6d20 2074 6f20 6661 7374 2066  1b[0m  to fast f
-00010a70: 6f72 7761 7264 2035 730a 2020 2020 5c78  orward 5s.    \x
-00010a80: 3162 5b31 6d5b 5c78 3162 5b30 6d20 2074  1b[1m[\x1b[0m  t
-00010a90: 6f20 6465 6372 6561 7365 2076 6f6c 756d  o decrease volum
-00010aa0: 650a 2020 2020 5c78 3162 5b31 6d5d 5c78  e.    \x1b[1m]\x
-00010ab0: 3162 5b30 6d20 2074 6f20 696e 6372 6561  1b[0m  to increa
-00010ac0: 7365 2076 6f6c 756d 650a 2020 2020 5c78  se volume.    \x
-00010ad0: 3162 5b31 6d6d 5c78 3162 5b30 6d20 2074  1b[1mm\x1b[0m  t
-00010ae0: 6f20 5b6d 5d75 7465 2f75 6e6d 7574 650a  o [m]ute/unmute.
-00010af0: 2020 2020 5c78 3162 5b31 6d65 5c78 3162      \x1b[1me\x1b
-00010b00: 5b30 6d20 2074 6f20 5b65 5d6e 6420 7468  [0m  to [e]nd th
-00010b10: 6520 736f 6e67 2070 6c61 7965 7220 6166  e song player af
-00010b20: 7465 7220 7468 6520 6375 7272 656e 7420  ter the current 
-00010b30: 736f 6e67 2028 696e 6469 6361 746f 7220  song (indicator 
-00010b40: 696e 2073 7461 7475 7320 6261 722c 2027  in status bar, '
-00010b50: 6527 2074 6f20 6361 6e63 656c 290a 2020  e' to cancel).  
-00010b60: 2020 5c78 3162 5b31 6d71 5c78 3162 5b30    \x1b[1mq\x1b[0
-00010b70: 6d20 2074 6f20 5b71 5d75 6974 2074 6865  m  to [q]uit the
-00010b80: 2073 6f6e 6720 706c 6179 6572 2069 6d6d   song player imm
-00010b90: 6564 6961 7465 6c79 0a20 2020 205c 7831  ediately.    \x1
-00010ba0: 625b 316d 5550 2f44 4f57 4e5c 7831 625b  b[1mUP/DOWN\x1b[
-00010bb0: 306d 2020 746f 2073 6372 6f6c 6c20 7468  0m  to scroll th
-00010bc0: 726f 7567 6820 7468 6520 706c 6179 6c69  rough the playli
-00010bd0: 7374 2028 6d6f 7573 6520 7363 726f 6c6c  st (mouse scroll
-00010be0: 696e 6720 7368 6f75 6c64 2061 6c73 6f20  ing should also 
-00010bf0: 776f 726b 290a 2020 2020 5c78 3162 5b31  work).    \x1b[1
-00010c00: 6d42 4143 4b53 5041 4345 2f44 454c 4554  mBACKSPACE/DELET
-00010c10: 455c 7831 625b 306d 2020 6465 6c65 7465  E\x1b[0m  delete
-00010c20: 2074 6865 2073 656c 6563 7465 6420 286e   the selected (n
-00010c30: 6f74 206e 6563 6573 7361 7269 6c79 2063  ot necessarily c
-00010c40: 7572 7265 6e74 6c79 2070 6c61 7969 6e67  urrently playing
-00010c50: 2129 2073 6f6e 6720 6672 6f6d 2074 6865  !) song from the
-00010c60: 2071 7565 7565 0a20 2020 205c 7831 625b   queue.    \x1b[
-00010c70: 316d 645c 7831 625b 306d 2020 746f 2074  1md\x1b[0m  to t
-00010c80: 6f67 676c 6520 5b44 5d69 7363 6f72 6420  oggle [D]iscord 
-00010c90: 7269 6368 2070 7265 7365 6e63 650a 2020  rich presence.  
-00010ca0: 2020 5c78 3162 5b31 6d61 5c78 3162 5b30    \x1b[1ma\x1b[0
-00010cb0: 6d20 2074 6f20 6164 6420 6120 736f 6e67  m  to add a song
-00010cc0: 2028 6279 2049 4429 2074 6f20 7468 6520   (by ID) to the 
-00010cd0: 656e 6420 6f66 2074 6865 2070 6c61 796c  end of the playl
-00010ce0: 6973 742e 204f 7065 6e73 2061 2070 726f  ist. Opens a pro
-00010cf0: 6d70 7420 746f 2065 6e74 6572 2074 6865  mpt to enter the
-00010d00: 2049 443a 2045 4e54 4552 2074 6f20 636f   ID: ENTER to co
-00010d10: 6e66 6972 6d2c 2045 5343 2074 6f20 6361  nfirm, ESC to ca
-00010d20: 6e63 656c 2e0a 2020 2020 5c78 3162 5b31  ncel..    \x1b[1
-00010d30: 6d69 5c78 3162 5b30 6d20 2074 6f20 696e  mi\x1b[0m  to in
-00010d40: 7365 7274 2061 2073 6f6e 6720 2862 7920  sert a song (by 
-00010d50: 4944 2920 696e 2074 6865 2070 6c61 796c  ID) in the playl
-00010d60: 6973 7420 6166 7465 7220 7468 6520 6375  ist after the cu
-00010d70: 7272 656e 7420 736f 6e67 2e20 4f70 656e  rrent song. Open
-00010d80: 7320 6120 7072 6f6d 7074 206c 696b 6520  s a prompt like 
-00010d90: 2761 272e 0a0a 2020 2020 5c62 0a20 2020  'a'...    \b.   
-00010da0: 2073 6f6e 6720 636f 6c6f 7220 696e 6469   song color indi
-00010db0: 6361 7465 7320 6d6f 6465 3a0a 2020 2020  cates mode:.    
-00010dc0: 2020 2020 5c78 3162 5b31 3b33 346d 626c      \x1b[1;34mbl
-00010dd0: 7565 5c78 3162 5b30 6d20 2020 2020 6e6f  ue\x1b[0m     no
-00010de0: 726d 616c 0a20 2020 2020 2020 205c 7831  rmal.        \x1
-00010df0: 625b 313b 3333 6d79 656c 6c6f 775c 7831  b[1;33myellow\x1
-00010e00: 625b 306d 2020 206c 6f6f 7069 6e67 2063  b[0m   looping c
-00010e10: 7572 7265 6e74 2073 6f6e 670a 0a20 2020  urrent song..   
-00010e20: 205c 620a 2020 2020 7072 6f67 7265 7373   \b.    progress
-00010e30: 2062 6172 2063 6f6c 6f72 2069 6e64 6963   bar color indic
-00010e40: 6174 6573 2073 7461 7475 733a 0a20 2020  ates status:.   
-00010e50: 2020 2020 205c 7831 625b 313b 3333 6d79       \x1b[1;33my
-00010e60: 656c 6c6f 775c 7831 625b 306d 2020 206e  ellow\x1b[0m   n
-00010e70: 6f72 6d61 6c20 286f 7220 6375 7272 656e  ormal (or curren
-00010e80: 7420 736f 6e67 2064 6f65 736e 2774 2068  t song doesn't h
-00010e90: 6176 6520 6120 636c 6970 290a 2020 2020  ave a clip).    
-00010ea0: 2020 2020 5c78 3162 5b31 3b33 356d 6d61      \x1b[1;35mma
-00010eb0: 6765 6e74 615c 7831 625b 306d 2020 706c  genta\x1b[0m  pl
-00010ec0: 6179 696e 6720 636c 6970 0a0a 2020 2020  aying clip..    
-00010ed0: 466f 7220 7468 6520 636f 6c6f 7220 7669  For the color vi
-00010ee0: 7369 6f6e 2064 6566 6963 6965 6e74 2c20  sion deficient, 
-00010ef0: 626f 7468 206d 6f64 6573 2061 6c73 6f20  both modes also 
-00010f00: 6861 7665 2069 6e64 6963 6174 6f72 7320  have indicators 
-00010f10: 696e 2074 6865 2073 7461 7475 7320 6261  in the status ba
-00010f20: 722e 0a20 2020 2022 2222 0a20 2020 2070  r..    """.    p
-00010f30: 6c61 796c 6973 7420 3d20 5b5d 0a0a 2020  laylist = []..  
-00010f40: 2020 6966 206f 6e6c 793a 0a20 2020 2020    if only:.     
-00010f50: 2020 206f 6e6c 7920 3d20 7365 7428 6f6e     only = set(on
-00010f60: 6c79 290a 2020 2020 2020 2020 7769 7468  ly).        with
-00010f70: 206f 7065 6e28 534f 4e47 535f 494e 464f   open(SONGS_INFO
-00010f80: 5f50 4154 482c 2022 7222 2c20 656e 636f  _PATH, "r", enco
-00010f90: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
-00010fa0: 2073 6f6e 6773 5f66 696c 653a 0a20 2020   songs_file:.   
-00010fb0: 2020 2020 2020 2020 2066 6f72 206c 696e           for lin
-00010fc0: 6520 696e 2073 6f6e 6773 5f66 696c 653a  e in songs_file:
-00010fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010fe0: 2064 6574 6169 6c73 203d 206c 696e 652e   details = line.
-00010ff0: 7374 7269 7028 292e 7370 6c69 7428 227c  strip().split("|
-00011000: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00011010: 2020 2073 6f6e 675f 6964 203d 2069 6e74     song_id = int
-00011020: 2864 6574 6169 6c73 5b30 5d29 0a20 2020  (details[0]).   
-00011030: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00011040: 736f 6e67 5f69 6420 696e 206f 6e6c 793a  song_id in only:
-00011050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011060: 2020 2020 2070 6c61 796c 6973 742e 6170       playlist.ap
-00011070: 7065 6e64 2864 6574 6169 6c73 290a 0a20  pend(details).. 
-00011080: 2020 2020 2020 2069 6620 6e6f 7420 706c         if not pl
-00011090: 6179 6c69 7374 3a0a 2020 2020 2020 2020  aylist:.        
-000110a0: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-000110b0: 224e 6f20 736f 6e67 7320 666f 756e 6420  "No songs found 
-000110c0: 7769 7468 2074 6865 2067 6976 656e 2049  with the given I
-000110d0: 4473 2e22 2c20 6667 3d22 7265 6422 290a  Ds.", fg="red").
-000110e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000110f0: 726e 0a20 2020 2065 6c73 653a 0a20 2020  rn.    else:.   
-00011100: 2020 2020 2069 6620 6e6f 7420 7461 6773       if not tags
-00011110: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
-00011120: 7468 206f 7065 6e28 534f 4e47 535f 494e  th open(SONGS_IN
-00011130: 464f 5f50 4154 482c 2022 7222 2c20 656e  FO_PATH, "r", en
-00011140: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-00011150: 6173 2073 6f6e 6773 5f66 696c 653a 0a20  as songs_file:. 
-00011160: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00011170: 6f72 206c 696e 6520 696e 2073 6f6e 6773  or line in songs
-00011180: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
-00011190: 2020 2020 2020 2020 2020 2064 6574 6169             detai
-000111a0: 6c73 203d 206c 696e 652e 7374 7269 7028  ls = line.strip(
-000111b0: 292e 7370 6c69 7428 227c 2229 0a20 2020  ).split("|").   
-000111c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000111d0: 2070 6c61 796c 6973 742e 6170 7065 6e64   playlist.append
-000111e0: 2864 6574 6169 6c73 290a 2020 2020 2020  (details).      
-000111f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00011200: 2020 2020 7461 6773 203d 2073 6574 2874      tags = set(t
-00011210: 6167 7329 0a20 2020 2020 2020 2020 2020  ags).           
-00011220: 2070 6c61 796c 6973 7420 3d20 5b5d 0a20   playlist = []. 
-00011230: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00011240: 6f70 656e 2853 4f4e 4753 5f49 4e46 4f5f  open(SONGS_INFO_
-00011250: 5041 5448 2c20 2272 222c 2065 6e63 6f64  PATH, "r", encod
-00011260: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
-00011270: 736f 6e67 735f 6669 6c65 3a0a 2020 2020  songs_file:.    
-00011280: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00011290: 6c69 6e65 2069 6e20 736f 6e67 735f 6669  line in songs_fi
-000112a0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
-000112b0: 2020 2020 2020 2020 6465 7461 696c 7320          details 
-000112c0: 3d20 6c69 6e65 2e73 7472 6970 2829 2e73  = line.strip().s
-000112d0: 706c 6974 2822 7c22 290a 2020 2020 2020  plit("|").      
-000112e0: 2020 2020 2020 2020 2020 2020 2020 736f                so
-000112f0: 6e67 5f74 6167 7320 3d20 7365 7428 6465  ng_tags = set(de
-00011300: 7461 696c 735b 325d 2e73 706c 6974 2822  tails[2].split("
-00011310: 2c22 2929 0a20 2020 2020 2020 2020 2020  ,")).           
-00011320: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00011330: 6d61 7463 685f 616c 6c3a 0a20 2020 2020  match_all:.     
-00011340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011350: 2020 2069 6620 7461 6773 2026 2073 6f6e     if tags & son
-00011360: 675f 7461 6773 3a20 2023 2069 6e74 6572  g_tags:  # inter
-00011370: 7365 6374 696f 6e0a 2020 2020 2020 2020  section.        
-00011380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011390: 2020 2020 706c 6179 6c69 7374 2e61 7070      playlist.app
-000113a0: 656e 6428 6465 7461 696c 7329 0a20 2020  end(details).   
-000113b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113c0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000113d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000113e0: 6620 7461 6773 203c 3d20 736f 6e67 5f74  f tags <= song_t
-000113f0: 6167 733a 2020 2320 7375 6273 6574 0a20  ags:  # subset. 
-00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011410: 2020 2020 2020 2020 2020 2070 6c61 796c             playl
-00011420: 6973 742e 6170 7065 6e64 2864 6574 6169  ist.append(detai
-00011430: 6c73 290a 0a20 2020 2066 6f72 2064 6574  ls)..    for det
-00011440: 6169 6c73 2069 6e20 706c 6179 6c69 7374  ails in playlist
-00011450: 3a0a 2020 2020 2020 2020 736f 6e67 5f64  :.        song_d
-00011460: 6174 6120 3d20 6d75 7369 635f 7461 672e  ata = music_tag.
-00011470: 6c6f 6164 5f66 696c 6528 6f73 2e70 6174  load_file(os.pat
-00011480: 682e 6a6f 696e 2853 4f4e 4753 5f44 4952  h.join(SONGS_DIR
-00011490: 2c20 6465 7461 696c 735b 315d 2929 0a20  , details[1])). 
-000114a0: 2020 2020 2020 2064 6574 6169 6c73 202b         details +
-000114b0: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-000114c0: 2873 6f6e 675f 6461 7461 5b22 6172 7469  (song_data["arti
-000114d0: 7374 225d 2e76 616c 7565 206f 7220 2255  st"].value or "U
-000114e0: 6e6b 6e6f 776e 2041 7274 6973 7422 292c  nknown Artist"),
-000114f0: 0a20 2020 2020 2020 2020 2020 2028 736f  .            (so
-00011500: 6e67 5f64 6174 615b 2261 6c62 756d 225d  ng_data["album"]
-00011510: 2e76 616c 7565 206f 7220 2255 6e6b 6e6f  .value or "Unkno
-00011520: 776e 2041 6c62 756d 2229 2c0a 2020 2020  wn Album"),.    
-00011530: 2020 2020 2020 2020 2873 6f6e 675f 6461          (song_da
-00011540: 7461 5b22 616c 6275 6d61 7274 6973 7422  ta["albumartist"
-00011550: 5d2e 7661 6c75 6520 6f72 2022 556e 6b6e  ].value or "Unkn
-00011560: 6f77 6e20 416c 6275 6d20 4172 7469 7374  own Album Artist
-00011570: 2229 2c0a 2020 2020 2020 2020 5d0a 0a20  "),.        ].. 
-00011580: 2020 2069 6620 7368 7566 666c 655f 203d     if shuffle_ =
-00011590: 3d20 303a 0a20 2020 2020 2020 2073 6875  = 0:.        shu
-000115a0: 6666 6c65 5f20 3d20 5472 7565 0a20 2020  ffle_ = True.   
-000115b0: 2020 2020 2072 6573 6875 6666 6c65 203d       reshuffle =
-000115c0: 2046 616c 7365 0a20 2020 2065 6c69 6620   False.    elif 
-000115d0: 7368 7566 666c 655f 203d 3d20 313a 0a20  shuffle_ == 1:. 
-000115e0: 2020 2020 2020 2073 6875 6666 6c65 5f20         shuffle_ 
-000115f0: 3d20 5472 7565 0a20 2020 2020 2020 2072  = True.        r
-00011600: 6573 6875 6666 6c65 203d 2054 7275 650a  eshuffle = True.
-00011610: 2020 2020 656c 6966 2073 6875 6666 6c65      elif shuffle
-00011620: 5f20 3d3d 2032 3a0a 2020 2020 2020 2020  _ == 2:.        
-00011630: 7368 7566 666c 655f 203d 2046 616c 7365  shuffle_ = False
-00011640: 0a20 2020 2020 2020 2072 6573 6875 6666  .        reshuff
-00011650: 6c65 203d 2054 7275 650a 2020 2020 656c  le = True.    el
-00011660: 7365 3a20 2023 2073 6875 6666 6c65 5f20  se:  # shuffle_ 
-00011670: 3d20 4e6f 6e65 0a20 2020 2020 2020 2073  = None.        s
-00011680: 6875 6666 6c65 5f20 3d20 4661 6c73 650a  huffle_ = False.
-00011690: 2020 2020 2020 2020 7265 7368 7566 666c          reshuffl
-000116a0: 6520 3d20 4661 6c73 650a 0a20 2020 2069  e = False..    i
-000116b0: 6620 7368 7566 666c 655f 3a0a 2020 2020  f shuffle_:.    
-000116c0: 2020 2020 7368 7566 666c 6528 706c 6179      shuffle(play
-000116d0: 6c69 7374 290a 2020 2020 656c 6966 2072  list).    elif r
-000116e0: 6576 6572 7365 3a0a 2020 2020 2020 2020  everse:.        
-000116f0: 706c 6179 6c69 7374 2e72 6576 6572 7365  playlist.reverse
-00011700: 2829 0a0a 2020 2020 6966 206e 6f74 2070  ()..    if not p
-00011710: 6c61 796c 6973 743a 0a20 2020 2020 2020  laylist:.       
-00011720: 2063 6c69 636b 2e73 6563 686f 2822 4e6f   click.secho("No
-00011730: 2073 6f6e 6773 2066 6f75 6e64 206d 6174   songs found mat
-00011740: 6368 696e 6720 7461 6720 6372 6974 6572  ching tag criter
-00011750: 6961 2e22 2c20 6667 3d22 7265 6422 290a  ia.", fg="red").
-00011760: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00011770: 2020 766f 6c75 6d65 202f 3d20 3130 300a    volume /= 100.
-00011780: 2020 2020 2020 2020 6375 7273 6573 2e77          curses.w
-00011790: 7261 7070 6572 280a 2020 2020 2020 2020  rapper(.        
-000117a0: 2020 2020 5f70 6c61 792c 0a20 2020 2020      _play,.     
-000117b0: 2020 2020 2020 2070 6c61 796c 6973 742c         playlist,
-000117c0: 0a20 2020 2020 2020 2020 2020 2076 6f6c  .            vol
-000117d0: 756d 652c 0a20 2020 2020 2020 2020 2020  ume,.           
-000117e0: 206c 6f6f 702c 0a20 2020 2020 2020 2020   loop,.         
-000117f0: 2020 2063 6c69 7073 2c0a 2020 2020 2020     clips,.      
-00011800: 2020 2020 2020 7265 7368 7566 666c 652c        reshuffle,
-00011810: 0a20 2020 2020 2020 2020 2020 2064 6973  .            dis
-00011820: 636f 7264 2061 6e64 2063 616e 5f75 7064  cord and can_upd
-00011830: 6174 655f 6469 7363 6f72 642c 0a20 2020  ate_discord,.   
-00011840: 2020 2020 2020 2020 2076 6973 7561 6c69           visuali
-00011850: 7a65 2c0a 2020 2020 2020 2020 290a 0a0a  ze,.        )...
-00011860: 4063 6c69 2e63 6f6d 6d61 6e64 2829 0a40  @cli.command().@
-00011870: 636c 6963 6b2e 6f70 7469 6f6e 280a 2020  click.option(.  
-00011880: 2020 222d 542f 2d6e 5422 2c0a 2020 2020    "-T/-nT",.    
-00011890: 222d 2d74 6167 2f2d 2d6e 6f2d 7461 6722  "--tag/--no-tag"
-000118a0: 2c0a 2020 2020 2272 656e 616d 696e 675f  ,.    "renaming_
-000118b0: 7461 6722 2c0a 2020 2020 6465 6661 756c  tag",.    defaul
-000118c0: 743d 4661 6c73 652c 0a20 2020 2068 656c  t=False,.    hel
-000118d0: 703d 2249 6620 7061 7373 6564 2c20 7265  p="If passed, re
-000118e0: 6e61 6d65 2074 6167 2069 6e73 7465 6164  name tag instead
-000118f0: 206f 6620 736f 6e67 2028 7472 6561 7420   of song (treat 
-00011900: 7468 6520 6172 6775 6d65 6e74 7320 6173  the arguments as
-00011910: 2074 6167 7329 2e22 2c0a 290a 4063 6c69   tags).",.).@cli
-00011920: 636b 2e61 7267 756d 656e 7428 226f 7269  ck.argument("ori
-00011930: 6769 6e61 6c22 290a 4063 6c69 636b 2e61  ginal").@click.a
-00011940: 7267 756d 656e 7428 226e 6577 5f6e 616d  rgument("new_nam
-00011950: 6522 290a 6465 6620 7265 6e61 6d65 286f  e").def rename(o
-00011960: 7269 6769 6e61 6c2c 206e 6577 5f6e 616d  riginal, new_nam
-00011970: 652c 2072 656e 616d 696e 675f 7461 6729  e, renaming_tag)
-00011980: 3a0a 2020 2020 2222 2252 656e 616d 6573  :.    """Renames
-00011990: 2074 6865 2073 6f6e 6720 7769 7468 2074   the song with t
-000119a0: 6865 2049 4420 4f52 4947 494e 414c 2074  he ID ORIGINAL t
-000119b0: 6f20 4e45 575f 4e41 4d45 2e20 5468 6520  o NEW_NAME. The 
-000119c0: 6578 7465 6e73 696f 6e20 6f66 2074 6865  extension of the
-000119d0: 0a20 2020 2073 6f6e 6720 2865 2e67 2e20  .    song (e.g. 
-000119e0: 272e 7761 7627 2c20 272e 6d70 3327 2920  '.wav', '.mp3') 
-000119f0: 6973 2070 7265 7365 7276 6564 e280 9464  is preserved...d
-00011a00: 6f20 6e6f 7420 696e 636c 7564 6520 6974  o not include it
-00011a10: 2069 6e20 7468 6520 6e61 6d65 2e0a 0a20   in the name... 
-00011a20: 2020 2049 6620 7468 6520 272d 542f 2d2d     If the '-T/--
-00011a30: 7461 6727 2066 6c61 6720 6973 2070 6173  tag' flag is pas
-00011a40: 7365 642c 2074 7265 6174 7320 4f52 4947  sed, treats ORIG
-00011a50: 494e 414c 2061 7320 6120 7461 672c 2072  INAL as a tag, r
-00011a60: 656e 616d 696e 6720 616c 6c0a 2020 2020  enaming all.    
-00011a70: 6f63 7572 7265 6e63 6573 206f 6620 6974  ocurrences of it
-00011a80: 2074 6f20 4e45 575f 4e41 4d45 e280 9464   to NEW_NAME...d
-00011a90: 6f65 736e 2774 2063 6865 636b 2069 6620  oesn't check if 
-00011aa0: 7468 6520 7461 6720 4e45 575f 4e41 4d45  the tag NEW_NAME
-00011ab0: 2061 6c72 6561 6479 2c0a 2020 2020 6578   already,.    ex
-00011ac0: 6973 7473 2c20 736f 2062 6520 6361 7265  ists, so be care
-00011ad0: 6675 6c21 0a20 2020 2022 2222 0a20 2020  ful!.    """.   
-00011ae0: 2073 6f6e 6773 5f66 696c 6520 3d20 6f70   songs_file = op
-00011af0: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
-00011b00: 5448 2c20 2272 222c 2065 6e63 6f64 696e  TH, "r", encodin
-00011b10: 673d 2275 7466 2d38 2229 0a20 2020 206c  g="utf-8").    l
-00011b20: 696e 6573 203d 2073 6f6e 6773 5f66 696c  ines = songs_fil
-00011b30: 652e 7265 6164 2829 2e73 706c 6974 6c69  e.read().splitli
-00011b40: 6e65 7328 290a 2020 2020 6966 206e 6f74  nes().    if not
-00011b50: 2072 656e 616d 696e 675f 7461 673a 0a20   renaming_tag:. 
-00011b60: 2020 2020 2020 2069 6620 6e6f 7420 6f72         if not or
-00011b70: 6967 696e 616c 2e69 736e 756d 6572 6963  iginal.isnumeric
-00011b80: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00011b90: 636c 6963 6b2e 7365 6368 6f28 0a20 2020  click.secho(.   
-00011ba0: 2020 2020 2020 2020 2020 2020 2022 536f               "So
-00011bb0: 6e67 2049 4420 6d75 7374 2062 6520 616e  ng ID must be an
-00011bc0: 2069 6e74 6567 6572 2e20 546f 2072 656e   integer. To ren
-00011bd0: 616d 6520 6120 7461 672c 2070 6173 7320  ame a tag, pass 
-00011be0: 7468 6520 272d 542f 2d2d 7461 6727 2066  the '-T/--tag' f
-00011bf0: 6c61 672e 222c 0a20 2020 2020 2020 2020  lag.",.         
-00011c00: 2020 2020 2020 2066 673d 2272 6564 222c         fg="red",
-00011c10: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00011c20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00011c30: 6e0a 0a20 2020 2020 2020 2066 6f72 2069  n..        for i
-00011c40: 2069 6e20 7261 6e67 6528 6c65 6e28 6c69   in range(len(li
-00011c50: 6e65 7329 293a 0a20 2020 2020 2020 2020  nes)):.         
-00011c60: 2020 2064 6574 6169 6c73 203d 206c 696e     details = lin
-00011c70: 6573 5b69 5d2e 7374 7269 7028 292e 7370  es[i].strip().sp
-00011c80: 6c69 7428 227c 2229 0a20 2020 2020 2020  lit("|").       
-00011c90: 2020 2020 2069 6620 6f73 2e70 6174 682e       if os.path.
-00011ca0: 7370 6c69 7465 7874 2864 6574 6169 6c73  splitext(details
-00011cb0: 5b31 5d29 5b30 5d20 3d3d 206e 6577 5f6e  [1])[0] == new_n
-00011cc0: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
-00011cd0: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
-00011ce0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00011cf0: 2020 2020 2020 6622 4120 736f 6e67 2077        f"A song w
-00011d00: 6974 6820 7468 6520 6e61 6d65 2027 7b6e  ith the name '{n
-00011d10: 6577 5f6e 616d 657d 2720 616c 7265 6164  ew_name}' alread
-00011d20: 7920 6578 6973 7473 2e20 506c 6561 7365  y exists. Please
-00011d30: 2063 686f 6f73 6520 616e 6f74 6865 7220   choose another 
-00011d40: 6e61 6d65 2e22 2c0a 2020 2020 2020 2020  name.",.        
-00011d50: 2020 2020 2020 2020 2020 2020 6667 3d22              fg="
-00011d60: 7265 6422 2c0a 2020 2020 2020 2020 2020  red",.          
-00011d70: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00011d80: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
-00011d90: 2020 2020 2020 2020 6f72 6967 696e 616c          original
-00011da0: 203d 2069 6e74 286f 7269 6769 6e61 6c29   = int(original)
-00011db0: 0a20 2020 2020 2020 2066 6f72 2069 2069  .        for i i
-00011dc0: 6e20 7261 6e67 6528 6c65 6e28 6c69 6e65  n range(len(line
-00011dd0: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
-00011de0: 2064 6574 6169 6c73 203d 206c 696e 6573   details = lines
-00011df0: 5b69 5d2e 7374 7269 7028 292e 7370 6c69  [i].strip().spli
-00011e00: 7428 227c 2229 0a20 2020 2020 2020 2020  t("|").         
-00011e10: 2020 2069 6620 696e 7428 6465 7461 696c     if int(detail
-00011e20: 735b 305d 2920 3d3d 206f 7269 6769 6e61  s[0]) == origina
-00011e30: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
-00011e40: 2020 206f 6c64 5f70 6174 6820 3d20 6465     old_path = de
-00011e50: 7461 696c 735b 315d 0a20 2020 2020 2020  tails[1].       
-00011e60: 2020 2020 2020 2020 2064 6574 6169 6c73           details
-00011e70: 5b31 5d20 3d20 6e65 775f 6e61 6d65 202b  [1] = new_name +
-00011e80: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
-00011e90: 7428 6f6c 645f 7061 7468 295b 315d 0a0a  t(old_path)[1]..
-00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011eb0: 6c69 6e65 735b 695d 203d 2022 7c22 2e6a  lines[i] = "|".j
-00011ec0: 6f69 6e28 6465 7461 696c 7329 0a20 2020  oin(details).   
-00011ed0: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
-00011ee0: 6773 5f66 696c 652e 636c 6f73 6528 290a  gs_file.close().
+0000e2e0: 2070 6c61 7965 725f 6f75 7470 7574 2e6c   player_output.l
+0000e2f0: 6f6f 7069 6e67 5f63 7572 7265 6e74 5f73  ooping_current_s
+0000e300: 6f6e 6720 3d20 4c4f 4f50 5f4d 4f44 4553  ong = LOOP_MODES
+0000e310: 5b22 6e6f 6e65 225d 0a20 2020 2020 2020  ["none"].       
+0000e320: 2020 2020 2020 2020 2070 7269 6e74 5f74           print_t
+0000e330: 6f5f 6c6f 6766 696c 6528 0a20 2020 2020  o_logfile(.     
+0000e340: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000e350: 6c61 7965 725f 6f75 7470 7574 2e6c 6f6f  layer_output.loo
+0000e360: 7069 6e67 5f63 7572 7265 6e74 5f73 6f6e  ping_current_son
+0000e370: 672c 204c 4f4f 505f 4d4f 4445 535b 226e  g, LOOP_MODES["n
+0000e380: 6f6e 6522 5d0a 2020 2020 2020 2020 2020  one"].          
+0000e390: 2020 2020 2020 290a 0a0a 2320 656e 6472        )...# endr
+0000e3a0: 6567 696f 6e0a 0a0a 4063 6c69 636b 2e67  egion...@click.g
+0000e3b0: 726f 7570 2863 6f6e 7465 7874 5f73 6574  roup(context_set
+0000e3c0: 7469 6e67 733d 6469 6374 2868 656c 705f  tings=dict(help_
+0000e3d0: 6f70 7469 6f6e 5f6e 616d 6573 3d5b 222d  option_names=["-
+0000e3e0: 6822 2c20 222d 2d68 656c 7022 5d29 290a  h", "--help"])).
+0000e3f0: 6465 6620 636c 6928 293a 0a20 2020 2022  def cli():.    "
+0000e400: 2222 4120 636f 6d6d 616e 6420 6c69 6e65  ""A command line
+0000e410: 2069 6e74 6572 6661 6365 2066 6f72 2070   interface for p
+0000e420: 6c61 7969 6e67 206d 7573 6963 2e22 2222  laying music."""
+0000e430: 0a20 2020 2069 6620 6e6f 7420 6f73 2e70  .    if not os.p
+0000e440: 6174 682e 6578 6973 7473 2853 4f4e 4753  ath.exists(SONGS
+0000e450: 5f44 4952 293a 0a20 2020 2020 2020 206f  _DIR):.        o
+0000e460: 732e 6d61 6b65 6469 7273 2853 4f4e 4753  s.makedirs(SONGS
+0000e470: 5f44 4952 290a 0a20 2020 2069 6620 6e6f  _DIR)..    if no
+0000e480: 7420 6f73 2e70 6174 682e 6578 6973 7473  t os.path.exists
+0000e490: 2853 4f4e 4753 5f49 4e46 4f5f 5041 5448  (SONGS_INFO_PATH
+0000e4a0: 293a 0a20 2020 2020 2020 2077 6974 6820  ):.        with 
+0000e4b0: 6f70 656e 2853 4f4e 4753 5f49 4e46 4f5f  open(SONGS_INFO_
+0000e4c0: 5041 5448 2c20 2278 222c 2065 6e63 6f64  PATH, "x", encod
+0000e4d0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+0000e4e0: 5f3a 0a20 2020 2020 2020 2020 2020 2070  _:.            p
+0000e4f0: 6173 730a 0a20 2020 2069 6620 6e6f 7420  ass..    if not 
+0000e500: 6f73 2e70 6174 682e 6578 6973 7473 2853  os.path.exists(S
+0000e510: 5441 5453 5f44 4952 293a 0a20 2020 2020  TATS_DIR):.     
+0000e520: 2020 206f 732e 6d61 6b65 6469 7273 2853     os.makedirs(S
+0000e530: 5441 5453 5f44 4952 290a 2020 2020 6966  TATS_DIR).    if
+0000e540: 206e 6f74 206f 732e 7061 7468 2e65 7869   not os.path.exi
+0000e550: 7374 7328 544f 5441 4c5f 5354 4154 535f  sts(TOTAL_STATS_
+0000e560: 5041 5448 293a 0a20 2020 2020 2020 2077  PATH):.        w
+0000e570: 6974 6820 280a 2020 2020 2020 2020 2020  ith (.          
+0000e580: 2020 6f70 656e 2854 4f54 414c 5f53 5441    open(TOTAL_STA
+0000e590: 5453 5f50 4154 482c 2022 7722 2c20 656e  TS_PATH, "w", en
+0000e5a0: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
+0000e5b0: 6173 2066 2c0a 2020 2020 2020 2020 2020  as f,.          
+0000e5c0: 2020 6f70 656e 2853 4f4e 4753 5f49 4e46    open(SONGS_INF
+0000e5d0: 4f5f 5041 5448 2c20 2272 222c 2065 6e63  O_PATH, "r", enc
+0000e5e0: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
+0000e5f0: 7320 672c 0a20 2020 2020 2020 2029 3a0a  s g,.        ):.
+0000e600: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000e610: 6c69 6e65 2069 6e20 673a 0a20 2020 2020  line in g:.     
+0000e620: 2020 2020 2020 2020 2020 2066 2e77 7269             f.wri
+0000e630: 7465 2866 227b 6c69 6e65 2e73 7472 6970  te(f"{line.strip
+0000e640: 2829 2e73 706c 6974 2827 7c27 295b 305d  ().split('|')[0]
+0000e650: 7d7c 305c 6e22 290a 2020 2020 6966 206e  }|0\n").    if n
+0000e660: 6f74 206f 732e 7061 7468 2e65 7869 7374  ot os.path.exist
+0000e670: 7328 4355 525f 5945 4152 5f53 5441 5453  s(CUR_YEAR_STATS
+0000e680: 5f50 4154 4829 3a0a 2020 2020 2020 2020  _PATH):.        
+0000e690: 7769 7468 2028 0a20 2020 2020 2020 2020  with (.         
+0000e6a0: 2020 206f 7065 6e28 4355 525f 5945 4152     open(CUR_YEAR
+0000e6b0: 5f53 5441 5453 5f50 4154 482c 2022 7722  _STATS_PATH, "w"
+0000e6c0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
+0000e6d0: 3822 2920 6173 2066 2c0a 2020 2020 2020  8") as f,.      
+0000e6e0: 2020 2020 2020 6f70 656e 2853 4f4e 4753        open(SONGS
+0000e6f0: 5f49 4e46 4f5f 5041 5448 2c20 2272 222c  _INFO_PATH, "r",
+0000e700: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+0000e710: 2229 2061 7320 672c 0a20 2020 2020 2020  ") as g,.       
+0000e720: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+0000e730: 666f 7220 6c69 6e65 2069 6e20 673a 0a20  for line in g:. 
+0000e740: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000e750: 2e77 7269 7465 2866 227b 6c69 6e65 2e73  .write(f"{line.s
+0000e760: 7472 6970 2829 2e73 706c 6974 2827 7c27  trip().split('|'
+0000e770: 295b 305d 7d7c 305c 6e22 290a 0a0a 4063  )[0]}|0\n")...@c
+0000e780: 6c69 2e63 6f6d 6d61 6e64 2829 0a40 636c  li.command().@cl
+0000e790: 6963 6b2e 6172 6775 6d65 6e74 2822 7061  ick.argument("pa
+0000e7a0: 7468 5f22 2c20 6d65 7461 7661 723d 2250  th_", metavar="P
+0000e7b0: 4154 485f 4f52 5f55 524c 2229 0a40 636c  ATH_OR_URL").@cl
+0000e7c0: 6963 6b2e 6172 6775 6d65 6e74 2822 7461  ick.argument("ta
+0000e7d0: 6773 222c 206e 6172 6773 3d2d 3129 0a40  gs", nargs=-1).@
+0000e7e0: 636c 6963 6b2e 6f70 7469 6f6e 280a 2020  click.option(.  
+0000e7f0: 2020 222d 4d2f 2d6e 4d22 2c0a 2020 2020    "-M/-nM",.    
+0000e800: 222d 2d6d 6f76 652f 2d2d 6e6f 2d6d 6f76  "--move/--no-mov
+0000e810: 6522 2c0a 2020 2020 226d 6f76 655f 222c  e",.    "move_",
+0000e820: 0a20 2020 2064 6566 6175 6c74 3d46 616c  .    default=Fal
+0000e830: 7365 2c0a 2020 2020 6865 6c70 3d22 4d6f  se,.    help="Mo
+0000e840: 7665 2066 696c 6520 6672 6f6d 2050 4154  ve file from PAT
+0000e850: 4820 746f 206d 6165 7374 726f 2773 2069  H to maestro's i
+0000e860: 6e74 6572 6e61 6c20 736f 6e67 2064 6174  nternal song dat
+0000e870: 6162 6173 6520 696e 7374 6561 6420 6f66  abase instead of
+0000e880: 2063 6f70 7969 6e67 2e22 2c0a 290a 4063   copying.",.).@c
+0000e890: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
+0000e8a0: 2022 2d6e 222c 0a20 2020 2022 2d2d 6e61   "-n",.    "--na
+0000e8b0: 6d65 222c 0a20 2020 2074 7970 653d 7374  me",.    type=st
+0000e8c0: 722c 0a20 2020 2068 656c 703d 2257 6861  r,.    help="Wha
+0000e8d0: 7420 746f 206e 616d 6520 7468 6520 736f  t to name the so
+0000e8e0: 6e67 2c20 6966 2079 6f75 2064 6f6e 2774  ng, if you don't
+0000e8f0: 2077 616e 7420 746f 2075 7365 2074 6865   want to use the
+0000e900: 2074 6974 6c65 2066 726f 6d20 596f 7574   title from Yout
+0000e910: 7562 652f 5370 6f74 6966 7920 6f72 2066  ube/Spotify or f
+0000e920: 696c 656e 616d 652e 2044 6f20 6e6f 7420  ilename. Do not 
+0000e930: 696e 636c 7564 6520 616e 2065 7874 656e  include an exten
+0000e940: 7369 6f6e 2028 652e 672e 2027 2e77 6176  sion (e.g. '.wav
+0000e950: 2729 2e20 4967 6e6f 7265 6420 6966 2061  '). Ignored if a
+0000e960: 6464 696e 6720 6d75 6c74 6970 6c65 2073  dding multiple s
+0000e970: 6f6e 6773 2e22 2c0a 290a 4063 6c69 636b  ongs.",.).@click
+0000e980: 2e6f 7074 696f 6e28 0a20 2020 2022 2d52  .option(.    "-R
+0000e990: 2c20 2d6e 5222 2c0a 2020 2020 222d 2d72  , -nR",.    "--r
+0000e9a0: 6563 7572 7369 7665 2f2d 2d6e 6f2d 7265  ecursive/--no-re
+0000e9b0: 6375 7273 6976 6522 2c0a 2020 2020 2272  cursive",.    "r
+0000e9c0: 6563 7572 7365 222c 0a20 2020 2064 6566  ecurse",.    def
+0000e9d0: 6175 6c74 3d46 616c 7365 2c0a 2020 2020  ault=False,.    
+0000e9e0: 6865 6c70 3d22 4966 2050 4154 4820 6973  help="If PATH is
+0000e9f0: 2061 2066 6f6c 6465 722c 2061 6464 2073   a folder, add s
+0000ea00: 6f6e 6773 2069 6e20 7375 6266 6f6c 6465  ongs in subfolde
+0000ea10: 7273 2e22 2c0a 290a 4063 6c69 636b 2e6f  rs.",.).@click.o
+0000ea20: 7074 696f 6e28 0a20 2020 2022 2d59 2f2d  ption(.    "-Y/-
+0000ea30: 6e59 222c 0a20 2020 2022 2d2d 796f 7574  nY",.    "--yout
+0000ea40: 7562 652f 2d2d 6e6f 2d79 6f75 7475 6265  ube/--no-youtube
+0000ea50: 222c 0a20 2020 2064 6566 6175 6c74 3d46  ",.    default=F
+0000ea60: 616c 7365 2c0a 2020 2020 6865 6c70 3d22  alse,.    help="
+0000ea70: 4164 6420 6120 736f 6e67 2066 726f 6d20  Add a song from 
+0000ea80: 6120 596f 7554 7562 6520 6f72 2059 6f75  a YouTube or You
+0000ea90: 5475 6265 204d 7573 6963 2055 524c 2e22  Tube Music URL."
+0000eaa0: 2c0a 290a 4063 6c69 636b 2e6f 7074 696f  ,.).@click.optio
+0000eab0: 6e28 0a20 2020 2022 2d53 2f2d 6e53 222c  n(.    "-S/-nS",
+0000eac0: 0a20 2020 2022 2d2d 7370 6f74 6966 792f  .    "--spotify/
+0000ead0: 2d2d 6e6f 2d73 706f 7469 6679 222c 0a20  --no-spotify",. 
+0000eae0: 2020 2064 6566 6175 6c74 3d46 616c 7365     default=False
+0000eaf0: 2c0a 2020 2020 6865 6c70 3d22 4164 6420  ,.    help="Add 
+0000eb00: 6120 736f 6e67 2066 726f 6d20 5370 6f74  a song from Spot
+0000eb10: 6966 7920 2874 7261 636b 2055 524c 2c20  ify (track URL, 
+0000eb20: 616c 6275 6d20 5552 4c2c 2070 6c61 796c  album URL, playl
+0000eb30: 6973 7420 5552 4c2c 2061 7274 6973 7420  ist URL, artist 
+0000eb40: 5552 4c2c 206f 7220 7365 6172 6368 2071  URL, or search q
+0000eb50: 7565 7279 292e 222c 0a29 0a40 636c 6963  uery).",.).@clic
+0000eb60: 6b2e 6f70 7469 6f6e 280a 2020 2020 222d  k.option(.    "-
+0000eb70: 6622 2c0a 2020 2020 222d 2d66 6f72 6d61  f",.    "--forma
+0000eb80: 7422 2c0a 2020 2020 2266 6f72 6d61 745f  t",.    "format_
+0000eb90: 222c 0a20 2020 2074 7970 653d 636c 6963  ",.    type=clic
+0000eba0: 6b2e 4368 6f69 6365 285b 2277 6176 222c  k.Choice(["wav",
+0000ebb0: 2022 6d70 3322 2c20 2266 6c61 6322 2c20   "mp3", "flac", 
+0000ebc0: 226f 6767 225d 292c 0a20 2020 2068 656c  "ogg"]),.    hel
+0000ebd0: 703d 2253 7065 6369 6679 2074 6865 2066  p="Specify the f
+0000ebe0: 6f72 6d61 7420 6f66 2074 6865 2073 6f6e  ormat of the son
+0000ebf0: 6720 6966 2064 6f77 6e6c 6f61 6469 6e67  g if downloading
+0000ec00: 2066 726f 6d20 596f 7554 7562 652c 2059   from YouTube, Y
+0000ec10: 6f75 5475 6265 204d 7573 6963 2c20 6f72  ouTube Music, or
+0000ec20: 2053 706f 7469 6679 2055 524c 2e22 2c0a   Spotify URL.",.
+0000ec30: 2020 2020 6465 6661 756c 743d 2266 6c61      default="fla
+0000ec40: 6322 2c0a 2020 2020 7368 6f77 5f64 6566  c",.    show_def
+0000ec50: 6175 6c74 3d54 7275 652c 0a29 0a40 636c  ault=True,.).@cl
+0000ec60: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
+0000ec70: 222d 6322 2c0a 2020 2020 222d 2d63 6c69  "-c",.    "--cli
+0000ec80: 7022 2c0a 2020 2020 6e61 7267 733d 322c  p",.    nargs=2,
+0000ec90: 0a20 2020 2074 7970 653d 666c 6f61 742c  .    type=float,
+0000eca0: 0a20 2020 2068 656c 703d 2241 6464 2061  .    help="Add a
+0000ecb0: 2063 6c69 702e 2049 676e 6f72 6564 2069   clip. Ignored i
+0000ecc0: 6620 6164 6469 6e67 206d 756c 7469 706c  f adding multipl
+0000ecd0: 6520 736f 6e67 732e 222c 0a29 0a40 636c  e songs.",.).@cl
+0000ece0: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
+0000ecf0: 222d 502f 2d6e 5022 2c0a 2020 2020 222d  "-P/-nP",.    "-
+0000ed00: 2d70 6c61 796c 6973 742f 2d2d 6e6f 2d70  -playlist/--no-p
+0000ed10: 6c61 796c 6973 7422 2c0a 2020 2020 2270  laylist",.    "p
+0000ed20: 6c61 796c 6973 745f 222c 0a20 2020 2064  laylist_",.    d
+0000ed30: 6566 6175 6c74 3d46 616c 7365 2c0a 2020  efault=False,.  
+0000ed40: 2020 6865 6c70 3d22 4966 2073 6f6e 6720    help="If song 
+0000ed50: 5552 4c20 7061 7373 6564 2069 7320 6672  URL passed is fr
+0000ed60: 6f6d 2061 2059 6f75 5475 6265 2070 6c61  om a YouTube pla
+0000ed70: 796c 6973 742c 2064 6f77 6e6c 6f61 6420  ylist, download 
+0000ed80: 616c 6c20 7468 6520 736f 6e67 732e 2049  all the songs. I
+0000ed90: 6620 7468 6520 5552 4c20 706f 696e 7473  f the URL points
+0000eda0: 2064 6972 6563 746c 7920 746f 2061 2070   directly to a p
+0000edb0: 6c61 796c 6973 742c 2074 6869 7320 666c  laylist, this fl
+0000edc0: 6167 2069 7320 756e 6e63 6573 7361 7279  ag is unncessary
+0000edd0: 2e22 2c0a 290a 4063 6c69 636b 2e6f 7074  .",.).@click.opt
+0000ede0: 696f 6e28 0a20 2020 2022 2d6d 222c 0a20  ion(.    "-m",. 
+0000edf0: 2020 2022 2d2d 6d65 7461 6461 7461 222c     "--metadata",
+0000ee00: 0a20 2020 2022 6d65 7461 6461 7461 5f70  .    "metadata_p
+0000ee10: 6169 7273 222c 0a20 2020 2064 6566 6175  airs",.    defau
+0000ee20: 6c74 3d4e 6f6e 652c 0a20 2020 2068 656c  lt=None,.    hel
+0000ee30: 703d 2241 6464 206d 6574 6164 6174 6120  p="Add metadata 
+0000ee40: 746f 2074 6865 2073 6f6e 672e 2049 676e  to the song. Ign
+0000ee50: 6f72 6564 2069 6620 6164 6469 6e67 206d  ored if adding m
+0000ee60: 756c 7469 706c 6520 736f 6e67 732e 2054  ultiple songs. T
+0000ee70: 6865 2066 6f72 6d61 7420 6973 2027 6b65  he format is 'ke
+0000ee80: 7931 3a76 616c 7565 317c 6b65 7932 3a76  y1:value1|key2:v
+0000ee90: 616c 7565 327c 2e2e 2e27 2e22 2c0a 290a  alue2|...'.",.).
+0000eea0: 6465 6620 6164 6428 0a20 2020 2070 6174  def add(.    pat
+0000eeb0: 685f 2c0a 2020 2020 7461 6773 2c0a 2020  h_,.    tags,.  
+0000eec0: 2020 6d6f 7665 5f2c 0a20 2020 206e 616d    move_,.    nam
+0000eed0: 652c 0a20 2020 2072 6563 7572 7365 2c0a  e,.    recurse,.
+0000eee0: 2020 2020 796f 7574 7562 652c 0a20 2020      youtube,.   
+0000eef0: 2073 706f 7469 6679 2c0a 2020 2020 666f   spotify,.    fo
+0000ef00: 726d 6174 5f2c 0a20 2020 2063 6c69 702c  rmat_,.    clip,
+0000ef10: 0a20 2020 2070 6c61 796c 6973 745f 2c0a  .    playlist_,.
+0000ef20: 2020 2020 6d65 7461 6461 7461 5f70 6169      metadata_pai
+0000ef30: 7273 2c0a 293a 0a20 2020 2022 2222 0a20  rs,.):.    """. 
+0000ef40: 2020 2041 6464 2061 206e 6577 2073 6f6e     Add a new son
+0000ef50: 672e 0a0a 2020 2020 4164 6473 2074 6865  g...    Adds the
+0000ef60: 2061 7564 696f 2066 696c 6520 6c6f 6361   audio file loca
+0000ef70: 7465 6420 6174 2050 4154 482e 2049 6620  ted at PATH. If 
+0000ef80: 5041 5448 2069 7320 6120 666f 6c64 6572  PATH is a folder
+0000ef90: 2c20 6164 6473 2061 6c6c 2066 696c 6573  , adds all files
+0000efa0: 0a20 2020 2069 6e20 5041 5448 2028 696e  .    in PATH (in
+0000efb0: 636c 7564 696e 6720 6669 6c65 7320 696e  cluding files in
+0000efc0: 2073 7562 666f 6c64 6572 7320 6966 2027   subfolders if '
+0000efd0: 2d72 2720 6973 2070 6173 7365 6429 2e20  -r' is passed). 
+0000efe0: 5468 6520 6e61 6d65 206f 6620 6561 6368  The name of each
+0000eff0: 0a20 2020 2073 6f6e 6720 7769 6c6c 2062  .    song will b
+0000f000: 6520 7468 6520 6669 6c65 6e61 6d65 2028  e the filename (
+0000f010: 756e 6c65 7373 2027 2d6e 2720 6973 2070  unless '-n' is p
+0000f020: 6173 7365 6429 2e20 4669 6c65 6e61 6d65  assed). Filename
+0000f030: 7320 616e 6420 7461 6773 2063 616e 6e6f  s and tags canno
+0000f040: 740a 2020 2020 636f 6e74 6169 6e20 7468  t.    contain th
+0000f050: 6520 6368 6172 6163 7465 7220 277c 272c  e character '|',
+0000f060: 2061 6e64 2074 6167 7320 6361 6e6e 6f74   and tags cannot
+0000f070: 2063 6f6e 7461 696e 2027 2c27 2e0a 0a20   contain ','... 
+0000f080: 2020 2049 6620 7468 6520 272d 5927 206f     If the '-Y' o
+0000f090: 7220 272d 2d79 6f75 7475 6265 2720 666c  r '--youtube' fl
+0000f0a0: 6167 2069 7320 7061 7373 6564 2c20 5041  ag is passed, PA
+0000f0b0: 5448 2069 7320 7472 6561 7465 6420 6173  TH is treated as
+0000f0c0: 2061 2059 6f75 5475 6265 206f 720a 2020   a YouTube or.  
+0000f0d0: 2020 596f 7554 7562 6520 4d75 7369 6320    YouTube Music 
+0000f0e0: 5552 4c20 696e 7374 6561 6420 6f66 2061  URL instead of a
+0000f0f0: 2066 696c 6520 7061 7468 2e0a 0a20 2020   file path...   
+0000f100: 2049 6620 7468 6520 272d 5327 206f 7220   If the '-S' or 
+0000f110: 272d 2d73 706f 7469 6679 2720 666c 6167  '--spotify' flag
+0000f120: 2069 7320 7061 7373 6564 2c20 5041 5448   is passed, PATH
+0000f130: 2069 7320 7472 6561 7465 6420 6173 2061   is treated as a
+0000f140: 2053 706f 7469 6679 0a20 2020 2074 7261   Spotify.    tra
+0000f150: 636b 2055 524c 2c20 616c 6275 6d20 5552  ck URL, album UR
+0000f160: 4c2c 2070 6c61 796c 6973 7420 5552 4c2c  L, playlist URL,
+0000f170: 2061 7274 6973 7420 5552 4c2c 206f 7220   artist URL, or 
+0000f180: 7365 6172 6368 2071 7565 7279 2069 6e73  search query ins
+0000f190: 7465 6164 206f 660a 2020 2020 6120 6669  tead of.    a fi
+0000f1a0: 6c65 2070 6174 682e 0a0a 2020 2020 5468  le path...    Th
+0000f1b0: 6520 272d 632f 2d2d 636c 6970 2720 6f70  e '-c/--clip' op
+0000f1c0: 7469 6f6e 2063 616e 2062 6520 7573 6564  tion can be used
+0000f1d0: 2074 6f20 6164 6420 6120 636c 6970 2066   to add a clip f
+0000f1e0: 6f72 2074 6865 2073 6f6e 672e 2049 7420  or the song. It 
+0000f1f0: 7461 6b65 7320 7477 6f0a 2020 2020 6172  takes two.    ar
+0000f200: 6775 6d65 6e74 732c 2062 7574 2075 6e6c  guments, but unl
+0000f210: 696b 6520 276d 6165 7374 726f 2063 6c69  ike 'maestro cli
+0000f220: 7027 2c20 796f 7520 6361 6e6e 6f74 2070  p', you cannot p
+0000f230: 6173 7320 6f6e 6c79 2074 6865 2073 7461  ass only the sta
+0000f240: 7274 2074 696d 650a 2020 2020 616e 6420  rt time.    and 
+0000f250: 6e6f 7420 7468 6520 656e 642e 2054 6f20  not the end. To 
+0000f260: 6765 7420 6172 6f75 6e64 2074 6869 732c  get around this,
+0000f270: 2079 6f75 2063 616e 2070 6173 7320 2d31   you can pass -1
+0000f280: 2061 7320 7468 6520 656e 6420 7469 6d65   as the end time
+0000f290: 2c20 652e 672e 0a20 2020 2027 6d61 6573  , e.g..    'maes
+0000f2a0: 7472 6f20 6164 6420 2d63 2033 3020 2d31  tro add -c 30 -1
+0000f2b0: 2068 7474 7073 3a2f 2f77 7777 2e79 6f75   https://www.you
+0000f2c0: 7475 6265 2e63 6f6d 2f77 6174 6368 3f76  tube.com/watch?v
+0000f2d0: 3d33 5678 754d 4572 4364 2d45 202d 7927  =3VxuMErCd-E -y'
+0000f2e0: 2e20 4966 0a20 2020 2061 6464 696e 6720  . If.    adding 
+0000f2f0: 6d75 6c74 6970 6c65 2073 6f6e 6773 2c20  multiple songs, 
+0000f300: 7468 6973 206f 7074 696f 6e20 6361 6e6e  this option cann
+0000f310: 6f74 2062 6520 7573 6564 2e0a 0a20 2020  ot be used...   
+0000f320: 2054 6865 2027 2d6d 2f2d 2d6d 6574 6164   The '-m/--metad
+0000f330: 6174 6127 206f 7074 696f 6e20 6361 6e20  ata' option can 
+0000f340: 6265 2075 7365 6420 746f 2061 6464 206d  be used to add m
+0000f350: 6574 6164 6174 6120 746f 2074 6865 2073  etadata to the s
+0000f360: 6f6e 672e 2049 7420 7461 6b65 730a 2020  ong. It takes.  
+0000f370: 2020 6120 7374 7269 6e67 206f 6620 7468    a string of th
+0000f380: 6520 666f 726d 6174 2027 6b65 7931 3a76  e format 'key1:v
+0000f390: 616c 7565 317c 6b65 7932 3a76 616c 7565  alue1|key2:value
+0000f3a0: 327c 2e2e 2e27 2e20 4966 2061 6464 696e  2|...'. If addin
+0000f3b0: 6720 6d75 6c74 6970 6c65 0a20 2020 2073  g multiple.    s
+0000f3c0: 6f6e 6773 2c20 7468 6973 206f 7074 696f  ongs, this optio
+0000f3d0: 6e20 6361 6e6e 6f74 2062 6520 7573 6564  n cannot be used
+0000f3e0: 2e0a 0a20 2020 2050 6f73 7369 626c 6520  ...    Possible 
+0000f3f0: 6564 6974 6162 6c65 206d 6574 6164 6174  editable metadat
+0000f400: 6120 6b65 7973 2061 7265 3a20 616c 6275  a keys are: albu
+0000f410: 6d2c 2061 6c62 756d 6172 7469 7374 2c20  m, albumartist, 
+0000f420: 6172 7469 7374 2c20 6172 7477 6f72 6b2c  artist, artwork,
+0000f430: 0a20 2020 2063 6f6d 6d65 6e74 2c20 636f  .    comment, co
+0000f440: 6d70 696c 6174 696f 6e2c 2063 6f6d 706f  mpilation, compo
+0000f450: 7365 722c 2064 6973 636e 756d 6265 722c  ser, discnumber,
+0000f460: 2067 656e 7265 2c20 6c79 7269 6373 2c20   genre, lyrics, 
+0000f470: 746f 7461 6c64 6973 6373 2c0a 2020 2020  totaldiscs,.    
+0000f480: 746f 7461 6c74 7261 636b 732c 2074 7261  totaltracks, tra
+0000f490: 636b 6e75 6d62 6572 2c20 7472 6163 6b74  cknumber, trackt
+0000f4a0: 6974 6c65 2c20 7965 6172 2c20 6973 7263  itle, year, isrc
+0000f4b0: 0a0a 2020 2020 4b65 7973 2061 7265 206e  ..    Keys are n
+0000f4c0: 6f74 2063 6173 6520 7365 6e73 6974 6976  ot case sensitiv
+0000f4d0: 6520 616e 6420 6361 6e20 636f 6e74 6169  e and can contai
+0000f4e0: 6e20 6172 6269 7472 6172 7920 7768 6974  n arbitrary whit
+0000f4f0: 6573 7061 6365 2c20 272d 272c 2061 6e64  espace, '-', and
+0000f500: 0a20 2020 2027 5f27 2063 6861 7261 6374  .    '_' charact
+0000f510: 6572 732e 2049 6e20 6f74 6865 7220 776f  ers. In other wo
+0000f520: 7264 732c 2027 416c 6275 6d20 4172 7469  rds, 'Album Arti
+0000f530: 7374 272c 2027 616c 6275 6d2d 6172 7469  st', 'album-arti
+0000f540: 7374 272c 2061 6e64 0a20 2020 2027 616c  st', and.    'al
+0000f550: 6275 6d5f 6172 7469 7374 2720 6172 6520  bum_artist' are 
+0000f560: 616c 6c20 7379 6e6f 6e79 6d73 2066 6f72  all synonyms for
+0000f570: 2027 616c 6275 6d61 7274 6973 7427 2e20   'albumartist'. 
+0000f580: 416c 736f 2c20 2764 6973 6b27 2069 730a  Also, 'disk' is.
+0000f590: 2020 2020 7379 6e6f 6e79 6d6f 7573 2077      synonymous w
+0000f5a0: 6974 6820 2764 6973 6327 2e0a 2020 2020  ith 'disc'..    
+0000f5b0: 2222 220a 0a20 2020 2070 6174 6873 203d  """..    paths =
+0000f5c0: 204e 6f6e 650a 2020 2020 6966 206e 6f74   None.    if not
+0000f5d0: 2028 796f 7574 7562 6520 6f72 2073 706f   (youtube or spo
+0000f5e0: 7469 6679 2920 616e 6420 6e6f 7420 6f73  tify) and not os
+0000f5f0: 2e70 6174 682e 6578 6973 7473 2870 6174  .path.exists(pat
+0000f600: 685f 293a 0a20 2020 2020 2020 2063 6c69  h_):.        cli
+0000f610: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
+0000f620: 2020 2020 2020 6622 5468 6520 7061 7468        f"The path
+0000f630: 2027 7b70 6174 685f 7d27 2064 6f65 7320   '{path_}' does 
+0000f640: 6e6f 7420 6578 6973 742e 2054 6f20 646f  not exist. To do
+0000f650: 776e 6c6f 6164 2066 726f 6d20 6120 596f  wnload from a Yo
+0000f660: 7554 7562 6520 6f72 2059 6f75 5475 6265  uTube or YouTube
+0000f670: 204d 7573 6963 2055 526c 2c20 7061 7373   Music URl, pass
+0000f680: 2074 6865 2027 2d59 2f2d 2d79 6f75 7475   the '-Y/--youtu
+0000f690: 6265 2720 666c 6167 2e20 546f 2064 6f77  be' flag. To dow
+0000f6a0: 6e6c 6f61 6420 6672 6f6d 2061 2053 706f  nload from a Spo
+0000f6b0: 7469 6679 2055 526c 2c20 7061 7373 2074  tify URl, pass t
+0000f6c0: 6865 2027 2d53 2f2d 2d73 706f 7469 6679  he '-S/--spotify
+0000f6d0: 2720 666c 6167 2e22 2c0a 2020 2020 2020  ' flag.",.      
+0000f6e0: 2020 2020 2020 6667 3d22 7265 6422 2c0a        fg="red",.
+0000f6f0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000f700: 2020 7265 7475 726e 0a0a 2020 2020 6966    return..    if
+0000f710: 2079 6f75 7475 6265 206f 7220 7370 6f74   youtube or spot
+0000f720: 6966 793a 0a20 2020 2020 2020 2069 6620  ify:.        if 
+0000f730: 796f 7574 7562 6520 616e 6420 7370 6f74  youtube and spot
+0000f740: 6966 793a 0a20 2020 2020 2020 2020 2020  ify:.           
+0000f750: 2063 6c69 636b 2e73 6563 686f 280a 2020   click.secho(.  
+0000f760: 2020 2020 2020 2020 2020 2020 2020 2243                "C
+0000f770: 616e 6e6f 7420 7061 7373 2062 6f74 6820  annot pass both 
+0000f780: 272d 792f 2d2d 796f 7574 7562 6527 2061  '-y/--youtube' a
+0000f790: 6e64 2027 2d73 2f2d 2d73 706f 7469 6679  nd '-s/--spotify
+0000f7a0: 2720 666c 6167 732e 222c 0a20 2020 2020  ' flags.",.     
+0000f7b0: 2020 2020 2020 2020 2020 2066 673d 2272             fg="r
+0000f7c0: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
+0000f7d0: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
+0000f7e0: 6574 7572 6e0a 0a20 2020 2020 2020 2069  eturn..        i
+0000f7f0: 6620 796f 7574 7562 653a 0a20 2020 2020  f youtube:.     
+0000f800: 2020 2020 2020 2069 6620 666f 726d 6174         if format
+0000f810: 5f20 3d3d 2022 6f67 6722 3a0a 2020 2020  _ == "ogg":.    
+0000f820: 2020 2020 2020 2020 2020 2020 636c 6963              clic
+0000f830: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
+0000f840: 2020 2020 2020 2020 2020 2020 2022 4361               "Ca
+0000f850: 6e6e 6f74 2064 6f77 6e6c 6f61 6420 736f  nnot download so
+0000f860: 6e67 7320 6672 6f6d 2059 6f75 5475 6265  ngs from YouTube
+0000f870: 2061 7320 272e 6f67 6727 2e20 506c 6561   as '.ogg'. Plea
+0000f880: 7365 2063 686f 6f73 6520 6120 6469 6666  se choose a diff
+0000f890: 6572 656e 7420 666f 726d 6174 2e22 2c0a  erent format.",.
+0000f8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8b0: 2020 2020 6667 3d22 7265 6422 2c0a 2020      fg="red",.  
+0000f8c0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8e0: 7265 7475 726e 0a20 2020 2020 2020 2020  return.         
+0000f8f0: 2020 2073 7562 7072 6f63 6573 732e 7275     subprocess.ru
+0000f900: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0000f910: 2020 205b 0a20 2020 2020 2020 2020 2020     [.           
+0000f920: 2020 2020 2020 2020 2022 7974 2d64 6c70           "yt-dlp
+0000f930: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000f940: 2020 2020 2020 2070 6174 685f 2c0a 2020         path_,.  
+0000f950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f960: 2020 222d 7822 2c20 2023 2065 7874 7261    "-x",  # extra
+0000f970: 6374 2061 7564 696f 2028 6e65 6365 7373  ct audio (necess
+0000f980: 6172 792c 206e 6565 6473 2066 666d 7065  ary, needs ffmpe
+0000f990: 6729 0a20 2020 2020 2020 2020 2020 2020  g).             
+0000f9a0: 2020 2020 2020 2022 2d2d 6175 6469 6f2d         "--audio-
+0000f9b0: 666f 726d 6174 222c 0a20 2020 2020 2020  format",.       
+0000f9c0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000f9d0: 6d61 745f 2c0a 2020 2020 2020 2020 2020  mat_,.          
+0000f9e0: 2020 2020 2020 2020 2020 222d 2d6e 6f2d            "--no-
+0000f9f0: 706c 6179 6c69 7374 2220 6966 206e 6f74  playlist" if not
+0000fa00: 2070 6c61 796c 6973 745f 2065 6c73 6520   playlist_ else 
+0000fa10: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+0000fa20: 2020 2020 2020 2020 222d 2d65 6d62 6564          "--embed
+0000fa30: 2d6d 6574 6164 6174 6122 2c0a 2020 2020  -metadata",.    
+0000fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa50: 222d 6f22 2c0a 2020 2020 2020 2020 2020  "-o",.          
+0000fa60: 2020 2020 2020 2020 2020 6f73 2e70 6174            os.pat
+0000fa70: 682e 6a6f 696e 284d 4145 5354 524f 5f44  h.join(MAESTRO_D
+0000fa80: 4952 2c20 2225 2874 6974 6c65 2973 2e25  IR, "%(title)s.%
+0000fa90: 2865 7874 2973 2229 2c0a 2020 2020 2020  (ext)s"),.      
+0000faa0: 2020 2020 2020 2020 2020 5d2c 0a20 2020            ],.   
+0000fab0: 2020 2020 2020 2020 2020 2020 2063 6865               che
+0000fac0: 636b 3d54 7275 652c 0a20 2020 2020 2020  ck=True,.       
+0000fad0: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
+0000fae0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000faf0: 2069 6620 666f 726d 6174 5f20 3d3d 2022   if format_ == "
+0000fb00: 7761 7622 3a0a 2020 2020 2020 2020 2020  wav":.          
+0000fb10: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
+0000fb20: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
+0000fb30: 2020 2020 2020 2022 4361 6e6e 6f74 2064         "Cannot d
+0000fb40: 6f77 6e6c 6f61 6420 736f 6e67 7320 6672  ownload songs fr
+0000fb50: 6f6d 2053 706f 7469 6679 2061 7320 272e  om Spotify as '.
+0000fb60: 7761 7627 2e20 506c 6561 7365 2063 686f  wav'. Please cho
+0000fb70: 6f73 6520 6120 6469 6666 6572 656e 7420  ose a different 
+0000fb80: 666f 726d 6174 2e22 2c0a 2020 2020 2020  format.",.      
+0000fb90: 2020 2020 2020 2020 2020 2020 2020 6667                fg
+0000fba0: 3d22 7265 6422 2c0a 2020 2020 2020 2020  ="red",.        
+0000fbb0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000fbc0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000fbd0: 0a0a 2020 2020 2020 2020 2020 2020 6377  ..            cw
+0000fbe0: 6420 3d20 6f73 2e67 6574 6377 6428 290a  d = os.getcwd().
+0000fbf0: 2020 2020 2020 2020 2020 2020 6f73 2e63              os.c
+0000fc00: 6864 6972 284d 4145 5354 524f 5f44 4952  hdir(MAESTRO_DIR
+0000fc10: 290a 2020 2020 2020 2020 2020 2020 7472  ).            tr
+0000fc20: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
+0000fc30: 2020 2073 7562 7072 6f63 6573 732e 7275     subprocess.ru
+0000fc40: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+0000fc50: 2020 2020 2020 205b 0a20 2020 2020 2020         [.       
+0000fc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc70: 2022 7370 6f74 646c 222c 0a20 2020 2020   "spotdl",.     
+0000fc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fc90: 2020 2022 646f 776e 6c6f 6164 222c 0a20     "download",. 
+0000fca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcb0: 2020 2020 2020 2070 6174 685f 2c0a 2020         path_,.  
+0000fcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fcd0: 2020 2020 2020 222d 2d6f 7574 7075 7422        "--output"
+0000fce0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000fcf0: 2020 2020 2020 2020 2020 227b 7469 746c            "{titl
+0000fd00: 657d 2e7b 6f75 7470 7574 2d65 7874 7d22  e}.{output-ext}"
+0000fd10: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000fd20: 2020 2020 2020 2020 2020 222d 2d66 6f72            "--for
+0000fd30: 6d61 7422 2c0a 2020 2020 2020 2020 2020  mat",.          
+0000fd40: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+0000fd50: 726d 6174 5f2c 0a20 2020 2020 2020 2020  rmat_,.         
+0000fd60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000fd70: 2d2d 6865 6164 6c65 7373 222c 0a20 2020  --headless",.   
+0000fd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd90: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
+0000fda0: 2020 2020 2020 2020 6368 6563 6b3d 5472          check=Tr
+0000fdb0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+0000fdc0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+0000fdd0: 2020 6578 6365 7074 2045 7863 6570 7469    except Excepti
+0000fde0: 6f6e 2061 7320 6572 723a 0a20 2020 2020  on as err:.     
+0000fdf0: 2020 2020 2020 2020 2020 206f 732e 6368             os.ch
+0000fe00: 6469 7228 6377 6429 0a20 2020 2020 2020  dir(cwd).       
+0000fe10: 2020 2020 2020 2020 2072 6169 7365 2065           raise e
+0000fe20: 7272 0a0a 2020 2020 2020 2020 7061 7468  rr..        path
+0000fe30: 7320 3d20 5b5d 0a20 2020 2020 2020 2066  s = [].        f
+0000fe40: 6f72 2066 6e61 6d65 2069 6e20 6f73 2e6c  or fname in os.l
+0000fe50: 6973 7464 6972 284d 4145 5354 524f 5f44  istdir(MAESTRO_D
+0000fe60: 4952 293a 0a20 2020 2020 2020 2020 2020  IR):.           
+0000fe70: 2066 6f72 2066 2069 6e20 5b22 2e77 6176   for f in [".wav
+0000fe80: 222c 2022 2e6d 7033 222c 2022 2e66 6c61  ", ".mp3", ".fla
+0000fe90: 6322 2c20 222e 6f67 6722 5d3a 0a20 2020  c", ".ogg"]:.   
+0000fea0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000feb0: 666e 616d 652e 656e 6473 7769 7468 2866  fname.endswith(f
+0000fec0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000fed0: 2020 2020 2020 2072 6177 5f70 6174 6820         raw_path 
+0000fee0: 3d20 6f73 2e70 6174 682e 6a6f 696e 284d  = os.path.join(M
+0000fef0: 4145 5354 524f 5f44 4952 2c20 666e 616d  AESTRO_DIR, fnam
+0000ff00: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0000ff10: 2020 2020 2020 2073 616e 6974 697a 6564         sanitized
+0000ff20: 5f70 6174 6820 3d20 7261 775f 7061 7468  _path = raw_path
+0000ff30: 2e72 6570 6c61 6365 2822 7c22 2c20 222d  .replace("|", "-
+0000ff40: 2229 0a0a 2020 2020 2020 2020 2020 2020  ")..            
+0000ff50: 2020 2020 2020 2020 6f73 2e72 656e 616d          os.renam
+0000ff60: 6528 7261 775f 7061 7468 2c20 7361 6e69  e(raw_path, sani
+0000ff70: 7469 7a65 645f 7061 7468 290a 0a20 2020  tized_path)..   
+0000ff80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ff90: 2070 6174 6873 2e61 7070 656e 6428 7361   paths.append(sa
+0000ffa0: 6e69 7469 7a65 645f 7061 7468 290a 2020  nitized_path).  
+0000ffb0: 2020 2020 2020 2020 2020 6966 2066 6e61            if fna
+0000ffc0: 6d65 2e65 6e64 7377 6974 6828 222e 7061  me.endswith(".pa
+0000ffd0: 7274 2229 3a20 2023 2064 656c 6574 6520  rt"):  # delete 
+0000ffe0: 696e 636f 6d70 6c65 7465 2064 6f77 6e6c  incomplete downl
+0000fff0: 6f61 6473 0a20 2020 2020 2020 2020 2020  oads.           
+00010000: 2020 2020 206f 732e 7265 6d6f 7665 286f       os.remove(o
+00010010: 732e 7061 7468 2e6a 6f69 6e28 4d41 4553  s.path.join(MAES
+00010020: 5452 4f5f 4449 522c 2066 6e61 6d65 2929  TRO_DIR, fname))
+00010030: 0a0a 2020 2020 2020 2020 6d6f 7665 5f20  ..        move_ 
+00010040: 3d20 5472 7565 0a0a 2020 2020 6966 2070  = True..    if p
+00010050: 6174 6873 2069 7320 4e6f 6e65 3a0a 2020  aths is None:.  
+00010060: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
+00010070: 2e69 7364 6972 2870 6174 685f 293a 0a20  .isdir(path_):. 
+00010080: 2020 2020 2020 2020 2020 2070 6174 6873             paths
+00010090: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+000100a0: 2020 6966 2072 6563 7572 7365 3a0a 2020    if recurse:.  
+000100b0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000100c0: 7220 6469 7270 6174 682c 205f 2c20 666e  r dirpath, _, fn
+000100d0: 616d 6573 2069 6e20 6f73 2e77 616c 6b28  ames in os.walk(
+000100e0: 7061 7468 5f29 3a0a 2020 2020 2020 2020  path_):.        
+000100f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00010100: 666e 616d 6520 696e 2066 6e61 6d65 733a  fname in fnames:
+00010110: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010120: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
+00010130: 6174 682e 7370 6c69 7465 7874 2866 6e61  ath.splitext(fna
+00010140: 6d65 295b 315d 2069 6e20 4558 5453 3a0a  me)[1] in EXTS:.
+00010150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010160: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00010170: 732e 6170 7065 6e64 286f 732e 7061 7468  s.append(os.path
+00010180: 2e6a 6f69 6e28 6469 7270 6174 682c 2066  .join(dirpath, f
+00010190: 6e61 6d65 2929 0a20 2020 2020 2020 2020  name)).         
+000101a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000101b0: 2020 2020 2020 2020 2066 6f72 2066 6e61           for fna
+000101c0: 6d65 2069 6e20 6f73 2e6c 6973 7464 6972  me in os.listdir
+000101d0: 2870 6174 685f 293a 0a20 2020 2020 2020  (path_):.       
+000101e0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000101f0: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
+00010200: 2866 6e61 6d65 295b 315d 2069 6e20 4558  (fname)[1] in EX
+00010210: 5453 3a0a 2020 2020 2020 2020 2020 2020  TS:.            
+00010220: 2020 2020 2020 2020 2020 2020 6675 6c6c              full
+00010230: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+00010240: 6a6f 696e 2870 6174 685f 2c20 666e 616d  join(path_, fnam
+00010250: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00010260: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+00010270: 2e70 6174 682e 6973 6669 6c65 2866 756c  .path.isfile(ful
+00010280: 6c5f 7061 7468 293a 0a20 2020 2020 2020  l_path):.       
+00010290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000102a0: 2020 2020 2070 6174 6873 2e61 7070 656e       paths.appen
+000102b0: 6428 6675 6c6c 5f70 6174 6829 0a20 2020  d(full_path).   
+000102c0: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+000102d0: 7061 7468 7329 203d 3d20 303a 0a20 2020  paths) == 0:.   
+000102e0: 2020 2020 2020 2020 2020 2020 2063 6c69               cli
+000102f0: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
+00010300: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00010310: 4e6f 2073 6f6e 6773 2066 6f75 6e64 2069  No songs found i
+00010320: 6e20 277b 7061 7468 5f7d 272e 222c 0a20  n '{path_}'.",. 
+00010330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010340: 2020 2066 673d 2272 6564 222c 0a20 2020     fg="red",.   
+00010350: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00010360: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00010370: 6574 7572 6e0a 2020 2020 2020 2020 656c  eturn.        el
+00010380: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00010390: 7061 7468 7320 3d20 5b70 6174 685f 5d0a  paths = [path_].
+000103a0: 0a20 2020 2069 6620 6c65 6e28 7061 7468  .    if len(path
+000103b0: 7329 203e 2031 3a0a 2020 2020 2020 2020  s) > 1:.        
+000103c0: 6966 2063 6c69 7020 6973 206e 6f74 204e  if clip is not N
+000103d0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000103e0: 2063 6c69 636b 2e73 6563 686f 280a 2020   click.secho(.  
+000103f0: 2020 2020 2020 2020 2020 2020 2020 2243                "C
+00010400: 616e 6e6f 7420 7061 7373 2027 2d63 2f2d  annot pass '-c/-
+00010410: 2d63 6c69 7027 206f 7074 696f 6e20 7768  -clip' option wh
+00010420: 656e 2061 6464 696e 6720 6d75 6c74 6970  en adding multip
+00010430: 6c65 2073 6f6e 6773 2e22 2c0a 2020 2020  le songs.",.    
+00010440: 2020 2020 2020 2020 2020 2020 6667 3d22              fg="
+00010450: 7265 6422 2c0a 2020 2020 2020 2020 2020  red",.          
+00010460: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00010470: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
+00010480: 6966 206e 616d 6520 6973 206e 6f74 204e  if name is not N
+00010490: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000104a0: 2063 6c69 636b 2e73 6563 686f 280a 2020   click.secho(.  
+000104b0: 2020 2020 2020 2020 2020 2020 2020 2243                "C
+000104c0: 616e 6e6f 7420 7061 7373 2027 2d6e 2f2d  annot pass '-n/-
+000104d0: 2d6e 616d 6527 206f 7074 696f 6e20 7768  -name' option wh
+000104e0: 656e 2061 6464 696e 6720 6d75 6c74 6970  en adding multip
+000104f0: 6c65 2073 6f6e 6773 2e22 2c0a 2020 2020  le songs.",.    
+00010500: 2020 2020 2020 2020 2020 2020 6667 3d22              fg="
+00010510: 7265 6422 2c0a 2020 2020 2020 2020 2020  red",.          
+00010520: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00010530: 7265 7475 726e 0a0a 2020 2020 6966 206c  return..    if l
+00010540: 656e 2870 6174 6873 2920 3d3d 2031 2061  en(paths) == 1 a
+00010550: 6e64 206e 616d 6520 6973 206e 6f74 204e  nd name is not N
+00010560: 6f6e 653a 0a20 2020 2020 2020 206e 6577  one:.        new
+00010570: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
+00010580: 6a6f 696e 280a 2020 2020 2020 2020 2020  join(.          
+00010590: 2020 4d41 4553 5452 4f5f 4449 522c 206e    MAESTRO_DIR, n
+000105a0: 616d 6520 2b20 6f73 2e70 6174 682e 7370  ame + os.path.sp
+000105b0: 6c69 7465 7874 2870 6174 6873 5b30 5d29  litext(paths[0])
+000105c0: 5b31 5d0a 2020 2020 2020 2020 290a 2020  [1].        ).  
+000105d0: 2020 2020 2020 2320 6d6f 7665 2f63 6f70        # move/cop
+000105e0: 7920 746f 204d 4145 5354 524f 5f44 4952  y to MAESTRO_DIR
+000105f0: 2028 6176 6f69 6420 6e61 6d65 2063 6f6e   (avoid name con
+00010600: 666c 6963 7473 290a 2020 2020 2020 2020  flicts).        
+00010610: 6966 206d 6f76 655f 3a0a 2020 2020 2020  if move_:.      
+00010620: 2020 2020 2020 6d6f 7665 2870 6174 6873        move(paths
+00010630: 5b30 5d2c 206e 6577 5f70 6174 6829 0a20  [0], new_path). 
+00010640: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00010650: 2020 2020 2020 2020 2063 6f70 7928 7061           copy(pa
+00010660: 7468 735b 305d 2c20 6e65 775f 7061 7468  ths[0], new_path
+00010670: 290a 2020 2020 2020 2020 7061 7468 7320  ).        paths 
+00010680: 3d20 5b6e 6577 5f70 6174 685d 0a20 2020  = [new_path].   
+00010690: 2020 2020 206d 6f76 655f 203d 2054 7275       move_ = Tru
+000106a0: 6520 2023 2061 6c77 6179 7320 6d6f 7665  e  # always move
+000106b0: 2028 6672 6f6d 2074 656d 7020 6c6f 6320   (from temp loc 
+000106c0: 696e 204d 4145 5354 524f 5f44 4952 2920  in MAESTRO_DIR) 
+000106d0: 6966 2072 656e 616d 696e 670a 0a20 2020  if renaming..   
+000106e0: 2069 6620 636c 6970 2069 7320 6e6f 7420   if clip is not 
+000106f0: 4e6f 6e65 2061 6e64 206c 656e 2870 6174  None and len(pat
+00010700: 6873 2920 3d3d 2031 3a0a 2020 2020 2020  hs) == 1:.      
+00010710: 2020 736f 6e67 5f64 7572 6174 696f 6e20    song_duration 
+00010720: 3d20 6d75 7369 635f 7461 672e 6c6f 6164  = music_tag.load
+00010730: 5f66 696c 6528 7061 7468 735b 305d 295b  _file(paths[0])[
+00010740: 2223 6c65 6e67 7468 225d 2e76 616c 7565  "#length"].value
+00010750: 0a0a 2020 2020 2020 2020 7374 6172 742c  ..        start,
+00010760: 2065 6e64 203d 2063 6c69 700a 2020 2020   end = clip.    
+00010770: 2020 2020 6966 2073 7461 7274 203c 2030      if start < 0
+00010780: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+00010790: 6963 6b2e 7365 6368 6f28 2243 6c69 7020  ick.secho("Clip 
+000107a0: 7374 6172 7420 7469 6d65 2063 616e 6e6f  start time canno
+000107b0: 7420 6265 206e 6567 6174 6976 652e 222c  t be negative.",
+000107c0: 2066 673d 2272 6564 2229 0a20 2020 2020   fg="red").     
+000107d0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000107e0: 2020 2020 2020 6966 2073 7461 7274 203e        if start >
+000107f0: 2073 6f6e 675f 6475 7261 7469 6f6e 3a0a   song_duration:.
+00010800: 2020 2020 2020 2020 2020 2020 636c 6963              clic
+00010810: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
+00010820: 2020 2020 2020 2020 2022 436c 6970 2073           "Clip s
+00010830: 7461 7274 2074 696d 6520 6361 6e6e 6f74  tart time cannot
+00010840: 2062 6520 6772 6561 7465 7220 7468 616e   be greater than
+00010850: 2074 6865 2073 6f6e 6720 6475 7261 7469   the song durati
+00010860: 6f6e 2e22 2c0a 2020 2020 2020 2020 2020  on.",.          
+00010870: 2020 2020 2020 6667 3d22 7265 6422 2c0a        fg="red",.
+00010880: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00010890: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000108a0: 0a0a 2020 2020 2020 2020 6966 2065 6e64  ..        if end
+000108b0: 203d 3d20 2d31 3a0a 2020 2020 2020 2020   == -1:.        
+000108c0: 2020 2020 656e 6420 3d20 736f 6e67 5f64      end = song_d
+000108d0: 7572 6174 696f 6e0a 2020 2020 2020 2020  uration.        
+000108e0: 656c 6966 2065 6e64 203c 2073 7461 7274  elif end < start
+000108f0: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+00010900: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
+00010910: 2020 2020 2020 2020 2020 2022 436c 6970             "Clip
+00010920: 2065 6e64 2074 696d 6520 6361 6e6e 6f74   end time cannot
+00010930: 2062 6520 6c65 7373 2074 6861 6e20 7468   be less than th
+00010940: 6520 636c 6970 2073 7461 7274 2074 696d  e clip start tim
+00010950: 652e 222c 0a20 2020 2020 2020 2020 2020  e.",.           
+00010960: 2020 2020 2066 673d 2272 6564 222c 0a20       fg="red",. 
+00010970: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00010980: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00010990: 2020 2020 2020 2020 656c 6966 2065 6e64          elif end
+000109a0: 203e 2073 6f6e 675f 6475 7261 7469 6f6e   > song_duration
+000109b0: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+000109c0: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
+000109d0: 2020 2020 2020 2020 2020 2022 436c 6970             "Clip
+000109e0: 2065 6e64 2074 696d 6520 6361 6e6e 6f74   end time cannot
+000109f0: 2062 6520 6772 6561 7465 7220 7468 616e   be greater than
+00010a00: 2074 6865 2073 6f6e 6720 6475 7261 7469   the song durati
+00010a10: 6f6e 2e22 2c0a 2020 2020 2020 2020 2020  on.",.          
+00010a20: 2020 2020 2020 6667 3d22 7265 6422 2c0a        fg="red",.
+00010a30: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00010a40: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010a50: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00010a60: 2020 2073 7461 7274 203d 2065 6e64 203d     start = end =
+00010a70: 204e 6f6e 650a 0a20 2020 2069 6620 6d65   None..    if me
+00010a80: 7461 6461 7461 5f70 6169 7273 2069 7320  tadata_pairs is 
+00010a90: 6e6f 7420 4e6f 6e65 2061 6e64 206c 656e  not None and len
+00010aa0: 2870 6174 6873 2920 3d3d 2031 3a0a 2020  (paths) == 1:.  
+00010ab0: 2020 2020 2020 2320 636f 6e76 6572 7420        # convert 
+00010ac0: 6672 6f6d 2022 6b65 793a 7661 6c75 652c  from "key:value,
+00010ad0: 6b65 793a 7661 6c75 6522 2074 6f20 5b28  key:value" to [(
+00010ae0: 226b 6579 222c 2022 7661 6c75 6522 295d  "key", "value")]
+00010af0: 0a20 2020 2020 2020 206d 6574 6164 6174  .        metadat
+00010b00: 615f 7061 6972 7320 3d20 5b0a 2020 2020  a_pairs = [.    
+00010b10: 2020 2020 2020 2020 7475 706c 6528 7061          tuple(pa
+00010b20: 6972 2e73 7472 6970 2829 2e73 706c 6974  ir.strip().split
+00010b30: 2822 3a22 2929 2066 6f72 2070 6169 7220  (":")) for pair 
+00010b40: 696e 206d 6574 6164 6174 615f 7061 6972  in metadata_pair
+00010b50: 732e 7370 6c69 7428 227c 2229 0a20 2020  s.split("|").   
+00010b60: 2020 2020 205d 0a20 2020 2020 2020 2073       ].        s
+00010b70: 6f6e 675f 6461 7461 203d 206d 7573 6963  ong_data = music
+00010b80: 5f74 6167 2e6c 6f61 645f 6669 6c65 2870  _tag.load_file(p
+00010b90: 6174 6873 5b30 5d29 0a20 2020 2020 2020  aths[0]).       
+00010ba0: 2066 6f72 206b 6579 2c20 7661 6c75 6520   for key, value 
+00010bb0: 696e 206d 6574 6164 6174 615f 7061 6972  in metadata_pair
+00010bc0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+00010bd0: 6620 6b65 7920 6e6f 7420 696e 204d 4554  f key not in MET
+00010be0: 4144 4154 415f 4b45 5953 206f 7220 6b65  ADATA_KEYS or ke
+00010bf0: 792e 7374 6172 7473 7769 7468 2822 2322  y.startswith("#"
+00010c00: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00010c10: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
+00010c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010c30: 2020 2020 6622 277b 6b65 797d 2720 6973      f"'{key}' is
+00010c40: 206e 6f74 2061 2076 616c 6964 2065 6469   not a valid edi
+00010c50: 7461 626c 6520 6d65 7461 6461 7461 206b  table metadata k
+00010c60: 6579 2e22 2c20 6667 3d22 7265 6422 0a20  ey.", fg="red". 
+00010c70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010c90: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
+00010ca0: 2020 2020 2020 736f 6e67 5f64 6174 615b        song_data[
+00010cb0: 6b65 795d 203d 2076 616c 7565 0a20 2020  key] = value.   
+00010cc0: 2020 2020 2073 6f6e 675f 6461 7461 2e73       song_data.s
+00010cd0: 6176 6528 290a 0a20 2020 2066 6f72 2070  ave()..    for p
+00010ce0: 6174 6820 696e 2070 6174 6873 3a0a 2020  ath in paths:.  
+00010cf0: 2020 2020 2020 6578 7420 3d20 6f73 2e70        ext = os.p
+00010d00: 6174 682e 7370 6c69 7465 7874 2870 6174  ath.splitext(pat
+00010d10: 6829 5b31 5d0a 2020 2020 2020 2020 6966  h)[1].        if
+00010d20: 206e 6f74 206f 732e 7061 7468 2e69 7364   not os.path.isd
+00010d30: 6972 2870 6174 6829 2061 6e64 2065 7874  ir(path) and ext
+00010d40: 206e 6f74 2069 6e20 4558 5453 3a0a 2020   not in EXTS:.  
+00010d50: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+00010d60: 7365 6368 6f28 6622 277b 6578 747d 2720  secho(f"'{ext}' 
+00010d70: 6973 206e 6f74 2073 7570 706f 7274 6564  is not supported
+00010d80: 2e22 2c20 6667 3d22 7265 6422 290a 2020  .", fg="red").  
+00010d90: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00010da0: 0a0a 2020 2020 2020 2020 666f 7220 7461  ..        for ta
+00010db0: 6720 696e 2074 6167 733a 0a20 2020 2020  g in tags:.     
+00010dc0: 2020 2020 2020 2069 6620 222c 2220 696e         if "," in
+00010dd0: 2074 6167 206f 7220 227c 2220 696e 2074   tag or "|" in t
+00010de0: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
+00010df0: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
+00010e00: 2254 6167 7320 6361 6e6e 6f74 2063 6f6e  "Tags cannot con
+00010e10: 7461 696e 2027 2c27 206f 7220 277c 272e  tain ',' or '|'.
+00010e20: 222c 2066 673d 2272 6564 2229 0a20 2020  ", fg="red").   
+00010e30: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00010e40: 7572 6e0a 0a20 2020 2020 2020 2077 6974  urn..        wit
+00010e50: 6820 6f70 656e 2853 4f4e 4753 5f49 4e46  h open(SONGS_INF
+00010e60: 4f5f 5041 5448 2c20 2261 2b22 2c20 656e  O_PATH, "a+", en
+00010e70: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
+00010e80: 6173 2073 6f6e 6773 5f66 696c 653a 0a20  as songs_file:. 
+00010e90: 2020 2020 2020 2020 2020 2073 6f6e 6773             songs
+00010ea0: 5f66 696c 652e 7365 656b 2830 2920 2023  _file.seek(0)  #
+00010eb0: 2073 7461 7274 2072 6561 6469 6e67 2066   start reading f
+00010ec0: 726f 6d20 6265 6769 6e6e 696e 670a 0a20  rom beginning.. 
+00010ed0: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+00010ee0: 203d 2073 6f6e 6773 5f66 696c 652e 7265   = songs_file.re
+00010ef0: 6164 6c69 6e65 7328 290a 0a20 2020 2020  adlines()..     
+00010f00: 2020 2020 2020 2073 6f6e 675f 6964 203d         song_id =
+00010f10: 2031 0a20 2020 2020 2020 2020 2020 2066   1.            f
+00010f20: 6f72 206c 696e 6520 696e 206c 696e 6573  or line in lines
+00010f30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010f40: 2020 736f 6e67 5f69 6420 3d20 6d61 7828    song_id = max(
+00010f50: 736f 6e67 5f69 642c 2069 6e74 286c 696e  song_id, int(lin
+00010f60: 652e 7370 6c69 7428 227c 2229 5b30 5d29  e.split("|")[0])
+00010f70: 202b 2031 290a 0a20 2020 2020 2020 2020   + 1)..         
+00010f80: 2020 2070 7265 7065 6e64 5f6e 6577 6c69     prepend_newli
+00010f90: 6e65 203d 206c 696e 6573 2061 6e64 206c  ne = lines and l
+00010fa0: 696e 6573 5b2d 315d 5b2d 315d 2021 3d20  ines[-1][-1] != 
+00010fb0: 225c 6e22 0a0a 2020 2020 2020 2020 2020  "\n"..          
+00010fc0: 2020 6164 645f 736f 6e67 280a 2020 2020    add_song(.    
+00010fd0: 2020 2020 2020 2020 2020 2020 7061 7468              path
+00010fe0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010ff0: 2020 7461 6773 2c0a 2020 2020 2020 2020    tags,.        
+00011000: 2020 2020 2020 2020 6d6f 7665 5f2c 0a20          move_,. 
+00011010: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00011020: 6f6e 6773 5f66 696c 652c 0a20 2020 2020  ongs_file,.     
+00011030: 2020 2020 2020 2020 2020 206c 696e 6573             lines
+00011040: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011050: 2020 736f 6e67 5f69 642c 0a20 2020 2020    song_id,.     
+00011060: 2020 2020 2020 2020 2020 2070 7265 7065             prepe
+00011070: 6e64 5f6e 6577 6c69 6e65 2c0a 2020 2020  nd_newline,.    
+00011080: 2020 2020 2020 2020 2020 2020 7374 6172              star
+00011090: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+000110a0: 2020 2065 6e64 2c0a 2020 2020 2020 2020     end,.        
+000110b0: 2020 2020 290a 0a0a 4063 6c69 2e63 6f6d      )...@cli.com
+000110c0: 6d61 6e64 2829 0a40 636c 6963 6b2e 6172  mand().@click.ar
+000110d0: 6775 6d65 6e74 2822 4152 4753 222c 2072  gument("ARGS", r
+000110e0: 6571 7569 7265 643d 5472 7565 2c20 6e61  equired=True, na
+000110f0: 7267 733d 2d31 290a 4063 6c69 636b 2e6f  rgs=-1).@click.o
+00011100: 7074 696f 6e28 0a20 2020 2022 2d46 2f2d  ption(.    "-F/-
+00011110: 6e46 222c 2022 2d2d 666f 7263 652f 2d2d  nF", "--force/--
+00011120: 6e6f 2d66 6f72 6365 222c 2064 6566 6175  no-force", defau
+00011130: 6c74 3d46 616c 7365 2c20 6865 6c70 3d22  lt=False, help="
+00011140: 466f 7263 6520 6465 6c65 7469 6f6e 2e22  Force deletion."
+00011150: 0a29 0a40 636c 6963 6b2e 6f70 7469 6f6e  .).@click.option
+00011160: 280a 2020 2020 222d 542f 2d6e 5422 2c0a  (.    "-T/-nT",.
+00011170: 2020 2020 222d 2d74 6167 2f2d 2d6e 6f2d      "--tag/--no-
+00011180: 7461 6722 2c0a 2020 2020 6465 6661 756c  tag",.    defaul
+00011190: 743d 4661 6c73 652c 0a20 2020 2068 656c  t=False,.    hel
+000111a0: 703d 2249 6620 7061 7373 6564 2c20 7472  p="If passed, tr
+000111b0: 6561 7420 616c 6c20 6172 6775 6d65 6e74  eat all argument
+000111c0: 7320 6173 2074 6167 732c 2064 656c 6574  s as tags, delet
+000111d0: 696e 6720 6576 6572 7920 6f63 7572 7265  ing every ocurre
+000111e0: 6e63 6520 6f66 2065 6163 6820 7461 672e  nce of each tag.
+000111f0: 222c 0a29 0a64 6566 2072 656d 6f76 6528  ",.).def remove(
+00011200: 6172 6773 2c20 666f 7263 652c 2074 6167  args, force, tag
+00011210: 293a 0a20 2020 2022 2222 5265 6d6f 7665  ):.    """Remove
+00011220: 2065 6974 6865 7220 7461 6728 7329 206f   either tag(s) o
+00011230: 7220 736f 6e67 2873 2920 7061 7373 6564  r song(s) passed
+00011240: 2061 7320 4944 2873 292e 2222 220a 2020   as ID(s).""".  
+00011250: 2020 6966 206e 6f74 2074 6167 3a0a 2020    if not tag:.  
+00011260: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
+00011270: 2020 2020 2020 2073 6f6e 675f 6964 7320         song_ids 
+00011280: 3d20 7b69 6e74 2873 6f6e 675f 6964 2920  = {int(song_id) 
+00011290: 666f 7220 736f 6e67 5f69 6420 696e 2061  for song_id in a
+000112a0: 7267 737d 0a20 2020 2020 2020 2020 2020  rgs}.           
+000112b0: 2072 656d 6169 6e69 6e67 5f73 6f6e 675f   remaining_song_
+000112c0: 6964 7320 3d20 7b6e 2066 6f72 206e 2069  ids = {n for n i
+000112d0: 6e20 736f 6e67 5f69 6473 7d0a 2020 2020  n song_ids}.    
+000112e0: 2020 2020 6578 6365 7074 2056 616c 7565      except Value
+000112f0: 4572 726f 723a 0a20 2020 2020 2020 2020  Error:.         
+00011300: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
+00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011320: 2253 6f6e 6720 4944 7320 6d75 7374 2062  "Song IDs must b
+00011330: 6520 696e 7465 6765 7273 2e20 546f 2064  e integers. To d
+00011340: 656c 6574 6520 7461 6773 2c20 7061 7373  elete tags, pass
+00011350: 2074 6865 2027 2d54 2f2d 2d74 6167 2720   the '-T/--tag' 
+00011360: 666c 6167 2e22 2c0a 2020 2020 2020 2020  flag.",.        
+00011370: 2020 2020 2020 2020 6667 3d22 7265 6422          fg="red"
+00011380: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00011390: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000113a0: 726e 0a0a 2020 2020 2020 2020 6966 206e  rn..        if n
+000113b0: 6f74 2066 6f72 6365 3a0a 2020 2020 2020  ot force:.      
+000113c0: 2020 2020 2020 6368 6172 203d 2069 6e70        char = inp
+000113d0: 7574 280a 2020 2020 2020 2020 2020 2020  ut(.            
+000113e0: 2020 2020 6622 4172 6520 796f 7520 7375      f"Are you su
+000113f0: 7265 2079 6f75 2077 616e 7420 746f 2064  re you want to d
+00011400: 656c 6574 6520 7b6c 656e 2873 6f6e 675f  elete {len(song_
+00011410: 6964 7329 7d20 736f 6e67 2873 293f 205b  ids)} song(s)? [
+00011420: 792f 6e5d 2022 0a20 2020 2020 2020 2020  y/n] ".         
+00011430: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00011440: 2020 6966 2063 6861 722e 6c6f 7765 7228    if char.lower(
+00011450: 2920 213d 2022 7922 3a0a 2020 2020 2020  ) != "y":.      
+00011460: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00011470: 2244 6964 206e 6f74 2064 656c 6574 652e  "Did not delete.
+00011480: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00011490: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
+000114a0: 2020 2077 6974 6820 6f70 656e 2853 4f4e     with open(SON
+000114b0: 4753 5f49 4e46 4f5f 5041 5448 2c20 2272  GS_INFO_PATH, "r
+000114c0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+000114d0: 2d38 2229 2061 7320 736f 6e67 735f 6669  -8") as songs_fi
+000114e0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+000114f0: 6c69 6e65 7320 3d20 736f 6e67 735f 6669  lines = songs_fi
+00011500: 6c65 2e72 6561 6428 292e 7370 6c69 746c  le.read().splitl
+00011510: 696e 6573 2829 0a0a 2020 2020 2020 2020  ines()..        
+00011520: 2020 2020 746f 5f62 655f 6465 6c65 7465      to_be_delete
+00011530: 6420 3d20 5b5d 0a20 2020 2020 2020 2020  d = [].         
+00011540: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00011550: 6528 6c65 6e28 6c69 6e65 7329 293a 0a20  e(len(lines)):. 
+00011560: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00011570: 6574 6169 6c73 203d 206c 696e 6573 5b69  etails = lines[i
+00011580: 5d2e 7374 7269 7028 292e 7370 6c69 7428  ].strip().split(
+00011590: 227c 2229 0a20 2020 2020 2020 2020 2020  "|").           
+000115a0: 2020 2020 2073 6f6e 675f 6964 203d 2069       song_id = i
+000115b0: 6e74 2864 6574 6169 6c73 5b30 5d29 0a20  nt(details[0]). 
+000115c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000115d0: 6620 736f 6e67 5f69 6420 696e 2072 656d  f song_id in rem
+000115e0: 6169 6e69 6e67 5f73 6f6e 675f 6964 733a  aining_song_ids:
+000115f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011600: 2020 2020 2072 656d 6169 6e69 6e67 5f73       remaining_s
+00011610: 6f6e 675f 6964 732e 7265 6d6f 7665 2873  ong_ids.remove(s
+00011620: 6f6e 675f 6964 290a 2020 2020 2020 2020  ong_id).        
+00011630: 2020 2020 2020 2020 2020 2020 746f 5f62              to_b
+00011640: 655f 6465 6c65 7465 642e 6170 7065 6e64  e_deleted.append
+00011650: 2869 290a 0a20 2020 2020 2020 2020 2020  (i)..           
+00011660: 2020 2020 2020 2020 2073 6f6e 675f 6e61           song_na
+00011670: 6d65 203d 2064 6574 6169 6c73 5b31 5d0a  me = details[1].
+00011680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011690: 2020 2020 6f73 2e72 656d 6f76 6528 2020      os.remove(  
+000116a0: 2320 7265 6d6f 7665 2061 6374 7561 6c20  # remove actual 
+000116b0: 736f 6e67 0a20 2020 2020 2020 2020 2020  song.           
+000116c0: 2020 2020 2020 2020 2020 2020 206f 732e               os.
+000116d0: 7061 7468 2e6a 6f69 6e28 534f 4e47 535f  path.join(SONGS_
+000116e0: 4449 522c 2073 6f6e 675f 6e61 6d65 290a  DIR, song_name).
+000116f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011700: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+00011710: 2020 2020 2020 2020 2020 2063 6c69 636b             click
+00011720: 2e73 6563 686f 280a 2020 2020 2020 2020  .secho(.        
+00011730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011740: 6622 5265 6d6f 7665 6420 736f 6e67 2027  f"Removed song '
+00011750: 7b73 6f6e 675f 6e61 6d65 7d27 2077 6974  {song_name}' wit
+00011760: 6820 4944 207b 736f 6e67 5f69 647d 2e22  h ID {song_id}."
+00011770: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011780: 2020 2020 2020 2020 2020 6667 3d22 6772            fg="gr
+00011790: 6565 6e22 2c0a 2020 2020 2020 2020 2020  een",.          
+000117a0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000117b0: 2020 2020 2066 6f72 2069 2069 6e20 7265       for i in re
+000117c0: 7665 7273 6564 2874 6f5f 6265 5f64 656c  versed(to_be_del
+000117d0: 6574 6564 293a 0a20 2020 2020 2020 2020  eted):.         
+000117e0: 2020 2064 656c 206c 696e 6573 5b69 5d0a     del lines[i].
+000117f0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
+00011800: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
+00011810: 5448 2c20 2277 222c 2065 6e63 6f64 696e  TH, "w", encodin
+00011820: 673d 2275 7466 2d38 2229 2061 7320 736f  g="utf-8") as so
+00011830: 6e67 735f 6669 6c65 3a0a 2020 2020 2020  ngs_file:.      
+00011840: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
+00011850: 2e77 7269 7465 2822 5c6e 222e 6a6f 696e  .write("\n".join
+00011860: 286c 696e 6573 2929 0a0a 2020 2020 2020  (lines))..      
+00011870: 2020 666f 7220 7374 6174 735f 6669 6c65    for stats_file
+00011880: 2069 6e20 6f73 2e6c 6973 7464 6972 2853   in os.listdir(S
+00011890: 5441 5453 5f44 4952 293a 0a20 2020 2020  TATS_DIR):.     
+000118a0: 2020 2020 2020 2069 6620 6e6f 7420 7374         if not st
+000118b0: 6174 735f 6669 6c65 2e65 6e64 7377 6974  ats_file.endswit
+000118c0: 6828 222e 7478 7422 293a 0a20 2020 2020  h(".txt"):.     
+000118d0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+000118e0: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
+000118f0: 2073 7461 7473 5f70 6174 6820 3d20 6f73   stats_path = os
+00011900: 2e70 6174 682e 6a6f 696e 2853 5441 5453  .path.join(STATS
+00011910: 5f44 4952 2c20 7374 6174 735f 6669 6c65  _DIR, stats_file
+00011920: 290a 2020 2020 2020 2020 2020 2020 7769  ).            wi
+00011930: 7468 206f 7065 6e28 7374 6174 735f 7061  th open(stats_pa
+00011940: 7468 2c20 2272 222c 2065 6e63 6f64 696e  th, "r", encodin
+00011950: 673d 2275 7466 2d38 2229 2061 7320 7374  g="utf-8") as st
+00011960: 6174 735f 6669 6c65 3a0a 2020 2020 2020  ats_file:.      
+00011970: 2020 2020 2020 2020 2020 7374 6174 735f            stats_
+00011980: 6c69 6e65 7320 3d20 7374 6174 735f 6669  lines = stats_fi
+00011990: 6c65 2e72 6561 6428 292e 7370 6c69 746c  le.read().splitl
+000119a0: 696e 6573 2829 0a0a 2020 2020 2020 2020  ines()..        
+000119b0: 2020 2020 2020 2020 746f 5f62 655f 6465          to_be_de
+000119c0: 6c65 7465 6420 3d20 5b5d 0a20 2020 2020  leted = [].     
+000119d0: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
+000119e0: 2069 6e20 7261 6e67 6528 6c65 6e28 7374   in range(len(st
+000119f0: 6174 735f 6c69 6e65 7329 293a 0a20 2020  ats_lines)):.   
+00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a10: 2064 6574 6169 6c73 203d 2073 7461 7473   details = stats
+00011a20: 5f6c 696e 6573 5b69 5d2e 7374 7269 7028  _lines[i].strip(
+00011a30: 292e 7370 6c69 7428 227c 2229 0a20 2020  ).split("|").   
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a50: 2073 6f6e 675f 6964 203d 2069 6e74 2864   song_id = int(d
+00011a60: 6574 6169 6c73 5b30 5d29 0a20 2020 2020  etails[0]).     
+00011a70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011a80: 6620 736f 6e67 5f69 6420 696e 2073 6f6e  f song_id in son
+00011a90: 675f 6964 733a 0a20 2020 2020 2020 2020  g_ids:.         
+00011aa0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00011ab0: 6f5f 6265 5f64 656c 6574 6564 2e61 7070  o_be_deleted.app
+00011ac0: 656e 6428 6929 0a0a 2020 2020 2020 2020  end(i)..        
+00011ad0: 2020 2020 666f 7220 6920 696e 2072 6576      for i in rev
+00011ae0: 6572 7365 6428 746f 5f62 655f 6465 6c65  ersed(to_be_dele
+00011af0: 7465 6429 3a0a 2020 2020 2020 2020 2020  ted):.          
+00011b00: 2020 2020 2020 6465 6c20 7374 6174 735f        del stats_
+00011b10: 6c69 6e65 735b 695d 0a0a 2020 2020 2020  lines[i]..      
+00011b20: 2020 2020 2020 7769 7468 206f 7065 6e28        with open(
+00011b30: 7374 6174 735f 7061 7468 2c20 2277 222c  stats_path, "w",
+00011b40: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+00011b50: 2229 2061 7320 7374 6174 735f 6669 6c65  ") as stats_file
+00011b60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011b70: 2020 7374 6174 735f 6669 6c65 2e77 7269    stats_file.wri
+00011b80: 7465 2822 5c6e 222e 6a6f 696e 2873 7461  te("\n".join(sta
+00011b90: 7473 5f6c 696e 6573 2929 0a0a 2020 2020  ts_lines))..    
+00011ba0: 2020 2020 6966 2072 656d 6169 6e69 6e67      if remaining
+00011bb0: 5f73 6f6e 675f 6964 733a 0a20 2020 2020  _song_ids:.     
+00011bc0: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
+00011bd0: 686f 280a 2020 2020 2020 2020 2020 2020  ho(.            
+00011be0: 2020 2020 6622 436f 756c 6420 6e6f 7420      f"Could not 
+00011bf0: 6669 6e64 2074 6865 2066 6f6c 6c6f 7769  find the followi
+00011c00: 6e67 2073 6f6e 6720 4944 733a 207b 272c  ng song IDs: {',
+00011c10: 2027 2e6a 6f69 6e28 6d61 7028 7374 722c   '.join(map(str,
+00011c20: 2072 656d 6169 6e69 6e67 5f73 6f6e 675f   remaining_song_
+00011c30: 6964 7329 297d 2e22 2c0a 2020 2020 2020  ids))}.",.      
+00011c40: 2020 2020 2020 2020 2020 6667 3d22 7265            fg="re
+00011c50: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+00011c60: 290a 2020 2020 656c 7365 3a0a 2020 2020  ).    else:.    
+00011c70: 2020 2020 7461 6773 5f74 6f5f 7265 6d6f      tags_to_remo
+00011c80: 7665 203d 2073 6574 2861 7267 7329 0a20  ve = set(args). 
+00011c90: 2020 2020 2020 2069 6620 6e6f 7420 666f         if not fo
+00011ca0: 7263 653a 0a20 2020 2020 2020 2020 2020  rce:.           
+00011cb0: 2063 6861 7220 3d20 696e 7075 7428 0a20   char = input(. 
+00011cc0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00011cd0: 2241 7265 2079 6f75 2073 7572 6520 796f  "Are you sure yo
+00011ce0: 7520 7761 6e74 2074 6f20 6465 6c65 7465  u want to delete
+00011cf0: 207b 6c65 6e28 7461 6773 5f74 6f5f 7265   {len(tags_to_re
+00011d00: 6d6f 7665 297d 2074 6167 2873 293f 205b  move)} tag(s)? [
+00011d10: 792f 6e5d 2022 0a20 2020 2020 2020 2020  y/n] ".         
+00011d20: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00011d30: 2020 6966 2063 6861 722e 6c6f 7765 7228    if char.lower(
+00011d40: 2920 213d 2022 7922 3a0a 2020 2020 2020  ) != "y":.      
+00011d50: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00011d60: 2244 6964 206e 6f74 2064 656c 6574 652e  "Did not delete.
+00011d70: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00011d80: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
+00011d90: 2020 2077 6974 6820 6f70 656e 2853 4f4e     with open(SON
+00011da0: 4753 5f49 4e46 4f5f 5041 5448 2c20 2272  GS_INFO_PATH, "r
+00011db0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+00011dc0: 2d38 2229 2061 7320 736f 6e67 735f 6669  -8") as songs_fi
+00011dd0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00011de0: 6c69 6e65 7320 3d20 736f 6e67 735f 6669  lines = songs_fi
+00011df0: 6c65 2e72 6561 6428 292e 7370 6c69 746c  le.read().splitl
+00011e00: 696e 6573 2829 0a20 2020 2020 2020 2020  ines().         
+00011e10: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00011e20: 6528 6c65 6e28 6c69 6e65 7329 293a 0a20  e(len(lines)):. 
+00011e30: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00011e40: 6574 6169 6c73 203d 206c 696e 6573 5b69  etails = lines[i
+00011e50: 5d2e 7374 7269 7028 292e 7370 6c69 7428  ].strip().split(
+00011e60: 227c 2229 0a20 2020 2020 2020 2020 2020  "|").           
+00011e70: 2020 2020 2074 6167 7320 3d20 6465 7461       tags = deta
+00011e80: 696c 735b 325d 2e73 706c 6974 2822 2c22  ils[2].split(","
+00011e90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00011ea0: 2020 666f 7220 6a20 696e 2072 616e 6765    for j in range
+00011eb0: 286c 656e 2874 6167 7329 293a 0a20 2020  (len(tags)):.   
+00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ed0: 2069 6620 7461 6773 5b6a 5d20 696e 2074   if tags[j] in t
+00011ee0: 6167 735f 746f 5f72 656d 6f76 653a 0a20  ags_to_remove:. 
 00011ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f00: 736f 6e67 735f 6669 6c65 203d 206f 7065  songs_file = ope
-00011f10: 6e28 534f 4e47 535f 494e 464f 5f50 4154  n(SONGS_INFO_PAT
-00011f20: 482c 2022 7722 2c20 656e 636f 6469 6e67  H, "w", encoding
-00011f30: 3d22 7574 662d 3822 290a 2020 2020 2020  ="utf-8").      
-00011f40: 2020 2020 2020 2020 2020 736f 6e67 735f            songs_
-00011f50: 6669 6c65 2e77 7269 7465 2822 5c6e 222e  file.write("\n".
-00011f60: 6a6f 696e 286c 696e 6573 2929 0a0a 2020  join(lines))..  
-00011f70: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00011f80: 2e72 656e 616d 6528 0a20 2020 2020 2020  .rename(.       
-00011f90: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-00011fa0: 7061 7468 2e6a 6f69 6e28 534f 4e47 535f  path.join(SONGS_
-00011fb0: 4449 522c 206f 6c64 5f70 6174 6829 2c0a  DIR, old_path),.
-00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fd0: 2020 2020 6f73 2e70 6174 682e 6a6f 696e      os.path.join
-00011fe0: 2853 4f4e 4753 5f44 4952 2c20 6465 7461  (SONGS_DIR, deta
-00011ff0: 696c 735b 315d 292c 0a20 2020 2020 2020  ils[1]),.       
-00012000: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00012010: 2020 2020 2020 2020 2020 2020 2320 7265              # re
-00012020: 6e61 6d65 2063 6163 6865 6420 7669 7375  name cached visu
-00012030: 616c 697a 6174 696f 6e20 6672 6571 7565  alization freque
-00012040: 6e63 6965 730a 2020 2020 2020 2020 2020  ncies.          
-00012050: 2020 2020 2020 7669 735f 6361 6368 655f        vis_cache_
-00012060: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-00012070: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
-00012080: 2020 2020 2020 2020 2046 5245 515f 4341           FREQ_CA
-00012090: 4348 455f 4449 522c 206f 732e 7061 7468  CHE_DIR, os.path
-000120a0: 2e73 706c 6974 6578 7428 6f6c 645f 7061  .splitext(old_pa
-000120b0: 7468 295b 305d 202b 2022 2e6e 7079 220a  th)[0] + ".npy".
-000120c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000120d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000120e0: 2020 6966 206f 732e 7061 7468 2e65 7869    if os.path.exi
-000120f0: 7374 7328 7669 735f 6361 6368 655f 7061  sts(vis_cache_pa
-00012100: 7468 293a 0a20 2020 2020 2020 2020 2020  th):.           
-00012110: 2020 2020 2020 2020 206f 732e 7265 6e61           os.rena
-00012120: 6d65 280a 2020 2020 2020 2020 2020 2020  me(.            
-00012130: 2020 2020 2020 2020 2020 2020 7669 735f              vis_
-00012140: 6361 6368 655f 7061 7468 2c0a 2020 2020  cache_path,.    
-00012150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012160: 2020 2020 6f73 2e70 6174 682e 6a6f 696e      os.path.join
-00012170: 2846 5245 515f 4341 4348 455f 4449 522c  (FREQ_CACHE_DIR,
-00012180: 206e 6577 5f6e 616d 6520 2b20 222e 6e70   new_name + ".np
-00012190: 7922 292c 0a20 2020 2020 2020 2020 2020  y"),.           
-000121a0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-000121b0: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-000121c0: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
-000121d0: 2020 2020 2020 2020 2020 2020 2066 2252               f"R
-000121e0: 656e 616d 6564 2073 6f6e 6720 277b 6f6c  enamed song '{ol
-000121f0: 645f 7061 7468 7d27 2077 6974 6820 4944  d_path}' with ID
-00012200: 207b 6f72 6967 696e 616c 7d20 746f 2027   {original} to '
-00012210: 7b64 6574 6169 6c73 5b31 5d7d 272e 222c  {details[1]}'.",
-00012220: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012230: 2020 2020 2066 673d 2267 7265 656e 222c       fg="green",
-00012240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012250: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00012260: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
-00012270: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00012280: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-00012290: 6622 536f 6e67 2077 6974 6820 4944 207b  f"Song with ID {
-000122a0: 6f72 6967 696e 616c 7d20 6e6f 7420 666f  original} not fo
-000122b0: 756e 642e 222c 2066 673d 2272 6564 2229  und.", fg="red")
-000122c0: 0a20 2020 2020 2020 2020 2020 2073 6f6e  .            son
-000122d0: 6773 5f66 696c 652e 636c 6f73 6528 290a  gs_file.close().
-000122e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000122f0: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
-00012300: 286c 656e 286c 696e 6573 2929 3a0a 2020  (len(lines)):.  
-00012310: 2020 2020 2020 2020 2020 6465 7461 696c            detail
-00012320: 7320 3d20 6c69 6e65 735b 695d 2e73 7472  s = lines[i].str
-00012330: 6970 2829 2e73 706c 6974 2822 7c22 290a  ip().split("|").
-00012340: 2020 2020 2020 2020 2020 2020 7461 6773              tags
-00012350: 203d 2064 6574 6169 6c73 5b32 5d2e 7370   = details[2].sp
-00012360: 6c69 7428 222c 2229 0a20 2020 2020 2020  lit(",").       
-00012370: 2020 2020 2066 6f72 2074 2069 6e20 7261       for t in ra
-00012380: 6e67 6528 6c65 6e28 7461 6773 2929 3a0a  nge(len(tags)):.
-00012390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123a0: 6966 2074 6167 735b 745d 203d 3d20 6f72  if tags[t] == or
-000123b0: 6967 696e 616c 3a0a 2020 2020 2020 2020  iginal:.        
-000123c0: 2020 2020 2020 2020 2020 2020 7461 6773              tags
-000123d0: 5b74 5d20 3d20 6e65 775f 6e61 6d65 0a20  [t] = new_name. 
-000123e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000123f0: 2020 2064 6574 6169 6c73 5b32 5d20 3d20     details[2] = 
-00012400: 222c 222e 6a6f 696e 2874 6167 7329 0a0a  ",".join(tags)..
-00012410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012420: 2020 2020 6c69 6e65 735b 695d 203d 2022      lines[i] = "
-00012430: 7c22 2e6a 6f69 6e28 6465 7461 696c 7329  |".join(details)
-00012440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012450: 2020 2020 2062 7265 616b 0a0a 2020 2020       break..    
-00012460: 2020 2020 736f 6e67 735f 6669 6c65 2e63      songs_file.c
-00012470: 6c6f 7365 2829 0a20 2020 2020 2020 2073  lose().        s
-00012480: 6f6e 6773 5f66 696c 6520 3d20 6f70 656e  ongs_file = open
-00012490: 2853 4f4e 4753 5f49 4e46 4f5f 5041 5448  (SONGS_INFO_PATH
-000124a0: 2c20 2277 222c 2065 6e63 6f64 696e 673d  , "w", encoding=
-000124b0: 2275 7466 2d38 2229 0a20 2020 2020 2020  "utf-8").       
-000124c0: 2073 6f6e 6773 5f66 696c 652e 7772 6974   songs_file.writ
-000124d0: 6528 225c 6e22 2e6a 6f69 6e28 6c69 6e65  e("\n".join(line
-000124e0: 7329 290a 0a20 2020 2020 2020 2063 6c69  s))..        cli
-000124f0: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
-00012500: 2020 2020 2020 6622 5265 706c 6163 6564        f"Replaced
-00012510: 2061 6c6c 206f 6375 7272 656e 6365 7320   all ocurrences 
-00012520: 6f66 2074 6167 2027 7b6f 7269 6769 6e61  of tag '{origina
-00012530: 6c7d 2720 746f 2027 7b6e 6577 5f6e 616d  l}' to '{new_nam
-00012540: 657d 272e 222c 0a20 2020 2020 2020 2020  e}'.",.         
-00012550: 2020 2066 673d 2267 7265 656e 222c 0a20     fg="green",. 
-00012560: 2020 2020 2020 2029 0a0a 0a40 636c 692e         )...@cli.
-00012570: 636f 6d6d 616e 6428 290a 4063 6c69 636b  command().@click
-00012580: 2e61 7267 756d 656e 7428 2270 6872 6173  .argument("phras
-00012590: 6522 290a 4063 6c69 636b 2e6f 7074 696f  e").@click.optio
-000125a0: 6e28 0a20 2020 2022 2d54 2f2d 6e54 222c  n(.    "-T/-nT",
-000125b0: 0a20 2020 2022 2d2d 7461 672f 2d2d 6e6f  .    "--tag/--no
-000125c0: 2d74 6167 222c 0a20 2020 2022 7365 6172  -tag",.    "sear
-000125d0: 6368 696e 675f 666f 725f 7461 6773 222c  ching_for_tags",
-000125e0: 0a20 2020 2064 6566 6175 6c74 3d46 616c  .    default=Fal
-000125f0: 7365 2c0a 2020 2020 6865 6c70 3d22 5365  se,.    help="Se
-00012600: 6172 6368 6573 2066 6f72 206d 6174 6368  arches for match
-00012610: 696e 6720 7461 6773 2069 6e73 7465 6164  ing tags instead
-00012620: 206f 6620 736f 6e67 206e 616d 6573 2e22   of song names."
-00012630: 2c0a 290a 6465 6620 7365 6172 6368 2870  ,.).def search(p
-00012640: 6872 6173 652c 2073 6561 7263 6869 6e67  hrase, searching
-00012650: 5f66 6f72 5f74 6167 7329 3a0a 2020 2020  _for_tags):.    
-00012660: 2222 2253 6561 7263 6865 7320 666f 7220  """Searches for 
-00012670: 736f 6e67 7320 7468 6174 2063 6f6e 7461  songs that conta
-00012680: 696e 2050 4852 4153 452e 2041 6c6c 2073  in PHRASE. All s
-00012690: 6f6e 6773 2073 7461 7274 696e 6720 7769  ongs starting wi
-000126a0: 7468 2050 4852 4153 450a 2020 2020 7769  th PHRASE.    wi
-000126b0: 6c6c 2061 7070 6561 7220 6265 666f 7265  ll appear before
-000126c0: 2073 6f6e 6773 2063 6f6e 7461 696e 696e   songs containin
-000126d0: 6720 6275 7420 6e6f 7420 7374 6172 7469  g but not starti
-000126e0: 6e67 2077 6974 6820 5048 5241 5345 2e20  ng with PHRASE. 
-000126f0: 5468 6973 0a20 2020 2073 6561 7263 6820  This.    search 
-00012700: 6973 2063 6173 652d 696e 7365 6e73 6974  is case-insensit
-00012710: 6976 652e 0a0a 2020 2020 4966 2074 6865  ive...    If the
-00012720: 2027 2d54 2720 666c 6167 2069 7320 7061   '-T' flag is pa
-00012730: 7373 6564 2c20 7365 6172 6368 6573 2066  ssed, searches f
-00012740: 6f72 2074 6167 7320 696e 7374 6561 6420  or tags instead 
-00012750: 6f66 2073 6f6e 6720 6e61 6d65 732e 2222  of song names.""
-00012760: 220a 2020 2020 7068 7261 7365 203d 2070  ".    phrase = p
-00012770: 6872 6173 652e 6c6f 7765 7228 290a 2020  hrase.lower().  
-00012780: 2020 7769 7468 206f 7065 6e28 534f 4e47    with open(SONG
-00012790: 535f 494e 464f 5f50 4154 482c 2022 7222  S_INFO_PATH, "r"
-000127a0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-000127b0: 3822 2920 6173 2073 6f6e 6773 5f66 696c  8") as songs_fil
-000127c0: 653a 0a20 2020 2020 2020 2069 6620 6e6f  e:.        if no
-000127d0: 7420 7365 6172 6368 696e 675f 666f 725f  t searching_for_
-000127e0: 7461 6773 3a0a 2020 2020 2020 2020 2020  tags:.          
-000127f0: 2020 7265 7375 6c74 7320 3d20 5b5d 2c20    results = [], 
-00012800: 5b5d 2020 2320 7374 6172 7473 2c20 636f  []  # starts, co
-00012810: 6e74 6169 6e73 2062 7574 2064 6f65 7320  ntains but does 
-00012820: 6e6f 7420 7374 6172 740a 2020 2020 2020  not start.      
-00012830: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
-00012840: 6e20 736f 6e67 735f 6669 6c65 3a0a 2020  n songs_file:.  
-00012850: 2020 2020 2020 2020 2020 2020 2020 736f                so
-00012860: 6e67 5f69 642c 2073 6f6e 675f 6e61 6d65  ng_id, song_name
-00012870: 2c20 7461 6773 2c20 2a5f 203d 206c 696e  , tags, *_ = lin
-00012880: 652e 7374 7269 7028 292e 7370 6c69 7428  e.strip().split(
-00012890: 227c 2229 0a20 2020 2020 2020 2020 2020  "|").           
-000128a0: 2020 2020 2073 6f6e 675f 6964 203d 2069       song_id = i
-000128b0: 6e74 2873 6f6e 675f 6964 290a 2020 2020  nt(song_id).    
-000128c0: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-000128d0: 5f6e 616d 6520 3d20 736f 6e67 5f6e 616d  _name = song_nam
-000128e0: 652e 6c6f 7765 7228 290a 0a20 2020 2020  e.lower()..     
-000128f0: 2020 2020 2020 2020 2020 2069 6620 736f             if so
-00012900: 6e67 5f6e 616d 652e 7374 6172 7473 7769  ng_name.startswi
-00012910: 7468 2870 6872 6173 6529 3a0a 2020 2020  th(phrase):.    
-00012920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012930: 7265 7375 6c74 735b 305d 2e61 7070 656e  results[0].appen
-00012940: 6428 736f 6e67 5f69 6429 0a20 2020 2020  d(song_id).     
-00012950: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00012960: 7068 7261 7365 2069 6e20 736f 6e67 5f6e  phrase in song_n
-00012970: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
-00012980: 2020 2020 2020 2020 2072 6573 756c 7473           results
-00012990: 5b31 5d2e 6170 7065 6e64 2873 6f6e 675f  [1].append(song_
-000129a0: 6964 290a 0a20 2020 2020 2020 2020 2020  id)..           
-000129b0: 2069 6620 6e6f 7420 616e 7928 7265 7375   if not any(resu
-000129c0: 6c74 7329 3a0a 2020 2020 2020 2020 2020  lts):.          
-000129d0: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
-000129e0: 6f28 224e 6f20 7265 7375 6c74 7320 666f  o("No results fo
-000129f0: 756e 642e 222c 2066 673d 2272 6564 2229  und.", fg="red")
-00012a00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012a10: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-00012a20: 2020 2020 2073 6f6e 6773 5f66 696c 652e       songs_file.
-00012a30: 7365 656b 2830 290a 2020 2020 2020 2020  seek(0).        
-00012a40: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-00012a50: 736f 6e67 735f 6669 6c65 3a0a 2020 2020  songs_file:.    
-00012a60: 2020 2020 2020 2020 2020 2020 6465 7461              deta
-00012a70: 696c 7320 3d20 6c69 6e65 2e73 7472 6970  ils = line.strip
-00012a80: 2829 2e73 706c 6974 2822 7c22 290a 2020  ().split("|").  
-00012a90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00012aa0: 2069 6e74 2864 6574 6169 6c73 5b30 5d29   int(details[0])
-00012ab0: 2069 6e20 7265 7375 6c74 735b 305d 3a0a   in results[0]:.
-00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ad0: 2020 2020 7072 696e 745f 656e 7472 7928      print_entry(
-00012ae0: 6465 7461 696c 7329 0a0a 2020 2020 2020  details)..      
-00012af0: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
-00012b00: 2e73 6565 6b28 3029 0a20 2020 2020 2020  .seek(0).       
-00012b10: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
-00012b20: 2073 6f6e 6773 5f66 696c 653a 0a20 2020   songs_file:.   
-00012b30: 2020 2020 2020 2020 2020 2020 2064 6574               det
-00012b40: 6169 6c73 203d 206c 696e 652e 7374 7269  ails = line.stri
-00012b50: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
-00012b60: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012b70: 6620 696e 7428 6465 7461 696c 735b 305d  f int(details[0]
-00012b80: 2920 696e 2072 6573 756c 7473 5b31 5d3a  ) in results[1]:
-00012b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012ba0: 2020 2020 2070 7269 6e74 5f65 6e74 7279       print_entry
-00012bb0: 2864 6574 6169 6c73 290a 0a20 2020 2020  (details)..     
-00012bc0: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
-00012bd0: 686f 280a 2020 2020 2020 2020 2020 2020  ho(.            
-00012be0: 2020 2020 6622 466f 756e 6420 7b6c 656e      f"Found {len
-00012bf0: 2872 6573 756c 7473 5b30 5d29 202b 206c  (results[0]) + l
-00012c00: 656e 2872 6573 756c 7473 5b31 5d29 7d20  en(results[1])} 
-00012c10: 736f 6e67 2873 292e 222c 0a20 2020 2020  song(s).",.     
-00012c20: 2020 2020 2020 2020 2020 2066 673d 2267             fg="g
-00012c30: 7265 656e 222c 0a20 2020 2020 2020 2020  reen",.         
-00012c40: 2020 2029 0a20 2020 2020 2020 2065 6c73     ).        els
-00012c50: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
-00012c60: 6573 756c 7473 203d 2073 6574 2829 2c20  esults = set(), 
-00012c70: 7365 7428 2920 2023 2073 7461 7274 732c  set()  # starts,
-00012c80: 2063 6f6e 7461 696e 7320 6275 7420 646f   contains but do
-00012c90: 6573 206e 6f74 2073 7461 7274 0a20 2020  es not start.   
-00012ca0: 2020 2020 2020 2020 2066 6f72 206c 696e           for lin
-00012cb0: 6520 696e 2073 6f6e 6773 5f66 696c 653a  e in songs_file:
-00012cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012cd0: 2073 6f6e 675f 6964 2c20 736f 6e67 5f6e   song_id, song_n
-00012ce0: 616d 652c 2074 6167 732c 202a 5f20 3d20  ame, tags, *_ = 
-00012cf0: 6c69 6e65 2e73 7472 6970 2829 2e73 706c  line.strip().spl
-00012d00: 6974 2822 7c22 290a 2020 2020 2020 2020  it("|").        
-00012d10: 2020 2020 2020 2020 6966 2074 6167 733a          if tags:
-00012d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012d30: 2020 2020 2074 6167 7320 3d20 7461 6773       tags = tags
-00012d40: 2e73 706c 6974 2822 2c22 290a 0a20 2020  .split(",")..   
-00012d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d60: 2066 6f72 2074 6167 2069 6e20 7461 6773   for tag in tags
-00012d70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012d80: 2020 2020 2020 2020 2020 7461 675f 6c6f            tag_lo
-00012d90: 7765 7220 3d20 7461 672e 6c6f 7765 7228  wer = tag.lower(
-00012da0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00012db0: 2020 2020 2020 2020 2020 6966 2074 6167            if tag
-00012dc0: 5f6c 6f77 6572 2e73 7461 7274 7377 6974  _lower.startswit
-00012dd0: 6828 7068 7261 7365 293a 0a20 2020 2020  h(phrase):.     
-00012de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012df0: 2020 2020 2020 2072 6573 756c 7473 5b30         results[0
-00012e00: 5d2e 6164 6428 7461 6729 0a20 2020 2020  ].add(tag).     
-00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e20: 2020 2065 6c69 6620 7068 7261 7365 2069     elif phrase i
-00012e30: 6e20 7461 675f 6c6f 7765 723a 0a20 2020  n tag_lower:.   
-00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e50: 2020 2020 2020 2020 2072 6573 756c 7473           results
-00012e60: 5b31 5d2e 6164 6428 7461 6729 0a0a 2020  [1].add(tag)..  
-00012e70: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00012e80: 2061 6e79 2872 6573 756c 7473 293a 0a20   any(results):. 
-00012e90: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00012ea0: 6c69 636b 2e73 6563 686f 2822 4e6f 2072  lick.secho("No r
-00012eb0: 6573 756c 7473 2066 6f75 6e64 2e22 2c20  esults found.", 
-00012ec0: 6667 3d22 7265 6422 290a 2020 2020 2020  fg="red").      
-00012ed0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00012ee0: 0a0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00012ef0: 7220 7461 6720 696e 2072 6573 756c 7473  r tag in results
-00012f00: 5b30 5d3a 0a20 2020 2020 2020 2020 2020  [0]:.           
-00012f10: 2020 2020 2070 7269 6e74 2874 6167 290a       print(tag).
-00012f20: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00012f30: 2074 6167 2069 6e20 7265 7375 6c74 735b   tag in results[
-00012f40: 315d 3a0a 2020 2020 2020 2020 2020 2020  1]:.            
-00012f50: 2020 2020 7072 696e 7428 7461 6729 0a0a      print(tag)..
-00012f60: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-00012f70: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
-00012f80: 2020 2020 2020 2020 2066 2246 6f75 6e64           f"Found
-00012f90: 207b 6c65 6e28 7265 7375 6c74 735b 305d   {len(results[0]
-00012fa0: 2920 2b20 6c65 6e28 7265 7375 6c74 735b  ) + len(results[
-00012fb0: 315d 297d 2074 6167 2873 292e 222c 2066  1])} tag(s).", f
-00012fc0: 673d 2267 7265 656e 220a 2020 2020 2020  g="green".      
-00012fd0: 2020 2020 2020 290a 0a0a 4063 6c69 2e63        )...@cli.c
-00012fe0: 6f6d 6d61 6e64 286e 616d 653d 226c 6973  ommand(name="lis
-00012ff0: 7422 290a 4063 6c69 636b 2e61 7267 756d  t").@click.argum
-00013000: 656e 7428 2273 6561 7263 685f 7461 6773  ent("search_tags
-00013010: 222c 206d 6574 6176 6172 3d22 5441 4753  ", metavar="TAGS
-00013020: 222c 206e 6172 6773 3d2d 3129 0a40 636c  ", nargs=-1).@cl
-00013030: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
-00013040: 222d 7322 2c0a 2020 2020 222d 2d73 6f72  "-s",.    "--sor
-00013050: 7422 2c0a 2020 2020 2273 6f72 745f 222c  t",.    "sort_",
-00013060: 0a20 2020 2074 7970 653d 636c 6963 6b2e  .    type=click.
-00013070: 4368 6f69 6365 280a 2020 2020 2020 2020  Choice(.        
-00013080: 280a 2020 2020 2020 2020 2020 2020 226e  (.            "n
-00013090: 6f6e 6522 2c0a 2020 2020 2020 2020 2020  one",.          
-000130a0: 2020 226e 616d 6522 2c0a 2020 2020 2020    "name",.      
-000130b0: 2020 2020 2020 226e 222c 0a20 2020 2020        "n",.     
-000130c0: 2020 2020 2020 2022 7365 6373 2d6c 6973         "secs-lis
-000130d0: 7465 6e65 6422 2c0a 2020 2020 2020 2020  tened",.        
-000130e0: 2020 2020 2273 222c 0a20 2020 2020 2020      "s",.       
-000130f0: 2020 2020 2022 6475 7261 7469 6f6e 222c       "duration",
-00013100: 0a20 2020 2020 2020 2020 2020 2022 6422  .            "d"
-00013110: 2c0a 2020 2020 2020 2020 2020 2020 2274  ,.            "t
-00013120: 696d 6573 2d6c 6973 7465 6e65 6422 2c0a  imes-listened",.
-00013130: 2020 2020 2020 2020 2020 2020 2274 222c              "t",
-00013140: 0a20 2020 2020 2020 2029 0a20 2020 2029  .        ).    )
-00013150: 2c0a 2020 2020 6865 6c70 3d22 536f 7274  ,.    help="Sort
-00013160: 2062 7920 6e61 6d65 2c20 7365 636f 6e64   by name, second
-00013170: 7320 6c69 7374 656e 6564 2c20 6f72 2074  s listened, or t
-00013180: 696d 6573 206c 6973 7465 6e65 6420 2873  imes listened (s
-00013190: 6563 6f6e 6473 2f73 6f6e 6720 6475 7261  econds/song dura
-000131a0: 7469 6f6e 292e 2047 7265 6174 6573 7420  tion). Greatest 
-000131b0: 6669 7273 742e 222c 0a20 2020 2064 6566  first.",.    def
-000131c0: 6175 6c74 3d22 6e6f 6e65 222c 0a20 2020  ault="none",.   
-000131d0: 2073 686f 775f 6465 6661 756c 743d 5472   show_default=Tr
-000131e0: 7565 2c0a 290a 4063 6c69 636b 2e6f 7074  ue,.).@click.opt
-000131f0: 696f 6e28 0a20 2020 2022 2d52 2f2d 6e52  ion(.    "-R/-nR
-00013200: 222c 0a20 2020 2022 2d2d 7265 7665 7273  ",.    "--revers
-00013210: 652f 2d2d 6e6f 2d72 6576 6572 7365 222c  e/--no-reverse",
-00013220: 0a20 2020 2022 7265 7665 7273 655f 222c  .    "reverse_",
-00013230: 0a20 2020 2064 6566 6175 6c74 3d46 616c  .    default=Fal
-00013240: 7365 2c0a 2020 2020 6865 6c70 3d22 5265  se,.    help="Re
-00013250: 7665 7273 6520 7468 6520 736f 7274 696e  verse the sortin
-00013260: 6720 6f72 6465 7220 2867 7265 6174 6573  g order (greates
-00013270: 7420 6669 7273 7429 2e22 2c0a 290a 4063  t first).",.).@c
-00013280: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
-00013290: 2022 2d54 2f2d 6e54 222c 0a20 2020 2022   "-T/-nT",.    "
-000132a0: 2d2d 7461 672f 2d2d 6e6f 2d74 6167 222c  --tag/--no-tag",
-000132b0: 0a20 2020 2022 6c69 7374 696e 675f 7461  .    "listing_ta
-000132c0: 6773 222c 0a20 2020 2064 6566 6175 6c74  gs",.    default
-000132d0: 3d46 616c 7365 2c0a 2020 2020 6865 6c70  =False,.    help
-000132e0: 3d22 4c69 7374 2074 6167 7320 6d61 7463  ="List tags matc
-000132f0: 6869 6e67 2054 4147 5320 696e 7374 6561  hing TAGS instea
-00013300: 6420 6f66 2073 6f6e 6773 2e22 2c0a 290a  d of songs.",.).
-00013310: 4063 6c69 636b 2e6f 7074 696f 6e28 0a20  @click.option(. 
-00013320: 2020 2022 2d79 222c 0a20 2020 2022 2d2d     "-y",.    "--
-00013330: 7965 6172 222c 0a20 2020 2022 7965 6172  year",.    "year
-00013340: 222c 0a20 2020 2068 656c 703d 2253 686f  ",.    help="Sho
-00013350: 7720 7469 6d65 206c 6973 7465 6e65 6420  w time listened 
-00013360: 666f 7220 6120 7370 6563 6966 6963 2079  for a specific y
-00013370: 6561 722c 2069 6e73 7465 6164 206f 6620  ear, instead of 
-00013380: 7468 6520 746f 7461 6c2e 2050 6173 7369  the total. Passi
-00013390: 6e67 2027 6375 7227 2077 696c 6c20 7368  ng 'cur' will sh
-000133a0: 6f77 2074 6865 2074 696d 6520 6c69 7374  ow the time list
-000133b0: 656e 6564 2066 6f72 2074 6865 2063 7572  ened for the cur
-000133c0: 7265 6e74 2079 6561 722e 222c 0a29 0a40  rent year.",.).@
-000133d0: 636c 6963 6b2e 6f70 7469 6f6e 2822 2d74  click.option("-t
-000133e0: 222c 2022 2d2d 746f 7022 2c20 2274 6f70  ", "--top", "top
-000133f0: 222c 2074 7970 653d 696e 742c 2068 656c  ", type=int, hel
-00013400: 703d 2253 686f 7720 7468 6520 746f 7020  p="Show the top 
-00013410: 6e20 736f 6e67 732f 7461 6773 2e22 290a  n songs/tags.").
-00013420: 4063 6c69 636b 2e6f 7074 696f 6e28 0a20  @click.option(. 
-00013430: 2020 2022 2d4d 2f2d 6e4d 222c 0a20 2020     "-M/-nM",.   
-00013440: 2022 2d2d 6d61 7463 682d 616c 6c2f 2d2d   "--match-all/--
-00013450: 6e6f 2d6d 6174 6368 2d61 6c6c 222c 0a20  no-match-all",. 
-00013460: 2020 2022 6d61 7463 685f 616c 6c22 2c0a     "match_all",.
-00013470: 2020 2020 6465 6661 756c 743d 4661 6c73      default=Fals
-00013480: 652c 0a20 2020 2068 656c 703d 2253 686f  e,.    help="Sho
-00013490: 7773 2073 6f6e 6773 2074 6861 7420 6d61  ws songs that ma
-000134a0: 7463 6820 616c 6c20 7461 6773 2069 6e73  tch all tags ins
-000134b0: 7465 6164 206f 6620 616e 7920 7461 672e  tead of any tag.
-000134c0: 2049 676e 6f72 6564 2069 6620 272d 742f   Ignored if '-t/
-000134d0: 2d2d 7461 6727 2069 7320 7061 7373 6564  --tag' is passed
-000134e0: 2e22 2c0a 290a 6465 6620 6c69 7374 5f28  .",.).def list_(
-000134f0: 7365 6172 6368 5f74 6167 732c 206c 6973  search_tags, lis
-00013500: 7469 6e67 5f74 6167 732c 2079 6561 722c  ting_tags, year,
-00013510: 2073 6f72 745f 2c20 746f 702c 2072 6576   sort_, top, rev
-00013520: 6572 7365 5f2c 206d 6174 6368 5f61 6c6c  erse_, match_all
-00013530: 293a 0a20 2020 2022 2222 4c69 7374 2074  ):.    """List t
-00013540: 6865 2065 6e74 7269 6573 2066 6f72 2061  he entries for a
-00013550: 6c6c 2073 6f6e 6773 2e0a 0a20 2020 204f  ll songs...    O
-00013560: 7574 7075 7420 666f 726d 6174 3a20 4944  utput format: ID
-00013570: 2c20 6e61 6d65 2c20 6475 7261 7469 6f6e  , name, duration
-00013580: 2c20 6c69 7374 656e 2074 696d 652c 2074  , listen time, t
-00013590: 696d 6573 206c 6973 7465 6e65 642c 205b  imes listened, [
-000135a0: 636c 6970 2d73 7461 7274 2c20 636c 6970  clip-start, clip
-000135b0: 2d65 6e64 5d20 6966 2063 6c69 7020 6578  -end] if clip ex
-000135c0: 6973 7473 2c20 636f 6d6d 612d 7365 7061  ists, comma-sepa
-000135d0: 7261 7465 6420 7461 6773 2069 6620 616e  rated tags if an
-000135e0: 790a 0a20 2020 2049 6620 7468 6520 272d  y..    If the '-
-000135f0: 5427 2066 6c61 6720 6973 2070 6173 7365  T' flag is passe
-00013600: 642c 2074 6167 7320 7769 6c6c 2062 6520  d, tags will be 
-00013610: 6c69 7374 6564 2069 6e73 7465 6164 206f  listed instead o
-00013620: 6620 736f 6e67 732e 0a0a 2020 2020 4f75  f songs...    Ou
-00013630: 7470 7574 2066 6f72 6d61 743a 2074 6167  tput format: tag
-00013640: 2c20 6475 7261 7469 6f6e 2c20 6c69 7374  , duration, list
-00013650: 656e 2074 696d 652c 2074 696d 6573 206c  en time, times l
-00013660: 6973 7465 6e65 640a 0a20 2020 2049 6620  istened..    If 
-00013670: 5441 4753 2061 7265 2070 6173 7365 642c  TAGS are passed,
-00013680: 2061 6e79 2074 6167 2f73 6f6e 6720 6d61   any tag/song ma
-00013690: 7463 6869 6e67 2061 6e79 2074 6167 2069  tching any tag i
-000136a0: 6e20 5441 4753 2077 696c 6c20 6265 206c  n TAGS will be l
-000136b0: 6973 7465 642c 0a20 2020 2075 6e6c 6573  isted,.    unles
-000136c0: 7320 7468 6520 272d 4d2f 2d2d 6d61 7463  s the '-M/--matc
-000136d0: 682d 616c 6c27 2066 6c61 6720 6973 2070  h-all' flag is p
-000136e0: 6173 7365 642c 2069 6e20 7768 6963 6820  assed, in which 
-000136f0: 6361 7365 2065 7665 7279 2074 6167 206d  case every tag m
-00013700: 7573 740a 2020 2020 6265 206d 6174 6368  ust.    be match
-00013710: 6564 2028 6967 6e6f 7265 6420 6966 206c  ed (ignored if l
-00013720: 6973 7469 6e67 2074 6167 7329 2e0a 2020  isting tags)..  
-00013730: 2020 2222 220a 2020 2020 6966 2074 6f70    """.    if top
-00013740: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00013750: 2020 2020 2020 6966 2074 6f70 203c 2031        if top < 1
-00013760: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
-00013770: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
-00013780: 2020 2020 2020 2020 2020 2022 5468 6520             "The 
-00013790: 6f70 7469 6f6e 2027 2d74 2f2d 2d74 6f70  option '-t/--top
-000137a0: 2720 6d75 7374 2062 6520 6120 706f 7369  ' must be a posi
-000137b0: 7469 7665 206e 756d 6265 722e 222c 2066  tive number.", f
-000137c0: 673d 2272 6564 220a 2020 2020 2020 2020  g="red".        
-000137d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000137e0: 2020 7265 7475 726e 0a0a 2020 2020 6966    return..    if
-000137f0: 2079 6561 7220 6973 204e 6f6e 653a 0a20   year is None:. 
-00013800: 2020 2020 2020 2073 7461 7473 5f70 6174         stats_pat
-00013810: 6820 3d20 544f 5441 4c5f 5354 4154 535f  h = TOTAL_STATS_
-00013820: 5041 5448 0a20 2020 2065 6c73 653a 0a20  PATH.    else:. 
-00013830: 2020 2020 2020 2069 6620 7965 6172 203d         if year =
-00013840: 3d20 2263 7572 223a 0a20 2020 2020 2020  = "cur":.       
-00013850: 2020 2020 2079 6561 7220 3d20 4355 525f       year = CUR_
-00013860: 5945 4152 0a20 2020 2020 2020 2020 2020  YEAR.           
-00013870: 2073 7461 7473 5f70 6174 6820 3d20 4355   stats_path = CU
-00013880: 525f 5945 4152 5f53 5441 5453 5f50 4154  R_YEAR_STATS_PAT
-00013890: 480a 2020 2020 2020 2020 656c 7365 3a0a  H.        else:.
-000138a0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-000138b0: 6f74 2079 6561 722e 6973 6469 6769 7428  ot year.isdigit(
-000138c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000138d0: 2020 2063 6c69 636b 2e73 6563 686f 2822     click.secho("
-000138e0: 5965 6172 206d 7573 7420 6265 2061 206e  Year must be a n
-000138f0: 756d 6265 7220 6f72 2027 6375 7227 2e22  umber or 'cur'."
-00013900: 2c20 6667 3d22 7265 6422 290a 2020 2020  , fg="red").    
-00013910: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00013920: 726e 0a20 2020 2020 2020 2020 2020 2073  rn.            s
-00013930: 7461 7473 5f70 6174 6820 3d20 6f73 2e70  tats_path = os.p
-00013940: 6174 682e 6a6f 696e 2853 5441 5453 5f44  ath.join(STATS_D
-00013950: 4952 2c20 6622 7b79 6561 727d 2e74 7874  IR, f"{year}.txt
-00013960: 2229 0a20 2020 2020 2020 2020 2020 2069  ").            i
-00013970: 6620 6e6f 7420 6f73 2e70 6174 682e 6578  f not os.path.ex
-00013980: 6973 7473 2873 7461 7473 5f70 6174 6829  ists(stats_path)
-00013990: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000139a0: 2020 636c 6963 6b2e 7365 6368 6f28 6622    click.secho(f"
-000139b0: 4e6f 2073 7461 7473 2066 6f75 6e64 2066  No stats found f
-000139c0: 6f72 2079 6561 7220 7b79 6561 727d 2e22  or year {year}."
-000139d0: 2c20 6667 3d22 7265 6422 290a 2020 2020  , fg="red").    
-000139e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000139f0: 726e 0a0a 2020 2020 6966 2073 6561 7263  rn..    if searc
-00013a00: 685f 7461 6773 3a0a 2020 2020 2020 2020  h_tags:.        
-00013a10: 7365 6172 6368 5f74 6167 7320 3d20 7365  search_tags = se
-00013a20: 7428 7365 6172 6368 5f74 6167 7329 0a0a  t(search_tags)..
-00013a30: 2020 2020 6e75 6d5f 6c69 6e65 7320 3d20      num_lines = 
-00013a40: 300a 0a20 2020 2069 6620 6c69 7374 696e  0..    if listin
-00013a50: 675f 7461 6773 3a0a 2020 2020 2020 2020  g_tags:.        
-00013a60: 7769 7468 2028 0a20 2020 2020 2020 2020  with (.         
-00013a70: 2020 206f 7065 6e28 534f 4e47 535f 494e     open(SONGS_IN
-00013a80: 464f 5f50 4154 482c 2022 7222 2c20 656e  FO_PATH, "r", en
-00013a90: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-00013aa0: 6173 2073 6f6e 6773 5f66 696c 652c 0a20  as songs_file,. 
-00013ab0: 2020 2020 2020 2020 2020 206f 7065 6e28             open(
-00013ac0: 7374 6174 735f 7061 7468 2c20 2272 222c  stats_path, "r",
-00013ad0: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
-00013ae0: 2229 2061 7320 7374 6174 735f 6669 6c65  ") as stats_file
-00013af0: 2c0a 2020 2020 2020 2020 293a 0a20 2020  ,.        ):.   
-00013b00: 2020 2020 2020 2020 2074 6167 7320 3d20           tags = 
-00013b10: 6465 6661 756c 7464 6963 7428 6c61 6d62  defaultdict(lamb
-00013b20: 6461 3a20 2830 2e30 2c20 302e 3029 290a  da: (0.0, 0.0)).
-00013b30: 0a20 2020 2020 2020 2020 2020 2073 6f6e  .            son
-00013b40: 6773 5f6c 696e 6573 203d 2073 6f6e 6773  gs_lines = songs
-00013b50: 5f66 696c 652e 7265 6164 6c69 6e65 7328  _file.readlines(
-00013b60: 290a 2020 2020 2020 2020 2020 2020 7374  ).            st
-00013b70: 6174 735f 6c69 6e65 7320 3d20 7374 6174  ats_lines = stat
-00013b80: 735f 6669 6c65 2e72 6561 646c 696e 6573  s_file.readlines
-00013b90: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
-00013ba0: 7374 6174 7320 3d20 6469 6374 280a 2020  stats = dict(.  
-00013bb0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-00013bc0: 7028 0a20 2020 2020 2020 2020 2020 2020  p(.             
-00013bd0: 2020 2020 2020 206c 616d 6264 6120 783a         lambda x:
-00013be0: 2074 7570 6c65 286d 6170 2866 6c6f 6174   tuple(map(float
-00013bf0: 2c20 782e 7374 7269 7028 292e 7370 6c69  , x.strip().spli
-00013c00: 7428 227c 2229 2929 2c0a 2020 2020 2020  t("|"))),.      
-00013c10: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00013c20: 6174 735f 6c69 6e65 732c 0a20 2020 2020  ats_lines,.     
-00013c30: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00013c40: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00013c50: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00013c60: 2072 616e 6765 286c 656e 2873 6f6e 6773   range(len(songs
-00013c70: 5f6c 696e 6573 2929 3a0a 2020 2020 2020  _lines)):.      
-00013c80: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
-00013c90: 642c 2073 6f6e 675f 6e61 6d65 2c20 7461  d, song_name, ta
-00013ca0: 675f 7374 7269 6e67 203d 2028 0a20 2020  g_string = (.   
-00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cc0: 2073 6f6e 6773 5f6c 696e 6573 5b69 5d2e   songs_lines[i].
-00013cd0: 7374 7269 7028 292e 7370 6c69 7428 227c  strip().split("|
-00013ce0: 2229 5b30 3a33 5d0a 2020 2020 2020 2020  ")[0:3].        
-00013cf0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00013d00: 2020 2020 2020 2020 2020 6966 2074 6167            if tag
-00013d10: 5f73 7472 696e 673a 0a20 2020 2020 2020  _string:.       
-00013d20: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00013d30: 2074 6167 2069 6e20 7461 675f 7374 7269   tag in tag_stri
-00013d40: 6e67 2e73 706c 6974 2822 2c22 293a 0a20  ng.split(","):. 
-00013d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d60: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00013d70: 6172 6368 5f74 6167 7320 6f72 2074 6167  arch_tags or tag
-00013d80: 2069 6e20 7365 6172 6368 5f74 6167 733a   in search_tags:
-00013d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013da0: 2020 2020 2020 2020 2020 2020 2074 6167               tag
-00013db0: 735b 7461 675d 203d 2028 0a20 2020 2020  s[tag] = (.     
-00013dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013dd0: 2020 2020 2020 2020 2020 2074 6167 735b             tags[
-00013de0: 7461 675d 5b30 5d20 2b20 7374 6174 735f  tag][0] + stats_
-00013df0: 6c69 6e65 735b 666c 6f61 7428 736f 6e67  lines[float(song
-00013e00: 5f69 6429 5d2c 0a20 2020 2020 2020 2020  _id)],.         
-00013e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e20: 2020 2020 2020 2074 6167 735b 7461 675d         tags[tag]
-00013e30: 5b31 5d0a 2020 2020 2020 2020 2020 2020  [1].            
-00013e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e50: 2020 2020 2b20 6d75 7369 635f 7461 672e      + music_tag.
-00013e60: 6c6f 6164 5f66 696c 6528 0a20 2020 2020  load_file(.     
-00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e80: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00013e90: 732e 7061 7468 2e6a 6f69 6e28 534f 4e47  s.path.join(SONG
-00013ea0: 535f 4449 522c 2073 6f6e 675f 6e61 6d65  S_DIR, song_name
-00013eb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00013ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ed0: 2020 295b 2223 6c65 6e67 7468 225d 2e76    )["#length"].v
-00013ee0: 616c 7565 2c0a 2020 2020 2020 2020 2020  alue,.          
-00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f00: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-00013f10: 2066 6f72 2074 6167 2c20 286c 6973 7465   for tag, (liste
-00013f20: 6e5f 7469 6d65 2c20 746f 7461 6c5f 6475  n_time, total_du
-00013f30: 7261 7469 6f6e 2920 696e 2074 6167 732e  ration) in tags.
-00013f40: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-00013f50: 2020 2020 2020 2020 2063 6c69 636b 2e65           click.e
-00013f60: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
-00013f70: 2020 2020 2020 2020 2066 227b 7461 677d           f"{tag}
-00013f80: 207b 636c 6963 6b2e 7374 796c 6528 666f   {click.style(fo
-00013f90: 726d 6174 5f73 6563 6f6e 6473 2874 6f74  rmat_seconds(tot
-00013fa0: 616c 5f64 7572 6174 696f 6e2c 2073 686f  al_duration, sho
-00013fb0: 775f 6465 6369 6d61 6c3d 5472 7565 292c  w_decimal=True),
-00013fc0: 2066 673d 2762 7269 6768 745f 626c 6163   fg='bright_blac
-00013fd0: 6b27 297d 207b 636c 6963 6b2e 7374 796c  k')} {click.styl
-00013fe0: 6528 666f 726d 6174 5f73 6563 6f6e 6473  e(format_seconds
-00013ff0: 286c 6973 7465 6e5f 7469 6d65 2c20 7368  (listen_time, sh
-00014000: 6f77 5f64 6563 696d 616c 3d54 7275 6529  ow_decimal=True)
-00014010: 2c20 6667 3d27 7965 6c6c 6f77 2729 7d20  , fg='yellow')} 
-00014020: 7b63 6c69 636b 2e73 7479 6c65 2827 252e  {click.style('%.
-00014030: 3266 2725 286c 6973 7465 6e5f 7469 6d65  2f'%(listen_time
-00014040: 2f74 6f74 616c 5f64 7572 6174 696f 6e29  /total_duration)
-00014050: 2c20 6667 3d27 6272 6967 6874 5f62 6c61  , fg='bright_bla
-00014060: 636b 2729 7d22 0a20 2020 2020 2020 2020  ck')}".         
-00014070: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00014080: 2020 2020 2020 2020 206e 756d 5f6c 696e           num_lin
-00014090: 6573 202b 3d20 310a 2020 2020 2020 2020  es += 1.        
-000140a0: 2020 2020 2020 2020 6966 2074 6f70 2069          if top i
-000140b0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206e  s not None and n
-000140c0: 756d 5f6c 696e 6573 203d 3d20 746f 703a  um_lines == top:
-000140d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000140e0: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
-000140f0: 2020 2072 6574 7572 6e0a 0a20 2020 206e     return..    n
-00014100: 6f5f 7265 7375 6c74 7320 3d20 5472 7565  o_results = True
-00014110: 0a20 2020 2077 6974 6820 280a 2020 2020  .    with (.    
-00014120: 2020 2020 6f70 656e 2853 4f4e 4753 5f49      open(SONGS_I
-00014130: 4e46 4f5f 5041 5448 2c20 2272 222c 2065  NFO_PATH, "r", e
-00014140: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
-00014150: 2061 7320 736f 6e67 735f 6669 6c65 2c0a   as songs_file,.
-00014160: 2020 2020 2020 2020 6f70 656e 2873 7461          open(sta
-00014170: 7473 5f70 6174 682c 2022 7222 2c20 656e  ts_path, "r", en
-00014180: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-00014190: 6173 2073 7461 7473 5f66 696c 652c 0a20  as stats_file,. 
-000141a0: 2020 2029 3a0a 2020 2020 2020 2020 6c69     ):.        li
-000141b0: 6e65 7320 3d20 736f 6e67 735f 6669 6c65  nes = songs_file
-000141c0: 2e72 6561 646c 696e 6573 2829 0a20 2020  .readlines().   
-000141d0: 2020 2020 2073 7461 7473 203d 2073 7461       stats = sta
-000141e0: 7473 5f66 696c 652e 7265 6164 6c69 6e65  ts_file.readline
-000141f0: 7328 290a 0a20 2020 2020 2020 2073 7461  s()..        sta
-00014200: 7473 203d 2064 6963 7428 0a20 2020 2020  ts = dict(.     
-00014210: 2020 2020 2020 206d 6170 286c 616d 6264         map(lambd
-00014220: 6120 783a 2074 7570 6c65 286d 6170 2866  a x: tuple(map(f
-00014230: 6c6f 6174 2c20 782e 7374 7269 7028 292e  loat, x.strip().
-00014240: 7370 6c69 7428 227c 2229 2929 2c20 7374  split("|"))), st
-00014250: 6174 7329 0a20 2020 2020 2020 2029 0a0a  ats).        )..
-00014260: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-00014270: 2072 616e 6765 286c 656e 286c 696e 6573   range(len(lines
-00014280: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
-00014290: 6465 7461 696c 7320 3d20 6c69 6e65 735b  details = lines[
-000142a0: 695d 2e73 7472 6970 2829 2e73 706c 6974  i].strip().split
-000142b0: 2822 7c22 290a 2020 2020 2020 2020 2020  ("|").          
-000142c0: 2020 736f 6e67 5f69 6420 3d20 696e 7428    song_id = int(
-000142d0: 6465 7461 696c 735b 305d 290a 0a20 2020  details[0])..   
-000142e0: 2020 2020 2020 2020 2074 6167 7320 3d20           tags = 
-000142f0: 7365 7428 6465 7461 696c 735b 325d 2e73  set(details[2].s
-00014300: 706c 6974 2822 2c22 2929 0a20 2020 2020  plit(",")).     
-00014310: 2020 2020 2020 2069 6620 7365 6172 6368         if search
-00014320: 5f74 6167 733a 0a20 2020 2020 2020 2020  _tags:.         
-00014330: 2020 2020 2020 2069 6620 6d61 7463 685f         if match_
-00014340: 616c 6c3a 0a20 2020 2020 2020 2020 2020  all:.           
-00014350: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-00014360: 7365 6172 6368 5f74 6167 7320 3c3d 2074  search_tags <= t
-00014370: 6167 733a 2020 2320 7375 6273 6574 0a20  ags:  # subset. 
-00014380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014390: 2020 2020 2020 206c 696e 6573 5b69 5d20         lines[i] 
-000143a0: 3d20 2222 0a20 2020 2020 2020 2020 2020  = "".           
-000143b0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000143c0: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
-000143d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000143e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143f0: 6966 206e 6f74 2073 6561 7263 685f 7461  if not search_ta
-00014400: 6773 2026 2074 6167 733a 2020 2320 696e  gs & tags:  # in
-00014410: 7465 7273 6563 7469 6f6e 0a20 2020 2020  tersection.     
-00014420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014430: 2020 206c 696e 6573 5b69 5d20 3d20 2222     lines[i] = ""
-00014440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014450: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00014460: 650a 0a20 2020 2020 2020 2020 2020 2074  e..            t
-00014470: 696d 655f 6c69 7374 656e 6564 203d 2073  ime_listened = s
-00014480: 7461 7473 5b66 6c6f 6174 2873 6f6e 675f  tats[float(song_
-00014490: 6964 295d 0a20 2020 2020 2020 2020 2020  id)].           
-000144a0: 206c 696e 6573 5b69 5d20 3d20 7475 706c   lines[i] = tupl
-000144b0: 6528 6465 7461 696c 7329 202b 2028 0a20  e(details) + (. 
-000144c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-000144d0: 696d 655f 6c69 7374 656e 6564 2c0a 2020  ime_listened,.  
-000144e0: 2020 2020 2020 2020 2020 2020 2020 6d75                mu
-000144f0: 7369 635f 7461 672e 6c6f 6164 5f66 696c  sic_tag.load_fil
-00014500: 6528 6f73 2e70 6174 682e 6a6f 696e 2853  e(os.path.join(S
-00014510: 4f4e 4753 5f44 4952 2c20 6465 7461 696c  ONGS_DIR, detail
-00014520: 735b 315d 2929 5b0a 2020 2020 2020 2020  s[1]))[.        
-00014530: 2020 2020 2020 2020 2020 2020 2223 6c65              "#le
-00014540: 6e67 7468 220a 2020 2020 2020 2020 2020  ngth".          
-00014550: 2020 2020 2020 5d2e 7661 6c75 652c 0a20        ].value,. 
-00014560: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00014570: 2020 2020 2020 6c69 6e65 7320 3d20 5b6c        lines = [l
-00014580: 696e 6520 666f 7220 6c69 6e65 2069 6e20  ine for line in 
-00014590: 6c69 6e65 7320 6966 206c 696e 655d 0a0a  lines if line]..
-000145a0: 2020 2020 2020 2020 6966 2073 6f72 745f          if sort_
-000145b0: 2021 3d20 226e 6f6e 6522 3a0a 2020 2020   != "none":.    
-000145c0: 2020 2020 2020 2020 6966 2073 6f72 745f          if sort_
-000145d0: 2069 6e20 2822 6e61 6d65 222c 2022 6e22   in ("name", "n"
-000145e0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000145f0: 2020 2073 6f72 745f 6b65 7920 3d20 6c61     sort_key = la
-00014600: 6d62 6461 2074 3a20 745b 315d 0a20 2020  mbda t: t[1].   
-00014610: 2020 2020 2020 2020 2065 6c69 6620 736f           elif so
-00014620: 7274 5f20 696e 2028 2273 6563 732d 6c69  rt_ in ("secs-li
-00014630: 7374 656e 6564 222c 2022 7322 293a 0a20  stened", "s"):. 
-00014640: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00014650: 6f72 745f 6b65 7920 3d20 6c61 6d62 6461  ort_key = lambda
-00014660: 2074 3a20 666c 6f61 7428 745b 2d32 5d29   t: float(t[-2])
-00014670: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00014680: 6620 736f 7274 5f20 696e 2028 2264 7572  f sort_ in ("dur
-00014690: 6174 696f 6e22 2c20 2264 2229 3a0a 2020  ation", "d"):.  
-000146a0: 2020 2020 2020 2020 2020 2020 2020 736f                so
-000146b0: 7274 5f6b 6579 203d 206c 616d 6264 6120  rt_key = lambda 
-000146c0: 743a 2066 6c6f 6174 2874 5b2d 315d 290a  t: float(t[-1]).
-000146d0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000146e0: 2073 6f72 745f 2069 6e20 2822 7469 6d65   sort_ in ("time
-000146f0: 732d 6c69 7374 656e 6564 222c 2022 7422  s-listened", "t"
-00014700: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00014710: 2020 2073 6f72 745f 6b65 7920 3d20 6c61     sort_key = la
-00014720: 6d62 6461 2074 3a20 666c 6f61 7428 745b  mbda t: float(t[
-00014730: 2d32 5d29 202f 2066 6c6f 6174 2874 5b2d  -2]) / float(t[-
-00014740: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-00014750: 6c69 6e65 732e 736f 7274 280a 2020 2020  lines.sort(.    
-00014760: 2020 2020 2020 2020 2020 2020 6b65 793d              key=
-00014770: 736f 7274 5f6b 6579 2c0a 2020 2020 2020  sort_key,.      
-00014780: 2020 2020 2020 2020 2020 7265 7665 7273            revers
-00014790: 653d 6e6f 7420 7265 7665 7273 655f 2c0a  e=not reverse_,.
-000147a0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000147b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000147c0: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-000147d0: 6576 6572 7365 5f3a 0a20 2020 2020 2020  everse_:.       
-000147e0: 2020 2020 2020 2020 206c 696e 6573 2e72           lines.r
-000147f0: 6576 6572 7365 2829 0a0a 2020 2020 2020  everse()..      
-00014800: 2020 666f 7220 6465 7461 696c 7320 696e    for details in
-00014810: 206c 696e 6573 3a0a 2020 2020 2020 2020   lines:.        
-00014820: 2020 2020 7072 696e 745f 656e 7472 7928      print_entry(
-00014830: 6465 7461 696c 7329 0a20 2020 2020 2020  details).       
-00014840: 2020 2020 206e 756d 5f6c 696e 6573 202b       num_lines +
-00014850: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-00014860: 6e6f 5f72 6573 756c 7473 203d 2046 616c  no_results = Fal
-00014870: 7365 0a20 2020 2020 2020 2020 2020 2069  se.            i
-00014880: 6620 746f 7020 6973 206e 6f74 204e 6f6e  f top is not Non
-00014890: 6520 616e 6420 6e75 6d5f 6c69 6e65 7320  e and num_lines 
-000148a0: 3d3d 2074 6f70 3a0a 2020 2020 2020 2020  == top:.        
-000148b0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
-000148c0: 2020 2069 6620 6e6f 5f72 6573 756c 7473     if no_results
-000148d0: 2061 6e64 2073 6561 7263 685f 7461 6773   and search_tags
-000148e0: 3a0a 2020 2020 2020 2020 636c 6963 6b2e  :.        click.
-000148f0: 7365 6368 6f28 224e 6f20 736f 6e67 7320  secho("No songs 
-00014900: 666f 756e 6420 6d61 7463 6869 6e67 2074  found matching t
-00014910: 6167 732e 222c 2066 673d 2272 6564 2229  ags.", fg="red")
-00014920: 0a20 2020 2065 6c69 6620 6e6f 5f72 6573  .    elif no_res
-00014930: 756c 7473 3a0a 2020 2020 2020 2020 636c  ults:.        cl
-00014940: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
-00014950: 2020 2020 2020 2022 4e6f 2073 6f6e 6773         "No songs
-00014960: 2066 6f75 6e64 2e20 5573 6520 276d 6165   found. Use 'mae
-00014970: 7374 726f 2061 6464 2720 746f 2061 6464  stro add' to add
-00014980: 2061 2073 6f6e 672e 222c 2066 673d 2272   a song.", fg="r
-00014990: 6564 220a 2020 2020 2020 2020 290a 0a0a  ed".        )...
-000149a0: 4063 6c69 2e63 6f6d 6d61 6e64 2829 0a40  @cli.command().@
-000149b0: 636c 6963 6b2e 6f70 7469 6f6e 280a 2020  click.option(.  
-000149c0: 2020 222d 7922 2c0a 2020 2020 222d 2d79    "-y",.    "--y
-000149d0: 6561 7222 2c0a 2020 2020 2279 6561 7222  ear",.    "year"
-000149e0: 2c0a 2020 2020 6865 6c70 3d22 5368 6f77  ,.    help="Show
-000149f0: 2074 696d 6520 6c69 7374 656e 6564 2066   time listened f
-00014a00: 6f72 2061 2073 7065 6369 6669 6320 7965  or a specific ye
-00014a10: 6172 2c20 696e 7374 6561 6420 6f66 2074  ar, instead of t
-00014a20: 6865 2074 6f74 616c 2e20 5061 7373 696e  he total. Passin
-00014a30: 6720 2763 7572 2720 7769 6c6c 2073 686f  g 'cur' will sho
-00014a40: 7720 7468 6520 7469 6d65 206c 6973 7465  w the time liste
-00014a50: 6e65 6420 666f 7220 7468 6520 6375 7272  ned for the curr
-00014a60: 656e 7420 7965 6172 2e22 2c0a 290a 4063  ent year.",.).@c
-00014a70: 6c69 636b 2e61 7267 756d 656e 7428 2273  lick.argument("s
-00014a80: 6f6e 675f 6964 7322 2c20 7479 7065 3d63  ong_ids", type=c
-00014a90: 6c69 636b 2e49 4e54 2c20 6e61 7267 733d  lick.INT, nargs=
-00014aa0: 2d31 2c20 7265 7175 6972 6564 3d54 7275  -1, required=Tru
-00014ab0: 6529 0a64 6566 2065 6e74 7279 2873 6f6e  e).def entry(son
-00014ac0: 675f 6964 732c 2079 6561 7229 3a0a 2020  g_ids, year):.  
-00014ad0: 2020 2222 2250 7269 6e74 7320 7468 6520    """Prints the 
-00014ae0: 6465 7461 696c 7320 6f66 2074 6865 2073  details of the s
-00014af0: 6f6e 6728 7329 2077 6974 6820 7468 6520  ong(s) with the 
-00014b00: 4944 2873 2920 534f 4e47 5f49 4453 2e0a  ID(s) SONG_IDS..
-00014b10: 0a20 2020 204f 7574 7075 7420 666f 726d  .    Output form
-00014b20: 6174 3a20 4944 2c20 6e61 6d65 2c20 6475  at: ID, name, du
-00014b30: 7261 7469 6f6e 2c20 6c69 7374 656e 2074  ration, listen t
-00014b40: 696d 652c 2074 696d 6573 206c 6973 7465  ime, times liste
-00014b50: 6e65 642c 205b 636c 6970 2d73 7461 7274  ned, [clip-start
-00014b60: 2c20 636c 6970 2d65 6e64 5d20 6966 2063  , clip-end] if c
-00014b70: 6c69 7020 6578 6973 7473 2c20 636f 6d6d  lip exists, comm
-00014b80: 612d 7365 7061 7261 7465 6420 7461 6773  a-separated tags
-00014b90: 2069 6620 616e 7922 2222 0a20 2020 2073   if any""".    s
-00014ba0: 6f6e 675f 6964 7320 3d20 7365 7428 736f  ong_ids = set(so
-00014bb0: 6e67 5f69 6473 290a 0a20 2020 2069 6620  ng_ids)..    if 
-00014bc0: 7965 6172 2069 7320 4e6f 6e65 3a0a 2020  year is None:.  
-00014bd0: 2020 2020 2020 7374 6174 735f 7061 7468        stats_path
-00014be0: 203d 2054 4f54 414c 5f53 5441 5453 5f50   = TOTAL_STATS_P
-00014bf0: 4154 480a 2020 2020 656c 7365 3a0a 2020  ATH.    else:.  
-00014c00: 2020 2020 2020 6966 2079 6561 7220 3d3d        if year ==
-00014c10: 2022 6375 7222 3a0a 2020 2020 2020 2020   "cur":.        
-00014c20: 2020 2020 7965 6172 203d 2043 5552 5f59      year = CUR_Y
-00014c30: 4541 520a 2020 2020 2020 2020 2020 2020  EAR.            
-00014c40: 7374 6174 735f 7061 7468 203d 2043 5552  stats_path = CUR
-00014c50: 5f59 4541 525f 5354 4154 535f 5041 5448  _YEAR_STATS_PATH
-00014c60: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00014c70: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00014c80: 7420 7965 6172 2e69 7364 6967 6974 2829  t year.isdigit()
-00014c90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014ca0: 2020 636c 6963 6b2e 7365 6368 6f28 2259    click.secho("Y
-00014cb0: 6561 7220 6d75 7374 2062 6520 6120 6e75  ear must be a nu
-00014cc0: 6d62 6572 2e22 2c20 6667 3d22 7265 6422  mber.", fg="red"
-00014cd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00014ce0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00014cf0: 2020 2020 2073 7461 7473 5f70 6174 6820       stats_path 
-00014d00: 3d20 6f73 2e70 6174 682e 6a6f 696e 2853  = os.path.join(S
-00014d10: 5441 5453 5f44 4952 2c20 6622 7b79 6561  TATS_DIR, f"{yea
-00014d20: 727d 2e74 7874 2229 0a0a 2020 2020 7472  r}.txt")..    tr
-00014d30: 793a 0a20 2020 2020 2020 2077 6974 6820  y:.        with 
-00014d40: 280a 2020 2020 2020 2020 2020 2020 6f70  (.            op
-00014d50: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
-00014d60: 5448 2c20 2272 222c 2065 6e63 6f64 696e  TH, "r", encodin
-00014d70: 673d 2275 7466 2d38 2229 2061 7320 736f  g="utf-8") as so
-00014d80: 6e67 735f 6669 6c65 2c0a 2020 2020 2020  ngs_file,.      
-00014d90: 2020 2020 2020 6f70 656e 2873 7461 7473        open(stats
-00014da0: 5f70 6174 682c 2022 7222 2c20 656e 636f  _path, "r", enco
-00014db0: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
-00014dc0: 2073 7461 7473 5f66 696c 652c 0a20 2020   stats_file,.   
-00014dd0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00014de0: 2020 2020 6c69 6e65 7320 3d20 736f 6e67      lines = song
-00014df0: 735f 6669 6c65 2e72 6561 646c 696e 6573  s_file.readlines
-00014e00: 2829 0a20 2020 2020 2020 2020 2020 2073  ().            s
-00014e10: 7461 7473 5f6c 696e 6573 203d 2073 7461  tats_lines = sta
-00014e20: 7473 5f66 696c 652e 7265 6164 6c69 6e65  ts_file.readline
-00014e30: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-00014e40: 7374 6174 735f 6c69 6e65 7320 3d20 6469  stats_lines = di
-00014e50: 6374 280a 2020 2020 2020 2020 2020 2020  ct(.            
-00014e60: 2020 2020 6d61 7028 0a20 2020 2020 2020      map(.       
-00014e70: 2020 2020 2020 2020 2020 2020 206c 616d               lam
-00014e80: 6264 6120 783a 2074 7570 6c65 286d 6170  bda x: tuple(map
-00014e90: 2866 6c6f 6174 2c20 782e 7374 7269 7028  (float, x.strip(
-00014ea0: 292e 7370 6c69 7428 227c 2229 2929 2c0a  ).split("|"))),.
-00014eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ec0: 2020 2020 7374 6174 735f 6c69 6e65 732c      stats_lines,
-00014ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ee0: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
-00014ef0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00014f00: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
-00014f10: 6c69 6e65 7329 293a 0a20 2020 2020 2020  lines)):.       
-00014f20: 2020 2020 2020 2020 2064 6574 6169 6c73           details
-00014f30: 203d 206c 696e 6573 5b69 5d2e 7374 7269   = lines[i].stri
-00014f40: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
-00014f50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014f60: 6620 696e 7428 6465 7461 696c 735b 305d  f int(details[0]
-00014f70: 2920 696e 2073 6f6e 675f 6964 733a 0a20  ) in song_ids:. 
-00014f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f90: 2020 2070 7269 6e74 5f65 6e74 7279 280a     print_entry(.
-00014fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fb0: 2020 2020 2020 2020 6465 7461 696c 730a          details.
-00014fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fd0: 2020 2020 2020 2020 2b20 7374 6174 735f          + stats_
-00014fe0: 6c69 6e65 735b 666c 6f61 7428 6465 7461  lines[float(deta
-00014ff0: 696c 735b 305d 295d 2e73 7472 6970 2829  ils[0])].strip()
-00015000: 2e73 706c 6974 2822 7c22 295b 313a 325d  .split("|")[1:2]
-00015010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015020: 2020 2020 2020 2020 202b 205b 0a20 2020           + [.   
-00015030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015040: 2020 2020 2020 2020 206d 7573 6963 5f74           music_t
-00015050: 6167 2e6c 6f61 645f 6669 6c65 280a 2020  ag.load_file(.  
-00015060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015070: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00015080: 2e70 6174 682e 6a6f 696e 2853 4f4e 4753  .path.join(SONGS
-00015090: 5f44 4952 2c20 6465 7461 696c 735b 315d  _DIR, details[1]
-000150a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000150b0: 2020 2020 2020 2020 2020 2020 2020 295b                )[
-000150c0: 2223 6c65 6e67 7468 225d 2e76 616c 7565  "#length"].value
-000150d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000150e0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-000150f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00015100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015110: 2020 2020 2073 6f6e 675f 6964 732e 7265       song_ids.re
-00015120: 6d6f 7665 2869 6e74 2864 6574 6169 6c73  move(int(details
-00015130: 5b30 5d29 290a 2020 2020 6578 6365 7074  [0])).    except
-00015140: 2046 696c 654e 6f74 466f 756e 6445 7272   FileNotFoundErr
-00015150: 6f72 3a0a 2020 2020 2020 2020 636c 6963  or:.        clic
-00015160: 6b2e 7365 6368 6f28 6622 4e6f 2073 7461  k.secho(f"No sta
-00015170: 7473 2066 6f75 6e64 2066 6f72 2079 6561  ts found for yea
-00015180: 7220 7b79 6561 727d 2e22 2c20 6667 3d22  r {year}.", fg="
-00015190: 7265 6422 290a 0a20 2020 2069 6620 736f  red")..    if so
-000151a0: 6e67 5f69 6473 3a0a 2020 2020 2020 2020  ng_ids:.        
-000151b0: 736f 6e67 5f69 6473 203d 205b 7374 7228  song_ids = [str(
-000151c0: 6964 5f29 2066 6f72 2069 645f 2069 6e20  id_) for id_ in 
-000151d0: 736f 6e67 5f69 6473 5d0a 2020 2020 2020  song_ids].      
-000151e0: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
-000151f0: 2020 2020 2020 2020 2020 2066 224e 6f20             f"No 
-00015200: 736f 6e67 7320 666f 756e 6420 7769 7468  songs found with
-00015210: 2049 4473 3a20 7b27 2c20 272e 6a6f 696e   IDs: {', '.join
-00015220: 2873 6f6e 675f 6964 7329 7d2e 222c 2066  (song_ids)}.", f
-00015230: 673d 2272 6564 220a 2020 2020 2020 2020  g="red".        
-00015240: 290a 0a0a 4063 6c69 2e63 6f6d 6d61 6e64  )...@cli.command
-00015250: 2829 0a40 636c 6963 6b2e 6172 6775 6d65  ().@click.argume
-00015260: 6e74 2822 736f 6e67 222c 2072 6571 7569  nt("song", requi
-00015270: 7265 643d 5472 7565 290a 4063 6c69 636b  red=True).@click
-00015280: 2e6f 7074 696f 6e28 0a20 2020 2022 2d4e  .option(.    "-N
-00015290: 2f2d 6e4e 222c 0a20 2020 2022 2d2d 6e61  /-nN",.    "--na
-000152a0: 6d65 2f2d 2d6e 6f2d 6e61 6d65 222c 0a20  me/--no-name",. 
-000152b0: 2020 2022 7469 746c 6522 2c0a 2020 2020     "title",.    
-000152c0: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
-000152d0: 2020 2068 656c 703d 2254 7265 6174 2053     help="Treat S
-000152e0: 4f4e 4720 6173 2061 2073 6f6e 6720 6e61  ONG as a song na
-000152f0: 6d65 2069 6e73 7465 6164 206f 6620 616e  me instead of an
-00015300: 2049 442e 222c 0a29 0a64 6566 2072 6563   ID.",.).def rec
-00015310: 6f6d 6d65 6e64 2873 6f6e 672c 2074 6974  ommend(song, tit
-00015320: 6c65 293a 0a20 2020 2022 2222 0a20 2020  le):.    """.   
-00015330: 204e 6f74 653a 2074 6869 7320 6665 6174   Note: this feat
-00015340: 7572 6520 6973 2065 7870 6572 696d 656e  ure is experimen
-00015350: 7461 6c2e 0a0a 2020 2020 5265 636f 6d6d  tal...    Recomm
-00015360: 656e 6473 2073 6f6e 6773 2028 706f 7373  ends songs (poss
-00015370: 6962 6c79 2065 7870 6c69 6369 7429 2075  ibly explicit) u
-00015380: 7369 6e67 2074 6865 2059 6f75 5475 6265  sing the YouTube
-00015390: 204d 7573 6963 2041 5049 2073 696d 696c   Music API simil
-000153a0: 6172 0a20 2020 2074 6f20 7468 6520 736f  ar.    to the so
-000153b0: 6e67 2077 6974 6820 4944 2053 4f4e 4720  ng with ID SONG 
-000153c0: 746f 206c 6973 7465 6e20 746f 2e0a 0a20  to listen to... 
-000153d0: 2020 2049 6620 7468 6520 272d 4e27 2066     If the '-N' f
-000153e0: 6c61 6720 6973 2070 6173 7365 642c 2053  lag is passed, S
-000153f0: 4f4e 4720 6973 2074 7265 6174 6564 2061  ONG is treated a
-00015400: 7320 6120 736f 6e67 206e 616d 6520 746f  s a song name to
-00015410: 2073 6561 7263 6820 666f 720a 2020 2020   search for.    
-00015420: 6f6e 2059 6f75 5475 6265 204d 7573 6963  on YouTube Music
-00015430: 2e22 2222 0a20 2020 2074 7279 3a0a 2020  .""".    try:.  
-00015440: 2020 2020 2020 6672 6f6d 2079 746d 7573        from ytmus
-00015450: 6963 6170 6920 696d 706f 7274 2059 544d  icapi import YTM
-00015460: 7573 6963 0a20 2020 2065 7863 6570 7420  usic.    except 
-00015470: 496d 706f 7274 4572 726f 723a 0a20 2020  ImportError:.   
-00015480: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
-00015490: 280a 2020 2020 2020 2020 2020 2020 2254  (.            "T
-000154a0: 6865 2027 7265 636f 6d6d 656e 6427 2063  he 'recommend' c
-000154b0: 6f6d 6d61 6e64 2072 6571 7569 7265 7320  ommand requires 
-000154c0: 7468 6520 2779 746d 7573 6963 6170 6927  the 'ytmusicapi'
-000154d0: 2070 6163 6b61 6765 2074 6f20 6265 2069   package to be i
-000154e0: 6e73 7461 6c6c 6564 2e20 5275 6e20 2770  nstalled. Run 'p
-000154f0: 6970 2069 6e73 7461 6c6c 2079 746d 7573  ip install ytmus
-00015500: 6963 6170 6927 2074 6f20 696e 7374 616c  icapi' to instal
-00015510: 6c20 6974 2e22 2c0a 2020 2020 2020 2020  l it.",.        
-00015520: 2020 2020 6667 3d22 7265 6422 2c0a 2020      fg="red",.  
-00015530: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00015540: 7265 7475 726e 0a0a 2020 2020 7974 6d75  return..    ytmu
-00015550: 7369 6320 3d20 5954 4d75 7369 6328 290a  sic = YTMusic().
-00015560: 0a20 2020 2069 6620 7469 746c 653a 0a20  .    if title:. 
-00015570: 2020 2020 2020 2072 6573 756c 7473 203d         results =
-00015580: 2079 746d 7573 6963 2e73 6561 7263 6828   ytmusic.search(
-00015590: 736f 6e67 2c20 6669 6c74 6572 3d22 736f  song, filter="so
-000155a0: 6e67 7322 290a 2020 2020 656c 7365 3a0a  ngs").    else:.
-000155b0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-000155c0: 6f6e 672e 6973 6469 6769 7428 293a 0a20  ong.isdigit():. 
-000155d0: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-000155e0: 2e73 6563 686f 280a 2020 2020 2020 2020  .secho(.        
-000155f0: 2020 2020 2020 2020 2253 6f6e 6720 4944          "Song ID
-00015600: 206d 7573 7420 6265 2061 206e 756d 6265   must be a numbe
-00015610: 722e 2054 6f20 6765 7420 7265 636f 6d6d  r. To get recomm
-00015620: 656e 6461 7469 6f6e 7320 6279 206e 616d  endations by nam
-00015630: 652c 2070 6173 7320 7468 6520 272d 4e2f  e, pass the '-N/
-00015640: 2d2d 6e61 6d65 2720 666c 6167 2e22 2c0a  --name' flag.",.
-00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015660: 6667 3d22 7265 6422 2c0a 2020 2020 2020  fg="red",.      
-00015670: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00015680: 2020 2020 7265 7475 726e 0a0a 2020 2020      return..    
-00015690: 2020 2020 7769 7468 206f 7065 6e28 534f      with open(SO
-000156a0: 4e47 535f 494e 464f 5f50 4154 482c 2022  NGS_INFO_PATH, "
-000156b0: 7222 2c20 656e 636f 6469 6e67 3d22 7574  r", encoding="ut
-000156c0: 662d 3822 2920 6173 2073 6f6e 6773 5f66  f-8") as songs_f
-000156d0: 696c 653a 0a20 2020 2020 2020 2020 2020  ile:.           
-000156e0: 2066 6f72 206c 696e 6520 696e 2073 6f6e   for line in son
-000156f0: 6773 5f66 696c 653a 0a20 2020 2020 2020  gs_file:.       
-00015700: 2020 2020 2020 2020 2064 6574 6169 6c73           details
-00015710: 203d 206c 696e 652e 7374 7269 7028 292e   = line.strip().
-00015720: 7370 6c69 7428 227c 2229 0a20 2020 2020  split("|").     
-00015730: 2020 2020 2020 2020 2020 2069 6620 6465             if de
-00015740: 7461 696c 735b 305d 203d 3d20 736f 6e67  tails[0] == song
-00015750: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015760: 2020 2020 2020 7265 7375 6c74 7320 3d20        results = 
-00015770: 7974 6d75 7369 632e 7365 6172 6368 280a  ytmusic.search(.
-00015780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015790: 2020 2020 2020 2020 6f73 2e70 6174 682e          os.path.
-000157a0: 7370 6c69 7465 7874 2864 6574 6169 6c73  splitext(details
-000157b0: 5b31 5d29 5b30 5d2c 2066 696c 7465 723d  [1])[0], filter=
-000157c0: 2273 6f6e 6773 220a 2020 2020 2020 2020  "songs".        
-000157d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-000157e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157f0: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00015800: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00015810: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
-00015820: 7365 6368 6f28 6622 4e6f 2073 6f6e 6720  secho(f"No song 
-00015830: 666f 756e 6420 7769 7468 2049 4420 7b73  found with ID {s
-00015840: 6f6e 677d 2e22 2c20 6667 3d22 7265 6422  ong}.", fg="red"
-00015850: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00015860: 2020 7265 7475 726e 0a0a 2020 2020 7974    return..    yt
-00015870: 5f6d 7573 6963 5f70 6c61 796c 6973 7420  _music_playlist 
-00015880: 3d20 7974 6d75 7369 632e 6765 745f 7761  = ytmusic.get_wa
-00015890: 7463 685f 706c 6179 6c69 7374 2872 6573  tch_playlist(res
-000158a0: 756c 7473 5b30 5d5b 2276 6964 656f 4964  ults[0]["videoId
-000158b0: 225d 290a 0a20 2020 2063 6c69 636b 2e65  "])..    click.e
-000158c0: 6368 6f28 2252 6563 6f6d 6d65 6e64 6174  cho("Recommendat
-000158d0: 696f 6e73 2066 6f72 2022 2c20 6e6c 3d46  ions for ", nl=F
-000158e0: 616c 7365 290a 2020 2020 636c 6963 6b2e  alse).    click.
-000158f0: 7365 6368 6f28 0a20 2020 2020 2020 2079  secho(.        y
-00015900: 745f 6d75 7369 635f 706c 6179 6c69 7374  t_music_playlist
-00015910: 5b22 7472 6163 6b73 225d 5b30 5d5b 2274  ["tracks"][0]["t
-00015920: 6974 6c65 225d 202b 2022 2022 2c0a 2020  itle"] + " ",.  
-00015930: 2020 2020 2020 6667 3d22 626c 7565 222c        fg="blue",
-00015940: 0a20 2020 2020 2020 206e 6c3d 4661 6c73  .        nl=Fals
-00015950: 652c 0a20 2020 2029 0a20 2020 2063 6c69  e,.    ).    cli
-00015960: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
-00015970: 2020 6622 2868 7474 7073 3a2f 2f6d 7573    f"(https://mus
-00015980: 6963 2e79 6f75 7475 6265 2e63 6f6d 2f77  ic.youtube.com/w
-00015990: 6174 6368 3f76 3d7b 7974 5f6d 7573 6963  atch?v={yt_music
-000159a0: 5f70 6c61 796c 6973 745b 2774 7261 636b  _playlist['track
-000159b0: 7327 5d5b 305d 5b27 7669 6465 6f49 6427  s'][0]['videoId'
-000159c0: 5d7d 2922 2c0a 2020 2020 2020 2020 6667  ]})",.        fg
-000159d0: 3d22 6272 6967 6874 5f62 6c61 636b 222c  ="bright_black",
-000159e0: 0a20 2020 2020 2020 206e 6c3d 4661 6c73  .        nl=Fals
-000159f0: 652c 0a20 2020 2029 0a20 2020 2063 6c69  e,.    ).    cli
-00015a00: 636b 2e65 6368 6f28 223a 2229 0a20 2020  ck.echo(":").   
-00015a10: 2066 6f72 2074 7261 636b 2069 6e20 7974   for track in yt
-00015a20: 5f6d 7573 6963 5f70 6c61 796c 6973 745b  _music_playlist[
-00015a30: 2274 7261 636b 7322 5d5b 313a 5d3a 0a20  "tracks"][1:]:. 
-00015a40: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
-00015a50: 686f 2874 7261 636b 5b22 7469 746c 6522  ho(track["title"
-00015a60: 5d20 2b20 2220 222c 2066 673d 2262 6c75  ] + " ", fg="blu
-00015a70: 6522 2c20 626f 6c64 3d54 7275 652c 206e  e", bold=True, n
-00015a80: 6c3d 4661 6c73 6529 0a20 2020 2020 2020  l=False).       
-00015a90: 2063 6c69 636b 2e73 6563 686f 280a 2020   click.secho(.  
-00015aa0: 2020 2020 2020 2020 2020 6622 6874 7470            f"http
-00015ab0: 733a 2f2f 6d75 7369 632e 796f 7574 7562  s://music.youtub
-00015ac0: 652e 636f 6d2f 7761 7463 683f 763d 7b74  e.com/watch?v={t
-00015ad0: 7261 636b 5b27 7669 6465 6f49 6427 5d7d  rack['videoId']}
-00015ae0: 222c 0a20 2020 2020 2020 2020 2020 2066  ",.            f
-00015af0: 673d 2262 7269 6768 745f 626c 6163 6b22  g="bright_black"
-00015b00: 2c0a 2020 2020 2020 2020 290a 0a0a 4063  ,.        )...@c
-00015b10: 6c69 2e63 6f6d 6d61 6e64 2829 0a40 636c  li.command().@cl
-00015b20: 6963 6b2e 6172 6775 6d65 6e74 2822 736f  ick.argument("so
-00015b30: 6e67 5f69 6473 222c 2072 6571 7569 7265  ng_ids", require
-00015b40: 643d 5472 7565 2c20 7479 7065 3d69 6e74  d=True, type=int
-00015b50: 2c20 6e61 7267 733d 2d31 290a 4063 6c69  , nargs=-1).@cli
-00015b60: 636b 2e6f 7074 696f 6e28 222d 422f 2d6e  ck.option("-B/-n
-00015b70: 4222 2c20 222d 2d62 6f74 746f 6d2f 2d2d  B", "--bottom/--
-00015b80: 6e6f 2d62 6f74 746f 6d22 2c20 2262 6f74  no-bottom", "bot
-00015b90: 746f 6d22 2c20 6465 6661 756c 743d 4661  tom", default=Fa
-00015ba0: 6c73 6529 0a64 6566 2070 7573 6828 736f  lse).def push(so
-00015bb0: 6e67 5f69 6473 2c20 626f 7474 6f6d 293a  ng_ids, bottom):
-00015bc0: 0a20 2020 2022 2222 0a20 2020 2050 7573  .    """.    Pus
-00015bd0: 6820 7468 6520 736f 6e67 2873 2920 7769  h the song(s) wi
-00015be0: 7468 2049 4428 7329 2053 4f4e 475f 4944  th ID(s) SONG_ID
-00015bf0: 5320 746f 2074 6865 2074 6f70 206f 6620  S to the top of 
-00015c00: 7468 6520 706c 6179 6c69 7374 2028 6173  the playlist (as
-00015c10: 2069 6620 7468 6579 0a20 2020 2077 6572   if they.    wer
-00015c20: 6520 7468 6520 736f 6e67 7320 6d6f 7374  e the songs most
-00015c30: 2072 6563 656e 746c 7920 6164 6465 6429   recently added)
-00015c40: 2069 6e20 7468 6520 6f72 6465 7220 7468   in the order th
-00015c50: 6579 2061 7265 2070 6173 7365 6420 2865  ey are passed (e
-00015c60: 2e67 2e0a 2020 2020 276d 6165 7374 726f  .g..    'maestro
-00015c70: 2070 7573 6820 3120 3220 3327 2077 696c   push 1 2 3' wil
-00015c80: 6c20 6d61 6b65 2074 6865 206d 6f73 7420  l make the most 
-00015c90: 7265 6365 6e74 2073 6f6e 6720 6265 2033  recent song be 3
-00015ca0: 292e 0a0a 2020 2020 4966 2074 6865 2027  )...    If the '
-00015cb0: 2d42 2720 666c 6167 2069 7320 7061 7373  -B' flag is pass
-00015cc0: 6564 2c20 7468 6520 736f 6e67 2873 2920  ed, the song(s) 
-00015cd0: 7769 6c6c 2062 6520 7075 7368 6564 2074  will be pushed t
-00015ce0: 6f20 7468 6520 626f 7474 6f6d 206f 6620  o the bottom of 
-00015cf0: 7468 650a 2020 2020 6c69 7374 2069 6e73  the.    list ins
-00015d00: 7465 6164 2e0a 2020 2020 2222 220a 2020  tead..    """.  
-00015d10: 2020 7769 7468 206f 7065 6e28 534f 4e47    with open(SONG
-00015d20: 535f 494e 464f 5f50 4154 482c 2022 722b  S_INFO_PATH, "r+
-00015d30: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
-00015d40: 2d38 2229 2061 7320 736f 6e67 735f 6669  -8") as songs_fi
-00015d50: 6c65 3a0a 2020 2020 2020 2020 6c69 6e65  le:.        line
-00015d60: 7320 3d20 736f 6e67 735f 6669 6c65 2e72  s = songs_file.r
-00015d70: 6561 646c 696e 6573 2829 0a0a 2020 2020  eadlines()..    
-00015d80: 2020 2020 6c69 6e65 735f 746f 5f6d 6f76      lines_to_mov
-00015d90: 6520 3d20 5b5d 0a20 2020 2020 2020 2066  e = [].        f
-00015da0: 6f72 2069 2069 6e20 7261 6e67 6528 6c65  or i in range(le
-00015db0: 6e28 6c69 6e65 7329 293a 0a20 2020 2020  n(lines)):.     
-00015dc0: 2020 2020 2020 2069 6620 696e 7428 6c69         if int(li
-00015dd0: 6e65 735b 695d 2e73 706c 6974 2822 7c22  nes[i].split("|"
-00015de0: 295b 305d 2920 696e 2073 6f6e 675f 6964  )[0]) in song_id
-00015df0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00015e00: 2020 206c 696e 6573 5f74 6f5f 6d6f 7665     lines_to_move
-00015e10: 2e61 7070 656e 6428 2869 2c20 6c69 6e65  .append((i, line
-00015e20: 735b 695d 2929 0a0a 2020 2020 2020 2020  s[i]))..        
-00015e30: 666f 7220 692c 205f 2069 6e20 7265 7665  for i, _ in reve
-00015e40: 7273 6564 286c 696e 6573 5f74 6f5f 6d6f  rsed(lines_to_mo
-00015e50: 7665 293a 0a20 2020 2020 2020 2020 2020  ve):.           
-00015e60: 206c 696e 6573 2e70 6f70 2869 290a 0a20   lines.pop(i).. 
-00015e70: 2020 2020 2020 2073 6f6e 675f 6964 735f         song_ids_
-00015e80: 7769 7468 5f6f 7264 6572 203d 2064 6963  with_order = dic
-00015e90: 7428 0a20 2020 2020 2020 2020 2020 206d  t(.            m
-00015ea0: 6170 286c 616d 6264 6120 783a 2028 785b  ap(lambda x: (x[
-00015eb0: 315d 2c20 785b 305d 292c 2065 6e75 6d65  1], x[0]), enume
-00015ec0: 7261 7465 2873 6f6e 675f 6964 7329 290a  rate(song_ids)).
-00015ed0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00015ee0: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00015ef0: 6528 6c65 6e28 6c69 6e65 735f 746f 5f6d  e(len(lines_to_m
-00015f00: 6f76 6529 293a 0a20 2020 2020 2020 2020  ove)):.         
-00015f10: 2020 206c 696e 6573 5f74 6f5f 6d6f 7665     lines_to_move
-00015f20: 5b69 5d20 3d20 280a 2020 2020 2020 2020  [i] = (.        
-00015f30: 2020 2020 2020 2020 736f 6e67 5f69 6473          song_ids
-00015f40: 5f77 6974 685f 6f72 6465 725b 696e 7428  _with_order[int(
-00015f50: 6c69 6e65 735f 746f 5f6d 6f76 655b 695d  lines_to_move[i]
-00015f60: 5b31 5d2e 7370 6c69 7428 227c 2229 5b30  [1].split("|")[0
-00015f70: 5d29 5d2c 0a20 2020 2020 2020 2020 2020  ])],.           
-00015f80: 2020 2020 202a 6c69 6e65 735f 746f 5f6d       *lines_to_m
-00015f90: 6f76 655b 695d 2c0a 2020 2020 2020 2020  ove[i],.        
-00015fa0: 2020 2020 290a 0a20 2020 2020 2020 206c      )..        l
-00015fb0: 696e 6573 5f74 6f5f 6d6f 7665 2e73 6f72  ines_to_move.sor
-00015fc0: 7428 6b65 793d 6c61 6d62 6461 2078 3a20  t(key=lambda x: 
-00015fd0: 785b 305d 2c20 7265 7665 7273 653d 626f  x[0], reverse=bo
-00015fe0: 7474 6f6d 290a 0a20 2020 2020 2020 2069  ttom)..        i
-00015ff0: 6620 6e6f 7420 626f 7474 6f6d 3a0a 2020  f not bottom:.  
-00016000: 2020 2020 2020 2020 2020 6c69 6e65 7320            lines 
-00016010: 2b3d 205b 745b 325d 2066 6f72 2074 2069  += [t[2] for t i
-00016020: 6e20 6c69 6e65 735f 746f 5f6d 6f76 655d  n lines_to_move]
-00016030: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00016040: 2020 2020 2020 2020 2020 206c 696e 6573             lines
-00016050: 203d 205b 745b 325d 2066 6f72 2074 2069   = [t[2] for t i
-00016060: 6e20 6c69 6e65 735f 746f 5f6d 6f76 655d  n lines_to_move]
-00016070: 202b 206c 696e 6573 0a0a 2020 2020 2020   + lines..      
-00016080: 2020 736f 6e67 735f 6669 6c65 2e73 6565    songs_file.see
-00016090: 6b28 3029 0a20 2020 2020 2020 2073 6f6e  k(0).        son
-000160a0: 6773 5f66 696c 652e 7772 6974 6528 2222  gs_file.write(""
-000160b0: 2e6a 6f69 6e28 6c69 6e65 7329 290a 2020  .join(lines)).  
-000160c0: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
-000160d0: 2e74 7275 6e63 6174 6528 290a 0a0a 4063  .truncate()...@c
-000160e0: 6c69 2e63 6f6d 6d61 6e64 286e 616d 653d  li.command(name=
-000160f0: 2263 6c69 7022 290a 4063 6c69 636b 2e61  "clip").@click.a
-00016100: 7267 756d 656e 7428 2273 6f6e 675f 6964  rgument("song_id
-00016110: 222c 2072 6571 7569 7265 643d 5472 7565  ", required=True
-00016120: 2c20 7479 7065 3d69 6e74 290a 4063 6c69  , type=int).@cli
-00016130: 636b 2e61 7267 756d 656e 7428 2273 7461  ck.argument("sta
-00016140: 7274 222c 2072 6571 7569 7265 643d 4661  rt", required=Fa
-00016150: 6c73 652c 2074 7970 653d 666c 6f61 742c  lse, type=float,
-00016160: 2064 6566 6175 6c74 3d4e 6f6e 6529 0a40   default=None).@
-00016170: 636c 6963 6b2e 6172 6775 6d65 6e74 2822  click.argument("
-00016180: 656e 6422 2c20 7265 7175 6972 6564 3d46  end", required=F
-00016190: 616c 7365 2c20 7479 7065 3d66 6c6f 6174  alse, type=float
-000161a0: 2c20 6465 6661 756c 743d 4e6f 6e65 290a  , default=None).
-000161b0: 6465 6620 636c 6970 5f28 736f 6e67 5f69  def clip_(song_i
-000161c0: 642c 2073 7461 7274 2c20 656e 6429 3a0a  d, start, end):.
-000161d0: 2020 2020 2222 220a 2020 2020 5365 7473      """.    Sets
-000161e0: 2074 6865 2063 6c69 7020 666f 7220 7468   the clip for th
-000161f0: 6520 736f 6e67 2077 6974 6820 4944 2053  e song with ID S
-00016200: 4f4e 475f 4944 2074 6f20 7468 6520 7469  ONG_ID to the ti
-00016210: 6d65 2072 616e 6765 2053 5441 5254 2074  me range START t
-00016220: 6f20 454e 440a 2020 2020 2869 6e20 7365  o END.    (in se
-00016230: 636f 6e64 7329 2e0a 0a20 2020 2049 6620  conds)...    If 
-00016240: 454e 4420 6973 206e 6f74 2070 6173 7365  END is not passe
-00016250: 642c 2074 6865 2063 6c69 7020 7769 6c6c  d, the clip will
-00016260: 2062 6520 6672 6f6d 2053 5441 5254 2074   be from START t
-00016270: 6f20 7468 6520 656e 6420 6f66 2074 6865  o the end of the
-00016280: 2073 6f6e 672e 0a0a 2020 2020 4966 206e   song...    If n
-00016290: 6569 7468 6572 2053 5441 5254 206e 6f72  either START nor
-000162a0: 2045 4e44 2061 7265 2070 6173 7365 642c   END are passed,
-000162b0: 2061 2063 6c69 7020 6564 6974 6f72 2077   a clip editor w
-000162c0: 696c 6c20 6265 206f 7065 6e65 642c 2069  ill be opened, i
-000162d0: 6e20 7768 6963 680a 2020 2020 796f 7520  n which.    you 
-000162e0: 6361 6e20 6d6f 7665 2074 6865 2073 7461  can move the sta
-000162f0: 7274 2061 6e64 2065 6e64 206f 6620 7468  rt and end of th
-00016300: 6520 636c 6970 2061 726f 756e 6420 7573  e clip around us
-00016310: 696e 6720 7468 6520 6172 726f 7720 6b65  ing the arrow ke
-00016320: 7973 2077 6869 6c65 0a20 2020 206c 6973  ys while.    lis
-00016330: 7465 6e69 6e67 2074 6f20 7468 6520 736f  tening to the so
-00016340: 6e67 2028 616c 736f 2073 686f 7773 2077  ng (also shows w
-00016350: 6176 6566 6f72 6d29 2e0a 0a20 2020 205c  aveform)...    \
-00016360: 620a 2020 2020 5468 6520 6564 6974 6f72  b.    The editor
-00016370: 2073 7461 7274 7320 6f75 7420 6564 6974   starts out edit
-00016380: 696e 6720 7468 6520 7374 6172 7420 6f66  ing the start of
-00016390: 2074 6865 2063 6c69 702e 0a20 2020 205c   the clip..    \
-000163a0: 7831 625b 316d 745c 7831 625b 306d 2074  x1b[1mt\x1b[0m t
-000163b0: 6f20 746f 6767 6c65 2062 6574 7765 656e  o toggle between
-000163c0: 2065 6469 7469 6e67 2074 6865 2073 7461   editing the sta
-000163d0: 7274 2061 6e64 2065 6e64 206f 6620 7468  rt and end of th
-000163e0: 6520 636c 6970 2e0a 2020 2020 5c78 3162  e clip..    \x1b
-000163f0: 5b31 6d53 4849 4654 2b4c 4546 542f 5249  [1mSHIFT+LEFT/RI
-00016400: 4748 545c 7831 625b 306d 2077 696c 6c20  GHT\x1b[0m will 
-00016410: 6d6f 7665 2077 6869 6368 6576 6572 2063  move whichever c
-00016420: 6c69 7020 656e 6420 796f 7520 6172 6520  lip end you are 
-00016430: 6564 6974 696e 670a 2020 2020 2020 2020  editing.        
-00016440: 6279 2030 2e31 2073 6563 6f6e 6473 2c20  by 0.1 seconds, 
-00016450: 736e 6170 2074 6865 2063 7572 7265 6e74  snap the current
-00016460: 2070 6c61 7962 6163 6b20 746f 2074 6861   playback to tha
-00016470: 7420 636c 6970 2065 6e64 2028 746f 2065  t clip end (to e
-00016480: 7861 6374 6c79 0a20 2020 2020 2020 2074  xactly.        t
-00016490: 6865 2063 6c69 7020 7374 6172 7420 6966  he clip start if
-000164a0: 2065 6469 7469 6e67 2073 7461 7274 2c20   editing start, 
-000164b0: 656e 642d 3120 6966 2065 6469 7469 6e67  end-1 if editing
-000164c0: 2065 6e64 292c 2061 6e64 2070 6175 7365   end), and pause
-000164d0: 2e0a 2020 2020 5c78 3162 5b31 6d4c 4546  ..    \x1b[1mLEF
-000164e0: 542f 5249 4748 545c 7831 625b 306d 2077  T/RIGHT\x1b[0m w
-000164f0: 696c 6c20 6d6f 7665 2077 6869 6368 6576  ill move whichev
-00016500: 6572 2063 6c69 7020 656e 6420 796f 7520  er clip end you 
-00016510: 6172 6520 6564 6974 696e 6720 6279 2031  are editing by 1
-00016520: 0a20 2020 2020 2020 2073 6563 6f6e 642c  .        second,
-00016530: 2073 6e61 7020 7468 6520 6375 7272 656e   snap the curren
-00016540: 7420 706c 6179 6261 636b 2074 6f20 7468  t playback to th
-00016550: 6174 2063 6c69 7020 656e 642c 2061 6e64  at clip end, and
-00016560: 2070 6175 7365 2e0a 2020 2020 5c78 3162   pause..    \x1b
-00016570: 5b31 6d45 4e54 4552 5c78 3162 5b30 6d20  [1mENTER\x1b[0m 
-00016580: 7769 6c6c 2065 7869 7420 7468 6520 6564  will exit the ed
-00016590: 6974 6f72 2061 6e64 2073 6176 6520 7468  itor and save th
-000165a0: 6520 636c 6970 2e0a 2020 2020 5c78 3162  e clip..    \x1b
-000165b0: 5b31 6d71 5c78 3162 5b30 6d20 7769 6c6c  [1mq\x1b[0m will
-000165c0: 2065 7869 7420 7468 6520 6564 6974 6f72   exit the editor
-000165d0: 2077 6974 686f 7574 2073 6176 696e 6720   without saving 
-000165e0: 7468 6520 636c 6970 2e0a 2020 2020 2222  the clip..    ""
-000165f0: 220a 2020 2020 6966 2073 7461 7274 2069  ".    if start i
-00016600: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00016610: 2020 2020 6966 2073 7461 7274 203c 2030      if start < 0
-00016620: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
-00016630: 6963 6b2e 7365 6368 6f28 2253 5441 5254  ick.secho("START
-00016640: 206d 7573 7420 6265 2061 2070 6f73 6974   must be a posit
-00016650: 6976 6520 6e75 6d62 6572 2e22 2c20 6667  ive number.", fg
-00016660: 3d22 7265 6422 290a 2020 2020 2020 2020  ="red").        
-00016670: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-00016680: 2020 2069 6620 656e 6420 6973 206e 6f74     if end is not
-00016690: 204e 6f6e 6520 616e 6420 656e 6420 3c20   None and end < 
-000166a0: 303a 0a20 2020 2020 2020 2020 2020 2063  0:.            c
-000166b0: 6c69 636b 2e73 6563 686f 2822 454e 4420  lick.secho("END 
-000166c0: 6d75 7374 2062 6520 6120 706f 7369 7469  must be a positi
-000166d0: 7665 206e 756d 6265 722e 222c 2066 673d  ve number.", fg=
-000166e0: 2272 6564 2229 0a20 2020 2020 2020 2020  "red").         
-000166f0: 2020 2072 6574 7572 6e0a 0a20 2020 2077     return..    w
-00016700: 6974 6820 6f70 656e 2853 4f4e 4753 5f49  ith open(SONGS_I
-00016710: 4e46 4f5f 5041 5448 2c20 2272 2b22 2c20  NFO_PATH, "r+", 
-00016720: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
-00016730: 2920 6173 2073 6f6e 6773 5f66 696c 653a  ) as songs_file:
-00016740: 0a20 2020 2020 2020 206c 696e 6573 203d  .        lines =
-00016750: 2073 6f6e 6773 5f66 696c 652e 7265 6164   songs_file.read
-00016760: 6c69 6e65 7328 290a 0a20 2020 2020 2020  lines()..       
-00016770: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
-00016780: 6c65 6e28 6c69 6e65 7329 293a 0a20 2020  len(lines)):.   
-00016790: 2020 2020 2020 2020 2064 6574 6169 6c73           details
-000167a0: 203d 206c 696e 6573 5b69 5d2e 7374 7269   = lines[i].stri
-000167b0: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
-000167c0: 2020 2020 2020 2020 2020 2069 6620 696e             if in
-000167d0: 7428 6465 7461 696c 735b 305d 2920 3d3d  t(details[0]) ==
-000167e0: 2073 6f6e 675f 6964 3a0a 2020 2020 2020   song_id:.      
-000167f0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-00016800: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00016810: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
-00016820: 7365 6368 6f28 6622 4e6f 2073 6f6e 6720  secho(f"No song 
-00016830: 666f 756e 6420 7769 7468 2049 4420 7b73  found with ID {s
-00016840: 6f6e 675f 6964 7d2e 222c 2066 673d 2272  ong_id}.", fg="r
-00016850: 6564 2229 0a20 2020 2020 2020 2020 2020  ed").           
-00016860: 2072 6574 7572 6e0a 0a20 2020 2020 2020   return..       
-00016870: 2069 6620 7374 6172 7420 6973 204e 6f6e   if start is Non
-00016880: 653a 2020 2320 636c 6970 2065 6469 746f  e:  # clip edito
-00016890: 720a 2020 2020 2020 2020 2020 2020 7374  r.            st
-000168a0: 6172 742c 2065 6e64 203d 2063 7572 7365  art, end = curse
-000168b0: 732e 7772 6170 7065 7228 636c 6970 5f65  s.wrapper(clip_e
-000168c0: 6469 746f 722c 2064 6574 6169 6c73 290a  ditor, details).
-000168d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000168e0: 7461 7274 2069 7320 4e6f 6e65 3a0a 2020  tart is None:.  
-000168f0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00016900: 7475 726e 0a0a 2020 2020 2020 2020 736f  turn..        so
-00016910: 6e67 5f6e 616d 6520 3d20 6465 7461 696c  ng_name = detail
-00016920: 735b 315d 0a20 2020 2020 2020 2073 6f6e  s[1].        son
-00016930: 675f 7061 7468 203d 206f 732e 7061 7468  g_path = os.path
-00016940: 2e6a 6f69 6e28 534f 4e47 535f 4449 522c  .join(SONGS_DIR,
-00016950: 2073 6f6e 675f 6e61 6d65 290a 2020 2020   song_name).    
-00016960: 2020 2020 6475 7261 7469 6f6e 203d 206d      duration = m
-00016970: 7573 6963 5f74 6167 2e6c 6f61 645f 6669  usic_tag.load_fi
-00016980: 6c65 2873 6f6e 675f 7061 7468 295b 2223  le(song_path)["#
-00016990: 6c65 6e67 7468 225d 2e76 616c 7565 0a0a  length"].value..
-000169a0: 2020 2020 2020 2020 6966 2065 6e64 2069          if end i
-000169b0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-000169c0: 2020 2020 656e 6420 3d20 6475 7261 7469      end = durati
-000169d0: 6f6e 0a0a 2020 2020 2020 2020 6966 2073  on..        if s
-000169e0: 7461 7274 203e 2064 7572 6174 696f 6e3a  tart > duration:
-000169f0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00016a00: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
-00016a10: 2020 2020 2020 2020 2020 2253 5441 5254            "START
-00016a20: 206d 7573 7420 6e6f 7420 6265 206d 6f72   must not be mor
-00016a30: 6520 7468 616e 2074 6865 2073 6f6e 6720  e than the song 
-00016a40: 6475 7261 7469 6f6e 2e22 2c20 6667 3d22  duration.", fg="
-00016a50: 7265 6422 0a20 2020 2020 2020 2020 2020  red".           
-00016a60: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
-00016a70: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-00016a80: 2065 6e64 203e 2064 7572 6174 696f 6e3a   end > duration:
-00016a90: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-00016aa0: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
-00016ab0: 2020 2020 2020 2020 2020 2245 4e44 206d            "END m
-00016ac0: 7573 7420 6e6f 7420 6265 206d 6f72 6520  ust not be more 
-00016ad0: 7468 616e 2074 6865 2073 6f6e 6720 6475  than the song du
-00016ae0: 7261 7469 6f6e 2e22 2c20 6667 3d22 7265  ration.", fg="re
-00016af0: 6422 0a20 2020 2020 2020 2020 2020 2029  d".            )
-00016b00: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00016b10: 7572 6e0a 2020 2020 2020 2020 6966 2073  urn.        if s
-00016b20: 7461 7274 203e 2065 6e64 3a0a 2020 2020  tart > end:.    
-00016b30: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
-00016b40: 6368 6f28 2253 5441 5254 206d 7573 7420  cho("START must 
-00016b50: 6e6f 7420 6265 206d 6f72 6520 7468 616e  not be more than
-00016b60: 2045 4e44 2e22 2c20 6667 3d22 7265 6422   END.", fg="red"
-00016b70: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00016b80: 7475 726e 0a0a 2020 2020 2020 2020 6c69  turn..        li
-00016b90: 6e65 735b 695d 203d 2028 0a20 2020 2020  nes[i] = (.     
-00016ba0: 2020 2020 2020 2022 7c22 2e6a 6f69 6e28         "|".join(
-00016bb0: 6465 7461 696c 735b 3a33 5d20 2b20 5b73  details[:3] + [s
-00016bc0: 7472 2873 7461 7274 2920 2b20 2220 2220  tr(start) + " " 
-00016bd0: 2b20 7374 7228 656e 6429 5d20 2b20 6465  + str(end)] + de
-00016be0: 7461 696c 735b 353a 5d29 0a20 2020 2020  tails[5:]).     
-00016bf0: 2020 2020 2020 202b 2022 5c6e 220a 2020         + "\n".  
-00016c00: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00016c10: 2073 6f6e 6773 5f66 696c 652e 7365 656b   songs_file.seek
-00016c20: 2830 290a 2020 2020 2020 2020 736f 6e67  (0).        song
-00016c30: 735f 6669 6c65 2e77 7269 7465 2822 222e  s_file.write("".
-00016c40: 6a6f 696e 286c 696e 6573 2929 0a20 2020  join(lines)).   
-00016c50: 2020 2020 2073 6f6e 6773 5f66 696c 652e       songs_file.
-00016c60: 7472 756e 6361 7465 2829 0a0a 2020 2020  truncate()..    
-00016c70: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-00016c80: 6622 436c 6970 7065 6420 7b73 6f6e 675f  f"Clipped {song_
-00016c90: 6e61 6d65 7d20 6672 6f6d 207b 7374 6172  name} from {star
-00016ca0: 747d 2074 6f20 7b65 6e64 7d2e 222c 2066  t} to {end}.", f
-00016cb0: 673d 2267 7265 656e 2229 0a0a 0a40 636c  g="green")...@cl
-00016cc0: 692e 636f 6d6d 616e 6428 290a 4063 6c69  i.command().@cli
-00016cd0: 636b 2e61 7267 756d 656e 7428 2273 6f6e  ck.argument("son
-00016ce0: 675f 6964 7322 2c20 7479 7065 3d69 6e74  g_ids", type=int
-00016cf0: 2c20 6e61 7267 733d 2d31 2c20 7265 7175  , nargs=-1, requ
-00016d00: 6972 6564 3d46 616c 7365 290a 4063 6c69  ired=False).@cli
-00016d10: 636b 2e6f 7074 696f 6e28 0a20 2020 2022  ck.option(.    "
-00016d20: 2d41 2f2d 6e41 222c 0a20 2020 2022 2d2d  -A/-nA",.    "--
-00016d30: 616c 6c2f 2d2d 6e6f 2d61 6c6c 222c 0a20  all/--no-all",. 
-00016d40: 2020 2022 616c 6c5f 222c 0a20 2020 2064     "all_",.    d
-00016d50: 6566 6175 6c74 3d46 616c 7365 2c0a 2020  efault=False,.  
-00016d60: 2020 6865 6c70 3d22 5265 6d6f 7665 2063    help="Remove c
-00016d70: 6c69 7073 2066 6f72 2061 6c6c 2073 6f6e  lips for all son
-00016d80: 6773 2e20 4967 6e6f 7265 7320 534f 4e47  gs. Ignores SONG
-00016d90: 5f49 4453 2e22 2c0a 290a 4063 6c69 636b  _IDS.",.).@click
-00016da0: 2e6f 7074 696f 6e28 222d 462f 2d6e 4622  .option("-F/-nF"
-00016db0: 2c20 222d 2d66 6f72 6365 2f2d 2d6e 6f2d  , "--force/--no-
-00016dc0: 666f 7263 6522 2c20 2266 6f72 6365 222c  force", "force",
-00016dd0: 2064 6566 6175 6c74 3d46 616c 7365 290a   default=False).
-00016de0: 6465 6620 756e 636c 6970 2873 6f6e 675f  def unclip(song_
-00016df0: 6964 732c 2061 6c6c 5f2c 2066 6f72 6365  ids, all_, force
-00016e00: 293a 0a20 2020 2022 2222 0a20 2020 2052  ):.    """.    R
-00016e10: 656d 6f76 6573 2063 6c69 7020 666f 7220  emoves clip for 
-00016e20: 7468 6520 736f 6e67 2873 2920 7769 7468  the song(s) with
-00016e30: 2049 4428 7329 2053 4f4e 475f 4944 532e   ID(s) SONG_IDS.
-00016e40: 0a0a 2020 2020 4966 2074 6865 2027 2d41  ..    If the '-A
-00016e50: 2f2d 2d61 6c6c 2720 666c 6167 2069 7320  /--all' flag is 
-00016e60: 7061 7373 6564 2c20 7468 6520 636c 6970  passed, the clip
-00016e70: 7320 666f 7220 616c 6c20 736f 6e67 7320  s for all songs 
-00016e80: 7769 6c6c 2062 6520 7265 6d6f 7665 642c  will be removed,
-00016e90: 0a20 2020 2069 676e 6f72 696e 6720 534f  .    ignoring SO
-00016ea0: 4e47 5f49 4453 2e20 5468 6973 2070 726f  NG_IDS. This pro
-00016eb0: 6d70 7473 2066 6f72 2063 6f6e 6669 726d  mpts for confirm
-00016ec0: 6174 696f 6e20 756e 6c65 7373 2074 6865  ation unless the
-00016ed0: 2027 2d46 2f2d 2d66 6f72 6365 270a 2020   '-F/--force'.  
-00016ee0: 2020 666c 6167 2069 7320 7061 7373 6564    flag is passed
-00016ef0: 2e0a 2020 2020 2222 220a 2020 2020 6966  ..    """.    if
-00016f00: 206e 6f74 2061 6c6c 5f3a 0a20 2020 2020   not all_:.     
-00016f10: 2020 2069 6620 736f 6e67 5f69 6473 3a0a     if song_ids:.
-00016f20: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-00016f30: 5f69 6473 203d 2073 6574 2873 6f6e 675f  _ids = set(song_
-00016f40: 6964 7329 0a20 2020 2020 2020 2065 6c73  ids).        els
-00016f50: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
-00016f60: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
-00016f70: 2020 2020 2020 2020 2020 2020 224e 6f20              "No 
-00016f80: 736f 6e67 2049 4473 2070 6173 7365 642e  song IDs passed.
-00016f90: 2054 6f20 7265 6d6f 7665 2063 6c69 7073   To remove clips
-00016fa0: 2066 6f72 2061 6c6c 2073 6f6e 6773 2c20   for all songs, 
-00016fb0: 7061 7373 2074 6865 2027 2d41 2f2d 2d61  pass the '-A/--a
-00016fc0: 6c6c 2720 666c 6167 2e22 2c0a 2020 2020  ll' flag.",.    
-00016fd0: 2020 2020 2020 2020 2020 2020 6667 3d22              fg="
-00016fe0: 7265 6422 2c0a 2020 2020 2020 2020 2020  red",.          
-00016ff0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00017000: 7265 7475 726e 0a0a 2020 2020 6966 2061  return..    if a
-00017010: 6c6c 5f20 616e 6420 6e6f 7420 666f 7263  ll_ and not forc
-00017020: 653a 0a20 2020 2020 2020 2063 6c69 636b  e:.        click
-00017030: 2e65 6368 6f28 0a20 2020 2020 2020 2020  .echo(.         
-00017040: 2020 2022 4172 6520 796f 7520 7375 7265     "Are you sure
-00017050: 2079 6f75 2077 616e 7420 746f 2072 656d   you want to rem
-00017060: 6f76 6520 636c 6970 7320 666f 7220 616c  ove clips for al
-00017070: 6c20 736f 6e67 733f 2054 6869 7320 6361  l songs? This ca
-00017080: 6e6e 6f74 2062 6520 756e 646f 6e65 2e20  nnot be undone. 
-00017090: 5b79 2f6e 5d20 222c 0a20 2020 2020 2020  [y/n] ",.       
-000170a0: 2029 0a20 2020 2020 2020 2069 6620 696e   ).        if in
-000170b0: 7075 7428 292e 6c6f 7765 7228 2920 213d  put().lower() !=
-000170c0: 2022 7922 3a0a 2020 2020 2020 2020 2020   "y":.          
-000170d0: 2020 7265 7475 726e 0a0a 2020 2020 7769    return..    wi
-000170e0: 7468 206f 7065 6e28 534f 4e47 535f 494e  th open(SONGS_IN
-000170f0: 464f 5f50 4154 482c 2022 722b 222c 2065  FO_PATH, "r+", e
-00017100: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
-00017110: 2061 7320 736f 6e67 735f 6669 6c65 3a0a   as songs_file:.
-00017120: 2020 2020 2020 2020 6c69 6e65 7320 3d20          lines = 
-00017130: 736f 6e67 735f 6669 6c65 2e72 6561 646c  songs_file.readl
-00017140: 696e 6573 2829 0a0a 2020 2020 2020 2020  ines()..        
-00017150: 666f 7220 6920 696e 2072 616e 6765 286c  for i in range(l
-00017160: 656e 286c 696e 6573 2929 3a0a 2020 2020  en(lines)):.    
-00017170: 2020 2020 2020 2020 6465 7461 696c 7320          details 
-00017180: 3d20 6c69 6e65 735b 695d 2e73 7472 6970  = lines[i].strip
-00017190: 2829 2e73 706c 6974 2822 7c22 290a 2020  ().split("|").  
-000171a0: 2020 2020 2020 2020 2020 6966 2061 6c6c            if all
-000171b0: 5f20 6f72 2069 6e74 2864 6574 6169 6c73  _ or int(details
-000171c0: 5b30 5d29 2069 6e20 736f 6e67 5f69 6473  [0]) in song_ids
-000171d0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000171e0: 2020 6c69 6e65 735b 695d 203d 2022 7c22    lines[i] = "|"
-000171f0: 2e6a 6f69 6e28 6465 7461 696c 735b 3a33  .join(details[:3
-00017200: 5d20 2b20 5b22 225d 202b 2064 6574 6169  ] + [""] + detai
-00017210: 6c73 5b35 3a5d 2920 2b20 225c 6e22 0a0a  ls[5:]) + "\n"..
-00017220: 2020 2020 2020 2020 736f 6e67 735f 6669          songs_fi
-00017230: 6c65 2e73 6565 6b28 3029 0a20 2020 2020  le.seek(0).     
-00017240: 2020 2073 6f6e 6773 5f66 696c 652e 7772     songs_file.wr
-00017250: 6974 6528 2222 2e6a 6f69 6e28 6c69 6e65  ite("".join(line
-00017260: 7329 290a 2020 2020 2020 2020 736f 6e67  s)).        song
-00017270: 735f 6669 6c65 2e74 7275 6e63 6174 6528  s_file.truncate(
-00017280: 290a 0a20 2020 2069 6620 616c 6c5f 3a0a  )..    if all_:.
-00017290: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
-000172a0: 6368 6f28 2252 656d 6f76 6564 2063 6c69  cho("Removed cli
-000172b0: 7073 2066 6f72 2061 6c6c 2073 6f6e 6773  ps for all songs
-000172c0: 2e22 2c20 6667 3d22 6772 6565 6e22 290a  .", fg="green").
-000172d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000172e0: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
-000172f0: 2020 2020 2020 2020 2020 2066 2252 656d             f"Rem
-00017300: 6f76 6564 2063 6c69 7028 7329 2066 6f72  oved clip(s) for
-00017310: 2073 6f6e 6728 7329 2077 6974 6820 4944   song(s) with ID
-00017320: 2873 2920 7b27 2c20 272e 6a6f 696e 286d  (s) {', '.join(m
-00017330: 6170 2873 7472 2c20 736f 6e67 5f69 6473  ap(str, song_ids
-00017340: 2929 7d2e 222c 0a20 2020 2020 2020 2020  ))}.",.         
-00017350: 2020 2066 673d 2267 7265 656e 222c 0a20     fg="green",. 
-00017360: 2020 2020 2020 2029 0a0a 0a40 636c 692e         )...@cli.
-00017370: 636f 6d6d 616e 6428 290a 4063 6c69 636b  command().@click
-00017380: 2e61 7267 756d 656e 7428 2273 6f6e 675f  .argument("song_
-00017390: 6964 7322 2c20 7479 7065 3d69 6e74 2c20  ids", type=int, 
-000173a0: 6e61 7267 733d 2d31 2c20 7265 7175 6972  nargs=-1, requir
-000173b0: 6564 3d46 616c 7365 290a 4063 6c69 636b  ed=False).@click
-000173c0: 2e6f 7074 696f 6e28 0a20 2020 2022 2d46  .option(.    "-F
-000173d0: 2f2d 6e46 222c 0a20 2020 2022 2d2d 666f  /-nF",.    "--fo
-000173e0: 7263 652f 2d2d 6e6f 2d66 6f72 6365 222c  rce/--no-force",
-000173f0: 0a20 2020 2022 7265 6361 6368 6522 2c0a  .    "recache",.
-00017400: 2020 2020 6465 6661 756c 743d 4661 6c73      default=Fals
-00017410: 652c 0a20 2020 2068 656c 703d 2246 6f72  e,.    help="For
-00017420: 6365 2072 6563 616c 6375 6c61 7469 6f6e  ce recalculation
-00017430: 206f 6620 6578 6973 7469 6e67 2076 6973   of existing vis
-00017440: 7561 6c69 7a61 7469 6f6e 2066 7265 7175  ualization frequ
-00017450: 656e 6379 2063 6163 6865 732e 222c 0a29  ency caches.",.)
-00017460: 0a40 636c 6963 6b2e 6f70 7469 6f6e 280a  .@click.option(.
-00017470: 2020 2020 222d 412f 2d6e 4122 2c0a 2020      "-A/-nA",.  
-00017480: 2020 222d 2d61 6c6c 2f2d 2d6e 6f2d 616c    "--all/--no-al
-00017490: 6c22 2c0a 2020 2020 2261 6c6c 5f22 2c0a  l",.    "all_",.
-000174a0: 2020 2020 6465 6661 756c 743d 4661 6c73      default=Fals
-000174b0: 652c 0a20 2020 2068 656c 703d 2243 616c  e,.    help="Cal
-000174c0: 6375 6c61 7465 2076 6973 7561 6c69 7a61  culate visualiza
-000174d0: 7469 6f6e 2066 7265 7175 656e 6379 2063  tion frequency c
-000174e0: 6163 6865 7320 666f 7220 616c 6c20 736f  aches for all so
-000174f0: 6e67 732e 2049 676e 6f72 6573 2053 4f4e  ngs. Ignores SON
-00017500: 475f 4944 532e 222c 0a29 0a64 6566 2063  G_IDS.",.).def c
-00017510: 6163 6865 2873 6f6e 675f 6964 732c 2072  ache(song_ids, r
-00017520: 6563 6163 6865 2c20 616c 6c5f 293a 0a20  ecache, all_):. 
-00017530: 2020 2022 2222 0a20 2020 2043 616c 6375     """.    Calcu
-00017540: 6c61 7465 2061 6e64 2063 6163 6865 2061  late and cache a
-00017550: 7564 696f 2064 6174 6120 616e 6420 7669  udio data and vi
-00017560: 7375 616c 697a 6174 696f 6e20 6672 6571  sualization freq
-00017570: 7565 6e63 6965 7320 666f 7220 7468 6520  uencies for the 
-00017580: 736f 6e67 2873 290a 2020 2020 7769 7468  song(s).    with
-00017590: 2049 4428 7329 2053 4f4e 475f 4944 532e   ID(s) SONG_IDS.
-000175a0: 2049 6620 616e 7920 6361 6368 6564 2064   If any cached d
-000175b0: 6174 6120 6f66 2065 6974 6865 7220 6b69  ata of either ki
-000175c0: 6e64 2061 6c72 6561 6479 2065 7869 7374  nd already exist
-000175d0: 732c 2074 6869 730a 2020 2020 636f 6d6d  s, this.    comm
-000175e0: 616e 6420 646f 6573 206e 6f74 6869 6e67  and does nothing
-000175f0: 2075 6e6c 6573 7320 272d 462f 2d2d 666f   unless '-F/--fo
-00017600: 7263 6527 2069 7320 7061 7373 6564 2e0a  rce' is passed..
-00017610: 0a20 2020 2054 6f20 7275 6e20 7468 6973  .    To run this
-00017620: 2063 6f6d 6d61 6e64 2066 6f72 2061 6c6c   command for all
-00017630: 2073 6f6e 6773 2c20 7061 7373 2074 6865   songs, pass the
-00017640: 2027 2d41 2f2d 2d61 6c6c 2720 666c 6167   '-A/--all' flag
-00017650: 2028 6967 6e6f 7265 730a 2020 2020 534f   (ignores.    SO
-00017660: 4e47 5f49 4453 292e 0a20 2020 2022 2222  NG_IDS)..    """
-00017670: 0a20 2020 2069 6620 736f 6e67 5f69 6473  .    if song_ids
-00017680: 3a0a 2020 2020 2020 2020 736f 6e67 5f69  :.        song_i
-00017690: 6473 203d 2073 6574 2873 6f6e 675f 6964  ds = set(song_id
-000176a0: 7329 0a20 2020 2065 6c73 653a 0a20 2020  s).    else:.   
-000176b0: 2020 2020 2069 6620 6e6f 7420 616c 6c5f       if not all_
-000176c0: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
-000176d0: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
-000176e0: 2020 2020 2020 2020 2020 2022 4e6f 2073             "No s
-000176f0: 6f6e 6720 4944 7320 7061 7373 6564 2e20  ong IDs passed. 
-00017700: 546f 2063 6163 6865 2064 6174 6120 666f  To cache data fo
-00017710: 7220 616c 6c20 736f 6e67 732c 2070 6173  r all songs, pas
-00017720: 7320 7468 6520 272d 412f 2d2d 616c 6c27  s the '-A/--all'
-00017730: 2066 6c61 672e 222c 0a20 2020 2020 2020   flag.",.       
-00017740: 2020 2020 2020 2020 2066 673d 2272 6564           fg="red
-00017750: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
-00017760: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00017770: 7572 6e0a 2020 2020 2020 2020 736f 6e67  urn.        song
-00017780: 5f69 6473 203d 2073 6574 2829 0a0a 2020  _ids = set()..  
-00017790: 2020 7769 7468 206f 7065 6e28 534f 4e47    with open(SONG
-000177a0: 535f 494e 464f 5f50 4154 482c 2022 7222  S_INFO_PATH, "r"
-000177b0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-000177c0: 3822 2920 6173 2073 6f6e 6773 5f66 696c  8") as songs_fil
-000177d0: 653a 0a20 2020 2020 2020 206c 696e 6573  e:.        lines
-000177e0: 203d 2073 6f6e 6773 5f66 696c 652e 7265   = songs_file.re
-000177f0: 6164 6c69 6e65 7328 290a 0a20 2020 2020  adlines()..     
-00017800: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00017810: 6528 6c65 6e28 6c69 6e65 7329 293a 0a20  e(len(lines)):. 
-00017820: 2020 2020 2020 2020 2020 2073 6f6e 675f             song_
-00017830: 6964 2c20 736f 6e67 5f6e 616d 652c 202a  id, song_name, *
-00017840: 5f20 3d20 6c69 6e65 735b 695d 2e73 7472  _ = lines[i].str
-00017850: 6970 2829 2e73 706c 6974 2822 7c22 290a  ip().split("|").
-00017860: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-00017870: 5f69 6420 3d20 696e 7428 736f 6e67 5f69  _id = int(song_i
-00017880: 6429 0a0a 2020 2020 2020 2020 2020 2020  d)..            
-00017890: 6966 2073 6f6e 675f 6964 7320 616e 6420  if song_ids and 
-000178a0: 736f 6e67 5f69 6420 6e6f 7420 696e 2073  song_id not in s
-000178b0: 6f6e 675f 6964 733a 0a20 2020 2020 2020  ong_ids:.       
-000178c0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-000178d0: 650a 0a20 2020 2020 2020 2020 2020 2076  e..            v
-000178e0: 6973 5f63 6163 6865 5f70 6174 6820 3d20  is_cache_path = 
-000178f0: 6f73 2e70 6174 682e 6a6f 696e 280a 2020  os.path.join(.  
-00017900: 2020 2020 2020 2020 2020 2020 2020 4652                FR
-00017910: 4551 5f43 4143 4845 5f44 4952 2c0a 2020  EQ_CACHE_DIR,.  
-00017920: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00017930: 2e70 6174 682e 7370 6c69 7465 7874 2873  .path.splitext(s
-00017940: 6f6e 675f 6e61 6d65 295b 305d 202b 2022  ong_name)[0] + "
-00017950: 2e6e 7079 222c 0a20 2020 2020 2020 2020  .npy",.         
-00017960: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00017970: 2064 6174 615f 6361 6368 655f 7061 7468   data_cache_path
-00017980: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-00017990: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000179a0: 2044 4154 415f 4341 4348 455f 4449 522c   DATA_CACHE_DIR,
-000179b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000179c0: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
-000179d0: 7428 736f 6e67 5f6e 616d 6529 5b30 5d20  t(song_name)[0] 
-000179e0: 2b20 222e 6e70 7922 2c0a 2020 2020 2020  + ".npy",.      
-000179f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00017a00: 2020 2020 6966 206f 732e 7061 7468 2e65      if os.path.e
-00017a10: 7869 7374 7328 7669 735f 6361 6368 655f  xists(vis_cache_
-00017a20: 7061 7468 2920 6f72 206f 732e 7061 7468  path) or os.path
-00017a30: 2e65 7869 7374 7328 0a20 2020 2020 2020  .exists(.       
-00017a40: 2020 2020 2020 2020 2064 6174 615f 6361           data_ca
-00017a50: 6368 655f 7061 7468 0a20 2020 2020 2020  che_path.       
-00017a60: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00017a70: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-00017a80: 6563 6163 6865 3a0a 2020 2020 2020 2020  ecache:.        
-00017a90: 2020 2020 2020 2020 2020 2020 636c 6963              clic
-00017aa0: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
-00017ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ac0: 2066 2254 6865 2073 6f6e 6720 7b73 6f6e   f"The song {son
-00017ad0: 675f 6e61 6d65 7d20 7769 7468 2049 4420  g_name} with ID 
-00017ae0: 7b73 6f6e 675f 6964 7d20 616c 7265 6164  {song_id} alread
-00017af0: 7920 6861 7320 6361 6368 6564 2064 6174  y has cached dat
-00017b00: 612e 2054 6f20 666f 7263 6520 7265 6361  a. To force reca
-00017b10: 6c63 756c 6174 696f 6e2c 2070 6173 7320  lculation, pass 
-00017b20: 7468 6520 272d 462f 2d2d 666f 7263 6527  the '-F/--force'
-00017b30: 2066 6c61 672e 222c 0a20 2020 2020 2020   flag.",.       
-00017b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b50: 2066 673d 2279 656c 6c6f 7722 2c0a 2020   fg="yellow",.  
-00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017b70: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00017b80: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00017b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017ba0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00017bb0: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
-00017bc0: 2e70 6174 682e 6578 6973 7473 2876 6973  .path.exists(vis
-00017bd0: 5f63 6163 6865 5f70 6174 6829 3a0a 2020  _cache_path):.  
-00017be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017bf0: 2020 2020 2020 6f73 2e72 656d 6f76 6528        os.remove(
-00017c00: 7669 735f 6361 6368 655f 7061 7468 290a  vis_cache_path).
-00017c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c20: 2020 2020 6966 206f 732e 7061 7468 2e65      if os.path.e
-00017c30: 7869 7374 7328 6461 7461 5f63 6163 6865  xists(data_cache
-00017c40: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
-00017c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c60: 6f73 2e72 656d 6f76 6528 6461 7461 5f63  os.remove(data_c
-00017c70: 6163 6865 5f70 6174 6829 0a0a 2020 2020  ache_path)..    
-00017c80: 2020 2020 2020 2020 6461 7461 203d 2041          data = A
-00017c90: 7564 696f 4461 7461 286f 732e 7061 7468  udioData(os.path
-00017ca0: 2e6a 6f69 6e28 534f 4e47 535f 4449 522c  .join(SONGS_DIR,
-00017cb0: 2073 6f6e 675f 6e61 6d65 2929 0a0a 2020   song_name))..  
-00017cc0: 2020 2020 2020 2020 2020 6966 2064 6174            if dat
-00017cd0: 612e 6c6f 6164 6564 5f73 6f6e 6720 6973  a.loaded_song is
-00017ce0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00017cf0: 2020 2020 2020 2020 2020 2063 6c69 636b             click
-00017d00: 2e73 6563 686f 280a 2020 2020 2020 2020  .secho(.        
-00017d10: 2020 2020 2020 2020 2020 2020 6622 4361              f"Ca
-00017d20: 6368 6564 2064 6174 6120 666f 7220 736f  ched data for so
-00017d30: 6e67 207b 736f 6e67 5f6e 616d 657d 2077  ng {song_name} w
-00017d40: 6974 6820 4944 207b 736f 6e67 5f69 647d  ith ID {song_id}
-00017d50: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
-00017d60: 2020 2020 2020 2020 6667 3d22 6772 6565          fg="gree
-00017d70: 6e22 2c0a 2020 2020 2020 2020 2020 2020  n",.            
-00017d80: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00017d90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00017da0: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
-00017db0: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
-00017dc0: 2020 2020 2020 2020 2066 2246 6169 6c65           f"Faile
-00017dd0: 6420 746f 2063 6163 6865 2064 6174 6120  d to cache data 
-00017de0: 666f 7220 736f 6e67 207b 736f 6e67 5f6e  for song {song_n
-00017df0: 616d 657d 2077 6974 6820 4944 207b 736f  ame} with ID {so
-00017e00: 6e67 5f69 647d 2e20 4d61 7962 6520 796f  ng_id}. Maybe yo
-00017e10: 7520 6861 7665 6e27 7420 696e 7374 616c  u haven't instal
-00017e20: 6c65 6420 7468 6520 7265 7175 6972 6564  led the required
-00017e30: 2064 6570 656e 6465 6e63 6965 7320 286c   dependencies (l
-00017e40: 6962 726f 7361 2c20 6e75 6d62 612c 206e  ibrosa, numba, n
-00017e50: 756d 7079 293f 222c 0a20 2020 2020 2020  umpy)?",.       
-00017e60: 2020 2020 2020 2020 2020 2020 2066 673d               fg=
-00017e70: 2272 6564 222c 0a20 2020 2020 2020 2020  "red",.         
-00017e80: 2020 2020 2020 2029 0a0a 0a40 636c 692e         )...@cli.
-00017e90: 636f 6d6d 616e 6428 290a 4063 6c69 636b  command().@click
-00017ea0: 2e61 7267 756d 656e 7428 2273 6f6e 675f  .argument("song_
-00017eb0: 6964 222c 2074 7970 653d 696e 742c 2072  id", type=int, r
-00017ec0: 6571 7569 7265 643d 5472 7565 290a 4063  equired=True).@c
-00017ed0: 6c69 636b 2e61 7267 756d 656e 7428 2270  lick.argument("p
-00017ee0: 6169 7273 222c 2074 7970 653d 7374 722c  airs", type=str,
-00017ef0: 2072 6571 7569 7265 643d 4661 6c73 6529   required=False)
-00017f00: 0a64 6566 206d 6574 6164 6174 6128 736f  .def metadata(so
-00017f10: 6e67 5f69 642c 2070 6169 7273 293a 0a20  ng_id, pairs):. 
-00017f20: 2020 2022 2222 0a20 2020 2049 6620 6e6f     """.    If no
-00017f30: 2050 4149 5253 2061 7265 2070 6173 7365   PAIRS are passe
-00017f40: 642c 2070 7269 6e74 7320 7468 6520 6d65  d, prints the me
-00017f50: 7461 6461 7461 2066 6f72 2074 6865 2073  tadata for the s
-00017f60: 6f6e 6720 7769 7468 2049 4420 534f 4e47  ong with ID SONG
-00017f70: 5f49 442e 0a0a 2020 2020 4966 2050 4149  _ID...    If PAI
-00017f80: 5253 2061 7265 2070 6173 7365 642c 2073  RS are passed, s
-00017f90: 6574 7320 7468 6520 6d65 7461 6461 7461  ets the metadata
-00017fa0: 2066 6f72 2074 6865 2073 6f6e 6720 7769   for the song wi
-00017fb0: 7468 2049 4420 534f 4e47 5f49 4420 746f  th ID SONG_ID to
-00017fc0: 2074 6865 0a20 2020 206b 6579 2d76 616c   the.    key-val
-00017fd0: 7565 2070 6169 7273 2069 6e20 5041 4952  ue pairs in PAIR
-00017fe0: 532e 2050 4149 5253 2073 686f 756c 6420  S. PAIRS should 
-00017ff0: 6265 2061 2073 7472 696e 6720 6f66 2074  be a string of t
-00018000: 6865 2066 6f72 6d0a 2020 2020 276b 6579  he form.    'key
-00018010: 313a 7661 6c75 6531 7c6b 6579 323a 7661  1:value1|key2:va
-00018020: 6c75 6532 7c2e 2e2e 272e 0a0a 2020 2020  lue2|...'...    
-00018030: 506f 7373 6962 6c65 2065 6469 7461 626c  Possible editabl
-00018040: 6520 6d65 7461 6461 7461 206b 6579 7320  e metadata keys 
-00018050: 6172 653a 2061 6c62 756d 2c20 616c 6275  are: album, albu
-00018060: 6d61 7274 6973 742c 2061 7274 6973 742c  martist, artist,
-00018070: 2061 7274 776f 726b 2c0a 2020 2020 636f   artwork,.    co
-00018080: 6d6d 656e 742c 2063 6f6d 7069 6c61 7469  mment, compilati
-00018090: 6f6e 2c20 636f 6d70 6f73 6572 2c20 6469  on, composer, di
-000180a0: 7363 6e75 6d62 6572 2c20 6765 6e72 652c  scnumber, genre,
-000180b0: 206c 7972 6963 732c 2074 6f74 616c 6469   lyrics, totaldi
-000180c0: 7363 732c 0a20 2020 2074 6f74 616c 7472  scs,.    totaltr
-000180d0: 6163 6b73 2c20 7472 6163 6b6e 756d 6265  acks, tracknumbe
-000180e0: 722c 2074 7261 636b 7469 746c 652c 2079  r, tracktitle, y
-000180f0: 6561 722c 2069 7372 630a 0a20 2020 204b  ear, isrc..    K
-00018100: 6579 7320 6172 6520 6e6f 7420 6361 7365  eys are not case
-00018110: 2073 656e 7369 7469 7665 2061 6e64 2063   sensitive and c
-00018120: 616e 2063 6f6e 7461 696e 2061 7262 6974  an contain arbit
-00018130: 7261 7279 2077 6869 7465 7370 6163 652c  rary whitespace,
-00018140: 2027 2d27 2c20 616e 640a 2020 2020 275f   '-', and.    '_
-00018150: 2720 6368 6172 6163 7465 7273 2e20 496e  ' characters. In
-00018160: 206f 7468 6572 2077 6f72 6473 2c20 2741   other words, 'A
-00018170: 6c62 756d 2041 7274 6973 7427 2c20 2761  lbum Artist', 'a
-00018180: 6c62 756d 2d61 7274 6973 7427 2c20 616e  lbum-artist', an
-00018190: 640a 2020 2020 2761 6c62 756d 5f61 7274  d.    'album_art
-000181a0: 6973 7427 2061 7265 2061 6c6c 2073 796e  ist' are all syn
-000181b0: 6f6e 796d 7320 666f 7220 2761 6c62 756d  onyms for 'album
-000181c0: 6172 7469 7374 272e 2041 6c73 6f2c 2027  artist'. Also, '
-000181d0: 6469 736b 2720 6973 0a20 2020 2073 796e  disk' is.    syn
-000181e0: 6f6e 796d 6f75 7320 7769 7468 2027 6469  onymous with 'di
-000181f0: 7363 272e 0a20 2020 2022 2222 0a0a 2020  sc'..    """..  
-00018200: 2020 7769 7468 206f 7065 6e28 534f 4e47    with open(SONG
-00018210: 535f 494e 464f 5f50 4154 482c 2022 7222  S_INFO_PATH, "r"
-00018220: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-00018230: 3822 2920 6173 2073 6f6e 6773 5f66 696c  8") as songs_fil
-00018240: 653a 0a20 2020 2020 2020 206c 696e 6573  e:.        lines
-00018250: 203d 2073 6f6e 6773 5f66 696c 652e 7265   = songs_file.re
-00018260: 6164 6c69 6e65 7328 290a 0a20 2020 2020  adlines()..     
-00018270: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00018280: 6528 6c65 6e28 6c69 6e65 7329 293a 0a20  e(len(lines)):. 
-00018290: 2020 2020 2020 2020 2020 2064 6574 6169             detai
-000182a0: 6c73 203d 206c 696e 6573 5b69 5d2e 7374  ls = lines[i].st
-000182b0: 7269 7028 292e 7370 6c69 7428 227c 2229  rip().split("|")
-000182c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000182d0: 696e 7428 6465 7461 696c 735b 305d 2920  int(details[0]) 
-000182e0: 3d3d 2073 6f6e 675f 6964 3a0a 2020 2020  == song_id:.    
-000182f0: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-00018300: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-00018310: 6a6f 696e 2853 4f4e 4753 5f44 4952 2c20  join(SONGS_DIR, 
-00018320: 6465 7461 696c 735b 315d 290a 2020 2020  details[1]).    
-00018330: 2020 2020 2020 2020 2020 2020 736f 6e67              song
-00018340: 5f6e 616d 6520 3d20 6465 7461 696c 735b  _name = details[
-00018350: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
-00018360: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00018370: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00018380: 2020 2063 6c69 636b 2e73 6563 686f 280a     click.secho(.
+00011f00: 2020 2020 2020 2064 656c 2074 6167 735b         del tags[
+00011f10: 6a5d 0a20 2020 2020 2020 2020 2020 2020  j].             
+00011f20: 2020 2064 6574 6169 6c73 5b32 5d20 3d20     details[2] = 
+00011f30: 222c 222e 6a6f 696e 2874 6167 7329 0a20  ",".join(tags). 
+00011f40: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00011f50: 696e 6573 5b69 5d20 3d20 227c 222e 6a6f  ines[i] = "|".jo
+00011f60: 696e 2864 6574 6169 6c73 290a 0a20 2020  in(details)..   
+00011f70: 2020 2020 2077 6974 6820 6f70 656e 2853       with open(S
+00011f80: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
+00011f90: 2277 222c 2065 6e63 6f64 696e 673d 2275  "w", encoding="u
+00011fa0: 7466 2d38 2229 2061 7320 736f 6e67 735f  tf-8") as songs_
+00011fb0: 6669 6c65 3a0a 2020 2020 2020 2020 2020  file:.          
+00011fc0: 2020 736f 6e67 735f 6669 6c65 2e77 7269    songs_file.wri
+00011fd0: 7465 2822 5c6e 222e 6a6f 696e 286c 696e  te("\n".join(lin
+00011fe0: 6573 2929 0a0a 2020 2020 2020 2020 636c  es))..        cl
+00011ff0: 6963 6b2e 7365 6368 6f28 0a20 2020 2020  ick.secho(.     
+00012000: 2020 2020 2020 2066 2244 656c 6574 6564         f"Deleted
+00012010: 2061 6c6c 206f 6363 7572 7265 6e63 6573   all occurrences
+00012020: 206f 6620 7b6c 656e 2874 6167 735f 746f   of {len(tags_to
+00012030: 5f72 656d 6f76 6529 7d20 7461 6728 7329  _remove)} tag(s)
+00012040: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00012050: 6667 3d22 6772 6565 6e22 2c0a 2020 2020  fg="green",.    
+00012060: 2020 2020 290a 0a0a 4063 6c69 2e63 6f6d      )...@cli.com
+00012070: 6d61 6e64 286e 616d 653d 2274 6167 2229  mand(name="tag")
+00012080: 0a40 636c 6963 6b2e 6172 6775 6d65 6e74  .@click.argument
+00012090: 2822 736f 6e67 5f69 6473 222c 2074 7970  ("song_ids", typ
+000120a0: 653d 636c 6963 6b2e 494e 542c 2072 6571  e=click.INT, req
+000120b0: 7569 7265 643d 5472 7565 2c20 6e61 7267  uired=True, narg
+000120c0: 733d 2d31 290a 4063 6c69 636b 2e6f 7074  s=-1).@click.opt
+000120d0: 696f 6e28 0a20 2020 2022 2d74 222c 0a20  ion(.    "-t",. 
+000120e0: 2020 2022 2d2d 7461 6722 2c0a 2020 2020     "--tag",.    
+000120f0: 2274 6167 7322 2c0a 2020 2020 6865 6c70  "tags",.    help
+00012100: 3d22 5461 6773 2074 6f20 6164 642e 222c  ="Tags to add.",
+00012110: 0a20 2020 206d 756c 7469 706c 653d 5472  .    multiple=Tr
+00012120: 7565 2c0a 290a 6465 6620 7461 675f 2873  ue,.).def tag_(s
+00012130: 6f6e 675f 6964 732c 2074 6167 7329 3a0a  ong_ids, tags):.
+00012140: 2020 2020 2222 2241 6464 2074 6167 7320      """Add tags 
+00012150: 746f 2061 2073 6f6e 6720 2870 6173 7365  to a song (passe
+00012160: 6420 6173 2049 4429 2e20 5461 6773 2063  d as ID). Tags c
+00012170: 616e 6e6f 7420 636f 6e74 6169 6e20 7468  annot contain th
+00012180: 6520 6368 6172 6163 7465 7273 0a20 2020  e characters.   
+00012190: 2027 2c27 206f 7220 277c 272e 2222 220a   ',' or '|'.""".
+000121a0: 2020 2020 736f 6e67 5f69 6473 203d 2073      song_ids = s
+000121b0: 6574 2873 6f6e 675f 6964 7329 0a20 2020  et(song_ids).   
+000121c0: 206e 756d 5f73 6f6e 6773 203d 206c 656e   num_songs = len
+000121d0: 2873 6f6e 675f 6964 7329 0a20 2020 2074  (song_ids).    t
+000121e0: 6167 7320 3d20 7365 7428 7461 6773 290a  ags = set(tags).
+000121f0: 2020 2020 666f 7220 7461 6720 696e 2074      for tag in t
+00012200: 6167 733a 0a20 2020 2020 2020 2069 6620  ags:.        if 
+00012210: 222c 2220 696e 2074 6167 206f 7220 227c  "," in tag or "|
+00012220: 2220 696e 2074 6167 3a0a 2020 2020 2020  " in tag:.      
+00012230: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
+00012240: 6f28 2254 6167 7320 6361 6e6e 6f74 2063  o("Tags cannot c
+00012250: 6f6e 7461 696e 2027 2c27 206f 7220 277c  ontain ',' or '|
+00012260: 272e 222c 2066 673d 2272 6564 2229 0a20  '.", fg="red"). 
+00012270: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00012280: 6e0a 2020 2020 6966 2074 6167 733a 0a20  n.    if tags:. 
+00012290: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
+000122a0: 6520 3d20 6f70 656e 2853 4f4e 4753 5f49  e = open(SONGS_I
+000122b0: 4e46 4f5f 5041 5448 2c20 2272 222c 2065  NFO_PATH, "r", e
+000122c0: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
+000122d0: 0a20 2020 2020 2020 206c 696e 6573 203d  .        lines =
+000122e0: 2073 6f6e 6773 5f66 696c 652e 7265 6164   songs_file.read
+000122f0: 2829 2e73 706c 6974 6c69 6e65 7328 290a  ().splitlines().
+00012300: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00012310: 2072 616e 6765 286c 656e 286c 696e 6573   range(len(lines
+00012320: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00012330: 6465 7461 696c 7320 3d20 6c69 6e65 735b  details = lines[
+00012340: 695d 2e73 7472 6970 2829 2e73 706c 6974  i].strip().split
+00012350: 2822 7c22 290a 2020 2020 2020 2020 2020  ("|").          
+00012360: 2020 736f 6e67 5f69 6420 3d20 696e 7428    song_id = int(
+00012370: 6465 7461 696c 735b 305d 290a 2020 2020  details[0]).    
+00012380: 2020 2020 2020 2020 6966 2073 6f6e 675f          if song_
+00012390: 6964 2069 6e20 736f 6e67 5f69 6473 3a0a  id in song_ids:.
+000123a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000123b0: 736f 6e67 5f69 6473 2e72 656d 6f76 6528  song_ids.remove(
+000123c0: 736f 6e67 5f69 6429 0a0a 2020 2020 2020  song_id)..      
+000123d0: 2020 2020 2020 2020 2020 6966 2064 6574            if det
+000123e0: 6169 6c73 5b32 5d3a 0a20 2020 2020 2020  ails[2]:.       
+000123f0: 2020 2020 2020 2020 2020 2020 206e 6577               new
+00012400: 5f74 6167 7320 3d20 6465 7461 696c 735b  _tags = details[
+00012410: 325d 2e73 706c 6974 2822 2c22 290a 2020  2].split(",").  
+00012420: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00012430: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00012440: 2020 2020 2020 2020 6e65 775f 7461 6773          new_tags
+00012450: 203d 205b 5d0a 2020 2020 2020 2020 2020   = [].          
+00012460: 2020 2020 2020 6e65 775f 7461 6773 202b        new_tags +
+00012470: 3d20 5b74 6167 2066 6f72 2074 6167 2069  = [tag for tag i
+00012480: 6e20 7461 6773 2069 6620 7461 6720 6e6f  n tags if tag no
+00012490: 7420 696e 206e 6577 5f74 6167 735d 0a20  t in new_tags]. 
+000124a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000124b0: 6574 6169 6c73 5b32 5d20 3d20 222c 222e  etails[2] = ",".
+000124c0: 6a6f 696e 286e 6577 5f74 6167 7329 0a20  join(new_tags). 
+000124d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000124e0: 696e 6573 5b69 5d20 3d20 227c 222e 6a6f  ines[i] = "|".jo
+000124f0: 696e 2864 6574 6169 6c73 290a 2020 2020  in(details).    
+00012500: 2020 2020 736f 6e67 735f 6669 6c65 2e63      songs_file.c
+00012510: 6c6f 7365 2829 0a0a 2020 2020 2020 2020  lose()..        
+00012520: 736f 6e67 735f 6669 6c65 203d 206f 7065  songs_file = ope
+00012530: 6e28 534f 4e47 535f 494e 464f 5f50 4154  n(SONGS_INFO_PAT
+00012540: 482c 2022 7722 2c20 656e 636f 6469 6e67  H, "w", encoding
+00012550: 3d22 7574 662d 3822 290a 2020 2020 2020  ="utf-8").      
+00012560: 2020 736f 6e67 735f 6669 6c65 2e77 7269    songs_file.wri
+00012570: 7465 2822 5c6e 222e 6a6f 696e 286c 696e  te("\n".join(lin
+00012580: 6573 2929 0a20 2020 2020 2020 2073 6f6e  es)).        son
+00012590: 6773 5f66 696c 652e 636c 6f73 6528 290a  gs_file.close().
+000125a0: 0a20 2020 2020 2020 2069 6620 736f 6e67  .        if song
+000125b0: 5f69 6473 3a0a 2020 2020 2020 2020 2020  _ids:.          
+000125c0: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
+000125d0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000125e0: 2243 6f75 6c64 206e 6f74 2066 696e 6420  "Could not find 
+000125f0: 736f 6e67 2873 2920 7769 7468 2049 4428  song(s) with ID(
+00012600: 7329 207b 272c 2027 2e6a 6f69 6e28 6d61  s) {', '.join(ma
+00012610: 7028 7374 722c 2073 6f6e 675f 6964 7329  p(str, song_ids)
+00012620: 297d 2e22 2c0a 2020 2020 2020 2020 2020  )}.",.          
+00012630: 2020 2020 2020 6667 3d22 7265 6422 2c0a        fg="red",.
+00012640: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00012650: 2020 2020 2020 2020 2020 6966 206c 656e            if len
+00012660: 2873 6f6e 675f 6964 7329 203d 3d20 6e75  (song_ids) == nu
+00012670: 6d5f 736f 6e67 733a 0a20 2020 2020 2020  m_songs:.       
+00012680: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00012690: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
+000126a0: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+000126b0: 2066 2241 6464 6564 207b 6c65 6e28 7461   f"Added {len(ta
+000126c0: 6773 297d 2074 6167 2873 2920 746f 207b  gs)} tag(s) to {
+000126d0: 6e75 6d5f 736f 6e67 7320 2d20 6c65 6e28  num_songs - len(
+000126e0: 736f 6e67 5f69 6473 297d 2073 6f6e 6728  song_ids)} song(
+000126f0: 7329 2e22 2c0a 2020 2020 2020 2020 2020  s).",.          
+00012700: 2020 6667 3d22 6772 6565 6e22 2c0a 2020    fg="green",.  
+00012710: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
+00012720: 3a0a 2020 2020 2020 2020 636c 6963 6b2e  :.        click.
+00012730: 7365 6368 6f28 224e 6f20 7461 6773 2070  secho("No tags p
+00012740: 6173 7365 642e 222c 2066 673d 2272 6564  assed.", fg="red
+00012750: 2229 0a0a 0a40 636c 692e 636f 6d6d 616e  ")...@cli.comman
+00012760: 6428 290a 4063 6c69 636b 2e61 7267 756d  d().@click.argum
+00012770: 656e 7428 2273 6f6e 675f 6964 7322 2c20  ent("song_ids", 
+00012780: 7479 7065 3d63 6c69 636b 2e49 4e54 2c20  type=click.INT, 
+00012790: 7265 7175 6972 6564 3d54 7275 652c 206e  required=True, n
+000127a0: 6172 6773 3d2d 3129 0a40 636c 6963 6b2e  args=-1).@click.
+000127b0: 6f70 7469 6f6e 280a 2020 2020 222d 7422  option(.    "-t"
+000127c0: 2c0a 2020 2020 222d 2d74 6167 222c 0a20  ,.    "--tag",. 
+000127d0: 2020 2022 7461 6773 222c 0a20 2020 2068     "tags",.    h
+000127e0: 656c 703d 2254 6167 7320 746f 2072 656d  elp="Tags to rem
+000127f0: 6f76 652e 222c 0a20 2020 206d 756c 7469  ove.",.    multi
+00012800: 706c 653d 5472 7565 2c0a 290a 4063 6c69  ple=True,.).@cli
+00012810: 636b 2e6f 7074 696f 6e28 222d 412f 2d6e  ck.option("-A/-n
+00012820: 4122 2c20 222d 2d61 6c6c 2f2d 2d6e 6f2d  A", "--all/--no-
+00012830: 616c 6c22 2c20 2261 6c6c 5f22 2c20 6465  all", "all_", de
+00012840: 6661 756c 743d 4661 6c73 6529 0a64 6566  fault=False).def
+00012850: 2075 6e74 6167 2873 6f6e 675f 6964 732c   untag(song_ids,
+00012860: 2074 6167 732c 2061 6c6c 5f29 3a0a 2020   tags, all_):.  
+00012870: 2020 2222 2252 656d 6f76 6520 7461 6773    """Remove tags
+00012880: 2066 726f 6d20 6120 7370 6563 6966 6963   from a specific
+00012890: 2073 6f6e 6720 2870 6173 7365 6420 6173   song (passed as
+000128a0: 2049 4429 2e20 5461 6773 2074 6861 7420   ID). Tags that 
+000128b0: 7468 6520 736f 6e67 0a20 2020 2064 6f65  the song.    doe
+000128c0: 736e 2774 2068 6176 6520 7769 6c6c 2062  sn't have will b
+000128d0: 6520 6967 6e6f 7265 642e 0a0a 2020 2020  e ignored...    
+000128e0: 5061 7373 696e 6720 7468 6520 272d 412f  Passing the '-A/
+000128f0: 2d2d 616c 6c27 2066 6c61 6720 7769 6c6c  --all' flag will
+00012900: 2072 656d 6f76 6520 616c 6c20 7461 6773   remove all tags
+00012910: 2066 726f 6d20 7468 6520 736f 6e67 2c20   from the song, 
+00012920: 756e 6c65 7373 2054 4147 530a 2020 2020  unless TAGS.    
+00012930: 6973 2070 6173 7365 6420 2869 6e20 7768  is passed (in wh
+00012940: 6963 6820 6361 7365 2074 6865 2066 6c61  ich case the fla
+00012950: 6720 6973 2069 676e 6f72 6564 292e 2222  g is ignored).""
+00012960: 220a 2020 2020 736f 6e67 5f69 6473 203d  ".    song_ids =
+00012970: 2073 6574 2873 6f6e 675f 6964 7329 0a20   set(song_ids). 
+00012980: 2020 206e 756d 5f73 6f6e 6773 203d 206c     num_songs = l
+00012990: 656e 2873 6f6e 675f 6964 7329 0a20 2020  en(song_ids).   
+000129a0: 2074 6167 7320 3d20 7365 7428 7461 6773   tags = set(tags
+000129b0: 290a 2020 2020 6966 2074 6167 733a 0a20  ).    if tags:. 
+000129c0: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
+000129d0: 6520 3d20 6f70 656e 2853 4f4e 4753 5f49  e = open(SONGS_I
+000129e0: 4e46 4f5f 5041 5448 2c20 2272 222c 2065  NFO_PATH, "r", e
+000129f0: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
+00012a00: 0a20 2020 2020 2020 206c 696e 6573 203d  .        lines =
+00012a10: 2073 6f6e 6773 5f66 696c 652e 7265 6164   songs_file.read
+00012a20: 2829 2e73 706c 6974 6c69 6e65 7328 290a  ().splitlines().
+00012a30: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00012a40: 2072 616e 6765 286c 656e 286c 696e 6573   range(len(lines
+00012a50: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00012a60: 6465 7461 696c 7320 3d20 6c69 6e65 735b  details = lines[
+00012a70: 695d 2e73 7472 6970 2829 2e73 706c 6974  i].strip().split
+00012a80: 2822 7c22 290a 2020 2020 2020 2020 2020  ("|").          
+00012a90: 2020 736f 6e67 5f69 6420 3d20 696e 7428    song_id = int(
+00012aa0: 6465 7461 696c 735b 305d 290a 2020 2020  details[0]).    
+00012ab0: 2020 2020 2020 2020 6966 2073 6f6e 675f          if song_
+00012ac0: 6964 2069 6e20 736f 6e67 5f69 6473 3a0a  id in song_ids:.
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ae0: 736f 6e67 5f69 6473 2e72 656d 6f76 6528  song_ids.remove(
+00012af0: 736f 6e67 5f69 6429 0a0a 2020 2020 2020  song_id)..      
+00012b00: 2020 2020 2020 2020 2020 7461 6773 5f74            tags_t
+00012b10: 6f5f 6b65 6570 203d 205b 0a20 2020 2020  o_keep = [.     
+00012b20: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00012b30: 6167 2066 6f72 2074 6167 2069 6e20 6465  ag for tag in de
+00012b40: 7461 696c 735b 325d 2e73 706c 6974 2822  tails[2].split("
+00012b50: 2c22 2920 6966 2074 6167 206e 6f74 2069  ,") if tag not i
+00012b60: 6e20 7461 6773 0a20 2020 2020 2020 2020  n tags.         
+00012b70: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00012b80: 2020 2020 2020 2020 206c 696e 6573 5b69           lines[i
+00012b90: 5d20 3d20 227c 222e 6a6f 696e 280a 2020  ] = "|".join(.  
+00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012bb0: 2020 6465 7461 696c 735b 3a32 5d20 2b20    details[:2] + 
+00012bc0: 5b22 2c22 2e6a 6f69 6e28 7461 6773 5f74  [",".join(tags_t
+00012bd0: 6f5f 6b65 6570 295d 202b 2064 6574 6169  o_keep)] + detai
+00012be0: 6c73 5b33 3a5d 0a20 2020 2020 2020 2020  ls[3:].         
+00012bf0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00012c00: 2073 6f6e 6773 5f66 696c 652e 636c 6f73   songs_file.clos
+00012c10: 6528 290a 0a20 2020 2020 2020 2073 6f6e  e()..        son
+00012c20: 6773 5f66 696c 6520 3d20 6f70 656e 2853  gs_file = open(S
+00012c30: 4f4e 4753 5f49 4e46 4f5f 5041 5448 2c20  ONGS_INFO_PATH, 
+00012c40: 2277 222c 2065 6e63 6f64 696e 673d 2275  "w", encoding="u
+00012c50: 7466 2d38 2229 0a20 2020 2020 2020 2073  tf-8").        s
+00012c60: 6f6e 6773 5f66 696c 652e 7772 6974 6528  ongs_file.write(
+00012c70: 225c 6e22 2e6a 6f69 6e28 6c69 6e65 7329  "\n".join(lines)
+00012c80: 290a 2020 2020 2020 2020 736f 6e67 735f  ).        songs_
+00012c90: 6669 6c65 2e63 6c6f 7365 2829 0a0a 2020  file.close()..  
+00012ca0: 2020 2020 2020 6966 2073 6f6e 675f 6964        if song_id
+00012cb0: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+00012cc0: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
+00012cd0: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
+00012ce0: 756c 6420 6e6f 7420 6669 6e64 2073 6f6e  uld not find son
+00012cf0: 6728 7329 2077 6974 6820 4944 2873 2920  g(s) with ID(s) 
+00012d00: 7b27 2c20 272e 6a6f 696e 286d 6170 2873  {', '.join(map(s
+00012d10: 7472 2c20 736f 6e67 5f69 6473 2929 7d2e  tr, song_ids))}.
+00012d20: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00012d30: 2020 2066 673d 2272 6564 222c 0a20 2020     fg="red",.   
+00012d40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00012d50: 2020 2020 2020 2069 6620 6c65 6e28 736f         if len(so
+00012d60: 6e67 5f69 6473 2920 3d3d 206e 756d 5f73  ng_ids) == num_s
+00012d70: 6f6e 6773 3a0a 2020 2020 2020 2020 2020  ongs:.          
+00012d80: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
+00012d90: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
+00012da0: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+00012db0: 5265 6d6f 7665 6420 616e 7920 6f63 6375  Removed any occu
+00012dc0: 7272 656e 6365 7320 6f66 207b 6c65 6e28  rrences of {len(
+00012dd0: 7461 6773 297d 2074 6167 2873 2920 6672  tags)} tag(s) fr
+00012de0: 6f6d 207b 6e75 6d5f 736f 6e67 7320 2d20  om {num_songs - 
+00012df0: 6c65 6e28 736f 6e67 5f69 6473 297d 2073  len(song_ids)} s
+00012e00: 6f6e 6728 7329 2e22 2c0a 2020 2020 2020  ong(s).",.      
+00012e10: 2020 2020 2020 6667 3d22 6772 6565 6e22        fg="green"
+00012e20: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00012e30: 656c 7365 3a0a 2020 2020 2020 2020 6966  else:.        if
+00012e40: 206e 6f74 2061 6c6c 5f3a 0a20 2020 2020   not all_:.     
+00012e50: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
+00012e60: 686f 280a 2020 2020 2020 2020 2020 2020  ho(.            
+00012e70: 2020 2020 224e 6f20 7461 6773 2070 6173      "No tags pas
+00012e80: 7365 64e2 8094 746f 2072 656d 6f76 6520  sed...to remove 
+00012e90: 616c 6c20 7461 6773 2c20 7061 7373 2074  all tags, pass t
+00012ea0: 6865 2027 2d41 2f2d 2d61 6c6c 2720 666c  he '-A/--all' fl
+00012eb0: 6167 2e22 2c0a 2020 2020 2020 2020 2020  ag.",.          
+00012ec0: 2020 2020 2020 6667 3d22 7265 6422 2c0a        fg="red",.
+00012ed0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00012ee0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00012ef0: 2020 2020 2020 2020 736f 6e67 735f 6669          songs_fi
+00012f00: 6c65 203d 206f 7065 6e28 534f 4e47 535f  le = open(SONGS_
+00012f10: 494e 464f 5f50 4154 482c 2022 7222 2c20  INFO_PATH, "r", 
+00012f20: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+00012f30: 290a 2020 2020 2020 2020 2020 2020 6c69  ).            li
+00012f40: 6e65 7320 3d20 736f 6e67 735f 6669 6c65  nes = songs_file
+00012f50: 2e72 6561 6428 292e 7370 6c69 746c 696e  .read().splitlin
+00012f60: 6573 2829 0a20 2020 2020 2020 2020 2020  es().           
+00012f70: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00012f80: 6c65 6e28 6c69 6e65 7329 293a 0a20 2020  len(lines)):.   
+00012f90: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+00012fa0: 6520 3d20 6c69 6e65 735b 695d 0a20 2020  e = lines[i].   
+00012fb0: 2020 2020 2020 2020 2020 2020 2064 6574               det
+00012fc0: 6169 6c73 203d 206c 696e 652e 7374 7269  ails = line.stri
+00012fd0: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
+00012fe0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00012ff0: 6620 696e 7428 6465 7461 696c 735b 305d  f int(details[0]
+00013000: 2920 696e 2073 6f6e 675f 6964 733a 0a20  ) in song_ids:. 
+00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013020: 2020 206c 696e 6573 5b69 5d20 3d20 227c     lines[i] = "|
+00013030: 222e 6a6f 696e 2864 6574 6169 6c73 5b3a  ".join(details[:
+00013040: 325d 202b 205b 2222 5d20 2b20 6465 7461  2] + [""] + deta
+00013050: 696c 735b 333a 5d29 0a20 2020 2020 2020  ils[3:]).       
+00013060: 2020 2020 2073 6f6e 6773 5f66 696c 652e       songs_file.
+00013070: 636c 6f73 6528 290a 0a20 2020 2020 2020  close()..       
+00013080: 2020 2020 2073 6f6e 6773 5f66 696c 6520       songs_file 
+00013090: 3d20 6f70 656e 2853 4f4e 4753 5f49 4e46  = open(SONGS_INF
+000130a0: 4f5f 5041 5448 2c20 2277 222c 2065 6e63  O_PATH, "w", enc
+000130b0: 6f64 696e 673d 2275 7466 2d38 2229 0a20  oding="utf-8"). 
+000130c0: 2020 2020 2020 2020 2020 2073 6f6e 6773             songs
+000130d0: 5f66 696c 652e 7772 6974 6528 225c 6e22  _file.write("\n"
+000130e0: 2e6a 6f69 6e28 6c69 6e65 7329 290a 2020  .join(lines)).  
+000130f0: 2020 2020 2020 2020 2020 736f 6e67 735f            songs_
+00013100: 6669 6c65 2e63 6c6f 7365 2829 0a0a 2020  file.close()..  
+00013110: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+00013120: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
+00013130: 2020 2020 2020 2066 2252 656d 6f76 6564         f"Removed
+00013140: 207b 6c65 6e28 7461 6773 297d 2074 6167   {len(tags)} tag
+00013150: 2873 2920 6672 6f6d 207b 6c65 6e28 736f  (s) from {len(so
+00013160: 6e67 5f69 6473 297d 2073 6f6e 6728 7329  ng_ids)} song(s)
+00013170: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00013180: 2020 2020 6667 3d22 6772 6565 6e22 2c0a      fg="green",.
+00013190: 2020 2020 2020 2020 2020 2020 290a 0a0a              )...
+000131a0: 4063 6c69 2e63 6f6d 6d61 6e64 2829 0a40  @cli.command().@
+000131b0: 636c 6963 6b2e 6172 6775 6d65 6e74 2822  click.argument("
+000131c0: 7461 6773 222c 206e 6172 6773 3d2d 3129  tags", nargs=-1)
+000131d0: 0a40 636c 6963 6b2e 6f70 7469 6f6e 280a  .@click.option(.
+000131e0: 2020 2020 222d 7322 2c0a 2020 2020 222d      "-s",.    "-
+000131f0: 2d73 6875 6666 6c65 222c 0a20 2020 2022  -shuffle",.    "
+00013200: 7368 7566 666c 655f 222c 0a20 2020 2074  shuffle_",.    t
+00013210: 7970 653d 636c 6963 6b2e 496e 7452 616e  ype=click.IntRan
+00013220: 6765 2830 2c20 3229 2c0a 2020 2020 6865  ge(0, 2),.    he
+00013230: 6c70 3d22 303a 2073 6875 6666 6c65 206f  lp="0: shuffle o
+00013240: 6e63 652c 2031 3a20 7368 7566 666c 6520  nce, 1: shuffle 
+00013250: 6576 6572 7920 6c6f 6f70 2c20 323a 2073  every loop, 2: s
+00013260: 6875 6666 6c65 2065 7665 7279 206c 6f6f  huffle every loo
+00013270: 7020 6578 6365 7074 2066 6f72 2074 6865  p except for the
+00013280: 2066 6972 7374 206f 6e65 2e22 2c0a 290a   first one.",.).
+00013290: 4063 6c69 636b 2e6f 7074 696f 6e28 0a20  @click.option(. 
+000132a0: 2020 2022 2d52 2f2d 6e52 222c 0a20 2020     "-R/-nR",.   
+000132b0: 2022 2d2d 7265 7665 7273 652f 2d2d 6e6f   "--reverse/--no
+000132c0: 2d72 6576 6572 7365 222c 0a20 2020 2022  -reverse",.    "
+000132d0: 7265 7665 7273 6522 2c0a 2020 2020 6465  reverse",.    de
+000132e0: 6661 756c 743d 4661 6c73 652c 0a20 2020  fault=False,.   
+000132f0: 2068 656c 703d 2250 6c61 7920 736f 6e67   help="Play song
+00013300: 7320 696e 2072 6576 6572 7365 2028 6d6f  s in reverse (mo
+00013310: 7374 2072 6563 656e 746c 7920 6164 6465  st recently adde
+00013320: 6420 6669 7273 7429 2e22 2c0a 290a 4063  d first).",.).@c
+00013330: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
+00013340: 2022 2d6f 222c 0a20 2020 2022 2d2d 6f6e   "-o",.    "--on
+00013350: 6c79 222c 0a20 2020 2022 6f6e 6c79 222c  ly",.    "only",
+00013360: 0a20 2020 2074 7970 653d 636c 6963 6b2e  .    type=click.
+00013370: 494e 542c 0a20 2020 206d 756c 7469 706c  INT,.    multipl
+00013380: 653d 5472 7565 2c0a 2020 2020 6865 6c70  e=True,.    help
+00013390: 3d22 506c 6179 206f 6e6c 7920 7468 6973  ="Play only this
+000133a0: 2f74 6865 7365 2073 6f6e 6728 7329 2028  /these song(s) (
+000133b0: 6361 6e20 6265 2070 6173 7365 6420 6d75  can be passed mu
+000133c0: 6c74 6970 6c65 2074 696d 6573 2c20 652e  ltiple times, e.
+000133d0: 672e 2027 6d61 6573 7472 6f20 706c 6179  g. 'maestro play
+000133e0: 202d 6f20 3120 2d6f 2031 3727 292e 222c   -o 1 -o 17').",
+000133f0: 0a29 0a40 636c 6963 6b2e 6f70 7469 6f6e  .).@click.option
+00013400: 280a 2020 2020 222d 7622 2c0a 2020 2020  (.    "-v",.    
+00013410: 222d 2d76 6f6c 756d 6522 2c0a 2020 2020  "--volume",.    
+00013420: 2276 6f6c 756d 6522 2c0a 2020 2020 7479  "volume",.    ty
+00013430: 7065 3d63 6c69 636b 2e49 6e74 5261 6e67  pe=click.IntRang
+00013440: 6528 302c 2031 3030 292c 0a20 2020 2064  e(0, 100),.    d
+00013450: 6566 6175 6c74 3d31 3030 2c0a 2020 2020  efault=100,.    
+00013460: 7368 6f77 5f64 6566 6175 6c74 3d54 7275  show_default=Tru
+00013470: 652c 0a29 0a40 636c 6963 6b2e 6f70 7469  e,.).@click.opti
+00013480: 6f6e 280a 2020 2020 222d 4c2f 2d6e 4c22  on(.    "-L/-nL"
+00013490: 2c0a 2020 2020 222d 2d6c 6f6f 702f 2d2d  ,.    "--loop/--
+000134a0: 6e6f 2d6c 6f6f 7022 2c0a 2020 2020 226c  no-loop",.    "l
+000134b0: 6f6f 7022 2c0a 2020 2020 6465 6661 756c  oop",.    defaul
+000134c0: 743d 4661 6c73 652c 0a20 2020 2068 656c  t=False,.    hel
+000134d0: 703d 224c 6f6f 7020 7468 6520 706c 6179  p="Loop the play
+000134e0: 6c69 7374 2e20 4361 6e20 6265 2074 6f67  list. Can be tog
+000134f0: 676c 6564 2077 6974 6820 276c 272e 222c  gled with 'l'.",
+00013500: 0a29 0a40 636c 6963 6b2e 6f70 7469 6f6e  .).@click.option
+00013510: 280a 2020 2020 222d 432f 2d6e 4322 2c0a  (.    "-C/-nC",.
+00013520: 2020 2020 222d 2d63 6c69 7073 2f2d 2d6e      "--clips/--n
+00013530: 6f2d 636c 6970 7322 2c0a 2020 2020 2263  o-clips",.    "c
+00013540: 6c69 7073 222c 0a20 2020 2064 6566 6175  lips",.    defau
+00013550: 6c74 3d46 616c 7365 2c0a 2020 2020 6865  lt=False,.    he
+00013560: 6c70 3d22 5374 6172 7420 696e 2063 6c69  lp="Start in cli
+00013570: 7020 6d6f 6465 2e20 4361 6e20 6265 2074  p mode. Can be t
+00013580: 6f67 676c 6564 2077 6974 6820 2763 272e  oggled with 'c'.
+00013590: 222c 0a29 0a40 636c 6963 6b2e 6f70 7469  ",.).@click.opti
+000135a0: 6f6e 280a 2020 2020 222d 442f 2d6e 4422  on(.    "-D/-nD"
+000135b0: 2c0a 2020 2020 222d 2d64 6973 636f 7264  ,.    "--discord
+000135c0: 2f2d 2d6e 6f2d 6469 7363 6f72 6422 2c0a  /--no-discord",.
+000135d0: 2020 2020 2264 6973 636f 7264 222c 0a20      "discord",. 
+000135e0: 2020 2064 6566 6175 6c74 3d46 616c 7365     default=False
+000135f0: 2c0a 2020 2020 6865 6c70 3d22 4469 7363  ,.    help="Disc
+00013600: 6f72 6420 7269 6368 2070 7265 7365 6e63  ord rich presenc
+00013610: 652e 2049 676e 6f72 6564 2069 6620 7265  e. Ignored if re
+00013620: 7175 6972 6564 2064 6570 656e 6465 6e63  quired dependenc
+00013630: 6965 7320 6172 6520 6e6f 7420 696e 7374  ies are not inst
+00013640: 616c 6c65 642e 2057 696c 6c20 6661 696c  alled. Will fail
+00013650: 2073 696c 656e 746c 7920 616e 6420 7265   silently and re
+00013660: 7472 7920 6576 6572 7920 7469 6d65 2074  try every time t
+00013670: 6865 2073 6f6e 6720 6368 616e 6765 7320  he song changes 
+00013680: 6966 2044 6973 636f 7264 2063 6f6e 6e65  if Discord conne
+00013690: 6374 696f 6e20 6661 696c 7320 2865 2e67  ction fails (e.g
+000136a0: 2e20 4469 7363 6f72 6420 6e6f 7420 6f70  . Discord not op
+000136b0: 656e 292e 222c 0a29 0a40 636c 6963 6b2e  en).",.).@click.
+000136c0: 6f70 7469 6f6e 280a 2020 2020 222d 4d2f  option(.    "-M/
+000136d0: 2d6e 4d22 2c0a 2020 2020 222d 2d6d 6174  -nM",.    "--mat
+000136e0: 6368 2d61 6c6c 2f2d 2d6e 6f2d 6d61 7463  ch-all/--no-matc
+000136f0: 682d 616c 6c22 2c0a 2020 2020 226d 6174  h-all",.    "mat
+00013700: 6368 5f61 6c6c 222c 0a20 2020 2064 6566  ch_all",.    def
+00013710: 6175 6c74 3d46 616c 7365 2c0a 2020 2020  ault=False,.    
+00013720: 6865 6c70 3d22 506c 6179 2073 6f6e 6773  help="Play songs
+00013730: 2074 6861 7420 6d61 7463 6820 616c 6c20   that match all 
+00013740: 7461 6773 2c20 6e6f 7420 616e 792e 222c  tags, not any.",
+00013750: 0a29 0a40 636c 6963 6b2e 6f70 7469 6f6e  .).@click.option
+00013760: 280a 2020 2020 222d 562f 2d6e 5622 2c0a  (.    "-V/-nV",.
+00013770: 2020 2020 222d 2d76 6973 7561 6c69 7a65      "--visualize
+00013780: 2f2d 2d6e 6f2d 7669 7375 616c 697a 6522  /--no-visualize"
+00013790: 2c0a 2020 2020 2276 6973 7561 6c69 7a65  ,.    "visualize
+000137a0: 222c 0a20 2020 2064 6566 6175 6c74 3d46  ",.    default=F
+000137b0: 616c 7365 2c0a 2020 2020 6865 6c70 3d22  alse,.    help="
+000137c0: 5669 7375 616c 697a 6520 7468 6520 736f  Visualize the so
+000137d0: 6e67 2062 6569 6e67 2070 6c61 7965 642e  ng being played.
+000137e0: 2049 676e 6f72 6564 2069 6620 7265 7175   Ignored if requ
+000137f0: 6972 6564 2064 6570 656e 6465 6e63 6965  ired dependencie
+00013800: 7320 6172 6520 6e6f 7420 696e 7374 616c  s are not instal
+00013810: 6c65 642e 222c 0a29 0a64 6566 2070 6c61  led.",.).def pla
+00013820: 7928 0a20 2020 2074 6167 732c 0a20 2020  y(.    tags,.   
+00013830: 2073 6875 6666 6c65 5f2c 0a20 2020 2072   shuffle_,.    r
+00013840: 6576 6572 7365 2c0a 2020 2020 6f6e 6c79  everse,.    only
+00013850: 2c0a 2020 2020 766f 6c75 6d65 2c0a 2020  ,.    volume,.  
+00013860: 2020 6c6f 6f70 2c0a 2020 2020 636c 6970    loop,.    clip
+00013870: 732c 0a20 2020 2064 6973 636f 7264 2c0a  s,.    discord,.
+00013880: 2020 2020 6d61 7463 685f 616c 6c2c 0a20      match_all,. 
+00013890: 2020 2076 6973 7561 6c69 7a65 2c0a 293a     visualize,.):
+000138a0: 0a20 2020 2022 2222 506c 6179 2079 6f75  .    """Play you
+000138b0: 7220 736f 6e67 732e 2049 6620 7461 6773  r songs. If tags
+000138c0: 2061 7265 2070 6173 7365 642c 2061 6e79   are passed, any
+000138d0: 2073 6f6e 6720 6d61 7463 6869 6e67 2061   song matching a
+000138e0: 6e79 2074 6167 2077 696c 6c20 6265 2069  ny tag will be i
+000138f0: 6e0a 2020 2020 796f 7572 2070 6c61 796c  n.    your playl
+00013900: 6973 742c 2075 6e6c 6573 7320 7468 6520  ist, unless the 
+00013910: 272d 4d2f 2d2d 6d61 7463 682d 616c 6c27  '-M/--match-all'
+00013920: 2066 6c61 6720 6973 2070 6173 7365 642c   flag is passed,
+00013930: 2069 6e20 7768 6963 6820 6361 7365 0a20   in which case. 
+00013940: 2020 2065 7665 7279 2074 6167 206d 7573     every tag mus
+00013950: 7420 6265 206d 6174 6368 6564 2e0a 0a20  t be matched... 
+00013960: 2020 205c 620a 2020 2020 5c78 3162 5b31     \b.    \x1b[1
+00013970: 6d53 5041 4345 5c78 3162 5b30 6d20 2074  mSPACE\x1b[0m  t
+00013980: 6f20 7061 7573 652f 706c 6179 0a20 2020  o pause/play.   
+00013990: 205c 7831 625b 316d 625c 7831 625b 306d   \x1b[1mb\x1b[0m
+000139a0: 2020 746f 2067 6f20 5b62 5d61 636b 2074    to go [b]ack t
+000139b0: 6f20 7072 6576 696f 7573 2073 6f6e 670a  o previous song.
+000139c0: 2020 2020 5c78 3162 5b31 6d72 5c78 3162      \x1b[1mr\x1b
+000139d0: 5b30 6d20 2074 6f20 5b72 5d65 706c 6179  [0m  to [r]eplay
+000139e0: 2073 6f6e 670a 2020 2020 5c78 3162 5b31   song.    \x1b[1
+000139f0: 6d6e 5c78 3162 5b30 6d20 2074 6f20 736b  mn\x1b[0m  to sk
+00013a00: 6970 2074 6f20 5b6e 5d65 7874 2073 6f6e  ip to [n]ext son
+00013a10: 670a 2020 2020 5c78 3162 5b31 6d6c 5c78  g.    \x1b[1ml\x
+00013a20: 3162 5b30 6d20 2074 6f20 5b6c 5d6f 6f70  1b[0m  to [l]oop
+00013a30: 2074 6865 2063 7572 7265 6e74 2073 6f6e   the current son
+00013a40: 6720 6f6e 6365 2028 276c 2720 696e 2073  g once ('l' in s
+00013a50: 7461 7475 7320 6261 7229 2e20 7072 6573  tatus bar). pres
+00013a60: 7320 6167 6169 6e20 746f 206c 6f6f 7020  s again to loop 
+00013a70: 696e 6669 6e69 7465 6c79 2028 274c 2720  infinitely ('L' 
+00013a80: 696e 2073 7461 7475 7320 6261 7229 2e20  in status bar). 
+00013a90: 7072 6573 7320 6f6e 6365 2061 6761 696e  press once again
+00013aa0: 2074 6f20 7475 726e 206f 6666 206c 6f6f   to turn off loo
+00013ab0: 7069 6e67 0a20 2020 205c 7831 625b 316d  ping.    \x1b[1m
+00013ac0: 635c 7831 625b 306d 2020 746f 2074 6f67  c\x1b[0m  to tog
+00013ad0: 676c 6520 5b63 5d6c 6970 206d 6f64 650a  gle [c]lip mode.
+00013ae0: 2020 2020 5c78 3162 5b31 6d76 5c78 3162      \x1b[1mv\x1b
+00013af0: 5b30 6d20 2074 6f20 746f 6767 6c65 205b  [0m  to toggle [
+00013b00: 765d 6973 7561 6c69 7a61 7469 6f6e 0a20  v]isualization. 
+00013b10: 2020 205c 7831 625b 316d 4c45 4654 5c78     \x1b[1mLEFT\x
+00013b20: 3162 5b30 6d20 2074 6f20 7265 7769 6e64  1b[0m  to rewind
+00013b30: 2035 730a 2020 2020 5c78 3162 5b31 6d52   5s.    \x1b[1mR
+00013b40: 4947 4854 5c78 3162 5b30 6d20 2074 6f20  IGHT\x1b[0m  to 
+00013b50: 6661 7374 2066 6f72 7761 7264 2035 730a  fast forward 5s.
+00013b60: 2020 2020 5c78 3162 5b31 6d5b 5c78 3162      \x1b[1m[\x1b
+00013b70: 5b30 6d20 2074 6f20 6465 6372 6561 7365  [0m  to decrease
+00013b80: 2076 6f6c 756d 650a 2020 2020 5c78 3162   volume.    \x1b
+00013b90: 5b31 6d5d 5c78 3162 5b30 6d20 2074 6f20  [1m]\x1b[0m  to 
+00013ba0: 696e 6372 6561 7365 2076 6f6c 756d 650a  increase volume.
+00013bb0: 2020 2020 5c78 3162 5b31 6d6d 5c78 3162      \x1b[1mm\x1b
+00013bc0: 5b30 6d20 2074 6f20 5b6d 5d75 7465 2f75  [0m  to [m]ute/u
+00013bd0: 6e6d 7574 650a 2020 2020 5c78 3162 5b31  nmute.    \x1b[1
+00013be0: 6d65 5c78 3162 5b30 6d20 2074 6f20 5b65  me\x1b[0m  to [e
+00013bf0: 5d6e 6420 7468 6520 736f 6e67 2070 6c61  ]nd the song pla
+00013c00: 7965 7220 6166 7465 7220 7468 6520 6375  yer after the cu
+00013c10: 7272 656e 7420 736f 6e67 2066 696e 6973  rrent song finis
+00013c20: 6865 7320 2869 6e64 6963 6174 6f72 2069  hes (indicator i
+00013c30: 6e20 7374 6174 7573 2062 6172 2c20 2765  n status bar, 'e
+00013c40: 2720 746f 2063 616e 6365 6c29 0a20 2020  ' to cancel).   
+00013c50: 205c 7831 625b 316d 715c 7831 625b 306d   \x1b[1mq\x1b[0m
+00013c60: 2020 746f 205b 715d 7569 7420 7468 6520    to [q]uit the 
+00013c70: 736f 6e67 2070 6c61 7965 7220 696d 6d65  song player imme
+00013c80: 6469 6174 656c 790a 2020 2020 5c78 3162  diately.    \x1b
+00013c90: 5b31 6d55 502f 444f 574e 5c78 3162 5b30  [1mUP/DOWN\x1b[0
+00013ca0: 6d20 2074 6f20 7363 726f 6c6c 2074 6872  m  to scroll thr
+00013cb0: 6f75 6768 2074 6865 2070 6c61 796c 6973  ough the playlis
+00013cc0: 7420 286d 6f75 7365 2073 6372 6f6c 6c69  t (mouse scrolli
+00013cd0: 6e67 2073 686f 756c 6420 616c 736f 2077  ng should also w
+00013ce0: 6f72 6b29 0a20 2020 205c 7831 625b 316d  ork).    \x1b[1m
+00013cf0: 705c 7831 625b 306d 2020 746f 2073 6e61  p\x1b[0m  to sna
+00013d00: 5b70 5d20 6261 636b 2074 6f20 7468 6520  [p] back to the 
+00013d10: 6375 7272 656e 746c 7920 706c 6179 696e  currently playin
+00013d20: 6720 736f 6e67 0a20 2020 205c 7831 625b  g song.    \x1b[
+00013d30: 316d 675c 7831 625b 306d 2020 746f 2067  1mg\x1b[0m  to g
+00013d40: 6f20 746f 2074 6865 206e 6578 7420 7061  o to the next pa
+00013d50: 5b67 5d65 2f6c 6f6f 7020 6f66 2074 6865  [g]e/loop of the
+00013d60: 2070 6c61 796c 6973 7420 2869 676e 6f72   playlist (ignor
+00013d70: 6564 2069 6620 6e6f 7420 7265 7065 6174  ed if not repeat
+00013d80: 696e 6720 706c 6179 6c69 7374 290a 2020  ing playlist).  
+00013d90: 2020 5c78 3162 5b31 6d42 4143 4b53 5041    \x1b[1mBACKSPA
+00013da0: 4345 2f44 454c 4554 455c 7831 625b 306d  CE/DELETE\x1b[0m
+00013db0: 2020 6465 6c65 7465 2074 6865 2073 656c    delete the sel
+00013dc0: 6563 7465 6420 286e 6f74 206e 6563 6573  ected (not neces
+00013dd0: 7361 7269 6c79 2063 7572 7265 6e74 6c79  sarily currently
+00013de0: 2070 6c61 7969 6e67 2129 2073 6f6e 6720   playing!) song 
+00013df0: 6672 6f6d 2074 6865 2071 7565 7565 0a20  from the queue. 
+00013e00: 2020 205c 7831 625b 316d 645c 7831 625b     \x1b[1md\x1b[
+00013e10: 306d 2020 746f 2074 6f67 676c 6520 5b44  0m  to toggle [D
+00013e20: 5d69 7363 6f72 6420 7269 6368 2070 7265  ]iscord rich pre
+00013e30: 7365 6e63 650a 2020 2020 5c78 3162 5b31  sence.    \x1b[1
+00013e40: 6d61 5c78 3162 5b30 6d20 2074 6f20 6164  ma\x1b[0m  to ad
+00013e50: 6420 6120 736f 6e67 2028 6279 2049 4429  d a song (by ID)
+00013e60: 2074 6f20 7468 6520 656e 6420 6f66 2074   to the end of t
+00013e70: 6865 2070 6c61 796c 6973 742e 204f 7065  he playlist. Ope
+00013e80: 6e73 2061 2070 726f 6d70 7420 746f 2065  ns a prompt to e
+00013e90: 6e74 6572 2074 6865 2049 443a 2045 4e54  nter the ID: ENT
+00013ea0: 4552 2074 6f20 636f 6e66 6972 6d2c 2045  ER to confirm, E
+00013eb0: 5343 2074 6f20 6361 6e63 656c 2e0a 2020  SC to cancel..  
+00013ec0: 2020 5c78 3162 5b31 6d69 5c78 3162 5b30    \x1b[1mi\x1b[0
+00013ed0: 6d20 2074 6f20 696e 7365 7274 2061 2073  m  to insert a s
+00013ee0: 6f6e 6720 2862 7920 4944 2920 696e 2074  ong (by ID) in t
+00013ef0: 6865 2070 6c61 796c 6973 7420 6166 7465  he playlist afte
+00013f00: 7220 7468 6520 7365 6c65 6374 6564 2073  r the selected s
+00013f10: 6f6e 672e 204f 7065 6e73 2061 2070 726f  ong. Opens a pro
+00013f20: 6d70 7420 6c69 6b65 2027 6127 2e0a 2020  mpt like 'a'..  
+00013f30: 2020 5c78 3162 5b31 6d74 5c78 3162 5b30    \x1b[1mt\x1b[0
+00013f40: 6d20 2074 6f20 6164 6420 6120 7461 6720  m  to add a tag 
+00013f50: 746f 2061 6c6c 2073 6f6e 6773 2069 6e20  to all songs in 
+00013f60: 7468 6520 706c 6179 6c69 7374 2e20 4f70  the playlist. Op
+00013f70: 656e 7320 6120 7072 6f6d 7074 2074 6f20  ens a prompt to 
+00013f80: 656e 7465 7220 7468 6520 7461 673a 2045  enter the tag: E
+00013f90: 4e54 4552 2074 6f20 636f 6e66 6972 6d2c  NTER to confirm,
+00013fa0: 2045 5343 2074 6f20 6361 6e63 656c 2e0a   ESC to cancel..
+00013fb0: 0a20 2020 205c 620a 2020 2020 736f 6e67  .    \b.    song
+00013fc0: 2063 6f6c 6f72 2069 6e64 6963 6174 6573   color indicates
+00013fd0: 206d 6f64 653a 0a20 2020 2020 2020 205c   mode:.        \
+00013fe0: 7831 625b 313b 3334 6d62 6c75 655c 7831  x1b[1;34mblue\x1
+00013ff0: 625b 306d 2020 2020 206e 6f72 6d61 6c0a  b[0m     normal.
+00014000: 2020 2020 2020 2020 5c78 3162 5b31 3b33          \x1b[1;3
+00014010: 336d 7965 6c6c 6f77 5c78 3162 5b30 6d20  3myellow\x1b[0m 
+00014020: 2020 6c6f 6f70 696e 6720 6375 7272 656e    looping curren
+00014030: 7420 736f 6e67 2028 6f6e 6365 206f 7220  t song (once or 
+00014040: 7265 7065 6174 6564 6c79 290a 0a20 2020  repeatedly)..   
+00014050: 205c 620a 2020 2020 7072 6f67 7265 7373   \b.    progress
+00014060: 2062 6172 2063 6f6c 6f72 2069 6e64 6963   bar color indic
+00014070: 6174 6573 2073 7461 7475 733a 0a20 2020  ates status:.   
+00014080: 2020 2020 205c 7831 625b 313b 3333 6d79       \x1b[1;33my
+00014090: 656c 6c6f 775c 7831 625b 306d 2020 206e  ellow\x1b[0m   n
+000140a0: 6f72 6d61 6c20 286f 7220 6375 7272 656e  ormal (or curren
+000140b0: 7420 736f 6e67 2064 6f65 736e 2774 2068  t song doesn't h
+000140c0: 6176 6520 6120 636c 6970 290a 2020 2020  ave a clip).    
+000140d0: 2020 2020 5c78 3162 5b31 3b33 356d 6d61      \x1b[1;35mma
+000140e0: 6765 6e74 615c 7831 625b 306d 2020 706c  genta\x1b[0m  pl
+000140f0: 6179 696e 6720 636c 6970 0a0a 2020 2020  aying clip..    
+00014100: 466f 7220 7468 6520 636f 6c6f 7220 7669  For the color vi
+00014110: 7369 6f6e 2064 6566 6963 6965 6e74 2c20  sion deficient, 
+00014120: 626f 7468 206d 6f64 6573 2061 6c73 6f20  both modes also 
+00014130: 6861 7665 2069 6e64 6963 6174 6f72 7320  have indicators 
+00014140: 696e 2074 6865 2073 7461 7475 7320 6261  in the status ba
+00014150: 722e 0a20 2020 2022 2222 0a20 2020 2070  r..    """.    p
+00014160: 6c61 796c 6973 7420 3d20 5b5d 0a0a 2020  laylist = []..  
+00014170: 2020 6966 206f 6e6c 793a 0a20 2020 2020    if only:.     
+00014180: 2020 206f 6e6c 7920 3d20 7365 7428 6f6e     only = set(on
+00014190: 6c79 290a 2020 2020 2020 2020 7769 7468  ly).        with
+000141a0: 206f 7065 6e28 534f 4e47 535f 494e 464f   open(SONGS_INFO
+000141b0: 5f50 4154 482c 2022 7222 2c20 656e 636f  _PATH, "r", enco
+000141c0: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
+000141d0: 2073 6f6e 6773 5f66 696c 653a 0a20 2020   songs_file:.   
+000141e0: 2020 2020 2020 2020 2066 6f72 206c 696e           for lin
+000141f0: 6520 696e 2073 6f6e 6773 5f66 696c 653a  e in songs_file:
+00014200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014210: 2064 6574 6169 6c73 203d 206c 696e 652e   details = line.
+00014220: 7374 7269 7028 292e 7370 6c69 7428 227c  strip().split("|
+00014230: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00014240: 2020 2073 6f6e 675f 6964 203d 2069 6e74     song_id = int
+00014250: 2864 6574 6169 6c73 5b30 5d29 0a20 2020  (details[0]).   
+00014260: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00014270: 736f 6e67 5f69 6420 696e 206f 6e6c 793a  song_id in only:
+00014280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014290: 2020 2020 2070 6c61 796c 6973 742e 6170       playlist.ap
+000142a0: 7065 6e64 2864 6574 6169 6c73 290a 0a20  pend(details).. 
+000142b0: 2020 2020 2020 2069 6620 6e6f 7420 706c         if not pl
+000142c0: 6179 6c69 7374 3a0a 2020 2020 2020 2020  aylist:.        
+000142d0: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
+000142e0: 224e 6f20 736f 6e67 7320 666f 756e 6420  "No songs found 
+000142f0: 7769 7468 2074 6865 2067 6976 656e 2049  with the given I
+00014300: 4473 2e22 2c20 6667 3d22 7265 6422 290a  Ds.", fg="red").
+00014310: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014320: 726e 0a20 2020 2065 6c73 653a 0a20 2020  rn.    else:.   
+00014330: 2020 2020 2069 6620 6e6f 7420 7461 6773       if not tags
+00014340: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00014350: 7468 206f 7065 6e28 534f 4e47 535f 494e  th open(SONGS_IN
+00014360: 464f 5f50 4154 482c 2022 7222 2c20 656e  FO_PATH, "r", en
+00014370: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
+00014380: 6173 2073 6f6e 6773 5f66 696c 653a 0a20  as songs_file:. 
+00014390: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000143a0: 6f72 206c 696e 6520 696e 2073 6f6e 6773  or line in songs
+000143b0: 5f66 696c 653a 0a20 2020 2020 2020 2020  _file:.         
+000143c0: 2020 2020 2020 2020 2020 2064 6574 6169             detai
+000143d0: 6c73 203d 206c 696e 652e 7374 7269 7028  ls = line.strip(
+000143e0: 292e 7370 6c69 7428 227c 2229 0a20 2020  ).split("|").   
+000143f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014400: 2070 6c61 796c 6973 742e 6170 7065 6e64   playlist.append
+00014410: 2864 6574 6169 6c73 290a 2020 2020 2020  (details).      
+00014420: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00014430: 2020 2020 7461 6773 203d 2073 6574 2874      tags = set(t
+00014440: 6167 7329 0a20 2020 2020 2020 2020 2020  ags).           
+00014450: 2077 6974 6820 6f70 656e 2853 4f4e 4753   with open(SONGS
+00014460: 5f49 4e46 4f5f 5041 5448 2c20 2272 222c  _INFO_PATH, "r",
+00014470: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+00014480: 2229 2061 7320 736f 6e67 735f 6669 6c65  ") as songs_file
+00014490: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000144a0: 2020 666f 7220 6c69 6e65 2069 6e20 736f    for line in so
+000144b0: 6e67 735f 6669 6c65 3a0a 2020 2020 2020  ngs_file:.      
+000144c0: 2020 2020 2020 2020 2020 2020 2020 6465                de
+000144d0: 7461 696c 7320 3d20 6c69 6e65 2e73 7472  tails = line.str
+000144e0: 6970 2829 2e73 706c 6974 2822 7c22 290a  ip().split("|").
+000144f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014500: 2020 2020 736f 6e67 5f74 6167 7320 3d20      song_tags = 
+00014510: 7365 7428 6465 7461 696c 735b 325d 2e73  set(details[2].s
+00014520: 706c 6974 2822 2c22 2929 0a20 2020 2020  plit(",")).     
+00014530: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00014540: 6620 6e6f 7420 6d61 7463 685f 616c 6c3a  f not match_all:
+00014550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014560: 2020 2020 2020 2020 2069 6620 7461 6773           if tags
+00014570: 2026 2073 6f6e 675f 7461 6773 3a20 2023   & song_tags:  #
+00014580: 2069 6e74 6572 7365 6374 696f 6e0a 2020   intersection.  
+00014590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145a0: 2020 2020 2020 2020 2020 706c 6179 6c69            playli
+000145b0: 7374 2e61 7070 656e 6428 6465 7461 696c  st.append(detail
+000145c0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+000145d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000145e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000145f0: 2020 2020 2069 6620 7461 6773 203c 3d20       if tags <= 
+00014600: 736f 6e67 5f74 6167 733a 2020 2320 7375  song_tags:  # su
+00014610: 6273 6574 0a20 2020 2020 2020 2020 2020  bset.           
+00014620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014630: 2070 6c61 796c 6973 742e 6170 7065 6e64   playlist.append
+00014640: 2864 6574 6169 6c73 290a 0a20 2020 2066  (details)..    f
+00014650: 6f72 2064 6574 6169 6c73 2069 6e20 706c  or details in pl
+00014660: 6179 6c69 7374 3a0a 2020 2020 2020 2020  aylist:.        
+00014670: 736f 6e67 5f64 6174 6120 3d20 6d75 7369  song_data = musi
+00014680: 635f 7461 672e 6c6f 6164 5f66 696c 6528  c_tag.load_file(
+00014690: 6f73 2e70 6174 682e 6a6f 696e 2853 4f4e  os.path.join(SON
+000146a0: 4753 5f44 4952 2c20 6465 7461 696c 735b  GS_DIR, details[
+000146b0: 315d 2929 0a20 2020 2020 2020 2064 6574  1])).        det
+000146c0: 6169 6c73 202b 3d20 5b0a 2020 2020 2020  ails += [.      
+000146d0: 2020 2020 2020 2873 6f6e 675f 6461 7461        (song_data
+000146e0: 5b22 6172 7469 7374 225d 2e76 616c 7565  ["artist"].value
+000146f0: 206f 7220 2255 6e6b 6e6f 776e 2041 7274   or "Unknown Art
+00014700: 6973 7422 292c 0a20 2020 2020 2020 2020  ist"),.         
+00014710: 2020 2028 736f 6e67 5f64 6174 615b 2261     (song_data["a
+00014720: 6c62 756d 225d 2e76 616c 7565 206f 7220  lbum"].value or 
+00014730: 2255 6e6b 6e6f 776e 2041 6c62 756d 2229  "Unknown Album")
+00014740: 2c0a 2020 2020 2020 2020 2020 2020 2873  ,.            (s
+00014750: 6f6e 675f 6461 7461 5b22 616c 6275 6d61  ong_data["albuma
+00014760: 7274 6973 7422 5d2e 7661 6c75 6520 6f72  rtist"].value or
+00014770: 2022 556e 6b6e 6f77 6e20 416c 6275 6d20   "Unknown Album 
+00014780: 4172 7469 7374 2229 2c0a 2020 2020 2020  Artist"),.      
+00014790: 2020 5d0a 0a20 2020 2069 6620 7368 7566    ]..    if shuf
+000147a0: 666c 655f 203d 3d20 303a 0a20 2020 2020  fle_ == 0:.     
+000147b0: 2020 2073 6875 6666 6c65 5f20 3d20 5472     shuffle_ = Tr
+000147c0: 7565 0a20 2020 2020 2020 2072 6573 6875  ue.        reshu
+000147d0: 6666 6c65 203d 2046 616c 7365 0a20 2020  ffle = False.   
+000147e0: 2065 6c69 6620 7368 7566 666c 655f 203d   elif shuffle_ =
+000147f0: 3d20 313a 0a20 2020 2020 2020 2073 6875  = 1:.        shu
+00014800: 6666 6c65 5f20 3d20 5472 7565 0a20 2020  ffle_ = True.   
+00014810: 2020 2020 2072 6573 6875 6666 6c65 203d       reshuffle =
+00014820: 2054 7275 650a 2020 2020 656c 6966 2073   True.    elif s
+00014830: 6875 6666 6c65 5f20 3d3d 2032 3a0a 2020  huffle_ == 2:.  
+00014840: 2020 2020 2020 7368 7566 666c 655f 203d        shuffle_ =
+00014850: 2046 616c 7365 0a20 2020 2020 2020 2072   False.        r
+00014860: 6573 6875 6666 6c65 203d 2054 7275 650a  eshuffle = True.
+00014870: 2020 2020 656c 7365 3a20 2023 2073 6875      else:  # shu
+00014880: 6666 6c65 5f20 3d20 4e6f 6e65 0a20 2020  ffle_ = None.   
+00014890: 2020 2020 2073 6875 6666 6c65 5f20 3d20       shuffle_ = 
+000148a0: 4661 6c73 650a 2020 2020 2020 2020 7265  False.        re
+000148b0: 7368 7566 666c 6520 3d20 4661 6c73 650a  shuffle = False.
+000148c0: 0a20 2020 2069 6620 7368 7566 666c 655f  .    if shuffle_
+000148d0: 3a0a 2020 2020 2020 2020 7368 7566 666c  :.        shuffl
+000148e0: 6528 706c 6179 6c69 7374 290a 2020 2020  e(playlist).    
+000148f0: 656c 6966 2072 6576 6572 7365 3a0a 2020  elif reverse:.  
+00014900: 2020 2020 2020 706c 6179 6c69 7374 2e72        playlist.r
+00014910: 6576 6572 7365 2829 0a0a 2020 2020 6966  everse()..    if
+00014920: 206e 6f74 2070 6c61 796c 6973 743a 0a20   not playlist:. 
+00014930: 2020 2020 2020 2063 6c69 636b 2e73 6563         click.sec
+00014940: 686f 2822 4e6f 2073 6f6e 6773 2066 6f75  ho("No songs fou
+00014950: 6e64 206d 6174 6368 696e 6720 7461 6720  nd matching tag 
+00014960: 6372 6974 6572 6961 2e22 2c20 6667 3d22  criteria.", fg="
+00014970: 7265 6422 290a 2020 2020 656c 7365 3a0a  red").    else:.
+00014980: 2020 2020 2020 2020 766f 6c75 6d65 202f          volume /
+00014990: 3d20 3130 300a 2020 2020 2020 2020 6375  = 100.        cu
+000149a0: 7273 6573 2e77 7261 7070 6572 280a 2020  rses.wrapper(.  
+000149b0: 2020 2020 2020 2020 2020 5f70 6c61 792c            _play,
+000149c0: 0a20 2020 2020 2020 2020 2020 2070 6c61  .            pla
+000149d0: 796c 6973 742c 0a20 2020 2020 2020 2020  ylist,.         
+000149e0: 2020 2076 6f6c 756d 652c 0a20 2020 2020     volume,.     
+000149f0: 2020 2020 2020 206c 6f6f 702c 0a20 2020         loop,.   
+00014a00: 2020 2020 2020 2020 2063 6c69 7073 2c0a           clips,.
+00014a10: 2020 2020 2020 2020 2020 2020 7265 7368              resh
+00014a20: 7566 666c 652c 0a20 2020 2020 2020 2020  uffle,.         
+00014a30: 2020 2064 6973 636f 7264 2061 6e64 2063     discord and c
+00014a40: 616e 5f75 7064 6174 655f 6469 7363 6f72  an_update_discor
+00014a50: 642c 0a20 2020 2020 2020 2020 2020 2076  d,.            v
+00014a60: 6973 7561 6c69 7a65 2c0a 2020 2020 2020  isualize,.      
+00014a70: 2020 290a 0a0a 4063 6c69 2e63 6f6d 6d61    )...@cli.comma
+00014a80: 6e64 2829 0a40 636c 6963 6b2e 6f70 7469  nd().@click.opti
+00014a90: 6f6e 280a 2020 2020 222d 542f 2d6e 5422  on(.    "-T/-nT"
+00014aa0: 2c0a 2020 2020 222d 2d74 6167 2f2d 2d6e  ,.    "--tag/--n
+00014ab0: 6f2d 7461 6722 2c0a 2020 2020 2272 656e  o-tag",.    "ren
+00014ac0: 616d 696e 675f 7461 6722 2c0a 2020 2020  aming_tag",.    
+00014ad0: 6465 6661 756c 743d 4661 6c73 652c 0a20  default=False,. 
+00014ae0: 2020 2068 656c 703d 2249 6620 7061 7373     help="If pass
+00014af0: 6564 2c20 7265 6e61 6d65 2074 6167 2069  ed, rename tag i
+00014b00: 6e73 7465 6164 206f 6620 736f 6e67 2028  nstead of song (
+00014b10: 7472 6561 7420 7468 6520 6172 6775 6d65  treat the argume
+00014b20: 6e74 7320 6173 2074 6167 7329 2e22 2c0a  nts as tags).",.
+00014b30: 290a 4063 6c69 636b 2e61 7267 756d 656e  ).@click.argumen
+00014b40: 7428 226f 7269 6769 6e61 6c22 290a 4063  t("original").@c
+00014b50: 6c69 636b 2e61 7267 756d 656e 7428 226e  lick.argument("n
+00014b60: 6577 5f6e 616d 6522 290a 6465 6620 7265  ew_name").def re
+00014b70: 6e61 6d65 286f 7269 6769 6e61 6c2c 206e  name(original, n
+00014b80: 6577 5f6e 616d 652c 2072 656e 616d 696e  ew_name, renamin
+00014b90: 675f 7461 6729 3a0a 2020 2020 2222 220a  g_tag):.    """.
+00014ba0: 2020 2020 5265 6e61 6d65 2061 2073 6f6e      Rename a son
+00014bb0: 672e 0a0a 2020 2020 5265 6e61 6d65 7320  g...    Renames 
+00014bc0: 7468 6520 736f 6e67 2077 6974 6820 7468  the song with th
+00014bd0: 6520 4944 204f 5249 4749 4e41 4c20 746f  e ID ORIGINAL to
+00014be0: 204e 4557 5f4e 414d 452e 2054 6865 2065   NEW_NAME. The e
+00014bf0: 7874 656e 7369 6f6e 206f 6620 7468 650a  xtension of the.
+00014c00: 2020 2020 736f 6e67 2028 652e 672e 2027      song (e.g. '
+00014c10: 2e77 6176 272c 2027 2e6d 7033 2729 2069  .wav', '.mp3') i
+00014c20: 7320 7072 6573 6572 7665 64e2 8094 646f  s preserved...do
+00014c30: 206e 6f74 2069 6e63 6c75 6465 2069 7420   not include it 
+00014c40: 696e 2074 6865 206e 616d 652e 0a0a 2020  in the name...  
+00014c50: 2020 4966 2074 6865 2027 2d54 2f2d 2d74    If the '-T/--t
+00014c60: 6167 2720 666c 6167 2069 7320 7061 7373  ag' flag is pass
+00014c70: 6564 2c20 7472 6561 7473 204f 5249 4749  ed, treats ORIGI
+00014c80: 4e41 4c20 6173 2061 2074 6167 2c20 7265  NAL as a tag, re
+00014c90: 6e61 6d69 6e67 2061 6c6c 0a20 2020 206f  naming all.    o
+00014ca0: 6375 7272 656e 6365 7320 6f66 2069 7420  currences of it 
+00014cb0: 746f 204e 4557 5f4e 414d 45e2 8094 646f  to NEW_NAME...do
+00014cc0: 6573 6e27 7420 6368 6563 6b20 6966 2074  esn't check if t
+00014cd0: 6865 2074 6167 204e 4557 5f4e 414d 4520  he tag NEW_NAME 
+00014ce0: 616c 7265 6164 792c 0a20 2020 2065 7869  already,.    exi
+00014cf0: 7374 732c 2073 6f20 6265 2063 6172 6566  sts, so be caref
+00014d00: 756c 210a 2020 2020 2222 220a 2020 2020  ul!.    """.    
+00014d10: 736f 6e67 735f 6669 6c65 203d 206f 7065  songs_file = ope
+00014d20: 6e28 534f 4e47 535f 494e 464f 5f50 4154  n(SONGS_INFO_PAT
+00014d30: 482c 2022 7222 2c20 656e 636f 6469 6e67  H, "r", encoding
+00014d40: 3d22 7574 662d 3822 290a 2020 2020 6c69  ="utf-8").    li
+00014d50: 6e65 7320 3d20 736f 6e67 735f 6669 6c65  nes = songs_file
+00014d60: 2e72 6561 6428 292e 7370 6c69 746c 696e  .read().splitlin
+00014d70: 6573 2829 0a20 2020 2069 6620 6e6f 7420  es().    if not 
+00014d80: 7265 6e61 6d69 6e67 5f74 6167 3a0a 2020  renaming_tag:.  
+00014d90: 2020 2020 2020 6966 206e 6f74 206f 7269        if not ori
+00014da0: 6769 6e61 6c2e 6973 6e75 6d65 7269 6328  ginal.isnumeric(
+00014db0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00014dc0: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
+00014dd0: 2020 2020 2020 2020 2020 2020 2253 6f6e              "Son
+00014de0: 6720 4944 206d 7573 7420 6265 2061 6e20  g ID must be an 
+00014df0: 696e 7465 6765 722e 2054 6f20 7265 6e61  integer. To rena
+00014e00: 6d65 2061 2074 6167 2c20 7061 7373 2074  me a tag, pass t
+00014e10: 6865 2027 2d54 2f2d 2d74 6167 2720 666c  he '-T/--tag' fl
+00014e20: 6167 2e22 2c0a 2020 2020 2020 2020 2020  ag.",.          
+00014e30: 2020 2020 2020 6667 3d22 7265 6422 2c0a        fg="red",.
+00014e40: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00014e50: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014e60: 0a0a 2020 2020 2020 2020 666f 7220 6920  ..        for i 
+00014e70: 696e 2072 616e 6765 286c 656e 286c 696e  in range(len(lin
+00014e80: 6573 2929 3a0a 2020 2020 2020 2020 2020  es)):.          
+00014e90: 2020 6465 7461 696c 7320 3d20 6c69 6e65    details = line
+00014ea0: 735b 695d 2e73 7472 6970 2829 2e73 706c  s[i].strip().spl
+00014eb0: 6974 2822 7c22 290a 2020 2020 2020 2020  it("|").        
+00014ec0: 2020 2020 6966 206f 732e 7061 7468 2e73      if os.path.s
+00014ed0: 706c 6974 6578 7428 6465 7461 696c 735b  plitext(details[
+00014ee0: 315d 295b 305d 203d 3d20 6e65 775f 6e61  1])[0] == new_na
+00014ef0: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+00014f00: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
+00014f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014f20: 2020 2020 2066 2241 2073 6f6e 6720 7769       f"A song wi
+00014f30: 7468 2074 6865 206e 616d 6520 277b 6e65  th the name '{ne
+00014f40: 775f 6e61 6d65 7d27 2061 6c72 6561 6479  w_name}' already
+00014f50: 2065 7869 7374 732e 2050 6c65 6173 6520   exists. Please 
+00014f60: 6368 6f6f 7365 2061 6e6f 7468 6572 206e  choose another n
+00014f70: 616d 652e 222c 0a20 2020 2020 2020 2020  ame.",.         
+00014f80: 2020 2020 2020 2020 2020 2066 673d 2272             fg="r
+00014f90: 6564 222c 0a20 2020 2020 2020 2020 2020  ed",.           
+00014fa0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00014fb0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+00014fc0: 2020 2020 2020 206f 7269 6769 6e61 6c20         original 
+00014fd0: 3d20 696e 7428 6f72 6967 696e 616c 290a  = int(original).
+00014fe0: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
+00014ff0: 2072 616e 6765 286c 656e 286c 696e 6573   range(len(lines
+00015000: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00015010: 6465 7461 696c 7320 3d20 6c69 6e65 735b  details = lines[
+00015020: 695d 2e73 7472 6970 2829 2e73 706c 6974  i].strip().split
+00015030: 2822 7c22 290a 2020 2020 2020 2020 2020  ("|").          
+00015040: 2020 6966 2069 6e74 2864 6574 6169 6c73    if int(details
+00015050: 5b30 5d29 203d 3d20 6f72 6967 696e 616c  [0]) == original
+00015060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015070: 2020 6f6c 645f 7061 7468 203d 2064 6574    old_path = det
+00015080: 6169 6c73 5b31 5d0a 2020 2020 2020 2020  ails[1].        
+00015090: 2020 2020 2020 2020 6465 7461 696c 735b          details[
+000150a0: 315d 203d 206e 6577 5f6e 616d 6520 2b20  1] = new_name + 
+000150b0: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
+000150c0: 286f 6c64 5f70 6174 6829 5b31 5d0a 0a20  (old_path)[1].. 
+000150d0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+000150e0: 696e 6573 5b69 5d20 3d20 227c 222e 6a6f  ines[i] = "|".jo
+000150f0: 696e 2864 6574 6169 6c73 290a 2020 2020  in(details).    
+00015100: 2020 2020 2020 2020 2020 2020 736f 6e67              song
+00015110: 735f 6669 6c65 2e63 6c6f 7365 2829 0a20  s_file.close(). 
+00015120: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015130: 6f6e 6773 5f66 696c 6520 3d20 6f70 656e  ongs_file = open
+00015140: 2853 4f4e 4753 5f49 4e46 4f5f 5041 5448  (SONGS_INFO_PATH
+00015150: 2c20 2277 222c 2065 6e63 6f64 696e 673d  , "w", encoding=
+00015160: 2275 7466 2d38 2229 0a20 2020 2020 2020  "utf-8").       
+00015170: 2020 2020 2020 2020 2073 6f6e 6773 5f66           songs_f
+00015180: 696c 652e 7772 6974 6528 225c 6e22 2e6a  ile.write("\n".j
+00015190: 6f69 6e28 6c69 6e65 7329 290a 0a20 2020  oin(lines))..   
+000151a0: 2020 2020 2020 2020 2020 2020 206f 732e               os.
+000151b0: 7265 6e61 6d65 280a 2020 2020 2020 2020  rename(.        
+000151c0: 2020 2020 2020 2020 2020 2020 6f73 2e70              os.p
+000151d0: 6174 682e 6a6f 696e 2853 4f4e 4753 5f44  ath.join(SONGS_D
+000151e0: 4952 2c20 6f6c 645f 7061 7468 292c 0a20  IR, old_path),. 
+000151f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015200: 2020 206f 732e 7061 7468 2e6a 6f69 6e28     os.path.join(
+00015210: 534f 4e47 535f 4449 522c 2064 6574 6169  SONGS_DIR, detai
+00015220: 6c73 5b31 5d29 2c0a 2020 2020 2020 2020  ls[1]),.        
+00015230: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00015240: 2020 2020 2020 2020 2020 2063 6c69 636b             click
+00015250: 2e73 6563 686f 280a 2020 2020 2020 2020  .secho(.        
+00015260: 2020 2020 2020 2020 2020 2020 6622 5265              f"Re
+00015270: 6e61 6d65 6420 736f 6e67 2027 7b6f 6c64  named song '{old
+00015280: 5f70 6174 687d 2720 7769 7468 2049 4420  _path}' with ID 
+00015290: 7b6f 7269 6769 6e61 6c7d 2074 6f20 277b  {original} to '{
+000152a0: 6465 7461 696c 735b 315d 7d27 2e22 2c0a  details[1]}'.",.
+000152b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152c0: 2020 2020 6667 3d22 6772 6565 6e22 2c0a      fg="green",.
+000152d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000152e0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+000152f0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+00015300: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00015310: 2020 2063 6c69 636b 2e73 6563 686f 2866     click.secho(f
+00015320: 2253 6f6e 6720 7769 7468 2049 4420 7b6f  "Song with ID {o
+00015330: 7269 6769 6e61 6c7d 206e 6f74 2066 6f75  riginal} not fou
+00015340: 6e64 2e22 2c20 6667 3d22 7265 6422 290a  nd.", fg="red").
+00015350: 2020 2020 2020 2020 2020 2020 736f 6e67              song
+00015360: 735f 6669 6c65 2e63 6c6f 7365 2829 0a20  s_file.close(). 
+00015370: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00015380: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00015390: 6c65 6e28 6c69 6e65 7329 293a 0a20 2020  len(lines)):.   
+000153a0: 2020 2020 2020 2020 2064 6574 6169 6c73           details
+000153b0: 203d 206c 696e 6573 5b69 5d2e 7374 7269   = lines[i].stri
+000153c0: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
+000153d0: 2020 2020 2020 2020 2020 2074 6167 7320             tags 
+000153e0: 3d20 6465 7461 696c 735b 325d 2e73 706c  = details[2].spl
+000153f0: 6974 2822 2c22 290a 2020 2020 2020 2020  it(",").        
+00015400: 2020 2020 666f 7220 7420 696e 2072 616e      for t in ran
+00015410: 6765 286c 656e 2874 6167 7329 293a 0a20  ge(len(tags)):. 
+00015420: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00015430: 6620 7461 6773 5b74 5d20 3d3d 206f 7269  f tags[t] == ori
+00015440: 6769 6e61 6c3a 0a20 2020 2020 2020 2020  ginal:.         
+00015450: 2020 2020 2020 2020 2020 2074 6167 735b             tags[
+00015460: 745d 203d 206e 6577 5f6e 616d 650a 2020  t] = new_name.  
+00015470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015480: 2020 6465 7461 696c 735b 325d 203d 2022    details[2] = "
+00015490: 2c22 2e6a 6f69 6e28 7461 6773 290a 0a20  ,".join(tags).. 
+000154a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154b0: 2020 206c 696e 6573 5b69 5d20 3d20 227c     lines[i] = "|
+000154c0: 222e 6a6f 696e 2864 6574 6169 6c73 290a  ".join(details).
+000154d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154e0: 2020 2020 6272 6561 6b0a 0a20 2020 2020      break..     
+000154f0: 2020 2073 6f6e 6773 5f66 696c 652e 636c     songs_file.cl
+00015500: 6f73 6528 290a 2020 2020 2020 2020 736f  ose().        so
+00015510: 6e67 735f 6669 6c65 203d 206f 7065 6e28  ngs_file = open(
+00015520: 534f 4e47 535f 494e 464f 5f50 4154 482c  SONGS_INFO_PATH,
+00015530: 2022 7722 2c20 656e 636f 6469 6e67 3d22   "w", encoding="
+00015540: 7574 662d 3822 290a 2020 2020 2020 2020  utf-8").        
+00015550: 736f 6e67 735f 6669 6c65 2e77 7269 7465  songs_file.write
+00015560: 2822 5c6e 222e 6a6f 696e 286c 696e 6573  ("\n".join(lines
+00015570: 2929 0a0a 2020 2020 2020 2020 636c 6963  ))..        clic
+00015580: 6b2e 7365 6368 6f28 0a20 2020 2020 2020  k.secho(.       
+00015590: 2020 2020 2066 2252 6570 6c61 6365 6420       f"Replaced 
+000155a0: 616c 6c20 6f63 7572 7265 6e63 6573 206f  all ocurrences o
+000155b0: 6620 7461 6720 277b 6f72 6967 696e 616c  f tag '{original
+000155c0: 7d27 2074 6f20 277b 6e65 775f 6e61 6d65  }' to '{new_name
+000155d0: 7d27 2e22 2c0a 2020 2020 2020 2020 2020  }'.",.          
+000155e0: 2020 6667 3d22 6772 6565 6e22 2c0a 2020    fg="green",.  
+000155f0: 2020 2020 2020 290a 0a0a 4063 6c69 2e63        )...@cli.c
+00015600: 6f6d 6d61 6e64 2829 0a40 636c 6963 6b2e  ommand().@click.
+00015610: 6172 6775 6d65 6e74 2822 7068 7261 7365  argument("phrase
+00015620: 2229 0a40 636c 6963 6b2e 6f70 7469 6f6e  ").@click.option
+00015630: 280a 2020 2020 222d 542f 2d6e 5422 2c0a  (.    "-T/-nT",.
+00015640: 2020 2020 222d 2d74 6167 2f2d 2d6e 6f2d      "--tag/--no-
+00015650: 7461 6722 2c0a 2020 2020 2273 6561 7263  tag",.    "searc
+00015660: 6869 6e67 5f66 6f72 5f74 6167 7322 2c0a  hing_for_tags",.
+00015670: 2020 2020 6465 6661 756c 743d 4661 6c73      default=Fals
+00015680: 652c 0a20 2020 2068 656c 703d 2253 6561  e,.    help="Sea
+00015690: 7263 6865 7320 666f 7220 6d61 7463 6869  rches for matchi
+000156a0: 6e67 2074 6167 7320 696e 7374 6561 6420  ng tags instead 
+000156b0: 6f66 2073 6f6e 6720 6e61 6d65 732e 222c  of song names.",
+000156c0: 0a29 0a64 6566 2073 6561 7263 6828 7068  .).def search(ph
+000156d0: 7261 7365 2c20 7365 6172 6368 696e 675f  rase, searching_
+000156e0: 666f 725f 7461 6773 293a 0a20 2020 2022  for_tags):.    "
+000156f0: 2222 5365 6172 6368 6573 2066 6f72 2073  ""Searches for s
+00015700: 6f6e 6773 2074 6861 7420 636f 6e74 6169  ongs that contai
+00015710: 6e20 5048 5241 5345 2e20 416c 6c20 736f  n PHRASE. All so
+00015720: 6e67 7320 7374 6172 7469 6e67 2077 6974  ngs starting wit
+00015730: 6820 5048 5241 5345 0a20 2020 2077 696c  h PHRASE.    wil
+00015740: 6c20 6170 7065 6172 2062 6566 6f72 6520  l appear before 
+00015750: 736f 6e67 7320 636f 6e74 6169 6e69 6e67  songs containing
+00015760: 2062 7574 206e 6f74 2073 7461 7274 696e   but not startin
+00015770: 6720 7769 7468 2050 4852 4153 452e 2054  g with PHRASE. T
+00015780: 6869 730a 2020 2020 7365 6172 6368 2069  his.    search i
+00015790: 7320 6361 7365 2d69 6e73 656e 7369 7469  s case-insensiti
+000157a0: 7665 2e0a 0a20 2020 2049 6620 7468 6520  ve...    If the 
+000157b0: 272d 5427 2066 6c61 6720 6973 2070 6173  '-T' flag is pas
+000157c0: 7365 642c 2073 6561 7263 6865 7320 666f  sed, searches fo
+000157d0: 7220 7461 6773 2069 6e73 7465 6164 206f  r tags instead o
+000157e0: 6620 736f 6e67 206e 616d 6573 2e22 2222  f song names."""
+000157f0: 0a20 2020 2070 6872 6173 6520 3d20 7068  .    phrase = ph
+00015800: 7261 7365 2e6c 6f77 6572 2829 0a20 2020  rase.lower().   
+00015810: 2077 6974 6820 6f70 656e 2853 4f4e 4753   with open(SONGS
+00015820: 5f49 4e46 4f5f 5041 5448 2c20 2272 222c  _INFO_PATH, "r",
+00015830: 2065 6e63 6f64 696e 673d 2275 7466 2d38   encoding="utf-8
+00015840: 2229 2061 7320 736f 6e67 735f 6669 6c65  ") as songs_file
+00015850: 3a0a 2020 2020 2020 2020 6966 206e 6f74  :.        if not
+00015860: 2073 6561 7263 6869 6e67 5f66 6f72 5f74   searching_for_t
+00015870: 6167 733a 0a20 2020 2020 2020 2020 2020  ags:.           
+00015880: 2072 6573 756c 7473 203d 205b 5d2c 205b   results = [], [
+00015890: 5d20 2023 2073 7461 7274 732c 2063 6f6e  ]  # starts, con
+000158a0: 7461 696e 7320 6275 7420 646f 6573 206e  tains but does n
+000158b0: 6f74 2073 7461 7274 0a20 2020 2020 2020  ot start.       
+000158c0: 2020 2020 2066 6f72 206c 696e 6520 696e       for line in
+000158d0: 2073 6f6e 6773 5f66 696c 653a 0a20 2020   songs_file:.   
+000158e0: 2020 2020 2020 2020 2020 2020 2073 6f6e               son
+000158f0: 675f 6964 2c20 736f 6e67 5f6e 616d 652c  g_id, song_name,
+00015900: 2074 6167 732c 202a 5f20 3d20 6c69 6e65   tags, *_ = line
+00015910: 2e73 7472 6970 2829 2e73 706c 6974 2822  .strip().split("
+00015920: 7c22 290a 2020 2020 2020 2020 2020 2020  |").            
+00015930: 2020 2020 736f 6e67 5f69 6420 3d20 696e      song_id = in
+00015940: 7428 736f 6e67 5f69 6429 0a20 2020 2020  t(song_id).     
+00015950: 2020 2020 2020 2020 2020 2073 6f6e 675f             song_
+00015960: 6e61 6d65 203d 2073 6f6e 675f 6e61 6d65  name = song_name
+00015970: 2e6c 6f77 6572 2829 0a0a 2020 2020 2020  .lower()..      
+00015980: 2020 2020 2020 2020 2020 6966 2073 6f6e            if son
+00015990: 675f 6e61 6d65 2e73 7461 7274 7377 6974  g_name.startswit
+000159a0: 6828 7068 7261 7365 293a 0a20 2020 2020  h(phrase):.     
+000159b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000159c0: 6573 756c 7473 5b30 5d2e 6170 7065 6e64  esults[0].append
+000159d0: 2873 6f6e 675f 6964 290a 2020 2020 2020  (song_id).      
+000159e0: 2020 2020 2020 2020 2020 656c 6966 2070            elif p
+000159f0: 6872 6173 6520 696e 2073 6f6e 675f 6e61  hrase in song_na
+00015a00: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
+00015a10: 2020 2020 2020 2020 7265 7375 6c74 735b          results[
+00015a20: 315d 2e61 7070 656e 6428 736f 6e67 5f69  1].append(song_i
+00015a30: 6429 0a0a 2020 2020 2020 2020 2020 2020  d)..            
+00015a40: 6966 206e 6f74 2061 6e79 2872 6573 756c  if not any(resul
+00015a50: 7473 293a 0a20 2020 2020 2020 2020 2020  ts):.           
+00015a60: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
+00015a70: 2822 4e6f 2072 6573 756c 7473 2066 6f75  ("No results fou
+00015a80: 6e64 2e22 2c20 6667 3d22 7265 6422 290a  nd.", fg="red").
+00015a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015aa0: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
+00015ab0: 2020 2020 736f 6e67 735f 6669 6c65 2e73      songs_file.s
+00015ac0: 6565 6b28 3029 0a20 2020 2020 2020 2020  eek(0).         
+00015ad0: 2020 2066 6f72 206c 696e 6520 696e 2073     for line in s
+00015ae0: 6f6e 6773 5f66 696c 653a 0a20 2020 2020  ongs_file:.     
+00015af0: 2020 2020 2020 2020 2020 2064 6574 6169             detai
+00015b00: 6c73 203d 206c 696e 652e 7374 7269 7028  ls = line.strip(
+00015b10: 292e 7370 6c69 7428 227c 2229 0a20 2020  ).split("|").   
+00015b20: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00015b30: 696e 7428 6465 7461 696c 735b 305d 2920  int(details[0]) 
+00015b40: 696e 2072 6573 756c 7473 5b30 5d3a 0a20  in results[0]:. 
+00015b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b60: 2020 2070 7269 6e74 5f65 6e74 7279 2864     print_entry(d
+00015b70: 6574 6169 6c73 2c20 7068 7261 7365 290a  etails, phrase).
+00015b80: 0a20 2020 2020 2020 2020 2020 2073 6f6e  .            son
+00015b90: 6773 5f66 696c 652e 7365 656b 2830 290a  gs_file.seek(0).
+00015ba0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00015bb0: 6c69 6e65 2069 6e20 736f 6e67 735f 6669  line in songs_fi
+00015bc0: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00015bd0: 2020 2020 6465 7461 696c 7320 3d20 6c69      details = li
+00015be0: 6e65 2e73 7472 6970 2829 2e73 706c 6974  ne.strip().split
+00015bf0: 2822 7c22 290a 2020 2020 2020 2020 2020  ("|").          
+00015c00: 2020 2020 2020 6966 2069 6e74 2864 6574        if int(det
+00015c10: 6169 6c73 5b30 5d29 2069 6e20 7265 7375  ails[0]) in resu
+00015c20: 6c74 735b 315d 3a0a 2020 2020 2020 2020  lts[1]:.        
+00015c30: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00015c40: 745f 656e 7472 7928 6465 7461 696c 732c  t_entry(details,
+00015c50: 2070 6872 6173 6529 0a0a 2020 2020 2020   phrase)..      
+00015c60: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
+00015c70: 6f28 0a20 2020 2020 2020 2020 2020 2020  o(.             
+00015c80: 2020 2066 2246 6f75 6e64 207b 6c65 6e28     f"Found {len(
+00015c90: 7265 7375 6c74 735b 305d 2920 2b20 6c65  results[0]) + le
+00015ca0: 6e28 7265 7375 6c74 735b 315d 297d 2073  n(results[1])} s
+00015cb0: 6f6e 6728 7329 2e22 2c0a 2020 2020 2020  ong(s).",.      
+00015cc0: 2020 2020 2020 2020 2020 6667 3d22 6772            fg="gr
+00015cd0: 6565 6e22 2c0a 2020 2020 2020 2020 2020  een",.          
+00015ce0: 2020 290a 2020 2020 2020 2020 656c 7365    ).        else
+00015cf0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00015d00: 7375 6c74 7320 3d20 7365 7428 292c 2073  sults = set(), s
+00015d10: 6574 2829 2020 2320 7374 6172 7473 2c20  et()  # starts, 
+00015d20: 636f 6e74 6169 6e73 2062 7574 2064 6f65  contains but doe
+00015d30: 7320 6e6f 7420 7374 6172 740a 2020 2020  s not start.    
+00015d40: 2020 2020 2020 2020 666f 7220 6c69 6e65          for line
+00015d50: 2069 6e20 736f 6e67 735f 6669 6c65 3a0a   in songs_file:.
+00015d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d70: 736f 6e67 5f69 642c 2073 6f6e 675f 6e61  song_id, song_na
+00015d80: 6d65 2c20 7461 6773 2c20 2a5f 203d 206c  me, tags, *_ = l
+00015d90: 696e 652e 7374 7269 7028 292e 7370 6c69  ine.strip().spli
+00015da0: 7428 227c 2229 0a20 2020 2020 2020 2020  t("|").         
+00015db0: 2020 2020 2020 2069 6620 7461 6773 3a0a         if tags:.
+00015dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015dd0: 2020 2020 7461 6773 203d 2074 6167 732e      tags = tags.
+00015de0: 7370 6c69 7428 222c 2229 0a0a 2020 2020  split(",")..    
+00015df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e00: 666f 7220 7461 6720 696e 2074 6167 733a  for tag in tags:
+00015e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015e20: 2020 2020 2020 2020 2074 6167 5f6c 6f77           tag_low
+00015e30: 6572 203d 2074 6167 2e6c 6f77 6572 2829  er = tag.lower()
+00015e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015e50: 2020 2020 2020 2020 2069 6620 7461 675f           if tag_
+00015e60: 6c6f 7765 722e 7374 6172 7473 7769 7468  lower.startswith
+00015e70: 2870 6872 6173 6529 3a0a 2020 2020 2020  (phrase):.      
+00015e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015e90: 2020 2020 2020 7265 7375 6c74 735b 305d        results[0]
+00015ea0: 2e61 6464 2874 6167 290a 2020 2020 2020  .add(tag).      
+00015eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ec0: 2020 656c 6966 2070 6872 6173 6520 696e    elif phrase in
+00015ed0: 2074 6167 5f6c 6f77 6572 3a0a 2020 2020   tag_lower:.    
+00015ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ef0: 2020 2020 2020 2020 7265 7375 6c74 735b          results[
+00015f00: 315d 2e61 6464 2874 6167 290a 0a20 2020  1].add(tag)..   
+00015f10: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00015f20: 616e 7928 7265 7375 6c74 7329 3a0a 2020  any(results):.  
+00015f30: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00015f40: 6963 6b2e 7365 6368 6f28 224e 6f20 7265  ick.secho("No re
+00015f50: 7375 6c74 7320 666f 756e 642e 222c 2066  sults found.", f
+00015f60: 673d 2272 6564 2229 0a20 2020 2020 2020  g="red").       
+00015f70: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00015f80: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00015f90: 2074 6167 2069 6e20 7265 7375 6c74 735b   tag in results[
+00015fa0: 305d 3a0a 2020 2020 2020 2020 2020 2020  0]:.            
+00015fb0: 2020 2020 7072 696e 7428 7461 6729 0a0a      print(tag)..
+00015fc0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00015fd0: 7461 6720 696e 2072 6573 756c 7473 5b31  tag in results[1
+00015fe0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+00015ff0: 2020 2070 7269 6e74 2874 6167 290a 0a20     print(tag).. 
+00016000: 2020 2020 2020 2020 2020 2063 6c69 636b             click
+00016010: 2e73 6563 686f 280a 2020 2020 2020 2020  .secho(.        
+00016020: 2020 2020 2020 2020 6622 466f 756e 6420          f"Found 
+00016030: 7b6c 656e 2872 6573 756c 7473 5b30 5d29  {len(results[0])
+00016040: 202b 206c 656e 2872 6573 756c 7473 5b31   + len(results[1
+00016050: 5d29 7d20 7461 6728 7329 2e22 2c20 6667  ])} tag(s).", fg
+00016060: 3d22 6772 6565 6e22 0a20 2020 2020 2020  ="green".       
+00016070: 2020 2020 2029 0a0a 0a40 636c 692e 636f       )...@cli.co
+00016080: 6d6d 616e 6428 6e61 6d65 3d22 6c69 7374  mmand(name="list
+00016090: 2229 0a40 636c 6963 6b2e 6172 6775 6d65  ").@click.argume
+000160a0: 6e74 2822 7365 6172 6368 5f74 6167 7322  nt("search_tags"
+000160b0: 2c20 6d65 7461 7661 723d 2254 4147 5322  , metavar="TAGS"
+000160c0: 2c20 6e61 7267 733d 2d31 290a 4063 6c69  , nargs=-1).@cli
+000160d0: 636b 2e6f 7074 696f 6e28 0a20 2020 2022  ck.option(.    "
+000160e0: 2d73 222c 0a20 2020 2022 2d2d 736f 7274  -s",.    "--sort
+000160f0: 222c 0a20 2020 2022 736f 7274 5f22 2c0a  ",.    "sort_",.
+00016100: 2020 2020 7479 7065 3d63 6c69 636b 2e43      type=click.C
+00016110: 686f 6963 6528 0a20 2020 2020 2020 2028  hoice(.        (
+00016120: 0a20 2020 2020 2020 2020 2020 2022 6e6f  .            "no
+00016130: 6e65 222c 0a20 2020 2020 2020 2020 2020  ne",.           
+00016140: 2022 6e61 6d65 222c 0a20 2020 2020 2020   "name",.       
+00016150: 2020 2020 2022 6e22 2c0a 2020 2020 2020       "n",.      
+00016160: 2020 2020 2020 2273 6563 732d 6c69 7374        "secs-list
+00016170: 656e 6564 222c 0a20 2020 2020 2020 2020  ened",.         
+00016180: 2020 2022 7322 2c0a 2020 2020 2020 2020     "s",.        
+00016190: 2020 2020 2264 7572 6174 696f 6e22 2c0a      "duration",.
+000161a0: 2020 2020 2020 2020 2020 2020 2264 222c              "d",
+000161b0: 0a20 2020 2020 2020 2020 2020 2022 7469  .            "ti
+000161c0: 6d65 732d 6c69 7374 656e 6564 222c 0a20  mes-listened",. 
+000161d0: 2020 2020 2020 2020 2020 2022 7422 2c0a             "t",.
+000161e0: 2020 2020 2020 2020 290a 2020 2020 292c          ).    ),
+000161f0: 0a20 2020 2068 656c 703d 2253 6f72 7420  .    help="Sort 
+00016200: 6279 206e 616d 652c 2073 6563 6f6e 6473  by name, seconds
+00016210: 206c 6973 7465 6e65 642c 206f 7220 7469   listened, or ti
+00016220: 6d65 7320 6c69 7374 656e 6564 2028 7365  mes listened (se
+00016230: 636f 6e64 732f 736f 6e67 2064 7572 6174  conds/song durat
+00016240: 696f 6e29 2e20 4772 6561 7465 7374 2066  ion). Greatest f
+00016250: 6972 7374 2e22 2c0a 2020 2020 6465 6661  irst.",.    defa
+00016260: 756c 743d 226e 6f6e 6522 2c0a 2020 2020  ult="none",.    
+00016270: 7368 6f77 5f64 6566 6175 6c74 3d54 7275  show_default=Tru
+00016280: 652c 0a29 0a40 636c 6963 6b2e 6f70 7469  e,.).@click.opti
+00016290: 6f6e 280a 2020 2020 222d 522f 2d6e 5222  on(.    "-R/-nR"
+000162a0: 2c0a 2020 2020 222d 2d72 6576 6572 7365  ,.    "--reverse
+000162b0: 2f2d 2d6e 6f2d 7265 7665 7273 6522 2c0a  /--no-reverse",.
+000162c0: 2020 2020 2272 6576 6572 7365 5f22 2c0a      "reverse_",.
+000162d0: 2020 2020 6465 6661 756c 743d 4661 6c73      default=Fals
+000162e0: 652c 0a20 2020 2068 656c 703d 2252 6576  e,.    help="Rev
+000162f0: 6572 7365 2074 6865 2073 6f72 7469 6e67  erse the sorting
+00016300: 206f 7264 6572 2028 6772 6561 7465 7374   order (greatest
+00016310: 2066 6972 7374 292e 222c 0a29 0a40 636c   first).",.).@cl
+00016320: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
+00016330: 222d 542f 2d6e 5422 2c0a 2020 2020 222d  "-T/-nT",.    "-
+00016340: 2d74 6167 2f2d 2d6e 6f2d 7461 6722 2c0a  -tag/--no-tag",.
+00016350: 2020 2020 226c 6973 7469 6e67 5f74 6167      "listing_tag
+00016360: 7322 2c0a 2020 2020 6465 6661 756c 743d  s",.    default=
+00016370: 4661 6c73 652c 0a20 2020 2068 656c 703d  False,.    help=
+00016380: 224c 6973 7420 7461 6773 206d 6174 6368  "List tags match
+00016390: 696e 6720 5441 4753 2069 6e73 7465 6164  ing TAGS instead
+000163a0: 206f 6620 736f 6e67 732e 222c 0a29 0a40   of songs.",.).@
+000163b0: 636c 6963 6b2e 6f70 7469 6f6e 280a 2020  click.option(.  
+000163c0: 2020 222d 7922 2c0a 2020 2020 222d 2d79    "-y",.    "--y
+000163d0: 6561 7222 2c0a 2020 2020 2279 6561 7222  ear",.    "year"
+000163e0: 2c0a 2020 2020 6865 6c70 3d22 5368 6f77  ,.    help="Show
+000163f0: 2074 696d 6520 6c69 7374 656e 6564 2066   time listened f
+00016400: 6f72 2061 2073 7065 6369 6669 6320 7965  or a specific ye
+00016410: 6172 2c20 696e 7374 6561 6420 6f66 2074  ar, instead of t
+00016420: 6865 2074 6f74 616c 2e20 5061 7373 696e  he total. Passin
+00016430: 6720 2763 7572 2720 7769 6c6c 2073 686f  g 'cur' will sho
+00016440: 7720 7468 6520 7469 6d65 206c 6973 7465  w the time liste
+00016450: 6e65 6420 666f 7220 7468 6520 6375 7272  ned for the curr
+00016460: 656e 7420 7965 6172 2e22 2c0a 290a 4063  ent year.",.).@c
+00016470: 6c69 636b 2e6f 7074 696f 6e28 222d 7422  lick.option("-t"
+00016480: 2c20 222d 2d74 6f70 222c 2022 746f 7022  , "--top", "top"
+00016490: 2c20 7479 7065 3d69 6e74 2c20 6865 6c70  , type=int, help
+000164a0: 3d22 5368 6f77 2074 6865 2074 6f70 206e  ="Show the top n
+000164b0: 2073 6f6e 6773 2f74 6167 732e 2229 0a40   songs/tags.").@
+000164c0: 636c 6963 6b2e 6f70 7469 6f6e 280a 2020  click.option(.  
+000164d0: 2020 222d 4d2f 2d6e 4d22 2c0a 2020 2020    "-M/-nM",.    
+000164e0: 222d 2d6d 6174 6368 2d61 6c6c 2f2d 2d6e  "--match-all/--n
+000164f0: 6f2d 6d61 7463 682d 616c 6c22 2c0a 2020  o-match-all",.  
+00016500: 2020 226d 6174 6368 5f61 6c6c 222c 0a20    "match_all",. 
+00016510: 2020 2064 6566 6175 6c74 3d46 616c 7365     default=False
+00016520: 2c0a 2020 2020 6865 6c70 3d22 5368 6f77  ,.    help="Show
+00016530: 7320 736f 6e67 7320 7468 6174 206d 6174  s songs that mat
+00016540: 6368 2061 6c6c 2074 6167 7320 696e 7374  ch all tags inst
+00016550: 6561 6420 6f66 2061 6e79 2074 6167 2e20  ead of any tag. 
+00016560: 4967 6e6f 7265 6420 6966 2027 2d74 2f2d  Ignored if '-t/-
+00016570: 2d74 6167 2720 6973 2070 6173 7365 642e  -tag' is passed.
+00016580: 222c 0a29 0a64 6566 206c 6973 745f 2873  ",.).def list_(s
+00016590: 6561 7263 685f 7461 6773 2c20 6c69 7374  earch_tags, list
+000165a0: 696e 675f 7461 6773 2c20 7965 6172 2c20  ing_tags, year, 
+000165b0: 736f 7274 5f2c 2074 6f70 2c20 7265 7665  sort_, top, reve
+000165c0: 7273 655f 2c20 6d61 7463 685f 616c 6c29  rse_, match_all)
+000165d0: 3a0a 2020 2020 2222 224c 6973 7420 7468  :.    """List th
+000165e0: 6520 656e 7472 6965 7320 666f 7220 616c  e entries for al
+000165f0: 6c20 736f 6e67 732e 0a0a 2020 2020 4f75  l songs...    Ou
+00016600: 7470 7574 2066 6f72 6d61 743a 2049 442c  tput format: ID,
+00016610: 206e 616d 652c 2064 7572 6174 696f 6e2c   name, duration,
+00016620: 206c 6973 7465 6e20 7469 6d65 2c20 7469   listen time, ti
+00016630: 6d65 7320 6c69 7374 656e 6564 2c20 5b63  mes listened, [c
+00016640: 6c69 702d 7374 6172 742c 2063 6c69 702d  lip-start, clip-
+00016650: 656e 645d 2069 6620 636c 6970 2065 7869  end] if clip exi
+00016660: 7374 732c 2063 6f6d 6d61 2d73 6570 6172  sts, comma-separ
+00016670: 6174 6564 2074 6167 7320 6966 2061 6e79  ated tags if any
+00016680: 0a0a 2020 2020 4966 2074 6865 2027 2d54  ..    If the '-T
+00016690: 2720 666c 6167 2069 7320 7061 7373 6564  ' flag is passed
+000166a0: 2c20 7461 6773 2077 696c 6c20 6265 206c  , tags will be l
+000166b0: 6973 7465 6420 696e 7374 6561 6420 6f66  isted instead of
+000166c0: 2073 6f6e 6773 2e0a 0a20 2020 204f 7574   songs...    Out
+000166d0: 7075 7420 666f 726d 6174 3a20 7461 672c  put format: tag,
+000166e0: 2064 7572 6174 696f 6e2c 206c 6973 7465   duration, liste
+000166f0: 6e20 7469 6d65 2c20 7469 6d65 7320 6c69  n time, times li
+00016700: 7374 656e 6564 0a0a 2020 2020 4966 2054  stened..    If T
+00016710: 4147 5320 6172 6520 7061 7373 6564 2c20  AGS are passed, 
+00016720: 616e 7920 7461 672f 736f 6e67 206d 6174  any tag/song mat
+00016730: 6368 696e 6720 616e 7920 7461 6720 696e  ching any tag in
+00016740: 2054 4147 5320 7769 6c6c 2062 6520 6c69   TAGS will be li
+00016750: 7374 6564 2c0a 2020 2020 756e 6c65 7373  sted,.    unless
+00016760: 2074 6865 2027 2d4d 2f2d 2d6d 6174 6368   the '-M/--match
+00016770: 2d61 6c6c 2720 666c 6167 2069 7320 7061  -all' flag is pa
+00016780: 7373 6564 2c20 696e 2077 6869 6368 2063  ssed, in which c
+00016790: 6173 6520 6576 6572 7920 7461 6720 6d75  ase every tag mu
+000167a0: 7374 0a20 2020 2062 6520 6d61 7463 6865  st.    be matche
+000167b0: 6420 2869 676e 6f72 6564 2069 6620 6c69  d (ignored if li
+000167c0: 7374 696e 6720 7461 6773 292e 0a20 2020  sting tags)..   
+000167d0: 2022 2222 0a20 2020 2069 6620 746f 7020   """.    if top 
+000167e0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000167f0: 2020 2020 2069 6620 746f 7020 3c20 313a       if top < 1:
+00016800: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+00016810: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
+00016820: 2020 2020 2020 2020 2020 2254 6865 206f            "The o
+00016830: 7074 696f 6e20 272d 742f 2d2d 746f 7027  ption '-t/--top'
+00016840: 206d 7573 7420 6265 2061 2070 6f73 6974   must be a posit
+00016850: 6976 6520 6e75 6d62 6572 2e22 2c20 6667  ive number.", fg
+00016860: 3d22 7265 6422 0a20 2020 2020 2020 2020  ="red".         
+00016870: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+00016880: 2072 6574 7572 6e0a 0a20 2020 2069 6620   return..    if 
+00016890: 7965 6172 2069 7320 4e6f 6e65 3a0a 2020  year is None:.  
+000168a0: 2020 2020 2020 7374 6174 735f 7061 7468        stats_path
+000168b0: 203d 2054 4f54 414c 5f53 5441 5453 5f50   = TOTAL_STATS_P
+000168c0: 4154 480a 2020 2020 656c 7365 3a0a 2020  ATH.    else:.  
+000168d0: 2020 2020 2020 6966 2079 6561 7220 3d3d        if year ==
+000168e0: 2022 6375 7222 3a0a 2020 2020 2020 2020   "cur":.        
+000168f0: 2020 2020 7965 6172 203d 2043 5552 5f59      year = CUR_Y
+00016900: 4541 520a 2020 2020 2020 2020 2020 2020  EAR.            
+00016910: 7374 6174 735f 7061 7468 203d 2043 5552  stats_path = CUR
+00016920: 5f59 4541 525f 5354 4154 535f 5041 5448  _YEAR_STATS_PATH
+00016930: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00016940: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00016950: 7420 7965 6172 2e69 7364 6967 6974 2829  t year.isdigit()
+00016960: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016970: 2020 636c 6963 6b2e 7365 6368 6f28 2259    click.secho("Y
+00016980: 6561 7220 6d75 7374 2062 6520 6120 6e75  ear must be a nu
+00016990: 6d62 6572 206f 7220 2763 7572 272e 222c  mber or 'cur'.",
+000169a0: 2066 673d 2272 6564 2229 0a20 2020 2020   fg="red").     
+000169b0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000169c0: 6e0a 2020 2020 2020 2020 2020 2020 7374  n.            st
+000169d0: 6174 735f 7061 7468 203d 206f 732e 7061  ats_path = os.pa
+000169e0: 7468 2e6a 6f69 6e28 5354 4154 535f 4449  th.join(STATS_DI
+000169f0: 522c 2066 227b 7965 6172 7d2e 7478 7422  R, f"{year}.txt"
+00016a00: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+00016a10: 206e 6f74 206f 732e 7061 7468 2e65 7869   not os.path.exi
+00016a20: 7374 7328 7374 6174 735f 7061 7468 293a  sts(stats_path):
+00016a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016a40: 2063 6c69 636b 2e73 6563 686f 2866 224e   click.secho(f"N
+00016a50: 6f20 7374 6174 7320 666f 756e 6420 666f  o stats found fo
+00016a60: 7220 7965 6172 207b 7965 6172 7d2e 222c  r year {year}.",
+00016a70: 2066 673d 2272 6564 2229 0a20 2020 2020   fg="red").     
+00016a80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00016a90: 6e0a 0a20 2020 2069 6620 7365 6172 6368  n..    if search
+00016aa0: 5f74 6167 733a 0a20 2020 2020 2020 2073  _tags:.        s
+00016ab0: 6561 7263 685f 7461 6773 203d 2073 6574  earch_tags = set
+00016ac0: 2873 6561 7263 685f 7461 6773 290a 0a20  (search_tags).. 
+00016ad0: 2020 206e 756d 5f6c 696e 6573 203d 2030     num_lines = 0
+00016ae0: 0a0a 2020 2020 6966 206c 6973 7469 6e67  ..    if listing
+00016af0: 5f74 6167 733a 0a20 2020 2020 2020 2077  _tags:.        w
+00016b00: 6974 6820 280a 2020 2020 2020 2020 2020  ith (.          
+00016b10: 2020 6f70 656e 2853 4f4e 4753 5f49 4e46    open(SONGS_INF
+00016b20: 4f5f 5041 5448 2c20 2272 222c 2065 6e63  O_PATH, "r", enc
+00016b30: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
+00016b40: 7320 736f 6e67 735f 6669 6c65 2c0a 2020  s songs_file,.  
+00016b50: 2020 2020 2020 2020 2020 6f70 656e 2873            open(s
+00016b60: 7461 7473 5f70 6174 682c 2022 7222 2c20  tats_path, "r", 
+00016b70: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+00016b80: 2920 6173 2073 7461 7473 5f66 696c 652c  ) as stats_file,
+00016b90: 0a20 2020 2020 2020 2029 3a0a 2020 2020  .        ):.    
+00016ba0: 2020 2020 2020 2020 736f 6e67 735f 6c69          songs_li
+00016bb0: 6e65 7320 3d20 736f 6e67 735f 6669 6c65  nes = songs_file
+00016bc0: 2e72 6561 646c 696e 6573 2829 0a20 2020  .readlines().   
+00016bd0: 2020 2020 2020 2020 2073 7461 7473 203d           stats =
+00016be0: 2064 6963 7428 0a20 2020 2020 2020 2020   dict(.         
+00016bf0: 2020 2020 2020 206d 6170 280a 2020 2020         map(.    
+00016c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c10: 6c61 6d62 6461 2074 3a20 2869 6e74 2874  lambda t: (int(t
+00016c20: 5b30 5d29 2c29 202b 2074 5b31 3a5d 2c0a  [0]),) + t[1:],.
+00016c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c40: 2020 2020 6d61 7028 0a20 2020 2020 2020      map(.       
+00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c60: 206c 616d 6264 6120 783a 2074 7570 6c65   lambda x: tuple
+00016c70: 286d 6170 2866 6c6f 6174 2c20 782e 7374  (map(float, x.st
+00016c80: 7269 7028 292e 7370 6c69 7428 227c 2229  rip().split("|")
+00016c90: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00016ca0: 2020 2020 2020 2020 2020 2020 7374 6174              stat
+00016cb0: 735f 6669 6c65 2e72 6561 646c 696e 6573  s_file.readlines
+00016cc0: 2829 2c0a 2020 2020 2020 2020 2020 2020  (),.            
+00016cd0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
+00016ce0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00016cf0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+00016d00: 2020 2020 2020 2020 7461 6773 203d 2064          tags = d
+00016d10: 6566 6175 6c74 6469 6374 286c 616d 6264  efaultdict(lambd
+00016d20: 613a 2028 302e 302c 2030 2e30 2929 0a0a  a: (0.0, 0.0))..
+00016d30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00016d40: 6920 696e 2072 616e 6765 286c 656e 2873  i in range(len(s
+00016d50: 6f6e 6773 5f6c 696e 6573 2929 3a0a 2020  ongs_lines)):.  
+00016d60: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00016d70: 6e67 5f69 642c 2073 6f6e 675f 6e61 6d65  ng_id, song_name
+00016d80: 2c20 7461 675f 7374 7269 6e67 203d 2028  , tag_string = (
+00016d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016da0: 2020 2020 2073 6f6e 6773 5f6c 696e 6573       songs_lines
+00016db0: 5b69 5d2e 7374 7269 7028 292e 7370 6c69  [i].strip().spli
+00016dc0: 7428 227c 2229 5b30 3a33 5d0a 2020 2020  t("|")[0:3].    
+00016dd0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00016de0: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00016df0: 6e67 5f69 6420 3d20 696e 7428 736f 6e67  ng_id = int(song
+00016e00: 5f69 6429 0a20 2020 2020 2020 2020 2020  _id).           
+00016e10: 2020 2020 2069 6620 7461 675f 7374 7269       if tag_stri
+00016e20: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+00016e30: 2020 2020 2020 2020 666f 7220 7461 6720          for tag 
+00016e40: 696e 2074 6167 5f73 7472 696e 672e 7370  in tag_string.sp
+00016e50: 6c69 7428 222c 2229 3a0a 2020 2020 2020  lit(","):.      
+00016e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e70: 2020 6966 206e 6f74 2073 6561 7263 685f    if not search_
+00016e80: 7461 6773 206f 7220 7461 6720 696e 2073  tags or tag in s
+00016e90: 6561 7263 685f 7461 6773 3a0a 2020 2020  earch_tags:.    
+00016ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016eb0: 2020 2020 2020 2020 7461 6773 5b74 6167          tags[tag
+00016ec0: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+00016ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ee0: 2020 2020 2020 7461 6773 5b74 6167 5d5b        tags[tag][
+00016ef0: 305d 202b 2073 7461 7473 5b73 6f6e 675f  0] + stats[song_
+00016f00: 6964 5d2c 0a20 2020 2020 2020 2020 2020  id],.           
+00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f20: 2020 2020 2074 6167 735b 7461 675d 5b31       tags[tag][1
+00016f30: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00016f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f50: 2020 2b20 6d75 7369 635f 7461 672e 6c6f    + music_tag.lo
+00016f60: 6164 5f66 696c 6528 0a20 2020 2020 2020  ad_file(.       
+00016f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f80: 2020 2020 2020 2020 2020 2020 206f 732e               os.
+00016f90: 7061 7468 2e6a 6f69 6e28 534f 4e47 535f  path.join(SONGS_
+00016fa0: 4449 522c 2073 6f6e 675f 6e61 6d65 290a  DIR, song_name).
+00016fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fd0: 295b 2223 6c65 6e67 7468 225d 2e76 616c  )["#length"].val
+00016fe0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00016ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017000: 290a 0a20 2020 2020 2020 2020 2020 2074  )..            t
+00017010: 6167 5f69 7465 6d73 203d 206c 6973 7428  ag_items = list(
+00017020: 7461 6773 2e69 7465 6d73 2829 290a 0a20  tags.items()).. 
+00017030: 2020 2020 2020 2020 2020 2069 6620 736f             if so
+00017040: 7274 5f20 213d 2022 6e6f 6e65 223a 0a20  rt_ != "none":. 
+00017050: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00017060: 6620 736f 7274 5f20 696e 2028 226e 616d  f sort_ in ("nam
+00017070: 6522 2c20 226e 2229 3a0a 2020 2020 2020  e", "n"):.      
+00017080: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00017090: 7274 5f6b 6579 203d 206c 616d 6264 6120  rt_key = lambda 
+000170a0: 743a 2074 5b30 5d0a 2020 2020 2020 2020  t: t[0].        
+000170b0: 2020 2020 2020 2020 656c 6966 2073 6f72          elif sor
+000170c0: 745f 2069 6e20 2822 7365 6373 2d6c 6973  t_ in ("secs-lis
+000170d0: 7465 6e65 6422 2c20 2273 2229 3a0a 2020  tened", "s"):.  
+000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170f0: 2020 736f 7274 5f6b 6579 203d 206c 616d    sort_key = lam
+00017100: 6264 6120 743a 2074 5b31 5d5b 305d 0a20  bda t: t[1][0]. 
+00017110: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00017120: 6c69 6620 736f 7274 5f20 696e 2028 2264  lif sort_ in ("d
+00017130: 7572 6174 696f 6e22 2c20 2264 2229 3a0a  uration", "d"):.
+00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017150: 2020 2020 736f 7274 5f6b 6579 203d 206c      sort_key = l
+00017160: 616d 6264 6120 743a 2074 5b31 5d5b 315d  ambda t: t[1][1]
+00017170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017180: 2065 6c69 6620 736f 7274 5f20 696e 2028   elif sort_ in (
+00017190: 2274 696d 6573 2d6c 6973 7465 6e65 6422  "times-listened"
+000171a0: 2c20 2274 2229 3a0a 2020 2020 2020 2020  , "t"):.        
+000171b0: 2020 2020 2020 2020 2020 2020 736f 7274              sort
+000171c0: 5f6b 6579 203d 206c 616d 6264 6120 743a  _key = lambda t:
+000171d0: 2074 5b31 5d5b 305d 202f 2074 5b31 5d5b   t[1][0] / t[1][
+000171e0: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
+000171f0: 2020 2074 6167 5f69 7465 6d73 2e73 6f72     tag_items.sor
+00017200: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00017210: 2020 2020 2020 206b 6579 3d73 6f72 745f         key=sort_
+00017220: 6b65 792c 0a20 2020 2020 2020 2020 2020  key,.           
+00017230: 2020 2020 2020 2020 2072 6576 6572 7365           reverse
+00017240: 3d6e 6f74 2072 6576 6572 7365 5f2c 0a20  =not reverse_,. 
+00017250: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00017260: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00017270: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00017280: 2020 2069 6620 6e6f 7420 7265 7665 7273     if not revers
+00017290: 655f 3a0a 2020 2020 2020 2020 2020 2020  e_:.            
+000172a0: 2020 2020 2020 2020 7461 675f 6974 656d          tag_item
+000172b0: 732e 7265 7665 7273 6528 290a 0a20 2020  s.reverse()..   
+000172c0: 2020 2020 2020 2020 2066 6f72 2074 6167           for tag
+000172d0: 2c20 286c 6973 7465 6e5f 7469 6d65 2c20  , (listen_time, 
+000172e0: 746f 7461 6c5f 6475 7261 7469 6f6e 2920  total_duration) 
+000172f0: 696e 2074 6167 5f69 7465 6d73 3a0a 2020  in tag_items:.  
+00017300: 2020 2020 2020 2020 2020 2020 2020 636c                cl
+00017310: 6963 6b2e 6563 686f 280a 2020 2020 2020  ick.echo(.      
+00017320: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00017330: 7b74 6167 7d20 7b63 6c69 636b 2e73 7479  {tag} {click.sty
+00017340: 6c65 2866 6f72 6d61 745f 7365 636f 6e64  le(format_second
+00017350: 7328 746f 7461 6c5f 6475 7261 7469 6f6e  s(total_duration
+00017360: 2c20 7368 6f77 5f64 6563 696d 616c 3d54  , show_decimal=T
+00017370: 7275 6529 2c20 6667 3d27 6272 6967 6874  rue), fg='bright
+00017380: 5f62 6c61 636b 2729 7d20 7b63 6c69 636b  _black')} {click
+00017390: 2e73 7479 6c65 2866 6f72 6d61 745f 7365  .style(format_se
+000173a0: 636f 6e64 7328 6c69 7374 656e 5f74 696d  conds(listen_tim
+000173b0: 652c 2073 686f 775f 6465 6369 6d61 6c3d  e, show_decimal=
+000173c0: 5472 7565 292c 2066 673d 2779 656c 6c6f  True), fg='yello
+000173d0: 7727 297d 207b 636c 6963 6b2e 7374 796c  w')} {click.styl
+000173e0: 6528 2725 2e32 6627 2528 6c69 7374 656e  e('%.2f'%(listen
+000173f0: 5f74 696d 652f 746f 7461 6c5f 6475 7261  _time/total_dura
+00017400: 7469 6f6e 292c 2066 673d 2767 7265 656e  tion), fg='green
+00017410: 2729 7d22 0a20 2020 2020 2020 2020 2020  ')}".           
+00017420: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00017430: 2020 2020 2020 206e 756d 5f6c 696e 6573         num_lines
+00017440: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
+00017450: 2020 2020 2020 6966 2074 6f70 2069 7320        if top is 
+00017460: 6e6f 7420 4e6f 6e65 2061 6e64 206e 756d  not None and num
+00017470: 5f6c 696e 6573 203d 3d20 746f 703a 0a20  _lines == top:. 
+00017480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017490: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
+000174a0: 2072 6574 7572 6e0a 0a20 2020 206e 6f5f   return..    no_
+000174b0: 7265 7375 6c74 7320 3d20 5472 7565 0a20  results = True. 
+000174c0: 2020 2077 6974 6820 280a 2020 2020 2020     with (.      
+000174d0: 2020 6f70 656e 2853 4f4e 4753 5f49 4e46    open(SONGS_INF
+000174e0: 4f5f 5041 5448 2c20 2272 222c 2065 6e63  O_PATH, "r", enc
+000174f0: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
+00017500: 7320 736f 6e67 735f 6669 6c65 2c0a 2020  s songs_file,.  
+00017510: 2020 2020 2020 6f70 656e 2873 7461 7473        open(stats
+00017520: 5f70 6174 682c 2022 7222 2c20 656e 636f  _path, "r", enco
+00017530: 6469 6e67 3d22 7574 662d 3822 2920 6173  ding="utf-8") as
+00017540: 2073 7461 7473 5f66 696c 652c 0a20 2020   stats_file,.   
+00017550: 2029 3a0a 2020 2020 2020 2020 6c69 6e65   ):.        line
+00017560: 7320 3d20 736f 6e67 735f 6669 6c65 2e72  s = songs_file.r
+00017570: 6561 646c 696e 6573 2829 0a20 2020 2020  eadlines().     
+00017580: 2020 2073 7461 7473 203d 2064 6963 7428     stats = dict(
+00017590: 0a20 2020 2020 2020 2020 2020 206d 6170  .            map
+000175a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000175b0: 2020 6c61 6d62 6461 2074 3a20 2869 6e74    lambda t: (int
+000175c0: 2874 5b30 5d29 2c29 202b 2074 5b31 3a5d  (t[0]),) + t[1:]
+000175d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000175e0: 2020 6d61 7028 0a20 2020 2020 2020 2020    map(.         
+000175f0: 2020 2020 2020 2020 2020 206c 616d 6264             lambd
+00017600: 6120 783a 2074 7570 6c65 286d 6170 2866  a x: tuple(map(f
+00017610: 6c6f 6174 2c20 782e 7374 7269 7028 292e  loat, x.strip().
+00017620: 7370 6c69 7428 227c 2229 2929 2c0a 2020  split("|"))),.  
+00017630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017640: 2020 7374 6174 735f 6669 6c65 2e72 6561    stats_file.rea
+00017650: 646c 696e 6573 2829 2c0a 2020 2020 2020  dlines(),.      
+00017660: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00017670: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00017680: 2020 2029 0a0a 2020 2020 2020 2020 666f     )..        fo
+00017690: 7220 6920 696e 2072 616e 6765 286c 656e  r i in range(len
+000176a0: 286c 696e 6573 2929 3a0a 2020 2020 2020  (lines)):.      
+000176b0: 2020 2020 2020 6465 7461 696c 7320 3d20        details = 
+000176c0: 6c69 6e65 735b 695d 2e73 7472 6970 2829  lines[i].strip()
+000176d0: 2e73 706c 6974 2822 7c22 290a 2020 2020  .split("|").    
+000176e0: 2020 2020 2020 2020 736f 6e67 5f69 6420          song_id 
+000176f0: 3d20 696e 7428 6465 7461 696c 735b 305d  = int(details[0]
+00017700: 290a 0a20 2020 2020 2020 2020 2020 2074  )..            t
+00017710: 6167 7320 3d20 7365 7428 6465 7461 696c  ags = set(detail
+00017720: 735b 325d 2e73 706c 6974 2822 2c22 2929  s[2].split(","))
+00017730: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00017740: 7365 6172 6368 5f74 6167 733a 0a20 2020  search_tags:.   
+00017750: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00017760: 6d61 7463 685f 616c 6c3a 0a20 2020 2020  match_all:.     
+00017770: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00017780: 6620 6e6f 7420 7365 6172 6368 5f74 6167  f not search_tag
+00017790: 7320 3c3d 2074 6167 733a 2020 2320 7375  s <= tags:  # su
+000177a0: 6273 6574 0a20 2020 2020 2020 2020 2020  bset.           
+000177b0: 2020 2020 2020 2020 2020 2020 206c 696e               lin
+000177c0: 6573 5b69 5d20 3d20 2222 0a20 2020 2020  es[i] = "".     
+000177d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000177e0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+000177f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00017800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017810: 2020 2020 2020 6966 206e 6f74 2073 6561        if not sea
+00017820: 7263 685f 7461 6773 2026 2074 6167 733a  rch_tags & tags:
+00017830: 2020 2320 696e 7465 7273 6563 7469 6f6e    # intersection
+00017840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017850: 2020 2020 2020 2020 206c 696e 6573 5b69           lines[i
+00017860: 5d20 3d20 2222 0a20 2020 2020 2020 2020  ] = "".         
+00017870: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00017880: 6f6e 7469 6e75 650a 0a20 2020 2020 2020  ontinue..       
+00017890: 2020 2020 2074 696d 655f 6c69 7374 656e       time_listen
+000178a0: 6564 203d 2073 7461 7473 5b73 6f6e 675f  ed = stats[song_
+000178b0: 6964 5d0a 2020 2020 2020 2020 2020 2020  id].            
+000178c0: 6c69 6e65 735b 695d 203d 2074 7570 6c65  lines[i] = tuple
+000178d0: 2864 6574 6169 6c73 2920 2b20 280a 2020  (details) + (.  
+000178e0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+000178f0: 6d65 5f6c 6973 7465 6e65 642c 0a20 2020  me_listened,.   
+00017900: 2020 2020 2020 2020 2020 2020 206d 7573               mus
+00017910: 6963 5f74 6167 2e6c 6f61 645f 6669 6c65  ic_tag.load_file
+00017920: 286f 732e 7061 7468 2e6a 6f69 6e28 534f  (os.path.join(SO
+00017930: 4e47 535f 4449 522c 2064 6574 6169 6c73  NGS_DIR, details
+00017940: 5b31 5d29 295b 0a20 2020 2020 2020 2020  [1]))[.         
+00017950: 2020 2020 2020 2020 2020 2022 236c 656e             "#len
+00017960: 6774 6822 0a20 2020 2020 2020 2020 2020  gth".           
+00017970: 2020 2020 205d 2e76 616c 7565 2c0a 2020       ].value,.  
+00017980: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00017990: 2020 2020 206c 696e 6573 203d 205b 6c69       lines = [li
+000179a0: 6e65 2066 6f72 206c 696e 6520 696e 206c  ne for line in l
+000179b0: 696e 6573 2069 6620 6c69 6e65 5d0a 0a20  ines if line].. 
+000179c0: 2020 2020 2020 2069 6620 736f 7274 5f20         if sort_ 
+000179d0: 213d 2022 6e6f 6e65 223a 0a20 2020 2020  != "none":.     
+000179e0: 2020 2020 2020 2069 6620 736f 7274 5f20         if sort_ 
+000179f0: 696e 2028 226e 616d 6522 2c20 226e 2229  in ("name", "n")
+00017a00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017a10: 2020 736f 7274 5f6b 6579 203d 206c 616d    sort_key = lam
+00017a20: 6264 6120 743a 2074 5b31 5d0a 2020 2020  bda t: t[1].    
+00017a30: 2020 2020 2020 2020 656c 6966 2073 6f72          elif sor
+00017a40: 745f 2069 6e20 2822 7365 6373 2d6c 6973  t_ in ("secs-lis
+00017a50: 7465 6e65 6422 2c20 2273 2229 3a0a 2020  tened", "s"):.  
+00017a60: 2020 2020 2020 2020 2020 2020 2020 736f                so
+00017a70: 7274 5f6b 6579 203d 206c 616d 6264 6120  rt_key = lambda 
+00017a80: 743a 2066 6c6f 6174 2874 5b2d 325d 290a  t: float(t[-2]).
+00017a90: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00017aa0: 2073 6f72 745f 2069 6e20 2822 6475 7261   sort_ in ("dura
+00017ab0: 7469 6f6e 222c 2022 6422 293a 0a20 2020  tion", "d"):.   
+00017ac0: 2020 2020 2020 2020 2020 2020 2073 6f72               sor
+00017ad0: 745f 6b65 7920 3d20 6c61 6d62 6461 2074  t_key = lambda t
+00017ae0: 3a20 666c 6f61 7428 745b 2d31 5d29 0a20  : float(t[-1]). 
+00017af0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00017b00: 736f 7274 5f20 696e 2028 2274 696d 6573  sort_ in ("times
+00017b10: 2d6c 6973 7465 6e65 6422 2c20 2274 2229  -listened", "t")
+00017b20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017b30: 2020 736f 7274 5f6b 6579 203d 206c 616d    sort_key = lam
+00017b40: 6264 6120 743a 2066 6c6f 6174 2874 5b2d  bda t: float(t[-
+00017b50: 325d 2920 2f20 666c 6f61 7428 745b 2d31  2]) / float(t[-1
+00017b60: 5d29 0a20 2020 2020 2020 2020 2020 206c  ]).            l
+00017b70: 696e 6573 2e73 6f72 7428 0a20 2020 2020  ines.sort(.     
+00017b80: 2020 2020 2020 2020 2020 206b 6579 3d73             key=s
+00017b90: 6f72 745f 6b65 792c 0a20 2020 2020 2020  ort_key,.       
+00017ba0: 2020 2020 2020 2020 2072 6576 6572 7365           reverse
+00017bb0: 3d6e 6f74 2072 6576 6572 7365 5f2c 0a20  =not reverse_,. 
+00017bc0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00017bd0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00017be0: 2020 2020 2020 2069 6620 6e6f 7420 7265         if not re
+00017bf0: 7665 7273 655f 3a0a 2020 2020 2020 2020  verse_:.        
+00017c00: 2020 2020 2020 2020 6c69 6e65 732e 7265          lines.re
+00017c10: 7665 7273 6528 290a 0a20 2020 2020 2020  verse()..       
+00017c20: 2066 6f72 2064 6574 6169 6c73 2069 6e20   for details in 
+00017c30: 6c69 6e65 733a 0a20 2020 2020 2020 2020  lines:.         
+00017c40: 2020 2070 7269 6e74 5f65 6e74 7279 2864     print_entry(d
+00017c50: 6574 6169 6c73 290a 2020 2020 2020 2020  etails).        
+00017c60: 2020 2020 6e75 6d5f 6c69 6e65 7320 2b3d      num_lines +=
+00017c70: 2031 0a20 2020 2020 2020 2020 2020 206e   1.            n
+00017c80: 6f5f 7265 7375 6c74 7320 3d20 4661 6c73  o_results = Fals
+00017c90: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
+00017ca0: 2074 6f70 2069 7320 6e6f 7420 4e6f 6e65   top is not None
+00017cb0: 2061 6e64 206e 756d 5f6c 696e 6573 203d   and num_lines =
+00017cc0: 3d20 746f 703a 0a20 2020 2020 2020 2020  = top:.         
+00017cd0: 2020 2020 2020 2062 7265 616b 0a0a 2020         break..  
+00017ce0: 2020 6966 206e 6f5f 7265 7375 6c74 7320    if no_results 
+00017cf0: 616e 6420 7365 6172 6368 5f74 6167 733a  and search_tags:
+00017d00: 0a20 2020 2020 2020 2063 6c69 636b 2e73  .        click.s
+00017d10: 6563 686f 2822 4e6f 2073 6f6e 6773 2066  echo("No songs f
+00017d20: 6f75 6e64 206d 6174 6368 696e 6720 7461  ound matching ta
+00017d30: 6773 2e22 2c20 6667 3d22 7265 6422 290a  gs.", fg="red").
+00017d40: 2020 2020 656c 6966 206e 6f5f 7265 7375      elif no_resu
+00017d50: 6c74 733a 0a20 2020 2020 2020 2063 6c69  lts:.        cli
+00017d60: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
+00017d70: 2020 2020 2020 224e 6f20 736f 6e67 7320        "No songs 
+00017d80: 666f 756e 642e 2055 7365 2027 6d61 6573  found. Use 'maes
+00017d90: 7472 6f20 6164 6427 2074 6f20 6164 6420  tro add' to add 
+00017da0: 6120 736f 6e67 2e22 2c20 6667 3d22 7265  a song.", fg="re
+00017db0: 6422 0a20 2020 2020 2020 2029 0a0a 0a40  d".        )...@
+00017dc0: 636c 692e 636f 6d6d 616e 6428 290a 4063  cli.command().@c
+00017dd0: 6c69 636b 2e6f 7074 696f 6e28 0a20 2020  lick.option(.   
+00017de0: 2022 2d79 222c 0a20 2020 2022 2d2d 7965   "-y",.    "--ye
+00017df0: 6172 222c 0a20 2020 2022 7965 6172 222c  ar",.    "year",
+00017e00: 0a20 2020 2068 656c 703d 2253 686f 7720  .    help="Show 
+00017e10: 7469 6d65 206c 6973 7465 6e65 6420 666f  time listened fo
+00017e20: 7220 6120 7370 6563 6966 6963 2079 6561  r a specific yea
+00017e30: 722c 2069 6e73 7465 6164 206f 6620 7468  r, instead of th
+00017e40: 6520 746f 7461 6c2e 2050 6173 7369 6e67  e total. Passing
+00017e50: 2027 6375 7227 2077 696c 6c20 7368 6f77   'cur' will show
+00017e60: 2074 6865 2074 696d 6520 6c69 7374 656e   the time listen
+00017e70: 6564 2066 6f72 2074 6865 2063 7572 7265  ed for the curre
+00017e80: 6e74 2079 6561 722e 222c 0a29 0a40 636c  nt year.",.).@cl
+00017e90: 6963 6b2e 6f70 7469 6f6e 280a 2020 2020  ick.option(.    
+00017ea0: 222d 492f 2d6e 4922 2c0a 2020 2020 222d  "-I/-nI",.    "-
+00017eb0: 2d73 6f6e 672d 696e 666f 2f2d 2d6e 6f2d  -song-info/--no-
+00017ec0: 736f 6e67 2d69 6e66 6f22 2c0a 2020 2020  song-info",.    
+00017ed0: 2273 6f6e 675f 696e 666f 222c 0a20 2020  "song_info",.   
+00017ee0: 2064 6566 6175 6c74 3d46 616c 7365 2c0a   default=False,.
+00017ef0: 2020 2020 6865 6c70 3d22 5368 6f77 2074      help="Show t
+00017f00: 6865 2061 7274 6973 742c 2061 6c62 756d  he artist, album
+00017f10: 2c20 616e 6420 616c 6275 6d20 6172 7469  , and album arti
+00017f20: 7374 2066 6f72 2065 6163 6820 736f 6e67  st for each song
+00017f30: 2e22 2c0a 290a 4063 6c69 636b 2e61 7267  .",.).@click.arg
+00017f40: 756d 656e 7428 2273 6f6e 675f 6964 7322  ument("song_ids"
+00017f50: 2c20 7479 7065 3d63 6c69 636b 2e49 4e54  , type=click.INT
+00017f60: 2c20 6e61 7267 733d 2d31 2c20 7265 7175  , nargs=-1, requ
+00017f70: 6972 6564 3d54 7275 6529 0a64 6566 2065  ired=True).def e
+00017f80: 6e74 7279 2873 6f6e 675f 6964 732c 2079  ntry(song_ids, y
+00017f90: 6561 722c 2073 6f6e 675f 696e 666f 293a  ear, song_info):
+00017fa0: 0a20 2020 2022 2222 0a20 2020 2056 6965  .    """.    Vie
+00017fb0: 7720 7468 6520 6465 7461 696c 7320 666f  w the details fo
+00017fc0: 7220 7370 6563 6966 6963 2073 6f6e 6728  r specific song(
+00017fd0: 7329 2e0a 0a20 2020 2050 7269 6e74 7320  s)...    Prints 
+00017fe0: 7468 6520 6465 7461 696c 7320 6f66 2074  the details of t
+00017ff0: 6865 2073 6f6e 6728 7329 2077 6974 6820  he song(s) with 
+00018000: 7468 6520 4944 2873 2920 534f 4e47 5f49  the ID(s) SONG_I
+00018010: 4453 2e0a 0a20 2020 205c 620a 2020 2020  DS...    \b.    
+00018020: 4f75 7470 7574 2066 6f72 6d61 743a 0a20  Output format:. 
+00018030: 2020 2020 2020 2049 442c 206e 616d 652c         ID, name,
+00018040: 2064 7572 6174 696f 6e2c 206c 6973 7465   duration, liste
+00018050: 6e20 7469 6d65 2c20 7469 6d65 7320 6c69  n time, times li
+00018060: 7374 656e 6564 2c20 5b63 6c69 702d 7374  stened, [clip-st
+00018070: 6172 742c 2063 6c69 702d 656e 645d 2069  art, clip-end] i
+00018080: 6620 636c 6970 2065 7869 7374 732c 2063  f clip exists, c
+00018090: 6f6d 6d61 2d73 6570 6172 6174 6564 2074  omma-separated t
+000180a0: 6167 7320 6966 2061 6e79 0a20 2020 2020  ags if any.     
+000180b0: 2020 2061 7274 6973 7420 2d20 616c 6275     artist - albu
+000180c0: 6d20 2861 6c62 756d 2061 7274 6973 7429  m (album artist)
+000180d0: 2069 6620 2d49 2f2d 2d73 6f6e 672d 696e   if -I/--song-in
+000180e0: 666f 2069 7320 7061 7373 6564 0a20 2020  fo is passed.   
+000180f0: 2022 2222 0a20 2020 2073 6f6e 675f 6964   """.    song_id
+00018100: 7320 3d20 7365 7428 736f 6e67 5f69 6473  s = set(song_ids
+00018110: 290a 0a20 2020 2069 6620 7965 6172 2069  )..    if year i
+00018120: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00018130: 7374 6174 735f 7061 7468 203d 2054 4f54  stats_path = TOT
+00018140: 414c 5f53 5441 5453 5f50 4154 480a 2020  AL_STATS_PATH.  
+00018150: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00018160: 6966 2079 6561 7220 3d3d 2022 6375 7222  if year == "cur"
+00018170: 3a0a 2020 2020 2020 2020 2020 2020 7965  :.            ye
+00018180: 6172 203d 2043 5552 5f59 4541 520a 2020  ar = CUR_YEAR.  
+00018190: 2020 2020 2020 2020 2020 7374 6174 735f            stats_
+000181a0: 7061 7468 203d 2043 5552 5f59 4541 525f  path = CUR_YEAR_
+000181b0: 5354 4154 535f 5041 5448 0a20 2020 2020  STATS_PATH.     
+000181c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000181d0: 2020 2020 2069 6620 6e6f 7420 7965 6172       if not year
+000181e0: 2e69 7364 6967 6974 2829 3a0a 2020 2020  .isdigit():.    
+000181f0: 2020 2020 2020 2020 2020 2020 636c 6963              clic
+00018200: 6b2e 7365 6368 6f28 2259 6561 7220 6d75  k.secho("Year mu
+00018210: 7374 2062 6520 6120 6e75 6d62 6572 2e22  st be a number."
+00018220: 2c20 6667 3d22 7265 6422 290a 2020 2020  , fg="red").    
+00018230: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00018240: 726e 0a20 2020 2020 2020 2020 2020 2073  rn.            s
+00018250: 7461 7473 5f70 6174 6820 3d20 6f73 2e70  tats_path = os.p
+00018260: 6174 682e 6a6f 696e 2853 5441 5453 5f44  ath.join(STATS_D
+00018270: 4952 2c20 6622 7b79 6561 727d 2e74 7874  IR, f"{year}.txt
+00018280: 2229 0a0a 2020 2020 7472 793a 0a20 2020  ")..    try:.   
+00018290: 2020 2020 2077 6974 6820 280a 2020 2020       with (.    
+000182a0: 2020 2020 2020 2020 6f70 656e 2853 4f4e          open(SON
+000182b0: 4753 5f49 4e46 4f5f 5041 5448 2c20 2272  GS_INFO_PATH, "r
+000182c0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
+000182d0: 2d38 2229 2061 7320 736f 6e67 735f 6669  -8") as songs_fi
+000182e0: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+000182f0: 6f70 656e 2873 7461 7473 5f70 6174 682c  open(stats_path,
+00018300: 2022 7222 2c20 656e 636f 6469 6e67 3d22   "r", encoding="
+00018310: 7574 662d 3822 2920 6173 2073 7461 7473  utf-8") as stats
+00018320: 5f66 696c 652c 0a20 2020 2020 2020 2029  _file,.        )
+00018330: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
+00018340: 6e65 7320 3d20 736f 6e67 735f 6669 6c65  nes = songs_file
+00018350: 2e72 6561 646c 696e 6573 2829 0a20 2020  .readlines().   
+00018360: 2020 2020 2020 2020 2073 7461 7473 203d           stats =
+00018370: 2064 6963 7428 0a20 2020 2020 2020 2020   dict(.         
+00018380: 2020 2020 2020 206d 6170 280a 2020 2020         map(.    
 00018390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183a0: 6622 4e6f 2073 6f6e 6720 7769 7468 2049  f"No song with I
-000183b0: 4420 7b73 6f6e 675f 6964 7d20 666f 756e  D {song_id} foun
-000183c0: 642e 222c 0a20 2020 2020 2020 2020 2020  d.",.           
-000183d0: 2020 2020 2066 673d 2272 6564 222c 0a20       fg="red",. 
-000183e0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-000183f0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
-00018400: 0a20 2020 2069 6620 7061 6972 733a 0a20  .    if pairs:. 
-00018410: 2020 2020 2020 2070 6169 7273 203d 205b         pairs = [
-00018420: 7475 706c 6528 7061 6972 2e73 7472 6970  tuple(pair.strip
-00018430: 2829 2e73 706c 6974 2822 3a22 2929 2066  ().split(":")) f
-00018440: 6f72 2070 6169 7220 696e 2070 6169 7273  or pair in pairs
-00018450: 2e73 706c 6974 2822 7c22 295d 0a0a 2020  .split("|")]..  
-00018460: 2020 2020 2020 736f 6e67 5f64 6174 6120        song_data 
-00018470: 3d20 6d75 7369 635f 7461 672e 6c6f 6164  = music_tag.load
-00018480: 5f66 696c 6528 736f 6e67 5f70 6174 6829  _file(song_path)
-00018490: 0a20 2020 2020 2020 2076 616c 6964 5f70  .        valid_p
-000184a0: 6169 7273 203d 2070 6169 7273 5b3a 5d0a  airs = pairs[:].
-000184b0: 2020 2020 2020 2020 666f 7220 6b65 792c          for key,
-000184c0: 2076 616c 7565 2069 6e20 7061 6972 733a   value in pairs:
-000184d0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000184e0: 6b65 7920 6e6f 7420 696e 204d 4554 4144  key not in METAD
-000184f0: 4154 415f 4b45 5953 206f 7220 6b65 792e  ATA_KEYS or key.
-00018500: 7374 6172 7473 7769 7468 2822 2322 293a  startswith("#"):
-00018510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018520: 2063 6c69 636b 2e73 6563 686f 280a 2020   click.secho(.  
-00018530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018540: 2020 6622 277b 6b65 797d 2720 6973 206e    f"'{key}' is n
-00018550: 6f74 2061 2076 616c 6964 2065 6469 7461  ot a valid edita
-00018560: 626c 6520 6d65 7461 6461 7461 206b 6579  ble metadata key
-00018570: 2e22 2c20 6667 3d22 7265 6422 0a20 2020  .", fg="red".   
-00018580: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00018590: 2020 2020 2020 2020 2020 2020 2020 2076                 v
-000185a0: 616c 6964 5f70 6169 7273 2e72 656d 6f76  alid_pairs.remov
-000185b0: 6528 286b 6579 2c20 7661 6c75 6529 290a  e((key, value)).
-000185c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000185d0: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-000185e0: 2020 2020 2073 6f6e 675f 6461 7461 5b6b       song_data[k
-000185f0: 6579 5d20 3d20 7661 6c75 650a 0a20 2020  ey] = value..   
-00018600: 2020 2020 2073 6f6e 675f 6461 7461 2e73       song_data.s
-00018610: 6176 6528 290a 0a20 2020 2020 2020 2063  ave()..        c
-00018620: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
-00018630: 2020 2020 2020 2020 6622 5365 7420 6d65          f"Set me
-00018640: 7461 6461 7461 2066 6f72 2027 7b73 6f6e  tadata for '{son
-00018650: 675f 6e61 6d65 7d27 2077 6974 6820 4944  g_name}' with ID
-00018660: 207b 736f 6e67 5f69 647d 2074 6f20 7b76   {song_id} to {v
-00018670: 616c 6964 5f70 6169 7273 7d2e 222c 0a20  alid_pairs}.",. 
-00018680: 2020 2020 2020 2020 2020 2066 673d 2267             fg="g
-00018690: 7265 656e 222c 0a20 2020 2020 2020 2029  reen",.        )
-000186a0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-000186b0: 2020 2073 6f6e 675f 6461 7461 203d 206d     song_data = m
-000186c0: 7573 6963 5f74 6167 2e6c 6f61 645f 6669  usic_tag.load_fi
-000186d0: 6c65 2873 6f6e 675f 7061 7468 290a 2020  le(song_path).  
-000186e0: 2020 2020 2020 636c 6963 6b2e 6563 686f        click.echo
-000186f0: 2822 4d65 7461 6461 7461 2066 6f72 2022  ("Metadata for "
-00018700: 2c20 6e6c 3d46 616c 7365 290a 2020 2020  , nl=False).    
-00018710: 2020 2020 636c 6963 6b2e 7365 6368 6f28      click.secho(
-00018720: 736f 6e67 5f6e 616d 652c 2066 673d 2262  song_name, fg="b
-00018730: 6c75 6522 2c20 626f 6c64 3d54 7275 652c  lue", bold=True,
-00018740: 206e 6c3d 4661 6c73 6529 0a20 2020 2020   nl=False).     
-00018750: 2020 2063 6c69 636b 2e65 6368 6f28 6622     click.echo(f"
-00018760: 7769 7468 2049 4420 7b73 6f6e 675f 6964  with ID {song_id
-00018770: 7d3a 2229 0a0a 2020 2020 2020 2020 666f  }:")..        fo
-00018780: 7220 6b65 7920 696e 204d 4554 4144 4154  r key in METADAT
-00018790: 415f 4b45 5953 3a0a 2020 2020 2020 2020  A_KEYS:.        
-000187a0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-000187b0: 2020 2020 2020 2020 2063 6c69 636b 2e65           click.e
-000187c0: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
-000187d0: 2020 2020 2020 2020 2066 227b 6b65 7920           f"{key 
-000187e0: 6966 206e 6f74 206b 6579 2e73 7461 7274  if not key.start
-000187f0: 7377 6974 6828 2723 2729 2065 6c73 6520  swith('#') else 
-00018800: 6b65 795b 313a 5d7d 3a20 7b73 6f6e 675f  key[1:]}: {song_
-00018810: 6461 7461 5b6b 6579 5d2e 7661 6c75 657d  data[key].value}
-00018820: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00018830: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00018840: 6578 6365 7074 3a0a 2020 2020 2020 2020  except:.        
-00018850: 2020 2020 2020 2020 7061 7373 0a                 pass.
+000183a0: 6c61 6d62 6461 2074 3a20 2869 6e74 2874  lambda t: (int(t
+000183b0: 5b30 5d29 2c29 202b 2074 5b31 3a5d 2c20  [0]),) + t[1:], 
+000183c0: 2023 2063 6f6e 7665 7274 206b 6579 2074   # convert key t
+000183d0: 6f20 696e 740a 2020 2020 2020 2020 2020  o int.          
+000183e0: 2020 2020 2020 2020 2020 6d61 7028 0a20            map(. 
+000183f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018400: 2020 2020 2020 206c 616d 6264 6120 783a         lambda x:
+00018410: 2074 7570 6c65 286d 6170 2866 6c6f 6174   tuple(map(float
+00018420: 2c20 782e 7374 7269 7028 292e 7370 6c69  , x.strip().spli
+00018430: 7428 227c 2229 2929 2c0a 2020 2020 2020  t("|"))),.      
+00018440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018450: 2020 7374 6174 735f 6669 6c65 2e72 6561    stats_file.rea
+00018460: 646c 696e 6573 2829 2c0a 2020 2020 2020  dlines(),.      
+00018470: 2020 2020 2020 2020 2020 2020 2020 292c                ),
+00018480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018490: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
+000184a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000184b0: 2069 2069 6e20 7261 6e67 6528 6c65 6e28   i in range(len(
+000184c0: 6c69 6e65 7329 293a 0a20 2020 2020 2020  lines)):.       
+000184d0: 2020 2020 2020 2020 2064 6574 6169 6c73           details
+000184e0: 203d 206c 696e 6573 5b69 5d2e 7374 7269   = lines[i].stri
+000184f0: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
+00018500: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018510: 6f6e 675f 6964 203d 2069 6e74 2864 6574  ong_id = int(det
+00018520: 6169 6c73 5b30 5d29 0a20 2020 2020 2020  ails[0]).       
+00018530: 2020 2020 2020 2020 2069 6620 736f 6e67           if song
+00018540: 5f69 6420 696e 2073 6f6e 675f 6964 733a  _id in song_ids:
+00018550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018560: 2020 2020 2070 7269 6e74 5f65 6e74 7279       print_entry
+00018570: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00018580: 2020 2020 2020 2020 2020 6465 7461 696c            detail
+00018590: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000185a0: 2020 2020 2020 2020 2020 2b20 5b0a 2020            + [.  
+000185b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185c0: 2020 2020 2020 2020 2020 7374 6174 735b            stats[
+000185d0: 736f 6e67 5f69 645d 2c0a 2020 2020 2020  song_id],.      
+000185e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185f0: 2020 2020 2020 6d75 7369 635f 7461 672e        music_tag.
+00018600: 6c6f 6164 5f66 696c 6528 0a20 2020 2020  load_file(.     
+00018610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018620: 2020 2020 2020 2020 2020 206f 732e 7061             os.pa
+00018630: 7468 2e6a 6f69 6e28 534f 4e47 535f 4449  th.join(SONGS_DI
+00018640: 522c 2064 6574 6169 6c73 5b31 5d29 0a20  R, details[1]). 
+00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018660: 2020 2020 2020 2020 2020 2029 5b22 236c             )["#l
+00018670: 656e 6774 6822 5d2e 7661 6c75 652c 0a20  ength"].value,. 
+00018680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018690: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
+000186a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186b0: 2020 7368 6f77 5f73 6f6e 675f 696e 666f    show_song_info
+000186c0: 3d73 6f6e 675f 696e 666f 2c0a 2020 2020  =song_info,.    
+000186d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186e0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000186f0: 2020 2020 2020 736f 6e67 5f69 6473 2e72        song_ids.r
+00018700: 656d 6f76 6528 736f 6e67 5f69 6429 0a20  emove(song_id). 
+00018710: 2020 2065 7863 6570 7420 4669 6c65 4e6f     except FileNo
+00018720: 7446 6f75 6e64 4572 726f 723a 0a20 2020  tFoundError:.   
+00018730: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
+00018740: 2866 224e 6f20 7374 6174 7320 666f 756e  (f"No stats foun
+00018750: 6420 666f 7220 7965 6172 207b 7965 6172  d for year {year
+00018760: 7d2e 222c 2066 673d 2272 6564 2229 0a0a  }.", fg="red")..
+00018770: 2020 2020 6966 2073 6f6e 675f 6964 733a      if song_ids:
+00018780: 0a20 2020 2020 2020 2073 6f6e 675f 6964  .        song_id
+00018790: 7320 3d20 5b73 7472 2869 645f 2920 666f  s = [str(id_) fo
+000187a0: 7220 6964 5f20 696e 2073 6f6e 675f 6964  r id_ in song_id
+000187b0: 735d 0a20 2020 2020 2020 2063 6c69 636b  s].        click
+000187c0: 2e73 6563 686f 280a 2020 2020 2020 2020  .secho(.        
+000187d0: 2020 2020 6622 4e6f 2073 6f6e 6773 2066      f"No songs f
+000187e0: 6f75 6e64 2077 6974 6820 4944 733a 207b  ound with IDs: {
+000187f0: 272c 2027 2e6a 6f69 6e28 736f 6e67 5f69  ', '.join(song_i
+00018800: 6473 297d 2e22 2c20 6667 3d22 7265 6422  ds)}.", fg="red"
+00018810: 0a20 2020 2020 2020 2029 0a0a 0a40 636c  .        )...@cl
+00018820: 692e 636f 6d6d 616e 6428 290a 4063 6c69  i.command().@cli
+00018830: 636b 2e61 7267 756d 656e 7428 2273 6f6e  ck.argument("son
+00018840: 6722 2c20 7265 7175 6972 6564 3d54 7275  g", required=Tru
+00018850: 6529 0a40 636c 6963 6b2e 6f70 7469 6f6e  e).@click.option
+00018860: 280a 2020 2020 222d 4e2f 2d6e 4e22 2c0a  (.    "-N/-nN",.
+00018870: 2020 2020 222d 2d6e 616d 652f 2d2d 6e6f      "--name/--no
+00018880: 2d6e 616d 6522 2c0a 2020 2020 2274 6974  -name",.    "tit
+00018890: 6c65 222c 0a20 2020 2064 6566 6175 6c74  le",.    default
+000188a0: 3d46 616c 7365 2c0a 2020 2020 6865 6c70  =False,.    help
+000188b0: 3d22 5472 6561 7420 534f 4e47 2061 7320  ="Treat SONG as 
+000188c0: 6120 736f 6e67 206e 616d 6520 696e 7374  a song name inst
+000188d0: 6561 6420 6f66 2061 6e20 4944 2e22 2c0a  ead of an ID.",.
+000188e0: 290a 6465 6620 7265 636f 6d6d 656e 6428  ).def recommend(
+000188f0: 736f 6e67 2c20 7469 746c 6529 3a0a 2020  song, title):.  
+00018900: 2020 2222 220a 2020 2020 4765 7420 7265    """.    Get re
+00018910: 636f 6d6d 656e 6461 7469 6f6e 7320 6672  commendations fr
+00018920: 6f6d 2059 5420 4d75 7369 6320 6261 7365  om YT Music base
+00018930: 6420 6f6e 2073 6f6e 6720 7469 746c 6573  d on song titles
+00018940: 2e20 4e6f 7465 3a20 7468 6973 2066 6561  . Note: this fea
+00018950: 7475 7265 0a20 2020 2069 7320 6578 7065  ture.    is expe
+00018960: 7269 6d65 6e74 616c 2e0a 0a20 2020 2052  rimental...    R
+00018970: 6563 6f6d 6d65 6e64 7320 736f 6e67 7320  ecommends songs 
+00018980: 2870 6f73 7369 626c 7920 6578 706c 6963  (possibly explic
+00018990: 6974 2920 7573 696e 6720 7468 6520 596f  it) using the Yo
+000189a0: 7554 7562 6520 4d75 7369 6320 4150 4920  uTube Music API 
+000189b0: 7369 6d69 6c61 720a 2020 2020 746f 2074  similar.    to t
+000189c0: 6865 2073 6f6e 6720 7769 7468 2049 4420  he song with ID 
+000189d0: 534f 4e47 2074 6f20 6c69 7374 656e 2074  SONG to listen t
+000189e0: 6f2e 0a0a 2020 2020 4966 2074 6865 2027  o...    If the '
+000189f0: 2d4e 2720 666c 6167 2069 7320 7061 7373  -N' flag is pass
+00018a00: 6564 2c20 534f 4e47 2069 7320 7472 6561  ed, SONG is trea
+00018a10: 7465 6420 6173 2061 2073 6f6e 6720 6e61  ted as a song na
+00018a20: 6d65 2074 6f20 7365 6172 6368 2066 6f72  me to search for
+00018a30: 0a20 2020 206f 6e20 596f 7554 7562 6520  .    on YouTube 
+00018a40: 4d75 7369 632e 2222 220a 2020 2020 7472  Music.""".    tr
+00018a50: 793a 0a20 2020 2020 2020 2066 726f 6d20  y:.        from 
+00018a60: 7974 6d75 7369 6361 7069 2069 6d70 6f72  ytmusicapi impor
+00018a70: 7420 5954 4d75 7369 630a 2020 2020 6578  t YTMusic.    ex
+00018a80: 6365 7074 2049 6d70 6f72 7445 7272 6f72  cept ImportError
+00018a90: 3a0a 2020 2020 2020 2020 636c 6963 6b2e  :.        click.
+00018aa0: 7365 6368 6f28 0a20 2020 2020 2020 2020  secho(.         
+00018ab0: 2020 2022 5468 6520 2772 6563 6f6d 6d65     "The 'recomme
+00018ac0: 6e64 2720 636f 6d6d 616e 6420 7265 7175  nd' command requ
+00018ad0: 6972 6573 2074 6865 2027 7974 6d75 7369  ires the 'ytmusi
+00018ae0: 6361 7069 2720 7061 636b 6167 6520 746f  capi' package to
+00018af0: 2062 6520 696e 7374 616c 6c65 642e 2052   be installed. R
+00018b00: 756e 2027 7069 7020 696e 7374 616c 6c20  un 'pip install 
+00018b10: 7974 6d75 7369 6361 7069 2720 746f 2069  ytmusicapi' to i
+00018b20: 6e73 7461 6c6c 2069 742e 222c 0a20 2020  nstall it.",.   
+00018b30: 2020 2020 2020 2020 2066 673d 2272 6564           fg="red
+00018b40: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
+00018b50: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+00018b60: 2079 746d 7573 6963 203d 2059 544d 7573   ytmusic = YTMus
+00018b70: 6963 2829 0a0a 2020 2020 6966 2074 6974  ic()..    if tit
+00018b80: 6c65 3a0a 2020 2020 2020 2020 7265 7375  le:.        resu
+00018b90: 6c74 7320 3d20 7974 6d75 7369 632e 7365  lts = ytmusic.se
+00018ba0: 6172 6368 2873 6f6e 672c 2066 696c 7465  arch(song, filte
+00018bb0: 723d 2273 6f6e 6773 2229 0a20 2020 2065  r="songs").    e
+00018bc0: 6c73 653a 0a20 2020 2020 2020 2069 6620  lse:.        if 
+00018bd0: 6e6f 7420 736f 6e67 2e69 7364 6967 6974  not song.isdigit
+00018be0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00018bf0: 636c 6963 6b2e 7365 6368 6f28 0a20 2020  click.secho(.   
+00018c00: 2020 2020 2020 2020 2020 2020 2022 536f               "So
+00018c10: 6e67 2049 4420 6d75 7374 2062 6520 6120  ng ID must be a 
+00018c20: 6e75 6d62 6572 2e20 546f 2067 6574 2072  number. To get r
+00018c30: 6563 6f6d 6d65 6e64 6174 696f 6e73 2062  ecommendations b
+00018c40: 7920 6e61 6d65 2c20 7061 7373 2074 6865  y name, pass the
+00018c50: 2027 2d4e 2f2d 2d6e 616d 6527 2066 6c61   '-N/--name' fla
+00018c60: 672e 222c 0a20 2020 2020 2020 2020 2020  g.",.           
+00018c70: 2020 2020 2066 673d 2272 6564 222c 0a20       fg="red",. 
+00018c80: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00018c90: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00018ca0: 0a20 2020 2020 2020 2077 6974 6820 6f70  .        with op
+00018cb0: 656e 2853 4f4e 4753 5f49 4e46 4f5f 5041  en(SONGS_INFO_PA
+00018cc0: 5448 2c20 2272 222c 2065 6e63 6f64 696e  TH, "r", encodin
+00018cd0: 673d 2275 7466 2d38 2229 2061 7320 736f  g="utf-8") as so
+00018ce0: 6e67 735f 6669 6c65 3a0a 2020 2020 2020  ngs_file:.      
+00018cf0: 2020 2020 2020 666f 7220 6c69 6e65 2069        for line i
+00018d00: 6e20 736f 6e67 735f 6669 6c65 3a0a 2020  n songs_file:.  
+00018d10: 2020 2020 2020 2020 2020 2020 2020 6465                de
+00018d20: 7461 696c 7320 3d20 6c69 6e65 2e73 7472  tails = line.str
+00018d30: 6970 2829 2e73 706c 6974 2822 7c22 290a  ip().split("|").
+00018d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d50: 6966 2064 6574 6169 6c73 5b30 5d20 3d3d  if details[0] ==
+00018d60: 2073 6f6e 673a 0a20 2020 2020 2020 2020   song:.         
+00018d70: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00018d80: 7473 203d 2079 746d 7573 6963 2e73 6561  ts = ytmusic.sea
+00018d90: 7263 6828 0a20 2020 2020 2020 2020 2020  rch(.           
+00018da0: 2020 2020 2020 2020 2020 2020 206f 732e               os.
+00018db0: 7061 7468 2e73 706c 6974 6578 7428 6465  path.splitext(de
+00018dc0: 7461 696c 735b 315d 295b 305d 2c20 6669  tails[1])[0], fi
+00018dd0: 6c74 6572 3d22 736f 6e67 7322 0a20 2020  lter="songs".   
+00018de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018df0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+00018e00: 2020 2020 2020 2062 7265 616b 0a20 2020         break.   
+00018e10: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00018e20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00018e30: 6c69 636b 2e73 6563 686f 2866 224e 6f20  lick.secho(f"No 
+00018e40: 736f 6e67 2066 6f75 6e64 2077 6974 6820  song found with 
+00018e50: 4944 207b 736f 6e67 7d2e 222c 2066 673d  ID {song}.", fg=
+00018e60: 2272 6564 2229 0a20 2020 2020 2020 2020  "red").         
+00018e70: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+00018e80: 2020 2079 745f 6d75 7369 635f 706c 6179     yt_music_play
+00018e90: 6c69 7374 203d 2079 746d 7573 6963 2e67  list = ytmusic.g
+00018ea0: 6574 5f77 6174 6368 5f70 6c61 796c 6973  et_watch_playlis
+00018eb0: 7428 7265 7375 6c74 735b 305d 5b22 7669  t(results[0]["vi
+00018ec0: 6465 6f49 6422 5d29 0a0a 2020 2020 636c  deoId"])..    cl
+00018ed0: 6963 6b2e 6563 686f 2822 5265 636f 6d6d  ick.echo("Recomm
+00018ee0: 656e 6461 7469 6f6e 7320 666f 7220 222c  endations for ",
+00018ef0: 206e 6c3d 4661 6c73 6529 0a20 2020 2063   nl=False).    c
+00018f00: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
+00018f10: 2020 2020 7974 5f6d 7573 6963 5f70 6c61      yt_music_pla
+00018f20: 796c 6973 745b 2274 7261 636b 7322 5d5b  ylist["tracks"][
+00018f30: 305d 5b22 7469 746c 6522 5d20 2b20 2220  0]["title"] + " 
+00018f40: 222c 0a20 2020 2020 2020 2066 673d 2262  ",.        fg="b
+00018f50: 6c75 6522 2c0a 2020 2020 2020 2020 6e6c  lue",.        nl
+00018f60: 3d46 616c 7365 2c0a 2020 2020 290a 2020  =False,.    ).  
+00018f70: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
+00018f80: 2020 2020 2020 2066 2228 6874 7470 733a         f"(https:
+00018f90: 2f2f 6d75 7369 632e 796f 7574 7562 652e  //music.youtube.
+00018fa0: 636f 6d2f 7761 7463 683f 763d 7b79 745f  com/watch?v={yt_
+00018fb0: 6d75 7369 635f 706c 6179 6c69 7374 5b27  music_playlist['
+00018fc0: 7472 6163 6b73 275d 5b30 5d5b 2776 6964  tracks'][0]['vid
+00018fd0: 656f 4964 275d 7d29 222c 0a20 2020 2020  eoId']})",.     
+00018fe0: 2020 2066 673d 2262 7269 6768 745f 626c     fg="bright_bl
+00018ff0: 6163 6b22 2c0a 2020 2020 2020 2020 6e6c  ack",.        nl
+00019000: 3d46 616c 7365 2c0a 2020 2020 290a 2020  =False,.    ).  
+00019010: 2020 636c 6963 6b2e 6563 686f 2822 3a22    click.echo(":"
+00019020: 290a 2020 2020 666f 7220 7472 6163 6b20  ).    for track 
+00019030: 696e 2079 745f 6d75 7369 635f 706c 6179  in yt_music_play
+00019040: 6c69 7374 5b22 7472 6163 6b73 225d 5b31  list["tracks"][1
+00019050: 3a5d 3a0a 2020 2020 2020 2020 636c 6963  :]:.        clic
+00019060: 6b2e 7365 6368 6f28 7472 6163 6b5b 2274  k.secho(track["t
+00019070: 6974 6c65 225d 202b 2022 2022 2c20 6667  itle"] + " ", fg
+00019080: 3d22 626c 7565 222c 2062 6f6c 643d 5472  ="blue", bold=Tr
+00019090: 7565 2c20 6e6c 3d46 616c 7365 290a 2020  ue, nl=False).  
+000190a0: 2020 2020 2020 636c 6963 6b2e 7365 6368        click.sech
+000190b0: 6f28 0a20 2020 2020 2020 2020 2020 2066  o(.            f
+000190c0: 2268 7474 7073 3a2f 2f6d 7573 6963 2e79  "https://music.y
+000190d0: 6f75 7475 6265 2e63 6f6d 2f77 6174 6368  outube.com/watch
+000190e0: 3f76 3d7b 7472 6163 6b5b 2776 6964 656f  ?v={track['video
+000190f0: 4964 275d 7d22 2c0a 2020 2020 2020 2020  Id']}",.        
+00019100: 2020 2020 6667 3d22 6272 6967 6874 5f62      fg="bright_b
+00019110: 6c61 636b 222c 0a20 2020 2020 2020 2029  lack",.        )
+00019120: 0a0a 0a40 636c 692e 636f 6d6d 616e 6428  ...@cli.command(
+00019130: 290a 4063 6c69 636b 2e61 7267 756d 656e  ).@click.argumen
+00019140: 7428 2273 6f6e 675f 6964 7322 2c20 7265  t("song_ids", re
+00019150: 7175 6972 6564 3d54 7275 652c 2074 7970  quired=True, typ
+00019160: 653d 696e 742c 206e 6172 6773 3d2d 3129  e=int, nargs=-1)
+00019170: 0a40 636c 6963 6b2e 6f70 7469 6f6e 2822  .@click.option("
+00019180: 2d42 2f2d 6e42 222c 2022 2d2d 626f 7474  -B/-nB", "--bott
+00019190: 6f6d 2f2d 2d6e 6f2d 626f 7474 6f6d 222c  om/--no-bottom",
+000191a0: 2022 626f 7474 6f6d 222c 2064 6566 6175   "bottom", defau
+000191b0: 6c74 3d46 616c 7365 290a 6465 6620 7075  lt=False).def pu
+000191c0: 7368 2873 6f6e 675f 6964 732c 2062 6f74  sh(song_ids, bot
+000191d0: 746f 6d29 3a0a 2020 2020 2222 220a 2020  tom):.    """.  
+000191e0: 2020 4d6f 7665 2073 6f6e 6773 2061 726f    Move songs aro
+000191f0: 756e 6420 746f 2074 6865 2062 6f74 746f  und to the botto
+00019200: 6d20 6f72 2074 6f70 206f 6620 7468 6520  m or top of the 
+00019210: 6461 7461 6261 7365 2e0a 0a20 2020 2050  database...    P
+00019220: 7573 6820 7468 6520 736f 6e67 2873 2920  ush the song(s) 
+00019230: 7769 7468 2049 4428 7329 2053 4f4e 475f  with ID(s) SONG_
+00019240: 4944 5320 746f 2074 6865 2074 6f70 206f  IDS to the top o
+00019250: 6620 7468 6520 6461 7461 6261 7365 2028  f the database (
+00019260: 6173 2069 6620 7468 6579 0a20 2020 2077  as if they.    w
+00019270: 6572 6520 7468 6520 736f 6e67 7320 6d6f  ere the songs mo
+00019280: 7374 2072 6563 656e 746c 7920 6164 6465  st recently adde
+00019290: 6429 2069 6e20 7468 6520 6f72 6465 7220  d) in the order 
+000192a0: 7468 6579 2061 7265 2070 6173 7365 6420  they are passed 
+000192b0: 2865 2e67 2e0a 2020 2020 276d 6165 7374  (e.g..    'maest
+000192c0: 726f 2070 7573 6820 3120 3220 3327 2077  ro push 1 2 3' w
+000192d0: 696c 6c20 6d61 6b65 2074 6865 206d 6f73  ill make the mos
+000192e0: 7420 7265 6365 6e74 2073 6f6e 6720 6265  t recent song be
+000192f0: 2033 292e 0a0a 2020 2020 4966 2074 6865   3)...    If the
+00019300: 2027 2d42 2720 666c 6167 2069 7320 7061   '-B' flag is pa
+00019310: 7373 6564 2c20 7468 6520 736f 6e67 2873  ssed, the song(s
+00019320: 2920 7769 6c6c 2062 6520 7075 7368 6564  ) will be pushed
+00019330: 2074 6f20 7468 6520 626f 7474 6f6d 206f   to the bottom o
+00019340: 6620 7468 650a 2020 2020 6c69 7374 2069  f the.    list i
+00019350: 6e73 7465 6164 2e0a 2020 2020 2222 220a  nstead..    """.
+00019360: 2020 2020 7769 7468 206f 7065 6e28 534f      with open(SO
+00019370: 4e47 535f 494e 464f 5f50 4154 482c 2022  NGS_INFO_PATH, "
+00019380: 722b 222c 2065 6e63 6f64 696e 673d 2275  r+", encoding="u
+00019390: 7466 2d38 2229 2061 7320 736f 6e67 735f  tf-8") as songs_
+000193a0: 6669 6c65 3a0a 2020 2020 2020 2020 6c69  file:.        li
+000193b0: 6e65 7320 3d20 736f 6e67 735f 6669 6c65  nes = songs_file
+000193c0: 2e72 6561 646c 696e 6573 2829 0a0a 2020  .readlines()..  
+000193d0: 2020 2020 2020 6c69 6e65 735f 746f 5f6d        lines_to_m
+000193e0: 6f76 6520 3d20 5b5d 0a20 2020 2020 2020  ove = [].       
+000193f0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00019400: 6c65 6e28 6c69 6e65 7329 293a 0a20 2020  len(lines)):.   
+00019410: 2020 2020 2020 2020 2069 6620 696e 7428           if int(
+00019420: 6c69 6e65 735b 695d 2e73 706c 6974 2822  lines[i].split("
+00019430: 7c22 295b 305d 2920 696e 2073 6f6e 675f  |")[0]) in song_
+00019440: 6964 733a 0a20 2020 2020 2020 2020 2020  ids:.           
+00019450: 2020 2020 206c 696e 6573 5f74 6f5f 6d6f       lines_to_mo
+00019460: 7665 2e61 7070 656e 6428 2869 2c20 6c69  ve.append((i, li
+00019470: 6e65 735b 695d 2929 0a0a 2020 2020 2020  nes[i]))..      
+00019480: 2020 666f 7220 692c 205f 2069 6e20 7265    for i, _ in re
+00019490: 7665 7273 6564 286c 696e 6573 5f74 6f5f  versed(lines_to_
+000194a0: 6d6f 7665 293a 0a20 2020 2020 2020 2020  move):.         
+000194b0: 2020 206c 696e 6573 2e70 6f70 2869 290a     lines.pop(i).
+000194c0: 0a20 2020 2020 2020 2073 6f6e 675f 6964  .        song_id
+000194d0: 735f 7769 7468 5f6f 7264 6572 203d 2064  s_with_order = d
+000194e0: 6963 7428 0a20 2020 2020 2020 2020 2020  ict(.           
+000194f0: 206d 6170 286c 616d 6264 6120 783a 2028   map(lambda x: (
+00019500: 785b 315d 2c20 785b 305d 292c 2065 6e75  x[1], x[0]), enu
+00019510: 6d65 7261 7465 2873 6f6e 675f 6964 7329  merate(song_ids)
+00019520: 290a 2020 2020 2020 2020 290a 0a20 2020  ).        )..   
+00019530: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00019540: 6e67 6528 6c65 6e28 6c69 6e65 735f 746f  nge(len(lines_to
+00019550: 5f6d 6f76 6529 293a 0a20 2020 2020 2020  _move)):.       
+00019560: 2020 2020 206c 696e 6573 5f74 6f5f 6d6f       lines_to_mo
+00019570: 7665 5b69 5d20 3d20 280a 2020 2020 2020  ve[i] = (.      
+00019580: 2020 2020 2020 2020 2020 736f 6e67 5f69            song_i
+00019590: 6473 5f77 6974 685f 6f72 6465 725b 696e  ds_with_order[in
+000195a0: 7428 6c69 6e65 735f 746f 5f6d 6f76 655b  t(lines_to_move[
+000195b0: 695d 5b31 5d2e 7370 6c69 7428 227c 2229  i][1].split("|")
+000195c0: 5b30 5d29 5d2c 0a20 2020 2020 2020 2020  [0])],.         
+000195d0: 2020 2020 2020 202a 6c69 6e65 735f 746f         *lines_to
+000195e0: 5f6d 6f76 655b 695d 2c0a 2020 2020 2020  _move[i],.      
+000195f0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00019600: 206c 696e 6573 5f74 6f5f 6d6f 7665 2e73   lines_to_move.s
+00019610: 6f72 7428 6b65 793d 6c61 6d62 6461 2078  ort(key=lambda x
+00019620: 3a20 785b 305d 2c20 7265 7665 7273 653d  : x[0], reverse=
+00019630: 626f 7474 6f6d 290a 0a20 2020 2020 2020  bottom)..       
+00019640: 2069 6620 6e6f 7420 626f 7474 6f6d 3a0a   if not bottom:.
+00019650: 2020 2020 2020 2020 2020 2020 6c69 6e65              line
+00019660: 7320 2b3d 205b 745b 325d 2066 6f72 2074  s += [t[2] for t
+00019670: 2069 6e20 6c69 6e65 735f 746f 5f6d 6f76   in lines_to_mov
+00019680: 655d 0a20 2020 2020 2020 2065 6c73 653a  e].        else:
+00019690: 0a20 2020 2020 2020 2020 2020 206c 696e  .            lin
+000196a0: 6573 203d 205b 745b 325d 2066 6f72 2074  es = [t[2] for t
+000196b0: 2069 6e20 6c69 6e65 735f 746f 5f6d 6f76   in lines_to_mov
+000196c0: 655d 202b 206c 696e 6573 0a0a 2020 2020  e] + lines..    
+000196d0: 2020 2020 736f 6e67 735f 6669 6c65 2e73      songs_file.s
+000196e0: 6565 6b28 3029 0a20 2020 2020 2020 2073  eek(0).        s
+000196f0: 6f6e 6773 5f66 696c 652e 7772 6974 6528  ongs_file.write(
+00019700: 2222 2e6a 6f69 6e28 6c69 6e65 7329 290a  "".join(lines)).
+00019710: 2020 2020 2020 2020 736f 6e67 735f 6669          songs_fi
+00019720: 6c65 2e74 7275 6e63 6174 6528 290a 0a0a  le.truncate()...
+00019730: 4063 6c69 2e63 6f6d 6d61 6e64 286e 616d  @cli.command(nam
+00019740: 653d 2263 6c69 7022 290a 4063 6c69 636b  e="clip").@click
+00019750: 2e61 7267 756d 656e 7428 2273 6f6e 675f  .argument("song_
+00019760: 6964 222c 2072 6571 7569 7265 643d 5472  id", required=Tr
+00019770: 7565 2c20 7479 7065 3d69 6e74 290a 4063  ue, type=int).@c
+00019780: 6c69 636b 2e61 7267 756d 656e 7428 2273  lick.argument("s
+00019790: 7461 7274 222c 2072 6571 7569 7265 643d  tart", required=
+000197a0: 4661 6c73 652c 2074 7970 653d 666c 6f61  False, type=floa
+000197b0: 742c 2064 6566 6175 6c74 3d4e 6f6e 6529  t, default=None)
+000197c0: 0a40 636c 6963 6b2e 6172 6775 6d65 6e74  .@click.argument
+000197d0: 2822 656e 6422 2c20 7265 7175 6972 6564  ("end", required
+000197e0: 3d46 616c 7365 2c20 7479 7065 3d66 6c6f  =False, type=flo
+000197f0: 6174 2c20 6465 6661 756c 743d 4e6f 6e65  at, default=None
+00019800: 290a 6465 6620 636c 6970 5f28 736f 6e67  ).def clip_(song
+00019810: 5f69 642c 2073 7461 7274 2c20 656e 6429  _id, start, end)
+00019820: 3a0a 2020 2020 2222 220a 2020 2020 4372  :.    """.    Cr
+00019830: 6561 7465 206f 7220 6564 6974 2074 6865  eate or edit the
+00019840: 2063 6c69 7020 666f 7220 6120 736f 6e67   clip for a song
+00019850: 2e0a 0a20 2020 2053 6574 7320 7468 6520  ...    Sets the 
+00019860: 636c 6970 2066 6f72 2074 6865 2073 6f6e  clip for the son
+00019870: 6720 7769 7468 2049 4420 534f 4e47 5f49  g with ID SONG_I
+00019880: 4420 746f 2074 6865 2074 696d 6520 7261  D to the time ra
+00019890: 6e67 6520 5354 4152 5420 746f 2045 4e44  nge START to END
+000198a0: 0a20 2020 2028 696e 2073 6563 6f6e 6473  .    (in seconds
+000198b0: 292e 0a0a 2020 2020 4966 2045 4e44 2069  )...    If END i
+000198c0: 7320 6e6f 7420 7061 7373 6564 2c20 7468  s not passed, th
+000198d0: 6520 636c 6970 2077 696c 6c20 6265 2066  e clip will be f
+000198e0: 726f 6d20 5354 4152 5420 746f 2074 6865  rom START to the
+000198f0: 2065 6e64 206f 6620 7468 6520 736f 6e67   end of the song
+00019900: 2e0a 0a20 2020 2049 6620 6e65 6974 6865  ...    If neithe
+00019910: 7220 5354 4152 5420 6e6f 7220 454e 4420  r START nor END 
+00019920: 6172 6520 7061 7373 6564 2c20 6120 636c  are passed, a cl
+00019930: 6970 2065 6469 746f 7220 7769 6c6c 2062  ip editor will b
+00019940: 6520 6f70 656e 6564 2c20 696e 2077 6869  e opened, in whi
+00019950: 6368 0a20 2020 2079 6f75 2063 616e 206d  ch.    you can m
+00019960: 6f76 6520 7468 6520 7374 6172 7420 616e  ove the start an
+00019970: 6420 656e 6420 6f66 2074 6865 2063 6c69  d end of the cli
+00019980: 7020 6172 6f75 6e64 2075 7369 6e67 2074  p around using t
+00019990: 6865 2061 7272 6f77 206b 6579 7320 7768  he arrow keys wh
+000199a0: 696c 650a 2020 2020 6c69 7374 656e 696e  ile.    listenin
+000199b0: 6720 746f 2074 6865 2073 6f6e 6720 2861  g to the song (a
+000199c0: 6c73 6f20 7368 6f77 7320 7761 7665 666f  lso shows wavefo
+000199d0: 726d 292e 0a0a 2020 2020 5c62 0a20 2020  rm)...    \b.   
+000199e0: 2054 6865 2065 6469 746f 7220 7374 6172   The editor star
+000199f0: 7473 206f 7574 2065 6469 7469 6e67 2074  ts out editing t
+00019a00: 6865 2073 7461 7274 206f 6620 7468 6520  he start of the 
+00019a10: 636c 6970 2e0a 2020 2020 5c78 3162 5b31  clip..    \x1b[1
+00019a20: 6d74 5c78 3162 5b30 6d20 746f 2074 6f67  mt\x1b[0m to tog
+00019a30: 676c 6520 6265 7477 6565 6e20 6564 6974  gle between edit
+00019a40: 696e 6720 7468 6520 7374 6172 7420 616e  ing the start an
+00019a50: 6420 656e 6420 6f66 2074 6865 2063 6c69  d end of the cli
+00019a60: 702e 0a20 2020 205c 7831 625b 316d 5348  p..    \x1b[1mSH
+00019a70: 4946 542b 4c45 4654 2f52 4947 4854 5c78  IFT+LEFT/RIGHT\x
+00019a80: 3162 5b30 6d20 7769 6c6c 206d 6f76 6520  1b[0m will move 
+00019a90: 7768 6963 6865 7665 7220 636c 6970 2065  whichever clip e
+00019aa0: 6e64 2079 6f75 2061 7265 2065 6469 7469  nd you are editi
+00019ab0: 6e67 0a20 2020 2020 2020 2062 7920 302e  ng.        by 0.
+00019ac0: 3120 7365 636f 6e64 732c 2073 6e61 7020  1 seconds, snap 
+00019ad0: 7468 6520 6375 7272 656e 7420 706c 6179  the current play
+00019ae0: 6261 636b 2074 6f20 7468 6174 2063 6c69  back to that cli
+00019af0: 7020 656e 6420 2874 6f20 6578 6163 746c  p end (to exactl
+00019b00: 790a 2020 2020 2020 2020 7468 6520 636c  y.        the cl
+00019b10: 6970 2073 7461 7274 2069 6620 6564 6974  ip start if edit
+00019b20: 696e 6720 7374 6172 742c 2065 6e64 2d31  ing start, end-1
+00019b30: 2069 6620 6564 6974 696e 6720 656e 6429   if editing end)
+00019b40: 2c20 616e 6420 7061 7573 652e 0a20 2020  , and pause..   
+00019b50: 205c 7831 625b 316d 4c45 4654 2f52 4947   \x1b[1mLEFT/RIG
+00019b60: 4854 5c78 3162 5b30 6d20 7769 6c6c 206d  HT\x1b[0m will m
+00019b70: 6f76 6520 7768 6963 6865 7665 7220 636c  ove whichever cl
+00019b80: 6970 2065 6e64 2079 6f75 2061 7265 2065  ip end you are e
+00019b90: 6469 7469 6e67 2062 7920 310a 2020 2020  diting by 1.    
+00019ba0: 2020 2020 7365 636f 6e64 2c20 736e 6170      second, snap
+00019bb0: 2074 6865 2063 7572 7265 6e74 2070 6c61   the current pla
+00019bc0: 7962 6163 6b20 746f 2074 6861 7420 636c  yback to that cl
+00019bd0: 6970 2065 6e64 2c20 616e 6420 7061 7573  ip end, and paus
+00019be0: 652e 0a20 2020 205c 7831 625b 316d 454e  e..    \x1b[1mEN
+00019bf0: 5445 525c 7831 625b 306d 2077 696c 6c20  TER\x1b[0m will 
+00019c00: 6578 6974 2074 6865 2065 6469 746f 7220  exit the editor 
+00019c10: 616e 6420 7361 7665 2074 6865 2063 6c69  and save the cli
+00019c20: 702e 0a20 2020 205c 7831 625b 316d 715c  p..    \x1b[1mq\
+00019c30: 7831 625b 306d 2077 696c 6c20 6578 6974  x1b[0m will exit
+00019c40: 2074 6865 2065 6469 746f 7220 7769 7468   the editor with
+00019c50: 6f75 7420 7361 7669 6e67 2074 6865 2063  out saving the c
+00019c60: 6c69 702e 0a20 2020 2022 2222 0a20 2020  lip..    """.   
+00019c70: 2069 6620 7374 6172 7420 6973 206e 6f74   if start is not
+00019c80: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
+00019c90: 6620 7374 6172 7420 3c20 303a 0a20 2020  f start < 0:.   
+00019ca0: 2020 2020 2020 2020 2063 6c69 636b 2e73           click.s
+00019cb0: 6563 686f 2822 5354 4152 5420 6d75 7374  echo("START must
+00019cc0: 2062 6520 6120 706f 7369 7469 7665 206e   be a positive n
+00019cd0: 756d 6265 722e 222c 2066 673d 2272 6564  umber.", fg="red
+00019ce0: 2229 0a20 2020 2020 2020 2020 2020 2072  ").            r
+00019cf0: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
+00019d00: 2065 6e64 2069 7320 6e6f 7420 4e6f 6e65   end is not None
+00019d10: 2061 6e64 2065 6e64 203c 2030 3a0a 2020   and end < 0:.  
+00019d20: 2020 2020 2020 2020 2020 636c 6963 6b2e            click.
+00019d30: 7365 6368 6f28 2245 4e44 206d 7573 7420  secho("END must 
+00019d40: 6265 2061 2070 6f73 6974 6976 6520 6e75  be a positive nu
+00019d50: 6d62 6572 2e22 2c20 6667 3d22 7265 6422  mber.", fg="red"
+00019d60: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
+00019d70: 7475 726e 0a0a 2020 2020 7769 7468 206f  turn..    with o
+00019d80: 7065 6e28 534f 4e47 535f 494e 464f 5f50  pen(SONGS_INFO_P
+00019d90: 4154 482c 2022 722b 222c 2065 6e63 6f64  ATH, "r+", encod
+00019da0: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+00019db0: 736f 6e67 735f 6669 6c65 3a0a 2020 2020  songs_file:.    
+00019dc0: 2020 2020 6c69 6e65 7320 3d20 736f 6e67      lines = song
+00019dd0: 735f 6669 6c65 2e72 6561 646c 696e 6573  s_file.readlines
+00019de0: 2829 0a0a 2020 2020 2020 2020 666f 7220  ()..        for 
+00019df0: 6920 696e 2072 616e 6765 286c 656e 286c  i in range(len(l
+00019e00: 696e 6573 2929 3a0a 2020 2020 2020 2020  ines)):.        
+00019e10: 2020 2020 6465 7461 696c 7320 3d20 6c69      details = li
+00019e20: 6e65 735b 695d 2e73 7472 6970 2829 2e73  nes[i].strip().s
+00019e30: 706c 6974 2822 7c22 290a 2020 2020 2020  plit("|").      
+00019e40: 2020 2020 2020 6966 2069 6e74 2864 6574        if int(det
+00019e50: 6169 6c73 5b30 5d29 203d 3d20 736f 6e67  ails[0]) == song
+00019e60: 5f69 643a 0a20 2020 2020 2020 2020 2020  _id:.           
+00019e70: 2020 2020 2062 7265 616b 0a20 2020 2020       break.     
+00019e80: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00019e90: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
+00019ea0: 2866 224e 6f20 736f 6e67 2066 6f75 6e64  (f"No song found
+00019eb0: 2077 6974 6820 4944 207b 736f 6e67 5f69   with ID {song_i
+00019ec0: 647d 2e22 2c20 6667 3d22 7265 6422 290a  d}.", fg="red").
+00019ed0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00019ee0: 726e 0a0a 2020 2020 2020 2020 736f 6e67  rn..        song
+00019ef0: 5f6e 616d 6520 3d20 6465 7461 696c 735b  _name = details[
+00019f00: 315d 0a0a 2020 2020 2020 2020 6966 2073  1]..        if s
+00019f10: 7461 7274 2069 7320 4e6f 6e65 3a20 2023  tart is None:  #
+00019f20: 2063 6c69 7020 6564 6974 6f72 0a20 2020   clip editor.   
+00019f30: 2020 2020 2020 2020 2073 7461 7274 2c20           start, 
+00019f40: 656e 6420 3d20 6375 7273 6573 2e77 7261  end = curses.wra
+00019f50: 7070 6572 2863 6c69 705f 6564 6974 6f72  pper(clip_editor
+00019f60: 2c20 6465 7461 696c 7329 0a20 2020 2020  , details).     
+00019f70: 2020 2020 2020 2069 6620 7374 6172 7420         if start 
+00019f80: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00019f90: 2020 2020 2020 2020 2063 6c69 636b 2e73           click.s
+00019fa0: 6563 686f 2866 224e 6f20 6368 616e 6765  echo(f"No change
+00019fb0: 2069 6e20 636c 6970 2066 6f72 207b 736f   in clip for {so
+00019fc0: 6e67 5f6e 616d 657d 2e22 2c20 6667 3d22  ng_name}.", fg="
+00019fd0: 6772 6565 6e22 290a 2020 2020 2020 2020  green").        
+00019fe0: 2020 2020 2020 2020 7265 7475 726e 0a0a          return..
+00019ff0: 2020 2020 2020 2020 736f 6e67 5f70 6174          song_pat
+0001a000: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+0001a010: 2853 4f4e 4753 5f44 4952 2c20 736f 6e67  (SONGS_DIR, song
+0001a020: 5f6e 616d 6529 0a20 2020 2020 2020 2064  _name).        d
+0001a030: 7572 6174 696f 6e20 3d20 6d75 7369 635f  uration = music_
+0001a040: 7461 672e 6c6f 6164 5f66 696c 6528 736f  tag.load_file(so
+0001a050: 6e67 5f70 6174 6829 5b22 236c 656e 6774  ng_path)["#lengt
+0001a060: 6822 5d2e 7661 6c75 650a 0a20 2020 2020  h"].value..     
+0001a070: 2020 2069 6620 656e 6420 6973 204e 6f6e     if end is Non
+0001a080: 653a 0a20 2020 2020 2020 2020 2020 2065  e:.            e
+0001a090: 6e64 203d 2064 7572 6174 696f 6e0a 0a20  nd = duration.. 
+0001a0a0: 2020 2020 2020 2069 6620 7374 6172 7420         if start 
+0001a0b0: 3e20 6475 7261 7469 6f6e 3a0a 2020 2020  > duration:.    
+0001a0c0: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
+0001a0d0: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+0001a0e0: 2020 2020 2022 5354 4152 5420 6d75 7374       "START must
+0001a0f0: 206e 6f74 2062 6520 6d6f 7265 2074 6861   not be more tha
+0001a100: 6e20 7468 6520 736f 6e67 2064 7572 6174  n the song durat
+0001a110: 696f 6e2e 222c 2066 673d 2272 6564 220a  ion.", fg="red".
+0001a120: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0001a130: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0001a140: 0a20 2020 2020 2020 2069 6620 656e 6420  .        if end 
+0001a150: 3e20 6475 7261 7469 6f6e 3a0a 2020 2020  > duration:.    
+0001a160: 2020 2020 2020 2020 636c 6963 6b2e 7365          click.se
+0001a170: 6368 6f28 0a20 2020 2020 2020 2020 2020  cho(.           
+0001a180: 2020 2020 2022 454e 4420 6d75 7374 206e       "END must n
+0001a190: 6f74 2062 6520 6d6f 7265 2074 6861 6e20  ot be more than 
+0001a1a0: 7468 6520 736f 6e67 2064 7572 6174 696f  the song duratio
+0001a1b0: 6e2e 222c 2066 673d 2272 6564 220a 2020  n.", fg="red".  
+0001a1c0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0001a1d0: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+0001a1e0: 2020 2020 2020 2069 6620 7374 6172 7420         if start 
+0001a1f0: 3e20 656e 643a 0a20 2020 2020 2020 2020  > end:.         
+0001a200: 2020 2063 6c69 636b 2e73 6563 686f 2822     click.secho("
+0001a210: 5354 4152 5420 6d75 7374 206e 6f74 2062  START must not b
+0001a220: 6520 6d6f 7265 2074 6861 6e20 454e 442e  e more than END.
+0001a230: 222c 2066 673d 2272 6564 2229 0a20 2020  ", fg="red").   
+0001a240: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+0001a250: 0a20 2020 2020 2020 206c 696e 6573 5b69  .        lines[i
+0001a260: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
+0001a270: 2020 227c 222e 6a6f 696e 2864 6574 6169    "|".join(detai
+0001a280: 6c73 5b3a 335d 202b 205b 7374 7228 7374  ls[:3] + [str(st
+0001a290: 6172 7429 202b 2022 2022 202b 2073 7472  art) + " " + str
+0001a2a0: 2865 6e64 295d 202b 2064 6574 6169 6c73  (end)] + details
+0001a2b0: 5b35 3a5d 290a 2020 2020 2020 2020 2020  [5:]).          
+0001a2c0: 2020 2b20 225c 6e22 0a20 2020 2020 2020    + "\n".       
+0001a2d0: 2029 0a0a 2020 2020 2020 2020 736f 6e67   )..        song
+0001a2e0: 735f 6669 6c65 2e73 6565 6b28 3029 0a20  s_file.seek(0). 
+0001a2f0: 2020 2020 2020 2073 6f6e 6773 5f66 696c         songs_fil
+0001a300: 652e 7772 6974 6528 2222 2e6a 6f69 6e28  e.write("".join(
+0001a310: 6c69 6e65 7329 290a 2020 2020 2020 2020  lines)).        
+0001a320: 736f 6e67 735f 6669 6c65 2e74 7275 6e63  songs_file.trunc
+0001a330: 6174 6528 290a 0a20 2020 2020 2020 2063  ate()..        c
+0001a340: 6c69 636b 2e73 6563 686f 2866 2243 6c69  lick.secho(f"Cli
+0001a350: 7070 6564 207b 736f 6e67 5f6e 616d 657d  pped {song_name}
+0001a360: 2066 726f 6d20 7b73 7461 7274 7d20 746f   from {start} to
+0001a370: 207b 656e 647d 2e22 2c20 6667 3d22 6772   {end}.", fg="gr
+0001a380: 6565 6e22 290a 0a0a 4063 6c69 2e63 6f6d  een")...@cli.com
+0001a390: 6d61 6e64 2829 0a40 636c 6963 6b2e 6172  mand().@click.ar
+0001a3a0: 6775 6d65 6e74 2822 736f 6e67 5f69 6473  gument("song_ids
+0001a3b0: 222c 2074 7970 653d 696e 742c 206e 6172  ", type=int, nar
+0001a3c0: 6773 3d2d 312c 2072 6571 7569 7265 643d  gs=-1, required=
+0001a3d0: 4661 6c73 6529 0a40 636c 6963 6b2e 6f70  False).@click.op
+0001a3e0: 7469 6f6e 280a 2020 2020 222d 412f 2d6e  tion(.    "-A/-n
+0001a3f0: 4122 2c0a 2020 2020 222d 2d61 6c6c 2f2d  A",.    "--all/-
+0001a400: 2d6e 6f2d 616c 6c22 2c0a 2020 2020 2261  -no-all",.    "a
+0001a410: 6c6c 5f22 2c0a 2020 2020 6465 6661 756c  ll_",.    defaul
+0001a420: 743d 4661 6c73 652c 0a20 2020 2068 656c  t=False,.    hel
+0001a430: 703d 2252 656d 6f76 6520 636c 6970 7320  p="Remove clips 
+0001a440: 666f 7220 616c 6c20 736f 6e67 732e 2049  for all songs. I
+0001a450: 676e 6f72 6573 2053 4f4e 475f 4944 532e  gnores SONG_IDS.
+0001a460: 222c 0a29 0a40 636c 6963 6b2e 6f70 7469  ",.).@click.opti
+0001a470: 6f6e 2822 2d46 2f2d 6e46 222c 2022 2d2d  on("-F/-nF", "--
+0001a480: 666f 7263 652f 2d2d 6e6f 2d66 6f72 6365  force/--no-force
+0001a490: 222c 2022 666f 7263 6522 2c20 6465 6661  ", "force", defa
+0001a4a0: 756c 743d 4661 6c73 6529 0a64 6566 2075  ult=False).def u
+0001a4b0: 6e63 6c69 7028 736f 6e67 5f69 6473 2c20  nclip(song_ids, 
+0001a4c0: 616c 6c5f 2c20 666f 7263 6529 3a0a 2020  all_, force):.  
+0001a4d0: 2020 2222 220a 2020 2020 5265 6d6f 7665    """.    Remove
+0001a4e0: 2063 6c69 7073 2066 6f72 2073 7065 6369   clips for speci
+0001a4f0: 6669 6320 736f 6e67 2873 292e 0a0a 2020  fic song(s)...  
+0001a500: 2020 5265 6d6f 7665 7320 636c 6970 2066    Removes clip f
+0001a510: 6f72 2074 6865 2073 6f6e 6728 7329 2077  or the song(s) w
+0001a520: 6974 6820 4944 2873 2920 534f 4e47 5f49  ith ID(s) SONG_I
+0001a530: 4453 2e0a 0a20 2020 2049 6620 7468 6520  DS...    If the 
+0001a540: 272d 412f 2d2d 616c 6c27 2066 6c61 6720  '-A/--all' flag 
+0001a550: 6973 2070 6173 7365 642c 2074 6865 2063  is passed, the c
+0001a560: 6c69 7073 2066 6f72 2061 6c6c 2073 6f6e  lips for all son
+0001a570: 6773 2077 696c 6c20 6265 2072 656d 6f76  gs will be remov
+0001a580: 6564 2c0a 2020 2020 6967 6e6f 7269 6e67  ed,.    ignoring
+0001a590: 2053 4f4e 475f 4944 532e 2054 6869 7320   SONG_IDS. This 
+0001a5a0: 7072 6f6d 7074 7320 666f 7220 636f 6e66  prompts for conf
+0001a5b0: 6972 6d61 7469 6f6e 2075 6e6c 6573 7320  irmation unless 
+0001a5c0: 7468 6520 272d 462f 2d2d 666f 7263 6527  the '-F/--force'
+0001a5d0: 0a20 2020 2066 6c61 6720 6973 2070 6173  .    flag is pas
+0001a5e0: 7365 642e 0a20 2020 2022 2222 0a20 2020  sed..    """.   
+0001a5f0: 2069 6620 6e6f 7420 616c 6c5f 3a0a 2020   if not all_:.  
+0001a600: 2020 2020 2020 6966 2073 6f6e 675f 6964        if song_id
+0001a610: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+0001a620: 6f6e 675f 6964 7320 3d20 7365 7428 736f  ong_ids = set(so
+0001a630: 6e67 5f69 6473 290a 2020 2020 2020 2020  ng_ids).        
+0001a640: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0001a650: 2020 636c 6963 6b2e 7365 6368 6f28 0a20    click.secho(. 
+0001a660: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001a670: 4e6f 2073 6f6e 6720 4944 7320 7061 7373  No song IDs pass
+0001a680: 6564 2e20 546f 2072 656d 6f76 6520 636c  ed. To remove cl
+0001a690: 6970 7320 666f 7220 616c 6c20 736f 6e67  ips for all song
+0001a6a0: 732c 2070 6173 7320 7468 6520 272d 412f  s, pass the '-A/
+0001a6b0: 2d2d 616c 6c27 2066 6c61 672e 222c 0a20  --all' flag.",. 
+0001a6c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0001a6d0: 673d 2272 6564 222c 0a20 2020 2020 2020  g="red",.       
+0001a6e0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0001a6f0: 2020 2072 6574 7572 6e0a 0a20 2020 2069     return..    i
+0001a700: 6620 616c 6c5f 2061 6e64 206e 6f74 2066  f all_ and not f
+0001a710: 6f72 6365 3a0a 2020 2020 2020 2020 636c  orce:.        cl
+0001a720: 6963 6b2e 6563 686f 280a 2020 2020 2020  ick.echo(.      
+0001a730: 2020 2020 2020 2241 7265 2079 6f75 2073        "Are you s
+0001a740: 7572 6520 796f 7520 7761 6e74 2074 6f20  ure you want to 
+0001a750: 7265 6d6f 7665 2063 6c69 7073 2066 6f72  remove clips for
+0001a760: 2061 6c6c 2073 6f6e 6773 3f20 5468 6973   all songs? This
+0001a770: 2063 616e 6e6f 7420 6265 2075 6e64 6f6e   cannot be undon
+0001a780: 652e 205b 792f 6e5d 2022 2c0a 2020 2020  e. [y/n] ",.    
+0001a790: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
+0001a7a0: 2069 6e70 7574 2829 2e6c 6f77 6572 2829   input().lower()
+0001a7b0: 2021 3d20 2279 223a 0a20 2020 2020 2020   != "y":.       
+0001a7c0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
+0001a7d0: 2077 6974 6820 6f70 656e 2853 4f4e 4753   with open(SONGS
+0001a7e0: 5f49 4e46 4f5f 5041 5448 2c20 2272 2b22  _INFO_PATH, "r+"
+0001a7f0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
+0001a800: 3822 2920 6173 2073 6f6e 6773 5f66 696c  8") as songs_fil
+0001a810: 653a 0a20 2020 2020 2020 206c 696e 6573  e:.        lines
+0001a820: 203d 2073 6f6e 6773 5f66 696c 652e 7265   = songs_file.re
+0001a830: 6164 6c69 6e65 7328 290a 0a20 2020 2020  adlines()..     
+0001a840: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+0001a850: 6528 6c65 6e28 6c69 6e65 7329 293a 0a20  e(len(lines)):. 
+0001a860: 2020 2020 2020 2020 2020 2064 6574 6169             detai
+0001a870: 6c73 203d 206c 696e 6573 5b69 5d2e 7374  ls = lines[i].st
+0001a880: 7269 7028 292e 7370 6c69 7428 227c 2229  rip().split("|")
+0001a890: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001a8a0: 616c 6c5f 206f 7220 696e 7428 6465 7461  all_ or int(deta
+0001a8b0: 696c 735b 305d 2920 696e 2073 6f6e 675f  ils[0]) in song_
+0001a8c0: 6964 733a 0a20 2020 2020 2020 2020 2020  ids:.           
+0001a8d0: 2020 2020 206c 696e 6573 5b69 5d20 3d20       lines[i] = 
+0001a8e0: 227c 222e 6a6f 696e 2864 6574 6169 6c73  "|".join(details
+0001a8f0: 5b3a 335d 202b 205b 2222 5d20 2b20 6465  [:3] + [""] + de
+0001a900: 7461 696c 735b 353a 5d29 202b 2022 5c6e  tails[5:]) + "\n
+0001a910: 220a 0a20 2020 2020 2020 2073 6f6e 6773  "..        songs
+0001a920: 5f66 696c 652e 7365 656b 2830 290a 2020  _file.seek(0).  
+0001a930: 2020 2020 2020 736f 6e67 735f 6669 6c65        songs_file
+0001a940: 2e77 7269 7465 2822 222e 6a6f 696e 286c  .write("".join(l
+0001a950: 696e 6573 2929 0a20 2020 2020 2020 2073  ines)).        s
+0001a960: 6f6e 6773 5f66 696c 652e 7472 756e 6361  ongs_file.trunca
+0001a970: 7465 2829 0a0a 2020 2020 6966 2061 6c6c  te()..    if all
+0001a980: 5f3a 0a20 2020 2020 2020 2063 6c69 636b  _:.        click
+0001a990: 2e73 6563 686f 2822 5265 6d6f 7665 6420  .secho("Removed 
+0001a9a0: 636c 6970 7320 666f 7220 616c 6c20 736f  clips for all so
+0001a9b0: 6e67 732e 222c 2066 673d 2267 7265 656e  ngs.", fg="green
+0001a9c0: 2229 0a20 2020 2065 6c73 653a 0a20 2020  ").    else:.   
+0001a9d0: 2020 2020 2063 6c69 636b 2e73 6563 686f       click.secho
+0001a9e0: 280a 2020 2020 2020 2020 2020 2020 6622  (.            f"
+0001a9f0: 5265 6d6f 7665 6420 636c 6970 2873 2920  Removed clip(s) 
+0001aa00: 666f 7220 736f 6e67 2873 2920 7769 7468  for song(s) with
+0001aa10: 2049 4428 7329 207b 272c 2027 2e6a 6f69   ID(s) {', '.joi
+0001aa20: 6e28 6d61 7028 7374 722c 2073 6f6e 675f  n(map(str, song_
+0001aa30: 6964 7329 297d 2e22 2c0a 2020 2020 2020  ids))}.",.      
+0001aa40: 2020 2020 2020 6667 3d22 6772 6565 6e22        fg="green"
+0001aa50: 2c0a 2020 2020 2020 2020 290a 0a0a 4063  ,.        )...@c
+0001aa60: 6c69 2e63 6f6d 6d61 6e64 2829 0a40 636c  li.command().@cl
+0001aa70: 6963 6b2e 6172 6775 6d65 6e74 2822 736f  ick.argument("so
+0001aa80: 6e67 5f69 6422 2c20 7479 7065 3d69 6e74  ng_id", type=int
+0001aa90: 2c20 7265 7175 6972 6564 3d54 7275 6529  , required=True)
+0001aaa0: 0a40 636c 6963 6b2e 6172 6775 6d65 6e74  .@click.argument
+0001aab0: 2822 7061 6972 7322 2c20 7479 7065 3d73  ("pairs", type=s
+0001aac0: 7472 2c20 7265 7175 6972 6564 3d46 616c  tr, required=Fal
+0001aad0: 7365 290a 6465 6620 6d65 7461 6461 7461  se).def metadata
+0001aae0: 2873 6f6e 675f 6964 2c20 7061 6972 7329  (song_id, pairs)
+0001aaf0: 3a0a 2020 2020 2222 220a 2020 2020 5669  :.    """.    Vi
+0001ab00: 6577 206f 7220 6564 6974 2074 6865 206d  ew or edit the m
+0001ab10: 6574 6164 6174 6120 666f 7220 6120 736f  etadata for a so
+0001ab20: 6e67 2e0a 0a20 2020 2049 6620 6e6f 2050  ng...    If no P
+0001ab30: 4149 5253 2061 7265 2070 6173 7365 642c  AIRS are passed,
+0001ab40: 2070 7269 6e74 7320 7468 6520 6d65 7461   prints the meta
+0001ab50: 6461 7461 2066 6f72 2074 6865 2073 6f6e  data for the son
+0001ab60: 6720 7769 7468 2049 4420 534f 4e47 5f49  g with ID SONG_I
+0001ab70: 442e 0a0a 2020 2020 4966 2050 4149 5253  D...    If PAIRS
+0001ab80: 2061 7265 2070 6173 7365 642c 2073 6574   are passed, set
+0001ab90: 7320 7468 6520 6d65 7461 6461 7461 2066  s the metadata f
+0001aba0: 6f72 2074 6865 2073 6f6e 6720 7769 7468  or the song with
+0001abb0: 2049 4420 534f 4e47 5f49 4420 746f 2074   ID SONG_ID to t
+0001abc0: 6865 0a20 2020 206b 6579 2d76 616c 7565  he.    key-value
+0001abd0: 2070 6169 7273 2069 6e20 5041 4952 532e   pairs in PAIRS.
+0001abe0: 2050 4149 5253 2073 686f 756c 6420 6265   PAIRS should be
+0001abf0: 2061 2073 7472 696e 6720 6f66 2074 6865   a string of the
+0001ac00: 2066 6f72 6d0a 2020 2020 276b 6579 313a   form.    'key1:
+0001ac10: 7661 6c75 6531 7c6b 6579 323a 7661 6c75  value1|key2:valu
+0001ac20: 6532 7c2e 2e2e 272e 0a0a 2020 2020 506f  e2|...'...    Po
+0001ac30: 7373 6962 6c65 2065 6469 7461 626c 6520  ssible editable 
+0001ac40: 6d65 7461 6461 7461 206b 6579 7320 6172  metadata keys ar
+0001ac50: 653a 2061 6c62 756d 2c20 616c 6275 6d61  e: album, albuma
+0001ac60: 7274 6973 742c 2061 7274 6973 742c 2061  rtist, artist, a
+0001ac70: 7274 776f 726b 2c0a 2020 2020 636f 6d6d  rtwork,.    comm
+0001ac80: 656e 742c 2063 6f6d 7069 6c61 7469 6f6e  ent, compilation
+0001ac90: 2c20 636f 6d70 6f73 6572 2c20 6469 7363  , composer, disc
+0001aca0: 6e75 6d62 6572 2c20 6765 6e72 652c 206c  number, genre, l
+0001acb0: 7972 6963 732c 2074 6f74 616c 6469 7363  yrics, totaldisc
+0001acc0: 732c 0a20 2020 2074 6f74 616c 7472 6163  s,.    totaltrac
+0001acd0: 6b73 2c20 7472 6163 6b6e 756d 6265 722c  ks, tracknumber,
+0001ace0: 2074 7261 636b 7469 746c 652c 2079 6561   tracktitle, yea
+0001acf0: 722c 2069 7372 630a 0a20 2020 204b 6579  r, isrc..    Key
+0001ad00: 7320 6172 6520 6e6f 7420 6361 7365 2073  s are not case s
+0001ad10: 656e 7369 7469 7665 2061 6e64 2063 616e  ensitive and can
+0001ad20: 2063 6f6e 7461 696e 2061 7262 6974 7261   contain arbitra
+0001ad30: 7279 2077 6869 7465 7370 6163 652c 2027  ry whitespace, '
+0001ad40: 2d27 2c20 616e 640a 2020 2020 275f 2720  -', and.    '_' 
+0001ad50: 6368 6172 6163 7465 7273 2e20 496e 206f  characters. In o
+0001ad60: 7468 6572 2077 6f72 6473 2c20 2741 6c62  ther words, 'Alb
+0001ad70: 756d 2041 7274 6973 7427 2c20 2761 6c62  um Artist', 'alb
+0001ad80: 756d 2d61 7274 6973 7427 2c20 616e 640a  um-artist', and.
+0001ad90: 2020 2020 2761 6c62 756d 5f61 7274 6973      'album_artis
+0001ada0: 7427 2061 7265 2061 6c6c 2073 796e 6f6e  t' are all synon
+0001adb0: 796d 7320 666f 7220 2761 6c62 756d 6172  yms for 'albumar
+0001adc0: 7469 7374 272e 2041 6c73 6f2c 2027 6469  tist'. Also, 'di
+0001add0: 736b 2720 6973 0a20 2020 2073 796e 6f6e  sk' is.    synon
+0001ade0: 796d 6f75 7320 7769 7468 2027 6469 7363  ymous with 'disc
+0001adf0: 272e 0a20 2020 2022 2222 0a0a 2020 2020  '..    """..    
+0001ae00: 7769 7468 206f 7065 6e28 534f 4e47 535f  with open(SONGS_
+0001ae10: 494e 464f 5f50 4154 482c 2022 7222 2c20  INFO_PATH, "r", 
+0001ae20: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+0001ae30: 2920 6173 2073 6f6e 6773 5f66 696c 653a  ) as songs_file:
+0001ae40: 0a20 2020 2020 2020 206c 696e 6573 203d  .        lines =
+0001ae50: 2073 6f6e 6773 5f66 696c 652e 7265 6164   songs_file.read
+0001ae60: 6c69 6e65 7328 290a 0a20 2020 2020 2020  lines()..       
+0001ae70: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+0001ae80: 6c65 6e28 6c69 6e65 7329 293a 0a20 2020  len(lines)):.   
+0001ae90: 2020 2020 2020 2020 2064 6574 6169 6c73           details
+0001aea0: 203d 206c 696e 6573 5b69 5d2e 7374 7269   = lines[i].stri
+0001aeb0: 7028 292e 7370 6c69 7428 227c 2229 0a20  p().split("|"). 
+0001aec0: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+0001aed0: 7428 6465 7461 696c 735b 305d 2920 3d3d  t(details[0]) ==
+0001aee0: 2073 6f6e 675f 6964 3a0a 2020 2020 2020   song_id:.      
+0001aef0: 2020 2020 2020 2020 2020 736f 6e67 5f70            song_p
+0001af00: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+0001af10: 696e 2853 4f4e 4753 5f44 4952 2c20 6465  in(SONGS_DIR, de
+0001af20: 7461 696c 735b 315d 290a 2020 2020 2020  tails[1]).      
+0001af30: 2020 2020 2020 2020 2020 736f 6e67 5f6e            song_n
+0001af40: 616d 6520 3d20 6465 7461 696c 735b 315d  ame = details[1]
+0001af50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001af60: 2062 7265 616b 0a20 2020 2020 2020 2065   break.        e
+0001af70: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0001af80: 2063 6c69 636b 2e73 6563 686f 280a 2020   click.secho(.  
+0001af90: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0001afa0: 4e6f 2073 6f6e 6720 7769 7468 2049 4420  No song with ID 
+0001afb0: 7b73 6f6e 675f 6964 7d20 666f 756e 642e  {song_id} found.
+0001afc0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0001afd0: 2020 2066 673d 2272 6564 222c 0a20 2020     fg="red",.   
+0001afe0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0001aff0: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+0001b000: 2020 2069 6620 7061 6972 733a 0a20 2020     if pairs:.   
+0001b010: 2020 2020 2070 6169 7273 203d 205b 7475       pairs = [tu
+0001b020: 706c 6528 7061 6972 2e73 7472 6970 2829  ple(pair.strip()
+0001b030: 2e73 706c 6974 2822 3a22 2929 2066 6f72  .split(":")) for
+0001b040: 2070 6169 7220 696e 2070 6169 7273 2e73   pair in pairs.s
+0001b050: 706c 6974 2822 7c22 295d 0a0a 2020 2020  plit("|")]..    
+0001b060: 2020 2020 736f 6e67 5f64 6174 6120 3d20      song_data = 
+0001b070: 6d75 7369 635f 7461 672e 6c6f 6164 5f66  music_tag.load_f
+0001b080: 696c 6528 736f 6e67 5f70 6174 6829 0a20  ile(song_path). 
+0001b090: 2020 2020 2020 2076 616c 6964 5f70 6169         valid_pai
+0001b0a0: 7273 203d 2070 6169 7273 5b3a 5d0a 2020  rs = pairs[:].  
+0001b0b0: 2020 2020 2020 666f 7220 6b65 792c 2076        for key, v
+0001b0c0: 616c 7565 2069 6e20 7061 6972 733a 0a20  alue in pairs:. 
+0001b0d0: 2020 2020 2020 2020 2020 2069 6620 6b65             if ke
+0001b0e0: 7920 6e6f 7420 696e 204d 4554 4144 4154  y not in METADAT
+0001b0f0: 415f 4b45 5953 206f 7220 6b65 792e 7374  A_KEYS or key.st
+0001b100: 6172 7473 7769 7468 2822 2322 293a 0a20  artswith("#"):. 
+0001b110: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001b120: 6c69 636b 2e73 6563 686f 280a 2020 2020  lick.secho(.    
+0001b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b140: 6622 277b 6b65 797d 2720 6973 206e 6f74  f"'{key}' is not
+0001b150: 2061 2076 616c 6964 2065 6469 7461 626c   a valid editabl
+0001b160: 6520 6d65 7461 6461 7461 206b 6579 2e22  e metadata key."
+0001b170: 2c20 6667 3d22 7265 6422 0a20 2020 2020  , fg="red".     
+0001b180: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0001b190: 2020 2020 2020 2020 2020 2020 2076 616c               val
+0001b1a0: 6964 5f70 6169 7273 2e72 656d 6f76 6528  id_pairs.remove(
+0001b1b0: 286b 6579 2c20 7661 6c75 6529 290a 2020  (key, value)).  
+0001b1c0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0001b1d0: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+0001b1e0: 2020 2073 6f6e 675f 6461 7461 5b6b 6579     song_data[key
+0001b1f0: 5d20 3d20 7661 6c75 650a 0a20 2020 2020  ] = value..     
+0001b200: 2020 2073 6f6e 675f 6461 7461 2e73 6176     song_data.sav
+0001b210: 6528 290a 0a20 2020 2020 2020 2063 6c69  e()..        cli
+0001b220: 636b 2e73 6563 686f 280a 2020 2020 2020  ck.secho(.      
+0001b230: 2020 2020 2020 6622 5365 7420 6d65 7461        f"Set meta
+0001b240: 6461 7461 2066 6f72 2027 7b73 6f6e 675f  data for '{song_
+0001b250: 6e61 6d65 7d27 2077 6974 6820 4944 207b  name}' with ID {
+0001b260: 736f 6e67 5f69 647d 2074 6f20 7b76 616c  song_id} to {val
+0001b270: 6964 5f70 6169 7273 7d2e 222c 0a20 2020  id_pairs}.",.   
+0001b280: 2020 2020 2020 2020 2066 673d 2267 7265           fg="gre
+0001b290: 656e 222c 0a20 2020 2020 2020 2029 0a20  en",.        ). 
+0001b2a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0001b2b0: 2073 6f6e 675f 6461 7461 203d 206d 7573   song_data = mus
+0001b2c0: 6963 5f74 6167 2e6c 6f61 645f 6669 6c65  ic_tag.load_file
+0001b2d0: 2873 6f6e 675f 7061 7468 290a 2020 2020  (song_path).    
+0001b2e0: 2020 2020 636c 6963 6b2e 6563 686f 2822      click.echo("
+0001b2f0: 4d65 7461 6461 7461 2066 6f72 2022 2c20  Metadata for ", 
+0001b300: 6e6c 3d46 616c 7365 290a 2020 2020 2020  nl=False).      
+0001b310: 2020 636c 6963 6b2e 7365 6368 6f28 736f    click.secho(so
+0001b320: 6e67 5f6e 616d 652c 2066 673d 2262 6c75  ng_name, fg="blu
+0001b330: 6522 2c20 626f 6c64 3d54 7275 652c 206e  e", bold=True, n
+0001b340: 6c3d 4661 6c73 6529 0a20 2020 2020 2020  l=False).       
+0001b350: 2063 6c69 636b 2e65 6368 6f28 6622 2077   click.echo(f" w
+0001b360: 6974 6820 4944 207b 736f 6e67 5f69 647d  ith ID {song_id}
+0001b370: 3a22 290a 0a20 2020 2020 2020 2066 6f72  :")..        for
+0001b380: 206b 6579 2069 6e20 4d45 5441 4441 5441   key in METADATA
+0001b390: 5f4b 4559 533a 0a20 2020 2020 2020 2020  _KEYS:.         
+0001b3a0: 2020 2074 7279 3a0a 2020 2020 2020 2020     try:.        
+0001b3b0: 2020 2020 2020 2020 636c 6963 6b2e 6563          click.ec
+0001b3c0: 686f 280a 2020 2020 2020 2020 2020 2020  ho(.            
+0001b3d0: 2020 2020 2020 2020 6622 5c74 7b6b 6579          f"\t{key
+0001b3e0: 2069 6620 6e6f 7420 6b65 792e 7374 6172   if not key.star
+0001b3f0: 7473 7769 7468 2827 2327 2920 656c 7365  tswith('#') else
+0001b400: 206b 6579 5b31 3a5d 7d3a 207b 736f 6e67   key[1:]}: {song
+0001b410: 5f64 6174 615b 6b65 795d 2e76 616c 7565  _data[key].value
+0001b420: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0001b430: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0001b440: 2065 7863 6570 743a 2020 2320 7079 6c69   except:  # pyli
+0001b450: 6e74 3a20 6469 7361 626c 653d 6261 7265  nt: disable=bare
+0001b460: 2d65 7863 6570 740a 2020 2020 2020 2020  -except.        
+0001b470: 2020 2020 2020 2020 7061 7373 0a                 pass.
```

### Comparing `maestro-music-1.0.1/maestro_music.egg-info/PKG-INFO` & `maestro-music-1.0.2/maestro_music.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: maestro-music
-Version: 1.0.1
+Version: 1.0.2
 Summary: A simple command line tool to play songs (or any audio files, really).
 Home-page: https://github.com/PrajwalVandana/maestro-cli
 Author: Prajwal Vandana
 License: MIT
 Keywords: music,sound,audio,music-player,cli,ogg,flac,mp3,wav,spotify,youtube,audio-visualization,audio-visualizer
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # maestro
 `maestro` is a command-line tool to play songs (or any audio, really) in the terminal.
 
 ## Features
 
 - cross-platform!
 - add songs directly from YouTube, YouTube Music, or Spotify!
 - audio visualization directly in the terminal!
 - Discord integration!
 - [clips!](#maestro-clip)
-- shuffle! (along with precise control over the behavior of shuffling when looping)
+- shuffle! (along with precise control over the behavior of shuffling when repeating)
 - filter by [tags](#usage)!
 
 ## Installation
 
 Make sure you have Python 3 and `pip` installed.
 
 First, run
@@ -91,54 +90,57 @@
 ```
 pip install PATH_TO_DOWNLOADED_WIN64_WHEEL
 ```
 and *now* installing `maestro` should work. Another option (especially if you're on a 32-bit Windows) is to just get Visual C++ Build Tools.
 
 #### Linux
 
-If you have issues, try:
+If you have issues (especially if you get `Illegal instruction (core dumped)` when running `maestro play`, even after installing succesfully), try:
  * upgrading pip: `pip install --upgrade pip`
  * uninstalling `just_playback`: `pip uninstall just_playback`
  * reinstalling `just_playback` with the `--no-binary` flag: `pip install just_playback --no-binary just_playback --force-reinstall --upgrade`
 
-Check this out: [https://github.com/cheofusi/just_playback/issues/21](https://github.com/cheofusi/just_playback/issues/21) ... and good luck 💀.
+Also check this out: [https://github.com/cheofusi/just_playback/issues/21](https://github.com/cheofusi/just_playback/issues/21) ... and good luck 💀.
+
+
+#### If all else fails ...
+You could uninstall and reinstall.
+```pip uninstall maestro-music```
+and also remove the `~/.maestro-files` folder.
+
+WARNING: this will delete all your songs! You should probably back up your `~/.maestro-files/songs/` folder first.
 
 ## Platforms
 
 Tested heavily on macOS Monterey, barely at all on Windows and Linux. `maestro` was coded to be cross-platform, but if there are any problems, please open an issue (or PR if you know how to fix it!).
 
 Supports `.mp3`, `.wav`, `.flac`, and `.ogg` (Ogg Vorbis).
 
 ## Usage
 
 Run `maestro -h` to get a list of commands. Run `maestro <some command> -h` to get comprehensive help for that command—the below is just an overview.
 
 `maestro` uses the concept of a positive integer **song ID** to uniquely refer to each song.
 
-Also, playlists don't exist—`maestro` uses **tags**. For example, let's say you want to be able to listen to all your Jon Bellion songs together. Instead of adding them all to a playlist, run `maestro -t jon-bellion <song IDs for each Jon Bellion song>`. Then `maestro play jon-bellion`. If song `s` has tag `t`, then you can think of song `s` as belonging to the playlist defined by tag `t`.
+Also, playlists don't exist—`maestro` uses **tags**. For example, let's say you want to be able to listen to all your Jon Bellion songs together. Instead of adding them all to a playlist, run `maestro tag <song IDs for each Jon Bellion song> -t jon-bellion `. Then `maestro play jon-bellion`. If song `s` has tag `t`, then you can think of song `s` as belonging to the playlist defined by tag `t`.
 
-`maestro` also tracks your listen time—total and by year. You can see this with `maestro list` and/or `maestro entry`. For example, to see your top 10 listened songs (by number of times listened; note that this is NOT the number of times the song was played but rather the total listen time for that song divided by the duration), run `maestro list -s times_listened -T 10 -y cur`—replace 'cur' with e.g. '2020' to get the listen times for 2020 instead.
+`maestro` also tracks your listen time—total and by year. You can see this with `maestro list` and/or `maestro entry`. For example, to see your top 10 listened songs (by average number of times listened; note that this is NOT the number of times the song was played but rather the total listen time for that song divided by the duration), run `maestro list -s times_listened -T 10 -y cur`—replace 'cur' with e.g. '2020' to get the listen times for 2020 instead.
 
 ### `maestro add`
 
 Add a song (can be a folder of songs too!) given a file path.
 
 Pass the `-Y` or `--youtube` flag to download from a YouTube or YouTube Music URL instead of a file path. This requires installing [FFmpeg](https://github.com/FFmpeg/FFmpeg). Passing a YouTube Music **song** URL (not "Video") is recommended, as passing "Video"s (i.e. just normal YouTube videos) can sometimes mess up the artist/album data.
 
 Pass the `-S` or `--spotify` flag to download from a Spotify URL instead of a file path. This also requires installing FFmpeg.
 
 Pass the `-P` or `--playlist` flag to download an entire YT playlist from a song URL with a playlist component, e.g. https://www.youtube.com/watch?v=V1Z586zoeeE&list=PLfSdF_HSSu55q-5p-maISZyr19erpZsTo. The `-p` flag is unnecessary if the URL points directly to a playlist, e.g. https://www.youtube.com/playlist?list=PLfSdF_HSSu55q-5p-maISZyr19erpZsTo.
 
 By default, `maestro add` copies the file to its internal database (`~/.maestro-files`), but you can pass the `-M` or `--move` flag to move the file instead.
 
-### `maestro cache`
-Calculate (or recalculate with the `-F/--force` flag) visualization frequency data (see [`maestro play`](#maestro-play)) for songs passed by ID (or all songs with the `-A/--all` flag.
-
-If you ever go into the song database (located at `~/.maestro-files`) and manually edit a song, e.g. trimming (not recommended but should be fine as long as you don't mess with the name of the file), you should run `maestro cache --recache <SONG_ID>` to readjust the visualization.
-
 ### `maestro clip`
 
 Ever been listening to music, and you're skipping every song because you keep getting bored of them? You like the songs, you're just not in the mood to listen to all of them entirely.
 
 Introducing clips, something I've always wished the big companies like Spotify, YT Music would do. Use `maestro clip ID START END` to define a clip for any song with a start and end timestamp (or use the clip editor for fine-grained control with `maestro clip ID`), then `maestro play -c` to play in "clip mode" (can also be toggled while playing a normal mode session with the `c` key)—this will play the clips for each song (or the entire song if there's no clip). Now you can listen to only the best parts of your music!
 
 ### `maestro entry`
@@ -149,24 +151,23 @@
 
 List songs (or tags) and details. Use `maestro list -h` to see full options (e.g. sort, list only songs with a certain tag, etc.).
 
 ### `maestro play`
 
 Play songs. Use `maestro play -h` to see full options. Has lots of features:
 - pass tag(s) as arguments to play songs with any of those tag(s) (or songs with all of those tag(s) if you pass the `-M` or `--match-all` flag)
-- shuffle playlist with the `-s` or `--shuffle option (shuffle once, shuffle every loop, or shuffle every loop except the first)
+- shuffle playlist with the `-s` or `--shuffle option (shuffle once, shuffle everytime the playlist repeats, or shuffle everytime the playlist repeats except the first)
 - play songs in reverse order with the `-R` or `--reverse` flag
 - loop playlist with the `-L` or `--loop` flag
 - show an audio visualization with the `-V` or `--visualize` flag
-  - you may notice some wait time for the visualization to properly load the first time a song is visualized (~7 seconds), but after that the visualization is cached and should load quickly
 - works with headphone buttons (and the Touch Bar and Siri!) on Mac using the Now Playing Center!
 - works with Discord status! (pass the `-D` or `--discord` flag)
 
 While playing:
-- like a song and want to play *that specific song* on loop? click `l` while playing to toggle loop mode (not the same as passing `-L` to `maestro play`!)
+- like a song and want to play it on loop? click `l` while playing to replay it once, and click it one more time to replay it infinitely (click it a third time to stop replaying it)
 - seek with left/right arrow keys
 - volume up/down with `[` and `]`
 - remove selected song (not necessarily the currently playing song) from current playlist with `backspace/delete`
 - scroll with mouse or up/down arrow keys to scroll the selected song
 - `c` to toggle clip mode
 - `v` to toggle visualization mode
 - `d` to toggle Discord status
@@ -211,9 +212,7 @@
 ### `maestro untag`
 
 Remove tags from a song, e.g. `maestro untag -t harry-styles 87` (removes the tag 'harry-styles' from the song with ID 87).
 
 ## Thanks
 
 Big thanks to the creators of [just_playback](https://github.com/cheofusi/just_playback), no doubt the best Python module for playing sound!
-
-
```

### Comparing `maestro-music-1.0.1/setup.py` & `maestro-music-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "pyobjc-framework-CoreMedia; sys_platform == 'darwin'",
     "pyobjc-framework-MediaPlayer; sys_platform == 'darwin'",
     "pyobjc-framework-Quartz; sys_platform == 'darwin'",
 ]
 
 setup(
     name="maestro-music",
-    version="1.0.1",
+    version="1.0.2",
     author="Prajwal Vandana",
     url="https://github.com/PrajwalVandana/maestro-cli",
     description="A simple command line tool to play songs (or any audio files, really).",
     long_description=open("readme.md", encoding="utf-8").read(),
     license="MIT",
     license_files=["LICENSE"],
     long_description_content_type="text/markdown",
```

