# Comparing `tmp/oganesson-0.1.4.tar.gz` & `tmp/oganesson-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oganesson-0.1.4.tar", last modified: Wed May 17 14:14:02 2023, max compression
+gzip compressed data, was "oganesson-0.1.5.tar", last modified: Thu Jun  8 01:32:58 2023, max compression
```

## Comparing `oganesson-0.1.4.tar` & `oganesson-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.086581 oganesson-0.1.4/
--rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.4/.gitattributes
--rw-rw-rw-   0        0        0     3018 2023-05-17 14:10:37.000000 oganesson-0.1.4/.gitignore
--rw-rw-rw-   0        0        0      471 2023-05-17 14:13:40.000000 oganesson-0.1.4/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.4/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3314 2023-05-17 14:14:02.085579 oganesson-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2930 2023-05-17 14:10:37.000000 oganesson-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.056537 oganesson-0.1.4/assets/
--rw-rw-rw-   0        0        0     2080 2023-05-16 02:19:45.000000 oganesson-0.1.4/assets/logo.svg
-drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.062079 oganesson-0.1.4/oganesson/
--rw-rw-rw-   0        0        0        5 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/VERSION
--rw-rw-rw-   0        0        0      901 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.4/oganesson/__main__.py
--rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.4/oganesson/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.074069 oganesson-0.1.4/oganesson/dataset/
--rw-rw-rw-   0        0        0     2315 2023-05-14 23:40:10.000000 oganesson-0.1.4/oganesson/dataset/vasp.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.079594 oganesson-0.1.4/oganesson/descriptors/
--rw-rw-rw-   0        0        0     1454 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/__init__.py
--rw-rw-rw-   0        0        0     7939 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/bacd.py
--rw-rw-rw-   0        0        0      901 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/descriptors.py
--rw-rw-rw-   0        0        0     5267 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/dscribe.py
--rw-rw-rw-   0        0        0     3606 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/rosa.py
--rw-rw-rw-   0        0        0     2805 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/descriptors/symmetry_functions.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.080593 oganesson-0.1.4/oganesson/genetic_algorithms/
--rw-rw-rw-   0        0        0     7853 2023-05-17 13:42:10.000000 oganesson-0.1.4/oganesson/genetic_algorithms/__init__.py
--rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.4/oganesson/ogai.py
--rw-rw-rw-   0        0        0    10992 2023-05-17 14:10:37.000000 oganesson-0.1.4/oganesson/ogstructure.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.081593 oganesson-0.1.4/oganesson/reinforcement_learning/
--rw-rw-rw-   0        0        0        0 2023-05-16 14:41:36.000000 oganesson-0.1.4/oganesson/reinforcement_learning/m3gnet.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.084580 oganesson-0.1.4/oganesson/utilities/
--rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.4/oganesson/utilities/__init__.py
--rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.4/oganesson/utilities/atomic_data.py
--rw-rw-rw-   0        0        0   405452 2023-05-17 13:20:45.000000 oganesson-0.1.4/oganesson/utilities/bonds_dictionary.py
--rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.4/oganesson/version.py
-drwxrwxrwx   0        0        0        0 2023-05-17 14:14:02.074069 oganesson-0.1.4/oganesson.egg-info/
--rw-rw-rw-   0        0        0     3314 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      878 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       45 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-17 14:14:02.000000 oganesson-0.1.4/oganesson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 14:14:02.086581 oganesson-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-05-17 00:46:24.000000 oganesson-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 01:32:58.064804 oganesson-0.1.5/
+-rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.5/.gitattributes
+-rw-rw-rw-   0        0        0     3036 2023-06-08 01:29:47.000000 oganesson-0.1.5/.gitignore
+-rw-rw-rw-   0        0        0      549 2023-06-08 01:28:19.000000 oganesson-0.1.5/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.5/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     3314 2023-06-08 01:32:58.063654 oganesson-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2930 2023-05-17 14:10:37.000000 oganesson-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 01:32:57.943189 oganesson-0.1.5/assets/
+-rw-rw-rw-   0        0        0     2080 2023-05-16 02:19:45.000000 oganesson-0.1.5/assets/logo.svg
+drwxrwxrwx   0        0        0        0 2023-06-08 01:32:57.979236 oganesson-0.1.5/oganesson/
+-rw-rw-rw-   0        0        0        5 2023-06-08 01:28:19.000000 oganesson-0.1.5/oganesson/VERSION
+-rw-rw-rw-   0        0        0      901 2023-05-17 14:10:37.000000 oganesson-0.1.5/oganesson/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.5/oganesson/__main__.py
+-rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.5/oganesson/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-08 01:32:58.032377 oganesson-0.1.5/oganesson/descriptors/
+-rw-rw-rw-   0        0        0     1679 2023-06-08 01:28:19.000000 oganesson-0.1.5/oganesson/descriptors/__init__.py
+-rw-rw-rw-   0        0        0     7939 2023-05-17 14:10:37.000000 oganesson-0.1.5/oganesson/descriptors/bacd.py
+-rw-rw-rw-   0        0        0     1620 2023-06-08 01:28:19.000000 oganesson-0.1.5/oganesson/descriptors/descriptors.py
+-rw-rw-rw-   0        0        0     5267 2023-05-18 08:13:51.000000 oganesson-0.1.5/oganesson/descriptors/dscribe.py
+-rw-rw-rw-   0        0        0     3606 2023-05-17 14:10:37.000000 oganesson-0.1.5/oganesson/descriptors/rosa.py
+-rw-rw-rw-   0        0        0     2805 2023-05-24 03:23:47.000000 oganesson-0.1.5/oganesson/descriptors/symmetry_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-08 01:32:58.040380 oganesson-0.1.5/oganesson/genetic_algorithms/
+-rw-rw-rw-   0        0        0     7853 2023-05-24 03:21:28.000000 oganesson-0.1.5/oganesson/genetic_algorithms/__init__.py
+-rw-rw-rw-   0        0        0     6399 2023-06-08 01:28:19.000000 oganesson-0.1.5/oganesson/molecular_dynamics.py
+-rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.5/oganesson/ogai.py
+-rw-rw-rw-   0        0        0    14851 2023-06-08 01:28:19.000000 oganesson-0.1.5/oganesson/ogstructure.py
+drwxrwxrwx   0        0        0        0 2023-06-08 01:32:58.042372 oganesson-0.1.5/oganesson/reinforcement_learning/
+-rw-rw-rw-   0        0        0        0 2023-05-16 14:41:36.000000 oganesson-0.1.5/oganesson/reinforcement_learning/m3gnet.py
+drwxrwxrwx   0        0        0        0 2023-06-08 01:32:58.062371 oganesson-0.1.5/oganesson/utilities/
+-rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.5/oganesson/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.5/oganesson/utilities/atomic_data.py
+-rw-rw-rw-   0        0        0   405452 2023-05-17 13:20:45.000000 oganesson-0.1.5/oganesson/utilities/bonds_dictionary.py
+-rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.5/oganesson/version.py
+drwxrwxrwx   0        0        0        0 2023-06-08 01:32:57.998384 oganesson-0.1.5/oganesson.egg-info/
+-rw-rw-rw-   0        0        0     3314 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      884 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       52 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-08 01:32:57.000000 oganesson-0.1.5/oganesson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 01:32:58.064804 oganesson-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1182 2023-06-08 01:28:19.000000 oganesson-0.1.5/setup.py
```

### Comparing `oganesson-0.1.4/.gitignore` & `oganesson-0.1.5/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -157,8 +157,10 @@
 neb_path_*/
 ./*.traj
 ./*.json
 ./*.vasp
 ./*.txt
 
 ./*.db
-./run_*/
+./run_*/
+jolt_lab
+og_lab
```

### Comparing `oganesson-0.1.4/CONTRIBUTING.rst` & `oganesson-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/LICENSE` & `oganesson-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/PKG-INFO` & `oganesson-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.4
+Version: 0.1.5
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
 Keywords: ai,machine learning
 Description-Content-Type: text/markdown
