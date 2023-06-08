# Comparing `tmp/aisp-0.1.0.tar.gz` & `tmp/aisp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aisp-0.1.0.tar", last modified: Mon May 22 13:47:29 2023, max compression
+gzip compressed data, was "aisp-0.1.1.tar", last modified: Thu Jun  8 16:10:38 2023, max compression
```

## Comparing `aisp-0.1.0.tar` & `aisp-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 13:47:29.606376 aisp-0.1.0/
--rw-rw-rw-   0        0        0     7817 2023-05-19 21:21:29.000000 aisp-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     8016 2023-05-22 13:47:29.605383 aisp-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     6852 2023-05-20 21:39:53.000000 aisp-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 13:47:29.586612 aisp-0.1.0/aisp/
-drwxrwxrwx   0        0        0        0 2023-05-22 13:47:29.602363 aisp-0.1.0/aisp/NSA/
--rw-rw-rw-   0        0        0      116 2023-03-29 21:36:25.000000 aisp-0.1.0/aisp/NSA/__init__.py
--rw-rw-rw-   0        0        0    48311 2023-05-05 00:43:00.000000 aisp-0.1.0/aisp/NSA/_negativeSelection.py
--rw-rw-rw-   0        0        0     6023 2023-04-26 02:06:12.000000 aisp-0.1.0/aisp/_base.py
-drwxrwxrwx   0        0        0        0 2023-05-22 13:47:29.598352 aisp-0.1.0/aisp.egg-info/
--rw-rw-rw-   0        0        0     8016 2023-05-22 13:47:29.000000 aisp-0.1.0/aisp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-05-22 13:47:29.000000 aisp-0.1.0/aisp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 13:47:29.000000 aisp-0.1.0/aisp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-05-22 13:47:29.000000 aisp-0.1.0/aisp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-22 13:47:29.000000 aisp-0.1.0/aisp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1349 2023-05-22 13:47:11.000000 aisp-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-22 13:47:29.607378 aisp-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.136405 aisp-0.1.1/
+-rw-rw-rw-   0        0        0     7817 2023-05-19 21:21:29.000000 aisp-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     8016 2023-06-08 16:10:38.133383 aisp-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6852 2023-06-08 15:06:17.000000 aisp-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.100382 aisp-0.1.1/aisp/
+drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.129382 aisp-0.1.1/aisp/NSA/
+-rw-rw-rw-   0        0        0      116 2023-05-28 13:47:18.000000 aisp-0.1.1/aisp/NSA/__init__.py
+-rw-rw-rw-   0        0        0    48346 2023-06-08 15:27:54.000000 aisp-0.1.1/aisp/NSA/_negativeSelection.py
+-rw-rw-rw-   0        0        0     8040 2023-06-08 15:52:49.000000 aisp-0.1.1/aisp/_base.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:10:38.119385 aisp-0.1.1/aisp.egg-info/
+-rw-rw-rw-   0        0        0     8016 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-08 16:10:38.000000 aisp-0.1.1/aisp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1349 2023-06-08 15:56:51.000000 aisp-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 16:10:38.137386 aisp-0.1.1/setup.cfg
```

### Comparing `aisp-0.1.0/LICENSE` & `aisp-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aisp-0.1.0/PKG-INFO` & `aisp-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package with techniques of artificial immune systems.
 Author-email: João Paulo da Silva Barros <jpsilvabarr@gmail.com>
 Maintainer-email: Alison Zille Lopes <alisonzille@gmail.com>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://ais-package.github.io/
 Project-URL: Documentation, https://ais-package.github.io/docs/intro
 Project-URL: Source Code, https://github.com/AIS-Package/aisp
@@ -95,15 +95,15 @@
 
 ##### **Dependencies:**
 <div align = center> 
 
 
 |    Packages   |     Version   |
 |:-------------:|:-------------:|
-|    numpy      |    ≥ 1.23.0   |
+|    numpy      |    ≥ 1.22.4   |
 |    scipy      |    ≥ 1.8.1    |
 |    tqdm       |    ≥ 4.64.1   |
 
 </div>
 
 </section>
 <section id='user-installation'>
@@ -204,15 +204,15 @@
 <section id='dependências'>
 
 ##### **Dependências:**
 <div align = center> 
 
 |    Pacotes    |     Versão    |
 |:-------------:|:-------------:|
