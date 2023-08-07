# Comparing `tmp/irispie-0.1.6.tar.gz` & `tmp/irispie-0.2.0.tar.gz`

## Comparing `irispie-0.1.6.tar` & `irispie-0.2.0.tar`

### file list

```diff
@@ -1,80 +1,83 @@
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 irispie-0.1.6/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 irispie-0.1.6/.github/workflows/test.yml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/.obsidian/app.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/.obsidian/appearance.json
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/.obsidian/core-plugins.json
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/.obsidian/hotkeys.json
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/.obsidian/workspace.json
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/algorithms/detach-unit-roots.md
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/architecture/Untitled.md
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/architecture/steady.canvas
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/dates/Ranger.md
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/milestones/March-2023.md
--rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/milestones/iris-gray.png
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.1.6/docs/series/example.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/__init__.py
--rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/equations.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/exceptions.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/incidence.py
--rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/quantities.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/requirements
--rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/session
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/tags
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/wrongdoings.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/aldi/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/aldi/adaptations.py
--rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/aldi/differentiators.py
--rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/aldi/express.py~
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/aldi/finite_differentiators.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/aldi/invariators.py
--rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/aldi/maps.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/__init__.py
--rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/databanks.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/dataslabs.py
--rw-r--r--   0        0        0    20362 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/dates.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/exports.py
--rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/filters.py
--rw-r--r--   0        0        0     5304 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/imports.py
--rw-r--r--   0        0        0     7526 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/imports2.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/plotly.py
--rw-r--r--   0        0        0    18655 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/series.py
--rw-r--r--   0        0        0     4539 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/dataman/views.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/equators/__init__.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/equators/abc.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/equators/plain.py
--rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/equators/steady.py
--rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/evaluators/printers.py
--rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/evaluators/steady.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/fords/__init__.py
--rw-r--r--   0        0        0    15846 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/fords/descriptors.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/fords/simulators.py
--rw-r--r--   0        0        0     9038 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/fords/solutions.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/fords/steadiers.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/fords/systems.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/jacobians/abc.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/jacobians/steady.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/mixins/userdata.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/models/__init__.py
--rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/models/facade.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/models/flags.py
--rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/models/gettables.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/models/invariants.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/models/simulatables.py
--rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/models/sources.py
--rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/models/steadiables.py
--rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/models/variants.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/parsers/__init__.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/parsers/common.py
--rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/parsers/model_source_parser.py
--rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/parsers/preparser.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/parsers/pseudofunctions.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/parsers/shifts.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.1.6/src/irispie/parsers/substitutions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.1.6/tests/.gitkeep
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 irispie-0.1.6/tests/dataman/series/hpf_test.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.1.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.1.6/LICENCE
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.1.6/README.md
--rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 irispie-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 irispie-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 irispie-0.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 irispie-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/.obsidian/app.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/.obsidian/appearance.json
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/.obsidian/hotkeys.json
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/.obsidian/workspace.json
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/algorithms/detach-unit-roots.md
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/architecture/Untitled.md
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/architecture/steady.canvas
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/dates/Ranger.md
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/milestones/March-2023.md
+-rw-r--r--   0        0        0    26724 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/milestones/iris-gray.png
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 irispie-0.2.0/docs/series/example.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/__init__.py
+-rw-r--r--   0        0        0     8577 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/equations.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/exceptions.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/incidence.py
+-rw-r--r--   0        0        0     6364 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/quantities.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/requirements
+-rw-r--r--   0        0        0     8751 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/session
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/tags
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/wrongdoings.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/aldi/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/aldi/adaptations.py
+-rw-r--r--   0        0        0    13603 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/aldi/differentiators.py
+-rw-r--r--   0        0        0     5989 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/aldi/express.py~
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/aldi/finite_differentiators.py
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/aldi/invariators.py
+-rw-r--r--   0        0        0     4526 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/aldi/maps.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/dataman/__init__.py
+-rw-r--r--   0        0        0    11507 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/dataman/databanks.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/dataman/dataslabs.py
+-rw-r--r--   0        0        0    22215 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/dataman/dates.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/dataman/exports.py
+-rw-r--r--   0        0        0     5312 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/dataman/imports.py
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/dataman/imports2.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/equators/__init__.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/equators/abc.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/equators/plain.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/equators/steady.py
+-rw-r--r--   0        0        0     6104 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/evaluators/printers.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/evaluators/steady.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/fords/__init__.py
+-rw-r--r--   0        0        0    15846 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/fords/descriptors.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/fords/simulators.py
+-rw-r--r--   0        0        0     9038 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/fords/solutions.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/fords/steadiers.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/fords/systems.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/jacobians/abc.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/jacobians/steady.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/models/__init__.py
+-rw-r--r--   0        0        0    12567 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/models/facade.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/models/flags.py
+-rw-r--r--   0        0        0     6779 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/models/gettables.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/models/invariants.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/models/simulatables.py
+-rw-r--r--   0        0        0     9895 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/models/sources.py
+-rw-r--r--   0        0        0     6094 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/models/steadiables.py
+-rw-r--r--   0        0        0     5802 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/models/variants.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/parsers/__init__.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/parsers/common.py
+-rw-r--r--   0        0        0     7940 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/parsers/model_source_parser.py
+-rw-r--r--   0        0        0     8130 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/parsers/preparser.py
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/parsers/pseudofunctions.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/parsers/shifts.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/parsers/substitutions.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/series/__init__.py
+-rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/series/conversion.py
+-rw-r--r--   0        0        0    18690 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/series/facade.py
+-rw-r--r--   0        0        0     6968 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/series/filters.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/series/plotly.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/user/description.py
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 irispie-0.2.0/src/irispie/user/views.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 irispie-0.2.0/tests/.gitkeep
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 irispie-0.2.0/tests/dataman/dates/sdmx_dates.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 irispie-0.2.0/tests/dataman/series/hpf_test.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 irispie-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 irispie-0.2.0/LICENCE
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 irispie-0.2.0/README.md
+-rw-r--r--   0        0        0      944 2020-02-02 00:00:00.000000 irispie-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 irispie-0.2.0/PKG-INFO
```

