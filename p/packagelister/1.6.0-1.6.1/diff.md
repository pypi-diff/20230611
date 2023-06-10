# Comparing `tmp/packagelister-1.6.0.tar.gz` & `tmp/packagelister-1.6.1.tar.gz`

## Comparing `packagelister-1.6.0.tar` & `packagelister-1.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 packagelister-1.6.0/CHANGELOG.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.6.0/docs/index.html
--rw-r--r--   0        0        0    34336 2020-02-02 00:00:00.000000 packagelister-1.6.0/docs/packagelister.html
--rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 packagelister-1.6.0/docs/search.js
--rw-r--r--   0        0        0    80468 2020-02-02 00:00:00.000000 packagelister-1.6.0/docs/packagelister/packagelister.html
--rw-r--r--   0        0        0    76578 2020-02-02 00:00:00.000000 packagelister-1.6.0/docs/packagelister/packagelister_cli.html
--rw-r--r--   0        0        0    56429 2020-02-02 00:00:00.000000 packagelister-1.6.0/docs/packagelister/whouses.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 packagelister-1.6.0/src/packagelister/__init__.py
--rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 packagelister-1.6.0/src/packagelister/packagelister.py
--rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 packagelister-1.6.0/src/packagelister/packagelister_cli.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 packagelister-1.6.0/src/packagelister/whouses.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.6.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.6.0/README.md
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 packagelister-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 packagelister-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 packagelister-1.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/index.html
+-rw-r--r--   0        0        0    34336 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/packagelister.html
+-rw-r--r--   0        0        0    25353 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/search.js
+-rw-r--r--   0        0        0    79722 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/packagelister/packagelister.html
+-rw-r--r--   0        0        0    77472 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/packagelister/packagelister_cli.html
+-rw-r--r--   0        0        0    56429 2020-02-02 00:00:00.000000 packagelister-1.6.1/docs/packagelister/whouses.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 packagelister-1.6.1/src/packagelister/__init__.py
+-rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 packagelister-1.6.1/src/packagelister/packagelister.py
+-rw-r--r--   0        0        0     3274 2020-02-02 00:00:00.000000 packagelister-1.6.1/src/packagelister/packagelister_cli.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 packagelister-1.6.1/src/packagelister/whouses.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.6.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.6.1/README.md
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 packagelister-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 packagelister-1.6.1/PKG-INFO
```

### Comparing `packagelister-1.6.0/CHANGELOG.md` & `packagelister-1.6.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,36 @@
 # Changelog
 
+## v1.6.0 (2023-06-10)
+
+#### New Features
+
+* replace package names with pip name when they don't match when generating requirements
+#### Fixes
+
+* fix not getting package versions
+#### Performance improvements
+
+* use ast module to extract packages
+#### Refactorings
+
+* add default value to ignore arg in find()
+* replace pathlib with pathier
+* rename top_dir to root
+* remove recursive option from get_packages_from_source
+#### Docs
+
+* update help message
+* improve docstrings
+#### Others
+
+* add missing version prefix
+* remove invalid assertion
+
+
 ## v1.5.1 (2023-05-02)
 
 #### Fixes
 
 * fix crash when trying to import something that isn't a module
```

### Comparing `packagelister-1.6.0/docs/packagelister.html` & `packagelister-1.6.1/docs/packagelister.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.0/docs/search.js` & `packagelister-1.6.1/docs/search.js`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.0/docs/packagelister/packagelister.html` & `packagelister-1.6.1/docs/packagelister/packagelister.html`

 * *Files 0% similar despite different names*