-|    numpy      |    ≥ 1.23.0   |
+|    numpy      |    ≥ 1.22.4   |
 |    scipy      |    ≥ 1.8.1    |
 |    tqdm       |    ≥ 4.64.1   |
 
 </div>
 </section>
 
 <section id='instalação-do-usuário'>
```

### Comparing `aisp-0.1.0/README.md` & `aisp-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
 ##### **Dependencies:**
 <div align = center> 
 
 
 |    Packages   |     Version   |
 |:-------------:|:-------------:|
-|    numpy      |    ≥ 1.23.0   |
+|    numpy      |    ≥ 1.22.4   |
 |    scipy      |    ≥ 1.8.1    |
 |    tqdm       |    ≥ 4.64.1   |
 
 </div>
 
 </section>
 <section id='user-installation'>
@@ -180,15 +180,15 @@
 <section id='dependências'>
 
 ##### **Dependências:**
 <div align = center> 
 
 |    Pacotes    |     Versão    |
 |:-------------:|:-------------:|
-|    numpy      |    ≥ 1.23.0   |
+|    numpy      |    ≥ 1.22.4   |
 |    scipy      |    ≥ 1.8.1    |
 |    tqdm       |    ≥ 4.64.1   |
 
 </div>
 </section>
 
 <section id='instalação-do-usuário'>
```

### Comparing `aisp-0.1.0/aisp/NSA/_negativeSelection.py` & `aisp-0.1.1/aisp/NSA/_negativeSelection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import numpy.typing as npt
 from tqdm import tqdm
-from typing import Literal
+from typing import Dict, Literal, Union
 from collections import namedtuple
 from scipy.spatial.distance import hamming
 
 from aisp._base import Base
 
 
 class RNSA(Base):
