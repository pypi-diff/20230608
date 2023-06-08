# Comparing `tmp/moftransformer-2.1.0.tar.gz` & `tmp/moftransformer-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moftransformer-2.1.0.tar", last modified: Tue May 16 04:19:12 2023, max compression
+gzip compressed data, was "moftransformer-2.1.1.tar", last modified: Thu Jun  8 07:01:28 2023, max compression
```

## Comparing `moftransformer-2.1.0.tar` & `moftransformer-2.1.1.tar`

### file list

```diff
@@ -1,277 +1,280 @@
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.888613 moftransformer-2.1.0/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8991 2023-05-16 04:19:12.888613 moftransformer-2.1.0/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8612 2023-05-10 05:12:24.000000 moftransformer-2.1.0/README.md
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      458 2023-05-11 02:34:27.000000 moftransformer-2.1.0/moftransformer/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/assets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       72 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/assets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/assets/bbs.json
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8140 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/assets/colors.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/assets/topology.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/cli/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       31 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/cli/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2443 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/cli/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      324 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/cli/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3040 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/cli/main.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      571 2023-05-11 05:33:02.000000 moftransformer-2.1.0/moftransformer/cli/run.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      328 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/cli/uninstall_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3431 2023-05-10 06:19:20.000000 moftransformer-2.1.0/moftransformer/config.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10515 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/config_ex.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/database/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      633 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/database/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/datamodules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/datamodules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2938 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/datamodules/datamodule.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10088 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/datamodules/dataset.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/examples/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      477 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/__init__.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/examples/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/examples/dataset/test/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       29 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/test_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.868613 moftransformer-2.1.0/moftransformer/examples/dataset/total/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-05-11 05:04:51.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-05-11 05:04:51.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:51.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:51.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-05-11 05:04:57.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-05-11 05:04:57.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:57.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:57.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:55.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-05-11 05:04:53.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-05-11 05:04:53.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:53.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:53.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:54.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-05-11 05:04:56.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-05-11 05:04:56.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:56.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:56.000000 moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.872614 moftransformer-2.1.0/moftransformer/examples/dataset/train/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      206 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/train_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.872614 moftransformer-2.1.0/moftransformer/examples/dataset/val/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       43 2023-05-11 05:04:58.000000 moftransformer-2.1.0/moftransformer/examples/dataset/val_example.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.872614 moftransformer-2.1.0/moftransformer/examples/raw/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/acs+N270+E33.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/fee+N254+E185.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/mok+N109+E146.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/msp+N624+E8.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/raw_example.json
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/sml+N696+E182.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/smm+N577+E166.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/ukg+N387+E203.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/vmk+N489+E8.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/vna+N650+E120.cif
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/raw/zzz+N96+N373+E34.cif
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/examples/visualize/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.872614 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.880613 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test.json
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.880613 moftransformer-2.1.0/moftransformer/gadgets/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       77 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/gadgets/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1806 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/gadgets/my_metrics.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer/libs/
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.884613 moftransformer-2.1.0/moftransformer/libs/GRIDAY/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    41808 2023-05-11 05:04:23.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Cell.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    33448 2023-05-11 05:04:24.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   143440 2023-05-11 05:04:25.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.o
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.884613 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/UFF_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/UFF_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    67552 2023-05-11 05:04:26.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    57152 2023-05-11 05:04:26.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    47328 2023-05-11 05:04:27.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15032 2023-05-11 05:04:27.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    80288 2023-05-11 05:04:28.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Griday.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15752 2023-05-11 05:04:28.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayTypes.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    14896 2023-05-11 05:04:29.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    75600 2023-05-11 05:04:29.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    65096 2023-05-11 05:04:30.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/PairEnergy.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Random.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15360 2023-05-11 05:04:30.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.o
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Timer.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/Vector.hpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   698550 2023-05-11 05:04:30.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/libgriday.a
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.888613 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/Makefile
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2023-05-11 05:04:33.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid2COTA
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   278928 2023-05-11 05:04:33.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid2props
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2023-05-11 05:04:31.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid2visit
--rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   161656 2023-05-11 05:04:31.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid_gen
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.888613 moftransformer-2.1.0/moftransformer/modules/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      122 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/modules/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5783 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/modules/cgcnn.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3255 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/modules/heads.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12893 2023-05-11 05:46:03.000000 moftransformer-2.1.0/moftransformer/modules/module.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7522 2023-05-11 02:40:22.000000 moftransformer-2.1.0/moftransformer/modules/module_utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8487 2023-05-11 02:35:20.000000 moftransformer-2.1.0/moftransformer/modules/objectives.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12812 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/modules/vision_transformer_3d.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11569 2023-05-11 05:23:53.000000 moftransformer-2.1.0/moftransformer/predict.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10348 2023-05-11 05:08:37.000000 moftransformer-2.1.0/moftransformer/run.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.888613 moftransformer-2.1.0/moftransformer/utils/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      242 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/utils/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5552 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/utils/download.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3913 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/utils/install_griday.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16072 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/utils/prepare_data.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3900 2023-05-10 06:19:25.000000 moftransformer-2.1.0/moftransformer/utils/validation.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.888613 moftransformer-2.1.0/moftransformer/visualize/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      130 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/visualize/__init__.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3994 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/visualize/drawer.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/visualize/setting.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9201 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/visualize/utils.py
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    27623 2023-05-05 06:58:55.000000 moftransformer-2.1.0/moftransformer/visualize/visualizer.py
-drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-05-16 04:19:12.860613 moftransformer-2.1.0/moftransformer.egg-info/
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8991 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/PKG-INFO
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12799 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/entry_points.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      313 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/requires.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-05-16 04:19:12.000000 moftransformer-2.1.0/moftransformer.egg-info/top_level.txt
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-05-16 04:19:12.888613 moftransformer-2.1.0/setup.cfg
--rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1524 2023-05-05 07:10:36.000000 moftransformer-2.1.0/setup.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.724438 moftransformer-2.1.1/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10998 2023-06-08 07:01:28.724438 moftransformer-2.1.1/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10620 2023-06-07 08:02:27.000000 moftransformer-2.1.1/README.md
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      509 2023-06-07 02:32:17.000000 moftransformer-2.1.1/moftransformer/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/assets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       72 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/assets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12616 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/assets/bbs.json
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8140 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/assets/colors.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12647 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/assets/topology.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/cli/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       31 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/cli/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2443 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/cli/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      324 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/cli/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3088 2023-06-01 07:55:51.000000 moftransformer-2.1.1/moftransformer/cli/main.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4370 2023-06-01 08:08:34.000000 moftransformer-2.1.1/moftransformer/cli/predict.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5488 2023-06-01 07:50:27.000000 moftransformer-2.1.1/moftransformer/cli/run.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4141 2023-06-07 07:17:33.000000 moftransformer-2.1.1/moftransformer/cli/test.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      328 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/cli/uninstall_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3431 2023-05-10 06:19:20.000000 moftransformer-2.1.1/moftransformer/config.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10515 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/config_ex.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/database/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      633 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/database/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/datamodules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      210 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/datamodules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2938 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/datamodules/datamodule.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10088 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/datamodules/dataset.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/examples/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      477 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/__init__.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/examples/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer/examples/dataset/test/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       29 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/test_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.700438 moftransformer-2.1.1/moftransformer/examples/dataset/total/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    17749 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    24064 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-05-11 05:04:51.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-05-11 05:04:51.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:51.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:51.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-05-11 05:04:57.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-05-11 05:04:57.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:57.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:57.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:55.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-05-11 05:04:53.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-05-11 05:04:53.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:53.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:53.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:52.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:54.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-05-11 05:04:56.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-05-11 05:04:56.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:56.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:56.000000 moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.704438 moftransformer-2.1.1/moftransformer/examples/dataset/train/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9819 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12999 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    11575 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15417 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    30948 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    42294 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18629 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25240 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12117 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16149 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    28743 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    39514 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    40614 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    55509 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    19271 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    26620 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    49650 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    68521 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      206 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/train_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.704438 moftransformer-2.1.1/moftransformer/examples/dataset/val/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7609 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9992 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    25342 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    34455 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54151 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       43 2023-05-11 05:04:58.000000 moftransformer-2.1.1/moftransformer/examples/dataset/val_example.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.708438 moftransformer-2.1.1/moftransformer/examples/raw/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7496 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/acs+N270+E33.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    17441 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9738 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/fee+N254+E185.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11392 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/mok+N109+E146.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    30404 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18345 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/msp+N624+E8.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      317 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/raw_example.json
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    11939 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/sml+N696+E182.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    24953 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/smm+N577+E166.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    28256 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/ukg+N387+E203.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    39904 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/vmk+N489+E8.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    18930 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/vna+N650+E120.cif
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)    48803 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/raw/zzz+N96+N373+E34.cif
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.688438 moftransformer-2.1.1/moftransformer/examples/visualize/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.708438 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.712438 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     9162 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12083 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6405 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8339 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     7074 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9292 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    98728 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6419 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8357 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    93472 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6410 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8347 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   101466 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)     6845 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8961 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      152 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.grid
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   170530 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      164 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test.json
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.712438 moftransformer-2.1.1/moftransformer/gadgets/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       77 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/gadgets/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1806 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/gadgets/my_metrics.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.688438 moftransformer-2.1.1/moftransformer/libs/
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.720438 moftransformer-2.1.1/moftransformer/libs/GRIDAY/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2799 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      654 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    41808 2023-05-11 05:04:23.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2448 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Cell.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7789 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      414 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    33448 2023-05-11 05:04:24.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    54588 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    18619 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3812 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   143440 2023-05-11 05:04:25.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.o
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.720438 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4751 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/UFF_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      845 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/UFF_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      202 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_FF.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      190 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_FF_Shifted.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      318 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_O_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      228 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_Gau_Si.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       26 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/Zeolite_Type.def
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7197 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      866 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    67552 2023-05-11 05:04:26.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13991 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      865 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    57152 2023-05-11 05:04:26.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7362 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1197 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    47328 2023-05-11 05:04:27.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3007 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15032 2023-05-11 05:04:27.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9534 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      936 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    80288 2023-05-11 05:04:28.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      320 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Griday.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      948 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      669 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15752 2023-05-11 05:04:28.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      567 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayTypes.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     4380 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      776 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    14896 2023-05-11 05:04:29.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      334 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    21824 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2366 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    75600 2023-05-11 05:04:29.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5664 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      922 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    65096 2023-05-11 05:04:30.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      730 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/PairEnergy.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      570 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Random.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5106 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      764 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    15360 2023-05-11 05:04:30.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.o
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      811 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Timer.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     2277 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/Vector.hpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)   698550 2023-05-11 05:04:30.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/libgriday.a
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.720438 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      563 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/Makefile
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5834 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2023-05-11 05:04:33.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid2COTA
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   278928 2023-05-11 05:04:33.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid2props
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   130000 2023-05-11 05:04:31.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid2visit
+-rwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)   161656 2023-05-11 05:04:31.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid_gen
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1046 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_cota.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1742 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      900 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_visit.cpp
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.720438 moftransformer-2.1.1/moftransformer/modules/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      122 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/modules/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5783 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/modules/cgcnn.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3255 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/modules/heads.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    13191 2023-06-08 05:11:08.000000 moftransformer-2.1.1/moftransformer/modules/module.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     7522 2023-05-11 02:40:22.000000 moftransformer-2.1.1/moftransformer/modules/module_utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8568 2023-06-08 05:11:29.000000 moftransformer-2.1.1/moftransformer/modules/objectives.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12812 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/modules/vision_transformer_3d.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10433 2023-06-08 05:35:34.000000 moftransformer-2.1.1/moftransformer/predict.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10576 2023-06-07 06:30:29.000000 moftransformer-2.1.1/moftransformer/run.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     8614 2023-06-07 07:19:44.000000 moftransformer-2.1.1/moftransformer/test.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.724438 moftransformer-2.1.1/moftransformer/utils/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      242 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/utils/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     5552 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/utils/download.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3913 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/utils/install_griday.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    16162 2023-05-25 04:50:04.000000 moftransformer-2.1.1/moftransformer/utils/prepare_data.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3986 2023-06-01 08:08:31.000000 moftransformer-2.1.1/moftransformer/utils/validation.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.724438 moftransformer-2.1.1/moftransformer/visualize/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      130 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/visualize/__init__.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3994 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/visualize/drawer.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     3705 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/visualize/setting.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     9201 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/visualize/utils.py
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    27623 2023-05-05 06:58:55.000000 moftransformer-2.1.1/moftransformer/visualize/visualizer.py
+drwxrwxr-x   0 dudgns1675  (1001) dudgns1675  (1001)        0 2023-06-08 07:01:28.692438 moftransformer-2.1.1/moftransformer.egg-info/
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    10998 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)    12879 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)        1 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       64 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/entry_points.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)      313 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/requires.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       15 2023-06-08 07:01:28.000000 moftransformer-2.1.1/moftransformer.egg-info/top_level.txt
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)       38 2023-06-08 07:01:28.724438 moftransformer-2.1.1/setup.cfg
+-rw-rw-r--   0 dudgns1675  (1001) dudgns1675  (1001)     1524 2023-05-05 07:10:36.000000 moftransformer-2.1.1/setup.py
```

### Comparing `moftransformer-2.1.0/PKG-INFO` & `moftransformer-2.1.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,15 @@
-Metadata-Version: 2.1
-Name: moftransformer
-Version: 2.1.0
-Summary: moftransformer
-Home-page: https://hspark1212.github.io/MOFTransformer/
-Download-URL: https://github.com/hspark1212/MOFTransformer
-Author: Yeonghun Kang, Hyunsoo Park
-Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.0-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.1-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.0-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.1-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
@@ -35,14 +23,16 @@
  This package provides a universal transfer learning model, `PMTransformer` (Porous Materials Transformer), which obtains the state-of-the-art performance in predicting various properties of porous materials. The PMTRansformer was pre-trainied with 1.9 million hypothetical porous materials including Metal-Organic Frameworks (MOFs), Covalent-Organic Frameworks (COFs), Porous Polymer Networks (PPNs), and zeolites. By fine-tuning the pre-trained `PMTransformer`, you can easily obtain machine learning models to accurately predict various properties of porous materials .
  
  NOTE: From version 2.0.0, the default pre-training model has been changed from `MOFTransformer` to `PMTransformer`, which was pre-trained with a larger dataset, containing other porous materials as well as MOFs. The `PMTransformer` outperforms the `MOFTransformer` in predicting various properties of porous materials.
 
 ## [Install](https://hspark1212.github.io/MOFTransformer/installation.html)
 
 ### Depedencies