```diff
@@ -79,82 +79,81 @@
 </span><span id="L-17"><a href="#L-17"><span class="linenos">17</span></a>            <span class="n">package</span> <span class="o">=</span> <span class="n">node</span><span class="o">.</span><span class="n">names</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">name</span>
 </span><span id="L-18"><a href="#L-18"><span class="linenos">18</span></a>        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">ImportFrom</span><span class="p">:</span>
 </span><span id="L-19"><a href="#L-19"><span class="linenos">19</span></a>            <span class="n">package</span> <span class="o">=</span> <span class="n">node</span><span class="o">.</span><span class="n">module</span>
 </span><span id="L-20"><a href="#L-20"><span class="linenos">20</span></a>        <span class="k">if</span> <span class="n">package</span><span class="p">:</span>
 </span><span id="L-21"><a href="#L-21"><span class="linenos">21</span></a>            <span class="k">if</span> <span class="s2">&quot;.&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
 </span><span id="L-22"><a href="#L-22"><span class="linenos">22</span></a>                <span class="n">package</span> <span class="o">=</span> <span class="n">package</span><span class="p">[:</span> <span class="n">package</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
 </span><span id="L-23"><a href="#L-23"><span class="linenos">23</span></a>            <span class="n">packages</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">packages</span><span class="p">)))</span>
-</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>    <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">packages</span><span class="p">)))</span>
+</span><span id="L-24"><a href="#L-24"><span class="linenos">24</span></a>    <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">packages</span><span class="p">)))</span>
+</span><span id="L-25"><a href="#L-25"><span class="linenos">25</span></a>
 </span><span id="L-26"><a href="#L-26"><span class="linenos">26</span></a>
-</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>
-</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a><span class="k">def</span> <span class="nf">remove_builtins</span><span class="p">(</span><span class="n">packages</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>    <span class="sd">&quot;&quot;&quot;Remove built in packages/modules from a list of package names.&quot;&quot;&quot;</span>
-</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>    <span class="n">builtins</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">sys</span><span class="o">.</span><span class="n">stdlib_module_names</span><span class="p">)</span>
-</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>    <span class="k">return</span> <span class="nb">filter</span><span class="p">(</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">builtins</span><span class="p">,</span> <span class="n">packages</span><span class="p">)</span>
+</span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a><span class="k">def</span> <span class="nf">remove_builtins</span><span class="p">(</span><span class="n">packages</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>    <span class="sd">&quot;&quot;&quot;Remove built in packages/modules from a list of package names.&quot;&quot;&quot;</span>
+</span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>    <span class="n">builtins</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">sys</span><span class="o">.</span><span class="n">stdlib_module_names</span><span class="p">)</span>
+</span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>    <span class="k">return</span> <span class="nb">filter</span><span class="p">(</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">builtins</span><span class="p">,</span> <span class="n">packages</span><span class="p">)</span>
+</span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>
 </span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>
-</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>
-</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a><span class="k">def</span> <span class="nf">scan</span><span class="p">(</span><span class="n">project_dir</span><span class="p">:</span> <span class="n">Pathish</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">include_builtins</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>    <span class="sd">&quot;&quot;&quot;Recursively scans a directory for python files to determine</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a><span class="sd">    what packages are in use, as well as the version number if applicable.</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>
-</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a><span class="sd">    Returns a dictionary where the keys are package names and</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a><span class="sd">    the values are dictionaries with the keys `version` for the version number of the package</span>
-</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a><span class="sd">    if there is one (None if there isn&#39;t) and `files` for a list of the files that import the package.</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>
-</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a><span class="sd">    :param project_dir: Can be an absolute or relative path to a directory or a single file (.py).</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a><span class="sd">    If it is relative, it will be assumed to be relative to the current working directory.</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a><span class="sd">    If an argument isn&#39;t given, the current working directory will be scanned.</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a><span class="sd">    If the path doesn&#39;t exist, an empty dictionary is returned.&quot;&quot;&quot;</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="p">:</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>    <span class="k">elif</span> <span class="nb">type</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span> <span class="ow">or</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span>
-</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
-</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos">52</span></a>
-</span><span id="L-53"><a href="#L-53"><span class="linenos">53</span></a>    <span class="c1"># Raise error if project_dir doesn&#39;t exist</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos">54</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos">55</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos">56</span></a>            <span class="sa">f</span><span class="s2">&quot;Can&#39;t scan directory that doesn&#39;t exist: </span><span class="si">{</span><span class="n">project_dir</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos">57</span></a>        <span class="p">)</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos">58</span></a>    <span class="c1"># You can scan a non python file one at a time if you reeeally want to.</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos">59</span></a>    <span class="k">if</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos">60</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">project_dir</span><span class="p">]</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos">61</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos">62</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">project_dir</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">))</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos">63</span></a>
-</span><span id="L-64"><a href="#L-64"><span class="linenos">64</span></a>    <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">),</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.33</span><span class="p">)</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos">65</span></a>    <span class="n">used_packages</span> <span class="o">=</span> <span class="p">{}</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos">66</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos">67</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Scanning </span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="L-68"><a href="#L-68"><span class="linenos">68</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="s2">&quot;utf-8&quot;</span><span class="p">)</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos">69</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="n">get_packages_from_source</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos">70</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">include_builtins</span><span class="p">:</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos">71</span></a>            <span class="n">packages</span> <span class="o">=</span> <span class="n">remove_builtins</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos">72</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos">73</span></a>            <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos">74</span></a>                <span class="k">if</span> <span class="p">(</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos">75</span></a>                    <span class="n">package</span> <span class="ow">in</span> <span class="n">used_packages</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos">76</span></a>                    <span class="ow">and</span> <span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos">77</span></a>                <span class="p">):</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos">78</span></a>                    <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">))</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos">79</span></a>                <span class="k">else</span><span class="p">:</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos">80</span></a>                    <span class="k">try</span><span class="p">:</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos">81</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="n">importlib</span><span class="o">.</span><span class="n">metadata</span><span class="o">.</span><span class="n">version</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos">82</span></a>                    <span class="k">except</span> <span class="ne">ModuleNotFoundError</span><span class="p">:</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos">83</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos">84</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos">85</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos">86</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="L-87"><a href="#L-87"><span class="linenos">87</span></a>                    <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">]</span> <span class="o">=</span> <span class="p">{</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos">88</span></a>                        <span class="s2">&quot;files&quot;</span><span class="p">:</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)],</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos">89</span></a>                        <span class="s2">&quot;version&quot;</span><span class="p">:</span> <span class="n">package_version</span><span class="p">,</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos">90</span></a>                    <span class="p">}</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos">91</span></a>    <span class="k">return</span> <span class="n">used_packages</span>
+</span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a><span class="k">def</span> <span class="nf">scan</span><span class="p">(</span><span class="n">project_dir</span><span class="p">:</span> <span class="n">Pathish</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">include_builtins</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>    <span class="sd">&quot;&quot;&quot;Recursively scans a directory for python files to determine</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a><span class="sd">    what packages are in use, as well as the version number if applicable.</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>
+</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a><span class="sd">    Returns a dictionary where the keys are package names and</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a><span class="sd">    the values are dictionaries with the keys `version` for the version number of the package</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a><span class="sd">    if there is one (None if there isn&#39;t) and `files` for a list of the files that import the package.</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>
+</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a><span class="sd">    :param project_dir: Can be an absolute or relative path to a directory or a single file (.py).</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a><span class="sd">    If it is relative, it will be assumed to be relative to the current working directory.</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a><span class="sd">    If an argument isn&#39;t given, the current working directory will be scanned.</span>
+</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a><span class="sd">    If the path doesn&#39;t exist, an empty dictionary is returned.&quot;&quot;&quot;</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="p">:</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>    <span class="k">elif</span> <span class="nb">type</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span> <span class="ow">or</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
+</span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>
+</span><span id="L-52"><a href="#L-52"><span class="linenos">52</span></a>    <span class="c1"># Raise error if project_dir doesn&#39;t exist</span>
+</span><span id="L-53"><a href="#L-53"><span class="linenos">53</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos">54</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos">55</span></a>            <span class="sa">f</span><span class="s2">&quot;Can&#39;t scan directory that doesn&#39;t exist: </span><span class="si">{</span><span class="n">project_dir</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos">56</span></a>        <span class="p">)</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos">57</span></a>    <span class="c1"># You can scan a non python file one at a time if you reeeally want to.</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos">58</span></a>    <span class="k">if</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos">59</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">project_dir</span><span class="p">]</span>
+</span><span id="L-60"><a href="#L-60"><span class="linenos">60</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos">61</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">project_dir</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">))</span>
+</span><span id="L-62"><a href="#L-62"><span class="linenos">62</span></a>
+</span><span id="L-63"><a href="#L-63"><span class="linenos">63</span></a>    <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">),</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.33</span><span class="p">)</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos">64</span></a>    <span class="n">used_packages</span> <span class="o">=</span> <span class="p">{}</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos">65</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos">66</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Scanning </span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos">67</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="s2">&quot;utf-8&quot;</span><span class="p">)</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos">68</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="n">get_packages_from_source</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos">69</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">include_builtins</span><span class="p">:</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos">70</span></a>            <span class="n">packages</span> <span class="o">=</span> <span class="n">remove_builtins</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos">71</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos">72</span></a>            <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos">73</span></a>                <span class="k">if</span> <span class="p">(</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos">74</span></a>                    <span class="n">package</span> <span class="ow">in</span> <span class="n">used_packages</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos">75</span></a>                    <span class="ow">and</span> <span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos">76</span></a>                <span class="p">):</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos">77</span></a>                    <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">))</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos">78</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos">79</span></a>                    <span class="k">try</span><span class="p">:</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos">80</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="n">importlib</span><span class="o">.</span><span class="n">metadata</span><span class="o">.</span><span class="n">version</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos">81</span></a>                    <span class="k">except</span> <span class="ne">ModuleNotFoundError</span><span class="p">:</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos">82</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos">83</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos">84</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos">85</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos">86</span></a>                    <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">]</span> <span class="o">=</span> <span class="p">{</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos">87</span></a>                        <span class="s2">&quot;files&quot;</span><span class="p">:</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)],</span>
+</span><span id="L-88"><a href="#L-88"><span class="linenos">88</span></a>                        <span class="s2">&quot;version&quot;</span><span class="p">:</span> <span class="n">package_version</span><span class="p">,</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos">89</span></a>                    <span class="p">}</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos">90</span></a>    <span class="k">return</span> <span class="n">used_packages</span>
 </span></pre></div>
 
 
             </section>
                 <section id="get_packages_from_source">
                             <input id="get_packages_from_source-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -177,16 +176,15 @@
 </span><span id="get_packages_from_source-18"><a href="#get_packages_from_source-18"><span class="linenos">18</span></a>            <span class="n">package</span> <span class="o">=</span> <span class="n">node</span><span class="o">.</span><span class="n">names</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">name</span>
 </span><span id="get_packages_from_source-19"><a href="#get_packages_from_source-19"><span class="linenos">19</span></a>        <span class="k">elif</span> <span class="n">type_</span> <span class="o">==</span> <span class="n">ast</span><span class="o">.</span><span class="n">ImportFrom</span><span class="p">:</span>
 </span><span id="get_packages_from_source-20"><a href="#get_packages_from_source-20"><span class="linenos">20</span></a>            <span class="n">package</span> <span class="o">=</span> <span class="n">node</span><span class="o">.</span><span class="n">module</span>
 </span><span id="get_packages_from_source-21"><a href="#get_packages_from_source-21"><span class="linenos">21</span></a>        <span class="k">if</span> <span class="n">package</span><span class="p">:</span>
 </span><span id="get_packages_from_source-22"><a href="#get_packages_from_source-22"><span class="linenos">22</span></a>            <span class="k">if</span> <span class="s2">&quot;.&quot;</span> <span class="ow">in</span> <span class="n">package</span><span class="p">:</span>
 </span><span id="get_packages_from_source-23"><a href="#get_packages_from_source-23"><span class="linenos">23</span></a>                <span class="n">package</span> <span class="o">=</span> <span class="n">package</span><span class="p">[:</span> <span class="n">package</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;.&quot;</span><span class="p">)]</span>
 </span><span id="get_packages_from_source-24"><a href="#get_packages_from_source-24"><span class="linenos">24</span></a>            <span class="n">packages</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="get_packages_from_source-25"><a href="#get_packages_from_source-25"><span class="linenos">25</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">packages</span><span class="p">)))</span>
-</span><span id="get_packages_from_source-26"><a href="#get_packages_from_source-26"><span class="linenos">26</span></a>    <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">packages</span><span class="p">)))</span>
+</span><span id="get_packages_from_source-25"><a href="#get_packages_from_source-25"><span class="linenos">25</span></a>    <span class="k">return</span> <span class="nb">sorted</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="nb">set</span><span class="p">(</span><span class="n">packages</span><span class="p">)))</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Scan <code>source</code> and extract the names of imported packages/modules.</p>
 </div>
 
 
@@ -198,18 +196,18 @@
         <span class="def">def</span>
         <span class="name">remove_builtins</span><span class="signature pdoc-code condensed">(<span class="param"><span class="n">packages</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span></span><span class="return-annotation">) -> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]</span>:</span></span>
 
                 <label class="view-source-button" for="remove_builtins-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#remove_builtins"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="remove_builtins-29"><a href="#remove_builtins-29"><span class="linenos">29</span></a><span class="k">def</span> <span class="nf">remove_builtins</span><span class="p">(</span><span class="n">packages</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
-</span><span id="remove_builtins-30"><a href="#remove_builtins-30"><span class="linenos">30</span></a>    <span class="sd">&quot;&quot;&quot;Remove built in packages/modules from a list of package names.&quot;&quot;&quot;</span>
-</span><span id="remove_builtins-31"><a href="#remove_builtins-31"><span class="linenos">31</span></a>    <span class="n">builtins</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">sys</span><span class="o">.</span><span class="n">stdlib_module_names</span><span class="p">)</span>
-</span><span id="remove_builtins-32"><a href="#remove_builtins-32"><span class="linenos">32</span></a>    <span class="k">return</span> <span class="nb">filter</span><span class="p">(</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">builtins</span><span class="p">,</span> <span class="n">packages</span><span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="remove_builtins-28"><a href="#remove_builtins-28"><span class="linenos">28</span></a><span class="k">def</span> <span class="nf">remove_builtins</span><span class="p">(</span><span class="n">packages</span><span class="p">:</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">])</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
+</span><span id="remove_builtins-29"><a href="#remove_builtins-29"><span class="linenos">29</span></a>    <span class="sd">&quot;&quot;&quot;Remove built in packages/modules from a list of package names.&quot;&quot;&quot;</span>
+</span><span id="remove_builtins-30"><a href="#remove_builtins-30"><span class="linenos">30</span></a>    <span class="n">builtins</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">sys</span><span class="o">.</span><span class="n">stdlib_module_names</span><span class="p">)</span>
+</span><span id="remove_builtins-31"><a href="#remove_builtins-31"><span class="linenos">31</span></a>    <span class="k">return</span> <span class="nb">filter</span><span class="p">(</span><span class="k">lambda</span> <span class="n">x</span><span class="p">:</span> <span class="n">x</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">builtins</span><span class="p">,</span> <span class="n">packages</span><span class="p">)</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Remove built in packages/modules from a list of package names.</p>
 </div>
 
 
@@ -221,72 +219,72 @@
         <span class="def">def</span>
         <span class="name">scan</span><span class="signature pdoc-code multiline">(<span class="param">	<span class="n">project_dir</span><span class="p">:</span> <span class="n">pathier</span><span class="o">.</span><span class="n">pathier</span><span class="o">.</span><span class="n">Pathier</span> <span class="o">|</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span> <span class="o">|</span> <span class="nb">str</span> <span class="o">=</span> <span class="kc">None</span>,</span><span class="param">	<span class="n">include_builtins</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span></span><span class="return-annotation">) -> <span class="nb">dict</span>:</span></span>
 
                 <label class="view-source-button" for="scan-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#scan"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="scan-35"><a href="#scan-35"><span class="linenos">35</span></a><span class="k">def</span> <span class="nf">scan</span><span class="p">(</span><span class="n">project_dir</span><span class="p">:</span> <span class="n">Pathish</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">include_builtins</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
-</span><span id="scan-36"><a href="#scan-36"><span class="linenos">36</span></a>    <span class="sd">&quot;&quot;&quot;Recursively scans a directory for python files to determine</span>
-</span><span id="scan-37"><a href="#scan-37"><span class="linenos">37</span></a><span class="sd">    what packages are in use, as well as the version number if applicable.</span>
-</span><span id="scan-38"><a href="#scan-38"><span class="linenos">38</span></a>
-</span><span id="scan-39"><a href="#scan-39"><span class="linenos">39</span></a><span class="sd">    Returns a dictionary where the keys are package names and</span>
-</span><span id="scan-40"><a href="#scan-40"><span class="linenos">40</span></a><span class="sd">    the values are dictionaries with the keys `version` for the version number of the package</span>
-</span><span id="scan-41"><a href="#scan-41"><span class="linenos">41</span></a><span class="sd">    if there is one (None if there isn&#39;t) and `files` for a list of the files that import the package.</span>
-</span><span id="scan-42"><a href="#scan-42"><span class="linenos">42</span></a>
-</span><span id="scan-43"><a href="#scan-43"><span class="linenos">43</span></a><span class="sd">    :param project_dir: Can be an absolute or relative path to a directory or a single file (.py).</span>
-</span><span id="scan-44"><a href="#scan-44"><span class="linenos">44</span></a><span class="sd">    If it is relative, it will be assumed to be relative to the current working directory.</span>
-</span><span id="scan-45"><a href="#scan-45"><span class="linenos">45</span></a><span class="sd">    If an argument isn&#39;t given, the current working directory will be scanned.</span>
-</span><span id="scan-46"><a href="#scan-46"><span class="linenos">46</span></a><span class="sd">    If the path doesn&#39;t exist, an empty dictionary is returned.&quot;&quot;&quot;</span>
-</span><span id="scan-47"><a href="#scan-47"><span class="linenos">47</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="p">:</span>
-</span><span id="scan-48"><a href="#scan-48"><span class="linenos">48</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="scan-49"><a href="#scan-49"><span class="linenos">49</span></a>    <span class="k">elif</span> <span class="nb">type</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span> <span class="ow">or</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="scan-50"><a href="#scan-50"><span class="linenos">50</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span>
-</span><span id="scan-51"><a href="#scan-51"><span class="linenos">51</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
-</span><span id="scan-52"><a href="#scan-52"><span class="linenos">52</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
-</span><span id="scan-53"><a href="#scan-53"><span class="linenos">53</span></a>
-</span><span id="scan-54"><a href="#scan-54"><span class="linenos">54</span></a>    <span class="c1"># Raise error if project_dir doesn&#39;t exist</span>
-</span><span id="scan-55"><a href="#scan-55"><span class="linenos">55</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
-</span><span id="scan-56"><a href="#scan-56"><span class="linenos">56</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span>
-</span><span id="scan-57"><a href="#scan-57"><span class="linenos">57</span></a>            <span class="sa">f</span><span class="s2">&quot;Can&#39;t scan directory that doesn&#39;t exist: </span><span class="si">{</span><span class="n">project_dir</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="scan-58"><a href="#scan-58"><span class="linenos">58</span></a>        <span class="p">)</span>
-</span><span id="scan-59"><a href="#scan-59"><span class="linenos">59</span></a>    <span class="c1"># You can scan a non python file one at a time if you reeeally want to.</span>
-</span><span id="scan-60"><a href="#scan-60"><span class="linenos">60</span></a>    <span class="k">if</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
-</span><span id="scan-61"><a href="#scan-61"><span class="linenos">61</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">project_dir</span><span class="p">]</span>
-</span><span id="scan-62"><a href="#scan-62"><span class="linenos">62</span></a>    <span class="k">else</span><span class="p">:</span>
-</span><span id="scan-63"><a href="#scan-63"><span class="linenos">63</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">project_dir</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">))</span>
-</span><span id="scan-64"><a href="#scan-64"><span class="linenos">64</span></a>
-</span><span id="scan-65"><a href="#scan-65"><span class="linenos">65</span></a>    <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">),</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.33</span><span class="p">)</span>
-</span><span id="scan-66"><a href="#scan-66"><span class="linenos">66</span></a>    <span class="n">used_packages</span> <span class="o">=</span> <span class="p">{}</span>
-</span><span id="scan-67"><a href="#scan-67"><span class="linenos">67</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="scan-68"><a href="#scan-68"><span class="linenos">68</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Scanning </span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
-</span><span id="scan-69"><a href="#scan-69"><span class="linenos">69</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="s2">&quot;utf-8&quot;</span><span class="p">)</span>
-</span><span id="scan-70"><a href="#scan-70"><span class="linenos">70</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="n">get_packages_from_source</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
-</span><span id="scan-71"><a href="#scan-71"><span class="linenos">71</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">include_builtins</span><span class="p">:</span>
-</span><span id="scan-72"><a href="#scan-72"><span class="linenos">72</span></a>            <span class="n">packages</span> <span class="o">=</span> <span class="n">remove_builtins</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
-</span><span id="scan-73"><a href="#scan-73"><span class="linenos">73</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
-</span><span id="scan-74"><a href="#scan-74"><span class="linenos">74</span></a>            <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
-</span><span id="scan-75"><a href="#scan-75"><span class="linenos">75</span></a>                <span class="k">if</span> <span class="p">(</span>
-</span><span id="scan-76"><a href="#scan-76"><span class="linenos">76</span></a>                    <span class="n">package</span> <span class="ow">in</span> <span class="n">used_packages</span>
-</span><span id="scan-77"><a href="#scan-77"><span class="linenos">77</span></a>                    <span class="ow">and</span> <span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
-</span><span id="scan-78"><a href="#scan-78"><span class="linenos">78</span></a>                <span class="p">):</span>
-</span><span id="scan-79"><a href="#scan-79"><span class="linenos">79</span></a>                    <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">))</span>
-</span><span id="scan-80"><a href="#scan-80"><span class="linenos">80</span></a>                <span class="k">else</span><span class="p">:</span>
-</span><span id="scan-81"><a href="#scan-81"><span class="linenos">81</span></a>                    <span class="k">try</span><span class="p">:</span>
-</span><span id="scan-82"><a href="#scan-82"><span class="linenos">82</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="n">importlib</span><span class="o">.</span><span class="n">metadata</span><span class="o">.</span><span class="n">version</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
-</span><span id="scan-83"><a href="#scan-83"><span class="linenos">83</span></a>                    <span class="k">except</span> <span class="ne">ModuleNotFoundError</span><span class="p">:</span>
-</span><span id="scan-84"><a href="#scan-84"><span class="linenos">84</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="scan-85"><a href="#scan-85"><span class="linenos">85</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
-</span><span id="scan-86"><a href="#scan-86"><span class="linenos">86</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
-</span><span id="scan-87"><a href="#scan-87"><span class="linenos">87</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="kc">None</span>
-</span><span id="scan-88"><a href="#scan-88"><span class="linenos">88</span></a>                    <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">]</span> <span class="o">=</span> <span class="p">{</span>
-</span><span id="scan-89"><a href="#scan-89"><span class="linenos">89</span></a>                        <span class="s2">&quot;files&quot;</span><span class="p">:</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)],</span>
-</span><span id="scan-90"><a href="#scan-90"><span class="linenos">90</span></a>                        <span class="s2">&quot;version&quot;</span><span class="p">:</span> <span class="n">package_version</span><span class="p">,</span>
-</span><span id="scan-91"><a href="#scan-91"><span class="linenos">91</span></a>                    <span class="p">}</span>
-</span><span id="scan-92"><a href="#scan-92"><span class="linenos">92</span></a>    <span class="k">return</span> <span class="n">used_packages</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="scan-34"><a href="#scan-34"><span class="linenos">34</span></a><span class="k">def</span> <span class="nf">scan</span><span class="p">(</span><span class="n">project_dir</span><span class="p">:</span> <span class="n">Pathish</span> <span class="o">=</span> <span class="kc">None</span><span class="p">,</span> <span class="n">include_builtins</span><span class="p">:</span> <span class="nb">bool</span> <span class="o">=</span> <span class="kc">False</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">dict</span><span class="p">:</span>
+</span><span id="scan-35"><a href="#scan-35"><span class="linenos">35</span></a>    <span class="sd">&quot;&quot;&quot;Recursively scans a directory for python files to determine</span>
+</span><span id="scan-36"><a href="#scan-36"><span class="linenos">36</span></a><span class="sd">    what packages are in use, as well as the version number if applicable.</span>
+</span><span id="scan-37"><a href="#scan-37"><span class="linenos">37</span></a>
+</span><span id="scan-38"><a href="#scan-38"><span class="linenos">38</span></a><span class="sd">    Returns a dictionary where the keys are package names and</span>
+</span><span id="scan-39"><a href="#scan-39"><span class="linenos">39</span></a><span class="sd">    the values are dictionaries with the keys `version` for the version number of the package</span>
+</span><span id="scan-40"><a href="#scan-40"><span class="linenos">40</span></a><span class="sd">    if there is one (None if there isn&#39;t) and `files` for a list of the files that import the package.</span>
+</span><span id="scan-41"><a href="#scan-41"><span class="linenos">41</span></a>
+</span><span id="scan-42"><a href="#scan-42"><span class="linenos">42</span></a><span class="sd">    :param project_dir: Can be an absolute or relative path to a directory or a single file (.py).</span>
+</span><span id="scan-43"><a href="#scan-43"><span class="linenos">43</span></a><span class="sd">    If it is relative, it will be assumed to be relative to the current working directory.</span>
+</span><span id="scan-44"><a href="#scan-44"><span class="linenos">44</span></a><span class="sd">    If an argument isn&#39;t given, the current working directory will be scanned.</span>
+</span><span id="scan-45"><a href="#scan-45"><span class="linenos">45</span></a><span class="sd">    If the path doesn&#39;t exist, an empty dictionary is returned.&quot;&quot;&quot;</span>
+</span><span id="scan-46"><a href="#scan-46"><span class="linenos">46</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="p">:</span>
+</span><span id="scan-47"><a href="#scan-47"><span class="linenos">47</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="scan-48"><a href="#scan-48"><span class="linenos">48</span></a>    <span class="k">elif</span> <span class="nb">type</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span> <span class="ow">is</span> <span class="nb">str</span> <span class="ow">or</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="scan-49"><a href="#scan-49"><span class="linenos">49</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">project_dir</span><span class="p">)</span>
+</span><span id="scan-50"><a href="#scan-50"><span class="linenos">50</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
+</span><span id="scan-51"><a href="#scan-51"><span class="linenos">51</span></a>        <span class="n">project_dir</span> <span class="o">=</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
+</span><span id="scan-52"><a href="#scan-52"><span class="linenos">52</span></a>
+</span><span id="scan-53"><a href="#scan-53"><span class="linenos">53</span></a>    <span class="c1"># Raise error if project_dir doesn&#39;t exist</span>
+</span><span id="scan-54"><a href="#scan-54"><span class="linenos">54</span></a>    <span class="k">if</span> <span class="ow">not</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">exists</span><span class="p">():</span>
+</span><span id="scan-55"><a href="#scan-55"><span class="linenos">55</span></a>        <span class="k">raise</span> <span class="ne">FileNotFoundError</span><span class="p">(</span>
+</span><span id="scan-56"><a href="#scan-56"><span class="linenos">56</span></a>            <span class="sa">f</span><span class="s2">&quot;Can&#39;t scan directory that doesn&#39;t exist: </span><span class="si">{</span><span class="n">project_dir</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="scan-57"><a href="#scan-57"><span class="linenos">57</span></a>        <span class="p">)</span>
+</span><span id="scan-58"><a href="#scan-58"><span class="linenos">58</span></a>    <span class="c1"># You can scan a non python file one at a time if you reeeally want to.</span>
+</span><span id="scan-59"><a href="#scan-59"><span class="linenos">59</span></a>    <span class="k">if</span> <span class="n">project_dir</span><span class="o">.</span><span class="n">is_file</span><span class="p">():</span>
+</span><span id="scan-60"><a href="#scan-60"><span class="linenos">60</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="p">[</span><span class="n">project_dir</span><span class="p">]</span>
+</span><span id="scan-61"><a href="#scan-61"><span class="linenos">61</span></a>    <span class="k">else</span><span class="p">:</span>
+</span><span id="scan-62"><a href="#scan-62"><span class="linenos">62</span></a>        <span class="n">files</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">project_dir</span><span class="o">.</span><span class="n">rglob</span><span class="p">(</span><span class="s2">&quot;*.py&quot;</span><span class="p">))</span>
+</span><span id="scan-63"><a href="#scan-63"><span class="linenos">63</span></a>
+</span><span id="scan-64"><a href="#scan-64"><span class="linenos">64</span></a>    <span class="n">bar</span> <span class="o">=</span> <span class="n">ProgBar</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">files</span><span class="p">),</span> <span class="n">width_ratio</span><span class="o">=</span><span class="mf">0.33</span><span class="p">)</span>
+</span><span id="scan-65"><a href="#scan-65"><span class="linenos">65</span></a>    <span class="n">used_packages</span> <span class="o">=</span> <span class="p">{}</span>
+</span><span id="scan-66"><a href="#scan-66"><span class="linenos">66</span></a>    <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="scan-67"><a href="#scan-67"><span class="linenos">67</span></a>        <span class="n">bar</span><span class="o">.</span><span class="n">display</span><span class="p">(</span><span class="n">suffix</span><span class="o">=</span><span class="sa">f</span><span class="s2">&quot;Scanning </span><span class="si">{</span><span class="n">file</span><span class="o">.</span><span class="n">name</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span>
+</span><span id="scan-68"><a href="#scan-68"><span class="linenos">68</span></a>        <span class="n">source</span> <span class="o">=</span> <span class="n">file</span><span class="o">.</span><span class="n">read_text</span><span class="p">(</span><span class="n">encoding</span><span class="o">=</span><span class="s2">&quot;utf-8&quot;</span><span class="p">)</span>
+</span><span id="scan-69"><a href="#scan-69"><span class="linenos">69</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="n">get_packages_from_source</span><span class="p">(</span><span class="n">source</span><span class="p">)</span>
+</span><span id="scan-70"><a href="#scan-70"><span class="linenos">70</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">include_builtins</span><span class="p">:</span>
+</span><span id="scan-71"><a href="#scan-71"><span class="linenos">71</span></a>            <span class="n">packages</span> <span class="o">=</span> <span class="n">remove_builtins</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="scan-72"><a href="#scan-72"><span class="linenos">72</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">:</span>
+</span><span id="scan-73"><a href="#scan-73"><span class="linenos">73</span></a>            <span class="k">if</span> <span class="n">file</span><span class="o">.</span><span class="n">with_stem</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">files</span><span class="p">:</span>
+</span><span id="scan-74"><a href="#scan-74"><span class="linenos">74</span></a>                <span class="k">if</span> <span class="p">(</span>
+</span><span id="scan-75"><a href="#scan-75"><span class="linenos">75</span></a>                    <span class="n">package</span> <span class="ow">in</span> <span class="n">used_packages</span>
+</span><span id="scan-76"><a href="#scan-76"><span class="linenos">76</span></a>                    <span class="ow">and</span> <span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
+</span><span id="scan-77"><a href="#scan-77"><span class="linenos">77</span></a>                <span class="p">):</span>
+</span><span id="scan-78"><a href="#scan-78"><span class="linenos">78</span></a>                    <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">))</span>
+</span><span id="scan-79"><a href="#scan-79"><span class="linenos">79</span></a>                <span class="k">else</span><span class="p">:</span>
+</span><span id="scan-80"><a href="#scan-80"><span class="linenos">80</span></a>                    <span class="k">try</span><span class="p">:</span>
+</span><span id="scan-81"><a href="#scan-81"><span class="linenos">81</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="n">importlib</span><span class="o">.</span><span class="n">metadata</span><span class="o">.</span><span class="n">version</span><span class="p">(</span><span class="n">package</span><span class="p">)</span>
+</span><span id="scan-82"><a href="#scan-82"><span class="linenos">82</span></a>                    <span class="k">except</span> <span class="ne">ModuleNotFoundError</span><span class="p">:</span>
+</span><span id="scan-83"><a href="#scan-83"><span class="linenos">83</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="scan-84"><a href="#scan-84"><span class="linenos">84</span></a>                    <span class="k">except</span> <span class="ne">Exception</span> <span class="k">as</span> <span class="n">e</span><span class="p">:</span>
+</span><span id="scan-85"><a href="#scan-85"><span class="linenos">85</span></a>                        <span class="nb">print</span><span class="p">(</span><span class="n">e</span><span class="p">)</span>
+</span><span id="scan-86"><a href="#scan-86"><span class="linenos">86</span></a>                        <span class="n">package_version</span> <span class="o">=</span> <span class="kc">None</span>
+</span><span id="scan-87"><a href="#scan-87"><span class="linenos">87</span></a>                    <span class="n">used_packages</span><span class="p">[</span><span class="n">package</span><span class="p">]</span> <span class="o">=</span> <span class="p">{</span>
+</span><span id="scan-88"><a href="#scan-88"><span class="linenos">88</span></a>                        <span class="s2">&quot;files&quot;</span><span class="p">:</span> <span class="p">[</span><span class="nb">str</span><span class="p">(</span><span class="n">file</span><span class="p">)],</span>
+</span><span id="scan-89"><a href="#scan-89"><span class="linenos">89</span></a>                        <span class="s2">&quot;version&quot;</span><span class="p">:</span> <span class="n">package_version</span><span class="p">,</span>
+</span><span id="scan-90"><a href="#scan-90"><span class="linenos">90</span></a>                    <span class="p">}</span>
+</span><span id="scan-91"><a href="#scan-91"><span class="linenos">91</span></a>    <span class="k">return</span> <span class="n">used_packages</span>
 </span></pre></div>
 
 
             <div class="docstring"><p>Recursively scans a directory for python files to determine
 what packages are in use, as well as the version number if applicable.</p>
 
 <p>Returns a dictionary where the keys are package names and
```