```

### Comparing `oganesson-0.1.4/README.md` & `oganesson-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/assets/logo.svg` & `oganesson-0.1.5/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson/__init__.py` & `oganesson-0.1.5/oganesson/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson/cli.py` & `oganesson-0.1.5/oganesson/cli.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson/descriptors/__init__.py` & `oganesson-0.1.5/oganesson/descriptors/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,29 +16,33 @@
     from oganesson.descriptors.rosa import _ROSA
     ROSA = _ROSA
 except ImportError:
     print('GPAW is not installed, and therefore you cannot use the ROSA descriptors.')
 
 try:
     imp.find_module('dscribe')
-    from oganesson.descriptors.dscribe import _DScribeACSF, _DScribeSOAP,_DScribeCoulombMatrix,_DScribeEwaldSumMatrix,_DScribeSineMatrix
+    from oganesson.descriptors.dscribe import _DScribeACSF, _DScribeSOAP, _DScribeCoulombMatrix, _DScribeEwaldSumMatrix, _DScribeSineMatrix
     DscribeACSF = _DScribeACSF
     DScribeSOAP = _DScribeSOAP
-    DScribeCoulombMatrix=_DScribeCoulombMatrix
-    DScribeEwaldSumMatrix=_DScribeEwaldSumMatrix
-    DScribeSineMatrix=_DScribeSineMatrix
+    DScribeCoulombMatrix = _DScribeCoulombMatrix
+    DScribeEwaldSumMatrix = _DScribeEwaldSumMatrix
+    DScribeSineMatrix = _DScribeSineMatrix
 except ImportError:
     print('DScribe is not installed, and therefore you cannot use the DScribe descriptors.')
 
 
 class DescriptorsName(Enum):
     BACD = 0
     ROSA = 1
     SymmetryFunctions = 2
