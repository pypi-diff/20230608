# Comparing `tmp/kanu-0.4.0.tar.gz` & `tmp/kanu-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kanu-0.4.0.tar", last modified: Fri Jun  2 03:37:51 2023, max compression
+gzip compressed data, was "kanu-0.5.0.tar", last modified: Thu Jun  8 00:32:08 2023, max compression
```

## Comparing `kanu-0.4.0.tar` & `kanu-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-02 03:37:51.877966 kanu-0.4.0/
--rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-06-02 03:37:35.000000 kanu-0.4.0/LICENSE
--rw-r--r--   0 sbslee     (501) staff       (20)      853 2023-06-02 03:37:51.877811 kanu-0.4.0/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      537 2023-06-02 03:37:35.000000 kanu-0.4.0/README.md
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-02 03:37:51.876967 kanu-0.4.0/kanu/
--rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/__init__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     7176 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/__main__.py
--rw-r--r--   0 sbslee     (501) staff       (20)     1959 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/chatgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)     7877 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/docgpt.py
--rw-r--r--   0 sbslee     (501) staff       (20)      844 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/utils.py
--rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-06-02 03:37:35.000000 kanu-0.4.0/kanu/version.py
-drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-02 03:37:51.877624 kanu-0.4.0/kanu.egg-info/
--rw-r--r--   0 sbslee     (501) staff       (20)      853 2023-06-02 03:37:51.000000 kanu-0.4.0/kanu.egg-info/PKG-INFO
--rw-r--r--   0 sbslee     (501) staff       (20)      264 2023-06-02 03:37:51.000000 kanu-0.4.0/kanu.egg-info/SOURCES.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-06-02 03:37:51.000000 kanu-0.4.0/kanu.egg-info/dependency_links.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-06-02 03:37:51.000000 kanu-0.4.0/kanu.egg-info/entry_points.txt
--rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-06-02 03:37:51.000000 kanu-0.4.0/kanu.egg-info/top_level.txt
--rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-06-02 03:37:51.878024 kanu-0.4.0/setup.cfg
--rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-06-02 03:37:35.000000 kanu-0.4.0/setup.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-08 00:32:08.635644 kanu-0.5.0/
+-rw-r--r--   0 sbslee     (501) staff       (20)     1080 2023-06-08 00:31:53.000000 kanu-0.5.0/LICENSE
+-rw-r--r--   0 sbslee     (501) staff       (20)      853 2023-06-08 00:32:08.635495 kanu-0.5.0/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      537 2023-06-08 00:31:53.000000 kanu-0.5.0/README.md
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-08 00:32:08.634660 kanu-0.5.0/kanu/
+-rw-r--r--   0 sbslee     (501) staff       (20)        0 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/__init__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     9960 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/__main__.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     1959 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/chatgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)     8295 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/docgpt.py
+-rw-r--r--   0 sbslee     (501) staff       (20)      844 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/utils.py
+-rw-r--r--   0 sbslee     (501) staff       (20)       21 2023-06-08 00:31:53.000000 kanu-0.5.0/kanu/version.py
+drwxr-xr-x   0 sbslee     (501) staff       (20)        0 2023-06-08 00:32:08.635302 kanu-0.5.0/kanu.egg-info/
+-rw-r--r--   0 sbslee     (501) staff       (20)      853 2023-06-08 00:32:08.000000 kanu-0.5.0/kanu.egg-info/PKG-INFO
+-rw-r--r--   0 sbslee     (501) staff       (20)      264 2023-06-08 00:32:08.000000 kanu-0.5.0/kanu.egg-info/SOURCES.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        1 2023-06-08 00:32:08.000000 kanu-0.5.0/kanu.egg-info/dependency_links.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       44 2023-06-08 00:32:08.000000 kanu-0.5.0/kanu.egg-info/entry_points.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)        5 2023-06-08 00:32:08.000000 kanu-0.5.0/kanu.egg-info/top_level.txt
+-rw-r--r--   0 sbslee     (501) staff       (20)       38 2023-06-08 00:32:08.635702 kanu-0.5.0/setup.cfg
+-rw-r--r--   0 sbslee     (501) staff       (20)      627 2023-06-08 00:31:53.000000 kanu-0.5.0/setup.py
```

### Comparing `kanu-0.4.0/LICENSE` & `kanu-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kanu-0.4.0/README.md` & `kanu-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `kanu-0.4.0/kanu/__main__.py` & `kanu-0.5.0/kanu/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import configparser
 import tkinter as tk
+from tkinter import filedialog
 import importlib.util
 
 from .version import __version__
 from .utils import Tooltip
 
 CHATGPT_PROMPT = """You are a helpful assistant."""
 DOCGPT_PROMPT = """Use the following pieces of context to answer the question at the end. If you don't know the answer, just say that you don't know, don't try to make up an answer.
@@ -13,15 +15,15 @@
 Helpful Answer:"""
 
 class KANU:
     def __init__(self, root):
         self.container = None
         self.root = root
         self.root.title(f"KANU ({__version__})")
-        self.root.geometry("600x500")
+        self.root.geometry("600x620")
         self.homepage()
 
     def homepage(self):
         if self.container is not None:
             self.container.pack_forget()
         self.container = tk.Frame(self.root)
         self.container.pack()
@@ -37,44 +39,64 @@
         self.container = tk.Frame(self.root)
         self.container.pack()
         l = tk.Label(self.container, text="ChatGPT")
         l.grid(row=0, column=0, columnspan=2)
         l = tk.Label(self.container, text="Required packages:")
         l.grid(row=1, column=0, columnspan=2)
         self.display_required_dependency(2, "openai")
+        m = tk.Message(self.container, width=300, text="Option 1. Upload a configuration file")
+        m.grid(row=3, column=0, columnspan=2)
+        b = tk.Button(self.container, text="Browse", command=self.parse_chatgpt_config)
+        b.grid(row=4, column=0)
+        b = tk.Button(self.container, text="Template", command=self.template_chatgpt_config)
+        b.grid(row=4, column=1)
+        m = tk.Message(self.container, width=300, text="Option 2. Configure manually")
+        m.grid(row=5, column=0, columnspan=2)
         self.model = tk.StringVar(self.container, value="gpt-3.5-turbo")
         l = tk.Label(self.container, text="Model:")
-        l.grid(row=3, column=0, columnspan=2)
+        l.grid(row=6, column=0, columnspan=2)
         b = tk.Radiobutton(self.container, variable=self.model, text="gpt-3.5-turbo", value="gpt-3.5-turbo")
-        b.grid(row=4, column=0)
+        b.grid(row=7, column=0)
         b = tk.Radiobutton(self.container, variable=self.model, text="gpt-4", value="gpt-4")
-        b.grid(row=4, column=1)
+        b.grid(row=7, column=1)
         l = tk.Label(self.container, text="System message ⓘ:")
         Tooltip(l, "The system message helps set the behavior of the chatbot.")
-        l.grid(row=5, column=0, columnspan=2)
+        l.grid(row=8, column=0, columnspan=2)
         self.prompt = tk.Text(self.container, height=9, width=42)
         sb = tk.Scrollbar(self.container, command=self.prompt.yview)
         self.prompt.insert("1.0", CHATGPT_PROMPT)
-        self.prompt.grid(row=6, column=0, columnspan=2, sticky="nsew")
-        sb.grid(row=6, column=2, sticky="ns")
+        self.prompt.grid(row=9, column=0, columnspan=2, sticky="nsew")
+        sb.grid(row=9, column=2, sticky="ns")
         self.prompt["yscrollcommand"] = sb.set
         l = tk.Label(self.container, text="Temperature ⓘ:")
         Tooltip(l, "The randomness in generating responses, which ranges between 0 and 1, with 0 indicating almost deterministic behavior.")
-        l.grid(row=7, column=0, columnspan=2)
+        l.grid(row=10, column=0, columnspan=2)
         self.temperature = tk.DoubleVar(self.container, value=0.5)
         e = tk.Entry(self.container, textvariable=self.temperature)
-        e.grid(row=8, column=0, columnspan=2)
+        e.grid(row=11, column=0, columnspan=2)
         l = tk.Label(self.container, text="OpenAI API key:")
-        l.grid(row=9, column=0, columnspan=2)
+        l.grid(row=12, column=0, columnspan=2)
         e = tk.Entry(self.container)
-        e.grid(row=10, column=0, columnspan=2)
+        e.grid(row=13, column=0, columnspan=2)
         b = tk.Button(self.container, text="Submit", command=lambda: self.deploy_agent("ChatGPT", e.get(), self.model.get(), self.temperature.get(), self.prompt.get("1.0", "end-1c")))
-        b.grid(row=11, column=0)
+        b.grid(row=14, column=0)
         b = tk.Button(self.container, text="Go back", command=lambda: self.homepage())
-        b.grid(row=11, column=1)
+        b.grid(row=14, column=1)
+
+    def parse_chatgpt_config(self):
+        config = configparser.ConfigParser()
+        config.read(filedialog.askopenfilename())
+        self.deploy_agent("ChatGPT", config["USER"]["openai_key"], config["DEFAULT"]["model"], float(config["DEFAULT"]["temperature"]), config["DEFAULT"]["prompt"])
+
+    def template_chatgpt_config(self):
+        config = configparser.ConfigParser()
+        config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": CHATGPT_PROMPT}
+        config["USER"] = {"openai_key": ""}
+        with open(filedialog.asksaveasfilename(), "w") as f:
+            config.write(f)
 
     def config_docgpt(self):
         self.container.pack_forget()
         self.container = tk.Frame(self.root)
         self.container.pack()
         l = tk.Label(self.container, text="DocGPT")
         l.grid(row=0, column=0, columnspan=2)
@@ -84,38 +106,64 @@
         self.display_required_dependency(3, "chromadb")
         self.display_required_dependency(4, "tiktoken")
         l = tk.Label(self.container, text="Optional packages:")
         l.grid(row=5, column=0, columnspan=2)        
         self.display_optional_dependency(6, "pdfminer.six", "pdfminer", "Required for .pdf documents.")
         self.display_optional_dependency(7, "unstructured", "unstructured", "Required for .doc and .docx documents.")
         self.display_optional_dependency(8, "tabulate", "tabulate", "Required for .doc and .docx documents.")
+        m = tk.Message(self.container, width=300, text="Option 1. Upload a configuration file")
+        m.grid(row=9, column=0, columnspan=2)
+        b = tk.Button(self.container, text="Browse", command=self.parse_docgpt_config)
+        b.grid(row=10, column=0)
+        b = tk.Button(self.container, text="Template", command=self.template_docgpt_config)
+        b.grid(row=10, column=1)
+        m = tk.Message(self.container, width=300, text="Option 2. Configure manually")
+        m.grid(row=11, column=0, columnspan=2)
         self.model = tk.StringVar(self.container, value="gpt-3.5-turbo")
         l = tk.Label(self.container, text="Model:")
-        l.grid(row=9, column=0, columnspan=2)
+        l.grid(row=12, column=0, columnspan=2)
         rb = tk.Radiobutton(self.container, variable=self.model, text="gpt-3.5-turbo", value="gpt-3.5-turbo")
-        rb.grid(row=10, column=0)
+        rb.grid(row=13, column=0)
         rb = tk.Radiobutton(self.container, variable=self.model, text="gpt-4", value="gpt-4")
-        rb.grid(row=10, column=1)
+        rb.grid(row=13, column=1)
         l = tk.Label(self.container, text="System message ⓘ:")
         Tooltip(l, "The system message helps set the behavior of the chatbot.")
-        l.grid(row=11, column=0, columnspan=3)
+        l.grid(row=14, column=0, columnspan=2)
         self.prompt = tk.Text(self.container, height=9, width=42)
         sb = tk.Scrollbar(self.container, command=self.prompt.yview)
         self.prompt.insert("1.0", DOCGPT_PROMPT)
-        self.prompt.grid(row=12, column=0, columnspan=3, sticky="nsew")
-        sb.grid(row=12, column=3, sticky="ns")
+        self.prompt.grid(row=15, column=0, columnspan=2, sticky="nsew")
+        sb.grid(row=15, column=2, sticky="ns")
         self.prompt["yscrollcommand"] = sb.set
+        l = tk.Label(self.container, text="Temperature ⓘ:")
+        Tooltip(l, "The randomness in generating responses, which ranges between 0 and 1, with 0 indicating almost deterministic behavior.")
+        l.grid(row=16, column=0, columnspan=2)
+        self.temperature = tk.DoubleVar(self.container, value=0.5)
+        e = tk.Entry(self.container, textvariable=self.temperature)
+        e.grid(row=17, column=0, columnspan=2)
         l = tk.Label(self.container, text="OpenAI API key:")
-        l.grid(row=13, column=0, columnspan=2)
+        l.grid(row=18, column=0, columnspan=2)
         e = tk.Entry(self.container)
-        e.grid(row=14, column=0, columnspan=2)
-        b = tk.Button(self.container, text="Submit", command=lambda: self.deploy_agent("DocGPT", e.get(), self.model.get(), self.prompt.get("1.0", "end-1c")))
-        b.grid(row=15, column=0)
+        e.grid(row=19, column=0, columnspan=2)
+        b = tk.Button(self.container, text="Submit", command=lambda: self.deploy_agent("DocGPT", e.get(), self.model.get(), self.prompt.get("1.0", "end-1c"), self.temperature.get()))
+        b.grid(row=20, column=0)
         b = tk.Button(self.container, text="Go back", command=lambda: self.homepage())
-        b.grid(row=15, column=1)
+        b.grid(row=20, column=1)
+
+    def parse_docgpt_config(self):
+        config = configparser.ConfigParser()
+        config.read(filedialog.askopenfilename())
+        self.deploy_agent("DocGPT", config["USER"]["openai_key"], config["DEFAULT"]["model"], float(config["DEFAULT"]["temperature"]), config["DEFAULT"]["prompt"])
+
+    def template_docgpt_config(self):
+        config = configparser.ConfigParser()
+        config["DEFAULT"] = {"model": "gpt-3.5-turbo", "temperature": "0.5", "prompt": DOCGPT_PROMPT}
+        config["USER"] = {"openai_key": ""}
+        with open(filedialog.asksaveasfilename(), "w") as f:
+            config.write(f)
 
     def deploy_agent(self, agent, *args, **kwargs):
         if agent == "ChatGPT":
             from .chatgpt import ChatGPT
             chatgpt = ChatGPT(self, *args, **kwargs)
             chatgpt.run()
         elif agent == "DocGPT":
```

