# Comparing `tmp/sequana_multicov-1.1.0.tar.gz` & `tmp/sequana_multicov-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_multicov-1.1.0.tar", last modified: Thu Nov 24 21:16:41 2022, max compression
+gzip compressed data, was "dist/sequana_multicov-1.1.1.tar", last modified: Tue May 23 21:28:26 2023, max compression
```

## Comparing `sequana_multicov-1.1.0.tar` & `sequana_multicov-1.1.1.tar`

### file list

```diff
@@ -1,36 +1,24 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-11-24 21:16:41.000000 sequana_multicov-1.1.0/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       29 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/.coveragerc
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-11-24 21:16:41.000000 sequana_multicov-1.1.0/.github/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-11-24 21:16:41.000000 sequana_multicov-1.1.0/.github/workflows/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1351 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/.github/workflows/apptainer.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1336 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/.github/workflows/main.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      965 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/.github/workflows/pypi.yml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1530 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/LICENSE
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      182 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6828 2022-11-24 21:16:41.000000 sequana_multicov-1.1.0/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5530 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       25 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/conda.yml
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-11-24 21:16:41.000000 sequana_multicov-1.1.0/doc/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4610 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/doc/Makefile
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     9988 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/doc/conf.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2387 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/doc/index.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       41 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/requirements.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-11-24 21:16:41.000000 sequana_multicov-1.1.0/sequana_multicov.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6828 2022-11-24 21:16:40.000000 sequana_multicov-1.1.0/sequana_multicov.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      767 2022-11-24 21:16:41.000000 sequana_multicov-1.1.0/sequana_multicov.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2022-11-24 21:16:40.000000 sequana_multicov-1.1.0/sequana_multicov.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       74 2022-11-24 21:16:40.000000 sequana_multicov-1.1.0/sequana_multicov.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2022-11-24 21:16:40.000000 sequana_multicov-1.1.0/sequana_multicov.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       41 2022-11-24 21:16:40.000000 sequana_multicov-1.1.0/sequana_multicov.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2022-11-24 21:16:40.000000 sequana_multicov-1.1.0/sequana_multicov.egg-info/top_level.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-11-24 21:16:41.000000 sequana_multicov-1.1.0/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2022-11-24 21:16:41.000000 sequana_multicov-1.1.0/sequana_pipelines/multicov/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      124 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/sequana_pipelines/multicov/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2468 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/sequana_pipelines/multicov/config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    43245 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/sequana_pipelines/multicov/dag.png
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     6071 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/sequana_pipelines/multicov/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3234 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/sequana_pipelines/multicov/multicov.rules
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       16 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/sequana_pipelines/multicov/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2073 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/sequana_pipelines/multicov/schema.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      229 2022-11-24 21:16:41.000000 sequana_multicov-1.1.0/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2641 2022-11-24 21:14:59.000000 sequana_multicov-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 21:28:26.000000 sequana_multicov-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8122 2023-05-23 21:28:26.000000 sequana_multicov-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5530 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 21:28:26.000000 sequana_multicov-1.1.1/sequana_multicov.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8122 2023-05-23 21:28:25.000000 sequana_multicov-1.1.1/sequana_multicov.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-23 21:28:26.000000 sequana_multicov-1.1.1/sequana_multicov.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 21:28:25.000000 sequana_multicov-1.1.1/sequana_multicov.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       75 2023-05-23 21:28:25.000000 sequana_multicov-1.1.1/sequana_multicov.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-23 21:28:25.000000 sequana_multicov-1.1.1/sequana_multicov.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-05-23 21:28:25.000000 sequana_multicov-1.1.1/sequana_multicov.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-23 21:28:25.000000 sequana_multicov-1.1.1/sequana_multicov.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 21:28:26.000000 sequana_multicov-1.1.1/sequana_pipelines/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-23 21:28:26.000000 sequana_multicov-1.1.1/sequana_pipelines/multicov/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/sequana_pipelines/multicov/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/sequana_pipelines/multicov/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    43245 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/sequana_pipelines/multicov/dag.png
+-rwxr-xr-x   0 runner    (1001) docker     (122)     6071 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/sequana_pipelines/multicov/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3130 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/sequana_pipelines/multicov/multicov.rules
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/sequana_pipelines/multicov/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2073 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/sequana_pipelines/multicov/schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-05-23 21:28:26.000000 sequana_multicov-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2642 2023-05-23 21:28:21.000000 sequana_multicov-1.1.1/setup.py
```

### Comparing `sequana_multicov-1.1.0/PKG-INFO` & `sequana_multicov-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,197 +1,194 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: sequana_multicov
-Version: 1.1.0
+Version: 1.1.1
 Summary: Parallelise version of sequana_coverage standalone application.
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
+Description: This is is the **coverage** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ project
+        
+        
+        .. image:: https://badge.fury.io/py/sequana-multicov.svg
+             :target: https://pypi.python.org/pypi/sequana_multicov
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+            :target: http://joss.theoj.org/papers/10.21105/joss.00352
+            :alt: JOSS (journal of open source software) DOI
+        
+        .. image:: https://github.com/sequana/multicov/actions/workflows/main.yml/badge.svg
+           :target: https://github.com/sequana/multicov/actions/workflows    
+        
+        
+        :Overview: Parallelised version of sequana_coverage for large eukaryotes genome.
+        :Input: A set of BAM or BED files. BED file must have 3 or 4 columns. First column is
+            the chromosome/contig name, second column stored positions and third the
+            coverage. Fourth optional columns contains a filtered coverage (not used in
+            the analysis but shown in the HTML reports)
+        :Output: a set of HTML reports for each chromosomes and a multiqc report
+        :Status: production
+        :Citation: 
+            Dimitri Desvillechabrol, Christiane Bouchier, Sean Kennedy, Thomas Cokelaer
+            *Sequana coverage: detection and characterization of genomic variations 
+            using running median and mixture models*
+            GigaScience, Volume 7, Issue 12, December 2018, giy110, 
+            https://doi.org/10.1093/gigascience/giy110
+        
+            and 
+        
+            Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
+        
+        
+        Installation
+        ~~~~~~~~~~~~
+        
+        
+        sequana_multicov is based on Python3, just install the package as follows::
+        
+            pip install sequana_multicov --upgrade
+        
+        
+        Usage
+        ~~~~~
+        
+        ::
+        
+            sequana_multicov --help
+            sequana_multicov --input-directory DATAPATH 
+        
+        By default, this looks for BED file. WARNING. This are BED3 meaning a 3-columns
+        tabulated file like this one::
+        
+            chr1 1 10
+            chr1 2 11
+            ...
+            chr1 N1 10
+            chr2 1 20
+            chr2 2 21
+            ...
+            chr2 N2 20
+        
+        where the first column stored the chromosome name, the second is the position
+        and the third is the coverage itself. See sequana_coverage documentation for
+        details. If you have BAM files as input, we will do the conversion for you. In
+        such case, use this option::
+        
+            --input-pattern "*.bam"
+        
+        The sequana_coverage script creates a directory with the pipeline and 
+        its configuration file. You will then need 
+        to execute the pipeline::
+        
+            cd coverage
+            sh coverage.sh  # for a local run
+        
+        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
+        retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
+        
+            snakemake -s multicov.rules -c config.yaml --cores 4 --stats stats.txt
+        
+        Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface as follows::
+        
+            sequanix -w analysis -i . -p coverage
+        
+        Go to the second panel, in Input data and then in Input directory. There, you
+        must modify the pattern (empty field by default meaning search for fastq files)
+        and set the field to either::
+        
+            *.bed
+        
+        or::
+        
+            *.bam
+        
+        
+        You are ready to go. Save the project and press Run. Once done, open the HTML report.
+        
+        
+        Requirements
+        ~~~~~~~~~~~~
+        
+        This pipelines requires the following executable(s):
+        
+        - sequana_coverage from **Sequana**, which should be installed automatically.
+        - multiqc
+        
+        .. .. image:: https://raw.githubusercontent.com/sequana/multicov/master/sequana_pipelines/multicov/dag.png
+        
+        
+        Details
+        ~~~~~~~~~
+        
+        This pipeline runs **coverage** in parallel on the input BAM files (or BED file). 
+        
+        
+        The coverage tool takes as input a BAM or a BED file. The BED file must have 3
+        or 4 columns as explained in the standalone application (sequana_coverage) 
+        `documentation <http://sequana.readthedocs.io/en/master/applications.html?highlight=coverage#sequana-coverage>`_. 
+        In short, the first column is the chromosome name, the second column is the
+        position (sorted) and the third column is the coverage (an optional fourth
+        column would contain a coverage signal, which could be high quality coverage for
+        instance).
+        
+        If you have only BAM files, you can convert them using **bioconvert** tool or
+        the command::
+        
+            samtools depth -aa input.bam > output.bed
+        
+        If you have a CRAM file::
+        
+            samtools view -@ 4 -T reference.fa -b -o out.bam  in.cram
+        
+        For very large BAM/BED files, we recommend to split the BED file by
+        chromosomes. For instance for the chromosome  chr1, type::
+        
+            # samtools index in.bam
+            samtools depth -aa input.bam -r chr1 in.bam > chr1.bed
+        
+        The standalone or Snakemake application can also take as input your BAM file and
+        will convert it automatically into a BED file.
+        
+        
+        Rules and configuration details
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/multicov/main/sequana_pipelines/multicov/config.yaml>`_
+        to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
+        
+        
+        Changelog
+        ~~~~~~~~~
+        
+        ========= ====================================================================
+        Version   Description
+        ========= ====================================================================
+        1.1.0     * set apptainer containers and use wrappers
+        1.0.0     * renamed into multicov.
+                  * update to use latest sequana_pipetools (v0.9.2)
+        0.9.1     * rename genbank field into annotation, window into window_size
+        0.9.0     * first version
+        ========= ====================================================================
+        
+        
 Keywords: coverage, snakemake, sequana, running median, CNV, depltion
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-License-File: LICENSE
-
-This is is the **coverage** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ project
-
-
-.. image:: https://badge.fury.io/py/sequana-multicov.svg
-     :target: https://pypi.python.org/pypi/sequana_multicov
-
-.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
-    :target: http://joss.theoj.org/papers/10.21105/joss.00352
-    :alt: JOSS (journal of open source software) DOI
-
-.. image:: https://github.com/sequana/multicov/actions/workflows/main.yml/badge.svg
-   :target: https://github.com/sequana/multicov/actions/workflows    
-
-
-:Overview: Parallelised version of sequana_coverage for large eukaryotes genome.
-:Input: A set of BAM or BED files. BED file must have 3 or 4 columns. First column is
-    the chromosome/contig name, second column stored positions and third the
-    coverage. Fourth optional columns contains a filtered coverage (not used in
-    the analysis but shown in the HTML reports)
-:Output: a set of HTML reports for each chromosomes and a multiqc report
-:Status: production
-:Citation: 
-    Dimitri Desvillechabrol, Christiane Bouchier, Sean Kennedy, Thomas Cokelaer
-    *Sequana coverage: detection and characterization of genomic variations 
-    using running median and mixture models*
-    GigaScience, Volume 7, Issue 12, December 2018, giy110, 
-    https://doi.org/10.1093/gigascience/giy110
-
-    and 
-
-    Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
-
-
-Installation
-~~~~~~~~~~~~
-
-
-sequana_multicov is based on Python3, just install the package as follows::
-
-    pip install sequana_multicov --upgrade
-
-
-Usage
-~~~~~
-
-::
-
-    sequana_multicov --help
-    sequana_multicov --input-directory DATAPATH 
-
-By default, this looks for BED file. WARNING. This are BED3 meaning a 3-columns
-tabulated file like this one::
-
-    chr1 1 10
-    chr1 2 11
-    ...
-    chr1 N1 10
-    chr2 1 20
-    chr2 2 21
-    ...
-    chr2 N2 20
-
-where the first column stored the chromosome name, the second is the position
-and the third is the coverage itself. See sequana_coverage documentation for
-details. If you have BAM files as input, we will do the conversion for you. In
-such case, use this option::
-
-    --input-pattern "*.bam"
-
-The sequana_coverage script creates a directory with the pipeline and 
-its configuration file. You will then need 
-to execute the pipeline::
-
-    cd coverage
-    sh coverage.sh  # for a local run
-
-This launch a snakemake pipeline. If you are familiar with snakemake, you can 
-retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
-
-    snakemake -s multicov.rules -c config.yaml --cores 4 --stats stats.txt
-
-Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface as follows::
-
-    sequanix -w analysis -i . -p coverage
-
-Go to the second panel, in Input data and then in Input directory. There, you
-must modify the pattern (empty field by default meaning search for fastq files)
-and set the field to either::
-
-    *.bed
-
-or::
-
-    *.bam
-
-
-You are ready to go. Save the project and press Run. Once done, open the HTML report.
-
-
-Requirements
-~~~~~~~~~~~~
-
-This pipelines requires the following executable(s):
-
-- sequana_coverage from **Sequana**, which should be installed automatically.
-- multiqc
-
-.. .. image:: https://raw.githubusercontent.com/sequana/multicov/master/sequana_pipelines/multicov/dag.png
-
-
-Details
-~~~~~~~~~
-
-This pipeline runs **coverage** in parallel on the input BAM files (or BED file). 
-
-
-The coverage tool takes as input a BAM or a BED file. The BED file must have 3
-or 4 columns as explained in the standalone application (sequana_coverage) 
-`documentation <http://sequana.readthedocs.io/en/master/applications.html?highlight=coverage#sequana-coverage>`_. 
-In short, the first column is the chromosome name, the second column is the
-position (sorted) and the third column is the coverage (an optional fourth
-column would contain a coverage signal, which could be high quality coverage for
-instance).
-
-If you have only BAM files, you can convert them using **bioconvert** tool or
-the command::
-
-    samtools depth -aa input.bam > output.bed
-
-If you have a CRAM file::
-
-    samtools view -@ 4 -T reference.fa -b -o out.bam  in.cram
-
-For very large BAM/BED files, we recommend to split the BED file by
-chromosomes. For instance for the chromosome  chr1, type::
-
-    # samtools index in.bam
-    samtools depth -aa input.bam -r chr1 in.bam > chr1.bed
-
-The standalone or Snakemake application can also take as input your BAM file and
-will convert it automatically into a BED file.
-
-
-Rules and configuration details
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/multicov/main/sequana_pipelines/multicov/config.yaml>`_
-to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
-
-
-Changelog
-~~~~~~~~~
-
-========= ====================================================================
-Version   Description
-========= ====================================================================
-1.1.0     * set apptainer containers and use wrappers
-1.0.0     * renamed into multicov.
-          * update to use latest sequana_pipetools (v0.9.2)
-0.9.1     * rename genbank field into annotation, window into window_size
-0.9.0     * first version
-========= ====================================================================
-
-
-
```