### Comparing `irispie-0.1.6/.github/workflows/publish-to-pypi.yml` & `irispie-0.2.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/docs/.obsidian/core-plugins-migration.json` & `irispie-0.2.0/docs/.obsidian/core-plugins-migration.json`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/docs/.obsidian/workspace.json` & `irispie-0.2.0/docs/.obsidian/workspace.json`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/docs/algorithms/detach-unit-roots.md` & `irispie-0.2.0/docs/algorithms/detach-unit-roots.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/docs/milestones/March-2023.md` & `irispie-0.2.0/docs/milestones/March-2023.md`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/docs/milestones/iris-gray.png` & `irispie-0.2.0/docs/milestones/iris-gray.png`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/docs/series/example.py` & `irispie-0.2.0/docs/series/example.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/equations.py` & `irispie-0.2.0/src/irispie/equations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/exceptions.py` & `irispie-0.2.0/src/irispie/exceptions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/incidence.py` & `irispie-0.2.0/src/irispie/incidence.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/quantities.py` & `irispie-0.2.0/src/irispie/quantities.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/requirements` & `irispie-0.2.0/src/irispie/requirements`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/session` & `irispie-0.2.0/src/irispie/session`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/tags` & `irispie-0.2.0/src/irispie/tags`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/wrongdoings.py` & `irispie-0.2.0/src/irispie/wrongdoings.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/aldi/adaptations.py` & `irispie-0.2.0/src/irispie/aldi/adaptations.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/aldi/differentiators.py` & `irispie-0.2.0/src/irispie/aldi/differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/aldi/express.py~` & `irispie-0.2.0/src/irispie/aldi/express.py~`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/aldi/finite_differentiators.py` & `irispie-0.2.0/src/irispie/aldi/finite_differentiators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/aldi/invariators.py` & `irispie-0.2.0/src/irispie/aldi/invariators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/aldi/maps.py` & `irispie-0.2.0/src/irispie/aldi/maps.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/dataman/databanks.py` & `irispie-0.2.0/src/irispie/dataman/databanks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 """
 """
 
 
 #[
 from __future__ import annotations
 
-import json as js_
-import copy as co_
-import types as ty_
-import numpy as np_
-import re as re_
-import operator as op_
-import functools as ft_
+import json as _js
+import copy as _co
+import types as _ty
+import numpy as _np
+import re as _re
+import operator as _op
+import functools as _ft
 from typing import (Self, TypeAlias, Literal, Sequence, Protocol, Any, )
 from collections.abc import (Iterable, Callable, )
 from numbers import (Number, )
 
-from ..dataman import (dates as da_, )
-from ..dataman import (series as se_, )
-from ..dataman import (views as vi_, )
-from ..dataman import (imports as im_, )
-from ..dataman import (exports as ex_, )
-from .. import (quantities as qu_, )
-from ..mixins import (userdata as ud_, )
+from ..user import views as _vi
+from ..user import description as _ud
+from ..series import facade as _sf
+from . import dates as _da
+from . import imports as _im
+from . import exports as _ex
 #]
 
 
 __all__ = [
     "Databank",
 ]
 
@@ -71,43 +70,44 @@
 _EXTENDED_RANGE_TUPLE_RESOLUTION = {
     "base": _extended_range_tuple_from_base_range,
     "extended": _extended_range_tuple_from_extended_range,
 }
 
 
 _SERIES_CONSTRUCTOR_RESOLUTION = {
-    "start_date": se_.Series.from_start_date_and_data,
-    "range": se_.Series.from_dates_and_data,
+    "start_date": _sf.Series.from_start_date_and_data,
+    "range": _sf.Series.from_dates_and_data,
 }
 
 
 _ARRAY_TRANSPOSER_RESOLUTION = {
-    "vertical": np_.transpose,
+    "vertical": _np.transpose,
     "horizontal": lambda x: x,
 }
 
 
 class Databank(
-    im_.DatabankImportMixin,
-    ex_.DatabankExportMixin,
-    ud_.DescriptionMixin,
-    vi_.DatabankViewMixin,
-    ty_.SimpleNamespace,
+    _im.DatabankImportMixin,
+    _ex.DatabankExportMixin,
+    _ud.DescriptionMixin,
+    _vi.DatabankViewMixin,
+    _ty.SimpleNamespace,
 ):
     """
     Create a databank object as a simple namespace with utility functions
     """
     #[
     def __init__(
         self,
         /,
         description: str = "",
     ) -> None:
         self.set_description(description)
 
+
     @classmethod
     def _from_dict(
         cls,
         _dict: dict,
         /,
     ) -> Self:
         """
@@ -116,17 +116,17 @@
         for k, v in _dict.items():
             self.__setattr__(k, v)
         return self
 
     @classmethod
     def _from_array(
         cls,
-        array: np_.ndarray,
+        array: _np.ndarray,
         qid_to_name: Sequence[str] | dict[int, str],
-        dates: da_.Dater,
+        dates: _da.Dater,
         /,
         add_to_databank: Self | None = None,
         qid_to_description: dict[int, str] | None = None,
         array_orientation: Literal["vertical"] | Literal["horizontal"] = "vertical",
         interpret_dates: Literal["start_date"] | Literal["range"] = "start_date",
     ) -> Self:
         """
@@ -167,15 +167,15 @@
         self: Self,
         /,
         source_names: SourceNames = None,
         target_names: TargetNames = None,
     ) -> Self:
         """
         """
-        new_databank = co_.deepcopy(self)
+        new_databank = _co.deepcopy(self)
         new_databank = new_databank._rename(source_names, target_names)
         new_databank._keep(target_names)
         return new_databank
 
     def _rename(
         self: Self,
         /,
@@ -247,87 +247,87 @@
             return names
         name_test = name_test if name_test else lambda x: True
         value_test = value_test if value_test else lambda x: True
         return [ n for n in names if name_test(n) and value_test(getattr(self, n)) ]
 
     def _get_series_names_by_frequency(
         self,
-        frequency: da_.Frequency,
+        frequency: _da.Frequency,
     ) -> Iterable[str]:
         """
         """
-        return self._filter(value_test=lambda x: isinstance(x, se_.Series) and x.frequency==frequency)
+        return self._filter(value_test=lambda x: isinstance(x, _sf.Series) and x.frequency==frequency)
 
     def _get_range_by_frequency(
         self,
-        frequency: da_.Frequency,
+        frequency: _da.Frequency,
     ) -> Ranger:
         names = self._get_series_names_by_frequency(frequency)
         if not names:
             return Ranger(None, None)
-        min_start_date = min((getattr(self, n).start_date for n in names), key=op_.attrgetter("serial"))
-        max_end_date = max((getattr(self, n).end_date for n in names), key=op_.attrgetter("serial"))
-        return da_.Ranger(min_start_date, max_end_date)
+        min_start_date = min((getattr(self, n).start_date for n in names), key=_op.attrgetter("serial"))
+        max_end_date = max((getattr(self, n).end_date for n in names), key=_op.attrgetter("serial"))
+        return _da.Ranger(min_start_date, max_end_date)
 
     def _to_json(self, **kwargs):
-        return js_.dumps(vars(self), **kwargs)
+        return _js.dumps(vars(self), **kwargs)
 
     def _underlay(self, other) -> None:
         """"
         """
-        self_names = self._filter(value_test=lambda x: isinstance(x, se_.Series))
-        other_names = other._filter(value_test=lambda x: isinstance(x, se_.Series))
+        self_names = self._filter(value_test=lambda x: isinstance(x, _sf.Series))
+        other_names = other._filter(value_test=lambda x: isinstance(x, _sf.Series))
         names = set(self_names).intersection(other_names)
         for n in names:
             self_n = getattr(self, n)
             other_n = getattr(other, n)
             if self_n.frequency == other_n.frequency:
                 self_n.underlay(other_n)
 
     def _clip(
         self,
-        new_start_date: da_.Dater | None = None,
-        new_end_date: da_.Dater | None = None,
+        new_start_date: _da.Dater | None = None,
+        new_end_date: _da.Dater | None = None,
     ) -> None:
         if new_start_date is None and new_end_date is None:
             return
         frequency = new_start_date.frequency if new_start_date is not None else new_end_date.frequency
-        names = self._filter(value_test=lambda x: isinstance(x, se_.Series) and x.frequency == frequency)
+        names = self._filter(value_test=lambda x: isinstance(x, _sf.Series) and x.frequency == frequency)
         for n in names:
             x = getattr(self, n)
             x.clip(new_start_date, new_end_date)
 
     def _add_steady(
         self,
         steady_databankable: SteadyDatabankableProtocol,
-        input_range: Iterable[da_.Dater],
+        input_range: Iterable[_da.Dater],
         /,
         deviation: bool = False,
         interpret_range: InterpretRange = "base",
     ) -> Self:
         """
         """
         min_shift, max_shift = steady_databankable._get_min_max_shifts()
         start_date, end_date = _resolve_input_range(input_range, min_shift, max_shift, interpret_range)
         num_columns = int(end_date - start_date + 1)
         if num_columns < 1:
             raise Exception("Empty date range is not allowed when creating steady databank")
         steady_databank = steady_databankable._get_steady_databank(start_date, end_date, deviation=deviation)
         self._update(steady_databank)
 
-    _add_zero = ft_.partialmethod(_add_steady, deviation=True)
+    _add_zero = _ft.partialmethod(_add_steady, deviation=True)
 
     def __getitem__(self, name):
         return self.__dict__[name]
 
     def __setitem__(self, name, value) -> None:
         self.__dict__[name] = value
 
     def __or__(self, other) -> Self:
-        new = co_.deepcopy(self)
+        new = _co.deepcopy(self)
         new.__dict__.update(other.__dict__)
         return new
 
     def _update(
         self,
         other: Databank,
         /,
@@ -338,20 +338,21 @@
         self.__dict__.update(other.__dict__)
     #]
 
 
 #
 # Add databank methods without the leading underscore
 #
+exceptions = ["_description", ]
 single_underscore_names = [
     n for n in dir(Databank) 
-    if n.startswith("_") and not n.startswith("__") and not n.endswith("_")
+    if n.startswith("_") and not n.startswith("__") and not n.endswith("_") and n not in exceptions
 ]
 for n in single_underscore_names:
-    setattr(Databank, n[1:], getattr(Databank, n))
+    setattr(Databank, n.removeprefix("_"), getattr(Databank, n))
 
 
 def _resolve_source_target_names(
     source_names: SourceNames,
     target_names: TargetNames,
     context_names: Iterable[str],
     /,
@@ -372,14 +373,14 @@
     if callable(target_names):
         func = target_names
         target_names = [ func(n) for n in source_names ]
     return source_names, target_names
 
 
 def _resolve_input_range(
-    input_range: Iterable[da_.Dater],
+    input_range: Iterable[_da.Dater],
     min_shift: int,
     max_shift: int,
     interpret_range: InterpretRange,
 ) -> tuple[Dater, Dater]:
     return _EXTENDED_RANGE_TUPLE_RESOLUTION[interpret_range](input_range, min_shift, max_shift)
```

### Comparing `irispie-0.1.6/src/irispie/dataman/dataslabs.py` & `irispie-0.2.0/src/irispie/dataman/dataslabs.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 #[
 from __future__ import annotations
 
 import numpy as np_
 from typing import (Self, )
 from collections.abc import (Iterable, )
 
+from ..series import facade as _sf
 from . import databanks as db_
 from . import dates as da_
-from . import series as se_
 #]
 
 
 class Dataslab:
     """
     """
     #[
@@ -104,12 +104,12 @@
     Add data from a dataslab to a new or existing databank
     """
     out_databank = target_databank if target_databank is not None else db_.Databank()
     self = selves[0]
     num_columns = len(selves)
     for row, n in enumerate(self.row_names):
         data = np_.hstack(tuple(ds.data[(row,), :].T for ds in selves))
