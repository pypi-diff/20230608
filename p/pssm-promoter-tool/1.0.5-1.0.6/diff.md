# Comparing `tmp/pssm-promoter-tool-1.0.5.tar.gz` & `tmp/pssm-promoter-tool-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssm-promoter-tool-1.0.5.tar", last modified: Mon May 29 01:39:10 2023, max compression
+gzip compressed data, was "pssm-promoter-tool-1.0.6.tar", last modified: Thu Jun  8 03:29:50 2023, max compression
```

## Comparing `pssm-promoter-tool-1.0.5.tar` & `pssm-promoter-tool-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-29 01:39:10.371258 pssm-promoter-tool-1.0.5/
--rw-r--r--   0 ellinium   (501) staff       (20)     1513 2023-04-26 02:33:30.000000 pssm-promoter-tool-1.0.5/LICENSE.txt
--rw-r--r--   0 ellinium   (501) staff       (20)       13 2023-04-26 03:55:14.000000 pssm-promoter-tool-1.0.5/MANIFEST.in
--rw-r--r--   0 ellinium   (501) staff       (20)     5268 2023-05-29 01:39:10.371084 pssm-promoter-tool-1.0.5/PKG-INFO
--rw-r--r--   0 ellinium   (501) staff       (20)     4811 2023-05-29 01:37:50.000000 pssm-promoter-tool-1.0.5/README.md
--rw-r--r--   0 ellinium   (501) staff       (20)     2872 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.5/free_energy_coeffs.npy
--rw-r--r--   0 ellinium   (501) staff       (20)      136 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.5/model_intercept.npy
--rw-r--r--   0 ellinium   (501) staff       (20)    14908 2023-05-29 01:13:36.000000 pssm-promoter-tool-1.0.5/pssm_promoter_calculator.py
-drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-29 01:39:10.370842 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/
--rw-r--r--   0 ellinium   (501) staff       (20)     5268 2023-05-29 01:39:10.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/PKG-INFO
--rw-r--r--   0 ellinium   (501) staff       (20)      378 2023-05-29 01:39:10.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/SOURCES.txt
--rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-05-29 01:39:10.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/dependency_links.txt
--rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/not-zip-safe
--rw-r--r--   0 ellinium   (501) staff       (20)      242 2023-05-29 01:39:10.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/requires.txt
--rw-r--r--   0 ellinium   (501) staff       (20)       25 2023-05-29 01:39:10.000000 pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/top_level.txt
--rw-r--r--   0 ellinium   (501) staff       (20)      103 2023-04-26 02:26:58.000000 pssm-promoter-tool-1.0.5/pyproject.toml
--rw-r--r--   0 ellinium   (501) staff       (20)       38 2023-05-29 01:39:10.371310 pssm-promoter-tool-1.0.5/setup.cfg
--rw-r--r--   0 ellinium   (501) staff       (20)     1246 2023-05-29 01:38:59.000000 pssm-promoter-tool-1.0.5/setup.py
+drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-06-08 03:29:50.213436 pssm-promoter-tool-1.0.6/
+-rw-r--r--   0 ellinium   (501) staff       (20)     1513 2023-04-26 02:33:30.000000 pssm-promoter-tool-1.0.6/LICENSE.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)       13 2023-04-26 03:55:14.000000 pssm-promoter-tool-1.0.6/MANIFEST.in
+-rw-r--r--   0 ellinium   (501) staff       (20)     6190 2023-06-08 03:29:50.213264 pssm-promoter-tool-1.0.6/PKG-INFO
+-rw-r--r--   0 ellinium   (501) staff       (20)     5733 2023-06-08 03:27:40.000000 pssm-promoter-tool-1.0.6/README.md
+-rw-r--r--   0 ellinium   (501) staff       (20)     2872 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.6/free_energy_coeffs.npy
+-rw-r--r--   0 ellinium   (501) staff       (20)      136 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.6/model_intercept.npy
+-rw-r--r--   0 ellinium   (501) staff       (20)    15049 2023-06-08 01:34:14.000000 pssm-promoter-tool-1.0.6/pssm_promoter_calculator.py
+drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-06-08 03:29:50.213025 pssm-promoter-tool-1.0.6/pssm_promoter_tool.egg-info/
+-rw-r--r--   0 ellinium   (501) staff       (20)     6190 2023-06-08 03:29:50.000000 pssm-promoter-tool-1.0.6/pssm_promoter_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ellinium   (501) staff       (20)      378 2023-06-08 03:29:50.000000 pssm-promoter-tool-1.0.6/pssm_promoter_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-06-08 03:29:50.000000 pssm-promoter-tool-1.0.6/pssm_promoter_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.6/pssm_promoter_tool.egg-info/not-zip-safe
+-rw-r--r--   0 ellinium   (501) staff       (20)      242 2023-06-08 03:29:50.000000 pssm-promoter-tool-1.0.6/pssm_promoter_tool.egg-info/requires.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)       25 2023-06-08 03:29:50.000000 pssm-promoter-tool-1.0.6/pssm_promoter_tool.egg-info/top_level.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)      103 2023-04-26 02:26:58.000000 pssm-promoter-tool-1.0.6/pyproject.toml
+-rw-r--r--   0 ellinium   (501) staff       (20)       38 2023-06-08 03:29:50.213491 pssm-promoter-tool-1.0.6/setup.cfg
+-rw-r--r--   0 ellinium   (501) staff       (20)     1246 2023-06-08 03:28:54.000000 pssm-promoter-tool-1.0.6/setup.py
```

### Comparing `pssm-promoter-tool-1.0.5/LICENSE.txt` & `pssm-promoter-tool-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.5/PKG-INFO` & `pssm-promoter-tool-1.0.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,14 @@
-Metadata-Version: 2.1
-Name: pssm-promoter-tool
-Version: 1.0.5
-Summary: The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence
-Home-page: https://github.com/ellinium/PSSM_PromoterTool
-Author: Ellina Trofimova
-Author-email: ellina.trofimova@gmail.com
-License: GNU General Public License
-Keywords: promoter prediction transcription rate
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 **PSSM Promoter Tool**
 
 The tool applies CORPSE (Codon Restrained Promoter Silencing) method and inverted CORPSE (iCORPSE) to the provided gene sequence.
 
