# Comparing `tmp/pyhelpers-1.5.0.tar.gz` & `tmp/pyhelpers-1.5.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelpers-1.5.0.tar", last modified: Thu Jun  8 12:15:32 2023, max compression
+gzip compressed data, was "pyhelpers-1.5.0rc2.tar", last modified: Wed Jun  7 09:17:50 2023, max compression
```

## Comparing `pyhelpers-1.5.0.tar` & `pyhelpers-1.5.0rc2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 12:15:32.834231 pyhelpers-1.5.0/
--rw-rw-rw-   0        0        0    35823 2022-02-10 15:02:05.000000 pyhelpers-1.5.0/LICENSE
--rw-rw-rw-   0        0        0       44 2023-06-07 08:24:32.000000 pyhelpers-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5173 2023-06-08 12:15:32.835230 pyhelpers-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     3995 2023-06-08 12:14:59.000000 pyhelpers-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 12:15:32.807104 pyhelpers-1.5.0/pyhelpers/
--rw-rw-rw-   0        0        0      769 2023-04-22 20:54:53.000000 pyhelpers-1.5.0/pyhelpers/__init__.py
--rw-rw-rw-   0        0        0    12333 2023-06-02 08:17:59.000000 pyhelpers-1.5.0/pyhelpers/_cache.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:15:32.833262 pyhelpers-1.5.0/pyhelpers/data/
--rw-rw-rw-   0        0        0     1763 2023-04-22 21:26:53.000000 pyhelpers-1.5.0/pyhelpers/data/english-numerals.json
--rw-rw-rw-   0        0        0      438 2023-06-07 09:52:17.000000 pyhelpers-1.5.0/pyhelpers/data/metadata.json
--rw-rw-rw-   0        0        0   483581 2023-06-02 09:31:29.000000 pyhelpers-1.5.0/pyhelpers/data/user-agent-strings.json
--rw-rw-rw-   0        0        0      764 2022-03-11 11:56:34.000000 pyhelpers-1.5.0/pyhelpers/data/xlsx2csv.vbs
--rw-rw-rw-   0        0        0   175426 2023-06-02 09:33:23.000000 pyhelpers-1.5.0/pyhelpers/dbms.py
--rw-rw-rw-   0        0        0    25930 2023-05-26 16:05:35.000000 pyhelpers-1.5.0/pyhelpers/dirs.py
--rw-rw-rw-   0        0        0    55052 2023-05-21 19:20:56.000000 pyhelpers-1.5.0/pyhelpers/geom.py
--rw-rw-rw-   0        0        0    85647 2023-06-02 08:38:46.000000 pyhelpers-1.5.0/pyhelpers/ops.py
--rw-rw-rw-   0        0        0    18142 2023-05-21 19:18:12.000000 pyhelpers-1.5.0/pyhelpers/settings.py
--rw-rw-rw-   0        0        0    86327 2023-06-08 10:53:19.000000 pyhelpers-1.5.0/pyhelpers/store.py
--rw-rw-rw-   0        0        0    24373 2023-05-21 18:41:23.000000 pyhelpers-1.5.0/pyhelpers/text.py
-drwxrwxrwx   0        0        0        0 2023-06-08 12:15:32.820056 pyhelpers-1.5.0/pyhelpers.egg-info/
--rw-rw-rw-   0        0        0     5173 2023-06-08 12:15:32.000000 pyhelpers-1.5.0/pyhelpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-06-08 12:15:32.000000 pyhelpers-1.5.0/pyhelpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 12:15:32.000000 pyhelpers-1.5.0/pyhelpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2023-06-08 12:15:32.000000 pyhelpers-1.5.0/pyhelpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-08 12:15:32.000000 pyhelpers-1.5.0/pyhelpers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2023-05-20 14:30:39.000000 pyhelpers-1.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      964 2023-06-08 12:15:32.837223 pyhelpers-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-05-22 10:01:48.000000 pyhelpers-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:17:50.910680 pyhelpers-1.5.0rc2/
+-rw-rw-rw-   0        0        0    35823 2022-02-10 15:02:05.000000 pyhelpers-1.5.0rc2/LICENSE
+-rw-rw-rw-   0        0        0       44 2023-06-07 08:24:32.000000 pyhelpers-1.5.0rc2/MANIFEST.in
+-rw-rw-rw-   0        0        0     5136 2023-06-07 09:17:50.910680 pyhelpers-1.5.0rc2/PKG-INFO
+-rw-rw-rw-   0        0        0     3952 2023-06-07 09:17:04.000000 pyhelpers-1.5.0rc2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 09:17:50.889693 pyhelpers-1.5.0rc2/pyhelpers/
+-rw-rw-rw-   0        0        0      769 2023-04-22 20:54:53.000000 pyhelpers-1.5.0rc2/pyhelpers/__init__.py
+-rw-rw-rw-   0        0        0    12333 2023-06-02 08:17:59.000000 pyhelpers-1.5.0rc2/pyhelpers/_cache.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:17:50.908682 pyhelpers-1.5.0rc2/pyhelpers/data/
+-rw-rw-rw-   0        0        0     1763 2023-04-22 21:26:53.000000 pyhelpers-1.5.0rc2/pyhelpers/data/english-numerals.json
+-rw-rw-rw-   0        0        0      441 2023-06-07 09:17:22.000000 pyhelpers-1.5.0rc2/pyhelpers/data/metadata.json
+-rw-rw-rw-   0        0        0   483581 2023-06-02 09:31:29.000000 pyhelpers-1.5.0rc2/pyhelpers/data/user-agent-strings.json
+-rw-rw-rw-   0        0        0      764 2022-03-11 11:56:34.000000 pyhelpers-1.5.0rc2/pyhelpers/data/xlsx2csv.vbs
+-rw-rw-rw-   0        0        0   175426 2023-06-02 09:33:23.000000 pyhelpers-1.5.0rc2/pyhelpers/dbms.py
+-rw-rw-rw-   0        0        0    25930 2023-05-26 16:05:35.000000 pyhelpers-1.5.0rc2/pyhelpers/dirs.py
+-rw-rw-rw-   0        0        0    55052 2023-05-21 19:20:56.000000 pyhelpers-1.5.0rc2/pyhelpers/geom.py
+-rw-rw-rw-   0        0        0    85647 2023-06-02 08:38:46.000000 pyhelpers-1.5.0rc2/pyhelpers/ops.py
+-rw-rw-rw-   0        0        0    18142 2023-05-21 18:40:53.000000 pyhelpers-1.5.0rc2/pyhelpers/settings.py
+-rw-rw-rw-   0        0        0    85554 2023-06-02 08:37:51.000000 pyhelpers-1.5.0rc2/pyhelpers/store.py
+-rw-rw-rw-   0        0        0    24373 2023-05-21 18:41:23.000000 pyhelpers-1.5.0rc2/pyhelpers/text.py
+drwxrwxrwx   0        0        0        0 2023-06-07 09:17:50.899688 pyhelpers-1.5.0rc2/pyhelpers.egg-info/
+-rw-rw-rw-   0        0        0     5136 2023-06-07 09:17:50.000000 pyhelpers-1.5.0rc2/pyhelpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-06-07 09:17:50.000000 pyhelpers-1.5.0rc2/pyhelpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 09:17:50.000000 pyhelpers-1.5.0rc2/pyhelpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2023-06-07 09:17:50.000000 pyhelpers-1.5.0rc2/pyhelpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-07 09:17:50.000000 pyhelpers-1.5.0rc2/pyhelpers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2023-05-20 14:30:39.000000 pyhelpers-1.5.0rc2/pyproject.toml
+-rw-rw-rw-   0        0        0      964 2023-06-07 09:17:50.912681 pyhelpers-1.5.0rc2/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-05-22 10:01:48.000000 pyhelpers-1.5.0rc2/setup.py
```

### Comparing `pyhelpers-1.5.0/LICENSE` & `pyhelpers-1.5.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/PKG-INFO` & `pyhelpers-1.5.0rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyhelpers
-Version: 1.5.0
+Version: 1.5.0rc2
 Summary: An open-source toolkit for facilitating Python users' data manipulation tasks.
 Home-page: https://github.com/mikeqfu/pyhelpers
 Author: Qian Fu
 Author-email: q.fu@bham.ac.uk
 License: GPLv3+
