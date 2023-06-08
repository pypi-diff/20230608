# Comparing `tmp/libretrofuzz-2.9.6.tar.gz` & `tmp/libretrofuzz-2.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.9.6.tar", max compression
+gzip compressed data, was "libretrofuzz-2.9.7.tar", max compression
```

## Comparing `libretrofuzz-2.9.6.tar` & `libretrofuzz-2.9.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-07 00:05:16.591403 libretrofuzz-2.9.6/LICENSE
--rw-r--r--   0        0        0     7570 2023-06-07 00:05:16.591403 libretrofuzz-2.9.6/README.rst
--rw-r--r--   0        0        0       22 2023-06-07 00:05:16.591403 libretrofuzz-2.9.6/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    48253 2023-06-07 00:05:16.591403 libretrofuzz-2.9.6/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      992 2023-06-07 00:05:16.591403 libretrofuzz-2.9.6/pyproject.toml
--rw-r--r--   0        0        0     8775 2023-06-07 00:05:25.661933 libretrofuzz-2.9.6/setup.py
--rw-r--r--   0        0        0     8799 2023-06-07 00:05:25.662751 libretrofuzz-2.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-07 03:35:33.448218 libretrofuzz-2.9.7/LICENSE
+-rw-r--r--   0        0        0     7567 2023-06-07 03:35:33.448218 libretrofuzz-2.9.7/README.rst
+-rw-r--r--   0        0        0       22 2023-06-07 03:35:33.448218 libretrofuzz-2.9.7/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    48116 2023-06-07 03:35:33.448218 libretrofuzz-2.9.7/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      992 2023-06-07 03:35:33.448218 libretrofuzz-2.9.7/pyproject.toml
+-rw-r--r--   0        0        0     8772 2023-06-07 03:35:47.719017 libretrofuzz-2.9.7/setup.py
+-rw-r--r--   0        0        0     8796 2023-06-07 03:35:47.719920 libretrofuzz-2.9.7/PKG-INFO
```

### Comparing `libretrofuzz-2.9.6/LICENSE` & `libretrofuzz-2.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.9.6/README.rst` & `libretrofuzz-2.9.7/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
-  --verbose N           | Show mininame, len N list (maxscore, server mininame).
+  --verbose N           | Show length N list (maxscore, mininame cover link).
                         | [x>=1]
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
```

### Comparing `libretrofuzz-2.9.6/libretrofuzz/__main__.py` & `libretrofuzz-2.9.7/libretrofuzz/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,30 +25,32 @@
 import collections
 import shutil
 import unicodedata
 import asyncio
 import subprocess
 import configparser
 #external libraries
-import typer
 from PIL import Image, ImageOps
 from rapidfuzz import process, fuzz
 from bs4 import BeautifulSoup
 from questionary import Style, select
 from httpx import RequestError, HTTPStatusError, Client, AsyncClient
 from tqdm import trange, tqdm
+from typer.colors import YELLOW, RED, BLUE, GREEN, MAGENTA
+from typer import style, echo, run, Exit, Argument, Option
 
 #makes a class with these fields, which are the subdir names on the server system dir of the types of thumbnails
 Thumbs = collections.namedtuple('Thumbs', ['Named_Boxarts', 'Named_Titles', 'Named_Snaps'])
 
 ###########################################
 ########### SCRIPT SETTINGS ###############
 ###########################################
 
 ADDRESS='https://thumbnails.libretro.com'
