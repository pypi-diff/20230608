# Comparing `tmp/hiperwalk-2.0a3.tar.gz` & `tmp/hiperwalk-2.0a4.tar.gz`

## Comparing `hiperwalk-2.0a3.tar` & `hiperwalk-2.0a4.tar`

### file list

```diff
@@ -1,95 +1,110 @@
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/.readthedocs.yaml
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/build_and_upload_to_pypi
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/config.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/custom.nbl
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/custom.py
--rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/distance.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/dtqw1d.nbl
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/dtqw1d.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/dtqw2d.nbl
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/dtqw2d.py
--rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/gnuplot.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/hiperwalk.py
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/install.sh
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/ioFunctions.py
--rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/neblina.py
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/operators.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/parsing.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/run.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/staggered1d.nbl
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/staggered1d.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/staggered2d.nbl
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/staggered2d.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/standardDeviation.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/state.py
--rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/testmode.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/walks.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/coined1D.in
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/coined2D.in
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/custom.in
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/psi0.dat
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/staggered1D.in
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/staggered2D.in
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/u0.dat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/Archive/examples/u1.dat
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/README.md
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/conf.py
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/go
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/make.bat
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/requirements.txt
--rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/test_docs
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/_static/switcher.json
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/_templates/autoclass.rst
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/_templates/autofunctions.rst
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/_templates/automodule.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/development/index.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/documentation/graph.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/documentation/index.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/documentation/plot.rst
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/documentation/quantum_walk.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/graphviz/coined-cycle-edges-labels.dot
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/graphviz/coined-model-edges-labels.dot
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/graphviz/coined-model-sample.dot
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/graphviz/coined-segment-edges-labels.dot
--rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/install/index.rst
--rw-r--r--   0        0        0     3690 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/tutorial/index.rst
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/docs/tutorial/plotting_customization.rst
--rw-r--r--   0        0        0   245035 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/examples/Untitled.ipynb
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/examples/Untitled1.ipynb
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/examples/coined-diagonal-lattice.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/examples/continuous-cycle.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/examples/refactor.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/__init__.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/_constants.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/graph/__init__.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/graph/cycle.py
--rw-r--r--   0        0        0     5764 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/graph/graph.py
--rw-r--r--   0        0        0    14531 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/graph/lattice.py
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/graph/line.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/plot/__init__.py
--rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/plot/_animation.py
--rw-r--r--   0        0        0    26318 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/plot/_plot.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/quantum_walk/__init__.py
--rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/quantum_walk/_pyneblina_interface.py
--rw-r--r--   0        0        0    33527 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/quantum_walk/coined_walk.py
--rw-r--r--   0        0        0    10565 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/quantum_walk/continuous_walk.py
--rw-r--r--   0        0        0    16075 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/hiperwalk/quantum_walk/quantum_walk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/__init__.py
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/run_all.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/run_hpc.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/run_nonhpc.sh
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/test_constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/coined_cycle.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/coined_line.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/coined_segment.py
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/continuous_graph.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/tests/unitary/lattice_uniform_state.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/.gitignore
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/LICENSE
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/README.md
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/pyproject.toml
--rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 hiperwalk-2.0a3/PKG-INFO
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/.readthedocs.yaml
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/build_and_upload_to_pypi
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/config.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/custom.nbl
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/custom.py
+-rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/distance.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/dtqw1d.nbl
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/dtqw1d.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/dtqw2d.nbl
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/dtqw2d.py
+-rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/gnuplot.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/hiperwalk.py
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/install.sh
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/ioFunctions.py
+-rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/neblina.py
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/operators.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/parsing.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/run.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/staggered1d.nbl
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/staggered1d.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/staggered2d.nbl
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/staggered2d.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/standardDeviation.py
+-rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/state.py
+-rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/testmode.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/walks.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/examples/coined1D.in
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/examples/coined2D.in
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/examples/custom.in
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/examples/psi0.dat
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/examples/staggered1D.in
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/examples/staggered2D.in
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/examples/u0.dat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/Archive/examples/u1.dat
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/README.md
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/conf.py
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/go
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/make.bat
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/requirements.txt
+-rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/test_docs
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/_static/switcher.json
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/_templates/autoclass.rst
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/_templates/autofunctions.rst
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/_templates/automodule.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/development/index.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/documentation/graph.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/documentation/index.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/documentation/plot.rst
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/documentation/quantum_walk.rst
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/cycle-arcs.dot
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/graph-arcs.dot
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/graph-example.dot
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/line-arcs.dot
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/bounded-diagonal.dot
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/bounded-diagonal.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/bounded-natural.dot
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/bounded-natural.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/diagonal-directions.dot
+-rw-r--r--   0        0        0     9307 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/even-dim-diagonal.dot
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/even-dim-diagonal.py
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/go
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/natural-directions.dot
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/periodic-diagonal.dot
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/periodic-diagonal.py
+-rw-r--r--   0        0        0     4252 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/periodic-natural.dot
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/graphviz/lattice/periodic-natural.py
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/install/index.rst
+-rw-r--r--   0        0        0     3363 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/tutorial/graphs.rst
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/tutorial/index.rst
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/tutorial/plotting_customization.rst
+-rw-r--r--   0        0        0    14334 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/docs/tutorial/quantum_walk_models.rst
+-rw-r--r--   0        0        0   245035 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/examples/Untitled.ipynb
+-rw-r--r--   0        0        0   765034 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/examples/Untitled1.ipynb
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/examples/coined-diagonal-lattice.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/examples/continuous-cycle.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/examples/refactor.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/__init__.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/_constants.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/graph/__init__.py
+-rw-r--r--   0        0        0     3409 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/graph/cycle.py
+-rw-r--r--   0        0        0     8362 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/graph/graph.py
+-rw-r--r--   0        0        0    19415 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/graph/lattice.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/graph/line.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/plot/__init__.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/plot/_animation.py
+-rw-r--r--   0        0        0    26318 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/plot/_plot.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/quantum_walk/__init__.py
+-rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/quantum_walk/_pyneblina_interface.py
+-rw-r--r--   0        0        0    30157 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/quantum_walk/coined_walk.py
+-rw-r--r--   0        0        0     9566 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/quantum_walk/continuous_walk.py
+-rw-r--r--   0        0        0    16555 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/hiperwalk/quantum_walk/quantum_walk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/__init__.py
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/run_all.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/run_hpc.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/run_nonhpc.sh
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/test_constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/unitary/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/unitary/coined_cycle.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/unitary/coined_line.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/unitary/coined_segment.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/unitary/continuous_graph.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/tests/unitary/lattice_uniform_state.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/.gitignore
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/LICENSE
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/pyproject.toml
+-rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 hiperwalk-2.0a4/PKG-INFO
```

