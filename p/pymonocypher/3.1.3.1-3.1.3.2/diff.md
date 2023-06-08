# Comparing `tmp/pymonocypher-3.1.3.1.tar.gz` & `tmp/pymonocypher-3.1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymonocypher-3.1.3.1.tar", last modified: Wed Nov 30 15:44:40 2022, max compression
+gzip compressed data, was "pymonocypher-3.1.3.2.tar", last modified: Thu Jun  8 11:42:35 2023, max compression
```

## Comparing `pymonocypher-3.1.3.1.tar` & `pymonocypher-3.1.3.2.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-11-30 15:44:40.640641 pymonocypher-3.1.3.1/
--rw-rw-rw-   0        0        0     9468 2020-05-11 12:46:17.000000 pymonocypher-3.1.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0       62 2018-10-09 23:57:56.000000 pymonocypher-3.1.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2060 2022-11-30 15:44:40.640641 pymonocypher-3.1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      966 2019-09-28 15:29:44.000000 pymonocypher-3.1.3.1/README.md
--rw-rw-rw-   0        0        0   456786 2022-11-30 15:44:13.000000 pymonocypher-3.1.3.1/c_monocypher.c
--rw-rw-rw-   0        0        0   107925 2020-04-22 00:00:00.000000 pymonocypher-3.1.3.1/monocypher.c
--rw-rw-rw-   0        0        0    15162 2020-04-22 00:00:00.000000 pymonocypher-3.1.3.1/monocypher.h
-drwxrwxrwx   0        0        0        0 2022-11-30 15:44:40.638629 pymonocypher-3.1.3.1/pymonocypher.egg-info/
--rw-rw-rw-   0        0        0     2060 2022-11-30 15:44:40.000000 pymonocypher-3.1.3.1/pymonocypher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2022-11-30 15:44:40.000000 pymonocypher-3.1.3.1/pymonocypher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-30 15:44:40.000000 pymonocypher-3.1.3.1/pymonocypher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2022-11-30 15:44:40.000000 pymonocypher-3.1.3.1/pymonocypher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      796 2022-11-30 15:29:07.000000 pymonocypher-3.1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      116 2022-11-30 15:44:40.641628 pymonocypher-3.1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2523 2022-11-30 15:29:46.000000 pymonocypher-3.1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-30 15:44:40.639628 pymonocypher-3.1.3.1/test/
--rw-rw-rw-   0        0        0     5026 2020-05-11 12:46:17.000000 pymonocypher-3.1.3.1/test/test_monocypher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:42:35.989597 pymonocypher-3.1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 2023-06-08 11:42:17.000000 pymonocypher-3.1.3.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-08 11:42:17.000000 pymonocypher-3.1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-08 11:42:35.989597 pymonocypher-3.1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-08 11:42:17.000000 pymonocypher-3.1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   516600 2023-06-08 11:42:35.000000 pymonocypher-3.1.3.2/c_monocypher.c
+-rw-r--r--   0 runner    (1001) docker     (123)   107925 2023-06-08 11:42:17.000000 pymonocypher-3.1.3.2/monocypher.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15162 2023-06-08 11:42:17.000000 pymonocypher-3.1.3.2/monocypher.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:42:35.985597 pymonocypher-3.1.3.2/pymonocypher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-08 11:42:35.000000 pymonocypher-3.1.3.2/pymonocypher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-08 11:42:35.000000 pymonocypher-3.1.3.2/pymonocypher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:42:35.000000 pymonocypher-3.1.3.2/pymonocypher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 11:42:35.000000 pymonocypher-3.1.3.2/pymonocypher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 11:42:35.000000 pymonocypher-3.1.3.2/pymonocypher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-08 11:42:17.000000 pymonocypher-3.1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 11:42:35.989597 pymonocypher-3.1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-08 11:42:17.000000 pymonocypher-3.1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:42:35.989597 pymonocypher-3.1.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:42:17.000000 pymonocypher-3.1.3.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1873923 2023-06-08 11:42:17.000000 pymonocypher-3.1.3.2/test/blake2-kat.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-08 11:42:17.000000 pymonocypher-3.1.3.2/test/test_monocypher.py
```

### Comparing `pymonocypher-3.1.3.1/LICENSE.txt` & `pymonocypher-3.1.3.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-Monocypher as a whole is dual-licensed.  Choose whichever licence you
-want from the two licences listed below.
-
-The first licence is a regular 2-clause BSD licence.  The second licence
-is the CC-0 from Creative Commons. It is intended to release Monocypher
-to the public domain.  The BSD licence serves as a fallback option.
-
-See the individual files for specific information about who contributed
-to what file during which years.  See below for special notes.
-
-Licence 1 (2-clause BSD)
-------------------------
-
-Copyright (c) 2017-2020, Loup Vaillant
-Copyright (c) 2017-2019, Michael Savage
-Copyright (c) 2017-2020, Fabio Scotoni
-Copyright (c) 2018-2020, Matt Liberty
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are
-met:
-
-1. Redistributions of source code must retain the above copyright
-   notice, this list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright
-   notice, this list of conditions and the following disclaimer in the
-   documentation and/or other materials provided with the
-   distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
-SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
-LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
-THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-
-Licence 2 (CC-0)
-----------------
-
-> CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
-> LEGAL SERVICES. DISTRIBUTION OF THIS DOCUMENT DOES NOT CREATE AN
-> ATTORNEY-CLIENT RELATIONSHIP. CREATIVE COMMONS PROVIDES THIS
-> INFORMATION ON AN "AS-IS" BASIS. CREATIVE COMMONS MAKES NO WARRANTIES
-> REGARDING THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS
-> PROVIDED HEREUNDER, AND DISCLAIMS LIABILITY FOR DAMAGES RESULTING FROM
-> THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS PROVIDED
-> HEREUNDER.
-
-### Statement of Purpose
-
-The laws of most jurisdictions throughout the world automatically confer
-exclusive Copyright and Related Rights (defined below) upon the creator
-and subsequent owner(s) (each and all, an "owner") of an original work
-of authorship and/or a database (each, a "Work").
-
-Certain owners wish to permanently relinquish those rights to a Work for
-the purpose of contributing to a commons of creative, cultural and
-scientific works ("Commons") that the public can reliably and without
-fear of later claims of infringement build upon, modify, incorporate in
-other works, reuse and redistribute as freely as possible in any form
-whatsoever and for any purposes, including without limitation commercial
-purposes. These owners may contribute to the Commons to promote the
-ideal of a free culture and the further production of creative, cultural
-and scientific works, or to gain reputation or greater distribution for
-their Work in part through the use and efforts of others.
-
-For these and/or other purposes and motivations, and without any
-expectation of additional consideration or compensation, the person
-associating CC0 with a Work (the "Affirmer"), to the extent that he or
-she is an owner of Copyright and Related Rights in the Work, voluntarily
-elects to apply CC0 to the Work and publicly distribute the Work under
-its terms, with knowledge of his or her Copyright and Related Rights in
-the Work and the meaning and intended legal effect of CC0 on those
-rights.
-
-1. **Copyright and Related Rights.** A Work made available under CC0 may
-   be protected by copyright and related or neighboring rights
-   ("Copyright and Related Rights"). Copyright and Related Rights
-   include, but are not limited to, the following:
-
-   - the right to reproduce, adapt, distribute, perform, display,
-     communicate, and translate a Work;
-   - moral rights retained by the original author(s) and/or
-     performer(s); publicity and privacy rights pertaining to a person's
-     image or likeness depicted in a Work;
-   - rights protecting against unfair competition in regards to a Work,
-     subject to the limitations in paragraph 4(a), below;
-   - rights protecting the extraction, dissemination, use and reuse of
-     data in a Work;
-   - database rights (such as those arising under Directive 96/9/EC of
-     the European Parliament and of the Council of 11 March 1996 on the
-     legal protection of databases, and under any national
-     implementation thereof, including any amended or successor version
-     of such directive); and
-   - other similar, equivalent or corresponding rights throughout the
-     world based on applicable law or treaty, and any national
-     implementations thereof.
-
-2. **Waiver.** To the greatest extent permitted by, but not in
-   contravention of, applicable law, Affirmer hereby overtly, fully,
-   permanently, irrevocably and unconditionally waives, abandons, and
-   surrenders all of Affirmer's Copyright and Related Rights and
-   associated claims and causes of action, whether now known or unknown
-   (including existing as well as future claims and causes of action),
-   in the Work (i) in all territories worldwide, (ii) for the maximum
-   duration provided by applicable law or treaty (including future time
-   extensions), (iii) in any current or future medium and for any number
-   of copies, and (iv) for any purpose whatsoever, including without
-   limitation commercial, advertising or promotional purposes (the
-   "Waiver"). Affirmer makes the Waiver for the benefit of each member
-   of the public at large and to the detriment of Affirmer's heirs and
-   successors, fully intending that such Waiver shall not be subject to
-   revocation, rescission, cancellation, termination, or any other legal
-   or equitable action to disrupt the quiet enjoyment of the Work by the
-   public as contemplated by Affirmer's express Statement of Purpose.
-
-3. **Public License Fallback.** Should any part of the Waiver for any
-   reason be judged legally invalid or ineffective under applicable law,
-   then the Waiver shall be preserved to the maximum extent permitted
-   taking into account Affirmer's express Statement of Purpose. In
-   addition, to the extent the Waiver is so judged Affirmer hereby
-   grants to each affected person a royalty-free, non transferable, non
-   sublicensable, non exclusive, irrevocable and unconditional license
-   to exercise Affirmer's Copyright and Related Rights in the Work (i)
-   in all territories worldwide, (ii) for the maximum duration provided
-   by applicable law or treaty (including future time extensions), (iii)
-   in any current or future medium and for any number of copies, and
-   (iv) for any purpose whatsoever, including without limitation
-   commercial, advertising or promotional purposes (the "License"). The
-   License shall be deemed effective as of the date CC0 was applied by
-   Affirmer to the Work. Should any part of the License for any reason
-   be judged legally invalid or ineffective under applicable law, such
-   partial invalidity or ineffectiveness shall not invalidate the
-   remainder of the License, and in such case Affirmer hereby affirms
-   that he or she will not (i) exercise any of his or her remaining
-   Copyright and Related Rights in the Work or (ii) assert any
-   associated claims and causes of action with respect to the Work, in
-   either case contrary to Affirmer's express Statement of Purpose.
-
-4. **Limitations and Disclaimers.**
-
-   - No trademark or patent rights held by Affirmer are waived,
-     abandoned, surrendered, licensed or otherwise affected by this
-     document.
-   - Affirmer offers the Work as-is and makes no representations or
-     warranties of any kind concerning the Work, express, implied,
-     statutory or otherwise, including without limitation warranties of
-     title, merchantability, fitness for a particular purpose, non
-     infringement, or the absence of latent or other defects, accuracy,
-     or the present or absence of errors, whether or not discoverable,
-     all to the greatest extent permissible under applicable law.
-   - Affirmer disclaims responsibility for clearing rights of other
-     persons that may apply to the Work or any use thereof, including
-     without limitation any person's Copyright and Related Rights in the
-     Work. Further, Affirmer disclaims responsibility for obtaining any
-     necessary consents, permissions or other rights required for any
-     use of the Work.
-   - Affirmer understands and acknowledges that Creative Commons is not
-     a party to this document and has no duty or obligation with respect
-     to this CC0 or use of the Work.
-
-Special notes
--------------
-
-The files in `tests/externals/` were placed in the public domain by
-their respective authors.  See the `AUTHORS.md` files in each directory.
+Monocypher as a whole is dual-licensed.  Choose whichever licence you
+want from the two licences listed below.
+
+The first licence is a regular 2-clause BSD licence.  The second licence
+is the CC-0 from Creative Commons. It is intended to release Monocypher
+to the public domain.  The BSD licence serves as a fallback option.
+
+See the individual files for specific information about who contributed
+to what file during which years.  See below for special notes.
+
+Licence 1 (2-clause BSD)
+------------------------
+
+Copyright (c) 2017-2020, Loup Vaillant
+Copyright (c) 2017-2019, Michael Savage
+Copyright (c) 2017-2020, Fabio Scotoni
+Copyright (c) 2018-2020, Matt Liberty
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are
+met:
+
+1. Redistributions of source code must retain the above copyright
+   notice, this list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright
+   notice, this list of conditions and the following disclaimer in the
+   documentation and/or other materials provided with the
+   distribution.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
+"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
+HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
+LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
+THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+
+Licence 2 (CC-0)
+----------------
+
+> CREATIVE COMMONS CORPORATION IS NOT A LAW FIRM AND DOES NOT PROVIDE
+> LEGAL SERVICES. DISTRIBUTION OF THIS DOCUMENT DOES NOT CREATE AN
+> ATTORNEY-CLIENT RELATIONSHIP. CREATIVE COMMONS PROVIDES THIS
+> INFORMATION ON AN "AS-IS" BASIS. CREATIVE COMMONS MAKES NO WARRANTIES
+> REGARDING THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS
+> PROVIDED HEREUNDER, AND DISCLAIMS LIABILITY FOR DAMAGES RESULTING FROM
+> THE USE OF THIS DOCUMENT OR THE INFORMATION OR WORKS PROVIDED
+> HEREUNDER.
+
+### Statement of Purpose
+
+The laws of most jurisdictions throughout the world automatically confer
+exclusive Copyright and Related Rights (defined below) upon the creator
+and subsequent owner(s) (each and all, an "owner") of an original work
+of authorship and/or a database (each, a "Work").
+
+Certain owners wish to permanently relinquish those rights to a Work for
+the purpose of contributing to a commons of creative, cultural and
+scientific works ("Commons") that the public can reliably and without
+fear of later claims of infringement build upon, modify, incorporate in
+other works, reuse and redistribute as freely as possible in any form
+whatsoever and for any purposes, including without limitation commercial
+purposes. These owners may contribute to the Commons to promote the
+ideal of a free culture and the further production of creative, cultural
+and scientific works, or to gain reputation or greater distribution for
+their Work in part through the use and efforts of others.
+
+For these and/or other purposes and motivations, and without any
+expectation of additional consideration or compensation, the person
+associating CC0 with a Work (the "Affirmer"), to the extent that he or
+she is an owner of Copyright and Related Rights in the Work, voluntarily
+elects to apply CC0 to the Work and publicly distribute the Work under
+its terms, with knowledge of his or her Copyright and Related Rights in
+the Work and the meaning and intended legal effect of CC0 on those
+rights.
+
+1. **Copyright and Related Rights.** A Work made available under CC0 may
+   be protected by copyright and related or neighboring rights
+   ("Copyright and Related Rights"). Copyright and Related Rights
+   include, but are not limited to, the following:
+
+   - the right to reproduce, adapt, distribute, perform, display,
+     communicate, and translate a Work;
+   - moral rights retained by the original author(s) and/or
+     performer(s); publicity and privacy rights pertaining to a person's
+     image or likeness depicted in a Work;
+   - rights protecting against unfair competition in regards to a Work,
+     subject to the limitations in paragraph 4(a), below;
+   - rights protecting the extraction, dissemination, use and reuse of
+     data in a Work;
+   - database rights (such as those arising under Directive 96/9/EC of
+     the European Parliament and of the Council of 11 March 1996 on the
+     legal protection of databases, and under any national
+     implementation thereof, including any amended or successor version
+     of such directive); and
+   - other similar, equivalent or corresponding rights throughout the
+     world based on applicable law or treaty, and any national
+     implementations thereof.
+
+2. **Waiver.** To the greatest extent permitted by, but not in
+   contravention of, applicable law, Affirmer hereby overtly, fully,
+   permanently, irrevocably and unconditionally waives, abandons, and
+   surrenders all of Affirmer's Copyright and Related Rights and
+   associated claims and causes of action, whether now known or unknown
+   (including existing as well as future claims and causes of action),
+   in the Work (i) in all territories worldwide, (ii) for the maximum
+   duration provided by applicable law or treaty (including future time
+   extensions), (iii) in any current or future medium and for any number
+   of copies, and (iv) for any purpose whatsoever, including without
+   limitation commercial, advertising or promotional purposes (the
+   "Waiver"). Affirmer makes the Waiver for the benefit of each member
+   of the public at large and to the detriment of Affirmer's heirs and
+   successors, fully intending that such Waiver shall not be subject to
+   revocation, rescission, cancellation, termination, or any other legal
+   or equitable action to disrupt the quiet enjoyment of the Work by the
+   public as contemplated by Affirmer's express Statement of Purpose.
+
+3. **Public License Fallback.** Should any part of the Waiver for any
+   reason be judged legally invalid or ineffective under applicable law,
+   then the Waiver shall be preserved to the maximum extent permitted
+   taking into account Affirmer's express Statement of Purpose. In
+   addition, to the extent the Waiver is so judged Affirmer hereby
+   grants to each affected person a royalty-free, non transferable, non
+   sublicensable, non exclusive, irrevocable and unconditional license
+   to exercise Affirmer's Copyright and Related Rights in the Work (i)
+   in all territories worldwide, (ii) for the maximum duration provided
+   by applicable law or treaty (including future time extensions), (iii)
+   in any current or future medium and for any number of copies, and
+   (iv) for any purpose whatsoever, including without limitation
+   commercial, advertising or promotional purposes (the "License"). The
+   License shall be deemed effective as of the date CC0 was applied by
+   Affirmer to the Work. Should any part of the License for any reason
+   be judged legally invalid or ineffective under applicable law, such
+   partial invalidity or ineffectiveness shall not invalidate the
+   remainder of the License, and in such case Affirmer hereby affirms
+   that he or she will not (i) exercise any of his or her remaining
+   Copyright and Related Rights in the Work or (ii) assert any
+   associated claims and causes of action with respect to the Work, in
+   either case contrary to Affirmer's express Statement of Purpose.
+
+4. **Limitations and Disclaimers.**
+
+   - No trademark or patent rights held by Affirmer are waived,
+     abandoned, surrendered, licensed or otherwise affected by this
+     document.
+   - Affirmer offers the Work as-is and makes no representations or
+     warranties of any kind concerning the Work, express, implied,
+     statutory or otherwise, including without limitation warranties of
+     title, merchantability, fitness for a particular purpose, non
+     infringement, or the absence of latent or other defects, accuracy,
+     or the present or absence of errors, whether or not discoverable,
+     all to the greatest extent permissible under applicable law.
+   - Affirmer disclaims responsibility for clearing rights of other
+     persons that may apply to the Work or any use thereof, including
+     without limitation any person's Copyright and Related Rights in the
+     Work. Further, Affirmer disclaims responsibility for obtaining any
+     necessary consents, permissions or other rights required for any
+     use of the Work.
+   - Affirmer understands and acknowledges that Creative Commons is not
+     a party to this document and has no duty or obligation with respect
+     to this CC0 or use of the Work.
+
+Special notes
+-------------
+
+The files in `tests/externals/` were placed in the public domain by
+their respective authors.  See the `AUTHORS.md` files in each directory.
```

### Comparing `pymonocypher-3.1.3.1/PKG-INFO` & `pymonocypher-3.1.3.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-Metadata-Version: 2.1
-Name: pymonocypher
-Version: 3.1.3.1
-Summary: Python ctypes bindings to the Monocypher library
-Home-page: https://github.com/jetperch/pymonocypher
-Author: Jetperch LLC
-Author-email: joulescope-dev@jetperch.com
-License: BSD 2-clause
-Project-URL: Bug Reports, https://github.com/jetperch/pymonocypher/issues
-Project-URL: Source, https://github.com/jetperch/pymonocypher/
-Keywords: cryto cryptography monocypher chacha blake2b 25519
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Natural Language :: English
-Classifier: Topic :: Security :: Cryptography
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: C
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
-# pymonocypher
-
-This python package uses cython to wrap the Monocypher C library. 
-Monocypher is an easy to use, easy to deploy, auditable crypto library
-written in portable C.  
-
-Normal Python installations have access to a wide
-selection of quality crypto libraries.  This python binding is intended to
-communicate with other implementations that do use the Monocypher library.
-A typical application is to communicate with a microcontroller that 
-uses Monocypher.
-
-*   pymonocypher [Source code](https://github.com/jetperch/pymonocypher)
-*   Monocypher [official site](https://monocypher.org/)
-
-The Python binding API mirrors the underlying C API, but with 
-simplifications to only pass bytes objects, not uint8_t * and length.
-
-
-## Installation
-
-You can install directly from pypi:
-
-    pip install pymonocypher
-    
-You can then use pymonocypher:
-
-    python
-    >>> import monocypher
-    >>> monocypher.blake2b(b'hello world')
-
+Metadata-Version: 2.1
+Name: pymonocypher
+Version: 3.1.3.2
+Summary: Python ctypes bindings to the Monocypher library
+Home-page: https://github.com/jetperch/pymonocypher
+Author: Jetperch LLC
+Author-email: joulescope-dev@jetperch.com
+License: BSD 2-clause
+Project-URL: Bug Reports, https://github.com/jetperch/pymonocypher/issues
+Project-URL: Source, https://github.com/jetperch/pymonocypher/
+Keywords: cryto cryptography monocypher chacha blake2b 25519
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Natural Language :: English
+Classifier: Topic :: Security :: Cryptography
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: C
+Requires-Python: ~=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# pymonocypher
+
+This python package uses cython to wrap the Monocypher C library. 
+Monocypher is an easy to use, easy to deploy, auditable crypto library
+written in portable C.  
+
+Normal Python installations have access to a wide
+selection of quality crypto libraries.  This python binding is intended to
+communicate with other implementations that do use the Monocypher library.
+A typical application is to communicate with a microcontroller that 
+uses Monocypher.
+
+*   pymonocypher [Source code](https://github.com/jetperch/pymonocypher)
+*   Monocypher [official site](https://monocypher.org/)
+
+The Python binding API mirrors the underlying C API, but with 
+simplifications to only pass bytes objects, not uint8_t * and length.
+
+
+## Installation
+
+You can install directly from pypi:
+
+    pip install pymonocypher
+    
+You can then use pymonocypher:
+
+    python
+    >>> import monocypher
+    >>> monocypher.blake2b(b'hello world')
+
```

### Comparing `pymonocypher-3.1.3.1/README.md` & `pymonocypher-3.1.3.2/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-
-# pymonocypher
-
-This python package uses cython to wrap the Monocypher C library. 
-Monocypher is an easy to use, easy to deploy, auditable crypto library
-written in portable C.  
-
-Normal Python installations have access to a wide
-selection of quality crypto libraries.  This python binding is intended to
-communicate with other implementations that do use the Monocypher library.
-A typical application is to communicate with a microcontroller that 
-uses Monocypher.
-
-*   pymonocypher [Source code](https://github.com/jetperch/pymonocypher)
-*   Monocypher [official site](https://monocypher.org/)
-
-The Python binding API mirrors the underlying C API, but with 
-simplifications to only pass bytes objects, not uint8_t * and length.
-
-
-## Installation
-
-You can install directly from pypi:
-
-    pip install pymonocypher
-    
-You can then use pymonocypher:
-
-    python
-    >>> import monocypher
-    >>> monocypher.blake2b(b'hello world')
-
+
+# pymonocypher
+
+This python package uses cython to wrap the Monocypher C library. 
+Monocypher is an easy to use, easy to deploy, auditable crypto library
+written in portable C.  
+
+Normal Python installations have access to a wide
+selection of quality crypto libraries.  This python binding is intended to
+communicate with other implementations that do use the Monocypher library.
+A typical application is to communicate with a microcontroller that 
+uses Monocypher.
+
+*   pymonocypher [Source code](https://github.com/jetperch/pymonocypher)
+*   Monocypher [official site](https://monocypher.org/)
+
+The Python binding API mirrors the underlying C API, but with 
+simplifications to only pass bytes objects, not uint8_t * and length.
+
+
+## Installation
+
+You can install directly from pypi:
+
+    pip install pymonocypher
+    
+You can then use pymonocypher:
+
+    python
+    >>> import monocypher
+    >>> monocypher.blake2b(b'hello world')
+
```

### Comparing `pymonocypher-3.1.3.1/c_monocypher.c` & `pymonocypher-3.1.3.2/c_monocypher.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.35 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "monocypher.h"
         ],
@@ -27,16 +27,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_35"
+#define CYTHON_HEX_VERSION 0x001D23F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -96,24 +96,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
   #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -221,15 +225,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -260,15 +264,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -570,35 +574,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1268,26 +1272,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1303,14 +1307,36 @@
 /* PyObjectCallNoArg.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 #else
 #define __Pyx_PyObject_CallNoArg(func) __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL)
 #endif
 
+/* ArgTypeTest.proto */
+#define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
+    ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
+        __Pyx__ArgTypeTest(obj, type, name, exact))
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
+
+/* GCCDiagnostics.proto */
+#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
+#define __Pyx_HAS_GCC_DIAGNOSTIC
+#endif
+
+/* BuildPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
+                                                int prepend_sign, char padding_char);
+
+/* CIntToPyUnicode.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_Py_ssize_t(Py_ssize_t value, Py_ssize_t width, char padding_char, char format_char);
+
+/* JoinPyUnicode.proto */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      Py_UCS4 max_char);
+
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
 #define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
@@ -1423,31 +1449,29 @@
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
-/* GCCDiagnostics.proto */
-#if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE size_t __Pyx_PyInt_As_size_t(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE uint32_t __Pyx_PyInt_As_uint32_t(PyObject *);
 
+/* CIntFromPy.proto */
+static CYTHON_INLINE uint8_t __Pyx_PyInt_As_uint8_t(PyObject *);
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
 /* FastTypeChecks.proto */
@@ -1490,14 +1514,15 @@
 /* Implementation of 'monocypher' */
 static PyObject *__pyx_builtin_ValueError;
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_DeprecationWarning;
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_p[] = "p";
+static const char __pyx_k_32[] = " != 32";
 static const char __pyx_k__3[] = "";
 static const char __pyx_k_ad[] = "ad";
 static const char __pyx_k_kp[] = "kp";
 static const char __pyx_k_os[] = "os";
 static const char __pyx_k_rv[] = "rv";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_mac[] = "mac";
@@ -1506,43 +1531,48 @@
 static const char __pyx_k_url[] = "__url__";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_hash[] = "hash";
 static const char __pyx_k_lock[] = "lock";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_salt[] = "salt";
+static const char __pyx_k_seed[] = "seed";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_warn[] = "warn";
 static const char __pyx_k_wipe[] = "wipe";
 static const char __pyx_k_wrap[] = "wrap";
+static const char __pyx_k_curve[] = "curve";
 static const char __pyx_k_nonce[] = "nonce";
 static const char __pyx_k_title[] = "__title__";
+static const char __pyx_k_tweak[] = "tweak";
 static const char __pyx_k_utf_8[] = "utf-8";
 static const char __pyx_k_author[] = "__author__";
 static const char __pyx_k_encode[] = "encode";
+static const char __pyx_k_hidden[] = "hidden";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_length[] = "length";
 static const char __pyx_k_method[] = "method";
 static const char __pyx_k_public[] = "public";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_result[] = "result";
 static const char __pyx_k_secret[] = "secret";
 static const char __pyx_k_unlock[] = "unlock";
-static const char __pyx_k_3_1_3_1[] = "3.1.3.1";
+static const char __pyx_k_3_1_3_2[] = "3.1.3.2";
 static const char __pyx_k_Blake2b[] = "Blake2b";
 static const char __pyx_k_blake2b[] = "blake2b";
 static const char __pyx_k_default[] = "default";
 static const char __pyx_k_license[] = "__license__";
 static const char __pyx_k_message[] = "message";
 static const char __pyx_k_secrets[] = "secrets";
 static const char __pyx_k_version[] = "__version__";
 static const char __pyx_k_binascii[] = "binascii";
 static const char __pyx_k_chacha20[] = "chacha20";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_password[] = "password";
+static const char __pyx_k_randbits[] = "randbits";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_warnings[] = "warnings";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_copyright[] = "__copyright__";
 static const char __pyx_k_hash_size[] = "hash_size";
 static const char __pyx_k_nb_blocks[] = "nb_blocks";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
@@ -1561,50 +1591,61 @@
 static const char __pyx_k_BSD_2_clause[] = "BSD 2-clause";
 static const char __pyx_k_Jetperch_LLC[] = "Jetperch LLC";
 static const char __pyx_k_author_email[] = "__author_email__";
 static const char __pyx_k_generate_key[] = "generate_key";
 static const char __pyx_k_key_exchange[] = "key_exchange";
 static const char __pyx_k_pymonocypher[] = "pymonocypher";
 static const char __pyx_k_stringsource[] = "stringsource";
+static const char __pyx_k_elligator_map[] = "elligator_map";
+static const char __pyx_k_elligator_rev[] = "elligator_rev";
 static const char __pyx_k_nb_iterations[] = "nb_iterations";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
 static const char __pyx_k_signature_sign[] = "signature_sign";
 static const char __pyx_k_SignatureVerify[] = "SignatureVerify";
 static const char __pyx_k_associated_data[] = "associated_data";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_signature_check[] = "signature_check";
 static const char __pyx_k_your_secret_key[] = "your_secret_key";
 static const char __pyx_k_c_monocypher_pyx[] = "c_monocypher.pyx";
 static const char __pyx_k_their_public_key[] = "their_public_key";
 static const char __pyx_k_generate_key_pair[] = "generate_key_pair";
 static const char __pyx_k_DeprecationWarning[] = "DeprecationWarning";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_elligator_key_pair[] = "elligator_key_pair";
 static const char __pyx_k_public_key_compute[] = "public_key_compute";
+static const char __pyx_k_Invalid_seed_length[] = "Invalid seed length ";
+static const char __pyx_k_Invalid_curve_length[] = "Invalid curve length ";
 static const char __pyx_k_invalid_nonce_length[] = "invalid nonce length";
 static const char __pyx_k_unsupported_method_s[] = "unsupported method: %s";
+static const char __pyx_k_Invalid_hidden_length[] = "Invalid hidden length ";
 static const char __pyx_k_generate_signing_key_pair[] = "generate_signing_key_pair";
 static const char __pyx_k_Pyx_CFunc_void____uint8__t[] = "__Pyx_CFunc_void____uint8__t________const__uint8__t_______to_py.<locals>.wrap";
 static const char __pyx_k_compute_signing_public_key[] = "compute_signing_public_key";
 static const char __pyx_k_joulescope_dev_jetperch_com[] = "joulescope-dev@jetperch.com";
 static const char __pyx_k_Pyx_CFunc_int____const__uint8[] = "__Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py.<locals>.wrap";
 static const char __pyx_k_generate_key_exchange_key_pair[] = "generate_key_exchange_key_pair";
 static const char __pyx_k_Monocypher_library_Python_bindi[] = "\nMonocypher library Python bindings.\n\nMonocypher is an easy to use, easy to deploy, auditable crypto library\nwritten in portable C.\n";
 static const char __pyx_k_Pickling_of_struct_members_such[] = "Pickling of struct members such as self._ctx must be explicitly requested with @auto_pickle(True)";
 static const char __pyx_k_compute_key_exchange_public_key[] = "compute_key_exchange_public_key";
 static const char __pyx_k_deprecated_use_generate_signing[] = "deprecated: use generate_signing_key_pair";
 static const char __pyx_k_Copyright_2018_2022_Jetperch_LLC[] = "Copyright 2018-2022 Jetperch LLC";
 static const char __pyx_k_Python_ctypes_bindings_to_the_Mo[] = "Python ctypes bindings to the Monocypher library";
+static const char __pyx_k_curve_point_is_unsuitable_for_hi[] = "curve point is unsuitable for hiding";
 static const char __pyx_k_deprecated_use_compute_signing_p[] = "deprecated: use compute_signing_public_key";
 static const char __pyx_k_https_github_com_jetperch_pymono[] = "https://github.com/jetperch/pymonocypher";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
-static PyObject *__pyx_kp_u_3_1_3_1;
+static PyObject *__pyx_kp_u_32;
+static PyObject *__pyx_kp_u_3_1_3_2;
 static PyObject *__pyx_kp_u_BSD_2_clause;
 static PyObject *__pyx_n_s_Blake2b;
 static PyObject *__pyx_kp_u_Copyright_2018_2022_Jetperch_LLC;
 static PyObject *__pyx_n_s_DeprecationWarning;
+static PyObject *__pyx_kp_u_Invalid_curve_length;
+static PyObject *__pyx_kp_u_Invalid_hidden_length;
+static PyObject *__pyx_kp_u_Invalid_seed_length;
 static PyObject *__pyx_kp_u_Jetperch_LLC;
 static PyObject *__pyx_kp_s_Pickling_of_struct_members_such;
 static PyObject *__pyx_kp_u_Python_ctypes_bindings_to_the_Mo;
 static PyObject *__pyx_n_s_Pyx_CFunc_int____const__uint8;
 static PyObject *__pyx_n_s_Pyx_CFunc_void____uint8__t;
 static PyObject *__pyx_n_s_SignatureVerify;
 static PyObject *__pyx_n_s_TypeError;
@@ -1625,27 +1666,33 @@
 static PyObject *__pyx_n_s_chacha20;
 static PyObject *__pyx_n_u_chacha20;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_compute_key_exchange_public_key;
 static PyObject *__pyx_n_s_compute_signing_public_key;
 static PyObject *__pyx_n_s_copyright;
 static PyObject *__pyx_n_s_crypto_text;
+static PyObject *__pyx_n_s_curve;
+static PyObject *__pyx_kp_u_curve_point_is_unsuitable_for_hi;
 static PyObject *__pyx_n_s_data;
 static PyObject *__pyx_n_u_default;
 static PyObject *__pyx_kp_u_deprecated_use_compute_signing_p;
 static PyObject *__pyx_kp_u_deprecated_use_generate_signing;
 static PyObject *__pyx_n_s_description;
+static PyObject *__pyx_n_s_elligator_key_pair;
+static PyObject *__pyx_n_s_elligator_map;
+static PyObject *__pyx_n_s_elligator_rev;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_generate_key;
 static PyObject *__pyx_n_s_generate_key_exchange_key_pair;
 static PyObject *__pyx_n_s_generate_key_pair;
 static PyObject *__pyx_n_s_generate_signing_key_pair;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_n_s_hash;
 static PyObject *__pyx_n_s_hash_size;
+static PyObject *__pyx_n_s_hidden;
 static PyObject *__pyx_kp_u_https_github_com_jetperch_pymono;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_kp_u_invalid_nonce_length;
 static PyObject *__pyx_kp_u_joulescope_dev_jetperch_com;
 static PyObject *__pyx_n_s_key;
 static PyObject *__pyx_n_s_key_exchange;
 static PyObject *__pyx_n_s_kp;
@@ -1667,35 +1714,38 @@
 static PyObject *__pyx_n_s_p;
 static PyObject *__pyx_n_s_password;
 static PyObject *__pyx_n_s_plain_text;
 static PyObject *__pyx_n_s_public;
 static PyObject *__pyx_n_s_public_key;
 static PyObject *__pyx_n_s_public_key_compute;
 static PyObject *__pyx_n_u_pymonocypher;
+static PyObject *__pyx_n_s_randbits;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_result;
 static PyObject *__pyx_n_s_rv;
 static PyObject *__pyx_n_s_salt;
 static PyObject *__pyx_n_s_secret;
 static PyObject *__pyx_n_s_secret_key;
 static PyObject *__pyx_n_s_secrets;
 static PyObject *__pyx_n_u_secrets;
+static PyObject *__pyx_n_s_seed;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_sig;
 static PyObject *__pyx_n_s_signature;
 static PyObject *__pyx_n_s_signature_check;
 static PyObject *__pyx_n_s_signature_sign;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_their_public_key;
 static PyObject *__pyx_n_s_title;
 static PyObject *__pyx_n_s_token_bytes;
+static PyObject *__pyx_n_s_tweak;
 static PyObject *__pyx_n_s_unlock;
 static PyObject *__pyx_kp_u_unsupported_method_s;
 static PyObject *__pyx_n_s_url;
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_s_version;
 static PyObject *__pyx_n_s_warn;
 static PyObject *__pyx_n_s_warnings;
@@ -1725,20 +1775,24 @@
 static PyObject *__pyx_pf_10monocypher_15SignatureVerify_4finalize(struct __pyx_obj_10monocypher_SignatureVerify *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10monocypher_15SignatureVerify_6__reduce_cython__(CYTHON_UNUSED struct __pyx_obj_10monocypher_SignatureVerify *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_10monocypher_15SignatureVerify_8__setstate_cython__(CYTHON_UNUSED struct __pyx_obj_10monocypher_SignatureVerify *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_10monocypher_24generate_key(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_length, PyObject *__pyx_v_method); /* proto */
 static PyObject *__pyx_pf_10monocypher_26generate_signing_key_pair(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_10monocypher_28generate_key_pair(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_10monocypher_30generate_key_exchange_key_pair(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_10monocypher_32elligator_map(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_hidden); /* proto */
+static PyObject *__pyx_pf_10monocypher_34elligator_rev(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_curve, PyObject *__pyx_v_tweak); /* proto */
+static PyObject *__pyx_pf_10monocypher_36elligator_key_pair(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_seed); /* proto */
 static PyObject *__pyx_pf_11cfunc_dot_to_py_69__Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py_wrap(PyObject *__pyx_self, uint8_t const *__pyx_v_a, uint8_t const *__pyx_v_b); /* proto */
 static PyObject *__pyx_pf_11cfunc_dot_to_py_63__Pyx_CFunc_void____uint8__t________const__uint8__t_______to_py_wrap(PyObject *__pyx_self, uint8_t *__pyx_v_public_key, uint8_t const *__pyx_v_secret_key); /* proto */
 static PyObject *__pyx_tp_new_10monocypher_Blake2b(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_10monocypher_SignatureVerify(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new___pyx_scope_struct____Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new___pyx_scope_struct____Pyx_CFunc_void____uint8__t________const__uint8__t_______to_py(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_int_8;
 static PyObject *__pyx_int_16;
 static PyObject *__pyx_int_24;
 static PyObject *__pyx_int_32;
 static PyObject *__pyx_int_64;
 static PyObject *__pyx_int_1024;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
@@ -1747,48 +1801,55 @@
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
 static PyObject *__pyx_tuple__10;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_tuple__14;
-static PyObject *__pyx_tuple__16;
-static PyObject *__pyx_tuple__18;
-static PyObject *__pyx_tuple__20;
-static PyObject *__pyx_tuple__22;
-static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_tuple__26;
-static PyObject *__pyx_tuple__28;
-static PyObject *__pyx_tuple__30;
-static PyObject *__pyx_tuple__32;
-static PyObject *__pyx_tuple__34;
-static PyObject *__pyx_tuple__36;
-static PyObject *__pyx_tuple__38;
-static PyObject *__pyx_tuple__40;
-static PyObject *__pyx_tuple__42;
-static PyObject *__pyx_tuple__45;
-static PyObject *__pyx_codeobj__13;
-static PyObject *__pyx_codeobj__15;
-static PyObject *__pyx_codeobj__17;
-static PyObject *__pyx_codeobj__19;
-static PyObject *__pyx_codeobj__21;
-static PyObject *__pyx_codeobj__23;
-static PyObject *__pyx_codeobj__25;
-static PyObject *__pyx_codeobj__27;
-static PyObject *__pyx_codeobj__29;
-static PyObject *__pyx_codeobj__31;
-static PyObject *__pyx_codeobj__33;
-static PyObject *__pyx_codeobj__35;
-static PyObject *__pyx_codeobj__37;
-static PyObject *__pyx_codeobj__39;
-static PyObject *__pyx_codeobj__41;
-static PyObject *__pyx_codeobj__43;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__15;
+static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_tuple__19;
+static PyObject *__pyx_tuple__21;
+static PyObject *__pyx_tuple__23;
+static PyObject *__pyx_tuple__25;
+static PyObject *__pyx_tuple__27;
+static PyObject *__pyx_tuple__29;
+static PyObject *__pyx_tuple__31;
+static PyObject *__pyx_tuple__33;
+static PyObject *__pyx_tuple__35;
+static PyObject *__pyx_tuple__37;
+static PyObject *__pyx_tuple__39;
+static PyObject *__pyx_tuple__41;
+static PyObject *__pyx_tuple__43;
+static PyObject *__pyx_tuple__46;
+static PyObject *__pyx_tuple__48;
+static PyObject *__pyx_tuple__50;
+static PyObject *__pyx_tuple__52;
+static PyObject *__pyx_codeobj__14;
+static PyObject *__pyx_codeobj__16;
+static PyObject *__pyx_codeobj__18;
+static PyObject *__pyx_codeobj__20;
+static PyObject *__pyx_codeobj__22;
+static PyObject *__pyx_codeobj__24;
+static PyObject *__pyx_codeobj__26;
+static PyObject *__pyx_codeobj__28;
+static PyObject *__pyx_codeobj__30;
+static PyObject *__pyx_codeobj__32;
+static PyObject *__pyx_codeobj__34;
+static PyObject *__pyx_codeobj__36;
+static PyObject *__pyx_codeobj__38;
+static PyObject *__pyx_codeobj__40;
+static PyObject *__pyx_codeobj__42;
 static PyObject *__pyx_codeobj__44;
-static PyObject *__pyx_codeobj__46;
+static PyObject *__pyx_codeobj__45;
+static PyObject *__pyx_codeobj__47;
+static PyObject *__pyx_codeobj__49;
+static PyObject *__pyx_codeobj__51;
+static PyObject *__pyx_codeobj__53;
 /* Late includes */
 
 /* "monocypher.pyx":312
  *                                const uint8_t curve_point[32])
  * 
  * def wipe(data):             # <<<<<<<<<<<<<<
  *     """Wipe a bytes object from memory.
@@ -5485,14 +5546,15 @@
   __pyx_t_1 = 0;
 
   /* "monocypher.pyx":616
  *     """
  *     secret = generate_key()
  *     public = compute_key_exchange_public_key(secret)             # <<<<<<<<<<<<<<
  *     return secret, public
+ * 
  */
   __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_compute_key_exchange_public_key); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 616, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -5510,14 +5572,16 @@
   __pyx_v_public = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "monocypher.pyx":617
  *     secret = generate_key()
  *     public = compute_key_exchange_public_key(secret)
  *     return secret, public             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 617, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_secret);
   __Pyx_GIVEREF(__pyx_v_secret);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_secret);
@@ -5547,14 +5611,794 @@
   __Pyx_XDECREF(__pyx_v_secret);
   __Pyx_XDECREF(__pyx_v_public);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "monocypher.pyx":623
+ * 
+ * 
+ * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
+ *     """Computes the point corresponding to a representative.
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10monocypher_33elligator_map(PyObject *__pyx_self, PyObject *__pyx_v_hidden); /*proto*/
+static char __pyx_doc_10monocypher_32elligator_map[] = "Computes the point corresponding to a representative.\n\n    :param hidden: The 32 byte hidden key.\n    :return: The 32-byte little-endian encoded public key.\n        Since positive representatives fits in 254 bits,\n        the two most significant bits are ignored.\n    ";
+static PyMethodDef __pyx_mdef_10monocypher_33elligator_map = {"elligator_map", (PyCFunction)__pyx_pw_10monocypher_33elligator_map, METH_O, __pyx_doc_10monocypher_32elligator_map};
+static PyObject *__pyx_pw_10monocypher_33elligator_map(PyObject *__pyx_self, PyObject *__pyx_v_hidden) {
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("elligator_map (wrapper)", 0);
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_hidden), (&PyBytes_Type), 1, "hidden", 1))) __PYX_ERR(0, 623, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10monocypher_32elligator_map(__pyx_self, ((PyObject*)__pyx_v_hidden));
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10monocypher_32elligator_map(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_hidden) {
+  PyObject *__pyx_v_curve = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  int __pyx_t_3;
+  Py_UCS4 __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  uint8_t *__pyx_t_7;
+  uint8_t const *__pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("elligator_map", 0);
+
+  /* "monocypher.pyx":631
+ *         the two most significant bits are ignored.
+ *     """
+ *     curve = bytes(32)             # <<<<<<<<<<<<<<
+ *     if len(hidden) != 32:
+ *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 631, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_curve = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "monocypher.pyx":632
+ *     """
+ *     curve = bytes(32)
+ *     if len(hidden) != 32:             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
+ *     crypto_hidden_to_curve(curve, hidden)
+ */
+  if (unlikely(__pyx_v_hidden == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(0, 632, __pyx_L1_error)
+  }
+  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_hidden); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 632, __pyx_L1_error)
+  __pyx_t_3 = ((__pyx_t_2 != 32) != 0);
+  if (unlikely(__pyx_t_3)) {
+
+    /* "monocypher.pyx":633
+ *     curve = bytes(32)
+ *     if len(hidden) != 32:
+ *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')             # <<<<<<<<<<<<<<
+ *     crypto_hidden_to_curve(curve, hidden)
+ *     return curve
+ */
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = 0;
+    __pyx_t_4 = 127;
+    __Pyx_INCREF(__pyx_kp_u_Invalid_hidden_length);
+    __pyx_t_2 += 22;
+    __Pyx_GIVEREF(__pyx_kp_u_Invalid_hidden_length);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_hidden_length);
+    if (unlikely(__pyx_v_hidden == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+      __PYX_ERR(0, 633, __pyx_L1_error)
+    }
+    __pyx_t_5 = PyBytes_GET_SIZE(__pyx_v_hidden); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 633, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 633, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
+    __pyx_t_6 = 0;
+    __Pyx_INCREF(__pyx_kp_u_32);
+    __pyx_t_2 += 6;
+    __Pyx_GIVEREF(__pyx_kp_u_32);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_32);
+    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 633, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 633, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __PYX_ERR(0, 633, __pyx_L1_error)
+
+    /* "monocypher.pyx":632
+ *     """
+ *     curve = bytes(32)
+ *     if len(hidden) != 32:             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
+ *     crypto_hidden_to_curve(curve, hidden)
+ */
+  }
+
+  /* "monocypher.pyx":634
+ *     if len(hidden) != 32:
+ *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
+ *     crypto_hidden_to_curve(curve, hidden)             # <<<<<<<<<<<<<<
+ *     return curve
+ * 
+ */
+  __pyx_t_7 = __Pyx_PyBytes_AsWritableUString(__pyx_v_curve); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 634, __pyx_L1_error)
+  if (unlikely(__pyx_v_hidden == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
+    __PYX_ERR(0, 634, __pyx_L1_error)
+  }
+  __pyx_t_8 = __Pyx_PyBytes_AsUString(__pyx_v_hidden); if (unlikely((!__pyx_t_8) && PyErr_Occurred())) __PYX_ERR(0, 634, __pyx_L1_error)
+  crypto_hidden_to_curve(__pyx_t_7, __pyx_t_8);
+
+  /* "monocypher.pyx":635
+ *         raise ValueError(f'Invalid hidden length {len(hidden)} != 32')
+ *     crypto_hidden_to_curve(curve, hidden)
+ *     return curve             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_curve);
+  __pyx_r = __pyx_v_curve;
+  goto __pyx_L0;
+
+  /* "monocypher.pyx":623
+ * 
+ * 
+ * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
+ *     """Computes the point corresponding to a representative.
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("monocypher.elligator_map", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_curve);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "monocypher.pyx":638
+ * 
+ * 
+ * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
+ *     """Computes the representative of a point.
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10monocypher_35elligator_rev(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10monocypher_34elligator_rev[] = "Computes the representative of a point.\n\n    :param curve: The 32-byte little-endian encoded public key.\n    :param tweak: The optional random byte.  If None (default),\n        then automatically generate a random byte.\n    :return: The 32-byte secret key\n    :raise ValueError: If the combination of curve point and tweak\n        is unsuitable for hiding.  Choose another curve point\n        and try again.\n    ";
+static PyMethodDef __pyx_mdef_10monocypher_35elligator_rev = {"elligator_rev", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10monocypher_35elligator_rev, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10monocypher_34elligator_rev};
+static PyObject *__pyx_pw_10monocypher_35elligator_rev(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_curve = 0;
+  PyObject *__pyx_v_tweak = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("elligator_rev (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_curve,&__pyx_n_s_tweak,0};
+    PyObject* values[2] = {0,0};
+    values[1] = ((PyObject *)Py_None);
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_curve)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_tweak);
+          if (value) { values[1] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "elligator_rev") < 0)) __PYX_ERR(0, 638, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_curve = ((PyObject*)values[0]);
+    __pyx_v_tweak = values[1];
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("elligator_rev", 0, 1, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 638, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("monocypher.elligator_rev", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_curve), (&PyBytes_Type), 1, "curve", 1))) __PYX_ERR(0, 638, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10monocypher_34elligator_rev(__pyx_self, __pyx_v_curve, __pyx_v_tweak);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10monocypher_34elligator_rev(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_curve, PyObject *__pyx_v_tweak) {
+  PyObject *__pyx_v_hidden = NULL;
+  int __pyx_v_rv;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  Py_ssize_t __pyx_t_2;
+  int __pyx_t_3;
+  Py_UCS4 __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_7;
+  PyObject *__pyx_t_8 = NULL;
+  uint8_t *__pyx_t_9;
+  uint8_t const *__pyx_t_10;
+  uint8_t __pyx_t_11;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("elligator_rev", 0);
+  __Pyx_INCREF(__pyx_v_tweak);
+
+  /* "monocypher.pyx":649
+ *         and try again.
+ *     """
+ *     hidden = bytes(32)             # <<<<<<<<<<<<<<
+ *     if len(curve) != 32:
+ *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 649, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_hidden = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "monocypher.pyx":650
+ *     """
+ *     hidden = bytes(32)
+ *     if len(curve) != 32:             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
+ *     if tweak is None:
+ */
+  if (unlikely(__pyx_v_curve == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(0, 650, __pyx_L1_error)
+  }
+  __pyx_t_2 = PyBytes_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_2 == ((Py_ssize_t)-1))) __PYX_ERR(0, 650, __pyx_L1_error)
+  __pyx_t_3 = ((__pyx_t_2 != 32) != 0);
+  if (unlikely(__pyx_t_3)) {
+
+    /* "monocypher.pyx":651
+ *     hidden = bytes(32)
+ *     if len(curve) != 32:
+ *         raise ValueError(f'Invalid curve length {len(curve)} != 32')             # <<<<<<<<<<<<<<
+ *     if tweak is None:
+ *         tweak = secrets.randbits(8)
+ */
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 651, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = 0;
+    __pyx_t_4 = 127;
+    __Pyx_INCREF(__pyx_kp_u_Invalid_curve_length);
+    __pyx_t_2 += 21;
+    __Pyx_GIVEREF(__pyx_kp_u_Invalid_curve_length);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_curve_length);
+    if (unlikely(__pyx_v_curve == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+      __PYX_ERR(0, 651, __pyx_L1_error)
+    }
+    __pyx_t_5 = PyBytes_GET_SIZE(__pyx_v_curve); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 651, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_5, 0, ' ', 'd'); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 651, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_2 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_6);
+    __Pyx_GIVEREF(__pyx_t_6);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_6);
+    __pyx_t_6 = 0;
+    __Pyx_INCREF(__pyx_kp_u_32);
+    __pyx_t_2 += 6;
+    __Pyx_GIVEREF(__pyx_kp_u_32);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_32);
+    __pyx_t_6 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 651, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_6); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 651, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __PYX_ERR(0, 651, __pyx_L1_error)
+
+    /* "monocypher.pyx":650
+ *     """
+ *     hidden = bytes(32)
+ *     if len(curve) != 32:             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
+ *     if tweak is None:
+ */
+  }
+
+  /* "monocypher.pyx":652
+ *     if len(curve) != 32:
+ *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
+ *     if tweak is None:             # <<<<<<<<<<<<<<
+ *         tweak = secrets.randbits(8)
+ *     rv = crypto_curve_to_hidden(hidden, curve, tweak)
+ */
+  __pyx_t_3 = (__pyx_v_tweak == Py_None);
+  __pyx_t_7 = (__pyx_t_3 != 0);
+  if (__pyx_t_7) {
+
+    /* "monocypher.pyx":653
+ *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
+ *     if tweak is None:
+ *         tweak = secrets.randbits(8)             # <<<<<<<<<<<<<<
+ *     rv = crypto_curve_to_hidden(hidden, curve, tweak)
+ *     if rv:
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_secrets); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 653, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_6);
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_randbits); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 653, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_6 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_8))) {
+      __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_8);
+      if (likely(__pyx_t_6)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_6);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_8, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_6) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_6, __pyx_int_8) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_int_8);
+    __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 653, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
+    __Pyx_DECREF_SET(__pyx_v_tweak, __pyx_t_1);
+    __pyx_t_1 = 0;
+
+    /* "monocypher.pyx":652
+ *     if len(curve) != 32:
+ *         raise ValueError(f'Invalid curve length {len(curve)} != 32')
+ *     if tweak is None:             # <<<<<<<<<<<<<<
+ *         tweak = secrets.randbits(8)
+ *     rv = crypto_curve_to_hidden(hidden, curve, tweak)
+ */
+  }
+
+  /* "monocypher.pyx":654
+ *     if tweak is None:
+ *         tweak = secrets.randbits(8)
+ *     rv = crypto_curve_to_hidden(hidden, curve, tweak)             # <<<<<<<<<<<<<<
+ *     if rv:
+ *         raise ValueError('curve point is unsuitable for hiding')
+ */
+  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hidden); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 654, __pyx_L1_error)
+  if (unlikely(__pyx_v_curve == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
+    __PYX_ERR(0, 654, __pyx_L1_error)
+  }
+  __pyx_t_10 = __Pyx_PyBytes_AsUString(__pyx_v_curve); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 654, __pyx_L1_error)
+  __pyx_t_11 = __Pyx_PyInt_As_uint8_t(__pyx_v_tweak); if (unlikely((__pyx_t_11 == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 654, __pyx_L1_error)
+  __pyx_v_rv = crypto_curve_to_hidden(__pyx_t_9, __pyx_t_10, __pyx_t_11);
+
+  /* "monocypher.pyx":655
+ *         tweak = secrets.randbits(8)
+ *     rv = crypto_curve_to_hidden(hidden, curve, tweak)
+ *     if rv:             # <<<<<<<<<<<<<<
+ *         raise ValueError('curve point is unsuitable for hiding')
+ *     return hidden
+ */
+  __pyx_t_7 = (__pyx_v_rv != 0);
+  if (unlikely(__pyx_t_7)) {
+
+    /* "monocypher.pyx":656
+ *     rv = crypto_curve_to_hidden(hidden, curve, tweak)
+ *     if rv:
+ *         raise ValueError('curve point is unsuitable for hiding')             # <<<<<<<<<<<<<<
+ *     return hidden
+ * 
+ */
+    __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 656, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __PYX_ERR(0, 656, __pyx_L1_error)
+
+    /* "monocypher.pyx":655
+ *         tweak = secrets.randbits(8)
+ *     rv = crypto_curve_to_hidden(hidden, curve, tweak)
+ *     if rv:             # <<<<<<<<<<<<<<
+ *         raise ValueError('curve point is unsuitable for hiding')
+ *     return hidden
+ */
+  }
+
+  /* "monocypher.pyx":657
+ *     if rv:
+ *         raise ValueError('curve point is unsuitable for hiding')
+ *     return hidden             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_hidden);
+  __pyx_r = __pyx_v_hidden;
+  goto __pyx_L0;
+
+  /* "monocypher.pyx":638
+ * 
+ * 
+ * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
+ *     """Computes the representative of a point.
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_8);
+  __Pyx_AddTraceback("monocypher.elligator_rev", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_hidden);
+  __Pyx_XDECREF(__pyx_v_tweak);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "monocypher.pyx":660
+ * 
+ * 
+ * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
+ *     """Generate a key pair.
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_10monocypher_37elligator_key_pair(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_10monocypher_36elligator_key_pair[] = "Generate a key pair.\n\n    :param seed: The 32-byte seed that is used to derive the key pair.\n        None (default) generate a cryptographically secure random seed.\n    :return: The tuple of hidden and secret_key.\n        * hidden: The 32-byte little ending encoding of a point on the curve\n          which is effectively indistinguishable from random.\n        * secret_key: The generated 32-byte little endian secret key.\n    ";
+static PyMethodDef __pyx_mdef_10monocypher_37elligator_key_pair = {"elligator_key_pair", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_10monocypher_37elligator_key_pair, METH_VARARGS|METH_KEYWORDS, __pyx_doc_10monocypher_36elligator_key_pair};
+static PyObject *__pyx_pw_10monocypher_37elligator_key_pair(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_seed = 0;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("elligator_key_pair (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_seed,0};
+    PyObject* values[1] = {0};
+    values[0] = ((PyObject*)Py_None);
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_seed);
+          if (value) { values[0] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "elligator_key_pair") < 0)) __PYX_ERR(0, 660, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_seed = ((PyObject*)values[0]);
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("elligator_key_pair", 0, 0, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 660, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("monocypher.elligator_key_pair", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seed), (&PyBytes_Type), 1, "seed", 1))) __PYX_ERR(0, 660, __pyx_L1_error)
+  __pyx_r = __pyx_pf_10monocypher_36elligator_key_pair(__pyx_self, __pyx_v_seed);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_10monocypher_36elligator_key_pair(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_seed) {
+  PyObject *__pyx_v_hidden = NULL;
+  PyObject *__pyx_v_secret_key = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_t_2;
+  int __pyx_t_3;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  Py_ssize_t __pyx_t_6;
+  Py_UCS4 __pyx_t_7;
+  Py_ssize_t __pyx_t_8;
+  uint8_t *__pyx_t_9;
+  uint8_t *__pyx_t_10;
+  uint8_t *__pyx_t_11;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("elligator_key_pair", 0);
+  __Pyx_INCREF(__pyx_v_seed);
+
+  /* "monocypher.pyx":670
+ *         * secret_key: The generated 32-byte little endian secret key.
+ *     """
+ *     hidden = bytes(32)             # <<<<<<<<<<<<<<
+ *     secret_key = bytes(32)
+ *     if seed is None:
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 670, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_hidden = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "monocypher.pyx":671
+ *     """
+ *     hidden = bytes(32)
+ *     secret_key = bytes(32)             # <<<<<<<<<<<<<<
+ *     if seed is None:
+ *         seed = secrets.token_bytes(32)
+ */
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)(&PyBytes_Type)), __pyx_tuple__7, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 671, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_secret_key = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "monocypher.pyx":672
+ *     hidden = bytes(32)
+ *     secret_key = bytes(32)
+ *     if seed is None:             # <<<<<<<<<<<<<<
+ *         seed = secrets.token_bytes(32)
+ *     elif len(seed) != 32:
+ */
+  __pyx_t_2 = (__pyx_v_seed == ((PyObject*)Py_None));
+  __pyx_t_3 = (__pyx_t_2 != 0);
+  if (__pyx_t_3) {
+
+    /* "monocypher.pyx":673
+ *     secret_key = bytes(32)
+ *     if seed is None:
+ *         seed = secrets.token_bytes(32)             # <<<<<<<<<<<<<<
+ *     elif len(seed) != 32:
+ *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_secrets); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 673, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_token_bytes); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 673, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __pyx_t_4 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_4)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_4);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+      }
+    }
+    __pyx_t_1 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_5, __pyx_t_4, __pyx_int_32) : __Pyx_PyObject_CallOneArg(__pyx_t_5, __pyx_int_32);
+    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 673, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    if (!(likely(PyBytes_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(0, 673, __pyx_L1_error)
+    __Pyx_DECREF_SET(__pyx_v_seed, ((PyObject*)__pyx_t_1));
+    __pyx_t_1 = 0;
+
+    /* "monocypher.pyx":672
+ *     hidden = bytes(32)
+ *     secret_key = bytes(32)
+ *     if seed is None:             # <<<<<<<<<<<<<<
+ *         seed = secrets.token_bytes(32)
+ *     elif len(seed) != 32:
+ */
+    goto __pyx_L3;
+  }
+
+  /* "monocypher.pyx":674
+ *     if seed is None:
+ *         seed = secrets.token_bytes(32)
+ *     elif len(seed) != 32:             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
+ *     crypto_hidden_key_pair(hidden, secret_key, seed)
+ */
+  if (unlikely(__pyx_v_seed == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+    __PYX_ERR(0, 674, __pyx_L1_error)
+  }
+  __pyx_t_6 = PyBytes_GET_SIZE(__pyx_v_seed); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 674, __pyx_L1_error)
+  __pyx_t_3 = ((__pyx_t_6 != 32) != 0);
+  if (unlikely(__pyx_t_3)) {
+
+    /* "monocypher.pyx":675
+ *         seed = secrets.token_bytes(32)
+ *     elif len(seed) != 32:
+ *         raise ValueError(f'Invalid seed length {len(seed)} != 32')             # <<<<<<<<<<<<<<
+ *     crypto_hidden_key_pair(hidden, secret_key, seed)
+ *     return hidden, secret_key
+ */
+    __pyx_t_1 = PyTuple_New(3); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 675, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_6 = 0;
+    __pyx_t_7 = 127;
+    __Pyx_INCREF(__pyx_kp_u_Invalid_seed_length);
+    __pyx_t_6 += 20;
+    __Pyx_GIVEREF(__pyx_kp_u_Invalid_seed_length);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_kp_u_Invalid_seed_length);
+    if (unlikely(__pyx_v_seed == Py_None)) {
+      PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
+      __PYX_ERR(0, 675, __pyx_L1_error)
+    }
+    __pyx_t_8 = PyBytes_GET_SIZE(__pyx_v_seed); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(0, 675, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_t_8, 0, ' ', 'd'); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 675, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_6 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_5);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_5);
+    __pyx_t_5 = 0;
+    __Pyx_INCREF(__pyx_kp_u_32);
+    __pyx_t_6 += 6;
+    __Pyx_GIVEREF(__pyx_kp_u_32);
+    PyTuple_SET_ITEM(__pyx_t_1, 2, __pyx_kp_u_32);
+    __pyx_t_5 = __Pyx_PyUnicode_Join(__pyx_t_1, 3, __pyx_t_6, __pyx_t_7); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 675, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_1 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_5); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 675, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_Raise(__pyx_t_1, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __PYX_ERR(0, 675, __pyx_L1_error)
+
+    /* "monocypher.pyx":674
+ *     if seed is None:
+ *         seed = secrets.token_bytes(32)
+ *     elif len(seed) != 32:             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
+ *     crypto_hidden_key_pair(hidden, secret_key, seed)
+ */
+  }
+  __pyx_L3:;
+
+  /* "monocypher.pyx":676
+ *     elif len(seed) != 32:
+ *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
+ *     crypto_hidden_key_pair(hidden, secret_key, seed)             # <<<<<<<<<<<<<<
+ *     return hidden, secret_key
+ */
+  __pyx_t_9 = __Pyx_PyBytes_AsWritableUString(__pyx_v_hidden); if (unlikely((!__pyx_t_9) && PyErr_Occurred())) __PYX_ERR(0, 676, __pyx_L1_error)
+  __pyx_t_10 = __Pyx_PyBytes_AsWritableUString(__pyx_v_secret_key); if (unlikely((!__pyx_t_10) && PyErr_Occurred())) __PYX_ERR(0, 676, __pyx_L1_error)
+  if (unlikely(__pyx_v_seed == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
+    __PYX_ERR(0, 676, __pyx_L1_error)
+  }
+  __pyx_t_11 = __Pyx_PyBytes_AsWritableUString(__pyx_v_seed); if (unlikely((!__pyx_t_11) && PyErr_Occurred())) __PYX_ERR(0, 676, __pyx_L1_error)
+  crypto_hidden_key_pair(__pyx_t_9, __pyx_t_10, __pyx_t_11);
+
+  /* "monocypher.pyx":677
+ *         raise ValueError(f'Invalid seed length {len(seed)} != 32')
+ *     crypto_hidden_key_pair(hidden, secret_key, seed)
+ *     return hidden, secret_key             # <<<<<<<<<<<<<<
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 677, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_v_hidden);
+  __Pyx_GIVEREF(__pyx_v_hidden);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_hidden);
+  __Pyx_INCREF(__pyx_v_secret_key);
+  __Pyx_GIVEREF(__pyx_v_secret_key);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_secret_key);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "monocypher.pyx":660
+ * 
+ * 
+ * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
+ *     """Generate a key pair.
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("monocypher.elligator_key_pair", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_hidden);
+  __Pyx_XDECREF(__pyx_v_secret_key);
+  __Pyx_XDECREF(__pyx_v_seed);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "cfunc.to_py":65
  * @cname("__Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py")
  * cdef object __Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py(int (*f)(const uint8_t *, const uint8_t *) except *):
  *     def wrap(const uint8_t * a, const uint8_t * b):             # <<<<<<<<<<<<<<
  *         """wrap(a: 'const uint8_t *', b: 'const uint8_t *') -> 'int'"""
  *         return f(a, b)
  */
@@ -5704,15 +6548,15 @@
   /* "cfunc.to_py":65
  * @cname("__Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py")
  * cdef object __Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py(int (*f)(const uint8_t *, const uint8_t *) except *):
  *     def wrap(const uint8_t * a, const uint8_t * b):             # <<<<<<<<<<<<<<
  *         """wrap(a: 'const uint8_t *', b: 'const uint8_t *') -> 'int'"""
  *         return f(a, b)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_69__Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_int____const__uint8, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_69__Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_int____const__uint8, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_wrap = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "cfunc.to_py":68
  *         """wrap(a: 'const uint8_t *', b: 'const uint8_t *') -> 'int'"""
  *         return f(a, b)
@@ -5892,15 +6736,15 @@
   /* "cfunc.to_py":65
  * @cname("__Pyx_CFunc_void____uint8__t________const__uint8__t_______to_py")
  * cdef object __Pyx_CFunc_void____uint8__t________const__uint8__t_______to_py(void (*f)(uint8_t *, const uint8_t *) except *):
  *     def wrap(uint8_t * public_key, const uint8_t * secret_key):             # <<<<<<<<<<<<<<
  *         """wrap(public_key: 'uint8_t *', secret_key: 'const uint8_t *') -> 'void'"""
  *         f(public_key, secret_key)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_63__Pyx_CFunc_void____uint8__t________const__uint8__t_______to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_void____uint8__t, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_11cfunc_dot_to_py_63__Pyx_CFunc_void____uint8__t________const__uint8__t_______to_py_1wrap, 0, __pyx_n_s_Pyx_CFunc_void____uint8__t, ((PyObject*)__pyx_cur_scope), __pyx_n_s_cfunc_to_py, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 65, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_wrap = __pyx_t_1;
   __pyx_t_1 = 0;
 
   /* "cfunc.to_py":68
  *         """wrap(public_key: 'uint8_t *', secret_key: 'const uint8_t *') -> 'void'"""
  *         f(public_key, secret_key)
@@ -6025,15 +6869,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_10monocypher_SignatureVerify(PyTypeObject *t, PyObject *a, PyObject *k) {
   PyObject *o;
   if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
@@ -6129,15 +6973,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py[8];
 static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py = 0;
 
@@ -6225,15 +7069,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj___pyx_scope_struct____Pyx_CFunc_void____uint8__t________const__uint8__t_______to_py *__pyx_freelist___pyx_scope_struct____Pyx_CFunc_void____uint8__t________const__uint8__t_______to_py[8];
 static int __pyx_freecount___pyx_scope_struct____Pyx_CFunc_void____uint8__t________const__uint8__t_______to_py = 0;
 
@@ -6321,15 +7165,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -6372,19 +7216,23 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
-  {&__pyx_kp_u_3_1_3_1, __pyx_k_3_1_3_1, sizeof(__pyx_k_3_1_3_1), 0, 1, 0, 0},
+  {&__pyx_kp_u_32, __pyx_k_32, sizeof(__pyx_k_32), 0, 1, 0, 0},
+  {&__pyx_kp_u_3_1_3_2, __pyx_k_3_1_3_2, sizeof(__pyx_k_3_1_3_2), 0, 1, 0, 0},
   {&__pyx_kp_u_BSD_2_clause, __pyx_k_BSD_2_clause, sizeof(__pyx_k_BSD_2_clause), 0, 1, 0, 0},
   {&__pyx_n_s_Blake2b, __pyx_k_Blake2b, sizeof(__pyx_k_Blake2b), 0, 0, 1, 1},
   {&__pyx_kp_u_Copyright_2018_2022_Jetperch_LLC, __pyx_k_Copyright_2018_2022_Jetperch_LLC, sizeof(__pyx_k_Copyright_2018_2022_Jetperch_LLC), 0, 1, 0, 0},
   {&__pyx_n_s_DeprecationWarning, __pyx_k_DeprecationWarning, sizeof(__pyx_k_DeprecationWarning), 0, 0, 1, 1},
+  {&__pyx_kp_u_Invalid_curve_length, __pyx_k_Invalid_curve_length, sizeof(__pyx_k_Invalid_curve_length), 0, 1, 0, 0},
+  {&__pyx_kp_u_Invalid_hidden_length, __pyx_k_Invalid_hidden_length, sizeof(__pyx_k_Invalid_hidden_length), 0, 1, 0, 0},
+  {&__pyx_kp_u_Invalid_seed_length, __pyx_k_Invalid_seed_length, sizeof(__pyx_k_Invalid_seed_length), 0, 1, 0, 0},
   {&__pyx_kp_u_Jetperch_LLC, __pyx_k_Jetperch_LLC, sizeof(__pyx_k_Jetperch_LLC), 0, 1, 0, 0},
   {&__pyx_kp_s_Pickling_of_struct_members_such, __pyx_k_Pickling_of_struct_members_such, sizeof(__pyx_k_Pickling_of_struct_members_such), 0, 0, 1, 0},
   {&__pyx_kp_u_Python_ctypes_bindings_to_the_Mo, __pyx_k_Python_ctypes_bindings_to_the_Mo, sizeof(__pyx_k_Python_ctypes_bindings_to_the_Mo), 0, 1, 0, 0},
   {&__pyx_n_s_Pyx_CFunc_int____const__uint8, __pyx_k_Pyx_CFunc_int____const__uint8, sizeof(__pyx_k_Pyx_CFunc_int____const__uint8), 0, 0, 1, 1},
   {&__pyx_n_s_Pyx_CFunc_void____uint8__t, __pyx_k_Pyx_CFunc_void____uint8__t, sizeof(__pyx_k_Pyx_CFunc_void____uint8__t), 0, 0, 1, 1},
   {&__pyx_n_s_SignatureVerify, __pyx_k_SignatureVerify, sizeof(__pyx_k_SignatureVerify), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
@@ -6405,27 +7253,33 @@
   {&__pyx_n_s_chacha20, __pyx_k_chacha20, sizeof(__pyx_k_chacha20), 0, 0, 1, 1},
   {&__pyx_n_u_chacha20, __pyx_k_chacha20, sizeof(__pyx_k_chacha20), 0, 1, 0, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_compute_key_exchange_public_key, __pyx_k_compute_key_exchange_public_key, sizeof(__pyx_k_compute_key_exchange_public_key), 0, 0, 1, 1},
   {&__pyx_n_s_compute_signing_public_key, __pyx_k_compute_signing_public_key, sizeof(__pyx_k_compute_signing_public_key), 0, 0, 1, 1},
   {&__pyx_n_s_copyright, __pyx_k_copyright, sizeof(__pyx_k_copyright), 0, 0, 1, 1},
   {&__pyx_n_s_crypto_text, __pyx_k_crypto_text, sizeof(__pyx_k_crypto_text), 0, 0, 1, 1},
+  {&__pyx_n_s_curve, __pyx_k_curve, sizeof(__pyx_k_curve), 0, 0, 1, 1},
+  {&__pyx_kp_u_curve_point_is_unsuitable_for_hi, __pyx_k_curve_point_is_unsuitable_for_hi, sizeof(__pyx_k_curve_point_is_unsuitable_for_hi), 0, 1, 0, 0},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
   {&__pyx_n_u_default, __pyx_k_default, sizeof(__pyx_k_default), 0, 1, 0, 1},
   {&__pyx_kp_u_deprecated_use_compute_signing_p, __pyx_k_deprecated_use_compute_signing_p, sizeof(__pyx_k_deprecated_use_compute_signing_p), 0, 1, 0, 0},
   {&__pyx_kp_u_deprecated_use_generate_signing, __pyx_k_deprecated_use_generate_signing, sizeof(__pyx_k_deprecated_use_generate_signing), 0, 1, 0, 0},
   {&__pyx_n_s_description, __pyx_k_description, sizeof(__pyx_k_description), 0, 0, 1, 1},
+  {&__pyx_n_s_elligator_key_pair, __pyx_k_elligator_key_pair, sizeof(__pyx_k_elligator_key_pair), 0, 0, 1, 1},
+  {&__pyx_n_s_elligator_map, __pyx_k_elligator_map, sizeof(__pyx_k_elligator_map), 0, 0, 1, 1},
+  {&__pyx_n_s_elligator_rev, __pyx_k_elligator_rev, sizeof(__pyx_k_elligator_rev), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_generate_key, __pyx_k_generate_key, sizeof(__pyx_k_generate_key), 0, 0, 1, 1},
   {&__pyx_n_s_generate_key_exchange_key_pair, __pyx_k_generate_key_exchange_key_pair, sizeof(__pyx_k_generate_key_exchange_key_pair), 0, 0, 1, 1},
   {&__pyx_n_s_generate_key_pair, __pyx_k_generate_key_pair, sizeof(__pyx_k_generate_key_pair), 0, 0, 1, 1},
   {&__pyx_n_s_generate_signing_key_pair, __pyx_k_generate_signing_key_pair, sizeof(__pyx_k_generate_signing_key_pair), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_n_s_hash, __pyx_k_hash, sizeof(__pyx_k_hash), 0, 0, 1, 1},
   {&__pyx_n_s_hash_size, __pyx_k_hash_size, sizeof(__pyx_k_hash_size), 0, 0, 1, 1},
+  {&__pyx_n_s_hidden, __pyx_k_hidden, sizeof(__pyx_k_hidden), 0, 0, 1, 1},
   {&__pyx_kp_u_https_github_com_jetperch_pymono, __pyx_k_https_github_com_jetperch_pymono, sizeof(__pyx_k_https_github_com_jetperch_pymono), 0, 1, 0, 0},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_kp_u_invalid_nonce_length, __pyx_k_invalid_nonce_length, sizeof(__pyx_k_invalid_nonce_length), 0, 1, 0, 0},
   {&__pyx_kp_u_joulescope_dev_jetperch_com, __pyx_k_joulescope_dev_jetperch_com, sizeof(__pyx_k_joulescope_dev_jetperch_com), 0, 1, 0, 0},
   {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
   {&__pyx_n_s_key_exchange, __pyx_k_key_exchange, sizeof(__pyx_k_key_exchange), 0, 0, 1, 1},
   {&__pyx_n_s_kp, __pyx_k_kp, sizeof(__pyx_k_kp), 0, 0, 1, 1},
@@ -6447,35 +7301,38 @@
   {&__pyx_n_s_p, __pyx_k_p, sizeof(__pyx_k_p), 0, 0, 1, 1},
   {&__pyx_n_s_password, __pyx_k_password, sizeof(__pyx_k_password), 0, 0, 1, 1},
   {&__pyx_n_s_plain_text, __pyx_k_plain_text, sizeof(__pyx_k_plain_text), 0, 0, 1, 1},
   {&__pyx_n_s_public, __pyx_k_public, sizeof(__pyx_k_public), 0, 0, 1, 1},
   {&__pyx_n_s_public_key, __pyx_k_public_key, sizeof(__pyx_k_public_key), 0, 0, 1, 1},
   {&__pyx_n_s_public_key_compute, __pyx_k_public_key_compute, sizeof(__pyx_k_public_key_compute), 0, 0, 1, 1},
   {&__pyx_n_u_pymonocypher, __pyx_k_pymonocypher, sizeof(__pyx_k_pymonocypher), 0, 1, 0, 1},
+  {&__pyx_n_s_randbits, __pyx_k_randbits, sizeof(__pyx_k_randbits), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
   {&__pyx_n_s_rv, __pyx_k_rv, sizeof(__pyx_k_rv), 0, 0, 1, 1},
   {&__pyx_n_s_salt, __pyx_k_salt, sizeof(__pyx_k_salt), 0, 0, 1, 1},
   {&__pyx_n_s_secret, __pyx_k_secret, sizeof(__pyx_k_secret), 0, 0, 1, 1},
   {&__pyx_n_s_secret_key, __pyx_k_secret_key, sizeof(__pyx_k_secret_key), 0, 0, 1, 1},
   {&__pyx_n_s_secrets, __pyx_k_secrets, sizeof(__pyx_k_secrets), 0, 0, 1, 1},
   {&__pyx_n_u_secrets, __pyx_k_secrets, sizeof(__pyx_k_secrets), 0, 1, 0, 1},
+  {&__pyx_n_s_seed, __pyx_k_seed, sizeof(__pyx_k_seed), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_sig, __pyx_k_sig, sizeof(__pyx_k_sig), 0, 0, 1, 1},
   {&__pyx_n_s_signature, __pyx_k_signature, sizeof(__pyx_k_signature), 0, 0, 1, 1},
   {&__pyx_n_s_signature_check, __pyx_k_signature_check, sizeof(__pyx_k_signature_check), 0, 0, 1, 1},
   {&__pyx_n_s_signature_sign, __pyx_k_signature_sign, sizeof(__pyx_k_signature_sign), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_their_public_key, __pyx_k_their_public_key, sizeof(__pyx_k_their_public_key), 0, 0, 1, 1},
   {&__pyx_n_s_title, __pyx_k_title, sizeof(__pyx_k_title), 0, 0, 1, 1},
   {&__pyx_n_s_token_bytes, __pyx_k_token_bytes, sizeof(__pyx_k_token_bytes), 0, 0, 1, 1},
+  {&__pyx_n_s_tweak, __pyx_k_tweak, sizeof(__pyx_k_tweak), 0, 0, 1, 1},
   {&__pyx_n_s_unlock, __pyx_k_unlock, sizeof(__pyx_k_unlock), 0, 0, 1, 1},
   {&__pyx_kp_u_unsupported_method_s, __pyx_k_unsupported_method_s, sizeof(__pyx_k_unsupported_method_s), 0, 1, 0, 0},
   {&__pyx_n_s_url, __pyx_k_url, sizeof(__pyx_k_url), 0, 0, 1, 1},
   {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_n_s_version, __pyx_k_version, sizeof(__pyx_k_version), 0, 0, 1, 1},
   {&__pyx_n_s_warn, __pyx_k_warn, sizeof(__pyx_k_warn), 0, 0, 1, 1},
   {&__pyx_n_s_warnings, __pyx_k_warnings, sizeof(__pyx_k_warnings), 0, 0, 1, 1},
@@ -6598,227 +7455,275 @@
  *     return generate_signing_key_pair()
  * 
  */
   __pyx_tuple__11 = PyTuple_Pack(2, __pyx_kp_u_deprecated_use_generate_signing, __pyx_builtin_DeprecationWarning); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 606, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__11);
   __Pyx_GIVEREF(__pyx_tuple__11);
 
