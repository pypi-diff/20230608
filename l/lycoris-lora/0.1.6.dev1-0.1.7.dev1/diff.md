# Comparing `tmp/lycoris_lora-0.1.6.dev1.tar.gz` & `tmp/lycoris_lora-0.1.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-0.1.6.dev1.tar", last modified: Sun Apr 16 15:51:22 2023, max compression
+gzip compressed data, was "lycoris_lora-0.1.7.dev1.tar", last modified: Thu Jun  8 06:59:36 2023, max compression
```

## Comparing `lycoris_lora-0.1.6.dev1.tar` & `lycoris_lora-0.1.7.dev1.tar`

### file list

```diff
@@ -1,42 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.484260 lycoris_lora-0.1.6.dev1/
--rw-rw-rw-   0        0        0     1623 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-0.1.6.dev1/Algo.md
--rw-rw-rw-   0        0        0      552 2023-03-29 07:12:55.000000 lycoris_lora-0.1.6.dev1/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-0.1.6.dev1/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/LICENSE.md
--rw-rw-rw-   0        0        0      353 2023-04-16 15:51:22.484260 lycoris_lora-0.1.6.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     6498 2023-04-10 10:28:19.000000 lycoris_lora-0.1.6.dev1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.470741 lycoris_lora-0.1.6.dev1/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-0.1.6.dev1/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-0.1.6.dev1/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-0.1.6.dev1/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-0.1.6.dev1/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-0.1.6.dev1/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-0.1.6.dev1/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-0.1.6.dev1/experiments/time_test.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.475241 lycoris_lora-0.1.6.dev1/lycoris/
--rw-rw-rw-   0        0        0      113 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2514 2023-04-11 15:07:08.000000 lycoris_lora-0.1.6.dev1/lycoris/config.py
--rw-rw-rw-   0        0        0     6222 2023-04-16 14:58:02.000000 lycoris_lora-0.1.6.dev1/lycoris/dylora.py
--rw-rw-rw-   0        0        0     2103 2023-04-04 08:21:48.000000 lycoris_lora-0.1.6.dev1/lycoris/ia3.py
--rw-rw-rw-   0        0        0    21664 2023-04-16 14:10:06.000000 lycoris_lora-0.1.6.dev1/lycoris/kohya.py
--rw-rw-rw-   0        0        0    48868 2023-04-09 15:10:02.000000 lycoris_lora-0.1.6.dev1/lycoris/kohya_model_utils.py
--rw-rw-rw-   0        0        0     1512 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/lycoris/kohya_utils.py
--rw-rw-rw-   0        0        0     3178 2023-04-07 16:38:33.000000 lycoris_lora-0.1.6.dev1/lycoris/locon.py
--rw-rw-rw-   0        0        0     7657 2023-04-07 16:38:27.000000 lycoris_lora-0.1.6.dev1/lycoris/loha.py
--rw-rw-rw-   0        0        0     8974 2023-04-08 05:53:19.000000 lycoris_lora-0.1.6.dev1/lycoris/lokr.py
--rw-rw-rw-   0        0        0    20963 2023-04-10 16:04:23.000000 lycoris_lora-0.1.6.dev1/lycoris/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.483260 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      353 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      791 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-16 15:51:22.000000 lycoris_lora-0.1.6.dev1/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2023-03-09 05:37:07.000000 lycoris_lora-0.1.6.dev1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-16 15:51:22.484260 lycoris_lora-0.1.6.dev1/setup.cfg
--rw-rw-rw-   0        0        0      547 2023-04-16 15:51:09.000000 lycoris_lora-0.1.6.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-16 15:51:22.483760 lycoris_lora-0.1.6.dev1/tools/
--rw-rw-rw-   0        0        0     4087 2023-03-12 16:11:52.000000 lycoris_lora-0.1.6.dev1/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-04-10 15:31:09.000000 lycoris_lora-0.1.6.dev1/tools/merge.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2023-06-08 06:59:36.248775 lycoris_lora-0.1.7.dev1/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    11344 2023-03-09 06:17:28.000000 lycoris_lora-0.1.7.dev1/LICENSE.md
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      345 2023-06-08 06:59:36.248624 lycoris_lora-0.1.7.dev1/PKG-INFO
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     7228 2023-06-08 06:27:42.000000 lycoris_lora-0.1.7.dev1/README.md
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2023-06-08 06:59:36.240374 lycoris_lora-0.1.7.dev1/lycoris/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      106 2023-03-09 06:17:28.000000 lycoris_lora-0.1.7.dev1/lycoris/__init__.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     6048 2023-06-08 06:27:42.000000 lycoris_lora-0.1.7.dev1/lycoris/dylora.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     2036 2023-06-08 06:27:42.000000 lycoris_lora-0.1.7.dev1/lycoris/ia3.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    21843 2023-06-08 06:55:21.000000 lycoris_lora-0.1.7.dev1/lycoris/kohya.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    47703 2023-06-08 06:27:42.000000 lycoris_lora-0.1.7.dev1/lycoris/kohya_model_utils.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     1465 2023-03-09 06:17:28.000000 lycoris_lora-0.1.7.dev1/lycoris/kohya_utils.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     3705 2023-06-08 06:56:30.000000 lycoris_lora-0.1.7.dev1/lycoris/locon.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     8121 2023-06-08 06:58:19.000000 lycoris_lora-0.1.7.dev1/lycoris/loha.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)     9768 2023-06-08 06:58:09.000000 lycoris_lora-0.1.7.dev1/lycoris/lokr.py
+-rw-r--r--   0 kblueleaf   (501) staff       (20)    20459 2023-06-08 06:27:42.000000 lycoris_lora-0.1.7.dev1/lycoris/utils.py
+drwxr-xr-x   0 kblueleaf   (501) staff       (20)        0 2023-06-08 06:59:36.248452 lycoris_lora-0.1.7.dev1/lycoris_lora.egg-info/
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      345 2023-06-08 06:59:36.000000 lycoris_lora-0.1.7.dev1/lycoris_lora.egg-info/PKG-INFO
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      431 2023-06-08 06:59:36.000000 lycoris_lora-0.1.7.dev1/lycoris_lora.egg-info/SOURCES.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2023-06-08 06:59:36.000000 lycoris_lora-0.1.7.dev1/lycoris_lora.egg-info/dependency_links.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        1 2023-03-09 06:17:38.000000 lycoris_lora-0.1.7.dev1/lycoris_lora.egg-info/not-zip-safe
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       41 2023-06-08 06:59:36.000000 lycoris_lora-0.1.7.dev1/lycoris_lora.egg-info/requires.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)        8 2023-06-08 06:59:36.000000 lycoris_lora-0.1.7.dev1/lycoris_lora.egg-info/top_level.txt
+-rw-r--r--   0 kblueleaf   (501) staff       (20)       38 2023-06-08 06:59:36.248811 lycoris_lora-0.1.7.dev1/setup.cfg
+-rw-r--r--   0 kblueleaf   (501) staff       (20)      530 2023-06-08 06:59:07.000000 lycoris_lora-0.1.7.dev1/setup.py
```

### Comparing `lycoris_lora-0.1.6.dev1/LICENSE.md` & `lycoris_lora-0.1.7.dev1/LICENSE.md`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2023 KohakuBlueLeaf
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2023 KohakuBlueLeaf
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `lycoris_lora-0.1.6.dev1/README.md` & `lycoris_lora-0.1.7.dev1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,158 +1,168 @@
-# LyCORIS - Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion.
-
-![image](https://user-images.githubusercontent.com/59680068/224026402-7b779d58-5164-4ecd-a807-f98badae589e.png)
-(This image is generated by the model trained in Hadamard product representation)
-
-A project for implementing different algorithm to do parameter-efficient finetuning on stable diffusion or more.
-
-This project is started from LoCon(see archive branch).
-
-
-## What we have now
-See [Algo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Algo.md) or [Demo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Demo.md) for more example and explanation
-
-### Conventional LoRA
-* Include Conv layer implementation from LoCon
-* recommended settings
-  * dim <= 64
-  * alpha = 1 (or lower, like 0.3)
-
-### LoRA with Hadamard Product representation (LoHa)
-* Ref: [FedPara Low-Rank Hadamard Product For Communication-Efficient Federated Learning](https://openreview.net/pdf?id=d71n4ftoCBy)
-* designed for federated learning, but has some cool property like rank<=dim^2 so should be good for parameter-efficient finetuning.
-  * Conventional LoRA is rank<=dim
-* recommended settings
-  * dim <= 32
-  * alpha = 1 (or lower)
-  
-**WARNING: You are not supposed to use dim>64 in LoHa, which is over sqrt(original_dim) for almost all layer in SD**
-
-**High dim with LoHa may cause unstable loss or just goes to NaN. If you want to use high dim LoHa, please use lower lr**
-
-**WARNING-AGAIN: Use parameter-efficient algorithim in parameter-unefficient way is not a good idea**
-
-### (IA)^3
-* Ref: [Few-Shot Parameter-Efficient Fine-Tuning is Better and Cheaper than In-Context Learning](https://arxiv.org/abs/2205.05638)
-* You can try this algo with dev version package(or install from source code) and set algo=ia3
-* This algo need much higher lr (about 5e-3~1e-2)
-* This algo is good at learning style, but hard to transfer(You can only get reasonable result on the model you trained on).
-* This algo produce very tiny file(about 200~300KB)
-* **Experimental**
-
-### LoKR
-* Basically same idea of LoHA, but use kronecker product
-* This algo is quite sensitive and you may need to tune the lr
-* This algo can learn both character and style, but since it is small (auto factor, full rank, 2.5MB), it is also hard to transfer.
-* This algo produce relatively small file(auto factor: 900~2500KB)
-* Use smaller factor will produce bigger file, you can tune it if you think 2.5MB full rank is not good enough.
-
----
-
-## usage
-
-You can just use these training scripts.
-* [derrian-distro/LoRA_Easy_Training_Scripts](https://github.com/derrian-distro/LoRA_Easy_Training_Scripts)
-* [Linaqruf/kohya-trainer](https://github.com/Linaqruf/kohya-trainer)
-* [bmaltais/kohya_ss](https://github.com/bmaltais/kohya_ss)
-* [hollowstrawberry/kohya-colab](https://github.com/hollowstrawberry/kohya-colab)
-
-### For kohya script
-Activate sd-scripts' venv and then install this package
-```bash
-source PATH_TO_SDSCRIPTS_VENV/Scripts/activate
-```
-or
-```powershell
-PATH_TO_SDSCRIPTS_VENV\Scripts\Activate.ps1 # or .bat for cmd
-```
-
-And then you can install this package:
-* through pip
-```bash
-pip install lycoris_lora
-```
-
-* from source
-```bash
-git clone https://github.com/KohakuBlueleaf/LyCORIS
-cd LyCORIS
-pip install .
-```
-
-Finally you can use this package's kohya module to run kohya's training script
-```bash
-python3 sd-scripts/train_network.py \
-  --network_module lycoris.kohya \
-  --network_dim "DIM_FOR_LINEAR" --network_alpha "ALPHA_FOR_LINEAR"\
-  --network_args "conv_dim=DIM_FOR_CONV" "conv_alpha=ALPHA_FOR_CONV" \
-  "dropout=DROPOUT_RATE" "algo=locon" \
-```
-to train lycoris module for SD model
-
-* algo list:
-  * locon: Conventional Methods
-  * loha: Hadamard product representation introduced by FedPara
-  * lokr: Kronecker product representation
-  * ia3 : (IA)^3
-
-* Tips:
-  * Use network_dim=0 or conv_dim=0 to disable linear/conv layer
-  * LoHa/LoKr/(IA)^3 doesn't support dropout yet.
-
-
-### For a1111's sd-webui
-download [Extension](https://github.com/KohakuBlueleaf/a1111-sd-webui-lycoris) into sd-webui, and then use LyCORIS model in the extra netowrks tabs.
-
-**Not For Kohya-ss' Additional Network**
-
-
-### Extract LoCon
-You can extract LoCon from a dreambooth model with its base model.
-```bash
-python3 extract_locon.py <settings> <base_model> <db_model> <output>
-```
-Use --help to get more info
-```
-$ python3 extract_locon.py --help
-usage: extract_locon.py [-h] [--is_v2] [--device DEVICE] [--mode MODE] [--safetensors] [--linear_dim LINEAR_DIM] [--conv_dim CONV_DIM]
-                        [--linear_threshold LINEAR_THRESHOLD] [--conv_threshold CONV_THRESHOLD] [--linear_ratio LINEAR_RATIO] [--conv_ratio CONV_RATIO]
-                        [--linear_percentile LINEAR_PERCENTILE] [--conv_percentile CONV_PERCENTILE]
-                        base_model db_model output_name
-```
-
-
-## Example and Comparing for different algo
-see [Demo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Demo.md) and [Algo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Algo.md)
-
-
-## Change Log
-For full log, please see [Change.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Change.md)
-
-### 2023/04/08 Update for 0.1.5
-* Add (IA)^3 algorithm
-* Add lokr algorithm
-
-## Todo list
-- [ ] Module and Document for using LyCORIS in any other model, Not only SD.
-- [x] Proposition3 in [FedPara](https://arxiv.org/abs/2108.06098)
-  * also need custom backward to save the vram
-- [ ] Low rank + sparse representation
-  - [x] For extraction
-  - [ ] For training
-- [ ] Support more operation, not only linear and conv2d.
-- [ ] Configure varying ranks or dimensions for specific modules as needed.
-- [ ] Automatically selecting an algorithm based on the specific rank requirement.
-- [ ] Explore other low-rank representations or parameter-efficient methods to fine-tune either the entire model or specific parts of it.
-- [ ] More experiments for different task, not only diffusion models.
-
-
-## Citation
-```bibtex
-@misc{LyCORIS,
-  author       = "Shih-Ying Yeh (Kohaku-BlueLeaf), Yu-Guan Hsieh, Zhidong Gao",
-  title        = "LyCORIS - Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion",
-  howpublished = "\url{https://github.com/KohakuBlueleaf/LyCORIS}",
-  month        = "March",
-  year         = "2023"
-}
-```
+# LyCORIS - Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion.
+
+![image](https://user-images.githubusercontent.com/59680068/224026402-7b779d58-5164-4ecd-a807-f98badae589e.png)
+(This image is generated by the model trained in Hadamard product representation)
+
+A project for implementing different algorithm to do parameter-efficient finetuning on stable diffusion or more.
+
+This project is started from LoCon(see archive branch).
+
+
+## What we have now
+See [Algo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Algo.md) or [Demo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Demo.md) for more example and explanation
+
+### Conventional LoRA
+* Include Conv layer implementation from LoCon
+* recommended settings
+  * dim <= 64
+  * alpha = 1 (or lower, like 0.3)
+
+### LoRA with Hadamard Product representation (LoHa)
+* Ref: [FedPara Low-Rank Hadamard Product For Communication-Efficient Federated Learning](https://openreview.net/pdf?id=d71n4ftoCBy)
+* designed for federated learning, but has some cool property like rank<=dim^2 so should be good for parameter-efficient finetuning.
+  * Conventional LoRA is rank<=dim
+* recommended settings
+  * dim <= 32
+  * alpha = 1 (or lower)
+  
+**WARNING: You are not supposed to use dim>64 in LoHa, which is over sqrt(original_dim) for almost all layer in SD**
+
+**High dim with LoHa may cause unstable loss or just goes to NaN. If you want to use high dim LoHa, please use lower lr**
+
+**WARNING-AGAIN: Use parameter-efficient algorithim in parameter-unefficient way is not a good idea**
+
+### (IA)^3
+* Ref: [Few-Shot Parameter-Efficient Fine-Tuning is Better and Cheaper than In-Context Learning](https://arxiv.org/abs/2205.05638)
+* You can try this algo with dev version package(or install from source code) and set algo=ia3
+* This algo need much higher lr (about 5e-3~1e-2)
+* This algo is good at learning style, but hard to transfer(You can only get reasonable result on the model you trained on).
+* This algo produce very tiny file(about 200~300KB)
+* **Experimental**
+
+### LoKR
+* Basically same idea of LoHA, but use kronecker product
+* This algo is quite sensitive and you may need to tune the lr
+* This algo can learn both character and style, but since it is small (auto factor, full rank, 2.5MB), it is also hard to transfer.
+* This algo produce relatively small file(auto factor: 900~2500KB)
+* Use smaller factor will produce bigger file, you can tune it if you think 2.5MB full rank is not good enough.
+
+### DyLoRA
+* Ref [DyLoRA: Parameter Efficient Tuning of Pre-trained Models using Dynamic Search-Free Low Rank Adaptation](https://arxiv.org/pdf/2210.07558.pdf)
+* Basically a training trick of lora.
+* Every step, only update one row/col of LoRA weight.
+* When we want to update k row/col, we only use 0~k row/col to rebuild the weight (0<=k<=dim)
+* You can easily resize DyLoRA to target and get similar or even better result than LoRA trained at target dim. (And you don't need to train lot loras with different dim to check which is better)
+* You should use large dim with alpha=dim/4~dim (1 or dim is not very recommended)
+    * Example: dim=128, alpha=64
+* Since we only update 1 row/col each step, you will need more step to get reasonable result. If you want to train it with few steps, you may need to set block_size (update multiple row/col every step) to higer value (default=0)
+
+---
+
+## usage
+
+You can just use these training scripts.
+* [derrian-distro/LoRA_Easy_Training_Scripts](https://github.com/derrian-distro/LoRA_Easy_Training_Scripts)
+* [Linaqruf/kohya-trainer](https://github.com/Linaqruf/kohya-trainer)
+* [bmaltais/kohya_ss](https://github.com/bmaltais/kohya_ss)
+* [hollowstrawberry/kohya-colab](https://github.com/hollowstrawberry/kohya-colab)
+
+### For kohya script
+Activate sd-scripts' venv and then install this package
+```bash
+source PATH_TO_SDSCRIPTS_VENV/Scripts/activate
+```
+or
+```powershell
+PATH_TO_SDSCRIPTS_VENV\Scripts\Activate.ps1 # or .bat for cmd
+```
+
+And then you can install this package:
+* through pip
+```bash
+pip install lycoris_lora
+```
+
+* from source
+```bash
+git clone https://github.com/KohakuBlueleaf/LyCORIS
+cd LyCORIS
+pip install .
+```
+
+Finally you can use this package's kohya module to run kohya's training script
+```bash
+python3 sd-scripts/train_network.py \
+  --network_module lycoris.kohya \
+  --network_dim "DIM_FOR_LINEAR" --network_alpha "ALPHA_FOR_LINEAR"\
+  --network_args "conv_dim=DIM_FOR_CONV" "conv_alpha=ALPHA_FOR_CONV" \
+  "dropout=DROPOUT_RATE" "algo=locon" \
+```
+to train lycoris module for SD model
+
+* algo list:
+  * locon: Conventional Methods
+  * loha: Hadamard product representation introduced by FedPara
+  * lokr: Kronecker product representation
+  * ia3 : (IA)^3
+
+* Tips:
+  * Use network_dim=0 or conv_dim=0 to disable linear/conv layer
+  * LoHa/LoKr/(IA)^3 doesn't support dropout yet.
+
+
+### For a1111's sd-webui
+download [Extension](https://github.com/KohakuBlueleaf/a1111-sd-webui-lycoris) into sd-webui, and then use LyCORIS model in the extra netowrks tabs.
+
+**Not For Kohya-ss' Additional Network**
+
+
+### Extract LoCon
+You can extract LoCon from a dreambooth model with its base model.
+```bash
+python3 extract_locon.py <settings> <base_model> <db_model> <output>
+```
+Use --help to get more info
+```
+$ python3 extract_locon.py --help
+usage: extract_locon.py [-h] [--is_v2] [--device DEVICE] [--mode MODE] [--safetensors] [--linear_dim LINEAR_DIM] [--conv_dim CONV_DIM]
+                        [--linear_threshold LINEAR_THRESHOLD] [--conv_threshold CONV_THRESHOLD] [--linear_ratio LINEAR_RATIO] [--conv_ratio CONV_RATIO]
+                        [--linear_percentile LINEAR_PERCENTILE] [--conv_percentile CONV_PERCENTILE]
+                        base_model db_model output_name
+```
+
+
+## Example and Comparing for different algo
+see [Demo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Demo.md) and [Algo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Algo.md)
+
+
+## Change Log
+For full log, please see [Change.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Change.md)
+
+### 2023/04/08 Update for 0.1.5
+* Add (IA)^3 algorithm
+* Add lokr algorithm
+
+## Todo list
+- [ ] Module and Document for using LyCORIS in any other model, Not only SD.
+- [x] Proposition3 in [FedPara](https://arxiv.org/abs/2108.06098)
+  * also need custom backward to save the vram
+- [ ] Low rank + sparse representation
+  - [x] For extraction
+  - [ ] For training
+- [ ] Support more operation, not only linear and conv2d.
+- [ ] Configure varying ranks or dimensions for specific modules as needed.
+- [ ] Automatically selecting an algorithm based on the specific rank requirement.
+- [ ] Explore other low-rank representations or parameter-efficient methods to fine-tune either the entire model or specific parts of it.
+- [ ] More experiments for different task, not only diffusion models.
+
+
+## Citation
+```bibtex
+@misc{LyCORIS,
+  author       = "Shih-Ying Yeh (Kohaku-BlueLeaf), Yu-Guan Hsieh, Zhidong Gao",
+  title        = "LyCORIS - Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion",
+  howpublished = "\url{https://github.com/KohakuBlueleaf/LyCORIS}",
+  month        = "March",
+  year         = "2023"
+}
+```
```

### Comparing `lycoris_lora-0.1.6.dev1/lycoris/dylora.py` & `lycoris_lora-0.1.7.dev1/lycoris/dylora.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-import math
-import random
-
-from collections import OrderedDict, abc as container_abcs
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-
-class DyLoraModule(nn.Module):
-    """
-    Hadamard product Implementaion for Dynamic Low Rank adaptation
-    """
-
-    def __init__(
-        self, 
-        lora_name, 
-        org_module: nn.Module, 
-        multiplier=1.0, 
-        lora_dim=4, alpha=1, 
-        dropout=0.,
-        use_cp=False, 
-        block_size=1,
-        **kwargs,
-    ):
-        """ if alpha == 0 or None, alpha is rank (no scaling). """
-        super().__init__()
-        self.lora_name = lora_name
-        self.lora_dim = lora_dim
-        assert lora_dim % block_size == 0, 'lora_dim must be a multiple of block_size'
-        self.block_count = lora_dim//block_size
-        self.block_size = block_size
-        
-        self.shape = org_module.weight.shape
-        if org_module.__class__.__name__ == 'Conv2d':
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            out_dim = org_module.out_channels
-            shape = (out_dim, in_dim*k_size[0]*k_size[1])
-            self.op = F.conv2d
-            self.extra_args = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups
-            }
-        else:
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            shape = (out_dim, in_dim)
-            self.op = F.linear
-            self.extra_args = {}
-        
-        self.lora_dim = lora_dim
-        self.up_list = nn.ParameterList([
-            torch.empty(shape[0], 1)
-            for i in range(lora_dim)
-        ])
-        self.up_list.requires_grad_(False)
-        self.up_update = [
-            torch.zeros_like(self.up_list[i])
-            for i in range(lora_dim)
-        ]
-        
-        self.down_list = nn.ParameterList([
-            torch.empty(1, shape[1])
-            for i in range(lora_dim)
-        ])
-        self.down_list.requires_grad_(False)
-        self.down_update = [
-            torch.zeros_like(self.down_list[i])
-            for i in range(lora_dim)
-        ]
-        
-        self.index = 0
-        
-        if type(alpha) == torch.Tensor:
-            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-        alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        self.scale = alpha / self.lora_dim
-        self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
-
-        # Need more experiences on init method
-        
-        for v in self.down_list:
-            torch.nn.init.kaiming_uniform_(v, a=math.sqrt(5))
-        for v in self.up_list:
-            torch.nn.init.zeros_(v)
-        for i, v in enumerate(self.up_update):
-            v.copy_(self.up_list[i])
-        for i, v in enumerate(self.down_update):
-            v.copy_(self.down_list[i])
-
-        self.multiplier = multiplier
-        self.org_module = [org_module] # remove in applying
-        self.grad_ckpt = False
-        
-        self.apply_train(0)
-    
-    def state_dict(self, *args, destination=None, prefix='', keep_vars=False):
-        # TODO: Remove `args` and the parsing logic when BC allows.
-        if len(args) > 0:
-            if destination is None:
-                destination = args[0]
-            if len(args) > 1 and prefix == '':
-                prefix = args[1]
-            if len(args) > 2 and keep_vars is False:
-                keep_vars = args[2]
-            # DeprecationWarning is ignored by default
-
-        if destination is None:
-            destination = OrderedDict()
-            destination._metadata = OrderedDict()
-
-        local_metadata = dict(version=self._version)
-        if hasattr(destination, "_metadata"):
-            destination._metadata[prefix[:-1]] = local_metadata
-
-        destination[f'{prefix}alpha'] = self.alpha
-        destination[f'{prefix}lora_up.weight'] = nn.Parameter(
-            torch.concat(self.up_update, dim=1)
-        )
-        destination[f'{prefix}lora_down.weight'] = nn.Parameter(
-            torch.concat(self.down_update)
-        )
-        return destination
-
-    def apply_to(self):
-        self.org_module[0].forward = self.forward
-    
-    def apply_train(self, b:int):
-        self.up_list.requires_grad_(False)
-        self.down_list.requires_grad_(False)
-            
-        for i in range(self.index*self.block_size, (self.index+1)*self.block_size):
-            self.up_update[i].copy_(self.up_list[i])
-            self.down_update[i].copy_(self.down_list[i])
-        
-        for i in range(b*self.block_size, (b+1)*self.block_size):
-            self.up_list[i].copy_(self.up_update[i])
-            self.down_list[i].copy_(self.down_update[i])
-        
-        self.up_list.requires_grad_(True)
-        self.down_list.requires_grad_(True)
-        self.index = b
-
-    @torch.enable_grad()
-    def forward(self, x):
-        b = random.randint(0, self.block_count-1)
-        if self.up_update[b].device != self.up_list[b].device:
-            device = self.up_list[b].device
-            for i in range(self.lora_dim):
-                self.up_update[i] = self.up_update[i].to(device)
-                self.down_update[i] = self.down_update[i].to(device)
-        
-        if self.training:
-            self.apply_train(b)
-        down = torch.concat(
-            list(self.down_update[:b*self.block_size]) 
-            + list(self.down_list[b*self.block_size:(b+1)*self.block_size])
-        )
-        up = torch.concat(
-            list(self.up_update[:b*self.block_size]) 
-            + list(self.up_list[b*self.block_size:(b+1)*self.block_size]),
-            dim=1
-        )
-        
-        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
-        return self.op(
-            x, 
-            self.org_module[0].weight + (up@down).view(self.shape) * self.alpha/(b+1),
-            bias,
-            **self.extra_args
+import math
+import random
+
+from collections import OrderedDict, abc as container_abcs
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+
+class DyLoraModule(nn.Module):
+    """
+    Hadamard product Implementaion for Dynamic Low Rank adaptation
+    """
+
+    def __init__(
+        self, 
+        lora_name, 
+        org_module: nn.Module, 
+        multiplier=1.0, 
+        lora_dim=4, alpha=1, 
+        dropout=0.,
+        use_cp=False, 
+        block_size=1,
+        **kwargs,
+    ):
+        """ if alpha == 0 or None, alpha is rank (no scaling). """
+        super().__init__()
+        self.lora_name = lora_name
+        self.lora_dim = lora_dim
+        assert lora_dim % block_size == 0, 'lora_dim must be a multiple of block_size'
+        self.block_count = lora_dim//block_size
+        self.block_size = block_size
+        
+        self.shape = org_module.weight.shape
+        if org_module.__class__.__name__ == 'Conv2d':
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            out_dim = org_module.out_channels
+            shape = (out_dim, in_dim*k_size[0]*k_size[1])
+            self.op = F.conv2d
+            self.extra_args = {
+                "stride": org_module.stride,
+                "padding": org_module.padding,
+                "dilation": org_module.dilation,
+                "groups": org_module.groups
+            }
+        else:
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            shape = (out_dim, in_dim)
+            self.op = F.linear
+            self.extra_args = {}
+        
+        self.lora_dim = lora_dim
+        self.up_list = nn.ParameterList([
+            torch.empty(shape[0], 1)
+            for i in range(lora_dim)
+        ])
+        self.up_list.requires_grad_(False)
+        self.up_update = [
+            torch.zeros_like(self.up_list[i])
+            for i in range(lora_dim)
+        ]
+        
+        self.down_list = nn.ParameterList([
+            torch.empty(1, shape[1])
+            for i in range(lora_dim)
+        ])
+        self.down_list.requires_grad_(False)
+        self.down_update = [
+            torch.zeros_like(self.down_list[i])
+            for i in range(lora_dim)
+        ]
+        
+        self.index = 0
+        
+        if type(alpha) == torch.Tensor:
+            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
+        alpha = lora_dim if alpha is None or alpha == 0 else alpha
+        self.scale = alpha / self.lora_dim
+        self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
+
+        # Need more experiences on init method
+        
+        for v in self.down_list:
+            torch.nn.init.kaiming_uniform_(v, a=math.sqrt(5))
+        for v in self.up_list:
+            torch.nn.init.zeros_(v)
+        for i, v in enumerate(self.up_update):
+            v.copy_(self.up_list[i])
+        for i, v in enumerate(self.down_update):
+            v.copy_(self.down_list[i])
+
+        self.multiplier = multiplier
+        self.org_module = [org_module] # remove in applying
+        self.grad_ckpt = False
+        
+        self.apply_train(0)
+    
+    def state_dict(self, *args, destination=None, prefix='', keep_vars=False):
+        # TODO: Remove `args` and the parsing logic when BC allows.
+        if len(args) > 0:
+            if destination is None:
+                destination = args[0]
+            if len(args) > 1 and prefix == '':
+                prefix = args[1]
+            if len(args) > 2 and keep_vars is False:
+                keep_vars = args[2]
+            # DeprecationWarning is ignored by default
+
+        if destination is None:
+            destination = OrderedDict()
+            destination._metadata = OrderedDict()
+
+        local_metadata = dict(version=self._version)
+        if hasattr(destination, "_metadata"):
+            destination._metadata[prefix[:-1]] = local_metadata
+
+        destination[f'{prefix}alpha'] = self.alpha
+        destination[f'{prefix}lora_up.weight'] = nn.Parameter(
+            torch.concat(self.up_update, dim=1)
+        )
+        destination[f'{prefix}lora_down.weight'] = nn.Parameter(
+            torch.concat(self.down_update)
+        )
+        return destination
+
+    def apply_to(self):
+        self.org_module[0].forward = self.forward
+    
+    def apply_train(self, b:int):
+        self.up_list.requires_grad_(False)
+        self.down_list.requires_grad_(False)
+            
+        for i in range(self.index*self.block_size, (self.index+1)*self.block_size):
+            self.up_update[i].copy_(self.up_list[i])
+            self.down_update[i].copy_(self.down_list[i])
+        
+        for i in range(b*self.block_size, (b+1)*self.block_size):
+            self.up_list[i].copy_(self.up_update[i])
+            self.down_list[i].copy_(self.down_update[i])
+        
+        self.up_list.requires_grad_(True)
+        self.down_list.requires_grad_(True)
+        self.index = b
+
+    @torch.enable_grad()
+    def forward(self, x):
+        b = random.randint(0, self.block_count-1)
+        if self.up_update[b].device != self.up_list[b].device:
+            device = self.up_list[b].device
+            for i in range(self.lora_dim):
+                self.up_update[i] = self.up_update[i].to(device)
+                self.down_update[i] = self.down_update[i].to(device)
+        
+        if self.training:
+            self.apply_train(b)
+        down = torch.concat(
+            list(self.down_update[:b*self.block_size]) 
+            + list(self.down_list[b*self.block_size:(b+1)*self.block_size])
+        )
+        up = torch.concat(
+            list(self.up_update[:b*self.block_size]) 
+            + list(self.up_list[b*self.block_size:(b+1)*self.block_size]),
+            dim=1
+        )
+        
+        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
+        return self.op(
+            x, 
+            self.org_module[0].weight + (up@down).view(self.shape) * self.alpha/(b+1),
+            bias,
+            **self.extra_args
         )
```

### Comparing `lycoris_lora-0.1.6.dev1/lycoris/ia3.py` & `lycoris_lora-0.1.7.dev1/lycoris/ia3.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import math
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-
-class IA3Module(nn.Module):
-    """
-    Hadamard product Implementaion for Low Rank Adaptation
-    """
-
-    def __init__(
-        self, 
-        lora_name, 
-        org_module: nn.Module, 
-        multiplier=1.0, 
-        train_on_input=False, 
-        **kwargs
-    ):
-        """ if alpha == 0 or None, alpha is rank (no scaling). """
-        super().__init__()
-        self.lora_name = lora_name
-        self.cp=False
-        
-        self.shape = org_module.weight.shape
-        if org_module.__class__.__name__ == 'Conv2d':
-            in_dim = org_module.in_channels
-            out_dim = org_module.out_channels
-            if train_on_input:
-                train_dim = in_dim
-            else:
-                train_dim = out_dim
-            self.weight = nn.Parameter(torch.empty(1, train_dim, 1, 1))
-        else:
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            if train_on_input:
-                train_dim = in_dim
-            else:
-                train_dim = out_dim
-            
-            self.weight = nn.Parameter(torch.empty(train_dim))
-
-        # Need more experiences on init method
-        torch.nn.init.constant_(self.weight, 0)
-
-        self.multiplier = multiplier
-        self.org_forward = None
-        self.org_module = [org_module] # remove in applying
-        self.grad_ckpt = False
-        self.train_input = train_on_input
-        self.register_buffer('on_input', torch.tensor(int(train_on_input)))
-
-    def apply_to(self):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-
-    @torch.enable_grad()
-    def forward(self, x):
-        if self.train_input:
-            x = x * (1 + self.weight * self.multiplier)
-        out = self.org_forward(x)
-        dtype = out.dtype
-        if not self.train_input:
-            out = out * (1 + self.weight * self.multiplier)
-            out = out.to(dtype)
+import math
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+
+class IA3Module(nn.Module):
+    """
+    Hadamard product Implementaion for Low Rank Adaptation
+    """
+
+    def __init__(
+        self, 
+        lora_name, 
+        org_module: nn.Module, 
+        multiplier=1.0, 
+        train_on_input=False, 
+        **kwargs
+    ):
+        """ if alpha == 0 or None, alpha is rank (no scaling). """
+        super().__init__()
+        self.lora_name = lora_name
+        self.cp=False
+        
+        self.shape = org_module.weight.shape
+        if org_module.__class__.__name__ == 'Conv2d':
+            in_dim = org_module.in_channels
+            out_dim = org_module.out_channels
+            if train_on_input:
+                train_dim = in_dim
+            else:
+                train_dim = out_dim
+            self.weight = nn.Parameter(torch.empty(1, train_dim, 1, 1))
+        else:
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            if train_on_input:
+                train_dim = in_dim
+            else:
+                train_dim = out_dim
+            
+            self.weight = nn.Parameter(torch.empty(train_dim))
+
+        # Need more experiences on init method
+        torch.nn.init.constant_(self.weight, 0)
+
+        self.multiplier = multiplier
+        self.org_forward = None
+        self.org_module = [org_module] # remove in applying
+        self.grad_ckpt = False
+        self.train_input = train_on_input
+        self.register_buffer('on_input', torch.tensor(int(train_on_input)))
+
+    def apply_to(self):
+        self.org_forward = self.org_module[0].forward
+        self.org_module[0].forward = self.forward
+
+    @torch.enable_grad()
+    def forward(self, x):
+        if self.train_input:
+            x = x * (1 + self.weight * self.multiplier)
+        out = self.org_forward(x)
+        dtype = out.dtype
+        if not self.train_input:
+            out = out * (1 + self.weight * self.multiplier)
+            out = out.to(dtype)
         return out
```

### Comparing `lycoris_lora-0.1.6.dev1/lycoris/kohya_model_utils.py` & `lycoris_lora-0.1.7.dev1/lycoris/kohya_model_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,1165 +1,1165 @@
-# v1: split from train_db_fixed.py.
-# v2: support safetensors
-
-import math
-import os
-import torch
-from transformers import CLIPTextModel, CLIPTokenizer, CLIPTextConfig, logging
-from diffusers import AutoencoderKL, DDIMScheduler, StableDiffusionPipeline, UNet2DConditionModel
-from safetensors.torch import load_file, save_file
-
-# DiffUsers版StableDiffusionのモデルパラメータ
-NUM_TRAIN_TIMESTEPS = 1000
-BETA_START = 0.00085
-BETA_END = 0.0120
-
-UNET_PARAMS_MODEL_CHANNELS = 320
-UNET_PARAMS_CHANNEL_MULT = [1, 2, 4, 4]
-UNET_PARAMS_ATTENTION_RESOLUTIONS = [4, 2, 1]
-UNET_PARAMS_IMAGE_SIZE = 64  # fixed from old invalid value `32`
-UNET_PARAMS_IN_CHANNELS = 4
-UNET_PARAMS_OUT_CHANNELS = 4
-UNET_PARAMS_NUM_RES_BLOCKS = 2
-UNET_PARAMS_CONTEXT_DIM = 768
-UNET_PARAMS_NUM_HEADS = 8
-
-VAE_PARAMS_Z_CHANNELS = 4
-VAE_PARAMS_RESOLUTION = 256
-VAE_PARAMS_IN_CHANNELS = 3
-VAE_PARAMS_OUT_CH = 3
-VAE_PARAMS_CH = 128
-VAE_PARAMS_CH_MULT = [1, 2, 4, 4]
-VAE_PARAMS_NUM_RES_BLOCKS = 2
-
-# V2
-V2_UNET_PARAMS_ATTENTION_HEAD_DIM = [5, 10, 20, 20]
-V2_UNET_PARAMS_CONTEXT_DIM = 1024
-
-# Diffusersの設定を読み込むための参照モデル
-DIFFUSERS_REF_MODEL_ID_V1 = "runwayml/stable-diffusion-v1-5"
-DIFFUSERS_REF_MODEL_ID_V2 = "stabilityai/stable-diffusion-2-1"
-
-
-# region StableDiffusion->Diffusersの変換コード
-# convert_original_stable_diffusion_to_diffusers をコピーして修正している（ASL 2.0）
-
-
-def shave_segments(path, n_shave_prefix_segments=1):
-    """
-    Removes segments. Positive values shave the first segments, negative shave the last segments.
-    """
-    if n_shave_prefix_segments >= 0:
-        return ".".join(path.split(".")[n_shave_prefix_segments:])
-    else:
-        return ".".join(path.split(".")[:n_shave_prefix_segments])
-
-
-def renew_resnet_paths(old_list, n_shave_prefix_segments=0):
-    """
-    Updates paths inside resnets to the new naming scheme (local renaming)
-    """
-    mapping = []
-    for old_item in old_list:
-        new_item = old_item.replace("in_layers.0", "norm1")
-        new_item = new_item.replace("in_layers.2", "conv1")
-
-        new_item = new_item.replace("out_layers.0", "norm2")
-        new_item = new_item.replace("out_layers.3", "conv2")
-
-        new_item = new_item.replace("emb_layers.1", "time_emb_proj")
-        new_item = new_item.replace("skip_connection", "conv_shortcut")
-
-        new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
-
-        mapping.append({"old": old_item, "new": new_item})
-
-    return mapping
-
-
-def renew_vae_resnet_paths(old_list, n_shave_prefix_segments=0):
-    """
-    Updates paths inside resnets to the new naming scheme (local renaming)
-    """
-    mapping = []
-    for old_item in old_list:
-        new_item = old_item
-
-        new_item = new_item.replace("nin_shortcut", "conv_shortcut")
-        new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
-
-        mapping.append({"old": old_item, "new": new_item})
-
-    return mapping
-
-
-def renew_attention_paths(old_list, n_shave_prefix_segments=0):
-    """
-    Updates paths inside attentions to the new naming scheme (local renaming)
-    """
-    mapping = []
-    for old_item in old_list:
-        new_item = old_item
-
-        #         new_item = new_item.replace('norm.weight', 'group_norm.weight')
-        #         new_item = new_item.replace('norm.bias', 'group_norm.bias')
-
-        #         new_item = new_item.replace('proj_out.weight', 'proj_attn.weight')
-        #         new_item = new_item.replace('proj_out.bias', 'proj_attn.bias')
-
-        #         new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
-
-        mapping.append({"old": old_item, "new": new_item})
-
-    return mapping
-
-
-def renew_vae_attention_paths(old_list, n_shave_prefix_segments=0):
-    """
-    Updates paths inside attentions to the new naming scheme (local renaming)
-    """
-    mapping = []
-    for old_item in old_list:
-        new_item = old_item
-
-        new_item = new_item.replace("norm.weight", "group_norm.weight")
-        new_item = new_item.replace("norm.bias", "group_norm.bias")
-
-        new_item = new_item.replace("q.weight", "query.weight")
-        new_item = new_item.replace("q.bias", "query.bias")
-
-        new_item = new_item.replace("k.weight", "key.weight")
-        new_item = new_item.replace("k.bias", "key.bias")
-
-        new_item = new_item.replace("v.weight", "value.weight")
-        new_item = new_item.replace("v.bias", "value.bias")
-
-        new_item = new_item.replace("proj_out.weight", "proj_attn.weight")
-        new_item = new_item.replace("proj_out.bias", "proj_attn.bias")
-
-        new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
-
-        mapping.append({"old": old_item, "new": new_item})
-
-    return mapping
-
-
-def assign_to_checkpoint(
-    paths, checkpoint, old_checkpoint, attention_paths_to_split=None, additional_replacements=None, config=None
-):
-    """
-    This does the final conversion step: take locally converted weights and apply a global renaming
-    to them. It splits attention layers, and takes into account additional replacements
-    that may arise.
-
-    Assigns the weights to the new checkpoint.
-    """
-    assert isinstance(paths, list), "Paths should be a list of dicts containing 'old' and 'new' keys."
-
-    # Splits the attention layers into three variables.
-    if attention_paths_to_split is not None:
-        for path, path_map in attention_paths_to_split.items():
-            old_tensor = old_checkpoint[path]
-            channels = old_tensor.shape[0] // 3
-
-            target_shape = (-1, channels) if len(old_tensor.shape) == 3 else (-1)
-
-            num_heads = old_tensor.shape[0] // config["num_head_channels"] // 3
-
-            old_tensor = old_tensor.reshape((num_heads, 3 * channels // num_heads) + old_tensor.shape[1:])
-            query, key, value = old_tensor.split(channels // num_heads, dim=1)
-
-            checkpoint[path_map["query"]] = query.reshape(target_shape)
-            checkpoint[path_map["key"]] = key.reshape(target_shape)
-            checkpoint[path_map["value"]] = value.reshape(target_shape)
-
-    for path in paths:
-        new_path = path["new"]
-
-        # These have already been assigned
-        if attention_paths_to_split is not None and new_path in attention_paths_to_split:
-            continue
-
-        # Global renaming happens here
-        new_path = new_path.replace("middle_block.0", "mid_block.resnets.0")
-        new_path = new_path.replace("middle_block.1", "mid_block.attentions.0")
-        new_path = new_path.replace("middle_block.2", "mid_block.resnets.1")
-
-        if additional_replacements is not None:
-            for replacement in additional_replacements:
-                new_path = new_path.replace(replacement["old"], replacement["new"])
-
-        # proj_attn.weight has to be converted from conv 1D to linear
-        if "proj_attn.weight" in new_path:
-            checkpoint[new_path] = old_checkpoint[path["old"]][:, :, 0]
-        else:
-            checkpoint[new_path] = old_checkpoint[path["old"]]
-
-
-def conv_attn_to_linear(checkpoint):
-    keys = list(checkpoint.keys())
-    attn_keys = ["query.weight", "key.weight", "value.weight"]
-    for key in keys:
-        if ".".join(key.split(".")[-2:]) in attn_keys:
-            if checkpoint[key].ndim > 2:
-                checkpoint[key] = checkpoint[key][:, :, 0, 0]
-        elif "proj_attn.weight" in key:
-            if checkpoint[key].ndim > 2:
-                checkpoint[key] = checkpoint[key][:, :, 0]
-
-
-def linear_transformer_to_conv(checkpoint):
-    keys = list(checkpoint.keys())
-    tf_keys = ["proj_in.weight", "proj_out.weight"]
-    for key in keys:
-        if ".".join(key.split(".")[-2:]) in tf_keys:
-            if checkpoint[key].ndim == 2:
-                checkpoint[key] = checkpoint[key].unsqueeze(2).unsqueeze(2)
-
-
-def convert_ldm_unet_checkpoint(v2, checkpoint, config):
-    """
-    Takes a state dict and a config, and returns a converted checkpoint.
-    """
-
-    # extract state_dict for UNet
-    unet_state_dict = {}
-    unet_key = "model.diffusion_model."
-    keys = list(checkpoint.keys())
-    for key in keys:
-        if key.startswith(unet_key):
-            unet_state_dict[key.replace(unet_key, "")] = checkpoint.pop(key)
-
-    new_checkpoint = {}
-
-    new_checkpoint["time_embedding.linear_1.weight"] = unet_state_dict["time_embed.0.weight"]
-    new_checkpoint["time_embedding.linear_1.bias"] = unet_state_dict["time_embed.0.bias"]
-    new_checkpoint["time_embedding.linear_2.weight"] = unet_state_dict["time_embed.2.weight"]
-    new_checkpoint["time_embedding.linear_2.bias"] = unet_state_dict["time_embed.2.bias"]
-
-    new_checkpoint["conv_in.weight"] = unet_state_dict["input_blocks.0.0.weight"]
-    new_checkpoint["conv_in.bias"] = unet_state_dict["input_blocks.0.0.bias"]
-
-    new_checkpoint["conv_norm_out.weight"] = unet_state_dict["out.0.weight"]
-    new_checkpoint["conv_norm_out.bias"] = unet_state_dict["out.0.bias"]
-    new_checkpoint["conv_out.weight"] = unet_state_dict["out.2.weight"]
-    new_checkpoint["conv_out.bias"] = unet_state_dict["out.2.bias"]
-
-    # Retrieves the keys for the input blocks only
-    num_input_blocks = len({".".join(layer.split(".")[:2]) for layer in unet_state_dict if "input_blocks" in layer})
-    input_blocks = {
-        layer_id: [key for key in unet_state_dict if f"input_blocks.{layer_id}." in key] for layer_id in range(num_input_blocks)
-    }
-
-    # Retrieves the keys for the middle blocks only
-    num_middle_blocks = len({".".join(layer.split(".")[:2]) for layer in unet_state_dict if "middle_block" in layer})
-    middle_blocks = {
-        layer_id: [key for key in unet_state_dict if f"middle_block.{layer_id}." in key] for layer_id in range(num_middle_blocks)
-    }
-
-    # Retrieves the keys for the output blocks only
-    num_output_blocks = len({".".join(layer.split(".")[:2]) for layer in unet_state_dict if "output_blocks" in layer})
-    output_blocks = {
-        layer_id: [key for key in unet_state_dict if f"output_blocks.{layer_id}." in key] for layer_id in range(num_output_blocks)
-    }
-
-    for i in range(1, num_input_blocks):
-        block_id = (i - 1) // (config["layers_per_block"] + 1)
-        layer_in_block_id = (i - 1) % (config["layers_per_block"] + 1)
-
-        resnets = [key for key in input_blocks[i] if f"input_blocks.{i}.0" in key and f"input_blocks.{i}.0.op" not in key]
-        attentions = [key for key in input_blocks[i] if f"input_blocks.{i}.1" in key]
-
-        if f"input_blocks.{i}.0.op.weight" in unet_state_dict:
-            new_checkpoint[f"down_blocks.{block_id}.downsamplers.0.conv.weight"] = unet_state_dict.pop(
-                f"input_blocks.{i}.0.op.weight"
-            )
-            new_checkpoint[f"down_blocks.{block_id}.downsamplers.0.conv.bias"] = unet_state_dict.pop(f"input_blocks.{i}.0.op.bias")
-
-        paths = renew_resnet_paths(resnets)
-        meta_path = {"old": f"input_blocks.{i}.0", "new": f"down_blocks.{block_id}.resnets.{layer_in_block_id}"}
-        assign_to_checkpoint(paths, new_checkpoint, unet_state_dict, additional_replacements=[meta_path], config=config)
-
-        if len(attentions):
-            paths = renew_attention_paths(attentions)
-            meta_path = {"old": f"input_blocks.{i}.1", "new": f"down_blocks.{block_id}.attentions.{layer_in_block_id}"}
-            assign_to_checkpoint(paths, new_checkpoint, unet_state_dict, additional_replacements=[meta_path], config=config)
-
-    resnet_0 = middle_blocks[0]
-    attentions = middle_blocks[1]
-    resnet_1 = middle_blocks[2]
-
-    resnet_0_paths = renew_resnet_paths(resnet_0)
-    assign_to_checkpoint(resnet_0_paths, new_checkpoint, unet_state_dict, config=config)
-
-    resnet_1_paths = renew_resnet_paths(resnet_1)
-    assign_to_checkpoint(resnet_1_paths, new_checkpoint, unet_state_dict, config=config)
-
-    attentions_paths = renew_attention_paths(attentions)
-    meta_path = {"old": "middle_block.1", "new": "mid_block.attentions.0"}
-    assign_to_checkpoint(attentions_paths, new_checkpoint, unet_state_dict, additional_replacements=[meta_path], config=config)
-
-    for i in range(num_output_blocks):
-        block_id = i // (config["layers_per_block"] + 1)
-        layer_in_block_id = i % (config["layers_per_block"] + 1)
-        output_block_layers = [shave_segments(name, 2) for name in output_blocks[i]]
-        output_block_list = {}
-
-        for layer in output_block_layers:
-            layer_id, layer_name = layer.split(".")[0], shave_segments(layer, 1)
-            if layer_id in output_block_list:
-                output_block_list[layer_id].append(layer_name)
-            else:
-                output_block_list[layer_id] = [layer_name]
-
-        if len(output_block_list) > 1:
-            resnets = [key for key in output_blocks[i] if f"output_blocks.{i}.0" in key]
-            attentions = [key for key in output_blocks[i] if f"output_blocks.{i}.1" in key]
-
-            resnet_0_paths = renew_resnet_paths(resnets)
-            paths = renew_resnet_paths(resnets)
-
-            meta_path = {"old": f"output_blocks.{i}.0", "new": f"up_blocks.{block_id}.resnets.{layer_in_block_id}"}
-            assign_to_checkpoint(paths, new_checkpoint, unet_state_dict, additional_replacements=[meta_path], config=config)
-
-            # オリジナル：
-            # if ["conv.weight", "conv.bias"] in output_block_list.values():
-            #   index = list(output_block_list.values()).index(["conv.weight", "conv.bias"])
-
-            # biasとweightの順番に依存しないようにする：もっといいやり方がありそうだが
-            for l in output_block_list.values():
-                l.sort()
-
-            if ["conv.bias", "conv.weight"] in output_block_list.values():
-                index = list(output_block_list.values()).index(["conv.bias", "conv.weight"])
-                new_checkpoint[f"up_blocks.{block_id}.upsamplers.0.conv.bias"] = unet_state_dict[
-                    f"output_blocks.{i}.{index}.conv.bias"
-                ]
-                new_checkpoint[f"up_blocks.{block_id}.upsamplers.0.conv.weight"] = unet_state_dict[
-                    f"output_blocks.{i}.{index}.conv.weight"
-                ]
-
-                # Clear attentions as they have been attributed above.
-                if len(attentions) == 2:
-                    attentions = []
-
-            if len(attentions):
-                paths = renew_attention_paths(attentions)
-                meta_path = {
-                    "old": f"output_blocks.{i}.1",
-                    "new": f"up_blocks.{block_id}.attentions.{layer_in_block_id}",
-                }
-                assign_to_checkpoint(paths, new_checkpoint, unet_state_dict, additional_replacements=[meta_path], config=config)
-        else:
-            resnet_0_paths = renew_resnet_paths(output_block_layers, n_shave_prefix_segments=1)
-            for path in resnet_0_paths:
-                old_path = ".".join(["output_blocks", str(i), path["old"]])
-                new_path = ".".join(["up_blocks", str(block_id), "resnets", str(layer_in_block_id), path["new"]])
-
-                new_checkpoint[new_path] = unet_state_dict[old_path]
-
-    # SDのv2では1*1のconv2dがlinearに変わっているので、linear->convに変換する
-    if v2:
-        linear_transformer_to_conv(new_checkpoint)
-
-    return new_checkpoint
-
-
-def convert_ldm_vae_checkpoint(checkpoint, config):
-    # extract state dict for VAE
-    vae_state_dict = {}
-    vae_key = "first_stage_model."
-    keys = list(checkpoint.keys())
-    for key in keys:
-        if key.startswith(vae_key):
-            vae_state_dict[key.replace(vae_key, "")] = checkpoint.get(key)
-    # if len(vae_state_dict) == 0:
-    #   # 渡されたcheckpointは.ckptから読み込んだcheckpointではなくvaeのstate_dict
-    #   vae_state_dict = checkpoint
-
-    new_checkpoint = {}
-
-    new_checkpoint["encoder.conv_in.weight"] = vae_state_dict["encoder.conv_in.weight"]
-    new_checkpoint["encoder.conv_in.bias"] = vae_state_dict["encoder.conv_in.bias"]
-    new_checkpoint["encoder.conv_out.weight"] = vae_state_dict["encoder.conv_out.weight"]
-    new_checkpoint["encoder.conv_out.bias"] = vae_state_dict["encoder.conv_out.bias"]
-    new_checkpoint["encoder.conv_norm_out.weight"] = vae_state_dict["encoder.norm_out.weight"]
-    new_checkpoint["encoder.conv_norm_out.bias"] = vae_state_dict["encoder.norm_out.bias"]
-
-    new_checkpoint["decoder.conv_in.weight"] = vae_state_dict["decoder.conv_in.weight"]
-    new_checkpoint["decoder.conv_in.bias"] = vae_state_dict["decoder.conv_in.bias"]
-    new_checkpoint["decoder.conv_out.weight"] = vae_state_dict["decoder.conv_out.weight"]
-    new_checkpoint["decoder.conv_out.bias"] = vae_state_dict["decoder.conv_out.bias"]
-    new_checkpoint["decoder.conv_norm_out.weight"] = vae_state_dict["decoder.norm_out.weight"]
-    new_checkpoint["decoder.conv_norm_out.bias"] = vae_state_dict["decoder.norm_out.bias"]
-
-    new_checkpoint["quant_conv.weight"] = vae_state_dict["quant_conv.weight"]
-    new_checkpoint["quant_conv.bias"] = vae_state_dict["quant_conv.bias"]
-    new_checkpoint["post_quant_conv.weight"] = vae_state_dict["post_quant_conv.weight"]
-    new_checkpoint["post_quant_conv.bias"] = vae_state_dict["post_quant_conv.bias"]
-
-    # Retrieves the keys for the encoder down blocks only
-    num_down_blocks = len({".".join(layer.split(".")[:3]) for layer in vae_state_dict if "encoder.down" in layer})
-    down_blocks = {layer_id: [key for key in vae_state_dict if f"down.{layer_id}" in key] for layer_id in range(num_down_blocks)}
-
-    # Retrieves the keys for the decoder up blocks only
-    num_up_blocks = len({".".join(layer.split(".")[:3]) for layer in vae_state_dict if "decoder.up" in layer})
-    up_blocks = {layer_id: [key for key in vae_state_dict if f"up.{layer_id}" in key] for layer_id in range(num_up_blocks)}
-
-    for i in range(num_down_blocks):
-        resnets = [key for key in down_blocks[i] if f"down.{i}" in key and f"down.{i}.downsample" not in key]
-
-        if f"encoder.down.{i}.downsample.conv.weight" in vae_state_dict:
-            new_checkpoint[f"encoder.down_blocks.{i}.downsamplers.0.conv.weight"] = vae_state_dict.pop(
-                f"encoder.down.{i}.downsample.conv.weight"
-            )
-            new_checkpoint[f"encoder.down_blocks.{i}.downsamplers.0.conv.bias"] = vae_state_dict.pop(
-                f"encoder.down.{i}.downsample.conv.bias"
-            )
-
-        paths = renew_vae_resnet_paths(resnets)
-        meta_path = {"old": f"down.{i}.block", "new": f"down_blocks.{i}.resnets"}
-        assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
-
-    mid_resnets = [key for key in vae_state_dict if "encoder.mid.block" in key]
-    num_mid_res_blocks = 2
-    for i in range(1, num_mid_res_blocks + 1):
-        resnets = [key for key in mid_resnets if f"encoder.mid.block_{i}" in key]
-
-        paths = renew_vae_resnet_paths(resnets)
-        meta_path = {"old": f"mid.block_{i}", "new": f"mid_block.resnets.{i - 1}"}
-        assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
-
-    mid_attentions = [key for key in vae_state_dict if "encoder.mid.attn" in key]
-    paths = renew_vae_attention_paths(mid_attentions)
-    meta_path = {"old": "mid.attn_1", "new": "mid_block.attentions.0"}
-    assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
-    conv_attn_to_linear(new_checkpoint)
-
-    for i in range(num_up_blocks):
-        block_id = num_up_blocks - 1 - i
-        resnets = [key for key in up_blocks[block_id] if f"up.{block_id}" in key and f"up.{block_id}.upsample" not in key]
-
-        if f"decoder.up.{block_id}.upsample.conv.weight" in vae_state_dict:
-            new_checkpoint[f"decoder.up_blocks.{i}.upsamplers.0.conv.weight"] = vae_state_dict[
-                f"decoder.up.{block_id}.upsample.conv.weight"
-            ]
-            new_checkpoint[f"decoder.up_blocks.{i}.upsamplers.0.conv.bias"] = vae_state_dict[
-                f"decoder.up.{block_id}.upsample.conv.bias"
-            ]
-
-        paths = renew_vae_resnet_paths(resnets)
-        meta_path = {"old": f"up.{block_id}.block", "new": f"up_blocks.{i}.resnets"}
-        assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
-
-    mid_resnets = [key for key in vae_state_dict if "decoder.mid.block" in key]
-    num_mid_res_blocks = 2
-    for i in range(1, num_mid_res_blocks + 1):
-        resnets = [key for key in mid_resnets if f"decoder.mid.block_{i}" in key]
-
-        paths = renew_vae_resnet_paths(resnets)
-        meta_path = {"old": f"mid.block_{i}", "new": f"mid_block.resnets.{i - 1}"}
-        assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
-
-    mid_attentions = [key for key in vae_state_dict if "decoder.mid.attn" in key]
-    paths = renew_vae_attention_paths(mid_attentions)
-    meta_path = {"old": "mid.attn_1", "new": "mid_block.attentions.0"}
-    assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
-    conv_attn_to_linear(new_checkpoint)
-    return new_checkpoint
-
-
-def create_unet_diffusers_config(v2):
-    """
-    Creates a config for the diffusers based on the config of the LDM model.
-    """
-    # unet_params = original_config.model.params.unet_config.params
-
-    block_out_channels = [UNET_PARAMS_MODEL_CHANNELS * mult for mult in UNET_PARAMS_CHANNEL_MULT]
-
-    down_block_types = []
-    resolution = 1
-    for i in range(len(block_out_channels)):
-        block_type = "CrossAttnDownBlock2D" if resolution in UNET_PARAMS_ATTENTION_RESOLUTIONS else "DownBlock2D"
-        down_block_types.append(block_type)
-        if i != len(block_out_channels) - 1:
-            resolution *= 2
-
-    up_block_types = []
-    for i in range(len(block_out_channels)):
-        block_type = "CrossAttnUpBlock2D" if resolution in UNET_PARAMS_ATTENTION_RESOLUTIONS else "UpBlock2D"
-        up_block_types.append(block_type)
-        resolution //= 2
-
-    config = dict(
-        sample_size=UNET_PARAMS_IMAGE_SIZE,
-        in_channels=UNET_PARAMS_IN_CHANNELS,
-        out_channels=UNET_PARAMS_OUT_CHANNELS,
-        down_block_types=tuple(down_block_types),
-        up_block_types=tuple(up_block_types),
-        block_out_channels=tuple(block_out_channels),
-        layers_per_block=UNET_PARAMS_NUM_RES_BLOCKS,
-        cross_attention_dim=UNET_PARAMS_CONTEXT_DIM if not v2 else V2_UNET_PARAMS_CONTEXT_DIM,
-        attention_head_dim=UNET_PARAMS_NUM_HEADS if not v2 else V2_UNET_PARAMS_ATTENTION_HEAD_DIM,
-    )
-
-    return config
-
-
-def create_vae_diffusers_config():
-    """
-    Creates a config for the diffusers based on the config of the LDM model.
-    """
-    # vae_params = original_config.model.params.first_stage_config.params.ddconfig
-    # _ = original_config.model.params.first_stage_config.params.embed_dim
-    block_out_channels = [VAE_PARAMS_CH * mult for mult in VAE_PARAMS_CH_MULT]
-    down_block_types = ["DownEncoderBlock2D"] * len(block_out_channels)
-    up_block_types = ["UpDecoderBlock2D"] * len(block_out_channels)
-
-    config = dict(
-        sample_size=VAE_PARAMS_RESOLUTION,
-        in_channels=VAE_PARAMS_IN_CHANNELS,
-        out_channels=VAE_PARAMS_OUT_CH,
-        down_block_types=tuple(down_block_types),
-        up_block_types=tuple(up_block_types),
-        block_out_channels=tuple(block_out_channels),
-        latent_channels=VAE_PARAMS_Z_CHANNELS,
-        layers_per_block=VAE_PARAMS_NUM_RES_BLOCKS,
-    )
-    return config
-
-
-def convert_ldm_clip_checkpoint_v1(checkpoint):
-    keys = list(checkpoint.keys())
-    text_model_dict = {}
-    for key in keys:
-        if key.startswith("cond_stage_model.transformer"):
-            text_model_dict[key[len("cond_stage_model.transformer.") :]] = checkpoint[key]
-    return text_model_dict
-
-
-def convert_ldm_clip_checkpoint_v2(checkpoint, max_length):
-    # 嫌になるくらい違うぞ！
-    def convert_key(key):
-        if not key.startswith("cond_stage_model"):
-            return None
-
-        # common conversion
-        key = key.replace("cond_stage_model.model.transformer.", "text_model.encoder.")
-        key = key.replace("cond_stage_model.model.", "text_model.")
-
-        if "resblocks" in key:
-            # resblocks conversion
-            key = key.replace(".resblocks.", ".layers.")
-            if ".ln_" in key:
-                key = key.replace(".ln_", ".layer_norm")
-            elif ".mlp." in key:
-                key = key.replace(".c_fc.", ".fc1.")
-                key = key.replace(".c_proj.", ".fc2.")
-            elif ".attn.out_proj" in key:
-                key = key.replace(".attn.out_proj.", ".self_attn.out_proj.")
-            elif ".attn.in_proj" in key:
-                key = None  # 特殊なので後で処理する
-            else:
-                raise ValueError(f"unexpected key in SD: {key}")
-        elif ".positional_embedding" in key:
-            key = key.replace(".positional_embedding", ".embeddings.position_embedding.weight")
-        elif ".text_projection" in key:
-            key = None  # 使われない???
-        elif ".logit_scale" in key:
-            key = None  # 使われない???
-        elif ".token_embedding" in key:
-            key = key.replace(".token_embedding.weight", ".embeddings.token_embedding.weight")
-        elif ".ln_final" in key:
-            key = key.replace(".ln_final", ".final_layer_norm")
-        return key
-
-    keys = list(checkpoint.keys())
-    new_sd = {}
-    for key in keys:
-        # remove resblocks 23
-        if ".resblocks.23." in key:
-            continue
-        new_key = convert_key(key)
-        if new_key is None:
-            continue
-        new_sd[new_key] = checkpoint[key]
-
-    # attnの変換
-    for key in keys:
-        if ".resblocks.23." in key:
-            continue
-        if ".resblocks" in key and ".attn.in_proj_" in key:
-            # 三つに分割
-            values = torch.chunk(checkpoint[key], 3)
-
-            key_suffix = ".weight" if "weight" in key else ".bias"
-            key_pfx = key.replace("cond_stage_model.model.transformer.resblocks.", "text_model.encoder.layers.")
-            key_pfx = key_pfx.replace("_weight", "")
-            key_pfx = key_pfx.replace("_bias", "")
-            key_pfx = key_pfx.replace(".attn.in_proj", ".self_attn.")
-            new_sd[key_pfx + "q_proj" + key_suffix] = values[0]
-            new_sd[key_pfx + "k_proj" + key_suffix] = values[1]
-            new_sd[key_pfx + "v_proj" + key_suffix] = values[2]
-
-    # rename or add position_ids
-    ANOTHER_POSITION_IDS_KEY = "text_model.encoder.text_model.embeddings.position_ids"
-    if ANOTHER_POSITION_IDS_KEY in new_sd:
-        # waifu diffusion v1.4
-        position_ids = new_sd[ANOTHER_POSITION_IDS_KEY]
-        del new_sd[ANOTHER_POSITION_IDS_KEY]
-    else:
-        position_ids = torch.Tensor([list(range(max_length))]).to(torch.int64)
-
-    new_sd["text_model.embeddings.position_ids"] = position_ids
-    return new_sd
-
-
-# endregion
-
-
-# region Diffusers->StableDiffusion の変換コード
-# convert_diffusers_to_original_stable_diffusion をコピーして修正している（ASL 2.0）
-
-
-def conv_transformer_to_linear(checkpoint):
-    keys = list(checkpoint.keys())
-    tf_keys = ["proj_in.weight", "proj_out.weight"]
-    for key in keys:
-        if ".".join(key.split(".")[-2:]) in tf_keys:
-            if checkpoint[key].ndim > 2:
-                checkpoint[key] = checkpoint[key][:, :, 0, 0]
-
-
-def convert_unet_state_dict_to_sd(v2, unet_state_dict):
-    unet_conversion_map = [
-        # (stable-diffusion, HF Diffusers)
-        ("time_embed.0.weight", "time_embedding.linear_1.weight"),
-        ("time_embed.0.bias", "time_embedding.linear_1.bias"),
-        ("time_embed.2.weight", "time_embedding.linear_2.weight"),
-        ("time_embed.2.bias", "time_embedding.linear_2.bias"),
-        ("input_blocks.0.0.weight", "conv_in.weight"),
-        ("input_blocks.0.0.bias", "conv_in.bias"),
-        ("out.0.weight", "conv_norm_out.weight"),
-        ("out.0.bias", "conv_norm_out.bias"),
-        ("out.2.weight", "conv_out.weight"),
-        ("out.2.bias", "conv_out.bias"),
-    ]
-
-    unet_conversion_map_resnet = [
-        # (stable-diffusion, HF Diffusers)
-        ("in_layers.0", "norm1"),
-        ("in_layers.2", "conv1"),
-        ("out_layers.0", "norm2"),
-        ("out_layers.3", "conv2"),
-        ("emb_layers.1", "time_emb_proj"),
-        ("skip_connection", "conv_shortcut"),
-    ]
-
-    unet_conversion_map_layer = []
-    for i in range(4):
-        # loop over downblocks/upblocks
-
-        for j in range(2):
-            # loop over resnets/attentions for downblocks
-            hf_down_res_prefix = f"down_blocks.{i}.resnets.{j}."
-            sd_down_res_prefix = f"input_blocks.{3*i + j + 1}.0."
-            unet_conversion_map_layer.append((sd_down_res_prefix, hf_down_res_prefix))
-
-            if i < 3:
-                # no attention layers in down_blocks.3
-                hf_down_atn_prefix = f"down_blocks.{i}.attentions.{j}."
-                sd_down_atn_prefix = f"input_blocks.{3*i + j + 1}.1."
-                unet_conversion_map_layer.append((sd_down_atn_prefix, hf_down_atn_prefix))
-
-        for j in range(3):
-            # loop over resnets/attentions for upblocks
-            hf_up_res_prefix = f"up_blocks.{i}.resnets.{j}."
-            sd_up_res_prefix = f"output_blocks.{3*i + j}.0."
-            unet_conversion_map_layer.append((sd_up_res_prefix, hf_up_res_prefix))
-
-            if i > 0:
-                # no attention layers in up_blocks.0
-                hf_up_atn_prefix = f"up_blocks.{i}.attentions.{j}."
-                sd_up_atn_prefix = f"output_blocks.{3*i + j}.1."
-                unet_conversion_map_layer.append((sd_up_atn_prefix, hf_up_atn_prefix))
-
-        if i < 3:
-            # no downsample in down_blocks.3
-            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0.conv."
-            sd_downsample_prefix = f"input_blocks.{3*(i+1)}.0.op."
-            unet_conversion_map_layer.append((sd_downsample_prefix, hf_downsample_prefix))
-
-            # no upsample in up_blocks.3
-            hf_upsample_prefix = f"up_blocks.{i}.upsamplers.0."
-            sd_upsample_prefix = f"output_blocks.{3*i + 2}.{1 if i == 0 else 2}."
-            unet_conversion_map_layer.append((sd_upsample_prefix, hf_upsample_prefix))
-
-    hf_mid_atn_prefix = "mid_block.attentions.0."
-    sd_mid_atn_prefix = "middle_block.1."
-    unet_conversion_map_layer.append((sd_mid_atn_prefix, hf_mid_atn_prefix))
-
-    for j in range(2):
-        hf_mid_res_prefix = f"mid_block.resnets.{j}."
-        sd_mid_res_prefix = f"middle_block.{2*j}."
-        unet_conversion_map_layer.append((sd_mid_res_prefix, hf_mid_res_prefix))
-
-    # buyer beware: this is a *brittle* function,
-    # and correct output requires that all of these pieces interact in
-    # the exact order in which I have arranged them.
-    mapping = {k: k for k in unet_state_dict.keys()}
-    for sd_name, hf_name in unet_conversion_map:
-        mapping[hf_name] = sd_name
-    for k, v in mapping.items():
-        if "resnets" in k:
-            for sd_part, hf_part in unet_conversion_map_resnet:
-                v = v.replace(hf_part, sd_part)
-            mapping[k] = v
-    for k, v in mapping.items():
-        for sd_part, hf_part in unet_conversion_map_layer:
-            v = v.replace(hf_part, sd_part)
-        mapping[k] = v
-    new_state_dict = {v: unet_state_dict[k] for k, v in mapping.items()}
-
-    if v2:
-        conv_transformer_to_linear(new_state_dict)
-
-    return new_state_dict
-
-
-# ================#
-# VAE Conversion #
-# ================#
-
-
-def reshape_weight_for_sd(w):
-    # convert HF linear weights to SD conv2d weights
-    return w.reshape(*w.shape, 1, 1)
-
-
-def convert_vae_state_dict(vae_state_dict):
-    vae_conversion_map = [
-        # (stable-diffusion, HF Diffusers)
-        ("nin_shortcut", "conv_shortcut"),
-        ("norm_out", "conv_norm_out"),
-        ("mid.attn_1.", "mid_block.attentions.0."),
-    ]
-
-    for i in range(4):
-        # down_blocks have two resnets
-        for j in range(2):
-            hf_down_prefix = f"encoder.down_blocks.{i}.resnets.{j}."
-            sd_down_prefix = f"encoder.down.{i}.block.{j}."
-            vae_conversion_map.append((sd_down_prefix, hf_down_prefix))
-
-        if i < 3:
-            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0."
-            sd_downsample_prefix = f"down.{i}.downsample."
-            vae_conversion_map.append((sd_downsample_prefix, hf_downsample_prefix))
-
-            hf_upsample_prefix = f"up_blocks.{i}.upsamplers.0."
-            sd_upsample_prefix = f"up.{3-i}.upsample."
-            vae_conversion_map.append((sd_upsample_prefix, hf_upsample_prefix))
-
-        # up_blocks have three resnets
-        # also, up blocks in hf are numbered in reverse from sd
-        for j in range(3):
-            hf_up_prefix = f"decoder.up_blocks.{i}.resnets.{j}."
-            sd_up_prefix = f"decoder.up.{3-i}.block.{j}."
-            vae_conversion_map.append((sd_up_prefix, hf_up_prefix))
-
-    # this part accounts for mid blocks in both the encoder and the decoder
-    for i in range(2):
-        hf_mid_res_prefix = f"mid_block.resnets.{i}."
-        sd_mid_res_prefix = f"mid.block_{i+1}."
-        vae_conversion_map.append((sd_mid_res_prefix, hf_mid_res_prefix))
-
-    vae_conversion_map_attn = [
-        # (stable-diffusion, HF Diffusers)
-        ("norm.", "group_norm."),
-        ("q.", "query."),
-        ("k.", "key."),
-        ("v.", "value."),
-        ("proj_out.", "proj_attn."),
-    ]
-
-    mapping = {k: k for k in vae_state_dict.keys()}
-    for k, v in mapping.items():
-        for sd_part, hf_part in vae_conversion_map:
-            v = v.replace(hf_part, sd_part)
-        mapping[k] = v
-    for k, v in mapping.items():
-        if "attentions" in k:
-            for sd_part, hf_part in vae_conversion_map_attn:
-                v = v.replace(hf_part, sd_part)
-            mapping[k] = v
-    new_state_dict = {v: vae_state_dict[k] for k, v in mapping.items()}
-    weights_to_convert = ["q", "k", "v", "proj_out"]
-    for k, v in new_state_dict.items():
-        for weight_name in weights_to_convert:
-            if f"mid.attn_1.{weight_name}.weight" in k:
-                # print(f"Reshaping {k} for SD format")
-                new_state_dict[k] = reshape_weight_for_sd(v)
-
-    return new_state_dict
-
-
-# endregion
-
-# region 自作のモデル読み書きなど
-
-
-def is_safetensors(path):
-    return os.path.splitext(path)[1].lower() == ".safetensors"
-
-
-def load_checkpoint_with_text_encoder_conversion(ckpt_path, device="cpu"):
-    # text encoderの格納形式が違うモデルに対応する ('text_model'がない)
-    TEXT_ENCODER_KEY_REPLACEMENTS = [
-        ("cond_stage_model.transformer.embeddings.", "cond_stage_model.transformer.text_model.embeddings."),
-        ("cond_stage_model.transformer.encoder.", "cond_stage_model.transformer.text_model.encoder."),
-        ("cond_stage_model.transformer.final_layer_norm.", "cond_stage_model.transformer.text_model.final_layer_norm."),
-    ]
-
-    if is_safetensors(ckpt_path):
-        checkpoint = None
-        state_dict = load_file(ckpt_path)  # , device) # may causes error
-    else:
-        checkpoint = torch.load(ckpt_path, map_location=device)
-        if "state_dict" in checkpoint:
-            state_dict = checkpoint["state_dict"]
-        else:
-            state_dict = checkpoint
-            checkpoint = None
-
-    key_reps = []
-    for rep_from, rep_to in TEXT_ENCODER_KEY_REPLACEMENTS:
-        for key in state_dict.keys():
-            if key.startswith(rep_from):
-                new_key = rep_to + key[len(rep_from) :]
-                key_reps.append((key, new_key))
-
-    for key, new_key in key_reps:
-        state_dict[new_key] = state_dict[key]
-        del state_dict[key]
-
-    return checkpoint, state_dict
-
-
-# TODO dtype指定の動作が怪しいので確認する text_encoderを指定形式で作れるか未確認
-def load_models_from_stable_diffusion_checkpoint(v2, ckpt_path, device="cpu", dtype=None):
-    _, state_dict = load_checkpoint_with_text_encoder_conversion(ckpt_path, device)
-
-    # Convert the UNet2DConditionModel model.
-    unet_config = create_unet_diffusers_config(v2)
-    converted_unet_checkpoint = convert_ldm_unet_checkpoint(v2, state_dict, unet_config)
-
-    unet = UNet2DConditionModel(**unet_config).to(device)
-    info = unet.load_state_dict(converted_unet_checkpoint)
-    print("loading u-net:", info)
-
-    # Convert the VAE model.
-    vae_config = create_vae_diffusers_config()
-    converted_vae_checkpoint = convert_ldm_vae_checkpoint(state_dict, vae_config)
-
-    vae = AutoencoderKL(**vae_config).to(device)
-    info = vae.load_state_dict(converted_vae_checkpoint)
-    print("loading vae:", info)
-
-    # convert text_model
-    if v2:
-        converted_text_encoder_checkpoint = convert_ldm_clip_checkpoint_v2(state_dict, 77)
-        cfg = CLIPTextConfig(
-            vocab_size=49408,
-            hidden_size=1024,
-            intermediate_size=4096,
-            num_hidden_layers=23,
-            num_attention_heads=16,
-            max_position_embeddings=77,
-            hidden_act="gelu",
-            layer_norm_eps=1e-05,
-            dropout=0.0,
-            attention_dropout=0.0,
-            initializer_range=0.02,
-            initializer_factor=1.0,
-            pad_token_id=1,
-            bos_token_id=0,
-            eos_token_id=2,
-            model_type="clip_text_model",
-            projection_dim=512,
-            torch_dtype="float32",
-            transformers_version="4.25.0.dev0",
-        )
-        text_model = CLIPTextModel._from_config(cfg)
-        info = text_model.load_state_dict(converted_text_encoder_checkpoint)
-    else:
-        converted_text_encoder_checkpoint = convert_ldm_clip_checkpoint_v1(state_dict)
-
-        logging.set_verbosity_error()  # don't show annoying warning
-        text_model = CLIPTextModel.from_pretrained("openai/clip-vit-large-patch14").to(device)
-        logging.set_verbosity_warning()
-
-        info = text_model.load_state_dict(converted_text_encoder_checkpoint)
-    print("loading text encoder:", info)
-
-    return text_model, vae, unet
-
-
-def convert_text_encoder_state_dict_to_sd_v2(checkpoint, make_dummy_weights=False):
-    def convert_key(key):
-        # position_idsの除去
-        if ".position_ids" in key:
-            return None
-
-        # common
-        key = key.replace("text_model.encoder.", "transformer.")
-        key = key.replace("text_model.", "")
-        if "layers" in key:
-            # resblocks conversion
-            key = key.replace(".layers.", ".resblocks.")
-            if ".layer_norm" in key:
-                key = key.replace(".layer_norm", ".ln_")
-            elif ".mlp." in key:
-                key = key.replace(".fc1.", ".c_fc.")
-                key = key.replace(".fc2.", ".c_proj.")
-            elif ".self_attn.out_proj" in key:
-                key = key.replace(".self_attn.out_proj.", ".attn.out_proj.")
-            elif ".self_attn." in key:
-                key = None  # 特殊なので後で処理する
-            else:
-                raise ValueError(f"unexpected key in DiffUsers model: {key}")
-        elif ".position_embedding" in key:
-            key = key.replace("embeddings.position_embedding.weight", "positional_embedding")
-        elif ".token_embedding" in key:
-            key = key.replace("embeddings.token_embedding.weight", "token_embedding.weight")
-        elif "final_layer_norm" in key:
-            key = key.replace("final_layer_norm", "ln_final")
-        return key
-
-    keys = list(checkpoint.keys())
-    new_sd = {}
-    for key in keys:
-        new_key = convert_key(key)
-        if new_key is None:
-            continue
-        new_sd[new_key] = checkpoint[key]
-
-    # attnの変換
-    for key in keys:
-        if "layers" in key and "q_proj" in key:
-            # 三つを結合
-            key_q = key
-            key_k = key.replace("q_proj", "k_proj")
-            key_v = key.replace("q_proj", "v_proj")
-
-            value_q = checkpoint[key_q]
-            value_k = checkpoint[key_k]
-            value_v = checkpoint[key_v]
-            value = torch.cat([value_q, value_k, value_v])
-
-            new_key = key.replace("text_model.encoder.layers.", "transformer.resblocks.")
-            new_key = new_key.replace(".self_attn.q_proj.", ".attn.in_proj_")
-            new_sd[new_key] = value
-
-    # 最後の層などを捏造するか
-    if make_dummy_weights:
-        print("make dummy weights for resblock.23, text_projection and logit scale.")
-        keys = list(new_sd.keys())
-        for key in keys:
-            if key.startswith("transformer.resblocks.22."):
-                new_sd[key.replace(".22.", ".23.")] = new_sd[key].clone()  # copyしないとsafetensorsの保存で落ちる
-
-        # Diffusersに含まれない重みを作っておく
-        new_sd["text_projection"] = torch.ones((1024, 1024), dtype=new_sd[keys[0]].dtype, device=new_sd[keys[0]].device)
-        new_sd["logit_scale"] = torch.tensor(1)
-
-    return new_sd
-
-
-def save_stable_diffusion_checkpoint(v2, output_file, text_encoder, unet, ckpt_path, epochs, steps, save_dtype=None, vae=None):
-    if ckpt_path is not None:
-        # epoch/stepを参照する。またVAEがメモリ上にないときなど、もう一度VAEを含めて読み込む
-        checkpoint, state_dict = load_checkpoint_with_text_encoder_conversion(ckpt_path)
-        if checkpoint is None:  # safetensors または state_dictのckpt
-            checkpoint = {}
-            strict = False
-        else:
-            strict = True
-        if "state_dict" in state_dict:
-            del state_dict["state_dict"]
-    else:
-        # 新しく作る
-        assert vae is not None, "VAE is required to save a checkpoint without a given checkpoint"
-        checkpoint = {}
-        state_dict = {}
-        strict = False
-
-    def update_sd(prefix, sd):
-        for k, v in sd.items():
-            key = prefix + k
-            assert not strict or key in state_dict, f"Illegal key in save SD: {key}"
-            if save_dtype is not None:
-                v = v.detach().clone().to("cpu").to(save_dtype)
-            state_dict[key] = v
-
-    # Convert the UNet model
-    unet_state_dict = convert_unet_state_dict_to_sd(v2, unet.state_dict())
-    update_sd("model.diffusion_model.", unet_state_dict)
-
-    # Convert the text encoder model
-    if v2:
-        make_dummy = ckpt_path is None  # 参照元のcheckpointがない場合は最後の層を前の層から複製して作るなどダミーの重みを入れる
-        text_enc_dict = convert_text_encoder_state_dict_to_sd_v2(text_encoder.state_dict(), make_dummy)
-        update_sd("cond_stage_model.model.", text_enc_dict)
-    else:
-        text_enc_dict = text_encoder.state_dict()
-        update_sd("cond_stage_model.transformer.", text_enc_dict)
-
-    # Convert the VAE
-    if vae is not None:
-        vae_dict = convert_vae_state_dict(vae.state_dict())
-        update_sd("first_stage_model.", vae_dict)
-
-    # Put together new checkpoint
-    key_count = len(state_dict.keys())
-    new_ckpt = {"state_dict": state_dict}
-
-    # epoch and global_step are sometimes not int
-    try:
-        if "epoch" in checkpoint:
-            epochs += checkpoint["epoch"]
-        if "global_step" in checkpoint:
-            steps += checkpoint["global_step"]
-    except:
-        pass
-
-    new_ckpt["epoch"] = epochs
-    new_ckpt["global_step"] = steps
-
-    if is_safetensors(output_file):
-        # TODO Tensor以外のdictの値を削除したほうがいいか
-        save_file(state_dict, output_file)
-    else:
-        torch.save(new_ckpt, output_file)
-
-    return key_count
-
-
-def save_diffusers_checkpoint(v2, output_dir, text_encoder, unet, pretrained_model_name_or_path, vae=None, use_safetensors=False):
-    if pretrained_model_name_or_path is None:
-        # load default settings for v1/v2
-        if v2:
-            pretrained_model_name_or_path = DIFFUSERS_REF_MODEL_ID_V2
-        else:
-            pretrained_model_name_or_path = DIFFUSERS_REF_MODEL_ID_V1
-
-    scheduler = DDIMScheduler.from_pretrained(pretrained_model_name_or_path, subfolder="scheduler")
-    tokenizer = CLIPTokenizer.from_pretrained(pretrained_model_name_or_path, subfolder="tokenizer")
-    if vae is None:
-        vae = AutoencoderKL.from_pretrained(pretrained_model_name_or_path, subfolder="vae")
-
-    pipeline = StableDiffusionPipeline(
-        unet=unet,
-        text_encoder=text_encoder,
-        vae=vae,
-        scheduler=scheduler,
-        tokenizer=tokenizer,
-        safety_checker=None,
-        feature_extractor=None,
-        requires_safety_checker=None,
-    )
-    pipeline.save_pretrained(output_dir, safe_serialization=use_safetensors)
-
-
-VAE_PREFIX = "first_stage_model."
-
-
-def load_vae(vae_id, dtype):
-    print(f"load VAE: {vae_id}")
-    if os.path.isdir(vae_id) or not os.path.isfile(vae_id):
-        # Diffusers local/remote
-        try:
-            vae = AutoencoderKL.from_pretrained(vae_id, subfolder=None, torch_dtype=dtype)
-        except EnvironmentError as e:
-            print(f"exception occurs in loading vae: {e}")
-            print("retry with subfolder='vae'")
-            vae = AutoencoderKL.from_pretrained(vae_id, subfolder="vae", torch_dtype=dtype)
-        return vae
-
-    # local
-    vae_config = create_vae_diffusers_config()
-
-    if vae_id.endswith(".bin"):
-        # SD 1.5 VAE on Huggingface
-        converted_vae_checkpoint = torch.load(vae_id, map_location="cpu")
-    else:
-        # StableDiffusion
-        vae_model = load_file(vae_id, "cpu") if is_safetensors(vae_id) else torch.load(vae_id, map_location="cpu")
-        vae_sd = vae_model["state_dict"] if "state_dict" in vae_model else vae_model
-
-        # vae only or full model
-        full_model = False
-        for vae_key in vae_sd:
-            if vae_key.startswith(VAE_PREFIX):
-                full_model = True
-                break
-        if not full_model:
-            sd = {}
-            for key, value in vae_sd.items():
-                sd[VAE_PREFIX + key] = value
-            vae_sd = sd
-            del sd
-
-        # Convert the VAE model.
-        converted_vae_checkpoint = convert_ldm_vae_checkpoint(vae_sd, vae_config)
-
-    vae = AutoencoderKL(**vae_config)
-    vae.load_state_dict(converted_vae_checkpoint)
-    return vae
-
-
-# endregion
-
-
-def make_bucket_resolutions(max_reso, min_size=256, max_size=1024, divisible=64):
-    max_width, max_height = max_reso
-    max_area = (max_width // divisible) * (max_height // divisible)
-
-    resos = set()
-
-    size = int(math.sqrt(max_area)) * divisible
-    resos.add((size, size))
-
-    size = min_size
-    while size <= max_size:
-        width = size
-        height = min(max_size, (max_area // (width // divisible)) * divisible)
-        resos.add((width, height))
-        resos.add((height, width))
-
-        # # make additional resos
-        # if width >= height and width - divisible >= min_size:
-        #   resos.add((width - divisible, height))
-        #   resos.add((height, width - divisible))
-        # if height >= width and height - divisible >= min_size:
-        #   resos.add((width, height - divisible))
-        #   resos.add((height - divisible, width))
-
-        size += divisible
-
-    resos = list(resos)
-    resos.sort()
-    return resos
-
-
-if __name__ == "__main__":
-    resos = make_bucket_resolutions((512, 768))
-    print(len(resos))
-    print(resos)
-    aspect_ratios = [w / h for w, h in resos]
-    print(aspect_ratios)
-
-    ars = set()
-    for ar in aspect_ratios:
-        if ar in ars:
-            print("error! duplicate ar:", ar)
-        ars.add(ar)
+# v1: split from train_db_fixed.py.
+# v2: support safetensors
+
+import math
+import os
+import torch
+from transformers import CLIPTextModel, CLIPTokenizer, CLIPTextConfig, logging
+from diffusers import AutoencoderKL, DDIMScheduler, StableDiffusionPipeline, UNet2DConditionModel
+from safetensors.torch import load_file, save_file
+
+# DiffUsers版StableDiffusionのモデルパラメータ
+NUM_TRAIN_TIMESTEPS = 1000
+BETA_START = 0.00085
+BETA_END = 0.0120
+
+UNET_PARAMS_MODEL_CHANNELS = 320
+UNET_PARAMS_CHANNEL_MULT = [1, 2, 4, 4]
+UNET_PARAMS_ATTENTION_RESOLUTIONS = [4, 2, 1]
+UNET_PARAMS_IMAGE_SIZE = 64  # fixed from old invalid value `32`
+UNET_PARAMS_IN_CHANNELS = 4
+UNET_PARAMS_OUT_CHANNELS = 4
+UNET_PARAMS_NUM_RES_BLOCKS = 2
+UNET_PARAMS_CONTEXT_DIM = 768
+UNET_PARAMS_NUM_HEADS = 8
+
+VAE_PARAMS_Z_CHANNELS = 4
+VAE_PARAMS_RESOLUTION = 256
+VAE_PARAMS_IN_CHANNELS = 3
+VAE_PARAMS_OUT_CH = 3
+VAE_PARAMS_CH = 128
+VAE_PARAMS_CH_MULT = [1, 2, 4, 4]
+VAE_PARAMS_NUM_RES_BLOCKS = 2
+
+# V2
+V2_UNET_PARAMS_ATTENTION_HEAD_DIM = [5, 10, 20, 20]
+V2_UNET_PARAMS_CONTEXT_DIM = 1024
+
+# Diffusersの設定を読み込むための参照モデル
+DIFFUSERS_REF_MODEL_ID_V1 = "runwayml/stable-diffusion-v1-5"
+DIFFUSERS_REF_MODEL_ID_V2 = "stabilityai/stable-diffusion-2-1"
+
+
+# region StableDiffusion->Diffusersの変換コード
+# convert_original_stable_diffusion_to_diffusers をコピーして修正している（ASL 2.0）
+
+
+def shave_segments(path, n_shave_prefix_segments=1):
+    """
+    Removes segments. Positive values shave the first segments, negative shave the last segments.
+    """
+    if n_shave_prefix_segments >= 0:
+        return ".".join(path.split(".")[n_shave_prefix_segments:])
+    else:
+        return ".".join(path.split(".")[:n_shave_prefix_segments])
+
+
+def renew_resnet_paths(old_list, n_shave_prefix_segments=0):
+    """
+    Updates paths inside resnets to the new naming scheme (local renaming)
+    """
+    mapping = []
+    for old_item in old_list:
+        new_item = old_item.replace("in_layers.0", "norm1")
+        new_item = new_item.replace("in_layers.2", "conv1")
+
+        new_item = new_item.replace("out_layers.0", "norm2")
+        new_item = new_item.replace("out_layers.3", "conv2")
+
+        new_item = new_item.replace("emb_layers.1", "time_emb_proj")
+        new_item = new_item.replace("skip_connection", "conv_shortcut")
+
+        new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
+
+        mapping.append({"old": old_item, "new": new_item})
+
+    return mapping
+
+
+def renew_vae_resnet_paths(old_list, n_shave_prefix_segments=0):
+    """
+    Updates paths inside resnets to the new naming scheme (local renaming)
+    """
+    mapping = []
+    for old_item in old_list:
+        new_item = old_item
+
+        new_item = new_item.replace("nin_shortcut", "conv_shortcut")
+        new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
+
+        mapping.append({"old": old_item, "new": new_item})
+
+    return mapping
+
+
+def renew_attention_paths(old_list, n_shave_prefix_segments=0):
+    """
+    Updates paths inside attentions to the new naming scheme (local renaming)
+    """
+    mapping = []
+    for old_item in old_list:
+        new_item = old_item
+
+        #         new_item = new_item.replace('norm.weight', 'group_norm.weight')
+        #         new_item = new_item.replace('norm.bias', 'group_norm.bias')
+
+        #         new_item = new_item.replace('proj_out.weight', 'proj_attn.weight')
+        #         new_item = new_item.replace('proj_out.bias', 'proj_attn.bias')
+
+        #         new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
+
+        mapping.append({"old": old_item, "new": new_item})
+
+    return mapping
+
+
+def renew_vae_attention_paths(old_list, n_shave_prefix_segments=0):
+    """
+    Updates paths inside attentions to the new naming scheme (local renaming)
+    """
+    mapping = []
+    for old_item in old_list:
+        new_item = old_item
+
+        new_item = new_item.replace("norm.weight", "group_norm.weight")
+        new_item = new_item.replace("norm.bias", "group_norm.bias")
+
+        new_item = new_item.replace("q.weight", "query.weight")
+        new_item = new_item.replace("q.bias", "query.bias")
+
+        new_item = new_item.replace("k.weight", "key.weight")
+        new_item = new_item.replace("k.bias", "key.bias")
+
+        new_item = new_item.replace("v.weight", "value.weight")
+        new_item = new_item.replace("v.bias", "value.bias")
+
+        new_item = new_item.replace("proj_out.weight", "proj_attn.weight")
+        new_item = new_item.replace("proj_out.bias", "proj_attn.bias")
+
+        new_item = shave_segments(new_item, n_shave_prefix_segments=n_shave_prefix_segments)
+
+        mapping.append({"old": old_item, "new": new_item})
+
+    return mapping
+
+
+def assign_to_checkpoint(
+    paths, checkpoint, old_checkpoint, attention_paths_to_split=None, additional_replacements=None, config=None
+):
+    """
+    This does the final conversion step: take locally converted weights and apply a global renaming
+    to them. It splits attention layers, and takes into account additional replacements
+    that may arise.
+
+    Assigns the weights to the new checkpoint.
+    """
+    assert isinstance(paths, list), "Paths should be a list of dicts containing 'old' and 'new' keys."
+
+    # Splits the attention layers into three variables.
+    if attention_paths_to_split is not None:
+        for path, path_map in attention_paths_to_split.items():
+            old_tensor = old_checkpoint[path]
+            channels = old_tensor.shape[0] // 3
+
+            target_shape = (-1, channels) if len(old_tensor.shape) == 3 else (-1)
+
+            num_heads = old_tensor.shape[0] // config["num_head_channels"] // 3
+
+            old_tensor = old_tensor.reshape((num_heads, 3 * channels // num_heads) + old_tensor.shape[1:])
+            query, key, value = old_tensor.split(channels // num_heads, dim=1)
+
+            checkpoint[path_map["query"]] = query.reshape(target_shape)
+            checkpoint[path_map["key"]] = key.reshape(target_shape)
+            checkpoint[path_map["value"]] = value.reshape(target_shape)
+
+    for path in paths:
+        new_path = path["new"]
+
+        # These have already been assigned
+        if attention_paths_to_split is not None and new_path in attention_paths_to_split:
+            continue
+
+        # Global renaming happens here
+        new_path = new_path.replace("middle_block.0", "mid_block.resnets.0")
+        new_path = new_path.replace("middle_block.1", "mid_block.attentions.0")
+        new_path = new_path.replace("middle_block.2", "mid_block.resnets.1")
+
+        if additional_replacements is not None:
+            for replacement in additional_replacements:
+                new_path = new_path.replace(replacement["old"], replacement["new"])
+
+        # proj_attn.weight has to be converted from conv 1D to linear
+        if "proj_attn.weight" in new_path:
+            checkpoint[new_path] = old_checkpoint[path["old"]][:, :, 0]
+        else:
+            checkpoint[new_path] = old_checkpoint[path["old"]]
+
+
+def conv_attn_to_linear(checkpoint):
+    keys = list(checkpoint.keys())
+    attn_keys = ["query.weight", "key.weight", "value.weight"]
+    for key in keys:
+        if ".".join(key.split(".")[-2:]) in attn_keys:
+            if checkpoint[key].ndim > 2:
+                checkpoint[key] = checkpoint[key][:, :, 0, 0]
+        elif "proj_attn.weight" in key:
+            if checkpoint[key].ndim > 2:
+                checkpoint[key] = checkpoint[key][:, :, 0]
+
+
+def linear_transformer_to_conv(checkpoint):
+    keys = list(checkpoint.keys())
+    tf_keys = ["proj_in.weight", "proj_out.weight"]
+    for key in keys:
+        if ".".join(key.split(".")[-2:]) in tf_keys:
+            if checkpoint[key].ndim == 2:
+                checkpoint[key] = checkpoint[key].unsqueeze(2).unsqueeze(2)
+
+
+def convert_ldm_unet_checkpoint(v2, checkpoint, config):
+    """
+    Takes a state dict and a config, and returns a converted checkpoint.
+    """
+
+    # extract state_dict for UNet
+    unet_state_dict = {}
+    unet_key = "model.diffusion_model."
+    keys = list(checkpoint.keys())
+    for key in keys:
+        if key.startswith(unet_key):
+            unet_state_dict[key.replace(unet_key, "")] = checkpoint.pop(key)
+
+    new_checkpoint = {}
+
+    new_checkpoint["time_embedding.linear_1.weight"] = unet_state_dict["time_embed.0.weight"]
+    new_checkpoint["time_embedding.linear_1.bias"] = unet_state_dict["time_embed.0.bias"]
+    new_checkpoint["time_embedding.linear_2.weight"] = unet_state_dict["time_embed.2.weight"]
+    new_checkpoint["time_embedding.linear_2.bias"] = unet_state_dict["time_embed.2.bias"]
+
+    new_checkpoint["conv_in.weight"] = unet_state_dict["input_blocks.0.0.weight"]
+    new_checkpoint["conv_in.bias"] = unet_state_dict["input_blocks.0.0.bias"]
+
+    new_checkpoint["conv_norm_out.weight"] = unet_state_dict["out.0.weight"]
+    new_checkpoint["conv_norm_out.bias"] = unet_state_dict["out.0.bias"]
+    new_checkpoint["conv_out.weight"] = unet_state_dict["out.2.weight"]
+    new_checkpoint["conv_out.bias"] = unet_state_dict["out.2.bias"]
+
+    # Retrieves the keys for the input blocks only
+    num_input_blocks = len({".".join(layer.split(".")[:2]) for layer in unet_state_dict if "input_blocks" in layer})
+    input_blocks = {
+        layer_id: [key for key in unet_state_dict if f"input_blocks.{layer_id}." in key] for layer_id in range(num_input_blocks)
+    }
+
+    # Retrieves the keys for the middle blocks only
+    num_middle_blocks = len({".".join(layer.split(".")[:2]) for layer in unet_state_dict if "middle_block" in layer})
+    middle_blocks = {
+        layer_id: [key for key in unet_state_dict if f"middle_block.{layer_id}." in key] for layer_id in range(num_middle_blocks)
+    }
+
+    # Retrieves the keys for the output blocks only
+    num_output_blocks = len({".".join(layer.split(".")[:2]) for layer in unet_state_dict if "output_blocks" in layer})
+    output_blocks = {
+        layer_id: [key for key in unet_state_dict if f"output_blocks.{layer_id}." in key] for layer_id in range(num_output_blocks)
+    }
+
+    for i in range(1, num_input_blocks):
+        block_id = (i - 1) // (config["layers_per_block"] + 1)
+        layer_in_block_id = (i - 1) % (config["layers_per_block"] + 1)
+
+        resnets = [key for key in input_blocks[i] if f"input_blocks.{i}.0" in key and f"input_blocks.{i}.0.op" not in key]
+        attentions = [key for key in input_blocks[i] if f"input_blocks.{i}.1" in key]
+
+        if f"input_blocks.{i}.0.op.weight" in unet_state_dict:
+            new_checkpoint[f"down_blocks.{block_id}.downsamplers.0.conv.weight"] = unet_state_dict.pop(
+                f"input_blocks.{i}.0.op.weight"
+            )
+            new_checkpoint[f"down_blocks.{block_id}.downsamplers.0.conv.bias"] = unet_state_dict.pop(f"input_blocks.{i}.0.op.bias")
+
+        paths = renew_resnet_paths(resnets)
+        meta_path = {"old": f"input_blocks.{i}.0", "new": f"down_blocks.{block_id}.resnets.{layer_in_block_id}"}
+        assign_to_checkpoint(paths, new_checkpoint, unet_state_dict, additional_replacements=[meta_path], config=config)
+
+        if len(attentions):
+            paths = renew_attention_paths(attentions)
+            meta_path = {"old": f"input_blocks.{i}.1", "new": f"down_blocks.{block_id}.attentions.{layer_in_block_id}"}
+            assign_to_checkpoint(paths, new_checkpoint, unet_state_dict, additional_replacements=[meta_path], config=config)
+
+    resnet_0 = middle_blocks[0]
+    attentions = middle_blocks[1]
+    resnet_1 = middle_blocks[2]
+
+    resnet_0_paths = renew_resnet_paths(resnet_0)
+    assign_to_checkpoint(resnet_0_paths, new_checkpoint, unet_state_dict, config=config)
+
+    resnet_1_paths = renew_resnet_paths(resnet_1)
+    assign_to_checkpoint(resnet_1_paths, new_checkpoint, unet_state_dict, config=config)
+
+    attentions_paths = renew_attention_paths(attentions)
+    meta_path = {"old": "middle_block.1", "new": "mid_block.attentions.0"}
+    assign_to_checkpoint(attentions_paths, new_checkpoint, unet_state_dict, additional_replacements=[meta_path], config=config)
+
+    for i in range(num_output_blocks):
+        block_id = i // (config["layers_per_block"] + 1)
+        layer_in_block_id = i % (config["layers_per_block"] + 1)
+        output_block_layers = [shave_segments(name, 2) for name in output_blocks[i]]
+        output_block_list = {}
+
+        for layer in output_block_layers:
+            layer_id, layer_name = layer.split(".")[0], shave_segments(layer, 1)
+            if layer_id in output_block_list:
+                output_block_list[layer_id].append(layer_name)
+            else:
+                output_block_list[layer_id] = [layer_name]
+
+        if len(output_block_list) > 1:
+            resnets = [key for key in output_blocks[i] if f"output_blocks.{i}.0" in key]
+            attentions = [key for key in output_blocks[i] if f"output_blocks.{i}.1" in key]
+
+            resnet_0_paths = renew_resnet_paths(resnets)
+            paths = renew_resnet_paths(resnets)
+
+            meta_path = {"old": f"output_blocks.{i}.0", "new": f"up_blocks.{block_id}.resnets.{layer_in_block_id}"}
+            assign_to_checkpoint(paths, new_checkpoint, unet_state_dict, additional_replacements=[meta_path], config=config)
+
+            # オリジナル：
+            # if ["conv.weight", "conv.bias"] in output_block_list.values():
+            #   index = list(output_block_list.values()).index(["conv.weight", "conv.bias"])
+
+            # biasとweightの順番に依存しないようにする：もっといいやり方がありそうだが
+            for l in output_block_list.values():
+                l.sort()
+
+            if ["conv.bias", "conv.weight"] in output_block_list.values():
+                index = list(output_block_list.values()).index(["conv.bias", "conv.weight"])
+                new_checkpoint[f"up_blocks.{block_id}.upsamplers.0.conv.bias"] = unet_state_dict[
+                    f"output_blocks.{i}.{index}.conv.bias"
+                ]
+                new_checkpoint[f"up_blocks.{block_id}.upsamplers.0.conv.weight"] = unet_state_dict[
+                    f"output_blocks.{i}.{index}.conv.weight"
+                ]
+
+                # Clear attentions as they have been attributed above.
+                if len(attentions) == 2:
+                    attentions = []
+
+            if len(attentions):
+                paths = renew_attention_paths(attentions)
+                meta_path = {
+                    "old": f"output_blocks.{i}.1",
+                    "new": f"up_blocks.{block_id}.attentions.{layer_in_block_id}",
+                }
+                assign_to_checkpoint(paths, new_checkpoint, unet_state_dict, additional_replacements=[meta_path], config=config)
+        else:
+            resnet_0_paths = renew_resnet_paths(output_block_layers, n_shave_prefix_segments=1)
+            for path in resnet_0_paths:
+                old_path = ".".join(["output_blocks", str(i), path["old"]])
+                new_path = ".".join(["up_blocks", str(block_id), "resnets", str(layer_in_block_id), path["new"]])
+
+                new_checkpoint[new_path] = unet_state_dict[old_path]
+
+    # SDのv2では1*1のconv2dがlinearに変わっているので、linear->convに変換する
+    if v2:
+        linear_transformer_to_conv(new_checkpoint)
+
+    return new_checkpoint
+
+
+def convert_ldm_vae_checkpoint(checkpoint, config):
+    # extract state dict for VAE
+    vae_state_dict = {}
+    vae_key = "first_stage_model."
+    keys = list(checkpoint.keys())
+    for key in keys:
+        if key.startswith(vae_key):
+            vae_state_dict[key.replace(vae_key, "")] = checkpoint.get(key)
+    # if len(vae_state_dict) == 0:
+    #   # 渡されたcheckpointは.ckptから読み込んだcheckpointではなくvaeのstate_dict
+    #   vae_state_dict = checkpoint
+
+    new_checkpoint = {}
+
+    new_checkpoint["encoder.conv_in.weight"] = vae_state_dict["encoder.conv_in.weight"]
+    new_checkpoint["encoder.conv_in.bias"] = vae_state_dict["encoder.conv_in.bias"]
+    new_checkpoint["encoder.conv_out.weight"] = vae_state_dict["encoder.conv_out.weight"]
+    new_checkpoint["encoder.conv_out.bias"] = vae_state_dict["encoder.conv_out.bias"]
+    new_checkpoint["encoder.conv_norm_out.weight"] = vae_state_dict["encoder.norm_out.weight"]
+    new_checkpoint["encoder.conv_norm_out.bias"] = vae_state_dict["encoder.norm_out.bias"]
+
+    new_checkpoint["decoder.conv_in.weight"] = vae_state_dict["decoder.conv_in.weight"]
+    new_checkpoint["decoder.conv_in.bias"] = vae_state_dict["decoder.conv_in.bias"]
+    new_checkpoint["decoder.conv_out.weight"] = vae_state_dict["decoder.conv_out.weight"]
+    new_checkpoint["decoder.conv_out.bias"] = vae_state_dict["decoder.conv_out.bias"]
+    new_checkpoint["decoder.conv_norm_out.weight"] = vae_state_dict["decoder.norm_out.weight"]
+    new_checkpoint["decoder.conv_norm_out.bias"] = vae_state_dict["decoder.norm_out.bias"]
+
+    new_checkpoint["quant_conv.weight"] = vae_state_dict["quant_conv.weight"]
+    new_checkpoint["quant_conv.bias"] = vae_state_dict["quant_conv.bias"]
+    new_checkpoint["post_quant_conv.weight"] = vae_state_dict["post_quant_conv.weight"]
+    new_checkpoint["post_quant_conv.bias"] = vae_state_dict["post_quant_conv.bias"]
+
+    # Retrieves the keys for the encoder down blocks only
+    num_down_blocks = len({".".join(layer.split(".")[:3]) for layer in vae_state_dict if "encoder.down" in layer})
+    down_blocks = {layer_id: [key for key in vae_state_dict if f"down.{layer_id}" in key] for layer_id in range(num_down_blocks)}
+
+    # Retrieves the keys for the decoder up blocks only
+    num_up_blocks = len({".".join(layer.split(".")[:3]) for layer in vae_state_dict if "decoder.up" in layer})
+    up_blocks = {layer_id: [key for key in vae_state_dict if f"up.{layer_id}" in key] for layer_id in range(num_up_blocks)}
+
+    for i in range(num_down_blocks):
+        resnets = [key for key in down_blocks[i] if f"down.{i}" in key and f"down.{i}.downsample" not in key]
+
+        if f"encoder.down.{i}.downsample.conv.weight" in vae_state_dict:
+            new_checkpoint[f"encoder.down_blocks.{i}.downsamplers.0.conv.weight"] = vae_state_dict.pop(
+                f"encoder.down.{i}.downsample.conv.weight"
+            )
+            new_checkpoint[f"encoder.down_blocks.{i}.downsamplers.0.conv.bias"] = vae_state_dict.pop(
+                f"encoder.down.{i}.downsample.conv.bias"
+            )
+
+        paths = renew_vae_resnet_paths(resnets)
+        meta_path = {"old": f"down.{i}.block", "new": f"down_blocks.{i}.resnets"}
+        assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
+
+    mid_resnets = [key for key in vae_state_dict if "encoder.mid.block" in key]
+    num_mid_res_blocks = 2
+    for i in range(1, num_mid_res_blocks + 1):
+        resnets = [key for key in mid_resnets if f"encoder.mid.block_{i}" in key]
+
+        paths = renew_vae_resnet_paths(resnets)
+        meta_path = {"old": f"mid.block_{i}", "new": f"mid_block.resnets.{i - 1}"}
+        assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
+
+    mid_attentions = [key for key in vae_state_dict if "encoder.mid.attn" in key]
+    paths = renew_vae_attention_paths(mid_attentions)
+    meta_path = {"old": "mid.attn_1", "new": "mid_block.attentions.0"}
+    assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
+    conv_attn_to_linear(new_checkpoint)
+
+    for i in range(num_up_blocks):
+        block_id = num_up_blocks - 1 - i
+        resnets = [key for key in up_blocks[block_id] if f"up.{block_id}" in key and f"up.{block_id}.upsample" not in key]
+
+        if f"decoder.up.{block_id}.upsample.conv.weight" in vae_state_dict:
+            new_checkpoint[f"decoder.up_blocks.{i}.upsamplers.0.conv.weight"] = vae_state_dict[
+                f"decoder.up.{block_id}.upsample.conv.weight"
+            ]
+            new_checkpoint[f"decoder.up_blocks.{i}.upsamplers.0.conv.bias"] = vae_state_dict[
+                f"decoder.up.{block_id}.upsample.conv.bias"
+            ]
+
+        paths = renew_vae_resnet_paths(resnets)
+        meta_path = {"old": f"up.{block_id}.block", "new": f"up_blocks.{i}.resnets"}
+        assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
+
+    mid_resnets = [key for key in vae_state_dict if "decoder.mid.block" in key]
+    num_mid_res_blocks = 2
+    for i in range(1, num_mid_res_blocks + 1):
+        resnets = [key for key in mid_resnets if f"decoder.mid.block_{i}" in key]
+
+        paths = renew_vae_resnet_paths(resnets)
+        meta_path = {"old": f"mid.block_{i}", "new": f"mid_block.resnets.{i - 1}"}
+        assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
+
+    mid_attentions = [key for key in vae_state_dict if "decoder.mid.attn" in key]
+    paths = renew_vae_attention_paths(mid_attentions)
+    meta_path = {"old": "mid.attn_1", "new": "mid_block.attentions.0"}
+    assign_to_checkpoint(paths, new_checkpoint, vae_state_dict, additional_replacements=[meta_path], config=config)
+    conv_attn_to_linear(new_checkpoint)
+    return new_checkpoint
+
+
+def create_unet_diffusers_config(v2):
+    """
+    Creates a config for the diffusers based on the config of the LDM model.
+    """
+    # unet_params = original_config.model.params.unet_config.params
+
+    block_out_channels = [UNET_PARAMS_MODEL_CHANNELS * mult for mult in UNET_PARAMS_CHANNEL_MULT]
+
+    down_block_types = []
+    resolution = 1
+    for i in range(len(block_out_channels)):
+        block_type = "CrossAttnDownBlock2D" if resolution in UNET_PARAMS_ATTENTION_RESOLUTIONS else "DownBlock2D"
+        down_block_types.append(block_type)
+        if i != len(block_out_channels) - 1:
+            resolution *= 2
+
+    up_block_types = []
+    for i in range(len(block_out_channels)):
+        block_type = "CrossAttnUpBlock2D" if resolution in UNET_PARAMS_ATTENTION_RESOLUTIONS else "UpBlock2D"
+        up_block_types.append(block_type)
+        resolution //= 2
+
+    config = dict(
+        sample_size=UNET_PARAMS_IMAGE_SIZE,
+        in_channels=UNET_PARAMS_IN_CHANNELS,
+        out_channels=UNET_PARAMS_OUT_CHANNELS,
+        down_block_types=tuple(down_block_types),
+        up_block_types=tuple(up_block_types),
+        block_out_channels=tuple(block_out_channels),
+        layers_per_block=UNET_PARAMS_NUM_RES_BLOCKS,
+        cross_attention_dim=UNET_PARAMS_CONTEXT_DIM if not v2 else V2_UNET_PARAMS_CONTEXT_DIM,
+        attention_head_dim=UNET_PARAMS_NUM_HEADS if not v2 else V2_UNET_PARAMS_ATTENTION_HEAD_DIM,
+    )
+
+    return config
+
+
+def create_vae_diffusers_config():
+    """
+    Creates a config for the diffusers based on the config of the LDM model.
+    """
+    # vae_params = original_config.model.params.first_stage_config.params.ddconfig
+    # _ = original_config.model.params.first_stage_config.params.embed_dim
+    block_out_channels = [VAE_PARAMS_CH * mult for mult in VAE_PARAMS_CH_MULT]
+    down_block_types = ["DownEncoderBlock2D"] * len(block_out_channels)
+    up_block_types = ["UpDecoderBlock2D"] * len(block_out_channels)
+
+    config = dict(
+        sample_size=VAE_PARAMS_RESOLUTION,
+        in_channels=VAE_PARAMS_IN_CHANNELS,
+        out_channels=VAE_PARAMS_OUT_CH,
+        down_block_types=tuple(down_block_types),
+        up_block_types=tuple(up_block_types),
+        block_out_channels=tuple(block_out_channels),
+        latent_channels=VAE_PARAMS_Z_CHANNELS,
+        layers_per_block=VAE_PARAMS_NUM_RES_BLOCKS,
+    )
+    return config
+
+
+def convert_ldm_clip_checkpoint_v1(checkpoint):
+    keys = list(checkpoint.keys())
+    text_model_dict = {}
+    for key in keys:
+        if key.startswith("cond_stage_model.transformer"):
+            text_model_dict[key[len("cond_stage_model.transformer.") :]] = checkpoint[key]
+    return text_model_dict
+
+
+def convert_ldm_clip_checkpoint_v2(checkpoint, max_length):
+    # 嫌になるくらい違うぞ！
+    def convert_key(key):
+        if not key.startswith("cond_stage_model"):
+            return None
+
+        # common conversion
+        key = key.replace("cond_stage_model.model.transformer.", "text_model.encoder.")
+        key = key.replace("cond_stage_model.model.", "text_model.")
+
+        if "resblocks" in key:
+            # resblocks conversion
+            key = key.replace(".resblocks.", ".layers.")
+            if ".ln_" in key:
+                key = key.replace(".ln_", ".layer_norm")
+            elif ".mlp." in key:
+                key = key.replace(".c_fc.", ".fc1.")
+                key = key.replace(".c_proj.", ".fc2.")
+            elif ".attn.out_proj" in key:
+                key = key.replace(".attn.out_proj.", ".self_attn.out_proj.")
+            elif ".attn.in_proj" in key:
+                key = None  # 特殊なので後で処理する
+            else:
+                raise ValueError(f"unexpected key in SD: {key}")
+        elif ".positional_embedding" in key:
+            key = key.replace(".positional_embedding", ".embeddings.position_embedding.weight")
+        elif ".text_projection" in key:
+            key = None  # 使われない???
+        elif ".logit_scale" in key:
+            key = None  # 使われない???
+        elif ".token_embedding" in key:
+            key = key.replace(".token_embedding.weight", ".embeddings.token_embedding.weight")
+        elif ".ln_final" in key:
+            key = key.replace(".ln_final", ".final_layer_norm")
+        return key
+
+    keys = list(checkpoint.keys())
+    new_sd = {}
+    for key in keys:
+        # remove resblocks 23
+        if ".resblocks.23." in key:
+            continue
+        new_key = convert_key(key)
+        if new_key is None:
+            continue
+        new_sd[new_key] = checkpoint[key]
+
+    # attnの変換
+    for key in keys:
+        if ".resblocks.23." in key:
+            continue
+        if ".resblocks" in key and ".attn.in_proj_" in key:
+            # 三つに分割
+            values = torch.chunk(checkpoint[key], 3)
+
+            key_suffix = ".weight" if "weight" in key else ".bias"
+            key_pfx = key.replace("cond_stage_model.model.transformer.resblocks.", "text_model.encoder.layers.")
+            key_pfx = key_pfx.replace("_weight", "")
+            key_pfx = key_pfx.replace("_bias", "")
+            key_pfx = key_pfx.replace(".attn.in_proj", ".self_attn.")
+            new_sd[key_pfx + "q_proj" + key_suffix] = values[0]
+            new_sd[key_pfx + "k_proj" + key_suffix] = values[1]
+            new_sd[key_pfx + "v_proj" + key_suffix] = values[2]
+
+    # rename or add position_ids
+    ANOTHER_POSITION_IDS_KEY = "text_model.encoder.text_model.embeddings.position_ids"
+    if ANOTHER_POSITION_IDS_KEY in new_sd:
+        # waifu diffusion v1.4
+        position_ids = new_sd[ANOTHER_POSITION_IDS_KEY]
+        del new_sd[ANOTHER_POSITION_IDS_KEY]
+    else:
+        position_ids = torch.Tensor([list(range(max_length))]).to(torch.int64)
+
+    new_sd["text_model.embeddings.position_ids"] = position_ids
+    return new_sd
+
+
+# endregion
+
+
+# region Diffusers->StableDiffusion の変換コード
+# convert_diffusers_to_original_stable_diffusion をコピーして修正している（ASL 2.0）
+
+
+def conv_transformer_to_linear(checkpoint):
+    keys = list(checkpoint.keys())
+    tf_keys = ["proj_in.weight", "proj_out.weight"]
+    for key in keys:
+        if ".".join(key.split(".")[-2:]) in tf_keys:
+            if checkpoint[key].ndim > 2:
+                checkpoint[key] = checkpoint[key][:, :, 0, 0]
+
+
+def convert_unet_state_dict_to_sd(v2, unet_state_dict):
+    unet_conversion_map = [
+        # (stable-diffusion, HF Diffusers)
+        ("time_embed.0.weight", "time_embedding.linear_1.weight"),
+        ("time_embed.0.bias", "time_embedding.linear_1.bias"),
+        ("time_embed.2.weight", "time_embedding.linear_2.weight"),
+        ("time_embed.2.bias", "time_embedding.linear_2.bias"),
+        ("input_blocks.0.0.weight", "conv_in.weight"),
+        ("input_blocks.0.0.bias", "conv_in.bias"),
+        ("out.0.weight", "conv_norm_out.weight"),
+        ("out.0.bias", "conv_norm_out.bias"),
+        ("out.2.weight", "conv_out.weight"),
+        ("out.2.bias", "conv_out.bias"),
+    ]
+
+    unet_conversion_map_resnet = [
+        # (stable-diffusion, HF Diffusers)
+        ("in_layers.0", "norm1"),
+        ("in_layers.2", "conv1"),
+        ("out_layers.0", "norm2"),
+        ("out_layers.3", "conv2"),
+        ("emb_layers.1", "time_emb_proj"),
+        ("skip_connection", "conv_shortcut"),
+    ]
+
+    unet_conversion_map_layer = []
+    for i in range(4):
+        # loop over downblocks/upblocks
+
+        for j in range(2):
+            # loop over resnets/attentions for downblocks
+            hf_down_res_prefix = f"down_blocks.{i}.resnets.{j}."
+            sd_down_res_prefix = f"input_blocks.{3*i + j + 1}.0."
+            unet_conversion_map_layer.append((sd_down_res_prefix, hf_down_res_prefix))
+
+            if i < 3:
+                # no attention layers in down_blocks.3
+                hf_down_atn_prefix = f"down_blocks.{i}.attentions.{j}."
+                sd_down_atn_prefix = f"input_blocks.{3*i + j + 1}.1."
+                unet_conversion_map_layer.append((sd_down_atn_prefix, hf_down_atn_prefix))
+
+        for j in range(3):
+            # loop over resnets/attentions for upblocks
+            hf_up_res_prefix = f"up_blocks.{i}.resnets.{j}."
+            sd_up_res_prefix = f"output_blocks.{3*i + j}.0."
+            unet_conversion_map_layer.append((sd_up_res_prefix, hf_up_res_prefix))
+
+            if i > 0:
+                # no attention layers in up_blocks.0
+                hf_up_atn_prefix = f"up_blocks.{i}.attentions.{j}."
+                sd_up_atn_prefix = f"output_blocks.{3*i + j}.1."
+                unet_conversion_map_layer.append((sd_up_atn_prefix, hf_up_atn_prefix))
+
+        if i < 3:
+            # no downsample in down_blocks.3
+            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0.conv."
+            sd_downsample_prefix = f"input_blocks.{3*(i+1)}.0.op."
+            unet_conversion_map_layer.append((sd_downsample_prefix, hf_downsample_prefix))
+
+            # no upsample in up_blocks.3
+            hf_upsample_prefix = f"up_blocks.{i}.upsamplers.0."
+            sd_upsample_prefix = f"output_blocks.{3*i + 2}.{1 if i == 0 else 2}."
+            unet_conversion_map_layer.append((sd_upsample_prefix, hf_upsample_prefix))
+
+    hf_mid_atn_prefix = "mid_block.attentions.0."
+    sd_mid_atn_prefix = "middle_block.1."
+    unet_conversion_map_layer.append((sd_mid_atn_prefix, hf_mid_atn_prefix))
+
+    for j in range(2):
+        hf_mid_res_prefix = f"mid_block.resnets.{j}."
+        sd_mid_res_prefix = f"middle_block.{2*j}."
+        unet_conversion_map_layer.append((sd_mid_res_prefix, hf_mid_res_prefix))
+
+    # buyer beware: this is a *brittle* function,
+    # and correct output requires that all of these pieces interact in
+    # the exact order in which I have arranged them.
+    mapping = {k: k for k in unet_state_dict.keys()}
+    for sd_name, hf_name in unet_conversion_map:
+        mapping[hf_name] = sd_name
+    for k, v in mapping.items():
+        if "resnets" in k:
+            for sd_part, hf_part in unet_conversion_map_resnet:
+                v = v.replace(hf_part, sd_part)
+            mapping[k] = v
+    for k, v in mapping.items():
+        for sd_part, hf_part in unet_conversion_map_layer:
+            v = v.replace(hf_part, sd_part)
+        mapping[k] = v
+    new_state_dict = {v: unet_state_dict[k] for k, v in mapping.items()}
+
+    if v2:
+        conv_transformer_to_linear(new_state_dict)
+
+    return new_state_dict
+
+
+# ================#
+# VAE Conversion #
+# ================#
+
+
+def reshape_weight_for_sd(w):
+    # convert HF linear weights to SD conv2d weights
+    return w.reshape(*w.shape, 1, 1)
+
+
+def convert_vae_state_dict(vae_state_dict):
+    vae_conversion_map = [
+        # (stable-diffusion, HF Diffusers)
+        ("nin_shortcut", "conv_shortcut"),
+        ("norm_out", "conv_norm_out"),
+        ("mid.attn_1.", "mid_block.attentions.0."),
+    ]
+
+    for i in range(4):
+        # down_blocks have two resnets
+        for j in range(2):
+            hf_down_prefix = f"encoder.down_blocks.{i}.resnets.{j}."
+            sd_down_prefix = f"encoder.down.{i}.block.{j}."
+            vae_conversion_map.append((sd_down_prefix, hf_down_prefix))
+
+        if i < 3:
+            hf_downsample_prefix = f"down_blocks.{i}.downsamplers.0."
+            sd_downsample_prefix = f"down.{i}.downsample."
+            vae_conversion_map.append((sd_downsample_prefix, hf_downsample_prefix))
+
+            hf_upsample_prefix = f"up_blocks.{i}.upsamplers.0."
+            sd_upsample_prefix = f"up.{3-i}.upsample."
+            vae_conversion_map.append((sd_upsample_prefix, hf_upsample_prefix))
+
+        # up_blocks have three resnets
+        # also, up blocks in hf are numbered in reverse from sd
+        for j in range(3):
+            hf_up_prefix = f"decoder.up_blocks.{i}.resnets.{j}."
+            sd_up_prefix = f"decoder.up.{3-i}.block.{j}."
+            vae_conversion_map.append((sd_up_prefix, hf_up_prefix))
+
+    # this part accounts for mid blocks in both the encoder and the decoder
+    for i in range(2):
+        hf_mid_res_prefix = f"mid_block.resnets.{i}."
+        sd_mid_res_prefix = f"mid.block_{i+1}."
+        vae_conversion_map.append((sd_mid_res_prefix, hf_mid_res_prefix))
+
+    vae_conversion_map_attn = [
+        # (stable-diffusion, HF Diffusers)
+        ("norm.", "group_norm."),
+        ("q.", "query."),
+        ("k.", "key."),
+        ("v.", "value."),
+        ("proj_out.", "proj_attn."),
+    ]
+
+    mapping = {k: k for k in vae_state_dict.keys()}
+    for k, v in mapping.items():
+        for sd_part, hf_part in vae_conversion_map:
+            v = v.replace(hf_part, sd_part)
+        mapping[k] = v
+    for k, v in mapping.items():
+        if "attentions" in k:
+            for sd_part, hf_part in vae_conversion_map_attn:
+                v = v.replace(hf_part, sd_part)
+            mapping[k] = v
+    new_state_dict = {v: vae_state_dict[k] for k, v in mapping.items()}
+    weights_to_convert = ["q", "k", "v", "proj_out"]
+    for k, v in new_state_dict.items():
+        for weight_name in weights_to_convert:
+            if f"mid.attn_1.{weight_name}.weight" in k:
+                # print(f"Reshaping {k} for SD format")
+                new_state_dict[k] = reshape_weight_for_sd(v)
+
+    return new_state_dict
+
+
+# endregion
+
+# region 自作のモデル読み書きなど
+
+
+def is_safetensors(path):
+    return os.path.splitext(path)[1].lower() == ".safetensors"
+
+
+def load_checkpoint_with_text_encoder_conversion(ckpt_path, device="cpu"):
+    # text encoderの格納形式が違うモデルに対応する ('text_model'がない)
+    TEXT_ENCODER_KEY_REPLACEMENTS = [
+        ("cond_stage_model.transformer.embeddings.", "cond_stage_model.transformer.text_model.embeddings."),
+        ("cond_stage_model.transformer.encoder.", "cond_stage_model.transformer.text_model.encoder."),
+        ("cond_stage_model.transformer.final_layer_norm.", "cond_stage_model.transformer.text_model.final_layer_norm."),
+    ]
+
+    if is_safetensors(ckpt_path):
+        checkpoint = None
+        state_dict = load_file(ckpt_path)  # , device) # may causes error
+    else:
+        checkpoint = torch.load(ckpt_path, map_location=device)
+        if "state_dict" in checkpoint:
+            state_dict = checkpoint["state_dict"]
+        else:
+            state_dict = checkpoint
+            checkpoint = None
+
+    key_reps = []
+    for rep_from, rep_to in TEXT_ENCODER_KEY_REPLACEMENTS:
+        for key in state_dict.keys():
+            if key.startswith(rep_from):
+                new_key = rep_to + key[len(rep_from) :]
+                key_reps.append((key, new_key))
+
+    for key, new_key in key_reps:
+        state_dict[new_key] = state_dict[key]
+        del state_dict[key]
+
+    return checkpoint, state_dict
+
+
+# TODO dtype指定の動作が怪しいので確認する text_encoderを指定形式で作れるか未確認
+def load_models_from_stable_diffusion_checkpoint(v2, ckpt_path, device="cpu", dtype=None):
+    _, state_dict = load_checkpoint_with_text_encoder_conversion(ckpt_path, device)
+
+    # Convert the UNet2DConditionModel model.
+    unet_config = create_unet_diffusers_config(v2)
+    converted_unet_checkpoint = convert_ldm_unet_checkpoint(v2, state_dict, unet_config)
+
+    unet = UNet2DConditionModel(**unet_config).to(device)
+    info = unet.load_state_dict(converted_unet_checkpoint)
+    print("loading u-net:", info)
+
+    # Convert the VAE model.
+    vae_config = create_vae_diffusers_config()
+    converted_vae_checkpoint = convert_ldm_vae_checkpoint(state_dict, vae_config)
+
+    vae = AutoencoderKL(**vae_config).to(device)
+    info = vae.load_state_dict(converted_vae_checkpoint)
+    print("loading vae:", info)
+
+    # convert text_model
+    if v2:
+        converted_text_encoder_checkpoint = convert_ldm_clip_checkpoint_v2(state_dict, 77)
+        cfg = CLIPTextConfig(
+            vocab_size=49408,
+            hidden_size=1024,
+            intermediate_size=4096,
+            num_hidden_layers=23,
+            num_attention_heads=16,
+            max_position_embeddings=77,
+            hidden_act="gelu",
+            layer_norm_eps=1e-05,
+            dropout=0.0,
+            attention_dropout=0.0,
+            initializer_range=0.02,
+            initializer_factor=1.0,
+            pad_token_id=1,
+            bos_token_id=0,
+            eos_token_id=2,
+            model_type="clip_text_model",
+            projection_dim=512,
+            torch_dtype="float32",
+            transformers_version="4.25.0.dev0",
+        )
+        text_model = CLIPTextModel._from_config(cfg)
+        info = text_model.load_state_dict(converted_text_encoder_checkpoint)
+    else:
+        converted_text_encoder_checkpoint = convert_ldm_clip_checkpoint_v1(state_dict)
+
+        logging.set_verbosity_error()  # don't show annoying warning
+        text_model = CLIPTextModel.from_pretrained("openai/clip-vit-large-patch14").to(device)
+        logging.set_verbosity_warning()
+
+        info = text_model.load_state_dict(converted_text_encoder_checkpoint)
+    print("loading text encoder:", info)
+
+    return text_model, vae, unet
+
+
+def convert_text_encoder_state_dict_to_sd_v2(checkpoint, make_dummy_weights=False):
+    def convert_key(key):
+        # position_idsの除去
+        if ".position_ids" in key:
+            return None
+
+        # common
+        key = key.replace("text_model.encoder.", "transformer.")
+        key = key.replace("text_model.", "")
+        if "layers" in key:
+            # resblocks conversion
+            key = key.replace(".layers.", ".resblocks.")
+            if ".layer_norm" in key:
+                key = key.replace(".layer_norm", ".ln_")
+            elif ".mlp." in key:
+                key = key.replace(".fc1.", ".c_fc.")
+                key = key.replace(".fc2.", ".c_proj.")
+            elif ".self_attn.out_proj" in key:
+                key = key.replace(".self_attn.out_proj.", ".attn.out_proj.")
+            elif ".self_attn." in key:
+                key = None  # 特殊なので後で処理する
+            else:
+                raise ValueError(f"unexpected key in DiffUsers model: {key}")
+        elif ".position_embedding" in key:
+            key = key.replace("embeddings.position_embedding.weight", "positional_embedding")
+        elif ".token_embedding" in key:
+            key = key.replace("embeddings.token_embedding.weight", "token_embedding.weight")
+        elif "final_layer_norm" in key:
+            key = key.replace("final_layer_norm", "ln_final")
+        return key
+
+    keys = list(checkpoint.keys())
+    new_sd = {}
+    for key in keys:
+        new_key = convert_key(key)
+        if new_key is None:
+            continue
+        new_sd[new_key] = checkpoint[key]
+
+    # attnの変換
+    for key in keys:
+        if "layers" in key and "q_proj" in key:
+            # 三つを結合
+            key_q = key
+            key_k = key.replace("q_proj", "k_proj")
+            key_v = key.replace("q_proj", "v_proj")
+
+            value_q = checkpoint[key_q]
+            value_k = checkpoint[key_k]
+            value_v = checkpoint[key_v]
+            value = torch.cat([value_q, value_k, value_v])
+
+            new_key = key.replace("text_model.encoder.layers.", "transformer.resblocks.")
+            new_key = new_key.replace(".self_attn.q_proj.", ".attn.in_proj_")
+            new_sd[new_key] = value
+
+    # 最後の層などを捏造するか
+    if make_dummy_weights:
+        print("make dummy weights for resblock.23, text_projection and logit scale.")
+        keys = list(new_sd.keys())
+        for key in keys:
+            if key.startswith("transformer.resblocks.22."):
+                new_sd[key.replace(".22.", ".23.")] = new_sd[key].clone()  # copyしないとsafetensorsの保存で落ちる
+
+        # Diffusersに含まれない重みを作っておく
+        new_sd["text_projection"] = torch.ones((1024, 1024), dtype=new_sd[keys[0]].dtype, device=new_sd[keys[0]].device)
+        new_sd["logit_scale"] = torch.tensor(1)
+
+    return new_sd
+
+
+def save_stable_diffusion_checkpoint(v2, output_file, text_encoder, unet, ckpt_path, epochs, steps, save_dtype=None, vae=None):
+    if ckpt_path is not None:
+        # epoch/stepを参照する。またVAEがメモリ上にないときなど、もう一度VAEを含めて読み込む
+        checkpoint, state_dict = load_checkpoint_with_text_encoder_conversion(ckpt_path)
+        if checkpoint is None:  # safetensors または state_dictのckpt
+            checkpoint = {}
+            strict = False
+        else:
+            strict = True
+        if "state_dict" in state_dict:
+            del state_dict["state_dict"]
+    else:
+        # 新しく作る
+        assert vae is not None, "VAE is required to save a checkpoint without a given checkpoint"
+        checkpoint = {}
+        state_dict = {}
+        strict = False
+
+    def update_sd(prefix, sd):
+        for k, v in sd.items():
+            key = prefix + k
+            assert not strict or key in state_dict, f"Illegal key in save SD: {key}"
+            if save_dtype is not None:
+                v = v.detach().clone().to("cpu").to(save_dtype)
+            state_dict[key] = v
+
+    # Convert the UNet model
+    unet_state_dict = convert_unet_state_dict_to_sd(v2, unet.state_dict())
+    update_sd("model.diffusion_model.", unet_state_dict)
+
+    # Convert the text encoder model
+    if v2:
+        make_dummy = ckpt_path is None  # 参照元のcheckpointがない場合は最後の層を前の層から複製して作るなどダミーの重みを入れる
+        text_enc_dict = convert_text_encoder_state_dict_to_sd_v2(text_encoder.state_dict(), make_dummy)
+        update_sd("cond_stage_model.model.", text_enc_dict)
+    else:
+        text_enc_dict = text_encoder.state_dict()
+        update_sd("cond_stage_model.transformer.", text_enc_dict)
+
+    # Convert the VAE
+    if vae is not None:
+        vae_dict = convert_vae_state_dict(vae.state_dict())
+        update_sd("first_stage_model.", vae_dict)
+
+    # Put together new checkpoint
+    key_count = len(state_dict.keys())
+    new_ckpt = {"state_dict": state_dict}
+
+    # epoch and global_step are sometimes not int
+    try:
+        if "epoch" in checkpoint:
+            epochs += checkpoint["epoch"]
+        if "global_step" in checkpoint:
+            steps += checkpoint["global_step"]
+    except:
+        pass
+
+    new_ckpt["epoch"] = epochs
+    new_ckpt["global_step"] = steps
+
+    if is_safetensors(output_file):
+        # TODO Tensor以外のdictの値を削除したほうがいいか
+        save_file(state_dict, output_file)
+    else:
+        torch.save(new_ckpt, output_file)
+
+    return key_count
+
+
+def save_diffusers_checkpoint(v2, output_dir, text_encoder, unet, pretrained_model_name_or_path, vae=None, use_safetensors=False):
+    if pretrained_model_name_or_path is None:
+        # load default settings for v1/v2
+        if v2:
+            pretrained_model_name_or_path = DIFFUSERS_REF_MODEL_ID_V2
+        else:
+            pretrained_model_name_or_path = DIFFUSERS_REF_MODEL_ID_V1
+
+    scheduler = DDIMScheduler.from_pretrained(pretrained_model_name_or_path, subfolder="scheduler")
+    tokenizer = CLIPTokenizer.from_pretrained(pretrained_model_name_or_path, subfolder="tokenizer")
+    if vae is None:
+        vae = AutoencoderKL.from_pretrained(pretrained_model_name_or_path, subfolder="vae")
+
+    pipeline = StableDiffusionPipeline(
+        unet=unet,
+        text_encoder=text_encoder,
+        vae=vae,
+        scheduler=scheduler,
+        tokenizer=tokenizer,
+        safety_checker=None,
+        feature_extractor=None,
+        requires_safety_checker=None,
+    )
+    pipeline.save_pretrained(output_dir, safe_serialization=use_safetensors)
+
+
+VAE_PREFIX = "first_stage_model."
+
+
+def load_vae(vae_id, dtype):
+    print(f"load VAE: {vae_id}")
+    if os.path.isdir(vae_id) or not os.path.isfile(vae_id):
+        # Diffusers local/remote
+        try:
+            vae = AutoencoderKL.from_pretrained(vae_id, subfolder=None, torch_dtype=dtype)
+        except EnvironmentError as e:
+            print(f"exception occurs in loading vae: {e}")
+            print("retry with subfolder='vae'")
+            vae = AutoencoderKL.from_pretrained(vae_id, subfolder="vae", torch_dtype=dtype)
+        return vae
+
+    # local
+    vae_config = create_vae_diffusers_config()
+
+    if vae_id.endswith(".bin"):
+        # SD 1.5 VAE on Huggingface
+        converted_vae_checkpoint = torch.load(vae_id, map_location="cpu")
+    else:
+        # StableDiffusion
+        vae_model = load_file(vae_id, "cpu") if is_safetensors(vae_id) else torch.load(vae_id, map_location="cpu")
+        vae_sd = vae_model["state_dict"] if "state_dict" in vae_model else vae_model
+
+        # vae only or full model
+        full_model = False
+        for vae_key in vae_sd:
+            if vae_key.startswith(VAE_PREFIX):
+                full_model = True
+                break
+        if not full_model:
+            sd = {}
+            for key, value in vae_sd.items():
+                sd[VAE_PREFIX + key] = value
+            vae_sd = sd
+            del sd
+
+        # Convert the VAE model.
+        converted_vae_checkpoint = convert_ldm_vae_checkpoint(vae_sd, vae_config)
+
+    vae = AutoencoderKL(**vae_config)
+    vae.load_state_dict(converted_vae_checkpoint)
+    return vae
+
+
+# endregion
+
+
+def make_bucket_resolutions(max_reso, min_size=256, max_size=1024, divisible=64):
+    max_width, max_height = max_reso
+    max_area = (max_width // divisible) * (max_height // divisible)
+
+    resos = set()
+
+    size = int(math.sqrt(max_area)) * divisible
+    resos.add((size, size))
+
+    size = min_size
+    while size <= max_size:
+        width = size
+        height = min(max_size, (max_area // (width // divisible)) * divisible)
+        resos.add((width, height))
+        resos.add((height, width))
+
+        # # make additional resos
+        # if width >= height and width - divisible >= min_size:
+        #   resos.add((width - divisible, height))
+        #   resos.add((height, width - divisible))
+        # if height >= width and height - divisible >= min_size:
+        #   resos.add((width, height - divisible))
+        #   resos.add((height - divisible, width))
+
+        size += divisible
+
+    resos = list(resos)
+    resos.sort()
+    return resos
+
+
+if __name__ == "__main__":
+    resos = make_bucket_resolutions((512, 768))
+    print(len(resos))
+    print(resos)
+    aspect_ratios = [w / h for w, h in resos]
+    print(aspect_ratios)
+
+    ars = set()
+    for ar in aspect_ratios:
+        if ar in ars:
+            print("error! duplicate ar:", ar)
+        ars.add(ar)
```

### Comparing `lycoris_lora-0.1.6.dev1/lycoris/kohya_utils.py` & `lycoris_lora-0.1.7.dev1/lycoris/kohya_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# part of https://github.com/kohya-ss/sd-scripts/blob/main/library/train_util.py
-
-import hashlib
-import safetensors
-from io import BytesIO
-
-
-def addnet_hash_legacy(b):
-    """Old model hash used by sd-webui-additional-networks for .safetensors format files"""
-    m = hashlib.sha256()
-
-    b.seek(0x100000)
-    m.update(b.read(0x10000))
-    return m.hexdigest()[0:8]
-
-
-def addnet_hash_safetensors(b):
-    """New model hash used by sd-webui-additional-networks for .safetensors format files"""
-    hash_sha256 = hashlib.sha256()
-    blksize = 1024 * 1024
-
-    b.seek(0)
-    header = b.read(8)
-    n = int.from_bytes(header, "little")
-
-    offset = n + 8
-    b.seek(offset)
-    for chunk in iter(lambda: b.read(blksize), b""):
-        hash_sha256.update(chunk)
-
-    return hash_sha256.hexdigest()
-
-
-def precalculate_safetensors_hashes(tensors, metadata):
-    """Precalculate the model hashes needed by sd-webui-additional-networks to
-    save time on indexing the model later."""
-
-    # Because writing user metadata to the file can change the result of
-    # sd_models.model_hash(), only retain the training metadata for purposes of
-    # calculating the hash, as they are meant to be immutable
-    metadata = {k: v for k, v in metadata.items() if k.startswith("ss_")}
-
-    bytes = safetensors.torch.save(tensors, metadata)
-    b = BytesIO(bytes)
-
-    model_hash = addnet_hash_safetensors(b)
-    legacy_hash = addnet_hash_legacy(b)
+# part of https://github.com/kohya-ss/sd-scripts/blob/main/library/train_util.py
+
+import hashlib
+import safetensors
+from io import BytesIO
+
+
+def addnet_hash_legacy(b):
+    """Old model hash used by sd-webui-additional-networks for .safetensors format files"""
+    m = hashlib.sha256()
+
+    b.seek(0x100000)
+    m.update(b.read(0x10000))
+    return m.hexdigest()[0:8]
+
+
+def addnet_hash_safetensors(b):
+    """New model hash used by sd-webui-additional-networks for .safetensors format files"""
+    hash_sha256 = hashlib.sha256()
+    blksize = 1024 * 1024
+
+    b.seek(0)
+    header = b.read(8)
+    n = int.from_bytes(header, "little")
+
+    offset = n + 8
+    b.seek(offset)
+    for chunk in iter(lambda: b.read(blksize), b""):
+        hash_sha256.update(chunk)
+
+    return hash_sha256.hexdigest()
+
+
+def precalculate_safetensors_hashes(tensors, metadata):
+    """Precalculate the model hashes needed by sd-webui-additional-networks to
+    save time on indexing the model later."""
+
+    # Because writing user metadata to the file can change the result of
+    # sd_models.model_hash(), only retain the training metadata for purposes of
+    # calculating the hash, as they are meant to be immutable
+    metadata = {k: v for k, v in metadata.items() if k.startswith("ss_")}
+
+    bytes = safetensors.torch.save(tensors, metadata)
+    b = BytesIO(bytes)
+
+    model_hash = addnet_hash_safetensors(b)
+    legacy_hash = addnet_hash_legacy(b)
     return model_hash, legacy_hash
```

### Comparing `lycoris_lora-0.1.6.dev1/lycoris/locon.py` & `lycoris_lora-0.1.7.dev1/lycoris/locon.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,103 @@
-import math
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-
-class LoConModule(nn.Module):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-    """
-
-    def __init__(
-        self, 
-        lora_name, org_module: nn.Module, 
-        multiplier=1.0, 
-        lora_dim=4, alpha=1, 
-        dropout=0.,
-        use_cp=False,
-        **kwargs,
-    ):
-        """ if alpha == 0 or None, alpha is rank (no scaling). """
-        super().__init__()
-        self.lora_name = lora_name
-        self.lora_dim = lora_dim
-        self.cp = False
-
-        if org_module.__class__.__name__ == 'Conv2d':
-            # For general LoCon
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            stride = org_module.stride
-            padding = org_module.padding
-            out_dim = org_module.out_channels
-            if use_cp and k_size != (1, 1):
-                self.lora_down = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
-                self.lora_mid = nn.Conv2d(lora_dim, lora_dim, k_size, stride, padding, bias=False)
-                self.cp = True
-            else:
-                self.lora_down = nn.Conv2d(in_dim, lora_dim, k_size, stride, padding, bias=False)
-            self.lora_up = nn.Conv2d(lora_dim, out_dim, (1, 1), bias=False)
-        else:
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            self.lora_down = nn.Linear(in_dim, lora_dim, bias=False)
-            self.lora_up = nn.Linear(lora_dim, out_dim, bias=False)
-        self.shape = org_module.weight.shape
-        
-        if dropout:
-            self.dropout = nn.Dropout(dropout)
-        else:
-            self.dropout = nn.Identity()
-        
-        if type(alpha) == torch.Tensor:
-            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-        alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        self.scale = alpha / self.lora_dim
-        self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
-
-        # same as microsoft's
-        torch.nn.init.kaiming_uniform_(self.lora_down.weight, a=math.sqrt(5))
-        torch.nn.init.zeros_(self.lora_up.weight)
-        if self.cp:
-            torch.nn.init.kaiming_uniform_(self.lora_mid.weight, a=math.sqrt(5))
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-
-    def apply_to(self):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-
-    def make_weight(self):
-        wa = self.lora_up.weight
-        wb = self.lora_down.weight
-        return (wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)).view(self.shape)
-
-    def forward(self, x):
-        if self.cp:
-            return self.org_forward(x)  + self.dropout(
-                self.lora_up(self.lora_mid(self.lora_down(x)))* self.multiplier * self.scale
-            )
-        else:
-            return self.org_forward(x)  + self.dropout(
-                self.lora_up(self.lora_down(x))* self.multiplier * self.scale
-            )
+import math
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+
+class LoConModule(nn.Module):
+    """
+    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
+    """
+
+    def __init__(
+        self, 
+        lora_name, org_module: nn.Module, 
+        multiplier=1.0, 
+        lora_dim=4, alpha=1, 
+        dropout=0.,
+        use_cp=False,
+        **kwargs,
+    ):
+        """ if alpha == 0 or None, alpha is rank (no scaling). """
+        super().__init__()
+        self.lora_name = lora_name
+        self.lora_dim = lora_dim
+        self.cp = False
+
+        if org_module.__class__.__name__ == 'Conv2d':
+            # For general LoCon
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            stride = org_module.stride
+            padding = org_module.padding
+            out_dim = org_module.out_channels
+            if use_cp and k_size != (1, 1):
+                self.lora_down = nn.Conv2d(in_dim, lora_dim, (1, 1), bias=False)
+                self.lora_mid = nn.Conv2d(lora_dim, lora_dim, k_size, stride, padding, bias=False)
+                self.cp = True
+            else:
+                self.lora_down = nn.Conv2d(in_dim, lora_dim, k_size, stride, padding, bias=False)
+            self.lora_up = nn.Conv2d(lora_dim, out_dim, (1, 1), bias=False)
+        else:
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            self.lora_down = nn.Linear(in_dim, lora_dim, bias=False)
+            self.lora_up = nn.Linear(lora_dim, out_dim, bias=False)
+        self.shape = org_module.weight.shape
+        
+        if dropout:
+            self.dropout = nn.Dropout(dropout)
+        else:
+            self.dropout = nn.Identity()
+        
+        if type(alpha) == torch.Tensor:
+            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
+        alpha = lora_dim if alpha is None or alpha == 0 else alpha
+        self.scale = alpha / self.lora_dim
+        self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
+
+        # same as microsoft's
+        torch.nn.init.kaiming_uniform_(self.lora_down.weight, a=math.sqrt(5))
+        torch.nn.init.zeros_(self.lora_up.weight)
+        if self.cp:
+            torch.nn.init.kaiming_uniform_(self.lora_mid.weight, a=math.sqrt(5))
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]
+
+    def apply_to(self):
+        self.org_forward = self.org_module[0].forward
+        self.org_module[0].forward = self.forward
+
+    def make_weight(self, device=None):
+        wa = self.lora_up.weight.to(device)
+        wb = self.lora_down.weight.to(device)
+        return (wa.view(wa.size(0), -1) @ wb.view(wb.size(0), -1)).view(self.shape)
+
+    @torch.no_grad()
+    def apply_max_norm(self, max_norm, device=None):
+        norm = torch.clamp(self.make_weight(device).norm()*self.scale, max_norm/2)
+        desired = torch.clamp(norm, max=max_norm)
+        ratio = desired.cpu()/norm.cpu()
+        
+        scaled = ratio != 1.0
+        if scaled:
+            modules = self.cp + 2
+            self.lora_up.weight *= ratio**(1/modules)
+            self.lora_down.weight *= ratio**(1/modules)
+            if self.cp:
+                self.lora_mid.weight *= ratio**(1/modules)
+        
+        return scaled, norm*ratio
+
+    def forward(self, x):
+        scale = self.scale * self.multiplier
+        if self.cp:
+            return self.org_forward(x)  + self.dropout(
+                self.lora_up(self.lora_mid(self.lora_down(x))) * scale
+            )
+        else:
+            return self.org_forward(x)  + self.dropout(
+                self.lora_up(self.lora_down(x)) * scale
+            )
```

### Comparing `lycoris_lora-0.1.6.dev1/lycoris/loha.py` & `lycoris_lora-0.1.7.dev1/lycoris/loha.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,199 +1,220 @@
-import math
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-
-class HadaWeight(torch.autograd.Function):
-    @staticmethod
-    def forward(ctx, orig_weight, w1a, w1b, w2a, w2b, scale=torch.tensor(1)):
-        ctx.save_for_backward(w1a, w1b, w2a, w2b, scale)
-        diff_weight = ((w1a@w1b)*(w2a@w2b)) * scale
-        return orig_weight.reshape(diff_weight.shape) + diff_weight
-
-    @staticmethod
-    def backward(ctx, grad_out):
-        (w1a, w1b, w2a, w2b, scale) = ctx.saved_tensors
-        grad_out = grad_out * scale
-        temp = grad_out*(w2a@w2b)
-        grad_w1a = temp @ w1b.T
-        grad_w1b = w1a.T @ temp
-
-        temp = grad_out * (w1a@w1b)
-        grad_w2a = temp @ w2b.T
-        grad_w2b = w2a.T @ temp
-        
-        del temp
-        return grad_out, grad_w1a, grad_w1b, grad_w2a, grad_w2b, None
-
-
-class HadaWeightCP(torch.autograd.Function):
-    @staticmethod
-    def forward(ctx, orig_weight, t1, w1a, w1b, t2, w2a, w2b, scale=torch.tensor(1)):
-        ctx.save_for_backward(t1, w1a, w1b, t2, w2a, w2b, scale)
-        
-        rebuild1 = torch.einsum('i j k l, j r, i p -> p r k l', t1, w1b, w1a)
-        rebuild2 = torch.einsum('i j k l, j r, i p -> p r k l', t2, w2b, w2a)
-        
-        return orig_weight + rebuild1*rebuild2*scale
-
-    @staticmethod
-    def backward(ctx, grad_out):
-        (t1, w1a, w1b, t2, w2a, w2b, scale) = ctx.saved_tensors
-        
-        grad_out = grad_out*scale
-        
-        temp = torch.einsum('i j k l, j r -> i r k l', t2, w2b)
-        rebuild = torch.einsum('i j k l, i r -> r j k l', temp, w2a)
-        
-        grad_w = rebuild*grad_out
-        del rebuild
-        
-        grad_w1a = torch.einsum('r j k l, i j k l -> r i', temp, grad_w)
-        grad_temp = torch.einsum('i j k l, i r -> r j k l', grad_w, w1a.T)
-        del grad_w, temp
-        
-        grad_w1b = torch.einsum('i r k l, i j k l -> r j', t1, grad_temp)
-        grad_t1 = torch.einsum('i j k l, j r -> i r k l', grad_temp, w1b.T)
-        del grad_temp
-        
-        temp = torch.einsum('i j k l, j r -> i r k l', t1, w1b)
-        rebuild = torch.einsum('i j k l, i r -> r j k l', temp, w1a)
-        
-        grad_w = rebuild*grad_out
-        del rebuild
-        
-        grad_w2a = torch.einsum('r j k l, i j k l -> r i', temp, grad_w)
-        grad_temp = torch.einsum('i j k l, i r -> r j k l', grad_w, w2a.T)
-        del grad_w, temp
-        
-        grad_w2b = torch.einsum('i r k l, i j k l -> r j', t2, grad_temp)
-        grad_t2 = torch.einsum('i j k l, j r -> i r k l', grad_temp, w2b.T)
-        del grad_temp
-        return grad_out, grad_t1, grad_w1a, grad_w1b, grad_t2, grad_w2a, grad_w2b, None
-
-
-def make_weight(orig_weight, w1a, w1b, w2a, w2b, scale):
-    return HadaWeight.apply(orig_weight, w1a, w1b, w2a, w2b, scale)
-
-
-def make_weight_cp(orig_weight, t1, w1a, w1b, t2, w2a, w2b, scale):
-    return HadaWeightCP.apply(orig_weight, t1, w1a, w1b, t2, w2a, w2b, scale)
-
-
-class LohaModule(nn.Module):
-    """
-    Hadamard product Implementaion for Low Rank Adaptation
-    """
-
-    def __init__(
-        self, 
-        lora_name, 
-        org_module: nn.Module, 
-        multiplier=1.0, lora_dim=4, alpha=1, dropout=0.,
-        use_cp=False,
-        **kwargs,
-    ):
-        """ if alpha == 0 or None, alpha is rank (no scaling). """
-        super().__init__()
-        self.lora_name = lora_name
-        self.lora_dim = lora_dim
-        self.cp=False
-        
-        self.shape = org_module.weight.shape
-        if org_module.__class__.__name__ == 'Conv2d':
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            out_dim = org_module.out_channels
-            self.cp = use_cp and k_size!=(1, 1)
-            if self.cp:
-                shape = (out_dim, in_dim, *k_size)
-            else:
-                shape = (out_dim, in_dim*k_size[0]*k_size[1])
-            self.op = F.conv2d
-            self.extra_args = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups
-            }
-        else:
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            shape = (out_dim, in_dim)
-            self.op = F.linear
-            self.extra_args = {}
-        
-        if self.cp:
-            self.hada_t1 = nn.Parameter(torch.empty(lora_dim, lora_dim, shape[2], shape[3]))
-            self.hada_w1_a = nn.Parameter(torch.empty(lora_dim, shape[0])) # out_dim, 1-mode
-            self.hada_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1])) # in_dim , 2-mode
-            
-            self.hada_t2 = nn.Parameter(torch.empty(lora_dim, lora_dim, shape[2], shape[3]))
-            self.hada_w2_a = nn.Parameter(torch.empty(lora_dim, shape[0])) # out_dim, 1-mode
-            self.hada_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1])) # in_dim , 2-mode
-        else:
-            self.hada_w1_a = nn.Parameter(torch.empty(shape[0], lora_dim))
-            self.hada_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1]))
-            
-            self.hada_w2_a = nn.Parameter(torch.empty(shape[0], lora_dim))
-            self.hada_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1]))
-        
-        if dropout:
-            self.dropout = nn.Dropout(dropout)
-        else:
-            self.dropout = nn.Identity()
-        
-        if type(alpha) == torch.Tensor:
-            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-        alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        self.scale = alpha / self.lora_dim
-        self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
-
-        # Need more experiences on init method
-        if self.cp:
-            torch.nn.init.normal_(self.hada_t1, std=0.1)
-            torch.nn.init.normal_(self.hada_t2, std=0.1)
-        torch.nn.init.normal_(self.hada_w1_b, std=1)
-        torch.nn.init.normal_(self.hada_w2_b, std=0.01)
-        torch.nn.init.normal_(self.hada_w1_a, std=1)
-        torch.nn.init.constant_(self.hada_w2_a, 0)
-
-        self.multiplier = multiplier
-        self.org_module = [org_module] # remove in applying
-        self.grad_ckpt = False
-
-    def apply_to(self):
-        self.org_module[0].forward = self.forward
-
-    def get_weight(self):
-        d_weight = self.hada_w1_a @ self.hada_w1_b
-        d_weight *= self.hada_w2_a @ self.hada_w2_b
-        return (d_weight).reshape(self.shape)
-
-    @torch.enable_grad()
-    def forward(self, x):
-        # print(torch.mean(torch.abs(self.orig_w1a.to(x.device) - self.hada_w1_a)), end='\r')
-        if self.cp:
-            weight = make_weight_cp(
-                self.org_module[0].weight.data, 
-                self.hada_t1, self.hada_w1_a, self.hada_w1_b,
-                self.hada_t1, self.hada_w2_a, self.hada_w2_b,
-                scale = torch.tensor(self.scale*self.multiplier),
-            )
-        else:
-            weight = make_weight(
-                self.org_module[0].weight.data, 
-                self.hada_w1_a, self.hada_w1_b,
-                self.hada_w2_a, self.hada_w2_b,
-                scale = torch.tensor(self.scale*self.multiplier),
-            )
-        
-        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
-        return self.op(
-            x, 
-            weight.view(self.shape),
-            bias,
-            **self.extra_args
+import math
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+
+class HadaWeight(torch.autograd.Function):
+    @staticmethod
+    def forward(ctx, orig_weight, w1a, w1b, w2a, w2b, scale=torch.tensor(1)):
+        ctx.save_for_backward(w1a, w1b, w2a, w2b, scale)
+        diff_weight = ((w1a@w1b)*(w2a@w2b)) * scale
+        
+        if isinstance(orig_weight, torch.Tensor):
+            orig_weight = orig_weight.reshape(diff_weight.shape)
+        return orig_weight + diff_weight
+
+    @staticmethod
+    def backward(ctx, grad_out):
+        (w1a, w1b, w2a, w2b, scale) = ctx.saved_tensors
+        grad_out = grad_out * scale
+        temp = grad_out*(w2a@w2b)
+        grad_w1a = temp @ w1b.T
+        grad_w1b = w1a.T @ temp
+
+        temp = grad_out * (w1a@w1b)
+        grad_w2a = temp @ w2b.T
+        grad_w2b = w2a.T @ temp
+        
+        del temp
+        return grad_out, grad_w1a, grad_w1b, grad_w2a, grad_w2b, None
+
+
+class HadaWeightCP(torch.autograd.Function):
+    @staticmethod
+    def forward(ctx, orig_weight, t1, w1a, w1b, t2, w2a, w2b, scale=torch.tensor(1)):
+        ctx.save_for_backward(t1, w1a, w1b, t2, w2a, w2b, scale)
+        
+        rebuild1 = torch.einsum('i j k l, j r, i p -> p r k l', t1, w1b, w1a)
+        rebuild2 = torch.einsum('i j k l, j r, i p -> p r k l', t2, w2b, w2a)
+        
+        return orig_weight + rebuild1*rebuild2*scale
+
+    @staticmethod
+    def backward(ctx, grad_out):
+        (t1, w1a, w1b, t2, w2a, w2b, scale) = ctx.saved_tensors
+        
+        grad_out = grad_out*scale
+        
+        temp = torch.einsum('i j k l, j r -> i r k l', t2, w2b)
+        rebuild = torch.einsum('i j k l, i r -> r j k l', temp, w2a)
+        
+        grad_w = rebuild*grad_out
+        del rebuild
+        
+        grad_w1a = torch.einsum('r j k l, i j k l -> r i', temp, grad_w)
+        grad_temp = torch.einsum('i j k l, i r -> r j k l', grad_w, w1a.T)
+        del grad_w, temp
+        
+        grad_w1b = torch.einsum('i r k l, i j k l -> r j', t1, grad_temp)
+        grad_t1 = torch.einsum('i j k l, j r -> i r k l', grad_temp, w1b.T)
+        del grad_temp
+        
+        temp = torch.einsum('i j k l, j r -> i r k l', t1, w1b)
+        rebuild = torch.einsum('i j k l, i r -> r j k l', temp, w1a)
+        
+        grad_w = rebuild*grad_out
+        del rebuild
+        
+        grad_w2a = torch.einsum('r j k l, i j k l -> r i', temp, grad_w)
+        grad_temp = torch.einsum('i j k l, i r -> r j k l', grad_w, w2a.T)
+        del grad_w, temp
+        
+        grad_w2b = torch.einsum('i r k l, i j k l -> r j', t2, grad_temp)
+        grad_t2 = torch.einsum('i j k l, j r -> i r k l', grad_temp, w2b.T)
+        del grad_temp
+        return grad_out, grad_t1, grad_w1a, grad_w1b, grad_t2, grad_w2a, grad_w2b, None
+
+
+def make_weight(orig_weight, w1a, w1b, w2a, w2b, scale):
+    return HadaWeight.apply(orig_weight, w1a, w1b, w2a, w2b, scale)
+
+
+def make_weight_cp(orig_weight, t1, w1a, w1b, t2, w2a, w2b, scale):
+    return HadaWeightCP.apply(orig_weight, t1, w1a, w1b, t2, w2a, w2b, scale)
+
+
+class LohaModule(nn.Module):
+    """
+    Hadamard product Implementaion for Low Rank Adaptation
+    """
+
+    def __init__(
+        self, 
+        lora_name, 
+        org_module: nn.Module, 
+        multiplier=1.0, lora_dim=4, alpha=1, dropout=0.,
+        use_cp=False,
+        **kwargs,
+    ):
+        """ if alpha == 0 or None, alpha is rank (no scaling). """
+        super().__init__()
+        self.lora_name = lora_name
+        self.lora_dim = lora_dim
+        self.cp=False
+        
+        self.shape = org_module.weight.shape
+        if org_module.__class__.__name__ == 'Conv2d':
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            out_dim = org_module.out_channels
+            self.cp = use_cp and k_size!=(1, 1)
+            if self.cp:
+                shape = (out_dim, in_dim, *k_size)
+            else:
+                shape = (out_dim, in_dim*k_size[0]*k_size[1])
+            self.op = F.conv2d
+            self.extra_args = {
+                "stride": org_module.stride,
+                "padding": org_module.padding,
+                "dilation": org_module.dilation,
+                "groups": org_module.groups
+            }
+        else:
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            shape = (out_dim, in_dim)
+            self.op = F.linear
+            self.extra_args = {}
+        
+        if self.cp:
+            self.hada_t1 = nn.Parameter(torch.empty(lora_dim, lora_dim, shape[2], shape[3]))
+            self.hada_w1_a = nn.Parameter(torch.empty(lora_dim, shape[0])) # out_dim, 1-mode
+            self.hada_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1])) # in_dim , 2-mode
+            
+            self.hada_t2 = nn.Parameter(torch.empty(lora_dim, lora_dim, shape[2], shape[3]))
+            self.hada_w2_a = nn.Parameter(torch.empty(lora_dim, shape[0])) # out_dim, 1-mode
+            self.hada_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1])) # in_dim , 2-mode
+        else:
+            self.hada_w1_a = nn.Parameter(torch.empty(shape[0], lora_dim))
+            self.hada_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1]))
+            
+            self.hada_w2_a = nn.Parameter(torch.empty(shape[0], lora_dim))
+            self.hada_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1]))
+        
+        if dropout:
+            self.dropout = nn.Dropout(dropout)
+        else:
+            self.dropout = nn.Identity()
+        
+        if type(alpha) == torch.Tensor:
+            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
+        alpha = lora_dim if alpha is None or alpha == 0 else alpha
+        self.scale = alpha / self.lora_dim
+        self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
+
+        # Need more experiences on init method
+        if self.cp:
+            torch.nn.init.normal_(self.hada_t1, std=0.1)
+            torch.nn.init.normal_(self.hada_t2, std=0.1)
+        torch.nn.init.normal_(self.hada_w1_b, std=1)
+        torch.nn.init.normal_(self.hada_w2_b, std=0.01)
+        torch.nn.init.normal_(self.hada_w1_a, std=1)
+        torch.nn.init.constant_(self.hada_w2_a, 0)
+
+        self.multiplier = multiplier
+        self.org_module = [org_module] # remove in applying
+        self.grad_ckpt = False
+
+    def apply_to(self):
+        self.org_module[0].forward = self.forward
+
+    def get_weight(self):
+        if self.cp:
+            weight = make_weight_cp(
+                0, 
+                self.hada_t1, self.hada_w1_a, self.hada_w1_b,
+                self.hada_t1, self.hada_w2_a, self.hada_w2_b,
+                scale = torch.tensor(self.scale),
+            )
+        else:
+            weight = make_weight(
+                0, 
+                self.hada_w1_a, self.hada_w1_b,
+                self.hada_w2_a, self.hada_w2_b,
+                scale = torch.tensor(self.scale),
+            )
+        return weight
+
+    @torch.no_grad()
+    def apply_max_norm(self, max_norm, device=None):
+        norm = torch.clamp(self.get_weight().norm(), max_norm/2)
+        desired = torch.clamp(norm, max=max_norm)
+        ratio = desired.cpu()/norm.cpu()
+        
+        scaled = ratio != 1.0
+        if scaled:
+            modules = (self.cp + 2)*2
+            self.hada_w1_a *= ratio**(1/modules)
+            self.hada_w1_b *= ratio**(1/modules)
+            self.hada_w2_a *= ratio**(1/modules)
+            self.hada_w2_b *= ratio**(1/modules)
+            
+            if self.cp:
+                self.hada_t1 *= ratio**(1/modules)
+                self.hada_t2 *= ratio**(1/modules)
+        
+        return scaled, norm*ratio
+
+    @torch.enable_grad()
+    def forward(self, x):
+        # print(torch.mean(torch.abs(self.orig_w1a.to(x.device) - self.hada_w1_a)), end='\r')
+        weight = self.org_module[0].weight.data + self.get_weight() * self.multiplier
+        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
+        return self.op(
+            x, 
+            weight.view(self.shape),
+            bias,
+            **self.extra_args
         )
```

### Comparing `lycoris_lora-0.1.6.dev1/lycoris/lokr.py` & `lycoris_lora-0.1.7.dev1/lycoris/lokr.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,220 +1,249 @@
-import math
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-# 4, build custom backward function
-#  - 
-
-
-def factorization(dimension: int, factor:int=-1) -> tuple[int, int]:
-    '''
-    return a tuple of two value of input dimension decomposed by the number closest to factor
-    second value is higher or equal than first value.
-    
-    In LoRA with Kroneckor Product, first value is a value for weight scale.
-    secon value is a value for weight.
-    
-    Becuase of non-commutative property, A⊗B ≠ B⊗A. Meaning of two matrices is slightly different.
-    
-    examples)
-    factor
-        -1               2                4               8               16               ...
-    127 -> 127, 1   127 -> 127, 1    127 -> 127, 1   127 -> 127, 1   127 -> 127, 1
-    128 -> 16, 8    128 -> 64, 2     128 -> 32, 4    128 -> 16, 8    128 -> 16, 8
-    250 -> 125, 2   250 -> 125, 2    250 -> 125, 2   250 -> 125, 2   250 -> 125, 2
-    360 -> 45, 8    360 -> 180, 2    360 -> 90, 4    360 -> 45, 8    360 -> 45, 8
-    512 -> 32, 16   512 -> 256, 2    512 -> 128, 4   512 -> 64, 8    512 -> 32, 16
-    1024 -> 32, 32  1024 -> 512, 2   1024 -> 256, 4  1024 -> 128, 8  1024 -> 64, 16
-    '''
-    
-    if factor > 0 and (dimension % factor) == 0:
-        m = factor
-        n = dimension // factor
-        return m, n
-    if factor == -1:
-        factor = dimension
-    m, n = 1, dimension
-    length = m + n
-    while m<n:
-        new_m = m + 1
-        while dimension%new_m != 0:
-            new_m += 1
-        new_n = dimension // new_m
-        if new_m + new_n > length or new_m>factor:
-            break
-        else:
-            m, n = new_m, new_n
-    if m > n:
-        n, m = m, n
-    return m, n
-
-
-def make_weight_cp(t, wa, wb):
-    rebuild2 = torch.einsum('i j k l, i p, j r -> p r k l', t, wa, wb) # [c, d, k1, k2]
-    return rebuild2
-
-
-def make_kron(orig_weight, w1, w2, scale):
-    if len(w2.shape) == 4:
-        w1 = w1.unsqueeze(2).unsqueeze(2)
-    w2 = w2.contiguous()
-    return orig_weight + torch.kron(w1, w2).reshape(orig_weight.shape)*scale
-
-
-class LokrModule(nn.Module):
-    """
-    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
-        and from KohakuBlueleaf/LyCORIS/lycoris:loha:LoHaModule
-        and from KohakuBlueleaf/LyCORIS/lycoris:locon:LoconModule
-    """
-
-    def __init__(
-        self, 
-        lora_name, org_module: nn.Module, 
-        multiplier=1.0, 
-        lora_dim=4, alpha=1, 
-        dropout=0.,
-        use_cp=False,
-        decompose_both = False,
-        factor:int=-1, # factorization factor
-        **kwargs,
-    ):
-        """ if alpha == 0 or None, alpha is rank (no scaling). """
-        super().__init__()
-        factor = int(factor)
-        self.lora_name = lora_name
-        self.lora_dim = lora_dim
-        self.cp = False
-        self.use_w1 = False
-        self.use_w2 = False
-
-        self.shape = org_module.weight.shape
-        if org_module.__class__.__name__ == 'Conv2d':
-            in_dim = org_module.in_channels
-            k_size = org_module.kernel_size
-            out_dim = org_module.out_channels
-            
-            in_m, in_n = factorization(in_dim, factor)
-            out_l, out_k = factorization(out_dim, factor)
-            shape = ((out_l, out_k), (in_m, in_n), *k_size) # ((a, b), (c, d), *k_size)
-            
-            self.cp = use_cp and k_size!=(1, 1)
-            if decompose_both and lora_dim < max(shape[0][0], shape[1][0])/2:
-                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
-                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
-            else:
-                self.use_w1 = True
-                self.lokr_w1 = nn.Parameter(torch.empty(shape[0][0], shape[1][0]))  # a*c, 1-mode
-            
-            if lora_dim >= max(shape[0][1], shape[1][1])/2:
-                self.use_w2 = True
-                self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1], *k_size))
-            elif self.cp:
-                self.lokr_t2 = nn.Parameter(torch.empty(lora_dim, lora_dim, shape[2], shape[3]))
-                self.lokr_w2_a = nn.Parameter(torch.empty(lora_dim, shape[0][1])) # b, 1-mode
-                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1])) # d, 2-mode
-            else: # Conv2d not cp
-                # bigger part. weight and LoRA. [b, dim] x [dim, d*k1*k2]
-                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
-                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1]*shape[2]*shape[3]))
-                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d*k1*k2)) = (a, b)⊗(c, d*k1*k2) = (ac, bd*k1*k2)
-            
-            self.op = F.conv2d
-            self.extra_args = {
-                "stride": org_module.stride,
-                "padding": org_module.padding,
-                "dilation": org_module.dilation,
-                "groups": org_module.groups
-            }
-
-        else: # Linear
-            in_dim = org_module.in_features
-            out_dim = org_module.out_features
-            
-            in_m, in_n = factorization(in_dim, factor)
-            out_l, out_k = factorization(out_dim, factor)
-            shape = ((out_l, out_k), (in_m, in_n)) # ((a, b), (c, d)), out_dim = a*c, in_dim = b*d
-            
-            # smaller part. weight scale
-            if decompose_both and lora_dim < max(shape[0][0], shape[1][0])/2:
-                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
-                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
-            else:
-                self.use_w1 = True
-                self.lokr_w1 = nn.Parameter(torch.empty(shape[0][0], shape[1][0]))  # a*c, 1-mode
-
-            if lora_dim < max(shape[0][1], shape[1][1])/2:
-                # bigger part. weight and LoRA. [b, dim] x [dim, d]
-                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
-                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1]))
-                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d)) = (a, b)⊗(c, d) = (ac, bd)
-            else:
-                self.use_w2 = True
-                self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1]))
-
-            self.op = F.linear
-            self.extra_args = {}
-        
-        if dropout:
-            self.dropout = nn.Dropout(dropout)
-        else:
-            self.dropout = nn.Identity()
-        
-        if isinstance(alpha, torch.Tensor):
-            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
-        alpha = lora_dim if alpha is None or alpha == 0 else alpha
-        if self.use_w2 and self.use_w1:
-            #use scale = 1
-            alpha = lora_dim
-        self.scale = alpha / self.lora_dim
-        self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
-
-        if self.use_w2:
-            torch.nn.init.constant_(self.lokr_w2, 0)
-        else:
-            if self.cp:
-                torch.nn.init.normal_(self.lokr_t2, std=0.1)
-            torch.nn.init.normal_(self.lokr_w2_a, std=1)
-            torch.nn.init.constant_(self.lokr_w2_b, 0)
-        
-        if self.use_w1:
-            torch.nn.init.normal_(self.lokr_w1, std=1)
-        else:
-            torch.nn.init.normal_(self.lokr_w1_a, std=1)
-            torch.nn.init.normal_(self.lokr_w1_b, std=0.1)
-
-        self.multiplier = multiplier
-        self.org_module = [org_module]
-        weight = make_kron(
-            self.org_module[0].weight.data, 
-            self.lokr_w1 if self.use_w1 else self.lokr_w1_a@self.lokr_w1_b,
-            (self.lokr_w2 if self.use_w2 
-             else make_weight_cp(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b) if self.cp 
-             else self.lokr_w2_a@self.lokr_w2_b),
-            torch.tensor(self.multiplier * self.scale)
-        )
-        assert torch.sum(torch.isnan(weight)) == 0, "weight is nan"
-
-    # Same as locon.py
-    def apply_to(self):
-        self.org_forward = self.org_module[0].forward
-        self.org_module[0].forward = self.forward
-
-    def forward(self, x):
-        weight = make_kron(
-            self.org_module[0].weight.data, 
-            self.lokr_w1 if self.use_w1 else self.lokr_w1_a@self.lokr_w1_b,
-            (self.lokr_w2 if self.use_w2 
-             else make_weight_cp(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b) if self.cp 
-             else self.lokr_w2_a@self.lokr_w2_b),
-            torch.tensor(self.multiplier * self.scale)
-        )
-        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
-        return self.op(
-            x, 
-            weight.view(self.shape),
-            bias,
-            **self.extra_args
-        )
+import math
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+# 4, build custom backward function
+#  - 
+
+
+def factorization(dimension: int, factor:int=-1) -> tuple[int, int]:
+    '''
+    return a tuple of two value of input dimension decomposed by the number closest to factor
+    second value is higher or equal than first value.
+    
+    In LoRA with Kroneckor Product, first value is a value for weight scale.
+    secon value is a value for weight.
+    
+    Becuase of non-commutative property, A⊗B ≠ B⊗A. Meaning of two matrices is slightly different.
+    
+    examples)
+    factor
+        -1               2                4               8               16               ...
+    127 -> 127, 1   127 -> 127, 1    127 -> 127, 1   127 -> 127, 1   127 -> 127, 1
+    128 -> 16, 8    128 -> 64, 2     128 -> 32, 4    128 -> 16, 8    128 -> 16, 8
+    250 -> 125, 2   250 -> 125, 2    250 -> 125, 2   250 -> 125, 2   250 -> 125, 2
+    360 -> 45, 8    360 -> 180, 2    360 -> 90, 4    360 -> 45, 8    360 -> 45, 8
+    512 -> 32, 16   512 -> 256, 2    512 -> 128, 4   512 -> 64, 8    512 -> 32, 16
+    1024 -> 32, 32  1024 -> 512, 2   1024 -> 256, 4  1024 -> 128, 8  1024 -> 64, 16
+    '''
+    
+    if factor > 0 and (dimension % factor) == 0:
+        m = factor
+        n = dimension // factor
+        return m, n
+    if factor == -1:
+        factor = dimension
+    m, n = 1, dimension
+    length = m + n
+    while m<n:
+        new_m = m + 1
+        while dimension%new_m != 0:
+            new_m += 1
+        new_n = dimension // new_m
+        if new_m + new_n > length or new_m>factor:
+            break
+        else:
+            m, n = new_m, new_n
+    if m > n:
+        n, m = m, n
+    return m, n
+
+
+def make_weight_cp(t, wa, wb):
+    rebuild2 = torch.einsum('i j k l, i p, j r -> p r k l', t, wa, wb) # [c, d, k1, k2]
+    return rebuild2
+
+
+def make_kron(orig_weight, w1, w2, scale):
+    if len(w2.shape) == 4:
+        w1 = w1.unsqueeze(2).unsqueeze(2)
+    w2 = w2.contiguous()
+    return orig_weight + torch.kron(w1, w2).reshape(orig_weight.shape)*scale
+
+
+class LokrModule(nn.Module):
+    """
+    modifed from kohya-ss/sd-scripts/networks/lora:LoRAModule
+        and from KohakuBlueleaf/LyCORIS/lycoris:loha:LoHaModule
+        and from KohakuBlueleaf/LyCORIS/lycoris:locon:LoconModule
+    """
+
+    def __init__(
+        self, 
+        lora_name, org_module: nn.Module, 
+        multiplier=1.0, 
+        lora_dim=4, alpha=1, 
+        dropout=0.,
+        use_cp=False,
+        decompose_both = False,
+        factor:int=-1, # factorization factor
+        **kwargs,
+    ):
+        """ if alpha == 0 or None, alpha is rank (no scaling). """
+        super().__init__()
+        factor = int(factor)
+        self.lora_name = lora_name
+        self.lora_dim = lora_dim
+        self.cp = False
+        self.use_w1 = False
+        self.use_w2 = False
+
+        self.shape = org_module.weight.shape
+        if org_module.__class__.__name__ == 'Conv2d':
+            in_dim = org_module.in_channels
+            k_size = org_module.kernel_size
+            out_dim = org_module.out_channels
+            
+            in_m, in_n = factorization(in_dim, factor)
+            out_l, out_k = factorization(out_dim, factor)
+            shape = ((out_l, out_k), (in_m, in_n), *k_size) # ((a, b), (c, d), *k_size)
+            
+            self.cp = use_cp and k_size!=(1, 1)
+            if decompose_both and lora_dim < max(shape[0][0], shape[1][0])/2:
+                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
+                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
+            else:
+                self.use_w1 = True
+                self.lokr_w1 = nn.Parameter(torch.empty(shape[0][0], shape[1][0]))  # a*c, 1-mode
+            
+            if lora_dim >= max(shape[0][1], shape[1][1])/2:
+                self.use_w2 = True
+                self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1], *k_size))
+            elif self.cp:
+                self.lokr_t2 = nn.Parameter(torch.empty(lora_dim, lora_dim, shape[2], shape[3]))
+                self.lokr_w2_a = nn.Parameter(torch.empty(lora_dim, shape[0][1])) # b, 1-mode
+                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1])) # d, 2-mode
+            else: # Conv2d not cp
+                # bigger part. weight and LoRA. [b, dim] x [dim, d*k1*k2]
+                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
+                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1]*shape[2]*shape[3]))
+                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d*k1*k2)) = (a, b)⊗(c, d*k1*k2) = (ac, bd*k1*k2)
+            
+            self.op = F.conv2d
+            self.extra_args = {
+                "stride": org_module.stride,
+                "padding": org_module.padding,
+                "dilation": org_module.dilation,
+                "groups": org_module.groups
+            }
+
+        else: # Linear
+            in_dim = org_module.in_features
+            out_dim = org_module.out_features
+            
+            in_m, in_n = factorization(in_dim, factor)
+            out_l, out_k = factorization(out_dim, factor)
+            shape = ((out_l, out_k), (in_m, in_n)) # ((a, b), (c, d)), out_dim = a*c, in_dim = b*d
+            
+            # smaller part. weight scale
+            if decompose_both and lora_dim < max(shape[0][0], shape[1][0])/2:
+                self.lokr_w1_a = nn.Parameter(torch.empty(shape[0][0], lora_dim))
+                self.lokr_w1_b = nn.Parameter(torch.empty(lora_dim, shape[1][0]))
+            else:
+                self.use_w1 = True
+                self.lokr_w1 = nn.Parameter(torch.empty(shape[0][0], shape[1][0]))  # a*c, 1-mode
+
+            if lora_dim < max(shape[0][1], shape[1][1])/2:
+                # bigger part. weight and LoRA. [b, dim] x [dim, d]
+                self.lokr_w2_a = nn.Parameter(torch.empty(shape[0][1], lora_dim))
+                self.lokr_w2_b = nn.Parameter(torch.empty(lora_dim, shape[1][1]))
+                # w1 ⊗ (w2_a x w2_b) = (a, b)⊗((c, dim)x(dim, d)) = (a, b)⊗(c, d) = (ac, bd)
+            else:
+                self.use_w2 = True
+                self.lokr_w2 = nn.Parameter(torch.empty(shape[0][1], shape[1][1]))
+
+            self.op = F.linear
+            self.extra_args = {}
+        
+        if dropout:
+            self.dropout = nn.Dropout(dropout)
+        else:
+            self.dropout = nn.Identity()
+        
+        if isinstance(alpha, torch.Tensor):
+            alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
+        alpha = lora_dim if alpha is None or alpha == 0 else alpha
+        if self.use_w2 and self.use_w1:
+            #use scale = 1
+            alpha = lora_dim
+        self.scale = alpha / self.lora_dim
+        self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
+
+        if self.use_w2:
+            torch.nn.init.constant_(self.lokr_w2, 0)
+        else:
+            if self.cp:
+                torch.nn.init.normal_(self.lokr_t2, std=0.1)
+            torch.nn.init.normal_(self.lokr_w2_a, std=1)
+            torch.nn.init.constant_(self.lokr_w2_b, 0)
+        
+        if self.use_w1:
+            torch.nn.init.normal_(self.lokr_w1, std=1)
+        else:
+            torch.nn.init.normal_(self.lokr_w1_a, std=1)
+            torch.nn.init.normal_(self.lokr_w1_b, std=0.1)
+
+        self.multiplier = multiplier
+        self.org_module = [org_module]
+        weight = make_kron(
+            self.org_module[0].weight.data, 
+            self.lokr_w1 if self.use_w1 else self.lokr_w1_a@self.lokr_w1_b,
+            (self.lokr_w2 if self.use_w2 
+             else make_weight_cp(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b) if self.cp 
+             else self.lokr_w2_a@self.lokr_w2_b),
+            torch.tensor(self.multiplier * self.scale)
+        )
+        assert torch.sum(torch.isnan(weight)) == 0, "weight is nan"
+
+    # Same as locon.py
+    def apply_to(self):
+        self.org_forward = self.org_module[0].forward
+        self.org_module[0].forward = self.forward
+    
+    def get_weight(self):
+        weight = make_kron(
+            0, 
+            self.lokr_w1 if self.use_w1 else self.lokr_w1_a@self.lokr_w1_b,
+            (self.lokr_w2 if self.use_w2 
+             else make_weight_cp(self.lokr_t2, self.lokr_w2_a, self.lokr_w2_b) if self.cp 
+             else self.lokr_w2_a@self.lokr_w2_b),
+            torch.tensor(self.scale)
+        )
+        return weight
+
+    @torch.no_grad()
+    def apply_max_norm(self, max_norm, device=None):
+        norm = torch.clamp(self.get_weight().norm(), max_norm/2)
+        desired = torch.clamp(norm, max=max_norm)
+        ratio = desired.cpu()/norm.cpu()
+        
+        scaled = ratio != 1.0
+        if scaled:
+            modules = (4 - self.use_w1 - self.use_w2 + (not self.use_w2 and self.cp))
+            if self.use_w1:
+                self.lokr_w1_a *= ratio**(1/modules)
+                self.lokr_w1_b *= ratio**(1/modules)
+            else:
+                self.lokr_w1 *= ratio**(1/modules)
+            
+            if self.use_w2:
+                if self.cp:
+                    self.lokr_t2 *= ratio**(1/modules)
+                self.lokr_w2_a  *= ratio**(1/modules)
+                self.lokr_w2_b  *= ratio**(1/modules)
+            else:
+                self.lokr_w2 *= ratio**(1/modules)
+        
+        return scaled, norm*ratio
+
+    def forward(self, x):
+        weight = self.org_module[0].weight.data + self.get_weight() * self.multiplier
+        bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
+        return self.op(
+            x, 
+            weight.view(self.shape),
+            bias,
+            **self.extra_args
+        )
```

### Comparing `lycoris_lora-0.1.6.dev1/lycoris/utils.py` & `lycoris_lora-0.1.7.dev1/lycoris/utils.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,504 +1,504 @@
-from typing import *
-
-import numpy as np
-
-import torch
-import torch.nn as nn
-import torch.nn.functional as F
-
-import torch.linalg as linalg
-
-from tqdm import tqdm
-
-
-def make_sparse(t: torch.Tensor, sparsity=0.95):
-    abs_t = torch.abs(t)
-    np_array = abs_t.detach().cpu().numpy()
-    quan = float(np.quantile(np_array, sparsity))
-    sparse_t = t.masked_fill(abs_t < quan, 0)
-    return sparse_t
-
-
-def extract_conv(
-    weight: Union[torch.Tensor, nn.Parameter],
-    mode = 'fixed',
-    mode_param = 0,
-    device = 'cpu',
-    is_cp = False,
-) -> Tuple[nn.Parameter, nn.Parameter]:
-    weight = weight.to(device)
-    out_ch, in_ch, kernel_size, _ = weight.shape
-    
-    U, S, Vh = linalg.svd(weight.reshape(out_ch, -1))
-    
-    if mode=='fixed':
-        lora_rank = mode_param
-    elif mode=='threshold':
-        assert mode_param>=0
-        lora_rank = torch.sum(S>mode_param)
-    elif mode=='ratio':
-        assert 1>=mode_param>=0
-        min_s = torch.max(S)*mode_param
-        lora_rank = torch.sum(S>min_s)
-    elif mode=='quantile' or mode=='percentile':
-        assert 1>=mode_param>=0
-        s_cum = torch.cumsum(S, dim=0)
-        min_cum_sum = mode_param * torch.sum(S)
-        lora_rank = torch.sum(s_cum<min_cum_sum)
-    else:
-        raise NotImplementedError('Extract mode should be "fixed", "threshold", "ratio" or "quantile"')
-    lora_rank = max(1, lora_rank)
-    lora_rank = min(out_ch, in_ch, lora_rank)
-    if lora_rank>=out_ch/2 and not is_cp:
-        return weight, 'full'
-    
-    U = U[:, :lora_rank]
-    S = S[:lora_rank]
-    U = U @ torch.diag(S)
-    Vh = Vh[:lora_rank, :]
-    
-    diff = (weight - (U @ Vh).reshape(out_ch, in_ch, kernel_size, kernel_size)).detach()
-    extract_weight_A = Vh.reshape(lora_rank, in_ch, kernel_size, kernel_size).detach()
-    extract_weight_B = U.reshape(out_ch, lora_rank, 1, 1).detach()
-    del U, S, Vh, weight
-    return (extract_weight_A, extract_weight_B, diff), 'low rank'
-
-
-def extract_linear(
-    weight: Union[torch.Tensor, nn.Parameter],
-    mode = 'fixed',
-    mode_param = 0,
-    device = 'cpu',
-) -> Tuple[nn.Parameter, nn.Parameter]:
-    weight = weight.to(device)
-    out_ch, in_ch = weight.shape
-    
-    U, S, Vh = linalg.svd(weight)
-    
-    if mode=='fixed':
-        lora_rank = mode_param
-    elif mode=='threshold':
-        assert mode_param>=0
-        lora_rank = torch.sum(S>mode_param)
-    elif mode=='ratio':
-        assert 1>=mode_param>=0
-        min_s = torch.max(S)*mode_param
-        lora_rank = torch.sum(S>min_s)
-    elif mode=='quantile' or mode=='percentile':
-        assert 1>=mode_param>=0
-        s_cum = torch.cumsum(S, dim=0)
-        min_cum_sum = mode_param * torch.sum(S)
-        lora_rank = torch.sum(s_cum<min_cum_sum)
-    else:
-        raise NotImplementedError('Extract mode should be "fixed", "threshold", "ratio" or "quantile"')
-    lora_rank = max(1, lora_rank)
-    lora_rank = min(out_ch, in_ch, lora_rank)
-    if lora_rank>=out_ch/2:
-        return weight, 'full'
-    
-    U = U[:, :lora_rank]
-    S = S[:lora_rank]
-    U = U @ torch.diag(S)
-    Vh = Vh[:lora_rank, :]
-    
-    diff = (weight - U @ Vh).detach()
-    extract_weight_A = Vh.reshape(lora_rank, in_ch).detach()
-    extract_weight_B = U.reshape(out_ch, lora_rank).detach()
-    del U, S, Vh, weight
-    return (extract_weight_A, extract_weight_B, diff), 'low rank'
-
-
-def extract_diff(
-    base_model,
-    db_model,
-    mode = 'fixed',
-    linear_mode_param = 0,
-    conv_mode_param = 0,
-    extract_device = 'cpu',
-    use_bias = False,
-    sparsity = 0.98,
-    small_conv = True
-):
-    UNET_TARGET_REPLACE_MODULE = [
-        "Transformer2DModel", 
-        "Attention", 
-        "ResnetBlock2D", 
-        "Downsample2D", 
-        "Upsample2D"
-    ]
-    UNET_TARGET_REPLACE_NAME = [
-        "conv_in",
-        "conv_out",
-        "time_embedding.linear_1",
-        "time_embedding.linear_2",
-    ]
-    TEXT_ENCODER_TARGET_REPLACE_MODULE = ["CLIPAttention", "CLIPMLP"]
-    LORA_PREFIX_UNET = 'lora_unet'
-    LORA_PREFIX_TEXT_ENCODER = 'lora_te'
-    def make_state_dict(
-        prefix, 
-        root_module: torch.nn.Module,
-        target_module: torch.nn.Module,
-        target_replace_modules,
-        target_replace_names = []
-    ):
-        loras = {}
-        temp = {}
-        temp_name = {}
-        
-        for name, module in root_module.named_modules():
-            if module.__class__.__name__ in target_replace_modules:
-                temp[name] = {}
-                for child_name, child_module in module.named_modules():
-                    if child_module.__class__.__name__ not in {'Linear', 'Conv2d'}:
-                        continue
-                    temp[name][child_name] = child_module.weight
-            elif name in target_replace_names:
-                temp_name[name] = module.weight
-        
-        for name, module in tqdm(list(target_module.named_modules())):
-            if name in temp:
-                weights = temp[name]
-                for child_name, child_module in module.named_modules():
-                    lora_name = prefix + '.' + name + '.' + child_name
-                    lora_name = lora_name.replace('.', '_')
-                    layer = child_module.__class__.__name__
-                    if layer in {'Linear', 'Conv2d'}:
-                        root_weight = child_module.weight
-                        if torch.allclose(root_weight, weights[child_name]):
-                            continue
-                    
-                    if layer == 'Linear':
-                        weight, decompose_mode = extract_linear(
-                            (child_module.weight - weights[child_name]),
-                            mode,
-                            linear_mode_param,
-                            device = extract_device,
-                        )
-                        if decompose_mode == 'low rank':
-                            extract_a, extract_b, diff = weight
-                    elif layer == 'Conv2d':
-                        is_linear = (child_module.weight.shape[2] == 1
-                                     and child_module.weight.shape[3] == 1)
-                        weight, decompose_mode = extract_conv(
-                            (child_module.weight - weights[child_name]), 
-                            mode,
-                            linear_mode_param if is_linear else conv_mode_param,
-                            device = extract_device,
-                        )
-                        if decompose_mode == 'low rank':
-                            extract_a, extract_b, diff = weight
-                        if small_conv and not is_linear and decompose_mode == 'low rank':
-                            dim = extract_a.size(0)
-                            (extract_c, extract_a, _), _ = extract_conv(
-                                extract_a.transpose(0, 1), 
-                                'fixed', dim, 
-                                extract_device, True
-                            )
-                            extract_a = extract_a.transpose(0, 1)
-                            extract_c = extract_c.transpose(0, 1)
-                            loras[f'{lora_name}.lora_mid.weight'] = extract_c.detach().cpu().contiguous().half()
-                            diff = child_module.weight - torch.einsum(
-                                'i j k l, j r, p i -> p r k l', 
-                                extract_c, extract_a.flatten(1, -1), extract_b.flatten(1, -1)
-                            ).detach().cpu().contiguous()
-                            del extract_c
-                    else:
-                        continue
-                    if decompose_mode == 'low rank':
-                        loras[f'{lora_name}.lora_down.weight'] = extract_a.detach().cpu().contiguous().half()
-                        loras[f'{lora_name}.lora_up.weight'] = extract_b.detach().cpu().contiguous().half()
-                        loras[f'{lora_name}.alpha'] = torch.Tensor([extract_a.shape[0]]).half()
-                        if use_bias:
-                            diff = diff.detach().cpu().reshape(extract_b.size(0), -1)
-                            sparse_diff = make_sparse(diff, sparsity).to_sparse().coalesce()
-                            
-                            indices = sparse_diff.indices().to(torch.int16)
-                            values = sparse_diff.values().half()
-                            loras[f'{lora_name}.bias_indices'] = indices
-                            loras[f'{lora_name}.bias_values'] = values
-                            loras[f'{lora_name}.bias_size'] = torch.tensor(diff.shape).to(torch.int16)
-                        del extract_a, extract_b, diff
-                    elif decompose_mode == 'full':
-                        loras[f'{lora_name}.diff'] = weight.detach().cpu().contiguous().half()
-                    else:
-                        raise NotImplementedError
-            elif name in temp_name:
-                weights = temp_name[name]
-                lora_name = prefix + '.' + name
-                lora_name = lora_name.replace('.', '_')
-                layer = module.__class__.__name__
-                
-                if layer in {'Linear', 'Conv2d'}:
-                    root_weight = module.weight
-                    if torch.allclose(root_weight, weights):
-                        continue
-                
-                if layer == 'Linear':
-                    weight, decompose_mode = extract_linear(
-                        (root_weight - weights),
-                        mode,
-                        linear_mode_param,
-                        device = extract_device,
-                    )
-                    if decompose_mode == 'low rank':
-                        extract_a, extract_b, diff = weight
-                elif layer == 'Conv2d':
-                    is_linear = (
-                        root_weight.shape[2] == 1
-                        and root_weight.shape[3] == 1
-                    )
-                    weight, decompose_mode = extract_conv(
-                        (root_weight - weights), 
-                        mode,
-                        linear_mode_param if is_linear else conv_mode_param,
-                        device = extract_device,
-                    )
-                    if decompose_mode == 'low rank':
-                        extract_a, extract_b, diff = weight
-                    if small_conv and not is_linear and decompose_mode == 'low rank':
-                        dim = extract_a.size(0)
-                        (extract_c, extract_a, _), _ = extract_conv(
-                            extract_a.transpose(0, 1), 
-                            'fixed', dim, 
-                            extract_device, True
-                        )
-                        extract_a = extract_a.transpose(0, 1)
-                        extract_c = extract_c.transpose(0, 1)
-                        loras[f'{lora_name}.lora_mid.weight'] = extract_c.detach().cpu().contiguous().half()
-                        diff = root_weight - torch.einsum(
-                            'i j k l, j r, p i -> p r k l', 
-                            extract_c, extract_a.flatten(1, -1), extract_b.flatten(1, -1)
-                        ).detach().cpu().contiguous()
-                        del extract_c
-                else:
-                    continue
-                if decompose_mode == 'low rank':
-                    loras[f'{lora_name}.lora_down.weight'] = extract_a.detach().cpu().contiguous().half()
-                    loras[f'{lora_name}.lora_up.weight'] = extract_b.detach().cpu().contiguous().half()
-                    loras[f'{lora_name}.alpha'] = torch.Tensor([extract_a.shape[0]]).half()
-                    if use_bias:
-                        diff = diff.detach().cpu().reshape(extract_b.size(0), -1)
-                        sparse_diff = make_sparse(diff, sparsity).to_sparse().coalesce()
-                        
-                        indices = sparse_diff.indices().to(torch.int16)
-                        values = sparse_diff.values().half()
-                        loras[f'{lora_name}.bias_indices'] = indices
-                        loras[f'{lora_name}.bias_values'] = values
-                        loras[f'{lora_name}.bias_size'] = torch.tensor(diff.shape).to(torch.int16)
-                    del extract_a, extract_b, diff
-                elif decompose_mode == 'full':
-                    loras[f'{lora_name}.diff'] = weight.detach().cpu().contiguous().half()
-                else:
-                    raise NotImplementedError
-        return loras
-    
-    text_encoder_loras = make_state_dict(
-        LORA_PREFIX_TEXT_ENCODER, 
-        base_model[0], db_model[0], 
-        TEXT_ENCODER_TARGET_REPLACE_MODULE
-    )
-    
-    unet_loras = make_state_dict(
-        LORA_PREFIX_UNET,
-        base_model[2], db_model[2], 
-        UNET_TARGET_REPLACE_MODULE,
-        UNET_TARGET_REPLACE_NAME
-    )
-    print(len(text_encoder_loras), len(unet_loras))
-    return text_encoder_loras|unet_loras
-
-
-def get_module(
-    lyco_state_dict: Dict,
-    lora_name
-):
-    if f'{lora_name}.lora_up.weight' in lyco_state_dict:
-        up = lyco_state_dict[f'{lora_name}.lora_up.weight']
-        down = lyco_state_dict[f'{lora_name}.lora_down.weight']
-        mid = lyco_state_dict.get(f'{lora_name}.lora_mid.weight', None)
-        alpha = lyco_state_dict.get(f'{lora_name}.alpha', None)
-        return 'locon', (up, down, mid, alpha)
-    elif f'{lora_name}.hada_w1_a' in lyco_state_dict:
-        w1a = lyco_state_dict[f'{lora_name}.hada_w1_a']
-        w1b = lyco_state_dict[f'{lora_name}.hada_w1_b']
-        w2a = lyco_state_dict[f'{lora_name}.hada_w2_a']
-        w2b = lyco_state_dict[f'{lora_name}.hada_w2_b']
-        t1 = lyco_state_dict.get(f'{lora_name}.hada_t1', None)
-        t2 = lyco_state_dict.get(f'{lora_name}.hada_t2', None)
-        alpha = lyco_state_dict.get(f'{lora_name}.alpha', None)
-        return 'hada', (w1a, w1b, w2a, w2b, t1, t2, alpha)
-    elif f'{lora_name}.weight' in lyco_state_dict:
-        weight = lyco_state_dict[f'{lora_name}.weight']
-        on_input = lyco_state_dict.get(f'{lora_name}.on_input', False)
-        return 'ia3', (weight, on_input)
-    elif (f'{lora_name}.lokr_w1' in lyco_state_dict
-          or f'{lora_name}.lokr_w1_a' in lyco_state_dict):
-        w1 = lyco_state_dict.get(f'{lora_name}.lokr_w1', None)
-        w1a = lyco_state_dict.get(f'{lora_name}.lokr_w1_a', None)
-        w1b = lyco_state_dict.get(f'{lora_name}.lokr_w1_b', None)
-        w2 = lyco_state_dict.get(f'{lora_name}.lokr_w2', None)
-        w2a = lyco_state_dict.get(f'{lora_name}.lokr_w2_a', None)
-        w2b = lyco_state_dict.get(f'{lora_name}.lokr_w2_b', None)
-        t1 = lyco_state_dict.get(f'{lora_name}.lokr_t1', None)
-        t2 = lyco_state_dict.get(f'{lora_name}.lokr_t2', None)
-        alpha = lyco_state_dict.get(f'{lora_name}.alpha', None)
-        return 'kron', (w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha)
-    elif f'{lora_name}.diff' in lyco_state_dict:
-        return 'full', lyco_state_dict[f'{lora_name}.diff']
-    else:
-        return 'None', ()
-
-
-def cp_weight_from_conv(
-    up, down, mid
-):
-    up = up.reshape(up.size(0), up.size(1))
-    down = down.reshape(down.size(0), down.size(1))
-    return torch.einsum('m n w h, i m, n j -> i j w h', mid, up, down)
-
-def cp_weight(
-    wa, wb, t
-):
-    temp = torch.einsum('i j k l, j r -> i r k l', t, wb)
-    return torch.einsum('i j k l, i r -> r j k l', temp, wa)
-
-
-@torch.no_grad()
-def rebuild_weight(module_type, params, orig_weight, scale=1):
-    if orig_weight is None:
-        return orig_weight
-    merged = orig_weight
-    if module_type == 'locon':
-        up, down, mid, alpha = params
-        if alpha is not None:
-            scale *= alpha/up.size(1)
-        if mid is not None:
-            rebuild = cp_weight_from_conv(up, down, mid)
-        else:
-            rebuild = up.reshape(up.size(0),-1) @ down.reshape(down.size(0), -1)
-        merged = orig_weight + rebuild.reshape(orig_weight.shape) * scale
-        del up, down, mid, alpha, params, rebuild
-    elif module_type == 'hada':
-        w1a, w1b, w2a, w2b, t1, t2, alpha = params
-        if alpha is not None:
-            scale *= alpha / w1b.size(0)
-        if t1 is not None:
-            rebuild1 = cp_weight(w1a, w1b, t1)
-        else:
-            rebuild1 = w1a @ w1b
-        if t2 is not None:
-            rebuild2 = cp_weight(w2a, w2b, t2)
-        else:
-            rebuild2 = w2a @ w2b
-        rebuild = (rebuild1 * rebuild2).reshape(orig_weight.shape)
-        merged = orig_weight + rebuild * scale
-        del w1a, w1b, w2a, w2b, t1, t2, alpha, params, rebuild, rebuild1, rebuild2
-    elif module_type == 'ia3':
-        weight, on_input = params
-        if not on_input:
-            weight = weight.reshape(-1, 1)
-        merged = orig_weight + weight * orig_weight * scale
-        del weight, on_input, params
-    elif module_type == 'kron':
-        w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha = params
-        if alpha is not None and (w1b is not None or w2b is not None):
-            scale *= alpha / (w1b.size(0) if w1b else w2b.size(0))
-        if w1a is not None and w1b is not None:
-            if t1:
-                w1 = cp_weight(w1a, w1b, t1)
-            else:
-                w1 = w1a @ w1b
-        if w2a is not None and w2b is not None:
-            if t2:
-                w2 = cp_weight(w2a, w2b, t2)
-            else:
-                w2 = w2a @ w2b
-        rebuild = torch.kron(w1, w2).reshape(orig_weight.shape) 
-        merged = orig_weight + rebuild* scale
-        del w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha, params, rebuild
-    elif module_type == 'full':
-        rebuild = params.reshape(orig_weight.shape) 
-        merged = orig_weight + rebuild * scale
-        del params, rebuild
-    
-    return merged
-
-
-def merge(
-    base_model,
-    lyco_state_dict,
-    scale: float = 1.0,
-    device = 'cpu'
-):
-    UNET_TARGET_REPLACE_MODULE = [
-        "Transformer2DModel", 
-        "Attention", 
-        "ResnetBlock2D", 
-        "Downsample2D", 
-        "Upsample2D"
-    ]
-    UNET_TARGET_REPLACE_NAME = [
-        "conv_in",
-        "conv_out",
-        "time_embedding.linear_1",
-        "time_embedding.linear_2",
-    ]
-    TEXT_ENCODER_TARGET_REPLACE_MODULE = ["CLIPAttention", "CLIPMLP"]
-    LORA_PREFIX_UNET = 'lora_unet'
-    LORA_PREFIX_TEXT_ENCODER = 'lora_te'
-    merged = 0
-    def merge_state_dict(
-        prefix, 
-        root_module: torch.nn.Module,
-        lyco_state_dict: Dict[str,torch.Tensor],
-        target_replace_modules,
-        target_replace_names = []
-    ):
-        nonlocal merged
-        for name, module in tqdm(list(root_module.named_modules()), desc=f'Merging {prefix}'):
-            if module.__class__.__name__ in target_replace_modules:
-                for child_name, child_module in module.named_modules():
-                    if child_module.__class__.__name__ not in {'Linear', 'Conv2d'}:
-                        continue
-                    lora_name = prefix + '.' + name + '.' + child_name
-                    lora_name = lora_name.replace('.', '_')
-                    
-                    result = rebuild_weight(*get_module(
-                        lyco_state_dict, lora_name
-                    ), getattr(child_module, 'weight'), scale)
-                    if result is not None:
-                        merged += 1
-                        child_module.requires_grad_(False)
-                        child_module.weight.copy_(result)
-            elif name in target_replace_names:
-                lora_name = prefix + '.' + name
-                lora_name = lora_name.replace('.', '_')
-                    
-                result = rebuild_weight(*get_module(
-                    lyco_state_dict, lora_name
-                ), getattr(module, 'weight'), scale)
-                if result is not None:
-                    merged += 1
-                    module.requires_grad_(False)
-                    module.weight.copy_(result)
-    
-    if device == 'cpu':
-        for k, v in tqdm(list(lyco_state_dict.items()), desc='Converting Dtype'):
-            lyco_state_dict[k] = v.float()
-    
-    merge_state_dict(
-        LORA_PREFIX_TEXT_ENCODER,
-        base_model[0],
-        lyco_state_dict,
-        TEXT_ENCODER_TARGET_REPLACE_MODULE,
-        UNET_TARGET_REPLACE_NAME
-    )
-    merge_state_dict(
-        LORA_PREFIX_UNET,
-        base_model[2],
-        lyco_state_dict,
-        UNET_TARGET_REPLACE_MODULE,
-        UNET_TARGET_REPLACE_NAME
-    )
-    print(f'{merged} Modules been merged')
+from typing import *
+
+import numpy as np
+
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+
+import torch.linalg as linalg
+
+from tqdm import tqdm
+
+
+def make_sparse(t: torch.Tensor, sparsity=0.95):
+    abs_t = torch.abs(t)
+    np_array = abs_t.detach().cpu().numpy()
+    quan = float(np.quantile(np_array, sparsity))
+    sparse_t = t.masked_fill(abs_t < quan, 0)
+    return sparse_t
+
+
+def extract_conv(
+    weight: Union[torch.Tensor, nn.Parameter],
+    mode = 'fixed',
+    mode_param = 0,
+    device = 'cpu',
+    is_cp = False,
+) -> Tuple[nn.Parameter, nn.Parameter]:
+    weight = weight.to(device)
+    out_ch, in_ch, kernel_size, _ = weight.shape
+    
+    U, S, Vh = linalg.svd(weight.reshape(out_ch, -1))
+    
+    if mode=='fixed':
+        lora_rank = mode_param
+    elif mode=='threshold':
+        assert mode_param>=0
+        lora_rank = torch.sum(S>mode_param)
+    elif mode=='ratio':
+        assert 1>=mode_param>=0
+        min_s = torch.max(S)*mode_param
+        lora_rank = torch.sum(S>min_s)
+    elif mode=='quantile' or mode=='percentile':
+        assert 1>=mode_param>=0
+        s_cum = torch.cumsum(S, dim=0)
+        min_cum_sum = mode_param * torch.sum(S)
+        lora_rank = torch.sum(s_cum<min_cum_sum)
+    else:
+        raise NotImplementedError('Extract mode should be "fixed", "threshold", "ratio" or "quantile"')
+    lora_rank = max(1, lora_rank)
+    lora_rank = min(out_ch, in_ch, lora_rank)
+    if lora_rank>=out_ch/2 and not is_cp:
+        return weight, 'full'
+    
+    U = U[:, :lora_rank]
+    S = S[:lora_rank]
+    U = U @ torch.diag(S)
+    Vh = Vh[:lora_rank, :]
+    
+    diff = (weight - (U @ Vh).reshape(out_ch, in_ch, kernel_size, kernel_size)).detach()
+    extract_weight_A = Vh.reshape(lora_rank, in_ch, kernel_size, kernel_size).detach()
+    extract_weight_B = U.reshape(out_ch, lora_rank, 1, 1).detach()
+    del U, S, Vh, weight
+    return (extract_weight_A, extract_weight_B, diff), 'low rank'
+
+
+def extract_linear(
+    weight: Union[torch.Tensor, nn.Parameter],
+    mode = 'fixed',
+    mode_param = 0,
+    device = 'cpu',
+) -> Tuple[nn.Parameter, nn.Parameter]:
+    weight = weight.to(device)
+    out_ch, in_ch = weight.shape
+    
+    U, S, Vh = linalg.svd(weight)
+    
+    if mode=='fixed':
+        lora_rank = mode_param
+    elif mode=='threshold':
+        assert mode_param>=0
+        lora_rank = torch.sum(S>mode_param)
+    elif mode=='ratio':
+        assert 1>=mode_param>=0
+        min_s = torch.max(S)*mode_param
+        lora_rank = torch.sum(S>min_s)
+    elif mode=='quantile' or mode=='percentile':
+        assert 1>=mode_param>=0
+        s_cum = torch.cumsum(S, dim=0)
+        min_cum_sum = mode_param * torch.sum(S)
+        lora_rank = torch.sum(s_cum<min_cum_sum)
+    else:
+        raise NotImplementedError('Extract mode should be "fixed", "threshold", "ratio" or "quantile"')
+    lora_rank = max(1, lora_rank)
+    lora_rank = min(out_ch, in_ch, lora_rank)
+    if lora_rank>=out_ch/2:
+        return weight, 'full'
+    
+    U = U[:, :lora_rank]
+    S = S[:lora_rank]
+    U = U @ torch.diag(S)
+    Vh = Vh[:lora_rank, :]
+    
+    diff = (weight - U @ Vh).detach()
+    extract_weight_A = Vh.reshape(lora_rank, in_ch).detach()
+    extract_weight_B = U.reshape(out_ch, lora_rank).detach()
+    del U, S, Vh, weight
+    return (extract_weight_A, extract_weight_B, diff), 'low rank'
+
+
+def extract_diff(
+    base_model,
+    db_model,
+    mode = 'fixed',
+    linear_mode_param = 0,
+    conv_mode_param = 0,
+    extract_device = 'cpu',
+    use_bias = False,
+    sparsity = 0.98,
+    small_conv = True
+):
+    UNET_TARGET_REPLACE_MODULE = [
+        "Transformer2DModel", 
+        "Attention", 
+        "ResnetBlock2D", 
+        "Downsample2D", 
+        "Upsample2D"
+    ]
+    UNET_TARGET_REPLACE_NAME = [
+        "conv_in",
+        "conv_out",
+        "time_embedding.linear_1",
+        "time_embedding.linear_2",
+    ]
+    TEXT_ENCODER_TARGET_REPLACE_MODULE = ["CLIPAttention", "CLIPMLP"]
+    LORA_PREFIX_UNET = 'lora_unet'
+    LORA_PREFIX_TEXT_ENCODER = 'lora_te'
+    def make_state_dict(
+        prefix, 
+        root_module: torch.nn.Module,
+        target_module: torch.nn.Module,
+        target_replace_modules,
+        target_replace_names = []
+    ):
+        loras = {}
+        temp = {}
+        temp_name = {}
+        
+        for name, module in root_module.named_modules():
+            if module.__class__.__name__ in target_replace_modules:
+                temp[name] = {}
+                for child_name, child_module in module.named_modules():
+                    if child_module.__class__.__name__ not in {'Linear', 'Conv2d'}:
+                        continue
+                    temp[name][child_name] = child_module.weight
+            elif name in target_replace_names:
+                temp_name[name] = module.weight
+        
+        for name, module in tqdm(list(target_module.named_modules())):
+            if name in temp:
+                weights = temp[name]
+                for child_name, child_module in module.named_modules():
+                    lora_name = prefix + '.' + name + '.' + child_name
+                    lora_name = lora_name.replace('.', '_')
+                    layer = child_module.__class__.__name__
+                    if layer in {'Linear', 'Conv2d'}:
+                        root_weight = child_module.weight
+                        if torch.allclose(root_weight, weights[child_name]):
+                            continue
+                    
+                    if layer == 'Linear':
+                        weight, decompose_mode = extract_linear(
+                            (child_module.weight - weights[child_name]),
+                            mode,
+                            linear_mode_param,
+                            device = extract_device,
+                        )
+                        if decompose_mode == 'low rank':
+                            extract_a, extract_b, diff = weight
+                    elif layer == 'Conv2d':
+                        is_linear = (child_module.weight.shape[2] == 1
+                                     and child_module.weight.shape[3] == 1)
+                        weight, decompose_mode = extract_conv(
+                            (child_module.weight - weights[child_name]), 
+                            mode,
+                            linear_mode_param if is_linear else conv_mode_param,
+                            device = extract_device,
+                        )
+                        if decompose_mode == 'low rank':
+                            extract_a, extract_b, diff = weight
+                        if small_conv and not is_linear and decompose_mode == 'low rank':
+                            dim = extract_a.size(0)
+                            (extract_c, extract_a, _), _ = extract_conv(
+                                extract_a.transpose(0, 1), 
+                                'fixed', dim, 
+                                extract_device, True
+                            )
+                            extract_a = extract_a.transpose(0, 1)
+                            extract_c = extract_c.transpose(0, 1)
+                            loras[f'{lora_name}.lora_mid.weight'] = extract_c.detach().cpu().contiguous().half()
+                            diff = child_module.weight - torch.einsum(
+                                'i j k l, j r, p i -> p r k l', 
+                                extract_c, extract_a.flatten(1, -1), extract_b.flatten(1, -1)
+                            ).detach().cpu().contiguous()
+                            del extract_c
+                    else:
+                        continue
+                    if decompose_mode == 'low rank':
+                        loras[f'{lora_name}.lora_down.weight'] = extract_a.detach().cpu().contiguous().half()
+                        loras[f'{lora_name}.lora_up.weight'] = extract_b.detach().cpu().contiguous().half()
+                        loras[f'{lora_name}.alpha'] = torch.Tensor([extract_a.shape[0]]).half()
+                        if use_bias:
+                            diff = diff.detach().cpu().reshape(extract_b.size(0), -1)
+                            sparse_diff = make_sparse(diff, sparsity).to_sparse().coalesce()
+                            
+                            indices = sparse_diff.indices().to(torch.int16)
+                            values = sparse_diff.values().half()
+                            loras[f'{lora_name}.bias_indices'] = indices
+                            loras[f'{lora_name}.bias_values'] = values
+                            loras[f'{lora_name}.bias_size'] = torch.tensor(diff.shape).to(torch.int16)
+                        del extract_a, extract_b, diff
+                    elif decompose_mode == 'full':
+                        loras[f'{lora_name}.diff'] = weight.detach().cpu().contiguous().half()
+                    else:
+                        raise NotImplementedError
+            elif name in temp_name:
+                weights = temp_name[name]
+                lora_name = prefix + '.' + name
+                lora_name = lora_name.replace('.', '_')
+                layer = module.__class__.__name__
+                
+                if layer in {'Linear', 'Conv2d'}:
+                    root_weight = module.weight
+                    if torch.allclose(root_weight, weights):
+                        continue
+                
+                if layer == 'Linear':
+                    weight, decompose_mode = extract_linear(
+                        (root_weight - weights),
+                        mode,
+                        linear_mode_param,
+                        device = extract_device,
+                    )
+                    if decompose_mode == 'low rank':
+                        extract_a, extract_b, diff = weight
+                elif layer == 'Conv2d':
+                    is_linear = (
+                        root_weight.shape[2] == 1
+                        and root_weight.shape[3] == 1
+                    )
+                    weight, decompose_mode = extract_conv(
+                        (root_weight - weights), 
+                        mode,
+                        linear_mode_param if is_linear else conv_mode_param,
+                        device = extract_device,
+                    )
+                    if decompose_mode == 'low rank':
+                        extract_a, extract_b, diff = weight
+                    if small_conv and not is_linear and decompose_mode == 'low rank':
+                        dim = extract_a.size(0)
+                        (extract_c, extract_a, _), _ = extract_conv(
+                            extract_a.transpose(0, 1), 
+                            'fixed', dim, 
+                            extract_device, True
+                        )
+                        extract_a = extract_a.transpose(0, 1)
+                        extract_c = extract_c.transpose(0, 1)
+                        loras[f'{lora_name}.lora_mid.weight'] = extract_c.detach().cpu().contiguous().half()
+                        diff = root_weight - torch.einsum(
+                            'i j k l, j r, p i -> p r k l', 
+                            extract_c, extract_a.flatten(1, -1), extract_b.flatten(1, -1)
+                        ).detach().cpu().contiguous()
+                        del extract_c
+                else:
+                    continue
+                if decompose_mode == 'low rank':
+                    loras[f'{lora_name}.lora_down.weight'] = extract_a.detach().cpu().contiguous().half()
+                    loras[f'{lora_name}.lora_up.weight'] = extract_b.detach().cpu().contiguous().half()
+                    loras[f'{lora_name}.alpha'] = torch.Tensor([extract_a.shape[0]]).half()
+                    if use_bias:
+                        diff = diff.detach().cpu().reshape(extract_b.size(0), -1)
+                        sparse_diff = make_sparse(diff, sparsity).to_sparse().coalesce()
+                        
+                        indices = sparse_diff.indices().to(torch.int16)
+                        values = sparse_diff.values().half()
+                        loras[f'{lora_name}.bias_indices'] = indices
+                        loras[f'{lora_name}.bias_values'] = values
+                        loras[f'{lora_name}.bias_size'] = torch.tensor(diff.shape).to(torch.int16)
+                    del extract_a, extract_b, diff
+                elif decompose_mode == 'full':
+                    loras[f'{lora_name}.diff'] = weight.detach().cpu().contiguous().half()
+                else:
+                    raise NotImplementedError
+        return loras
+    
+    text_encoder_loras = make_state_dict(
+        LORA_PREFIX_TEXT_ENCODER, 
+        base_model[0], db_model[0], 
+        TEXT_ENCODER_TARGET_REPLACE_MODULE
+    )
+    
+    unet_loras = make_state_dict(
+        LORA_PREFIX_UNET,
+        base_model[2], db_model[2], 
+        UNET_TARGET_REPLACE_MODULE,
+        UNET_TARGET_REPLACE_NAME
+    )
+    print(len(text_encoder_loras), len(unet_loras))
+    return text_encoder_loras|unet_loras
+
+
+def get_module(
+    lyco_state_dict: Dict,
+    lora_name
+):
+    if f'{lora_name}.lora_up.weight' in lyco_state_dict:
+        up = lyco_state_dict[f'{lora_name}.lora_up.weight']
+        down = lyco_state_dict[f'{lora_name}.lora_down.weight']
+        mid = lyco_state_dict.get(f'{lora_name}.lora_mid.weight', None)
+        alpha = lyco_state_dict.get(f'{lora_name}.alpha', None)
+        return 'locon', (up, down, mid, alpha)
+    elif f'{lora_name}.hada_w1_a' in lyco_state_dict:
+        w1a = lyco_state_dict[f'{lora_name}.hada_w1_a']
+        w1b = lyco_state_dict[f'{lora_name}.hada_w1_b']
+        w2a = lyco_state_dict[f'{lora_name}.hada_w2_a']
+        w2b = lyco_state_dict[f'{lora_name}.hada_w2_b']
+        t1 = lyco_state_dict.get(f'{lora_name}.hada_t1', None)
+        t2 = lyco_state_dict.get(f'{lora_name}.hada_t2', None)
+        alpha = lyco_state_dict.get(f'{lora_name}.alpha', None)
+        return 'hada', (w1a, w1b, w2a, w2b, t1, t2, alpha)
+    elif f'{lora_name}.weight' in lyco_state_dict:
+        weight = lyco_state_dict[f'{lora_name}.weight']
+        on_input = lyco_state_dict.get(f'{lora_name}.on_input', False)
+        return 'ia3', (weight, on_input)
+    elif (f'{lora_name}.lokr_w1' in lyco_state_dict
+          or f'{lora_name}.lokr_w1_a' in lyco_state_dict):
+        w1 = lyco_state_dict.get(f'{lora_name}.lokr_w1', None)
+        w1a = lyco_state_dict.get(f'{lora_name}.lokr_w1_a', None)
+        w1b = lyco_state_dict.get(f'{lora_name}.lokr_w1_b', None)
+        w2 = lyco_state_dict.get(f'{lora_name}.lokr_w2', None)
+        w2a = lyco_state_dict.get(f'{lora_name}.lokr_w2_a', None)
+        w2b = lyco_state_dict.get(f'{lora_name}.lokr_w2_b', None)
+        t1 = lyco_state_dict.get(f'{lora_name}.lokr_t1', None)
+        t2 = lyco_state_dict.get(f'{lora_name}.lokr_t2', None)
+        alpha = lyco_state_dict.get(f'{lora_name}.alpha', None)
+        return 'kron', (w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha)
+    elif f'{lora_name}.diff' in lyco_state_dict:
+        return 'full', lyco_state_dict[f'{lora_name}.diff']
+    else:
+        return 'None', ()
+
+
+def cp_weight_from_conv(
+    up, down, mid
+):
+    up = up.reshape(up.size(0), up.size(1))
+    down = down.reshape(down.size(0), down.size(1))
+    return torch.einsum('m n w h, i m, n j -> i j w h', mid, up, down)
+
+def cp_weight(
+    wa, wb, t
+):
+    temp = torch.einsum('i j k l, j r -> i r k l', t, wb)
+    return torch.einsum('i j k l, i r -> r j k l', temp, wa)
+
+
+@torch.no_grad()
+def rebuild_weight(module_type, params, orig_weight, scale=1):
+    if orig_weight is None:
+        return orig_weight
+    merged = orig_weight
+    if module_type == 'locon':
+        up, down, mid, alpha = params
+        if alpha is not None:
+            scale *= alpha/up.size(1)
+        if mid is not None:
+            rebuild = cp_weight_from_conv(up, down, mid)
+        else:
+            rebuild = up.reshape(up.size(0),-1) @ down.reshape(down.size(0), -1)
+        merged = orig_weight + rebuild.reshape(orig_weight.shape) * scale
+        del up, down, mid, alpha, params, rebuild
+    elif module_type == 'hada':
+        w1a, w1b, w2a, w2b, t1, t2, alpha = params
+        if alpha is not None:
+            scale *= alpha / w1b.size(0)
+        if t1 is not None:
+            rebuild1 = cp_weight(w1a, w1b, t1)
+        else:
+            rebuild1 = w1a @ w1b
+        if t2 is not None:
+            rebuild2 = cp_weight(w2a, w2b, t2)
+        else:
+            rebuild2 = w2a @ w2b
+        rebuild = (rebuild1 * rebuild2).reshape(orig_weight.shape)
+        merged = orig_weight + rebuild * scale
+        del w1a, w1b, w2a, w2b, t1, t2, alpha, params, rebuild, rebuild1, rebuild2
+    elif module_type == 'ia3':
+        weight, on_input = params
+        if not on_input:
+            weight = weight.reshape(-1, 1)
+        merged = orig_weight + weight * orig_weight * scale
+        del weight, on_input, params
+    elif module_type == 'kron':
+        w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha = params
+        if alpha is not None and (w1b is not None or w2b is not None):
+            scale *= alpha / (w1b.size(0) if w1b else w2b.size(0))
+        if w1a is not None and w1b is not None:
+            if t1:
+                w1 = cp_weight(w1a, w1b, t1)
+            else:
+                w1 = w1a @ w1b
+        if w2a is not None and w2b is not None:
+            if t2:
+                w2 = cp_weight(w2a, w2b, t2)
+            else:
+                w2 = w2a @ w2b
+        rebuild = torch.kron(w1, w2).reshape(orig_weight.shape) 
+        merged = orig_weight + rebuild* scale
+        del w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha, params, rebuild
+    elif module_type == 'full':
+        rebuild = params.reshape(orig_weight.shape) 
+        merged = orig_weight + rebuild * scale
+        del params, rebuild
+    
+    return merged
+
+
+def merge(
+    base_model,
+    lyco_state_dict,
+    scale: float = 1.0,
+    device = 'cpu'
+):
+    UNET_TARGET_REPLACE_MODULE = [
+        "Transformer2DModel", 
+        "Attention", 
+        "ResnetBlock2D", 
+        "Downsample2D", 
+        "Upsample2D"
+    ]
+    UNET_TARGET_REPLACE_NAME = [
+        "conv_in",
+        "conv_out",
+        "time_embedding.linear_1",
+        "time_embedding.linear_2",
+    ]
+    TEXT_ENCODER_TARGET_REPLACE_MODULE = ["CLIPAttention", "CLIPMLP"]
+    LORA_PREFIX_UNET = 'lora_unet'
+    LORA_PREFIX_TEXT_ENCODER = 'lora_te'
+    merged = 0
+    def merge_state_dict(
+        prefix, 
+        root_module: torch.nn.Module,
+        lyco_state_dict: Dict[str,torch.Tensor],
+        target_replace_modules,
+        target_replace_names = []
+    ):
+        nonlocal merged
+        for name, module in tqdm(list(root_module.named_modules()), desc=f'Merging {prefix}'):
+            if module.__class__.__name__ in target_replace_modules:
+                for child_name, child_module in module.named_modules():
+                    if child_module.__class__.__name__ not in {'Linear', 'Conv2d'}:
+                        continue
+                    lora_name = prefix + '.' + name + '.' + child_name
+                    lora_name = lora_name.replace('.', '_')
+                    
+                    result = rebuild_weight(*get_module(
+                        lyco_state_dict, lora_name
+                    ), getattr(child_module, 'weight'), scale)
+                    if result is not None:
+                        merged += 1
+                        child_module.requires_grad_(False)
+                        child_module.weight.copy_(result)
+            elif name in target_replace_names:
+                lora_name = prefix + '.' + name
+                lora_name = lora_name.replace('.', '_')
+                    
+                result = rebuild_weight(*get_module(
+                    lyco_state_dict, lora_name
+                ), getattr(module, 'weight'), scale)
+                if result is not None:
+                    merged += 1
+                    module.requires_grad_(False)
+                    module.weight.copy_(result)
+    
+    if device == 'cpu':
+        for k, v in tqdm(list(lyco_state_dict.items()), desc='Converting Dtype'):
+            lyco_state_dict[k] = v.float()
+    
+    merge_state_dict(
+        LORA_PREFIX_TEXT_ENCODER,
+        base_model[0],
+        lyco_state_dict,
+        TEXT_ENCODER_TARGET_REPLACE_MODULE,
+        UNET_TARGET_REPLACE_NAME
+    )
+    merge_state_dict(
+        LORA_PREFIX_UNET,
+        base_model[2],
+        lyco_state_dict,
+        UNET_TARGET_REPLACE_MODULE,
+        UNET_TARGET_REPLACE_NAME
+    )
+    print(f'{merged} Modules been merged')
```