### Comparing `kanu-0.4.0/kanu/chatgpt.py` & `kanu-0.5.0/kanu/chatgpt.py`

 * *Files identical despite different names*

### Comparing `kanu-0.4.0/kanu/docgpt.py` & `kanu-0.5.0/kanu/docgpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,35 +2,38 @@
 import tkinter as tk
 from tkinter import filedialog
 
 from langchain.embeddings.openai import OpenAIEmbeddings
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain.vectorstores import Chroma
 from langchain.chat_models import ChatOpenAI
-from langchain.chains import RetrievalQA
+from langchain.chains import ConversationalRetrievalChain
 from langchain.prompts import PromptTemplate
+from langchain.memory import ConversationBufferMemory
 
 from langchain.document_loaders import (
     TextLoader,
     PDFMinerLoader,
     UnstructuredWordDocumentLoader
 )
 
 from .utils import Tooltip
 
 DOCUMENT_LOADERS = {
-    ".txt": TextLoader,
-    ".pdf": PDFMinerLoader,
-    ".doc": UnstructuredWordDocumentLoader,
-    ".docx": UnstructuredWordDocumentLoader,
+    ".txt": (TextLoader, {"encoding": "utf8"}),
+    ".pdf": (PDFMinerLoader, {}),
+    ".doc": (UnstructuredWordDocumentLoader, {}),
+    ".docx": (UnstructuredWordDocumentLoader, {}),
 }