### Comparing `hiperwalk-2.0a3/Archive/config.py` & `hiperwalk-2.0a4/Archive/config.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/custom.nbl` & `hiperwalk-2.0a4/Archive/custom.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/custom.py` & `hiperwalk-2.0a4/Archive/custom.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/distance.py` & `hiperwalk-2.0a4/Archive/distance.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/dtqw1d.nbl` & `hiperwalk-2.0a4/Archive/dtqw1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/dtqw1d.py` & `hiperwalk-2.0a4/Archive/dtqw1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/dtqw2d.nbl` & `hiperwalk-2.0a4/Archive/dtqw2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/dtqw2d.py` & `hiperwalk-2.0a4/Archive/dtqw2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/gnuplot.py` & `hiperwalk-2.0a4/Archive/gnuplot.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/hiperwalk.py` & `hiperwalk-2.0a4/Archive/hiperwalk.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/install.sh` & `hiperwalk-2.0a4/Archive/install.sh`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/ioFunctions.py` & `hiperwalk-2.0a4/Archive/ioFunctions.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/neblina.py` & `hiperwalk-2.0a4/Archive/neblina.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/operators.py` & `hiperwalk-2.0a4/Archive/operators.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/parsing.py` & `hiperwalk-2.0a4/Archive/parsing.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/run.py` & `hiperwalk-2.0a4/Archive/run.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/staggered1d.nbl` & `hiperwalk-2.0a4/Archive/staggered1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/staggered1d.py` & `hiperwalk-2.0a4/Archive/staggered1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/staggered2d.nbl` & `hiperwalk-2.0a4/Archive/staggered2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/staggered2d.py` & `hiperwalk-2.0a4/Archive/staggered2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/standardDeviation.py` & `hiperwalk-2.0a4/Archive/standardDeviation.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/state.py` & `hiperwalk-2.0a4/Archive/state.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/testmode.py` & `hiperwalk-2.0a4/Archive/testmode.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/Archive/walks.py` & `hiperwalk-2.0a4/Archive/walks.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/docs/Makefile` & `hiperwalk-2.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/docs/conf.py` & `hiperwalk-2.0a4/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'Hiperwalk'
 copyright = '2023'
 author = 'Gustavo Bezerra'
 
 # The full version, including alpha/beta/rc tags
-release = '2.0a3'
+release = '2.0a4'
 version = 'stable'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `hiperwalk-2.0a3/docs/index.rst` & `hiperwalk-2.0a4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/docs/make.bat` & `hiperwalk-2.0a4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/docs/_templates/automodule.rst` & `hiperwalk-2.0a4/docs/_templates/automodule.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/docs/development/index.rst` & `hiperwalk-2.0a4/docs/development/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _docs_development:
+
 ===========
 Development
 ===========
 
 HiperWalk is built on top of some Python libraries.
 Before developing for HiperWalk,
 we must install these libraries.
```

### Comparing `hiperwalk-2.0a3/docs/graphviz/coined-model-edges-labels.dot` & `hiperwalk-2.0a4/docs/graphviz/graph-arcs.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/docs/install/index.rst` & `hiperwalk-2.0a4/docs/install/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/docs/tutorial/index.rst` & `hiperwalk-2.0a4/docs/tutorial/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -16,107 +16,115 @@
 We just illustrate the steps.
 
 .. testsetup::
 
    from sys import path as sys_path
    sys_path.append("../..")
 
-#. Import Hiperwalk.
+Import Hiperwalk
+----------------
 
-   >>> import hiperwalk as hpw
+>>> import hiperwalk as hpw
 
-#. Create the graph.
+Create the graph
+----------------
 
-   Here we create a line with 11 vertices.
-   The result is an object of the :class:`hiperwalk.Line` class.
+Here we create a line with 11 vertices.
+The result is an object of the :class:`hiperwalk.Line` class.
 
-   >>> N = 11
-   >>> line = hpw.Line(N)
-   >>> line #doctest: +SKIP
-   <hiperwalk.graph.line.Line object at 0x7ff59f1900d0>
+>>> N = 11
+>>> line = hpw.Line(N)
+>>> line #doctest: +SKIP
+<hiperwalk.graph.line.Line object at 0x7ff59f1900d0>
 
-#. Create the quantum walk based on the previous graph.
+Create the quantum walk based on the previous graph
+---------------------------------------------------
 
-   We create a coined quantum walk on the line with
-   11 vertices by passing the created graph as an
-   argument to the quantum walk constructor.
-   This results in an object of the :class:`hiperwalk.CoinedWalk` class.
+We create a coined quantum walk on the line with
+11 vertices by passing the created graph as an
+argument to the quantum walk constructor.
+This results in an object of the :class:`hiperwalk.CoinedWalk` class.
 
-   >>> qw = hpw.CoinedWalk(line)
-   >>> qw #doctest: +SKIP
-   <hiperwalk.quantum_walk.coined_walk.CoinedWalk object at 0x7f2691de9840>
+>>> qw = hpw.CoinedWalk(line)
+>>> qw #doctest: +SKIP
+<hiperwalk.quantum_walk.coined_walk.CoinedWalk object at 0x7f2691de9840>
 
-#. Simulate the walk.
+Simulate the walk
+-----------------
 
-   Before simulating the walk,
-   To simulate the walk we need to specify the initial condition.
-   One way to create the initial condition is by using the
-   :meth:`hiperwalk.CoinedWalk.ket` method,
-   which creates a valid state of the computational basis.
+Before simulating the walk,
+To simulate the walk we need to specify the initial state.
+One way to create the initial state is by using the
+:meth:`hiperwalk.CoinedWalk.ket` method,
+which creates a valid state of the computational basis.
 