-        x = se_.Series(num_columns=num_columns)
+        x = _sf.Series(num_columns=num_columns)
         x.set_data(self.column_dates, data)
         setattr(out_databank, n, x)
     return out_databank
```

### Comparing `irispie-0.1.6/src/irispie/dataman/dates.py` & `irispie-0.2.0/src/irispie/dataman/dates.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 #[
 from __future__ import annotations
 
 import re as _re
 import datetime as _dt
 import enum as _en
 import functools as _ft
-from typing import (Union, Self, Any, Protocol, runtime_checkable, )
+from typing import (Union, Self, Any, Protocol, TypeAlias, runtime_checkable, )
 from collections.abc import (Iterable, Callable, )
 from numbers import (Number, )
 #]
 
 
 __all__ = [
     "Frequency",
     "yy", "hh", "qq", "mm", "dd", "ii",
     "Ranger", "start", "end",
     "dater_from_sdmx_string",
+    "daters_from_sdmx_strings",
     "dater_from_iso_string",
+    "daters_from_iso_strings",
 ]
 
 
 class Frequency(_en.IntEnum):
     """
     Enumeration of date frequencies
     """
@@ -36,40 +38,28 @@
     QUARTERLY = 4
     MONTHLY = 12
     WEEKLY = 52
     DAILY = 365
     UNKNOWN = -1
 
     @property
-    def letter(self) -> str:
+    def letter(self, /, ) -> str:
         return self.name[0] if self is not self.UNKNOWN else "?"
 
     @property
-    def sdmx_format(self) -> str:
-        return SDMX_FORMATS[self]
-
-    @property
-    def plotly_format(self) -> str:
+    def plotly_format(self, /, ) -> str:
         return PLOTLY_FORMATS[self]
 
     @property
-    def is_regular(self) -> bool:
+    def is_regular(self, /, ) -> bool:
         return self in [self.YEARLY, self.HALFYEARLY, self.QUARTERLY, self.MONTHLY]
-    #]
-
 