#### html2text {}

```diff
@@ -29,24 +29,117 @@
 17            package = node.names[0].name
 18        elif type_ == ast.ImportFrom:
 19            package = node.module
 20        if package:
 21            if "." in package:
 22                package = package[: package.find(".")]
 23            packages.append(package)
-24    packages = sorted(list(set(packages)))
-25    return sorted(list(set(packages)))
+24    return sorted(list(set(packages)))
+25
 26
-27
+27def remove_builtins(packages: list[str]) -> list[str]:
+28    """Remove built in packages/modules from a list of package names."""
+29    builtins = list(sys.stdlib_module_names)
+30    return filter(lambda x: x not in builtins, packages)
+31
+32
+33def scan(project_dir: Pathish = None, include_builtins: bool = False) -
+> dict:
+34    """Recursively scans a directory for python files to determine
+35    what packages are in use, as well as the version number if applicable.
+36
+37    Returns a dictionary where the keys are package names and
+38    the values are dictionaries with the keys `version` for the version
+number of the package
+39    if there is one (None if there isn't) and `files` for a list of the files
+that import the package.
+40
+41    :param project_dir: Can be an absolute or relative path to a directory or
+a single file (.py).
+42    If it is relative, it will be assumed to be relative to the current
+working directory.
+43    If an argument isn't given, the current working directory will be
+scanned.
+44    If the path doesn't exist, an empty dictionary is returned."""
+45    if not project_dir:
+46        project_dir = Pathier.cwd()
+47    elif type(project_dir) is str or project_dir.is_file():
+48        project_dir = Pathier(project_dir)
+49    if not project_dir.is_absolute():
+50        project_dir = project_dir.absolute()
+51
+52    # Raise error if project_dir doesn't exist
+53    if not project_dir.exists():
+54        raise FileNotFoundError(
+55            f"Can't scan directory that doesn't exist: {project_dir}"
+56        )
+57    # You can scan a non python file one at a time if you reeeally want to.
+58    if project_dir.is_file():
+59        files = [project_dir]
+60    else:
+61        files = list(project_dir.rglob("*.py"))
+62
+63    bar = ProgBar(len(files), width_ratio=0.33)
+64    used_packages = {}
+65    for file in files:
+66        bar.display(suffix=f"Scanning {file.name}")
+67        source = file.read_text(encoding="utf-8")
+68        packages = get_packages_from_source(source)
+69        if not include_builtins:
+70            packages = remove_builtins(packages)
+71        for package in packages:
+72            if file.with_stem(package) not in files:
+73                if (
+74                    package in used_packages
+75                    and str(file) not in used_packages[package]["files"]
+76                ):
+77                    used_packages[package]["files"].append(str(file))
+78                else:
+79                    try:
+80                        package_version = importlib.metadata.version(package)
+81                    except ModuleNotFoundError:
+82                        package_version = None
+83                    except Exception as e:
+84                        print(e)
+85                        package_version = None
+86                    used_packages[package] = {
+87                        "files": [str(file)],
+88                        "version": package_version,
+89                    }
+90    return used_packages
+  ⁰
+def get_packages_from_source(source: str) -> list[str]: View Source
+10def get_packages_from_source(source: str) -> list[str]:
+11    """Scan `source` and extract the names of imported packages/modules."""
+12    tree = ast.parse(source)
+13    packages = []
+14    for node in ast.walk(tree):
+15        type_ = type(node)
+16        package = ""
+17        if type_ == ast.Import:
+18            package = node.names[0].name
+19        elif type_ == ast.ImportFrom:
+20            package = node.module
+21        if package:
+22            if "." in package:
+23                package = package[: package.find(".")]
+24            packages.append(package)
+25    return sorted(list(set(packages)))
+Scan source and extract the names of imported packages/modules.
+  ⁰
+def remove_builtins(packages: list[str]) -> list[str]: View Source
 28def remove_builtins(packages: list[str]) -> list[str]:
 29    """Remove built in packages/modules from a list of package names."""
 30    builtins = list(sys.stdlib_module_names)
 31    return filter(lambda x: x not in builtins, packages)
-32
-33
+Remove built in packages/modules from a list of package names.
+  ⁰
+def scan(
+project_dir: pathier.pathier.Pathier | pathlib.Path | str = None,
+include_builtins: bool = False) -> dict: View Source
 34def scan(project_dir: Pathish = None, include_builtins: bool = False) -
 > dict:
 35    """Recursively scans a directory for python files to determine
 36    what packages are in use, as well as the version number if applicable.
 37
 38    Returns a dictionary where the keys are package names and
 39    the values are dictionaries with the keys `version` for the version
@@ -103,109 +196,14 @@
 85                        print(e)
 86                        package_version = None
 87                    used_packages[package] = {
 88                        "files": [str(file)],
 89                        "version": package_version,
 90                    }
 91    return used_packages
-  ⁰
-def get_packages_from_source(source: str) -> list[str]: View Source
-10def get_packages_from_source(source: str) -> list[str]:
-11    """Scan `source` and extract the names of imported packages/modules."""
-12    tree = ast.parse(source)
-13    packages = []
-14    for node in ast.walk(tree):
-15        type_ = type(node)
-16        package = ""
-17        if type_ == ast.Import:
-18            package = node.names[0].name
-19        elif type_ == ast.ImportFrom:
-20            package = node.module
-21        if package:
-22            if "." in package:
-23                package = package[: package.find(".")]
-24            packages.append(package)
-25    packages = sorted(list(set(packages)))
-26    return sorted(list(set(packages)))
-Scan source and extract the names of imported packages/modules.
-  ⁰
-def remove_builtins(packages: list[str]) -> list[str]: View Source
-29def remove_builtins(packages: list[str]) -> list[str]:
-30    """Remove built in packages/modules from a list of package names."""
-31    builtins = list(sys.stdlib_module_names)
-32    return filter(lambda x: x not in builtins, packages)
-Remove built in packages/modules from a list of package names.
-  ⁰
-def scan(
-project_dir: pathier.pathier.Pathier | pathlib.Path | str = None,
-include_builtins: bool = False) -> dict: View Source
-35def scan(project_dir: Pathish = None, include_builtins: bool = False) -
-> dict:
-36    """Recursively scans a directory for python files to determine
-37    what packages are in use, as well as the version number if applicable.
-38
-39    Returns a dictionary where the keys are package names and
-40    the values are dictionaries with the keys `version` for the version
-number of the package
-41    if there is one (None if there isn't) and `files` for a list of the files
-that import the package.
-42
-43    :param project_dir: Can be an absolute or relative path to a directory or
-a single file (.py).
-44    If it is relative, it will be assumed to be relative to the current
-working directory.
-45    If an argument isn't given, the current working directory will be
-scanned.
-46    If the path doesn't exist, an empty dictionary is returned."""
-47    if not project_dir:
-48        project_dir = Pathier.cwd()
-49    elif type(project_dir) is str or project_dir.is_file():
-50        project_dir = Pathier(project_dir)
-51    if not project_dir.is_absolute():
-52        project_dir = project_dir.absolute()
-53
-54    # Raise error if project_dir doesn't exist
-55    if not project_dir.exists():
-56        raise FileNotFoundError(
-57            f"Can't scan directory that doesn't exist: {project_dir}"
-58        )
-59    # You can scan a non python file one at a time if you reeeally want to.
-60    if project_dir.is_file():
-61        files = [project_dir]
-62    else:
-63        files = list(project_dir.rglob("*.py"))
-64
-65    bar = ProgBar(len(files), width_ratio=0.33)
-66    used_packages = {}
-67    for file in files:
-68        bar.display(suffix=f"Scanning {file.name}")
-69        source = file.read_text(encoding="utf-8")
-70        packages = get_packages_from_source(source)
-71        if not include_builtins:
-72            packages = remove_builtins(packages)
-73        for package in packages:
-74            if file.with_stem(package) not in files:
-75                if (
-76                    package in used_packages
-77                    and str(file) not in used_packages[package]["files"]
-78                ):
-79                    used_packages[package]["files"].append(str(file))
-80                else:
-81                    try:
-82                        package_version = importlib.metadata.version(package)
-83                    except ModuleNotFoundError:
-84                        package_version = None
-85                    except Exception as e:
-86                        print(e)
-87                        package_version = None
-88                    used_packages[package] = {
-89                        "files": [str(file)],
-90                        "version": package_version,
-91                    }
-92    return used_packages
 Recursively scans a directory for python files to determine what packages are
 in use, as well as the version number if applicable.
 Returns a dictionary where the keys are package names and the values are
 dictionaries with the keys version for the version number of the package if
 there is one (None if there isn't) and files for a list of the files that
 import the package.
 * Parameters *
```

