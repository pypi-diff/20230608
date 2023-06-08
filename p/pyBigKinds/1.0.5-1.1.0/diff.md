# Comparing `tmp/pyBigKinds-1.0.5-py3-none-any.whl.zip` & `tmp/pyBigKinds-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7143 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      753 b- defN 23-Jun-03 07:43 pyBigKinds/__init__.py
--rw-rw-rw-  2.0 fat       22 b- defN 23-Jun-06 07:37 pyBigKinds/_version.py
--rw-rw-rw-  2.0 fat     2475 b- defN 23-Jun-06 07:38 pyBigKinds/base.py
--rw-rw-rw-  2.0 fat     4744 b- defN 23-Jun-06 07:38 pyBigKinds/preprocessing.py
--rw-rw-rw-  2.0 fat      720 b- defN 23-Jun-06 07:38 pyBigKinds/representation.py
--rw-rw-rw-  2.0 fat     2374 b- defN 23-Jun-06 07:38 pyBigKinds/visualization.py
--rw-rw-rw-  2.0 fat     1070 b- defN 23-Jun-06 07:44 pyBigKinds-1.0.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1600 b- defN 23-Jun-06 07:44 pyBigKinds-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-06 07:44 pyBigKinds-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-06 07:44 pyBigKinds-1.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      883 b- defN 23-Jun-06 07:44 pyBigKinds-1.0.5.dist-info/RECORD
-11 files, 14744 bytes uncompressed, 5649 bytes compressed:  61.7%
+Zip file size: 7585 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      783 b- defN 23-Jun-08 16:52 pyBigKinds/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-08 16:52 pyBigKinds/_version.py
+-rw-r--r--  2.0 unx     2475 b- defN 23-Jun-08 16:52 pyBigKinds/base.py
+-rw-r--r--  2.0 unx     2552 b- defN 23-Jun-08 16:52 pyBigKinds/preprocessing.py
+-rw-r--r--  2.0 unx     4080 b- defN 23-Jun-08 16:52 pyBigKinds/representation.py
+-rw-r--r--  2.0 unx     2374 b- defN 23-Jun-08 16:52 pyBigKinds/visualization.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Jun-08 16:53 pyBigKinds-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1601 b- defN 23-Jun-08 16:53 pyBigKinds-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 16:53 pyBigKinds-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-08 16:53 pyBigKinds-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      884 b- defN 23-Jun-08 16:53 pyBigKinds-1.1.0.dist-info/RECORD
+11 files, 15944 bytes uncompressed, 6091 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: pyBigKinds/representation.py
 Comment: 
 
 Filename: pyBigKinds/visualization.py
 Comment: 
 
-Filename: pyBigKinds-1.0.5.dist-info/LICENSE
+Filename: pyBigKinds-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: pyBigKinds-1.0.5.dist-info/METADATA
+Filename: pyBigKinds-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pyBigKinds-1.0.5.dist-info/WHEEL
+Filename: pyBigKinds-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pyBigKinds-1.0.5.dist-info/top_level.txt
+Filename: pyBigKinds-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pyBigKinds-1.0.5.dist-info/RECORD
+Filename: pyBigKinds-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyBigKinds/__init__.py

```diff
@@ -28,8 +28,10 @@
     "normalize_vector",
     "pca",
     "nmf",
     "t_sne",
     "lsa",
     "kmeans",
     "dbscan",
+    "lda",
+    "association",
 ]
```

## pyBigKinds/_version.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.5"
+__version__ = "1.1.0"
```

## pyBigKinds/preprocessing.py

```diff
@@ -1,43 +1,22 @@
 import numpy as np
 import pandas as pd
-from sklearn.decomposition import NMF, PCA, TruncatedSVD
 from sklearn.feature_extraction.text import CountVectorizer, TfidfTransformer, TfidfVectorizer
-from sklearn.manifold import TSNE
 from sklearn.pipeline import Pipeline
 from sklearn.preprocessing import Normalizer
 
 from .base import (
     counter_to_dataframe,
     duplication_remover,
     keyword_list,
     keyword_parser,
     word_counter,
 )
 
 
-def day_range(df):
-    """날짜 범위 파악"""
-    if isinstance(df, pd.DataFrame):
-        print("first day: ", df["일자"].min(), "\n", "last day: ", df["일자"].max())
-    else:
-        raise TypeError("input type is to be have to DataFrame")
-
-
-def press_counter(df):
-    """언론사 별 보도 빈도"""
-    if isinstance(df, pd.DataFrame):
-        freq = df["언론사"].value_counts()
-        brod_df = pd.DataFrame(freq).reset_index()
-        brod_df.rename(columns={"index": "언론사", "언론사": "기사"}, inplace=True)
-        return brod_df
-    else:
-        raise TypeError("input type is to be have to DataFrame")
-
-
 def keyword_dataframe(df):
     """키워드 단어 빈도"""
     if isinstance(df, pd.DataFrame):
         lis = keyword_list(df)
         keywords = keyword_parser(lis)
         counter = word_counter(keywords)
         df = counter_to_dataframe(counter)
