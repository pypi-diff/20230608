# Comparing `tmp/similarnames-0.1.6.tar.gz` & `tmp/similarnames-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "similarnames-0.1.6.tar", max compression
+gzip compressed data, was "similarnames-0.1.7.tar", max compression
```

## Comparing `similarnames-0.1.6.tar` & `similarnames-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1094 2022-08-06 17:33:25.042373 similarnames-0.1.6/LICENSE
--rw-r--r--   0        0        0      589 2022-08-11 00:53:36.854847 similarnames-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5229 2022-08-06 21:38:58.625940 similarnames-0.1.6/README.md
--rw-r--r--   0        0        0      766 2022-08-11 00:52:21.478137 similarnames-0.1.6/similarnames/__init__.py
--rw-r--r--   0        0        0     2928 2022-08-11 00:51:16.966884 similarnames-0.1.6/similarnames/similarnames.py
--rw-r--r--   0        0        0     6186 2022-08-11 00:54:04.661896 similarnames-0.1.6/setup.py
--rw-r--r--   0        0        0     6006 2022-08-11 00:54:04.661896 similarnames-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1094 2022-08-06 17:33:25.042373 similarnames-0.1.7/LICENSE
+-rw-r--r--   0        0        0      589 2023-06-08 13:28:14.769488 similarnames-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5246 2023-06-08 13:23:42.244067 similarnames-0.1.7/README.md
+-rw-r--r--   0        0        0      775 2023-06-08 13:29:00.859422 similarnames-0.1.7/similarnames/__init__.py
+-rw-r--r--   0        0        0     2992 2023-06-08 13:15:05.133962 similarnames-0.1.7/similarnames/similarnames.py
+-rw-r--r--   0        0        0     6203 2023-06-08 13:32:22.878781 similarnames-0.1.7/setup.py
+-rw-r--r--   0        0        0     6023 2023-06-08 13:32:22.879785 similarnames-0.1.7/PKG-INFO
```

### Comparing `similarnames-0.1.6/LICENSE` & `similarnames-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `similarnames-0.1.6/pyproject.toml` & `similarnames-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "similarnames"
-version = "0.1.6"
+version = "0.1.7"
 description = "Library for Standardizing names from a Pandas dataframe"
 authors = ["paulobrunheroto <paulobrunheroto@hotmail.com>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = 'https://github.com/paulobrunheroto/similarnames'
 repository = 'https://github.com/paulobrunheroto/similarnames'
```

### Comparing `similarnames-0.1.6/README.md` & `similarnames-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 # Similar Names
 Library for Standardizing names from a Pandas dataframe
 
 ## Description
-Similar Names is basically a package for names manipulation. That is, if you have a Pandas dataframe with multiple names written in different ways (e.g.: John Doe, John E. Doe and John Edson Doe), the "closeMatches" function will look for all similar names on that column and then add two columns: "Close Matches" (list of all close matches) and "StandardName" (shortest name of the list).
+Similar Names is basically a package for names manipulation. That is, if you have a Pandas dataframe with multiple names written in different ways (e.g.: John Doe, John E. Doe and John Edson Doe), the "close_matches" function will look for all similar names on that column and then add two columns: "Close Matches" (list of all close matches) and "standard_name" (shortest name of the list).
 
 ## Instalation
 Similar Names can be installed directly through pip
 ```
 pip install similarnames
 ```
 
 ## How to use?
-If you have a pandas dataframe with the names that you want to standardize, or look for close matches, simply follow the steps described next. As for the "closeMatches" parameters, they are basically 6:
+If you have a pandas dataframe with the names that you want to standardize, or look for close matches, simply follow the steps described next. As for the "close_matches" parameters, they are basically 6:
 ```python
-closeMatches(obj, names, sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], customWords = None)
+close_matches(obj, names, sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], custom_words = None)
 ```
 - obj (dataframe): The pandas dataframe
 - names (str): The name of the pandas dataframe with the names that you want to analyze
 - sep (str or None): The separator to be used to split multiple names
 - connectors (str, list or None): Words to also be used as separators (e.g.: "and")
 - languages (str, list or None): Lanaguages for the default stopwords config (All stopwords are not considered names)
