# Comparing `tmp/SBMLDiagrams-1.3.5.tar.gz` & `tmp/SBMLDiagrams-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SBMLDiagrams-1.3.5.tar", last modified: Fri May 19 16:46:38 2023, max compression
+gzip compressed data, was "dist\SBMLDiagrams-1.3.6.tar", last modified: Thu Jun  8 15:53:00 2023, max compression
```

## Comparing `SBMLDiagrams-1.3.5.tar` & `SBMLDiagrams-1.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 16:46:38.352775 SBMLDiagrams-1.3.5/
--rw-rw-rw-   0        0        0     2653 2023-05-19 16:46:38.352775 SBMLDiagrams-1.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     1809 2023-02-23 20:31:51.000000 SBMLDiagrams-1.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 16:46:38.341805 SBMLDiagrams-1.3.5/SBMLDiagrams/
--rw-rw-rw-   0        0        0      784 2022-02-24 16:03:36.000000 SBMLDiagrams-1.3.5/SBMLDiagrams/__init__.py
--rw-rw-rw-   0        0        0       71 2023-05-19 16:40:49.000000 SBMLDiagrams-1.3.5/SBMLDiagrams/_version.py
--rw-rw-rw-   0        0        0   122135 2023-05-16 18:57:09.000000 SBMLDiagrams-1.3.5/SBMLDiagrams/drawNetwork.py
--rw-rw-rw-   0        0        0   123007 2023-05-16 21:57:52.000000 SBMLDiagrams-1.3.5/SBMLDiagrams/editSBML.py
--rw-rw-rw-   0        0        0   104173 2023-05-19 00:45:55.000000 SBMLDiagrams-1.3.5/SBMLDiagrams/exportSBML.py
--rw-rw-rw-   0        0        0     1631 2023-05-16 21:58:12.000000 SBMLDiagrams-1.3.5/SBMLDiagrams/point.py
--rw-rw-rw-   0        0        0   347877 2023-05-19 00:20:33.000000 SBMLDiagrams-1.3.5/SBMLDiagrams/processSBML.py
--rw-rw-rw-   0        0        0    10485 2023-05-16 21:58:22.000000 SBMLDiagrams-1.3.5/SBMLDiagrams/styleSBML.py
--rw-rw-rw-   0        0        0     1194 2023-05-16 21:58:30.000000 SBMLDiagrams-1.3.5/SBMLDiagrams/visualizeInfo.py
--rw-rw-rw-   0        0        0   157788 2023-05-16 18:57:09.000000 SBMLDiagrams-1.3.5/SBMLDiagrams/visualizeSBML.py
-drwxrwxrwx   0        0        0        0 2023-05-19 16:46:38.350781 SBMLDiagrams-1.3.5/SBMLDiagrams.egg-info/
--rw-rw-rw-   0        0        0     2653 2023-05-19 16:46:37.000000 SBMLDiagrams-1.3.5/SBMLDiagrams.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      473 2023-05-19 16:46:38.000000 SBMLDiagrams-1.3.5/SBMLDiagrams.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 16:46:37.000000 SBMLDiagrams-1.3.5/SBMLDiagrams.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2023-05-19 16:46:38.000000 SBMLDiagrams-1.3.5/SBMLDiagrams.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-19 16:46:38.000000 SBMLDiagrams-1.3.5/SBMLDiagrams.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-19 16:46:38.353791 SBMLDiagrams-1.3.5/setup.cfg
--rw-rw-rw-   0        0        0     2034 2022-09-13 05:34:26.000000 SBMLDiagrams-1.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:53:00.563085 SBMLDiagrams-1.3.6/
+-rw-rw-rw-   0        0        0     2653 2023-06-08 15:53:00.573087 SBMLDiagrams-1.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1809 2023-02-23 20:31:51.000000 SBMLDiagrams-1.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 15:53:00.553111 SBMLDiagrams-1.3.6/SBMLDiagrams/
+-rw-rw-rw-   0        0        0      784 2022-02-24 16:03:36.000000 SBMLDiagrams-1.3.6/SBMLDiagrams/__init__.py
+-rw-rw-rw-   0        0        0       71 2023-06-08 15:49:45.000000 SBMLDiagrams-1.3.6/SBMLDiagrams/_version.py
+-rw-rw-rw-   0        0        0   122135 2023-05-16 18:57:09.000000 SBMLDiagrams-1.3.6/SBMLDiagrams/drawNetwork.py
+-rw-rw-rw-   0        0        0   123007 2023-05-16 21:57:52.000000 SBMLDiagrams-1.3.6/SBMLDiagrams/editSBML.py
+-rw-rw-rw-   0        0        0   104489 2023-05-19 17:26:01.000000 SBMLDiagrams-1.3.6/SBMLDiagrams/exportSBML.py
+-rw-rw-rw-   0        0        0     1631 2023-05-16 21:58:12.000000 SBMLDiagrams-1.3.6/SBMLDiagrams/point.py
+-rw-rw-rw-   0        0        0   347877 2023-05-19 17:05:44.000000 SBMLDiagrams-1.3.6/SBMLDiagrams/processSBML.py
+-rw-rw-rw-   0        0        0    10485 2023-05-16 21:58:22.000000 SBMLDiagrams-1.3.6/SBMLDiagrams/styleSBML.py
+-rw-rw-rw-   0        0        0     1194 2023-05-16 21:58:30.000000 SBMLDiagrams-1.3.6/SBMLDiagrams/visualizeInfo.py
+-rw-rw-rw-   0        0        0   157788 2023-05-16 18:57:09.000000 SBMLDiagrams-1.3.6/SBMLDiagrams/visualizeSBML.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:53:00.562087 SBMLDiagrams-1.3.6/SBMLDiagrams.egg-info/
+-rw-rw-rw-   0        0        0     2653 2023-06-08 15:53:00.000000 SBMLDiagrams-1.3.6/SBMLDiagrams.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      473 2023-06-08 15:53:00.000000 SBMLDiagrams-1.3.6/SBMLDiagrams.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 15:53:00.000000 SBMLDiagrams-1.3.6/SBMLDiagrams.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2023-06-08 15:53:00.000000 SBMLDiagrams-1.3.6/SBMLDiagrams.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 15:53:00.000000 SBMLDiagrams-1.3.6/SBMLDiagrams.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-08 15:53:00.574055 SBMLDiagrams-1.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     2034 2023-06-08 15:50:51.000000 SBMLDiagrams-1.3.6/setup.py
```

### Comparing `SBMLDiagrams-1.3.5/PKG-INFO` & `SBMLDiagrams-1.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SBMLDiagrams
-Version: 1.3.5
+Version: 1.3.6
 Summary: Visualize, edit and write SBML files.
