# Comparing `tmp/mistletoe-1.0.1.tar.gz` & `tmp/mistletoe-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistletoe-1.0.1.tar", last modified: Fri Jan 20 21:09:44 2023, max compression
+gzip compressed data, was "mistletoe-1.1.0.tar", last modified: Sun Jun 11 14:49:44 2023, max compression
```

## Comparing `mistletoe-1.0.1.tar` & `mistletoe-1.1.0.tar`

### file list

```diff
@@ -1,51 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-01-20 21:09:44.938606 mistletoe-1.0.1/
--rw-rw-rw-   0        0        0     1062 2020-06-28 12:58:34.000000 mistletoe-1.0.1/LICENSE
--rw-rw-rw-   0        0        0       16 2020-06-28 12:58:34.000000 mistletoe-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1160 2023-01-20 21:09:44.937608 mistletoe-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     8484 2023-01-10 08:02:41.000000 mistletoe-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-20 21:09:44.875580 mistletoe-1.0.1/mistletoe/
--rw-rw-rw-   0        0        0      715 2023-01-20 20:53:21.000000 mistletoe-1.0.1/mistletoe/__init__.py
--rw-rw-rw-   0        0        0      219 2020-06-28 12:58:34.000000 mistletoe-1.0.1/mistletoe/__main__.py
--rw-rw-rw-   0        0        0     1214 2022-07-04 20:11:46.000000 mistletoe-1.0.1/mistletoe/ast_renderer.py
--rw-rw-rw-   0        0        0     7567 2023-01-10 08:01:32.000000 mistletoe-1.0.1/mistletoe/base_renderer.py
--rw-rw-rw-   0        0        0    36196 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/block_token.py
--rw-rw-rw-   0        0        0     2531 2022-04-09 16:39:05.000000 mistletoe-1.0.1/mistletoe/block_tokenizer.py
--rw-rw-rw-   0        0        0     2881 2022-07-04 20:11:46.000000 mistletoe-1.0.1/mistletoe/cli.py
-drwxrwxrwx   0        0        0        0 2023-01-20 21:09:44.917604 mistletoe-1.0.1/mistletoe/contrib/
--rw-rw-rw-   0        0        0        0 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/contrib/__init__.py
--rw-rw-rw-   0        0        0      725 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/contrib/github_wiki.py
--rw-rw-rw-   0        0        0     8691 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/contrib/jira_renderer.py
--rw-rw-rw-   0        0        0      954 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/contrib/mathjax.py
--rw-rw-rw-   0        0        0     3560 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/contrib/md2jira.py
--rw-rw-rw-   0        0        0      724 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/contrib/pygments_renderer.py
--rw-rw-rw-   0        0        0     5310 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/contrib/scheme.py
--rw-rw-rw-   0        0        0     2307 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/contrib/toc_renderer.py
--rw-rw-rw-   0        0        0     8934 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/contrib/xwiki20_renderer.py
--rw-rw-rw-   0        0        0    17293 2023-01-14 20:16:14.000000 mistletoe-1.0.1/mistletoe/core_tokens.py
--rw-rw-rw-   0        0        0     8250 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/html_renderer.py
--rw-rw-rw-   0        0        0     6489 2023-01-10 08:01:32.000000 mistletoe-1.0.1/mistletoe/latex_renderer.py
--rw-rw-rw-   0        0        0      202 2020-06-28 12:58:34.000000 mistletoe-1.0.1/mistletoe/latex_token.py
--rw-rw-rw-   0        0        0     9557 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/span_token.py
--rw-rw-rw-   0        0        0     4042 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/span_tokenizer.py
--rw-rw-rw-   0        0        0     2273 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/token.py
--rw-rw-rw-   0        0        0     1344 2023-01-10 08:02:41.000000 mistletoe-1.0.1/mistletoe/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-20 21:09:44.902579 mistletoe-1.0.1/mistletoe.egg-info/
--rw-rw-rw-   0        0        0     1160 2023-01-20 21:09:44.000000 mistletoe-1.0.1/mistletoe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1133 2023-01-20 21:09:44.000000 mistletoe-1.0.1/mistletoe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-20 21:09:44.000000 mistletoe-1.0.1/mistletoe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-01-20 21:09:44.000000 mistletoe-1.0.1/mistletoe.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2020-06-28 13:15:10.000000 mistletoe-1.0.1/mistletoe.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-01-20 21:09:44.000000 mistletoe-1.0.1/mistletoe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-20 21:09:44.938606 mistletoe-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1455 2023-01-20 20:51:13.000000 mistletoe-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-20 21:09:44.935609 mistletoe-1.0.1/test/
--rw-rw-rw-   0        0        0     1993 2022-07-04 20:11:46.000000 mistletoe-1.0.1/test/test_ast_renderer.py
--rw-rw-rw-   0        0        0    23661 2023-01-10 08:02:41.000000 mistletoe-1.0.1/test/test_block_token.py
--rw-rw-rw-   0        0        0     5710 2022-07-04 20:11:46.000000 mistletoe-1.0.1/test/test_cli.py
--rw-rw-rw-   0        0        0     3273 2023-01-10 08:01:32.000000 mistletoe-1.0.1/test/test_core_tokens.py
--rw-rw-rw-   0        0        0     6143 2023-01-10 08:02:41.000000 mistletoe-1.0.1/test/test_html_renderer.py
--rw-rw-rw-   0        0        0     6270 2023-01-10 08:01:32.000000 mistletoe-1.0.1/test/test_latex_renderer.py
--rw-rw-rw-   0        0        0      544 2020-06-28 12:58:34.000000 mistletoe-1.0.1/test/test_latex_token.py
--rw-rw-rw-   0        0        0     5203 2023-01-10 08:02:41.000000 mistletoe-1.0.1/test/test_repr.py
--rw-rw-rw-   0        0        0     8100 2023-01-10 08:02:41.000000 mistletoe-1.0.1/test/test_span_token.py
--rw-rw-rw-   0        0        0     3983 2023-01-10 08:02:41.000000 mistletoe-1.0.1/test/test_traverse.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:49:44.931550 mistletoe-1.1.0/
+-rw-rw-rw-   0        0        0     1062 2020-06-28 12:58:34.000000 mistletoe-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0       16 2020-06-28 12:58:34.000000 mistletoe-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1160 2023-06-11 14:49:44.931550 mistletoe-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     9024 2023-06-11 10:43:44.000000 mistletoe-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-11 14:49:44.888889 mistletoe-1.1.0/mistletoe/
+-rw-rw-rw-   0        0        0      715 2023-06-11 14:47:01.000000 mistletoe-1.1.0/mistletoe/__init__.py
+-rw-rw-rw-   0        0        0      219 2020-06-28 12:58:34.000000 mistletoe-1.1.0/mistletoe/__main__.py
+-rw-rw-rw-   0        0        0     1437 2023-02-11 13:57:01.000000 mistletoe-1.1.0/mistletoe/ast_renderer.py
+-rw-rw-rw-   0        0        0     7577 2023-06-11 14:47:01.000000 mistletoe-1.1.0/mistletoe/base_renderer.py
+-rw-rw-rw-   0        0        0    37756 2023-06-11 10:43:44.000000 mistletoe-1.1.0/mistletoe/block_token.py
+-rw-rw-rw-   0        0        0     2531 2022-04-09 16:39:05.000000 mistletoe-1.1.0/mistletoe/block_tokenizer.py
+-rw-rw-rw-   0        0        0     2881 2022-07-04 20:11:46.000000 mistletoe-1.1.0/mistletoe/cli.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:49:44.909997 mistletoe-1.1.0/mistletoe/contrib/
+-rw-rw-rw-   0        0        0        0 2023-02-06 20:53:58.000000 mistletoe-1.1.0/mistletoe/contrib/__init__.py
+-rw-rw-rw-   0        0        0      898 2023-06-11 14:47:01.000000 mistletoe-1.1.0/mistletoe/contrib/github_wiki.py
+-rw-rw-rw-   0        0        0     8691 2023-04-02 07:04:55.000000 mistletoe-1.1.0/mistletoe/contrib/jira_renderer.py
+-rw-rw-rw-   0        0        0     1072 2023-06-11 14:47:01.000000 mistletoe-1.1.0/mistletoe/contrib/mathjax.py
+-rw-rw-rw-   0        0        0     3560 2023-02-06 20:53:58.000000 mistletoe-1.1.0/mistletoe/contrib/md2jira.py
+-rw-rw-rw-   0        0        0      712 2023-04-02 07:05:02.000000 mistletoe-1.1.0/mistletoe/contrib/pygments_renderer.py
+-rw-rw-rw-   0        0        0     5457 2023-02-11 07:15:35.000000 mistletoe-1.1.0/mistletoe/contrib/scheme.py
+-rw-rw-rw-   0        0        0     2486 2023-06-11 14:47:01.000000 mistletoe-1.1.0/mistletoe/contrib/toc_renderer.py
+-rw-rw-rw-   0        0        0     8934 2023-04-02 07:04:55.000000 mistletoe-1.1.0/mistletoe/contrib/xwiki20_renderer.py
+-rw-rw-rw-   0        0        0    17766 2023-06-11 10:43:44.000000 mistletoe-1.1.0/mistletoe/core_tokens.py
+-rw-rw-rw-   0        0        0     9359 2023-06-11 14:47:01.000000 mistletoe-1.1.0/mistletoe/html_renderer.py
+-rw-rw-rw-   0        0        0     6621 2023-06-11 14:47:01.000000 mistletoe-1.1.0/mistletoe/latex_renderer.py
+-rw-rw-rw-   0        0        0      202 2020-06-28 12:58:34.000000 mistletoe-1.1.0/mistletoe/latex_token.py
+-rw-rw-rw-   0        0        0    20015 2023-06-11 10:43:44.000000 mistletoe-1.1.0/mistletoe/markdown_renderer.py
+-rw-rw-rw-   0        0        0    10455 2023-06-11 10:43:44.000000 mistletoe-1.1.0/mistletoe/span_token.py
+-rw-rw-rw-   0        0        0     4042 2023-02-06 20:53:58.000000 mistletoe-1.1.0/mistletoe/span_tokenizer.py
+-rw-rw-rw-   0        0        0     2271 2023-02-11 13:57:01.000000 mistletoe-1.1.0/mistletoe/token.py
+-rw-rw-rw-   0        0        0     1344 2023-02-06 20:53:58.000000 mistletoe-1.1.0/mistletoe/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:49:44.899421 mistletoe-1.1.0/mistletoe.egg-info/
+-rw-rw-rw-   0        0        0     1160 2023-06-11 14:49:44.000000 mistletoe-1.1.0/mistletoe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1195 2023-06-11 14:49:44.000000 mistletoe-1.1.0/mistletoe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-11 14:49:44.000000 mistletoe-1.1.0/mistletoe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-11 14:49:44.000000 mistletoe-1.1.0/mistletoe.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2020-06-28 13:15:10.000000 mistletoe-1.1.0/mistletoe.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-06-11 14:49:44.000000 mistletoe-1.1.0/mistletoe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-11 14:49:44.931550 mistletoe-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1455 2023-02-11 07:15:35.000000 mistletoe-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-11 14:49:44.931550 mistletoe-1.1.0/test/
+-rw-rw-rw-   0        0        0     3865 2023-02-11 13:57:01.000000 mistletoe-1.1.0/test/test_ast_renderer.py
+-rw-rw-rw-   0        0        0    25865 2023-06-11 10:43:44.000000 mistletoe-1.1.0/test/test_block_token.py
+-rw-rw-rw-   0        0        0     5710 2022-07-04 20:11:46.000000 mistletoe-1.1.0/test/test_cli.py
+-rw-rw-rw-   0        0        0     3273 2023-02-10 20:23:49.000000 mistletoe-1.1.0/test/test_core_tokens.py
+-rw-rw-rw-   0        0        0     6734 2023-06-11 14:47:01.000000 mistletoe-1.1.0/test/test_html_renderer.py
+-rw-rw-rw-   0        0        0     6272 2023-02-11 07:15:35.000000 mistletoe-1.1.0/test/test_latex_renderer.py
+-rw-rw-rw-   0        0        0      544 2020-06-28 12:58:34.000000 mistletoe-1.1.0/test/test_latex_token.py
+-rw-rw-rw-   0        0        0    19632 2023-06-11 10:43:44.000000 mistletoe-1.1.0/test/test_markdown_renderer.py
+-rw-rw-rw-   0        0        0     5604 2023-06-11 10:43:44.000000 mistletoe-1.1.0/test/test_repr.py
+-rw-rw-rw-   0        0        0     8564 2023-06-11 10:43:44.000000 mistletoe-1.1.0/test/test_span_token.py
+-rw-rw-rw-   0        0        0     3983 2023-02-06 20:53:58.000000 mistletoe-1.1.0/test/test_traverse.py
```

### Comparing `mistletoe-1.0.1/LICENSE` & `mistletoe-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/PKG-INFO` & `mistletoe-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistletoe
-Version: 1.0.1
+Version: 1.1.0
 Summary: A fast, extensible Markdown parser in pure Python.
 Home-page: https://github.com/miyuchina/mistletoe
 Author: Mi Yu
 Author-email: hello@afteryu.me
 License: MIT
 Keywords: markdown lexer parser development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mistletoe-1.0.1/README.md` & `mistletoe-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <h1>mistletoe<img src='https://cdn.rawgit.com/miyuchina/mistletoe/master/resources/logo.svg' align='right' width='128' height='128'></h1>
 
