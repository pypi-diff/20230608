# Comparing `tmp/weathon-0.0.0.8.tar.gz` & `tmp/weathon-0.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/weathon-0.0.0.8.tar", last modified: Thu Oct  6 08:38:34 2022, max compression
+gzip compressed data, was "dist/weathon-0.0.0.9.tar", last modified: Sun Oct  9 15:21:33 2022, max compression
```

## Comparing `weathon-0.0.0.8.tar` & `weathon-0.0.0.9.tar`

### file list

```diff
@@ -1,234 +1,234 @@
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/
--rw-r--r--   0 lizhen     (501) staff       (20)      430 2022-10-06 08:38:34.000000 weathon-0.0.0.8/PKG-INFO
--rw-r--r--   0 lizhen     (501) staff       (20)       17 2022-10-02 00:18:23.000000 weathon-0.0.0.8/README.md
--rw-r--r--   0 lizhen     (501) staff       (20)       38 2022-10-06 08:38:34.000000 weathon-0.0.0.8/setup.cfg
--rw-r--r--   0 lizhen     (501) staff       (20)     5005 2022-10-06 07:00:17.000000 weathon-0.0.0.8/setup.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/
--rw-r--r--   0 lizhen     (501) staff       (20)      275 2022-10-06 08:38:32.000000 weathon-0.0.0.8/weathon/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/cv/
--rw-r--r--   0 lizhen     (501) staff       (20)      160 2022-10-02 00:28:31.000000 weathon-0.0.0.8/weathon/cv/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/data/
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/data/dictionary/
--rw-r--r--   0 lizhen     (501) staff       (20)   320552 2022-10-06 07:12:12.000000 weathon-0.0.0.8/weathon/data/dictionary/animal.txt
--rw-r--r--   0 lizhen     (501) staff       (20)   341639 2022-10-06 06:18:37.000000 weathon-0.0.0.8/weathon/data/dictionary/antonym_word.txt
--rw-r--r--   0 lizhen     (501) staff       (20)    63549 2022-10-06 07:12:13.000000 weathon-0.0.0.8/weathon/data/dictionary/car.txt
--rw-r--r--   0 lizhen     (501) staff       (20)     7500 2022-10-06 07:12:31.000000 weathon-0.0.0.8/weathon/data/dictionary/family_name.txt
--rw-r--r--   0 lizhen     (501) staff       (20)    62296 2022-10-06 07:12:31.000000 weathon-0.0.0.8/weathon/data/dictionary/finance.txt
--rw-r--r--   0 lizhen     (501) staff       (20)   144749 2022-10-06 07:12:31.000000 weathon-0.0.0.8/weathon/data/dictionary/food.txt
--rw-r--r--   0 lizhen     (501) staff       (20)   308187 2022-10-06 07:12:32.000000 weathon-0.0.0.8/weathon/data/dictionary/it.txt
--rw-r--r--   0 lizhen     (501) staff       (20)   277745 2022-10-06 07:12:32.000000 weathon-0.0.0.8/weathon/data/dictionary/legal.txt
--rw-r--r--   0 lizhen     (501) staff       (20)   308805 2022-10-06 07:12:33.000000 weathon-0.0.0.8/weathon/data/dictionary/medical.txt
--rw-r--r--   0 lizhen     (501) staff       (20)   640666 2022-10-06 07:12:38.000000 weathon-0.0.0.8/weathon/data/dictionary/place_name.txt
--rw-r--r--   0 lizhen     (501) staff       (20)   190579 2022-10-06 07:12:38.000000 weathon-0.0.0.8/weathon/data/dictionary/professions.txt
--rw-r--r--   0 lizhen     (501) staff       (20)   244737 2022-10-06 07:12:39.000000 weathon-0.0.0.8/weathon/data/dictionary/same_pinyin.txt
--rw-r--r--   0 lizhen     (501) staff       (20)   404268 2022-10-06 07:12:39.000000 weathon-0.0.0.8/weathon/data/dictionary/same_stroke.txt
--rw-r--r--   0 lizhen     (501) staff       (20)    50256 2022-10-06 06:18:44.000000 weathon-0.0.0.8/weathon/data/dictionary/simple2traditional.txt
--rw-r--r--   0 lizhen     (501) staff       (20)     3660 2022-10-06 08:32:27.000000 weathon-0.0.0.8/weathon/data/dictionary/stopwords.txt
--rw-r--r--   0 lizhen     (501) staff       (20)    24274 2022-10-06 06:18:18.000000 weathon-0.0.0.8/weathon/data/dictionary/traditional2simple.txt
--rw-r--r--   0 lizhen     (501) staff       (20)     3137 2022-10-06 07:25:23.000000 weathon-0.0.0.8/weathon/data/dictionary/wechat_expression.txt
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/
--rw-r--r--   0 lizhen     (501) staff       (20)      160 2022-10-02 00:43:25.000000 weathon-0.0.0.8/weathon/nlp/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/base/
--rw-r--r--   0 lizhen     (501) staff       (20)      288 2022-10-04 01:09:19.000000 weathon-0.0.0.8/weathon/nlp/base/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6216 2022-10-02 06:29:57.000000 weathon-0.0.0.8/weathon/nlp/base/dataset.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1603 2022-10-03 08:04:07.000000 weathon-0.0.0.8/weathon/nlp/base/model.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2772 2022-10-04 01:09:19.000000 weathon-0.0.0.8/weathon/nlp/base/predictor.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6652 2022-10-04 02:20:51.000000 weathon-0.0.0.8/weathon/nlp/base/task.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1177 2022-10-02 02:57:12.000000 weathon-0.0.0.8/weathon/nlp/base/tokenizer.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1319 2022-10-02 01:55:42.000000 weathon-0.0.0.8/weathon/nlp/base/vocab.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/dataset/
--rw-r--r--   0 lizhen     (501) staff       (20)     1361 2022-10-02 09:08:08.000000 weathon-0.0.0.8/weathon/nlp/dataset/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)    11703 2022-10-02 09:04:09.000000 weathon-0.0.0.8/weathon/nlp/dataset/sentence_classification_dataset.py
--rw-r--r--   0 lizhen     (501) staff       (20)     9541 2022-10-02 09:08:08.000000 weathon-0.0.0.8/weathon/nlp/dataset/token_classification_dataset.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/factory/
--rw-r--r--   0 lizhen     (501) staff       (20)        2 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/factory/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/factory/loss/
--rw-r--r--   0 lizhen     (501) staff       (20)      856 2022-10-04 01:53:17.000000 weathon-0.0.0.8/weathon/nlp/factory/loss/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1466 2022-10-06 02:46:02.000000 weathon-0.0.0.8/weathon/nlp/factory/loss/casrel_loss.py
--rw-r--r--   0 lizhen     (501) staff       (20)      798 2022-10-06 02:46:14.000000 weathon-0.0.0.8/weathon/nlp/factory/loss/focal_loss.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1101 2022-10-06 02:46:35.000000 weathon-0.0.0.8/weathon/nlp/factory/loss/global_pointer_ce_loss.py
--rw-r--r--   0 lizhen     (501) staff       (20)      914 2022-10-06 02:46:25.000000 weathon-0.0.0.8/weathon/nlp/factory/loss/label_smoothing_ce_loss.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1879 2022-10-06 02:46:43.000000 weathon-0.0.0.8/weathon/nlp/factory/loss/r_drop_cross_entropy_loss.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/factory/metric/
--rw-r--r--   0 lizhen     (501) staff       (20)      297 2022-10-04 01:48:04.000000 weathon-0.0.0.8/weathon/nlp/factory/metric/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1173 2022-10-04 01:20:12.000000 weathon-0.0.0.8/weathon/nlp/factory/metric/biaffine_span_metrics.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4874 2022-10-04 01:48:04.000000 weathon-0.0.0.8/weathon/nlp/factory/metric/metrics.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2015 2022-10-04 01:20:12.000000 weathon-0.0.0.8/weathon/nlp/factory/metric/span_metrics.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/factory/optimizer/
--rw-r--r--   0 lizhen     (501) staff       (20)      615 2022-10-03 12:02:38.000000 weathon-0.0.0.8/weathon/nlp/factory/optimizer/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     9048 2022-10-03 11:27:17.000000 weathon-0.0.0.8/weathon/nlp/factory/optimizer/adafactor.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4953 2022-10-03 12:02:26.000000 weathon-0.0.0.8/weathon/nlp/factory/optimizer/adamw.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6476 2022-10-03 12:02:26.000000 weathon-0.0.0.8/weathon/nlp/factory/optimizer/madgrad.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1753 2022-10-06 02:45:46.000000 weathon-0.0.0.8/weathon/nlp/factory/optimizer/prior_wd.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/
--rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-04 03:04:39.000000 weathon-0.0.0.8/weathon/nlp/model/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/ie/
--rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/ie/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/
--rw-r--r--   0 lizhen     (501) staff       (20)     1273 2022-10-04 03:15:12.000000 weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6979 2022-10-04 03:14:23.000000 weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/prompt_uie.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2859 2022-10-04 03:14:23.000000 weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_dataset.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2877 2022-10-04 03:04:39.000000 weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_predictor.py
--rw-r--r--   0 lizhen     (501) staff       (20)     5386 2022-10-04 03:14:23.000000 weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_task.py
--rw-r--r--   0 lizhen     (501) staff       (20)     5024 2022-10-04 03:04:39.000000 weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/utils.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/ner/
--rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/ner/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/ner/biaffine_bert/
--rw-r--r--   0 lizhen     (501) staff       (20)     1166 2022-10-04 03:47:14.000000 weathon-0.0.0.8/weathon/nlp/model/ner/biaffine_bert/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3042 2022-10-04 03:47:14.000000 weathon-0.0.0.8/weathon/nlp/model/ner/biaffine_bert/biaffine_bert.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2949 2022-10-04 03:47:14.000000 weathon-0.0.0.8/weathon/nlp/model/ner/biaffine_bert/biaffine_named_entity_recognition.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/ner/crf_bert/
--rw-r--r--   0 lizhen     (501) staff       (20)      918 2022-10-04 05:09:01.000000 weathon-0.0.0.8/weathon/nlp/model/ner/crf_bert/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)      577 2022-10-04 04:47:49.000000 weathon-0.0.0.8/weathon/nlp/model/ner/crf_bert/crf_bert.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/ner/global_pointer_bert/
--rw-r--r--   0 lizhen     (501) staff       (20)     1316 2022-10-04 06:45:44.000000 weathon-0.0.0.8/weathon/nlp/model/ner/global_pointer_bert/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3072 2022-10-04 05:34:07.000000 weathon-0.0.0.8/weathon/nlp/model/ner/global_pointer_bert/global_pointer_bert.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2998 2022-10-04 06:45:44.000000 weathon-0.0.0.8/weathon/nlp/model/ner/global_pointer_bert/global_pointer_bert_named_entity_recognition.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/ner/span_bert/
--rw-r--r--   0 lizhen     (501) staff       (20)     1269 2022-10-04 06:54:49.000000 weathon-0.0.0.8/weathon/nlp/model/ner/span_bert/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4186 2022-10-04 06:49:22.000000 weathon-0.0.0.8/weathon/nlp/model/ner/span_bert/span_bert.py
--rw-r--r--   0 lizhen     (501) staff       (20)     5583 2022-10-04 06:49:22.000000 weathon-0.0.0.8/weathon/nlp/model/ner/span_bert/span_bert_named_entity_recognition.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/
--rw-r--r--   0 lizhen     (501) staff       (20)     1032 2022-10-04 07:03:49.000000 weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)    11323 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/w2ner_bert.py
--rw-r--r--   0 lizhen     (501) staff       (20)     5388 2022-10-04 07:03:49.000000 weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_dataset.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6392 2022-10-04 07:03:49.000000 weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_predictor.py
--rw-r--r--   0 lizhen     (501) staff       (20)     9151 2022-10-04 07:03:49.000000 weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_task.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/prompt/
--rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/prompt/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/prompt/prompt_bert/
--rw-r--r--   0 lizhen     (501) staff       (20)     1090 2022-10-04 07:06:41.000000 weathon-0.0.0.8/weathon/nlp/model/prompt/prompt_bert/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/
--rw-r--r--   0 lizhen     (501) staff       (20)     1396 2022-10-04 07:11:14.000000 weathon-0.0.0.8/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1945 2022-10-04 07:06:41.000000 weathon-0.0.0.8/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/prompt_ernie_ctm_nptag.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3277 2022-10-04 07:07:06.000000 weathon-0.0.0.8/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/prompt_ernie_ctm_nptag_tokenizer.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/re/
--rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/re/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/
--rw-r--r--   0 lizhen     (501) staff       (20)     1263 2022-10-04 07:16:08.000000 weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2865 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/casrel_bert.py
--rw-r--r--   0 lizhen     (501) staff       (20)     5141 2022-10-04 07:12:45.000000 weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_dataset.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4928 2022-10-04 07:12:45.000000 weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_predictor.py
--rw-r--r--   0 lizhen     (501) staff       (20)    12750 2022-10-04 07:12:45.000000 weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_task.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/
--rw-r--r--   0 lizhen     (501) staff       (20)     1205 2022-10-04 08:24:48.000000 weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     9607 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/prgc_bert.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6483 2022-10-04 08:21:00.000000 weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_dataset.py
--rw-r--r--   0 lizhen     (501) staff       (20)     7695 2022-10-04 08:21:00.000000 weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_predictor.py
--rw-r--r--   0 lizhen     (501) staff       (20)    11907 2022-10-04 08:21:00.000000 weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_task.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/tc/
--rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/tc/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/tc/bert/
--rw-r--r--   0 lizhen     (501) staff       (20)      899 2022-10-04 08:24:48.000000 weathon-0.0.0.8/weathon/nlp/model/tc/bert/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/tc/ernie/
--rw-r--r--   0 lizhen     (501) staff       (20)      948 2022-10-04 08:28:54.000000 weathon-0.0.0.8/weathon/nlp/model/tc/ernie/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/tm/
--rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/tm/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/tm/bert/
--rw-r--r--   0 lizhen     (501) staff       (20)      909 2022-10-04 08:33:30.000000 weathon-0.0.0.8/weathon/nlp/model/tm/bert/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/
--rw-r--r--   0 lizhen     (501) staff       (20)     2028 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6067 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2684 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_dataset.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3751 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_predictor.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3679 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_task.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/nlp/nn/
--rw-r--r--   0 lizhen     (501) staff       (20)      503 2022-10-04 04:47:49.000000 weathon-0.0.0.8/weathon/nlp/nn/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/nlp/nn/basic/
--rw-r--r--   0 lizhen     (501) staff       (20)      622 2022-10-03 11:02:53.000000 weathon-0.0.0.8/weathon/nlp/nn/basic/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6602 2022-10-03 08:53:07.000000 weathon-0.0.0.8/weathon/nlp/nn/basic/bert.py
--rw-r--r--   0 lizhen     (501) staff       (20)      892 2022-10-03 08:53:07.000000 weathon-0.0.0.8/weathon/nlp/nn/basic/ernie.py
--rw-r--r--   0 lizhen     (501) staff       (20)    10437 2022-10-03 09:25:19.000000 weathon-0.0.0.8/weathon/nlp/nn/basic/nezha.py
--rw-r--r--   0 lizhen     (501) staff       (20)     5723 2022-10-03 08:53:07.000000 weathon-0.0.0.8/weathon/nlp/nn/basic/rnn.py
--rw-r--r--   0 lizhen     (501) staff       (20)    10685 2022-10-03 11:00:32.000000 weathon-0.0.0.8/weathon/nlp/nn/basic/roformer.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3390 2022-10-03 08:53:07.000000 weathon-0.0.0.8/weathon/nlp/nn/basic/textcnn.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3077 2022-10-03 11:00:32.000000 weathon-0.0.0.8/weathon/nlp/nn/biaffine_bert.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/nlp/nn/configuration/
--rw-r--r--   0 lizhen     (501) staff       (20)      239 2022-10-03 08:58:28.000000 weathon-0.0.0.8/weathon/nlp/nn/configuration/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6343 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/nn/configuration/configuration_nezha.py
--rw-r--r--   0 lizhen     (501) staff       (20)     5912 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/nn/configuration/configuration_roformer.py
--rw-r--r--   0 lizhen     (501) staff       (20)      640 2022-10-03 11:03:54.000000 weathon-0.0.0.8/weathon/nlp/nn/crf_bert.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1707 2022-10-03 11:03:54.000000 weathon-0.0.0.8/weathon/nlp/nn/global_pointer_bert.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/
--rw-r--r--   0 lizhen     (501) staff       (20)      760 2022-10-04 07:06:41.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1158 2022-10-03 10:43:24.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/biaffine_block.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2008 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/cnn_block.py
--rw-r--r--   0 lizhen     (501) staff       (20)    20178 2022-10-03 10:49:57.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/crf_block.py
--rw-r--r--   0 lizhen     (501) staff       (20)    13337 2022-10-03 11:00:32.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/ernie_ctm_block.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4542 2022-10-03 11:00:32.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/global_pointer_block.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1059 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/layer_norm_block.py
--rw-r--r--   0 lizhen     (501) staff       (20)    14574 2022-10-03 09:22:38.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/nezha_block.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1466 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/pooler_block.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1292 2022-10-03 11:00:32.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/position_embedding_block.py
--rw-r--r--   0 lizhen     (501) staff       (20)    14036 2022-10-03 09:34:38.000000 weathon-0.0.0.8/weathon/nlp/nn/layer/reformer_block.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2633 2022-10-03 11:04:20.000000 weathon-0.0.0.8/weathon/nlp/nn/prompt_bert.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1905 2022-10-03 11:05:22.000000 weathon-0.0.0.8/weathon/nlp/nn/span_bert.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2419 2022-10-03 11:05:31.000000 weathon-0.0.0.8/weathon/nlp/nn/text_level_gcn.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/nlp/predictor/
--rw-r--r--   0 lizhen     (501) staff       (20)      327 2022-10-03 13:32:05.000000 weathon-0.0.0.8/weathon/nlp/predictor/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)    14281 2022-10-04 01:09:19.000000 weathon-0.0.0.8/weathon/nlp/predictor/sequence_classification.py
--rw-r--r--   0 lizhen     (501) staff       (20)    21509 2022-10-04 01:13:33.000000 weathon-0.0.0.8/weathon/nlp/predictor/token_classification.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/nlp/processor/
--rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/nlp/processor/__init__.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/nlp/processor/graph/
--rw-r--r--   0 lizhen     (501) staff       (20)       73 2022-10-02 05:56:42.000000 weathon-0.0.0.8/weathon/nlp/processor/graph/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4368 2022-10-02 05:56:19.000000 weathon-0.0.0.8/weathon/nlp/processor/graph/text_level_gcn.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/nlp/processor/tokenizer/
--rw-r--r--   0 lizhen     (501) staff       (20)      337 2022-10-02 05:54:45.000000 weathon-0.0.0.8/weathon/nlp/processor/tokenizer/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1498 2022-10-02 04:06:39.000000 weathon-0.0.0.8/weathon/nlp/processor/tokenizer/graph.py
--rw-r--r--   0 lizhen     (501) staff       (20)    16527 2022-10-02 05:53:19.000000 weathon-0.0.0.8/weathon/nlp/processor/tokenizer/transfomer.py
--rw-r--r--   0 lizhen     (501) staff       (20)      963 2022-10-02 03:06:00.000000 weathon-0.0.0.8/weathon/nlp/processor/tokenizer/vanilla.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/nlp/processor/vocab/
--rw-r--r--   0 lizhen     (501) staff       (20)      101 2022-10-02 03:06:57.000000 weathon-0.0.0.8/weathon/nlp/processor/vocab/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3407 2022-10-02 02:17:29.000000 weathon-0.0.0.8/weathon/nlp/processor/vocab/char_vocab.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1732 2022-10-02 02:17:29.000000 weathon-0.0.0.8/weathon/nlp/processor/vocab/label_vocab.py
--rw-r--r--   0 lizhen     (501) staff       (20)      449 2022-10-02 02:19:09.000000 weathon-0.0.0.8/weathon/nlp/processor/vocab/transfomer_vocab.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2848 2022-10-02 02:17:29.000000 weathon-0.0.0.8/weathon/nlp/processor/vocab/word_vocab.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/nlp/task/
--rw-r--r--   0 lizhen     (501) staff       (20)      540 2022-10-04 02:30:31.000000 weathon-0.0.0.8/weathon/nlp/task/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)    17987 2022-10-04 02:30:31.000000 weathon-0.0.0.8/weathon/nlp/task/named_entity_recognition.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3721 2022-10-04 02:30:31.000000 weathon-0.0.0.8/weathon/nlp/task/prompt_masked_language_model.py
--rw-r--r--   0 lizhen     (501) staff       (20)    13945 2022-10-04 02:20:51.000000 weathon-0.0.0.8/weathon/nlp/task/sequence_classification.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4705 2022-10-04 02:30:31.000000 weathon-0.0.0.8/weathon/nlp/task/text_classification.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1987 2022-10-04 02:30:31.000000 weathon-0.0.0.8/weathon/nlp/task/text_level_gcn_classification.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4705 2022-10-04 02:30:31.000000 weathon-0.0.0.8/weathon/nlp/task/text_match.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2359 2022-10-04 02:30:31.000000 weathon-0.0.0.8/weathon/nlp/task/token_classification.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:34.000000 weathon-0.0.0.8/weathon/utils/
--rw-r--r--   0 lizhen     (501) staff       (20)     2025 2022-10-06 08:25:12.000000 weathon-0.0.0.8/weathon/utils/__init__.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4930 2022-10-02 15:50:08.000000 weathon-0.0.0.8/weathon/utils/aho_corasick.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4790 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/utils/attack.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2373 2022-10-06 08:32:50.000000 weathon-0.0.0.8/weathon/utils/char_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)    12460 2022-10-04 00:56:42.000000 weathon-0.0.0.8/weathon/utils/conlleval.py
--rw-r--r--   0 lizhen     (501) staff       (20)      706 2022-10-06 08:14:53.000000 weathon-0.0.0.8/weathon/utils/constants.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4546 2022-10-06 08:37:25.000000 weathon-0.0.0.8/weathon/utils/dictionary.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3814 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/utils/ema.py
--rw-r--r--   0 lizhen     (501) staff       (20)      668 2022-10-06 04:49:44.000000 weathon-0.0.0.8/weathon/utils/encrypt_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)     9594 2022-10-06 04:51:59.000000 weathon-0.0.0.8/weathon/utils/file_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3878 2022-10-06 03:00:34.000000 weathon-0.0.0.8/weathon/utils/find_word.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4488 2022-10-06 04:55:20.000000 weathon-0.0.0.8/weathon/utils/gpu_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1457 2022-10-06 05:00:24.000000 weathon-0.0.0.8/weathon/utils/ip_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)      627 2022-10-06 05:00:24.000000 weathon-0.0.0.8/weathon/utils/json_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6569 2022-10-06 05:00:24.000000 weathon-0.0.0.8/weathon/utils/label_studio_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)     4481 2022-10-06 05:00:24.000000 weathon-0.0.0.8/weathon/utils/loss_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)     5159 2022-10-03 02:16:46.000000 weathon-0.0.0.8/weathon/utils/minjoin.py
--rw-r--r--   0 lizhen     (501) staff       (20)      661 2022-10-06 05:00:24.000000 weathon-0.0.0.8/weathon/utils/model_ensemble.py
--rw-r--r--   0 lizhen     (501) staff       (20)    21209 2022-10-06 05:00:24.000000 weathon-0.0.0.8/weathon/utils/ner_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)     5214 2022-10-06 05:02:11.000000 weathon-0.0.0.8/weathon/utils/optimizer_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)     2434 2022-10-02 00:42:07.000000 weathon-0.0.0.8/weathon/utils/sampler.py
--rw-r--r--   0 lizhen     (501) staff       (20)     9394 2022-10-06 05:02:11.000000 weathon-0.0.0.8/weathon/utils/schedule_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)      499 2022-10-06 05:02:11.000000 weathon-0.0.0.8/weathon/utils/seed_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3194 2022-10-06 08:37:25.000000 weathon-0.0.0.8/weathon/utils/states_machine.py
--rw-r--r--   0 lizhen     (501) staff       (20)     3678 2022-10-06 08:37:25.000000 weathon-0.0.0.8/weathon/utils/string_converter.py
--rw-r--r--   0 lizhen     (501) staff       (20)    25723 2022-10-06 05:46:56.000000 weathon-0.0.0.8/weathon/utils/string_similarity.py
--rw-r--r--   0 lizhen     (501) staff       (20)     5750 2022-10-06 08:23:36.000000 weathon-0.0.0.8/weathon/utils/string_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)    10283 2022-10-06 05:57:55.000000 weathon-0.0.0.8/weathon/utils/text_cluster.py
--rw-r--r--   0 lizhen     (501) staff       (20)     1334 2022-10-06 02:39:57.000000 weathon-0.0.0.8/weathon/utils/textrank.py
--rw-r--r--   0 lizhen     (501) staff       (20)     7745 2022-10-06 05:03:44.000000 weathon-0.0.0.8/weathon/utils/transformer_utils.py
--rw-r--r--   0 lizhen     (501) staff       (20)     6909 2022-10-03 03:09:05.000000 weathon-0.0.0.8/weathon/utils/union_find.py
-drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon.egg-info/
--rw-r--r--   0 lizhen     (501) staff       (20)      430 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon.egg-info/PKG-INFO
--rw-r--r--   0 lizhen     (501) staff       (20)     7651 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon.egg-info/SOURCES.txt
--rw-r--r--   0 lizhen     (501) staff       (20)        1 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon.egg-info/dependency_links.txt
--rw-r--r--   0 lizhen     (501) staff       (20)        1 2022-10-02 00:36:48.000000 weathon-0.0.0.8/weathon.egg-info/not-zip-safe
--rw-r--r--   0 lizhen     (501) staff       (20)      218 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon.egg-info/requires.txt
--rw-r--r--   0 lizhen     (501) staff       (20)        8 2022-10-06 08:38:33.000000 weathon-0.0.0.8/weathon.egg-info/top_level.txt
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/
+-rw-r--r--   0 lizhen     (501) staff       (20)      430 2022-10-09 15:21:33.000000 weathon-0.0.0.9/PKG-INFO
+-rw-r--r--   0 lizhen     (501) staff       (20)       17 2022-10-02 00:18:23.000000 weathon-0.0.0.9/README.md
+-rw-r--r--   0 lizhen     (501) staff       (20)       38 2022-10-09 15:21:33.000000 weathon-0.0.0.9/setup.cfg
+-rw-r--r--   0 lizhen     (501) staff       (20)     5006 2022-10-09 13:35:42.000000 weathon-0.0.0.9/setup.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/
+-rw-r--r--   0 lizhen     (501) staff       (20)      275 2022-10-09 15:21:31.000000 weathon-0.0.0.9/weathon/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/cv/
+-rw-r--r--   0 lizhen     (501) staff       (20)      160 2022-10-02 00:28:31.000000 weathon-0.0.0.9/weathon/cv/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/data/
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/data/dictionary/
+-rw-r--r--   0 lizhen     (501) staff       (20)   320552 2022-10-06 07:12:12.000000 weathon-0.0.0.9/weathon/data/dictionary/animal.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)   341639 2022-10-06 06:18:37.000000 weathon-0.0.0.9/weathon/data/dictionary/antonym_word.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)    63549 2022-10-06 07:12:13.000000 weathon-0.0.0.9/weathon/data/dictionary/car.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)     7500 2022-10-06 07:12:31.000000 weathon-0.0.0.9/weathon/data/dictionary/family_name.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)    62296 2022-10-06 07:12:31.000000 weathon-0.0.0.9/weathon/data/dictionary/finance.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)   144749 2022-10-06 07:12:31.000000 weathon-0.0.0.9/weathon/data/dictionary/food.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)   308187 2022-10-06 07:12:32.000000 weathon-0.0.0.9/weathon/data/dictionary/it.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)   277745 2022-10-06 07:12:32.000000 weathon-0.0.0.9/weathon/data/dictionary/legal.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)   308805 2022-10-06 07:12:33.000000 weathon-0.0.0.9/weathon/data/dictionary/medical.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)   640666 2022-10-06 07:12:38.000000 weathon-0.0.0.9/weathon/data/dictionary/place_name.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)   190579 2022-10-06 07:12:38.000000 weathon-0.0.0.9/weathon/data/dictionary/professions.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)   244737 2022-10-06 07:12:39.000000 weathon-0.0.0.9/weathon/data/dictionary/same_pinyin.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)   404268 2022-10-06 07:12:39.000000 weathon-0.0.0.9/weathon/data/dictionary/same_stroke.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)    50256 2022-10-06 06:18:44.000000 weathon-0.0.0.9/weathon/data/dictionary/simple2traditional.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)     3660 2022-10-06 08:32:27.000000 weathon-0.0.0.9/weathon/data/dictionary/stopwords.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)    24274 2022-10-06 06:18:18.000000 weathon-0.0.0.9/weathon/data/dictionary/traditional2simple.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)     3137 2022-10-06 07:25:23.000000 weathon-0.0.0.9/weathon/data/dictionary/wechat_expression.txt
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/
+-rw-r--r--   0 lizhen     (501) staff       (20)      160 2022-10-02 00:43:25.000000 weathon-0.0.0.9/weathon/nlp/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/base/
+-rw-r--r--   0 lizhen     (501) staff       (20)      288 2022-10-04 01:09:19.000000 weathon-0.0.0.9/weathon/nlp/base/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6560 2022-10-09 13:51:31.000000 weathon-0.0.0.9/weathon/nlp/base/dataset.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1603 2022-10-03 08:04:07.000000 weathon-0.0.0.9/weathon/nlp/base/model.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2772 2022-10-04 01:09:19.000000 weathon-0.0.0.9/weathon/nlp/base/predictor.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     7560 2022-10-09 15:15:26.000000 weathon-0.0.0.9/weathon/nlp/base/task.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1168 2022-10-09 13:59:36.000000 weathon-0.0.0.9/weathon/nlp/base/tokenizer.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1319 2022-10-02 01:55:42.000000 weathon-0.0.0.9/weathon/nlp/base/vocab.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/dataset/
+-rw-r--r--   0 lizhen     (501) staff       (20)     1361 2022-10-02 09:08:08.000000 weathon-0.0.0.9/weathon/nlp/dataset/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    11871 2022-10-09 14:05:11.000000 weathon-0.0.0.9/weathon/nlp/dataset/sentence_classification_dataset.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     9541 2022-10-02 09:08:08.000000 weathon-0.0.0.9/weathon/nlp/dataset/token_classification_dataset.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/factory/
+-rw-r--r--   0 lizhen     (501) staff       (20)        2 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/factory/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/factory/loss/
+-rw-r--r--   0 lizhen     (501) staff       (20)      856 2022-10-04 01:53:17.000000 weathon-0.0.0.9/weathon/nlp/factory/loss/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1466 2022-10-06 02:46:02.000000 weathon-0.0.0.9/weathon/nlp/factory/loss/casrel_loss.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      798 2022-10-06 02:46:14.000000 weathon-0.0.0.9/weathon/nlp/factory/loss/focal_loss.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1101 2022-10-06 02:46:35.000000 weathon-0.0.0.9/weathon/nlp/factory/loss/global_pointer_ce_loss.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      914 2022-10-06 02:46:25.000000 weathon-0.0.0.9/weathon/nlp/factory/loss/label_smoothing_ce_loss.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1879 2022-10-06 02:46:43.000000 weathon-0.0.0.9/weathon/nlp/factory/loss/r_drop_cross_entropy_loss.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/factory/metric/
+-rw-r--r--   0 lizhen     (501) staff       (20)      297 2022-10-04 01:48:04.000000 weathon-0.0.0.9/weathon/nlp/factory/metric/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1173 2022-10-04 01:20:12.000000 weathon-0.0.0.9/weathon/nlp/factory/metric/biaffine_span_metrics.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4874 2022-10-04 01:48:04.000000 weathon-0.0.0.9/weathon/nlp/factory/metric/metrics.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2015 2022-10-04 01:20:12.000000 weathon-0.0.0.9/weathon/nlp/factory/metric/span_metrics.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/factory/optimizer/
+-rw-r--r--   0 lizhen     (501) staff       (20)      590 2022-10-09 14:09:44.000000 weathon-0.0.0.9/weathon/nlp/factory/optimizer/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     9048 2022-10-03 11:27:17.000000 weathon-0.0.0.9/weathon/nlp/factory/optimizer/adafactor.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4953 2022-10-03 12:02:26.000000 weathon-0.0.0.9/weathon/nlp/factory/optimizer/adamw.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6476 2022-10-03 12:02:26.000000 weathon-0.0.0.9/weathon/nlp/factory/optimizer/madgrad.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1753 2022-10-06 02:45:46.000000 weathon-0.0.0.9/weathon/nlp/factory/optimizer/prior_wd.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/
+-rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-04 03:04:39.000000 weathon-0.0.0.9/weathon/nlp/model/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/ie/
+-rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/ie/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/
+-rw-r--r--   0 lizhen     (501) staff       (20)     1273 2022-10-04 03:15:12.000000 weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6979 2022-10-04 03:14:23.000000 weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/prompt_uie.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2859 2022-10-04 03:14:23.000000 weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_dataset.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2877 2022-10-04 03:04:39.000000 weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_predictor.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     5386 2022-10-04 03:14:23.000000 weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_task.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     5024 2022-10-04 03:04:39.000000 weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/utils.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/ner/
+-rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/ner/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/ner/biaffine_bert/
+-rw-r--r--   0 lizhen     (501) staff       (20)     1166 2022-10-04 03:47:14.000000 weathon-0.0.0.9/weathon/nlp/model/ner/biaffine_bert/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3042 2022-10-04 03:47:14.000000 weathon-0.0.0.9/weathon/nlp/model/ner/biaffine_bert/biaffine_bert.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2949 2022-10-04 03:47:14.000000 weathon-0.0.0.9/weathon/nlp/model/ner/biaffine_bert/biaffine_named_entity_recognition.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/ner/crf_bert/
+-rw-r--r--   0 lizhen     (501) staff       (20)      918 2022-10-04 05:09:01.000000 weathon-0.0.0.9/weathon/nlp/model/ner/crf_bert/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      577 2022-10-04 04:47:49.000000 weathon-0.0.0.9/weathon/nlp/model/ner/crf_bert/crf_bert.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/ner/global_pointer_bert/
+-rw-r--r--   0 lizhen     (501) staff       (20)     1316 2022-10-04 06:45:44.000000 weathon-0.0.0.9/weathon/nlp/model/ner/global_pointer_bert/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3072 2022-10-04 05:34:07.000000 weathon-0.0.0.9/weathon/nlp/model/ner/global_pointer_bert/global_pointer_bert.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2998 2022-10-04 06:45:44.000000 weathon-0.0.0.9/weathon/nlp/model/ner/global_pointer_bert/global_pointer_bert_named_entity_recognition.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/ner/span_bert/
+-rw-r--r--   0 lizhen     (501) staff       (20)     1269 2022-10-04 06:54:49.000000 weathon-0.0.0.9/weathon/nlp/model/ner/span_bert/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4186 2022-10-04 06:49:22.000000 weathon-0.0.0.9/weathon/nlp/model/ner/span_bert/span_bert.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     5583 2022-10-04 06:49:22.000000 weathon-0.0.0.9/weathon/nlp/model/ner/span_bert/span_bert_named_entity_recognition.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/
+-rw-r--r--   0 lizhen     (501) staff       (20)     1032 2022-10-04 07:03:49.000000 weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    11323 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/w2ner_bert.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     5388 2022-10-04 07:03:49.000000 weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_dataset.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6392 2022-10-04 07:03:49.000000 weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_predictor.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     9151 2022-10-04 07:03:49.000000 weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_task.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/prompt/
+-rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/prompt/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/prompt/prompt_bert/
+-rw-r--r--   0 lizhen     (501) staff       (20)     1090 2022-10-04 07:06:41.000000 weathon-0.0.0.9/weathon/nlp/model/prompt/prompt_bert/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/
+-rw-r--r--   0 lizhen     (501) staff       (20)     1396 2022-10-04 07:11:14.000000 weathon-0.0.0.9/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1945 2022-10-04 07:06:41.000000 weathon-0.0.0.9/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/prompt_ernie_ctm_nptag.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3277 2022-10-04 07:07:06.000000 weathon-0.0.0.9/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/prompt_ernie_ctm_nptag_tokenizer.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/re/
+-rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/re/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/
+-rw-r--r--   0 lizhen     (501) staff       (20)     1263 2022-10-04 07:16:08.000000 weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2865 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/casrel_bert.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     5141 2022-10-04 07:12:45.000000 weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_dataset.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4928 2022-10-04 07:12:45.000000 weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_predictor.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    12750 2022-10-04 07:12:45.000000 weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_task.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/
+-rw-r--r--   0 lizhen     (501) staff       (20)     1205 2022-10-04 08:24:48.000000 weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     9607 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/prgc_bert.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6483 2022-10-04 08:21:00.000000 weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_dataset.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     7695 2022-10-04 08:21:00.000000 weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_predictor.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    11907 2022-10-04 08:21:00.000000 weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_task.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/tc/
+-rw-r--r--   0 lizhen     (501) staff       (20)      668 2022-10-09 14:19:50.000000 weathon-0.0.0.9/weathon/nlp/model/tc/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/tc/bert/
+-rw-r--r--   0 lizhen     (501) staff       (20)        9 2022-10-09 14:15:00.000000 weathon-0.0.0.9/weathon/nlp/model/tc/bert/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/tc/ernie/
+-rw-r--r--   0 lizhen     (501) staff       (20)      948 2022-10-04 08:28:54.000000 weathon-0.0.0.9/weathon/nlp/model/tc/ernie/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/tm/
+-rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/tm/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/tm/bert/
+-rw-r--r--   0 lizhen     (501) staff       (20)      909 2022-10-04 08:33:30.000000 weathon-0.0.0.9/weathon/nlp/model/tm/bert/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/
+-rw-r--r--   0 lizhen     (501) staff       (20)     2028 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6067 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2684 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_dataset.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3751 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_predictor.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3679 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_task.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/nn/
+-rw-r--r--   0 lizhen     (501) staff       (20)      770 2022-10-09 14:19:36.000000 weathon-0.0.0.9/weathon/nlp/nn/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/nn/basic/
+-rw-r--r--   0 lizhen     (501) staff       (20)      683 2022-10-09 14:18:56.000000 weathon-0.0.0.9/weathon/nlp/nn/basic/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     5378 2022-10-09 14:52:42.000000 weathon-0.0.0.9/weathon/nlp/nn/basic/bert.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      892 2022-10-03 08:53:07.000000 weathon-0.0.0.9/weathon/nlp/nn/basic/ernie.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    10437 2022-10-03 09:25:19.000000 weathon-0.0.0.9/weathon/nlp/nn/basic/nezha.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6927 2022-10-09 14:17:36.000000 weathon-0.0.0.9/weathon/nlp/nn/basic/rnn.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    10685 2022-10-03 11:00:32.000000 weathon-0.0.0.9/weathon/nlp/nn/basic/roformer.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3390 2022-10-03 08:53:07.000000 weathon-0.0.0.9/weathon/nlp/nn/basic/textcnn.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3077 2022-10-03 11:00:32.000000 weathon-0.0.0.9/weathon/nlp/nn/biaffine_bert.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/nn/configuration/
+-rw-r--r--   0 lizhen     (501) staff       (20)      239 2022-10-03 08:58:28.000000 weathon-0.0.0.9/weathon/nlp/nn/configuration/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6343 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/nn/configuration/configuration_nezha.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     5912 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/nn/configuration/configuration_roformer.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      640 2022-10-03 11:03:54.000000 weathon-0.0.0.9/weathon/nlp/nn/crf_bert.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1707 2022-10-03 11:03:54.000000 weathon-0.0.0.9/weathon/nlp/nn/global_pointer_bert.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/
+-rw-r--r--   0 lizhen     (501) staff       (20)      760 2022-10-04 07:06:41.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1158 2022-10-03 10:43:24.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/biaffine_block.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2008 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/cnn_block.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    20178 2022-10-03 10:49:57.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/crf_block.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    13337 2022-10-03 11:00:32.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/ernie_ctm_block.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4542 2022-10-03 11:00:32.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/global_pointer_block.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1059 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/layer_norm_block.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    14574 2022-10-03 09:22:38.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/nezha_block.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1466 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/pooler_block.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1292 2022-10-03 11:00:32.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/position_embedding_block.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    14036 2022-10-03 09:34:38.000000 weathon-0.0.0.9/weathon/nlp/nn/layer/reformer_block.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2633 2022-10-03 11:04:20.000000 weathon-0.0.0.9/weathon/nlp/nn/prompt_bert.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1905 2022-10-03 11:05:22.000000 weathon-0.0.0.9/weathon/nlp/nn/span_bert.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2419 2022-10-03 11:05:31.000000 weathon-0.0.0.9/weathon/nlp/nn/text_level_gcn.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/predictor/
+-rw-r--r--   0 lizhen     (501) staff       (20)      327 2022-10-03 13:32:05.000000 weathon-0.0.0.9/weathon/nlp/predictor/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    14281 2022-10-04 01:09:19.000000 weathon-0.0.0.9/weathon/nlp/predictor/sequence_classification.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    21509 2022-10-04 01:13:33.000000 weathon-0.0.0.9/weathon/nlp/predictor/token_classification.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/processor/
+-rw-r--r--   0 lizhen     (501) staff       (20)        0 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/nlp/processor/__init__.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/processor/graph/
+-rw-r--r--   0 lizhen     (501) staff       (20)       73 2022-10-02 05:56:42.000000 weathon-0.0.0.9/weathon/nlp/processor/graph/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4368 2022-10-02 05:56:19.000000 weathon-0.0.0.9/weathon/nlp/processor/graph/text_level_gcn.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/processor/tokenizer/
+-rw-r--r--   0 lizhen     (501) staff       (20)      337 2022-10-02 05:54:45.000000 weathon-0.0.0.9/weathon/nlp/processor/tokenizer/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1498 2022-10-02 04:06:39.000000 weathon-0.0.0.9/weathon/nlp/processor/tokenizer/graph.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    17263 2022-10-09 15:15:26.000000 weathon-0.0.0.9/weathon/nlp/processor/tokenizer/transfomer.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      963 2022-10-02 03:06:00.000000 weathon-0.0.0.9/weathon/nlp/processor/tokenizer/vanilla.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/processor/vocab/
+-rw-r--r--   0 lizhen     (501) staff       (20)      101 2022-10-02 03:06:57.000000 weathon-0.0.0.9/weathon/nlp/processor/vocab/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3407 2022-10-02 02:17:29.000000 weathon-0.0.0.9/weathon/nlp/processor/vocab/char_vocab.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1732 2022-10-02 02:17:29.000000 weathon-0.0.0.9/weathon/nlp/processor/vocab/label_vocab.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      449 2022-10-02 02:19:09.000000 weathon-0.0.0.9/weathon/nlp/processor/vocab/transfomer_vocab.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2848 2022-10-02 02:17:29.000000 weathon-0.0.0.9/weathon/nlp/processor/vocab/word_vocab.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/nlp/task/
+-rw-r--r--   0 lizhen     (501) staff       (20)      540 2022-10-04 02:30:31.000000 weathon-0.0.0.9/weathon/nlp/task/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    17987 2022-10-04 02:30:31.000000 weathon-0.0.0.9/weathon/nlp/task/named_entity_recognition.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3721 2022-10-04 02:30:31.000000 weathon-0.0.0.9/weathon/nlp/task/prompt_masked_language_model.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    13309 2022-10-09 15:15:26.000000 weathon-0.0.0.9/weathon/nlp/task/sequence_classification.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4689 2022-10-09 15:15:26.000000 weathon-0.0.0.9/weathon/nlp/task/text_classification.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1987 2022-10-04 02:30:31.000000 weathon-0.0.0.9/weathon/nlp/task/text_level_gcn_classification.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4705 2022-10-04 02:30:31.000000 weathon-0.0.0.9/weathon/nlp/task/text_match.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2359 2022-10-04 02:30:31.000000 weathon-0.0.0.9/weathon/nlp/task/token_classification.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon/utils/
+-rw-r--r--   0 lizhen     (501) staff       (20)     2044 2022-10-09 14:31:12.000000 weathon-0.0.0.9/weathon/utils/__init__.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4930 2022-10-02 15:50:08.000000 weathon-0.0.0.9/weathon/utils/aho_corasick.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4790 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/utils/attack.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2373 2022-10-06 08:32:50.000000 weathon-0.0.0.9/weathon/utils/char_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    12460 2022-10-04 00:56:42.000000 weathon-0.0.0.9/weathon/utils/conlleval.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      706 2022-10-06 08:14:53.000000 weathon-0.0.0.9/weathon/utils/constants.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4546 2022-10-06 08:37:25.000000 weathon-0.0.0.9/weathon/utils/dictionary.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3814 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/utils/ema.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      668 2022-10-06 04:49:44.000000 weathon-0.0.0.9/weathon/utils/encrypt_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      621 2022-10-09 13:33:19.000000 weathon-0.0.0.9/weathon/utils/environment_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     9594 2022-10-06 04:51:59.000000 weathon-0.0.0.9/weathon/utils/file_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3878 2022-10-06 03:00:34.000000 weathon-0.0.0.9/weathon/utils/find_word.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4488 2022-10-06 04:55:20.000000 weathon-0.0.0.9/weathon/utils/gpu_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1457 2022-10-06 05:00:24.000000 weathon-0.0.0.9/weathon/utils/ip_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      627 2022-10-06 05:00:24.000000 weathon-0.0.0.9/weathon/utils/json_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6569 2022-10-06 05:00:24.000000 weathon-0.0.0.9/weathon/utils/label_studio_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     4481 2022-10-06 05:00:24.000000 weathon-0.0.0.9/weathon/utils/loss_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     5159 2022-10-03 02:16:46.000000 weathon-0.0.0.9/weathon/utils/minjoin.py
+-rw-r--r--   0 lizhen     (501) staff       (20)      661 2022-10-06 05:00:24.000000 weathon-0.0.0.9/weathon/utils/model_ensemble.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    21209 2022-10-06 05:00:24.000000 weathon-0.0.0.9/weathon/utils/ner_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6843 2022-10-09 15:19:18.000000 weathon-0.0.0.9/weathon/utils/optimizer_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     2434 2022-10-02 00:42:07.000000 weathon-0.0.0.9/weathon/utils/sampler.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     9394 2022-10-06 05:02:11.000000 weathon-0.0.0.9/weathon/utils/schedule_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3194 2022-10-06 08:37:25.000000 weathon-0.0.0.9/weathon/utils/states_machine.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     3678 2022-10-06 08:37:25.000000 weathon-0.0.0.9/weathon/utils/string_converter.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    25723 2022-10-06 05:46:56.000000 weathon-0.0.0.9/weathon/utils/string_similarity.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     5750 2022-10-06 08:23:36.000000 weathon-0.0.0.9/weathon/utils/string_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)    10283 2022-10-06 05:57:55.000000 weathon-0.0.0.9/weathon/utils/text_cluster.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     1334 2022-10-06 02:39:57.000000 weathon-0.0.0.9/weathon/utils/textrank.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     7762 2022-10-09 15:20:28.000000 weathon-0.0.0.9/weathon/utils/transformer_utils.py
+-rw-r--r--   0 lizhen     (501) staff       (20)     6909 2022-10-03 03:09:05.000000 weathon-0.0.0.9/weathon/utils/union_find.py
+drwxr-xr-x   0 lizhen     (501) staff       (20)        0 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon.egg-info/
+-rw-r--r--   0 lizhen     (501) staff       (20)      430 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon.egg-info/PKG-INFO
+-rw-r--r--   0 lizhen     (501) staff       (20)     7658 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon.egg-info/SOURCES.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)        1 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon.egg-info/dependency_links.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)        1 2022-10-02 00:36:48.000000 weathon-0.0.0.9/weathon.egg-info/not-zip-safe
+-rw-r--r--   0 lizhen     (501) staff       (20)      219 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon.egg-info/requires.txt
+-rw-r--r--   0 lizhen     (501) staff       (20)        8 2022-10-09 15:21:33.000000 weathon-0.0.0.9/weathon.egg-info/top_level.txt
```

### Comparing `weathon-0.0.0.8/setup.py` & `weathon-0.0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,12 +131,12 @@
         "seqeval==1.2.2",
         "paramiko==2.11.0",
         "Levenshtein==0.20.5",
         "mmh3==3.0.0",
         "pandas==1.3.3",
         "scipy >= 1.2.0",
         "requests==2.28.1",
