# Comparing `tmp/libretrofuzz-2.7.8.tar.gz` & `tmp/libretrofuzz-2.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libretrofuzz-2.7.8.tar", max compression
+gzip compressed data, was "libretrofuzz-2.7.9.tar", max compression
```

## Comparing `libretrofuzz-2.7.8.tar` & `libretrofuzz-2.7.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-01-11 07:54:49.517476 libretrofuzz-2.7.8/LICENSE
--rw-r--r--   0        0        0     7136 2023-01-11 07:54:49.517476 libretrofuzz-2.7.8/README.rst
--rw-r--r--   0        0        0       22 2023-01-11 07:54:49.517476 libretrofuzz-2.7.8/libretrofuzz/__init__.py
--rw-r--r--   0        0        0    47019 2023-01-11 07:54:49.521476 libretrofuzz-2.7.8/libretrofuzz/__main__.py
--rw-r--r--   0        0        0      952 2023-01-11 07:54:49.521476 libretrofuzz-2.7.8/pyproject.toml
--rw-r--r--   0        0        0     8296 2023-01-11 07:55:00.208726 libretrofuzz-2.7.8/setup.py
--rw-r--r--   0        0        0     8280 2023-01-11 07:55:00.210094 libretrofuzz-2.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-23 11:57:43.897853 libretrofuzz-2.7.9/LICENSE
+-rw-r--r--   0        0        0     7147 2023-05-23 11:57:43.897853 libretrofuzz-2.7.9/README.rst
+-rw-r--r--   0        0        0       22 2023-05-23 11:57:43.897853 libretrofuzz-2.7.9/libretrofuzz/__init__.py
+-rw-r--r--   0        0        0    47310 2023-05-23 11:57:43.897853 libretrofuzz-2.7.9/libretrofuzz/__main__.py
+-rw-r--r--   0        0        0      952 2023-05-23 11:57:43.897853 libretrofuzz-2.7.9/pyproject.toml
+-rw-r--r--   0        0        0     8310 2023-05-23 11:57:52.895553 libretrofuzz-2.7.9/setup.py
+-rw-r--r--   0        0        0     8291 2023-05-23 11:57:52.896421 libretrofuzz-2.7.9/PKG-INFO
```

### Comparing `libretrofuzz-2.7.8/LICENSE` & `libretrofuzz-2.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `libretrofuzz-2.7.8/README.rst` & `libretrofuzz-2.7.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -54,26 +54,27 @@
                         Directory name in the server to download thumbnails.
                         If not provided, asked from the user.
   --delay-after FLOAT   Seconds after download to skip replacing thumbnails.
                         No effect if called with --no-image.  [1<=x<=10]
   --delay FLOAT         Seconds to skip thumbnails download.  [1<=x<=10]
   --filter GLOB         Restricts downloads to game labels globs - not paths -
                         in the playlist, can be used multiple times and
-                        matches reset thumbnails, --filter '*' downloads all.
+                        matches reset thumbnails, --filter '\*' downloads all.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if
                         there is at least one in cache to avoid mixing
                         thumbnails from different server directories on
                         repeated calls. No effect if called with --filter.
-  --no-fail             Download any score. To restrict or retry use --filter.
   --no-subtitle         Remove subtitle after ' - ' or ': ' for mismatched
                         labels and server names. ':' can't occur in server
                         names, so if the server has 'Name\_ subtitle.png' and
                         not 'Name - subtitle.png' (uncommon), this option
-                        doesn't help. To restrict or retry use --filter.
+                        doesn't help.
+  --no-fail             Download any score.
+  --perfect             Download max score. No effect if called with --nofail.
   --no-meta             Ignores () delimited metadata and may cause false
                         positives. Forced with --before.
   --hack                Matches [] delimited metadata and may cause false
                         positives, Best used if the hack has thumbnails.
                         Ignored with --before.
   --before TEXT         Use only the part of the label before TEXT to match.
                         TEXT may not be inside of brackets of any kind, may
@@ -84,14 +85,15 @@
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or
                         customize the installation.
   --help                Show this message and exit.
 
 
 
+
 To install the program, type on the cmd line
 
 +----------------+---------------------------------------------------------------------------------------------+
 | Latest release | ``pip install --force-reinstall libretrofuzz``                                              |
 +----------------+---------------------------------------------------------------------------------------------+
 | Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |
 +----------------+---------------------------------------------------------------------------------------------+
```

