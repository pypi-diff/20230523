# Comparing `tmp/transcribe_allign_textgrid-0.1.3.tar.gz` & `tmp/transcribe_allign_textgrid-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transcribe_allign_textgrid-0.1.3.tar", last modified: Sat Apr  8 19:03:43 2023, max compression
+gzip compressed data, was "transcribe_allign_textgrid-0.1.4.tar", last modified: Tue May 23 10:41:56 2023, max compression
```

## Comparing `transcribe_allign_textgrid-0.1.3.tar` & `transcribe_allign_textgrid-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-08 19:03:43.458562 transcribe_allign_textgrid-0.1.3/
--rw-r--r--   0 jjw       (1000) jjw       (1000)    34523 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/LICENCE
--rw-r--r--   0 jjw       (1000) jjw       (1000)     6587 2023-04-08 19:03:43.458562 transcribe_allign_textgrid-0.1.3/PKG-INFO
--rw-r--r--   0 jjw       (1000) jjw       (1000)     5814 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/README.md
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1047 2023-04-08 19:02:07.000000 transcribe_allign_textgrid-0.1.3/pyproject.toml
--rw-r--r--   0 jjw       (1000) jjw       (1000)       29 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/requirements.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)       38 2023-04-08 19:03:43.458562 transcribe_allign_textgrid-0.1.3/setup.cfg
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-08 19:03:43.456562 transcribe_allign_textgrid-0.1.3/src/
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-08 19:03:43.457562 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1001 2023-04-08 19:02:26.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/__init__.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)       79 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/__main__.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     3315 2023-04-08 18:57:03.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/adapter.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     3846 2023-04-08 18:58:22.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/cli.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)     1994 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/whisper_schema.py
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-08 19:03:43.458562 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/
--rw-r--r--   0 jjw       (1000) jjw       (1000)     6587 2023-04-08 19:03:43.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/PKG-INFO
--rw-r--r--   0 jjw       (1000) jjw       (1000)      576 2023-04-08 19:03:43.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/SOURCES.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)        1 2023-04-08 19:03:43.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/dependency_links.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)       29 2023-04-08 19:03:43.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/requires.txt
--rw-r--r--   0 jjw       (1000) jjw       (1000)       27 2023-04-08 19:03:43.000000 transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/top_level.txt
-drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-04-08 19:03:43.458562 transcribe_allign_textgrid-0.1.3/tests/
--rw-r--r--   0 jjw       (1000) jjw       (1000)      795 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/tests/test_adapter.py
--rw-r--r--   0 jjw       (1000) jjw       (1000)      225 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.3/tests/test_schema.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-23 10:41:56.707075 transcribe_allign_textgrid-0.1.4/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)    34523 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.4/LICENCE
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     6839 2023-05-23 10:41:56.707075 transcribe_allign_textgrid-0.1.4/PKG-INFO
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     6066 2023-05-23 10:35:51.000000 transcribe_allign_textgrid-0.1.4/README.md
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1048 2023-05-23 10:39:19.000000 transcribe_allign_textgrid-0.1.4/pyproject.toml
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       29 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.4/requirements.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       38 2023-05-23 10:41:56.707075 transcribe_allign_textgrid-0.1.4/setup.cfg
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-23 10:41:56.704075 transcribe_allign_textgrid-0.1.4/src/
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-23 10:41:56.706075 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1001 2023-05-23 10:39:44.000000 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid/__init__.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       79 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid/__main__.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     3315 2023-04-08 18:57:03.000000 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid/adapter.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     4582 2023-05-23 10:34:23.000000 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid/cli.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     1994 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid/whisper_schema.py
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-23 10:41:56.706075 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid.egg-info/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)     6839 2023-05-23 10:41:56.000000 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid.egg-info/PKG-INFO
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      576 2023-05-23 10:41:56.000000 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)        1 2023-05-23 10:41:56.000000 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       29 2023-05-23 10:41:56.000000 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid.egg-info/requires.txt
+-rw-r--r--   0 jjw       (1000) jjw       (1000)       27 2023-05-23 10:41:56.000000 transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid.egg-info/top_level.txt
+drwxr-xr-x   0 jjw       (1000) jjw       (1000)        0 2023-05-23 10:41:56.706075 transcribe_allign_textgrid-0.1.4/tests/
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      795 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.4/tests/test_adapter.py
+-rw-r--r--   0 jjw       (1000) jjw       (1000)      225 2023-03-27 20:58:30.000000 transcribe_allign_textgrid-0.1.4/tests/test_schema.py
```

### Comparing `transcribe_allign_textgrid-0.1.3/LICENCE` & `transcribe_allign_textgrid-0.1.4/LICENCE`

 * *Files identical despite different names*

### Comparing `transcribe_allign_textgrid-0.1.3/PKG-INFO` & `transcribe_allign_textgrid-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe_allign_textgrid
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create for-alligned transcription TextGrids from Audio
 Author-email: JJWRoeloffs <jelleroeloffs@gmail.com>
 Project-URL: Homepage, https://github.com/JJWRoeloffs/transcribe_allign_textgrid
 Project-URL: Bug Tracker, https://github.com/JJWRoeloffs/transcribe_allign_textgrid/issues
 Keywords: praat,whisper,force-allign,TextGrid
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -23,15 +23,15 @@
 
 ## Requirements
 * `Python3.9` Other python versions might work, but dependency `onnxruntime` is quite iffy.
     * Use the executable `python3.9` on Unix, available in most package managers, or `py -3.9` on Windows.
     * The command line executable of python3.9 will be referred to as `[python-executable]` for the rest of the instructions
     * Install pip on old python versions with `[python-executable] -m ensurepip --default-pip`
 * `ffmpeg` Usually preinstalled on Linux. For windows see instructions for installation on the [whisper repository](https://github.com/openai/whisper)
-* `git` Usually preinstalled on Linux. For windows, visit [the git site](https://git-scm.com/download/win). 
+* `git` Usually preinstalled on Linux. For windows, visit [the git site](https://git-scm.com/download/win).
     * Needed for installation of whisper-timestamped, as it is not available on pypi
     * Note that it needs to be available from the command line; git-bash might not work.
 
 ## Light installation
 If you don't have a Nvidea GPU, or don't want to use it, you cannot use the CUDA platform on which Whisper is run. In this case, you should install a light version of torch **before** installing whisper-timestamped (and thus this application). Do this with:
 ```bash
 [python-executable] -m pip install \
@@ -51,17 +51,19 @@
 
 # Running from the command line
 Once the application is installed, you can run it with:
 ```bash
 [python-executable] -m transcribe_allign_textgrid [path]
 ```
 
-here `path` is the path to the audio files. 
+here `path` is the path to the audio files.
 * If a directory path is passed, all audio files in the directory will be transcribed, and force-alligned transcription textgrids of the same name will be generated in this directory.
-* If a file path is passed, a force-alligned transcription textgrid will be generated into the same directory as the original file.
+* If a file path is passed, a force-alligned transcription textgrid will be generated into the same directory with the same name as the original file.
+* If a glob is passed, the glob will be resoled and all matches will be processed as if the files were passed individually
+* By default, if a non-audio file is passed, an error is raised. To skip those instead, pass the `--skip` flag.
 
 ## Selecting a different model
 By default, this will run on the smallest, that is, least accurate and fastest, model, `tiny`. To run with another model, pass it as an argument:
 ```bash
 [python-executable] -m transcribe_allign_textgrid [path] --model [model]
 ```
```

### Comparing `transcribe_allign_textgrid-0.1.3/README.md` & `transcribe_allign_textgrid-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## Requirements
 * `Python3.9` Other python versions might work, but dependency `onnxruntime` is quite iffy.
     * Use the executable `python3.9` on Unix, available in most package managers, or `py -3.9` on Windows.
     * The command line executable of python3.9 will be referred to as `[python-executable]` for the rest of the instructions
     * Install pip on old python versions with `[python-executable] -m ensurepip --default-pip`
 * `ffmpeg` Usually preinstalled on Linux. For windows see instructions for installation on the [whisper repository](https://github.com/openai/whisper)
-* `git` Usually preinstalled on Linux. For windows, visit [the git site](https://git-scm.com/download/win). 
+* `git` Usually preinstalled on Linux. For windows, visit [the git site](https://git-scm.com/download/win).
     * Needed for installation of whisper-timestamped, as it is not available on pypi
     * Note that it needs to be available from the command line; git-bash might not work.
 
 ## Light installation
 If you don't have a Nvidea GPU, or don't want to use it, you cannot use the CUDA platform on which Whisper is run. In this case, you should install a light version of torch **before** installing whisper-timestamped (and thus this application). Do this with:
 ```bash
 [python-executable] -m pip install \
@@ -34,17 +34,19 @@
 
 # Running from the command line
 Once the application is installed, you can run it with:
 ```bash
 [python-executable] -m transcribe_allign_textgrid [path]
 ```
 
-here `path` is the path to the audio files. 
+here `path` is the path to the audio files.
 * If a directory path is passed, all audio files in the directory will be transcribed, and force-alligned transcription textgrids of the same name will be generated in this directory.
-* If a file path is passed, a force-alligned transcription textgrid will be generated into the same directory as the original file.
+* If a file path is passed, a force-alligned transcription textgrid will be generated into the same directory with the same name as the original file.
+* If a glob is passed, the glob will be resoled and all matches will be processed as if the files were passed individually
+* By default, if a non-audio file is passed, an error is raised. To skip those instead, pass the `--skip` flag.
 
 ## Selecting a different model
 By default, this will run on the smallest, that is, least accurate and fastest, model, `tiny`. To run with another model, pass it as an argument:
 ```bash
 [python-executable] -m transcribe_allign_textgrid [path] --model [model]
 ```
```

### Comparing `transcribe_allign_textgrid-0.1.3/pyproject.toml` & `transcribe_allign_textgrid-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "transcribe_allign_textgrid"
-version = "0.1.3"
-authors = [
-  { name="JJWRoeloffs", email="jelleroeloffs@gmail.com" },
-]
+version = "0.1.4"
+authors = [{ name = "JJWRoeloffs", email = "jelleroeloffs@gmail.com" }]
 description = "Create for-alligned transcription TextGrids from Audio"
 keywords = ["praat", "whisper", "force-allign", "TextGrid"]
 readme = "README.md"
 requires-python = ">=3.7, <3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
@@ -24,12 +22,12 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools.dynamic]
-dependencies = {file = ["requirements.txt"]}
+dependencies = { file = ["requirements.txt"] }
 
 [project.urls]
 "Homepage" = "https://github.com/JJWRoeloffs/transcribe_allign_textgrid"
 "Bug Tracker" = "https://github.com/JJWRoeloffs/transcribe_allign_textgrid/issues"
```

### Comparing `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/__init__.py` & `transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 You should have received a copy of the GNU Affero General Public License
 along with this program.  If not see LICENSE for more details.
 """
 
 __title__ = "transcribe_allign_textgrid"
 __author__ = "JJWRoeloffs"
 __license__ = "AGPL-3.0"
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 
 from transcribe_allign_textgrid.adapter import (
     whisper_to_textgrid as whisper_to_textgrid,
 )
```

### Comparing `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/adapter.py` & `transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid/adapter.py`

 * *Files identical despite different names*

### Comparing `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/cli.py` & `transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -44,20 +44,33 @@
 
 
 @dataclass
 class Args:
     paths: List[Path]
     model: str
     language: Optional[str]
+    continue_on_err: bool
 
 
-def get_files(path: Path) -> List[Path]:
+def parse_path(path: Path) -> List[Path]:
     return [path] if path.is_file() else [x for x in path.iterdir() if x.is_file()]
 
 
+def parse_glob(pathstr: str) -> List[Path]:
+    return list(Path().glob(pathstr))
+
+
+def parse_pathstr(ctx: argparse.ArgumentParser, pathstr: str) -> List[Path]:
+    pathspec = Path(pathstr)
+    paths = parse_path(pathspec) if pathspec.exists() else parse_glob(pathstr)
+    if not paths:
+        ctx.error(f"Could not resolve to filepaths: {pathspec}")
+    return [path.resolve() for path in paths]
+
+
 def parse_args(args: List[str]) -> Args:
     parser = argparse.ArgumentParser(
         prog="transcribe_allign_textgrid",
         description="""
             A small wrapper cli around whisper-timestamped.
             Create force-alligned transcription TextGrids from raw audio!
             """,
@@ -85,38 +98,53 @@
     parser.add_argument(
         "--language",
         choices=LANGUAGES.values(),
         help="Language size to use for the transcription, Default automatic",
         nargs="?",
         required=False,
     )
-    arguments = parser.parse_args(args)
-    paths = [Path(x).resolve() for x in arguments.paths]
+    parser.add_argument(
+        "--skip",
+        action="store_true",
+        help="If passed, any non-audio files passed are skipped.",
+        default=False,
+        required=False,
+    )
 
-    for path in paths:
-        if not path.exists():
-            parser.error(f"Passed path does not exist: {path}")
+    arguments = parser.parse_args(args)
 
-    paths = [file for path in paths for file in get_files(path)]
+    paths = [file for path in arguments.paths for file in parse_pathstr(parser, path)]
 
-    return Args(paths=paths, model=arguments.model, language=arguments.language)
+    return Args(
+        paths=paths,
+        model=arguments.model,
+        language=arguments.language,
+        continue_on_err=arguments.skip,
+    )
 
 
 def run(args: Args) -> None:
     if not check_cli_dependencies():
         raise ImportError
 
     print("Loading Model...")
     import whisper_timestamped
 
     model = whisper_timestamped.load_model(args.model)
 
     for path in args.paths:
         print(f"Processing: {str(path.name)}")
-        audio = whisper_timestamped.load_audio(str(path))
+        try:
+            audio = whisper_timestamped.load_audio(str(path))
+        except RuntimeError:
+            if args.continue_on_err:
+                print(f"Could not process {path}, as audio, skipping")
+                continue
+            raise
+
         result = whisper_timestamped.transcribe(model, audio, language=args.language)
         textgrid = whisper_to_textgrid(result)
 
         new_name = str(path.with_suffix(".TextGrid"))
         print(f"Saving: {new_name}")
         textgrid.save(new_name, format="long_textgrid", includeBlankSpaces=True)
```

### Comparing `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid/whisper_schema.py` & `transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid/whisper_schema.py`

 * *Files identical despite different names*

### Comparing `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/PKG-INFO` & `transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transcribe-allign-textgrid
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create for-alligned transcription TextGrids from Audio
 Author-email: JJWRoeloffs <jelleroeloffs@gmail.com>
 Project-URL: Homepage, https://github.com/JJWRoeloffs/transcribe_allign_textgrid
 Project-URL: Bug Tracker, https://github.com/JJWRoeloffs/transcribe_allign_textgrid/issues
 Keywords: praat,whisper,force-allign,TextGrid
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
@@ -23,15 +23,15 @@
 
 ## Requirements
 * `Python3.9` Other python versions might work, but dependency `onnxruntime` is quite iffy.
     * Use the executable `python3.9` on Unix, available in most package managers, or `py -3.9` on Windows.
     * The command line executable of python3.9 will be referred to as `[python-executable]` for the rest of the instructions
     * Install pip on old python versions with `[python-executable] -m ensurepip --default-pip`
 * `ffmpeg` Usually preinstalled on Linux. For windows see instructions for installation on the [whisper repository](https://github.com/openai/whisper)
-* `git` Usually preinstalled on Linux. For windows, visit [the git site](https://git-scm.com/download/win). 
+* `git` Usually preinstalled on Linux. For windows, visit [the git site](https://git-scm.com/download/win).
     * Needed for installation of whisper-timestamped, as it is not available on pypi
     * Note that it needs to be available from the command line; git-bash might not work.
 
 ## Light installation
 If you don't have a Nvidea GPU, or don't want to use it, you cannot use the CUDA platform on which Whisper is run. In this case, you should install a light version of torch **before** installing whisper-timestamped (and thus this application). Do this with:
 ```bash
 [python-executable] -m pip install \
@@ -51,17 +51,19 @@
 
 # Running from the command line
 Once the application is installed, you can run it with:
 ```bash
 [python-executable] -m transcribe_allign_textgrid [path]
 ```
 
-here `path` is the path to the audio files. 
+here `path` is the path to the audio files.
 * If a directory path is passed, all audio files in the directory will be transcribed, and force-alligned transcription textgrids of the same name will be generated in this directory.
-* If a file path is passed, a force-alligned transcription textgrid will be generated into the same directory as the original file.
+* If a file path is passed, a force-alligned transcription textgrid will be generated into the same directory with the same name as the original file.
+* If a glob is passed, the glob will be resoled and all matches will be processed as if the files were passed individually
+* By default, if a non-audio file is passed, an error is raised. To skip those instead, pass the `--skip` flag.
 
 ## Selecting a different model
 By default, this will run on the smallest, that is, least accurate and fastest, model, `tiny`. To run with another model, pass it as an argument:
 ```bash
 [python-executable] -m transcribe_allign_textgrid [path] --model [model]
 ```
```

### Comparing `transcribe_allign_textgrid-0.1.3/src/transcribe_allign_textgrid.egg-info/SOURCES.txt` & `transcribe_allign_textgrid-0.1.4/src/transcribe_allign_textgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `transcribe_allign_textgrid-0.1.3/tests/test_adapter.py` & `transcribe_allign_textgrid-0.1.4/tests/test_adapter.py`

 * *Files identical despite different names*

