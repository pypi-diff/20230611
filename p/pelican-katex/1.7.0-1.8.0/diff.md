# Comparing `tmp/pelican_katex-1.7.0.tar.gz` & `tmp/pelican_katex-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pelican_katex-1.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pelican_katex-1.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pelican_katex-1.7.0.tar` & `pelican_katex-1.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       58 2023-05-19 10:58:13.918511 pelican_katex-1.7.0/.gitignore
--rw-r--r--   0        0        0      572 2023-05-19 11:26:48.061015 pelican_katex-1.7.0/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-05-19 10:58:13.918511 pelican_katex-1.7.0/LICENSE
--rw-r--r--   0        0        0     4715 2023-05-19 10:58:13.918511 pelican_katex-1.7.0/README.md
--rw-r--r--   0        0        0      144 2023-05-19 11:27:28.047730 pelican_katex-1.7.0/pelican_katex/__init__.py
--rw-r--r--   0        0        0   629396 2023-04-28 11:42:18.000000 pelican_katex-1.7.0/pelican_katex/katex.js
--rw-r--r--   0        0        0     3606 2023-05-19 11:24:24.927500 pelican_katex-1.7.0/pelican_katex/markdown.py
--rw-r--r--   0        0        0     1888 2023-05-19 11:24:24.927500 pelican_katex-1.7.0/pelican_katex/plugin.py
--rw-r--r--   0        0        0     4044 2023-05-19 10:58:13.921844 pelican_katex-1.7.0/pelican_katex/render-katex.js
--rw-r--r--   0        0        0    10541 2023-05-19 10:58:13.921844 pelican_katex-1.7.0/pelican_katex/rendering.py
--rw-r--r--   0        0        0     1565 2023-05-19 11:24:24.927500 pelican_katex-1.7.0/pelican_katex/restructuredtext.py
--rw-r--r--   0        0        0      851 2023-05-19 11:24:24.924167 pelican_katex-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      206 2023-05-19 10:58:13.921844 pelican_katex-1.7.0/test/conftest.py
--rw-r--r--   0        0        0     2684 2023-05-19 10:58:13.921844 pelican_katex-1.7.0/test/html_template.py
--rw-r--r--   0        0        0     1637 2023-05-19 10:58:13.921844 pelican_katex-1.7.0/test/test_markdown.py
--rw-r--r--   0        0        0     5637 1970-01-01 00:00:00.000000 pelican_katex-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0       58 2023-05-19 10:58:13.918511 pelican_katex-1.8.0/.gitignore
+-rw-r--r--   0        0        0      645 2023-06-11 07:24:12.051475 pelican_katex-1.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-19 10:58:13.918511 pelican_katex-1.8.0/LICENSE
+-rw-r--r--   0        0        0     4801 2023-06-11 07:22:41.648749 pelican_katex-1.8.0/README.md
+-rw-r--r--   0        0        0      144 2023-06-11 07:24:18.252096 pelican_katex-1.8.0/pelican_katex/__init__.py
+-rw-r--r--   0        0        0   629396 2023-04-28 11:42:18.000000 pelican_katex-1.8.0/pelican_katex/katex.js
+-rw-r--r--   0        0        0     4058 2023-06-11 07:19:59.880631 pelican_katex-1.8.0/pelican_katex/markdown.py
+-rw-r--r--   0        0        0     1888 2023-05-19 11:24:24.927500 pelican_katex-1.8.0/pelican_katex/plugin.py
+-rw-r--r--   0        0        0     4044 2023-05-19 10:58:13.921844 pelican_katex-1.8.0/pelican_katex/render-katex.js
+-rw-r--r--   0        0        0    10541 2023-05-19 10:58:13.921844 pelican_katex-1.8.0/pelican_katex/rendering.py
+-rw-r--r--   0        0        0     1565 2023-05-19 11:24:24.927500 pelican_katex-1.8.0/pelican_katex/restructuredtext.py
+-rw-r--r--   0        0        0      851 2023-05-19 11:24:24.924167 pelican_katex-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      206 2023-05-19 10:58:13.921844 pelican_katex-1.8.0/test/conftest.py
+-rw-r--r--   0        0        0     2684 2023-05-19 10:58:13.921844 pelican_katex-1.8.0/test/html_template.py
+-rw-r--r--   0        0        0     2212 2023-06-11 07:18:58.402214 pelican_katex-1.8.0/test/test_markdown.py
+-rw-r--r--   0        0        0     5723 1970-01-01 00:00:00.000000 pelican_katex-1.8.0/PKG-INFO
```

### Comparing `pelican_katex-1.7.0/CHANGELOG.md` & `pelican_katex-1.8.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog
 
