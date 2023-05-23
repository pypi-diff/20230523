# Comparing `tmp/hepcrawl-9.0.8.tar.gz` & `tmp/hepcrawl-9.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hepcrawl-9.0.8.tar", last modified: Tue Feb 13 09:56:06 2018, max compression
+gzip compressed data, was "dist/hepcrawl-9.0.9.tar", last modified: Tue Feb 13 21:54:30 2018, max compression
```

## Comparing `hepcrawl-9.0.8.tar` & `hepcrawl-9.0.9.tar`

### file list

```diff
@@ -1,256 +1,256 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9021 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/contributing.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      381 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/changes.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1590 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      357 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/releasenotes.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     8349 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/Makefile
--rw-rw-r--   0 travis    (2000) travis    (2000)     1814 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/license.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      344 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/authors.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1846 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/spiders.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      617 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/overview.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1510 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/guide.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/installation.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     4388 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/operations.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)    11864 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     3079 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2487 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/mappings.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl/testlib/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3460 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/testlib/celery_monitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1441 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/testlib/tasks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      327 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/testlib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      665 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/testlib/scrapyd_coverage_runner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4397 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/testlib/fixtures.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1023 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/testlib/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5655 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12471 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/tohep.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3939 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/inputs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6060 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/dateutils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6243 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/pipelines.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      926 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/scrapyd.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1724 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/outputs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      681 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      529 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/downloaders.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6428 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/middlewares.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      561 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/extensions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl/extractors/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4062 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/extractors/jats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      381 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/extractors/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4800 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/extractors/nlm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      525 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/scrapy.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     7719 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/items.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14926 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl/spiders/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8438 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/brown_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8113 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/hindawi_spider.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl/spiders/common/
--rw-rw-r--   0 travis    (2000) travis    (2000)      309 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/common/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3928 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/common/last_run_store.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5729 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/common/oaipmh_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7101 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/aps_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2798 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/cds_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40838 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/elsevier_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6482 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/magic_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4449 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/phenix_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9050 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/base_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5991 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/t2k_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6541 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/phil_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8916 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/infn_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      569 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8634 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/mit_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25033 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/edp_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8742 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/iop_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8064 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/wsp_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8684 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/arxiv_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13473 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/pos_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8861 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/dnb_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9783 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/desy_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5158 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/spiders/alpha_spider.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5600 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/loaders.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl/parsers/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19523 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/parsers/jats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      395 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/hepcrawl/parsers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17897 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/CHANGELOG
--rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     2069 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/INSTALL.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      212 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/wsp/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/wsp/fixtures/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/wsp/fixtures/ftp_server/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/wsp/fixtures/ftp_server/WSP/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4412 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/wsp/fixtures/ftp_server/WSP/IDAQPv20i01-03160015-1510863.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)     4224 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/wsp/fixtures/wsp_smoke_records.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     5346 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/wsp/test_wsp.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/arxiv/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/arxiv/test_arxiv.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/arxiv/fixtures/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18755 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/arxiv/fixtures/arxiv_expected.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/arxiv/fixtures/http_server/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/arxiv/fixtures/http_server/records/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7668 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/arxiv/fixtures/http_server/records/arxiv-physics-hep-ex.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     6528 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/arxiv/fixtures/http_server/records/arxiv-physics-hep-th.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/pos/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3226 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/pos/test_pos.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/pos/fixtures/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/pos/fixtures/oai_harvested/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2361 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/pos/fixtures/oai_harvested/pos_record.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/pos/fixtures/pos_conference_proceedings_records.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/pos/fixtures/https_server/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/pos/fixtures/https_server/records/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2470 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/pos/fixtures/https_server/records/PoS(LATTICE 2013)001.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     7535 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/pos/fixtures/https_server/records/187.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/desy/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/desy/fixtures/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/desy/fixtures/ftp_server/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/desy/fixtures/ftp_server/DESY/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/desy/fixtures/ftp_server/DESY/FFT/
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/desy/fixtures/ftp_server/DESY/FFT/desy-thesis-17-036.title.pdf
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/desy/fixtures/ftp_server/DESY/FFT/desy-thesis-17-035.title.pdf
--rw-rw-r--   0 travis    (2000) travis    (2000)    18509 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/desy/fixtures/ftp_server/DESY/desy_collection_records.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    17816 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/desy/fixtures/desy_records_ftp_expected.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    17816 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/desy/fixtures/desy_records_local_expected.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4712 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/desy/test_desy.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/cds/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/cds/fixtures/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/functional/cds/fixtures/oai_harvested/
--rw-rw-r--   0 travis    (2000) travis    (2000)    13058 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/cds/fixtures/oai_harvested/cds_smoke_records.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     4089 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/cds/fixtures/cds_smoke_records_expected.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4405 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/functional/cds/test_cds.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2175 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_testlib_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8223 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_iop.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6581 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_pos.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5280 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_t2k.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10591 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_phil.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1314 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_extensions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7025 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_aps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5836 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_mit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3068 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_dateutils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2823 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_phenix.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13325 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_world_scientific.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/elsevier/
--rw-rw-r--   0 travis    (2000) travis    (2000)    16279 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/elsevier/sample_consyn_record.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      828 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/elsevier/fake_astropart.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)      913 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/elsevier/fake_nima.zip
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/hindawi/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4761 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/hindawi/test_1.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/brown/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3604 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/brown/test_1.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4796 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/brown/test_splash.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/mit/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6103 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/mit/test_splash.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/mit/test_list.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/iop/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/iop/xml/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6270 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/iop/xml/test_standard.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/iop/packages/
--rw-rw-r--   0 travis    (2000) travis    (2000)      924 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/iop/packages/test.tar.gz
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/iop/pdf/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1868 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/iop/pdf/test_143_3_336.pdf
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/t2k/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19178 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/t2k/001.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1869 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/t2k/test_1_nourl.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1925 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/t2k/test_1.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2639 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record2.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2545 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record5.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     3757 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record10_parsed.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6622 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record4.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     3948 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record8.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record1.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2372 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record3.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     3003 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record6.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)    25506 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     3248 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record10.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     3104 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record7.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record0.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record9.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/pos/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1303 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/pos/sample_splash_page.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     2361 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/pos/sample_pos_record.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     7999 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/pos/sample_proceedings_page.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/base/
--rw-rw-r--   0 travis    (2000) travis    (2000)    33726 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/base/test_1_splash.htm
--rw-rw-r--   0 travis    (2000) travis    (2000)     5253 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/base/test_1.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/world_scientific/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4600 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/world_scientific/wsp_record.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     7476 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/world_scientific/sample_ws_record.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/alpha/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3243 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/alpha/test_1.htm
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/phil/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3322 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/phil/test_journal.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     4383 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/phil/test_thesis.json
--rw-rw-r--   0 travis    (2000) travis    (2000)       52 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/phil/fake_splash.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/desy/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8824 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/desy/faulty_record.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     8512 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/desy/desy_record_expected.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    17824 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/desy/desy_collection_records_expected.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    18512 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/desy/desy_collection_records.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     8818 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/desy/desy_record.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/infn/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/infn/test_1.html
--rw-rw-r--   0 travis    (2000) travis    (2000)      964 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/infn/test_1_nolink.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     8097 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/infn/test_splash.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/edp/
--rw-rw-r--   0 travis    (2000) travis    (2000)      878 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/edp/jats_splash.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     3466 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/edp/test_gz.tar.gz
--rw-rw-r--   0 travis    (2000) travis    (2000)     6265 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/edp/jats.xml
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4157 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/edp/rich.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)      736 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/edp/rich_splash.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     1937 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/edp/test_rich.tar.bz2
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/magic/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/magic/test_1.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4611 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/magic/test_splash.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     4536 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/magic/test_list.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/aps/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5408 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/aps/aps_single_parsed.json
--rw-rw-r--   0 travis    (2000) travis    (2000)   376368 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/aps/PhysRevX.7.021022.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)   427811 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/aps/PhysRevX.4.021018.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)   752507 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/aps/PhysRevD.96.095036.xml
--rw-rw-r--   0 travis    (2000) travis    (2000)     5765 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/aps/aps_single_response.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/dnb/
--rw-rw-r--   0 travis    (2000) travis    (2000)    21213 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/dnb/test_splash.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     8523 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/dnb/test_1.xml
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/responses/phenix/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2233 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/responses/phenix/test_1.html
--rw-rw-r--   0 travis    (2000) travis    (2000)     6415 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_arxiv_single.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8624 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_brown.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4255 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_hindawi.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5275 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_infn.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    23617 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_edp.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9661 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_magic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3214 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_parsers_jats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9235 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      681 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_inputs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3577 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_desy.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2545 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_oaipmh.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1639 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_tohep.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6756 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_arxiv_all.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5097 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_alpha.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12449 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      496 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    60585 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_elsevier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2675 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_pipelines.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/tests/unit/data/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/data/test.zip
--rw-rw-r--   0 travis    (2000) travis    (2000)       49 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/data/netrc
--rw-rw-r--   0 travis    (2000) travis    (2000)     9555 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/tests/unit/test_dnb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      903 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2601 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1229 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/RELEASE-NOTES.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      426 2018-02-13 09:52:53.000000 hepcrawl-9.0.8/pytest.ini
--rw-rw-r--   0 travis    (2000) travis    (2000)      542 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/AUTHORS
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)     1129 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2601 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       39 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     7038 2018-02-13 09:56:06.000000 hepcrawl-9.0.8/hepcrawl.egg-info/SOURCES.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9021 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/contributing.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      381 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/changes.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1590 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      357 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/releasenotes.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8349 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/Makefile
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1814 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/license.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      344 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/authors.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1846 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/spiders.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      617 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/overview.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1510 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/guide.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/installation.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4388 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/operations.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11864 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1356 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/README.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3079 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/hepcrawl/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2487 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/mappings.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/hepcrawl/testlib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3460 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/testlib/celery_monitor.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1441 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/testlib/tasks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      327 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/testlib/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      665 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/testlib/scrapyd_coverage_runner.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4397 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/testlib/fixtures.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1023 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/testlib/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5655 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12471 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/tohep.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3939 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/inputs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6060 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/dateutils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6243 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/pipelines.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      926 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/scrapyd.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1724 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/outputs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      681 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      529 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/downloaders.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6428 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/middlewares.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      561 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1002 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/extensions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/hepcrawl/extractors/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4062 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/extractors/jats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      381 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/extractors/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4800 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/extractors/nlm.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      525 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/scrapy.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7719 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/items.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14946 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/hepcrawl/spiders/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8438 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/brown_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8113 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/hindawi_spider.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/hepcrawl/spiders/common/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      309 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/common/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3928 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/common/last_run_store.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5729 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/common/oaipmh_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7101 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/aps_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2798 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/cds_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40838 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/elsevier_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6482 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/magic_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4449 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/phenix_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9050 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/base_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5991 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/t2k_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6541 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/phil_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8916 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/infn_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      569 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8634 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/mit_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25033 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/edp_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8742 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/iop_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8064 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/wsp_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8684 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/arxiv_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13473 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/pos_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8861 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/dnb_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9783 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/desy_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5158 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/spiders/alpha_spider.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5600 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/loaders.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/hepcrawl/parsers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19523 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/parsers/jats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      395 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/hepcrawl/parsers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17675 2018-02-13 21:54:29.000000 hepcrawl-9.0.9/CHANGELOG
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1798 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2069 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/INSTALL.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      212 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/setup.cfg
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/wsp/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/wsp/fixtures/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/wsp/fixtures/ftp_server/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/wsp/fixtures/ftp_server/WSP/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4412 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/wsp/fixtures/ftp_server/WSP/IDAQPv20i01-03160015-1510863.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4224 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/wsp/fixtures/wsp_smoke_records.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5346 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/wsp/test_wsp.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/arxiv/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2536 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/arxiv/test_arxiv.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/arxiv/fixtures/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18755 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/arxiv/fixtures/arxiv_expected.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/arxiv/fixtures/http_server/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/arxiv/fixtures/http_server/records/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7668 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/arxiv/fixtures/http_server/records/arxiv-physics-hep-ex.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6528 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/arxiv/fixtures/http_server/records/arxiv-physics-hep-th.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/pos/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3226 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/pos/test_pos.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/pos/fixtures/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/pos/fixtures/oai_harvested/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2361 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/pos/fixtures/oai_harvested/pos_record.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/pos/fixtures/pos_conference_proceedings_records.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/pos/fixtures/https_server/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/pos/fixtures/https_server/records/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2470 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/pos/fixtures/https_server/records/PoS(LATTICE 2013)001.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7535 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/pos/fixtures/https_server/records/187.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/desy/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/desy/fixtures/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/desy/fixtures/ftp_server/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/desy/fixtures/ftp_server/DESY/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/desy/fixtures/ftp_server/DESY/FFT/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/desy/fixtures/ftp_server/DESY/FFT/desy-thesis-17-036.title.pdf
+-rw-rw-r--   0 travis    (2000) travis    (2000)       12 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/desy/fixtures/ftp_server/DESY/FFT/desy-thesis-17-035.title.pdf
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18509 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/desy/fixtures/ftp_server/DESY/desy_collection_records.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17816 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/desy/fixtures/desy_records_ftp_expected.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17816 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/desy/fixtures/desy_records_local_expected.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4712 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/desy/test_desy.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/cds/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/cds/fixtures/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/functional/cds/fixtures/oai_harvested/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13058 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/cds/fixtures/oai_harvested/cds_smoke_records.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4089 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/cds/fixtures/cds_smoke_records_expected.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4405 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/functional/cds/test_cds.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2175 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_testlib_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8223 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_iop.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6581 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_pos.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5280 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_t2k.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10591 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_phil.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1314 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_extensions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7025 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_aps.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5836 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_mit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3068 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_dateutils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2823 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_phenix.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13325 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_world_scientific.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/elsevier/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16279 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/elsevier/sample_consyn_record.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      828 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/elsevier/fake_astropart.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)      913 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/elsevier/fake_nima.zip
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/hindawi/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4761 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/hindawi/test_1.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/brown/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3604 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/brown/test_1.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4796 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/brown/test_splash.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/mit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6103 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/mit/test_splash.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1144 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/mit/test_list.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/iop/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/iop/xml/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6270 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/iop/xml/test_standard.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/iop/packages/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      924 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/iop/packages/test.tar.gz
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/iop/pdf/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1868 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/iop/pdf/test_143_3_336.pdf
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/t2k/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19178 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/t2k/001.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1869 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/t2k/test_1_nourl.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1925 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/t2k/test_1.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2639 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record2.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2545 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record5.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3757 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record10_parsed.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6622 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record4.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3948 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record8.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2385 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record1.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2372 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record3.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3003 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record6.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25506 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3248 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record10.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3104 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record7.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2357 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record0.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2254 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record9.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/pos/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1303 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/pos/sample_splash_page.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2361 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/pos/sample_pos_record.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7999 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/pos/sample_proceedings_page.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/base/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    33726 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/base/test_1_splash.htm
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5253 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/base/test_1.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/world_scientific/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4600 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/world_scientific/wsp_record.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7476 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/world_scientific/sample_ws_record.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/alpha/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3243 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/alpha/test_1.htm
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/phil/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3322 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/phil/test_journal.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4383 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/phil/test_thesis.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)       52 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/phil/fake_splash.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/desy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8824 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/desy/faulty_record.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8512 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/desy/desy_record_expected.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17824 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/desy/desy_collection_records_expected.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18512 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/desy/desy_collection_records.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8818 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/desy/desy_record.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/infn/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/infn/test_1.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)      964 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/infn/test_1_nolink.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8097 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/infn/test_splash.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/edp/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      878 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/edp/jats_splash.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3466 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/edp/test_gz.tar.gz
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6265 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/edp/jats.xml
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4157 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/edp/rich.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      736 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/edp/rich_splash.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1937 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/edp/test_rich.tar.bz2
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/magic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1083 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/magic/test_1.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4611 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/magic/test_splash.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4536 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/magic/test_list.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/aps/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5408 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/aps/aps_single_parsed.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)   376368 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/aps/PhysRevX.7.021022.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)   427811 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/aps/PhysRevX.4.021018.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)   752507 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/aps/PhysRevD.96.095036.xml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5765 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/aps/aps_single_response.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/dnb/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21213 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/dnb/test_splash.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8523 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/dnb/test_1.xml
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/responses/phenix/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2233 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/responses/phenix/test_1.html
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6415 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_arxiv_single.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8624 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_brown.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4255 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_hindawi.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5275 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_infn.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    23617 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_edp.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9661 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_magic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3214 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_parsers_jats.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9315 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      681 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_inputs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3577 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_desy.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2545 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_oaipmh.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1639 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_tohep.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6756 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_arxiv_all.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5097 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_alpha.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12449 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      496 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/conftest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    60585 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_elsevier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2675 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_pipelines.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/tests/unit/data/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2652 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/data/test.zip
+-rw-rw-r--   0 travis    (2000) travis    (2000)       49 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/data/netrc
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9555 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/tests/unit/test_dnb.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      903 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2601 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1229 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/RELEASE-NOTES.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)      426 2018-02-13 21:51:08.000000 hepcrawl-9.0.9/pytest.ini
+-rw-rw-r--   0 travis    (2000) travis    (2000)      594 2018-02-13 21:54:29.000000 hepcrawl-9.0.9/AUTHORS
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/hepcrawl.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        9 2018-02-13 21:54:29.000000 hepcrawl-9.0.9/hepcrawl.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-02-13 21:54:29.000000 hepcrawl-9.0.9/hepcrawl.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1129 2018-02-13 21:54:29.000000 hepcrawl-9.0.9/hepcrawl.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2601 2018-02-13 21:54:29.000000 hepcrawl-9.0.9/hepcrawl.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-02-13 21:54:29.000000 hepcrawl-9.0.9/hepcrawl.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       39 2018-02-13 21:54:29.000000 hepcrawl-9.0.9/hepcrawl.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7038 2018-02-13 21:54:30.000000 hepcrawl-9.0.9/hepcrawl.egg-info/SOURCES.txt
```

### Comparing `hepcrawl-9.0.8/docs/contributing.rst` & `hepcrawl-9.0.9/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/docs/index.rst` & `hepcrawl-9.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/docs/Makefile` & `hepcrawl-9.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/docs/license.rst` & `hepcrawl-9.0.9/docs/license.rst`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/docs/spiders.rst` & `hepcrawl-9.0.9/docs/spiders.rst`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/docs/overview.rst` & `hepcrawl-9.0.9/docs/overview.rst`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/docs/guide.rst` & `hepcrawl-9.0.9/docs/guide.rst`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/docs/operations.rst` & `hepcrawl-9.0.9/docs/operations.rst`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/docs/conf.py` & `hepcrawl-9.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/README.rst` & `hepcrawl-9.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/setup.py` & `hepcrawl-9.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/mappings.py` & `hepcrawl-9.0.9/hepcrawl/mappings.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/testlib/celery_monitor.py` & `hepcrawl-9.0.9/hepcrawl/testlib/celery_monitor.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/testlib/tasks.py` & `hepcrawl-9.0.9/hepcrawl/testlib/tasks.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/testlib/scrapyd_coverage_runner.py` & `hepcrawl-9.0.9/hepcrawl/testlib/scrapyd_coverage_runner.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/testlib/fixtures.py` & `hepcrawl-9.0.9/hepcrawl/testlib/fixtures.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/testlib/utils.py` & `hepcrawl-9.0.9/hepcrawl/testlib/utils.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/settings.py` & `hepcrawl-9.0.9/hepcrawl/settings.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/tohep.py` & `hepcrawl-9.0.9/hepcrawl/tohep.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/inputs.py` & `hepcrawl-9.0.9/hepcrawl/inputs.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/dateutils.py` & `hepcrawl-9.0.9/hepcrawl/dateutils.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/pipelines.py` & `hepcrawl-9.0.9/hepcrawl/pipelines.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/scrapyd.cfg` & `hepcrawl-9.0.9/hepcrawl/scrapyd.cfg`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/outputs.py` & `hepcrawl-9.0.9/hepcrawl/outputs.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/__init__.py` & `hepcrawl-9.0.9/hepcrawl/__init__.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/downloaders.py` & `hepcrawl-9.0.9/hepcrawl/downloaders.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/middlewares.py` & `hepcrawl-9.0.9/hepcrawl/middlewares.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/version.py` & `hepcrawl-9.0.9/hepcrawl/version.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/extensions.py` & `hepcrawl-9.0.9/hepcrawl/extensions.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/extractors/jats.py` & `hepcrawl-9.0.9/hepcrawl/extractors/jats.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/extractors/nlm.py` & `hepcrawl-9.0.9/hepcrawl/extractors/nlm.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/scrapy.cfg` & `hepcrawl-9.0.9/hepcrawl/scrapy.cfg`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/items.py` & `hepcrawl-9.0.9/hepcrawl/items.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/utils.py` & `hepcrawl-9.0.9/hepcrawl/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,15 +402,15 @@
 
     Returns:
         function: method which will disallow any keyword arguments that
             do not begin with an underscore sign.
     """
     argspec = inspect.getargspec(func)
     defined_arguments = argspec.args[1:]
-    spider_fields = ['settings']
+    spider_fields = ['settings', 'crawler_settings']
 
     allowed_arguments = defined_arguments + spider_fields
 
     @wraps(func)
     def wrapper(self, *args, **kwargs):
         disallowed_kwargs = [
             key for key in kwargs
```

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/brown_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/brown_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/hindawi_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/hindawi_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/common/last_run_store.py` & `hepcrawl-9.0.9/hepcrawl/spiders/common/last_run_store.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/common/oaipmh_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/common/oaipmh_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/aps_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/aps_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/cds_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/cds_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/elsevier_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/elsevier_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/magic_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/magic_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/phenix_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/phenix_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/base_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/base_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/t2k_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/t2k_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/phil_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/phil_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/infn_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/infn_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/__init__.py` & `hepcrawl-9.0.9/hepcrawl/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/mit_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/mit_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/edp_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/edp_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/iop_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/iop_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/wsp_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/wsp_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/arxiv_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/arxiv_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/pos_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/pos_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/dnb_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/dnb_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/desy_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/desy_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/spiders/alpha_spider.py` & `hepcrawl-9.0.9/hepcrawl/spiders/alpha_spider.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/loaders.py` & `hepcrawl-9.0.9/hepcrawl/loaders.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl/parsers/jats.py` & `hepcrawl-9.0.9/hepcrawl/parsers/jats.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/CHANGELOG` & `hepcrawl-9.0.9/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+* 9.0.9 "Jacopo Notarstefano <jacopo.notarstefano@gmail.com>"
+    MINOR f509bc37: Merge pull request #225 from
+    david-caro/whitelist_crawler_settings
+    MINOR 018c3f34: utils.strict_kwargs: whitelist crawler_settings pram
+    MINOR 811c1cac: tests: add test for crawler_settings whitelist
+
 * 9.0.8 "David Caro <david@dcaro.es>"
     MINOR 72988427: Merge pull request #224 from david-caro/fix_travis_deploy
     MINOR 60f2ab51: travis: deploy only on one of the test suites
 
 * 9.0.7 "Harris Tzovanakis <me@drjova.com>"
     MINOR 38003b98: Merge pull request #223 from Glignos/catch_faulty_records
     MINOR 9c215a9a: removed attached schema from record