@@ -103,55 +82,7 @@
 def normalize_vector(vec):
     """normalize vector"""
     if isinstance(vec, np.ndarray):
         vec_nor = Normalizer().fit_transform(vec)
         return vec_nor
     else:
         raise TypeError("input type is to be have to ndarray")
-
-
-def pca(vec, Random_State=123):
-    """PCA"""
-    if isinstance(vec, np.ndarray):
-        pca_df = PCA(n_components=2, random_state=Random_State, copy=False).fit_transform(
-            vec,
-        )
-        pca_df = pd.DataFrame(pca_df, columns=["component 0", "component 1"])
-
-        return pca_df
-    else:
-        raise TypeError("input type is to be have to ndarray")
-
-
-def nmf(vec, Random_State=123):
-    """NMF"""
-    if isinstance(vec, np.ndarray):
-        nmf_df = NMF(
-            n_components=2, random_state=Random_State, init="random",
-        ).fit_transform(vec)
-        nmf_df = pd.DataFrame(nmf_df, columns=["component 0", "component 1"])
-
-        return nmf_df
-    else:
-        raise TypeError("input type is to be have to ndarray")
-
-
-def t_sne(vec, learn_Rate=100):
-    """t-sne"""
-    if isinstance(vec, np.ndarray):
-        tsne = TSNE(n_components=2, learning_rate=learn_Rate).fit_transform(vec)
-        tsne_df = pd.DataFrame(tsne, columns=["component 0", "component 1"])
-    else:
-        raise TypeError("input type is to be have to ndarray")
-
-    return tsne_df
-
-
-def lsa(vec):
-    """LSA"""
-    if isinstance(vec, np.ndarray):
-        svd = TruncatedSVD(n_components=2).fit_transform(vec)
-        svd_df = pd.DataFrame(data=svd, columns=["component 0", "component 1"])
-    else:
-        raise TypeError("input type is to be have to ndarray")
-
-    return svd_df
```

## pyBigKinds/representation.py

```diff
@@ -1,11 +1,86 @@
-# pylint: disable=E0601,W0612
+# pylint: disable=E1101
 
 import numpy as np
+import pandas as pd
+import tomotopy as tp
+from mlxtend.frequent_patterns import apriori, association_rules
+from mlxtend.preprocessing import TransactionEncoder
 from sklearn.cluster import DBSCAN, KMeans
+from sklearn.decomposition import NMF, PCA, TruncatedSVD
+from sklearn.manifold import TSNE
+
+from .base import keyword_list, keyword_parser
+
+
+def day_range(df):
+    """날짜 범위 파악"""
+    if isinstance(df, pd.DataFrame):
+        print("first day: ", df["일자"].min(), "\n", "last day: ", df["일자"].max())
+    else:
+        raise TypeError("input type is to be have to DataFrame")
+
+
+def press_counter(df):
+    """언론사 별 보도 빈도"""
+    if isinstance(df, pd.DataFrame):
+        freq = df["언론사"].value_counts()
+        brod_df = pd.DataFrame(freq).reset_index()
+        brod_df.rename(columns={"index": "언론사", "언론사": "기사"}, inplace=True)
+        return brod_df
+    else:
+        raise TypeError("input type is to be have to DataFrame")
+
+
+def pca(vec, Random_State=123):
+    """PCA"""
+    if isinstance(vec, np.ndarray):
+        pca_df = PCA(n_components=2, random_state=Random_State, copy=False).fit_transform(
+            vec,
+        )
+        pca_df = pd.DataFrame(pca_df, columns=["component 0", "component 1"])
+
+        return pca_df
+    else:
+        raise TypeError("input type is to be have to ndarray")
+
+
+def nmf(vec, Random_State=123):
+    """NMF"""
+    if isinstance(vec, np.ndarray):
+        nmf_df = NMF(
+            n_components=2, random_state=Random_State, init="random",
+        ).fit_transform(vec)
+        nmf_df = pd.DataFrame(nmf_df, columns=["component 0", "component 1"])
+
+        return nmf_df
+    else:
+        raise TypeError("input type is to be have to ndarray")
+
+
+def t_sne(vec, learn_Rate=100):
+    """t-sne"""
+    if isinstance(vec, np.ndarray):
+        tsne = TSNE(n_components=2, learning_rate=learn_Rate).fit_transform(vec)
+        tsne_df = pd.DataFrame(tsne, columns=["component 0", "component 1"])
+    else:
+        raise TypeError("input type is to be have to ndarray")
+
+    return tsne_df
+
+
+def lsa(vec):
+    """LSA"""
+    if isinstance(vec, np.ndarray):
+        svd = TruncatedSVD(n_components=2).fit_transform(vec)
+        svd_df = pd.DataFrame(data=svd, columns=["component 0", "component 1"])
+    else:
+        raise TypeError("input type is to be have to ndarray")
+
+    return svd_df
 
 
 def kmeans(vec, k, random_state=123):
     """K-Means"""
     if isinstance(vec, np.ndarray):
         kmeans_model = KMeans(n_clusters=k, max_iter=1000, random_state=random_state)
         return kmeans_model.fit_predict(vec)