+SEARCHADDRESS='https://www.mobygames.com/search/?q='
 MAX_SCORE = 200
 MAX_RETRIES = 3
 MAX_WAIT_SECS = 30
 #00-1f are ascii control codes, rest is 'normal' illegal windows filename chars according to powershell + &
 forbidden = regex.compile( \
             r'[\u0022\u003c\u003e\u007c\u0000\u0001\u0002\u0003\u0004\u0005\u0006\u0007\u0008' + \
             r'\u0009\u000a\u000b\u000c\u000d\u000e\u000f\u0010\u0011\u0012\u0013\u0014\u0015' + \
@@ -60,15 +62,15 @@
 if sys.platform == 'win32': #this is for 64 bits too
   #this order is to make 'portable' installs have priority in windows, a concept that doesn't exist in linux or macosx
   #these are the default 32 and 64 bits installer paths, since there is no way to know what the user choses, check the defaults only.
   CONFIG = Path(r'C:/RetroArch-Win64/retroarch.cfg')
   if not CONFIG.exists():
     CONFIG = Path(r'C:/RetroArch/retroarch.cfg')
     if not CONFIG.exists():
-      typer.echo('Portable install default location config not found, trying with APPDATA location')
+      echo('Portable install default location config not found, trying with APPDATA location')
       var = os.getenv('APPDATA')
       if var:
         CONFIG = Path(var, 'RetroArch', 'retroarch.cfg')
 elif sys.platform == 'darwin':
   CONFIG = Path(Path.home(), 'Library', 'Application Support', 'RetroArch', 'config', 'retroarch.cfg')
 else: #all the rest based on linux. If they arent based on linux, they'll try the else and fail harmlessly later
   var = os.getenv('XDG_CONFIG_HOME')
@@ -166,31 +168,29 @@
         skip = True
   try:
     with input.raw_mode():
       with input.attach(keys_ready):
         #ignore keys in buffer before we are ready
         input.read_keys()
         input.flush_keys()
-        typer.echo(typer.style(f'Press escape to quit, enter to continue and most other non-meta keys to skip downloads', bold=True))
+        echo(style(f'Press escape to quit, enter to continue and most other non-meta keys to skip downloads', bold=True))
         yield
   finally:
     #in windows 7 and python 3.8 for some reason prompt_toolkit
     #tries to send a 'handle ready' not 'remove' event after detaching (the with above)
     #not sure if it happens in python later than 3.8. This throws a 'RuntimeError: Event Loop is closed'
     #the sleep avoids it
     if sys.platform == "win32":
       await asyncio.sleep(0.1)
 
 #----------------non contextual str manipulation------------------------
 def link(uri, label=None, parameters=''):
   '''
   Found in https://gist.github.com/egmontkob/eb114294efbcd5adb1944c9f3cb5feda
   '''
-  if type(uri) is str: #just hover text and show same hyperlinks if possible
-    uri = quote(uri)
   if label is None:
     label = uri
   # OSC 8 ; params ; URI ST <name> OSC 8 ;; ST
   escape_mask = '\033]8;{};{}\033\\{}\033]8;;\033\\'
   return escape_mask.format(parameters, uri, label)
 
 ppatterns = { '()': regex.compile(r'\([^)(]*\)'), '[]': regex.compile(r'\[[^][]*\]') }
@@ -460,89 +460,89 @@
     if default_value:
       return cfg.parent / default_value
     else:
       return None
   return Path(fdir)
 
 def error(error: str):
-  typer.echo(typer.style(error, fg=typer.colors.RED, bold=True))
+  echo(style(error, fg=RED, bold=True))
 
 def test_common_errors(cfg: Path, playlist: str, system: str, address: str):
   '''returns a tuple with (playlist_dir: Path, thumbnail_dir: Path, PLAYLISTS: [Path], SYSTEMS: [str]) '''
   #stop showing the variables - a library installed this behind my back
   try:
     from rich.traceback import install
     install(show_locals=False)
   except ImportError:
     pass
   global ADDRESS
   ADDRESS = address.rstrip('/')
   global viewer
   viewer = which('chafa')
   if not viewer:
-    typer.echo(f'Shell image viewer chafa was not found')
+    echo(f'Shell image viewer chafa was not found')
   if not cfg or not cfg.is_file():
     error(f'Invalid Retroarch cfg file: {cfg}')
-    raise typer.Exit(code=1)
+    raise Exit(code=1)
   thumbnails_directory = getPath(cfg, 'thumbnails_directory', 'thumbnails')
   if not thumbnails_directory or not thumbnails_directory.is_dir() or not os.access(thumbnails_directory, os.W_OK):
     error(f'Invalid retroarch.cfg line: thumbnails_directory="{thumbnails_directory}"')
-    raise typer.Exit(code=1)
+    raise Exit(code=1)
   playlist_dir = getPath(cfg, 'playlist_directory', 'playlists')
   if not playlist_dir or not playlist_dir.is_dir() or not os.access(playlist_dir, os.R_OK):
     error(f'Invalid retroarch.cfg line: playlist_directory="{playlist_dir}"')
-    raise typer.Exit(code=1)
+    raise Exit(code=1)
   PLAYLISTS = [ pl for pl in playlist_dir.glob('./*.lpl') if pl.is_file() and os.access(pl, os.R_OK) ]
   if not PLAYLISTS:
     error(f'Invalid playlist files in playlist directory: {playlist_dir}')
-    raise typer.Exit(code=1)
+    raise Exit(code=1)
   if playlist and Path(playlist_dir, playlist) not in PLAYLISTS:
     error(f'Invalid user provided playlist: {playlist}')
-    raise typer.Exit(code=1)
+    raise Exit(code=1)
   #windows can only print images and urls in windows 10 up (requires a better console)
   #since python 3.8 is the very minimum of this application, it can only be used on windows 7 and up
   #ie: we only have to disallow 7, 8
   basic_verbose = False
   import platform
   if sys.platform == "win32" and platform.release() in ('7','8','8.1'):
-    typer.echo(f'Disabling rich verbose and image output because your windows does not support it')
+    echo(f'Disabling rich verbose and image output because your windows does not support it')
     basic_verbose = True
   try:
     with Client() as client:
       page = client.get(ADDRESS, timeout=15)
       soup = BeautifulSoup(page.text, 'html.parser')
     SYSTEMS = [ unquote(node.get('href')[:-1]) for node in soup.find_all('a') if node.get('href').endswith('/') and not node.get('href').endswith('../') ]
   except (RequestError,HTTPStatusError) as err:
     error(f'Could not get the remote thumbnail system names, exiting: {err}')
-    raise typer.Exit(code=1)
+    raise Exit(code=1)
   if system and system not in SYSTEMS:
     error(f'The user provided system name {system} does not match any remote thumbnail system names')
-    raise typer.Exit(code=1)
+    raise Exit(code=1)
   return (basic_verbose, playlist_dir, thumbnails_directory, sorted(PLAYLISTS), sorted(SYSTEMS))
 
 #####################
 # Main programs code
 #####################
 
-def mainfuzzsingle(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
-  playlist: str = typer.Option(None, metavar='NAME', help='Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.'),
-  system: str = typer.Option(None, metavar='NAME', help='Directory name in the server to download thumbnails. If not provided, asked from the user.'),
-  wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
-  wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
-  filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
-  score: int = typer.Option(MAX_SCORE, '--min', min=0, max=MAX_SCORE, metavar='SCORE', help=f'0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.'),
-  nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
-  noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
-  nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
-  nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
-  nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
-  hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
-  before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
-  address: Optional[str] = typer.Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
-  verbose: Optional[int] = typer.Option(None, '--verbose', min=1, metavar='N', help=f'Show mininame, len N list (maxscore, server mininame).')
+def mainfuzzsingle(cfg: Path = Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
+  playlist: str = Option(None, metavar='NAME', help='Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.'),
+  system: str = Option(None, metavar='NAME', help='Directory name in the server to download thumbnails. If not provided, asked from the user.'),
+  wait_after: Optional[float] = Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
+  wait_before: Optional[float] = Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
+  filters: Optional[List[str]] = Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
+  score: int = Option(MAX_SCORE, '--min', min=0, max=MAX_SCORE, metavar='SCORE', help=f'0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.'),
+  nofail: bool = Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
+  noimage: bool = Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
+  nomerge: bool = Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
+  nosubtitle: bool = Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
+  nometa: bool = Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
+  hack: bool = Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
+  before: Optional[str] = Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
+  address: Optional[str] = Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
+  verbose: Optional[int] = Option(None, '--verbose', min=1, metavar='N', help=f'Show length N list (maxscore, mininame cover link).')
   ):
   if playlist and not playlist.lower().endswith('.lpl'):
     playlist = playlist + '.lpl'
 
   basic_verbose,playlist_dir,thumbnails_dir,PLAYLISTS,SYSTEMS = test_common_errors(cfg,playlist,system,address)
   if basic_verbose : noimage = True
 
@@ -551,83 +551,83 @@
   ])
 
   #ask user for these 2 arguments if they're still not set
   if not playlist:
     display_playlists = list(map(os.path.basename, PLAYLISTS))
     playlist = select('Which playlist do you want to download thumbnails for?', display_playlists, style=custom_style, qmark='').ask()
     if not playlist:
-      raise typer.Exit()
+      raise Exit()
 
   if not system:
     #start with the playlist system selected, if any
     playlist_sys = playlist[:-4]
     question = 'Which directory should be used to download thumbnails?'
     system = select(question, SYSTEMS, style=custom_style, qmark='', default=playlist_sys if playlist_sys in SYSTEMS else None).ask()
     if not system:
-      raise typer.Exit()
+      raise Exit()
 
   async def runit():
     try:
       async with lock_keys(), AsyncClient() as client:
         #temporary dir for downloads (required to prevent clobbering of files in case of no internet and filters being used)
         #parent directory of this temp dir is the same as the RA thumbnail dir to make mv the file just renaming it, not cp it
         with TemporaryDirectory(prefix='libretrofuzz', dir=thumbnails_dir) as tmpdir:
-          typer.echo(typer.style(f'{playlist} -> {system}', bold=True))
+          echo(style(f'{playlist} -> {system}', bold=True))
           names = readPlaylistAndPrepareDirectories(Path(playlist_dir, playlist), tmpdir, thumbnails_dir)
           await downloader(names,system,wait_before,wait_after,filters,score,noimage,nomerge,nofail,nometa, \
                            hack,nosubtitle,verbose,basic_verbose,before,tmpdir,thumbnails_dir,client)
     except StopPlaylist as e:
       error(f'Cloudflare is down for {system}')