-   >>> vertex = N // 2
-   >>> initial_condition = qw.ket(vertex, vertex + 1)
-   >>> initial_condition
-   array([0., 0., 0., 0., 0., 0., 0., 0., 0., 0., 1., 0., 0., 0., 0., 0., 0.,
-          0., 0., 0.])
+>>> vertex = N // 2
+>>> initial_state = qw.ket(vertex, vertex + 1)
+>>> initial_state
+array([0., 0., 0., 0., 0., 0., 0., 0., 0., 1., 0., 0., 0., 0., 0., 0., 0.,
+       0., 0., 0.])
 
-   This state corresponds to the walker being on
-   vertex 5 pointing to vertex 6
-   (the labels of the vertices go from 0 to 10).
+This state corresponds to the walker being on
+vertex 5 pointing to vertex 6
+(the labels of the vertices go from 0 to 10).
 
-   To simulate the walk we must specify the number of steps
-   (number of applications of the evolution operator)
-   and the initial condition.
-   By specifying only the final time,
-   the result is the final state.
-   If everything was installed properly,
-   the :meth:`hiperwalk.CoinedWalk.simulate` method automatically uses
-   high-performance computing to perform the matrix-vector multiplications.
+To simulate the walk we must specify the number of steps
+(number of applications of the evolution operator)
+and the initial state.
+By specifying only the final time,
+the result is the final state.
+If everything was installed properly,
+the :meth:`hiperwalk.CoinedWalk.simulate` method automatically uses
+high-performance computing to perform the matrix-vector multiplications.
 
-   >>> final_state = qw.simulate(time=N//2,
-   ...                           initial_condition=initial_condition)
+>>> final_state = qw.simulate(time=N//2,
+...                           initial_state=initial_state)
 
 
 
-#. Exhibit the results.
+Exhibit the results
+-------------------
 
-   The results exhibition may be a simple print
+The results exhibition may be a simple print
 
-   >>> final_state
-   array([[ 0.1767767 ,  0.        ,  0.        ,  0.35355339,  0.1767767 ,
-            0.        ,  0.        , -0.35355339,  0.        ,  0.        ,
-            0.        ,  0.35355339,  0.        ,  0.        ,  0.        ,
-            0.1767767 , -0.70710678,  0.        ,  0.        , -0.1767767 ]])
+>>> final_state
+array([[ 0.1767767 ,  0.        ,  0.        , -0.1767767 ,  0.35355339,
+         0.        ,  0.        ,  0.        , -0.35355339,  0.        ,
+         0.        ,  0.        ,  0.35355339,  0.        ,  0.        ,
+         0.70710678,  0.1767767 ,  0.        ,  0.        ,  0.1767767 ]])
+         
 
-   or a more sofisticated output.
-   Frequently, we are interested in the probability of the walker being
-   found on each vertex.
-   This can be done via the
-   :meth:`hiperwalk.CoinedWalk.probability_distribution` method
-   by passing the final state as argument.
+or a more sofisticated output.
+Frequently, we are interested in the probability of the walker being
+found on each vertex.
+This can be done via the
+:meth:`hiperwalk.CoinedWalk.probability_distribution` method
+by passing the final state as argument.
 
-   >>> probability = qw.probability_distribution(final_state)
-   >>> probability
-   array([[0.03125, 0.     , 0.15625, 0.     , 0.125  , 0.     , 0.125  ,
-           0.     , 0.53125, 0.     , 0.03125]])
+>>> probability = qw.probability_distribution(final_state)
+>>> probability
+array([[0.03125, 0.     , 0.15625, 0.     , 0.125  , 0.     , 0.125  ,
+        0.     , 0.53125, 0.     , 0.03125]])
 
-   It is also possible to plot the probability distribution
-   with a simple command.
+It is also possible to plot the probability distribution
+with a simple command.
 
-   >>> hpw.plot_probability_distribution(probability) #doctest: +SKIP
+>>> hpw.plot_probability_distribution(probability) #doctest: +SKIP
 
-   Resulting in the following plot.
+Resulting in the following plot.
 
-   .. figure:: probability_distribution.png
-       :alt: Plot of the probability distribution.
+.. figure:: probability_distribution.png
+    :alt: Plot of the probability distribution.
 
-       Probability distribution of a quantum walk on a line.
+    Probability distribution of a quantum walk on a line.
 
 Next Steps
 ----------
 
 The remainder of the tutorial is subdivided into the following sections.
 
 .. toctree::
     :maxdepth: 1
 
+    graphs.rst
+    quantum_walk_models.rst
     plotting_customization.rst
```

### Comparing `hiperwalk-2.0a3/examples/Untitled.ipynb` & `hiperwalk-2.0a4/examples/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/examples/coined-diagonal-lattice.py` & `hiperwalk-2.0a4/examples/coined-diagonal-lattice.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,10 +4,10 @@
 lat = hpw.Lattice(dim, diagonal=True)
 center = lat.get_central_vertex()
 dtqw = hpw.CoinedWalk(lat, shift='persistent', coin='grover')
 psi0 = dtqw.state([0.5, (center, center + (1, 1))],
                   [-0.5, (center, center + (1, -1))],
                   [-0.5, (center, center + (-1, 1))],
                   [0.5, (center, center + (-1, -1))])
