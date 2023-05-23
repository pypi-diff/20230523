# Comparing `tmp/kingfisher-0.1.2.tar.gz` & `tmp/kingfisher-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingfisher-0.1.2.tar", last modified: Mon Dec 19 07:31:08 2022, max compression
+gzip compressed data, was "kingfisher-0.2.0.tar", last modified: Tue May 23 21:16:56 2023, max compression
```

## Comparing `kingfisher-0.1.2.tar` & `kingfisher-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 07:31:08.660155 kingfisher-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2022-12-19 07:30:58.000000 kingfisher-0.1.2/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      872 2022-12-19 07:31:08.660155 kingfisher-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2022-12-19 07:30:58.000000 kingfisher-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 07:31:08.660155 kingfisher-0.1.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)    14749 2022-12-19 07:30:58.000000 kingfisher-0.1.2/bin/kingfisher
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 07:31:08.660155 kingfisher-0.1.2/kingfisher/
--rw-r--r--   0 runner    (1001) docker     (123)    38151 2022-12-19 07:30:58.000000 kingfisher-0.1.2/kingfisher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 07:31:08.660155 kingfisher-0.1.2/kingfisher/data/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2022-12-19 07:30:58.000000 kingfisher-0.1.2/kingfisher/data/asperaweb_id_dsa.openssh
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2022-12-19 07:30:58.000000 kingfisher-0.1.2/kingfisher/ena.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2022-12-19 07:30:58.000000 kingfisher-0.1.2/kingfisher/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2022-12-19 07:30:58.000000 kingfisher-0.1.2/kingfisher/location.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-19 07:30:58.000000 kingfisher-0.1.2/kingfisher/md5sum.py
--rw-r--r--   0 runner    (1001) docker     (123)    14620 2022-12-19 07:30:58.000000 kingfisher-0.1.2/kingfisher/sra_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-19 07:30:58.000000 kingfisher-0.1.2/kingfisher/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 07:31:08.660155 kingfisher-0.1.2/kingfisher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2022-12-19 07:31:08.000000 kingfisher-0.1.2/kingfisher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      481 2022-12-19 07:31:08.000000 kingfisher-0.1.2/kingfisher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 07:31:08.000000 kingfisher-0.1.2/kingfisher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2022-12-19 07:31:08.000000 kingfisher-0.1.2/kingfisher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2022-12-19 07:31:08.000000 kingfisher-0.1.2/kingfisher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 07:31:08.660155 kingfisher-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2022-12-19 07:30:58.000000 kingfisher-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 07:31:08.660155 kingfisher-0.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9068 2022-12-19 07:30:58.000000 kingfisher-0.1.2/test/test_annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2022-12-19 07:30:58.000000 kingfisher-0.1.2/test/test_ena.py
--rw-r--r--   0 runner    (1001) docker     (123)    12391 2022-12-19 07:30:58.000000 kingfisher-0.1.2/test/test_get_sra_and_aws.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:16:56.783866 kingfisher-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-23 21:16:44.000000 kingfisher-0.2.0/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-23 21:16:56.783866 kingfisher-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-23 21:16:44.000000 kingfisher-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:16:56.779866 kingfisher-0.2.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14749 2023-05-23 21:16:44.000000 kingfisher-0.2.0/bin/kingfisher
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:16:56.779866 kingfisher-0.2.0/kingfisher/
+-rw-r--r--   0 runner    (1001) docker     (123)    38156 2023-05-23 21:16:44.000000 kingfisher-0.2.0/kingfisher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:16:56.779866 kingfisher-0.2.0/kingfisher/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 21:16:44.000000 kingfisher-0.2.0/kingfisher/data/asperaweb_id_dsa.openssh
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-23 21:16:44.000000 kingfisher-0.2.0/kingfisher/ena.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-23 21:16:44.000000 kingfisher-0.2.0/kingfisher/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-05-23 21:16:44.000000 kingfisher-0.2.0/kingfisher/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-23 21:16:44.000000 kingfisher-0.2.0/kingfisher/md5sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14793 2023-05-23 21:16:44.000000 kingfisher-0.2.0/kingfisher/sra_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-23 21:16:44.000000 kingfisher-0.2.0/kingfisher/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:16:56.779866 kingfisher-0.2.0/kingfisher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-23 21:16:56.000000 kingfisher-0.2.0/kingfisher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-23 21:16:56.000000 kingfisher-0.2.0/kingfisher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 21:16:56.000000 kingfisher-0.2.0/kingfisher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-23 21:16:56.000000 kingfisher-0.2.0/kingfisher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-23 21:16:56.000000 kingfisher-0.2.0/kingfisher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 21:16:56.783866 kingfisher-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-23 21:16:44.000000 kingfisher-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 21:16:56.783866 kingfisher-0.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-05-23 21:16:44.000000 kingfisher-0.2.0/test/test_annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-23 21:16:44.000000 kingfisher-0.2.0/test/test_ena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12391 2023-05-23 21:16:44.000000 kingfisher-0.2.0/test/test_get_sra_and_aws.py
```

### Comparing `kingfisher-0.1.2/LICENCE.txt` & `kingfisher-0.2.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `kingfisher-0.1.2/PKG-INFO` & `kingfisher-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingfisher
-Version: 0.1.2
+Version: 0.2.0
 Summary: Download/extract biological FASTA/Q read data and metadata
 Home-page: https://github.com/wwood/kingfisher-download
 Author: Ben Woodcroft
 Author-email: benjwoodcroft@gmail.com
 License: GPL3+
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
```