### Comparing `libretrofuzz-2.7.8/libretrofuzz/__main__.py` & `libretrofuzz-2.7.9/libretrofuzz/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 Thumbs = collections.namedtuple('Thumbs', ['Named_Boxarts', 'Named_Titles', 'Named_Snaps'])
 
 ###########################################
 ########### SCRIPT SETTINGS ###############
 ###########################################
 
 
-CONFIDENCE = 100
+WIN_SCORE = 100
+MAX_SCORE = 200
 MAX_RETRIES = 3
 #00-1f are ascii control codes, rest is 'normal' illegal windows filename chars according to powershell + &
 forbidden = r'[\u0022\u003c\u003e\u007c\u0000\u0001\u0002\u0003\u0004\u0005\u0006\u0007\u0008' + \
             r'\u0009\u000a\u000b\u000c\u000d\u000e\u000f\u0010\u0011\u0012\u0013\u0014\u0015' + \
             r'\u0016\u0017\u0018\u0019\u001a\u001b\u001c\u001d\u001e\u001f\u003a\u002a\u003f\u005c\u002f\u0026]'
 #external terminal image viewer application
 viewer = None
@@ -192,27 +193,27 @@
 
 #-----------------------------------------------------------------------------------------------------------------------
 #The heart of the program, what orders titles to be 'more similar' or less to the local labels (after the normalization)
 #-----------------------------------------------------------------------------------------------------------------------
 class TitleScorer(object):
     def __init__(self):
         #rapidfuzz says to use range 0-100, but this doesn't (it's much easier that way), so it uses internal api to prevent a possible early exit at == 100
-        self._RF_ScorerPy = { 'get_scorer_flags': lambda **kwargs: {'optimal_score': 200, 'worst_score': 0, 'flags': (1 << 6)} }
+        self._RF_ScorerPy = { 'get_scorer_flags': lambda **kwargs: {'optimal_score': MAX_SCORE, 'worst_score': 0, 'flags': (1 << 6)} }
 
     def __call__(self, s1, s2, processor=None, score_cutoff=None):
         prefix = len(os.path.commonprefix([s1, s2]))
         if prefix <= 2 and len(s1) != len(s2):
             #ideally this branch wouldn't exist, but since many games do not have
             #images, they get caught up on a short title '100' from token_set_ratio
             #without the real title to win the similarity+prefix heuristic
             #this removes many false positives and causes few false negatives.
             return 0
         else:
             if s1 == s2:
-                return 200
+                return MAX_SCORE
             #score_cutoff needs to be 0 from a combination of 3 factors that create a bug:
             #1. the caller of this, extractOne passes the 'current best score' as score_cutoff
             #2. the token_set_ratio function returns 0 if the calculated score < score_cutoff
             #3. 'current best score' includes the prefix, which this call can't include in 2.
             similarity = fuzz.token_set_ratio(s1,s2,processor=None,score_cutoff=0)
             #Combine the scorer with a common prefix heuristic to give priority to longer similar
             #names, this helps prevents false positives for shorter strings which token set ratio
@@ -407,15 +408,15 @@
         fdir = fdir[2:]
         #imagine a retroarch.cfg file created in windows is read in posix
         if os.sep == '/':
             fdir = fdir.replace('\\', '/')
         return cfg.parent / fdir
     elif fdir == 'default':
         if default_value:
-            return Path(cfg.parent,default_value)
+            return cfg.parent / default_value
         else:
             return None
     return Path(fdir)
 
 def error(error: str):
     typer.echo(typer.style(error, fg=typer.colors.RED, bold=True))
 