-        "transformers >= 3.0.0",
+        "transformers >= 4.22.2",
         "scikit-learn >= 0.17.0",
         "pypinyin >= 0.47.1"
     ],
 )
```

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/animal.txt` & `weathon-0.0.0.9/weathon/data/dictionary/animal.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/antonym_word.txt` & `weathon-0.0.0.9/weathon/data/dictionary/antonym_word.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/car.txt` & `weathon-0.0.0.9/weathon/data/dictionary/car.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/family_name.txt` & `weathon-0.0.0.9/weathon/data/dictionary/family_name.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/finance.txt` & `weathon-0.0.0.9/weathon/data/dictionary/finance.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/food.txt` & `weathon-0.0.0.9/weathon/data/dictionary/food.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/it.txt` & `weathon-0.0.0.9/weathon/data/dictionary/it.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/legal.txt` & `weathon-0.0.0.9/weathon/data/dictionary/legal.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/medical.txt` & `weathon-0.0.0.9/weathon/data/dictionary/medical.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/place_name.txt` & `weathon-0.0.0.9/weathon/data/dictionary/place_name.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/professions.txt` & `weathon-0.0.0.9/weathon/data/dictionary/professions.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/same_pinyin.txt` & `weathon-0.0.0.9/weathon/data/dictionary/same_pinyin.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/same_stroke.txt` & `weathon-0.0.0.9/weathon/data/dictionary/same_stroke.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/simple2traditional.txt` & `weathon-0.0.0.9/weathon/data/dictionary/simple2traditional.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/stopwords.txt` & `weathon-0.0.0.9/weathon/data/dictionary/stopwords.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/traditional2simple.txt` & `weathon-0.0.0.9/weathon/data/dictionary/traditional2simple.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/data/dictionary/wechat_expression.txt` & `weathon-0.0.0.9/weathon/data/dictionary/wechat_expression.txt`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/base/dataset.py` & `weathon-0.0.0.9/weathon/nlp/base/dataset.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,87 +5,83 @@
 # @github  : https://github.com/Lizhen0628
 # @Description:
 
 import json
 import copy
 import codecs
 import pandas as pd
