# Comparing `tmp/unassigner-0.0.3.tar.gz` & `tmp/unassigner-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unassigner-0.0.3.tar", last modified: Wed Apr 17 19:38:51 2019, max compression
+gzip compressed data, was "unassigner-0.0.5.tar", last modified: Tue May 23 19:19:24 2023, max compression
```

## Comparing `unassigner-0.0.3.tar` & `unassigner-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,36 @@
-drwxr-xr-x   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)        0 2019-04-17 19:38:51.000000 unassigner-0.0.3/
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     4202 2019-04-17 19:38:51.000000 unassigner-0.0.3/PKG-INFO
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     2946 2019-04-17 19:30:20.000000 unassigner-0.0.3/README.md
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)       38 2019-04-17 19:38:51.000000 unassigner-0.0.3/setup.cfg
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     1237 2019-04-17 19:35:53.000000 unassigner-0.0.3/setup.py
-drwxr-xr-x   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)        0 2019-04-17 19:38:51.000000 unassigner-0.0.3/unassigner/
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)        1 2015-11-11 15:18:51.000000 unassigner-0.0.3/unassigner/__init__.py
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     5651 2019-04-17 16:50:16.000000 unassigner-0.0.3/unassigner/algorithm.py
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     7645 2019-04-17 16:47:47.000000 unassigner-0.0.3/unassigner/align.py
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     6857 2019-04-12 20:36:52.000000 unassigner-0.0.3/unassigner/alignment.py
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     4443 2019-04-17 16:46:29.000000 unassigner-0.0.3/unassigner/command.py
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     3603 2019-04-17 16:17:40.000000 unassigner-0.0.3/unassigner/download.py
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     1958 2019-04-17 12:13:06.000000 unassigner-0.0.3/unassigner/find.py
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     1945 2019-04-12 20:36:52.000000 unassigner-0.0.3/unassigner/parse.py
--rwxr-xr-x   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     2661 2019-04-17 16:51:20.000000 unassigner-0.0.3/unassigner/prepare_strain_data.py
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)    14323 2019-04-17 12:13:35.000000 unassigner-0.0.3/unassigner/trim.py
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)      494 2019-04-17 12:13:44.000000 unassigner-0.0.3/unassigner/unassignment_probability.py
-drwxr-xr-x   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)        0 2019-04-17 19:38:51.000000 unassigner-0.0.3/unassigner.egg-info/
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)     4202 2019-04-17 19:38:51.000000 unassigner-0.0.3/unassigner.egg-info/PKG-INFO
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)      491 2019-04-17 19:38:51.000000 unassigner-0.0.3/unassigner.egg-info/SOURCES.txt
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)        1 2019-04-17 19:38:51.000000 unassigner-0.0.3/unassigner.egg-info/dependency_links.txt
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)       88 2019-04-17 19:38:51.000000 unassigner-0.0.3/unassigner.egg-info/entry_points.txt
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)       16 2019-04-17 19:38:51.000000 unassigner-0.0.3/unassigner.egg-info/requires.txt
--rw-r--r--   0 bittingerk (790488037) CHOP-EDU\Domain Users (1768498755)       11 2019-04-17 19:38:51.000000 unassigner-0.0.3/unassigner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:19:24.073719 unassigner-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-23 19:19:24.073719 unassigner-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4301 2023-05-23 19:19:13.000000 unassigner-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 19:19:24.073719 unassigner-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-23 19:19:13.000000 unassigner-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:19:24.073719 unassigner-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4650 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_aligned.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_ani.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      171 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_mismatch_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-23 19:19:13.000000 unassigner-0.0.5/tests/test_trim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:19:24.073719 unassigner-0.0.5/unassigner/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11611 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8430 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/ani.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5969 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7543 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/mismatch_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2856 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/prepare_strain_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14782 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-23 19:19:13.000000 unassigner-0.0.5/unassigner/unassignment_probability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 19:19:24.073719 unassigner-0.0.5/unassigner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 19:19:24.000000 unassigner-0.0.5/unassigner.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `unassigner-0.0.3/unassigner/align.py` & `unassigner-0.0.5/unassigner/align.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 import abc
+import os.path
 import subprocess
 import tempfile
 from Bio import pairwise2
 
 from unassigner.parse import write_fasta, load_fasta, parse_fasta
 from unassigner.alignment import AlignedPair
 
 BLAST_FMT = (
     "qseqid sseqid pident length mismatch gapopen "
-    "qstart qend sstart send qlen slen qseq sseq")
+    "qstart qend sstart send qlen slen qseq sseq"
+)
 BLAST_FIELDS = BLAST_FMT.split()
 BLAST_FIELD_TYPES = [
-    str, str, float, int, int, int,
-    int, int, int, int, int, int, str, str]
+    str,
+    str,
+    float,
+    int,
+    int,
+    int,
+    int,
+    int,
+    int,
+    int,
+    int,
+    int,
+    str,
+    str,
+]
 
-# TODO: Need a BlastFilter to collect multiple hits and get the best one
 
 class Aligner(abc.ABC):
     def __init__(self, ref_seqs_fp):
         self.ref_seqs_fp = ref_seqs_fp
 
     def search(self, seqs, input_fp=None, output_fp=None, **kwargs):
         if input_fp is None:
@@ -37,181 +51,226 @@
         self._call(input_fp, self.ref_seqs_fp, output_fp, **kwargs)
 
         with open(output_fp) as f:
             for hit in self._parse(f):
                 yield hit
 
     @classmethod
-    def _parse(self, f):
+    def _parse(self, f, convert_types=True):
         """Parse a BLAST output file."""
         for line in f:
             line = line.strip()
             if line.startswith("#"):
                 continue
             vals = line.split("\t")
-            vals = [fn(v) for fn, v in zip(BLAST_FIELD_TYPES, vals)]
+            if convert_types:
+                vals = [fn(v) for fn, v in zip(BLAST_FIELD_TYPES, vals)]
             yield dict(zip(BLAST_FIELDS, vals))
 
 
 class VsearchAligner(Aligner):
+    @property
+    def ref_seqs_udb_fp(self):
+        base_fp, _ = os.path.splitext(self.ref_seqs_fp)
+        return base_fp + ".udb"
+
+    def make_reference_udb(self):
+        if os.path.exists(self.ref_seqs_udb_fp):
+            return
+        args = [
+            "vsearch",
+            "--makeudb_usearch",
+            self.ref_seqs_fp,
+            "--output",
+            self.ref_seqs_udb_fp,
+        ]
+        return subprocess.check_call(args)
+
     @staticmethod
     def _index(fasta_fp):
         pass
 
-    def _call(self, query_fp, database_fp, output_fp, min_id = 0.5, **kwargs):
+    def _call(self, query_fp, database_fp, output_fp, min_id=0.5, **kwargs):
         """Call the VSEARCH program.
 
         --id is a required argument to run the program. We expose the
         argument here as min_id.
         """
+        if not os.path.exists(self.ref_seqs_udb_fp):
+            self.make_reference_udb()
         args = [
-            "vsearch", "--usearch_global", query_fp,
-            "--db", database_fp,
-            "--iddef", "2",
-            "--id", str(min_id),
-            "--userout", output_fp,
+            "vsearch",
+            "--usearch_global",
+            query_fp,
+            "--db",
+            self.ref_seqs_udb_fp,
+            "--iddef",
+            "2",
+            "--id",
+            str(min_id),
+            "--userout",
+            output_fp,
             "--userfields",
-            "query+target+id2+alnlen+mism+gaps+qilo+qihi+tilo+tihi+qs+ts+qrow+trow"
-            ]
+            "query+target+id2+alnlen+mism+gaps+qilo+qihi+tilo+tihi+qs+ts+qrow+trow",
+        ]
         for arg, val in kwargs.items():
             arg = "--" + arg
             if val is None:
                 args.append(arg)
             else:
                 args += [arg, str(val)]
         subprocess.check_call(args, stderr=subprocess.DEVNULL)
 
 
 class BlastAligner(Aligner):
     @staticmethod
     def _index(fasta_fp):
-        return subprocess.check_call([
-            "makeblastdb",
-            "-dbtype", "nucl",
-            "-in", fasta_fp,
-            ], stdout=subprocess.DEVNULL)
+        return subprocess.check_call(
+            [
+                "makeblastdb",
+                "-dbtype",
+                "nucl",
+                "-in",
+                fasta_fp,
+            ],
+            stdout=subprocess.DEVNULL,
+        )
 
     def _call(self, query_fp, database_fp, output_fp, **kwargs):
         """Call the BLAST program."""
         args = [
             "blastn",
-            "-evalue", "1e-5",
-            "-outfmt", "6 " + BLAST_FMT,
-            ]
+            "-evalue",
+            "1e-5",
+            "-outfmt",
+            "6 " + BLAST_FMT,
+        ]
         for arg, val in kwargs.items():
             arg = "-" + arg
             if val is None:
                 args.append(arg)
             else:
                 args += [arg, str(val)]
         args += [
-            "-query", query_fp,
-            "-db", database_fp,
-            "-out", output_fp,
-            ]
+            "-query",
+            query_fp,
+            "-db",
+            database_fp,
+            "-out",
+            output_fp,
+        ]
         subprocess.check_call(args)
 
+
 class HitExtender:
     def __init__(self, query_seqs, ref_seqs):
         self.query_seqs = dict(query_seqs)
         self.ref_seqs = dict(ref_seqs)
 
     def extend_hit(self, hit):
         # Handle the simple case where the local alignment covers both
         # sequences completely
         if self._is_global(hit):
             return AlignedPair(
-                (hit['qseqid'], hit['qseq']),
-                (hit['sseqid'], hit['sseq']))
+                (hit["qseqid"], hit["qseq"]), (hit["sseqid"], hit["sseq"])
+            )
 
         # We are going to need some repair or realignment.
-        qseq = self.query_seqs[hit['qseqid']]
-        assert(len(qseq) == hit['qlen'])
-        sseq = self.ref_seqs[hit['sseqid']]
-        assert(len(sseq) == hit['slen'])
+        qseq = self.query_seqs[hit["qseqid"]]
+        assert len(qseq) == hit["qlen"]
+        sseq = self.ref_seqs[hit["sseqid"]]
+        assert len(sseq) == hit["slen"]
 
         if self._needs_realignment(hit):
             aligned_qseq, aligned_sseq = align_semiglobal(qseq, sseq)
             return AlignedPair(
-                (hit['qseqid'], aligned_qseq),
-                (hit['sseqid'], aligned_sseq))
+                (hit["qseqid"], aligned_qseq), (hit["sseqid"], aligned_sseq)
+            )
 
         qleft, sleft = self._add_endgaps_left(hit, qseq, sseq)
         qright, sright = self._add_endgaps_right(hit, qseq, sseq)
-        aligned_qseq = qleft + hit['qseq'] + qright
-        aligned_sseq = sleft + hit['sseq'] + sright
-        return AlignedPair(
-                (hit['qseqid'], aligned_qseq),
-                (hit['sseqid'], aligned_sseq))
+        aligned_qseq = qleft + hit["qseq"] + qright
+        aligned_sseq = sleft + hit["sseq"] + sright
+        return AlignedPair((hit["qseqid"], aligned_qseq), (hit["sseqid"], aligned_sseq))
 
     @staticmethod
     def _is_global(hit):
         return (
-            (hit['qstart'] == 1) and \
-            (hit['sstart'] == 1) and \
-            (hit['qend'] == hit['qlen']) and \
-            (hit['send'] == hit['slen']))
+            (hit["qstart"] == 1)
+            and (hit["sstart"] == 1)
+            and (hit["qend"] == hit["qlen"])
+            and (hit["send"] == hit["slen"])
+        )
 
     @staticmethod
     def _needs_realignment(hit):
-        more_to_the_left = (hit['qstart'] > 1) and \
-                           (hit['sstart'] > 1)
-        more_to_the_right = (hit['qend'] < hit['qlen']) and \
-                            (hit['send'] < hit['slen'])
-        return (more_to_the_left or more_to_the_right)
+        more_to_the_left = (hit["qstart"] > 1) and (hit["sstart"] > 1)
+        more_to_the_right = (hit["qend"] < hit["qlen"]) and (hit["send"] < hit["slen"])
+        return more_to_the_left or more_to_the_right
 
     @staticmethod
     def _add_endgaps_left(hit, qseq, sseq):
         # No repair needed
-        if (hit['qstart'] == 1) and (hit['sstart'] == 1):
+        if (hit["qstart"] == 1) and (hit["sstart"] == 1):
             return ("", "")
         # Query hanging off to the left
-        if (hit['qstart'] > 1) and (hit['sstart'] == 1):
-            endgap_len = hit['qstart'] - 1
+        if (hit["qstart"] > 1) and (hit["sstart"] == 1):
+            endgap_len = hit["qstart"] - 1
             return (qseq[:endgap_len], "-" * endgap_len)
         # Subject hanging off to the left
-        if (hit['qstart'] == 1) and (hit['sstart'] > 1):
-            endgap_len = hit['sstart'] - 1
+        if (hit["qstart"] == 1) and (hit["sstart"] > 1):
+            endgap_len = hit["sstart"] - 1
             return ("-" * endgap_len, sseq[:endgap_len])
         # Anything not meeting these conditions is bad
-        if (hit['qstart'] > 1) and (hit['sstart'] > 1):
+        if (hit["qstart"] > 1) and (hit["sstart"] > 1):
             raise ValueError("Unaligned sequence on left")
         raise ValueError("Query or subject start position less than 1")
 
     @staticmethod
     def _add_endgaps_right(hit, qseq, sseq):
         # No repair needed
-        if (hit['qend'] == hit['qlen']) and (hit['send'] == hit['slen']):
+        if (hit["qend"] == hit["qlen"]) and (hit["send"] == hit["slen"]):
             return ("", "")
         # Query hanging off to the right
-        if (hit['qend'] < hit['qlen']) and (hit['send'] == hit['slen']):
-            endgap_len = hit['qlen'] - hit['qend']
+        if (hit["qend"] < hit["qlen"]) and (hit["send"] == hit["slen"]):
+            endgap_len = hit["qlen"] - hit["qend"]
             return (qseq[-endgap_len:], "-" * endgap_len)
         # Subject hanging off to the right
-        if (hit['qend'] == hit['qlen']) and (hit['send'] < hit['slen']):
-            endgap_len = hit['slen'] - hit['send']
+        if (hit["qend"] == hit["qlen"]) and (hit["send"] < hit["slen"]):
+            endgap_len = hit["slen"] - hit["send"]
             return ("-" * endgap_len, sseq[-endgap_len:])
         # Anything not meeting these conditions is bad
-        if (hit['qend'] < hit['qlen']) and (hit['send'] < hit['qlen']):
+        if (hit["qend"] < hit["qlen"]) and (hit["send"] < hit["qlen"]):
             raise ValueError("Unaligned sequence on right")
         raise ValueError("Query or subject end position greater than length")
 
     def _get_subject_seq(self, subject_id):
         subject_outfile = tempfile.NamedTemporaryFile()
         subject_outfile_fp = subject_outfile.name
-        args = ["blastdbcmd",
-                "-db", self.db,
-                "-entry", subject_id,
-                "-out", subject_outfile_fp
+        args = [
+            "blastdbcmd",
+            "-db",
+            self.db,
+            "-entry",
+            subject_id,
+            "-out",
+            subject_outfile_fp,
         ]
         subprocess.check_call(args)
         with open(subject_outfile_fp) as f:
             return list(parse_fasta(f, trim_desc=True))[0][1]
 
+
 def align_semiglobal(qseq, sseq):
     alignment = pairwise2.align.globalms(
-        sseq, qseq,
-        5, -4, -10, -0.5, #match, mismatch, gapopen, gapextend
-        penalize_end_gaps=False, one_alignment_only=True)
+        sseq,
+        qseq,
+        5,
+        -4,
+        -10,
+        -0.5,  # match, mismatch, gapopen, gapextend
+        penalize_end_gaps=False,
+        one_alignment_only=True,
+    )
     subj_seq = alignment[0][0]
     query_seq = alignment[0][1]
     return query_seq, subj_seq
```