### Comparing `kingfisher-0.1.2/bin/kingfisher` & `kingfisher-0.2.0/bin/kingfisher`

 * *Files identical despite different names*

### Comparing `kingfisher-0.1.2/kingfisher/__init__.py` & `kingfisher-0.2.0/kingfisher/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,15 +592,15 @@
         logging.error("No runs to annotate")
         sys.exit(1)
     _output_formatted_metadata(metadata, output_file, output_format, all_columns)
 
 
 def _output_formatted_metadata(metadata, output_file, output_format, all_columns):
     # default_columns = ['Run','SRAStudy','Gbp','LibraryStrategy','LibrarySelection','Model','SampleName','ScientificName']
-    default_columns = [RUN_ACCESSION_KEY,STUDY_ACCESSION_KEY,'Gbp','library_strategy','library_selection','model',SAMPLE_NAME_KEY,'taxon_name']
+    default_columns = [RUN_ACCESSION_KEY,BIOPROJECT_ACCESSION_KEY,'Gbp','library_strategy','library_selection','model',SAMPLE_NAME_KEY,'taxon_name']
 
     def prepare_for_tsv_csv(metadata, default_columns, all_columns):
         metadata_sorted = metadata.sort_values(RUN_ACCESSION_KEY)
         # For very large data frames, pandas throws an error 'InvalidIndexError:
         # Reindexing only valid with uniquely valued Index objects' when doing
         # the pd.concat() below. We have to do that concat because a simple
         # metadata_sorted['Gbp'] = ... gives a Performance warning. To get
```

### Comparing `kingfisher-0.1.2/kingfisher/data/asperaweb_id_dsa.openssh` & `kingfisher-0.2.0/kingfisher/data/asperaweb_id_dsa.openssh`

 * *Files identical despite different names*

### Comparing `kingfisher-0.1.2/kingfisher/ena.py` & `kingfisher-0.2.0/kingfisher/ena.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,18 @@
                     run_id))
             return False
         elif len(df) != 1:
             logging.error("Expected 1 row from ENA API for accession {}, got {}".format(run_id, len(df)))
             return False
 
         for _, row in df.iterrows():
+            # e.g. ERR1346134 at time of writing. See https://github.com/wwood/kingfisher-download/issues/25
+            if isinstance(float("nan"), type(row['fastq_ftp'])):
+                logging.error("No ENA FTP download URLs found for run {}, cannot continue".format(run_id))
+                return False
             ftp_urls = row['fastq_ftp'].split(';')
             md5sums = row['fastq_md5'].split(';')
             logging.debug("Found {} FTP URLs for download: {}".format(
                 len(ftp_urls), ", ".join(ftp_urls)))
 
         return EnaFileReport(ftp_urls, md5sums)
```

### Comparing `kingfisher-0.1.2/kingfisher/location.py` & `kingfisher-0.2.0/kingfisher/location.py`

 * *Files identical despite different names*

### Comparing `kingfisher-0.1.2/kingfisher/sra_metadata.py` & `kingfisher-0.2.0/kingfisher/sra_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 # Define these constants so that they can be referred to in other classes
 # without index errors.
 STUDY_ACCESSION_KEY = 'study_accession'
 RUN_ACCESSION_KEY = 'run'
 BASES_KEY = 'bases'
 SAMPLE_NAME_KEY = 'sample_name'
 NCBI_API_KEY_ENV = 'NCBI_API_KEY'