--35 and -10 promoters along with the additional non-canonical sequence motifs are predicted based on the Salis Lab Promoter Calculator (https://github.com/hsalis/SalisLabCode/tree/master/Promoter_Calculator).
+-35 and -10 promoters, along with the additional non-canonical sequence motifs, are predicted based on the Salis Lab Promoter Calculator (https://github.com/hsalis/SalisLabCode/tree/master/Promoter_Calculator).
 Position-specific scoring matrix (PSSM) is applied to all the synonymous codon variants of the promoters associated with the lowest and highest transcription rates in order to maximally decrease (CORPSE) or increase the transcription rate (iCORPSE).
-The output CSV file/files contain synonymous codon promoters and sequence motifs for the minimal and maximal transcriptional rates along with the non-canonical sequence motifs for forward and reverse strands.
+The output CSV file/files contain synonymous codon promoters and sequence motifs for the minimal and maximal transcriptional rates, along with the non-canonical sequence motifs for forward and reverse strands.
 
 For a web (Google Colab) version, please navigate to https://colab.research.google.com/drive/171iBNCrA1hMS-LpX_qaFani34HiueTZO?usp=sharing.
 
 INSTALLATION:
 
 1. Install required libraries using pip:
 ```
@@ -28,61 +16,71 @@
 ```
 
 2. Download and unpack the archive with files using "Code"->"Download ZIP" buttons in the right corner at https://github.com/ellinium/pssm_promoter_tool. 
 Or use
 ```
 git clone https://github.com/ellinium/pssm-promoter-tool
 ```
-[! you need to have a Git account and be authorised in the system to run the command !]
+[! it's necessary to have a Git account and be authorised in the system to run the command !]
 
 
 USAGE:
 
 The tool requires a text or fasta file with a nucleotide sequence of a gene to process.
-From the folder with the downloaded files run:
+From the folder with the downloaded files, run:
 ```
 python pssm_promoter_calculator.py <file_name>
 ```
 where 'file_name' is a path to the file with a gene sequence (TXT or FASTA format).
 
+By default, the command processes 40 PSSM promoter combinations with the highest PSSM scores for transcription rate maximisation or 40 combinations with the lowest PSSM scores for transcription rate minimisation.
+To run all the promoter combinations, use an additional argument 'all':
+```
+python pssm_promoter_calculator.py <file_name> all
+```
+
+
 Depending on the result, up to four output CSV files can be generated:
 1) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
 2) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
 3) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
 4) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
 1) Type - 'Original Promoter' - for original sequence promoters; 'Modified Promoter' - for synonymous promoters. 
-2) TSS -  transcriptional start site 
-3) Tx_rate - transcription initiation rate 
-4) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers 
-5) hex35 -  an upstream 6-nucleotide site called the −35 motif 
-6) PSSM_hex35 - position-specific scoring matrix value for the -35 motif 
-7) AA_hex35 - an amino acid sequence for the -35 motif 
-8) hex10 - a downstream 6-nucleotide site called the −10 motif 
-9) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
-10) AA_hex10 - an amino acid sequence for the -10 motif 
-11) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
-12) spacer - a spacer region that separates the −10 and −35 motifs 
-13) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
-14) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
-15) new_gene_sequence - contains a gene sequence (nt) with substituted (Type = 'Modified Promoter') or  original promoters (Type = 'Original Promoter')
-16) promoter_sequence - contains -35 motif, spacer and - 10 motif 
-17) dG_total - total Gibbs free energy for the sequence 
-18) dG_10 - -10 motif Gibbs free energy 
-19) dG_35 - -35 motif Gibbs free energy 
-20) dG_disc - a discriminator Gibbs free energy 
-21) dG_ITR - an ITR Gibbs free energy 
-22) dG_ext10 −10 extended motif Gibbs free energy 
-23) dG_spacer - a spacer Gibbs free energy 
-24) dG_UP - an UP Gibbs free energy 
-25) dG_bind - binding Gibbs free energy 
-26) UP_position - a position of the UP element 
-27) hex35_position - a position of the -35 motif 
-28) spacer_position - a position of the spacer 
-29) hex10_position - a position of the -10 motif 
-30) disc_position - a position of the discriminator
+2) TSS -  transcriptional start Site position (nt) 
+3) Tx_rate - transcription unitiation rate (au)
+4) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
+5) frame - a reading frame for the promoters 
+6) hex35 - -35 hexamer sequence (an upstream 6-nucleotide site called the −35 motif)
+7) PSSM_hex35 - position-specific scoring matrix value for the -35 motif 
+8) hex35_sequence - contains 9nt sequence that includes -hex35 promoter if it's in the 2nd or 3rd frame
+9) hex35_aa - an amino acid sequence for the -35 motif 
+10) hex10 - -10 hexamer sequence (a downstream 6-nucleotide site called the −10 motif)
+11) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
+12) hex10_sequence - contains 9nt sequence that includes -hex35 promoter if it's in the 2nd or 3rd frame
+13) hex10_aa - an amino acid sequence for the -10 motif 
+14) UP - an upstream sequence (UP). A 20-nucleotide region that appears upstream of the −35 motif.
+15) spacer - a spacer sequence that separates the −10 and −35 motifs 
+16) disc - discriminator sequence. A typically 6-nucleotide region in between the −10 motif and TSS. 
+17) ITR - the first 20 transcribed nucleotides called the initial transcribed region (ITR)
+18) new_gene_sequence - contains a gene sequence (nt) with substituted (Type = 'Modified Promoter') or  original promoters (Type = 'Original Promoter')
+19) promoter_sequence - contains -35 motif, spacer and - 10 motif 
+20) dG_total - total Gibbs free energy change (kcal/mol)
+21) dG_10 - Gibbs binding free Energy for -10 hexamer (kcal/mol)
+22) dG_35 - Gibbs binding free Energy for -35 hexamer (kcal/mol)
+23) dG_disc - Gibbs free energy penalty for non-optimal discriminator element (kcal/mol)
+24) dG_ITR - Gibbs free energy change for R-loop formation at the initial transcribed region (kcal/mol)
+25) dG_ext10 - Gibbs binding free energy for the extended -10 hexamer (kcal/mol)
+26) dG_spacer - Gibbs free energy penalty for non-optimal spacing (kcal/mol)
+27) dG_UP - Gibbs binding free energy for the upstream element (kcal/mol)
+28) dG_bind - binding Gibbs free energy 
+29) UP_position - a position of the UP element 
+30) hex35_position - a position of the -35 motif 
+31) spacer_position - a position of the spacer 
+32) hex10_position - a position of the -10 motif 
+33) disc_position - a position of the discriminator
 
 References:
 
 1. Logel DY, Trofimova E, Jaschke PR. Codon-Restrained Method for Both Eliminating and Creating Intragenic Bacterial Promoters. ACS Synth Biol. 2022 Jan 19;acssynbio.1c00359. Available from https://pubs.acs.org/doi/10.1021/acssynbio.1c00359. doi: 10.1021/acssynbio.1c00359