-psi_final = dtqw.simulate(time=dim // 2, initial_condition=psi0, hpc=False)
+psi_final = dtqw.simulate(time=dim // 2, initial_state=psi0, hpc=False)
 prob = dtqw.probability_distribution(psi_final)
 hpw.plot_probability_distribution(prob, graph=lat)
```

### Comparing `hiperwalk-2.0a3/hiperwalk/_constants.py` & `hiperwalk-2.0a4/hiperwalk/_constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.0a3'
+__version__ = '2.0a4'
 
 #Declares data types according to neblina-core
 #TODO: make it so it is not hardcoded
 NEBLINA_FLOAT = 2
 NEBLINA_COMPLEX = 13 
 
 from sys import modules as sys_modules
```

### Comparing `hiperwalk-2.0a3/hiperwalk/graph/cycle.py` & `hiperwalk-2.0a4/hiperwalk/graph/cycle.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,22 @@
     num_vert : int
         Number of vertices in the cycle.
 
     Notes
     -----
     The cycle may be interpreted as being embedded on the line
     with cyclic boundary condition.
+    Then, we assign 0 the right direction and 1 with the left direction.
+    This changes the arc order.
+    Any arc with tail :math:`v`
+    has label :math:`2v` if pointing rightwards,
+    and label :math:`2v + 1` if pointing leftwards.
+    Figure 1 illustrates the arc labels of a 3 vertices cycle.
 
-
-    .. todo::
-        
-        update below
-
-    The edge order respects the default vertex-coin notation.
-    In other words, 0 corresponds to the coin pointing rightwards,
-    and 1 to the coin pointing leftwards.
-    Therefore, the arcs are sorted with respect to this order
-    (vertex has precedence over direction and
-    right has precedence over left):
-
-    .. math::
-        \begin{align*}
-            \ket{(v, c)} = \ket{2v + c}
-        \end{align*}
-
-    where :math:`v \in V` and :math:`c \in \{0, 1\}`.
-    Figure 1 illustrates the arcs of a 3 vertices cycle.
-
-    .. graphviz:: ../../graphviz/coined-cycle-edges-labels.dot
+    .. graphviz:: ../../graphviz/cycle-arcs.dot
         :align: center
         :layout: neato
         :caption: Figure 1.
 
     """
 
     def __init__(self, num_vert):
```

### Comparing `hiperwalk-2.0a3/hiperwalk/graph/line.py` & `hiperwalk-2.0a4/hiperwalk/graph/line.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,33 +10,47 @@
     Parameters
     ----------
     num_vert : int
         Number of vertices on the line.
 
     Notes
     -----
-    .. todo::
+    On the Line,
+    we can assign directions to the arcs.
+    If an arc is pointing rightwards it has direction 0 --
+    i.e., (1, 2).
+    If an arc is pointing leftwards, it has direction 1 --
+    i.e., (2, 1).
+
+    We use the arc directions to define the arcs order.
+    Hence, for a vertex :math:`v \in V`,
+    the arcs :math:`(v, v + 1)` and :math:`(v, v - 1)`
+    have labels :math:`a_0` and :math:`a_1` (respectively)
+    such that  :math:`a_0 < a_1`.
+    This order is coherent with the Coined Quantum Walk on the line [1]_.
+    The only exceptions to this rule are the extreme vertices
+    0 and :math:`|V| - 1`.
+    Since they only have one arc.
+    Besides that,
+    for any two vertices :math:`v_1 < v_2`,
+    any arc with tail :math:`v_1` has label smaller than
+    any arc with tail :math:`v_2`.
 
-        update
-
-
-    Since :class:`Segment` is built on top of :class:`Graph`,
-    operators and states respect the edge order
-    (See :class:`Graph` notes for more details).
-    As a consequence, for any vertex :math:`v \in V`,
-    the state :math:`\ket{2v - d}` for :math:`d \in \{0, 1\}`
-    corresponds to the walker being on vertex :math:`v` and the
-    coin pointing rightwars (:math:`d = 0`) or leftwards (:math:`d = 1`).
-    For example, the edges labels of the 4-vertices :class:`Segment`
+    For example, the arc labels of the 4-vertices Line
     are represented in Figure 1.
     
-    .. graphviz:: ../../graphviz/coined-segment-edges-labels.dot
+    .. graphviz:: ../../graphviz/line-arcs.dot
         :align: center
         :layout: neato
         :caption: Figure 1.
+
+    References
+    ----------
+    .. [1] Portugal, Renato. "Quantum walks and search algorithms".
+        Vol. 19. New York: Springer, 2013.
     """
 
     def __init__(self, num_vert):
         # Creating adjacency matrix
         # The end vertices are only adjacent to 1 vertex.
         # Every other vertex is adjacent to two vertices.
         data = np.ones(2*(num_vert-1), dtype=np.int8)
@@ -64,19 +78,26 @@
         return 'hadamard'
 
     def arc_label(self, tail, head):
         diff = head - tail
         if diff != 1 and diff != -1:
             raise ValueError('Invalid arc.')
 
-        return tail*2 if diff == 1 else tail*2 - 1 
+        num_vert = self.number_of_vertices()
+        return (2*tail - 1 if (diff == 1 and tail != 0
+                               or head == num_vert - 1)
+                else tail*2)
 
     def arc(self, label):
-        tail = (label + 1)//2
-        head = tail + (-1)**(label % 2)
+        label += 1
+        tail = label//2
+        num_vert = self.number_of_vertices()
+        head = (tail + (-1)**(label % 2)
+                if tail != 0 and tail != num_vert - 1
+                else tail - (-1)**(label % 2))
         return (tail, head)
 
     def next_arc(self, arc):
         # implemented only if is embeddable
         try:
             tail, head = arc
             diff = head - tail
@@ -85,20 +106,20 @@
 
             if head == 0 or head == self.number_of_vertices() - 1:
                 return (head, tail)
             
             return ((tail + 1, head + 1) if diff == 1
                     else (tail - 1, head - 1))
         except TypeError:
-            if arc == 1:
-                return 0
+            if arc == 0:
+                return 1
             num_arcs = self.number_of_arcs() 
-            if arc == num_arcs - 2:
-                return num_arcs - 1
-            return arc + 2 if arc % 2 == 0 else arc - 2
+            if arc == num_arcs - 1:
+                return num_arcs - 2
+            return arc + 2 if arc % 2 == 1 else arc - 2
 
     def previous_arc(self, arc):
         # implemented only if is embeddable
         try:
             tail, head = arc
             diff = head - tail
             if diff != 1 and diff != -1:
@@ -106,13 +127,18 @@
 
             if tail == 0 or tail == self.number_of_vertices() - 1:
                 return (head, tail)
             
             return ((tail - 1, head - 1) if diff == 1
                     else (tail + 1, head + 1))
         except TypeError:
-            if arc == 0:
-                return 1
-            num_arcs = self.number_of_arcs() 
-            if arc == num_arcs - 1:
-                return num_arcs - 2
-            return arc - 2 if arc % 2 == 0 else arc + 2
+            num_arcs = self.number_of_arcs()
+            if arc < 0 or arc >= num_arcs:
+                raise ValueError('Invalid arc')
+
+            arc = arc + 2 if arc % 2 == 0 else arc - 2
+            if arc < 0:
+                arc += 1
+            elif arc >= num_arcs:
+                arc -= 1
+
+            return arc
```

### Comparing `hiperwalk-2.0a3/hiperwalk/plot/_animation.py` & `hiperwalk-2.0a4/hiperwalk/plot/_animation.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/hiperwalk/plot/_plot.py` & `hiperwalk-2.0a4/hiperwalk/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/hiperwalk/quantum_walk/_pyneblina_interface.py` & `hiperwalk-2.0a4/hiperwalk/quantum_walk/_pyneblina_interface.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/hiperwalk/quantum_walk/coined_walk.py` & `hiperwalk-2.0a4/hiperwalk/quantum_walk/coined_walk.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     ----------
     graph
         Graph on which the quantum walk occurs.
         It can be the graph itself (:class:`hiperwalk.graph.Graph`) or
         its adjacency matrix (:class:`scipy.sparse.csr_array`).
 
     adjacency : :class:`scipy.sparse.csr_array`, optional
-        .. deprecated:: 2.0
-            It will be removed in version 2.1.
+        .. deprecated:: 2.0a1
+            It will be removed in version 2.0.
             Use ``graph`` instead.
 
         Use ``graph`` instead.
         Adjacency matrix of the graph.
 
     **kwargs : optional
         Optional arguments for setting the non-default evolution operator.
@@ -54,121 +54,24 @@
 
     See Also
     --------
     set_evolution
 
     Notes
     -----
-    The recommended parameter type is
-    :class:`scipy.sparse.csr_array` using ``dtype=np.int8``
-    with 1 denoting adjacency and 0 denoting non-adjacency.
-    If any entry is different from 0 or 1,
-    some methods may not work as expected.
 
-    For more information about the general general Coined Quantum Walk Model,
+    The Hilbert space of the general Coined Quantum Walk model is
+    :math:`\mathcal{H}^{2|E|}`.
+    The computational basis is given by the graph arcs.
+    Refer to each graph for more information about the arcs order.
+
+    For more information about the general Coined Quantum Walk Model,
     check Quantum Walks and Search Algorithms's
     Section 7.2: Coined Walks on Arbitrary Graphs [1]_.
 
-    The Graph class uses the arc notation
-    and the Hilbert space :math:`\mathcal{H}^{2|E|}` for general Graphs.
-    That is, for a given graph :math:`G(V, E)`,
-    the walk occurs in the graph :math:`\vec{G}(V, A)`
-    where
-
-    .. math::
-        \begin{align*}
-            A = \bigcup_{(v,u) \in E} \{(v, u), (u, v)\}.
-        \end{align*}
-
-    Matrices and states respect the sorted arcs order,
-    i.e. :math:`(v, u) < (v', u')` if either :math:`v < v'` or
-    :math:`v = v'` and :math:`u < u'`
-    where :math:`(v, u), (v', u')` are valid arcs.
-
-    For example, the graph :math:`G(V, E)` shown in
-    Figure 1 has adjacency matrix ``adj_matrix``.
-
-    .. testsetup::
-
-        import numpy as np
-
-    >>> adj_matrix = np.array([
-    ...     [0, 1, 0, 0],
-    ...     [1, 0, 1, 1],
-    ...     [0, 1, 0, 1],
-    ...     [0, 1, 1, 0]])
-    >>> adj_matrix
-    array([[0, 1, 0, 0],
-           [1, 0, 1, 1],
-           [0, 1, 0, 1],
-           [0, 1, 1, 0]])
-
-    .. graphviz:: ../../graphviz/coined-model-sample.dot
-        :align: center
-        :layout: neato
-        :caption: Figure 1
-
-    The corresponding arcs are
-
-    >>> arcs = [(i, j) for i in range(4)
-    ...                for j in range(4) if adj_matrix[i,j] == 1]
-    >>> arcs
-    [(0, 1), (1, 0), (1, 2), (1, 3), (2, 1), (2, 3), (3, 1), (3, 2)]
-
-    Note that ``arcs`` is already sorted, hence the labels are
-
-    >>> arcs_labels = {arcs[i]: i for i in range(len(arcs))}
-    >>> arcs_labels
-    {(0, 1): 0, (1, 0): 1, (1, 2): 2, (1, 3): 3, (2, 1): 4, (2, 3): 5, (3, 1): 6, (3, 2): 7}
-
-    The arcs labels are illustrated in Figure 2.
-
-    .. graphviz:: ../../graphviz/coined-model-edges-labels.dot
-        :align: center
-        :layout: neato
-        :caption: Figure 2
-
-    If we would write the arcs labels respecting the the adjacency matrix format,
-    we would have the matrix ``adj_labels``.
-    Intuitively, the arcs are labeled in left-to-right top-to-bottom fashion.
-
-    >>> adj_labels = [[arcs_labels[(i,j)] if (i,j) in arcs_labels
-    ...                                   else '' for j in range(4)]
-    ...               for i in range(4)]
-    >>> adj_labels = np.matrix(adj_labels)
-    >>> adj_labels
-    matrix([['', '0', '', ''],
-            ['1', '', '2', '3'],
-            ['', '4', '', '5'],
-            ['', '6', '7', '']], dtype='<U21')
-
-    For consistency, any state :math:`\ket\psi \in \mathcal{H}^{2|E|}`
-    is such that :math:`\ket\psi = \sum_{i = 0}^{2|E| - 1} \psi_i \ket{i}`
-    where :math:`\ket{i}` is the computational basis state
-    associated to the :math:`i`-th arc.
-    In our example, the state
-
-    >>> psi = np.array([1/np.sqrt(2), 0, 1j/np.sqrt(2), 0, 0, 0, 0, 0])
-    >>> psi
-    array([0.70710678+0.j        , 0.        +0.j        ,
-           0.        +0.70710678j, 0.        +0.j        ,
-           0.        +0.j        , 0.        +0.j        ,
-           0.        +0.j        , 0.        +0.j        ])
-
-    corresponds to the walker being at vertex 0
-    and the coin pointing to vertex 1 with
-    associated amplitude of :math:`\frac{1}{\sqrt 2}`, and
-    to the walker being at vertex 1
-    and the coin pointing to vertex 2 with
-    associated amplitude of :math:`\frac{\text{i}}{\sqrt 2}`.
-
-    .. todo::
-        * Add option: numpy dense matrix as parameters.
-        * Add option: networkx graph as parameter.
-
     References
     ----------
     .. [1] Portugal, Renato. "Quantum walks and search algorithms".
         Vol. 19. New York: Springer, 2013.
     """
 
     # static attributes.
```

### Comparing `hiperwalk-2.0a3/hiperwalk/quantum_walk/continuous_walk.py` & `hiperwalk-2.0a4/hiperwalk/quantum_walk/continuous_walk.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         :class:`hiperwalk.graph.Graph` :
             The graph itself.
 
         :class:`class:scipy.sparse.csr_array`:
             The graph adjacency matrix.
 
     adjacency : :class:`scipy.sparse.csr_array`, optional
-        .. deprecated:: 2.0
-            It will be removed in version 2.1.
+        .. deprecated:: 2.0a1
+            It will be removed in version 2.0.
             Use ``graph`` instead.
 
         Adjacency matrix of the graph on which the quantum occurs
         is going to occur.
 
     **kwargs : optional
         Arguments for setting Hamiltonian.
@@ -91,16 +91,21 @@
         gamma : float, default = 1
             Gamma value.
         """
         if gamma is None or gamma.imag != 0:
             raise TypeError("Value of 'gamma' is not float.")
 
         self._gamma = gamma
+        self._hamiltonian = None
         self._evolution = None
 
+    def set_marked(self, marked=[]):
+        super().set_marked(marked)
+        self._hamiltonian = None
+
     def get_gamma(self):
         r"""
         Get the gamma used for the Hamiltonian.
 
         Returns
         -------
         float
@@ -115,18 +120,14 @@
         Parameters
         ----------
         **kwargs : 
             Additional arguments.
             Used for determining the gamma value and marked vertices.
             See :meth:`set_gamma` and :meth:`set_marked`.
 
-        Returns
-        -------
-        :class:`scipy.sparse.csr_array`
-            
         Notes
         -----
         The Hamiltonian is given by
 
         .. math::
             H = -\gamma A  - \sum_{m \in M} \ket m \bra m
 
@@ -151,41 +152,43 @@
                               ContinuousWalk._hamiltonian_kwargs['gamma'])
         marked_kwargs = ContinuousWalk._filter_valid_kwargs(
                               kwargs,
                               ContinuousWalk._hamiltonian_kwargs['marked'])
 
         self.set_gamma(**gamma_kwargs)
         self.set_marked(**marked_kwargs)
+
+    def get_hamiltonian(self):
+        r"""
+        Returns Hamiltonian.
+
+        Returns
+        -------
+        :class:`scipy.sparse.csr_array`
+        """
+        if self._hamiltonian is not None:
+            return self._hamiltonian
+
         H = -self._gamma * self._graph.adj_matrix
 
         # creating oracle
         if len(self._marked) > 0:
             data = np.ones(len(self._marked), dtype=np.int8)
             oracle = scipy.sparse.csr_array(
                     (data, (self._marked, self._marked)),
                     shape=(self.hilb_dim, self.hilb_dim))
 
-            H -= self._oracle
+            H -= oracle
 
         self._hamiltonian = H
         # since the hamiltonian was changed,
         # the previous evolution operator may not be coherent.
         self._evolution_operator = None
         return H
 
-    def get_hamiltonian(self):
-        r"""
-        Returns Hamiltonian.
-
-        Returns
-        -------
-        :class:`scipy.sparse.csr_array`
-        """
-        return self._hamiltonian
-
     def set_evolution(self, **kwargs):
         r"""
         Alias for :meth:`set_hamiltonian`.
         """
         self.set_hamiltonian(**kwargs)
 
     def get_evolution(self, time=None, hpc=True):
@@ -207,15 +210,15 @@
         Returns
         -------
         :class:`numpy.ndarray`.
 
         Raises
         ------
         ValueError
-            If `time < 0`.
+            If ``time < 0``.
 
         See Also
         --------
         set_hamiltonian
 
         Notes
         -----
@@ -237,26 +240,25 @@
             mitigate uounding errors.
         """
         if time is None or time < 0:
             raise ValueError(
                 "Expected non-negative `time` value."
             )
 
-        if self._hamiltonian is None:
-            raise AssertionError
+        H = self.get_hamiltonian()
 
         if hpc and not self._pyneblina_imported():
             hpc = False
 
         if hpc:
             # determining the number of terms in power series
-            max_val = np.max(np.abs(self._hamiltonian))
+            max_val = np.max(np.abs(H))
             if max_val*time <= 1:
                 nbl_U = nbl.matrix_power_series(
-                        -1j*time*self._hamiltonian, 30)
+                        -1j*time*H, 30)
 
             else:
                 # if the order of magnitude is very large,
                 # float point errors may occur
                 if ((isinstance(time, int) or time.is_integer())
                     and max_val <= 1
                 ):
@@ -265,98 +267,68 @@
                 else:
                     new_time = max_val*time
                     order = np.ceil(np.math.log(new_time, 20))
                     new_time /= 10**order
                     num_mult = int(np.round(time/new_time)) - 1
 
                 new_nbl_U = nbl.matrix_power_series(
-                        -1j*new_time*self._hamiltonian, 20)
+                        -1j*new_time*H, 20)
                 nbl_U = nbl.multiply_matrices(new_nbl_U, new_nbl_U)
                 for i in range(num_mult - 1):
                     nbl_U = nbl.multiply_matrices(nbl_U, new_nbl_U)
 
             U = nbl.retrieve_matrix(nbl_U)
 
         else:
-            U = scipy.linalg.expm(-1j*time*self._hamiltonian.todense())
+            U = scipy.linalg.expm(-1j*time*H.todense())
 
         self._evolution = U
         return U
 
-    def simulate(self, time=None, initial_condition=None, hpc=True):
+    def simulate(self, time=None, initial_state=None,
+                 initial_condition=None, hpc=True):
         r"""
-        Simulate the Continuous Time Quantum Walk Hamiltonian.
-
-        Analogous to the :meth:`QuantumWalk.simulate`
-        but uses the Hamiltonian to construct the evolution operator.
-        The Hamiltonian may be the previously set or
-        passed in the arguments.
+        Analogous to :meth:`QuantumWalk.simulate`
+        accepting float entries for ``time``.
 
         Parameters
         ----------
         time : float or tuple of floats
             Analogous to the parameters of :meth:`QuantumWalk.simulate`,
             but accepts float inputs.
             ``step`` is used to construct the evolution operator.
             The states in the interval
             ***[* ``start/step``, ``end/step`` **]** are saved.
             The values that describe this interval are
             rounded up if the decimal part is greater than ``1 - 1e-5``,
             and rounded down otherwise.
 
-        hamiltonian : :class:`numpy.ndarray` or None
-            Hamiltonian matrix to be used for constructing
-            the evolution operator.
-            If ``None``, uses the previously set Hamiltonian
-
         Other Parameters
         ----------------
-        initial_condition :
-            See :meth:`QuantumWalk.simulate`.
-        hpc :
-            See :meth:`QuantumWalk.simulate`.
-
-
-        Raises
-        ------
-        ValueError
-            If ``time_range=None`` or ``initial_condition=None``,
-            or ``hamiltonian`` has invalid Hilbert space dimension.
-
-
-        Notes
-        -----
-        It is recommended to call this method with ``hamiltonian=None``
-        to guarantee that a valid Hamiltonian was used.
-        If the Hamiltonian is passed by the user,
-        there is no guarantee that the Hamiltonian is local.
+        See :meth:`QuantumWalk.simulate`.
 
         See Also
         --------
-        :meth:`QuantumWalk.simulate`
-        hamiltonian
+        set_evolution
+        get_evolution
         """
         if time is None:
             raise ValueError(
                 "Invalid `time_range`. Expected a float, 2-tuple, "
                 + "or 3-tuple of float."
             )
 
