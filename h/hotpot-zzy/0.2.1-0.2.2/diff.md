# Comparing `tmp/hotpot-zzy-0.2.1.tar.gz` & `tmp/hotpot-zzy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-i134ha33/hotpot-zzy-0.2.1.tar", last modified: Tue Jun  6 07:46:36 2023, max compression
+gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-53s7j1d6/hotpot-zzy-0.2.2.tar", last modified: Thu Jun  8 01:49:14 2023, max compression
```

## Comparing `hotpot-zzy-0.2.1.tar` & `hotpot-zzy-0.2.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       17 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/MANIFEST.in
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/PKG-INFO
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      398 2023-05-19 15:58:44.000000 hotpot-zzy-0.2.1/hotpot/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    39992 2023-05-20 11:35:21.000000 hotpot-zzy-0.2.1/hotpot/_io.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    14731 2023-06-06 07:26:56.000000 hotpot-zzy-0.2.1/hotpot/bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    83164 2023-06-06 07:13:56.000000 hotpot-zzy-0.2.1/hotpot/cheminfo.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/data/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/data/force_field/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/data/force_field/UFF/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     4710 2023-05-04 02:36:48.000000 hotpot-zzy-0.2.1/hotpot/data/force_field/UFF/LJ.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/data/force_field/aMaterials/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1742 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/data/force_field/aMaterials/SiC.tersoff
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       88 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/data/force_field/contents.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-06-06 06:50:07.000000 hotpot-zzy-0.2.1/hotpot/data/periodic_table.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      195 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/data/units.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/tanks/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      217 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/tanks/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      365 2023-06-05 01:59:39.000000 hotpot-zzy-0.2.1/hotpot/tanks/cc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      161 2023-03-23 08:00:45.000000 hotpot-zzy-0.2.1/hotpot/tanks/features.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/tanks/lmp/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      284 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/tanks/lmp/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8118 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/hotpot/tanks/lmp/base.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8704 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/hotpot/tanks/lmp/gcmc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     9577 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/hotpot/tanks/lmp/materials.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     7857 2023-03-30 08:04:59.000000 hotpot-zzy-0.2.1/hotpot/tanks/quantum.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2949 2023-05-13 03:01:23.000000 hotpot-zzy-0.2.1/hotpot/tmo.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2882 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/tools.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot/utils/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      134 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/utils/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      669 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.1/hotpot/utils/units_convert.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-06 07:46:36.000000 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/PKG-INFO
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      813 2023-06-06 07:46:36.000000 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/SOURCES.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-06-06 07:46:36.000000 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/dependency_links.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       26 2023-06-06 07:46:36.000000 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/requires.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-06-06 07:46:36.000000 hotpot-zzy-0.2.1/hotpot_zzy.egg-info/top_level.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      263 2023-06-06 07:33:50.000000 hotpot-zzy-0.2.1/pyproject.toml
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/setup.cfg
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-06 07:46:36.324825 hotpot-zzy-0.2.1/test/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      550 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/test/test_amorphous_maker.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1162 2023-05-20 11:40:18.000000 hotpot-zzy-0.2.1/test/test_bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1932 2023-06-06 07:26:56.000000 hotpot-zzy-0.2.1/test/test_chemif.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     7081 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.1/test/test_lmp.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       17 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/MANIFEST.in
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/PKG-INFO
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      398 2023-05-19 15:58:44.000000 hotpot-zzy-0.2.2/hotpot/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    39992 2023-05-20 11:35:21.000000 hotpot-zzy-0.2.2/hotpot/_io.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    14652 2023-06-06 11:58:39.000000 hotpot-zzy-0.2.2/hotpot/bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)    88345 2023-06-08 01:37:04.000000 hotpot-zzy-0.2.2/hotpot/cheminfo.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/data/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/data/force_field/
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/data/force_field/UFF/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     4710 2023-05-04 02:36:48.000000 hotpot-zzy-0.2.2/hotpot/data/force_field/UFF/LJ.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/data/force_field/aMaterials/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1742 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       88 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/data/force_field/contents.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-06-06 06:50:07.000000 hotpot-zzy-0.2.2/hotpot/data/periodic_table.json
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      195 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/data/units.json
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/tanks/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      217 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/tanks/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      365 2023-06-05 01:59:39.000000 hotpot-zzy-0.2.2/hotpot/tanks/cc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      161 2023-03-23 08:00:45.000000 hotpot-zzy-0.2.2/hotpot/tanks/features.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/tanks/lmp/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      284 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/tanks/lmp/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8118 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/hotpot/tanks/lmp/base.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     8704 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/hotpot/tanks/lmp/gcmc.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     9577 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/hotpot/tanks/lmp/materials.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     7857 2023-03-30 08:04:59.000000 hotpot-zzy-0.2.2/hotpot/tanks/quantum.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2949 2023-05-13 03:01:23.000000 hotpot-zzy-0.2.2/hotpot/tmo.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     2882 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/tools.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot/utils/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      134 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/utils/__init__.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      669 2023-04-27 07:38:36.000000 hotpot-zzy-0.2.2/hotpot/utils/units_convert.py
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       54 2023-06-08 01:49:14.000000 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/PKG-INFO
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      813 2023-06-08 01:49:14.000000 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/SOURCES.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-06-08 01:49:14.000000 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/dependency_links.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       26 2023-06-08 01:49:14.000000 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/requires.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-06-08 01:49:14.000000 hotpot-zzy-0.2.2/hotpot_zzy.egg-info/top_level.txt
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      263 2023-06-08 01:48:17.000000 hotpot-zzy-0.2.2/pyproject.toml
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/setup.cfg
+drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-06-08 01:49:14.123445 hotpot-zzy-0.2.2/test/
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)      550 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/test/test_amorphous_maker.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1162 2023-05-20 11:40:18.000000 hotpot-zzy-0.2.2/test/test_bundle.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     1891 2023-06-08 01:38:26.000000 hotpot-zzy-0.2.2/test/test_chemif.py
+-rw-rw-r--   0 zz1       (1005) zz1       (1008)     7081 2023-05-20 00:06:32.000000 hotpot-zzy-0.2.2/test/test_lmp.py
```

### Comparing `hotpot-zzy-0.2.1/hotpot/_io.py` & `hotpot-zzy-0.2.2/hotpot/_io.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot/bundle.py` & `hotpot-zzy-0.2.2/hotpot/bundle.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,22 +200,18 @@
         generator = mol_mp_generator() if num_proc else mol_generator()
 
         if generate:
             return cls(generator)
         else:
             return cls([m for m in tqdm(generator, 'reading molecules')])
 
