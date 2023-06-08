# Comparing `tmp/frasa-0.1.54.tar.gz` & `tmp/frasa-0.1.55.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frasa-0.1.54.tar", last modified: Thu Jun  8 12:54:10 2023, max compression
+gzip compressed data, was "frasa-0.1.55.tar", last modified: Thu Jun  8 17:58:54 2023, max compression
```

## Comparing `frasa-0.1.54.tar` & `frasa-0.1.55.tar`

### file list

```diff
@@ -1,100 +1,111 @@
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.634201 frasa-0.1.54/
--rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.1.54/LICENSE
--rw-r--r--   0 novay      (501) staff       (20)      691 2023-06-04 18:05:03.000000 frasa-0.1.54/MANIFEST.in
--rw-r--r--   0 novay      (501) staff       (20)     1323 2023-06-08 12:54:10.634029 frasa-0.1.54/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)      613 2023-04-28 16:40:32.000000 frasa-0.1.54/README.md
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.593319 frasa-0.1.54/frasa/
--rw-r--r--   0 novay      (501) staff       (20)      677 2023-06-08 12:53:46.000000 frasa-0.1.54/frasa/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)      794 2023-06-08 10:08:17.000000 frasa-0.1.54/frasa/base.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.594425 frasa-0.1.54/frasa/datasets/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.1.54/frasa/datasets/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.594539 frasa-0.1.54/frasa/datasets/corpus/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.1.54/frasa/datasets/corpus/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.594677 frasa-0.1.54/frasa/datasets/corpus/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.1.54/frasa/datasets/corpus/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.594931 frasa-0.1.54/frasa/datasets/corpus/indonesia/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.1.54/frasa/datasets/corpus/indonesia/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.607200 frasa-0.1.54/frasa/datasets/corpus/indonesia/lemma/
--rw-r--r--   0 novay      (501) staff       (20)      377 2023-04-15 21:44:57.000000 frasa-0.1.54/frasa/datasets/corpus/indonesia/lemma/clitics.txt
--rw-r--r--   0 novay      (501) staff       (20) 19937523 2023-04-04 17:44:44.000000 frasa-0.1.54/frasa/datasets/corpus/indonesia/lemma/dict.json
--rw-r--r--   0 novay      (501) staff       (20)   236286 2023-04-04 17:43:21.000000 frasa-0.1.54/frasa/datasets/corpus/indonesia/lemma/root.txt
--rw-r--r--   0 novay      (501) staff       (20)    10520 2023-04-15 22:25:42.000000 frasa-0.1.54/frasa/datasets/corpus/indonesia/stopword.txt
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.612259 frasa-0.1.54/frasa/datasets/corpus/sensor/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.1.54/frasa/datasets/corpus/sensor/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)    71076 2023-04-14 16:22:53.000000 frasa-0.1.54/frasa/datasets/corpus/sensor/alphabetic_unicode.json
--rw-r--r--   0 novay      (501) staff       (20)      118 2023-04-15 23:06:01.000000 frasa-0.1.54/frasa/datasets/corpus/sensor/sensor-aturan.csv
--rw-r--r--   0 novay      (501) staff       (20)     7997 2023-04-15 23:06:01.000000 frasa-0.1.54/frasa/datasets/corpus/sensor/sensor-kata.csv
--rw-r--r--   0 novay      (501) staff       (20)      112 2023-04-15 23:06:01.000000 frasa-0.1.54/frasa/datasets/corpus/sensor/sensor-pengganti.csv
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.612500 frasa-0.1.54/frasa/datasets/corpus/tweets/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.1.54/frasa/datasets/corpus/tweets/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.612767 frasa-0.1.54/frasa/datasets/models/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:51:39.000000 frasa-0.1.54/frasa/datasets/models/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)   121561 2023-04-15 23:49:13.000000 frasa-0.1.54/frasa/datasets/models/frasa-gender.pickle
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.625666 frasa-0.1.54/frasa/datasets/models/nusax/
--rw-r--r--   0 novay      (501) staff       (20)   141300 2023-06-04 17:03:55.000000 frasa-0.1.54/frasa/datasets/models/nusax/aceh_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    33057 2023-06-04 17:03:57.000000 frasa-0.1.54/frasa/datasets/models/nusax/aceh_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   164436 2023-06-04 17:03:59.000000 frasa-0.1.54/frasa/datasets/models/nusax/bali_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    39361 2023-06-04 17:04:01.000000 frasa-0.1.54/frasa/datasets/models/nusax/bali_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   154020 2023-06-04 17:04:04.000000 frasa-0.1.54/frasa/datasets/models/nusax/banjar_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    37829 2023-06-04 17:04:05.000000 frasa-0.1.54/frasa/datasets/models/nusax/banjar_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   153924 2023-06-04 17:04:07.000000 frasa-0.1.54/frasa/datasets/models/nusax/batak_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    37447 2023-06-04 17:04:08.000000 frasa-0.1.54/frasa/datasets/models/nusax/batak_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   164004 2023-06-04 17:04:10.000000 frasa-0.1.54/frasa/datasets/models/nusax/bugis_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    40991 2023-06-04 17:04:12.000000 frasa-0.1.54/frasa/datasets/models/nusax/bugis_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   144948 2023-06-04 17:04:16.000000 frasa-0.1.54/frasa/datasets/models/nusax/indo_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    35227 2023-06-04 17:04:17.000000 frasa-0.1.54/frasa/datasets/models/nusax/indo_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   154404 2023-06-04 17:04:19.000000 frasa-0.1.54/frasa/datasets/models/nusax/jawa_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    36524 2023-06-04 17:04:20.000000 frasa-0.1.54/frasa/datasets/models/nusax/jawa_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   159828 2023-06-04 17:04:23.000000 frasa-0.1.54/frasa/datasets/models/nusax/madura_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    38306 2023-06-04 17:04:24.000000 frasa-0.1.54/frasa/datasets/models/nusax/madura_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   149268 2023-06-04 17:04:26.000000 frasa-0.1.54/frasa/datasets/models/nusax/minang_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    36144 2023-06-04 17:04:27.000000 frasa-0.1.54/frasa/datasets/models/nusax/minang_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   135204 2023-06-04 17:04:31.000000 frasa-0.1.54/frasa/datasets/models/nusax/ngaju_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    31596 2023-06-04 17:04:32.000000 frasa-0.1.54/frasa/datasets/models/nusax/ngaju_vectorizer.pkl
--rw-r--r--   0 novay      (501) staff       (20)   157332 2023-06-04 17:04:34.000000 frasa-0.1.54/frasa/datasets/models/nusax/sunda_model.pkl
--rw-r--r--   0 novay      (501) staff       (20)    38239 2023-06-04 17:04:36.000000 frasa-0.1.54/frasa/datasets/models/nusax/sunda_vectorizer.pkl
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.625920 frasa-0.1.54/frasa/deteksi/
--rw-r--r--   0 novay      (501) staff       (20)      865 2023-04-16 00:07:31.000000 frasa-0.1.54/frasa/deteksi/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.626309 frasa-0.1.54/frasa/deteksi/bahasa/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.1.54/frasa/deteksi/bahasa/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.626424 frasa-0.1.54/frasa/deteksi/bahasa/data/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.1.54/frasa/deteksi/bahasa/data/__init__.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.627341 frasa-0.1.54/frasa/deteksi/gender/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:39:09.000000 frasa-0.1.54/frasa/deteksi/gender/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     3129 2023-04-18 19:44:26.000000 frasa-0.1.54/frasa/deteksi/gender/classify.py
--rw-r--r--   0 novay      (501) staff       (20)      992 2023-04-16 00:06:23.000000 frasa-0.1.54/frasa/deteksi/gender/gender.py
--rw-r--r--   0 novay      (501) staff       (20)      747 2023-04-15 23:49:34.000000 frasa-0.1.54/frasa/deteksi/gender/utils.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.628811 frasa-0.1.54/frasa/deteksi/plagiat/
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:14:54.000000 frasa-0.1.54/frasa/deteksi/plagiat/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     1363 2023-04-16 09:16:31.000000 frasa-0.1.54/frasa/deteksi/plagiat/cosine.py
--rw-r--r--   0 novay      (501) staff       (20)      911 2023-04-16 09:14:51.000000 frasa-0.1.54/frasa/deteksi/plagiat/jaccard.py
--rw-r--r--   0 novay      (501) staff       (20)     4247 2023-04-16 11:45:48.000000 frasa-0.1.54/frasa/deteksi/plagiat/plagiat.py
--rw-r--r--   0 novay      (501) staff       (20)     1176 2023-04-16 01:06:12.000000 frasa-0.1.54/frasa/deteksi/plagiat/rabin_karp.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.630452 frasa-0.1.54/frasa/preprocess/
--rw-r--r--   0 novay      (501) staff       (20)      286 2023-06-08 10:41:49.000000 frasa-0.1.54/frasa/preprocess/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)     8758 2023-04-15 21:37:48.000000 frasa-0.1.54/frasa/preprocess/lemma.py
--rw-r--r--   0 novay      (501) staff       (20)     1476 2023-06-04 18:04:23.000000 frasa-0.1.54/frasa/preprocess/sentimen.py
--rw-r--r--   0 novay      (501) staff       (20)      850 2023-04-15 22:28:40.000000 frasa-0.1.54/frasa/preprocess/stopword.py
--rw-r--r--   0 novay      (501) staff       (20)     9372 2023-04-16 13:15:30.000000 frasa-0.1.54/frasa/preprocess/token.py
--rw-r--r--   0 novay      (501) staff       (20)     5129 2023-06-08 12:52:05.000000 frasa-0.1.54/frasa/preprocess/tweet.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.633015 frasa-0.1.54/frasa/scrap/
--rw-r--r--   0 novay      (501) staff       (20)      145 2023-04-28 16:45:53.000000 frasa-0.1.54/frasa/scrap/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:09.000000 frasa-0.1.54/frasa/scrap/cnn.py
--rw-r--r--   0 novay      (501) staff       (20)     7902 2023-06-08 09:49:52.000000 frasa-0.1.54/frasa/scrap/detiknews.py
--rw-r--r--   0 novay      (501) staff       (20)     8492 2023-06-08 09:49:43.000000 frasa-0.1.54/frasa/scrap/liputan6.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:30.000000 frasa-0.1.54/frasa/scrap/tribun.py
--rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 16:58:21.000000 frasa-0.1.54/frasa/scrap/viva.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.633771 frasa-0.1.54/frasa/sensor/
--rw-r--r--   0 novay      (501) staff       (20)       76 2023-04-15 23:12:29.000000 frasa-0.1.54/frasa/sensor/__init__.py
--rw-r--r--   0 novay      (501) staff       (20)      428 2023-04-15 23:10:24.000000 frasa-0.1.54/frasa/sensor/constants.py
--rw-r--r--   0 novay      (501) staff       (20)     9267 2023-04-15 23:12:36.000000 frasa-0.1.54/frasa/sensor/sensor.py
--rw-r--r--   0 novay      (501) staff       (20)     1584 2023-04-15 23:10:52.000000 frasa-0.1.54/frasa/sensor/utils.py
--rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.1.54/frasa/sensor/variasi.py
--rw-r--r--   0 novay      (501) staff       (20)     1640 2023-04-19 21:40:39.000000 frasa-0.1.54/frasa/update.py
-drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 12:54:10.594290 frasa-0.1.54/frasa.egg-info/
--rw-r--r--   0 novay      (501) staff       (20)     1323 2023-06-08 12:54:10.000000 frasa-0.1.54/frasa.egg-info/PKG-INFO
--rw-r--r--   0 novay      (501) staff       (20)     2723 2023-06-08 12:54:10.000000 frasa-0.1.54/frasa.egg-info/SOURCES.txt
--rw-r--r--   0 novay      (501) staff       (20)        1 2023-06-08 12:54:10.000000 frasa-0.1.54/frasa.egg-info/dependency_links.txt
--rw-r--r--   0 novay      (501) staff       (20)       12 2023-06-08 12:54:10.000000 frasa-0.1.54/frasa.egg-info/top_level.txt
--rw-r--r--   0 novay      (501) staff       (20)       38 2023-06-08 12:54:10.634254 frasa-0.1.54/setup.cfg
--rw-r--r--   0 novay      (501) staff       (20)     1599 2023-06-08 12:53:34.000000 frasa-0.1.54/setup.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.596665 frasa-0.1.55/
+-rw-r--r--   0 novay      (501) staff       (20)     1074 2023-04-12 07:34:01.000000 frasa-0.1.55/LICENSE
+-rw-r--r--   0 novay      (501) staff       (20)      691 2023-06-04 18:05:03.000000 frasa-0.1.55/MANIFEST.in
+-rw-r--r--   0 novay      (501) staff       (20)     1323 2023-06-08 17:58:54.596516 frasa-0.1.55/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)      613 2023-04-28 16:40:32.000000 frasa-0.1.55/README.md
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.553660 frasa-0.1.55/frasa/
+-rw-r--r--   0 novay      (501) staff       (20)      677 2023-06-08 17:58:46.000000 frasa-0.1.55/frasa/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      794 2023-06-08 10:08:17.000000 frasa-0.1.55/frasa/base.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.554835 frasa-0.1.55/frasa/datasets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:13.000000 frasa-0.1.55/frasa/datasets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.554971 frasa-0.1.55/frasa/datasets/corpus/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:21.000000 frasa-0.1.55/frasa/datasets/corpus/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.555119 frasa-0.1.55/frasa/datasets/corpus/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:27.000000 frasa-0.1.55/frasa/datasets/corpus/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.555373 frasa-0.1.55/frasa/datasets/corpus/indonesia/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:26.000000 frasa-0.1.55/frasa/datasets/corpus/indonesia/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.567178 frasa-0.1.55/frasa/datasets/corpus/indonesia/lemma/
+-rw-r--r--   0 novay      (501) staff       (20)      377 2023-04-15 21:44:57.000000 frasa-0.1.55/frasa/datasets/corpus/indonesia/lemma/clitics.txt
+-rw-r--r--   0 novay      (501) staff       (20) 19937523 2023-04-04 17:44:44.000000 frasa-0.1.55/frasa/datasets/corpus/indonesia/lemma/dict.json
+-rw-r--r--   0 novay      (501) staff       (20)   236286 2023-04-04 17:43:21.000000 frasa-0.1.55/frasa/datasets/corpus/indonesia/lemma/root.txt
+-rw-r--r--   0 novay      (501) staff       (20)    10520 2023-04-15 22:25:42.000000 frasa-0.1.55/frasa/datasets/corpus/indonesia/stopword.txt
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.573713 frasa-0.1.55/frasa/datasets/corpus/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:24.000000 frasa-0.1.55/frasa/datasets/corpus/sensor/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)    71076 2023-04-14 16:22:53.000000 frasa-0.1.55/frasa/datasets/corpus/sensor/alphabetic_unicode.json
+-rw-r--r--   0 novay      (501) staff       (20)      118 2023-04-15 23:06:01.000000 frasa-0.1.55/frasa/datasets/corpus/sensor/sensor-aturan.csv
+-rw-r--r--   0 novay      (501) staff       (20)     7997 2023-04-15 23:06:01.000000 frasa-0.1.55/frasa/datasets/corpus/sensor/sensor-kata.csv
+-rw-r--r--   0 novay      (501) staff       (20)      112 2023-04-15 23:06:01.000000 frasa-0.1.55/frasa/datasets/corpus/sensor/sensor-pengganti.csv
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.573979 frasa-0.1.55/frasa/datasets/corpus/tweets/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:23.000000 frasa-0.1.55/frasa/datasets/corpus/tweets/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.574226 frasa-0.1.55/frasa/datasets/models/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:51:39.000000 frasa-0.1.55/frasa/datasets/models/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)   121561 2023-04-15 23:49:13.000000 frasa-0.1.55/frasa/datasets/models/frasa-gender.pickle
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.586498 frasa-0.1.55/frasa/datasets/models/nusax/
+-rw-r--r--   0 novay      (501) staff       (20)   141300 2023-06-04 17:03:55.000000 frasa-0.1.55/frasa/datasets/models/nusax/aceh_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    33057 2023-06-04 17:03:57.000000 frasa-0.1.55/frasa/datasets/models/nusax/aceh_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   164436 2023-06-04 17:03:59.000000 frasa-0.1.55/frasa/datasets/models/nusax/bali_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    39361 2023-06-04 17:04:01.000000 frasa-0.1.55/frasa/datasets/models/nusax/bali_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   154020 2023-06-04 17:04:04.000000 frasa-0.1.55/frasa/datasets/models/nusax/banjar_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    37829 2023-06-04 17:04:05.000000 frasa-0.1.55/frasa/datasets/models/nusax/banjar_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   153924 2023-06-04 17:04:07.000000 frasa-0.1.55/frasa/datasets/models/nusax/batak_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    37447 2023-06-04 17:04:08.000000 frasa-0.1.55/frasa/datasets/models/nusax/batak_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   164004 2023-06-04 17:04:10.000000 frasa-0.1.55/frasa/datasets/models/nusax/bugis_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    40991 2023-06-04 17:04:12.000000 frasa-0.1.55/frasa/datasets/models/nusax/bugis_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   144948 2023-06-04 17:04:16.000000 frasa-0.1.55/frasa/datasets/models/nusax/indo_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    35227 2023-06-04 17:04:17.000000 frasa-0.1.55/frasa/datasets/models/nusax/indo_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   154404 2023-06-04 17:04:19.000000 frasa-0.1.55/frasa/datasets/models/nusax/jawa_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    36524 2023-06-04 17:04:20.000000 frasa-0.1.55/frasa/datasets/models/nusax/jawa_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   159828 2023-06-04 17:04:23.000000 frasa-0.1.55/frasa/datasets/models/nusax/madura_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    38306 2023-06-04 17:04:24.000000 frasa-0.1.55/frasa/datasets/models/nusax/madura_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   149268 2023-06-04 17:04:26.000000 frasa-0.1.55/frasa/datasets/models/nusax/minang_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    36144 2023-06-04 17:04:27.000000 frasa-0.1.55/frasa/datasets/models/nusax/minang_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   135204 2023-06-04 17:04:31.000000 frasa-0.1.55/frasa/datasets/models/nusax/ngaju_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    31596 2023-06-04 17:04:32.000000 frasa-0.1.55/frasa/datasets/models/nusax/ngaju_vectorizer.pkl
+-rw-r--r--   0 novay      (501) staff       (20)   157332 2023-06-04 17:04:34.000000 frasa-0.1.55/frasa/datasets/models/nusax/sunda_model.pkl
+-rw-r--r--   0 novay      (501) staff       (20)    38239 2023-06-04 17:04:36.000000 frasa-0.1.55/frasa/datasets/models/nusax/sunda_vectorizer.pkl
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.586748 frasa-0.1.55/frasa/deteksi/
+-rw-r--r--   0 novay      (501) staff       (20)      865 2023-04-16 00:07:31.000000 frasa-0.1.55/frasa/deteksi/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.587116 frasa-0.1.55/frasa/deteksi/bahasa/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-12 09:15:48.000000 frasa-0.1.55/frasa/deteksi/bahasa/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.587226 frasa-0.1.55/frasa/deteksi/bahasa/data/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-14 22:44:46.000000 frasa-0.1.55/frasa/deteksi/bahasa/data/__init__.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.588098 frasa-0.1.55/frasa/deteksi/gender/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:39:09.000000 frasa-0.1.55/frasa/deteksi/gender/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     3129 2023-04-18 19:44:26.000000 frasa-0.1.55/frasa/deteksi/gender/classify.py
+-rw-r--r--   0 novay      (501) staff       (20)      992 2023-04-16 00:06:23.000000 frasa-0.1.55/frasa/deteksi/gender/gender.py
+-rw-r--r--   0 novay      (501) staff       (20)      747 2023-04-15 23:49:34.000000 frasa-0.1.55/frasa/deteksi/gender/utils.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.589688 frasa-0.1.55/frasa/deteksi/plagiat/
+-rw-r--r--   0 novay      (501) staff       (20)        0 2023-04-15 23:14:54.000000 frasa-0.1.55/frasa/deteksi/plagiat/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     1363 2023-04-16 09:16:31.000000 frasa-0.1.55/frasa/deteksi/plagiat/cosine.py
+-rw-r--r--   0 novay      (501) staff       (20)      911 2023-04-16 09:14:51.000000 frasa-0.1.55/frasa/deteksi/plagiat/jaccard.py
+-rw-r--r--   0 novay      (501) staff       (20)     4247 2023-04-16 11:45:48.000000 frasa-0.1.55/frasa/deteksi/plagiat/plagiat.py
+-rw-r--r--   0 novay      (501) staff       (20)     1176 2023-04-16 01:06:12.000000 frasa-0.1.55/frasa/deteksi/plagiat/rabin_karp.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.590821 frasa-0.1.55/frasa/preprocess/
+-rw-r--r--   0 novay      (501) staff       (20)      286 2023-06-08 10:41:49.000000 frasa-0.1.55/frasa/preprocess/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     8758 2023-04-15 21:37:48.000000 frasa-0.1.55/frasa/preprocess/lemma.py
+-rw-r--r--   0 novay      (501) staff       (20)     1476 2023-06-04 18:04:23.000000 frasa-0.1.55/frasa/preprocess/sentimen.py
+-rw-r--r--   0 novay      (501) staff       (20)      850 2023-04-15 22:28:40.000000 frasa-0.1.55/frasa/preprocess/stopword.py
+-rw-r--r--   0 novay      (501) staff       (20)     9372 2023-04-16 13:15:30.000000 frasa-0.1.55/frasa/preprocess/token.py
+-rw-r--r--   0 novay      (501) staff       (20)     5129 2023-06-08 12:52:05.000000 frasa-0.1.55/frasa/preprocess/tweet.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.595446 frasa-0.1.55/frasa/scrap/
+-rw-r--r--   0 novay      (501) staff       (20)      778 2023-06-08 15:37:47.000000 frasa-0.1.55/frasa/scrap/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)     3214 2023-06-08 16:58:22.000000 frasa-0.1.55/frasa/scrap/antara.py
+-rw-r--r--   0 novay      (501) staff       (20)     1251 2023-06-08 17:23:32.000000 frasa-0.1.55/frasa/scrap/cnbc.py
+-rw-r--r--   0 novay      (501) staff       (20)     1201 2023-06-08 17:26:45.000000 frasa-0.1.55/frasa/scrap/cnn.py
+-rw-r--r--   0 novay      (501) staff       (20)     7902 2023-06-08 09:49:52.000000 frasa-0.1.55/frasa/scrap/detiknews.py
+-rw-r--r--   0 novay      (501) staff       (20)      359 2023-06-08 17:28:05.000000 frasa-0.1.55/frasa/scrap/jpnn.py
+-rw-r--r--   0 novay      (501) staff       (20)      367 2023-06-08 17:28:15.000000 frasa-0.1.55/frasa/scrap/kumparan.py
+-rw-r--r--   0 novay      (501) staff       (20)     8492 2023-06-08 09:49:43.000000 frasa-0.1.55/frasa/scrap/liputan6.py
+-rw-r--r--   0 novay      (501) staff       (20)     1243 2023-06-08 17:51:32.000000 frasa-0.1.55/frasa/scrap/merdeka.py
+-rw-r--r--   0 novay      (501) staff       (20)     1149 2023-06-08 17:52:54.000000 frasa-0.1.55/frasa/scrap/okezone.py
+-rw-r--r--   0 novay      (501) staff       (20)     1149 2023-06-08 17:53:27.000000 frasa-0.1.55/frasa/scrap/republika.py
+-rw-r--r--   0 novay      (501) staff       (20)     1329 2023-06-08 17:54:41.000000 frasa-0.1.55/frasa/scrap/sindonews.py
+-rw-r--r--   0 novay      (501) staff       (20)     1149 2023-06-08 17:55:25.000000 frasa-0.1.55/frasa/scrap/suara.py
+-rw-r--r--   0 novay      (501) staff       (20)     1192 2023-06-08 17:56:57.000000 frasa-0.1.55/frasa/scrap/tempo.py
+-rw-r--r--   0 novay      (501) staff       (20)     1251 2023-06-08 17:57:59.000000 frasa-0.1.55/frasa/scrap/tribun.py
+-rw-r--r--   0 novay      (501) staff       (20)      776 2023-06-08 15:49:48.000000 frasa-0.1.55/frasa/scrap/utils.py
+-rw-r--r--   0 novay      (501) staff       (20)      454 2023-06-08 15:39:44.000000 frasa-0.1.55/frasa/scrap/viva.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.596291 frasa-0.1.55/frasa/sensor/
+-rw-r--r--   0 novay      (501) staff       (20)       76 2023-04-15 23:12:29.000000 frasa-0.1.55/frasa/sensor/__init__.py
+-rw-r--r--   0 novay      (501) staff       (20)      428 2023-04-15 23:10:24.000000 frasa-0.1.55/frasa/sensor/constants.py
+-rw-r--r--   0 novay      (501) staff       (20)     9267 2023-04-15 23:12:36.000000 frasa-0.1.55/frasa/sensor/sensor.py
+-rw-r--r--   0 novay      (501) staff       (20)     1584 2023-04-15 23:10:52.000000 frasa-0.1.55/frasa/sensor/utils.py
+-rw-r--r--   0 novay      (501) staff       (20)     2364 2023-04-14 16:23:34.000000 frasa-0.1.55/frasa/sensor/variasi.py
+-rw-r--r--   0 novay      (501) staff       (20)     1640 2023-04-19 21:40:39.000000 frasa-0.1.55/frasa/update.py
+drwxr-xr-x   0 novay      (501) staff       (20)        0 2023-06-08 17:58:54.554676 frasa-0.1.55/frasa.egg-info/
+-rw-r--r--   0 novay      (501) staff       (20)     1323 2023-06-08 17:58:54.000000 frasa-0.1.55/frasa.egg-info/PKG-INFO
+-rw-r--r--   0 novay      (501) staff       (20)     2968 2023-06-08 17:58:54.000000 frasa-0.1.55/frasa.egg-info/SOURCES.txt
+-rw-r--r--   0 novay      (501) staff       (20)        1 2023-06-08 17:58:54.000000 frasa-0.1.55/frasa.egg-info/dependency_links.txt
+-rw-r--r--   0 novay      (501) staff       (20)       12 2023-06-08 17:58:54.000000 frasa-0.1.55/frasa.egg-info/top_level.txt
+-rw-r--r--   0 novay      (501) staff       (20)       38 2023-06-08 17:58:54.596713 frasa-0.1.55/setup.cfg
+-rw-r--r--   0 novay      (501) staff       (20)     1599 2023-06-08 17:58:42.000000 frasa-0.1.55/setup.py
```

### Comparing `frasa-0.1.54/LICENSE` & `frasa-0.1.55/LICENSE`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/MANIFEST.in` & `frasa-0.1.55/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/PKG-INFO` & `frasa-0.1.55/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.1.54
+Version: 0.1.55
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.1.54/README.md` & `frasa-0.1.55/README.md`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/__init__.py` & `frasa-0.1.55/frasa/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 Kunjungi http://frasa.id untuk informasi selengkapnya.
 """
 
 import os
 
 __name__ = "frasa"
-__version__ = "0.1.54"
+__version__ = "0.1.55"
 __license__ = 'MIT'
 __author__ = 'Novianto Rahmadi'
 
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
 DATASET_DIR = PACKAGE_DIR + '/datasets/corpus'
 MODELS_DIR = PACKAGE_DIR + '/datasets/models'
```

### Comparing `frasa-0.1.54/frasa/base.py` & `frasa-0.1.55/frasa/base.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/corpus/indonesia/lemma/dict.json` & `frasa-0.1.55/frasa/datasets/corpus/indonesia/lemma/dict.json`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/corpus/indonesia/lemma/root.txt` & `frasa-0.1.55/frasa/datasets/corpus/indonesia/lemma/root.txt`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/corpus/indonesia/stopword.txt` & `frasa-0.1.55/frasa/datasets/corpus/indonesia/stopword.txt`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/corpus/sensor/alphabetic_unicode.json` & `frasa-0.1.55/frasa/datasets/corpus/sensor/alphabetic_unicode.json`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/corpus/sensor/sensor-kata.csv` & `frasa-0.1.55/frasa/datasets/corpus/sensor/sensor-kata.csv`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/frasa-gender.pickle` & `frasa-0.1.55/frasa/datasets/models/frasa-gender.pickle`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/aceh_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/aceh_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/aceh_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/aceh_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/bali_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/bali_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/bali_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/bali_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/banjar_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/banjar_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/banjar_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/banjar_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/batak_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/batak_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/batak_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/batak_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/bugis_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/bugis_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/bugis_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/bugis_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/indo_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/indo_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/indo_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/indo_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/jawa_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/jawa_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/jawa_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/jawa_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/madura_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/madura_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/madura_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/madura_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/minang_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/minang_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/minang_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/minang_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/ngaju_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/ngaju_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/ngaju_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/ngaju_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/sunda_model.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/sunda_model.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/datasets/models/nusax/sunda_vectorizer.pkl` & `frasa-0.1.55/frasa/datasets/models/nusax/sunda_vectorizer.pkl`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/deteksi/__init__.py` & `frasa-0.1.55/frasa/deteksi/__init__.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/deteksi/gender/classify.py` & `frasa-0.1.55/frasa/deteksi/gender/classify.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/deteksi/gender/gender.py` & `frasa-0.1.55/frasa/deteksi/gender/gender.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/deteksi/gender/utils.py` & `frasa-0.1.55/frasa/deteksi/gender/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/deteksi/plagiat/cosine.py` & `frasa-0.1.55/frasa/deteksi/plagiat/cosine.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/deteksi/plagiat/jaccard.py` & `frasa-0.1.55/frasa/deteksi/plagiat/jaccard.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/deteksi/plagiat/plagiat.py` & `frasa-0.1.55/frasa/deteksi/plagiat/plagiat.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/deteksi/plagiat/rabin_karp.py` & `frasa-0.1.55/frasa/deteksi/plagiat/rabin_karp.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/preprocess/lemma.py` & `frasa-0.1.55/frasa/preprocess/lemma.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/preprocess/sentimen.py` & `frasa-0.1.55/frasa/preprocess/sentimen.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/preprocess/stopword.py` & `frasa-0.1.55/frasa/preprocess/stopword.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/preprocess/token.py` & `frasa-0.1.55/frasa/preprocess/token.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/preprocess/tweet.py` & `frasa-0.1.55/frasa/preprocess/tweet.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/scrap/detiknews.py` & `frasa-0.1.55/frasa/scrap/detiknews.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/scrap/liputan6.py` & `frasa-0.1.55/frasa/scrap/liputan6.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/sensor/sensor.py` & `frasa-0.1.55/frasa/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/sensor/utils.py` & `frasa-0.1.55/frasa/sensor/utils.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/sensor/variasi.py` & `frasa-0.1.55/frasa/sensor/variasi.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa/update.py` & `frasa-0.1.55/frasa/update.py`

 * *Files identical despite different names*

### Comparing `frasa-0.1.54/frasa.egg-info/PKG-INFO` & `frasa-0.1.55/frasa.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frasa
-Version: 0.1.54
+Version: 0.1.55
 Summary: Koleksi NLP Pribadi untuk Bahasa Indonesia.
 Home-page: https://github.com/novay/frasa
 Author: Novianto Rahmadi
 Author-email: novay@btekno.id
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `frasa-0.1.54/frasa.egg-info/SOURCES.txt` & `frasa-0.1.55/frasa.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -62,17 +62,28 @@
 frasa/preprocess/__init__.py
 frasa/preprocess/lemma.py
 frasa/preprocess/sentimen.py
 frasa/preprocess/stopword.py
 frasa/preprocess/token.py
 frasa/preprocess/tweet.py
 frasa/scrap/__init__.py
+frasa/scrap/antara.py
+frasa/scrap/cnbc.py
 frasa/scrap/cnn.py
 frasa/scrap/detiknews.py
+frasa/scrap/jpnn.py
+frasa/scrap/kumparan.py
 frasa/scrap/liputan6.py
+frasa/scrap/merdeka.py
+frasa/scrap/okezone.py
+frasa/scrap/republika.py
+frasa/scrap/sindonews.py
+frasa/scrap/suara.py
+frasa/scrap/tempo.py
 frasa/scrap/tribun.py
+frasa/scrap/utils.py
 frasa/scrap/viva.py
 frasa/sensor/__init__.py
 frasa/sensor/constants.py
 frasa/sensor/sensor.py
 frasa/sensor/utils.py
 frasa/sensor/variasi.py
```

### Comparing `frasa-0.1.54/setup.py` & `frasa-0.1.55/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 HERE = path.abspath(path.dirname(__file__))
 
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
     
 setup(
     name="frasa",
-    version="0.1.54",
+    version="0.1.55",
     description="Koleksi NLP Pribadi untuk Bahasa Indonesia.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/novay/frasa",
     author="Novianto Rahmadi",
     author_email="novay@btekno.id",
     license="MIT",
```