-        if initial_condition is None:
-            raise ValueError(
-                "`initial_condition` not specified."
-            )
-
         time = np.array(self._time_to_tuple(time))
 
         self.get_evolution(time=time[2], hpc=hpc)
 
         # cleaning time_range to int
         tol = 1e-5
         time = [int(val/time[2])
                 if int(val/time[2])
                    <= np.ceil(val/time[2]) - tol
                 else int(np.ceil(val/time[2]))
                 for val in time]
 
-        states = super().simulate(time, initial_condition,  hpc)
+        states = super().simulate(time, initial_state,
+                                  initial_condition, hpc)
         return states
```

### Comparing `hiperwalk-2.0a3/hiperwalk/quantum_walk/quantum_walk.py` & `hiperwalk-2.0a4/hiperwalk/quantum_walk/quantum_walk.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,26 +22,20 @@
     ----------
     graph
         Graph on which the quantum walk occurs.
         It can be the graph itself (:class:`hiperwalk.graph.Graph`) or
         its adjacency matrix (:class:`scipy.sparse.csr_array`).
 
     adjacency : :class:`scipy.sparse.csr_array`, optional
-        .. deprecated:: 2.0
-            It will be removed in version 2.1.
+        .. deprecated:: 2.0a1
+            It will be removed in version 2.0.
             Use ``graph`` instead.
 
         The adjacency matrix.
 