+BIOPROJECT_ACCESSION_KEY = 'bioproject'
 
 class SraMetadata:
     def add_api_key(self, other_params):
         if NCBI_API_KEY_ENV in os.environ:
             other_params['api_key'] = os.environ[NCBI_API_KEY_ENV]
         return other_params
 
@@ -134,14 +135,15 @@
             for k, v in pkg.find('./SUBMISSION').attrib.items():
                 if k not in ('accession','alias'):
                     if d['submitter'] == '':
                         d['submitter'] = v
                     else:
                         d['submitter'] = "{}, {}".format(d['submitter'], v)
             d[STUDY_ACCESSION_KEY] = try_get(lambda: pkg.find('./STUDY').attrib['accession'])
+            d[BIOPROJECT_ACCESSION_KEY] = try_get(lambda: pkg.find('./STUDY/IDENTIFIERS/EXTERNAL_ID[@namespace="BioProject"]').text)
             d['study_alias'] = try_get(lambda: pkg.find('./STUDY').attrib['alias'])
             d['study_centre_project_name'] = try_get(lambda: pkg.find('./STUDY/DESCRIPTOR/CENTER_PROJECT_NAME').text)
             d['organisation'] = try_get(lambda: pkg.find('./Organization/Name').text)
             d['organisation_department'] = try_get(lambda: pkg.find('./Organization/Address/Department').text)
             d['organisation_institution'] = try_get(lambda: pkg.find('./Organization/Address/Institution').text)
             d['organisation_street'] = try_get(lambda: pkg.find('./Organization/Address/Street').text)
             d['organisation_city'] = try_get(lambda: pkg.find('./Organization/Address/City').text)
