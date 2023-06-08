# Comparing `tmp/magicsoup-0.3.9.tar.gz` & `tmp/magicsoup-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.3.9.tar", last modified: Tue May  2 11:49:54 2023, max compression
+gzip compressed data, was "magicsoup-0.4.0.tar", last modified: Thu Jun  8 20:20:10 2023, max compression
```

## Comparing `magicsoup-0.3.9.tar` & `magicsoup-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-02 11:49:54.675226 magicsoup-0.3.9/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.9/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-05-02 11:49:54.675226 magicsoup-0.3.9/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.9/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.9/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-05-02 11:49:54.675226 magicsoup-0.3.9/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-02 11:49:54.675226 magicsoup-0.3.9/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-02 11:49:54.675226 magicsoup-0.3.9/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-05-02 11:49:42.000000 magicsoup-0.3.9/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.3.9/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-27 20:14:11.000000 magicsoup-0.3.9/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-02 11:49:54.675226 magicsoup-0.3.9/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.9/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.9/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.9/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.9/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.3.9/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    30687 2023-04-27 20:15:08.000000 magicsoup-0.3.9/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.3.9/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.9/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    42969 2023-05-02 11:48:17.000000 magicsoup-0.3.9/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-02 11:49:54.675226 magicsoup-0.3.9/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-05-02 11:49:54.000000 magicsoup-0.3.9/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      671 2023-05-02 11:49:54.000000 magicsoup-0.3.9/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-05-02 11:49:54.000000 magicsoup-0.3.9/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-05-02 11:49:54.000000 magicsoup-0.3.9/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-05-02 11:49:54.675226 magicsoup-0.3.9/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.9/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.9/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    46871 2023-04-27 20:17:09.000000 magicsoup-0.3.9/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.3.9/tests/test_mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.9/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    19437 2023-05-01 19:52:39.000000 magicsoup-0.3.9/tests/test_world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.4.0/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-06-08 20:20:10.332495 magicsoup-0.4.0/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4361 2023-05-29 15:40:09.000000 magicsoup-0.4.0/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.4.0/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-06-08 20:20:10.332495 magicsoup-0.4.0/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      119 2023-06-08 20:19:57.000000 magicsoup-0.4.0/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-27 20:14:44.000000 magicsoup-0.4.0/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    25381 2023-06-08 20:05:48.000000 magicsoup-0.4.0/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.4.0/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.4.0/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.4.0/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.4.0/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-27 20:14:54.000000 magicsoup-0.4.0/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    40436 2023-06-08 19:43:19.000000 magicsoup-0.4.0/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-05-01 20:15:52.000000 magicsoup-0.4.0/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.4.0/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    45267 2023-05-29 15:43:01.000000 magicsoup-0.4.0/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5298 2023-06-08 20:20:10.000000 magicsoup-0.4.0/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      671 2023-06-08 20:20:10.000000 magicsoup-0.4.0/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-06-08 20:20:10.000000 magicsoup-0.4.0/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-06-08 20:20:10.000000 magicsoup-0.4.0/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-06-08 20:20:10.332495 magicsoup-0.4.0/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      950 2023-05-29 15:58:52.000000 magicsoup-0.4.0/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.4.0/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    49435 2023-06-06 21:41:32.000000 magicsoup-0.4.0/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1041 2023-05-01 20:29:24.000000 magicsoup-0.4.0/tests/test_mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.4.0/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    24597 2023-06-08 18:10:34.000000 magicsoup-0.4.0/tests/test_world.py
```

### Comparing `magicsoup-0.3.9/LICENSE` & `magicsoup-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/PKG-INFO` & `magicsoup-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.9
+Version: 0.4.0
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
@@ -130,12 +130,12 @@
 ```python
 for _ in range(1000):
     world.enzymatic_activity()
     kill_cells()
     replicate_cells()
     mutate_cells()
     world.diffuse_molecules()
-    world.increment_cell_survival()
+    world.increment_cell_lifetimes()
 ```
 
 See the [Docs](https://magic-soup.readthedocs.io/) for more examples and a description of all the mechanics of this simulation
```

### Comparing `magicsoup-0.3.9/README.md` & `magicsoup-0.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -107,12 +107,12 @@
 ```python
 for _ in range(1000):
     world.enzymatic_activity()
     kill_cells()
     replicate_cells()
     mutate_cells()
     world.diffuse_molecules()
-    world.increment_cell_survival()
+    world.increment_cell_lifetimes()
 ```
 
 See the [Docs](https://magic-soup.readthedocs.io/) for more examples and a description of all the mechanics of this simulation
```

### Comparing `magicsoup-0.3.9/pyproject.toml` & `magicsoup-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/src/magicsoup/constants.py` & `magicsoup-0.4.0/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/src/magicsoup/containers.py` & `magicsoup-0.4.0/src/magicsoup/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import torch
 import warnings
+from collections import Counter
 
 
 class Molecule:
     """
     Represents a molecule species which is part of the world, can diffuse, degrade,
     and be converted into other molecules.
 
@@ -188,22 +189,31 @@
 
     Arguments:
         molecules: List of all molecules species that are part of this simulation
         reactions: List of all possible reactions in this simulation as a list of tuples: `(substrates, products)`.
             All reactions can happen in both directions (left to right or vice versa).
 
     `molecules` should include at least all molecule species that are mentioned in `reactions`.
-    But it is possible to define more molecule species. Cells could use any molecule species in transporer or regulatory domains.
+    But it is possible to define more molecule species. Cells can use any molecule species in transporer or regulatory domains.
 
     Duplicate reactions and molecules will be removed on initialization.
     As any reaction can take place in both directions, it is not necessary to define both directions.
     To combine multiple chemistries you can do `both = chemistry1 & chemistry2` which will combine all molecules and reactions.
 
     The chemistry object is used by [World][magicsoup.world.World] to know what molecule species exist.
     Reactions and molecule species are used to set up the world and create mappings for domains.
+    On the [world][magicsoup.world.World] object there are some tensors that refer to molecule species (e.g. `world.molecule_map`).
+    The molecule ordering in such tensors is always the same as the ordering in `chemistry.molecules`.
+    So, e.g. if `chemistry.molecules[2]` is pyruvate, `world.molecule_map[2]` refers to the pyruvate concentration
+    of the world molecule map.
+    For convenience mappings are provided:
+
+    - `chemistry.mol_2_idx` to map a [Molecule][magicsoup.containers.Molecule] object
+    - `chemistry.molname_2_idx` to map a [Molecule][magicsoup.containers.Molecule] name string to its index.
+
     """
 
     def __init__(
         self,
         molecules: list[Molecule],
         reactions: list[tuple[list[Molecule], list[Molecule]]],
     ):
@@ -223,14 +233,17 @@
         if react_mols > dfnd_mols:
             raise ValueError(
                 "These molecules were not defined but are part of some reactions:"
                 f" {', '.join(str(d) for d in react_mols - dfnd_mols)}."
                 "Please define all molecules."
             )
 
+        self.mol_2_idx = {d: i for i, d in enumerate(self.molecules)}
+        self.molname_2_idx = {d.name: i for i, d in enumerate(self.molecules)}
+
     def __and__(self, other: "Chemistry") -> "Chemistry":
         return Chemistry(
             molecules=self.molecules + other.molecules,
             reactions=self.reactions + other.reactions,
         )
 
     def to_dict(self) -> dict:
@@ -291,15 +304,23 @@
         self.products = prods
         self.km = km
         self.vmax = vmax
 
     def __repr__(self) -> str:
         ins = ",".join(str(d) for d in self.substrates)
         outs = ",".join(str(d) for d in self.products)
-        return f"CatalyticDomain({ins}->{outs},Km={self.km:.2e},Vmax{self.vmax:.2e})"
+        return f"CatalyticDomain({ins}<->{outs},Km={self.km:.2e},Vmax{self.vmax:.2e})"
+
+    def __str__(self) -> str:
+        subs_cnts = Counter(str(d) for d in self.substrates)
+        prods_cnts = Counter([str(d) for d in self.products])
+        subs_str = " + ".join([f"{d} {k}" for k, d in subs_cnts.items()])
+        prods_str = " + ".join([f"{d} {k}" for k, d in prods_cnts.items()])
+        spec = self.vmax / self.km
+        return f"{subs_str} <-> {prods_str} | spec {spec:.2e}"
 
 
 class CatalyticDomainFact:
     """
     Container for describing a catalytic domain.
 
     Arguments:
@@ -342,14 +363,18 @@
         self.vmax = vmax
 
     def __repr__(self) -> str:
         return (
             f"TransporterDomain({self.molecule},Km={self.km:.2e},Vmax={self.vmax:.2e})"
         )
 
+    def __str__(self) -> str:
+        spec = self.vmax / self.km
+        return f"{self.molecule} transporter | spec {spec:.2e}"
+
 
 class TransporterDomainFact:
     """
     Container for describing a transporter domain.
 
     Arguments:
         molecule: The molecule species which can be transported into or out of the cell by this domain.
@@ -397,14 +422,19 @@
         self.is_inhibiting = is_inhibiting
 
     def __repr__(self) -> str:
         loc = "transmembrane" if self.is_transmembrane else "cytosolic"
         eff = "inhibiting" if self.is_inhibiting else "activating"
         return f"ReceptorDomain({self.effector},Km={self.km:.2e},{loc},{eff})"
 
+    def __str__(self) -> str:
+        loc = "[e]" if self.is_transmembrane else "[i]"
+        post = "inhibitor" if self.is_inhibiting else "activator"
+        return f"{self.effector}{loc} {post} | Km {self.km:.2e}"
+
 
 class RegulatoryDomainFact:
     """
     Container for describing a regulatory domain.
 
     Arguments:
         effector: The molecule species which will be the effector molecule.
@@ -443,14 +473,18 @@
         self.n_domains = len(domains)
 
     def __repr__(self) -> str:
         kwargs = {"domains": self.domains}
         args = [f"{k}:{repr(d)}" for k, d in kwargs.items()]
         return f"{type(self).__name__}({','.join(args)})"
 
+    def __str__(self) -> str:
+        domstrs = [str(d).split(" | ")[0] for d in self.domains]
+        return " | ".join(domstrs)
+
 
 class ProteinFact:
     """
     Container for describing a protein
 
     Arguments:
         domain_facts: List of all domains, each described by a domain factory.
@@ -458,15 +492,17 @@
     This is currently only used for [World.generate_genome()][magicsoup.world.World.generate_genome].
     Use this factory to describe a protein that should eventually be encoded.
     Domain factories can be [CatalyticDomainFact][magicsoup.containers.CatalyticDomainFact],
     [TransporterDomainFact][magicsoup.containers.TransporterDomainFact],
     [RegulatoryDomainFact][magicsoup.containers.RegulatoryDomainFact].
     """
 
-    def __init__(self, domain_facts: list[DomainFactType]):
+    def __init__(self, domain_facts: list[DomainFactType] | DomainFactType):
+        if not isinstance(domain_facts, list):
+            domain_facts = [domain_facts]
         self.domain_facts = domain_facts
         self.n_domains = len(domain_facts)
 
 
 class Cell:
     """
     Object representing a cell with its environment.
@@ -478,15 +514,15 @@
             each molecule species in the same order as defined in [Chemistry][magicsoup.containers.Chemistry].
         ext_molecules: Extracellular molecules. A tensor with one dimension that represents
             each molecule species in the same order as defined in [Chemistry][magicsoup.containers.Chemistry].
             These are the molecules of the pixel the cell is currently living on.
         position: Position on the cell map.
         idx: The current index of this cell.
         label: Label which can be used to track cells. Has no effect.
-        n_survived_steps: Number of time steps this cell has survived.
+        n_steps_alive: Number of time steps this cell has lived since last division.
         n_divisions: Number of times this cell's ancestors already divided.
 
     Usually, you wouldn't instantiate this object.
     You get it when calling [get_cell()][magicsoup.world.World.get_cell] after you have added some
     cells to a world (via [add_cells()][magicsoup.world.World.add_cells]).
     On the `world` object all cells are actually represented as a combination of lists and tensors.
     [get_cell()][magicsoup.world.World.get_cell] gathers all information for one cell and
@@ -504,44 +540,44 @@
         genome: str,
         proteome: list[Protein],
         int_molecules: torch.Tensor,
         ext_molecules: torch.Tensor,
         position: tuple[int, int] = (-1, -1),
         idx: int = -1,
         label: str = "C",
-        n_survived_steps: int = -1,
+        n_steps_alive: int = -1,
         n_divisions: int = -1,
     ):
         self.genome = genome
         self.proteome = proteome
         self.label = label
         self.int_molecules = int_molecules
         self.ext_molecules = ext_molecules
         self.position = position
         self.idx = idx
-        self.n_survived_steps = n_survived_steps
+        self.n_steps_alive = n_steps_alive
         self.n_divisions = n_divisions
 
     def copy(self, **kwargs) -> "Cell":
         old_kwargs = {
             "genome": self.genome,
             "proteome": self.proteome,
             "position": self.position,
             "idx": self.idx,
             "label": self.label,
-            "n_survived_steps": self.n_survived_steps,
+            "n_steps_alive": self.n_steps_alive,
             "n_divisions": self.n_divisions,
         }
         return Cell(**{**old_kwargs, **kwargs})  # type: ignore
 
     def __repr__(self) -> str:
         kwargs = {
             "genome": self.genome,
             "proteome": self.proteome,
             "position": self.position,
             "idx": self.idx,
             "label": self.label,
-            "n_survived_steps": self.n_survived_steps,
+            "n_steps_alive": self.n_steps_alive,
             "n_divisions": self.n_divisions,
         }
         args = [f"{k}:{repr(d)}" for k, d in kwargs.items()]
         return f"{type(self).__name__}({','.join(args)})"
```

### Comparing `magicsoup-0.3.9/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.4.0/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.4.0/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.4.0/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/src/magicsoup/genetics.py` & `magicsoup-0.4.0/src/magicsoup/genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/src/magicsoup/kinetics.py` & `magicsoup-0.4.0/src/magicsoup/kinetics.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,37 +8,45 @@
     Protein,
     CatalyticDomain,
     TransporterDomain,
     RegulatoryDomain,
     DomainType,
 )
 
+_EPS = 1e-8
+_MIN = 1e-45
+_MAX = 1e38
 
-_EPS = 1e-5
 
-
-class _LogWeightMapFact:
+class _LogNormWeightMapFact:
     """
     Creates an object that maps tokens to a float
-    which is sampled from a log uniform distribution.
+    which is sampled from a log normal distribution.
     """
 
     def __init__(
         self,
         max_token: int,
         weight_range: tuple[float, float],
         device: str = "cpu",
         zero_value: float = torch.nan,
     ):
-        l_min_w = math.log(min(weight_range))
-        l_max_w = math.log(max(weight_range))
-        weights = torch.tensor(
-            [zero_value]
-            + [math.exp(random.uniform(l_min_w, l_max_w)) for _ in range(max_token)]
-        )
+        min_w = min(weight_range)
+        max_w = max(weight_range)
+        l_min_w = math.log(min_w)
+        l_max_w = math.log(max_w)
+        mu = (l_min_w + l_max_w) / 2
+        sig = l_max_w - l_min_w
+        non_zero_weights: list[float] = []
+        for _ in range(max_token):
+            sample = math.exp(random.gauss(mu, sig))
+            while not min_w <= sample <= max_w:
+                sample = math.exp(random.gauss(mu, sig))
+            non_zero_weights.append(sample)
+        weights = torch.tensor([zero_value] + non_zero_weights)
         self.weights = weights.to(device)
 
     def __call__(self, t: torch.Tensor) -> torch.Tensor:
         """t: long (c, p, d)"""
         return self.weights[t]
 
 
@@ -55,15 +63,15 @@
 
     def __call__(self, t: torch.Tensor) -> torch.Tensor:
         """t: long (c, p, d)"""
         return self.signs[t]
 
     def inverse(self) -> dict[bool, list[int]]:
         sign_map = {}
-        M = self.signs
+        M = self.signs.to("cpu")
         sign_map[True] = torch.argwhere(M == 1.0).flatten().tolist()
         sign_map[False] = torch.argwhere(M == -1.0).flatten().tolist()
         return sign_map
 
 
 class _VectorMapFact:
     """
@@ -158,15 +166,15 @@
         react_map = {}
         for subs, prods in reactions:
             t = torch.zeros(n_signals)
             for sub in subs:
                 t[molmap[sub]] -= 1
             for prod in prods:
                 t[molmap[prod]] += 1
-            M = self.M
+            M = self.M.to("cpu")
             idxs = torch.argwhere((M == t).all(dim=1)).flatten().tolist()
             react_map[(tuple(subs), tuple(prods))] = idxs
         return react_map
 
 
 class _TransporterMapFact(_VectorMapFact):
     """
@@ -199,15 +207,15 @@
             device=device,
             zero_value=zero_value,
         )
 
     def inverse(self, molecules: list[Molecule]) -> dict[Molecule, list[int]]:
         trnsp_map = {}
         for mi, mol in enumerate(molecules):
-            M = self.M
+            M = self.M.to("cpu")
             idxs = torch.argwhere(M[:, mi] != 0).flatten().tolist()
             trnsp_map[mol] = idxs
         return trnsp_map
 
 
 class _RegulatoryMapFact(_VectorMapFact):
     """
@@ -238,15 +246,15 @@
             device=device,
             zero_value=zero_value,
         )
 
     def inverse(self, molecules: list[Molecule]) -> dict[Molecule, list[int]]:
         reg_map = {}
         for mi, mol in enumerate(molecules):
-            M = self.M
+            M = self.M.to("cpu")
             idxs = torch.argwhere(M[:, mi] != 0).flatten().tolist()
             reg_map[mol] = idxs
         return reg_map
 
 
 class Kinetics:
     """
@@ -254,102 +262,156 @@
     Usually this class is instantiated automatically when initializing [World][magicsoup.world.World].
     You can access it on `world.kinetics`.
 
     Arguments:
         molecules: List of molecule species.
             They have to be in the same order as they are on `chemistry.molecules`.
         reactions: List of all possible reactions in this simulation as a list of tuples: `(substrates, products)`.
-            All reactions can happen in both directions (left to right or vice versa).
+            All reactions are reversible and happen in both directions (left to right or vice versa).
         abs_temp: Absolute temperature in Kelvin will influence the free Gibbs energy calculation of reactions.
             Higher temperature will give the reaction quotient term higher importance.