@@ -465,16 +466,17 @@
         playlist: str = typer.Option(None, metavar='NAME', help='Playlist name with labels used for thumbnail fuzzy matching. If not provided, asked from the user.'),
         system: str = typer.Option(None, metavar='NAME', help='Directory name in the server to download thumbnails. If not provided, asked from the user.'),
         wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails. No effect if called with --no-image.'),
         wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download.'),
         filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and matches reset thumbnails, --filter \'*\' downloads all.'),
         noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
         nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No effect if called with --filter.'),
-        nofail: bool = typer.Option(False, '--no-fail', help='Download any score. To restrict or retry use --filter.'),
-        nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Remove subtitle after \' - \' or \': \' for mismatched labels and server names. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help. To restrict or retry use --filter.'),
+        nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Remove subtitle after \' - \' or \': \' for mismatched labels and server names. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
+        nofail: bool = typer.Option(False, '--no-fail', help='Download any score.'),
+        perfect: bool = typer.Option(False, '--perfect', help='Download max score. No effect if called with --nofail.'),
         nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
         hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
         before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces metadata to be ignored.'),
         verbose: bool = typer.Option(False, '--verbose', help='Shows the failures, score and normalized local and server names in output (score >= 100 is succesful).')
     ):
     if playlist and not playlist.lower().endswith('.lpl'):
         playlist = playlist + '.lpl'
@@ -504,31 +506,32 @@
         try:
             async with lock_keys(), AsyncClient() as client:
                 #temporary dir for downloads (required to prevent clobbering of files in case of no internet and filters being used)
                 #parent directory of this temp dir is the same as the retroarch thumbnail dir to make moving the file just renaming it, not copy it
                 with TemporaryDirectory(prefix='libretrofuzz', dir=thumbnails_dir) as tmpdir:
                     typer.echo(typer.style(f'{playlist} -> {system}', bold=True))
                     names = readPlaylistAndPrepareDirectories(Path(playlist_dir, playlist), tmpdir, thumbnails_dir)
-                    await downloader(names,system,wait_before,wait_after,filters,noimage,nomerge,nofail,nometa,hack,nosubtitle,verbose,before,tmpdir,thumbnails_dir,client)
+                    await downloader(names,system,wait_before,wait_after,filters,noimage,nomerge,nofail,nometa,perfect,hack,nosubtitle,verbose,before,tmpdir,thumbnails_dir,client)
         except StopPlaylist as e:
             error(f'Cloudflare is down for {system}')
             raise typer.Exit(code=1)
         except StopProgram as e:
             error(f'Cancelled by user, exiting')
             raise typer.Exit()
     asyncio.run(runit(), debug=False)
 
 def mainfuzzall(cfg: Path = typer.Argument(CONFIG, help='Path to the retroarch cfg file. If not default, asked from the user.'),
         wait_after: Optional[float] = typer.Option(None, '--delay-after', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds after download to skip replacing thumbnails. No effect if called with --no-image.'),
         wait_before: Optional[float] = typer.Option(None, '--delay', min=1, max=10, clamp=True, metavar='FLOAT', help='Seconds to skip thumbnails download.'),
         filters: Optional[List[str]] = typer.Option(None, '--filter', metavar='GLOB', help='Restricts downloads to game labels globs - not paths - in the playlist, can be used multiple times and matches reset thumbnails, --filter \'*\' downloads all.'),
         noimage: bool = typer.Option(False, '--no-image', help='Don\'t show images even with chafa installed.'),
         nomerge: bool = typer.Option(False, '--no-merge', help='Disables missing thumbnails download for a label if there is at least one in cache to avoid mixing thumbnails from different server directories on repeated calls. No effect if called with --filter.'),
-        nofail: bool = typer.Option(False, '--no-fail', help='Download any score. To restrict or retry use --filter.'),
-        nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Remove subtitle after \' - \' or \': \' for mismatched labels and server names. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help. To restrict or retry use --filter.'),
+        nosubtitle: bool = typer.Option(False, '--no-subtitle', help='Remove subtitle after \' - \' or \': \' for mismatched labels and server names. \':\' can\'t occur in server names, so if the server has \'Name_ subtitle.png\' and not \'Name - subtitle.png\' (uncommon), this option doesn\'t help.'),
+        nofail: bool = typer.Option(False, '--no-fail', help='Download any score.'),
+        perfect: bool = typer.Option(False, '--perfect', help='Download max score. No effect if called with --nofail.'),
         nometa: bool = typer.Option(False, '--no-meta', help='Ignores () delimited metadata and may cause false positives. Forced with --before.'),
         hack: bool = typer.Option(False, '--hack', help='Matches [] delimited metadata and may cause false positives, Best used if the hack has thumbnails. Ignored with --before.'),
         before: Optional[str] = typer.Option(None, help='Use only the part of the label before TEXT to match. TEXT may not be inside of brackets of any kind, may cause false positives but some labels do not have traditional separators. Forces metadata to be ignored.'),
         verbose: bool = typer.Option(False, '--verbose', help='Shows the failures, score and normalized local and server names in output (score >= 100 is succesful).')
     ):
     playlist_dir, thumbnails_dir, PLAYLISTS, SYSTEMS = test_common_errors(cfg, None, None)
     