+
 class DocGPT:
-    def __init__(self, kanu, openai_key, model, prompt):
+    def __init__(self, kanu, openai_key, model, temperature, prompt):
         self.kanu = kanu
         self.model = model
+        self.temperature = temperature
         self.prompt = prompt
         os.environ["OPENAI_API_KEY"] = openai_key
 
     def run(self):
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
@@ -81,20 +84,22 @@
         b = tk.Button(self.kanu.container, text="Browse", command=self.specify_old_database_directory)
         b.grid(row=9, column=2)
         self.option2_button = tk.Button(self.kanu.container, text="Go with Option 2", command=self.go_with_option2)
         self.option2_button.grid(row=10, column=0, columnspan=3)
         self.option2_button["state"] = tk.DISABLED
 
     def query(self):
+        self.memory = ConversationBufferMemory(memory_key="chat_history", return_messages=True)
         self.db = Chroma(persist_directory=self.database_directory, embedding_function=OpenAIEmbeddings())
-        self.qa = RetrievalQA.from_chain_type(
-            llm=ChatOpenAI(model_name=self.model),
-            chain_type="stuff",
+        self.qa = ConversationalRetrievalChain.from_llm(
+            llm=ChatOpenAI(model_name=self.model, temperature=self.temperature),
             retriever=self.db.as_retriever(),
-            chain_type_kwargs={"prompt": PromptTemplate(template=self.prompt, input_variables=["context", "question"])}
+            memory=self.memory,
+            chain_type="stuff",
+            combine_docs_chain_kwargs={"prompt": PromptTemplate(template=self.prompt, input_variables=["context", "question"])}
         )
         self.kanu.container.pack_forget()
         self.kanu.container = tk.Frame(self.kanu.root)
         self.kanu.container.pack()
         l = tk.Label(self.kanu.container, text="DocGPT")
         l.grid(row=0, column=0, columnspan=3)    
         self.session = tk.Text(self.kanu.container, width=70, height=20)
@@ -106,27 +111,28 @@
         b = tk.Button(self.kanu.container, text="Clear", command=lambda: self.clear_session())
         b.grid(row=3, column=1)
         b = tk.Button(self.kanu.container, text="Go back", command=lambda: self.run())
         b.grid(row=3, column=2)
 
     def send_message(self, entry):
         self.session.insert(tk.END, "You: " + entry.get() + "\n")
-        response = self.qa(entry.get())["result"]
+        response = self.qa(entry.get())["answer"]
         self.session.insert(tk.END, "Bot: " + response + "\n")
         entry.delete(0, tk.END)
 
     def go_with_option1(self):
         documents = []
         for root, dirs, files in os.walk(self.document_directory):
             for file in files:
                 file_path = os.path.join(root, file)
                 file_ext = os.path.splitext(file_path)[1]
                 if file_ext not in DOCUMENT_LOADERS:
                     continue
-                loader = DOCUMENT_LOADERS[file_ext](file_path)
+                loader_class, loader_kwargs = DOCUMENT_LOADERS[file_ext]
+                loader = loader_class(file_path, **loader_kwargs)
                 document = loader.load()[0]
                 documents.append(document)
         text_splitter = RecursiveCharacterTextSplitter(chunk_size=self.chunk_size.get(), chunk_overlap=self.chunk_overlap.get())
         texts = text_splitter.split_documents(documents)
         db = Chroma.from_documents(texts, OpenAIEmbeddings(), persist_directory=self.database_directory)
         db.add_documents(texts)    
         db.persist()
```

### Comparing `kanu-0.4.0/kanu/utils.py` & `kanu-0.5.0/kanu/utils.py`

 * *Files identical despite different names*

### Comparing `kanu-0.4.0/setup.py` & `kanu-0.5.0/setup.py`

 * *Files identical despite different names*