+## 1.8.0
+
+- Allow escaping dollar delimiters in markdown with backslash
+
 ## 1.7.0
 
 - Update the bundled katex to 0.16.7
 
 ## 1.6.1
 
 - Serialize the namespace of `math` elements in markdown properly
```

### Comparing `pelican_katex-1.7.0/LICENSE` & `pelican_katex-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.7.0/README.md` & `pelican_katex-1.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,16 +45,17 @@
     \int \textrm{math block}.
 
 # markdown
 
 In markdown you get inline math in between $ signs, like $f(x) = \sqrt{x}$.
 Note, that $ only creates a math environment if it is preceded by whitespace
 or at the beginning of a block and followed by some non-whitespace character.
-This is necessary so that you can still write about the 5$ in your pocket.
-Block math is triggered with
+This is necessary so that you can still write about the 5$ in your pocket. To
+write a dollar sign preceded by whitespace, escape it with a backslash as in
+\$10. Block math is triggered with
 
 $$\int \textrm{math block}.$$
 
 Math blocks can have linebreaks but no empty lines.
 ```
 
 ## Configuration
```

### Comparing `pelican_katex-1.7.0/pelican_katex/katex.js` & `pelican_katex-1.8.0/pelican_katex/katex.js`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.7.0/pelican_katex/markdown.py` & `pelican_katex-1.8.0/pelican_katex/markdown.py`

 * *Files 7% similar despite different names*

```diff
@@ -79,12 +79,28 @@
         for elem in node.iter():
             if elem.text is not None:
                 elem.text = AtomicString(elem.text)
 
         return node, match_start, match_end
 
 
+ESCAPE_PATTERN = r"\\(?P<delimiter>\$\$?)"
+
+
+class DollarEscapePattern(InlineProcessor):
+    """Allow escaping dollar delimiters with backslash."""
+
+    def __init__(self, md=None):
+        super().__init__(pattern=ESCAPE_PATTERN, md=md)
+
+    def handleMatch(self, m, data):
+        delimiter = m.group("delimiter")
+
+        return delimiter, m.start(), m.end()
+
+
 class KatexExtension(Extension):
     def extendMarkdown(self, md):
         # render_math uses priority 186 as well because apparently it needs to be
         # higher than 180 which some "escape" extension uses.
         md.inlinePatterns.register(KatexPattern(md), "katex", 186)
+        md.inlinePatterns.register(DollarEscapePattern(md), "katex-dollar-escape", 185)
```

### Comparing `pelican_katex-1.7.0/pelican_katex/plugin.py` & `pelican_katex-1.8.0/pelican_katex/plugin.py`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.7.0/pelican_katex/render-katex.js` & `pelican_katex-1.8.0/pelican_katex/render-katex.js`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.7.0/pelican_katex/rendering.py` & `pelican_katex-1.8.0/pelican_katex/rendering.py`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.7.0/pelican_katex/restructuredtext.py` & `pelican_katex-1.8.0/pelican_katex/restructuredtext.py`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.7.0/pyproject.toml` & `pelican_katex-1.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.7.0/test/html_template.py` & `pelican_katex-1.8.0/test/html_template.py`

 * *Files identical despite different names*