@@ -16,7 +91,36 @@
 def dbscan(vec, eps, min_samples, metric="euclidean"):
     """DBSCAN"""
     if isinstance(vec, np.ndarray):
         dbscan_model = DBSCAN(eps=eps, min_samples=min_samples, metric=metric)
         return dbscan_model.fit_predict(vec)
     else:
         raise TypeError("input type is to be have to ndarray")
+
+
+def lda(dataframe, k=10, train=100, fit=10):
+    """topic modeling"""
+    if isinstance(dataframe, pd.DataFrame):
+        lis = keyword_parser(keyword_list(dataframe))
+        model = tp.LDAModel(k=k)
+
+        for words in lis:
+            model.add_doc(words)
+
+        for i in range(0, train, fit):
+            model.train(i)
+
+        return model
+    else:
+        raise TypeError("input type is to be have to DataFrame")
+
+
+def association(dataframe, min_support=0.5, use_colnames=True, min_threshold=0.1, metric="confidence"):
+    """apriopri"""
+    words = keyword_parser(keyword_list(dataframe))
+    te = TransactionEncoder()
+    te_data = te.fit(words).transform(words, sparse=True)
+    te_df = pd.DataFrame.sparse.from_spmatrix(te_data, columns=te.columns_)
+
+    result = apriori(te_df, min_support=min_support, use_colnames=use_colnames)
+
+    return association_rules(result, metric=metric, min_threshold=min_threshold)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `pyBigKinds-1.0.5.dist-info/LICENSE` & `pyBigKinds-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyBigKinds-1.0.5.dist-info/METADATA` & `pyBigKinds-1.1.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,70 @@
-Metadata-Version: 2.1
-Name: pyBigKinds
-Version: 1.0.5
-Summary: BigKinds Data Analysis Toolkit for python
-Home-page: https://github.com/sorrychoe/pyBigKinds
-Author: Sorrychoe
-License: MIT
-Project-URL: Source Code, https://github.com/sorrychoe/pyBigKinds
-Project-URL: Bug Tracker, https://github.com/sorrychoe/pyBigKinds/issues
-Keywords: Journalism,preprocessing-data,BigKinds
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: matplotlib (>=3.5.3)
-Requires-Dist: pandas (<2)
-Requires-Dist: wordcloud (>=1.8.2.2)
-Requires-Dist: scikit-learn (>=1.0.0)
-Requires-Dist: openpyxl (>=3.1.2)
-Provides-Extra: dev
-Requires-Dist: flake8 (>=3.9) ; extra == 'dev'
-Requires-Dist: isort (>=5.7) ; extra == 'dev'
-Requires-Dist: pre-commit (>=2.13) ; extra == 'dev'
-Requires-Dist: pylint (>=2.9) ; extra == 'dev'
-Requires-Dist: pytest (>=7) ; extra == 'dev'
-
-# pyBigKinds
-
-pyBigKinds는 한국 언론의 빅데이터 저장소인 BigKinds에서 추출한 데이터를 low-Code로 분석할 수 있게 만든 툴입니다.
-
-## Requirements
-
-- Python >= 3.8
-
-## Installation
-
-- macOS
-
-  ```bash
-  python3 -m pip install pyBigKinds
-  ```
-
-- Windows, linux
-
-  ```bash
-  python -m pip install pyBigKinds
-  ```
-
-## Example
-
-```python
-import pyBigKinds as bk
-
-bk.press_counter(df)
-
-```
-
-## Authors
-
-- [sorrychoe](https://www.github.com/sorrychoe)
-
-
-## License
-
-- [MIT](https://choosealicense.com/licenses/mit/)
-
-## you have some issue?
-
-사용 중 문제 발생 시, 해당 Repo issue에 등록해주세요.
+Metadata-Version: 2.1
+Name: pyBigKinds
+Version: 1.1.0
+Summary: BigKinds Data Analysis Toolkit for python
+Home-page: https://github.com/sorrychoe/pyBigKinds
+Author: Sorrychoe
+License: MIT
+Project-URL: Source Code, https://github.com/sorrychoe/pyBigKinds
+Project-URL: Bug Tracker, https://github.com/sorrychoe/pyBigKinds/issues
+Keywords: Journalism,preprocessing-data,BigKinds
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib (>=3.5.3)
+Requires-Dist: pandas (<2)
+Requires-Dist: wordcloud (>=1.8.2.2)
+Requires-Dist: scikit-learn (>=1.0.0)
+Requires-Dist: tomotopy (>=0.12.4)
+Requires-Dist: openpyxl (>=3.1.2)
+Requires-Dist: mlxtend (>=0.22.0)
+Provides-Extra: dev
+Requires-Dist: flake8 (>=3.9) ; extra == 'dev'
+Requires-Dist: isort (>=5.7) ; extra == 'dev'
+Requires-Dist: pre-commit (>=2.13) ; extra == 'dev'
+Requires-Dist: pylint (>=2.9) ; extra == 'dev'
+Requires-Dist: pytest (>=7) ; extra == 'dev'
+
+# pyBigKinds
+
+pyBigKinds는 한국 언론의 빅데이터 저장소인 BigKinds에서 추출한 데이터를 low-Code로 분석할 수 있게 만든 툴입니다.
+
+## Requirements
+
+- Python >= 3.8
+
+## Installation
+
+- macOS
+
+  ```bash
+  python3 -m pip install pyBigKinds
+  ```
+
+- Windows, linux
+
+  ```bash
+  python -m pip install pyBigKinds
+  ```
+
+## Example
+
+```python
+import pyBigKinds as bk
+
+bk.press_counter(df)
+
+```
+
+## Authors
+
+- [sorrychoe](https://www.github.com/sorrychoe)
+
+
+## License
+
+- [MIT](https://choosealicense.com/licenses/mit/)
+
+## you have some issue?
+
+사용 중 문제 발생 시, 해당 Repo issue에 등록해주세요.
```