-[![Build Status][build-badge]][travis]
+[![Build Status][build-badge]][github-actions]
 [![Coverage Status][cover-badge]][coveralls]
 [![PyPI][pypi-badge]][pypi]
 [![is wheel][wheel-badge]][pypi]
 
 mistletoe is a Markdown parser in pure Python,
 designed to be fast, spec-compliant and fully customizable.
 
@@ -42,14 +42,16 @@
 
 Renderers for the following "core" output formats exist within the mistletoe
 main package:
 
 * HTML
 * LaTeX
 * AST (Abstract Syntax Tree; handy for debugging the parsing process)
+* Markdown (Can be used to reflow the text, or make other types of automated
+  changes to Markdown documents)
 
 Renderers for the following output formats can be found
 in the [contrib][contrib] package:
 
 * HTML with MathJax (_mathjax.py_)
 * HTML with code highlighting (using Pygments) (_pygments\_renderer.py_)
 * HTML with TOC (for programmatical use) (_toc\_renderer.py_)
@@ -104,14 +106,25 @@
 import mistletoe
 from mistletoe.latex_renderer import LaTeXRenderer
 
 with open('foo.md', 'r') as fin:
     rendered = mistletoe.markdown(fin, LaTeXRenderer)
 ```
 
+To reflow the text in a Markdown document with a max line length of 20 characters:
+
+```python
+import mistletoe
+from mistletoe.markdown_renderer import MarkdownRenderer
+
+with open('dev-guide.md', 'r') as fin:
+    with MarkdownRenderer(max_line_length=20) as renderer:
+        print(renderer.render(mistletoe.Document(fin)))
+```
+
 Finally, here's how you would manually specify extra tokens via a renderer.
 In the following example, we use `HTMLRenderer` to render
 the AST. The renderer itself adds `HTMLBlock` and `HTMLSpan` tokens to the parsing
 process. The result should be equal to the output obtained from
 the first example above.
 
 ```python
@@ -224,19 +237,19 @@
 
 Copyright & License
 -------------------
 * mistletoe's logo uses artwork by [Freepik][icon], under
   [CC BY 3.0][cc-by].
 * mistletoe is released under [MIT][license].
 
-[build-badge]: https://img.shields.io/travis/miyuchina/mistletoe.svg?style=flat-square
+[build-badge]: https://img.shields.io/github/actions/workflow/status/miyuchina/mistletoe/python-package.yml?style=flat-square
 [cover-badge]: https://img.shields.io/coveralls/miyuchina/mistletoe.svg?style=flat-square
 [pypi-badge]: https://img.shields.io/pypi/v/mistletoe.svg?style=flat-square
 [wheel-badge]: https://img.shields.io/pypi/wheel/mistletoe.svg?style=flat-square
-[travis]: https://travis-ci.org/miyuchina/mistletoe
+[github-actions]: https://github.com/miyuchina/mistletoe/actions/workflows/python-package.yml
 [coveralls]: https://coveralls.io/github/miyuchina/mistletoe?branch=master
 [pypi]: https://pypi.python.org/pypi/mistletoe
 [mistune]: https://github.com/lepture/mistune
 [python-markdown]: https://github.com/waylan/Python-Markdown
 [python-markdown2]: https://github.com/trentm/python-markdown2
 [commonmark-py]: https://github.com/rtfd/CommonMark-py
 [performance]: performance.md
