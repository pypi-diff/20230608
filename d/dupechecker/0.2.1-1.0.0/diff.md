# Comparing `tmp/dupechecker-0.2.1.tar.gz` & `tmp/dupechecker-1.0.0.tar.gz`

## Comparing `dupechecker-0.2.1.tar` & `dupechecker-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 dupechecker-0.2.1/CHANGELOG.md
--rw-r--r--   0        0        0    33570 2020-02-02 00:00:00.000000 dupechecker-0.2.1/docs/dupechecker.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dupechecker-0.2.1/docs/index.html
--rw-r--r--   0        0        0    23051 2020-02-02 00:00:00.000000 dupechecker-0.2.1/docs/search.js
--rw-r--r--   0        0        0   110839 2020-02-02 00:00:00.000000 dupechecker-0.2.1/docs/dupechecker/dupechecker.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dupechecker-0.2.1/src/dupechecker/__init__.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 dupechecker-0.2.1/src/dupechecker/dupechecker.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dupechecker-0.2.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dupechecker-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 dupechecker-0.2.1/README.md
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 dupechecker-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 dupechecker-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 dupechecker-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0    34158 2020-02-02 00:00:00.000000 dupechecker-1.0.0/docs/dupechecker.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 dupechecker-1.0.0/docs/index.html
+-rw-r--r--   0        0        0    24923 2020-02-02 00:00:00.000000 dupechecker-1.0.0/docs/search.js
+-rw-r--r--   0        0        0   121350 2020-02-02 00:00:00.000000 dupechecker-1.0.0/docs/dupechecker/dupechecker.html
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 dupechecker-1.0.0/src/dupechecker/__init__.py
+-rw-r--r--   0        0        0     5739 2020-02-02 00:00:00.000000 dupechecker-1.0.0/src/dupechecker/dupechecker.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 dupechecker-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dupechecker-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 dupechecker-1.0.0/README.md
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 dupechecker-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1995 2020-02-02 00:00:00.000000 dupechecker-1.0.0/PKG-INFO
```

### Comparing `dupechecker-0.2.1/docs/dupechecker.html` & `dupechecker-1.0.0/docs/dupechecker.html`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,22 @@
     </nav>
     <main class="pdoc">
             <section class="module-info">
                     <h1 class="modulename">
 dupechecker    </h1>
 
                 
-                
-                
-                
+                        <input id="mod-dupechecker-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+
+                        <label class="view-source-button" for="mod-dupechecker-view-source"><span>View Source</span></label>
+
+                        <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">1</span></a><span class="kn">from</span> <span class="nn">dupechecker.dupechecker</span> <span class="kn">import</span> <span class="n">find_dupes</span><span class="p">,</span> <span class="n">group_by_size</span>
+</span></pre></div>
+
+
             </section>
     </main>
 <script>
     function escapeHTML(html) {
         return document.createElement('div').appendChild(document.createTextNode(html)).parentNode.innerHTML;
     }
```

#### html2text {}

```diff
@@ -3,8 +3,10 @@
   ⁰
 [Unknown INPUT type]
 ***** Submodules *****
     * dupechecker
 built_with_pdoc[pdoc_logo]
 
 ****** dupechecker ******
+⁰ View Source
+1from dupechecker.dupechecker import find_dupes, group_by_size
```

### Comparing `dupechecker-0.2.1/docs/search.js` & `dupechecker-1.0.0/docs/search.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -689,28 +689,28 @@
         "doc": "<p></p>\n"
     }, {
         "fullname": "dupechecker.dupechecker",
         "modulename": "dupechecker.dupechecker",
         "kind": "module",
         "doc": "<p></p>\n"
     }, {
-        "fullname": "dupechecker.dupechecker.get_duplicates",
+        "fullname": "dupechecker.dupechecker.find_dupes",
         "modulename": "dupechecker.dupechecker",
-        "qualname": "get_duplicates",
+        "qualname": "find_dupes",
         "kind": "function",
         "doc": "<p>Return a list of lists for duplicate files in <code>paths</code>.</p>\n",
         "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">paths</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span><span class=\"p\">]]</span>:</span></span>",
         "funcdef": "def"
     }, {
-        "fullname": "dupechecker.dupechecker.get_args",
+        "fullname": "dupechecker.dupechecker.group_by_size",
         "modulename": "dupechecker.dupechecker",
-        "qualname": "get_args",
+        "qualname": "group_by_size",
         "kind": "function",
-        "doc": "<p></p>\n",
-        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span>:</span></span>",
+        "doc": "<p>Returns a list of lists where each sublist is a list of files that have the same size.</p>\n",
+        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">paths</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span><span class=\"p\">]]</span>:</span></span>",
         "funcdef": "def"
     }, {
         "fullname": "dupechecker.dupechecker.delete_wizard",
         "modulename": "dupechecker.dupechecker",
         "qualname": "delete_wizard",
         "kind": "function",
         "doc": "<p>Ask which file to keep for each set.</p>\n",
@@ -726,14 +726,30 @@
         "funcdef": "def"
     }, {
         "fullname": "dupechecker.dupechecker.dupechecker",
         "modulename": "dupechecker.dupechecker",
         "qualname": "dupechecker",
         "kind": "function",
         "doc": "<p></p>\n",
+        "signature": "<span class=\"signature pdoc-code multiline\">(<span class=\"param\">\t<span class=\"n\">paths</span><span class=\"p\">:</span> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span><span class=\"p\">]</span></span><span class=\"return-annotation\">) -> <span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"nb\">list</span><span class=\"p\">[</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">pathier</span><span class=\"o\">.</span><span class=\"n\">Pathier</span><span class=\"p\">]]</span>:</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "dupechecker.dupechecker.get_args",
+        "modulename": "dupechecker.dupechecker",
+        "qualname": "get_args",
+        "kind": "function",
+        "doc": "<p></p>\n",
+        "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"return-annotation\">) -> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span>:</span></span>",
+        "funcdef": "def"
+    }, {
+        "fullname": "dupechecker.dupechecker.main",
+        "modulename": "dupechecker.dupechecker",
+        "qualname": "main",
+        "kind": "function",
+        "doc": "<p></p>\n",
         "signature": "<span class=\"signature pdoc-code condensed\">(<span class=\"param\"><span class=\"n\">args</span><span class=\"p\">:</span> <span class=\"n\">argparse</span><span class=\"o\">.</span><span class=\"n\">Namespace</span> <span class=\"o\">|</span> <span class=\"kc\">None</span> <span class=\"o\">=</span> <span class=\"kc\">None</span></span><span class=\"return-annotation\">):</span></span>",
         "funcdef": "def"
     }];
 
     // mirrored in build-search-index.js (part 1)
     // Also split on html tags. this is a cheap heuristic, but good enough.
     elasticlunr.tokenizer.setSeperator(/[\s\-.;&_'"=,()]+|<[^>]*>/);
```

### Comparing `dupechecker-0.2.1/docs/dupechecker/dupechecker.html` & `dupechecker-1.0.0/docs/dupechecker/dupechecker.html`

 * *Files 4% similar despite different names*

```diff
@@ -27,28 +27,34 @@
                    pattern=".+" required>
 
 
 
         <h2>API Documentation</h2>
             <ul class="memberlist">
             <li>
-                    <a class="function" href="#get_duplicates">get_duplicates</a>
+                    <a class="function" href="#find_dupes">find_dupes</a>
             </li>
             <li>
-                    <a class="function" href="#get_args">get_args</a>
+                    <a class="function" href="#group_by_size">group_by_size</a>
             </li>
             <li>
                     <a class="function" href="#delete_wizard">delete_wizard</a>
             </li>
             <li>
                     <a class="function" href="#autodelete">autodelete</a>
             </li>
             <li>
                     <a class="function" href="#dupechecker">dupechecker</a>
             </li>
+            <li>
+                    <a class="function" href="#get_args">get_args</a>
+            </li>
+            <li>
+                    <a class="function" href="#main">main</a>
+            </li>
     </ul>
 
 
 
         <a class="attribution" title="pdoc: Python API documentation generator" href="https://pdoc.dev" target="_blank">
             built with <span class="visually-hidden">pdoc</span><img
                 alt="pdoc logo"
@@ -69,312 +75,274 @@
                         <div class="pdoc-code codehilite"><pre><span></span><span id="L-1"><a href="#L-1"><span class="linenos">  1</span></a><span class="kn">import</span> <span class="nn">argparse</span>
 </span><span id="L-2"><a href="#L-2"><span class="linenos">  2</span></a><span class="kn">import</span> <span class="nn">filecmp</span>
 </span><span id="L-3"><a href="#L-3"><span class="linenos">  3</span></a><span class="kn">import</span> <span class="nn">time</span>
 </span><span id="L-4"><a href="#L-4"><span class="linenos">  4</span></a><span class="kn">from</span> <span class="nn">concurrent.futures</span> <span class="kn">import</span> <span class="n">ThreadPoolExecutor</span>
 </span><span id="L-5"><a href="#L-5"><span class="linenos">  5</span></a><span class="kn">from</span> <span class="nn">copy</span> <span class="kn">import</span> <span class="n">deepcopy</span>
 </span><span id="L-6"><a href="#L-6"><span class="linenos">  6</span></a>
 </span><span id="L-7"><a href="#L-7"><span class="linenos">  7</span></a><span class="kn">from</span> <span class="nn">griddle</span> <span class="kn">import</span> <span class="n">griddy</span>
-</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
-</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">from</span> <span class="nn">printbuddies</span> <span class="kn">import</span> <span class="n">Spinner</span>
-</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">from</span> <span class="nn">younotyou</span> <span class="kn">import</span> <span class="n">younotyou</span>
-</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a>
+</span><span id="L-8"><a href="#L-8"><span class="linenos">  8</span></a><span class="kn">from</span> <span class="nn">noiftimer</span> <span class="kn">import</span> <span class="n">Timer</span>
+</span><span id="L-9"><a href="#L-9"><span class="linenos">  9</span></a><span class="kn">from</span> <span class="nn">pathier</span> <span class="kn">import</span> <span class="n">Pathier</span>
+</span><span id="L-10"><a href="#L-10"><span class="linenos"> 10</span></a><span class="kn">from</span> <span class="nn">printbuddies</span> <span class="kn">import</span> <span class="n">Spinner</span>
+</span><span id="L-11"><a href="#L-11"><span class="linenos"> 11</span></a><span class="kn">from</span> <span class="nn">younotyou</span> <span class="kn">import</span> <span class="n">younotyou</span>
 </span><span id="L-12"><a href="#L-12"><span class="linenos"> 12</span></a>
-</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a><span class="k">def</span> <span class="nf">get_duplicates</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
-</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a>    <span class="sd">&quot;&quot;&quot;Return a list of lists for duplicate files in `paths`.&quot;&quot;&quot;</span>
-</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="n">matching_sets</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>    <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="n">paths</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>        <span class="n">comparee</span> <span class="o">=</span> <span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>        <span class="n">matching_files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">paths</span> <span class="k">if</span> <span class="n">filecmp</span><span class="o">.</span><span class="n">cmp</span><span class="p">(</span><span class="n">comparee</span><span class="p">,</span> <span class="n">file</span><span class="p">,</span> <span class="kc">False</span><span class="p">)]</span>
-</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>        <span class="k">if</span> <span class="n">matching_files</span><span class="p">:</span>
-</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>            <span class="p">[</span><span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">paths</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">file</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">matching_files</span><span class="p">]</span>
-</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>            <span class="n">matching_files</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">comparee</span><span class="p">)</span>
-</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>            <span class="n">matching_sets</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">matching_files</span><span class="p">)</span>
-</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>    <span class="k">return</span> <span class="n">matching_sets</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>
-</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>
-</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a>
-</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
-</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Glob files to compare recursively. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>    <span class="p">)</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>
-</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>        <span class="s2">&quot;--ignores&quot;</span><span class="p">,</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Ignore files matching these patterns.</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a><span class="s2">        e.g. `dupechecker -i *.wav` will compare all files in the current working directory except .wav files.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="p">)</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>
-</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>        <span class="s2">&quot;--delete_dupes&quot;</span><span class="p">,</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; After finding duplicates, delete all but one copy.</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a><span class="s2">        For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep.</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a><span class="s2">        Pressing &#39;enter&#39; without entering a number will skip that set without deleting anything.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>    <span class="p">)</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>
-</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>        <span class="s2">&quot;-ad&quot;</span><span class="p">,</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>        <span class="s2">&quot;--autodelete&quot;</span><span class="p">,</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Automatically decide which file to keep and which to delete from each set of duplicate files instead of asking which to keep. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="p">)</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>
-</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>        <span class="s2">&quot;-ns&quot;</span><span class="p">,</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>        <span class="s2">&quot;--no_show&quot;</span><span class="p">,</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t show printout of matching files. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="p">)</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="s2">&quot;paths&quot;</span><span class="p">,</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()],</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The paths to compare files in. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>    <span class="p">)</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">==</span> <span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()]:</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Gathering files...&quot;</span><span class="p">)</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>            <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span> <span class="k">else</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="p">)</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">younotyou</span><span class="p">(</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>            <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">],</span> <span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignores</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="p">)</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>    <span class="p">]</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Comparing </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span><span class="si">}</span><span class="s2"> files...&quot;</span><span class="p">)</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="k">return</span> <span class="n">args</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
-</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="p">)</span>
-</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
-</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
-</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
-</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
-</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
-</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>
+</span><span id="L-13"><a href="#L-13"><span class="linenos"> 13</span></a>
+</span><span id="L-14"><a href="#L-14"><span class="linenos"> 14</span></a><span class="k">def</span> <span class="nf">find_dupes</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
+</span><span id="L-15"><a href="#L-15"><span class="linenos"> 15</span></a>    <span class="sd">&quot;&quot;&quot;Return a list of lists for duplicate files in `paths`.&quot;&quot;&quot;</span>
+</span><span id="L-16"><a href="#L-16"><span class="linenos"> 16</span></a>    <span class="n">matching_sets</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-17"><a href="#L-17"><span class="linenos"> 17</span></a>    <span class="n">paths</span> <span class="o">=</span> <span class="n">deepcopy</span><span class="p">(</span><span class="n">paths</span><span class="p">)</span>
+</span><span id="L-18"><a href="#L-18"><span class="linenos"> 18</span></a>    <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="n">paths</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="L-19"><a href="#L-19"><span class="linenos"> 19</span></a>        <span class="n">comparee</span> <span class="o">=</span> <span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="L-20"><a href="#L-20"><span class="linenos"> 20</span></a>        <span class="n">matching_files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">paths</span> <span class="k">if</span> <span class="n">filecmp</span><span class="o">.</span><span class="n">cmp</span><span class="p">(</span><span class="n">comparee</span><span class="p">,</span> <span class="n">file</span><span class="p">,</span> <span class="kc">False</span><span class="p">)]</span>
+</span><span id="L-21"><a href="#L-21"><span class="linenos"> 21</span></a>        <span class="k">if</span> <span class="n">matching_files</span><span class="p">:</span>
+</span><span id="L-22"><a href="#L-22"><span class="linenos"> 22</span></a>            <span class="p">[</span><span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">paths</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">file</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">matching_files</span><span class="p">]</span>
+</span><span id="L-23"><a href="#L-23"><span class="linenos"> 23</span></a>            <span class="n">matching_files</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">comparee</span><span class="p">)</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos"> 24</span></a>            <span class="n">matching_sets</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">matching_files</span><span class="p">)</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos"> 25</span></a>    <span class="k">return</span> <span class="n">matching_sets</span>
+</span><span id="L-26"><a href="#L-26"><span class="linenos"> 26</span></a>
+</span><span id="L-27"><a href="#L-27"><span class="linenos"> 27</span></a>
+</span><span id="L-28"><a href="#L-28"><span class="linenos"> 28</span></a><span class="k">def</span> <span class="nf">group_by_size</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos"> 29</span></a>    <span class="sd">&quot;&quot;&quot;Returns a list of lists where each sublist is a list of files that have the same size.&quot;&quot;&quot;</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos"> 30</span></a>    <span class="n">sizes</span> <span class="o">=</span> <span class="p">{}</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos"> 31</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">paths</span><span class="p">:</span>
+</span><span id="L-32"><a href="#L-32"><span class="linenos"> 32</span></a>        <span class="n">size</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos"> 33</span></a>        <span class="k">if</span> <span class="n">size</span> <span class="ow">in</span> <span class="n">sizes</span><span class="p">:</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos"> 34</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">size</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos"> 35</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos"> 36</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">size</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="p">]</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos"> 37</span></a>    <span class="k">return</span> <span class="nb">list</span><span class="p">(</span><span class="n">sizes</span><span class="o">.</span><span class="n">values</span><span class="p">())</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos"> 38</span></a>
+</span><span id="L-39"><a href="#L-39"><span class="linenos"> 39</span></a>
+</span><span id="L-40"><a href="#L-40"><span class="linenos"> 40</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos"> 41</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos"> 42</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos"> 43</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos"> 44</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos"> 45</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos"> 46</span></a>    <span class="p">)</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos"> 47</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos"> 48</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos"> 49</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos"> 50</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos"> 51</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos"> 52</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos"> 53</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos"> 54</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos"> 55</span></a>        <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos"> 56</span></a>
+</span><span id="L-57"><a href="#L-57"><span class="linenos"> 57</span></a>
+</span><span id="L-58"><a href="#L-58"><span class="linenos"> 58</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos"> 59</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos"> 60</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos"> 61</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>
+</span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
+</span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>    <span class="n">grouped_paths</span> <span class="o">=</span> <span class="n">group_by_size</span><span class="p">(</span><span class="n">paths</span><span class="p">)</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">()</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>            <span class="n">threads</span> <span class="o">=</span> <span class="p">[</span><span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">find_dupes</span><span class="p">,</span> <span class="n">paths</span><span class="p">)</span> <span class="k">for</span> <span class="n">paths</span> <span class="ow">in</span> <span class="n">grouped_paths</span><span class="p">]</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>            <span class="k">while</span> <span class="nb">any</span><span class="p">(</span><span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">()</span> <span class="k">for</span> <span class="n">thread</span> <span class="ow">in</span> <span class="n">threads</span><span class="p">):</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>            <span class="k">for</span> <span class="n">thread</span> <span class="ow">in</span> <span class="n">threads</span><span class="p">:</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>                <span class="n">matches</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">())</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>    <span class="k">return</span> <span class="n">matches</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Glob files to compare recursively. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="p">)</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>        <span class="s2">&quot;--ignores&quot;</span><span class="p">,</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Ignore files matching these patterns.</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a><span class="s2">        e.g. `dupechecker -i *.wav` will compare all files in the current working directory except .wav files.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>    <span class="p">)</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>        <span class="s2">&quot;--delete_dupes&quot;</span><span class="p">,</span>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; After finding duplicates, delete all but one copy.</span>
+</span><span id="L-104"><a href="#L-104"><span class="linenos">104</span></a><span class="s2">        For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep.</span>
+</span><span id="L-105"><a href="#L-105"><span class="linenos">105</span></a><span class="s2">        Pressing &#39;enter&#39; without entering a number will skip that set without deleting anything.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-106"><a href="#L-106"><span class="linenos">106</span></a>    <span class="p">)</span>
+</span><span id="L-107"><a href="#L-107"><span class="linenos">107</span></a>
+</span><span id="L-108"><a href="#L-108"><span class="linenos">108</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-109"><a href="#L-109"><span class="linenos">109</span></a>        <span class="s2">&quot;-ad&quot;</span><span class="p">,</span>
+</span><span id="L-110"><a href="#L-110"><span class="linenos">110</span></a>        <span class="s2">&quot;--autodelete&quot;</span><span class="p">,</span>
+</span><span id="L-111"><a href="#L-111"><span class="linenos">111</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-112"><a href="#L-112"><span class="linenos">112</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Automatically decide which file to keep and which to delete from each set of duplicate files instead of asking which to keep. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-113"><a href="#L-113"><span class="linenos">113</span></a>    <span class="p">)</span>
 </span><span id="L-114"><a href="#L-114"><span class="linenos">114</span></a>