-2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
+2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
```

### Comparing `pssm-promoter-tool-1.0.5/README.md` & `pssm-promoter-tool-1.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,26 @@
+Metadata-Version: 2.1
+Name: pssm-promoter-tool
+Version: 1.0.6
+Summary: The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence
+Home-page: https://github.com/ellinium/PSSM_PromoterTool
+Author: Ellina Trofimova
+Author-email: ellina.trofimova@gmail.com
+License: GNU General Public License
+Keywords: promoter prediction transcription rate
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 **PSSM Promoter Tool**
 
 The tool applies CORPSE (Codon Restrained Promoter Silencing) method and inverted CORPSE (iCORPSE) to the provided gene sequence.
 
--35 and -10 promoters along with the additional non-canonical sequence motifs are predicted based on the Salis Lab Promoter Calculator (https://github.com/hsalis/SalisLabCode/tree/master/Promoter_Calculator).
+-35 and -10 promoters, along with the additional non-canonical sequence motifs, are predicted based on the Salis Lab Promoter Calculator (https://github.com/hsalis/SalisLabCode/tree/master/Promoter_Calculator).
 Position-specific scoring matrix (PSSM) is applied to all the synonymous codon variants of the promoters associated with the lowest and highest transcription rates in order to maximally decrease (CORPSE) or increase the transcription rate (iCORPSE).
-The output CSV file/files contain synonymous codon promoters and sequence motifs for the minimal and maximal transcriptional rates along with the non-canonical sequence motifs for forward and reverse strands.
+The output CSV file/files contain synonymous codon promoters and sequence motifs for the minimal and maximal transcriptional rates, along with the non-canonical sequence motifs for forward and reverse strands.
 
 For a web (Google Colab) version, please navigate to https://colab.research.google.com/drive/171iBNCrA1hMS-LpX_qaFani34HiueTZO?usp=sharing.
 
 INSTALLATION:
 
 1. Install required libraries using pip:
 ```
@@ -16,61 +28,71 @@
 ```
 
 2. Download and unpack the archive with files using "Code"->"Download ZIP" buttons in the right corner at https://github.com/ellinium/pssm_promoter_tool. 
 Or use
 ```
 git clone https://github.com/ellinium/pssm-promoter-tool
 ```
-[! you need to have a Git account and be authorised in the system to run the command !]
+[! it's necessary to have a Git account and be authorised in the system to run the command !]
 
 
 USAGE:
 
 The tool requires a text or fasta file with a nucleotide sequence of a gene to process.
-From the folder with the downloaded files run:
+From the folder with the downloaded files, run:
 ```
 python pssm_promoter_calculator.py <file_name>
 ```
 where 'file_name' is a path to the file with a gene sequence (TXT or FASTA format).
 
+By default, the command processes 40 PSSM promoter combinations with the highest PSSM scores for transcription rate maximisation or 40 combinations with the lowest PSSM scores for transcription rate minimisation.
+To run all the promoter combinations, use an additional argument 'all':
+```
+python pssm_promoter_calculator.py <file_name> all
+```
+
+
 Depending on the result, up to four output CSV files can be generated:
 1) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
 2) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
 3) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
 4) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
 1) Type - 'Original Promoter' - for original sequence promoters; 'Modified Promoter' - for synonymous promoters. 
-2) TSS -  transcriptional start site 
-3) Tx_rate - transcription initiation rate 
-4) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers 
-5) hex35 -  an upstream 6-nucleotide site called the −35 motif 
-6) PSSM_hex35 - position-specific scoring matrix value for the -35 motif 
-7) AA_hex35 - an amino acid sequence for the -35 motif 
-8) hex10 - a downstream 6-nucleotide site called the −10 motif 
-9) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
-10) AA_hex10 - an amino acid sequence for the -10 motif 
-11) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
-12) spacer - a spacer region that separates the −10 and −35 motifs 
-13) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
-14) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
-15) new_gene_sequence - contains a gene sequence (nt) with substituted (Type = 'Modified Promoter') or  original promoters (Type = 'Original Promoter')
-16) promoter_sequence - contains -35 motif, spacer and - 10 motif 
-17) dG_total - total Gibbs free energy for the sequence 
-18) dG_10 - -10 motif Gibbs free energy 
-19) dG_35 - -35 motif Gibbs free energy 
-20) dG_disc - a discriminator Gibbs free energy 
-21) dG_ITR - an ITR Gibbs free energy 
-22) dG_ext10 −10 extended motif Gibbs free energy 
-23) dG_spacer - a spacer Gibbs free energy 
-24) dG_UP - an UP Gibbs free energy 
-25) dG_bind - binding Gibbs free energy 
-26) UP_position - a position of the UP element 
-27) hex35_position - a position of the -35 motif 
-28) spacer_position - a position of the spacer 
-29) hex10_position - a position of the -10 motif 
-30) disc_position - a position of the discriminator
+2) TSS -  transcriptional start Site position (nt) 
+3) Tx_rate - transcription unitiation rate (au)
+4) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
+5) frame - a reading frame for the promoters 
+6) hex35 - -35 hexamer sequence (an upstream 6-nucleotide site called the −35 motif)
+7) PSSM_hex35 - position-specific scoring matrix value for the -35 motif 
+8) hex35_sequence - contains 9nt sequence that includes -hex35 promoter if it's in the 2nd or 3rd frame
+9) hex35_aa - an amino acid sequence for the -35 motif 
+10) hex10 - -10 hexamer sequence (a downstream 6-nucleotide site called the −10 motif)
+11) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
+12) hex10_sequence - contains 9nt sequence that includes -hex35 promoter if it's in the 2nd or 3rd frame
+13) hex10_aa - an amino acid sequence for the -10 motif 
+14) UP - an upstream sequence (UP). A 20-nucleotide region that appears upstream of the −35 motif.
+15) spacer - a spacer sequence that separates the −10 and −35 motifs 
+16) disc - discriminator sequence. A typically 6-nucleotide region in between the −10 motif and TSS. 
+17) ITR - the first 20 transcribed nucleotides called the initial transcribed region (ITR)
+18) new_gene_sequence - contains a gene sequence (nt) with substituted (Type = 'Modified Promoter') or  original promoters (Type = 'Original Promoter')
+19) promoter_sequence - contains -35 motif, spacer and - 10 motif 
+20) dG_total - total Gibbs free energy change (kcal/mol)
+21) dG_10 - Gibbs binding free Energy for -10 hexamer (kcal/mol)
+22) dG_35 - Gibbs binding free Energy for -35 hexamer (kcal/mol)
+23) dG_disc - Gibbs free energy penalty for non-optimal discriminator element (kcal/mol)
+24) dG_ITR - Gibbs free energy change for R-loop formation at the initial transcribed region (kcal/mol)
+25) dG_ext10 - Gibbs binding free energy for the extended -10 hexamer (kcal/mol)
+26) dG_spacer - Gibbs free energy penalty for non-optimal spacing (kcal/mol)
+27) dG_UP - Gibbs binding free energy for the upstream element (kcal/mol)
+28) dG_bind - binding Gibbs free energy 
+29) UP_position - a position of the UP element 
+30) hex35_position - a position of the -35 motif 
+31) spacer_position - a position of the spacer 
+32) hex10_position - a position of the -10 motif 
+33) disc_position - a position of the discriminator
 
 References:
 
 1. Logel DY, Trofimova E, Jaschke PR. Codon-Restrained Method for Both Eliminating and Creating Intragenic Bacterial Promoters. ACS Synth Biol. 2022 Jan 19;acssynbio.1c00359. Available from https://pubs.acs.org/doi/10.1021/acssynbio.1c00359. doi: 10.1021/acssynbio.1c00359
