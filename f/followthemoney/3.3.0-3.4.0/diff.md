# Comparing `tmp/followthemoney-3.3.0.tar.gz` & `tmp/followthemoney-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "followthemoney-3.3.0.tar", last modified: Fri Feb 10 14:28:43 2023, max compression
+gzip compressed data, was "followthemoney-3.4.0.tar", last modified: Tue May 23 06:19:57 2023, max compression
```

## Comparing `followthemoney-3.3.0.tar` & `followthemoney-3.4.0.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.192974 followthemoney-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-02-10 14:26:53.000000 followthemoney-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-02-10 14:26:53.000000 followthemoney-3.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-02-10 14:28:43.192974 followthemoney-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-02-10 14:26:53.000000 followthemoney-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.180974 followthemoney-3.3.0/followthemoney/
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.180974 followthemoney-3.3.0/followthemoney/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/cli/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/cli/exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/cli/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/cli/sieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.180974 followthemoney-3.3.0/followthemoney/export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/export/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/export/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/export/excel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/export/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/export/neo4j.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/export/rdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.180974 followthemoney-3.3.0/followthemoney/mapping/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/mapping/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/mapping/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/mapping/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/mapping/query.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/mapping/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/mapping/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/namespace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/offshore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/ontology.py
--rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/property.py
--rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/rdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.188974 followthemoney-3.3.0/followthemoney/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Address.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Airplane.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Analyzable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Article.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Assessment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Asset.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Associate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Audio.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/BankAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Call.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/CallForTenders.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Company.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Contract.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/ContractAward.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/CourtCase.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/CourtCaseParty.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/CryptoWallet.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Debt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Directorship.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Document.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Documentation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/EconomicActivity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Email.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Employment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Event.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Family.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Folder.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/HyperText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Identification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Interest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Interval.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/LegalEntity.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/License.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Membership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Mention.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Message.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Note.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Organization.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Ownership.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Package.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Page.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Pages.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Passport.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Payment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Person.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/PlainText.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Post.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Project.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/ProjectParticipant.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/PublicBody.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/RealEstate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Representation.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Sanction.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Security.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Similar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Succession.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Table.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/TaxRoll.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Thing.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Trip.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/UnknownLink.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/UserAccount.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Value.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Vehicle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Vessel.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Video.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema/Workbook.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.188974 followthemoney-3.3.0/followthemoney/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.176974 followthemoney-3.3.0/followthemoney/translations/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.188974 followthemoney-3.3.0/followthemoney/translations/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    39021 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   110484 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.176974 followthemoney-3.3.0/followthemoney/translations/bs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.188974 followthemoney-3.3.0/followthemoney/translations/bs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.176974 followthemoney-3.3.0/followthemoney/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.188974 followthemoney-3.3.0/followthemoney/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    36742 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   105691 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.176974 followthemoney-3.3.0/followthemoney/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.188974 followthemoney-3.3.0/followthemoney/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    32360 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   104328 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.188974 followthemoney-3.3.0/followthemoney/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.188974 followthemoney-3.3.0/followthemoney/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    43316 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   109418 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/fr/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)    99827 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.176974 followthemoney-3.3.0/followthemoney/translations/nb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.188974 followthemoney-3.3.0/followthemoney/translations/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.176974 followthemoney-3.3.0/followthemoney/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.192974 followthemoney-3.3.0/followthemoney/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.176974 followthemoney-3.3.0/followthemoney/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.192974 followthemoney-3.3.0/followthemoney/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.192974 followthemoney-3.3.0/followthemoney/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.192974 followthemoney-3.3.0/followthemoney/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    61028 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)   131321 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
--rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/ru/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.176974 followthemoney-3.3.0/followthemoney/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.192974 followthemoney-3.3.0/followthemoney/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
--rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.192974 followthemoney-3.3.0/followthemoney/types/
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/address.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/checksum.py
--rw-r--r--   0 runner    (1001) docker     (123)     9573 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/email.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/gender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/iban.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/mimetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/phone.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/types/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-02-10 14:26:53.000000 followthemoney-3.3.0/followthemoney/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-10 14:28:43.180974 followthemoney-3.3.0/followthemoney.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-02-10 14:28:43.000000 followthemoney-3.3.0/followthemoney.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-02-10 14:28:43.000000 followthemoney-3.3.0/followthemoney.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:28:43.000000 followthemoney-3.3.0/followthemoney.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-02-10 14:28:43.000000 followthemoney-3.3.0/followthemoney.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:28:43.000000 followthemoney-3.3.0/followthemoney.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-10 14:28:25.000000 followthemoney-3.3.0/followthemoney.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-02-10 14:28:43.000000 followthemoney-3.3.0/followthemoney.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-10 14:28:43.000000 followthemoney-3.3.0/followthemoney.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-10 14:28:43.196974 followthemoney-3.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-02-10 14:26:53.000000 followthemoney-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.251635 followthemoney-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-23 06:18:02.000000 followthemoney-3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-23 06:18:02.000000 followthemoney-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-23 06:19:57.251635 followthemoney-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-23 06:18:02.000000 followthemoney-3.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.235635 followthemoney-3.4.0/followthemoney/
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.235635 followthemoney-3.4.0/followthemoney/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/sieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.235635 followthemoney-3.4.0/followthemoney/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/excel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/export/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10847 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.235635 followthemoney-3.4.0/followthemoney/mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4579 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/mapping/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/offshore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6790 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19523 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/rdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.243635 followthemoney-3.4.0/followthemoney/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Address.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Airplane.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Analyzable.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Article.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Assessment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Asset.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Associate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Audio.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/BankAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Call.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/CallForTenders.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Company.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Contract.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/ContractAward.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/CourtCase.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/CourtCaseParty.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/CryptoWallet.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Debt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Directorship.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Document.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Documentation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/EconomicActivity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Email.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Employment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Event.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Family.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Folder.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/HyperText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Identification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Interest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Interval.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/LegalEntity.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/License.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Membership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Mention.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Message.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Note.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Organization.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Ownership.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Package.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Page.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Pages.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Passport.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Payment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Person.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/PlainText.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Post.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Project.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/ProjectParticipant.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/PublicBody.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/RealEstate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Representation.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Sanction.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Security.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Similar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Succession.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Table.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/TaxRoll.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Thing.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Trip.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/UnknownLink.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/UserAccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Value.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Vehicle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Vessel.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Video.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema/Workbook.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    16362 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.243635 followthemoney-3.4.0/followthemoney/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.243635 followthemoney-3.4.0/followthemoney/translations/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    39021 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   110484 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/bs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.243635 followthemoney-3.4.0/followthemoney/translations/bs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    93147 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.243635 followthemoney-3.4.0/followthemoney/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    36742 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   105691 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    32360 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   104328 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    43316 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   109418 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   106802 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/fr/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)    99827 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/nb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89796 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    90876 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89847 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    61028 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)   131500 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po
+-rw-r--r--   0 runner    (1001) docker     (123)   130621 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/ru/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.231635 followthemoney-3.4.0/followthemoney/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.247635 followthemoney-3.4.0/followthemoney/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    89829 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.251635 followthemoney-3.4.0/followthemoney/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/gender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/iban.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/mimetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/phone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/types/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-05-23 06:18:02.000000 followthemoney-3.4.0/followthemoney/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:19:57.235635 followthemoney-3.4.0/followthemoney.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:19:34.000000 followthemoney-3.4.0/followthemoney.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 06:19:57.000000 followthemoney-3.4.0/followthemoney.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 06:19:57.251635 followthemoney-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-05-23 06:18:02.000000 followthemoney-3.4.0/setup.py
```

### Comparing `followthemoney-3.3.0/LICENSE` & `followthemoney-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/PKG-INFO` & `followthemoney-3.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.3.0
-Summary: UNKNOWN
+Version: 3.4.0
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
-Description: # Follow the Money
-        
-        [![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
-        
-        This repository contains a pragmatic data model for the entities most
-        commonly used in investigative reporting: people, companies, assets,
-        payments, court cases, etc.
-        
-        The purpose of this is not to model reality in an ideal data model, but
-        rather to have a working data structure for researchers.
-        
-        `followthemoney` also contains code used to validate and normalize many
-        of the elements of data, and to map tabular data into the model.
-        
-        ## Documentation
-        
-        For a general introduction to `followthemoney`, check the high-level introduction:
-        
-        * https://followthemoney.tech
-        
-        Part of this package is a command-line tool that can be used to process and
-        transform data in various ways. You can find a tutorial here:
-        
-        * https://followthemoney.tech/docs/cli/
-        
-        Besides the introductions, there is also a full reference documentation for the
-        library and the contained ontology: 
-        
-        * https://followthemoney.tech/explorer/
-        
-        There's also a number of viewers for the RDF schema definitions generated
-        from FollowTheMoney, e.g.:
-        
-        * [LODE documentation](http://150.146.207.114/lode/extract?url=https%3A%2F%2Falephdata.github.io%2Ffollowthemoney%2Fns%2Fftm.xml&owlapi=true&imported=true&lang=en)
-        * [WebVOWL](https://service.tib.eu/webvowl/#iri=https://alephdata.github.io/followthemoney/ns/ftm.xml)
-        * RDF/OWL specification in [XML](https://alephdata.github.io/followthemoney/ns/ftm.xml).
-        
-        ## Development environment
-        
-        For local development with a virtualenv:
-        
-        ```bash
-        python3 -mvenv .env
-        source .env/bin/activate
-        pip install -e ".[dev]"
-        ```
-        
-        Now you can run the tests with
-        
-        ```bash
-        make test
-        ```
-        
-        ## Releasing
-        
-        We release a lot of version of `followthemoney` because even small changes
-        to the code base require a pypi release to begin being used in `aleph`. To
-        this end, here's the steps for making a release:
-        
-        ```bash
-        git pull --rebase
-        make build
-        make test
-        git add . && git commit -m "Updating translation files"
-        bumpversion patch
-        git push --atomic origin main $(git describe --tags --abbrev=0)
-        ```
-        
-        This will create a new patch release and upload a distribution of it. If
-        the changes are more significant, you can run `bumpversion` with the `minor`
-        or `major` arguments.
-        
-        When the schema is updated, please update the docs, ideally including the
-        diagrams. For the RDF namespace and JavaScript version of the model, 
-        run `make generate`.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# Follow the Money
+
+[![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
+
+This repository contains a pragmatic data model for the entities most
+commonly used in investigative reporting: people, companies, assets,
+payments, court cases, etc.
+
+The purpose of this is not to model reality in an ideal data model, but
+rather to have a working data structure for researchers.
+
+`followthemoney` also contains code used to validate and normalize many
+of the elements of data, and to map tabular data into the model.
+
+## Documentation
+
+For a general introduction to `followthemoney`, check the high-level introduction:
+
+* https://followthemoney.tech
+
+Part of this package is a command-line tool that can be used to process and
+transform data in various ways. You can find a tutorial here:
+
+* https://followthemoney.tech/docs/cli/
+
+Besides the introductions, there is also a full reference documentation for the
+library and the contained ontology: 
+
+* https://followthemoney.tech/explorer/
+
+There's also a number of viewers for the RDF schema definitions generated
+from FollowTheMoney, e.g.:
+
+* [LODE documentation](http://150.146.207.114/lode/extract?url=https%3A%2F%2Falephdata.github.io%2Ffollowthemoney%2Fns%2Fftm.xml&owlapi=true&imported=true&lang=en)
+* [WebVOWL](https://service.tib.eu/webvowl/#iri=https://alephdata.github.io/followthemoney/ns/ftm.xml)
+* RDF/OWL specification in [XML](https://alephdata.github.io/followthemoney/ns/ftm.xml).
+
+## Development environment
+
+For local development with a virtualenv:
+
+```bash
+python3 -mvenv .env
+source .env/bin/activate
+pip install -e ".[dev]"
+```
+
+Now you can run the tests with
+
+```bash
+make test
+```
+
+## Releasing
+
+We release a lot of version of `followthemoney` because even small changes
+to the code base require a pypi release to begin being used in `aleph`. To
+this end, here's the steps for making a release:
+
+```bash
+git pull --rebase
+make build
+make test
+git add . && git commit -m "Updating translation files"
+bumpversion patch
+git push --atomic origin main $(git describe --tags --abbrev=0)
+```
+
+This will create a new patch release and upload a distribution of it. If
+the changes are more significant, you can run `bumpversion` with the `minor`
+or `major` arguments.
+
+When the schema is updated, please update the docs, ideally including the
+diagrams. For the RDF namespace and JavaScript version of the model, 
+run `make generate`.
```

### Comparing `followthemoney-3.3.0/README.md` & `followthemoney-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/cli/aggregate.py` & `followthemoney-3.4.0/followthemoney/cli/aggregate.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/cli/cli.py` & `followthemoney-3.4.0/followthemoney/cli/cli.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/cli/exports.py` & `followthemoney-3.4.0/followthemoney/cli/exports.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/cli/mapping.py` & `followthemoney-3.4.0/followthemoney/cli/mapping.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/cli/sieve.py` & `followthemoney-3.4.0/followthemoney/cli/sieve.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/cli/util.py` & `followthemoney-3.4.0/followthemoney/cli/util.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/compare.py` & `followthemoney-3.4.0/followthemoney/compare.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/exc.py` & `followthemoney-3.4.0/followthemoney/exc.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/export/common.py` & `followthemoney-3.4.0/followthemoney/export/common.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/export/csv.py` & `followthemoney-3.4.0/followthemoney/export/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/export/excel.py` & `followthemoney-3.4.0/followthemoney/export/excel.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/export/graph.py` & `followthemoney-3.4.0/followthemoney/export/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/export/neo4j.py` & `followthemoney-3.4.0/followthemoney/export/neo4j.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/export/rdf.py` & `followthemoney-3.4.0/followthemoney/export/rdf.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/graph.py` & `followthemoney-3.4.0/followthemoney/graph.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/helpers.py` & `followthemoney-3.4.0/followthemoney/helpers.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/mapping/csv.py` & `followthemoney-3.4.0/followthemoney/mapping/csv.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/mapping/entity.py` & `followthemoney-3.4.0/followthemoney/mapping/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/mapping/property.py` & `followthemoney-3.4.0/followthemoney/mapping/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/mapping/query.py` & `followthemoney-3.4.0/followthemoney/mapping/query.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/mapping/source.py` & `followthemoney-3.4.0/followthemoney/mapping/source.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/mapping/sql.py` & `followthemoney-3.4.0/followthemoney/mapping/sql.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/messages.py` & `followthemoney-3.4.0/followthemoney/messages.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/model.py` & `followthemoney-3.4.0/followthemoney/model.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/namespace.py` & `followthemoney-3.4.0/followthemoney/namespace.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/offshore.py` & `followthemoney-3.4.0/followthemoney/offshore.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/ontology.py` & `followthemoney-3.4.0/followthemoney/ontology.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/property.py` & `followthemoney-3.4.0/followthemoney/property.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/proxy.py` & `followthemoney-3.4.0/followthemoney/proxy.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Address.yaml` & `followthemoney-3.4.0/followthemoney/schema/Address.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Airplane.yaml` & `followthemoney-3.4.0/followthemoney/schema/Airplane.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Analyzable.yaml` & `followthemoney-3.4.0/followthemoney/schema/Analyzable.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Assessment.yaml` & `followthemoney-3.4.0/followthemoney/schema/Assessment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Associate.yaml` & `followthemoney-3.4.0/followthemoney/schema/Associate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/BankAccount.yaml` & `followthemoney-3.4.0/followthemoney/schema/BankAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Call.yaml` & `followthemoney-3.4.0/followthemoney/schema/Call.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/CallForTenders.yaml` & `followthemoney-3.4.0/followthemoney/schema/CallForTenders.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Company.yaml` & `followthemoney-3.4.0/followthemoney/schema/Company.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -54,14 +54,16 @@
       type: identifier
     mbsCode:
       label: "MBS"
       type: identifier
     ibcRuc:
       label: "ibcRUC"
       type: identifier
+      # TODO: Remove this. It's a column name in the ICIJ-released OffshoreLeaks datasets
+      # but seems to just mean "company number".
     caemCode:
       label: "COD CAEM"
       description: "(RO) What kind of activity a legal entity is allowed to develop"
       matchable: false
     kppCode:
       label: "KPP"
       description: "(RU, КПП) in addition to INN for orgs; reason for registration at FNS"
@@ -90,7 +92,14 @@
       label: "PFR Number"
       description: "(RU, ПФР) Pension Fund Registration number. AAA-BBB-CCCCCC, where AAA is organisation region, BBB is district, CCCCCC number at a specific branch"
       type: identifier
     oksmCode:
       label: OKSM
       description: "Russian (ОКСМ) countries classifer"
       matchable: false
+    isinCode:
+      label: ISIN
+      description: International Securities Identification Number
+      type: identifier
+    ticker:
+      label: Stock ticker symbol
+      type: identifier
```

### Comparing `followthemoney-3.3.0/followthemoney/schema/Contract.yaml` & `followthemoney-3.4.0/followthemoney/schema/Contract.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,13 @@
       label: "Status"
     method:
       label: "Procurement method"
     criteria:
       label: Contract award criteria
     classification:
       label: Classification
-      type: text
     cancelled:
       label: "Cancelled?"
     language:
       label: "Language"
       type: language
       rdf: http://purl.org/dc/terms/language
```

### Comparing `followthemoney-3.3.0/followthemoney/schema/ContractAward.yaml` & `followthemoney-3.4.0/followthemoney/schema/ContractAward.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/CourtCase.yaml` & `followthemoney-3.4.0/followthemoney/schema/CourtCase.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/CourtCaseParty.yaml` & `followthemoney-3.4.0/followthemoney/schema/CourtCaseParty.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/CryptoWallet.yaml` & `followthemoney-3.4.0/followthemoney/schema/CryptoWallet.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Debt.yaml` & `followthemoney-3.4.0/followthemoney/schema/Debt.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Directorship.yaml` & `followthemoney-3.4.0/followthemoney/schema/Directorship.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Document.yaml` & `followthemoney-3.4.0/followthemoney/schema/Document.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -107,7 +107,15 @@
         label: "Descendants"
     processingStatus:
       label: "Processing status"
       hidden: true
     processingError:
       label: "Processing error"
       hidden: true
+    processingAgent:
+      label: "Name and version of the processing agent used to process the Document"
+      type: string
+      hidden: true
+    processedAt:
+      label: "Date and time of the most recent ingestion of the Document"
+      type: date
+      matchable: false
```

### Comparing `followthemoney-3.3.0/followthemoney/schema/Documentation.yml` & `followthemoney-3.4.0/followthemoney/schema/Documentation.yml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/EconomicActivity.yaml` & `followthemoney-3.4.0/followthemoney/schema/EconomicActivity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Email.yaml` & `followthemoney-3.4.0/followthemoney/schema/Email.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Employment.yaml` & `followthemoney-3.4.0/followthemoney/schema/Employment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Event.yaml` & `followthemoney-3.4.0/followthemoney/schema/Event.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Family.yaml` & `followthemoney-3.4.0/followthemoney/schema/Family.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Identification.yaml` & `followthemoney-3.4.0/followthemoney/schema/Identification.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Interval.yaml` & `followthemoney-3.4.0/followthemoney/schema/Interval.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/LegalEntity.yaml` & `followthemoney-3.4.0/followthemoney/schema/LegalEntity.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Membership.yaml` & `followthemoney-3.4.0/followthemoney/schema/Membership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Mention.yaml` & `followthemoney-3.4.0/followthemoney/schema/Mention.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Message.yaml` & `followthemoney-3.4.0/followthemoney/schema/Message.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Ownership.yaml` & `followthemoney-3.4.0/followthemoney/schema/Ownership.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Page.yaml` & `followthemoney-3.4.0/followthemoney/schema/Page.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Passport.yaml` & `followthemoney-3.4.0/followthemoney/schema/Passport.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Payment.yaml` & `followthemoney-3.4.0/followthemoney/schema/Payment.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Person.yaml` & `followthemoney-3.4.0/followthemoney/schema/Person.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Post.yaml` & `followthemoney-3.4.0/followthemoney/schema/Post.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/ProjectParticipant.yaml` & `followthemoney-3.4.0/followthemoney/schema/ProjectParticipant.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/RealEstate.yaml` & `followthemoney-3.4.0/followthemoney/schema/RealEstate.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Representation.yaml` & `followthemoney-3.4.0/followthemoney/schema/Representation.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Sanction.yaml` & `followthemoney-3.4.0/followthemoney/schema/Sanction.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Security.yaml` & `followthemoney-3.4.0/followthemoney/schema/Security.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Similar.yaml` & `followthemoney-3.4.0/followthemoney/schema/Similar.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Succession.yaml` & `followthemoney-3.4.0/followthemoney/schema/Succession.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Table.yaml` & `followthemoney-3.4.0/followthemoney/schema/Table.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/TaxRoll.yaml` & `followthemoney-3.4.0/followthemoney/schema/TaxRoll.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Thing.yaml` & `followthemoney-3.4.0/followthemoney/schema/Thing.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Trip.yaml` & `followthemoney-3.4.0/followthemoney/schema/Trip.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/UnknownLink.yaml` & `followthemoney-3.4.0/followthemoney/schema/UnknownLink.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/UserAccount.yaml` & `followthemoney-3.4.0/followthemoney/schema/UserAccount.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Vehicle.yaml` & `followthemoney-3.4.0/followthemoney/schema/Vehicle.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema/Vessel.yaml` & `followthemoney-3.4.0/followthemoney/schema/Vessel.yaml`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/schema.py` & `followthemoney-3.4.0/followthemoney/schema.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/ar/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/bs/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/de/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/es/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/fr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/fr/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/fr/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/messages.pot` & `followthemoney-3.4.0/followthemoney/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/nb/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/nl/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/pt_BR/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo` & `followthemoney-3.4.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.mo`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/ru/LC_MESSAGES/followthemoney.po`

 * *Files 0% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 # jen occrp, 2023
 # 
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2023-01-04 09:58+0100\n"
+"POT-Creation-Date: 2023-02-10 14:09+0100\n"
 "PO-Revision-Date: 2021-05-07 13:11+0000\n"
 "Last-Translator: jen occrp, 2023\n"
 "Language-Team: Russian (https://www.transifex.com/aleph/teams/76591/ru/)\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.11.0\n"
 "Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 
 #: followthemoney/property.py:166
 msgid "Property cannot be written"
 msgstr "Не удалось сохранить свойство"
 
@@ -487,14 +487,24 @@
 msgstr "Банк"
 
 #. BankAccount.properties.accountType.label
 #: followthemoney/schema/BankAccount.yaml
 msgid "Account type"
 msgstr "Тип счёта"
 
+#. BankAccount.properties.openingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Opening date"
+msgstr "Дата открытия"
+
+#. BankAccount.properties.closingDate.label
+#: followthemoney/schema/BankAccount.yaml
+msgid "Closing date"
+msgstr "Дата закрытия"
+
 #. BankAccount.properties.balance.label
 #. CryptoWallet.properties.balance.label
 #: followthemoney/schema/BankAccount.yaml
 #: followthemoney/schema/CryptoWallet.yaml
 msgid "Balance"
 msgstr "Баланс"
 
@@ -1710,22 +1720,14 @@
 msgid ""
 "(Описание кода ТН ВЭД) Foreign Economic Activity Commodity Code description"
 msgstr ""
 "(Описание кода ТН ВЭД) Описание кода товарной номенклатуры "
 "внешнеэкономической деятельности"
 
 #. EconomicActivity.properties.goodsDescription.label
-#. Interval.properties.description.label
-#. Thing.properties.description.label
-#: followthemoney/schema/EconomicActivity.yaml
-#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
-msgid "Description"
-msgstr "Описание"
-
-#. EconomicActivity.properties.goodsDescription.description
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Description of goods"
 msgstr "Описание и характеристика товаров"
 
 #. EconomicActivity.properties.declarant.label
 #: followthemoney/schema/EconomicActivity.yaml
 msgid "Declarant"
@@ -2246,14 +2248,20 @@
 
 #. Interval.properties.summary.label
 #. Thing.properties.summary.label
 #: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
 msgid "Summary"
 msgstr "Информация"
 
+#. Interval.properties.description.label
+#. Thing.properties.description.label
+#: followthemoney/schema/Interval.yaml followthemoney/schema/Thing.yaml
+msgid "Description"
+msgstr "Описание"
+
 #. Interval.properties.recordId.label
 #: followthemoney/schema/Interval.yaml
 msgid "Record ID"
 msgstr "ID записи"
 
 #. Interval.properties.sourceUrl.label
 #. Thing.properties.sourceUrl.label
```

### Comparing `followthemoney-3.3.0/followthemoney/translations/ru/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/ru/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po` & `followthemoney-3.4.0/followthemoney/translations/tr/LC_MESSAGES/followthemoney.po`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/__init__.py` & `followthemoney-3.4.0/followthemoney/types/__init__.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/address.py` & `followthemoney-3.4.0/followthemoney/types/address.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/checksum.py` & `followthemoney-3.4.0/followthemoney/types/checksum.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/common.py` & `followthemoney-3.4.0/followthemoney/types/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import product
-from babel.core import Locale  # type: ignore
+from babel.core import Locale
 from banal import ensure_list
 from normality import stringify
 from typing import Any, Dict, Optional, Sequence, Callable, TYPE_CHECKING, TypedDict
 
 from followthemoney.rdf import Literal, Identifier
 from followthemoney.util import get_locale
 from followthemoney.util import gettext, sanitize_text
@@ -213,15 +213,15 @@
     """Enumerated type properties are used for types which have a defined set
     of possible values, like languages and countries."""
 
     def __init__(self) -> None:
         self._names: Dict[Locale, EnumValues] = {}
         self.codes = set(self.names.keys())
 
-    def _locale_names(self, locale: str) -> EnumValues:
+    def _locale_names(self, locale: Locale) -> EnumValues:
         return {}
 
     @property
     def names(self) -> EnumValues:
         """Return a mapping from property values to their labels in the current
         locale."""
         locale = get_locale()
```

### Comparing `followthemoney-3.3.0/followthemoney/types/country.py` & `followthemoney-3.4.0/followthemoney/types/country.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import countrynames
 from typing import Optional, TYPE_CHECKING
-from babel.core import Locale  # type: ignore
+from babel.core import Locale
 
 from followthemoney.rdf import URIRef, Identifier
 from followthemoney.types.common import EnumType, EnumValues
 from followthemoney.util import gettext, defer as _
 
 if TYPE_CHECKING:
     from followthemoney.proxy import EntityProxy
```

### Comparing `followthemoney-3.3.0/followthemoney/types/date.py` & `followthemoney-3.4.0/followthemoney/types/date.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/email.py` & `followthemoney-3.4.0/followthemoney/types/email.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/entity.py` & `followthemoney-3.4.0/followthemoney/types/entity.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/gender.py` & `followthemoney-3.4.0/followthemoney/types/gender.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, TYPE_CHECKING
-from babel.core import Locale  # type: ignore
+from babel.core import Locale
 
 from followthemoney.types.common import EnumType, EnumValues
 from followthemoney.rdf import URIRef, Identifier
 from followthemoney.util import gettext, defer as _
 
 if TYPE_CHECKING:
     from followthemoney.proxy import EntityProxy
```

### Comparing `followthemoney-3.3.0/followthemoney/types/iban.py` & `followthemoney-3.4.0/followthemoney/types/iban.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/identifier.py` & `followthemoney-3.4.0/followthemoney/types/identifier.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/ip.py` & `followthemoney-3.4.0/followthemoney/types/ip.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/json.py` & `followthemoney-3.4.0/followthemoney/types/json.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/language.py` & `followthemoney-3.4.0/followthemoney/types/language.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Optional, TYPE_CHECKING
-from babel.core import Locale  # type: ignore
+from babel.core import Locale
 from languagecodes import iso_639_alpha3
 
 from followthemoney.types.common import EnumType, EnumValues
 from followthemoney.rdf import URIRef, Identifier
 from followthemoney.util import defer as _
 from followthemoney.util import get_env_list
```

### Comparing `followthemoney-3.3.0/followthemoney/types/mimetype.py` & `followthemoney-3.4.0/followthemoney/types/mimetype.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/name.py` & `followthemoney-3.4.0/followthemoney/types/name.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from typing import Dict, List, Optional, Sequence, TYPE_CHECKING, Union
-from banal import first
+from typing import TYPE_CHECKING, Dict, List, Optional, Sequence, Union
+
+from Levenshtein import distance, setmedian
 from normality import slugify
 from normality.cleaning import collapse_spaces, strip_quotes
-from Levenshtein import distance, setmedian
 
 from followthemoney.types.common import PropertyType
 from followthemoney.util import dampen
 from followthemoney.util import defer as _
 
 if TYPE_CHECKING:
     from followthemoney.proxy import EntityProxy
@@ -53,14 +53,17 @@
             norm = slugify(value, sep=" ")
             if norm is None:
                 continue
             normalised.append(norm)
             lookup.setdefault(norm, [])
             lookup[norm].append(value)
 
+        if not normalised:
+            return None
+
         norm = setmedian(normalised)
         if norm is None:
             return None
         forms = lookup.get(norm, [])
         if len(forms) > 1:
             return setmedian(forms)
         for form in forms:
```

### Comparing `followthemoney-3.3.0/followthemoney/types/number.py` & `followthemoney-3.4.0/followthemoney/types/number.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/phone.py` & `followthemoney-3.4.0/followthemoney/types/phone.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/registry.py` & `followthemoney-3.4.0/followthemoney/types/registry.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/string.py` & `followthemoney-3.4.0/followthemoney/types/string.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/types/topic.py` & `followthemoney-3.4.0/followthemoney/types/topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from babel.core import Locale  # type: ignore
+from babel.core import Locale
 
 from followthemoney.types.common import EnumType, EnumValues
 from followthemoney.rdf import URIRef, Identifier
 from followthemoney.util import gettext, defer as _
 
 
 class TopicType(EnumType):
@@ -42,15 +42,15 @@
         "gov.muni": _("Municipal government"),
         "gov.soe": _("State-owned enterprise"),
         "gov.igo": _("Intergovernmental organization"),
         "fin": _("Financial services"),
         "fin.bank": _("Bank"),
         "fin.fund": _("Fund"),
         "fin.adivsor": _("Financial advisor"),
-        "role.pep": _("Politician"),  # don't FATF-splain me, bro.
+        "role.pep": _("Politican"),
         "role.rca": _("Close Associate"),
         "role.judge": _("Judge"),
         "role.civil": _("Civil servant"),
         "role.diplo": _("Diplomat"),
         "role.lawyer": _("Lawyer"),
         "role.acct": _("Accountant"),
         "role.spy": _("Spy"),
@@ -59,14 +59,15 @@
         "role.act": _("Activist"),
         "pol.party": _("Political party"),
         "pol.union": _("Union"),
         "rel": _("Religion"),
         "mil": _("Military"),
         "asset.frozen": _("Frozen asset"),
         "sanction": _("Sanctioned entity"),
+        "sanction.linked": _("Sanction-linked entity"),
         "debarment": _("Debarred entity"),
         "poi": _("Person of interest"),
     }
 
     def _locale_names(self, locale: Locale) -> EnumValues:
         return {k: gettext(v) for (k, v) in self._TOPICS.items()}
```

### Comparing `followthemoney-3.3.0/followthemoney/types/url.py` & `followthemoney-3.4.0/followthemoney/types/url.py`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney/util.py` & `followthemoney-3.4.0/followthemoney/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import logging
 from hashlib import sha1
-from babel import Locale  # type: ignore
+from babel import Locale
 from gettext import translation
 
 from threading import local
 from typing import cast, Dict, Any, List, Optional, TypeVar, Union, Sequence
 from normality import stringify
 from normality.cleaning import compose_nfc
 from normality.cleaning import remove_unsafe_chars
@@ -27,33 +27,33 @@
 i18n_path = os.path.join(os.path.dirname(__file__), "translations")
 state = local()
 log = logging.getLogger(__name__)
 
 
 def gettext(*args: Optional[str], **kwargs: Dict[str, str]) -> str:
     if not hasattr(state, "translation"):
-        set_model_locale(DEFAULT_LOCALE)
+        set_model_locale(Locale.parse(DEFAULT_LOCALE))
     return cast(str, state.translation.gettext(*args, **kwargs))
 
 
 def defer(text: str) -> str:
     return text
 
 
 def set_model_locale(locale: Locale) -> None:
     state.locale = locale
     state.translation = translation(
-        "followthemoney", i18n_path, [locale], fallback=True
+        "followthemoney", i18n_path, [str(locale)], fallback=True
     )
 
 
 def get_locale() -> Locale:
     if not hasattr(state, "locale"):
-        return Locale(DEFAULT_LOCALE)
-    return Locale(state.locale)
+        return Locale.parse(DEFAULT_LOCALE)
+    return cast(Locale, state.locale)
 
 
 def get_env_list(name: str, default: List[str] = []) -> List[str]:
     value = stringify(os.environ.get(name))
     if value is not None:
         values = value.split(":")
         if len(values):
@@ -134,14 +134,16 @@
 
 def merge_context(left: Dict[K, V], right: Dict[K, V]) -> Dict[K, List[V]]:
     """When merging two entities, make lists of all the duplicate context
     keys."""
     combined = {}
     keys = [*left.keys(), *right.keys()]
     for key in set(keys):
+        if key in ("caption",):
+            continue
         lval: List[V] = [i for i in ensure_list(left.get(key)) if i is not None]
         rval: List[V] = [i for i in ensure_list(right.get(key)) if i is not None]
         combined[key] = unique_list([*lval, *rval])
     return combined
 
 
 def dampen(short: int, long: int, text: str) -> float:
```

### Comparing `followthemoney-3.3.0/followthemoney.egg-info/PKG-INFO` & `followthemoney-3.4.0/followthemoney.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,90 @@
 Metadata-Version: 2.1
 Name: followthemoney
-Version: 3.3.0
-Summary: UNKNOWN
+Version: 3.4.0
 Home-page: https://followthemoney.tech/
 Author: Organized Crime and Corruption Reporting Project
 Author-email: data@occrp.org
 License: MIT
-Description: # Follow the Money
-        
-        [![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
-        
-        This repository contains a pragmatic data model for the entities most
-        commonly used in investigative reporting: people, companies, assets,
-        payments, court cases, etc.
-        
-        The purpose of this is not to model reality in an ideal data model, but
-        rather to have a working data structure for researchers.
-        
-        `followthemoney` also contains code used to validate and normalize many
-        of the elements of data, and to map tabular data into the model.
-        
-        ## Documentation
-        
-        For a general introduction to `followthemoney`, check the high-level introduction:
-        
-        * https://followthemoney.tech
-        
-        Part of this package is a command-line tool that can be used to process and
-        transform data in various ways. You can find a tutorial here:
-        
-        * https://followthemoney.tech/docs/cli/
-        
-        Besides the introductions, there is also a full reference documentation for the
-        library and the contained ontology: 
-        
-        * https://followthemoney.tech/explorer/
-        
-        There's also a number of viewers for the RDF schema definitions generated
-        from FollowTheMoney, e.g.:
-        
-        * [LODE documentation](http://150.146.207.114/lode/extract?url=https%3A%2F%2Falephdata.github.io%2Ffollowthemoney%2Fns%2Fftm.xml&owlapi=true&imported=true&lang=en)
-        * [WebVOWL](https://service.tib.eu/webvowl/#iri=https://alephdata.github.io/followthemoney/ns/ftm.xml)
-        * RDF/OWL specification in [XML](https://alephdata.github.io/followthemoney/ns/ftm.xml).
-        
-        ## Development environment
-        
-        For local development with a virtualenv:
-        
-        ```bash
-        python3 -mvenv .env
-        source .env/bin/activate
-        pip install -e ".[dev]"
-        ```
-        
-        Now you can run the tests with
-        
-        ```bash
-        make test
-        ```
-        
-        ## Releasing
-        
-        We release a lot of version of `followthemoney` because even small changes
-        to the code base require a pypi release to begin being used in `aleph`. To
-        this end, here's the steps for making a release:
-        
-        ```bash
-        git pull --rebase
-        make build
-        make test
-        git add . && git commit -m "Updating translation files"
-        bumpversion patch
-        git push --atomic origin main $(git describe --tags --abbrev=0)
-        ```
-        
-        This will create a new patch release and upload a distribution of it. If
-        the changes are more significant, you can run `bumpversion` with the `minor`
-        or `major` arguments.
-        
-        When the schema is updated, please update the docs, ideally including the
-        diagrams. For the RDF namespace and JavaScript version of the model, 
-        run `make generate`.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
+
+# Follow the Money
+
+[![ftm-build](https://github.com/alephdata/followthemoney/actions/workflows/build.yml/badge.svg)](https://github.com/alephdata/followthemoney/actions/workflows/build.yml)
+
+This repository contains a pragmatic data model for the entities most
+commonly used in investigative reporting: people, companies, assets,
+payments, court cases, etc.
+
+The purpose of this is not to model reality in an ideal data model, but
+rather to have a working data structure for researchers.
+
+`followthemoney` also contains code used to validate and normalize many
+of the elements of data, and to map tabular data into the model.
+
+## Documentation
+
+For a general introduction to `followthemoney`, check the high-level introduction:
+
+* https://followthemoney.tech
+
+Part of this package is a command-line tool that can be used to process and
+transform data in various ways. You can find a tutorial here:
+
+* https://followthemoney.tech/docs/cli/
+
+Besides the introductions, there is also a full reference documentation for the
+library and the contained ontology: 
+
+* https://followthemoney.tech/explorer/
+
+There's also a number of viewers for the RDF schema definitions generated
+from FollowTheMoney, e.g.:
+
+* [LODE documentation](http://150.146.207.114/lode/extract?url=https%3A%2F%2Falephdata.github.io%2Ffollowthemoney%2Fns%2Fftm.xml&owlapi=true&imported=true&lang=en)
+* [WebVOWL](https://service.tib.eu/webvowl/#iri=https://alephdata.github.io/followthemoney/ns/ftm.xml)
+* RDF/OWL specification in [XML](https://alephdata.github.io/followthemoney/ns/ftm.xml).
+
+## Development environment
+
+For local development with a virtualenv:
+
+```bash
+python3 -mvenv .env
+source .env/bin/activate
+pip install -e ".[dev]"
+```
+
+Now you can run the tests with
+
+```bash
+make test
+```
+
+## Releasing
+
+We release a lot of version of `followthemoney` because even small changes
+to the code base require a pypi release to begin being used in `aleph`. To
+this end, here's the steps for making a release:
+
+```bash
+git pull --rebase
+make build
+make test
+git add . && git commit -m "Updating translation files"
+bumpversion patch
+git push --atomic origin main $(git describe --tags --abbrev=0)
+```
+
+This will create a new patch release and upload a distribution of it. If
+the changes are more significant, you can run `bumpversion` with the `minor`
+or `major` arguments.
+
+When the schema is updated, please update the docs, ideally including the
+diagrams. For the RDF namespace and JavaScript version of the model, 
+run `make generate`.
```

### Comparing `followthemoney-3.3.0/followthemoney.egg-info/SOURCES.txt` & `followthemoney-3.4.0/followthemoney.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `followthemoney-3.3.0/followthemoney.egg-info/entry_points.txt` & `followthemoney-3.4.0/followthemoney.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,7 @@
 csv = followthemoney.cli.exports:export_csv
 cypher = followthemoney.cli.exports:export_cypher
 excel = followthemoney.cli.exports:export_excel
 gexf = followthemoney.cli.exports:export_gexf
 mapping = followthemoney.cli.mapping:run_mapping
 rdf = followthemoney.cli.exports:export_rdf
 sieve = followthemoney.cli.sieve:sieve
-
```

### Comparing `followthemoney-3.3.0/followthemoney.egg-info/requires.txt` & `followthemoney-3.4.0/followthemoney.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 languagecodes<2.0.0,>=1.1.0
 prefixdate<1.0.0,>=0.4.0
 fingerprints<2.0.0,>=1.0.1
 phonenumbers<9.0.0,>=8.12.22
 python-stdnum<2.0.0,>=1.16
 pantomime<1.0.0,>=0.5.1
 pytz>=2021.1
-rdflib<6.3.0,>=6.2.0
-networkx<3.1,>=2.5
+rdflib<6.4.0,>=6.2.0
+networkx<3.2,>=2.5
 openpyxl<4.0.0,>=3.0.5
 orjson<4.0,>=3.7
 
 [dev]
 pip>=10.0.0
 bump2version
 wheel>=0.29.0
```

### Comparing `followthemoney-3.3.0/setup.py` & `followthemoney-3.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages  # type: ignore
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="followthemoney",
-    version="3.3.0",
+    version="3.4.0",
     author="Organized Crime and Corruption Reporting Project",
     author_email="data@occrp.org",
     url="https://followthemoney.tech/",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
@@ -45,16 +45,16 @@
         "languagecodes >= 1.1.0, < 2.0.0",
         "prefixdate >= 0.4.0, < 1.0.0",
         "fingerprints >= 1.0.1, < 2.0.0",
         "phonenumbers >= 8.12.22, < 9.0.0",
         "python-stdnum >= 1.16, < 2.0.0",
         "pantomime >= 0.5.1, < 1.0.0",
         "pytz >= 2021.1",
-        "rdflib >= 6.2.0, < 6.3.0",
-        "networkx >= 2.5, < 3.1",
+        "rdflib >= 6.2.0, < 6.4.0",
+        "networkx >= 2.5, < 3.2",
         "openpyxl >= 3.0.5, < 4.0.0",
         "orjson >= 3.7, < 4.0",
     ],
     extras_require={
         "dev": [
             "pip>=10.0.0",
             "bump2version",
```