-Project-URL: Documentation, https://pyhelpers.readthedocs.io/en/1.5.0/
+Project-URL: Documentation, https://pyhelpers.readthedocs.io/en/1.5.0rc2/
 Project-URL: Source, https://github.com/mikeqfu/pyhelpers
 Project-URL: Bug Tracker, https://github.com/mikeqfu/pyhelpers/issues
 Keywords: Python,Utilities,Data preprocessing,Data manipulation
 Platform: nt
 Platform: posix
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -31,35 +31,35 @@
 
 [![Python version](https://img.shields.io/pypi/pyversions/pyhelpers)](https://docs.python.org/3/) 
 [![Documentation status](https://readthedocs.org/projects/pyhelpers/badge/?version=latest)](https://pyhelpers.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/pypi/l/pyhelpers)](https://github.com/mikeqfu/pyhelpers/blob/master/LICENSE)
 [![Codacy grade (Code quality)](https://app.codacy.com/project/badge/Grade/c3ed8571c494450da12cb0c4d3c8c7e9)](https://www.codacy.com/gh/mikeqfu/pyhelpers/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mikeqfu/pyhelpers&amp;utm_campaign=Badge_Grade)
 [![Zenodo - DOI](https://zenodo.org/badge/173177909.svg)](https://zenodo.org/badge/latestdoi/173177909)
 
-PyHelpers is a lightweight open-source Python package designed as a versatile toolkit for simplifying data (pre)processing tasks. It offers a comprehensive range of practical utilities to facilitate common data manipulation operations. These utilities encompass the ability to read and write file-like objects, efficiently handle various data types such as geographical and textual data, and establish streamlined communication with relational databases like PostgreSQL and Microsoft SQL Server.
+PyHelpers is an open-source Python package designed as a lite toolkit for facilitating data (pre)processing. It offers a miscellaneous collection of handy utilities, which could assist us in performing many common data manipulation tasks, such as reading/writing of file-like objects, handling of various types of data (e.g. geographical data and textual data) and communication with relational databases (e.g. PostgreSQL and Microsoft SQL Server).
 
 ## Installation
 
 To install the latest release of pyhelpers from [PyPI](https://pypi.org/project/pyhelpers/) via [pip](https://pip.pypa.io/en/stable/cli/pip/):
 
-```bash
+```{bash}
 pip install --upgrade pyhelpers
 ```
 
 For more information, please refer to [Installation](https://pyhelpers.readthedocs.io/en/latest/installation.html).
 
 ## Documentation
 
 The full PyHelpers documentation (including detailed examples and a quick-start tutorial) is hosted on [ReadTheDocs](https://readthedocs.org/projects/pyhelpers/): [[HTML](https://pyhelpers.readthedocs.io/en/latest/)\] \[[PDF](https://pyhelpers.readthedocs.io/_/downloads/en/latest/pdf/)].
 
 ## Cite as
 
 Fu, Q. (2020). PyHelpers: an open-source toolkit for facilitating Python users' data manipulation tasks. Zenodo. [doi:10.5281/zenodo.4017438](https://doi.org/10.5281/zenodo.4017438)
 
-```bibtex
+```{bibtex}
 @software{qian_fu_pyhelpers_4017438,
   author    = {Qian Fu},
   title     = {{PyHelpers: an open-source toolkit for facilitating
                 Python users' data manipulation tasks}},
   year      = 2020,
   publisher = {Zenodo},
   doi       = {10.5281/zenodo.4017438},
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: pyhelpers Version: 1.5.0 Summary: An open-source
+Metadata-Version: 2.1 Name: pyhelpers Version: 1.5.0rc2 Summary: An open-source
 toolkit for facilitating Python users' data manipulation tasks. Home-page:
 https://github.com/mikeqfu/pyhelpers Author: Qian Fu Author-email:
 q.fu@bham.ac.uk License: GPLv3+ Project-URL: Documentation, https://
-pyhelpers.readthedocs.io/en/1.5.0/ Project-URL: Source, https://github.com/
+pyhelpers.readthedocs.io/en/1.5.0rc2/ Project-URL: Source, https://github.com/
 mikeqfu/pyhelpers Project-URL: Bug Tracker, https://github.com/mikeqfu/
 pyhelpers/issues Keywords: Python,Utilities,Data preprocessing,Data
 manipulation Platform: nt Platform: posix Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Education Classifier: Topic
 :: Scientific/Engineering Classifier: Topic :: Software Development Classifier:
 Topic :: Utilities Classifier: License :: OSI Approved :: GNU General Public
@@ -19,37 +19,36 @@
 ?version=latest)](https://pyhelpers.readthedocs.io/en/latest/?badge=latest) [!
 [License](https://img.shields.io/pypi/l/pyhelpers)](https://github.com/mikeqfu/
 pyhelpers/blob/master/LICENSE) [![Codacy grade (Code quality)](https://
 app.codacy.com/project/badge/Grade/c3ed8571c494450da12cb0c4d3c8c7e9)](https://
 www.codacy.com/gh/mikeqfu/pyhelpers/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=mikeqfu/
 pyhelpers&utm_campaign=Badge_Grade) [![Zenodo - DOI](https://zenodo.org/badge/
-173177909.svg)](https://zenodo.org/badge/latestdoi/173177909) PyHelpers is a
-lightweight open-source Python package designed as a versatile toolkit for
-simplifying data (pre)processing tasks. It offers a comprehensive range of
-practical utilities to facilitate common data manipulation operations. These
-utilities encompass the ability to read and write file-like objects,
-efficiently handle various data types such as geographical and textual data,
-and establish streamlined communication with relational databases like
-PostgreSQL and Microsoft SQL Server. ## Installation To install the latest
-release of pyhelpers from [PyPI](https://pypi.org/project/pyhelpers/) via [pip]
-(https://pip.pypa.io/en/stable/cli/pip/): ```bash pip install --upgrade
-pyhelpers ``` For more information, please refer to [Installation](https://
-pyhelpers.readthedocs.io/en/latest/installation.html). ## Documentation The
-full PyHelpers documentation (including detailed examples and a quick-start
-tutorial) is hosted on [ReadTheDocs](https://readthedocs.org/projects/
-pyhelpers/): [[HTML](https://pyhelpers.readthedocs.io/en/latest/)\] \[[PDF]
-(https://pyhelpers.readthedocs.io/_/downloads/en/latest/pdf/)]. ## Cite as Fu,
-Q. (2020). PyHelpers: an open-source toolkit for facilitating Python users'
+173177909.svg)](https://zenodo.org/badge/latestdoi/173177909) PyHelpers is an
+open-source Python package designed as a lite toolkit for facilitating data
+(pre)processing. It offers a miscellaneous collection of handy utilities, which
+could assist us in performing many common data manipulation tasks, such as
+reading/writing of file-like objects, handling of various types of data (e.g.
+geographical data and textual data) and communication with relational databases
+(e.g. PostgreSQL and Microsoft SQL Server). ## Installation To install the
+latest release of pyhelpers from [PyPI](https://pypi.org/project/pyhelpers/
+) via [pip](https://pip.pypa.io/en/stable/cli/pip/): ```{bash} pip install --
+upgrade pyhelpers ``` For more information, please refer to [Installation]
+(https://pyhelpers.readthedocs.io/en/latest/installation.html). ##
+Documentation The full PyHelpers documentation (including detailed examples and
+a quick-start tutorial) is hosted on [ReadTheDocs](https://readthedocs.org/
+projects/pyhelpers/): [[HTML](https://pyhelpers.readthedocs.io/en/latest/)\] \[
+[PDF](https://pyhelpers.readthedocs.io/_/downloads/en/latest/pdf/)]. ## Cite as
+Fu, Q. (2020). PyHelpers: an open-source toolkit for facilitating Python users'
 data manipulation tasks. Zenodo. [doi:10.5281/zenodo.4017438](https://doi.org/
-10.5281/zenodo.4017438) ```bibtex @software{qian_fu_pyhelpers_4017438, author =
-{Qian Fu}, title = {{PyHelpers: an open-source toolkit for facilitating Python
-users' data manipulation tasks}}, year = 2020, publisher = {Zenodo}, doi =
-{10.5281/zenodo.4017438}, url = {https://doi.org/10.5281/zenodo.4017438} } ```
-(Please also refer to the export options from [Zenodo](https://zenodo.org/
+10.5281/zenodo.4017438) ```{bibtex} @software{qian_fu_pyhelpers_4017438, author
+= {Qian Fu}, title = {{PyHelpers: an open-source toolkit for facilitating
+Python users' data manipulation tasks}}, year = 2020, publisher = {Zenodo}, doi
+= {10.5281/zenodo.4017438}, url = {https://doi.org/10.5281/zenodo.4017438} }
+``` (Please also refer to the export options from [Zenodo](https://zenodo.org/
 search?page=1&size=20&q=conceptrecid:%224017438%22&sort=-
 version&all_versions=True) to reference the specific version of PyHelpers as
 appropriate.) ## Contributors
              [Qian_Fu]              [Xiangyong_Luo]
               Qian_Fu                Xiangyong_Luo
         ð± ð» ð§ª �     ð»
 ## License PyHelpers is licensed under [GNU General Public License v3](https://
```

### Comparing `pyhelpers-1.5.0/README.md` & `pyhelpers-1.5.0rc2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 
 [![Python version](https://img.shields.io/pypi/pyversions/pyhelpers)](https://docs.python.org/3/) 
 [![Documentation status](https://readthedocs.org/projects/pyhelpers/badge/?version=latest)](https://pyhelpers.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/pypi/l/pyhelpers)](https://github.com/mikeqfu/pyhelpers/blob/master/LICENSE)
 [![Codacy grade (Code quality)](https://app.codacy.com/project/badge/Grade/c3ed8571c494450da12cb0c4d3c8c7e9)](https://www.codacy.com/gh/mikeqfu/pyhelpers/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mikeqfu/pyhelpers&amp;utm_campaign=Badge_Grade)
 [![Zenodo - DOI](https://zenodo.org/badge/173177909.svg)](https://zenodo.org/badge/latestdoi/173177909)
 
-PyHelpers is a lightweight open-source Python package designed as a versatile toolkit for simplifying data (pre)processing tasks. It offers a comprehensive range of practical utilities to facilitate common data manipulation operations. These utilities encompass the ability to read and write file-like objects, efficiently handle various data types such as geographical and textual data, and establish streamlined communication with relational databases like PostgreSQL and Microsoft SQL Server.
+PyHelpers is an open-source Python package designed as a lite toolkit for facilitating data (pre)processing. It offers a miscellaneous collection of handy utilities, which could assist us in performing many common data manipulation tasks, such as reading/writing of file-like objects, handling of various types of data (e.g. geographical data and textual data) and communication with relational databases (e.g. PostgreSQL and Microsoft SQL Server).
 
 ## Installation
 
 To install the latest release of pyhelpers from [PyPI](https://pypi.org/project/pyhelpers/) via [pip](https://pip.pypa.io/en/stable/cli/pip/):
 
-```bash
+```{bash}
 pip install --upgrade pyhelpers
 ```
 
 For more information, please refer to [Installation](https://pyhelpers.readthedocs.io/en/latest/installation.html).
 
 ## Documentation
 
 The full PyHelpers documentation (including detailed examples and a quick-start tutorial) is hosted on [ReadTheDocs](https://readthedocs.org/projects/pyhelpers/): [[HTML](https://pyhelpers.readthedocs.io/en/latest/)\] \[[PDF](https://pyhelpers.readthedocs.io/_/downloads/en/latest/pdf/)].
 
 ## Cite as
 
 Fu, Q. (2020). PyHelpers: an open-source toolkit for facilitating Python users' data manipulation tasks. Zenodo. [doi:10.5281/zenodo.4017438](https://doi.org/10.5281/zenodo.4017438)
 
-```bibtex
+```{bibtex}
 @software{qian_fu_pyhelpers_4017438,
   author    = {Qian Fu},
   title     = {{PyHelpers: an open-source toolkit for facilitating
                 Python users' data manipulation tasks}},
   year      = 2020,
   publisher = {Zenodo},
   doi       = {10.5281/zenodo.4017438},
```

#### html2text {}

```diff
@@ -4,37 +4,36 @@
 pyhelpers.readthedocs.io/en/latest/?badge=latest) [![License](https://
 img.shields.io/pypi/l/pyhelpers)](https://github.com/mikeqfu/pyhelpers/blob/
 master/LICENSE) [![Codacy grade (Code quality)](https://app.codacy.com/project/
 badge/Grade/c3ed8571c494450da12cb0c4d3c8c7e9)](https://www.codacy.com/gh/
 mikeqfu/pyhelpers/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=mikeqfu/
 pyhelpers&utm_campaign=Badge_Grade) [![Zenodo - DOI](https://zenodo.org/badge/
-173177909.svg)](https://zenodo.org/badge/latestdoi/173177909) PyHelpers is a
-lightweight open-source Python package designed as a versatile toolkit for
-simplifying data (pre)processing tasks. It offers a comprehensive range of
-practical utilities to facilitate common data manipulation operations. These
-utilities encompass the ability to read and write file-like objects,
-efficiently handle various data types such as geographical and textual data,
-and establish streamlined communication with relational databases like
-PostgreSQL and Microsoft SQL Server. ## Installation To install the latest
-release of pyhelpers from [PyPI](https://pypi.org/project/pyhelpers/) via [pip]
-(https://pip.pypa.io/en/stable/cli/pip/): ```bash pip install --upgrade
-pyhelpers ``` For more information, please refer to [Installation](https://
-pyhelpers.readthedocs.io/en/latest/installation.html). ## Documentation The
-full PyHelpers documentation (including detailed examples and a quick-start
-tutorial) is hosted on [ReadTheDocs](https://readthedocs.org/projects/
-pyhelpers/): [[HTML](https://pyhelpers.readthedocs.io/en/latest/)\] \[[PDF]
-(https://pyhelpers.readthedocs.io/_/downloads/en/latest/pdf/)]. ## Cite as Fu,
-Q. (2020). PyHelpers: an open-source toolkit for facilitating Python users'
+173177909.svg)](https://zenodo.org/badge/latestdoi/173177909) PyHelpers is an
+open-source Python package designed as a lite toolkit for facilitating data
+(pre)processing. It offers a miscellaneous collection of handy utilities, which
+could assist us in performing many common data manipulation tasks, such as
+reading/writing of file-like objects, handling of various types of data (e.g.
+geographical data and textual data) and communication with relational databases
+(e.g. PostgreSQL and Microsoft SQL Server). ## Installation To install the
+latest release of pyhelpers from [PyPI](https://pypi.org/project/pyhelpers/
+) via [pip](https://pip.pypa.io/en/stable/cli/pip/): ```{bash} pip install --
+upgrade pyhelpers ``` For more information, please refer to [Installation]
+(https://pyhelpers.readthedocs.io/en/latest/installation.html). ##
+Documentation The full PyHelpers documentation (including detailed examples and
+a quick-start tutorial) is hosted on [ReadTheDocs](https://readthedocs.org/
+projects/pyhelpers/): [[HTML](https://pyhelpers.readthedocs.io/en/latest/)\] \[
+[PDF](https://pyhelpers.readthedocs.io/_/downloads/en/latest/pdf/)]. ## Cite as
+Fu, Q. (2020). PyHelpers: an open-source toolkit for facilitating Python users'
 data manipulation tasks. Zenodo. [doi:10.5281/zenodo.4017438](https://doi.org/
-10.5281/zenodo.4017438) ```bibtex @software{qian_fu_pyhelpers_4017438, author =
-{Qian Fu}, title = {{PyHelpers: an open-source toolkit for facilitating Python
-users' data manipulation tasks}}, year = 2020, publisher = {Zenodo}, doi =
-{10.5281/zenodo.4017438}, url = {https://doi.org/10.5281/zenodo.4017438} } ```
-(Please also refer to the export options from [Zenodo](https://zenodo.org/
+10.5281/zenodo.4017438) ```{bibtex} @software{qian_fu_pyhelpers_4017438, author
+= {Qian Fu}, title = {{PyHelpers: an open-source toolkit for facilitating
+Python users' data manipulation tasks}}, year = 2020, publisher = {Zenodo}, doi
+= {10.5281/zenodo.4017438}, url = {https://doi.org/10.5281/zenodo.4017438} }
+``` (Please also refer to the export options from [Zenodo](https://zenodo.org/
 search?page=1&size=20&q=conceptrecid:%224017438%22&sort=-
 version&all_versions=True) to reference the specific version of PyHelpers as
 appropriate.) ## Contributors
              [Qian_Fu]              [Xiangyong_Luo]
               Qian_Fu                Xiangyong_Luo
         ð± ð» ð§ª �     ð»
 ## License PyHelpers is licensed under [GNU General Public License v3](https://
```

### Comparing `pyhelpers-1.5.0/pyhelpers/__init__.py` & `pyhelpers-1.5.0rc2/pyhelpers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers/_cache.py` & `pyhelpers-1.5.0rc2/pyhelpers/_cache.py`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers/data/english-numerals.json` & `pyhelpers-1.5.0rc2/pyhelpers/data/english-numerals.json`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers/data/user-agent-strings.json` & `pyhelpers-1.5.0rc2/pyhelpers/data/user-agent-strings.json`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers/data/xlsx2csv.vbs` & `pyhelpers-1.5.0rc2/pyhelpers/data/xlsx2csv.vbs`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers/dbms.py` & `pyhelpers-1.5.0rc2/pyhelpers/dbms.py`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers/dirs.py` & `pyhelpers-1.5.0rc2/pyhelpers/dirs.py`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers/geom.py` & `pyhelpers-1.5.0rc2/pyhelpers/geom.py`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers/ops.py` & `pyhelpers-1.5.0rc2/pyhelpers/ops.py`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers/settings.py` & `pyhelpers-1.5.0rc2/pyhelpers/settings.py`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers/store.py` & `pyhelpers-1.5.0rc2/pyhelpers/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1923,30 +1923,27 @@
               'however, it is not found on this device.\nInstall it and then try again.')
 
 
 # ==================================================================================================
 # Convert data
 # ==================================================================================================
 
-def markdown_to_rst(path_to_md, path_to_rst, reverse=False, engine=None, pandoc_exe=None,
-                    verbose=False, **kwargs):
+def markdown_to_rst(path_to_md, path_to_rst, engine=None, pandoc_exe=None, verbose=False, **kwargs):
     """
     Convert a `Markdown <https://daringfireball.net/projects/markdown/>`_ file (.md)
     to a `reStructuredText <https://docutils.readthedocs.io/en/sphinx-docs/user/rst/quickstart.html>`_
     (.rst) file.
 
     This function relies on
     `Pandoc <https://pandoc.org/>`_ or `pypandoc <https://github.com/bebraw/pypandoc>`_.
 
     :param path_to_md: path where a markdown file is saved
     :type path_to_md: str | os.PathLike
     :param path_to_rst: path where a reStructuredText file is saved
     :type path_to_rst: str | os.PathLike
-    :param reverse: whether to convert a .rst file to a .md file, defaults to ``False``
-    :type reverse: bool
     :param engine: engine/module used for performing the conversion, defaults to ``None``;
         an alternative option is ``'pypandoc'``
     :type engine: None | str
     :param pandoc_exe: absolute path to the executable "pandoc.exe", defaults to ``None``;
         when ``pandoc_exe=None``, use the default installation path, e.g. (on Windows)
         "*C:\\\\Program Files\\\\Pandoc\\\\pandoc.exe*"
     :type pandoc_exe: str | None
@@ -1960,70 +1957,57 @@
 
     **Examples**::
 
         >>> from pyhelpers.store import markdown_to_rst
         >>> from pyhelpers.dirs import cd
 
         >>> dat_dir = cd("tests\\documents")
+
         >>> path_to_md_file = cd(dat_dir, "readme.md")
         >>> path_to_rst_file = cd(dat_dir, "readme.rst")
 
         >>> markdown_to_rst(path_to_md_file, path_to_rst_file, verbose=True)
         Converting "tests\\data\\markdown.md" to "tests\\data\\markdown.rst" ... Done.
-
-        >>> markdown_to_rst(path_to_md_file, path_to_rst_file, engine='pypandoc', verbose=True)
-        Updating "readme.rst" at "tests\\documents\\" ... Done.
     """
 
     exe_name = "pandoc.exe"
-    optional_pathnames = {exe_name, f"C:\\Program Files\\Pandoc\\{exe_name}"}
+    optional_pathnames = {exe_name, f"C:/Program Files/Pandoc/{exe_name}"}
     pandoc_exists, pandoc_exe_ = _check_file_pathname(exe_name, optional_pathnames, target=pandoc_exe)
 
-    input_path, output_path = path_to_md, path_to_rst
-    arg_f, arg_t = 'markdown+smart', 'rst+smart'
-    if reverse:
-        input_path, output_path = output_path, input_path
-        arg_f, arg_t = arg_t, arg_f
-
-    abs_input_path, abs_output_path = map(pathlib.Path, [input_path, output_path])
-    # assert abs_from_path.suffix == ".md" and abs_to_path.suffix == ".rst"
+    abs_md_path, abs_rst_path = pathlib.Path(path_to_md), pathlib.Path(path_to_rst)
+    # assert abs_md_path.suffix == ".md" and abs_rst_path.suffix == ".rst"
 
     if verbose:
-        rel_input_path, rel_output_path = map(
-            lambda x: pathlib.Path(os.path.relpath(x)), (abs_input_path, abs_output_path))
+        rel_md_path, rel_rst_path = map(
+            lambda x: pathlib.Path(os.path.relpath(x)), (abs_md_path, abs_rst_path))
 
-        if not os.path.exists(abs_output_path):
-            msg = "Converting \"{}\" to \"{}\"".format(rel_input_path, rel_output_path)
+        if not os.path.exists(abs_rst_path):
+            msg = "Converting \"{}\" to \"{}\"".format(rel_md_path, rel_rst_path)
         else:
-            msg = "Updating \"{}\" at \"{}\\\"".format(rel_output_path.name, rel_output_path.parent)
+            msg = "Updating \"{}\" at \"{}\\\"".format(rel_rst_path.name, rel_rst_path.parent)
         print(msg, end=" ... ")
 
     try:
         if engine is None:
             if pandoc_exists:
-                cmd_args = [pandoc_exe_, '--wrap=preserve', abs_input_path, '-f', arg_f, '-t', arg_t]
-                if reverse:
-                    cmd_args += ['-o', abs_output_path]
-                else:
-                    cmd_args += ['-s', '-o', abs_output_path]
-                rslt = subprocess.run(cmd_args, **kwargs)
+                # subprocess.run(
+                #     f'"{pandoc_exe_}" "{abs_md_path}" -f markdown -t rst -s -o "{abs_rst_path}"')
+                command_args = [
+                    pandoc_exe_, abs_md_path, '-f', 'markdown', '-t', 'rst', '-s', '-o', abs_rst_path]
+                rslt = subprocess.run(command_args, **kwargs)
                 ret_code = rslt.returncode
 
             else:
                 ret_code = -1
 
         else:
             py_pandoc = _check_dependency(name='pypandoc')
 
-            if 'extra_args' in kwargs:
-                kwargs['extra_args'].append(['--wrap=preserve'])
-            else:
-                kwargs.update({'extra_args': ['--wrap=preserve']})
             rslt = py_pandoc.convert_file(
-                source_file=str(abs_input_path), to=arg_t, outputfile=str(abs_output_path), **kwargs)
+                str(abs_md_path), 'rst', outputfile=str(abs_rst_path), **kwargs)
 
             ret_code = 0 if rslt == '' else -2
 
         if verbose:
             if ret_code == 0:
                 print("Done.")
             elif ret_code == -1:
```

### Comparing `pyhelpers-1.5.0/pyhelpers/text.py` & `pyhelpers-1.5.0rc2/pyhelpers/text.py`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/pyhelpers.egg-info/PKG-INFO` & `pyhelpers-1.5.0rc2/pyhelpers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pyhelpers
-Version: 1.5.0
+Version: 1.5.0rc2
 Summary: An open-source toolkit for facilitating Python users' data manipulation tasks.
 Home-page: https://github.com/mikeqfu/pyhelpers
 Author: Qian Fu
 Author-email: q.fu@bham.ac.uk
 License: GPLv3+
-Project-URL: Documentation, https://pyhelpers.readthedocs.io/en/1.5.0/
+Project-URL: Documentation, https://pyhelpers.readthedocs.io/en/1.5.0rc2/
 Project-URL: Source, https://github.com/mikeqfu/pyhelpers
 Project-URL: Bug Tracker, https://github.com/mikeqfu/pyhelpers/issues
 Keywords: Python,Utilities,Data preprocessing,Data manipulation
 Platform: nt
 Platform: posix
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -31,35 +31,35 @@
 
 [![Python version](https://img.shields.io/pypi/pyversions/pyhelpers)](https://docs.python.org/3/) 
 [![Documentation status](https://readthedocs.org/projects/pyhelpers/badge/?version=latest)](https://pyhelpers.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/pypi/l/pyhelpers)](https://github.com/mikeqfu/pyhelpers/blob/master/LICENSE)
 [![Codacy grade (Code quality)](https://app.codacy.com/project/badge/Grade/c3ed8571c494450da12cb0c4d3c8c7e9)](https://www.codacy.com/gh/mikeqfu/pyhelpers/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=mikeqfu/pyhelpers&amp;utm_campaign=Badge_Grade)
 [![Zenodo - DOI](https://zenodo.org/badge/173177909.svg)](https://zenodo.org/badge/latestdoi/173177909)
 
-PyHelpers is a lightweight open-source Python package designed as a versatile toolkit for simplifying data (pre)processing tasks. It offers a comprehensive range of practical utilities to facilitate common data manipulation operations. These utilities encompass the ability to read and write file-like objects, efficiently handle various data types such as geographical and textual data, and establish streamlined communication with relational databases like PostgreSQL and Microsoft SQL Server.
+PyHelpers is an open-source Python package designed as a lite toolkit for facilitating data (pre)processing. It offers a miscellaneous collection of handy utilities, which could assist us in performing many common data manipulation tasks, such as reading/writing of file-like objects, handling of various types of data (e.g. geographical data and textual data) and communication with relational databases (e.g. PostgreSQL and Microsoft SQL Server).
 
 ## Installation
 
 To install the latest release of pyhelpers from [PyPI](https://pypi.org/project/pyhelpers/) via [pip](https://pip.pypa.io/en/stable/cli/pip/):
 
-```bash
+```{bash}
 pip install --upgrade pyhelpers
 ```
 
 For more information, please refer to [Installation](https://pyhelpers.readthedocs.io/en/latest/installation.html).
 
 ## Documentation
 
 The full PyHelpers documentation (including detailed examples and a quick-start tutorial) is hosted on [ReadTheDocs](https://readthedocs.org/projects/pyhelpers/): [[HTML](https://pyhelpers.readthedocs.io/en/latest/)\] \[[PDF](https://pyhelpers.readthedocs.io/_/downloads/en/latest/pdf/)].
 
 ## Cite as
 
 Fu, Q. (2020). PyHelpers: an open-source toolkit for facilitating Python users' data manipulation tasks. Zenodo. [doi:10.5281/zenodo.4017438](https://doi.org/10.5281/zenodo.4017438)
 
-```bibtex
+```{bibtex}
 @software{qian_fu_pyhelpers_4017438,
   author    = {Qian Fu},
   title     = {{PyHelpers: an open-source toolkit for facilitating
                 Python users' data manipulation tasks}},
   year      = 2020,
   publisher = {Zenodo},
   doi       = {10.5281/zenodo.4017438},
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: pyhelpers Version: 1.5.0 Summary: An open-source
+Metadata-Version: 2.1 Name: pyhelpers Version: 1.5.0rc2 Summary: An open-source
 toolkit for facilitating Python users' data manipulation tasks. Home-page:
 https://github.com/mikeqfu/pyhelpers Author: Qian Fu Author-email:
 q.fu@bham.ac.uk License: GPLv3+ Project-URL: Documentation, https://
-pyhelpers.readthedocs.io/en/1.5.0/ Project-URL: Source, https://github.com/
+pyhelpers.readthedocs.io/en/1.5.0rc2/ Project-URL: Source, https://github.com/
 mikeqfu/pyhelpers Project-URL: Bug Tracker, https://github.com/mikeqfu/
 pyhelpers/issues Keywords: Python,Utilities,Data preprocessing,Data
 manipulation Platform: nt Platform: posix Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Education Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Education Classifier: Topic
 :: Scientific/Engineering Classifier: Topic :: Software Development Classifier:
 Topic :: Utilities Classifier: License :: OSI Approved :: GNU General Public
@@ -19,37 +19,36 @@
 ?version=latest)](https://pyhelpers.readthedocs.io/en/latest/?badge=latest) [!
 [License](https://img.shields.io/pypi/l/pyhelpers)](https://github.com/mikeqfu/
 pyhelpers/blob/master/LICENSE) [![Codacy grade (Code quality)](https://
 app.codacy.com/project/badge/Grade/c3ed8571c494450da12cb0c4d3c8c7e9)](https://
 www.codacy.com/gh/mikeqfu/pyhelpers/
 dashboard?utm_source=github.com&utm_medium=referral&utm_content=mikeqfu/
 pyhelpers&utm_campaign=Badge_Grade) [![Zenodo - DOI](https://zenodo.org/badge/
-173177909.svg)](https://zenodo.org/badge/latestdoi/173177909) PyHelpers is a
-lightweight open-source Python package designed as a versatile toolkit for
-simplifying data (pre)processing tasks. It offers a comprehensive range of
-practical utilities to facilitate common data manipulation operations. These
-utilities encompass the ability to read and write file-like objects,
-efficiently handle various data types such as geographical and textual data,
-and establish streamlined communication with relational databases like
-PostgreSQL and Microsoft SQL Server. ## Installation To install the latest
-release of pyhelpers from [PyPI](https://pypi.org/project/pyhelpers/) via [pip]
-(https://pip.pypa.io/en/stable/cli/pip/): ```bash pip install --upgrade
-pyhelpers ``` For more information, please refer to [Installation](https://
-pyhelpers.readthedocs.io/en/latest/installation.html). ## Documentation The
-full PyHelpers documentation (including detailed examples and a quick-start
-tutorial) is hosted on [ReadTheDocs](https://readthedocs.org/projects/
-pyhelpers/): [[HTML](https://pyhelpers.readthedocs.io/en/latest/)\] \[[PDF]
-(https://pyhelpers.readthedocs.io/_/downloads/en/latest/pdf/)]. ## Cite as Fu,
-Q. (2020). PyHelpers: an open-source toolkit for facilitating Python users'
+173177909.svg)](https://zenodo.org/badge/latestdoi/173177909) PyHelpers is an
+open-source Python package designed as a lite toolkit for facilitating data
+(pre)processing. It offers a miscellaneous collection of handy utilities, which
+could assist us in performing many common data manipulation tasks, such as
+reading/writing of file-like objects, handling of various types of data (e.g.
+geographical data and textual data) and communication with relational databases
+(e.g. PostgreSQL and Microsoft SQL Server). ## Installation To install the
+latest release of pyhelpers from [PyPI](https://pypi.org/project/pyhelpers/
+) via [pip](https://pip.pypa.io/en/stable/cli/pip/): ```{bash} pip install --
+upgrade pyhelpers ``` For more information, please refer to [Installation]
+(https://pyhelpers.readthedocs.io/en/latest/installation.html). ##
+Documentation The full PyHelpers documentation (including detailed examples and
+a quick-start tutorial) is hosted on [ReadTheDocs](https://readthedocs.org/
+projects/pyhelpers/): [[HTML](https://pyhelpers.readthedocs.io/en/latest/)\] \[
+[PDF](https://pyhelpers.readthedocs.io/_/downloads/en/latest/pdf/)]. ## Cite as
+Fu, Q. (2020). PyHelpers: an open-source toolkit for facilitating Python users'
 data manipulation tasks. Zenodo. [doi:10.5281/zenodo.4017438](https://doi.org/
-10.5281/zenodo.4017438) ```bibtex @software{qian_fu_pyhelpers_4017438, author =
-{Qian Fu}, title = {{PyHelpers: an open-source toolkit for facilitating Python
-users' data manipulation tasks}}, year = 2020, publisher = {Zenodo}, doi =
-{10.5281/zenodo.4017438}, url = {https://doi.org/10.5281/zenodo.4017438} } ```
-(Please also refer to the export options from [Zenodo](https://zenodo.org/
+10.5281/zenodo.4017438) ```{bibtex} @software{qian_fu_pyhelpers_4017438, author
+= {Qian Fu}, title = {{PyHelpers: an open-source toolkit for facilitating
+Python users' data manipulation tasks}}, year = 2020, publisher = {Zenodo}, doi
+= {10.5281/zenodo.4017438}, url = {https://doi.org/10.5281/zenodo.4017438} }
+``` (Please also refer to the export options from [Zenodo](https://zenodo.org/
 search?page=1&size=20&q=conceptrecid:%224017438%22&sort=-
 version&all_versions=True) to reference the specific version of PyHelpers as
 appropriate.) ## Contributors
              [Qian_Fu]              [Xiangyong_Luo]
               Qian_Fu                Xiangyong_Luo
         ð± ð» ð§ª �     ð»
 ## License PyHelpers is licensed under [GNU General Public License v3](https://
```

### Comparing `pyhelpers-1.5.0/pyhelpers.egg-info/SOURCES.txt` & `pyhelpers-1.5.0rc2/pyhelpers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/setup.cfg` & `pyhelpers-1.5.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyhelpers-1.5.0/setup.py` & `pyhelpers-1.5.0rc2/setup.py`

 * *Files identical despite different names*

