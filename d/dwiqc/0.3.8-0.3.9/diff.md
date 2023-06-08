# Comparing `tmp/dwiqc-0.3.8-py2.py3-none-any.whl.zip` & `tmp/dwiqc-0.3.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
 Zip file size: 24317 bytes, number of entries: 22
 -rw-r--r--  2.0 unx      225 b- defN 23-May-31 00:20 dwiqc/__init__.py
--rw-r--r--  2.0 unx      247 b- defN 23-May-31 10:08 dwiqc/__version__.py
+-rw-r--r--  2.0 unx      247 b- defN 23-May-31 14:57 dwiqc/__version__.py
 -rw-r--r--  2.0 unx      283 b- defN 23-May-31 00:20 dwiqc/browser/__init__.py
 -rw-r--r--  2.0 unx       62 b- defN 23-May-31 00:20 dwiqc/cli/__init__.py
 -rw-r--r--  2.0 unx     6651 b- defN 23-May-31 00:20 dwiqc/cli/get.py
 -rw-r--r--  2.0 unx     5597 b- defN 23-May-31 00:21 dwiqc/cli/process.py
 -rw-r--r--  2.0 unx     3722 b- defN 23-May-31 00:20 dwiqc/cli/tandem.py
 -rw-r--r--  2.0 unx      160 b- defN 23-May-31 00:20 dwiqc/config/__init__.py
 -rw-r--r--  2.0 unx      274 b- defN 23-May-31 00:20 dwiqc/config/dwiqc.yaml
 -rw-r--r--  2.0 unx       98 b- defN 23-May-31 00:20 dwiqc/state/__init__.py
 -rw-r--r--  2.0 unx     1892 b- defN 23-May-31 00:20 dwiqc/tasks/__init__.py
 -rw-r--r--  2.0 unx    10168 b- defN 23-May-31 00:20 dwiqc/tasks/prequal.py
 -rw-r--r--  2.0 unx     4483 b- defN 23-May-31 00:20 dwiqc/tasks/prequal_EQ.py
--rw-r--r--  2.0 unx     6146 b- defN 23-May-31 10:01 dwiqc/tasks/qsiprep.py
+-rw-r--r--  2.0 unx     6146 b- defN 23-May-31 16:20 dwiqc/tasks/qsiprep.py
 -rw-r--r--  2.0 unx     3872 b- defN 23-May-31 00:20 dwiqc/tasks/qsiprep_EQ.py
--rw-r--r--  2.0 unx    16453 b- defN 23-May-31 09:50 dwiqc/xnat/__init__.py
--rwxr-xr-x  2.0 unx     5766 b- defN 23-May-31 10:09 dwiqc-0.3.8.data/scripts/dwiQC.py
--rw-r--r--  2.0 unx     1541 b- defN 23-May-31 10:09 dwiqc-0.3.8.dist-info/LICENSE
--rw-r--r--  2.0 unx      432 b- defN 23-May-31 10:09 dwiqc-0.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-31 10:09 dwiqc-0.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-31 10:09 dwiqc-0.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1717 b- defN 23-May-31 10:09 dwiqc-0.3.8.dist-info/RECORD
+-rw-r--r--  2.0 unx    16453 b- defN 23-May-31 13:49 dwiqc/xnat/__init__.py
+-rwxr-xr-x  2.0 unx     5766 b- defN 23-May-31 16:21 dwiqc-0.3.9.data/scripts/dwiQC.py
+-rw-r--r--  2.0 unx     1541 b- defN 23-May-31 16:21 dwiqc-0.3.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      432 b- defN 23-May-31 16:21 dwiqc-0.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-31 16:21 dwiqc-0.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-31 16:21 dwiqc-0.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1717 b- defN 23-May-31 16:21 dwiqc-0.3.9.dist-info/RECORD
 22 files, 69905 bytes uncompressed, 21565 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: dwiqc/tasks/qsiprep_EQ.py
 Comment: 
 
 Filename: dwiqc/xnat/__init__.py
 Comment: 
 
-Filename: dwiqc-0.3.8.data/scripts/dwiQC.py
+Filename: dwiqc-0.3.9.data/scripts/dwiQC.py
 Comment: 
 
-Filename: dwiqc-0.3.8.dist-info/LICENSE
+Filename: dwiqc-0.3.9.dist-info/LICENSE
 Comment: 
 
-Filename: dwiqc-0.3.8.dist-info/METADATA
+Filename: dwiqc-0.3.9.dist-info/METADATA
 Comment: 
 
