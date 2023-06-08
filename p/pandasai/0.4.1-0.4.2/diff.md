# Comparing `tmp/pandasai-0.4.1.tar.gz` & `tmp/pandasai-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.4.1.tar", max compression
+gzip compressed data, was "pandasai-0.4.2.tar", max compression
```

## Comparing `pandasai-0.4.1.tar` & `pandasai-0.4.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
--rw-r--r--   0        0        0     1055 2023-06-06 22:10:54.840191 pandasai-0.4.1/LICENSE
--rw-r--r--   0        0        0     8904 2023-06-06 22:10:54.840191 pandasai-0.4.1/README.md
--rw-r--r--   0        0        0    18471 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/__init__.py
--rw-r--r--   0        0        0     1678 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/constants.py
--rw-r--r--   0        0        0     1494 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3774 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5347 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1827 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1487 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3040 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0        0 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4325 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    10698 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1838 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     1481 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     2869 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1220 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      734 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1786 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1333 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1603 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      505 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1414 2023-06-06 22:10:54.848191 pandasai-0.4.1/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     1456 2023-06-06 22:10:54.848191 pandasai-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     9804 1970-01-01 00:00:00.000000 pandasai-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-08 11:05:39.970090 pandasai-0.4.2/LICENSE
+-rw-r--r--   0        0        0     9138 2023-06-08 11:05:39.974090 pandasai-0.4.2/README.md
+-rw-r--r--   0        0        0    18471 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/__init__.py
+-rw-r--r--   0        0        0     1678 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/constants.py
+-rw-r--r--   0        0        0     1494 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3774 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5432 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1827 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1487 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3040 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0        0 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4325 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    10701 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1213 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     1838 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     1482 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     2869 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1220 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      734 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1786 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1333 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1603 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      505 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1414 2023-06-08 11:05:39.978090 pandasai-0.4.2/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     1456 2023-06-08 11:05:39.982090 pandasai-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0    10038 1970-01-01 00:00:00.000000 pandasai-0.4.2/PKG-INFO
```

### Comparing `pandasai-0.4.1/LICENSE` & `pandasai-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/README.md` & `pandasai-0.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 pai [OPTIONS]
 ```
 
 Options:
 
 - **-d, --dataset**: The file path to the dataset.
 - **-t, --token**: Your HuggingFace or OpenAI API token, if no token provided pai will pull from the `.env` file.
-- **-m, --model**: Choice of LLM, either `openai`, `open-assistant`, `starcoder`, or Google `palm`.
+- **-m, --model**: Choice of LLM, either `openai`, `open-assistant`, `starcoder`, `falcon`, `azure-openai` or `google-palm`.
 - **-p, --prompt**: Prompt that PandasAI will run.
 
 To view a full list of available options and their descriptions, run the following command:
 
 ```
 pai --help
 
@@ -201,16 +201,21 @@
 
 ```python
 # OpenAI
 llm = OpenAI(api_token="YOUR_API_KEY")
 
 # Starcoder
 llm = Starcoder(api_token="YOUR_HF_API_KEY")
+
+# Falcon
+llm = Falcon(api_token="YOUR_HF_API_KEY")
 ```
 
+Please note that at the moment OpenAI provides the best results, as the prompts are specifically designed for OpenAI and might hallucinate with other LLMs.
+
 ## License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Contributing
 
 Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
@@ -225,14 +230,14 @@
 ## Acknowledgements
 
 - This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
 - This project is meant to be used as a tool for data exploration and analysis, and it's not meant to be used for production purposes. Please use it responsibly.
 
 ### Todo
 
-- [ ] Add support for more LLMs
+- [x] Add support for more LLMs
 - [x] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
-- [ ] Add unit tests
+- [x] Add unit tests
 - [x] Add contributing guidelines
 - [x] Add CI
 - [x] Add support for conversational responses
