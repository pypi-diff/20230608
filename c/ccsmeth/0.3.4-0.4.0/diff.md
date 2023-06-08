# Comparing `tmp/ccsmeth-0.3.4.tar.gz` & `tmp/ccsmeth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccsmeth-0.3.4.tar", last modified: Fri May 26 03:04:43 2023, max compression
+gzip compressed data, was "ccsmeth-0.4.0.tar", last modified: Thu Jun  8 06:50:24 2023, max compression
```

## Comparing `ccsmeth-0.3.4.tar` & `ccsmeth-0.4.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 03:04:43.336925 ccsmeth-0.3.4/
--rw-rw-rw-   0        0        0     1683 2023-03-22 03:41:13.000000 ccsmeth-0.3.4/LICENSE
--rw-rw-rw-   0        0        0       84 2023-03-22 03:41:13.000000 ccsmeth-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2319 2023-05-26 03:04:43.336925 ccsmeth-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0     1513 2023-05-26 02:48:04.000000 ccsmeth-0.3.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-26 03:04:43.187017 ccsmeth-0.3.4/ccsmeth/
--rw-rw-rw-   0        0        0        0 2022-05-16 12:12:40.000000 ccsmeth-0.3.4/ccsmeth/__init__.py
--rw-rw-rw-   0        0        0    15200 2023-03-22 03:41:13.000000 ccsmeth-0.3.4/ccsmeth/_bam2modbam.py
--rw-rw-rw-   0        0        0       18 2023-05-26 03:01:01.000000 ccsmeth-0.3.4/ccsmeth/_version.py
--rw-rw-rw-   0        0        0     9878 2023-03-22 03:41:13.000000 ccsmeth-0.3.4/ccsmeth/align_hifi_reads.py
--rw-rw-rw-   0        0        0     6040 2023-03-22 03:41:13.000000 ccsmeth-0.3.4/ccsmeth/call_hifi_reads.py
--rw-rw-rw-   0        0        0    30718 2023-05-09 07:02:54.000000 ccsmeth-0.3.4/ccsmeth/call_modifications.py
--rw-rw-rw-   0        0        0    37939 2023-05-09 07:03:05.000000 ccsmeth-0.3.4/ccsmeth/call_mods_freq_bam.py
--rw-rw-rw-   0        0        0    18444 2023-03-22 03:41:14.000000 ccsmeth-0.3.4/ccsmeth/call_mods_freq_txt.py
--rw-rw-rw-   0        0        0    54823 2023-05-09 07:02:13.000000 ccsmeth-0.3.4/ccsmeth/ccsmeth.py
--rw-rw-rw-   0        0        0     6872 2023-05-26 02:33:38.000000 ccsmeth-0.3.4/ccsmeth/dataloader.py
--rw-rw-rw-   0        0        0    31796 2023-05-26 02:33:21.000000 ccsmeth-0.3.4/ccsmeth/extract_features.py
--rw-rw-rw-   0        0        0    10097 2023-04-26 02:27:23.000000 ccsmeth-0.3.4/ccsmeth/models.py
--rw-rw-rw-   0        0        0    20305 2023-03-22 03:41:14.000000 ccsmeth-0.3.4/ccsmeth/train.py
--rw-rw-rw-   0        0        0    25193 2023-04-23 13:09:00.000000 ccsmeth-0.3.4/ccsmeth/train_multigpu.py
-drwxrwxrwx   0        0        0        0 2023-05-26 03:04:43.329932 ccsmeth-0.3.4/ccsmeth/utils/
--rw-rw-rw-   0        0        0        0 2022-05-21 04:53:39.000000 ccsmeth-0.3.4/ccsmeth/utils/__init__.py
--rw-rw-rw-   0        0        0     2801 2023-03-22 03:41:14.000000 ccsmeth-0.3.4/ccsmeth/utils/attention.py
--rw-rw-rw-   0        0        0      756 2023-03-22 03:41:14.000000 ccsmeth-0.3.4/ccsmeth/utils/constants_torch.py
--rw-rw-rw-   0        0        0     4077 2023-03-22 03:41:14.000000 ccsmeth-0.3.4/ccsmeth/utils/lookahead.py
--rw-rw-rw-   0        0        0    13974 2023-03-22 03:41:15.000000 ccsmeth-0.3.4/ccsmeth/utils/process_utils.py
--rw-rw-rw-   0        0        0     9051 2022-05-16 12:12:41.000000 ccsmeth-0.3.4/ccsmeth/utils/ranger2020.py
--rw-rw-rw-   0        0        0     2789 2022-05-16 12:12:41.000000 ccsmeth-0.3.4/ccsmeth/utils/ref_reader.py
--rw-rw-rw-   0        0        0      963 2023-03-22 03:41:15.000000 ccsmeth-0.3.4/ccsmeth/utils/sam2fastq_std.py
-drwxrwxrwx   0        0        0        0 2023-05-26 03:04:43.252976 ccsmeth-0.3.4/ccsmeth.egg-info/
--rw-rw-rw-   0        0        0     2319 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 11:32:42.000000 ccsmeth-0.3.4/ccsmeth.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      134 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-26 03:04:41.000000 ccsmeth-0.3.4/ccsmeth.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      152 2023-03-22 03:41:16.000000 ccsmeth-0.3.4/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-26 03:04:43.344920 ccsmeth-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     2017 2023-03-22 03:41:17.000000 ccsmeth-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:50:24.398489 ccsmeth-0.4.0/
+-rw-rw-rw-   0        0        0     1683 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       60 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2405 2023-06-08 06:50:24.398489 ccsmeth-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1594 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-08 06:50:24.369586 ccsmeth-0.4.0/ccsmeth/
+-rw-rw-rw-   0        0        0        0 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/__init__.py
+-rw-rw-rw-   0        0        0    15258 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/_bam2modbam.py
+-rw-rw-rw-   0        0        0    16985 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/_call_modifications_txt.py
+-rw-rw-rw-   0        0        0       18 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/_version.py
+-rw-rw-rw-   0        0        0     9673 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/align_hifi_reads.py
+-rw-rw-rw-   0        0        0     5907 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/call_hifi_reads.py
+-rw-rw-rw-   0        0        0    32638 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/call_modifications.py
+-rw-rw-rw-   0        0        0    37997 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/call_mods_freq_bam.py
+-rw-rw-rw-   0        0        0    18546 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/call_mods_freq_txt.py
+-rw-rw-rw-   0        0        0    54821 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/ccsmeth.py
+-rw-rw-rw-   0        0        0     6872 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/dataloader.py
+-rw-rw-rw-   0        0        0    30220 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/extract_features.py
+-rw-rw-rw-   0        0        0    10097 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/models.py
+-rw-rw-rw-   0        0        0    20305 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/train.py
+-rw-rw-rw-   0        0        0    25193 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/train_multigpu.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:50:24.397492 ccsmeth-0.4.0/ccsmeth/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/__init__.py
+-rw-rw-rw-   0        0        0     2801 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/attention.py
+-rw-rw-rw-   0        0        0      756 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/constants_torch.py
+-rw-rw-rw-   0        0        0     4077 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/lookahead.py
+-rw-rw-rw-   0        0        0    13971 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/ccsmeth/utils/process_utils.py
+-rw-rw-rw-   0        0        0     9051 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/ranger2020.py
+-rw-rw-rw-   0        0        0     2789 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/ref_reader.py
+-rw-rw-rw-   0        0        0      963 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/ccsmeth/utils/sam2fastq_std.py
+drwxrwxrwx   0        0        0        0 2023-06-08 06:50:24.389520 ccsmeth-0.4.0/ccsmeth.egg-info/
+-rw-rw-rw-   0        0        0     2405 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      888 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      134 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-08 06:50:24.000000 ccsmeth-0.4.0/ccsmeth.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      152 2023-06-04 08:15:25.000000 ccsmeth-0.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-06-08 06:50:24.403473 ccsmeth-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     2034 2023-06-08 06:45:58.000000 ccsmeth-0.4.0/setup.py
```

### Comparing `ccsmeth-0.3.4/LICENSE` & `ccsmeth-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/PKG-INFO` & `ccsmeth-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ccsmeth
-Version: 0.3.4
+Version: 0.4.0
 Summary: Detecting DNA methylation from PacBio CCS reads
 Home-page: https://github.com/PengNi/ccsmeth
-Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.3.4.tar.gz
+Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.4.0.tar.gz
 Author: Peng Ni
 Author-email: 543943952@qq.com
 License: BSD-3-Clause-Clear license
 Keywords: methylation,pacbio,neural network
 Platform: Linux
 Platform: MacOS
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,19 @@
 
 ccsmeth
 ========
 
 
 Documentation
 -------------
+v0.4.0
+----------
+optimieze call_mods module, faster generating of modbam file
+
+
 v0.3.4
 ----------
 replace 'numpy.float' by 'float" in extract_features and call_mods modules
 
 
 v0.3.3
 ----------
```

### Comparing `ccsmeth-0.3.4/README.rst` & `ccsmeth-0.4.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 ccsmeth
 ========
 
 
 Documentation
 -------------
+v0.4.0
+----------
+optimieze call_mods module, faster generating of modbam file
+
+
 v0.3.4
 ----------
 replace 'numpy.float' by 'float" in extract_features and call_mods modules
 
 
 v0.3.3
 ----------
```

### Comparing `ccsmeth-0.3.4/ccsmeth/_bam2modbam.py` & `ccsmeth-0.4.0/ccsmeth/_bam2modbam.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 import pybedtools
 import gzip
 
 import multiprocessing as mp
 from multiprocessing import Queue
 
 from .utils.process_utils import complement_seq
+from .utils.process_utils import max_queue_size
 
 base = "C"
 pred_base = "CG"
 
-queue_size_border = 1000
+queue_size_border = max_queue_size
 time_wait = 1
 
 
 # generate per_read bed file ==============================
 def _generate_per_read_calls(per_readsite, output):
     # chromosome, pos, strand, read_name, read_loc, depth, prob_0, prob_1, called_label, seq
     wf = open(output, "w")