-Filename: dwiqc-0.3.8.dist-info/WHEEL
+Filename: dwiqc-0.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: dwiqc-0.3.8.dist-info/top_level.txt
+Filename: dwiqc-0.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: dwiqc-0.3.8.dist-info/RECORD
+Filename: dwiqc-0.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dwiqc/__version__.py

```diff
@@ -1,6 +1,6 @@
 __title__ = 'dwiqc'
 __description__ = 'Quality Assurance Pipeline for Diffusion MR Data'
 __url__ = 'https://github.com/harvard-nrg/dwiqc'
-__version__ = '0.3.8'
+__version__ = '0.3.9'
 __author__ = 'Neuroinformatics Research Group'
 __author_email__ = 'info@neuroinfo.org'
```

## dwiqc/tasks/qsiprep.py

```diff
@@ -189,15 +189,15 @@
 			"use_cuda": True,
 			"cnr_maps": True,
 			"residuals": True,
 			"output_type": "NIFTI_GZ",
 			"estimate_move_by_susceptibility": True,
 			"mporder": mporder,
 			"slice_order": f"{self._bids}/{spec_file}",
-			"args": "--ol_nstd=4 --ol_type=gw"
+			"args": "--ol_nstd=5 --ol_type=gw"
 		}
 
 		with open(f"{self._bids}/eddy_params_s2v_mbs.json", "w") as f:
 			json.dump(params_file, f)
 
 	# create qsiprep command to be executed
 
@@ -208,14 +208,16 @@
 		self._command = [
 			'selfie',
 			'--lock',
 			'--output-file', self._prov,
 			'singularity',
 			'run',
 			'--nv',
+			'-B',
+			'/n/sw/helmod-rocky8/apps/Core/cuda/9.1.85-fasrc01:/usr/local/cuda',
 			'/n/sw/ncf/apps/qsiprep/0.14.0/qsiprep.sif',			
 			self._bids,
 			self._outdir,
 			'participant',
 			'--output-resolution',
 			self._output_resolution,
 			'--separate-all-dwis',
@@ -229,17 +231,15 @@
 			'--n_cpus',
 			'2',
 			'--mem_mb',
 			'40000',
 			'--fs-license-file',
 			'/n/helmod/apps/centos7/Core/freesurfer/6.0.0-fasrc01/license.txt',
 			'-w',
-			self._tempdir,
-			'-B',
-			'/n/sw/helmod-rocky8/apps/Core/cuda/9.1.85-fasrc01:/usr/local/cuda'
+			self._tempdir
 		]
 
 		logdir = self.logdir()
 		logfile = os.path.join(logdir, 'dwiqc-qsiprep.log')
 		self.job = Job(
 			name='dwiqc-qsiprep',
 			time='2000',
```

## dwiqc/xnat/__init__.py

```diff
@@ -189,19 +189,19 @@
                 'dest': os.path.join('t1-registration', '{0}_t1_registration.svg'.format(aid))
             },
             {
                 'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_seg_brainmask.svg'),
                 'dest': os.path.join('seg-brainmask', '{0}_seg_brainmask.svg'.format(aid))
             },
             {
-                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + str(self.run) + '_dwi_denoise_ses_' + self.ses + '_run-' + str(self.run) + '_dwi_wf_denoising.svg'),
+                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + str(self.run) + '_dwi_denoise_ses_' + self.ses + '_run_' + str(self.run) + '_dwi_wf_denoising.svg'),
                 'dest': os.path.join('denoise', '{0}_denoise.svg'.format(aid))
             },
             {
-                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + str(self.run) + '_dwi_denoise_ses_' + self.ses + '_run-' + str(self.run) + '_dwi_wf_biascorr.svg'),
+                'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + str(self.run) + '_dwi_denoise_ses_' + self.ses + '_run_' + str(self.run) + '_dwi_wf_biascorr.svg'),
                 'dest': os.path.join('bias-corr', '{0}_bias_correction.svg'.format(aid))
             },
             {
                 'source': os.path.join(self.dirs['qsiprep'], 'qsiprep_output', 'qsiprep',  self.sub, 'figures', self.sub + '_ses-' + self.ses + '_run-' + str(self.run) + '_desc-resampled_b0ref.svg'),
                 'dest': os.path.join('b0-ref', '{0}_b0_reference.svg'.format(aid))
             },
             {
```

## Comparing `dwiqc-0.3.8.data/scripts/dwiQC.py` & `dwiqc-0.3.9.data/scripts/dwiQC.py`

 * *Files identical despite different names*