```

### Comparing `kingfisher-0.1.2/kingfisher.egg-info/PKG-INFO` & `kingfisher-0.2.0/kingfisher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingfisher
-Version: 0.1.2
+Version: 0.2.0
 Summary: Download/extract biological FASTA/Q read data and metadata
 Home-page: https://github.com/wwood/kingfisher-download
 Author: Ben Woodcroft
 Author-email: benjwoodcroft@gmail.com
 License: GPL3+
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
```

### Comparing `kingfisher-0.1.2/setup.py` & `kingfisher-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `kingfisher-0.1.2/test/test_annotate.py` & `kingfisher-0.2.0/test/test_annotate.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 import tempfile
 from io import StringIO
 
 sys.path = [os.path.join(os.path.dirname(os.path.realpath(__file__)),'..')]+sys.path
 sys.path = [os.path.join(os.path.dirname(os.path.realpath(__file__)),'..','..')]+sys.path
 kingfisher = os.path.join(os.path.dirname(os.path.realpath(__file__)),'..','bin','kingfisher')
 
-eg_df = pd.read_csv(StringIO('run,study_accession,Gbp,library_strategy,library_selection,model,sample_name,taxon_name\n'
-    'SRR13774710,SRP307844,10.342,WGS,RANDOM,Illumina NovaSeq 6000,SCB2WXA,human gut metagenome'))
+eg_df = pd.read_csv(StringIO('run,bioproject,Gbp,library_strategy,library_selection,model,sample_name,taxon_name\n'
+    'SRR13774710,PRJNA630999,10.342,WGS,RANDOM,Illumina NovaSeq 6000,SCB2WXA,human gut metagenome'))
 
 class Tests(unittest.TestCase):
     maxDiff = None
     
     def test_one_sample_annotate(self):
         self.assertEqual(
             'run        | study_accession | Gbp   | library_strategy | library_selection | model               | sample_name | taxon_name\n' \
@@ -60,28 +60,28 @@
         'ERR1739696 | ERP017539       | 2.351 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_6       | metagenome\n' \
         'ERR1739697 | ERP017539       | 2.524 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_7       | metagenome\n' \
         'ERR1739698 | ERP017539       | 2.358 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_8       | metagenome\n' \
         'ERR1739699 | ERP017539       | 2.465 | WGS              | RANDOM            | Illumina HiSeq 2500 | MM1_9       | metagenome\n',
             extern.run('{} annotate -p PRJEB15706 --debug'.format(kingfisher)))
 
     def test_one_sample_annotate_csv(self):
-        self.assertEqual('run,study_accession,Gbp,library_strategy,library_selection,model,sample_name,taxon_name,experiment_accession,experiment_title,library_name,library_source,submitter,study_alias,study_centre_project_name,organisation,organisation_department,organisation_institution,organisation_street,organisation_city,organisation_country,organisation_contact_name,organisation_contact_email,sample_description,sample_alias,sample_accession,ENA first public,ENA last update,External Id,INSDC center alias,INSDC center name,INSDC first public,INSDC last update,INSDC status,Submitter Id,collection date,depth,environment (biome),environment (feature),environment (material),geographic location (country and/or sea),geographic location (depth),geographic location (elevation),geographic location (latitude),geographic location (longitude),investigation type,microbial mat/biofilm environmental package,project name,sample name,sample storage duration,sample storage temperature,sequencing method,study_title,design_description,study_abstract,study_links,number_of_runs_for_sample,spots,bases,run_size,published,read1_length_average,read1_length_stdev,read2_length_average,read2_length_stdev\n' \
-            'ERR1739691,ERP017539,2.382,WGS,RANDOM,Illumina HiSeq 2500,MM1_1,metagenome,ERX1809317,Illumina HiSeq 2500 paired end sequencing,unspecified,METAGENOMIC,European Nucleotide Archive,ena-STUDY-NIOZ-10-10-2016-11:18:17:022-1157,Minimal Mat 1,Royal Netherlands Institute for Sea Research,,,,,, ,,"artificial minimal coastal microbial mats at dilution 0, replicate 1",SAMEA4497179,ERS1396358,2017-06-08,2016-11-23,SAMEA4497179,NIOZ,Royal Netherlands Institute for Sea Research,2017-06-08T17:01:18Z,2016-11-23T11:15:32Z,public,MM1_1,2015-11,0.01,Microbial Mat Material,Beach,soil,Netherlands,0,0,53.489606,6.139913,metagenome,microbial mat/biofilm,Minimal Mat,MM1_1,10,20,illumina PE100,construction of minimal coastal microbial mats,,"Minimal coastal microbial mats were created with diluted coastal mat samples obtained from the Dutch barrier island of Schiermonnikoog. The MM\'s were inoculated in fresh sterilized sand in glass containers contained in a MicroBox. The MicroBox has a transparent lid (allowing photosynthetic growth) and a gas exchange filter. The MM\'s are propagated under laboratory conditions at a 16h light / 8h dark regime and at a constant 23 C. Serial dilutions used for this data-set are 0, 3 and 5-fold.",[],1,7938968,2381690400,936643449,2017-06-13 08:05:22,150,0,150,0\n',
+        self.assertEqual('run,bioproject,Gbp,library_strategy,library_selection,model,sample_name,taxon_name,experiment_accession,experiment_title,library_name,library_source,submitter,study_accession,study_alias,study_centre_project_name,organisation,organisation_department,organisation_institution,organisation_street,organisation_city,organisation_country,organisation_contact_name,organisation_contact_email,sample_description,sample_alias,sample_accession,ENA first public,ENA last update,External Id,INSDC center alias,INSDC center name,INSDC first public,INSDC last update,INSDC status,Submitter Id,collection date,depth,environment (biome),environment (feature),environment (material),geographic location (country and/or sea),geographic location (depth),geographic location (elevation),geographic location (latitude),geographic location (longitude),investigation type,microbial mat/biofilm environmental package,project name,sample name,sample storage duration,sample storage temperature,sequencing method,study_title,design_description,study_abstract,study_links,number_of_runs_for_sample,spots,bases,run_size,published,read1_length_average,read1_length_stdev,read2_length_average,read2_length_stdev\n' \
+            'ERR1739691,PRJEB15706,2.382,WGS,RANDOM,Illumina HiSeq 2500,MM1_1,metagenome,ERX1809317,Illumina HiSeq 2500 paired end sequencing,unspecified,METAGENOMIC,European Nucleotide Archive,ERP017539,ena-STUDY-NIOZ-10-10-2016-11:18:17:022-1157,Minimal Mat 1,Royal Netherlands Institute for Sea Research,,,,,, ,,"artificial minimal coastal microbial mats at dilution 0, replicate 1",SAMEA4497179,ERS1396358,2017-06-08,2016-11-23,SAMEA4497179,NIOZ,Royal Netherlands Institute for Sea Research,2017-06-08T17:01:18Z,2016-11-23T11:15:32Z,public,MM1_1,2015-11,0.01,Microbial Mat Material,Beach,soil,Netherlands,0,0,53.489606,6.139913,metagenome,microbial mat/biofilm,Minimal Mat,MM1_1,10,20,illumina PE100,construction of minimal coastal microbial mats,,"Minimal coastal microbial mats were created with diluted coastal mat samples obtained from the Dutch barrier island of Schiermonnikoog. The MM\'s were inoculated in fresh sterilized sand in glass containers contained in a MicroBox. The MicroBox has a transparent lid (allowing photosynthetic growth) and a gas exchange filter. The MM\'s are propagated under laboratory conditions at a 16h light / 8h dark regime and at a constant 23 C. Serial dilutions used for this data-set are 0, 3 and 5-fold.",[],1,7938968,2381690400,936643449,2017-06-13 08:05:22,150,0,150,0\n',
             extern.run('{} annotate -r ERR1739691 -f csv --all-columns'.format(kingfisher)))
 
     def test_json_to_stdout(self):
         self.assertEqual(
-            [{"run":"SRR13774710","study_accession":"SRP307844","Gbp":10.342,"library_strategy":"WGS","library_selection":"RANDOM","model":"Illumina NovaSeq 6000","sample_name":"SCB2WXA","taxon_name":"human gut metagenome"}],
+            [{"run":"SRR13774710","bioproject":"PRJNA630999","Gbp":10.342,"library_strategy":"WGS","library_selection":"RANDOM","model":"Illumina NovaSeq 6000","sample_name":"SCB2WXA","taxon_name":"human gut metagenome"}],
             json.loads(extern.run('{} annotate -r SRR13774710 --output-format json'.format(kingfisher))))
 
     def test_json_to_file(self):
         with tempfile.NamedTemporaryFile() as f:
             extern.run('{} annotate -r SRR13774710 --output-format json --output-file {}'.format(kingfisher, f.name))
             self.assertEqual(
-                [{"run":"SRR13774710","study_accession":"SRP307844","Gbp":10.342,"library_strategy":"WGS","library_selection":"RANDOM","model":"Illumina NovaSeq 6000","sample_name":"SCB2WXA","taxon_name":"human gut metagenome"}],
+                [{"run":"SRR13774710","bioproject":"PRJNA630999","Gbp":10.342,"library_strategy":"WGS","library_selection":"RANDOM","model":"Illumina NovaSeq 6000","sample_name":"SCB2WXA","taxon_name":"human gut metagenome"}],
                 json.loads(f.read()))
     
     def test_parquet(self):
         with tempfile.NamedTemporaryFile() as f:
             extern.run('{} annotate -r SRR13774710 --output-format parquet --output-file {}'.format(kingfisher, f.name))
             self.assertEqual(eg_df.to_dict(), pd.read_parquet(f.name).to_dict())
     
@@ -95,15 +95,15 @@
             extern.run('{} annotate -r SRR13774710 --output-format feather --output-file {}'.format(kingfisher, f.name))
             self.assertEqual(eg_df.to_dict(), pd.read_feather(f.name).to_dict())
 
     def test_bases_missing_field(self):
         with tempfile.NamedTemporaryFile() as f:
             extern.run('{} annotate -r ERR2178284 --output-format csv --output-file {}'.format(kingfisher, f.name))
             expected = {'run': {0: 'ERR2178284'},
-                'study_accession': {0: 'ERP104812'},
+                'bioproject': {0: 'PRJEB23079'},
                 'library_strategy': {0: 'WGS'},
                 'library_selection': {0: 'Hybrid Selection'},
                 'model': {0: 'Illumina HiSeq 2500'},
                 'sample_name': {0: 'STR486'},
                 'taxon_name': {0: 'Homo sapiens'}}
             observed = pd.read_csv(f.name).to_dict()
             self.assertTrue(math.isnan(observed['Gbp'][0]))
```

### Comparing `kingfisher-0.1.2/test/test_ena.py` & `kingfisher-0.2.0/test/test_ena.py`

 * *Files identical despite different names*

### Comparing `kingfisher-0.1.2/test/test_get_sra_and_aws.py` & `kingfisher-0.2.0/test/test_get_sra_and_aws.py`

 * *Files identical despite different names*