+NOTE: This package is primarily tested on Linux. We strongly recommend using Linux for the installation.
+
 ```
 python>=3.8
 ```
 Given that MOFTransformer is based on pytorch, please install pytorch (>= 1.12.0) according to your environments.
 
 ### Installation using PIP 
 ```
@@ -70,23 +60,89 @@
 ```
 2. Fine-tune the pretrained MOFTransformer.
 ```python
 import moftransformer
 from moftransformer.examples import example_path
 
 # data root and downstream from example
-data_root = example_path['data_root']
+root_dataset = example_path['root_dataset']
 downstream = example_path['downstream']
 log_dir = './logs/'
 # load_path = "pmtransformer" (default)
 
-moftransformer.run(data_root, downstream, log_dir=log_dir, 
-                   max_epochs=max_epochs, batch_size=batch_size,)
+# kwargs (optional)
+max_epochs = 10
+batch_size = 8
+mean = 0
+std = 1
+
+
+moftransformer.run(root_dataset, downstream, log_dir=log_dir,                   
+                   max_epochs=max_epochs, batch_size=batch_size,
+                   mean=mean, std=std)
+```
+
+3. Test fine-tuned model
+```python
+from pathlib import Path
+import moftransformer
+from moftransformer.examples import example_path
+
+root_dataset = example_path['root_dataset']
+downstream = example_path['downstream']
+
+# Get ckpt file
+seed = 0               # default seeds
+version = 0            # version for model. It increases with the number of trains
+
+# For version > 2.1.1, best.ckpt exists
+checkpoint = 'best'    # Epochs where the model is stored. 
+save_dir = 'result/'
+
+# optional keyword
+mean = 0
+std = 1
+
+load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/version_{version}/checkpoints/{checkpoint}.ckpt'
+
+if not load_path.exists():
+    raise ValueError(f'load_path does not exists. check path for .ckpt file : {load_path}')
+
+moftransformer.test(root_dataset, load_path, downstream=downstream,
+                   save_dir=save_dir, mean=mean, std=std)
 ```
