# Comparing `tmp/ncOrtho-0.3.8.tar.gz` & `tmp/ncOrtho-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/felixl/PycharmProjects/ncOrtho/dist/.tmp-hoy7sh8d/ncOrtho-0.3.8.tar", last modified: Thu Feb  9 10:00:59 2023, max compression
+gzip compressed data, was "/home/felixl/PycharmProjects/ncOrtho/dist/.tmp-fekyc34f/ncOrtho-0.3.9.tar", last modified: Thu Feb  9 10:54:16 2023, max compression
```

## Comparing `ncOrtho-0.3.8.tar` & `ncOrtho-0.3.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:00:59.741810 ncOrtho-0.3.8/
--rw-r--r--   0 felixl   (10024) users      (501)    35149 2021-06-22 08:19:32.000000 ncOrtho-0.3.8/LICENSE
--rw-r--r--   0 felixl   (10024) users      (501)     6388 2023-02-09 10:00:59.740811 ncOrtho-0.3.8/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)     5798 2022-12-12 15:43:22.000000 ncOrtho-0.3.8/README.md
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:00:59.404836 ncOrtho-0.3.8/ncOrtho/
--rw-r--r--   0 felixl   (10024) users      (501)       43 2021-06-22 08:19:32.000000 ncOrtho-0.3.8/ncOrtho/__init__.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:00:59.543824 ncOrtho-0.3.8/ncOrtho/analysis/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2021-07-08 09:25:07.000000 ncOrtho-0.3.8/ncOrtho/analysis/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     5931 2021-07-08 10:23:46.000000 ncOrtho-0.3.8/ncOrtho/analysis/concat_alignments_dmp.pl
--rw-r--r--   0 felixl   (10024) users      (501)     1596 2021-07-08 10:23:46.000000 ncOrtho-0.3.8/ncOrtho/analysis/degapper.pl
--rw-r--r--   0 felixl   (10024) users      (501)    11893 2022-12-14 16:24:43.000000 ncOrtho-0.3.8/ncOrtho/analysis/ncAnalyze.py
--rw-r--r--   0 felixl   (10024) users      (501)     7367 2021-11-16 15:22:46.000000 ncOrtho-0.3.8/ncOrtho/blastparser.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:00:59.566823 ncOrtho-0.3.8/ncOrtho/check/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2023-02-01 12:48:24.000000 ncOrtho-0.3.8/ncOrtho/check/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     6569 2023-02-09 09:56:18.000000 ncOrtho-0.3.8/ncOrtho/check/core_synteny.py
--rw-r--r--   0 felixl   (10024) users      (501)     6037 2023-02-03 14:32:30.000000 ncOrtho-0.3.8/ncOrtho/check/tmp.py
--rw-r--r--   0 felixl   (10024) users      (501)    14276 2021-11-16 15:30:23.000000 ncOrtho-0.3.8/ncOrtho/cmsearch.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:00:59.705813 ncOrtho-0.3.8/ncOrtho/coreset/
--rw-r--r--   0 felixl   (10024) users      (501)        0 2021-06-22 08:19:32.000000 ncOrtho-0.3.8/ncOrtho/coreset/__init__.py
--rw-r--r--   0 felixl   (10024) users      (501)     6308 2022-12-14 12:48:16.000000 ncOrtho-0.3.8/ncOrtho/coreset/core_reblast.py
--rw-r--r--   0 felixl   (10024) users      (501)     9117 2023-02-09 09:45:50.000000 ncOrtho-0.3.8/ncOrtho/coreset/coreset.py
--rw-r--r--   0 felixl   (10024) users      (501)     8446 2023-02-09 09:41:32.000000 ncOrtho-0.3.8/ncOrtho/coreset/coreset_utils.py
--rw-r--r--   0 felixl   (10024) users      (501)     3163 2021-11-16 15:37:13.000000 ncOrtho-0.3.8/ncOrtho/coreset/createcm.py
--rw-r--r--   0 felixl   (10024) users      (501)     1019 2021-06-22 08:54:38.000000 ncOrtho-0.3.8/ncOrtho/coreset/example_parameters.yaml
--rw-r--r--   0 felixl   (10024) users      (501)     6493 2022-12-14 12:42:11.000000 ncOrtho-0.3.8/ncOrtho/coreset/locate_position.py
--rw-r--r--   0 felixl   (10024) users      (501)     4640 2023-01-30 12:01:49.000000 ncOrtho-0.3.8/ncOrtho/coreset/synteny.py
--rw-r--r--   0 felixl   (10024) users      (501)    17311 2022-12-12 15:44:00.000000 ncOrtho-0.3.8/ncOrtho/coreset/tmp.py
--rw-r--r--   0 felixl   (10024) users      (501)     1971 2021-06-23 13:13:57.000000 ncOrtho-0.3.8/ncOrtho/genparser.py
--rwxr-xr-x   0 felixl   (10024) users      (501)    21811 2022-12-12 16:48:28.000000 ncOrtho-0.3.8/ncOrtho/ncortho.py
--rw-r--r--   0 felixl   (10024) users      (501)      913 2022-12-09 10:21:59.000000 ncOrtho-0.3.8/ncOrtho/utils.py
-drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:00:59.473828 ncOrtho-0.3.8/ncOrtho.egg-info/
--rw-r--r--   0 felixl   (10024) users      (501)     6388 2023-02-09 10:00:59.000000 ncOrtho-0.3.8/ncOrtho.egg-info/PKG-INFO
--rw-r--r--   0 felixl   (10024) users      (501)      829 2023-02-09 10:00:59.000000 ncOrtho-0.3.8/ncOrtho.egg-info/SOURCES.txt
--rw-r--r--   0 felixl   (10024) users      (501)        1 2023-02-09 10:00:59.000000 ncOrtho-0.3.8/ncOrtho.egg-info/dependency_links.txt
--rw-r--r--   0 felixl   (10024) users      (501)      176 2023-02-09 10:00:59.000000 ncOrtho-0.3.8/ncOrtho.egg-info/entry_points.txt
--rw-r--r--   0 felixl   (10024) users      (501)       25 2023-02-09 10:00:59.000000 ncOrtho-0.3.8/ncOrtho.egg-info/requires.txt
--rw-r--r--   0 felixl   (10024) users      (501)        8 2023-02-09 10:00:59.000000 ncOrtho-0.3.8/ncOrtho.egg-info/top_level.txt
--rw-r--r--   0 felixl   (10024) users      (501)      103 2021-06-30 12:35:13.000000 ncOrtho-0.3.8/pyproject.toml
--rw-r--r--   0 felixl   (10024) users      (501)       38 2023-02-09 10:00:59.741812 ncOrtho-0.3.8/setup.cfg
--rw-r--r--   0 felixl   (10024) users      (501)     1959 2023-02-09 10:00:50.000000 ncOrtho-0.3.8/setup.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.379438 ncOrtho-0.3.9/
+-rw-r--r--   0 felixl   (10024) users      (501)    35149 2021-06-22 08:19:32.000000 ncOrtho-0.3.9/LICENSE
+-rw-r--r--   0 felixl   (10024) users      (501)     6388 2023-02-09 10:54:16.378440 ncOrtho-0.3.9/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)     5798 2022-12-12 15:43:22.000000 ncOrtho-0.3.9/README.md
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.208456 ncOrtho-0.3.9/ncOrtho/
+-rw-r--r--   0 felixl   (10024) users      (501)       43 2021-06-22 08:19:32.000000 ncOrtho-0.3.9/ncOrtho/__init__.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.283451 ncOrtho-0.3.9/ncOrtho/analysis/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2021-07-08 09:25:07.000000 ncOrtho-0.3.9/ncOrtho/analysis/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     5931 2021-07-08 10:23:46.000000 ncOrtho-0.3.9/ncOrtho/analysis/concat_alignments_dmp.pl
+-rw-r--r--   0 felixl   (10024) users      (501)     1596 2021-07-08 10:23:46.000000 ncOrtho-0.3.9/ncOrtho/analysis/degapper.pl
+-rw-r--r--   0 felixl   (10024) users      (501)    11893 2022-12-14 16:24:43.000000 ncOrtho-0.3.9/ncOrtho/analysis/ncAnalyze.py
+-rw-r--r--   0 felixl   (10024) users      (501)     7367 2021-11-16 15:22:46.000000 ncOrtho-0.3.9/ncOrtho/blastparser.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.321445 ncOrtho-0.3.9/ncOrtho/check/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2023-02-01 12:48:24.000000 ncOrtho-0.3.9/ncOrtho/check/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     6967 2023-02-09 10:46:00.000000 ncOrtho-0.3.9/ncOrtho/check/core_synteny.py
+-rw-r--r--   0 felixl   (10024) users      (501)     6037 2023-02-03 14:32:30.000000 ncOrtho-0.3.9/ncOrtho/check/tmp.py
+-rw-r--r--   0 felixl   (10024) users      (501)    14276 2021-11-16 15:30:23.000000 ncOrtho-0.3.9/ncOrtho/cmsearch.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.360446 ncOrtho-0.3.9/ncOrtho/coreset/
+-rw-r--r--   0 felixl   (10024) users      (501)        0 2021-06-22 08:19:32.000000 ncOrtho-0.3.9/ncOrtho/coreset/__init__.py
+-rw-r--r--   0 felixl   (10024) users      (501)     6308 2022-12-14 12:48:16.000000 ncOrtho-0.3.9/ncOrtho/coreset/core_reblast.py
+-rw-r--r--   0 felixl   (10024) users      (501)     9117 2023-02-09 09:45:50.000000 ncOrtho-0.3.9/ncOrtho/coreset/coreset.py
+-rw-r--r--   0 felixl   (10024) users      (501)     8446 2023-02-09 09:41:32.000000 ncOrtho-0.3.9/ncOrtho/coreset/coreset_utils.py
+-rw-r--r--   0 felixl   (10024) users      (501)     3163 2021-11-16 15:37:13.000000 ncOrtho-0.3.9/ncOrtho/coreset/createcm.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1019 2021-06-22 08:54:38.000000 ncOrtho-0.3.9/ncOrtho/coreset/example_parameters.yaml
+-rw-r--r--   0 felixl   (10024) users      (501)     6493 2022-12-14 12:42:11.000000 ncOrtho-0.3.9/ncOrtho/coreset/locate_position.py
+-rw-r--r--   0 felixl   (10024) users      (501)     4640 2023-01-30 12:01:49.000000 ncOrtho-0.3.9/ncOrtho/coreset/synteny.py
+-rw-r--r--   0 felixl   (10024) users      (501)    17311 2022-12-12 15:44:00.000000 ncOrtho-0.3.9/ncOrtho/coreset/tmp.py
+-rw-r--r--   0 felixl   (10024) users      (501)     1971 2021-06-23 13:13:57.000000 ncOrtho-0.3.9/ncOrtho/genparser.py
+-rwxr-xr-x   0 felixl   (10024) users      (501)    21811 2022-12-12 16:48:28.000000 ncOrtho-0.3.9/ncOrtho/ncortho.py
+-rw-r--r--   0 felixl   (10024) users      (501)      913 2022-12-09 10:21:59.000000 ncOrtho-0.3.9/ncOrtho/utils.py
+drwxr-xr-x   0 felixl   (10024) users      (501)        0 2023-02-09 10:54:16.246447 ncOrtho-0.3.9/ncOrtho.egg-info/
+-rw-r--r--   0 felixl   (10024) users      (501)     6388 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/PKG-INFO
+-rw-r--r--   0 felixl   (10024) users      (501)      829 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/SOURCES.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        1 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/dependency_links.txt
+-rw-r--r--   0 felixl   (10024) users      (501)      176 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/entry_points.txt
+-rw-r--r--   0 felixl   (10024) users      (501)       25 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/requires.txt
+-rw-r--r--   0 felixl   (10024) users      (501)        8 2023-02-09 10:54:16.000000 ncOrtho-0.3.9/ncOrtho.egg-info/top_level.txt
+-rw-r--r--   0 felixl   (10024) users      (501)      103 2021-06-30 12:35:13.000000 ncOrtho-0.3.9/pyproject.toml
+-rw-r--r--   0 felixl   (10024) users      (501)       38 2023-02-09 10:54:16.380439 ncOrtho-0.3.9/setup.cfg
+-rw-r--r--   0 felixl   (10024) users      (501)     1959 2023-02-09 10:10:05.000000 ncOrtho-0.3.9/setup.py
```

### Comparing `ncOrtho-0.3.8/LICENSE` & `ncOrtho-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/PKG-INFO` & `ncOrtho-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncOrtho
-Version: 0.3.8
+Version: 0.3.9
 Summary:  Targeted ortholog search for miRNAs 
 Home-page: https://github.com/felixlangschied/ncortho
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncOrtho-0.3.8/README.md` & `ncOrtho-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/analysis/concat_alignments_dmp.pl` & `ncOrtho-0.3.9/ncOrtho/analysis/concat_alignments_dmp.pl`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/analysis/degapper.pl` & `ncOrtho-0.3.9/ncOrtho/analysis/degapper.pl`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/analysis/ncAnalyze.py` & `ncOrtho-0.3.9/ncOrtho/analysis/ncAnalyze.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/blastparser.py` & `ncOrtho-0.3.9/ncOrtho/blastparser.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/check/core_synteny.py` & `ncOrtho-0.3.9/ncOrtho/check/core_synteny.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,40 +96,46 @@
     optional.add_argument(
         '--idtype', metavar='str', type=str,
         help='Choose the ID in the reference gff file that is '
              'compared to the IDs in the pairwise orthologs file (default:GeneID) '
              'Options: ID, Name, GeneID, gene_id, CDS',
         nargs='?', const='ID=', default='ID'
     )