@@ -181,15 +187,14 @@
     FEATURE 1a53584b: pipelines: added extra debug log
     FEATURE a82a158f: global: add `CRAWL_ONCE_PATH` to settings
     FEATURE 28a2603c: testlib: refactored `clean_dir` default arguments
     FEATURE bcf8f76f: tohep: add some useful debug logs
     FEATURE 026bdfb9: tests: add `clean_dir` to tests that using the DB
     FEATURE a283b21a: tests: support for `scrapy-crawl-once`
     FEATURE 1ac8785f: setup: pin scrapy-crawl-once to the major version
-    FEATURE 7694fe37: middlewares: add support for crawling only once
     FEATURE a7588190: wsp: add temporary folder to the crawlings
     FEATURE f111993c: celery_monitor: small refactor and default event fix
     FEATURE 6dffdc8c: tests: remove unneeded var dir chown
     FEATURE b509c82b: pipelines: minor fix
     FEATURE 5aacb1ce: middlewares: use better key for crawl-once
     FEATURE 3110b0f9: desy: adapt to the new middleware
     FEATURE 6ffa2df6: unit: small pep8 refactor
@@ -309,67 +314,58 @@
     MAJOR 5c6b039a: Merge pull request #140 from
     spirosdelviniotis/hepcrawl_upgrade_schemas_34_3
     MAJOR 5fb49a2c: tests: adapt functional tests to latest `schemas`
     MAJOR bc6e79c3: wsp: support latest `inspire-schemas`
     MAJOR 9501bd64: setup: upgrade `inspire-schemas` to latest version
     MAJOR 9411978b: tests: adapt unit tests to latest `inspire-schemas`
 