+  /* "monocypher.pyx":656
+ *     rv = crypto_curve_to_hidden(hidden, curve, tweak)
+ *     if rv:
+ *         raise ValueError('curve point is unsuitable for hiding')             # <<<<<<<<<<<<<<
+ *     return hidden
+ * 
+ */
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_u_curve_point_is_unsuitable_for_hi); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 656, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
+
   /* "cfunc.to_py":65
  * @cname("__Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py")
  * cdef object __Pyx_CFunc_int____const__uint8__t________const__uint8__t_______to_py(int (*f)(const uint8_t *, const uint8_t *) except *):
  *     def wrap(const uint8_t * a, const uint8_t * b):             # <<<<<<<<<<<<<<
  *         """wrap(a: 'const uint8_t *', b: 'const uint8_t *') -> 'int'"""
  *         return f(a, b)
  */
-  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(1, 65, __pyx_L1_error)
-  __pyx_tuple__14 = PyTuple_Pack(2, __pyx_n_s_public_key, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 65, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(2, __pyx_n_s_public_key, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 65, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_wrap, 65, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(1, 65, __pyx_L1_error)
 
   /* "monocypher.pyx":312
  *                                const uint8_t curve_point[32])
  * 
  * def wipe(data):             # <<<<<<<<<<<<<<
  *     """Wipe a bytes object from memory.
  * 
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_n_s_data); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(0, 312, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
-  __pyx_codeobj__17 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_wipe, 312, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__17)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_n_s_data); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 312, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_wipe, 312, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 312, __pyx_L1_error)
 
   /* "monocypher.pyx":323
  * 
  * 
  * def lock(key, nonce, message, associated_data=None):             # <<<<<<<<<<<<<<
  *     """Perform authenticated encryption.
  * 
  */
-  __pyx_tuple__18 = PyTuple_Pack(6, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_mac, __pyx_n_s_crypto_text); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(0, 323, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(4, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__18, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_lock, 323, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __pyx_tuple__19 = PyTuple_Pack(6, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_mac, __pyx_n_s_crypto_text); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(0, 323, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(4, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__19, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_lock, 323, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 323, __pyx_L1_error)
 
   /* "monocypher.pyx":344
  * 
  * 
  * def unlock(key, nonce, mac, message, associated_data=None):             # <<<<<<<<<<<<<<
  *     """Perform authenticated decryption.
  * 
  */
-  __pyx_tuple__20 = PyTuple_Pack(7, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_mac, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_plain_text, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(0, 344, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(5, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_unlock, 344, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 344, __pyx_L1_error)
+  __pyx_tuple__21 = PyTuple_Pack(7, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_mac, __pyx_n_s_message, __pyx_n_s_associated_data, __pyx_n_s_plain_text, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(0, 344, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(5, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__21, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_unlock, 344, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 344, __pyx_L1_error)
 
   /* "monocypher.pyx":366
  * 
  * 
  * def chacha20(key, nonce, message):             # <<<<<<<<<<<<<<
  *     """Encrypt/Decrypt a message with ChaCha20.
  * 
  */
-  __pyx_tuple__22 = PyTuple_Pack(4, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message, __pyx_n_s_result); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 366, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
-  __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_chacha20, 366, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_tuple__23 = PyTuple_Pack(4, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message, __pyx_n_s_result); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
+  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__23, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_chacha20, 366, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 366, __pyx_L1_error)
 
   /* "monocypher.pyx":385
  * 
  * 
  * def blake2b(msg, key=None):             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     if isinstance(msg, str):
  */
-  __pyx_tuple__24 = PyTuple_Pack(3, __pyx_n_s_msg, __pyx_n_s_key, __pyx_n_s_hash); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 385, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_blake2b, 385, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 385, __pyx_L1_error)
+  __pyx_tuple__25 = PyTuple_Pack(3, __pyx_n_s_msg, __pyx_n_s_key, __pyx_n_s_hash); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(0, 385, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_blake2b, 385, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(0, 385, __pyx_L1_error)
 
   /* "monocypher.pyx":425
  * 
  * 
  * def argon2i_32(nb_blocks, nb_iterations, password, salt, key=None, ad=None):             # <<<<<<<<<<<<<<
  *     key = b'' if key is None else key
  *     ad = b'' if ad is None else ad
  */
-  __pyx_tuple__26 = PyTuple_Pack(8, __pyx_n_s_nb_blocks, __pyx_n_s_nb_iterations, __pyx_n_s_password, __pyx_n_s_salt, __pyx_n_s_key, __pyx_n_s_ad, __pyx_n_s_hash, __pyx_n_s_work_area); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 425, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(6, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_argon2i_32, 425, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(8, __pyx_n_s_nb_blocks, __pyx_n_s_nb_iterations, __pyx_n_s_password, __pyx_n_s_salt, __pyx_n_s_key, __pyx_n_s_ad, __pyx_n_s_hash, __pyx_n_s_work_area); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 425, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(6, 0, 8, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_argon2i_32, 425, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 425, __pyx_L1_error)
 
   /* "monocypher.pyx":445
  * 
  * 
  * def compute_key_exchange_public_key(secret_key):             # <<<<<<<<<<<<<<
  *     """Generate the public key for key exchange from the secret key.
  * 
  */
-  __pyx_tuple__28 = PyTuple_Pack(2, __pyx_n_s_secret_key, __pyx_n_s_public_key); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 445, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_key_exchange_public_key, 445, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 445, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(2, __pyx_n_s_secret_key, __pyx_n_s_public_key); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 445, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__29);
+  __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_key_exchange_public_key, 445, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 445, __pyx_L1_error)
 
   /* "monocypher.pyx":456
  * 
  * 
  * def key_exchange(your_secret_key, their_public_key):             # <<<<<<<<<<<<<<
  *     """Compute a shared secret based upon public-key crytography.
  * 
  */
-  __pyx_tuple__30 = PyTuple_Pack(3, __pyx_n_s_your_secret_key, __pyx_n_s_their_public_key, __pyx_n_s_p); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 456, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_key_exchange, 456, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 456, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(3, __pyx_n_s_your_secret_key, __pyx_n_s_their_public_key, __pyx_n_s_p); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 456, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_key_exchange, 456, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 456, __pyx_L1_error)
 
   /* "monocypher.pyx":469
  * 
  * 
  * def compute_signing_public_key(secret_key):             # <<<<<<<<<<<<<<
  *     """Generate the public key from the secret key.
  * 
  */
-  __pyx_tuple__32 = PyTuple_Pack(2, __pyx_n_s_secret_key, __pyx_n_s_public_key); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 469, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_signing_public_key, 469, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(2, __pyx_n_s_secret_key, __pyx_n_s_public_key); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_compute_signing_public_key, 469, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 469, __pyx_L1_error)
 
   /* "monocypher.pyx":480
  * 
  * 
  * def public_key_compute(secret_key):             # <<<<<<<<<<<<<<
  *     warnings.warn("deprecated: use compute_signing_public_key", DeprecationWarning)
  *     return compute_signing_public_key(secret_key)
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 480, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_public_key_compute, 480, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 480, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_public_key_compute, 480, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 480, __pyx_L1_error)
 
   /* "monocypher.pyx":485
  * 
  * 
  * def signature_sign(secret_key, message):             # <<<<<<<<<<<<<<
  *     """Cryptographically sign a messge.
  * 
  */
-  __pyx_tuple__36 = PyTuple_Pack(4, __pyx_n_s_secret_key, __pyx_n_s_message, __pyx_n_s_sig, __pyx_n_s_kp); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(0, 485, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__36, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_sign, 485, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 485, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(4, __pyx_n_s_secret_key, __pyx_n_s_message, __pyx_n_s_sig, __pyx_n_s_kp); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 485, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_sign, 485, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 485, __pyx_L1_error)
 
   /* "monocypher.pyx":502
  * 
  * 
  * def signature_check(signature, public_key, message):             # <<<<<<<<<<<<<<
  *     """Verify the signature.
  * 
  */
-  __pyx_tuple__38 = PyTuple_Pack(3, __pyx_n_s_signature, __pyx_n_s_public_key, __pyx_n_s_message); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 502, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__38);
-  __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_check, 502, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_tuple__39 = PyTuple_Pack(3, __pyx_n_s_signature, __pyx_n_s_public_key, __pyx_n_s_message); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_codeobj__40 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__39, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_signature_check, 502, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__40)) __PYX_ERR(0, 502, __pyx_L1_error)
 
   /* "monocypher.pyx":563
  * 
  * 
  * def generate_key(length=None, method=None):             # <<<<<<<<<<<<<<
  *     """Generate a random key.
  * 
  */
-  __pyx_tuple__40 = PyTuple_Pack(5, __pyx_n_s_length, __pyx_n_s_method, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 563, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__40);
-  __Pyx_GIVEREF(__pyx_tuple__40);
-  __pyx_codeobj__41 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__40, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key, 563, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__41)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(5, __pyx_n_s_length, __pyx_n_s_method, __pyx_n_s_key, __pyx_n_s_nonce, __pyx_n_s_message); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 563, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(2, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key, 563, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 563, __pyx_L1_error)
 
   /* "monocypher.pyx":590
  * 
  * 
  * def generate_signing_key_pair():             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for signing using default settings.
  * 
  */
-  __pyx_tuple__42 = PyTuple_Pack(2, __pyx_n_s_secret, __pyx_n_s_public); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(0, 590, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__42);
-  __Pyx_GIVEREF(__pyx_tuple__42);
-  __pyx_codeobj__43 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__42, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_signing_key_pair, 590, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__43)) __PYX_ERR(0, 590, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(2, __pyx_n_s_secret, __pyx_n_s_public); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 590, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_signing_key_pair, 590, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 590, __pyx_L1_error)
 
   /* "monocypher.pyx":605
  * 
  * 
  * def generate_key_pair():             # <<<<<<<<<<<<<<
  *     warnings.warn("deprecated: use generate_signing_key_pair", DeprecationWarning)
  *     return generate_signing_key_pair()
  */
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key_pair, 605, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 605, __pyx_L1_error)
+  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key_pair, 605, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 605, __pyx_L1_error)
 
   /* "monocypher.pyx":610
  * 
  * 
  * def generate_key_exchange_key_pair():             # <<<<<<<<<<<<<<
  *     """Generate a new keypair for key exchange using default settings.
  * 
  */