-3. Visualize analysis of feature importance for the fine-tuned model.
+
+4. predict from fine-tuned model
+```python
+from pathlib import Path
+import moftransformer
+from moftransformer.examples import example_path
+
+root_dataset = example_path['root_dataset']
+downstream = example_path['downstream']
+
+# Get ckpt file
+log_dir = './logs/'    # same directory make from training
+seed = 0               # default seeds
+version = 0            # version for model. It increases with the number of trains
+checkpoint = 'best'    # Epochs where the model is stored. 
+mean = 0
+std = 1
+
+load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/version_{version}/checkpoints/{checkpoint}.ckpt'
+
+if not load_path.exists():
+    raise ValueError(f'load_path does not exists. check path for .ckpt file : {load_path}')
+    
+moftransformer.predict(
+    root_dataset, load_path=load_path, downstream=downstream, split='all', mean=mean, std=std
+)
+```
+
+5. Visualize analysis of feature importance for the fine-tuned model.
 ```python
 %matplotlib widget
 from visualize import PatchVisualizer
 
 model_path = "examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
 data_path = 'examples/visualize/dataset/'
 cifname = 'MIBQAR01_FSR'
```

#### html2text {}

```diff
@@ -1,14 +1,9 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 2.1.0 Summary:
-moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
-Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
-Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
-docs/source/assets/fig1.jpg)
+![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
+source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
 # [PMTransformer (MOFTransformer)](https://hspark1212.github.io/MOFTransformer/
 index.html) This package provides a universal transfer learning model,
 `PMTransformer` (Porous Materials Transformer), which obtains the state-of-the-
 art performance in predicting various properties of porous materials. The
 PMTRansformer was pre-trainied with 1.9 million hypothetical porous materials
 including Metal-Organic Frameworks (MOFs), Covalent-Organic Frameworks (COFs),
@@ -16,37 +11,62 @@
 `PMTransformer`, you can easily obtain machine learning models to accurately
 predict various properties of porous materials . NOTE: From version 2.0.0, the
 default pre-training model has been changed from `MOFTransformer` to
 `PMTransformer`, which was pre-trained with a larger dataset, containing other
 porous materials as well as MOFs. The `PMTransformer` outperforms the
 `MOFTransformer` in predicting various properties of porous materials. ##
 [Install](https://hspark1212.github.io/MOFTransformer/installation.html) ###
-Depedencies ``` python>=3.8 ``` Given that MOFTransformer is based on pytorch,
-please install pytorch (>= 1.12.0) according to your environments. ###
-Installation using PIP ``` $ pip install moftransformer ``` ### Download the
-pretrained models (ckpt file) - you can download the pretrained models
-(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) via [figshare](https://
-figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2) or
-you can download with a command line: ``` $ moftransformer download
-pretrain_model ``` ### (Optional) Download pre-embeddings for CoREMOF, QMOF -
-we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-
-grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database. ``` $
-moftransformer download coremof $ moftransformer download qmof ``` ## [Getting
-Started](https://hspark1212.github.io/MOFTransformer/tutorial.html) 1. At
-first, you download dataset of hMOFs (20,000 MOFs) as an example. ``` $
-moftransformer download hmof ``` 2. Fine-tune the pretrained MOFTransformer.
-```python import moftransformer from moftransformer.examples import
-example_path # data root and downstream from example data_root = example_path
-['data_root'] downstream = example_path['downstream'] log_dir = './logs/' #
-load_path = "pmtransformer" (default) moftransformer.run(data_root, downstream,
-log_dir=log_dir, max_epochs=max_epochs, batch_size=batch_size,) ``` 3.
-Visualize analysis of feature importance for the fine-tuned model. ```python
-%matplotlib widget from visualize import PatchVisualizer model_path =
-"examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
-data_path = 'examples/visualize/dataset/' cifname = 'MIBQAR01_FSR' vis =
+Depedencies NOTE: This package is primarily tested on Linux. We strongly
+recommend using Linux for the installation. ``` python>=3.8 ``` Given that
+MOFTransformer is based on pytorch, please install pytorch (>= 1.12.0)
+according to your environments. ### Installation using PIP ``` $ pip install
+moftransformer ``` ### Download the pretrained models (ckpt file) - you can
+download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`)
+via [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-
+trained_model/22698655/2) or you can download with a command line: ``` $
+moftransformer download pretrain_model ``` ### (Optional) Download pre-
+embeddings for CoREMOF, QMOF - we've provide the pre-embeddings (i.e., atom-
+based graph embeddings and energy-grid embeddings), inputs of `PMTransformer`,
+for CoREMOF, QMOF database. ``` $ moftransformer download coremof $
+moftransformer download qmof ``` ## [Getting Started](https://
+hspark1212.github.io/MOFTransformer/tutorial.html) 1. At first, you download
+dataset of hMOFs (20,000 MOFs) as an example. ``` $ moftransformer download
+hmof ``` 2. Fine-tune the pretrained MOFTransformer. ```python import
+moftransformer from moftransformer.examples import example_path # data root and
+downstream from example root_dataset = example_path['root_dataset'] downstream
+= example_path['downstream'] log_dir = './logs/' # load_path = "pmtransformer"
+(default) # kwargs (optional) max_epochs = 10 batch_size = 8 mean = 0 std = 1
+moftransformer.run(root_dataset, downstream, log_dir=log_dir,
+max_epochs=max_epochs, batch_size=batch_size, mean=mean, std=std) ``` 3. Test
+fine-tuned model ```python from pathlib import Path import moftransformer from
+moftransformer.examples import example_path root_dataset = example_path
+['root_dataset'] downstream = example_path['downstream'] # Get ckpt file seed =
+0 # default seeds version = 0 # version for model. It increases with the number
+of trains # For version > 2.1.1, best.ckpt exists checkpoint = 'best' # Epochs
+where the model is stored. save_dir = 'result/' # optional keyword mean = 0 std
+= 1 load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/
+version_{version}/checkpoints/{checkpoint}.ckpt' if not load_path.exists():
+raise ValueError(f'load_path does not exists. check path for .ckpt file :
+{load_path}') moftransformer.test(root_dataset, load_path,
+downstream=downstream, save_dir=save_dir, mean=mean, std=std) ``` 4. predict
+from fine-tuned model ```python from pathlib import Path import moftransformer
+from moftransformer.examples import example_path root_dataset = example_path
+['root_dataset'] downstream = example_path['downstream'] # Get ckpt file
+log_dir = './logs/' # same directory make from training seed = 0 # default
+seeds version = 0 # version for model. It increases with the number of trains
+checkpoint = 'best' # Epochs where the model is stored. mean = 0 std = 1
+load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/
+version_{version}/checkpoints/{checkpoint}.ckpt' if not load_path.exists():
+raise ValueError(f'load_path does not exists. check path for .ckpt file :
+{load_path}') moftransformer.predict( root_dataset, load_path=load_path,
+downstream=downstream, split='all', mean=mean, std=std ) ``` 5. Visualize
+analysis of feature importance for the fine-tuned model. ```python %matplotlib
+widget from visualize import PatchVisualizer model_path = "examples/
+finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt' data_path =
+'examples/visualize/dataset/' cifname = 'MIBQAR01_FSR' vis =
 PatchVisualizer.from_cifname(cifname, model_path, data_path) vis.draw_graph() #
 or vis.draw_grid() ``` ## [Architecture](https://hspark1212.github.io/
 MOFTransformer/introduction.html) It is a multi-modal pre-training Transformer
 encoder which is designed to capture both local and global features of porous
 materials. The pre-traning tasks are as follows: (1) Topology Prediction (2)
 Void Fraction Prediction (3) Building Block Classification It takes two
 different representations as input - Atom-based Graph Embedding : CGCNN w/