-* 0.0.9 "David Caro <david@dcaro.es>"
+* 0.0.8 "David Caro <david@dcaro.es>"
     MINOR 73adb254: Merge pull request #142 from
     spirosdelviniotis/hepcrawl_pin_setuptools_version
     MINOR a1bfdc83: docker_entrypoint: pin setuptools to `<36`
 
-* 0.0.8 "David Caro <david@dcaro.es>"
+* 0.0.7 "David Caro <david@dcaro.es>"
     MINOR 36c90217: Merge pull request #135 from
     spirosdelviniotis/hepcrawl_arxiv_functional_tests
     MINOR 56063d50: tests: add arxiv functional test to docker-compose
     MINOR 3ffd527a: gitignore: add auto-generated files from tests
     MINOR feb94e3f: tests: refactored `docker-compose.test.yml`
     MINOR 9773d225: tests: add arxiv functional test
 
-* 0.0.7 "David Caro <david@dcaro.es>"
+* 0.0.6 "David Caro <david@dcaro.es>"
     MINOR 15702bd3: Merge pull request #136 from
     spirosdelviniotis/hepcrawl_bug_source_130
-    MINOR dd556857: crawler2hep: pass `source` to `LiteratureBuilder`
     MINOR bc179ba5: pipelines: populate `acquisition_source.source`