@@ -70,18 +70,18 @@
     def __init__(
         self, 
         N: int = 100, 
         r: float = 0.05, 
         r_s: float = 0.0001, 
         k: int = 1, 
         metric: Literal['manhattan', 'minkowski', 'euclidean'] = 'euclidean', 
-        max_discards: int = 100, 
+        max_discards: int = 1000, 
         seed: int = None, 
         algorithm: Literal['default-NSA', 'V-detector'] ='default-NSA', 
-        cell_bounds: bool = False
+        **kwargs: Dict[str, Union[bool, str]]
     ):
         """
         Negative Selection class constructor (``RNSA``).
 
         Details:
         ---
             This method initializes the ``detectors``, ``classes``, ``k``, ``metric``, ``N``, ``r``, ``r_S``, 
@@ -99,28 +99,30 @@
                 * ``'Euclidean'`` ➜ The calculation of the distance is given by the expression: √( (x₁ – x₂)² + (y₁ – y₂)² + ... + (yn – yn)²).
                 * ``'minkowski'`` ➜ The calculation of the distance is given by the expression: ( |X₁ – Y₁|p + |X₂ – Y₂|p + ... + |Xn – Yn|p) ¹/ₚ, In this project ``p == 2``.
                 * ``'manhattan'`` ➜ The calculation of the distance is given by the expression: ( |x₁ – x₂| + |y₁ – y₂| + ... + |yn – yn|) .
 
             Defaults to ``'euclidean'``.
 
             * max_discards (``int``): This parameter indicates the maximum number of consecutive detector discards, aimed at preventing a 
-            possible infinite loop in case a radius is defined that cannot generate non-self detectors. Defaults to ``100``.
+            possible infinite loop in case a radius is defined that cannot generate non-self detectors. Defaults to ``1000``.
             * seed (``int``): Seed for the random generation of values in the detectors. Defaults to ``None``.
 
             * algorithm(``str``), Set the algorithm version:
 
                 * ``'default-NSA'``: Default algorithm with fixed radius.
                 * ``'V-detector'``: This algorithm is based on the article "[Real-Valued Negative Selection Algorithm with Variable-Sized Detectors](https://doi.org/10.1007/978-3-540-24854-5_30)", by Ji, Z., Dasgupta, D. (2004), and uses a variable radius for anomaly detection in feature spaces.
 
             Defaults to ``'default-NSA'``.
 
-            
-            * cell_bounds (``bool``): If set to ``True``, this option limits the generation of detectors to the space within 
-            the plane between 0 and 1. This means that any detector whose radius exceeds this limit is discarded, 
-            this variable is only used in the ``V-detector`` algorithm. Defaults to ``False``.
+            - ``**kwargs``:
+                    - non_self_label (``str``): This variable stores the label that will be assigned when the data has only one 
+                    output class, and the sample is classified as not belonging to that class. Defaults to ``'non-self'``.
+                    - cell_bounds (``bool``): If set to ``True``, this option limits the generation of detectors to the space within 
+                    the plane between 0 and 1. This means that any detector whose radius exceeds this limit is discarded, 
+                    this variable is only used in the ``V-detector`` algorithm. Defaults to ``False``.
 
         ---
 
         Construtor da classe de Seleção negativa (``RNSA``).
 
         Details:
         ---
@@ -138,26 +140,29 @@
                 * ``'euclidiana'`` ➜ O cálculo da distância dá-se pela expressão: √( (x₁ – x₂)² + (y₁ – y₂)² + ... + (yn – yn)²).
                 * ``'minkowski'``  ➜ O cálculo da distância dá-se pela expressão: ( |X₁ – Y₁|p + |X₂ – Y₂|p + ... + |Xn – Yn|p) ¹/ₚ, Neste projeto ``p == 2``.
                 * ``'manhattan'``  ➜ O cálculo da distância dá-se pela expressão: ( |x₁ – x₂| + |y₁ – y₂| + ... + |yn – yn|).
 
             Defaults to ``'euclidean'``.
 
             * max_discards (``int``): Este parâmetro indica o número máximo de descartes de detectores em sequência, que tem como objetivo evitar um 
-            possível loop infinito caso seja definido um raio que não seja possível gerar detectores do não-próprio. Defaults to ``100``.
+            possível loop infinito caso seja definido um raio que não seja possível gerar detectores do não-próprio. Defaults to ``1000``.
             * seed (``int``): Semente para a geração randômica dos valores nos detectores. Defaults to ``None``.
             * algorithm (``str``), Definir a versão do algoritmo:
 
                 * ``'default-NSA'``: Algoritmo padrão com raio fixo.
                 * ``'V-detector'``: Este algoritmo é baseado no artigo "[Real-Valued Negative Selection Algorithm with Variable-Sized Detectors](https://doi.org/10.1007/978-3-540-24854-5_30)", de autoria de Ji, Z., Dasgupta, D. (2004), e utiliza um raio variável para a detecção de anomalias em espaços de características. 
 
             Defaults to ``'default-NSA'``.
 
-            * cell_bounds (``bool``):  Se definido como ``True``, esta opção limita a geração dos detectores ao espaço do plano 
-            compreendido entre 0 e 1. Isso significa que qualquer detector cujo raio ultrapasse esse limite é descartado, 
-            e esta variável é usada exclusivamente no algoritmo ``V-detector``.
+            - ``**kwargs``:
+                    - non_self_label (``str``): Esta variável armazena o rótulo que será atribuído quando os dados possuírem 
+                    apenas uma classe de saída, e a amostra for classificada como não pertencente a essa classe. Defaults to ``'non-self'``.
+                    - cell_bounds (``bool``):  Se definido como ``True``, esta opção limita a geração dos detectores ao espaço do plano 
+                    compreendido entre 0 e 1. Isso significa que qualquer detector cujo raio ultrapasse esse limite é descartado, 
+                    e esta variável é usada exclusivamente no algoritmo ``V-detector``.
         """
         
         if metric == 'manhattan' or metric == 'minkowski' or metric == 'euclidean':
             self.metric = metric
         else:
             self.metric = 'euclidean'
 
@@ -190,17 +195,18 @@
         if algorithm == 'V-detector':
             self._Detector = namedtuple("Detector", "position radius")
             self._algorithm: str = algorithm
         else:
             self._Detector = namedtuple("Detector", "position")
             self._algorithm: str = 'default-NSA'
             
-        self._cell_bounds: bool = cell_bounds 
+        self._cell_bounds: bool = kwargs.get('cell_bounds', False)
+        self.non_self_label: str = kwargs.get('non_self_label', 'non-self')
         self.max_discards: int = max_discards
-        self.detectors: dict = None
+        self.detectors: Union[dict, None] = None
         self.classes: npt.NDArray = None
 
     def fit(self, X: npt.NDArray, y: npt.NDArray, verbose: bool = True):
         """
         The function ``fit(...)``, performs the training according to ``X`` and ``y``, using the method
         negative selection method(``NegativeSelect``).
 
@@ -225,27 +231,15 @@
             [``N amostras`` (linhas)][``N características`` (colunas)].
             * y (``npt.NDArray``):  Array com as classes alvos de ``X`` com [``N amostras`` (linhas)].
             * verbose (``bool``): Feedback da geração de detectores para o usuário.
         Returns:
         ---
             (``self``): Retorna a própria instância.
         """