-    Attributes
-    ----------
-    hilb_dim : int, default=0
-        Hilbert Space dimension.
-        It must be updated by the subclass' ``__init__``.
-
     Warns
     -----
     If ``adjacency`` is set. It is deprecated. Use ``graph`` instead.
 
     Raises
     ------
     TypeError
@@ -111,24 +105,24 @@
 
 
     def uniform_state(self):
         r"""
         Generate the uniform state.
 
         The state is constructed based on the ``hilb_dim`` attribute.
-        The uniform initial condition is the state where
+        The uniform initial state is the state where
         all entries have the same amplitude.
 
         Returns
         -------
         :obj:`numpy.ndarray`
 
         Notes
         -----
-        The uniform initial condition is the state
+        The uniform initial state is the state
 
         .. math::
 
             \ket{d} = \frac{1}{\sqrt{N}} \sum_{i = 0}^{N - 1} \ket{i}
 
         where :math:`N` is the dimension of the Hilbert space.
         """
@@ -143,15 +137,15 @@
         ----------
         marked : list of int or int
             List of vertices to be marked.
             If empty list, no vertex is marked.
         """
         if not hasattr(marked, '__iter__'):
             marked = [marked]
-        self._marked = set(marked)
+        self._marked = list(set(marked))
         self._evolution = None
 
     def get_marked(self):
         r"""
         Gets marked vertices.
 
         Returns
@@ -350,20 +344,21 @@
     def _pyneblina_imported(self):
         """
         Expects pyneblina interface to be imported as nbl
         """
         return ('hiperwalk.quantum_walk._pyneblina_interface'
                 in sys_modules)
 