### Comparing `unassigner-0.0.3/unassigner/alignment.py` & `unassigner-0.0.5/unassigner/alignment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 import itertools
 import operator
 
+
 class AlignedPair(object):
     def __init__(self, qseq, sseq):
         self.query_id, self.query_seq = qseq
         self.subject_id, self.subject_seq = sseq
-        assert(len(self.query_seq) == len(self.subject_seq))
+        assert len(self.query_seq) == len(self.subject_seq)
+
+    def __eq__(self, other):
+        self_vals = (self.query_id, self.query_seq, self.subject_id, self.subject_seq)
+        other_vals = (
+            other.query_id,
+            other.query_seq,
+            other.subject_id,
+            other.subject_seq,
+        )
+        return self_vals == other_vals
 
     @property
     def alignment_len(self):
         return len(self.query_seq)
 
     @property
     def query_len(self):
@@ -26,166 +37,180 @@
     @property
     def unaligned_subject_seq(self):
         return self.subject_seq.replace("-", "")
 
     def count_matches(self):
         return sum(q == s for q, s in zip(self.query_seq, self.subject_seq))
 
+    @property
+    def percent_id(self):
+        return self.count_matches() / self.query_len
+
+    def trim_endgaps(self):
+        return AlignedRegion.without_endgaps(self).trim_ends()
+
+
 class AlignedRegion:
+    """Specify and extract regions of a pairwise sequence alignment"""
+
     def __init__(self, alignment, start_idx, end_idx):
-        assert(start_idx >= 0)
-        assert(start_idx <= alignment.alignment_len)
-        assert(end_idx >= 0)
-        assert(end_idx <= alignment.alignment_len)
-        assert(start_idx <= end_idx)
+        assert start_idx >= 0
+        assert start_idx <= alignment.alignment_len
+        assert end_idx >= 0
+        assert end_idx <= alignment.alignment_len
+        assert start_idx <= end_idx
         self.alignment = alignment
         self.start_idx = start_idx
         self.end_idx = end_idx
 
     def trim_ends(self):
-        qseq = self.alignment.query_seq[self.start_idx:self.end_idx]
-        sseq = self.alignment.subject_seq[self.start_idx:self.end_idx]
+        qseq = self.alignment.query_seq[self.start_idx : self.end_idx]
+        sseq = self.alignment.subject_seq[self.start_idx : self.end_idx]
         return AlignedPair(
-            (self.alignment.query_id, qseq),
-            (self.alignment.subject_id, sseq))
+            (self.alignment.query_id, qseq), (self.alignment.subject_id, sseq)
+        )
 
     def trim_left(self, include_region=False):
         if include_region:
             idx = self.start_idx
         else:
             idx = self.end_idx
         qseq = self.alignment.query_seq[idx:]
         sseq = self.alignment.subject_seq[idx:]
         return AlignedPair(
-            (self.alignment.query_id, qseq),
-            (self.alignment.subject_id, sseq))
+            (self.alignment.query_id, qseq), (self.alignment.subject_id, sseq)
+        )
 
     def trim_right(self, include_region=False):
         if include_region:
             idx = self.end_idx
         else:
             idx = self.start_idx
         qseq = self.alignment.query_seq[:idx]
         sseq = self.alignment.subject_seq[:idx]
         return AlignedPair(
-            (self.alignment.query_id, qseq),
-            (self.alignment.subject_id, sseq))
+            (self.alignment.query_id, qseq), (self.alignment.subject_id, sseq)
+        )
 
     def in_alignment(self):
         return (self.start_idx, self.end_idx)
 
     def in_subject(self):
-        return in_aligned_seq(
-            self.alignment.subject_seq, self.start_idx, self.end_idx)
+        return in_aligned_seq(self.alignment.subject_seq, self.start_idx, self.end_idx)
 
     def in_query(self):
-        return in_aligned_seq(
-            self.alignment.query_seq, self.start_idx, self.end_idx)
+        return in_aligned_seq(self.alignment.query_seq, self.start_idx, self.end_idx)
 
     def subject_offset(self):
         qstart, qend = self.in_subject()
         qlen = self.alignment.subject_len
         if (qstart == 0) and (qend == 0):
             # Subject is off to right side, offset is positive
-            subject_right = self.alignment.subject_seq[self.end_idx:]
+            subject_right = self.alignment.subject_seq[self.end_idx :]
             return count_endgaps(subject_right)
         if (qstart == qlen) and (qend == qlen):
             # Subject is off to left side, offset is negative
-            subject_left = self.alignment.subject_seq[:self.start_idx]
+            subject_left = self.alignment.subject_seq[: self.start_idx]
             return -count_endgaps(subject_left, reverse=True)
         return 0
 
     def query_offset(self):
         qstart, qend = self.in_query()
         qlen = self.alignment.query_len
         if (qstart == 0) and (qend == 0):
             # Query is off to right side, offset is positive
-            query_right = self.alignment.query_seq[self.end_idx:]
+            query_right = self.alignment.query_seq[self.end_idx :]
             return count_endgaps(query_right)
         if (qstart == qlen) and (qend == qlen):
             # Query is off to left side, offset is negative
-            query_left = self.alignment.query_seq[:self.start_idx]
+            query_left = self.alignment.query_seq[: self.start_idx]
             return -count_endgaps(query_left, reverse=True)
         return 0
 
     @classmethod
     def without_endgaps(cls, a):
-        left_endgaps = max(
-            count_endgaps(a.query_seq),
-            count_endgaps(a.subject_seq))
+        """Create a new region with no endgaps"""
+        left_endgaps = max(count_endgaps(a.query_seq), count_endgaps(a.subject_seq))
         right_endgaps = max(
             count_endgaps(a.query_seq, reverse=True),
-            count_endgaps(a.subject_seq, reverse=True))
+            count_endgaps(a.subject_seq, reverse=True),
+        )
         start_idx = left_endgaps
         end_idx = a.alignment_len - right_endgaps
         return cls(a, start_idx, end_idx)
 
     @classmethod
     def from_subject(cls, a, subject_start_idx=0, subject_end_idx=None):
+        """Create a new region using coordinates in subject sequence"""
         if subject_end_idx is None:
             subject_end_idx = a.subject_len