```

### Comparing `mistletoe-1.0.1/mistletoe/__init__.py` & `mistletoe-1.1.0/mistletoe/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Make mistletoe easier to import.
 """
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 __all__ = ['html_renderer', 'ast_renderer', 'block_token', 'block_tokenizer',
            'span_token', 'span_tokenizer']
 
 from mistletoe.block_token import Document
 from mistletoe.html_renderer import HTMLRenderer
 
 def markdown(iterable, renderer=HTMLRenderer):
```

### Comparing `mistletoe-1.0.1/mistletoe/ast_renderer.py` & `mistletoe-1.1.0/mistletoe/ast_renderer.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,13 +29,17 @@
     # Python 3.6 uses [ordered dicts] [1].
     # Put in 'type' entry first to make the final tree format somewhat
     # similar to [MDAST] [2].
     #
     #   [1]: https://docs.python.org/3/whatsnew/3.6.html
     #   [2]: https://github.com/syntax-tree/mdast
     node['type'] = token.__class__.__name__
-    node.update(token.__dict__)
-    if 'header' in node:
-        node['header'] = get_ast(node['header'])
-    if 'children' in node:
-        node['children'] = [get_ast(child) for child in node['children']]
+    for attrname in ['content', 'footnotes']:
+        if attrname in vars(token):
+            node[attrname] = getattr(token, attrname)
+    for attrname in token.repr_attributes:
+        node[attrname] = getattr(token, attrname)
+    if 'header' in vars(token):
+        node['header'] = get_ast(getattr(token, 'header'))
+    if 'children' in vars(token):
+        node['children'] = [get_ast(child) for child in token.children]
     return node
```

### Comparing `mistletoe-1.0.1/mistletoe/base_renderer.py` & `mistletoe-1.1.0/mistletoe/base_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     Attributes:
         render_map (dict): maps tokens to their corresponding render functions.
         _extras (list): a list of custom tokens to be added to the
                         parsing process.
     """
     _parse_name = re.compile(r"([A-Z][a-z]+|[A-Z]+(?![a-z]))")
 