```

### Comparing `ccsmeth-0.3.4/ccsmeth/align_hifi_reads.py` & `ccsmeth-0.4.0/ccsmeth/align_hifi_reads.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-import os
-import argparse
-import sys
-import time
-
-from .utils.process_utils import run_cmd
-from .utils.process_utils import display_args
-from .utils.process_utils import pbmm2_exec
-from .utils.process_utils import minimap2_exec
-from .utils.process_utils import bwa_exec
-from .utils.process_utils import generate_samtools_view_cmd
-from .utils.process_utils import generate_samtools_index_cmd
-from .utils.process_utils import generate_samtools_sort_cmd
-
-
-here = os.path.abspath(os.path.dirname(__file__))
-sam2fq_exec = "python " + here + "/utils/sam2fastq_std.py"
-
-
-def check_input_file(inputfile):
-    if not (inputfile.endswith(".bam") or inputfile.endswith(".sam") or inputfile.endswith(".fq")
-            or inputfile.endswith(".fastq")):
-        raise ValueError("--hifireads/-i must be in bam/sam/fastq format!")
-    inputpath = os.path.abspath(inputfile)
-    return inputpath
-
-
-def check_output_file(outputfile, inputfile, is_minimap2, is_bwa):
-    if outputfile is None:
-        fname, fext = os.path.splitext(inputfile)
-        aligner = "pbmm2"
-        if is_minimap2:
-            aligner = "minimap2"
-        elif is_bwa:
-            aligner = "bwa"
-        output_path = fname + "." + aligner + ".bam"
-    else:
-        if not (outputfile.endswith(".sam") or outputfile.endswith(".bam")):
-            raise ValueError("--output/-o must be in bam/sam format!")
-        output_path = os.path.abspath(outputfile)
-    return output_path
-
-
-def generate_aligner_with_options(is_minimap2, path_to_minimap2, is_bwa, path_to_bwa, path_to_pbmm2,
-                                  bestn, threads):
-    aligner = pbmm2_exec
-    if is_minimap2:
-        aligner = minimap2_exec
-        if path_to_minimap2 is not None:
-            aligner = os.path.abspath(path_to_minimap2)
-        num_sencondary = bestn - 1
-        if num_sencondary == 0:
-            aligner += " -ax map-hifi -y -t {t} --secondary=no".format(t=threads)  # avoid -N0
-        if num_sencondary == 1:
-            aligner += " -ax map-hifi -y -t {t} --secondary=no".format(t=threads)  # avoid -N1
-        else:
-            aligner += " -ax map-hifi -y -t {t} -N {N}".format(t=threads,
-                                                               N=num_sencondary)
-    elif is_bwa:
-        aligner = bwa_exec
-        if path_to_bwa is not None:
-            aligner = os.path.abspath(path_to_bwa)
-        aligner += " mem -x pacbio -C -V -t {t}".format(t=threads)
-    else:
-        if path_to_pbmm2 is not None:
-            aligner = os.path.abspath(path_to_pbmm2)
-        aligner += " align --preset HIFI -j {t} --sort ".format(t=threads)
-    return aligner
-
-
-def align_hifi_reads_to_genome(args):
-    sys.stderr.write("[align_hifi_reads]start..\n")
-    start = time.time()
-    inputpath = check_input_file(args.hifireads)
-    outputpath = check_output_file(args.output, inputpath, args.minimap2, args.bwa)
-    reference = os.path.abspath(args.ref)
-
-    if not os.path.exists(inputpath):
-        raise IOError("input file does not exist!")
-    if not os.path.exists(reference):
-        raise IOError("refernce(--ref) file does not exist!")
-
-    aligner = generate_aligner_with_options(args.minimap2,
-                                            args.path_to_minimap2,
-                                            args.bwa,
-                                            args.path_to_bwa,
-                                            args.path_to_pbmm2,
-                                            args.bestn,
-                                            args.threads)
-    samtools_view = generate_samtools_view_cmd(args.path_to_samtools, args.threads // 2)
-    samtools_index = generate_samtools_index_cmd(args.path_to_samtools, args.threads)
-
-    if (not args.minimap2) and (not args.bwa):
-        if outputpath.endswith(".bam"):
-            align_cmds = " ".join([aligner, reference, inputpath, outputpath])
-            post_align_cmd = " ".join([samtools_index, outputpath])
-            align_cmds = " && ".join([align_cmds, post_align_cmd])
-        elif outputpath.endswith(".sam"):
-            align_cmds = " ".join([aligner, reference, inputpath])
-            post_align_cmds = " ".join([samtools_view, "- >", outputpath])
-            align_cmds = " | ".join([align_cmds, post_align_cmds])
-        else:
-            raise ValueError("--output/-o must be in bam/sam format!")
-    else:
-        align_cmds = " ".join([aligner, reference, "-"])
-        if inputpath.endswith(".fq") or inputpath.endswith(".fastq"):
-            align_cmds = " ".join([aligner, reference, inputpath])
-        if outputpath.endswith(".sam"):
-            align_cmds += " > {}".format(outputpath)
-
-        pre_align_cmds = ""
-        if inputpath.endswith(".fq") or inputpath.endswith(".fastq"):
-            # pre_align_cmds += " ".join(["cat", inputpath])
-            pass
-        else:
-            if inputpath.endswith(".bam"):
-                pre_align_cmds += " ".join([samtools_view, inputpath])
-                pre_align_cmds += " | " + sam2fq_exec
-            elif inputpath.endswith(".sam"):
-                # pre_align_cmds += " ".join(["cat", inputpath])
-                pre_align_cmds += sam2fq_exec + " < " + inputpath
-            else:
-                raise ValueError()
-
-        post_align_cmds = ""
-        if outputpath.endswith(".bam"):
-            samtools_sort = generate_samtools_sort_cmd(args.path_to_samtools, outputpath, args.threads // 2)
-            post_align_cmds = " ".join([samtools_view, "-b |",
-                                        samtools_sort, "- &&",
-                                        samtools_index, outputpath])
-        elif outputpath.endswith(".sam"):
-            pass
-
-        if pre_align_cmds != "":
-            align_cmds = " | ".join([pre_align_cmds, align_cmds])
-        if post_align_cmds != "":
-            align_cmds = " | ".join([align_cmds, post_align_cmds])
-
-    sys.stderr.write("cmds: {}\n".format(align_cmds))
-    stdinfo, returncode = run_cmd(align_cmds)
-    stdout, stderr = stdinfo
-    if returncode:
-        sys.stderr.write("failed..\n")
-    else:
-        sys.stderr.write("succeeded..\n")
-    sys.stderr.write("==stdout:\n{}\n".format(str(stdout, 'utf-8')))
-    sys.stderr.write("==stderr:\n{}\n".format(str(stderr, 'utf-8')))
-
-    endtime = time.time()
-    sys.stderr.write("[align_hifi_reads]costs {:.1f} seconds\n".format(endtime - start))
-
-
-def main():
-    parser = argparse.ArgumentParser("align hifi reads using pbmm2/minimap2/bwa, default pbmm2")
-    p_input = parser.add_argument_group("INPUT")
-    p_input.add_argument("--hifireads", "-i", type=str, required=True,
-                         help="path to hifireads.bam/sam/fastq_with_pulseinfo file as input")
-    p_input.add_argument("--ref", type=str, required=True,
-                         help="path to genome reference to be aligned, in fasta/fa format. "
-                              "If using bwa, the reference must have already been indexed.")
-
-    p_output = parser.add_argument_group("OUTPUT")
-    p_output.add_argument("--output", "-o", type=str, required=False,
-                          help="output file path for alignment results, bam/sam supported. "
-                               "If not specified, the results will be saved in "
-                               "input_file_prefix.bam by default.")
-    p_output.add_argument("--header", action="store_true", default=False, required=False,
-                          help="save header annotations from bam/sam. DEPRECATED")
-
-    p_align = parser.add_argument_group("ALIGN")
-    p_align.add_argument("--path_to_pbmm2", type=str, default=None, required=False,
-                         help="full path to the executable binary pbmm2 file. "
-                              "If not specified, it is assumed that pbmm2 is "
-                              "in the PATH.")
-    p_align.add_argument("--minimap2", action="store_true", default=False, required=False,
-                         help="use minimap2 instead of pbmm2 for alignment")
-    p_align.add_argument("--path_to_minimap2", type=str, default=None, required=False,
-                         help="full path to the executable binary minimap2 file. "
-                              "If not specified, it is assumed that minimap2 is "
-                              "in the PATH.")
-    p_align.add_argument("--bestn", "-n", type=int, default=3, required=False,
-                         help="retain at most n alignments in minimap2. "
-                              "default 3, which means 2 secondary alignments are retained. "
-                              "Do not use 2, cause -N1 is not suggested for high accuracy of alignment. "
-                              "[This arg is for further extension.]")
-    p_align.add_argument("--bwa", action="store_true", default=False, required=False,
-                         help="use bwa instead of pbmm2 for alignment")
-    p_align.add_argument("--path_to_bwa", type=str, default=None, required=False,
-                         help="full path to the executable binary bwa file. If not "
-                              "specified, it is assumed that bwa is in the PATH.")
-    p_align.add_argument("--path_to_samtools", type=str, default=None, required=False,
-                         help="full path to the executable binary samtools file. "
-                              "If not specified, it is assumed that samtools is in "
-                              "the PATH.")
-    p_align.add_argument("--threads", "-t", type=int, default=5, required=False,
-                         help="number of threads, default 5")
-
-    args = parser.parse_args()
-
-    display_args(args, True)
-    align_hifi_reads_to_genome(args)
-
-
-if __name__ == '__main__':
-    main()
+import os
+import argparse
+import sys
+import time
+
+from .utils.process_utils import run_cmd
+from .utils.process_utils import display_args
+from .utils.process_utils import pbmm2_exec
+from .utils.process_utils import minimap2_exec
+from .utils.process_utils import bwa_exec
+from .utils.process_utils import generate_samtools_view_cmd
+from .utils.process_utils import generate_samtools_index_cmd
+from .utils.process_utils import generate_samtools_sort_cmd
+
+
+here = os.path.abspath(os.path.dirname(__file__))
+sam2fq_exec = "python " + here + "/utils/sam2fastq_std.py"
+
+
+def check_input_file(inputfile):
+    if not (inputfile.endswith(".bam") or inputfile.endswith(".sam") or inputfile.endswith(".fq")
+            or inputfile.endswith(".fastq")):
+        raise ValueError("--hifireads/-i must be in bam/sam/fastq format!")
+    inputpath = os.path.abspath(inputfile)
+    return inputpath
+
+
+def check_output_file(outputfile, inputfile, is_minimap2, is_bwa):
+    if outputfile is None:
+        fname, fext = os.path.splitext(inputfile)
+        aligner = "pbmm2"
+        if is_minimap2:
+            aligner = "minimap2"
+        elif is_bwa:
+            aligner = "bwa"
+        output_path = fname + "." + aligner + ".bam"
+    else:
+        if not (outputfile.endswith(".sam") or outputfile.endswith(".bam")):
+            raise ValueError("--output/-o must be in bam/sam format!")
+        output_path = os.path.abspath(outputfile)
+    return output_path
+
+
+def generate_aligner_with_options(is_minimap2, path_to_minimap2, is_bwa, path_to_bwa, path_to_pbmm2,
+                                  bestn, threads):
+    aligner = pbmm2_exec
+    if is_minimap2:
+        aligner = minimap2_exec
+        if path_to_minimap2 is not None:
+            aligner = os.path.abspath(path_to_minimap2)
+        num_sencondary = bestn - 1
+        if num_sencondary == 0:
+            aligner += " -ax map-hifi -y -t {t} --secondary=no".format(t=threads)  # avoid -N0
+        if num_sencondary == 1:
+            aligner += " -ax map-hifi -y -t {t} --secondary=no".format(t=threads)  # avoid -N1
+        else:
+            aligner += " -ax map-hifi -y -t {t} -N {N}".format(t=threads,
+                                                               N=num_sencondary)
+    elif is_bwa:
+        aligner = bwa_exec
+        if path_to_bwa is not None:
+            aligner = os.path.abspath(path_to_bwa)
+        aligner += " mem -x pacbio -C -V -t {t}".format(t=threads)
+    else:
+        if path_to_pbmm2 is not None:
+            aligner = os.path.abspath(path_to_pbmm2)
+        aligner += " align --preset HIFI -j {t} --sort ".format(t=threads)
+    return aligner
+
+
+def align_hifi_reads_to_genome(args):
+    sys.stderr.write("[align_hifi_reads]start..\n")
+    start = time.time()
+    inputpath = check_input_file(args.hifireads)
+    outputpath = check_output_file(args.output, inputpath, args.minimap2, args.bwa)
+    reference = os.path.abspath(args.ref)
+
+    if not os.path.exists(inputpath):
+        raise IOError("input file does not exist!")
+    if not os.path.exists(reference):
+        raise IOError("refernce(--ref) file does not exist!")
+
+    aligner = generate_aligner_with_options(args.minimap2,
+                                            args.path_to_minimap2,
+                                            args.bwa,
+                                            args.path_to_bwa,
+                                            args.path_to_pbmm2,
+                                            args.bestn,
+                                            args.threads)
+    samtools_view = generate_samtools_view_cmd(args.path_to_samtools, args.threads // 2)
+    samtools_index = generate_samtools_index_cmd(args.path_to_samtools, args.threads)
+
+    if (not args.minimap2) and (not args.bwa):
+        if outputpath.endswith(".bam"):
+            align_cmds = " ".join([aligner, reference, inputpath, outputpath])
+            post_align_cmd = " ".join([samtools_index, outputpath])
+            align_cmds = " && ".join([align_cmds, post_align_cmd])
+        elif outputpath.endswith(".sam"):
+            align_cmds = " ".join([aligner, reference, inputpath])
+            post_align_cmds = " ".join([samtools_view, "- >", outputpath])
+            align_cmds = " | ".join([align_cmds, post_align_cmds])
+        else:
+            raise ValueError("--output/-o must be in bam/sam format!")
+    else:
+        align_cmds = " ".join([aligner, reference, "-"])
+        if inputpath.endswith(".fq") or inputpath.endswith(".fastq"):
+            align_cmds = " ".join([aligner, reference, inputpath])
+        if outputpath.endswith(".sam"):
+            align_cmds += " > {}".format(outputpath)
+
+        pre_align_cmds = ""
+        if inputpath.endswith(".fq") or inputpath.endswith(".fastq"):
+            # pre_align_cmds += " ".join(["cat", inputpath])
+            pass
+        else:
+            if inputpath.endswith(".bam"):
+                pre_align_cmds += " ".join([samtools_view, inputpath])
+                pre_align_cmds += " | " + sam2fq_exec
+            elif inputpath.endswith(".sam"):
+                # pre_align_cmds += " ".join(["cat", inputpath])
+                pre_align_cmds += sam2fq_exec + " < " + inputpath
+            else:
+                raise ValueError()
+
+        post_align_cmds = ""
+        if outputpath.endswith(".bam"):
+            samtools_sort = generate_samtools_sort_cmd(args.path_to_samtools, outputpath, args.threads // 2)
+            post_align_cmds = " ".join([samtools_view, "-b |",
+                                        samtools_sort, "- &&",
+                                        samtools_index, outputpath])
+        elif outputpath.endswith(".sam"):
+            pass
+
+        if pre_align_cmds != "":
+            align_cmds = " | ".join([pre_align_cmds, align_cmds])
+        if post_align_cmds != "":
+            align_cmds = " | ".join([align_cmds, post_align_cmds])
+
+    sys.stderr.write("cmds: {}\n".format(align_cmds))
+    stdinfo, returncode = run_cmd(align_cmds)
+    stdout, stderr = stdinfo
+    if returncode:
+        sys.stderr.write("failed..\n")
+    else:
+        sys.stderr.write("succeeded..\n")
+    sys.stderr.write("==stdout:\n{}\n".format(str(stdout, 'utf-8')))
+    sys.stderr.write("==stderr:\n{}\n".format(str(stderr, 'utf-8')))
+
+    endtime = time.time()
+    sys.stderr.write("[align_hifi_reads]costs {:.1f} seconds\n".format(endtime - start))
+
+
+def main():
+    parser = argparse.ArgumentParser("align hifi reads using pbmm2/minimap2/bwa, default pbmm2")
+    p_input = parser.add_argument_group("INPUT")
+    p_input.add_argument("--hifireads", "-i", type=str, required=True,
+                         help="path to hifireads.bam/sam/fastq_with_pulseinfo file as input")
+    p_input.add_argument("--ref", type=str, required=True,
+                         help="path to genome reference to be aligned, in fasta/fa format. "
+                              "If using bwa, the reference must have already been indexed.")
+
+    p_output = parser.add_argument_group("OUTPUT")
+    p_output.add_argument("--output", "-o", type=str, required=False,
+                          help="output file path for alignment results, bam/sam supported. "
+                               "If not specified, the results will be saved in "
+                               "input_file_prefix.bam by default.")
+    p_output.add_argument("--header", action="store_true", default=False, required=False,
+                          help="save header annotations from bam/sam. DEPRECATED")
+
+    p_align = parser.add_argument_group("ALIGN")
+    p_align.add_argument("--path_to_pbmm2", type=str, default=None, required=False,
+                         help="full path to the executable binary pbmm2 file. "
+                              "If not specified, it is assumed that pbmm2 is "
+                              "in the PATH.")
+    p_align.add_argument("--minimap2", action="store_true", default=False, required=False,
+                         help="use minimap2 instead of pbmm2 for alignment")
+    p_align.add_argument("--path_to_minimap2", type=str, default=None, required=False,
+                         help="full path to the executable binary minimap2 file. "
+                              "If not specified, it is assumed that minimap2 is "
+                              "in the PATH.")
+    p_align.add_argument("--bestn", "-n", type=int, default=3, required=False,
+                         help="retain at most n alignments in minimap2. "
+                              "default 3, which means 2 secondary alignments are retained. "
+                              "Do not use 2, cause -N1 is not suggested for high accuracy of alignment. "
+                              "[This arg is for further extension.]")
+    p_align.add_argument("--bwa", action="store_true", default=False, required=False,
+                         help="use bwa instead of pbmm2 for alignment")
+    p_align.add_argument("--path_to_bwa", type=str, default=None, required=False,
+                         help="full path to the executable binary bwa file. If not "
+                              "specified, it is assumed that bwa is in the PATH.")
+    p_align.add_argument("--path_to_samtools", type=str, default=None, required=False,
+                         help="full path to the executable binary samtools file. "
+                              "If not specified, it is assumed that samtools is in "
+                              "the PATH.")
+    p_align.add_argument("--threads", "-t", type=int, default=5, required=False,
+                         help="number of threads, default 5")
+
+    args = parser.parse_args()
+
+    display_args(args, True)
+    align_hifi_reads_to_genome(args)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `ccsmeth-0.3.4/ccsmeth/call_modifications.py` & `ccsmeth-0.4.0/ccsmeth/call_modifications.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,222 +6,172 @@
 
 import argparse
 import os
 import sys
 
 import numpy as np
 import torch
+# import threading
 import torch.multiprocessing as mp
-from sklearn import metrics
-
-import gzip
 
 try:
     mp.set_start_method('spawn')
 except RuntimeError:
     pass
 except AttributeError:
     pass
 
 # from utils.process_utils import Queue
 from torch.multiprocessing import Queue
 import time
-# import random
 
-from tqdm import tqdm
+import pysam
+
+from collections import OrderedDict
 
 from .models import ModelAttRNN
 
 from .utils.process_utils import base2code_dna
-from .utils.process_utils import code2base_dna
 from .utils.process_utils import display_args
 from .utils.process_utils import nproc_to_call_mods_in_cpu_mode
 from .utils.process_utils import str2bool
 from .utils.process_utils import get_motif_seqs
 from .utils.process_utils import index_bam_if_needed2
+from .utils.process_utils import max_queue_size
+from .utils.process_utils import complement_seq
 
 from .utils.ref_reader import DNAReference
 
 from .utils.constants_torch import FloatTensor
 from .utils.constants_torch import use_cuda
 
 from .extract_features import worker_read_split_holebatches_to_queue
-from .extract_features import worker_extract_features_from_holebatches
+from .extract_features import process_one_holebatch
 from .extract_features import _get_holes
+from .extract_features import _open_inputfile
+
+from ._bam2modbam import _get_necessary_alignment_items
+from ._bam2modbam import _convert_locs_to_mmtag
+from ._bam2modbam import _convert_probs_to_mltag
+from ._bam2modbam import _refill_tags
+
+from ._version import VERSION
 
 # add this export temporarily
 # https://github.com/pytorch/pytorch/issues/37377
 os.environ['MKL_THREADING_LAYER'] = 'GNU'
 
-queue_size_border = 1000
-time_wait = 1
+# queue_size_border = max_queue_size
+time_wait = 0.2
 
 
-# read features from feature file ==============================================
-def _count_holenum(features_file):
-    h_num = 0
-    preholeid = None
-    if features_file.endswith(".gz"):
-        infile = gzip.open(features_file, 'rt')
-    else:
-        infile = open(features_file, 'r')
-    for line in infile:
-        words = line.strip().split("\t")
-        holeid = words[3]
-        if preholeid is None:
-            preholeid = holeid
-        elif preholeid != holeid:
-            preholeid = holeid
-            h_num += 1
-    h_num += 1
-    infile.close()
-    return h_num
-
-
-def _read_features_file_to_str(features_file, featurestrs_batch_q, holes_batch=50):
-    print("read_features process-{} starts".format(os.getpid()))
-    h_num_total = _count_holenum(features_file)
-    hbatch_num = h_num_total // holes_batch
-    if h_num_total % holes_batch > 0:
-        hbatch_num += 1
-    print("read_features process-{} - generate {} hole/read batches({})\n".format(os.getpid(),
-                                                                                  hbatch_num,
-                                                                                  holes_batch))
-
-    h_num = 0
-    hbatch_num_got = 0
-    preholeid = None
-    if features_file.endswith(".gz"):
-        infile = gzip.open(features_file, 'rt')
+# extract features ======================================================
+def _batch_feature_list2s(feature_list):
+    sampleinfo = []  # contains: chrom, abs_loc, strand, holeid, loc
+
+    fkmers = []
+    fpasss = []
+    fipdms = []
+    fipdsds = []
+    fpwms = []
+    fpwsds = []
+    fquals = []
+    fmaps = []
+
+    rkmers = []
+    rpasss = []
+    ripdms = []
+    ripdsds = []
+    rpwms = []
+    rpwsds = []
+    rquals = []
+    rmaps = []
+
+    labels = []
+    for featureline in feature_list:
+        chrom, abs_loc, strand, holeid, loc, \
+            kmer_seq, kmer_pass, kmer_ipdm, kmer_ipds, kmer_pwm, kmer_pws, kmer_qual, kmer_map, \
+            kmer_seq2, kmer_pass2, kmer_ipdm2, kmer_ipds2, kmer_pwm2, kmer_pws2, kmer_qual2, kmer_map2, \
+            label = featureline
+
+        sampleinfo.append("\t".join(list(map(str, [chrom, abs_loc, strand, holeid, loc]))))
+
+        fkmers.append(np.array([base2code_dna[x] for x in kmer_seq]))
+        fpasss.append(np.array([kmer_pass] * len(kmer_seq)))
+        fipdms.append(np.array(kmer_ipdm, dtype=float))
+        fipdsds.append(np.array(kmer_ipds, dtype=float) if type(kmer_ipds) is not str else 0)
+        fpwms.append(np.array(kmer_pwm, dtype=float))
+        fpwsds.append(np.array(kmer_pws, dtype=float) if type(kmer_pws) is not str else 0)
+        fquals.append(np.array(kmer_qual, dtype=float))
+        fmaps.append(np.array(kmer_map, dtype=float) if type(kmer_map) is not str else 0)
+
+        rkmers.append(np.array([base2code_dna[x] for x in kmer_seq2]))
+        rpasss.append(np.array([kmer_pass2] * len(kmer_seq2)))
+        ripdms.append(np.array(kmer_ipdm2, dtype=float))
+        ripdsds.append(np.array(kmer_ipds2, dtype=float) if type(kmer_ipds2) is not str else 0)
+        rpwms.append(np.array(kmer_pwm2, dtype=float))
+        rpwsds.append(np.array(kmer_pws2, dtype=float) if type(kmer_pws2) is not str else 0)
+        rquals.append(np.array(kmer_qual2, dtype=float))
+        rmaps.append(np.array(kmer_map2, dtype=float) if type(kmer_map2) is not str else 0)
+
+        labels.append(label)
+    return sampleinfo, fkmers, fpasss, fipdms, fipdsds, fpwms, fpwsds, fquals, fmaps, \
+        rkmers, rpasss, ripdms, ripdsds, rpwms, rpwsds, rquals, rmaps, labels
+
+
+def worker_extract_features_with_holeinfo(input_header, holebatch_q, features_q,
+                                          motifs, holeids_e, holeids_ne, dnacontigs, args):
+    sys.stderr.write("extract_features process-{} starts\n".format(os.getpid()))
+
+    if isinstance(input_header, OrderedDict) or isinstance(input_header, dict):
+        input_header2 = pysam.AlignmentHeader.from_dict(input_header)
     else:
-        infile = open(features_file, 'r')
-    featurestrs = []
-    with tqdm(total=hbatch_num,
-              desc="batch_reader") as pbar:
-        for line in infile:
-            words = line.strip().split("\t")
-            holeid = words[3]
-            if preholeid is None:
-                preholeid = holeid
-            elif preholeid != holeid:
-                preholeid = holeid
-                h_num += 1
-                if h_num % holes_batch == 0:
-                    featurestrs_batch_q.put(featurestrs)
-                    while featurestrs_batch_q.qsize() > queue_size_border:
-                        time.sleep(time_wait)
-                    featurestrs = []
-                    pbar.update(1)
-                    hbatch_num_got += 1
-            featurestrs.append(words)
-        infile.close()
-        h_num += 1
-        if len(featurestrs) > 0:
-            featurestrs_batch_q.put(featurestrs)
-            pbar.update(1)
-            hbatch_num_got += 1
-        assert hbatch_num_got == hbatch_num
-    featurestrs_batch_q.put("kill")
-    print("read_features process-{} ending, read {} reads/holes batches({})".format(os.getpid(),
-                                                                                    hbatch_num_got,
-                                                                                    holes_batch))
-
-
-def _format_features_from_strbatch2s(featurestrs_batch_q, features_batch_q, seq_len,
-                                     holeids_e, holeids_ne):
-    print("format_features process-{} starts".format(os.getpid()))
-    b_num = 0
+        input_header2 = input_header
+
+    cnt_holesbatch = 0
+    total_num_batch, failed_num_batch = 0, 0
     while True:
-        if featurestrs_batch_q.empty():
+        if holebatch_q.empty():
             time.sleep(time_wait)
             continue
-        featurestrs = featurestrs_batch_q.get()
-        if featurestrs == "kill":
-            featurestrs_batch_q.put("kill")
+        holebatch = holebatch_q.get()
+        if holebatch == "kill":
+            holebatch_q.put("kill")
             break
-        b_num += 1
-
-        sampleinfo = []  # contains: chrom, abs_loc, strand, holeid, loc
-
-        fkmers = []
-        fpasss = []
-        fipdms = []
-        fipdsds = []
-        fpwms = []
-        fpwsds = []
-        fquals = []
-        fmaps = []
-
-        rkmers = []
-        rpasss = []
-        ripdms = []
-        ripdsds = []
-        rpwms = []
-        rpwsds = []
-        rquals = []
-        rmaps = []
-
-        labels = []
-
-        if len(featurestrs) < 1:
-            continue
-        oriklen = len(featurestrs[0][5])
-        if oriklen == seq_len:
-            left_cut = 0
-            right_cut = -oriklen
-        elif oriklen > seq_len:
-            left_cut = right_cut = (oriklen - seq_len) // 2
-        else:
-            continue
-        for words in featurestrs:
-            holeid = words[3]
-            if holeids_e is not None and holeid not in holeids_e:
-                continue
-            if holeids_ne is not None and holeid in holeids_ne:
-                continue
-
-            sampleinfo.append("\t".join(words[0:5]))
-
-            fkmer = [base2code_dna[x] for x in words[5][left_cut:-right_cut]]
-            fkmers.append(fkmer)
-            fpasss.append([int(words[6])] * len(fkmer))
-            fipdms.append([float(x) for x in words[7].split(",")[left_cut:-right_cut]])
-            fipdsds.append([float(x) for x in words[8].split(",")[left_cut:-right_cut]] if words[8] != "." else 0)
-            fpwms.append([float(x) for x in words[9].split(",")[left_cut:-right_cut]])
-            fpwsds.append([float(x) for x in words[10].split(",")[left_cut:-right_cut]] if words[10] != "." else 0)
-            fquals.append([float(x) for x in words[11].split(",")[left_cut:-right_cut]])
-            fmaps.append([float(x) for x in words[12].split(",")[left_cut:-right_cut]] if words[12] != "." else 0)
-
-            rkmer = [base2code_dna[x] for x in words[13][left_cut:-right_cut]]
-            rkmers.append(rkmer)
-            rpasss.append([int(words[14])] * len(rkmer))
-            ripdms.append([float(x) for x in words[15].split(",")[left_cut:-right_cut]])
-            ripdsds.append([float(x) for x in words[16].split(",")[left_cut:-right_cut]] if words[16] != "." else 0)
-            rpwms.append([float(x) for x in words[17].split(",")[left_cut:-right_cut]])
-            rpwsds.append([float(x) for x in words[18].split(",")[left_cut:-right_cut]] if words[18] != "." else 0)
-            rquals.append([float(x) for x in words[19].split(",")[left_cut:-right_cut]])
-            rmaps.append([float(x) for x in words[20].split(",")[left_cut:-right_cut]] if words[20] != "." else 0)
-
-            labels.append(int(words[21]))
-
-        features_batch_q.put((sampleinfo, fkmers, fpasss, fipdms, fipdsds, fpwms, fpwsds, fquals, fmaps,
-                              rkmers, rpasss, ripdms, ripdsds, rpwms, rpwsds, rquals, rmaps, labels))
-        while features_batch_q.qsize() > queue_size_border:
-            time.sleep(time_wait)
-    print("format_features process-{} ending, read {} batches".format(os.getpid(), b_num))
+        # handle one holebatch
+        holeidxes, feature_list, total_num, failed_num = process_one_holebatch(input_header2, holebatch,
+                                                                               motifs, holeids_e, holeids_ne,
+                                                                               dnacontigs,
+                                                                               args)
+        total_num_batch += total_num
+        failed_num_batch += failed_num
+        if len(feature_list) > 0:
+            feature_batch = _batch_feature_list2s(feature_list)
+            features_oneholebatch = (holebatch, holeidxes, feature_batch)
+            features_q.put(features_oneholebatch)
+            # while features_q.qsize() > queue_size_border:
+            while features_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
+                time.sleep(time_wait)
+        cnt_holesbatch += 1
+    sys.stderr.write("extract_features process-{} ending, proceed {} "
+                     "hole_batches({}): {} holes/reads in total, "
+                     "{} skipped/failed.\n".format(os.getpid(),
+                                                   cnt_holesbatch,
+                                                   args.holes_batch,
+                                                   total_num_batch,
+                                                   failed_num_batch))
 
 
 # call mods =============================================================
 def _call_mods2s(features_batch, model, batch_size, device=0):
     sampleinfo, fkmers, fpasss, fipdms, fipdsds, fpwms, fpwsds, fquals, fmaps, \
         rkmers, rpasss, ripdms, ripdsds, rpwms, rpwsds, rquals, rmaps, labels = features_batch
     labels = np.reshape(labels, (len(labels)))
 
-    pred_str = []
-    accuracys = []
+    pred_info = []
     batch_num = 0
     for i in np.arange(0, len(sampleinfo), batch_size):
         batch_s, batch_e = i, i + batch_size
         b_sampleinfo = sampleinfo[batch_s:batch_e]
 
         b_fkmers = np.array(fkmers[batch_s:batch_e])
         b_fpasss = np.array(fpasss[batch_s:batch_e])
@@ -237,56 +187,129 @@
         b_ripdms = np.array(ripdms[batch_s:batch_e])
         b_ripdsds = np.array(ripdsds[batch_s:batch_e])
         b_rpwms = np.array(rpwms[batch_s:batch_e])
         b_rpwsds = np.array(rpwsds[batch_s:batch_e])
         b_rquals = np.array(rquals[batch_s:batch_e])
         b_rmaps = np.array(rmaps[batch_s:batch_e])
 
-        b_labels = np.array(labels[batch_s:batch_e])
+        # b_labels = np.array(labels[batch_s:batch_e])
         if len(b_sampleinfo) > 0:
             voutputs, vlogits = model(FloatTensor(b_fkmers, device), FloatTensor(b_fpasss, device),
                                       FloatTensor(b_fipdms, device), FloatTensor(b_fipdsds, device),
                                       FloatTensor(b_fpwms, device), FloatTensor(b_fpwsds, device),
                                       FloatTensor(b_fquals, device), FloatTensor(b_fmaps, device),
                                       FloatTensor(b_rkmers, device), FloatTensor(b_rpasss, device),
                                       FloatTensor(b_ripdms, device), FloatTensor(b_ripdsds, device),
                                       FloatTensor(b_rpwms, device), FloatTensor(b_rpwsds, device),
                                       FloatTensor(b_rquals, device), FloatTensor(b_rmaps, device))
             _, vpredicted = torch.max(vlogits.data, 1)
             if use_cuda:
                 vlogits = vlogits.cpu()
                 vpredicted = vpredicted.cpu()
 
-            predicted = vpredicted.numpy()
+            # predicted = vpredicted.numpy()
             logits = vlogits.data.numpy()
 
-            acc_batch = metrics.accuracy_score(
-                y_true=b_labels, y_pred=predicted)
-            accuracys.append(acc_batch)
-
             for idx in range(len(b_sampleinfo)):
                 # chromosome, pos, strand, holeid, loc, depth, prob_0, prob_1, called_label, seq
+                b_sampleinfo[idx] = b_sampleinfo[idx].split("\t")
+                holeid = b_sampleinfo[idx][3]
+                loc = int(b_sampleinfo[idx][4])
                 prob_0, prob_1 = logits[idx][0], logits[idx][1]
-                prob_0_norm = round(prob_0 / (prob_0 + prob_1), 6)
-                prob_1_norm = round(1 - prob_0_norm, 6)
-                b_idx_kmer = ''.join([code2base_dna[x] for x in b_fkmers[idx]])
-                center_idx = int(np.floor(len(b_idx_kmer)/2))
-                bkmer_start = center_idx - 2 if center_idx - 2 >= 0 else 0
-                bkmer_end = center_idx + 3 if center_idx + 3 <= len(b_idx_kmer) else len(b_idx_kmer)
-                pred_str.append("\t".join([b_sampleinfo[idx],
-                                           str(b_fpasss[idx][0]) + "," + str(b_rpasss[idx][0]),
-                                           str(prob_0_norm), str(prob_1_norm), str(predicted[idx]),
-                                           b_idx_kmer[bkmer_start:bkmer_end]]))
+                prob_1_norm = round(prob_1 / (prob_0 + prob_1), 6)
+                pred_info.append((holeid, loc, prob_1_norm))
             batch_num += 1
-    accuracy = np.mean(accuracys) if len(accuracys) > 0 else 0.
 
-    return pred_str, accuracy, batch_num
+    return pred_info, batch_num
+
+
+def _add_modinfo2alignedseg(read_info, pred_info, input_header, rm_pulse):
+    segment_tmp = pysam.AlignedSegment.from_dict(read_info, input_header)
+
+    seq_name, flag, ref_name, ref_start, mapq, cigartuples, rnext, pnext, \
+        tlen, seq_seq, seq_qual, all_tags, is_reverse = _get_necessary_alignment_items(segment_tmp)
+
+    # MM: Base modifications / methylation, ML:Base modification probabilities tags
+    mm_values = ml_values = None
+    mm_flag = 0
+    if len(pred_info) == 0:
+        new_tags = _refill_tags(all_tags, mm_values, ml_values, rm_pulse)
+        return (seq_name, flag, ref_name, ref_start, mapq, cigartuples, rnext, pnext, tlen,
+                seq_seq, seq_qual, new_tags, mm_flag)
+    
+    seq_fwdseq = complement_seq(seq_seq) if is_reverse else seq_seq
+    locs_probs = []
+    for pred in pred_info:
+        holeid_tmp, loc_tmp, prob_tmp = pred
+        if holeid_tmp == seq_name:
+            locs_probs.append((loc_tmp, prob_tmp))
+        else:
+            raise ValueError("holeid_tmp != seq_name, {} != {}".format(holeid_tmp, seq_name))
+    try:
+        locs_probs = sorted(locs_probs, key=lambda x: x[0])
+        locs_probs = list(zip(*locs_probs))
+        locs = locs_probs[0]
+        probs = locs_probs[1]
+        mm_values = _convert_locs_to_mmtag(locs, seq_fwdseq)
+        ml_values = _convert_probs_to_mltag(probs)
+        mm_flag = 1
+    except AssertionError:
+        # sys.stderr.write("AssertionError, skip this alignment.\n"
+        #       "\tDetails: {}, {}, {}\n".format(seq_name, locs, probs))
+        sys.stderr.write("AssertionError, skip this alignment-{}.\n".format(seq_name))
+    new_tags = _refill_tags(all_tags, mm_values, ml_values, rm_pulse)
+    return (seq_name, flag, ref_name, ref_start, mapq, cigartuples, rnext, pnext, tlen,
+            seq_seq, seq_qual, new_tags, mm_flag)
+
+
+def _add_modinfo2alignedseg_batch(holebatch, holeidxes, preds_info, input_header, rm_pulse):
+    new_read_infos = []
+
+    def catch_up(holebatch_cnt, cur_holeid):
+        while holebatch_cnt < cur_holeid:
+            new_read_info = _add_modinfo2alignedseg(holebatch[holebatch_cnt], [], input_header, rm_pulse)
+            new_read_infos.append(new_read_info)
+            holebatch_cnt += 1
+        return holebatch_cnt
+    
+    if len(holeidxes) == 0:
+        for idx, read_info in enumerate(holebatch):
+            new_read_info = _add_modinfo2alignedseg(read_info, [], input_header, rm_pulse)
+            new_read_infos.append(new_read_info)
+        return new_read_infos
+
+    assert len(holeidxes) == len(preds_info)
+    holebatch_cnt = 0
+    pred_info_tmp = []
+    cur_holeid = holeidxes[0]
+    for idx, holeid in enumerate(holeidxes):
+        if holeid != cur_holeid:
+            holebatch_cnt = catch_up(holebatch_cnt, cur_holeid)
+            assert holebatch_cnt == cur_holeid
+            new_read_info = _add_modinfo2alignedseg(holebatch[holebatch_cnt], pred_info_tmp, input_header, rm_pulse)
+            new_read_infos.append(new_read_info)
+            pred_info_tmp = []
+            holebatch_cnt += 1
+            cur_holeid = holeid
+        pred_info_tmp.append(preds_info[idx])
+    # last pred_info
+    holebatch_cnt = catch_up(holebatch_cnt, cur_holeid)
+    assert holebatch_cnt == cur_holeid
+    new_read_info = _add_modinfo2alignedseg(holebatch[holebatch_cnt], pred_info_tmp, input_header, rm_pulse)
+    new_read_infos.append(new_read_info)
+    # last holebatches
+    if holebatch_cnt < len(holebatch) - 1:
+        for idx in range(holebatch_cnt + 1, len(holebatch)):
+            new_read_info = _add_modinfo2alignedseg(holebatch[idx], [], input_header, rm_pulse)
+            new_read_infos.append(new_read_info)
+    assert len(holebatch) == len(new_read_infos)
+    return new_read_infos
 
 
-def _call_mods_q(model_path, features_batch_q, pred_str_q, args, device=0):
+def _call_mods_q(model_path, features_batch_q, out_info_q, input_header, args, device=0):
     print('call_mods process-{} starts'.format(os.getpid()))
     if args.model_type in {"attbigru2s", "attbilstm2s"}:
         model = ModelAttRNN(args.seq_len, args.layer_rnn, args.class_num,
                             args.dropout_rate, args.hid_rnn,
                             args.n_vocab, args.n_embed,
                             is_qual=str2bool(args.is_qual),
                             is_map=str2bool(args.is_map),
@@ -304,81 +327,121 @@
         model_dict.update(para_dict)
         model.load_state_dict(model_dict)
         if str2bool(args.loginfo):
             print('call_mods process-{} loads model param successfully'.format(os.getpid()))
         del model_dict
     except RuntimeError:
         # for DDP model convertion (key: module.embed.weight -> embed.weight)
-        from collections import OrderedDict
         para_dict = torch.load(model_path, map_location=torch.device('cpu'))
         para_dict_new = OrderedDict()
         for param_tensor in para_dict.keys():
             para_dict_new[param_tensor[7:]] = para_dict[param_tensor]
         model.load_state_dict(para_dict_new)
         if str2bool(args.loginfo):
             print('call_mods process-{} loads model param successfully-1'.format(os.getpid()))
         del para_dict_new
     sys.stdout.flush()
 
     if use_cuda:
         model = model.cuda(device)
     model.eval()
 
-    accuracy_list = []
+    if isinstance(input_header, OrderedDict) or isinstance(input_header, dict):
+        input_header2 = pysam.AlignmentHeader.from_dict(input_header)
+    else:
+        input_header2 = input_header
+    rm_pulse = not args.keep_pulse
+    
     batch_num_total = 0
     while True:
 
         if features_batch_q.empty():
             time.sleep(time_wait)
             continue
 
         features_batch = features_batch_q.get()
         if features_batch == "kill":
             features_batch_q.put("kill")
             break
 
+        holebatch, holeidxes, features_oneholebatch = features_batch
         if args.model_type in {"attbigru2s", "attbilstm2s"}:
-            pred_str, accuracy, batch_num = _call_mods2s(features_batch, model, args.batch_size, device)
+            pred_info, batch_num = _call_mods2s(features_oneholebatch, model, args.batch_size, device)
+            del features_oneholebatch
         else:
             raise ValueError("--model_type not right!")
-
-        pred_str_q.put(pred_str)
-        while pred_str_q.qsize() > queue_size_border:
+        
+        new_read_infos = _add_modinfo2alignedseg_batch(holebatch, holeidxes, pred_info, input_header2, rm_pulse)
+        out_info_q.put(new_read_infos)
+        # while out_info_q.qsize() > queue_size_border:
+        while out_info_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
             time.sleep(time_wait)
         # for debug
         # print("call_mods process-{} reads 1 batch, features_batch_q:{}, "
-        #       "pred_str_q: {}".format(os.getpid(), features_batch_q.qsize(), pred_str_q.qsize()))
-        accuracy_list.append(accuracy)
+        #       "pred_info_q: {}".format(os.getpid(), features_batch_q.qsize(), pred_info_q.qsize()))
         batch_num_total += batch_num
-    # print('total accuracy in process {}: {}'.format(os.getpid(), np.mean(accuracy_list)))
     print('call_mods process-{} ending, proceed {} batches({})'.format(os.getpid(), batch_num_total,
                                                                        args.batch_size))
 
 
-def _write_predstr_to_file(write_fp, predstr_q, is_gzip):
-    print('write_process-{} starts'.format(os.getpid()))
-    if is_gzip:
-        if not write_fp.endswith(".gz"):
-            write_fp += ".gz"
-        wf = gzip.open(write_fp, "wt")
+# write modbam =============================================================
+def write_alignedsegment(readitem_info, output_bam):
+    """
+    Writes the readitem_info(tuple) to a bam file
+    :param readitem_info:
+    :param output_bam:
+    :return:
+    """
+    seq_name, flag, ref_name, ref_start, mapq, cigartuples, \
+        rnext, pnext, tlen, seq_seq, seq_qual, all_tags, _ = readitem_info
+
+    out_read = pysam.AlignedSegment(output_bam.header)
+    out_read.query_name = seq_name
+    out_read.flag = flag
+    out_read.reference_name = ref_name
+    out_read.reference_start = ref_start
+    out_read.mapping_quality = mapq
+    out_read.cigar = cigartuples
+    out_read.next_reference_name = rnext
+    out_read.next_reference_start = pnext
+    out_read.template_length = tlen
+    out_read.query_sequence = seq_seq
+    out_read.query_qualities = seq_qual
+    if len(all_tags) >= 1:
+        out_read.set_tags(all_tags)
+    output_bam.write(out_read)
+
+
+def _worker_write_modbam(wreads_q, modbamfile, inputheader, threads=1):
+    if not (isinstance(inputheader, OrderedDict) or isinstance(inputheader, dict)):
+        header2 = inputheader.to_dict()
     else:
-        wf = open(write_fp, 'w')
+        from copy import deepcopy
+        header2 = deepcopy(inputheader)
+    # try adding PG tag here
+    # MUST have the ID entry
+    header2["PG"].append({"PN": "ccsmeth", "ID": "ccsmeth", "VN": VERSION, "CL": " ".join(sys.argv)})
+
+    w_bam = pysam.AlignmentFile(modbamfile, "wb", header=header2, threads=threads)
+    cnt_w, cnt_mm = 0, 0
     while True:
-        # during test, it's ok without the sleep()
-        if predstr_q.empty():
+        if wreads_q.empty():
             time.sleep(time_wait)
             continue
-        pred_str = predstr_q.get()
-        if pred_str == "kill":
-            wf.close()
-            print('write_process-{} finished'.format(os.getpid()))
+        wreads_batch = wreads_q.get()
+        if wreads_batch == "kill":
+            w_bam.close()
+            sys.stderr.write("wrote {} reads, in which {} were added mm tags\n".format(cnt_w,
+                                                                                       cnt_mm))
             break
-        for one_pred_str in pred_str:
-            wf.write(one_pred_str + "\n")
-        wf.flush()
+        for walignseg in wreads_batch:
+            mm_flag = walignseg[-1]
+            write_alignedsegment(walignseg, w_bam)
+            cnt_w += 1
+            cnt_mm += mm_flag
 
 
 def _get_gpus():
     num_gpus = torch.cuda.device_count()
     if num_gpus > 0:
         gpulist = list(range(num_gpus))
     else:
@@ -401,16 +464,16 @@
     input_path = os.path.abspath(args.input)
     if not os.path.exists(input_path):
         raise ValueError("--input_file does not exist!")
 
     out_dir = os.path.dirname(os.path.abspath(args.output))
     if not os.path.exists(out_dir):
         os.makedirs(out_dir)
-
-    out_per_readsite = args.output + ".per_readsite.tsv"
+    
+    out_modbam = args.output + ".modbam.bam"
 
     holeids_e = None if args.holeids_e is None else _get_holes(args.holeids_e)
     holeids_ne = None if args.holeids_ne is None else _get_holes(args.holeids_ne)
 
     if input_path.endswith(".bam") or input_path.endswith(".sam"):
         if args.seq_len % 2 == 0:
             raise ValueError("--seq_len must be odd")
@@ -430,147 +493,104 @@
                 raise IOError("refernce(--ref) file does not exist!")
             dnacontigs = DNAReference(reference).getcontigs()
 
         motifs = get_motif_seqs(args.motifs)
 
         hole_batch_q = Queue()
         features_batch_q = Queue()
-        pred_str_q = Queue()
+        out_info_q = Queue()
 
         nproc = args.threads
         nproc_dp = args.threads_call
         if use_cuda:
             if nproc_dp < 1:
                 nproc_dp = 1
         else:
             if nproc_dp > nproc_to_call_mods_in_cpu_mode:
                 nproc_dp = nproc_to_call_mods_in_cpu_mode
-        if nproc <= nproc_dp + 3:
-            print("--threads must be > --threads_call + 3!!")
-            nproc = nproc_dp + 3 + 1  # 2 for reading, 1 for writing, 1 for extracting
+        if nproc <= nproc_dp + 4:
+            print("--threads must be > --threads_call + 4!!")
+            nproc = nproc_dp + 4 + 1  # 2 for reading, 2 for writing, 1 for extracting
+            threads_r, threads_w = 2, 2
+        else:
+            threads_r = 2
+            if nproc - nproc_dp - threads_r >= 16:
+                threads_w = 4
+            elif nproc - nproc_dp - threads_r >= 12:
+                threads_w = 3
+            else:
+                threads_w = 2
+
+        inputreads = _open_inputfile(input_path, args.mode, threads=args.threads)
+        input_header = inputreads.header.to_dict()
+        inputreads.close()
 
-        # 2 threads/processes
         p_read = mp.Process(target=worker_read_split_holebatches_to_queue,
-                            args=(input_path, hole_batch_q, 2, args))
+                            args=(input_path, hole_batch_q, threads_r, args))
         p_read.daemon = True
         p_read.start()
 
-        # 1 processes
-        p_w = mp.Process(target=_write_predstr_to_file, args=(out_per_readsite, pred_str_q, args.gzip))
+        p_w = mp.Process(target=_worker_write_modbam, args=(out_info_q, out_modbam, input_header, threads_w))
         p_w.daemon = True
         p_w.start()
 
         # TODO: why the processes in ps_extract start so slowly?
         ps_extract = []
         ps_call = []
-        nproc_ext = nproc - nproc_dp - 3
+        nproc_ext = nproc - nproc_dp - threads_r - threads_w
         gpulist = _get_gpus()
         gpuindex = 0
         for i in range(max(nproc_ext, nproc_dp)):
             if i < nproc_ext:
-                p = mp.Process(target=worker_extract_features_from_holebatches,
-                               args=(hole_batch_q, features_batch_q,
-                                     motifs, holeids_e, holeids_ne, dnacontigs,
-                                     args, False, True))
+                p = mp.Process(target=worker_extract_features_with_holeinfo,
+                               args=(input_header, hole_batch_q, features_batch_q,
+                                     motifs, holeids_e, holeids_ne, dnacontigs, args))
                 p.daemon = True
                 p.start()
                 ps_extract.append(p)
             if i < nproc_dp:
-                p = mp.Process(target=_call_mods_q, args=(model_path, features_batch_q, pred_str_q,
-                                                          args, gpulist[gpuindex]))
+                p = mp.Process(target=_call_mods_q, args=(model_path, features_batch_q, out_info_q, 
+                                                          input_header, args, gpulist[gpuindex]))
                 gpuindex += 1
                 p.daemon = True
                 p.start()
                 ps_call.append(p)
-
+        
         p_read.join()
 
         for p in ps_extract:
             p.join()
         features_batch_q.put("kill")
 
         for p in ps_call:
             p.join()
-        pred_str_q.put("kill")
+        out_info_q.put("kill")
 
         p_w.join()
 
-        if str2bool(args.modbam):
-            from ._bam2modbam import add_mm_ml_tags_to_bam
-            out_modbam = args.output + ".modbam.bam"
-            add_mm_ml_tags_to_bam(input_path, out_per_readsite, out_modbam,
-                                  rm_pulse=True, threads=args.threads,
-                                  mode=args.mode)
-            if args.rm_per_readsite:
-                os.remove(out_per_readsite)
+        if not args.no_sort:
+            post_time_start = time.time()
+            print("[post_process] bam_sort_index starts..")
+            try:
+                sys.stderr.write("sorting modbam file..\n")
+                modbam_sorted = os.path.splitext(out_modbam)[0] + ".sorted.bam"
+                pysam.sort("-o", modbam_sorted, "-@", str(args.threads), out_modbam)
+                os.rename(modbam_sorted, out_modbam)
+            except Exception:
+                sys.stderr.write("failed sorting modbam file..\n")
+            try:
+                sys.stderr.write("indexing modbam file..\n")
+                pysam.index("-@", str(args.threads), out_modbam)
+            except Exception:
+                sys.stderr.write("failed indexing modbam file..\n")
+            print("[post_process] bam_sort_index costs %.2f seconds.." % (time.time() - post_time_start))
     else:
-        # features_batch_q = mp.Queue()
-        features_batch_q = Queue()
-        # pred_str_q = mp.Queue()
-        pred_str_q = Queue()
-        featurestrs_batch_q = Queue()
-
-        nproc = args.threads
-        nproc_dp = args.threads_call
-        if use_cuda:
-            if nproc_dp < 1:
-                nproc_dp = 1
-        else:
-            if nproc_dp > nproc_to_call_mods_in_cpu_mode:
-                nproc_dp = nproc_to_call_mods_in_cpu_mode
-        if nproc < nproc_dp + 2:
-            print("--threads must be > --threads_call + 2!!")
-            nproc = nproc_dp + 2 + 1  # 1 for reading, 1 for writing, 1 for extracting
-        nproc_cnvt = nproc - nproc_dp - 2
-
-        p_read = mp.Process(target=_read_features_file_to_str, args=(input_path, featurestrs_batch_q,
-                                                                     args.holes_batch))
-        p_read.daemon = True
-        p_read.start()
-
-        ps_str2value = []
-        if args.model_type in {"attbigru2s", "attbilstm2s"}:
-            for _ in range(nproc_cnvt):
-                p = mp.Process(target=_format_features_from_strbatch2s, args=(featurestrs_batch_q,
-                                                                              features_batch_q,
-                                                                              args.seq_len,
-                                                                              holeids_e, holeids_ne))
-                p.daemon = True
-                p.start()
-                ps_str2value.append(p)
-        else:
-            raise ValueError("--model_type not right!")
-
-        predstr_procs = []
-        gpulist = _get_gpus()
-        gpuindex = 0
-        for _ in range(nproc_dp):
-            p = mp.Process(target=_call_mods_q, args=(model_path, features_batch_q, pred_str_q,
-                                                      args, gpulist[gpuindex]))
-            gpuindex += 1
-            p.daemon = True
-            p.start()
-            predstr_procs.append(p)
-
-        # print("write_process started..")
-        p_w = mp.Process(target=_write_predstr_to_file, args=(out_per_readsite, pred_str_q, args.gzip))
-        p_w.daemon = True
-        p_w.start()
-
-        p_read.join()
-
-        for p in ps_str2value:
-            p.join()
-        features_batch_q.put("kill")
-
-        for p in predstr_procs:
-            p.join()
-        pred_str_q.put("kill")
-
-        p_w.join()
+        from ._call_modifications_txt import call_mods_txt
+        out_per_readsite = args.output + ".per_readsite.tsv"
+        call_mods_txt(input_path, holeids_e, holeids_ne, out_per_readsite, model_path, args)
 
     print("[main]call_mods costs %.2f seconds.." % (time.time() - start))
 
 
 def main():
     parser = argparse.ArgumentParser("call modifications")
 
@@ -578,19 +598,29 @@
     p_input.add_argument("--input", "-i", action="store", type=str,
                          required=True,
                          help="input file, can be bam/sam, or features.tsv generated by "
                               "extract_features.py.")
     p_input.add_argument("--holes_batch", type=int, default=50, required=False,
                          help="number of holes/hifi-reads in an batch to get/put in queues, default 50. "
                               "only used when --input is bam/sam")
+    
+    p_output = parser.add_argument_group("OUTPUT")
+    p_output.add_argument("--output", "-o", action="store", type=str, required=True,
+                          help="the prefix of output files to save the predicted results. "
+                               "output files will be [--output].per_readsite.tsv/.modbam.bam")
+    p_output.add_argument("--gzip", action="store_true", default=False, required=False,
+                          help="if compressing .per_readsite.tsv when --input is not in bam/sam format.")
+    p_output.add_argument("--keep_pulse", action="store_true", default=False, required=False,
+                          help="if keeping ipd/pw tags in .modbam.bam when --input is in bam/sam format.")
+    p_output.add_argument("--no_sort", action="store_true", default=False, required=False,
+                          help="don't sort .modbam.bam when --input is in bam/sam format.")
 
     p_call = parser.add_argument_group("CALL")
     p_call.add_argument("--model_file", "-m", action="store", type=str, required=True,
                         help="file path of the trained model (.ckpt)")
-
     # model param
     p_call.add_argument('--model_type', type=str, default="attbigru2s",
                         choices=["attbilstm2s", "attbigru2s"],
                         required=False,
                         help="type of model to use, 'attbilstm2s', 'attbigru2s', "
                              "default: attbigru2s")
     p_call.add_argument('--seq_len', type=int, default=21, required=False,
@@ -604,37 +634,24 @@
     p_call.add_argument('--is_stds', type=str, default="no", required=False,
                         help="if using std features, yes or no, default no")
     p_call.add_argument('--class_num', type=int, default=2, required=False)
     p_call.add_argument('--dropout_rate', type=float, default=0, required=False)
 
     p_call.add_argument("--batch_size", "-b", default=512, type=int, required=False,
                         action="store", help="batch size, default 512")
-
     # BiRNN model param
     p_call.add_argument('--n_vocab', type=int, default=16, required=False,
                         help="base_seq vocab_size (15 base kinds from iupac)")
     p_call.add_argument('--n_embed', type=int, default=4, required=False,
                         help="base_seq embedding_size")
     p_call.add_argument('--layer_rnn', type=int, default=3,
                         required=False, help="BiRNN layer num, default 3")
     p_call.add_argument('--hid_rnn', type=int, default=256, required=False,
                         help="BiRNN hidden_size, default 256")
 
-    p_output = parser.add_argument_group("OUTPUT")
-    p_output.add_argument("--output", "-o", action="store", type=str, required=True,
-                          help="the prefix of output files to save the predicted results. "
-                               "output files will be [--output].per_readsite.tsv/.modbam.bam")
-    p_output.add_argument("--gzip", action="store_true", default=False, required=False,
-                          help="if compressing .per_readsite.tsv using gzip")
-    p_output.add_argument("--modbam", type=str, default="yes", required=False,
-                          help="if generating modbam file when --input is in bam/sam format. "
-                               "yes or no, default yes")
-    p_output.add_argument("--rm_per_readsite", action="store_true", default=False, required=False,
-                          help="if rm per_readsite.tsv when --mobam is set to yes")
-
     p_extract = parser.add_argument_group("EXTRACTION")
     p_extract.add_argument("--mode", type=str, default="denovo", required=False,
                            choices=["denovo", "align"],
                            help="denovo mode: extract features from unaligned/aligned hifi.bam without "
                                 "reference position info;\n"
                                 "align mode: extract features from aligned hifi.bam with "
                                 "reference position info. default: denovo")
```

### Comparing `ccsmeth-0.3.4/ccsmeth/call_mods_freq_bam.py` & `ccsmeth-0.4.0/ccsmeth/call_mods_freq_bam.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     sys.stderr.write("worker_split_regions process-{} generates {} regions\n".format(os.getpid(),
                                                                                      len(ref_chunks)))
     with tqdm(total=len(ref_chunks),
               desc="region_reader") as pbar:
         for ref_chunk in ref_chunks:
             region_q.put(ref_chunk)
             pbar.update(1)
-            while region_q.qsize() > args.threads * 3:
+            while region_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
                 time.sleep(time_wait)
     region_q.put("kill")
 
 
 def _cal_mod_prob(ml_value):
     # WARN: if ori_prob exactly = 0.5, ml_value = floor(0.5*256) = 128
     # WARN: then if we use the following to convert ml_value to prob, the the new_prob = 0.5000001.
@@ -600,15 +600,15 @@
             region_q.put("kill")
             break
         cnt_regions += 1
         bed_all, bed_hp1, bed_hp2 = _readmods_to_bed_of_one_region(bam_reader, region,
                                                                    dnacontigs, motifs_filter, args)
         if len(bed_all) > 0:
             bed_q.put((bed_all, bed_hp1, bed_hp2))
-            while bed_q.qsize() > args.threads * 3:
+            while bed_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
                 time.sleep(time_wait)
 
     bam_reader.close()
     sys.stderr.write("worker_gen_bed process-{} ending, proceed {} regions\n".format(os.getpid(),
                                                                                      cnt_regions))
```

### Comparing `ccsmeth-0.3.4/ccsmeth/call_mods_freq_txt.py` & `ccsmeth-0.4.0/ccsmeth/call_mods_freq_txt.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,16 @@
             sitekey2stats[mod_record._site_key]._coverage += 1
             if mod_record._called_label == 1:
                 sitekey2stats[mod_record._site_key]._met += 1
             else:
                 sitekey2stats[mod_record._site_key]._unmet += 1
             used += 1
         infile.close()
+    if count == 0:
+        raise ValueError("No modification calls found in {}..".format(mods_files))
     if contig_name is None:
         print("{:.2f}% ({} of {}) calls used..".format(used/float(count) * 100, used, count))
     else:
         print("{:.2f}% ({} of {}) calls used for {}..".format(used / float(count) * 100, used, count, contig_name))
     return sitekey2stats
```

### Comparing `ccsmeth-0.3.4/ccsmeth/ccsmeth.py` & `ccsmeth-0.4.0/ccsmeth/ccsmeth.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,19 +203,29 @@
     scm_input.add_argument("--input", "-i", action="store", type=str,
                            required=True,
                            help="input file, can be bam/sam, or features.tsv generated by "
                                 "extract_features.py.")
     scm_input.add_argument("--holes_batch", type=int, default=50, required=False,
                            help="number of holes/hifi-reads in an batch to get/put in queues, default 50. "
                                 "only used when --input is bam/sam")
+    
+    scm_output = sub_call_mods.add_argument_group("OUTPUT")
+    scm_output.add_argument("--output", "-o", action="store", type=str, required=True,
+                            help="the prefix of output files to save the predicted results. "
+                                 "output files will be [--output].per_readsite.tsv/.modbam.bam")
+    scm_output.add_argument("--gzip", action="store_true", default=False, required=False,
+                            help="if compressing .per_readsite.tsv when --input is not in bam/sam format.")
+    scm_output.add_argument("--keep_pulse", action="store_true", default=False, required=False,
+                            help="if keeping ipd/pw tags in .modbam.bam when --input is in bam/sam format.")
+    scm_output.add_argument("--no_sort", action="store_true", default=False, required=False,
+                            help="don't sort .modbam.bam when --input is in bam/sam format.")
 
     scm_call = sub_call_mods.add_argument_group("CALL")
     scm_call.add_argument("--model_file", "-m", action="store", type=str, required=True,
                           help="file path of the trained model (.ckpt)")
-
     # model param
     scm_call.add_argument('--model_type', type=str, default="attbigru2s",
                           choices=["attbilstm2s", "attbigru2s"],
                           required=False,
                           help="type of model to use, 'attbilstm2s', 'attbigru2s', "
                                "default: attbigru2s")
     scm_call.add_argument('--seq_len', type=int, default=21, required=False,
@@ -229,37 +239,24 @@
     scm_call.add_argument('--is_stds', type=str, default="no", required=False,
                           help="if using std features, yes or no, default no")
     scm_call.add_argument('--class_num', type=int, default=2, required=False)
     scm_call.add_argument('--dropout_rate', type=float, default=0, required=False)
 
     scm_call.add_argument("--batch_size", "-b", default=512, type=int, required=False,
                           action="store", help="batch size, default 512")
-
     # BiRNN model param
     scm_call.add_argument('--n_vocab', type=int, default=16, required=False,
                           help="base_seq vocab_size (15 base kinds from iupac)")
     scm_call.add_argument('--n_embed', type=int, default=4, required=False,
                           help="base_seq embedding_size")
     scm_call.add_argument('--layer_rnn', type=int, default=3,
                           required=False, help="BiRNN layer num, default 3")
     scm_call.add_argument('--hid_rnn', type=int, default=256, required=False,
                           help="BiRNN hidden_size, default 256")
 
-    scm_output = sub_call_mods.add_argument_group("OUTPUT")
-    scm_output.add_argument("--output", "-o", action="store", type=str, required=True,
-                            help="the prefix of output files to save the predicted results. "
-                                 "output files will be [--output].per_readsite.tsv/.modbam.bam")
-    scm_output.add_argument("--gzip", action="store_true", default=False, required=False,
-                            help="if compressing .per_readsite.tsv using gzip")
-    scm_output.add_argument("--modbam", type=str, default="yes", required=False,
-                            help="if generating modbam file when --input is in bam/sam format. "
-                                 "yes or no, default yes")
-    scm_output.add_argument("--rm_per_readsite", action="store_true", default=False, required=False,
-                            help="if rm per_readsite.tsv when --mobam is set to yes")
-
     scm_extract = sub_call_mods.add_argument_group("EXTRACTION")
     scm_extract.add_argument("--mode", type=str, default="denovo", required=False,
                              choices=["denovo", "align"],
                              help="denovo mode: extract features from unaligned/aligned hifi.bam without "
                                   "reference position info;\n"
                                   "align mode: extract features from aligned hifi.bam with "
                                   "reference position info. default: denovo")
```

### Comparing `ccsmeth-0.3.4/ccsmeth/dataloader.py` & `ccsmeth-0.4.0/ccsmeth/dataloader.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/ccsmeth/extract_features.py` & `ccsmeth-0.4.0/ccsmeth/extract_features.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,37 +5,39 @@
 import numpy as np
 from statsmodels import robust
 import multiprocessing as mp
 from multiprocessing import Queue
 import gzip
 
 import pysam
+from collections import OrderedDict
 from tqdm import tqdm
 
 from .utils.process_utils import display_args
 from .utils.process_utils import codecv1_to_frame2
 from .utils.process_utils import get_refloc_of_methysite_in_motif
 from .utils.process_utils import get_motif_seqs
 from .utils.process_utils import complement_seq
 from .utils.process_utils import base2code_dna
 from .utils.process_utils import compute_pct_identity
 from .utils.process_utils import get_q2tloc_from_cigar
 from .utils.process_utils import str2bool
 from .utils.process_utils import index_bam_if_needed2
+from .utils.process_utils import max_queue_size
 
 # from .utils.process_utils import run_cmd
 # from .utils.process_utils import generate_samtools_index_cmd
 
 from .utils.ref_reader import DNAReference
 
 from .utils.process_utils import default_ref_loc
 
 code2frames = codecv1_to_frame2()
-queue_size_border = 1000
-time_wait = 1
+# queue_size_border = max_queue_size
+time_wait = 0.2
 
 
 # check and read some inputs =============================================
 def check_input_file(inputfile):
     if not (inputfile.endswith(".bam") or inputfile.endswith(".sam")):
         raise ValueError("--input/-i must be in bam/sam format!")
     inputpath = os.path.abspath(inputfile)
@@ -141,23 +143,24 @@
               desc="batch_reader") as pbar:
         inputreads = _open_inputfile(inputfile, args.mode, threads=threads)
         all_reads = inputreads.fetch(until_eof=True)
         count = 0
         count_batch = 0
         holebatchtmp = []
         for readitem in all_reads:
-            readinfo = _get_necessary_items_of_a_alignedsegment(readitem)
-            holebatchtmp.append(readinfo)
+            readinfo_dict = readitem.to_dict()
+            holebatchtmp.append(readinfo_dict)
             count += 1
             if count % args.holes_batch == 0 or count == totalnum:
                 holebatch_q.put(holebatchtmp)
                 pbar.update(1)
                 count_batch += 1
                 holebatchtmp = []
-                while holebatch_q.qsize() > queue_size_border:
+                # while holebatch_q.qsize() > queue_size_border:
+                while holebatch_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
                     time.sleep(time_wait)
         inputreads.close()
         if count_batch != len(holebatches):
             sys.stderr.write("[WARN]read {} batches while it should be {} batches!".format(count_batch,
                                                                                            len(holebatches)))
         if len(holebatchtmp) > 0:
             sys.stderr.write("[WARN]There are still holes/reads that do not belong any batches!")
@@ -239,19 +242,19 @@
     rkmer_map = np.flip(np.pad(q_to_r_mapinfo_s[offset_s:offset_e],
                                (pad_l, pad_r),
                                mode='constant', constant_values=1))
 
     return fkmer_map, rkmer_map
 
 
-def extract_features_from_double_strand_read(readinfo, motifs, holeids_e, holeids_ne, dnacontigs,
+def extract_features_from_double_strand_read(alignedsegment_tmp, motifs, holeids_e, holeids_ne, dnacontigs,
                                              args):
     seq_name, qalign_start, qalign_end, fwd_seq, fwd_qual, ref_name, ref_start, ref_end, \
         cigar_tuples, cigar_stats, flag, mapq, is_unmapped, is_secondary, is_duplicate, is_supplementary, \
-        is_reverse, tag_fi, tag_ri, tag_fp, tag_rp, tag_fn, tag_rn = readinfo
+        is_reverse, tag_fi, tag_ri, tag_fp, tag_rp, tag_fn, tag_rn = _get_necessary_items_of_a_alignedsegment(alignedsegment_tmp)
 
     if holeids_e is not None and seq_name not in holeids_e:
         return []
     if holeids_ne is not None and seq_name in holeids_ne:
         return []
     if args.mode == "align":
         if is_unmapped or is_secondary or is_duplicate:
@@ -387,31 +390,37 @@
                                  fkmer_qual, fkmer_map,
                                  rkmer_seq, npass_rev, rkmer_im, rkmer_isd, rkmer_pm, rkmer_psd,
                                  rkmer_qual, rkmer_map,
                                  args.methy_label])
     return feature_list
 
 
-def process_one_holebatch(holebatch, motifs, holeids_e, holeids_ne, dnacontigs, args):
+def process_one_holebatch(input_header, holebatch, motifs, holeids_e, holeids_ne, dnacontigs, args):
     feature_list = []
-    read_idx = 0
     total_num = 0
     failed_num = 0
-    for readinfo in holebatch:
-        features_one = extract_features_from_double_strand_read(readinfo,
-                                                                motifs, holeids_e, holeids_ne,
-                                                                dnacontigs,
-                                                                args)
-        if len(features_one) == 0:
+    holeidxes = []
+
+    for read_idx, readinfo in enumerate(holebatch):
+        try:
+            alignedsegment_tmp = pysam.AlignedSegment.from_dict(readinfo, input_header)
+            features_one = extract_features_from_double_strand_read(alignedsegment_tmp,
+                                                                    motifs, holeids_e, holeids_ne,
+                                                                    dnacontigs,
+                                                                    args)
+            if len(features_one) == 0:
+                failed_num += 1
+            else:
+                feature_list += features_one
+                holeidxes += [read_idx] * len(features_one)
+        except Exception as e:
+            print("Exception: ", e)
             failed_num += 1
-        else:
-            feature_list += features_one
         total_num += 1
-        read_idx += 1
-    return feature_list, total_num, failed_num
+    return holeidxes, feature_list, total_num, failed_num
 
 
 def _features_to_str(features):
     """
 
     :param features: a tuple
     :return:
@@ -441,101 +450,48 @@
                       fkmer_seq, str(npass_fwd), fkmer_im_str, fkmer_isd_str, fkmer_pm_str, fkmer_psd_str,
                       fkmer_qual_str, fkmer_map_str,
                       rkmer_seq, str(npass_rev), rkmer_im_str, rkmer_isd_str, rkmer_pm_str, rkmer_psd_str,
                       rkmer_qual_str, rkmer_map_str,
                       str(label)])
 
 
-def _batch_feature_list2s(feature_list):
-    sampleinfo = []  # contains: chrom, abs_loc, strand, holeid, loc
-
-    fkmers = []
-    fpasss = []
-    fipdms = []
-    fipdsds = []
-    fpwms = []
-    fpwsds = []
-    fquals = []
-    fmaps = []
-
-    rkmers = []
-    rpasss = []
-    ripdms = []
-    ripdsds = []
-    rpwms = []
-    rpwsds = []
-    rquals = []
-    rmaps = []
-
-    labels = []
-    for featureline in feature_list:
-        chrom, abs_loc, strand, holeid, loc, \
-            kmer_seq, kmer_pass, kmer_ipdm, kmer_ipds, kmer_pwm, kmer_pws, kmer_qual, kmer_map, \
-            kmer_seq2, kmer_pass2, kmer_ipdm2, kmer_ipds2, kmer_pwm2, kmer_pws2, kmer_qual2, kmer_map2, \
-            label = featureline
-
-        sampleinfo.append("\t".join(list(map(str, [chrom, abs_loc, strand, holeid, loc]))))
-
-        fkmers.append(np.array([base2code_dna[x] for x in kmer_seq]))
-        fpasss.append(np.array([kmer_pass] * len(kmer_seq)))
-        fipdms.append(np.array(kmer_ipdm, dtype=float))
-        fipdsds.append(np.array(kmer_ipds, dtype=float) if type(kmer_ipds) is not str else 0)
-        fpwms.append(np.array(kmer_pwm, dtype=float))
-        fpwsds.append(np.array(kmer_pws, dtype=float) if type(kmer_pws) is not str else 0)
-        fquals.append(np.array(kmer_qual, dtype=float))
-        fmaps.append(np.array(kmer_map, dtype=float) if type(kmer_map) is not str else 0)
-
-        rkmers.append(np.array([base2code_dna[x] for x in kmer_seq2]))
-        rpasss.append(np.array([kmer_pass2] * len(kmer_seq2)))
-        ripdms.append(np.array(kmer_ipdm2, dtype=float))
-        ripdsds.append(np.array(kmer_ipds2, dtype=float) if type(kmer_ipds2) is not str else 0)
-        rpwms.append(np.array(kmer_pwm2, dtype=float))
-        rpwsds.append(np.array(kmer_pws2, dtype=float) if type(kmer_pws2) is not str else 0)
-        rquals.append(np.array(kmer_qual2, dtype=float))
-        rmaps.append(np.array(kmer_map2, dtype=float) if type(kmer_map2) is not str else 0)
-
-        labels.append(label)
-    return sampleinfo, fkmers, fpasss, fipdms, fipdsds, fpwms, fpwsds, fquals, fmaps, \
-        rkmers, rpasss, ripdms, ripdsds, rpwms, rpwsds, rquals, rmaps, labels
-
-
-def worker_extract_features_from_holebatches(holebatch_q, features_q,
-                                             motifs, holeids_e, holeids_ne, dnacontigs, args,
-                                             is_tostr=True, is_batchlize=False):
-    assert not (is_tostr and is_batchlize)
+def worker_extract_features_from_holebatches(input_header, holebatch_q, features_q,
+                                             motifs, holeids_e, holeids_ne, dnacontigs, args):
     sys.stderr.write("extract_features process-{} starts\n".format(os.getpid()))
+    
+    if isinstance(input_header, OrderedDict) or isinstance(input_header, dict):
+        input_header2 = pysam.AlignmentHeader.from_dict(input_header)
+    else:
+        input_header2 = input_header
+    
     cnt_holesbatch = 0
     total_num_batch, failed_num_batch = 0, 0
     while True:
         if holebatch_q.empty():
             time.sleep(time_wait)
             continue
         holebatch = holebatch_q.get()
         if holebatch == "kill":
             holebatch_q.put("kill")
             break
         # handle one holebatch
-        feature_list, total_num, failed_num = process_one_holebatch(holebatch,
-                                                                    motifs, holeids_e, holeids_ne,
-                                                                    dnacontigs,
-                                                                    args)
+        _, feature_list, total_num, failed_num = process_one_holebatch(input_header2, holebatch,
+                                                                       motifs, holeids_e, holeids_ne,
+                                                                       dnacontigs,
+                                                                       args)
         total_num_batch += total_num
         failed_num_batch += failed_num
         if len(feature_list) > 0:
             features_batch = []
-            if is_tostr:
-                for feature in feature_list:
-                    features_batch.append(_features_to_str(feature))
-            else:
-                features_batch = feature_list
-            if not is_tostr and is_batchlize:  # if is_to_str, then ignore is_batchlize
-                features_batch = _batch_feature_list2s(features_batch)
-
+            # to str
+            for feature in feature_list:
+                features_batch.append(_features_to_str(feature))
             features_q.put(features_batch)
-            while features_q.qsize() > queue_size_border:
+            # while features_q.qsize() > queue_size_border:
+            while features_q.qsize() > (args.threads if args.threads > 1 else 2) * 3:
                 time.sleep(time_wait)
         cnt_holesbatch += 1
     sys.stderr.write("extract_features process-{} ending, proceed {} "
                      "hole_batches({}): {} holes/reads in total, "
                      "{} skipped/failed.\n".format(os.getpid(),
                                                    cnt_holesbatch,
                                                    args.holes_batch,
@@ -593,30 +549,32 @@
     holeids_e = None if args.holeids_e is None else _get_holes(args.holeids_e)
     holeids_ne = None if args.holeids_ne is None else _get_holes(args.holeids_ne)
     motifs = get_motif_seqs(args.motifs)
 
     holebatch_q = Queue()
     features_q = Queue()
 
-    # holebatches = split_inputreads_by_holebatch(inputpath, args)
+    inputreads = _open_inputfile(inputpath, args.mode, threads=args.threads)
+    input_header = inputreads.header
+    inputreads.close()
+
     p_split = mp.Process(target=worker_read_split_holebatches_to_queue,
                          args=(inputpath, holebatch_q, 2, args))
     p_split.daemon = True
     p_split.start()
 
     ps_extract = []
     nproc = args.threads
     if nproc <= 3:
         nproc = 1
     else:
         nproc -= 3  # 2 for reading, 1 for writing
     for _ in range(nproc):
         p = mp.Process(target=worker_extract_features_from_holebatches,
-                       args=(holebatch_q, features_q, motifs, holeids_e, holeids_ne, dnacontigs, args,
-                             True, False))
+                       args=(input_header, holebatch_q, features_q, motifs, holeids_e, holeids_ne, dnacontigs, args))
         p.daemon = True
         p.start()
         ps_extract.append(p)
 
     p_w = mp.Process(target=_write_featurestr_to_file, args=(outputpath, features_q, args.gzip))
     p_w.daemon = True
     p_w.start()
```

### Comparing `ccsmeth-0.3.4/ccsmeth/models.py` & `ccsmeth-0.4.0/ccsmeth/models.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/ccsmeth/train.py` & `ccsmeth-0.4.0/ccsmeth/train.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/ccsmeth/train_multigpu.py` & `ccsmeth-0.4.0/ccsmeth/train_multigpu.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/ccsmeth/utils/attention.py` & `ccsmeth-0.4.0/ccsmeth/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/ccsmeth/utils/constants_torch.py` & `ccsmeth-0.4.0/ccsmeth/utils/constants_torch.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/ccsmeth/utils/lookahead.py` & `ccsmeth-0.4.0/ccsmeth/utils/lookahead.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/ccsmeth/utils/process_utils.py` & `ccsmeth-0.4.0/ccsmeth/utils/process_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                        'H': ['A', 'C', 'U'], 'V': ['A', 'C', 'G'],
                        'N': ['A', 'C', 'G', 'U']}
 
 CODE2CIGAR = "MIDNSHP=XB"
 CIGAR_REGEX = re.compile("(\d+)([MIDNSHP=XB])")
 CIGAR2CODE = dict([y, x] for x, y in enumerate(CODE2CIGAR))
 
-# max_queue_size = 2000
+max_queue_size = 600
 
 nproc_to_call_mods_in_cpu_mode = 2
 
 pbmm2_exec = "pbmm2"
 minimap2_exec = "minimap2"
 bwa_exec = "bwa"
 samtools_exec = "samtools"
```

### Comparing `ccsmeth-0.3.4/ccsmeth/utils/ranger2020.py` & `ccsmeth-0.4.0/ccsmeth/utils/ranger2020.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/ccsmeth/utils/ref_reader.py` & `ccsmeth-0.4.0/ccsmeth/utils/ref_reader.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/ccsmeth/utils/sam2fastq_std.py` & `ccsmeth-0.4.0/ccsmeth/utils/sam2fastq_std.py`

 * *Files identical despite different names*

### Comparing `ccsmeth-0.3.4/ccsmeth.egg-info/PKG-INFO` & `ccsmeth-0.4.0/ccsmeth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ccsmeth
-Version: 0.3.4
+Version: 0.4.0
 Summary: Detecting DNA methylation from PacBio CCS reads
 Home-page: https://github.com/PengNi/ccsmeth
-Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.3.4.tar.gz
+Download-URL: https://github.com/PengNi/ccsmeth/archive/refs/tags/0.4.0.tar.gz
 Author: Peng Ni
 Author-email: 543943952@qq.com
 License: BSD-3-Clause-Clear license
 Keywords: methylation,pacbio,neural network
 Platform: Linux
 Platform: MacOS
 Classifier: Programming Language :: Python :: 3
@@ -20,14 +20,19 @@
 
 ccsmeth
 ========
 
 
 Documentation
 -------------
+v0.4.0
+----------
+optimieze call_mods module, faster generating of modbam file
+
+
 v0.3.4
 ----------
 replace 'numpy.float' by 'float" in extract_features and call_mods modules
 
 
 v0.3.3
 ----------
```

### Comparing `ccsmeth-0.3.4/ccsmeth.egg-info/SOURCES.txt` & `ccsmeth-0.4.0/ccsmeth.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 ccsmeth/__init__.py
 ccsmeth/_bam2modbam.py
+ccsmeth/_call_modifications_txt.py
 ccsmeth/_version.py
 ccsmeth/align_hifi_reads.py
 ccsmeth/call_hifi_reads.py
 ccsmeth/call_modifications.py
 ccsmeth/call_mods_freq_bam.py
 ccsmeth/call_mods_freq_txt.py
 ccsmeth/ccsmeth.py
```

### Comparing `ccsmeth-0.3.4/setup.py` & `ccsmeth-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 with open('requirements.txt', 'r') as rf:
     required = rf.read().splitlines()
 
 
 setup(
     name='ccsmeth',
-    packages=['ccsmeth'],
+    packages=['ccsmeth', 'ccsmeth.utils'],
     keywords=['methylation', 'pacbio', 'neural network'],
     version=__version__,
     url='https://github.com/PengNi/ccsmeth',
     download_url='https://github.com/PengNi/ccsmeth/archive/refs/tags/{}.tar.gz'.format(__version__),
     license='BSD-3-Clause-Clear license',
     author='Peng Ni',
     # install_requires=['numpy>=1.15.3',
```