-  __pyx_tuple__45 = PyTuple_Pack(2, __pyx_n_s_secret, __pyx_n_s_public); if (unlikely(!__pyx_tuple__45)) __PYX_ERR(0, 610, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__45);
-  __Pyx_GIVEREF(__pyx_tuple__45);
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__45, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key_exchange_key_pair, 610, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_tuple__46 = PyTuple_Pack(2, __pyx_n_s_secret, __pyx_n_s_public); if (unlikely(!__pyx_tuple__46)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__46);
+  __Pyx_GIVEREF(__pyx_tuple__46);
+  __pyx_codeobj__47 = (PyObject*)__Pyx_PyCode_New(0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__46, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_generate_key_exchange_key_pair, 610, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__47)) __PYX_ERR(0, 610, __pyx_L1_error)
+
+  /* "monocypher.pyx":623
+ * 
+ * 
+ * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
+ *     """Computes the point corresponding to a representative.
+ * 
+ */
+  __pyx_tuple__48 = PyTuple_Pack(2, __pyx_n_s_hidden, __pyx_n_s_curve); if (unlikely(!__pyx_tuple__48)) __PYX_ERR(0, 623, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__48);
+  __Pyx_GIVEREF(__pyx_tuple__48);
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__48, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_map, 623, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 623, __pyx_L1_error)
+
+  /* "monocypher.pyx":638
+ * 
+ * 
+ * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
+ *     """Computes the representative of a point.
+ * 
+ */
+  __pyx_tuple__50 = PyTuple_Pack(4, __pyx_n_s_curve, __pyx_n_s_tweak, __pyx_n_s_hidden, __pyx_n_s_rv); if (unlikely(!__pyx_tuple__50)) __PYX_ERR(0, 638, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__50);
+  __Pyx_GIVEREF(__pyx_tuple__50);
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(2, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__50, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_rev, 638, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 638, __pyx_L1_error)
+
+  /* "monocypher.pyx":660
+ * 
+ * 
+ * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
+ *     """Generate a key pair.
+ * 
+ */
+  __pyx_tuple__52 = PyTuple_Pack(3, __pyx_n_s_seed, __pyx_n_s_hidden, __pyx_n_s_secret_key); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__52);
+  __Pyx_GIVEREF(__pyx_tuple__52);
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(1, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_c_monocypher_pyx, __pyx_n_s_elligator_key_pair, 660, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 660, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_24 = PyInt_FromLong(24); if (unlikely(!__pyx_int_24)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_32 = PyInt_FromLong(32); if (unlikely(!__pyx_int_32)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_64 = PyInt_FromLong(64); if (unlikely(!__pyx_int_64)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1024 = PyInt_FromLong(1024); if (unlikely(!__pyx_int_1024)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
@@ -7093,15 +7998,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_monocypher) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -7166,31 +8071,31 @@
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_warnings, __pyx_t_1) < 0) __PYX_ERR(0, 12, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "monocypher.pyx":16
  * 
  * # also edit setup.py
- * __version__ = '3.1.3.1'   # also change setup.py             # <<<<<<<<<<<<<<
+ * __version__ = '3.1.3.2'   # also change setup.py             # <<<<<<<<<<<<<<
  * __title__ = 'pymonocypher'
  * __description__ = 'Python ctypes bindings to the Monocypher library'
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_3_1_3_1) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_3_1_3_2) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
 
   /* "monocypher.pyx":17
  * # also edit setup.py
- * __version__ = '3.1.3.1'   # also change setup.py
+ * __version__ = '3.1.3.2'   # also change setup.py
  * __title__ = 'pymonocypher'             # <<<<<<<<<<<<<<
  * __description__ = 'Python ctypes bindings to the Monocypher library'
  * __url__ = 'https://github.com/jetperch/pymonocypher'
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_title, __pyx_n_u_pymonocypher) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
 
   /* "monocypher.pyx":18
- * __version__ = '3.1.3.1'   # also change setup.py
+ * __version__ = '3.1.3.2'   # also change setup.py
  * __title__ = 'pymonocypher'
  * __description__ = 'Python ctypes bindings to the Monocypher library'             # <<<<<<<<<<<<<<
  * __url__ = 'https://github.com/jetperch/pymonocypher'
  * __author__ = 'Jetperch LLC'
  */
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_description, __pyx_kp_u_Python_ctypes_bindings_to_the_Mo) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
 
