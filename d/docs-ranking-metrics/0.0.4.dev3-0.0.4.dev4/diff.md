# Comparing `tmp/docs-ranking-metrics-0.0.4.dev3.tar.gz` & `tmp/docs-ranking-metrics-0.0.4.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\docs-ranking-metrics-0.0.4.dev3.tar", last modified: Thu Jun  1 05:54:32 2023, max compression
+gzip compressed data, was "dist\docs-ranking-metrics-0.0.4.dev4.tar", last modified: Thu Jun  1 06:24:50 2023, max compression
```

## Comparing `docs-ranking-metrics-0.0.4.dev3.tar` & `docs-ranking-metrics-0.0.4.dev4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 05:54:32.784800 docs-ranking-metrics-0.0.4.dev3/
--rw-rw-rw-   0        0        0     3432 2023-06-01 05:54:32.783801 docs-ranking-metrics-0.0.4.dev3/PKG-INFO
--rw-rw-rw-   0        0        0     2694 2023-06-01 05:54:20.000000 docs-ranking-metrics-0.0.4.dev3/README.md
--rw-rw-rw-   0        0        0       97 2023-05-31 06:23:53.000000 docs-ranking-metrics-0.0.4.dev3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 05:54:32.784800 docs-ranking-metrics-0.0.4.dev3/setup.cfg
--rw-rw-rw-   0        0        0     8957 2023-05-31 06:23:53.000000 docs-ranking-metrics-0.0.4.dev3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 05:54:32.639148 docs-ranking-metrics-0.0.4.dev3/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 05:54:32.696510 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/
--rw-rw-rw-   0        0        0      195 2023-06-01 05:51:41.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/__init__.py
--rw-rw-rw-   0        0        0    17858 2023-06-01 04:47:09.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/evaluation_metrics.py
--rw-rw-rw-   0        0        0     1534 2023-06-01 04:57:10.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/models.py
--rw-rw-rw-   0        0        0    16333 2023-06-01 04:57:10.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/ranking_metrics.py
-drwxrwxrwx   0        0        0        0 2023-06-01 05:54:32.781799 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/
--rw-rw-rw-   0        0        0     3432 2023-06-01 05:54:32.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2023-06-01 05:54:32.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 05:54:32.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-06-01 05:54:32.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-01 05:54:32.000000 docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 06:24:50.230245 docs-ranking-metrics-0.0.4.dev4/
+-rw-rw-rw-   0        0        0     3432 2023-06-01 06:24:50.226246 docs-ranking-metrics-0.0.4.dev4/PKG-INFO
+-rw-rw-rw-   0        0        0     2694 2023-06-01 05:54:20.000000 docs-ranking-metrics-0.0.4.dev4/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-31 06:23:53.000000 docs-ranking-metrics-0.0.4.dev4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 06:24:50.230245 docs-ranking-metrics-0.0.4.dev4/setup.cfg
+-rw-rw-rw-   0        0        0     8957 2023-05-31 06:23:53.000000 docs-ranking-metrics-0.0.4.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:24:50.167249 docs-ranking-metrics-0.0.4.dev4/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 06:24:50.180281 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics/
+-rw-rw-rw-   0        0        0      195 2023-06-01 06:21:21.000000 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics/__init__.py
+-rw-rw-rw-   0        0        0    17644 2023-06-01 06:14:35.000000 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     1534 2023-06-01 04:57:10.000000 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics/models.py
+-rw-rw-rw-   0        0        0    16335 2023-06-01 06:14:35.000000 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics/ranking_metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:24:50.224247 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics.egg-info/
+-rw-rw-rw-   0        0        0     3432 2023-06-01 06:24:50.000000 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      435 2023-06-01 06:24:50.000000 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 06:24:50.000000 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       92 2023-06-01 06:24:50.000000 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-01 06:24:50.000000 docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics.egg-info/top_level.txt
```

### Comparing `docs-ranking-metrics-0.0.4.dev3/PKG-INFO` & `docs-ranking-metrics-0.0.4.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.4.dev3
+Version: 0.0.4.dev4
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 License: UNKNOWN
 Keywords: test
 Platform: UNKNOWN