-SDMX_FORMATS = {
-    Frequency.INTEGER: "({serial})",
-    Frequency.YEARLY: "{year:04g}",
-    Frequency.HALFYEARLY: "{year:04g}-{letter}{per:1g}",
-    Frequency.QUARTERLY: "{year:04g}-{letter}{per:1g}",
-    Frequency.MONTHLY: "{year:04g}-{per:02g}",
-    Frequency.WEEKLY: "{year:04g}-{per:02g}",
-    Frequency.DAILY: "{year:04g}-{month:02g}-{day:02g}",
-}
+    def __str__(self, /, ) -> str:
+        return self.name
+    #]
 
 
 PLOTLY_FORMATS = {
     Frequency.INTEGER: None,
     Frequency.YEARLY: "%Y",
     Frequency.HALFYEARLY: "%Y-%m",
     Frequency.QUARTERLY: "%Y-Q%q",
@@ -120,15 +110,15 @@
 def _check_offset_decorator(func: Callable) -> Callable:
     def wrapper(*args, **kwargs):
         _check_offset(args[1])
         return func(*args, **kwargs)
     return wrapper
 
 
-def _remove_blanks_decorate(func: Callable,) -> Callable:
+def _remove_blanks(func: Callable,) -> Callable:
     def wrapper(*args, **kwargs, ):
         return func(*args, **kwargs, ).replace(" ", "", )
     return wrapper
 
 
 class RangeableMixin:
     #[
@@ -143,19 +133,19 @@
         return Ranger(start_date, self, -1) 
     #]
 
 
 class IsoMixin:
     #[
     def to_iso_string(
-        self: Self,
+        self,
         /,
         position: Literal["start"] | Literal["center"] | Literal["end"] = "start",
     ) -> str:
-        year, month, day = self.to_ymd()
+        year, month, day = self.to_ymd(position=position, )
         return f"{year:04g}-{month:02g}-{day:02g}"
 
     @classmethod
     def from_iso_string(cls: type, iso_string: str, ) -> Self:
         year, month, day = iso_string.split("-", )
         return cls.from_ymd(int(year), int(month), int(day), )
 
@@ -184,14 +174,19 @@
 
     def __len__(self):
         return 1
 
     def __repr__(self) -> str:
         return self.__str__()
 
+    def __str__(self) -> str:
+        return self.to_sdmx_string()
+
+    _databank_repr = __str__
+
     def __format__(self, *args) -> str:
         str_format = args[0] if args else ""
         return ("{date_str:"+str_format+"}").format(date_str=self.__str__())
 
     def __iter__(self) -> Iterable[Self]:
         yield self
 
@@ -242,36 +237,34 @@
 
     @_check_daters_decorate
     def __ge__(self, other) -> bool:
         return self.serial >= other.serial
     #]
 
 
-class IntegerDater(Dater):
+class IntegerDater(Dater, ):
     #[
     frequency = Frequency.INTEGER
     needs_resolve = False
     origin = 0
 
     @classmethod
     def from_sdmx_string(cls, sdmx_string: str) -> IntegerDater:
-        sdmx_string = sdmx_string.replace("(", "")
-        sdmx_string = sdmx_string.replace(")", "")
+        sdmx_string = sdmx_string.strip().removeprefix("(", "").removesuffix(")")
         return cls(int(sdmx_string))
 
+    def to_sdmx_string(self) -> str:
+        return f"({self.serial})"
+
     def to_plotly_date(self) -> str:
         return str(self.serial)
 
     def __repr__(self) -> str:
         return f"ii({self.serial})"
 
-    def __str__(self) -> str:
-        serial = self.serial
-        return self.frequency.sdmx_format.format(serial=serial)
-
     def to_plotly_date(self):
         return self.serial
     #]
 
 
 class DailyDater(Dater, IsoMixin):
     #[
@@ -288,35 +281,55 @@
     def from_year_period(cls, year: int, period: int) -> Self:
         boy_serial = _dt.date(year, 1, 1).toordinal()
         serial = boy_serial + int(period) - 1
         return cls(serial)
 
     @classmethod
     def from_sdmx_string(cls, sdmx_string: str) -> DailyDater:
-        year, month, day = sdmx_string.split("-")
+        year, month, day, *_ = sdmx_string.split("-")
         return cls.from_ymd(int(year), int(month), int(day))
 
-    def to_year_period(self: Self) -> tuple[int, int]:
+    def to_sdmx_string(self, /, **kwargs) -> str:
+        year, month, day = self.to_ymd()
+        return f"{year:04g}-{month:02g}-{day:02g}"
+
+    def to_year_period(self) -> tuple[int, int]:
         boy_serial = _dt.date(_dt.date.fromordinal(self.serial).year, 1, 1)
         per = self.serial - boy_serial + 1
         year = _dt.date.fromordinal(self.serial).year
         return year, per
 
-    def to_ymd(self: Self, /, **kwargs) -> tuple[int, int, int]:
+    def to_ymd(self, /, **kwargs) -> tuple[int, int, int]:
         py_date = _dt.date.fromordinal(self.serial)
         return py_date.year, py_date.month, py_date.day
 
-    def __str__(self) -> str:
-        year, month, day = self.to_ymd()
-        letter = self.frequency.letter
-        return self.frequency.sdmx_format.format(year=year, month=month, day=day, letter=letter)
+    def get_year(self, /, ) -> int:
+        return _dt.date.fromordinal(self.serial).year
 
-    @_remove_blanks_decorate
+    @_remove_blanks
     def __repr__(self) -> str:
         return f"dd{self.to_ymd()}"
+
+    def to_start_of_year(self, ) -> Self:
+        year = self.get_year()
+        serial = _dt.date(year, 1, 1).toordinal()
+        return type(self)(serial)
+
+    def to_end_of_year(self, ) -> Self:
+        year = self.get_year()
+        serial = _dt.date(year, 12, 31).toordinal()
+        return type(self)(serial)
+
+    def to_end_of_previous_year(self, ) -> Self:
+        year = self.get_year()
+        serial = _dt.date(year-1, 12, 31).toordinal()
+        return type(self)(serial)
+
+    def to_daily(self, /, **kwargs, ) -> Self:
+        return self
     #]
 
 
 def _serial_from_ypf(year: int, per: int, freq: int) -> int:
     return int(year)*int(freq) + int(per) - 1
 
 
@@ -324,16 +337,15 @@
     #[
     @classmethod
     def from_year_period(
             cls: type,
             year: int,
             per: int | str = 1,
         ) -> Self:
-        if per=="end":
-            per = cls.frequency.value
+        per = per if per != "end" else cls.frequency.value
         new_serial = _serial_from_ypf(year, per, cls.frequency.value)
         return cls(new_serial)
 
     @classmethod
     def from_ymd(cls, year: int, month: int=1, day: int=1, ) -> YearlyDater:
         return cls.from_year_period(year, cls.month_to_period(month, ), )
 
@@ -347,19 +359,37 @@
         self, 
         /,
         position: Literal["start"] | Literal["center"] | Literal["end"] = "center",
     ) -> tuple[int, int, int]:
         year, per = self.to_year_period()
         return year, *self.month_day_resolution[position][per]
 
-
     def __str__(self) -> str:
         year, per = self.to_year_period()
         letter = self.frequency.letter
         return self.frequency.sdmx_format.format(year=year, per=per, letter=letter)
+
+    def to_start_of_year(self, ) -> Self:
+        year, *_ = self.to_year_period()
+        return self.from_year_period(year, 1)
+
+    def to_end_of_year(self, ) -> Self:
+        year, *_ = self.to_year_period()
+        return self.from_year_period(year, self.frequency.value)
+
+    def to_end_of_previous_year(self, ) -> Self:
+        year, *_ = self.to_year_period()
+        return self.from_year_period(year-1, self.frequency.value)
+
+    def to_daily(
+        self,
+        /,
+        position: Literal["start"] | Literal["center"] | Literal["end"] = "center"
+    ) -> DailyDater:
+        return DailyDater.from_ymd(*self.to_ymd(position=position))
     #]
 
 
 class YearlyDater(Dater, RegularDaterMixin, ): 
     #[
     frequency: Frequency = Frequency.YEARLY
     needs_resolve: bool = False
@@ -370,15 +400,18 @@
         "end": {1: (12, 31)},
     }
 
     @classmethod
     def from_sdmx_string(cls, sdmx_string: str) -> YearlyDater:
         return cls(int(sdmx_string))
 
-    @_remove_blanks_decorate
+    def to_sdmx_string(self) -> str:
+        return f"{self.get_year():04g}"
+
+    @_remove_blanks
     def __repr__(self) -> str: return f"yy({self.get_year()})"
 
     @staticmethod
     def month_to_period(month: int, ) -> int:
         return 1
     #]
 
@@ -392,19 +425,22 @@
         "start": {1: (1, 1), 2: (7, 1)},
         "center": {1: (3, 15), 2: (9, 15)},
         "end": {1: (6, 30), 2: (12, 31)}
     }
 
     @classmethod
     def from_sdmx_string(cls, sdmx_string: str) -> HalfyearlyDater:
-        year, halfyear = sdmx_string.split("-")
-        halfyear = halfyear.upper().replace("H", "")
+        year, halfyear = sdmx_string.split("-H")
         return cls.from_year_period(int(year), int(halfyear))
 
-    @_remove_blanks_decorate
+    def to_sdmx_string(self) -> str:
+        year, per = self.to_year_period()
+        return f"{year:04g}-{self.frequency.letter}{per:1g}"
+
+    @_remove_blanks
     def __repr__(self) -> str: return f"hh{self.to_year_period()}"
 
     def to_ymd(
         self, 
         /,
         position: Literal["start"] | Literal["center"] | Literal["end"] = "center",
     ) -> tuple[int, int, int]:
@@ -431,24 +467,27 @@
 class QuarterlyDater(Dater, RegularDaterMixin, ):
     frequency: Frequency = Frequency.QUARTERLY
     needs_resolve: bool = False
     origin = _serial_from_ypf(BASE_YEAR, 1, Frequency.QUARTERLY)
     month_day_resolution = {
         "start": {1: (1, 1), 2: (4, 1), 3: (7, 1), 4: (10, 1)},
         "center": {1: (2, 15), 2: (5, 15), 3: (8, 15), 4: (11, 15)},
-        "end": {1: (3, 30), 2: (5, 31), 3: (8, 31), 4: (11, 30)},
+        "end": {1: (3, 30), 2: (6, 31), 3: (9, 31), 4: (12, 31)},
     }
 
     @classmethod
     def from_sdmx_string(cls, sdmx_string: str) -> QuarterlyDater:
-        year, quarter = sdmx_string.split("-")
-        quarter = quarter.upper().replace("Q", "")
+        year, quarter = sdmx_string.split("-Q")
         return cls.from_year_period(int(year), int(quarter))
 
-    @_remove_blanks_decorate
+    def to_sdmx_string(self) -> str:
+        year, per = self.to_year_period()
+        return f"{year:04g}-{self.frequency.letter}{per:1g}"
+
+    @_remove_blanks
     def __repr__(self) -> str: return f"qq{self.to_year_period()}"
 
     @staticmethod
     def month_to_period(month: int, ) -> int:
         return 1+((month-1)//3)
 
 
@@ -464,15 +503,19 @@
     }
 
     @classmethod
     def from_sdmx_string(cls, sdmx_string: str) -> MonthlyDater:
         year, month = sdmx_string.split("-")
         return cls.from_year_period(int(year), int(month))
 
-    @_remove_blanks_decorate
+    def to_sdmx_string(self) -> str:
+        year, per = self.to_year_period()
+        return f"{year:04g}-{per:02g}"
+
+    @_remove_blanks
     def __repr__(self) -> str: return f"mm{self.to_year_period()}"
 
     @staticmethod
     def month_to_period(month: int, ) -> int:
         return month
     #]
 
@@ -594,15 +637,15 @@
 
     def __enter__(self):
         return self
 
     def __exit__(self, *args):
         pass
 
-    def __eq__(self: Self, other: Self) -> bool:
+    def __eq__(self, other: Self) -> bool:
         return self._start_date==other._start_date and self._end_date==other._end_date and self._step==other._step
 
     def __bool__(self) -> bool:
         return not self.needs_resolve
     #]
 
 
@@ -655,34 +698,52 @@
     Convert non-dater to integer dater
     """
     if isinstance(input_date, Number):
         input_date = IntegerDater(int(input_date))
     return input_date
 
 
-_DATER_CLASS_FROM_FREQUENCY_RESOLUTION = {
+DATER_CLASS_FROM_FREQUENCY_RESOLUTION = {
     Frequency.INTEGER: IntegerDater,
     Frequency.YEARLY: YearlyDater,
     Frequency.HALFYEARLY: HalfyearlyDater,
     Frequency.QUARTERLY: QuarterlyDater,
     Frequency.MONTHLY: MonthlyDater,
     Frequency.DAILY: DailyDater,
 }
 
 
 def dater_from_sdmx_string(freq: Frequency, sdmx_string: str, ) -> Dater:
     """
     """
-    return _DATER_CLASS_FROM_FREQUENCY_RESOLUTION[freq].from_sdmx_string(sdmx_string)
+    return DATER_CLASS_FROM_FREQUENCY_RESOLUTION[freq].from_sdmx_string(sdmx_string)
+
+
+def daters_from_sdmx_strings(freq: Frequency, sdmx_strings: Iterable[str], ) -> Iterable[Dater]:
+    """
+    """
+    return (DATER_CLASS_FROM_FREQUENCY_RESOLUTION[freq].from_sdmx_string(x) for x in sdmx_strings)
 
 
 def dater_from_iso_string(freq: Frequency, iso_string: str, ) -> Dater:
     """
     """
-    return _DATER_CLASS_FROM_FREQUENCY_RESOLUTION[freq].from_iso_string(iso_string)
+    return DATER_CLASS_FROM_FREQUENCY_RESOLUTION[freq].from_iso_string(iso_string)
+
+
+def daters_from_iso_strings(freq: Frequency, iso_strings: Iterable[str], ) -> Iterable[Dater]:
+    """
+    """
+    return (DATER_CLASS_FROM_FREQUENCY_RESOLUTION[freq].from_iso_string(x) for x in iso_strings)
+
+
+def dater_from_ymd(freq: Frequency, *args, ) -> Dater:
+    """
+    """
+    return DATER_CLASS_FROM_FREQUENCY_RESOLUTION[freq].from_ymd(*args, )
 
 
 _FREQUENCY_FROM_STRING_RESOLUTION = {
     "I": Frequency.INTEGER,
     "Y": Frequency.YEARLY,
     "H": Frequency.HALFYEARLY,
     "Q": Frequency.QUARTERLY,
@@ -702,8 +763,7 @@
 def get_encompassing_range(*args: ResolutionContextProtocol, ) -> Ranger:
     start_dates = [x.start_date for x in args if hasattr(x, "start_date") and x.start_date]
     end_dates = [x.end_date for x in args if hasattr(x, "end_date") and x.end_date]
     start_date = min(start_dates) if start_dates else None
     end_date = max(end_dates) if end_dates else None
     return Ranger(start_date, end_date)
 
-
```

### Comparing `irispie-0.1.6/src/irispie/dataman/exports.py` & `irispie-0.2.0/src/irispie/dataman/exports.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,29 +7,28 @@
 from __future__ import annotations
 
 import csv as cs_
 import numpy as np_
 import dataclasses as dc_
 import itertools as it_
 
-from ..dataman import dates as da_
-from ..dataman import series as se_
+from . import dates as _da
 #]
 
 
 class NotImplementedYet(Exception):
     pass
 
 
 @dc_.dataclass
 class _ExportBlockDescriptor:
     """
     """
     #[
-    frequency: da_.Frequency | None = None
+    frequency: _da.Frequency | None = None
     names: Iterable[str] | None = None
     descriptors: Iterable[str] | None = None
     descriptor_row: bool | None = None
     num_series_columns: int | None = None
     dates: Iterable[Dater] | None = None
     data_array: np_.ndarray | None = None
     delimiter: str | None = None
@@ -62,25 +61,25 @@
     #[
     def _to_sheet(
         self,
         file_name: str,
         /,
         descriptor_row: bool = False,
         range: Iterable[Dater] | None = None,
-        frequency: da_.Frequency | None = None,
+        frequency: _da.Frequency | None = None,
         delimiter: str = ",",
         numeric_format: str = "g",
         nan_str: str = "",
         csv_writer_settings: dict = {},
     ) -> Iterable[str]:
         """
         """
         if not frequency:
             raise NotImplementedYet("frequency=None")
-        frequency = da_.Frequency(frequency)
+        frequency = _da.Frequency(frequency)
         range = range if range else self._get_range_by_frequency(frequency)
         range = [ t for t in range ]
         num_data_rows = len(range)
         #
         names = self._get_series_names_by_frequency(frequency)
         descriptors = [ getattr(self, n)._description for n in names ]
         #
```

### Comparing `irispie-0.1.6/src/irispie/dataman/filters.py` & `irispie-0.2.0/src/irispie/series/filters.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/dataman/imports.py` & `irispie-0.2.0/src/irispie/dataman/imports.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 
 
 #[
 from __future__ import annotations
 
 from typing import (Self, )
 from collections.abc import (Iterable, Callable, )
-import csv as cs_
-import numpy as np_
-import dataclasses as dc_
+import csv as _cs
+import numpy as _np
+import dataclasses as _dc
 
-from ..dataman import (dates as dd_, series as ds_, )
+from . import dates as _dd
+from ..series import facade as _sf
 #]
 
 
-@dc_.dataclass
+@_dc.dataclass
 class _ImportBlockDescriptor:
     """
     """
     #[
     row_index: Iterable[int] | None = None,
-    dates: Iterable[dd_.Dater] | None = None,
+    dates: Iterable[_dd.Dater] | None = None,
     column_start: int | None = None,
     num_columns: int | None = None,
     names: Iterable[str] | None = None,
     descriptions: Iterable[str] | None = None,
 
     def column_iterator(self, /, ):
         """