@@ -7427,14 +8332,50 @@
  * 
  */
   __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10monocypher_31generate_key_exchange_key_pair, NULL, __pyx_n_s_monocypher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_generate_key_exchange_key_pair, __pyx_t_1) < 0) __PYX_ERR(0, 610, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
+  /* "monocypher.pyx":623
+ * 
+ * 
+ * def elligator_map(hidden: bytes) -> bytes:             # <<<<<<<<<<<<<<
+ *     """Computes the point corresponding to a representative.
+ * 
+ */
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10monocypher_33elligator_map, NULL, __pyx_n_s_monocypher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 623, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_map, __pyx_t_1) < 0) __PYX_ERR(0, 623, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "monocypher.pyx":638
+ * 
+ * 
+ * def elligator_rev(curve: bytes, tweak=None) -> bytes:             # <<<<<<<<<<<<<<
+ *     """Computes the representative of a point.
+ * 
+ */
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10monocypher_35elligator_rev, NULL, __pyx_n_s_monocypher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 638, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_rev, __pyx_t_1) < 0) __PYX_ERR(0, 638, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "monocypher.pyx":660
+ * 
+ * 
+ * def elligator_key_pair(seed: bytes = None) -> tuple[bytes, bytes]:             # <<<<<<<<<<<<<<
+ *     """Generate a key pair.
+ * 
+ */
+  __pyx_t_1 = PyCFunction_NewEx(&__pyx_mdef_10monocypher_37elligator_key_pair, NULL, __pyx_n_s_monocypher); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_elligator_key_pair, __pyx_t_1) < 0) __PYX_ERR(0, 660, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
   /* "monocypher.pyx":1
  * """             # <<<<<<<<<<<<<<
  * Monocypher library Python bindings.
  * 
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -8060,28 +9001,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -8494,28 +9435,288 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
         }
     }
     return __Pyx_PyObject_Call(func, __pyx_empty_tuple, NULL);
 }
 #endif
 
+/* ArgTypeTest */
+static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact)
+{
+    if (unlikely(!type)) {
+        PyErr_SetString(PyExc_SystemError, "Missing type object");
+        return 0;
+    }
+    else if (exact) {
+        #if PY_MAJOR_VERSION == 2
+        if ((type == &PyBaseString_Type) && likely(__Pyx_PyBaseString_CheckExact(obj))) return 1;
+        #endif
+    }
+    else {
+        if (likely(__Pyx_TypeCheck(obj, type))) return 1;
+    }
+    PyErr_Format(PyExc_TypeError,
+        "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
+        name, type->tp_name, Py_TYPE(obj)->tp_name);
+    return 0;
+}
+
+/* CIntToDigits */
+static const char DIGIT_PAIRS_10[2*10*10+1] = {
+    "00010203040506070809"
+    "10111213141516171819"
+    "20212223242526272829"
+    "30313233343536373839"
+    "40414243444546474849"
+    "50515253545556575859"
+    "60616263646566676869"
+    "70717273747576777879"
+    "80818283848586878889"
+    "90919293949596979899"
+};
+static const char DIGIT_PAIRS_8[2*8*8+1] = {
+    "0001020304050607"
+    "1011121314151617"
+    "2021222324252627"
+    "3031323334353637"
+    "4041424344454647"
+    "5051525354555657"
+    "6061626364656667"
+    "7071727374757677"
+};
+static const char DIGITS_HEX[2*16+1] = {
+    "0123456789abcdef"
+    "0123456789ABCDEF"
+};
+
+/* BuildPyUnicode */
+static PyObject* __Pyx_PyUnicode_BuildFromAscii(Py_ssize_t ulength, char* chars, int clength,
+                                                int prepend_sign, char padding_char) {
+    PyObject *uval;
+    Py_ssize_t uoffset = ulength - clength;
+#if CYTHON_USE_UNICODE_INTERNALS
+    Py_ssize_t i;
+#if CYTHON_PEP393_ENABLED
+    void *udata;
+    uval = PyUnicode_New(ulength, 127);
+    if (unlikely(!uval)) return NULL;
+    udata = PyUnicode_DATA(uval);
+#else
+    Py_UNICODE *udata;
+    uval = PyUnicode_FromUnicode(NULL, ulength);
+    if (unlikely(!uval)) return NULL;
+    udata = PyUnicode_AS_UNICODE(uval);
+#endif
+    if (uoffset > 0) {
+        i = 0;
+        if (prepend_sign) {
+            __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, 0, '-');
+            i++;
+        }
+        for (; i < uoffset; i++) {
+            __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, i, padding_char);
+        }
+    }
+    for (i=0; i < clength; i++) {
+        __Pyx_PyUnicode_WRITE(PyUnicode_1BYTE_KIND, udata, uoffset+i, chars[i]);
+    }
+#else
+    {
+        PyObject *sign = NULL, *padding = NULL;
+        uval = NULL;
+        if (uoffset > 0) {
+            prepend_sign = !!prepend_sign;
+            if (uoffset > prepend_sign) {
+                padding = PyUnicode_FromOrdinal(padding_char);
+                if (likely(padding) && uoffset > prepend_sign + 1) {
+                    PyObject *tmp;
+                    PyObject *repeat = PyInt_FromSsize_t(uoffset - prepend_sign);
+                    if (unlikely(!repeat)) goto done_or_error;
+                    tmp = PyNumber_Multiply(padding, repeat);
+                    Py_DECREF(repeat);
+                    Py_DECREF(padding);
+                    padding = tmp;
+                }
+                if (unlikely(!padding)) goto done_or_error;
+            }
+            if (prepend_sign) {
+                sign = PyUnicode_FromOrdinal('-');
+                if (unlikely(!sign)) goto done_or_error;
+            }
+        }
+        uval = PyUnicode_DecodeASCII(chars, clength, NULL);
+        if (likely(uval) && padding) {
+            PyObject *tmp = PyNumber_Add(padding, uval);
+            Py_DECREF(uval);
+            uval = tmp;
+        }
+        if (likely(uval) && sign) {
+            PyObject *tmp = PyNumber_Add(sign, uval);
+            Py_DECREF(uval);
+            uval = tmp;
+        }
+done_or_error:
+        Py_XDECREF(padding);
+        Py_XDECREF(sign);
+    }
+#endif
+    return uval;
+}
+
+/* CIntToPyUnicode */
+static CYTHON_INLINE PyObject* __Pyx_PyUnicode_From_Py_ssize_t(Py_ssize_t value, Py_ssize_t width, char padding_char, char format_char) {
+    char digits[sizeof(Py_ssize_t)*3+2];
+    char *dpos, *end = digits + sizeof(Py_ssize_t)*3+2;
+    const char *hex_digits = DIGITS_HEX;
+    Py_ssize_t length, ulength;
+    int prepend_sign, last_one_off;
+    Py_ssize_t remaining;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const Py_ssize_t neg_one = (Py_ssize_t) -1, const_zero = (Py_ssize_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (format_char == 'X') {
+        hex_digits += 16;
+        format_char = 'x';
+    }
+    remaining = value;
+    last_one_off = 0;
+    dpos = end;
+    do {
+        int digit_pos;
+        switch (format_char) {
+        case 'o':
+            digit_pos = abs((int)(remaining % (8*8)));
+            remaining = (Py_ssize_t) (remaining / (8*8));
+            dpos -= 2;
+            memcpy(dpos, DIGIT_PAIRS_8 + digit_pos * 2, 2);
+            last_one_off = (digit_pos < 8);
+            break;
+        case 'd':
+            digit_pos = abs((int)(remaining % (10*10)));
+            remaining = (Py_ssize_t) (remaining / (10*10));
+            dpos -= 2;
+            memcpy(dpos, DIGIT_PAIRS_10 + digit_pos * 2, 2);
+            last_one_off = (digit_pos < 10);
+            break;
+        case 'x':
+            *(--dpos) = hex_digits[abs((int)(remaining % 16))];
+            remaining = (Py_ssize_t) (remaining / 16);
+            break;
+        default:
+            assert(0);
+            break;
+        }
+    } while (unlikely(remaining != 0));
+    if (last_one_off) {
+        assert(*dpos == '0');
+        dpos++;
+    }
+    length = end - dpos;
+    ulength = length;
+    prepend_sign = 0;
+    if (!is_unsigned && value <= neg_one) {
+        if (padding_char == ' ' || width <= length + 1) {
+            *(--dpos) = '-';
+            ++length;
+        } else {
+            prepend_sign = 1;
+        }
+        ++ulength;
+    }
+    if (width > ulength) {
+        ulength = width;
+    }
+    if (ulength == 1) {
+        return PyUnicode_FromOrdinal(*dpos);
+    }
+    return __Pyx_PyUnicode_BuildFromAscii(ulength, dpos, (int) length, prepend_sign, padding_char);
+}
+
+/* JoinPyUnicode */
+static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
+                                      CYTHON_UNUSED Py_UCS4 max_char) {
+#if CYTHON_USE_UNICODE_INTERNALS && CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    PyObject *result_uval;
+    int result_ukind;
+    Py_ssize_t i, char_pos;
+    void *result_udata;
+#if CYTHON_PEP393_ENABLED
+    result_uval = PyUnicode_New(result_ulength, max_char);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = (max_char <= 255) ? PyUnicode_1BYTE_KIND : (max_char <= 65535) ? PyUnicode_2BYTE_KIND : PyUnicode_4BYTE_KIND;
+    result_udata = PyUnicode_DATA(result_uval);
+#else
+    result_uval = PyUnicode_FromUnicode(NULL, result_ulength);
+    if (unlikely(!result_uval)) return NULL;
+    result_ukind = sizeof(Py_UNICODE);
+    result_udata = PyUnicode_AS_UNICODE(result_uval);
+#endif
+    char_pos = 0;
+    for (i=0; i < value_count; i++) {
+        int ukind;
+        Py_ssize_t ulength;
+        void *udata;
+        PyObject *uval = PyTuple_GET_ITEM(value_tuple, i);
+        if (unlikely(__Pyx_PyUnicode_READY(uval)))
+            goto bad;
+        ulength = __Pyx_PyUnicode_GET_LENGTH(uval);
+        if (unlikely(!ulength))
+            continue;
+        if (unlikely(char_pos + ulength < 0))
+            goto overflow;
+        ukind = __Pyx_PyUnicode_KIND(uval);
+        udata = __Pyx_PyUnicode_DATA(uval);
+        if (!CYTHON_PEP393_ENABLED || ukind == result_ukind) {
+            memcpy((char *)result_udata + char_pos * result_ukind, udata, (size_t) (ulength * result_ukind));
+        } else {
+            #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030300F0 || defined(_PyUnicode_FastCopyCharacters)
+            _PyUnicode_FastCopyCharacters(result_uval, char_pos, uval, 0, ulength);
+            #else
+            Py_ssize_t j;
+            for (j=0; j < ulength; j++) {
+                Py_UCS4 uchar = __Pyx_PyUnicode_READ(ukind, udata, j);
+                __Pyx_PyUnicode_WRITE(result_ukind, result_udata, char_pos+j, uchar);
+            }
+            #endif
+        }
+        char_pos += ulength;
+    }
+    return result_uval;
+overflow:
+    PyErr_SetString(PyExc_OverflowError, "join() result is too long for a Python string");
+bad:
+    Py_DECREF(result_uval);
+    return NULL;
+#else
+    result_ulength++;
+    value_count++;
+    return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
+#endif
+}
+
 /* FetchCommonType */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
     PyObject* fake_module;
     PyTypeObject* cached_type = NULL;
     fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
     if (!fake_module) return NULL;
     Py_INCREF(fake_module);
