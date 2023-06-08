# Comparing `tmp/jquants_derivatives-0.1.0a2.tar.gz` & `tmp/jquants_derivatives-0.1.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jquants_derivatives-0.1.0a2.tar", max compression
+gzip compressed data, was "jquants_derivatives-0.1.0a3.tar", max compression
```

## Comparing `jquants_derivatives-0.1.0a2.tar` & `jquants_derivatives-0.1.0a3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8758 2023-06-08 05:22:56.205337 jquants_derivatives-0.1.0a2/README.md
--rw-r--r--   0        0        0      124 2023-06-06 14:36:12.452162 jquants_derivatives-0.1.0a2/jquants_derivatives/__init__.py
--rw-r--r--   0        0        0     1870 2023-06-06 15:52:55.552479 jquants_derivatives-0.1.0a2/jquants_derivatives/client.py
--rw-r--r--   0        0        0     1290 2023-06-05 23:18:08.508412 jquants_derivatives-0.1.0a2/jquants_derivatives/database.py
--rw-r--r--   0        0        0     5337 2023-06-06 15:43:26.519073 jquants_derivatives-0.1.0a2/jquants_derivatives/derivatievs.py
--rw-r--r--   0        0        0     1302 2023-06-06 15:08:31.605466 jquants_derivatives-0.1.0a2/jquants_derivatives/models.py
--rw-r--r--   0        0        0      656 2023-06-08 05:27:40.458941 jquants_derivatives-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     9716 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a2/setup.py
--rw-r--r--   0        0        0     9258 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11613 2023-06-08 05:55:52.593917 jquants_derivatives-0.1.0a3/README.md
+-rw-r--r--   0        0        0      124 2023-06-06 14:36:12.452162 jquants_derivatives-0.1.0a3/jquants_derivatives/__init__.py
+-rw-r--r--   0        0        0     1870 2023-06-06 15:52:55.552479 jquants_derivatives-0.1.0a3/jquants_derivatives/client.py
+-rw-r--r--   0        0        0     1290 2023-06-05 23:18:08.508412 jquants_derivatives-0.1.0a3/jquants_derivatives/database.py
+-rw-r--r--   0        0        0     5337 2023-06-06 15:43:26.519073 jquants_derivatives-0.1.0a3/jquants_derivatives/derivatievs.py
+-rw-r--r--   0        0        0     1302 2023-06-06 15:08:31.605466 jquants_derivatives-0.1.0a3/jquants_derivatives/models.py
+-rw-r--r--   0        0        0      656 2023-06-08 05:55:53.680623 jquants_derivatives-0.1.0a3/pyproject.toml
+-rw-r--r--   0        0        0    12658 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a3/setup.py
+-rw-r--r--   0        0        0    12113 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a3/PKG-INFO
```

### Comparing `jquants_derivatives-0.1.0a2/README.md` & `jquants_derivatives-0.1.0a3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -52,14 +52,97 @@
 
 |    | Date                |      Code |   WholeDayOpen |   WholeDayHigh |   WholeDayLow |   WholeDayClose |
 |---:|:--------------------|----------:|---------------:|---------------:|--------------:|----------------:|
 |  0 | 2023-06-05 00:00:00 | 130060018 |              0 |              0 |             0 |               0 |
 |  1 | 2023-06-05 00:00:00 | 130060218 |              0 |              0 |             0 |               0 |
 |  2 | 2023-06-05 00:00:00 | 130060518 |              0 |              0 |             0 |               0 |
 