-
+from pathlib import Path
+from typing import Union, List, Set, Dict
 from collections import defaultdict
 from torch.utils.data import Dataset
 from pandas.core.frame import DataFrame
 
 
+# TODO:dataset split
 class BaseDataset(Dataset):
     """
     Dataset基类
 
     Args:
         data (:obj:`DataFrame` or :obj:`string`): 数据或者数据地址
         categories (:obj:`list`, optional, defaults to `None`): 数据类别
         is_retain_df (:obj:`bool`, optional, defaults to False): 是否将DataFrame格式的原始数据复制到属性retain_df中
         is_retain_dataset (:obj:`bool`, optional, defaults to False): 是否将处理成dataset格式的原始数据复制到属性retain_dataset中
         is_train (:obj:`bool`, optional, defaults to True): 数据集是否为训练集数据
         is_test (:obj:`bool`, optional, defaults to False): 数据集是否为测试集数据
     """  # noqa: ignore flake8"
 
-    def __init__(self, data, categories=None, is_retain_df: bool = False, is_retain_dataset: bool = False,
-                 is_train: bool = True,
-                 is_test: bool = False):
+    def __init__(self,
+                 data: Union[DataFrame, str, Path],  # 数据或者数据地址
+                 categories=None,  # 数据类别
+                 is_retain_df: bool = False,  # 是否将DataFrame格式的原始数据复制到属性retain_df中
+                 is_retain_dataset: bool = False,  # 是否将处理成dataset格式的原始数据复制到属性retain_dataset中
+                 is_test: bool = False
+                 ):
 
         self.is_test = is_test