-    MINOR 4539ca4c: tests: check `source` field for pipeline unit test
-    MINOR 2c90d80f: tests: check `source` field for wsp unit tests
     MINOR 116f7ad5: arxiv: add `source` to `report_numbers`
+    MINOR 4539ca4c: tests: check `source` field for pipeline unit test
+    MINOR dd556857: crawler2hep: pass `source` to `LiteratureBuilder`
     MINOR 844b2216: tests: check `source` field for pos unit tests
 
-* 0.0.6 "David Caro <david@dcaro.es>"
+* 0.0.5 "David Caro <david@dcaro.es>"
     MINOR c3abf763: Merge pull request #129 from
     spirosdelviniotis/hepcrawl_migrate_to_google_doc_style
     MINOR 87a9ec61: items: migrate to google style docstrings
-    MINOR e2803515: utils: migrate to google style docstrings
     MINOR 0fdcf5f7: loaders: migrate to google style docstrings
     MINOR 98ab2073: outputs: migrate to google style docstrings
     MINOR 3022766a: inputs: migrate to google style docstrings
 
-* 0.0.5 "David Caro <david@dcaro.es>"
+* 0.0.4 "David Caro <david@dcaro.es>"
     MINOR c471f61f: Merge pull request #132 from
     spirosdelviniotis/hepcrawl_move_reusable_functions_to_testlib
     MINOR ce56129f: tests: refactor `wsp` functional test
     MINOR bceb8fdb: tests: use `get_test_suite_path`