-- customWords (str, list or None): Additional words that should not be considered as names (e.g.: "jr")
+- custom_words (str, list or None): Additional words that should not be considered as names (e.g.: "jr")
 
 ### 1st Scenario: 1 name per row
-In case your dataframe is already formatted with one name per row, simply execute the following command setting the "sep" parameter to "None". In case you are having some trouble with the results, you can set the "languages" and "customWords" parameters to include, or exclude, names from the analyses (by default, stopwords in english, portuguese and spanish are not considered names).
+In case your dataframe is already formatted with one name per row, simply execute the following command setting the "sep" parameter to "None". In case you are having some trouble with the results, you can set the "languages" and "custom_words" parameters to include, or exclude, names from the analyses (by default, stopwords in english, portuguese and spanish are not considered names).
 
 ```python
 '''
 Input (df): df and the name of the column with the names to check
 
 | Names          | ... |
 |----------------|-----|
 | John Doe       |     |
 | John Edson Doe |     |
 | John E. Doe    |     |
 | John Edson D.  |     |
 '''
-from similarnames import closeMatches
+from similarnames import close_matches
 
-# Default config: sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], customWords = None
-df_standard = closeMatches(df, 'Names', sep = None)
+# Default config: sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], custom_words = None
+df_standard = close_matches(df, 'Names', sep = None)
 
 '''
 Output (df_standard)
 
-| Names          | ... | CloseMatches                                                   | StandardName |
+| Names          | ... | close_matches                                                   | standard_name |
 |----------------|-----|----------------------------------------------------------------|--------------|
 | John Doe       |     | ['John Doe', 'John E. Doe', 'John Edson Doe', 'John Edson D.'] | John Doe     |
 | John Edson Doe |     | ['John Doe', 'John E. Doe', 'John Edson Doe', 'John Edson D.'] | John Doe     |
 | John E. Doe    |     | ['John Doe', 'John E. Doe', 'John Edson Doe', 'John Edson D.'] | John Doe     |
 | John Edson D.  |     | ['John Doe', 'John E. Doe', 'John Edson Doe', 'John Edson D.'] | John Doe     |
 
 '''
@@ -62,23 +62,23 @@
 
 | Names                                        | Other columns           | ... |
 |----------------------------------------------|-------------------------|-----|
 | John Doe, Jane Doe                           | Two names (sep = ',')   |     |
 | John E. Doe and Michael Johnson              | Two names (without sep) |     |
 | Jane A. Doe, Michael M. Johnson and John Doe | Three names (sep = ',') |     |
 '''
-from similarnames import closeMatches
+from similarnames import close_matches
 
-# Default config: sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], customWords = None
-df_standard = closeMatches(df, 'Names', sep = ',')
+# Default config: sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], custom_words = None
+df_standard = close_matches(df, 'Names', sep = ',')
 
 '''
 Output (df_standard)
 
-| Names              | Other columns           | ... | CloseMatches                              | StandardName    |
+| Names              | Other columns           | ... | close_matches                              | standard_name    |
 |--------------------|-------------------------|-----|-------------------------------------------|-----------------|
 | John Doe           | Two names (sep = ',')   |     | ['John Doe', 'John E. Doe']               | John Doe        |
 | Jane Doe           | Two names (sep = ',')   |     | ['Jane Doe', 'Jane A. Doe']               | Jane Doe        |
 | John E. Doe        | Two names (without sep) |     | ['John Doe', 'John E. Doe']               | John Doe        |
 | Michael Johnson    | Two names (without sep) |     | ['Michael Johnson', 'Michael M. Johnson'] | Michael Johnson |
 | Jane A. Doe        | Three names (sep = ',') |     | ['Jane Doe', 'Jane A. Doe']               | Jane Doe        |
 | Michael M. Johnson | Three names (sep = ',') |     | ['Michael Johnson', 'Michael M. Johnson'] | Michael Johnson |
```