@@ -86,28 +87,28 @@
 
 
 def _read_csv_lines(file_name, num_header_lines, /, delimiter=",", **kwargs, ):
     """
     """
     #[
     with open(file_name, "r") as fid:
-        reader = cs_.reader(fid, **kwargs, )
+        reader = _cs.reader(fid, **kwargs, )
         all_lines = [ line for line in reader ]
     if all_lines:
         all_lines[0][0] = all_lines[0][0].replace("\ufeff", "", )
     return all_lines
     #]
 
 
 def _block_iterator(name_line, description_row, data_lines, start_date_only, /, ):
     """
     """
     #[
     _is_end = lambda cell: cell.startswith("__")
-    _is_start = lambda cell: cell.startswith("__") and dd_.frequency_from_string(cell) is not dd_.Frequency.UNKNOWN
+    _is_start = lambda cell: cell.startswith("__") and _dd.frequency_from_string(cell) is not _dd.Frequency.UNKNOWN
     name_line += ["__"]
     status = False
     blocks = []
     current_date_column = None
     current_start = None
     current_frequency = None
     num_columns = len(name_line)
@@ -119,55 +120,55 @@
             descriptions = description_row[current_start:column]
             row_index, dates = _extract_dates_from_data_lines(data_lines, current_frequency, current_date_column, start_date_only, )
             yield _ImportBlockDescriptor(row_index, dates, current_start, num_columns, names, descriptions)
         if not status and _is_start(cell):
             status = True
             current_date_column = column
             current_start = column + 1
-            current_frequency = dd_.frequency_from_string(cell)
+            current_frequency = _dd.frequency_from_string(cell)
     #]
 
 
 def _extract_dates_from_data_lines(
     data_lines,
     frequency,
     column,
     start_date_only,
     /,
-) -> tuple[tuple[int], tuple[dd_.Dater]]:
+) -> tuple[tuple[int], tuple[_dd.Dater]]:
     """
     """
     #[
-    start_date = dd_.dater_from_sdmx_string(frequency, data_lines[0][column])
+    start_date = _dd.dater_from_sdmx_string(frequency, data_lines[0][column])
     date_extractor = {
         True: lambda i, line: start_date + i,
-        False: lambda i, line: dd_.dater_from_sdmx_string(frequency, line[column]),
+        False: lambda i, line: _dd.dater_from_sdmx_string(frequency, line[column]),
     }[start_date_only]
     row_index_and_dates = [ 
         (i, date_extractor(i, line))
         for i, line in enumerate(data_lines)
         if start_date_only or line[column]
     ]
     return tuple(zip(*row_index_and_dates))
     #]
 
 
 def _read_array_for_block(file_name, block, num_header_lines, /, delimiter=",", **kwargs, ):
     #[
     skip_header = num_header_lines
     usecols = [ c for c in range(block.column_start, block.column_start+block.num_columns) ]
-    return np_.genfromtxt(file_name, skip_header=skip_header, usecols=usecols, delimiter=delimiter, ndmin=2, **kwargs)
+    return _np.genfromtxt(file_name, skip_header=skip_header, usecols=usecols, delimiter=delimiter, ndmin=2, **kwargs)
     #]
 
 
 def _add_series_for_block(self, block, array, /, ):
     """
     """
     #[
     array = array[block.row_index, :]
     for columns, name, description in block.column_iterator():
-        series = ds_.Series(num_columns=len(columns), description=description)
+        series = _sf.Series(num_columns=len(columns), description=description)
         series.set_data(block.dates, array[:, columns])
         setattr(self, name, series)
     #]
```

### Comparing `irispie-0.1.6/src/irispie/dataman/imports2.py` & `irispie-0.2.0/src/irispie/dataman/imports2.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,28 +3,30 @@
 """
 
 
 #[
 from typing import (TypeAlias, Protocol, Callable, )
 from collections.abc import (Iterator, Iterable, Generator, )
 
-import csv as cs_
-import numpy as np_
-import itertools as it_
-import functools as ft_
-
-from . import (dates as dd_, series as ds_, databanks as _da, )
+import csv as _cs
+import numpy as _np
+import itertools as _it
+import functools as _ft
+
+from ..series import facade as _sf
+from . import dates as _dd
+from . import databanks as _da
 #]
 
 
 _Header: TypeAlias = tuple[str, str]
 _DataVector: TypeAlias = tuple[str, ...]
 _HeaderIterator: TypeAlias = Iterator[_Header, ]
 _DataIterator: TypeAlias = Iterator[_DataVector, ]
-_DataArrayReader: TypeAlias = Callable[[Iterable[int], ], np_.ndarray]
+_DataArrayReader: TypeAlias = Callable[[Iterable[int], ], _np.ndarray]
 
 
 _GENFROMTXT_SETTINGS = dict(
     delimiter=",",
     ndmin=2,
 )
 
@@ -101,15 +103,15 @@
         header: _Header | None,
         date_str_vector: _DataVector | None,
         /,
         **kwargs,
     ) -> None:
         self._start_index = start_index
         self._headers = []
-        freq = dd_.frequency_from_string(header[0]) if header is not None else None
+        freq = _dd.frequency_from_string(header[0]) if header is not None else None
         self._dates = _create_dates_for_block(freq, date_str_vector, **kwargs, )
         self._data_array = None
 
     def add_header(
         self,
         header: _Header,
         /,
@@ -131,15 +133,15 @@
         self._load_data_array(data_array_reader, )
         return self._data_array
 
     def _load_data_array(
         self,
         data_array_reader: _DataArrayReader,
         /,
-    ) -> np_.ndarray:
+    ) -> _np.ndarray:
         """
         Load block data as a numpy array
         """
         self._data_array = data_array_reader(usecols=self.column_indices, )
 
     @property
     def num_columns(
@@ -205,29 +207,29 @@
         self._has_description_row = kwargs.get("has_description_row", False, )
 
     def create_header_and_data_iterators(
         self,
         /,
     ) -> tuple[Iterator[_Header], Iterator[_DataVector], ]:
         with open(self._file_path, newline="", ) as file:
-            csv_reader = cs_.reader(file, )
+            csv_reader = _cs.reader(file, )
             header_iterator = self._create_header_iterator(csv_reader, )
             data_iterator = self._create_data_iterator(csv_reader, )
         return header_iterator, data_iterator, 
 
     def create_data_array_reader(
         self,
         /,
-    ) -> Callable[[Iterable[int], ], np_.ndarray]:
+    ) -> Callable[[Iterable[int], ], _np.ndarray]:
         """
         Create a reader for the data array
         """
         skip_rows = self._skip_rows + 1 + int(self._has_description_row)
-        return ft_.partial(
-            np_.genfromtxt,
+        return _ft.partial(
+            _np.genfromtxt,
             self._file_path,
             skip_header=skip_rows,
             **_GENFROMTXT_SETTINGS,
         )
 
     def _create_header_iterator(
         self,
@@ -236,30 +238,30 @@
     ) -> Iterator[_Header]:
         """
         Create an iterator over headers (name, description, )
         """
         for _ in range(self._skip_rows):
             next(csv_reader, )
         name_row = next(csv_reader, )
-        description_row = next(csv_reader, ) if self._has_description_row else it_.repeat("", )
+        description_row = next(csv_reader, ) if self._has_description_row else _it.repeat("", )
         return zip(name_row, description_row, )
 
     def _create_data_iterator(
         self,
         csv_reader,
         /,
     ) -> Iterator[_DataVector]:
         """
         Create an iterator over individual data series or dates
         """
-        return it_.zip_longest(*csv_reader, fillvalue="", )
+        return _it.zip_longest(*csv_reader, fillvalue="", )
 
 
 def _create_dates_for_block(
-    freq: dd_.Frequency | None,
+    freq: _dd.Frequency | None,
     date_str_vector: _DataVector | None,
     /,
     start_date_only: bool = False,
     **kwargs,
 ) -> tuple[Dater]:
     """
     Create dates for a block