-        km_range: The range from which to sample Michaelis Menten constants for domains (in mol).
-            The sampling will happen in the log transformed intervall, so all values must be > 0.
-        vmax_range: The range from which to sample maximum velocities for domains (in mol per time step).
-            The sampling will happen in the log transformed intervall, so all values must be > 0.
+        km_range: The range from which to sample Michaelis Menten constants for domains (in mM).
+            They are sampled from a lognormal distribution, so all values must be > 0.
+        vmax_range: The range from which to sample maximum velocities for domains (in mM/s).
+            They are sampled from a lognormal distribution, so all values must be > 0.
         device: Device to use for tensors
             (see [pytorch CUDA semantics](https://pytorch.org/docs/stable/notes/cuda.html)).
             This has to be the same device that is used by `world`.
         scalar_enc_size: Number of tokens that can be used to encode the scalars Vmax, Km, and sign.
             This should be the output of `max(genetics.one_codon_map.values())`.
         vector_enc_size: Number of tokens that can be used to encode the vectors for reactions and molecules.
             This should be the output of `max(genetics.two_codon_map.values())`.
+        n_computations: In how many computations to integrate signals. With a higher number chemical equilibriums
+            are reached smoother but it takes more time to compute (see details below about computation).
+        alpha: A trimming factor used to trim velocity at each step during signal integration. This number
+            can be adjusted if `n_computations` is changed and reactions don't reach their equilibrium state
+            anymore (see details below about computation).
 
     There are `c` cells, `p` proteins, `s` signals.
     Signals are basically molecule species, but we have to differentiate between intra- and extracellular molecule species.
     So, there are twice as many signals as molecule species.
     The order of molecule species is always the same as in `chemistry.molecules`.
     First, all intracellular molecule species are listed, then all extracellular.
     The order of cells is always the same as in `world.genomes` and the order of proteins
     for every cell is always the same as the order of proteins in a cell object `cell.proteome`.
 
     Attributes on this class describe cell parameters:
 
-    - `Km` Affinities to every signal that is processed by each protein in every cell (c, p, s).
+    - `Kmf`, `Kmb`, `Kmr` Affinities to every signal that is processed by each protein in every cell (c, p, s).
+      There are affinities for (f)orward and (b)ackward reactions, and for (r)egulatory domains.
     - `Vmax` Maximum velocities of every protein in every cell (c, p).
     - `E` Standard reaction Gibbs free energy of every protein in every cell (c, p).
     - `N` Stoichiometric number for every signal that is processed by each protein in every cell (c, p, s).
+      Additionally, there are `Nf` and `Nb` which describe only forward and backward stoichiometric numbers.
+      This is needed in addition to `N` to properly describe reactions that involve molecules
+      which are not changed, _i.e._ where `n=0`.
     - `A` Regulatory effect for each signal in every protein in every cell (c, p, s).
       This is looks similar to a stoichiometric number. Numbers > 0.0 mean these molecules
       act as activating effectors, numbers < 0.0 mean these molecules act as inhibiting effectors.
 
     The main method is [integrate_signals()][magicsoup.kinetics.Kinetics].
     When calling [enzymatic_activity()][magicsoup.world.World.enzymatic_activity], a matrix `X` of signals (c, s) is prepared
     and then [integrate_signals(X)][magicsoup.kinetics.Kinetics] is called.
     Updated signals are returned and [World][magicsoup.world.World] writes them back to `world.cell_molecules` and `world.molecule_map`.
 
     Another method, which ended up here, is [set_cell_params()][magicsoup.kinetics.Kinetics.set_cell_params]
     which reads proteomes and updates cell parameters accordingly.
     This is called whenever the proteomes of some cells changed.
-    Currently, this is also the main bottleneck in performance.
+    Currently, this is also the main performance bottleneck.
 
     When this class is initialized it generates the mappings from nucleotide sequences to domains by random sampling.
     These mappings are then used throughout the simulation.
     If you initialize this class again, these mappings will be different.
     Initializing [World][magicsoup.world.World] will also create one `Kinetics` instance. It is on `world.kinetics`.
     If you want to access nucleotide to domain mappings of your simulation, you should use `world.kinetics`.
+
+    The kinetics used here can never create negative molecule concentrations and make the reaction quotient move
+    towards to equilibrium constant at all times.
+    However, this simulation computes these things one step at a time
+    (with the premise that one step should be something similar to 1s).
+    This and the numerical limits of data types used here can create edge cases that need to be dealth with:
+    reaction quotients overshooting the equilibrium state and negative concentrations.
+    Both are caused by high $V_{max}$ with low $K_m$ values.
+
+    If an enzyme is far away from its equilibrium state $K_e$ and substrate concentrations are far above $K_M$ it
+    will progress its reaction at full speed $V_{max}$. This rate can be so high that, within one step, $Q$ surpasses
+    $K_E$. In the next step it will move at full speed into the opposite direction, overshooting $K_E$ again, and so on.
+    Reactions with high stoichiometric numbers are more prone to this as their rate functions are sharper.
+    To combat this one can divide the whole computation into many steps.
+    This is what `n_computations` is for. $V_{max}$ is decreased appropriately.
+    However, with this alone one would have to perform over 100 computations per step in order to make some
+    extreme reactions reach their equilibrium state.
+    Thus, with each computation in `n_computations` the reaction rate is exponentially decayed.
+    This has the effect that, while in the first few computations a reaction might still overshoot $K_E$,
+    during the last computations rates are so low, that even extremely volatile reactions can come close
+    to their intended equilibrium. The factor of this exponential decay is `alpha`.
+    For $V_{max} \le 100$ and $K_M \ge 0.01$ `n_computations=11` and `alpha=0.6` seem to work very well
+    (few computations, but stable equilibriums). You can always increase `n_computations`, but if you
+    decrease it, you might also want to try out different `alpha` values.
+
+    With the `n_computation` and `alpha` trick above, chances of enzymes trying to deconstruct more
+    substrate than available is very low. However, it can still happen. Sometimes it is also floating point
+    inaccuracies that can tip a near-zero value below zero. Thus, before the updated signals tensor `X`
+    gets returned, it is checked for negative concentrations.
+    Then, protein velocities for all cells with below zero concentrations is reduced and `X` is calculated again.
+    They are reduced by a factor that will create $X = \epsilon \gt 0$ for the signals that
+    were negative in the first calculation.
     """
 
     def __init__(
         self,
         molecules: list[Molecule],
         reactions: list[tuple[list[Molecule], list[Molecule]]],
         abs_temp: float = 310.0,
-        km_range: tuple[float, float] = (1e-5, 1.0),
-        vmax_range: tuple[float, float] = (0.01, 10.0),
+        km_range: tuple[float, float] = (1e-2, 100.0),
+        vmax_range: tuple[float, float] = (1e-3, 100.0),
         device: str = "cpu",
         scalar_enc_size: int = 64 - 3,
         vector_enc_size: int = 4096 - 3 * 64,
+        n_computations: int = 11,
+        alpha: float = 0.6,
     ):
         self.abs_temp = abs_temp
         self.device = device
         self.abs_temp = abs_temp
 
+        # calculate signal integration in n_computation steps
+        # to reach equilibrium Ke faster, steps get increasingly slower
+        # trim(i) = trim0 * alpha^i and sum(trim0 * alpha^i) = 1 over all i
+        self.n_computations = n_computations
+        self.alpha = alpha
+        self.n_comp_trim = 1 / sum(self.alpha**d for d in range(self.n_computations))
+
         self.mol_energies = self._tensor_from([d.energy for d in molecules] * 2)
         self.mol_2_mi = {d: i for i, d in enumerate(molecules)}
         self.mi_2_mol = {v: k for k, v in self.mol_2_mi.items()}
+        self.molecules = molecules
 
         # working cell params
         n_signals = 2 * len(molecules)
-        self.Km = self._tensor(0, 0, n_signals)
+        self.Kmf = self._tensor(0, 0)
+        self.Kmb = self._tensor(0, 0)
+        self.Kmr = self._tensor(0, 0)
         self.Vmax = self._tensor(0, 0)
-        self.E = self._tensor(0, 0)
         self.N = self._tensor(0, 0, n_signals)
+        self.Nf = self._tensor(0, 0, n_signals)
+        self.Nb = self._tensor(0, 0, n_signals)
         self.A = self._tensor(0, 0, n_signals)
 
         # the domain specifications return 4 indexes
         # idx 0-2 are 1-codon idxs for scalars (n=64)
         # idx3 is a 2-codon idx for vetors (n=4096)
 
-        self.km_map = _LogWeightMapFact(
+        self.km_map = _LogNormWeightMapFact(
             max_token=scalar_enc_size,
             weight_range=km_range,
             device=device,
         )
 
-        self.vmax_map = _LogWeightMapFact(
+        self.vmax_map = _LogNormWeightMapFact(
             max_token=scalar_enc_size,
             weight_range=vmax_range,
             device=device,
         )
 
         self.sign_map = _SignMapFact(max_token=scalar_enc_size, device=device)
 
@@ -390,75 +452,68 @@
             A list of objects that represent proteins with domains and their
             specifications.
         """
         N_d, A_d, Km_d, Vmax_d, dom_types = self._get_proteome_tensors(
             proteomes=[proteome]
         )
 
+        Nf_d = torch.where(N_d < 0.0, -N_d, 0.0)
+        Nb_d = torch.where(N_d > 0.0, N_d, 0.0)
+        mols = self.molecules
+        n_mols = len(mols)
+
         prots: list[Protein] = []
         for pi in range(dom_types.size(1)):
-            is_useful = False
-
             doms: list[DomainType] = []
             for di in range(dom_types.size(2)):
                 # catalytic domain (N has positive and negative integers)
                 if dom_types[0][pi][di].item() == 1:
-                    lfts: list[Molecule] = []
-                    rgts: list[Molecule] = []
-                    for mi, n in enumerate(N_d[0][pi][di].tolist()):
-                        if n >= 1:
-                            rgts.extend(([self.mi_2_mol[mi]] * int(n)))
-                        elif n <= -1:
-                            lfts.extend(([self.mi_2_mol[mi]] * -int(n)))
+                    lft_ns = Nf_d[0][pi][di].int().tolist()
+                    rgt_ns = Nb_d[0][pi][di].int().tolist()
+                    lfts = [m for m, n in zip(mols, lft_ns) for _ in range(n)]
+                    rgts = [m for m, n in zip(mols, rgt_ns) for _ in range(n)]
                     if len(lfts) > 0:
-                        mi = self.mol_2_mi[lfts[0]]
                         doms.append(
                             CatalyticDomain(
                                 reaction=(lfts, rgts),
-                                km=Km_d[0][pi][di][mi].item(),
+                                km=Km_d[0][pi][di].item(),
                                 vmax=Vmax_d[0][pi][di].item(),
                             )
                         )
-                        is_useful = True
 
                 # transporter domain (N has one +1 and one -1)
                 if dom_types[0][pi][di].item() == 2:
-                    lft = int(torch.argwhere(N_d[0][pi][di] == -1)[0].item())
-                    rgt = int(torch.argwhere(N_d[0][pi][di] == 1)[0].item())
-                    mi = lft if lft in self.mi_2_mol else rgt
+                    mis = torch.argwhere(N_d[0][pi][di] != 0).int().flatten().tolist()
                     doms.append(
                         TransporterDomain(
-                            molecule=self.mi_2_mol[mi],
-                            km=Km_d[0][pi][di][mi].item(),
+                            molecule=self.mi_2_mol[min(mis)],
+                            km=Km_d[0][pi][di].item(),
                             vmax=Vmax_d[0][pi][di].item(),
                         )
                     )
-                    is_useful = True
 
-                # regulatory domain (A has values != 0)
+                # regulatory domain (A has one +1 or -1)
                 if dom_types[0][pi][di].item() == 3:
                     mi = int(torch.argwhere(A_d[0][pi][di] != 0)[0].item())
                     if mi in self.mi_2_mol:
                         is_trnsm = False
                         mol = self.mi_2_mol[mi]
                     else:
                         is_trnsm = True
-                        mol = self.mi_2_mol[mi - len(self.mi_2_mol)]
+                        mol = self.mi_2_mol[mi - n_mols]
                     doms.append(
                         RegulatoryDomain(
                             effector=mol,
-                            km=Km_d[0][pi][di][mi].item(),
+                            km=Km_d[0][pi][di].item(),
                             is_inhibiting=bool((A_d[0][pi][di][mi] == -1).item()),
                             is_transmembrane=is_trnsm,
                         )
                     )
 
-            # ignore proteins without a non-regulatory domain
-            if is_useful:
-                prots.append(Protein(domains=doms))
+            prots.append(Protein(domains=doms))
 
         return prots
 
     def set_cell_params(
         self,
         cell_idxs: list[int],
         proteomes: list[list[list[tuple[int, int, int, int, int]]]],
@@ -472,39 +527,106 @@
 
         Proteomes must be represented as a list (proteomes) of lists (proteins)
         of lists (domains) which each carry tuples. These tuples are domain specifications
         that are derived by [Genetics][magicsoup.genetics.Genetics].
         These are indices which will be mapped to concrete values
         (molecule species, Km, Vmax, reactions, ...).
         """
-        N_d, A_d, Km_d, Vmax_d, _ = self._get_proteome_tensors(proteomes=proteomes)
+        # get proteome tensors
+        dom_types, idxs0, idxs1, idxs2, idxs3 = self._collect_proteome_idxs(
+            proteomes=proteomes
+        )
 
-        # N (c, p, d, s)
+        # identify domain types
+        # 1=catalytic, 2=transporter, 3=regulatory
+        is_catal = dom_types == 1  # (c, p, d)
+        is_trnsp = dom_types == 2  # (c, p, d)
+        is_reg = dom_types == 3  # (c, p, d)
+
+        # map indices of domain specifications to concrete values
+        # idx0 is a 2-codon index specific for every domain type (n=4096)
+        # idx1-3 are 1-codon used for the floats (n=64)
+        # some values are not defined for certain domain types
+        # setting their indices to 0 lets them map to empty values (0-vector, NaN)
+        catal_lng = (is_catal).long()
+        trnsp_lng = (is_trnsp).long()
+        reg_lng = (is_reg).long()
+        not_reg_lng = (~is_reg).long()
+
+        # idxs 0-2 are 1-codon indexes used for scalars (n=64 (- stop codons))
+        Vmaxs = self.vmax_map(idxs0 * not_reg_lng)  # float (c, p, d)
+        Kms = self.km_map(idxs1)  # float (c, p, d)
+        signs = self.sign_map(idxs2)  # float (c, p, d)
+
+        # idx3 is a 2-codon index used for vectors (n=4096 (- stop codons))
+        reacts = self.reaction_map(idxs3 * catal_lng)  # float (c, p, d, s)
+        trnspts = self.transport_map(idxs3 * trnsp_lng)  # float (c, p, d, s)
+        effectors = self.effector_map(idxs3 * reg_lng)  # float (c, p, d, s)
+
+        # Vmax are averaged over domains
+        # undefined Vmax enries are NaN and are ignored by nanmean
+        self.Vmax[cell_idxs] = Vmaxs.nanmean(dim=2).nan_to_num(0.0)
+
+        # effector vectors are summed up over domains
+        # undefined vectors are all 0s
+        self.A[cell_idxs] = torch.einsum("cpds,cpd->cpds", effectors, signs).sum(dim=2)
+
+        # Kms of regulatory domains are aggregated for effectors
+        # Kms from other domains are ignored using NaNs and nanmean
+        self.Kmr[cell_idxs] = (
+            torch.where(is_reg, Kms, torch.nan).nanmean(dim=2).nan_to_num(0.0)
+        )
+
+        # reaction stoichiometry N is derived from transporter and catalytic vectors
+        # vectors for regulatory domains or emptpy proteins are all 0s
+        N_d = torch.einsum("cpds,cpd->cpds", (reacts + trnspts), signs)
         N = N_d.sum(dim=2)
         self.N[cell_idxs] = N
 
-        # A (c, p, d, s)
-        A = A_d.sum(dim=2)
-        # reactants on the first domain must be added as effectors
-        # if their stoichiometric number became 0 during summing up
-        delta_N = N_d[:, :, 0].clamp(max=0.0) - N.clamp(max=0.0)
-        # A += -1.0 * delta_N.clamp(max=0.0)
-        self.A[cell_idxs] = A - delta_N.clamp(max=0.0)
-
-        # Km (c, p, d, s)
-        Km = Km_d.nanmean(dim=2).nan_to_num(0.0)
-        self.Km[cell_idxs] = Km
+        # N for forward and backward reactions is distinguished
+        # to not loose molecules like co-facors whose net N would become 0
+        self.Nf[cell_idxs] = torch.where(N_d < 0.0, -N_d, 0.0).sum(dim=2)
+        self.Nb[cell_idxs] = torch.where(N_d > 0.0, N_d, 0.0).sum(dim=2)
+
+        # Kms of catalytic and transporter domains are aggregated
+        # Kms from other domains are ignored using NaNs and nanmean
+        Kmn = torch.where(~is_reg, Kms, torch.nan).nanmean(dim=2).nan_to_num(0.0)
 
-        # Vmax_d (c, p, d)
-        Vmax = Vmax_d.nanmean(dim=2).nan_to_num(0.0)
-        self.Vmax[cell_idxs] = Vmax
-
-        # N (c, p, s)
+        # energies define Ke which defines Ke = Kmf/Kmb
+        # extreme energies can create Inf or 0.0, avoid them with clamp
         E = torch.einsum("cps,s->cp", N, self.mol_energies)
-        self.E[cell_idxs] = E
+        Ke = torch.exp(-E / self.abs_temp / GAS_CONSTANT).clamp(_MIN, _MAX)
+
+        # Km is sampled between a defined range
+        # exessively small Km can create numerical instability
+        # thus, sampled Km should define the smaller Km of Ke = Kmf/Kmb
+        # Ke>=1  => Kmf=Km,         Kmb=Ke*Km
+        # Ke<1   => Kmf=Km/Ke,      Kmb=Km
+        # this operation can create again Inf or 0.0, avoided with clamp
+        # this effectively limits Ke around 1e38
+        is_fwd = Ke >= 1.0
+        self.Kmf[cell_idxs] = torch.where(is_fwd, Kmn, Kmn / Ke).clamp(_MIN, _MAX)
+        self.Kmb[cell_idxs] = torch.where(is_fwd, Kmn * Ke, Kmn).clamp(_MIN, _MAX)
+
+    def unset_cell_params(self, cell_idxs: list[int]):
+        """
+        Unset cell parameters (Vmax, Km, ...) for cells with empty
+        or non-viable proteomes.
+
+        Arguments:
+            cell_idxs: Indexes of cells
+        """
+        self.N[cell_idxs] = 0.0
+        self.Nf[cell_idxs] = 0.0
+        self.Nb[cell_idxs] = 0.0
+        self.A[cell_idxs] = 0.0
+        self.Kmf[cell_idxs] = 0.0
+        self.Kmb[cell_idxs] = 0.0
+        self.Kmr[cell_idxs] = 0.0
+        self.Vmax[cell_idxs] = 0.0
 
     def integrate_signals(self, X: torch.Tensor) -> torch.Tensor:
         """
         Simulate protein work by integrating all signals.
 
         Arguments:
             X: Tensor of every signal in every cell (c, s). Must all be >= 0.0.
@@ -514,114 +636,212 @@
 
         The order of cells in `X` is the same as in `world.genomes`
         The order of signals is first all intracellular molecule species in the same order as `chemistry.molecules`,
         then again all molecule species in the same order but this time describing extracellular molecule species.
         The number of intracellular molecules comes from `world.cell_molecules` for any particular cell.
         The number of extracellular molecules comes from `world.molecule_map` from the pixel the particular cell currently lives on.
         """
-        # adjust direction
-        lKe = -self.E / self.abs_temp / GAS_CONSTANT  # (c, p)
-        lQ = self._get_ln_reaction_quotients(X=X)  # (c, p)
-        adj_N = torch.where(lQ > lKe, -1.0, 1.0)  # (c, p)
-        N_adj = torch.einsum("cps,cp->cps", self.N, adj_N)
-
-        # activations
-        a_inh = self._get_inhibitor_activity(X=X)  # (c, p)
-        a_act = self._get_activator_activity(X=X)  # (c, p)
-        a_cat = self._get_catalytic_activity(X=X, N=N_adj)  # (c, p)
-
-        # trim velocities when approaching equilibrium Q -> Ke
-        # and stop reaction if Q ~= Ke
-        # f(x) = {1.0 if x > 1.0; 0.0 if x <= 0.1; x otherwise}
-        # with x being the abs(ln(Q) - ln(Ke))
-        trim = (lQ - lKe).abs().clamp(max=1.0)  # (c, p)
-        trim[trim.abs() <= 0.1] = 0.0
-
-        # velocity and naive Xd
-        V = self.Vmax * a_cat * (1 - a_inh) * a_act * trim  # (c, p)
-        Xd = torch.einsum("cps,cp->cs", N_adj, V)  # (c, s)
-
-        # proteins can deconstruct more of a molecule than available in a cell
-        # Here, I am reducing the velocity of all proteins in a cell by the same
-        # amount to just not deconstruct more of any molecule species than
-        # available in this cell
-        # One can also reduce only the velocity of the proteins which are part
-        # of deconstructing the molecule species that is becomming the problem
-        # but these reduced protein speeds could also have a downstream effect
-        # on the construction of another molecule species, which could then
-        # create the same problem again.
-        # By reducing all proteins by the same factor, this cannot happen.
-        fact = torch.where(X + Xd < 0.0, X * 0.99 / -Xd, 1.0)  # (c, s)
-        Xd = torch.einsum("cs,c->cs", Xd, fact.amin(1))
+        is_fwd = self.Nf > 0.0
+        is_bwd = self.Nb > 0.0
+        is_inh = self.A < 0.0
+        is_act = self.A > 0.0
+        Vmax_adj = self.Vmax * self.n_comp_trim
+
+        for i in range(self.n_computations):
+            # catalytic activity
+
+            # signals are aggregated for forward and backward reaction
+            # proteins that had no involved catalytic region should not be active
+            xxf, f_prots = self._aggregate_signals(X=X, mask=is_fwd, N=self.Nf)
+            kf = xxf / self.Kmf
+            kf[~f_prots] = 0.0  # rm artifacts created by ln
+
+            xxb, b_prots = self._aggregate_signals(X=X, mask=is_bwd, N=self.Nb)
+            kb = xxb / self.Kmb
+            kb[~b_prots] = 0.0  # rm artifacts created by ln
+
+            # the correct formula yields 2 * (ks - kp) / (1 + ks + kp)
+            # but then there can be a maximum activity of 200%
+            # while regulatory regions can only go up to 100%
+            # thus (ks - kp) / (1 + ks + kp)
+            a_cat = (kf - kb) / (1 + kf + kb)  # (c, p)
+
+            # NaNs could have been propagated so far by stray NaN Kms
+            # they should represent 0 velocity
+            a_cat = a_cat.nan_to_num(0.0)
+
+            # inhibitor activity
+            xxi, i_prots = self._aggregate_signals(X=X, mask=is_inh, N=-self.A)
+            a_inh = xxi / (xxi + self.Kmr)
+            a_inh[~i_prots] = 0.0  # proteins without inhibitor should be active
+
+            # activator activity
+            xxa, a_prots = self._aggregate_signals(X=X, mask=is_act, N=self.A)
+            a_act = xxa / (xxa + self.Kmr)
+            a_act[~a_prots] = 1.0  # proteins without activator should be active
+
+            # velocity from activities
+            # as well as trimming factor of n_computations
+            V = Vmax_adj * a_cat * (1 - a_inh) * a_act * self.alpha**i  # (c, p)
+
+            # Kms can be close to Inf, they can create Infs
+            # thus result velocity should be clamped again
+            V = V.clamp(max=_MAX)
+
+            # naive Xd
+            Xd = torch.einsum("cps,cp->cs", self.N, V)  # (c, s)
+
+            # proteins can deconstruct more of a molecule than available in a cell
+            # but I can't just clip X at 0 because then reactions would not adhere
+            # to their stoichiometry anymore
+            # instead I need to reduce protein velocity
+            # However, a cell's Xd is the sum of all its protein's activities
+            # if I reduce the velocity of 1 protein, it could create a new
+            # below-zero situation for another one
+            # One would have to repeat this action until all conflicts are satisfied
+            # Here, I am instead reducing all the cell's proteins by the same factor
+            # that way these secondary below-zero situations cannot appear
+            trim_to_zero = torch.where(X + Xd < 0.0, (X - _EPS) / -Xd, 1.0)  # (c, s)
+            Xd = torch.einsum("cs,c->cs", Xd, trim_to_zero.amin(1))
+
+            # should not be necessary but floating point precision
+            # can still create very small negative values (<1e-7)
+            # these are so small that they should not matter in the overall simulation
+            X = (X + Xd).clamp(min=0.0)
+
+        # NaNs can be created when overflow creates Infs (most likely in aggregate_signals)
+        # with kinetics default values I have not been able to achieve this (>100 testruns)
+        # however non-default values (e.g. large Vmax) might achieve that
+        # once a 1 NaN is generated, it will spread over the whole simulation
+        # this is a last effort in avoiding that
+        X[X.isnan()] = 0.0
 
-        return (X + Xd).clamp(min=0.0)
+        return X
 
     def copy_cell_params(self, from_idxs: list[int], to_idxs: list[int]):
         """
         Copy paremeters from a list of cells to another list of cells
 
         Arguments:
             from_idxs: List of cell indexes to copy from
             to_idxs: List of cell indexes to copy to
 
         `from_idxs` and `to_idxs` must have the same length.
         They refer to the same cell indexes as in `world.genomes`.
         """
-        self.Km[to_idxs] = self.Km[from_idxs]
+        self.Kmf[to_idxs] = self.Kmf[from_idxs]
+        self.Kmb[to_idxs] = self.Kmb[from_idxs]
+        self.Kmr[to_idxs] = self.Kmr[from_idxs]
         self.Vmax[to_idxs] = self.Vmax[from_idxs]
-        self.E[to_idxs] = self.E[from_idxs]
         self.N[to_idxs] = self.N[from_idxs]
+        self.Nf[to_idxs] = self.Nf[from_idxs]
+        self.Nb[to_idxs] = self.Nb[from_idxs]
         self.A[to_idxs] = self.A[from_idxs]
 
     def remove_cell_params(self, keep: torch.Tensor):
         """
         Remove cells from cell params
 
         Arguments:
             keep: Bool tensor (c,) which is true for every cell that should not be removed
                 and false for every cell that should be removed.
 
         `keep` must have the same length as `world.genomes`.
         The indexes on `keep` reflect the indexes in `world.genomes`.
         """
-        self.Km = self.Km[keep]
+        self.Kmf = self.Kmf[keep]
+        self.Kmb = self.Kmb[keep]
+        self.Kmr = self.Kmr[keep]
         self.Vmax = self.Vmax[keep]
-        self.E = self.E[keep]
         self.N = self.N[keep]
+        self.Nf = self.Nf[keep]
+        self.Nb = self.Nb[keep]
         self.A = self.A[keep]
 
     def increase_max_cells(self, by_n: int):
         """
         Increase the cell dimension of all cell parameters
 
         Arguments:
             by_n: By how many rows to increase the cell dimension
         """
-        self.Km = self._expand_c(t=self.Km, n=by_n)
+        self.Kmf = self._expand_c(t=self.Kmf, n=by_n)
+        self.Kmb = self._expand_c(t=self.Kmb, n=by_n)
+        self.Kmr = self._expand_c(t=self.Kmr, n=by_n)
         self.Vmax = self._expand_c(t=self.Vmax, n=by_n)
-        self.E = self._expand_c(t=self.E, n=by_n)
         self.N = self._expand_c(t=self.N, n=by_n)
+        self.Nf = self._expand_c(t=self.Nf, n=by_n)
+        self.Nb = self._expand_c(t=self.Nb, n=by_n)
         self.A = self._expand_c(t=self.A, n=by_n)
 
     def increase_max_proteins(self, max_n: int):
         """
         Increase the protein dimension of all cell parameters
 
         Arguments:
             max_n: The maximum number of rows required in the protein dimension
         """
-        n_prots = int(self.Km.shape[1])
+        n_prots = int(self.N.size(1))
         if max_n > n_prots:
             by_n = max_n - n_prots
-            self.Km = self._expand_p(t=self.Km, n=by_n)
+            self.Kmf = self._expand_p(t=self.Kmf, n=by_n)
+            self.Kmb = self._expand_p(t=self.Kmb, n=by_n)
+            self.Kmr = self._expand_p(t=self.Kmr, n=by_n)
             self.Vmax = self._expand_p(t=self.Vmax, n=by_n)
-            self.E = self._expand_p(t=self.E, n=by_n)
             self.N = self._expand_p(t=self.N, n=by_n)
+            self.Nf = self._expand_p(t=self.Nf, n=by_n)
+            self.Nb = self._expand_p(t=self.Nb, n=by_n)
             self.A = self._expand_p(t=self.A, n=by_n)
 
+    def _aggregate_signals(
+        self, X: torch.Tensor, mask: torch.Tensor, N: torch.Tensor
+    ) -> tuple[torch.Tensor, torch.Tensor]:
+        # consider:
+        # - a) some proteins are not involved at all (their Ns are all 0)
+        # - b) some are involved but the signal 0 (required X is 0)
+        # - c) there can be multiple signals (Xs must be multiplied)
+        # - d) each signal has a stoichiometric number (X must be raised)
+
+        # signals are prepared as c,p,s
+        # all non-involved signals (or involved but 0)
+        # are set to NaN so that it is possible
+        # to log them later without need of EPS addition
+        x = torch.einsum("cps,cs->cps", mask, X)  # (c, p, s)
+        x[x == 0.0] = torch.nan
+
+        # stoichiometric numbers are prepared
+        # all non-involved fields are 0
+        n = mask * N  # (c, p, s)
+
+        # proteins which have at least 1 non-zero stoichiometric number
+        involved_prots = n.sum(2) != 0.0
+
+        # proteins which have all zero signals or which
+        # don't have at least 1 non-zero stoichiometric number
+        zero_prots = x.isnan().all(2)
+
+        # (1) raise each signal to its stoichiometric number
+        # then (2) multiply all over protein
+        # while ignoring non-involved signals
+        # (1) is done in log-space, all NaNs stay NaN, then
+        # (2) can be done as nansum (treats NaNs as 0) so
+        # if a protein had only 0 stoichiometric numbers or
+        # all involved signals were 0 it will be 0
+        # after exp it will become 1
+        xx = torch.exp((torch.log(x) * n).nansum(2))
+
+        # proteins that actually had a stoichiometric number
+        # but its signal was 0 became 1, but they should be 0
+        # I have to identify them with the masks calculated earlier
+        # because in xx a signal could theoretically become 1
+        # from a legitimate stoichiometric number and non-zero signal
+        xx[involved_prots & zero_prots] = 0.0
+
+        return xx, involved_prots
+
     def _get_proteome_tensors(
         self, proteomes: list[list[list[tuple[int, int, int, int, int]]]]
     ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
         # separate domain specifications into different tensors
         dom_types, idxs0, idxs1, idxs2, idxs3 = self._collect_proteome_idxs(
             proteomes=proteomes
         )
@@ -653,30 +873,24 @@
         N_t = torch.einsum("cpds,cpd->cpds", trnspts, trnsp_mask)
         N_d = torch.einsum("cpds,cpd->cpds", (N_r + N_t), signs)
 
         # A (c, p, d, s)
         A_r = torch.einsum("cpds,cpd->cpds", effectors, reg_mask)
         A_d = torch.einsum("cpds,cpd->cpds", A_r, signs)
 
-        # Km (c, p, d, s)
-        is_lft = (A_d != 0.0) | (N_d < 0.0)
-        is_rgt = N_d > 0.0
-        Km_l = torch.einsum("cpds,cpd->cpds", is_lft.float(), Kms)
-        Km_r = torch.einsum("cpds,cpd->cpds", is_rgt.float(), 1 / Kms)
-        Km_d = Km_l + Km_r
-        Km_d[~(is_lft | is_rgt)] = torch.nan
+        # Km (c, p, d)
 
         # Vmax_d (c, p, d)
         Vmax_d = Vmaxs * catal_trnsp_mask
 
-        return N_d, A_d, Km_d, Vmax_d, dom_types
+        return N_d, A_d, Kms, Vmax_d, dom_types
 
     def _collect_proteome_idxs(
         self, proteomes: list[list[list[tuple[int, int, int, int, int]]]]
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor,]:
+    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
         n_prots = self.N.size(1)
         n_doms = max(len(dd) for d in proteomes for dd in d)
         empty_seq = [0] * n_doms
 
         c_dts = []
         c_idxs0 = []
         c_idxs1 = []
@@ -717,61 +931,22 @@
         dom_types = self._tensor_from(c_dts)  # long (c, p, d)
         idxs0 = self._tensor_from(c_idxs0)  # long (c, p, d)
         idxs1 = self._tensor_from(c_idxs1)  # long (c, p, d)
         idxs2 = self._tensor_from(c_idxs2)  # long (c, p, d)
         idxs3 = self._tensor_from(c_idxs3)  # long (c, p, d)
         return dom_types, idxs0, idxs1, idxs2, idxs3
 
-    def _get_ln_reaction_quotients(self, X: torch.Tensor) -> torch.Tensor:
-        # substrates
-        smask = self.N < 0.0
-        sub_X = torch.einsum("cps,cs->cps", smask, X)  # (c, p, s)
-        sub_N = smask * -self.N  # (c, p, s)
-
-        # products
-        pmask = self.N > 0.0
-        pro_X = torch.einsum("cps,cs->cps", pmask, X)  # (c, p, s)
-        pro_N = pmask * self.N  # (c, p, s)
-
-        # quotients
-        prods = (torch.log(pro_X + _EPS) * pro_N).sum(2)  # (c, p)
-        subs = (torch.log(sub_X + _EPS) * sub_N).sum(2)  # (c, p)
-        return prods - subs  # (c, p)
-
-    def _get_catalytic_activity(self, X: torch.Tensor, N: torch.Tensor) -> torch.Tensor:
-        mask = N < 0.0
-        sub_X = torch.einsum("cps,cs->cps", mask, X)  # (c, p, s)
-        sub_N = mask * -N  # (c, p, s)
-        lact = torch.log(sub_X + _EPS) - torch.log(self.Km + sub_X + _EPS)  # (c, p, s)
-        return (lact * sub_N).sum(2).exp()
-
-    def _get_inhibitor_activity(self, X: torch.Tensor) -> torch.Tensor:
-        inh_N = (-self.A).clamp(0)  # (c, p, s)
-        inh_X = torch.einsum("cps,cs->cps", inh_N, X)  # (c, p, s)
-        lact = torch.log(inh_X + _EPS) - torch.log(self.Km + inh_X + _EPS)  # (c, p, s)
-        V = (lact * inh_N).sum(2).exp()  # (c, p)
-        return torch.where(torch.any(self.A < 0.0, dim=2), V, 0.0)  # (c, p)
-
-    def _get_activator_activity(self, X: torch.Tensor) -> torch.Tensor:
-        act_N = self.A.clamp(0)  # (c, p, s)
-        act_X = torch.einsum("cps,cs->cps", act_N, X)  # (c, p, s)
-        lact = torch.log(act_X + _EPS) - torch.log(self.Km + act_X + _EPS)  # (c, p, s)
-        V = (lact * act_N).sum(2).exp()  # (c, p)
-        return torch.where(torch.any(self.A > 0.0, dim=2), V, 1.0)  # (c, p)
-
     def _expand_c(self, t: torch.Tensor, n: int) -> torch.Tensor:
         size = t.size()
         zeros = self._tensor(n, *size[1:])
         return torch.cat([t, zeros], dim=0)
 
     def _expand_p(self, t: torch.Tensor, n: int) -> torch.Tensor:
         size = t.size()
         zeros = self._tensor(size[0], n, *size[2:])
         return torch.cat([t, zeros], dim=1)
 
-    def _tensor(self, *args, d: float | None = None) -> torch.Tensor:
-        if d is None:
-            return torch.zeros(*args).to(self.device)
-        return torch.full(tuple(args), d).to(self.device)
+    def _tensor(self, *args) -> torch.Tensor:
+        return torch.zeros(*args).to(self.device)
 
     def _tensor_from(self, d: Any) -> torch.Tensor:
         return torch.tensor(d).to(self.device)
```

### Comparing `magicsoup-0.3.9/src/magicsoup/mutations.py` & `magicsoup-0.4.0/src/magicsoup/mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/src/magicsoup/util.py` & `magicsoup-0.4.0/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/src/magicsoup/world.py` & `magicsoup-0.4.0/src/magicsoup/world.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import pickle
 from pathlib import Path
 import torch
 from magicsoup.constants import CODON_SIZE
 from magicsoup.util import moore_nghbrhd, round_down, random_genome, randstr
 from magicsoup.containers import (
     Cell,
-    Molecule,
     Chemistry,
     ProteinFact,
     CatalyticDomainFact,
     TransporterDomainFact,
     RegulatoryDomainFact,
 )
 from magicsoup.kinetics import Kinetics
@@ -78,15 +77,15 @@
             Dimension 0 describes the molecule species. They are in the same order as `chemistry.molecules`.
             Dimension 1 represents x, dimension 2 y.
             So, `world.molecule_map[0, 1, 2]` is number of molecules of the 0th molecule species on pixel 1, 2.
         cell_molecules: Float 2D tensor describing the number of molecules (in mol) for each molecule species in each cell.
             Dimension 0 is the cell index. It is the same as in `world.genomes` and the same as on a cell object (`cell.idx`).
             Dimension 1 describes the molecule species. They are in the same order as `chemistry.molecules`.
             So, `world.cell_molecules[0, 1]` represents how many mol of the 1st molecule species the 0th cell contains.
-        cell_survival: Integer 1D tensor describing how many time steps each cell survived.
+        cell_lifetimes: Integer 1D tensor describing how many time steps each cell survived since the last division.
             This tensor is for monitoring and doesn't have any other effect.
             Cells are in the same as in `world.genomes` and the same as on a cell object (`cell.idx`).
         cell_divisions: Integer 1D tensor describing how many times each cell's ancestors divided.
             This tensor is for monitoring and doesn't have any other effect.
             Cells are in the same order as in `world.genomes` and the same as on a cell object (`cell.idx`).
 
     Methods for advancing the simulation and to use during a simulation:
@@ -94,15 +93,15 @@
     - [add_cells()][magicsoup.world.World.add_cells] add new cells and place them randomly on the map
     - [divide_cells()][magicsoup.world.World.divide_cells] replicate existing cells
     - [update_cells()][magicsoup.world.World.update_cells] update existing cells if their genome has changed
     - [kill_cells()][magicsoup.world.World.kill_cells] kill existing cells
     - [move_cells()][magicsoup.world.World.move_cells] move existing cells to a random position in their Moore's neighborhood
     - [diffuse_molecules()][magicsoup.world.World.diffuse_molecules] let molecules diffuse and permeate by one time step
     - [degrade_molecules()][magicsoup.world.World.degrade_molecules] let molecules degrade by one time step
-    - [increment_cell_survival()][magicsoup.world.World.increment_cell_survival] increment `world.cell_survival` by 1
+    - [increment_cell_lifetimes()][magicsoup.world.World.increment_cell_lifetimes] increment `world.cell_lifetimes` by 1
     - [enzymatic_activity()][magicsoup.world.World.enzymatic_activity] let cell proteins work for one time step
 
     If you want to get a cell with all information about its contents and its current environment use [get_cell()][magicsoup.world.World.get_cell].
     During the simulation you should however work directly with the tensors mentioned above for performance reasons.
 
     Furthermore, there are methods for saving and loading a simulation.
     For any new simulation use [save()][magicsoup.world.World.save] once to save the whole world object (with chemistry, genetics, kinetics)
@@ -171,36 +170,21 @@
         }
 
         self.n_cells = 0
         self.genomes: list[str] = []
         self.labels: list[str] = []
         self.cell_map: torch.Tensor = torch.zeros(map_size, map_size).to(device).bool()
         self.cell_positions: torch.Tensor = torch.zeros(0, 2).to(device).long()
-        self.cell_survival: torch.Tensor = torch.zeros(0).to(device).int()
+        self.cell_lifetimes: torch.Tensor = torch.zeros(0).to(device).int()
         self.cell_divisions: torch.Tensor = torch.zeros(0).to(device).int()
         self.cell_molecules: torch.Tensor = torch.zeros(0, self.n_molecules).to(device)
         self.molecule_map: torch.Tensor = self._get_molecule_map(
             n=self.n_molecules, size=map_size, init=mol_map_init
         )
 
-    def _get_catal_2_idxs(
-        self,
-    ) -> dict[tuple[tuple[Molecule, ...], tuple[Molecule, ...]], list[int]]:
-        react_map = {}
-        for subs, prods in self.chemistry.reactions:
-            t = torch.zeros(self.n_molecules * 2)
-            for sub in subs:
-                t[self.kinetics.mol_2_mi[sub]] -= 1
-            for prod in prods:
-                t[self.kinetics.mol_2_mi[prod]] += 1
-            M = self.kinetics.reaction_map.M
-            idxs = torch.argwhere((M == t).all(dim=1)).flatten().tolist()
-            react_map[(tuple(subs), tuple(prods))] = idxs
-        return react_map
-
     def get_cell(
         self,
         by_idx: int | None = None,
         by_position: tuple[int, int] | None = None,
     ) -> Cell:
         """
         Get a cell with information about its current environment.
@@ -226,29 +210,79 @@
             mask = (self.cell_positions == pos).all(dim=1)
             idxs = torch.argwhere(mask).flatten().tolist()
             if len(idxs) == 0:
                 raise ValueError(f"Cell at {by_position} not found")
             idx = idxs[0]
 
         genome = self.genomes[idx]
-        (cdss,) = self.genetics.translate_genomes(genomes=[genome])
         pos = self.cell_positions[idx]
+        (cdss,) = self.genetics.translate_genomes(genomes=[genome])
+        proteome = self.kinetics.get_proteome(proteome=cdss) if len(cdss) > 0 else []
 
         return Cell(
             idx=idx,
             genome=genome,
-            proteome=self.kinetics.get_proteome(proteome=cdss),
+            proteome=proteome,
             position=tuple(pos.tolist()),  # type: ignore
             int_molecules=self.cell_molecules[idx, :],
             ext_molecules=self.molecule_map[:, pos[0], pos[1]],
             label=self.labels[idx],
-            n_survived_steps=int(self.cell_survival[idx].item()),
+            n_steps_alive=int(self.cell_lifetimes[idx].item()),
             n_divisions=int(self.cell_divisions[idx].item()),
         )
 
+    def get_neighbors(
+        self, cell_idxs: list[int], nghbr_idxs: list[int] | None = None
+    ) -> list[tuple[int, int]]:
+        """
+        For each cell from a list of cell indexes find all other cells that
+        are in the Moore's neighborhood of this cell.
+
+        Parameters:
+            cell_idxs: Indexes of cells for which to find neighbors
+            nghbr_idxs: Optional list of cells regarded as neighbors.
+                If `None` (default) each cell in `cell_idxs` can form a pair
+                with any other neighboring cell. With `nghbr_idxs` provided
+                each cell in `cell_idxs` can only form a pair with a neighboring
+                cell that is in `nghbr_idxs`.
+
+        Returns:
+            List of tuples of cell indexes for each unique neighboring pair.
+        """
+
+        if len(cell_idxs) == 0:
+            return []
+
+        # rm duplicates to avoid unnecessary compute
+        cell_idxs = list(set(cell_idxs))
+
+        if nghbr_idxs is None:
+            nghbr_map = self.cell_map
+        else:
+            nghbr_idxs = list(set(nghbr_idxs))
+            nghbr_map = torch.zeros_like(self.cell_map).bool()
+            pos = self.cell_positions[nghbr_idxs]
+            nghbr_map[pos[:, 0], pos[:, 1]] = True
+
+        nghbrs: list[tuple[int, int]] = []
+        for c_idx in cell_idxs:
+            c_pos = self.cell_positions[c_idx]
+            nghbrhd = self._nghbrhd_map[tuple(c_pos.tolist())]  # type: ignore
+            pxls = nghbrhd[nghbr_map[nghbrhd[:, 0], nghbrhd[:, 1]]]
+            n = pxls.size(0)
+
+            if n == 0:
+                continue
+
+            idx_ts = [(self.cell_positions == d).all(dim=1).argwhere() for d in pxls]
+            n_idxs: list[int] = torch.cat(idx_ts).flatten().tolist()
+            nghbrs.extend(tuple(sorted([c_idx, d])) for d in n_idxs)  # type:ignore
+
+        return list(set(nghbrs))
+
     def generate_genome(self, proteome: list[ProteinFact], size: int = 500) -> str:
         """
         Generate a random genome that encodes a desired proteome
 
         Arguments:
             proteome: list of [ProteinFactories][magicsoup.containers.ProteinFact] that describe each protein
             size: total length of the resulting genome (in nucleotides/base pairs)
@@ -342,87 +376,91 @@
             parts.append(d_pads.pop())
             parts.append(random.choice(stop_codons))
         parts.append(p_pads.pop())
         parts.append(tail)
 
         return "".join(parts)
 
-    def add_cells(self, genomes: list[str]) -> list[int]:
+    def add_cells(self, genomes: list[str], batch_size: int = 1000) -> list[int]:
         """
         Create new cells and place them randomly on the map.
         All lists and tensors that reference cells will be updated.
 
         Parameters:
             genomes: List of genomes of the newly added cells
+            batch_size: Batch size used for updating cell kinetics. Reduce this number
+                to reduce memory required during update.
 
         Returns:
             The indexes of successfully added cells.
 
         Each cell will be placed randomly on the map and receive half the molecules of the pixel where it was added.
         If there are less pixels left on the cell map than cells you want to add,
         only the remaining pixels will be filled with new cells.
         Each cell will also receive a random label.
         """
-        genomes = [d for d in genomes if len(d) > 0]
         n_new_cells = len(genomes)
         if n_new_cells == 0:
             return []
 
         free_pos = self._find_free_random_positions(n_cells=n_new_cells)
         n_avail_pos = free_pos.size(0)
         if n_avail_pos == 0:
             return []
 
         if n_avail_pos < n_new_cells:
             n_new_cells = n_avail_pos
             random.shuffle(genomes)
             genomes = genomes[:n_new_cells]
 
-        proteomes = self.genetics.translate_genomes(genomes=genomes)
-
-        new_genomes = []
-        new_proteomes = []
-        new_labels = []
-        for proteome, genome in zip(proteomes, genomes):
-            if len(proteome) > 0:
-                new_genomes.append(genome)
-                new_proteomes.append(proteome)
-                new_labels.append(randstr(n=12))
-
-        n_new_cells = len(new_genomes)
-        if n_new_cells == 0:
-            return []
-
         new_pos = free_pos[:n_new_cells]
         new_idxs = list(range(self.n_cells, self.n_cells + n_new_cells))
         self.n_cells += n_new_cells
-        self.genomes.extend(new_genomes)
-        self.labels.extend(new_labels)
+        self.genomes.extend(genomes)
+        self.labels.extend(randstr(n=12) for _ in range(n_new_cells))
 
-        self.cell_survival = self._expand_c(t=self.cell_survival, n=n_new_cells)
+        self.cell_lifetimes = self._expand_c(t=self.cell_lifetimes, n=n_new_cells)
         self.cell_positions = self._expand_c(t=self.cell_positions, n=n_new_cells)
         self.cell_divisions = self._expand_c(t=self.cell_divisions, n=n_new_cells)
         self.cell_molecules = self._expand_c(t=self.cell_molecules, n=n_new_cells)
-
-        n_max_prots = max(len(d) for d in new_proteomes)
-        self.kinetics.increase_max_proteins(max_n=n_max_prots)
         self.kinetics.increase_max_cells(by_n=n_new_cells)
-        self.kinetics.set_cell_params(cell_idxs=new_idxs, proteomes=new_proteomes)
 
         # occupy positions
         xs = new_pos[:, 0]
         ys = new_pos[:, 1]
         self.cell_map[xs, ys] = True
         self.cell_positions[new_idxs] = new_pos
 
         # cell is picking up half the molecules of the pxl it is born on
         pickup = self.molecule_map[:, xs, ys] * 0.5
         self.cell_molecules[new_idxs, :] += pickup.T
         self.molecule_map[:, xs, ys] -= pickup
 
+        proteomes = self.genetics.translate_genomes(genomes=genomes)
+
+        set_proteomes = []
+        set_idxs = []
+        for proteome, idx in zip(proteomes, new_idxs):
+            if len(proteome) > 0:
+                set_proteomes.append(proteome)
+                set_idxs.append(idx)
+
+        n_new_proteomes = len(set_proteomes)
+        if n_new_proteomes == 0:
+            return []
+
+        n_max_prots = max(len(d) for d in set_proteomes)
+        self.kinetics.increase_max_proteins(max_n=n_max_prots)
+
+        for a in range(0, n_new_proteomes, batch_size):
+            b = a + batch_size
+            self.kinetics.set_cell_params(
+                cell_idxs=set_idxs[a:b], proteomes=set_proteomes[a:b]
+            )
+
         return new_idxs
 
     def divide_cells(self, cell_idxs: list[int]) -> list[tuple[int, int]]:
         """
         Bring cells to divide.
         All lists and tensors that reference cells will be updated.
 
@@ -447,27 +485,30 @@
         Of the list of descendant index tuples,
         the first descendant in each tuple is the cell that still lives on the same pixel.
         The second descendant in that tuple is the cell that was newly created.
         """
         if len(cell_idxs) == 0:
             return []
 
+        # duplicates could lead to unexpected results
+        cell_idxs = list(set(cell_idxs))
+
         (
             parent_idxs,
             child_idxs,
             child_pos,
         ) = self._divide_cells_as_possible(parent_idxs=cell_idxs)
 
         n_new_cells = len(child_idxs)
         if n_new_cells == 0:
             return []
 
         self.n_cells += n_new_cells
 
-        self.cell_survival = self._expand_c(t=self.cell_survival, n=n_new_cells)
+        self.cell_lifetimes = self._expand_c(t=self.cell_lifetimes, n=n_new_cells)
         self.cell_positions = self._expand_c(t=self.cell_positions, n=n_new_cells)
         self.cell_divisions = self._expand_c(t=self.cell_divisions, n=n_new_cells)
         self.cell_molecules = self._expand_c(t=self.cell_molecules, n=n_new_cells)
         self.kinetics.increase_max_cells(by_n=n_new_cells)
         self.kinetics.copy_cell_params(from_idxs=parent_idxs, to_idxs=child_idxs)
 
         # position new cells
@@ -476,59 +517,60 @@
 
         # cells share molecules and increment cell divisions
         descendant_idxs = parent_idxs + child_idxs
         self.cell_molecules[child_idxs] = self.cell_molecules[parent_idxs]
         self.cell_molecules[descendant_idxs] *= 0.5
         self.cell_divisions[child_idxs] = self.cell_divisions[parent_idxs]
         self.cell_divisions[descendant_idxs] += 1
-        self.cell_survival[descendant_idxs] = 0
+        self.cell_lifetimes[descendant_idxs] = 0
 
         return list(zip(parent_idxs, child_idxs))
 
-    def update_cells(self, genome_idx_pairs: list[tuple[str, int]]):
+    def update_cells(
+        self, genome_idx_pairs: list[tuple[str, int]], batch_size: int = 1000
+    ):
         """
         Update existing cells with new genomes.
 
         Parameters:
             genome_idx_pairs: List of tuples of genomes and cell indexes
+            batch_size: Batch size used for updating cell kinetics. Reduce this number
+                to reduce memory required during update.
 
         The indexes refer to the index of each cell that is changed.
         The genomes refer to the genome of each cell that is changed.
         """
         if len(genome_idx_pairs) == 0:
             return
 
-        kill_idxs = []
-        transl_idxs = []
-        transl_genomes = []
-        for genome, idx in genome_idx_pairs:
-            if len(genome) > 0:
-                transl_genomes.append(genome)
-                transl_idxs.append(idx)
-            else:
-                kill_idxs.append(idx)
-
-        proteomes = self.genetics.translate_genomes(genomes=transl_genomes)
+        genomes = [d[0] for d in genome_idx_pairs]
+        proteomes = self.genetics.translate_genomes(genomes=genomes)
 
-        set_idxs = []
-        set_proteomes = []
-        for proteome, idx, genome in zip(proteomes, transl_idxs, transl_genomes):
+        set_idxs: list[int] = []
+        unset_idxs: list[int] = []
+        set_proteomes: list[list[list[tuple[int, int, int, int, int]]]] = []
+        for (genome, idx), proteome in zip(genome_idx_pairs, proteomes):
+            self.genomes[idx] = genome
             if len(proteome) > 0:
-                set_proteomes.append(proteome)
                 set_idxs.append(idx)
-                self.genomes[idx] = genome
+                set_proteomes.append(proteome)
             else:
-                kill_idxs.append(idx)
+                unset_idxs.append(idx)
 
-        if len(set_proteomes) > 0:
+        self.kinetics.unset_cell_params(cell_idxs=unset_idxs)
+
+        n_set_proteomes = len(set_proteomes)
+        if n_set_proteomes > 0:
             max_prots = max(len(d) for d in set_proteomes)
             self.kinetics.increase_max_proteins(max_n=max_prots)
-            self.kinetics.set_cell_params(cell_idxs=set_idxs, proteomes=set_proteomes)
-
-        self.kill_cells(cell_idxs=kill_idxs)
+            for a in range(0, n_set_proteomes, batch_size):
+                b = a + batch_size
+                self.kinetics.set_cell_params(
+                    cell_idxs=set_idxs[a:b], proteomes=set_proteomes[a:b]
+                )
 
     def kill_cells(self, cell_idxs: list[int]):
         """
         Remove existing cells.
         All lists and tensors referencing cells will be updated.
 
         Parameters:
@@ -537,54 +579,57 @@
         Cells that are killed dump their molecule contents onto the pixel they used to live on.
 
         Cells will be removed from all lists and tensors that reference cells.
         Thus, after killing cells the index of some living cells will be updated.
         E.g. if there are 10 cells and you kill the cell with index 8 (the 9th cell),
         the cell that used to have index 9 (10th cell) will now have index 9.
         """
-        n_killed_cells = len(cell_idxs)
-        if n_killed_cells == 0:
+        if len(cell_idxs) == 0:
             return
 
-        # TODO: do list(set(cell_idxs))?
-        #       because further down .pop would fail if duplicates
+        # duplicates could raise error later
+        cell_idxs = list(set(cell_idxs))
+
         xs = self.cell_positions[cell_idxs, 0]
         ys = self.cell_positions[cell_idxs, 1]
         self.cell_map[xs, ys] = False
 
         spillout = self.cell_molecules[cell_idxs, :]
         self.molecule_map[:, xs, ys] += spillout.T
 
-        n_cells = self.cell_survival.size(0)
+        n_cells = self.cell_lifetimes.size(0)
         keep = torch.ones(n_cells, dtype=torch.bool).to(self.device)
         keep[cell_idxs] = False
-        self.cell_survival = self.cell_survival[keep]
+        self.cell_lifetimes = self.cell_lifetimes[keep]
         self.cell_positions = self.cell_positions[keep]
         self.cell_divisions = self.cell_divisions[keep]
         self.cell_molecules = self.cell_molecules[keep]
         self.kinetics.remove_cell_params(keep=keep)
 
         for idx in sorted(cell_idxs, reverse=True):
             self.genomes.pop(idx)
             self.labels.pop(idx)
 
-        self.n_cells -= n_killed_cells
+        self.n_cells -= len(cell_idxs)
 
     def move_cells(self, cell_idxs: list[int]):
         """
         Move cells to a random position in their Moore's neighborhood.
         If every pixel in the cells' Moore neighborhood is taken the cell will not be moved.
         `world.cell_map` will be updated.
 
         Parameters:
             cell_idxs: Indexes of cells that should be moved
         """
         if len(cell_idxs) == 0:
             return
 
+        # duplicates could lead to unexpected results
+        cell_idxs = list(set(cell_idxs))
+
         for cell_idx in cell_idxs:
             old_pos = self.cell_positions[cell_idx]
             nghbrhd = self._nghbrhd_map[tuple(old_pos.tolist())]  # type: ignore
             pxls = nghbrhd[~self.cell_map[nghbrhd[:, 0], nghbrhd[:, 1]]]
             n = pxls.size(0)
 
             if n == 0:
@@ -603,23 +648,25 @@
         Parameters:
             cell_idxs: Indexes of cells that should be moved
 
         Cells are removed from their current pixels on the cell map
         and repositioned randomly on any free pixel on the cell map.
         Only cell positions change (_e.g._ genomes, proteomes, cell molecules, cell indexes stay the same).
         """
-        n_cells = len(cell_idxs)
-        if n_cells == 0:
+        if len(cell_idxs) == 0:
             return
 
+        # duplicates could lead to unexpected results
+        cell_idxs = list(set(cell_idxs))
+
         old_xs = self.cell_positions[cell_idxs, 0]
         old_ys = self.cell_positions[cell_idxs, 1]
         self.cell_map[old_xs, old_ys] = False
 
-        new_pos = self._find_free_random_positions(n_cells=n_cells)
+        new_pos = self._find_free_random_positions(n_cells=len(cell_idxs))
         new_xs = new_pos[:, 0]
         new_ys = new_pos[:, 1]
 
         self.cell_map[new_xs, new_ys] = True
         self.cell_positions[cell_idxs] = new_pos
 
     def enzymatic_activity(self):
@@ -687,20 +734,20 @@
         How quickly each molecule species degrades depends on its half life
         which is defined on the `Molecule` object of that species.
         """
         for mol_i, degrad in enumerate(self._mol_degrads):
             self.molecule_map[mol_i] *= degrad
             self.cell_molecules[:, mol_i] *= degrad
 
-    def increment_cell_survival(self):
+    def increment_cell_lifetimes(self):
         """
-        Increment `world.cell_survival` by 1.
+        Increment `world.cell_lifetimes` by 1.
         This is for monitoring and doesn't have any other effect.
         """
-        self.cell_survival += 1
+        self.cell_lifetimes += 1
 
     def save(self, rundir: Path, name: str = "world.pkl"):
         """
         Write whole world object to pickle file
 
         Parameters:
             rundir: Directory of the pickle file
@@ -764,80 +811,82 @@
         To restore a whole `world` object you need to save it at least once with [save()][magicsoup.world.World.save].
         Then, `world.save_state()` can be used to save different states of that world object.
         """
         statedir.mkdir(parents=True, exist_ok=True)
         torch.save(self.cell_molecules, statedir / "cell_molecules.pt")
         torch.save(self.cell_map, statedir / "cell_map.pt")
         torch.save(self.molecule_map, statedir / "molecule_map.pt")
-        torch.save(self.cell_survival, statedir / "cell_survival.pt")
+        torch.save(self.cell_lifetimes, statedir / "cell_lifetimes.pt")
         torch.save(self.cell_positions, statedir / "cell_positions.pt")
         torch.save(self.cell_divisions, statedir / "cell_divisions.pt")
 
         lines: list[str] = []
         for idx, (genome, label) in enumerate(zip(self.genomes, self.labels)):
             lines.append(f">{idx} {label}\n{genome}")
 
         with open(statedir / "cells.fasta", "w", encoding="utf-8") as fh:
             fh.write("\n".join(lines))
 
     def load_state(
-        self,
-        statedir: Path,
-        ignore_cell_params: bool = False,
+        self, statedir: Path, ignore_cell_params: bool = False, batch_size: int = 1000
     ):
         """
         Load a saved world state.
         The state had to be saved with [save_state()][magicsoup.world.World.save_state] previously.
 
         Parameters:
             statedir: Directory that contains all files of that state
             ignore_cell_params: Whether to not update cell parameters as well.
                 If you are only interested in the cells' genomes and molecules
                 you can set this to `True` to make loading a lot faster.
+            batch_size: Batch size used for updating cell kinetics. Reduce this number
+                to reduce memory required during update. This is irrelevant with
+                `ignore_cell_params=True`.
         """
-
         self.cell_molecules = torch.load(
             statedir / "cell_molecules.pt", map_location=self.device
         )
         self.cell_map = torch.load(
             statedir / "cell_map.pt", map_location=self.device
         ).bool()
         self.molecule_map = torch.load(
             statedir / "molecule_map.pt", map_location=self.device
         )
-        self.cell_survival = torch.load(
-            statedir / "cell_survival.pt", map_location=self.device
+        self.cell_lifetimes = torch.load(
+            statedir / "cell_lifetimes.pt", map_location=self.device
         ).int()
         self.cell_positions = torch.load(
             statedir / "cell_positions.pt", map_location=self.device
-        ).int()
+        ).long()
         self.cell_divisions = torch.load(
             statedir / "cell_divisions.pt", map_location=self.device
         ).int()
 
         with open(statedir / "cells.fasta", "r", encoding="utf-8") as fh:
             text: str = fh.read()
             entries = [d.strip() for d in text.split(">") if len(d.strip()) > 0]
 
         self.labels = []
         self.genomes = []
         genome_idx_pairs: list[tuple[str, int]] = []
         for idx, entry in enumerate(entries):
-            descr, seq = entry.split("\n")
+            parts = entry.split("\n")
+            descr = parts[0]
+            seq = "" if len(parts) < 2 else parts[1]
             names = descr.split()
             label = names[1].strip() if len(names) > 1 else ""
             self.genomes.append(seq)
             self.labels.append(label)
             genome_idx_pairs.append((seq, idx))
 
         self.n_cells = len(genome_idx_pairs)
 
         if not ignore_cell_params:
             self.kinetics.increase_max_cells(by_n=self.n_cells)
-            self.update_cells(genome_idx_pairs=genome_idx_pairs)
+            self.update_cells(genome_idx_pairs=genome_idx_pairs, batch_size=batch_size)
 
     def _divide_cells_as_possible(
         self, parent_idxs: list[int]
     ) -> tuple[list[int], list[int], list[torch.Tensor]]:
         run_idx = self.n_cells
         child_idxs = []
         successful_parent_idxs = []
```

### Comparing `magicsoup-0.3.9/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.4.0/src/magicsoup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.9
+Version: 0.4.0
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
@@ -130,12 +130,12 @@
 ```python
 for _ in range(1000):
     world.enzymatic_activity()
     kill_cells()
     replicate_cells()
     mutate_cells()
     world.diffuse_molecules()
-    world.increment_cell_survival()
+    world.increment_cell_lifetimes()
 ```
 
 See the [Docs](https://magic-soup.readthedocs.io/) for more examples and a description of all the mechanics of this simulation
```

### Comparing `magicsoup-0.3.9/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.4.0/src/magicsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/tests/test_containers.py` & `magicsoup-0.4.0/tests/test_containers.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,7 +20,15 @@
 
 
 def test_similar_molecule_warning():
     with warnings.catch_warnings(record=True) as warn:
         cntnrs.Molecule(name="x", energy=10)
     assert len(warn) > 0
     assert issubclass(warn[-1].category, UserWarning)
+
+
+def test_molecule_mappings():
+    chem = cntnrs.Chemistry(molecules=[X, Y], reactions=[])
+    assert chem.mol_2_idx[X] == 0
+    assert chem.mol_2_idx[Y] == 1
+    assert chem.molname_2_idx["X"] == 0
+    assert chem.molname_2_idx["Y"] == 1
```

### Comparing `magicsoup-0.3.9/tests/test_genetics.py` & `magicsoup-0.4.0/tests/test_genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/tests/test_kinetics.py` & `magicsoup-0.4.0/tests/test_kinetics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import pytest
+import math
 import torch
 from magicsoup.containers import (
     Molecule,
     CatalyticDomain,
     RegulatoryDomain,
     TransporterDomain,
 )
+from magicsoup.constants import GAS_CONSTANT
 from magicsoup.kinetics import Kinetics
 
 TOLERANCE = 1e-4
+EPS = 1e-8
 
 
-ma = Molecule("a", energy=15)
-mb = Molecule("b", energy=10)
-mc = Molecule("c", energy=10)
-md = Molecule("d", energy=5)
+ma = Molecule("a", energy=15 * 1e3)
+mb = Molecule("b", energy=10 * 1e3)
+mc = Molecule("c", energy=10 * 1e3)
+md = Molecule("d", energy=5 * 1e3)
 MOLECULES = [ma, mb, mc, md]
 
 r_a_b = ([ma], [mb])
 r_b_c = ([mb], [mc])
 r_bc_d = ([mb, mc], [md])
 r_d_bb = ([md], [mb, mb])
 REACTIONS = [r_a_b, r_b_c, r_bc_d, r_d_bb]
@@ -72,126 +75,37 @@
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
     [0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0, 0.0],
 ])
 
 # fmt: on
 
 
-def get_kinetics() -> Kinetics:
-    kinetics = Kinetics(molecules=MOLECULES, reactions=REACTIONS)
+def get_kinetics(n_computations=1) -> Kinetics:
+    kinetics = Kinetics(
+        molecules=MOLECULES,
+        reactions=REACTIONS,
+        n_computations=n_computations,
+        abs_temp=310,
+    )
     kinetics.km_map.weights = KM_WEIGHTS.clone()
     kinetics.vmax_map.weights = VMAX_WEIGHTS.clone()
     kinetics.sign_map.signs = SIGNS.clone()
     kinetics.transport_map.M = TRANSPORT_M.clone()
     kinetics.effector_map.M = EFFECTOR_M.clone()
     kinetics.reaction_map.M = REACTION_M.clone()
     return kinetics
 
 
-def avg(*x):
-    return sum(x) / len(x)
-
-
-def test_cell_params_with_catalytic_domains_and_co_factors():
-    # Dealing with stoichiometric numbers that cancel each other out
-    # in general, intermediate molecules should be 0 in N
-    # but the reaction must depend on abundance of the starting molecules
-    # the first domain defines these starting molecules
-    # if these are 0 in N, they must appear in A
-
-    # C0, P0:
-    # bc->d then d->2b so bc->2b, with N b=1 c=-1 d=0
-    # b needs to be added as activating effector A b=1
-    # C0, P1:
-    # d->2b then bc->d, with N b=1 c=-1 d=0
-    # d needs to be added as activating effector A d=1
-    #
-    # the stoichiometry in both proteins in C0 is the same, but
-    # the order in which domains were defined is different
-    # That's why they differ in A
-
-    # Domain spec indexes: (dom_types, reacts_trnspts_effctrs, Vmaxs, Kms, signs)
-    # fmt: off
-    c0 = [
-        [
-            (1, 2, 15, 1, 3), # catal, Vmax 1.2, Km 1.5, fwd, bc->d
-            (1, 1, 5, 1, 4), # catal, Vmax 1.1, Km 0.5, fwd, d->2b
-        ],
-        [
-            (1, 1, 5, 1, 4), # catal, Vmax 1.1, Km 0.5, fwd, d->2b
-            (1, 2, 15, 1, 3), # catal, Vmax 1.2, Km 1.5, fwd, bc->d
-        ]
-    ]
-
-    # fmt: on
-
-    Km = torch.zeros(1, 3, 8)
-    Vmax = torch.zeros(1, 3)
-    E = torch.zeros(1, 3)
-    N = torch.zeros(1, 3, 8)
-    A = torch.zeros(1, 3, 8)
-
-    # test
-    kinetics = get_kinetics()
-    kinetics.Km = Km
-    kinetics.Vmax = Vmax
-    kinetics.E = E
-    kinetics.N = N
-    kinetics.A = A
-    kinetics.set_cell_params(cell_idxs=[0], proteomes=[c0])
+def ke(subs: list[Molecule], prods: list[Molecule]):
+    e = sum(d.energy for d in prods) - sum(d.energy for d in subs)
+    return math.exp(-e / 310 / GAS_CONSTANT)
 
-    # proteins in C0 only differ in A
-    for p in [0, 1]:
-        assert Km[0, p, 1] == pytest.approx(avg(1.5, 1 / 0.5), abs=TOLERANCE)
-        assert Km[0, p, 2] == pytest.approx(1.5, abs=TOLERANCE)
-        assert Km[0, p, 3] == pytest.approx(avg(0.5, 1 / 1.5), abs=TOLERANCE)
-        for i in [0, 4, 5, 6, 7]:
-            assert Km[0, p, i] == 0.0
-
-        assert Vmax[0, p] == pytest.approx(avg(1.1, 1.2), abs=TOLERANCE)
-
-        assert E[0, p] == 10 - 10
-
-        assert N[0, p, 1] == 1
-        assert N[0, p, 2] == -1
-        assert N[0, p, 3] == 0
-        for i in [0, 4, 5, 6, 7]:
-            assert N[0, p, i] == 0
-
-    assert A[0, 0, 1] == 1
-    assert A[0, 1, 3] == 1
-    assert A.sum() == 2
 
-    # test proteome representation
-
-    proteins = kinetics.get_proteome(proteome=c0)
-
-    p0 = proteins[0]
-    assert isinstance(p0.domains[0], CatalyticDomain)
-    assert p0.domains[0].substrates == [mb, mc]
-    assert p0.domains[0].products == [md]
-    assert p0.domains[0].vmax == pytest.approx(1.2, abs=TOLERANCE)
-    assert p0.domains[0].km == pytest.approx(1.5, abs=TOLERANCE)
-    assert isinstance(p0.domains[1], CatalyticDomain)
-    assert p0.domains[1].substrates == [md]
-    assert p0.domains[1].products == [mb, mb]
-    assert p0.domains[1].vmax == pytest.approx(1.1, abs=TOLERANCE)
-    assert p0.domains[1].km == pytest.approx(0.5, abs=TOLERANCE)
-
-    p1 = proteins[1]
-    assert isinstance(p1.domains[0], CatalyticDomain)
-    assert p1.domains[0].substrates == [md]
-    assert p1.domains[0].products == [mb, mb]
-    assert p1.domains[0].vmax == pytest.approx(1.1, abs=TOLERANCE)
-    assert p1.domains[0].km == pytest.approx(0.5, abs=TOLERANCE)
-    assert isinstance(p1.domains[1], CatalyticDomain)
-    assert p1.domains[1].substrates == [mb, mc]
-    assert p1.domains[1].products == [md]
-    assert p1.domains[1].vmax == pytest.approx(1.2, abs=TOLERANCE)
-    assert p1.domains[1].km == pytest.approx(1.5, abs=TOLERANCE)
+def avg(*x):
+    return sum(x) / len(x)
 
 
 def test_cell_params_with_transporter_domains():
     # Domain spec indexes: (dom_types, reacts_trnspts_effctrs, Vmaxs, Kms, signs)
     # fmt: off
     c0 = [
         [
@@ -212,95 +126,94 @@
         [
             (1, 10, 5, 1, 1), # catal, Vmax 2.0, Km 0.5, fwd, a->b
             (2, 5, 5, 1, 1)   # transporter, Vmax 1.5, Km 0.5, fwd, mol a
         ],
     ]
     # fmt: on
 
-    Km = torch.zeros(2, 3, 8)
+    Kmf = torch.zeros(2, 3)
+    Kmb = torch.zeros(2, 3)
+    Kmr = torch.zeros(2, 3)
     Vmax = torch.zeros(2, 3)
-    E = torch.zeros(2, 3)
     N = torch.zeros(2, 3, 8)
+    Nf = torch.zeros(2, 3, 8)
+    Nb = torch.zeros(2, 3, 8)
     A = torch.zeros(2, 3, 8)
 
     # test
     kinetics = get_kinetics()
-    kinetics.Km = Km
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
-    kinetics.E = E
     kinetics.N = N
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
     kinetics.A = A
     kinetics.set_cell_params(cell_idxs=[0, 1], proteomes=[c0, c1])
 
-    assert Km[0, 0, 0] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Km[0, 0, 4] == pytest.approx(1 / 0.5, abs=TOLERANCE)
-    for i in [1, 2, 3, 5, 6, 7]:
-        assert Km[0, 0, i] == 0.0
-    assert Km[0, 1, 0] == pytest.approx(avg(0.5, 1 / 0.2), abs=TOLERANCE)
-    assert Km[0, 1, 4] == pytest.approx(avg(1 / 0.5, 0.2), abs=TOLERANCE)
-    for i in [1, 2, 3, 5, 6, 7]:
-        assert Km[0, 1, i] == 0.0
-
-    assert Km[1, 0, 0] == pytest.approx(avg(0.4, 0.5), abs=TOLERANCE)
-    assert Km[1, 0, 1] == pytest.approx(0.6, abs=TOLERANCE)
-    assert Km[1, 0, 2] == pytest.approx(0.7, abs=TOLERANCE)
-    assert Km[1, 0, 4] == pytest.approx(avg(1 / 0.4, 1 / 0.5), abs=TOLERANCE)
-    assert Km[1, 0, 5] == pytest.approx(1 / 0.6, abs=TOLERANCE)
-    assert Km[1, 0, 6] == pytest.approx(1 / 0.7, abs=TOLERANCE)
-    for i in [3, 7]:
-        assert Km[1, 0, i] == 0.0
-    assert Km[1, 1, 0] == pytest.approx(avg(0.5, 0.5), abs=TOLERANCE)
-    assert Km[1, 1, 1] == pytest.approx(1 / 0.5, abs=TOLERANCE)
-    assert Km[1, 1, 4] == pytest.approx(1 / 0.5, abs=TOLERANCE)
-    for i in [2, 3, 5, 6, 7]:
-        assert Km[1, 1, i] == 0.0
+    assert Kmf[0, 0] == pytest.approx(0.5, abs=TOLERANCE)
+    assert Kmb[0, 0] == pytest.approx(0.5, abs=TOLERANCE)
+    assert Kmf[0, 1] == pytest.approx(avg(0.5, 0.2), abs=TOLERANCE)
+    assert Kmb[0, 1] == pytest.approx(avg(0.5, 0.2), abs=TOLERANCE)
+    assert Kmf[0, 2] == pytest.approx(0.0, TOLERANCE)
+    assert Kmb[0, 2] == pytest.approx(0.0, TOLERANCE)
+
+    ke_c1_1 = ke([ma], [mb])
+    assert Kmf[1, 0] == pytest.approx(avg(0.4, 0.5, 0.6, 0.7), abs=TOLERANCE)
+    assert Kmb[1, 0] == pytest.approx(avg(0.4, 0.5, 0.6, 0.7), abs=TOLERANCE)
+    assert Kmf[1, 1] == pytest.approx(avg(0.5, 0.5), abs=TOLERANCE)
+    assert Kmb[1, 1] == pytest.approx(avg(0.5, 0.5) * ke_c1_1, abs=TOLERANCE)
+    assert Kmf[1, 2] == pytest.approx(0.0, TOLERANCE)
+    assert Kmb[1, 2] == pytest.approx(0.0, TOLERANCE)
+
+    assert (Kmr < TOLERANCE).all()
 
     assert Vmax[0, 0] == pytest.approx(1.5, abs=TOLERANCE)
     assert Vmax[0, 1] == pytest.approx(avg(1.5, 1.1), abs=TOLERANCE)
     assert Vmax[0, 2] == 0.0
 
     assert Vmax[1, 0] == pytest.approx(avg(1.5, 1.4, 1.3, 1.2), abs=TOLERANCE)
     assert Vmax[1, 1] == pytest.approx(avg(2.0, 1.5), abs=TOLERANCE)
     assert Vmax[1, 2] == 0.0
 
-    assert E[0, 0] == 0
-    assert E[0, 1] == 0
-    assert E[0, 2] == 0
-
-    assert E[1, 0] == 0
-    assert E[1, 1] == 10 - 15
-    assert E[1, 2] == 0
-
     assert N[0, 0, 0] == -1
     assert N[0, 0, 4] == 1
-    for i in [1, 2, 3, 5, 6, 7]:
-        assert N[0, 0, i] == 0
-    assert N[0, 1, 0] == 0
-    assert N[0, 1, 4] == 0
-    for i in [1, 2, 3, 5, 6, 7]:
-        assert N[0, 1, i] == 0
+    assert (N[0, 0, [1, 2, 3, 5, 6, 7]] == 0).all()
+    assert Nf[0, 0, 0] == 1
+    assert (Nf[0, 0, [1, 2, 3, 4, 5, 6, 7]] == 0).all()
+    assert Nb[0, 1, 4] == 1
+    assert (Nb[0, 0, [0, 1, 2, 3, 5, 6, 7]] == 0).all()
 
     assert N[1, 0, 0] == -2
     assert N[1, 0, 1] == -1
     assert N[1, 0, 2] == -1
     assert N[1, 0, 4] == 2
     assert N[1, 0, 5] == 1
     assert N[1, 0, 6] == 1
-    for i in [3, 7]:
-        assert N[1, 0, i] == 0
+    assert (N[1, 0, [3, 7]] == 0).all()
+    assert Nf[1, 0, 0] == 2
+    assert Nf[1, 0, 1] == 1
+    assert Nf[1, 0, 2] == 1
+    assert (Nf[1, 0, [4, 5, 6, 3, 7]] == 0).all()
+    assert Nb[1, 0, 4] == 2
+    assert Nb[1, 0, 5] == 1
+    assert Nb[1, 0, 6] == 1
+    assert (Nb[1, 0, [0, 1, 2, 3, 7]] == 0).all()
     assert N[1, 1, 0] == -2
     assert N[1, 1, 1] == 1
     assert N[1, 1, 4] == 1
-    for i in [2, 3, 5, 6, 7]:
-        assert N[1, 1, i] == 0
+    assert (N[1, 1, [2, 3, 5, 6, 7]] == 0).all()
+    assert Nf[1, 1, 0] == 2
+    assert (Nf[1, 1, [1, 2, 3, 4, 5, 6, 7]] == 0).all()
+    assert Nb[1, 1, 1] == 1
+    assert Nb[1, 1, 4] == 1
+    assert (Nb[1, 1, [0, 2, 3, 5, 6, 7]] == 0).all()
 
-    # a was imported and exported, so its N=0
-    # but it must be added as effector
-    assert A[0, 1, 0] == 1
-    assert A.sum() == 1
+    assert (A == 0).all()
 
     # test proteome representation
 
     proteins = kinetics.get_proteome(proteome=c0)
 
     p0 = proteins[0]
     assert isinstance(p0.domains[0], TransporterDomain)
@@ -312,15 +225,15 @@
     assert isinstance(p1.domains[0], TransporterDomain)
     assert p1.domains[0].molecule is ma
     assert p1.domains[0].vmax == pytest.approx(1.5, abs=TOLERANCE)
     assert p1.domains[0].km == pytest.approx(0.5, abs=TOLERANCE)
     assert isinstance(p1.domains[1], TransporterDomain)
     assert p1.domains[1].molecule is ma
     assert p1.domains[1].vmax == pytest.approx(1.1, abs=TOLERANCE)
-    assert p1.domains[1].km == pytest.approx(1 / 0.2, abs=TOLERANCE)
+    assert p1.domains[1].km == pytest.approx(0.2, abs=TOLERANCE)
 
     proteins = kinetics.get_proteome(proteome=c1)
 
     p0 = proteins[0]
     assert isinstance(p0.domains[0], TransporterDomain)
     assert p0.domains[0].molecule is ma
     assert p0.domains[0].vmax == pytest.approx(1.5, abs=TOLERANCE)
@@ -376,138 +289,113 @@
             (1, 10, 5, 1, 1), # catal, Vmax 2.0, Km 0.5, fwd, a->b
             (3, 0, 10, 1, 4), # reg, Km 1.0, cyto, act, d
             (3, 0, 15, 1, 4), # reg, Km 1.5, cyto, act, d
         ]
     ]
     # fmt: on
 
-    Km = torch.zeros(2, 3, 8)
+    Kmf = torch.zeros(2, 3)
+    Kmb = torch.zeros(2, 3)
+    Kmr = torch.zeros(2, 3)
     Vmax = torch.zeros(2, 3)
-    E = torch.zeros(2, 3)
     N = torch.zeros(2, 3, 8)
+    Nf = torch.zeros(2, 3, 8)
+    Nb = torch.zeros(2, 3, 8)
     A = torch.zeros(2, 3, 8)
 
     # test
     kinetics = get_kinetics()
-    kinetics.Km = Km
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
-    kinetics.E = E
     kinetics.N = N
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
     kinetics.A = A
     kinetics.set_cell_params(cell_idxs=[0, 1], proteomes=[c0, c1])
 
-    assert Km[0, 0, 0] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Km[0, 0, 1] == pytest.approx(1 / 0.5, abs=TOLERANCE)
-    assert Km[0, 0, 2] == pytest.approx(1.0, abs=TOLERANCE)
-    assert Km[0, 0, 3] == pytest.approx(2.0, abs=TOLERANCE)
-    for i in [4, 5, 6, 7]:
-        assert Km[0, 0, i] == 0.0
-    assert Km[0, 1, 0] == pytest.approx(avg(0.5, 1.0), abs=TOLERANCE)
-    assert Km[0, 1, 1] == pytest.approx(1 / 0.5, abs=TOLERANCE)
-    assert Km[0, 1, 2] == pytest.approx(0.0, abs=TOLERANCE)
-    assert Km[0, 1, 3] == pytest.approx(0.0, abs=TOLERANCE)
-    assert Km[0, 1, 4] == pytest.approx(1.5, abs=TOLERANCE)
-    for i in [5, 6, 7]:
-        assert Km[0, 1, i] == 0.0
-    for i in range(8):
-        assert Km[0, 2, i] == 0.0
-
-    assert Km[1, 0, 0] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Km[1, 0, 1] == pytest.approx(avg(1 / 0.5, 1.0), abs=TOLERANCE)
-    assert Km[1, 0, 2] == pytest.approx(0.0, abs=TOLERANCE)
-    assert Km[1, 0, 3] == pytest.approx(0.0, abs=TOLERANCE)
-    assert Km[1, 0, 5] == pytest.approx(1.5, abs=TOLERANCE)
-    for i in [4, 6, 7]:
-        assert Km[1, 0, i] == 0.0
-    assert Km[1, 1, 0] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Km[1, 1, 1] == pytest.approx(1 / 0.5, abs=TOLERANCE)
-    assert Km[1, 1, 2] == pytest.approx(0.0, abs=TOLERANCE)
-    assert Km[1, 1, 3] == pytest.approx(avg(1.0, 1.5), abs=TOLERANCE)
-    for i in [4, 5, 6, 7]:
-        assert Km[1, 1, i] == 0.0
-    for i in range(8):
-        assert Km[1, 2, i] == 0.0
+    ke_c0_0 = ke([ma], [mb])
+    ke_c0_1 = ke([ma], [mb])
+    assert Kmf[0, 0] == pytest.approx(0.5, abs=TOLERANCE)
+    assert Kmb[0, 0] == pytest.approx(0.5 * ke_c0_0, abs=TOLERANCE)
+    assert Kmr[0, 0] == pytest.approx(avg(1.0, 2.0), abs=TOLERANCE)
+    assert Kmf[0, 1] == pytest.approx(0.5, abs=TOLERANCE)
+    assert Kmb[0, 1] == pytest.approx(0.5 * ke_c0_1, abs=TOLERANCE)
+    assert Kmr[0, 1] == pytest.approx(avg(1.0, 1.5), abs=TOLERANCE)
+    assert Kmf[0, 2] == pytest.approx(0.0, TOLERANCE)
+    assert Kmb[0, 2] == pytest.approx(0.0, TOLERANCE)
+    assert Kmr[0, 2] == pytest.approx(0.0, TOLERANCE)
+
+    assert Kmf[1, 0] == pytest.approx(0.5, abs=TOLERANCE)
+    assert Kmb[1, 0] == pytest.approx(0.5 * ke_c0_0, abs=TOLERANCE)
+    assert Kmf[1, 1] == pytest.approx(0.5, abs=TOLERANCE)
+    assert Kmb[1, 1] == pytest.approx(0.5 * ke_c0_1, abs=TOLERANCE)
+    assert Kmf[1, 2] == pytest.approx(0.0, TOLERANCE)
+    assert Kmb[1, 2] == pytest.approx(0.0, TOLERANCE)
 
     assert Vmax[0, 0] == pytest.approx(2.0, abs=TOLERANCE)
     assert Vmax[0, 1] == pytest.approx(2.0, abs=TOLERANCE)
     assert Vmax[0, 2] == 0.0
 
     assert Vmax[1, 0] == pytest.approx(2.0, abs=TOLERANCE)
     assert Vmax[1, 1] == pytest.approx(2.0, abs=TOLERANCE)
     assert Vmax[1, 2] == 0.0
 
-    assert E[0, 0] == 10 - 15
-    assert E[0, 1] == 10 - 15
-    assert E[0, 2] == 0
-
-    assert E[1, 0] == 10 - 15
-    assert E[1, 1] == 10 - 15
-    assert E[1, 2] == 0
-
     assert N[0, 0, 0] == -1
     assert N[0, 0, 1] == 1
-    assert N[0, 0, 2] == 0
-    assert N[0, 0, 3] == 0
-    for i in [4, 5, 6, 7]:
-        assert N[0, 0, i] == 0
+    assert (N[0, 0, [2, 3, 4, 5, 6]] == 0).all()
+    assert Nf[0, 0, 0] == 1
+    assert (Nf[0, 0, [1, 2, 3, 4, 5, 6]] == 0).all()
+    assert Nb[0, 0, 1] == 1
+    assert (Nb[0, 0, [0, 2, 3, 4, 5, 6]] == 0).all()
     assert N[0, 1, 0] == -1
     assert N[0, 1, 1] == 1
-    assert N[0, 1, 2] == 0
-    assert N[0, 1, 3] == 0
-    for i in [4, 5, 6, 7]:
-        assert N[0, 1, i] == 0
-    for i in range(8):
-        assert N[0, 2, i] == 0
+    assert (N[0, 1, [2, 3, 4, 5, 6, 7]] == 0).all()
+    assert Nf[0, 1, 0] == 1
+    assert (Nf[0, 1, [1, 2, 3, 4, 5, 6, 7]] == 0).all()
+    assert Nb[0, 1, 1] == 1
+    assert (Nb[0, 1, [0, 2, 3, 4, 5, 6, 7]] == 0).all()
+    assert (N[0, 2] == 0).all()
+    assert (Nf[0, 2] == 0).all()
+    assert (Nb[0, 2] == 0).all()
 
     assert N[1, 0, 0] == -1
     assert N[1, 0, 1] == 1
-    assert N[1, 0, 2] == 0
-    assert N[1, 0, 3] == 0
-    for i in [4, 5, 6, 7]:
-        assert N[1, 0, i] == 0
+    assert (N[1, 0, [2, 3, 4, 5, 6, 7]] == 0).all()
+    assert Nf[1, 0, 0] == 1
+    assert (Nf[1, 0, [1, 2, 3, 4, 5, 6, 7]] == 0).all()
+    assert Nb[1, 0, 1] == 1
+    assert (Nb[1, 0, [0, 2, 3, 4, 5, 6, 7]] == 0).all()
     assert N[1, 1, 0] == -1
     assert N[1, 1, 1] == 1
-    assert N[1, 1, 2] == 0
-    assert N[1, 1, 3] == 0
-    for i in [4, 5, 6, 7]:
-        assert N[1, 1, i] == 0
-    for i in range(8):
-        assert N[1, 2, i] == 0
+    assert (N[1, 1, [2, 3, 4, 5, 6, 7]] == 0).all()
+    assert Nf[1, 1, 0] == 1
+    assert (Nf[1, 1, [1, 2, 3, 4, 5, 6, 7]] == 0).all()
+    assert Nb[1, 1, 1] == 1
+    assert (Nb[1, 1, [0, 2, 3, 4, 5, 6, 7]] == 0).all()
+    assert (N[1, 2] == 0).all()
+    assert (Nf[1, 2] == 0).all()
+    assert (Nb[1, 2] == 0).all()
 
-    assert A[0, 0, 0] == 0
-    assert A[0, 0, 1] == 0
     assert A[0, 0, 2] == 1
     assert A[0, 0, 3] == -1
-    for i in [4, 5, 6, 7]:
-        assert A[0, 0, i] == 0
+    assert (A[0, 0, [0, 1, 4, 5, 6, 7]] == 0).all()
     assert A[0, 1, 0] == 1
-    assert A[0, 1, 1] == 0
-    assert A[0, 1, 2] == 0
-    assert A[0, 1, 3] == 0
     assert A[0, 1, 4] == 1
-    for i in [5, 6, 7]:
-        assert A[0, 1, i] == 0
-    for i in range(8):
-        assert A[0, 2, i] == 0
+    assert (A[0, 1, [1, 2, 3, 5, 6, 7]] == 0).all()
+    assert (A[0, 2] == 0).all()
 
-    assert A[1, 0, 0] == 0
     assert A[1, 0, 1] == -1
-    assert A[1, 0, 2] == 0
-    assert A[1, 0, 3] == 0
     assert A[1, 0, 5] == -1
-    for i in [4, 6, 7]:
-        assert A[0, 0, i] == 0
+    assert (A[1, 0, [0, 2, 3, 4, 6, 7]] == 0).all()
     assert A[1, 1, 0] == 0
-    assert A[1, 1, 1] == 0
-    assert A[1, 1, 2] == 0
     assert A[1, 1, 3] == 2
-    for i in [4, 5, 6, 7]:
-        assert A[1, 1, i] == 0
-    for i in range(8):
-        assert A[1, 2, i] == 0
+    assert (A[1, 1, [1, 2, 4, 5, 6, 7]] == 0).all()
+    assert (A[1, 2] == 0).all()
 
     # test protein representation
 
     proteins = kinetics.get_proteome(proteome=c0)
 
     p0 = proteins[0]
     assert isinstance(p0.domains[0], CatalyticDomain)
@@ -605,119 +493,122 @@
             (1, 9, 3, 1, 2), # catal, Vmax 1.9, Km 0.3, fwd, b->c
             (1, 13, 17, 1, 3), # catal, Vmax 2.3, Km 1.7, fwd, bc->d
         ]
     ]
 
     # fmt: on
 
-    Km = torch.zeros(2, 3, 8)
+    Kmf = torch.zeros(2, 3)
+    Kmb = torch.zeros(2, 3)
+    Kmr = torch.zeros(2, 3)
     Vmax = torch.zeros(2, 3)
-    E = torch.zeros(2, 3)
     N = torch.zeros(2, 3, 8)
+    Nf = torch.zeros(2, 3, 8)
+    Nb = torch.zeros(2, 3, 8)
     A = torch.zeros(2, 3, 8)
 
     # test
     kinetics = get_kinetics()
-    kinetics.Km = Km
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
-    kinetics.E = E
     kinetics.N = N
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
     kinetics.A = A
     kinetics.set_cell_params(cell_idxs=[0, 1], proteomes=[c0, c1])
 
-    assert Km[0, 0, 0] == pytest.approx(0.5, abs=TOLERANCE)
-    assert Km[0, 0, 1] == pytest.approx(avg(1 / 0.5, 1 / 1.5), abs=TOLERANCE)
-    assert Km[0, 0, 2] == pytest.approx(1 / 1.5, abs=TOLERANCE)
-    assert Km[0, 0, 3] == pytest.approx(1.5, abs=TOLERANCE)
-    for i in [4, 5, 6, 7]:
-        assert Km[0, 0, i] == 0.0
-    assert Km[0, 1, 0] == 0.0
-    assert Km[0, 1, 1] == pytest.approx(avg(0.9, 1 / 1.2), abs=TOLERANCE)
-    assert Km[0, 1, 2] == pytest.approx(avg(1 / 0.9, 1 / 1.2), abs=TOLERANCE)
-    assert Km[0, 1, 3] == pytest.approx(1.2, abs=TOLERANCE)
-    for i in [4, 5, 6, 7]:
-        assert Km[0, 1, i] == 0.0
-    assert Km[0, 2, 0] == 0.0
-    assert Km[0, 2, 1] == pytest.approx(1 / 2.9, abs=TOLERANCE)
-    assert Km[0, 2, 2] == 0.0
-    assert Km[0, 2, 3] == pytest.approx(2.9, abs=TOLERANCE)
-    for i in [4, 5, 6, 7]:
-        assert Km[0, 2, i] == 0.0
-
-    assert Km[1, 0, 0] == pytest.approx(1 / 0.3, abs=TOLERANCE)
-    assert Km[1, 0, 1] == pytest.approx(avg(0.3, 1 / 1.4), abs=TOLERANCE)
-    assert Km[1, 0, 2] == pytest.approx(1 / 1.4, abs=TOLERANCE)
-    assert Km[1, 0, 3] == pytest.approx(1.4, abs=TOLERANCE)
-    for i in [4, 5, 6, 7]:
-        assert Km[1, 0, i] == 0.0
-    assert Km[1, 1, 0] == 0.0
-    assert Km[1, 1, 1] == pytest.approx(avg(0.3, 1.7), abs=TOLERANCE)
-    assert Km[1, 1, 2] == pytest.approx(avg(1 / 0.3, 1.7), abs=TOLERANCE)
-    assert Km[1, 1, 3] == pytest.approx(1 / 1.7, abs=TOLERANCE)
-    for i in [4, 5, 6, 7]:
-        assert Km[1, 1, i] == 0.0
-    for i in range(8):
-        assert Km[1, 2, i] == 0.0
+    ke_c0_0 = ke([ma, md], [mb, mb, mc])
+    ke_c0_1 = ke([mb, md], [mc, mb, mc])
+    ke_c0_2 = ke([md], [mb, mb])
+    assert Kmf[0, 0] == pytest.approx(avg(0.5, 1.5) / ke_c0_0, abs=TOLERANCE)
+    assert Kmb[0, 0] == pytest.approx(avg(0.5, 1.5), abs=TOLERANCE)
+    assert Kmf[0, 1] == pytest.approx(avg(0.9, 1.2) / ke_c0_1, abs=TOLERANCE)
+    assert Kmb[0, 1] == pytest.approx(avg(0.9, 1.2), abs=TOLERANCE)
+    assert Kmf[0, 2] == pytest.approx(2.9 / ke_c0_2, abs=TOLERANCE)
+    assert Kmb[0, 2] == pytest.approx(2.9, abs=TOLERANCE)
+
+    ke_c1_0 = ke([mb, md], [ma, mb, mc])
+    ke_c1_1 = ke([mb, mb, mc], [mc, md])
+    assert Kmf[1, 0] == pytest.approx(avg(0.3, 1.4) / ke_c1_0, TOLERANCE)
+    assert Kmb[1, 0] == pytest.approx(avg(0.3, 1.4), TOLERANCE)
+    assert Kmf[1, 1] == pytest.approx(avg(0.3, 1.7), TOLERANCE)
+    assert Kmb[1, 1] == pytest.approx(avg(0.3, 1.7) * ke_c1_1, TOLERANCE)
+    assert Kmf[1, 2] == pytest.approx(0.0, TOLERANCE)
+    assert Kmb[1, 2] == pytest.approx(0.0, TOLERANCE)
+
+    assert (Kmr < TOLERANCE).all()
 
     assert Vmax[0, 0] == pytest.approx(avg(1.1, 1.2), abs=TOLERANCE)
     assert Vmax[0, 1] == pytest.approx(avg(2.0, 1.3), abs=TOLERANCE)
     assert Vmax[0, 2] == pytest.approx(2.9, abs=TOLERANCE)
 
     assert Vmax[1, 0] == pytest.approx(avg(1.1, 2.1), abs=TOLERANCE)
     assert Vmax[1, 1] == pytest.approx(avg(1.9, 2.3), abs=TOLERANCE)
     assert Vmax[1, 2] == 0.0
 
-    assert E[0, 0] == 10 - 15 + 10 + 10 - 5
-    assert E[0, 1] == 10 - 10 - 5 + 10 + 10
-    assert E[0, 2] == 10 + 10 - 5
-
-    assert E[1, 0] == 15 - 10 - 5 + 10 + 10
-    assert E[1, 1] == 10 - 10 + 5 - 10 - 10
-    assert E[1, 2] == 0
-
     assert N[0, 0, 0] == -1
     assert N[0, 0, 1] == 2
     assert N[0, 0, 2] == 1
     assert N[0, 0, 3] == -1
-    for i in [4, 5, 6, 7]:
-        assert N[0, 0, i] == 0
-    assert N[0, 1, 0] == 0
-    assert N[0, 1, 1] == 0  # b is added and removed
+    assert (N[0, 0, [4, 5, 6, 7]] == 0).all()
+    assert Nf[0, 0, 0] == 1
+    assert Nf[0, 0, 3] == 1
+    assert (Nf[0, 0, [1, 2, 4, 5, 6, 7]] == 0).all()
+    assert Nb[0, 0, 1] == 2
+    assert Nb[0, 0, 2] == 1
+    assert (Nb[0, 0, [0, 3, 4, 5, 6, 7]] == 0).all()
     assert N[0, 1, 2] == 2
     assert N[0, 1, 3] == -1
-    for i in [4, 5, 6, 7]:
-        assert N[0, 1, i] == 0
+    assert (N[0, 1, [0, 1, 4, 5, 6, 7]] == 0).all()
+    assert Nf[0, 1, 1] == 1
+    assert Nf[0, 1, 3] == 1
+    assert (Nf[0, 1, [0, 2, 4, 5, 6, 7]] == 0).all()
+    assert Nb[0, 1, 1] == 1
+    assert Nb[0, 1, 2] == 2
+    assert (Nb[0, 1, [0, 3, 4, 5, 6, 7]] == 0).all()
     assert N[0, 2, 0] == 0
     assert N[0, 2, 1] == 2
     assert N[0, 2, 2] == 0
     assert N[0, 2, 3] == -1
-    for i in [4, 5, 6, 7]:
-        assert N[0, 2, i] == 0
+    assert (N[0, 2, [4, 5, 6, 7]] == 0).all()
+    assert Nf[0, 2, 3] == 1
+    assert (Nf[0, 2, [0, 1, 2, 4, 5, 6, 7]] == 0).all()
+    assert Nb[0, 2, 1] == 2
+    assert (Nb[0, 2, [0, 2, 3, 4, 5, 6, 7]] == 0).all()
 
     assert N[1, 0, 0] == 1
     assert N[1, 0, 1] == 0  # b is added and removed
     assert N[1, 0, 2] == 1
     assert N[1, 0, 3] == -1
-    for i in [4, 5, 6, 7]:
-        assert N[1, 0, i] == 0
+    assert (N[1, 0, [4, 5, 6, 7]] == 0).all()
+    assert Nf[1, 0, 1] == 1
+    assert Nf[1, 0, 3] == 1
+    assert (Nf[1, 0, [0, 2, 4, 5, 6, 7]] == 0).all()
+    assert Nb[1, 0, 0] == 1
+    assert Nb[1, 0, 1] == 1
+    assert Nb[1, 0, 2] == 1
+    assert (Nb[1, 0, [3, 4, 5, 6, 7]] == 0).all()
     assert N[1, 1, 0] == 0
     assert N[1, 1, 1] == -2
     assert N[1, 1, 2] == 0  # c is added and removed
     assert N[1, 1, 3] == 1
-    for i in [4, 5, 6, 7]:
-        assert N[1, 1, i] == 0
-    for i in range(8):
-        assert N[1, 2, i] == 0
-
-    # b was a reactant in the first domain,
-    # but was then created again yielding N b=0
-    # it thus has to be added as activating effector
-    assert A[0, 1, 1] == 1
-    assert A[1, 0, 1] == 1
-    assert A.sum() == 2
+    assert (N[1, 1, [4, 5, 6, 7]] == 0).all()
+    assert Nf[1, 1, 1] == 2
+    assert Nf[1, 1, 2] == 1
+    assert (Nf[1, 1, [0, 3, 4, 5, 6, 7]] == 0).all()
+    assert Nb[1, 1, 2] == 1
+    assert Nb[1, 1, 3] == 1
+    assert (Nb[1, 1, [0, 1, 4, 5, 6, 7]] == 0).all()
+    assert (N[1, 2] == 0).all()
+    assert (Nf[1, 2] == 0).all()
+    assert (Nb[1, 2] == 0).all()
+
+    assert (A == 0).all()
 
     # test protein representation
 
     proteins = kinetics.get_proteome(proteome=c0)
 
     p0 = proteins[0]
     assert isinstance(p0.domains[0], CatalyticDomain)
@@ -795,142 +686,167 @@
         [   [-1.0, 1.0, 0.0, 0.0],
             [0.0, -1.0, 0.0, 1.0],
             [0.0, 0.0, 0.0, 0.0]    ],
         [   [0.0, 0.0, -1.0, 1.0],
             [-1.0, 0.0, 0.0, 1.0],
             [0.0, 0.0, 0.0, 0.0]    ],
     ])
+    Nf = torch.where(N < 0.0, -N, 0.0)
+    Nb = torch.where(N > 0.0, N, 0.0)
 
-    # affinities (c, p, s)
-    Km = torch.tensor([
-        [   [1.2, 1.5, 0.0, 0.0],
-            [0.0, 0.5, 0.0, 3.5],
-            [0.0, 0.0, 0.0, 0.0] ],
-        [   [0.0, 0.0, 0.5, 1.5],
-            [1.2, 0.0, 0.0, 1.9],
-            [0.0, 0.0, 0.0, 0.0] ],
+    # affinities (c, p)
+    Kmf = torch.tensor([
+        [1.3, 2.1, 0.0],
+        [1.0, 1.7, 0.0],
+    ])
+    Kmb = torch.tensor([
+        [0.3, 1.1, 0.0],
+        [1.5, 0.7, 0.0],
     ])
+    Kmr = torch.zeros(2, 3)
 
     # max velocities (c, p)
     Vmax = torch.tensor([
         [2.1, 1.0, 0.0],
         [1.1, 2.0, 0.0],
     ])
 
     # allosterics (c, p, s)
     A = torch.zeros(2, 3, 4)
 
-    # reaction energies (c, p)
-    E = torch.full((2, 3), -99999.9)
-
     # fmt: on
 
-    def mm(x, k, v):
-        return v * x / (k + x)
+    def mm(s, p, kf, kb, v):
+        vf = v * (s / kf - p / kb) / (1 + s / kf + p / kb)
+        vb = v * (p / kb - s / kf) / (1 + s / kf + p / kb)
+        return (vf - vb) / 2
 
     # expected outcome
-    dx_c0_b = mm(x=X0[0, 0], v=Vmax[0, 0], k=Km[0, 0, 0])
-    dx_c0_a = -dx_c0_b
-    dx_c0_d = mm(x=X0[0, 1], v=Vmax[0, 1], k=Km[0, 1, 1])
-    dx_c0_b = dx_c0_b - dx_c0_d
-
-    dx_c1_d_1 = mm(x=X0[1, 2], v=Vmax[1, 0], k=Km[1, 0, 2])
-    dx_c1_c = -dx_c1_d_1
-    dx_c1_d_2 = mm(x=X0[1, 0], v=Vmax[1, 1], k=Km[1, 1, 0])
-    dx_c1_a = -dx_c1_d_2
-    dx_c1_d = dx_c1_d_1 + dx_c1_d_2
+    v_c0_0 = mm(X0[0, 0], X0[0, 1], Kmf[0, 0], Kmb[0, 0], Vmax[0, 0])
+    v_c0_1 = mm(X0[0, 1], X0[0, 3], Kmf[0, 1], Kmb[0, 1], Vmax[0, 1])
+    dx_c0_a = -v_c0_0
+    dx_c0_b = v_c0_0 - v_c0_1
+    dx_c0_c = 0.0
+    dx_c0_d = v_c0_1
+
+    v_c1_0 = mm(X0[1, 2], X0[1, 3], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0])
+    v_c1_1 = mm(X0[1, 0], X0[1, 3], Kmf[1, 1], Kmb[1, 1], Vmax[1, 1])
+    dx_c1_a = -v_c1_1
+    dx_c1_b = 0.0
+    dx_c1_c = -v_c1_0
+    dx_c1_d = v_c1_0 + v_c1_1
 
     # test
     kinetics = get_kinetics()
     kinetics.N = N
-    kinetics.Km = Km
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
-    kinetics.E = E
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
     assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
     assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
-    assert Xd[0, 2] == 0.0
+    assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
     assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
 
     assert (Xd[1, 0] - dx_c1_a).abs() < TOLERANCE
-    assert Xd[1, 1] == 0.0
+    assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
     assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
     assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
 
 
 def test_mm_kinetic_with_proportions():
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
     # cell 0: P0: a -> 2b, P1: 2c -> d
     # cell 1: P0: 3b -> 2c
 
     # fmt: off
 
     # concentrations (c, s)
     X0 = torch.tensor([
         [1.1, 0.1, 2.9, 0.8],
-        [1.2, 3.1, 1.5, 1.4],
+        [1.2, 4.9, 5.1, 1.4],
     ])
 
     # reactions (c, p, s)
     N = torch.tensor([
         [   [-1.0, 2.0, 0.0, 0.0],
             [0.0, 0.0, -2.0, 1.0],
             [0.0, 0.0, 0.0, 0.0]    ],
         [   [0.0, -3.0, 2.0, 0.0],
             [0.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 0.0, 0.0]    ],
     ])
+    Nf = torch.where(N < 0.0, -N, 0.0)
+    Nb = torch.where(N > 0.0, N, 0.0)
 
     # affinities (c, p, s)
-    Km = torch.tensor([
-        [   [1.2, 0.2, 0.0, 0.0],
-            [0.0, 0.0, 0.9, 1.2],
-            [0.0, 0.0, 0.0, 0.0] ],
-        [   [0.0, 1.5, 0.9, 0.0],
-            [0.0, 0.0, 0.0, 0.0],
-            [0.0, 0.0, 0.0, 0.0] ],
+    Kmf = torch.tensor([
+        [1.3, 2.1, 0.0],
+        [1.4, 0.0, 0.0],
+    ])
+    Kmb = torch.tensor([
+        [0.3, 1.1, 0.0],
+        [1.5, 0.0, 0.0],
     ])
+    Kmr = torch.zeros(2, 3)
     
     # max velocities (c, p)
     Vmax = torch.tensor([
         [2.1, 1.1, 0.0],
         [1.9, 0.0, 0.0],
     ])
 
     # allosterics (c, p, s)
     A = torch.zeros(2, 3, 4)
 
-    # reaction energies (c, p)
-    E = torch.full((2, 3), -99999.9)
-
     # fmt: on
 
-    def mm(x, k, v, n):
-        return v * x**n / (k + x) ** n
+    def mm12(s, p, kf, kb, v):
+        vf = v * (s / kf - p**2 / kb) / (1 + s / kf + p**2 / kb)
+        vb = v * (p**2 / kb - s / kf) / (1 + s / kf + p**2 / kb)
+        return (vf - vb) / 2
+
+    def mm21(s, p, kf, kb, v):
+        vf = v * (s**2 / kf - p / kb) / (1 + s**2 / kf + p / kb)
+        vb = v * (p / kb - s**2 / kf) / (1 + s**2 / kf + p / kb)
+        return (vf - vb) / 2
+
+    def mm32(s, p, kf, kb, v):
+        vf = v * (s**3 / kf - p**2 / kb) / (1 + s**3 / kf + p**2 / kb)
+        vb = v * (p**2 / kb - s**3 / kf) / (1 + s**3 / kf + p**2 / kb)
+        return (vf - vb) / 2
 
     # expected outcome
-    dx_c0_b = 2 * mm(x=X0[0, 0], v=Vmax[0, 0], k=Km[0, 0, 0], n=1)
-    dx_c0_a = -dx_c0_b / 2
-    dx_c0_d = mm(x=X0[0, 2], v=Vmax[0, 1], k=Km[0, 1, 2], n=2)
-    dx_c0_c = -2 * dx_c0_d
+    v_c0_0 = mm12(X0[0, 0], X0[0, 1], Kmf[0, 0], Kmb[0, 0], Vmax[0, 0])
+    v_c0_1 = mm21(X0[0, 2], X0[0, 3], Kmf[0, 1], Kmb[0, 1], Vmax[0, 1])
+    dx_c0_a = -v_c0_0
+    dx_c0_b = 2 * v_c0_0
+    dx_c0_c = -2 * v_c0_1
+    dx_c0_d = v_c0_1
 
-    v0_c1 = mm(x=X0[1, 1], v=Vmax[1, 0], k=Km[1, 0, 1], n=3)
+    v_c1_0 = mm32(X0[1, 1], X0[1, 2], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0])
     dx_c1_a = 0.0
-    dx_c1_b = -3 * v0_c1
-    dx_c1_c = 2 * v0_c1
+    dx_c1_b = -3 * v_c1_0
+    dx_c1_c = 2 * v_c1_0
     dx_c1_d = 0.0
 
     # test
     kinetics = get_kinetics()
     kinetics.N = N
-    kinetics.Km = Km
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
-    kinetics.E = E
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
     assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
     assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
     assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
     assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
@@ -939,15 +855,15 @@
     assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
     assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
     assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
 
 
 def test_mm_kinetic_with_multiple_substrates():
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
-    # cell 0: P0: a,b -> c, P1: b,d -> a2,c
+    # cell 0: P0: a,b -> c, P1: b,d -> 2a,c
     # cell 1: P0: a,d -> b
 
     # fmt: off
 
     # concentrations (c, s)
     X0 = torch.tensor([
         [1.1, 2.1, 2.9, 0.8],
@@ -959,61 +875,182 @@
         [   [-1.0, -1.0, 1.0, 0.0],
             [2.0, -1.0, 1.0, -1.0],
             [0.0, 0.0, 0.0, 0.0]    ],
         [   [-1.0, 1.0, 0.0, -1.0],
             [0.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 0.0, 0.0]    ],
     ])
+    Nf = torch.where(N < 0.0, -N, 0.0)
+    Nb = torch.where(N > 0.0, N, 0.0)
 
     # affinities (c, p, s)
-    Km = torch.tensor([
-        [   [2.2, 1.2, 0.2, 0.0],
-            [0.8, 1.9, 0.4, 1.2],
-            [0.0, 0.0, 0.0, 0.0] ],
-        [   [2.3, 0.2, 0.0, 1.2],
-            [0.0, 0.0, 0.0, 0.0],
-            [0.0, 0.0, 0.0, 0.0] ],
+    Kmf = torch.tensor([
+        [1.3, 2.1, 0.0],
+        [1.4, 0.0, 0.0],
+    ])
+    Kmb = torch.tensor([
+        [0.3, 1.1, 0.0],
+        [1.5, 0.0, 0.0],
     ])
+    Kmr = torch.zeros(2, 3)
 
     # max velocities (c, p)
     Vmax = torch.tensor([
         [2.1, 1.1, 0.0],
         [1.2, 0.0, 0.0],
     ])
 
     # allosterics (c, p, s)
     A = torch.zeros(2, 3, 4)
 
-    # reaction energies (c, p)
-    E = torch.full((2, 3), -99999.9)
+    # fmt: on
+
+    def mm111(s1, s2, p, kf, kb, v):
+        vf = v * (s1 * s2 / kf - p / kb) / (1 + s1 * s2 / kf + p / kb)
+        vb = v * (p / kb - s1 * s2 / kf) / (1 + s1 * s2 / kf + p / kb)
+        return (vf - vb) / 2
+
+    def mm1121(s1, s2, p1, p2, kf, kb, v):
+        base = 1 + s1 * s2 / kf + p1**2 * p2 / kb
+        vf = v * (s1 * s2 / kf - p1**2 * p2 / kb) / base
+        vb = v * (p1**2 * p2 / kb - s1 * s2 / kf) / base
+        return (vf - vb) / 2
+
+    # expected outcome
+    v_c0_0 = mm111(X0[0, 0], X0[0, 1], X0[0, 2], Kmf[0, 0], Kmb[0, 0], Vmax[0, 0])
+    v_c0_1 = mm1121(
+        X0[0, 1], X0[0, 3], X0[0, 0], X0[0, 2], Kmf[0, 1], Kmb[0, 1], Vmax[0, 1]
+    )
+    dx_c0_a = -v_c0_0 + 2 * v_c0_1
+    dx_c0_b = -v_c0_0 + -v_c0_1
+    dx_c0_c = v_c0_0 + v_c0_1
+    dx_c0_d = -v_c0_1
+
+    v_c1_0 = mm111(X0[1, 0], X0[1, 3], X0[1, 1], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0])
+    dx_c1_a = -v_c1_0
+    dx_c1_b = v_c1_0
+    dx_c1_c = 0.0
+    dx_c1_d = -v_c1_0
+
+    # test
+    kinetics = get_kinetics()
+    kinetics.N = N
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
+    kinetics.Vmax = Vmax
+    kinetics.A = A
+    Xd = kinetics.integrate_signals(X=X0) - X0
+
+    assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
+    assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
+    assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
+    assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
+
+    assert (Xd[1, 0] - dx_c1_a).abs() < TOLERANCE
+    assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
+    assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
+    assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
+
+
+def test_mm_kinetic_with_cofactors():
+    # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
+    # N for a molecule might be 0 but it's still required
+    # cell 0: P0: a -> b | b -> c
+    # cell 0: P1: a + c -> b + c
+
+    # fmt: off
+
+    # concentrations (c, s)
+    X0 = torch.tensor([
+        [10.0, 0.1, 3.0, 0.8],
+        [10.0, 3.0, 0.1, 0.0],
+    ])
+
+    # reactions (c, p, s)
+    N = torch.tensor([
+        [   [-1.0, 0.0, 1.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0]    ],
+        [   [-1.0, 1.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0]    ],
+    ])
+    Nf = torch.tensor([
+        [   [1.0, 1.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0]    ],
+        [   [1.0, 0.0, 1.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0]    ],
+    ])
+    Nb = torch.tensor([
+        [   [0.0, 1.0, 1.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0]    ],
+        [   [0.0, 1.0, 1.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0]    ],
+    ])
+
+    # affinities (c, p)
+    Kmf = torch.tensor([
+        [2.0, 0.0, 0.0],
+        [2.0, 0.0, 0.0],
+    ])
+    Kmb = torch.tensor([
+        [1.0, 0.0, 0.0],
+        [1.0, 0.0, 0.0],
+    ])
+    Kmr = torch.zeros(2, 3)
+
+    # max velocities (c, p)
+    Vmax = torch.tensor([
+        [1.0, 0.0, 0.0],
+        [1.0, 0.0, 0.0],
+    ])
+
+    # allosterics (c, p, s)
+    A = torch.zeros(2, 3, 4)
 
     # fmt: on
 
-    def mm(x1, x2, k1, k2, v):
-        return v * x1 * x2 / ((k1 + x1) * (k2 + x2))
+    def mm(s1, s2, p1, p2, kf, kb, v):
+        vf = v * (s1 * s2 / kf - p1 * p2 / kb) / (1 + s1 * s2 / kf + p1 * p2 / kb)
+        vb = v * (p1 * p2 / kb - s1 * s2 / kf) / (1 + s1 * s2 / kf + p1 * p2 / kb)
+        return (vf - vb) / 2
 
     # expected outcome
-    c0_v0 = mm(x1=X0[0, 0], k1=Km[0, 0, 0], x2=X0[0, 1], k2=Km[0, 0, 1], v=Vmax[0, 0])
-    c0_v1 = mm(x1=X0[0, 1], k1=Km[0, 1, 1], x2=X0[0, 3], k2=Km[0, 1, 3], v=Vmax[0, 1])
-    dx_c0_a = 2 * c0_v1 - c0_v0
-    dx_c0_b = -c0_v0 - c0_v1
-    dx_c0_c = c0_v0 + c0_v1
-    dx_c0_d = -c0_v1
-    c1_v0 = mm(x1=X0[1, 0], k1=Km[1, 0, 0], x2=X0[1, 3], k2=Km[1, 0, 3], v=Vmax[1, 0])
-    dx_c1_a = -c1_v0
-    dx_c1_b = c1_v0
+    v_c0_0 = mm(
+        X0[0, 0], X0[0, 1], X0[0, 1], X0[0, 2], Kmf[0, 0], Kmb[0, 0], Vmax[0, 0]
+    )
+    dx_c0_a = -v_c0_0
+    dx_c0_b = 0.0
+    dx_c0_c = v_c0_0
+    dx_c0_d = 0.0
+
+    v_c1_0 = mm(
+        X0[1, 0], X0[1, 2], X0[1, 1], X0[1, 2], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0]
+    )
+    dx_c1_a = -v_c1_0
+    dx_c1_b = v_c1_0
     dx_c1_c = 0.0
-    dx_c1_d = -c1_v0
+    dx_c1_d = 0.0
 
     # test
     kinetics = get_kinetics()
     kinetics.N = N
-    kinetics.Km = Km
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
-    kinetics.E = E
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
     assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
     assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
     assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
     assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
@@ -1022,15 +1059,15 @@
     assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
     assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
     assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
 
 
 def test_mm_kinetic_with_allosteric_action():
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
-    # cell 0: P0: a -> b, inhibitor=c, P1: c -> d, activator=a, P3: a -> b, inh=c, act=d
+    # cell 0: P0: a -> b, inhibitor=c, P1: c -> d, activator=a, P2: a -> b, inh=c, act=d
     # cell 1: P0: a -> b, inhibitor=c,d, P1: c -> d, activator=a,b
 
     # fmt: off
 
     # concentrations (c, s)
     X0 = torch.tensor([
         [2.1, 3.5, 1.9, 2.0],
@@ -1042,23 +1079,29 @@
         [   [-1.0, 1.0, 0.0, 0.0],
             [0.0, 0.0, -1.0, 1.0],
             [-1.0, 1.0, 0.0, 0.0]   ],
         [   [-1.0, 1.0, 0.0, 0.0],
             [0.0, 0.0, -1.0, 1.0],
             [0.0, 0.0, 0.0, 0.0]   ],
     ])
+    Nf = torch.where(N < 0.0, -N, 0.0)
+    Nb = torch.where(N > 0.0, N, 0.0)
 
     # affinities (c, p, s)
-    Km = torch.tensor([
-        [   [1.2, 3.1, 0.7, 0.0],
-            [1.0, 0.0, 0.9, 1.2],
-            [1.0, 0.1, 1.0, 1.0] ],
-        [   [2.1, 1.3, 1.0, 0.6],
-            [1.3, 0.8, 0.3, 1.1],
-            [0.0, 0.0, 0.0, 0.0] ],
+    Kmf = torch.tensor([
+        [1.3, 2.1, 0.9],
+        [1.4, 2.2, 0.0],
+    ])
+    Kmb = torch.tensor([
+        [1.1, 1.1, 1.0],
+        [1.5, 1.9, 0.0],
+    ])
+    Kmr = torch.tensor([
+        [1.3, 2.1, 0.9],
+        [1.4, 2.2, 0.0],
     ])
 
     # max velocities (c, p)
     Vmax = torch.tensor([
         [2.1, 2.0, 1.0],
         [3.2, 2.5, 0.0],
     ])
@@ -1069,71 +1112,69 @@
             [1.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, -1.0, 1.0]   ],
         [   [0.0, 0.0, -1.0, -1.0],
             [1.0, 1.0, 0.0, 0.0],
             [0.0, 0.0, 0.0, 0.0]   ],
     ])
 
-    # reaction energies (c, p)
-    E = torch.full((2, 3), -99999.9)
-
     # fmt: on
 
-    def mm(x, kx, v):
-        return v * x / (kx + x)
+    def mm(s, p, kf, kb, v):
+        vf = v * (s / kf - p / kb) / (1 + s / kf + p / kb)
+        vb = v * (p / kb - s / kf) / (1 + s / kf + p / kb)
+        return (vf - vb) / 2
 
     def fi(i, ki):
         return 1 - i / (ki + i)
 
-    def fi2(i1, ki1, i2, ki2):
-        return max(0, 1 - i1 * i2 / ((ki1 + i1) * (ki2 + i2)))
+    def fi2(i1, i2, ki):
+        return max(0, 1 - i1 * i2 / (ki + i1 * i2))
 
     def fa(a, ka):
         return a / (ka + a)
 
-    def fa2(a1, ka1, a2, ka2):
-        return min(1, a1 * a2 / ((ka1 + a1) * (ka2 + a2)))
+    def fa2(a1, a2, ka):
+        return min(1, a1 * a2 / (ka + a1 * a2))
 
     # expected outcome
-    v0_c0 = mm(x=X0[0, 0], v=Vmax[0, 0], kx=Km[0, 0, 0]) * fi(
-        i=X0[0, 2], ki=Km[0, 0, 2]
-    )
-    v1_c0 = mm(x=X0[0, 2], v=Vmax[0, 1], kx=Km[0, 1, 2]) * fa(
-        a=X0[0, 0], ka=Km[0, 1, 0]
+    v_c0_0 = mm(X0[0, 0], X0[0, 1], Kmf[0, 0], Kmb[0, 0], Vmax[0, 0]) * fi(
+        X0[0, 2], Kmr[0, 0]
     )
-    v2_c0 = (
-        mm(x=X0[0, 0], v=Vmax[0, 2], kx=Km[0, 2, 0])
-        * fi(i=X0[0, 2], ki=Km[0, 2, 2])
-        * fa(a=X0[0, 3], ka=Km[0, 2, 3])
+    v_c0_1 = mm(X0[0, 2], X0[0, 3], Kmf[0, 1], Kmb[0, 1], Vmax[0, 1]) * fa(
+        X0[0, 0], Kmr[0, 1]
     )
-    dx_c0_b = v0_c0 + v2_c0
-    dx_c0_a = -v0_c0 - v2_c0
-    dx_c0_c = -v1_c0
-    dx_c0_d = v1_c0
-
-    v0_c1 = mm(x=X0[1, 0], v=Vmax[1, 0], kx=Km[1, 0, 0]) * fi2(
-        i1=X0[1, 2], ki1=Km[1, 0, 2], i2=X0[1, 3], ki2=Km[1, 0, 3]
+    v_c0_2 = (
+        mm(X0[0, 0], X0[0, 1], Kmf[0, 2], Kmb[0, 2], Vmax[0, 2])
+        * fi(X0[0, 2], Kmr[0, 2])
+        * fa(X0[0, 3], Kmr[0, 2])
     )
-    v1_c1 = mm(x=X0[1, 2], v=Vmax[1, 1], kx=Km[1, 1, 2]) * fa2(
-        a1=X0[1, 0],
-        ka1=Km[1, 1, 0],
-        a2=X0[1, 1],
-        ka2=Km[1, 1, 1],
+    dx_c0_a = -v_c0_0 - v_c0_2
+    dx_c0_b = v_c0_0 + v_c0_2
+    dx_c0_c = -v_c0_1
+    dx_c0_d = v_c0_1
+
+    i_c1_0 = fi2(X0[1, 2], X0[1, 3], Kmr[1, 0])
+    v_c1_0 = mm(X0[1, 0], X0[1, 1], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0]) * i_c1_0
+    v_c1_1 = mm(X0[1, 2], X0[1, 3], Kmf[1, 1], Kmb[1, 1], Vmax[1, 1]) * fa2(
+        X0[1, 0], X0[1, 1], Kmr[1, 1]
     )
-    dx_c1_a = -v0_c1
-    dx_c1_b = v0_c1
-    dx_c1_c = -v1_c1
-    dx_c1_d = v1_c1
+    dx_c1_a = -v_c1_0
+    dx_c1_b = v_c1_0
+    dx_c1_c = -v_c1_1
+    dx_c1_d = v_c1_1
 
     # test
     kinetics = get_kinetics()
     kinetics.N = N
-    kinetics.Km = Km
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
-    kinetics.E = E
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
     assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
     assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
     assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
     assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
@@ -1150,86 +1191,96 @@
     # cell 1: P0: 2c -> d
 
     # fmt: off
 
     # concentrations (c, s)
     X0 = torch.tensor([
         [0.1, 1.0, 2.9, 0.8],
-        [2.9, 3.1, 0.1, 1.0],
+        [2.9, 3.1, 0.1, 0.3],
     ])
 
     # reactions (c, p, s)
     N = torch.tensor([
         [   [-1.0, 1.0, 0.0, 0.0],
             [0.0, -1.0, 0.0, 1.0],
             [0.0, 0.0, 0.0, 0.0]    ],
         [   [0.0, 0.0, -2.0, 1.0],
             [0.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 0.0, 0.0]    ],
     ])
+    Nf = torch.where(N < 0.0, -N, 0.0)
+    Nb = torch.where(N > 0.0, N, 0.0)
 
     # affinities (c, p, s)
-    Km = torch.tensor([
-        [   [1.2, 1.5, 0.0, 0.0],
-            [0.0, 0.5, 0.0, 3.5],
-            [0.0, 0.0, 0.0, 0.0] ],
-        [   [0.0, 0.0, 0.5, 1.5],
-            [0.0, 0.0, 0.0, 0.0],
-            [0.0, 0.0, 0.0, 0.0] ],
+    Kmf = torch.tensor([
+        [0.1, 2.1, 0.0],
+        [0.1, 0.0, 0.0],
+    ])
+    Kmb = torch.tensor([
+        [10.3, 1.1, 0.0],
+        [10.5, 0.0, 0.0],
     ])
+    Kmr = torch.zeros(2, 3)
 
     # max velocities (c, p)
     Vmax = torch.tensor([
         [2.1, 1.0, 0.0],
         [3.1, 0.0, 0.0],
     ])
 
     # allosterics (c, p, s)
     A = torch.zeros(2, 3, 4)
 
-    # reaction energies (c, p)
-    E = torch.full((2, 3), -99999.9)
-
     # fmt: on
 
-    def mm(x, k, v, n=1):
-        return v * x**n / (k + x) ** n
+    def mm(s, p, kf, kb, v):
+        vf = v * (s / kf - p / kb) / (1 + s / kf + p / kb)
+        vb = v * (p / kb - s / kf) / (1 + s / kf + p / kb)
+        return (vf - vb) / 2
+
+    def mm21(s, p, kf, kb, v):
+        vf = v * (s**2 / kf - p / kb) / (1 + s**2 / kf + p / kb)
+        vb = v * (p / kb - s**2 / kf) / (1 + s**2 / kf + p / kb)
+        return (vf - vb) / 2
 
     # expected outcome
-    v0_c0 = mm(x=X0[0, 0], v=Vmax[0, 0], k=Km[0, 0, 0])
-    v1_c0 = mm(x=X0[0, 1], v=Vmax[0, 1], k=Km[0, 1, 1])
+    v_c0_0 = mm(X0[0, 0], X0[0, 1], Kmf[0, 0], Kmb[0, 0], Vmax[0, 0])
+    v_c0_1 = mm(X0[0, 1], X0[0, 3], Kmf[0, 1], Kmb[0, 1], Vmax[0, 1])
     # but this would lead to Xd + X0 = -0.0615 (for a)
-    assert X0[0, 0] - v0_c0 < 0.0
+    assert X0[0, 0] - v_c0_0 < 0.0
     # so velocity should be reduced by a factor depending on current a
     # all other proteins in this cell are reduce by the same factor
     # to avoid follow up problems with other molecules being destroyed by other proteins
-    f = X0[0, 0] * 0.99 / v0_c0
-    v0_c0 = f * v0_c0
-    v1_c1 = f * v1_c0
-    dx_c0_a = -v0_c0
-    dx_c0_b = v0_c0 - v1_c1
+    f = (X0[0, 0] - EPS) / v_c0_0
+    v_c0_0 = f * v_c0_0
+    v_c0_1 = f * v_c0_1
+    dx_c0_a = -v_c0_0
+    dx_c0_b = v_c0_0 - v_c0_1
     dx_c0_c = 0.0
-    dx_c0_d = v1_c1
+    dx_c0_d = v_c0_1
 
-    v0_c1 = mm(x=X0[1, 2], v=Vmax[1, 0], k=Km[1, 0, 2], n=2)
+    v_c1_0 = mm21(X0[1, 2], X0[1, 3], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0])
     # but this would lead to Xd + X0 = -0.0722 (for c)
-    assert X0[1, 2] - 2 * v0_c1 < 0.0
+    assert X0[1, 2] - 2 * v_c1_0 < 0.0
     # as above, velocities are reduced. here its only this protein
-    v0_c1 = X0[1, 2] * 0.99 / 2
+    v_c1_0 = (X0[1, 2] - EPS) / 2
     dx_c1_a = 0.0
     dx_c1_b = 0.0
-    dx_c1_c = -2 * v0_c1
-    dx_c1_d = v0_c1
+    dx_c1_c = -2 * v_c1_0
+    dx_c1_d = v_c1_0
 
     # test
     kinetics = get_kinetics()
     kinetics.N = N
-    kinetics.Km = Km
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
-    kinetics.E = E
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
     assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
     assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
     assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
     assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
@@ -1261,71 +1312,84 @@
         [   [-1.0, 1.0, 0.0, 0.0],
             [-2.0, 0.0, 0.0, 1.0],
             [0.0, 0.0, 0.0, 0.0]    ],
         [   [-1.0, 1.0, 0.0, 0.0],
             [0.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 0.0, 0.0]    ],
     ])
+    Nf = torch.where(N < 0.0, -N, 0.0)
+    Nb = torch.where(N > 0.0, N, 0.0)
 
     # affinities (c, p, s)
-    Km = torch.tensor([
-        [   [0.5, 1.5, 0.0, 0.0],
-            [0.5, 0.0, 0.0, 3.5],
-            [0.0, 0.0, 0.0, 0.0] ],
-        [   [0.5, 1.5, 0.0, 0.0],
-            [0.0, 0.0, 0.0, 0.0],
-            [0.0, 0.0, 0.0, 0.0] ],
+    Kmf = torch.tensor([
+        [0.1, 2.1, 0.0],
+        [0.1, 0.0, 0.0],
+    ])
+    Kmb = torch.tensor([
+        [10.3, 1.1, 0.0],
+        [1.5, 0.0, 0.0],
     ])
+    Kmr = torch.zeros(2, 3)
 
     # max velocities (c, p)
     Vmax = torch.tensor([
         [3.1, 2.0, 0.0],
         [3.1, 0.0, 0.0],
     ])
 
     # allosterics (c, p, s)
     A = torch.zeros(2, 3, 4)
 
     # reaction energies (c, p)
-    E = torch.full((2, 3), -99999.9)
+    torch.full((2, 3), -99999.9)
 
     # fmt: on
 
-    def mm(x, k, v, n=1):
-        return v * x**n / (k + x) ** n
+    def mm(s, p, kf, kb, v):
+        vf = v * (s / kf - p / kb) / (1 + s / kf + p / kb)
+        vb = v * (p / kb - s / kf) / (1 + s / kf + p / kb)
+        return (vf - vb) / 2
+
+    def mm21(s, p, kf, kb, v):
+        vf = v * (s**2 / kf - p / kb) / (1 + s**2 / kf + p / kb)
+        vb = v * (p / kb - s**2 / kf) / (1 + s**2 / kf + p / kb)
+        return (vf - vb) / 2
 
     # expected outcome
-    v0_c0 = mm(x=X0[0, 0], v=Vmax[0, 0], k=Km[0, 0, 0])
-    v1_c0 = mm(x=X0[0, 0], v=Vmax[0, 1], k=Km[0, 1, 0], n=2)
+    v_c0_0 = mm(X0[0, 0], X0[0, 1], Kmf[0, 0], Kmb[0, 0], Vmax[0, 0])
+    v_c0_1 = mm21(X0[0, 0], X0[0, 3], Kmf[0, 1], Kmb[0, 1], Vmax[0, 1])
     # but this would lead to a < 0.0
-    naive_dx_c0_a = -v0_c0 - 2 * v1_c0
+    naive_dx_c0_a = -v_c0_0 - 2 * v_c0_1
     assert X0[0, 0] + naive_dx_c0_a < 0.0
     # so velocity should be reduced to by a factor to not deconstruct too much a
     # all other proteins have to be reduced by the same factor to not cause downstream problems
-    f = X0[0, 0] * 0.99 / -naive_dx_c0_a
-    v0_c0 = v0_c0 * f
-    v1_c0 = v1_c0 * f
-    dx_c0_a = -v0_c0 - v1_c0 * 2
-    dx_c0_b = v0_c0
+    f = (X0[0, 0] - EPS) / -naive_dx_c0_a
+    v_c0_0 = v_c0_0 * f
+    v_c0_1 = v_c0_1 * f
+    dx_c0_a = -v_c0_0 - v_c0_1 * 2
+    dx_c0_b = v_c0_0
     dx_c0_c = 0.0
-    dx_c0_d = v1_c0
+    dx_c0_d = v_c0_1
 
     # cell1 is business as usual
-    v0_c0 = mm(x=X0[1, 0], v=Vmax[1, 0], k=Km[1, 0, 0])
-    dx_c1_a = -v0_c0
-    dx_c1_b = v0_c0
+    v_c1_0 = mm(X0[1, 0], X0[1, 1], Kmf[1, 0], Kmb[1, 0], Vmax[1, 0])
+    dx_c1_a = -v_c1_0
+    dx_c1_b = v_c1_0
     dx_c1_c = 0.0
     dx_c1_d = 0.0
 
     # test
     kinetics = get_kinetics()
     kinetics.N = N
-    kinetics.Km = Km
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
     kinetics.Vmax = Vmax
-    kinetics.E = E
     kinetics.A = A
     Xd = kinetics.integrate_signals(X=X0) - X0
 
     assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
     assert (Xd[0, 1] - dx_c0_b).abs() < TOLERANCE
     assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
     assert (Xd[0, 3] - dx_c0_d).abs() < TOLERANCE
@@ -1335,134 +1399,155 @@
     assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
     assert (Xd[1, 3] - dx_c1_d).abs() < TOLERANCE
 
     X1 = X0 + Xd
     assert not torch.any(X1 < 0.0)
 
 
-def test_equilibrium_constants():
+def test_equilibrium_is_reached():
+    # molecules should reach equilibrium after a few steps
+    # with Vmax > 1.0 higher order reactions cant reach equilibrium
+    # because they overshoot
+
     # 2 cell, 3 max proteins, 4 molecules (a, b, c, d)
-    # cell 0: P0: a -> b (but b/a > Ke), P1: b -> d (but Q almost Ke)
-    # cell 1: P0: c -> d (but Q ~= Ke), P1: a -> d (but d/a > Ke, and Q almost Ke)
+    # cell 0: P0: a -> b (Ke=1.0), P1: c -> d (Ke=20.0)
+    # cell 1: P0: a,2b -> c (Ke=10.0)
 
     # fmt: off
 
     # concentrations (c, s)
     X0 = torch.tensor([
-        [2.0, 20.0, 2.9, 20.0],
-        [1.0, 3.1, 1.3, 2.9],
+        [2.0, 20.0, 5.0, 5.0],
+        [2.0, 3.1, 1.3, 2.9],
     ])
 
     # reactions (c, p, s)
     N = torch.tensor([
         [   [-1.0, 1.0, 0.0, 0.0],
-            [0.0, -1.0, 0.0, 1.0],
+            [0.0, 0.0, -1.0, 1.0],
             [0.0, 0.0, 0.0, 0.0]    ],
-        [   [0.0, 0.0, -1.0, 1.0],
-            [-1.0, 0.0, 0.0, 1.0],
+        [   [-1.0, -2.0, 1.0, 0.0],
+            [0.0, 0.0, 0.0, 0.0],
             [0.0, 0.0, 0.0, 0.0]    ],
     ])
+    Nf = torch.where(N < 0.0, -N, 0.0)
+    Nb = torch.where(N > 0.0, N, 0.0)
 
-    # affinities (c, p, s)
-    Km = torch.tensor([
-        [   [1.2, 1.5, 0.0, 0.0],
-            [0.0, 0.5, 0.0, 3.5],
-            [0.0, 0.0, 0.0, 0.0] ],
-        [   [0.0, 0.0, 0.5, 1.5],
-            [1.2, 0.0, 0.0, 1.9],
-            [0.0, 0.0, 0.0, 0.0] ],
+    # affinities (c, p)
+    Kmf = torch.tensor([
+        [1.0, 1.0, 0.0],
+        [1.0, 0.0, 0.0],
+    ])
+    Kmb = torch.tensor([
+        [1.0, 20.0, 0.0],
+        [10.0, 0.0, 0.0],
     ])
+    Kmr = torch.zeros(2, 3)
 
     # max velocities (c, p)
     Vmax = torch.tensor([
-        [2.1, 4.0, 0.0],
-        [1.1, 3.0, 0.0],
+        [100.0, 100.0, 0.0],
+        [100.0, 0.0, 0.0],
     ])
 
     # allosterics (c, p, s)
     A = torch.zeros(2, 3, 4)
 
-    # reaction energies (c, p)
-    E = torch.full((2, 3), -99999.9)
-    # E = -2000 ^= # ln(Ke) = 0.77
-    E[0, 0] = -2000 # ln(Q) - ln(Ke) = 1.53 (switch N)
-    E[0, 1] = -2000 # ln(Q) - ln(Ke) = -0.76 (reduce V)
-    E[1, 0] = -2000 # ln(Q) - ln(Ke) = 0.02 (switch off)
-    E[1, 1] = -2000 # ln(Q) - ln(Ke) = 0.28 (switch N, reduce V)
-
-    # fmt: on
+    # test
+    kinetics = get_kinetics(n_computations=11)
+    kinetics.N = N
+    kinetics.Nf = Nf
+    kinetics.Nb = Nb
+    kinetics.Kmf = Kmf
+    kinetics.Kmb = Kmb
+    kinetics.Kmr = Kmr
+    kinetics.Vmax = Vmax
+    kinetics.A = A
 
-    def mm(x, k, v):
-        return v * x / (k + x)
+    for _ in range(10):
+        X0 = kinetics.integrate_signals(X=X0)
 
-    # expected outcome
-    # v0 is turned around, v1 is reduced by a factor of around 0.37
-    v0_c0 = mm(x=X0[0, 1], v=Vmax[0, 0], k=Km[0, 0, 1]) * -1.0
-    v1_c0 = mm(x=X0[0, 1], v=Vmax[0, 1], k=Km[0, 1, 1]) * 0.76
-    dx_c0_a = -v0_c0
-    dx_c0_b = v0_c0 - v1_c0
-    dx_c0_c = 0.0
-    dx_c0_d = v1_c0
+    q_c0_0 = X0[0, 1] / X0[0, 0]
+    q_c0_1 = X0[0, 3] / X0[0, 2]
+    q_c1_0 = X0[1, 2] / (X0[1, 0] * X0[1, 1] * X0[1, 1])
+
+    assert (q_c0_0 - 1.0).abs() < 0.1
+    assert (q_c0_1 - 20.0).abs() < 2.0
+    assert (q_c1_0 - 10.0).abs() < 1.0
+
+
+def test_zero_substrates_stay_zero():
+    # Typical reasons for cells creating signals from 0:
+    # 1. when using exp(ln(x)) 1s can accidentally be created
+    # 2. when doing a^b 1s can be created (0^1=0 but 0^0=1)
 
-    # v0 is switched off, v1 is reduced by 0.28 and turned around
-    v0_c1 = 0.0
-    v1_c1 = mm(x=X0[1, 3], v=Vmax[1, 1], k=Km[1, 1, 3]) * -0.28
-    dx_c1_a = -v1_c1
-    dx_c1_b = 0.0
-    dx_c1_c = -v0_c1
-    dx_c1_d = v0_c1 + v1_c1
+    n_cells = 100
+    n_prots = 100
+    n_steps = 100
 
-    # test
     kinetics = get_kinetics()
-    kinetics.N = N
-    kinetics.Km = Km
-    kinetics.Vmax = Vmax
-    kinetics.E = E
-    kinetics.A = A
-    Xd = kinetics.integrate_signals(X=X0) - X0
+    n_mols = len(MOLECULES) * 2
 
-    tolerance = 1e-1  # floating point problems
-    assert (Xd[0, 0] - dx_c0_a).abs() < TOLERANCE
-    assert (Xd[0, 1] - dx_c0_b).abs() < tolerance
-    assert (Xd[0, 2] - dx_c0_c).abs() < TOLERANCE
-    assert (Xd[0, 3] - dx_c0_d).abs() < tolerance
+    # concentrations (c, s)
+    X = torch.zeros(n_cells, n_mols).abs()
 
-    assert (Xd[1, 0] - dx_c1_a).abs() < tolerance
-    assert (Xd[1, 1] - dx_c1_b).abs() < TOLERANCE
-    assert (Xd[1, 2] - dx_c1_c).abs() < TOLERANCE
-    assert (Xd[1, 3] - dx_c1_d).abs() < tolerance
+    # reactions (c, p, s)
+    kinetics.N = torch.randint(low=-3, high=4, size=(n_cells, n_prots, n_mols)).float()
+    kinetics.Nf = torch.where(kinetics.N < 0.0, -kinetics.N, 0.0)
+    kinetics.Nb = torch.where(kinetics.N > 0.0, kinetics.N, 0.0)
+
+    # max velocities (c, p)
+    kinetics.Vmax = torch.randn(n_cells, n_prots).abs() * 100
+
+    # allosterics (c, p, s)
+    kinetics.A = torch.randint(low=-2, high=3, size=(n_cells, n_prots, n_mols))
 
+    # affinities (c, p)
+    Ke = torch.randn(n_cells, n_prots)
+    kinetics.Kmf = torch.randn(n_cells, n_prots).abs()
+    kinetics.Kmb = kinetics.Kmf * Ke
+    kinetics.Kmr = torch.randn(n_cells, n_prots).abs()
 
-@pytest.mark.parametrize("gen", [torch.zeros, torch.randn])
-def test_substrate_concentrations_are_always_finite_and_positive(gen):
+    # test
+    for _ in range(n_steps):
+        X = kinetics.integrate_signals(X=X)
+        assert X.min() == 0.0
+        assert X.max() == 0.0
+
+
+def test_substrate_concentrations_are_always_finite_and_positive():
+    # interaction terms can overflow float32 when they become too big
+    # i.g. exponents too high and many substrates
+    # this will create infinites which will eventually become NaN
     n_cells = 100
     n_prots = 100
     n_steps = 100
 
     kinetics = get_kinetics()
     n_mols = len(MOLECULES) * 2
 
     # concentrations (c, s)
-    X = gen(n_cells, n_mols).abs()
+    X = torch.randn(n_cells, n_mols).abs()
 
     # reactions (c, p, s)
-    kinetics.N = torch.randint(low=-3, high=4, size=(n_cells, n_prots, n_mols))
-
-    # affinities (c, p, s)
-    kinetics.Km = torch.randn(n_cells, n_prots, n_mols).abs()
+    kinetics.N = torch.randint(low=-3, high=4, size=(n_cells, n_prots, n_mols)).float()
+    kinetics.Nf = torch.where(kinetics.N < 0.0, -kinetics.N, 0.0)
+    kinetics.Nb = torch.where(kinetics.N > 0.0, kinetics.N, 0.0)
 
     # max velocities (c, p)
-    kinetics.Vmax = torch.randn(n_cells, n_prots).abs() * 10
+    kinetics.Vmax = torch.randn(n_cells, n_prots).abs().clamp(max=1.0) * 100
 
     # allosterics (c, p, s)
     kinetics.A = torch.randint(low=-2, high=3, size=(n_cells, n_prots, n_mols))
 
-    # reaction energies (c, p)
-    kinetics.E = torch.randn(n_cells, n_prots)
+    # affinities (c, p)
+    Ke = torch.randn(n_cells, n_prots)
+    kinetics.Kmf = torch.randn(n_cells, n_prots).abs().clamp(0.001)
+    kinetics.Kmb = (kinetics.Kmf * Ke).clamp(0.001)
+    kinetics.Kmr = torch.randn(n_cells, n_prots).abs().clamp(0.001)
 
     # test
     for _ in range(n_steps):
-        Xd = kinetics.integrate_signals(X=X)
-        X = X + Xd
+        X = kinetics.integrate_signals(X=X)
         assert not torch.any(X < 0.0), X[X < 0.0].min()
         assert not torch.any(X.isnan()), X.isnan().sum()
         assert torch.all(X.isfinite()), ~X.isfinite().sum()
```

### Comparing `magicsoup-0.3.9/tests/test_mutations.py` & `magicsoup-0.4.0/tests/test_mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/tests/test_util.py` & `magicsoup-0.4.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.9/tests/test_world.py` & `magicsoup-0.4.0/tests/test_world.py`

 * *Files 15% similar despite different names*

```diff
@@ -83,14 +83,33 @@
     chemistry = ms.Chemistry(molecules=MOLECULES[:2], reactions=[])
     world = ms.World(chemistry=chemistry, map_size=5)
     old_molmap = world.molecule_map.clone()
 
     genomes = [ms.random_genome(s=500) for _ in range(3)]
     world.add_cells(genomes=genomes)
 
+    assert world.n_cells == 3
+    xs = world.cell_positions[:, 0]
+    ys = world.cell_positions[:, 1]
+    assert torch.all(old_molmap[:, xs, ys] / 2 == world.molecule_map[:, xs, ys])
+    assert torch.all(old_molmap[:, xs, ys] / 2 == world.cell_molecules.T)
+
+    genomes = ["" for _ in range(2)]
+    world.add_cells(genomes=genomes)
+
+    assert world.n_cells == 5
+    xs = world.cell_positions[:, 0]
+    ys = world.cell_positions[:, 1]
+    assert torch.all(old_molmap[:, xs, ys] / 2 == world.molecule_map[:, xs, ys])
+    assert torch.all(old_molmap[:, xs, ys] / 2 == world.cell_molecules.T)
+
+    genomes = [ms.random_genome(100), "", ms.random_genome(100)]
+    world.add_cells(genomes=genomes)
+
+    assert world.n_cells == 8
     xs = world.cell_positions[:, 0]
     ys = world.cell_positions[:, 1]
     assert torch.all(old_molmap[:, xs, ys] / 2 == world.molecule_map[:, xs, ys])
     assert torch.all(old_molmap[:, xs, ys] / 2 == world.cell_molecules.T)
 
 
 def test_divide_cells():
@@ -174,15 +193,15 @@
 
 
 def test_molecule_amount_integrity_during_diffusion():
     chemistry = ms.Chemistry(molecules=MOLECULES, reactions=[])
     world = ms.World(chemistry=chemistry, map_size=128)
 
     exp = world.molecule_map.sum(dim=[1, 2])
-    for step_i in range(1000):
+    for step_i in range(100):
         world.diffuse_molecules()
         res = world.molecule_map.sum(dim=[1, 2])
         assert (res.sum() - exp.sum()).abs() < 10.0, step_i
         assert torch.all(torch.abs(res - exp) < 1.0), step_i
 
 
 def test_molecule_amount_integrity_during_reactions():
@@ -203,15 +222,15 @@
         mij = world.molecule_map[[0, 1]].sum().item()
         mk = world.molecule_map[2].sum().item() * 2
         cij = world.cell_molecules[:, [0, 1]].sum().item()
         ck = world.cell_molecules[:, 2].sum().item() * 2
         return mij + mk + cij + ck
 
     n0 = count(world)
-    for step_i in range(1000):
+    for step_i in range(100):
         world.enzymatic_activity()
         n = count(world)
         assert n == pytest.approx(n0, abs=1.0), step_i
 
 
 def test_run_world_without_reactions():
     chemistry = ms.Chemistry(molecules=MOLECULES[:2], reactions=[])
@@ -380,30 +399,39 @@
         world.generate_genome(proteome=[ms.ProteinFact(domain_facts=doms)], size=100)
 
 
 def test_saving_and_loading_world_obj():
     mi = ms.Molecule("i", 10 * 1e3)
     mj = ms.Molecule("j", 20 * 1e3)
     chemistry = ms.Chemistry(molecules=[mi, mj], reactions=[([mi], [mj])])
-
     world = ms.World(chemistry=chemistry, map_size=7)
+
+    for i, mol in enumerate(chemistry.molecules):
+        assert world.chemistry.mol_2_idx[mol] == i
+        assert world.chemistry.molname_2_idx[mol.name] == i
+
     with tempfile.TemporaryDirectory() as tmpdir:
         rundir = Path(tmpdir)
         world.save(rundir=rundir)
         del world
         world = ms.World.from_file(rundir=rundir)
 
     assert world.abs_temp == 310.0
     assert world.map_size == 7
     assert world.workers == 2
     assert world.genetics.workers == 2
     assert world.device == "cpu"
     assert world.chemistry.molecules[0] is mi
     assert world.chemistry.molecules[1] is mj
     assert world.chemistry.reactions == [([mi], [mj])]
+
+    for i, mol in enumerate(chemistry.molecules):
+        assert world.chemistry.mol_2_idx[mol] == i
+        assert world.chemistry.molname_2_idx[mol.name] == i
+
     del world
 
     world = ms.World(chemistry=chemistry, map_size=9, workers=2, abs_temp=300.0)
     with tempfile.TemporaryDirectory() as tmpdir:
         rundir = Path(tmpdir)
         world.save(rundir=rundir)
         del world
@@ -413,14 +441,19 @@
     assert world.map_size == 9
     assert world.workers == 4
     assert world.genetics.workers == 4
     assert world.device == "cpu"
     assert world.chemistry.molecules[0] is mi
     assert world.chemistry.molecules[1] is mj
     assert world.chemistry.reactions == [([mi], [mj])]
+
+    for i, mol in enumerate(chemistry.molecules):
+        assert world.chemistry.mol_2_idx[mol] == i
+        assert world.chemistry.molname_2_idx[mol.name] == i
+
     del world
 
 
 def test_saving_and_loading_state():
     mi = ms.Molecule("i", 10 * 1e3)
     mj = ms.Molecule("j", 20 * 1e3)
     chemistry = ms.Chemistry(molecules=[mi, mj], reactions=[([mi], [mj])])
@@ -449,34 +482,34 @@
     chemistry = ms.Chemistry(molecules=MOLECULES, reactions=[])
 
     world = ms.World(chemistry=chemistry)
     world.add_cells(genomes=[ms.random_genome(s=500) for _ in range(2)])
     assert world.n_cells == 2
     world.cell_divisions[0] = 1
     world.cell_divisions[1] = 11
-    world.cell_survival[0] = 5
-    world.cell_survival[1] = 15
+    world.cell_lifetimes[0] = 5
+    world.cell_lifetimes[1] = 15
 
     world.divide_cells(cell_idxs=[0])
     assert world.n_cells == 3
     assert world.cell_divisions[0] == 2
     assert world.cell_divisions[1] == 11
     assert world.cell_divisions[2] == 2
-    assert world.cell_survival[0] == 0
-    assert world.cell_survival[1] == 15
-    assert world.cell_survival[2] == 0
+    assert world.cell_lifetimes[0] == 0
+    assert world.cell_lifetimes[1] == 15
+    assert world.cell_lifetimes[2] == 0
 
-    world.increment_cell_survival()
+    world.increment_cell_lifetimes()
     assert world.n_cells == 3
     assert world.cell_divisions[0] == 2
     assert world.cell_divisions[1] == 11
     assert world.cell_divisions[2] == 2
-    assert world.cell_survival[0] == 1
-    assert world.cell_survival[1] == 16
-    assert world.cell_survival[2] == 1
+    assert world.cell_lifetimes[0] == 1
+    assert world.cell_lifetimes[1] == 16
+    assert world.cell_lifetimes[2] == 1
 
 
 def test_reference_to_tensors_not_lost():
     class A:
         def __init__(self, world: ms.World):
             self.world = world
 
@@ -548,18 +581,20 @@
 def test_change_genomes():
     chemistry = ms.Chemistry(molecules=MOLECULES, reactions=[])
     world = ms.World(chemistry=chemistry)
 
     g0 = ms.random_genome(s=500)
     world.add_cells(genomes=[g0] * 2)
     assert world.genomes == [g0] * 2
+    assert (world.kinetics.N[0] == world.kinetics.N[1]).all()
 
     g1 = ms.random_genome(s=1000)
     world.add_cells(genomes=[g1])
     assert world.genomes == [g0] * 2 + [g1]
+    assert (world.kinetics.N[0] == world.kinetics.N[1]).all()
 
     g2 = ms.random_genome(s=600)
     world.update_cells(genome_idx_pairs=[(g2, 1)])
     assert world.genomes == [g0, g2, g1]
 
     world.kill_cells(cell_idxs=[0])
     assert world.genomes == [g2, g1]
@@ -567,7 +602,128 @@
     g3 = ms.random_genome(s=700)
     world.update_cells(genome_idx_pairs=[(g3, 1)])
     assert world.genomes == [g2, g3]
 
     g4 = ms.random_genome(s=500)
     world.add_cells(genomes=[g4])
     assert world.genomes == [g2, g3, g4]
+
+    g5 = ""
+    world.update_cells(genome_idx_pairs=[(g4, 0), (g5, 1), (g4, 2)])
+    assert world.genomes == [g4, g5, g4]
+    assert (world.kinetics.N[0] == world.kinetics.N[2]).all()
+    assert (world.kinetics.N[1] == 0.0).all()
+
+    world.update_cells(genome_idx_pairs=[(g5, 0), (g5, 1), (g5, 2)])
+    assert world.genomes == [g5, g5, g5]
+    assert (world.kinetics.N[0] == 0.0).all()
+    assert (world.kinetics.N[1] == 0.0).all()
+    assert (world.kinetics.N[2] == 0.0).all()
+
+
+def test_get_neighbours():
+    chemistry = ms.Chemistry(molecules=MOLECULES, reactions=[])
+    world = ms.World(chemistry=chemistry, map_size=9)
+
+    # fmt: off
+    world.cell_map = torch.tensor([
+        [0, 1, 0, 0, 0, 0, 0, 0, 1],
+        [0, 1, 1, 0, 0, 0, 0, 0, 0],
+        [1, 1, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 0, 0, 0],
+        [0, 0, 0, 0, 0, 0, 1, 1, 1]
+    ]).bool()
+    
+    world.cell_positions = torch.tensor([
+        [1, 1],  # 0
+        [1, 2],  # 1
+        [0, 1],  # 2
+        [2, 1],  # 3
+        [8, 8],  # 4
+        [0, 8],  # 5
+        [2, 0],  # 6
+        [8, 6],  # 7
+        [8, 7],  # 8
+    ])
+
+    # always sorted lower idx first
+    nghbrs = [
+        {(0, 2), (0, 1), (0, 6), (0, 3)},  # 0
+        {(1, 2), (0, 1), (1, 3)},  # 1
+        {(0, 2), (1, 2)},  # 2
+        {(0, 3), (1, 3), (3, 6)},  # 3
+        {(4, 8), (4, 5)},  # 4
+        {(5, 8), (4, 5)},  # 5
+        {(0, 6), (3, 6)},  # 6
+        {(7, 8)},  # 7
+        {(7, 8), (4, 8), (5, 8)},  # 8
+    ]
+    # fmt: on
+
+    for idx, exp in enumerate(nghbrs):
+        res = world.get_neighbors(cell_idxs=[idx])
+        assert len(res) == len(exp), idx
+        assert set(res) == exp, idx
+
+        # should effectively be the same
+        res = world.get_neighbors(cell_idxs=[idx], nghbr_idxs=list(range(len(nghbrs))))
+        assert len(res) == len(exp), idx
+        assert set(res) == exp, idx
+
+    res = world.get_neighbors(cell_idxs=[0, 1, 2])
+    exp = nghbrs[0] | nghbrs[1] | nghbrs[2]
+    assert len(res) == len(exp)
+    assert set(res) == exp
+
+    res = world.get_neighbors(cell_idxs=[1, 4, 8])
+    exp = nghbrs[1] | nghbrs[4] | nghbrs[8]
+    assert len(res) == len(exp)
+    assert set(res) == exp
+
+    res = world.get_neighbors(cell_idxs=[1, 4, 8])
+    exp = nghbrs[1] | nghbrs[4] | nghbrs[8]
+    assert len(res) == len(exp)
+    assert set(res) == exp
+
+    nghbr_idxs = [2, 3]
+    res = world.get_neighbors(cell_idxs=[0], nghbr_idxs=nghbr_idxs)
+    exp = nghbrs[0]
+    exp = set(d for d in exp if d[0] in nghbr_idxs or d[1] in nghbr_idxs)
+    assert len(res) == len(exp)
+    assert set(res) == exp
+
+    nghbr_idxs = [6, 2]
+    res = world.get_neighbors(cell_idxs=[0, 3], nghbr_idxs=nghbr_idxs)
+    exp = nghbrs[0] | nghbrs[3]
+    exp = set(d for d in exp if d[0] in nghbr_idxs or d[1] in nghbr_idxs)
+    assert len(res) == len(exp)
+    assert set(res) == exp
+
+
+def test_empty_proteome_and_genome_cells():
+    genomes = [ms.random_genome(10), "", ms.random_genome(10)]
+
+    chemistry = ms.Chemistry(molecules=MOLECULES, reactions=[])
+    world = ms.World(chemistry=chemistry, map_size=9)
+
+    world.add_cells(genomes=genomes)
+    assert world.n_cells == 3
+
+    # get cells with empty proteomes
+    assert len(world.get_cell(by_idx=0).proteome) == 0
+    assert len(world.get_cell(by_idx=1).proteome) == 0
+    assert len(world.get_cell(by_idx=2).proteome) == 0
+
+    # load cells with empty fastAs
+    with tempfile.TemporaryDirectory() as tmpdir:
+        statedir = Path(tmpdir)
+        world.save_state(statedir=statedir)
+
+        del world
+        world = ms.World(chemistry=chemistry, map_size=9)
+        world.load_state(statedir=statedir)
+
+    assert world.genomes == genomes
```