```

### Comparing `moftransformer-2.1.0/README.md` & `moftransformer-2.1.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,27 @@
+Metadata-Version: 2.1
+Name: moftransformer
+Version: 2.1.1
+Summary: moftransformer
+Home-page: https://hspark1212.github.io/MOFTransformer/
+Download-URL: https://github.com/hspark1212/MOFTransformer
+Author: Yeonghun Kang, Hyunsoo Park
+Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.0-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.1-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.0-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.1-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
@@ -23,14 +35,16 @@
  This package provides a universal transfer learning model, `PMTransformer` (Porous Materials Transformer), which obtains the state-of-the-art performance in predicting various properties of porous materials. The PMTRansformer was pre-trainied with 1.9 million hypothetical porous materials including Metal-Organic Frameworks (MOFs), Covalent-Organic Frameworks (COFs), Porous Polymer Networks (PPNs), and zeolites. By fine-tuning the pre-trained `PMTransformer`, you can easily obtain machine learning models to accurately predict various properties of porous materials .
  
  NOTE: From version 2.0.0, the default pre-training model has been changed from `MOFTransformer` to `PMTransformer`, which was pre-trained with a larger dataset, containing other porous materials as well as MOFs. The `PMTransformer` outperforms the `MOFTransformer` in predicting various properties of porous materials.
 
 ## [Install](https://hspark1212.github.io/MOFTransformer/installation.html)
 
 ### Depedencies
+NOTE: This package is primarily tested on Linux. We strongly recommend using Linux for the installation.
+
 ```
 python>=3.8
 ```
 Given that MOFTransformer is based on pytorch, please install pytorch (>= 1.12.0) according to your environments.
 
 ### Installation using PIP 
 ```
@@ -58,23 +72,89 @@
 ```
 2. Fine-tune the pretrained MOFTransformer.
 ```python
 import moftransformer
 from moftransformer.examples import example_path
 
 # data root and downstream from example
-data_root = example_path['data_root']
+root_dataset = example_path['root_dataset']
 downstream = example_path['downstream']
 log_dir = './logs/'
 # load_path = "pmtransformer" (default)
 
-moftransformer.run(data_root, downstream, log_dir=log_dir, 
-                   max_epochs=max_epochs, batch_size=batch_size,)
+# kwargs (optional)
+max_epochs = 10
+batch_size = 8
+mean = 0
+std = 1
+
+
+moftransformer.run(root_dataset, downstream, log_dir=log_dir,                   
+                   max_epochs=max_epochs, batch_size=batch_size,
+                   mean=mean, std=std)
+```
+
+3. Test fine-tuned model
+```python
+from pathlib import Path
+import moftransformer
+from moftransformer.examples import example_path
+
+root_dataset = example_path['root_dataset']
+downstream = example_path['downstream']
+
+# Get ckpt file
+seed = 0               # default seeds
+version = 0            # version for model. It increases with the number of trains
+
+# For version > 2.1.1, best.ckpt exists
+checkpoint = 'best'    # Epochs where the model is stored. 
+save_dir = 'result/'
+
+# optional keyword
+mean = 0
+std = 1
+
+load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/version_{version}/checkpoints/{checkpoint}.ckpt'
+
+if not load_path.exists():
+    raise ValueError(f'load_path does not exists. check path for .ckpt file : {load_path}')
+
+moftransformer.test(root_dataset, load_path, downstream=downstream,
+                   save_dir=save_dir, mean=mean, std=std)
 ```
-3. Visualize analysis of feature importance for the fine-tuned model.
+
+4. predict from fine-tuned model
+```python
+from pathlib import Path
+import moftransformer
+from moftransformer.examples import example_path
+
+root_dataset = example_path['root_dataset']
+downstream = example_path['downstream']
+
+# Get ckpt file
+log_dir = './logs/'    # same directory make from training
+seed = 0               # default seeds
+version = 0            # version for model. It increases with the number of trains
+checkpoint = 'best'    # Epochs where the model is stored. 
+mean = 0
+std = 1
+
+load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/version_{version}/checkpoints/{checkpoint}.ckpt'
+
+if not load_path.exists():
+    raise ValueError(f'load_path does not exists. check path for .ckpt file : {load_path}')
+    
+moftransformer.predict(
+    root_dataset, load_path=load_path, downstream=downstream, split='all', mean=mean, std=std
+)
+```
+
+5. Visualize analysis of feature importance for the fine-tuned model.
 ```python
 %matplotlib widget
 from visualize import PatchVisualizer
 
 model_path = "examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
 data_path = 'examples/visualize/dataset/'
 cifname = 'MIBQAR01_FSR'
@@ -156,8 +236,8 @@
 
 ## Contributing 🙌
 
 Contributions are welcome! If you have any suggestions or find any issues, please open an issue or a pull request.
 
 ## License 📄
 
-This project is licensed under the MIT License. See the `LICENSE` file for more information.
+This project is licensed under the MIT License. See the `LICENSE` file for more information.
```

#### html2text {}

```diff
@@ -1,9 +1,14 @@
-![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/
-source/assets/fig1.jpg)
+Metadata-Version: 2.1 Name: moftransformer Version: 2.1.1 Summary:
+moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
+Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
+Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
+Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
+docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
+docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
 # [PMTransformer (MOFTransformer)](https://hspark1212.github.io/MOFTransformer/
 index.html) This package provides a universal transfer learning model,
 `PMTransformer` (Porous Materials Transformer), which obtains the state-of-the-
 art performance in predicting various properties of porous materials. The
 PMTRansformer was pre-trainied with 1.9 million hypothetical porous materials
 including Metal-Organic Frameworks (MOFs), Covalent-Organic Frameworks (COFs),
@@ -11,37 +16,62 @@
 `PMTransformer`, you can easily obtain machine learning models to accurately
 predict various properties of porous materials . NOTE: From version 2.0.0, the
 default pre-training model has been changed from `MOFTransformer` to
 `PMTransformer`, which was pre-trained with a larger dataset, containing other
 porous materials as well as MOFs. The `PMTransformer` outperforms the
 `MOFTransformer` in predicting various properties of porous materials. ##
 [Install](https://hspark1212.github.io/MOFTransformer/installation.html) ###
-Depedencies ``` python>=3.8 ``` Given that MOFTransformer is based on pytorch,
-please install pytorch (>= 1.12.0) according to your environments. ###
-Installation using PIP ``` $ pip install moftransformer ``` ### Download the
-pretrained models (ckpt file) - you can download the pretrained models
-(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) via [figshare](https://
-figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2) or
-you can download with a command line: ``` $ moftransformer download
-pretrain_model ``` ### (Optional) Download pre-embeddings for CoREMOF, QMOF -
-we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-
-grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database. ``` $
-moftransformer download coremof $ moftransformer download qmof ``` ## [Getting
-Started](https://hspark1212.github.io/MOFTransformer/tutorial.html) 1. At
-first, you download dataset of hMOFs (20,000 MOFs) as an example. ``` $
-moftransformer download hmof ``` 2. Fine-tune the pretrained MOFTransformer.
-```python import moftransformer from moftransformer.examples import
-example_path # data root and downstream from example data_root = example_path
-['data_root'] downstream = example_path['downstream'] log_dir = './logs/' #
-load_path = "pmtransformer" (default) moftransformer.run(data_root, downstream,
-log_dir=log_dir, max_epochs=max_epochs, batch_size=batch_size,) ``` 3.
-Visualize analysis of feature importance for the fine-tuned model. ```python
-%matplotlib widget from visualize import PatchVisualizer model_path =
-"examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
-data_path = 'examples/visualize/dataset/' cifname = 'MIBQAR01_FSR' vis =
+Depedencies NOTE: This package is primarily tested on Linux. We strongly
+recommend using Linux for the installation. ``` python>=3.8 ``` Given that
+MOFTransformer is based on pytorch, please install pytorch (>= 1.12.0)
+according to your environments. ### Installation using PIP ``` $ pip install
+moftransformer ``` ### Download the pretrained models (ckpt file) - you can
+download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`)
+via [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-
+trained_model/22698655/2) or you can download with a command line: ``` $
+moftransformer download pretrain_model ``` ### (Optional) Download pre-
+embeddings for CoREMOF, QMOF - we've provide the pre-embeddings (i.e., atom-
+based graph embeddings and energy-grid embeddings), inputs of `PMTransformer`,
+for CoREMOF, QMOF database. ``` $ moftransformer download coremof $
+moftransformer download qmof ``` ## [Getting Started](https://
+hspark1212.github.io/MOFTransformer/tutorial.html) 1. At first, you download
+dataset of hMOFs (20,000 MOFs) as an example. ``` $ moftransformer download
+hmof ``` 2. Fine-tune the pretrained MOFTransformer. ```python import
+moftransformer from moftransformer.examples import example_path # data root and
+downstream from example root_dataset = example_path['root_dataset'] downstream
+= example_path['downstream'] log_dir = './logs/' # load_path = "pmtransformer"
+(default) # kwargs (optional) max_epochs = 10 batch_size = 8 mean = 0 std = 1
+moftransformer.run(root_dataset, downstream, log_dir=log_dir,
+max_epochs=max_epochs, batch_size=batch_size, mean=mean, std=std) ``` 3. Test
+fine-tuned model ```python from pathlib import Path import moftransformer from
+moftransformer.examples import example_path root_dataset = example_path
+['root_dataset'] downstream = example_path['downstream'] # Get ckpt file seed =
+0 # default seeds version = 0 # version for model. It increases with the number
+of trains # For version > 2.1.1, best.ckpt exists checkpoint = 'best' # Epochs
+where the model is stored. save_dir = 'result/' # optional keyword mean = 0 std
+= 1 load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/
+version_{version}/checkpoints/{checkpoint}.ckpt' if not load_path.exists():
+raise ValueError(f'load_path does not exists. check path for .ckpt file :
+{load_path}') moftransformer.test(root_dataset, load_path,
+downstream=downstream, save_dir=save_dir, mean=mean, std=std) ``` 4. predict
+from fine-tuned model ```python from pathlib import Path import moftransformer
+from moftransformer.examples import example_path root_dataset = example_path
+['root_dataset'] downstream = example_path['downstream'] # Get ckpt file
+log_dir = './logs/' # same directory make from training seed = 0 # default
+seeds version = 0 # version for model. It increases with the number of trains
+checkpoint = 'best' # Epochs where the model is stored. mean = 0 std = 1
+load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/
+version_{version}/checkpoints/{checkpoint}.ckpt' if not load_path.exists():
+raise ValueError(f'load_path does not exists. check path for .ckpt file :
+{load_path}') moftransformer.predict( root_dataset, load_path=load_path,
+downstream=downstream, split='all', mean=mean, std=std ) ``` 5. Visualize
+analysis of feature importance for the fine-tuned model. ```python %matplotlib
+widget from visualize import PatchVisualizer model_path = "examples/
+finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt' data_path =
+'examples/visualize/dataset/' cifname = 'MIBQAR01_FSR' vis =
 PatchVisualizer.from_cifname(cifname, model_path, data_path) vis.draw_graph() #
 or vis.draw_grid() ``` ## [Architecture](https://hspark1212.github.io/
 MOFTransformer/introduction.html) It is a multi-modal pre-training Transformer
 encoder which is designed to capture both local and global features of porous
 materials. The pre-traning tasks are as follows: (1) Topology Prediction (2)
 Void Fraction Prediction (3) Building Block Classification It takes two
 different representations as input - Atom-based Graph Embedding : CGCNN w/