@@ -270,34 +272,34 @@
     else:
         dates_factory = _create_dates_from_date_column
     return dates_factory(freq, date_str_vector, )
     #]
 
 
 def _create_dates_from_start_date(
-    freq: dd_.Frequency | None,
+    freq: _dd.Frequency | None,
     date_str_vector: _DataVector | None,
 ) -> tuple[Dater]:
     """
     Create dates from a start date
     """
     #[
     num_dates = len(date_str_vector)
-    start_date = dd_.from_sdmx_string(freq, date_str_vector[0], )
-    return tuple(dd_.Ranger(start_date, num_dates, ))
+    start_date = _dd.from_sdmx_string(freq, date_str_vector[0], )
+    return tuple(_dd.Ranger(start_date, num_dates, ))
     #]
 
 
 def _create_dates_from_date_column(
-    freq: dd_.Frequency | None,
+    freq: _dd.Frequency | None,
     date_str_vector: _DataVector | None,
 ) -> tuple[Dater]:
     """
     Create dates from a date column
     """
     #[
     return tuple(
-        dd_.dater_from_sdmx_string(freq, s, ) if s else None
+        _dd.dater_from_sdmx_string(freq, s, ) if s else None
         for s in date_str_vector
     )
     #]
```

### Comparing `irispie-0.1.6/src/irispie/dataman/plotly.py` & `irispie-0.2.0/src/irispie/series/plotly.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #[
 from __future__ import annotations
 
 import plotly.graph_objects as _pg
 import plotly.subplots as _ps
 from types import (EllipsisType, )
 