-2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
+2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
```

### Comparing `pssm-promoter-tool-1.0.5/free_energy_coeffs.npy` & `pssm-promoter-tool-1.0.6/free_energy_coeffs.npy`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.5/pssm_promoter_calculator.py` & `pssm-promoter-tool-1.0.6/pssm_promoter_calculator.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,14 +25,25 @@
         gene_sequence = str(records[0].seq)
     else:
         gene_sequence = f_content
 
     print("processing " + gene_file_name)
     return str.upper(gene_sequence)
 
+#number of promoter combinations to run: top 20 - by default and all - to run all combinations
+def get_promoter_opt():
+    if len(sys.argv) == 3:
+        prom_opt = str.lower(sys.argv[2])
+        if (prom_opt != 'all'):
+            raise Exception(
+                'Unrecognised value for the promoter combinations. Please specify "''all''" for all combinations.')
+    else:
+        prom_opt = 'min'
+
+    return prom_opt
 
 if __name__ == "__main__":
 
     from dask.distributed import Client, LocalCluster
     # cluster = LocalCluster()  # Launches a scheduler and workers locally
     # client = Client(cluster)
     client = Client()
@@ -46,27 +57,25 @@
     #sequence = "TCTATGCTCCAGGGCGATTAGGGAACAGCGTGTTGCTGGTCAGTAGTGTACCCTAGCCCACATAGCTACTTTTACTTCGTCCGTTCAGCGGACAAACGCT"
     #sequence = "ATGGTACGCTGGACTTTGTGGGATACCCTCGCTTTCCTGCTCCTGTTGAGTTTATTGCTGCCGTCATTGCTTATTATGTTCATCCCGTCAACATTCAAACGGCCTGTCTCATCATGGAAGGCGCTGAATTTACGGAAAACATTATTAATGGCGTCGAGCGTCCGGTTAAAGCCGCTGAATTGTTCGCGTTTACCTTGCGTGTACGCGCAGGAAACACTGACGTTCTTACTGACGCAGAAGAAAACGTGCGTCAAAAATTACGTGCGGAAAGAATGA"
     #sequence = "ATGAGTCAAGTTACTGAACAATCCGTACGTTTCCAGACCGCTTTGGCCTCTATTAAGCTCATTCAGGCTTCTGCCGTTTTGGATTTAACCGAAGATGATTTCGATTTTCTGACGAGTAACAAAGTTTGGATTGCTACTGACCGCTCTCGTGCTCGTCGCTGCGTTGAAGCTTGCGTTTACGGTACGCTGGACTTTGTGGGATACCCTCGCTTTCCTGCTCCTGTTGAGTTTATTGCTGCCGTCATTGCTTATTATGTTCATCCCGTCAACATTCAAACGGCCTGTCTCATCATGGAAGGCGCTGAATTTACGGAAAACATTATTAATGGCGTCGAGCGTCCGGTTAAAGCCGCTGAATTGTTCGCGTTTACCTTGCGTGTACGCGCAGGAAACACTGACGTTCTTACTGACGCAGAAGAAAACGTGCGTCAAAAATTACGTGCGGAGGGTGTGATGTAA"
     #sequence = "atgtctaaaggtaaaaaacgttctggcgctcgccctggtcgtccgcagccgttgcgaggtactaaaggcaagcgtaaaggcgctcgtctttggtatgtaggtggtcaacaattttaa"
 
 
     sequence = get_gene_sequence()
+
     calc = pssm_util.Promoter_Calculator()
     calc.run(sequence, TSS_range = [0, len(sequence)])
+    rev_TSS_df = calc.output()
     fwd_TSS_df, rev_TSS_df = calc.output()
-    end_time = datetime.now()
-    ##print('Duration of 1 salis calc run: {}'.format(end_time - start_time))
-
-    #fwd_TSS_df = TSS_results_to_df(output['Forward_Predictions_per_TSS'])
-    #rev_TSS_df = TSS_results_to_df(output['Reverse_Predictions_per_TSS'])
 
-    ##fwd_TSS_df = fwd_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer', 'ITR'], keep='last')
-    fwd_TSS_df = fwd_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer'], keep='last')
-    ##rev_TSS_df = rev_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer', 'ITR'], keep='last')
-    rev_TSS_df = rev_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer'], keep='last')
+    #fwd_TSS_df.groupby(by=['hex35', 'hex10', 'spacer']).first()
+    #fwd_TSS_df = fwd_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer', 'ITR'], keep='last')
+    fwd_TSS_df = fwd_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer'], keep='first')
+    #rev_TSS_df = rev_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer', 'ITR'], keep='last')
+    rev_TSS_df = rev_TSS_df.drop_duplicates(subset=['hex35', 'hex10', 'spacer'], keep='first')
 
     fwd_TSS_df = fwd_TSS_df.sort_values(by = 'Tx_rate', ascending = False)
     rev_TSS_df = rev_TSS_df.sort_values(by = 'Tx_rate', ascending = False)
 
     fwd_TSS_df['AA_Promoter_35'] = fwd_TSS_df['hex35'].apply(lambda x: str(Seq(x).translate()))
     fwd_TSS_df = fwd_TSS_df[fwd_TSS_df['AA_Promoter_35'].str.contains('*', regex = False) == False]
 
@@ -91,88 +100,71 @@
 
     min_rev_TSS_df = rev_TSS_df.head(1)
     def_rev_min_tx_rate = min_rev_TSS_df['Tx_rate'].values[0]
 
     max_rev_TSS_df = rev_TSS_df.tail(1)
     def_rev_max_tx_rate = max_rev_TSS_df['Tx_rate'].values[0]
 
-    max_min_tx_rate_df = {"sequence": sequence, "sequence_compl": str(Seq(sequence).reverse_complement()), "max_fwd": def_fwd_max_tx_rate, "max_rev": def_rev_max_tx_rate, "min_fwd": def_fwd_min_tx_rate, "min_rev": def_rev_min_tx_rate}
-
-    # for (TSS, result) in output['Forward_Predictions_per_TSS'].items():
-    #     print("Fwd TSS: %s. TX Rate: %s. Calcs: %s" % (TSS, result['Tx_rate'], str(result) ))
-    #     process_TSS_results(TSS, result)
-    #
-    # for (TSS, result) in output['Reverse_Predictions_per_TSS'].items():
-    #     print("Rev TSS: %s. TX Rate: %s. Calcs: %s" % (TSS, result['Tx_rate'], str(result) ))
-    #
-    # print("Elapsed Time: ", time.time() - begin, " seconds.")
-
-
-    #prm_df = process_promoters_nt(promoters_35, promoters_10, spacers)
-
-
+    max_min_tx_rate_df = {"sequence": sequence, "sequence_compl": str(Seq(sequence).reverse_complement()), "max_fwd": def_fwd_max_tx_rate, "max_rev": def_rev_max_tx_rate, "min_fwd": def_fwd_min_tx_rate, "min_rev": def_rev_min_tx_rate, "prom_opt": get_promoter_opt()}
 
     #processes 10 records to maximise and 10 to minimise
-    #IF PRIMERS ARE DUPLICATED TAKE ONLY with higher/lower tx rate
-
-    fwd_res_df_max = pssm_util.process_df_promoters(fwd_TSS_df.tail(10), 'fwd', 'max', max_min_tx_rate_df)
-    #fwd_res_df_max = pssm_util.process_df_promoters(fwd_TSS_df, 'fwd', 'max', max_min_tx_rate_df)
-    rev_res_df_max = pssm_util.process_df_promoters(rev_TSS_df.tail(12), 'rev', 'max', max_min_tx_rate_df)
-    #rev_res_df_max = pssm_util.process_df_promoters(rev_TSS_df, 'rev', 'max', max_min_tx_rate_df)
-
+    print("Minimising transcription rate on the forward strand..")
     fwd_res_df_min = pssm_util.process_df_promoters(fwd_TSS_df.head(10), 'fwd', 'min', max_min_tx_rate_df)
-    #fwd_res_df_min = pssm_util.process_df_promoters(fwd_TSS_df, 'fwd', 'min', max_min_tx_rate_df)
+    ##fwd_res_df_min = pssm_util.process_df_promoters(fwd_TSS_df, 'fwd', 'min', max_min_tx_rate_df)
+
+    print("Minimising transcription rate on the reverse strand..")
     rev_res_df_min = pssm_util.process_df_promoters(rev_TSS_df.head(10), 'rev', 'min', max_min_tx_rate_df)
-    #rev_res_df_min = pssm_util.process_df_promoters(rev_TSS_df, 'rev', 'min', max_min_tx_rate_df)
+    ##rev_res_df_min = pssm_util.process_df_promoters(rev_TSS_df, 'rev', 'min', max_min_tx_rate_df)
 
+    print("Maximising transcription rate on the forward strand..")
+    fwd_res_df_max = pssm_util.process_df_promoters(fwd_TSS_df.head(10), 'fwd', 'max', max_min_tx_rate_df)
+    ##fwd_res_df_max = pssm_util.process_df_promoters(fwd_TSS_df, 'fwd', 'max', max_min_tx_rate_df)
+
+    print("Maximising transcription rate on the reverse strand..")
+    rev_res_df_max = pssm_util.process_df_promoters(rev_TSS_df.head(10), 'rev', 'max', max_min_tx_rate_df)
+    ##rev_res_df_max = pssm_util.process_df_promoters(rev_TSS_df, 'rev', 'max', max_min_tx_rate_df)
 
-    #TODO:  keep original_TSS
-    #max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float) >= float(def_fwd_max_tx_rate)]
-##    max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float) >= float(def_fwd_max_tx_rate)]
-    #max_rev_TSS_df = rev_res_df_max.loc[rev_res_df_max['Tx_rate'].astype(float) >= float(def_rev_max_tx_rate)]
-##    max_rev_TSS_df = rev_res_df_max.loc[rev_res_df_max['Tx_rate'].astype(float) >= float(def_rev_max_tx_rate)]
-
-    #min_fwd_TSS_df = fwd_res_df_min.loc[fwd_res_df_min['Tx_rate'].astype(float) <= float(def_fwd_min_tx_rate)]
-##    min_fwd_TSS_df = fwd_res_df_min.loc[fwd_res_df_min['Tx_rate'].astype(float) <= float(def_fwd_min_tx_rate)]
-    #min_rev_TSS_df = rev_res_df_min.loc[rev_res_df_min['Tx_rate'].astype(float) <= float(def_rev_min_tx_rate)]
-##    min_rev_TSS_df = rev_res_df_min.loc[rev_res_df_min['Tx_rate'].astype(float) <= float(def_rev_min_tx_rate)]
 
     #res_final_df_max = pd.concat([max_fwd_TSS_df, max_rev_TSS_df], ignore_index=True, sort=False)
     res_final_df_max = pd.concat([fwd_res_df_max, rev_res_df_max], ignore_index=True, sort=False)
 
     #res_final_df_min = pd.concat([min_fwd_TSS_df, min_rev_TSS_df], ignore_index=True, sort=False)
     res_final_df_min = pd.concat([fwd_res_df_min, rev_res_df_min], ignore_index=True, sort=False)
 
     #res_final_df = res_final_df.drop_duplicates()
     res_final_df_max = res_final_df_max.drop_duplicates(
-        subset=['hex35', 'hex10', 'Tx_rate', 'ITR', 'Type', 'direction'],
+        subset=['hex35', 'hex10', 'Tx_rate', 'UP', 'ITR', 'Type', 'direction'],
         keep='last').reset_index(drop=True)
 
 
     res_final_df_min = res_final_df_min.drop_duplicates(
-        subset=['hex35', 'hex10', 'Tx_rate', 'ITR', 'Type', 'direction'],
+        subset=['hex35', 'hex10', 'Tx_rate', 'UP', 'ITR', 'Type', 'direction'],
         keep='last').reset_index(drop=True)
 
-    res_final_df_max['AA_hex35'] = res_final_df_max['hex35'].apply(lambda x: str(Seq(x).translate()))
-    res_final_df_min['AA_hex35'] = res_final_df_min['hex35'].apply(lambda x: str(Seq(x).translate()))
-    res_final_df_max['AA_hex10'] = res_final_df_max['hex10'].apply(lambda x: str(Seq(x).translate()))
-    res_final_df_min['AA_hex10'] = res_final_df_min['hex10'].apply(lambda x: str(Seq(x).translate()))
+    res_final_df_max['hex35_aa'] = res_final_df_max['hex35_9nt'].apply(lambda x: str(Seq(x).translate()))
+    res_final_df_min['hex35_aa'] = res_final_df_min['hex35_9nt'].apply(lambda x: str(Seq(x).translate()))
+    res_final_df_max['hex10_aa'] = res_final_df_max['hex10_9nt'].apply(lambda x: str(Seq(x).translate()))
+    res_final_df_min['hex10_aa'] = res_final_df_min['hex10_9nt'].apply(lambda x: str(Seq(x).translate()))
 
     #+PSSM values
-    res_final_df_max['PSSM_hex35'] = res_final_df_max['hex35'].apply(lambda x: pssm_util.calc_PSSM(x, '35'))
-    res_final_df_max['PSSM_hex10'] = res_final_df_max['hex10'].apply(lambda x: pssm_util.calc_PSSM(x, '10'))
-    res_final_df_min['PSSM_hex35'] = res_final_df_max['hex35'].apply(lambda x: pssm_util.calc_PSSM(x, '35'))
-    res_final_df_min['PSSM_hex10'] = res_final_df_max['hex10'].apply(lambda x: pssm_util.calc_PSSM(x, '10'))
+    res_final_df_max['PSSM_hex35'] = res_final_df_max['hex35'].apply(lambda x: pssm_util.calc_PSSM(x, 0, '35'))
+    res_final_df_max['PSSM_hex10'] = res_final_df_max['hex10'].apply(lambda x: pssm_util.calc_PSSM(x, 0, '10'))
+    res_final_df_min['PSSM_hex35'] = res_final_df_min['hex35'].apply(lambda x: pssm_util.calc_PSSM(x, 0, '35'))
+    res_final_df_min['PSSM_hex10'] = res_final_df_min['hex10'].apply(lambda x: pssm_util.calc_PSSM(x, 0, '10'))
 
     #perm_prom_pssm_df['PSSM_Promoters_perm'] = perm_prom_pssm_df['Promoters_perm_nt'].apply(lambda x: calc_PSSM(x, type))
 
     #res_final_df_max.to_csv('SalisLogelPromoterCalculator_MAX_results.csv')
     #res_final_df_min.to_csv('SalisLogelPromoterCalculator_MIN_results.csv')
 
-    print(sequence)
+    print("The processed gene sequence is " + sequence)
+
+    res_final_df_max = res_final_df_max.rename(columns={'hex35_9nt': 'hex35_sequence', 'hex10_9nt': 'hex10_sequence'})
+    res_final_df_min = res_final_df_min.rename(columns={'hex35_9nt': 'hex35_sequence', 'hex10_9nt': 'hex10_sequence'})
+
 
     res_final_df_max_fwd_df = res_final_df_max.loc[res_final_df_max["direction"] == 'fwd']
     new_max_fwd_Tx_rate_df = res_final_df_max_fwd_df.sort_values(by='Tx_rate', ascending=False)
     new_min_max_fwd_Tx_rate = new_max_fwd_Tx_rate_df['Tx_rate'].tail(1).values[0]
     new_max_max_fwd_Tx_rate = new_max_fwd_Tx_rate_df['Tx_rate'].head(1).values[0]
 
 
@@ -189,44 +181,49 @@
     new_min_max_rev_Tx_rate = new_max_rev_Tx_rate_df['Tx_rate'].tail(1).values[0]
 
     res_final_df_min_rev_df = res_final_df_min.loc[res_final_df_min["direction"] == 'rev']
     new_min_rev_Tx_rate_df = res_final_df_min_rev_df.sort_values(by='Tx_rate', ascending=False)
     new_max_min_rev_Tx_rate = new_min_rev_Tx_rate_df['Tx_rate'].head(1).values[0]
     new_min_min_rev_Tx_rate = new_min_rev_Tx_rate_df['Tx_rate'].tail(1).values[0]
 
-    column_list =  ["Type", "TSS", "Tx_rate", "Tx_rate_FoldChange", "hex35", "PSSM_hex35", "AA_hex35", "hex10", "PSSM_hex10", "AA_hex10", "UP", "spacer", "disc", "ITR", "new_gene_sequence", "promoter_sequence", "dG_total", "dG_10", "dG_35", "dG_disc", "dG_ITR", "dG_ext10", "dG_spacer", "dG_UP", "dG_bind",  "UP_position", "hex35_position", "spacer_position", "hex10_position", "disc_position"]
+
+
+    #column_list =  ["Type", "TSS", "Tx_rate", "Tx_rate_FoldChange", "hex35", "PSSM_hex35", "AA_hex35", "hex10", "PSSM_hex10", "AA_hex10", "UP", "spacer", "disc", "ITR", "new_gene_sequence", "promoter_sequence", "dG_total", "dG_10", "dG_35", "dG_disc", "dG_ITR", "dG_ext10", "dG_spacer", "dG_UP", "dG_bind",  "UP_position", "hex35_position", "spacer_position", "hex10_position", "disc_position"]
+    column_list =  ["Type", "TSS", "Tx_rate", "Tx_rate_FoldChange", "frame", "hex35", "PSSM_hex35", "hex35_sequence", "hex35_aa", "hex10", "PSSM_hex10", "hex10_sequence", "hex10_aa", "UP", "spacer", "disc", "ITR", "new_gene_sequence", "promoter_sequence", "dG_total", "dG_10", "dG_35", "dG_disc", "dG_ITR", "dG_ext10", "dG_spacer", "dG_UP", "dG_bind",  "UP_position", "hex35_position", "spacer_position", "hex10_position", "disc_position"]
 
     ##max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float)
     ##max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float) >= float(def_fwd_max_tx_rate)]
 
     print("\nThe maximum transcription rate for the sequence (forward) is " + str(new_max_min_fwd_Tx_rate))
     if len(res_final_df_min_fwd_df) > 1:
         min_fwd_output_file = OUTPUT_FILE_NAME + "_MIN_FWD_results.csv"
         #if float(new_min_fwd_Tx_rate) < float(def_fwd_min_tx_rate):
         if float(new_min_min_fwd_Tx_rate) < float(new_max_min_fwd_Tx_rate):
             print ("can be decreased up to " + str(new_min_min_fwd_Tx_rate))
             print(USE_PROMOTERS_OUTPUT + "(" + min_fwd_output_file + ")")
             #res_final_df_min_fwd_df['Tx_rate_FoldChange'] = res_final_df_min_fwd_df['Tx_rate'].copy()/def_fwd_min_tx_rate.astype(float)
             res_final_df_min_fwd_df = pssm_util.add_txrate_foldchange_col(res_final_df_min_fwd_df, 'min')
-            res_final_df_min_fwd_df.to_csv(min_fwd_output_file, columns = column_list, float_format='%.2f')
+            ##res_final_df_min_fwd_df.to_csv(min_fwd_output_file, columns = column_list, float_format='%.2f')
+            res_final_df_min_fwd_df.to_csv(min_fwd_output_file, columns = column_list)
 
             ##files.download(min_fwd_output_file)
 
     else:
         print(" cannot be further decreased")
 
     print("\nThe maximum transcription rate for the sequence (reverse) is " + str(new_max_min_rev_Tx_rate))
     if len(res_final_df_min_rev_df) > 1:
         min_rev_output_file = OUTPUT_FILE_NAME + "_MIN_REV_results.csv"
         #if float(new_min_rev_Tx_rate) < float(def_rev_min_tx_rate):
         if float(new_min_min_rev_Tx_rate) < float(new_max_min_rev_Tx_rate):
             print ("can be decreased up to " + str(new_min_min_rev_Tx_rate))
             print(USE_PROMOTERS_OUTPUT + "(" + min_rev_output_file + ")")
             res_final_df_min_rev_df = pssm_util.add_txrate_foldchange_col(res_final_df_min_rev_df, 'min')
-            res_final_df_min_rev_df.to_csv(min_rev_output_file, columns = column_list, float_format='%.2f')
+            #res_final_df_min_rev_df.to_csv(min_rev_output_file, columns = column_list, float_format='%.2f')
+            res_final_df_min_rev_df.to_csv(min_rev_output_file, columns = column_list)
 
             ##files.download(min_rev_output_file)
 
     else:
         print(" cannot be further decreased")
 
     print("\nThe minimum transcription rate for the sequence (forward) is " + str(new_min_max_fwd_Tx_rate))
@@ -234,29 +231,31 @@
         max_fwd_output_file = OUTPUT_FILE_NAME + "_MAX_FWD_results.csv"
         #if float(new_max_fwd_Tx_rate) > float(def_fwd_max_tx_rate):
         if float(new_max_max_fwd_Tx_rate) > float(new_min_max_fwd_Tx_rate):
             print ("can be increased up to " + str(new_max_max_fwd_Tx_rate))
             print(USE_PROMOTERS_OUTPUT + "(" + max_fwd_output_file + ")")
             res_final_df_max_fwd_df = pssm_util.add_txrate_foldchange_col(res_final_df_max_fwd_df, 'max')
 
-            res_final_df_max_fwd_df.to_csv(max_fwd_output_file, columns = column_list, float_format='%.2f')
+            #res_final_df_max_fwd_df.to_csv(max_fwd_output_file, columns = column_list, float_format='%.2f')
+            res_final_df_max_fwd_df.to_csv(max_fwd_output_file, columns = column_list)
             ##files.download(max_fwd_output_file)
     else:
         print(" cannot be further increased")
 
     print("\nThe minimum transcription rate for the sequence (reverse) is " + str(new_min_max_rev_Tx_rate))
     if len(res_final_df_max_rev_df) > 1:
         max_rev_output_file = OUTPUT_FILE_NAME + "_MAX_REV_results.csv"
         #if float(new_max_rev_Tx_rate) > float(def_rev_max_tx_rate):
         if float(new_max_max_rev_Tx_rate) > float(new_min_max_rev_Tx_rate):
             print ("can be increased up to " + str(new_max_max_rev_Tx_rate))
             print(USE_PROMOTERS_OUTPUT + "(" + max_rev_output_file + ")")
             res_final_df_max_rev_df = pssm_util.add_txrate_foldchange_col(res_final_df_max_rev_df, 'max')
 
-            res_final_df_max_rev_df.to_csv(max_rev_output_file, columns = column_list, float_format='%.2f')
+            #res_final_df_max_rev_df.to_csv(max_rev_output_file, columns = column_list, float_format='%.2f')
+            res_final_df_max_rev_df.to_csv(max_rev_output_file, columns = column_list)
             ##files.download(max_rev_output_file)
 
     else:
         print(" cannot be further increased")
 
     print("\n")
```