```

### Comparing `pandasai-0.4.1/pandasai/__init__.py` & `pandasai-0.4.2/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/constants.py` & `pandasai-0.4.2/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/exceptions.py` & `pandasai-0.4.2/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/helpers/_optional.py` & `pandasai-0.4.2/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/helpers/anonymizer.py` & `pandasai-0.4.2/pandasai/helpers/anonymizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,61 +4,58 @@
  hence the df.head() is processed to remove any personal or sensitive information.
 
 """
 
 import random
 import re
 import string
+
 import pandas as pd
 
 
 def is_valid_email(email: str) -> bool:
-
     """Check if the given email is valid based on regex pattern.
 
     Args:
         email (str): email address to be checked.
 
     Returns (bool): True if the email is valid, otherwise False.
     """
 
     email_regex = r"^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$"
     return re.match(email_regex, email) is not None
 
 
 def is_valid_phone_number(phone_number: str) -> bool:
-
     """Check if the given phone number is valid based on regex pattern.
 
     Args:
         phone_number (str): phone number to be checked.
 
     Returns (bool): True if the phone number is valid, otherwise False.
     """
 
     pattern = r"\b(?:\+?\d{1,3}[- ]?)?\(?\d{3}\)?[- ]?\d{3}[- ]?\d{4}\b"
     return re.search(pattern, phone_number) is not None
 
 
 def is_valid_credit_card(credit_card_number: str) -> bool:
-
     """Check if the given credit card number is valid based on regex pattern.
 
     Args:
         credit_card_number (str): credit card number to be checked.
 
     Returns (str): True if the credit card number is valid, otherwise False.
     """
 
     pattern = r"^\d{4}[- ]?\d{4}[- ]?\d{4}[- ]?\d{4}$"
     return re.search(pattern, credit_card_number) is not None
 
 
 def generate_random_email() -> str:
-
     """Generates a random email address using predefined domains.
 
     Returns (str): generated random email address.
     """
 
     domains = [
         "gmail.com",
@@ -75,15 +72,14 @@
     letters = string.ascii_lowercase + string.digits + "-_"
     username = "".join(random.choice(letters) for i in range(name_length))
     email = username + "@" + domain
     return email
 
 
 def generate_random_phone_number(original_field: str) -> str:
-
     """Generate a random phone number with country code if originally present.
 
     Args:
         original_field (str): original phone number field.
 
     Returns (str): generated random phone number.
     """
@@ -101,45 +97,42 @@
     else:
         phone_number = number
 
     return phone_number
 
 
 def generate_random_credit_card() -> str:
-
     """Generate a random credit card number.
 
     Returns (str): generated random credit card number.
     """
 
     groups = []
     for _i in range(4):
         group = "".join(random.choices("0123456789", k=4))
         groups.append(group)
     separator = random.choice(["-", " "])
     return separator.join(groups)
 
 
 def copy_head(data_frame: pd.DataFrame) -> pd.DataFrame:
-
     """Copy the head of a DataFrame.
 
     Args:
         data_frame (pd.DataFrame): The pd.DataFrame to copy the head from.
 
     Returns (pd.DataFrame): copied head of the DataFrame.
     """
 
     return data_frame.head().copy()
 
 
 def anonymize_dataframe_head(
     data_frame: pd.DataFrame, force_conversion: bool = True
 ) -> pd.DataFrame:
-
     """Anonymize the head of a given DataFrame by replacing sensitive data.
 
     Args:
 
         data_frame (pd.DataFrame):  The DataFrame to anonymize the head data.
         force_conversion (bool): Convert it with instruction. Default is True.
 
@@ -172,11 +165,13 @@
 
             # anonymize data
             random_row_index = random.choice(
                 [i for i in range(len(data_frame.index)) if i != row_idx]
             )
             random_value = data_frame.iloc[random_row_index, col_idx]
             data_frame.iloc[row_idx, col_idx] = random_value
-            data_frame.iloc[random_row_index, col_idx] = cell_value
+            data_frame.iloc[random_row_index, col_idx] = (
+                pd.eval(cell_value) if cell_value in ["True", "False"] else cell_value
+            )
     # restore the original data types
     data_frame = data_frame.astype(dtypes)
     return data_frame
```

### Comparing `pandasai-0.4.1/pandasai/helpers/cache.py` & `pandasai-0.4.2/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/helpers/from_excel.py` & `pandasai-0.4.2/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/helpers/notebook.py` & `pandasai-0.4.2/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/helpers/save_chart.py` & `pandasai-0.4.2/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/llm/azure_openai.py` & `pandasai-0.4.2/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/llm/base.py` & `pandasai-0.4.2/pandasai/llm/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
         raise MethodNotImplementedError("method has not been implemented")
 
     def call(self, instruction: Prompt, value: str, suffix: str = "") -> str:
         """
         Call the Google LLM.
 
         Args:
-            instruction (str): Instruction to pass
+            instruction (object): Instruction to pass
             value (str): Value to pass
             suffix (str): Suffix to pass
 
         Returns:
             str: Response
         """
         self.last_prompt = str(instruction) + str(value)