+    optional.add_argument(
+        '--outformat', metavar='str', type=str,
+        help='Choose format for output figures, as accepted by matplotlib package (Default: png)',
+        nargs='?', const='png', default='png'
+    )
     # Show help when no arguments are added.
     if len(sys.argv) == 1:
         parser.print_help()
         sys.exit(1)
     else:
         args = parser.parse_args()
 
     # parameters
     add_pos_orthos = args.max_anchor_dist
     idtype = args.idtype
 
     core_dict, ref_paths, all_paths = cu.parse_yaml(args.parameters)
     # check if files exist
-    #for cp in all_paths:
+    # for cp in all_paths:
     #    if not os.path.isfile(cp):
     #        raise ValueError(f'{cp} does not exist')
 
     ref_anno_dict = cu.gff_parser(ref_paths['annotation'], 'ID')
     print('# Reading pairwise orthologs', flush=True)
     if idtype == 'CDS':
         ortho_dict = cu.pairwise_orthologs_from_cds(core_dict, ref_paths['annotation'])
     else:
         ortho_dict = cu.read_pairwise_orthologs(core_dict)
 
     syn_col = []
     ortho_col = []
+    print('# Checking synteny conservation', flush=True)
     for corespec, pairwiseorthos in ortho_dict.items():
 
         core_col = []
         print(corespec)
         ortho_col.append([corespec, len(pairwiseorthos.keys())])
 
         core_anno_dict = cu.gff_parser(core_dict[corespec]['annotation'], 'ID')