### Comparing `packagelister-1.6.0/docs/packagelister/packagelister_cli.html` & `packagelister-1.6.1/docs/packagelister/packagelister_cli.html`

 * *Files 2% similar despite different names*

```diff
@@ -118,48 +118,49 @@
 </span><span id="L-62"><a href="#L-62"><span class="linenos"> 62</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
 </span><span id="L-63"><a href="#L-63"><span class="linenos"> 63</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
 </span><span id="L-64"><a href="#L-64"><span class="linenos"> 64</span></a>
 </span><span id="L-65"><a href="#L-65"><span class="linenos"> 65</span></a>        <span class="k">return</span> <span class="n">args</span>
 </span><span id="L-66"><a href="#L-66"><span class="linenos"> 66</span></a>
 </span><span id="L-67"><a href="#L-67"><span class="linenos"> 67</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
 </span><span id="L-68"><a href="#L-68"><span class="linenos"> 68</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">scan</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">include_builtins</span><span class="p">)</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_requirements</span><span class="p">:</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>        <span class="n">req_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">/</span> <span class="s2">&quot;requirements.txt&quot;</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="n">requirements</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="n">args</span><span class="o">.</span><span class="n">versions</span><span class="si">}{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>            <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">versions</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>            <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>            <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>            <span class="k">else</span> <span class="n">package</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>        <span class="p">)</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="k">for</span> <span class="n">mapping</span> <span class="ow">in</span> <span class="n">pipmappings</span><span class="p">:</span>
-</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>            <span class="n">requirements</span> <span class="o">=</span> <span class="n">requirements</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">mapping</span><span class="p">,</span> <span class="n">pipmappings</span><span class="p">[</span><span class="n">mapping</span><span class="p">])</span>
-</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>        <span class="n">req_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">requirements</span><span class="p">)</span>
-</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">==</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">:</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
-</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
-</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>    <span class="p">}</span>
-</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>
-</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">show_files</span><span class="p">:</span>
-</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>        <span class="n">longest_key</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">)</span>
-</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="p">(</span><span class="n">longest_key</span><span class="o">-</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span><span class="o">+</span><span class="mi">4</span><span class="p">)</span><span class="si">}{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">relative_to</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>        <span class="p">]</span>
-</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>
-</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Packages used in </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
-</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>        <span class="o">*</span><span class="n">packages</span><span class="p">,</span>
-</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>        <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>    <span class="p">)</span>
-</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>
+</span><span id="L-69"><a href="#L-69"><span class="linenos"> 69</span></a>    <span class="n">packages</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos"> 70</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_requirements</span><span class="p">:</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos"> 71</span></a>        <span class="n">req_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">/</span> <span class="s2">&quot;requirements.txt&quot;</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos"> 72</span></a>        <span class="n">requirements</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos"> 73</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="n">args</span><span class="o">.</span><span class="n">versions</span><span class="si">}{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos"> 74</span></a>            <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">versions</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos"> 75</span></a>            <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos"> 76</span></a>            <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos"> 77</span></a>            <span class="k">else</span> <span class="n">package</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos"> 78</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos"> 79</span></a>        <span class="p">)</span>
+</span><span id="L-80"><a href="#L-80"><span class="linenos"> 80</span></a>        <span class="k">for</span> <span class="n">mapping</span> <span class="ow">in</span> <span class="n">pipmappings</span><span class="p">:</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos"> 81</span></a>            <span class="n">requirements</span> <span class="o">=</span> <span class="n">requirements</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">mapping</span><span class="p">,</span> <span class="n">pipmappings</span><span class="p">[</span><span class="n">mapping</span><span class="p">])</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos"> 82</span></a>        <span class="n">req_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">requirements</span><span class="p">)</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos"> 83</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos"> 84</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">==</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">:</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos"> 85</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos"> 86</span></a>    <span class="p">}</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos"> 87</span></a>
+</span><span id="L-88"><a href="#L-88"><span class="linenos"> 88</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">show_files</span><span class="p">:</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos"> 89</span></a>        <span class="n">longest_key</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">)</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos"> 90</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos"> 91</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="p">(</span><span class="n">longest_key</span><span class="o">-</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span><span class="o">+</span><span class="mi">4</span><span class="p">)</span><span class="si">}{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">relative_to</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos"> 92</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos"> 93</span></a>        <span class="p">]</span>
+</span><span id="L-94"><a href="#L-94"><span class="linenos"> 94</span></a>
+</span><span id="L-95"><a href="#L-95"><span class="linenos"> 95</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Packages used in </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos"> 96</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-97"><a href="#L-97"><span class="linenos"> 97</span></a>        <span class="o">*</span><span class="n">packages</span><span class="p">,</span>
+</span><span id="L-98"><a href="#L-98"><span class="linenos"> 98</span></a>        <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="L-99"><a href="#L-99"><span class="linenos"> 99</span></a>    <span class="p">)</span>
 </span><span id="L-100"><a href="#L-100"><span class="linenos">100</span></a>
-</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a>    <span class="n">main</span><span class="p">()</span>
+</span><span id="L-101"><a href="#L-101"><span class="linenos">101</span></a>
+</span><span id="L-102"><a href="#L-102"><span class="linenos">102</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-103"><a href="#L-103"><span class="linenos">103</span></a>    <span class="n">main</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="main">
                             <input id="main-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -167,100 +168,101 @@
         <span class="def">def</span>
         <span class="name">main</span><span class="signature pdoc-code condensed">(<span class="return-annotation">):</span></span>
 
                 <label class="view-source-button" for="main-view-source"><span>View Source</span></label>
 
     </div>
     <a class="headerlink" href="#main"></a>
-            <div class="pdoc-code codehilite"><pre><span></span><span id="main-14"><a href="#main-14"><span class="linenos">14</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
-</span><span id="main-15"><a href="#main-15"><span class="linenos">15</span></a>    <span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
-</span><span id="main-16"><a href="#main-16"><span class="linenos">16</span></a>        <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
-</span><span id="main-17"><a href="#main-17"><span class="linenos">17</span></a>
-</span><span id="main-18"><a href="#main-18"><span class="linenos">18</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="main-19"><a href="#main-19"><span class="linenos">19</span></a>            <span class="s2">&quot;project_path&quot;</span><span class="p">,</span>
-</span><span id="main-20"><a href="#main-20"><span class="linenos">20</span></a>            <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
-</span><span id="main-21"><a href="#main-21"><span class="linenos">21</span></a>            <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="main-22"><a href="#main-22"><span class="linenos">22</span></a>            <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="main-23"><a href="#main-23"><span class="linenos">23</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The project directory path to scan. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="main-24"><a href="#main-24"><span class="linenos">24</span></a>        <span class="p">)</span>
-</span><span id="main-25"><a href="#main-25"><span class="linenos">25</span></a>
-</span><span id="main-26"><a href="#main-26"><span class="linenos">26</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="main-27"><a href="#main-27"><span class="linenos">27</span></a>            <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
-</span><span id="main-28"><a href="#main-28"><span class="linenos">28</span></a>            <span class="s2">&quot;--show_files&quot;</span><span class="p">,</span>
-</span><span id="main-29"><a href="#main-29"><span class="linenos">29</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="main-30"><a href="#main-30"><span class="linenos">30</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Show which files imported each of the packages. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="main-31"><a href="#main-31"><span class="linenos">31</span></a>        <span class="p">)</span>
-</span><span id="main-32"><a href="#main-32"><span class="linenos">32</span></a>
-</span><span id="main-33"><a href="#main-33"><span class="linenos">33</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="main-34"><a href="#main-34"><span class="linenos">34</span></a>            <span class="s2">&quot;-g&quot;</span><span class="p">,</span>
-</span><span id="main-35"><a href="#main-35"><span class="linenos">35</span></a>            <span class="s2">&quot;--generate_requirements&quot;</span><span class="p">,</span>
-</span><span id="main-36"><a href="#main-36"><span class="linenos">36</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="main-37"><a href="#main-37"><span class="linenos">37</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate a requirements.txt file in --project_path. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="main-38"><a href="#main-38"><span class="linenos">38</span></a>        <span class="p">)</span>
-</span><span id="main-39"><a href="#main-39"><span class="linenos">39</span></a>
-</span><span id="main-40"><a href="#main-40"><span class="linenos">40</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="main-41"><a href="#main-41"><span class="linenos">41</span></a>            <span class="s2">&quot;-v&quot;</span><span class="p">,</span>
-</span><span id="main-42"><a href="#main-42"><span class="linenos">42</span></a>            <span class="s2">&quot;--versions&quot;</span><span class="p">,</span>
-</span><span id="main-43"><a href="#main-43"><span class="linenos">43</span></a>            <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
-</span><span id="main-44"><a href="#main-44"><span class="linenos">44</span></a>            <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
-</span><span id="main-45"><a href="#main-45"><span class="linenos">45</span></a>            <span class="n">choices</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;==&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;~=&quot;</span><span class="p">],</span>
-</span><span id="main-46"><a href="#main-46"><span class="linenos">46</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When generating a requirements.txt file, include the versions of the packages using this relation.</span>
-</span><span id="main-47"><a href="#main-47"><span class="linenos">47</span></a><span class="s2">            (You may need to put quotes around some of the options.)&quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="main-48"><a href="#main-48"><span class="linenos">48</span></a>        <span class="p">)</span>
-</span><span id="main-49"><a href="#main-49"><span class="linenos">49</span></a>
-</span><span id="main-50"><a href="#main-50"><span class="linenos">50</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="main-51"><a href="#main-51"><span class="linenos">51</span></a>            <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
-</span><span id="main-52"><a href="#main-52"><span class="linenos">52</span></a>            <span class="s2">&quot;--include_builtins&quot;</span><span class="p">,</span>
-</span><span id="main-53"><a href="#main-53"><span class="linenos">53</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="main-54"><a href="#main-54"><span class="linenos">54</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include built in standard library modules. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="main-55"><a href="#main-55"><span class="linenos">55</span></a>        <span class="p">)</span>
-</span><span id="main-56"><a href="#main-56"><span class="linenos">56</span></a>
-</span><span id="main-57"><a href="#main-57"><span class="linenos">57</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="main-58"><a href="#main-58"><span class="linenos">58</span></a>
-</span><span id="main-59"><a href="#main-59"><span class="linenos">59</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">:</span>
-</span><span id="main-60"><a href="#main-60"><span class="linenos">60</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="main-61"><a href="#main-61"><span class="linenos">61</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="main-62"><a href="#main-62"><span class="linenos">62</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">)</span>
-</span><span id="main-63"><a href="#main-63"><span class="linenos">63</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
-</span><span id="main-64"><a href="#main-64"><span class="linenos">64</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
-</span><span id="main-65"><a href="#main-65"><span class="linenos">65</span></a>
-</span><span id="main-66"><a href="#main-66"><span class="linenos">66</span></a>        <span class="k">return</span> <span class="n">args</span>
-</span><span id="main-67"><a href="#main-67"><span class="linenos">67</span></a>
-</span><span id="main-68"><a href="#main-68"><span class="linenos">68</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-69"><a href="#main-69"><span class="linenos">69</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">scan</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">include_builtins</span><span class="p">)</span>
-</span><span id="main-70"><a href="#main-70"><span class="linenos">70</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_requirements</span><span class="p">:</span>
-</span><span id="main-71"><a href="#main-71"><span class="linenos">71</span></a>        <span class="n">req_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">/</span> <span class="s2">&quot;requirements.txt&quot;</span>
-</span><span id="main-72"><a href="#main-72"><span class="linenos">72</span></a>        <span class="n">requirements</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="main-73"><a href="#main-73"><span class="linenos">73</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="n">args</span><span class="o">.</span><span class="n">versions</span><span class="si">}{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="main-74"><a href="#main-74"><span class="linenos">74</span></a>            <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">versions</span>
-</span><span id="main-75"><a href="#main-75"><span class="linenos">75</span></a>            <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="main-76"><a href="#main-76"><span class="linenos">76</span></a>            <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="main-77"><a href="#main-77"><span class="linenos">77</span></a>            <span class="k">else</span> <span class="n">package</span>
-</span><span id="main-78"><a href="#main-78"><span class="linenos">78</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
-</span><span id="main-79"><a href="#main-79"><span class="linenos">79</span></a>        <span class="p">)</span>
-</span><span id="main-80"><a href="#main-80"><span class="linenos">80</span></a>        <span class="k">for</span> <span class="n">mapping</span> <span class="ow">in</span> <span class="n">pipmappings</span><span class="p">:</span>
-</span><span id="main-81"><a href="#main-81"><span class="linenos">81</span></a>            <span class="n">requirements</span> <span class="o">=</span> <span class="n">requirements</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">mapping</span><span class="p">,</span> <span class="n">pipmappings</span><span class="p">[</span><span class="n">mapping</span><span class="p">])</span>
-</span><span id="main-82"><a href="#main-82"><span class="linenos">82</span></a>        <span class="n">req_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">requirements</span><span class="p">)</span>
-</span><span id="main-83"><a href="#main-83"><span class="linenos">83</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{</span>
-</span><span id="main-84"><a href="#main-84"><span class="linenos">84</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">==</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">:</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
-</span><span id="main-85"><a href="#main-85"><span class="linenos">85</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
-</span><span id="main-86"><a href="#main-86"><span class="linenos">86</span></a>    <span class="p">}</span>
-</span><span id="main-87"><a href="#main-87"><span class="linenos">87</span></a>
-</span><span id="main-88"><a href="#main-88"><span class="linenos">88</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">show_files</span><span class="p">:</span>
-</span><span id="main-89"><a href="#main-89"><span class="linenos">89</span></a>        <span class="n">longest_key</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">)</span>
-</span><span id="main-90"><a href="#main-90"><span class="linenos">90</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="main-91"><a href="#main-91"><span class="linenos">91</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="p">(</span><span class="n">longest_key</span><span class="o">-</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span><span class="o">+</span><span class="mi">4</span><span class="p">)</span><span class="si">}{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">relative_to</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="main-92"><a href="#main-92"><span class="linenos">92</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="main-93"><a href="#main-93"><span class="linenos">93</span></a>        <span class="p">]</span>
-</span><span id="main-94"><a href="#main-94"><span class="linenos">94</span></a>
-</span><span id="main-95"><a href="#main-95"><span class="linenos">95</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Packages used in </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
-</span><span id="main-96"><a href="#main-96"><span class="linenos">96</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="main-97"><a href="#main-97"><span class="linenos">97</span></a>        <span class="o">*</span><span class="n">packages</span><span class="p">,</span>
-</span><span id="main-98"><a href="#main-98"><span class="linenos">98</span></a>        <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="main-99"><a href="#main-99"><span class="linenos">99</span></a>    <span class="p">)</span>
+            <div class="pdoc-code codehilite"><pre><span></span><span id="main-14"><a href="#main-14"><span class="linenos"> 14</span></a><span class="k">def</span> <span class="nf">main</span><span class="p">():</span>
+</span><span id="main-15"><a href="#main-15"><span class="linenos"> 15</span></a>    <span class="k">def</span> <span class="nf">get_args</span><span class="p">()</span> <span class="o">-&gt;</span> <span class="n">argparse</span><span class="o">.</span><span class="n">Namespace</span><span class="p">:</span>
+</span><span id="main-16"><a href="#main-16"><span class="linenos"> 16</span></a>        <span class="n">parser</span> <span class="o">=</span> <span class="n">argparse</span><span class="o">.</span><span class="n">ArgumentParser</span><span class="p">()</span>
+</span><span id="main-17"><a href="#main-17"><span class="linenos"> 17</span></a>
+</span><span id="main-18"><a href="#main-18"><span class="linenos"> 18</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-19"><a href="#main-19"><span class="linenos"> 19</span></a>            <span class="s2">&quot;project_path&quot;</span><span class="p">,</span>
+</span><span id="main-20"><a href="#main-20"><span class="linenos"> 20</span></a>            <span class="n">nargs</span><span class="o">=</span><span class="s2">&quot;?&quot;</span><span class="p">,</span>
+</span><span id="main-21"><a href="#main-21"><span class="linenos"> 21</span></a>            <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="main-22"><a href="#main-22"><span class="linenos"> 22</span></a>            <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="main-23"><a href="#main-23"><span class="linenos"> 23</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; The project directory path to scan. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-24"><a href="#main-24"><span class="linenos"> 24</span></a>        <span class="p">)</span>
+</span><span id="main-25"><a href="#main-25"><span class="linenos"> 25</span></a>
+</span><span id="main-26"><a href="#main-26"><span class="linenos"> 26</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-27"><a href="#main-27"><span class="linenos"> 27</span></a>            <span class="s2">&quot;-s&quot;</span><span class="p">,</span>
+</span><span id="main-28"><a href="#main-28"><span class="linenos"> 28</span></a>            <span class="s2">&quot;--show_files&quot;</span><span class="p">,</span>
+</span><span id="main-29"><a href="#main-29"><span class="linenos"> 29</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="main-30"><a href="#main-30"><span class="linenos"> 30</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Show which files imported each of the packages. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-31"><a href="#main-31"><span class="linenos"> 31</span></a>        <span class="p">)</span>
+</span><span id="main-32"><a href="#main-32"><span class="linenos"> 32</span></a>
+</span><span id="main-33"><a href="#main-33"><span class="linenos"> 33</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-34"><a href="#main-34"><span class="linenos"> 34</span></a>            <span class="s2">&quot;-g&quot;</span><span class="p">,</span>
+</span><span id="main-35"><a href="#main-35"><span class="linenos"> 35</span></a>            <span class="s2">&quot;--generate_requirements&quot;</span><span class="p">,</span>
+</span><span id="main-36"><a href="#main-36"><span class="linenos"> 36</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="main-37"><a href="#main-37"><span class="linenos"> 37</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate a requirements.txt file in --project_path. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-38"><a href="#main-38"><span class="linenos"> 38</span></a>        <span class="p">)</span>
+</span><span id="main-39"><a href="#main-39"><span class="linenos"> 39</span></a>
+</span><span id="main-40"><a href="#main-40"><span class="linenos"> 40</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-41"><a href="#main-41"><span class="linenos"> 41</span></a>            <span class="s2">&quot;-v&quot;</span><span class="p">,</span>
+</span><span id="main-42"><a href="#main-42"><span class="linenos"> 42</span></a>            <span class="s2">&quot;--versions&quot;</span><span class="p">,</span>
+</span><span id="main-43"><a href="#main-43"><span class="linenos"> 43</span></a>            <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="main-44"><a href="#main-44"><span class="linenos"> 44</span></a>            <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="main-45"><a href="#main-45"><span class="linenos"> 45</span></a>            <span class="n">choices</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;==&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;~=&quot;</span><span class="p">],</span>
+</span><span id="main-46"><a href="#main-46"><span class="linenos"> 46</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When generating a requirements.txt file, include the versions of the packages using this relation.</span>
+</span><span id="main-47"><a href="#main-47"><span class="linenos"> 47</span></a><span class="s2">            (You may need to put quotes around some of the options.)&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-48"><a href="#main-48"><span class="linenos"> 48</span></a>        <span class="p">)</span>
+</span><span id="main-49"><a href="#main-49"><span class="linenos"> 49</span></a>
+</span><span id="main-50"><a href="#main-50"><span class="linenos"> 50</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-51"><a href="#main-51"><span class="linenos"> 51</span></a>            <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="main-52"><a href="#main-52"><span class="linenos"> 52</span></a>            <span class="s2">&quot;--include_builtins&quot;</span><span class="p">,</span>
+</span><span id="main-53"><a href="#main-53"><span class="linenos"> 53</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="main-54"><a href="#main-54"><span class="linenos"> 54</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include built in standard library modules. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-55"><a href="#main-55"><span class="linenos"> 55</span></a>        <span class="p">)</span>
+</span><span id="main-56"><a href="#main-56"><span class="linenos"> 56</span></a>
+</span><span id="main-57"><a href="#main-57"><span class="linenos"> 57</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="main-58"><a href="#main-58"><span class="linenos"> 58</span></a>
+</span><span id="main-59"><a href="#main-59"><span class="linenos"> 59</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">:</span>
+</span><span id="main-60"><a href="#main-60"><span class="linenos"> 60</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="main-61"><a href="#main-61"><span class="linenos"> 61</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="main-62"><a href="#main-62"><span class="linenos"> 62</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Pathier</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">)</span>
+</span><span id="main-63"><a href="#main-63"><span class="linenos"> 63</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
+</span><span id="main-64"><a href="#main-64"><span class="linenos"> 64</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
+</span><span id="main-65"><a href="#main-65"><span class="linenos"> 65</span></a>
+</span><span id="main-66"><a href="#main-66"><span class="linenos"> 66</span></a>        <span class="k">return</span> <span class="n">args</span>
+</span><span id="main-67"><a href="#main-67"><span class="linenos"> 67</span></a>
+</span><span id="main-68"><a href="#main-68"><span class="linenos"> 68</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-69"><a href="#main-69"><span class="linenos"> 69</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">scan</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">include_builtins</span><span class="p">)</span>
+</span><span id="main-70"><a href="#main-70"><span class="linenos"> 70</span></a>    <span class="n">packages</span><span class="o">.</span><span class="n">pop</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
+</span><span id="main-71"><a href="#main-71"><span class="linenos"> 71</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_requirements</span><span class="p">:</span>
+</span><span id="main-72"><a href="#main-72"><span class="linenos"> 72</span></a>        <span class="n">req_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">/</span> <span class="s2">&quot;requirements.txt&quot;</span>
+</span><span id="main-73"><a href="#main-73"><span class="linenos"> 73</span></a>        <span class="n">requirements</span> <span class="o">=</span> <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="main-74"><a href="#main-74"><span class="linenos"> 74</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="n">args</span><span class="o">.</span><span class="n">versions</span><span class="si">}{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-75"><a href="#main-75"><span class="linenos"> 75</span></a>            <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">versions</span>
+</span><span id="main-76"><a href="#main-76"><span class="linenos"> 76</span></a>            <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-77"><a href="#main-77"><span class="linenos"> 77</span></a>            <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="main-78"><a href="#main-78"><span class="linenos"> 78</span></a>            <span class="k">else</span> <span class="n">package</span>
+</span><span id="main-79"><a href="#main-79"><span class="linenos"> 79</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="main-80"><a href="#main-80"><span class="linenos"> 80</span></a>        <span class="p">)</span>
+</span><span id="main-81"><a href="#main-81"><span class="linenos"> 81</span></a>        <span class="k">for</span> <span class="n">mapping</span> <span class="ow">in</span> <span class="n">pipmappings</span><span class="p">:</span>
+</span><span id="main-82"><a href="#main-82"><span class="linenos"> 82</span></a>            <span class="n">requirements</span> <span class="o">=</span> <span class="n">requirements</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="n">mapping</span><span class="p">,</span> <span class="n">pipmappings</span><span class="p">[</span><span class="n">mapping</span><span class="p">])</span>
+</span><span id="main-83"><a href="#main-83"><span class="linenos"> 83</span></a>        <span class="n">req_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span><span class="n">requirements</span><span class="p">)</span>
+</span><span id="main-84"><a href="#main-84"><span class="linenos"> 84</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{</span>
+</span><span id="main-85"><a href="#main-85"><span class="linenos"> 85</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">==</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">:</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
+</span><span id="main-86"><a href="#main-86"><span class="linenos"> 86</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="main-87"><a href="#main-87"><span class="linenos"> 87</span></a>    <span class="p">}</span>
+</span><span id="main-88"><a href="#main-88"><span class="linenos"> 88</span></a>
+</span><span id="main-89"><a href="#main-89"><span class="linenos"> 89</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">show_files</span><span class="p">:</span>
+</span><span id="main-90"><a href="#main-90"><span class="linenos"> 90</span></a>        <span class="n">longest_key</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">)</span>
+</span><span id="main-91"><a href="#main-91"><span class="linenos"> 91</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="main-92"><a href="#main-92"><span class="linenos"> 92</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="p">(</span><span class="n">longest_key</span><span class="o">-</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span><span class="o">+</span><span class="mi">4</span><span class="p">)</span><span class="si">}{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">Pathier</span><span class="p">(</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">relative_to</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-93"><a href="#main-93"><span class="linenos"> 93</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="main-94"><a href="#main-94"><span class="linenos"> 94</span></a>        <span class="p">]</span>
+</span><span id="main-95"><a href="#main-95"><span class="linenos"> 95</span></a>
+</span><span id="main-96"><a href="#main-96"><span class="linenos"> 96</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Packages used in </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
+</span><span id="main-97"><a href="#main-97"><span class="linenos"> 97</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="main-98"><a href="#main-98"><span class="linenos"> 98</span></a>        <span class="o">*</span><span class="n">packages</span><span class="p">,</span>
+</span><span id="main-99"><a href="#main-99"><span class="linenos"> 99</span></a>        <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="main-100"><a href="#main-100"><span class="linenos">100</span></a>    <span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -75,137 +75,140 @@
 _62        if not args.project_path.is_absolute():
 _63            args.project_path = args.project_path.absolute()
 _64
 _65        return args
 _66
 _67    args = get_args()
 _68    packages = scan(args.project_path, args.include_builtins)
-_69    if args.generate_requirements:
-_70        req_path = args.project_path / "requirements.txt"
-_71        requirements = "\n".join(
-_72            f"{package}{args.versions}{packages[package]['version']}"
-_73            if args.versions
-_74            else f"{package}"
-_75            if packages[package]["version"]
-_76            else package
-_77            for package in sorted(packages)
-_78        )
-_79        for mapping in pipmappings:
-_80            requirements = requirements.replace(mapping, pipmappings
+_69    packages.pop(args.project_path.stem, None)
+_70    if args.generate_requirements:
+_71        req_path = args.project_path / "requirements.txt"
+_72        requirements = "\n".join(
+_73            f"{package}{args.versions}{packages[package]['version']}"
+_74            if args.versions
+_75            else f"{package}"
+_76            if packages[package]["version"]
+_77            else package
+_78            for package in sorted(packages)
+_79        )
+_80        for mapping in pipmappings:
+_81            requirements = requirements.replace(mapping, pipmappings
 [mapping])
-_81        req_path.write_text(requirements)
-_82    packages = {
-_83        f"{package}=={packages[package]['version']}": packages[package]
+_82        req_path.write_text(requirements)
+_83    packages = {
+_84        f"{package}=={packages[package]['version']}": packages[package]
 ["files"]
-_84        for package in sorted(packages)
-_85    }
-_86
-_87    if args.show_files:
-_88        longest_key = max(len(package) for package in packages)
-_89        packages = [
-_90            f"{package}{' '*(longest_key-len(package)+4)}{', '.join(str
+_85        for package in sorted(packages)
+_86    }
+_87
+_88    if args.show_files:
+_89        longest_key = max(len(package) for package in packages)
+_90        packages = [
+_91            f"{package}{' '*(longest_key-len(package)+4)}{', '.join(str
 (Pathier(file).relative_to(args.project_path)) for file in packages[package])}"
-_91            for package in packages
-_92        ]
-_93
-_94    print(f"Packages used in {args.project_path.stem}:")
-_95    print(
-_96        *packages,
-_97        sep="\n",
-_98    )
-_99
+_92            for package in packages
+_93        ]
+_94
+_95    print(f"Packages used in {args.project_path.stem}:")
+_96    print(
+_97        *packages,
+_98        sep="\n",
+_99    )
 100
-101if __name__ == "__main__":
-102    main()
+101
+102if __name__ == "__main__":
+103    main()
   ⁰
 def main(): View Source
-14def main():
-15    def get_args() -> argparse.Namespace:
-16        parser = argparse.ArgumentParser()
-17
-18        parser.add_argument(
-19            "project_path",
-20            nargs="?",
-21            type=str,
-22            default=None,
-23            help=""" The project directory path to scan. """,
-24        )
-25
-26        parser.add_argument(
-27            "-s",
-28            "--show_files",
-29            action="store_true",
-30            help=""" Show which files imported each of the packages. """,
-31        )
-32
-33        parser.add_argument(
-34            "-g",
-35            "--generate_requirements",
-36            action="store_true",
-37            help=""" Generate a requirements.txt file in --project_path. """,
-38        )
-39
-40        parser.add_argument(
-41            "-v",
-42            "--versions",
-43            type=str,
-44            default=None,
-45            choices=["==", "<", "<=", ">", ">=", "~="],
-46            help=""" When generating a requirements.txt file, include the
+_14def main():
+_15    def get_args() -> argparse.Namespace:
+_16        parser = argparse.ArgumentParser()
+_17
+_18        parser.add_argument(
+_19            "project_path",
+_20            nargs="?",
+_21            type=str,
+_22            default=None,
+_23            help=""" The project directory path to scan. """,
+_24        )
+_25
+_26        parser.add_argument(
+_27            "-s",
+_28            "--show_files",
+_29            action="store_true",
+_30            help=""" Show which files imported each of the packages. """,
+_31        )
+_32
+_33        parser.add_argument(
+_34            "-g",
+_35            "--generate_requirements",
+_36            action="store_true",
+_37            help=""" Generate a requirements.txt file in --project_path.
+""",
+_38        )
+_39
+_40        parser.add_argument(
+_41            "-v",
+_42            "--versions",
+_43            type=str,
+_44            default=None,
+_45            choices=["==", "<", "<=", ">", ">=", "~="],
+_46            help=""" When generating a requirements.txt file, include the
 versions of the packages using this relation.
-47            (You may need to put quotes around some of the options.)""",
-48        )
-49
-50        parser.add_argument(
-51            "-i",
-52            "--include_builtins",
-53            action="store_true",
-54            help=""" Include built in standard library modules. """,
-55        )
-56
-57        args = parser.parse_args()
-58
-59        if not args.project_path:
-60            args.project_path = Pathier.cwd()
-61        else:
-62            args.project_path = Pathier(args.project_path)
-63        if not args.project_path.is_absolute():
-64            args.project_path = args.project_path.absolute()
-65
-66        return args
-67
-68    args = get_args()
-69    packages = scan(args.project_path, args.include_builtins)
-70    if args.generate_requirements:
-71        req_path = args.project_path / "requirements.txt"
-72        requirements = "\n".join(
-73            f"{package}{args.versions}{packages[package]['version']}"
-74            if args.versions
-75            else f"{package}"
-76            if packages[package]["version"]
-77            else package
-78            for package in sorted(packages)
-79        )
-80        for mapping in pipmappings:
-81            requirements = requirements.replace(mapping, pipmappings
+_47            (You may need to put quotes around some of the options.)""",
+_48        )
+_49
+_50        parser.add_argument(
+_51            "-i",
+_52            "--include_builtins",
+_53            action="store_true",
+_54            help=""" Include built in standard library modules. """,
+_55        )
+_56
+_57        args = parser.parse_args()
+_58
+_59        if not args.project_path:
+_60            args.project_path = Pathier.cwd()
+_61        else:
+_62            args.project_path = Pathier(args.project_path)
+_63        if not args.project_path.is_absolute():
+_64            args.project_path = args.project_path.absolute()
+_65
+_66        return args
+_67
+_68    args = get_args()
+_69    packages = scan(args.project_path, args.include_builtins)
+_70    packages.pop(args.project_path.stem, None)
+_71    if args.generate_requirements:
+_72        req_path = args.project_path / "requirements.txt"
+_73        requirements = "\n".join(
+_74            f"{package}{args.versions}{packages[package]['version']}"
+_75            if args.versions
+_76            else f"{package}"
+_77            if packages[package]["version"]
+_78            else package
+_79            for package in sorted(packages)
+_80        )
+_81        for mapping in pipmappings:
+_82            requirements = requirements.replace(mapping, pipmappings
 [mapping])
-82        req_path.write_text(requirements)
-83    packages = {
-84        f"{package}=={packages[package]['version']}": packages[package]
+_83        req_path.write_text(requirements)
+_84    packages = {
+_85        f"{package}=={packages[package]['version']}": packages[package]
 ["files"]
-85        for package in sorted(packages)
-86    }
-87
-88    if args.show_files:
-89        longest_key = max(len(package) for package in packages)
-90        packages = [
-91            f"{package}{' '*(longest_key-len(package)+4)}{', '.join(str
+_86        for package in sorted(packages)
+_87    }
+_88
+_89    if args.show_files:
+_90        longest_key = max(len(package) for package in packages)
+_91        packages = [
+_92            f"{package}{' '*(longest_key-len(package)+4)}{', '.join(str
 (Pathier(file).relative_to(args.project_path)) for file in packages[package])}"
-92            for package in packages
-93        ]
-94
-95    print(f"Packages used in {args.project_path.stem}:")
-96    print(
-97        *packages,
-98        sep="\n",
-99    )
+_93            for package in packages
+_94        ]
+_95
+_96    print(f"Packages used in {args.project_path.stem}:")
+_97    print(
+_98        *packages,
+_99        sep="\n",
+100    )
```