+### 型変換機能
+
+DataFrameの各列データ型は [jquants_derivatives.models](https://github.com/drillan/jquants-derivatives/blob/main/jquants_derivatives/models.py) で定義したデータ型にしたがって、自動的に型変換されます。
+
+```python
+jquants_derivatives.models.IndexOption??
+```
+
+```python
+Init signature:
+jquants_derivatives.models.IndexOption(
+    Date: dtype('<M8[ns]'),
+    Code: str,
+    WholeDayOpen: float,
+    WholeDayHigh: float,
+    WholeDayLow: float,
+    WholeDayClose: float,
+    NightSessionOpen: float,
+    NightSessionHigh: float,
+    NightSessionLow: float,
+    NightSessionClose: float,
+    DaySessionOpen: float,
+    DaySessionHigh: float,
+    DaySessionLow: float,
+    DaySessionClose: float,
+    Volume: float,
+    OpenInterest: float,
+    TurnoverValue: float,
+    ContractMonth: str,
+    StrikePrice: float,
+    VolumeOnlyAuction: float,
+    EmergencyMarginTriggerDivision: str,
+    PutCallDivision: int,
+    LastTradingDay: dtype('<M8[ns]'),
+...
+        key = field.replace("(", "").replace(")", "")
+        return cls.__annotations__[key]
+File:           ~/repo/jquants-derivatives/jquants_derivatives/models.py
+Type:           ABCMeta
+Subclasses:     
+```
+
+```python
+df_20230605.dtypes
+```
+
+```
+Date                              datetime64[ns]
+Code                                      object
+WholeDayOpen                             float64
+WholeDayHigh                             float64
+WholeDayLow                              float64
+WholeDayClose                            float64
+NightSessionOpen                         float64
+NightSessionHigh                         float64
+NightSessionLow                          float64
+NightSessionClose                        float64
+DaySessionOpen                           float64
+DaySessionHigh                           float64
+DaySessionLow                            float64
+DaySessionClose                          float64
+Volume                                   float64
+OpenInterest                             float64
+TurnoverValue                            float64
+ContractMonth                             object
+StrikePrice                              float64
+Volume(OnlyAuction)                      float64
+EmergencyMarginTriggerDivision            object
+PutCallDivision                            int64
+LastTradingDay                    datetime64[ns]
+SpecialQuotationDay               datetime64[ns]
+SettlementPrice                          float64
+...
+BaseVolatility                           float64
+UnderlyingPrice                          float64
+ImpliedVolatility                        float64
+InterestRate                             float64
+dtype: object
+```
+
+
+### キャッシュ機能
+
 同じデータを取得した場合、データはsqlite3のデータベースにキャッシュされるため、2回目以降の実行ではキャッシュされたデータをもとに DataFrame を返します。
 
 ```python
 %%time
 df_20230605 = cli.get_option_index_option("2023-06-05")
 ```
 
@@ -208,22 +291,22 @@
 
 `plot_volatility` 関数はボラティリティスマイルを可視化します。引数には `Option` クラスのインスタンスを渡します。
 
 ```python
 jquants_derivatives.plot_volatility(op_20230605)
 ```
 
-![op_20230605](./docs/images/op_20230605.png)
+![op_20230605](https://github.com/drillan/jquants-derivatives/blob/main/docs/images/op_20230605.png?raw=true)
 
 ```python
 op_2023060 = Option(df_20230605, contracts=2)
 ```
 
 複数の時間帯を比較して可視化するには、 `plot_volatility` 関数の第2引数に比較対象の `Option` インスタンスを渡します。
 
 ```python
 df_20230602 = cli.get_option_index_option("2023-06-02")
 op_20230602 = Option(df_20230602)
 jquants_derivatives.plot_volatility(op_20230605, op_20230602)
 ```
 
-![op_20230602](./docs/images/op_20230602.png)
+![op_20230602](https://github.com/drillan/jquants-derivatives/blob/main/docs/images/op_20230602.png?raw=true)
```

### Comparing `jquants_derivatives-0.1.0a2/jquants_derivatives/client.py` & `jquants_derivatives-0.1.0a3/jquants_derivatives/client.py`

 * *Files identical despite different names*

### Comparing `jquants_derivatives-0.1.0a2/jquants_derivatives/database.py` & `jquants_derivatives-0.1.0a3/jquants_derivatives/database.py`

 * *Files identical despite different names*

### Comparing `jquants_derivatives-0.1.0a2/jquants_derivatives/derivatievs.py` & `jquants_derivatives-0.1.0a3/jquants_derivatives/derivatievs.py`

 * *Files identical despite different names*

### Comparing `jquants_derivatives-0.1.0a2/jquants_derivatives/models.py` & `jquants_derivatives-0.1.0a3/jquants_derivatives/models.py`

 * *Files identical despite different names*

### Comparing `jquants_derivatives-0.1.0a2/pyproject.toml` & `jquants_derivatives-0.1.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jquants-derivatives"
-version = "0.1.0-alpha2"
+version = "0.1.0-alpha3"
 description = "J-Quants API Client Derivatives Library"
 authors = ["driller"]
 readme = "README.md"
 packages = [{include = "jquants_derivatives"}]
 homepage = "https://github.com/drillan/jquants-derivatives"
 
 [tool.poetry.dependencies]
```

### Comparing `jquants_derivatives-0.1.0a2/setup.py` & `jquants_derivatives-0.1.0a3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['jquants-api-client>=1.2.0,<2.0.0', 'plotly>=5.14.1,<6.0.0']
 
 setup_kwargs = {
     'name': 'jquants-derivatives',
-    'version': '0.1.0a2',
+    'version': '0.1.0a3',
     'description': 'J-Quants API Client Derivatives Library',
-    'long_description': '# jquants-derivatives\n\n[![PyPI version](https://badge.fury.io/py/jquants-derivatives.svg)](https://badge.fury.io/py/jquants-derivatives)\n\n個人投資家向けデータ API 配信サービス「 [J-Quants API](https://jpx-jquants.com/#jquants-api) 」の [Python クライアントライブラリ](https://github.com/J-Quants/jquants-api-client-python) のデリバティブ用ラッパーです。\n\njquants-derivatives ではオプションのデータを利用するため、J-Quants APIのスタンダード以上のプランが必要です。\n\nJ-Quants や API 仕様についての詳細を知りたい方は [公式ウェブサイト](https://jpx-jquants.com/) をご参照ください。\n現在、J-Quants API は有償版サービスとして提供されています。\n\n## インストール方法\n\n`pip` コマンドでインストールします。\n\n```bash\npip install jquants-derivatives\n```\n\n### J-Quants API の利用\n\nTo use J-Quants API, you need to "Applications for J-Quants API" from [J-Quants API Web site](https://jpx-jquants.com/?lang=en) and to select a plan.\n\nJ-Quants API を利用するためには[J-Quants API の Web サイト](https://jpx-jquants.com/) から「J-Quants API 申し込み」及び利用プランの選択が必要になります。\n\njquants-api-client-python を使用するためには「J-Quants API ログインページで使用するメールアドレスおよびパスワード」または「J-Quants API メニューページから取得したリフレッシュトークン」が必要になります。必要に応じて下記の Web サイトより取得してください。\n\n[J-Quants API ログインページ](https://jpx-jquants.com/auth/signin/)\n\n## 認証設定\n\nコードを実行する前に認証設定をしておきます。設定方法は [jquants-api-clientの設定](https://github.com/J-Quants/jquants-api-client-python#%E8%A8%AD%E5%AE%9A) を参照してください。\n\n\n[Google Colab](https://colab.research.google.com/) を利用する場合は [jquants-api-clientのサンプルノートブック](https://github.com/J-Quants/jquants-api-client-python/tree/main/examples#google-colab) を参考にしてください。\n\n## 使用方法\n\n### Clientクラス\n\n`jquants_derivatives.Client` クラスは `jquantsapi.Client` クラスを継承しています。\n[\njquants-api-client-python](https://github.com/J-Quants/jquants-api-client-python) の `Client` クラスと同じ方法で `pandas.DataFrame` を取得します。\n\n```python\nimport jquants_derivatives\n\ncli = jquants_derivatives.Client()\ndf_20230605 = cli.get_option_index_option("2023-06-05")\ndf_20230605.iloc[:3, :6]\n```\n\n|    | Date                |      Code |   WholeDayOpen |   WholeDayHigh |   WholeDayLow |   WholeDayClose |\n|---:|:--------------------|----------:|---------------:|---------------:|--------------:|----------------:|\n|  0 | 2023-06-05 00:00:00 | 130060018 |              0 |              0 |             0 |               0 |\n|  1 | 2023-06-05 00:00:00 | 130060218 |              0 |              0 |             0 |               0 |\n|  2 | 2023-06-05 00:00:00 | 130060518 |              0 |              0 |             0 |               0 |\n\n同じデータを取得した場合、データはsqlite3のデータベースにキャッシュされるため、2回目以降の実行ではキャッシュされたデータをもとに DataFrame を返します。\n\n```python\n%%time\ndf_20230605 = cli.get_option_index_option("2023-06-05")\n```\n\n```\nCPU times: user 289 ms, sys: 194 ms, total: 483 ms\nWall time: 482 ms\n```\n\nキャッシュされたデータは `${HOME}/.jquants-api/jquantsapi.db` に格納されます。\n\n次のようにSQLを使ってデータを取得できます。\nIPythonまたはノートブック（Jupyter/Colabなど）からSQLを実行する場合は [ipython-sql](https://jupyter-tutorial.readthedocs.io/en/stable/data-processing/postgresql/ipython-sql.html) をインストールし、ロードします。\n\n```bash\npip install ipython-sql\n```\n\n```\n%load_ext sql\n```\n\nキャッシュの保存先を確認します。\n\n```python\nprint(jquants_derivatives.database.db)\n```\n\n```\n/your_home_dir/.jquants-api/jquantsapi.db\n```\n\nDBに接続し、SQLを実行します。\n\n```\n%sql sqlite:////your_home_dir/.jquants-api/jquantsapi.db\n```\n\n```\n%sql SELECT name FROM sqlite_master WHERE type=\'table\';\n```\n\n|    | name                        |\n|---:|:----------------------------|\n|  0 | FINS_ANNOUNCEMENT           |\n|  1 | FINS_DIVIDEND               |\n|  2 | FINS_STATEMENTS             |\n|  3 | INDICES_TOPIX               |\n|  4 | LISTED_INFO                 |\n|  5 | MARKETS_BREAKDOWN           |\n|  6 | MARKET_SEGMENT              |\n|  7 | MARKET_SHORT_SELLING        |\n|  8 | OPTION_INDEX_OPTION         |\n|  9 | PRICES_DAILY_QUOTES         |\n| 10 | PRICES_DAILY_QUOTES_PREMIUM |\n| 11 | PRICES_PRICES_AM            |\n| 12 | SECTOR_17                   |\n| 13 | SECTOR_33                   |\n\n```\n%sql SELECT UnderlyingPrice from OPTION_INDEX_OPTION LIMIT 3;\n```\n\n|    |   UnderlyingPrice |\n|---:|------------------:|\n|  0 |           29520.1 |\n|  1 |           29520.1 |\n|  2 |           29520.1 |\n\n### Optionクラス\n\n`jquants_derivatives.Option` クラスはAPIから得られたオプションのデータを整形し、実務上扱いやすい形式に変換するクラスです。引数には `get_option_index_option` メソッドで取得した DataFrme を渡します。引数 `contracts` には対象とする限月数を渡します（デフォルトは2）。\n\n```python\nop_20230605 = Option(df_20230605, contracts=2)\n```\n\n`contract_month` 属性は限月（ContractMonth）のリストを返します。\n\n```python\nop_20230605.contract_month\n```\n\n```python\n[\'2023-06\', \'2023-07\']\n```\n\n\n`underlying_price` 属性は限月ごとの原資産価格（UnderlyingPrice）の辞書を返します。\n\n```python\nop_20230605.underlying_price\n```\n\n```python\n{\'2023-06\': 32217.43, \'2023-07\': 32217.43}\n```\n\n`base_volatility` 属性は限月ごとの基準ボラティリティ（BaseVolatility）の辞書を返します。\n\n```python\nop_20230605.base_volatility\n```\n\n```python\n{\'2023-06\': 0.1951205, \'2023-07\': 0.1951205}\n```\n\n`op_2023060.interest_rate` 属性は限月ごとの理論価格計算用金利（InterestRate）の辞書を返します。\n\n```python\nop_20230605.interest_rate\n```\n\n```python\n{\'2023-06\': -0.000664, \'2023-07\': 0.000455}\n```\n\n`contracts_dfs` 属性は限月ごとの次の処理をした DataFrame を返します。\n\n- 取引高（Volume）が0のデータを除外\n- ITMのデータを除外し、OTMのデータを抽出\n- プレミアム（WholeDayClose）の最小値（デフォルトは1）までとし、最小値よりアウト型のデータを除外\n\n```python\nop_20230605.contracts_dfs["2023-06"].iloc[:3, :5]\n```\n\n|    | Date                |      Code |   WholeDayOpen |   WholeDayHigh |   WholeDayLow |\n|---:|:--------------------|----------:|---------------:|---------------:|--------------:|\n|  0 | 2023-06-05 00:00:00 | 138067618 |              3 |              3 |             1 |\n|  1 | 2023-06-05 00:00:00 | 188067718 |              3 |              4 |             1 |\n|  2 | 2023-06-05 00:00:00 | 138067818 |              3 |              4 |             2 |\n\n\n```python\nop_20230605.contracts_dfs["2023-07"].iloc[:3, :5]\n```\n\n|    | Date                |      Code |   WholeDayOpen |   WholeDayHigh |   WholeDayLow |   WholeDayClose |   NightSessionOpen |\n|---:|:--------------------|----------:|---------------:|---------------:|--------------:|----------------:|-------------------:|\n|  0 | 2023-06-05 00:00:00 | 138067618 |              3 |              3 |             1 |               1 |                  3 |\n|  1 | 2023-06-05 00:00:00 | 188067718 |              3 |              4 |             1 |               2 |                  3 |\n|  2 | 2023-06-05 00:00:00 | 138067818 |              3 |              4 |             2 |               2 |                  3 |\n\n### ボラティリティの可視化\n\n`plot_volatility` 関数はボラティリティスマイルを可視化します。引数には `Option` クラスのインスタンスを渡します。\n\n```python\njquants_derivatives.plot_volatility(op_20230605)\n```\n\n![op_20230605](./docs/images/op_20230605.png)\n\n```python\nop_2023060 = Option(df_20230605, contracts=2)\n```\n\n複数の時間帯を比較して可視化するには、 `plot_volatility` 関数の第2引数に比較対象の `Option` インスタンスを渡します。\n\n```python\ndf_20230602 = cli.get_option_index_option("2023-06-02")\nop_20230602 = Option(df_20230602)\njquants_derivatives.plot_volatility(op_20230605, op_20230602)\n```\n\n![op_20230602](./docs/images/op_20230602.png)',
+    'long_description': '# jquants-derivatives\n\n[![PyPI version](https://badge.fury.io/py/jquants-derivatives.svg)](https://badge.fury.io/py/jquants-derivatives)\n\n個人投資家向けデータ API 配信サービス「 [J-Quants API](https://jpx-jquants.com/#jquants-api) 」の [Python クライアントライブラリ](https://github.com/J-Quants/jquants-api-client-python) のデリバティブ用ラッパーです。\n\njquants-derivatives ではオプションのデータを利用するため、J-Quants APIのスタンダード以上のプランが必要です。\n\nJ-Quants や API 仕様についての詳細を知りたい方は [公式ウェブサイト](https://jpx-jquants.com/) をご参照ください。\n現在、J-Quants API は有償版サービスとして提供されています。\n\n## インストール方法\n\n`pip` コマンドでインストールします。\n\n```bash\npip install jquants-derivatives\n```\n\n### J-Quants API の利用\n\nTo use J-Quants API, you need to "Applications for J-Quants API" from [J-Quants API Web site](https://jpx-jquants.com/?lang=en) and to select a plan.\n\nJ-Quants API を利用するためには[J-Quants API の Web サイト](https://jpx-jquants.com/) から「J-Quants API 申し込み」及び利用プランの選択が必要になります。\n\njquants-api-client-python を使用するためには「J-Quants API ログインページで使用するメールアドレスおよびパスワード」または「J-Quants API メニューページから取得したリフレッシュトークン」が必要になります。必要に応じて下記の Web サイトより取得してください。\n\n[J-Quants API ログインページ](https://jpx-jquants.com/auth/signin/)\n\n## 認証設定\n\nコードを実行する前に認証設定をしておきます。設定方法は [jquants-api-clientの設定](https://github.com/J-Quants/jquants-api-client-python#%E8%A8%AD%E5%AE%9A) を参照してください。\n\n\n[Google Colab](https://colab.research.google.com/) を利用する場合は [jquants-api-clientのサンプルノートブック](https://github.com/J-Quants/jquants-api-client-python/tree/main/examples#google-colab) を参考にしてください。\n\n## 使用方法\n\n### Clientクラス\n\n`jquants_derivatives.Client` クラスは `jquantsapi.Client` クラスを継承しています。\n[\njquants-api-client-python](https://github.com/J-Quants/jquants-api-client-python) の `Client` クラスと同じ方法で `pandas.DataFrame` を取得します。\n\n```python\nimport jquants_derivatives\n\ncli = jquants_derivatives.Client()\ndf_20230605 = cli.get_option_index_option("2023-06-05")\ndf_20230605.iloc[:3, :6]\n```\n\n|    | Date                |      Code |   WholeDayOpen |   WholeDayHigh |   WholeDayLow |   WholeDayClose |\n|---:|:--------------------|----------:|---------------:|---------------:|--------------:|----------------:|\n|  0 | 2023-06-05 00:00:00 | 130060018 |              0 |              0 |             0 |               0 |\n|  1 | 2023-06-05 00:00:00 | 130060218 |              0 |              0 |             0 |               0 |\n|  2 | 2023-06-05 00:00:00 | 130060518 |              0 |              0 |             0 |               0 |\n\n### 型変換機能\n\nDataFrameの各列データ型は [jquants_derivatives.models](https://github.com/drillan/jquants-derivatives/blob/main/jquants_derivatives/models.py) で定義したデータ型にしたがって、自動的に型変換されます。\n\n```python\njquants_derivatives.models.IndexOption??\n```\n\n```python\nInit signature:\njquants_derivatives.models.IndexOption(\n    Date: dtype(\'<M8[ns]\'),\n    Code: str,\n    WholeDayOpen: float,\n    WholeDayHigh: float,\n    WholeDayLow: float,\n    WholeDayClose: float,\n    NightSessionOpen: float,\n    NightSessionHigh: float,\n    NightSessionLow: float,\n    NightSessionClose: float,\n    DaySessionOpen: float,\n    DaySessionHigh: float,\n    DaySessionLow: float,\n    DaySessionClose: float,\n    Volume: float,\n    OpenInterest: float,\n    TurnoverValue: float,\n    ContractMonth: str,\n    StrikePrice: float,\n    VolumeOnlyAuction: float,\n    EmergencyMarginTriggerDivision: str,\n    PutCallDivision: int,\n    LastTradingDay: dtype(\'<M8[ns]\'),\n...\n        key = field.replace("(", "").replace(")", "")\n        return cls.__annotations__[key]\nFile:           ~/repo/jquants-derivatives/jquants_derivatives/models.py\nType:           ABCMeta\nSubclasses:     \n```\n\n```python\ndf_20230605.dtypes\n```\n\n```\nDate                              datetime64[ns]\nCode                                      object\nWholeDayOpen                             float64\nWholeDayHigh                             float64\nWholeDayLow                              float64\nWholeDayClose                            float64\nNightSessionOpen                         float64\nNightSessionHigh                         float64\nNightSessionLow                          float64\nNightSessionClose                        float64\nDaySessionOpen                           float64\nDaySessionHigh                           float64\nDaySessionLow                            float64\nDaySessionClose                          float64\nVolume                                   float64\nOpenInterest                             float64\nTurnoverValue                            float64\nContractMonth                             object\nStrikePrice                              float64\nVolume(OnlyAuction)                      float64\nEmergencyMarginTriggerDivision            object\nPutCallDivision                            int64\nLastTradingDay                    datetime64[ns]\nSpecialQuotationDay               datetime64[ns]\nSettlementPrice                          float64\n...\nBaseVolatility                           float64\nUnderlyingPrice                          float64\nImpliedVolatility                        float64\nInterestRate                             float64\ndtype: object\n```\n\n\n### キャッシュ機能\n\n同じデータを取得した場合、データはsqlite3のデータベースにキャッシュされるため、2回目以降の実行ではキャッシュされたデータをもとに DataFrame を返します。\n\n```python\n%%time\ndf_20230605 = cli.get_option_index_option("2023-06-05")\n```\n\n```\nCPU times: user 289 ms, sys: 194 ms, total: 483 ms\nWall time: 482 ms\n```\n\nキャッシュされたデータは `${HOME}/.jquants-api/jquantsapi.db` に格納されます。\n\n次のようにSQLを使ってデータを取得できます。\nIPythonまたはノートブック（Jupyter/Colabなど）からSQLを実行する場合は [ipython-sql](https://jupyter-tutorial.readthedocs.io/en/stable/data-processing/postgresql/ipython-sql.html) をインストールし、ロードします。\n\n```bash\npip install ipython-sql\n```\n\n```\n%load_ext sql\n```\n\nキャッシュの保存先を確認します。\n\n```python\nprint(jquants_derivatives.database.db)\n```\n\n```\n/your_home_dir/.jquants-api/jquantsapi.db\n```\n\nDBに接続し、SQLを実行します。\n\n```\n%sql sqlite:////your_home_dir/.jquants-api/jquantsapi.db\n```\n\n```\n%sql SELECT name FROM sqlite_master WHERE type=\'table\';\n```\n\n|    | name                        |\n|---:|:----------------------------|\n|  0 | FINS_ANNOUNCEMENT           |\n|  1 | FINS_DIVIDEND               |\n|  2 | FINS_STATEMENTS             |\n|  3 | INDICES_TOPIX               |\n|  4 | LISTED_INFO                 |\n|  5 | MARKETS_BREAKDOWN           |\n|  6 | MARKET_SEGMENT              |\n|  7 | MARKET_SHORT_SELLING        |\n|  8 | OPTION_INDEX_OPTION         |\n|  9 | PRICES_DAILY_QUOTES         |\n| 10 | PRICES_DAILY_QUOTES_PREMIUM |\n| 11 | PRICES_PRICES_AM            |\n| 12 | SECTOR_17                   |\n| 13 | SECTOR_33                   |\n\n```\n%sql SELECT UnderlyingPrice from OPTION_INDEX_OPTION LIMIT 3;\n```\n\n|    |   UnderlyingPrice |\n|---:|------------------:|\n|  0 |           29520.1 |\n|  1 |           29520.1 |\n|  2 |           29520.1 |\n\n### Optionクラス\n\n`jquants_derivatives.Option` クラスはAPIから得られたオプションのデータを整形し、実務上扱いやすい形式に変換するクラスです。引数には `get_option_index_option` メソッドで取得した DataFrme を渡します。引数 `contracts` には対象とする限月数を渡します（デフォルトは2）。\n\n```python\nop_20230605 = Option(df_20230605, contracts=2)\n```\n\n`contract_month` 属性は限月（ContractMonth）のリストを返します。\n\n```python\nop_20230605.contract_month\n```\n\n```python\n[\'2023-06\', \'2023-07\']\n```\n\n\n`underlying_price` 属性は限月ごとの原資産価格（UnderlyingPrice）の辞書を返します。\n\n```python\nop_20230605.underlying_price\n```\n\n```python\n{\'2023-06\': 32217.43, \'2023-07\': 32217.43}\n```\n\n`base_volatility` 属性は限月ごとの基準ボラティリティ（BaseVolatility）の辞書を返します。\n\n```python\nop_20230605.base_volatility\n```\n\n```python\n{\'2023-06\': 0.1951205, \'2023-07\': 0.1951205}\n```\n\n`op_2023060.interest_rate` 属性は限月ごとの理論価格計算用金利（InterestRate）の辞書を返します。\n\n```python\nop_20230605.interest_rate\n```\n\n```python\n{\'2023-06\': -0.000664, \'2023-07\': 0.000455}\n```\n\n`contracts_dfs` 属性は限月ごとの次の処理をした DataFrame を返します。\n\n- 取引高（Volume）が0のデータを除外\n- ITMのデータを除外し、OTMのデータを抽出\n- プレミアム（WholeDayClose）の最小値（デフォルトは1）までとし、最小値よりアウト型のデータを除外\n\n```python\nop_20230605.contracts_dfs["2023-06"].iloc[:3, :5]\n```\n\n|    | Date                |      Code |   WholeDayOpen |   WholeDayHigh |   WholeDayLow |\n|---:|:--------------------|----------:|---------------:|---------------:|--------------:|\n|  0 | 2023-06-05 00:00:00 | 138067618 |              3 |              3 |             1 |\n|  1 | 2023-06-05 00:00:00 | 188067718 |              3 |              4 |             1 |\n|  2 | 2023-06-05 00:00:00 | 138067818 |              3 |              4 |             2 |\n\n\n```python\nop_20230605.contracts_dfs["2023-07"].iloc[:3, :5]\n```\n\n|    | Date                |      Code |   WholeDayOpen |   WholeDayHigh |   WholeDayLow |   WholeDayClose |   NightSessionOpen |\n|---:|:--------------------|----------:|---------------:|---------------:|--------------:|----------------:|-------------------:|\n|  0 | 2023-06-05 00:00:00 | 138067618 |              3 |              3 |             1 |               1 |                  3 |\n|  1 | 2023-06-05 00:00:00 | 188067718 |              3 |              4 |             1 |               2 |                  3 |\n|  2 | 2023-06-05 00:00:00 | 138067818 |              3 |              4 |             2 |               2 |                  3 |\n\n### ボラティリティの可視化\n\n`plot_volatility` 関数はボラティリティスマイルを可視化します。引数には `Option` クラスのインスタンスを渡します。\n\n```python\njquants_derivatives.plot_volatility(op_20230605)\n```\n\n![op_20230605](https://github.com/drillan/jquants-derivatives/blob/main/docs/images/op_20230605.png?raw=true)\n\n```python\nop_2023060 = Option(df_20230605, contracts=2)\n```\n\n複数の時間帯を比較して可視化するには、 `plot_volatility` 関数の第2引数に比較対象の `Option` インスタンスを渡します。\n\n```python\ndf_20230602 = cli.get_option_index_option("2023-06-02")\nop_20230602 = Option(df_20230602)\njquants_derivatives.plot_volatility(op_20230605, op_20230602)\n```\n\n![op_20230602](https://github.com/drillan/jquants-derivatives/blob/main/docs/images/op_20230602.png?raw=true)',
     'author': 'driller',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/drillan/jquants-derivatives',
     'packages': packages,
     'package_data': package_data,
```