-        self.is_train = is_train
         self.is_retain_df = is_retain_df
         self.is_retain_dataset = is_retain_dataset
 
-        if self.is_test is True:
-            self.is_train = False
-
         if isinstance(data, DataFrame):
             if 'label' in data.columns:
-                data['label'] = data['label'].apply(lambda x: str(x))
-
-            if self.is_retain_df:
-                self.df = data
+                data.loc[:]['label'] = data.loc[:]['label'].apply(lambda x: str(x))
 
+            self.df = data if is_retain_df else None
             self.dataset = self._convert_to_dataset(data)
         else:
             self.dataset = self._load_dataset(data)
 
-        if categories is None:
-            self.categories = self._get_categories()
-        else:
-            self.categories = categories
+        self.retain_dataset = copy.deepcopy(self.dataset) if is_retain_dataset else None
+
+        self.categories = categories if categories else self._get_categories()
 
         if self.categories is not None:
             self.cat2id = dict(zip(self.categories, range(len(self.categories))))
             self.id2cat = dict(zip(range(len(self.categories)), self.categories))
 
             self.class_num = len(self.cat2id)
 
     def _get_categories(self):
-        return None
+        raise NotImplementedError("_get_categories method not implement")
 
-    def _load_dataset(self, data_path):
+    def _load_dataset(self, data_path: Union[str, Path]):
         """
         加载数据集
 
         Args:
             data_path (:obj:`string`): 数据地址
         """  # noqa: ignore flake8"
 
         data_df = self._read_data(data_path)