### Comparing `pssm-promoter-tool-1.0.5/pssm_promoter_tool.egg-info/PKG-INFO` & `pssm-promoter-tool-1.0.6/pssm_promoter_tool.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: pssm-promoter-tool
-Version: 1.0.5
+Version: 1.0.6
 Summary: The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence
 Home-page: https://github.com/ellinium/PSSM_PromoterTool
 Author: Ellina Trofimova
 Author-email: ellina.trofimova@gmail.com
 License: GNU General Public License
 Keywords: promoter prediction transcription rate
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 **PSSM Promoter Tool**
 
 The tool applies CORPSE (Codon Restrained Promoter Silencing) method and inverted CORPSE (iCORPSE) to the provided gene sequence.
 
--35 and -10 promoters along with the additional non-canonical sequence motifs are predicted based on the Salis Lab Promoter Calculator (https://github.com/hsalis/SalisLabCode/tree/master/Promoter_Calculator).
+-35 and -10 promoters, along with the additional non-canonical sequence motifs, are predicted based on the Salis Lab Promoter Calculator (https://github.com/hsalis/SalisLabCode/tree/master/Promoter_Calculator).
 Position-specific scoring matrix (PSSM) is applied to all the synonymous codon variants of the promoters associated with the lowest and highest transcription rates in order to maximally decrease (CORPSE) or increase the transcription rate (iCORPSE).
-The output CSV file/files contain synonymous codon promoters and sequence motifs for the minimal and maximal transcriptional rates along with the non-canonical sequence motifs for forward and reverse strands.
+The output CSV file/files contain synonymous codon promoters and sequence motifs for the minimal and maximal transcriptional rates, along with the non-canonical sequence motifs for forward and reverse strands.
 
 For a web (Google Colab) version, please navigate to https://colab.research.google.com/drive/171iBNCrA1hMS-LpX_qaFani34HiueTZO?usp=sharing.
 
 INSTALLATION:
 
 1. Install required libraries using pip:
 ```
@@ -28,61 +28,71 @@
 ```
 
 2. Download and unpack the archive with files using "Code"->"Download ZIP" buttons in the right corner at https://github.com/ellinium/pssm_promoter_tool. 
 Or use
 ```
 git clone https://github.com/ellinium/pssm-promoter-tool
 ```
-[! you need to have a Git account and be authorised in the system to run the command !]
+[! it's necessary to have a Git account and be authorised in the system to run the command !]
 
 
 USAGE:
 
 The tool requires a text or fasta file with a nucleotide sequence of a gene to process.
-From the folder with the downloaded files run:
+From the folder with the downloaded files, run:
 ```
 python pssm_promoter_calculator.py <file_name>
 ```
 where 'file_name' is a path to the file with a gene sequence (TXT or FASTA format).
 
+By default, the command processes 40 PSSM promoter combinations with the highest PSSM scores for transcription rate maximisation or 40 combinations with the lowest PSSM scores for transcription rate minimisation.
+To run all the promoter combinations, use an additional argument 'all':
+```
+python pssm_promoter_calculator.py <file_name> all
+```
+
+
 Depending on the result, up to four output CSV files can be generated:
 1) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
 2) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
 3) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
 4) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
 1) Type - 'Original Promoter' - for original sequence promoters; 'Modified Promoter' - for synonymous promoters. 
