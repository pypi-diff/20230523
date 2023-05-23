# Comparing `tmp/python-rtmidi-1.4.9.tar.gz` & `tmp/python-rtmidi-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-rtmidi-1.4.9.tar", last modified: Mon Apr 26 17:44:07 2021, max compression
+gzip compressed data, was "python-rtmidi-1.5.0.tar", last modified: Tue May 23 15:02:06 2023, max compression
```

## Comparing `python-rtmidi-1.4.9.tar` & `python-rtmidi-1.5.0.tar`

### file list

```diff
@@ -1,113 +1,176 @@
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.755232 python-rtmidi-1.4.9/
--rw-r--r--   0 chris     (1000) users      (100)      566 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/.gitignore
--rw-r--r--   0 chris     (1000) users      (100)      118 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/.gitmodules
--rw-r--r--   0 chris     (1000) users      (100)      274 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/AUTHORS.rst
--rw-r--r--   0 chris     (1000) users      (100)    22165 2021-04-26 16:58:09.000000 python-rtmidi-1.4.9/CHANGELOG.rst
--rw-r--r--   0 chris     (1000) users      (100)     3943 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/INSTALL-windows.rst
--rw-r--r--   0 chris     (1000) users      (100)     9803 2021-04-26 17:44:07.000000 python-rtmidi-1.4.9/INSTALL.rst
--rw-r--r--   0 chris     (1000) users      (100)     2771 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/LICENSE.txt
--rw-r--r--   0 chris     (1000) users      (100)      470 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/MANIFEST.in
--rw-r--r--   0 chris     (1000) users      (100)     1882 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/Makefile
--rw-r--r--   0 chris     (1000) users      (100)     5368 2021-04-26 17:44:07.755232 python-rtmidi-1.4.9/PKG-INFO
--rw-r--r--   0 chris     (1000) users      (100)     3375 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/README.rst
--rwxr-xr-x   0 chris     (1000) users      (100)      291 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/deploy.sh
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.744232 python-rtmidi-1.4.9/docs/
--rw-r--r--   0 chris     (1000) users      (100)     6778 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/Makefile
--rw-r--r--   0 chris     (1000) users      (100)      759 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/api.rst.inc
--rw-r--r--   0 chris     (1000) users      (100)       28 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/authors.rst
--rwxr-xr-x   0 chris     (1000) users      (100)     8734 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/conf.py
--rw-r--r--   0 chris     (1000) users      (100)     3257 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/contributing.rst
--rw-r--r--   0 chris     (1000) users      (100)       30 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/history.rst
--rw-r--r--   0 chris     (1000) users      (100)      496 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/index.rst
--rw-r--r--   0 chris     (1000) users      (100)       36 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/install-windows.rst
--rw-r--r--   0 chris     (1000) users      (100)       28 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/installation.rst
--rw-r--r--   0 chris     (1000) users      (100)       28 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/license.rst
--rw-r--r--   0 chris     (1000) users      (100)     6467 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/make.bat
--rw-r--r--   0 chris     (1000) users      (100)       55 2021-04-26 17:42:22.000000 python-rtmidi-1.4.9/docs/modules.rst
--rw-r--r--   0 chris     (1000) users      (100)     1337 2021-04-26 17:42:22.000000 python-rtmidi-1.4.9/docs/rtmidi.rst
--rw-r--r--   0 chris     (1000) users      (100)     1129 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/docs/usage.rst
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.744232 python-rtmidi-1.4.9/examples/
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.745232 python-rtmidi-1.4.9/examples/advanced/
--rw-r--r--   0 chris     (1000) users      (100)     1687 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/advanced/ccstore.py
--rw-r--r--   0 chris     (1000) users      (100)     2398 2021-04-04 13:25:46.000000 python-rtmidi-1.4.9/examples/advanced/midiclock.py
--rw-r--r--   0 chris     (1000) users      (100)     8741 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/advanced/midioutwrapper.py
--rw-r--r--   0 chris     (1000) users      (100)     2585 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/advanced/recvrpn.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.746232 python-rtmidi-1.4.9/examples/basic/
--rw-r--r--   0 chris     (1000) users      (100)      545 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/basic/contextmanager.py
--rwxr-xr-x   0 chris     (1000) users      (100)     1359 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/basic/midiin_callback.py
--rwxr-xr-x   0 chris     (1000) users      (100)     1050 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/basic/midiin_poll.py
--rwxr-xr-x   0 chris     (1000) users      (100)      991 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/basic/midiout.py
--rw-r--r--   0 chris     (1000) users      (100)     1012 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/basic/noteon2osc.py
--rw-r--r--   0 chris     (1000) users      (100)      745 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/basic/panic.py
--rwxr-xr-x   0 chris     (1000) users      (100)     1571 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/basic/probe_ports.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.748232 python-rtmidi-1.4.9/examples/drumseq/
--rw-r--r--   0 chris     (1000) users      (100)     2195 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/README.rst
--rw-r--r--   0 chris     (1000) users      (100)      275 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/break-on-through.txt
--rwxr-xr-x   0 chris     (1000) users      (100)     6485 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/drumseq.py
--rw-r--r--   0 chris     (1000) users      (100)      303 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_01.txt
--rw-r--r--   0 chris     (1000) users      (100)      303 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_02.txt
--rw-r--r--   0 chris     (1000) users      (100)      255 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_03.txt
--rw-r--r--   0 chris     (1000) users      (100)      206 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_04.txt
--rw-r--r--   0 chris     (1000) users      (100)      294 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_05.txt
--rw-r--r--   0 chris     (1000) users      (100)      303 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_06.txt
--rw-r--r--   0 chris     (1000) users      (100)      302 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_07.txt
--rw-r--r--   0 chris     (1000) users      (100)      302 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_08.txt
--rw-r--r--   0 chris     (1000) users      (100)      434 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_09.txt
--rw-r--r--   0 chris     (1000) users      (100)      435 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_10.txt
--rw-r--r--   0 chris     (1000) users      (100)      299 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_11.txt
--rw-r--r--   0 chris     (1000) users      (100)      347 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/example_12.txt
--rw-r--r--   0 chris     (1000) users      (100)      157 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/funkydrummer.txt
--rw-r--r--   0 chris     (1000) users      (100)      205 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/rosanna-shuffle.txt
--rw-r--r--   0 chris     (1000) users      (100)      477 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/drumseq/template.txt
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.748232 python-rtmidi-1.4.9/examples/midi2command/
--rw-r--r--   0 chris     (1000) users      (100)    45974 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/midi2command/000-playback.mp3
--rw-r--r--   0 chris     (1000) users      (100)     2506 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/midi2command/000-sheet.pdf
--rw-r--r--   0 chris     (1000) users      (100)     5624 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/midi2command/README.rst
--rw-r--r--   0 chris     (1000) users      (100)      522 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/midi2command/example.cfg
--rw-r--r--   0 chris     (1000) users      (100)     7132 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/midi2command/midi2command.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.749232 python-rtmidi-1.4.9/examples/midifilter/
--rw-r--r--   0 chris     (1000) users      (100)        0 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/midifilter/__init__.py
--rw-r--r--   0 chris     (1000) users      (100)     3667 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/midifilter/__main__.py
--rw-r--r--   0 chris     (1000) users      (100)     3119 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/midifilter/filters.py
--rwxr-xr-x   0 chris     (1000) users      (100)     5328 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/sendsysex.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.749232 python-rtmidi-1.4.9/examples/sequencer/
--rw-r--r--   0 chris     (1000) users      (100)     7155 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/sequencer/sequencer.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.749232 python-rtmidi-1.4.9/examples/sysex/
--rwxr-xr-x   0 chris     (1000) users      (100)      745 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/sysex/send_sysex.py
--rwxr-xr-x   0 chris     (1000) users      (100)     1056 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/sysex/send_sysex_file.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.750232 python-rtmidi-1.4.9/examples/sysexsaver/
--rw-r--r--   0 chris     (1000) users      (100)        0 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/sysexsaver/__init__.py
--rw-r--r--   0 chris     (1000) users      (100)     7022 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/sysexsaver/__main__.py
--rw-r--r--   0 chris     (1000) users      (100)    11493 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/sysexsaver/manufacturers.csv
--rw-r--r--   0 chris     (1000) users      (100)    12337 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/sysexsaver/manufacturers.py
--rw-r--r--   0 chris     (1000) users      (100)    12147 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/sysexsaver/models.py
--rw-r--r--   0 chris     (1000) users      (100)     3247 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/examples/wavetablemodstep.py
--rwxr-xr-x   0 chris     (1000) users      (100)     2266 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/fill_template.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.750232 python-rtmidi-1.4.9/python_rtmidi.egg-info/
--rw-r--r--   0 chris     (1000) users      (100)     5368 2021-04-26 17:43:59.000000 python-rtmidi-1.4.9/python_rtmidi.egg-info/PKG-INFO
--rw-r--r--   0 chris     (1000) users      (100)     2397 2021-04-26 17:43:59.000000 python-rtmidi-1.4.9/python_rtmidi.egg-info/SOURCES.txt
--rw-r--r--   0 chris     (1000) users      (100)        1 2021-04-26 17:43:59.000000 python-rtmidi-1.4.9/python_rtmidi.egg-info/dependency_links.txt
--rw-r--r--   0 chris     (1000) users      (100)        1 2021-04-26 17:43:59.000000 python-rtmidi-1.4.9/python_rtmidi.egg-info/not-zip-safe
--rw-r--r--   0 chris     (1000) users      (100)        7 2021-04-26 17:43:59.000000 python-rtmidi-1.4.9/python_rtmidi.egg-info/top_level.txt
--rw-r--r--   0 chris     (1000) users      (100)      863 2021-04-25 19:01:24.000000 python-rtmidi-1.4.9/requirements-dev.txt
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.751232 python-rtmidi-1.4.9/rtmidi/
--rw-r--r--   0 chris     (1000) users      (100)      202 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/rtmidi/__init__.py
--rw-r--r--   0 chris     (1000) users      (100)     7533 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/rtmidi/midiconstants.py
--rw-r--r--   0 chris     (1000) users      (100)     9158 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/rtmidi/midiutil.py
--rw-r--r--   0 chris     (1000) users      (100)       18 2021-04-26 17:40:18.000000 python-rtmidi-1.4.9/rtmidi/version.py
--rw-r--r--   0 chris     (1000) users      (100)     1614 2021-04-26 17:44:07.756232 python-rtmidi-1.4.9/setup.cfg
--rw-r--r--   0 chris     (1000) users      (100)     6411 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/setup.py
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.754233 python-rtmidi-1.4.9/src/
--rw-r--r--   0 chris     (1000) users      (100)   734092 2021-04-26 17:43:59.000000 python-rtmidi-1.4.9/src/_rtmidi.cpp
--rw-r--r--   0 chris     (1000) users      (100)    39445 2021-04-26 15:11:54.000000 python-rtmidi-1.4.9/src/_rtmidi.pyx
--rw-r--r--   0 chris     (1000) users      (100)      706 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/src/pyinit.h
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.754233 python-rtmidi-1.4.9/src/rtmidi/
--rw-r--r--   0 chris     (1000) users      (100)   113976 2021-04-26 16:50:00.000000 python-rtmidi-1.4.9/src/rtmidi/RtMidi.cpp
--rw-r--r--   0 chris     (1000) users      (100)    25866 2021-04-26 16:45:12.000000 python-rtmidi-1.4.9/src/rtmidi/RtMidi.h
-drwxr-xr-x   0 chris     (1000) users      (100)        0 2021-04-26 17:44:07.755232 python-rtmidi-1.4.9/tests/
--rw-r--r--   0 chris     (1000) users      (100)     2484 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/tests/test_delete.py
--rw-r--r--   0 chris     (1000) users      (100)     2100 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/tests/test_errorcallback.py
--rw-r--r--   0 chris     (1000) users      (100)     2299 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/tests/test_errors.py
--rw-r--r--   0 chris     (1000) users      (100)     9256 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/tests/test_rtmidi.py
--rw-r--r--   0 chris     (1000) users      (100)      278 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/tox.ini
--rwxr-xr-x   0 chris     (1000) users      (100)      346 2021-01-27 20:58:15.000000 python-rtmidi-1.4.9/update-docs.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:02:01.428790 python-rtmidi-1.5.0/
+-rw-rw-r--   0 runner    (1001) docker     (123)       94 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.flake8
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.github/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.github/workflows/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2232 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.github/workflows/development.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     2124 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.github/workflows/production.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)     1553 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.github/workflows/tests.yml
+-rw-rw-r--   0 runner    (1001) docker     (123)      571 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.gitignore
+-rw-rw-r--   0 runner    (1001) docker     (123)      118 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/.gitmodules
+-rw-rw-r--   0 runner    (1001) docker     (123)      246 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/AUTHORS.md
+-rw-rw-r--   0 runner    (1001) docker     (123)    21032 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/CHANGELOG.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     3849 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/INSTALL-windows.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     8352 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/INSTALL.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     2771 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/LICENSE.md
+-rw-rw-r--   0 runner    (1001) docker     (123)      393 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/MANIFEST.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     2497 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (123)     2778 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/README.md
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/
+-rw-rw-r--   0 runner    (1001) docker     (123)     6778 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/Makefile
+-rw-rw-r--   0 runner    (1001) docker     (123)      759 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/api.rst.inc
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/authors.md
+-rwxrwxr-x   0 runner    (1001) docker     (123)     8521 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/conf.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3257 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/contributing.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)       33 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/history.md
+-rw-rw-r--   0 runner    (1001) docker     (123)      478 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/index.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)       39 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/install-windows.md
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/installation.md
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/license.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     6467 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/make.bat
+-rw-rw-r--   0 runner    (1001) docker     (123)       55 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/modules.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/readme.md
+-rw-rw-r--   0 runner    (1001) docker     (123)     1337 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/rtmidi.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)     1129 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/docs/usage.rst
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/advanced/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1687 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/advanced/ccstore.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2398 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/advanced/midiclock.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     8741 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/advanced/midioutwrapper.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2585 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/advanced/recvrpn.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/
+-rw-rw-r--   0 runner    (1001) docker     (123)      545 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/contextmanager.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1359 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/midiin_callback.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1050 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/midiin_poll.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)      991 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/midiout.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1012 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/noteon2osc.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      765 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/panic.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1571 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/basic/probe_ports.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2195 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)      275 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/break-on-through.txt
+-rwxrwxr-x   0 runner    (1001) docker     (123)     6485 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/drumseq.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_01.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_02.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      255 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_03.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      206 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_04.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      294 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_05.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      303 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_06.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_07.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      302 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_08.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      434 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_09.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      435 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_10.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      299 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_11.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      347 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/example_12.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      157 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/funkydrummer.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      205 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/rosanna-shuffle.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      477 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/drumseq/template.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/
+-rw-rw-r--   0 runner    (1001) docker     (123)    45974 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/000-playback.mp3
+-rw-rw-r--   0 runner    (1001) docker     (123)     2506 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/000-sheet.pdf
+-rw-rw-r--   0 runner    (1001) docker     (123)     5624 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/README.rst
+-rw-rw-r--   0 runner    (1001) docker     (123)      522 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/example.cfg
+-rw-rw-r--   0 runner    (1001) docker     (123)     7132 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midi2command/midi2command.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midifilter/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midifilter/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3667 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midifilter/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3119 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/midifilter/filters.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     5328 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sendsysex.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sequencer/
+-rw-rw-r--   0 runner    (1001) docker     (123)     7155 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sequencer/sequencer.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysex/
+-rwxrwxr-x   0 runner    (1001) docker     (123)      745 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysex/send_sysex.py
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1067 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysex/send_sysex_file.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     7022 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/__main__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    11493 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/manufacturers.csv
+-rw-rw-r--   0 runner    (1001) docker     (123)    12337 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/manufacturers.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    12147 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/sysexsaver/models.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3247 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/examples/wavetablemodstep.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2687 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)      801 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/meson_options.txt
+-rwxrwxr-x   0 runner    (1001) docker     (123)      405 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/meson_postinstall.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3004 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (123)       91 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/requirements-dev.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     2845 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/requirements-dev.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/
+-rw-rw-r--   0 runner    (1001) docker     (123)      165 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1826 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/meson.build
+-rw-rw-r--   0 runner    (1001) docker     (123)     7533 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/midiconstants.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9261 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/midiutil.py
+-rw-rw-r--   0 runner    (1001) docker     (123)       30 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/rtmidi/version.py.in
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:02:02.088810 python-rtmidi-1.5.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   735881 2023-05-23 15:02:02.088810 python-rtmidi-1.5.0/src/_rtmidi.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)    39464 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/src/_rtmidi.pyx
+-rw-rw-r--   0 runner    (1001) docker     (123)      857 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/src/meson.build
+-rwxrwxr-x   0 runner    (1001) docker     (123)     1260 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/src/meson_dist_cython.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/
+-rw-rw-r--   0 runner    (1001) docker     (123)     9589 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/CMakeLists.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)     1349 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/LICENSE
+-rw-rw-r--   0 runner    (1001) docker     (123)      533 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/Makefile.am
+-rw-rw-r--   0 runner    (1001) docker     (123)     2396 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/README.md
+-rw-rw-r--   0 runner    (1001) docker     (123)   126832 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/RtMidi.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)    27069 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/RtMidi.h
+-rwxrwxr-x   0 runner    (1001) docker     (123)     2884 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/autogen.sh
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/cmake/
+-rw-rw-r--   0 runner    (1001) docker     (123)      252 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/cmake/RtMidi-config.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      940 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/cmake/RtMidiConfigUninstall.cmake.in
+-rw-rw-r--   0 runner    (1001) docker     (123)     9307 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/configure.ac
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/
+-rw-rw-r--   0 runner    (1001) docker     (123)     8909 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/rtmidi.go
+-rw-rw-r--   0 runner    (1001) docker     (123)       94 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)       31 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/rtmidi_stub.h
+-rw-rw-r--   0 runner    (1001) docker     (123)      758 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/contrib/go/rtmidi/rtmidi_test.go
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/
+-rw-rw-r--   0 runner    (1001) docker     (123)      682 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/Makefile.am
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/
+-rw-rw-r--   0 runner    (1001) docker     (123)    81155 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/Doxyfile.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      254 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/footer.html
+-rw-rw-r--   0 runner    (1001) docker     (123)      494 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/header.html
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/samples/
+-rw-rw-r--   0 runner    (1001) docker     (123)      173 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/samples/getting_started.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)    21717 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/doxygen/tutorial.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/images/
+-rw-rw-r--   0 runner    (1001) docker     (123)     3527 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/images/ccrma.gif
+-rw-rw-r--   0 runner    (1001) docker     (123)     4614 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/images/mcgill.gif
+-rw-rw-r--   0 runner    (1001) docker     (123)     7130 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/doc/release.txt
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/m4/
+-rw-rw-r--   0 runner    (1001) docker     (123)    19367 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/m4/ax_cxx_compile_stdcxx.m4
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/msw/
+-rw-rw-r--   0 runner    (1001) docker     (123)      171 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/msw/readme
+-rwxrwxr-x   0 runner    (1001) docker     (123)      883 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/msw/rtmidilib.sln
+-rwxrwxr-x   0 runner    (1001) docker     (123)     3734 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/msw/rtmidilib.vcproj
+-rw-rw-r--   0 runner    (1001) docker     (123)      388 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/rtmidi-config.in
+-rw-rw-r--   0 runner    (1001) docker     (123)      369 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/rtmidi.pc.in
+-rw-rw-r--   0 runner    (1001) docker     (123)    10140 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/rtmidi_c.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     9470 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/rtmidi_c.h
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/Debug/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/Debug/.placeholder
+-rw-rw-r--   0 runner    (1001) docker     (123)     1018 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/Makefile.am
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/Release/
+-rw-rw-r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/Release/.placeholder
+-rw-rw-r--   0 runner    (1001) docker     (123)     1311 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/RtMidi.dsw
+-rw-rw-r--   0 runner    (1001) docker     (123)     5284 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/apinames.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     2873 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/cmidiin.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/cmidiin.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     5541 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/midiclock.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     3147 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/midiout.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/midiout.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     2138 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/midiprobe.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4356 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/midiprobe.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     2361 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/qmidiin.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4320 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/qmidiin.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)     3926 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/sysextest.cpp
+-rw-rw-r--   0 runner    (1001) docker     (123)     4360 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/sysextest.dsp
+-rw-rw-r--   0 runner    (1001) docker     (123)      667 2023-05-22 16:26:33.000000 python-rtmidi-1.5.0/src/rtmidi/tests/testcapi.c
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tests/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2484 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tests/test_delete.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2100 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tests/test_errorcallback.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2299 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tests/test_errors.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     9256 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tests/test_rtmidi.py
+-rw-rw-r--   0 runner    (1001) docker     (123)      298 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/tox.ini
+-rwxrwxr-x   0 runner    (1001) docker     (123)      346 2023-05-23 15:01:07.000000 python-rtmidi-1.5.0/update-docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-05-23 15:02:06.152952 python-rtmidi-1.5.0/PKG-INFO
```

### Comparing `python-rtmidi-1.4.9/.gitignore` & `python-rtmidi-1.5.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,19 @@
 
 # Cython output
 src/_rtmidi.cpp
 
 # C extensions
 *.so
 
-# Generated documentation
-#INSTALL.rst
-
 # Packages
 *.egg
 *.egg-info
 dist/
-build/
+wheelhouse/
 *.eggs/
 eggs/
 parts/
 .installed.cfg
 setuptools-*.tar.gz
 distribute-*.tar.gz
 MANIFEST
@@ -45,10 +42,12 @@
 
 # Complexity
 output/*.html
 output/*/index.html
 
 # Sphinx
 docs/_build
+# docs build artifact
+rtmidi/version.py
 
 # Geany project
 python-rtmidi.geany
```

### Comparing `python-rtmidi-1.4.9/CHANGELOG.rst` & `python-rtmidi-1.5.0/CHANGELOG.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,659 +1,677 @@
-Changelog
-=========
+# Changelog
 
-For details and minor changes, please see the `version control log messages
-<https://github.com/SpotlightKid/python-rtmidi/commits/master>`_.
+For details and minor changes, please see the [version control log
+messages](https://github.com/SpotlightKid/python-rtmidi/commits/master).
 
 
-2021-04-26 version 1.4.9
-------------------------
+## 1.4.9 (2021-04-26)
 
 Fixes:
-    * Fixed Windows build for 64-bit Python 3.9 on AppVeyor CI.
+
+-   Fixed Windows build for 64-bit Python 3.9 on AppVeyor CI.
 
 Changes:
-    * The SysEx reception buffer size for the Windows MM backend was changed
-      from 8096 to 8196.
-    * Synced with upstream RtMidi_ (3dc525baf3cac345cdd3511316571c20b47f30b5,
-      fixes #89).
+
+-   The SysEx reception buffer size for the Windows MM backend was
+    changed from 8096 to 8196.
+-   Synced with upstream [RtMidi](https://github.com/thestk/rtmidi)
+    (3dc525baf3cac345cdd3511316571c20b47f30b5, fixes #89).
 
 
-2021-04-26 version 1.4.8
-------------------------
+## 1.4.8 (2021-04-26)
 
 Fixes:
-    * Fixed Windows builds on AppVeyor CI.
-    * Fixed command line parsing in ``midiclock.py`` example script.
+
+-   Fixed Windows builds on AppVeyor CI.
+-   Fixed command line parsing in `midiclock.py` example script.
 
 Changes:
-    * Release GIL in ``MidiOut.send_message`` so that on backend APIs where
-      this operation is blocking (``WINDOWS_MM``), multiple Python threads
-      using this method on different ``MidiOut`` instances can run concurently.
+
+-   Release GIL in `MidiOut.send_message` so that on backend APIs
+    where this operation is blocking (`WINDOWS_MM`), multiple Python
+    threads using this method on different `MidiOut` instances can
+    run concurently.
 
 
-2021-01-27 version 1.4.7
-------------------------
+## 1.4.7 (2021-01-27)
 
 Fixes:
-    * Fixed compiler deprecation warning about ``PyEval_InitThreads`` on
-      Python 3.9+.
+
+-   Fixed compiler deprecation warning about `PyEval_InitThreads` on
+    Python 3.9+.
 
 Examples:
-    * Added ``send_sysex`` and ``send_sysex_file`` example scripts.
+
+-   Added `send_sysex` and `send_sysex_file` example scripts.
 
 Documentation:
-    * Remove references to old project homepage URL and fix readme badges.
+
+-   Remove references to old project homepage URL and fix readme
+    badges.
 
 
-2020-10-15 version 1.4.6
-------------------------
+## 1.4.6 (2020-10-15)
 
 Project infrastructure:
-    * Declared/documented Python 3.9 support and updated CI.
-    * Dropped official support for Python 3.5.
-    * Updated Python versions for building macOS binary wheels.
 
+-   Declared/documented Python 3.9 support and updated CI.
+-   Dropped official support for Python 3.5.
+-   Updated Python versions for building macOS binary wheels.
 
-2020-08-26 version 1.4.5
-------------------------
+
+## 1.4.5 (2020-08-26)
 
 Fixes:
-    * Revert to old way of reading version number via ``exec`` (see 8d9a8f9
-      for background info).
+
+-   Revert to old way of reading version number via `exec` (see
+    8d9a8f9 for background info).
 
 
-2020-08-26 version 1.4.4
-------------------------
+## 1.4.4 (2020-08-26)
 
 Fixes:
-    * Fixed ``setup.py`` to work with Python 2 again, though it is not
-      officially supported anymore (#70, #72).
 
+-   Fixed `setup.py` to work with Python 2 again, though it is not
+    officially supported anymore (#70, #72).
 
-2020-08-11 version 1.4.3
-------------------------
+
+## 1.4.3 (2020-08-11)
 
 Fixes:
-    * Fixed error when trying to import version number from ``rtmidi.release``
-      when Python is running with ``-OO`` optimization enabled (#69).
+
+-   Fixed error when trying to import version number from `rtmidi.release`
+    when Python is running with `-OO` optimization enabled (#69).
 
 Project infrastructure:
-    * Moved distribution meta data to ``setup.cfg``, added
-      ``rtmidi/version.py`` and removed ``rtmidi/release.py`` (#69).
 
+-   Moved distribution meta data to `setup.cfg`, added
+    `rtmidi/version.py` and removed `rtmidi/release.py` (#69).
 
-2020-07-18 version 1.4.2
-------------------------
+
+## 1.4.2 (2020-07-18)
 
 Enhancements:
-    * Added more helpful aliases for MIDI events/controllers constants.
+
+-   Added more helpful aliases for MIDI events/controllers constants.
 
 Examples:
-    * Added ``ccstore`` advanced example to show how to remember last seen
-      controller change values (#64).
+
+-   Added `ccstore` advanced example to show how to remember last seen
+    controller change values (#64).
 
 
-2020-04-16 version 1.4.1
-------------------------
+## 1.4.1 (2020-04-16)
 
 Changes:
-    * Suppress RtMidi warnings to stderr, so that warnings issued in the
-      constructor of the ``RtMidiIn/Out`` C++ class instances before the
-      default error handler function can be attached, don't end up in the
-      output.
-
-      The suppression of RtMidi warnings can be disabled at compile time
-      by setting the pre-compiler define ``__RTMIDI_SUPPRESS_WARNINGS__``
-      via a command line option to ``setup.py``.
-
-      As before, RtMidi warnings are turned into Python a ``UserWarning``
-      as soon as the default error handler is attached, but this can only
-      happen after the RtMidi C++ class has been instantiated (#59).
-    * Allow deletion of internal C++ RtMidiIn/Out instance via new
-      ``delete`` method of ``rtmidi.MidiIn`` and ``rtmidi.MidiOut``
-      instances (but see warning in docstring!). Also added a
-      ``is_deleted`` property to both classes (#60).
 
+-   Suppress RtMidi warnings to stderr, so that warnings issued in
+    the constructor of the `RtMidiIn/Out` C++ class instances before
+    the default error handler function can be attached, don't end
+    up in the output.
 
-2020-01-19 version 1.4.0
-------------------------
+    The suppression of RtMidi warnings can be disabled at compile time by
+    setting the pre-compiler define `__RTMIDI_SUPPRESS_WARNINGS__` via a
+    command line option to `setup.py`.
+
+    As before, RtMidi warnings are turned into Python a `UserWarning` as soon
+    as the default error handler is attached, but this can only happen after
+    the RtMidi C++ class has been instantiated (#59).
+
+-   Allow deletion of internal C++ RtMidiIn/Out instance via new `delete`
+    method of `rtmidi.MidiIn` and `rtmidi.MidiOut` instances (but see warning
+    in docstring!). Also added a `is_deleted` property to both classes (#60).
+
+
+## 1.4.0 (2020-01-19)
 
 Changes:
-    * Dropped nominal Python 2 support (no code changes or removals related
-      to this, though).
-    * Dropped Python 3.4 support.
-    * Added Python 3.8 to ``setup.py`` classifier.
+
+-   Dropped nominal Python 2 support (no code changes or removals
+    related to this, though).
+-   Dropped Python 3.4 support.
+-   Added Python 3.8 to `setup.py` classifier.
 
 Enhancements:
-    * Added ``MODULATION`` as an alias for ``MODULATION_WHEEL`` to
-      ``rtmidi.midiconstants``.
+
+-   Added `MODULATION` as an alias for `MODULATION_WHEEL` to
+    `rtmidi.midiconstants`.
 
 Examples:
-    * Added ``midiclock`` example to show how to receive MIDI timing clock
-      (#48).
-    * Changed ``midioutwrapper`` example to use
-      ``rtmidi.midiutil.open_midiout`` so that it also works on Windows (with
-      no virtual ports support) (#51).
-
-Documentation:
-  * Added note about ``pip`` being called ``pip3`` on Debian-based systems
-    to install instructions (#49).
-  * Documented context manager protocol support better (#52).
-  * Clarified purpose of ``data`` argument of ``MidiIn.set_callback`` (#55).
-  * Updated year in copyright info in license file and Sphinx documentation.
+
+-   Added `midiclock` example to show how to receive MIDI timing clock (#48).
+-   Changed `midioutwrapper` example to use `rtmidi.midiutil.open_midiout` so
+    that it also works on Windows (with no virtual ports support) (#51).
+
+Documentation:
+
+-   Added note about `pip` being called `pip3` on Debian-based systems to
+    install instructions (#49).
+-   Documented context manager protocol support better (#52).
+-   Clarified purpose of `data` argument of `MidiIn.set_callback` (#55).
+-   Updated year in copyright info in license file and Sphinx documentation.
+
 
 Project infrastructure:
-    * Removed Python 2.7 from CI tests and package builds.
-    * Added Python 3.8 to CI and package builds.
 
+-   Removed Python 2.7 from CI tests and package builds.
+-   Added Python 3.8 to CI and package builds.
 
-2019-10-15 version 1.3.1
-------------------------
+
+## 1.3.1 (2019-10-15)
 
 Enhancements / Changes:
-  * RtMidi C++ exceptions are now caught when creating ``RtMidiIn/Out``
-    instances and converted into a Python ``rtmidi.SystemError``
-    exception.
-  * Helper functions in ``rtmidi.midiutil`` now raise sub-classes of
-    ``rtmidi.RtMidiError`` wherever appropriate. The docstrings where updated
+
+-   RtMidi C++ exceptions are now caught when creating `RtMidiIn/Out` instances
+    and converted into a Python `rtmidi.SystemError` exception.
+-   Helper functions in `rtmidi.midiutil` now raise sub-classes of
+    `rtmidi.RtMidiError` wherever appropriate. The docstrings were updated
     accordingly.
-  * Updated ``rtmidi`` sub-module, which includes the following changes:
+-   Updated `rtmidi` sub-module, which includes the following changes:
+    -   C++ exceptions, when thrown, do not print the error message to stderr
+        anymore.
+    -   When the JACK backend can't be initialized (e.g. when the server isn't
+        running) it causes a `DRIVER_ERROR` instead of just a printing a
+        `WARNING`.
 
-    * C++ exceptions, when thrown, do not print the error message to stderr
-      anymore.
-    * When the JACK backend can't be initialized (e.g. when the server isn't
-      running) it causes a ``DRIVER_ERROR`` instead of just a printing a
-      ``WARNING``.
-
-Examples:
-  * ``midiout.py``: removed surplus second argument to ``open_midioutput``
-    left over from previous version of script.
-  * Renamed example script ``midiwrapper.py`` to ``midioutwrapper.py`` to
-    better indicate its function.
-  * ``sendsysex.py``: use helper functions from midiutil module to list
-    and open MIDI ports; improve error handling.
-  * Made sure MIDI ports are always properly closed and ``MidiIn/Out``
-    instances are deleted.
-  * Inserted delay before closing/deleting output (may be needed with
-    Windows MMS).
-  * Simplified command line argument handling.
-  * Fixed example script file names in header comments.
+Examples:
+
+-   `midiout.py`: removed surplus second argument to `open_midioutput` left
+    over from previous version of script.
+-   Renamed example script `midiwrapper.py` to `midioutwrapper.py` to better
+    indicate its function.
+-   `sendsysex.py`: use helper functions from midiutil module to list and open
+    MIDI ports; improve error handling.
+-   Made sure MIDI ports are always properly closed and `MidiIn/Out` instances
+    are deleted.
+-   Inserted delay before closing/deleting output (may be needed with Windows
+    MMS).
+-   Simplified command line argument handling.
+-   Fixed example script file names in header comments.
 
 Documentation:
-  * Made various small documentation wording changes and typo fixes.
-  * Updated year in copyright info in license file and Sphinx documentation.
+
+-   Made various small documentation wording changes and typo fixes.
+-   Updated year in copyright info in license file and Sphinx documentation.
 
 Project infrastructure:
-  * Updated development dependency on ``urllib3`` to 1.24.2 (CVE-2019-11324).
 
+-   Updated development dependency on `urllib3` to 1.24.2 (CVE-2019-11324).
 
-2019-04-15 version 1.3.0
-------------------------
+
+## 1.3.0 (2019-04-15)
 
 Enhancements / Changes:
-  * Added ``get_api_display_name`` module-level function.
-  * Added ``get_api_name`` module-level function.
-  * Added ``get_compiled_api_by_name`` module-level function.
-  * Updated ``rtmidi`` sub-module to include all changes from upstream up to
+
+-   Added `get_api_display_name` module-level function.
+-   Added `get_api_name` module-level function.
+-   Added `get_compiled_api_by_name` module-level function.
+-   Updated `rtmidi` sub-module to include all changes from upstream up to
     commit 791dfea.
 
 Documentation:
-  * Improved installation instructions and listed options recognized by
-    ``setup.py``.
 
+-   Improved installation instructions and listed options recognized by
+    `setup.py`.
 
-2019-01-18 version 1.2.1
-------------------------
+
+## 1.2.1 (2019-01-18)
 
 Fixes:
-  * Fixed build when compiling with JACK support, but JACK version is too old
-    to have ``jack_port_rename`` function (#40).
+
+-   Fixed build when compiling with JACK support, but JACK version is too old
+    to have `jack_port_rename` function (#40).
 
 Project infrastructure:
-  * Added Linux builds for Python 2.7 and 3.4 - 3.7 to Travis CI setup.
+
+-   Added Linux builds for Python 2.7 and 3.4 - 3.7 to Travis CI setup.
 
 
-2019-01-13 version 1.2.0
-------------------------
+## 1.2.0 (2019-01-13)
 
 Project infrastructure:
-  * RtMidi Sources and header are now included as a git sub-module from
-    the 'python-rtmidi' branch of a fork_ of the upstream RtMidi repository.
-    This fork incorporates changes and fixes by pull requests to the
-    upstream repository, which are (yet) unmerged, and some changes
-    specific to python-rtmidi.
+
+-   RtMidi Sources and header are now included as a git sub-module from the
+    'python-rtmidi' branch of a [fork] of the upstream RtMidi repository. This
+    fork incorporates changes and fixes by pull requests to the upstream
+    repository, which are (yet) unmerged, and some changes specific to
+    python-rtmidi.
+
+[fork]: https://github.com/SpotlightKid/rtmidi
 
 Enhancements / Changes:
-  * Added ``get_rtmidi_version`` module-level function.
-  * Added ``set_client_name`` and ``set_port_name`` methods to ``MidiIn``'s and
-    ``MidiOut``'s base class.
-  * Added a bunch of new custom exceptions, all derived from ``RtMidiError``.
-  * A default error handler callback is now set for ``MidiIn`` and ``MidiOut``
+
+-   Added `get_rtmidi_version` module-level function.
+-   Added `set_client_name` and `set_port_name` methods to `MidiIn`'s and
+    `MidiOut`'s base class.
+-   Added a bunch of new custom exceptions, all derived from `RtMidiError`.
+-   A default error handler callback is now set for `MidiIn` and`MidiOut`
     instances, which maps C++ level errors into custom Python exceptions.
 
 Examples:
-  * Enhanced example script ``midiwrapper.py`` with methods for more MIDI
-    messages, including sending all kinds of controller change and of (N)RPN
-    messages.
+
+-   Enhanced example script `midiwrapper.py` with methods for more MIDI
+    messages, including sending all kinds of controller change and of
+    (N)RPN messages.
 
 Fixes:
-  * Fixed SysEx message reception in JACK backend in RtMidi: messages broken up
+
+-   Fixed SysEx message reception in JACK backend in RtMidi: messages broken up
     over several events are now collected into a single event before being
-    passed to the input callback or returned by ``MidiIn.get_message``.
-  * Fixed missing MIDI message input filtering in JACK backend in RtMidi:
-    ``MidiIn.ignoreTypes`` now works as intended.
+    passed to the input callback or returned by `MidiIn.get_message`.
+-   Fixed missing MIDI message input filtering in JACK backend in RtMidi:
+    `MidiIn.ignoreTypes` now works as intended.
 
 Testing:
-  * Restructured tests in ``test_rtmidi`` and added tests for new methods.
-
 
-.. _fork:
-    https://github.com/SpotlightKid/rtmidi
+-   Restructured tests in `test_rtmidi` and added tests for new methods.
 
 
-2018-10-10 version 1.1.2
-------------------------
+## 1.1.2 (2018-10-10)
 
 Project infrastructure:
-  * Added bagdes and link to documentation to README visible on GitHub page.
-  * Tweaked project description wording.
-  * Updated copyright year in various documentation files.
 
-Building:
-  * Binary wheels for Windows and OS X for Python 2.7, 3.5 (only Windows), 3.6,
-    and 3.7 are automatically built on AppVeyor resp. Travis CI and uploaded to
-    PyPI when a new release tag is pushed to GitHub.
+-   Added bagdes and link to documentation to README visible on GitHub page.
+-   Tweaked project description wording.
+-   Updated copyright year in various documentation files.
 
-    Thanks to Benoit Pierre for the PR (#36).
-  * Upload Gzip'ed instead Bzip'ed tarballs for source distributions to PyPI.
-  * ``python setup.py test`` now runs ``tox``, so ``tests_require`` in
-    ``setup.py`` is empty now. We want dependencies to be only handled by
-    ``pip``, never by ``setuptools``.
+Building:
 
-Documentation:
-  * Minor additions, updates, fixes and wording tweaks.
+-   Binary wheels for Windows and OS X for Python 2.7, 3.5 (only Windows), 3.6,
+    and 3.7 are automatically built on AppVeyor resp. Travis CI and uploaded
+    to PyPI when a new release tag is pushed to GitHub.
 
+    Thanks to Benoit Pierre for the PR (#36).
 
-2018-08-06 version 1.1.1
-------------------------
+-   Upload Gzip\'ed instead Bzip\'ed tarballs for source distributions to PyPI.
 
-Building:
-  * Rebuild ``src/_rtmidi.cpp`` with current Cython for Python 3.7
-    compatibility.
-  * Remove testing with Python 3.3 environment from ``tox.ini`` and add Python
-    3.6 and 3.7.
-  * Update dev requirements for Python 3.7 compatibility.
-  * Upload releases with twine.
+-   `python setup.py test` now runs `tox`, so `tests_require` in `setup.py` is
+    empty now. We want dependencies to be only handled by `pip`, never by
+    `setuptools`.
 
 Documentation:
-  * Python 3.3 is not officially tested or supported anymore.
 
+-   Minor additions, updates, fixes and wording tweaks.
 
-2017-04-21 version 1.1.0
-------------------------
 
-Project infrastructure:
-  * Updated project homepage URL; copyright year and link to docs in readme.
+## 1.1.1 (2018-08-06)
 
 Building:
-  * Added script to automate updating github pages docs.
 
-Enhancements / Changes:
-  * Synced with upstream RtMidi_ (2.1.1-907a94c).
-  * Applied patch from https://github.com/thestk/rtmidi/pull/89.
-    This means that when using the ALSA API port names are reported in the form
-    ``<client name>:<port name> <port id>`` (this change was actually already
-    in version 1.0.0).
-  * Added new ``MidiIn`` / ``MidiOut`` method ``is_port_open``.
-  * ``MidiIn`` / ``MidiOut`` constructors and ``open_port`` /
-    ``open_virtual_port`` methods now raise ``TypeError`` when an
-    invalid type is passed as the client resp. port name.
+-   Rebuild `src/_rtmidi.cpp` with current Cython for Python 3.7 compatibility.
+-   Remove testing with Python 3.3 environment from `tox.ini` and add Python
+    3.6 and 3.7.
+-   Update dev requirements for Python 3.7 compatibility.
+-   Upload releases with twine.
 
 Documentation:
-  * Various small documentation improvements.
 
-Examples:
-  * Basic examples: some clean-up, more comments, updated API usage.
-  * Added new advanced example script ``midiwrapper.py``.
-  * Added new advanced example script ``recvrpn.py``.
-  * ``wavetablemodstep.py``: added command line param to set controller number.
-  * ``midi2command``: Fixed wrong mock lru_cache substitution for Python < 3.2.
+-   Python 3.3 is not officially tested or supported anymore.
 
 
-2016-11-07 version 1.0.0
-------------------------
+## 1.1.0 (2017-04-21)
 
 Project infrastructure:
-  * Added automatic documentation publishing on readthedocs.org.
 
-Documentation:
-  * Added auto docs for MidiIn/MidiOut classes to sphinx docs.
-  * Removed pre-release related information from installation docs.
+-   Updated project homepage URL; copyright year and link to docs in readme.
 
 Building:
-  * Added generated INSTALL.rst to repo to make ReadTheDocs integration work.
-
-Examples:
-  * Added new example script ``panic.py``.
 
+-   Added script to automate updating github pages docs.
 
-2016-10-09 version 1.0.0rc1
----------------------------
-
-Project infrastructure:
-  * Moved repository to Github.
+Enhancements / Changes:
 
-Fixes:
-  * ``midiutil.open_midiport``:
+-   Synced with upstream [RtMidi] (2.1.1-907a94c).
+-   Applied patch from <https://github.com/thestk/rtmidi/pull/89>.
+    This means that when using the ALSA API port names are reported
+    in the form `<client name>:<port name> <port id>` (this change
+    was actually already in version 1.0.0).
+-   Added new `MidiIn` / `MidiOut` method `is_port_open`.
+-   `MidiIn` / `MidiOut` constructors and `open_port` / `open_virtual_port`
+    methods now raise `TypeError` when an invalid type is passed as the
+    client resp. port name.
 
-    * Correctly report and log I/O direction and instance type.
-    * Fix naming of virtual port.
+[RtMidi]: (https://github.com/thestk/rtmidi
 
-Enhancements / Changes:
-  * Synced with upstream RtMidi_ (2.1.1-399a8ee).
-  * ``midiutil``:
+Documentation:
 
-    * The function ``midiutil.open_port`` has been renamed to ``open_midiport``.
+-   Various small documentation improvements.
 
-    * Added convenience functions ``open_midiinput`` and ``open_midioutput``,
-      which wrap ``open_midiport``.
+Examples:
 
-    * RtMidi API to use can be specified via the ``RTMIDI_API`` environment
-      variable. Only used when ``API_UNSPECIFIED`` is passed for the ``api``
-      argument. Value should be one of the ``API_*`` constant names with out
-      the ``API_`` prefix, e.g. ``UNIX_JACK`` for the Jack API.
+-   Basic examples: some clean-up, more comments, updated API usage.
+-   Added new advanced example script `midiwrapper.py`.
+-   Added new advanced example script `recvrpn.py`.
+-   `wavetablemodstep.py`: added command line param to set controller number.
+-   `midi2command`: Fixed wrong mock lru_cache substitution for Python < 3.2.
 
-  * Cython wrapper class hierarchy restructured to better match the underlying
-    C++ classes and remove code duplication.
-  * Some source code re-ordering was done.
 
-Documentation:
-  * Added basic structure and initial content of Sphinx documentation.
-  * Documented exceptions raised by ``MidiIn/Out.open_[virtual_]port()``.
-  * Some docstring corrections and formatting fixes.
+## 1.0.0 (2016-11-07)
 
-Building:
-  * Simplified ``setup.py`` by throwing out old compatibility stuff.
-  * Explicitly call ``PyEval_InitThreads`` from Cython code instead of using
-    undocumented compiler macro.
+Project infrastructure:
 
-Examples:
-  * Moved `osc2midi` example into its own repository at
-    https://github.com/SpotlightKid/osc2rtmidi.git
+-   Added automatic documentation publishing on readthedocs.org.
 
-  * Add new ``sequencer`` example.
+Documentation:
 
-  * Add new ``noteon2osc`` example.
+-   Added auto docs for MidiIn/MidiOut classes to sphinx docs.
+-   Removed pre-release related information from installation docs.
 
-  * ``midifilter``:
+Building:
 
-    * Moved ``main.py`` to ``__main__.py``, removed old code and fixed command
-      line args access.
-    * Streamlined event matching.
-    * Added ``CCToBankChange`` filter.
-    * ``Queue`` module renamed to ``queue`` in Python 3.
-    * Fixed opening of output port erroneously used ``"input"``.
-    * Fixed positional command line args handling.
-    * Set command name for argparse.
+-   Added generated INSTALL.rst to repo to make ReadTheDocs integration work.
 
-  * ``midi2command``:
+Examples:
 
-    * Added README.
-    * Added command line option to select backend API.
-    * Catch errors when opening port.
-    * Set client and port name.
-    * Cache command lookup (Python 3.2+ only).
+-   Added new example script `panic.py`.
 
-  * ``sysexsaver``:
 
-    * Moved ``main.py`` to ``__main__.py``, some refactoring.
-    * ``models.py``: Fixed wrong entry for manufacturer ``(0, 32, 81)``.
-    * Moved module level code into ``main`` function.
-    * Include model name in output file, if possible.
+## 1.0.0rc1 (2016-10-09)
 
-  * ``drumseq``:
+Project infrastructure:
 
-    * Fixed global access in ``Sequencer`` class.
-    * Use ``args.FileType`` for pattern command line args.
+-   Moved repository to Github.
 
+Fixes:
 
-2014-06-11 version 0.5b1
-------------------------
+-   `midiutil.open_midiport`:
+    -   Correctly report and log I/O direction and instance type.
+    -   Fix naming of virtual port.
 
-Fixes:
-  * Synced RtMidi_ code with git repo @ 2c7a6664d6, which fixed several issues
-    (see https://github.com/thestk/rtmidi/issues?state=closed).
-  * ``MidiIn/Out.open_virtual_port`` returns ``self`` for context manager
-    support, consistent with ``MidiIn/Out.open_port``.
-  * Fix Python <= 2.6 incompatible encode method call (python-rtmidi
-    officially only supports Python >= 2.7). Thanks to Michiel Overtoom for
-    reporting this.
-  * Respect passed MIDI api when requesting MidiOut instance from
-    ``midiutil.open_midiport``.
+Enhancements / Changes:
 
-.. _rtmidi: https://github.com/thestk/rtmidi
+-   Synced with upstream [RtMidi] (2.1.1-399a8ee).
+-   `midiutil`:
+    -   The function `midiutil.open_port` has been renamed to
+        `open_midiport`.
+    -   Added convenience functions `open_midiinput` and
+        `open_midioutput`, which wrap `open_midiport`.
+    -   RtMidi API to use can be specified via the `RTMIDI_API`
+        environment variable. Only used when `API_UNSPECIFIED` is
+        passed for the `api` argument. Value should be one of the
+        `API_*` constant names with out the `API_` prefix, e.g.
+        `UNIX_JACK` for the Jack API.
+-   Cython wrapper class hierarchy restructured to better match the
+    underlying C++ classes and remove code duplication.
+-   Some source code re-ordering was done.
+
+Documentation:
+
+-   Added basic structure and initial content of Sphinx documentation.
+-   Documented exceptions raised by `MidiIn/Out.open_[virtual_]port()`.
+-   Some docstring corrections and formatting fixes.
+
+Building:
+
+-   Simplified `setup.py` by throwing out old compatibility stuff.
+-   Explicitly call `PyEval_InitThreads` from Cython code instead of
+    using undocumented compiler macro.
+
+Examples:
+
+-   Moved [osc2midi] example into its own repository.
+-   Add new `sequencer` example.
+-   Add new `noteon2osc` example.
+-   `midifilter`:
+    -   Moved `main.py` to `__main__.py`, removed old code and fixed
+        command line args access.
+    -   Streamlined event matching.
+    -   Added `CCToBankChange` filter.
+    -   `Queue` module renamed to `queue` in Python 3.
+    -   Fixed opening of output port erroneously used `"input"`.
+    -   Fixed positional command line args handling.
+    -   Set command name for argparse.
+-   `midi2command`:
+    -   Added README.
+    -   Added command line option to select backend API.
+    -   Catch errors when opening port.
+    -   Set client and port name.
+    -   Cache command lookup (Python 3.2+ only).
+-   `sysexsaver`:
+    -   Moved `main.py` to `__main__.py`, some refactoring.
+    -   `models.py`: Fixed wrong entry for manufacturer
+        `(0, 32, 81)`.
+    -   Moved module level code into `main` function.
+    -   Include model name in output file, if possible.
+-   `drumseq`:
+    -   Fixed global access in `Sequencer` class.
+    -   Use `args.FileType` for pattern command line args.
+
+[osc2midi]: https://github.com/SpotlightKid/osc2rtmidi.git
+
+
+## 0.5b1 (2014-06-11)
+
+Fixes:
+
+-   Synced [RtMidi] code with git repo @ 2c7a6664d6, which fixed
+    several issues (see
+    <https://github.com/thestk/rtmidi/issues?state=closed>).
+-   `MidiIn/Out.open_virtual_port` returns `self` for context
+    manager support, consistent with `MidiIn/Out.open_port`.
+-   Fix Python \<= 2.6 incompatible encode method call
+    (python-rtmidi officially only supports Python \>= 2.7). Thanks
+    to Michiel Overtoom for reporting this.
+-   Respect passed MIDI api when requesting MidiOut instance from
+    `midiutil.open_midiport`.
 
 Enhancements / Changes:
-  * Support for Windows Kernel Streaming API was removed in RtMidi (it was
-    broken anyway) and consequently in ``python-rtmidi`` as well.
-  * Raise ``RtMidiError`` exception when trying to open a (virtual) port on a
-    ``MidiIn/Out`` instance that already has an open (virtual) port.
-  * Add some common synonyms for MIDI events and controllers and some source
-    comments about controller usage to ``midiconstants`` module.
+
+-   Support for Windows Kernel Streaming API was removed in RtMidi
+    (it was broken anyway) and consequently in `python-rtmidi` as
+    well.
+-   Raise `RtMidiError` exception when trying to open a (virtual)
+    port on a `MidiIn/Out` instance that already has an open
+    (virtual) port.
+-   Add some common synonyms for MIDI events and controllers and
+    some source comments about controller usage to `midiconstants`
+    module.
 
 Documentation:
-  * Fix and clarify ``queue_size_limit`` default value in docstrings
-  * Various docstring consistency improvements and minor fixes.
+
+-   Fix and clarify `queue_size_limit` default value in docstrings
+-   Various docstring consistency improvements and minor fixes.
 
 Examples:
-  * New example script ``midi2command.py``, which executes external commands
-    on reception of configurable MIDI events, with example configuration.
-  * New example directory ``drumseq`` with a simple drum pattern sequencer
-    and example drum patterns. Thanks to Michiel Overtoom for the original
-    script!
 
+-   New example script `midi2command.py`, which executes external
+    commands on reception of configurable MIDI events, with example
+    configuration.
+-   New example directory `drumseq` with a simple drum pattern
+    sequencer and example drum patterns. Thanks to Michiel Overtoom
+    for the original script!
 
-2013-11-10 version 0.4.3b1
---------------------------
+
+## 0.4.3b1 (2013-11-10)
 
 Building:
-  * Add numeric suffix to version number to comply with PEP 440.
-  * Add missing ``fill_template.py`` to source distribution.
-  * Set default setuptools version in ``ez_setup.py`` to 1.3.2, which
+
+-   Add numeric suffix to version number to comply with PEP 440.
+-   Add missing `fill_template.py` to source distribution.
+-   Set default setuptools version in `ez_setup.py` to 1.3.2, which
     contains fix for bug #99 mentioned below.
 
 Documentation:
-  * Add note to installation guide about required ``--pre`` option with pip.
 
+-   Add note to installation guide about required `--pre` option with pip.
 
-2013-11-07 version 0.4.2b
--------------------------
+
+## 0.4.2b (2013-11-07)
 
 Fixes:
-  * Add missing ``API_*`` constant to list of exported names of ``_rtmidi``
-    module.
 
-Enhancements / Changes:
-  * Change default value of ``encoding`` argument of ``get_ports`` and
-    ``get_port_name`` methods to `"auto"`, which selects appropriate encoding
-    based on system and backend API used.
+-   Add missing `API_*` constant to list of exported names of
+    `_rtmidi` module.
 
-  * Add ``api`` parameter to ``midiutil.open_midiport`` function to select
-    backend API.
+Enhancements / Changes:
 
-  * Make client name for ``MidiOut`` and `` MidiIn`` different again,
+-   Change default value of `encoding` argument of `get_ports` and
+    `get_port_name` methods to [\"auto\"]{.title-ref}, which selects
+    appropriate encoding based on system and backend API used.
+-   Add `api` parameter to `midiutil.open_midiport` function to
+    select backend API.
+-   Make client name for `MidiOut` and `MidiIn` different again,
     because some backend APIs might require unique client names.
 
 Building:
-  * Include workaround for setuptools bug (see bitbucket issue #99) in
-    setup file.
-
-  * Add custom distutils command to fill placeholders in ``INSTALL.rst.in``
-    template with release meta data.
 
-  * Setuptools is now required, pure distutils won't work anymore, so removing
-    the fallback import of ``setup`` from distutils.
+-   Include workaround for setuptools bug (see bitbucket issue #99)
+    in setup file.
+-   Add custom distutils command to fill placeholders in
+    `INSTALL.rst.in` template with release meta data.
+-   Setuptools is now required, pure distutils won\'t work anymore,
+    so removing the fallback import of `setup` from distutils.
 
 
-2013-11-05 version 0.4.1b
--------------------------
+## 0.4.1b (2013-11-05)
 
 Building:
-  * Include missing ``_rtmidi.cpp`` file in source distribution.
+
+-   Include missing `_rtmidi.cpp` file in source distribution.
 
 Documentation:
-  * Fill in release data placeholders in ``INSTALL.rst``.
+
+-   Fill in release data placeholders in `INSTALL.rst`.
 
 
-2013-11-05 version 0.4b
------------------------
+## 0.4b (2013-11-05 )
 
 Fixes:
-  * Fix string conversion in constructors and ``open_*`` methods.
 
-  * Change default value ``queue_size_limit`` argument to ``MidiIn``
+-   Fix string conversion in constructors and `open_*` methods.
+-   Change default value `queue_size_limit` argument to `MidiIn`
     constructor to 1024.
-
-  * Update version number in ``RtMidi.cpp/h`` to reflect actual code state.
+-   Update version number in `RtMidi.cpp/h` to reflect actual code
+    state.
 
 Enhancements / Changes:
-  * Elevated development status to beta.
 
-  * Allow ``MidiIn/Out.open_port`` methods to be used with the ``with``
+-   Elevated development status to beta.
+-   Allow `MidiIn/Out.open_port` methods to be used with the `with`
     statement and the port will be closed at the end of the block.
-
-  * ``MidiIn``/``MidiOut`` and ``open*()`` methods: allow to specify ``None``
-    as client or port name to get the default names.
-
-  * Move ``midiconstants`` module from examples into ``rtmidi`` package
-    and added ``midiutil`` module.
-
-  * ``midiutils.open_midiport``:
-
-    * Allow to pass (substring of) port name as alternative to port number.
-    * Re-raise ``EOFError`` and ``KeyboardInterrupt`` instead of using
-      ``sys.exit()``.
-    * Add ``client_name`` and ``port_name`` arguments.
-    * Add ``use_virtual`` argument (default ``False``) to request opening
-      of a virtual MIDI port.
-    * Add ``interactive`` keyword argument (default ``True``) to disable
-      interactive prompt for port.
-
-  * Raise ``NotImplemented`` error when trying to open a virtual port with
-    Windows MultiMedia API.
-
-  * Change default name of virtual ports.
+-   `MidiIn`/`MidiOut` and `open*()` methods: allow to specify
+    `None` as client or port name to get the default names.
+-   Move `midiconstants` module from examples into `rtmidi` package
+    and added `midiutil` module.
+-   `midiutils.open_midiport`:
+    -   Allow to pass (substring of) port name as alternative to
+        port number.
+    -   Re-raise `EOFError` and `KeyboardInterrupt` instead of using
+        `sys.exit()`.
+    -   Add `client_name` and `port_name` arguments.
+    -   Add `use_virtual` argument (default `False`) to request
+        opening of a virtual MIDI port.
+    -   Add `interactive` keyword argument (default `True`) to
+        disable interactive prompt for port.
+-   Raise `NotImplemented` error when trying to open a virtual port
+    with Windows MultiMedia API.
+-   Change default name of virtual ports.
 
 Documentation:
-  * Re-organize package description and installation instructions into several
-    files and add separate text files with changelog and license information.
 
-  * Add detailed instructions for compiling from source on Windows
+-   Re-organize package description and installation instructions
+    into several files and add separate text files with changelog
+    and license information.
+-   Add detailed instructions for compiling from source on Windows
+-   Add docstrings to all methods and functions in `_rtmidi` module.
+-   Add docstring for `midiutils.open_midiport` function.
 
-  * Add docstrings to all methods and functions in ``_rtmidi`` module.
-
-  * Add docstring for ``midiutils.open_midiport`` function.
+Examples:
 
+-   Add new example package `osc2midi`, a simple, uni-directional
+    OSC to MIDI mapper.
+-   New example script `sendsysex.py` to demonstrate sending of MIDI
+    system exclusive messages.
+-   New example script `wavetablemodstep.py` to demonstrate sending
+    of MIDI control change messages.
+-   New `sysexsaver` example.
+-   Convert `midifilter` example script into a package.
+-   Upgrade from `optparse` to `argparse` in example scripts.
+-   Enable logging in test scripts.
 
-Examples:
-  * Add new example package ``osc2midi``, a simple, uni-directional OSC to MIDI
-    mapper.
+Building:
 
-  * New example script ``sendsysex.py`` to demonstrate sending of MIDI system
-    exclusive messages.
+-   Switch from `distribute` back to `setuptools`.
+-   Include `ez_setup.py` in source distribution.
+-   Include examples in source distribution.
+-   Install `osc2midi` example as package and command line script.
+-   Enable C++ exceptions on Windows build.
 
-  * New example script ``wavetablemodstep.py`` to demonstrate sending of
-    MIDI control change messages.
 
-  * New ``sysexsaver`` example.
+## 0.3.1a (2013-01-23)
 
-  * Convert ``midifilter`` example script into a package.
+Enhancements:
 
-  * Upgrade  from ``optparse`` to ``argparse`` in example scripts.
+-   Increase sysex input buffer size for WinMM API again to 8192
+    (8k) bytes. Requested by Martin Tarenskeen.
 
-  * Enable logging in test scripts.
 
+## 0.3a (2013-01-14)
 
-Building:
-  * Switch from ``distribute`` back to ``setuptools``.
+Bug fixes:
 
-  * Include ``ez_setup.py`` in source distribution.
+-   Add `encoding` parameter to `get_port_name` methods of `MidiIn`
+    and `MidiOut` to be able to handle non-UTF-8 port names, e.g. on
+    Windows (reported by Pierre Castellotti).
+-   Add `encoding` parameter to `get_ports` method as well and pass
+    it through to `get_port_name`. Use it in the test scripts.
 
-  * Include examples in source distribution.
+Enhancements:
 
-  * Install ``osc2midi`` example as package and command line script.
+-   Increase sysex input buffer size for WinMM API to 4096 bytes.
 
-  * Enable C++ exceptions on Windows build.
+Examples:
 
+-   Add new `midifilter.py` example script.
 
-2013-01-23 version 0.3.1a
--------------------------
+Building:
 
-Enhancements:
-    * Increase sysex input buffer size for WinMM API again to 8192 (8k) bytes.
-      Requested by Martin Tarenskeen.
+-   Add `setuptools`/`distribute` support.
 
 
-2013-01-14 version 0.3a
------------------------
+## 0.2a (2012-07-22)
 
 Bug fixes:
-    * Add ``encoding`` parameter to ``get_port_name`` methods of ``MidiIn``
-      and ``MidiOut`` to be able to handle non-UTF-8 port names, e.g. on
-      Windows (reported by Pierre Castellotti).
-    * Add ``encoding`` parameter to ``get_ports`` method as well and pass it
-      through to ``get_port_name``. Use it in the test scripts.
+
+-   Fix uninitialized pointer bug in `RtMidi.cpp` in \'MidiOutJack\'
+    class, which caused a warning in the jack process callback when
+    creating a `MidiOut` instance with the JACK API.
+-   `testmidiin_*.py`: fix superfluous decoding of port name (caused
+    error with Python 3).
 
 Enhancements:
-    * Increase sysex input buffer size for WinMM API to 4096 bytes.
 
-Examples:
-    * Add new ``midifilter.py`` example script.
+-   Simplify some code, some things gleaned from rtmidi_python.
+-   Documentation typo fixes and more information on Windows
+    compilation.
+-   Enhancements in test scripts:
+    -   `test_probe_ports.py`: Catch exceptions when creating port.
+    -   `test_midiin_*.py`:
+        -   Better error message for missing/invalid port number.
+        -   Show how to convert event delta time into absolute time
+            when receiving input.
 
 Building:
-    * Add ``setuptools``/``distribute`` support.
-
-
-2012-07-22 version 0.2a
------------------------
 
-Bug fixes:
-    * Fix uninitialized pointer bug in ``RtMidi.cpp`` in 'MidiOutJack' class,
-      which caused a warning in the jack process callback when creating a
-      ``MidiOut`` instance with the JACK API.
-    * ``testmidiin_*.py``: fix superfluous decoding of port name (caused error
-      with Python 3).
-
-Enhancements:
-    * Simplify some code, some things gleaned from rtmidi_python.
-    * Documentation typo fixes and more information on Windows compilation.
-    * Enhancements in test scripts:
-
-      * ``test_probe_ports.py``: Catch exceptions when creating port.
-      * ``test_midiin_*.py``:
-
-        * Better error message for missing/invalid port number.
-        * Show how to convert event delta time into absolute time when
-          receiving input.
-
-Building:
-    * Building on OS X 10.6.9 with CoreMIDI and JACK for OS X successfully
-      tested and test run without errors.
-    * WinMM support now compiles with Visual Studio 2008 Express and tests
-      work under Windows XP SP3 32-bit.
-    * Add command line option to exclude WinMM or WinKS API from compilation.
-    * Add missing ``extra_compile_args`` to Extension kwargs in setup file.
-    * Add ``library_dirs`` to Extension kwargs in setup file.
-    * Use ``-frtti`` compiler option on OS X (neccessary on 10.7?).
-    * Fix file name conflict on case-insensitive file systems by prefixing
-      ``rtmidi.{pyx,cpp}`` with an underscore
-    * Provide correct compiler flags for compiling with Windows MultiMedia API.
-    * Adapt windows library and include path for Visual Studio 2008 Express.
-    * add support for compiling with Windows Kernel Streaming API (does not
-      not compile due to syntax errors in RtMidi.cpp yet).
+-   Building on OS X 10.6.9 with CoreMIDI and JACK for OS X
+    successfully tested and test run without errors.
+-   WinMM support now compiles with Visual Studio 2008 Express and
+    tests work under Windows XP SP3 32-bit.
+-   Add command line option to exclude WinMM or WinKS API from
+    compilation.
+-   Add missing `extra_compile_args` to Extension kwargs in setup
+    file.
+-   Add `library_dirs` to Extension kwargs in setup file.
+-   Use `-frtti` compiler option on OS X (neccessary on 10.7?).
+-   Fix file name conflict on case-insensitive file systems by
+    prefixing `rtmidi.{pyx,cpp}` with an underscore
+-   Provide correct compiler flags for compiling with Windows
+    MultiMedia API.
+-   Adapt windows library and include path for Visual Studio 2008
+    Express.
+-   add support for compiling with Windows Kernel Streaming API
+    (does not not compile due to syntax errors in RtMidi.cpp yet).
 
 
-2012-07-13 version 0.1a
------------------------
+## 0.1a (2012-07-13)
 
 First public release.
```

### Comparing `python-rtmidi-1.4.9/INSTALL-windows.rst` & `python-rtmidi-1.5.0/INSTALL-windows.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,123 +1,131 @@
-How to install python-rtmidi from source on Windows
-===================================================
+# How to install python-rtmidi from source on Windows
 
-These instruction should work for installing ``python-rtmidi`` from source
-Python 3.x in the 64-bit or 32-bit vsersions (you can run the latter on
-Windows 64-bit versions with no problems).
+These instructions should work for installing `python-rtmidi` from source with
+Python 3.7+ in the 64-bit or 32-bit versions (you can run the latter on Windows
+64-bit versions with no problems).
 
 Please follow all the steps below in the exact order.
 
-
-Installing required software
-----------------------------
+## Installing required software
 
 You probably need administrator rights for some or all of the following steps.
 
-#. Install the latest release of Python 3.6+ from
-   https://www.python.org/downloads/windows/ to the default location (e.g.
-   ``C:\Python36``). You can install either or both the 32-bit and the 64-bit
-   version.
-
-   In the installer, enable the option to install pip_. Optionally, *for only
-   one of the chosen Python versions*, enable the options to add the
-   installation directory to your ``PATH`` and set it as the system's default
-   version. Also enable the option to install the ``py`` helper script (only
-   available with some Python versions).
+1.  Install the latest release of Python (3.11 at the time of writing, at least
+    3.7+) from <https://www.python.org/downloads/windows/> to the default
+    location (e.g. `C:\Python311`). You can install either or both the 32-bit
+    and the 64-bit version.
 
-#. Install virtualenv_ from a command prompt::
+    In the installer, enable the option to install [pip]. Optionally, *for only
+    one of the chosen Python versions*, enable the options to add the
+    installation directory to your `PATH` and set it as the system's default
+    version. Also enable the option to install the `py` helper script (only
+    available with some Python versions).
 
-        > python -m pip install -U virtualenv
+2.  Install [virtualenv] from a command prompt:
 
-   Repeat this for all Python versions you have installed (run ``py --help``
-   to get help on how to run different python version from the command line).
+    ```console
+    python -m pip install -U virtualenv
+    ```
 
-#. Go to https://wiki.python.org/moin/WindowsCompilers and follow the
-   instructions there to select and install the correct version(s) of the
-   Visual C++ compiler for the version(s) of Python you installed.
+    Repeat this for all Python versions you have installed (run `py --help` to
+    get help on how to run different python version from the command line).
 
-   You can install several versions of Visual C++ at the same time.
+3.  Go to <https://wiki.python.org/moin/WindowsCompilers> and follow the
+    instructions there to select and install the correct version(s) of
+    the Visual C++ compiler for the version(s) of Python you installed.
 
-   After installation, use Windows Update to get any pending security updates
-   and fixes.
+    You can install several versions of Visual C++ at the same time.
 
+    After installation, use Windows Update to get any pending security updates
+    and fixes.
 
-Setting up a virtual environment
---------------------------------
 
-#. Open a command line and run::
+## Setting up a virtual environment
 
-        > python -m virtualenv rtmidi
-        > rtmidi\Scripts\activate
+1.  Open a command line and run:
 
-#. Update pip and setuptools_ within your virtual environment to the latest
-   versions with::
+    ```console
+    python -m virtualenv rtmidi
+    rtmidi\Scripts\activate
+    ```
 
-        (rtmidi)> pip install -U pip setuptools
+2.  Update pip within your virtual environment to the latest version with:
 
-#. Install Cython (still in the same command line window)::
+    ```console
+    (rtmidi)> pip install -U pip
+    ```
 
-        (rtmidi)> pip install Cython
+3.  Install build dependencies (still in the same command line window):
 
+    ```console
+    (rtmidi)> pip install build installer
+    ```
 
-Download & unpack python-rtmidi source
---------------------------------------
+## Download & unpack python-rtmidi source
 
 Get the latest python-rtmidi distribution as a Zip archive from
-https://pypi.python.org/pypi/python-rtmidi and unpack it somewhere.
-You can do the downloading and unpacking in one step using pip::
+<https://pypi.python.org/pypi/python-rtmidi> and unpack it somewhere. You can
+do the downloading and unpacking in one step using pip:
 
-    > pip install --no-install -d . "python-rtmidi"
+```console
+pip install --no-install -d . "python-rtmidi"
+```
 
-Alternatively, clone the python-rtmidi git repository::
+Alternatively, clone the python-rtmidi git repository:
 
-    > git clone https://github.com/SpotlightKid/python-rtmidi.git
+```console
+git clone https://github.com/SpotlightKid/python-rtmidi.git
+```
 
-In the command line window you opened above, change into the ``python-rtmidi``
-directory, which you created by unpacking the source or cloning the
-repository::
+In the command line window you opened above, change into the `python-rtmidi`
+directory, which you created by unpacking the source or cloning the repository:
 
-    (rtmidi)> cd python-rtmidi
 
+```console
+(rtmidi)> cd python-rtmidi
+```
 
-Build & install python-rtmidi
------------------------------
-
-Just run the usual setup command from within the source directory with the
-active virtual environment, i.e. from still the same command line window::
 
-    (rtmidi)> python setup.py install
+## Build & install python-rtmidi
 
+Just run the usual setup command from within the source directory with the
+active virtual environment, i.e. from still the same command line window:
 
-Verify your installation
-------------------------
-
-Change out of the ``python-rtmidi`` source directory (important!) and run::
-
-    (rtmidi)> cd ..
-    (rtmidi)> python
-    >>> import rtmidi
-    >>> rtmidi.API_WINDOWS_MM in rtmidi.get_compiled_api()
-    True
-    >>> midiout = rtmidi.MidiOut()
-    >>> midiout.get_ports()
-    ['Microsoft GS Wavetable Synth']
+```console
+(rtmidi)> python -m build
+(rtmidi)> python -m installer dist/*.whl
+```
+
+
+## Verify your installation
+
+Change out of the `python-rtmidi` source directory (important!) and run:
+
+```console
+(rtmidi)> cd ..
+(rtmidi)> python
+>>> import rtmidi
+>>> rtmidi.API_WINDOWS_MM in rtmidi.get_compiled_api()
+True
+>>> midiout = rtmidi.MidiOut()
+>>> midiout.get_ports()
+['Microsoft GS Wavetable Synth']
+```
 
 If you have any other MIDI outputs (hardware MIDI interfaces, MIDI Yoke etc.)
-active, they should be listed by ``get_ports()`` as well.
+active, they should be listed by `get_ports()` as well.
 
 *That's it, congratulations!*
 
 
-Notes
------
+## Notes
 
-Windows Kernel Streaming support in RtMidi has been removed (it was broken
-anyway) and consequently in ``python-rtmidi`` as well.
+Windows Kernel Streaming support in RtMidi has been removed (it was
+broken anyway) and consequently in `python-rtmidi` as well.
 
-Compiling with MinGW also does not work out-of-the-box yet. If you have any
-useful hints, please let the author know.
+Compiling with MinGW also does not work out-of-the-box yet. If you have
+any useful hints, please let the author know.
 
 
-.. _pip: https://pypi.python.org/pypi/pip
-.. _setuptools: https://pypi.python.org/pypi/setuptools
-.. _virtualenv: https://pypi.python.org/pypi/virtualenv
+[pip]: https://pypi.python.org/pypi/pip
+[virtualenv]: https://pypi.python.org/pypi/virtualenv
```

### Comparing `python-rtmidi-1.4.9/INSTALL.rst` & `python-rtmidi-1.5.0/INSTALL.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,236 +1,224 @@
-============
-Installation
-============
-
-**python-rtmidi** uses the de-facto standard Python distutils and setuptools_
-based packaging system and can be installed from the Python Package Index via
-pip_. Since it is a Python C(++)-extension, a C++ compiler and build
+# Installation
+
+**python-rtmidi** uses a modern [PEP 517] compliant Python build system based
+on [meson] and [mesonpep517] and can be installed from the Python Package Index
+via [pip]. Since it is a Python C(++)-extension, a C++ compiler and build
 environment as well as some system-dependent libraries are needed to install,
 unless wheel packages with pre-compiled binaries are available for your system.
-See the Requirements_ section below for details.
+See the [Requirements] section below for details.
 
 
-From PyPI
----------
+## From PyPI
 
-If you have all the requirements_, you should be able to install the package
-with pip_::
+If you have all the [requirements], you should be able to install the package
+with [pip]:
 
     $ pip install python-rtmidi
 
-This will download the source distribution from python-rtmidi's `PyPI page`_,
-compile the extension (if no pre-compiled binary wheel is available) and
-install it in your active Python installation. Unless you want to change the
-Cython_ source file ``_rtmidi.pyx``, there is no need to have Cython installed.
-
-.. note::
-    On some Linux distributions, e.g. *Debian*, which support both Python 2 and
-    Python 3, pip may installed under the name ``pip2`` resp. ``pip3``. In this
-    case, just ``pip2`` instead of ``pip`` if you're still using Python 2 (not
-    officially supported), or ``pip3`` if you are using Python 3.
+This will download a pre-compiled binary wheel from python-rtmidi's
+[PyPI page], if available, and install it in your active Python installation.
+If no fitting binary wheel is available, it will download the source
+distribution, compile the extension (downloading all the build tools needed in
+the process) and install it.
+
+**Note:**
 
-python-rtmidi also works well with virtualenv_ and virtualenvwrapper_. If you
+*On some Linux distributions pip may installed under the name `pip3`. In
+this case, just substitute `pip3` for `pip`.*
+
+python-rtmidi also works well with [virtualenv] and [virtualenvwrapper]. If you
 have both installed, creating an isolated environment for testing and/or using
-python-rtmidi is as easy as::
+python-rtmidi is as easy as:
 
     $ mkvirtualenv rtmidi
     (rtmidi)$ pip install python-rtmidi
 
-If you want to pass options to the build process, use pip's ``install-option``
-option. See the `From Source`_  section below for available options.
+If you want to pass options to the build process, you need to compile
+python-rtmidi from source manually. See the [From Source](#from-source) section
+below for moe information.
 
 
-Pre-compiled Binaries
----------------------
+## Pre-compiled Binaries
 
 Pre-compiled binary wheels of the latest python-rtmidi version for Windows and
 macOS / OS X are available on PyPI for several major Python versions. If you
 install python-rtmidi via pip (see above), these wheels will be selected by pip
 automatically, if you have a compatible Python and Windows or macOS version.
 
 The Windows binary wheels are compiled with Windows MultiMedia API support and
 are available in 32-bit and 64-bit versions. The macOS / OS X binary wheels are
-compiled with CoreMIDI support and are only available in 64-bit versions for
-OS X 10.6 and later. If you need JACK support on OS X, you need to compile
-python-rtmidi yourself (see the macOS_ section below for details).
+compiled with CoreMIDI support and are only available in 64-bit versions for OS
+X 10.6 and later. If you need JACK support on OS X, you need to compile
+python-rtmidi yourself (see the [macOS] section below for details).
 
 
-From Source
------------
+## From Source
 
 To compile python-rtmidi from source and install it manually without pip, you
 can either download a source distribution archive or check out the sources from
 the Git repository.
 
-While the steps to get the sources differ, the actual compilation step consists
-only of the usual ``python setup.py install`` command in both cases.
+While the steps to get the sources differ, the actual compilation and
+installation steps consist of the same standard meson commands in both cases:
 
-``setup.py`` recognizes several options to control which OS-dependent MIDI
-backends will be supported by the python-rtmidi extension binary it produces
-plus other options to control compilation of the RtMidi C++ library:
-
-+-----------------------------+-----------+---------------+-----------+----------------------------------------------------------+
-| Option                      | Linux     | mac OS / OS X | Windows   |  Note                                                    |
-+=============================+===========+===============+===========+==========================================================+
-| ``--no-alsa``               | supported |               |           | Don't compile in support for ALSA backend.               |
-+-----------------------------+-----------+---------------+-----------+----------------------------------------------------------+
-| ``--no-jack``               | supported | supported     |           | Don't compile in support for JACK backend.               |
-+-----------------------------+-----------+---------------+-----------+----------------------------------------------------------+
-| ``--no-coremidi``           |           | supported     |           | Don't compile in support for CoreMIDI backend.           |
-+-----------------------------+-----------+---------------+-----------+----------------------------------------------------------+
-| ``--no-winmm``              |           |               | supported | Don't compile in support for Windows MultiMedia backend. |
-+-----------------------------+-----------+---------------+-----------+----------------------------------------------------------+
-| ``--no-suppress-warnings``  |           |               |           | Don't suppress RtMidi warnings to stderr.                |
-+-----------------------------+-----------+---------------+-----------+----------------------------------------------------------+
+```console
+meson setup --prefix=/usr --buildtype=plain builddir
+meson compile -C builddir
+meson install -C builddir
+```
+
+The `meson setup` command recognizes several options to control which
+OS-dependent MIDI backends will be supported by the python-rtmidi extension
+binary it produces, plus other options to control compilation of the RtMidi C++
+library:
+
+|  Option            | Linux | macOS | Windows | Note                                                     |
+| ------------------ | ----- | ----- | ------- | -------------------------------------------------------- |
+| `-Dalsa=false`     | x     | n/a   | n/a     | Don't compile in support for ALSA backend.               |
+| `-Djack=false`     | x     | x     | n/a     | Don't compile in support for JACK backend.               |
+| `-Dcoremidi=false` | n/a   | x     | n/a     | Don't compile in support for CoreMIDI backend.           |
+| `-Dwinmm=false`    | n/a   | n/a   | x       | Don't compile in support for Windows MultiMedia backend. |
+| `-Dverbose=true`   | x     | x     | x       | Don't suppress RtMidi warnings to stderr.                |
 
 Support for each OS dependent MIDI backend is only enabled when the required
-library and header files are actually present on the system. When the options
-passed to ``setup.py`` change, it may be necessary to remove previously built
-files by deleting the ``build`` directory.
-
-You can also pass these options to ``setup.py`` when using pip, by using its
-``--install-option`` option, for example::
+library and header files are actually present on the system.
 
-    pip install python-rtmidi --install-option="--no-jack"
 
-
-From the Source Distribution
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### From the Source Distribution
 
 To download the python-rtmidi source distribution archive for the current
-version, extract and install it, use the following commands::
+version, extract and install it, use the following commands:
 
-    $ pip download python-rtmidi
-    $ tar -xzf python-rtmidi-1.4.9.tar.gz
-    $ cd python-rtmidi-1.4.9
-    $ python setup.py install
+```console
+pip download python-rtmidi
+tar -xzf python-rtmidi-1.X.Y.tar.gz
+cd python-rtmidi-1.X.Y
+meson setup --prefix=/usr --buildtype=plain builddir
+meson compile -C builddir
+meson install -C builddir
+```
 
 On Linux or macOS / OS X, if you want to install python-rtmidi into the
-system-wide Python library directory, you may have to prefix the last
-command with ``sudo``, e.g.::
+system-wide Python library directory, you may have to prefix the last command
+with `sudo`, e.g.:
 
-    $ sudo python setup.py install
+```console
+sudo meson install -C builddir
+```
 
 The recommended way, though, is to install python-rtmidi only for your current
-user (which pip does by default) or into a virtual environment::
+user (which `installer` does by default) or into a virtual environment:
 
-    $ python setup.py install --user
+```console
+python -m installer dist/*.whl
+```
 
 
-From the Source Code Repository
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+### From the Source Code Repository
 
 Alternatively, you can check out the python-rtmidi source code from the Git
 repository and then install it from your working copy. Since the repository
 does not include the C++ module source code pre-compiled from the Cython
 source, you'll also need to install Cython >= 0.28, either via pip or from its
-Git repository. Using virtualenv / virtualenvwrapper is strongly recommended
-in this scenario:
-
-Make a virtual environment::
-
-    $ mkvirtualenv rtmidi
-    (rtmidi)$ cdvirtualenv
+Git repository. Using virtualenv / virtualenvwrapper is strongly recommended in
+this scenario:
 
-Install Cython from PyPI::
+Make a virtual environment:
 
-    (rtmidi)$ pip install Cython
+```console
+mkvirtualenv rtmidi
+(rtmidi)$ cdvirtualenv
+```
+
+Install Cython from PyPI:
+
+```console
+(rtmidi)$ pip install Cython meson ninja wheel
+```
+
+Then install python-rtmidi:
+
+```console
+(rtmidi)$ git clone --recursive https://github.com/SpotlightKid/python-rtmidi.git
+(rtmidi)$ cd python-rtmidi
+(rtmidi)$ meson setup --prefix=/usr --buildtype=plain builddir
+(rtmidi)$ meson compile -C builddir
+(rtmidi)$ meson install -C builddir
+```
 
-*or* from its Git repository::
-
-    (rtmidi)$ git clone https://github.com/cython/cython.git
-    (rtmidi)$ cd cython
-    (rtmidi)$ python setup.py install
-    (rtmidi)$ cd ..
-
-Then install python-rtmidi::
-
-    (rtmidi)$ git clone https://github.com/SpotlightKid/python-rtmidi.git
-    (rtmidi)$ cd python-rtmidi
-    (rtmidi)$ git submodule update --init
-    (rtmidi)$ python setup.py install
-
-
-.. _requirements:
-
-Requirements
-============
+(requirements)=
+#### Requirements
 
 Naturally, you'll need a C++ compiler and a build environment. See the
 platform-specific hints below.
 
-If you want to change the Cython source file ``_rtmidi.pyx`` or want to
-recompile ``_rtmidi.cpp`` with a newer Cython version, you'll need to install
-Cython >= 0.28. The ``_rtmidi.cpp`` file in the current source distribution
-(version 1.4.9) is tagged with::
-
-    /* Generated by Cython 0.29.23 */
+If you want to change the Cython source file `_rtmidi.pyx` or want to recompile
+`_rtmidi.cpp` with a newer Cython version, you'll need to install Cython.
 
 RtMidi (and therefore python-rtmidi) supports several low-level MIDI frameworks
 on different operating systems. Only one of the available options needs to be
 present on the target system, but support for more than one can be compiled in.
-The setup script will try to detect available libraries and should use the
+The `meson.build` script will detect available libraries and should use the
 appropriate compilations flags automatically.
 
-    * Linux: ALSA, JACK
-    * macOS (OS X): CoreMIDI, JACK
-    * Windows: MultiMedia (MM)
+-   Linux: ALSA, JACK
+-   macOS (OS X): CoreMIDI, JACK
+-   Windows: MultiMedia (MM)
 
 
-Linux
------
+## Linux
 
 First you need a C++ compiler and the pthread library. Install the
-``build-essential`` package on debian-based systems to get these.
+`build-essential` package on debian-based systems to get these.
 
 Then you'll need Python development headers and libraries. On debian-based
-systems, install the ``python-dev`` package. If you use the official installers
+systems, install the `python-dev` package. If you use the official installers
 from python.org you should already have these.
 
-To get ALSA support, you must install development files for the ``libasound2``
-library (debian package: ``libasound2-dev``). For JACK support, install the
-``libjack`` development files (if you are using Jack1, install ``libjack-dev``,
-if you are using Jack2, install ``libjack-jackd2-dev``).
+To get ALSA support, you must install development files for the `libasound2`
+library (debian package: `libasound2-dev`). For JACK support, install the
+`libjack` development files (if you are using Jack1, install `libjack-dev`, if
+you are using Jack2, install `libjack-jackd2-dev`).
 
 
-.. _macos:
+(macos)=
+## macOS (OS X)
 
-macOS (OS X)
-------------
+Install the latest Xcode version or `g++` from MacPorts or homebrew (untested).
+CoreMIDI support comes with installing Xcode. For JACK support, install
+[JackOSX] with the installer or build JACK from source.
 
-Install the latest Xcode version or ``g++`` from MacPorts or homebrew
-(untested). CoreMIDI support comes with installing Xcode. For JACK support,
-install `JackOSX`_ with the installer or build JACK from source.
+**Note:**
 
-.. note::
-    If you have an old version of OS X and Xcode which still support building
-    binaries for PPC, you'll have to tell distribute to build the package only
-    for i386 and x86_64 architectures::
+*If you have a very old version of OS X and Xcode which still supports building
+binaries for PPC, you'll have to tell distribute to build the package only for
+i386 and x86_64 architectures:*
 
-        env ARCHFLAGS="-arch i386 -arch x86_64" python setup.py install
+```console
+env ARCHFLAGS=\"-arch i386 -arch x86_64\" python setup.py install
+```
 
 
-Windows
--------
+## Windows
 
-Please see the detailed instructions for Windows in :doc:`install-windows`.
+Please see the detailed instructions for Windows in `install-windows`.
 
 
-User Contributed Documentation
-------------------------------
+## User Contributed Documentation
 
-The python-rtmidi wiki on GitHub contains some `user contributed
-documentation`_ for additional installation scenarios. Please check these, if
-you have trouble installing python-rtmidi in an uncommon or not-yet-covered
-environment.
+The python-rtmidi wiki on GitHub contains some [user contributed documentation]
+for additional installation scenarios. Please check these, if you have trouble
+installing python-rtmidi in an uncommon or not-yet-covered environment.
 
 
-.. _pypi page: http://python.org/pypi/python-rtmidi#downloads
-.. _cython: http://cython.org/
-.. _pip: http://python.org/pypi/pip
-.. _setuptools: http://python.org/pypi/setuptools
-.. _virtualenv: http://pypi.python.org/pypi/virtualenv
-.. _virtualenvwrapper: http://www.doughellmann.com/projects/virtualenvwrapper/
-.. _jackosx: http://jackaudio.org/downloads/
-.. _user contributed documentation:
-    https://github.com/SpotlightKid/python-rtmidi/wiki/User-contributed-documentation
+[Cython]: http://cython.org/
+[JackOSX]: http://jackaudio.org/downloads/
+[meson]: https://mesonbuild.com/
+[mesonpep517]: https://thiblahute.gitlab.io/mesonpep517/
+[pep 517]: https://peps.python.org/pep-0517/
+[pip]: https://pypi.python.org/pypi/pip
+[PyPI page]: http://python.org/pypi/python-rtmidi#downloads
+[setuptools]: https://pypi.python.org/pypi/setuptools
+[user contributed documentation]: https://github.com/SpotlightKid/python-rtmidi/wiki/User-contributed-documentation
+[virtualenv]: https://pypi.python.org/pypi/virtualenv
+[virtualenvwrapper]: http://www.doughellmann.com/projects/virtualenvwrapper/
```

### Comparing `python-rtmidi-1.4.9/LICENSE.txt` & `python-rtmidi-1.5.0/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Copyright & License
 ===================
 
 python-rtmidi was written by Christopher Arndt, 2012 - 2021.
 
 The software is released unter the MIT License:
 
-Copyright (c) 2012 - 2021 Christopher Arndt
+Copyright (c) 2012 - 2022 Christopher Arndt
 
     Permission is hereby granted, free of charge, to any person obtaining a
     copy of this software and associated documentation files (the "Software"),
     to deal in the Software without restriction, including without limitation
     the rights to use, copy, modify, merge, publish, distribute, sublicense,
     and/or sell copies of the Software, and to permit persons to whom the
     Software is furnished to do so, subject to the following conditions:
```

### Comparing `python-rtmidi-1.4.9/docs/Makefile` & `python-rtmidi-1.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/docs/api.rst.inc` & `python-rtmidi-1.5.0/docs/api.rst.inc`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/docs/conf.py` & `python-rtmidi-1.5.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import configparser
 import sys
 import os
 
 # If extensions (or modules to document with autodoc) are in another
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
@@ -30,43 +29,42 @@
 # Insert the project root dir as the first element in the PYTHONPATH.
 # This lets us ensure that the source package is imported, and that its
 # version is used.
 sys.path.insert(0, project_root)
 
 
 meta = {}
-setupcfg = configparser.ConfigParser()
-setupcfg.read(os.path.join(project_root, 'setup.cfg'))
 version = os.path.join(project_root, 'rtmidi', 'version.py')
 exec(compile(open(version).read(), version, 'exec'), {}, meta)
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = ['myst_parser', 'sphinx.ext.autodoc', 'sphinx.ext.viewcode']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
-source_suffix = '.rst'
+source_suffix = ['.md', '.rst']
 
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = setupcfg['metadata']['name']
-copyright = u'2012 - 2021, %s' % setupcfg['metadata']['author']
+project = 'python-rtmidi'
+author = 'Christopher Arndt'
+copyright = f'2012 - 2022, {author}'
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = meta['version']
@@ -192,14 +190,15 @@
 
 # This is the file name suffix for HTML files (e.g. ".xhtml").
 #html_file_suffix = None
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'rtmididoc'
 
+myst_heading_anchors = 3
 
 # -- Options for LaTeX output ------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #'papersize': 'letterpaper',
 
@@ -211,16 +210,16 @@
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto/manual]).
 latex_documents = [
     ('index', 'rtmidi.tex',
-     u'python-rtmidi Documentation',
-     setupcfg['metadata']['author'], 'manual'),
+     'python-rtmidi Documentation',
+     author, 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at
 # the top of the title page.
 #latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings
@@ -242,33 +241,33 @@
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
     ('index', 'rtmidi',
-     u'python-rtmidi Documentation',
-     [setupcfg['metadata']['author']], 1)
+     f'{project} Documentation',
+     author, 1)
 ]
 
 # If true, show URL addresses after external links.
 #man_show_urls = False
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     ('index', 'rtmidi',
-     u'python-rtmidi Documentation',
-     setupcfg['metadata']['author'],
-     setupcfg['metadata']['name'],
-     setupcfg['metadata']['description'],
+     f'{project} Documentation',
+     author,
+     project,
+     '',
      'Miscellaneous'),
 ]
 
 # Documents to append as an appendix to all manuals.
 #texinfo_appendices = []
 
 # If false, no module index is generated.
```

### Comparing `python-rtmidi-1.4.9/docs/contributing.rst` & `python-rtmidi-1.5.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/docs/make.bat` & `python-rtmidi-1.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/docs/rtmidi.rst` & `python-rtmidi-1.5.0/docs/rtmidi.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/docs/usage.rst` & `python-rtmidi-1.5.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/advanced/ccstore.py` & `python-rtmidi-1.5.0/examples/advanced/ccstore.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/advanced/midiclock.py` & `python-rtmidi-1.5.0/examples/advanced/midiclock.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/advanced/midioutwrapper.py` & `python-rtmidi-1.5.0/examples/advanced/midioutwrapper.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/advanced/recvrpn.py` & `python-rtmidi-1.5.0/examples/advanced/recvrpn.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/basic/contextmanager.py` & `python-rtmidi-1.5.0/examples/basic/contextmanager.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/basic/midiin_callback.py` & `python-rtmidi-1.5.0/examples/basic/midiin_callback.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/basic/midiin_poll.py` & `python-rtmidi-1.5.0/examples/basic/midiin_poll.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/basic/midiout.py` & `python-rtmidi-1.5.0/examples/basic/midiout.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/basic/noteon2osc.py` & `python-rtmidi-1.5.0/examples/basic/noteon2osc.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/basic/panic.py` & `python-rtmidi-1.5.0/examples/basic/panic.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 print(__doc__)
 
 for portnum, portname in enumerate(midiout.get_ports()):
     print("Port:", portname)
 
     with midiout.open_port(portnum):
         for channel in range(16):
-            midiout.send_message([CONTROL_CHANGE, ALL_SOUND_OFF, 0])
-            midiout.send_message([CONTROL_CHANGE, RESET_ALL_CONTROLLERS, 0])
+            midiout.send_message([CONTROL_CHANGE | channel, ALL_SOUND_OFF, 0])
+            midiout.send_message([CONTROL_CHANGE | channel, RESET_ALL_CONTROLLERS, 0])
             time.sleep(0.05)
 
         time.sleep(0.1)
```

### Comparing `python-rtmidi-1.4.9/examples/basic/probe_ports.py` & `python-rtmidi-1.5.0/examples/basic/probe_ports.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/drumseq/README.rst` & `python-rtmidi-1.5.0/examples/drumseq/README.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/drumseq/drumseq.py` & `python-rtmidi-1.5.0/examples/drumseq/drumseq.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/midi2command/000-playback.mp3` & `python-rtmidi-1.5.0/examples/midi2command/000-playback.mp3`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/midi2command/000-sheet.pdf` & `python-rtmidi-1.5.0/examples/midi2command/000-sheet.pdf`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/midi2command/README.rst` & `python-rtmidi-1.5.0/examples/midi2command/README.rst`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/midi2command/example.cfg` & `python-rtmidi-1.5.0/examples/midi2command/example.cfg`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/midi2command/midi2command.py` & `python-rtmidi-1.5.0/examples/midi2command/midi2command.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/midifilter/__main__.py` & `python-rtmidi-1.5.0/examples/midifilter/__main__.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/midifilter/filters.py` & `python-rtmidi-1.5.0/examples/midifilter/filters.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/sendsysex.py` & `python-rtmidi-1.5.0/examples/sendsysex.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/sequencer/sequencer.py` & `python-rtmidi-1.5.0/examples/sequencer/sequencer.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/sysex/send_sysex.py` & `python-rtmidi-1.5.0/examples/sysex/send_sysex.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/sysex/send_sysex_file.py` & `python-rtmidi-1.5.0/examples/sysex/send_sysex_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     args = ap.parse_args()
 
     midiout, name = open_midioutput(args.port)
     print("Opened port '%s'." % name)
 
     for filename in getattr(args, "sysex-file"):
         with open(filename, 'rb') as syx:
-            data = syx.read()
+            data = bytearray(syx.read())
             assert data[0] == 0xF0 and data[-1] == 0xF7
 
             if args.length:
                 data = bytearray(data[:args.length])
 
             data[-1] = 0xF7
             print("Sending %d bytes from '%s'..." % (len(data), filename))
```

### Comparing `python-rtmidi-1.4.9/examples/sysexsaver/__main__.py` & `python-rtmidi-1.5.0/examples/sysexsaver/__main__.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/sysexsaver/manufacturers.csv` & `python-rtmidi-1.5.0/examples/sysexsaver/manufacturers.csv`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/sysexsaver/manufacturers.py` & `python-rtmidi-1.5.0/examples/sysexsaver/manufacturers.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/sysexsaver/models.py` & `python-rtmidi-1.5.0/examples/sysexsaver/models.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/examples/wavetablemodstep.py` & `python-rtmidi-1.5.0/examples/wavetablemodstep.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/rtmidi/midiconstants.py` & `python-rtmidi-1.5.0/rtmidi/midiconstants.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/rtmidi/midiutil.py` & `python-rtmidi-1.5.0/rtmidi/midiutil.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 
     ``rtmidi.SystemError``
         Raised when RtMidi backend initialization fails.
 
     """
     midiin = rtmidi.MidiIn(get_api_from_environment(api))
     list_available_ports(midiio=midiin)
+    midiin.delete()
 
 
 def list_output_ports(api=rtmidi.API_UNSPECIFIED):
     """List available MIDI output ports.
 
     Optionally the RtMidi API can be passed with the ``api`` argument. If not
     it will be determined via the ``get_api_from_environment`` function.
@@ -111,20 +112,21 @@
 
     ``rtmidi.SystemError``
         Raised when RtMidi backend initialization fails.
 
     """
     midiout = rtmidi.MidiOut(get_api_from_environment(api))
     list_available_ports(midiio=midiout)
+    midiout.delete()
 
 
 def open_midiport(port=None, type_="input", api=rtmidi.API_UNSPECIFIED,
                   use_virtual=False, interactive=True, client_name=None,
                   port_name=None):
-    """Open MIDI port for input or output and return MidiIn/MidiOut instance.
+    """Open MIDI port for in-/output and return MidiIn/-Out instance and port name.
 
     Arguments:
 
     ``port``
         A MIDI port number or (substring of) a port name or ``None``.
 
         Available ports are enumerated starting from zero separately for input
@@ -257,27 +259,27 @@
         return midiobj, port_name
     else:
         raise rtmidi.InvalidPortError("Invalid port.")
 
 
 def open_midiinput(port=None, api=rtmidi.API_UNSPECIFIED, use_virtual=False,
                    interactive=True, client_name=None, port_name=None):
-    """Open a MIDI port for input and return a MidiIn instance.
+    """Open a MIDI port for input and return a MidiIn instance and port name.
 
-    See the ``open_midiport`` function for information on parameters and
-    possible exceptions.
+    See the ``open_midiport`` function for information on parameters, return
+    types and possible exceptions.
 
     """
     return open_midiport(port, "input", api, use_virtual, interactive,
                          client_name, port_name)
 
 
 def open_midioutput(port=None, api=rtmidi.API_UNSPECIFIED, use_virtual=False,
                     interactive=True, client_name=None, port_name=None):
-    """Open a MIDI port for output and return a MidiOut instance.
+    """Open a MIDI port for output and return a MidiOut instance and port name.
 
-    See the ``open_midiport`` function for information on parameters and
-    possible exceptions.
+    See the ``open_midiport`` function for information on parameters, return
+    types and possible exceptions.
 
     """
     return open_midiport(port, "output", api, use_virtual, interactive,
                          client_name, port_name)
```

### Comparing `python-rtmidi-1.4.9/src/_rtmidi.cpp` & `python-rtmidi-1.5.0/src/_rtmidi.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,65 +1,20 @@
-/* Generated by Cython 0.29.23 */
-
-/* BEGIN: Cython Metadata
-{
-    "distutils": {
-        "define_macros": [
-            [
-                "__RTMIDI_SILENCE_WARNINGS__",
-                null
-            ],
-            [
-                "__LINUX_ALSA__",
-                null
-            ],
-            [
-                "__UNIX_JACK__",
-                null
-            ],
-            [
-                "JACK_HAS_PORT_RENAME",
-                null
-            ]
-        ],
-        "depends": [
-            "src/pyinit.h",
-            "src/rtmidi/RtMidi.h"
-        ],
-        "include_dirs": [
-            "src",
-            "src/rtmidi"
-        ],
-        "language": "c++",
-        "libraries": [
-            "asound",
-            "jack",
-            "pthread"
-        ],
-        "name": "rtmidi._rtmidi",
-        "sources": [
-            "src/_rtmidi.pyx",
-            "src/rtmidi/RtMidi.cpp"
-        ]
-    },
-    "module_name": "rtmidi._rtmidi"
-}
-END: Cython Metadata */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_23"
-#define CYTHON_HEX_VERSION 0x001D17F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -90,14 +45,15 @@
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
 #ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
@@ -126,18 +82,22 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #undef CYTHON_USE_ASYNC_SLOTS
   #define CYTHON_USE_ASYNC_SLOTS 0
@@ -167,18 +127,67 @@
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
+  #endif
+#elif defined(PY_NOGIL)
+  #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
+  #define CYTHON_COMPILING_IN_CPYTHON 0
+  #define CYTHON_COMPILING_IN_NOGIL 1
+  #ifndef CYTHON_USE_TYPE_SLOTS
+    #define CYTHON_USE_TYPE_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYTYPE_LOOKUP
+  #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #ifndef CYTHON_USE_ASYNC_SLOTS
+    #define CYTHON_USE_ASYNC_SLOTS 1
+  #endif
+  #undef CYTHON_USE_PYLIST_INTERNALS
+  #define CYTHON_USE_PYLIST_INTERNALS 0
+  #ifndef CYTHON_USE_UNICODE_INTERNALS
+    #define CYTHON_USE_UNICODE_INTERNALS 1
+  #endif
+  #undef CYTHON_USE_UNICODE_WRITER
+  #define CYTHON_USE_UNICODE_WRITER 0
+  #undef CYTHON_USE_PYLONG_INTERNALS
+  #define CYTHON_USE_PYLONG_INTERNALS 0
+  #ifndef CYTHON_AVOID_BORROWED_REFS
+    #define CYTHON_AVOID_BORROWED_REFS 0
+  #endif
+  #ifndef CYTHON_ASSUME_SAFE_MACROS
+    #define CYTHON_ASSUME_SAFE_MACROS 1
+  #endif
+  #ifndef CYTHON_UNPACK_METHODS
+    #define CYTHON_UNPACK_METHODS 1
+  #endif
+  #undef CYTHON_FAST_THREAD_STATE
+  #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_PYCALL
+  #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE 1
+  #endif
+  #undef CYTHON_USE_DICT_VERSIONS
+  #define CYTHON_USE_DICT_VERSIONS 0
+  #undef CYTHON_USE_EXC_INFO_STACK
+  #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
+  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYTYPE_LOOKUP
     #define CYTHON_USE_PYTYPE_LOOKUP 0
   #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
@@ -190,61 +199,72 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0
+  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
-    #define CYTHON_FAST_PYCALL 1
+    #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030A0000)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
-  #include "longintrepr.h"
+  #if PY_MAJOR_VERSION < 3
+    #include "longintrepr.h"
+  #endif
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -367,17 +387,76 @@
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
-  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyType_Type
+#if PY_VERSION_HEX >= 0x030B00A1
+    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int k, int l, int s, int f,
+                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
+                                                    PyObject *fv, PyObject *cell, PyObject* fn,
+                                                    PyObject *name, int fline, PyObject *lnos) {
+        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
+        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *call_result=NULL, *empty=NULL;
+        const char *fn_cstr=NULL;
+        const char *name_cstr=NULL;
+        PyCodeObject* co=NULL;
+        PyObject *type, *value, *traceback;
+        PyErr_Fetch(&type, &value, &traceback);
+        if (!(kwds=PyDict_New())) goto end;
+        if (!(argcount=PyLong_FromLong(a))) goto end;
+        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
+        if (!(posonlyargcount=PyLong_FromLong(0))) goto end;
+        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
+        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
+        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
+        if (!(nlocals=PyLong_FromLong(l))) goto end;
+        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
+        if (!(stacksize=PyLong_FromLong(s))) goto end;
+        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
+        if (!(flags=PyLong_FromLong(f))) goto end;
+        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
+        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
+        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
+        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
+        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
+        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto cleanup_code_too;
+        if (!(empty = PyTuple_New(0))) goto cleanup_code_too; // unfortunately __pyx_empty_tuple isn't available here
+        if (!(call_result = PyObject_Call(replace, empty, kwds))) goto cleanup_code_too;
+        Py_XDECREF((PyObject*)co);
+        co = (PyCodeObject*)call_result;
+        call_result = NULL;
+        if (0) {
+            cleanup_code_too:
+            Py_XDECREF((PyObject*)co);
+            co = NULL;
+        }
+        end:
+        Py_XDECREF(kwds);
+        Py_XDECREF(argcount);
+        Py_XDECREF(posonlyargcount);
+        Py_XDECREF(kwonlyargcount);
+        Py_XDECREF(nlocals);
+        Py_XDECREF(stacksize);
+        Py_XDECREF(replace);
+        Py_XDECREF(call_result);
+        Py_XDECREF(empty);
+        if (type) {
+            PyErr_Restore(type, value, traceback);
+        }
+        return co;
+    }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
@@ -483,27 +562,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
+  #else
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
+  #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -627,16 +714,18 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(WIN32) || defined(MS_WINDOWS)
-  #define _USE_MATH_DEFINES
+#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
+  #if !defined(_USE_MATH_DEFINES)
+    #define _USE_MATH_DEFINES
+  #endif
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -659,25 +748,24 @@
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__rtmidi___rtmidi
-#define __PYX_HAVE_API__rtmidi___rtmidi
+#define __PYX_HAVE___rtmidi
+#define __PYX_HAVE_API___rtmidi
 /* Early includes */
 #include <string.h>
+#include <string>
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
-#include <string>
 #include <vector>
-#include "pyinit.h"
 #include "RtMidi.h"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -880,15 +968,15 @@
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
 static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
 
 static const char *__pyx_f[] = {
-  "src/_rtmidi.pyx",
+  "_rtmidi.pyx",
   "stringsource",
 };
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
@@ -897,102 +985,102 @@
 #define __Pyx_PyGILState_Release PyGILState_Release
 #define __Pyx_FastGIL_Remember()
 #define __Pyx_FastGIL_Forget()
 #define __Pyx_FastGilFuncInit()
 
 
 /*--- Type declarations ---*/
-struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase;
-struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn;
-struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut;
+struct __pyx_obj_7_rtmidi_MidiBase;
+struct __pyx_obj_7_rtmidi_MidiIn;
+struct __pyx_obj_7_rtmidi_MidiOut;
 
-/* "src/_rtmidi.pyx":431
+/* "_rtmidi.pyx":430
  * 
  * 
  * cdef class MidiBase:             # <<<<<<<<<<<<<<
  *     cdef object _port
  *     cdef object _error_callback
  */
-struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase {
+struct __pyx_obj_7_rtmidi_MidiBase {
   PyObject_HEAD
-  struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase *__pyx_vtab;
+  struct __pyx_vtabstruct_7_rtmidi_MidiBase *__pyx_vtab;
   PyObject *_port;
   PyObject *_error_callback;
   PyObject *_deleted;
 };
 
 
-/* "src/_rtmidi.pyx":757
+/* "_rtmidi.pyx":756
  * 
  * 
  * cdef class MidiIn(MidiBase):             # <<<<<<<<<<<<<<
  *     """Midi input client interface.
  * 
  */
-struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn {
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase __pyx_base;
+struct __pyx_obj_7_rtmidi_MidiIn {
+  struct __pyx_obj_7_rtmidi_MidiBase __pyx_base;
   RtMidiIn *thisptr;
   PyObject *_callback;
 };
 
 
-/* "src/_rtmidi.pyx":969
+/* "_rtmidi.pyx":968
  * 
  * 
  * cdef class MidiOut(MidiBase):             # <<<<<<<<<<<<<<
  *     """Midi output client interface.
  * 
  */
-struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut {
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase __pyx_base;
+struct __pyx_obj_7_rtmidi_MidiOut {
+  struct __pyx_obj_7_rtmidi_MidiBase __pyx_base;
   RtMidiOut *thisptr;
 };
 
 
 
-/* "src/_rtmidi.pyx":431
+/* "_rtmidi.pyx":430
  * 
  * 
  * cdef class MidiBase:             # <<<<<<<<<<<<<<
  *     cdef object _port
  *     cdef object _error_callback
  */
 
-struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase {
-  RtMidi *(*baseptr)(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *);
+struct __pyx_vtabstruct_7_rtmidi_MidiBase {
+  RtMidi *(*baseptr)(struct __pyx_obj_7_rtmidi_MidiBase *);
 };
-static struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase *__pyx_vtabptr_6rtmidi_7_rtmidi_MidiBase;
+static struct __pyx_vtabstruct_7_rtmidi_MidiBase *__pyx_vtabptr_7_rtmidi_MidiBase;
 
 
-/* "src/_rtmidi.pyx":757
+/* "_rtmidi.pyx":756
  * 
  * 
  * cdef class MidiIn(MidiBase):             # <<<<<<<<<<<<<<
  *     """Midi input client interface.
  * 
  */
 
-struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiIn {
-  struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase __pyx_base;
+struct __pyx_vtabstruct_7_rtmidi_MidiIn {
+  struct __pyx_vtabstruct_7_rtmidi_MidiBase __pyx_base;
 };
-static struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiIn *__pyx_vtabptr_6rtmidi_7_rtmidi_MidiIn;
+static struct __pyx_vtabstruct_7_rtmidi_MidiIn *__pyx_vtabptr_7_rtmidi_MidiIn;
 
 
-/* "src/_rtmidi.pyx":969
+/* "_rtmidi.pyx":968
  * 
  * 
  * cdef class MidiOut(MidiBase):             # <<<<<<<<<<<<<<
  *     """Midi output client interface.
  * 
  */
 
-struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiOut {
-  struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase __pyx_base;
+struct __pyx_vtabstruct_7_rtmidi_MidiOut {
+  struct __pyx_vtabstruct_7_rtmidi_MidiBase __pyx_base;
 };
-static struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiOut *__pyx_vtabptr_6rtmidi_7_rtmidi_MidiOut;
+static struct __pyx_vtabstruct_7_rtmidi_MidiOut *__pyx_vtabptr_7_rtmidi_MidiOut;
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
@@ -1103,21 +1191,29 @@
 #define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
+#if CYTHON_FAST_PYCALL
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
+#endif // CYTHON_FAST_PYCALL
 #endif
 
 /* PyCFunctionFastCall.proto */
 #if CYTHON_FAST_PYCCALL
 static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
 #else
 #define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
@@ -1206,26 +1302,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1641,44 +1737,44 @@
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
-static RtMidi *__pyx_f_6rtmidi_7_rtmidi_8MidiBase_baseptr(CYTHON_UNUSED struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self); /* proto*/
-static RtMidi *__pyx_f_6rtmidi_7_rtmidi_6MidiIn_baseptr(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self); /* proto*/
-static RtMidi *__pyx_f_6rtmidi_7_rtmidi_7MidiOut_baseptr(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self); /* proto*/
+static RtMidi *__pyx_f_7_rtmidi_8MidiBase_baseptr(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self); /* proto*/
+static RtMidi *__pyx_f_7_rtmidi_6MidiIn_baseptr(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self); /* proto*/
+static RtMidi *__pyx_f_7_rtmidi_7MidiOut_baseptr(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self); /* proto*/
 
 /* Module declarations from 'libcpp' */
 
 /* Module declarations from 'libc.string' */
 
 /* Module declarations from 'libcpp.string' */
 
 /* Module declarations from 'libcpp.vector' */
 
-/* Module declarations from 'rtmidi._rtmidi' */
-static PyTypeObject *__pyx_ptype_6rtmidi_7_rtmidi_MidiBase = 0;
-static PyTypeObject *__pyx_ptype_6rtmidi_7_rtmidi_MidiIn = 0;
-static PyTypeObject *__pyx_ptype_6rtmidi_7_rtmidi_MidiOut = 0;
-static void __pyx_f_6rtmidi_7_rtmidi__cb_func(double, std::vector<unsigned char>  *, void *); /*proto*/
-static void __pyx_f_6rtmidi_7_rtmidi__cb_error_func(enum RtMidiError::Type, std::string const &, void *); /*proto*/
-static PyObject *__pyx_f_6rtmidi_7_rtmidi___pyx_unpickle_MidiBase__set_state(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *, PyObject *); /*proto*/
+/* Module declarations from '_rtmidi' */
+static PyTypeObject *__pyx_ptype_7_rtmidi_MidiBase = 0;
+static PyTypeObject *__pyx_ptype_7_rtmidi_MidiIn = 0;
+static PyTypeObject *__pyx_ptype_7_rtmidi_MidiOut = 0;
+static void __pyx_f_7_rtmidi__cb_func(double, std::vector<unsigned char>  *, void *); /*proto*/
+static void __pyx_f_7_rtmidi__cb_error_func(enum RtMidiError::Type, std::string const &, void *); /*proto*/
+static PyObject *__pyx_f_7_rtmidi___pyx_unpickle_MidiBase__set_state(struct __pyx_obj_7_rtmidi_MidiBase *, PyObject *); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyObject_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyUnicode_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyStr_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyBytes_string_to_py_std__in_string(std::string const &); /*proto*/
 static CYTHON_INLINE PyObject *__pyx_convert_PyByteArray_string_to_py_std__in_string(std::string const &); /*proto*/
 static std::string __pyx_convert_string_from_py_std__in_string(PyObject *); /*proto*/
-#define __Pyx_MODULE_NAME "rtmidi._rtmidi"
-extern int __pyx_module_is_main_rtmidi___rtmidi;
-int __pyx_module_is_main_rtmidi___rtmidi = 0;
+#define __Pyx_MODULE_NAME "_rtmidi"
+extern int __pyx_module_is_main__rtmidi;
+int __pyx_module_is_main__rtmidi = 0;
 
-/* Implementation of 'rtmidi._rtmidi' */
+/* Implementation of '_rtmidi' */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_MemoryError;
 static PyObject *__pyx_builtin_OSError;
 static PyObject *__pyx_builtin_range;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_super;
@@ -1722,14 +1818,15 @@
 static const char __pyx_k_latin1[] = "latin1";
 static const char __pyx_k_module[] = "__module__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_output[] = "output";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_port_2[] = "port";
 static const char __pyx_k_reduce[] = "__reduce__";
+static const char __pyx_k_rtmidi[] = "_rtmidi";
 static const char __pyx_k_timing[] = "timing";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_MidiOut[] = "MidiOut";
 static const char __pyx_k_OSError[] = "OSError";
 static const char __pyx_k_prepare[] = "__prepare__";
 static const char __pyx_k_thisptr[] = "thisptr";
 static const char __pyx_k_MidiBase[] = "MidiBase";
@@ -1770,24 +1867,22 @@
 static const char __pyx_k_decode_string[] = "_decode_string";
 static const char __pyx_k_get_port_name[] = "get_port_name";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_API_LINUX_ALSA[] = "API_LINUX_ALSA";
 static const char __pyx_k_API_WINDOWS_MM[] = "API_WINDOWS_MM";
 static const char __pyx_k_NoDevicesError[] = "NoDevicesError";
 static const char __pyx_k_get_port_count[] = "get_port_count";
-static const char __pyx_k_rtmidi__rtmidi[] = "rtmidi._rtmidi";
 static const char __pyx_k_API_MACOSX_CORE[] = "API_MACOSX_CORE";
 static const char __pyx_k_API_UNSPECIFIED[] = "API_UNSPECIFIED";
 static const char __pyx_k_InvalidUseError[] = "InvalidUseError";
 static const char __pyx_k_RtMidiIn_Client[] = "RtMidiIn Client";
 static const char __pyx_k_cancel_callback[] = "cancel_callback";
 static const char __pyx_k_get_current_api[] = "get_current_api";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
-static const char __pyx_k_src__rtmidi_pyx[] = "src/_rtmidi.pyx";
 static const char __pyx_k_API_RTMIDI_DUMMY[] = "API_RTMIDI_DUMMY";
 static const char __pyx_k_InvalidPortError[] = "InvalidPortError";
 static const char __pyx_k_RtMidiOut_Client[] = "RtMidiOut Client";
 static const char __pyx_k_RtMidi_virtual_s[] = "RtMidi virtual %s";
 static const char __pyx_k_get_compiled_api[] = "get_compiled_api";
 static const char __pyx_k_queue_size_limit[] = "queue_size_limit";
 static const char __pyx_k_ERRORTYPE_WARNING[] = "ERRORTYPE_WARNING";
@@ -1816,20 +1911,21 @@
 static const char __pyx_k_get_compiled_api_by_name[] = "get_compiled_api_by_name";
 static const char __pyx_k_UnsupportedOperationError[] = "UnsupportedOperationError";
 static const char __pyx_k_message_must_not_be_empty[] = "'message' must not be empty.";
 static const char __pyx_k_r_already_opened_s_port_i[] = "%r already opened %s port %i.";
 static const char __pyx_k_ERRORTYPE_NO_DEVICES_FOUND[] = "ERRORTYPE_NO_DEVICES_FOUND";
 static const char __pyx_k_ERRORTYPE_INVALID_PARAMETER[] = "ERRORTYPE_INVALID_PARAMETER";
 static const char __pyx_k_error_looking_for_port_name[] = "error looking for port name!";
+static const char __pyx_k_home_runner_work_python_rtmidi[] = "/home/runner/work/python-rtmidi/python-rtmidi/src/_rtmidi.pyx";
 static const char __pyx_k_A_Python_binding_for_the_RtMidi[] = "A Python binding for the RtMidi C++ library implemented using Cython.\n\nOverview\n========\n\n**RtMidi** is a set of C++ classes which provides a concise and simple,\ncross-platform API (Application Programming Interface) for realtime MIDI\ninput / output across Linux (ALSA & JACK), macOS / OS X (CoreMIDI & JACK),\nand Windows (MultiMedia System) operating systems.\n\n**python-rtmidi** is a Python binding for RtMidi implemented using Cython_ and\nprovides a thin wrapper around the RtMidi C++ interface. The API is basically\nthe same as the C++ one but with the naming scheme of classes, methods and\nparameters adapted to the Python PEP-8 conventions and requirements of the\nPython package naming structure. **python-rtmidi** supports Python 3 (3.6, 3.7,\n3.8, and 3.9).\n\n\nUsage example\n=============\n\nHere's a short example of how to use **python-rtmidi** to open the first\navailable MIDI output port and send a middle C note on MIDI channel 1::\n\n    import time\n    import rtmidi\n\n    midiout = rtmidi.MidiOut()\n    available_ports = midiout.get_ports()\n\n    if available_ports:\n        midiout.open_port(0)\n    else:\n        midiout.open_virtual_port(\"My virtual output\")\n\n    with midiout:\n        note_on = [0x90, 60, 112] # channel 1, middle C, velocity 112\n        note_off = [0x80, 60, 0]\n        midiout.send_message(note_on)\n        time.sleep(0.5)\n        midiout.send_message(note_off)\n        time.sleep(0.1)\n\n    del midiout\n\n\nConstants\n=========\n\n\nLow-level APIs\n--------------\n\nThese constants are returned by the ``get_compiled_api`` function and the\n``MidiIn.get_current_api`` resp. ``MidiOut.get_current_api`` methods and are\nused to specify the low-level MIDI backend API to use when creating a\n``MidiIn`` or ``MidiOut`` instance.\n\n``API_UNSPECIFIED``\n    Use first compiled-in API, which has any input resp. output ports\n``API_MACOSX_CORE``\n    macOS (OS X) CoreMIDI\n``API_LINUX_ALSA``\n    Linux ALSA\n``API_UNIX_JACK``""\n    Jack Client\n``API_WINDOWS_MM``\n    Windows MultiMedia\n``API_RTMIDI_DUMMY``\n    RtMidi Dummy API (used when no suitable API was found)\n\n\nError types\n-----------\n\nThese constants are passed as the first argument to an error handler\nfunction registered with ``set_error_callback`` method of a ``MidiIn``\nor ``MidiOut`` instance. For the meaning of each value, please see\nthe `RtMidi API reference`_.\n\n* ``ERRORTYPE_DEBUG_WARNING``\n* ``ERRORTYPE_DRIVER_ERROR``\n* ``ERRORTYPE_INVALID_DEVICE``\n* ``ERRORTYPE_INVALID_PARAMETER``\n* ``ERRORTYPE_INVALID_USE``\n* ``ERRORTYPE_MEMORY_ERROR``\n* ``ERRORTYPE_NO_DEVICES_FOUND``\n* ``ERRORTYPE_SYSTEM_ERROR``\n* ``ERRORTYPE_THREAD_ERROR``\n* ``ERRORTYPE_UNSPECIFIED``\n* ``ERRORTYPE_WARNING``\n\n\n.. _cython: http://cython.org/\n.. _rtmidi api reference:\n    http://www.music.mcgill.ca/~gary/rtmidi/classRtMidiError.html\n\n";
 static const char __pyx_k_Virtual_ports_are_not_supported[] = "Virtual ports are not supported by the Windows MultiMedia API.";
 static const char __pyx_k_message_longer_than_3_bytes_but[] = "'message' longer than 3 bytes but does not start with 0xF0.";
 static const char __pyx_k_API_backend_does_not_support_cha[] = "API backend does not support changing the client name.";
 static const char __pyx_k_Base_general_RtMidi_exception_Al[] = "Base general RtMidi exception.\n\n    All other exceptions in this module derive form this exception.\n\n    Instances have a ``type`` attribute that maps to one of the\n    ``ERRORTYPE_*`` constants.\n\n    ";
-static const char __pyx_k_Incompatible_checksums_s_vs_0x91[] = "Incompatible checksums (%s vs 0x9171c0f = (_deleted, _error_callback, _port))";
+static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x9171c0f, 0x2133db3, 0x021d8b9) = (_deleted, _error_callback, _port))";
 static const char __pyx_k_Raised_if_a_memory_allocation_fa[] = "Raised if a memory allocation failed on the C++ level.\n\n    Also derives from ``MemoryError``.\n\n    ";
 static const char __pyx_k_Raised_if_a_method_is_not_suppor[] = "Raised if a method is not supported by the low-level API.\n\n    Also derives from ``RuntimeError``.\n\n    ";
 static const char __pyx_k_Raised_if_an_error_happened_at_t[] = "Raised if an error happened at the MIDI driver or OS level.\n\n    Also derives from ``OSError``.\n\n    ";
 static const char __pyx_k_Raised_if_no_MIDI_devices_are_fo[] = "Raised if no MIDI devices are found.\n\n    Derives from ``rtmidi.SystemError``.\n\n    ";
 static const char __pyx_k_Raised_when_an_invalid_port_numb[] = "Raised when an invalid port number is used.\n\n    Also derives from ``ValueError``.\n\n    ";
 static const char __pyx_k_Raised_when_an_method_call_is_no[] = "Raised when an method call is not allowed in the current state.\n\n    Also derives from ``RuntimeError``.\n\n    ";
 static const char __pyx_k_error_sending_MIDI_message_to_po[] = "error sending MIDI message to port.";
@@ -1870,15 +1966,15 @@
 static PyObject *__pyx_n_u_ERRORTYPE_SYSTEM_ERROR;
 static PyObject *__pyx_n_s_ERRORTYPE_THREAD_ERROR;
 static PyObject *__pyx_n_u_ERRORTYPE_THREAD_ERROR;
 static PyObject *__pyx_n_s_ERRORTYPE_UNSPECIFIED;
 static PyObject *__pyx_n_u_ERRORTYPE_UNSPECIFIED;
 static PyObject *__pyx_n_s_ERRORTYPE_WARNING;
 static PyObject *__pyx_n_u_ERRORTYPE_WARNING;
-static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0x91;
+static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_InvalidPortError;
 static PyObject *__pyx_n_u_InvalidPortError;
 static PyObject *__pyx_n_s_InvalidUseError;
 static PyObject *__pyx_n_u_InvalidUseError;
 static PyObject *__pyx_kp_u_JACK_server_not_running;
 static PyObject *__pyx_n_s_MemoryAllocationError;
 static PyObject *__pyx_n_u_MemoryAllocationError;
@@ -1952,14 +2048,15 @@
 static PyObject *__pyx_n_u_get_compiled_api_by_name;
 static PyObject *__pyx_n_s_get_current_api;
 static PyObject *__pyx_n_s_get_port_count;
 static PyObject *__pyx_n_s_get_port_name;
 static PyObject *__pyx_n_s_get_rtmidi_version;
 static PyObject *__pyx_n_u_get_rtmidi_version;
 static PyObject *__pyx_n_s_getstate;
+static PyObject *__pyx_kp_s_home_runner_work_python_rtmidi;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_u_ignore;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_init;
 static PyObject *__pyx_n_u_input;
 static PyObject *__pyx_kp_u_is_invalid;
 static PyObject *__pyx_n_u_latin1;
@@ -1994,21 +2091,20 @@
 static PyObject *__pyx_n_s_queue_size_limit;
 static PyObject *__pyx_kp_u_r_already_opened_s_port_i;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_rtapi;
-static PyObject *__pyx_n_s_rtmidi__rtmidi;
+static PyObject *__pyx_n_s_rtmidi;
 static PyObject *__pyx_n_s_s;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_n_s_set_error_callback;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
-static PyObject *__pyx_kp_s_src__rtmidi_pyx;
 static PyObject *__pyx_n_s_startswith;
 static PyObject *__pyx_n_s_string_types;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_super;
 static PyObject *__pyx_n_s_sys;
 static PyObject *__pyx_n_s_sysex;
 static PyObject *__pyx_n_s_test;
@@ -2017,64 +2113,66 @@
 static PyObject *__pyx_n_s_to_bytes;
 static PyObject *__pyx_n_s_type;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_s_warn;
 static PyObject *__pyx_n_s_warnings;
 static PyObject *__pyx_n_u_win;
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi__to_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_11RtMidiError___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_msg, PyObject *__pyx_v_type); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_2get_api_display_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_api); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_4get_api_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_api); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6get_compiled_api(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8get_compiled_api_by_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_10get_rtmidi_version(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_12_default_error_handler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_etype, PyObject *__pyx_v_msg, CYTHON_UNUSED PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase___enter__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_2__exit__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_exc_info); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_4_check_port(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_6_decode_string(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_s, PyObject *__pyx_v_encoding); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_8get_port_count(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_10get_port_name(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, unsigned int __pyx_v_port, PyObject *__pyx_v_encoding); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_12get_ports(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_encoding); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_14is_port_open(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_16open_port(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, unsigned int __pyx_v_port, PyObject *__pyx_v_name); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_18open_virtual_port(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_20close_port(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_22set_client_name(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_24set_port_name(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_26set_error_callback(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_func, PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_28cancel_error_callback(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_30__reduce_cython__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_32__setstate_cython__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_6rtmidi_7_rtmidi_6MidiIn___cinit__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self, enum RtMidi::Api __pyx_v_rtapi, PyObject *__pyx_v_name, unsigned int __pyx_v_queue_size_limit); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_2get_current_api(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
-static void __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_4__dealloc__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_6delete(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_10is_deleted___get__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_8cancel_callback(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_10close_port(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_12get_message(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_14ignore_types(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self, PyObject *__pyx_v_sysex, PyObject *__pyx_v_timing, PyObject *__pyx_v_active_sense); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_16set_callback(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self, PyObject *__pyx_v_func, PyObject *__pyx_v_data); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static int __pyx_pf_6rtmidi_7_rtmidi_7MidiOut___cinit__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self, enum RtMidi::Api __pyx_v_rtapi, PyObject *__pyx_v_name); /* proto */
-static void __pyx_pf_6rtmidi_7_rtmidi_7MidiOut_2__dealloc__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_4delete(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_10is_deleted___get__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_6get_current_api(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_8send_message(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self, PyObject *__pyx_v_message); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_14__pyx_unpickle_MidiBase(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_6rtmidi_7_rtmidi_MidiBase(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_6rtmidi_7_rtmidi_MidiIn(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-static PyObject *__pyx_tp_new_6rtmidi_7_rtmidi_MidiOut(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_pf_7_rtmidi__to_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_11RtMidiError___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_msg, PyObject *__pyx_v_type); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_2get_api_display_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_api); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_4get_api_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_api); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6get_compiled_api(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8get_compiled_api_by_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_10get_rtmidi_version(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_12_default_error_handler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_etype, PyObject *__pyx_v_msg, CYTHON_UNUSED PyObject *__pyx_v_data); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase___enter__(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_2__exit__(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_exc_info); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_4_check_port(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_6_decode_string(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_s, PyObject *__pyx_v_encoding); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_8get_port_count(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_10get_port_name(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, unsigned int __pyx_v_port, PyObject *__pyx_v_encoding); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_12get_ports(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_encoding); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_14is_port_open(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_16open_port(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, unsigned int __pyx_v_port, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_18open_virtual_port(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_20close_port(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_22set_client_name(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_24set_port_name(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_26set_error_callback(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_func, PyObject *__pyx_v_data); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_28cancel_error_callback(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_30__reduce_cython__(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_32__setstate_cython__(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_7_rtmidi_6MidiIn___cinit__(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self, enum RtMidi::Api __pyx_v_rtapi, PyObject *__pyx_v_name, unsigned int __pyx_v_queue_size_limit); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_2get_current_api(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
+static void __pyx_pf_7_rtmidi_6MidiIn_4__dealloc__(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_6delete(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_10is_deleted___get__(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_8cancel_callback(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_10close_port(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_12get_message(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_14ignore_types(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self, PyObject *__pyx_v_sysex, PyObject *__pyx_v_timing, PyObject *__pyx_v_active_sense); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_16set_callback(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self, PyObject *__pyx_v_func, PyObject *__pyx_v_data); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static int __pyx_pf_7_rtmidi_7MidiOut___cinit__(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self, enum RtMidi::Api __pyx_v_rtapi, PyObject *__pyx_v_name); /* proto */
+static void __pyx_pf_7_rtmidi_7MidiOut_2__dealloc__(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_4delete(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_10is_deleted___get__(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_6get_current_api(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_8send_message(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self, PyObject *__pyx_v_message); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_7_rtmidi_14__pyx_unpickle_MidiBase(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_tp_new_7_rtmidi_MidiBase(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_7_rtmidi_MidiIn(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_tp_new_7_rtmidi_MidiOut(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_240;
+static PyObject *__pyx_int_2218169;
+static PyObject *__pyx_int_34815411;
 static PyObject *__pyx_int_152509455;
 static PyObject *__pyx_int_neg_1;
 static enum RtMidi::Api __pyx_k__4;
 static enum RtMidi::Api __pyx_k__7;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
@@ -2082,42 +2180,43 @@
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
-static PyObject *__pyx_tuple__15;
-static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_tuple__14;
+static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_tuple__27;
-static PyObject *__pyx_tuple__29;
-static PyObject *__pyx_codeobj__14;
-static PyObject *__pyx_codeobj__16;
-static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
-static PyObject *__pyx_codeobj__25;
+static PyObject *__pyx_tuple__19;
+static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__23;
+static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_tuple__28;
+static PyObject *__pyx_tuple__30;
+static PyObject *__pyx_codeobj__15;
+static PyObject *__pyx_codeobj__17;
+static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__22;
+static PyObject *__pyx_codeobj__24;
 static PyObject *__pyx_codeobj__26;
-static PyObject *__pyx_codeobj__28;
-static PyObject *__pyx_codeobj__30;
+static PyObject *__pyx_codeobj__27;
+static PyObject *__pyx_codeobj__29;
+static PyObject *__pyx_codeobj__31;
 /* Late includes */
 
-/* "src/_rtmidi.pyx":208
+/* "_rtmidi.pyx":207
  * # internal functions
  * 
  * cdef void _cb_func(double delta_time, vector[unsigned char] *msg_v,             # <<<<<<<<<<<<<<
  *                    void *cb_info) with gil:
  *     """Wrapper for a Python callback function for MIDI input."""
  */
 
-static void __pyx_f_6rtmidi_7_rtmidi__cb_func(double __pyx_v_delta_time, std::vector<unsigned char>  *__pyx_v_msg_v, void *__pyx_v_cb_info) {
+static void __pyx_f_7_rtmidi__cb_func(double __pyx_v_delta_time, std::vector<unsigned char>  *__pyx_v_msg_v, void *__pyx_v_cb_info) {
   PyObject *__pyx_v_func = NULL;
   PyObject *__pyx_v_data = NULL;
   PyObject *__pyx_v_message = NULL;
   std::vector<unsigned char> ::size_type __pyx_7genexpr__pyx_v_i;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
@@ -2134,113 +2233,113 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_cb_func", 0);
 
-  /* "src/_rtmidi.pyx":211
+  /* "_rtmidi.pyx":210
  *                    void *cb_info) with gil:
  *     """Wrapper for a Python callback function for MIDI input."""
  *     func, data = (<object> cb_info)             # <<<<<<<<<<<<<<
  *     message = [msg_v.at(i) for i in range(msg_v.size())]
  *     func((message, delta_time), data)
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_cb_info);
   __Pyx_INCREF(__pyx_t_1);
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 211, __pyx_L1_error)
+      __PYX_ERR(0, 210, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 210, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_5 = Py_TYPE(__pyx_t_4)->tp_iternext;
     index = 0; __pyx_t_2 = __pyx_t_5(__pyx_t_4); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_5(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_5(__pyx_t_4), 2) < 0) __PYX_ERR(0, 211, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_5(__pyx_t_4), 2) < 0) __PYX_ERR(0, 210, __pyx_L1_error)
     __pyx_t_5 = NULL;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 211, __pyx_L1_error)
+    __PYX_ERR(0, 210, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_func = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_data = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "src/_rtmidi.pyx":212
+  /* "_rtmidi.pyx":211
  *     """Wrapper for a Python callback function for MIDI input."""
  *     func, data = (<object> cb_info)
  *     message = [msg_v.at(i) for i in range(msg_v.size())]             # <<<<<<<<<<<<<<
  *     func((message, delta_time), data)
  * 
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_6 = __pyx_v_msg_v->size();
     __pyx_t_7 = __pyx_t_6;
     for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
       __pyx_7genexpr__pyx_v_i = __pyx_t_8;
       try {
         __pyx_t_9 = __pyx_v_msg_v->at(__pyx_7genexpr__pyx_v_i);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 212, __pyx_L1_error)
+        __PYX_ERR(0, 211, __pyx_L1_error)
       }
-      __pyx_t_3 = __Pyx_PyInt_From_unsigned_char(__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyInt_From_unsigned_char(__pyx_t_9); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 211, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 212, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 211, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
   } /* exit inner scope */
   __pyx_v_message = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":213
+  /* "_rtmidi.pyx":212
  *     func, data = (<object> cb_info)
  *     message = [msg_v.at(i) for i in range(msg_v.size())]
  *     func((message, delta_time), data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_message);
   __Pyx_GIVEREF(__pyx_v_message);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_message);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_3);
   __pyx_t_3 = 0;
@@ -2256,49 +2355,49 @@
       __Pyx_DECREF_SET(__pyx_t_3, function);
       __pyx_t_10 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_3)) {
     PyObject *__pyx_temp[3] = {__pyx_t_4, __pyx_t_2, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_3, __pyx_temp+1-__pyx_t_10, 2+__pyx_t_10); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   } else
   #endif
   {
-    __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_11 = PyTuple_New(2+__pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_11);
     if (__pyx_t_4) {
       __Pyx_GIVEREF(__pyx_t_4); PyTuple_SET_ITEM(__pyx_t_11, 0, __pyx_t_4); __pyx_t_4 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_11, 0+__pyx_t_10, __pyx_t_2);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyTuple_SET_ITEM(__pyx_t_11, 1+__pyx_t_10, __pyx_v_data);
     __pyx_t_2 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_11, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
   }
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":208
+  /* "_rtmidi.pyx":207
  * # internal functions
  * 
  * cdef void _cb_func(double delta_time, vector[unsigned char] *msg_v,             # <<<<<<<<<<<<<<
  *                    void *cb_info) with gil:
  *     """Wrapper for a Python callback function for MIDI input."""
  */
 
@@ -2306,34 +2405,34 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_11);
-  __Pyx_WriteUnraisable("rtmidi._rtmidi._cb_func", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("_rtmidi._cb_func", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_func);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XDECREF(__pyx_v_message);
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "src/_rtmidi.pyx":216
+/* "_rtmidi.pyx":215
  * 
  * 
  * cdef void _cb_error_func(ErrorType errorType, const string &errorText,             # <<<<<<<<<<<<<<
  *                          void *cb_info) except * with gil:
  *     """Wrapper for a Python callback function for errors."""
  */
 
-static void __pyx_f_6rtmidi_7_rtmidi__cb_error_func(enum RtMidiError::Type __pyx_v_errorType, std::string const &__pyx_v_errorText, void *__pyx_v_cb_info) {
+static void __pyx_f_7_rtmidi__cb_error_func(enum RtMidiError::Type __pyx_v_errorType, std::string const &__pyx_v_errorText, void *__pyx_v_cb_info) {
   PyObject *__pyx_v_func = NULL;
   PyObject *__pyx_v_data = NULL;
   PyObject *__pyx_v_decoder = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
@@ -2346,30 +2445,30 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
   #endif
   __Pyx_RefNannySetupContext("_cb_error_func", 0);
 
-  /* "src/_rtmidi.pyx":219
+  /* "_rtmidi.pyx":218
  *                          void *cb_info) except * with gil:
  *     """Wrapper for a Python callback function for errors."""
  *     func, data, decoder = (<object> cb_info)             # <<<<<<<<<<<<<<
  *     func(errorType, decoder(errorText), data)
  * 
  */
   __pyx_t_1 = ((PyObject *)__pyx_v_cb_info);
   __Pyx_INCREF(__pyx_t_1);
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 219, __pyx_L1_error)
+      __PYX_ERR(0, 218, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 2); 
     } else {
@@ -2377,62 +2476,62 @@
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyList_GET_ITEM(sequence, 2); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 218, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = Py_TYPE(__pyx_t_5)->tp_iternext;
     index = 0; __pyx_t_2 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 2; __pyx_t_4 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_4)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 219, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 218, __pyx_L1_error)
     __pyx_t_6 = NULL;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 219, __pyx_L1_error)
+    __PYX_ERR(0, 218, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_func = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_data = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v_decoder = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "src/_rtmidi.pyx":220
+  /* "_rtmidi.pyx":219
  *     """Wrapper for a Python callback function for errors."""
  *     func, data, decoder = (<object> cb_info)
  *     func(errorType, decoder(errorText), data)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(__pyx_v_errorType); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(__pyx_v_errorType); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_errorText); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_errorText); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_decoder);
   __pyx_t_5 = __pyx_v_decoder; __pyx_t_7 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_5);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
@@ -2440,15 +2539,15 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_5, function);
     }
   }
   __pyx_t_3 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_7, __pyx_t_2) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_t_2);
   __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 220, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 219, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_INCREF(__pyx_v_func);
   __pyx_t_5 = __pyx_v_func; __pyx_t_2 = NULL;
   __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_5);
@@ -2459,54 +2558,54 @@
       __Pyx_DECREF_SET(__pyx_t_5, function);
       __pyx_t_8 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_4, __pyx_t_3, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_5)) {
     PyObject *__pyx_temp[4] = {__pyx_t_2, __pyx_t_4, __pyx_t_3, __pyx_v_data};
-    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyCFunction_FastCall(__pyx_t_5, __pyx_temp+1-__pyx_t_8, 3+__pyx_t_8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3+__pyx_t_8); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_8, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_8, __pyx_t_3);
     __Pyx_INCREF(__pyx_v_data);
     __Pyx_GIVEREF(__pyx_v_data);
     PyTuple_SET_ITEM(__pyx_t_7, 2+__pyx_t_8, __pyx_v_data);
     __pyx_t_4 = 0;
     __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_5, __pyx_t_7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":216
+  /* "_rtmidi.pyx":215
  * 
  * 
  * cdef void _cb_error_func(ErrorType errorType, const string &errorText,             # <<<<<<<<<<<<<<
  *                          void *cb_info) except * with gil:
  *     """Wrapper for a Python callback function for errors."""
  */
 
@@ -2515,49 +2614,49 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("rtmidi._rtmidi._cb_error_func", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi._cb_error_func", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_func);
   __Pyx_XDECREF(__pyx_v_data);
   __Pyx_XDECREF(__pyx_v_decoder);
   __Pyx_RefNannyFinishContext();
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
 }
 
-/* "src/_rtmidi.pyx":223
+/* "_rtmidi.pyx":222
  * 
  * 
  * def _to_bytes(name):             # <<<<<<<<<<<<<<
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_1_to_bytes(PyObject *__pyx_self, PyObject *__pyx_v_name); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi__to_bytes[] = "_to_bytes(name)\nConvert a unicode (Python 2) or str (Python 3) object into bytes.";
-static PyMethodDef __pyx_mdef_6rtmidi_7_rtmidi_1_to_bytes = {"_to_bytes", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_1_to_bytes, METH_O, __pyx_doc_6rtmidi_7_rtmidi__to_bytes};
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_1_to_bytes(PyObject *__pyx_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pw_7_rtmidi_1_to_bytes(PyObject *__pyx_self, PyObject *__pyx_v_name); /*proto*/
+static char __pyx_doc_7_rtmidi__to_bytes[] = "_to_bytes(name)\nConvert a unicode (Python 2) or str (Python 3) object into bytes.";
+static PyMethodDef __pyx_mdef_7_rtmidi_1_to_bytes = {"_to_bytes", (PyCFunction)__pyx_pw_7_rtmidi_1_to_bytes, METH_O, __pyx_doc_7_rtmidi__to_bytes};
+static PyObject *__pyx_pw_7_rtmidi_1_to_bytes(PyObject *__pyx_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_to_bytes (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi__to_bytes(__pyx_self, ((PyObject *)__pyx_v_name));
+  __pyx_r = __pyx_pf_7_rtmidi__to_bytes(__pyx_self, ((PyObject *)__pyx_v_name));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi__to_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pf_7_rtmidi__to_bytes(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
@@ -2570,29 +2669,29 @@
   PyObject *__pyx_t_12 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_to_bytes", 0);
   __Pyx_INCREF(__pyx_v_name);
 
-  /* "src/_rtmidi.pyx":226
+  /* "_rtmidi.pyx":225
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  *     if isinstance(name, string_types):             # <<<<<<<<<<<<<<
  *         try:
  *             name = bytes(name, 'utf-8')  # Python 3
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_string_types); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_string_types); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_IsInstance(__pyx_v_name, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 226, __pyx_L1_error)
+  __pyx_t_2 = PyObject_IsInstance(__pyx_v_name, __pyx_t_1); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(0, 225, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "src/_rtmidi.pyx":227
+    /* "_rtmidi.pyx":226
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  *     if isinstance(name, string_types):
  *         try:             # <<<<<<<<<<<<<<
  *             name = bytes(name, 'utf-8')  # Python 3
  *         except TypeError:
  */
     {
@@ -2600,36 +2699,36 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_4, &__pyx_t_5, &__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       /*try:*/ {
 
-        /* "src/_rtmidi.pyx":228
+        /* "_rtmidi.pyx":227
  *     if isinstance(name, string_types):
  *         try:
  *             name = bytes(name, 'utf-8')  # Python 3             # <<<<<<<<<<<<<<
  *         except TypeError:
  *             name = name.encode('utf-8')  # Python 2
  */
-        __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L4_error)
+        __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_INCREF(__pyx_v_name);
         __Pyx_GIVEREF(__pyx_v_name);
         PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_name);
         __Pyx_INCREF(__pyx_kp_u_utf_8);
         __Pyx_GIVEREF(__pyx_kp_u_utf_8);
         PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_kp_u_utf_8);
-        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_t_1, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 228, __pyx_L4_error)
+        __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_t_1, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 227, __pyx_L4_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_DECREF_SET(__pyx_v_name, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "src/_rtmidi.pyx":227
+        /* "_rtmidi.pyx":226
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  *     if isinstance(name, string_types):
  *         try:             # <<<<<<<<<<<<<<
  *             name = bytes(name, 'utf-8')  # Python 3
  *         except TypeError:
  */
       }
@@ -2637,64 +2736,64 @@
       __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L9_try_end;
       __pyx_L4_error:;
       __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "src/_rtmidi.pyx":229
+      /* "_rtmidi.pyx":228
  *         try:
  *             name = bytes(name, 'utf-8')  # Python 3
  *         except TypeError:             # <<<<<<<<<<<<<<
  *             name = name.encode('utf-8')  # Python 2
  * 
  */
       __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_TypeError);
       if (__pyx_t_8) {
-        __Pyx_AddTraceback("rtmidi._rtmidi._to_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_1, &__pyx_t_9) < 0) __PYX_ERR(0, 229, __pyx_L6_except_error)
+        __Pyx_AddTraceback("_rtmidi._to_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_1, &__pyx_t_9) < 0) __PYX_ERR(0, 228, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_1);
         __Pyx_GOTREF(__pyx_t_9);
 
-        /* "src/_rtmidi.pyx":230
+        /* "_rtmidi.pyx":229
  *             name = bytes(name, 'utf-8')  # Python 3
  *         except TypeError:
  *             name = name.encode('utf-8')  # Python 2             # <<<<<<<<<<<<<<
  * 
  *     if not isinstance(name, bytes):
  */
-        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 230, __pyx_L6_except_error)
+        __pyx_t_11 = __Pyx_PyObject_GetAttrStr(__pyx_v_name, __pyx_n_s_encode); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 229, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_11);
         __pyx_t_12 = NULL;
         if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_11))) {
           __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_11);
           if (likely(__pyx_t_12)) {
             PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_11);
             __Pyx_INCREF(__pyx_t_12);
             __Pyx_INCREF(function);
             __Pyx_DECREF_SET(__pyx_t_11, function);
           }
         }
         __pyx_t_10 = (__pyx_t_12) ? __Pyx_PyObject_Call2Args(__pyx_t_11, __pyx_t_12, __pyx_kp_u_utf_8) : __Pyx_PyObject_CallOneArg(__pyx_t_11, __pyx_kp_u_utf_8);
         __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 230, __pyx_L6_except_error)
+        if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 229, __pyx_L6_except_error)
         __Pyx_GOTREF(__pyx_t_10);
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
         __Pyx_DECREF_SET(__pyx_v_name, __pyx_t_10);
         __pyx_t_10 = 0;
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
         __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         goto __pyx_L5_exception_handled;
       }
       goto __pyx_L6_except_error;
       __pyx_L6_except_error:;
 
-      /* "src/_rtmidi.pyx":227
+      /* "_rtmidi.pyx":226
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  *     if isinstance(name, string_types):
  *         try:             # <<<<<<<<<<<<<<
  *             name = bytes(name, 'utf-8')  # Python 3
  *         except TypeError:
  */
       __Pyx_XGIVEREF(__pyx_t_4);
@@ -2706,69 +2805,69 @@
       __Pyx_XGIVEREF(__pyx_t_4);
       __Pyx_XGIVEREF(__pyx_t_5);
       __Pyx_XGIVEREF(__pyx_t_6);
       __Pyx_ExceptionReset(__pyx_t_4, __pyx_t_5, __pyx_t_6);
       __pyx_L9_try_end:;
     }
 
-    /* "src/_rtmidi.pyx":226
+    /* "_rtmidi.pyx":225
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  *     if isinstance(name, string_types):             # <<<<<<<<<<<<<<
  *         try:
  *             name = bytes(name, 'utf-8')  # Python 3
  */
   }
 
-  /* "src/_rtmidi.pyx":232
+  /* "_rtmidi.pyx":231
  *             name = name.encode('utf-8')  # Python 2
  * 
  *     if not isinstance(name, bytes):             # <<<<<<<<<<<<<<
  *         raise TypeError("name must be bytes or (unicode) string.")
  * 
  */
   __pyx_t_3 = PyBytes_Check(__pyx_v_name); 
   __pyx_t_2 = ((!(__pyx_t_3 != 0)) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "src/_rtmidi.pyx":233
+    /* "_rtmidi.pyx":232
  * 
  *     if not isinstance(name, bytes):
  *         raise TypeError("name must be bytes or (unicode) string.")             # <<<<<<<<<<<<<<
  * 
  *     return name
  */
-    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 233, __pyx_L1_error)
+    __pyx_t_9 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 232, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_9);
     __Pyx_Raise(__pyx_t_9, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    __PYX_ERR(0, 233, __pyx_L1_error)
+    __PYX_ERR(0, 232, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":232
+    /* "_rtmidi.pyx":231
  *             name = name.encode('utf-8')  # Python 2
  * 
  *     if not isinstance(name, bytes):             # <<<<<<<<<<<<<<
  *         raise TypeError("name must be bytes or (unicode) string.")
  * 
  */
   }
 
-  /* "src/_rtmidi.pyx":235
+  /* "_rtmidi.pyx":234
  *         raise TypeError("name must be bytes or (unicode) string.")
  * 
  *     return name             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_name);
   __pyx_r = __pyx_v_name;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":223
+  /* "_rtmidi.pyx":222
  * 
  * 
  * def _to_bytes(name):             # <<<<<<<<<<<<<<
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  */
 
@@ -2776,36 +2875,36 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_9);
   __Pyx_XDECREF(__pyx_t_10);
   __Pyx_XDECREF(__pyx_t_11);
   __Pyx_XDECREF(__pyx_t_12);
-  __Pyx_AddTraceback("rtmidi._rtmidi._to_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi._to_bytes", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":277
+/* "_rtmidi.pyx":276
  *     type = ERR_UNSPECIFIED
  * 
  *     def __init__(self, msg, type=None):             # <<<<<<<<<<<<<<
  *         super().__init__(msg)
  *         self.type = self.type if type is None else type
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_11RtMidiError_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_11RtMidiError___init__[] = "RtMidiError.__init__(self, msg, type=None)";
-static PyMethodDef __pyx_mdef_6rtmidi_7_rtmidi_11RtMidiError_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_11RtMidiError_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_11RtMidiError___init__};
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_11RtMidiError_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_11RtMidiError_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_11RtMidiError___init__[] = "RtMidiError.__init__(self, msg, type=None)";
+static PyMethodDef __pyx_mdef_7_rtmidi_11RtMidiError_1__init__ = {"__init__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_11RtMidiError_1__init__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_11RtMidiError___init__};
+static PyObject *__pyx_pw_7_rtmidi_11RtMidiError_1__init__(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_msg = 0;
   PyObject *__pyx_v_type = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -2833,25 +2932,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_self)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_msg)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 277, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, 1); __PYX_ERR(0, 276, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_type);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 277, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 276, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -2861,516 +2960,516 @@
     }
     __pyx_v_self = values[0];
     __pyx_v_msg = values[1];
     __pyx_v_type = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 277, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 276, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.RtMidiError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.RtMidiError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_11RtMidiError___init__(__pyx_self, __pyx_v_self, __pyx_v_msg, __pyx_v_type);
+  __pyx_r = __pyx_pf_7_rtmidi_11RtMidiError___init__(__pyx_self, __pyx_v_self, __pyx_v_msg, __pyx_v_type);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_11RtMidiError___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_msg, PyObject *__pyx_v_type) {
+static PyObject *__pyx_pf_7_rtmidi_11RtMidiError___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_msg, PyObject *__pyx_v_type) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "src/_rtmidi.pyx":278
+  /* "_rtmidi.pyx":277
  * 
  *     def __init__(self, msg, type=None):
  *         super().__init__(msg)             # <<<<<<<<<<<<<<
  *         self.type = self.type if type is None else type
  * 
  */
   __pyx_t_2 = __Pyx_CyFunction_GetClassObj(__pyx_self);
-  if (!__pyx_t_2) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 278, __pyx_L1_error) }
+  if (!__pyx_t_2) { PyErr_SetString(PyExc_SystemError, "super(): empty __class__ cell"); __PYX_ERR(0, 277, __pyx_L1_error) }
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2);
   __Pyx_INCREF(__pyx_v_self);
   __Pyx_GIVEREF(__pyx_v_self);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_v_self);
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_super, __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 278, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_init); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_msg);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 278, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":279
+  /* "_rtmidi.pyx":278
  *     def __init__(self, msg, type=None):
  *         super().__init__(msg)
  *         self.type = self.type if type is None else type             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_4 = (__pyx_v_type == Py_None);
   if ((__pyx_t_4 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 279, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_type); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 278, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_type);
     __pyx_t_1 = __pyx_v_type;
   }
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 279, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 278, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":277
+  /* "_rtmidi.pyx":276
  *     type = ERR_UNSPECIFIED
  * 
  *     def __init__(self, msg, type=None):             # <<<<<<<<<<<<<<
  *         super().__init__(msg)
  *         self.type = self.type if type is None else type
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("rtmidi._rtmidi.RtMidiError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.RtMidiError.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":338
+/* "_rtmidi.pyx":337
  * # wrappers for RtMidi's static methods and classes
  * 
  * def get_api_display_name(api):             # <<<<<<<<<<<<<<
  *     """Return the display name of a specified MIDI API.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_3get_api_display_name(PyObject *__pyx_self, PyObject *__pyx_v_api); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_2get_api_display_name[] = "get_api_display_name(api)\nReturn the display name of a specified MIDI API.\n\n    This returns a long name used for display purposes.\n\n    The ``api`` should be given as the one of ``API_*`` constants in the\n    module namespace, e.g.::\n\n        display_name = rtmidi.get_api_display_name(rtmidi.API_UNIX_JACK)\n\n    If the API is unknown, this function will return the empty string.\n\n    ";
-static PyMethodDef __pyx_mdef_6rtmidi_7_rtmidi_3get_api_display_name = {"get_api_display_name", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_3get_api_display_name, METH_O, __pyx_doc_6rtmidi_7_rtmidi_2get_api_display_name};
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_3get_api_display_name(PyObject *__pyx_self, PyObject *__pyx_v_api) {
+static PyObject *__pyx_pw_7_rtmidi_3get_api_display_name(PyObject *__pyx_self, PyObject *__pyx_v_api); /*proto*/
+static char __pyx_doc_7_rtmidi_2get_api_display_name[] = "get_api_display_name(api)\nReturn the display name of a specified MIDI API.\n\n    This returns a long name used for display purposes.\n\n    The ``api`` should be given as the one of ``API_*`` constants in the\n    module namespace, e.g.::\n\n        display_name = rtmidi.get_api_display_name(rtmidi.API_UNIX_JACK)\n\n    If the API is unknown, this function will return the empty string.\n\n    ";
+static PyMethodDef __pyx_mdef_7_rtmidi_3get_api_display_name = {"get_api_display_name", (PyCFunction)__pyx_pw_7_rtmidi_3get_api_display_name, METH_O, __pyx_doc_7_rtmidi_2get_api_display_name};
+static PyObject *__pyx_pw_7_rtmidi_3get_api_display_name(PyObject *__pyx_self, PyObject *__pyx_v_api) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_api_display_name (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_2get_api_display_name(__pyx_self, ((PyObject *)__pyx_v_api));
+  __pyx_r = __pyx_pf_7_rtmidi_2get_api_display_name(__pyx_self, ((PyObject *)__pyx_v_api));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_2get_api_display_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_api) {
+static PyObject *__pyx_pf_7_rtmidi_2get_api_display_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_api) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   enum RtMidi::Api __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_api_display_name", 0);
 
-  /* "src/_rtmidi.pyx":351
+  /* "_rtmidi.pyx":350
  * 
  *     """
  *     return RtMidi_getApiDisplayName(api).decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(__pyx_v_api)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 351, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_decode_cpp_string(RtMidi::getApiDisplayName(__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 351, __pyx_L1_error)
+  __pyx_t_1 = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(__pyx_v_api)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(RtMidi::getApiDisplayName(__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":338
+  /* "_rtmidi.pyx":337
  * # wrappers for RtMidi's static methods and classes
  * 
  * def get_api_display_name(api):             # <<<<<<<<<<<<<<
  *     """Return the display name of a specified MIDI API.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("rtmidi._rtmidi.get_api_display_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.get_api_display_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":354
+/* "_rtmidi.pyx":353
  * 
  * 
  * def get_api_name(api):             # <<<<<<<<<<<<<<
  *     """Return the name of a specified MIDI API.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_5get_api_name(PyObject *__pyx_self, PyObject *__pyx_v_api); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_4get_api_name[] = "get_api_name(api)\nReturn the name of a specified MIDI API.\n\n    This returns a short lower-case name used for identification purposes.\n\n    The ``api`` should be given as the one of ``API_*`` constants in the\n    module namespace, e.g.::\n\n        name = rtmidi.get_api_name(rtmidi.API_UNIX_JACK)\n\n    If the API is unknown, this function will return the empty string.\n\n    ";
-static PyMethodDef __pyx_mdef_6rtmidi_7_rtmidi_5get_api_name = {"get_api_name", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_5get_api_name, METH_O, __pyx_doc_6rtmidi_7_rtmidi_4get_api_name};
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_5get_api_name(PyObject *__pyx_self, PyObject *__pyx_v_api) {
+static PyObject *__pyx_pw_7_rtmidi_5get_api_name(PyObject *__pyx_self, PyObject *__pyx_v_api); /*proto*/
+static char __pyx_doc_7_rtmidi_4get_api_name[] = "get_api_name(api)\nReturn the name of a specified MIDI API.\n\n    This returns a short lower-case name used for identification purposes.\n\n    The ``api`` should be given as the one of ``API_*`` constants in the\n    module namespace, e.g.::\n\n        name = rtmidi.get_api_name(rtmidi.API_UNIX_JACK)\n\n    If the API is unknown, this function will return the empty string.\n\n    ";
+static PyMethodDef __pyx_mdef_7_rtmidi_5get_api_name = {"get_api_name", (PyCFunction)__pyx_pw_7_rtmidi_5get_api_name, METH_O, __pyx_doc_7_rtmidi_4get_api_name};
+static PyObject *__pyx_pw_7_rtmidi_5get_api_name(PyObject *__pyx_self, PyObject *__pyx_v_api) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_api_name (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_4get_api_name(__pyx_self, ((PyObject *)__pyx_v_api));
+  __pyx_r = __pyx_pf_7_rtmidi_4get_api_name(__pyx_self, ((PyObject *)__pyx_v_api));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_4get_api_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_api) {
+static PyObject *__pyx_pf_7_rtmidi_4get_api_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_api) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   enum RtMidi::Api __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_api_name", 0);
 
-  /* "src/_rtmidi.pyx":367
+  /* "_rtmidi.pyx":366
  * 
  *     """
  *     return RtMidi_getApiName(api).decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(__pyx_v_api)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 367, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_decode_cpp_string(RtMidi::getApiName(__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_1 = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(__pyx_v_api)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_cpp_string(RtMidi::getApiName(__pyx_t_1), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 366, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":354
+  /* "_rtmidi.pyx":353
  * 
  * 
  * def get_api_name(api):             # <<<<<<<<<<<<<<
  *     """Return the name of a specified MIDI API.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("rtmidi._rtmidi.get_api_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.get_api_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":370
+/* "_rtmidi.pyx":369
  * 
  * 
  * def get_compiled_api():             # <<<<<<<<<<<<<<
  *     """Return a list of low-level MIDI backend APIs this module supports.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7get_compiled_api(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_6get_compiled_api[] = "get_compiled_api()\nReturn a list of low-level MIDI backend APIs this module supports.\n\n    Check for support for a particular API by using the ``API_*`` constants in\n    the module namespace, i.e.::\n\n        if rtmidi.API_UNIX_JACK in rtmidi.get_compiled_api():\n            ...\n\n    ";
-static PyMethodDef __pyx_mdef_6rtmidi_7_rtmidi_7get_compiled_api = {"get_compiled_api", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_7get_compiled_api, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_6get_compiled_api};
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7get_compiled_api(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_7get_compiled_api(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_6get_compiled_api[] = "get_compiled_api()\nReturn a list of low-level MIDI backend APIs this module supports.\n\n    Check for support for a particular API by using the ``API_*`` constants in\n    the module namespace, i.e.::\n\n        if rtmidi.API_UNIX_JACK in rtmidi.get_compiled_api():\n            ...\n\n    ";
+static PyMethodDef __pyx_mdef_7_rtmidi_7get_compiled_api = {"get_compiled_api", (PyCFunction)__pyx_pw_7_rtmidi_7get_compiled_api, METH_NOARGS, __pyx_doc_7_rtmidi_6get_compiled_api};
+static PyObject *__pyx_pw_7_rtmidi_7get_compiled_api(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_compiled_api (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6get_compiled_api(__pyx_self);
+  __pyx_r = __pyx_pf_7_rtmidi_6get_compiled_api(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6get_compiled_api(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_7_rtmidi_6get_compiled_api(CYTHON_UNUSED PyObject *__pyx_self) {
   std::vector<enum RtMidi::Api>  __pyx_v_api_v;
   std::vector<enum RtMidi::Api> ::size_type __pyx_8genexpr1__pyx_v_i;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   std::vector<enum RtMidi::Api> ::size_type __pyx_t_2;
   std::vector<enum RtMidi::Api> ::size_type __pyx_t_3;
   std::vector<enum RtMidi::Api> ::size_type __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_compiled_api", 0);
 
-  /* "src/_rtmidi.pyx":382
+  /* "_rtmidi.pyx":381
  *     cdef vector[Api] api_v
  * 
  *     RtMidi_getCompiledApi(api_v)             # <<<<<<<<<<<<<<
  *     return [api_v[i] for i in range(api_v.size())]
  * 
  */
   RtMidi::getCompiledApi(__pyx_v_api_v);
 
-  /* "src/_rtmidi.pyx":383
+  /* "_rtmidi.pyx":382
  * 
  *     RtMidi_getCompiledApi(api_v)
  *     return [api_v[i] for i in range(api_v.size())]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 383, __pyx_L1_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 382, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = __pyx_v_api_v.size();
     __pyx_t_3 = __pyx_t_2;
     for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
       __pyx_8genexpr1__pyx_v_i = __pyx_t_4;
-      __pyx_t_5 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api((__pyx_v_api_v[__pyx_8genexpr1__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 383, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api((__pyx_v_api_v[__pyx_8genexpr1__pyx_v_i])); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 382, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 383, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 382, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":370
+  /* "_rtmidi.pyx":369
  * 
  * 
  * def get_compiled_api():             # <<<<<<<<<<<<<<
  *     """Return a list of low-level MIDI backend APIs this module supports.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("rtmidi._rtmidi.get_compiled_api", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.get_compiled_api", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":386
+/* "_rtmidi.pyx":385
  * 
  * 
  * def get_compiled_api_by_name(name):             # <<<<<<<<<<<<<<
  *     """Return the compiled MIDI API having the given name.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_9get_compiled_api_by_name(PyObject *__pyx_self, PyObject *__pyx_v_name); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8get_compiled_api_by_name[] = "get_compiled_api_by_name(name)\nReturn the compiled MIDI API having the given name.\n\n    A case insensitive comparison will check the specified name against the\n    list of compiled APIs, and return the one which matches. On failure, the\n    function returns ``API_UNSPECIFIED``.\n\n    ";
-static PyMethodDef __pyx_mdef_6rtmidi_7_rtmidi_9get_compiled_api_by_name = {"get_compiled_api_by_name", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_9get_compiled_api_by_name, METH_O, __pyx_doc_6rtmidi_7_rtmidi_8get_compiled_api_by_name};
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_9get_compiled_api_by_name(PyObject *__pyx_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pw_7_rtmidi_9get_compiled_api_by_name(PyObject *__pyx_self, PyObject *__pyx_v_name); /*proto*/
+static char __pyx_doc_7_rtmidi_8get_compiled_api_by_name[] = "get_compiled_api_by_name(name)\nReturn the compiled MIDI API having the given name.\n\n    A case insensitive comparison will check the specified name against the\n    list of compiled APIs, and return the one which matches. On failure, the\n    function returns ``API_UNSPECIFIED``.\n\n    ";
+static PyMethodDef __pyx_mdef_7_rtmidi_9get_compiled_api_by_name = {"get_compiled_api_by_name", (PyCFunction)__pyx_pw_7_rtmidi_9get_compiled_api_by_name, METH_O, __pyx_doc_7_rtmidi_8get_compiled_api_by_name};
+static PyObject *__pyx_pw_7_rtmidi_9get_compiled_api_by_name(PyObject *__pyx_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_compiled_api_by_name (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8get_compiled_api_by_name(__pyx_self, ((PyObject *)__pyx_v_name));
+  __pyx_r = __pyx_pf_7_rtmidi_8get_compiled_api_by_name(__pyx_self, ((PyObject *)__pyx_v_name));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8get_compiled_api_by_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pf_7_rtmidi_8get_compiled_api_by_name(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   std::string __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_compiled_api_by_name", 0);
 
-  /* "src/_rtmidi.pyx":394
+  /* "_rtmidi.pyx":393
  * 
  *     """
  *     return RtMidi_getCompiledApiByName(_to_bytes(name))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 394, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 394, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 394, __pyx_L1_error)
+  __pyx_t_4 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::getCompiledApiByName(__pyx_t_4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 394, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::getCompiledApiByName(__pyx_t_4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":386
+  /* "_rtmidi.pyx":385
  * 
  * 
  * def get_compiled_api_by_name(name):             # <<<<<<<<<<<<<<
  *     """Return the compiled MIDI API having the given name.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("rtmidi._rtmidi.get_compiled_api_by_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.get_compiled_api_by_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":397
+/* "_rtmidi.pyx":396
  * 
  * 
  * def get_rtmidi_version():             # <<<<<<<<<<<<<<
  *     """Return the version string of the wrapped RtMidi library."""
  *     return RtMidi_getVersion().decode('utf-8')
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_11get_rtmidi_version(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_10get_rtmidi_version[] = "get_rtmidi_version()\nReturn the version string of the wrapped RtMidi library.";
-static PyMethodDef __pyx_mdef_6rtmidi_7_rtmidi_11get_rtmidi_version = {"get_rtmidi_version", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_11get_rtmidi_version, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_10get_rtmidi_version};
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_11get_rtmidi_version(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_11get_rtmidi_version(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_10get_rtmidi_version[] = "get_rtmidi_version()\nReturn the version string of the wrapped RtMidi library.";
+static PyMethodDef __pyx_mdef_7_rtmidi_11get_rtmidi_version = {"get_rtmidi_version", (PyCFunction)__pyx_pw_7_rtmidi_11get_rtmidi_version, METH_NOARGS, __pyx_doc_7_rtmidi_10get_rtmidi_version};
+static PyObject *__pyx_pw_7_rtmidi_11get_rtmidi_version(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_rtmidi_version (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_10get_rtmidi_version(__pyx_self);
+  __pyx_r = __pyx_pf_7_rtmidi_10get_rtmidi_version(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_10get_rtmidi_version(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_7_rtmidi_10get_rtmidi_version(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_rtmidi_version", 0);
 
-  /* "src/_rtmidi.pyx":399
+  /* "_rtmidi.pyx":398
  * def get_rtmidi_version():
  *     """Return the version string of the wrapped RtMidi library."""
  *     return RtMidi_getVersion().decode('utf-8')             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_decode_cpp_string(RtMidi::getVersion(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_cpp_string(RtMidi::getVersion(), 0, PY_SSIZE_T_MAX, NULL, NULL, PyUnicode_DecodeUTF8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":397
+  /* "_rtmidi.pyx":396
  * 
  * 
  * def get_rtmidi_version():             # <<<<<<<<<<<<<<
  *     """Return the version string of the wrapped RtMidi library."""
  *     return RtMidi_getVersion().decode('utf-8')
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rtmidi._rtmidi.get_rtmidi_version", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.get_rtmidi_version", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":402
+/* "_rtmidi.pyx":401
  * 
  * 
  * def _default_error_handler(etype, msg, data=None):             # <<<<<<<<<<<<<<
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_13_default_error_handler(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_12_default_error_handler[] = "_default_error_handler(etype, msg, data=None)";
-static PyMethodDef __pyx_mdef_6rtmidi_7_rtmidi_13_default_error_handler = {"_default_error_handler", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_13_default_error_handler, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_12_default_error_handler};
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_13_default_error_handler(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_13_default_error_handler(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_12_default_error_handler[] = "_default_error_handler(etype, msg, data=None)";
+static PyMethodDef __pyx_mdef_7_rtmidi_13_default_error_handler = {"_default_error_handler", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_13_default_error_handler, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_12_default_error_handler};
+static PyObject *__pyx_pw_7_rtmidi_13_default_error_handler(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_etype = 0;
   PyObject *__pyx_v_msg = 0;
   CYTHON_UNUSED PyObject *__pyx_v_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -3398,25 +3497,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_etype)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_msg)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("_default_error_handler", 0, 2, 3, 1); __PYX_ERR(0, 402, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_default_error_handler", 0, 2, 3, 1); __PYX_ERR(0, 401, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_default_error_handler") < 0)) __PYX_ERR(0, 402, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_default_error_handler") < 0)) __PYX_ERR(0, 401, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -3426,1008 +3525,1008 @@
     }
     __pyx_v_etype = values[0];
     __pyx_v_msg = values[1];
     __pyx_v_data = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_default_error_handler", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 402, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_default_error_handler", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 401, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi._default_error_handler", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi._default_error_handler", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_12_default_error_handler(__pyx_self, __pyx_v_etype, __pyx_v_msg, __pyx_v_data);
+  __pyx_r = __pyx_pf_7_rtmidi_12_default_error_handler(__pyx_self, __pyx_v_etype, __pyx_v_msg, __pyx_v_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_12_default_error_handler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_etype, PyObject *__pyx_v_msg, CYTHON_UNUSED PyObject *__pyx_v_data) {
+static PyObject *__pyx_pf_7_rtmidi_12_default_error_handler(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_etype, PyObject *__pyx_v_msg, CYTHON_UNUSED PyObject *__pyx_v_data) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_default_error_handler", 0);
 
-  /* "src/_rtmidi.pyx":403
+  /* "_rtmidi.pyx":402
  * 
  * def _default_error_handler(etype, msg, data=None):
  *     if etype == ERR_MEMORY_ERROR:             # <<<<<<<<<<<<<<
  *         raise MemoryAllocationError(msg)
  *     elif etype == ERR_INVALID_PARAMETER:
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_v_etype, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_v_etype, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "src/_rtmidi.pyx":404
+    /* "_rtmidi.pyx":403
  * def _default_error_handler(etype, msg, data=None):
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)             # <<<<<<<<<<<<<<
  *     elif etype == ERR_INVALID_PARAMETER:
  *         raise InvalidPortError(msg)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MemoryAllocationError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 404, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_MemoryAllocationError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v_msg);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(0, 404, __pyx_L1_error)
+    __PYX_ERR(0, 403, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":403
+    /* "_rtmidi.pyx":402
  * 
  * def _default_error_handler(etype, msg, data=None):
  *     if etype == ERR_MEMORY_ERROR:             # <<<<<<<<<<<<<<
  *         raise MemoryAllocationError(msg)
  *     elif etype == ERR_INVALID_PARAMETER:
  */
   }
 
-  /* "src/_rtmidi.pyx":405
+  /* "_rtmidi.pyx":404
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  *     elif etype == ERR_INVALID_PARAMETER:             # <<<<<<<<<<<<<<
  *         raise InvalidPortError(msg)
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = PyObject_RichCompare(__pyx_v_etype, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_v_etype, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_3)) {
 
-    /* "src/_rtmidi.pyx":406
+    /* "_rtmidi.pyx":405
  *         raise MemoryAllocationError(msg)
  *     elif etype == ERR_INVALID_PARAMETER:
  *         raise InvalidPortError(msg)             # <<<<<<<<<<<<<<
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  *         raise SystemError(msg, type=etype)
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 406, __pyx_L1_error)
+    __PYX_ERR(0, 405, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":405
+    /* "_rtmidi.pyx":404
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  *     elif etype == ERR_INVALID_PARAMETER:             # <<<<<<<<<<<<<<
  *         raise InvalidPortError(msg)
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  */
   }
 
-  /* "src/_rtmidi.pyx":407
+  /* "_rtmidi.pyx":406
  *     elif etype == ERR_INVALID_PARAMETER:
  *         raise InvalidPortError(msg)
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):             # <<<<<<<<<<<<<<
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  */
   __Pyx_INCREF(__pyx_v_etype);
   __pyx_t_1 = __pyx_v_etype;
-  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_3 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::SYSTEM_ERROR); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::SYSTEM_ERROR); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_3 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::THREAD_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::THREAD_ERROR); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 407, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_3 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = (__pyx_t_3 != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "src/_rtmidi.pyx":408
+    /* "_rtmidi.pyx":407
  *         raise InvalidPortError(msg)
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  *         raise SystemError(msg, type=etype)             # <<<<<<<<<<<<<<
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 408, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_v_msg);
     __Pyx_GIVEREF(__pyx_v_msg);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_msg);
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_type, __pyx_v_etype) < 0) __PYX_ERR(0, 408, __pyx_L1_error)
-    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 408, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_type, __pyx_v_etype) < 0) __PYX_ERR(0, 407, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 407, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_6, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    __PYX_ERR(0, 408, __pyx_L1_error)
+    __PYX_ERR(0, 407, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":407
+    /* "_rtmidi.pyx":406
  *     elif etype == ERR_INVALID_PARAMETER:
  *         raise InvalidPortError(msg)
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):             # <<<<<<<<<<<<<<
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  */
   }
 
-  /* "src/_rtmidi.pyx":409
+  /* "_rtmidi.pyx":408
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):             # <<<<<<<<<<<<<<
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  *             raise InvalidPortError(msg)
  */
   __Pyx_INCREF(__pyx_v_etype);
   __pyx_t_6 = __pyx_v_etype;
-  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::WARNING); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::WARNING); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_6, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_6, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!__pyx_t_3) {
   } else {
     __pyx_t_5 = __pyx_t_3;
     goto __pyx_L7_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DEBUG_WARNING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DEBUG_WARNING); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_6, __pyx_t_4, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 409, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_5 = __pyx_t_3;
   __pyx_L7_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __pyx_t_3 = (__pyx_t_5 != 0);
   if (__pyx_t_3) {
 
-    /* "src/_rtmidi.pyx":410
+    /* "_rtmidi.pyx":409
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('no ports available!'):
  */
-    __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_portNumber, __pyx_v_msg, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 410, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PySequence_ContainsTF(__pyx_n_u_portNumber, __pyx_v_msg, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 409, __pyx_L1_error)
     __pyx_t_7 = (__pyx_t_5 != 0);
     if (__pyx_t_7) {
     } else {
       __pyx_t_3 = __pyx_t_7;
       goto __pyx_L10_bool_binop_done;
     }
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 409, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_is_invalid) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_is_invalid);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 410, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 409, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 410, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_7 < 0)) __PYX_ERR(0, 409, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __pyx_t_3 = __pyx_t_7;
     __pyx_L10_bool_binop_done:;
     if (unlikely(__pyx_t_3)) {
 
-      /* "src/_rtmidi.pyx":411
+      /* "_rtmidi.pyx":410
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  *             raise InvalidPortError(msg)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('no ports available!'):
  *             raise InvalidPortError(msg)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 411, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 410, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 411, __pyx_L1_error)
+      __PYX_ERR(0, 410, __pyx_L1_error)
 
-      /* "src/_rtmidi.pyx":410
+      /* "_rtmidi.pyx":409
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('no ports available!'):
  */
     }
 
-    /* "src/_rtmidi.pyx":412
+    /* "_rtmidi.pyx":411
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('no ports available!'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('error looking for port name!'):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_no_ports_available) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_no_ports_available);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "src/_rtmidi.pyx":413
+      /* "_rtmidi.pyx":412
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('no ports available!'):
  *             raise InvalidPortError(msg)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('error looking for port name!'):
  *             raise InvalidPortError(msg)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 412, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 413, __pyx_L1_error)
+      __PYX_ERR(0, 412, __pyx_L1_error)
 
-      /* "src/_rtmidi.pyx":412
+      /* "_rtmidi.pyx":411
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('no ports available!'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('error looking for port name!'):
  */
     }
 
-    /* "src/_rtmidi.pyx":414
+    /* "_rtmidi.pyx":413
  *         elif msg.endswith('no ports available!'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('error looking for port name!'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('event parsing error!'):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_error_looking_for_port_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_error_looking_for_port_name);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "src/_rtmidi.pyx":415
+      /* "_rtmidi.pyx":414
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('error looking for port name!'):
  *             raise InvalidPortError(msg)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('event parsing error!'):
  *             raise ValueError(msg)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 415, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidPortError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 414, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 415, __pyx_L1_error)
+      __PYX_ERR(0, 414, __pyx_L1_error)
 
-      /* "src/_rtmidi.pyx":414
+      /* "_rtmidi.pyx":413
  *         elif msg.endswith('no ports available!'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('error looking for port name!'):             # <<<<<<<<<<<<<<
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('event parsing error!'):
  */
     }
 
-    /* "src/_rtmidi.pyx":416
+    /* "_rtmidi.pyx":415
  *         elif msg.endswith('error looking for port name!'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('event parsing error!'):             # <<<<<<<<<<<<<<
  *             raise ValueError(msg)
  *         elif msg.endswith('error sending MIDI message to port.'):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_event_parsing_error) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_event_parsing_error);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 416, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "src/_rtmidi.pyx":417
+      /* "_rtmidi.pyx":416
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('event parsing error!'):
  *             raise ValueError(msg)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('error sending MIDI message to port.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  */
-      __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_v_msg); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 417, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_v_msg); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 416, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 417, __pyx_L1_error)
+      __PYX_ERR(0, 416, __pyx_L1_error)
 
-      /* "src/_rtmidi.pyx":416
+      /* "_rtmidi.pyx":415
  *         elif msg.endswith('error looking for port name!'):
  *             raise InvalidPortError(msg)
  *         elif msg.endswith('event parsing error!'):             # <<<<<<<<<<<<<<
  *             raise ValueError(msg)
  *         elif msg.endswith('error sending MIDI message to port.'):
  */
     }
 
-    /* "src/_rtmidi.pyx":418
+    /* "_rtmidi.pyx":417
  *         elif msg.endswith('event parsing error!'):
  *             raise ValueError(msg)
  *         elif msg.endswith('error sending MIDI message to port.'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_error_sending_MIDI_message_to_po) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_error_sending_MIDI_message_to_po);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 418, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "src/_rtmidi.pyx":419
+      /* "_rtmidi.pyx":418
  *             raise ValueError(msg)
  *         elif msg.endswith('error sending MIDI message to port.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 419, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_v_msg);
       __Pyx_GIVEREF(__pyx_v_msg);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_msg);
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 419, __pyx_L1_error)
+      __PYX_ERR(0, 418, __pyx_L1_error)
 
-      /* "src/_rtmidi.pyx":418
+      /* "_rtmidi.pyx":417
  *         elif msg.endswith('event parsing error!'):
  *             raise ValueError(msg)
  *         elif msg.endswith('error sending MIDI message to port.'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  */
     }
 
-    /* "src/_rtmidi.pyx":420
+    /* "_rtmidi.pyx":419
  *         elif msg.endswith('error sending MIDI message to port.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('JACK server not running?'):
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_2 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
       if (likely(__pyx_t_2)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_2);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_4, function);
       }
     }
     __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_4, __pyx_t_2, __pyx_kp_u_error_sending_MIDI_to_virtual_de) : __Pyx_PyObject_CallOneArg(__pyx_t_4, __pyx_kp_u_error_sending_MIDI_to_virtual_de);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 420, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 420, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 419, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "src/_rtmidi.pyx":421
+      /* "_rtmidi.pyx":420
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)             # <<<<<<<<<<<<<<
  *         elif msg.endswith('JACK server not running?'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_v_msg);
       __Pyx_GIVEREF(__pyx_v_msg);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_v_msg);
-      __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_type, __pyx_t_6) < 0) __PYX_ERR(0, 421, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_type, __pyx_t_6) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 421, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_4, __pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 420, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      __PYX_ERR(0, 421, __pyx_L1_error)
+      __PYX_ERR(0, 420, __pyx_L1_error)
 
-      /* "src/_rtmidi.pyx":420
+      /* "_rtmidi.pyx":419
  *         elif msg.endswith('error sending MIDI message to port.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('JACK server not running?'):
  */
     }
 
-    /* "src/_rtmidi.pyx":422
+    /* "_rtmidi.pyx":421
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('JACK server not running?'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         else:
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_msg, __pyx_n_s_endswith); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_6 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_kp_u_JACK_server_not_running) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_JACK_server_not_running);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 422, __pyx_L1_error)
+    if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 421, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 422, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely(__pyx_t_3 < 0)) __PYX_ERR(0, 421, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     if (unlikely(__pyx_t_3)) {
 
-      /* "src/_rtmidi.pyx":423
+      /* "_rtmidi.pyx":422
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('JACK server not running?'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)             # <<<<<<<<<<<<<<
  *         else:
  *             warnings.warn(msg)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 423, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 423, __pyx_L1_error)
+      __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_INCREF(__pyx_v_msg);
       __Pyx_GIVEREF(__pyx_v_msg);
       PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_msg);
-      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
-      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 423, __pyx_L1_error)
+      if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_t_1) < 0) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 422, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_Raise(__pyx_t_1, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-      __PYX_ERR(0, 423, __pyx_L1_error)
+      __PYX_ERR(0, 422, __pyx_L1_error)
 
-      /* "src/_rtmidi.pyx":422
+      /* "_rtmidi.pyx":421
  *         elif msg.endswith('error sending MIDI to virtual destinations.'):
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         elif msg.endswith('JACK server not running?'):             # <<<<<<<<<<<<<<
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         else:
  */
     }
 
-    /* "src/_rtmidi.pyx":425
+    /* "_rtmidi.pyx":424
  *             raise SystemError(msg, type=ERR_DRIVER_ERROR)
  *         else:
  *             warnings.warn(msg)             # <<<<<<<<<<<<<<
  *             return
  * 
  */
     /*else*/ {
-      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_warnings); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 425, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_warnings); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 424, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_warn); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 425, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_warn); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 424, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __pyx_t_4 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
         __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
         if (likely(__pyx_t_4)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
           __Pyx_INCREF(__pyx_t_4);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_2, function);
         }
       }
       __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v_msg) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_msg);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 425, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 424, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-      /* "src/_rtmidi.pyx":426
+      /* "_rtmidi.pyx":425
  *         else:
  *             warnings.warn(msg)
  *             return             # <<<<<<<<<<<<<<
  * 
  *     raise RtMidiError(msg, type=etype)
  */
       __Pyx_XDECREF(__pyx_r);
       __pyx_r = Py_None; __Pyx_INCREF(Py_None);
       goto __pyx_L0;
     }
 
-    /* "src/_rtmidi.pyx":409
+    /* "_rtmidi.pyx":408
  *     elif etype in (ERR_DRIVER_ERROR, ERR_SYSTEM_ERROR, ERR_THREAD_ERROR):
  *         raise SystemError(msg, type=etype)
  *     elif etype in (ERR_WARNING, ERR_DEBUG_WARNING):             # <<<<<<<<<<<<<<
  *         if 'portNumber' in msg and msg.endswith('is invalid.'):
  *             raise InvalidPortError(msg)
  */
   }
 
-  /* "src/_rtmidi.pyx":428
+  /* "_rtmidi.pyx":427
  *             return
  * 
  *     raise RtMidiError(msg, type=etype)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_msg);
   __Pyx_GIVEREF(__pyx_v_msg);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_msg);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_v_etype) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 428, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_type, __pyx_v_etype) < 0) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 427, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_Raise(__pyx_t_6, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __PYX_ERR(0, 428, __pyx_L1_error)
+  __PYX_ERR(0, 427, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":402
+  /* "_rtmidi.pyx":401
  * 
  * 
  * def _default_error_handler(etype, msg, data=None):             # <<<<<<<<<<<<<<
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rtmidi._rtmidi._default_error_handler", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi._default_error_handler", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":436
+/* "_rtmidi.pyx":435
  *     cdef object _deleted
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return NULL
  * 
  */
 
-static RtMidi *__pyx_f_6rtmidi_7_rtmidi_8MidiBase_baseptr(CYTHON_UNUSED struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self) {
+static RtMidi *__pyx_f_7_rtmidi_8MidiBase_baseptr(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self) {
   RtMidi *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("baseptr", 0);
 
-  /* "src/_rtmidi.pyx":437
+  /* "_rtmidi.pyx":436
  * 
  *     cdef RtMidi* baseptr(self):
  *         return NULL             # <<<<<<<<<<<<<<
  * 
  *     # context management
  */
   __pyx_r = NULL;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":436
+  /* "_rtmidi.pyx":435
  *     cdef object _deleted
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return NULL
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":440
+/* "_rtmidi.pyx":439
  * 
  *     # context management
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         """Support context manager protocol.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_1__enter__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase___enter__[] = "MidiBase.__enter__(self)\nSupport context manager protocol.\n\n        This means you can use ``MidiIn`` / ``MidiOut`` instances like this:\n\n        :\n\n            midiout = MidiIn()\n            midiout.open_port(0)\n\n            with midiout:\n                midiout.send_message([...])\n\n        and ``midiout.close_port()`` will be called automatically when exiting\n        the ``with`` block.\n\n        Since ``open_port()`` also returns the instance, you can even do:\n\n        :\n\n            midiout = MidiIn()\n\n            with midiout.open_port(0):\n                midiout.send_message([...])\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_1__enter__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_1__enter__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase___enter__[] = "MidiBase.__enter__(self)\nSupport context manager protocol.\n\n        This means you can use ``MidiIn`` / ``MidiOut`` instances like this:\n\n        :\n\n            midiout = MidiIn()\n            midiout.open_port(0)\n\n            with midiout:\n                midiout.send_message([...])\n\n        and ``midiout.close_port()`` will be called automatically when exiting\n        the ``with`` block.\n\n        Since ``open_port()`` also returns the instance, you can even do:\n\n        :\n\n            midiout = MidiIn()\n\n            with midiout.open_port(0):\n                midiout.send_message([...])\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_1__enter__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase___enter__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase___enter__(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase___enter__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase___enter__(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "src/_rtmidi.pyx":466
+  /* "_rtmidi.pyx":465
  * 
  *         """
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, *exc_info):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":440
+  /* "_rtmidi.pyx":439
  * 
  *     # context management
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         """Support context manager protocol.
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":468
+/* "_rtmidi.pyx":467
  *         return self
  * 
  *     def __exit__(self, *exc_info):             # <<<<<<<<<<<<<<
  *         """Support context manager protocol.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_3__exit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_2__exit__[] = "MidiBase.__exit__(self, *exc_info)\nSupport context manager protocol.\n\n        This method is called when using a ``MidiIn`` / ``MidiOut`` instance as\n        a context manager and closes open ports when exiting the ``with`` block.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_3__exit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_3__exit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_2__exit__[] = "MidiBase.__exit__(self, *exc_info)\nSupport context manager protocol.\n\n        This method is called when using a ``MidiIn`` / ``MidiOut`` instance as\n        a context manager and closes open ports when exiting the ``with`` block.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_3__exit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   CYTHON_UNUSED PyObject *__pyx_v_exc_info = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__exit__ (wrapper)", 0);
   if (unlikely(__pyx_kwds) && unlikely(PyDict_Size(__pyx_kwds) > 0) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__exit__", 0))) return NULL;
   __Pyx_INCREF(__pyx_args);
   __pyx_v_exc_info = __pyx_args;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_2__exit__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_exc_info);
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_2__exit__(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_exc_info);
 
   /* function exit code */
   __Pyx_XDECREF(__pyx_v_exc_info);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_2__exit__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_exc_info) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_2__exit__(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_exc_info) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "src/_rtmidi.pyx":475
+  /* "_rtmidi.pyx":474
  * 
  *         """
  *         self.close_port()             # <<<<<<<<<<<<<<
  * 
  *     def _check_port(self):
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 475, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":468
+  /* "_rtmidi.pyx":467
  *         return self
  * 
  *     def __exit__(self, *exc_info):             # <<<<<<<<<<<<<<
  *         """Support context manager protocol.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.__exit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":477
+/* "_rtmidi.pyx":476
  *         self.close_port()
  * 
  *     def _check_port(self):             # <<<<<<<<<<<<<<
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_5_check_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_4_check_port[] = "MidiBase._check_port(self)";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_5_check_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_5_check_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_4_check_port[] = "MidiBase._check_port(self)";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_5_check_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_check_port (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_4_check_port(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_4_check_port(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_4_check_port(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_4_check_port(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self) {
   PyObject *__pyx_v_inout = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -4436,97 +4535,97 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_check_port", 0);
 
-  /* "src/_rtmidi.pyx":478
+  /* "_rtmidi.pyx":477
  * 
  *     def _check_port(self):
  *         inout = "input" if isinstance(self, MidiIn) else "output"             # <<<<<<<<<<<<<<
  *         if self._port == -1:
  *             raise InvalidUseError("%r already opened virtual %s port." %
  */
-  __pyx_t_2 = __Pyx_TypeCheck(((PyObject *)__pyx_v_self), __pyx_ptype_6rtmidi_7_rtmidi_MidiIn); 
+  __pyx_t_2 = __Pyx_TypeCheck(((PyObject *)__pyx_v_self), __pyx_ptype_7_rtmidi_MidiIn); 
   if ((__pyx_t_2 != 0)) {
     __Pyx_INCREF(__pyx_n_u_input);
     __pyx_t_1 = __pyx_n_u_input;
   } else {
     __Pyx_INCREF(__pyx_n_u_output);
     __pyx_t_1 = __pyx_n_u_output;
   }
   __pyx_v_inout = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":479
+  /* "_rtmidi.pyx":478
  *     def _check_port(self):
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("%r already opened virtual %s port." %
  *                                   (self, inout))
  */
-  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_self->_port, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 479, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_EqObjC(__pyx_v_self->_port, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 479, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 478, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (unlikely(__pyx_t_2)) {
 
-    /* "src/_rtmidi.pyx":480
+    /* "_rtmidi.pyx":479
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:
  *             raise InvalidUseError("%r already opened virtual %s port." %             # <<<<<<<<<<<<<<
  *                                   (self, inout))
  *         elif self._port is not None:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 479, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 479, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_5 = 0;
     __pyx_t_6 = 127;
 
-    /* "src/_rtmidi.pyx":481
+    /* "_rtmidi.pyx":480
  *         if self._port == -1:
  *             raise InvalidUseError("%r already opened virtual %s port." %
  *                                   (self, inout))             # <<<<<<<<<<<<<<
  *         elif self._port is not None:
  *             raise InvalidUseError("%r already opened %s port %i." %
  */
-    __pyx_t_7 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(((PyObject *)__pyx_v_self)), __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 481, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(((PyObject *)__pyx_v_self)), __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 480, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_already_opened_virtual);
     __pyx_t_5 += 24;
     __Pyx_GIVEREF(__pyx_kp_u_already_opened_virtual);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_kp_u_already_opened_virtual);
-    __pyx_t_7 = __Pyx_PyUnicode_Unicode(__pyx_v_inout); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 481, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Unicode(__pyx_v_inout); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 480, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
     __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_7);
     PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_t_7);
     __pyx_t_7 = 0;
     __Pyx_INCREF(__pyx_kp_u_port);
     __pyx_t_5 += 6;
     __Pyx_GIVEREF(__pyx_kp_u_port);
     PyTuple_SET_ITEM(__pyx_t_4, 3, __pyx_kp_u_port);
 
-    /* "src/_rtmidi.pyx":480
+    /* "_rtmidi.pyx":479
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:
  *             raise InvalidUseError("%r already opened virtual %s port." %             # <<<<<<<<<<<<<<
  *                                   (self, inout))
  *         elif self._port is not None:
  */
-    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_4, 4, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 479, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4534,78 +4633,78 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_7);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 480, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 479, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 480, __pyx_L1_error)
+    __PYX_ERR(0, 479, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":479
+    /* "_rtmidi.pyx":478
  *     def _check_port(self):
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("%r already opened virtual %s port." %
  *                                   (self, inout))
  */
   }
 
-  /* "src/_rtmidi.pyx":482
+  /* "_rtmidi.pyx":481
  *             raise InvalidUseError("%r already opened virtual %s port." %
  *                                   (self, inout))
  *         elif self._port is not None:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("%r already opened %s port %i." %
  *                                   (self, inout, self._port))
  */
   __pyx_t_2 = (__pyx_v_self->_port != Py_None);
   __pyx_t_8 = (__pyx_t_2 != 0);
   if (unlikely(__pyx_t_8)) {
 
-    /* "src/_rtmidi.pyx":483
+    /* "_rtmidi.pyx":482
  *                                   (self, inout))
  *         elif self._port is not None:
  *             raise InvalidUseError("%r already opened %s port %i." %             # <<<<<<<<<<<<<<
  *                                   (self, inout, self._port))
  *         return inout
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 483, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
 
-    /* "src/_rtmidi.pyx":484
+    /* "_rtmidi.pyx":483
  *         elif self._port is not None:
  *             raise InvalidUseError("%r already opened %s port %i." %
  *                                   (self, inout, self._port))             # <<<<<<<<<<<<<<
  *         return inout
  * 
  */
-    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(3); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 483, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_INCREF(((PyObject *)__pyx_v_self));
     __Pyx_GIVEREF(((PyObject *)__pyx_v_self));
     PyTuple_SET_ITEM(__pyx_t_7, 0, ((PyObject *)__pyx_v_self));
     __Pyx_INCREF(__pyx_v_inout);
     __Pyx_GIVEREF(__pyx_v_inout);
     PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_v_inout);
     __Pyx_INCREF(__pyx_v_self->_port);
     __Pyx_GIVEREF(__pyx_v_self->_port);
     PyTuple_SET_ITEM(__pyx_t_7, 2, __pyx_v_self->_port);
 
-    /* "src/_rtmidi.pyx":483
+    /* "_rtmidi.pyx":482
  *                                   (self, inout))
  *         elif self._port is not None:
  *             raise InvalidUseError("%r already opened %s port %i." %             # <<<<<<<<<<<<<<
  *                                   (self, inout, self._port))
  *         return inout
  */
-    __pyx_t_4 = PyUnicode_Format(__pyx_kp_u_r_already_opened_s_port_i, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 483, __pyx_L1_error)
+    __pyx_t_4 = PyUnicode_Format(__pyx_kp_u_r_already_opened_s_port_i, __pyx_t_7); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __pyx_t_7 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_7)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
@@ -4613,77 +4712,77 @@
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_1 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_7, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 483, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 482, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 483, __pyx_L1_error)
+    __PYX_ERR(0, 482, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":482
+    /* "_rtmidi.pyx":481
  *             raise InvalidUseError("%r already opened virtual %s port." %
  *                                   (self, inout))
  *         elif self._port is not None:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("%r already opened %s port %i." %
  *                                   (self, inout, self._port))
  */
   }
 
-  /* "src/_rtmidi.pyx":485
+  /* "_rtmidi.pyx":484
  *             raise InvalidUseError("%r already opened %s port %i." %
  *                                   (self, inout, self._port))
  *         return inout             # <<<<<<<<<<<<<<
  * 
  *     def _decode_string(self, s, encoding='auto'):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_inout);
   __pyx_r = __pyx_v_inout;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":477
+  /* "_rtmidi.pyx":476
  *         self.close_port()
  * 
  *     def _check_port(self):             # <<<<<<<<<<<<<<
  *         inout = "input" if isinstance(self, MidiIn) else "output"
  *         if self._port == -1:
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase._check_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase._check_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_inout);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":487
+/* "_rtmidi.pyx":486
  *         return inout
  * 
  *     def _decode_string(self, s, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_7_decode_string(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_6_decode_string[] = "MidiBase._decode_string(self, s, encoding=u'auto')\nDecode given byte string with given encoding.";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_7_decode_string(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_7_decode_string(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_6_decode_string[] = "MidiBase._decode_string(self, s, encoding=u'auto')\nDecode given byte string with given encoding.";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_7_decode_string(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_s = 0;
   PyObject *__pyx_v_encoding = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -4712,15 +4811,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_decode_string") < 0)) __PYX_ERR(0, 487, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "_decode_string") < 0)) __PYX_ERR(0, 486, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -4728,28 +4827,28 @@
       }
     }
     __pyx_v_s = values[0];
     __pyx_v_encoding = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_decode_string", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 487, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_decode_string", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 486, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase._decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase._decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_6_decode_string(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_s, __pyx_v_encoding);
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_6_decode_string(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_s, __pyx_v_encoding);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_6_decode_string(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_s, PyObject *__pyx_v_encoding) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_6_decode_string(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_s, PyObject *__pyx_v_encoding) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_t_5;
@@ -4757,192 +4856,192 @@
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_decode_string", 0);
   __Pyx_INCREF(__pyx_v_encoding);
 
-  /* "src/_rtmidi.pyx":489
+  /* "_rtmidi.pyx":488
  *     def _decode_string(self, s, encoding='auto'):
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':             # <<<<<<<<<<<<<<
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'
  */
-  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_encoding, __pyx_n_u_auto, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_1 = (__Pyx_PyUnicode_Equals(__pyx_v_encoding, __pyx_n_u_auto, Py_EQ)); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 488, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "src/_rtmidi.pyx":490
+    /* "_rtmidi.pyx":489
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':
  *             if sys.platform.startswith('win'):             # <<<<<<<<<<<<<<
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_sys); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_sys); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_platform); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_platform); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_startswith); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_n_u_win) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_n_u_win);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 490, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 490, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 489, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (__pyx_t_1) {
 
-      /* "src/_rtmidi.pyx":491
+      /* "_rtmidi.pyx":490
  *         if encoding == 'auto':
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'             # <<<<<<<<<<<<<<
  *             elif (self.get_current_api() == API_MACOSX_CORE and
  *                   sys.platform == 'darwin'):
  */
       __Pyx_INCREF(__pyx_n_u_latin1);
       __Pyx_DECREF_SET(__pyx_v_encoding, __pyx_n_u_latin1);
 
-      /* "src/_rtmidi.pyx":490
+      /* "_rtmidi.pyx":489
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':
  *             if sys.platform.startswith('win'):             # <<<<<<<<<<<<<<
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and
  */
       goto __pyx_L4;
     }
 
-    /* "src/_rtmidi.pyx":492
+    /* "_rtmidi.pyx":491
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and             # <<<<<<<<<<<<<<
  *                   sys.platform == 'darwin'):
  *                 encoding = 'macroman'
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 492, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 491, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 491, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 491, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 491, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     if (__pyx_t_5) {
     } else {
       __pyx_t_1 = __pyx_t_5;
       goto __pyx_L5_bool_binop_done;
     }
 
-    /* "src/_rtmidi.pyx":493
+    /* "_rtmidi.pyx":492
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and
  *                   sys.platform == 'darwin'):             # <<<<<<<<<<<<<<
  *                 encoding = 'macroman'
  *             else:
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_sys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 493, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_sys); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 492, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_platform); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 493, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_platform); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_darwin, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 493, __pyx_L1_error)
+    __pyx_t_5 = (__Pyx_PyUnicode_Equals(__pyx_t_3, __pyx_n_u_darwin, Py_EQ)); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 492, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_1 = __pyx_t_5;
     __pyx_L5_bool_binop_done:;
 
-    /* "src/_rtmidi.pyx":492
+    /* "_rtmidi.pyx":491
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and             # <<<<<<<<<<<<<<
  *                   sys.platform == 'darwin'):
  *                 encoding = 'macroman'
  */
     if (__pyx_t_1) {
 
-      /* "src/_rtmidi.pyx":494
+      /* "_rtmidi.pyx":493
  *             elif (self.get_current_api() == API_MACOSX_CORE and
  *                   sys.platform == 'darwin'):
  *                 encoding = 'macroman'             # <<<<<<<<<<<<<<
  *             else:
  *                 encoding = 'utf-8'
  */
       __Pyx_INCREF(__pyx_n_u_macroman);
       __Pyx_DECREF_SET(__pyx_v_encoding, __pyx_n_u_macroman);
 
-      /* "src/_rtmidi.pyx":492
+      /* "_rtmidi.pyx":491
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'
  *             elif (self.get_current_api() == API_MACOSX_CORE and             # <<<<<<<<<<<<<<
  *                   sys.platform == 'darwin'):
  *                 encoding = 'macroman'
  */
       goto __pyx_L4;
     }
 
-    /* "src/_rtmidi.pyx":496
+    /* "_rtmidi.pyx":495
  *                 encoding = 'macroman'
  *             else:
  *                 encoding = 'utf-8'             # <<<<<<<<<<<<<<
  * 
  *         return s.decode(encoding, "ignore")
  */
     /*else*/ {
       __Pyx_INCREF(__pyx_kp_u_utf_8);
       __Pyx_DECREF_SET(__pyx_v_encoding, __pyx_kp_u_utf_8);
     }
     __pyx_L4:;
 
-    /* "src/_rtmidi.pyx":489
+    /* "_rtmidi.pyx":488
  *     def _decode_string(self, s, encoding='auto'):
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':             # <<<<<<<<<<<<<<
  *             if sys.platform.startswith('win'):
  *                 encoding = 'latin1'
  */
   }
 
-  /* "src/_rtmidi.pyx":498
+  /* "_rtmidi.pyx":497
  *                 encoding = 'utf-8'
  * 
  *         return s.decode(encoding, "ignore")             # <<<<<<<<<<<<<<
  * 
  *     def get_port_count(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 498, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_s, __pyx_n_s_decode); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 497, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_2 = NULL;
   __pyx_t_6 = 0;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_4);
@@ -4951,149 +5050,149 @@
       __Pyx_DECREF_SET(__pyx_t_4, function);
       __pyx_t_6 = 1;
     }
   }
   #if CYTHON_FAST_PYCALL
   if (PyFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_encoding, __pyx_n_u_ignore};
-    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   #if CYTHON_FAST_PYCCALL
   if (__Pyx_PyFastCFunction_Check(__pyx_t_4)) {
     PyObject *__pyx_temp[3] = {__pyx_t_2, __pyx_v_encoding, __pyx_n_u_ignore};
-    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyCFunction_FastCall(__pyx_t_4, __pyx_temp+1-__pyx_t_6, 2+__pyx_t_6); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_GOTREF(__pyx_t_3);
   } else
   #endif
   {
-    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2+__pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 497, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     if (__pyx_t_2) {
       __Pyx_GIVEREF(__pyx_t_2); PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_2); __pyx_t_2 = NULL;
     }
     __Pyx_INCREF(__pyx_v_encoding);
     __Pyx_GIVEREF(__pyx_v_encoding);
     PyTuple_SET_ITEM(__pyx_t_7, 0+__pyx_t_6, __pyx_v_encoding);
     __Pyx_INCREF(__pyx_n_u_ignore);
     __Pyx_GIVEREF(__pyx_n_u_ignore);
     PyTuple_SET_ITEM(__pyx_t_7, 1+__pyx_t_6, __pyx_n_u_ignore);
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 498, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_7, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 497, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":487
+  /* "_rtmidi.pyx":486
  *         return inout
  * 
  *     def _decode_string(self, s, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Decode given byte string with given encoding."""
  *         if encoding == 'auto':
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase._decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase._decode_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_encoding);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":500
+/* "_rtmidi.pyx":499
  *         return s.decode(encoding, "ignore")
  * 
  *     def get_port_count(self):             # <<<<<<<<<<<<<<
  *         """Return the number of available MIDI input or output ports."""
  *         return self.baseptr().getPortCount()
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_9get_port_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_8get_port_count[] = "MidiBase.get_port_count(self)\nReturn the number of available MIDI input or output ports.";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_9get_port_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_9get_port_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_8get_port_count[] = "MidiBase.get_port_count(self)\nReturn the number of available MIDI input or output ports.";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_9get_port_count(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_port_count (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_8get_port_count(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_8get_port_count(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_8get_port_count(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_8get_port_count(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   unsigned int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_port_count", 0);
 
-  /* "src/_rtmidi.pyx":502
+  /* "_rtmidi.pyx":501
  *     def get_port_count(self):
  *         """Return the number of available MIDI input or output ports."""
  *         return self.baseptr().getPortCount()             # <<<<<<<<<<<<<<
  * 
  *     def get_port_name(self, unsigned int port, encoding='auto'):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->getPortCount(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 502, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->getPortCount(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 501, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_unsigned_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 501, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":500
+  /* "_rtmidi.pyx":499
  *         return s.decode(encoding, "ignore")
  * 
  *     def get_port_count(self):             # <<<<<<<<<<<<<<
  *         """Return the number of available MIDI input or output ports."""
  *         return self.baseptr().getPortCount()
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.get_port_count", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.get_port_count", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":504
+/* "_rtmidi.pyx":503
  *         return self.baseptr().getPortCount()
  * 
  *     def get_port_name(self, unsigned int port, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Return the name of the MIDI input or output port with given number.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_11get_port_name(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_10get_port_name[] = "MidiBase.get_port_name(self, unsigned int port, encoding=u'auto')\nReturn the name of the MIDI input or output port with given number.\n\n        Ports are numbered from zero, separately for input and output ports.\n        The number of available ports is returned by the ``get_port_count``\n        method.\n\n        The port name is decoded to a (unicode) string with the encoding given\n        by ``encoding``. If ``encoding`` is ``\"auto\"`` (the default), then an\n        appropriate encoding is chosen based on the system and the used backend\n        API. If ``encoding`` is ``None``, the name is returned un-decoded, i.e.\n        as type ``str`` in Python 2 or ``bytes`` in Python 3.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_11get_port_name(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_11get_port_name(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_10get_port_name[] = "MidiBase.get_port_name(self, unsigned int port, encoding=u'auto')\nReturn the name of the MIDI input or output port with given number.\n\n        Ports are numbered from zero, separately for input and output ports.\n        The number of available ports is returned by the ``get_port_count``\n        method.\n\n        The port name is decoded to a (unicode) string with the encoding given\n        by ``encoding``. If ``encoding`` is ``\"auto\"`` (the default), then an\n        appropriate encoding is chosen based on the system and the used backend\n        API. If ``encoding`` is ``None``, the name is returned un-decoded, i.e.\n        as type ``str`` in Python 2 or ``bytes`` in Python 3.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_11get_port_name(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   unsigned int __pyx_v_port;
   PyObject *__pyx_v_encoding = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5122,44 +5221,44 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_port_name") < 0)) __PYX_ERR(0, 504, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_port_name") < 0)) __PYX_ERR(0, 503, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_port = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_port == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 504, __pyx_L3_error)
+    __pyx_v_port = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_port == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 503, __pyx_L3_error)
     __pyx_v_encoding = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_port_name", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 504, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_port_name", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 503, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.get_port_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.get_port_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_10get_port_name(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_port, __pyx_v_encoding);
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_10get_port_name(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_port, __pyx_v_encoding);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_10get_port_name(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, unsigned int __pyx_v_port, PyObject *__pyx_v_encoding) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_10get_port_name(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, unsigned int __pyx_v_port, PyObject *__pyx_v_encoding) {
   std::string __pyx_v_name;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   std::string __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
@@ -5170,51 +5269,51 @@
   int __pyx_t_9;
   PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_port_name", 0);
 
-  /* "src/_rtmidi.pyx":518
+  /* "_rtmidi.pyx":517
  * 
  *         """
  *         cdef string name = self.baseptr().getPortName(port)             # <<<<<<<<<<<<<<
  * 
  *         if len(name):
  */
-  __pyx_t_1 = ((struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->getPortName(__pyx_v_port); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 518, __pyx_L1_error)
+  __pyx_t_1 = ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->getPortName(__pyx_v_port); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 517, __pyx_L1_error)
   __pyx_v_name = __pyx_t_1;
 
-  /* "src/_rtmidi.pyx":520
+  /* "_rtmidi.pyx":519
  *         cdef string name = self.baseptr().getPortName(port)
  * 
  *         if len(name):             # <<<<<<<<<<<<<<
  *             return self._decode_string(name, encoding) if encoding else name
  * 
  */
-  __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_2 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 519, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_3 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 519, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = (__pyx_t_3 != 0);
   if (__pyx_t_4) {
 
-    /* "src/_rtmidi.pyx":521
+    /* "_rtmidi.pyx":520
  * 
  *         if len(name):
  *             return self._decode_string(name, encoding) if encoding else name             # <<<<<<<<<<<<<<
  * 
  *     def get_ports(self, encoding='auto'):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_encoding); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 521, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_v_encoding); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 520, __pyx_L1_error)
     if (__pyx_t_4) {
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode_string); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 521, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode_string); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 520, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 521, __pyx_L1_error)
+      __pyx_t_7 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 520, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       __pyx_t_9 = 0;
       if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
@@ -5223,68 +5322,68 @@
           __Pyx_DECREF_SET(__pyx_t_6, function);
           __pyx_t_9 = 1;
         }
       }
       #if CYTHON_FAST_PYCALL
       if (PyFunction_Check(__pyx_t_6)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_7, __pyx_v_encoding};
-        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       #if CYTHON_FAST_PYCCALL
       if (__Pyx_PyFastCFunction_Check(__pyx_t_6)) {
         PyObject *__pyx_temp[3] = {__pyx_t_8, __pyx_t_7, __pyx_v_encoding};
-        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyCFunction_FastCall(__pyx_t_6, __pyx_temp+1-__pyx_t_9, 2+__pyx_t_9); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
         __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       } else
       #endif
       {
-        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 521, __pyx_L1_error)
+        __pyx_t_10 = PyTuple_New(2+__pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 520, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (__pyx_t_8) {
           __Pyx_GIVEREF(__pyx_t_8); PyTuple_SET_ITEM(__pyx_t_10, 0, __pyx_t_8); __pyx_t_8 = NULL;
         }
         __Pyx_GIVEREF(__pyx_t_7);
         PyTuple_SET_ITEM(__pyx_t_10, 0+__pyx_t_9, __pyx_t_7);
         __Pyx_INCREF(__pyx_v_encoding);
         __Pyx_GIVEREF(__pyx_v_encoding);
         PyTuple_SET_ITEM(__pyx_t_10, 1+__pyx_t_9, __pyx_v_encoding);
         __pyx_t_7 = 0;
-        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_10, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_2 = __pyx_t_5;
       __pyx_t_5 = 0;
     } else {
-      __pyx_t_5 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 521, __pyx_L1_error)
+      __pyx_t_5 = __pyx_convert_PyBytes_string_to_py_std__in_string(__pyx_v_name); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 520, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __pyx_t_2 = __pyx_t_5;
       __pyx_t_5 = 0;
     }
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "src/_rtmidi.pyx":520
+    /* "_rtmidi.pyx":519
  *         cdef string name = self.baseptr().getPortName(port)
  * 
  *         if len(name):             # <<<<<<<<<<<<<<
  *             return self._decode_string(name, encoding) if encoding else name
  * 
  */
   }
 
-  /* "src/_rtmidi.pyx":504
+  /* "_rtmidi.pyx":503
  *         return self.baseptr().getPortCount()
  * 
  *     def get_port_name(self, unsigned int port, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Return the name of the MIDI input or output port with given number.
  * 
  */
 
@@ -5294,34 +5393,34 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_10);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.get_port_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.get_port_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":523
+/* "_rtmidi.pyx":522
  *             return self._decode_string(name, encoding) if encoding else name
  * 
  *     def get_ports(self, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Return a list of names of available MIDI input or output ports.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_13get_ports(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_12get_ports[] = "MidiBase.get_ports(self, encoding=u'auto')\nReturn a list of names of available MIDI input or output ports.\n\n        The list index of each port name corresponds to its port number.\n\n        The port names are decoded to (unicode) strings with the encoding given\n        by ``encoding``. If ``encoding`` is ``\"auto\"`` (the default), then an\n        appropriate encoding is chosen based on the system and the used backend\n        API. If ``encoding`` is ``None``, the names are returned un-decoded,\n        i.e. as type ``str`` in Python 2 or ``bytes`` in Python 3.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_13get_ports(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_13get_ports(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_12get_ports[] = "MidiBase.get_ports(self, encoding=u'auto')\nReturn a list of names of available MIDI input or output ports.\n\n        The list index of each port name corresponds to its port number.\n\n        The port names are decoded to (unicode) strings with the encoding given\n        by ``encoding``. If ``encoding`` is ``\"auto\"`` (the default), then an\n        appropriate encoding is chosen based on the system and the used backend\n        API. If ``encoding`` is ``None``, the names are returned un-decoded,\n        i.e. as type ``str`` in Python 2 or ``bytes`` in Python 3.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_13get_ports(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_encoding = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_ports (wrapper)", 0);
@@ -5343,42 +5442,42 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_encoding);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_ports") < 0)) __PYX_ERR(0, 523, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "get_ports") < 0)) __PYX_ERR(0, 522, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_encoding = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("get_ports", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 523, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("get_ports", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 522, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.get_ports", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.get_ports", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_12get_ports(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_encoding);
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_12get_ports(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_encoding);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_12get_ports(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_encoding) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_12get_ports(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_encoding) {
   PyObject *__pyx_8genexpr2__pyx_v_p = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -5387,122 +5486,122 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_ports", 0);
 
-  /* "src/_rtmidi.pyx":535
+  /* "_rtmidi.pyx":534
  * 
  *         """
  *         return [self.get_port_name(p, encoding=encoding)             # <<<<<<<<<<<<<<
  *                 for p in range(self.get_port_count())]
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 535, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 534, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "src/_rtmidi.pyx":536
+    /* "_rtmidi.pyx":535
  *         """
  *         return [self.get_port_name(p, encoding=encoding)
  *                 for p in range(self.get_port_count())]             # <<<<<<<<<<<<<<
  * 
  *     def is_port_open(self):
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_port_count); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 536, __pyx_L5_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_port_count); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 536, __pyx_L5_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 535, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 536, __pyx_L5_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
       __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2); __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 536, __pyx_L5_error)
+      __pyx_t_5 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 535, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 536, __pyx_L5_error)
+      __pyx_t_6 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 535, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 536, __pyx_L5_error)
+          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 535, __pyx_L5_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 536, __pyx_L5_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         } else {
           if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 536, __pyx_L5_error)
+          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_5); __Pyx_INCREF(__pyx_t_3); __pyx_t_5++; if (unlikely(0 < 0)) __PYX_ERR(0, 535, __pyx_L5_error)
           #else
-          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 536, __pyx_L5_error)
+          __pyx_t_3 = PySequence_ITEM(__pyx_t_2, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_6(__pyx_t_2);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 536, __pyx_L5_error)
+            else __PYX_ERR(0, 535, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_p, __pyx_t_3);
       __pyx_t_3 = 0;
 
-      /* "src/_rtmidi.pyx":535
+      /* "_rtmidi.pyx":534
  * 
  *         """
  *         return [self.get_port_name(p, encoding=encoding)             # <<<<<<<<<<<<<<
  *                 for p in range(self.get_port_count())]
  * 
  */
-      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_port_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 535, __pyx_L5_error)
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_port_name); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 534, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 535, __pyx_L5_error)
+      __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 534, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_8genexpr2__pyx_v_p);
       __Pyx_GIVEREF(__pyx_8genexpr2__pyx_v_p);
       PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_8genexpr2__pyx_v_p);
-      __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 535, __pyx_L5_error)
+      __pyx_t_7 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 534, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_7);
-      if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_encoding, __pyx_v_encoding) < 0) __PYX_ERR(0, 535, __pyx_L5_error)
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 535, __pyx_L5_error)
+      if (PyDict_SetItem(__pyx_t_7, __pyx_n_s_encoding, __pyx_v_encoding) < 0) __PYX_ERR(0, 534, __pyx_L5_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 534, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 535, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 534, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-      /* "src/_rtmidi.pyx":536
+      /* "_rtmidi.pyx":535
  *         """
  *         return [self.get_port_name(p, encoding=encoding)
  *                 for p in range(self.get_port_count())]             # <<<<<<<<<<<<<<
  * 
  *     def is_port_open(self):
  */
     }
@@ -5514,15 +5613,15 @@
     goto __pyx_L1_error;
     __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":523
+  /* "_rtmidi.pyx":522
  *             return self._decode_string(name, encoding) if encoding else name
  * 
  *     def get_ports(self, encoding='auto'):             # <<<<<<<<<<<<<<
  *         """Return a list of names of available MIDI input or output ports.
  * 
  */
 
@@ -5530,101 +5629,101 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.get_ports", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.get_ports", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_p);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":538
+/* "_rtmidi.pyx":537
  *                 for p in range(self.get_port_count())]
  * 
  *     def is_port_open(self):             # <<<<<<<<<<<<<<
  *         """Return ``True`` if a port has been opened and ``False`` if not.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_15is_port_open(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_14is_port_open[] = "MidiBase.is_port_open(self)\nReturn ``True`` if a port has been opened and ``False`` if not.\n\n        .. note::\n            The ``isPortOpen`` method of the RtMidi C++ library does not\n            return ``True`` when a virtual port has been openend. The\n            python-rtmidi implementation, on the other hand, does.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_15is_port_open(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_15is_port_open(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_14is_port_open[] = "MidiBase.is_port_open(self)\nReturn ``True`` if a port has been opened and ``False`` if not.\n\n        .. note::\n            The ``isPortOpen`` method of the RtMidi C++ library does not\n            return ``True`` when a virtual port has been openend. The\n            python-rtmidi implementation, on the other hand, does.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_15is_port_open(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_port_open (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_14is_port_open(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_14is_port_open(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_14is_port_open(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_14is_port_open(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("is_port_open", 0);
 
-  /* "src/_rtmidi.pyx":547
+  /* "_rtmidi.pyx":546
  * 
  *         """
  *         return self._port is not None             # <<<<<<<<<<<<<<
  * 
  *     def open_port(self, unsigned int port=0, name=None):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = (__pyx_v_self->_port != Py_None);
-  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 547, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBool_FromLong(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 546, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":538
+  /* "_rtmidi.pyx":537
  *                 for p in range(self.get_port_count())]
  * 
  *     def is_port_open(self):             # <<<<<<<<<<<<<<
  *         """Return ``True`` if a port has been opened and ``False`` if not.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.is_port_open", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.is_port_open", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":549
+/* "_rtmidi.pyx":548
  *         return self._port is not None
  * 
  *     def open_port(self, unsigned int port=0, name=None):             # <<<<<<<<<<<<<<
  *         """Open the MIDI input or output port with the given port number.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_17open_port(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_16open_port[] = "MidiBase.open_port(self, unsigned int port=0, name=None)\nOpen the MIDI input or output port with the given port number.\n\n        Only one port can be opened per ``MidiIn`` or ``MidiOut`` instance. An\n        ``InvalidUseError`` exception is raised if an attempt is made to open a\n        port on a ``MidiIn`` or ``MidiOut`` instance, which already opened a\n        (virtual) port.\n\n        You can optionally pass a name for the RtMidi port with the ``name``\n        keyword or the second positional argument. Names with non-ASCII\n        characters in them have to be passed as unicode or UTF-8 encoded\n        strings in Python 2. The default name is \"RtMidi input\" resp. \"RtMidi\n        output\".\n\n        .. note::\n            Closing a port and opening it again with a different name does not\n            change the port name. To change the port name, use the\n            ``set_port_name`` method where supported, or delete its instance,\n            create a new one and open the port again giving a different name.\n\n        Exceptions:\n\n        ``InvalidPortError``\n            Raised when an invalid port number is passed.\n        ``InvalidUseError``\n            Raised when trying to open a MIDI port when a (virtual) port has\n            already been opened by this instance.\n        ``TypeError``\n            Raised when an incompatible value type is passed for the ``port``\n            or ``name`` parameter.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_17open_port(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_17open_port(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_16open_port[] = "MidiBase.open_port(self, unsigned int port=0, name=None)\nOpen the MIDI input or output port with the given port number.\n\n        Only one port can be opened per ``MidiIn`` or ``MidiOut`` instance. An\n        ``InvalidUseError`` exception is raised if an attempt is made to open a\n        port on a ``MidiIn`` or ``MidiOut`` instance, which already opened a\n        (virtual) port.\n\n        You can optionally pass a name for the RtMidi port with the ``name``\n        keyword or the second positional argument. Names with non-ASCII\n        characters in them have to be passed as unicode or UTF-8 encoded\n        strings in Python 2. The default name is \"RtMidi input\" resp. \"RtMidi\n        output\".\n\n        .. note::\n            Closing a port and opening it again with a different name does not\n            change the port name. To change the port name, use the\n            ``set_port_name`` method where supported, or delete its instance,\n            create a new one and open the port again giving a different name.\n\n        Exceptions:\n\n        ``InvalidPortError``\n            Raised when an invalid port number is passed.\n        ``InvalidUseError``\n            Raised when trying to open a MIDI port when a (virtual) port has\n            already been opened by this instance.\n        ``TypeError``\n            Raised when an incompatible value type is passed for the ``port``\n            or ``name`` parameter.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_17open_port(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   unsigned int __pyx_v_port;
   PyObject *__pyx_v_name = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -5655,49 +5754,49 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open_port") < 0)) __PYX_ERR(0, 549, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open_port") < 0)) __PYX_ERR(0, 548, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_port = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_port == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 549, __pyx_L3_error)
+      __pyx_v_port = __Pyx_PyInt_As_unsigned_int(values[0]); if (unlikely((__pyx_v_port == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 548, __pyx_L3_error)
     } else {
       __pyx_v_port = ((unsigned int)0);
     }
     __pyx_v_name = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("open_port", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 549, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("open_port", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 548, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.open_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.open_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_16open_port(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_port, __pyx_v_name);
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_16open_port(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_port, __pyx_v_name);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_16open_port(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, unsigned int __pyx_v_port, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_16open_port(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, unsigned int __pyx_v_port, PyObject *__pyx_v_name) {
   PyObject *__pyx_v_inout = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
@@ -5705,163 +5804,163 @@
   std::string __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open_port", 0);
   __Pyx_INCREF(__pyx_v_name);
 
-  /* "src/_rtmidi.pyx":581
+  /* "_rtmidi.pyx":580
  * 
  *         """
  *         inout = self._check_port()             # <<<<<<<<<<<<<<
  * 
  *         if name is None:
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_check_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 581, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_check_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 581, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 580, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_inout = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":583
+  /* "_rtmidi.pyx":582
  *         inout = self._check_port()
  * 
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidi %s" % inout
  * 
  */
   __pyx_t_4 = (__pyx_v_name == Py_None);
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (__pyx_t_5) {
 
-    /* "src/_rtmidi.pyx":584
+    /* "_rtmidi.pyx":583
  * 
  *         if name is None:
  *             name = "RtMidi %s" % inout             # <<<<<<<<<<<<<<
  * 
  *         self.baseptr().openPort(port, _to_bytes(name))
  */
-    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_RtMidi_s, __pyx_v_inout); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 584, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_RtMidi_s, __pyx_v_inout); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 583, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF_SET(__pyx_v_name, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "src/_rtmidi.pyx":583
+    /* "_rtmidi.pyx":582
  *         inout = self._check_port()
  * 
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidi %s" % inout
  * 
  */
   }
 
-  /* "src/_rtmidi.pyx":586
+  /* "_rtmidi.pyx":585
  *             name = "RtMidi %s" % inout
  * 
  *         self.baseptr().openPort(port, _to_bytes(name))             # <<<<<<<<<<<<<<
  *         self._port = port
  *         return self
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 586, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 585, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 586, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 585, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  ((struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->openPort(__pyx_v_port, __pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 586, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->openPort(__pyx_v_port, __pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 585, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":587
+  /* "_rtmidi.pyx":586
  * 
  *         self.baseptr().openPort(port, _to_bytes(name))
  *         self._port = port             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_unsigned_int(__pyx_v_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 587, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_unsigned_int(__pyx_v_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 586, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_port);
   __Pyx_DECREF(__pyx_v_self->_port);
   __pyx_v_self->_port = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":588
+  /* "_rtmidi.pyx":587
  *         self.baseptr().openPort(port, _to_bytes(name))
  *         self._port = port
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def open_virtual_port(self, name=None):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":549
+  /* "_rtmidi.pyx":548
  *         return self._port is not None
  * 
  *     def open_port(self, unsigned int port=0, name=None):             # <<<<<<<<<<<<<<
  *         """Open the MIDI input or output port with the given port number.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.open_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.open_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_inout);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":590
+/* "_rtmidi.pyx":589
  *         return self
  * 
  *     def open_virtual_port(self, name=None):             # <<<<<<<<<<<<<<
  *         """Open a virtual MIDI input or output port.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_19open_virtual_port(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_18open_virtual_port[] = "MidiBase.open_virtual_port(self, name=None)\nOpen a virtual MIDI input or output port.\n\n        Only one port can be opened per ``MidiIn`` or ``MidiOut`` instance. An\n        ``InvalidUseError`` exception is raised if an attempt is made to open a\n        port on a ``MidiIn`` or ``MidiOut`` instance, which already opened a\n        (virtual) port.\n\n        A virtual port is not connected to a physical MIDI device or system\n        port when first opened. You can connect it to another MIDI output with\n        the OS-dependent tools provided by the low-level MIDI framework, e.g.\n        ``aconnect`` for ALSA, ``jack_connect`` for JACK, or the Audio & MIDI\n        settings dialog for CoreMIDI.\n\n        .. note::\n            Virtual ports are not supported by some backend APIs, namely the\n            Windows MultiMedia API. You can use special MIDI drivers like `MIDI\n            Yoke`_ or loopMIDI_ to provide hardware-independent virtual MIDI\n            ports as an alternative.\n\n        You can optionally pass a name for the RtMidi port with the ``name``\n        keyword or the second positional argument. Names with non-ASCII\n        characters in them have to be passed as unicode or UTF-8 encoded\n        strings in Python 2. The default name is \"RtMidi virtual input\" resp.\n        \"RtMidi virtual output\".\n\n        .. note::\n            Closing a port and opening it again with a different name does not\n            change the port name. To change the port name, use the\n            ``set_port_name`` method where supported, or delete its instance,\n            create a new one and open the port again giving a different name.\n\n            Also, to close a virtual input port, you have to delete its\n            ``MidiIn`` or ``MidiOut`` instance.\n\n        Exceptions:\n\n        ``InvalidUseError``\n            Raised when trying to open a virtual port when a (virtual) port has\n            already been opened by this instance.\n        ``Typ""eError``\n            Raised when an incompatible value type is passed for the ``name``\n            parameter.\n        ``UnsupportedOperationError``\n            Raised when trying to open a virtual MIDI port with the Windows\n            MultiMedia API, which doesn't support virtual ports.\n\n        .. _midi yoke: http://www.midiox.com/myoke.htm\n        .. _loopmidi: http://www.tobias-erichsen.de/software/loopmidi.html\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_19open_virtual_port(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_19open_virtual_port(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_18open_virtual_port[] = "MidiBase.open_virtual_port(self, name=None)\nOpen a virtual MIDI input or output port.\n\n        Only one port can be opened per ``MidiIn`` or ``MidiOut`` instance. An\n        ``InvalidUseError`` exception is raised if an attempt is made to open a\n        port on a ``MidiIn`` or ``MidiOut`` instance, which already opened a\n        (virtual) port.\n\n        A virtual port is not connected to a physical MIDI device or system\n        port when first opened. You can connect it to another MIDI output with\n        the OS-dependent tools provided by the low-level MIDI framework, e.g.\n        ``aconnect`` for ALSA, ``jack_connect`` for JACK, or the Audio & MIDI\n        settings dialog for CoreMIDI.\n\n        .. note::\n            Virtual ports are not supported by some backend APIs, namely the\n            Windows MultiMedia API. You can use special MIDI drivers like `MIDI\n            Yoke`_ or loopMIDI_ to provide hardware-independent virtual MIDI\n            ports as an alternative.\n\n        You can optionally pass a name for the RtMidi port with the ``name``\n        keyword or the second positional argument. Names with non-ASCII\n        characters in them have to be passed as unicode or UTF-8 encoded\n        strings in Python 2. The default name is \"RtMidi virtual input\" resp.\n        \"RtMidi virtual output\".\n\n        .. note::\n            Closing a port and opening it again with a different name does not\n            change the port name. To change the port name, use the\n            ``set_port_name`` method where supported, or delete its instance,\n            create a new one and open the port again giving a different name.\n\n            Also, to close a virtual input port, you have to delete its\n            ``MidiIn`` or ``MidiOut`` instance.\n\n        Exceptions:\n\n        ``InvalidUseError``\n            Raised when trying to open a virtual port when a (virtual) port has\n            already been opened by this instance.\n        ``Typ""eError``\n            Raised when an incompatible value type is passed for the ``name``\n            parameter.\n        ``UnsupportedOperationError``\n            Raised when trying to open a virtual MIDI port with the Windows\n            MultiMedia API, which doesn't support virtual ports.\n\n        .. _midi yoke: http://www.midiox.com/myoke.htm\n        .. _loopmidi: http://www.tobias-erichsen.de/software/loopmidi.html\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_19open_virtual_port(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_name = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("open_virtual_port (wrapper)", 0);
@@ -5883,172 +5982,172 @@
         case  0:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name);
           if (value) { values[0] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open_virtual_port") < 0)) __PYX_ERR(0, 590, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "open_virtual_port") < 0)) __PYX_ERR(0, 589, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_name = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("open_virtual_port", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 590, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("open_virtual_port", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 589, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.open_virtual_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.open_virtual_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_18open_virtual_port(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_name);
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_18open_virtual_port(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_name);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_18open_virtual_port(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_18open_virtual_port(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_v_inout = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   std::string __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("open_virtual_port", 0);
 
-  /* "src/_rtmidi.pyx":641
+  /* "_rtmidi.pyx":640
  * 
  *         """
  *         if self.get_current_api() == API_WINDOWS_MM:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError("Virtual ports are not supported "
  *                                       "by the Windows MultiMedia API.")
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 641, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 641, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 641, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 641, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 641, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_4 < 0)) __PYX_ERR(0, 640, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (unlikely(__pyx_t_4)) {
 
-    /* "src/_rtmidi.pyx":642
+    /* "_rtmidi.pyx":641
  *         """
  *         if self.get_current_api() == API_WINDOWS_MM:
  *             raise NotImplementedError("Virtual ports are not supported "             # <<<<<<<<<<<<<<
  *                                       "by the Windows MultiMedia API.")
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 642, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 641, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 642, __pyx_L1_error)
+    __PYX_ERR(0, 641, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":641
+    /* "_rtmidi.pyx":640
  * 
  *         """
  *         if self.get_current_api() == API_WINDOWS_MM:             # <<<<<<<<<<<<<<
  *             raise NotImplementedError("Virtual ports are not supported "
  *                                       "by the Windows MultiMedia API.")
  */
   }
 
-  /* "src/_rtmidi.pyx":645
+  /* "_rtmidi.pyx":644
  *                                       "by the Windows MultiMedia API.")
  * 
  *         inout = self._check_port()             # <<<<<<<<<<<<<<
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)
  *                                                 if name is None else name))
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_check_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 645, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_check_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_1)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_1);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_3 = (__pyx_t_1) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 645, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 644, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_inout = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "src/_rtmidi.pyx":646
+  /* "_rtmidi.pyx":645
  * 
  *         inout = self._check_port()
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)             # <<<<<<<<<<<<<<
  *                                                 if name is None else name))
  *         self._port = -1
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 646, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
 
-  /* "src/_rtmidi.pyx":647
+  /* "_rtmidi.pyx":646
  *         inout = self._check_port()
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)
  *                                                 if name is None else name))             # <<<<<<<<<<<<<<
  *         self._port = -1
  *         return self
  */
   __pyx_t_4 = (__pyx_v_name == Py_None);
   if ((__pyx_t_4 != 0)) {
 
-    /* "src/_rtmidi.pyx":646
+    /* "_rtmidi.pyx":645
  * 
  *         inout = self._check_port()
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)             # <<<<<<<<<<<<<<
  *                                                 if name is None else name))
  *         self._port = -1
  */
-    __pyx_t_5 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_RtMidi_virtual_s, __pyx_v_inout); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 646, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_FormatSafe(__pyx_kp_u_RtMidi_virtual_s, __pyx_v_inout); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 645, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_1 = __pyx_t_5;
     __pyx_t_5 = 0;
   } else {
 
-    /* "src/_rtmidi.pyx":647
+    /* "_rtmidi.pyx":646
  *         inout = self._check_port()
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)
  *                                                 if name is None else name))             # <<<<<<<<<<<<<<
  *         self._port = -1
  *         return self
  */
     __Pyx_INCREF(__pyx_v_name);
@@ -6063,572 +6162,572 @@
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_1) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 646, __pyx_L1_error)
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "src/_rtmidi.pyx":646
+  /* "_rtmidi.pyx":645
  * 
  *         inout = self._check_port()
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)             # <<<<<<<<<<<<<<
  *                                                 if name is None else name))
  *         self._port = -1
  */
-  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 646, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 645, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  ((struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->openVirtualPort(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 646, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->openVirtualPort(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 645, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":648
+  /* "_rtmidi.pyx":647
  *         self.baseptr().openVirtualPort(_to_bytes(("RtMidi virtual %s" % inout)
  *                                                 if name is None else name))
  *         self._port = -1             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
   __Pyx_GOTREF(__pyx_v_self->_port);
   __Pyx_DECREF(__pyx_v_self->_port);
   __pyx_v_self->_port = __pyx_int_neg_1;
 
-  /* "src/_rtmidi.pyx":649
+  /* "_rtmidi.pyx":648
  *                                                 if name is None else name))
  *         self._port = -1
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def close_port(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_self));
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":590
+  /* "_rtmidi.pyx":589
  *         return self
  * 
  *     def open_virtual_port(self, name=None):             # <<<<<<<<<<<<<<
  *         """Open a virtual MIDI input or output port.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.open_virtual_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.open_virtual_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_inout);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":651
+/* "_rtmidi.pyx":650
  *         return self
  * 
  *     def close_port(self):             # <<<<<<<<<<<<<<
  *         """Close the MIDI input or output port opened via ``open_port``.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_21close_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_20close_port[] = "MidiBase.close_port(self)\nClose the MIDI input or output port opened via ``open_port``.\n\n        It is safe to call this method repeatedly or if no port has been opened\n        (yet) by this instance.\n\n        Also cancels a callback function set with ``set_callback``.\n\n        To close a virtual port opened via ``open_virtual_port``, you have to\n        delete its ``MidiIn`` or ``MidiOut`` instance.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_21close_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_21close_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_20close_port[] = "MidiBase.close_port(self)\nClose the MIDI input or output port opened via ``open_port``.\n\n        It is safe to call this method repeatedly or if no port has been opened\n        (yet) by this instance.\n\n        Also cancels a callback function set with ``set_callback``.\n\n        To close a virtual port opened via ``open_virtual_port``, you have to\n        delete its ``MidiIn`` or ``MidiOut`` instance.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_21close_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close_port (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_20close_port(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_20close_port(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_20close_port(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_20close_port(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close_port", 0);
 
-  /* "src/_rtmidi.pyx":663
+  /* "_rtmidi.pyx":662
  * 
  *         """
  *         if self._port != -1:             # <<<<<<<<<<<<<<
  *             self._port = None
  *         self.baseptr().closePort()
  */
-  __pyx_t_1 = __Pyx_PyInt_NeObjC(__pyx_v_self->_port, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 663, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_NeObjC(__pyx_v_self->_port, __pyx_int_neg_1, -1L, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 662, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 663, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(0, 662, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "src/_rtmidi.pyx":664
+    /* "_rtmidi.pyx":663
  *         """
  *         if self._port != -1:
  *             self._port = None             # <<<<<<<<<<<<<<
  *         self.baseptr().closePort()
  * 
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->_port);
     __Pyx_DECREF(__pyx_v_self->_port);
     __pyx_v_self->_port = Py_None;
 
-    /* "src/_rtmidi.pyx":663
+    /* "_rtmidi.pyx":662
  * 
  *         """
  *         if self._port != -1:             # <<<<<<<<<<<<<<
  *             self._port = None
  *         self.baseptr().closePort()
  */
   }
 
-  /* "src/_rtmidi.pyx":665
+  /* "_rtmidi.pyx":664
  *         if self._port != -1:
  *             self._port = None
  *         self.baseptr().closePort()             # <<<<<<<<<<<<<<
  * 
  *     def set_client_name(self, name):
  */
-  ((struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->closePort(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 665, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->closePort(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 664, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":651
+  /* "_rtmidi.pyx":650
  *         return self
  * 
  *     def close_port(self):             # <<<<<<<<<<<<<<
  *         """Close the MIDI input or output port opened via ``open_port``.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.close_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.close_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":667
+/* "_rtmidi.pyx":666
  *         self.baseptr().closePort()
  * 
  *     def set_client_name(self, name):             # <<<<<<<<<<<<<<
  *         """Set the name of the MIDI client.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_23set_client_name(PyObject *__pyx_v_self, PyObject *__pyx_v_name); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_22set_client_name[] = "MidiBase.set_client_name(self, name)\nSet the name of the MIDI client.\n\n        Names with non-ASCII characters in them have to be passed as unicode\n        or UTF-8 encoded strings in Python 2.\n\n        Currently only supported by the ALSA API backend.\n\n        Exceptions:\n\n        ``TypeError``\n            Raised when an incompatible value type is passed for the ``name``\n            parameter.\n        ``UnsupportedOperationError``\n            Raised when trying the backend API does not support changing the\n            client name.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_23set_client_name(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_23set_client_name(PyObject *__pyx_v_self, PyObject *__pyx_v_name); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_22set_client_name[] = "MidiBase.set_client_name(self, name)\nSet the name of the MIDI client.\n\n        Names with non-ASCII characters in them have to be passed as unicode\n        or UTF-8 encoded strings in Python 2.\n\n        Currently only supported by the ALSA API backend.\n\n        Exceptions:\n\n        ``TypeError``\n            Raised when an incompatible value type is passed for the ``name``\n            parameter.\n        ``UnsupportedOperationError``\n            Raised when trying the backend API does not support changing the\n            client name.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_23set_client_name(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_client_name (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_22set_client_name(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self), ((PyObject *)__pyx_v_name));
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_22set_client_name(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), ((PyObject *)__pyx_v_name));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_22set_client_name(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_22set_client_name(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   std::string __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_client_name", 0);
 
-  /* "src/_rtmidi.pyx":685
+  /* "_rtmidi.pyx":684
  * 
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_UNIX_JACK, API_WINDOWS_MM):             # <<<<<<<<<<<<<<
  *             raise NotImplementedError(
  *                 "API backend does not support changing the client name.")
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 685, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_UNIX_JACK); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_UNIX_JACK); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 685, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 684, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_4 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "src/_rtmidi.pyx":686
+    /* "_rtmidi.pyx":685
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_UNIX_JACK, API_WINDOWS_MM):
  *             raise NotImplementedError(             # <<<<<<<<<<<<<<
  *                 "API backend does not support changing the client name.")
  * 
  */
-    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 686, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_NotImplementedError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 685, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 686, __pyx_L1_error)
+    __PYX_ERR(0, 685, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":685
+    /* "_rtmidi.pyx":684
  * 
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_UNIX_JACK, API_WINDOWS_MM):             # <<<<<<<<<<<<<<
  *             raise NotImplementedError(
  *                 "API backend does not support changing the client name.")
  */
   }
 
-  /* "src/_rtmidi.pyx":689
+  /* "_rtmidi.pyx":688
  *                 "API backend does not support changing the client name.")
  * 
  *         self.baseptr().setClientName(_to_bytes(name))             # <<<<<<<<<<<<<<
  * 
  *     def set_port_name(self, name):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 689, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 688, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_2 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
     if (likely(__pyx_t_2)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
       __Pyx_INCREF(__pyx_t_2);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_3, function);
     }
   }
   __pyx_t_1 = (__pyx_t_2) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_2, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 689, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 688, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 689, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 688, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  ((struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setClientName(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 689, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setClientName(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 688, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":667
+  /* "_rtmidi.pyx":666
  *         self.baseptr().closePort()
  * 
  *     def set_client_name(self, name):             # <<<<<<<<<<<<<<
  *         """Set the name of the MIDI client.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.set_client_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.set_client_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":691
+/* "_rtmidi.pyx":690
  *         self.baseptr().setClientName(_to_bytes(name))
  * 
  *     def set_port_name(self, name):             # <<<<<<<<<<<<<<
  *         """Set the name of the currently opened port.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_25set_port_name(PyObject *__pyx_v_self, PyObject *__pyx_v_name); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_24set_port_name[] = "MidiBase.set_port_name(self, name)\nSet the name of the currently opened port.\n\n        Names with non-ASCII characters in them have to be passed as unicode\n        or UTF-8 encoded strings in Python 2.\n\n        Currently only supported by the ALSA and JACK API backends.\n\n        Exceptions:\n\n        ``InvalidUseError``\n            Raised when no port is currently opened.\n        ``TypeError``\n            Raised when an incompatible value type is passed for the ``name``\n            parameter.\n        ``UnsupportedOperationError``\n            Raised when trying the backend API does not support changing the\n            port name.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_25set_port_name(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_25set_port_name(PyObject *__pyx_v_self, PyObject *__pyx_v_name); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_24set_port_name[] = "MidiBase.set_port_name(self, name)\nSet the name of the currently opened port.\n\n        Names with non-ASCII characters in them have to be passed as unicode\n        or UTF-8 encoded strings in Python 2.\n\n        Currently only supported by the ALSA and JACK API backends.\n\n        Exceptions:\n\n        ``InvalidUseError``\n            Raised when no port is currently opened.\n        ``TypeError``\n            Raised when an incompatible value type is passed for the ``name``\n            parameter.\n        ``UnsupportedOperationError``\n            Raised when trying the backend API does not support changing the\n            port name.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_25set_port_name(PyObject *__pyx_v_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_port_name (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_24set_port_name(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self), ((PyObject *)__pyx_v_name));
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_24set_port_name(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), ((PyObject *)__pyx_v_name));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_24set_port_name(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_24set_port_name(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_name) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_t_5;
   std::string __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_port_name", 0);
 
-  /* "src/_rtmidi.pyx":711
+  /* "_rtmidi.pyx":710
  * 
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_WINDOWS_MM):             # <<<<<<<<<<<<<<
  *             raise UnsupportedOperationError(
  *                 "API backend does not support changing the port name.")
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_get_current_api); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 711, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_API_MACOSX_CORE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_3 = PyObject_RichCompare(__pyx_t_1, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (!__pyx_t_5) {
   } else {
     __pyx_t_4 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_API_WINDOWS_MM); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 711, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_5 < 0)) __PYX_ERR(0, 710, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_4 = __pyx_t_5;
   __pyx_L4_bool_binop_done:;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_5 = (__pyx_t_4 != 0);
   if (unlikely(__pyx_t_5)) {
 
-    /* "src/_rtmidi.pyx":712
+    /* "_rtmidi.pyx":711
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_WINDOWS_MM):
  *             raise UnsupportedOperationError(             # <<<<<<<<<<<<<<
  *                 "API backend does not support changing the port name.")
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UnsupportedOperationError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 712, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_UnsupportedOperationError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 711, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_API_backend_does_not_support_cha_2) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_API_backend_does_not_support_cha_2);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 712, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 711, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 712, __pyx_L1_error)
+    __PYX_ERR(0, 711, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":711
+    /* "_rtmidi.pyx":710
  * 
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_WINDOWS_MM):             # <<<<<<<<<<<<<<
  *             raise UnsupportedOperationError(
  *                 "API backend does not support changing the port name.")
  */
   }
 
-  /* "src/_rtmidi.pyx":715
+  /* "_rtmidi.pyx":714
  *                 "API backend does not support changing the port name.")
  * 
  *         if self._port is None:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("No port currently opened.")
  * 
  */
   __pyx_t_5 = (__pyx_v_self->_port == Py_None);
   __pyx_t_4 = (__pyx_t_5 != 0);
   if (unlikely(__pyx_t_4)) {
 
-    /* "src/_rtmidi.pyx":716
+    /* "_rtmidi.pyx":715
  * 
  *         if self._port is None:
  *             raise InvalidUseError("No port currently opened.")             # <<<<<<<<<<<<<<
  * 
  *         self.baseptr().setPortName(_to_bytes(name))
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 716, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_InvalidUseError); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 715, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_t_3 = NULL;
     if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
       __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
       if (likely(__pyx_t_3)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
         __Pyx_INCREF(__pyx_t_3);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_2, function);
       }
     }
     __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_kp_u_No_port_currently_opened) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_kp_u_No_port_currently_opened);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 716, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 715, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_Raise(__pyx_t_1, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __PYX_ERR(0, 716, __pyx_L1_error)
+    __PYX_ERR(0, 715, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":715
+    /* "_rtmidi.pyx":714
  *                 "API backend does not support changing the port name.")
  * 
  *         if self._port is None:             # <<<<<<<<<<<<<<
  *             raise InvalidUseError("No port currently opened.")
  * 
  */
   }
 
-  /* "src/_rtmidi.pyx":718
+  /* "_rtmidi.pyx":717
  *             raise InvalidUseError("No port currently opened.")
  * 
  *         self.baseptr().setPortName(_to_bytes(name))             # <<<<<<<<<<<<<<
  * 
  *     def set_error_callback(self, func, data=None):
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 718, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 717, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v_name);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 718, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 717, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 718, __pyx_L1_error)
+  __pyx_t_6 = __pyx_convert_string_from_py_std__in_string(__pyx_t_1); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 717, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  ((struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setPortName(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 718, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setPortName(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 717, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":691
+  /* "_rtmidi.pyx":690
  *         self.baseptr().setClientName(_to_bytes(name))
  * 
  *     def set_port_name(self, name):             # <<<<<<<<<<<<<<
  *         """Set the name of the currently opened port.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.set_port_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.set_port_name", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":720
+/* "_rtmidi.pyx":719
  *         self.baseptr().setPortName(_to_bytes(name))
  * 
  *     def set_error_callback(self, func, data=None):             # <<<<<<<<<<<<<<
  *         """Register a callback function for errors.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_27set_error_callback(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_26set_error_callback[] = "MidiBase.set_error_callback(self, func, data=None)\nRegister a callback function for errors.\n\n        The callback function is called when an error occurs and must take\n        three arguments. The first argument is a member of enum\n        ``RtMidiError::Type``, represented by one of the ``ERRORTYPE_*``\n        constants. The second argument is an error message. The third argument\n        is the value of the ``data`` argument passed to this function when the\n        callback is registered.\n\n        .. note::\n            A default error handler function is registered on new instances of\n            ``MidiIn`` and ``MidiOut``, which turns errors reported by the C++\n            layer into custom exceptions derived from ``RtMidiError``.\n\n            If you replace this default error handler, be aware that the\n            exception handling in your code probably needs to be adapted.\n\n        Registering an error callback function replaces any previously\n        registered error callback, including the above mentioned default error\n        handler.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_27set_error_callback(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_27set_error_callback(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_26set_error_callback[] = "MidiBase.set_error_callback(self, func, data=None)\nRegister a callback function for errors.\n\n        The callback function is called when an error occurs and must take\n        three arguments. The first argument is a member of enum\n        ``RtMidiError::Type``, represented by one of the ``ERRORTYPE_*``\n        constants. The second argument is an error message. The third argument\n        is the value of the ``data`` argument passed to this function when the\n        callback is registered.\n\n        .. note::\n            A default error handler function is registered on new instances of\n            ``MidiIn`` and ``MidiOut``, which turns errors reported by the C++\n            layer into custom exceptions derived from ``RtMidiError``.\n\n            If you replace this default error handler, be aware that the\n            exception handling in your code probably needs to be adapted.\n\n        Registering an error callback function replaces any previously\n        registered error callback, including the above mentioned default error\n        handler.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_27set_error_callback(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_func = 0;
   PyObject *__pyx_v_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -6657,15 +6756,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_error_callback") < 0)) __PYX_ERR(0, 720, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_error_callback") < 0)) __PYX_ERR(0, 719, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -6673,47 +6772,47 @@
       }
     }
     __pyx_v_func = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_error_callback", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 720, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_error_callback", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 719, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.set_error_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.set_error_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_26set_error_callback(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_func, __pyx_v_data);
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_26set_error_callback(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), __pyx_v_func, __pyx_v_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_26set_error_callback(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_func, PyObject *__pyx_v_data) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_26set_error_callback(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v_func, PyObject *__pyx_v_data) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_error_callback", 0);
 
-  /* "src/_rtmidi.pyx":743
+  /* "_rtmidi.pyx":742
  * 
  *         """
  *         self._error_callback = (func, data, self._decode_string)             # <<<<<<<<<<<<<<
  *         self.baseptr().setErrorCallback(&_cb_error_func,
  *                                         <void *>self._error_callback)
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode_string); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 743, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_decode_string); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 743, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_func);
   __Pyx_GIVEREF(__pyx_v_func);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_func);
   __Pyx_INCREF(__pyx_v_data);
   __Pyx_GIVEREF(__pyx_v_data);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_data);
@@ -6722,109 +6821,109 @@
   __pyx_t_1 = 0;
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_error_callback);
   __Pyx_DECREF(__pyx_v_self->_error_callback);
   __pyx_v_self->_error_callback = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "src/_rtmidi.pyx":744
+  /* "_rtmidi.pyx":743
  *         """
  *         self._error_callback = (func, data, self._decode_string)
  *         self.baseptr().setErrorCallback(&_cb_error_func,             # <<<<<<<<<<<<<<
  *                                         <void *>self._error_callback)
  * 
  */
-  ((struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setErrorCallback((&__pyx_f_6rtmidi_7_rtmidi__cb_error_func), ((void *)__pyx_v_self->_error_callback)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 744, __pyx_L1_error)
+  ((struct __pyx_vtabstruct_7_rtmidi_MidiBase *)__pyx_v_self->__pyx_vtab)->baseptr(__pyx_v_self)->setErrorCallback((&__pyx_f_7_rtmidi__cb_error_func), ((void *)__pyx_v_self->_error_callback)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 743, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":720
+  /* "_rtmidi.pyx":719
  *         self.baseptr().setPortName(_to_bytes(name))
  * 
  *     def set_error_callback(self, func, data=None):             # <<<<<<<<<<<<<<
  *         """Register a callback function for errors.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.set_error_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.set_error_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":747
+/* "_rtmidi.pyx":746
  *                                         <void *>self._error_callback)
  * 
  *     def cancel_error_callback(self):             # <<<<<<<<<<<<<<
  *         """Remove the registered callback function for errors.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_29cancel_error_callback(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_28cancel_error_callback[] = "MidiBase.cancel_error_callback(self)\nRemove the registered callback function for errors.\n\n        This can be safely called even when no callback function has been\n        registered and reinstates the default error handler.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_29cancel_error_callback(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_29cancel_error_callback(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_28cancel_error_callback[] = "MidiBase.cancel_error_callback(self)\nRemove the registered callback function for errors.\n\n        This can be safely called even when no callback function has been\n        registered and reinstates the default error handler.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_29cancel_error_callback(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("cancel_error_callback (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_28cancel_error_callback(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_28cancel_error_callback(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_28cancel_error_callback(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_28cancel_error_callback(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cancel_error_callback", 0);
 
-  /* "src/_rtmidi.pyx":754
+  /* "_rtmidi.pyx":753
  * 
  *         """
  *         self.set_error_callback(_default_error_handler)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 754, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 753, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 754, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 753, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_4 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_t_3) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 754, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 753, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":747
+  /* "_rtmidi.pyx":746
  *                                         <void *>self._error_callback)
  * 
  *     def cancel_error_callback(self):             # <<<<<<<<<<<<<<
  *         """Remove the registered callback function for errors.
  * 
  */
 
@@ -6832,43 +6931,43 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.cancel_error_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.cancel_error_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_31__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_30__reduce_cython__[] = "MidiBase.__reduce_cython__(self)";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_31__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_31__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_30__reduce_cython__[] = "MidiBase.__reduce_cython__(self)";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_31__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_30__reduce_cython__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_30__reduce_cython__(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_30__reduce_cython__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_30__reduce_cython__(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
@@ -7089,15 +7188,15 @@
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_6);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -7107,43 +7206,43 @@
  *     else:
  *         return __pyx_unpickle_MidiBase, (type(self), 0x9171c0f, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_MidiBase__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_33__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_32__setstate_cython__[] = "MidiBase.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_33__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_33__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_7_rtmidi_8MidiBase_32__setstate_cython__[] = "MidiBase.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_7_rtmidi_8MidiBase_33__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_8MidiBase_32__setstate_cython__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_7_rtmidi_8MidiBase_32__setstate_cython__(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_8MidiBase_32__setstate_cython__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7_rtmidi_8MidiBase_32__setstate_cython__(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_MidiBase, (type(self), 0x9171c0f, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_MidiBase__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_6rtmidi_7_rtmidi___pyx_unpickle_MidiBase__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7_rtmidi___pyx_unpickle_MidiBase__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_MidiBase, (type(self), 0x9171c0f, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
@@ -7151,70 +7250,70 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiBase.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiBase.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":801
+/* "_rtmidi.pyx":800
  *     cdef object _callback
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr
  * 
  */
 
-static RtMidi *__pyx_f_6rtmidi_7_rtmidi_6MidiIn_baseptr(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self) {
+static RtMidi *__pyx_f_7_rtmidi_6MidiIn_baseptr(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   RtMidi *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("baseptr", 0);
 
-  /* "src/_rtmidi.pyx":802
+  /* "_rtmidi.pyx":801
  * 
  *     cdef RtMidi* baseptr(self):
  *         return self.thisptr             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None,
  */
   __pyx_r = __pyx_v_self->thisptr;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":801
+  /* "_rtmidi.pyx":800
  *     cdef object _callback
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":804
+/* "_rtmidi.pyx":803
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None,             # <<<<<<<<<<<<<<
  *                   unsigned int queue_size_limit=1024):
  *         """Create a new client instance for MIDI input.
  */
 
 /* Python wrapper */
-static int __pyx_pw_6rtmidi_7_rtmidi_6MidiIn_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_6rtmidi_7_rtmidi_6MidiIn_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_7_rtmidi_6MidiIn_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_7_rtmidi_6MidiIn_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   enum RtMidi::Api __pyx_v_rtapi;
   PyObject *__pyx_v_name = 0;
   unsigned int __pyx_v_queue_size_limit;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
@@ -7254,56 +7353,56 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_queue_size_limit);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 804, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 803, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_rtapi = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 804, __pyx_L3_error)
+      __pyx_v_rtapi = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 803, __pyx_L3_error)
     } else {
       __pyx_v_rtapi = __pyx_k__4;
     }
     __pyx_v_name = values[1];
     if (values[2]) {
-      __pyx_v_queue_size_limit = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_queue_size_limit == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 805, __pyx_L3_error)
+      __pyx_v_queue_size_limit = __Pyx_PyInt_As_unsigned_int(values[2]); if (unlikely((__pyx_v_queue_size_limit == (unsigned int)-1) && PyErr_Occurred())) __PYX_ERR(0, 804, __pyx_L3_error)
     } else {
       __pyx_v_queue_size_limit = ((unsigned int)0x400);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 804, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 803, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn___cinit__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self), __pyx_v_rtapi, __pyx_v_name, __pyx_v_queue_size_limit);
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn___cinit__(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self), __pyx_v_rtapi, __pyx_v_name, __pyx_v_queue_size_limit);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_6rtmidi_7_rtmidi_6MidiIn___cinit__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self, enum RtMidi::Api __pyx_v_rtapi, PyObject *__pyx_v_name, unsigned int __pyx_v_queue_size_limit) {
+static int __pyx_pf_7_rtmidi_6MidiIn___cinit__(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self, enum RtMidi::Api __pyx_v_rtapi, PyObject *__pyx_v_name, unsigned int __pyx_v_queue_size_limit) {
   PyObject *__pyx_v_exc = NULL;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -7328,45 +7427,45 @@
   PyObject *__pyx_t_23 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
   __Pyx_INCREF(__pyx_v_name);
 
-  /* "src/_rtmidi.pyx":811
+  /* "_rtmidi.pyx":810
  * 
  *         """
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidiIn Client"
  * 
  */
   __pyx_t_1 = (__pyx_v_name == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "src/_rtmidi.pyx":812
+    /* "_rtmidi.pyx":811
  *         """
  *         if name is None:
  *             name = "RtMidiIn Client"             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
     __Pyx_INCREF(__pyx_kp_u_RtMidiIn_Client);
     __Pyx_DECREF_SET(__pyx_v_name, __pyx_kp_u_RtMidiIn_Client);
 
-    /* "src/_rtmidi.pyx":811
+    /* "_rtmidi.pyx":810
  * 
  *         """
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidiIn Client"
  * 
  */
   }
 
-  /* "src/_rtmidi.pyx":814
+  /* "_rtmidi.pyx":813
  *             name = "RtMidiIn Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:
  */
   {
@@ -7374,49 +7473,49 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_5);
     /*try:*/ {
 
-      /* "src/_rtmidi.pyx":815
+      /* "_rtmidi.pyx":814
  * 
  *         try:
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)             # <<<<<<<<<<<<<<
  *         except RuntimeError as exc:
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 815, __pyx_L4_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 814, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
       __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_name);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 815, __pyx_L4_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 814, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 815, __pyx_L4_error)
+      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 814, __pyx_L4_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       try {
         __pyx_t_10 = new RtMidiIn(__pyx_v_rtapi, __pyx_t_9, __pyx_v_queue_size_limit);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 815, __pyx_L4_error)
+        __PYX_ERR(0, 814, __pyx_L4_error)
       }
       __pyx_v_self->thisptr = __pyx_t_10;
 
-      /* "src/_rtmidi.pyx":814
+      /* "_rtmidi.pyx":813
  *             name = "RtMidiIn Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:
  */
     }
@@ -7425,65 +7524,65 @@
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L9_try_end;
     __pyx_L4_error:;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "src/_rtmidi.pyx":816
+    /* "_rtmidi.pyx":815
  *         try:
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:             # <<<<<<<<<<<<<<
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  */
     __pyx_t_11 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_RuntimeError);
     if (__pyx_t_11) {
-      __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 816, __pyx_L6_except_error)
+      __Pyx_AddTraceback("_rtmidi.MidiIn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 815, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_7);
       __pyx_v_exc = __pyx_t_7;
       /*try:*/ {
 
-        /* "src/_rtmidi.pyx":817
+        /* "_rtmidi.pyx":816
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)             # <<<<<<<<<<<<<<
  * 
  *         self.set_error_callback(_default_error_handler)
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 817, __pyx_L15_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 816, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_exc); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 817, __pyx_L15_error)
+        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_exc); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 816, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 817, __pyx_L15_error)
+        __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 816, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_14);
         __Pyx_GIVEREF(__pyx_t_13);
         PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13);
         __pyx_t_13 = 0;
-        __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 817, __pyx_L15_error)
+        __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 816, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_15 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 817, __pyx_L15_error)
+        __pyx_t_15 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 816, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_15);
-        if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_type, __pyx_t_15) < 0) __PYX_ERR(0, 817, __pyx_L15_error)
+        if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_type, __pyx_t_15) < 0) __PYX_ERR(0, 816, __pyx_L15_error)
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 817, __pyx_L15_error)
+        __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 816, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_Raise(__pyx_t_15, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __PYX_ERR(0, 817, __pyx_L15_error)
+        __PYX_ERR(0, 816, __pyx_L15_error)
       }
 
-      /* "src/_rtmidi.pyx":816
+      /* "_rtmidi.pyx":815
  *         try:
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:             # <<<<<<<<<<<<<<
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  */
       /*finally:*/ {
@@ -7524,98 +7623,98 @@
           goto __pyx_L6_except_error;
         }
       }
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
-    /* "src/_rtmidi.pyx":814
+    /* "_rtmidi.pyx":813
  *             name = "RtMidiIn Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiIn(rtapi, _to_bytes(name), queue_size_limit)
  *         except RuntimeError as exc:
  */
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
     goto __pyx_L1_error;
     __pyx_L9_try_end:;
   }
 
-  /* "src/_rtmidi.pyx":819
+  /* "_rtmidi.pyx":818
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  *         self.set_error_callback(_default_error_handler)             # <<<<<<<<<<<<<<
  *         self._callback = None
  *         self._port = None
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 819, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 818, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 819, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 818, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_8 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_15, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 819, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 818, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "src/_rtmidi.pyx":820
+  /* "_rtmidi.pyx":819
  * 
  *         self.set_error_callback(_default_error_handler)
  *         self._callback = None             # <<<<<<<<<<<<<<
  *         self._port = None
  *         self._deleted = False
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->_callback);
   __Pyx_DECREF(__pyx_v_self->_callback);
   __pyx_v_self->_callback = Py_None;
 
-  /* "src/_rtmidi.pyx":821
+  /* "_rtmidi.pyx":820
  *         self.set_error_callback(_default_error_handler)
  *         self._callback = None
  *         self._port = None             # <<<<<<<<<<<<<<
  *         self._deleted = False
  * 
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base._port);
   __Pyx_DECREF(__pyx_v_self->__pyx_base._port);
   __pyx_v_self->__pyx_base._port = Py_None;
 
-  /* "src/_rtmidi.pyx":822
+  /* "_rtmidi.pyx":821
  *         self._callback = None
  *         self._port = None
  *         self._deleted = False             # <<<<<<<<<<<<<<
  * 
  *     def get_current_api(self):
  */
   __Pyx_INCREF(Py_False);
   __Pyx_GIVEREF(Py_False);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base._deleted);
   __Pyx_DECREF(__pyx_v_self->__pyx_base._deleted);
   __pyx_v_self->__pyx_base._deleted = Py_False;
 
-  /* "src/_rtmidi.pyx":804
+  /* "_rtmidi.pyx":803
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None,             # <<<<<<<<<<<<<<
  *                   unsigned int queue_size_limit=1024):
  *         """Create a new client instance for MIDI input.
  */
 
@@ -7626,530 +7725,530 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_exc);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":824
+/* "_rtmidi.pyx":823
  *         self._deleted = False
  * 
  *     def get_current_api(self):             # <<<<<<<<<<<<<<
  *         """Return the low-level MIDI backend API used by this instance.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_3get_current_api(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_2get_current_api[] = "MidiIn.get_current_api(self)\nReturn the low-level MIDI backend API used by this instance.\n\n        Use this by comparing the returned value to the module-level ``API_*``\n        constants, e.g.::\n\n            midiin = rtmidi.MidiIn()\n\n            if midiin.get_current_api() == rtmidi.API_UNIX_JACK:\n                print(\"Using JACK API for MIDI input.\")\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_3get_current_api(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_3get_current_api(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_6MidiIn_2get_current_api[] = "MidiIn.get_current_api(self)\nReturn the low-level MIDI backend API used by this instance.\n\n        Use this by comparing the returned value to the module-level ``API_*``\n        constants, e.g.::\n\n            midiin = rtmidi.MidiIn()\n\n            if midiin.get_current_api() == rtmidi.API_UNIX_JACK:\n                print(\"Using JACK API for MIDI input.\")\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_3get_current_api(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_current_api (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_2get_current_api(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_2get_current_api(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_2get_current_api(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_2get_current_api(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_current_api", 0);
 
-  /* "src/_rtmidi.pyx":836
+  /* "_rtmidi.pyx":835
  * 
  *         """
  *         return self.thisptr.getCurrentApi()             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(__pyx_v_self->thisptr->getCurrentApi()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 836, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(__pyx_v_self->thisptr->getCurrentApi()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 835, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":824
+  /* "_rtmidi.pyx":823
  *         self._deleted = False
  * 
  *     def get_current_api(self):             # <<<<<<<<<<<<<<
  *         """Return the low-level MIDI backend API used by this instance.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.get_current_api", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.get_current_api", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":838
+/* "_rtmidi.pyx":837
  *         return self.thisptr.getCurrentApi()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  */
 
 /* Python wrapper */
-static void __pyx_pw_6rtmidi_7_rtmidi_6MidiIn_5__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_6rtmidi_7_rtmidi_6MidiIn_5__dealloc__(PyObject *__pyx_v_self) {
+static void __pyx_pw_7_rtmidi_6MidiIn_5__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_7_rtmidi_6MidiIn_5__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_4__dealloc__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self));
+  __pyx_pf_7_rtmidi_6MidiIn_4__dealloc__(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-static void __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_4__dealloc__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self) {
+static void __pyx_pf_7_rtmidi_6MidiIn_4__dealloc__(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "src/_rtmidi.pyx":840
+  /* "_rtmidi.pyx":839
  *     def __dealloc__(self):
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):             # <<<<<<<<<<<<<<
  *             del self.thisptr
  * 
  */
-  __pyx_t_1 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_thisptr); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 840, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_thisptr); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 839, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "src/_rtmidi.pyx":841
+    /* "_rtmidi.pyx":840
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  *             del self.thisptr             # <<<<<<<<<<<<<<
  * 
  *     def delete(self):
  */
     delete __pyx_v_self->thisptr;
 
-    /* "src/_rtmidi.pyx":840
+    /* "_rtmidi.pyx":839
  *     def __dealloc__(self):
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):             # <<<<<<<<<<<<<<
  *             del self.thisptr
  * 
  */
   }
 
-  /* "src/_rtmidi.pyx":838
+  /* "_rtmidi.pyx":837
  *         return self.thisptr.getCurrentApi()
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_WriteUnraisable("rtmidi._rtmidi.MidiIn.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("_rtmidi.MidiIn.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "src/_rtmidi.pyx":843
+/* "_rtmidi.pyx":842
  *             del self.thisptr
  * 
  *     def delete(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_7delete(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_6delete[] = "MidiIn.delete(self)\nDe-allocate pointer to C++ class instance.\n\n        .. warning:: the instance **must not** be used anymore after calling\n            this method, otherwise the program will crash with a segmentation\n            fault!\n\n            The reason this potentially dangerous method exists is that in\n            some cases it is desirable to destroy the internal ``RtMidiIn``\n            C++ class instance with immediate effect, thereby closing the\n            backend MIDI API client and all the ports it opened. By merely\n            using ``del`` on the ``rtmidi.MidiIn`` Python instance, the\n            destruction of the C++ instance may be delayed for an arbitrary\n            amount of time, until the Python garbage collector cleans up the\n            instance.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_7delete(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_7delete(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_6MidiIn_6delete[] = "MidiIn.delete(self)\nDe-allocate pointer to C++ class instance.\n\n        .. warning:: the instance **must not** be used anymore after calling\n            this method, otherwise the program will crash with a segmentation\n            fault!\n\n            The reason this potentially dangerous method exists is that in\n            some cases it is desirable to destroy the internal ``RtMidiIn``\n            C++ class instance with immediate effect, thereby closing the\n            backend MIDI API client and all the ports it opened. By merely\n            using ``del`` on the ``rtmidi.MidiIn`` Python instance, the\n            destruction of the C++ instance may be delayed for an arbitrary\n            amount of time, until the Python garbage collector cleans up the\n            instance.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_7delete(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("delete (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_6delete(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_6delete(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_6delete(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_6delete(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("delete", 0);
 
-  /* "src/_rtmidi.pyx":860
+  /* "_rtmidi.pyx":859
  * 
  *         """
  *         if not self._deleted:             # <<<<<<<<<<<<<<
  *             del self.thisptr
  *             self._deleted = True
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->__pyx_base._deleted); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 860, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->__pyx_base._deleted); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 859, __pyx_L1_error)
   __pyx_t_2 = ((!__pyx_t_1) != 0);
   if (__pyx_t_2) {
 
-    /* "src/_rtmidi.pyx":861
+    /* "_rtmidi.pyx":860
  *         """
  *         if not self._deleted:
  *             del self.thisptr             # <<<<<<<<<<<<<<
  *             self._deleted = True
  * 
  */
     delete __pyx_v_self->thisptr;
 
-    /* "src/_rtmidi.pyx":862
+    /* "_rtmidi.pyx":861
  *         if not self._deleted:
  *             del self.thisptr
  *             self._deleted = True             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
     __Pyx_INCREF(Py_True);
     __Pyx_GIVEREF(Py_True);
     __Pyx_GOTREF(__pyx_v_self->__pyx_base._deleted);
     __Pyx_DECREF(__pyx_v_self->__pyx_base._deleted);
     __pyx_v_self->__pyx_base._deleted = Py_True;
 
-    /* "src/_rtmidi.pyx":860
+    /* "_rtmidi.pyx":859
  * 
  *         """
  *         if not self._deleted:             # <<<<<<<<<<<<<<
  *             del self.thisptr
  *             self._deleted = True
  */
   }
 
-  /* "src/_rtmidi.pyx":843
+  /* "_rtmidi.pyx":842
  *             del self.thisptr
  * 
  *     def delete(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.delete", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.delete", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":865
+/* "_rtmidi.pyx":864
  * 
  *     @property
  *     def is_deleted(self):             # <<<<<<<<<<<<<<
  *         return self._deleted
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_10is_deleted_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_10is_deleted_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_10is_deleted_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_10is_deleted_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_10is_deleted___get__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_10is_deleted___get__(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_10is_deleted___get__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_10is_deleted___get__(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "src/_rtmidi.pyx":866
+  /* "_rtmidi.pyx":865
  *     @property
  *     def is_deleted(self):
  *         return self._deleted             # <<<<<<<<<<<<<<
  * 
  *     def cancel_callback(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->__pyx_base._deleted);
   __pyx_r = __pyx_v_self->__pyx_base._deleted;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":865
+  /* "_rtmidi.pyx":864
  * 
  *     @property
  *     def is_deleted(self):             # <<<<<<<<<<<<<<
  *         return self._deleted
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":868
+/* "_rtmidi.pyx":867
  *         return self._deleted
  * 
  *     def cancel_callback(self):             # <<<<<<<<<<<<<<
  *         """Remove the registered callback function for MIDI input.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_9cancel_callback(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_8cancel_callback[] = "MidiIn.cancel_callback(self)\nRemove the registered callback function for MIDI input.\n\n        This can be safely called even when no callback function has been\n        registered.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_9cancel_callback(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_9cancel_callback(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_6MidiIn_8cancel_callback[] = "MidiIn.cancel_callback(self)\nRemove the registered callback function for MIDI input.\n\n        This can be safely called even when no callback function has been\n        registered.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_9cancel_callback(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("cancel_callback (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_8cancel_callback(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_8cancel_callback(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_8cancel_callback(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_8cancel_callback(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("cancel_callback", 0);
 
-  /* "src/_rtmidi.pyx":875
+  /* "_rtmidi.pyx":874
  * 
  *         """
  *         if self._callback:             # <<<<<<<<<<<<<<
  *             self.thisptr.cancelCallback()
  *             self._callback = None
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_callback); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 875, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_callback); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 874, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "src/_rtmidi.pyx":876
+    /* "_rtmidi.pyx":875
  *         """
  *         if self._callback:
  *             self.thisptr.cancelCallback()             # <<<<<<<<<<<<<<
  *             self._callback = None
  * 
  */
-    __pyx_v_self->thisptr->cancelCallback(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 876, __pyx_L1_error)
+    __pyx_v_self->thisptr->cancelCallback(); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 875, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":877
+    /* "_rtmidi.pyx":876
  *         if self._callback:
  *             self.thisptr.cancelCallback()
  *             self._callback = None             # <<<<<<<<<<<<<<
  * 
  *     def close_port(self):
  */
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     __Pyx_GOTREF(__pyx_v_self->_callback);
     __Pyx_DECREF(__pyx_v_self->_callback);
     __pyx_v_self->_callback = Py_None;
 
-    /* "src/_rtmidi.pyx":875
+    /* "_rtmidi.pyx":874
  * 
  *         """
  *         if self._callback:             # <<<<<<<<<<<<<<
  *             self.thisptr.cancelCallback()
  *             self._callback = None
  */
   }
 
-  /* "src/_rtmidi.pyx":868
+  /* "_rtmidi.pyx":867
  *         return self._deleted
  * 
  *     def cancel_callback(self):             # <<<<<<<<<<<<<<
  *         """Remove the registered callback function for MIDI input.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.cancel_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.cancel_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":879
+/* "_rtmidi.pyx":878
  *             self._callback = None
  * 
  *     def close_port(self):             # <<<<<<<<<<<<<<
  *         self.cancel_callback()
  *         MidiBase.close_port(self)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_11close_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_10close_port[] = "MidiIn.close_port(self)";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_11close_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_11close_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_6MidiIn_10close_port[] = "MidiIn.close_port(self)";
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_11close_port(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("close_port (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_10close_port(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_10close_port(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_10close_port(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_10close_port(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close_port", 0);
 
-  /* "src/_rtmidi.pyx":880
+  /* "_rtmidi.pyx":879
  * 
  *     def close_port(self):
  *         self.cancel_callback()             # <<<<<<<<<<<<<<
  *         MidiBase.close_port(self)
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cancel_callback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 880, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cancel_callback); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_3) : __Pyx_PyObject_CallNoArg(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 880, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 879, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":881
+  /* "_rtmidi.pyx":880
  *     def close_port(self):
  *         self.cancel_callback()
  *         MidiBase.close_port(self)             # <<<<<<<<<<<<<<
  * 
  *     close_port.__doc__ == MidiBase.close_port.__doc__
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6rtmidi_7_rtmidi_MidiBase), __pyx_n_s_close_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 881, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7_rtmidi_MidiBase), __pyx_n_s_close_port); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 880, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_3);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
   __pyx_t_1 = (__pyx_t_3) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_3, ((PyObject *)__pyx_v_self)) : __Pyx_PyObject_CallOneArg(__pyx_t_2, ((PyObject *)__pyx_v_self));
   __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 881, __pyx_L1_error)
+  if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 880, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":879
+  /* "_rtmidi.pyx":878
  *             self._callback = None
  * 
  *     def close_port(self):             # <<<<<<<<<<<<<<
  *         self.cancel_callback()
  *         MidiBase.close_port(self)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.close_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.close_port", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":885
+/* "_rtmidi.pyx":884
  *     close_port.__doc__ == MidiBase.close_port.__doc__
  * 
  *     def get_message(self):             # <<<<<<<<<<<<<<
  *         """Poll for MIDI input.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_13get_message(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_12get_message[] = "MidiIn.get_message(self)\nPoll for MIDI input.\n\n        Checks whether a MIDI event is available in the input buffer and\n        returns a two-element tuple with the MIDI message and a delta time. The\n        MIDI message is a list of integers representing the data bytes of the\n        message, the delta time is a float representing the time in seconds\n        elapsed since the reception of the previous MIDI event.\n\n        The function does not block. When no MIDI message is available, it\n        returns ``None``.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_13get_message(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_13get_message(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_6MidiIn_12get_message[] = "MidiIn.get_message(self)\nPoll for MIDI input.\n\n        Checks whether a MIDI event is available in the input buffer and\n        returns a two-element tuple with the MIDI message and a delta time. The\n        MIDI message is a list of integers representing the data bytes of the\n        message, the delta time is a float representing the time in seconds\n        elapsed since the reception of the previous MIDI event.\n\n        The function does not block. When no MIDI message is available, it\n        returns ``None``.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_13get_message(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_message (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_12get_message(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_12get_message(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_12get_message(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_12get_message(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   std::vector<unsigned char>  __pyx_v_msg_v;
   double __pyx_v_delta_time;
   PyObject *__pyx_v_message = NULL;
   std::vector<unsigned char> ::size_type __pyx_8genexpr3__pyx_v_i;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
@@ -8161,129 +8260,129 @@
   __Pyx_FakeReference<unsigned char> __pyx_t_7;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_message", 0);
 
-  /* "src/_rtmidi.pyx":899
+  /* "_rtmidi.pyx":898
  *         """
  *         cdef vector[unsigned char] msg_v
  *         cdef double delta_time = self.thisptr.getMessage(&msg_v)             # <<<<<<<<<<<<<<
  * 
  *         if not msg_v.empty():
  */
-  __pyx_t_1 = __pyx_v_self->thisptr->getMessage((&__pyx_v_msg_v)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 899, __pyx_L1_error)
+  __pyx_t_1 = __pyx_v_self->thisptr->getMessage((&__pyx_v_msg_v)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 898, __pyx_L1_error)
   __pyx_v_delta_time = __pyx_t_1;
 
-  /* "src/_rtmidi.pyx":901
+  /* "_rtmidi.pyx":900
  *         cdef double delta_time = self.thisptr.getMessage(&msg_v)
  * 
  *         if not msg_v.empty():             # <<<<<<<<<<<<<<
  *             message = [msg_v.at(i) for i in range(msg_v.size())]
  *             return (message, delta_time)
  */
   __pyx_t_2 = ((!(__pyx_v_msg_v.empty() != 0)) != 0);
   if (__pyx_t_2) {
 
-    /* "src/_rtmidi.pyx":902
+    /* "_rtmidi.pyx":901
  * 
  *         if not msg_v.empty():
  *             message = [msg_v.at(i) for i in range(msg_v.size())]             # <<<<<<<<<<<<<<
  *             return (message, delta_time)
  * 
  */
     { /* enter inner scope */
-      __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 902, __pyx_L1_error)
+      __pyx_t_3 = PyList_New(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 901, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __pyx_t_4 = __pyx_v_msg_v.size();
       __pyx_t_5 = __pyx_t_4;
       for (__pyx_t_6 = 0; __pyx_t_6 < __pyx_t_5; __pyx_t_6+=1) {
         __pyx_8genexpr3__pyx_v_i = __pyx_t_6;
         try {
           __pyx_t_7 = __pyx_v_msg_v.at(__pyx_8genexpr3__pyx_v_i);
         } catch(...) {
           __Pyx_CppExn2PyErr();
-          __PYX_ERR(0, 902, __pyx_L1_error)
+          __PYX_ERR(0, 901, __pyx_L1_error)
         }
-        __pyx_t_8 = __Pyx_PyInt_From_unsigned_char(__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 902, __pyx_L1_error)
+        __pyx_t_8 = __Pyx_PyInt_From_unsigned_char(__pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 901, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 902, __pyx_L1_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_3, (PyObject*)__pyx_t_8))) __PYX_ERR(0, 901, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
     } /* exit inner scope */
     __pyx_v_message = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "src/_rtmidi.pyx":903
+    /* "_rtmidi.pyx":902
  *         if not msg_v.empty():
  *             message = [msg_v.at(i) for i in range(msg_v.size())]
  *             return (message, delta_time)             # <<<<<<<<<<<<<<
  * 
  *     def ignore_types(self, sysex=True, timing=True, active_sense=True):
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 903, __pyx_L1_error)
+    __pyx_t_3 = PyFloat_FromDouble(__pyx_v_delta_time); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 902, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 903, __pyx_L1_error)
+    __pyx_t_8 = PyTuple_New(2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 902, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_INCREF(__pyx_v_message);
     __Pyx_GIVEREF(__pyx_v_message);
     PyTuple_SET_ITEM(__pyx_t_8, 0, __pyx_v_message);
     __Pyx_GIVEREF(__pyx_t_3);
     PyTuple_SET_ITEM(__pyx_t_8, 1, __pyx_t_3);
     __pyx_t_3 = 0;
     __pyx_r = __pyx_t_8;
     __pyx_t_8 = 0;
     goto __pyx_L0;
 
-    /* "src/_rtmidi.pyx":901
+    /* "_rtmidi.pyx":900
  *         cdef double delta_time = self.thisptr.getMessage(&msg_v)
  * 
  *         if not msg_v.empty():             # <<<<<<<<<<<<<<
  *             message = [msg_v.at(i) for i in range(msg_v.size())]
  *             return (message, delta_time)
  */
   }
 
-  /* "src/_rtmidi.pyx":885
+  /* "_rtmidi.pyx":884
  *     close_port.__doc__ == MidiBase.close_port.__doc__
  * 
  *     def get_message(self):             # <<<<<<<<<<<<<<
  *         """Poll for MIDI input.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.get_message", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.get_message", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_message);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":905
+/* "_rtmidi.pyx":904
  *             return (message, delta_time)
  * 
  *     def ignore_types(self, sysex=True, timing=True, active_sense=True):             # <<<<<<<<<<<<<<
  *         """Enable/Disable input filtering of certain types of MIDI events.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_15ignore_types(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_14ignore_types[] = "MidiIn.ignore_types(self, sysex=True, timing=True, active_sense=True)\nEnable/Disable input filtering of certain types of MIDI events.\n\n        By default System Exclusive (aka sysex), MIDI Clock and Active Sensing\n        messages are filtered from the MIDI input and never reach your code,\n        because they can fill up input buffers very quickly.\n\n        To receive them, you can selectively disable the filtering of these\n        event types.\n\n        To enable reception - i.e. turn off the default filtering - of sysex\n        messages, pass ``sysex = False``.\n\n        To enable reception of MIDI Clock, pass ``timing = False``.\n\n        To enable reception of Active Sensing, pass ``active_sense = False``.\n\n        These arguments can of course be combined in one call, and they all\n        default to ``True``.\n\n        If you enable reception of any of these event types, be sure to either\n        use an input callback function, which returns quickly or poll for MIDI\n        input often. Otherwise you might lose MIDI input because the input\n        buffer overflows.\n\n        **Windows note:** the Windows Multi Media API uses fixed size buffers\n        for the reception of sysex messages, whose number and size is set at\n        compile time. Sysex messages longer than the buffer size can not be\n        received properly when using the Windows Multi Media API.\n\n        The default distribution of python-rtmidi sets the number of sysex\n        buffers to four and the size of each to 8192 bytes. To change these\n        values, edit the ``RT_SYSEX_BUFFER_COUNT`` and ``RT_SYSEX_BUFFER_SIZE``\n        preprocessor defines in ``RtMidi.cpp`` and recompile.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_15ignore_types(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_15ignore_types(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_6MidiIn_14ignore_types[] = "MidiIn.ignore_types(self, sysex=True, timing=True, active_sense=True)\nEnable/Disable input filtering of certain types of MIDI events.\n\n        By default System Exclusive (aka sysex), MIDI Clock and Active Sensing\n        messages are filtered from the MIDI input and never reach your code,\n        because they can fill up input buffers very quickly.\n\n        To receive them, you can selectively disable the filtering of these\n        event types.\n\n        To enable reception - i.e. turn off the default filtering - of sysex\n        messages, pass ``sysex = False``.\n\n        To enable reception of MIDI Clock, pass ``timing = False``.\n\n        To enable reception of Active Sensing, pass ``active_sense = False``.\n\n        These arguments can of course be combined in one call, and they all\n        default to ``True``.\n\n        If you enable reception of any of these event types, be sure to either\n        use an input callback function, which returns quickly or poll for MIDI\n        input often. Otherwise you might lose MIDI input because the input\n        buffer overflows.\n\n        **Windows note:** the Windows Multi Media API uses fixed size buffers\n        for the reception of sysex messages, whose number and size is set at\n        compile time. Sysex messages longer than the buffer size can not be\n        received properly when using the Windows Multi Media API.\n\n        The default distribution of python-rtmidi sets the number of sysex\n        buffers to four and the size of each to 8192 bytes. To change these\n        values, edit the ``RT_SYSEX_BUFFER_COUNT`` and ``RT_SYSEX_BUFFER_SIZE``\n        preprocessor defines in ``RtMidi.cpp`` and recompile.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_15ignore_types(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_sysex = 0;
   PyObject *__pyx_v_timing = 0;
   PyObject *__pyx_v_active_sense = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -8325,15 +8424,15 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_active_sense);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "ignore_types") < 0)) __PYX_ERR(0, 905, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "ignore_types") < 0)) __PYX_ERR(0, 904, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -8345,82 +8444,82 @@
     }
     __pyx_v_sysex = values[0];
     __pyx_v_timing = values[1];
     __pyx_v_active_sense = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("ignore_types", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 905, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("ignore_types", 0, 0, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 904, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.ignore_types", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.ignore_types", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_14ignore_types(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self), __pyx_v_sysex, __pyx_v_timing, __pyx_v_active_sense);
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_14ignore_types(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self), __pyx_v_sysex, __pyx_v_timing, __pyx_v_active_sense);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_14ignore_types(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self, PyObject *__pyx_v_sysex, PyObject *__pyx_v_timing, PyObject *__pyx_v_active_sense) {
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_14ignore_types(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self, PyObject *__pyx_v_sysex, PyObject *__pyx_v_timing, PyObject *__pyx_v_active_sense) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   bool __pyx_t_1;
   bool __pyx_t_2;
   bool __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("ignore_types", 0);
 
-  /* "src/_rtmidi.pyx":941
+  /* "_rtmidi.pyx":940
  * 
  *         """
  *         self.thisptr.ignoreTypes(sysex, timing, active_sense)             # <<<<<<<<<<<<<<
  * 
  *     def set_callback(self, func, data=None):
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_sysex); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 941, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_timing); if (unlikely((__pyx_t_2 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 941, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_active_sense); if (unlikely((__pyx_t_3 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 941, __pyx_L1_error)
-  __pyx_v_self->thisptr->ignoreTypes(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 941, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_sysex); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 940, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_IsTrue(__pyx_v_timing); if (unlikely((__pyx_t_2 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 940, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_IsTrue(__pyx_v_active_sense); if (unlikely((__pyx_t_3 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(0, 940, __pyx_L1_error)
+  __pyx_v_self->thisptr->ignoreTypes(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 940, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":905
+  /* "_rtmidi.pyx":904
  *             return (message, delta_time)
  * 
  *     def ignore_types(self, sysex=True, timing=True, active_sense=True):             # <<<<<<<<<<<<<<
  *         """Enable/Disable input filtering of certain types of MIDI events.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.ignore_types", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.ignore_types", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":943
+/* "_rtmidi.pyx":942
  *         self.thisptr.ignoreTypes(sysex, timing, active_sense)
  * 
  *     def set_callback(self, func, data=None):             # <<<<<<<<<<<<<<
  *         """Register a callback function for MIDI input.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_17set_callback(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_16set_callback[] = "MidiIn.set_callback(self, func, data=None)\nRegister a callback function for MIDI input.\n\n        The callback function is called whenever a MIDI message is received and\n        must take two arguments. The first argument is a two-element tuple with\n        the MIDI message and a delta time, like the one returned by the\n        ``get_message`` method. The second argument is value of the ``data``\n        argument passed to ``set_callback`` when the callback is registered.\n        The value of ``data`` can be any Python object. It can be used inside\n        the callback function to access data that would not be in scope\n        otherwise.\n\n        Registering a callback function replaces any previously registered\n        callback.\n\n        The callback function is safely removed when the input port is closed\n        or the ``MidiIn`` instance is deleted.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_17set_callback(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_17set_callback(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_6MidiIn_16set_callback[] = "MidiIn.set_callback(self, func, data=None)\nRegister a callback function for MIDI input.\n\n        The callback function is called whenever a MIDI message is received and\n        must take two arguments. The first argument is a two-element tuple with\n        the MIDI message and a delta time, like the one returned by the\n        ``get_message`` method. The second argument is value of the ``data``\n        argument passed to ``set_callback`` when the callback is registered.\n        The value of ``data`` can be any Python object. It can be used inside\n        the callback function to access data that would not be in scope\n        otherwise.\n\n        Registering a callback function replaces any previously registered\n        callback.\n\n        The callback function is safely removed when the input port is closed\n        or the ``MidiIn`` instance is deleted.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_17set_callback(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_func = 0;
   PyObject *__pyx_v_data = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -8449,15 +8548,15 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_callback") < 0)) __PYX_ERR(0, 943, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "set_callback") < 0)) __PYX_ERR(0, 942, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
@@ -8465,158 +8564,158 @@
       }
     }
     __pyx_v_func = values[0];
     __pyx_v_data = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("set_callback", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 943, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("set_callback", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 942, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.set_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.set_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_16set_callback(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self), __pyx_v_func, __pyx_v_data);
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_16set_callback(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self), __pyx_v_func, __pyx_v_data);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_16set_callback(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self, PyObject *__pyx_v_func, PyObject *__pyx_v_data) {
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_16set_callback(struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self, PyObject *__pyx_v_func, PyObject *__pyx_v_data) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_callback", 0);
 
-  /* "src/_rtmidi.pyx":962
+  /* "_rtmidi.pyx":961
  * 
  *         """
  *         if self._callback:             # <<<<<<<<<<<<<<
  *             self.cancel_callback()
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_callback); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 962, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->_callback); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 961, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "src/_rtmidi.pyx":963
+    /* "_rtmidi.pyx":962
  *         """
  *         if self._callback:
  *             self.cancel_callback()             # <<<<<<<<<<<<<<
  * 
  *         self._callback = (func, data)
  */
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cancel_callback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 963, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_cancel_callback); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 962, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = NULL;
     if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_4)) {
         PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
         __Pyx_INCREF(__pyx_t_4);
         __Pyx_INCREF(function);
         __Pyx_DECREF_SET(__pyx_t_3, function);
       }
     }
     __pyx_t_2 = (__pyx_t_4) ? __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_4) : __Pyx_PyObject_CallNoArg(__pyx_t_3);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 963, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 962, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "src/_rtmidi.pyx":962
+    /* "_rtmidi.pyx":961
  * 
  *         """
  *         if self._callback:             # <<<<<<<<<<<<<<
  *             self.cancel_callback()
  * 
  */
   }
 
-  /* "src/_rtmidi.pyx":965
+  /* "_rtmidi.pyx":964
  *             self.cancel_callback()
  * 
  *         self._callback = (func, data)             # <<<<<<<<<<<<<<
  *         self.thisptr.setCallback(&_cb_func, <void *>self._callback)
  * 
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 965, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 964, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_func);
   __Pyx_GIVEREF(__pyx_v_func);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_func);
   __Pyx_INCREF(__pyx_v_data);
   __Pyx_GIVEREF(__pyx_v_data);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_data);
   __Pyx_GIVEREF(__pyx_t_2);
   __Pyx_GOTREF(__pyx_v_self->_callback);
   __Pyx_DECREF(__pyx_v_self->_callback);
   __pyx_v_self->_callback = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "src/_rtmidi.pyx":966
+  /* "_rtmidi.pyx":965
  * 
  *         self._callback = (func, data)
  *         self.thisptr.setCallback(&_cb_func, <void *>self._callback)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_v_self->thisptr->setCallback((&__pyx_f_6rtmidi_7_rtmidi__cb_func), ((void *)__pyx_v_self->_callback)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 966, __pyx_L1_error)
+  __pyx_v_self->thisptr->setCallback((&__pyx_f_7_rtmidi__cb_func), ((void *)__pyx_v_self->_callback)); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 965, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":943
+  /* "_rtmidi.pyx":942
  *         self.thisptr.ignoreTypes(sysex, timing, active_sense)
  * 
  *     def set_callback(self, func, data=None):             # <<<<<<<<<<<<<<
  *         """Register a callback function for MIDI input.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.set_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.set_callback", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_18__reduce_cython__[] = "MidiIn.__reduce_cython__(self)";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_6MidiIn_18__reduce_cython__[] = "MidiIn.__reduce_cython__(self)";
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_19__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_18__reduce_cython__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_18__reduce_cython__(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_18__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -8638,43 +8737,43 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_20__setstate_cython__[] = "MidiIn.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_7_rtmidi_6MidiIn_20__setstate_cython__[] = "MidiIn.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_7_rtmidi_6MidiIn_21__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_6MidiIn_20__setstate_cython__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_7_rtmidi_6MidiIn_20__setstate_cython__(((struct __pyx_obj_7_rtmidi_MidiIn *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_6MidiIn_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7_rtmidi_6MidiIn_20__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiIn *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -8696,69 +8795,69 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiIn.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiIn.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":1006
+/* "_rtmidi.pyx":1005
  *     cdef RtMidiOut *thisptr
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr
  * 
  */
 
-static RtMidi *__pyx_f_6rtmidi_7_rtmidi_7MidiOut_baseptr(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self) {
+static RtMidi *__pyx_f_7_rtmidi_7MidiOut_baseptr(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self) {
   RtMidi *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("baseptr", 0);
 
-  /* "src/_rtmidi.pyx":1007
+  /* "_rtmidi.pyx":1006
  * 
  *     cdef RtMidi* baseptr(self):
  *         return self.thisptr             # <<<<<<<<<<<<<<
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None):
  */
   __pyx_r = __pyx_v_self->thisptr;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":1006
+  /* "_rtmidi.pyx":1005
  *     cdef RtMidiOut *thisptr
  * 
  *     cdef RtMidi* baseptr(self):             # <<<<<<<<<<<<<<
  *         return self.thisptr
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":1009
+/* "_rtmidi.pyx":1008
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None):             # <<<<<<<<<<<<<<
  *         """Create a new client instance for MIDI output.
  * 
  */
 
 /* Python wrapper */
-static int __pyx_pw_6rtmidi_7_rtmidi_7MidiOut_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_6rtmidi_7_rtmidi_7MidiOut_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_7_rtmidi_7MidiOut_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_7_rtmidi_7MidiOut_1__cinit__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   enum RtMidi::Api __pyx_v_rtapi;
   PyObject *__pyx_v_name = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
@@ -8789,49 +8888,49 @@
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_name);
           if (value) { values[1] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 1009, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__cinit__") < 0)) __PYX_ERR(0, 1008, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     if (values[0]) {
-      __pyx_v_rtapi = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1009, __pyx_L3_error)
+      __pyx_v_rtapi = ((enum RtMidi::Api)__Pyx_PyInt_As_enum__RtMidi_3a__3a_Api(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1008, __pyx_L3_error)
     } else {
       __pyx_v_rtapi = __pyx_k__7;
     }
     __pyx_v_name = values[1];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1009, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 0, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 1008, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiOut.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiOut.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_7MidiOut___cinit__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *)__pyx_v_self), __pyx_v_rtapi, __pyx_v_name);
+  __pyx_r = __pyx_pf_7_rtmidi_7MidiOut___cinit__(((struct __pyx_obj_7_rtmidi_MidiOut *)__pyx_v_self), __pyx_v_rtapi, __pyx_v_name);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_6rtmidi_7_rtmidi_7MidiOut___cinit__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self, enum RtMidi::Api __pyx_v_rtapi, PyObject *__pyx_v_name) {
+static int __pyx_pf_7_rtmidi_7MidiOut___cinit__(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self, enum RtMidi::Api __pyx_v_rtapi, PyObject *__pyx_v_name) {
   PyObject *__pyx_v_exc = NULL;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
@@ -8856,45 +8955,45 @@
   PyObject *__pyx_t_23 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
   __Pyx_INCREF(__pyx_v_name);
 
-  /* "src/_rtmidi.pyx":1015
+  /* "_rtmidi.pyx":1014
  * 
  *         """
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidiOut Client"
  * 
  */
   __pyx_t_1 = (__pyx_v_name == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "src/_rtmidi.pyx":1016
+    /* "_rtmidi.pyx":1015
  *         """
  *         if name is None:
  *             name = "RtMidiOut Client"             # <<<<<<<<<<<<<<
  * 
  *         try:
  */
     __Pyx_INCREF(__pyx_kp_u_RtMidiOut_Client);
     __Pyx_DECREF_SET(__pyx_v_name, __pyx_kp_u_RtMidiOut_Client);
 
-    /* "src/_rtmidi.pyx":1015
+    /* "_rtmidi.pyx":1014
  * 
  *         """
  *         if name is None:             # <<<<<<<<<<<<<<
  *             name = "RtMidiOut Client"
  * 
  */
   }
 
-  /* "src/_rtmidi.pyx":1018
+  /* "_rtmidi.pyx":1017
  *             name = "RtMidiOut Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:
  */
   {
@@ -8902,49 +9001,49 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_3, &__pyx_t_4, &__pyx_t_5);
     __Pyx_XGOTREF(__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_4);
     __Pyx_XGOTREF(__pyx_t_5);
     /*try:*/ {
 
-      /* "src/_rtmidi.pyx":1019
+      /* "_rtmidi.pyx":1018
  * 
  *         try:
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))             # <<<<<<<<<<<<<<
  *         except RuntimeError as exc:
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1019, __pyx_L4_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_to_bytes); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1018, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_t_8 = NULL;
       if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_7))) {
         __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
         if (likely(__pyx_t_8)) {
           PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
           __Pyx_INCREF(__pyx_t_8);
           __Pyx_INCREF(function);
           __Pyx_DECREF_SET(__pyx_t_7, function);
         }
       }
       __pyx_t_6 = (__pyx_t_8) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_8, __pyx_v_name) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_v_name);
       __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1019, __pyx_L4_error)
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1018, __pyx_L4_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1019, __pyx_L4_error)
+      __pyx_t_9 = __pyx_convert_string_from_py_std__in_string(__pyx_t_6); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1018, __pyx_L4_error)
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       try {
         __pyx_t_10 = new RtMidiOut(__pyx_v_rtapi, __pyx_t_9);
       } catch(...) {
         __Pyx_CppExn2PyErr();
-        __PYX_ERR(0, 1019, __pyx_L4_error)
+        __PYX_ERR(0, 1018, __pyx_L4_error)
       }
       __pyx_v_self->thisptr = __pyx_t_10;
 
-      /* "src/_rtmidi.pyx":1018
+      /* "_rtmidi.pyx":1017
  *             name = "RtMidiOut Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:
  */
     }
@@ -8953,65 +9052,65 @@
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L9_try_end;
     __pyx_L4_error:;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-    /* "src/_rtmidi.pyx":1020
+    /* "_rtmidi.pyx":1019
  *         try:
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:             # <<<<<<<<<<<<<<
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  */
     __pyx_t_11 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_RuntimeError);
     if (__pyx_t_11) {
-      __Pyx_AddTraceback("rtmidi._rtmidi.MidiOut.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 1020, __pyx_L6_except_error)
+      __Pyx_AddTraceback("_rtmidi.MidiOut.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      if (__Pyx_GetException(&__pyx_t_6, &__pyx_t_7, &__pyx_t_8) < 0) __PYX_ERR(0, 1019, __pyx_L6_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_INCREF(__pyx_t_7);
       __pyx_v_exc = __pyx_t_7;
       /*try:*/ {
 
-        /* "src/_rtmidi.pyx":1021
+        /* "_rtmidi.pyx":1020
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)             # <<<<<<<<<<<<<<
  * 
  *         self.set_error_callback(_default_error_handler)
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1021, __pyx_L15_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_12, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 1020, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_exc); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1021, __pyx_L15_error)
+        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyUnicode_Type)), __pyx_v_exc); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1020, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1021, __pyx_L15_error)
+        __pyx_t_14 = PyTuple_New(1); if (unlikely(!__pyx_t_14)) __PYX_ERR(0, 1020, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_14);
         __Pyx_GIVEREF(__pyx_t_13);
         PyTuple_SET_ITEM(__pyx_t_14, 0, __pyx_t_13);
         __pyx_t_13 = 0;
-        __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1021, __pyx_L15_error)
+        __pyx_t_13 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 1020, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_13);
-        __pyx_t_15 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 1021, __pyx_L15_error)
+        __pyx_t_15 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 1020, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_15);
-        if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_type, __pyx_t_15) < 0) __PYX_ERR(0, 1021, __pyx_L15_error)
+        if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_type, __pyx_t_15) < 0) __PYX_ERR(0, 1020, __pyx_L15_error)
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 1021, __pyx_L15_error)
+        __pyx_t_15 = __Pyx_PyObject_Call(__pyx_t_12, __pyx_t_14, __pyx_t_13); if (unlikely(!__pyx_t_15)) __PYX_ERR(0, 1020, __pyx_L15_error)
         __Pyx_GOTREF(__pyx_t_15);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
         __Pyx_Raise(__pyx_t_15, 0, 0, 0);
         __Pyx_DECREF(__pyx_t_15); __pyx_t_15 = 0;
-        __PYX_ERR(0, 1021, __pyx_L15_error)
+        __PYX_ERR(0, 1020, __pyx_L15_error)
       }
 
-      /* "src/_rtmidi.pyx":1020
+      /* "_rtmidi.pyx":1019
  *         try:
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:             # <<<<<<<<<<<<<<
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  */
       /*finally:*/ {
@@ -9052,85 +9151,85 @@
           goto __pyx_L6_except_error;
         }
       }
     }
     goto __pyx_L6_except_error;
     __pyx_L6_except_error:;
 
-    /* "src/_rtmidi.pyx":1018
+    /* "_rtmidi.pyx":1017
  *             name = "RtMidiOut Client"
  * 
  *         try:             # <<<<<<<<<<<<<<
  *             self.thisptr = new RtMidiOut(rtapi, _to_bytes(name))
  *         except RuntimeError as exc:
  */
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_XGIVEREF(__pyx_t_4);
     __Pyx_XGIVEREF(__pyx_t_5);
     __Pyx_ExceptionReset(__pyx_t_3, __pyx_t_4, __pyx_t_5);
     goto __pyx_L1_error;
     __pyx_L9_try_end:;
   }
 
-  /* "src/_rtmidi.pyx":1023
+  /* "_rtmidi.pyx":1022
  *             raise SystemError(str(exc), type=ERR_DRIVER_ERROR)
  * 
  *         self.set_error_callback(_default_error_handler)             # <<<<<<<<<<<<<<
  *         self._port = None
  *         self._deleted = False
  */
-  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1023, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_set_error_callback); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 1022, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1023, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_default_error_handler); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1022, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_15 = NULL;
   if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_15 = PyMethod_GET_SELF(__pyx_t_7);
     if (likely(__pyx_t_15)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
       __Pyx_INCREF(__pyx_t_15);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_7, function);
     }
   }
   __pyx_t_8 = (__pyx_t_15) ? __Pyx_PyObject_Call2Args(__pyx_t_7, __pyx_t_15, __pyx_t_6) : __Pyx_PyObject_CallOneArg(__pyx_t_7, __pyx_t_6);
   __Pyx_XDECREF(__pyx_t_15); __pyx_t_15 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1023, __pyx_L1_error)
+  if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 1022, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "src/_rtmidi.pyx":1024
+  /* "_rtmidi.pyx":1023
  * 
  *         self.set_error_callback(_default_error_handler)
  *         self._port = None             # <<<<<<<<<<<<<<
  *         self._deleted = False
  * 
  */
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base._port);
   __Pyx_DECREF(__pyx_v_self->__pyx_base._port);
   __pyx_v_self->__pyx_base._port = Py_None;
 
-  /* "src/_rtmidi.pyx":1025
+  /* "_rtmidi.pyx":1024
  *         self.set_error_callback(_default_error_handler)
  *         self._port = None
  *         self._deleted = False             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
   __Pyx_INCREF(Py_False);
   __Pyx_GIVEREF(Py_False);
   __Pyx_GOTREF(__pyx_v_self->__pyx_base._deleted);
   __Pyx_DECREF(__pyx_v_self->__pyx_base._deleted);
   __pyx_v_self->__pyx_base._deleted = Py_False;
 
-  /* "src/_rtmidi.pyx":1009
+  /* "_rtmidi.pyx":1008
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None):             # <<<<<<<<<<<<<<
  *         """Create a new client instance for MIDI output.
  * 
  */
 
@@ -9141,330 +9240,330 @@
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
   __Pyx_XDECREF(__pyx_t_12);
   __Pyx_XDECREF(__pyx_t_13);
   __Pyx_XDECREF(__pyx_t_14);
   __Pyx_XDECREF(__pyx_t_15);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiOut.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiOut.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_exc);
   __Pyx_XDECREF(__pyx_v_name);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":1027
+/* "_rtmidi.pyx":1026
  *         self._deleted = False
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  */
 
 /* Python wrapper */
-static void __pyx_pw_6rtmidi_7_rtmidi_7MidiOut_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
-static void __pyx_pw_6rtmidi_7_rtmidi_7MidiOut_3__dealloc__(PyObject *__pyx_v_self) {
+static void __pyx_pw_7_rtmidi_7MidiOut_3__dealloc__(PyObject *__pyx_v_self); /*proto*/
+static void __pyx_pw_7_rtmidi_7MidiOut_3__dealloc__(PyObject *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__dealloc__ (wrapper)", 0);
-  __pyx_pf_6rtmidi_7_rtmidi_7MidiOut_2__dealloc__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *)__pyx_v_self));
+  __pyx_pf_7_rtmidi_7MidiOut_2__dealloc__(((struct __pyx_obj_7_rtmidi_MidiOut *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-static void __pyx_pf_6rtmidi_7_rtmidi_7MidiOut_2__dealloc__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self) {
+static void __pyx_pf_7_rtmidi_7MidiOut_2__dealloc__(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "src/_rtmidi.pyx":1029
+  /* "_rtmidi.pyx":1028
  *     def __dealloc__(self):
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):             # <<<<<<<<<<<<<<
  *             del self.thisptr
  * 
  */
-  __pyx_t_1 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_thisptr); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1029, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_HasAttr(((PyObject *)__pyx_v_self), __pyx_n_u_thisptr); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 1028, __pyx_L1_error)
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "src/_rtmidi.pyx":1030
+    /* "_rtmidi.pyx":1029
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  *             del self.thisptr             # <<<<<<<<<<<<<<
  * 
  *     def delete(self):
  */
     delete __pyx_v_self->thisptr;
 
-    /* "src/_rtmidi.pyx":1029
+    /* "_rtmidi.pyx":1028
  *     def __dealloc__(self):
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):             # <<<<<<<<<<<<<<
  *             del self.thisptr
  * 
  */
   }
 
-  /* "src/_rtmidi.pyx":1027
+  /* "_rtmidi.pyx":1026
  *         self._deleted = False
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance."""
  *         if hasattr(self, "thisptr"):
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_WriteUnraisable("rtmidi._rtmidi.MidiOut.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __Pyx_WriteUnraisable("_rtmidi.MidiOut.__dealloc__", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "src/_rtmidi.pyx":1032
+/* "_rtmidi.pyx":1031
  *             del self.thisptr
  * 
  *     def delete(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_5delete(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_7MidiOut_4delete[] = "MidiOut.delete(self)\nDe-allocate pointer to C++ class instance.\n\n        .. warning:: the instance **must not** be used anymore after calling\n            this method, otherwise the program will crash with a segmentation\n            fault!\n\n            The reason this potentially dangerous method exists is that in\n            some cases it is desirable to destroy the internal ``RtMidiOut``\n            C++ class instance with immediate effect, thereby closing the\n            backend MIDI API client and all the ports it opened. By merely\n            using ``del`` on the ``rtmidi.MidiOut`` Python instance, the\n            destruction of the C++ instance may be delayed for an arbitrary\n            amount of time, until the Python garbage collector cleans up the\n            instance.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_5delete(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_5delete(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_7MidiOut_4delete[] = "MidiOut.delete(self)\nDe-allocate pointer to C++ class instance.\n\n        .. warning:: the instance **must not** be used anymore after calling\n            this method, otherwise the program will crash with a segmentation\n            fault!\n\n            The reason this potentially dangerous method exists is that in\n            some cases it is desirable to destroy the internal ``RtMidiOut``\n            C++ class instance with immediate effect, thereby closing the\n            backend MIDI API client and all the ports it opened. By merely\n            using ``del`` on the ``rtmidi.MidiOut`` Python instance, the\n            destruction of the C++ instance may be delayed for an arbitrary\n            amount of time, until the Python garbage collector cleans up the\n            instance.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_5delete(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("delete (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_7MidiOut_4delete(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_7MidiOut_4delete(((struct __pyx_obj_7_rtmidi_MidiOut *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_4delete(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_4delete(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("delete", 0);
 
-  /* "src/_rtmidi.pyx":1049
+  /* "_rtmidi.pyx":1048
  * 
  *         """
  *         if not self._deleted:             # <<<<<<<<<<<<<<
  *             del self.thisptr
  *             self._deleted = True
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->__pyx_base._deleted); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1049, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_self->__pyx_base._deleted); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1048, __pyx_L1_error)
   __pyx_t_2 = ((!__pyx_t_1) != 0);
   if (__pyx_t_2) {
 
-    /* "src/_rtmidi.pyx":1050
+    /* "_rtmidi.pyx":1049
  *         """
  *         if not self._deleted:
  *             del self.thisptr             # <<<<<<<<<<<<<<
  *             self._deleted = True
  * 
  */
     delete __pyx_v_self->thisptr;
 
-    /* "src/_rtmidi.pyx":1051
+    /* "_rtmidi.pyx":1050
  *         if not self._deleted:
  *             del self.thisptr
  *             self._deleted = True             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
     __Pyx_INCREF(Py_True);
     __Pyx_GIVEREF(Py_True);
     __Pyx_GOTREF(__pyx_v_self->__pyx_base._deleted);
     __Pyx_DECREF(__pyx_v_self->__pyx_base._deleted);
     __pyx_v_self->__pyx_base._deleted = Py_True;
 
-    /* "src/_rtmidi.pyx":1049
+    /* "_rtmidi.pyx":1048
  * 
  *         """
  *         if not self._deleted:             # <<<<<<<<<<<<<<
  *             del self.thisptr
  *             self._deleted = True
  */
   }
 
-  /* "src/_rtmidi.pyx":1032
+  /* "_rtmidi.pyx":1031
  *             del self.thisptr
  * 
  *     def delete(self):             # <<<<<<<<<<<<<<
  *         """De-allocate pointer to C++ class instance.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiOut.delete", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiOut.delete", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":1054
+/* "_rtmidi.pyx":1053
  * 
  *     @property
  *     def is_deleted(self):             # <<<<<<<<<<<<<<
  *         return self._deleted
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_10is_deleted_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_10is_deleted_1__get__(PyObject *__pyx_v_self) {
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_10is_deleted_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_10is_deleted_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_7MidiOut_10is_deleted___get__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_7MidiOut_10is_deleted___get__(((struct __pyx_obj_7_rtmidi_MidiOut *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_10is_deleted___get__(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_10is_deleted___get__(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "src/_rtmidi.pyx":1055
+  /* "_rtmidi.pyx":1054
  *     @property
  *     def is_deleted(self):
  *         return self._deleted             # <<<<<<<<<<<<<<
  * 
  *     def get_current_api(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->__pyx_base._deleted);
   __pyx_r = __pyx_v_self->__pyx_base._deleted;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":1054
+  /* "_rtmidi.pyx":1053
  * 
  *     @property
  *     def is_deleted(self):             # <<<<<<<<<<<<<<
  *         return self._deleted
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":1057
+/* "_rtmidi.pyx":1056
  *         return self._deleted
  * 
  *     def get_current_api(self):             # <<<<<<<<<<<<<<
  *         """Return the low-level MIDI backend API used by this instance.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_7get_current_api(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_7MidiOut_6get_current_api[] = "MidiOut.get_current_api(self)\nReturn the low-level MIDI backend API used by this instance.\n\n        Use this by comparing the returned value to the module-level ``API_*``\n        constants, e.g.::\n\n            midiout = rtmidi.MidiOut()\n\n            if midiout.get_current_api() == rtmidi.API_UNIX_JACK:\n                print(\"Using JACK API for MIDI output.\")\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_7get_current_api(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_7get_current_api(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_7MidiOut_6get_current_api[] = "MidiOut.get_current_api(self)\nReturn the low-level MIDI backend API used by this instance.\n\n        Use this by comparing the returned value to the module-level ``API_*``\n        constants, e.g.::\n\n            midiout = rtmidi.MidiOut()\n\n            if midiout.get_current_api() == rtmidi.API_UNIX_JACK:\n                print(\"Using JACK API for MIDI output.\")\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_7get_current_api(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("get_current_api (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_7MidiOut_6get_current_api(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_7MidiOut_6get_current_api(((struct __pyx_obj_7_rtmidi_MidiOut *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_6get_current_api(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_6get_current_api(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_current_api", 0);
 
-  /* "src/_rtmidi.pyx":1069
+  /* "_rtmidi.pyx":1068
  * 
  *         """
  *         return self.thisptr.getCurrentApi()             # <<<<<<<<<<<<<<
  * 
  *     def send_message(self, message):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(__pyx_v_self->thisptr->getCurrentApi()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1069, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(__pyx_v_self->thisptr->getCurrentApi()); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1068, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "src/_rtmidi.pyx":1057
+  /* "_rtmidi.pyx":1056
  *         return self._deleted
  * 
  *     def get_current_api(self):             # <<<<<<<<<<<<<<
  *         """Return the low-level MIDI backend API used by this instance.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiOut.get_current_api", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiOut.get_current_api", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "src/_rtmidi.pyx":1071
+/* "_rtmidi.pyx":1070
  *         return self.thisptr.getCurrentApi()
  * 
  *     def send_message(self, message):             # <<<<<<<<<<<<<<
  *         """Send a MIDI message to the output port.
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_9send_message(PyObject *__pyx_v_self, PyObject *__pyx_v_message); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_7MidiOut_8send_message[] = "MidiOut.send_message(self, message)\nSend a MIDI message to the output port.\n\n        The message must be passed as an iterable yielding integers, each\n        element representing one byte of the MIDI message.\n\n        Normal MIDI messages have a length of one to three bytes, but you can\n        also send system exclusive messages, which can be arbitrarily long, via\n        this method.\n\n        No check is made whether the passed data constitutes a valid MIDI\n        message but if it is longer than 3 bytes, the value of the first byte\n        must be a start-of-sysex status byte, i.e. 0xF0.\n\n        .. note:: with some backend APIs (notably ```WINDOWS_MM``) this function\n            blocks until the whole message is sent. While sending the message\n            the global interpreter lock is released, so multiple Python threads\n            can send messages using *different* MidiOut instances concurrently.\n\n        Exceptions:\n\n        ``ValueError``\n            Raised if ``message`` argument is empty or more than 3 bytes long\n            and not a SysEx message.\n\n        ";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_9send_message(PyObject *__pyx_v_self, PyObject *__pyx_v_message) {
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_9send_message(PyObject *__pyx_v_self, PyObject *__pyx_v_message); /*proto*/
+static char __pyx_doc_7_rtmidi_7MidiOut_8send_message[] = "MidiOut.send_message(self, message)\nSend a MIDI message to the output port.\n\n        The message must be passed as an iterable yielding integers, each\n        element representing one byte of the MIDI message.\n\n        Normal MIDI messages have a length of one to three bytes, but you can\n        also send system exclusive messages, which can be arbitrarily long, via\n        this method.\n\n        No check is made whether the passed data constitutes a valid MIDI\n        message but if it is longer than 3 bytes, the value of the first byte\n        must be a start-of-sysex status byte, i.e. 0xF0.\n\n        .. note:: with some backend APIs (notably ```WINDOWS_MM``) this function\n            blocks until the whole message is sent. While sending the message\n            the global interpreter lock is released, so multiple Python threads\n            can send messages using *different* MidiOut instances concurrently.\n\n        Exceptions:\n\n        ``ValueError``\n            Raised if ``message`` argument is empty or more than 3 bytes long\n            and not a SysEx message.\n\n        ";
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_9send_message(PyObject *__pyx_v_self, PyObject *__pyx_v_message) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("send_message (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_7MidiOut_8send_message(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *)__pyx_v_self), ((PyObject *)__pyx_v_message));
+  __pyx_r = __pyx_pf_7_rtmidi_7MidiOut_8send_message(((struct __pyx_obj_7_rtmidi_MidiOut *)__pyx_v_self), ((PyObject *)__pyx_v_message));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_8send_message(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self, PyObject *__pyx_v_message) {
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_8send_message(struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self, PyObject *__pyx_v_message) {
   std::vector<unsigned char>  __pyx_v_msg_v;
   PyObject *__pyx_v_c = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
@@ -9473,191 +9572,191 @@
   PyObject *(*__pyx_t_6)(PyObject *);
   unsigned char __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("send_message", 0);
 
-  /* "src/_rtmidi.pyx":1099
+  /* "_rtmidi.pyx":1098
  *         cdef vector[unsigned char] msg_v
  * 
  *         if not message:             # <<<<<<<<<<<<<<
  *             raise ValueError("'message' must not be empty.")
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_message); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1099, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_message); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1098, __pyx_L1_error)
   __pyx_t_2 = ((!__pyx_t_1) != 0);
   if (unlikely(__pyx_t_2)) {
 
-    /* "src/_rtmidi.pyx":1100
+    /* "_rtmidi.pyx":1099
  * 
  *         if not message:
  *             raise ValueError("'message' must not be empty.")             # <<<<<<<<<<<<<<
  * 
  *         if len(message) > 3 and message[0] != 0xF0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1100, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__8, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1099, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __PYX_ERR(0, 1100, __pyx_L1_error)
+    __PYX_ERR(0, 1099, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":1099
+    /* "_rtmidi.pyx":1098
  *         cdef vector[unsigned char] msg_v
  * 
  *         if not message:             # <<<<<<<<<<<<<<
  *             raise ValueError("'message' must not be empty.")
  * 
  */
   }
 
-  /* "src/_rtmidi.pyx":1102
+  /* "_rtmidi.pyx":1101
  *             raise ValueError("'message' must not be empty.")
  * 
  *         if len(message) > 3 and message[0] != 0xF0:             # <<<<<<<<<<<<<<
  *             raise ValueError("'message' longer than 3 bytes but does not "
  *                              "start with 0xF0.")
  */
-  __pyx_t_4 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1102, __pyx_L1_error)
+  __pyx_t_4 = PyObject_Length(__pyx_v_message); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 1101, __pyx_L1_error)
   __pyx_t_1 = ((__pyx_t_4 > 3) != 0);
   if (__pyx_t_1) {
   } else {
     __pyx_t_2 = __pyx_t_1;
     goto __pyx_L5_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_message, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1102, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_message, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_NeObjC(__pyx_t_3, __pyx_int_240, 0xF0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1102, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_NeObjC(__pyx_t_3, __pyx_int_240, 0xF0, 0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1101, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1102, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_5); if (unlikely(__pyx_t_1 < 0)) __PYX_ERR(0, 1101, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_2 = __pyx_t_1;
   __pyx_L5_bool_binop_done:;
   if (unlikely(__pyx_t_2)) {
 
-    /* "src/_rtmidi.pyx":1103
+    /* "_rtmidi.pyx":1102
  * 
  *         if len(message) > 3 and message[0] != 0xF0:
  *             raise ValueError("'message' longer than 3 bytes but does not "             # <<<<<<<<<<<<<<
  *                              "start with 0xF0.")
  * 
  */
-    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1103, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1102, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_Raise(__pyx_t_5, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    __PYX_ERR(0, 1103, __pyx_L1_error)
+    __PYX_ERR(0, 1102, __pyx_L1_error)
 
-    /* "src/_rtmidi.pyx":1102
+    /* "_rtmidi.pyx":1101
  *             raise ValueError("'message' must not be empty.")
  * 
  *         if len(message) > 3 and message[0] != 0xF0:             # <<<<<<<<<<<<<<
  *             raise ValueError("'message' longer than 3 bytes but does not "
  *                              "start with 0xF0.")
  */
   }
 
-  /* "src/_rtmidi.pyx":1106
+  /* "_rtmidi.pyx":1105
  *                              "start with 0xF0.")
  * 
  *         for c in message:             # <<<<<<<<<<<<<<
  *             msg_v.push_back(c)
  * 
  */
   if (likely(PyList_CheckExact(__pyx_v_message)) || PyTuple_CheckExact(__pyx_v_message)) {
     __pyx_t_5 = __pyx_v_message; __Pyx_INCREF(__pyx_t_5); __pyx_t_4 = 0;
     __pyx_t_6 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1106, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_5 = PyObject_GetIter(__pyx_v_message); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 1105, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
-    __pyx_t_6 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1106, __pyx_L1_error)
+    __pyx_t_6 = Py_TYPE(__pyx_t_5)->tp_iternext; if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 1105, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_6)) {
       if (likely(PyList_CheckExact(__pyx_t_5))) {
         if (__pyx_t_4 >= PyList_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 1106, __pyx_L1_error)
+        __pyx_t_3 = PyList_GET_ITEM(__pyx_t_5, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 1105, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1106, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1105, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       } else {
         if (__pyx_t_4 >= PyTuple_GET_SIZE(__pyx_t_5)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 1106, __pyx_L1_error)
+        __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_5, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely(0 < 0)) __PYX_ERR(0, 1105, __pyx_L1_error)
         #else
-        __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1106, __pyx_L1_error)
+        __pyx_t_3 = PySequence_ITEM(__pyx_t_5, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1105, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
         #endif
       }
     } else {
       __pyx_t_3 = __pyx_t_6(__pyx_t_5);
       if (unlikely(!__pyx_t_3)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 1106, __pyx_L1_error)
+          else __PYX_ERR(0, 1105, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_3);
     }
     __Pyx_XDECREF_SET(__pyx_v_c, __pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "src/_rtmidi.pyx":1107
+    /* "_rtmidi.pyx":1106
  * 
  *         for c in message:
  *             msg_v.push_back(c)             # <<<<<<<<<<<<<<
  * 
  *         with nogil:
  */
-    __pyx_t_7 = __Pyx_PyInt_As_unsigned_char(__pyx_v_c); if (unlikely((__pyx_t_7 == (unsigned char)-1) && PyErr_Occurred())) __PYX_ERR(0, 1107, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_As_unsigned_char(__pyx_v_c); if (unlikely((__pyx_t_7 == (unsigned char)-1) && PyErr_Occurred())) __PYX_ERR(0, 1106, __pyx_L1_error)
     try {
       __pyx_v_msg_v.push_back(__pyx_t_7);
     } catch(...) {
       __Pyx_CppExn2PyErr();
-      __PYX_ERR(0, 1107, __pyx_L1_error)
+      __PYX_ERR(0, 1106, __pyx_L1_error)
     }
 
-    /* "src/_rtmidi.pyx":1106
+    /* "_rtmidi.pyx":1105
  *                              "start with 0xF0.")
  * 
  *         for c in message:             # <<<<<<<<<<<<<<
  *             msg_v.push_back(c)
  * 
  */
   }
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
 
-  /* "src/_rtmidi.pyx":1109
+  /* "_rtmidi.pyx":1108
  *             msg_v.push_back(c)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             self.thisptr.sendMessage(&msg_v)
  */
   {
       #ifdef WITH_THREAD
       PyThreadState *_save;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "src/_rtmidi.pyx":1110
+        /* "_rtmidi.pyx":1109
  * 
  *         with nogil:
  *             self.thisptr.sendMessage(&msg_v)             # <<<<<<<<<<<<<<
  */
-        __pyx_v_self->thisptr->sendMessage((&__pyx_v_msg_v)); if (unlikely(__Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 1110, __pyx_L10_error)
+        __pyx_v_self->thisptr->sendMessage((&__pyx_v_msg_v)); if (unlikely(__Pyx_ErrOccurredWithGIL())) __PYX_ERR(0, 1109, __pyx_L10_error)
       }
 
-      /* "src/_rtmidi.pyx":1109
+      /* "_rtmidi.pyx":1108
  *             msg_v.push_back(c)
  * 
  *         with nogil:             # <<<<<<<<<<<<<<
  *             self.thisptr.sendMessage(&msg_v)
  */
       /*finally:*/ {
         /*normal exit:*/{
@@ -9674,29 +9773,29 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L11:;
       }
   }
 
-  /* "src/_rtmidi.pyx":1071
+  /* "_rtmidi.pyx":1070
  *         return self.thisptr.getCurrentApi()
  * 
  *     def send_message(self, message):             # <<<<<<<<<<<<<<
  *         """Send a MIDI message to the output port.
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiOut.send_message", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiOut.send_message", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_c);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
@@ -9704,28 +9803,28 @@
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_7MidiOut_10__reduce_cython__[] = "MidiOut.__reduce_cython__(self)";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static char __pyx_doc_7_rtmidi_7MidiOut_10__reduce_cython__[] = "MidiOut.__reduce_cython__(self)";
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_11__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_7MidiOut_10__reduce_cython__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7_rtmidi_7MidiOut_10__reduce_cython__(((struct __pyx_obj_7_rtmidi_MidiOut *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self) {
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_10__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
@@ -9747,43 +9846,43 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiOut.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiOut.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_7MidiOut_12__setstate_cython__[] = "MidiOut.__setstate_cython__(self, __pyx_state)";
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static char __pyx_doc_7_rtmidi_7MidiOut_12__setstate_cython__[] = "MidiOut.__setstate_cython__(self, __pyx_state)";
+static PyObject *__pyx_pw_7_rtmidi_7MidiOut_13__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_7MidiOut_12__setstate_cython__(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
+  __pyx_r = __pyx_pf_7_rtmidi_7MidiOut_12__setstate_cython__(((struct __pyx_obj_7_rtmidi_MidiOut *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_7MidiOut_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7_rtmidi_7MidiOut_12__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_7_rtmidi_MidiOut *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
@@ -9805,32 +9904,32 @@
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("rtmidi._rtmidi.MidiOut.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.MidiOut.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __pyx_unpickle_MidiBase(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_15__pyx_unpickle_MidiBase(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_6rtmidi_7_rtmidi_14__pyx_unpickle_MidiBase[] = "__pyx_unpickle_MidiBase(__pyx_type, long __pyx_checksum, __pyx_state)";
-static PyMethodDef __pyx_mdef_6rtmidi_7_rtmidi_15__pyx_unpickle_MidiBase = {"__pyx_unpickle_MidiBase", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_15__pyx_unpickle_MidiBase, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_14__pyx_unpickle_MidiBase};
-static PyObject *__pyx_pw_6rtmidi_7_rtmidi_15__pyx_unpickle_MidiBase(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_7_rtmidi_15__pyx_unpickle_MidiBase(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_7_rtmidi_14__pyx_unpickle_MidiBase[] = "__pyx_unpickle_MidiBase(__pyx_type, long __pyx_checksum, __pyx_state)";
+static PyMethodDef __pyx_mdef_7_rtmidi_15__pyx_unpickle_MidiBase = {"__pyx_unpickle_MidiBase", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_15__pyx_unpickle_MidiBase, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_14__pyx_unpickle_MidiBase};
+static PyObject *__pyx_pw_7_rtmidi_15__pyx_unpickle_MidiBase(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -9884,167 +9983,171 @@
     __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_MidiBase", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("rtmidi._rtmidi.__pyx_unpickle_MidiBase", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.__pyx_unpickle_MidiBase", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_6rtmidi_7_rtmidi_14__pyx_unpickle_MidiBase(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_7_rtmidi_14__pyx_unpickle_MidiBase(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_6rtmidi_7_rtmidi_14__pyx_unpickle_MidiBase(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7_rtmidi_14__pyx_unpickle_MidiBase(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
   PyObject *__pyx_t_4 = NULL;
   PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_MidiBase", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x9171c0f:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x9171c0f, 0x2133db3, 0x021d8b9):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9171c0f = (_deleted, _error_callback, _port))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9171c0f, 0x2133db3, 0x021d8b9) = (_deleted, _error_callback, _port))" % __pyx_checksum)
  */
-  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0x9171c0f) != 0);
-  if (__pyx_t_1) {
+  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__12, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x9171c0f:
+ *     if __pyx_checksum not in (0x9171c0f, 0x2133db3, 0x021d8b9):
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9171c0f = (_deleted, _error_callback, _port))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9171c0f, 0x2133db3, 0x021d8b9) = (_deleted, _error_callback, _port))" % __pyx_checksum)
  *     __pyx_result = MidiBase.__new__(__pyx_type)
  */
-    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_INCREF(__pyx_t_2);
-    __pyx_v___pyx_PickleError = __pyx_t_2;
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
+    __pyx_t_4 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_4, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_t_1);
+    __pyx_v___pyx_PickleError = __pyx_t_1;
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum != 0x9171c0f:
+ *     if __pyx_checksum not in (0x9171c0f, 0x2133db3, 0x021d8b9):
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9171c0f = (_deleted, _error_callback, _port))" % __pyx_checksum)             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9171c0f, 0x2133db3, 0x021d8b9) = (_deleted, _error_callback, _port))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = MidiBase.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0x91, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_5 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_INCREF(__pyx_v___pyx_PickleError);
-    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
-    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
-      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
-      if (likely(__pyx_t_5)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-        __Pyx_INCREF(__pyx_t_5);
+    __pyx_t_1 = __pyx_v___pyx_PickleError; __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_1))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_1);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+        __Pyx_INCREF(__pyx_t_6);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_2, function);
+        __Pyx_DECREF_SET(__pyx_t_1, function);
       }
     }
-    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
-    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __pyx_t_4 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_6, __pyx_t_5) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_t_5);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_Raise(__pyx_t_4, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum != 0x9171c0f:             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum not in (0x9171c0f, 0x2133db3, 0x021d8b9):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9171c0f = (_deleted, _error_callback, _port))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9171c0f, 0x2133db3, 0x021d8b9) = (_deleted, _error_callback, _port))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9171c0f = (_deleted, _error_callback, _port))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9171c0f, 0x2133db3, 0x021d8b9) = (_deleted, _error_callback, _port))" % __pyx_checksum)
  *     __pyx_result = MidiBase.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_MidiBase__set_state(<MidiBase> __pyx_result, __pyx_state)
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6rtmidi_7_rtmidi_MidiBase), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_4 = NULL;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
-    if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
-      __Pyx_INCREF(__pyx_t_4);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7_rtmidi_MidiBase), __pyx_n_s_new); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = NULL;
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_1))) {
+    __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_1);
+    if (likely(__pyx_t_5)) {
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+      __Pyx_INCREF(__pyx_t_5);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_2, function);
+      __Pyx_DECREF_SET(__pyx_t_1, function);
     }
   }
-  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
-  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_v___pyx_result = __pyx_t_3;
-  __pyx_t_3 = 0;
+  __pyx_t_4 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_1, __pyx_t_5, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_1, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+  if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v___pyx_result = __pyx_t_4;
+  __pyx_t_4 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9171c0f = (_deleted, _error_callback, _port))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9171c0f, 0x2133db3, 0x021d8b9) = (_deleted, _error_callback, _port))" % __pyx_checksum)
  *     __pyx_result = MidiBase.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_MidiBase__set_state(<MidiBase> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
-  __pyx_t_6 = (__pyx_t_1 != 0);
-  if (__pyx_t_6) {
+  __pyx_t_3 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_2 = (__pyx_t_3 != 0);
+  if (__pyx_t_2) {
 
     /* "(tree fragment)":9
  *     __pyx_result = MidiBase.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_MidiBase__set_state(<MidiBase> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_MidiBase__set_state(MidiBase __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_3 = __pyx_f_6rtmidi_7_rtmidi___pyx_unpickle_MidiBase__set_state(((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_4 = __pyx_f_7_rtmidi___pyx_unpickle_MidiBase__set_state(((struct __pyx_obj_7_rtmidi_MidiBase *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError("Incompatible checksums (%s vs 0x9171c0f = (_deleted, _error_callback, _port))" % __pyx_checksum)
+ *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0x9171c0f, 0x2133db3, 0x021d8b9) = (_deleted, _error_callback, _port))" % __pyx_checksum)
  *     __pyx_result = MidiBase.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_MidiBase__set_state(<MidiBase> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -10064,19 +10167,19 @@
  * def __pyx_unpickle_MidiBase(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
-  __Pyx_AddTraceback("rtmidi._rtmidi.__pyx_unpickle_MidiBase", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("_rtmidi.__pyx_unpickle_MidiBase", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -10086,15 +10189,15 @@
  *         __pyx_unpickle_MidiBase__set_state(<MidiBase> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_MidiBase__set_state(MidiBase __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result._deleted = __pyx_state[0]; __pyx_result._error_callback = __pyx_state[1]; __pyx_result._port = __pyx_state[2]
  *     if len(__pyx_state) > 3 and hasattr(__pyx_result, '__dict__'):
  */
 
-static PyObject *__pyx_f_6rtmidi_7_rtmidi___pyx_unpickle_MidiBase__set_state(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_f_7_rtmidi___pyx_unpickle_MidiBase__set_state(struct __pyx_obj_7_rtmidi_MidiBase *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
@@ -10224,15 +10327,15 @@
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("rtmidi._rtmidi.__pyx_unpickle_MidiBase__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("_rtmidi.__pyx_unpickle_MidiBase__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
@@ -10545,104 +10648,104 @@
   __pyx_L1_error:;
   __Pyx_AddTraceback("string.from_py.__pyx_convert_string_from_py_std__in_string", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_pretend_to_initialize(&__pyx_r);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase __pyx_vtable_6rtmidi_7_rtmidi_MidiBase;
+static struct __pyx_vtabstruct_7_rtmidi_MidiBase __pyx_vtable_7_rtmidi_MidiBase;
 
-static PyObject *__pyx_tp_new_6rtmidi_7_rtmidi_MidiBase(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *p;
+static PyObject *__pyx_tp_new_7_rtmidi_MidiBase(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_7_rtmidi_MidiBase *p;
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)o);
-  p->__pyx_vtab = __pyx_vtabptr_6rtmidi_7_rtmidi_MidiBase;
+  p = ((struct __pyx_obj_7_rtmidi_MidiBase *)o);
+  p->__pyx_vtab = __pyx_vtabptr_7_rtmidi_MidiBase;
   p->_port = Py_None; Py_INCREF(Py_None);
   p->_error_callback = Py_None; Py_INCREF(Py_None);
   p->_deleted = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
-static void __pyx_tp_dealloc_6rtmidi_7_rtmidi_MidiBase(PyObject *o) {
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *p = (struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)o;
+static void __pyx_tp_dealloc_7_rtmidi_MidiBase(PyObject *o) {
+  struct __pyx_obj_7_rtmidi_MidiBase *p = (struct __pyx_obj_7_rtmidi_MidiBase *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->_port);
   Py_CLEAR(p->_error_callback);
   Py_CLEAR(p->_deleted);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static int __pyx_tp_traverse_6rtmidi_7_rtmidi_MidiBase(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_7_rtmidi_MidiBase(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *p = (struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)o;
+  struct __pyx_obj_7_rtmidi_MidiBase *p = (struct __pyx_obj_7_rtmidi_MidiBase *)o;
   if (p->_port) {
     e = (*v)(p->_port, a); if (e) return e;
   }
   if (p->_error_callback) {
     e = (*v)(p->_error_callback, a); if (e) return e;
   }
   if (p->_deleted) {
     e = (*v)(p->_deleted, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_6rtmidi_7_rtmidi_MidiBase(PyObject *o) {
+static int __pyx_tp_clear_7_rtmidi_MidiBase(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *p = (struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *)o;
+  struct __pyx_obj_7_rtmidi_MidiBase *p = (struct __pyx_obj_7_rtmidi_MidiBase *)o;
   tmp = ((PyObject*)p->_port);
   p->_port = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->_error_callback);
   p->_error_callback = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   tmp = ((PyObject*)p->_deleted);
   p->_deleted = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyMethodDef __pyx_methods_6rtmidi_7_rtmidi_MidiBase[] = {
-  {"__enter__", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_1__enter__, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase___enter__},
-  {"__exit__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_3__exit__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_2__exit__},
-  {"_check_port", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_5_check_port, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_4_check_port},
-  {"_decode_string", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_7_decode_string, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_6_decode_string},
-  {"get_port_count", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_9get_port_count, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_8get_port_count},
-  {"get_port_name", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_11get_port_name, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_10get_port_name},
-  {"get_ports", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_13get_ports, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_12get_ports},
-  {"is_port_open", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_15is_port_open, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_14is_port_open},
-  {"open_port", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_17open_port, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_16open_port},
-  {"open_virtual_port", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_19open_virtual_port, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_18open_virtual_port},
-  {"close_port", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_21close_port, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_20close_port},
-  {"set_client_name", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_23set_client_name, METH_O, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_22set_client_name},
-  {"set_port_name", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_25set_port_name, METH_O, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_24set_port_name},
-  {"set_error_callback", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_27set_error_callback, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_26set_error_callback},
-  {"cancel_error_callback", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_29cancel_error_callback, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_28cancel_error_callback},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_31__reduce_cython__, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_30__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_8MidiBase_33__setstate_cython__, METH_O, __pyx_doc_6rtmidi_7_rtmidi_8MidiBase_32__setstate_cython__},
+static PyMethodDef __pyx_methods_7_rtmidi_MidiBase[] = {
+  {"__enter__", (PyCFunction)__pyx_pw_7_rtmidi_8MidiBase_1__enter__, METH_NOARGS, __pyx_doc_7_rtmidi_8MidiBase___enter__},
+  {"__exit__", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_8MidiBase_3__exit__, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_8MidiBase_2__exit__},
+  {"_check_port", (PyCFunction)__pyx_pw_7_rtmidi_8MidiBase_5_check_port, METH_NOARGS, __pyx_doc_7_rtmidi_8MidiBase_4_check_port},
+  {"_decode_string", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_8MidiBase_7_decode_string, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_8MidiBase_6_decode_string},
+  {"get_port_count", (PyCFunction)__pyx_pw_7_rtmidi_8MidiBase_9get_port_count, METH_NOARGS, __pyx_doc_7_rtmidi_8MidiBase_8get_port_count},
+  {"get_port_name", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_8MidiBase_11get_port_name, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_8MidiBase_10get_port_name},
+  {"get_ports", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_8MidiBase_13get_ports, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_8MidiBase_12get_ports},
+  {"is_port_open", (PyCFunction)__pyx_pw_7_rtmidi_8MidiBase_15is_port_open, METH_NOARGS, __pyx_doc_7_rtmidi_8MidiBase_14is_port_open},
+  {"open_port", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_8MidiBase_17open_port, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_8MidiBase_16open_port},
+  {"open_virtual_port", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_8MidiBase_19open_virtual_port, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_8MidiBase_18open_virtual_port},
+  {"close_port", (PyCFunction)__pyx_pw_7_rtmidi_8MidiBase_21close_port, METH_NOARGS, __pyx_doc_7_rtmidi_8MidiBase_20close_port},
+  {"set_client_name", (PyCFunction)__pyx_pw_7_rtmidi_8MidiBase_23set_client_name, METH_O, __pyx_doc_7_rtmidi_8MidiBase_22set_client_name},
+  {"set_port_name", (PyCFunction)__pyx_pw_7_rtmidi_8MidiBase_25set_port_name, METH_O, __pyx_doc_7_rtmidi_8MidiBase_24set_port_name},
+  {"set_error_callback", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_8MidiBase_27set_error_callback, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_8MidiBase_26set_error_callback},
+  {"cancel_error_callback", (PyCFunction)__pyx_pw_7_rtmidi_8MidiBase_29cancel_error_callback, METH_NOARGS, __pyx_doc_7_rtmidi_8MidiBase_28cancel_error_callback},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_7_rtmidi_8MidiBase_31__reduce_cython__, METH_NOARGS, __pyx_doc_7_rtmidi_8MidiBase_30__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_7_rtmidi_8MidiBase_33__setstate_cython__, METH_O, __pyx_doc_7_rtmidi_8MidiBase_32__setstate_cython__},
   {0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_6rtmidi_7_rtmidi_MidiBase = {
+static PyTypeObject __pyx_type_7_rtmidi_MidiBase = {
   PyVarObject_HEAD_INIT(0, 0)
-  "rtmidi._rtmidi.MidiBase", /*tp_name*/
-  sizeof(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase), /*tp_basicsize*/
+  "_rtmidi.MidiBase", /*tp_name*/
+  sizeof(struct __pyx_obj_7_rtmidi_MidiBase), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_6rtmidi_7_rtmidi_MidiBase, /*tp_dealloc*/
+  __pyx_tp_dealloc_7_rtmidi_MidiBase, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -10661,135 +10764,138 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   0, /*tp_doc*/
-  __pyx_tp_traverse_6rtmidi_7_rtmidi_MidiBase, /*tp_traverse*/
-  __pyx_tp_clear_6rtmidi_7_rtmidi_MidiBase, /*tp_clear*/
+  __pyx_tp_traverse_7_rtmidi_MidiBase, /*tp_traverse*/
+  __pyx_tp_clear_7_rtmidi_MidiBase, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_6rtmidi_7_rtmidi_MidiBase, /*tp_methods*/
+  __pyx_methods_7_rtmidi_MidiBase, /*tp_methods*/
   0, /*tp_members*/
   0, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_6rtmidi_7_rtmidi_MidiBase, /*tp_new*/
+  __pyx_tp_new_7_rtmidi_MidiBase, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
-static struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiIn __pyx_vtable_6rtmidi_7_rtmidi_MidiIn;
+static struct __pyx_vtabstruct_7_rtmidi_MidiIn __pyx_vtable_7_rtmidi_MidiIn;
 
-static PyObject *__pyx_tp_new_6rtmidi_7_rtmidi_MidiIn(PyTypeObject *t, PyObject *a, PyObject *k) {
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *p;
-  PyObject *o = __pyx_tp_new_6rtmidi_7_rtmidi_MidiBase(t, a, k);
+static PyObject *__pyx_tp_new_7_rtmidi_MidiIn(PyTypeObject *t, PyObject *a, PyObject *k) {
+  struct __pyx_obj_7_rtmidi_MidiIn *p;
+  PyObject *o = __pyx_tp_new_7_rtmidi_MidiBase(t, a, k);
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)o);
-  p->__pyx_base.__pyx_vtab = (struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase*)__pyx_vtabptr_6rtmidi_7_rtmidi_MidiIn;
+  p = ((struct __pyx_obj_7_rtmidi_MidiIn *)o);
+  p->__pyx_base.__pyx_vtab = (struct __pyx_vtabstruct_7_rtmidi_MidiBase*)__pyx_vtabptr_7_rtmidi_MidiIn;
   p->_callback = Py_None; Py_INCREF(Py_None);
-  if (unlikely(__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_1__cinit__(o, a, k) < 0)) goto bad;
+  if (unlikely(__pyx_pw_7_rtmidi_6MidiIn_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_6rtmidi_7_rtmidi_MidiIn(PyObject *o) {
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *p = (struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)o;
+static void __pyx_tp_dealloc_7_rtmidi_MidiIn(PyObject *o) {
+  struct __pyx_obj_7_rtmidi_MidiIn *p = (struct __pyx_obj_7_rtmidi_MidiIn *)o;
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_6rtmidi_7_rtmidi_6MidiIn_5__dealloc__(o);
+    __pyx_pw_7_rtmidi_6MidiIn_5__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   Py_CLEAR(p->_callback);
   PyObject_GC_Track(o);
-  __pyx_tp_dealloc_6rtmidi_7_rtmidi_MidiBase(o);
+  __pyx_tp_dealloc_7_rtmidi_MidiBase(o);
 }
 
-static int __pyx_tp_traverse_6rtmidi_7_rtmidi_MidiIn(PyObject *o, visitproc v, void *a) {
+static int __pyx_tp_traverse_7_rtmidi_MidiIn(PyObject *o, visitproc v, void *a) {
   int e;
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *p = (struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)o;
-  e = __pyx_tp_traverse_6rtmidi_7_rtmidi_MidiBase(o, v, a); if (e) return e;
+  struct __pyx_obj_7_rtmidi_MidiIn *p = (struct __pyx_obj_7_rtmidi_MidiIn *)o;
+  e = __pyx_tp_traverse_7_rtmidi_MidiBase(o, v, a); if (e) return e;
   if (p->_callback) {
     e = (*v)(p->_callback, a); if (e) return e;
   }
   return 0;
 }
 
-static int __pyx_tp_clear_6rtmidi_7_rtmidi_MidiIn(PyObject *o) {
+static int __pyx_tp_clear_7_rtmidi_MidiIn(PyObject *o) {
   PyObject* tmp;
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *p = (struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn *)o;
-  __pyx_tp_clear_6rtmidi_7_rtmidi_MidiBase(o);
+  struct __pyx_obj_7_rtmidi_MidiIn *p = (struct __pyx_obj_7_rtmidi_MidiIn *)o;
+  __pyx_tp_clear_7_rtmidi_MidiBase(o);
   tmp = ((PyObject*)p->_callback);
   p->_callback = Py_None; Py_INCREF(Py_None);
   Py_XDECREF(tmp);
   return 0;
 }
 
-static PyObject *__pyx_getprop_6rtmidi_7_rtmidi_6MidiIn_is_deleted(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_6rtmidi_7_rtmidi_6MidiIn_10is_deleted_1__get__(o);
+static PyObject *__pyx_getprop_7_rtmidi_6MidiIn_is_deleted(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7_rtmidi_6MidiIn_10is_deleted_1__get__(o);
 }
 
-static PyMethodDef __pyx_methods_6rtmidi_7_rtmidi_MidiIn[] = {
-  {"get_current_api", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_3get_current_api, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_2get_current_api},
-  {"delete", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_7delete, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_6delete},
-  {"cancel_callback", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_9cancel_callback, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_8cancel_callback},
-  {"close_port", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_11close_port, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_10close_port},
-  {"get_message", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_13get_message, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_12get_message},
-  {"ignore_types", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_15ignore_types, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_14ignore_types},
-  {"set_callback", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_17set_callback, METH_VARARGS|METH_KEYWORDS, __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_16set_callback},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_19__reduce_cython__, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_18__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_6MidiIn_21__setstate_cython__, METH_O, __pyx_doc_6rtmidi_7_rtmidi_6MidiIn_20__setstate_cython__},
+static PyMethodDef __pyx_methods_7_rtmidi_MidiIn[] = {
+  {"get_current_api", (PyCFunction)__pyx_pw_7_rtmidi_6MidiIn_3get_current_api, METH_NOARGS, __pyx_doc_7_rtmidi_6MidiIn_2get_current_api},
+  {"delete", (PyCFunction)__pyx_pw_7_rtmidi_6MidiIn_7delete, METH_NOARGS, __pyx_doc_7_rtmidi_6MidiIn_6delete},
+  {"cancel_callback", (PyCFunction)__pyx_pw_7_rtmidi_6MidiIn_9cancel_callback, METH_NOARGS, __pyx_doc_7_rtmidi_6MidiIn_8cancel_callback},
+  {"close_port", (PyCFunction)__pyx_pw_7_rtmidi_6MidiIn_11close_port, METH_NOARGS, __pyx_doc_7_rtmidi_6MidiIn_10close_port},
+  {"get_message", (PyCFunction)__pyx_pw_7_rtmidi_6MidiIn_13get_message, METH_NOARGS, __pyx_doc_7_rtmidi_6MidiIn_12get_message},
+  {"ignore_types", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_6MidiIn_15ignore_types, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_6MidiIn_14ignore_types},
+  {"set_callback", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7_rtmidi_6MidiIn_17set_callback, METH_VARARGS|METH_KEYWORDS, __pyx_doc_7_rtmidi_6MidiIn_16set_callback},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_7_rtmidi_6MidiIn_19__reduce_cython__, METH_NOARGS, __pyx_doc_7_rtmidi_6MidiIn_18__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_7_rtmidi_6MidiIn_21__setstate_cython__, METH_O, __pyx_doc_7_rtmidi_6MidiIn_20__setstate_cython__},
   {0, 0, 0, 0}
 };
 
-static struct PyGetSetDef __pyx_getsets_6rtmidi_7_rtmidi_MidiIn[] = {
-  {(char *)"is_deleted", __pyx_getprop_6rtmidi_7_rtmidi_6MidiIn_is_deleted, 0, (char *)0, 0},
+static struct PyGetSetDef __pyx_getsets_7_rtmidi_MidiIn[] = {
+  {(char *)"is_deleted", __pyx_getprop_7_rtmidi_6MidiIn_is_deleted, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_6rtmidi_7_rtmidi_MidiIn = {
+static PyTypeObject __pyx_type_7_rtmidi_MidiIn = {
   PyVarObject_HEAD_INIT(0, 0)
-  "rtmidi._rtmidi.MidiIn", /*tp_name*/
-  sizeof(struct __pyx_obj_6rtmidi_7_rtmidi_MidiIn), /*tp_basicsize*/
+  "_rtmidi.MidiIn", /*tp_name*/
+  sizeof(struct __pyx_obj_7_rtmidi_MidiIn), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_6rtmidi_7_rtmidi_MidiIn, /*tp_dealloc*/
+  __pyx_tp_dealloc_7_rtmidi_MidiIn, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -10808,108 +10914,111 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   "Midi input client interface.\n\n    ``rtmidi.MidiIn(rtapi=API_UNSPECIFIED, name=\"RtMidi Client\", queue_size_limit=1024)``\n\n    You can specify the low-level MIDI backend API to use via the ``rtapi``\n    keyword or the first positional argument, passing one of the module-level\n    ``API_*`` constants. You can get a list of compiled-in APIs with the\n    module-level ``get_compiled_api`` function. If you pass ``API_UNSPECIFIED``\n    (the default), the first compiled-in API, which has any input ports\n    available, will be used.\n\n    You can optionally pass a name for the MIDI client with the ``name``\n    keyword or the second positional argument. Names with non-ASCII characters\n    in them have to be passed as unicode or UTF-8 encoded strings in Python 2.\n    The default name is ``\"RtMidiIn Client\"``.\n\n    .. note::\n        With some backend APIs (e.g. ALSA), the client name is set by the first\n        ``MidiIn`` *or* ``MidiOut`` created by your program and does not change\n        unless you either use the ``set_client_name`` method, or until *all*\n        ``MidiIn`` and ``MidiOut`` instances are deleted and then a new one is\n        created.\n\n    The ``queue_size_limit`` argument specifies the size of the internal ring\n    buffer in which incoming MIDI events are placed until retrieved via the\n    ``get_message`` method (i.e. when no callback function is registered).\n    The default value is ``1024`` (overriding the default value ``100`` of the\n    underlying C++ RtMidi library).\n\n    Exceptions:\n\n    ``SystemError``\n        Raised when the RtMidi backend initialization fails. The execption\n        message should have more information on the cause of the error.\n\n    ``TypeError``\n        Raised when an incompatible value type is passed for a parameter.\n\n    ", /*tp_doc*/
-  __pyx_tp_traverse_6rtmidi_7_rtmidi_MidiIn, /*tp_traverse*/
-  __pyx_tp_clear_6rtmidi_7_rtmidi_MidiIn, /*tp_clear*/
+  __pyx_tp_traverse_7_rtmidi_MidiIn, /*tp_traverse*/
+  __pyx_tp_clear_7_rtmidi_MidiIn, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_6rtmidi_7_rtmidi_MidiIn, /*tp_methods*/
+  __pyx_methods_7_rtmidi_MidiIn, /*tp_methods*/
   0, /*tp_members*/
-  __pyx_getsets_6rtmidi_7_rtmidi_MidiIn, /*tp_getset*/
+  __pyx_getsets_7_rtmidi_MidiIn, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_6rtmidi_7_rtmidi_MidiIn, /*tp_new*/
+  __pyx_tp_new_7_rtmidi_MidiIn, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
-static struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiOut __pyx_vtable_6rtmidi_7_rtmidi_MidiOut;
+static struct __pyx_vtabstruct_7_rtmidi_MidiOut __pyx_vtable_7_rtmidi_MidiOut;
 
-static PyObject *__pyx_tp_new_6rtmidi_7_rtmidi_MidiOut(PyTypeObject *t, PyObject *a, PyObject *k) {
-  struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *p;
-  PyObject *o = __pyx_tp_new_6rtmidi_7_rtmidi_MidiBase(t, a, k);
+static PyObject *__pyx_tp_new_7_rtmidi_MidiOut(PyTypeObject *t, PyObject *a, PyObject *k) {
+  struct __pyx_obj_7_rtmidi_MidiOut *p;
+  PyObject *o = __pyx_tp_new_7_rtmidi_MidiBase(t, a, k);
   if (unlikely(!o)) return 0;
-  p = ((struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut *)o);
-  p->__pyx_base.__pyx_vtab = (struct __pyx_vtabstruct_6rtmidi_7_rtmidi_MidiBase*)__pyx_vtabptr_6rtmidi_7_rtmidi_MidiOut;
-  if (unlikely(__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_1__cinit__(o, a, k) < 0)) goto bad;
+  p = ((struct __pyx_obj_7_rtmidi_MidiOut *)o);
+  p->__pyx_base.__pyx_vtab = (struct __pyx_vtabstruct_7_rtmidi_MidiBase*)__pyx_vtabptr_7_rtmidi_MidiOut;
+  if (unlikely(__pyx_pw_7_rtmidi_7MidiOut_1__cinit__(o, a, k) < 0)) goto bad;
   return o;
   bad:
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
-static void __pyx_tp_dealloc_6rtmidi_7_rtmidi_MidiOut(PyObject *o) {
+static void __pyx_tp_dealloc_7_rtmidi_MidiOut(PyObject *o) {
   #if CYTHON_USE_TP_FINALIZE
   if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
-    __pyx_pw_6rtmidi_7_rtmidi_7MidiOut_3__dealloc__(o);
+    __pyx_pw_7_rtmidi_7MidiOut_3__dealloc__(o);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) - 1);
     PyErr_Restore(etype, eval, etb);
   }
   PyObject_GC_Track(o);
-  __pyx_tp_dealloc_6rtmidi_7_rtmidi_MidiBase(o);
+  __pyx_tp_dealloc_7_rtmidi_MidiBase(o);
 }
 
-static PyObject *__pyx_getprop_6rtmidi_7_rtmidi_7MidiOut_is_deleted(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_6rtmidi_7_rtmidi_7MidiOut_10is_deleted_1__get__(o);
+static PyObject *__pyx_getprop_7_rtmidi_7MidiOut_is_deleted(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7_rtmidi_7MidiOut_10is_deleted_1__get__(o);
 }
 
-static PyMethodDef __pyx_methods_6rtmidi_7_rtmidi_MidiOut[] = {
-  {"delete", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_5delete, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_7MidiOut_4delete},
-  {"get_current_api", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_7get_current_api, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_7MidiOut_6get_current_api},
-  {"send_message", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_9send_message, METH_O, __pyx_doc_6rtmidi_7_rtmidi_7MidiOut_8send_message},
-  {"__reduce_cython__", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_11__reduce_cython__, METH_NOARGS, __pyx_doc_6rtmidi_7_rtmidi_7MidiOut_10__reduce_cython__},
-  {"__setstate_cython__", (PyCFunction)__pyx_pw_6rtmidi_7_rtmidi_7MidiOut_13__setstate_cython__, METH_O, __pyx_doc_6rtmidi_7_rtmidi_7MidiOut_12__setstate_cython__},
+static PyMethodDef __pyx_methods_7_rtmidi_MidiOut[] = {
+  {"delete", (PyCFunction)__pyx_pw_7_rtmidi_7MidiOut_5delete, METH_NOARGS, __pyx_doc_7_rtmidi_7MidiOut_4delete},
+  {"get_current_api", (PyCFunction)__pyx_pw_7_rtmidi_7MidiOut_7get_current_api, METH_NOARGS, __pyx_doc_7_rtmidi_7MidiOut_6get_current_api},
+  {"send_message", (PyCFunction)__pyx_pw_7_rtmidi_7MidiOut_9send_message, METH_O, __pyx_doc_7_rtmidi_7MidiOut_8send_message},
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_7_rtmidi_7MidiOut_11__reduce_cython__, METH_NOARGS, __pyx_doc_7_rtmidi_7MidiOut_10__reduce_cython__},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_7_rtmidi_7MidiOut_13__setstate_cython__, METH_O, __pyx_doc_7_rtmidi_7MidiOut_12__setstate_cython__},
   {0, 0, 0, 0}
 };
 
-static struct PyGetSetDef __pyx_getsets_6rtmidi_7_rtmidi_MidiOut[] = {
-  {(char *)"is_deleted", __pyx_getprop_6rtmidi_7_rtmidi_7MidiOut_is_deleted, 0, (char *)0, 0},
+static struct PyGetSetDef __pyx_getsets_7_rtmidi_MidiOut[] = {
+  {(char *)"is_deleted", __pyx_getprop_7_rtmidi_7MidiOut_is_deleted, 0, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
 
-static PyTypeObject __pyx_type_6rtmidi_7_rtmidi_MidiOut = {
+static PyTypeObject __pyx_type_7_rtmidi_MidiOut = {
   PyVarObject_HEAD_INIT(0, 0)
-  "rtmidi._rtmidi.MidiOut", /*tp_name*/
-  sizeof(struct __pyx_obj_6rtmidi_7_rtmidi_MidiOut), /*tp_basicsize*/
+  "_rtmidi.MidiOut", /*tp_name*/
+  sizeof(struct __pyx_obj_7_rtmidi_MidiOut), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_6rtmidi_7_rtmidi_MidiOut, /*tp_dealloc*/
+  __pyx_tp_dealloc_7_rtmidi_MidiOut, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -10928,49 +11037,52 @@
   0, /*tp_call*/
   0, /*tp_str*/
   0, /*tp_getattro*/
   0, /*tp_setattro*/
   0, /*tp_as_buffer*/
   Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE|Py_TPFLAGS_HAVE_GC, /*tp_flags*/
   "Midi output client interface.\n\n    ``rtmidi.MidiOut(rtapi=API_UNSPECIFIED, name=\"RtMidi Client\")``\n\n    You can specify the low-level MIDI backend API to use via the ``rtapi``\n    keyword or the first positional argument, passing one of the module-level\n    ``API_*`` constants. You can get a list of compiled-in APIs with the\n    module-level ``get_compiled_api`` function. If you pass ``API_UNSPECIFIED``\n    (the default), the first compiled-in API, which has any input ports\n    available, will be used.\n\n    You can optionally pass a name for the MIDI client with the ``name``\n    keyword or the second positional argument. Names with non-ASCII characters\n    in them have to be passed as unicode or UTF-8 encoded strings in Python 2.\n    The default name is ``\"RtMidiOut Client\"``.\n\n    .. note::\n        With some backend APIs (e.g. ALSA), the client name is set by the first\n        ``MidiIn`` *or* ``MidiOut`` created by your program and does not change\n        unless you either use the ``set_client_name`` method, or until *all*\n        ``MidiIn`` and ``MidiOut`` instances are deleted and then a new one is\n        created.\n\n    Exceptions:\n\n    ``SystemError``\n        Raised when the RtMidi backend initialization fails. The execption\n        message should have more information on the cause of the error.\n\n    ``TypeError``\n        Raised when an incompatible value type is passed for a parameter.\n\n    ", /*tp_doc*/
-  __pyx_tp_traverse_6rtmidi_7_rtmidi_MidiBase, /*tp_traverse*/
-  __pyx_tp_clear_6rtmidi_7_rtmidi_MidiBase, /*tp_clear*/
+  __pyx_tp_traverse_7_rtmidi_MidiBase, /*tp_traverse*/
+  __pyx_tp_clear_7_rtmidi_MidiBase, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_6rtmidi_7_rtmidi_MidiOut, /*tp_methods*/
+  __pyx_methods_7_rtmidi_MidiOut, /*tp_methods*/
   0, /*tp_members*/
-  __pyx_getsets_6rtmidi_7_rtmidi_MidiOut, /*tp_getset*/
+  __pyx_getsets_7_rtmidi_MidiOut, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
   0, /*tp_dictoffset*/
   0, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_6rtmidi_7_rtmidi_MidiOut, /*tp_new*/
+  __pyx_tp_new_7_rtmidi_MidiOut, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  0, /*tp_pypy_flags*/
+  #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
 
 #if PY_MAJOR_VERSION >= 3
@@ -11048,15 +11160,15 @@
   {&__pyx_n_u_ERRORTYPE_SYSTEM_ERROR, __pyx_k_ERRORTYPE_SYSTEM_ERROR, sizeof(__pyx_k_ERRORTYPE_SYSTEM_ERROR), 0, 1, 0, 1},
   {&__pyx_n_s_ERRORTYPE_THREAD_ERROR, __pyx_k_ERRORTYPE_THREAD_ERROR, sizeof(__pyx_k_ERRORTYPE_THREAD_ERROR), 0, 0, 1, 1},
   {&__pyx_n_u_ERRORTYPE_THREAD_ERROR, __pyx_k_ERRORTYPE_THREAD_ERROR, sizeof(__pyx_k_ERRORTYPE_THREAD_ERROR), 0, 1, 0, 1},
   {&__pyx_n_s_ERRORTYPE_UNSPECIFIED, __pyx_k_ERRORTYPE_UNSPECIFIED, sizeof(__pyx_k_ERRORTYPE_UNSPECIFIED), 0, 0, 1, 1},
   {&__pyx_n_u_ERRORTYPE_UNSPECIFIED, __pyx_k_ERRORTYPE_UNSPECIFIED, sizeof(__pyx_k_ERRORTYPE_UNSPECIFIED), 0, 1, 0, 1},
   {&__pyx_n_s_ERRORTYPE_WARNING, __pyx_k_ERRORTYPE_WARNING, sizeof(__pyx_k_ERRORTYPE_WARNING), 0, 0, 1, 1},
   {&__pyx_n_u_ERRORTYPE_WARNING, __pyx_k_ERRORTYPE_WARNING, sizeof(__pyx_k_ERRORTYPE_WARNING), 0, 1, 0, 1},
-  {&__pyx_kp_s_Incompatible_checksums_s_vs_0x91, __pyx_k_Incompatible_checksums_s_vs_0x91, sizeof(__pyx_k_Incompatible_checksums_s_vs_0x91), 0, 0, 1, 0},
+  {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_InvalidPortError, __pyx_k_InvalidPortError, sizeof(__pyx_k_InvalidPortError), 0, 0, 1, 1},
   {&__pyx_n_u_InvalidPortError, __pyx_k_InvalidPortError, sizeof(__pyx_k_InvalidPortError), 0, 1, 0, 1},
   {&__pyx_n_s_InvalidUseError, __pyx_k_InvalidUseError, sizeof(__pyx_k_InvalidUseError), 0, 0, 1, 1},
   {&__pyx_n_u_InvalidUseError, __pyx_k_InvalidUseError, sizeof(__pyx_k_InvalidUseError), 0, 1, 0, 1},
   {&__pyx_kp_u_JACK_server_not_running, __pyx_k_JACK_server_not_running, sizeof(__pyx_k_JACK_server_not_running), 0, 1, 0, 0},
   {&__pyx_n_s_MemoryAllocationError, __pyx_k_MemoryAllocationError, sizeof(__pyx_k_MemoryAllocationError), 0, 0, 1, 1},
   {&__pyx_n_u_MemoryAllocationError, __pyx_k_MemoryAllocationError, sizeof(__pyx_k_MemoryAllocationError), 0, 1, 0, 1},
@@ -11130,14 +11242,15 @@
   {&__pyx_n_u_get_compiled_api_by_name, __pyx_k_get_compiled_api_by_name, sizeof(__pyx_k_get_compiled_api_by_name), 0, 1, 0, 1},
   {&__pyx_n_s_get_current_api, __pyx_k_get_current_api, sizeof(__pyx_k_get_current_api), 0, 0, 1, 1},
   {&__pyx_n_s_get_port_count, __pyx_k_get_port_count, sizeof(__pyx_k_get_port_count), 0, 0, 1, 1},
   {&__pyx_n_s_get_port_name, __pyx_k_get_port_name, sizeof(__pyx_k_get_port_name), 0, 0, 1, 1},
   {&__pyx_n_s_get_rtmidi_version, __pyx_k_get_rtmidi_version, sizeof(__pyx_k_get_rtmidi_version), 0, 0, 1, 1},
   {&__pyx_n_u_get_rtmidi_version, __pyx_k_get_rtmidi_version, sizeof(__pyx_k_get_rtmidi_version), 0, 1, 0, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+  {&__pyx_kp_s_home_runner_work_python_rtmidi, __pyx_k_home_runner_work_python_rtmidi, sizeof(__pyx_k_home_runner_work_python_rtmidi), 0, 0, 1, 0},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_u_ignore, __pyx_k_ignore, sizeof(__pyx_k_ignore), 0, 1, 0, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_init, __pyx_k_init, sizeof(__pyx_k_init), 0, 0, 1, 1},
   {&__pyx_n_u_input, __pyx_k_input, sizeof(__pyx_k_input), 0, 1, 0, 1},
   {&__pyx_kp_u_is_invalid, __pyx_k_is_invalid, sizeof(__pyx_k_is_invalid), 0, 1, 0, 0},
   {&__pyx_n_u_latin1, __pyx_k_latin1, sizeof(__pyx_k_latin1), 0, 1, 0, 1},
@@ -11172,21 +11285,20 @@
   {&__pyx_n_s_queue_size_limit, __pyx_k_queue_size_limit, sizeof(__pyx_k_queue_size_limit), 0, 0, 1, 1},
   {&__pyx_kp_u_r_already_opened_s_port_i, __pyx_k_r_already_opened_s_port_i, sizeof(__pyx_k_r_already_opened_s_port_i), 0, 1, 0, 0},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_rtapi, __pyx_k_rtapi, sizeof(__pyx_k_rtapi), 0, 0, 1, 1},
-  {&__pyx_n_s_rtmidi__rtmidi, __pyx_k_rtmidi__rtmidi, sizeof(__pyx_k_rtmidi__rtmidi), 0, 0, 1, 1},
+  {&__pyx_n_s_rtmidi, __pyx_k_rtmidi, sizeof(__pyx_k_rtmidi), 0, 0, 1, 1},
   {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_n_s_set_error_callback, __pyx_k_set_error_callback, sizeof(__pyx_k_set_error_callback), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
-  {&__pyx_kp_s_src__rtmidi_pyx, __pyx_k_src__rtmidi_pyx, sizeof(__pyx_k_src__rtmidi_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_startswith, __pyx_k_startswith, sizeof(__pyx_k_startswith), 0, 0, 1, 1},
   {&__pyx_n_s_string_types, __pyx_k_string_types, sizeof(__pyx_k_string_types), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_super, __pyx_k_super, sizeof(__pyx_k_super), 0, 0, 1, 1},
   {&__pyx_n_s_sys, __pyx_k_sys, sizeof(__pyx_k_sys), 0, 0, 1, 1},
   {&__pyx_n_s_sysex, __pyx_k_sysex, sizeof(__pyx_k_sysex), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
@@ -11198,61 +11310,61 @@
   {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
   {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
   {&__pyx_n_u_win, __pyx_k_win, sizeof(__pyx_k_win), 0, 1, 0, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 282, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 291, __pyx_L1_error)
-  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 300, __pyx_L1_error)
-  __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(0, 309, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 212, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 229, __pyx_L1_error)
-  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 278, __pyx_L1_error)
-  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 642, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 281, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(0, 290, __pyx_L1_error)
+  __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 299, __pyx_L1_error)
+  __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(0, 308, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 211, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 228, __pyx_L1_error)
+  __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_builtin_NotImplementedError = __Pyx_GetBuiltinName(__pyx_n_s_NotImplementedError); if (!__pyx_builtin_NotImplementedError) __PYX_ERR(0, 641, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "src/_rtmidi.pyx":233
+  /* "_rtmidi.pyx":232
  * 
  *     if not isinstance(name, bytes):
  *         raise TypeError("name must be bytes or (unicode) string.")             # <<<<<<<<<<<<<<
  * 
  *     return name
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_name_must_be_bytes_or_unicode_st); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 233, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_name_must_be_bytes_or_unicode_st); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 232, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "src/_rtmidi.pyx":642
+  /* "_rtmidi.pyx":641
  *         """
  *         if self.get_current_api() == API_WINDOWS_MM:
  *             raise NotImplementedError("Virtual ports are not supported "             # <<<<<<<<<<<<<<
  *                                       "by the Windows MultiMedia API.")
  * 
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Virtual_ports_are_not_supported); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 642, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_Virtual_ports_are_not_supported); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 641, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "src/_rtmidi.pyx":686
+  /* "_rtmidi.pyx":685
  *         """
  *         if self.get_current_api() in (API_MACOSX_CORE, API_UNIX_JACK, API_WINDOWS_MM):
  *             raise NotImplementedError(             # <<<<<<<<<<<<<<
  *                 "API backend does not support changing the client name.")
  * 
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_API_backend_does_not_support_cha); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 686, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_API_backend_does_not_support_cha); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 685, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__3);
   __Pyx_GIVEREF(__pyx_tuple__3);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -11267,33 +11379,33 @@
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__6 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__6);
   __Pyx_GIVEREF(__pyx_tuple__6);
 
-  /* "src/_rtmidi.pyx":1100
+  /* "_rtmidi.pyx":1099
  * 
  *         if not message:
  *             raise ValueError("'message' must not be empty.")             # <<<<<<<<<<<<<<
  * 
  *         if len(message) > 3 and message[0] != 0xF0:
  */
-  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_message_must_not_be_empty); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 1100, __pyx_L1_error)
+  __pyx_tuple__8 = PyTuple_Pack(1, __pyx_kp_u_message_must_not_be_empty); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 1099, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "src/_rtmidi.pyx":1103
+  /* "_rtmidi.pyx":1102
  * 
  *         if len(message) > 3 and message[0] != 0xF0:
  *             raise ValueError("'message' longer than 3 bytes but does not "             # <<<<<<<<<<<<<<
  *                              "start with 0xF0.")
  * 
  */
-  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_message_longer_than_3_bytes_but); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 1103, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_message_longer_than_3_bytes_but); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 1102, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
@@ -11307,141 +11419,146 @@
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
   __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__12 = PyTuple_Pack(3, __pyx_int_152509455, __pyx_int_34815411, __pyx_int_2218169); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
-  /* "src/_rtmidi.pyx":115
+  /* "_rtmidi.pyx":115
  * 
  * __all__ = (
  *     'API_UNSPECIFIED', 'API_MACOSX_CORE', 'API_LINUX_ALSA', 'API_UNIX_JACK',             # <<<<<<<<<<<<<<
  *     'API_WINDOWS_MM', 'API_RTMIDI_DUMMY', 'ERRORTYPE_DEBUG_WARNING',
  *     'ERRORTYPE_DRIVER_ERROR', 'ERRORTYPE_INVALID_DEVICE',
  */
-  __pyx_tuple__12 = PyTuple_Pack(31, __pyx_n_u_API_UNSPECIFIED, __pyx_n_u_API_MACOSX_CORE, __pyx_n_u_API_LINUX_ALSA, __pyx_n_u_API_UNIX_JACK, __pyx_n_u_API_WINDOWS_MM, __pyx_n_u_API_RTMIDI_DUMMY, __pyx_n_u_ERRORTYPE_DEBUG_WARNING, __pyx_n_u_ERRORTYPE_DRIVER_ERROR, __pyx_n_u_ERRORTYPE_INVALID_DEVICE, __pyx_n_u_ERRORTYPE_INVALID_PARAMETER, __pyx_n_u_ERRORTYPE_INVALID_USE, __pyx_n_u_ERRORTYPE_MEMORY_ERROR, __pyx_n_u_ERRORTYPE_NO_DEVICES_FOUND, __pyx_n_u_ERRORTYPE_SYSTEM_ERROR, __pyx_n_u_ERRORTYPE_THREAD_ERROR, __pyx_n_u_ERRORTYPE_UNSPECIFIED, __pyx_n_u_ERRORTYPE_WARNING, __pyx_n_u_InvalidPortError, __pyx_n_u_InvalidUseError, __pyx_n_u_MemoryAllocationError, __pyx_n_u_MidiIn, __pyx_n_u_MidiOut, __pyx_n_u_NoDevicesError, __pyx_n_u_RtMidiError, __pyx_n_u_SystemError, __pyx_n_u_UnsupportedOperationError, __pyx_n_u_get_api_display_name, __pyx_n_u_get_api_name, __pyx_n_u_get_compiled_api, __pyx_n_u_get_compiled_api_by_name, __pyx_n_u_get_rtmidi_version); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 115, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__13 = PyTuple_Pack(31, __pyx_n_u_API_UNSPECIFIED, __pyx_n_u_API_MACOSX_CORE, __pyx_n_u_API_LINUX_ALSA, __pyx_n_u_API_UNIX_JACK, __pyx_n_u_API_WINDOWS_MM, __pyx_n_u_API_RTMIDI_DUMMY, __pyx_n_u_ERRORTYPE_DEBUG_WARNING, __pyx_n_u_ERRORTYPE_DRIVER_ERROR, __pyx_n_u_ERRORTYPE_INVALID_DEVICE, __pyx_n_u_ERRORTYPE_INVALID_PARAMETER, __pyx_n_u_ERRORTYPE_INVALID_USE, __pyx_n_u_ERRORTYPE_MEMORY_ERROR, __pyx_n_u_ERRORTYPE_NO_DEVICES_FOUND, __pyx_n_u_ERRORTYPE_SYSTEM_ERROR, __pyx_n_u_ERRORTYPE_THREAD_ERROR, __pyx_n_u_ERRORTYPE_UNSPECIFIED, __pyx_n_u_ERRORTYPE_WARNING, __pyx_n_u_InvalidPortError, __pyx_n_u_InvalidUseError, __pyx_n_u_MemoryAllocationError, __pyx_n_u_MidiIn, __pyx_n_u_MidiOut, __pyx_n_u_NoDevicesError, __pyx_n_u_RtMidiError, __pyx_n_u_SystemError, __pyx_n_u_UnsupportedOperationError, __pyx_n_u_get_api_display_name, __pyx_n_u_get_api_name, __pyx_n_u_get_compiled_api, __pyx_n_u_get_compiled_api_by_name, __pyx_n_u_get_rtmidi_version); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 115, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
-  /* "src/_rtmidi.pyx":223
+  /* "_rtmidi.pyx":222
  * 
  * 
  * def _to_bytes(name):             # <<<<<<<<<<<<<<
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_n_s_name); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 223, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__rtmidi_pyx, __pyx_n_s_to_bytes, 223, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_n_s_name); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(0, 222, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_to_bytes, 222, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(0, 222, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":277
+  /* "_rtmidi.pyx":276
  *     type = ERR_UNSPECIFIED
  * 
  *     def __init__(self, msg, type=None):             # <<<<<<<<<<<<<<
  *         super().__init__(msg)
  *         self.type = self.type if type is None else type
  */
-  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_type); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 277, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__rtmidi_pyx, __pyx_n_s_init, 277, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 277, __pyx_L1_error)
-  __pyx_tuple__17 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 277, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__16 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_msg, __pyx_n_s_type); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_init, 276, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __pyx_tuple__18 = PyTuple_Pack(1, ((PyObject *)Py_None)); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 276, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
-  /* "src/_rtmidi.pyx":338
+  /* "_rtmidi.pyx":337
  * # wrappers for RtMidi's static methods and classes
  * 
  * def get_api_display_name(api):             # <<<<<<<<<<<<<<
  *     """Return the display name of a specified MIDI API.
  * 
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_n_s_api); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 338, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__rtmidi_pyx, __pyx_n_s_get_api_display_name, 338, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_n_s_api); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 337, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_api_display_name, 337, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 337, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":354
+  /* "_rtmidi.pyx":353
  * 
  * 
  * def get_api_name(api):             # <<<<<<<<<<<<<<
  *     """Return the name of a specified MIDI API.
  * 
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_n_s_api); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 354, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__rtmidi_pyx, __pyx_n_s_get_api_name, 354, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_n_s_api); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 353, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_api_name, 353, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 353, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":370
+  /* "_rtmidi.pyx":369
  * 
  * 
  * def get_compiled_api():             # <<<<<<<<<<<<<<
  *     """Return a list of low-level MIDI backend APIs this module supports.
  * 
  */
-  __pyx_tuple__22 = PyTuple_Pack(2, __pyx_n_s_api_v, __pyx_n_s_i); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 370, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__rtmidi_pyx, __pyx_n_s_get_compiled_api, 370, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(2, __pyx_n_s_api_v, __pyx_n_s_i); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 369, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_compiled_api, 369, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 369, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":386
+  /* "_rtmidi.pyx":385
  * 
  * 
  * def get_compiled_api_by_name(name):             # <<<<<<<<<<<<<<
  *     """Return the compiled MIDI API having the given name.
  * 
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_n_s_name); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 386, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__rtmidi_pyx, __pyx_n_s_get_compiled_api_by_name, 386, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_n_s_name); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 385, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_compiled_api_by_name, 385, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 385, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":397
+  /* "_rtmidi.pyx":396
  * 
  * 
  * def get_rtmidi_version():             # <<<<<<<<<<<<<<
  *     """Return the version string of the wrapped RtMidi library."""
  *     return RtMidi_getVersion().decode('utf-8')
  */
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__rtmidi_pyx, __pyx_n_s_get_rtmidi_version, 397, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_get_rtmidi_version, 396, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 396, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":402
+  /* "_rtmidi.pyx":401
  * 
  * 
  * def _default_error_handler(etype, msg, data=None):             # <<<<<<<<<<<<<<
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  */
-  __pyx_tuple__27 = PyTuple_Pack(3, __pyx_n_s_etype, __pyx_n_s_msg, __pyx_n_s_data); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 402, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
-  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_src__rtmidi_pyx, __pyx_n_s_default_error_handler, 402, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(3, __pyx_n_s_etype, __pyx_n_s_msg, __pyx_n_s_data); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_home_runner_work_python_rtmidi, __pyx_n_s_default_error_handler, 401, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 401, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_MidiBase(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__29 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__29);
-  __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MidiBase, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__30 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_MidiBase, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_240 = PyInt_FromLong(240); if (unlikely(!__pyx_int_240)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_2218169 = PyInt_FromLong(2218169L); if (unlikely(!__pyx_int_2218169)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_34815411 = PyInt_FromLong(34815411L); if (unlikely(!__pyx_int_34815411)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_152509455 = PyInt_FromLong(152509455L); if (unlikely(!__pyx_int_152509455)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
@@ -11480,57 +11597,57 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  __pyx_vtabptr_6rtmidi_7_rtmidi_MidiBase = &__pyx_vtable_6rtmidi_7_rtmidi_MidiBase;
-  __pyx_vtable_6rtmidi_7_rtmidi_MidiBase.baseptr = (RtMidi *(*)(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *))__pyx_f_6rtmidi_7_rtmidi_8MidiBase_baseptr;
-  if (PyType_Ready(&__pyx_type_6rtmidi_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_vtabptr_7_rtmidi_MidiBase = &__pyx_vtable_7_rtmidi_MidiBase;
+  __pyx_vtable_7_rtmidi_MidiBase.baseptr = (RtMidi *(*)(struct __pyx_obj_7_rtmidi_MidiBase *))__pyx_f_7_rtmidi_8MidiBase_baseptr;
+  if (PyType_Ready(&__pyx_type_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_6rtmidi_7_rtmidi_MidiBase.tp_print = 0;
+  __pyx_type_7_rtmidi_MidiBase.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6rtmidi_7_rtmidi_MidiBase.tp_dictoffset && __pyx_type_6rtmidi_7_rtmidi_MidiBase.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_6rtmidi_7_rtmidi_MidiBase.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7_rtmidi_MidiBase.tp_dictoffset && __pyx_type_7_rtmidi_MidiBase.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_7_rtmidi_MidiBase.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6rtmidi_7_rtmidi_MidiBase.tp_dict, __pyx_vtabptr_6rtmidi_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiBase, (PyObject *)&__pyx_type_6rtmidi_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6rtmidi_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
-  __pyx_ptype_6rtmidi_7_rtmidi_MidiBase = &__pyx_type_6rtmidi_7_rtmidi_MidiBase;
-  __pyx_vtabptr_6rtmidi_7_rtmidi_MidiIn = &__pyx_vtable_6rtmidi_7_rtmidi_MidiIn;
-  __pyx_vtable_6rtmidi_7_rtmidi_MidiIn.__pyx_base = *__pyx_vtabptr_6rtmidi_7_rtmidi_MidiBase;
-  __pyx_vtable_6rtmidi_7_rtmidi_MidiIn.__pyx_base.baseptr = (RtMidi *(*)(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *))__pyx_f_6rtmidi_7_rtmidi_6MidiIn_baseptr;
-  __pyx_type_6rtmidi_7_rtmidi_MidiIn.tp_base = __pyx_ptype_6rtmidi_7_rtmidi_MidiBase;
-  if (PyType_Ready(&__pyx_type_6rtmidi_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 757, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7_rtmidi_MidiBase.tp_dict, __pyx_vtabptr_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiBase, (PyObject *)&__pyx_type_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7_rtmidi_MidiBase) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_ptype_7_rtmidi_MidiBase = &__pyx_type_7_rtmidi_MidiBase;
+  __pyx_vtabptr_7_rtmidi_MidiIn = &__pyx_vtable_7_rtmidi_MidiIn;
+  __pyx_vtable_7_rtmidi_MidiIn.__pyx_base = *__pyx_vtabptr_7_rtmidi_MidiBase;
+  __pyx_vtable_7_rtmidi_MidiIn.__pyx_base.baseptr = (RtMidi *(*)(struct __pyx_obj_7_rtmidi_MidiBase *))__pyx_f_7_rtmidi_6MidiIn_baseptr;
+  __pyx_type_7_rtmidi_MidiIn.tp_base = __pyx_ptype_7_rtmidi_MidiBase;
+  if (PyType_Ready(&__pyx_type_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_6rtmidi_7_rtmidi_MidiIn.tp_print = 0;
+  __pyx_type_7_rtmidi_MidiIn.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6rtmidi_7_rtmidi_MidiIn.tp_dictoffset && __pyx_type_6rtmidi_7_rtmidi_MidiIn.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_6rtmidi_7_rtmidi_MidiIn.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7_rtmidi_MidiIn.tp_dictoffset && __pyx_type_7_rtmidi_MidiIn.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_7_rtmidi_MidiIn.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6rtmidi_7_rtmidi_MidiIn.tp_dict, __pyx_vtabptr_6rtmidi_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 757, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiIn, (PyObject *)&__pyx_type_6rtmidi_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 757, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6rtmidi_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 757, __pyx_L1_error)
-  __pyx_ptype_6rtmidi_7_rtmidi_MidiIn = &__pyx_type_6rtmidi_7_rtmidi_MidiIn;
-  __pyx_vtabptr_6rtmidi_7_rtmidi_MidiOut = &__pyx_vtable_6rtmidi_7_rtmidi_MidiOut;
-  __pyx_vtable_6rtmidi_7_rtmidi_MidiOut.__pyx_base = *__pyx_vtabptr_6rtmidi_7_rtmidi_MidiBase;
-  __pyx_vtable_6rtmidi_7_rtmidi_MidiOut.__pyx_base.baseptr = (RtMidi *(*)(struct __pyx_obj_6rtmidi_7_rtmidi_MidiBase *))__pyx_f_6rtmidi_7_rtmidi_7MidiOut_baseptr;
-  __pyx_type_6rtmidi_7_rtmidi_MidiOut.tp_base = __pyx_ptype_6rtmidi_7_rtmidi_MidiBase;
-  if (PyType_Ready(&__pyx_type_6rtmidi_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_type_7_rtmidi_MidiIn.tp_dict, __pyx_vtabptr_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiIn, (PyObject *)&__pyx_type_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7_rtmidi_MidiIn) < 0) __PYX_ERR(0, 756, __pyx_L1_error)
+  __pyx_ptype_7_rtmidi_MidiIn = &__pyx_type_7_rtmidi_MidiIn;
+  __pyx_vtabptr_7_rtmidi_MidiOut = &__pyx_vtable_7_rtmidi_MidiOut;
+  __pyx_vtable_7_rtmidi_MidiOut.__pyx_base = *__pyx_vtabptr_7_rtmidi_MidiBase;
+  __pyx_vtable_7_rtmidi_MidiOut.__pyx_base.baseptr = (RtMidi *(*)(struct __pyx_obj_7_rtmidi_MidiBase *))__pyx_f_7_rtmidi_7MidiOut_baseptr;
+  __pyx_type_7_rtmidi_MidiOut.tp_base = __pyx_ptype_7_rtmidi_MidiBase;
+  if (PyType_Ready(&__pyx_type_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 968, __pyx_L1_error)
   #if PY_VERSION_HEX < 0x030800B1
-  __pyx_type_6rtmidi_7_rtmidi_MidiOut.tp_print = 0;
+  __pyx_type_7_rtmidi_MidiOut.tp_print = 0;
   #endif
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_6rtmidi_7_rtmidi_MidiOut.tp_dictoffset && __pyx_type_6rtmidi_7_rtmidi_MidiOut.tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_type_6rtmidi_7_rtmidi_MidiOut.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7_rtmidi_MidiOut.tp_dictoffset && __pyx_type_7_rtmidi_MidiOut.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_7_rtmidi_MidiOut.tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
-  if (__Pyx_SetVtable(__pyx_type_6rtmidi_7_rtmidi_MidiOut.tp_dict, __pyx_vtabptr_6rtmidi_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiOut, (PyObject *)&__pyx_type_6rtmidi_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
-  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_6rtmidi_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 969, __pyx_L1_error)
-  __pyx_ptype_6rtmidi_7_rtmidi_MidiOut = &__pyx_type_6rtmidi_7_rtmidi_MidiOut;
+  if (__Pyx_SetVtable(__pyx_type_7_rtmidi_MidiOut.tp_dict, __pyx_vtabptr_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 968, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_MidiOut, (PyObject *)&__pyx_type_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 968, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7_rtmidi_MidiOut) < 0) __PYX_ERR(0, 968, __pyx_L1_error)
+  __pyx_ptype_7_rtmidi_MidiOut = &__pyx_type_7_rtmidi_MidiOut;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -11705,19 +11822,17 @@
   if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
   if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
-  #ifdef WITH_THREAD /* Python build with threading support? */
+  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
   PyEval_InitThreads();
   #endif
-  #endif
   /*--- Module creation code ---*/
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   __pyx_m = __pyx_pyinit_module;
   Py_INCREF(__pyx_m);
   #else
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_rtmidi", __pyx_methods, __pyx_k_A_Python_binding_for_the_RtMidi, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
@@ -11728,28 +11843,28 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_rtmidi___rtmidi) {
+  if (__pyx_module_is_main__rtmidi) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "rtmidi._rtmidi")) {
-      if (unlikely(PyDict_SetItemString(modules, "rtmidi._rtmidi", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "_rtmidi")) {
+      if (unlikely(PyDict_SetItemString(modules, "_rtmidi", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -11762,59 +11877,59 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "src/_rtmidi.pyx":106
+  /* "_rtmidi.pyx":106
  * """
  * 
  * import sys             # <<<<<<<<<<<<<<
  * import warnings
  * 
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_sys, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_sys, __pyx_t_1) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":107
+  /* "_rtmidi.pyx":107
  * 
  * import sys
  * import warnings             # <<<<<<<<<<<<<<
  * 
  * from libcpp cimport bool
  */
   __pyx_t_1 = __Pyx_Import(__pyx_n_s_warnings, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_1) < 0) __PYX_ERR(0, 107, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":115
+  /* "_rtmidi.pyx":115
  * 
  * __all__ = (
  *     'API_UNSPECIFIED', 'API_MACOSX_CORE', 'API_LINUX_ALSA', 'API_UNIX_JACK',             # <<<<<<<<<<<<<<
  *     'API_WINDOWS_MM', 'API_RTMIDI_DUMMY', 'ERRORTYPE_DEBUG_WARNING',
  *     'ERRORTYPE_DRIVER_ERROR', 'ERRORTYPE_INVALID_DEVICE',
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_tuple__12) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_all, __pyx_tuple__13) < 0) __PYX_ERR(0, 114, __pyx_L1_error)
 
-  /* "src/_rtmidi.pyx":128
+  /* "_rtmidi.pyx":128
  * )
  * 
  * if bytes is str:             # <<<<<<<<<<<<<<
  *     string_types = (str, unicode)
  * else:
  */
   __pyx_t_2 = ((&PyBytes_Type) == (&PyUnicode_Type));
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
-    /* "src/_rtmidi.pyx":129
+    /* "_rtmidi.pyx":129
  * 
  * if bytes is str:
  *     string_types = (str, unicode)             # <<<<<<<<<<<<<<
  * else:
  *     string_types = (str,)
  */
     __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
@@ -11824,708 +11939,708 @@
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&PyUnicode_Type)));
     __Pyx_INCREF(((PyObject *)(&PyUnicode_Type)));
     __Pyx_GIVEREF(((PyObject *)(&PyUnicode_Type)));
     PyTuple_SET_ITEM(__pyx_t_1, 1, ((PyObject *)(&PyUnicode_Type)));
     if (PyDict_SetItem(__pyx_d, __pyx_n_s_string_types, __pyx_t_1) < 0) __PYX_ERR(0, 129, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "src/_rtmidi.pyx":128
+    /* "_rtmidi.pyx":128
  * )
  * 
  * if bytes is str:             # <<<<<<<<<<<<<<
  *     string_types = (str, unicode)
  * else:
  */
     goto __pyx_L2;
   }
 
-  /* "src/_rtmidi.pyx":131
+  /* "_rtmidi.pyx":131
  *     string_types = (str, unicode)
  * else:
  *     string_types = (str,)             # <<<<<<<<<<<<<<
  * 
- * 
+ * cdef extern from "Python.h":
  */
   /*else*/ {
     __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(((PyObject *)(&PyUnicode_Type)));
     __Pyx_GIVEREF(((PyObject *)(&PyUnicode_Type)));
     PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&PyUnicode_Type)));
     if (PyDict_SetItem(__pyx_d, __pyx_n_s_string_types, __pyx_t_1) < 0) __PYX_ERR(0, 131, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L2:;
 
-  /* "src/_rtmidi.pyx":137
- *     void py_init()
+  /* "_rtmidi.pyx":136
+ *     void Py_Initialize()
  * 
- * py_init()             # <<<<<<<<<<<<<<
+ * Py_Initialize()             # <<<<<<<<<<<<<<
  * 
  * # Declarations for RtMidi C++ classes and their methods we use
  */
-  py_init();
+  Py_Initialize();
 
-  /* "src/_rtmidi.pyx":223
+  /* "_rtmidi.pyx":222
  * 
  * 
  * def _to_bytes(name):             # <<<<<<<<<<<<<<
  *     """Convert a unicode (Python 2) or str (Python 3) object into bytes."""
  *     # 'bytes' == 'str' in Python 2 but a separate type in Python 3
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6rtmidi_7_rtmidi_1_to_bytes, NULL, __pyx_n_s_rtmidi__rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_1_to_bytes, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_bytes, __pyx_t_1) < 0) __PYX_ERR(0, 223, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_to_bytes, __pyx_t_1) < 0) __PYX_ERR(0, 222, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":242
+  /* "_rtmidi.pyx":241
  * # export Api enum values to Python
  * 
  * API_UNSPECIFIED = UNSPECIFIED             # <<<<<<<<<<<<<<
  * API_MACOSX_CORE = MACOSX_CORE
  * API_LINUX_ALSA = LINUX_ALSA
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::UNSPECIFIED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::UNSPECIFIED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_UNSPECIFIED, __pyx_t_1) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_UNSPECIFIED, __pyx_t_1) < 0) __PYX_ERR(0, 241, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":243
+  /* "_rtmidi.pyx":242
  * 
  * API_UNSPECIFIED = UNSPECIFIED
  * API_MACOSX_CORE = MACOSX_CORE             # <<<<<<<<<<<<<<
  * API_LINUX_ALSA = LINUX_ALSA
  * API_UNIX_JACK = UNIX_JACK
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::MACOSX_CORE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::MACOSX_CORE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_MACOSX_CORE, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_MACOSX_CORE, __pyx_t_1) < 0) __PYX_ERR(0, 242, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":244
+  /* "_rtmidi.pyx":243
  * API_UNSPECIFIED = UNSPECIFIED
  * API_MACOSX_CORE = MACOSX_CORE
  * API_LINUX_ALSA = LINUX_ALSA             # <<<<<<<<<<<<<<
  * API_UNIX_JACK = UNIX_JACK
  * API_WINDOWS_MM = WINDOWS_MM
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::LINUX_ALSA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::LINUX_ALSA); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_LINUX_ALSA, __pyx_t_1) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_LINUX_ALSA, __pyx_t_1) < 0) __PYX_ERR(0, 243, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":245
+  /* "_rtmidi.pyx":244
  * API_MACOSX_CORE = MACOSX_CORE
  * API_LINUX_ALSA = LINUX_ALSA
  * API_UNIX_JACK = UNIX_JACK             # <<<<<<<<<<<<<<
  * API_WINDOWS_MM = WINDOWS_MM
  * API_RTMIDI_DUMMY = RTMIDI_DUMMY
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::UNIX_JACK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::UNIX_JACK); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_UNIX_JACK, __pyx_t_1) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_UNIX_JACK, __pyx_t_1) < 0) __PYX_ERR(0, 244, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":246
+  /* "_rtmidi.pyx":245
  * API_LINUX_ALSA = LINUX_ALSA
  * API_UNIX_JACK = UNIX_JACK
  * API_WINDOWS_MM = WINDOWS_MM             # <<<<<<<<<<<<<<
  * API_RTMIDI_DUMMY = RTMIDI_DUMMY
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::WINDOWS_MM); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::WINDOWS_MM); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_WINDOWS_MM, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_WINDOWS_MM, __pyx_t_1) < 0) __PYX_ERR(0, 245, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":247
+  /* "_rtmidi.pyx":246
  * API_UNIX_JACK = UNIX_JACK
  * API_WINDOWS_MM = WINDOWS_MM
  * API_RTMIDI_DUMMY = RTMIDI_DUMMY             # <<<<<<<<<<<<<<
  * 
  * # export error values to Python
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::RTMIDI_DUMMY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 247, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidi_3a__3a_Api(RtMidi::RTMIDI_DUMMY); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_RTMIDI_DUMMY, __pyx_t_1) < 0) __PYX_ERR(0, 247, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_API_RTMIDI_DUMMY, __pyx_t_1) < 0) __PYX_ERR(0, 246, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":251
+  /* "_rtmidi.pyx":250
  * # export error values to Python
  * 
  * ERRORTYPE_WARNING = ERR_WARNING             # <<<<<<<<<<<<<<
  * ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING
  * ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::WARNING); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::WARNING); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_WARNING, __pyx_t_1) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_WARNING, __pyx_t_1) < 0) __PYX_ERR(0, 250, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":252
+  /* "_rtmidi.pyx":251
  * 
  * ERRORTYPE_WARNING = ERR_WARNING
  * ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING             # <<<<<<<<<<<<<<
  * ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED
  * ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DEBUG_WARNING); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DEBUG_WARNING); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_DEBUG_WARNING, __pyx_t_1) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_DEBUG_WARNING, __pyx_t_1) < 0) __PYX_ERR(0, 251, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":253
+  /* "_rtmidi.pyx":252
  * ERRORTYPE_WARNING = ERR_WARNING
  * ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING
  * ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED             # <<<<<<<<<<<<<<
  * ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND
  * ERRORTYPE_INVALID_DEVICE = ERR_INVALID_DEVICE
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::UNSPECIFIED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::UNSPECIFIED); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_UNSPECIFIED, __pyx_t_1) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_UNSPECIFIED, __pyx_t_1) < 0) __PYX_ERR(0, 252, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":254
+  /* "_rtmidi.pyx":253
  * ERRORTYPE_DEBUG_WARNING = ERR_DEBUG_WARNING
  * ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED
  * ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND             # <<<<<<<<<<<<<<
  * ERRORTYPE_INVALID_DEVICE = ERR_INVALID_DEVICE
  * ERRORTYPE_MEMORY_ERROR = ERR_MEMORY_ERROR
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::NO_DEVICES_FOUND); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::NO_DEVICES_FOUND); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_NO_DEVICES_FOUND, __pyx_t_1) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_NO_DEVICES_FOUND, __pyx_t_1) < 0) __PYX_ERR(0, 253, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":255
+  /* "_rtmidi.pyx":254
  * ERRORTYPE_UNSPECIFIED = ERR_UNSPECIFIED
  * ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND
  * ERRORTYPE_INVALID_DEVICE = ERR_INVALID_DEVICE             # <<<<<<<<<<<<<<
  * ERRORTYPE_MEMORY_ERROR = ERR_MEMORY_ERROR
  * ERRORTYPE_INVALID_PARAMETER = ERR_INVALID_PARAMETER
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_DEVICE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_DEVICE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_DEVICE, __pyx_t_1) < 0) __PYX_ERR(0, 255, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_DEVICE, __pyx_t_1) < 0) __PYX_ERR(0, 254, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":256
+  /* "_rtmidi.pyx":255
  * ERRORTYPE_NO_DEVICES_FOUND = ERR_NO_DEVICES_FOUND
  * ERRORTYPE_INVALID_DEVICE = ERR_INVALID_DEVICE
  * ERRORTYPE_MEMORY_ERROR = ERR_MEMORY_ERROR             # <<<<<<<<<<<<<<
  * ERRORTYPE_INVALID_PARAMETER = ERR_INVALID_PARAMETER
  * ERRORTYPE_INVALID_USE = ERR_INVALID_USE
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_MEMORY_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 256, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_MEMORY_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 255, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":257
+  /* "_rtmidi.pyx":256
  * ERRORTYPE_INVALID_DEVICE = ERR_INVALID_DEVICE
  * ERRORTYPE_MEMORY_ERROR = ERR_MEMORY_ERROR
  * ERRORTYPE_INVALID_PARAMETER = ERR_INVALID_PARAMETER             # <<<<<<<<<<<<<<
  * ERRORTYPE_INVALID_USE = ERR_INVALID_USE
  * ERRORTYPE_DRIVER_ERROR = ERR_DRIVER_ERROR
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_PARAMETER, __pyx_t_1) < 0) __PYX_ERR(0, 257, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_PARAMETER, __pyx_t_1) < 0) __PYX_ERR(0, 256, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":258
+  /* "_rtmidi.pyx":257
  * ERRORTYPE_MEMORY_ERROR = ERR_MEMORY_ERROR
  * ERRORTYPE_INVALID_PARAMETER = ERR_INVALID_PARAMETER
  * ERRORTYPE_INVALID_USE = ERR_INVALID_USE             # <<<<<<<<<<<<<<
  * ERRORTYPE_DRIVER_ERROR = ERR_DRIVER_ERROR
  * ERRORTYPE_SYSTEM_ERROR = ERR_SYSTEM_ERROR
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_USE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_USE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_USE, __pyx_t_1) < 0) __PYX_ERR(0, 258, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_INVALID_USE, __pyx_t_1) < 0) __PYX_ERR(0, 257, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":259
+  /* "_rtmidi.pyx":258
  * ERRORTYPE_INVALID_PARAMETER = ERR_INVALID_PARAMETER
  * ERRORTYPE_INVALID_USE = ERR_INVALID_USE
  * ERRORTYPE_DRIVER_ERROR = ERR_DRIVER_ERROR             # <<<<<<<<<<<<<<
  * ERRORTYPE_SYSTEM_ERROR = ERR_SYSTEM_ERROR
  * ERRORTYPE_THREAD_ERROR = ERR_THREAD_ERROR
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::DRIVER_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_DRIVER_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_DRIVER_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 258, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":260
+  /* "_rtmidi.pyx":259
  * ERRORTYPE_INVALID_USE = ERR_INVALID_USE
  * ERRORTYPE_DRIVER_ERROR = ERR_DRIVER_ERROR
  * ERRORTYPE_SYSTEM_ERROR = ERR_SYSTEM_ERROR             # <<<<<<<<<<<<<<
  * ERRORTYPE_THREAD_ERROR = ERR_THREAD_ERROR
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::SYSTEM_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::SYSTEM_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_SYSTEM_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 260, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_SYSTEM_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 259, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":261
+  /* "_rtmidi.pyx":260
  * ERRORTYPE_DRIVER_ERROR = ERR_DRIVER_ERROR
  * ERRORTYPE_SYSTEM_ERROR = ERR_SYSTEM_ERROR
  * ERRORTYPE_THREAD_ERROR = ERR_THREAD_ERROR             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::THREAD_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 261, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::THREAD_ERROR); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_THREAD_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 261, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ERRORTYPE_THREAD_ERROR, __pyx_t_1) < 0) __PYX_ERR(0, 260, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":266
+  /* "_rtmidi.pyx":265
  * # custom exceptions
  * 
  * class RtMidiError(Exception):             # <<<<<<<<<<<<<<
  *     """Base general RtMidi exception.
  * 
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   __Pyx_GIVEREF(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
   PyTuple_SET_ITEM(__pyx_t_1, 0, ((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_RtMidiError, __pyx_n_s_RtMidiError, (PyObject *) NULL, __pyx_n_s_rtmidi__rtmidi, __pyx_kp_s_Base_general_RtMidi_exception_Al); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_RtMidiError, __pyx_n_s_RtMidiError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Base_general_RtMidi_exception_Al); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_6 = PyList_New(0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
 
-  /* "src/_rtmidi.pyx":275
+  /* "_rtmidi.pyx":274
  * 
  *     """
  *     type = ERR_UNSPECIFIED             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, msg, type=None):
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::UNSPECIFIED); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 275, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::UNSPECIFIED); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 275, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "src/_rtmidi.pyx":277
+  /* "_rtmidi.pyx":276
  *     type = ERR_UNSPECIFIED
  * 
  *     def __init__(self, msg, type=None):             # <<<<<<<<<<<<<<
  *         super().__init__(msg)
  *         self.type = self.type if type is None else type
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_6rtmidi_7_rtmidi_11RtMidiError_1__init__, 0, __pyx_n_s_RtMidiError___init, NULL, __pyx_n_s_rtmidi__rtmidi, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_7_rtmidi_11RtMidiError_1__init__, 0, __pyx_n_s_RtMidiError___init, NULL, __pyx_n_s_rtmidi, __pyx_d, ((PyObject *)__pyx_codeobj__17)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_INCREF(__pyx_t_7);
   PyList_Append(__pyx_t_6, __pyx_t_7);
   __Pyx_GIVEREF(__pyx_t_7);
-  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__17);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_init, __pyx_t_7) < 0) __PYX_ERR(0, 277, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__18);
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_init, __pyx_t_7) < 0) __PYX_ERR(0, 276, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "src/_rtmidi.pyx":266
+  /* "_rtmidi.pyx":265
  * # custom exceptions
  * 
  * class RtMidiError(Exception):             # <<<<<<<<<<<<<<
  *     """Base general RtMidi exception.
  * 
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_RtMidiError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 266, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_RtMidiError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_CyFunction_InitClassCell(__pyx_t_6, __pyx_t_7) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+  if (__Pyx_CyFunction_InitClassCell(__pyx_t_6, __pyx_t_7) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RtMidiError, __pyx_t_7) < 0) __PYX_ERR(0, 266, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_RtMidiError, __pyx_t_7) < 0) __PYX_ERR(0, 265, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":282
+  /* "_rtmidi.pyx":281
  * 
  * 
  * class InvalidPortError(RtMidiError, ValueError):             # <<<<<<<<<<<<<<
  *     """Raised when an invalid port number is used.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_builtin_ValueError);
   __Pyx_GIVEREF(__pyx_builtin_ValueError);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_builtin_ValueError);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_InvalidPortError, __pyx_n_s_InvalidPortError, (PyObject *) NULL, __pyx_n_s_rtmidi__rtmidi, __pyx_kp_s_Raised_when_an_invalid_port_numb); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_InvalidPortError, __pyx_n_s_InvalidPortError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_when_an_invalid_port_numb); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "src/_rtmidi.pyx":288
+  /* "_rtmidi.pyx":287
  * 
  *     """
  *     type = ERR_INVALID_PARAMETER             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 288, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_PARAMETER); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 288, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 287, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "src/_rtmidi.pyx":282
+  /* "_rtmidi.pyx":281
  * 
  * 
  * class InvalidPortError(RtMidiError, ValueError):             # <<<<<<<<<<<<<<
  *     """Raised when an invalid port number is used.
  * 
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_InvalidPortError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 282, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_InvalidPortError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InvalidPortError, __pyx_t_7) < 0) __PYX_ERR(0, 282, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InvalidPortError, __pyx_t_7) < 0) __PYX_ERR(0, 281, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "src/_rtmidi.pyx":291
+  /* "_rtmidi.pyx":290
  * 
  * 
  * class InvalidUseError(RtMidiError, RuntimeError):             # <<<<<<<<<<<<<<
  *     """Raised when an method call is not allowed in the current state.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __Pyx_INCREF(__pyx_builtin_RuntimeError);
   __Pyx_GIVEREF(__pyx_builtin_RuntimeError);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_builtin_RuntimeError);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_InvalidUseError, __pyx_n_s_InvalidUseError, (PyObject *) NULL, __pyx_n_s_rtmidi__rtmidi, __pyx_kp_s_Raised_when_an_method_call_is_no); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_InvalidUseError, __pyx_n_s_InvalidUseError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_when_an_method_call_is_no); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "src/_rtmidi.pyx":297
+  /* "_rtmidi.pyx":296
  * 
  *     """
  *     type = ERR_INVALID_USE             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_USE); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 297, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::INVALID_USE); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 297, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 296, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "src/_rtmidi.pyx":291
+  /* "_rtmidi.pyx":290
  * 
  * 
  * class InvalidUseError(RtMidiError, RuntimeError):             # <<<<<<<<<<<<<<
  *     """Raised when an method call is not allowed in the current state.
  * 
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_InvalidUseError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 291, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_InvalidUseError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InvalidUseError, __pyx_t_7) < 0) __PYX_ERR(0, 291, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InvalidUseError, __pyx_t_7) < 0) __PYX_ERR(0, 290, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":300
+  /* "_rtmidi.pyx":299
  * 
  * 
  * class MemoryAllocationError(RtMidiError, MemoryError):             # <<<<<<<<<<<<<<
  *     """Raised if a memory allocation failed on the C++ level.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __Pyx_INCREF(__pyx_builtin_MemoryError);
   __Pyx_GIVEREF(__pyx_builtin_MemoryError);
   PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_builtin_MemoryError);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_MemoryAllocationError, __pyx_n_s_MemoryAllocationError, (PyObject *) NULL, __pyx_n_s_rtmidi__rtmidi, __pyx_kp_s_Raised_if_a_memory_allocation_fa); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_MemoryAllocationError, __pyx_n_s_MemoryAllocationError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_a_memory_allocation_fa); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "src/_rtmidi.pyx":306
+  /* "_rtmidi.pyx":305
  * 
  *     """
  *     type = ERR_MEMORY_ERROR             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 306, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::MEMORY_ERROR); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 305, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 306, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 305, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "src/_rtmidi.pyx":300
+  /* "_rtmidi.pyx":299
  * 
  * 
  * class MemoryAllocationError(RtMidiError, MemoryError):             # <<<<<<<<<<<<<<
  *     """Raised if a memory allocation failed on the C++ level.
  * 
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_MemoryAllocationError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 300, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_MemoryAllocationError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MemoryAllocationError, __pyx_t_7) < 0) __PYX_ERR(0, 300, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_MemoryAllocationError, __pyx_t_7) < 0) __PYX_ERR(0, 299, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "src/_rtmidi.pyx":309
+  /* "_rtmidi.pyx":308
  * 
  * 
  * class SystemError(RtMidiError, OSError):             # <<<<<<<<<<<<<<
  *     """Raised if an error happened at the MIDI driver or OS level.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 308, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __Pyx_INCREF(__pyx_builtin_OSError);
   __Pyx_GIVEREF(__pyx_builtin_OSError);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_builtin_OSError);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 308, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_SystemError, __pyx_n_s_SystemError, (PyObject *) NULL, __pyx_n_s_rtmidi__rtmidi, __pyx_kp_s_Raised_if_an_error_happened_at_t); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_SystemError, __pyx_n_s_SystemError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_an_error_happened_at_t); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 308, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_SystemError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 309, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_SystemError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 308, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SystemError, __pyx_t_7) < 0) __PYX_ERR(0, 309, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_SystemError, __pyx_t_7) < 0) __PYX_ERR(0, 308, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":318
+  /* "_rtmidi.pyx":317
  * 
  * 
  * class NoDevicesError(SystemError):             # <<<<<<<<<<<<<<
  *     """Raised if no MIDI devices are found.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_SystemError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CalculateMetaclass(NULL, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_NoDevicesError, __pyx_n_s_NoDevicesError, (PyObject *) NULL, __pyx_n_s_rtmidi__rtmidi, __pyx_kp_s_Raised_if_no_MIDI_devices_are_fo); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_1, __pyx_t_4, __pyx_n_s_NoDevicesError, __pyx_n_s_NoDevicesError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_no_MIDI_devices_are_fo); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
 
-  /* "src/_rtmidi.pyx":324
+  /* "_rtmidi.pyx":323
  * 
  *     """
  *     type = ERR_NO_DEVICES_FOUND             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::NO_DEVICES_FOUND); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 324, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum__RtMidiError_3a__3a_Type(RtMidiError::NO_DEVICES_FOUND); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 324, __pyx_L1_error)
+  if (__Pyx_SetNameInClass(__pyx_t_5, __pyx_n_s_type, __pyx_t_7) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "src/_rtmidi.pyx":318
+  /* "_rtmidi.pyx":317
  * 
  * 
  * class NoDevicesError(SystemError):             # <<<<<<<<<<<<<<
  *     """Raised if no MIDI devices are found.
  * 
  */
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_NoDevicesError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 318, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_1, __pyx_n_s_NoDevicesError, __pyx_t_4, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NoDevicesError, __pyx_t_7) < 0) __PYX_ERR(0, 318, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NoDevicesError, __pyx_t_7) < 0) __PYX_ERR(0, 317, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "src/_rtmidi.pyx":327
+  /* "_rtmidi.pyx":326
  * 
  * 
  * class UnsupportedOperationError(RtMidiError, RuntimeError):             # <<<<<<<<<<<<<<
  *     """Raised if a method is not supported by the low-level API.
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_RtMidiError); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
   __Pyx_INCREF(__pyx_builtin_RuntimeError);
   __Pyx_GIVEREF(__pyx_builtin_RuntimeError);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_builtin_RuntimeError);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_CalculateMetaclass(NULL, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_UnsupportedOperationError, __pyx_n_s_UnsupportedOperationError, (PyObject *) NULL, __pyx_n_s_rtmidi__rtmidi, __pyx_kp_s_Raised_if_a_method_is_not_suppor); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_Py3MetaclassPrepare(__pyx_t_4, __pyx_t_1, __pyx_n_s_UnsupportedOperationError, __pyx_n_s_UnsupportedOperationError, (PyObject *) NULL, __pyx_n_s_rtmidi, __pyx_kp_s_Raised_if_a_method_is_not_suppor); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_UnsupportedOperationError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 327, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_Py3ClassCreate(__pyx_t_4, __pyx_n_s_UnsupportedOperationError, __pyx_t_1, __pyx_t_5, NULL, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UnsupportedOperationError, __pyx_t_7) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_UnsupportedOperationError, __pyx_t_7) < 0) __PYX_ERR(0, 326, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":338
+  /* "_rtmidi.pyx":337
  * # wrappers for RtMidi's static methods and classes
  * 
  * def get_api_display_name(api):             # <<<<<<<<<<<<<<
  *     """Return the display name of a specified MIDI API.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6rtmidi_7_rtmidi_3get_api_display_name, NULL, __pyx_n_s_rtmidi__rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 338, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_3get_api_display_name, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_api_display_name, __pyx_t_1) < 0) __PYX_ERR(0, 338, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_api_display_name, __pyx_t_1) < 0) __PYX_ERR(0, 337, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":354
+  /* "_rtmidi.pyx":353
  * 
  * 
  * def get_api_name(api):             # <<<<<<<<<<<<<<
  *     """Return the name of a specified MIDI API.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6rtmidi_7_rtmidi_5get_api_name, NULL, __pyx_n_s_rtmidi__rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 354, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_5get_api_name, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_api_name, __pyx_t_1) < 0) __PYX_ERR(0, 354, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_api_name, __pyx_t_1) < 0) __PYX_ERR(0, 353, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":370
+  /* "_rtmidi.pyx":369
  * 
  * 
  * def get_compiled_api():             # <<<<<<<<<<<<<<
  *     """Return a list of low-level MIDI backend APIs this module supports.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6rtmidi_7_rtmidi_7get_compiled_api, NULL, __pyx_n_s_rtmidi__rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_7get_compiled_api, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_compiled_api, __pyx_t_1) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_compiled_api, __pyx_t_1) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":386
+  /* "_rtmidi.pyx":385
  * 
  * 
  * def get_compiled_api_by_name(name):             # <<<<<<<<<<<<<<
  *     """Return the compiled MIDI API having the given name.
  * 
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6rtmidi_7_rtmidi_9get_compiled_api_by_name, NULL, __pyx_n_s_rtmidi__rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_9get_compiled_api_by_name, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 385, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_compiled_api_by_name, __pyx_t_1) < 0) __PYX_ERR(0, 386, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_compiled_api_by_name, __pyx_t_1) < 0) __PYX_ERR(0, 385, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":397
+  /* "_rtmidi.pyx":396
  * 
  * 
  * def get_rtmidi_version():             # <<<<<<<<<<<<<<
  *     """Return the version string of the wrapped RtMidi library."""
  *     return RtMidi_getVersion().decode('utf-8')
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6rtmidi_7_rtmidi_11get_rtmidi_version, NULL, __pyx_n_s_rtmidi__rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_11get_rtmidi_version, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_rtmidi_version, __pyx_t_1) < 0) __PYX_ERR(0, 397, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_get_rtmidi_version, __pyx_t_1) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":402
+  /* "_rtmidi.pyx":401
  * 
  * 
  * def _default_error_handler(etype, msg, data=None):             # <<<<<<<<<<<<<<
  *     if etype == ERR_MEMORY_ERROR:
  *         raise MemoryAllocationError(msg)
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6rtmidi_7_rtmidi_13_default_error_handler, NULL, __pyx_n_s_rtmidi__rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_13_default_error_handler, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_default_error_handler, __pyx_t_1) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_default_error_handler, __pyx_t_1) < 0) __PYX_ERR(0, 401, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":804
+  /* "_rtmidi.pyx":803
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None,             # <<<<<<<<<<<<<<
  *                   unsigned int queue_size_limit=1024):
  *         """Create a new client instance for MIDI input.
  */
   __pyx_k__4 = RtMidi::UNSPECIFIED;
 
-  /* "src/_rtmidi.pyx":883
+  /* "_rtmidi.pyx":882
  *         MidiBase.close_port(self)
  * 
  *     close_port.__doc__ == MidiBase.close_port.__doc__             # <<<<<<<<<<<<<<
  * 
  *     def get_message(self):
  */
-  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_6rtmidi_7_rtmidi_MidiIn, __pyx_n_s_close_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 883, __pyx_L1_error)
+  __Pyx_GetNameInClass(__pyx_t_1, (PyObject *)__pyx_ptype_7_rtmidi_MidiIn, __pyx_n_s_close_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_doc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 883, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_doc); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 882, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_6rtmidi_7_rtmidi_MidiBase), __pyx_n_s_close_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 883, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7_rtmidi_MidiBase), __pyx_n_s_close_port); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_doc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 883, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_doc); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 882, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyObject_RichCompare(__pyx_t_4, __pyx_t_5, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 883, __pyx_L1_error)
+  __pyx_t_1 = PyObject_RichCompare(__pyx_t_4, __pyx_t_5, Py_EQ); __Pyx_XGOTREF(__pyx_t_1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 882, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":1009
+  /* "_rtmidi.pyx":1008
  *         return self.thisptr
  * 
  *     def __cinit__(self, Api rtapi=UNSPECIFIED, name=None):             # <<<<<<<<<<<<<<
  *         """Create a new client instance for MIDI output.
  * 
  */
   __pyx_k__7 = RtMidi::UNSPECIFIED;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_MidiBase(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_6rtmidi_7_rtmidi_15__pyx_unpickle_MidiBase, NULL, __pyx_n_s_rtmidi__rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_7_rtmidi_15__pyx_unpickle_MidiBase, NULL, __pyx_n_s_rtmidi); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_MidiBase, __pyx_t_1) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "src/_rtmidi.pyx":1
- * # -*- encoding: utf-8 -*-             # <<<<<<<<<<<<<<
- * #cython: embedsignature=True
- * #cython: language_level=3
+  /* "_rtmidi.pyx":1
+ * # cython: embedsignature = True             # <<<<<<<<<<<<<<
+ * # cython: language_level = 3
+ * # distutils: language = c++
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "string.from_py":13
@@ -12543,19 +12658,19 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_4);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   if (__pyx_m) {
     if (__pyx_d) {
-      __Pyx_AddTraceback("init rtmidi._rtmidi", __pyx_clineno, __pyx_lineno, __pyx_filename);
+      __Pyx_AddTraceback("init _rtmidi", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     Py_CLEAR(__pyx_m);
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init rtmidi._rtmidi");
+    PyErr_SetString(PyExc_ImportError, "init _rtmidi");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
@@ -12660,18 +12775,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* PyFunctionFastCall */
 #if CYTHON_FAST_PYCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
@@ -12812,15 +12925,15 @@
 }
 #endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = func->ob_type->tp_call;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -12863,17 +12976,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -13336,28 +13447,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -13589,15 +13700,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -13778,15 +13889,15 @@
         ps2 = PyBytes_AS_STRING(s2);
         if (ps1[0] != ps2[0]) {
             return (equals == Py_NE);
         } else if (length == 1) {
             return (equals == Py_EQ);
         } else {
             int result;
-#if CYTHON_USE_UNICODE_INTERNALS
+#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
             Py_hash_t hash1, hash2;
             hash1 = ((PyBytesObject*)s1)->ob_shash;
             hash2 = ((PyBytesObject*)s2)->ob_shash;
             if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
                 return (equals == Py_NE);
             }
 #endif
@@ -14331,25 +14442,43 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
+    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
+    PyObject *getstate = NULL;
 #if CYTHON_USE_PYTYPE_LOOKUP
-    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
 #else
-    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
+    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
+    if (!getstate && PyErr_Occurred()) {
+        goto __PYX_BAD;
+    }
 #endif
+    if (getstate) {
+#if CYTHON_USE_PYTYPE_LOOKUP
+        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+#else
+        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
+        if (!object_getstate && PyErr_Occurred()) {
+            goto __PYX_BAD;
+        }
+#endif
+        if (object_getstate != getstate) {
+            goto __PYX_GOOD;
+        }
+    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -14386,14 +14515,16 @@
     if (!PyErr_Occurred())
         PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
+    Py_XDECREF(object_getstate);
+    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
@@ -14766,15 +14897,16 @@
     {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), PY_WRITE_RESTRICTED, 0},
     {0, 0, 0,  0, 0}
 };
 static PyObject *
 __Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, CYTHON_UNUSED PyObject *args)
 {
 #if PY_MAJOR_VERSION >= 3
-    return PyUnicode_FromString(m->func.m_ml->ml_name);
+    Py_INCREF(m->func_qualname);
+    return m->func_qualname;
 #else
     return PyString_FromString(m->func.m_ml->ml_name);
 #endif
 }
 static PyMethodDef __pyx_CyFunction_methods[] = {
     {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
     {0, 0, 0, 0}
@@ -14969,14 +15101,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
+            PyErr_Format(PyExc_TypeError,
+                         "unbound method %.200S() needs an argument",
+                         cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -15037,20 +15177,23 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+    0,
+#endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
     }
     return 0;
@@ -15200,15 +15343,15 @@
         result = __Pyx_GetGlobalNameAfterAttributeLookup(name);
     }
     return result;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -15230,15 +15373,15 @@
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
@@ -15324,41 +15467,48 @@
     Py_INCREF(code_object);
 }
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
+#if PY_VERSION_HEX >= 0x030b00a6
+  #ifndef Py_BUILD_CORE
+    #define Py_BUILD_CORE 1
+  #endif
+  #include "internal/pycore_frame.h"
+#endif
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = 0;
-    PyObject *py_srcfile = 0;
-    PyObject *py_funcname = 0;
+    PyCodeObject *py_code = NULL;
+    PyObject *py_funcname = NULL;
     #if PY_MAJOR_VERSION < 3
+    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    #else
-    py_srcfile = PyUnicode_FromString(filename);
-    #endif
     if (!py_srcfile) goto bad;
+    #endif
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
+        if (!py_funcname) goto bad;
+        funcname = PyUnicode_AsUTF8(py_funcname);
+        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        #else
-        py_funcname = PyUnicode_FromString(funcname);
+        if (!py_funcname) goto bad;
         #endif
     }
-    if (!py_funcname) goto bad;
+    #if PY_MAJOR_VERSION < 3
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
         __pyx_empty_bytes, /*PyObject *code,*/
@@ -15369,34 +15519,49 @@
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    Py_DECREF(py_funcname);
+    #else
+    py_code = PyCode_NewEmpty(filename, funcname, py_line);
+    #endif
+    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
     return py_code;
 bad:
-    Py_XDECREF(py_srcfile);
     Py_XDECREF(py_funcname);
+    #if PY_MAJOR_VERSION < 3
+    Py_XDECREF(py_srcfile);
+    #endif
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
+    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
+        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) goto bad;
+        if (!py_code) {
+            /* If the code object creation fails, then we should clear the
+               fetched exception references and propagate the new exception */
+            Py_XDECREF(ptype);
+            Py_XDECREF(pvalue);
+            Py_XDECREF(ptraceback);
+            goto bad;
+        }
+        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -16908,19 +17073,41 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[4], rtversion[4];
-    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
-    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
+    char ctversion[5];
+    int same=1, i, found_dot;
+    const char* rt_from_call = Py_GetVersion();
+    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    found_dot = 0;
+    for (i = 0; i < 4; i++) {
+        if (!ctversion[i]) {
+            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
+            break;
+        }
+        if (rt_from_call[i] != ctversion[i]) {
+            same = 0;
+            break;
+        }
+    }
+    if (!same) {
+        char rtversion[5] = {'\0'};
         char message[200];
+        for (i=0; i<4; ++i) {
+            if (rt_from_call[i] == '.') {
+                if (found_dot) break;
+                found_dot = 1;
+            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
+                break;
+            }
+            rtversion[i] = rt_from_call[i];
+        }
         PyOS_snprintf(message, sizeof(message),
                       "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
@@ -17172,15 +17359,15 @@
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
 static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
   if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
-    return __Pyx_PyIndex_AsSsize_t(o);
+    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
 #if PY_MAJOR_VERSION < 3
   } else if (likely(PyInt_CheckExact(o))) {
     return PyInt_AS_LONG(o);
 #endif
   } else {
     Py_ssize_t ival;
     PyObject *x;
```

### Comparing `python-rtmidi-1.4.9/src/_rtmidi.pyx` & `python-rtmidi-1.5.0/src/_rtmidi.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# -*- encoding: utf-8 -*-
-#cython: embedsignature=True
-#cython: language_level=3
+# cython: embedsignature = True
+# cython: language_level = 3
+# distutils: language = c++
 #
 # rtmidi.pyx
 #
 """A Python binding for the RtMidi C++ library implemented using Cython.
 
 Overview
 ========
@@ -126,19 +126,18 @@
 )
 
 if bytes is str:
     string_types = (str, unicode)
 else:
     string_types = (str,)
 
+cdef extern from "Python.h":
+    void Py_Initialize()
 
-cdef extern from "pyinit.h":
-    void py_init()
-
-py_init()
+Py_Initialize()
 
 # Declarations for RtMidi C++ classes and their methods we use
 
 cdef extern from "RtMidi.h":
     # Enums nested in classes are apparently not supported by Cython yet
     # therefore we need to use the following work-around.
     # https://groups.google.com/d/msg/cython-users/monwJxJCb-g/k_h1rcU-3TgJ
```

### Comparing `python-rtmidi-1.4.9/src/rtmidi/RtMidi.cpp` & `python-rtmidi-1.5.0/src/rtmidi/RtMidi.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     This class implements some common functionality for the realtime
     MIDI input/output subclasses RtMidiIn and RtMidiOut.
 
     RtMidi GitHub site: https://github.com/thestk/rtmidi
     RtMidi WWW site: http://www.music.mcgill.ca/~gary/rtmidi/
 
     RtMidi: realtime MIDI i/o C++ classes
-    Copyright (c) 2003-2019 Gary P. Scavone
+    Copyright (c) 2003-2021 Gary P. Scavone
 
     Permission is hereby granted, free of charge, to any person
     obtaining a copy of this software and associated documentation files
     (the "Software"), to deal in the Software without restriction,
     including without limitation the rights to use, copy, modify, merge,
     publish, distribute, sublicense, and/or sell copies of the Software,
     and to permit persons to whom the Software is furnished to do so,
@@ -73,19 +73,20 @@
 
 // **************************************************************** //
 //
 // MidiInApi and MidiOutApi subclass prototypes.
 //
 // **************************************************************** //
 
-#if !defined(__LINUX_ALSA__) && !defined(__UNIX_JACK__) && !defined(__MACOSX_CORE__) && !defined(__WINDOWS_MM__) && !defined(TARGET_IPHONE_OS)
+#if !defined(__LINUX_ALSA__) && !defined(__UNIX_JACK__) && !defined(__MACOSX_CORE__) && !defined(__WINDOWS_MM__) && !defined(TARGET_IPHONE_OS) && !defined(__WEB_MIDI_API__)
   #define __RTMIDI_DUMMY__
 #endif
 
 #if defined(__MACOSX_CORE__)
+#include <CoreMIDI/CoreMIDI.h>
 
 class MidiInCore: public MidiInApi
 {
  public:
   MidiInCore( const std::string &clientName, unsigned int queueSizeLimit );
   ~MidiInCore( void );
   RtMidi::Api getCurrentApi( void ) { return RtMidi::MACOSX_CORE; };
@@ -249,14 +250,65 @@
 
  protected:
   void initialize( const std::string& clientName );
 };
 
 #endif
 
+#if defined(__WEB_MIDI_API__)
+
+class MidiInWeb : public MidiInApi
+{
+  std::string client_name{};
+  std::string web_midi_id{};
+  int open_port_number{-1};
+
+ public:
+  MidiInWeb(const std::string &/*clientName*/, unsigned int queueSizeLimit );
+  ~MidiInWeb( void );
+  RtMidi::Api getCurrentApi( void ) { return RtMidi::WEB_MIDI_API; };
+  void openPort( unsigned int portNumber, const std::string &portName );
+  void openVirtualPort( const std::string &portName );
+  void closePort( void );
+  void setClientName( const std::string &clientName );
+  void setPortName( const std::string &portName );
+  unsigned int getPortCount( void );
+  std::string getPortName( unsigned int portNumber );
+
+  void onMidiMessage( uint8_t* data, double domHishResTimeStamp );
+
+ protected:
+  void initialize( const std::string& clientName );
+};
+
+class MidiOutWeb: public MidiOutApi
+{
+  std::string client_name{};
+  std::string web_midi_id{};
+  int open_port_number{-1};
+
+ public:
+  MidiOutWeb( const std::string &clientName );
+  ~MidiOutWeb( void );
+  RtMidi::Api getCurrentApi( void ) { return RtMidi::WEB_MIDI_API; };
+  void openPort( unsigned int portNumber, const std::string &portName );
+  void openVirtualPort( const std::string &portName );
+  void closePort( void );
+  void setClientName( const std::string &clientName );
+  void setPortName( const std::string &portName );
+  unsigned int getPortCount( void );
+  std::string getPortName( unsigned int portNumber );
+  void sendMessage( const unsigned char *message, size_t size );
+
+ protected:
+  void initialize( const std::string& clientName );
+};
+
+#endif
+
 #if defined(__RTMIDI_DUMMY__)
 
 class MidiInDummy: public MidiInApi
 {
  public:
  MidiInDummy( const std::string &/*clientName*/, unsigned int queueSizeLimit ) : MidiInApi( queueSizeLimit ) { errorString_ = "MidiInDummy: This class provides no functionality."; error( RtMidiError::WARNING, errorString_ ); }
   RtMidi::Api getCurrentApi( void ) { return RtMidi::RTMIDI_DUMMY; }
@@ -303,28 +355,34 @@
 
 RtMidi :: ~RtMidi()
 {
   delete rtapi_;
   rtapi_ = 0;
 }
 
+RtMidi::RtMidi(RtMidi&& other) noexcept {
+    rtapi_ = other.rtapi_;
+    other.rtapi_ = nullptr;
+}
+
 std::string RtMidi :: getVersion( void ) throw()
 {
   return std::string( RTMIDI_VERSION );
 }
 
 // Define API names and display names.
 // Must be in same order as API enum.
 extern "C" {
 const char* rtmidi_api_names[][2] = {
   { "unspecified" , "Unknown" },
   { "core"        , "CoreMidi" },
   { "alsa"        , "ALSA" },
   { "jack"        , "Jack" },
   { "winmm"       , "Windows MultiMedia" },
+  { "web"         , "Web MIDI API" },
   { "dummy"       , "Dummy" },
 };
 const unsigned int rtmidi_num_api_names =
   sizeof(rtmidi_api_names)/sizeof(rtmidi_api_names[0]);
 
 // The order here will control the order of RtMidi's API search in
 // the constructor.
@@ -337,14 +395,17 @@
 #endif
 #if defined(__UNIX_JACK__)
   RtMidi::UNIX_JACK,
 #endif
 #if defined(__WINDOWS_MM__)
   RtMidi::WINDOWS_MM,
 #endif
+#if defined(__WEB_MIDI_API__)
+  RtMidi::WEB_MIDI_API,
+#endif
 #if defined(__RTMIDI_DUMMY__)
   RtMidi::RTMIDI_DUMMY,
 #endif
   RtMidi::UNSPECIFIED,
 };
 extern "C" const unsigned int rtmidi_num_compiled_apis =
   sizeof(rtmidi_compiled_apis)/sizeof(rtmidi_compiled_apis[0])-1;
@@ -362,22 +423,22 @@
 {
   apis = std::vector<RtMidi::Api>(rtmidi_compiled_apis,
                                   rtmidi_compiled_apis + rtmidi_num_compiled_apis);
 }
 
 std::string RtMidi :: getApiName( RtMidi::Api api )
 {
-  if (api < 0 || api >= RtMidi::NUM_APIS)
+  if (api < RtMidi::UNSPECIFIED || api >= RtMidi::NUM_APIS)
     return "";
   return rtmidi_api_names[api][0];
 }
 
 std::string RtMidi :: getApiDisplayName( RtMidi::Api api )
 {
-  if (api < 0 || api >= RtMidi::NUM_APIS)
+  if (api < RtMidi::UNSPECIFIED || api >= RtMidi::NUM_APIS)
     return "Unknown";
   return rtmidi_api_names[api][1];
 }
 
 RtMidi::Api RtMidi :: getCompiledApiByName( const std::string &name )
 {
   unsigned int i=0;
@@ -419,14 +480,18 @@
   if ( api == WINDOWS_MM )
     rtapi_ = new MidiInWinMM( clientName, queueSizeLimit );
 #endif
 #if defined(__MACOSX_CORE__)
   if ( api == MACOSX_CORE )
     rtapi_ = new MidiInCore( clientName, queueSizeLimit );
 #endif
+#if defined(__WEB_MIDI_API__)
+    if ( api == WEB_MIDI_API )
+    rtapi_ = new MidiInWeb( clientName, queueSizeLimit );
+#endif
 #if defined(__RTMIDI_DUMMY__)
   if ( api == RTMIDI_DUMMY )
     rtapi_ = new MidiInDummy( clientName, queueSizeLimit );
 #endif
 }
 
 RTMIDI_DLL_PUBLIC RtMidiIn :: RtMidiIn( RtMidi::Api api, const std::string &clientName, unsigned int queueSizeLimit )
@@ -487,14 +552,18 @@
   if ( api == WINDOWS_MM )
     rtapi_ = new MidiOutWinMM( clientName );
 #endif
 #if defined(__MACOSX_CORE__)
   if ( api == MACOSX_CORE )
     rtapi_ = new MidiOutCore( clientName );
 #endif
+#if defined(__WEB_MIDI_API__)
+    if ( api == WEB_MIDI_API )
+    rtapi_ = new MidiOutWeb( clientName );
+#endif
 #if defined(__RTMIDI_DUMMY__)
   if ( api == RTMIDI_DUMMY )
     rtapi_ = new MidiOutDummy( clientName );
 #endif
 }
 
 RTMIDI_DLL_PUBLIC RtMidiOut :: RtMidiOut( RtMidi::Api api, const std::string &clientName)
@@ -654,14 +723,20 @@
   double timeStamp;
   if ( !inputData_.queue.pop( message, &timeStamp ) )
     return 0.0;
 
   return timeStamp;
 }
 
+void MidiInApi :: setBufferSize( unsigned int size, unsigned int count )
+{
+    inputData_.bufferSize = size;
+    inputData_.bufferCount = count;
+}
+
 unsigned int MidiInApi::MidiQueue::size( unsigned int *__back,
                                          unsigned int *__front )
 {
   // Access back/front members exactly once and make stack copies for
   // size calculation
   unsigned int _back = back, _front = front, _size;
   if ( _back >= _front )
@@ -736,17 +811,15 @@
 
 #if defined(__MACOSX_CORE__)
 
 // The CoreMIDI API is based on the use of a callback function for
 // MIDI input.  We convert the system specific time stamps to delta
 // time values.
 
-// OS-X CoreMIDI header files. (<CoreMIDI/CoreMIDI.h> moved to RtMidi.h)
-
-// these are not available on iOS.
+// These are not available on iOS.
 #if (TARGET_OS_IPHONE == 0)
   #include <CoreAudio/HostTime.h>
   #include <CoreServices/CoreServices.h>
 #endif
 
 // A structure to hold variables related to the CoreMIDI API
 // implementation.
@@ -755,15 +828,14 @@
   MIDIPortRef port;
   MIDIEndpointRef endpoint;
   MIDIEndpointRef destinationId;
   unsigned long long lastTime;
   MIDISysexSendRequest sysexreq;
 };
 
-
 static MIDIClientRef CoreMidiClientSingleton = 0;
 
 void RtMidi_setCoreMidiClientSingleton(MIDIClientRef client){
   CoreMidiClientSingleton = client;
 }
 
 void RtMidi_disposeCoreMidiClientSingleton(){
@@ -1115,14 +1187,19 @@
   str = NULL;
   MIDIObjectGetStringProperty( endpoint, kMIDIPropertyName, &str );
   if ( str != NULL ) {
     CFStringAppend( result, str );
     CFRelease( str );
   }
 
+  // some MIDI devices have a leading space in endpoint name. trim
+  CFStringRef space = CFStringCreateWithCString(NULL, " ", kCFStringEncodingUTF8);
+  CFStringTrim(result, space);
+  CFRelease(space);
+
   MIDIEntityRef entity = 0;
   MIDIEndpointGetEntity( endpoint, &entity );
   if ( entity == 0 )
     // probably virtual
     return result;
 
   if ( CFStringGetLength( result ) == 0 ) {
@@ -1459,58 +1536,62 @@
   unsigned int nBytes = static_cast<unsigned int> (size);
   if ( nBytes == 0 ) {
     errorString_ = "MidiOutCore::sendMessage: no data in message argument!";
     error( RtMidiError::WARNING, errorString_ );
     return;
   }
 
-  MIDITimeStamp timeStamp = AudioGetCurrentHostTime();
-  CoreMidiData *data = static_cast<CoreMidiData *> (apiData_);
-  OSStatus result;
-
   if ( message[0] != 0xF0 && nBytes > 3 ) {
     errorString_ = "MidiOutCore::sendMessage: message format problem ... not sysex but > 3 bytes?";
     error( RtMidiError::WARNING, errorString_ );
     return;
   }
 
-  Byte buffer[nBytes+(sizeof( MIDIPacketList ))];
+  MIDITimeStamp timeStamp = AudioGetCurrentHostTime();
+  CoreMidiData *data = static_cast<CoreMidiData *> (apiData_);
+  OSStatus result;
+
+  ByteCount bufsize = nBytes > 65535 ? 65535 : nBytes;
+  Byte buffer[bufsize+16]; // pad for other struct members
   ByteCount listSize = sizeof( buffer );
   MIDIPacketList *packetList = (MIDIPacketList*)buffer;
-  MIDIPacket *packet = MIDIPacketListInit( packetList );
 
   ByteCount remainingBytes = nBytes;
-  while ( remainingBytes && packet ) {
-    ByteCount bytesForPacket = remainingBytes > 65535 ? 65535 : remainingBytes; // 65535 = maximum size of a MIDIPacket
+  while ( remainingBytes ) {
+    MIDIPacket *packet = MIDIPacketListInit( packetList );
+    // A MIDIPacketList can only contain a maximum of 64K of data, so if our message is longer,
+    // break it up into chunks of 64K or less and send out as a MIDIPacketList with only one
+    // MIDIPacket. Here, we reuse the memory allocated above on the stack for all.
+    ByteCount bytesForPacket = remainingBytes > 65535 ? 65535 : remainingBytes;
     const Byte* dataStartPtr = (const Byte *) &message[nBytes - remainingBytes];
     packet = MIDIPacketListAdd( packetList, listSize, packet, timeStamp, bytesForPacket, dataStartPtr );
     remainingBytes -= bytesForPacket;
-  }
 
-  if ( !packet ) {
-    errorString_ = "MidiOutCore::sendMessage: could not allocate packet list";
-    error( RtMidiError::DRIVER_ERROR, errorString_ );
-    return;
-  }
+    if ( !packet ) {
+      errorString_ = "MidiOutCore::sendMessage: could not allocate packet list";
+      error( RtMidiError::DRIVER_ERROR, errorString_ );
+      return;
+    }
 
-  // Send to any destinations that may have connected to us.
-  if ( data->endpoint ) {
-    result = MIDIReceived( data->endpoint, packetList );
-    if ( result != noErr ) {
-      errorString_ = "MidiOutCore::sendMessage: error sending MIDI to virtual destinations.";
-      error( RtMidiError::WARNING, errorString_ );
+    // Send to any destinations that may have connected to us.
+    if ( data->endpoint ) {
+      result = MIDIReceived( data->endpoint, packetList );
+      if ( result != noErr ) {
+        errorString_ = "MidiOutCore::sendMessage: error sending MIDI to virtual destinations.";
+        error( RtMidiError::WARNING, errorString_ );
+      }
     }
-  }
 
-  // And send to an explicit destination port if we're connected.
-  if ( connected_ ) {
-    result = MIDISend( data->port, data->destinationId, packetList );
-    if ( result != noErr ) {
-      errorString_ = "MidiOutCore::sendMessage: error sending MIDI message to port.";
-      error( RtMidiError::WARNING, errorString_ );
+    // And send to an explicit destination port if we're connected.
+    if ( connected_ ) {
+      result = MIDISend( data->port, data->destinationId, packetList );
+      if ( result != noErr ) {
+        errorString_ = "MidiOutCore::sendMessage: error sending MIDI message to port.";
+        error( RtMidiError::WARNING, errorString_ );
+      }
     }
   }
 }
 
 #endif  // __MACOSX_CORE__
 
 
@@ -1544,14 +1625,15 @@
 struct AlsaMidiData {
   snd_seq_t *seq;
   unsigned int portNum;
   int vport;
   snd_seq_port_subscribe_t *subscription;
   snd_midi_event_t *coder;
   unsigned int bufferSize;
+  unsigned int requestedBufferSize;
   unsigned char *buffer;
   pthread_t thread;
   pthread_t dummy_thread_id;
   snd_seq_real_time_t lastTime;
   int queue_id; // an input queue is needed to get timestamped events
   int trigger_fds[2];
 };
@@ -1574,15 +1656,14 @@
   bool doDecode = false;
   MidiInApi::MidiMessage message;
   int poll_fd_count;
   struct pollfd *poll_fds;
 
   snd_seq_event_t *ev;
   int result;
-  apiData->bufferSize = 32;
   result = snd_midi_event_new( 0, &apiData->coder );
   if ( result < 0 ) {
     data->doInput = false;
     std::cerr << "\nMidiInAlsa::alsaMidiHandler: error initializing MIDI event parser!\n\n";
     return 0;
   }
   unsigned char *buffer = (unsigned char *) malloc( apiData->bufferSize );
@@ -1826,14 +1907,15 @@
   data->portNum = -1;
   data->vport = -1;
   data->subscription = 0;
   data->dummy_thread_id = pthread_self();
   data->thread = data->dummy_thread_id;
   data->trigger_fds[0] = -1;
   data->trigger_fds[1] = -1;
+  data->bufferSize = inputData_.bufferSize;
   apiData_ = (void *) data;
   inputData_.apiData = (void *) data;
 
   if ( pipe(data->trigger_fds) == -1 ) {
     errorString_ = "MidiInAlsa::initialize: error creating pipe objects.";
     error( RtMidiError::DRIVER_ERROR, errorString_ );
     return;
@@ -2466,15 +2548,15 @@
 // A structure to hold variables related to the CoreMIDI API
 // implementation.
 struct WinMidiData {
   HMIDIIN inHandle;    // Handle to Midi Input Device
   HMIDIOUT outHandle;  // Handle to Midi Output Device
   DWORD lastTime;
   MidiInApi::MidiMessage message;
-  LPMIDIHDR sysexBuffer[RT_SYSEX_BUFFER_COUNT];
+  std::vector<LPMIDIHDR> sysexBuffer;
   CRITICAL_SECTION _mutex; // [Patrice] see https://groups.google.com/forum/#!topic/mididev/6OUjHutMpEo
 };
 
 //*********************************************************************//
 //  API: Windows MM
 //  Class Definitions: MidiInWinMM
 //*********************************************************************//
@@ -2646,18 +2728,19 @@
   if ( result != MMSYSERR_NOERROR ) {
     errorString_ = "MidiInWinMM::openPort: error creating Windows MM MIDI input port.";
     error( RtMidiError::DRIVER_ERROR, errorString_ );
     return;
   }
 
   // Allocate and init the sysex buffers.
-  for ( int i=0; i<RT_SYSEX_BUFFER_COUNT; ++i ) {
+  data->sysexBuffer.resize( inputData_.bufferCount );
+  for ( int i=0; i < inputData_.bufferCount; ++i ) {
     data->sysexBuffer[i] = (MIDIHDR*) new char[ sizeof(MIDIHDR) ];
-    data->sysexBuffer[i]->lpData = new char[ RT_SYSEX_BUFFER_SIZE ];
-    data->sysexBuffer[i]->dwBufferLength = RT_SYSEX_BUFFER_SIZE;
+    data->sysexBuffer[i]->lpData = new char[ inputData_.bufferSize ];
+    data->sysexBuffer[i]->dwBufferLength = inputData_.bufferSize;
     data->sysexBuffer[i]->dwUser = i; // We use the dwUser parameter as buffer indicator
     data->sysexBuffer[i]->dwFlags = 0;
 
     result = midiInPrepareHeader( data->inHandle, data->sysexBuffer[i], sizeof(MIDIHDR) );
     if ( result != MMSYSERR_NOERROR ) {
       midiInClose( data->inHandle );
       data->inHandle = 0;
@@ -2700,15 +2783,15 @@
 {
   if ( connected_ ) {
     WinMidiData *data = static_cast<WinMidiData *> (apiData_);
     EnterCriticalSection( &(data->_mutex) );
     midiInReset( data->inHandle );
     midiInStop( data->inHandle );
 
-    for ( int i=0; i<RT_SYSEX_BUFFER_COUNT; ++i ) {
+    for ( int i=0; i < data->sysexBuffer.size(); ++i ) {
       int result = midiInUnprepareHeader(data->inHandle, data->sysexBuffer[i], sizeof(MIDIHDR));
       delete [] data->sysexBuffer[i]->lpData;
       delete [] data->sysexBuffer[i];
       if ( result != MMSYSERR_NOERROR ) {
         midiInClose( data->inHandle );
         data->inHandle = 0;
         errorString_ = "MidiInWinMM::openPort: error closing Windows MM MIDI input port (midiInUnprepareHeader).";
@@ -2881,15 +2964,18 @@
   connected_ = true;
 }
 
 void MidiOutWinMM :: closePort( void )
 {
   if ( connected_ ) {
     WinMidiData *data = static_cast<WinMidiData *> (apiData_);
-    midiOutReset( data->outHandle );
+    // Disabled because midiOutReset triggers 0x7b (if any note was ON) and 0x79 "Reset All
+    // Controllers" (to all 16 channels) CC messages which is undesirable (see issue #222)
+    // midiOutReset( data->outHandle );
+
     midiOutClose( data->outHandle );
     data->outHandle = 0;
     connected_ = false;
   }
 }
 
 void MidiOutWinMM :: setClientName ( const std::string& )
@@ -3006,25 +3092,26 @@
 
 #if defined(__UNIX_JACK__)
 
 // JACK header files
 #include <jack/jack.h>
 #include <jack/midiport.h>
 #include <jack/ringbuffer.h>
+#include <pthread.h>
 #ifdef HAVE_SEMAPHORE
   #include <semaphore.h>
 #endif
 
 #define JACK_RINGBUFFER_SIZE 16384 // Default size for ringbuffer
 
 struct JackMidiData {
   jack_client_t *client;
   jack_port_t *port;
-  jack_ringbuffer_t *buffSize;
-  jack_ringbuffer_t *buffMessage;
+  jack_ringbuffer_t *buff;
+  int buffMaxWrite; // actual writable size, usually 1 less than ringbuffer
   jack_time_t lastTime;
 #ifdef HAVE_SEMAPHORE
   sem_t sem_cleanup;
   sem_t sem_needpost;
 #endif
   MidiInApi :: RtMidiInData *rtMidiIn;
   };
@@ -3171,14 +3258,16 @@
   // Creating new port
   if ( data->port == NULL )
     data->port = jack_port_register( data->client, portName.c_str(),
                                      JACK_DEFAULT_MIDI_TYPE, JackPortIsInput, 0 );
 
   if ( data->port == NULL ) {
     errorString_ = "MidiInJack::openPort: JACK error creating port";
+    if (portName.size() >= (size_t)jack_port_name_size())
+        errorString_ += " (port name too long?)";
     error( RtMidiError::DRIVER_ERROR, errorString_ );
     return;
   }
 
   // Connecting to the output
   std::string name = getPortName( portNumber );
   jack_connect( data->client, name.c_str(), jack_port_name( data->port ) );
@@ -3193,14 +3282,16 @@
   connect();
   if ( data->port == NULL )
     data->port = jack_port_register( data->client, portName.c_str(),
                                      JACK_DEFAULT_MIDI_TYPE, JackPortIsInput, 0 );
 
   if ( data->port == NULL ) {
     errorString_ = "MidiInJack::openVirtualPort: JACK error creating virtual port";
+    if (portName.size() >= (size_t)jack_port_name_size())
+        errorString_ += " (port name too long?)";
     error( RtMidiError::DRIVER_ERROR, errorString_ );
   }
 }
 
 unsigned int MidiInJack :: getPortCount()
 {
   int count = 0;
@@ -3296,19 +3387,23 @@
 
   // Is port created?
   if ( data->port == NULL ) return 0;
 
   void *buff = jack_port_get_buffer( data->port, nframes );
   jack_midi_clear_buffer( buff );
 
-  while ( jack_ringbuffer_read_space( data->buffSize ) > 0 ) {
-    jack_ringbuffer_read( data->buffSize, (char *) &space, (size_t) sizeof( space ) );
-    midiData = jack_midi_event_reserve( buff, 0, space );
+  while ( jack_ringbuffer_peek( data->buff, (char *) &space, sizeof( space ) ) == sizeof(space) &&
+          jack_ringbuffer_read_space( data->buff ) >= sizeof(space) + space ) {
+    jack_ringbuffer_read_advance( data->buff, sizeof(space) );
 
-    jack_ringbuffer_read( data->buffMessage, (char *) midiData, (size_t) space );
+    midiData = jack_midi_event_reserve( buff, 0, space );
+    if ( midiData )
+        jack_ringbuffer_read( data->buff, (char *) midiData, (size_t) space );
+    else
+        jack_ringbuffer_read_advance( data->buff, (size_t) space );
   }
 
 #ifdef HAVE_SEMAPHORE
   if ( !sem_trywait( &data->sem_needpost ) )
     sem_post( &data->sem_cleanup );
 #endif
 
@@ -3339,16 +3434,16 @@
 void MidiOutJack :: connect()
 {
   JackMidiData *data = static_cast<JackMidiData *> (apiData_);
   if ( data->client )
     return;
 
   // Initialize output ringbuffers
-  data->buffSize = jack_ringbuffer_create( JACK_RINGBUFFER_SIZE );
-  data->buffMessage = jack_ringbuffer_create( JACK_RINGBUFFER_SIZE );
+  data->buff = jack_ringbuffer_create( JACK_RINGBUFFER_SIZE );
+  data->buffMaxWrite = (int) jack_ringbuffer_write_space( data->buff );
 
   // Initialize JACK client
   if ( ( data->client = jack_client_open( clientName.c_str(), JackNoStartServer, NULL ) ) == 0 ) {
     errorString_ = "MidiOutJack::initialize: JACK server not running?";
     error( RtMidiError::DRIVER_ERROR, errorString_ );
     return;
   }
@@ -3359,16 +3454,15 @@
 
 MidiOutJack :: ~MidiOutJack()
 {
   JackMidiData *data = static_cast<JackMidiData *> (apiData_);
   MidiOutJack::closePort();
 
   // Cleanup
-  jack_ringbuffer_free( data->buffSize );
-  jack_ringbuffer_free( data->buffMessage );
+  jack_ringbuffer_free( data->buff );
   if ( data->client ) {
     jack_client_close( data->client );
   }
 
 #ifdef HAVE_SEMAPHORE
   sem_destroy( &data->sem_cleanup );
   sem_destroy( &data->sem_needpost );
@@ -3386,14 +3480,16 @@
   // Creating new port
   if ( data->port == NULL )
     data->port = jack_port_register( data->client, portName.c_str(),
                                      JACK_DEFAULT_MIDI_TYPE, JackPortIsOutput, 0 );
 
   if ( data->port == NULL ) {
     errorString_ = "MidiOutJack::openPort: JACK error creating port";
+    if (portName.size() >= (size_t)jack_port_name_size())
+        errorString_ += " (port name too long?)";
     error( RtMidiError::DRIVER_ERROR, errorString_ );
     return;
   }
 
   // Connecting to the output
   std::string name = getPortName( portNumber );
   jack_connect( data->client, jack_port_name( data->port ), name.c_str() );
@@ -3408,14 +3504,16 @@
   connect();
   if ( data->port == NULL )
     data->port = jack_port_register( data->client, portName.c_str(),
                                      JACK_DEFAULT_MIDI_TYPE, JackPortIsOutput, 0 );
 
   if ( data->port == NULL ) {
     errorString_ = "MidiOutJack::openVirtualPort: JACK error creating virtual port";
+    if (portName.size() >= (size_t)jack_port_name_size())
+        errorString_ += " (port name too long?)";
     error( RtMidiError::DRIVER_ERROR, errorString_ );
   }
 }
 
 unsigned int MidiOutJack :: getPortCount()
 {
   int count = 0;
@@ -3507,13 +3605,335 @@
 }
 
 void MidiOutJack :: sendMessage( const unsigned char *message, size_t size )
 {
   int nBytes = static_cast<int>(size);
   JackMidiData *data = static_cast<JackMidiData *> (apiData_);
 
+  if ( size + sizeof(nBytes) > (size_t) data->buffMaxWrite )
+      return;
+
+  while ( jack_ringbuffer_write_space(data->buff) < sizeof(nBytes) + size )
+      pthread_yield();
+
   // Write full message to buffer
-  jack_ringbuffer_write( data->buffMessage, ( const char * ) message, nBytes );
-  jack_ringbuffer_write( data->buffSize, ( char * ) &nBytes, sizeof( nBytes ) );
+  jack_ringbuffer_write( data->buff, ( char * ) &nBytes, sizeof( nBytes ) );
+  jack_ringbuffer_write( data->buff, ( const char * ) message, nBytes );
 }
 
 #endif  // __UNIX_JACK__
+
+//*********************************************************************//
+//  API: Web MIDI
+//
+//  Written primarily by Atsushi Eno, February 2020.
+//
+//  *********************************************************************//
+
+#if defined(__WEB_MIDI_API__)
+
+#include <emscripten.h>
+
+//*********************************************************************//
+//  API: WEB MIDI
+//  Class Definitions: WebMidiAccessShim
+//*********************************************************************//
+
+class WebMidiAccessShim
+{
+public:
+  WebMidiAccessShim();
+  ~WebMidiAccessShim();
+  std::string getPortName( unsigned int portNumber, bool isInput );
+};
+
+std::unique_ptr<WebMidiAccessShim> shim{nullptr};
+
+void ensureShim()
+{
+  if ( shim.get() != nullptr )
+    return;
+  shim.reset( new WebMidiAccessShim() );
+}
+
+bool checkWebMidiAvailability()
+{
+  ensureShim();
+
+  return MAIN_THREAD_EM_ASM_INT( {
+    if ( typeof window._rtmidi_internals_waiting === "undefined" ) {
+      console.log ( "Attempted to use Web MIDI API without trying to open it." );
+      return false;
+    }
+    if ( window._rtmidi_internals_waiting ) {
+      console.log ( "Attempted to use Web MIDI API while it is being queried." );
+      return false;
+    }
+    if ( _rtmidi_internals_midi_access == null ) {
+      console.log ( "Attempted to use Web MIDI API while it already turned out to be unavailable." );
+      return false;
+    }
+    return true;
+  } );
+}
+
+WebMidiAccessShim::WebMidiAccessShim()
+{
+  MAIN_THREAD_ASYNC_EM_ASM( {
+    if( typeof window._rtmidi_internals_midi_access !== "undefined" )
+      return;
+    if( typeof window._rtmidi_internals_waiting !== "undefined" ) {
+       console.log( "MIDI Access was requested while another request is in progress." );
+       return;
+    }
+
+    // define functions
+    window._rtmidi_internals_get_port_by_number = function( portNumber, isInput ) {
+      var midi = window._rtmidi_internals_midi_access;
+      var devices = isInput ? midi.inputs : midi.outputs;
+      var i = 0;
+      for (var device of devices.values()) {
+        if ( i == portNumber )
+          return device;
+        i++;
+      }
+      console.log( "MIDI " + (isInput ? "input" : "output") + " device of portNumber " + portNumber + " is not found.");
+      return null;
+    };
+
+    window._rtmidi_internals_waiting = true;
+    window.navigator.requestMIDIAccess( {"sysex": true} ).then( (midiAccess) => {
+      window._rtmidi_internals_midi_access = midiAccess;
+      window._rtmidi_internals_latest_message_timestamp = 0.0;
+      window._rtmidi_internals_waiting = false;
+      if( midiAccess == null ) {
+        console.log ( "Could not get access to MIDI API" );
+      }
+    } );
+  } );
+}
+
+WebMidiAccessShim::~WebMidiAccessShim()
+{
+}
+
+std::string WebMidiAccessShim::getPortName( unsigned int portNumber, bool isInput )
+{
+  if( !checkWebMidiAvailability() )
+    return "";
+  char *ret = (char*) MAIN_THREAD_EM_ASM_INT( {
+    var port = window._rtmidi_internals_get_port_by_number($0, $1);
+    if( port == null)
+      return null;
+    var length = lengthBytesUTF8(port.name) + 1;
+    var ret = _malloc(length);
+    stringToUTF8(port.name, ret, length);
+    return ret;
+  }, portNumber, isInput, &ret );
+  if (ret == nullptr)
+      return "";
+  std::string s = ret;
+  free(ret);
+  return s;
+}
+
+//*********************************************************************//
+//  API: WEB MIDI
+//  Class Definitions: MidiInWeb
+//*********************************************************************//
+
+MidiInWeb::MidiInWeb( const std::string &clientName, unsigned int queueSizeLimit )
+  : MidiInApi( queueSizeLimit )
+{
+  initialize( clientName );
+}
+
+MidiInWeb::~MidiInWeb( void )
+{
+  closePort();
+}
+
+extern "C" void EMSCRIPTEN_KEEPALIVE rtmidi_onMidiMessageProc( MidiInApi::RtMidiInData* data, uint8_t* inputBytes, int32_t length, double domHighResTimeStamp )
+{
+  auto &message = data->message;
+  message.bytes.resize(message.bytes.size() + length);
+  memcpy(message.bytes.data(), inputBytes, length);
+  // FIXME: handle timestamp
+  if ( data->usingCallback ) {
+    RtMidiIn::RtMidiCallback callback = (RtMidiIn::RtMidiCallback) data->userCallback;
+    callback( message.timeStamp, &message.bytes, data->userData );
+  }
+}
+
+void MidiInWeb::openPort( unsigned int portNumber, const std::string &portName )
+{
+  if( !checkWebMidiAvailability() )
+    return;
+  if (open_port_number >= 0)
+    return;
+
+  MAIN_THREAD_EM_ASM( {
+    // In Web MIDI API world, there is no step to open a port, but we have to register the input callback instead.
+    var input = window._rtmidi_internals_get_port_by_number($0, true);
+    input.onmidimessage = function(e) {
+      // In RtMidi world, timestamps are delta time from previous message, while in Web MIDI world
+      // timestamps are relative to window creation time (i.e. kind of absolute time with window "epoch" time).
+      var rtmidiTimestamp = window._rtmidi_internals_latest_message_timestamp == 0.0 ? 0.0 : e.timeStamp - window._rtmidi_internals_latest_message_timestamp;
+      window._rtmidi_internals_latest_message_timestamp = e.timeStamp;
+      Module.ccall( 'rtmidi_onMidiMessageProc', 'void', ['number', 'array', 'number', 'number'], [$1, e.data, e.data.length, rtmidiTimestamp] );
+    };
+  }, portNumber, &inputData_ );
+  open_port_number = portNumber;
+}
+
+void MidiInWeb::openVirtualPort( const std::string &portName )
+{
+
+  errorString_ = "MidiInWeb::openVirtualPort: this function is not implemented for the Web MIDI API!";
+  error( RtMidiError::WARNING, errorString_ );
+
+}
+
+void MidiInWeb::closePort( void )
+{
+  if( open_port_number < 0 )
+    return;
+
+  MAIN_THREAD_EM_ASM( {
+    var input = _rtmidi_internals_get_port_by_number($0, true);
+    if( input == null ) {
+      console.log( "Port #" + $0 + " could not be found.");
+      return;
+    }
+    // unregister event handler
+    input.onmidimessage = null;
+  }, open_port_number );
+  open_port_number = -1;
+}
+
+void MidiInWeb::setClientName( const std::string &clientName )
+{
+  client_name = clientName;
+}
+
+void MidiInWeb::setPortName( const std::string &portName )
+{
+
+  errorString_ = "MidiInWeb::setPortName: this function is not implemented for the Web MIDI API!";
+  error( RtMidiError::WARNING, errorString_ );
+
+}
+
+unsigned int MidiInWeb::getPortCount( void )
+{
+  if( !checkWebMidiAvailability() )
+    return 0;
+  return MAIN_THREAD_EM_ASM_INT( { return _rtmidi_internals_midi_access.inputs.size; } );
+}
+
+std::string MidiInWeb::getPortName( unsigned int portNumber )
+{
+  if( !checkWebMidiAvailability() )
+    return "";
+  return shim->getPortName( portNumber, true );
+}
+
+void MidiInWeb::initialize( const std::string& clientName )
+{
+  ensureShim();
+  setClientName( clientName );
+}
+
+//*********************************************************************//
+//  API: WEB MIDI
+//  Class Definitions: MidiOutWeb
+//*********************************************************************//
+
+MidiOutWeb::MidiOutWeb( const std::string &clientName )
+{
+  initialize( clientName );
+}
+
+MidiOutWeb::~MidiOutWeb( void )
+{
+  closePort();
+}
+
+void MidiOutWeb::openPort( unsigned int portNumber, const std::string &portName )
+{
+  if( !checkWebMidiAvailability() )
+    return;
+  if (open_port_number >= 0)
+    return;
+  // In Web MIDI API world, there is no step to open a port.
+
+  open_port_number = portNumber;
+}
+
+void MidiOutWeb::openVirtualPort( const std::string &portName )
+{
+
+  errorString_ = "MidiOutWeb::openVirtualPort: this function is not implemented for the Web MIDI API!";
+  error( RtMidiError::WARNING, errorString_ );
+
+}
+
+void MidiOutWeb::closePort( void )
+{
+  // there is really nothing to do for output at JS side.
+  open_port_number = -1;
+}
+
+void MidiOutWeb::setClientName( const std::string &clientName )
+{
+  client_name = clientName;
+}
+
+void MidiOutWeb::setPortName( const std::string &portName )
+{
+
+  errorString_ = "MidiOutWeb::setPortName: this function is not implemented for the Web MIDI API!";
+  error( RtMidiError::WARNING, errorString_ );
+
+}
+
+unsigned int MidiOutWeb::getPortCount( void )
+{
+  if( !checkWebMidiAvailability() )
+    return 0;
+  return MAIN_THREAD_EM_ASM_INT( { return _rtmidi_internals_midi_access.outputs.size; } );
+}
+
+std::string MidiOutWeb::getPortName( unsigned int portNumber )
+{
+  if( !checkWebMidiAvailability() )
+    return "";
+  return shim->getPortName( portNumber, false );
+}
+
+void MidiOutWeb::sendMessage( const unsigned char *message, size_t size )
+{
+  if( open_port_number < 0 )
+    return;
+
+  MAIN_THREAD_EM_ASM( {
+    var output = _rtmidi_internals_get_port_by_number( $0, false );
+    if( output == null ) {
+      console.log( "Port #" + $0 + " could not be found.");
+      return;
+    }
+    var buf = new ArrayBuffer ($2);
+    var msg = new Uint8Array( buf );
+    msg.set( new Uint8Array( Module.HEAPU8.buffer.slice( $1, $1 + $2 ) ) );
+    output.send( msg );
+  }, open_port_number, message, size );
+}
+
+void MidiOutWeb::initialize( const std::string& clientName )
+{
+  if ( shim.get() != nullptr )
+    return;
+  shim.reset( new WebMidiAccessShim() );
+  setClientName( clientName );
+}
+
+#endif  // __WEB_MIDI_API__
```

### Comparing `python-rtmidi-1.4.9/src/rtmidi/RtMidi.h` & `python-rtmidi-1.5.0/src/rtmidi/RtMidi.h`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     This class implements some common functionality for the realtime
     MIDI input/output subclasses RtMidiIn and RtMidiOut.
 
     RtMidi GitHub site: https://github.com/thestk/rtmidi
     RtMidi WWW site: http://www.music.mcgill.ca/~gary/rtmidi/
 
     RtMidi: realtime MIDI i/o C++ classes
-    Copyright (c) 2003-2019 Gary P. Scavone
+    Copyright (c) 2003-2021 Gary P. Scavone
 
     Permission is hereby granted, free of charge, to any person
     obtaining a copy of this software and associated documentation files
     (the "Software"), to deal in the Software without restriction,
     including without limitation the rights to use, copy, modify, merge,
     publish, distribute, sublicense, and/or sell copies of the Software,
     and to permit persons to whom the Software is furnished to do so,
@@ -54,15 +54,15 @@
   #if __GNUC__ >= 4
     #define RTMIDI_DLL_PUBLIC __attribute__( (visibility( "default" )) )
   #else
     #define RTMIDI_DLL_PUBLIC
   #endif
 #endif
 
-#define RTMIDI_VERSION "4.0.0"
+#define RTMIDI_VERSION "5.0.0"
 
 #include <exception>
 #include <iostream>
 #include <string>
 #include <vector>
 
 
@@ -129,22 +129,25 @@
 typedef void (*RtMidiErrorCallback)( RtMidiError::Type type, const std::string &errorText, void *userData );
 
 class MidiApi;
 
 class RTMIDI_DLL_PUBLIC RtMidi
 {
  public:
+
+     RtMidi(RtMidi&& other) noexcept;
   //! MIDI API specifier arguments.
   enum Api {
     UNSPECIFIED,    /*!< Search for a working compiled API. */
     MACOSX_CORE,    /*!< Macintosh OS-X CoreMIDI API. */
     LINUX_ALSA,     /*!< The Advanced Linux Sound Architecture API. */
     UNIX_JACK,      /*!< The JACK Low-Latency MIDI Server API. */
     WINDOWS_MM,     /*!< The Microsoft Multimedia MIDI API. */
     RTMIDI_DUMMY,   /*!< A compilable but non-functional API. */
+    WEB_MIDI_API,   /*!< W3C Web MIDI API. */
     NUM_APIS        /*!< Number of values in this enum. */
   };
 
   //! A static function to determine the current RtMidi version.
   static std::string getVersion( void ) throw();
 
   //! A static function to determine the available compiled MIDI APIs.
@@ -210,14 +213,18 @@
   */
   virtual void setErrorCallback( RtMidiErrorCallback errorCallback = NULL, void *userData = 0 ) = 0;
 
  protected:
   RtMidi();
   virtual ~RtMidi();
   MidiApi *rtapi_;
+
+  /* Make the class non-copyable */
+  RtMidi(RtMidi& other) = delete;
+  RtMidi& operator=(RtMidi& other) = delete;
 };
 
 /**********************************************************************/
 /*! \class RtMidiIn
     \brief A realtime MIDI input class.
 
     This class provides a common, platform-independent API for
@@ -245,15 +252,14 @@
 // make a "logical" API selection.
 //
 // **************************************************************** //
 
 class RTMIDI_DLL_PUBLIC RtMidiIn : public RtMidi
 {
  public:
-
   //! User callback function type definition.
   typedef void (*RtMidiCallback)( double timeStamp, std::vector<unsigned char> *message, void *userData );
 
   //! Default constructor that allows an optional api, client name and queue size.
   /*!
     An exception will be thrown if a MIDI system initialization
     error occurs.  The queue size defines the maximum number of
@@ -271,14 +277,16 @@
                       by the application.
     \param queueSizeLimit An optional size of the MIDI input queue can be specified.
   */
   RtMidiIn( RtMidi::Api api=UNSPECIFIED,
             const std::string& clientName = "RtMidi Input Client",
             unsigned int queueSizeLimit = 100 );
 
+  RtMidiIn(RtMidiIn&& other) noexcept : RtMidi(std::move(other)) { }
+
   //! If a MIDI connection is still open, it will be closed by the destructor.
   ~RtMidiIn ( void ) throw();
 
   //! Returns the MIDI API specifier for the current instance of RtMidiIn.
   RtMidi::Api getCurrentApi( void ) throw();
 
   //! Open a MIDI input connection given by enumeration number.
@@ -368,14 +376,27 @@
   //! Set an error callback function to be invoked when an error has occured.
   /*!
     The callback function will be called whenever an error has occured. It is best
     to set the error callback function before opening a port.
   */
   virtual void setErrorCallback( RtMidiErrorCallback errorCallback = NULL, void *userData = 0 );
 
+  //! Set maximum expected incoming message size.
+  /*!
+    For APIs that require manual buffer management, it can be useful to set the buffer
+    size and buffer count when expecting to receive large SysEx messages.  Note that
+    currently this function has no effect when called after openPort().  The default
+    buffer size is 1024 with a count of 4 buffers, which should be sufficient for most
+    cases; as mentioned, this does not affect all API backends, since most either support
+    dynamically scalable buffers or take care of buffer handling themselves.  It is
+    principally intended for users of the Windows MM backend who must support receiving
+    especially large messages.
+  */
+  virtual void setBufferSize( unsigned int size, unsigned int count );
+
  protected:
   void openMidiApi( RtMidi::Api api, const std::string &clientName, unsigned int queueSizeLimit );
 };
 
 /**********************************************************************/
 /*! \class RtMidiOut
     \brief A realtime MIDI output class.
@@ -400,14 +421,16 @@
     If no API argument is specified and multiple API support has been
     compiled, the default order of use is ALSA, JACK (Linux) and CORE,
     JACK (OS-X).
   */
   RtMidiOut( RtMidi::Api api=UNSPECIFIED,
              const std::string& clientName = "RtMidi Output Client" );
 
+  RtMidiOut(RtMidiOut&& other) noexcept : RtMidi(std::move(other)) { }
+
   //! The destructor closes any open MIDI connections.
   ~RtMidiOut( void ) throw();
 
   //! Returns the MIDI API specifier for the current instance of RtMidiOut.
   RtMidi::Api getCurrentApi( void ) throw();
 
   //! Open a MIDI output connection.
@@ -533,14 +556,15 @@
 
   MidiInApi( unsigned int queueSizeLimit );
   virtual ~MidiInApi( void );
   void setCallback( RtMidiIn::RtMidiCallback callback, void *userData );
   void cancelCallback( void );
   virtual void ignoreTypes( bool midiSysex, bool midiTime, bool midiSense );
   double getMessage( std::vector<unsigned char> *message );
+  virtual void setBufferSize( unsigned int size, unsigned int count );
 
   // A MIDI structure used internally by the class to store incoming
   // messages.  Each message represents one and only one MIDI message.
   struct MidiMessage {
     std::vector<unsigned char> bytes;
 
     //! Time in seconds elapsed since the previous message
@@ -574,19 +598,21 @@
     bool doInput;
     bool firstMessage;
     void *apiData;
     bool usingCallback;
     RtMidiIn::RtMidiCallback userCallback;
     void *userData;
     bool continueSysex;
+    unsigned int bufferSize;
+    unsigned int bufferCount;
 
     // Default constructor.
     RtMidiInData()
       : ignoreFlags(7), doInput(false), firstMessage(true), apiData(0), usingCallback(false),
-        userCallback(0), userData(0), continueSysex(false) {}
+        userCallback(0), userData(0), continueSysex(false), bufferSize(1024), bufferCount(4) {}
   };
 
  protected:
   RtMidiInData inputData_;
 };
 
 class RTMIDI_DLL_PUBLIC MidiOutApi : public MidiApi
@@ -611,30 +637,22 @@
 inline bool RtMidiIn :: isPortOpen() const { return rtapi_->isPortOpen(); }
 inline void RtMidiIn :: setCallback( RtMidiCallback callback, void *userData ) { static_cast<MidiInApi *>(rtapi_)->setCallback( callback, userData ); }
 inline void RtMidiIn :: cancelCallback( void ) { static_cast<MidiInApi *>(rtapi_)->cancelCallback(); }
 inline unsigned int RtMidiIn :: getPortCount( void ) { return rtapi_->getPortCount(); }
 inline std::string RtMidiIn :: getPortName( unsigned int portNumber ) { return rtapi_->getPortName( portNumber ); }
 inline void RtMidiIn :: ignoreTypes( bool midiSysex, bool midiTime, bool midiSense ) { static_cast<MidiInApi *>(rtapi_)->ignoreTypes( midiSysex, midiTime, midiSense ); }
 inline double RtMidiIn :: getMessage( std::vector<unsigned char> *message ) { return static_cast<MidiInApi *>(rtapi_)->getMessage( message ); }
-inline void RtMidiIn :: setErrorCallback( RtMidiErrorCallback errorCallback, void *userData ) { rtapi_->setErrorCallback(errorCallback, userData ); }
+inline void RtMidiIn :: setErrorCallback( RtMidiErrorCallback errorCallback, void *userData ) { rtapi_->setErrorCallback(errorCallback, userData); }
+inline void RtMidiIn :: setBufferSize( unsigned int size, unsigned int count ) { static_cast<MidiInApi *>(rtapi_)->setBufferSize(size, count); }
 
 inline RtMidi::Api RtMidiOut :: getCurrentApi( void ) throw() { return rtapi_->getCurrentApi(); }
 inline void RtMidiOut :: openPort( unsigned int portNumber, const std::string &portName ) { rtapi_->openPort( portNumber, portName ); }
 inline void RtMidiOut :: openVirtualPort( const std::string &portName ) { rtapi_->openVirtualPort( portName ); }
 inline void RtMidiOut :: closePort( void ) { rtapi_->closePort(); }
 inline bool RtMidiOut :: isPortOpen() const { return rtapi_->isPortOpen(); }
 inline unsigned int RtMidiOut :: getPortCount( void ) { return rtapi_->getPortCount(); }
 inline std::string RtMidiOut :: getPortName( unsigned int portNumber ) { return rtapi_->getPortName( portNumber ); }
 inline void RtMidiOut :: sendMessage( const std::vector<unsigned char> *message ) { static_cast<MidiOutApi *>(rtapi_)->sendMessage( &message->at(0), message->size() ); }
 inline void RtMidiOut :: sendMessage( const unsigned char *message, size_t size ) { static_cast<MidiOutApi *>(rtapi_)->sendMessage( message, size ); }
 inline void RtMidiOut :: setErrorCallback( RtMidiErrorCallback errorCallback, void *userData ) { rtapi_->setErrorCallback(errorCallback, userData ); }
 
-#if defined(__APPLE__) || defined(__MACOSX_CORE__)
-
-#include <CoreMIDI/CoreMIDI.h>
-
-void RtMidi_setCoreMidiClientSingleton(MIDIClientRef client);
-void RtMidi_disposeCoreMidiClientSingleton();
-
-#endif /* __APPLE__ */
-
 #endif
```

### Comparing `python-rtmidi-1.4.9/tests/test_delete.py` & `python-rtmidi-1.5.0/tests/test_delete.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/tests/test_errorcallback.py` & `python-rtmidi-1.5.0/tests/test_errorcallback.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/tests/test_errors.py` & `python-rtmidi-1.5.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `python-rtmidi-1.4.9/tests/test_rtmidi.py` & `python-rtmidi-1.5.0/tests/test_rtmidi.py`

 * *Files identical despite different names*