-</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
-</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
-</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>
+</span><span id="L-115"><a href="#L-115"><span class="linenos">115</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-116"><a href="#L-116"><span class="linenos">116</span></a>        <span class="s2">&quot;-ns&quot;</span><span class="p">,</span>
+</span><span id="L-117"><a href="#L-117"><span class="linenos">117</span></a>        <span class="s2">&quot;--no_show&quot;</span><span class="p">,</span>
+</span><span id="L-118"><a href="#L-118"><span class="linenos">118</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-119"><a href="#L-119"><span class="linenos">119</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t show printout of matching files. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-120"><a href="#L-120"><span class="linenos">120</span></a>    <span class="p">)</span>
 </span><span id="L-121"><a href="#L-121"><span class="linenos">121</span></a>
-</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
-</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
-</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
-</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="p">]</span>
-</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
-</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
-</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">deepcopy</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">))</span>
-</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
-</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
-</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
-</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
-</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
-</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
-</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>                <span class="n">griddy</span><span class="p">(</span>
-</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>                    <span class="p">[[</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">])]</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>                <span class="p">)</span>
-</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>            <span class="p">)</span>
-</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
-</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="k">lambda</span><span class="p">:</span> <span class="nb">sum</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>            <span class="n">start_size</span> <span class="o">=</span> <span class="n">size</span><span class="p">()</span>
-</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
-</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">start_size</span> <span class="o">-</span> <span class="n">size</span><span class="p">()</span>
-</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
-</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>
-</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>
-</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>    <span class="n">dupechecker</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
+</span><span id="L-122"><a href="#L-122"><span class="linenos">122</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-123"><a href="#L-123"><span class="linenos">123</span></a>        <span class="s2">&quot;paths&quot;</span><span class="p">,</span>
+</span><span id="L-124"><a href="#L-124"><span class="linenos">124</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-125"><a href="#L-125"><span class="linenos">125</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()],</span>
+</span><span id="L-126"><a href="#L-126"><span class="linenos">126</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="L-127"><a href="#L-127"><span class="linenos">127</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The paths to compare files in. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-128"><a href="#L-128"><span class="linenos">128</span></a>    <span class="p">)</span>
+</span><span id="L-129"><a href="#L-129"><span class="linenos">129</span></a>
+</span><span id="L-130"><a href="#L-130"><span class="linenos">130</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-131"><a href="#L-131"><span class="linenos">131</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">==</span> <span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()]:</span>
+</span><span id="L-132"><a href="#L-132"><span class="linenos">132</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
+</span><span id="L-133"><a href="#L-133"><span class="linenos">133</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="L-134"><a href="#L-134"><span class="linenos">134</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Gathering files...&quot;</span><span class="p">)</span>
+</span><span id="L-135"><a href="#L-135"><span class="linenos">135</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
+</span><span id="L-136"><a href="#L-136"><span class="linenos">136</span></a>        <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="L-137"><a href="#L-137"><span class="linenos">137</span></a>            <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span> <span class="k">else</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
+</span><span id="L-138"><a href="#L-138"><span class="linenos">138</span></a>        <span class="p">)</span>
+</span><span id="L-139"><a href="#L-139"><span class="linenos">139</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-140"><a href="#L-140"><span class="linenos">140</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="L-141"><a href="#L-141"><span class="linenos">141</span></a>        <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">younotyou</span><span class="p">(</span>
+</span><span id="L-142"><a href="#L-142"><span class="linenos">142</span></a>            <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">],</span> <span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignores</span>
+</span><span id="L-143"><a href="#L-143"><span class="linenos">143</span></a>        <span class="p">)</span>
+</span><span id="L-144"><a href="#L-144"><span class="linenos">144</span></a>    <span class="p">]</span>
+</span><span id="L-145"><a href="#L-145"><span class="linenos">145</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Checking </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span><span class="si">}</span><span class="s2"> files...&quot;</span><span class="p">)</span>
+</span><span id="L-146"><a href="#L-146"><span class="linenos">146</span></a>
+</span><span id="L-147"><a href="#L-147"><span class="linenos">147</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-148"><a href="#L-148"><span class="linenos">148</span></a>
+</span><span id="L-149"><a href="#L-149"><span class="linenos">149</span></a>
+</span><span id="L-150"><a href="#L-150"><span class="linenos">150</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="L-151"><a href="#L-151"><span class="linenos">151</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="L-152"><a href="#L-152"><span class="linenos">152</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="L-153"><a href="#L-153"><span class="linenos">153</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-154"><a href="#L-154"><span class="linenos">154</span></a>    <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">()</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="L-155"><a href="#L-155"><span class="linenos">155</span></a>    <span class="n">matches</span> <span class="o">=</span> <span class="n">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>
+</span><span id="L-156"><a href="#L-156"><span class="linenos">156</span></a>    <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="L-157"><a href="#L-157"><span class="linenos">157</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="L-158"><a href="#L-158"><span class="linenos">158</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-159"><a href="#L-159"><span class="linenos">159</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
+</span><span id="L-160"><a href="#L-160"><span class="linenos">160</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-161"><a href="#L-161"><span class="linenos">161</span></a>                <span class="n">griddy</span><span class="p">(</span>
+</span><span id="L-162"><a href="#L-162"><span class="linenos">162</span></a>                    <span class="p">[[</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">])]</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="L-163"><a href="#L-163"><span class="linenos">163</span></a>                <span class="p">)</span>
+</span><span id="L-164"><a href="#L-164"><span class="linenos">164</span></a>            <span class="p">)</span>
+</span><span id="L-165"><a href="#L-165"><span class="linenos">165</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
+</span><span id="L-166"><a href="#L-166"><span class="linenos">166</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="k">lambda</span><span class="p">:</span> <span class="nb">sum</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="L-167"><a href="#L-167"><span class="linenos">167</span></a>            <span class="n">start_size</span> <span class="o">=</span> <span class="n">size</span><span class="p">()</span>
+</span><span id="L-168"><a href="#L-168"><span class="linenos">168</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
+</span><span id="L-169"><a href="#L-169"><span class="linenos">169</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">start_size</span> <span class="o">-</span> <span class="n">size</span><span class="p">()</span>
+</span><span id="L-170"><a href="#L-170"><span class="linenos">170</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="L-171"><a href="#L-171"><span class="linenos">171</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-172"><a href="#L-172"><span class="linenos">172</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
+</span><span id="L-173"><a href="#L-173"><span class="linenos">173</span></a>
+</span><span id="L-174"><a href="#L-174"><span class="linenos">174</span></a>
+</span><span id="L-175"><a href="#L-175"><span class="linenos">175</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-176"><a href="#L-176"><span class="linenos">176</span></a>    <span class="n">main</span><span class="p">(</span><span class="n">get_args</span><span class="p">())</span>
 </span></pre></div>
 
 
             </section>
-                <section id="get_duplicates">
-                            <input id="get_duplicates-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                <section id="find_dupes">
+                            <input id="find_dupes-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">get_duplicates</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span>:</span></span>
+        <span class="name">find_dupes</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span>:</span></span>
 
-                <label class="view-source-button" for="get_duplicates-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="find_dupes-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#get_duplicates"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_duplicates-14"><a href="#get_duplicates-14"><span class="linenos">14</span></a><span class="k">def</span> <span class="nf">get_duplicates</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
-</span><span id="get_duplicates-15"><a href="#get_duplicates-15"><span class="linenos">15</span></a>    <span class="sd">&quot;&quot;&quot;Return a list of lists for duplicate files in `paths`.&quot;&quot;&quot;</span>
-</span><span id="get_duplicates-16"><a href="#get_duplicates-16"><span class="linenos">16</span></a>    <span class="n">matching_sets</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="get_duplicates-17"><a href="#get_duplicates-17"><span class="linenos">17</span></a>    <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="n">paths</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
-</span><span id="get_duplicates-18"><a href="#get_duplicates-18"><span class="linenos">18</span></a>        <span class="n">comparee</span> <span class="o">=</span> <span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="get_duplicates-19"><a href="#get_duplicates-19"><span class="linenos">19</span></a>        <span class="n">matching_files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">paths</span> <span class="k">if</span> <span class="n">filecmp</span><span class="o">.</span><span class="n">cmp</span><span class="p">(</span><span class="n">comparee</span><span class="p">,</span> <span class="n">file</span><span class="p">,</span> <span class="kc">False</span><span class="p">)]</span>
-</span><span id="get_duplicates-20"><a href="#get_duplicates-20"><span class="linenos">20</span></a>        <span class="k">if</span> <span class="n">matching_files</span><span class="p">:</span>
-</span><span id="get_duplicates-21"><a href="#get_duplicates-21"><span class="linenos">21</span></a>            <span class="p">[</span><span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">paths</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">file</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">matching_files</span><span class="p">]</span>
-</span><span id="get_duplicates-22"><a href="#get_duplicates-22"><span class="linenos">22</span></a>            <span class="n">matching_files</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">comparee</span><span class="p">)</span>
-</span><span id="get_duplicates-23"><a href="#get_duplicates-23"><span class="linenos">23</span></a>            <span class="n">matching_sets</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">matching_files</span><span class="p">)</span>
-</span><span id="get_duplicates-24"><a href="#get_duplicates-24"><span class="linenos">24</span></a>    <span class="k">return</span> <span class="n">matching_sets</span>
+    <a class="headerlink" href="#find_dupes"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="find_dupes-15"><a href="#find_dupes-15"><span class="linenos">15</span></a><span class="k">def</span> <span class="nf">find_dupes</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
+</span><span id="find_dupes-16"><a href="#find_dupes-16"><span class="linenos">16</span></a>    <span class="sd">&quot;&quot;&quot;Return a list of lists for duplicate files in `paths`.&quot;&quot;&quot;</span>
+</span><span id="find_dupes-17"><a href="#find_dupes-17"><span class="linenos">17</span></a>    <span class="n">matching_sets</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="find_dupes-18"><a href="#find_dupes-18"><span class="linenos">18</span></a>    <span class="n">paths</span> <span class="o">=</span> <span class="n">deepcopy</span><span class="p">(</span><span class="n">paths</span><span class="p">)</span>
+</span><span id="find_dupes-19"><a href="#find_dupes-19"><span class="linenos">19</span></a>    <span class="k">while</span> <span class="nb">len</span><span class="p">(</span><span class="n">paths</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mi">0</span><span class="p">:</span>
+</span><span id="find_dupes-20"><a href="#find_dupes-20"><span class="linenos">20</span></a>        <span class="n">comparee</span> <span class="o">=</span> <span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="find_dupes-21"><a href="#find_dupes-21"><span class="linenos">21</span></a>        <span class="n">matching_files</span> <span class="o">=</span> <span class="p">[</span><span class="n">file</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">paths</span> <span class="k">if</span> <span class="n">filecmp</span><span class="o">.</span><span class="n">cmp</span><span class="p">(</span><span class="n">comparee</span><span class="p">,</span> <span class="n">file</span><span class="p">,</span> <span class="kc">False</span><span class="p">)]</span>
+</span><span id="find_dupes-22"><a href="#find_dupes-22"><span class="linenos">22</span></a>        <span class="k">if</span> <span class="n">matching_files</span><span class="p">:</span>
+</span><span id="find_dupes-23"><a href="#find_dupes-23"><span class="linenos">23</span></a>            <span class="p">[</span><span class="n">paths</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">paths</span><span class="o">.</span><span class="n">index</span><span class="p">(</span><span class="n">file</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">matching_files</span><span class="p">]</span>
+</span><span id="find_dupes-24"><a href="#find_dupes-24"><span class="linenos">24</span></a>            <span class="n">matching_files</span><span class="o">.</span><span class="n">insert</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">comparee</span><span class="p">)</span>
+</span><span id="find_dupes-25"><a href="#find_dupes-25"><span class="linenos">25</span></a>            <span class="n">matching_sets</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">matching_files</span><span class="p">)</span>
+</span><span id="find_dupes-26"><a href="#find_dupes-26"><span class="linenos">26</span></a>    <span class="k">return</span> <span class="n">matching_sets</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Return a list of lists for duplicate files in <code>paths</code>.</p>
 </div>
 
 
                 </section>
-                <section id="get_args">
-                            <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+                <section id="group_by_size">
+                            <input id="group_by_size-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
+        <span class="name">group_by_size</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span>:</span></span>
 
-                <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
+                <label class="view-source-button" for="group_by_size-view-source"><span>View Source</span></label>
 
     </div>
-    <a class="headerlink" href="#get_args"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-27"><a href="#get_args-27"><span class="linenos">27</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="get_args-28"><a href="#get_args-28"><span class="linenos">28</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="get_args-29"><a href="#get_args-29"><span class="linenos">29</span></a>
-</span><span id="get_args-30"><a href="#get_args-30"><span class="linenos">30</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-31"><a href="#get_args-31"><span class="linenos">31</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
-</span><span id="get_args-32"><a href="#get_args-32"><span class="linenos">32</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
-</span><span id="get_args-33"><a href="#get_args-33"><span class="linenos">33</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-34"><a href="#get_args-34"><span class="linenos">34</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Glob files to compare recursively. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-35"><a href="#get_args-35"><span class="linenos">35</span></a>    <span class="p">)</span>
-</span><span id="get_args-36"><a href="#get_args-36"><span class="linenos">36</span></a>
-</span><span id="get_args-37"><a href="#get_args-37"><span class="linenos">37</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-38"><a href="#get_args-38"><span class="linenos">38</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
-</span><span id="get_args-39"><a href="#get_args-39"><span class="linenos">39</span></a>        <span class="s2">&quot;--ignores&quot;</span><span class="p">,</span>
-</span><span id="get_args-40"><a href="#get_args-40"><span class="linenos">40</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-41"><a href="#get_args-41"><span class="linenos">41</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-42"><a href="#get_args-42"><span class="linenos">42</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
-</span><span id="get_args-43"><a href="#get_args-43"><span class="linenos">43</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Ignore files matching these patterns.</span>
-</span><span id="get_args-44"><a href="#get_args-44"><span class="linenos">44</span></a><span class="s2">        e.g. `dupechecker -i *.wav` will compare all files in the current working directory except .wav files.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-45"><a href="#get_args-45"><span class="linenos">45</span></a>    <span class="p">)</span>
-</span><span id="get_args-46"><a href="#get_args-46"><span class="linenos">46</span></a>
-</span><span id="get_args-47"><a href="#get_args-47"><span class="linenos">47</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-48"><a href="#get_args-48"><span class="linenos">48</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
-</span><span id="get_args-49"><a href="#get_args-49"><span class="linenos">49</span></a>        <span class="s2">&quot;--delete_dupes&quot;</span><span class="p">,</span>
-</span><span id="get_args-50"><a href="#get_args-50"><span class="linenos">50</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-51"><a href="#get_args-51"><span class="linenos">51</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; After finding duplicates, delete all but one copy.</span>
-</span><span id="get_args-52"><a href="#get_args-52"><span class="linenos">52</span></a><span class="s2">        For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep.</span>
-</span><span id="get_args-53"><a href="#get_args-53"><span class="linenos">53</span></a><span class="s2">        Pressing &#39;enter&#39; without entering a number will skip that set without deleting anything.&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-54"><a href="#get_args-54"><span class="linenos">54</span></a>    <span class="p">)</span>
-</span><span id="get_args-55"><a href="#get_args-55"><span class="linenos">55</span></a>
-</span><span id="get_args-56"><a href="#get_args-56"><span class="linenos">56</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-57"><a href="#get_args-57"><span class="linenos">57</span></a>        <span class="s2">&quot;-ad&quot;</span><span class="p">,</span>
-</span><span id="get_args-58"><a href="#get_args-58"><span class="linenos">58</span></a>        <span class="s2">&quot;--autodelete&quot;</span><span class="p">,</span>
-</span><span id="get_args-59"><a href="#get_args-59"><span class="linenos">59</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-60"><a href="#get_args-60"><span class="linenos">60</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Automatically decide which file to keep and which to delete from each set of duplicate files instead of asking which to keep. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-61"><a href="#get_args-61"><span class="linenos">61</span></a>    <span class="p">)</span>
-</span><span id="get_args-62"><a href="#get_args-62"><span class="linenos">62</span></a>
-</span><span id="get_args-63"><a href="#get_args-63"><span class="linenos">63</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-64"><a href="#get_args-64"><span class="linenos">64</span></a>        <span class="s2">&quot;-ns&quot;</span><span class="p">,</span>
-</span><span id="get_args-65"><a href="#get_args-65"><span class="linenos">65</span></a>        <span class="s2">&quot;--no_show&quot;</span><span class="p">,</span>
-</span><span id="get_args-66"><a href="#get_args-66"><span class="linenos">66</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="get_args-67"><a href="#get_args-67"><span class="linenos">67</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t show printout of matching files. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-68"><a href="#get_args-68"><span class="linenos">68</span></a>    <span class="p">)</span>
-</span><span id="get_args-69"><a href="#get_args-69"><span class="linenos">69</span></a>
-</span><span id="get_args-70"><a href="#get_args-70"><span class="linenos">70</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="get_args-71"><a href="#get_args-71"><span class="linenos">71</span></a>        <span class="s2">&quot;paths&quot;</span><span class="p">,</span>
-</span><span id="get_args-72"><a href="#get_args-72"><span class="linenos">72</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="get_args-73"><a href="#get_args-73"><span class="linenos">73</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()],</span>
-</span><span id="get_args-74"><a href="#get_args-74"><span class="linenos">74</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
-</span><span id="get_args-75"><a href="#get_args-75"><span class="linenos">75</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The paths to compare files in. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="get_args-76"><a href="#get_args-76"><span class="linenos">76</span></a>    <span class="p">)</span>
-</span><span id="get_args-77"><a href="#get_args-77"><span class="linenos">77</span></a>
-</span><span id="get_args-78"><a href="#get_args-78"><span class="linenos">78</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="get_args-79"><a href="#get_args-79"><span class="linenos">79</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">==</span> <span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()]:</span>
-</span><span id="get_args-80"><a href="#get_args-80"><span class="linenos">80</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
-</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos">81</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
-</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos">82</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Gathering files...&quot;</span><span class="p">)</span>
-</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos">83</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
-</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos">84</span></a>        <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
-</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos">85</span></a>            <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span> <span class="k">else</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
-</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos">86</span></a>        <span class="p">)</span>
-</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos">87</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos">88</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
-</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos">89</span></a>        <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">younotyou</span><span class="p">(</span>
-</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos">90</span></a>            <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">],</span> <span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignores</span>
-</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos">91</span></a>        <span class="p">)</span>
-</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos">92</span></a>    <span class="p">]</span>
-</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos">93</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Comparing </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span><span class="si">}</span><span class="s2"> files...&quot;</span><span class="p">)</span>
-</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos">94</span></a>
-</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos">95</span></a>    <span class="k">return</span> <span class="n">args</span>
+    <a class="headerlink" href="#group_by_size"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="group_by_size-29"><a href="#group_by_size-29"><span class="linenos">29</span></a><span class="k">def</span> <span class="nf">group_by_size</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
+</span><span id="group_by_size-30"><a href="#group_by_size-30"><span class="linenos">30</span></a>    <span class="sd">&quot;&quot;&quot;Returns a list of lists where each sublist is a list of files that have the same size.&quot;&quot;&quot;</span>
+</span><span id="group_by_size-31"><a href="#group_by_size-31"><span class="linenos">31</span></a>    <span class="n">sizes</span> <span class="o">=</span> <span class="p">{}</span>
+</span><span id="group_by_size-32"><a href="#group_by_size-32"><span class="linenos">32</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">paths</span><span class="p">:</span>
+</span><span id="group_by_size-33"><a href="#group_by_size-33"><span class="linenos">33</span></a>        <span class="n">size</span> <span class="o">=</span> <span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span>
+</span><span id="group_by_size-34"><a href="#group_by_size-34"><span class="linenos">34</span></a>        <span class="k">if</span> <span class="n">size</span> <span class="ow">in</span> <span class="n">sizes</span><span class="p">:</span>
+</span><span id="group_by_size-35"><a href="#group_by_size-35"><span class="linenos">35</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">size</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="group_by_size-36"><a href="#group_by_size-36"><span class="linenos">36</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="group_by_size-37"><a href="#group_by_size-37"><span class="linenos">37</span></a>            <span class="n">sizes</span><span class="p">[</span><span class="n">size</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">path</span><span class="p">]</span>
+</span><span id="group_by_size-38"><a href="#group_by_size-38"><span class="linenos">38</span></a>    <span class="k">return</span> <span class="nb">list</span><span class="p">(</span><span class="n">sizes</span><span class="o">.</span><span class="n">values</span><span class="p">())</span>
 </span></pre></div>
 
 
-    
+            <div class="docstring"><p>Returns a list of lists where each sublist is a list of files that have the same size.</p>
+</div>
+
 
                 </section>
                 <section id="delete_wizard">
                             <input id="delete_wizard-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
         <span class="name">delete_wizard</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="delete_wizard-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#delete_wizard"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_wizard-98"><a href="#delete_wizard-98"><span class="linenos"> 98</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="delete_wizard-99"><a href="#delete_wizard-99"><span class="linenos"> 99</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
-</span><span id="delete_wizard-100"><a href="#delete_wizard-100"><span class="linenos">100</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="delete_wizard-101"><a href="#delete_wizard-101"><span class="linenos">101</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
-</span><span id="delete_wizard-102"><a href="#delete_wizard-102"><span class="linenos">102</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="delete_wizard-103"><a href="#delete_wizard-103"><span class="linenos">103</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
-</span><span id="delete_wizard-104"><a href="#delete_wizard-104"><span class="linenos">104</span></a>    <span class="p">)</span>
-</span><span id="delete_wizard-105"><a href="#delete_wizard-105"><span class="linenos">105</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="delete_wizard-106"><a href="#delete_wizard-106"><span class="linenos">106</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="delete_wizard-107"><a href="#delete_wizard-107"><span class="linenos">107</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
-</span><span id="delete_wizard-108"><a href="#delete_wizard-108"><span class="linenos">108</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
-</span><span id="delete_wizard-109"><a href="#delete_wizard-109"><span class="linenos">109</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
-</span><span id="delete_wizard-110"><a href="#delete_wizard-110"><span class="linenos">110</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
-</span><span id="delete_wizard-111"><a href="#delete_wizard-111"><span class="linenos">111</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
-</span><span id="delete_wizard-112"><a href="#delete_wizard-112"><span class="linenos">112</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
-</span><span id="delete_wizard-113"><a href="#delete_wizard-113"><span class="linenos">113</span></a>        <span class="nb">print</span><span class="p">()</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="delete_wizard-41"><a href="#delete_wizard-41"><span class="linenos">41</span></a><span class="k">def</span> <span class="nf">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="delete_wizard-42"><a href="#delete_wizard-42"><span class="linenos">42</span></a>    <span class="sd">&quot;&quot;&quot;Ask which file to keep for each set.&quot;&quot;&quot;</span>
+</span><span id="delete_wizard-43"><a href="#delete_wizard-43"><span class="linenos">43</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="delete_wizard-44"><a href="#delete_wizard-44"><span class="linenos">44</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Enter the corresponding number of the file to keep.&quot;</span><span class="p">)</span>
+</span><span id="delete_wizard-45"><a href="#delete_wizard-45"><span class="linenos">45</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="delete_wizard-46"><a href="#delete_wizard-46"><span class="linenos">46</span></a>        <span class="s2">&quot;Press &#39;Enter&#39; without giving a number to skip deleting any files for the given set.&quot;</span>
+</span><span id="delete_wizard-47"><a href="#delete_wizard-47"><span class="linenos">47</span></a>    <span class="p">)</span>
+</span><span id="delete_wizard-48"><a href="#delete_wizard-48"><span class="linenos">48</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="delete_wizard-49"><a href="#delete_wizard-49"><span class="linenos">49</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="delete_wizard-50"><a href="#delete_wizard-50"><span class="linenos">50</span></a>        <span class="n">map_</span> <span class="o">=</span> <span class="p">{</span><span class="nb">str</span><span class="p">(</span><span class="n">i</span><span class="p">):</span> <span class="n">file</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">(</span><span class="n">match</span><span class="p">,</span> <span class="mi">1</span><span class="p">)}</span>
+</span><span id="delete_wizard-51"><a href="#delete_wizard-51"><span class="linenos">51</span></a>        <span class="n">options</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;(</span><span class="si">{</span><span class="n">i</span><span class="si">}</span><span class="s2">) </span><span class="si">{</span><span class="n">file</span><span class="si">}</span><span class="s2">&quot;</span> <span class="k">for</span> <span class="n">i</span><span class="p">,</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">map_</span><span class="o">.</span><span class="n">items</span><span class="p">())</span> <span class="o">+</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span>
+</span><span id="delete_wizard-52"><a href="#delete_wizard-52"><span class="linenos">52</span></a>        <span class="nb">print</span><span class="p">(</span><span class="n">options</span><span class="p">)</span>
+</span><span id="delete_wizard-53"><a href="#delete_wizard-53"><span class="linenos">53</span></a>        <span class="n">keeper</span> <span class="o">=</span> <span class="nb">input</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Enter number of file to keep (</span><span class="si">{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="n">map_</span><span class="o">.</span><span class="n">keys</span><span class="p">())</span><span class="si">}</span><span class="s2">): &quot;</span><span class="p">)</span>
+</span><span id="delete_wizard-54"><a href="#delete_wizard-54"><span class="linenos">54</span></a>        <span class="k">if</span> <span class="n">keeper</span><span class="p">:</span>
+</span><span id="delete_wizard-55"><a href="#delete_wizard-55"><span class="linenos">55</span></a>            <span class="p">[</span><span class="n">map_</span><span class="p">[</span><span class="n">num</span><span class="p">]</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">num</span> <span class="ow">in</span> <span class="n">map_</span> <span class="k">if</span> <span class="n">num</span> <span class="o">!=</span> <span class="n">keeper</span><span class="p">]</span>
+</span><span id="delete_wizard-56"><a href="#delete_wizard-56"><span class="linenos">56</span></a>        <span class="nb">print</span><span class="p">()</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Ask which file to keep for each set.</p>
 </div>
 
 
@@ -386,71 +354,176 @@
         <span class="def">def</span>
         <span class="name">autodelete</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span></span><span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="autodelete-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#autodelete"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="autodelete-116"><a href="#autodelete-116"><span class="linenos">116</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
-</span><span id="autodelete-117"><a href="#autodelete-117"><span class="linenos">117</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
-</span><span id="autodelete-118"><a href="#autodelete-118"><span class="linenos">118</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="autodelete-119"><a href="#autodelete-119"><span class="linenos">119</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
-</span><span id="autodelete-120"><a href="#autodelete-120"><span class="linenos">120</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="autodelete-59"><a href="#autodelete-59"><span class="linenos">59</span></a><span class="k">def</span> <span class="nf">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]):</span>
+</span><span id="autodelete-60"><a href="#autodelete-60"><span class="linenos">60</span></a>    <span class="sd">&quot;&quot;&quot;Keep one of each set in `matches` and delete the others.&quot;&quot;&quot;</span>
+</span><span id="autodelete-61"><a href="#autodelete-61"><span class="linenos">61</span></a>    <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="autodelete-62"><a href="#autodelete-62"><span class="linenos">62</span></a>        <span class="k">match</span><span class="o">.</span><span class="n">pop</span><span class="p">()</span>
+</span><span id="autodelete-63"><a href="#autodelete-63"><span class="linenos">63</span></a>        <span class="p">[</span><span class="n">file</span><span class="o">.</span><span class="n">delete</span><span class="p">()</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">]</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Keep one of each set in <code>matches</code> and delete the others.</p>
 </div>
 
 
                 </section>
                 <section id="dupechecker">
                             <input id="dupechecker-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
             
         <span class="def">def</span>
-        <span class="name">dupechecker</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
+        <span class="name">dupechecker</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span><span class="p">]]</span>:</span></span>
 
                 <label class="view-source-button" for="dupechecker-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#dupechecker"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="dupechecker-123"><a href="#dupechecker-123"><span class="linenos">123</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
