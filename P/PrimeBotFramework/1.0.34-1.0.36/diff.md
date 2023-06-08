# Comparing `tmp/PrimeBotFramework-1.0.34.tar.gz` & `tmp/PrimeBotFramework-1.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-xdhe40q0/PrimeBotFramework-1.0.34.tar", last modified: Thu Jun  8 11:54:56 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-mlxcdra4/PrimeBotFramework-1.0.36.tar", last modified: Thu Jun  8 14:34:16 2023, max compression
```

## Comparing `PrimeBotFramework-1.0.34.tar` & `PrimeBotFramework-1.0.36.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/B2E/
--rw-rw-rw-   0 root         (0) root         (0)     4028 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/B2E/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/Cnab750/
--rw-rw-rw-   0 root         (0) root         (0)    10211 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/Cnab750/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/
--rw-rw-rw-   0 root         (0) root         (0)     1963 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/api_codes.py
--rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/D4Sign/
--rw-rw-rw-   0 root         (0) root         (0)     2600 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/D4Sign/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.195003 PrimeBotFramework-1.0.34/PrimeBot/DeathByCaptcha/
--rw-rw-rw-   0 root         (0) root         (0)     2822 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/DeathByCaptcha/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/Documents/
--rw-rw-rw-   0 root         (0) root         (0)     1098 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/Documents/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/Elastic/
--rw-rw-rw-   0 root         (0) root         (0)     1239 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/Elastic/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/ExchangeGraph/
--rw-rw-rw-   0 root         (0) root         (0)     8987 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/ExchangeGraph/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/FeriadosBancarios/
--rw-rw-rw-   0 root         (0) root         (0)     1925 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/FeriadosBancarios/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/FeriadosBancarios/model.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/IntegracaoSendGrid/
--rw-rw-rw-   0 root         (0) root         (0)     4251 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/IntegracaoSendGrid/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/ListenerECS/
--rw-rw-rw-   0 root         (0) root         (0)     4096 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/ListenerECS/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/Mongo/
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/Mongo/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/OracleDB/
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/OracleDB/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBot/Vault/
--rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/Vault/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/PrimeBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-08 11:54:56.000000 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-06-08 11:54:56.000000 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-08 11:54:56.000000 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-08 11:54:56.000000 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-08 11:54:56.000000 PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-08 11:54:56.199003 PrimeBotFramework-1.0.34/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-08 11:54:46.000000 PrimeBotFramework-1.0.34/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.742540 PrimeBotFramework-1.0.36/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PKG-INFO
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.742540 PrimeBotFramework-1.0.36/PrimeBot/
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.742540 PrimeBotFramework-1.0.36/PrimeBot/B2E/
+-rw-rw-rw-   0 root         (0) root         (0)     4028 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/B2E/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.742540 PrimeBotFramework-1.0.36/PrimeBot/Cnab750/
+-rw-rw-rw-   0 root         (0) root         (0)    10192 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/Cnab750/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/api_codes.py
+-rw-rw-rw-   0 root         (0) root         (0)      365 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/D4Sign/
+-rw-rw-rw-   0 root         (0) root         (0)     2600 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/D4Sign/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/DeathByCaptcha/
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/DeathByCaptcha/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/Documents/
+-rw-rw-rw-   0 root         (0) root         (0)     1098 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/Documents/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/Elastic/
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/Elastic/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/ExchangeGraph/
+-rw-rw-rw-   0 root         (0) root         (0)     8987 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/ExchangeGraph/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/FeriadosBancarios/
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/FeriadosBancarios/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/FeriadosBancarios/model.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/IntegracaoSendGrid/
+-rw-rw-rw-   0 root         (0) root         (0)     4251 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/IntegracaoSendGrid/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/ListenerECS/
+-rw-rw-rw-   0 root         (0) root         (0)     4096 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/ListenerECS/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/Mongo/
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/Mongo/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/OracleDB/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/OracleDB/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBot/Vault/
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/Vault/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/PrimeBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)      516 2023-06-08 14:34:16.000000 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-06-08 14:34:16.000000 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-08 14:34:16.000000 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-06-08 14:34:16.000000 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-08 14:34:16.000000 PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-08 14:34:16.746541 PrimeBotFramework-1.0.36/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      928 2023-06-08 14:34:07.000000 PrimeBotFramework-1.0.36/setup.py
```

### Comparing `PrimeBotFramework-1.0.34/PKG-INFO` & `PrimeBotFramework-1.0.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.34
+Version: 1.0.36
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/B2E/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/B2E/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/Cnab750/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/Cnab750/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,101 +116,101 @@
             tipo_arquivo (str): tipo 'remessa' ou tipo 'retorno'
             linha (str): dados da linha
 
         Returns:
             dict: dados do header
         """
         if versao_arquivo == '001' and tipo_arquivo == 'retorno':
-            dict_dados = {'TIPO_DE_REGISTRO':self.extrair_campo(linha, 0, 0),
-                        'CODIGO_DE_RETORNO':self.extrair_campo(linha, 1, 1),
-                        'LITERAL_DE_RETORNO':self.extrair_campo(linha, 2, 9),
-                        'CODIGO_DO_SERVIÇO':self.extrair_campo(linha, 9, 11),
-                        'LITERAL_DE_SERVIÇO':self.extrair_campo(linha, 11, 26),
-                        'ISPB_PARTICIPANTE':self.extrair_campo(linha, 26, 34),
-                        'CODIGO_DE_INSCRIÇAO':self.extrair_campo(linha, 34, 36),
-                        'CPF_CNPJ':self.extrair_campo(linha, 36, 50),
-                        'AGÊNCIA':self.extrair_campo(linha, 50, 54),
-                        'CONTA':self.extrair_campo(linha, 54, 74),
-                        'TIPO_CONTA':self.extrair_campo(linha, 74, 78),
-                        'CHAVE_PIX':self.extrair_campo(linha, 78, 155),
-                        'DATA_DE_GERAÇAO':self.extrair_campo(linha, 155, 163),
-                        'CODIGO_DO_CONVENIO':self.extrair_campo(linha, 163, 193),
-                        'EXCLUSIVO_PSP_RECEBEDOR':self.extrair_campo(linha, 193, 253),
-                        'CODIGOS_DE_ERRO':self.extrair_campo(linha, 253, 283),
-                        'BRANCOS':self.extrair_campo(linha, 283, 741),
-                        'VERSAO_DO_ARQUIVO':self.extrair_campo(linha, 741, 744),
-                        'NUMERO_SEQÜENCIAL_DO_ARQUIVO':self.extrair_campo(linha, 744, 750)}
+            dict_dados = {'tipo_de_registro':self.extrair_campo(linha, 0, 0),
+                        'codigo_de_retorno':self.extrair_campo(linha, 1, 1),
+                        'literal_de_retorno':self.extrair_campo(linha, 2, 9),
+                        'codigo_do_servico':self.extrair_campo(linha, 9, 11),
+                        'literal_de_servico':self.extrair_campo(linha, 11, 26),
+                        'ispb_participante':self.extrair_campo(linha, 26, 34),
+                        'codigo_de_inscricao':self.extrair_campo(linha, 34, 36),
+                        'cpf_cnpj':self.extrair_campo(linha, 36, 50),
+                        'agencia':self.extrair_campo(linha, 50, 54),
+                        'conta':self.extrair_campo(linha, 54, 74),
+                        'tipo_conta':self.extrair_campo(linha, 74, 78),
+                        'chave_pix':self.extrair_campo(linha, 78, 155),
+                        'data_de_geracao':self.extrair_campo(linha, 155, 163),
+                        'codigo_do_convenio':self.extrair_campo(linha, 163, 193),
+                        'exclusivo_psp_recebedor':self.extrair_campo(linha, 193, 253),
+                        'codigos_de_erro':self.extrair_campo(linha, 253, 283),
+                        'brancos':self.extrair_campo(linha, 283, 741),
+                        'versao_do_arquivo':self.extrair_campo(linha, 741, 744),
+                        'numero_sequencial_do_arquivo':self.extrair_campo(linha, 744, 750)}
         return dict_dados
     
     def leitura_detalhe(self, versao_arquivo: str, tipo_arquivo: str, linha: str) -> dict:
         """Efetua a leitura do detalhe
 
         Args:
             versao_arquivo (str): versão do layout CNAB750
             tipo_arquivo (str): tipo 'remessa' ou tipo 'retorno'
             linha (str): dados da linha
 
         Returns:
             dict: dados do detalhe
         """
         if versao_arquivo == '001' and tipo_arquivo == 'retorno':
-            dict_dados = {'TIPO_DE_REGISTRO':self.extrair_campo(linha, 0, 0),
-                        'ISPB_PARTICIPANTE':self.extrair_campo(linha, 1, 9),
-                        'CODIGO_DE_INSCRIÇAO':self.extrair_campo(linha, 9, 11),
-                        'CPF_CNPJ':self.extrair_campo(linha, 11, 25),
-                        'AGÊNCIA':self.extrair_campo(linha, 25, 29),
-                        'CONTA':self.extrair_campo(linha, 29, 49),
-                        'TIPO_CONTA':self.extrair_campo(linha, 49, 53),
-                        'CHAVE_PIX':self.extrair_campo(linha, 53, 130),
-                        'TIPO_COBRANÇA':self.extrair_campo(linha, 130, 130),
-                        'COD._DO_MOVIMENTO':self.extrair_campo(linha, 131, 133),
-                        'DATA_DO_MOVIMENTO':self.extrair_campo(linha, 133, 141),
-                        'IDENTIFICADOR':self.extrair_campo(linha, 141, 176),
-                        'EXPIRAÇAO':self.extrair_campo(linha, 176, 191),
-                        'DATA_DE_VENCIMENTO':self.extrair_campo(linha, 191, 199),
-                        'VALOR ORIGINAL':self.extrair_campo(linha, 199, 216),
-                        'VALOR JUROS':self.extrair_campo(linha, 216, 233),
-                        'VALOR MULTA':self.extrair_campo(linha, 233, 250),
-                        'VALOR_DESCONTO/ABATIMENTO':self.extrair_campo(linha, 250, 267),
-                        'VALOR_FINAL':self.extrair_campo(linha, 267, 284),
-                        'VALOR_PAGO':self.formata_valor(self.extrair_campo(linha, 284, 301), 2),
-                        'TARIFA_DE_COBRANÇA':self.extrair_campo(linha, 301, 318),
-                        'CODIGO_DE_INSCRIÇAO_DEVEDOR':self.extrair_campo(linha, 318, 320),
-                        'CPF_CNPJ_DEVEDOR':self.extrair_campo(linha, 320, 334),
-                        'MENSAGEM_PAGADOR_FINAL':self.extrair_campo(linha, 334, 474),
-                        'CODIGO_DE_INSCRIÇAO_PAGADOR_FINAL':self.extrair_campo(linha, 474, 476),
-                        'CPF_CNPJ_PAGADOR_FINAL':self.extrair_campo(linha, 476, 490),
-                        'NOME_PAGADOR_FINAL':self.extrair_campo(linha, 490, 630),
-                        'COD._DE_LIQUIDAÇAO':self.extrair_campo(linha, 630, 632),
-                        'END_TO_END_ID':self.extrair_campo(linha, 632, 667),
-                        'CODIGOS_DE_ERRO':self.extrair_campo(linha, 667, 697),
-                        'BRANCOS':self.extrair_campo(linha, 697, 744),
-                        'NUMERO_SEQÜENCIAL':self.extrair_campo(linha, 744, 750)}
+            dict_dados = {'tipo_de_registro':self.extrair_campo(linha, 0, 0),
+                        'ispb_participante':self.extrair_campo(linha, 1, 9),
+                        'codigo_de_inscricao':self.extrair_campo(linha, 9, 11),
+                        'cpf_cnpj':self.extrair_campo(linha, 11, 25),
+                        'agencia':self.extrair_campo(linha, 25, 29),
+                        'conta':self.extrair_campo(linha, 29, 49),
+                        'tipo_conta':self.extrair_campo(linha, 49, 53),
+                        'chave_pix':self.extrair_campo(linha, 53, 130),
+                        'tipo_cobranca':self.extrair_campo(linha, 130, 130),
+                        'cod_do_movimento':self.extrair_campo(linha, 131, 133),
+                        'data_do_movimento':self.extrair_campo(linha, 133, 141),
+                        'identificador':self.extrair_campo(linha, 141, 176),
+                        'expiracao':self.extrair_campo(linha, 176, 191),
+                        'data_de_vencimento':self.extrair_campo(linha, 191, 199),
+                        'valor_original':self.extrair_campo(linha, 199, 216),
+                        'valor_juros':self.extrair_campo(linha, 216, 233),
+                        'valor_multa':self.extrair_campo(linha, 233, 250),
+                        'valor_desconto_abatimento':self.extrair_campo(linha, 250, 267),
+                        'valor_final':self.extrair_campo(linha, 267, 284),
+                        'valor_pago':self.formata_valor(self.extrair_campo(linha, 284, 301), 2),
+                        'tarifa_de_cobranca':self.extrair_campo(linha, 301, 318),
+                        'codigo_de_inscricao_devedor':self.extrair_campo(linha, 318, 320),
+                        'cpf_cnpj_devedor':self.extrair_campo(linha, 320, 334),
+                        'mensagem_pagador_final':self.extrair_campo(linha, 334, 474),
+                        'codigo_de_inscricao_pagador_final':self.extrair_campo(linha, 474, 476),
+                        'cpf_cnpj_pagador_final':self.extrair_campo(linha, 476, 490),
+                        'nome_pagador_final':self.extrair_campo(linha, 490, 630),
+                        'cod_de_liquidacao':self.extrair_campo(linha, 630, 632),
+                        'end_to_end_id':self.extrair_campo(linha, 632, 667),
+                        'codigos_de_erro':self.extrair_campo(linha, 667, 697),
+                        'brancos':self.extrair_campo(linha, 697, 744),
+                        'numero_sequencial':self.extrair_campo(linha, 744, 750)}
         return dict_dados
 
     def leitura_trailer(self, versao_arquivo: str, tipo_arquivo: str, linha: str) -> dict:
         """Efetua a leitura do trailer
 
         Args:
             versao_arquivo (str): versão do layout CNAB750
             tipo_arquivo (str): tipo 'remessa' ou tipo 'retorno'
             linha (str): dados da linha
 
         Returns:
             dict: dados do trailer
         """
         if versao_arquivo == '001' and tipo_arquivo == 'retorno':
-            dict_dados = {'TIPO_DE_REGISTRO':self.extrair_campo(linha, 0, 0),
-                        'CODIGO_DE_RETORNO':self.extrair_campo(linha, 1, 1),
-                        'CODIGO_DE_SERVIÇO':self.extrair_campo(linha, 2, 4),
-                        'ISPB':self.extrair_campo(linha, 4, 12),
-                        'CODIGOS_DE_ERRO':self.extrair_campo(linha, 12, 42),
-                        'BRANCOS':self.extrair_campo(linha, 42, 729),
-                        'QTDE_DE_DETALHES':self.extrair_campo(linha, 729, 744),
-                        'NUMERO_SEQÜENCIAL':self.extrair_campo(linha, 745, 750)}
+            dict_dados = {'tipo_de_registro':self.extrair_campo(linha, 0, 0),
+                        'codigo_de_retorno':self.extrair_campo(linha, 1, 1),
+                        'codigo_de_servico':self.extrair_campo(linha, 2, 4),
+                        'ispb':self.extrair_campo(linha, 4, 12),
+                        'codigos_de_erro':self.extrair_campo(linha, 12, 42),
+                        'brancos':self.extrair_campo(linha, 42, 729),
+                        'qtde_de_detalhes':self.extrair_campo(linha, 729, 744),
+                        'numero_sequencial':self.extrair_campo(linha, 745, 750)}
         return dict_dados
     
     def formata_valor(self, valor: str, qtd_decimais: int) -> str:
         """Formata um valor para eliminar os zeros a esquerda e inserir a vírgula para marcação dos decimais.
 
         Args:
             valor (str): valor a ser formatado
