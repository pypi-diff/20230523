# Comparing `tmp/poonia-0.1.8.tar.gz` & `tmp/poonia-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/poonia-0.1.8.tar", last modified: Wed Jul  1 23:28:31 2020, max compression
+gzip compressed data, was "dist/poonia-0.1.9.tar", last modified: Tue Apr 13 10:12:22 2021, max compression
```

## Comparing `poonia-0.1.8.tar` & `poonia-0.1.9.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-01 23:28:31.000000 poonia-0.1.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-01 23:28:31.000000 poonia-0.1.8/poonia/
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-01 23:28:31.000000 poonia-0.1.8/poonia/commands/
--rw-rw-rw-   0 root         (0) root         (0)     2251 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/duration.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4642 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/ffbook.py
--rw-rw-rw-   0 root         (0) root         (0)      533 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/sdel.py
--rw-rw-rw-   0 root         (0) root         (0)     1885 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/flatten.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/rename.py
--rw-rw-rw-   0 root         (0) root         (0)     1295 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/run.py
--rw-rw-rw-   0 root         (0) root         (0)     1626 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/esub.py
--rw-rw-rw-   0 root         (0) root         (0)     6760 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/ffsel.py
--rw-rw-rw-   0 root         (0) root         (0)      275 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/which.py
--rw-rw-rw-   0 root         (0) root         (0)     1444 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/encoding.py
--rw-rw-rw-   0 root         (0) root         (0)     3602 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/commands/pn.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2020-07-01 23:28:26.000000 poonia-0.1.8/poonia/__main__.py
--rw-r--r--   0 root         (0) root         (0)      394 2020-07-01 23:28:31.000000 poonia-0.1.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-01 23:28:31.000000 poonia-0.1.8/poonia.egg-info/
--rw-r--r--   0 root         (0) root         (0)      394 2020-07-01 23:28:31.000000 poonia-0.1.8/poonia.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      534 2020-07-01 23:28:31.000000 poonia-0.1.8/poonia.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-07-01 23:28:31.000000 poonia-0.1.8/poonia.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2020-07-01 23:28:31.000000 poonia-0.1.8/poonia.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       62 2020-07-01 23:28:31.000000 poonia-0.1.8/poonia.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        7 2020-07-01 23:28:31.000000 poonia-0.1.8/poonia.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2020-07-01 23:28:31.000000 poonia-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      605 2020-07-01 23:28:26.000000 poonia-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 10:12:22.000000 poonia-0.1.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 10:12:22.000000 poonia-0.1.9/poonia/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 10:12:22.000000 poonia-0.1.9/poonia/commands/
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/duration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/moveup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4336 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/foldertag.py
+-rw-rw-rw-   0 root         (0) root         (0)     4642 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/ffbook.py
+-rw-rw-rw-   0 root         (0) root         (0)      533 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/sdel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/flatten.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/rename.py
+-rw-rw-rw-   0 root         (0) root         (0)     1295 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/run.py
+-rw-rw-rw-   0 root         (0) root         (0)     1626 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/esub.py
+-rw-rw-rw-   0 root         (0) root         (0)     6866 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/ffsel.py
+-rw-rw-rw-   0 root         (0) root         (0)      275 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/which.py
+-rw-rw-rw-   0 root         (0) root         (0)     1444 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/encoding.py
+-rw-rw-rw-   0 root         (0) root         (0)     4173 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/commands/pn.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2021-04-13 10:12:16.000000 poonia-0.1.9/poonia/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      394 2021-04-13 10:12:22.000000 poonia-0.1.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-04-13 10:12:22.000000 poonia-0.1.9/poonia.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      394 2021-04-13 10:12:22.000000 poonia-0.1.9/poonia.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      589 2021-04-13 10:12:22.000000 poonia-0.1.9/poonia.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-04-13 10:12:22.000000 poonia-0.1.9/poonia.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2021-04-13 10:12:22.000000 poonia-0.1.9/poonia.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2021-04-13 10:12:22.000000 poonia-0.1.9/poonia.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2021-04-13 10:12:22.000000 poonia-0.1.9/poonia.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-04-13 10:12:22.000000 poonia-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      605 2021-04-13 10:12:16.000000 poonia-0.1.9/setup.py
```

### Comparing `poonia-0.1.8/poonia/commands/duration.py` & `poonia-0.1.9/poonia/commands/duration.py`

 * *Files identical despite different names*

### Comparing `poonia-0.1.8/poonia/commands/__init__.py` & `poonia-0.1.9/poonia/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `poonia-0.1.8/poonia/commands/ffbook.py` & `poonia-0.1.9/poonia/commands/ffbook.py`

 * *Files identical despite different names*