-        assert(subject_start_idx >= 0)
-        assert(subject_start_idx <= a.subject_len)
-        assert(subject_end_idx >= 0)
-        assert(subject_end_idx <= a.subject_len)
-        assert(subject_start_idx <= subject_end_idx)
+        assert subject_start_idx >= 0
+        assert subject_start_idx <= a.subject_len
+        assert subject_end_idx >= 0
+        assert subject_end_idx <= a.subject_len
+        assert subject_start_idx <= subject_end_idx
         start_idx = aligned_start_idx(a.subject_seq, subject_start_idx)
         end_idx = aligned_end_idx(a.subject_seq, subject_end_idx)
         return cls(a, start_idx, end_idx)
 
     @classmethod
     def from_query(cls, a, query_start_idx=0, query_end_idx=None):
+        """Create a new region using coordinates in query sequence"""
         if query_end_idx is None:
             query_end_idx = a.query_len
-        assert(query_start_idx >= 0)
-        assert(query_start_idx <= a.query_len)
-        assert(query_end_idx >= 0)
-        assert(query_end_idx <= a.query_len)
-        assert(query_start_idx <= query_end_idx)
+        assert query_start_idx >= 0
+        assert query_start_idx <= a.query_len
+        assert query_end_idx >= 0
+        assert query_end_idx <= a.query_len
+        assert query_start_idx <= query_end_idx
         start_idx = aligned_start_idx(a.query_seq, query_start_idx)
         end_idx = aligned_end_idx(a.query_seq, query_end_idx)
         return cls(a, start_idx, end_idx)
 
 
 def in_aligned_seq(seq, start_idx, end_idx):
     seq_start = seq[:start_idx]
     seq_start_idx = start_idx - seq_start.count("-")
     seq_end = seq[:end_idx]
     seq_end_idx = end_idx - seq_end.count("-")
     return seq_start_idx, seq_end_idx
 
+
 def aligned_end_idx(seq, end_idx):
     # Work in reverse mode, find the complimentary start_idx
     ungapped_seq_len = len(seq) - seq.count("-")
     rev_start_idx = ungapped_seq_len - end_idx
     rev_seq = seq[::-1]
     rev_alignment_start_idx = aligned_start_idx(rev_seq, rev_start_idx)
     return len(seq) - rev_alignment_start_idx
 
+
 def aligned_start_idx(seq, start_idx):
     ungapped_seq_len = len(seq) - seq.count("-")
     # Special case: start_idx is equal to ungapped sequence length
     # We will never count enough bases to reach the start_idx
     # Reverse the sequence and find the start position for index 0,
     # then subtract from the alignment length to get the forward-facing
     # index after the last base.
     if start_idx == ungapped_seq_len:
         rev_seq = seq[::-1]
         rev_alignment_start_idx = aligned_start_idx(rev_seq, 0)
         return len(seq) - rev_alignment_start_idx
     start_idxs = [n - 1 for n in cumulative_bases(seq)]
     return start_idxs.index(start_idx)
 
+
 def cumulative_bases(seq):
     return itertools.accumulate(int(b != "-") for b in seq)
 
+
 def iter_len(xs):
     n = 0
     for _ in xs:
         n += 1
     return n
 
-def count_endgaps(seq, reverse = False):
+
+def count_endgaps(seq, reverse=False):
     if reverse:
         seq = reversed(seq)
     return iter_len(itertools.takewhile(lambda x: x == "-", seq))
-
```

### Comparing `unassigner-0.0.3/unassigner/command.py` & `unassigner-0.0.5/unassigner/command.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,98 @@
 import argparse
+import datetime
+import gzip
+import logging
 import os
 
 from unassigner.algorithm import (
-    UnassignAligner, FileAligner, ThresholdAlgorithm,
+    UnassignAligner,
+    FileAligner,
+    UnassignerApp,
+    VariableMismatchRate,
 )
 from unassigner.parse import parse_fasta, parse_species_names
 from unassigner.prepare_strain_data import download_type_strain_data
 
+
 def main(argv=None):
     p = argparse.ArgumentParser()
-    p.add_argument("query_fasta", type=argparse.FileType("r"),
-        help="Query sequences FASTA file")
-    p.add_argument("--output_dir",
+    p.add_argument(
+        "query_fasta", type=argparse.FileType("r"), help="Query sequences FASTA file"
+    )
+    p.add_argument(
+        "--output_dir",
         help=(
             "Output directory (default: basename of query sequences FASTA "
-            "file, plus '_unassigned')"))
-    p.add_argument("--type_strain_fasta", default="unassigner_species.fasta",
+            "file, plus '_unassigned')"
+        ),
+    )
+    p.add_argument(
+        "--type_strain_fasta",
+        default="unassigner_species.fasta",
         help=(
             "Type strain sequences FASTA file (default: %(default)s). "
             "If the default file is not found, sequences are downloaded "
-            "and re-formatted automatically."))
-    p.add_argument("--num_cpus", type=int,
+            "and re-formatted automatically."
+        ),
+    )
+    p.add_argument(
+        "--threshold",
+        type=float,
+        help=(
+            "Sequence identity threshold for ruling out species-level "
+            "compatibility. Default value is 0.975 for the standard "
+            "algorithm and 0.991 for the soft threshold algorithm."
+        ),
+    )
+    p.add_argument(
+        "--ref_mismatch_positions",
+        help=(
+            "File of mismatch positions in reference database. The file may "
+            "be compressed in gzip format."
+        ),
+    )
+    p.add_argument(
+        "--num_cpus",
+        type=int,
         help=(
             "Number of CPUs to use during sequence aligment (default: "
-            "use all the CPUs)"))
-    p.add_argument("--verbose", action="store_true",
-        help= "Activate verbose mode.")
+            "use all the CPUs)"
+        ),
+    )
+    p.add_argument(
+        "--soft_threshold", action="store_true", help="Use soft threshold algorithm."
+    )
+    p.add_argument("--verbose", action="store_true", help="Activate verbose mode.")
     args = p.parse_args(argv)
 
+    if args.threshold is None:
+        if args.soft_threshold:
+            min_id = 0.991
+        else:
+            min_id = 0.975
+    else:
+        min_id = args.threshold
+
     if args.verbose is True:
-        logging.basicConfig(level=logging.INFO)
+        logging.basicConfig(format="%(levelname)s: %(message)s", level=logging.INFO)
+
+    logging.info(f"Starting at {datetime.datetime.now()}")
 
     query_seqs = list(parse_fasta(args.query_fasta, trim_desc=True))
 
     if args.output_dir is None:
         output_dir = os.path.splitext(args.query_fasta.name)[0] + "_unassigned"
     else:
         output_dir = args.output_dir
 
     # Download type strain files if needed
-    type_strain_fp_is_default = (
-        args.type_strain_fasta == p.get_default("type_strain_fasta"))
+    type_strain_fp_is_default = args.type_strain_fasta == p.get_default(
+        "type_strain_fasta"
+    )
     type_strain_fp_is_missing = not os.path.exists(args.type_strain_fasta)
     if type_strain_fp_is_default and type_strain_fp_is_missing:
         download_type_strain_data()
 
     with open(args.type_strain_fasta) as f:
         species_names = dict(parse_species_names(f))
 
@@ -56,23 +104,37 @@
         a = FileAligner(args.type_strain_fasta, alignment_output_fp)
     else:
         a = UnassignAligner(args.type_strain_fasta)
         a.species_input_fp = alignment_query_fp
         a.species_output_fp = alignment_output_fp
         a.num_cpus = args.num_cpus
 