```

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/CpfCnpj/api_codes.py` & `PrimeBotFramework-1.0.36/PrimeBot/CpfCnpj/api_codes.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/D4Sign/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/D4Sign/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/DeathByCaptcha/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/DeathByCaptcha/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/Documents/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/Documents/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/Elastic/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/Elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/ExchangeGraph/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/ExchangeGraph/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/FeriadosBancarios/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/FeriadosBancarios/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/IntegracaoSendGrid/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/IntegracaoSendGrid/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/ListenerECS/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/ListenerECS/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/OracleDB/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/OracleDB/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBot/Vault/__init__.py` & `PrimeBotFramework-1.0.36/PrimeBot/Vault/__init__.py`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/PKG-INFO` & `PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrimeBotFramework
-Version: 1.0.34
+Version: 1.0.36
 Summary: Um pacote de padronizacao de pacotes a serem utilizados pela Prime
 Home-page: 
 Author: Prime Control
 Author-email: 
 License: MIT
 Keywords: PrimeBotFramework
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PrimeBotFramework-1.0.34/PrimeBotFramework.egg-info/SOURCES.txt` & `PrimeBotFramework-1.0.36/PrimeBotFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrimeBotFramework-1.0.34/setup.py` & `PrimeBotFramework-1.0.36/setup.py`

 * *Files identical despite different names*