@@ -543,15 +546,15 @@
                 with TemporaryDirectory(prefix='libretrofuzz', dir=thumbnails_dir) as tmpdir:
                     for playlist, system in notInSystems:
                         typer.echo(typer.style(f'Custom playlist skipped: ', fg=typer.colors.RED, bold=True)+typer.style(f'{system}.lpl', bold=True))
                     for playlist, system in inSystems:
                         typer.echo(typer.style(f'{system}.lpl -> {system}', bold=True))
                         names = readPlaylistAndPrepareDirectories(playlist, tmpdir, thumbnails_dir)
                         try:
-                            await downloader(names,system,wait_before,wait_after,filters,noimage,nomerge,nofail,nometa,hack,nosubtitle,verbose,before,tmpdir,thumbnails_dir,client)
+                            await downloader(names,system,wait_before,wait_after,filters,noimage,nomerge,nofail,nometa,perfect,hack,nosubtitle,verbose,before,tmpdir,thumbnails_dir,client)
                         except StopPlaylist as e:
                             error(f'Cloudflare is down for {system}')
         except StopProgram as e:
             error(f'Cancelled by user, exiting')
             raise typer.Exit()
     asyncio.run(runit(), debug=False)
 
@@ -587,15 +590,15 @@
     return args
 
 async def downloader(names: [(str,str)],
                system: str,
                wait_before: Optional[float],
                wait_after: Optional[float],
                filters: Optional[List[str]],
-               noimage : bool, nomerge: bool, nofail: bool, nometa: bool, hack: bool, nosubtitle: bool, verbose: bool,
+               noimage : bool, nomerge: bool, nofail: bool, nometa: bool, perfect: bool, hack: bool, nosubtitle: bool, verbose: bool,
                before: Optional[str],
                tmpdir: Path,
                thumbnails_dir: Path,
                client: AsyncClient
                ):
     #not a error to pass a empty playlist
     if len(names) == 0:
@@ -603,14 +606,17 @@
     
     thumbs = Thumbs._make( await downloadgamenames(client, system) )
     
     #before implies that the names of the playlists may be cut, so the hack and meta matching must be disabled
     if before:
         hack = False
         nometa = True
+    #no-fail requires perfect to be disabled
+    if nofail:
+        perfect = False
     
     #preprocess data so it's not redone every loop iteration.
     title_scorer = TitleScorer()
     #normalize with or without subtitles, besides the remote_names this is used on the iterated local names later
     norm = nosubtitle_normalizer if nosubtitle else normalizer
     #we choose the highest similarity of all 3 directories, since no mixed matches are allowed
     remote_names = set()
