# Comparing `tmp/ezqc-0.3.tar.gz` & `tmp/ezqc-0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezqc-0.3.tar", last modified: Sun Jun  4 06:06:13 2023, max compression
+gzip compressed data, was "ezqc-0.35.tar", last modified: Thu Jun  8 03:05:43 2023, max compression
```

## Comparing `ezqc-0.3.tar` & `ezqc-0.35.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:06:13.304559 ezqc-0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-04 06:06:03.000000 ezqc-0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-04 06:06:13.304559 ezqc-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-04 06:06:03.000000 ezqc-0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:06:13.300559 ezqc-0.3/ezqc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/ac8.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/blast.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/color_print.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/ezqc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/os7.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/pbnc5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/pbsc3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3537 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/pbsq1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/psgc4.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/psqs2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-04 06:06:03.000000 ezqc-0.3/ezqc/sld6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:06:13.304559 ezqc-0.3/ezqc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 06:06:13.000000 ezqc-0.3/ezqc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 06:06:13.304559 ezqc-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-04 06:06:03.000000 ezqc-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 06:06:13.304559 ezqc-0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-04 06:06:03.000000 ezqc-0.3/tests/test_ezqc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:05:43.373781 ezqc-0.35/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-08 03:05:35.000000 ezqc-0.35/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-08 03:05:43.373781 ezqc-0.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-06-08 03:05:35.000000 ezqc-0.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:05:43.373781 ezqc-0.35/ezqc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/ac8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/blast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/color_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/ezqc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/os7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/pbnc5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/pbsc3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/pbsq1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/psgc4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/psqs2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-08 03:05:35.000000 ezqc-0.35/ezqc/sld6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:05:43.373781 ezqc-0.35/ezqc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-08 03:05:43.000000 ezqc-0.35/ezqc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-08 03:05:43.000000 ezqc-0.35/ezqc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:05:43.000000 ezqc-0.35/ezqc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 03:05:43.000000 ezqc-0.35/ezqc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 03:05:43.000000 ezqc-0.35/ezqc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 03:05:43.000000 ezqc-0.35/ezqc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 03:05:43.373781 ezqc-0.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-08 03:05:35.000000 ezqc-0.35/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:05:43.373781 ezqc-0.35/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-08 03:05:35.000000 ezqc-0.35/tests/test_ezqc.py
```

### Comparing `ezqc-0.3/LICENSE` & `ezqc-0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `ezqc-0.3/PKG-INFO` & `ezqc-0.35/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: ezqc
-Version: 0.3
+Version: 0.35
 Summary: EZQC is a streamlined, terminal-based alternative to FastQC.
 Author: Tinger Shi & Sky Li
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![EZQC Main Tests](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml/badge.svg)](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml)
 [![PyPI](https://img.shields.io/pypi/v/ezqc?color=blue)](https://pypi.org/project/ezqc/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 
 
 # EZQC: Easy Quality Control for FastQ Files
 <p align="center">
   <img src="tests/test1.gif" alt="test Gif" width="100%">
 </p>
 
 ## Table of Contents
 - [EZQC: Easy Quality Control for FastQ Files](#ezqc-easy-quality-control-for-fastq-files)
   - [Table of Contents](#table-of-contents)
   - [Introduction](#introduction)
+  - [Why Choose EZQC VS FastQC?](#why-choose-ezqc-vs-fastqc)
   - [Quick Start Guide](#quick-start-guide)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Analysis Methods](#analysis-methods)
   - [Contributing](#contributing)
 
 ## Introduction
@@ -37,18 +39,24 @@
 3. Per base sequence content
 4. Per sequence GC content
 5. Per base N content
 6. Sequence Length Distribution
 7. Overrepresented sequences
 8. Adapter Content
 
+## Why Choose EZQC VS FastQC?
+
+- **Fast Result Readout When Batch Processing**: With EZQC, there's no need to click into each HTML report like you would with FastQC.
+- **Automatic Interpretation of Analysis Results**: The results are color-coded and provided in plain English, complete with suggestions. This makes it easier for users to interpret the results quickly.
+- **Generate Detailed Figures for Advanced Users**: For those who want a more in-depth analysis, EZQC is capable of generating detailed figures that aid in understanding the quality of your FastQ files.
+
 ## Quick Start Guide
 
 1. Install EZQC following [Installation guide](#installation).
-2. Run the tool on a toy example using the command `ezqc tests/SRR020182.fastq` (fastq file from [IGSR](https://www.internationalgenome.org/data-portal/sample/NA18486)).
+2. Run the tool on a toy example using the command `ezqc tests/SRR020192.fastq` (fastq file from [IGSR](https://www.internationalgenome.org/data-portal/sample/NA18486)).
 3. The results will be displayed in the terminal, and figures as well as csv tables will be saved to a directory named `ezqc_output` in your current working directory. Note that this file is choosen intentionally to fail multiple QC tests.
 
 ## Installation
 
 You can install EZQC using pip:
 ```
 pip install ezqc
