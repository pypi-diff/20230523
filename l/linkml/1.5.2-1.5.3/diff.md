# Comparing `tmp/linkml-1.5.2.tar.gz` & `tmp/linkml-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml-1.5.2.tar", max compression
+gzip compressed data, was "linkml-1.5.3.tar", max compression
```

## Comparing `linkml-1.5.2.tar` & `linkml-1.5.3.tar`

### file list

```diff
@@ -1,108 +1,109 @@
--rw-r--r--   0        0        0     6555 2023-05-05 00:39:55.714937 linkml-1.5.2/LICENSE
--rw-r--r--   0        0        0     1369 2023-05-05 00:39:55.714937 linkml-1.5.2/README.md
--rw-r--r--   0        0        0     3227 2023-05-05 00:39:55.734937 linkml-1.5.2/linkml/__init__.py
--rw-r--r--   0        0        0      326 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/_version.py
--rw-r--r--   0        0        0    51005 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/PythonGenNotes.md
--rw-r--r--   0        0        0     3926 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/README.md
--rw-r--r--   0        0        0      616 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/common/__init__.py
--rw-r--r--   0        0        0     2040 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/common/type_designators.py
--rw-r--r--   0        0        0     3118 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/csvgen.py
--rw-r--r--   0        0        0     2873 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/class.md.jinja2
--rw-r--r--   0        0        0     2682 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/class_diagram.md.jinja2
--rw-r--r--   0        0        0     1321 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/common_metadata.md.jinja2
--rw-r--r--   0        0        0     1018 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/enum.md.jinja2
--rw-r--r--   0        0        0     1190 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/index.md.jinja2
--rw-r--r--   0        0        0      501 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/index.tex.jinja2
--rw-r--r--   0        0        0       70 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/schema.md.jinja2
--rw-r--r--   0        0        0     2557 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/slot.md.jinja2
--rw-r--r--   0        0        0     1704 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/subset.md.jinja2
--rw-r--r--   0        0        0      635 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/type.md.jinja2
--rw-r--r--   0        0        0    32663 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen.py
--rw-r--r--   0        0        0     5112 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/dotgen.py
--rw-r--r--   0        0        0    10863 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/erdiagramgen.py
--rw-r--r--   0        0        0     6894 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/excelgen.py
--rw-r--r--   0        0        0     3575 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/golrgen.py
--rw-r--r--   0        0        0     2347 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/graphqlgen.py
--rw-r--r--   0        0        0      444 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/javagen/example_template.java.jinja2
--rw-r--r--   0        0        0     1737 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/javagen/java_record_template.jinja2
--rw-r--r--   0        0        0     5499 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/javagen.py
--rw-r--r--   0        0        0     8821 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/jsonldcontextgen.py
--rw-r--r--   0        0        0     7952 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/jsonldgen.py
--rw-r--r--   0        0        0    22730 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/jsonschemagen.py
--rw-r--r--   0        0        0     3555 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/linkmlgen.py
--rw-r--r--   0        0        0    34422 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/markdowngen.py
--rw-r--r--   0        0        0     6532 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/namespacegen.py
--rw-r--r--   0        0        0     6695 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/oocodegen.py
--rw-r--r--   0        0        0    27365 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/owlgen.py
--rw-r--r--   0        0        0     4911 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/prefixmapgen.py
--rw-r--r--   0        0        0     9811 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/projectgen.py
--rw-r--r--   0        0        0     2443 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/protogen.py
--rw-r--r--   0        0        0    21783 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/pydanticgen.py
--rw-r--r--   0        0        0    50389 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/pythongen.py
--rw-r--r--   0        0        0     2825 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/rdfgen.py
--rw-r--r--   0        0        0     5621 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/shaclgen.py
--rw-r--r--   0        0        0     9547 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/shexgen.py
--rw-r--r--   0        0        0     6632 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sparqlgen.py
--rw-r--r--   0        0        0      166 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2575 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
--rw-r--r--   0        0        0     1625 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
--rw-r--r--   0        0        0     9334 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqlalchemygen.py
--rw-r--r--   0        0        0    18626 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqlddlgen.py
--rw-r--r--   0        0        0    11387 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqltablegen.py
--rw-r--r--   0        0        0     7177 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/sssomgen.py
--rw-r--r--   0        0        0     1788 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/string_template.md
--rw-r--r--   0        0        0     3020 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/summarygen.py
--rw-r--r--   0        0        0     4760 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/terminusdbgen.py
--rw-r--r--   0        0        0     5555 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/typescriptgen.py
--rw-r--r--   0        0        0     1746 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/yamlgen.py
--rw-r--r--   0        0        0    13311 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/yumlgen.py
--rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/__init__.py
--rw-r--r--   0        0        0     4323 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/cli.py
--rw-r--r--   0        0        0      292 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/datamodel/.linkmllint.yaml
--rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/datamodel/__init__.py
--rw-r--r--   0        0        0    17711 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/datamodel/config.py
--rw-r--r--   0        0        0     6980 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/datamodel/config.yaml
--rw-r--r--   0        0        0      540 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/default.yaml
--rw-r--r--   0        0        0      198 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/recommended.yaml
--rw-r--r--   0        0        0      269 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/__init__.py
--rw-r--r--   0        0        0      518 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/formatter.py
--rw-r--r--   0        0        0      767 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/json_formatter.py
--rw-r--r--   0        0        0     2605 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/markdown_formatter.py
--rw-r--r--   0        0        0     2085 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/terminal_formatter.py
--rw-r--r--   0        0        0      871 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/tsv_formatter.py
--rw-r--r--   0        0        0     5004 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/linter.py
--rw-r--r--   0        0        0    11649 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/rules.py
--rw-r--r--   0        0        0       55 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/reporting/__init__.py
--rw-r--r--   0        0        0     9189 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/reporting/model.py
--rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/transformers/__init__.py
--rw-r--r--   0        0        0    18594 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/transformers/relmodel_transformer.py
--rw-r--r--   0        0        0     5455 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/transformers/schema_renamer.py
--rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/__init__.py
--rw-r--r--   0        0        0     6463 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/converter.py
--rw-r--r--   0        0        0     4384 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/datautils.py
--rw-r--r--   0        0        0      490 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/datavalidator.py
--rw-r--r--   0        0        0     6999 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/execute_tutorial.py
--rw-r--r--   0        0        0    39740 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/generator.py
--rw-r--r--   0        0        0      445 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/helpers.py
--rw-r--r--   0        0        0     5773 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/ifabsent_functions.py
--rw-r--r--   0        0        0     9498 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/mergeutils.py
--rw-r--r--   0        0        0     4560 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/rawloader.py
--rw-r--r--   0        0        0     9065 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/schema_builder.py
--rw-r--r--   0        0        0    13464 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/schema_fixer.py
--rw-r--r--   0        0        0    48537 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/schemaloader.py
--rw-r--r--   0        0        0    19733 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/schemasynopsis.py
--rw-r--r--   0        0        0    16297 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/sqlutils.py
--rw-r--r--   0        0        0     2395 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/typereferences.py
--rw-r--r--   0        0        0     1514 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/validation.py
--rw-r--r--   0        0        0      140 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/validators/__init__.py
--rw-r--r--   0        0        0     6255 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/validators/jsonschemavalidator.py
--rw-r--r--   0        0        0     4873 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/validators/sparqlvalidator.py
--rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/workspaces/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/workspaces/datamodel/__init__.py
--rw-r--r--   0        0        0    15641 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/workspaces/datamodel/workspaces.py
--rw-r--r--   0        0        0     4233 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/workspaces/datamodel/workspaces.yaml
--rw-r--r--   0        0        0    11759 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/workspaces/example_runner.py
--rw-r--r--   0        0        0     4868 2023-05-05 00:40:31.907169 linkml-1.5.2/pyproject.toml
--rw-r--r--   0        0        0     6564 1970-01-01 00:00:00.000000 linkml-1.5.2/setup.py
--rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 linkml-1.5.2/PKG-INFO
+-rw-r--r--   0        0        0     6555 2023-05-23 20:25:52.064652 linkml-1.5.3/LICENSE
+-rw-r--r--   0        0        0     1369 2023-05-23 20:25:52.064652 linkml-1.5.3/README.md
+-rw-r--r--   0        0        0     3227 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/_version.py
+-rw-r--r--   0        0        0    51005 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/PythonGenNotes.md
+-rw-r--r--   0        0        0     4158 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/README.md
+-rw-r--r--   0        0        0      616 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/common/__init__.py
+-rw-r--r--   0        0        0     2040 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/common/type_designators.py
+-rw-r--r--   0        0        0     3118 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/csvgen.py
+-rw-r--r--   0        0        0     2873 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/class.md.jinja2
+-rw-r--r--   0        0        0     2682 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/class_diagram.md.jinja2
+-rw-r--r--   0        0        0     1321 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/common_metadata.md.jinja2
+-rw-r--r--   0        0        0     1018 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/enum.md.jinja2
+-rw-r--r--   0        0        0     1190 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/index.md.jinja2
+-rw-r--r--   0        0        0      501 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/index.tex.jinja2
+-rw-r--r--   0        0        0       70 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen/schema.md.jinja2
+-rw-r--r--   0        0        0     2557 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/docgen/slot.md.jinja2
+-rw-r--r--   0        0        0     1704 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/docgen/subset.md.jinja2
+-rw-r--r--   0        0        0      635 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/docgen/type.md.jinja2
+-rw-r--r--   0        0        0    32663 2023-05-23 20:25:52.084652 linkml-1.5.3/linkml/generators/docgen.py
+-rw-r--r--   0        0        0     5112 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/dotgen.py
+-rw-r--r--   0        0        0    10913 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/erdiagramgen.py
+-rw-r--r--   0        0        0     6894 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/excelgen.py
+-rw-r--r--   0        0        0     6393 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/golanggen.py
+-rw-r--r--   0        0        0     3575 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/golrgen.py
+-rw-r--r--   0        0        0     2347 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/graphqlgen.py
+-rw-r--r--   0        0        0      444 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/javagen/example_template.java.jinja2
+-rw-r--r--   0        0        0     1737 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/javagen/java_record_template.jinja2
+-rw-r--r--   0        0        0     5499 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/javagen.py
+-rw-r--r--   0        0        0     8821 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/jsonldcontextgen.py
+-rw-r--r--   0        0        0     7952 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/jsonldgen.py
+-rw-r--r--   0        0        0    21688 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/jsonschemagen.py
+-rw-r--r--   0        0        0     3555 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/linkmlgen.py
+-rw-r--r--   0        0        0    34422 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/markdowngen.py
+-rw-r--r--   0        0        0     6532 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/namespacegen.py
+-rw-r--r--   0        0        0     7831 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/oocodegen.py
+-rw-r--r--   0        0        0    27365 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/owlgen.py
+-rw-r--r--   0        0        0     4911 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/prefixmapgen.py
+-rw-r--r--   0        0        0     9811 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/projectgen.py
+-rw-r--r--   0        0        0     2443 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/protogen.py
+-rw-r--r--   0        0        0    22150 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/pydanticgen.py
+-rw-r--r--   0        0        0    50389 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/pythongen.py
+-rw-r--r--   0        0        0     2825 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/rdfgen.py
+-rw-r--r--   0        0        0     5621 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/shaclgen.py
+-rw-r--r--   0        0        0     9547 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/shexgen.py
+-rw-r--r--   0        0        0     6632 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sparqlgen.py
+-rw-r--r--   0        0        0      166 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2575 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
+-rw-r--r--   0        0        0     1625 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
+-rw-r--r--   0        0        0     9334 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqlalchemygen.py
+-rw-r--r--   0        0        0    18626 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqlddlgen.py
+-rw-r--r--   0        0        0    11387 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sqltablegen.py
+-rw-r--r--   0        0        0     7177 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/sssomgen.py
+-rw-r--r--   0        0        0     1788 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/string_template.md
+-rw-r--r--   0        0        0     3020 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/summarygen.py
+-rw-r--r--   0        0        0     4760 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/terminusdbgen.py
+-rw-r--r--   0        0        0     6094 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/typescriptgen.py
+-rw-r--r--   0        0        0     1746 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/yamlgen.py
+-rw-r--r--   0        0        0    13311 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/generators/yumlgen.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/__init__.py
+-rw-r--r--   0        0        0     4323 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/cli.py
+-rw-r--r--   0        0        0      292 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/datamodel/.linkmllint.yaml
+-rw-r--r--   0        0        0        0 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/datamodel/__init__.py
+-rw-r--r--   0        0        0    17711 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/datamodel/config.py
+-rw-r--r--   0        0        0     6980 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/datamodel/config.yaml
+-rw-r--r--   0        0        0      540 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/default.yaml
+-rw-r--r--   0        0        0      198 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/config/recommended.yaml
+-rw-r--r--   0        0        0      269 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/__init__.py
+-rw-r--r--   0        0        0      518 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/formatter.py
+-rw-r--r--   0        0        0      767 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/json_formatter.py
+-rw-r--r--   0        0        0     2605 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/markdown_formatter.py
+-rw-r--r--   0        0        0     2085 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/terminal_formatter.py
+-rw-r--r--   0        0        0      871 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/formatters/tsv_formatter.py
+-rw-r--r--   0        0        0     5004 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/linter.py
+-rw-r--r--   0        0        0    11649 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/linter/rules.py
+-rw-r--r--   0        0        0       55 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/reporting/__init__.py
+-rw-r--r--   0        0        0     9189 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/reporting/model.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/transformers/__init__.py
+-rw-r--r--   0        0        0    18594 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/transformers/relmodel_transformer.py
+-rw-r--r--   0        0        0     5455 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/transformers/schema_renamer.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/utils/__init__.py
+-rw-r--r--   0        0        0     6463 2023-05-23 20:25:52.088652 linkml-1.5.3/linkml/utils/converter.py
+-rw-r--r--   0        0        0     4384 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/datautils.py
+-rw-r--r--   0        0        0      490 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/datavalidator.py
+-rw-r--r--   0        0        0     6999 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/execute_tutorial.py
+-rw-r--r--   0        0        0    39737 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/generator.py
+-rw-r--r--   0        0        0      445 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/helpers.py
+-rw-r--r--   0        0        0     5773 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/ifabsent_functions.py
+-rw-r--r--   0        0        0     9498 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/mergeutils.py
+-rw-r--r--   0        0        0     4560 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/rawloader.py
+-rw-r--r--   0        0        0     9065 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/schema_builder.py
+-rw-r--r--   0        0        0    13464 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/schema_fixer.py
+-rw-r--r--   0        0        0    48537 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/schemaloader.py
+-rw-r--r--   0        0        0    19733 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/schemasynopsis.py
+-rw-r--r--   0        0        0    16297 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/sqlutils.py
+-rw-r--r--   0        0        0     2395 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/typereferences.py
+-rw-r--r--   0        0        0     1514 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/utils/validation.py
+-rw-r--r--   0        0        0      140 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/validators/__init__.py
+-rw-r--r--   0        0        0     6255 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/validators/jsonschemavalidator.py
+-rw-r--r--   0        0        0     4873 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/validators/sparqlvalidator.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/workspaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/workspaces/datamodel/__init__.py
+-rw-r--r--   0        0        0    15641 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/workspaces/datamodel/workspaces.py
+-rw-r--r--   0        0        0     4233 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/workspaces/datamodel/workspaces.yaml
+-rw-r--r--   0        0        0    11912 2023-05-23 20:25:52.092652 linkml-1.5.3/linkml/workspaces/example_runner.py
+-rw-r--r--   0        0        0     4973 2023-05-23 20:26:21.032995 linkml-1.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6700 1970-01-01 00:00:00.000000 linkml-1.5.3/setup.py
+-rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 linkml-1.5.3/PKG-INFO
```

### Comparing `linkml-1.5.2/LICENSE` & `linkml-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/README.md` & `linkml-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/__init__.py` & `linkml-1.5.3/linkml/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/PythonGenNotes.md` & `linkml-1.5.3/linkml/generators/PythonGenNotes.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/README.md` & `linkml-1.5.3/linkml/generators/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 | command line | module | Generator name | function | help file |
 | -----------  | ------ | -------------  | -------- | --------- |
 |  gen-yaml    | [yamlgen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/yamlgen.py) | YamlGenerator | Validate YAML or emit compiled module | [yamlgen help](../../tests/test_scripts/output/genyaml/help) |
 |  gen-jsonld-context   | [jsonldcontextgen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/jsonldcontextgen.py) |    ContextGenerator | generate a JSON-LD @context block  | [contextgen help](../../tests/test_scripts/output/gencontext/help) |
 |  gen-csv   | [csvgen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/csvgen.py) |    CsvGenerator | generate a csv summary  | [csvgen help](../../tests/test_scripts/output/gencsv/help) |
 |  gen-graphviz   | [dotgen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/dotgen.py) |    DotGenerator | generate graphviz representation  | [dotgen help](../../tests/test_scripts/output/gengraphviz/help) |