### Comparing `poonia-0.1.8/poonia/commands/sdel.py` & `poonia-0.1.9/poonia/commands/sdel.py`

 * *Files identical despite different names*

### Comparing `poonia-0.1.8/poonia/commands/flatten.py` & `poonia-0.1.9/poonia/commands/flatten.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 def split(path):
   return os.path.normpath(path).split(os.path.sep)
 
 join = os.path.join
 
 def random_name():
-  return uuid.uuid4().hex;
+  return uuid.uuid4().hex
 
 def is_single_child(path):
   base, _ = os.path.split(path)
   if base in ('', '.'): return False
   return len(os.listdir(base)) == 1
 
 def replace(path, newname, level=0):
@@ -69,12 +69,12 @@
     return None
 
 @click.command(help='Move single dirs one level up, combine names')
 @click.option('--sep', default=' - ', help='separator for joining directory names')
 def flatten(sep):
   while dir_to_flatten():
     d = dir_to_flatten()
-    click.echo(d)
-    moveup(d, sep)
+    if click.confirm(d):
+      moveup(d, sep)
 
 if __name__ == '__main__':
     flatten()
```

### Comparing `poonia-0.1.8/poonia/commands/rename.py` & `poonia-0.1.9/poonia/commands/rename.py`

 * *Files identical despite different names*

### Comparing `poonia-0.1.8/poonia/commands/run.py` & `poonia-0.1.9/poonia/commands/run.py`

 * *Files identical despite different names*

### Comparing `poonia-0.1.8/poonia/commands/esub.py` & `poonia-0.1.9/poonia/commands/esub.py`

 * *Files identical despite different names*

### Comparing `poonia-0.1.8/poonia/commands/ffsel.py` & `poonia-0.1.9/poonia/commands/ffsel.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import subprocess
 import re
 import time
 import json
 import operator
 import sys
+import locale
 
 from functools import reduce
 from collections import defaultdict
 
 def group_by(key, seq):
     return dict(reduce(lambda grp, val: grp[key(val)].append(val) or grp, seq, defaultdict(list)))
 
@@ -26,15 +27,15 @@
     if r is None: return ''
     return str(r)
 
 def findall(regexp, s):
     return [m.groupdict() for m in re.finditer(regexp, s)]
 
 def parse_stream_filters(filter, default_action='-'):
-    filters = findall('(?P<type>[vas])(?P<action>\+|\-)(?P<text>\w+)', filter)
+    filters = findall(r'(?P<type>[vas])(?P<action>\+|\-)(?P<text>\w+)', filter)
     filters = group_by(operator.itemgetter('type'), filters)
 
     actions_per_type = {t: set(f['action'] for f in fs) for t,fs in filters.items()}
     if any(1 for _,a in actions_per_type.items() if len(a) > 1):
         click.secho('You can use only one filter action type (+ or -) per stream type!', fg='red', err=True)
         sys.exit(1)
     actions_per_type = {t: list(f)[0] for t,f in actions_per_type.items()}
@@ -60,16 +61,17 @@
             return "%3.1f%s%s" % (num, unit, suffix)
         num /= 1024.0
     return "%.1f%s%s" % (num, 'Yi', suffix)
 
 FFPROBE_CMD = 'ffprobe -hide_banner -loglevel fatal -show_error -show_format -show_streams -show_programs -show_chapters -show_private_data -print_format json'.split(' ')
 def ffprobe(fn):
     try:
+        fn = fn.encode(locale.getpreferredencoding())
         r = subprocess.check_output(FFPROBE_CMD + [fn], stderr=subprocess.STDOUT)
-        return json.loads(str(r))
+        return json.loads(r.decode('utf-8'))
     except subprocess.CalledProcessError as e:
         return {'error': str(e.output)}
     return {}
 
 
 def escape_csv(s):
     if '"' or "," in s:
@@ -97,15 +99,15 @@
 @click.option('--apply', is_flag=True, help='Run conversion')
 @click.option('--force-stereo', is_flag=True, help="Convert 5.1 audio streams to stereo")
 @click.option('-c:a', 'acodec', type=click.Choice(['mp3', 'aac', 'opus']), help="Audio codec")
 @click.option('-b:a', 'abitrate', type=str, help="Audio bitrate", default='96k')
 @click.option('--hevc', is_flag=True, help='Convert video to HEVC')
 @click.option('--crf', default=28, help='Sets quality when converting video (default for HEVC 28)')
 def ffsel(input, filters, print_output, apply, force_stereo, acodec, abitrate, hevc, crf):