```

### Comparing `docs-ranking-metrics-0.0.4.dev3/README.md` & `docs-ranking-metrics-0.0.4.dev4/README.md`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.4.dev3/setup.py` & `docs-ranking-metrics-0.0.4.dev4/setup.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/evaluation_metrics.py` & `docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics/evaluation_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,22 +78,22 @@
     """
     Метрика оценивает как часто фейковый документ находится выше релевантного.
     Представлены две версии. Первая (FDARO@v1) оценивает как часто фейк документ
     находится выше ВСЕХ релевантных. Вторая (FDARO@v2) - как часто фейковый документ
     оказывается выше хотя бы одного.
     """
 
-    def __init__(self, ranking_metrics: List, relevant_doc_label: Union[int, List] = 1) -> None:
+    def __init__(self, ranking_metrics: List, relevant_doc_labelss: Union[int, List] = 1) -> None:
         self._separator = "_"
         self.metrics, self.calls_cnt = {}, {}
         self.versions = ["v1", "v2"]
-        if isinstance(relevant_doc_label, int):
-            self.relevant_doc_label = [relevant_doc_label]
+        if isinstance(relevant_doc_labelss, int):
+            self.relevant_doc_labelss = [relevant_doc_labelss]
         else:
-            self.relevant_doc_label = relevant_doc_label
+            self.relevant_doc_labelss = relevant_doc_labelss
 
         for cur_metric in ranking_metrics:
             for version in self.versions:
                 self.metrics[cur_metric.name() + self._separator + self.name() + version] = 0
                 self.calls_cnt[cur_metric.name() + self._separator + self.name() + version] = 0
 
     def update(self, metric_name: str,
@@ -106,25 +106,25 @@
         -------------
         metric_name: `str`
             Название метрики
         ranking_list: `List[Union[Tuple[float, int], List[float, int]]]`
             Результат ранжирующей модели
         fake_doc_label: `Union[int, List[int]]`
             Метка или массив меток, принадлежащих фейковым документам
-        relevant_doc_label: `Union[int, List[int]]`
+        relevant_doc_labelss: `Union[int, List[int]]`
             Метка или массив меток, принадлежащих релевантным документам
         """
         if isinstance(fake_doc_label, int):
             fake_doc_label = [fake_doc_label]
 
         _check_update_args(fake_doc_label, ranking_list)
 
         is_first = False
         for item in ranking_list:
-            if item[1] in self.relevant_doc_label:
+            if item[1] in self.relevant_doc_labelss:
                 break
             elif item[1] in fake_doc_label:
                 is_first = True
                 break
 
         if is_first:
             self.metrics[metric_name + self._separator + self.name() + self.versions[0]] += 1
@@ -136,15 +136,15 @@
             scores.append(item[0])
             selected.append(item[1])
 
         scores_relevant = -1e9
         scores_fake = -1e9
         for ind in range(len(selected)):
             # Выбираем последний релевантный элемент
-            if selected[ind] in self.relevant_doc_label:
+            if selected[ind] in self.relevant_doc_labelss:
                 scores_relevant = scores[ind]
             elif selected[ind] in fake_doc_label and scores_fake == -1e9:
                 scores_fake = scores[ind]
 
         upper_or_not = (scores_fake - scores_relevant) > 1e-12
         self.metrics[metric_name + self._separator + self.name() + self.versions[1]] += int(upper_or_not)
         self.calls_cnt[metric_name + self._separator + self.name() + self.versions[1]] += 1
@@ -357,15 +357,15 @@
         for item in ranking_list:
             scores.append(item[0])
             selected.append(item[1])
         selected = np.array(selected)
         scores = np.array(scores)
 
         upper_quartile = np.quantile(scores, 0.75)
-        # fake_idxs = np.where(selected == fake_doc_label[0])[0]
+
         scores_fake = -1e9
         for ind in range(len(selected)):
             if selected[ind] in fake_doc_label:
                 scores_fake = selected[ind]
                 break
 
         if scores_fake >= upper_quartile:
@@ -407,16 +407,14 @@
     '''
     Функция для валидации списка меток и списка для ранжирования
 
     Parameters
     -------------
     fake_doc_label: `Union[int, List[int]]`
         Метка или список меток, обозначающих фейковый документ
-    relevant_doc_label: `Union[int, List[int]]`
-        Метка или список меток, обозначающих релевантные документы
     ranking_list: `List[Union[Tuple[float, int], List[float, int]]]`
         Список оценок ранжировщика
     '''
     if not isinstance(fake_doc_label, list):
         raise TypeError("The tags of fake documents must be 'int' or 'list!'")
     else:
         for label in fake_doc_label:
```

### Comparing `docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/models.py` & `docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics/models.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics/ranking_metrics.py` & `docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics/ranking_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,29 +300,29 @@
         """
         return sorted([item for item in zip(scores, labels)], key=lambda x: x[0], reverse=True)
 
 class RankingMetrics:
     """Класс аккумулирующий все метрики"""
     FAKE_DOC_LABEL: int = -1
 
-    def __init__(self, metrics, relevant_doc_label: Union[int, List] = 1) -> None:
+    def __init__(self, metrics, relevant_doc_labels: Union[int, List] = 1) -> None:
         """
 
         Parameters
         ------------
         metrics: `Union[LaBSE, USE, Bm25, MsMarcoCE, MsMarcoST]`
             Классы метрик ранжирования
 
         relevant_doc_label: `Union[int, List]`
             Метка или массив меток, обозначающих релевантные документы. (Используется для оценки FDARO)
         """
         # Среднее место фейковых документов в финальной выдаче
         self.average_place_fake_doc = AverageLoc(metrics)
         # Количество случаев когда фейковый документ выше релевантного
-        self.fake_doc_above_relevant_one = FDARO(metrics, relevant_doc_label)
+        self.fake_doc_above_relevant_one = FDARO(metrics, relevant_doc_labels)
         # Количество случаев когда фейковый документ вошел в топ 1
         self.fake_top_k = TopK(metrics)
         self.upper_quartile = UpQuartile(metrics)
         # Среднее относительное место фейковых документов в выдаче
         self.average_rel_place_fake_doc = AverageRelLoc(metrics)
         # Массив метрик для подсчета
         self.metrics = metrics
```

### Comparing `docs-ranking-metrics-0.0.4.dev3/src/docs_ranking_metrics.egg-info/PKG-INFO` & `docs-ranking-metrics-0.0.4.dev4/src/docs_ranking_metrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.4.dev3
+Version: 0.0.4.dev4
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 License: UNKNOWN
 Keywords: test
 Platform: UNKNOWN
```