-</span><span id="dupechecker-124"><a href="#dupechecker-124"><span class="linenos">124</span></a>    <span class="nb">print</span><span class="p">()</span>
-</span><span id="dupechecker-125"><a href="#dupechecker-125"><span class="linenos">125</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
-</span><span id="dupechecker-126"><a href="#dupechecker-126"><span class="linenos">126</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="dupechecker-127"><a href="#dupechecker-127"><span class="linenos">127</span></a>    <span class="n">s</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="dupechecker-128"><a href="#dupechecker-128"><span class="linenos">128</span></a>        <span class="n">ch</span><span class="o">.</span><span class="n">rjust</span><span class="p">(</span><span class="n">i</span> <span class="o">+</span> <span class="n">j</span><span class="p">)</span>
-</span><span id="dupechecker-129"><a href="#dupechecker-129"><span class="linenos">129</span></a>        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">1</span><span class="p">,</span> <span class="mi">25</span><span class="p">,</span> <span class="mi">3</span><span class="p">)</span>
-</span><span id="dupechecker-130"><a href="#dupechecker-130"><span class="linenos">130</span></a>        <span class="k">for</span> <span class="n">j</span><span class="p">,</span> <span class="n">ch</span> <span class="ow">in</span> <span class="nb">enumerate</span><span class="p">([</span><span class="s2">&quot;/&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">,</span> <span class="s2">&quot;</span><span class="se">\\</span><span class="s2">&quot;</span><span class="p">])</span>
-</span><span id="dupechecker-131"><a href="#dupechecker-131"><span class="linenos">131</span></a>    <span class="p">]</span>
-</span><span id="dupechecker-132"><a href="#dupechecker-132"><span class="linenos">132</span></a>    <span class="n">s</span> <span class="o">+=</span> <span class="n">s</span><span class="p">[::</span><span class="o">-</span><span class="mi">1</span><span class="p">]</span>
-</span><span id="dupechecker-133"><a href="#dupechecker-133"><span class="linenos">133</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">(</span><span class="n">s</span><span class="p">)</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
-</span><span id="dupechecker-134"><a href="#dupechecker-134"><span class="linenos">134</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
-</span><span id="dupechecker-135"><a href="#dupechecker-135"><span class="linenos">135</span></a>            <span class="n">thread</span> <span class="o">=</span> <span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">get_duplicates</span><span class="p">,</span> <span class="n">deepcopy</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">))</span>
-</span><span id="dupechecker-136"><a href="#dupechecker-136"><span class="linenos">136</span></a>            <span class="k">while</span> <span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">():</span>
-</span><span id="dupechecker-137"><a href="#dupechecker-137"><span class="linenos">137</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
-</span><span id="dupechecker-138"><a href="#dupechecker-138"><span class="linenos">138</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
-</span><span id="dupechecker-139"><a href="#dupechecker-139"><span class="linenos">139</span></a>            <span class="n">matches</span> <span class="o">=</span> <span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">()</span>
-</span><span id="dupechecker-140"><a href="#dupechecker-140"><span class="linenos">140</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
-</span><span id="dupechecker-141"><a href="#dupechecker-141"><span class="linenos">141</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files.&quot;</span><span class="p">)</span>
-</span><span id="dupechecker-142"><a href="#dupechecker-142"><span class="linenos">142</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
-</span><span id="dupechecker-143"><a href="#dupechecker-143"><span class="linenos">143</span></a>            <span class="nb">print</span><span class="p">(</span>
-</span><span id="dupechecker-144"><a href="#dupechecker-144"><span class="linenos">144</span></a>                <span class="n">griddy</span><span class="p">(</span>
-</span><span id="dupechecker-145"><a href="#dupechecker-145"><span class="linenos">145</span></a>                    <span class="p">[[</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">])]</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
-</span><span id="dupechecker-146"><a href="#dupechecker-146"><span class="linenos">146</span></a>                <span class="p">)</span>
-</span><span id="dupechecker-147"><a href="#dupechecker-147"><span class="linenos">147</span></a>            <span class="p">)</span>
-</span><span id="dupechecker-148"><a href="#dupechecker-148"><span class="linenos">148</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
-</span><span id="dupechecker-149"><a href="#dupechecker-149"><span class="linenos">149</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="k">lambda</span><span class="p">:</span> <span class="nb">sum</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
-</span><span id="dupechecker-150"><a href="#dupechecker-150"><span class="linenos">150</span></a>            <span class="n">start_size</span> <span class="o">=</span> <span class="n">size</span><span class="p">()</span>
-</span><span id="dupechecker-151"><a href="#dupechecker-151"><span class="linenos">151</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
-</span><span id="dupechecker-152"><a href="#dupechecker-152"><span class="linenos">152</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">start_size</span> <span class="o">-</span> <span class="n">size</span><span class="p">()</span>
-</span><span id="dupechecker-153"><a href="#dupechecker-153"><span class="linenos">153</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
-</span><span id="dupechecker-154"><a href="#dupechecker-154"><span class="linenos">154</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="dupechecker-155"><a href="#dupechecker-155"><span class="linenos">155</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="dupechecker-66"><a href="#dupechecker-66"><span class="linenos">66</span></a><span class="k">def</span> <span class="nf">dupechecker</span><span class="p">(</span><span class="n">paths</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">list</span><span class="p">[</span><span class="n">Pathier</span><span class="p">]]:</span>
+</span><span id="dupechecker-67"><a href="#dupechecker-67"><span class="linenos">67</span></a>    <span class="n">grouped_paths</span> <span class="o">=</span> <span class="n">group_by_size</span><span class="p">(</span><span class="n">paths</span><span class="p">)</span>
+</span><span id="dupechecker-68"><a href="#dupechecker-68"><span class="linenos">68</span></a>    <span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="dupechecker-69"><a href="#dupechecker-69"><span class="linenos">69</span></a>    <span class="k">with</span> <span class="n">Spinner</span><span class="p">()</span> <span class="k">as</span> <span class="n">spinner</span><span class="p">:</span>
+</span><span id="dupechecker-70"><a href="#dupechecker-70"><span class="linenos">70</span></a>        <span class="k">with</span> <span class="n">ThreadPoolExecutor</span><span class="p">()</span> <span class="k">as</span> <span class="n">exc</span><span class="p">:</span>
+</span><span id="dupechecker-71"><a href="#dupechecker-71"><span class="linenos">71</span></a>            <span class="n">threads</span> <span class="o">=</span> <span class="p">[</span><span class="n">exc</span><span class="o">.</span><span class="n">submit</span><span class="p">(</span><span class="n">find_dupes</span><span class="p">,</span> <span class="n">paths</span><span class="p">)</span> <span class="k">for</span> <span class="n">paths</span> <span class="ow">in</span> <span class="n">grouped_paths</span><span class="p">]</span>
+</span><span id="dupechecker-72"><a href="#dupechecker-72"><span class="linenos">72</span></a>            <span class="k">while</span> <span class="nb">any</span><span class="p">(</span><span class="ow">not</span> <span class="n">thread</span><span class="o">.</span><span class="n">done</span><span class="p">()</span> <span class="k">for</span> <span class="n">thread</span> <span class="ow">in</span> <span class="n">threads</span><span class="p">):</span>
+</span><span id="dupechecker-73"><a href="#dupechecker-73"><span class="linenos">73</span></a>                <span class="n">spinner</span><span class="o">.</span><span class="n">display</span><span class="p">()</span>
+</span><span id="dupechecker-74"><a href="#dupechecker-74"><span class="linenos">74</span></a>                <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.025</span><span class="p">)</span>
+</span><span id="dupechecker-75"><a href="#dupechecker-75"><span class="linenos">75</span></a>            <span class="k">for</span> <span class="n">thread</span> <span class="ow">in</span> <span class="n">threads</span><span class="p">:</span>
+</span><span id="dupechecker-76"><a href="#dupechecker-76"><span class="linenos">76</span></a>                <span class="n">matches</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span><span class="n">thread</span><span class="o">.</span><span class="n">result</span><span class="p">())</span>
+</span><span id="dupechecker-77"><a href="#dupechecker-77"><span class="linenos">77</span></a>    <span class="k">return</span> <span class="n">matches</span>
+</span></pre></div>
+
+
+    
+
+                </section>
+                <section id="get_args">
+                            <input id="get_args-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">get_args</span><span class="signature pdoc-code condensed">(<span class="return-annotation">) -> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span>:</span></span>
+
+                <label class="view-source-button" for="get_args-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#get_args"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="get_args-80"><a href="#get_args-80"><span class="linenos"> 80</span></a><span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="get_args-81"><a href="#get_args-81"><span class="linenos"> 81</span></a>    <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="get_args-82"><a href="#get_args-82"><span class="linenos"> 82</span></a>
+</span><span id="get_args-83"><a href="#get_args-83"><span class="linenos"> 83</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-84"><a href="#get_args-84"><span class="linenos"> 84</span></a>        <span class="s2">&quot;-r&quot;</span><span class="p">,</span>
+</span><span id="get_args-85"><a href="#get_args-85"><span class="linenos"> 85</span></a>        <span class="s2">&quot;--recursive&quot;</span><span class="p">,</span>
+</span><span id="get_args-86"><a href="#get_args-86"><span class="linenos"> 86</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-87"><a href="#get_args-87"><span class="linenos"> 87</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Glob files to compare recursively. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-88"><a href="#get_args-88"><span class="linenos"> 88</span></a>    <span class="p">)</span>
+</span><span id="get_args-89"><a href="#get_args-89"><span class="linenos"> 89</span></a>
+</span><span id="get_args-90"><a href="#get_args-90"><span class="linenos"> 90</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-91"><a href="#get_args-91"><span class="linenos"> 91</span></a>        <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="get_args-92"><a href="#get_args-92"><span class="linenos"> 92</span></a>        <span class="s2">&quot;--ignores&quot;</span><span class="p">,</span>
+</span><span id="get_args-93"><a href="#get_args-93"><span class="linenos"> 93</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-94"><a href="#get_args-94"><span class="linenos"> 94</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-95"><a href="#get_args-95"><span class="linenos"> 95</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[],</span>
+</span><span id="get_args-96"><a href="#get_args-96"><span class="linenos"> 96</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Ignore files matching these patterns.</span>
+</span><span id="get_args-97"><a href="#get_args-97"><span class="linenos"> 97</span></a><span class="s2">        e.g. `dupechecker -i *.wav` will compare all files in the current working directory except .wav files.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-98"><a href="#get_args-98"><span class="linenos"> 98</span></a>    <span class="p">)</span>
+</span><span id="get_args-99"><a href="#get_args-99"><span class="linenos"> 99</span></a>
+</span><span id="get_args-100"><a href="#get_args-100"><span class="linenos">100</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-101"><a href="#get_args-101"><span class="linenos">101</span></a>        <span class="s2">&quot;-d&quot;</span><span class="p">,</span>
+</span><span id="get_args-102"><a href="#get_args-102"><span class="linenos">102</span></a>        <span class="s2">&quot;--delete_dupes&quot;</span><span class="p">,</span>
+</span><span id="get_args-103"><a href="#get_args-103"><span class="linenos">103</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-104"><a href="#get_args-104"><span class="linenos">104</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; After finding duplicates, delete all but one copy.</span>
+</span><span id="get_args-105"><a href="#get_args-105"><span class="linenos">105</span></a><span class="s2">        For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep.</span>
+</span><span id="get_args-106"><a href="#get_args-106"><span class="linenos">106</span></a><span class="s2">        Pressing &#39;enter&#39; without entering a number will skip that set without deleting anything.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-107"><a href="#get_args-107"><span class="linenos">107</span></a>    <span class="p">)</span>
+</span><span id="get_args-108"><a href="#get_args-108"><span class="linenos">108</span></a>
+</span><span id="get_args-109"><a href="#get_args-109"><span class="linenos">109</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-110"><a href="#get_args-110"><span class="linenos">110</span></a>        <span class="s2">&quot;-ad&quot;</span><span class="p">,</span>
+</span><span id="get_args-111"><a href="#get_args-111"><span class="linenos">111</span></a>        <span class="s2">&quot;--autodelete&quot;</span><span class="p">,</span>
+</span><span id="get_args-112"><a href="#get_args-112"><span class="linenos">112</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-113"><a href="#get_args-113"><span class="linenos">113</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Automatically decide which file to keep and which to delete from each set of duplicate files instead of asking which to keep. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-114"><a href="#get_args-114"><span class="linenos">114</span></a>    <span class="p">)</span>
+</span><span id="get_args-115"><a href="#get_args-115"><span class="linenos">115</span></a>
+</span><span id="get_args-116"><a href="#get_args-116"><span class="linenos">116</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-117"><a href="#get_args-117"><span class="linenos">117</span></a>        <span class="s2">&quot;-ns&quot;</span><span class="p">,</span>
+</span><span id="get_args-118"><a href="#get_args-118"><span class="linenos">118</span></a>        <span class="s2">&quot;--no_show&quot;</span><span class="p">,</span>
+</span><span id="get_args-119"><a href="#get_args-119"><span class="linenos">119</span></a>        <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="get_args-120"><a href="#get_args-120"><span class="linenos">120</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Don&#39;t show printout of matching files. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-121"><a href="#get_args-121"><span class="linenos">121</span></a>    <span class="p">)</span>
+</span><span id="get_args-122"><a href="#get_args-122"><span class="linenos">122</span></a>
+</span><span id="get_args-123"><a href="#get_args-123"><span class="linenos">123</span></a>    <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="get_args-124"><a href="#get_args-124"><span class="linenos">124</span></a>        <span class="s2">&quot;paths&quot;</span><span class="p">,</span>
+</span><span id="get_args-125"><a href="#get_args-125"><span class="linenos">125</span></a>        <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="get_args-126"><a href="#get_args-126"><span class="linenos">126</span></a>        <span class="n">default</span><span class="o">=</span><span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()],</span>
+</span><span id="get_args-127"><a href="#get_args-127"><span class="linenos">127</span></a>        <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;*&quot;</span><span class="p">,</span>
+</span><span id="get_args-128"><a href="#get_args-128"><span class="linenos">128</span></a>        <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The paths to compare files in. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="get_args-129"><a href="#get_args-129"><span class="linenos">129</span></a>    <span class="p">)</span>
+</span><span id="get_args-130"><a href="#get_args-130"><span class="linenos">130</span></a>
+</span><span id="get_args-131"><a href="#get_args-131"><span class="linenos">131</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="get_args-132"><a href="#get_args-132"><span class="linenos">132</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">==</span> <span class="p">[</span><span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()]:</span>
+</span><span id="get_args-133"><a href="#get_args-133"><span class="linenos">133</span></a>        <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span><span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">]</span>
+</span><span id="get_args-134"><a href="#get_args-134"><span class="linenos">134</span></a>    <span class="n">files</span> <span class="o">=</span> <span class="p">[]</span>
+</span><span id="get_args-135"><a href="#get_args-135"><span class="linenos">135</span></a>    <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Gathering files...&quot;</span><span class="p">)</span>
+</span><span id="get_args-136"><a href="#get_args-136"><span class="linenos">136</span></a>    <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">:</span>
+</span><span id="get_args-137"><a href="#get_args-137"><span class="linenos">137</span></a>        <span class="n">files</span><span class="o">.</span><span class="n">extend</span><span class="p">(</span>
+</span><span id="get_args-138"><a href="#get_args-138"><span class="linenos">138</span></a>            <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">recursive</span> <span class="k">else</span> <span class="nb">list</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="s2">&quot;*.*&quot;</span><span class="p">))</span>
+</span><span id="get_args-139"><a href="#get_args-139"><span class="linenos">139</span></a>        <span class="p">)</span>
+</span><span id="get_args-140"><a href="#get_args-140"><span class="linenos">140</span></a>    <span class="n">args</span><span class="o">.</span><span class="n">paths</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="get_args-141"><a href="#get_args-141"><span class="linenos">141</span></a>        <span class="n">Pathier</span><span class="p">(</span><span class="n">path</span><span class="p">)</span>
+</span><span id="get_args-142"><a href="#get_args-142"><span class="linenos">142</span></a>        <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">younotyou</span><span class="p">(</span>
+</span><span id="get_args-143"><a href="#get_args-143"><span class="linenos">143</span></a>            <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">],</span> <span class="n">exclude_patterns</span><span class="o">=</span><span class="n">args</span><span class="o">.</span><span class="n">ignores</span>
+</span><span id="get_args-144"><a href="#get_args-144"><span class="linenos">144</span></a>        <span class="p">)</span>
+</span><span id="get_args-145"><a href="#get_args-145"><span class="linenos">145</span></a>    <span class="p">]</span>
+</span><span id="get_args-146"><a href="#get_args-146"><span class="linenos">146</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Checking </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span><span class="si">}</span><span class="s2"> files...&quot;</span><span class="p">)</span>
+</span><span id="get_args-147"><a href="#get_args-147"><span class="linenos">147</span></a>
+</span><span id="get_args-148"><a href="#get_args-148"><span class="linenos">148</span></a>    <span class="k">return</span> <span class="n">args</span>
+</span></pre></div>
+
+
+    
+
+                </section>
+                <section id="main">
+                            <input id="main-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
+<div class="attr function">
+            
+        <span class="def">def</span>
+        <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span></span><span class="return-annotation">):</span></span>
+
+                <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
+
+    </div>
+    <a class="headerlink" href="#main"></a>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-151"><a href="#main-151"><span class="linenos">151</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">(</span><span class="n">args</span><span class="p">:</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span> <span class="o">|</span> <span class="kc">None</span> <span class="o">=</span> <span class="kc">None</span><span class="p">):</span>
+</span><span id="main-152"><a href="#main-152"><span class="linenos">152</span></a>    <span class="nb">print</span><span class="p">()</span>
+</span><span id="main-153"><a href="#main-153"><span class="linenos">153</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="p">:</span>
+</span><span id="main-154"><a href="#main-154"><span class="linenos">154</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-155"><a href="#main-155"><span class="linenos">155</span></a>    <span class="n">timer</span> <span class="o">=</span> <span class="n">Timer</span><span class="p">()</span><span class="o">.</span><span class="n">start</span><span class="p">()</span>
+</span><span id="main-156"><a href="#main-156"><span class="linenos">156</span></a>    <span class="n">matches</span> <span class="o">=</span> <span class="n">dupechecker</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>
+</span><span id="main-157"><a href="#main-157"><span class="linenos">157</span></a>    <span class="n">timer</span><span class="o">.</span><span class="n">stop</span><span class="p">()</span>
+</span><span id="main-158"><a href="#main-158"><span class="linenos">158</span></a>    <span class="k">if</span> <span class="n">matches</span><span class="p">:</span>
+</span><span id="main-159"><a href="#main-159"><span class="linenos">159</span></a>        <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Found </span><span class="si">{</span><span class="nb">len</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span><span class="si">}</span><span class="s2"> duplicate sets of files in </span><span class="si">{</span><span class="n">timer</span><span class="o">.</span><span class="n">elapsed_str</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="main-160"><a href="#main-160"><span class="linenos">160</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">no_show</span><span class="p">:</span>
+</span><span id="main-161"><a href="#main-161"><span class="linenos">161</span></a>            <span class="nb">print</span><span class="p">(</span>
+</span><span id="main-162"><a href="#main-162"><span class="linenos">162</span></a>                <span class="n">griddy</span><span class="p">(</span>
+</span><span id="main-163"><a href="#main-163"><span class="linenos">163</span></a>                    <span class="p">[[</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">([</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">match</span><span class="p">])]</span> <span class="k">for</span> <span class="n">match</span> <span class="ow">in</span> <span class="n">matches</span><span class="p">]</span>
+</span><span id="main-164"><a href="#main-164"><span class="linenos">164</span></a>                <span class="p">)</span>
+</span><span id="main-165"><a href="#main-165"><span class="linenos">165</span></a>            <span class="p">)</span>
+</span><span id="main-166"><a href="#main-166"><span class="linenos">166</span></a>        <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="ow">or</span> <span class="n">args</span><span class="o">.</span><span class="n">autodelete</span><span class="p">:</span>
+</span><span id="main-167"><a href="#main-167"><span class="linenos">167</span></a>            <span class="n">size</span> <span class="o">=</span> <span class="k">lambda</span><span class="p">:</span> <span class="nb">sum</span><span class="p">(</span><span class="n">path</span><span class="o">.</span><span class="n">size</span><span class="p">()</span> <span class="k">for</span> <span class="n">path</span> <span class="ow">in</span> <span class="n">args</span><span class="o">.</span><span class="n">paths</span><span class="p">)</span>  <span class="c1"># type: ignore</span>
+</span><span id="main-168"><a href="#main-168"><span class="linenos">168</span></a>            <span class="n">start_size</span> <span class="o">=</span> <span class="n">size</span><span class="p">()</span>
+</span><span id="main-169"><a href="#main-169"><span class="linenos">169</span></a>            <span class="n">delete_wizard</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span> <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">delete_dupes</span> <span class="k">else</span> <span class="n">autodelete</span><span class="p">(</span><span class="n">matches</span><span class="p">)</span>
+</span><span id="main-170"><a href="#main-170"><span class="linenos">170</span></a>            <span class="n">deleted_size</span> <span class="o">=</span> <span class="n">start_size</span> <span class="o">-</span> <span class="n">size</span><span class="p">()</span>
+</span><span id="main-171"><a href="#main-171"><span class="linenos">171</span></a>            <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Deleted </span><span class="si">{</span><span class="n">Pathier</span><span class="o">.</span><span class="n">format_size</span><span class="p">(</span><span class="n">deleted_size</span><span class="p">)</span><span class="si">}</span><span class="s2">.&quot;</span><span class="p">)</span>
+</span><span id="main-172"><a href="#main-172"><span class="linenos">172</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="main-173"><a href="#main-173"><span class="linenos">173</span></a>        <span class="nb">print</span><span class="p">(</span><span class="s2">&quot;No duplicates detected.&quot;</span><span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -1,346 +1,395 @@
 
 
   ⁰
 ____ dupechecker [Unknown INPUT type]
 ***** API Documentation *****
-    * get_duplicates
-    * get_args
+    * find_dupes
+    * group_by_size
     * delete_wizard
     * autodelete
     * dupechecker
+    * get_args
+    * main
 built_with_pdoc[pdoc_logo]
 
 ****** dupechecker.dupechecker ******
 ⁰ View Source
 __1import argparse
 __2import filecmp
 __3import time
 __4from concurrent.futures import ThreadPoolExecutor
 __5from copy import deepcopy
 __6
 __7from griddle import griddy
-__8from pathier import Pathier
-__9from printbuddies import Spinner
-_10from younotyou import younotyou
-_11
+__8from noiftimer import Timer
+__9from pathier import Pathier
+_10from printbuddies import Spinner
+_11from younotyou import younotyou
 _12
-_13def get_duplicates(paths: list[Pathier]) -> list[list[Pathier]]:
-_14    """Return a list of lists for duplicate files in `paths`."""
-_15    matching_sets = []
-_16    while len(paths) > 0:
-_17        comparee = paths.pop()
-_18        matching_files = [file for file in paths if filecmp.cmp(comparee,
+_13
+_14def find_dupes(paths: list[Pathier]) -> list[list[Pathier]]:
+_15    """Return a list of lists for duplicate files in `paths`."""
+_16    matching_sets = []
+_17    paths = deepcopy(paths)
+_18    while len(paths) > 0:
+_19        comparee = paths.pop()
+_20        matching_files = [file for file in paths if filecmp.cmp(comparee,
 file, False)]
-_19        if matching_files:
-_20            [paths.pop(paths.index(file)) for file in matching_files]
-_21            matching_files.insert(0, comparee)
-_22            matching_sets.append(matching_files)
-_23    return matching_sets
-_24
-_25
-_26def get_args() -> argparse.Namespace:
-_27    parser = argparse.ArgumentParser()
-_28
-_29    parser.add_argument(
-_30        "-r",
-_31        "--recursive",
-_32        action="store_true",
-_33        help=""" Glob files to compare recursively. """,
-_34    )
-_35
-_36    parser.add_argument(
-_37        "-i",
-_38        "--ignores",
-_39        type=str,
-_40        nargs="*",
-_41        default=[],
-_42        help=""" Ignore files matching these patterns.
-_43        e.g. `dupechecker -i *.wav` will compare all files in the current
+_21        if matching_files:
+_22            [paths.pop(paths.index(file)) for file in matching_files]
+_23            matching_files.insert(0, comparee)
+_24            matching_sets.append(matching_files)
+_25    return matching_sets
+_26
+_27
+_28def group_by_size(paths: list[Pathier]) -> list[list[Pathier]]:
+_29    """Returns a list of lists where each sublist is a list of files that
+have the same size."""
+_30    sizes = {}
+_31    for path in paths:
+_32        size = path.size()
+_33        if size in sizes:
+_34            sizes[size].append(path)
+_35        else:
+_36            sizes[size] = [path]
+_37    return list(sizes.values())
+_38
+_39
+_40def delete_wizard(matches: list[list[Pathier]]):
+_41    """Ask which file to keep for each set."""
+_42    print()
+_43    print("Enter the corresponding number of the file to keep.")
+_44    print(
+_45        "Press 'Enter' without giving a number to skip deleting any files
+for the given set."
+_46    )
+_47    print()
+_48    for match in matches:
+_49        map_ = {str(i): file for i, file in enumerate(match, 1)}
+_50        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
+"\n"
+_51        print(options)
+_52        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
+())}): ")
+_53        if keeper:
+_54            [map_[num].delete() for num in map_ if num != keeper]
+_55        print()
+_56
+_57
+_58def autodelete(matches: list[list[Pathier]]):
+_59    """Keep one of each set in `matches` and delete the others."""
+_60    for match in matches:
+_61        match.pop()
+_62        [file.delete() for file in match]
+_63
+_64
+_65def dupechecker(paths: list[Pathier]) -> list[list[Pathier]]:
+_66    grouped_paths = group_by_size(paths)
+_67    matches = []
+_68    with Spinner() as spinner:
+_69        with ThreadPoolExecutor() as exc:
+_70            threads = [exc.submit(find_dupes, paths) for paths in
+grouped_paths]
+_71            while any(not thread.done() for thread in threads):
+_72                spinner.display()
+_73                time.sleep(0.025)
+_74            for thread in threads:
+_75                matches.extend(thread.result())
+_76    return matches
+_77
+_78
+_79def get_args() -> argparse.Namespace:
+_80    parser = argparse.ArgumentParser()
+_81
+_82    parser.add_argument(
+_83        "-r",
+_84        "--recursive",
+_85        action="store_true",
+_86        help=""" Glob files to compare recursively. """,
+_87    )
+_88
+_89    parser.add_argument(
+_90        "-i",
+_91        "--ignores",
+_92        type=str,
+_93        nargs="*",
+_94        default=[],
+_95        help=""" Ignore files matching these patterns.
+_96        e.g. `dupechecker -i *.wav` will compare all files in the current
 working directory except .wav files.""",
-_44    )
-_45
-_46    parser.add_argument(
-_47        "-d",
-_48        "--delete_dupes",
-_49        action="store_true",
-_50        help=""" After finding duplicates, delete all but one copy.
-_51        For each set of duplicates, the tool will ask you to enter the
+_97    )
+_98
+_99    parser.add_argument(
+100        "-d",
+101        "--delete_dupes",
+102        action="store_true",
+103        help=""" After finding duplicates, delete all but one copy.
+104        For each set of duplicates, the tool will ask you to enter the
 number corresponding to the copy you want to keep.
-_52        Pressing 'enter' without entering a number will skip that set
+105        Pressing 'enter' without entering a number will skip that set
 without deleting anything.""",
-_53    )
-_54
-_55    parser.add_argument(
-_56        "-ad",
-_57        "--autodelete",
-_58        action="store_true",
-_59        help=""" Automatically decide which file to keep and which to delete
+106    )
+107
+108    parser.add_argument(
+109        "-ad",
+110        "--autodelete",
+111        action="store_true",
+112        help=""" Automatically decide which file to keep and which to delete
 from each set of duplicate files instead of asking which to keep. """,
-_60    )
-_61
-_62    parser.add_argument(
-_63        "-ns",
-_64        "--no_show",
-_65        action="store_true",
-_66        help=""" Don't show printout of matching files. """,
-_67    )
-_68
-_69    parser.add_argument(
-_70        "paths",
-_71        type=str,
-_72        default=[Pathier.cwd()],
-_73        nargs="*",
-_74        help=""" The paths to compare files in. """,
-_75    )
-_76
-_77    args = parser.parse_args()
-_78    if not args.paths == [Pathier.cwd()]:
-_79        args.paths = [Pathier(path) for path in args.paths]
-_80    files = []
-_81    print("Gathering files...")
-_82    for path in args.paths:
-_83        files.extend(
-_84            list(path.rglob("*.*")) if args.recursive else list(path.glob
-("*.*"))
-_85        )
-_86    args.paths = [
-_87        Pathier(path)
-_88        for path in younotyou(
-_89            [str(file) for file in files], exclude_patterns=args.ignores
-_90        )
-_91    ]
-_92    print(f"Comparing {len(args.paths)} files...")
-_93
-_94    return args
-_95
-_96
-_97def delete_wizard(matches: list[list[Pathier]]):
-_98    """Ask which file to keep for each set."""
-_99    print()
-100    print("Enter the corresponding number of the file to keep.")
-101    print(
-102        "Press 'Enter' without giving a number to skip deleting any files
-for the given set."
-103    )
-104    print()
-105    for match in matches:
-106        map_ = {str(i): file for i, file in enumerate(match, 1)}
-107        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
-"\n"
-108        print(options)
-109        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
-())}): ")
-110        if keeper:
-111            [map_[num].delete() for num in map_ if num != keeper]
-112        print()
-113
+113    )
 114