### Comparing `pelican_katex-1.7.0/test/test_markdown.py` & `pelican_katex-1.8.0/test/test_markdown.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import markdown
+from pelican_katex.markdown import KatexExtension
 
 from html_template import HTMLTemplate
-from pelican_katex.markdown import KatexExtension
 
 
 def test_renders_standalone_inline_math():
     input = "Hello $x^2$ world!"
     output = markdown.markdown(input, extensions=[KatexExtension()])
 
     template = HTMLTemplate('<p>Hello <span class="katex">...</span> world!</p>')
@@ -32,21 +32,39 @@
     input = "I have 10$."
     output = markdown.markdown(input, extensions=[KatexExtension()])
 
     template = HTMLTemplate("<p>I have 10$.</p>")
     assert template == output
 
 
-def test_double_dollar_renders_inline_math():
+def test_double_dollar_renders_display_math():
     input = "$$x^2$$"
     output = markdown.markdown(input, extensions=[KatexExtension()])
 
     template = HTMLTemplate('<p><span class="katex-display">...</span></p>')
     assert template == output
 
 
 def test_preamble_block_does_not_show_up():
     input = "$$@\\def\\pelican{x^2}$$\nUse it\n$$\\pelican = 1$$"
     output = markdown.markdown(input, extensions=[KatexExtension()])
 
     template = HTMLTemplate('<p>\nUse it\n<span class="katex-display">...</span></p>')
     assert template == output
+
+
+def test_backslash_escapes_dollar_delimiter():
+    input = r"My bank account has \$1 and my wallet \$0."
+    output = markdown.markdown(input, extensions=[KatexExtension()])
+
+    target = input.replace("\\", "")
+    template = HTMLTemplate(f"<p>{target}</p>")
+    assert template == output
+
+
+def test_backslash_escapes_double_dollar_delimiter():
+    input = r"A is \$$1 and B is \$$10."
+    output = markdown.markdown(input, extensions=[KatexExtension()])
+
+    target = input.replace("\\", "")
+    template = HTMLTemplate(f"<p>{target}</p>")
+    assert template == output
```

### Comparing `pelican_katex-1.7.0/PKG-INFO` & `pelican_katex-1.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pelican-katex
-Version: 1.7.0
+Version: 1.8.0
 Summary: LaTeX pre-rendering for pelican with katex.js
 Author-email: Marten Lienen <marten.lienen@gmail.com>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Pelican :: Plugins
@@ -69,16 +69,17 @@
     \int \textrm{math block}.
 
 # markdown
 
 In markdown you get inline math in between $ signs, like $f(x) = \sqrt{x}$.
 Note, that $ only creates a math environment if it is preceded by whitespace
 or at the beginning of a block and followed by some non-whitespace character.
-This is necessary so that you can still write about the 5$ in your pocket.
-Block math is triggered with
+This is necessary so that you can still write about the 5$ in your pocket. To
+write a dollar sign preceded by whitespace, escape it with a backslash as in
+\$10. Block math is triggered with
 
 $$\int \textrm{math block}.$$
 
 Math blocks can have linebreaks but no empty lines.
 ```
 
 ## Configuration
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_cy7kjmuf_/tmpcw6mgm3r_TarContainer/0/15", line 183, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_cy7kjmuf_/tmpcw6mgm3r_TarContainer/0/15", line 183, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pelican-katex Version: 1.7.0 Summary: LaTeX pre-
+Metadata-Version: 2.1 Name: pelican-katex Version: 1.8.0 Summary: LaTeX pre-
 rendering for pelican with katex.js Author-email: Marten Lienen
 lienen@gmail.com> Requires-Python: >= 3.6 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Framework
 :: Pelican :: Plugins Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Science/Research Classifier: Intended Audience :: Education Requires-Dist:
```