-    def simulate(self, time=None, initial_condition=None, hpc=True):
+    def simulate(self, time=None, initial_state=None,
+                 initial_condition=None, hpc=True):
         r"""
         Simulates the quantum walk.
 
         Simulates the quantum walk applying the evolution operator
-        multiple times to the initial condition.
+        multiple times to the initial state.
 
         Parameters
         ----------
         time : int, tuple of int, default=None
             Describes at which time instants the state must be saved.
             It can be specified in three different ways.
             
@@ -376,18 +371,24 @@
                 that is multiple of ``step``.
 
             * (start, end, step)
                 Saves every state from time ``start`` (inclusive)
                 to time ``end`` (inclusive)
                 that is multiple of ``step``.
 
-        initial_condition : :class:`numpy.array`, default=None
-            The initial condition which the evolution operator
+        initial_state : :class:`numpy.array`, default=None
+            The initial state which the evolution operator
             is going to be applied to.
 
+        initial_condition :
+            .. deprecated:: 2.0a4
+                It will be removed in Hiperwalk 2.0
+                due to nomenclature consistency.
+                Use ``initial_state`` instead.
+
         hpc : bool, default=True
             Whether or not to use neblina's high-performance computing
             to perform matrix multiplications.
             If ``hpc=False`` uses standalone python.
 
         Returns
         -------
@@ -396,26 +397,26 @@
             ``states[i]`` corresponds to the ``i``-th saved state.
 
         Raises
         ------
         ValueError
             If any of the following occurs
             * ``time=None``.
-            * ``initial_condition=None``.
+            * ``initial_state=None``.
             * ``evolution_operator=None`` and it was no set previously.
 
         See Also
         --------
         evolution_operator
         state
 
         Notes
         -----
         The walk is simulated by applying the
-        evolution operator to the initial condition multiple times.
+        evolution operator to the initial state multiple times.
         The maximum and intermediate applications
         are describred by ``time``.
 
         Examples
         --------
         If ``time=(0, 13, 3)``, the saved states will be:
         the initial state (0), the intermediate states (3, 6, and 9),
@@ -426,38 +427,44 @@
         ############################################
         if time is None:
             raise ValueError(
                 "``time` not specified`. "
                 + "Must be an int or tuple of int."
             )
 
-        if initial_condition is None:
-            raise ValueError(
-                "``initial_condition`` not specified. "
-                + "Expected a np.array."
-            )
+        if initial_state is None:
+            if initial_condition is None:
+                raise ValueError(
+                    "``initial_state`` not specified. "
+                    + "Expected a np.array."
+                )
+            else:
+                initial_state = initial_condition
+                warn('\n`initial_condition` is deprecated. '
+                     + 'It will be removed in version 2.0. '
+                     + 'Use `initial_state` instead.')
 
-        if len(initial_condition) != self.hilb_dim:
+        if len(initial_state) != self.hilb_dim:
             raise ValueError(
                 "Initial condition has invalid dimension. "
                 + "Expected an np.array with length " + str(self.hilb_dim)
             )
 
         ###########################
         ### Auxiliary functions ###
         ###########################
 
         def __prepare_engine(self):
             if hpc:
                 self._simul_mat = nbl.send_matrix(self._evolution)
-                self._simul_vec = nbl.send_vector(initial_condition)
+                self._simul_vec = nbl.send_vector(initial_state)
 
             else:
                 self._simul_mat = self._evolution
-                self._simul_vec = initial_condition
+                self._simul_vec = initial_state
 
         def __simulate_step(self, step):
             """
             Apply the simulation evolution operator ``step`` times
             to the simulation vector.
             Simulation vector is then updated.
             """
@@ -507,28 +514,28 @@
         __prepare_engine(self)
 
         # number of states to save
         num_states = int(end/step) + 1
         num_states -= (int((start - 1)/step) + 1) if start > 0 else 0
 
         # create saved states matrix
-        # TODO: error: if initial condition is int and
+        # TODO: error: if initial state is int and
         # evolution operator is float, dtype is complex
-        dtype = (initial_condition.dtype if
-            initial_condition.dtype == self._evolution.dtype
+        dtype = (initial_state.dtype if
+            initial_state.dtype == self._evolution.dtype
             else complex
         )
         saved_states = np.zeros(
-            (num_states, initial_condition.shape[0]), dtype=dtype
+            (num_states, initial_state.shape[0]), dtype=dtype
         )
         state_index = 0 # index of the state to be saved
 
         # if save_initial_state:
         if start == 0:
-            saved_states[0] = initial_condition.copy()
+            saved_states[0] = initial_state.copy()
             state_index += 1
             num_states -= 1
 
         # simulate walk / apply evolution operator
         if start > 0:
             __simulate_step(self, start - step)
 
@@ -547,7 +554,13 @@
     def _get_valid_kwargs(method):
         return inspect.getfullargspec(method)[0][1:]
 
     @staticmethod
     def _filter_valid_kwargs(kwargs, valid_kwargs):
         return {k : kwargs.get(k) for k in valid_kwargs if k in kwargs}
                 #if kwargs.get(k) is not None}
+
+    def hilbert_space_dimension(self):
+        """
+        Returns dimension of the Hilbert space.
+        """
+        return self.hilb_dim
```

### Comparing `hiperwalk-2.0a3/tests/unitary/coined_cycle.py` & `hiperwalk-2.0a4/tests/unitary/coined_cycle.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/tests/unitary/coined_line.py` & `hiperwalk-2.0a4/tests/unitary/coined_line.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/tests/unitary/coined_segment.py` & `hiperwalk-2.0a4/tests/unitary/coined_segment.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/tests/unitary/continuous_graph.py` & `hiperwalk-2.0a4/tests/unitary/continuous_graph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/.gitignore` & `hiperwalk-2.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/LICENSE` & `hiperwalk-2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/README.md` & `hiperwalk-2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a3/pyproject.toml` & `hiperwalk-2.0a4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hiperwalk"
-version = "2.0a3"
+version = "2.0a4"
 description = "High-Performance Quantum Walk Simulator"
 license = {file="LICENSE"}
 readme = "README.md"
 authors = [
   { name="Gustavo Bezerra", email="gbezerra@posgrad.lncc.br" },
   { name="Paulo Motta", email="prmottajr@gmail.com" },
   { name="Renato Portugal", email="portugal@lncc.br" },
```

### Comparing `hiperwalk-2.0a3/PKG-INFO` & `hiperwalk-2.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiperwalk
-Version: 2.0a3
+Version: 2.0a4
 Summary: High-Performance Quantum Walk Simulator
 Project-URL: homepage, http://qubit.lncc.br/qwalk/
 Project-URL: documentation, https://hiperwalk.readthedocs.io/
 Project-URL: source, https://github.com/hiperwalk/hiperwalk
 Author-email: Gustavo Bezerra <gbezerra@posgrad.lncc.br>, Paulo Motta <prmottajr@gmail.com>, Renato Portugal <portugal@lncc.br>
 Maintainer-email: Hiperwalk Organization <hiperwalk@gmail.com>
 License: GNU Lesser General Public License
```

