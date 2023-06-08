# Comparing `tmp/pkilint-0.8.4.tar.gz` & `tmp/pkilint-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkilint-0.8.4.tar", last modified: Wed May 10 13:20:29 2023, max compression
+gzip compressed data, was "pkilint-0.8.5.tar", last modified: Thu Jun  8 14:19:30 2023, max compression
```

## Comparing `pkilint-0.8.4.tar` & `pkilint-0.8.5.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 13:20:20.000000 pkilint-0.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-10 13:20:29.015799 pkilint-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-05-10 13:20:20.000000 pkilint-0.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 13:20:20.000000 pkilint-0.8.4/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.007799 pkilint-0.8.4/pkilint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.007799 pkilint-0.8.4/pkilint/adobe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/adobe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/adobe/adobe_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.007799 pkilint-0.8.4/pkilint/adobe/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/adobe/asn1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/convert_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_cabf_serverauth_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_cabf_smime_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_pkix_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/cabf/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/cabf_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/cabf_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/cabf_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/cabf_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/cabf_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/cabf/servercert/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/cabf/servercert/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/asn1/ev_guidelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/servercert_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/servercert_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/servercert_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/servercert_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/cabf/smime/
--rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/smime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/smime/smime_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/smime/smime_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/smime/smime_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/smime/smime_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/etsi/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/etsi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/etsi/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/etsi/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/etsi/asn1/en_319_412_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/etsi/asn1/ts_119_495.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/iso/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/iso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/iso/lei.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/itu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/itu/bitstring.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/itu/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/itu/x520_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/msft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/msft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/msft/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/msft/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/msft/msft_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/oid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/pkilint/pkix/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/algorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/pkilint/pkix/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26221 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/certificate_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/certificate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/certificate_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/certificate_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/certificate_validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/pkilint/pkix/crl/
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/crl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/crl/crl_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/crl/crl_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/crl/crl_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/general_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/pkilint/pkix/ocsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/ocsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_basic_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.007799 pkilint-0.8.4/pkilint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-10 13:20:29.000000 pkilint-0.8.4/pkilint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-10 13:20:29.015799 pkilint-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 13:20:20.000000 pkilint-0.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/tests/integration_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/integration_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/integration_certificate/test_cabf_smime_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/integration_certificate/test_pkix_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/tests/itu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/itu/test_bitstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/itu/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.221162 pkilint-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-08 14:19:21.000000 pkilint-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-06-08 14:19:30.221162 pkilint-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-06-08 14:19:21.000000 pkilint-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 14:19:21.000000 pkilint-0.8.5/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.213162 pkilint-0.8.5/pkilint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.213162 pkilint-0.8.5/pkilint/adobe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/adobe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/adobe/adobe_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.213162 pkilint-0.8.5/pkilint/adobe/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/adobe/asn1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.213162 pkilint-0.8.5/pkilint/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/bin/convert_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/bin/lint_cabf_serverauth_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/bin/lint_cabf_smime_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/bin/lint_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/bin/lint_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/bin/lint_pkix_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.213162 pkilint-0.8.5/pkilint/cabf/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/cabf_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/cabf_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/cabf_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/cabf_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/cabf_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/cabf/servercert/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/servercert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/cabf/servercert/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/servercert/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/servercert/asn1/ev_guidelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/servercert/servercert_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/servercert/servercert_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/servercert/servercert_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/servercert/servercert_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/cabf/smime/
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/smime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/smime/smime_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/smime/smime_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/smime/smime_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/cabf/smime/smime_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/etsi/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/etsi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/etsi/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/etsi/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/etsi/asn1/en_319_412_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/etsi/asn1/ts_119_495.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/iso/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/iso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/iso/lei.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/itu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/itu/bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/itu/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/itu/x520_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/msft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/msft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/msft/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/msft/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/msft/msft_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/oid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/pkix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.217162 pkilint-0.8.5/pkilint/pkix/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26221 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/certificate/certificate_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/certificate/certificate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/certificate/certificate_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/certificate/certificate_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/certificate/certificate_validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.221162 pkilint-0.8.5/pkilint/pkix/crl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/crl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/crl/crl_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/crl/crl_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/crl/crl_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/general_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.221162 pkilint-0.8.5/pkilint/pkix/ocsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/ocsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/ocsp/ocsp_basic_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/ocsp/ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/ocsp/ocsp_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/pkix/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-06-08 14:19:21.000000 pkilint-0.8.5/pkilint/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.213162 pkilint-0.8.5/pkilint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-06-08 14:19:30.000000 pkilint-0.8.5/pkilint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-06-08 14:19:30.000000 pkilint-0.8.5/pkilint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:19:30.000000 pkilint-0.8.5/pkilint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-08 14:19:30.000000 pkilint-0.8.5/pkilint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 14:19:30.000000 pkilint-0.8.5/pkilint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 14:19:30.000000 pkilint-0.8.5/pkilint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:19:30.000000 pkilint-0.8.5/pkilint.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-08 14:19:30.221162 pkilint-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 14:19:21.000000 pkilint-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.221162 pkilint-0.8.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:21.000000 pkilint-0.8.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.221162 pkilint-0.8.5/tests/integration_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-08 14:19:21.000000 pkilint-0.8.5/tests/integration_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-08 14:19:21.000000 pkilint-0.8.5/tests/integration_certificate/test_cabf_smime_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-06-08 14:19:21.000000 pkilint-0.8.5/tests/integration_certificate/test_pkix_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:30.221162 pkilint-0.8.5/tests/itu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 14:19:21.000000 pkilint-0.8.5/tests/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-06-08 14:19:21.000000 pkilint-0.8.5/tests/itu/test_bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-06-08 14:19:21.000000 pkilint-0.8.5/tests/itu/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-08 14:19:21.000000 pkilint-0.8.5/tests/util.py
```

### Comparing `pkilint-0.8.4/LICENSE` & `pkilint-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/PKG-INFO` & `pkilint-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.8.4
+Version: 0.8.5
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pkilint-0.8.4/README.md` & `pkilint-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/adobe/adobe_validator.py` & `pkilint-0.8.5/pkilint/adobe/adobe_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/adobe/asn1/__init__.py` & `pkilint-0.8.5/pkilint/adobe/asn1/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/bin/convert_cert.py` & `pkilint-0.8.5/pkilint/bin/convert_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/bin/lint_cabf_serverauth_cert.py` & `pkilint-0.8.5/pkilint/bin/lint_cabf_serverauth_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/bin/lint_cabf_smime_cert.py` & `pkilint-0.8.5/pkilint/bin/lint_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/bin/lint_crl.py` & `pkilint-0.8.5/pkilint/bin/lint_crl.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/bin/lint_ocsp_response.py` & `pkilint-0.8.5/pkilint/bin/lint_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/bin/lint_pkix_cert.py` & `pkilint-0.8.5/pkilint/bin/lint_pkix_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/bin/lint_pkix_signer_signee_cert_chain.py` & `pkilint-0.8.5/pkilint/bin/lint_pkix_signer_signee_cert_chain.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/__init__.py` & `pkilint-0.8.5/pkilint/cabf/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/cabf_constants.py` & `pkilint-0.8.5/pkilint/cabf/cabf_constants.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     XG = 1
     ISO3166 = 2
 
 
 class RegistrationSchemeNamingConvention(typing.NamedTuple):
     country_identifier_type: RegistrationSchemeCountryIdentifierType
     allow_state_province: bool