-115def autodelete(matches: list[list[Pathier]]):
-116    """Keep one of each set in `matches` and delete the others."""
-117    for match in matches:
-118        match.pop()
-119        [file.delete() for file in match]
-120
+115    parser.add_argument(
+116        "-ns",
+117        "--no_show",
+118        action="store_true",
+119        help=""" Don't show printout of matching files. """,
+120    )
 121
-122def dupechecker(args: argparse.Namespace | None = None):
-123    print()
-124    if not args:
-125        args = get_args()
-126    s = [
-127        ch.rjust(i + j)
-128        for i in range(1, 25, 3)
-129        for j, ch in enumerate(["/", "-", "\\"])
-130    ]
-131    s += s[::-1]
-132    with Spinner(s) as spinner:
-133        with ThreadPoolExecutor() as exc:
-134            thread = exc.submit(get_duplicates, deepcopy(args.paths))
-135            while not thread.done():
-136                spinner.display()
-137                time.sleep(0.025)
-138            matches = thread.result()
-139    if matches:
-140        print(f"Found {len(matches)} duplicate sets of files.")
-141        if not args.no_show:
-142            print(
-143                griddy(
-144                    [["\n".join([str(file) for file in match])] for match in
+122    parser.add_argument(
+123        "paths",
+124        type=str,
+125        default=[Pathier.cwd()],
+126        nargs="*",
+127        help=""" The paths to compare files in. """,
+128    )
+129
+130    args = parser.parse_args()
+131    if not args.paths == [Pathier.cwd()]:
+132        args.paths = [Pathier(path) for path in args.paths]
+133    files = []
+134    print("Gathering files...")
+135    for path in args.paths:
+136        files.extend(
+137            list(path.rglob("*.*")) if args.recursive else list(path.glob
+("*.*"))
+138        )
+139    args.paths = [
+140        Pathier(path)
+141        for path in younotyou(
+142            [str(file) for file in files], exclude_patterns=args.ignores
+143        )
+144    ]
+145    print(f"Checking {len(args.paths)} files...")
+146
+147    return args
+148
+149
+150def main(args: argparse.Namespace | None = None):
+151    print()
+152    if not args:
+153        args = get_args()
+154    timer = Timer().start()
+155    matches = dupechecker(args.paths)
+156    timer.stop()
+157    if matches:
+158        print(f"Found {len(matches)} duplicate sets of files in
+{timer.elapsed_str}.")
+159        if not args.no_show:
+160            print(
+161                griddy(
+162                    [["\n".join([str(file) for file in match])] for match in
 matches]
-145                )
-146            )
-147        if args.delete_dupes or args.autodelete:
-148            size = lambda: sum(path.size() for path in args.paths)  # type:
+163                )
+164            )
+165        if args.delete_dupes or args.autodelete:
+166            size = lambda: sum(path.size() for path in args.paths)  # type:
 ignore
-149            start_size = size()
-150            delete_wizard(matches) if args.delete_dupes else autodelete
+167            start_size = size()
+168            delete_wizard(matches) if args.delete_dupes else autodelete
 (matches)
-151            deleted_size = start_size - size()
-152            print(f"Deleted {Pathier.format_size(deleted_size)}.")
-153    else:
-154        print("No duplicates detected.")
-155
-156
-157if __name__ == "__main__":
-158    dupechecker(get_args())
+169            deleted_size = start_size - size()
+170            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+171    else:
+172        print("No duplicates detected.")
+173
+174
+175if __name__ == "__main__":
+176    main(get_args())
   ⁰
-def get_duplicates(
+def find_dupes(
 paths: list[pathier.pathier.Pathier]) -> list[list[pathier.pathier.Pathier]]:
 View Source
-14def get_duplicates(paths: list[Pathier]) -> list[list[Pathier]]:
-15    """Return a list of lists for duplicate files in `paths`."""
-16    matching_sets = []
-17    while len(paths) > 0:
-18        comparee = paths.pop()
-19        matching_files = [file for file in paths if filecmp.cmp(comparee,
+15def find_dupes(paths: list[Pathier]) -> list[list[Pathier]]:
+16    """Return a list of lists for duplicate files in `paths`."""
+17    matching_sets = []
+18    paths = deepcopy(paths)
+19    while len(paths) > 0:
+20        comparee = paths.pop()
+21        matching_files = [file for file in paths if filecmp.cmp(comparee,
 file, False)]
-20        if matching_files:
-21            [paths.pop(paths.index(file)) for file in matching_files]
-22            matching_files.insert(0, comparee)
-23            matching_sets.append(matching_files)
-24    return matching_sets
+22        if matching_files:
+23            [paths.pop(paths.index(file)) for file in matching_files]
+24            matching_files.insert(0, comparee)
+25            matching_sets.append(matching_files)
+26    return matching_sets
 Return a list of lists for duplicate files in paths.
   ⁰
-def get_args() -> argparse.Namespace: View Source
-27def get_args() -> argparse.Namespace:
-28    parser = argparse.ArgumentParser()
-29
-30    parser.add_argument(
-31        "-r",
-32        "--recursive",
-33        action="store_true",
-34        help=""" Glob files to compare recursively. """,
-35    )
-36
-37    parser.add_argument(
-38        "-i",
-39        "--ignores",
-40        type=str,
-41        nargs="*",
-42        default=[],
-43        help=""" Ignore files matching these patterns.
-44        e.g. `dupechecker -i *.wav` will compare all files in the current
-working directory except .wav files.""",
-45    )
-46
-47    parser.add_argument(
-48        "-d",
-49        "--delete_dupes",
-50        action="store_true",
-51        help=""" After finding duplicates, delete all but one copy.
-52        For each set of duplicates, the tool will ask you to enter the number
-corresponding to the copy you want to keep.
-53        Pressing 'enter' without entering a number will skip that set without
-deleting anything.""",
-54    )
-55
-56    parser.add_argument(
-57        "-ad",
-58        "--autodelete",
-59        action="store_true",
-60        help=""" Automatically decide which file to keep and which to delete
-from each set of duplicate files instead of asking which to keep. """,
-61    )
-62
-63    parser.add_argument(
-64        "-ns",
-65        "--no_show",
-66        action="store_true",
-67        help=""" Don't show printout of matching files. """,
-68    )
-69
-70    parser.add_argument(
-71        "paths",
-72        type=str,
-73        default=[Pathier.cwd()],
-74        nargs="*",
-75        help=""" The paths to compare files in. """,
-76    )
-77
-78    args = parser.parse_args()
-79    if not args.paths == [Pathier.cwd()]:
-80        args.paths = [Pathier(path) for path in args.paths]
-81    files = []
-82    print("Gathering files...")
-83    for path in args.paths:
-84        files.extend(
-85            list(path.rglob("*.*")) if args.recursive else list(path.glob
-("*.*"))
-86        )
-87    args.paths = [
-88        Pathier(path)
-89        for path in younotyou(
-90            [str(file) for file in files], exclude_patterns=args.ignores
-91        )
-92    ]
-93    print(f"Comparing {len(args.paths)} files...")
-94
-95    return args
+def group_by_size(
+paths: list[pathier.pathier.Pathier]) -> list[list[pathier.pathier.Pathier]]:
+View Source
+29def group_by_size(paths: list[Pathier]) -> list[list[Pathier]]:
+30    """Returns a list of lists where each sublist is a list of files that
+have the same size."""
+31    sizes = {}
+32    for path in paths:
+33        size = path.size()
+34        if size in sizes:
+35            sizes[size].append(path)
+36        else:
+37            sizes[size] = [path]
+38    return list(sizes.values())
+Returns a list of lists where each sublist is a list of files that have the
+same size.
   ⁰
 def delete_wizard(matches: list[list[pathier.pathier.Pathier]]): View Source
-_98def delete_wizard(matches: list[list[Pathier]]):
-_99    """Ask which file to keep for each set."""
-100    print()
-101    print("Enter the corresponding number of the file to keep.")
-102    print(
-103        "Press 'Enter' without giving a number to skip deleting any files
-for the given set."
-104    )
-105    print()
-106    for match in matches:
-107        map_ = {str(i): file for i, file in enumerate(match, 1)}
-108        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
+41def delete_wizard(matches: list[list[Pathier]]):
+42    """Ask which file to keep for each set."""
+43    print()
+44    print("Enter the corresponding number of the file to keep.")
+45    print(
+46        "Press 'Enter' without giving a number to skip deleting any files for
+the given set."
+47    )
+48    print()
+49    for match in matches:
+50        map_ = {str(i): file for i, file in enumerate(match, 1)}
+51        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) +
 "\n"
-109        print(options)
-110        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
+52        print(options)
+53        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys
 ())}): ")
-111        if keeper:
-112            [map_[num].delete() for num in map_ if num != keeper]
-113        print()
+54        if keeper:
+55            [map_[num].delete() for num in map_ if num != keeper]
+56        print()
 Ask which file to keep for each set.
   ⁰
 def autodelete(matches: list[list[pathier.pathier.Pathier]]): View Source
-116def autodelete(matches: list[list[Pathier]]):
-117    """Keep one of each set in `matches` and delete the others."""
-118    for match in matches:
-119        match.pop()
-120        [file.delete() for file in match]
+59def autodelete(matches: list[list[Pathier]]):
+60    """Keep one of each set in `matches` and delete the others."""
+61    for match in matches:
+62        match.pop()
+63        [file.delete() for file in match]
 Keep one of each set in matches and delete the others.
   ⁰
-def dupechecker(args: argparse.Namespace | None = None): View Source
-123def dupechecker(args: argparse.Namespace | None = None):
-124    print()
-125    if not args:
-126        args = get_args()
-127    s = [
-128        ch.rjust(i + j)
-129        for i in range(1, 25, 3)
-130        for j, ch in enumerate(["/", "-", "\\"])
-131    ]
-132    s += s[::-1]
-133    with Spinner(s) as spinner:
-134        with ThreadPoolExecutor() as exc:
-135            thread = exc.submit(get_duplicates, deepcopy(args.paths))
-136            while not thread.done():
-137                spinner.display()
-138                time.sleep(0.025)
-139            matches = thread.result()
-140    if matches:
-141        print(f"Found {len(matches)} duplicate sets of files.")
-142        if not args.no_show:
-143            print(
-144                griddy(
-145                    [["\n".join([str(file) for file in match])] for match in
+def dupechecker(
+paths: list[pathier.pathier.Pathier]) -> list[list[pathier.pathier.Pathier]]:
+View Source
+66def dupechecker(paths: list[Pathier]) -> list[list[Pathier]]:
+67    grouped_paths = group_by_size(paths)
+68    matches = []
+69    with Spinner() as spinner:
+70        with ThreadPoolExecutor() as exc:
+71            threads = [exc.submit(find_dupes, paths) for paths in
+grouped_paths]
+72            while any(not thread.done() for thread in threads):
+73                spinner.display()
+74                time.sleep(0.025)
+75            for thread in threads:
+76                matches.extend(thread.result())
+77    return matches
+  ⁰
+def get_args() -> argparse.Namespace: View Source
+_80def get_args() -> argparse.Namespace:
+_81    parser = argparse.ArgumentParser()
+_82
+_83    parser.add_argument(
+_84        "-r",
+_85        "--recursive",
+_86        action="store_true",
+_87        help=""" Glob files to compare recursively. """,
+_88    )
+_89
+_90    parser.add_argument(
+_91        "-i",
+_92        "--ignores",
+_93        type=str,
+_94        nargs="*",
+_95        default=[],
+_96        help=""" Ignore files matching these patterns.
+_97        e.g. `dupechecker -i *.wav` will compare all files in the current
+working directory except .wav files.""",
+_98    )
+_99
+100    parser.add_argument(
+101        "-d",
+102        "--delete_dupes",
+103        action="store_true",
+104        help=""" After finding duplicates, delete all but one copy.
+105        For each set of duplicates, the tool will ask you to enter the
+number corresponding to the copy you want to keep.
+106        Pressing 'enter' without entering a number will skip that set
+without deleting anything.""",
+107    )
+108
+109    parser.add_argument(
+110        "-ad",
+111        "--autodelete",
+112        action="store_true",
+113        help=""" Automatically decide which file to keep and which to delete
+from each set of duplicate files instead of asking which to keep. """,
+114    )
+115
+116    parser.add_argument(
+117        "-ns",
+118        "--no_show",
+119        action="store_true",
+120        help=""" Don't show printout of matching files. """,
+121    )
+122
+123    parser.add_argument(
+124        "paths",
+125        type=str,
+126        default=[Pathier.cwd()],
+127        nargs="*",
+128        help=""" The paths to compare files in. """,
+129    )
+130
+131    args = parser.parse_args()
+132    if not args.paths == [Pathier.cwd()]:
+133        args.paths = [Pathier(path) for path in args.paths]
+134    files = []
+135    print("Gathering files...")
+136    for path in args.paths:
+137        files.extend(
+138            list(path.rglob("*.*")) if args.recursive else list(path.glob
+("*.*"))
+139        )
+140    args.paths = [
+141        Pathier(path)
+142        for path in younotyou(
+143            [str(file) for file in files], exclude_patterns=args.ignores
+144        )
+145    ]
+146    print(f"Checking {len(args.paths)} files...")
+147
+148    return args
+  ⁰
+def main(args: argparse.Namespace | None = None): View Source
+151def main(args: argparse.Namespace | None = None):
+152    print()
+153    if not args:
+154        args = get_args()
+155    timer = Timer().start()
+156    matches = dupechecker(args.paths)
+157    timer.stop()
+158    if matches:
+159        print(f"Found {len(matches)} duplicate sets of files in
+{timer.elapsed_str}.")
+160        if not args.no_show:
+161            print(
+162                griddy(
+163                    [["\n".join([str(file) for file in match])] for match in
 matches]
-146                )
-147            )
-148        if args.delete_dupes or args.autodelete:
-149            size = lambda: sum(path.size() for path in args.paths)  # type:
+164                )
+165            )
+166        if args.delete_dupes or args.autodelete:
+167            size = lambda: sum(path.size() for path in args.paths)  # type:
 ignore
-150            start_size = size()
-151            delete_wizard(matches) if args.delete_dupes else autodelete
+168            start_size = size()
+169            delete_wizard(matches) if args.delete_dupes else autodelete
 (matches)
-152            deleted_size = start_size - size()
-153            print(f"Deleted {Pathier.format_size(deleted_size)}.")
-154    else:
-155        print("No duplicates detected.")
+170            deleted_size = start_size - size()
+171            print(f"Deleted {Pathier.format_size(deleted_size)}.")
+172    else:
+173        print("No duplicates detected.")
```

### Comparing `dupechecker-0.2.1/src/dupechecker/dupechecker.py` & `dupechecker-1.0.0/src/dupechecker/dupechecker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,85 @@
 import argparse
 import filecmp
 import time
 from concurrent.futures import ThreadPoolExecutor
 from copy import deepcopy
 
 from griddle import griddy
+from noiftimer import Timer
 from pathier import Pathier
 from printbuddies import Spinner
 from younotyou import younotyou
 
 
-def get_duplicates(paths: list[Pathier]) -> list[list[Pathier]]:
+def find_dupes(paths: list[Pathier]) -> list[list[Pathier]]:
     """Return a list of lists for duplicate files in `paths`."""
     matching_sets = []
+    paths = deepcopy(paths)
     while len(paths) > 0:
         comparee = paths.pop()
         matching_files = [file for file in paths if filecmp.cmp(comparee, file, False)]
         if matching_files:
             [paths.pop(paths.index(file)) for file in matching_files]
             matching_files.insert(0, comparee)
             matching_sets.append(matching_files)
     return matching_sets
 
 
+def group_by_size(paths: list[Pathier]) -> list[list[Pathier]]:
+    """Returns a list of lists where each sublist is a list of files that have the same size."""
+    sizes = {}
+    for path in paths:
+        size = path.size()
+        if size in sizes:
+            sizes[size].append(path)
+        else:
+            sizes[size] = [path]
+    return list(sizes.values())
+
+
+def delete_wizard(matches: list[list[Pathier]]):
+    """Ask which file to keep for each set."""
+    print()
+    print("Enter the corresponding number of the file to keep.")
+    print(
+        "Press 'Enter' without giving a number to skip deleting any files for the given set."
+    )
+    print()
+    for match in matches:
+        map_ = {str(i): file for i, file in enumerate(match, 1)}
+        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) + "\n"
+        print(options)
+        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys())}): ")
+        if keeper:
+            [map_[num].delete() for num in map_ if num != keeper]
+        print()
+
+
+def autodelete(matches: list[list[Pathier]]):
+    """Keep one of each set in `matches` and delete the others."""
+    for match in matches:
+        match.pop()
+        [file.delete() for file in match]
+
+
+def dupechecker(paths: list[Pathier]) -> list[list[Pathier]]:
+    grouped_paths = group_by_size(paths)
+    matches = []
+    with Spinner() as spinner:
+        with ThreadPoolExecutor() as exc:
+            threads = [exc.submit(find_dupes, paths) for paths in grouped_paths]
+            while any(not thread.done() for thread in threads):
+                spinner.display()
+                time.sleep(0.025)
+            for thread in threads:
+                matches.extend(thread.result())
+    return matches
+
+
 def get_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser()
 
     parser.add_argument(
         "-r",
         "--recursive",
         action="store_true",
@@ -85,63 +138,28 @@
         )
     args.paths = [
         Pathier(path)
         for path in younotyou(
             [str(file) for file in files], exclude_patterns=args.ignores
         )
     ]