### Comparing `similarnames-0.1.6/similarnames/__init__.py` & `similarnames-0.1.7/similarnames/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-__version__ = '0.1.6'
+__version__ = '0.1.7'
 
 from .similarnames import SimilarNames
 
-def closeMatches(obj, names, sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], customWords = None):
+def close_matches(obj, names, sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], custom_words = None):
     if connectors == None:
         connectors = []
     else:
         if not isinstance(connectors, list):
             connectors = [connectors]
 
     if languages == None:
         languages = []
     else:
         if not isinstance(languages, list):
             languages = [languages]
 
-    if customWords == None:
-        customWords = []
+    if custom_words == None:
+        custom_words = []
     else:
-        if not isinstance(customWords, list):
-            customWords = [customWords]
+        if not isinstance(custom_words, list):
+            custom_words = [custom_words]
 
     sn = SimilarNames()
-    return sn.closeMatches(obj, names, sep, connectors, languages, customWords)
+    return sn.close_matches(obj, names, sep, connectors, languages, custom_words)
```

### Comparing `similarnames-0.1.6/similarnames/similarnames.py` & `similarnames-0.1.7/similarnames/similarnames.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,90 +1,90 @@
 from unidecode import unidecode
 from nltk.corpus import stopwords
 
 class SimilarNames():
 
-    def allNames(self):
-        self.dictNames = {}
+    def all_names(self):
+        self.dict_names = {}
         for name in self.df[self.names].unique():
-            self.dictNames[name] = self.normName(name)
+            self.dict_names[name] = self.norm_name(name)
 
-    def uniqueNames(self):
-        self.similarList = []
-        for name in self.dictNames.keys():
-            self.similarList += [self.getSimilar(self.dictNames[name])]
+    def unique_names(self):
+        self.similar_list = []
+        for name in self.dict_names.keys():
+            self.similar_list += [self.get_similar(self.dict_names[name])]
         
-        self.uniqueList = []
-        for elem in self.similarList:
-            if elem not in self.uniqueList:
-                self.uniqueList.append(elem)
+        self.unique_list = []
+        for elem in self.similar_list:
+            if elem not in self.unique_list:
+                self.unique_list.append(elem)
 
-    def closeMatches(self, obj, names, sep, connectors, languages, customWords):
+    def close_matches(self, obj, names, sep, connectors, languages, custom_words):
         self.sep = sep
         self.connectors = connectors
 
-        self.stopList = []
+        self.stop_list = []
         for l in languages:
-            self.stopList += stopwords.words(l)
-        self.stopList += customWords
+            self.stop_list += stopwords.words(l)
+        self.stop_list += custom_words
 
         self.df = obj.copy()
         self.names = names
 
         if self.sep != None:
-            self.df[self.names] = [self.nameSplit(x) for x in self.df[self.names]]
+            self.df[self.names] = [self.name_split(x) for x in self.df[self.names]]
             self.df = self.df.explode('Authors')
         
-        self.df['NormName'] = [self.normName(x) for x in self.df[self.names]]
-        self.allNames()
-        self.uniqueNames()
+        self.df['norm_name'] = [self.norm_name(x) for x in self.df[self.names]]
+        self.all_names()
+        self.unique_names()
     
-        self.df['CloseMatches'] = [self.getSimilar(x) for x in self.df['NormName']]
+        self.df['close_matches'] = [self.get_similar(x) for x in self.df['norm_name']]
 
-        self.df['CloseMatches'] = [self.getMaxList(x) for x in self.df['CloseMatches']]
+        self.df['close_matches'] = [self.get_max_list(x) for x in self.df['close_matches']]
 