-    algorithm = ThresholdAlgorithm(a)
-    for query_id, query_results in algorithm.unassign(query_seqs):
+    if args.ref_mismatch_positions:
+        if args.ref_mismatch_positions.endswith(".gz"):
+            mm_db_file = gzip.open(args.ref_mismatch_positions, "rt")
+        else:
+            mm_db_file = open(args.ref_mismatch_positions)
+        VariableMismatchRate.load_database(mm_db_file)
+
+    app = UnassignerApp(
+        a, VariableMismatchRate, min_id=min_id, soft_threshold=args.soft_threshold
+    )
+    for query_id, query_results in app.unassign(query_seqs):
         writer.write_results(query_id, query_results)
 
+    logging.info(f"Finished at {datetime.datetime.now()}")
+
 
 class OutputWriter:
     standard_keys = [
-        "typestrain_id", "region_mismatches", "region_positions",
-        "probability_incompatible"]
+        "typestrain_id",
+        "region_mismatches",
+        "region_positions",
+        "probability_incompatible",
+    ]
 
     def __init__(self, output_dir, species_names):
         self.species_names = species_names
 
         if not os.path.exists(output_dir):
             os.mkdir(output_dir)
         self.output_dir = output_dir
@@ -102,14 +164,16 @@
 
             # Set custom algorithm keys based on the first result
             if self.algorithm_keys is None:
                 self.algorithm_keys = list(result.keys())
                 algorithm_header = ["query_id", "species_name"] + self.algorithm_keys
                 self._write_tsv_line(self.algorithm_file, algorithm_header)
 
-            standard_vals = [query_id, species_name] + \
-                [result[k] for k in self.standard_keys]
+            standard_vals = [query_id, species_name] + [
+                result[k] for k in self.standard_keys
+            ]
             self._write_tsv_line(self.standard_file, standard_vals)
 
-            algorithm_vals = [query_id, species_name] + \
-                [result[k] for k in self.algorithm_keys]
+            algorithm_vals = [query_id, species_name] + [
+                result[k] for k in self.algorithm_keys
+            ]
             self._write_tsv_line(self.algorithm_file, algorithm_vals)
```

### Comparing `unassigner-0.0.3/unassigner/download.py` & `unassigner-0.0.5/unassigner/download.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,95 @@
 import collections
+import logging
 import os
+import shutil
 import subprocess
-import tarfile
+import urllib.request
 
-from unassigner.parse import parse_fasta, parse_greengenes_accessions
+from unassigner.parse import parse_fasta, parse_desc, parse_greengenes_accessions
 
 LTP_METADATA_COLS = [
     "accession",
     "start",
     "stop",
     "unknown",
     "fullname_ltp",
     "type_ltp",
     "hi_tax_ltp",
     "riskgroup_ltp",
     "url_lpsn_ltp",
     "tax_ltp",
     "rel_ltp",
-    "NJ_support_pk4_ltp"
-    ]
-LTP_METADATA_URL = \
-    "https://www.arb-silva.de/fileadmin/silva_databases/living_tree/LTP_release_128/LTPs128_SSU/LTPs128_SSU.csv"
-LTP_SEQS_URL = \
-    "https://www.arb-silva.de/fileadmin/silva_databases/living_tree/LTP_release_128/LTPs128_SSU/LTPs128_SSU_unaligned.fasta"
-GG_SEQS_URL = \
-    "ftp://greengenes.microbio.me/greengenes_release/gg_13_5/gg_13_5.fasta.gz"
-GG_ACCESSIONS_URL = \
+    "NJ_support_pk4_ltp",
+]
+LTP_METADATA_URL = (
+    "https://imedea.uib-csic.es/mmg/ltp/wp-content/uploads/ltp/LTP_06_2022.csv"
+)
+LTP_SEQS_URL = "https://imedea.uib-csic.es/mmg/ltp/wp-content/uploads/ltp/LTP_06_2022_blastdb.fasta"
+GG_SEQS_URL = "ftp://greengenes.microbio.me/greengenes_release/gg_13_5/gg_13_5.fasta.gz"
+GG_ACCESSIONS_URL = (
     "ftp://greengenes.microbio.me/greengenes_release/gg_13_5/gg_13_5_accessions.txt.gz"
+)
 SPECIES_FASTA_FP = "unassigner_species.fasta"
 REFSEQS_FASTA_FP = "refseqs.fasta"
 GG_DUPLICATE_FP = "gg_duplicate_ids.txt"
 
+
 def clean(db_dir):
     fps = [
         url_fp(LTP_METADATA_URL),
         url_fp(LTP_SEQS_URL),
         SPECIES_FASTA_FP,
         gunzip_fp(url_fp(GG_SEQS_URL)),
         gunzip_fp(url_fp(GG_ACCESSIONS_URL)),
         REFSEQS_FASTA_FP,
-        GG_DUPLICATE_FP
-        ]
+        GG_DUPLICATE_FP,
+    ]
     for fp in fps:
         fp_full = os.path.join(db_dir, fp)
         if os.path.exists(fp_full):
             os.remove(fp_full)
 
 
 def url_fp(url):
-    return url.split('/')[-1]
+    return url.split("/")[-1]
 
 
 def gunzip_fp(fp):
     return fp[:-3]
 
 
 def get_url(url, fp):
-    if os.path.exists(fp):
-        os.remove(fp)
-    subprocess.check_call(["wget", "-O", fp, url])
+    logging.info("Downloading {0}".format(url))
+    with urllib.request.urlopen(url) as resp, open(fp, "wb") as f:
+        shutil.copyfileobj(resp, f)
     return fp
 
 
 def process_ltp_seqs(input_fp, output_fp=SPECIES_FASTA_FP):
     if os.path.isdir(output_fp):
         output_fp = os.path.join(output_fp, SPECIES_FASTA_FP)
+    accession_cts = collections.defaultdict(int)
     # Re-format FASTA file
     with open(input_fp) as f_in:
         seqs = parse_fasta(f_in)
         with open(output_fp, "w") as f_out:
             for desc, seq in seqs:
-                vals = desc.split("\t")
-                accession = vals[0]
-                species_name = vals[5]
-                f_out.write(
-                    ">{0}\t{1}\n{2}\n".format(accession, species_name, seq))
+                accession, species_name = parse_desc(desc)
+                if not accession or not species_name:
+                    continue
+                # Some accessions refer to genomes with more than one 16S gene
+                # So accessions can be legitiamtely repeated with distinct gene sequences
+                accession_times_previously_seen = accession_cts[accession]
+                accession_cts[accession] += 1
+                if accession_times_previously_seen > 0:
+                    accession = "{0}_repeat{1}".format(
+                        accession, accession_times_previously_seen
+                    )
+                f_out.write(">{0}\t{1}\n{2}\n".format(accession, species_name, seq))
     return output_fp
 
 
 def process_greengenes_seqs(seqs_fp, accessions_fp, output_fp=REFSEQS_FASTA_FP):
     duplicates_fp = GG_DUPLICATE_FP
     if os.path.isdir(output_fp):
         duplicates_fp = os.path.join(output_fp, duplicates_fp)
```

### Comparing `unassigner-0.0.3/unassigner/find.py` & `unassigner-0.0.5/unassigner/find.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,45 @@
 import argparse
 import sys
 
 from unassigner.parse import parse_fasta, write_fasta
 from unassigner.trim import (
-    CompleteMatcher, PartialMatcher,
-    deambiguate, reverse_complement,
-    )
+    CompleteMatcher,
+    PartialMatcher,
+    deambiguate,
+    reverse_complement,
+)
+
 
 def main(argv=None):
     p = argparse.ArgumentParser()