-    print(f"Comparing {len(args.paths)} files...")
+    print(f"Checking {len(args.paths)} files...")
 
     return args
 
 
-def delete_wizard(matches: list[list[Pathier]]):
-    """Ask which file to keep for each set."""
-    print()
-    print("Enter the corresponding number of the file to keep.")
-    print(
-        "Press 'Enter' without giving a number to skip deleting any files for the given set."
-    )
-    print()
-    for match in matches:
-        map_ = {str(i): file for i, file in enumerate(match, 1)}
-        options = "\n".join(f"({i}) {file}" for i, file in map_.items()) + "\n"
-        print(options)
-        keeper = input(f"Enter number of file to keep ({', '.join(map_.keys())}): ")
-        if keeper:
-            [map_[num].delete() for num in map_ if num != keeper]
-        print()
-
-
-def autodelete(matches: list[list[Pathier]]):
-    """Keep one of each set in `matches` and delete the others."""
-    for match in matches:
-        match.pop()
-        [file.delete() for file in match]
-
-
-def dupechecker(args: argparse.Namespace | None = None):
+def main(args: argparse.Namespace | None = None):
     print()
     if not args:
         args = get_args()
-    s = [
-        ch.rjust(i + j)
-        for i in range(1, 25, 3)
-        for j, ch in enumerate(["/", "-", "\\"])
-    ]
-    s += s[::-1]
-    with Spinner(s) as spinner:
-        with ThreadPoolExecutor() as exc:
-            thread = exc.submit(get_duplicates, deepcopy(args.paths))
-            while not thread.done():
-                spinner.display()
-                time.sleep(0.025)
-            matches = thread.result()
+    timer = Timer().start()
+    matches = dupechecker(args.paths)
+    timer.stop()
     if matches:
-        print(f"Found {len(matches)} duplicate sets of files.")
+        print(f"Found {len(matches)} duplicate sets of files in {timer.elapsed_str}.")
         if not args.no_show:
             print(
                 griddy(
                     [["\n".join([str(file) for file in match])] for match in matches]
                 )
             )
         if args.delete_dupes or args.autodelete:
@@ -151,8 +169,8 @@
             deleted_size = start_size - size()
             print(f"Deleted {Pathier.format_size(deleted_size)}.")
     else:
         print("No duplicates detected.")
 
 
 if __name__ == "__main__":
-    dupechecker(get_args())
+    main(get_args())
```

### Comparing `dupechecker-0.2.1/LICENSE.txt` & `dupechecker-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dupechecker-0.2.1/pyproject.toml` & `dupechecker-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -6,68 +6,69 @@
 00000050: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000060: 2022 6475 7065 6368 6563 6b65 7222 0d0a   "dupechecker"..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 2243  description = "C
 00000080: 6865 636b 2066 6f72 2061 6e64 2064 656c  heck for and del
 00000090: 6574 6520 6475 706c 6963 6174 6520 6669  ete duplicate fi
 000000a0: 6c65 7320 6672 6f6d 2074 6865 2063 6f6d  les from the com
 000000b0: 6d61 6e64 206c 696e 652e 220d 0a76 6572  mand line."..ver