@@ -9044,17 +10245,22 @@
         argc = PyTuple_GET_SIZE(args);
         new_args = PyTuple_GetSlice(args, 1, argc);
         if (unlikely(!new_args))
             return NULL;
         self = PyTuple_GetItem(args, 0);
         if (unlikely(!self)) {
             Py_DECREF(new_args);
+#if PY_MAJOR_VERSION > 2
             PyErr_Format(PyExc_TypeError,
                          "unbound method %.200S() needs an argument",
                          cyfunc->func_qualname);
+#else
+            PyErr_SetString(PyExc_TypeError,
+                            "unbound method needs an argument");
+#endif
             return NULL;
         }
         result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
         Py_DECREF(new_args);
     } else {
         result = __Pyx_CyFunction_Call(func, args, kw);
     }
@@ -9121,15 +10327,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -9439,15 +10648,15 @@
     Py_XDECREF(empty_list);
     Py_XDECREF(empty_dict);
     return module;
 }
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -9786,15 +10995,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -9982,15 +11191,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -10178,15 +11387,15 @@
                         } else if (8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT) {
                             return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -10314,14 +11523,210 @@
     return (uint32_t) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to uint32_t");
     return (uint32_t) -1;
 }
 
+/* CIntFromPy */
+static CYTHON_INLINE uint8_t __Pyx_PyInt_As_uint8_t(PyObject *x) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const uint8_t neg_one = (uint8_t) -1, const_zero = (uint8_t) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+#if PY_MAJOR_VERSION < 3
+    if (likely(PyInt_Check(x))) {
+        if (sizeof(uint8_t) < sizeof(long)) {
+            __PYX_VERIFY_RETURN_INT(uint8_t, long, PyInt_AS_LONG(x))
+        } else {
+            long val = PyInt_AS_LONG(x);
+            if (is_unsigned && unlikely(val < 0)) {
+                goto raise_neg_overflow;
+            }
+            return (uint8_t) val;
+        }
+    } else
+#endif
+    if (likely(PyLong_Check(x))) {
+        if (is_unsigned) {
+#if CYTHON_USE_PYLONG_INTERNALS
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (uint8_t) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(uint8_t, digit, digits[0])
+                case 2:
+                    if (8 * sizeof(uint8_t) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(uint8_t) >= 2 * PyLong_SHIFT) {
+                            return (uint8_t) (((((uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
+                        }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(uint8_t) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(uint8_t) >= 3 * PyLong_SHIFT) {
+                            return (uint8_t) (((((((uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
+                        }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(uint8_t) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(uint8_t) >= 4 * PyLong_SHIFT) {
+                            return (uint8_t) (((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0]));
+                        }
+                    }
+                    break;
+            }
+#endif
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+            if (unlikely(Py_SIZE(x) < 0)) {
+                goto raise_neg_overflow;
+            }
+#else
+            {
+                int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
+                if (unlikely(result < 0))
+                    return (uint8_t) -1;
+                if (unlikely(result == 1))
+                    goto raise_neg_overflow;
+            }
+#endif
+            if (sizeof(uint8_t) <= sizeof(unsigned long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(uint8_t, unsigned long, PyLong_AsUnsignedLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if (sizeof(uint8_t) <= sizeof(unsigned PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(uint8_t, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
+#endif
+            }
+        } else {
+#if CYTHON_USE_PYLONG_INTERNALS
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (uint8_t) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(uint8_t, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(uint8_t,  digit, +digits[0])
+                case -2:
+                    if (8 * sizeof(uint8_t) - 1 > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(uint8_t) - 1 > 2 * PyLong_SHIFT) {
+                            return (uint8_t) (((uint8_t)-1)*(((((uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+                case 2:
+                    if (8 * sizeof(uint8_t) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(uint8_t) - 1 > 2 * PyLong_SHIFT) {
+                            return (uint8_t) ((((((uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+                case -3:
+                    if (8 * sizeof(uint8_t) - 1 > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(uint8_t) - 1 > 3 * PyLong_SHIFT) {
+                            return (uint8_t) (((uint8_t)-1)*(((((((uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(uint8_t) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(uint8_t) - 1 > 3 * PyLong_SHIFT) {
+                            return (uint8_t) ((((((((uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+                case -4:
+                    if (8 * sizeof(uint8_t) - 1 > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(uint8_t) - 1 > 4 * PyLong_SHIFT) {
+                            return (uint8_t) (((uint8_t)-1)*(((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(uint8_t) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(uint8_t, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(uint8_t) - 1 > 4 * PyLong_SHIFT) {
+                            return (uint8_t) ((((((((((uint8_t)digits[3]) << PyLong_SHIFT) | (uint8_t)digits[2]) << PyLong_SHIFT) | (uint8_t)digits[1]) << PyLong_SHIFT) | (uint8_t)digits[0])));
+                        }
+                    }
+                    break;
+            }
+#endif
+            if (sizeof(uint8_t) <= sizeof(long)) {
+                __PYX_VERIFY_RETURN_INT_EXC(uint8_t, long, PyLong_AsLong(x))
+#ifdef HAVE_LONG_LONG
+            } else if (sizeof(uint8_t) <= sizeof(PY_LONG_LONG)) {
+                __PYX_VERIFY_RETURN_INT_EXC(uint8_t, PY_LONG_LONG, PyLong_AsLongLong(x))
+#endif
+            }
+        }
+        {
+#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
+            PyErr_SetString(PyExc_RuntimeError,
+                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
+#else
+            uint8_t val;
+            PyObject *v = __Pyx_PyNumber_IntOrLong(x);
+ #if PY_MAJOR_VERSION < 3
+            if (likely(v) && !PyLong_Check(v)) {
+                PyObject *tmp = v;
+                v = PyNumber_Long(tmp);
+                Py_DECREF(tmp);
+            }
+ #endif
+            if (likely(v)) {
+                int one = 1; int is_little = (int)*(unsigned char *)&one;
+                unsigned char *bytes = (unsigned char *)&val;
+                int ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                              bytes, sizeof(val),
+                                              is_little, !is_unsigned);
+                Py_DECREF(v);
+                if (likely(!ret))
+                    return val;
+            }
+#endif
+            return (uint8_t) -1;
+        }
+    } else {
+        uint8_t val;
+        PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
+        if (!tmp) return (uint8_t) -1;
+        val = __Pyx_PyInt_As_uint8_t(tmp);
+        Py_DECREF(tmp);
+        return val;
+    }
+raise_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "value too large to convert to uint8_t");
+    return (uint8_t) -1;
+raise_neg_overflow:
+    PyErr_SetString(PyExc_OverflowError,
+        "can't convert negative value to uint8_t");
+    return (uint8_t) -1;
+}
+
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -10412,15 +11817,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `pymonocypher-3.1.3.1/monocypher.c` & `pymonocypher-3.1.3.2/monocypher.c`

 * *Files identical despite different names*

### Comparing `pymonocypher-3.1.3.1/monocypher.h` & `pymonocypher-3.1.3.2/monocypher.h`

 * *Files identical despite different names*

### Comparing `pymonocypher-3.1.3.1/pymonocypher.egg-info/PKG-INFO` & `pymonocypher-3.1.3.2/pymonocypher.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-Metadata-Version: 2.1
-Name: pymonocypher
-Version: 3.1.3.1
-Summary: Python ctypes bindings to the Monocypher library
-Home-page: https://github.com/jetperch/pymonocypher
-Author: Jetperch LLC
-Author-email: joulescope-dev@jetperch.com
-License: BSD 2-clause
-Project-URL: Bug Reports, https://github.com/jetperch/pymonocypher/issues
-Project-URL: Source, https://github.com/jetperch/pymonocypher/
-Keywords: cryto cryptography monocypher chacha blake2b 25519
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Natural Language :: English
-Classifier: Topic :: Security :: Cryptography
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: C
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-
-# pymonocypher
-
-This python package uses cython to wrap the Monocypher C library. 
-Monocypher is an easy to use, easy to deploy, auditable crypto library
-written in portable C.  
-
-Normal Python installations have access to a wide
-selection of quality crypto libraries.  This python binding is intended to
-communicate with other implementations that do use the Monocypher library.
-A typical application is to communicate with a microcontroller that 
-uses Monocypher.
-
-*   pymonocypher [Source code](https://github.com/jetperch/pymonocypher)
-*   Monocypher [official site](https://monocypher.org/)
-
-The Python binding API mirrors the underlying C API, but with 
-simplifications to only pass bytes objects, not uint8_t * and length.
-
-
-## Installation
-
-You can install directly from pypi:
-
-    pip install pymonocypher
-    
-You can then use pymonocypher:
-
-    python
-    >>> import monocypher
-    >>> monocypher.blake2b(b'hello world')
-
+Metadata-Version: 2.1
+Name: pymonocypher
+Version: 3.1.3.2
+Summary: Python ctypes bindings to the Monocypher library
+Home-page: https://github.com/jetperch/pymonocypher
+Author: Jetperch LLC
+Author-email: joulescope-dev@jetperch.com
+License: BSD 2-clause
+Project-URL: Bug Reports, https://github.com/jetperch/pymonocypher/issues
+Project-URL: Source, https://github.com/jetperch/pymonocypher/
+Keywords: cryto cryptography monocypher chacha blake2b 25519
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
+Classifier: Natural Language :: English
+Classifier: Topic :: Security :: Cryptography
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: C
+Requires-Python: ~=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+
+# pymonocypher
+
+This python package uses cython to wrap the Monocypher C library. 
+Monocypher is an easy to use, easy to deploy, auditable crypto library
+written in portable C.  
+
+Normal Python installations have access to a wide
+selection of quality crypto libraries.  This python binding is intended to
+communicate with other implementations that do use the Monocypher library.
+A typical application is to communicate with a microcontroller that 
+uses Monocypher.
+
+*   pymonocypher [Source code](https://github.com/jetperch/pymonocypher)
+*   Monocypher [official site](https://monocypher.org/)
+
+The Python binding API mirrors the underlying C API, but with 
+simplifications to only pass bytes objects, not uint8_t * and length.
+
+
+## Installation
+
+You can install directly from pypi:
+
+    pip install pymonocypher
+    
+You can then use pymonocypher:
+
+    python
+    >>> import monocypher
+    >>> monocypher.blake2b(b'hello world')
+
```

### Comparing `pymonocypher-3.1.3.1/setup.py` & `pymonocypher-3.1.3.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,86 @@
-"""
-pymonocypher
-"""
-
-# See:
-# https://packaging.python.org/en/latest/distributing.html
-# https://github.com/pypa/sampleproject
-
-
-import setuptools
-import os
-
-MYPATH = os.path.abspath(os.path.dirname(__file__))
-VERSION = '3.1.3.1'  # also change c_monocypher.pyx
-
-
-try:
-    from Cython.Build import cythonize
-    USE_CYTHON = os.path.isfile(os.path.join(MYPATH, 'c_monocypher.pyx'))
-except ImportError:
-    USE_CYTHON = False
-
-
-ext = '.pyx' if USE_CYTHON else '.c'
-extensions = [
-    setuptools.Extension('monocypher',
-        sources=['c_monocypher' + ext, 'monocypher.c'],
-        include_dirs=['.'],
-        extra_compile_args=['-DBLAKE2_NO_UNROLLING'],
-    ),
-]
-
-if USE_CYTHON:
-    from Cython.Build import cythonize
-    extensions = cythonize(
-        extensions, 
-        compiler_directives={'language_level': '3'})
-
-
-# Get the long description from the README file
-with open(os.path.join(MYPATH, 'README.md'), 'r', encoding='utf-8') as f:
-    long_description = f.read()
-
-
-setuptools.setup(
-    # also edit c_monocypher.pyx
-    name='pymonocypher',
-    version=VERSION,
-    description='Python ctypes bindings to the Monocypher library',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    url='https://github.com/jetperch/pymonocypher',
-    author='Jetperch LLC',
-    author_email='joulescope-dev@jetperch.com',
-    license='BSD 2-clause',
-
-    # Classifiers help users find your project by categorizing it.
-    #
-    # For a list of valid classifiers, see https://pypi.org/classifiers/
-    classifiers=[  # Optional
-        'Development Status :: 5 - Production/Stable',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication',
-        'Natural Language :: English',
-        'Topic :: Security :: Cryptography',
-
-        # Supported Python versions
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: C',
-    ],
-
-    keywords='cryto cryptography monocypher chacha blake2b 25519',
-    install_requires=[],
-    ext_modules=extensions,
-
-    project_urls={
-        'Bug Reports': 'https://github.com/jetperch/pymonocypher/issues',
-        'Source': 'https://github.com/jetperch/pymonocypher/',
-    },
-)
+"""
+pymonocypher
+"""
+
+# See:
+# https://packaging.python.org/en/latest/distributing.html
+# https://github.com/pypa/sampleproject
+
+
+import setuptools
+import os
+
+MYPATH = os.path.abspath(os.path.dirname(__file__))
+VERSION = '3.1.3.2'  # also change c_monocypher.pyx
+
+
+try:
+    from Cython.Build import cythonize
+    USE_CYTHON = os.path.isfile(os.path.join(MYPATH, 'c_monocypher.pyx'))
+except ImportError:
+    USE_CYTHON = False
+
+
+ext = '.pyx' if USE_CYTHON else '.c'
+extensions = [
+    setuptools.Extension('monocypher',
+        sources=['c_monocypher' + ext, 'monocypher.c'],
+        include_dirs=['.'],
+        extra_compile_args=['-DBLAKE2_NO_UNROLLING'],
+    ),
+]
+
+if USE_CYTHON:
+    from Cython.Build import cythonize
+    extensions = cythonize(
+        extensions, 
+        compiler_directives={'language_level': '3'})
+
+
+# Get the long description from the README file
+with open(os.path.join(MYPATH, 'README.md'), 'r', encoding='utf-8') as f:
+    long_description = f.read()
+
+
+setuptools.setup(
+    # also edit c_monocypher.pyx
+    name='pymonocypher',
+    version=VERSION,
+    description='Python ctypes bindings to the Monocypher library',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    url='https://github.com/jetperch/pymonocypher',
+    author='Jetperch LLC',
+    author_email='joulescope-dev@jetperch.com',
+    license='BSD 2-clause',
+
+    # Classifiers help users find your project by categorizing it.
+    #
+    # For a list of valid classifiers, see https://pypi.org/classifiers/
+    classifiers=[  # Optional
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'License :: OSI Approved :: BSD License',
+        'License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication',
+        'Natural Language :: English',
+        'Topic :: Security :: Cryptography',
+
+        # Supported Python versions
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: C',
+    ],
+
+    keywords='cryto cryptography monocypher chacha blake2b 25519',
+    install_requires=[
+        'numpy>=1.23',
+    ],
+    ext_modules=extensions,
+    python_requires='~=3.9',
+
+    project_urls={
+        'Bug Reports': 'https://github.com/jetperch/pymonocypher/issues',
+        'Source': 'https://github.com/jetperch/pymonocypher/',
+    },
+)
```