-2) TSS -  transcriptional start site 
-3) Tx_rate - transcription initiation rate 
-4) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers 
-5) hex35 -  an upstream 6-nucleotide site called the −35 motif 
-6) PSSM_hex35 - position-specific scoring matrix value for the -35 motif 
-7) AA_hex35 - an amino acid sequence for the -35 motif 
-8) hex10 - a downstream 6-nucleotide site called the −10 motif 
-9) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
-10) AA_hex10 - an amino acid sequence for the -10 motif 
-11) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
-12) spacer - a spacer region that separates the −10 and −35 motifs 
-13) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
-14) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
-15) new_gene_sequence - contains a gene sequence (nt) with substituted (Type = 'Modified Promoter') or  original promoters (Type = 'Original Promoter')
-16) promoter_sequence - contains -35 motif, spacer and - 10 motif 
-17) dG_total - total Gibbs free energy for the sequence 
-18) dG_10 - -10 motif Gibbs free energy 
-19) dG_35 - -35 motif Gibbs free energy 
-20) dG_disc - a discriminator Gibbs free energy 
-21) dG_ITR - an ITR Gibbs free energy 
-22) dG_ext10 −10 extended motif Gibbs free energy 
-23) dG_spacer - a spacer Gibbs free energy 
-24) dG_UP - an UP Gibbs free energy 
-25) dG_bind - binding Gibbs free energy 
-26) UP_position - a position of the UP element 
-27) hex35_position - a position of the -35 motif 
-28) spacer_position - a position of the spacer 
-29) hex10_position - a position of the -10 motif 
-30) disc_position - a position of the discriminator
+2) TSS -  transcriptional start Site position (nt) 
+3) Tx_rate - transcription unitiation rate (au)
+4) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
+5) frame - a reading frame for the promoters 
+6) hex35 - -35 hexamer sequence (an upstream 6-nucleotide site called the −35 motif)
+7) PSSM_hex35 - position-specific scoring matrix value for the -35 motif 
+8) hex35_sequence - contains 9nt sequence that includes -hex35 promoter if it's in the 2nd or 3rd frame
+9) hex35_aa - an amino acid sequence for the -35 motif 
+10) hex10 - -10 hexamer sequence (a downstream 6-nucleotide site called the −10 motif)
+11) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
+12) hex10_sequence - contains 9nt sequence that includes -hex35 promoter if it's in the 2nd or 3rd frame
+13) hex10_aa - an amino acid sequence for the -10 motif 
+14) UP - an upstream sequence (UP). A 20-nucleotide region that appears upstream of the −35 motif.
+15) spacer - a spacer sequence that separates the −10 and −35 motifs 
+16) disc - discriminator sequence. A typically 6-nucleotide region in between the −10 motif and TSS. 
+17) ITR - the first 20 transcribed nucleotides called the initial transcribed region (ITR)
+18) new_gene_sequence - contains a gene sequence (nt) with substituted (Type = 'Modified Promoter') or  original promoters (Type = 'Original Promoter')
+19) promoter_sequence - contains -35 motif, spacer and - 10 motif 
+20) dG_total - total Gibbs free energy change (kcal/mol)
+21) dG_10 - Gibbs binding free Energy for -10 hexamer (kcal/mol)
+22) dG_35 - Gibbs binding free Energy for -35 hexamer (kcal/mol)
+23) dG_disc - Gibbs free energy penalty for non-optimal discriminator element (kcal/mol)
+24) dG_ITR - Gibbs free energy change for R-loop formation at the initial transcribed region (kcal/mol)
+25) dG_ext10 - Gibbs binding free energy for the extended -10 hexamer (kcal/mol)
+26) dG_spacer - Gibbs free energy penalty for non-optimal spacing (kcal/mol)
+27) dG_UP - Gibbs binding free energy for the upstream element (kcal/mol)
+28) dG_bind - binding Gibbs free energy 
+29) UP_position - a position of the UP element 
+30) hex35_position - a position of the -35 motif 
+31) spacer_position - a position of the spacer 
+32) hex10_position - a position of the -10 motif 
+33) disc_position - a position of the discriminator
 
 References:
 
 1. Logel DY, Trofimova E, Jaschke PR. Codon-Restrained Method for Both Eliminating and Creating Intragenic Bacterial Promoters. ACS Synth Biol. 2022 Jan 19;acssynbio.1c00359. Available from https://pubs.acs.org/doi/10.1021/acssynbio.1c00359. doi: 10.1021/acssynbio.1c00359
 2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
```

### Comparing `pssm-promoter-tool-1.0.5/setup.py` & `pssm-promoter-tool-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='pssm-promoter-tool',
-      version='1.0.5',
+      version='1.0.6',
       description='The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/ellinium/PSSM_PromoterTool',
       author='Ellina Trofimova',
       author_email='ellina.trofimova@gmail.com',
       license='GNU General Public License',
```