@@ -98,14 +106,15 @@
 
 Replace `<fastq file(s)>` with the path(s) to your FastQ files. If you want to analyze multiple files, separate the file paths with spaces:
 
 ```
 ezqc file1.fastq file2.fastq file3.fastq
 ```
 Use `-o` or `--output` to set the output directory.
+Use `-h` or `--help` to see help messages.
 
 ## Analysis Methods
 
 Here's a brief description of the analyses performed by EZQC:
 
 1. **Per Base Sequence Quality**: Checks the quality of each base call in a sequence read.
 2. **Per Sequence Quality Scores**: Provides a histogram of quality scores over all sequences.
@@ -114,8 +123,8 @@
 5. **Per Base N Content**: Identifies sequences with a high proportion of unknown (N) bases.
 6. **Sequence Length Distribution**: Provides a histogram showing the distribution of sequence lengths.
 7. **Overrepresented sequences**: Identifies any sequences that occur more often than expected.
 8. **Adapter Content**: Detects the presence of adapter sequences in the reads.
 
 ## Contributing
 
-We welcome contributions! Please see `CONTRIBUTING.md` for details on how to contribute.
+We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute.
```

### Comparing `ezqc-0.3/README.md` & `ezqc-0.35/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [![EZQC Main Tests](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml/badge.svg)](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml)
 [![PyPI](https://img.shields.io/pypi/v/ezqc?color=blue)](https://pypi.org/project/ezqc/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 
 
 # EZQC: Easy Quality Control for FastQ Files
 <p align="center">
   <img src="tests/test1.gif" alt="test Gif" width="100%">
 </p>
 
 ## Table of Contents
 - [EZQC: Easy Quality Control for FastQ Files](#ezqc-easy-quality-control-for-fastq-files)
   - [Table of Contents](#table-of-contents)
   - [Introduction](#introduction)
+  - [Why Choose EZQC VS FastQC?](#why-choose-ezqc-vs-fastqc)
   - [Quick Start Guide](#quick-start-guide)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Analysis Methods](#analysis-methods)
   - [Contributing](#contributing)
 
 ## Introduction
@@ -29,18 +31,24 @@
 3. Per base sequence content
 4. Per sequence GC content
 5. Per base N content
 6. Sequence Length Distribution
 7. Overrepresented sequences
 8. Adapter Content
 
+## Why Choose EZQC VS FastQC?
+
+- **Fast Result Readout When Batch Processing**: With EZQC, there's no need to click into each HTML report like you would with FastQC.
+- **Automatic Interpretation of Analysis Results**: The results are color-coded and provided in plain English, complete with suggestions. This makes it easier for users to interpret the results quickly.
+- **Generate Detailed Figures for Advanced Users**: For those who want a more in-depth analysis, EZQC is capable of generating detailed figures that aid in understanding the quality of your FastQ files.
+
 ## Quick Start Guide
 
 1. Install EZQC following [Installation guide](#installation).
-2. Run the tool on a toy example using the command `ezqc tests/SRR020182.fastq` (fastq file from [IGSR](https://www.internationalgenome.org/data-portal/sample/NA18486)).
+2. Run the tool on a toy example using the command `ezqc tests/SRR020192.fastq` (fastq file from [IGSR](https://www.internationalgenome.org/data-portal/sample/NA18486)).
 3. The results will be displayed in the terminal, and figures as well as csv tables will be saved to a directory named `ezqc_output` in your current working directory. Note that this file is choosen intentionally to fail multiple QC tests.
 
 ## Installation
 
 You can install EZQC using pip:
 ```
 pip install ezqc
@@ -90,14 +98,15 @@
 
 Replace `<fastq file(s)>` with the path(s) to your FastQ files. If you want to analyze multiple files, separate the file paths with spaces:
 
 ```
 ezqc file1.fastq file2.fastq file3.fastq
 ```
 Use `-o` or `--output` to set the output directory.
+Use `-h` or `--help` to see help messages.
 
 ## Analysis Methods
 
 Here's a brief description of the analyses performed by EZQC:
 
 1. **Per Base Sequence Quality**: Checks the quality of each base call in a sequence read.
 2. **Per Sequence Quality Scores**: Provides a histogram of quality scores over all sequences.
@@ -106,8 +115,8 @@
 5. **Per Base N Content**: Identifies sequences with a high proportion of unknown (N) bases.
 6. **Sequence Length Distribution**: Provides a histogram showing the distribution of sequence lengths.
 7. **Overrepresented sequences**: Identifies any sequences that occur more often than expected.
 8. **Adapter Content**: Detects the presence of adapter sequences in the reads.
 
 ## Contributing
 
-We welcome contributions! Please see `CONTRIBUTING.md` for details on how to contribute.
+We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute.
```

### Comparing `ezqc-0.3/ezqc/ac8.py` & `ezqc-0.35/ezqc/ac8.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,24 @@
     'Illumina Universal Adapter': 'AGATCGGAAGAG',
     'Illumina Small RNA 3\' Adapter': 'TGGAATTCTCGG',
     'Illumina Small RNA 5\' Adapter': 'GATCGTCGGACT',
     'SOLiD Small RNA Adapter': 'CTGCTGTACGGCCAAGGCG'
 }
 
 def calculate_adapter_content(sequences, adapters):
+    """
+    Calculate the adapter content in the provided sequences.
+
+    :param sequences: List of sequences to analyze for adapter content
+    :type sequences: list of str
+    :param adapters: Dictionary of adapters, where keys are adapter names and values are adapter sequences
+    :type adapters: dict
+    :return: A dictionary of percentages for each adapter and a boolean indicating if all sequences passed the check
+    :rtype: dict, bool
+    """
 
     counts = {name: [0]*len(sequences) for name, seq in adapters.items()}
 
     curr = 0
     for seq in sequences:
         for name, adapter in adapters.items():
             if len(seq) >= len(adapter):
@@ -33,27 +43,44 @@
             all_pass = False
     if (all_pass):
         print_color(f'O | No adaptor is present in more than 5% of all reads','green')
 
     return percentages, all_pass
 
 def plot_adapter_content(adapter_percentages,sub_directory_path):
+    """
+    Plot the adapter content percentages.
+
+    :param adapter_percentages: A dictionary of percentages for each adapter
+    :type adapter_percentages: dict
+    :param sub_directory_path: Path to the subdirectory where to save the plot image
+    :type sub_directory_path: str
+    """
     plt.figure()
     positions = list(range(1, max(map(len, adapter_percentages.values())) + 1))
 
     for name, percentages in adapter_percentages.items():
         plt.plot(positions[:len(percentages)], percentages, label=name)
 
     plt.xlabel('Position in read (bp)')
     plt.ylabel('% Adapter')
     plt.ylim(0, 100)
     plt.title('Adapter Content')
     plt.legend()
 
-    # Save and/or display the plot
     plt.savefig(f"{sub_directory_path}/adaptor_content_plot.png")
     #plt.show()
 
 def run_ac8(seqs,sub_directory_path):
+    """
+    Run the adapter content calculation and plot for the provided sequences.
+
+    :param seqs: List of sequences to analyze for adapter content
+    :type seqs: list of str
+    :param sub_directory_path: Path to the subdirectory where to save the plot image
+    :type sub_directory_path: str
+    :return: True if all sequences passed the adapter content check, False otherwise
+    :rtype: bool
+    """
     adapter_percentages, all_pass = calculate_adapter_content(seqs, adapters)
     plot_adapter_content(adapter_percentages,sub_directory_path)
     return all_pass
```

### Comparing `ezqc-0.3/ezqc/ezqc.py` & `ezqc-0.35/ezqc/ezqc.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,24 +7,40 @@
 from .pbnc5 import run_pbnc5
 from .sld6 import run_sld6
 from .os7 import run_os7
 from .ac8 import run_ac8
 import os
 
 def parse_fastq_file(file_obj):
+    """
+    This function reads a FASTQ file and yields the header, sequence and quality string line by line.
+
+    :param file_obj: A file object of a FASTQ file to be parsed.
+    :type file_obj: _io.TextIOWrapper
+    :yield: header, sequence and quality string from the FASTQ file.
+    :rtype: tuple
+    """
     while True:
         header = file_obj.readline().strip()
         if not header:
             break
         sequence = file_obj.readline().strip()
         file_obj.readline()
         quality_str = file_obj.readline().strip()
         yield header, sequence, quality_str
 
 def main():
+    """
+    This function is the main driver of the program. It accepts FASTQ files as input and generates quality analysis 
+    results as output.
+
+    It does so by taking user inputs (FASTQ files and an optional output directory) via command line arguments. It 
+    then creates necessary directories for output files. Finally, it processes each input FASTQ file using the 
+    parse_fastq_file function, performs quality analysis on the data, and writes the results to the output directory.
+    """
     logo = r'''
     ███████╗███████╗ ██████╗  ██████╗
     ██╔════╝╚══███╔╝██╔═══██╗██╔════╝
     █████╗    ███╔╝ ██║   ██║██║     
     ██╔══╝   ███╔╝  ██║▄▄ ██║██║     
     ███████╗███████╗╚██████╔╝╚██████╗
     ╚══════╝╚══════╝ ╚══▀▀═╝  ╚═════╝ made by Tinger Shi & Sky Li
@@ -37,17 +53,15 @@
     parser.add_argument('seqs', metavar='SEQ', nargs='+', help='input .fastq file(s)')
     parser.add_argument('-o', '--output', default='ezqc_output', help='output directory (default: ezqc_output)')
 
     # Parse the command-line arguments 
     args = parser.parse_args()
 
     directory_name = args.output
-    # Get the current working directory
     current_directory = os.getcwd()
-    # Create a path for the new directory
     new_directory_path = os.path.join(current_directory, directory_name)
 
     # Create the directory if it doesn't already exist
     if not os.path.exists(new_directory_path):
         os.makedirs(new_directory_path)
         print(f"Directory '{directory_name}' created successfully!")
     else:
```

### Comparing `ezqc-0.3/ezqc/os7.py` & `ezqc-0.35/ezqc/os7.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 import collections
 import csv
 from .color_print import print_color
 
 def run_os7(dna_sequences,sub_directory_path):
+    """
+    Perform analysis on overrepresented sequences in the provided DNA sequences. Sequences with representation over
+    1% and 0.1% are specifically identified. Also, writes these overrepresented sequences to a CSV file.
+
+    :param dna_sequences: List of DNA sequences to analyze
+    :type dna_sequences: list of str
+    :param sub_directory_path: Path to the subdirectory where to save the CSV file with overrepresented sequences
+    :type sub_directory_path: str
+    :return: True if the sequences pass the overrepresentation check, False otherwise
+    :rtype: bool
+    """
     # Track only the first 100,000 sequences
     dna_sequences = dna_sequences[:100000] if len(dna_sequences)>100000 else dna_sequences
 
     # Truncate sequences over 75bp to 50bp for analysis
     dna_sequences = [seq[:50] if len(seq) > 75 else seq for seq in dna_sequences]
 
     total_count = len(dna_sequences)
```

### Comparing `ezqc-0.3/ezqc/pbsc3.py` & `ezqc-0.35/ezqc/pbsc3.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 import matplotlib.pyplot as plt
 from .color_print import print_color
 
 
 def per_base_sequence_content(seqs):
+    """
+    This function calculates the percentage content of each base at each position in the sequences.
+
+    :param seqs: A list of sequences
+    :type seqs: list
+    :return: A tuple containing a dictionary of base contents, count of positions with greater than 10% differences, 
+             and count of positions with greater than 20% differences
+    :rtype: tuple
+    """
     greater_20 = 0
     greater_10 = 0
 
-    # Initialize a dictionary to hold our counts
     base_content = {'A': [], 'T': [], 'C': [], 'G': []}
 
-    # Determine the length of the longest sequence
     max_length = max(len(seq) for seq in seqs)
 
     # Loop over each position up to the maximum length
     for i in range(max_length):
-        # Initialize a dictionary to hold the counts for this position
         pos_counts = {'A': 0, 'T': 0, 'C': 0, 'G': 0, 'N': 0}
         
         # Loop over each sequence and count the bases at this position
         for seq in seqs:
             if i < len(seq):
                 pos_counts[seq[i]] += 1
         
@@ -33,34 +39,50 @@
             greater_10 += 1
 
     return base_content, greater_10, greater_20
 
 
 
 def plot_base_content(base_content,sub_directory_path):
+    """
+    This function plots the base content for each base at each position in the read and saves the plot to a file.
+
+    :param base_content: A dictionary where the keys are the bases and the values are lists of percentages for each position
+    :type base_content: dict
+    :param sub_directory_path: The directory path where the plot will be saved
+    :type sub_directory_path: str
+    """
     # Create the x-values for our plot (the position in the read)
     x_values = list(range(1, len(base_content['A'])+1))
 
     plt.figure()
 
     # Plot the base content for each base 
     for base, y_values in base_content.items():
         plt.plot(x_values, y_values, label=base)
 
-    # Add labels and a legend
     plt.xlabel('Position in read (bp)')
     plt.ylabel('Base content (%)')
     plt.ylim(0, 100)
     plt.legend()
 
-    # Save and/or display the plot
     plt.savefig(f"{sub_directory_path}/per_base_sequence_content_plot.png")
     #plt.show()
 
 def run_pbsc3(seqs,sub_directory_path):
+    """
+    This function runs the per base sequence content analysis on a set of sequences, plots the results, and checks for significant differences.
+
+    :param seqs: A list of sequences
+    :type seqs: list
+    :param sub_directory_path: The directory path where the plot will be saved
+    :type sub_directory_path: str
+    :return: True if the analysis passes, False otherwise
+    :rtype: bool
+    """
     content, greater_10, greater_20 = per_base_sequence_content(seqs)
     plot_base_content(content,sub_directory_path)
     if (greater_20>0):
         print_color(f"X | Per base sequence content NOT pass. {greater_20} positions with greater than 20% differences", "red")
         return False
     elif (greater_10):  
         print_color(f"- | Per base sequence content warning. {greater_10} positions with greater than 10% differences", "yellow")
```

### Comparing `ezqc-0.3/ezqc/psgc4.py` & `ezqc-0.35/ezqc/psgc4.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 import matplotlib.pyplot as plt
 import numpy as np
 from scipy.stats import norm
 from .color_print import print_color
 # need to pip install scipy
 
 def detect_warnings_failures(gc_contents,sequences):
+    """
+    This function detects warnings or failures based on GC content of sequences. A warning or failure is issued if the sum of 
+    deviations from the mean GC content exceeds 15% or 30% of the total sequences respectively.
+
+    :param gc_contents: A list of GC contents for each sequence
+    :type gc_contents: list
+    :param sequences: A list of sequences
+    :type sequences: list
+    :return: False if a warning or failure is detected, True otherwise
+    :rtype: bool
+    """
     mu, std = norm.fit(gc_contents)
     deviations = [abs(content - mu) for content in gc_contents]
 
     sum_deviation = sum(deviations)
 
     warning_threshold = 0.15 * len(sequences)
     failure_threshold = 0.30 * len(sequences)
@@ -20,22 +31,32 @@
         print_color("X | The sum of the deviations from the normal distribution represents more than 30% of the reads.","red")
         return False
     else:
         print_color("O | The sum of the deviations from the normal distribution are good","green")
         return True
 
 def run_psgc4(sequences,sub_directory_path):
+    """
+    This function calculates the GC content for each sequence, plots a histogram of GC contents and the theoretical 
+    normal distribution, then checks for warnings or failures.
+
+    :param sequences: A list of sequences
+    :type sequences: list
+    :param sub_directory_path: The directory path where the plot will be saved
+    :type sub_directory_path: str
+    :return: True if the analysis passes, False otherwise
+    :rtype: bool
+    """
     gc_contents = []
     # Iterate through each sequence
     for seq in sequences:
         # Compute the GC content for the current sequence
         count_gc = sum(base in "GC" for base in seq)
         gc_percent = 100 * count_gc / len(seq)
 
-        # Append the GC content to the list
         gc_contents.append(gc_percent)
         
     # plot GC distribution over all sequences
     plt.figure(figsize=(10,6))
     plt.hist(gc_contents, bins=100, alpha=0.5, label='Observed GC')
 
     # calculate and plot theoretical distribution
@@ -44,12 +65,11 @@
     plt.plot(s, norm.pdf(s, mu, sigma)*len(gc_contents)*(max(gc_contents)-min(gc_contents))/100, label='Theoretical GC')
 
     plt.title("GC distribution over all sequences")
     plt.xlabel("Mean GC content")
     plt.ylabel("Number of sequences")
     plt.legend(loc='upper right')
     plt.grid(True)
-    # Save and/or display the all the plots
     plt.savefig(f"{sub_directory_path}/per_sequence_GC_content.png")
     # plt.show()
 
     return detect_warnings_failures(gc_contents,sequences)
```

### Comparing `ezqc-0.3/ezqc/psqs2.py` & `ezqc-0.35/ezqc/psqs2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,65 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from .color_print import print_color
 
 def phred33_to_q(qual_string):
+    """
+    This function converts a Phred+33 ASCII-encoded quality string to a list of quality scores.
+
+    :param qual_string: The Phred+33 encoded quality string
+    :type qual_string: str
+    :return: The quality scores
+    :rtype: list
+    """
     return [ord(ch) - 33 for ch in qual_string]
 
 def mean_qual_score(qual_string):
+    """
+    This function calculates the mean quality score from a Phred+33 encoded quality string.
+
+    :param qual_string: The Phred+33 encoded quality string
+    :type qual_string: str
+    :return: The mean quality score
+    :rtype: float
+    """
     qual_scores = phred33_to_q(qual_string)
     return np.mean(qual_scores)
 
 def run_psqs2(quality_strings,sub_directory_path):
-# Calculate mean quality scores for each sequence
+    """
+    This function calculates the mean quality scores from a list of quality strings, and then plots the distribution of 
+    these mean scores. The plot is saved to a specified path. It also checks whether the proportion of sequences with 
+    low quality is greater than 5%.
+
+    :param quality_strings: A list of Phred+33 encoded quality strings
+    :type quality_strings: list
+    :param sub_directory_path: The path where the plot will be saved
+    :type sub_directory_path: str
+    :return: True if the proportion of sequences with low quality is less than 5%, False otherwise
+    :rtype: bool
+    """
     mean_qual_scores = [mean_qual_score(qual_string) for qual_string in quality_strings]
 
     # Set up bins for the x-axis (mean sequence quality)
     bin_edges = np.arange(0, np.ceil(max(mean_qual_scores)) + 1, 1)
 
-    # Calculate the frequency (counts) for each bin
     counts, _ = np.histogram(mean_qual_scores, bins=bin_edges)
 
     proportion_low_quality = sum(mqs < 20 for mqs in mean_qual_scores) / len(mean_qual_scores)
 
-
     # Create the plot
     plt.figure(figsize=(10, 6))
     plt.bar(bin_edges[:-1], counts, width=1, edgecolor="k", alpha=0.7)
     plt.xlabel("Mean Sequence Quality(Phred scores)")
     plt.ylabel("Number of Sequences")
     plt.title("Quality Scores distribution over all sequences")
     plt.xticks(bin_edges)
     plt.grid(True, linestyle='--', alpha=0.5)
 
-    # Save and/or display the plot
     plt.savefig(f"{sub_directory_path}/per_sequence_quality_scores.png")
     # plt.show()
 
 
     # print(proportion_low_quality)
     if (proportion_low_quality >= 0.05):
         print_color(f"X | Per sequence quality score NOT pass. Because proportion of low quality is {100*proportion_low_quality:.2f} %, which is more than 5%","red")
```

### Comparing `ezqc-0.3/ezqc/sld6.py` & `ezqc-0.35/ezqc/sld6.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,45 @@
 import matplotlib.pyplot as plt
 from .color_print import print_color
 from collections import Counter
 
 def detect_warnings_failures(sequences):
+    """
+    Detect warnings and failures based on the lengths of the sequences.
+
+    :param sequences: list of sequences
+    :type sequences: list of str
+    :return: True if no warnings or failures detected, False otherwise
+    :rtype: bool
+    """
     sequence_lengths = [len(seq) for seq in sequences]
     # Detect warning and failure situations
     if 0 in sequence_lengths:
         print_color("X | Some sequences have zero length.","red")
         return False
     if len(set(sequence_lengths)) > 1:
         print_color("- | Not all sequences are of the same length.","yellow")
         return False
     else:
         print_color("O | Lengths of Sequences are good","green")
         return True
 
 # version 2
 def run_sld6(sequences,sub_directory_path):
+    """
+    Execute the sequence analysis for sequence length distribution. This includes plotting the distribution and 
+    checking for warnings/failures.
+
+    :param sequences: list of sequences
+    :type sequences: list of str
+    :param sub_directory_path: The directory path where the plot will be saved
+    :type sub_directory_path: str
+    :return: True if the analysis passes, False otherwise
+    :rtype: bool
+    """
     sequence_lengths = [len(seq) for seq in sequences]
     length_freq = Counter(sequence_lengths)
     
     # separate keys and values for plotting, but sort them by sequence length
     if len(length_freq) == 1:
         unique_length = list(length_freq.keys())[0]
```

### Comparing `ezqc-0.3/ezqc.egg-info/PKG-INFO` & `ezqc-0.35/ezqc.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: ezqc
-Version: 0.3
+Version: 0.35
 Summary: EZQC is a streamlined, terminal-based alternative to FastQC.
 Author: Tinger Shi & Sky Li
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![EZQC Main Tests](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml/badge.svg)](https://github.com/skysky2333/EZQC/actions/workflows/ezqc_main_test.yml)
 [![PyPI](https://img.shields.io/pypi/v/ezqc?color=blue)](https://pypi.org/project/ezqc/)
+[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 
 
 
 # EZQC: Easy Quality Control for FastQ Files
 <p align="center">
   <img src="tests/test1.gif" alt="test Gif" width="100%">
 </p>
 
 ## Table of Contents
 - [EZQC: Easy Quality Control for FastQ Files](#ezqc-easy-quality-control-for-fastq-files)
   - [Table of Contents](#table-of-contents)
   - [Introduction](#introduction)
+  - [Why Choose EZQC VS FastQC?](#why-choose-ezqc-vs-fastqc)
   - [Quick Start Guide](#quick-start-guide)
   - [Installation](#installation)
   - [Usage](#usage)
   - [Analysis Methods](#analysis-methods)
   - [Contributing](#contributing)
 
 ## Introduction
@@ -37,18 +39,24 @@
 3. Per base sequence content
 4. Per sequence GC content
 5. Per base N content
 6. Sequence Length Distribution
 7. Overrepresented sequences
 8. Adapter Content
 
+## Why Choose EZQC VS FastQC?
+
+- **Fast Result Readout When Batch Processing**: With EZQC, there's no need to click into each HTML report like you would with FastQC.
+- **Automatic Interpretation of Analysis Results**: The results are color-coded and provided in plain English, complete with suggestions. This makes it easier for users to interpret the results quickly.
+- **Generate Detailed Figures for Advanced Users**: For those who want a more in-depth analysis, EZQC is capable of generating detailed figures that aid in understanding the quality of your FastQ files.
+
 ## Quick Start Guide
 
 1. Install EZQC following [Installation guide](#installation).
-2. Run the tool on a toy example using the command `ezqc tests/SRR020182.fastq` (fastq file from [IGSR](https://www.internationalgenome.org/data-portal/sample/NA18486)).
+2. Run the tool on a toy example using the command `ezqc tests/SRR020192.fastq` (fastq file from [IGSR](https://www.internationalgenome.org/data-portal/sample/NA18486)).
 3. The results will be displayed in the terminal, and figures as well as csv tables will be saved to a directory named `ezqc_output` in your current working directory. Note that this file is choosen intentionally to fail multiple QC tests.
 
 ## Installation
 
 You can install EZQC using pip:
 ```
 pip install ezqc
@@ -98,14 +106,15 @@
 
 Replace `<fastq file(s)>` with the path(s) to your FastQ files. If you want to analyze multiple files, separate the file paths with spaces:
 
 ```
 ezqc file1.fastq file2.fastq file3.fastq
 ```
 Use `-o` or `--output` to set the output directory.
+Use `-h` or `--help` to see help messages.
 
 ## Analysis Methods
 
 Here's a brief description of the analyses performed by EZQC:
 
 1. **Per Base Sequence Quality**: Checks the quality of each base call in a sequence read.
 2. **Per Sequence Quality Scores**: Provides a histogram of quality scores over all sequences.
@@ -114,8 +123,8 @@
 5. **Per Base N Content**: Identifies sequences with a high proportion of unknown (N) bases.
 6. **Sequence Length Distribution**: Provides a histogram showing the distribution of sequence lengths.
 7. **Overrepresented sequences**: Identifies any sequences that occur more often than expected.
 8. **Adapter Content**: Detects the presence of adapter sequences in the reads.
 
 ## Contributing
 
-We welcome contributions! Please see `CONTRIBUTING.md` for details on how to contribute.
+We welcome contributions! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute.
```

### Comparing `ezqc-0.3/setup.py` & `ezqc-0.35/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='ezqc',
-    version='0.3',
+    version='0.35',
     author='Tinger Shi & Sky Li',
     description='EZQC is a streamlined, terminal-based alternative to FastQC.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # Add your project dependencies here
         'numpy',
```

### Comparing `ezqc-0.3/tests/test_ezqc.py` & `ezqc-0.35/tests/test_ezqc.py`

 * *Files identical despite different names*