-    MINOR d15f91b8: tests: refactor `expected_results`
     MINOR a1900068: tests: rename `WSP` test folder
 
-* 0.0.4 "David Caro <david@dcaro.es>"
+* 0.0.3 "David Caro <david@dcaro.es>"
     MINOR df63cb32: Merge pull request #126 from
     spirosdelviniotis/hepcrawl_support_google_style_docstring
-    MINOR bd1b9b91: global: small fixes for sphinx-apidoc
     MINOR 158e324b: docs: add api doc and use the previous spiders doc
     MINOR 1361e3b9: gitignore: add docs/_source folder to .gitignore
 
-* 0.0.3 "David Caro <david@dcaro.es>"
+* 0.0.2 "David Caro <david@dcaro.es>"
     MINOR 4c1c8727: Merge pull request #122 from
     spirosdelviniotis/hepcrawl_docker_non_root
     MINOR b7208f97: docker: add user non root
 
-* 0.0.2 "David Caro <david@dcaro.es>"
+* 0.0.1 "David Caro <david@dcaro.es>"
     MINOR 7b05ad4d: Merge pull request #124 from
     spirosdelviniotis/hepcrawl_remove_doc_service
-    MINOR 5ecf4797: docker-compose: remove unused doc service
-
-* 0.0.1 "David Caro <david@dcaro.es>"
-    MINOR a743ce6b: Merge pull request #108 from
-    spirosdelviniotis/hepcrawl_uniform_future_imports
```

### Comparing `hepcrawl-9.0.8/LICENSE` & `hepcrawl-9.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/INSTALL.rst` & `hepcrawl-9.0.9/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/wsp/fixtures/ftp_server/WSP/IDAQPv20i01-03160015-1510863.zip` & `hepcrawl-9.0.9/tests/functional/wsp/fixtures/ftp_server/WSP/IDAQPv20i01-03160015-1510863.zip`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/wsp/fixtures/wsp_smoke_records.json` & `hepcrawl-9.0.9/tests/functional/wsp/fixtures/wsp_smoke_records.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/wsp/test_wsp.py` & `hepcrawl-9.0.9/tests/functional/wsp/test_wsp.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/arxiv/test_arxiv.py` & `hepcrawl-9.0.9/tests/functional/arxiv/test_arxiv.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/arxiv/fixtures/arxiv_expected.json` & `hepcrawl-9.0.9/tests/functional/arxiv/fixtures/arxiv_expected.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/arxiv/fixtures/http_server/records/arxiv-physics-hep-ex.xml` & `hepcrawl-9.0.9/tests/functional/arxiv/fixtures/http_server/records/arxiv-physics-hep-ex.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/arxiv/fixtures/http_server/records/arxiv-physics-hep-th.xml` & `hepcrawl-9.0.9/tests/functional/arxiv/fixtures/http_server/records/arxiv-physics-hep-th.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/pos/test_pos.py` & `hepcrawl-9.0.9/tests/functional/pos/test_pos.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/pos/fixtures/oai_harvested/pos_record.xml` & `hepcrawl-9.0.9/tests/functional/pos/fixtures/oai_harvested/pos_record.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/pos/fixtures/pos_conference_proceedings_records.json` & `hepcrawl-9.0.9/tests/functional/pos/fixtures/pos_conference_proceedings_records.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/pos/fixtures/https_server/records/PoS(LATTICE 2013)001.html` & `hepcrawl-9.0.9/tests/functional/pos/fixtures/https_server/records/PoS(LATTICE 2013)001.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/pos/fixtures/https_server/records/187.html` & `hepcrawl-9.0.9/tests/functional/pos/fixtures/https_server/records/187.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/desy/fixtures/ftp_server/DESY/desy_collection_records.xml` & `hepcrawl-9.0.9/tests/functional/desy/fixtures/ftp_server/DESY/desy_collection_records.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/desy/fixtures/desy_records_ftp_expected.json` & `hepcrawl-9.0.9/tests/functional/desy/fixtures/desy_records_ftp_expected.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/desy/fixtures/desy_records_local_expected.json` & `hepcrawl-9.0.9/tests/functional/desy/fixtures/desy_records_local_expected.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/desy/test_desy.py` & `hepcrawl-9.0.9/tests/functional/desy/test_desy.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/cds/fixtures/oai_harvested/cds_smoke_records.xml` & `hepcrawl-9.0.9/tests/functional/cds/fixtures/oai_harvested/cds_smoke_records.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/cds/fixtures/cds_smoke_records_expected.json` & `hepcrawl-9.0.9/tests/functional/cds/fixtures/cds_smoke_records_expected.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/functional/cds/test_cds.py` & `hepcrawl-9.0.9/tests/functional/cds/test_cds.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_testlib_utils.py` & `hepcrawl-9.0.9/tests/unit/test_testlib_utils.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_iop.py` & `hepcrawl-9.0.9/tests/unit/test_iop.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_pos.py` & `hepcrawl-9.0.9/tests/unit/test_pos.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_t2k.py` & `hepcrawl-9.0.9/tests/unit/test_t2k.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_phil.py` & `hepcrawl-9.0.9/tests/unit/test_phil.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_extensions.py` & `hepcrawl-9.0.9/tests/unit/test_extensions.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_aps.py` & `hepcrawl-9.0.9/tests/unit/test_aps.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_mit.py` & `hepcrawl-9.0.9/tests/unit/test_mit.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_dateutils.py` & `hepcrawl-9.0.9/tests/unit/test_dateutils.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_phenix.py` & `hepcrawl-9.0.9/tests/unit/test_phenix.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_world_scientific.py` & `hepcrawl-9.0.9/tests/unit/test_world_scientific.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/elsevier/sample_consyn_record.xml` & `hepcrawl-9.0.9/tests/unit/responses/elsevier/sample_consyn_record.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/elsevier/fake_astropart.zip` & `hepcrawl-9.0.9/tests/unit/responses/elsevier/fake_astropart.zip`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/elsevier/fake_nima.zip` & `hepcrawl-9.0.9/tests/unit/responses/elsevier/fake_nima.zip`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/hindawi/test_1.xml` & `hepcrawl-9.0.9/tests/unit/responses/hindawi/test_1.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/brown/test_1.json` & `hepcrawl-9.0.9/tests/unit/responses/brown/test_1.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/brown/test_splash.html` & `hepcrawl-9.0.9/tests/unit/responses/brown/test_splash.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/mit/test_splash.html` & `hepcrawl-9.0.9/tests/unit/responses/mit/test_splash.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/mit/test_list.html` & `hepcrawl-9.0.9/tests/unit/responses/mit/test_list.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/iop/xml/test_standard.xml` & `hepcrawl-9.0.9/tests/unit/responses/iop/xml/test_standard.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/iop/packages/test.tar.gz` & `hepcrawl-9.0.9/tests/unit/responses/iop/packages/test.tar.gz`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/iop/pdf/test_143_3_336.pdf` & `hepcrawl-9.0.9/tests/unit/responses/iop/pdf/test_143_3_336.pdf`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/t2k/001.html` & `hepcrawl-9.0.9/tests/unit/responses/t2k/001.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/t2k/test_1_nourl.html` & `hepcrawl-9.0.9/tests/unit/responses/t2k/test_1_nourl.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/t2k/test_1.html` & `hepcrawl-9.0.9/tests/unit/responses/t2k/test_1.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record2.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record2.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record5.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record5.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record10_parsed.json` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record10_parsed.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record4.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record4.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record8.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record8.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record1.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record1.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record3.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record3.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record6.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record6.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record10.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record10.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record7.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record7.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record0.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record0.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/arxiv/sample_arxiv_record9.xml` & `hepcrawl-9.0.9/tests/unit/responses/arxiv/sample_arxiv_record9.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/pos/sample_splash_page.html` & `hepcrawl-9.0.9/tests/unit/responses/pos/sample_splash_page.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/pos/sample_pos_record.xml` & `hepcrawl-9.0.9/tests/unit/responses/pos/sample_pos_record.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/pos/sample_proceedings_page.html` & `hepcrawl-9.0.9/tests/unit/responses/pos/sample_proceedings_page.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/base/test_1_splash.htm` & `hepcrawl-9.0.9/tests/unit/responses/base/test_1_splash.htm`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/base/test_1.xml` & `hepcrawl-9.0.9/tests/unit/responses/base/test_1.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/world_scientific/wsp_record.xml` & `hepcrawl-9.0.9/tests/unit/responses/world_scientific/wsp_record.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/world_scientific/sample_ws_record.xml` & `hepcrawl-9.0.9/tests/unit/responses/world_scientific/sample_ws_record.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/alpha/test_1.htm` & `hepcrawl-9.0.9/tests/unit/responses/alpha/test_1.htm`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/phil/test_journal.json` & `hepcrawl-9.0.9/tests/unit/responses/phil/test_journal.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/phil/test_thesis.json` & `hepcrawl-9.0.9/tests/unit/responses/phil/test_thesis.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/desy/faulty_record.xml` & `hepcrawl-9.0.9/tests/unit/responses/desy/faulty_record.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/desy/desy_record_expected.json` & `hepcrawl-9.0.9/tests/unit/responses/desy/desy_record_expected.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/desy/desy_collection_records_expected.json` & `hepcrawl-9.0.9/tests/unit/responses/desy/desy_collection_records_expected.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/desy/desy_collection_records.xml` & `hepcrawl-9.0.9/tests/unit/responses/desy/desy_collection_records.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/desy/desy_record.xml` & `hepcrawl-9.0.9/tests/unit/responses/desy/desy_record.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/infn/test_1.html` & `hepcrawl-9.0.9/tests/unit/responses/infn/test_1.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/infn/test_1_nolink.html` & `hepcrawl-9.0.9/tests/unit/responses/infn/test_1_nolink.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/infn/test_splash.html` & `hepcrawl-9.0.9/tests/unit/responses/infn/test_splash.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/edp/jats_splash.html` & `hepcrawl-9.0.9/tests/unit/responses/edp/jats_splash.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/edp/test_gz.tar.gz` & `hepcrawl-9.0.9/tests/unit/responses/edp/test_gz.tar.gz`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/edp/jats.xml` & `hepcrawl-9.0.9/tests/unit/responses/edp/jats.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/edp/rich.xml` & `hepcrawl-9.0.9/tests/unit/responses/edp/rich.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/edp/rich_splash.html` & `hepcrawl-9.0.9/tests/unit/responses/edp/rich_splash.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/edp/test_rich.tar.bz2` & `hepcrawl-9.0.9/tests/unit/responses/edp/test_rich.tar.bz2`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/magic/test_1.html` & `hepcrawl-9.0.9/tests/unit/responses/magic/test_1.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/magic/test_splash.html` & `hepcrawl-9.0.9/tests/unit/responses/magic/test_splash.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/magic/test_list.html` & `hepcrawl-9.0.9/tests/unit/responses/magic/test_list.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/aps/aps_single_parsed.json` & `hepcrawl-9.0.9/tests/unit/responses/aps/aps_single_parsed.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/aps/PhysRevX.7.021022.xml` & `hepcrawl-9.0.9/tests/unit/responses/aps/PhysRevX.7.021022.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/aps/PhysRevX.4.021018.xml` & `hepcrawl-9.0.9/tests/unit/responses/aps/PhysRevX.4.021018.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/aps/PhysRevD.96.095036.xml` & `hepcrawl-9.0.9/tests/unit/responses/aps/PhysRevD.96.095036.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/aps/aps_single_response.json` & `hepcrawl-9.0.9/tests/unit/responses/aps/aps_single_response.json`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/dnb/test_splash.html` & `hepcrawl-9.0.9/tests/unit/responses/dnb/test_splash.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/dnb/test_1.xml` & `hepcrawl-9.0.9/tests/unit/responses/dnb/test_1.xml`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/responses/phenix/test_1.html` & `hepcrawl-9.0.9/tests/unit/responses/phenix/test_1.html`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_arxiv_single.py` & `hepcrawl-9.0.9/tests/unit/test_arxiv_single.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_brown.py` & `hepcrawl-9.0.9/tests/unit/test_brown.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_hindawi.py` & `hepcrawl-9.0.9/tests/unit/test_hindawi.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_infn.py` & `hepcrawl-9.0.9/tests/unit/test_infn.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_edp.py` & `hepcrawl-9.0.9/tests/unit/test_edp.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_magic.py` & `hepcrawl-9.0.9/tests/unit/test_magic.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_parsers_jats.py` & `hepcrawl-9.0.9/tests/unit/test_parsers_jats.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_utils.py` & `hepcrawl-9.0.9/tests/unit/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,21 +279,22 @@
 def test_strict_kwargs_pass():
     """Test the `strict_kwargs` decorator allowing the kwargs."""
     dummy = Dummy(
         good1_no_default=1,
         good2=2,
         good3=None,
         _private=4,
-        settings={'DUMMY': True}
+        settings={'DUMMY': True},
+        crawler_settings={'DUMMY': True},
     )
     assert callable(dummy.__init__)
     assert dummy.good1_no_default == 1
     assert dummy.good2 == 2
     assert dummy.good3 == None
     assert dummy.good4 == 30
-    assert dummy.kwargs == {'_private': 4, 'settings': {'DUMMY': True}}
+    assert dummy.kwargs == {'_private': 4, 'settings': {'DUMMY': True}, 'crawler_settings': {'DUMMY': True}}
 
 
 def test_strict_kwargs_fail():
     """Test the `strict_kwargs` decorator disallowing some kwargs."""
     with pytest.raises(TypeError):
         Dummy(**{'good1_no_default': 1, 'good2': 2, u'bąd_þärãm': 4})
```