### Comparing `sequana_multicov-1.1.0/README.rst` & `sequana_multicov-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `sequana_multicov-1.1.0/sequana_multicov.egg-info/PKG-INFO` & `sequana_multicov-1.1.1/sequana_multicov.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,197 +1,194 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: sequana-multicov
-Version: 1.1.0
+Version: 1.1.1
 Summary: Parallelise version of sequana_coverage standalone application.
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
+Description: This is is the **coverage** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ project
+        
+        
+        .. image:: https://badge.fury.io/py/sequana-multicov.svg
+             :target: https://pypi.python.org/pypi/sequana_multicov
+        
+        .. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+            :target: http://joss.theoj.org/papers/10.21105/joss.00352
+            :alt: JOSS (journal of open source software) DOI
+        
+        .. image:: https://github.com/sequana/multicov/actions/workflows/main.yml/badge.svg
+           :target: https://github.com/sequana/multicov/actions/workflows    
+        
+        
+        :Overview: Parallelised version of sequana_coverage for large eukaryotes genome.
+        :Input: A set of BAM or BED files. BED file must have 3 or 4 columns. First column is
+            the chromosome/contig name, second column stored positions and third the
+            coverage. Fourth optional columns contains a filtered coverage (not used in
+            the analysis but shown in the HTML reports)
+        :Output: a set of HTML reports for each chromosomes and a multiqc report
+        :Status: production
+        :Citation: 
+            Dimitri Desvillechabrol, Christiane Bouchier, Sean Kennedy, Thomas Cokelaer
+            *Sequana coverage: detection and characterization of genomic variations 
+            using running median and mixture models*
+            GigaScience, Volume 7, Issue 12, December 2018, giy110, 
+            https://doi.org/10.1093/gigascience/giy110
+        
+            and 
+        
+            Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
+        
+        
+        Installation
+        ~~~~~~~~~~~~
+        
+        
+        sequana_multicov is based on Python3, just install the package as follows::
+        
+            pip install sequana_multicov --upgrade
+        
+        
+        Usage
+        ~~~~~
+        
+        ::
+        
+            sequana_multicov --help
+            sequana_multicov --input-directory DATAPATH 
+        
+        By default, this looks for BED file. WARNING. This are BED3 meaning a 3-columns
+        tabulated file like this one::
+        
+            chr1 1 10
+            chr1 2 11
+            ...
+            chr1 N1 10
+            chr2 1 20
+            chr2 2 21
+            ...
+            chr2 N2 20
+        
+        where the first column stored the chromosome name, the second is the position
+        and the third is the coverage itself. See sequana_coverage documentation for
+        details. If you have BAM files as input, we will do the conversion for you. In
+        such case, use this option::
+        
+            --input-pattern "*.bam"
+        
+        The sequana_coverage script creates a directory with the pipeline and 
+        its configuration file. You will then need 
+        to execute the pipeline::
+        
+            cd coverage
+            sh coverage.sh  # for a local run
+        
+        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
+        retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
+        
+            snakemake -s multicov.rules -c config.yaml --cores 4 --stats stats.txt
+        
+        Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface as follows::
+        
+            sequanix -w analysis -i . -p coverage
+        
+        Go to the second panel, in Input data and then in Input directory. There, you
+        must modify the pattern (empty field by default meaning search for fastq files)
+        and set the field to either::
+        
+            *.bed
+        
+        or::
+        
+            *.bam
+        
+        
+        You are ready to go. Save the project and press Run. Once done, open the HTML report.
+        
+        
+        Requirements
+        ~~~~~~~~~~~~
+        
+        This pipelines requires the following executable(s):
+        
+        - sequana_coverage from **Sequana**, which should be installed automatically.
+        - multiqc
+        
+        .. .. image:: https://raw.githubusercontent.com/sequana/multicov/master/sequana_pipelines/multicov/dag.png
+        
+        
+        Details
+        ~~~~~~~~~
+        
+        This pipeline runs **coverage** in parallel on the input BAM files (or BED file). 
+        
+        
+        The coverage tool takes as input a BAM or a BED file. The BED file must have 3
+        or 4 columns as explained in the standalone application (sequana_coverage) 
+        `documentation <http://sequana.readthedocs.io/en/master/applications.html?highlight=coverage#sequana-coverage>`_. 
+        In short, the first column is the chromosome name, the second column is the
+        position (sorted) and the third column is the coverage (an optional fourth
+        column would contain a coverage signal, which could be high quality coverage for
+        instance).
+        
+        If you have only BAM files, you can convert them using **bioconvert** tool or
+        the command::
+        
+            samtools depth -aa input.bam > output.bed
+        
+        If you have a CRAM file::
+        
+            samtools view -@ 4 -T reference.fa -b -o out.bam  in.cram
+        
+        For very large BAM/BED files, we recommend to split the BED file by
+        chromosomes. For instance for the chromosome  chr1, type::
+        
+            # samtools index in.bam
+            samtools depth -aa input.bam -r chr1 in.bam > chr1.bed
+        
+        The standalone or Snakemake application can also take as input your BAM file and
+        will convert it automatically into a BED file.
+        
+        
+        Rules and configuration details
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/multicov/main/sequana_pipelines/multicov/config.yaml>`_
+        to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
+        
+        
+        Changelog
+        ~~~~~~~~~
+        
+        ========= ====================================================================
+        Version   Description
+        ========= ====================================================================
+        1.1.0     * set apptainer containers and use wrappers
+        1.0.0     * renamed into multicov.
+                  * update to use latest sequana_pipetools (v0.9.2)
+        0.9.1     * rename genbank field into annotation, window into window_size
+        0.9.0     * first version
+        ========= ====================================================================
+        
+        
 Keywords: coverage, snakemake, sequana, running median, CNV, depltion
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-License-File: LICENSE
-
-This is is the **coverage** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ project
-
-
-.. image:: https://badge.fury.io/py/sequana-multicov.svg
-     :target: https://pypi.python.org/pypi/sequana_multicov
-
-.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
-    :target: http://joss.theoj.org/papers/10.21105/joss.00352
-    :alt: JOSS (journal of open source software) DOI
-
-.. image:: https://github.com/sequana/multicov/actions/workflows/main.yml/badge.svg
-   :target: https://github.com/sequana/multicov/actions/workflows    
-
-
-:Overview: Parallelised version of sequana_coverage for large eukaryotes genome.
-:Input: A set of BAM or BED files. BED file must have 3 or 4 columns. First column is
-    the chromosome/contig name, second column stored positions and third the
-    coverage. Fourth optional columns contains a filtered coverage (not used in
-    the analysis but shown in the HTML reports)
-:Output: a set of HTML reports for each chromosomes and a multiqc report
-:Status: production
-:Citation: 
-    Dimitri Desvillechabrol, Christiane Bouchier, Sean Kennedy, Thomas Cokelaer
-    *Sequana coverage: detection and characterization of genomic variations 
-    using running median and mixture models*
-    GigaScience, Volume 7, Issue 12, December 2018, giy110, 
-    https://doi.org/10.1093/gigascience/giy110
-
-    and 
-
-    Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI https://doi:10.21105/joss.00352
-
-
-Installation
-~~~~~~~~~~~~
-
-
-sequana_multicov is based on Python3, just install the package as follows::
-
-    pip install sequana_multicov --upgrade
-
-
-Usage
-~~~~~
-
-::
-
-    sequana_multicov --help
-    sequana_multicov --input-directory DATAPATH 
-
-By default, this looks for BED file. WARNING. This are BED3 meaning a 3-columns
-tabulated file like this one::
-
-    chr1 1 10
-    chr1 2 11
-    ...
-    chr1 N1 10
-    chr2 1 20
-    chr2 2 21
-    ...
-    chr2 N2 20
-
-where the first column stored the chromosome name, the second is the position
-and the third is the coverage itself. See sequana_coverage documentation for
-details. If you have BAM files as input, we will do the conversion for you. In
-such case, use this option::
-
-    --input-pattern "*.bam"
-
-The sequana_coverage script creates a directory with the pipeline and 
-its configuration file. You will then need 
-to execute the pipeline::
-
-    cd coverage
-    sh coverage.sh  # for a local run
-
-This launch a snakemake pipeline. If you are familiar with snakemake, you can 
-retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
-
-    snakemake -s multicov.rules -c config.yaml --cores 4 --stats stats.txt
-
-Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface as follows::
-
-    sequanix -w analysis -i . -p coverage
-
-Go to the second panel, in Input data and then in Input directory. There, you
-must modify the pattern (empty field by default meaning search for fastq files)
-and set the field to either::
-
-    *.bed
-
-or::
-
-    *.bam
-
-
-You are ready to go. Save the project and press Run. Once done, open the HTML report.
-
-
-Requirements
-~~~~~~~~~~~~
-
-This pipelines requires the following executable(s):
-
-- sequana_coverage from **Sequana**, which should be installed automatically.
-- multiqc
-
-.. .. image:: https://raw.githubusercontent.com/sequana/multicov/master/sequana_pipelines/multicov/dag.png
-
-
-Details
-~~~~~~~~~
-
-This pipeline runs **coverage** in parallel on the input BAM files (or BED file). 
-
-
-The coverage tool takes as input a BAM or a BED file. The BED file must have 3
-or 4 columns as explained in the standalone application (sequana_coverage) 
-`documentation <http://sequana.readthedocs.io/en/master/applications.html?highlight=coverage#sequana-coverage>`_. 
-In short, the first column is the chromosome name, the second column is the
-position (sorted) and the third column is the coverage (an optional fourth
-column would contain a coverage signal, which could be high quality coverage for
-instance).
-
-If you have only BAM files, you can convert them using **bioconvert** tool or
-the command::
-
-    samtools depth -aa input.bam > output.bed
-
-If you have a CRAM file::
-
-    samtools view -@ 4 -T reference.fa -b -o out.bam  in.cram
-
-For very large BAM/BED files, we recommend to split the BED file by
-chromosomes. For instance for the chromosome  chr1, type::
-
-    # samtools index in.bam
-    samtools depth -aa input.bam -r chr1 in.bam > chr1.bed
-
-The standalone or Snakemake application can also take as input your BAM file and
-will convert it automatically into a BED file.
-
-
-Rules and configuration details
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Here is the `latest documented configuration file <https://raw.githubusercontent.com/sequana/multicov/main/sequana_pipelines/multicov/config.yaml>`_
-to be used with the pipeline. Each rule used in the pipeline may have a section in the configuration file. 
-
-
-Changelog
-~~~~~~~~~
-
-========= ====================================================================
-Version   Description
-========= ====================================================================
-1.1.0     * set apptainer containers and use wrappers
-1.0.0     * renamed into multicov.
-          * update to use latest sequana_pipetools (v0.9.2)
-0.9.1     * rename genbank field into annotation, window into window_size
-0.9.0     * first version
-========= ====================================================================
-
-
-
```

### Comparing `sequana_multicov-1.1.0/sequana_pipelines/multicov/config.yaml` & `sequana_multicov-1.1.1/sequana_pipelines/multicov/config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_multicov-1.1.0/sequana_pipelines/multicov/dag.png` & `sequana_multicov-1.1.1/sequana_pipelines/multicov/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_multicov-1.1.0/sequana_pipelines/multicov/main.py` & `sequana_multicov-1.1.1/sequana_pipelines/multicov/main.py`

 * *Files identical despite different names*

### Comparing `sequana_multicov-1.1.0/sequana_pipelines/multicov/multicov.rules` & `sequana_multicov-1.1.1/sequana_pipelines/multicov/multicov.rules`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,14 @@
        "multiqc/multiqc.log"
     resources:
         **config["multiqc"]["resources"]
     wrapper:
        f"{sequana_wrapper_branch}/wrappers/multiqc"
 
 
-
 rule sequana_coverage:
     input:
         bed=manager.getrawdata(),
         fasta=config['sequana_coverage']['reference_file']
     output:
         "{sample}/sequana_coverage/sequana_coverage.html"
     params:
@@ -80,16 +79,14 @@
         high_threshold=config["sequana_coverage"]["high_threshold"],
         low_threshold=config["sequana_coverage"]["low_threshold"],
         mixture_models=config["sequana_coverage"]["mixture_models"],
         gbk=config["sequana_coverage"]["annotation_file"]
     wrapper:
         f"{sequana_wrapper_branch}/wrappers/sequana_coverage"
 
-#expected_output += expand("{sample}/sequana_coverage/sequana_coverage.html", sample=manager.samples)
-
 onsuccess:
     pass
 
 
 onerror:
     from sequana_pipetools.errors import PipeError
     p = PipeError("multicov")
```

### Comparing `sequana_multicov-1.1.0/sequana_pipelines/multicov/schema.yaml` & `sequana_multicov-1.1.1/sequana_pipelines/multicov/schema.yaml`

 * *Files identical despite different names*

### Comparing `sequana_multicov-1.1.0/setup.py` & `sequana_multicov-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_namespace_packages
 
 _MAJOR               = 1
 _MINOR               = 1
-_MICRO               = 0
+_MICRO               = 1
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
     'license' : 'new BSD',
@@ -18,17 +18,17 @@
           'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Education',
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: BSD License',
           'Operating System :: OS Independent',
-          'Programming Language :: Python :: 3.7',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
+          'Programming Language :: Python :: 3.10',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Scientific/Engineering :: Bio-Informatics',
           'Topic :: Scientific/Engineering :: Information Analysis',
           'Topic :: Scientific/Engineering :: Mathematics',
           'Topic :: Scientific/Engineering :: Physics']
     }
```

