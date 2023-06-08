# Comparing `tmp/DomiKnowS-0.534.dev0.tar.gz` & `tmp/DomiKnowS-0.535.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DomiKnowS-0.534.dev0.tar", last modified: Wed Jun  7 01:14:54 2023, max compression
+gzip compressed data, was "DomiKnowS-0.535.dev0.tar", last modified: Thu Jun  8 14:50:55 2023, max compression
```

## Comparing `DomiKnowS-0.534.dev0.tar` & `DomiKnowS-0.535.dev0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.428527 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-07 01:14:54.000000 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-07 01:14:54.000000 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 01:14:54.000000 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 01:14:54.000000 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 01:14:54.000000 DomiKnowS-0.534.dev0/DomiKnowS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.428527 DomiKnowS-0.534.dev0/domiknows/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.432528 DomiKnowS-0.534.dev0/domiknows/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/compiler/OntologyMLGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.432528 DomiKnowS-0.534.dev0/domiknows/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.432528 DomiKnowS-0.534.dev0/domiknows/data/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/data/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/data/allennlp/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.432528 DomiKnowS-0.534.dev0/domiknows/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.432528 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/allennlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)   108201 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/dataNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/dataNodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    28639 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/logicalConstrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/graph/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.436528 DomiKnowS-0.534.dev0/domiknows/program/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/batchprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/callbackprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/lossprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.436528 DomiKnowS-0.534.dev0/domiknows/program/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/gbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/ilpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/iml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/lossModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/model_program.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/program/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.436528 DomiKnowS-0.534.dev0/domiknows/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.440528 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.440528 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/learnerModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/query_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/relation_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.440528 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.440528 DomiKnowS-0.534.dev0/domiknows/sensor/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/torch/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/sensor/torch/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/domiknows/solver/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/allennlpInferenceSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/allennlplogInferenceSolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/domiknows/solver/constructor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/constructor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/constructor/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/dummyILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/gekkoILPBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/gekkoILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    38785 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/gurobiILPBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)   103195 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/gurobiILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/ilpBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/ilpConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/ilpOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/ilpOntSolverFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/lcLossBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/lcLossSampleBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/mini_solver_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/domiknows/solver/session/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/session/gurobi_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/session/solver_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/domiknows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 01:14:54.444528 DomiKnowS-0.534.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-07 01:14:44.000000 DomiKnowS-0.534.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.529276 DomiKnowS-0.535.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.521276 DomiKnowS-0.535.dev0/DomiKnowS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-08 14:50:55.000000 DomiKnowS-0.535.dev0/DomiKnowS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-08 14:50:55.000000 DomiKnowS-0.535.dev0/DomiKnowS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:50:55.000000 DomiKnowS-0.535.dev0/DomiKnowS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 14:50:55.000000 DomiKnowS-0.535.dev0/DomiKnowS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 14:50:55.000000 DomiKnowS-0.535.dev0/DomiKnowS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-08 14:50:55.529276 DomiKnowS-0.535.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.521276 DomiKnowS-0.535.dev0/domiknows/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.521276 DomiKnowS-0.535.dev0/domiknows/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/compiler/OntologyMLGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.521276 DomiKnowS-0.535.dev0/domiknows/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.521276 DomiKnowS-0.535.dev0/domiknows/data/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/data/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/data/allennlp/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.525276 DomiKnowS-0.535.dev0/domiknows/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.525276 DomiKnowS-0.535.dev0/domiknows/graph/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/allennlp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/allennlp/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/allennlp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/allennlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110759 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/dataNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/dataNodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28639 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/logicalConstrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/graph/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.525276 DomiKnowS-0.535.dev0/domiknows/program/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/batchprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/callbackprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/lossprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.525276 DomiKnowS-0.535.dev0/domiknows/program/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/model/gbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/model/ilpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/model/iml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/model/lossModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/model/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/model/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/model_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/program/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.525276 DomiKnowS-0.535.dev0/domiknows/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.525276 DomiKnowS-0.535.dev0/domiknows/sensor/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/allennlp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/allennlp/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/allennlp/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/allennlp/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.529276 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/learnerModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/query_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/relation_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.529276 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.529276 DomiKnowS-0.535.dev0/domiknows/sensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/torch/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/sensor/torch/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.529276 DomiKnowS-0.535.dev0/domiknows/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/allennlpInferenceSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/allennlplogInferenceSolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.529276 DomiKnowS-0.535.dev0/domiknows/solver/constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/constructor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/constructor/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/dummyILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/gekkoILPBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/gekkoILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38785 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/gurobiILPBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103195 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/gurobiILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/ilpBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/ilpConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/ilpOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/ilpOntSolverFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/lcLossBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/lcLossSampleBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/mini_solver_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:55.529276 DomiKnowS-0.535.dev0/domiknows/solver/session/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/session/gurobi_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/session/solver_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/domiknows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:50:55.529276 DomiKnowS-0.535.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-08 14:50:42.000000 DomiKnowS-0.535.dev0/setup.py
```

### Comparing `DomiKnowS-0.534.dev0/DomiKnowS.egg-info/PKG-INFO` & `DomiKnowS-0.535.dev0/DomiKnowS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomiKnowS
-Version: 0.534.dev0
+Version: 0.535.dev0
 Summary: A library provides integration between Domain Knowledge and Deep Learning.
 Home-page: https://github.com/HLR/DomiKnowS
 Author: Andrzej Uszok
 Author-email: auszok@ihmc.org
 License: MIT
 Description: The library allows to specify a problem domain with a conceptual [graph](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#graph) including declarations of edges and nodes, as well as [logical constraints](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#constraints) on the graph concepts and relations. [Neural network](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/MODEL.md#model-declaration) outputs bounded to the graph edges and nodes. The logical constraints are converted to ILP and Gurobi Solver is used for inferring. This adds a relational overlay over elements in a network that relates physical concepts in applications. <br> <br> The example running in Google CoLab environment, presenting the usage of the library is [here](https://colab.research.google.com/drive/1FvdePHv3h3NDSTkBw1VKwAmaZFWuGgTi).
 Platform: UNKNOWN
```

### Comparing `DomiKnowS-0.534.dev0/DomiKnowS.egg-info/SOURCES.txt` & `DomiKnowS-0.535.dev0/DomiKnowS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/PKG-INFO` & `DomiKnowS-0.535.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomiKnowS
-Version: 0.534.dev0
+Version: 0.535.dev0
 Summary: A library provides integration between Domain Knowledge and Deep Learning.
 Home-page: https://github.com/HLR/DomiKnowS
 Author: Andrzej Uszok
 Author-email: auszok@ihmc.org
 License: MIT
 Description: The library allows to specify a problem domain with a conceptual [graph](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#graph) including declarations of edges and nodes, as well as [logical constraints](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#constraints) on the graph concepts and relations. [Neural network](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/MODEL.md#model-declaration) outputs bounded to the graph edges and nodes. The logical constraints are converted to ILP and Gurobi Solver is used for inferring. This adds a relational overlay over elements in a network that relates physical concepts in applications. <br> <br> The example running in Google CoLab environment, presenting the usage of the library is [here](https://colab.research.google.com/drive/1FvdePHv3h3NDSTkBw1VKwAmaZFWuGgTi).
 Platform: UNKNOWN
```

### Comparing `DomiKnowS-0.534.dev0/README.md` & `DomiKnowS-0.535.dev0/README.md`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/base.py` & `DomiKnowS-0.535.dev0/domiknows/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/compiler/OntologyMLGraph.py` & `DomiKnowS-0.535.dev0/domiknows/compiler/OntologyMLGraph.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/data/allennlp/reader.py` & `DomiKnowS-0.535.dev0/domiknows/data/allennlp/reader.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/data/reader.py` & `DomiKnowS-0.535.dev0/domiknows/data/reader.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/__init__.py` & `DomiKnowS-0.535.dev0/domiknows/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/allennlp/base.py` & `DomiKnowS-0.535.dev0/domiknows/graph/allennlp/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/allennlp/metrics.py` & `DomiKnowS-0.535.dev0/domiknows/graph/allennlp/metrics.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/allennlp/model.py` & `DomiKnowS-0.535.dev0/domiknows/graph/allennlp/model.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/allennlp/utils.py` & `DomiKnowS-0.535.dev0/domiknows/graph/allennlp/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/base.py` & `DomiKnowS-0.535.dev0/domiknows/graph/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/candidates.py` & `DomiKnowS-0.535.dev0/domiknows/graph/candidates.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/concept.py` & `DomiKnowS-0.535.dev0/domiknows/graph/concept.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/dataNode.py` & `DomiKnowS-0.535.dev0/domiknows/graph/dataNode.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 from collections import OrderedDict, namedtuple
-from time import process_time_ns
+from time import process_time, process_time_ns
 import re
 
 from .dataNodeConfig import dnConfig 
 
 from ordered_set import OrderedSet 
 
 from domiknows import getRegrTimer_logger, getProductionModeStatus
@@ -87,14 +87,16 @@
         
         if attributes:
             self.attributes = attributes                 # Dictionary with node's attributes
         else:
             self.attributes = {}
             
         self.current_device = 'auto'
+        
+        self.myLoggerTime = getRegrTimer_logger()
                      
     class DataNodeError(Exception):
         pass
     
     def __str__(self):
         if self.instanceValue:
             return self.instanceValue
@@ -1021,27 +1023,30 @@
             
             if not dns:
                 continue
             
             vs = []
             
             for dn in dns:
-                if "softmax" in keys or "normalizedProb" in keys:
+                keySoftmax = "<" + c[0].name + ">/local/softmax"
+                normalized_keys = set(["normalizedProb", "meanNormalizedProb", "normalizedProbAll"])
+                if "softmax" in keys or normalized_keys.intersection(set(keys)):
                     keySoftmax = "<" + c[0].name + ">/local/softmax"
                     if not keySoftmax in dn.attributes: # Already calculated ?                    
                         v = dn.getAttribute(c[0])
                         
                         # check if v is None or not a tensor
                         if v is None or not torch.is_tensor(v):
                             continue
                         
                         if not(isinstance(v, torch.FloatTensor) or isinstance(v, torch.cuda.FloatTensor)):
                             v = v.float()
                             
                         vSoftmaxT = torch.nn.functional.softmax(v, dim=-1)
+                        # vSoftmaxT = v
                         
                         # Replace nan with 1/len
                         #for i, s in enumerate(vSoftmaxT):
                         #   if s != s:
                         #       vSoftmaxT[i] = 1/len(v)
                         
                         dn.attributes[keySoftmax] = vSoftmaxT
@@ -1050,23 +1055,59 @@
                 
                 if "normalizedProb" in keys:
                     keyNormalizedProb = "<" + c[0].name + ">/local/normalizedProb"
                     if not keyNormalizedProb in dn.attributes: # Already calculated ?   
                         vSoftmaxT = dn.attributes[keySoftmax]
                         
                         # Clamps the softmax probabilities
-                        vector = torch.clamp(vSoftmaxT, min=1e-12, max=1 - 1e-12) 
+                        vector = torch.clamp(vSoftmaxT, min=1e-18, max=1 - 1e-18) 
                         
                         # Calculates their entropy;
                         entropy = torch.distributions.Categorical(torch.log(vector)).entropy() / vector.shape[0]
                         
                         # Multiplies the reverse of entropy to the vector divided by its mean value. P
                         vNormalizedProbT = (1/entropy.item()) * (vector/torch.mean(vector))
                         
                         dn.attributes[keyNormalizedProb] = vNormalizedProbT
+
+                if "meanNormalizedProb" in keys:
+                    keyNormalizedProb = "<" + c[0].name + ">/local/meanNormalizedProb"
+                    if not keyNormalizedProb in dn.attributes: # Already calculated ?   
+                        vSoftmaxT = dn.attributes[keySoftmax]
+
+                        vector = vSoftmaxT
+                        
+                        # Multiplies the reverse of entropy to the vector divided by its mean value. P
+                        vNormalizedProbT = vector/torch.mean(vector)
+                        
+                        dn.attributes[keyNormalizedProb] = vNormalizedProbT
+
+                if "normalizedProbAll" in keys:
+                    keyNormalizedProb = "<" + c[0].name + ">/local/normalizedProbAll"
+                    if not keyNormalizedProb in dn.attributes: # Already calculated ?   
+                        vSoftmaxT = dn.attributes[keySoftmax]
+
+                        # Clamps the softmax probabilities
+                        vector = torch.clamp(vSoftmaxT, min=1e-12, max=1 - 1e-12) 
+                        
+                        # Calculates their entropy;
+                        entropy = torch.distributions.Categorical(torch.log(vector)).entropy() / vector.shape[0]
+                        
+                        
+                        dn.attributes[keyNormalizedProb] = vNormalizedProbT
+
+                        signs = vector - torch.mean(vector)
+                        signs[signs < 0] = -1
+                        signs[signs >= 0] = +1
+                        adjustment = signs * torch.pow(vector - torch.mean(vector), 4)
+                        
+                        # Multiplies the reverse of entropy to the vector divided by its mean value. P
+                        vNormalizedProbT = (1/entropy.item()) * (vector/torch.mean(vector)) + adjustment
+                        
+                        dn.attributes[keyNormalizedProb] = vNormalizedProbT
                 
                 if "argmax" in keys:
                     keyArgmax  = "<" + c[0].name + ">/local/argmax"
                     v = dn.getAttribute(c[0])
                     vArgmax = torch.clone(v)
                     vArgmaxIndex = torch.argmax(v).item()
                     
@@ -1097,17 +1138,22 @@
                 
         myilpOntSolver, conceptsRelations = self.__getILPSolver(_conceptsRelations)
         
         # Call ilpOntsolver with the collected probabilities for chosen candidates
         _DataNode__Logger.info("Calling ILP solver")
         
         if "local" in key:
+            startInferLocal = process_time() # timer()
+
             keys = (key[1],)
             self.inferLocal(keys=keys)
-            
+            endInferLocal = process_time() # timer()
+            elapsedInferLocalInMs = (endInferLocal - startInferLocal) * 1000
+            self.myLoggerTime.info('Infer Local Probabilities - keys: %s, time: %dms', keys, elapsedInferLocalInMs)     
+                   
         myilpOntSolver.calculateILPSelection(self, *conceptsRelations, key=key, fun=fun, epsilon = epsilon, minimizeObjective = minimizeObjective, ignorePinLCs = ignorePinLCs)    
         
     def inferGBIResults(self, *_conceptsRelations, model, builder):
         if len(_conceptsRelations) == 0:
             _DataNode__Logger.info('Called with empty list of concepts and relations for inference')
         else:
             _DataNode__Logger.info('Called with - %s - list of concepts and relations for inference'%([x.name if isinstance(x, Concept) else x for x in _conceptsRelations]))
```

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/graph.py` & `DomiKnowS-0.535.dev0/domiknows/graph/graph.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/logicalConstrain.py` & `DomiKnowS-0.535.dev0/domiknows/graph/logicalConstrain.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/property.py` & `DomiKnowS-0.535.dev0/domiknows/graph/property.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/relation.py` & `DomiKnowS-0.535.dev0/domiknows/graph/relation.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/graph/trial.py` & `DomiKnowS-0.535.dev0/domiknows/graph/trial.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/batchprogram.py` & `DomiKnowS-0.535.dev0/domiknows/program/batchprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/callbackprogram.py` & `DomiKnowS-0.535.dev0/domiknows/program/callbackprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/loss.py` & `DomiKnowS-0.535.dev0/domiknows/program/loss.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/lossprogram.py` & `DomiKnowS-0.535.dev0/domiknows/program/lossprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/metric.py` & `DomiKnowS-0.535.dev0/domiknows/program/metric.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/model/gbi.py` & `DomiKnowS-0.535.dev0/domiknows/program/model/gbi.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/model/ilpu.py` & `DomiKnowS-0.535.dev0/domiknows/program/model/ilpu.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/model/iml.py` & `DomiKnowS-0.535.dev0/domiknows/program/model/iml.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/model/lossModel.py` & `DomiKnowS-0.535.dev0/domiknows/program/model/lossModel.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/model/pytorch.py` & `DomiKnowS-0.535.dev0/domiknows/program/model/pytorch.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/model/torch.py` & `DomiKnowS-0.535.dev0/domiknows/program/model/torch.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/model_program.py` & `DomiKnowS-0.535.dev0/domiknows/program/model_program.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/program.py` & `DomiKnowS-0.535.dev0/domiknows/program/program.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/program/tracker.py` & `DomiKnowS-0.535.dev0/domiknows/program/tracker.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/base.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/allennlp/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/learner.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/allennlp/learner.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/module.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/allennlp/module.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/allennlp/sensor.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/allennlp/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/learnerModels.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/learnerModels.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/learners.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/learners.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/query_sensor.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/query_sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/relation_sensors.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/relation_sensors.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/sensors.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/sensors.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/pytorch/utils.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/sensor.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/torch/learner.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/torch/learner.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/sensor/torch/sensor.py` & `DomiKnowS-0.535.dev0/domiknows/sensor/torch/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/allennlpInferenceSolver.py` & `DomiKnowS-0.535.dev0/domiknows/solver/allennlpInferenceSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/allennlplogInferenceSolver.py` & `DomiKnowS-0.535.dev0/domiknows/solver/allennlplogInferenceSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/constructor/constructor.py` & `DomiKnowS-0.535.dev0/domiknows/solver/constructor/constructor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/dummyILPOntSolver.py` & `DomiKnowS-0.535.dev0/domiknows/solver/dummyILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/gekkoILPBooleanMethods.py` & `DomiKnowS-0.535.dev0/domiknows/solver/gekkoILPBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/gekkoILPOntSolver.py` & `DomiKnowS-0.535.dev0/domiknows/solver/gekkoILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/gurobiILPBooleanMethods.py` & `DomiKnowS-0.535.dev0/domiknows/solver/gurobiILPBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/gurobiILPOntSolver.py` & `DomiKnowS-0.535.dev0/domiknows/solver/gurobiILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/ilpBooleanMethods.py` & `DomiKnowS-0.535.dev0/domiknows/solver/ilpBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py` & `DomiKnowS-0.535.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/ilpOntSolver.py` & `DomiKnowS-0.535.dev0/domiknows/solver/ilpOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/ilpOntSolverFactory.py` & `DomiKnowS-0.535.dev0/domiknows/solver/ilpOntSolverFactory.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/lcLossBooleanMethods.py` & `DomiKnowS-0.535.dev0/domiknows/solver/lcLossBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/lcLossSampleBooleanMethods.py` & `DomiKnowS-0.535.dev0/domiknows/solver/lcLossSampleBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/mini_solver_debug.py` & `DomiKnowS-0.535.dev0/domiknows/solver/mini_solver_debug.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/session/gurobi_session.py` & `DomiKnowS-0.535.dev0/domiknows/solver/session/gurobi_session.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/solver/session/solver_session.py` & `DomiKnowS-0.535.dev0/domiknows/solver/session/solver_session.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/domiknows/utils.py` & `DomiKnowS-0.535.dev0/domiknows/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.534.dev0/setup.py` & `DomiKnowS-0.535.dev0/setup.py`

 * *Files identical despite different names*