@@ -676,15 +682,15 @@
         success_format = f'{prefix_format}{typer.style("Success",   fg=typer.colors.GREEN, bold=True)}: {name_format}'
         failure_format = f'{prefix_format}{typer.style("Failure",     fg=typer.colors.RED, bold=True)}: {name_format}'
         missing_format = f'{prefix_format}{typer.style("Missing",     fg=typer.colors.RED, bold=True)}:'
         cancel_format  = f'{prefix_format}{typer.style("Skipped",        fg=(135,135,135), bold=True)}: {name_format}'
         nomerge_format = f'{zeroth_format}{typer.style("Nomerge",        fg=(128,128,128), bold=True)}: {name_format}'
         getting_format = f'{prefix_format}{typer.style("Getting",    fg=typer.colors.BLUE, bold=True)}: {name_format}'
         waiting_format = f'{prefix_format}{typer.style("Waiting",  fg=typer.colors.YELLOW, bold=True)}: {name_format}' '{bar:-9b} {remaining_s:2.1f}s: {bar:10u}'
-        if thumbnail and ( i_max >= CONFIDENCE or nofail ):
+        if thumbnail and ((perfect and i_max == MAX_SCORE) or (not perfect and i_max >= WIN_SCORE) or nofail):
             #these parent directories were created when reading the playlist, more efficient than doing it a playlist game loop
             real_thumb_dir = Path(thumbnails_dir,destination)
             down_thumb_dir = Path(tmpdir,destination)
             allow = True
             if not filters and nomerge:
                 #to implement no-merge you have to disable downloads on 'at least one' thumbnail (including user added ones)
                 missing_thumbs = 0
```

### Comparing `libretrofuzz-2.7.8/pyproject.toml` & `libretrofuzz-2.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libretrofuzz"
-version = "2.7.8"
+version = "2.7.9"
 description = "Fuzzy Retroarch thumbnail downloader"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/i30817/libretrofuzz"
 
 [tool.poetry.dependencies]