-    files = [f for f in os.listdir(input) if os.path.isfile(f)] if os.path.isdir(input) else [input]
+    files = [f for f in os.listdir(input) if os.path.isfile(f) and not f.startswith('.')] if os.path.isdir(input) else [input]
     
     stream_filter = parse_stream_filters(filters)
     output = []
     
     for f in files:
         cmd = ['ffmpeg', '-i', f, '-c', 'copy']
```

### Comparing `poonia-0.1.8/poonia/commands/encoding.py` & `poonia-0.1.9/poonia/commands/encoding.py`

 * *Files identical despite different names*

### Comparing `poonia-0.1.8/poonia/commands/pn.py` & `poonia-0.1.9/poonia/commands/pn.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,14 +26,33 @@
         pass
     text = sorted(decoded, key=grade, reverse=True)[0].encode('utf-8')
   except:
     pass
   text = text[3:] if text[0:3] == codecs.BOM_UTF8 else text
   return text
 
+def try_match(regexes, s):
+  for r in regexes:
+    for m in re.finditer(r, s, re.UNICODE):
+      yield (m.start(), m.groups())
+
+def filename_to_title(s):
+  before_year = list(try_match([r'^(.+)[^\d]\d{4}[^\d]'], s))[-1:]
+  episode = list(try_match([
+    r'S(\d+)E(\d+)',
+    r'(\d+)x(\d+)'
+  ], s))[:1]
+  name = s
+  if before_year: name = before_year[0][1][0]
+  if episode: name = '%s S%sE%s' % (s[:episode[0][0]], episode[0][1][0], episode[0][1][1])
+  name = re.sub(r'[^\w ]', ' ', name)
+  name = re.sub(' +', ' ', name)
+  return name.strip()
+
+
 p = {
   'headers': {
     "Accept-Language": "en,pl;q=0.8", 
     "User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/47.0.2526.106 Safari/537.36",
   },
   'verify': False
 }
@@ -103,18 +122,17 @@
     if sel > 0 and last_fn and os.path.isfile(last_fn):
       click.secho('Removing %s...' % last_fn, fg='red')
       os.remove(last_fn)
     last_fn = getsubs(e['link'], target_fn, e['lang'] and e['lang'].strip() == 'pl')
 
 @click.command(help="Download movie subtitles from podnapisi website")
 @click.argument('filename')
-def pn(filename):
+@click.option('-d', 'language', type=click.Choice(['pl', 'en']), help="Download first candidate of selected language")
+def pn(filename, language):
   if os.path.isfile(filename):
-    basename, ext = os.path.splitext(filename)
-    search = re.findall('.+s\d{2}e\d{2}', basename, re.I)
-    search = search[0] if search else basename
-    search = search.replace('.', ' ')
+    basename, _ = os.path.splitext(filename)
+    search = filename_to_title(basename)
   else:
     basename = filename
     search = filename
   click.echo('Searching %s...' % search)
   find_movie(search, basename)
```

### Comparing `poonia-0.1.8/poonia/__main__.py` & `poonia-0.1.9/poonia/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from .commands.which import which
 from .commands.pn import pn
 from .commands.flatten import flatten
 from .commands.rename import rename
 from .commands.duration import duration
 from .commands.ffbook import ffbook
 from .commands.ffsel import ffsel
+from .commands.foldertag import foldertag
+from .commands.moveup import moveup
 
 @click.group()
 def main():
     pass
 
 
 main.add_command(encoding)
@@ -24,10 +26,12 @@
 main.add_command(which)
 main.add_command(pn)
 main.add_command(flatten)
 main.add_command(rename)
 main.add_command(duration)
 main.add_command(ffbook)
 main.add_command(ffsel)
+main.add_command(foldertag)
+main.add_command(moveup)
 
 if __name__ == '__main__':
     main()
```

### Comparing `poonia-0.1.8/poonia.egg-info/SOURCES.txt` & `poonia-0.1.9/poonia.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -10,12 +10,14 @@
 poonia/commands/__init__.py
 poonia/commands/duration.py
 poonia/commands/encoding.py
 poonia/commands/esub.py
 poonia/commands/ffbook.py
 poonia/commands/ffsel.py
 poonia/commands/flatten.py
+poonia/commands/foldertag.py
+poonia/commands/moveup.py
 poonia/commands/pn.py
 poonia/commands/rename.py
 poonia/commands/run.py
 poonia/commands/sdel.py
 poonia/commands/which.py
```

### Comparing `poonia-0.1.8/setup.py` & `poonia-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='poonia',
-    version='0.1.8',
+    version='0.1.9',
     description='Collection of small utilities',
     author='proteus',
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         'Click', 'requests'
     ],
```