-        self.df['StandardName'] = [self.getMinName(x) for x in self.df['CloseMatches']]
+        self.df['StandardName'] = [self.get_min_name(x) for x in self.df['close_matches']]
         
-        self.df.drop(columns = 'NormName', inplace = True)
+        self.df.drop(columns = 'norm_name', inplace = True)
         
         return self.df
 
-    def nameSplit(self, name):
+    def name_split(self, name):
         for c in self.connectors:
             name = name.replace(f' {c} ', ', ')
         return [x.strip() for x in name.split(self.sep)]
 
-    def lowName(self, names):
-        minName = names[0]
+    def low_name(self, names):
+        min_name = names[0]
         for name in names:
-            if len(name) < len(minName):
-                minName = name
-        return minName
+            if len(name) < len(min_name):
+                min_name = name
+        return min_name
 
-    def normName(self, name):
+    def norm_name(self, name):
         name = unidecode(name.lower()).replace('-',' ').replace('.', '').split()
-        name = [x.strip() for x in name if x not in self.stopList and len(x) > 1]
+        name = [x.strip() for x in name if x not in self.stop_list and len(x) > 1]
         return name
 
-    def getSimilar(self, name):
-        similarList = []    
-        for n in self.dictNames.keys():
-            if name[0] == self.dictNames[n][0] and len(set(name).intersection(self.dictNames[n])) >= 2:
-                similarList += [n]
-        if len(similarList) < 1:
+    def get_similar(self, name):
+        similar_list = []    
+        for n in self.dict_names.keys():
+            if name[0] == self.dict_names[n][0] and len(set(name).intersection(self.dict_names[n])) >= 2:
+                similar_list += [n]
+        if len(similar_list) < 1:
             return [f'Not found: {name}']
         else:
-            return similarList
+            return similar_list
 
-    def getMaxList(self, names):
-        maxList = names
-        for dup in self.uniqueList:
+    def get_max_list(self, names):
+        max_list = names
+        for dup in self.unique_list:
             if len(set(names).intersection(dup)) >= 2 and len(dup) > len(names):
-                maxList = dup
-        return maxList
+                max_list = dup
+        return max_list
 
-    def getMinName(self, names):
-        minName = names[0]
+    def get_min_name(self, names):
+        min_name = names[0]
         for name in names:
-            if len(name) < len(minName):
-                minName = name
-        return minName
+            if len(name) < len(min_name):
+                min_name = name
+        return min_name
```

### Comparing `similarnames-0.1.6/setup.py` & `similarnames-0.1.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['nltk>=3.7,<4.0', 'unidecode>=1.3.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'similarnames',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Library for Standardizing names from a Pandas dataframe',
-    'long_description': '# Similar Names\nLibrary for Standardizing names from a Pandas dataframe\n\n## Description\nSimilar Names is basically a package for names manipulation. That is, if you have a Pandas dataframe with multiple names written in different ways (e.g.: John Doe, John E. Doe and John Edson Doe), the "closeMatches" function will look for all similar names on that column and then add two columns: "Close Matches" (list of all close matches) and "StandardName" (shortest name of the list).\n\n## Instalation\nSimilar Names can be installed directly through pip\n```\npip install similarnames\n```\n\n## How to use?\nIf you have a pandas dataframe with the names that you want to standardize, or look for close matches, simply follow the steps described next. As for the "closeMatches" parameters, they are basically 6:\n```python\ncloseMatches(obj, names, sep = \',\', connectors = [\'and\',\'e\',\'y\'], languages = [\'english\', \'portuguese\', \'spanish\'], customWords = None)\n```\n- obj (dataframe): The pandas dataframe\n- names (str): The name of the pandas dataframe with the names that you want to analyze\n- sep (str or None): The separator to be used to split multiple names\n- connectors (str, list or None): Words to also be used as separators (e.g.: "and")\n- languages (str, list or None): Lanaguages for the default stopwords config (All stopwords are not considered names)\n- customWords (str, list or None): Additional words that should not be considered as names (e.g.: "jr")\n\n### 1st Scenario: 1 name per row\nIn case your dataframe is already formatted with one name per row, simply execute the following command setting the "sep" parameter to "None". In case you are having some trouble with the results, you can set the "languages" and "customWords" parameters to include, or exclude, names from the analyses (by default, stopwords in english, portuguese and spanish are not considered names).\n\n```python\n\'\'\'\nInput (df): df and the name of the column with the names to check\n\n| Names          | ... |\n|----------------|-----|\n| John Doe       |     |\n| John Edson Doe |     |\n| John E. Doe    |     |\n| John Edson D.  |     |\n\'\'\'\nfrom similarnames import closeMatches\n\n# Default config: sep = \',\', connectors = [\'and\',\'e\',\'y\'], languages = [\'english\', \'portuguese\', \'spanish\'], customWords = None\ndf_standard = closeMatches(df, \'Names\', sep = None)\n\n\'\'\'\nOutput (df_standard)\n\n| Names          | ... | CloseMatches                                                   | StandardName |\n|----------------|-----|----------------------------------------------------------------|--------------|\n| John Doe       |     | [\'John Doe\', \'John E. Doe\', \'John Edson Doe\', \'John Edson D.\'] | John Doe     |\n| John Edson Doe |     | [\'John Doe\', \'John E. Doe\', \'John Edson Doe\', \'John Edson D.\'] | John Doe     |\n| John E. Doe    |     | [\'John Doe\', \'John E. Doe\', \'John Edson Doe\', \'John Edson D.\'] | John Doe     |\n| John Edson D.  |     | [\'John Doe\', \'John E. Doe\', \'John Edson Doe\', \'John Edson D.\'] | John Doe     |\n\n\'\'\'\n```\n### 2nd Scenario: Multiple names per row\nIn case you have multiple names in a single row, the "explode" is automatically done for you. So, just provide the "sep" parameter to identify where we should use to split those names. By default, the connectors "and", "e" and "y" will also be considered as separators. Therefore, in case you are working in a different language, just set the "connectors" and "languagues" parameter as you wish.\n\n```python\n\'\'\'\nInput (df): df and the name of the column with the names to check\n\n| Names                                        | Other columns           | ... |\n|----------------------------------------------|-------------------------|-----|\n| John Doe, Jane Doe                           | Two names (sep = \',\')   |     |\n| John E. Doe and Michael Johnson              | Two names (without sep) |     |\n| Jane A. Doe, Michael M. Johnson and John Doe | Three names (sep = \',\') |     |\n\'\'\'\nfrom similarnames import closeMatches\n\n# Default config: sep = \',\', connectors = [\'and\',\'e\',\'y\'], languages = [\'english\', \'portuguese\', \'spanish\'], customWords = None\ndf_standard = closeMatches(df, \'Names\', sep = \',\')\n\n\'\'\'\nOutput (df_standard)\n\n| Names              | Other columns           | ... | CloseMatches                              | StandardName    |\n|--------------------|-------------------------|-----|-------------------------------------------|-----------------|\n| John Doe           | Two names (sep = \',\')   |     | [\'John Doe\', \'John E. Doe\']               | John Doe        |\n| Jane Doe           | Two names (sep = \',\')   |     | [\'Jane Doe\', \'Jane A. Doe\']               | Jane Doe        |\n| John E. Doe        | Two names (without sep) |     | [\'John Doe\', \'John E. Doe\']               | John Doe        |\n| Michael Johnson    | Two names (without sep) |     | [\'Michael Johnson\', \'Michael M. Johnson\'] | Michael Johnson |\n| Jane A. Doe        | Three names (sep = \',\') |     | [\'Jane Doe\', \'Jane A. Doe\']               | Jane Doe        |\n| Michael M. Johnson | Three names (sep = \',\') |     | [\'Michael Johnson\', \'Michael M. Johnson\'] | Michael Johnson |\n| John Doe           | Three names (sep = \',\') |     | [\'John Doe\', \'John E. Doe\']               | John Doe        |\n\n\'\'\'\n```\n',
+    'long_description': '# Similar Names\nLibrary for Standardizing names from a Pandas dataframe\n\n## Description\nSimilar Names is basically a package for names manipulation. That is, if you have a Pandas dataframe with multiple names written in different ways (e.g.: John Doe, John E. Doe and John Edson Doe), the "close_matches" function will look for all similar names on that column and then add two columns: "Close Matches" (list of all close matches) and "standard_name" (shortest name of the list).\n\n## Instalation\nSimilar Names can be installed directly through pip\n```\npip install similarnames\n```\n\n## How to use?\nIf you have a pandas dataframe with the names that you want to standardize, or look for close matches, simply follow the steps described next. As for the "close_matches" parameters, they are basically 6:\n```python\nclose_matches(obj, names, sep = \',\', connectors = [\'and\',\'e\',\'y\'], languages = [\'english\', \'portuguese\', \'spanish\'], custom_words = None)\n```\n- obj (dataframe): The pandas dataframe\n- names (str): The name of the pandas dataframe with the names that you want to analyze\n- sep (str or None): The separator to be used to split multiple names\n- connectors (str, list or None): Words to also be used as separators (e.g.: "and")\n- languages (str, list or None): Lanaguages for the default stopwords config (All stopwords are not considered names)\n- custom_words (str, list or None): Additional words that should not be considered as names (e.g.: "jr")\n\n### 1st Scenario: 1 name per row\nIn case your dataframe is already formatted with one name per row, simply execute the following command setting the "sep" parameter to "None". In case you are having some trouble with the results, you can set the "languages" and "custom_words" parameters to include, or exclude, names from the analyses (by default, stopwords in english, portuguese and spanish are not considered names).\n\n```python\n\'\'\'\nInput (df): df and the name of the column with the names to check\n\n| Names          | ... |\n|----------------|-----|\n| John Doe       |     |\n| John Edson Doe |     |\n| John E. Doe    |     |\n| John Edson D.  |     |\n\'\'\'\nfrom similarnames import close_matches\n\n# Default config: sep = \',\', connectors = [\'and\',\'e\',\'y\'], languages = [\'english\', \'portuguese\', \'spanish\'], custom_words = None\ndf_standard = close_matches(df, \'Names\', sep = None)\n\n\'\'\'\nOutput (df_standard)\n\n| Names          | ... | close_matches                                                   | standard_name |\n|----------------|-----|----------------------------------------------------------------|--------------|\n| John Doe       |     | [\'John Doe\', \'John E. Doe\', \'John Edson Doe\', \'John Edson D.\'] | John Doe     |\n| John Edson Doe |     | [\'John Doe\', \'John E. Doe\', \'John Edson Doe\', \'John Edson D.\'] | John Doe     |\n| John E. Doe    |     | [\'John Doe\', \'John E. Doe\', \'John Edson Doe\', \'John Edson D.\'] | John Doe     |\n| John Edson D.  |     | [\'John Doe\', \'John E. Doe\', \'John Edson Doe\', \'John Edson D.\'] | John Doe     |\n\n\'\'\'\n```\n### 2nd Scenario: Multiple names per row\nIn case you have multiple names in a single row, the "explode" is automatically done for you. So, just provide the "sep" parameter to identify where we should use to split those names. By default, the connectors "and", "e" and "y" will also be considered as separators. Therefore, in case you are working in a different language, just set the "connectors" and "languagues" parameter as you wish.\n\n```python\n\'\'\'\nInput (df): df and the name of the column with the names to check\n\n| Names                                        | Other columns           | ... |\n|----------------------------------------------|-------------------------|-----|\n| John Doe, Jane Doe                           | Two names (sep = \',\')   |     |\n| John E. Doe and Michael Johnson              | Two names (without sep) |     |\n| Jane A. Doe, Michael M. Johnson and John Doe | Three names (sep = \',\') |     |\n\'\'\'\nfrom similarnames import close_matches\n\n# Default config: sep = \',\', connectors = [\'and\',\'e\',\'y\'], languages = [\'english\', \'portuguese\', \'spanish\'], custom_words = None\ndf_standard = close_matches(df, \'Names\', sep = \',\')\n\n\'\'\'\nOutput (df_standard)\n\n| Names              | Other columns           | ... | close_matches                              | standard_name    |\n|--------------------|-------------------------|-----|-------------------------------------------|-----------------|\n| John Doe           | Two names (sep = \',\')   |     | [\'John Doe\', \'John E. Doe\']               | John Doe        |\n| Jane Doe           | Two names (sep = \',\')   |     | [\'Jane Doe\', \'Jane A. Doe\']               | Jane Doe        |\n| John E. Doe        | Two names (without sep) |     | [\'John Doe\', \'John E. Doe\']               | John Doe        |\n| Michael Johnson    | Two names (without sep) |     | [\'Michael Johnson\', \'Michael M. Johnson\'] | Michael Johnson |\n| Jane A. Doe        | Three names (sep = \',\') |     | [\'Jane Doe\', \'Jane A. Doe\']               | Jane Doe        |\n| Michael M. Johnson | Three names (sep = \',\') |     | [\'Michael Johnson\', \'Michael M. Johnson\'] | Michael Johnson |\n| John Doe           | Three names (sep = \',\') |     | [\'John Doe\', \'John E. Doe\']               | John Doe        |\n\n\'\'\'\n```\n',
     'author': 'paulobrunheroto',
     'author_email': 'paulobrunheroto@hotmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/paulobrunheroto/similarnames',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `similarnames-0.1.6/PKG-INFO` & `similarnames-0.1.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: similarnames
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library for Standardizing names from a Pandas dataframe
 Home-page: https://github.com/paulobrunheroto/similarnames
 License: MIT
 Author: paulobrunheroto
 Author-email: paulobrunheroto@hotmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -18,57 +18,57 @@
 Project-URL: Repository, https://github.com/paulobrunheroto/similarnames
 Description-Content-Type: text/markdown
 
 # Similar Names
 Library for Standardizing names from a Pandas dataframe
 
 ## Description
-Similar Names is basically a package for names manipulation. That is, if you have a Pandas dataframe with multiple names written in different ways (e.g.: John Doe, John E. Doe and John Edson Doe), the "closeMatches" function will look for all similar names on that column and then add two columns: "Close Matches" (list of all close matches) and "StandardName" (shortest name of the list).
+Similar Names is basically a package for names manipulation. That is, if you have a Pandas dataframe with multiple names written in different ways (e.g.: John Doe, John E. Doe and John Edson Doe), the "close_matches" function will look for all similar names on that column and then add two columns: "Close Matches" (list of all close matches) and "standard_name" (shortest name of the list).
 
 ## Instalation
 Similar Names can be installed directly through pip
 ```
 pip install similarnames
 ```
 
 ## How to use?
-If you have a pandas dataframe with the names that you want to standardize, or look for close matches, simply follow the steps described next. As for the "closeMatches" parameters, they are basically 6:
+If you have a pandas dataframe with the names that you want to standardize, or look for close matches, simply follow the steps described next. As for the "close_matches" parameters, they are basically 6:
 ```python
-closeMatches(obj, names, sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], customWords = None)
+close_matches(obj, names, sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], custom_words = None)
 ```
 - obj (dataframe): The pandas dataframe
 - names (str): The name of the pandas dataframe with the names that you want to analyze
 - sep (str or None): The separator to be used to split multiple names
 - connectors (str, list or None): Words to also be used as separators (e.g.: "and")
 - languages (str, list or None): Lanaguages for the default stopwords config (All stopwords are not considered names)
-- customWords (str, list or None): Additional words that should not be considered as names (e.g.: "jr")
+- custom_words (str, list or None): Additional words that should not be considered as names (e.g.: "jr")
 
 ### 1st Scenario: 1 name per row
-In case your dataframe is already formatted with one name per row, simply execute the following command setting the "sep" parameter to "None". In case you are having some trouble with the results, you can set the "languages" and "customWords" parameters to include, or exclude, names from the analyses (by default, stopwords in english, portuguese and spanish are not considered names).
+In case your dataframe is already formatted with one name per row, simply execute the following command setting the "sep" parameter to "None". In case you are having some trouble with the results, you can set the "languages" and "custom_words" parameters to include, or exclude, names from the analyses (by default, stopwords in english, portuguese and spanish are not considered names).
 
 ```python
 '''
 Input (df): df and the name of the column with the names to check
 
 | Names          | ... |
 |----------------|-----|
 | John Doe       |     |
 | John Edson Doe |     |
 | John E. Doe    |     |
 | John Edson D.  |     |
 '''