-        if not isinstance(X,  (np.ndarray)):
-            if isinstance(X,  (list)):
-                X = np.array(X)
-            else:
-                raise TypeError("X is not an ndarray.")
-        elif not isinstance(y, (np.ndarray)):
-            if isinstance(y, (list)):
-                y = np.array(y)
-            else:
-                raise TypeError("y is not an ndarray.")
-        if X.shape[0] != y.shape[0]:
-            raise TypeError(
-                "X does not have the same amount of sample for the output classes in y.")
+        super()._check_and_raise_exceptions_fit(X, y)
         
         # Identificando as classes possíveis, dentro do array de saídas ``y``.
         self.classes = np.unique(y)
         # Dict que armazenará os detectores com as classes como key.
         list_detectors_by_class = dict()
         # Separa as classes para o treinamento.
         sample_index = self.__slice_index_list_by_class(y)
@@ -348,15 +342,15 @@
                 class_found = False
             else:
                 C = np.append(C, [_class_])
                 class_found = True
 
             # Se possuir apenas uma classe e não classificar a amostra define a saída como não-própria.
             if not class_found and len(self.classes) == 1:
-                C = np.append(C, ['non-self'])
+                C = np.append(C, [self.non_self_label])
             # Se não identificar a classe com os detectores, coloca a classe com a maior distância da média dos seus detectores.
             elif not class_found:
                 average_distance = dict()
                 for _class_ in self.classes:
                     detectores = list(
                         map(lambda x: x.position, self.detectors[_class_]))
                     average_distance[_class_] = self.__distance(
@@ -408,25 +402,27 @@
             # Se a média das distâncias na lista dos knn, for menor que o raio, retorna verdadeiro.
             distance_mean = np.mean(knn_list)
             if self._algorithm == 'V-detector':
                 return self.__detector_is_valid_to_Vdetector(distance_mean, vector_x)
             elif distance_mean > (self.r + self.r_s):
                 return True  # Detector é valido!
         else:
-            distance = None
+            distance: Union[float, None] = None
             for i in samples_index_class:
                 if self._algorithm == 'V-detector':
-                    if distance == None:
-                        distance = self.__distance(X[i], vector_x)
-                    elif distance > self.__distance(X[i], vector_x):
-                        distance = self.__distance(X[i], vector_x)
+                    new_distance = self.__distance(X[i], vector_x)
+                    if distance is None:
+                        distance = new_distance
+                    elif distance > new_distance:
+                        distance = new_distance
                 else:
                     # Calcula a distância entre os vetores, se menor ou igual ao raio + raio da amostra define a validade do detector como falso.
                     if (self.r + self.r_s) >= self.__distance(X[i], vector_x):
                         return False  # Detector não é valido!
+                    
             if self._algorithm == 'V-detector':
                 return self.__detector_is_valid_to_Vdetector(distance, vector_x)
             return True  # Detector é valido!
 
         return False  # Detector não é valido!
 
     def __compare_KnearestNeighbors_List(self, knn: npt.NDArray, distance: float) -> npt.NDArray:
@@ -559,15 +555,15 @@
             * u (``npt.NDArray``): Coordenadas do primeiro ponto.
             * v (``npt.NDArray``): Coordenadas do segundo ponto.
 
         Returns:
         ---
             * Distância (``double``) entre os dois pontos.
         """
-        return super().distance(u, v)
+        return super()._distance(u, v)
 
     def __detector_is_valid_to_Vdetector(self, distance: float, vector_x: npt.NDArray):
         """
         Check if the distance between the detector and the samples, minus the radius of the samples, 
         is greater than the minimum radius.
 
         Parameters:
@@ -629,15 +625,15 @@
         ---
             * y (npt.NDArray): Recebe um array ``y``[``N amostra``] com as classes de saida do array de amostra ``X``.
 
         Returns:
         ---
             * dict: Um dicionário com a lista de posições do array(``y``), com as classes como chave.
         """
-        return super().slice_index_list_by_class(y)
+        return super()._slice_index_list_by_class(y)
  
     def score(self, X: npt.NDArray, y: list) -> float:
         """
         Score function calculates forecast accuracy.
 
         Details:
         ---
@@ -677,15 +673,15 @@
 
         returns:
         ---
 
         accuracy : float
             A acurácia do modelo.
         """
-        return super().score(X, y)
+        return super()._score(X, y)
 
     def get_params(self, deep: bool = True) -> dict:
         return {
             'N': self.N,
             'r': self.r,
             'k': self.k,
             'metric': self.metric,
@@ -731,15 +727,15 @@
         * classes (``npt.NDArray``): lista com as classes de saída.
 
     """
     def __init__(
         self, 
         N: int = 100, 
         aff_thresh: float = 0.1, 
-        max_discards: int = 100, 
+        max_discards: int = 1000, 
         seed: int = None
     ):
         """
         Constructor of the Negative Selection class (``BNSA``).
         
          Details:
          ---
@@ -747,15 +743,15 @@
 
          Parameters:
          ---
              * N (``int``): Number of detectors. Defaults to ``100``.
              * aff_thresh (``float``): The variable represents the percentage of similarity between the T cell and the own samples.
              The default value is 10% (0.1), while a value of 1.0 represents 100% similarity.
              * max_discards (``int``): This parameter indicates the maximum number of detector discards in sequence, which aims to avoid a
-             possible infinite loop if a radius is defined that it is not possible to generate non-self detectors. Defaults to ``100``.
+             possible infinite loop if a radius is defined that it is not possible to generate non-self detectors. Defaults to ``1000``.
              * seed (``int``): Seed for the random generation of values in the detectors. Defaults to ``None``.
 
         ---
 
         Construtor da classe de Seleção negativa (``BNSA``).
         
         Details:
@@ -764,15 +760,15 @@
 
         Parameters:
         ---
             * N (``int``): Quantidade de detectores. Defaults to ``100``.
             * aff_thresh (``float``): A variável representa a porcentagem de similaridade entre a célula T e as amostras próprias. 
             O valor padrão é de 10% (0,1), enquanto que o valor de 1,0 representa 100% de similaridade.
             * max_discards (``int``): Este parâmetro indica o número máximo de descartes de detectores em sequência, que tem como objetivo evitar um 
-            possível loop infinito caso seja definido um raio que não seja possível gerar detectores do não-próprio. Defaults to ``100``.
+            possível loop infinito caso seja definido um raio que não seja possível gerar detectores do não-próprio. Defaults to ``1000``.
             * seed (``int``): Semente para a geração randômica dos valores nos detectores. Defaults to ``None``.
         """
         if N > 0:
             self.N: int = N
         else:
             self.N: int = 100
 
@@ -819,30 +815,15 @@
             [``N amostras`` (linhas)][``N características`` (colunas)].
             * y (``npt.NDArray``):  Array com as classes alvos de ``X`` com [``N amostras`` (linhas)].
             * verbose (``bool``): Feedback da geração de detectores para o usuário.
         Returns:
         ---
             (``self``): Retorna a própria instância.
         """
-        if not isinstance(X,  (np.ndarray)):
-            if isinstance(X,  (list)):
-                X = np.array(X)
-            else:
-                raise TypeError("X is not an ndarray.")
-        elif not isinstance(y, (np.ndarray)):
-            if isinstance(y, (list)):
-                y = np.array(y)
-            else:
-                raise TypeError("y is not an ndarray.")
-        if X.shape[0] != y.shape[0]:
-            raise TypeError(
-                "X does not have the same amount of sample for the output classes in y.")
-        elif not np.isin(X, [0, 1]).all():
-            raise Exception(
-                "The array X contains values that are not composed only of 0 and 1.")
+        super()._check_and_raise_exceptions_fit(X, y, 'BNSA')
 
         if X.dtype != bool:
             X = X.astype(bool)
 
         self.classes = np.unique(y)
         # Dict que armazenará os detectores com as classes como key.
         list_detectors_by_class = dict()
@@ -923,28 +904,31 @@
 
         Returns:
         ---
             * C – (``npt.NDArray``): um ndarray de forma ``C`` [``N amostras``], 
             contendo as classes previstas para ``X``.
             * ``None``: Se não existir detectores para a previsão.
         """
-        if not isinstance(X,  (np.ndarray)):
-            if isinstance(X,  (list)):
-                X = np.array(X)
-            else:
-                raise TypeError("X is not an ndarray.")
-        
+        # se não houver detectores retorna None.
+        if self.detectors is None:
+            return None
+        elif not isinstance(X,  (np.ndarray, list)):
+            raise TypeError("X is not an ndarray or list")
+        elif len(self.detectors[self.classes[0]][0]) != len(X[0]):
+            raise Exception('X does not have {} features to make the prediction'.format(
+                len(self.detectors[self.classes[0]][0])))
+        # Verifica se a matriz X contém apenas amostras binárias. Caso contrário, lança uma exceção.
         if not np.isin(X, [0, 1]).all():
-            raise Exception(
+            raise ValueError(
                 "The array X contains values that are not composed only of 0 and 1.")
 
         if X.dtype != bool:
             X = X.astype(bool)
             
-         # Inicia um array vazio.
+        # Inicia um array vazio.
         C = np.empty(shape=(0))
         # Para cada linha de amostra em X.
         for line in X:
             class_found: bool = True
             # Lista para armazenar as possíveis classes às quais a amostra se adequou ao self na comparação com os detectores non-self.
             possible_classes: list = [] 
             for _class_ in self.classes:
@@ -1005,15 +989,15 @@
         ---
             * y (npt.NDArray): Recebe um array ``y``[``N amostra``] com as classes de saida do array de amostra ``X``.
 
         Returns:
         ---
             * dict: Um dicionário com a lista de posições do array(``y``), com as classes como chave.
         """
-        return super().slice_index_list_by_class(y)
+        return super()._slice_index_list_by_class(y)
 
     def score(self, X: npt.NDArray, y: list) -> float:
         """
         Score function calculates forecast accuracy.
 
         Details:
         ---
@@ -1053,15 +1037,15 @@
 
         returns:
         ---
 
         accuracy : float
             A acurácia do modelo.
         """
-        return super().score(X, y)
+        return super()._score(X, y)
 
     def get_params(self, deep: bool = True) -> dict:
         return {
             'N': self.N,
             'aff_thresh': self.aff_thresh,
             'max_discards': self.max_discards,
             'seed': self.seed,
```

### Comparing `aisp-0.1.0/aisp.egg-info/PKG-INFO` & `aisp-0.1.1/aisp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aisp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Package with techniques of artificial immune systems.
 Author-email: João Paulo da Silva Barros <jpsilvabarr@gmail.com>
 Maintainer-email: Alison Zille Lopes <alisonzille@gmail.com>
 License: LGPL-3.0 license
 Project-URL: Homepage, https://ais-package.github.io/
 Project-URL: Documentation, https://ais-package.github.io/docs/intro
 Project-URL: Source Code, https://github.com/AIS-Package/aisp
@@ -95,15 +95,15 @@
 
 ##### **Dependencies:**
 <div align = center> 
 
 
 |    Packages   |     Version   |
 |:-------------:|:-------------:|
-|    numpy      |    ≥ 1.23.0   |
+|    numpy      |    ≥ 1.22.4   |
 |    scipy      |    ≥ 1.8.1    |
 |    tqdm       |    ≥ 4.64.1   |
 
 </div>
 
 </section>
 <section id='user-installation'>
@@ -204,15 +204,15 @@
 <section id='dependências'>
 
 ##### **Dependências:**
 <div align = center> 
 
 |    Pacotes    |     Versão    |
 |:-------------:|:-------------:|
-|    numpy      |    ≥ 1.23.0   |
+|    numpy      |    ≥ 1.22.4   |
 |    scipy      |    ≥ 1.8.1    |
 |    tqdm       |    ≥ 4.64.1   |
 
 </div>
 </section>
 
 <section id='instalação-do-usuário'>
```

### Comparing `aisp-0.1.0/pyproject.toml` & `aisp-0.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aisp"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="João Paulo da Silva Barros", email="jpsilvabarr@gmail.com" },
 ]
 
 maintainers = [
   { name="Alison Zille Lopes",  email="alisonzille@gmail.com"},
 ]
@@ -29,15 +29,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
-    "numpy>=1.23.0",
+    "numpy>=1.22.4",
     "scipy>=1.8.1",
     "tqdm==4.64.1",
 ]
 
 keywords = ["Artificial Immune Systems", "classification", "Natural computing", "machine learning", "artificial intelligence"]
 
 [project.urls]
```