-
-        if self.is_retain_df:
-            self.df = data_df
-
+        self.df = data_df if self.is_retain_df else None
         return self._convert_to_dataset(data_df)
 
     def _convert_to_dataset(self, data_df):
-        pass
+        raise NotImplementedError("_convert_to_dataset method not implement")
 
     def _read_data(self, data_path, data_format=None, skiprows=-1):
         """
         读取所需数据
         Args:
             data_path (:obj:`string`): 数据地址
             data_format (:obj:`string`, defaults to `None`): 数据存储格式
@@ -96,15 +92,15 @@
             data_format = data_path.split('.')[-1]
 
         if data_format == 'csv':
             data_df = pd.read_csv(data_path, dtype={'label': str})
         elif data_format == 'json':
             try:
                 data_df = pd.read_json(data_path, dtype={'label': str})
-            except:
+            except ValueError:
                 data_df = self.read_line_json(data_path)
         elif data_format == 'tsv':
             data_df = pd.read_csv(data_path, sep='\t', dtype={'label': str})
         elif data_format == 'txt':
             data_df = pd.read_csv(data_path, sep='\t', dtype={'label': str})
         else:
             raise ValueError("The data format does not exist")
@@ -122,59 +118,53 @@
         datasets = []
 
         with codecs.open(data_path, mode='r', encoding='utf8') as f:
             reader = f.readlines()
             for index, line in enumerate(reader):
                 if index == skiprows:
                     continue
-                line = json.loads(line)
-                tokens = line['text']
-                label = line['label']
-                datasets.append({'text': tokens.strip(), 'label': label})
-
+                json_line = json.loads(line)
+                datasets.append(json_line)
+                # tokens = line['text']
+                # label = line['label']
+                # datasets.append({'text': tokens.strip(), 'label': label})
         return pd.DataFrame(datasets)
 
     def convert_to_ids(self, tokenizer):
         """
         将文本转化成id的形式
         Args:
             tokenizer: 编码器
         """
         if tokenizer.tokenizer_type == 'vanilla':
             features = self._convert_to_vanilla_ids(tokenizer)
-        elif tokenizer.tokenizer_type == 'transfomer':
+        elif tokenizer.tokenizer_type == 'transformer':
             features = self._convert_to_transfomer_ids(tokenizer)
         elif tokenizer.tokenizer_type == 'customized':
             features = self._convert_to_customized_ids(tokenizer)
         else:
             raise ValueError("The tokenizer type does not exist")
 
-        if self.is_retain_dataset:
-            self.retain_dataset = copy.deepcopy(self.dataset)
-
         self.dataset = features
 
     def _convert_to_transfomer_ids(self, bert_tokenizer):
         pass
 
     def _convert_to_vanilla_ids(self, vanilla_tokenizer):
         pass
 
     def _convert_to_customized_ids(self, customized_tokenizer):
         pass
 
-    def _get_input_length(self, text, bert_tokenizer):
-        pass
-
     @property
-    def dataset_cols(self):
+    def dataset_cols(self) -> List[str]:
         return list(self.dataset[0].keys())
 
     @property
-    def to_device_cols(self):
+    def to_device_cols(self) -> List[str]:
         return list(self.dataset[0].keys())
 
     @property
     def sample_num(self):
         return len(self.dataset)
 
     @property
```

### Comparing `weathon-0.0.0.8/weathon/nlp/base/model.py` & `weathon-0.0.0.9/weathon/nlp/base/model.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/base/predictor.py` & `weathon-0.0.0.9/weathon/nlp/base/predictor.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/base/task.py` & `weathon-0.0.0.9/weathon/nlp/base/task.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 # @Author  : LiZhen
 # @FileName: task.py
 # @github  : https://github.com/Lizhen0628
 # @Description:
 
 import torch
 from torch.utils.data._utils.collate import default_collate
-from weathon.utils import LossUtils
-from weathon.utils import EMA
+from weathon.utils import EMA, ScheduleUtils
 
 
 class BaseTask(object):
     """
     所有Task类的基类，封装Task类通用的方法和属性
 
     Args:
@@ -37,18 +36,19 @@
             scheduler=None,
             n_gpu=1,
             device=None,
             cuda_device=0,
             ema_decay=None,
             **kwargs
     ):
+        self.logs = dict()
         self.fit_counter = 0
         self.module = module
         self.optimizer = optimizer
-        self.loss_function = LossUtils.get_loss(loss_function)
+        self.loss_function = loss_function
 
         self.class_num = class_num
         self.scheduler = scheduler
 
         self.n_gpu = n_gpu
 
         self.device = device
@@ -86,15 +86,19 @@
     def _finish_train_begin(self, **kwargs):
         pass
 
     def _prepare_train_begin_record(self, **kwargs):
         pass
 
     def _on_train_begin_record(self, **kwargs):
-        pass
+        """ 训练开始之前的初始化操作：
+        1. 日志初始化
+        """
+        self.logs['global_step'] = 0
+        self.logs['global_loss'] = 0
 
     def _finish_train_begin_record(self, **kwargs):
         pass
 
     def _prepare_epoch_begin(self, **kwargs):
         pass
 
@@ -103,16 +107,27 @@
 
     def _finish_epoch_begin(self, **kwargs):
         pass
 
     def _prepare_epoch_begin_record(self, **kwargs):
         pass
 
+    def _prepare_scheduler(self, warmup_proportion, epochs, **kwargs):
+        if warmup_proportion:
+            num_training_steps = self.train_generator_length * epochs
+            num_warmup_steps = int(warmup_proportion * num_training_steps)
+            scheduler = ScheduleUtils.get_linear_schedule_with_warmup(self.optimizer,
+                                                                      num_warmup_steps=num_warmup_steps,
+                                                                      num_training_steps=num_training_steps)
+
     def _on_epoch_begin_record(self, **kwargs):
-        pass
+        self.logs['epoch_loss'] = 0
+        # 占位作用，子类仅使用单个指标进行评价，则直接使用该字段即可
+        self.logs['epoch_evaluation'] = 0
+        self.logs['epoch_step'] = 0
 
     def _finish_epoch_begin_record(self, **kwargs):
         pass
 
     def _prepare_step_begin(self, **kwargs):
         pass
 
@@ -148,15 +163,15 @@
 
     def _finish_compute_loss_record(self, **kwargs):
         pass
 
     def _prepare_backward(self, **kwargs):
         pass
 
-    def _on_backward(self, ):
+    def _on_backward(self, **kwargs):
         pass
 
     def _finish_backward(self, **kwargs):
         pass
 
     def _prepare_backward_record(self, **kwargs):
         pass
@@ -268,22 +283,18 @@
 
     def _on_evaluate_end(self, **kwargs):
         pass
 
     def _on_evaluate_end_record(self, **kwargs):
         pass
 
-    def _get_module_inputs_on_train(self):
+    def _get_module_inputs_on_train(self, **kwargs):
         pass
 
     def _get_module_label_on_train(self):
         pass
 
-    def _get_module_inputs_on_eval(self):
+    def _get_module_inputs_on_eval(self, **kwargs):
         pass
 
     def _get_module_label_on_eval(self):
         pass
-
-
-
-
```

### Comparing `weathon-0.0.0.8/weathon/nlp/base/tokenizer.py` & `weathon-0.0.0.9/weathon/nlp/base/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 
 
 class BaseTokenizer(object, metaclass=abc.ABCMeta):
     """
     分词器基类
     """
 
-    def __init__(self, vocab: Union[BaseVocab, BertTokenizer, AutoTokenizer], max_seq_length: int):
+    def __init__(self, vocab: Union[BaseVocab, BertTokenizer, AutoTokenizer], max_seq_len: int):
         self.vocab = vocab
-        self.max_seq_length = max_seq_length
+        self.max_seq_len = max_seq_len
 
     def tokenize(self, text: str) -> List[str]:
         return self.vocab.tokenize(text)
 
     def pad_and_truncate(self, sequence: List[int], maxlen: int, dtype: str = 'int64', padding: str = 'post',
                          truncating='post', value=0) -> np.ndarray:
         seq = (np.ones(maxlen) * value).astype(dtype)
```

### Comparing `weathon-0.0.0.8/weathon/nlp/base/vocab.py` & `weathon-0.0.0.9/weathon/nlp/base/vocab.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/dataset/__init__.py` & `weathon-0.0.0.9/weathon/nlp/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/dataset/sentence_classification_dataset.py` & `weathon-0.0.0.9/weathon/nlp/dataset/sentence_classification_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,63 +3,62 @@
 # @Author  : LiZhen
 # @FileName: sentence_classification_dataset.py.py
 # @github  : https://github.com/Lizhen0628
 # @Description:
 
 import copy
 import numpy as np
+from typing import List, Dict
 from weathon.nlp.base import BaseDataset
+from weathon.nlp.processor.tokenizer import SentenceTokenizer
 
 
 class SentenceClassificationDataset(BaseDataset):
     """
     用于序列分类任务的Dataset
     """
 
-    def _get_categories(self):
+    def _get_categories(self) -> List[str]:
         return sorted(list(set([data['label'] for data in self.dataset])))
 
-    def _convert_to_dataset(self, data_df):
+    def _convert_to_dataset(self, data_df) -> List[Dict]:
 
         dataset = []
-
-        data_df['text'] = data_df['text'].apply(lambda x: x.lower().strip())
+        data_df.loc[:]['text'] = data_df.loc[:]['text'].apply(lambda x: str(x).lower().strip())
 
         feature_names = list(data_df.columns)
         for index_, row_ in enumerate(data_df.itertuples()):
             dataset.append({
                 feature_name_: getattr(row_, feature_name_)
                 for feature_name_ in feature_names
             })
 
         return dataset
 
-    def _convert_to_transfomer_ids(self, bert_tokenizer):
+    def _convert_to_transfomer_ids(self, bert_tokenizer: SentenceTokenizer):
 
         features = []
         for (index_, row_) in enumerate(self.dataset):
             input_ids = bert_tokenizer.sequence_to_ids(row_['text'])
-
             input_ids, input_mask, segment_ids = input_ids
-
             feature = {
                 'input_ids': input_ids,
                 'attention_mask': input_mask,
                 'token_type_ids': segment_ids
             }
 
             if not self.is_test:
                 label_ids = self.cat2id[row_['label']]
                 feature['label_ids'] = label_ids
 
             features.append(feature)
 
         return features
 
-    def _convert_to_vanilla_ids(self, vanilla_tokenizer):
+    def _convert_to_vanilla_ids(self, vanilla_tokenizer) -> List[Dict]:
 
         features = []
         for (index_, row_) in enumerate(self.dataset):
             tokens = vanilla_tokenizer.tokenize(row_['text'])
             length = len(tokens)
             input_ids = vanilla_tokenizer.sequence_to_ids(tokens)
```

### Comparing `weathon-0.0.0.8/weathon/nlp/dataset/token_classification_dataset.py` & `weathon-0.0.0.9/weathon/nlp/dataset/token_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/loss/__init__.py` & `weathon-0.0.0.9/weathon/nlp/factory/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/loss/casrel_loss.py` & `weathon-0.0.0.9/weathon/nlp/factory/loss/casrel_loss.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/loss/focal_loss.py` & `weathon-0.0.0.9/weathon/nlp/factory/loss/focal_loss.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/loss/global_pointer_ce_loss.py` & `weathon-0.0.0.9/weathon/nlp/factory/loss/global_pointer_ce_loss.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/loss/label_smoothing_ce_loss.py` & `weathon-0.0.0.9/weathon/nlp/factory/loss/label_smoothing_ce_loss.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/loss/r_drop_cross_entropy_loss.py` & `weathon-0.0.0.9/weathon/nlp/factory/loss/r_drop_cross_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/metric/biaffine_span_metrics.py` & `weathon-0.0.0.9/weathon/nlp/factory/metric/biaffine_span_metrics.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/metric/metrics.py` & `weathon-0.0.0.9/weathon/nlp/factory/metric/metrics.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/metric/span_metrics.py` & `weathon-0.0.0.9/weathon/nlp/factory/metric/span_metrics.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/optimizer/__init__.py` & `weathon-0.0.0.9/weathon/nlp/factory/optimizer/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from transformers import AdamW
 from weathon.nlp.factory.optimizer.adafactor import Adafactor
 from weathon.nlp.factory.optimizer.madgrad import MADGRAD
 from weathon.nlp.factory.optimizer.prior_wd import PriorWD