+    require_registration_reference: bool
 
 
 REGISTRATION_SCHEMES = {
-    'NTR': RegistrationSchemeNamingConvention(RegistrationSchemeCountryIdentifierType.ISO3166, True),
-    'VAT': RegistrationSchemeNamingConvention(RegistrationSchemeCountryIdentifierType.ISO3166, False),
-    'PSD': RegistrationSchemeNamingConvention(RegistrationSchemeCountryIdentifierType.ISO3166, False),
+    'NTR': RegistrationSchemeNamingConvention(RegistrationSchemeCountryIdentifierType.ISO3166, True, True),
+    'VAT': RegistrationSchemeNamingConvention(RegistrationSchemeCountryIdentifierType.ISO3166, False, True),
+    'PSD': RegistrationSchemeNamingConvention(RegistrationSchemeCountryIdentifierType.ISO3166, False, True),
 }
```

### Comparing `pkilint-0.8.4/pkilint/cabf/cabf_crl.py` & `pkilint-0.8.5/pkilint/cabf/cabf_crl.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/cabf_extension.py` & `pkilint-0.8.5/pkilint/cabf/cabf_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/cabf_key.py` & `pkilint-0.8.5/pkilint/cabf/cabf_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/cabf_name.py` & `pkilint-0.8.5/pkilint/cabf/cabf_name.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                          value_path='value.x520countryName',
                          checked_validation=self.VALIDATION_INVALID_COUNTRY_CODE
                          )
 
 
 _ORG_ID_REGEX = re.compile(
     r'^(?P<scheme>[A-Z]{3})(?P<country>[a-zA-Z]{2})?(\+(?P<sp>[a-zA-Z0-9]{1,3}))?'
-    r'-(?P<reference>.+)$'
+    r'(-(?P<reference>.+))?$'
 )
 
 
 class OrganizationIdentifierAttributeValidator(validation.TypeMatchingValidator):
     VALIDATION_ORGANIZATION_ID_INVALID_ENCODING = validation.ValidationFinding(
         validation.ValidationFindingSeverity.ERROR,
         'cabf.invalid_subject_organization_identifier_encoding'
@@ -81,15 +81,15 @@
 
     VALIDATION_ORGANIZATION_ID_INVALID_SP_FORMAT = validation.ValidationFinding(
         validation.ValidationFindingSeverity.ERROR,
         'cabf.invalid_subject_organization_identifier_state_province_format'
     )
 
     def __init__(self, additional_schemes: typing.Optional[
-            typing.Mapping[str, cabf_constants.RegistrationSchemeNamingConvention]]=None):
+        typing.Mapping[str, cabf_constants.RegistrationSchemeNamingConvention]] = None):
         super().__init__(type_oid=x520_name.id_at_organizationIdentifier,
                          type_path='type', value_path='value.x520OrganizationIdentifier',
                          pdu_class=rfc5280.AttributeTypeAndValue,
                          validations=[
                              self.VALIDATION_ORGANIZATION_ID_INVALID_ENCODING,
                              self.VALIDATION_ORGANIZATION_ID_INVALID_FORMAT,
                              self.VALIDATION_ORGANIZATION_ID_INVALID_SCHEME,
@@ -124,14 +124,25 @@
 
         if scheme_info is None:
             raise validation.ValidationFindingEncountered(
                 self.VALIDATION_ORGANIZATION_ID_INVALID_SCHEME,
                 f'Invalid registration scheme: {m["scheme"]}'
             )
 
+        if scheme_info.require_registration_reference and m['reference'] is None:
+            raise validation.ValidationFindingEncountered(
+                self.VALIDATION_ORGANIZATION_ID_INVALID_FORMAT,
+                f'Missing Registration Reference: {value_node.pdu}'
+            )
+        elif not scheme_info.require_registration_reference and m['reference']:
+            raise validation.ValidationFindingEncountered(
+                self.VALIDATION_ORGANIZATION_ID_INVALID_FORMAT,
+                f'Prohibited Registration Reference is present: {value_node.pdu}'
+            )
+
         country_code = '' if m['country'] is None else m['country'].upper()
 
         if scheme_info.country_identifier_type == cabf_constants.RegistrationSchemeCountryIdentifierType.NONE:
             valid_country_code = (country_code == '')
         elif scheme_info.country_identifier_type == cabf_constants.RegistrationSchemeCountryIdentifierType.XG:
             valid_country_code = (country_code == 'XG')
         elif scheme_info.country_identifier_type == cabf_constants.RegistrationSchemeCountryIdentifierType.ISO3166:
@@ -198,19 +209,19 @@
             )
 
     def validate(self, node):
         domain_name = self.extract_domain_name(node)
 
         return self.validate_with_value(node, domain_name)
 
-        
+
 class GeneralNameDnsNameInternalDomainNameValidator(InternalDomainNameValidator):
     def __init__(self):
         super().__init__(predicate=general_name.create_generalname_type_predicate('dNSName'))
-        
+
     def validate_with_value(self, node, value):
         if len(value) == 0 and general_name.is_nameconstraints_child_node(node):
             return
         else:
             return super().validate_with_value(node, value)
 
 
@@ -230,15 +241,15 @@
         if general_name.is_nameconstraints_child_node(node):
             return str(node.pdu).lstrip('.')
         else:
             return urlparse(str(node.pdu)).netloc
 
     def validate_with_value(self, node, value):
         if len(value) == 0 and general_name.is_nameconstraints_child_node(node):
-                return
+            return
         else:
             return super().validate_with_value(node, value)
 
 
 class EmailAddressInternalDomainNameValidator(InternalDomainNameValidator):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `pkilint-0.8.4/pkilint/cabf/servercert/__init__.py` & `pkilint-0.8.5/pkilint/cabf/servercert/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/servercert/asn1/ev_guidelines.py` & `pkilint-0.8.5/pkilint/cabf/servercert/asn1/ev_guidelines.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/servercert/servercert_extension.py` & `pkilint-0.8.5/pkilint/cabf/servercert/servercert_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/servercert/servercert_key.py` & `pkilint-0.8.5/pkilint/cabf/servercert/servercert_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/servercert/servercert_name.py` & `pkilint-0.8.5/pkilint/cabf/servercert/servercert_name.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,15 @@
                     f'extension: {ext_sp}'
                 ))
 
         ext_reg_ref = str(ext.children['registrationReference'].pdu)
         if m['reference'] != ext_reg_ref:
             findings.append(validation.ValidationFindingDescription(
                 self.VALIDATION_CABF_ORG_ID_MISMATCHED_REFERENCE,
-                f'Mismatched registration reference: subject: {m["reference"]}'
+                f'Mismatched Registration Reference: subject: {m["reference"]}'
                 f', extension: {ext_reg_ref}'
             ))
 
         return validation.ValidationResult(self, node, findings)
 
 
 class EvSubscriberCertificateAllowedAttributesValidator(
```

### Comparing `pkilint-0.8.4/pkilint/cabf/smime/__init__.py` & `pkilint-0.8.5/pkilint/cabf/smime/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/smime/smime_constants.py` & `pkilint-0.8.5/pkilint/cabf/smime/smime_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/smime/smime_extension.py` & `pkilint-0.8.5/pkilint/cabf/smime/smime_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/smime/smime_key.py` & `pkilint-0.8.5/pkilint/cabf/smime/smime_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/cabf/smime/smime_name.py` & `pkilint-0.8.5/pkilint/cabf/smime/smime_name.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,23 +212,23 @@
         SubscriberSubjectValidator(validation_level, generation),
         SubjectAlternativeNameContainsSubjectEmailAddressesValidator(),
         cabf_name.ValidCountryValidator(),
         CommonNameValidator(validation_level, generation),
         OrganizationIdentifierAttributeValidator({
             'LEI': cabf_constants.RegistrationSchemeNamingConvention(
                 cabf_constants.RegistrationSchemeCountryIdentifierType.XG,
-                False
+                False, True
             ),
             'GOV': cabf_constants.RegistrationSchemeNamingConvention(
                 cabf_constants.RegistrationSchemeCountryIdentifierType.ISO3166,
-                True
+                True, False
             ),
             'INT': cabf_constants.RegistrationSchemeNamingConvention(
                 cabf_constants.RegistrationSchemeCountryIdentifierType.XG,
-                False
+                False, False
             )
         }),
         OrganizationIdentifierLeiValidator(),
         cabf_name.RelativeDistinguishedNameContainsOneElementValidator(),
     ]
 
     return certificate.create_subject_validator_container(
```

### Comparing `pkilint-0.8.4/pkilint/document.py` & `pkilint-0.8.5/pkilint/document.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/etsi/__init__.py` & `pkilint-0.8.5/pkilint/etsi/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/etsi/asn1/en_319_412_5.py` & `pkilint-0.8.5/pkilint/etsi/asn1/en_319_412_5.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/etsi/asn1/ts_119_495.py` & `pkilint-0.8.5/pkilint/etsi/asn1/ts_119_495.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/iso/lei.py` & `pkilint-0.8.5/pkilint/iso/lei.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/itu/bitstring.py` & `pkilint-0.8.5/pkilint/itu/bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/itu/string.py` & `pkilint-0.8.5/pkilint/itu/string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/itu/x520_name.py` & `pkilint-0.8.5/pkilint/itu/x520_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/loader.py` & `pkilint-0.8.5/pkilint/loader.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/msft/msft_name.py` & `pkilint-0.8.5/pkilint/msft/msft_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/__init__.py` & `pkilint-0.8.5/pkilint/pkix/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/algorithm.py` & `pkilint-0.8.5/pkilint/pkix/algorithm.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/certificate/__init__.py` & `pkilint-0.8.5/pkilint/pkix/certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/certificate/certificate_extension.py` & `pkilint-0.8.5/pkilint/pkix/certificate/certificate_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/certificate/certificate_key.py` & `pkilint-0.8.5/pkilint/pkix/certificate/certificate_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/certificate/certificate_name.py` & `pkilint-0.8.5/pkilint/pkix/certificate/certificate_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/certificate/certificate_validator.py` & `pkilint-0.8.5/pkilint/pkix/certificate/certificate_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/certificate/certificate_validity.py` & `pkilint-0.8.5/pkilint/pkix/certificate/certificate_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/crl/__init__.py` & `pkilint-0.8.5/pkilint/pkix/crl/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/crl/crl_extension.py` & `pkilint-0.8.5/pkilint/pkix/crl/crl_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/crl/crl_validator.py` & `pkilint-0.8.5/pkilint/pkix/crl/crl_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/crl/crl_validity.py` & `pkilint-0.8.5/pkilint/pkix/crl/crl_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/extension.py` & `pkilint-0.8.5/pkilint/pkix/extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/general_name.py` & `pkilint-0.8.5/pkilint/pkix/general_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/name.py` & `pkilint-0.8.5/pkilint/pkix/name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/ocsp/__init__.py` & `pkilint-0.8.5/pkilint/pkix/ocsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_basic_response.py` & `pkilint-0.8.5/pkilint/pkix/ocsp/ocsp_basic_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_response.py` & `pkilint-0.8.5/pkilint/pkix/ocsp/ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_validity.py` & `pkilint-0.8.5/pkilint/pkix/ocsp/ocsp_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/pkix/time.py` & `pkilint-0.8.5/pkilint/pkix/time.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/report.py` & `pkilint-0.8.5/pkilint/report.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/util.py` & `pkilint-0.8.5/pkilint/util.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint/validation.py` & `pkilint-0.8.5/pkilint/validation.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/pkilint.egg-info/PKG-INFO` & `pkilint-0.8.5/pkilint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.8.4
+Version: 0.8.5
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pkilint-0.8.4/pkilint.egg-info/SOURCES.txt` & `pkilint-0.8.5/pkilint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/setup.cfg` & `pkilint-0.8.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/tests/integration_certificate/__init__.py` & `pkilint-0.8.5/tests/integration_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/tests/integration_certificate/test_cabf_smime_cert.py` & `pkilint-0.8.5/tests/integration_certificate/test_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/tests/integration_certificate/test_pkix_cert.py` & `pkilint-0.8.5/tests/integration_certificate/test_pkix_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/tests/itu/test_bitstring.py` & `pkilint-0.8.5/tests/itu/test_bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/tests/itu/test_string.py` & `pkilint-0.8.5/tests/itu/test_string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.4/tests/util.py` & `pkilint-0.8.5/tests/util.py`

 * *Files identical despite different names*