+|  gen-golang   | [golanggen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/golanggen.py) |    GolangGenerator | generate Golang representation  | [golanggen help](../../tests/test_scripts/output/gengolang/help) |
 |  gen-golr-views   | [golrgen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/golrgen.py) |    GolrSchemaGenerator | generate a GOLR(?) representation  | [golrgen help](../../tests/test_scripts/output/genglor/help) |
 |  gen-graphql   | [graphqlgen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/graphqlgen.py) |    GraphqlGenerator | generate a graphql representation  | [graphql help](../../tests/test_scripts/output/gengraphql/help) |
 |  gen-proto  | [protogen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/protogen.py) | ProtoGenerator | generate Protobuf Schema representation | [proto help](../../tests/test_scripts/output/genproto/help) |
 |  gen-jsonld | [jsonldgen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/jsonldgen.py) | JSONLDGenerator | generate JSON representation | [jsonld help](../../tests/test_scripts/output/genjsonld/help) |
 |  gen-json-schema   | [jsonschemagen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/jsonschemagen.py) |    JsonSchemaGenerator | generate JSON Schema representation  | [jsonschmeagen help](../../tests/test_scripts/output/genjsonschema/help) |
 |  gen-markdown   | [markdowngen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/markdowngen.py) |    MarkdownGenerator | generate markdown documentation of the model  | [markdowngen help](../../tests/test_scripts/output/genmarkdown/help) |
 |  gen-namespaces | [namespacegen.py](https://github.com/linkml/linkml/blob/main/linkml/generators/namespacegen.py) | NamespaceGenerator | generate namespace manager for URI's in model | [namespacegen help](../../tests/test_scripts/output/gennamespace/help) |
```

### Comparing `linkml-1.5.2/linkml/generators/__init__.py` & `linkml-1.5.3/linkml/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/common/type_designators.py` & `linkml-1.5.3/linkml/generators/common/type_designators.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/csvgen.py` & `linkml-1.5.3/linkml/generators/csvgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/docgen/class.md.jinja2` & `linkml-1.5.3/linkml/generators/docgen/class.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/docgen/class_diagram.md.jinja2` & `linkml-1.5.3/linkml/generators/docgen/class_diagram.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/docgen/common_metadata.md.jinja2` & `linkml-1.5.3/linkml/generators/docgen/common_metadata.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/docgen/enum.md.jinja2` & `linkml-1.5.3/linkml/generators/docgen/enum.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/docgen/index.md.jinja2` & `linkml-1.5.3/linkml/generators/docgen/index.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/docgen/slot.md.jinja2` & `linkml-1.5.3/linkml/generators/docgen/slot.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/docgen/subset.md.jinja2` & `linkml-1.5.3/linkml/generators/docgen/subset.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/docgen/type.md.jinja2` & `linkml-1.5.3/linkml/generators/docgen/type.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/docgen.py` & `linkml-1.5.3/linkml/generators/docgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/dotgen.py` & `linkml-1.5.3/linkml/generators/dotgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/erdiagramgen.py` & `linkml-1.5.3/linkml/generators/erdiagramgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 class IdentifyingType(str, Enum):
     """ Identifying types.
 
     See: https://mermaid.js.org/syntax/entityRelationshipDiagram.html#identification"""
     IDENTIFYING = "--"
     NON_IDENTIFYING = ".."
 
+    def __str__(self):
+        return self.value
+
 
 class Cardinality(pydantic.BaseModel):
     """ Cardinality of a slot.
 
     See https://mermaid.js.org/syntax/entityRelationshipDiagram.html#relationship-syntax"""
     required: bool = True
     multivalued: bool = False
```

### Comparing `linkml-1.5.2/linkml/generators/excelgen.py` & `linkml-1.5.3/linkml/generators/excelgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/golrgen.py` & `linkml-1.5.3/linkml/generators/golrgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/graphqlgen.py` & `linkml-1.5.3/linkml/generators/graphqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/javagen/java_record_template.jinja2` & `linkml-1.5.3/linkml/generators/javagen/java_record_template.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/javagen.py` & `linkml-1.5.3/linkml/generators/javagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/jsonldcontextgen.py` & `linkml-1.5.3/linkml/generators/jsonldcontextgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/jsonldgen.py` & `linkml-1.5.3/linkml/generators/jsonldgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/jsonschemagen.py` & `linkml-1.5.3/linkml/generators/jsonschemagen.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,23 +313,25 @@
 
         slot_is_inlined = self.schemaview.is_inlined(slot)
         if slot.range in self.schemaview.all_types().keys():
             schema_type = self.schemaview.induced_type(slot.range)
             (typ, fmt) = json_schema_types.get(schema_type.base.lower(), ("string", None))
         elif slot.range in self.schemaview.all_enums().keys():
             reference = slot.range
-        elif (slot_is_inlined or parent_slot_is_inlined) and slot.range in self.schemaview.all_classes().keys():
-            descendants = [desc for desc in self.schemaview.class_descendants(slot.range) 
-                if not self.schemaview.get_class(desc).abstract]
-            if descendants and self.include_range_class_descendants:
-                reference = descendants
+        elif slot.range in self.schemaview.all_classes().keys():
+            if slot_is_inlined or parent_slot_is_inlined:
+                descendants = [desc for desc in self.schemaview.class_descendants(slot.range) 
+                    if not self.schemaview.get_class(desc).abstract]
+                if descendants and self.include_range_class_descendants:
+                    reference = descendants
+                else:
+                    reference = slot.range
             else:
-                reference = slot.range
-        else:
-            typ = "string"
+                id_slot = self.schemaview.get_identifier_slot(slot.range)
+                typ = id_slot.range or "string"
 
         return (typ, fmt, reference)
     
     def get_value_constraints_for_slot(self, slot: Union[AnonymousSlotExpression, None]) -> JsonSchema:
         if slot is None:
             return JsonSchema()
         
@@ -338,92 +340,66 @@
         constraints.add_keyword('minimum', slot.minimum_value)
         constraints.add_keyword('maximum', slot.maximum_value)
         constraints.add_keyword('const', slot.equals_string)
         constraints.add_keyword('const', slot.equals_number)
         return constraints
 
     def get_subschema_for_slot(self, slot: SlotDefinition, omit_type: bool = False) -> JsonSchema:
-        slot_has_range_union = slot.any_of is not None and len(slot.any_of) > 0 and all(s.range is not None for s in slot.any_of)
-        if omit_type:
-            prop = JsonSchema()
-        else:
-            slot_is_inlined = self.schemaview.is_inlined(slot)
-
-            if slot_has_range_union:
-                items = []
-                for sub_slot in slot.any_of:
-                    typ, fmt, reference = self.get_type_info_for_slot_subschema(sub_slot, slot_is_inlined)
-                    if reference is not None:
-                        item = JsonSchema.ref_for(reference)
-                    elif fmt is None:
-                        item = JsonSchema({"type": typ})
-                    else:
-                        item = JsonSchema({"type": typ, "format": fmt})
-                    items.append(item)
-                subschema = JsonSchema({
-                    "anyOf": items
-                })
-                if slot.multivalued:
-                    prop = JsonSchema.array_of(subschema)
-                else:
-                    prop = subschema
-            else:
-                typ, fmt, reference = self.get_type_info_for_slot_subschema(slot, slot_is_inlined)
-                if slot_is_inlined:
-                    # If inline we have to include redefined slots
-                    if slot.multivalued:
-                        range_id_slot, range_simple_dict_value_slot, range_required_slots = self._get_range_associated_slots(slot)
-                        # if the range class has an ID and the slot is not inlined as a list, then we need to consider
-                        # various inlined as dict formats
-                        if range_id_slot is not None and not slot.inlined_as_list:
-                            # At a minimum, the inlined dict can have keys (additionalProps) that are IDs
-                            # and the values are the range class but possibly omitting the ID.
-                            additionalProps = [JsonSchema.ref_for(reference, identifier_optional=True)]
-
-                            # If the range can be collected as a simple dict, then we can also accept the value
-                            # of that simple dict directly.
-                            if range_simple_dict_value_slot is not None:
-                                additionalProps.append(self.get_subschema_for_slot(range_simple_dict_value_slot))
-
-                            # If the range has no required slots, then null is acceptable
-                            if len(range_required_slots) == 0:
-                                additionalProps.append(JsonSchema({"type": "null"}))
-
-                            # If through the above logic we identified multiple acceptable forms, then wrap them
-                            # in an "anyOf", otherwise just take the only acceptable form
-                            if len(additionalProps) == 1:
-                                additionalProps = additionalProps[0]
-                            else:
-                                additionalProps = JsonSchema({
-                                    "anyOf": additionalProps
-                                })
-                            prop = JsonSchema({
-                                "type": "object",
-                                "additionalProperties": additionalProps
-                            })
-                            self.top_level_schema.add_lax_def(reference, self.aliased_slot_name(range_id_slot))
+        prop = JsonSchema()
+        slot_is_multivalued = 'multivalued' in slot and slot.multivalued
+        slot_is_inlined = self.schemaview.is_inlined(slot)
+        if not omit_type:
+            typ, fmt, reference = self.get_type_info_for_slot_subschema(slot, slot_is_inlined)
+            if slot_is_inlined:
+                # If inline we have to include redefined slots
+                if slot_is_multivalued:
+                    range_id_slot, range_simple_dict_value_slot, range_required_slots = self._get_range_associated_slots(slot)
+                    # if the range class has an ID and the slot is not inlined as a list, then we need to consider
+                    # various inlined as dict formats
+                    if range_id_slot is not None and not slot.inlined_as_list:
+                        # At a minimum, the inlined dict can have keys (additionalProps) that are IDs
+                        # and the values are the range class but possibly omitting the ID.
+                        additionalProps = [JsonSchema.ref_for(reference, identifier_optional=True)]
+
+                        # If the range can be collected as a simple dict, then we can also accept the value
+                        # of that simple dict directly.
+                        if range_simple_dict_value_slot is not None:
+                            additionalProps.append(self.get_subschema_for_slot(range_simple_dict_value_slot))
+
+                        # If the range has no required slots, then null is acceptable
+                        if len(range_required_slots) == 0:
+                            additionalProps.append(JsonSchema({"type": "null"}))
+
+                        # If through the above logic we identified multiple acceptable forms, then wrap them
+                        # in an "anyOf", otherwise just take the only acceptable form
+                        if len(additionalProps) == 1:
+                            additionalProps = additionalProps[0]
                         else:
-                            prop = JsonSchema.array_of(JsonSchema.ref_for(reference))
+                            additionalProps = JsonSchema({
+                                "anyOf": additionalProps
+                            })
+                        prop = JsonSchema({
+                            "type": "object",
+                            "additionalProperties": additionalProps
+                        })
+                        self.top_level_schema.add_lax_def(reference, self.aliased_slot_name(range_id_slot))
                     else:
-                        prop = JsonSchema.ref_for(reference)
+                        prop = JsonSchema.array_of(JsonSchema.ref_for(reference))
                 else:
-                    if slot.multivalued:
-                        if reference is not None:
-                            prop = JsonSchema.array_of(JsonSchema.ref_for(reference))
-                        elif fmt is None:
-                            prop = JsonSchema.array_of(JsonSchema({"type": typ}))
-                        else:
-                            prop = JsonSchema.array_of(JsonSchema({"type": typ, "format": fmt}))
-                    else:
-                        if reference is not None:
-                            prop = JsonSchema.ref_for(reference)
-                        elif fmt is None:
-                            prop = JsonSchema({"type": typ})
-                        else:
-                            prop = JsonSchema({"type": typ, "format": fmt})
+                    prop = JsonSchema.ref_for(reference)
+            else:
+                if reference is not None:
+                    prop = JsonSchema.ref_for(reference)
+                elif typ and fmt is None:
+                    prop = JsonSchema({"type": typ})
+                elif typ:
+                    prop = JsonSchema({"type": typ, "format": fmt})
+
+                if slot_is_multivalued:
+                    prop = JsonSchema.array_of(prop)
 
         prop.add_keyword('description', slot.description)
 
         own_constraints = self.get_value_constraints_for_slot(slot)
 
         if prop.is_array:
             all_element_constraints = self.get_value_constraints_for_slot(slot.all_members)
@@ -437,29 +413,38 @@
         else:
             prop.update(own_constraints)
 
         if prop.is_object:
             prop.add_keyword('minProperties', slot.minimum_cardinality)
             prop.add_keyword('maxProperties', slot.maximum_cardinality)
 
+        bool_subschema = JsonSchema()
         if slot.any_of is not None and len(slot.any_of) > 0:
-            if not slot_has_range_union:
-                prop['anyOf'] = [self.get_subschema_for_slot(s, omit_type=True) for s in slot.any_of]
+            bool_subschema['anyOf'] = [self.get_subschema_for_slot(s) for s in slot.any_of]
 
         if slot.all_of is not None and len(slot.all_of) > 0:
-            prop['allOf'] = [self.get_subschema_for_slot(s, omit_type=True) for s in slot.all_of]
+            bool_subschema['allOf'] = [self.get_subschema_for_slot(s) for s in slot.all_of]
 
         if slot.exactly_one_of is not None and len(slot.exactly_one_of) > 0:
-            prop['oneOf'] = [self.get_subschema_for_slot(s, omit_type=True) for s in slot.exactly_one_of]
+            bool_subschema['oneOf'] = [self.get_subschema_for_slot(s) for s in slot.exactly_one_of]
 
         if slot.none_of is not None and len(slot.none_of) > 0:
-            prop['not'] = {
-                'anyOf': [self.get_subschema_for_slot(s, omit_type=True) for s in slot.none_of]
+            bool_subschema['not'] = {
+                'anyOf': [self.get_subschema_for_slot(s) for s in slot.none_of]
             }
 
+        if bool_subschema:
+            if prop.is_array:
+                if 'items' not in prop:
+                    prop['items'] = {}
+                prop["type"] = "array"
+                prop['items'].update(bool_subschema)
+            else:
+                prop.update(bool_subschema)
+
         return prop
 
 
     def handle_class_slot(self, subschema: JsonSchema, cls: ClassDefinition, slot: SlotDefinition) -> None:
         class_id_slot = self.schemaview.get_identifier_slot(cls.name, use_key=True)
         slot_is_required = slot.required or slot == class_id_slot
```

### Comparing `linkml-1.5.2/linkml/generators/linkmlgen.py` & `linkml-1.5.3/linkml/generators/linkmlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/markdowngen.py` & `linkml-1.5.3/linkml/generators/markdowngen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/namespacegen.py` & `linkml-1.5.3/linkml/generators/namespacegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/oocodegen.py` & `linkml-1.5.3/linkml/generators/oocodegen.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import abc
 import re
 import unicodedata
 from dataclasses import dataclass, field
 from typing import List, Optional, Dict
 
 from linkml_runtime.linkml_model.meta import (ClassDefinition,
+                                              EnumDefinition, EnumDefinitionName,
                                               SchemaDefinition, SlotDefinition,
                                               TypeDefinition)
 from linkml_runtime.utils.formatutils import camelcase, lcamelcase, underscore
 from linkml_runtime.utils.schemaview import SchemaView
 
 from linkml.utils.generator import Generator
 
@@ -123,14 +124,45 @@
 
             safe_label = ""
             for character in label:
                 safe_label += self.replace_invalid_identifier_character(character)
 
             return safe_label
 
+    def generate_enums(
+        self, all_enums: Dict[EnumDefinitionName, EnumDefinition]
+    ) -> Dict:
+        # TODO: make an explicit class to represent how an enum is passed to the template
+        enums = {}
+        for enum_name, enum_original in all_enums.items():
+            enum = {
+                "name": camelcase(enum_name),
+                "values": {}
+            }
+
+            if hasattr(enum_original, "description"):
+                enum["description"] = enum_original.description
+
+            for pv in enum_original.permissible_values.values():
+                label = self.generate_enum_label(pv.text)
+                val = {
+                    "label": label,
+                    "value": pv.text.replace('"', '\\"')
+                }
+                if hasattr(pv, "description"):
+                    val["description"] = pv.description
+                else :
+                    val["description"] = None
+
+                enum["values"][label] = val
+                
+            enums[enum_name] = enum
+
+        return enums
+
     def create_documents(self) -> List[OODocument]:
         """
         Currently hardcoded for java-style
         :return:
         """
         sv: SchemaView
         sv = self.schemaview
```

### Comparing `linkml-1.5.2/linkml/generators/owlgen.py` & `linkml-1.5.3/linkml/generators/owlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/prefixmapgen.py` & `linkml-1.5.3/linkml/generators/prefixmapgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/projectgen.py` & `linkml-1.5.3/linkml/generators/projectgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/protogen.py` & `linkml-1.5.3/linkml/generators/protogen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/pydanticgen.py` & `linkml-1.5.3/linkml/generators/pydanticgen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
+import logging
 import os
 import logging
 from collections import defaultdict
 from copy import deepcopy
-from dataclasses import dataclass, field
-from typing import Dict, List, Optional, Set, TextIO, Union
+from dataclasses import field, dataclass
+from types import ModuleType
+from typing import Dict, List, TextIO, Union, Optional, Set
+
+from linkml_runtime.utils.compile_python import compile_python
+
+from linkml.utils.ifabsent_functions import ifabsent_value_declaration
 
 import click
 from jinja2 import Template
 # from linkml.generators import pydantic_GEN_VERSION
 from linkml_runtime.linkml_model.meta import (Annotation,
                                               AnonymousSlotExpression,
                                               ClassDefinition, EnumDefinition,
@@ -28,17 +34,23 @@
 {#-
 
   Jinja2 Template for a pydantic classes
 -#}
 from __future__ import annotations
 from datetime import datetime, date
 from enum import Enum
-from typing import List, Dict, Optional, Any, Union, Literal
+from typing import List, Dict, Optional, Any, Union
 from pydantic import BaseModel as BaseModel, Field
 from linkml_runtime.linkml_model import Decimal
+import sys
+if sys.version_info >= (3, 8):
+    from typing import Literal
+else:
+    from typing_extensions import Literal
+
 
 metamodel_version = "{{metamodel_version}}"
 version = "{{version if version else None}}"
 
 class WeakRefShimBaseModel(BaseModel):
    __slots__ = '__weakref__'
 
@@ -54,16 +66,19 @@
 {% for e in enums.values() %}
 class {{ e.name }}(str, Enum):
     {% if e.description -%}
     \"\"\"
     {{ e.description }}
     \"\"\"
     {%- endif %}
-    {% for label, value in e['values'].items() -%}
-    {{label}} = "{{value}}"
+    {% for _, pv in e['values'].items() -%}
+    {% if pv.description -%}
+    # {{pv.description}}
+    {%- endif %}
+    {{pv.label}} = "{{pv.value}}"
     {% endfor %}
     {% if not e['values'] -%}
     dummy = "dummy"
     {% endif %}
 {% endfor %}
 
 {%- for c in schema.classes.values() %}
@@ -79,14 +94,16 @@
     {{ c.description }}
     \"\"\"
     {%- endif %}
     {% for attr in c.attributes.values() if c.attributes -%}
     {{attr.name}}: {{ attr.annotations['python_range'].value }} = Field(
     {%- if predefined_slot_values[c.name][attr.name] -%}
         {{ predefined_slot_values[c.name][attr.name] }}
+    {%- elif attr.required -%}
+        ...
     {%- else -%}
         None
     {%- endif -%}
     {%- if attr.title != None %}, title="{{attr.title}}"{% endif -%}
     {%- if attr.description %}, description=\"\"\"{{attr.description}}\"\"\"{% endif -%}
     {%- if attr.minimum_value != None %}, ge={{attr.minimum_value}}{% endif -%}
     {%- if attr.maximum_value != None %}, le={{attr.maximum_value}}{% endif -%}
@@ -112,15 +129,15 @@
     if t.base == "XSDDateTime":
         pyrange = "datetime "
     if t.base == "XSDDate":
         pyrange = "date"
     if pyrange is None and t.typeof is not None:
         pyrange = _get_pyrange(sv.get_type(t.typeof), sv)
     if pyrange is None:
-        raise Exception(f"No python type for range: {s.range} // {t}")
+        raise Exception(f"No python type for range: {t.name} // {t}")
     return pyrange
 
 
 @dataclass
 class PydanticGenerator(OOCodeGenerator):
     """
     Generates Pydantic-compliant classes from a schema
@@ -140,29 +157,26 @@
 
     # ObjectVars (identical to pythongen)
     gen_classvars: bool = field(default_factory=lambda: True)
     gen_slots: bool = field(default_factory=lambda: True)
     genmeta: bool = field(default_factory=lambda: False)
     emit_metadata: bool = field(default_factory=lambda: True)
 
-    def generate_enums(
-        self, all_enums: Dict[EnumDefinitionName, EnumDefinition]
-    ) -> Dict[str, dict]:
-        # TODO: make an explicit class to represent how an enum is passed to the template
-        enums = {}
-        for enum_name, enum_original in all_enums.items():
-            enum = {"name": camelcase(enum_name), "values": {}}
-
-            for pv in enum_original.permissible_values.values():
-                label = self.generate_enum_label(pv.text)
-                enum["values"][label] = pv.text.replace('"', '\\"')
-
-            enums[enum_name] = enum
-
-        return enums
+    def compile_module(self, **kwargs) -> ModuleType:
+        """
+        Compiles generated python code to a module
+        :return:
+        """
+        pycode = self.serialize(**kwargs)
+        try:
+            return compile_python(pycode)
+        except NameError as e:
+            logging.error(f"Code:\n{pycode}")
+            logging.error(f"Error compiling generated python code: {e}")
+            raise e
 
     def sort_classes(self, clist: List[ClassDefinition]) -> List[ClassDefinition]:
         """
         sort classes such that if C is a child of P then C appears after P in the list
 
         Overridden method include mixin classes
 
@@ -441,16 +455,14 @@
                 f"Slot with any_of range has multiple identifier slot range types: {collection_keys}"
             )
         if len(collection_keys) == 1:
             return list(collection_keys)[0]
         return None
 
     def serialize(self) -> str:
-        sv = self.schemaview
-
         if self.template_file is not None:
             with open(self.template_file) as template_file:
                 template_obj = Template(template_file.read())
         else:
             template_obj = Template(default_template)
 
         sv: SchemaView
@@ -492,15 +504,17 @@
                 s.name = underscore(s.name)
                 if s.description:
                     s.description = s.description.replace('"', '\\"')
                 class_def.attributes[s.name] = s
 
                 slot_ranges: List[str] = []
 
-                if len(s.any_of) > 0 and s.range is not None:
+                # Confirm that the original slot range (ignoring the default that comes in from
+                # induced_slot) isn't in addition to setting any_of
+                if len(s.any_of) > 0 and sv.get_slot(sn).range is not None:
                     raise ValueError("Slot cannot have both range and any_of defined")
 
                 if s.any_of is not None and len(s.any_of) > 0:
                     # list comprehension here is pulling ranges from within AnonymousSlotExpression
                     slot_ranges.extend([r.range for r in s.any_of])
                 else:
                     slot_ranges.append(s.range)
```

### Comparing `linkml-1.5.2/linkml/generators/pythongen.py` & `linkml-1.5.3/linkml/generators/pythongen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/rdfgen.py` & `linkml-1.5.3/linkml/generators/rdfgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/shaclgen.py` & `linkml-1.5.3/linkml/generators/shaclgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/shexgen.py` & `linkml-1.5.3/linkml/generators/shexgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/sparqlgen.py` & `linkml-1.5.3/linkml/generators/sparqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py` & `linkml-1.5.3/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py` & `linkml-1.5.3/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/sqlalchemygen.py` & `linkml-1.5.3/linkml/generators/sqlalchemygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/sqlddlgen.py` & `linkml-1.5.3/linkml/generators/sqlddlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/sqltablegen.py` & `linkml-1.5.3/linkml/generators/sqltablegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/sssomgen.py` & `linkml-1.5.3/linkml/generators/sssomgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/string_template.md` & `linkml-1.5.3/linkml/generators/string_template.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/summarygen.py` & `linkml-1.5.3/linkml/generators/summarygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/terminusdbgen.py` & `linkml-1.5.3/linkml/generators/terminusdbgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/typescriptgen.py` & `linkml-1.5.3/linkml/generators/typescriptgen.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,85 +5,108 @@
 from pathlib import Path
 from typing import (Callable, Dict, Iterator, List, Optional, Set, TextIO,
                     Tuple, Union)
 
 import click
 from jinja2 import Environment, FileSystemLoader, Template
 from linkml_runtime.dumpers import yaml_dumper
-from linkml_runtime.linkml_model.meta import (Annotation, ClassDefinition,
-                                              ClassDefinitionName, Definition,
-                                              DefinitionName, Element,
-                                              EnumDefinition, SchemaDefinition,
-                                              SlotDefinition,
-                                              SlotDefinitionName,
-                                              TypeDefinition)
+from linkml_runtime.linkml_model.meta import (
+    Annotation, ClassDefinition,
+    ClassDefinitionName, Definition,
+    DefinitionName, Element,
+    EnumDefinition, SchemaDefinition,
+    SlotDefinition,
+    SlotDefinitionName,
+    TypeDefinition
+)
 from linkml_runtime.utils.formatutils import camelcase, underscore
 from linkml_runtime.utils.schemaview import SchemaView
 
 from linkml._version import __version__
-from linkml.utils.generator import Generator, shared_arguments
+from linkml.generators.oocodegen import OOCodeGenerator
+from linkml.utils.generator import shared_arguments
 
 type_map = {
     "str": "string",
     "int": "number",
     "Bool": "boolean",
     "float": "number",
     "XSDDate": "date",
 }
 
 default_template = """
 {%- for c in view.all_classes().values() -%}
 {%- set cref = gen.classref(c) -%}
 {% if cref -%}
-export type {{cref}} = string
+export type {{cref}} = string;
 {% endif -%}
 {%- endfor -%}
 
+{% for e in enums.values() %}
+{%- if e.description -%}
+/**
+* {{e.description}}
+*/
+{%- endif %}
+export enum {{e.name}} {
+    {% if not e.values -%}
+    dummy = "dummy"
+    {%- endif %}
+    {%- for _, pv in e['values'].items() %}
+    {% if pv.description -%}
+    /** {{pv.description}} */
+    {% endif -%}
+    {{pv.label}} = "{{pv.value}}",    
+    {%- endfor %}
+};
+{% endfor %}
+
 {% for c in view.all_classes().values() -%}
 {%- if c.description -%}
 /**
  * {{c.description}}
  */
 {%- endif -%} 
 {% set parents = gen.parents(c) %}
-export interface {{gen.name(c)}} {% if parents %} extends {{parents|join(', ')}} {% endif %} {
+export interface {{gen.name(c)}} {%- if parents %} extends {{parents|join(', ')}} {%- endif %} {
     {%- for sn in view.class_slots(c.name, direct=False) %}
     {% set s = view.induced_slot(sn, c.name) %}
     {%- if s.description -%}
-    /**
-     * {{s.description}}
-     */
-     {%- endif -%}
-    {{gen.name(s)}}?: {{gen.range(s)}},
+    /** {{s.description}} */
+    {% endif -%}
+    {{gen.name(s)}}{%- if not s.required -%}?{%- endif -%}: {{gen.range(s)}},
     {%- endfor %}
-}
+};
 {% endfor %}
 """
 
 
 @dataclass
-class TypescriptGenerator(Generator):
+class TypescriptGenerator(OOCodeGenerator):
     """
     Generates typescript from a schema
     """
 
     # ClassVars
     generatorname = os.path.basename(__file__)
     generatorversion = "0.0.1"
     valid_formats = ["text"]
     uses_schemaloader = False
 
     def serialize(self) -> str:
-        """
-        Serialize a schema to typescript string
-        :return:
-        """
+        """Serialize a schema to typescript string"""
+
+        sv: SchemaView = self.schemaview
+        enums = self.generate_enums(sv.all_enums())
         template_obj = Template(default_template)
         out_str = template_obj.render(
-            gen=self, schema=self.schemaview.schema, view=self.schemaview
+            gen=self,
+            schema=self.schemaview.schema,
+            view=self.schemaview,
+            enums=enums,
         )
         return out_str
 
     def name(self, element: Element) -> str:
         """
         Returns the name of the element in its canonical form
 
@@ -147,27 +170,33 @@
                 if not id_slot or slot.inlined:
                     return rc_name
                 else:
                     return f"{rc_ref}"
         else:
             if r in sv.all_types():
                 t = sv.get_type(r)
+                tsrange = "string"
                 if t.base and t.base in type_map:
-                    return type_map[t.base]
+                    tsrange = type_map[t.base]
                 else:
                     logging.warning(f"Unknown type.base: {t.name}")
+                if slot.multivalued:
+                    tsrange = f"{tsrange}[]"
+                return tsrange
             return "string"
 
     def parents(self, cls: ClassDefinition) -> List[ClassDefinitionName]:
         if cls.is_a:
             parents = [cls.is_a]
         else:
             parents = []
         return [ClassDefinitionName(camelcase(p)) for p in parents + cls.mixins]
 
+    def default_value_for_type(self, typ: str) -> str:
+        pass
 
 @shared_arguments(TypescriptGenerator)
 @click.version_option(__version__, "-V", "--version")
 @click.command()
 def cli(yamlfile, **args):
     """Generate typescript interfaces and types
```

### Comparing `linkml-1.5.2/linkml/generators/yamlgen.py` & `linkml-1.5.3/linkml/generators/yamlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/generators/yumlgen.py` & `linkml-1.5.3/linkml/generators/yumlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/cli.py` & `linkml-1.5.3/linkml/linter/cli.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/config/datamodel/config.py` & `linkml-1.5.3/linkml/linter/config/datamodel/config.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/config/datamodel/config.yaml` & `linkml-1.5.3/linkml/linter/config/datamodel/config.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/config/default.yaml` & `linkml-1.5.3/linkml/linter/config/default.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/formatters/formatter.py` & `linkml-1.5.3/linkml/linter/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/formatters/json_formatter.py` & `linkml-1.5.3/linkml/linter/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/formatters/markdown_formatter.py` & `linkml-1.5.3/linkml/linter/formatters/markdown_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/formatters/terminal_formatter.py` & `linkml-1.5.3/linkml/linter/formatters/terminal_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/formatters/tsv_formatter.py` & `linkml-1.5.3/linkml/linter/formatters/tsv_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/linter.py` & `linkml-1.5.3/linkml/linter/linter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/linter/rules.py` & `linkml-1.5.3/linkml/linter/rules.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/reporting/model.py` & `linkml-1.5.3/linkml/reporting/model.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/transformers/relmodel_transformer.py` & `linkml-1.5.3/linkml/transformers/relmodel_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/transformers/schema_renamer.py` & `linkml-1.5.3/linkml/transformers/schema_renamer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/converter.py` & `linkml-1.5.3/linkml/utils/converter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/datautils.py` & `linkml-1.5.3/linkml/utils/datautils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/execute_tutorial.py` & `linkml-1.5.3/linkml/utils/execute_tutorial.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/generator.py` & `linkml-1.5.3/linkml/utils/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
 
     def _initialize_using_schemaloader(self, schema: Union[str, TextIO, SchemaDefinition, "Generator"]):
         # currently generators are very liberal in what they accept, including
         # other generators.
         # See https://github.com/linkml/linkml/issues/923 for discussion on how
         # to simplify the overall framework
         if isinstance(schema, Generator):
-            logging.warning("Instantiating generator with another generator is deprecated")
+            logging.info("Instantiating generator with another generator is deprecated")
             gen = schema
             self.schema = gen.schema
             self.synopsis = gen.synopsis
             self.loaded = gen.loaded
             self.namespaces = gen.namespaces
             self.base_dir = gen.base_dir
             self.importmap = gen.importmap
```

### Comparing `linkml-1.5.2/linkml/utils/ifabsent_functions.py` & `linkml-1.5.3/linkml/utils/ifabsent_functions.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/mergeutils.py` & `linkml-1.5.3/linkml/utils/mergeutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/rawloader.py` & `linkml-1.5.3/linkml/utils/rawloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/schema_builder.py` & `linkml-1.5.3/linkml/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/schema_fixer.py` & `linkml-1.5.3/linkml/utils/schema_fixer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/schemaloader.py` & `linkml-1.5.3/linkml/utils/schemaloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/schemasynopsis.py` & `linkml-1.5.3/linkml/utils/schemasynopsis.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/sqlutils.py` & `linkml-1.5.3/linkml/utils/sqlutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/typereferences.py` & `linkml-1.5.3/linkml/utils/typereferences.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/utils/validation.py` & `linkml-1.5.3/linkml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/validators/jsonschemavalidator.py` & `linkml-1.5.3/linkml/validators/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/validators/sparqlvalidator.py` & `linkml-1.5.3/linkml/validators/sparqlvalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/workspaces/datamodel/workspaces.py` & `linkml-1.5.3/linkml/workspaces/datamodel/workspaces.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/workspaces/datamodel/workspaces.yaml` & `linkml-1.5.3/linkml/workspaces/datamodel/workspaces.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.2/linkml/workspaces/example_runner.py` & `linkml-1.5.3/linkml/workspaces/example_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,16 @@
                             f"### Input",
                             f"```yaml",
                             f"{yaml.dump(input_dict)}",
                             f"```")
                 success = True
                 try:
                     validator.validate_dict(input_dict, tc, closed=True)
+                    # json validation is incomplete: also try object instantiation
+                    self._load_from_dict(input_dict, target_class=tc)
                 except Exception as e:
                     success = False
                     if not counter_examples:
                         raise ValueError(f"Example {input_example} failed validation: {e}")
                 if counter_examples:
                     if success:
                         raise ValueError(f"Counter example {input_example} succeeded validation")
```

### Comparing `linkml-1.5.2/pyproject.toml` & `linkml-1.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml"
-version = "1.5.2"
+version = "1.5.3"
 description = "Linked Open Data Modeling Language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sujay Patil <spatil@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>",
     "Sierra Moxon <smoxon@lbl.gov>",
@@ -48,14 +48,15 @@
 style = "pep440"
 
 [tool.poetry.scripts]    
 gen-jsonld-context = "linkml.generators.jsonldcontextgen:cli"
 gen-prefix-map = "linkml.generators.prefixmapgen:cli"
 gen-csv = "linkml.generators.csvgen:cli"
 gen-graphviz = "linkml.generators.dotgen:cli"
+gen-golang = "linkml.generators.golanggen:cli"
 gen-golr-views = "linkml.generators.golrgen:cli"
 gen-graphql = "linkml.generators.graphqlgen:cli"
 gen-java = "linkml.generators.javagen:cli"
 gen-jsonld = "linkml.generators.jsonldgen:cli"
 gen-json-schema = "linkml.generators.jsonschemagen:cli"
 gen-markdown = "linkml.generators.markdowngen:cli"
 gen-doc = "linkml.generators.docgen:cli"
@@ -121,16 +122,17 @@
 requests = ">=2.22"
 sphinx = "*"
 sphinx-click = "*"
 sphinx-rtd-theme = "*"
 sqlalchemy = ">=1.4.31"
 watchdog = ">=0.9.0"
 tox = "^3.25.1"
-furo = {version = "^2022.9.29", extras = ["docs"]}
+furo = {version = "^2023.03.27", extras = ["docs"]}
 sphinxcontrib-mermaid = {version = "^0.7.1", extras = ["docs"]}
+typing-extensions = {version = "^4.5.0", python = "3.7"}
 
 [tool.poetry.dev-dependencies]
 chardet = "*"
 ipykernel = "*"
 ipython-genutils = "*"
 nbconvert = "*"
 nbformat = "*"
```

### Comparing `linkml-1.5.2/setup.py` & `linkml-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,22 +49,24 @@
  'sphinx-rtd-theme',
  'sqlalchemy>=1.4.31',
  'tox>=3.25.1,<4.0.0',
  'watchdog>=0.9.0']
 
 extras_require = \
 {':extra == "docs"': ['sphinx',
-                      'furo[docs]>=2022.9.29,<2023.0.0',
-                      'sphinxcontrib-mermaid[docs]>=0.7.1,<0.8.0']}
+                      'furo[docs]>=2023.03.27,<2024.0.0',
+                      'sphinxcontrib-mermaid[docs]>=0.7.1,<0.8.0'],
+ ':python_version == "3.7"': ['typing-extensions>=4.5.0,<5.0.0']}
 
 entry_points = \
 {'console_scripts': ['gen-csv = linkml.generators.csvgen:cli',
                      'gen-doc = linkml.generators.docgen:cli',
                      'gen-erdiagram = linkml.generators.erdiagramgen:cli',
                      'gen-excel = linkml.generators.excelgen:cli',
+                     'gen-golang = linkml.generators.golanggen:cli',
                      'gen-golr-views = linkml.generators.golrgen:cli',
                      'gen-graphql = linkml.generators.graphqlgen:cli',
                      'gen-graphviz = linkml.generators.dotgen:cli',
                      'gen-java = linkml.generators.javagen:cli',
                      'gen-json-schema = linkml.generators.jsonschemagen:cli',
                      'gen-jsonld = linkml.generators.jsonldgen:cli',
                      'gen-jsonld-context = '
@@ -106,15 +108,15 @@
                      'linkml-sqldb = linkml.utils.sqlutils:main',
                      'linkml-validate = '
                      'linkml.validators.jsonschemavalidator:cli',
                      'run-tutorial = linkml.utils.execute_tutorial:cli']}
 
 setup_kwargs = {
     'name': 'linkml',
-    'version': '1.5.2',
+    'version': '1.5.3',
     'description': 'Linked Open Data Modeling Language',
     'long_description': '[![Pyversions](https://img.shields.io/pypi/pyversions/linkml.svg)](https://pypi.python.org/pypi/linkml)\n![](https://github.com/linkml/linkml/workflows/Build/badge.svg)\n[![PyPi](https://img.shields.io/pypi/v/linkml.svg)](https://pypi.python.org/pypi/linkml)\n[![badge](https://img.shields.io/badge/launch-binder-579ACA.svg)](https://mybinder.org/v2/gh/linkml/linkml/main?filepath=notebooks)\n[![DOI](https://zenodo.org/badge/13996/linkml/linkml.svg)](https://zenodo.org/badge/latestdoi/13996/linkml/linkml)\n[![PyPIDownloadsTotal](https://pepy.tech/badge/linkml)](https://pepy.tech/project/linkml)\n[![PyPIDownloadsMonth](https://img.shields.io/pypi/dm/linkml?logo=PyPI&color=blue)](https://pypi.org/project/linkml)\n[![codecov](https://codecov.io/gh/linkml/linkml/branch/main/graph/badge.svg?token=WNQNG986UN)](https://codecov.io/gh/linkml/linkml)\n\n\n# LinkML - Linked Data Modeling Language\n\nLinkML is a linked data modeling language following object-oriented and ontological principles. LinkML models are typically authored in YAML, and can be converted to other schema representation formats such as JSON or RDF.\n\nThis repo holds the tools for generating and working with LinkML. For the LinkML schema (metamodel), please see https://github.com/linkml/linkml-model\n\nThe complete documentation for LinkML can be found here:\n\n - [linkml.io/linkml](https://linkml.io/linkml)\n',
     'author': 'Chris Mungall',
     'author_email': 'cjmungall@lbl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://linkml.io/linkml/',
```

### Comparing `linkml-1.5.2/PKG-INFO` & `linkml-1.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml
-Version: 1.5.2
+Version: 1.5.3
 Summary: Linked Open Data Modeling Language
 Home-page: https://linkml.io/linkml/
 Keywords: schema,linked data,data modeling,rdf,owl,biolink
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Requires-Dist: antlr4-python3-runtime (>=4.9.0,<4.10)
 Requires-Dist: click (>=7.0)
-Requires-Dist: furo[docs] (>=2022.9.29,<2023.0.0) ; extra == "docs"
+Requires-Dist: furo[docs] (>=2023.03.27,<2024.0.0) ; extra == "docs"
 Requires-Dist: graphviz (>=0.10.1)
 Requires-Dist: hbreader
 Requires-Dist: isodate (>=0.6.0)
 Requires-Dist: jinja2 (>=3.1.0)
 Requires-Dist: jsonasobj2 (>=1.0.3,<2.0.0)
 Requires-Dist: jsonschema[format] (>=4.0.0)
 Requires-Dist: linkml-dataops
@@ -50,14 +50,15 @@
 Requires-Dist: requests (>=2.22)
 Requires-Dist: sphinx ; extra == "docs"
 Requires-Dist: sphinx-click
 Requires-Dist: sphinx-rtd-theme
 Requires-Dist: sphinxcontrib-mermaid[docs] (>=0.7.1,<0.8.0) ; extra == "docs"
 Requires-Dist: sqlalchemy (>=1.4.31)
 Requires-Dist: tox (>=3.25.1,<4.0.0)
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ; python_version == "3.7"
 Requires-Dist: watchdog (>=0.9.0)
 Project-URL: Documentation, https://linkml.io/linkml/
 Project-URL: Repository, https://github.com/linkml/linkml
 Description-Content-Type: text/markdown
 
 [![Pyversions](https://img.shields.io/pypi/pyversions/linkml.svg)](https://pypi.python.org/pypi/linkml)
 ![](https://github.com/linkml/linkml/workflows/Build/badge.svg)
```