### Comparing `hepcrawl-9.0.8/tests/unit/test_inputs.py` & `hepcrawl-9.0.9/tests/unit/test_inputs.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_desy.py` & `hepcrawl-9.0.9/tests/unit/test_desy.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_oaipmh.py` & `hepcrawl-9.0.9/tests/unit/test_oaipmh.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_tohep.py` & `hepcrawl-9.0.9/tests/unit/test_tohep.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_arxiv_all.py` & `hepcrawl-9.0.9/tests/unit/test_arxiv_all.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_alpha.py` & `hepcrawl-9.0.9/tests/unit/test_alpha.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_base.py` & `hepcrawl-9.0.9/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_elsevier.py` & `hepcrawl-9.0.9/tests/unit/test_elsevier.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_pipelines.py` & `hepcrawl-9.0.9/tests/unit/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/data/test.zip` & `hepcrawl-9.0.9/tests/unit/data/test.zip`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/tests/unit/test_dnb.py` & `hepcrawl-9.0.9/tests/unit/test_dnb.py`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/MANIFEST.in` & `hepcrawl-9.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/PKG-INFO` & `hepcrawl-9.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hepcrawl
-Version: 9.0.8
+Version: 9.0.9
 Summary: Scrapy project for feeds into INSPIRE-HEP (http://inspirehep.net).
 Home-page: https://github.com/inspirehep/hepcrawl
 Author: CERN
 Author-email: admin@inspirehep.net
 License: UNKNOWN
 Description-Content-Type: UNKNOWN
 Description: ..
```

### Comparing `hepcrawl-9.0.8/RELEASE-NOTES.rst` & `hepcrawl-9.0.9/RELEASE-NOTES.rst`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/AUTHORS` & `hepcrawl-9.0.9/AUTHORS`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Chris Aslanoglou <chris.aslanoglou@gmail.com>
 David Caro <david@dcaro.es>
 Glignos <glignos93@gmail.com>
 Harris Tzovanakis <me@drjova.com>
 Iuliana Voinea <iuliana.voinea@student.manchester.ac.uk>
+Jacopo Notarstefano <jacopo.notarstefano@gmail.com>
 Micha Moskovic <michamos@gmail.com>
 Samuele Kaplun <Samuele.Kaplun@cern.ch>
 Samuele Kaplun <samuele.kaplun@cern.ch>
 Spiros Delviniotis <spirosdelviniotis@gmail.com>
 Spiros Delviniotis <spyridon.delviniotis@cern.ch>
 Spyridon Delviniotis <spirosdelviniotis@gmail.com>
 Szymon Łopaciuk <szymon.lopaciuk@cern.ch>
```

### Comparing `hepcrawl-9.0.8/hepcrawl.egg-info/requires.txt` & `hepcrawl-9.0.9/hepcrawl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hepcrawl-9.0.8/hepcrawl.egg-info/PKG-INFO` & `hepcrawl-9.0.9/hepcrawl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: hepcrawl
-Version: 9.0.8
+Version: 9.0.9
 Summary: Scrapy project for feeds into INSPIRE-HEP (http://inspirehep.net).
 Home-page: https://github.com/inspirehep/hepcrawl
 Author: CERN
 Author-email: admin@inspirehep.net
 License: UNKNOWN
 Description-Content-Type: UNKNOWN
 Description: ..
```

### Comparing `hepcrawl-9.0.8/hepcrawl.egg-info/SOURCES.txt` & `hepcrawl-9.0.9/hepcrawl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