+    p.add_argument("--input_file", type=argparse.FileType("r"), default=sys.stdin)
+    p.add_argument("--output_file", type=argparse.FileType("w"), default=sys.stdout)
     p.add_argument(
-        "--input_file", type=argparse.FileType("r"), default=sys.stdin)
-    p.add_argument(
-        "--output_file", type=argparse.FileType("w"), default=sys.stdout)
-    p.add_argument(
-        "--unmatched_output_file", type=argparse.FileType("w"),
+        "--unmatched_output_file",
+        type=argparse.FileType("w"),
     )
     p.add_argument("--query", required=True)
     p.add_argument(
-        "--max_mismatch", type=int, default=2,
-        help="Maximum number of mismatches in complete match")
+        "--max_mismatch",
+        type=int,
+        default=2,
+        help="Maximum number of mismatches in complete match",
+    )
     p.add_argument(
-        "--min_partial", type=int, default=5,
-        help="Minimum length of partial sequence match")
+        "--min_partial",
+        type=int,
+        default=5,
+        help="Minimum length of partial sequence match",
+    )
     p.add_argument(
-        "--reverse_complement_query", action="store_true",
-        help="Reverse complement the query seq before search")
+        "--reverse_complement_query",
+        action="store_true",
+        help="Reverse complement the query seq before search",
+    )
 
     args = p.parse_args(argv)
 
     queryset = deambiguate(args.query)
     if args.reverse_complement_query:
         queryset = [reverse_complement(q) for q in queryset]
 
@@ -54,9 +64,7 @@
             else:
                 write_fasta(args.output_file, [(seq_id, seq)])
     else:
         unmatched_pm = unmatched_cm
 
     if args.unmatched_output_file is not None:
         write_fasta(args.unmatched_output_file, unmatched_pm)
-
-
```

### Comparing `unassigner-0.0.3/unassigner/parse.py` & `unassigner-0.0.5/unassigner/parse.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import logging
+import re
 from io import StringIO
 
+
 def parse_species_names(f):
     for desc, seq in parse_fasta(f):
         vals = desc.split("\t", maxsplit=1)
         accession = vals[0]
         if len(vals) == 2:
             species_name = vals[1]
         else:
             species_name = accession
         yield accession, species_name
 
+
 def parse_fasta(f, trim_desc=False):
     """Parse a FASTA format file.
 
     Parameters
     ----------
     f : File object or iterator returning lines in FASTA format.
 
@@ -26,31 +30,45 @@
     Notes
     -----
     This function removes whitespace in the sequence and translates
     "U" to "T", in order to accommodate FASTA files downloaded from
     SILVA and the Living Tree Project.
     """
     f = iter(f)
-    desc = next(f).strip()[1:]
-    if trim_desc:
-        desc = desc.split()[0]
+    try:
+        desc = next(f).strip()[1:]
+        if trim_desc:
+            desc = desc.split()[0]
+    except StopIteration:
+        return
     seq = StringIO()
     for line in f:
         line = line.strip()
         if line.startswith(">"):
             yield desc, seq.getvalue()
             desc = line[1:]
             if trim_desc:
                 desc = desc.split()[0]
             seq = StringIO()
         else:
             seq.write(line.replace(" ", "").replace("U", "T"))
     yield desc, seq.getvalue()
 
 