```

### Comparing `libretrofuzz-2.7.8/setup.py` & `libretrofuzz-2.7.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 
 entry_points = \
 {'console_scripts': ['libretro-fuzz = libretrofuzz.__main__:fuzzsingle',
                      'libretro-fuzzall = libretrofuzz.__main__:fuzzall']}
 
 setup_kwargs = {
     'name': 'libretrofuzz',
-    'version': '2.7.8',
+    'version': '2.7.9',
     'description': 'Fuzzy Retroarch thumbnail downloader',
-    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get non-standard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels, but you can just run them to get the most restrictive default.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will dowload for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with grey border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n ``libretro-fuzz --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels don't have subtitles and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads and the system name ``Commodore - Amiga`` to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then mostly be from the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass the similarity test. Common false positives from this are sequels or prequels, or different releases, most often regions/languages.\n\nExample:\n  ``libretro-fuzz --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, the Ishar series in the WHDLoad playlist.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy\n                        matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails.\n                        If not provided, asked from the user.\n  --delay-after FLOAT   Seconds after download to skip replacing thumbnails.\n                        No effect if called with --no-image.  [1<=x<=10]\n  --delay FLOAT         Seconds to skip thumbnails download.  [1<=x<=10]\n  --filter GLOB         Restricts downloads to game labels globs - not paths -\n                        in the playlist, can be used multiple times and\n                        matches reset thumbnails, --filter '*' downloads all.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if\n                        there is at least one in cache to avoid mixing\n                        thumbnails from different server directories on\n                        repeated calls. No effect if called with --filter.\n  --no-fail             Download any score. To restrict or retry use --filter.\n  --no-subtitle         Remove subtitle after ' - ' or ': ' for mismatched\n                        labels and server names. ':' can't occur in server\n                        names, so if the server has 'Name\\_ subtitle.png' and\n                        not 'Name - subtitle.png' (uncommon), this option\n                        doesn't help. To restrict or retry use --filter.\n  --no-meta             Ignores () delimited metadata and may cause false\n                        positives. Forced with --before.\n  --hack                Matches [] delimited metadata and may cause false\n                        positives, Best used if the hack has thumbnails.\n                        Ignored with --before.\n  --before TEXT         Use only the part of the label before TEXT to match.\n                        TEXT may not be inside of brackets of any kind, may\n                        cause false positives but some labels do not have\n                        traditional separators. Forces metadata to be ignored.\n  --verbose             Shows the failures, score and normalized local and\n                        server names in output (score >= 100 is succesful).\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
+    'long_description': "**Fuzzy Retroarch thumbnail downloader**\n========================================\n\nIn Retroarch, when you use the manual scanner to get non-standard games or hacks in playlists, thumbnails often fail to download.\n\nThese programs, for each game label on a playlist, download the most similar named image to display in retroarch.\n\nThere are several options to fit unusual labels, but you can just run them to get the most restrictive default.\n\nIf you use ``libretro-fuzz``, it will download for a single playlist by asking for the playlist and system if they're not provided.\nIf you use ``libretro-fuzzall``, it will dowload for all playlists with standard libretro names, and will skip custom playlists.\n\nBesides those differences, if no retroarch.cfg is provided, both programs try to use the default retroarch.cfg.\n\nIf `chafa <https://github.com/hpjansson/chafa>`_ is installed, the program will display new thumbnails of a game, with grey border for images already in use and with green border for new images. Chafa works better with a recent release and on a `sixel <https://en.wikipedia.org/wiki/Sixel>`_ or `kitty <https://sw.kovidgoyal.net/kitty/graphics-protocol/>`_ compatible shell.\n\nExample:\n ``libretro-fuzz --no-subtitle --before '_'``\n \n The Retroplay WHDLoad set has labels like ``MonkeyIsland2_v1.3_0020`` after a manual scan. These labels don't have subtitles and all the metadata is not separated from the name by brackets. Select the playlist that contains those whdloads and the system name ``Commodore - Amiga`` to download from the libretro amiga thumbnails.\n\nNote that the system name you download from doesn't have to be the same as the playlist name.\n\nIf the thumbnail server contains games from multiple releases for the system (like ``ScummVM``), be careful using extra options since it is easy to end up with 'slightly wrong' covers.\n\nExample:\n ``libretro-fuzz --no-meta --no-merge``\n \n After downloading ``ScummVM`` thumbnails (and not before, to minimize false positives), we'd like to try to pickup a few covers from ``DOS`` thumbnails and skip download if there a risk of mixing thumbnails from ``DOS`` and ``ScummVM`` for a single game.\n Choose the ScummVM playlist and DOS system name, and covers would be downloaded with risk of false positives: CD vs floppy covers, USA vs Japan covers, or another platform vs DOS.\n\nBecause of this increased risk of false positives with options, the default is to count everything except hack metadata as part of the match, and the default pre-selected system name to be the same as the playlist name, which is safest.\n\nFalse positives will then mostly be from the thumbnail server not having a single thumbnail of the game, and the program selecting the best match it can which is still good enough to pass the similarity test. Common false positives from this are sequels or prequels, or different releases, most often regions/languages.\n\nExample:\n  ``libretro-fuzz --no-subtitle --before '_' --filter '[Ii]shar*'``\n  \n  The best way to solve these issues is to upload the right cover to the respective libretro-thumbnail subproject with the correct name of the game variant. Then you can redownload just the updated thumbnails with a label, in this example, the Ishar series in the WHDLoad playlist.\n\nlibretro-fuzzall/libretro-fuzz [OPTIONS] [CFG]\n  :CFG:                 Path to the retroarch cfg file. If not default, asked from the user.\n  \n                        Linux default:   ``~/.config/retroarch/retroarch.cfg``\n  \n                        Windows default: ``%APPDATA%/RetroArch/retroarch.cfg``\n  \n                        MacOS default:   ``~/Library/Application Support/RetroArch/config/retroarch.cfg``\n  \n  --playlist <NAME libretro-fuzz only>\n                        Playlist name with labels used for thumbnail fuzzy\n                        matching. If not provided, asked from the user.\n  --system <NAME libretro-fuzz only>\n                        Directory name in the server to download thumbnails.\n                        If not provided, asked from the user.\n  --delay-after FLOAT   Seconds after download to skip replacing thumbnails.\n                        No effect if called with --no-image.  [1<=x<=10]\n  --delay FLOAT         Seconds to skip thumbnails download.  [1<=x<=10]\n  --filter GLOB         Restricts downloads to game labels globs - not paths -\n                        in the playlist, can be used multiple times and\n                        matches reset thumbnails, --filter '\\*' downloads all.\n  --no-image            Don't show images even with chafa installed.\n  --no-merge            Disables missing thumbnails download for a label if\n                        there is at least one in cache to avoid mixing\n                        thumbnails from different server directories on\n                        repeated calls. No effect if called with --filter.\n  --no-subtitle         Remove subtitle after ' - ' or ': ' for mismatched\n                        labels and server names. ':' can't occur in server\n                        names, so if the server has 'Name\\_ subtitle.png' and\n                        not 'Name - subtitle.png' (uncommon), this option\n                        doesn't help.\n  --no-fail             Download any score.\n  --perfect             Download max score. No effect if called with --nofail.\n  --no-meta             Ignores () delimited metadata and may cause false\n                        positives. Forced with --before.\n  --hack                Matches [] delimited metadata and may cause false\n                        positives, Best used if the hack has thumbnails.\n                        Ignored with --before.\n  --before TEXT         Use only the part of the label before TEXT to match.\n                        TEXT may not be inside of brackets of any kind, may\n                        cause false positives but some labels do not have\n                        traditional separators. Forces metadata to be ignored.\n  --verbose             Shows the failures, score and normalized local and\n                        server names in output (score >= 100 is succesful).\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\n\n\nTo install the program, type on the cmd line\n\n+----------------+---------------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall libretrofuzz``                                              |\n+----------------+---------------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |\n+----------------+---------------------------------------------------------------------------------------------+\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python, to be able to install and execute the script from any path of the cmd line.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/libretrofuzz',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `libretrofuzz-2.7.8/PKG-INFO` & `libretrofuzz-2.7.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libretrofuzz
-Version: 2.7.8
+Version: 2.7.9
 Summary: Fuzzy Retroarch thumbnail downloader
 Home-page: https://github.com/i30817/libretrofuzz
 License: MIT
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -82,26 +82,27 @@
                         Directory name in the server to download thumbnails.
                         If not provided, asked from the user.
   --delay-after FLOAT   Seconds after download to skip replacing thumbnails.
                         No effect if called with --no-image.  [1<=x<=10]
   --delay FLOAT         Seconds to skip thumbnails download.  [1<=x<=10]
   --filter GLOB         Restricts downloads to game labels globs - not paths -
                         in the playlist, can be used multiple times and
-                        matches reset thumbnails, --filter '*' downloads all.
+                        matches reset thumbnails, --filter '\*' downloads all.
   --no-image            Don't show images even with chafa installed.
   --no-merge            Disables missing thumbnails download for a label if
                         there is at least one in cache to avoid mixing
                         thumbnails from different server directories on
                         repeated calls. No effect if called with --filter.
-  --no-fail             Download any score. To restrict or retry use --filter.
   --no-subtitle         Remove subtitle after ' - ' or ': ' for mismatched
                         labels and server names. ':' can't occur in server
                         names, so if the server has 'Name\_ subtitle.png' and
                         not 'Name - subtitle.png' (uncommon), this option
-                        doesn't help. To restrict or retry use --filter.
+                        doesn't help.
+  --no-fail             Download any score.
+  --perfect             Download max score. No effect if called with --nofail.
   --no-meta             Ignores () delimited metadata and may cause false
                         positives. Forced with --before.
   --hack                Matches [] delimited metadata and may cause false
                         positives, Best used if the hack has thumbnails.
                         Ignored with --before.
   --before TEXT         Use only the part of the label before TEXT to match.
                         TEXT may not be inside of brackets of any kind, may
@@ -112,14 +113,15 @@
   --install-completion  Install completion for the current shell.
   --show-completion     Show completion for the current shell, to copy it or
                         customize the installation.
   --help                Show this message and exit.
 
 
 
+
 To install the program, type on the cmd line
 
 +----------------+---------------------------------------------------------------------------------------------+
 | Latest release | ``pip install --force-reinstall libretrofuzz``                                              |
 +----------------+---------------------------------------------------------------------------------------------+
 | Current code   | ``pip install --force-reinstall https://github.com/i30817/libretrofuzz/archive/master.zip`` |
 +----------------+---------------------------------------------------------------------------------------------+
```