-000000c0: 7369 6f6e 203d 2022 302e 322e 3122 0d0a  sion = "0.2.1"..
+000000c0: 7369 6f6e 203d 2022 312e 302e 3022 0d0a  sion = "1.0.0"..
 000000d0: 7265 7175 6972 6573 2d70 7974 686f 6e20  requires-python 
 000000e0: 3d20 223e 3d33 2e31 3022 0d0a 6465 7065  = ">=3.10"..depe
 000000f0: 6e64 656e 6369 6573 203d 205b 2267 7269  ndencies = ["gri
 00000100: 6464 6c65 222c 2022 7061 7468 6965 7222  ddle", "pathier"
 00000110: 2c20 2270 7269 6e74 6275 6464 6965 7322  , "printbuddies"
 00000120: 2c20 2270 7974 6573 7422 2c20 2279 6f75  , "pytest", "you
-00000130: 6e6f 7479 6f75 225d 0d0a 7265 6164 6d65  notyou"]..readme
-00000140: 203d 2022 5245 4144 4d45 2e6d 6422 0d0a   = "README.md"..
-00000150: 6b65 7977 6f72 6473 203d 205b 2266 696c  keywords = ["fil
-00000160: 6563 6d70 222c 2022 636c 6922 2c20 2266  ecmp", "cli", "f
-00000170: 696c 6573 7973 7465 6d22 5d0d 0a63 6c61  ilesystem"]..cla
-00000180: 7373 6966 6965 7273 203d 205b 0d0a 2020  ssifiers = [..  
-00000190: 2020 2250 726f 6772 616d 6d69 6e67 204c    "Programming L
-000001a0: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-000001b0: 6e20 3a3a 2033 222c 0d0a 2020 2020 224c  n :: 3",..    "L
-000001c0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
-000001d0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
-000001e0: 6365 6e73 6522 2c0d 0a20 2020 2022 4f70  cense",..    "Op
-000001f0: 6572 6174 696e 6720 5379 7374 656d 203a  erating System :
-00000200: 3a20 4f53 2049 6e64 6570 656e 6465 6e74  : OS Independent
-00000210: 222c 0d0a 2020 2020 5d0d 0a0d 0a5b 5b70  ",..    ]....[[p
-00000220: 726f 6a65 6374 2e61 7574 686f 7273 5d5d  roject.authors]]
-00000230: 0d0a 6e61 6d65 203d 2022 4d61 7474 204d  ..name = "Matt M
-00000240: 616e 6573 220d 0a65 6d61 696c 203d 2022  anes"..email = "
-00000250: 6d61 7474 6d61 6e65 7340 706d 2e6d 6522  mattmanes@pm.me"
-00000260: 0d0a 0d0a 5b70 726f 6a65 6374 2e75 726c  ....[project.url
-00000270: 735d 0d0a 2248 6f6d 6570 6167 6522 203d  s].."Homepage" =
-00000280: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-00000290: 2e63 6f6d 2f6d 6174 742d 6d61 6e65 732f  .com/matt-manes/
-000002a0: 6475 7065 6368 6563 6b65 7222 0d0a 2244  dupechecker".."D
-000002b0: 6f63 756d 656e 7461 7469 6f6e 2220 3d20  ocumentation" = 
-000002c0: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
-000002d0: 636f 6d2f 6d61 7474 2d6d 616e 6573 2f64  com/matt-manes/d
-000002e0: 7570 6563 6865 636b 6572 2f74 7265 652f  upechecker/tree/
-000002f0: 6d61 696e 2f64 6f63 7322 0d0a 2253 6f75  main/docs".."Sou
-00000300: 7263 6520 636f 6465 2220 3d20 2268 7474  rce code" = "htt
-00000310: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000320: 6d61 7474 2d6d 616e 6573 2f64 7570 6563  matt-manes/dupec
-00000330: 6865 636b 6572 2f74 7265 652f 6d61 696e  hecker/tree/main
-00000340: 2f73 7263 2f64 7570 6563 6865 636b 6572  /src/dupechecker
-00000350: 220d 0a0d 0a5b 746f 6f6c 2e70 7974 6573  "....[tool.pytes
-00000360: 742e 696e 695f 6f70 7469 6f6e 735d 0d0a  t.ini_options]..
-00000370: 6164 646f 7074 7320 3d20 5b0d 0a20 2020  addopts = [..   
-00000380: 2022 2d2d 696d 706f 7274 2d6d 6f64 653d   "--import-mode=
-00000390: 696d 706f 7274 6c69 6222 2c0d 0a20 2020  importlib",..   
-000003a0: 205d 0d0a 7079 7468 6f6e 7061 7468 203d   ]..pythonpath =
-000003b0: 2022 7372 6322 0d0a 0d0a 5b74 6f6f 6c2e   "src"....[tool.
-000003c0: 6861 7463 682e 6275 696c 642e 7461 7267  hatch.build.targ
-000003d0: 6574 732e 7364 6973 745d 0d0a 6578 636c  ets.sdist]..excl
-000003e0: 7564 6520 3d20 5b0d 0a20 2020 2022 2e63  ude = [..    ".c
-000003f0: 6f76 6572 6167 6522 2c0d 0a20 2020 2022  overage",..    "
-00000400: 2e70 7974 6573 745f 6361 6368 6522 2c0d  .pytest_cache",.
-00000410: 0a20 2020 2022 2e76 7363 6f64 6522 2c0d  .    ".vscode",.
-00000420: 0a20 2020 2022 7465 7374 7322 2c0d 0a20  .    "tests",.. 
-00000430: 2020 2022 2e67 6974 6967 6e6f 7265 220d     ".gitignore".
-00000440: 0a20 2020 205d 0d0a 5b70 726f 6a65 6374  .    ]..[project
-00000450: 2e73 6372 6970 7473 5d0d 0a64 7570 6563  .scripts]..dupec
-00000460: 6865 636b 6572 203d 2022 6475 7065 6368  hecker = "dupech
-00000470: 6563 6b65 722e 6475 7065 6368 6563 6b65  ecker.dupechecke
-00000480: 723a 6475 7065 6368 6563 6b65 7222 0d0a  r:dupechecker"..
+00000130: 6e6f 7479 6f75 222c 2022 6e6f 6966 7469  notyou", "noifti
+00000140: 6d65 7222 5d0d 0a72 6561 646d 6520 3d20  mer"]..readme = 
+00000150: 2252 4541 444d 452e 6d64 220d 0a6b 6579  "README.md"..key
+00000160: 776f 7264 7320 3d20 5b22 6669 6c65 636d  words = ["filecm
+00000170: 7022 2c20 2263 6c69 222c 2022 6669 6c65  p", "cli", "file
+00000180: 7379 7374 656d 225d 0d0a 636c 6173 7369  system"]..classi
+00000190: 6669 6572 7320 3d20 5b0d 0a20 2020 2022  fiers = [..    "
+000001a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000001b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+000001c0: 3a20 3322 2c0d 0a20 2020 2022 4c69 6365  : 3",..    "Lice
+000001d0: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+000001e0: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+000001f0: 7365 222c 0d0a 2020 2020 224f 7065 7261  se",..    "Opera
+00000200: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
+00000210: 5320 496e 6465 7065 6e64 656e 7422 2c0d  S Independent",.
+00000220: 0a20 2020 205d 0d0a 0d0a 5b5b 7072 6f6a  .    ]....[[proj
+00000230: 6563 742e 6175 7468 6f72 735d 5d0d 0a6e  ect.authors]]..n
+00000240: 616d 6520 3d20 224d 6174 7420 4d61 6e65  ame = "Matt Mane
+00000250: 7322 0d0a 656d 6169 6c20 3d20 226d 6174  s"..email = "mat
+00000260: 746d 616e 6573 4070 6d2e 6d65 220d 0a0d  tmanes@pm.me"...
+00000270: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
+00000280: 0a22 486f 6d65 7061 6765 2220 3d20 2268  ."Homepage" = "h
+00000290: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000002a0: 6d2f 6d61 7474 2d6d 616e 6573 2f64 7570  m/matt-manes/dup
+000002b0: 6563 6865 636b 6572 220d 0a22 446f 6375  echecker".."Docu
+000002c0: 6d65 6e74 6174 696f 6e22 203d 2022 6874  mentation" = "ht
+000002d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000002e0: 2f6d 6174 742d 6d61 6e65 732f 6475 7065  /matt-manes/dupe
+000002f0: 6368 6563 6b65 722f 7472 6565 2f6d 6169  checker/tree/mai
+00000300: 6e2f 646f 6373 220d 0a22 536f 7572 6365  n/docs".."Source
+00000310: 2063 6f64 6522 203d 2022 6874 7470 733a   code" = "https:
+00000320: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 6174  //github.com/mat
+00000330: 742d 6d61 6e65 732f 6475 7065 6368 6563  t-manes/dupechec
+00000340: 6b65 722f 7472 6565 2f6d 6169 6e2f 7372  ker/tree/main/sr
+00000350: 632f 6475 7065 6368 6563 6b65 7222 0d0a  c/dupechecker"..
+00000360: 0d0a 5b74 6f6f 6c2e 7079 7465 7374 2e69  ..[tool.pytest.i
+00000370: 6e69 5f6f 7074 696f 6e73 5d0d 0a61 6464  ni_options]..add
+00000380: 6f70 7473 203d 205b 0d0a 2020 2020 222d  opts = [..    "-
+00000390: 2d69 6d70 6f72 742d 6d6f 6465 3d69 6d70  -import-mode=imp
+000003a0: 6f72 746c 6962 222c 0d0a 2020 2020 5d0d  ortlib",..    ].
+000003b0: 0a70 7974 686f 6e70 6174 6820 3d20 2273  .pythonpath = "s
+000003c0: 7263 220d 0a0d 0a5b 746f 6f6c 2e68 6174  rc"....[tool.hat
+000003d0: 6368 2e62 7569 6c64 2e74 6172 6765 7473  ch.build.targets
+000003e0: 2e73 6469 7374 5d0d 0a65 7863 6c75 6465  .sdist]..exclude
+000003f0: 203d 205b 0d0a 2020 2020 222e 636f 7665   = [..    ".cove
+00000400: 7261 6765 222c 0d0a 2020 2020 222e 7079  rage",..    ".py
+00000410: 7465 7374 5f63 6163 6865 222c 0d0a 2020  test_cache",..  
+00000420: 2020 222e 7673 636f 6465 222c 0d0a 2020    ".vscode",..  
+00000430: 2020 2274 6573 7473 222c 0d0a 2020 2020    "tests",..    
+00000440: 222e 6769 7469 676e 6f72 6522 0d0a 2020  ".gitignore"..  
+00000450: 2020 5d0d 0a5b 7072 6f6a 6563 742e 7363    ]..[project.sc
+00000460: 7269 7074 735d 0d0a 6475 7065 6368 6563  ripts]..dupechec
+00000470: 6b65 7220 3d20 2264 7570 6563 6865 636b  ker = "dupecheck
+00000480: 6572 2e64 7570 6563 6865 636b 6572 3a6d  er.dupechecker:m
+00000490: 6169 6e22 0d0a                           ain"..
```

### Comparing `dupechecker-0.2.1/PKG-INFO` & `dupechecker-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: dupechecker
-Version: 0.2.1
+Version: 1.0.0
 Summary: Check for and delete duplicate files from the command line.
 Project-URL: Homepage, https://github.com/matt-manes/dupechecker
 Project-URL: Documentation, https://github.com/matt-manes/dupechecker/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/dupechecker/tree/main/src/dupechecker
 Author-email: Matt Manes <mattmanes@pm.me>
 License-File: LICENSE.txt
 Keywords: cli,filecmp,filesystem
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: griddle
+Requires-Dist: noiftimer
 Requires-Dist: pathier
 Requires-Dist: printbuddies
 Requires-Dist: pytest
 Requires-Dist: younotyou
 Description-Content-Type: text/markdown
 
 # dupechecker
@@ -33,20 +34,22 @@
 
 
 
 ## Usage
 
 <pre>
 >dupechecker -h
-usage: dupechecker [-h] [-r] [-d] [-ad] [-ns] [path]
+
+usage: dupechecker [-h] [-r] [-i [IGNORES ...]] [-d] [-ad] [-ns] [paths ...]
 
 positional arguments:
-  path                The path to compare files in.
+  paths                 The paths to compare files in.
 
 options:
-  -h, --help          show this help message and exit
-  -r, --recursive     Glob files to compare recursively.
-  -d, --delete_dupes  After finding duplicates, delete all but one copy. For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep.
-                      Pressing 'enter' without entering a number will skip that set without deleting anything.
-  -ad, --autodelete   Automatically decide which file to keep and which to delete from each set of duplicate files instead of asking which to keep.
-  -ns, --no_show      Don't show printout of matching files.
+  -h, --help            show this help message and exit
+  -r, --recursive       Glob files to compare recursively.
+  -i [IGNORES ...], --ignores [IGNORES ...]
+                        Ignore files matching these patterns. e.g. `dupechecker -i *.wav` will compare all files in the current working directory except .wav files.
+  -d, --delete_dupes    After finding duplicates, delete all but one copy. For each set of duplicates, the tool will ask you to enter the number corresponding to the copy you want to keep. Pressing 'enter' without entering a number will skip that set without deleting anything.
+  -ad, --autodelete     Automatically decide which file to keep and which to delete from each set of duplicate files instead of asking which to keep.
+  -ns, --no_show        Don't show printout of matching files.
 </pre>
```