+def parse_desc(desc):
+    try:
+        accession = re.findall(r"\[accession=(.*?)\]", desc)[0]
+        species_name = re.findall(r"\[organism=(.*?)\]", desc)[0]
+    except IndexError as e:
+        logging.error(f"Couldn't find accession and/or organism identifier in {desc}")
+        logging.error(f"Skipping this sequence...")
+        return None, None
+    return accession, species_name
+
+
 def write_fasta(f, seqs):
     for desc, seq in seqs:
         f.write(">{0}\n{1}\n".format(desc, seq))
 
 
 def load_fasta(filepath, trim_desc=True):
     """Load all sequences from a FASTA file
@@ -70,7 +88,25 @@
 
 def parse_greengenes_accessions(f):
     for line in f:
         if line.startswith("#"):
             continue
         line = line.strip()
         yield line.split("\t")
+
+
+def parse_results(f):
+    float_fields = ["probability_incompatible"]
+    int_fields = ["region_mismatches", "region_positions"]
+    header_line = next(f)
+    header_line = header_line.rstrip()
+    fields = header_line.split("\t")
+    for line in f:
+        line = line.rstrip()
+        vals = line.split("\t")
+        res = dict(zip(fields, vals))
+        for field, val in res.items():
+            if field in float_fields:
+                res[field] = float(val)
+            elif field in int_fields:
+                res[field] = int(val)
+        yield res
```

### Comparing `unassigner-0.0.3/unassigner/prepare_strain_data.py` & `unassigner-0.0.5/unassigner/prepare_strain_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,97 @@
 import argparse
 import sys
 import os
 
 from unassigner.download import (
-    get_url, clean,
-    LTP_METADATA_URL, LTP_SEQS_URL,
-    GG_SEQS_URL, GG_ACCESSIONS_URL,
-    process_ltp_seqs, process_greengenes_seqs,
-    )
+    get_url,
+    clean,
+    LTP_METADATA_URL,
+    LTP_SEQS_URL,
+    GG_SEQS_URL,
+    GG_ACCESSIONS_URL,
+    process_ltp_seqs,
+    process_greengenes_seqs,
+)
 
 
 def use_or_download(optional_fp, url, db_dir):
     if optional_fp is None:
         return get_url(url, os.path.join(db_dir, os.path.basename(url)))
     else:
         return optional_fp
 
 
 def main(argv=None):
     p = argparse.ArgumentParser()
-    p.add_argument("--ltp_metadata_fp", help=(
-        "Filepath for LTP metadata (.csv file) "
-        "[default:download from LTP website]"))
-    p.add_argument("--ltp_seqs_fp", help=(
-        "Filepath for unaligned 16S sequences from LTP (.fasta file) "
-        "[default: download from LTP website]"))
-    p.add_argument("--download_greengenes", action="store_true",
-        help="Download GreenGenes reference files [default: False]")
-    p.add_argument("--greengenes_accessions_fp", help=(
-        "Filepath for table of GreenGenes accession numbers "
-        "(.txt or .txt.gz file) "
-        "[default: download from GreenGenes mirror]"))
-    p.add_argument("--greengenes_seqs_fp", help=(
-        "Filepath for unaligned 16S reference sequences "
-        "(.fasta or .fasta.gz file) "
-        "[default: download from GreenGenes mirror]"))
-    p.add_argument("--clean", action="store_true", help=(
-        "Remove all downloaded and processed files."))
-    p.add_argument("--db-dir", help=(
-        "Filepath to download the files to."))
+    p.add_argument(
+        "--ltp_metadata_fp",
+        help=(
+            "Filepath for LTP metadata (.csv file) "
+            "[default:download from LTP website]"
+        ),
+    )
+    p.add_argument(
+        "--ltp_seqs_fp",
+        help=(
+            "Filepath for unaligned 16S sequences from LTP (.fasta file) "
+            "[default: download from LTP website]"
+        ),
+    )
+    p.add_argument(
+        "--download_greengenes",
+        action="store_true",
+        help="Download GreenGenes reference files [default: False]",
+    )
+    p.add_argument(
+        "--greengenes_accessions_fp",
+        help=(
+            "Filepath for table of GreenGenes accession numbers "
+            "(.txt or .txt.gz file) "
+            "[default: download from GreenGenes mirror]"
+        ),
+    )
+    p.add_argument(
+        "--greengenes_seqs_fp",
+        help=(
+            "Filepath for unaligned 16S reference sequences "
+            "(.fasta or .fasta.gz file) "
+            "[default: download from GreenGenes mirror]"
+        ),
+    )
+    p.add_argument(
+        "--clean",
+        action="store_true",
+        help=("Remove all downloaded and processed files."),
+    )
+    p.add_argument("--db-dir", help=("Filepath to download the files to."))
     args = p.parse_args(argv)
 
     if args.db_dir:
         db_dir = args.db_dir
         if not os.path.exists(args.db_dir) and not args.clean:
             os.mkdir(args.db_dir)
     else:
         db_dir = os.getcwd()
 
     if args.clean is True:
         clean(db_dir)
         sys.exit(0)
 
-    ltp_metadata_fp = use_or_download(
-        args.ltp_metadata_fp, LTP_METADATA_URL, db_dir)
-    ltp_seqs_fp = use_or_download(
-        args.ltp_seqs_fp, LTP_SEQS_URL, db_dir)
+    ltp_metadata_fp = use_or_download(args.ltp_metadata_fp, LTP_METADATA_URL, db_dir)
+    ltp_seqs_fp = use_or_download(args.ltp_seqs_fp, LTP_SEQS_URL, db_dir)
     process_ltp_seqs(ltp_seqs_fp, db_dir)
 
     if args.download_greengenes:
-        gg_seqs_fp = use_or_download(
-            args.greengenes_seqs_fp, GG_SEQS_URL, db_dir)
+        gg_seqs_fp = use_or_download(args.greengenes_seqs_fp, GG_SEQS_URL, db_dir)
         gg_accessions_fp = use_or_download(
-            args.greengenes_accessions_fp, GG_ACCESSIONS_URL, db_dir)
+            args.greengenes_accessions_fp, GG_ACCESSIONS_URL, db_dir
+        )
         process_greengenes_seqs(gg_seqs_fp, gg_accessions_fp, db_dir)
 
+
 def download_type_strain_data(output_dir=None, metadata_fp=None, seqs_fp=None):
     if output_dir is None:
         output_dir = os.getcwd()
     metadata_fp = use_or_download(metadata_fp, LTP_METADATA_URL, output_dir)
     seqs_fp = use_or_download(seqs_fp, LTP_SEQS_URL, output_dir)
     return process_ltp_seqs(seqs_fp, output_dir)
```

### Comparing `unassigner-0.0.3/unassigner/trim.py` & `unassigner-0.0.5/unassigner/trim.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import sys
 import tempfile
 
 from unassigner.parse import parse_fasta, write_fasta
 from unassigner.align import VsearchAligner, HitExtender
 from unassigner.alignment import AlignedRegion
 
+
 class TrimmableSeqs:
     def __init__(self, recs):
         replicate_seqs = collections.defaultdict(list)
         self.descs = dict()
         for desc, seq in recs:
             seq_id = desc.split()[0]
             replicate_seqs[seq].append(seq_id)
@@ -61,15 +62,16 @@
     @classmethod
     def from_fasta(cls, f):
         recs = parse_fasta(f)
         return cls(recs)
 
 
 PrimerMatch = collections.namedtuple(
-    "PrimerMatch", ["start", "end", "offset", "message"])
+    "PrimerMatch", ["start", "end", "offset", "message"]
+)
 
 
 class Matcher(abc.ABC):
     def __init__(self, queryset):
         self.queryset = queryset
 
     # TODO: parallelize this
@@ -92,25 +94,26 @@
 
         # To look for near matches in the reference sequence, we
         # generate the set of qeury sequences with 0, 1, or 2 errors
         # and look for these in the reference.  This is our
         # "mismatched queryset."
         possible_mismatches = range(max_mismatch + 1)
         self.mismatched_queryset = [
-            self._mismatched_queries(n) for n in possible_mismatches]
+            self._mismatched_queries(n) for n in possible_mismatches
+        ]
 
     def _mismatched_queries(self, n_mismatch):
         # The generator is provides a sequence for one-time use, but
         # we need to go through it multiple times.  This function
         # wraps the generator to provide a list.
         return list(self._iter_mismatched_queries(n_mismatch))
 
     def _iter_mismatched_queries(self, n_mismatch):
         # This algorithm is terrible unless the number of mismatches is very small
-        assert(n_mismatch in [0, 1, 2, 3])
+        assert n_mismatch in [0, 1, 2, 3]
         for query in self.queryset:
             idx_sets = itertools.combinations(range(len(query)), n_mismatch)
             for idx_set in idx_sets:
                 # Replace base at each position with a literal "N", to match
                 # ambiguous bases in the reference
                 yield replace_with_n(query, idx_set)
                 # Change to list because strings are immutable
@@ -163,18 +166,18 @@
             if seq.startswith(partial_query):
                 end_idx = len(partial_query)
                 return PrimerMatch(0, end_idx, 0, "Partial")
 
 
 class AlignmentMatcher(Matcher):
     def __init__(
-            self, alignment_dir, min_pct_id=75, min_aligned_frac=0.6,
-            cores=1, suffix="0"):
-        assert(os.path.exists(alignment_dir))
-        assert(os.path.isdir(alignment_dir))
+        self, alignment_dir, min_pct_id=75, min_aligned_frac=0.6, cores=1, suffix="0"
+    ):
+        assert os.path.exists(alignment_dir)
+        assert os.path.isdir(alignment_dir)
         self.alignment_dir = alignment_dir
         self.min_pct_id = min_pct_id
         self.min_aligned_frac = min_aligned_frac
         self.cores = cores
         self.suffix = suffix
 
     def _make_fp(self, filename):
@@ -189,52 +192,57 @@
         query_fp = self._make_fp("query_{0}.fa".format(self.suffix))
         result_fp = self._make_fp("query_{0}.txt".format(self.suffix))
 
         # Search
         with open(subject_fp, "w") as f:
             write_fasta(f, seqs.get_matched_offset0())
         ba = VsearchAligner(subject_fp)
-        search_args = {
-            "min_id": round(self.min_pct_id / 100, 2),
-            "top_hits_only": None}
+        search_args = {"min_id": round(self.min_pct_id / 100, 2), "top_hits_only": None}
         if self.cores > 0:
             search_args["threads"] = self.cores
         hits = ba.search(
-            seqs.get_unmatched_recs(), input_fp=query_fp, output_fp=result_fp,
-            **search_args)
+            seqs.get_unmatched_recs(),
+            input_fp=query_fp,
+            output_fp=result_fp,
+            **search_args
+        )
 
         # Refine
         bext = HitExtender(seqs.get_unmatched_recs(), seqs.get_matched_offset0())
         for hit in hits:
             alignment = bext.extend_hit(hit)
             subject_match = seqs.matches[alignment.subject_id]
             aligned_region = AlignedRegion.from_subject(
-                alignment, subject_match.start, subject_match.end)
+                alignment, subject_match.start, subject_match.end
+            )
             query_start_idx, query_end_idx = aligned_region.in_query()
             query_offset = aligned_region.query_offset()
             matchobj = PrimerMatch(
-                query_start_idx, query_end_idx, query_offset, "Alignment")
+                query_start_idx, query_end_idx, query_offset, "Alignment"
+            )
             yield alignment.query_id, matchobj
 
 
 def partial_seqs(seq, min_length):
     max_start_idx = len(seq) - min_length + 1
     for start_idx in range(1, max_start_idx):
         yield seq[start_idx:]
 
+
 def aligned_frac(hit):
     unaligned_left = min(hit["qstart"], hit["sstart"])
     unaligned_right = min(
         hit["qlen"] - hit["qend"],
         hit["slen"] - hit["send"],
     )
     unaligned = unaligned_left + unaligned_right
     aligned = hit["length"]
     return aligned / (aligned + unaligned)
 
+
 class TrimraggedApp(object):
     def __init__(self, seqs, trim_right, writer, min_trimmed_length):
         self.seqs = seqs
         self.trim_right = trim_right
         self.writer = writer
         self.min_trimmed_length = min_trimmed_length
         self.matchers = []
@@ -271,73 +279,110 @@
     def write_trimmed(self, desc, seq):
         self.trimmed_file.write(">{0}\n{1}\n".format(desc, seq))
 
     def write_stats(self, seq_id, seq, matchobj):
         if matchobj is None:
             self.stats_file.write("{0}\tUnmatched\tNA\tNA\tNA\t\n".format(seq_id))
         else:
-            matched_seq = seq[matchobj.start:matchobj.end]
-            self.stats_file.write("{0}\t{1}\t{2}\t{3}\t{4}\t{5}\n".format(
-                seq_id, matchobj.message, matchobj.start, matchobj.end,
-                matchobj.offset, matched_seq))
+            matched_seq = seq[matchobj.start : matchobj.end]
+            self.stats_file.write(
+                "{0}\t{1}\t{2}\t{3}\t{4}\t{5}\n".format(
+                    seq_id,
+                    matchobj.message,
+                    matchobj.start,
+                    matchobj.end,
+                    matchobj.offset,
+                    matched_seq,
+                )
+            )
 
 
 def trim_left(seq, matchobj):
-    return seq[matchobj.end:]
+    return seq[matchobj.end :]
+
 
 def trim_right(seq, matchobj):
-    return seq[:matchobj.start]
+    return seq[: matchobj.start]
+
 
 def trim_middle(seq, matchobj):
-    return seq[matchobj.start:matchobj.end]
+    return seq[matchobj.start : matchobj.end]
+
 
 def main(argv=None):
-    p = argparse.ArgumentParser()
+    p = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
     p.add_argument("query", help="Query sequence to search and trim")
+    p.add_argument("--input_file", type=argparse.FileType("r"), default=sys.stdin)
     p.add_argument(
-        "--input_file", type=argparse.FileType("r"), default=sys.stdin)
-    p.add_argument(
-        "--trimmed_output_file", type=argparse.FileType("w"), default=sys.stdout)
+        "--trimmed_output_file", type=argparse.FileType("w"), default=sys.stdout
+    )
     p.add_argument(
-        "--stats_output_file", type=argparse.FileType("w"), default=sys.stderr)
+        "--stats_output_file", type=argparse.FileType("w"), default=sys.stderr
+    )
 
     # Matching parameters
     p.add_argument(
-        "--max_mismatch", type=int, default=0,
-        help="Maximum number of mismatches in complete match")
+        "--max_mismatch",
+        type=int,
+        default=0,
+        help="Maximum number of mismatches in complete match",
+    )
     p.add_argument(
-        "--min_partial", type=int, default=0,
+        "--min_partial",
+        type=int,
+        default=0,
         help=(
-            "Minimum length of partial sequence match. "
-            "Skip partial matching if 0."))
+            "Minimum length of partial sequence match. " "Skip partial matching if 0."
+        ),
+    )
     p.add_argument(
-        "--min_pct_id", type=float, default=70.0,
-        help="Minimum percent identity in alignment stage")
+        "--min_pct_id",
+        type=float,
+        default=70.0,
+        help="Minimum percent identity in alignment stage",
+    )
 
     # Overall program behavior
     p.add_argument(
-        "--min_trimmed_length", type=int, default=1,
-        help="Minimum length of trimmed output sequences")
+        "--min_trimmed_length",
+        type=int,
+        default=1,
+        help="Minimum length of trimmed output sequences",
+    )
     p.add_argument(
-        "--alignment_stages", type=int, default=1,
-        help= "Number of pairwise alignment stages")
+        "--alignment_stages",
+        type=int,
+        default=1,
+        help="Number of pairwise alignment stages",
+    )
     p.add_argument(
         "--alignment_dir",
         help=(
             "Directory for files in alignment stage.  If not provided, "
-            "a temporary directory will be used."))
+            "a temporary directory will be used."
+        ),
+    )
     p.add_argument(
-        "--cores", type=int, default = 1,
-        help="Number of CPU cores to use in alignment stage")
+        "--cores",
+        type=int,
+        default=1,
+        help="Number of CPU cores to use in alignment stage",
+    )
     p.add_argument(
-        "--reverse_complement_query", action="store_true",
-        help="Reverse complement the query seq before search")
+        "--reverse_complement_query",
+        action="store_true",
+        help="Reverse complement the query seq before search",
+    )
     p.add_argument(
-        "--trim_right", action="store_true",
-        help="Trim right side, rather than left side of sequences")
+        "--trim_right",
+        action="store_true",
+        help="Trim right side, rather than left side of sequences",
+    )
 
     args = p.parse_args(argv)
 
     seqs = TrimmableSeqs.from_fasta(args.input_file)
     writer = Writer(args.trimmed_output_file, args.stats_output_file)
     app = TrimraggedApp(seqs, args.trim_right, writer, args.min_trimmed_length)
 
@@ -348,35 +393,39 @@
     if args.alignment_dir is None:
         alignment_dir = tempfile.mkdtemp()
     else:
         alignment_dir = args.alignment_dir
         if os.path.exists(alignment_dir):
             if not os.path.isdir(alignment_dir):
                 raise RuntimeError(
-                    "{0} exists and is not a directory".format(alignment_dir))
+                    "{0} exists and is not a directory".format(alignment_dir)
+                )
         else:
             os.mkdir(alignment_dir)
 
     app.matchers.append(CompleteMatcher(queryset, args.max_mismatch))
     # TODO: Partial matching does not work on right hand side
     if args.min_partial > 0:
         app.matchers.append(PartialMatcher(queryset, args.min_partial))
     for n in range(args.alignment_stages):
-        app.matchers.append(AlignmentMatcher(
-            alignment_dir,
-            min_pct_id = args.min_pct_id,
-            cores = args.cores,
-            suffix = str(n),
-        ))
+        app.matchers.append(
+            AlignmentMatcher(
+                alignment_dir,
+                min_pct_id=args.min_pct_id,
+                cores=args.cores,
+                suffix=str(n),
+            )
+        )
 
     app.run()
 
     if args.alignment_dir is None:
         shutil.rmtree(alignment_dir)
 
+
 AMBIGUOUS_BASES = {
     "T": "T",
     "C": "C",
     "A": "A",
     "G": "G",
     "R": "AG",
     "Y": "TC",
@@ -385,36 +434,36 @@
     "S": "CG",
     "W": "TA",
     "H": "TCA",
     "B": "TCG",
     "V": "CAG",
     "D": "TAG",
     "N": "TCAG",
-    }
+}
 
 
 # Ambiguous base codes for all bases EXCEPT the key
 AMBIGUOUS_BASES_COMPLEMENT = {
     "T": "V",
     "C": "D",
     "A": "B",
     "G": "H",
-    }
+}
 
 
 def deambiguate(seq):
     nt_choices = [AMBIGUOUS_BASES[x] for x in seq]
     return ["".join(c) for c in itertools.product(*nt_choices)]
 
 
 COMPLEMENT_BASES = {
     "T": "A",
     "C": "G",
     "A": "T",
     "G": "C",
-    }
+}
 
 
 def reverse_complement(seq):
     rc = [COMPLEMENT_BASES[x] for x in seq]
     rc.reverse()
-    return ''.join(rc)
+    return "".join(rc)
```