-from ..dataman import (dates as _da, )
+from ..dataman import dates as _da
 #]
 
 
 builtin_range = range
 
 
 __all__ = [
```

### Comparing `irispie-0.1.6/src/irispie/dataman/series.py` & `irispie-0.2.0/src/irispie/series/facade.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
-Time series
+Time series facade
 """
 
 #[
 from __future__ import annotations
 
 from numbers import Number
 from collections.abc import (Iterable, Callable, )
 from typing import (Self, TypeAlias, )
 from types import (EllipsisType, )
 import numpy as np_
 import itertools as it_
 import copy as co_
 
-from ..dataman.dates import (Dater, Ranger, date_index, ResolvableProtocol, )
-from ..dataman import (views as vi_, )
-from ..dataman import (dates as _da, )
-from ..dataman import (filters as fi_, )
-from ..dataman import (plotly as pl_, )
-from ..mixins import (userdata as ud_, )
+from ..user import views as _vi
+from ..user import description as _ud
+from ..dataman import dates as _da
+from . import filters as _sg
+from . import plotly as _sp
+from . import conversion as _sc
 #]
 
 
 FUNCTION_ADAPTATIONS = ["log", "exp", "sqrt", "maximum", "minimum"] + ["cumsum"] + ["maxi", "mini", "mean", "median"]
 np_.maxi = np_.max
 np_.mini = np_.min
 
@@ -35,21 +35,21 @@
 for n in FUNCTION_ADAPTATIONS:
     exec(
         f"def {n}(x, *args, **kwargs): "
         f"return x._{n}_(*args, **kwargs) if hasattr(x, '_{n}_') else np_.{n}(x, *args, **kwargs)"
     )
 
 
-Dates: TypeAlias = Dater | Iterable[Dater] | Ranger | EllipsisType | None
+Dates: TypeAlias = _da.Dater | Iterable[_da.Dater] | _da.Ranger | EllipsisType | None
 Columns: TypeAlias = int | Iterable[int] | slice
 Data: TypeAlias = Number | Iterable[Number] | tuple | np_.ndarray
 
 
 def _get_date_positions(dates, base, num_periods):
-    pos = list(date_index(dates, base))
+    pos = list(_da.date_index(dates, base))
     min_pos = min(pos)
     max_pos = max(pos)
     add_before = max(-min_pos, 0)
     add_after = max(max_pos - num_periods, 0)
     pos_adjusted = [p + add_before for p in pos]
     return pos_adjusted, add_before, add_after
 
@@ -57,15 +57,21 @@
 def _trim_decorate(func):
     def wrapper(self, *args, **kwargs):
         func(self, *args, **kwargs)
         return self._trim()
     return wrapper
 
 
-class Series(fi_.HodrickPrescottMixin, pl_.PlotlyMixin, ud_.DescriptionMixin, vi_.SeriesViewMixin):
+class Series(
+    _sg.HodrickPrescottMixin,
+    _ud.DescriptionMixin,
+    _sc.ConversionMixin,
+    _vi.SeriesViewMixin,
+    _sp.PlotlyMixin,
+):
     """
     """
     __slots__ = (
         "start_date", "data", "data_type",
         "_description", "_column_titles", "_user_data",
     )
     _numeric_format: str = "15g"
@@ -101,56 +107,56 @@
 
     @property
     def num_columns(self):
         return self.data.shape[1]
 
     @property
     def range(self):
-        return Ranger(self.start_date, self.end_date) if self.start_date else []
+        return _da.Ranger(self.start_date, self.end_date) if self.start_date else []
 
     @property
     def end_date(self):
         return self.start_date + self.data.shape[0] - 1 if self.start_date else None
 
     @property
     def frequency(self):
         return self.start_date.frequency if self.start_date is not None else _da.Frequency.UNKNOWN
 
     @classmethod
     def from_dates_and_data(
         cls,
-        dates: Iterable[Dater],
+        dates: Iterable[_da.Dater],
         data: np_.ndarray,
         /,
     ) -> Self:
         num_columns = data.shape[1] if hasattr(data, "shape") else 1
         self = cls(num_columns=num_columns)
         self.set_data(dates, data)
         return self
 
     from_dates_and_values = from_dates_and_data
 
     @classmethod
     def from_start_date_and_data(
         cls,
-        start_date: Dater,
+        start_date: _da.Dater,
         data: np_.ndarray,
         /,
         **kwargs,
     ) -> Self:
         num_columns = data.shape[1] if hasattr(data, "shape") else 1
         self = cls(num_columns=num_columns, **kwargs)
         self.start_date = start_date
         self.data = data
-        return self
+        return self._trim()
 
     @classmethod
     def from_func(
         cls,
-        dates: Iterable[Dater],
+        dates: Iterable[_da.Dater],
         func: Callable,
         /,
         **kwargs,
     ) -> Self:
         """
         """
         self = cls(**kwargs)
@@ -246,26 +252,26 @@
             columns = (columns, )
         columns = [ c for c in columns ]
         self.data = self.data[:, columns]
         self.column_titles = [ self.column_titles[c] for c in columns ]
 
     def set_start_date(
         self,
-        new_start_date: Dater,
+        new_start_date: _da.Dater,
         /,
     ) -> Self:
         self.start_date = new_start_date
         return self
 
     def _resolve_dates(self, dates):
         if dates is None:
             return []
         if dates is Ellipsis:
-            dates = Ranger(None, None)
-        if isinstance(dates, ResolvableProtocol) and dates.needs_resolve:
+            dates = _da.Ranger(None, None)
+        if isinstance(dates, _da.ResolvableProtocol) and dates.needs_resolve:
             dates = dates.resolve(self)
         return dates
 
     def _resolve_columns(self, columns):
         if columns is None or columns is Ellipsis:
             columns = slice(None)
         if isinstance(columns, slice):
@@ -321,25 +327,25 @@
         new_data = np_.hstack((new_data, *add_data))
         new = Series(num_columns=new_data.shape[1]);
         new.set_data(encompassing_range, new_data)
         return new
 
     def clip(
         self,
-        new_start_date: Dater | None,
-        new_end_date: Dater | None,
+        new_start_date: _da.Dater | None,
+        new_end_date: _da.Dater | None,
     ) -> None:
         if new_start_date is None or new_start_date < self.start_date:
             new_start_date = self.start_date
         if new_end_date is None or new_end_date > self.end_date:
             new_end_date = self.end_date
         if new_start_date == self.start_date and new_end_date == self.end_date:
             return
         self.start_date = new_start_date
-        self.data = self.get_data(Ranger(new_start_date, new_end_date))
+        self.data = self.get_data(_da.Ranger(new_start_date, new_end_date))
 
     def overlay_by_range(
         self,
         other: Self,
         /,
     ) -> Self:
         self._trim()
@@ -592,15 +598,15 @@
 
 def hstack(first, *args) -> Self:
     return first.hstack(*args)
 
 
 def _create_data_from_number(
     number: Number,
-    range: Ranger,
+    range: _da.Ranger,
     data_type: type,
     /,
 ) -> np_.ndarray:
     return np_.full((len(range), 1), number, dtype=data_type)
 
 
 def shift(x, by):
```

### Comparing `irispie-0.1.6/src/irispie/dataman/views.py` & `irispie-0.2.0/src/irispie/user/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 
 #[
 from __future__ import annotations
 
 from numbers import (Number, )
 import numpy as np_
 import re as re_
-
-from ..dataman import dates as da_
 #]
 
 
 _VERTICAL_ELLIPSIS = "⋮"
 _REPEAT_SHORT_ROW = 2
 _REPR_MAX_LEN = 70
 _REPR_CONT = "..."
@@ -36,26 +34,28 @@
 
 
 def _databank_repr(x, /, ) -> str:
     """
     String representing one record in a databank
     """
     #[
-    if x is None:
+    if hasattr(x, "_databank_repr"):
+        s = x._databank_repr()
+    elif x is None:
         s = "None"
     elif x is ...:
         s = "..."
-    elif isinstance(x, Number) or isinstance(x, da_.Dater):
+    elif isinstance(x, Number):
         s = str(x)
     elif isinstance(x, str):
         s = f'"{x}"'
     elif isinstance(x, np_.ndarray) or isinstance(x, list) or isinstance(x, tuple):
         s = re_.sub("\n + ", " ", repr(x))
-    elif hasattr(x, "_get_first_line_view_"):
-        s = x._get_first_line_view_()
+    elif hasattr(x, "_get_first_line_view"):
+        s = x._get_first_line_view()
     else:
         s = repr(type(x))
     return s if len(s)<_REPR_MAX_LEN else s[0:_REPR_MAX_LEN] + _REPR_CONT
     #]
 
 
 class ViewMixin:
@@ -64,15 +64,15 @@
     _short_rows_: int = 5
     #[
     def _get_header_view_(self, /, ):
         """
         """
         return [ 
             "", 
-            self._get_first_line_view_(),
+            self._get_first_line_view(),
             f"Description: \"{self.get_description()}\"",
             "", 
         ]
 
     def _get_footer_view_(self, /, ):
         return ["", ]
 
@@ -106,15 +106,15 @@
     #]
 
 
 class SeriesViewMixin(ViewMixin):
     """
     """
     #[
-    def _get_first_line_view_(self, /, ):
+    def _get_first_line_view(self, /, ):
         """
         """
         shape = self.data.shape
         return f"Series {self.frequency.letter} {self.start_date}:{self.end_date} {shape[0]}-by-{shape[1]}"
 
     def _get_content_view_(self, /, ):
         """
@@ -136,15 +136,15 @@
     #]
 
 
 class DatabankViewMixin(ViewMixin):
     """
     """
     #[
-    def _get_first_line_view_(self, /, ):
+    def _get_first_line_view(self, /, ):
         """
         """
         return f"Databank with {self._get_num_records():g} record(s)"
 
     def _get_content_view_(self, /, ):
         """
         """
```

### Comparing `irispie-0.1.6/src/irispie/equators/abc.py` & `irispie-0.2.0/src/irispie/equators/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/equators/plain.py` & `irispie-0.2.0/src/irispie/equators/plain.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/equators/steady.py` & `irispie-0.2.0/src/irispie/equators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/evaluators/printers.py` & `irispie-0.2.0/src/irispie/evaluators/printers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/evaluators/steady.py` & `irispie-0.2.0/src/irispie/evaluators/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/fords/descriptors.py` & `irispie-0.2.0/src/irispie/fords/descriptors.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/fords/simulators.py` & `irispie-0.2.0/src/irispie/fords/simulators.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/fords/solutions.py` & `irispie-0.2.0/src/irispie/fords/solutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/fords/steadiers.py` & `irispie-0.2.0/src/irispie/fords/steadiers.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/fords/systems.py` & `irispie-0.2.0/src/irispie/fords/systems.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/jacobians/abc.py` & `irispie-0.2.0/src/irispie/jacobians/abc.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/jacobians/steady.py` & `irispie-0.2.0/src/irispie/jacobians/steady.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/models/facade.py` & `irispie-0.2.0/src/irispie/models/facade.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/models/flags.py` & `irispie-0.2.0/src/irispie/models/flags.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/models/gettables.py` & `irispie-0.2.0/src/irispie/models/gettables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/models/invariants.py` & `irispie-0.2.0/src/irispie/models/invariants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/models/simulatables.py` & `irispie-0.2.0/src/irispie/models/simulatables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/models/sources.py` & `irispie-0.2.0/src/irispie/models/sources.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/models/steadiables.py` & `irispie-0.2.0/src/irispie/models/steadiables.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/models/variants.py` & `irispie-0.2.0/src/irispie/models/variants.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/parsers/common.py` & `irispie-0.2.0/src/irispie/parsers/common.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/parsers/model_source_parser.py` & `irispie-0.2.0/src/irispie/parsers/model_source_parser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/parsers/preparser.py` & `irispie-0.2.0/src/irispie/parsers/preparser.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/parsers/pseudofunctions.py` & `irispie-0.2.0/src/irispie/parsers/pseudofunctions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/src/irispie/parsers/substitutions.py` & `irispie-0.2.0/src/irispie/parsers/substitutions.py`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/LICENCE` & `irispie-0.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `irispie-0.1.6/pyproject.toml` & `irispie-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["hatchling"]
     build-backend = "hatchling.build"
 
 [project]
     name = "irispie"
-    version = "0.1.6"
+    version = "0.2.0"
     authors = [
       { name="Jaromir Benes", email="jaromir.benes@gmail.com" },
     ]
     description = "Macroeconomic modeling package"
     readme = "README.md"
     requires-python = ">=3.11"
     classifiers = [
```

### Comparing `irispie-0.1.6/PKG-INFO` & `irispie-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irispie
-Version: 0.1.6
+Version: 0.2.0
 Summary: Macroeconomic modeling package
 Project-URL: Homepage, https://github.com/iris-solutions-team/irispie
 Project-URL: Bug Tracker, https://github.com/iris-solutions-team/irispie/issues
 Author-email: Jaromir Benes <jaromir.benes@gmail.com>
 License-File: LICENCE
 Keywords: dsge,economics,forecasting,macroeconomics,modeling,simulation
 Classifier: License :: OSI Approved :: MIT License
```