## Comparing `dwiqc-0.3.8.dist-info/LICENSE` & `dwiqc-0.3.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dwiqc-0.3.8.dist-info/RECORD` & `dwiqc-0.3.9.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 dwiqc/__init__.py,sha256=MZJhUZKhHHoZ2w_GeoFCITk1m_0ASdRw_ZaeDixFEPU,225
-dwiqc/__version__.py,sha256=KX9iCGe3tW9m_TkxqPqM9ZDezrLXea3qu0Tu_bxgG74,247
+dwiqc/__version__.py,sha256=GQPOtrp57z13rm-ZZXfGx96p4-KPexos6RdmDuSDSlw,247
 dwiqc/browser/__init__.py,sha256=MlUOz0v7bA_dtQyXX27WF0dzyGGo4xkEEt2PT2B0_aQ,283
 dwiqc/cli/__init__.py,sha256=zGIm7lrjh3wA191D-VjQBZNjSlspFUx148VwDNQGaTk,62
 dwiqc/cli/get.py,sha256=6ixaBdwEgY_GXh8L-_3QDY4MEsNqSJgXle_mxW99mlk,6651
 dwiqc/cli/process.py,sha256=-f2OK3WAc9cwTygv_aM0dawyGT_I3TSI24QBL0TIGdA,5597
 dwiqc/cli/tandem.py,sha256=_lSryhvKIzRRdnBnwfKPdfSBV98JwDfz6lzbqETQ3rw,3722
 dwiqc/config/__init__.py,sha256=k_w5JzoJN_7R7eI_sIJxHA4FQQHs0_KGf-6jsbG4Xs8,160
 dwiqc/config/dwiqc.yaml,sha256=x8gKMFZyChdzvNX3GthRe0eWvyKDDL5itXo0kLWVfd0,274
 dwiqc/state/__init__.py,sha256=NaRifw26bI3F1J9BqeLa-KLSzEPq2m_UNhMbXdmPdh4,98
 dwiqc/tasks/__init__.py,sha256=LnlN7iYjpqiBic2ihFrM-_h7m8FD_N7Beh7UIwKyGZ8,1892
 dwiqc/tasks/prequal.py,sha256=jQsq46tK9UdCtKW7iqh2VD9JsA3BKZ7Pp4pzCBCt0hM,10168
 dwiqc/tasks/prequal_EQ.py,sha256=cV3V6WP1_YHLz5dtwWGxS_HPdtbqnra2xT64-_TEdj0,4483
-dwiqc/tasks/qsiprep.py,sha256=W8XdWFzqsfPq4gLGTAlpUb1yXtogCPj0-rPVV0unmBE,6146
+dwiqc/tasks/qsiprep.py,sha256=CWalSV29PeSXhPANLR6MQiH6eAAFaaN6PxDITnTZ3Pw,6146
 dwiqc/tasks/qsiprep_EQ.py,sha256=oj9kJ4hRBlq8mT4Mp-ogakoOTVFbfJ2yUxcwoXPN4j8,3872
-dwiqc/xnat/__init__.py,sha256=5LJWoH7dIadKg7QNXq4-xcWh0Er22MKUJuEeDoNXRmA,16453
-dwiqc-0.3.8.data/scripts/dwiQC.py,sha256=76M57U-wyP0Webb3Q_KiQbK4setkfGpXjhKVFUHu9SY,5766
-dwiqc-0.3.8.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
-dwiqc-0.3.8.dist-info/METADATA,sha256=ErwhhYYLnxQWccpzrgsj-pPJm5k32ISFDWOFOLgazTU,432
-dwiqc-0.3.8.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
-dwiqc-0.3.8.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
-dwiqc-0.3.8.dist-info/RECORD,,
+dwiqc/xnat/__init__.py,sha256=D0e9MjRWxfFWF2zE2p8ckH0EDYikLk3VRte5lMFEklY,16453
+dwiqc-0.3.9.data/scripts/dwiQC.py,sha256=76M57U-wyP0Webb3Q_KiQbK4setkfGpXjhKVFUHu9SY,5766
+dwiqc-0.3.9.dist-info/LICENSE,sha256=ReOF9BmlQdkCj4b2gQYogJrk_QkbUAuz8W1ZVqI0pcs,1541
+dwiqc-0.3.9.dist-info/METADATA,sha256=Ntwubtr8lKsQxzKtpdJIro6dxwpjbgtDAFO4_BdU52k,432
+dwiqc-0.3.9.dist-info/WHEEL,sha256=z9j0xAa_JmUKMpmz72K0ZGALSM_n-wQVmGbleXx2VHg,110
+dwiqc-0.3.9.dist-info/top_level.txt,sha256=omH7pmKt7fzFyiNkTPDLX4yyBccoge5Saqc9rgyu0Wk,6
+dwiqc-0.3.9.dist-info/RECORD,,
```