-      raise typer.Exit(code=1)
+      raise Exit(code=1)
     except StopProgram as e:
       error(f'Cancelled by user, exiting')
-      raise typer.Exit()
+      raise Exit()
   asyncio.run(runit(), debug=False)
 
-def mainfuzzall(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
-  wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
-  wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
-  filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
-  score: int = typer.Option(MAX_SCORE, '--min', min=0, max=MAX_SCORE, metavar='SCORE', help=f'0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.'),
-  nofail: bool = typer.Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
-  noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
-  nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
-  nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
-  nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
-  hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
-  before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
-  address: Optional[str] = typer.Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
-  verbose: Optional[int] = typer.Option(None, '--verbose', min=1, metavar='N', help=f'Show mininame, len N list (maxscore, server mininame).')
+def mainfuzzall(cfg: Path = Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
+  wait_after: Optional[float] = Option(None, '--delay-after', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails, enter continues. No-op with --no-image.'),
+  wait_before: Optional[float] = Option(None, '--delay', min=1, max=MAX_WAIT_SECS, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download, enter continues.'),
+  filters: Optional[List[str]] = Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, --filter \'*\' redownloads all.'),
+  score: int = Option(MAX_SCORE, '--min', min=0, max=MAX_SCORE, metavar='SCORE', help=f'0=any, 100=fuzzy match, {MAX_SCORE}=equal mininames,default. No-op with --no-fail.'),
+  nofail: bool = Option(False, '--no-fail', help='Download any score. Equivalent to --score 0.'),
+  noimage: bool = Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
+  nomerge: bool = Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with --filter.'),
+  nosubtitle: bool = Option(False, '--no-subtitle', help='Ignores text after last \' - \' or \': \'. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
+  nometa: bool = Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
+  hack: bool = Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
+  before: Optional[str] = Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.'),
+  address: Optional[str] = Option(ADDRESS, metavar='URL', help='URL with libretro-thumbnails server. For local files, git clone/unzip packs, run \'python3 -m http.server\' in parent dir, and use --address \'http://localhost:8000\'.'),
+  verbose: Optional[int] = Option(None, '--verbose', min=1, metavar='N', help=f'Show length N list (maxscore, mininame cover link).')
   ):
   basic_verbose,playlist_dir,thumbnails_dir,PLAYLISTS,SYSTEMS = test_common_errors(cfg,None,None,address)
   if basic_verbose : noimage = True
 
   notInSystems = [ (playlist, os.path.basename(playlist)[:-4]) for playlist in PLAYLISTS if os.path.basename(playlist)[:-4] not in SYSTEMS]
   for playlist, system in notInSystems:
     PLAYLISTS.remove(playlist)
   inSystems = [ (playlist, os.path.basename(playlist)[:-4]) for playlist in PLAYLISTS ]
 
   async def runit():
     try:
       async with lock_keys(), AsyncClient() as client:
         with TemporaryDirectory(prefix='libretrofuzz', dir=thumbnails_dir) as tmpdir:
           for playlist, system in notInSystems:
-            typer.echo(typer.style(f'Custom playlist skipped: ', fg=typer.colors.RED, bold=True) + \
-                       typer.style(f'{system}.lpl', bold=True))
+            echo(style(f'Custom playlist skipped: ', fg=RED, bold=True) + \
+                       style(f'{system}.lpl', bold=True))
           for playlist, system in inSystems:
-            typer.echo(typer.style(f'{system}.lpl -> {system}', bold=True))
+            echo(style(f'{system}.lpl -> {system}', bold=True))
             names = readPlaylistAndPrepareDirectories(playlist, tmpdir, thumbnails_dir)
             try:
               await downloader(names,system,wait_before,wait_after,filters,score,noimage,nomerge,nofail,nometa, \
                                hack,nosubtitle,verbose,basic_verbose,before,tmpdir,thumbnails_dir,client)
             except StopPlaylist as e:
               error(f'Cloudflare is down for {system}')
     except StopProgram as e:
       error(f'Cancelled by user, exiting')
-      raise typer.Exit()
+      raise Exit()
   asyncio.run(runit(), debug=False)
 
 async def downloadgamenames(client, system):
   """returns [ dict(Game_Name, Game_Url), dict(Game_Name, Game_Url), dict(Game_Name, Game_Url) ]
       for each of the server directories '/Named_Boxarts/', '/Named_Titles/', '/Named_Snaps/'
       (potentially some of these dicts may be empty if the server doesn't have the directory)
   """
@@ -650,15 +650,15 @@
         #will go to except if there is a another error
         r.raise_for_status()
         soup = BeautifulSoup(response, 'html.parser')
         l1 = { unquote(Path(node.get('href')).name[:-4]) : lr_thumb+node.get('href') for node in soup.find_all('a') if node.get('href').endswith('.png')}
       args.append(l1)
   except (RequestError,HTTPStatusError) as err:
     error(f'Could not get the remote thumbnail game names, exiting: {err}')
-    raise typer.Exit(code=1)
+    raise Exit(code=1)
   return args
 
 async def downloader(names: [(str,str)],
                system: str,
                wait_before: Optional[float],
                wait_after: Optional[float],
                filters: Optional[List[str]],
@@ -735,40 +735,49 @@
     result = process.extract(nameaux, remote_names, scorer=title_scorer,processor=None,limit=verbose or 1,score_cutoff=None)
     #build the verbose format and decompose the first result, with a optimization if verbose is not on
     thumb_normal, thumb_score, thumb_name = (None, 0, None)
     verbose_format = []
     if verbose:
       for r in reversed(result):
         thumb_normal, thumb_score, thumb_name = r
-        color = typer.colors.RED if thumb_score < score else typer.colors.GREEN
-        verbose_score = typer.style(f'{int(thumb_score)}', fg=f'{color}', bold=True)
-        verbose_name  = thumb_normal if basic_verbose else link(thumb_name, thumb_normal)
+        color = RED if thumb_score < score else GREEN
+        verbose_score = style(f'{int(thumb_score)}', fg=f'{color}', bold=True)
+        #if the boxart exists link to it, otherwise link to a mobygames search
+        payload = None
+        if thumb_name in thumbs.Named_Boxarts:
+          payload = link(thumbs.Named_Boxarts[thumb_name],thumb_normal)
+          payload = style(payload, fg=MAGENTA)
+        else:
+          payload = link(SEARCHADDRESS+quote(thumb_name),thumb_normal)
+          payload = style(payload, fg=BLUE)
+        verbose_name  = thumb_normal if basic_verbose else payload
         verbose_format.insert(0, f"{verbose_score} {verbose_name}")
       verbose_format = ', '.join(verbose_format)
     elif len(result) > 0:
       thumb_normal, thumb_score, thumb_name = result[0]
     #hack, if result 1 and 2 have equal scores use the second thumbnail as a alternative if missing a thumb type
     #this is done because it's relatively common for the server to have a case mistake on thumb types
     thumb_name2 = None
     if len(result) >= 2:
       if result[0][1] == result[1][1]:
         thumb_name2 = result[1][2]
     #formating legos
-    name_format    = nameaux if basic_verbose else link(name,nameaux)
-    dull_format    = f'{name} -> {thumb_name}'
-    line_format    = name_format + ' -> ' + verbose_format if verbose else dull_format
-    success_format = f'{typer.style("Success",   fg=typer.colors.GREEN, bold=True)}: {line_format}'
-    failure_format = f'{typer.style("Failure",     fg=typer.colors.RED, bold=True)}: {line_format}'
-    missing_format = f'{typer.style("Missing",     fg=typer.colors.RED, bold=True)}: {line_format}'
-    skipped_format = f'{typer.style("Skipped",        fg=(135,135,135), bold=True)}: {line_format}'
-    nomerge_format = f'{typer.style("Nomerge",        fg=(128,128,128), bold=True)}: {line_format}'
-    getting_format = f'{typer.style("Getting",    fg=typer.colors.BLUE, bold=True)}: {dull_format}' \
-                     + typer.style(' {percentage:3.0f}%', fg=typer.colors.BLUE, bold=True)
-    waiting_format = f'{typer.style("Waiting",  fg=typer.colors.YELLOW, bold=True)}: {dull_format}' \
-                     + typer.style(' {remaining_s:2.1f}s', fg=typer.colors.RED, bold=True)                         
+    name_format    = style(name, bold=True)
+    dull_format    = name_format + ': ' + thumb_name
+    line_format    = name_format + ': ' + verbose_format if verbose else dull_format
+    success_format = f'{style("Success",   fg=GREEN, bold=True)}: {line_format}'
+    failure_format = f'{style("Failure",     fg=RED, bold=True)}: {line_format}'
+    missing_format = f'{style("Missing",     fg=RED, bold=True)}: {line_format}'
+    skipped_format = f'{style("Skipped",        fg=(135,135,135), bold=True)}: {line_format}'
+    nomerge_format = f'{style("Nomerge",        fg=(128,128,128), bold=True)}: {line_format}'
+    #these can't support links because of tqdm, show the normal names and replace them after
+    getting_format = f'{style("Getting",    fg=BLUE, bold=True)}: {dull_format}' \
+                     + style(' {percentage:3.0f}%', fg=BLUE, bold=True)
+    waiting_format = f'{style("Waiting",  fg=YELLOW, bold=True)}: {dull_format}' \
+                     + style(' {remaining_s:2.1f}s', fg=RED, bold=True)
     if thumb_name and thumb_score >= score:
       allow = True
       #these parent directories were created when reading the playlist, more efficient than doing it a playlist game loop
       real_thumb_dir = Path(thumbnails_dir,destination)
       down_thumb_dir = Path(tmpdir,destination)
       if not filters and nomerge:
         #to implement no-merge you have to disable downloads on 'at least one' thumbnail (including user added ones)
@@ -779,15 +788,15 @@
           if not real.exists():
             missing_thumbs += 1
             if thumb_name in getattr(thumbs, dirname) or thumb_name2 in getattr(thumbs, dirname):
               missing_server_thumbs += 1
         allow = missing_thumbs == 3
         #despite the above, print only for when it would download if it was allowed, otherwise it is confusing
         if not allow and missing_server_thumbs > 0:
-          typer.echo(nomerge_format)
+          echo(nomerge_format)
       if allow:
         first_wait      = wait_before is not None
         downloaded_once = False
         downloaded_dict = dict() #dictionary of thumbnailtype -> (old Path, new Path), paths may not exist
         try:
           for dirname in Thumbs._fields:
             real = Path(real_thumb_dir, dirname, name + '.png')
@@ -805,27 +814,27 @@
               #nothing to download but we want to remove images that may be there in the case of --filter.
               real.unlink(missing_ok=True)
           if not noimage and viewer and downloaded_once:
             displayImages(downloaded_dict)
             if wait_after is not None:
               await printwait(wait_after, waiting_format)
         except StopProgram as e:
-          typer.echo(skipped_format)
+          echo(skipped_format)
           raise e
         except StopDownload as e:
           downloaded_once = False
-          typer.echo(skipped_format)
+          echo(skipped_format)
         if downloaded_once:
           for (old, new) in downloaded_dict.values():
             if new.exists():
               shutil.move(new, old)
-          typer.echo(success_format)
+          echo(success_format)
     else:
       if verbose:
-        typer.echo(failure_format)
+        echo(failure_format)
       if filters:
         #nothing to download but we want to remove images that may be there in the case of --filter.
         for dirname in Thumbs._fields:
           Path(thumbnails_dir,destination, dirname, name + '.png').unlink(missing_ok=True)
 
 async def printwait(wait : Optional[float], waiting_format: str):
   count = int(wait/0.1)
@@ -840,34 +849,34 @@
   '''
   while True:
     try:
       async with client.stream('GET', url, timeout=15) as r:
         if r.status_code == 521: #cloudflare exploded, skip the whole playlist
           raise StopPlaylist()
         if r.status_code == 404: #broken image or symlink link, skip just this thumb
-          typer.echo(missing_format + ' ' + url)
+          echo(missing_format + ' ' + url)
           return False
         r.raise_for_status()     #error before reading the header goes into retrying
         length = int(r.headers['Content-Length'])
         if length < 100:         #obviously corrupt 'thumbnail', skip this thumb
-          typer.echo(missing_format + ' ' + url)
+          echo(missing_format + ' ' + url)
           return False
         with open(destination, 'w+b') as f:
           if first_wait:
             await printwait(wait_before, waiting_format)
           with tqdm.wrapattr(f, 'write', total=length, dynamic_ncols=True, bar_format=getting_format, leave=False) as w:
             async for chunk in r.aiter_raw(4096):
               with handleContinueDownload():
                 checkDownload()
               w.write(chunk)
       return True
     except (RequestError,HTTPStatusError) as e:
       if max_retries <= 0:
         error(f'Download max retries exceeded, exiting')
-        raise typer.Exit(code=1)
+        raise Exit(code=1)
       max_retries -= 1
 
 def displayImages(downloaded: dict):
   '''dict has all the tuple (old, new) with the key of the thumbnail type str (the files may not exist)
      this method will display the new images with a green border and the old with a gray border and missing as... missing
   '''
   imgs = dict()
@@ -935,15 +944,15 @@
   combined.paste(snap, box=(box.size[0], title.size[1]))
   #save it, print TODO if a _good_ python sixtel library happens, replace this
   with io.BytesIO() as f:
     combined.save(f, format='png')
     subprocess.run([viewer, '-'], input=f.getbuffer())
 
 def fuzzsingle():
-  typer.run(mainfuzzsingle)
+  run(mainfuzzsingle)
 
 def fuzzall():
-  typer.run(mainfuzzall)
+  run(mainfuzzall)
 
 if __name__ == "__main__":
   error('Please run libretro-fuzz or libretro-fuzzall instead of running the script directly')
-  raise typer.Exit(code=1)
+  raise Exit(code=1)
```

### Comparing `libretrofuzz-2.9.6/pyproject.toml` & `libretrofuzz-2.9.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.9.6"
+version = "2.9.7"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.9.6/setup.py` & `libretrofuzz-2.9.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.9.6',
+    'version': '2.9.7',
     'description': 'Fuzzy Retroarch thumbnail downloader',
-    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show mininame, len N list (maxscore, server mininame).\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
+    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get nonstandard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels and increase fuzziness, but you can just run them to get the most restrictive default (with the least fuzz).\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will download for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with gray border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n | ``libretro-fuzz --system 'Commodore - Amiga' --before '_'``\n | then\n | ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels *often* don't have subtitles (but not always) and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, only select the names that match exactly (after 'safe' heuristics like removing spaces) and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then be from using ``--score`` (allows inexact matches) or/and one of the commands that do not count metadata (``--before``, ``--no-meta`` and ``--no-subtitle``). A common scenario is the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass, like a sequel, prequel, or different release, most often regions/languages. It's not recommended to use ``--score`` less than 100 without ``--filter`` to a specific game.\n\nExample:\n  ``libretro-fuzz --system 'Commodore - Amiga' --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, because of ``--filter``, the Ishar series in the WHDLoad playlist would redownload.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails. If not provided, asked from the user.\n  --delay-after FLOAT   | Seconds after download to skip replacing thumbnails, enter continues. No-op with ``--no-image``.\n                        | [1<=x<=30]\n  --delay FLOAT         | Seconds to skip thumbnails download, enter continues.\n                        | [1<=x<=30]\n  --filter GLOB         Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and resets thumbnails, ``--filter '*'`` redownloads all.\n  --min SCORE           | 0=any, 100=fuzzy match, 200=equal mininames,default. No-op with ``--no-fail``.\n                        | [default: 200; 0<=x<=200]\n  --no-fail             Download any score. Equivalent to ``--score 0``.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.\n  --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.\n  --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.\n  --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.\n  --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.\n  --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.\n                        | [default: https://thumbnails.libretro.com]\n  --verbose N           | Show length N list (maxscore, mininame cover link).\n                        | [x>=1]\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libretrofuzz-2.9.6/PKG-INFO` & `libretrofuzz-2.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.9.6
+Version: 2.9.7
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -95,15 +95,15 @@
   --no-merge            Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No-op with ``--filter``.
   --no-subtitle         Ignores text after last ``' - '`` or ``': '``. ``':'`` can't occur in server names, so if the server has ``'Name_subtitle.png'`` and not ``'Name - subtitle.png'`` (uncommon), this option doesn't help.
   --no-meta             Ignores () delimited metadata and may cause false positives. Forced with ``--before``.
   --hack                Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with ``--before``.
   --before TEXT         Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces ignoring metadata.
   --address URL         | URL with libretro-thumbnails server. For local files, git clone/unzip packs, run ``'python3 -m http.server'`` in parent dir, and use ``--address 'http://localhost:8000'``.
                         | [default: https://thumbnails.libretro.com]
-  --verbose N           | Show mininame, len N list (maxscore, server mininame).
+  --verbose N           | Show length N list (maxscore, mininame cover link).
                         | [x>=1]
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or customize the installation.
   --help                Show this message and exit.
```