```

### Comparing `moftransformer-2.1.0/moftransformer/assets/bbs.json` & `moftransformer-2.1.1/moftransformer/assets/bbs.json`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/assets/colors.py` & `moftransformer-2.1.1/moftransformer/assets/colors.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/assets/topology.json` & `moftransformer-2.1.1/moftransformer/assets/topology.json`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/cli/download.py` & `moftransformer-2.1.1/moftransformer/cli/download.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/cli/main.py` & `moftransformer-2.1.1/moftransformer/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from moftransformer import __version__
 
 commands = [
     # ('info' , 'moftransformer.cli.info'),
     ("install-griday", "moftransformer.cli.install_griday"),
     ("uninstall-griday", "moftransformer.cli.uninstall_griday"),
     ("run", "moftransformer.cli.run"),
+    ("predict", "moftransformer.cli.predict"),
     ("download", "moftransformer.cli.download"),
 ]
 
 
 def main(prog="moftransformer", version=__version__, commands=commands, args=None):
     parser = argparse.ArgumentParser(
         prog=prog,
```

### Comparing `moftransformer-2.1.0/moftransformer/config.py` & `moftransformer-2.1.1/moftransformer/config.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/config_ex.py` & `moftransformer-2.1.1/moftransformer/config_ex.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/database/__init__.py` & `moftransformer-2.1.1/moftransformer/database/__init__.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/datamodules/datamodule.py` & `moftransformer-2.1.1/moftransformer/datamodules/datamodule.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/datamodules/dataset.py` & `moftransformer-2.1.1/moftransformer/datamodules/dataset.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/test/etc+N80+N60+E173+E76.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/acs+N270+E33.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/acs+N270+E33.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/etc+N80+N60+E173+E76.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/fee+N254+E185.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/fee+N254+E185.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/mok+N109+E146.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/mok+N109+E146.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/mrc+N568+N190+E116+E77.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/msp+N624+E8.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/msp+N624+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/sml+N696+E182.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/sml+N696+E182.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/smm+N577+E166.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/smm+N577+E166.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/ukg+N387+E203.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/vmk+N489+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/vna+N650+E120.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/vna+N650+E120.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/total/zzz+N96+N373+E34.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/fee+N254+E185.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/fee+N254+E185.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/mok+N109+E146.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/mok+N109+E146.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/mrc+N568+N190+E116+E77.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/msp+N624+E8.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/msp+N624+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/sml+N696+E182.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/sml+N696+E182.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/ukg+N387+E203.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/vmk+N489+E8.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/vna+N650+E120.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/vna+N650+E120.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/train/zzz+N96+N373+E34.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/val/acs+N270+E33.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/val/acs+N270+E33.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.cif` & `moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.graphdata` & `moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/dataset/val/smm+N577+E166.griddata16` & `moftransformer-2.1.1/moftransformer/examples/dataset/val/smm+N577+E166.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/acs+N270+E33.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/acs+N270+E33.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/etc+N80+N60+E173+E76.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/fee+N254+E185.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/fee+N254+E185.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/mok+N109+E146.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/mok+N109+E146.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/mrc+N568+N190+E116+E77.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/msp+N624+E8.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/msp+N624+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/sml+N696+E182.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/sml+N696+E182.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/smm+N577+E166.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/smm+N577+E166.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/ukg+N387+E203.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/ukg+N387+E203.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/vmk+N489+E8.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/vmk+N489+E8.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/vna+N650+E120.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/vna+N650+E120.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/raw/zzz+N96+N373+E34.cif` & `moftransformer-2.1.1/moftransformer/examples/raw/zzz+N96+N373+E34.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/DOTSOV01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MIBQAR01_FSR.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_42_1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/MOF-5_cooh_2_573_2.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/core_NEXVET_freeONLY.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.cif`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.graphdata`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16` & `moftransformer-2.1.1/moftransformer/examples/visualize/dataset/test/gmof_Uio66Zr-BDC_A_No1.griddata16`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/gadgets/my_metrics.py` & `moftransformer-2.1.1/moftransformer/gadgets/my_metrics.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/AtomTypeMap.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/AtomTypeMap.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Cell.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Cell.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ChannelAnalyzer.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ChannelAnalyzer.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.cpp-backup`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/EnergyGrid.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/EnergyGrid.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/UFF_FF.def` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/UFF_FF.def`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/FF/UFF_Type.def` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/FF/UFF_Type.def`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ForceField.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ForceField.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/FourierAnalyzer.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/FourierAnalyzer.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Framework.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Framework.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Gaussian.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Gaussian.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridMaker.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridMaker.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayException.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayException.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/GridayTypes.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/GridayTypes.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/LennardJones.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/LennardJones.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/MaterialGrid.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/MaterialGrid.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/NlistMaker.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/NlistMaker.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/PairEnergy.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/PairEnergy.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Random.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Random.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/ShiftedLJ.o` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/ShiftedLJ.o`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Timer.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Timer.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/Vector.hpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/Vector.hpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/libgriday.a` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/libgriday.a`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/Makefile` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/Makefile`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/adsorption_properties.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid2COTA` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid2COTA`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid2props` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid2props`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid2visit` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid2visit`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/grid_gen` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/grid_gen`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_cota.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_cota.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_make_egrid.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/libs/GRIDAY/scripts/main_visit.cpp` & `moftransformer-2.1.1/moftransformer/libs/GRIDAY/scripts/main_visit.cpp`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/modules/cgcnn.py` & `moftransformer-2.1.1/moftransformer/modules/cgcnn.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/modules/heads.py` & `moftransformer-2.1.1/moftransformer/modules/heads.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/modules/module.py` & `moftransformer-2.1.1/moftransformer/modules/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,19 +325,26 @@
     
     def on_predict_start(self):
         self.write_log = False
         module_utils.set_task(self)
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
         output = self(batch)
+        
+        softmax = torch.nn.Softmax(dim=1)
+        if 'classification_logits' in output:
+            output['classification_logits'] = softmax(output['classification_logits'])
+            output['classification_logits_index'] = torch.argmax(output['classification_logits'], dim=1)
+
         output = {
             k: (v.cpu().tolist() if torch.is_tensor(v) else v)
             for k, v in output.items()
             if ('logits' in k) or ('labels' in k) or 'cif_id' == k
         }
+
         return output
     
     def on_predict_epoch_end(self, *args):
         self.test_labels.clear()
         self.test_logits.clear()
 
     def on_predict_end(self, ):
```

### Comparing `moftransformer-2.1.0/moftransformer/modules/module_utils.py` & `moftransformer-2.1.1/moftransformer/modules/module_utils.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/modules/objectives.py` & `moftransformer-2.1.1/moftransformer/modules/objectives.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,18 @@
     logits = pl_module.regression_head(infer["cls_feats"]).squeeze(-1)  # [B]
     labels = torch.FloatTensor(batch["target"]).to(logits.device)  # [B]
     assert len(labels.shape) == 1
 
     # normalize encode if config["mean"] and config["std], else pass
     labels = normalizer.encode(labels)
     loss = F.mse_loss(logits, labels)
+
+    labels = labels.to(torch.float32)
+    logits = logits.to(torch.float32)
+
     ret = {
         "cif_id": infer["cif_id"],
         "cls_feats": infer["cls_feats"],
         "regression_loss": loss,
         "regression_logits": normalizer.decode(logits),
         "regression_labels": normalizer.decode(labels),
     }
@@ -59,15 +63,15 @@
     if binary:
         logits = logits.squeeze(dim=-1)
         loss = F.binary_cross_entropy_with_logits(input=logits, target=labels.float())
     else:
         loss = F.cross_entropy(logits, labels)
 
     ret = {
-        "cif_ids": infer["cif_id"],
+        "cif_id": infer["cif_id"],
         "cls_feats": infer["cls_feats"],
         "classification_loss": loss,
         "classification_logits": logits,
         "classification_labels": labels,
     }
 
     # call update() loss and acc
```

### Comparing `moftransformer-2.1.0/moftransformer/modules/vision_transformer_3d.py` & `moftransformer-2.1.1/moftransformer/modules/vision_transformer_3d.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/predict.py` & `moftransformer-2.1.1/moftransformer/predict.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# MOFTransformer version 2.1.0
+# MOFTransformer version 2.1.1
 import sys
 import os
 import copy
 import warnings
 from pathlib import Path
 import re
 import csv
@@ -25,15 +25,15 @@
 
 def predict(root_dataset, load_path, downstream=None, split='all', save_dir=None,
             **kwargs):
     """
      Predict MOFTransformer.
 
      Call signatures::
-         predict(root_dataset, laod_path, downstream, [split], **kwargs)
+         predict(root_dataset, load_path, downstream, [split], **kwargs)
 
      The basic usage of the code is as follows:
 
      >>> predict(root_dataset, load_path, downstream)  # predict MOFTransformer from [root_dataset] with train_{downstream}.json
      >>> predict(root_dataset, load_path, downstream, split='test', save_dir='./predict') # predict MOFTransformer from trained-model path
 
      Dataset preperation is necessary for learning
@@ -72,21 +72,14 @@
              if downstream is None, target json is 'train.json', 'val.json', and 'test.json'
      :param split : The split you want to predict on your dataset ('all', 'train', 'test', or 'val')
      :param save_dir : Path for directory you want to save *.csv file. (default : None -> path for loaded model)
 
      
      Other Parameters
      ________________
-     load_path: str, default: "pmtransformer"
-     This parameter specifies the path of the model that will be used for training/testing.
-     The available options are "pmtransformer", "moftransformer", other .ckpt paths, and None (scratch).
-     If you want to test a fine-tuned model, you should specify the path to the .ckpt file stored in the 'log' folder.
-     To download a pre-trained model, use the following command:
-     $ moftransformer download pretrain_model
-
      loss_names: str or list, or dict, default: "regression"
          One or more of the following loss : 'regression', 'classification', 'mpt', 'moc', and 'vfp'
 
      n_classes: int, default: 0
          Number of classes when your loss is 'classification'
 
      batch_size: int, default: 1024
@@ -235,50 +228,32 @@
     
     config = get_valid_config(config)  # valid config
     model = Module(config)
     dm = Datamodule(config)
     dm.setup()
     model.eval()
 
-    exp_name = f"{config['exp_name']}"
-    logger = pl.loggers.TensorBoardLogger(
-        config["log_dir"],
-        name=f'prediction_{exp_name}_seed{config["seed"]}_from_{str(config["load_path"]).split("/")[-1][:-5]}',
-    )
-
-    # gradient accumulation
-    if num_device == 0:
-        accumulate_grad_batches = config["batch_size"] // (
-                config["per_gpu_batchsize"]
-        )
-    else:
-        accumulate_grad_batches = config["batch_size"] // (
-                config["per_gpu_batchsize"]
-        )
-
-    max_steps = config["max_steps"] if config["max_steps"] is not None else None
-
     if _IS_INTERACTIVE:
         strategy = None
     elif pl.__version__ >= '2.0.0':
         strategy = "ddp_find_unused_parameters_true"
     else:
         strategy = "ddp"
 
     trainer = pl.Trainer(
         accelerator=config['accelerator'],
         devices=config["devices"],
         num_nodes=config["num_nodes"],
         precision=config["precision"],
         strategy=strategy,
         benchmark=True,
-        max_steps=max_steps,
-        accumulate_grad_batches=accumulate_grad_batches,
+        max_epochs=1,
+        log_every_n_steps=0,
         deterministic=True,
-        logger=logger,
+        logger=False,
     )
 
     # refine split
     split = config.get('split', 'all')
     if split == 'all':
         split = ['train', 'val', 'test']
     elif isinstance(split, str):
```

### Comparing `moftransformer-2.1.0/moftransformer/run.py` & `moftransformer-2.1.1/moftransformer/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # MOFTransformer version 2.1.0
 import sys
 import os
 import copy
 import warnings
+from pathlib import Path
+import shutil
 
 import pytorch_lightning as pl
 
 from moftransformer.config import ex
 from moftransformer.config import config as _config
 from moftransformer.datamodules.datamodule import Datamodule
 from moftransformer.modules.module import Module
@@ -281,9 +283,13 @@
         log_every_n_steps=log_every_n_steps,
         val_check_interval=_config["val_check_interval"],
         deterministic=True,
     )
 
     if not _config["test_only"]:
         trainer.fit(model, datamodule=dm, ckpt_path=_config["resume_from"])
+        log_dir = Path(logger.log_dir)/'checkpoints'
+        if best_model:= next(log_dir.glob('epoch=*.ckpt')):
+            shutil.copy(best_model, log_dir/'best.ckpt')
+            
     else:
         trainer.test(model, datamodule=dm)
```

### Comparing `moftransformer-2.1.0/moftransformer/utils/download.py` & `moftransformer-2.1.1/moftransformer/utils/download.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/utils/install_griday.py` & `moftransformer-2.1.1/moftransformer/utils/install_griday.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/utils/prepare_data.py` & `moftransformer-2.1.1/moftransformer/utils/prepare_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,14 +290,15 @@
             dest = root_dataset / split
             shutil.copy(src, dest)
 
 
 def _split_json(root_cifs: Path, root_dataset: Path, downstream: str):
     with open(str(root_cifs / f"raw_{downstream}.json")) as f:
         src = json.load(f)
+        src = {i.replace(".cif", ""):v for i, v in src.items()}  # if *.cif in JSON files
 
     for split in ["train", "test", "val"]:
         cif_folder = root_dataset / split
         cif_list = [cif.stem for cif in cif_folder.glob("*.cif")]
         split_json = {i: src[i] for i in cif_list if i in src}
         with open(str(root_dataset / f"{split}_{downstream}.json"), "w") as f:
             json.dump(split_json, f)
```

### Comparing `moftransformer-2.1.0/moftransformer/utils/validation.py` & `moftransformer-2.1.1/moftransformer/utils/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# MOFTransformer version 2.1.0
+# MOFTransformer version 2.1.1
 import sys
 import warnings
 import pytorch_lightning as pl
 from moftransformer.database import DEFAULT_PMTRANSFORMER_PATH, DEFAULT_MOFTRANSFORMER_PATH
 
 if pl.__version__ >= '2.0.0':
     from pytorch_lightning.trainer.connectors.accelerator_connector import _AcceleratorConnector as AC
@@ -55,15 +55,15 @@
         return DEFAULT_MOFTRANSFORMER_PATH
     elif not path:
         return ""
     elif str(path)[-4:] == 'ckpt':
         return path
     else:
         raise ConfigurationError(
-            "path must be 'pmtransformer', 'moftransformer', None, or *.ckpt, not {path}"
+            f"path must be 'pmtransformer', 'moftransformer', None, or *.ckpt, not {path}"
         )
 
 
 def get_num_devices(_config):
     if isinstance(devices := _config["devices"], list):
         devices = len(devices)
     elif isinstance(devices, int):
@@ -95,21 +95,23 @@
 
 
 def _check_valid_num_gpus(_config):
     devices = get_num_devices(_config)
 
     if devices > _config["batch_size"]:
         raise ConfigurationError(
-            "Number of devices must be smaller than batch_size."
+            "Number of devices must be smaller than batch_size. "
             f'num_gpus : {devices}, batch_size : {_config["batch_size"]}'
         )
 
     if _IS_INTERACTIVE and devices > 1:
-        raise ConfigurationError(
-            "The interactive environment (ex. jupyter notebook) does not supports multi-devices environment."
+        _config["devices"] = 1
+        warnings.warn(
+            "The interactive environment (ex. jupyter notebook) does not supports multi-devices environment. "
+            f"Adjusted number of devices : {devices} to 1. "
             "If you want to use multi-devices, make *.py file and run."
         )
     
     return devices
 
 
 def get_valid_config(_config):
```

### Comparing `moftransformer-2.1.0/moftransformer/visualize/drawer.py` & `moftransformer-2.1.1/moftransformer/visualize/drawer.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/visualize/setting.py` & `moftransformer-2.1.1/moftransformer/visualize/setting.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/visualize/utils.py` & `moftransformer-2.1.1/moftransformer/visualize/utils.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer/visualize/visualizer.py` & `moftransformer-2.1.1/moftransformer/visualize/visualizer.py`

 * *Files identical despite different names*

### Comparing `moftransformer-2.1.0/moftransformer.egg-info/PKG-INFO` & `moftransformer-2.1.1/moftransformer.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: moftransformer
-Version: 2.1.0
+Version: 2.1.1
 Summary: moftransformer
 Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer
 Author: Yeonghun Kang, Hyunsoo Park
 Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 
 ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/docs/source/assets/fig1.jpg)
 
 <p align="center">
  <a href="https://hspark1212.github.io/MOFTransformer/">
-     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.0-brightgreen.svg?style=plastic">
+     <img alt="Docs" src="https://img.shields.io/badge/Docs-v2.1.1-brightgreen.svg?style=plastic">
  </a>
   <a href="https://pypi.org/project/moftransformer/">
-     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.0-blue.svg?style=plastic&logo=PyPI">
+     <img alt="PypI" src="https://img.shields.io/badge/PyPI-v2.1.1-blue.svg?style=plastic&logo=PyPI">
  </a>
   <a href="https://doi.org/10.6084/m9.figshare.21155506.v2">
      <img alt="Figshare" src="https://img.shields.io/badge/Figshare-v2-blue.svg?style=plastic&logo=figshare">
  </a>
  <a href="https://doi.org/10.5281/zenodo.7593333">
      <img alt="DOI" src="https://img.shields.io/badge/DOI-doi-organge.svg?style=plastic">
  </a>
@@ -35,14 +35,16 @@
  This package provides a universal transfer learning model, `PMTransformer` (Porous Materials Transformer), which obtains the state-of-the-art performance in predicting various properties of porous materials. The PMTRansformer was pre-trainied with 1.9 million hypothetical porous materials including Metal-Organic Frameworks (MOFs), Covalent-Organic Frameworks (COFs), Porous Polymer Networks (PPNs), and zeolites. By fine-tuning the pre-trained `PMTransformer`, you can easily obtain machine learning models to accurately predict various properties of porous materials .
  
  NOTE: From version 2.0.0, the default pre-training model has been changed from `MOFTransformer` to `PMTransformer`, which was pre-trained with a larger dataset, containing other porous materials as well as MOFs. The `PMTransformer` outperforms the `MOFTransformer` in predicting various properties of porous materials.
 
 ## [Install](https://hspark1212.github.io/MOFTransformer/installation.html)
 
 ### Depedencies
+NOTE: This package is primarily tested on Linux. We strongly recommend using Linux for the installation.
+
 ```
 python>=3.8
 ```
 Given that MOFTransformer is based on pytorch, please install pytorch (>= 1.12.0) according to your environments.
 
 ### Installation using PIP 
 ```
@@ -70,23 +72,89 @@
 ```
 2. Fine-tune the pretrained MOFTransformer.
 ```python
 import moftransformer
 from moftransformer.examples import example_path
 
 # data root and downstream from example
-data_root = example_path['data_root']
+root_dataset = example_path['root_dataset']
 downstream = example_path['downstream']
 log_dir = './logs/'
 # load_path = "pmtransformer" (default)
 
-moftransformer.run(data_root, downstream, log_dir=log_dir, 
-                   max_epochs=max_epochs, batch_size=batch_size,)
+# kwargs (optional)
+max_epochs = 10
+batch_size = 8
+mean = 0
+std = 1
+
+
+moftransformer.run(root_dataset, downstream, log_dir=log_dir,                   
+                   max_epochs=max_epochs, batch_size=batch_size,
+                   mean=mean, std=std)
 ```
-3. Visualize analysis of feature importance for the fine-tuned model.
+
+3. Test fine-tuned model
+```python
+from pathlib import Path
+import moftransformer
+from moftransformer.examples import example_path
+
+root_dataset = example_path['root_dataset']
+downstream = example_path['downstream']
+
+# Get ckpt file
+seed = 0               # default seeds
+version = 0            # version for model. It increases with the number of trains
+
+# For version > 2.1.1, best.ckpt exists
+checkpoint = 'best'    # Epochs where the model is stored. 
+save_dir = 'result/'
+
+# optional keyword
+mean = 0
+std = 1
+
+load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/version_{version}/checkpoints/{checkpoint}.ckpt'
+
+if not load_path.exists():
+    raise ValueError(f'load_path does not exists. check path for .ckpt file : {load_path}')
+
+moftransformer.test(root_dataset, load_path, downstream=downstream,
+                   save_dir=save_dir, mean=mean, std=std)
+```
+
+4. predict from fine-tuned model
+```python
+from pathlib import Path
+import moftransformer
+from moftransformer.examples import example_path
+
+root_dataset = example_path['root_dataset']
+downstream = example_path['downstream']
+
+# Get ckpt file
+log_dir = './logs/'    # same directory make from training
+seed = 0               # default seeds
+version = 0            # version for model. It increases with the number of trains
+checkpoint = 'best'    # Epochs where the model is stored. 
+mean = 0
+std = 1
+
+load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/version_{version}/checkpoints/{checkpoint}.ckpt'
+
+if not load_path.exists():
+    raise ValueError(f'load_path does not exists. check path for .ckpt file : {load_path}')
+    
+moftransformer.predict(
+    root_dataset, load_path=load_path, downstream=downstream, split='all', mean=mean, std=std
+)
+```
+
+5. Visualize analysis of feature importance for the fine-tuned model.
 ```python
 %matplotlib widget
 from visualize import PatchVisualizer
 
 model_path = "examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
 data_path = 'examples/visualize/dataset/'
 cifname = 'MIBQAR01_FSR'
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: moftransformer Version: 2.1.0 Summary:
+Metadata-Version: 2.1 Name: moftransformer Version: 2.1.1 Summary:
 moftransformer Home-page: https://hspark1212.github.io/MOFTransformer/
 Download-URL: https://github.com/hspark1212/MOFTransformer Author: Yeonghun
 Kang, Hyunsoo Park Author-email: dudgns1675@kaist.ac.kr, phs68660888@gmail.com
 Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
 docs ![](https://raw.githubusercontent.com/hspark1212/MOFTransformer/master/
 docs/source/assets/fig1.jpg)
                    [Docs] [PypI] [Figshare] [DOI] [Lincense]
@@ -16,37 +16,62 @@
 `PMTransformer`, you can easily obtain machine learning models to accurately
 predict various properties of porous materials . NOTE: From version 2.0.0, the
 default pre-training model has been changed from `MOFTransformer` to
 `PMTransformer`, which was pre-trained with a larger dataset, containing other
 porous materials as well as MOFs. The `PMTransformer` outperforms the
 `MOFTransformer` in predicting various properties of porous materials. ##
 [Install](https://hspark1212.github.io/MOFTransformer/installation.html) ###
-Depedencies ``` python>=3.8 ``` Given that MOFTransformer is based on pytorch,
-please install pytorch (>= 1.12.0) according to your environments. ###
-Installation using PIP ``` $ pip install moftransformer ``` ### Download the
-pretrained models (ckpt file) - you can download the pretrained models
-(`PMTransformer.ckpt` and `MOFTransformer.ckpt`) via [figshare](https://
-figshare.com/articles/dataset/PMTransformer_pre-trained_model/22698655/2) or
-you can download with a command line: ``` $ moftransformer download
-pretrain_model ``` ### (Optional) Download pre-embeddings for CoREMOF, QMOF -
-we've provide the pre-embeddings (i.e., atom-based graph embeddings and energy-
-grid embeddings), inputs of `PMTransformer`, for CoREMOF, QMOF database. ``` $
-moftransformer download coremof $ moftransformer download qmof ``` ## [Getting
-Started](https://hspark1212.github.io/MOFTransformer/tutorial.html) 1. At
-first, you download dataset of hMOFs (20,000 MOFs) as an example. ``` $
-moftransformer download hmof ``` 2. Fine-tune the pretrained MOFTransformer.
-```python import moftransformer from moftransformer.examples import
-example_path # data root and downstream from example data_root = example_path
-['data_root'] downstream = example_path['downstream'] log_dir = './logs/' #
-load_path = "pmtransformer" (default) moftransformer.run(data_root, downstream,
-log_dir=log_dir, max_epochs=max_epochs, batch_size=batch_size,) ``` 3.
-Visualize analysis of feature importance for the fine-tuned model. ```python
-%matplotlib widget from visualize import PatchVisualizer model_path =
-"examples/finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt'
-data_path = 'examples/visualize/dataset/' cifname = 'MIBQAR01_FSR' vis =
+Depedencies NOTE: This package is primarily tested on Linux. We strongly
+recommend using Linux for the installation. ``` python>=3.8 ``` Given that
+MOFTransformer is based on pytorch, please install pytorch (>= 1.12.0)
+according to your environments. ### Installation using PIP ``` $ pip install
+moftransformer ``` ### Download the pretrained models (ckpt file) - you can
+download the pretrained models (`PMTransformer.ckpt` and `MOFTransformer.ckpt`)
+via [figshare](https://figshare.com/articles/dataset/PMTransformer_pre-
+trained_model/22698655/2) or you can download with a command line: ``` $
+moftransformer download pretrain_model ``` ### (Optional) Download pre-
+embeddings for CoREMOF, QMOF - we've provide the pre-embeddings (i.e., atom-
+based graph embeddings and energy-grid embeddings), inputs of `PMTransformer`,
+for CoREMOF, QMOF database. ``` $ moftransformer download coremof $
+moftransformer download qmof ``` ## [Getting Started](https://
+hspark1212.github.io/MOFTransformer/tutorial.html) 1. At first, you download
+dataset of hMOFs (20,000 MOFs) as an example. ``` $ moftransformer download
+hmof ``` 2. Fine-tune the pretrained MOFTransformer. ```python import
+moftransformer from moftransformer.examples import example_path # data root and
+downstream from example root_dataset = example_path['root_dataset'] downstream
+= example_path['downstream'] log_dir = './logs/' # load_path = "pmtransformer"
+(default) # kwargs (optional) max_epochs = 10 batch_size = 8 mean = 0 std = 1
+moftransformer.run(root_dataset, downstream, log_dir=log_dir,
+max_epochs=max_epochs, batch_size=batch_size, mean=mean, std=std) ``` 3. Test
+fine-tuned model ```python from pathlib import Path import moftransformer from
+moftransformer.examples import example_path root_dataset = example_path
+['root_dataset'] downstream = example_path['downstream'] # Get ckpt file seed =
+0 # default seeds version = 0 # version for model. It increases with the number
+of trains # For version > 2.1.1, best.ckpt exists checkpoint = 'best' # Epochs
+where the model is stored. save_dir = 'result/' # optional keyword mean = 0 std
+= 1 load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/
+version_{version}/checkpoints/{checkpoint}.ckpt' if not load_path.exists():
+raise ValueError(f'load_path does not exists. check path for .ckpt file :
+{load_path}') moftransformer.test(root_dataset, load_path,
+downstream=downstream, save_dir=save_dir, mean=mean, std=std) ``` 4. predict
+from fine-tuned model ```python from pathlib import Path import moftransformer
+from moftransformer.examples import example_path root_dataset = example_path
+['root_dataset'] downstream = example_path['downstream'] # Get ckpt file
+log_dir = './logs/' # same directory make from training seed = 0 # default
+seeds version = 0 # version for model. It increases with the number of trains
+checkpoint = 'best' # Epochs where the model is stored. mean = 0 std = 1
+load_path = Path(log_dir) / f'pretrained_mof_seed{seed}_from_pmtransformer/
+version_{version}/checkpoints/{checkpoint}.ckpt' if not load_path.exists():
+raise ValueError(f'load_path does not exists. check path for .ckpt file :
+{load_path}') moftransformer.predict( root_dataset, load_path=load_path,
+downstream=downstream, split='all', mean=mean, std=std ) ``` 5. Visualize
+analysis of feature importance for the fine-tuned model. ```python %matplotlib
+widget from visualize import PatchVisualizer model_path = "examples/
+finetuned_bandgap.ckpt" # or 'examples/finetuned_h2_uptake.ckpt' data_path =
+'examples/visualize/dataset/' cifname = 'MIBQAR01_FSR' vis =
 PatchVisualizer.from_cifname(cifname, model_path, data_path) vis.draw_graph() #
 or vis.draw_grid() ``` ## [Architecture](https://hspark1212.github.io/
 MOFTransformer/introduction.html) It is a multi-modal pre-training Transformer
 encoder which is designed to capture both local and global features of porous
 materials. The pre-traning tasks are as follows: (1) Topology Prediction (2)
 Void Fraction Prediction (3) Building Block Classification It takes two
 different representations as input - Atom-based Graph Embedding : CGCNN w/
```

### Comparing `moftransformer-2.1.0/moftransformer.egg-info/SOURCES.txt` & `moftransformer-2.1.1/moftransformer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 README.md
 setup.py
 moftransformer/__init__.py
 moftransformer/config.py
 moftransformer/config_ex.py
 moftransformer/predict.py
 moftransformer/run.py
+moftransformer/test.py
 moftransformer.egg-info/PKG-INFO
 moftransformer.egg-info/SOURCES.txt
 moftransformer.egg-info/dependency_links.txt
 moftransformer.egg-info/entry_points.txt
 moftransformer.egg-info/requires.txt
 moftransformer.egg-info/top_level.txt
 moftransformer/assets/__init__.py
 moftransformer/assets/bbs.json
 moftransformer/assets/colors.py
 moftransformer/assets/topology.json
 moftransformer/cli/__init__.py
 moftransformer/cli/download.py
 moftransformer/cli/install_griday.py
 moftransformer/cli/main.py
+moftransformer/cli/predict.py
 moftransformer/cli/run.py
+moftransformer/cli/test.py
 moftransformer/cli/uninstall_griday.py
 moftransformer/database/__init__.py
 moftransformer/datamodules/__init__.py
 moftransformer/datamodules/datamodule.py
 moftransformer/datamodules/dataset.py
 moftransformer/examples/__init__.py
 moftransformer/examples/dataset/test_example.json
```

### Comparing `moftransformer-2.1.0/setup.py` & `moftransformer-2.1.1/setup.py`

 * *Files identical despite different names*