-    def __init__(self, *extras):
+    def __init__(self, *extras, **kwargs):
         self.render_map = {
             'Strong':         self.render_strong,
             'Emphasis':       self.render_emphasis,
             'InlineCode':     self.render_inline_code,
             'RawText':        self.render_raw_text,
             'Strikethrough':  self.render_strikethrough,
             'Image':          self.render_image,
```

### Comparing `mistletoe-1.0.1/mistletoe/block_token.py` & `mistletoe-1.1.0/mistletoe/block_token.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,15 +124,19 @@
         return line_buffer
 
 
 class Document(BlockToken):
     """
     Document token.
     This is a container block token. Its children are block tokens - container or leaf ones.
+
+    Attributes:
+        footnotes (dictionary): link reference definitions.
     """
+
     def __init__(self, lines):
         if isinstance(lines, str):
             lines = lines.splitlines(keepends=True)
         lines = [line if line.endswith('\n') else '{}\n'.format(line) for line in lines]
         self.footnotes = {}
         token._root_node = self
         self.children = tokenize(lines)
@@ -142,54 +146,56 @@
 class Heading(BlockToken):
     """
     ATX heading token. (["### some heading ###\\n"])
     This is a leaf block token. Its children are inline (span) tokens.
 
     Attributes:
         level (int): heading level.
-        children (list): inner tokens.
     """
     repr_attributes = ("level",)
-    pattern = re.compile(r' {0,3}(#{1,6})(?:\n|\s+?(.*?)(?:\n|\s+?#+\s*?$))')
+    pattern = re.compile(r' {0,3}(#{1,6})(?:\n|\s+?(.*?)(\n|\s+?#+\s*?$))')
     level = 0
     content = ''
 
     def __init__(self, match):
-        self.level, content = match
+        self.level, content, self.closing_sequence = match
         super().__init__(content, span_token.tokenize_inner)
 
     @classmethod
     def start(cls, line):
         match_obj = cls.pattern.match(line)
         if match_obj is None:
             return False
         cls.level = len(match_obj.group(1))
         cls.content = (match_obj.group(2) or '').strip()
         if set(cls.content) == {'#'}:
             cls.content = ''
+        cls.closing_sequence = (match_obj.group(3) or '').strip()
         return True
 
     @classmethod
     def read(cls, lines):
         next(lines)
-        return cls.level, cls.content
+        return cls.level, cls.content, cls.closing_sequence
 
 class SetextHeading(BlockToken):
     """
     Setext heading token.
     This is a leaf block token. Its children are inline (span) tokens.
 
     Not included in the parsing process, but called by Paragraph.__new__.
 
     Attributes:
         level (int): heading level.
     """
     repr_attributes = ("level",)
+
     def __init__(self, lines):
-        self.level = 1 if lines.pop().lstrip().startswith('=') else 2
+        self.underline = lines.pop().rstrip()
+        self.level = 1 if self.underline.endswith('=') else 2
         content = '\n'.join([line.strip() for line in lines])
         super().__init__(content, span_token.tokenize_inner)
 
     @classmethod
     def start(cls, line):
         raise NotImplementedError()
 
@@ -347,37 +353,47 @@
 
 class BlockCode(BlockToken):
     """
     Indented code block token.
     This is a leaf block token with a single child of type span_token.RawText.
 
     Attributes:
-        children (list): contains a single span_token.RawText token.
         language (str): always the empty string.
     """
     repr_attributes = ("language",)
     def __init__(self, lines):
         self.language = ''
         self.children = (span_token.RawText(''.join(lines).strip('\n')+'\n'),)
 
+    @property
+    def content(self):
+        """Returns the code block content."""
+        return self.children[0].content
+
     @staticmethod
     def start(line):
         return line.replace('\t', '    ', 1).startswith('    ')
 
     @classmethod
     def read(cls, lines):
         line_buffer = []
+        trailing_blanks = 0
         for line in lines:
             if line.strip() == '':
                 line_buffer.append(line.lstrip(' ') if len(line) < 5 else line[4:])
+                trailing_blanks = trailing_blanks + 1 if line == '\n' else 0
                 continue
             if not line.replace('\t', '    ', 1).startswith('    '):
                 lines.backstep()
                 break
             line_buffer.append(cls.strip(line))
+            trailing_blanks = 0
+        for _ in range(trailing_blanks):
+            line_buffer.pop()
+            lines.backstep()
         return line_buffer
 
     @staticmethod
     def strip(string):
         count = 0
         for i, c in enumerate(string):
             if c == '\t':
@@ -393,36 +409,44 @@
 
 class CodeFence(BlockToken):
     """
     Fenced code block token. (["```sh\\n", "rm -rf /", ..., "```"])
     This is a leaf block token with a single child of type span_token.RawText.
 
     Attributes:
-        children (list): contains a single span_token.RawText token.
         language (str): language of code block (default to empty).
     """
     repr_attributes = ("language",)
-    pattern = re.compile(r'( {0,3})(`{3,}|~{3,}) *(\S*)')
+    pattern = re.compile(r'( {0,3})(`{3,}|~{3,})( *(\S*)[^\n]*)')
     _open_info = None
+
     def __init__(self, match):
         lines, open_info = match
-        self.language = span_token.EscapeSequence.strip(open_info[2])
+        self.indentation = open_info[0]
+        self.delimiter = open_info[1]
+        self.info_string = open_info[2]
+        self.language = span_token.EscapeSequence.strip(open_info[3])
         self.children = (span_token.RawText(''.join(lines)),)
 
+    @property
+    def content(self):
+        """Returns the code block content."""
+        return self.children[0].content
+
     @classmethod
     def start(cls, line):
         match_obj = cls.pattern.match(line)
         if not match_obj:
             return False
-        prepend, leader, lang = match_obj.groups()
+        prepend, leader, info_string, lang = match_obj.groups()
         # info strings for backtick code blocks may not contain backticks,
         # but info strings for tilde code blocks may contain both tildes and backticks.
-        if leader[0] == '`' and '`' in line[match_obj.end(2):]:
+        if leader[0] == '`' and '`' in info_string:
             return False
-        cls._open_info = len(prepend), leader, lang
+        cls._open_info = len(prepend), leader, info_string, lang
         return True
 
     @classmethod
     def read(cls, lines):
         next(lines)
         line_buffer = []
         for line in lines:
@@ -437,18 +461,17 @@
             line_buffer.append(stripped_line)
         return line_buffer, cls._open_info
 
 
 class List(BlockToken):
     """
     List token.
-    This is a container block token. Its children are list item tokens.
+    This is a container block token. Its children are ListItem tokens.
 
     Attributes:
-        children (list): a list of ListItem tokens.
         loose (bool): whether the list is loose.
         start (NoneType or int): None if unordered, starting number if ordered.
     """
     repr_attributes = ("loose", "start")
     pattern = re.compile(r' {0,3}(?:\d{0,9}[.)]|[+\-*])(?:[ \t]*$|[ \t]+)')
     def __init__(self, matches):
         self.children = [ListItem(*match) for match in matches]
@@ -495,14 +518,20 @@
 
 class ListItem(BlockToken):
     """
     List item token.
     This is a container block token. Its children are block tokens - container or leaf ones.
 
     Not included in the parsing process, but called by List.
+
+    Attributes:
+        leader (string): a bullet list marker or an ordered list marker.
+        prepend (int): the start position of the content, i.e., the indentation required
+                       for continuation lines.
+        loose (bool): whether the list is loose.
     """
     repr_attributes = ("leader", "prepend", "loose")
     pattern = re.compile(r' {0,3}(\d{0,9}[.)]|[+\-*])($|\s+)')
     continuation_pattern = re.compile(r'([ \t]*)(\S.*\n|\n)')
 
     def __init__(self, parse_buffer, prepend, leader):
         self.leader = leader
@@ -632,29 +661,29 @@
         parse_buffer = tokenizer.tokenize_block(line_buffer, _token_types)
         return (parse_buffer, prepend, leader), next_marker
 
 
 class Table(BlockToken):
     """
     Table token.
-    This is a container block token. Its children are table row tokens.
+    This is a container block token. Its children are TableRow tokens.
 
     Attributes:
-        has_header (bool): whether table has header row.
+        header: header row (TableRow).
         column_align (list): align options for each column (default to [None]).
-        children (list): inner tokens (TableRows).
     """
     repr_attributes = ("column_align",)
     def __init__(self, lines):
         if '---' in lines[1]:
             self.column_align = [self.parse_align(column)
                     for column in self.split_delimiter(lines[1])]
             self.header = TableRow(lines[0], self.column_align)
             self.children = [TableRow(line, self.column_align) for line in lines[2:]]
         else:
+            # note: not reachable, because read() guarantees the presence of three dashes
             self.column_align = [None]
             self.children = [TableRow(line) for line in lines]
 
     @staticmethod
     def split_delimiter(delimiter):
         """
         Helper function; returns a list of align options.
@@ -694,17 +723,20 @@
             return None
         return line_buffer
 
 
 class TableRow(BlockToken):
     """
     Table row token. Supports escaped pipes in table cells (for primary use within code spans).
-    This is a container block token. Its children are table cell tokens.
+    This is a container block token. Its children are TableCell tokens.
 
     Should only be called by Table.__init__().
+
+    Attributes:
+        row_align (list): align options for each column (default to [None]).
     """
     repr_attributes = ("row_align",)
     # Note: Python regex requires fixed-length look-behind,
     # so we cannot use a more precise alternative: r"(?<!\\(?:\\\\)*)(\|)"
     split_pattern = re.compile(r"(?<!\\)\|")
     escaped_pipe_pattern = re.compile(r"(?<!\\)(\\\\)*\\\|")
 
@@ -720,29 +752,29 @@
     Table cell token.
     This is a leaf block token. Its children are inline (span) tokens.
 
     Should only be called by TableRow.__init__().
 
     Attributes:
         align (bool): align option for current cell (default to None).
-        children (list): inner (span-)tokens.
     """
     repr_attributes = ("align",)
     def __init__(self, content, align=None):
         self.align = align
         super().__init__(content, span_token.tokenize_inner)
 
 
 class Footnote(BlockToken):
     """
-    Footnote token. A "link reference definition" according to the spec.
-    This is a leaf block token. Its children are inline (span) tokens.
+    Footnote token. One or more "link reference definitions" according to the CommonMark spec.
+    This is a leaf block token without children.
 
-    The constructor returns None, because the footnote information
-    is stored in Footnote.read.
+    The constructor returns None, because available footnote definitions are parsed
+    and stored into the root node within `Footnote.read()`. We don't put instances of
+    this class into the resulting AST.
     """
     def __new__(cls, _):
         return None
 
     @classmethod
     def start(cls, line):
         return line.lstrip().startswith('[')
@@ -786,14 +818,15 @@
             return None
 
         # link destination
         match_info = cls.match_link_dest(string, dest_start)
         if not match_info:
             return None
         _, dest_end, dest = match_info
+        dest_type = "angle_uri" if string[dest_start] == "<" else "uri"
 
         # either of:
         # 1) optional spaces or tabs and then a line break to finish the link reference definition.
         # 2) optional spaces or tabs (including up to one line ending) followed by a title.
         # in any case, if the destination is followed directly by non-whitespace, then it's not
         # a valid link reference definition.
         title_start = shift_whitespace(string, dest_end)
@@ -803,35 +836,36 @@
         # link title
         match_info = cls.match_link_title(string, title_start)
         if not match_info:
             # no valid title found. if there was a line break following the destination,
             # we still have a valid link reference definition. otherwise not.
             eol_pos = string[dest_end:title_start].find("\n")
             if eol_pos >= 0:
-                return dest_end + eol_pos + 1, (label, dest, "")
+                return dest_end + eol_pos + 1, (label, dest, "", dest_type, None)
             else:
                 return None
         _, title_end, title = match_info
 
         # optional spaces or tabs. final line ending.
         line_end = title_end
         while line_end < len(string):
             if string[line_end] == '\n':
-                return line_end + 1, (label, dest, title)
+                title_delimiter = string[title_start] if title_start < title_end else None
+                return line_end + 1, (label, dest, title, dest_type, title_delimiter)
             elif string[line_end] in whitespace:
                 line_end += 1
             else:
                 break
 
         # non-whitespace found on the same line as the title, making it invalid.
         # if there was a line break following the destination,
         # we still have a valid link reference definition. otherwise not.
         eol_pos = string[dest_end:title_start].find("\n")
         if eol_pos >= 0:
-            return dest_end + eol_pos + 1, (label, dest, "")
+            return dest_end + eol_pos + 1, (label, dest, "", dest_type, None)
         else:
             return None
 
     @classmethod
     def match_link_label(cls, string, offset):
         """
         Matches: up to three spaces, "[", label, "]".
@@ -913,56 +947,60 @@
                 return offset, i+1, string[offset+1:i]
             elif escaped:
                 escaped = False
         return None
 
     @staticmethod
     def append_footnotes(matches, root):
-        for key, dest, title in matches:
+        for key, dest, title, *_ in matches:
             key = normalize_label(key)
             dest = span_token.EscapeSequence.strip(dest.strip())
             title = span_token.EscapeSequence.strip(title)
             if key not in root.footnotes:
                 root.footnotes[key] = dest, title
 
 
 class ThematicBreak(BlockToken):
     """
     Thematic break token (a.k.a. horizontal rule.)
     This is a leaf block token without children.
     """
     pattern = re.compile(r' {0,3}(?:([-_*])\s*?)(?:\1\s*?){2,}$')
-    def __init__(self, _):
-        pass
+
+    def __init__(self, lines):
+        self.line = lines[0].strip('\n')
 
     @classmethod
     def start(cls, line):
         return cls.pattern.match(line)
 
     @staticmethod
     def read(lines):
         return [next(lines)]
 
 
 class HTMLBlock(BlockToken):
     """
     Block-level HTML token.
-    This is a leaf block token without children.
-
-    Attributes:
-        content (str): the raw HTML content.
+    This is a leaf block token with a single child of type span_token.RawText,
+    which holds the raw HTML content.
     """
     _end_cond = None
     multiblock = re.compile(r'<(pre|script|style|textarea)[ >\n]')
     predefined = re.compile(r'<\/?(.+?)(?:\/?>|[ \n])')
     custom_tag = re.compile(r'(?:' + '|'.join((span_token._open_tag,
                                 span_token._closing_tag)) + r')\s*$')
 
     def __init__(self, lines):
-        self.content = ''.join(lines).rstrip('\n')
+        self.children = (span_token.RawText(''.join(lines).rstrip('\n')),)
+
+    @property
+    def content(self):
+        """Returns the raw HTML content."""
+        return self.children[0].content
 
     @classmethod
     def start(cls, line):
         stripped = line.lstrip()
         if len(line) - len(stripped) >= 4:
             return False
         # rule 1: HTML tags designed to contain literal content, allow newlines in block
@@ -1005,14 +1043,15 @@
         for line in lines:
             line_buffer.append(line)
             if cls._end_cond is not None:
                 if cls._end_cond in line.casefold():
                     break
             elif line.strip() == '':
                 line_buffer.pop()
+                lines.backstep()
                 break
         return line_buffer
 
 
 _token_types = []
 reset_tokens()
```

### Comparing `mistletoe-1.0.1/mistletoe/block_tokenizer.py` & `mistletoe-1.1.0/mistletoe/block_tokenizer.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/mistletoe/cli.py` & `mistletoe-1.1.0/mistletoe/cli.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/mistletoe/contrib/jira_renderer.py` & `mistletoe-1.1.0/mistletoe/contrib/jira_renderer.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/mistletoe/contrib/md2jira.py` & `mistletoe-1.1.0/mistletoe/contrib/md2jira.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/mistletoe/contrib/pygments_renderer.py` & `mistletoe-1.1.0/mistletoe/contrib/pygments_renderer.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 
     def __init__(self, *extras, style='default'):
         super().__init__(*extras)
         self.formatter.style = get_style(style)
 
 
     def render_block_code(self, token):
-        code = token.children[0].content
+        code = token.content
         lexer = get_lexer(token.language) if token.language else guess_lexer(code)
         return highlight(code, lexer, self.formatter)
```

### Comparing `mistletoe-1.0.1/mistletoe/contrib/scheme.py` & `mistletoe-1.1.0/mistletoe/contrib/scheme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import re
 from collections import ChainMap
-from mistletoe import BaseRenderer, span_token, block_token
+from functools import reduce
+from mistletoe.base_renderer import BaseRenderer
+from mistletoe import span_token, block_token
 from mistletoe.core_tokens import MatchObj
 
 
 class Program(block_token.BlockToken):
     def __init__(self, lines):
         self.children = span_token.tokenize_inner(''.join([line.strip() for line in lines]))
 
@@ -99,14 +101,17 @@
             "cond": self.cond,
             "null": None,
             "null?": lambda x: self.render(x) is None,
             "list": lambda *args: reduce(lambda x, y: (y, x), map(self.render, reversed(args)), None),
             "display": lambda *args: print(*map(self.render, args)),
         })
 
+    def render_program(self, token):
+        return self.render_inner(token)
+
     def render_inner(self, token):
         result = None
         for child in token.children:
             result = self.render(child)
         return result
 
     def render_expr(self, token):
```

### Comparing `mistletoe-1.0.1/mistletoe/contrib/toc_renderer.py` & `mistletoe-1.1.0/mistletoe/contrib/toc_renderer.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 import re
 from mistletoe.html_renderer import HTMLRenderer
 from mistletoe import block_token
 
 class TOCRenderer(HTMLRenderer):
     """
     Extends HTMLRenderer class for table of contents support.
-
-    Args:
-        depth (int): the maximum level of heading to be included in TOC;
-        omit_title (bool): whether to ignore tokens where token.level == 1;
-        filter_conds (list): when any of these functions evaluate to true,
-                             current heading will not be included;
-        extras (list): allows subclasses to add even more custom tokens.
     """
-    def __init__(self, depth=5, omit_title=True, filter_conds=[], *extras):
-        super().__init__(*extras)
+    def __init__(self, *extras, depth=5, omit_title=True, filter_conds=[], **kwargs):
+        """
+        Args:
+            extras (list): allows subclasses to add even more custom tokens.
+            depth (int): the maximum level of heading to be included in TOC.
+            omit_title (bool): whether to ignore tokens where token.level == 1.
+            filter_conds (list): when any of these functions evaluate to true,
+                                current heading will not be included.
+            **kwargs: additional parameters to be passed to the ancestor's
+                      constructor.
+        """
+        super().__init__(*extras, **kwargs)
         self._headings = []
         self.depth = depth
         self.omit_title = omit_title
         self.filter_conds = filter_conds
 
     @property
     def toc(self):
```

### Comparing `mistletoe-1.0.1/mistletoe/contrib/xwiki20_renderer.py` & `mistletoe-1.1.0/mistletoe/contrib/xwiki20_renderer.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/mistletoe/core_tokens.py` & `mistletoe-1.1.0/mistletoe/core_tokens.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         if open_pos is not None:
             opener = delimiters[open_pos]
             n = 2 if closer.number >= 2 and opener.number >= 2 else 1
             start = opener.end - n
             end = closer.start + n
             match = MatchObj(start, end, (start+n, end-n, string[start+n:end-n]))
             match.type = 'Strong' if n == 2 else 'Emphasis'
+            match.delimiter = string[start]
             matches.append(match)
             # remove all delimiters in between
             del delimiters[open_pos+1:curr_pos]
             curr_pos -= curr_pos - open_pos - 1
             # remove appropriate number of chars from delimiters
             if not opener.remove(n, left=False):
                 delimiters.remove(opener)
@@ -171,51 +172,57 @@
                 if paren_index < len(string) and string[paren_index] == ')':
                     end = paren_index + 1
                     match = MatchObj(start, end,
                                       (text_start, text_end, text),
                                       (dest_start, dest_end, dest),
                                       (title_start, title_end, title))
                     match.type = 'Link' if not image else 'Image'
+                    match.dest_type = "angle_uri" if dest_start < dest_end and string[dest_start] == "<" else "uri"
+                    match.title_delimiter = string[title_start] if title_start < title_end else None
                     return match
     # footnote link
     if follows(string, offset, '['):
-        # full footnote link
+        # full footnote link: [label][dest]
         result = match_link_label(string, offset+1, root)
         if result:
             match_info, (dest, title) = result
             end = match_info[1]
             match = MatchObj(start, end,
                               (text_start, text_end, text),
                               (-1, -1, dest),
                               (-1, -1, title))
             match.type = 'Link' if not image else 'Image'
+            match.label = match_info[2]
+            match.dest_type = "full"
             return match
         ref = get_link_label(text, root)
         if ref:
-            # compact footnote link
+            # compact (collapsed) footnote link: [dest][]
             if follows(string, offset+1, ']'):
                 dest, title = ref
                 end = offset + 3
                 match = MatchObj(start, end,
                                   (text_start, text_end, text),
                                   (-1, -1, dest),
                                   (-1, -1, title))
                 match.type = 'Link' if not image else 'Image'
+                match.dest_type = "collapsed"
                 return match
         return None
-    # shortcut footnote link
+    # shortcut footnote link: [dest]
     ref = get_link_label(text, root)
     if ref:
         dest, title = ref
         end = offset + 1
         match = MatchObj(start, end,
                           (text_start, text_end, text),
                           (-1, -1, dest),
                           (-1, -1, title))
         match.type = 'Link' if not image else 'Image'
+        match.dest_type = "shortcut"
         return match
     return None
 
 
 def match_link_dest(string, offset):
     offset = shift_whitespace(string, offset+1)
     if offset == len(string):
```

### Comparing `mistletoe-1.0.1/mistletoe/html_renderer.py` & `mistletoe-1.1.0/mistletoe/html_renderer.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,21 +14,29 @@
 
 class HTMLRenderer(BaseRenderer):
     """
     HTML renderer class.
 
     See mistletoe.base_renderer module for more info.
     """
-    def __init__(self, *extras):
+    def __init__(self, *extras, html_escape_double_quotes=True, html_escape_single_quotes=False, **kwargs):
         """
         Args:
             extras (list): allows subclasses to add even more custom tokens.
+            html_escape_double_quotes (bool): whether to also escape double
+                quotes when HTML-escaping rendered text.
+            html_escape_single_quotes (bool): whether to also escape single
+                quotes when HTML-escaping rendered text.
+            **kwargs: additional parameters to be passed to the ancestor's
+                constructor.
         """
         self._suppress_ptag_stack = [False]
-        super().__init__(*chain((HTMLBlock, HTMLSpan), extras))
+        super().__init__(*chain((HTMLBlock, HTMLSpan), extras), **kwargs)
+        self.html_escape_double_quotes = html_escape_double_quotes
+        self.html_escape_single_quotes = html_escape_single_quotes
 
     def __exit__(self, *args):
         super().__exit__(*args)
 
     def render_to_plain(self, token) -> str:
         if hasattr(token, 'children'):
             inner = [self.render_to_plain(child) for child in token.children]
@@ -41,15 +49,15 @@
 
     def render_emphasis(self, token: span_token.Emphasis) -> str:
         template = '<em>{}</em>'
         return template.format(self.render_inner(token))
 
     def render_inline_code(self, token: span_token.InlineCode) -> str:
         template = '<code>{}</code>'
-        inner = html.escape(token.children[0].content)
+        inner = self.escape_html_text(token.children[0].content)
         return template.format(inner)
 
     def render_strikethrough(self, token: span_token.Strikethrough) -> str:
         template = '<del>{}</del>'
         return template.format(self.render_inner(token))
 
     def render_image(self, token: span_token.Image) -> str:
@@ -79,15 +87,15 @@
         inner = self.render_inner(token)
         return template.format(target=target, inner=inner)
 
     def render_escape_sequence(self, token: span_token.EscapeSequence) -> str:
         return self.render_inner(token)
 
     def render_raw_text(self, token: span_token.RawText) -> str:
-        return html.escape(token.content)
+        return self.escape_html_text(token.content)
 
     @staticmethod
     def render_html_span(token: span_token.HTMLSpan) -> str:
         return token.content
 
     def render_heading(self, token: block_token.Heading) -> str:
         template = '<h{level}>{inner}</h{level}>'
@@ -109,15 +117,15 @@
 
     def render_block_code(self, token: block_token.BlockCode) -> str:
         template = '<pre><code{attr}>{inner}</code></pre>'
         if token.language:
             attr = ' class="{}"'.format('language-{}'.format(html.escape(token.language)))
         else:
             attr = ''
-        inner = html.escape(token.children[0].content)
+        inner = self.escape_html_text(token.content)
         return template.format(attr=attr, inner=inner)
 
     def render_list(self, token: block_token.List) -> str:
         template = '<{tag}{attr}>\n{inner}\n</{tag}>'
         if token.start is not None:
             tag = 'ol'
             attr = ' start="{}"'.format(token.start) if token.start != 1 else ''
@@ -189,20 +197,30 @@
         return token.content
 
     def render_document(self, token: block_token.Document) -> str:
         self.footnotes.update(token.footnotes)
         inner = '\n'.join([self.render(child) for child in token.children])
         return '{}\n'.format(inner) if inner else ''
 
-    @staticmethod
-    def escape_html(raw: str) -> str:
+    def escape_html_text(self, s: str) -> str:
         """
-        This method is deprecated. Use `html.escape` instead.
+        Like `html.escape()`, but this  looks into the current rendering options
+        to decide which of the quotes (double, single, or both) to escape.
+
+        Intended for escaping text content. To escape content of an attribute,
+        simply call `html.escape()`.
         """
-        return html.escape(raw)
+        s = s.replace("&", "&amp;") # Must be done first!
+        s = s.replace("<", "&lt;")
+        s = s.replace(">", "&gt;")
+        if self.html_escape_double_quotes:
+            s = s.replace('"', "&quot;")
+        if self.html_escape_single_quotes:
+            s = s.replace('\'', "&#x27;")
+        return s
 
     @staticmethod
     def escape_url(raw: str) -> str:
         """
         Escape urls to prevent code injection craziness. (Hopefully.)
         """
         return html.escape(quote(raw, safe='/#:()*?=%@+,&;'))
```

### Comparing `mistletoe-1.0.1/mistletoe/latex_renderer.py` & `mistletoe-1.1.0/mistletoe/latex_renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 for delimiter in '*':  # remove invalid delimiters
     verb_delimiters.replace(delimiter, '')
 for delimiter in reversed('|!"\'=+'):  # start with most common delimiters
     verb_delimiters = delimiter + verb_delimiters.replace(delimiter, '')
 
 
 class LaTeXRenderer(BaseRenderer):
-    def __init__(self, *extras):
+    def __init__(self, *extras, **kwargs):
         """
         Args:
             extras (list): allows subclasses to add even more custom tokens.
+            **kwargs: additional parameters to be passed to the ancestor's
+                      constructor.
         """
         tokens = self._tokens_from_module(latex_token)
         self.packages = {}
         self.verb_delimiters = verb_delimiters
-        super().__init__(*chain(tokens, extras))
+        super().__init__(*chain(tokens, extras), **kwargs)
 
     def render_strong(self, token):
         return '\\textbf{{{}}}'.format(self.render_inner(token))
 
     def render_emphasis(self, token):
         return '\\textit{{{}}}'.format(self.render_inner(token))
```

### Comparing `mistletoe-1.0.1/mistletoe/span_token.py` & `mistletoe-1.1.0/mistletoe/span_token.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,37 +96,43 @@
 
 class Strong(SpanToken):
     """
     Strong token. ("**some text**")
     This is an inline token. Its children are inline (span) tokens.
     One of the core tokens.
     """
+    def __init__(self, match):
+        self.delimiter = match.delimiter
 
 
 class Emphasis(SpanToken):
     """
     Emphasis token. ("*some text*")
     This is an inline token. Its children are inline (span) tokens.
     One of the core tokens.
     """
+    def __init__(self, match):
+        self.delimiter = match.delimiter
 
 
 class InlineCode(SpanToken):
     """
     Inline code token. ("`some code`")
     This is an inline token with a single child of type RawText.
     """
     pattern = re.compile(r"(?<!\\|`)(?:\\\\)*(`+)(?!`)(.+?)(?<!`)\1(?!`)", re.DOTALL)
     parse_inner = False
     parse_group = 2
 
     def __init__(self, match):
         content = match.group(self.parse_group)
+        self.delimiter = match.group(1)
         content = content.replace('\n', ' ')
-        if not content.isspace() and content.startswith(" ") and content.endswith(" "):
+        self.padding = " " if not content.isspace() and content.startswith(" ") and content.endswith(" ") else ""
+        if self.padding:
             content = content[1:-1]
         self.children = (RawText(content),)
 
     @classmethod
     def find(cls, string):
         matches = core_tokens._code_matches
         core_tokens._code_matches = []
@@ -146,60 +152,69 @@
     Image token. ("![alt](src "title")")
     This is an inline token. Its children are inline (span) tokens holding the image description.
     One of the core tokens.
 
     Attributes:
         src (str): image source.
         title (str): image title (default to empty).
+        label (str): link label, for reference links.
     """
     repr_attributes = ("src", "title")
     def __init__(self, match):
         self.src = EscapeSequence.strip(match.group(2).strip())
         self.title = EscapeSequence.strip(match.group(3))
+        self.dest_type = getattr(match, "dest_type", None)
+        self.label = getattr(match, "label", None)
+        self.title_delimiter = getattr(match, "title_delimiter", None)
 
 
 class Link(SpanToken):
     """
-    Link token. ("[name](target)")
+    Link token. ("[name](target "title")")
     This is an inline token. Its children are inline (span) tokens holding the link text.
     One of the core tokens.
 
     Attributes:
         target (str): link target.
         title (str): link title (default to empty).
+        label (str): link label, for reference links.
     """
     repr_attributes = ("target", "title")
     def __init__(self, match):
         self.target = EscapeSequence.strip(match.group(2).strip())
         self.title = EscapeSequence.strip(match.group(3))
+        self.dest_type = getattr(match, "dest_type", None)
+        self.label = getattr(match, "label", None)
+        self.title_delimiter = getattr(match, "title_delimiter", None)
 
 
 class AutoLink(SpanToken):
     """
     Autolink token. ("<http://www.google.com>")
     This is an inline token with a single child of type RawText.
 
     Attributes:
-        children (iterator): a single RawText node for the link target.
+        children (list): a single RawText node for the link target.
         target (str): link target.
+        mailto (bool): true iff the target looks like an email address, but does not have the "mailto:" prefix.
     """
     repr_attributes = ("target", "mailto")
     pattern = re.compile(r"(?<!\\)(?:\\\\)*<([A-Za-z][A-Za-z0-9+.-]{1,31}:[^ <>]*?|[A-Za-z0-9.!#$%&'*+/=?^_`{|}~-]+@[A-Za-z0-9](?:[A-Za-z0-9-]{0,61}[A-Za-z0-9])?(?:\.[A-Za-z0-9](?:[A-Za-z0-9-]{0,61}[A-Za-z0-9])?)*)>")
     parse_inner = False
 
     def __init__(self, match):
         content = match.group(self.parse_group)
         self.children = (RawText(content),)
         self.target = content
         self.mailto = '@' in self.target and 'mailto' not in self.target.casefold()
 
 
 class EscapeSequence(SpanToken):
     """
-    Escape sequence token. ("\*")
+    Escape sequence token. ("\\\\*")
     This is an inline token with a single child of type RawText.
 
     Attributes:
         children (iterator): a single RawText node containing the escaped character.
     """
     pattern = re.compile(r"\\([!\"#$%&'()*+,-./:;<=>?@\[\\\]^_`{|}~])")
     parse_inner = False
@@ -211,26 +226,28 @@
     @classmethod
     def strip(cls, string):
         return html.unescape(cls.pattern.sub(r'\1', string))
 
 
 class LineBreak(SpanToken):
     """
-    Line break token. Hard or soft.
+    Line break token: hard or soft.
     This is an inline token without children.
+
+    Attributes:
+        soft (bool): true if this is a soft line break.
     """
     repr_attributes = ("soft",)
     pattern = re.compile(r'( *|\\)\n')
     parse_inner = False
     parse_group = 0
 
     def __init__(self, match):
-        content = match.group(1)
-        self.soft = not content.startswith(('  ', '\\'))
-        self.content = ''
+        self.content = match.group(1)
+        self.soft = not self.content.startswith(('  ', '\\'))
 
 
 class RawText(SpanToken):
     """
     Raw text token.
     This is an inline token without children.
```

### Comparing `mistletoe-1.0.1/mistletoe/span_tokenizer.py` & `mistletoe-1.1.0/mistletoe/span_tokenizer.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/mistletoe/token.py` & `mistletoe-1.1.0/mistletoe/token.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,22 +50,22 @@
 
     def __repr__(self):
         output = "<{}.{}".format(
             self.__class__.__module__,
             self.__class__.__name__
         )
 
-        if hasattr(self, "children"):
+        if "children" in vars(self):
             count = len(self.children)
             if count == 1:
                 output += " with 1 child"
             else:
                 output += " with {} children".format(count)
 
-        if hasattr(self, "content"):
+        if "content" in vars(self):
            output += " content=" + _short_repr(self.content)
 
         for attrname in self.repr_attributes:
             attrvalue = getattr(self, attrname)
             output += " {}={}".format(attrname, _short_repr(attrvalue))
         output += " at {:#x}>".format(id(self))
         return output
```

### Comparing `mistletoe-1.0.1/mistletoe/utils.py` & `mistletoe-1.1.0/mistletoe/utils.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/mistletoe.egg-info/PKG-INFO` & `mistletoe-1.1.0/mistletoe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistletoe
-Version: 1.0.1
+Version: 1.1.0
 Summary: A fast, extensible Markdown parser in pure Python.
 Home-page: https://github.com/miyuchina/mistletoe
 Author: Mi Yu
 Author-email: hello@afteryu.me
 License: MIT
 Keywords: markdown lexer parser development
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mistletoe-1.0.1/mistletoe.egg-info/SOURCES.txt` & `mistletoe-1.1.0/mistletoe.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 mistletoe/block_token.py
 mistletoe/block_tokenizer.py
 mistletoe/cli.py
 mistletoe/core_tokens.py
 mistletoe/html_renderer.py
 mistletoe/latex_renderer.py
 mistletoe/latex_token.py
+mistletoe/markdown_renderer.py
 mistletoe/span_token.py
 mistletoe/span_tokenizer.py
 mistletoe/token.py
 mistletoe/utils.py
 mistletoe.egg-info/PKG-INFO
 mistletoe.egg-info/SOURCES.txt
 mistletoe.egg-info/dependency_links.txt
@@ -35,10 +36,11 @@
 test/test_ast_renderer.py
 test/test_block_token.py
 test/test_cli.py
 test/test_core_tokens.py
 test/test_html_renderer.py
 test/test_latex_renderer.py
 test/test_latex_token.py
+test/test_markdown_renderer.py
 test/test_repr.py
 test/test_span_token.py
 test/test_traverse.py
```

### Comparing `mistletoe-1.0.1/setup.py` & `mistletoe-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/test/test_block_token.py` & `mistletoe-1.1.0/test/test_block_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,14 +121,19 @@
 
 class TestBlockCode(TestToken):
     def test_parse_indented_code(self):
         lines = ['    rm dir\n', '    mkdir test\n']
         arg = 'rm dir\nmkdir test\n'
         self._test_match(block_token.BlockCode, lines, arg, language='')
 
+    def test_parse_indented_code_with_blank_lines(self):
+        lines = ['    chunk1\n', '\n', '    chunk2\n', '  \n', ' \n', ' \n', '    chunk3\n']
+        arg = 'chunk1\n\nchunk2\n\n\n\nchunk3\n'
+        self._test_match(block_token.BlockCode, lines, arg, language='')
+
 
 class TestParagraph(TestToken):
     def test_parse(self):
         lines = ['some\n', 'continuous\n', 'lines\n']
         arg = 'some'
         self._test_match(block_token.Paragraph, lines, arg)
 
@@ -544,7 +549,58 @@
                  '_bar_\n',
                  '\n',
                  '</textarea>\n']
         document = block_token.Document(lines)
         tokens = document.children
         self.assertEqual(1, len(tokens))
         self.assertIsInstance(tokens[0], block_token.HTMLBlock)
+
+
+class TestLeafBlockTokenContentProperty(unittest.TestCase):
+    def setUp(self):
+        block_token.add_token(block_token.HTMLBlock)
+        self.addCleanup(block_token.reset_tokens)
+
+    def test_code_fence(self):
+        lines = ['```\n',
+                 'line 1\n',
+                 'line 2\n',
+                 '```\n']
+        document = block_token.Document(lines)
+        tokens = document.children
+        self.assertEqual(1, len(tokens))
+        self.assertIsInstance(tokens[0], block_token.CodeFence)
+
+        # option 1: direct access to the content
+        self.assertEqual('line 1\nline 2\n', tokens[0].children[0].content)
+
+        # option 2: using property getter to access the content
+        self.assertEqual('line 1\nline 2\n', tokens[0].content)
+
+    def test_block_code(self):
+        lines = ['    line 1\n',
+                 '    line 2\n']
+        document = block_token.Document(lines)
+        tokens = document.children
+        self.assertEqual(1, len(tokens))
+        self.assertIsInstance(tokens[0], block_token.BlockCode)
+
+        # option 1: direct access to the content
+        self.assertEqual('line 1\nline 2\n', tokens[0].children[0].content)
+
+        # option 2: using property getter to access the content
+        self.assertEqual('line 1\nline 2\n', tokens[0].content)
+
+    def test_html_block(self):
+        lines = ['<div>\n',
+                 'text\n'
+                 '</div>\n']
+        document = block_token.Document(lines)
+        tokens = document.children
+        self.assertEqual(1, len(tokens))
+        self.assertIsInstance(tokens[0], block_token.HTMLBlock)
+
+        # option 1: direct access to the content
+        self.assertEqual(''.join(lines).strip(), tokens[0].children[0].content)
+
+        # option 2: using property getter to access the content
+        self.assertEqual(''.join(lines).strip(), tokens[0].content)
```

### Comparing `mistletoe-1.0.1/test/test_cli.py` & `mistletoe-1.1.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/test/test_core_tokens.py` & `mistletoe-1.1.0/test/test_core_tokens.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/test/test_html_renderer.py` & `mistletoe-1.1.0/test/test_html_renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase, mock
 from mistletoe.html_renderer import HTMLRenderer
-
+from parameterized import parameterized
 
 class TestRenderer(TestCase):
     def setUp(self):
         self.renderer = HTMLRenderer()
         self.renderer.render_inner = mock.Mock(return_value='inner')
         self.renderer.__enter__()
         self.addCleanup(self.renderer.__exit__, None, None, None)
@@ -134,14 +134,27 @@
     def test_line_break(self):
         self._test_token('LineBreak', '<br />\n', children=False, soft=False)
 
     def test_document(self):
         self._test_token('Document', '', footnotes={})
 
 
+class TestHTMLRendererEscaping(TestCase):
+    @parameterized.expand([
+        (False, False, '" and \''),
+        (False, True, '" and &#x27;'),
+        (True, False, '&quot; and \''),
+        (True, True, '&quot; and &#x27;'),
+    ])
+    def test_escape_html_text(self, escape_double, escape_single, expected):
+        with HTMLRenderer(html_escape_double_quotes=escape_double,
+                          html_escape_single_quotes=escape_single) as renderer:
+            self.assertEqual(renderer.escape_html_text('" and \''), expected)
+
+
 class TestHTMLRendererFootnotes(TestCase):
     def setUp(self):
         self.renderer = HTMLRenderer()
         self.renderer.__enter__()
         self.addCleanup(self.renderer.__exit__, None, None, None)
 
     def test_footnote_image(self):
```

#### html2text {}

```diff
@@ -1,10 +1,11 @@
 from unittest import TestCase, mock from mistletoe.html_renderer import
-HTMLRenderer class TestRenderer(TestCase): def setUp(self): self.renderer =
-HTMLRenderer() self.renderer.render_inner = mock.Mock(return_value='inner')
+HTMLRenderer from parameterized import parameterized class TestRenderer
+(TestCase): def setUp(self): self.renderer = HTMLRenderer()
+self.renderer.render_inner = mock.Mock(return_value='inner')
 self.renderer.__enter__() self.addCleanup(self.renderer.__exit__, None, None,
 None) def _test_token(self, token_name, output, children=True,
 without_attrs=None, **kwargs): render_func = self.renderer.render_map
 [token_name] children = mock.MagicMock(spec=list) if children else None
 mock_token = mock.Mock(children=children, **kwargs) without_attrs =
 without_attrs or [] for attr in without_attrs: delattr(mock_token, attr)
 self.assertEqual(render_func(mock_token), output) class TestHTMLRenderer
@@ -66,18 +67,25 @@
 ', children=False) def test_html_block(self): content = output = '
 ****** hello ******
 \n
 this is\na paragraph
 \n' self._test_token('HTMLBlock', output, children=False, content=content) def
 test_line_break(self): self._test_token('LineBreak', '
 \n', children=False, soft=False) def test_document(self): self._test_token
-('Document', '', footnotes={}) class TestHTMLRendererFootnotes(TestCase): def
-setUp(self): self.renderer = HTMLRenderer() self.renderer.__enter__()
-self.addCleanup(self.renderer.__exit__, None, None, None) def
-test_footnote_image(self): from mistletoe import Document token = Document(['!
-[alt][foo]\n', '\n', '[foo]: bar "title"\n']) output = '
+('Document', '', footnotes={}) class TestHTMLRendererEscaping(TestCase):
+@parameterized.expand([ (False, False, '" and \''), (False, True, '" and
+&#x27;'), (True, False, '" and \''), (True, True, '" and &#x27;'), ]) def
+test_escape_html_text(self, escape_double, escape_single, expected): with
+HTMLRenderer(html_escape_double_quotes=escape_double,
+html_escape_single_quotes=escape_single) as renderer: self.assertEqual
+(renderer.escape_html_text('" and \''), expected) class
+TestHTMLRendererFootnotes(TestCase): def setUp(self): self.renderer =
+HTMLRenderer() self.renderer.__enter__() self.addCleanup
+(self.renderer.__exit__, None, None, None) def test_footnote_image(self): from
+mistletoe import Document token = Document(['![alt][foo]\n', '\n', '[foo]: bar
+"title"\n']) output = '
 [alt]
 \n' self.assertEqual(self.renderer.render(token), output) def
 test_footnote_link(self): from mistletoe import Document token = Document(['
 [name][foo]\n', '\n', '[foo]: target\n']) output = '
 name
 \n' self.assertEqual(self.renderer.render(token), output)
```

### Comparing `mistletoe-1.0.1/test/test_latex_renderer.py` & `mistletoe-1.1.0/test/test_latex_renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,18 +122,18 @@
                   'inner'
                   '\\end{document}\n')
         self._test_token('Document', output, footnotes={})
 
 
 class TestHtmlEntity(TestCase):
     def test_html_entity(self):
-        self.assertIn('hello \& goodbye', markdown('hello &amp; goodbye', LaTeXRenderer))
+        self.assertIn('hello \\& goodbye', markdown('hello &amp; goodbye', LaTeXRenderer))
 
     def test_html_entity_in_link_target(self):
-        self.assertIn('\href{foo}{hello}', markdown('[hello](f&#111;&#111;)', LaTeXRenderer))
+        self.assertIn('\\href{foo}{hello}', markdown('[hello](f&#111;&#111;)', LaTeXRenderer))
 
 
 class TestLaTeXFootnotes(TestCase):
     def setUp(self):
         self.renderer = LaTeXRenderer()
         self.renderer.__enter__()
         self.addCleanup(self.renderer.__exit__, None, None, None)
```

### Comparing `mistletoe-1.0.1/test/test_latex_token.py` & `mistletoe-1.1.0/test/test_latex_token.py`

 * *Files identical despite different names*

### Comparing `mistletoe-1.0.1/test/test_repr.py` & `mistletoe-1.1.0/test/test_repr.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,19 +14,21 @@
 
     def test_document(self):
         doc = Document("# Foo")
         self._check_repr_matches(doc, "block_token.Document with 1 child")
 
     def test_heading(self):
         doc = Document("# Foo")
-        self._check_repr_matches(doc.children[0], "block_token.Heading with 1 child content='Foo' level=1")
+        self._check_repr_matches(doc.children[0], "block_token.Heading with 1 child level=1")
+        self._check_repr_matches(doc.children[0].children[0], "span_token.RawText content='Foo'")
 
     def test_subheading(self):
         doc = Document("# Foo\n## Bar")
-        self._check_repr_matches(doc.children[1], "block_token.Heading with 1 child content='Bar' level=2")
+        self._check_repr_matches(doc.children[1], "block_token.Heading with 1 child level=2")
+        self._check_repr_matches(doc.children[1].children[0], "span_token.RawText content='Bar'")
 
     def test_quote(self):
         doc = Document("> Foo")
         self._check_repr_matches(doc.children[0], "block_token.Quote with 1 child")
 
     def test_paragraph(self):
         doc = Document("Foo")
@@ -59,16 +61,21 @@
     def test_thematicbreak(self):
         doc = Document("Foo\n\n---\n\nBar\n")
         self._check_repr_matches(doc.children[1], "block_token.ThematicBreak")
 
     # No test for ``Footnote``
 
     def test_htmlblock(self):
-        token = block_token.HTMLBlock("<pre>\nFoo\n</pre>\n")
-        self._check_repr_matches(token, "block_token.HTMLBlock content='<pre>\\nFoo\\n</pre>'")
+        try:
+            block_token.add_token(block_token.HTMLBlock)
+            doc = Document("<pre>\nFoo\n</pre>\n")
+        finally:
+            block_token.reset_tokens()
+        self._check_repr_matches(doc.children[0], "block_token.HTMLBlock with 1 child")
+        self._check_repr_matches(doc.children[0].children[0], "span_token.RawText content='<pre>\\nFoo\\n</pre>'")
 
     # Span tokens
 
     def test_strong(self):
         doc = Document("**foo**\n")
         self._check_repr_matches(doc.children[0].children[0], "span_token.Strong with 1 child")
 
@@ -102,12 +109,12 @@
 
     def test_soft_linebreak(self):
         doc = Document("Foo\nBar\n")
         self._check_repr_matches(doc.children[0].children[1], "span_token.LineBreak content='' soft=True")
 
     def test_hard_linebreak(self):
         doc = Document("Foo\\\nBar\n")
-        self._check_repr_matches(doc.children[0].children[1], "span_token.LineBreak content='' soft=False")
+        self._check_repr_matches(doc.children[0].children[1], "span_token.LineBreak content='\\\\' soft=False")
 
     def test_rawtext(self):
         doc = Document("Foo\n")
         self._check_repr_matches(doc.children[0].children[0], "span_token.RawText content='Foo'")
```

### Comparing `mistletoe-1.0.1/test/test_span_token.py` & `mistletoe-1.1.0/test/test_span_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,17 +161,28 @@
     def test_invalid_html_entities(self):
         text = '&nbsp &x; &#; &#x; &#87654321; &#abcdef0; &ThisIsNotDefined; &hi?;'
         tokens = span_token.tokenize_inner(text)
         self.assertEqual(tokens[0].content, text)
 
 
 class TestLineBreak(unittest.TestCase):
-    def test_parse(self):
+    def test_parse_soft_break(self):
+        token, = span_token.tokenize_inner('\n')
+        self.assertIsInstance(token, span_token.LineBreak)
+        self.assertTrue(token.soft)
+
+    def test_parse_hard_break_with_double_blanks(self):
         token, = span_token.tokenize_inner('  \n')
         self.assertIsInstance(token, span_token.LineBreak)
+        self.assertFalse(token.soft)
+
+    def test_parse_hard_break_with_backslash(self):
+        _, token, = span_token.tokenize_inner(' \\\n')
+        self.assertIsInstance(token, span_token.LineBreak)
+        self.assertFalse(token.soft)
 
 
 class TestContains(unittest.TestCase):
     def test_contains(self):
         token = next(iter(span_token.tokenize_inner('**with some *emphasis* text**')))
         self.assertTrue('text' in token)
         self.assertTrue('emphasis' in token)
```

### Comparing `mistletoe-1.0.1/test/test_traverse.py` & `mistletoe-1.1.0/test/test_traverse.py`

 * *Files identical despite different names*