+    DscribeACSF = 3
 
 
 class Describe:
-    def __init__(self,
-                 structure: Union[Atoms, Structure, str, OgStructure],
-                 descriptor: Union[DescriptorsName, Descriptors],
+    @staticmethod
+    def describe(structure: Union[Atoms, Structure, str, OgStructure],
+                 descriptor: Descriptors,
                  string_format: str = None) -> None:
-        pass
+        # if not isinstance(descriptor, Descriptors):
+        #     raise Exception('The descriptor argument must be of type Descriptors.')
+        descriptor_object = descriptor(structure)
+        return descriptor_object.describe()
```

### Comparing `oganesson-0.1.4/oganesson/descriptors/bacd.py` & `oganesson-0.1.5/oganesson/descriptors/bacd.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson/descriptors/dscribe.py` & `oganesson-0.1.5/oganesson/descriptors/dscribe.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson/descriptors/rosa.py` & `oganesson-0.1.5/oganesson/descriptors/rosa.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson/descriptors/symmetry_functions.py` & `oganesson-0.1.5/oganesson/descriptors/symmetry_functions.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson/genetic_algorithms/__init__.py` & `oganesson-0.1.5/oganesson/genetic_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson/ogstructure.py` & `oganesson-0.1.5/oganesson/ogstructure.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,23 +7,24 @@
 from ase.neb import NEB
 import os
 from ase.io import read
 from typing import Union
 from oganesson.utilities.bonds_dictionary import bonds_dictionary
 from m3gnet.models import Relaxer
 
-
 class OgStructure:
     '''
     The generic structure object in og.
     Unifies the type of the structure to be that of pymatgen.
     '''
 
     def __init__(self, structure: Union[Atoms, Structure, str] = None, file_name: str = None) -> None:
         if structure is not None:
+            if isinstance(structure, OgStructure):
+                self = structure
             if isinstance(structure, str):
                 parser = CifParser.from_string(structure)
                 structure = parser.get_structures()
                 self.structure = structure[0]
             elif isinstance(structure, Atoms):
                 self.structure = self.ase_to_pymatgen(structure)
             elif isinstance(structure, Structure):
@@ -185,14 +186,15 @@
             ii += 1
         return False
 
     def relax(self, relaxation_method='m3gnet', cellbounds=None):
         relaxer = Relaxer()
         relax_results = relaxer.relax(self.structure, verbose=True)
         self.structure = relax_results['final_structure']
+        self.total_energy = relax_results['trajectory'].energies[-1]
 
     def generate_neb(self, moving_atom_species, num_images=5, r=3, relaxation_method=None) -> None:
         structure = self.structure
         self.neb_paths = []
         for i_site in range(len(structure)):
             if structure[i_site].specie.symbol == moving_atom_species:
                 all_neighbors = structure.get_neighbors(
@@ -246,7 +248,83 @@
                             if relaxation_method == 'm3gnet':
                                 self.images[i] = self.images[i].relax()
                             image_str = self.images[i].structure.to(
                                 fmt='poscar')
                             f = open(neb_folder+'/'+str(i).zfill(2), 'w')
                             f.write(image_str)
                             f.close()
+
+    def substitutions(self, atom_X, atom_X_substitution, atol=0.001):
+        from bsym.interface.pymatgen import unique_structure_substitutions
+        new_structures = unique_structure_substitutions(
+            self.structure, atom_X, atom_X_substitution, atol=atol)
+        if 'X' not in atom_X_substitution.keys():
+            return new_structures
+        else:
+            updated_structures = []
+            for s in new_structures:
+                s.remove_species(['X'])
+                updated_structures += [s]
+            return updated_structures
+
+    def simulate(self, thermostat='anderson', steps=10000, temperature=300, ensemble='nvt', timestep=1, loginterval=1000, folder_tag=None):
+        from oganesson.molecular_dynamics import MolecularDynamics
+        import uuid
+        self.dt = timestep
+        if not os.path.isdir('og_lab'):
+            os.mkdir('og_lab')
+        if folder_tag is None:
+            self.folder_tag = str(uuid.uuid4())
+
+        self.folder_tag = 'simulation_' + self.folder_tag
+        os.mkdir('og_lab/'+self.folder_tag)
+
+        self.trajectory_file = 'og_lab/' + \
+            self.folder_tag+'/'+str(temperature)+".traj"
+        self.log_file = 'og_lab/'+self.folder_tag+'/'+str(temperature)+".log"
+        md = MolecularDynamics(atoms=self.to_ase(),
+                               thermostat=thermostat,
+                               temperature=temperature,
+                               timestep=timestep,
+                               ensemble=ensemble,
+                               trajectory=self.trajectory_file,
+                               logfile=self.log_file,
+                               loginterval=loginterval)
+        md.run(steps=steps)
+
+    def calculate_diffusivity(self, calculation_type='tracer', axis='all', ignore_n_images=0):
+        if self.trajectory_file:
+            from diffusivity.diffusion_coefficients import DiffusionCoefficient
+            from ase.md.md import Trajectory
+            diffusion_coefficients = DiffusionCoefficient(
+                Trajectory(self.trajectory_file), self.dt*1e-15, calculation_type=calculation_type, axis=axis)
+            diffusion_coefficients.calculate(ignore_n_images=ignore_n_images)
+            self.diffusion_coefficients = diffusion_coefficients.get_diffusion_coefficients()
+
+            # Plotting the MSD curve for each species in the structure
+            import matplotlib.pyplot as plt
+            plt.figure(figsize=(15, 10))
+            MSDs = []
+            plots = []
+            n = len(diffusion_coefficients.timesteps)
+            print('Plotting MSD using', n, 'images')
+
+            for sym_index in range(diffusion_coefficients.no_of_types_of_atoms):
+                MSD = np.zeros(len(diffusion_coefficients.timesteps[1:]))
+                for xyz in range(3):
+                    MSD += diffusion_coefficients.xyz_segment_ensemble_average[0][sym_index][xyz]
+                MSD /= 3
+                MSDs += [MSD]
+                label = diffusion_coefficients.types_of_atoms[sym_index]
+                # Add scatter graph  for the mean square displacement data in this segment
+                l, = plt.plot(diffusion_coefficients.timesteps[1:], MSD,
+                              label=label, linewidth=1)
+                plots += [l]
+            plt.legend(handles=plots)
+            plt.ylabel('MSD')
+            plt.savefig('og_lab/' +
+                        self.folder_tag+'/MSD_'+calculation_type+'_'+axis, bbox_inches='tight')
+            plt.clf()
+
+            return self.diffusion_coefficients
+        else:
+            print('You have to run a simulation first!')
```

### Comparing `oganesson-0.1.4/oganesson/utilities/__init__.py` & `oganesson-0.1.5/oganesson/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson/utilities/atomic_data.py` & `oganesson-0.1.5/oganesson/utilities/atomic_data.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson/utilities/bonds_dictionary.py` & `oganesson-0.1.5/oganesson/utilities/bonds_dictionary.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.4/oganesson.egg-info/PKG-INFO` & `oganesson-0.1.5/oganesson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oganesson
-Version: 0.1.4
+Version: 0.1.5
 Summary: oganesson enables rapid AI workflows for material science and chemistry
 Home-page: https://github.com/oganesson-ai/oganesson
 Author: Sherif Abdulkader Tawfik Abbas
 Author-email: sherif.tawfic@gmail.com
 License: mit
 Keywords: ai,machine learning
 Description-Content-Type: text/markdown
```

### Comparing `oganesson-0.1.4/oganesson.egg-info/SOURCES.txt` & `oganesson-0.1.5/oganesson.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 README.md
 setup.py
 assets/logo.svg
 oganesson/VERSION
 oganesson/__init__.py
 oganesson/__main__.py
 oganesson/cli.py
+oganesson/molecular_dynamics.py
 oganesson/ogai.py
 oganesson/ogstructure.py
 oganesson/version.py
 oganesson.egg-info/PKG-INFO
 oganesson.egg-info/SOURCES.txt
 oganesson.egg-info/dependency_links.txt
 oganesson.egg-info/entry_points.txt
 oganesson.egg-info/requires.txt
 oganesson.egg-info/top_level.txt
-oganesson/dataset/vasp.py
 oganesson/descriptors/__init__.py
 oganesson/descriptors/bacd.py
 oganesson/descriptors/descriptors.py
 oganesson/descriptors/dscribe.py
 oganesson/descriptors/rosa.py
 oganesson/descriptors/symmetry_functions.py
 oganesson/genetic_algorithms/__init__.py
```

### Comparing `oganesson-0.1.4/setup.py` & `oganesson-0.1.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,10 +24,11 @@
     keywords=['ai', 'machine learning'],
     install_requires=['ase',
                       'pandas',
                       'numpy',
                       'm3gnet',
                       'pymatgen',
                       'm3gnet',
-                      'gpaw'],
+                    #   'gpaw',
+                      'diffusivity'],
 
 )
```