-    def graph_represent(self, *feature_type):
-        """ Transform molecules to the molecule to graph representation """
-        feature_matrices = []
+    def graph_representation(self, *feature_names) -> Generator[Union[str, np.ndarray, np.ndarray], None, None]:
+        """ Transform molecules to their graph representation """
         for mol in self.mols:
-            feature_matrix = mol.feature_matrix(feature_names=feature_type)
-            feature_matrices.append(feature_matrix)
-
-        return feature_matrices
+            yield mol.graph_representation(*feature_names)
 
     def gaussian(
             self, g16root: Union[str, PathLike], dir_out: Union[str, PathLike],
             link0: Union[str, List[str]], route: Union[str, List[str]],
             dir_err: Optional[Union[str, PathLike]] = None,
             dir_chk: Optional[Union[str, PathLike]] = None,
             clean_configure: bool = True,
```

### Comparing `hotpot-zzy-0.2.1/hotpot/cheminfo.py` & `hotpot-zzy-0.2.2/hotpot/cheminfo.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,23 @@
 import numpy as np
 from openbabel import openbabel as ob, pybel as pb
 
 from hotpot import data_root
 from hotpot.tanks import lmp
 from hotpot.tanks.quantum import Gaussian
 
+# Define Exceptions
+class OperateOBMolFail(BaseException):
+    """ Raise for any fail that trys to operate the OBMol """
+class AddAtomFail(OperateOBMolFail):
+    """ Raise when add an atom into Molecule fail """
+
+class AddBondFail(OperateOBMolFail):
+    """ Raise when add a bond into Molecule fail """
+
 periodic_table = json.load(open(ptj(data_root, 'periodic_table.json'), encoding='utf-8'))
 # periodic_table = {d['symbol']: d for d in periodic_table}
 _symbols = ['unknown'] + list(periodic_table.keys())
 _max_valences = {n: v['max_valence'] for n, v in periodic_table.items()}
 _max_total_bond_order = {n: v['max_total_bond_order'] for n, v in periodic_table.items()}
 
 _bond_type = {
@@ -542,29 +551,39 @@
     def _set_spin_multiplicity(self, spin):
         self.ob_mol.SetTotalSpinMultiplicity(spin)
 
     @property
     def acentric_factor(self):
         return self._get_critical_params('acentric_factor')
 
-    def add_atom(self, atom: Union["Atom", str, int]):
+    def add_atom(self, atom: Union["Atom", str, int], **atom_kwargs):
         """
         Add a new atom out of the molecule into the molecule.
         Args:
             atom(Atom|str|int):
 
-        Returns:
+        atom_kwargs(kwargs for this added atom):
+            atomic_number(int): set atomic number
+            symbol(str): set atomic symbol
+            coordinates(Sequence, numpy.ndarray): coordinates of the atom
+            partial_charge:
+            label:
+            spin_density:
 
+        Returns:
+            the copy of atom in the molecule
         """
         if isinstance(atom, str):
-            atom = Atom(symbol=atom)
+            atom = Atom(symbol=atom, **atom_kwargs)
         elif isinstance(atom, int):
-            atom = Atom(atomic_number=atom)
+            atom = Atom(atomic_number=atom, **atom_kwargs)
+        elif isinstance(atom, Atom):
+            atom.set(**atom_kwargs)
 
-        # Avoid add a existed atom into the molecule
+        # Avoid add an existed atom into the molecule
         if atom.molecule and (atom.molecule is self or atom.molecule.ob_mol is self.ob_mol):
             raise AttributeError("This atom have exist in the molecule")
 
         success = self.ob_mol.AddAtom(atom.ob_atom)
         if success:
 
             # Get the last OBAtom
@@ -583,31 +602,31 @@
 
             # add the new atom into atoms list directly
             atoms = self._data.setdefault('atoms', {})
             if atom.ob_id not in atoms:
                 atoms.update({atom.ob_id: atom})
                 return atom
             else:
-                print(RuntimeWarning(f'the atom with ob_id {atom.ob_id} have exist in the Molecule'))
+                raise ValueError(f'the atom with ob_id {atom.ob_id} have exist in the Molecule')
 
         else:
-            print(RuntimeWarning("Fail to add atom"))
+            raise AddAtomFail(f'Add the atom {atom} into Molecule fail')
 
     def add_bond(
             self,
             atom1: Union[str, int, 'Atom'],
             atom2: Union[str, int, 'Atom'],
             bond_type: Union[str, int],
     ):
         """ Add a new bond into the molecule """
         inputs = (atom1, atom2)
         atoms: List[Atom] = []
         for a in inputs:
             if isinstance(a, int):
-                atoms.append(self.atoms[a])
+                atoms.append(self.atoms_dict[a])
             if isinstance(a, Atom):
                 atoms.append(a)
             if isinstance(a, str):
                 atoms.append(self.atom(a))
 
         # Represent the bond type by int, refer to _bond_type dict
         bond_type = bond_type if isinstance(bond_type, int) else _bond_type[bond_type]
@@ -671,26 +690,80 @@
     def all_energy(self):
         return self._data.get('all_energy')
 
     @property
     def angles(self):
         return [Angle(self, a_idx) for a_idx in ob.OBMolAngleIter(self.ob_mol)]
 
+    def generate_metal_ligand_pair(
+            self, metal_symbol: str, acceptor_atoms: Sequence = ('O',), opti_force_field: str = 'UFF'
+    ) -> Generator['Molecule', None, None]:
+        """
+        This method could work if the molecule is an organic ligand, or raise AttributeError.
+        Generate metal-ligand pair by link metal with acceptor atoms in the organic ligand.
+
+        Args:
+            metal_symbol: which metal element link to the ligand
+            acceptor_atoms: which elements to be acceptor atom to link to metal
+            opti_force_field: which force field could be used to optimize the configuration of ligand and M-L pair.
+
+        Return:
+            A generator for M-L pair
+
+        Raise:
+            AttributeError: if the molecule is not an organic ligand
+        """
+        if not self.is_organic:
+            raise AttributeError('the accepting molecule should be organic compound')
+
+        ligand = self.copy()
+        ligand.localed_optimize(opti_force_field)  # locally optimize the ligand
+        ligand.normalize_labels()
+
+        for atom in ligand.atoms:
+            if atom.symbol in acceptor_atoms:
+                acceptor_ligand = ligand.copy()
+
+                # assign the initial coordinates
+                # the sum of vector of relative position relate to the accepting atom
+                sum_relative_coordinates = sum([c for _, c in atom.neighbours_position])
+                metal_init_coordinates = atom.coordinates - sum_relative_coordinates
+
+                # add metal atom into the acceptor_ligand
+                added_metal = acceptor_ligand.add_atom(metal_symbol, coordinates=metal_init_coordinates)
+
+                # add the coordinating bond between metal atom and acceptor atoms
+                acceptor_ligand.add_bond(added_metal, atom.label, 1)
+
+                # remove redundant hydrogen
+                accepting_atom = acceptor_ligand.atom(atom.label)
+                while accepting_atom.valence > accepting_atom.valence_max and accepting_atom.neigh_hydrogens:
+                    acceptor_ligand.remove_atoms(accepting_atom.neigh_hydrogens[0])
+
+                # localize optimization of M-L pair by classical force field
+                acceptor_ligand.localed_optimize(opti_force_field)
+
+                yield acceptor_ligand
+
     def assign_bond_types(self):
         self.ob_mol.PerceiveBondOrders()
 
     def atom(self, id_label: Union[int, str]) -> 'Atom':
         """ get atom by label or idx """
         if not self.is_labels_unique:
             print(AttributeError('the molecule atoms labels are not unique!'))
 
         if isinstance(id_label, str):
-            return self.atoms[self.labels.index(id_label)]
+            for atom in self.atoms:
+                if atom.label == id_label:
+                    return atom
+            raise KeyError(f'No atom with label {id_label}')
+
         elif isinstance(id_label, int):
-            return self.atoms[id_label]
+            return self.atoms_dict[id_label]
         else:
             raise TypeError(f'the given idx_label is expected to be int or string, but given {type(id_label)}')
         
     @property
     def atom_num(self):
         return self.ob_mol.NumAtoms()
 
@@ -701,15 +774,15 @@
         Return list of Atom objects with the order their index.
         """
         atoms = self._load_atoms()
         return list(atoms.values())
 
     @property
     def atoms_dict(self) -> Dict[int, 'Atom']:
-        return copy.copy(self._data.get('atoms', {}))
+        return self._load_atoms()
 
     @property
     def all_atoms(self):
         return self.atoms + self.pseudo_atoms
 
     @property
     def atom_charges(self) -> np.ndarray:
@@ -901,15 +974,14 @@
         # Clone the old UnitCell data into new
         cell_data = self.ob_mol.GetData(12)  # the UnitCell of OBmol save with idx 12
         if cell_data:
             clone_mol.ob_mol.CloneData(cell_data)
 
         # copy, in turn, each Atom in this molecule and add them into new Molecule
         for atom in self.atoms:
-            # clone_atom = atom.copy()
             clone_mol.add_atom(atom)
 
         # generate Bonds in new Molecule with same graph pattern in this Molecule
         for bond in self.bonds:
             clone_mol.add_bond(*bond.atoms, bond_type=bond.type)
 
         return clone_mol
@@ -1036,33 +1108,26 @@
         return re.findall(r'[A-Z][a-z]*', self.formula)
 
     @property
     def energy(self):
         """ Return energy with kcal/mol as default """
         return self.ob_mol.GetEnergy()
 
-    def feature_matrix(self, feature_names):
-        n = self.atom_num
-        m = len(feature_names)
-        np.set_printoptions(suppress=True, precision=6)
-        feature_matrix = np.zeros((n, m+3))
-
-        for i, atom in enumerate(self.atoms):
-            atom_features = atom.element_features(output_type='dict', *feature_names)
-            for j, feature_name in enumerate(feature_names):
-                if feature_name == 'atom_orbital_feature':
-                    ao_features = atom_features[feature_name]
-                    feature_matrix[i, j] = ao_features['s']
-                    feature_matrix[i, j + 1] = ao_features['p']
-                    feature_matrix[i, j + 2] = ao_features['d']
-                    feature_matrix[i, j + 3] = ao_features['f']
-                    j += 3
-                else:
-                    feature_matrix[i, j] = atom_features[feature_name]
-        return feature_matrix
+    def feature_matrix(self, *feature_names: Sequence) -> np.ndarray:
+        """ Retrieve the feature matrix (collections of feature vector for every atoms),
+         The default feature is `atomic_orbital`, if the feature names not be specified, the `atomic_orbital` will be
+         retrieved.
+         Args:
+             feature_names: the feature names are offered in hotpot/data/periodic_table.json
+         """
+        if not feature_names:
+            feature_names = ('atomic_orbital',)
+
+        # Matrix with shape (atom_numbers, feature_length)
+        return np.stack([atom.element_features(*feature_names) for atom in self.atoms])
 
     @property
     def forces(self):
         """ return the all force vectors for all atoms in the molecule """
         return np.vstack((atom.force_vector for atom in self.atoms))
 
     @property
@@ -1128,14 +1193,17 @@
         if path_err_file:
             with open(path_err_file, 'w') as writer:
                 writer.write(stderr)
 
         # return results and error info
         return stdout, stderr
 
+    def graph_representation(self, *feature_names):
+        return self.identifier, self.feature_matrix(*feature_names), self.link_matrix
+
     @property
     def has_3d(self):
         """ Whether atoms in the molecule have 3d coordinates """
         return self.ob_mol.Has3D()
 
     @property
     def identifier(self):
@@ -1422,67 +1490,81 @@
                 source = Path(source)
 
             if isinstance(source, Path):
                 fmt = source.suffix.strip('.')
             else:
                 raise ValueError(f'the arguments should be specified for {type(source)} source')
 
-        parser = Parser(fmt, source, *args, **kwargs)
-        return parser()
+        mol = Parser(fmt, source, *args, **kwargs)()  # initialize parser object and call self
+
+        # Specify the mol identifier if it's None
+        if not mol.identifier:
+            mol.identifier = source
+
+        return mol
 
     def register_critical_params(self, name: str, temperature: float, pressure: float, acentric: float):
         """ Register new critical parameters into the critical parameters sheet """
         data = json.load(open(ptj(data_root, 'thermo', 'critical.json')))
         data[self.smiles] = {'name': name, 'temperature': temperature, 'pressure': pressure, 'acentric': acentric}
         with open(ptj(data_root, 'thermo', 'critical.json'), 'w') as writer:
             json.dump(data, writer, indent=True)
 
-    def remove_atoms(self, *atoms: Union[int, str, 'Atom']) -> None:
+    def remove_atoms(self, *atoms: Union[int, str, 'Atom'], remove_hydrogens: bool = True) -> None:
         """
         Remove atom according to given atom index, label or the atoms self.
         Args:
             atoms(int|str|Atom): the index, label or self of Removed atom
+            remove_hydrogens(bool): remove the hydrogens connecting in the atoms synchronously.
 
         Returns:
             None
         """
         for atom in atoms:
 
             # Check and locate the atom
             if isinstance(atom, int):
-                atom = self.atoms[atom]
+                atom = self.atoms_dict[atom]
             elif isinstance(atom, str):
-                atom = self.atoms[self.atom_labels.index(atom)]
+                atom = self.atom(atom)
             elif isinstance(atom, Atom):
                 if not (atom.molecule is self):
                     raise AttributeError('the given atom not in the molecule')
             else:
                 raise TypeError('the given atom should be int, str or Atom')
 
-            # Removing atom
+            # remove connecting hydrogens
+            if remove_hydrogens:
+                for nh in atom.neigh_hydrogens:
+                    self.ob_mol.DeleteAtom(nh.ob_atom)
+
+            # Removing the atom
             self.ob_mol.DeleteAtom(atom.ob_atom)
             atom._data['_mol'] = None
 
+            # Reload atoms
+            self._load_atoms()
+
     def remove_hydrogens(self):
         self.ob_mol.DeleteHydrogens()
 
     @property
     def rotatable_bonds_number(self):
         return self.ob_mol.NumRotors()
 
     def set(self, **kwargs):
         """ Set the attributes directly """
         self._set_attrs(**kwargs)
 
-    def set_label(self, idx: int, label: str):
-        self.atoms[idx].label = label
+    def set_label(self, ob_id: int, label: str):
+        self.atoms_dict[ob_id].label = label
 
     @property
     def smiles(self):
-        return self.dump('smi').strip().strip()
+        return self.dump('smi').split()[0]
 
     @property
     def spin(self):
         return self.ob_mol.GetTotalSpinMultiplicity()
 
     @spin.setter
     def spin(self, spin: int):
@@ -1765,16 +1847,16 @@
         return self.ob_atom.GetType()
 
     @property
     def atomic_number(self):
         return self.ob_atom.GetAtomicNum()
 
     @property
-    def coordinates(self):
-        return self.ob_atom.GetX(), self.ob_atom.GetY(), self.ob_atom.GetZ()
+    def coordinates(self) -> np.ndarray:
+        return np.array([self.ob_atom.GetX(), self.ob_atom.GetY(), self.ob_atom.GetZ()])
 
     @coordinates.setter
     def coordinates(self, value):
         self._set_coordinate(value)
 
     def copy(self):
         """ Make a copy of self """
@@ -1798,26 +1880,28 @@
 
         return Atom(**new_attrs)
 
     def copy_data(self):
         """ Make a copy of its data """
         return copy.copy(self._data)
 
-    def element_features(self, *feature_names, output_type='dict'):
+    def element_features(self, *feature_names) -> np.ndarray:
+        """ Retrieve the feature vector """
         atom_feature = periodic_table.get(self.symbol)
-        features = {}
-        for name in feature_names:
-            if name == "atom_orbital_feature":
-                features['atom_orbital_feature'] = self._atomic_orbital_feature()
+
+        features = []
+        for feature_name in feature_names:
+            if feature_name == 'atomic_orbital':
+                features.extend(self._atomic_orbital_feature().values())
+            elif feature_name == 'atomic_number':
+                features.append(self.atomic_number)
             else:
-                features[name] = atom_feature[name]
-        if output_type == 'list':
-            features = [features[name] for name in feature_names]
+                features.append(atom_feature[feature_name])
 
-        return features
+        return np.array(features)
 
     def _atomic_orbital_feature(self, outermost_layer=True, nonexistent_orbit=0):
         """    Calculating the feature about atomic orbital structures    """
         _atomic_orbital_structure_max = {
             "1s": 2,
             "2s": 2, "2p": 6,
             "3s": 2, "3p": 6,
@@ -1871,14 +1955,20 @@
         return self._data.get('force_vector', np.zeros(3, dtype=float))
 
     @force_vector.setter
     def force_vector(self, force_vector: Union[Sequence, np.ndarray]):
         self._set_force_vector(force_vector)
 
     @property
+    def hybridization(self):
+        """ The hybridization of this atom:
+        1 for sp, 2 for sp2, 3 for sp3, 4 for sq. planar, 5 for trig. bipy, 6 for octahedral """
+        return self.ob_atom.GetHyb()
+
+    @property
     def kwargs_attributes(self):
         return tuple(self._attr_setters.keys())
 
     @property
     def ob_id(self):
         return self.ob_atom.GetId()
 
@@ -1891,14 +1981,18 @@
         return self.ob_atom.IsAromatic()
 
     @property
     def is_chiral(self):
         return self.ob_atom.IsChiral()
 
     @property
+    def is_hydrogen(self):
+        return self.ob_atom.GetAtomicNum() == 1
+
+    @property
     def is_polar_hydrogen(self) -> bool:
         """ Is this atom a hydrogen connected to a polar atom """
         return self.ob_atom.IsPolarHydrogen()
 
     @property
     def is_metal(self):
         return self.ob_atom.IsMetal()
@@ -1925,33 +2019,62 @@
         return _max_total_bond_order[self.symbol]
 
     @property
     def molecule(self) -> Molecule:
         return self.mol
 
     @property
-    def neighbours(self):
+    def neigh_hydrogens(self):
+        return [a for a in self.neighbours if a.is_hydrogen]
+
+    @property
+    def neighbours(self) -> List['Atom']:
         """ Get all atoms bond with this atom in same molecule """
         if self.mol:
             _ = self.mol.atoms  # update the atoms dict
             return [self.mol.data.get('atoms')[ob_atom.GetId()] for ob_atom in ob.OBAtomAtomIter(self.ob_atom)]
         else:
             return []
 
     @property
+    def neighbours_position(self) -> Generator[Tuple[Union['Atom', np.ndarray]], None, None]:
+        """ Retrieve the relative position of neigh atoms, assign this atom as the origin """
+        for neigh_atom in self.neighbours:
+            yield neigh_atom, neigh_atom.coordinates - self.coordinates
+
+    @property
     def partial_charge(self):
         return self.ob_atom.GetPartialCharge()
 
     @partial_charge.setter
     def partial_charge(self, value: float):
         # This is necessary to take effect to the assignment.
         # the reason is unknown
         self.ob_atom.GetPartialCharge()
         self._set_partial_charge(value)
 
+    def set(self, **kwargs):
+        """
+        Set atom attributes by kwargs
+        Kwargs:
+            atomic_number(int): set atomic number
+            symbol(str): set atomic symbol
+            coordinates(Sequence, numpy.ndarray): coordinates of the atom
+            partial_charge:
+            label:
+            spin_density:
+        """
+        allow_kwargs = {'atomic_number', 'symbol', 'coordinates', 'partial_charge', 'label', 'spin_density'}
+
+        # check the correctness of given kwargs
+        if any(name not in allow_kwargs for name in kwargs):
+            raise NameError(f'the allow kwargs are just in {allow_kwargs}')
+
+        self._set_attrs(**kwargs)  # set attributes
+
     @property
     def spin_density(self):
         return self._data.get('spin_density', 0.0)
 
     @spin_density.setter
     def spin_density(self, spin_density: float):
         self._set_spin_density(spin_density)
```

### Comparing `hotpot-zzy-0.2.1/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.2.2/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.2.2/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot/data/periodic_table.json` & `hotpot-zzy-0.2.2/hotpot/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.2.2/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.2.2/hotpot/tanks/lmp/gcmc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.2.2/hotpot/tanks/lmp/materials.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot/tanks/quantum.py` & `hotpot-zzy-0.2.2/hotpot/tanks/quantum.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot/tmo.py` & `hotpot-zzy-0.2.2/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot/tools.py` & `hotpot-zzy-0.2.2/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot/utils/units_convert.py` & `hotpot-zzy-0.2.2/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/hotpot_zzy.egg-info/SOURCES.txt` & `hotpot-zzy-0.2.2/hotpot_zzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/test/test_amorphous_maker.py` & `hotpot-zzy-0.2.2/test/test_amorphous_maker.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/test/test_bundle.py` & `hotpot-zzy-0.2.2/test/test_bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.2.1/test/test_chemif.py` & `hotpot-zzy-0.2.2/test/test_chemif.py`

 * *Files 22% similar despite different names*

```diff
@@ -46,24 +46,21 @@
 
     for i, gen_mol in enumerate(gen):
         gen_mol.writefile('cif', f'output/gen_cif/aCarbon_{i}.cif')
 
 
 if __name__ == '__main__':
     from openbabel import openbabel as ob
-    mol = ci.Molecule.read_from('c1ccc(C(=O)O)cc1', 'smi')
-    print(
-        [a.GetAtomicNum() for a in ob.OBMolAtomIter(mol.ob_mol)], '\n',
-        [a.GetId() for a in ob.OBMolAtomIter(mol.ob_mol)], '\n',
-        mol.atoms
-    )
-    mol.build_conformer()
-    print(mol.atoms)
-    mol.remove_hydrogens()
-    sr = mol.add_atom('Sr')
+    mol = ci.Molecule.read_from('c1ccc(C(=O)O)c(O)c1CCCC', 'smi')
+    mol2 = ci.Molecule.read_from('c1ccc(C(=O)O)c(O)c1CCCC', 'smi')
+    mol.build_conformer('UFF')
+    mol2.build_conformer()
     mol.normalize_labels()
-    # mol.add_bond(sr, 'O1', 1)
-    b = mol.add_bond(sr, 'O2', 1)
-    mol.build_conformer()
-    mol.writefile('mol2', '/home/zz1/coor.mol2')
-    print([a.valence for a in mol.atoms])
-    print([a.link_degree for a in mol.atoms])
+    mol2.normalize_labels()
+    g = mol.generate_metal_ligand_pair('Sr')
+
+    # for a1, a2 in zip(mol.atoms, mol2.atoms):
+    #     print(f'{a1.label}: {a1.partial_charge}---{a2.label}: {a2.partial_charge}')
+
+    ps = [p for i, p in enumerate(g)]
+    ps[1].remove_atoms('C1', 'C2')
+    ps[1].writefile('mol2', f'/home/zz1/g01.mol2')
```

### Comparing `hotpot-zzy-0.2.1/test/test_lmp.py` & `hotpot-zzy-0.2.2/test/test_lmp.py`

 * *Files identical despite different names*