@@ -146,23 +152,25 @@
     orth = orth.sort_values(by='Number orthologs', ascending=False)
     o = orth.species.values
     sns.set(rc={'figure.figsize': (6, 6), 'ytick.left': True, 'xtick.bottom': True}, font_scale=1.2, style='whitegrid')
     sns.barplot(data=orth, x='species', y='Number orthologs')
     plt.xticks(rotation=45, ha='right')
     plt.xlabel('')
     plt.tight_layout()
-    plt.savefig(f'{args.output}/ortholog_distribution.svg')
+    plt.savefig(f'{args.output}/ortholog_distribution.{args.outformat}')
 
-    plt.figure()
+
+    plt.clf()
+    plt.figure(figsize=(12, 4))
     df = pd.DataFrame(syn_col, columns=['species', 'reference_protein', 'num_conserved_anchors'])
     sns.set(rc={'figure.figsize': (12, 4), 'ytick.left': True, 'xtick.bottom': True}, font_scale=1.2, style='whitegrid')
     ax = sns.histplot(data=df, x='num_conserved_anchors', hue='species', discrete=True, multiple='dodge', hue_order=o,
                       shrink=0.8)
     sns.move_legend(ax, "upper left", bbox_to_anchor=(1, 1))
     plt.xlabel(f'Number of conserved anchors in neighborhood k={add_pos_orthos}')