-from torch.optim import Adadelta, Adagrad, Adam, SparseAdam, Adamax, ASGD, LBFGS, RMSprop, Rprop, SGD
+from torch.optim import Adadelta, Adagrad, Adam,AdamW, SparseAdam, Adamax, ASGD, LBFGS, RMSprop, Rprop, SGD
 
 all_optimizers_dict = dict(
     adadelta=Adadelta,
     adagrad=Adagrad,
     adam=Adam,
     sparseadam=SparseAdam,
     adamax=Adamax,
```

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/optimizer/adafactor.py` & `weathon-0.0.0.9/weathon/nlp/factory/optimizer/adafactor.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/optimizer/adamw.py` & `weathon-0.0.0.9/weathon/nlp/factory/optimizer/adamw.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/optimizer/madgrad.py` & `weathon-0.0.0.9/weathon/nlp/factory/optimizer/madgrad.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/factory/optimizer/prior_wd.py` & `weathon-0.0.0.9/weathon/nlp/factory/optimizer/prior_wd.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/prompt_uie.py` & `weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/prompt_uie.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_dataset.py` & `weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_dataset.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_predictor.py` & `weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_predictor.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_task.py` & `weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/prompt_uie_information_extraction_task.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ie/prompt_uie/utils.py` & `weathon-0.0.0.9/weathon/nlp/model/ie/prompt_uie/utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/biaffine_bert/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/biaffine_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/biaffine_bert/biaffine_bert.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/biaffine_bert/biaffine_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/biaffine_bert/biaffine_named_entity_recognition.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/biaffine_bert/biaffine_named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/crf_bert/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/crf_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/crf_bert/crf_bert.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/crf_bert/crf_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/global_pointer_bert/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/global_pointer_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/global_pointer_bert/global_pointer_bert.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/global_pointer_bert/global_pointer_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/global_pointer_bert/global_pointer_bert_named_entity_recognition.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/global_pointer_bert/global_pointer_bert_named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/span_bert/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/span_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/span_bert/span_bert.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/span_bert/span_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/span_bert/span_bert_named_entity_recognition.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/span_bert/span_bert_named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/w2ner_bert.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/w2ner_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_dataset.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_dataset.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_predictor.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_predictor.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_task.py` & `weathon-0.0.0.9/weathon/nlp/model/ner/w2ner_bert/w2ner_named_entity_recognition_task.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/prompt/prompt_bert/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/prompt/prompt_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/prompt_ernie_ctm_nptag.py` & `weathon-0.0.0.9/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/prompt_ernie_ctm_nptag.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/prompt_ernie_ctm_nptag_tokenizer.py` & `weathon-0.0.0.9/weathon/nlp/model/prompt/prompt_ernie_ctm_nptag/prompt_ernie_ctm_nptag_tokenizer.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/casrel_bert.py` & `weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/casrel_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_dataset.py` & `weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_dataset.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_predictor.py` & `weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_predictor.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_task.py` & `weathon-0.0.0.9/weathon/nlp/model/re/casrel_bert/casrel_relation_extraction_task.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/prgc_bert.py` & `weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/prgc_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_dataset.py` & `weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_dataset.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_predictor.py` & `weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_predictor.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_task.py` & `weathon-0.0.0.9/weathon/nlp/model/re/prgc_bert/prgc_relation_extraction_task.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/tc/bert/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/tm/bert/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from weathon.nlp.dataset import SentenceClassificationDataset as Dataset
-from weathon.nlp.dataset import SentenceClassificationDataset as BertTCDataset
+from weathon.nlp.dataset import PairMergeSentenceClassificationDataset as Dataset
+from weathon.nlp.dataset import PairMergeSentenceClassificationDataset as BertTMDataset
 
-from weathon.nlp.processor.tokenizer import SentenceTokenizer as Tokenizer
-from weathon.nlp.processor.tokenizer import SentenceTokenizer as BertTCTokenizer
+from weathon.nlp.processor.tokenizer import PairTokenizer as Tokenizer
+from weathon.nlp.processor.tokenizer import PairTokenizer as BertTMTokenizer
 
 from weathon.nlp.nn import BertConfig
 from weathon.nlp.nn import BertConfig as ModuleConfig
 
 from weathon.nlp.nn import Bert
 from weathon.nlp.nn import Bert as Module
 
 from weathon.utils.optimizer_utils import OptimizerUtils
 
 get_default_model_optimizer = OptimizerUtils.get_default_bert_optimizer
 get_default_bert_optimizer = OptimizerUtils.get_default_bert_optimizer
 
-from weathon.nlp.task import TCTask as Task
-from weathon.nlp.task import TCTask as BertTCTask
+from weathon.nlp.task import TMTask as Task
+from weathon.nlp.task import TMTask as BertTMTask
 
-from weathon.nlp.predictor import TCPredictor as Predictor
-from weathon.nlp.predictor import TCPredictor as BertTCPredictor
+from weathon.nlp.predictor import TMPredictor as Predictor
+from weathon.nlp.predictor import TMPredictor as BertTMPredictor
```

### Comparing `weathon-0.0.0.8/weathon/nlp/model/tc/ernie/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/tc/ernie/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/__init__.py` & `weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse.py` & `weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_dataset.py` & `weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_dataset.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_predictor.py` & `weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_predictor.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_task.py` & `weathon-0.0.0.9/weathon/nlp/model/tm/unsupervised_simcse/unsupervised_simcse_task.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/basic/__init__.py` & `weathon-0.0.0.9/weathon/nlp/nn/basic/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 # @Time    : 2022/10/3 16:01
 # @Author  : LiZhen
 # @FileName: __init__.py.py
 # @github  : https://github.com/Lizhen0628
 # @Description:
 
 from weathon.nlp.nn.basic.textcnn import TextCNN
-from weathon.nlp.nn.basic.rnn import RNN
+from weathon.nlp.nn.basic.rnn import RNN, RNNForSequenceClassification, RNNForTokenizerClassification
 from weathon.nlp.nn.basic.bert import Bert, BertForSequenceClassification, BertForTokenClassification
 from weathon.nlp.nn.basic.ernie import Ernie, ErnieForSequenceClassification, ErnieForTokenClassification
 from weathon.nlp.nn.basic.nezha import NeZha, NeZhaForSequenceClassification
 from weathon.nlp.nn.basic.roformer import RoFormer, RoFormerForSequenceClassification
```

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/basic/bert.py` & `weathon-0.0.0.9/weathon/nlp/nn/basic/bert.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 # @github  : https://github.com/Lizhen0628
 # @Description:
 
 
 import torch
 from torch import nn
 from torch import Tensor
-from transformers import BertModel
-from transformers import BertPreTrainedModel
+from typing import Union
+from pathlib import Path
+from transformers import BertPreTrainedModel, AutoModel, AutoConfig, BertConfig, BertModel
 
 
 class Bert(BertPreTrainedModel):
     """
     原始的BERT模型
 
     Args:
@@ -28,21 +29,31 @@
 
     Reference:
         [1] BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding  
     """  # noqa: ignore flake8"
 
     def __init__(
             self,
-            config,
+            transformer_model_name: Union[str, Path],
+            num_labels: int,
             encoder_trained=True,
             pooling='cls_with_pooler'
     ):
+
+        try:
+            config = AutoConfig.from_pretrained(transformer_model_name, num_labels=num_labels)
+        except ValueError:
+            config = BertConfig.from_pretrained(transformer_model_name, num_labels=num_labels)
+
         super(Bert, self).__init__(config)
+        try:
+            self.bert = AutoModel.from_pretrained(config.name_or_path, config=config)
+        except ValueError:
+            self.bert = BertModel(config)
 
-        self.bert = BertModel(config)
         self.pooling = pooling
 
         for param in self.bert.parameters():
             param.requires_grad = encoder_trained
 
         self.num_labels = config.num_labels
 
@@ -73,110 +84,52 @@
         elif pooling == 'cls':
             return sequence_feature[-1][:, 0, :]
         else:
             raise Exception("unknown pooling {}".format(pooling))
 
         return self.mask_pooling(sequence_feature, attention_mask)
 
-    def get_encoder_feature(
-            self,
-            encoder_output,
-            attention_mask,
-            pooling=None
-    ):
+    def get_encoder_feature(self, encoder_output, attention_mask, pooling=None):
         if self.task == 'SequenceLevel':
-            return self.sequence_pooling(
-                encoder_output,
-                attention_mask,
-                pooling
-            )
+            return self.sequence_pooling(encoder_output, attention_mask, pooling)
         elif self.task == 'TokenLevel':
             return encoder_output[-1]
         else:
             return encoder_output[-1][:, 0, :]
 
     def forward(
             self,
             input_ids=None,
             attention_mask=None,
             token_type_ids=None,
             position_ids=None,
             **kwargs
     ):
-        outputs = self.bert(
-            input_ids,
-            attention_mask=attention_mask,
-            token_type_ids=token_type_ids,
-            position_ids=position_ids,
-            return_dict=True,
-            output_hidden_states=True
-        )
 
+        outputs = self.bert(input_ids, attention_mask=attention_mask, token_type_ids=token_type_ids,
+                            position_ids=position_ids, return_dict=True, output_hidden_states=True)
         encoder_feature = self.get_encoder_feature(outputs, attention_mask)
-
         encoder_feature = self.dropout(encoder_feature)
         out = self.classifier(encoder_feature)
-
         return out
 
 
 class BertForSequenceClassification(BertPreTrainedModel):
-    """
-    基于BERT的文本分类模型
-
-    Args:
-        config:
-            模型的配置对象
-        encoder_trained (:obj:`bool`, optional, defaults to True):
-            bert参数是否可训练，默认可训练
-
-    Reference:
-        [1] BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding  
-    """  # noqa: ignore flake8"
 
     def __init__(
             self,
-            config,
-            encoder_trained=True
-    ):
-        super(BertForSequenceClassification, self).__init__(config)
-
-        self.bert = BertModel(config)
-
-        for param in self.bert.parameters():
-            param.requires_grad = encoder_trained
-
-        self.num_labels = config.num_labels
-
-        self.dropout = nn.Dropout(config.hidden_dropout_prob)
-        self.classifier = nn.Linear(config.hidden_size, self.num_labels)
-
-        self.init_weights()
-
-    def forward(
-            self,
-            input_ids=None,
-            attention_mask=None,
-            token_type_ids=None,
-            position_ids=None,
-            **kwargs
+            transformer_model_name: str,
+            num_labels: int,
+            encoder_trained=True,
+            pooling='cls_with_pooler'
     ):
-        outputs = self.bert(
-            input_ids,
-            attention_mask=attention_mask,
-            token_type_ids=token_type_ids,
-            position_ids=position_ids
-        )
-
-        sequence_output = outputs[1]
-
-        sequence_output = self.dropout(sequence_output)
-        out = self.classifier(sequence_output)
-
-        return out
+        super(BertForSequenceClassification, self).__init__(transformer_model_name=transformer_model_name,
+                                                            num_labels=num_labels, encoder_trained=encoder_trained,
+                                                            pooling=pooling)
+        self.task = 'SequenceLevel'
 
 
 class BertForTokenClassification(BertPreTrainedModel):
     """
     基于BERT的命名实体模型
 
     Args:
@@ -187,45 +140,16 @@
 
     Reference:
         [1] BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding  
     """  # noqa: ignore flake8"
 
     def __init__(
             self,
-            config,
+            transformer_model_name: str,
+            num_labels: int,
             encoder_trained=True
     ):
-        super(BertForTokenClassification, self).__init__(config)
-
-        self.bert = BertModel(config)
-
-        for param in self.bert.parameters():
-            param.requires_grad = encoder_trained
 
-        self.num_labels = config.num_labels
+        super(BertForTokenClassification, self).__init__(transformer_model_name=transformer_model_name,
+                                                            num_labels=num_labels, encoder_trained=encoder_trained)
 
-        self.dropout = nn.Dropout(config.hidden_dropout_prob)
-        self.classifier = nn.Linear(config.hidden_size, self.num_labels)
-
-        self.init_weights()
-
-    def forward(
-            self,
-            input_ids=None,
-            attention_mask=None,
-            token_type_ids=None,
-            position_ids=None,
-            **kwargs
-    ):
-        outputs = self.bert(
-            input_ids,
-            attention_mask=attention_mask,
-            token_type_ids=token_type_ids,
-            position_ids=position_ids
-        )
-
-        sequence_output = outputs[0]
-
-        sequence_output = self.dropout(sequence_output)
-        out = self.classifier(sequence_output)
-
-        return out
+        self.task = 'TokenLevel'
```

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/basic/ernie.py` & `weathon-0.0.0.9/weathon/nlp/nn/basic/ernie.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/basic/nezha.py` & `weathon-0.0.0.9/weathon/nlp/nn/basic/nezha.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/basic/rnn.py` & `weathon-0.0.0.9/weathon/nlp/nn/basic/rnn.py`

 * *Files 11% similar despite different names*

```diff
@@ -173,7 +173,57 @@
 
         out = self.linear(F.relu(hidden))
         out = self.fc_dropout(out)
 
         output = self.classify(F.relu(out))
 
         return output
+
+
+class RNNForSequenceClassification(RNN):
+
+    def forward(
+            self,
+            input_ids: torch.LongTensor,
+            length: torch.LongTensor,
+            **kwargs
+    ):
+        device = input_ids.device
+        batch_size = input_ids.size()[0]
+
+        out = self.embed(input_ids)
+        out = self.embed_dropout(out)
+
+        if self.bidirectional is True:
+            hidden = self.init_hidden(batch_size, 2, device)
+        else:
+            hidden = self.init_hidden(batch_size, 1, device)
+
+        self.rnn.flatten_parameters()
+        out = pack_padded_sequence(
+            out,
+            length,
+            batch_first=True,
+            enforce_sorted=False
+        )
+        _, hidden = self.rnn(out, hidden)
+        if self.rnn_cell == 'lstm':
+            hidden = hidden[0]
+
+        hidden = self.get_last_hidden_output(hidden)
+
+        out = self.linear(F.relu(hidden))
+        out = self.fc_dropout(out)
+
+        output = self.classify(F.relu(out))
+
+        return output
+
+
+class RNNForTokenizerClassification(RNN):
+    def forward(
+            self,
+            input_ids: torch.LongTensor,
+            length: torch.LongTensor,
+            **kwargs
+    ):
+        pass
```

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/basic/roformer.py` & `weathon-0.0.0.9/weathon/nlp/nn/basic/roformer.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/basic/textcnn.py` & `weathon-0.0.0.9/weathon/nlp/nn/basic/textcnn.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/biaffine_bert.py` & `weathon-0.0.0.9/weathon/nlp/nn/biaffine_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/configuration/configuration_nezha.py` & `weathon-0.0.0.9/weathon/nlp/nn/configuration/configuration_nezha.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/configuration/configuration_roformer.py` & `weathon-0.0.0.9/weathon/nlp/nn/configuration/configuration_roformer.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/crf_bert.py` & `weathon-0.0.0.9/weathon/nlp/nn/crf_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/global_pointer_bert.py` & `weathon-0.0.0.9/weathon/nlp/nn/global_pointer_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/__init__.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/biaffine_block.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/biaffine_block.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/cnn_block.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/cnn_block.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/crf_block.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/crf_block.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/ernie_ctm_block.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/ernie_ctm_block.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/global_pointer_block.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/global_pointer_block.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/layer_norm_block.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/layer_norm_block.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/nezha_block.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/nezha_block.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/pooler_block.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/pooler_block.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/position_embedding_block.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/position_embedding_block.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/layer/reformer_block.py` & `weathon-0.0.0.9/weathon/nlp/nn/layer/reformer_block.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/prompt_bert.py` & `weathon-0.0.0.9/weathon/nlp/nn/prompt_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/span_bert.py` & `weathon-0.0.0.9/weathon/nlp/nn/span_bert.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/nn/text_level_gcn.py` & `weathon-0.0.0.9/weathon/nlp/nn/text_level_gcn.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/predictor/sequence_classification.py` & `weathon-0.0.0.9/weathon/nlp/predictor/sequence_classification.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/predictor/token_classification.py` & `weathon-0.0.0.9/weathon/nlp/predictor/token_classification.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/processor/graph/text_level_gcn.py` & `weathon-0.0.0.9/weathon/nlp/processor/graph/text_level_gcn.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/processor/tokenizer/graph.py` & `weathon-0.0.0.9/weathon/nlp/processor/tokenizer/graph.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/processor/tokenizer/transfomer.py` & `weathon-0.0.0.9/weathon/nlp/processor/tokenizer/transfomer.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,27 @@
     Transfomer文本编码器，用于对文本进行分词、ID化、填充等操作
 
     Args:
         vocab: transformers词典类对象、词典地址或词典名，用于实现文本分词和ID化
         max_seq_len (:obj:`int`): 预设的文本最大长度
     """  # noqa: ignore flake8"
 
-    def __init__(self, vocab: Union[BertTokenizer, AutoTokenizer, BaseVocab], max_seq_len: int, max_seq_length: int):
-        super().__init__(vocab, max_seq_length)
+    def __init__(self, vocab: Union[BertTokenizer, AutoTokenizer, BaseVocab], max_seq_len: int):
+        super().__init__(vocab, max_seq_len)
         if isinstance(vocab, str):
             # TODO: 改成由自定义的字典所决定
             try:
                 vocab = AutoTokenizer.from_pretrained(vocab)
             except ValueError:
                 vocab = BertTokenizer.from_pretrained(vocab)
 
         self.vocab = vocab
         self.max_seq_len = max_seq_len
         self.additional_special_tokens = set()
-        self.tokenizer_type = 'transfomer'
+        self.tokenizer_type = 'transformer'
 
     @staticmethod
     def _is_control(ch: str) -> bool:
         """控制类字符判断
         """
         return unicodedata.category(ch) in ('Cc', 'Cf')
 
@@ -94,18 +94,19 @@
         return token_mapping
 
     def sequence_to_ids(self, sequence_a: Union[str, List[str]], sequence_b: Union[str, List[str]] = None,
                         **kwargs) -> Tuple:
         return self.pair_to_ids(sequence_a, sequence_b, **kwargs) if sequence_b else self.sentence_to_ids(sequence_a,
                                                                                                           **kwargs)
 
-    def sentence_to_ids(self, sequence: Union[str, List[str]]) -> Tuple[np.ndarray, np.ndarray, np.ndarray, int]:
+    def sentence_to_ids(self, sequence: Union[str, List[str]], return_sequence_length: bool = False) -> Tuple[
+        np.ndarray, np.ndarray, np.ndarray]:
         if type(sequence) == str:
             sequence = self.tokenize(sequence)
-
+        token_length = len(sequence)
         # 对超长序列进行截断
         if len(sequence) > self.max_seq_len - 2:
             sequence = sequence[0:(self.max_seq_len - 2)]
         # 分别在首尾拼接特殊符号
         sequence = ['[CLS]'] + sequence + ['[SEP]']
         segment_ids = [0] * len(sequence)
         # ID化
@@ -119,18 +120,23 @@
         # 对seq拼接填充序列
         sequence += padding
 
         sequence = np.asarray(sequence, dtype='int64')
         sequence_mask = np.asarray(sequence_mask, dtype='int64')
         segment_ids = np.asarray(segment_ids, dtype='int64')
 
-        return sequence, sequence_mask, segment_ids, len(sequence)
+        return (sequence, sequence_mask, segment_ids, token_length) if return_sequence_length else (
+            sequence, sequence_mask, segment_ids)
 
-    def pair_to_ids(self, sequence_a: str, sequence_b: str, truncation_method: str = 'average') -> \
-            Tuple[np.ndarray, np.ndarray, np.ndarray, Tuple[int, int]]:
+    def pair_to_ids(self,
+                    sequence_a: str,
+                    sequence_b: str,
+                    truncation_method: str = 'average',
+                    return_sequence_length: bool = False
+                    ) -> Tuple[np.ndarray, np.ndarray, np.ndarray, Tuple[int, int]]:
         if type(sequence_a) == str:
             sequence_a = self.tokenize(sequence_a)
 
         if type(sequence_b) == str:
             sequence_b = self.tokenize(sequence_b)
 
         sequence_length = (len(sequence_a), len(sequence_b))
@@ -165,34 +171,43 @@
         # 对seq拼接填充序列
         sequence += padding
 
         sequence = np.asarray(sequence, dtype='int64')
         sequence_mask = np.asarray(sequence_mask, dtype='int64')
         segment_ids = np.asarray(segment_ids, dtype='int64')
 
-        return sequence, sequence_mask, segment_ids, sequence_length
+        return (sequence, sequence_mask, segment_ids, sequence_length) if return_sequence_length else (
+            sequence, sequence_mask, segment_ids)
 
 
 class SentenceTokenizer(TransfomerTokenizer):
     """
     单句分词器
     Args:
         vocab: transformers词典类对象、词典地址或词典名，用于实现文本分词和ID化
         max_seq_len (:obj:`int`): 预设的文本最大长度
     """  # noqa: ignore flake8"
 
+    def sequence_to_ids(self, sequence_a: Union[str, List[str]], sequence_b: Union[str, List[str]] = None,
+                        **kwargs) -> Tuple:
+        return self.sentence_to_ids(sequence_a, **kwargs)
+
 
 class PairTokenizer(TransfomerTokenizer):
     """
     句子对分词器
     Args:
         vocab: transformers词典类对象、词典地址或词典名，用于实现文本分词和ID化
         max_seq_len (:obj:`int`): 预设的文本最大长度
     """  # noqa: ignore flake8"
 
+    def sequence_to_ids(self, sequence_a: Union[str, List[str]], sequence_b: Union[str, List[str]] = None,
+                        **kwargs) -> Tuple:
+        return self.pair_to_ids(sequence_a, sequence_b, **kwargs)
+
 
 class TokenTokenizer(TransfomerTokenizer):
     """
     字符分词器，不
     Args:
         vocab: transformers词典类对象、词典地址或词典名，用于实现文本分词和ID化
         max_seq_len (:obj:`int`): 预设的文本最大长度
@@ -305,18 +320,17 @@
 
     Args:
         vocab: transformers词典类对象、词典地址或词典名，用于实现文本分词和ID化
         max_seq_len (int): 预设的文本最大长度
         cls_num (int): CLS类特殊字符的数量，例如"[CLS0]"、"[CLS1]", 默认值为2
     """  # noqa: ignore flake8"
 
-    def __init__(self, vocab: Union[BertTokenizer, AutoTokenizer, BaseVocab], max_seq_len: int, max_seq_length: int,
-                 cls_num: int = 2):
+    def __init__(self, vocab: Union[BertTokenizer, AutoTokenizer, BaseVocab], max_seq_len: int, cls_num: int = 2):
 
-        super().__init__(vocab, max_seq_len, max_seq_length)
+        super().__init__(vocab, max_seq_len, max_seq_len)
         self.additional_special_tokens = set()
 
         self.cls_num = cls_num
         self.cls_list = ['[CLS{}]'.format(index) for index in range(self.cls_num)]
 
         self.do_lower_case = self.vocab.do_lower_case
         self.vocab._tokenize = self._tokenize
```

### Comparing `weathon-0.0.0.8/weathon/nlp/processor/tokenizer/vanilla.py` & `weathon-0.0.0.9/weathon/nlp/processor/tokenizer/vanilla.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/processor/vocab/char_vocab.py` & `weathon-0.0.0.9/weathon/nlp/processor/vocab/char_vocab.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/processor/vocab/label_vocab.py` & `weathon-0.0.0.9/weathon/nlp/processor/vocab/label_vocab.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/processor/vocab/word_vocab.py` & `weathon-0.0.0.9/weathon/nlp/processor/vocab/word_vocab.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/task/__init__.py` & `weathon-0.0.0.9/weathon/nlp/task/__init__.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/task/named_entity_recognition.py` & `weathon-0.0.0.9/weathon/nlp/task/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/task/prompt_masked_language_model.py` & `weathon-0.0.0.9/weathon/nlp/task/prompt_masked_language_model.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/task/sequence_classification.py` & `weathon-0.0.0.9/weathon/nlp/task/sequence_classification.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import time
 import torch
 import warnings
 
 from tqdm import tqdm
 from torch.utils.data import DataLoader
 from weathon.nlp.base import BaseTask
-from weathon.utils import OptimizerUtils
+from weathon.utils import ScheduleUtils
 
 
 class SequenceClassificationTask(BaseTask):
     """
     序列分类任务的基类
 
     Args:
@@ -37,49 +37,37 @@
         if hasattr(self.module, 'task') is False:
             self.module.task = 'SequenceLevel'
 
     def fit(
             self,
             train_data,
             validation_data=None,
-            lr=False,
-            params=None,
             batch_size=32,
             epochs=1,
             gradient_accumulation_steps=1,
             **kwargs
     ):
         """
         训练方法
 
         Args:
             train_data (:obj:`ark_nlp dataset`): 训练的batch文本
             validation_data (:obj:`ark_nlp dataset`): 验证的batch文本
-            lr (:obj:`float` or :obj:`bool`, optional, defaults to False): 学习率
-            params (:obj:`str` or :obj:`torch.optim.Optimizer` or :obj:`list` or :obj:`None`, optional, defaults to None): 优化器，可能是名称、对象、参数列表
             batch_size (:obj:`int`, optional, defaults to 32): batch大小
             epochs (:obj:`int`, optional, defaults to 1): 训练轮数
             gradient_accumulation_steps (:obj:`int`, optional, defaults to 1): 梯度累计数
             **kwargs (optional): 其他可选参数
         """  # noqa: ignore flake8"
 
         self.logs = dict()
 
-        train_generator = self._on_train_begin(
-            train_data,
-            validation_data,
-            batch_size,
-            lr,
-            params,
-            shuffle=True,
-            **kwargs
-        )
+        train_generator = self._on_train_begin(train_data, validation_data, batch_size, shuffle=True, **kwargs)
 
         for epoch in range(epochs):
-
+            # module.train(), 重置 epoch_loss,epoch_evaluation, epoch_step
             self._on_epoch_begin(**kwargs)
 
             for step, inputs in enumerate(tqdm(train_generator)):
 
                 self._on_step_begin(epoch, step, inputs, **kwargs)
 
                 # input处理和设备转移
@@ -95,87 +83,66 @@
                 loss = self._on_backward(inputs, outputs, logits, loss, **kwargs)
 
                 if (step + 1) % gradient_accumulation_steps == 0:
                     # optimize
                     self._on_optimize(inputs, outputs, logits, loss, **kwargs)
 
                 # setp evaluate
-                self._on_step_end(step, inputs, outputs, logits, loss, **kwargs)
+                self._on_step_end(step, inputs, outputs, loss, **kwargs)
 
             self._on_epoch_end(epoch, **kwargs)
 
             if validation_data is not None:
                 self.evaluate(validation_data, **kwargs)
 
         self._on_train_end(**kwargs)
 
     def _on_train_begin(
             self,
             train_data,
             validation_data,
             batch_size,
-            lr,
-            params,
+            epochs,
             shuffle,
+            warmup_proportion=None,
             num_workers=0,
             train_to_device_cols=None,
             **kwargs
     ):
         if hasattr(train_data, 'id2cat'):
             self.id2cat = train_data.id2cat
-            self.cat2id = {v_: k_ for k_, v_ in train_data.id2cat.items()}
+            self.cat2id = train_data.cat2id
 
         # 在初始化时会有class_num参数，若在初始化时不指定，则在训练阶段从训练集获取信息
         if self.class_num is None:
             if hasattr(train_data, 'class_num'):
                 self.class_num = train_data.class_num
             else:
                 warnings.warn("The class_num is None.")
 
-        if train_to_device_cols is None:
-            self.train_to_device_cols = train_data.to_device_cols
-        else:
-            self.train_to_device_cols = train_to_device_cols
-
-        train_generator = DataLoader(
-            train_data,
-            batch_size=batch_size,
-            shuffle=True,
-            num_workers=num_workers,
-            collate_fn=self._train_collate_fn
-        )
+        self.train_to_device_cols = train_to_device_cols if train_to_device_cols else train_data.to_device_cols
+        train_generator = DataLoader(train_data, batch_size=batch_size, shuffle=shuffle, num_workers=num_workers,
+                                     collate_fn=self._train_collate_fn)
         self.train_generator_lenth = len(train_generator)
 
-        self.optimizer = OptimizerUtils.get_optimizer(self.optimizer, self.module, lr, params)
+        self.scheduler = self._prepare_scheduler(warmup_proportion, epochs) if warmup_proportion else None
+
         self.optimizer.zero_grad()
 
         self.module.train()
 
+        # 初始化 global_step 和 global_loss
         self._on_train_begin_record(**kwargs)
 
         return train_generator
 
-    def _on_train_begin_record(self, **kwargs):
-
-        self.logs['global_step'] = 0
-        self.logs['global_loss'] = 0
-
     def _on_epoch_begin(self, **kwargs):
-
         self.module.train()
-
         self._on_epoch_begin_record(**kwargs)
 
-    def _on_epoch_begin_record(self, **kwargs):
-
-        self.logs['epoch_loss'] = 0
-        # 占位作用，子类仅使用单个指标进行评价，则直接使用该字段即可
-        self.logs['epoch_evaluation'] = 0
-        self.logs['epoch_step'] = 0
-
     def _on_step_begin(
             self,
             epoch,
             step,
             inputs,
             **kwargs
     ):
@@ -228,25 +195,28 @@
 
     def _on_backward(
             self,
             inputs,
             outputs,
             logits,
             loss,
-            gradient_accumulation_steps=1,
+            gradient_accumulation_steps: int = 1,
+            loss_cut: float = None,
             **kwargs
     ):
 
         # 如果GPU数量大于1
         if self.n_gpu > 1:
             loss = loss.mean()
         # 如果使用了梯度累积，除以累积的轮数
         if gradient_accumulation_steps > 1:
             loss = loss / gradient_accumulation_steps
 
+        if loss_cut:
+            loss = torch.where(loss > float(loss_cut), loss, torch.zeros_like(loss))
         loss.backward()
 
         self._on_backward_record(loss, **kwargs)
 
         return loss
 
     def _on_backward_record(self, loss, **kwargs):
```

### Comparing `weathon-0.0.0.8/weathon/nlp/task/text_classification.py` & `weathon-0.0.0.9/weathon/nlp/task/text_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
                 self.logs['epoch_evaluation'] += torch.sum(preds == inputs['label_ids']).item() / len(inputs['label_ids'])
 
     def _on_step_end(
         self,
         step,
         inputs,
         outputs,
-        logits,
         loss,
         verbose=True,
         show_step=100,
         **kwargs
     ):
 
         if verbose and (step + 1) % show_step == 0:
```

### Comparing `weathon-0.0.0.8/weathon/nlp/task/text_level_gcn_classification.py` & `weathon-0.0.0.9/weathon/nlp/task/text_level_gcn_classification.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/task/text_match.py` & `weathon-0.0.0.9/weathon/nlp/task/text_match.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/nlp/task/token_classification.py` & `weathon-0.0.0.9/weathon/nlp/task/token_classification.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/__init__.py` & `weathon-0.0.0.9/weathon/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from weathon.utils.dictionary import Dictionary  # 词库
 
 # --------------------------------------------- deep learning ---------------------------------------------
 # transformers 下载、权重转换相关
 from weathon.utils.transformer_utils import TransformerUtils
 
 # 模型训练相关
-from weathon.utils.seed_utils import Seed  # 设置随机种子
+from weathon.utils.environment_utils import EnvironmentUtils  # 训练环境设置
 from weathon.utils.sampler import ImbalancedDatasetSampler  # 模型采样
 from weathon.utils.optimizer_utils import OptimizerUtils  # 优化器
 from weathon.utils.schedule_utils import ScheduleUtils  # 优化器 scheduler
 from weathon.utils.loss_utils import LossUtils  # 损失函数
 from weathon.utils.attack import FGM, PGD  # 模型训练trick
 from weathon.utils.ema import EMA  # 模型训练trick
```

### Comparing `weathon-0.0.0.8/weathon/utils/aho_corasick.py` & `weathon-0.0.0.9/weathon/utils/aho_corasick.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/attack.py` & `weathon-0.0.0.9/weathon/utils/attack.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/char_utils.py` & `weathon-0.0.0.9/weathon/utils/char_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/conlleval.py` & `weathon-0.0.0.9/weathon/utils/conlleval.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/constants.py` & `weathon-0.0.0.9/weathon/utils/constants.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/dictionary.py` & `weathon-0.0.0.9/weathon/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/ema.py` & `weathon-0.0.0.9/weathon/utils/ema.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/encrypt_utils.py` & `weathon-0.0.0.9/weathon/utils/encrypt_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/file_utils.py` & `weathon-0.0.0.9/weathon/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/find_word.py` & `weathon-0.0.0.9/weathon/utils/find_word.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/gpu_utils.py` & `weathon-0.0.0.9/weathon/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/ip_utils.py` & `weathon-0.0.0.9/weathon/utils/ip_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/json_utils.py` & `weathon-0.0.0.9/weathon/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/label_studio_utils.py` & `weathon-0.0.0.9/weathon/utils/label_studio_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/loss_utils.py` & `weathon-0.0.0.9/weathon/utils/loss_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/minjoin.py` & `weathon-0.0.0.9/weathon/utils/minjoin.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/model_ensemble.py` & `weathon-0.0.0.9/weathon/utils/model_ensemble.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/ner_utils.py` & `weathon-0.0.0.9/weathon/utils/ner_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/optimizer_utils.py` & `weathon-0.0.0.9/weathon/utils/optimizer_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 # @Time    : 2022/10/3 19:54
 # @Author  : LiZhen
 # @FileName: optimizer_utils.py
 # @github  : https://github.com/Lizhen0628
 # @Description:
 from torch.optim import Optimizer
-from weathon.nlp.factory.optimizer import all_optimizers_dict
+from weathon.nlp.factory.optimizer import all_optimizers_dict, AdamW
 
 
 class OptimizerUtils:
 
     @staticmethod
     def get_optimizer(optimizer, module, lr=False, params=None):
         if params is None:
@@ -97,14 +97,50 @@
         optimizer = all_optimizers_dict['adamw'](optimizer_grouped_parameters,
                                                  eps=eps,
                                                  correct_bias=correct_bias)
 
         return optimizer
 
     @staticmethod
+    def get_transformer_parameters(model, lr: float = 3e-5, weight_decay: float = 1e-3):
+        no_decay = ["bias", "LayerNorm.weight"]
+        group_parameters = [
+            {"params": [p for n, p in model.bert.name_parameters() if not any(nd in n for nd in no_decay)],
+             "weight_decay": weight_decay, "lr": lr},
+            {"params": [p for n, p in model.bert.name_parameters() if any(nd in n for nd in no_decay)],
+             "weight_decay": 0.0, "lr": lr},
+        ]
+        return group_parameters
+
+    @staticmethod
+    def get_classifier_parameters(model, lr: float = 1e-3, weight_decay: float = 1e-3):
+        no_decay = ["bias", "LayerNorm.weight"]
+        group_parameters = [
+            {"params": [p for n, p in model.classifier.name_parameters() if not any(nd in n for nd in no_decay)],
+             "weight_decay": weight_decay, "lr": lr},
+            {"params": [p for n, p in model.classifier.name_parameters() if any(nd in n for nd in no_decay)],
+             "weight_decay": 0.0, "lr": lr},
+        ]
+        return group_parameters
+
+    @staticmethod
+    def get_tc_transformer_optimizer_adamw(
+            model,
+            transformer_lr: float = 3e-5,
+            classifier_lr: float = 1e-3,
+            weight_decay: float = 1e-3,
+            eps: float = 1e-6
+    ):
+        group_parameters = OptimizerUtils.get_transformer_parameters(model, transformer_lr, weight_decay) + \
+                           OptimizerUtils.get_classifier_parameters(model, classifier_lr, weight_decay)
+
+        optimizer = AdamW(group_parameters, eps=eps)
+        return optimizer
+
+    @staticmethod
     def get_w2ner_model_optimizer(
             dl_module,
             lr: float = 1e-3,
             bert_lr: float = 5e-6,
             weight_decay=0.0
     ):
         bert_params = set(dl_module.bert.parameters())
```

### Comparing `weathon-0.0.0.8/weathon/utils/sampler.py` & `weathon-0.0.0.9/weathon/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/schedule_utils.py` & `weathon-0.0.0.9/weathon/utils/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/states_machine.py` & `weathon-0.0.0.9/weathon/utils/states_machine.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/string_converter.py` & `weathon-0.0.0.9/weathon/utils/string_converter.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/string_similarity.py` & `weathon-0.0.0.9/weathon/utils/string_similarity.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/string_utils.py` & `weathon-0.0.0.9/weathon/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/text_cluster.py` & `weathon-0.0.0.9/weathon/utils/text_cluster.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/textrank.py` & `weathon-0.0.0.9/weathon/utils/textrank.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon/utils/transformer_utils.py` & `weathon-0.0.0.9/weathon/utils/transformer_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             tokenizer = AutoTokenizer.from_pretrained(model_name)
         except Exception as e:
             tokenizer = BertTokenizer.from_pretrained(model_name)
         tokenizer.save_pretrained(path)
 
         model = AutoModel.from_pretrained(model_name)
         model.save_pretrained(path)
-        print(path, 'done.')
+        print(os.path.abspath(path), 'done.')
 
     @staticmethod
     def load_tf_weights_in_nezha(model, config, tf_checkpoint_path):
         """Load tf checkpoints in a pytorch model."""
         try:
 
             import tensorflow as tf
```

### Comparing `weathon-0.0.0.8/weathon/utils/union_find.py` & `weathon-0.0.0.9/weathon/utils/union_find.py`

 * *Files identical despite different names*

### Comparing `weathon-0.0.0.8/weathon.egg-info/SOURCES.txt` & `weathon-0.0.0.9/weathon.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -159,28 +159,28 @@
 weathon/utils/attack.py
 weathon/utils/char_utils.py
 weathon/utils/conlleval.py
 weathon/utils/constants.py
 weathon/utils/dictionary.py
 weathon/utils/ema.py
 weathon/utils/encrypt_utils.py
+weathon/utils/environment_utils.py
 weathon/utils/file_utils.py
 weathon/utils/find_word.py
 weathon/utils/gpu_utils.py
 weathon/utils/ip_utils.py
 weathon/utils/json_utils.py
 weathon/utils/label_studio_utils.py
 weathon/utils/loss_utils.py
 weathon/utils/minjoin.py
 weathon/utils/model_ensemble.py
 weathon/utils/ner_utils.py
 weathon/utils/optimizer_utils.py
 weathon/utils/sampler.py
 weathon/utils/schedule_utils.py
-weathon/utils/seed_utils.py
 weathon/utils/states_machine.py
 weathon/utils/string_converter.py
 weathon/utils/string_similarity.py
 weathon/utils/string_utils.py
 weathon/utils/text_cluster.py
 weathon/utils/textrank.py
 weathon/utils/transformer_utils.py
```