### Comparing `packagelister-1.6.0/docs/packagelister/whouses.html` & `packagelister-1.6.1/docs/packagelister/whouses.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.0/src/packagelister/packagelister.py` & `packagelister-1.6.1/src/packagelister/packagelister.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,14 @@
             package = node.names[0].name
         elif type_ == ast.ImportFrom:
             package = node.module
         if package:
             if "." in package:
                 package = package[: package.find(".")]
             packages.append(package)
-    packages = sorted(list(set(packages)))
     return sorted(list(set(packages)))
 
 
 def remove_builtins(packages: list[str]) -> list[str]:
     """Remove built in packages/modules from a list of package names."""
     builtins = list(sys.stdlib_module_names)
     return filter(lambda x: x not in builtins, packages)
```

### Comparing `packagelister-1.6.0/src/packagelister/packagelister_cli.py` & `packagelister-1.6.1/src/packagelister/packagelister_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
         if not args.project_path.is_absolute():
             args.project_path = args.project_path.absolute()
 
         return args
 
     args = get_args()
     packages = scan(args.project_path, args.include_builtins)
+    packages.pop(args.project_path.stem, None)
     if args.generate_requirements:
         req_path = args.project_path / "requirements.txt"
         requirements = "\n".join(
             f"{package}{args.versions}{packages[package]['version']}"
             if args.versions
             else f"{package}"
             if packages[package]["version"]
```

### Comparing `packagelister-1.6.0/src/packagelister/whouses.py` & `packagelister-1.6.1/src/packagelister/whouses.py`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.0/LICENSE.txt` & `packagelister-1.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.0/README.md` & `packagelister-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `packagelister-1.6.0/pyproject.toml` & `packagelister-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 00000070: 0d0a 6175 7468 6f72 7320 3d20 5b7b 6e61  ..authors = [{na
 00000080: 6d65 3d22 4d61 7474 204d 616e 6573 227d  me="Matt Manes"}
 00000090: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
 000000a0: 2022 4465 7465 726d 696e 6520 7768 6174   "Determine what
 000000b0: 2033 7264 2d70 6172 7479 2070 6163 6b61   3rd-party packa
 000000c0: 6765 7320 6120 7072 6f6a 6563 7420 696d  ges a project im
 000000d0: 706f 7274 732e 220d 0a76 6572 7369 6f6e  ports."..version
-000000e0: 203d 2022 312e 362e 3022 0d0a 7265 7175   = "1.6.0"..requ
+000000e0: 203d 2022 312e 362e 3122 0d0a 7265 7175   = "1.6.1"..requ
 000000f0: 6972 6573 2d70 7974 686f 6e20 3d20 223e  ires-python = ">
 00000100: 3d33 2e31 3022 0d0a 6465 7065 6e64 656e  =3.10"..dependen
 00000110: 6369 6573 203d 205b 2270 7269 6e74 6275  cies = ["printbu
 00000120: 6464 6965 7322 2c20 2270 7974 6573 7422  ddies", "pytest"
 00000130: 2c20 2270 6174 6869 6572 225d 0d0a 7265  , "pathier"]..re
 00000140: 6164 6d65 203d 2022 5245 4144 4d45 2e6d  adme = "README.m
 00000150: 6422 0d0a 6b65 7977 6f72 6473 203d 205b  d"..keywords = [
```

### Comparing `packagelister-1.6.0/PKG-INFO` & `packagelister-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagelister
-Version: 1.6.0
+Version: 1.6.1
 Summary: Determine what 3rd-party packages a project imports.
 Project-URL: Homepage, https://github.com/matt-manes/packagelister
 Project-URL: Documentation, https://github.com/matt-manes/packagelister/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/packagelister/tree/main/src/packagelister
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: import,module,package
```