-    plt.savefig(f'{args.output}/anchor_conservation.svg')
     plt.tight_layout()
+    plt.savefig(f'{args.output}/anchor_conservation.{args.outformat}')
+    print(f'# Finished. Output created at: {args.output}')
 
 
 if __name__ == '__main__':
     main()
-
```

### Comparing `ncOrtho-0.3.8/ncOrtho/check/tmp.py` & `ncOrtho-0.3.9/ncOrtho/check/tmp.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/cmsearch.py` & `ncOrtho-0.3.9/ncOrtho/cmsearch.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/coreset/core_reblast.py` & `ncOrtho-0.3.9/ncOrtho/coreset/core_reblast.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/coreset/coreset.py` & `ncOrtho-0.3.9/ncOrtho/coreset/coreset.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/coreset/coreset_utils.py` & `ncOrtho-0.3.9/ncOrtho/coreset/coreset_utils.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/coreset/createcm.py` & `ncOrtho-0.3.9/ncOrtho/coreset/createcm.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/coreset/example_parameters.yaml` & `ncOrtho-0.3.9/ncOrtho/coreset/example_parameters.yaml`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/coreset/locate_position.py` & `ncOrtho-0.3.9/ncOrtho/coreset/locate_position.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/coreset/synteny.py` & `ncOrtho-0.3.9/ncOrtho/coreset/synteny.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/coreset/tmp.py` & `ncOrtho-0.3.9/ncOrtho/coreset/tmp.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/genparser.py` & `ncOrtho-0.3.9/ncOrtho/genparser.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/ncortho.py` & `ncOrtho-0.3.9/ncOrtho/ncortho.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho/utils.py` & `ncOrtho-0.3.9/ncOrtho/utils.py`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/ncOrtho.egg-info/PKG-INFO` & `ncOrtho-0.3.9/ncOrtho.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncOrtho
-Version: 0.3.8
+Version: 0.3.9
 Summary:  Targeted ortholog search for miRNAs 
 Home-page: https://github.com/felixlangschied/ncortho
 Author: Felix Langschied
 Author-email: langschied@bio.uni-frankfurt.de
 License: GPL-3.0
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ncOrtho-0.3.8/ncOrtho.egg-info/SOURCES.txt` & `ncOrtho-0.3.9/ncOrtho.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncOrtho-0.3.8/setup.py` & `ncOrtho-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ncOrtho",
-    version="0.3.8",
+    version="0.3.9",
     python_requires='>=3.7.0',
     description=" Targeted ortholog search for miRNAs ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Felix Langschied",
     author_email="langschied@bio.uni-frankfurt.de",
     url="https://github.com/felixlangschied/ncortho",
```