-from similarnames import closeMatches
+from similarnames import close_matches
 
-# Default config: sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], customWords = None
-df_standard = closeMatches(df, 'Names', sep = None)
+# Default config: sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], custom_words = None
+df_standard = close_matches(df, 'Names', sep = None)
 
 '''
 Output (df_standard)
 
-| Names          | ... | CloseMatches                                                   | StandardName |
+| Names          | ... | close_matches                                                   | standard_name |
 |----------------|-----|----------------------------------------------------------------|--------------|
 | John Doe       |     | ['John Doe', 'John E. Doe', 'John Edson Doe', 'John Edson D.'] | John Doe     |
 | John Edson Doe |     | ['John Doe', 'John E. Doe', 'John Edson Doe', 'John Edson D.'] | John Doe     |
 | John E. Doe    |     | ['John Doe', 'John E. Doe', 'John Edson Doe', 'John Edson D.'] | John Doe     |
 | John Edson D.  |     | ['John Doe', 'John E. Doe', 'John Edson Doe', 'John Edson D.'] | John Doe     |
 
 '''
@@ -82,23 +82,23 @@
 
 | Names                                        | Other columns           | ... |
 |----------------------------------------------|-------------------------|-----|
 | John Doe, Jane Doe                           | Two names (sep = ',')   |     |
 | John E. Doe and Michael Johnson              | Two names (without sep) |     |
 | Jane A. Doe, Michael M. Johnson and John Doe | Three names (sep = ',') |     |
 '''
-from similarnames import closeMatches
+from similarnames import close_matches
 
-# Default config: sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], customWords = None
-df_standard = closeMatches(df, 'Names', sep = ',')
+# Default config: sep = ',', connectors = ['and','e','y'], languages = ['english', 'portuguese', 'spanish'], custom_words = None
+df_standard = close_matches(df, 'Names', sep = ',')
 
 '''
 Output (df_standard)
 
-| Names              | Other columns           | ... | CloseMatches                              | StandardName    |
+| Names              | Other columns           | ... | close_matches                              | standard_name    |
 |--------------------|-------------------------|-----|-------------------------------------------|-----------------|
 | John Doe           | Two names (sep = ',')   |     | ['John Doe', 'John E. Doe']               | John Doe        |
 | Jane Doe           | Two names (sep = ',')   |     | ['Jane Doe', 'Jane A. Doe']               | Jane Doe        |
 | John E. Doe        | Two names (without sep) |     | ['John Doe', 'John E. Doe']               | John Doe        |
 | Michael Johnson    | Two names (without sep) |     | ['Michael Johnson', 'Michael M. Johnson'] | Michael Johnson |
 | Jane A. Doe        | Three names (sep = ',') |     | ['Jane Doe', 'Jane A. Doe']               | Jane Doe        |
 | Michael M. Johnson | Three names (sep = ',') |     | ['Michael Johnson', 'Michael M. Johnson'] | Michael Johnson |
```