-Home-page: https://github.com/SunnyXu/SBMLDiagrams
+Home-page: https://github.com/sys-bio/SBMLDiagrams
 Author: Jin Xu, Jessie Jiang, Herbert M. Sauro
 Author-email: jxu2019@uw.edu
 License: MIT License
 Description: # SBMLDiagrams
         [![Coverage](https://codecov.io/gh/sunnyXu/SBMLDiagrams/branch/main/graph/badge.svg)](https://codecov.io/gh/sunnyXu/SBMLDiagrams)
         
         [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/SBMLDiagrams.svg)](https://badge.fury.io/py/SBMLDiagrams) [![PyPI download month](https://img.shields.io/pypi/dm/ansicolortags.svg)](https://pypi.python.org/pypi/SBMLDiagrams/) ![Funding](https://img.shields.io/badge/Funding-NIH%20(EB028887)-blue)
```

### Comparing `SBMLDiagrams-1.3.5/README.md` & `SBMLDiagrams-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.5/SBMLDiagrams/__init__.py` & `SBMLDiagrams-1.3.6/SBMLDiagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.5/SBMLDiagrams/drawNetwork.py` & `SBMLDiagrams-1.3.6/SBMLDiagrams/drawNetwork.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.5/SBMLDiagrams/editSBML.py` & `SBMLDiagrams-1.3.6/SBMLDiagrams/editSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.5/SBMLDiagrams/exportSBML.py` & `SBMLDiagrams-1.3.6/SBMLDiagrams/exportSBML.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,24 +186,25 @@
         # if the argument for the prefix is missing or empty. Thus the argument
         # for the prefix can be added as follows:
         # 
         #    SBMLNamespaces sbmlns(3,1,"layout",1,"LAYOUT")
         # 
 
         
-        if sbmlStr != "":
+        if sbmlStr != "": 
             document = libsbml.readSBMLFromString(sbmlStr)    
             document.enablePackage(libsbml.LayoutExtension_getXmlnsL3V1V1(), "layout", True)
             
             # set the "required" attribute of layout package  to "true"
             document.setPkgRequired("layout", False)  
             
             model = document.getModel()
             rxn_specRef_id = []
             
+            # to avoid conflicts of species reference ids
             for i in range(numReactions):
                 reaction = model.getReaction(i)
                 reaction_id = reaction.getId()
                 try: #from excel sheet
                     rct_list = list(df_ReactionData.iloc[i]['sources'][1:-1].split(","))
                     prd_list = list(df_ReactionData.iloc[i]['targets'][1:-1].split(","))
                     mod_list = list(df_ReactionData.iloc[i]['modifiers'][1:-1].split(","))
@@ -284,15 +285,15 @@
                         ref_id = "SpecRef_" + reaction_id + "_mod" + str(j)
                         reference.setId(ref_id)
                     mod_specRef_id.append(ref_id)
 
                 temp_rxn_specRef_id = [reaction_id, rct_specRef_id, prd_specRef_id, mod_specRef_id]
                 rxn_specRef_id.append(temp_rxn_specRef_id)
 
-        else:
+        else: #for test_exportSBML.py
             sbmlns = libsbml.SBMLNamespaces(3, 1, "layout", 1)
             # create the document
             document = libsbml.SBMLDocument(sbmlns)
 
             # set the "required" attribute of layout package  to "true"
             document.setPkgRequired("layout", False)  
 
@@ -519,24 +520,24 @@
         # if mplugin is None:
             # print(
             #     "[Fatal Error] Layout Extension Level " + layoutns.getLevel() + " Version " + layoutns.getVersion() + " package version " + layoutns.getPackageVersion() + " is not registered.")
             # sys.exit(1)
         #
         # Creates a Layout object via LayoutModelPlugin object.
         #
-        if mplugin != None:
+        if mplugin != None: #remove existed layout with local render
             numPlugins = mplugin.getNumLayouts()
             for i in range(numPlugins):
                 mplugin.removeLayout(i)
         try: 
             grPlugin = mplugin.getListOfLayouts().getPlugin("render")
         except:
             pass
 
-        if grPlugin != None:
+        if grPlugin != None: #remove existed global render
             numgrPlugin = grPlugin.getNumGlobalRenderInformationObjects()
             for i in range(numgrPlugin):
                 grPlugin.removeGlobalRenderInformation(i)
 
         layout = mplugin.createLayout()
         layout.setId("SBMLDiagrams_layout")
         layout.setDimensions(libsbml.Dimensions(layoutns, layout_width, layout_height))
@@ -733,15 +734,15 @@
                 textGlyph.setBoundingBox(libsbml.BoundingBox(layoutns, bb_id, pos_x_text, pos_y_text, width_text, height_text))
                 #textGlyph.setOriginOfTextId(specG_id)
                 textGlyph.setGraphicalObjectId(specG_id)
 
         # create the ReactionGlyphs and SpeciesReferenceGlyphs
         for i in range(numReactions):
             reaction_id = df_ReactionData.iloc[i]['id']
-            try:
+            try: #for test_exportSBML.py
                 for xx in range(len(rxn_specRef_id)):
                     if rxn_specRef_id[xx][0] == reaction_id:
                         temp_rxn_specRef_id = rxn_specRef_id[xx]
             except:
                 pass
 
             center_size = [0.,0.]
@@ -890,16 +891,17 @@
                 width  = float(center_size[0])
                 height = float(center_size[1])
                 pos_x  = center_value[0]-.5*width
                 pos_y  = center_value[1]-.5*height
                 reactionGlyph.setBoundingBox(libsbml.BoundingBox(layoutns, bb_id, pos_x, pos_y, width, height))
                       
             for j in range(rct_num):
-                try:
-                    if temp_rxn_specRef_id[1] != []:
+                #to make the species reference consistent
+                try: #for test_exportSBML.py if there is no temp_rxn_specRef_id
+                    if temp_rxn_specRef_id[1] != []: #check rct_num error
                         ref_id = temp_rxn_specRef_id[1][j]
                 except:
                     ref_id = "SpecRef_" + reaction_id + "_rct" + str(j)
                 speciesReferenceGlyph = reactionGlyph.createSpeciesReferenceGlyph()
                 specsRefG_id = "SpecRefG_" + reaction_id + "_rct" + str(j)
                 specG_id = "SpecG_" + rct[j] + '_idx_' + str(rct_index[j])
                 speciesReferenceGlyph.setId(specsRefG_id)
```

### Comparing `SBMLDiagrams-1.3.5/SBMLDiagrams/point.py` & `SBMLDiagrams-1.3.6/SBMLDiagrams/point.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.5/SBMLDiagrams/processSBML.py` & `SBMLDiagrams-1.3.6/SBMLDiagrams/processSBML.py`

 * *Files 0% similar despite different names*

```diff
@@ -7016,15 +7016,15 @@
     #long text and alias nodes
     #filename = "test_suite/Jana_WolfGlycolysis/Jana_WolfGlycolysis.xml"
 
     #sbml with errors
     #filename = "test_suite/sbml_error/testbigmodel.xml"
 
     #global render
-    #filename = "test_suite/global_render/global_render.xml"
+    filename = "test_suite/global_render/global_render.xml"
 
     #complex
     #filename = "test_suite/Carcione2020/Carcione2020.xml"
     #filename = "test_suite/Garde2020/Garde2020.xml"
     #filename = "test_suite/test_centroid/test_centroid.xml"
 
 ##############################
@@ -7033,15 +7033,15 @@
     #filename = "Bart/bart_arccenter.xml"
     #filename = "Bart/bart_spRefBezier.xml"
     #filename = "Bart/bart2.xml"
     #filename = "Bart/newSBML.xml"
     #filename = "Bart/newSBML2.xml"
     #filename = "Bart/output.xml"
 
-    filename = "copasi_global/feedback_AssignRuleGlobalRender.xml"
+    #filename = "copasi_global/feedback_AssignRuleGlobalRender.xml"
     #filename = "copasi_global/oscili_V3COPASI.xml"
 
     #filename = "libSBNW/testWithLayout.xml"
 
     #filename = "Sauro-Coyote/branch1.xml"
     #filename = "Sauro-Coyote/branch1-straight.xml"
     #filename = "Sauro-Coyote/branch1-straight2.xml"
```

### Comparing `SBMLDiagrams-1.3.5/SBMLDiagrams/styleSBML.py` & `SBMLDiagrams-1.3.6/SBMLDiagrams/styleSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.5/SBMLDiagrams/visualizeInfo.py` & `SBMLDiagrams-1.3.6/SBMLDiagrams/visualizeInfo.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.5/SBMLDiagrams/visualizeSBML.py` & `SBMLDiagrams-1.3.6/SBMLDiagrams/visualizeSBML.py`

 * *Files identical despite different names*

### Comparing `SBMLDiagrams-1.3.5/SBMLDiagrams.egg-info/PKG-INFO` & `SBMLDiagrams-1.3.6/SBMLDiagrams.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: SBMLDiagrams
-Version: 1.3.5
+Version: 1.3.6
 Summary: Visualize, edit and write SBML files.
-Home-page: https://github.com/SunnyXu/SBMLDiagrams
+Home-page: https://github.com/sys-bio/SBMLDiagrams
 Author: Jin Xu, Jessie Jiang, Herbert M. Sauro
 Author-email: jxu2019@uw.edu
 License: MIT License
 Description: # SBMLDiagrams
         [![Coverage](https://codecov.io/gh/sunnyXu/SBMLDiagrams/branch/main/graph/badge.svg)](https://codecov.io/gh/sunnyXu/SBMLDiagrams)
         
         [![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) [![PyPI version](https://badge.fury.io/py/SBMLDiagrams.svg)](https://badge.fury.io/py/SBMLDiagrams) [![PyPI download month](https://img.shields.io/pypi/dm/ansicolortags.svg)](https://pypi.python.org/pypi/SBMLDiagrams/) ![Funding](https://img.shields.io/badge/Funding-NIH%20(EB028887)-blue)
```

### Comparing `SBMLDiagrams-1.3.5/setup.py` & `SBMLDiagrams-1.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     packages=['SBMLDiagrams'],
     version=get_version('SBMLDiagrams/_version.py'),
     description='Visualize, edit and write SBML files.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jin Xu, Jessie Jiang, Herbert M. Sauro',
     author_email='jxu2019@uw.edu',
-    url='https://github.com/SunnyXu/SBMLDiagrams',
+    url='https://github.com/sys-bio/SBMLDiagrams',
     license='MIT License',
     install_requires=[
         'coverage',
         'pip>20',
         'numpy',
         'pandas',
         'python-libsbml',
```