## Comparing `pyBigKinds-1.0.5.dist-info/RECORD` & `pyBigKinds-1.1.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-pyBigKinds/__init__.py,sha256=SQtv2XrCav_1DGhOqDMrpzQ6QmR0ryFbuyEkNcCiroM,753
-pyBigKinds/_version.py,sha256=B9kKWJLln1i8LjtkcYecvNWGLTrez4gCUOHtnPlInFo,22
+pyBigKinds/__init__.py,sha256=3Trd45Kpi8CK1BvxsOR1d2Kf9v_wN3qdZLuVADyUwU4,783
+pyBigKinds/_version.py,sha256=LGVQyDsWifdACo7qztwb8RWWHds1E7uQ-ZqD8SAjyw4,22
 pyBigKinds/base.py,sha256=KrKO3O1wpXvWr8TVq-3hl2JwwWu4l3lLBtpuXUyv1mg,2475
-pyBigKinds/preprocessing.py,sha256=nuwrP1PoxxnjcWj7OMwOqfOYv7dYJ7Pju9FkV6rr3f8,4744
-pyBigKinds/representation.py,sha256=g5x9NLvPR9IUHrhlqAfNT06V5gCVqLQKyJ2G1bRogRM,720
+pyBigKinds/preprocessing.py,sha256=4blorjI5OFdg99mgioKLnybbD_xlyjLctCIAx1Ut15U,2552
+pyBigKinds/representation.py,sha256=uFqybooPWrrHvKTy6rcjrKbuvb3ay3_pTv9ajZvdH1g,4080
 pyBigKinds/visualization.py,sha256=5HuguRxYlzLms6xDAp8SMwAl_-upCESrtz6_aDh5KIY,2374
-pyBigKinds-1.0.5.dist-info/LICENSE,sha256=4qpntoObC47xSDR5kl1lMvxC4Hz6PuFVKIthT3E3j8Y,1070
-pyBigKinds-1.0.5.dist-info/METADATA,sha256=l8Yx1WArGz-57utSy-eIFRPmdEx_-pMCJfkX7bXah6k,1600
-pyBigKinds-1.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pyBigKinds-1.0.5.dist-info/top_level.txt,sha256=LDFcWpfU5Sf0n08ITRMJP20n-2u9ckNkEErPtU8iYbg,11
-pyBigKinds-1.0.5.dist-info/RECORD,,
+pyBigKinds-1.1.0.dist-info/LICENSE,sha256=4qpntoObC47xSDR5kl1lMvxC4Hz6PuFVKIthT3E3j8Y,1070
+pyBigKinds-1.1.0.dist-info/METADATA,sha256=JCBoJmF4CL1djPKWF-yh26x54UQrwwFSK_sy7Jxf18U,1601
+pyBigKinds-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pyBigKinds-1.1.0.dist-info/top_level.txt,sha256=LDFcWpfU5Sf0n08ITRMJP20n-2u9ckNkEErPtU8iYbg,11
+pyBigKinds-1.1.0.dist-info/RECORD,,
```