```

### Comparing `pandasai-0.4.1/pandasai/llm/fake.py` & `pandasai-0.4.2/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/llm/google_palm.py` & `pandasai-0.4.2/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/llm/open_assistant.py` & `pandasai-0.4.2/pandasai/llm/open_assistant.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ Open Assistant LLM
 
 This module is to run the HuggingFace OpenAssistant API hosted and maintained by HuggingFace.co.
 To generate HF_TOKEN go to https://huggingface.co/settings/tokens after creating Account on
 the platform.
 
 Example:
-    Use below example to call Starcoder Model
+    Use below example to call OpenAssistant Model
 
     >>> from pandasai.llm.open_assistant import OpenAssistant
 """
 
 import os
 from typing import Optional
 
@@ -19,27 +19,26 @@
 from .base import HuggingFaceLLM
 
 load_dotenv()
 
 
 class OpenAssistant(HuggingFaceLLM):
     """Open Assistant LLM
-     A base HuggingFaceLLM class is extended to use OpenAssistant Model via its API.
-     Currently `oasst-sft-1-pythia-12b` is supported via this module.
+    A base HuggingFaceLLM class is extended to use OpenAssistant Model via its API.
+    Currently `oasst-sft-1-pythia-12b` is supported via this module.
     """
 
     api_token: str
     _api_url: str = (
         "https://api-inference.huggingface.co/models/"
         "OpenAssistant/oasst-sft-1-pythia-12b"
     )
     _max_retries: int = 10
 
     def __init__(self, api_token: Optional[str] = None):
-
         """
         __init__ method of OpenAssistant Calss
 
         Raises:
             APIKeyNotFoundError: HuggingFace Hub API key is required
 
         Args:
```

### Comparing `pandasai-0.4.1/pandasai/llm/openai.py` & `pandasai-0.4.2/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/llm/starcoder.py` & `pandasai-0.4.2/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/prompts/base.py` & `pandasai-0.4.2/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.4.2/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.4.2/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/prompts/generate_python_code.py` & `pandasai-0.4.2/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.4.2/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.4.1/pyproject.toml` & `pandasai-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.4.1"
+version = "0.4.2"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.4.1/PKG-INFO` & `pandasai-0.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.4.1
+Version: 0.4.2
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -181,15 +181,15 @@
 pai [OPTIONS]
 ```
 
 Options:
 
 - **-d, --dataset**: The file path to the dataset.
 - **-t, --token**: Your HuggingFace or OpenAI API token, if no token provided pai will pull from the `.env` file.
-- **-m, --model**: Choice of LLM, either `openai`, `open-assistant`, `starcoder`, or Google `palm`.
+- **-m, --model**: Choice of LLM, either `openai`, `open-assistant`, `starcoder`, `falcon`, `azure-openai` or `google-palm`.
 - **-p, --prompt**: Prompt that PandasAI will run.
 
 To view a full list of available options and their descriptions, run the following command:
 
 ```
 pai --help
 
@@ -223,16 +223,21 @@
 
 ```python
 # OpenAI
 llm = OpenAI(api_token="YOUR_API_KEY")
 
 # Starcoder
 llm = Starcoder(api_token="YOUR_HF_API_KEY")
+
+# Falcon
+llm = Falcon(api_token="YOUR_HF_API_KEY")
 ```
 
+Please note that at the moment OpenAI provides the best results, as the prompts are specifically designed for OpenAI and might hallucinate with other LLMs.
+
 ## License
 
 PandasAI is licensed under the MIT License. See the LICENSE file for more details.
 
 ## Contributing
 
 Contributions are welcome! Please check out the todos below, and feel free to open a pull request.
@@ -247,15 +252,15 @@
 ## Acknowledgements
 
 - This project is based on the [pandas](https://github.com/pandas-dev/pandas) library by independent contributors, but it's in no way affiliated with the pandas project.
 - This project is meant to be used as a tool for data exploration and analysis, and it's not meant to be used for production purposes. Please use it responsibly.
 
 ### Todo
 
-- [ ] Add support for more LLMs
+- [x] Add support for more LLMs
 - [x] Make PandasAI available from a CLI
 - [ ] Create a web interface for PandasAI
-- [ ] Add unit tests
+- [x] Add unit tests
 - [x] Add contributing guidelines
 - [x] Add CI
 - [x] Add support for conversational responses
```

