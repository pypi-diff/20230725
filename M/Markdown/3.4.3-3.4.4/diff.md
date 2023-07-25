# Comparing `tmp/Markdown-3.4.3.tar.gz` & `tmp/Markdown-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/markdown/markdown/dist/.tmp-s10jhs02/Markdown-3.4.3.tar", last modified: Thu Mar 23 13:15:38 2023, max compression
+gzip compressed data, was "/home/runner/work/markdown/markdown/dist/.tmp-w_g7tn44/Markdown-3.4.4.tar", last modified: Tue Jul 25 15:13:32 2023, max compression
```

## Comparing `Markdown-3.4.3.tar` & `Markdown-3.4.4.tar`

### file list

```diff
@@ -1,400 +1,398 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-23 13:15:27.000000 Markdown-3.4.3/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-23 13:15:27.000000 Markdown-3.4.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-23 13:15:27.000000 Markdown-3.4.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/Markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-03-23 13:15:38.000000 Markdown-3.4.3/Markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12466 2023-03-23 13:15:38.000000 Markdown-3.4.3/Markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 13:15:38.000000 Markdown-3.4.3/Markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-23 13:15:38.000000 Markdown-3.4.3/Markdown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-23 13:15:38.000000 Markdown-3.4.3/Markdown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-23 13:15:38.000000 Markdown-3.4.3/Markdown.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6527 2023-03-23 13:15:38.000000 Markdown-3.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-03-23 13:15:27.000000 Markdown-3.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-23 13:15:27.000000 Markdown-3.4.3/doc-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/authors.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/docs/change_log/
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-2.0.md
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-2.1.md
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-2.2.md
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-2.3.md
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-2.4.md
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-2.5.md
--rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-2.6.md
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-3.0.md
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-3.1.md
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-3.2.md
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-3.3.md
--rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/change_log/release-3.4.md
--rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)    23251 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/docs/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/abbreviations.md
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/admonition.md
--rw-r--r--   0 runner    (1001) docker     (123)    42395 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/api.md
--rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/attr_list.md
--rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/code_hilite.md
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/definition_lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/extra.md
--rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/fenced_code_blocks.md
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/footnotes.md
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/legacy_attrs.md
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/legacy_em.md
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/md_in_html.md
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/meta_data.md
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/nl2br.md
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/sane_lists.md
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/smarty.md
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/tables.md
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/toc.md
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/extensions/wikilinks.md
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/install.md
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/py.png
--rw-r--r--   0 runner    (1001) docker     (123)    10268 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-03-23 13:15:27.000000 Markdown-3.4.3/docs/test_tools.md
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-23 13:15:27.000000 Markdown-3.4.3/makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/__meta__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/blockparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    24893 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/blockprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/markdown/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/abbr.py
--rw-r--r--   0 runner    (1001) docker     (123)     5847 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/admonition.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/attr_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    12906 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/codehilite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/def_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/fenced_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    15851 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/footnotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/legacy_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/legacy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/md_in_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/nl2br.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/sane_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/smarty.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/toc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/extensions/wikilinks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13038 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/htmlparser.py
--rw-r--r--   0 runner    (1001) docker     (123)    29654 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/inlinepatterns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/postprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    16240 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/treeprocessors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-03-23 13:15:27.000000 Markdown-3.4.3/markdown/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-03-23 13:15:27.000000 Markdown-3.4.3/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-03-23 13:15:27.000000 Markdown-3.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 13:15:38.000000 Markdown-3.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/basic/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/amps-and-angle-encoding.html
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/amps-and-angle-encoding.txt
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/angle-links-and-img.html
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/angle-links-and-img.txt
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/auto-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/auto-links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/backlash-escapes.html
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/backlash-escapes.txt
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/blockquotes-with-code-blocks.html
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/blockquotes-with-code-blocks.txt
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/codeblock-in-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/codeblock-in-list.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/hard-wrapped.html
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/hard-wrapped.txt
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/horizontal-rules.html
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/horizontal-rules.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/links-inline.html
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/links-inline.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/links-reference.html
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/links-reference.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/literal-quotes.html
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/literal-quotes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/markdown-documentation-basics.html
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/markdown-documentation-basics.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31591 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/markdown-syntax.html
--rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/markdown-syntax.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/nested-blockquotes.html
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/nested-blockquotes.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/ordered-and-unordered-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/ordered-and-unordered-list.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/strong-and-em-together.html
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/strong-and-em-together.txt
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/tabs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/tidyness.html
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/basic/tidyness.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/admonition.html
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/admonition.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/attr_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/attr_list.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/codehilite.html
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/codehilite.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/extensions/extra/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/def-in-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/def-in-list.txt
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/extra_config.html
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/extra_config.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/footnote.html
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/footnote.txt
--rw-r--r--   0 runner    (1001) docker     (123)   290757 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/footnote_many_footnotes.html
--rw-r--r--   0 runner    (1001) docker     (123)    48144 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/footnote_many_footnotes.txt
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/footnote_placeholder.html
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/footnote_placeholder.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/footnote_placeholder_depth.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/footnote_placeholder_depth.txt
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/loose_def_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/loose_def_list.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31591 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/markdown-syntax.html
--rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/markdown-syntax.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/named_markers.html
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/named_markers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/raw-html.html
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/raw-html.txt
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/simple_def-lists.html
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/extra/simple_def-lists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/github_flavored.html
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/github_flavored.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/nl2br_w_attr_list.html
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/nl2br_w_attr_list.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/sane_lists.html
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/sane_lists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/smarty.html
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/smarty.txt
--rw-r--r--   0 runner    (1001) docker     (123)    31178 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc.html
--rw-r--r--   0 runner    (1001) docker     (123)    25820 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc_invalid.html
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc_invalid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc_nested.html
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc_nested.txt
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc_nested2.html
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc_nested2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc_nested_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc_nested_list.txt
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc_out_of_order.html
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/toc_out_of_order.txt
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/wikilinks.html
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/extensions/wikilinks.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/misc/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/CRLF_line_ends.html
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/CRLF_line_ends.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/adjacent-headers.html
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/adjacent-headers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/arabic.html
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/arabic.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/autolinks_with_asterisks.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/autolinks_with_asterisks.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/autolinks_with_asterisks_russian.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/autolinks_with_asterisks_russian.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/backtick-escape.html
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/backtick-escape.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/bidi.html
--rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/bidi.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/blank-block-quote.html
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/blank-block-quote.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/blank_lines_in_codeblocks.html
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/blank_lines_in_codeblocks.txt
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/blockquote-below-paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/blockquote-below-paragraph.txt
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/blockquote-hr.html
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/blockquote-hr.txt
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/blockquote.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/bold_links.html
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/bold_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/br.html
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/br.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/bracket_re.html
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/bracket_re.txt
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/brackets-in-img-title.html
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/brackets-in-img-title.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/code-first-line.html
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/code-first-line.txt
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/em-around-links.html
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/em-around-links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/em_strong.html
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/em_strong.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/em_strong_complex.html
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/em_strong_complex.txt
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/email.html
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/email.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/escaped_links.html
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/escaped_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/funky-list.html
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/funky-list.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/h1.html
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/h1.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/hash.html
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/hash.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/header-in-lists.html
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/header-in-lists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/headers.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/headers.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/hline.html
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/hline.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/image-2.html
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/image-2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/image_in_links.html
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/image_in_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/ins-at-start-of-paragraph.html
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/ins-at-start-of-paragraph.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/inside_html.html
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/inside_html.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/japanese.html
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/japanese.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lazy-block-quote.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lazy-block-quote.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/link-with-parenthesis.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/link-with-parenthesis.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists.html
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists2.html
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists2.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists3.html
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists3.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists4.html
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists4.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists5.html
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists5.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists6.html
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists6.txt
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists7.html
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists7.txt
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists8.html
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/lists8.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/missing-link-def.html
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/missing-link-def.txt
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/multi-paragraph-block-quote.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/multi-paragraph-block-quote.txt
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/multi-test.html
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/multi-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/nested-lists.html
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/nested-lists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/nested-patterns.html
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/nested-patterns.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/normalize.html
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/normalize.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/numeric-entity.html
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/numeric-entity.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/para-with-hr.html
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/para-with-hr.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/russian.html
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/russian.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/smart_em.html
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/smart_em.txt
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/some-test.html
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/some-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/span.html
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/span.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/strong-with-underscores.html
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/strong-with-underscores.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/stronintags.html
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/stronintags.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/tabs-in-lists.html
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/tabs-in-lists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/two-spaces.html
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/two-spaces.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/uche.html
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/uche.txt
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/underscores.html
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/underscores.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/url_spaces.html
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/misc/url_spaces.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/pl/Tests_2004/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Amps and angle encoding.html
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Auto links.html
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Backslash escapes.html
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Blockquotes with code blocks.html
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Hard-wrapped paragraphs with list-like lines.html
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Horizontal rules.html
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Inline HTML (Advanced).html
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Inline HTML (Simple).html
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Inline HTML comments.html
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Links, inline style.html
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Links, reference style.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Literal quotes in titles.html
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Markdown Documentation - Basics.html
--rw-r--r--   0 runner    (1001) docker     (123)    31785 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Markdown Documentation - Syntax.html
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Nested blockquotes.html
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Ordered and unordered lists.html
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Strong and em together.html
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Tidyness.html
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Yuri-Attributes.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Yuri-Email.html
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Yuri-Footnotes.html
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2004/Yuri-Links-in-Headers.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/pl/Tests_2007/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Amps and angle encoding.html
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Auto links.html
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Backslash escapes.html
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Blockquotes with code blocks.html
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Code Blocks.html
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Code Spans.html
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Hard-wrapped paragraphs with list-like lines.html
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Horizontal rules.html
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Images.html
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Inline HTML (Advanced).html
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Inline HTML (Simple).html
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Inline HTML comments.html
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Links, inline style.html
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Links, reference style.html
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Links, shortcut references.html
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Literal quotes in titles.html
--rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Markdown Documentation - Basics.html
--rw-r--r--   0 runner    (1001) docker     (123)    31785 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Markdown Documentation - Syntax.html
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Nested blockquotes.html
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Ordered and unordered lists.html
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Strong and em together.html
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/pl/Tests_2007/Tidyness.html
--rw-r--r--   0 runner    (1001) docker     (123)    33487 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_apis.py
--rw-r--r--   0 runner    (1001) docker     (123)    24643 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/test_syntax/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/test_syntax/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/blocks/test_blockquotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/blocks/test_code_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/blocks/test_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/blocks/test_hr.py
--rw-r--r--   0 runner    (1001) docker     (123)    40929 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/blocks/test_html_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/blocks/test_paragraphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/test_syntax/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_abbr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_admonition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_attr_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    29152 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_code_hilite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_def_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    30861 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_fenced_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    11393 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_footnotes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_legacy_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_legacy_em.py
--rw-r--r--   0 runner    (1001) docker     (123)    31266 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_md_in_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_smarty.py
--rw-r--r--   0 runner    (1001) docker     (123)    26392 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)    26166 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/extensions/test_toc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 13:15:38.000000 Markdown-3.4.3/tests/test_syntax/inline/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/inline/test_autolinks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/inline/test_emphasis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/inline/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/inline/test_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/inline/test_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-23 13:15:27.000000 Markdown-3.4.3/tests/test_syntax/inline/test_raw_html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-25 15:13:14.000000 Markdown-3.4.4/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-25 15:13:14.000000 Markdown-3.4.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-07-25 15:13:14.000000 Markdown-3.4.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/Markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-25 15:13:32.000000 Markdown-3.4.4/Markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12396 2023-07-25 15:13:32.000000 Markdown-3.4.4/Markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:13:32.000000 Markdown-3.4.4/Markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-25 15:13:32.000000 Markdown-3.4.4/Markdown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-25 15:13:32.000000 Markdown-3.4.4/Markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-25 15:13:32.000000 Markdown-3.4.4/Markdown.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-07-25 15:13:32.000000 Markdown-3.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-25 15:13:14.000000 Markdown-3.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/authors.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/docs/change_log/
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-2.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-2.1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-2.2.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-2.3.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-2.4.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-2.5.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11513 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-2.6.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-3.0.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-3.1.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-3.2.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-3.3.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5381 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/change_log/release-3.4.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)    26457 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/docs/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/abbreviations.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/admonition.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42395 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/api.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7099 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/attr_list.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10283 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/code_hilite.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/definition_lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/extra.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/fenced_code_blocks.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/footnotes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/legacy_attrs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/legacy_em.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/md_in_html.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/meta_data.md
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/nl2br.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/sane_lists.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/smarty.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/toc.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/extensions/wikilinks.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/install.md
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/py.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10268 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-25 15:13:14.000000 Markdown-3.4.4/docs/test_tools.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-25 15:13:14.000000 Markdown-3.4.4/makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/__meta__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/blockparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24965 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/blockprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14729 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/markdown/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/abbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/admonition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/attr_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12966 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/codehilite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/def_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7240 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/fenced_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15887 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/legacy_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/legacy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15884 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/md_in_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/nl2br.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/sane_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/smarty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/toc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/extensions/wikilinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/htmlparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30121 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/inlinepatterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/postprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16345 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/treeprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11678 2023-07-25 15:13:14.000000 Markdown-3.4.4/markdown/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-07-25 15:13:14.000000 Markdown-3.4.4/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-07-25 15:13:14.000000 Markdown-3.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:13:32.000000 Markdown-3.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/basic/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/amps-and-angle-encoding.html
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/amps-and-angle-encoding.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/angle-links-and-img.html
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/angle-links-and-img.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/auto-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/auto-links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/backlash-escapes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/backlash-escapes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/blockquotes-with-code-blocks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/blockquotes-with-code-blocks.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/codeblock-in-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/codeblock-in-list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/hard-wrapped.html
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/hard-wrapped.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/horizontal-rules.html
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/horizontal-rules.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/links-inline.html
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/links-inline.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/links-reference.html
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/links-reference.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/literal-quotes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/literal-quotes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/markdown-documentation-basics.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/markdown-documentation-basics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31591 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/markdown-syntax.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/markdown-syntax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/nested-blockquotes.html
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/nested-blockquotes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/ordered-and-unordered-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/ordered-and-unordered-list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/strong-and-em-together.html
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/strong-and-em-together.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/tabs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/tidyness.html
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/basic/tidyness.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/admonition.html
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/admonition.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/attr_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/attr_list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/codehilite.html
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/codehilite.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/extensions/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/def-in-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/def-in-list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/extra_config.html
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/extra_config.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3992 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/footnote.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/footnote.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   290757 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/footnote_many_footnotes.html
+-rw-r--r--   0 runner    (1001) docker     (123)    48144 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/footnote_many_footnotes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/footnote_placeholder.html
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/footnote_placeholder.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/footnote_placeholder_depth.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/footnote_placeholder_depth.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/loose_def_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/loose_def_list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31591 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/markdown-syntax.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27432 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/markdown-syntax.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/named_markers.html
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/named_markers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/raw-html.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/raw-html.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/simple_def-lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/extra/simple_def-lists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/github_flavored.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/github_flavored.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/nl2br_w_attr_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/nl2br_w_attr_list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/sane_lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/sane_lists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31178 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc.html
+-rw-r--r--   0 runner    (1001) docker     (123)    25820 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc_invalid.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc_invalid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc_nested.html
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc_nested.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc_nested2.html
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc_nested2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc_nested_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc_nested_list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc_out_of_order.html
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/toc_out_of_order.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/wikilinks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/extensions/wikilinks.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/CRLF_line_ends.html
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/CRLF_line_ends.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/adjacent-headers.html
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/adjacent-headers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/arabic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/autolinks_with_asterisks.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/autolinks_with_asterisks.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/autolinks_with_asterisks_russian.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/autolinks_with_asterisks_russian.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/backtick-escape.html
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/backtick-escape.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/bidi.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7577 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/bidi.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/blank-block-quote.html
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/blank-block-quote.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/blank_lines_in_codeblocks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/blank_lines_in_codeblocks.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/blockquote-below-paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/blockquote-below-paragraph.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/blockquote-hr.html
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/blockquote-hr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/blockquote.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/bold_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/bold_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/br.html
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/br.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/bracket_re.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/bracket_re.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/brackets-in-img-title.html
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/brackets-in-img-title.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/code-first-line.html
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/code-first-line.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/em-around-links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/em-around-links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/em_strong.html
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/em_strong.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/em_strong_complex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/em_strong_complex.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/email.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/escaped_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/escaped_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/funky-list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/funky-list.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/h1.html
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/h1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/hash.html
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/hash.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/header-in-lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/header-in-lists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/headers.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/headers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/hline.html
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/hline.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/image-2.html
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/image-2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/image_in_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/image_in_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/ins-at-start-of-paragraph.html
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/ins-at-start-of-paragraph.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/inside_html.html
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/inside_html.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/japanese.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/japanese.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lazy-block-quote.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lazy-block-quote.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/link-with-parenthesis.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/link-with-parenthesis.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists2.html
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists3.html
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists4.html
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists4.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists5.html
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists5.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists6.html
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists6.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists7.html
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists8.html
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/lists8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/missing-link-def.html
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/missing-link-def.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/multi-paragraph-block-quote.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/multi-paragraph-block-quote.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/multi-test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/multi-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/nested-lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/nested-lists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/nested-patterns.html
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/nested-patterns.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/normalize.html
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/normalize.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/numeric-entity.html
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/numeric-entity.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/para-with-hr.html
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/para-with-hr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/russian.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/russian.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/smart_em.html
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/smart_em.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/some-test.html
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/some-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/span.html
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/span.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/strong-with-underscores.html
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/strong-with-underscores.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/stronintags.html
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/stronintags.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/tabs-in-lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/tabs-in-lists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/two-spaces.html
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/two-spaces.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/uche.html
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/uche.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/underscores.html
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/underscores.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/url_spaces.html
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/misc/url_spaces.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/pl/Tests_2004/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Amps and angle encoding.html
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Auto links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Backslash escapes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Blockquotes with code blocks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Hard-wrapped paragraphs with list-like lines.html
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Horizontal rules.html
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Inline HTML (Advanced).html
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Inline HTML (Simple).html
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Inline HTML comments.html
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Links, inline style.html
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Links, reference style.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Literal quotes in titles.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Markdown Documentation - Basics.html
+-rw-r--r--   0 runner    (1001) docker     (123)    31785 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Markdown Documentation - Syntax.html
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Nested blockquotes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Ordered and unordered lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Strong and em together.html
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Tidyness.html
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Yuri-Attributes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Yuri-Email.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Yuri-Footnotes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2004/Yuri-Links-in-Headers.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/pl/Tests_2007/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Amps and angle encoding.html
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Auto links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Backslash escapes.html
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Blockquotes with code blocks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Code Blocks.html
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Code Spans.html
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Hard-wrapped paragraphs with list-like lines.html
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Horizontal rules.html
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Images.html
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Inline HTML (Advanced).html
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Inline HTML (Simple).html
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Inline HTML comments.html
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Links, inline style.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Links, reference style.html
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Links, shortcut references.html
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Literal quotes in titles.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Markdown Documentation - Basics.html
+-rw-r--r--   0 runner    (1001) docker     (123)    31785 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Markdown Documentation - Syntax.html
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Nested blockquotes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Ordered and unordered lists.html
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Strong and em together.html
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/pl/Tests_2007/Tidyness.html
+-rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23467 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/test_syntax/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/test_syntax/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/blocks/test_blockquotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/blocks/test_code_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18618 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/blocks/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/blocks/test_hr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40931 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/blocks/test_html_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/blocks/test_paragraphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/test_syntax/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_abbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_admonition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_attr_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29185 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_code_hilite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_def_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30871 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_fenced_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_legacy_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_legacy_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31272 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_md_in_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_smarty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26394 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26953 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/extensions/test_toc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:13:32.000000 Markdown-3.4.4/tests/test_syntax/inline/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/inline/test_autolinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/inline/test_emphasis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/inline/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6969 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/inline/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/inline/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-07-25 15:13:14.000000 Markdown-3.4.4/tests/test_syntax/inline/test_raw_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-25 15:13:14.000000 Markdown-3.4.4/tox.ini
```

### Comparing `Markdown-3.4.3/LICENSE.md` & `Markdown-3.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/Markdown.egg-info/PKG-INFO` & `Markdown-3.4.4/Markdown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Markdown
-Version: 3.4.3
+Version: 3.4.4
 Summary: Python implementation of John Gruber's Markdown.
 Author: Manfred Stienstra, Yuri Takhteyev
 Author-email: Waylan limberg <python.markdown@gmail.com>
 Maintainer: Isaac Muse
 Maintainer-email: Waylan Limberg <python.markdown@gmail.com>
 License: Copyright 2007, 2008 The Python Markdown Project (v. 1.7 and later)
         Copyright 2004, 2005, 2006 Yuri Takhteyev (v. 0.2-1.6b)
@@ -62,14 +62,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+Provides-Extra: docs
 License-File: LICENSE.md
 
 [Python-Markdown][]
 ===================
 
 [![Build Status][build-button]][build]
 [![Coverage Status][codecov-button]][codecov]
```

### Comparing `Markdown-3.4.3/Markdown.egg-info/SOURCES.txt` & `Markdown-3.4.4/Markdown.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 INSTALL.md
 LICENSE.md
 MANIFEST.in
 README.md
-doc-requirements.txt
 makefile
 mkdocs.yml
 pyproject.toml
+tox.ini
 Markdown.egg-info/PKG-INFO
 Markdown.egg-info/SOURCES.txt
 Markdown.egg-info/dependency_links.txt
 Markdown.egg-info/entry_points.txt
 Markdown.egg-info/requires.txt
 Markdown.egg-info/top_level.txt
 docs/authors.md
@@ -136,16 +136,14 @@
 tests/extensions/codehilite.txt
 tests/extensions/github_flavored.html
 tests/extensions/github_flavored.txt
 tests/extensions/nl2br_w_attr_list.html
 tests/extensions/nl2br_w_attr_list.txt
 tests/extensions/sane_lists.html
 tests/extensions/sane_lists.txt
-tests/extensions/smarty.html
-tests/extensions/smarty.txt
 tests/extensions/toc.html
 tests/extensions/toc.txt
 tests/extensions/toc_invalid.html
 tests/extensions/toc_invalid.txt
 tests/extensions/toc_nested.html
 tests/extensions/toc_nested.txt
 tests/extensions/toc_nested2.html
```

### Comparing `Markdown-3.4.3/Markdown.egg-info/entry_points.txt` & `Markdown-3.4.4/Markdown.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/PKG-INFO` & `Markdown-3.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Markdown
-Version: 3.4.3
+Version: 3.4.4
 Summary: Python implementation of John Gruber's Markdown.
 Author: Manfred Stienstra, Yuri Takhteyev
 Author-email: Waylan limberg <python.markdown@gmail.com>
 Maintainer: Isaac Muse
 Maintainer-email: Waylan Limberg <python.markdown@gmail.com>
 License: Copyright 2007, 2008 The Python Markdown Project (v. 1.7 and later)
         Copyright 2004, 2005, 2006 Yuri Takhteyev (v. 0.2-1.6b)
@@ -62,14 +62,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Text Processing :: Markup :: HTML
 Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+Provides-Extra: docs
 License-File: LICENSE.md
 
 [Python-Markdown][]
 ===================
 
 [![Build Status][build-button]][build]
 [![Coverage Status][codecov-button]][codecov]
```

### Comparing `Markdown-3.4.3/README.md` & `Markdown-3.4.4/README.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/authors.md` & `Markdown-3.4.4/docs/authors.md`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 * __[Isaac Muse](https://github.com/facelessuser)__
 
     @facelessuser joined the team after providing a number of helpful patches
     and has been assisting with maintenance, reviewing pull requests and ticket
     triage.
 
-* __[Yuri Takteyev](https://github.com/yuri)__
+* __[Yuri Takhteyev](https://github.com/yuri)__
 
     Yuri wrote most of the code found in version 1.x while procrastinating his
     Ph.D. Various pieces of his code still exist, most notably the basic
     structure.
 
 * __Manfed Stienstra__
```

### Comparing `Markdown-3.4.3/docs/change_log/index.md` & `Markdown-3.4.4/docs/change_log/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 title: Change Log
 
 Python-Markdown Change Log
 =========================
 
+July 25, 2023: version 3.4.4 (a bug-fix release).
+
+* Add a special case for initial `'s` to smarty extension (#1305).
+* Unescape any backslash escaped inline raw HTML (#1358).
+* Unescape backslash escaped TOC token names (#1360).
+
 March 23, 2023: version 3.4.3 (a bug-fix release).
 
 * Restore console script (#1327).
 
 March 22, 2023: version 3.4.2 (a bug-fix release).
 
 * Improve standalone * and _ parsing (#1300).
@@ -178,18 +184,18 @@
 with WikiLinks (note the s) ext (uses bracketed links instead of CamelCase)
 and various bug fixes.
 
 August 18 2008: Reorganized directory structure. Added a 'docs' directory
 and moved all extensions into a 'markdown-extensions' package.
 Added additional documentation and a few bug fixes. (v2.0-beta)
 
-August 4 2008: Updated included extensions to ElementTree. Added a
+August 4 2008: Updated included extensions to `ElementTree`. Added a
 separate command line script. (v2.0-alpha)
 
-July 2008: Switched from home-grown NanoDOM to ElementTree and
+July 2008: Switched from home-grown `NanoDOM` to `ElementTree` and
 various related bugs (thanks Artem Yunusov).
 
 June 2008: Fixed issues with nested inline patterns and cleaned
 up testing framework (thanks Artem Yunusov).
 
 May 2008: Added a number of additional extensions to the
 distribution and other minor changes. Moved repository to git from svn.
@@ -306,15 +312,15 @@
 attribute support.
 
 Sept. 1, 2005: Changed the way headers are handled to allow inline
 syntax in headers (e.g. links) and got the lists to use p-tags
 correctly (v. 0.8)
 
 Aug. 29, 2005: Added flexible tabs, fixed a few small issues, added
-basic support for footnotes.  Got rid of xml.dom.minidom and added
+basic support for footnotes.  Got rid of `xml.dom.minidom` and added
 pretty-printing. (v. 0.7)
 
 Aug. 13, 2005: Fixed a number of small bugs in order to conform to the
 test suite.  (v. 0.6)
 
 Aug. 11, 2005: Added support for inline HTML and entities, inline
 images, auto-links, underscore emphasis. Cleaned up and refactored the
```

#### html2text {}

```diff
@@ -1,11 +1,14 @@
-title: Change Log Python-Markdown Change Log ========================= March
-23, 2023: version 3.4.3 (a bug-fix release). * Restore console script (#1327).
-March 22, 2023: version 3.4.2 (a bug-fix release). * Improve standalone * and _
-parsing (#1300). * Consider `
+title: Change Log Python-Markdown Change Log ========================= July 25,
+2023: version 3.4.4 (a bug-fix release). * Add a special case for initial `'s`
+to smarty extension (#1305). * Unescape any backslash escaped inline raw HTML
+(#1358). * Unescape backslash escaped TOC token names (#1360). March 23, 2023:
+version 3.4.3 (a bug-fix release). * Restore console script (#1327). March 22,
+2023: version 3.4.2 (a bug-fix release). * Improve standalone * and _ parsing
+(#1300). * Consider `
 ` HTML tag a block-level element (#1309). * Officially support Python 3.11. *
 Switch from `setup.py` to `pyproject.toml`. July 15, 2022: version 3.4.1 (a
 bug-fix release). * Fix an import issue with `importlib.util` (#1274). July 15,
 2022: version 3.4 ([Notes](release-3.4.md)). May 5, 2022: version 3.3.7 (a bug-
 fix release). * Disallow square brackets in reference link ids (#1209). *
 Retain configured `pygments_style` after first code block (#1240). * Ensure
 fenced code attributes are properly escaped (#1247). Nov 17, 2021: version
@@ -81,17 +84,17 @@
 Added `treap` implementation, then replaced with OrderedDict. Renamed various
 processors to better reflect what they actually do. Refactored footnote ext to
 match PHP Extra's output. Sept 2008: Moved `prettifyTree` to a Postprocessor,
 replaced WikiLink ext with WikiLinks (note the s) ext (uses bracketed links
 instead of CamelCase) and various bug fixes. August 18 2008: Reorganized
 directory structure. Added a 'docs' directory and moved all extensions into a
 'markdown-extensions' package. Added additional documentation and a few bug
-fixes. (v2.0-beta) August 4 2008: Updated included extensions to ElementTree.
+fixes. (v2.0-beta) August 4 2008: Updated included extensions to `ElementTree`.
 Added a separate command line script. (v2.0-alpha) July 2008: Switched from
-home-grown NanoDOM to ElementTree and various related bugs (thanks Artem
+home-grown `NanoDOM` to `ElementTree` and various related bugs (thanks Artem
 Yunusov). June 2008: Fixed issues with nested inline patterns and cleaned up
 testing framework (thanks Artem Yunusov). May 2008: Added a number of
 additional extensions to the distribution and other minor changes. Moved
 repository to git from svn. Mar 2008: Refactored extension API to accept either
 an extension name (as a string) or an instance of an extension (Thanks David
 Wolever). Fixed various bugs and added doc strings. Feb 2008: Various bug-fixes
 mostly regarding extensions. Feb 18, 2008: Version 1.7. Feb 13, 2008: A little
```

### Comparing `Markdown-3.4.3/docs/change_log/release-2.0.md` & `Markdown-3.4.4/docs/change_log/release-2.0.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/change_log/release-2.1.md` & `Markdown-3.4.4/docs/change_log/release-2.1.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/change_log/release-2.2.md` & `Markdown-3.4.4/docs/change_log/release-2.2.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/change_log/release-2.3.md` & `Markdown-3.4.4/docs/change_log/release-2.3.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/change_log/release-2.4.md` & `Markdown-3.4.4/docs/change_log/release-2.4.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/change_log/release-2.5.md` & `Markdown-3.4.4/docs/change_log/release-2.5.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/change_log/release-2.6.md` & `Markdown-3.4.4/docs/change_log/release-2.6.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/change_log/release-3.0.md` & `Markdown-3.4.4/docs/change_log/release-3.0.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/change_log/release-3.1.md` & `Markdown-3.4.4/docs/change_log/release-3.1.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/change_log/release-3.2.md` & `Markdown-3.4.4/docs/change_log/release-3.2.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/change_log/release-3.3.md` & `Markdown-3.4.4/docs/change_log/release-3.3.md`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 * [Fenced Code Blocks](../extensions/fenced_code_blocks.md) now work with
   [Attribute Lists](../extensions/attr_list.md) when syntax highlighting is disabled.
   Any random HTML attribute can be defined and set on the `<code>` tag of fenced code
   blocks when the `attr_list` extension is enabled (#816).
 
 * The HTML parser has been completely replaced. The new HTML parser is built on Python's
-  [html.parser.HTMLParser](https://docs.python.org/3/library/html.parser.html), which
+  [`html.parser.HTMLParser`](https://docs.python.org/3/library/html.parser.html), which
   alleviates various bugs and simplify maintenance of the code (#803, #830).
 
 * The [Markdown in HTML](../extensions/md_in_html.md) extension has been rebuilt on the
   new HTML Parser, which drastically simplifies it. Note that raw HTML elements with a
   `markdown` attribute defined are now converted to ElementTree Elements and are rendered
   by the serializer. Various bugs have been fixed (#803, #595, #780, and #1012).
```

### Comparing `Markdown-3.4.3/docs/change_log/release-3.4.md` & `Markdown-3.4.4/docs/change_log/release-3.4.md`

 * *Files 1% similar despite different names*

```diff
@@ -107,7 +107,8 @@
 ## Bug fixes
 
 The following bug fixes are included in the 3.4 release:
 
 * Extension entry-points are only loaded if needed (#1216).
 * Added additional checks to the `<pre><code>` handling of
   `PrettifyTreeprocessor` (#1261, #1263).
+* Fix XML deprecation warnings.
```

### Comparing `Markdown-3.4.3/docs/cli.md` & `Markdown-3.4.4/docs/cli.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/contributing.md` & `Markdown-3.4.4/docs/contributing.md`

 * *Files 10% similar despite different names*

```diff
@@ -52,17 +52,24 @@
 
 Feature requests will often be closed with a recommendation that they be
 implemented as third party extensions outside of the core Python-Markdown
 library. Keeping new feature requests implemented as third party extensions
 allows us to keep the maintenance overhead of Python-Markdown to a minimum, so
 that the focus can be on continued stability, bug fixes, and documentation.
 
-Closing an issue does not necessarily mean the end of a discussion. If you
-believe your issue has been closed incorrectly, explain why and we'll consider
-if it needs to be reopened.
+If you intend to submit a fix for your bug or provide an implementation of your
+feature request, it is not necessary to first open an issue. You can report a
+bug or make a feature request as part of a pull request. Of course, if you want
+to receive feedback on how to implement a bug-fix or feature before submitting
+a solution, then it would be appropriate to open an issue first and ask your
+questions there.
+
+Having your issue closed does not necessarily mean the end of a discussion. If
+you believe your issue has been closed incorrectly, explain why and we'll
+consider if it needs to be reopened.
 
 ## Pull Requests
 
 A pull request often represents the start of a discussion, and does not
 necessarily need to be the final, finished submission. In fact, if you discover
 an issue and intend to provide a fix for it, there is no need to open an issue
 first. You can report the issue and provide the fix together in a pull request.
@@ -95,14 +102,20 @@
 Pull requests will generally not be accepted if any tests are failing.
 Therefore, it is recommended that you run the tests before submitting your pull
 request. After making a pull request, check the build status in the
 GitHub interface to ensure that all tests are running as expected. If any checks
 fail, you may push additional commits to your branch. GitHub will add those
 commits to the pull request and rerun the checks.
 
+It is generally best not to squash multiple commits and force-push your changes
+to a pull request. Instead, the maintainers would like to be able to follow the
+series of commits along with the discussion about those changes as they
+progress over time. If your pull request is accepted, it will be squashed at
+that time if deemed appropriate.
+
 ## Style Guides
 
 In an effort to maintain consistency, Python-Markdown adheres to the following
 style guides in its code and documentation. A pull request may be rejected if it
 fails to match the relevant style guides.
 
 ### Code Style Guide
@@ -220,14 +233,42 @@
 
 ```md
 !!! note
 
     This is the content of the note.
 ```
 
+#### Release Notes
+
+Any commit/pull request which changes the behavior of the Markdown library in
+any way must include an entry in the release notes. If a change only alters the
+documentation or tooling for the project, then an entry in the release notes is
+not necessary. The release notes can be found at `docs/change_log`.
+
+Each release must have an entry in `docs/change_log/index.md` which follows the
+format of the existing entries. A MAJOR release (`X.0.0`) and a MINOR release
+(`X.X.0`) should only include a single line in `docs/change_log/index.md` which
+links to a full document outlining all changes included in the release.
+However, a PATCH release (X.X.X) should include a list of single line entries
+summarizing each change directly in the file `docs/change_log/index.md` (see
+[Versions](#versions) for an explanation of MAJOR, MINOR, and PATCH releases).
+The description of each change should include a reference to the relevant
+GitHub issue in the format `#123` (where `123` is the issue number).
+
+Prior to a version being released, the text `*under development*` should be
+used as a placeholder for the release date. That text will be replaced with the
+release date as part of the [release process](#release-process).
+
+If a change is the first since the last release, then the appropriate entries
+and/or files may need to be created and included in a pull request. A pull
+request should not alter an entry for an existing version which has already
+been released, unless it is editing an error in the release notes for that
+version, or is otherwise expressly deemed appropriate by the project
+maintainers.
+
 ### Commit Message Style Guide
 
 Use the present tense ("Add feature" not "Added feature").
 
 Use the imperative mood ("Move item to..." not "Moves item to...").
 
 Limit the first line to 72 characters or less.
@@ -276,49 +317,83 @@
 See the [User Guide] for more information on using virtual environments.
 
 To be able to run the Markdown library directly while working on it, install the
 working copy into the environment in [Development Mode] after activating the
 virtual environment for the first time:
 
 ```sh
-pip install --editable .
+pip install -e .
 ```
 
 Now any saved changes will immediately be available within the virtual
 environment.
 
 You can run the command line script with the following command:
 
 ```sh
 python -m markdown
 ```
 
+Before building the documentation for the first time, you will need to install
+some optional dependencies with the command:
+
+```sh
+pip install -e .[docs]
+```
+
+To build the documentation and serve it locally on a development server, run:
+
+```sh
+mkdocs serve
+```
+
+Then point your browser at `http://127.0.0.1:8000/`. For a complete list of
+options available, view MkDocs' help with the command:
+
+```sh
+mkdocs --help
+```
+
+Before running tests for the first time, you will need to install some optional
+dependencies with the command:
+
+```sh
+pip install -e .[testing]
+```
+
 And you can directly run the tests with:
 
 ```sh
 python -m unittest discover tests
 ```
 
+To get a coverage report after running the tests, use these commands instead:
+
+```sh
+coverage run --source=markdown -m unittest discover tests
+coverage report --show-missing
+```
+
 !!! note
 
     Some tests require the [PyTidyLib] library, which depends on the [HTML Tidy]
     library. If you do not have PyTidyLib installed, the tests which depend upon
     it will be skipped. Given the difficulty in installing the HTML Tidy library
     on many systems, you may choose to leave both libraries uninstalled and
-    depend on the Travis server to run those tests when you submit a pull
-    request.
+    depend on the continuous integration server to run those tests when you
+    submit a pull request.
 
 The above setup will only run tests against the code in one version of Python.
 However,  Python-Markdown supports multiple versions of Python. Therefore, a
 [tox] configuration is included in the repository, which includes test
 environments for all supported Python versions, a [Flake8] test environment, and
 a spellchecker for the documentation. While it is generally fine to leave those
-tests for the Travis server to run when a pull request is submitted, for more
-advanced changes, you may want to run those tests locally. To do so, simply
-install tox:
+tests for the continuous integration server to run when a pull request is
+submitted, for more advanced changes, you may want to run those tests locally.
+To do so, simply install tox:
 
 ```sh
 pip install tox
 ```
 
 Then, to run all configured test environments, simply call the command `tox`
 with no arguments. See help (`tox -h`) for more options.
@@ -333,15 +408,15 @@
     Finally, the `spellchecker` environment requires [aspell] and the
     `aspell-en` dictionary to be installed. Unfortunately, installing those
     dependencies may differ significantly from system to system and is outside
     the scope of this guide.
 
 !!! seealso "See Also"
 
-    Python-Markdown provides [test tools] which simply testing Markdown syntax.
+    Python-Markdown provides [test tools] which simply test Markdown syntax.
     Understanding those tools will often help in understanding why a test may be
     failing.
 
 ## Versions
 
 Python-Markdown follows [Semantic Versioning] and uses the
 `MAJOR.MINOR.PATCH[.dev#|a#|b#|rc#]` format for identifying releases. The status
@@ -417,16 +492,17 @@
     In the event that the deployment fails, the following steps can be taken to
     deploy manually:
 
     - Deploy the release to [PyPI] with the command `make deploy`.
 
     - Deploy an update to the documentation using [MkDocs]. The following example
       assumes that local clones of the [Python-Markdown/markdown] and
-      [Python-Markdown/Python-Markdown.github.io] repositories are in sibling
-      directories named `markdown` and `Python-Markdown.github.io` respectively.
+      [`Python-Markdown/Python-Markdown.github.io`][Python-Markdown/Python-Markdown.github.io]
+      repositories are in sibling directories named `markdown` and `Python-Markdown.github.io`
+      respectively.
 
             cd Python-Markdown.github.io
             mkdocs gh-deploy --config-file ../markdown/mkdocs.yml --remote-branch master
 
 ## Issue and Pull Request Labels
 
 Below are the labels used to track and manages issues and pull requests. The
```

### Comparing `Markdown-3.4.3/docs/extensions/abbreviations.md` & `Markdown-3.4.4/docs/extensions/abbreviations.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/admonition.md` & `Markdown-3.4.4/docs/extensions/admonition.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/api.md` & `Markdown-3.4.4/docs/extensions/api.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/attr_list.md` & `Markdown-3.4.4/docs/extensions/attr_list.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/code_hilite.md` & `Markdown-3.4.4/docs/extensions/code_hilite.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/definition_lists.md` & `Markdown-3.4.4/docs/extensions/definition_lists.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/extra.md` & `Markdown-3.4.4/docs/extensions/extra.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/fenced_code_blocks.md` & `Markdown-3.4.4/docs/extensions/fenced_code_blocks.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/footnotes.md` & `Markdown-3.4.4/docs/extensions/footnotes.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/index.md` & `Markdown-3.4.4/docs/extensions/index.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/legacy_attrs.md` & `Markdown-3.4.4/docs/extensions/legacy_attrs.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/legacy_em.md` & `Markdown-3.4.4/docs/extensions/legacy_em.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/md_in_html.md` & `Markdown-3.4.4/docs/extensions/md_in_html.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/meta_data.md` & `Markdown-3.4.4/docs/extensions/meta_data.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/nl2br.md` & `Markdown-3.4.4/docs/extensions/nl2br.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/sane_lists.md` & `Markdown-3.4.4/docs/extensions/sane_lists.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/smarty.md` & `Markdown-3.4.4/docs/extensions/smarty.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/tables.md` & `Markdown-3.4.4/docs/extensions/tables.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/toc.md` & `Markdown-3.4.4/docs/extensions/toc.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/extensions/wikilinks.md` & `Markdown-3.4.4/docs/extensions/wikilinks.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/favicon.ico` & `Markdown-3.4.4/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/index.md` & `Markdown-3.4.4/docs/index.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,21 +17,31 @@
 -----
 
 The Python-Markdown project is developed with the following goals in mind:
 
 * Maintain a Python library (with an optional CLI wrapper) suited to use in web
   server environments (never raise an exception, never write to stdout, etc.) as
   an implementation of the markdown parser that follows the
-  [syntax rules](https://daringfireball.net/projects/markdown/syntax) and the
-  behavior of the original (markdown.pl) implementation as reasonably as
-  possible (see [differences](#differences) for a few exceptions).
+  [syntax rules][] and the behavior of the original (markdown.pl)
+  implementation as reasonably as possible (see [differences](#differences) for
+  a few exceptions).
 
 * Provide an [Extension API](extensions/api.md) which makes it possible
   to change and/or extend the behavior of the parser.
 
+!!! Note
+
+    *This is not a CommonMark implementation*; nor is it trying to be!
+    Python-Markdown was developed long before the CommonMark specification was
+    released and has always (mostly) followed the [syntax rules][] and behavior
+    of the original reference implementation. No accommodations have been made
+    to address the changes which CommonMark has suggested. It is recommended
+    that you look elsewhere if you want an implementation which follows the
+    CommonMark specification.
+
 Features
 --------
 
 In addition to the basic markdown syntax, Python-Markdown supports the following
 features:
 
 * __International Input__
@@ -87,15 +97,15 @@
     This applies to any block level elements nested in a list, including
     paragraphs, sub-lists, blockquotes, code blocks, etc. They **must** always
     be indented by at least four spaces (or one tab) for each level of nesting.
 
     In the event that one would prefer different behavior,
     [tab_length](reference.md#tab_length) can be set to whatever length is
     desired. Be warned however, as this will affect indentation for all aspects
-    of the syntax (including root level code blocks). Alternatively, a 
+    of the syntax (including root level code blocks). Alternatively, a
     [third party extension] may offer a solution that meets your needs.
 
 * __Consecutive Lists__
 
     While the syntax rules are not clear on this, many implementations (including
     the original) do not end one list and start a second list when the list marker
     (asterisks, pluses, hyphens, and numbers) changes. For consistency,
@@ -105,8 +115,9 @@
 
 Support
 -------
 
 You may report bugs, ask for help, and discuss various other issues on the [bug tracker][].
 
 [third party extension]: https://github.com/Python-Markdown/markdown/wiki/Third-Party-Extensions
+[syntax rules]: https://daringfireball.net/projects/markdown/syntax
 [bug tracker]: https://github.com/Python-Markdown/markdown/issues
```

### Comparing `Markdown-3.4.3/docs/install.md` & `Markdown-3.4.4/docs/install.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/py.png` & `Markdown-3.4.4/docs/py.png`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/reference.md` & `Markdown-3.4.4/docs/reference.md`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/docs/test_tools.md` & `Markdown-3.4.4/docs/test_tools.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 required. While Python-Markdown uses the tools for its own tests, they were
 designed and built so that third party extensions could use them as well.
 Therefore, the tools are importable from `markdown.test_tools`.
 
 The test tools include two different `unittest.TestCase` subclasses:
 `markdown.test_tools.TestCase` and `markdown.test_tools.LegacyTestCase`.
 
-## markdown.test_tools.TestCase
+## `markdown.test_tools.TestCase`
 
 The `markdown.test_tools.TestCase` class is a `unittest.TestCase` subclass with
 a few additional helpers to make testing Markdown output easier.
 
 Properties
 : `default_kwargs`: A `dict` of keywords to pass to Markdown for each
 test. The defaults can be overridden on individual tests.
@@ -62,15 +62,15 @@
                 """
             ),
             # Other keyword arguments to pass to `markdown.markdown`
             output_format='html'
         )
 ```
 
-## markdown.test_tools.LegacyTestCase
+## `markdown.test_tools.LegacyTestCase`
 
 In the past Python-Markdown exclusively used file-based tests. Many of those
 tests still exist in Python-Markdown's test suite, including the test files from
 the [reference implementation][perl] (`markdown.pl`) and [PHP Markdown][PHP].
 Each test consists of a matching pair of text and HTML files. The text file
 contains a snippet of Markdown source text formatted for a specific syntax
 feature and the HTML file contains the expected HTML output of that snippet.
```

### Comparing `Markdown-3.4.3/makefile` & `Markdown-3.4.4/makefile`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/markdown/__init__.py` & `Markdown-3.4.4/markdown/__init__.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/markdown/__main__.py` & `Markdown-3.4.4/markdown/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,10 +142,10 @@
         warn_logger.addHandler(console_handler)
 
     # Run
     markdown.markdownFromFile(**options)
 
 
 if __name__ == '__main__':  # pragma: no cover
-    # Support running module as a commandline command.
-    # `python -m markdown [options] [args]`.
+    # Support running module as a command line command.
+    #     python -m markdown [options] [args]
     run()
```

### Comparing `Markdown-3.4.3/markdown/__meta__.py` & `Markdown-3.4.4/markdown/__meta__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,21 +16,21 @@
 Copyright 2004, 2005, 2006 Yuri Takhteyev (v. 0.2-1.6b)
 Copyright 2004 Manfred Stienstra (the original version)
 
 License: BSD (see LICENSE.md for details).
 """
 
 # __version_info__ format:
-# (major, minor, patch, dev/alpha/beta/rc/final, #)
-# (1, 1, 2, 'dev', 0) => "1.1.2.dev0"
-# (1, 1, 2, 'alpha', 1) => "1.1.2a1"
-# (1, 2, 0, 'beta', 2) => "1.2b2"
-# (1, 2, 0, 'rc', 4) => "1.2rc4"
-# (1, 2, 0, 'final', 0) => "1.2"
-__version_info__ = (3, 4, 3, 'final', 0)
+#     (major, minor, patch, dev/alpha/beta/rc/final, #)
+#     (1, 1, 2, 'dev', 0) => "1.1.2.dev0"
+#     (1, 1, 2, 'alpha', 1) => "1.1.2a1"
+#     (1, 2, 0, 'beta', 2) => "1.2b2"
+#     (1, 2, 0, 'rc', 4) => "1.2rc4"
+#     (1, 2, 0, 'final', 0) => "1.2"
+__version_info__ = (3, 4, 4, 'final', 0)
 
 
 def _get_version(version_info):
     " Returns a PEP 440-compliant version number from version_info. "
     assert len(version_info) == 5
     assert version_info[3] in ('dev', 'alpha', 'beta', 'rc', 'final')
```

### Comparing `Markdown-3.4.3/markdown/blockparser.py` & `Markdown-3.4.4/markdown/blockparser.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import xml.etree.ElementTree as etree
 from . import util
 
 
 class State(list):
     """ Track the current and nested state of the parser.
 
-    This utility class is used to track the state of the BlockParser and
+    This utility class is used to track the state of the `BlockParser` and
     support multiple levels if nesting. It's just a simple API wrapped around
     a list. Each time a state is set, that state is appended to the end of the
     list. Each time a state is reset, that state is removed from the end of
     the list.
 
     Therefore, each time a state is set for a nested block, that state must be
     reset when we back out of that level of nesting or the state could be
@@ -54,18 +54,18 @@
         if len(self):
             return self[-1] == state
         else:
             return False
 
 
 class BlockParser:
-    """ Parse Markdown blocks into an ElementTree object.
+    """ Parse Markdown blocks into an `ElementTree` object.
 
-    A wrapper class that stitches the various BlockProcessors together,
-    looping through them and creating an ElementTree object.
+    A wrapper class that stitches the various `BlockProcessors` together,
+    looping through them and creating an `ElementTree` object.
     """
 
     def __init__(self, md):
         self.blockprocessors = util.Registry()
         self.state = State()
         self.md = md
 
@@ -75,43 +75,43 @@
         Given a list of lines, an ElementTree object (not just a parent
         Element) is created and the root element is passed to the parser
         as the parent. The ElementTree object is returned.
 
         This should only be called on an entire document, not pieces.
 
         """
-        # Create a ElementTree from the lines
+        # Create an `ElementTree` from the lines
         self.root = etree.Element(self.md.doc_tag)
         self.parseChunk(self.root, '\n'.join(lines))
         return etree.ElementTree(self.root)
 
     def parseChunk(self, parent, text):
-        """ Parse a chunk of markdown text and attach to given etree node.
+        """ Parse a chunk of markdown text and attach to given `etree` node.
 
-        While the ``text`` argument is generally assumed to contain multiple
+        While the `text` argument is generally assumed to contain multiple
         blocks which will be split on blank lines, it could contain only one
         block. Generally, this method would be called by extensions when
         block parsing is required.
 
-        The ``parent`` etree Element passed in is altered in place.
+        The `parent` `etree` Element passed in is altered in place.
         Nothing is returned.
 
         """
         self.parseBlocks(parent, text.split('\n\n'))
 
     def parseBlocks(self, parent, blocks):
-        """ Process blocks of markdown text and attach to given etree node.
+        """ Process blocks of markdown text and attach to given `etree` node.
 
-        Given a list of ``blocks``, each blockprocessor is stepped through
+        Given a list of `blocks`, each `blockprocessor` is stepped through
         until there are no blocks left. While an extension could potentially
         call this method directly, it's generally expected to be used
         internally.
 
         This is a public method as an extension may need to add/alter
-        additional BlockProcessors which call this method to recursively
+        additional `BlockProcessors` which call this method to recursively
         parse a nested block.
 
         """
         while blocks:
             for processor in self.blockprocessors:
                 if processor.test(parent, blocks[0]):
                     if processor.run(parent, blocks) is not False:
```

### Comparing `Markdown-3.4.3/markdown/blockprocessors.py` & `Markdown-3.4.4/markdown/blockprocessors.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 CORE MARKDOWN BLOCKPARSER
 ===========================================================================
 
 This parser handles basic parsing of Markdown blocks.  It doesn't concern
 itself with inline elements such as **bold** or *italics*, but rather just
 catches blocks, lists, quotes, etc.
 
-The BlockParser is made up of a bunch of BlockProcessors, each handling a
-different type of block. Extensions may add/replace/remove BlockProcessors
+The `BlockParser` is made up of a bunch of `BlockProcessors`, each handling a
+different type of block. Extensions may add/replace/remove `BlockProcessors`
 as they need to alter how markdown blocks are parsed.
 """
 
 import logging
 import re
 import xml.etree.ElementTree as etree
 from . import util
@@ -56,27 +56,27 @@
     return parser
 
 
 class BlockProcessor:
     """ Base class for block processors.
 
     Each subclass will provide the methods below to work with the source and
-    tree. Each processor will need to define it's own ``test`` and ``run``
-    methods. The ``test`` method should return True or False, to indicate
+    tree. Each processor will need to define it's own `test` and `run`
+    methods. The `test` method should return True or False, to indicate
     whether the current block should be processed by this processor. If the
-    test passes, the parser will call the processors ``run`` method.
+    test passes, the parser will call the processors `run` method.
 
     """
 
     def __init__(self, parser):
         self.parser = parser
         self.tab_length = parser.md.tab_length
 
     def lastChild(self, parent):
-        """ Return the last child of an etree element. """
+        """ Return the last child of an `etree` element. """
         if len(parent):
             return parent[-1]
         else:
             return None
 
     def detab(self, text, length=None):
         """ Remove a tab from the front of each line of the given text. """
@@ -100,51 +100,51 @@
             if lines[i].startswith(' '*self.tab_length*level):
                 lines[i] = lines[i][self.tab_length*level:]
         return '\n'.join(lines)
 
     def test(self, parent, block):
         """ Test for block type. Must be overridden by subclasses.
 
-        As the parser loops through processors, it will call the ``test``
+        As the parser loops through processors, it will call the `test`
         method on each to determine if the given block of text is of that
-        type. This method must return a boolean ``True`` or ``False``. The
+        type. This method must return a boolean `True` or `False`. The
         actual method of testing is left to the needs of that particular
-        block type. It could be as simple as ``block.startswith(some_string)``
+        block type. It could be as simple as `block.startswith(some_string)`
         or a complex regular expression. As the block type may be different
         depending on the parent of the block (i.e. inside a list), the parent
-        etree element is also provided and may be used as part of the test.
+        `etree` element is also provided and may be used as part of the test.
 
         Keywords:
 
-        * ``parent``: A etree element which will be the parent of the block.
+        * ``parent``: An `etree` element which will be the parent of the block.
         * ``block``: A block of text from the source which has been split at
             blank lines.
         """
         pass  # pragma: no cover
 
     def run(self, parent, blocks):
         """ Run processor. Must be overridden by subclasses.
 
         When the parser determines the appropriate type of a block, the parser
         will call the corresponding processor's ``run`` method. This method
         should parse the individual lines of the block and append them to
-        the etree.
+        the `etree`.
 
         Note that both the ``parent`` and ``etree`` keywords are pointers
         to instances of the objects which should be edited in place. Each
         processor must make changes to the existing objects as there is no
         mechanism to return new/different objects to replace them.
 
-        This means that this method should be adding SubElements or adding text
+        This means that this method should be adding `SubElements` or adding text
         to the parent, and should remove (``pop``) or add (``insert``) items to
         the list of blocks.
 
         Keywords:
 
-        * ``parent``: A etree element which is the parent of the current block.
+        * ``parent``: An `etree` element which is the parent of the current block.
         * ``blocks``: A list of all remaining blocks of the document.
         """
         pass  # pragma: no cover
 
 
 class ListIndentProcessor(BlockProcessor):
     """ Process children of list items.
@@ -174,72 +174,72 @@
     def run(self, parent, blocks):
         block = blocks.pop(0)
         level, sibling = self.get_level(parent, block)
         block = self.looseDetab(block, level)
 
         self.parser.state.set('detabbed')
         if parent.tag in self.ITEM_TYPES:
-            # It's possible that this parent has a 'ul' or 'ol' child list
+            # It's possible that this parent has a `ul` or `ol` child list
             # with a member.  If that is the case, then that should be the
             # parent.  This is intended to catch the edge case of an indented
             # list whose first member was parsed previous to this point
-            # see OListProcessor
+            # see `OListProcessor`
             if len(parent) and parent[-1].tag in self.LIST_TYPES:
                 self.parser.parseBlocks(parent[-1], [block])
             else:
-                # The parent is already a li. Just parse the child block.
+                # The parent is already a `li`. Just parse the child block.
                 self.parser.parseBlocks(parent, [block])
         elif sibling.tag in self.ITEM_TYPES:
-            # The sibling is a li. Use it as parent.
+            # The sibling is a `li`. Use it as parent.
             self.parser.parseBlocks(sibling, [block])
         elif len(sibling) and sibling[-1].tag in self.ITEM_TYPES:
             # The parent is a list (``ol`` or ``ul``) which has children.
-            # Assume the last child li is the parent of this block.
+            # Assume the last child `li` is the parent of this block.
             if sibling[-1].text:
-                # If the parent li has text, that text needs to be moved to a p
-                # The p must be 'inserted' at beginning of list in the event
-                # that other children already exist i.e.; a nested sublist.
+                # If the parent `li` has text, that text needs to be moved to a `p`
+                # The `p` must be 'inserted' at beginning of list in the event
+                # that other children already exist i.e.; a nested sub-list.
                 p = etree.Element('p')
                 p.text = sibling[-1].text
                 sibling[-1].text = ''
                 sibling[-1].insert(0, p)
             self.parser.parseChunk(sibling[-1], block)
         else:
             self.create_item(sibling, block)
         self.parser.state.reset()
 
     def create_item(self, parent, block):
-        """ Create a new li and parse the block with it as the parent. """
+        """ Create a new `li` and parse the block with it as the parent. """
         li = etree.SubElement(parent, 'li')
         self.parser.parseBlocks(li, [block])
 
     def get_level(self, parent, block):
         """ Get level of indent based on list level. """
         # Get indent level
         m = self.INDENT_RE.match(block)
         if m:
             indent_level = len(m.group(1))/self.tab_length
         else:
             indent_level = 0
         if self.parser.state.isstate('list'):
-            # We're in a tightlist - so we already are at correct parent.
+            # We're in a tight-list - so we already are at correct parent.
             level = 1
         else:
-            # We're in a looselist - so we need to find parent.
+            # We're in a loose-list - so we need to find parent.
             level = 0
         # Step through children of tree to find matching indent level.
         while indent_level > level:
             child = self.lastChild(parent)
             if (child is not None and
                (child.tag in self.LIST_TYPES or child.tag in self.ITEM_TYPES)):
                 if child.tag in self.LIST_TYPES:
                     level += 1
                 parent = child
             else:
-                # No more child levels. If we're short of indent_level,
+                # No more child levels. If we're short of `indent_level`,
                 # we have a code block. So we stop here.
                 break
         return level, parent
 
 
 class CodeBlockProcessor(BlockProcessor):
     """ Process code blocks. """
@@ -251,22 +251,22 @@
         sibling = self.lastChild(parent)
         block = blocks.pop(0)
         theRest = ''
         if (sibling is not None and sibling.tag == "pre" and
            len(sibling) and sibling[0].tag == "code"):
             # The previous block was a code block. As blank lines do not start
             # new code blocks, append this block to the previous, adding back
-            # linebreaks removed from the split into a list.
+            # line breaks removed from the split into a list.
             code = sibling[0]
             block, theRest = self.detab(block)
             code.text = util.AtomicString(
                 '{}\n{}\n'.format(code.text, util.code_escape(block.rstrip()))
             )
         else:
-            # This is a new codeblock. Create the elements and insert text.
+            # This is a new code block. Create the elements and insert text.
             pre = etree.SubElement(parent, 'pre')
             code = etree.SubElement(pre, 'code')
             block, theRest = self.detab(block)
             code.text = util.AtomicString('%s\n' % util.code_escape(block.rstrip()))
         if theRest:
             # This block contained unindented line(s) after the first indented
             # line. Insert these lines as the first block of the master blocks
@@ -296,15 +296,15 @@
         if sibling is not None and sibling.tag == "blockquote":
             # Previous block was a blockquote so set that as this blocks parent
             quote = sibling
         else:
             # This is a new blockquote. Create a new parent element.
             quote = etree.SubElement(parent, 'blockquote')
         # Recursively parse block with blockquote as parent.
-        # change parser state so blockquotes embedded in lists use p tags
+        # change parser state so blockquotes embedded in lists use `p` tags
         self.parser.state.set('blockquote')
         self.parser.parseChunk(quote, block)
         self.parser.state.reset()
 
     def clean(self, line):
         """ Remove ``>`` from beginning of a line. """
         m = self.RE.match(line)
@@ -317,19 +317,18 @@
 
 
 class OListProcessor(BlockProcessor):
     """ Process ordered list blocks. """
 
     TAG = 'ol'
     # The integer (python string) with which the lists starts (default=1)
-    # Eg: If list is initialized as)
-    #   3. Item
-    # The ol tag will get starts="3" attribute
+    # Example: If list is initialized as: `3. Item`
+    # The `ol` tag will get `starts="3"` attribute
     STARTSWITH = '1'
-    # Lazy ol - ignore startswith
+    # Lazy `ol` - ignore `startswith`
     LAZY_OL = True
     # List of allowed sibling tags.
     SIBLING_TAGS = ['ol', 'ul']
 
     def __init__(self, parser):
         super().__init__(parser)
         # Detect an item (``1. item``). ``group(1)`` contains contents of item.
@@ -341,51 +340,51 @@
         self.INDENT_RE = re.compile(r'^[ ]{%d,%d}((\d+\.)|[*+-])[ ]+.*' %
                                     (self.tab_length, self.tab_length * 2 - 1))
 
     def test(self, parent, block):
         return bool(self.RE.match(block))
 
     def run(self, parent, blocks):
-        # Check fr multiple items in one block.
+        # Check for multiple items in one block.
         items = self.get_items(blocks.pop(0))
         sibling = self.lastChild(parent)
 
         if sibling is not None and sibling.tag in self.SIBLING_TAGS:
             # Previous block was a list item, so set that as parent
             lst = sibling
-            # make sure previous item is in a p- if the item has text,
-            # then it isn't in a p
+            # make sure previous item is in a `p` - if the item has text,
+            # then it isn't in a `p`
             if lst[-1].text:
                 # since it's possible there are other children for this
-                # sibling, we can't just SubElement the p, we need to
+                # sibling, we can't just `SubElement` the `p`, we need to
                 # insert it as the first item.
                 p = etree.Element('p')
                 p.text = lst[-1].text
                 lst[-1].text = ''
                 lst[-1].insert(0, p)
-            # if the last item has a tail, then the tail needs to be put in a p
+            # if the last item has a tail, then the tail needs to be put in a `p`
             # likely only when a header is not followed by a blank line
             lch = self.lastChild(lst[-1])
             if lch is not None and lch.tail:
                 p = etree.SubElement(lst[-1], 'p')
                 p.text = lch.tail.lstrip()
                 lch.tail = ''
 
-            # parse first block differently as it gets wrapped in a p.
+            # parse first block differently as it gets wrapped in a `p`.
             li = etree.SubElement(lst, 'li')
             self.parser.state.set('looselist')
             firstitem = items.pop(0)
             self.parser.parseBlocks(li, [firstitem])
             self.parser.state.reset()
         elif parent.tag in ['ol', 'ul']:
             # this catches the edge case of a multi-item indented list whose
             # first item is in a blank parent-list item:
-            # * * subitem1
-            #     * subitem2
-            # see also ListIndentProcessor
+            #     * * subitem1
+            #         * subitem2
+            # see also `ListIndentProcessor`
             lst = parent
         else:
             # This is a new list so create parent with appropriate tag.
             lst = etree.SubElement(parent, self.TAG)
             # Check if a custom start integer is set
             if not self.LAZY_OL and self.STARTSWITH != '1':
                 lst.attrib['start'] = self.STARTSWITH
@@ -394,15 +393,15 @@
         # Loop through items in block, recursively parsing each with the
         # appropriate parent.
         for item in items:
             if item.startswith(' '*self.tab_length):
                 # Item is indented. Parse with last item as parent
                 self.parser.parseBlocks(lst[-1], [item])
             else:
-                # New item. Create li and parse with it as parent
+                # New item. Create `li` and parse with it as parent
                 li = etree.SubElement(lst, 'li')
                 self.parser.parseBlocks(li, [item])
         self.parser.state.reset()
 
     def get_items(self, block):
         """ Break a block into list items. """
         items = []
@@ -494,15 +493,15 @@
             # Block contains additional lines. Add to  master blocks for later.
             blocks.insert(0, '\n'.join(lines[2:]))
 
 
 class HRProcessor(BlockProcessor):
     """ Process Horizontal Rules. """
 
-    # Python's re module doesn't officially support atomic grouping. However you can fake it.
+    # Python's `re` module doesn't officially support atomic grouping. However you can fake it.
     # See https://stackoverflow.com/a/13577411/866026
     RE = r'^[ ]{0,3}(?=(?P<atomicgroup>(-+[ ]{0,2}){3,}|(_+[ ]{0,2}){3,}|(\*+[ ]{0,2}){3,}))(?P=atomicgroup)[ ]*$'
     # Detect hr on any line of a block.
     SEARCH_RE = re.compile(RE, re.MULTILINE)
 
     def test(self, parent, block):
         m = self.SEARCH_RE.search(block)
@@ -511,25 +510,25 @@
             self.match = m
             return True
         return False
 
     def run(self, parent, blocks):
         block = blocks.pop(0)
         match = self.match
-        # Check for lines in block before hr.
+        # Check for lines in block before `hr`.
         prelines = block[:match.start()].rstrip('\n')
         if prelines:
-            # Recursively parse lines before hr so they get parsed first.
+            # Recursively parse lines before `hr` so they get parsed first.
             self.parser.parseBlocks(parent, [prelines])
         # create hr
         etree.SubElement(parent, 'hr')
-        # check for lines in block after hr.
+        # check for lines in block after `hr`.
         postlines = block[match.end():].lstrip('\n')
         if postlines:
-            # Add lines after hr to master blocks for later parsing.
+            # Add lines after `hr` to master blocks for later parsing.
             blocks.insert(0, postlines)
 
 
 class EmptyBlockProcessor(BlockProcessor):
     """ Process blocks that are empty or start with an empty line. """
 
     def test(self, parent, block):
@@ -546,15 +545,15 @@
             theRest = block[1:]
             if theRest:
                 # Add remaining lines to master blocks for later.
                 blocks.insert(0, theRest)
         sibling = self.lastChild(parent)
         if (sibling is not None and sibling.tag == 'pre' and
            len(sibling) and sibling[0].tag == 'code'):
-            # Last block is a codeblock. Append to preserve whitespace.
+            # Last block is a code block. Append to preserve whitespace.
             sibling[0].text = util.AtomicString(
                 '{}{}'.format(sibling[0].text, filler)
             )
 
 
 class ReferenceProcessor(BlockProcessor):
     """ Process link references. """
@@ -602,15 +601,15 @@
                 # tight-list when a header isn't followed by a blank line.
                 # For example:
                 #
                 #     * # Header
                 #     Line 2 of list item - not part of header.
                 sibling = self.lastChild(parent)
                 if sibling is not None:
-                    # Insetrt after sibling.
+                    # Insert after sibling.
                     if sibling.tail:
                         sibling.tail = '{}\n{}'.format(sibling.tail, block)
                     else:
                         sibling.tail = '\n%s' % block
                 else:
                     # Append to parent.text
                     if parent.text:
```

### Comparing `Markdown-3.4.3/markdown/core.py` & `Markdown-3.4.4/markdown/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,24 +51,24 @@
 
     def __init__(self, **kwargs):
         """
         Creates a new Markdown instance.
 
         Keyword arguments:
 
-        * extensions: A list of extensions.
+        * `extensions`: A list of extensions.
             If an item is an instance of a subclass of `markdown.extension.Extension`, the  instance will be used
             as-is. If an item is of type string, first an entry point will be loaded. If that fails, the string is
-            assumed to use Python dot notation (`path.to.module:ClassName`) to load a markdown.Extension subclass. If
+            assumed to use Python dot notation (`path.to.module:ClassName`) to load a `markdown.Extension` subclass. If
             no class is specified, then a `makeExtension` function is called within the specified module.
-        * extension_configs: Configuration settings for extensions.
-        * output_format: Format of output. Supported formats are:
-            * "xhtml": Outputs XHTML style tags. Default.
-            * "html": Outputs HTML style tags.
-        * tab_length: Length of tabs in the source. Default: 4
+        * `extension_configs`: Configuration settings for extensions.
+        * `output_format`: Format of output. Supported formats are:
+            * `xhtml`: Outputs XHTML style tags. Default.
+            * `html`: Outputs HTML style tags.
+        * `tab_length`: Length of tabs in the source. Default: 4
 
         """
 
         self.tab_length = kwargs.get('tab_length', 4)
 
         self.ESCAPED_CHARS = ['\\', '`', '*', '_', '{', '}', '[', ']',
                               '(', ')', '>', '#', '+', '-', '.', '!']
@@ -99,17 +99,17 @@
 
     def registerExtensions(self, extensions, configs):
         """
         Register extensions with this instance of Markdown.
 
         Keyword arguments:
 
-        * extensions: A list of extensions, which can either
+        * `extensions`: A list of extensions, which can either
            be strings or objects.
-        * configs: A dictionary mapping extension names to config options.
+        * `configs`: A dictionary mapping extension names to `configs` options.
 
         """
         for ext in extensions:
             if isinstance(ext, str):
                 ext = self.build_extension(ext, configs.get(ext, {}))
             if isinstance(ext, Extension):
                 ext.extendMarkdown(self)
@@ -132,15 +132,15 @@
 
         First attempt to load an entry point. The string name must be registered as an entry point in the
         `markdown.extensions` group which points to a subclass of the `markdown.extensions.Extension` class.
         If multiple distributions have registered the same name, the first one found is returned.
 
         If no entry point is found, assume dot notation (`path.to.module:ClassName`). Load the specified class and
         return an instance. If no class is specified, import the module and call a `makeExtension` function and return
-        the Extension instance returned by that function.
+        the `Extension` instance returned by that function.
         """
         configs = dict(configs)
 
         entry_points = [ep for ep in util.get_installed_extensions() if ep.name == ext_name]
         if entry_points:
             ext = entry_points[0].load()
             return ext(**configs)
@@ -158,15 +158,15 @@
             e.args = (message,) + e.args[1:]
             raise
 
         if class_name:
             # Load given class name from module.
             return getattr(module, class_name)(**configs)
         else:
-            # Expect  makeExtension() function to return a class.
+            # Expect  `makeExtension()` function to return a class.
             try:
                 return module.makeExtension(**configs)
             except AttributeError as e:
                 message = e.args[0]
                 message = "Failed to initiate extension " \
                           "'%s': %s" % (ext_name, message)
                 e.args = (message,) + e.args[1:]
@@ -188,15 +188,15 @@
             if hasattr(extension, 'reset'):
                 extension.reset()
 
         return self
 
     def set_output_format(self, format):
         """ Set the output format for the class instance. """
-        self.output_format = format.lower().rstrip('145')  # ignore num
+        self.output_format = format.lower().rstrip('145')  # ignore number
         try:
             self.serializer = self.output_formats[self.output_format]
         except KeyError as e:
             valid_formats = list(self.output_formats.keys())
             valid_formats.sort()
             message = 'Invalid Output Format: "%s". Use one of %s.' \
                 % (self.output_format,
@@ -214,39 +214,39 @@
 
     def convert(self, source):
         """
         Convert markdown to serialized XHTML or HTML.
 
         Keyword arguments:
 
-        * source: Source text as a Unicode string.
+        * `source`: Source text as a Unicode string.
 
         Markdown processing takes place in five steps:
 
-        1. A bunch of "preprocessors" munge the input text.
-        2. BlockParser() parses the high-level structural elements of the
-           pre-processed text into an ElementTree.
-        3. A bunch of "treeprocessors" are run against the ElementTree. One
-           such treeprocessor runs InlinePatterns against the ElementTree,
+        1. A bunch of `preprocessors` munge the input text.
+        2. `BlockParser()` parses the high-level structural elements of the
+           pre-processed text into an `ElementTree`.
+        3. A bunch of `treeprocessors` are run against the `ElementTree`. One
+           such `treeprocessor` runs `InlinePatterns` against the `ElementTree`,
            detecting inline markup.
-        4. Some post-processors are run against the text after the ElementTree
+        4. Some post-processors are run against the text after the `ElementTree`
            has been serialized into text.
         5. The output is written to a string.
 
         """
 
-        # Fixup the source text
+        # Fix up the source text
         if not source.strip():
-            return ''  # a blank unicode string
+            return ''  # a blank Unicode string
 
         try:
             source = str(source)
         except UnicodeDecodeError as e:  # pragma: no cover
-            # Customise error message while maintaining original trackback
-            e.reason += '. -- Note: Markdown only accepts unicode input!'
+            # Customize error message while maintaining original traceback
+            e.reason += '. -- Note: Markdown only accepts Unicode input!'
             raise
 
         # Split into lines and run the line preprocessors.
         self.lines = source.split("\n")
         for prep in self.preprocessors:
             self.lines = prep.run(self.lines)
 
@@ -279,31 +279,31 @@
         # Run the text post-processors
         for pp in self.postprocessors:
             output = pp.run(output)
 
         return output.strip()
 
     def convertFile(self, input=None, output=None, encoding=None):
-        """Converts a markdown file and returns the HTML as a unicode string.
+        """Converts a markdown file and returns the HTML as a Unicode string.
 
-        Decodes the file using the provided encoding (defaults to utf-8),
+        Decodes the file using the provided encoding (defaults to `utf-8`),
         passes the file content to markdown, and outputs the html to either
         the provided stream or the file with provided name, using the same
-        encoding as the source file. The 'xmlcharrefreplace' error handler is
+        encoding as the source file. The `xmlcharrefreplace` error handler is
         used when encoding the output.
 
-        **Note:** This is the only place that decoding and encoding of unicode
-        takes place in Python-Markdown.  (All other code is unicode-in /
-        unicode-out.)
+        **Note:** This is the only place that decoding and encoding of Unicode
+        takes place in Python-Markdown.  (All other code is Unicode-in /
+        Unicode-out.)
 
         Keyword arguments:
 
-        * input: File object or path. Reads from stdin if `None`.
-        * output: File object or path. Writes to stdout if `None`.
-        * encoding: Encoding of input and output files. Defaults to utf-8.
+        * `input`: File object or path. Reads from `stdin` if `None`.
+        * `output`: File object or path. Writes to `stdout` if `None`.
+        * `encoding`: Encoding of input and output files. Defaults to `utf-8`.
 
         """
 
         encoding = encoding or "utf-8"
 
         # Read the source
         if input:
@@ -349,49 +349,49 @@
         return self
 
 
 """
 EXPORTED FUNCTIONS
 =============================================================================
 
-Those are the two functions we really mean to export: markdown() and
-markdownFromFile().
+Those are the two functions we really mean to export: `markdown()` and
+`markdownFromFile()`.
 """
 
 
 def markdown(text, **kwargs):
-    """Convert a markdown string to HTML and return HTML as a unicode string.
+    """Convert a markdown string to HTML and return HTML as a Unicode string.
 
     This is a shortcut function for `Markdown` class to cover the most
-    basic use case.  It initializes an instance of Markdown, loads the
+    basic use case.  It initializes an instance of `Markdown`, loads the
     necessary extensions and runs the parser on the given text.
 
     Keyword arguments:
 
-    * text: Markdown formatted text as Unicode or ASCII string.
+    * `text`: Markdown formatted text as Unicode or ASCII string.
     * Any arguments accepted by the Markdown class.
 
     Returns: An HTML document as a string.
 
     """
     md = Markdown(**kwargs)
     return md.convert(text)
 
 
 def markdownFromFile(**kwargs):
     """Read markdown code from a file and write it to a file or a stream.
 
-    This is a shortcut function which initializes an instance of Markdown,
-    and calls the convertFile method rather than convert.
+    This is a shortcut function which initializes an instance of `Markdown`,
+    and calls the `convertFile` method rather than `convert`.
 
     Keyword arguments:
 
-    * input: a file name or readable object.
-    * output: a file name or writable object.
-    * encoding: Encoding of input and output.
-    * Any arguments accepted by the Markdown class.
+    * `input`: a file name or readable object.
+    * `output`: a file name or writable object.
+    * `encoding`: Encoding of input and output.
+    * Any arguments accepted by the `Markdown` class.
 
     """
     md = Markdown(**kwargs)
     md.convertFile(kwargs.get('input', None),
                    kwargs.get('output', None),
                    kwargs.get('encoding', None))
```

### Comparing `Markdown-3.4.3/markdown/extensions/__init__.py` & `Markdown-3.4.4/markdown/extensions/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 
 from ..util import parseBoolValue
 
 
 class Extension:
     """ Base class for extensions to subclass. """
 
-    # Default config -- to be overridden by a subclass
+    # Default configuration -- to be overridden by a subclass
     # Must be of the following format:
     #     {
     #       'key': ['value', 'description']
     #     }
-    # Note that Extension.setConfig will raise a KeyError
+    # Note that `Extension.setConfig` will raise a `KeyError`
     # if a default is not set here.
     config = {}
 
     def __init__(self, **kwargs):
         """ Initiate Extension and set up configs. """
         self.setConfigs(kwargs)
 
@@ -46,27 +46,27 @@
             return default
 
     def getConfigs(self):
         """ Return all configs settings as a dict. """
         return {key: self.getConfig(key) for key in self.config.keys()}
 
     def getConfigInfo(self):
-        """ Return all config descriptions as a list of tuples. """
+        """ Return all `config` descriptions as a list of tuples. """
         return [(key, self.config[key][1]) for key in self.config.keys()]
 
     def setConfig(self, key, value):
-        """ Set a config setting for `key` with the given `value`. """
+        """ Set a `config` setting for `key` with the given `value`. """
         if isinstance(self.config[key][0], bool):
             value = parseBoolValue(value)
         if self.config[key][0] is None:
             value = parseBoolValue(value, preserve_none=True)
         self.config[key][0] = value
 
     def setConfigs(self, items):
-        """ Set multiple config settings given a dict or list of tuples. """
+        """ Set multiple `config` settings given a dict or list of tuples. """
         if hasattr(items, 'items'):
             # it's a dict
             items = items.items()
         for key, value in items:
             self.setConfig(key, value)
 
     def extendMarkdown(self, md):
```

### Comparing `Markdown-3.4.3/markdown/extensions/abbr.py` & `Markdown-3.4.4/markdown/extensions/abbr.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ==========================================
 
 This extension adds abbreviation handling to Python-Markdown.
 
 See <https://Python-Markdown.github.io/extensions/abbreviations>
 for documentation.
 
-Oringinal code Copyright 2007-2008 [Waylan Limberg](http://achinghead.com/) and
+Original code Copyright 2007-2008 [Waylan Limberg](http://achinghead.com/) and
  [Seemant Kulleen](http://www.kulleen.org/)
 
 All changes Copyright 2008-2014 The Python Markdown Project
 
 License: [BSD](https://opensource.org/licenses/bsd-license.php)
 
 '''
@@ -24,30 +24,30 @@
 import xml.etree.ElementTree as etree
 
 
 class AbbrExtension(Extension):
     """ Abbreviation Extension for Python-Markdown. """
 
     def extendMarkdown(self, md):
-        """ Insert AbbrPreprocessor before ReferencePreprocessor. """
+        """ Insert `AbbrPreprocessor` before `ReferencePreprocessor`. """
         md.parser.blockprocessors.register(AbbrPreprocessor(md.parser), 'abbr', 16)
 
 
 class AbbrPreprocessor(BlockProcessor):
     """ Abbreviation Preprocessor - parse text for abbr references. """
 
     RE = re.compile(r'^[*]\[(?P<abbr>[^\]]*)\][ ]?:[ ]*\n?[ ]*(?P<title>.*)$', re.MULTILINE)
 
     def test(self, parent, block):
         return True
 
     def run(self, parent, blocks):
         '''
         Find and remove all Abbreviation references from the text.
-        Each reference is set as a new AbbrPattern in the markdown instance.
+        Each reference is set as a new `AbbrPattern` in the markdown instance.
 
         '''
         block = blocks.pop(0)
         m = self.RE.search(block)
         if m:
             abbr = m.group('abbr').strip()
             title = m.group('title').strip()
```

### Comparing `Markdown-3.4.3/markdown/extensions/admonition.py` & `Markdown-3.4.4/markdown/extensions/admonition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Admonition extension for Python-Markdown
 ========================================
 
 Adds rST-style admonitions. Inspired by [rST][] feature with the same name.
 
-[rST]: http://docutils.sourceforge.net/docs/ref/rst/directives.html#specific-admonitions  # noqa
+[rST]: http://docutils.sourceforge.net/docs/ref/rst/directives.html#specific-admonitions
 
 See <https://Python-Markdown.github.io/extensions/admonition>
 for documentation.
 
 Original code Copyright [Tiago Serafim](https://www.tiagoserafim.com/).
 
 All changes Copyright The Python Markdown Project
@@ -72,24 +72,24 @@
         if sibling is None or sibling.get('class', '').find(self.CLASSNAME) == -1:
             sibling = None
         else:
             # If the last child is a list and the content is sufficiently indented
             # to be under it, then the content's sibling is in the list.
             last_child = self.lastChild(sibling)
             indent = 0
-            while last_child:
+            while last_child is not None:
                 if (
-                    sibling and block.startswith(' ' * self.tab_length * 2) and
-                    last_child and last_child.tag in ('ul', 'ol', 'dl')
+                    sibling is not None and block.startswith(' ' * self.tab_length * 2) and
+                    last_child is not None and last_child.tag in ('ul', 'ol', 'dl')
                 ):
 
-                    # The expectation is that we'll find an <li> or <dt>.
+                    # The expectation is that we'll find an `<li>` or `<dt>`.
                     # We should get its last child as well.
                     sibling = self.lastChild(last_child)
-                    last_child = self.lastChild(sibling) if sibling else None
+                    last_child = self.lastChild(sibling) if sibling is not None else None
 
                     # Context has been lost at this point, so we must adjust the
                     # text's indentation level so it will be evaluated correctly
                     # under the list.
                     block = block[self.tab_length:]
                     indent += self.tab_length
                 else:
@@ -151,15 +151,15 @@
             # list for future processing.
             blocks.insert(0, theRest)
 
     def get_class_and_title(self, match):
         klass, title = match.group(1).lower(), match.group(2)
         klass = self.RE_SPACES.sub(' ', klass)
         if title is None:
-            # no title was provided, use the capitalized classname as title
+            # no title was provided, use the capitalized class name as title
             # e.g.: `!!! note` will render
             # `<p class="admonition-title">Note</p>`
             title = klass.split(' ', 1)[0].capitalize()
         elif title == '':
             # an explicit blank title should not be rendered
             # e.g.: `!!! warning ""` will *not* render `p` with a title
             title = None
```

### Comparing `Markdown-3.4.3/markdown/extensions/attr_list.py` & `Markdown-3.4.4/markdown/extensions/attr_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Attribute List Extension for Python-Markdown
 ============================================
 
 Adds attribute list syntax. Inspired by
-[maruku](http://maruku.rubyforge.org/proposal.html#attribute_lists)'s
+[Maruku](http://maruku.rubyforge.org/proposal.html#attribute_lists)'s
 feature of the same name.
 
 See <https://Python-Markdown.github.io/extensions/attr_list>
 for documentation.
 
 Original code Copyright 2011 [Waylan Limberg](http://achinghead.com/).
 
@@ -73,41 +73,41 @@
                          r'\u2070-\u218f\u2c00-\u2fef\u3001-\ud7ff'
                          r'\uf900-\ufdcf\ufdf0-\ufffd'
                          r'\:\-\.0-9\u00b7\u0300-\u036f\u203f-\u2040]+')
 
     def run(self, doc):
         for elem in doc.iter():
             if self.md.is_block_level(elem.tag):
-                # Block level: check for attrs on last line of text
+                # Block level: check for `attrs` on last line of text
                 RE = self.BLOCK_RE
                 if isheader(elem) or elem.tag in ['dt', 'td', 'th']:
-                    # header, def-term, or table cell: check for attrs at end of element
+                    # header, def-term, or table cell: check for attributes at end of element
                     RE = self.HEADER_RE
                 if len(elem) and elem.tag == 'li':
-                    # special case list items. children may include a ul or ol.
+                    # special case list items. children may include a `ul` or `ol`.
                     pos = None
-                    # find the ul or ol position
+                    # find the `ul` or `ol` position
                     for i, child in enumerate(elem):
                         if child.tag in ['ul', 'ol']:
                             pos = i
                             break
                     if pos is None and elem[-1].tail:
-                        # use tail of last child. no ul or ol.
+                        # use tail of last child. no `ul` or `ol`.
                         m = RE.search(elem[-1].tail)
                         if m:
                             self.assign_attrs(elem, m.group(1))
                             elem[-1].tail = elem[-1].tail[:m.start()]
                     elif pos is not None and pos > 0 and elem[pos-1].tail:
-                        # use tail of last child before ul or ol
+                        # use tail of last child before `ul` or `ol`
                         m = RE.search(elem[pos-1].tail)
                         if m:
                             self.assign_attrs(elem, m.group(1))
                             elem[pos-1].tail = elem[pos-1].tail[:m.start()]
                     elif elem.text:
-                        # use text. ul is first child.
+                        # use text. `ul` is first child.
                         m = RE.search(elem.text)
                         if m:
                             self.assign_attrs(elem, m.group(1))
                             elem.text = elem.text[:m.start()]
                 elif len(elem) and elem[-1].tail:
                     # has children. Get from tail of last child
                     m = RE.search(elem[-1].tail)
@@ -123,33 +123,33 @@
                     if m:
                         self.assign_attrs(elem, m.group(1))
                         elem.text = elem.text[:m.start()]
                         if isheader(elem):
                             # clean up trailing #s
                             elem.text = elem.text.rstrip('#').rstrip()
             else:
-                # inline: check for attrs at start of tail
+                # inline: check for `attrs` at start of tail
                 if elem.tail:
                     m = self.INLINE_RE.match(elem.tail)
                     if m:
                         self.assign_attrs(elem, m.group(1))
                         elem.tail = elem.tail[m.end():]
 
     def assign_attrs(self, elem, attrs):
-        """ Assign attrs to element. """
+        """ Assign `attrs` to element. """
         for k, v in get_attrs(attrs):
             if k == '.':
                 # add to class
                 cls = elem.get('class')
                 if cls:
                     elem.set('class', '{} {}'.format(cls, v))
                 else:
                     elem.set('class', v)
             else:
-                # assign attr k with v
+                # assign attribute `k` with `v`
                 elem.set(self.sanitize_name(k), v)
 
     def sanitize_name(self, name):
         """
         Sanitize name as 'an XML Name, minus the ":"'.
         See https://www.w3.org/TR/REC-xml-names/#NT-NCName
         """
```

### Comparing `Markdown-3.4.3/markdown/extensions/codehilite.py` & `Markdown-3.4.4/markdown/extensions/codehilite.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,46 +50,46 @@
     Determine language of source code, and pass it on to the Pygments highlighter.
 
     Usage:
         code = CodeHilite(src=some_code, lang='python')
         html = code.hilite()
 
     Arguments:
-    * src: Source string or any object with a .readline attribute.
+    * `src`: Source string or any object with a `.readline` attribute.
 
-    * lang: String name of Pygments lexer to use for highlighting. Default: `None`.
+    * `lang`: String name of Pygments lexer to use for highlighting. Default: `None`.
 
-    * guess_lang: Auto-detect which lexer to use. Ignored if `lang` is set to a valid
+    * `guess_lang`: Auto-detect which lexer to use. Ignored if `lang` is set to a valid
       value. Default: `True`.
 
-    * use_pygments: Pass code to pygments for code highlighting. If `False`, the code is
+    * `use_pygments`: Pass code to Pygments for code highlighting. If `False`, the code is
       instead wrapped for highlighting by a JavaScript library. Default: `True`.
 
-    * pygments_formatter: The name of a Pygments formatter or a formatter class used for
+    * `pygments_formatter`: The name of a Pygments formatter or a formatter class used for
       highlighting the code blocks. Default: `html`.
 
-    * linenums: An alias to Pygments `linenos` formatter option. Default: `None`.
+    * `linenums`: An alias to Pygments `linenos` formatter option. Default: `None`.
 
-    * css_class: An alias to Pygments `cssclass` formatter option. Default: 'codehilite'.
+    * `css_class`: An alias to Pygments `cssclass` formatter option. Default: 'codehilite'.
 
-    * lang_prefix: Prefix prepended to the language. Default: "language-".
+    * `lang_prefix`: Prefix prepended to the language. Default: "language-".
 
     Other Options:
     Any other options are accepted and passed on to the lexer and formatter. Therefore,
     valid options include any options which are accepted by the `html` formatter or
     whichever lexer the code's language uses. Note that most lexers do not have any
     options. However, a few have very useful options, such as PHP's `startinline` option.
     Any invalid options are ignored without error.
 
     Formatter options: https://pygments.org/docs/formatters/#HtmlFormatter
     Lexer Options: https://pygments.org/docs/lexers/
 
     Additionally, when Pygments is enabled, the code's language is passed to the
     formatter as an extra option `lang_str`, whose value being `{lang_prefix}{lang}`.
-    This option has no effect to the Pygments's builtin formatters.
+    This option has no effect to the Pygments' builtin formatters.
 
     Advanced Usage:
         code = CodeHilite(
             src = some_code,
             lang = 'php',
             startinline = True,      # Lexer option. Snippet does not start with `<?php`.
             linenostart = 42,        # Formatter option. Snippet starts on line 42.
@@ -109,27 +109,27 @@
         self.pygments_formatter = options.pop('pygments_formatter', 'html')
 
         if 'linenos' not in options:
             options['linenos'] = options.pop('linenums', None)
         if 'cssclass' not in options:
             options['cssclass'] = options.pop('css_class', 'codehilite')
         if 'wrapcode' not in options:
-            # Override pygments default
+            # Override Pygments default
             options['wrapcode'] = True
         # Disallow use of `full` option
         options['full'] = False
 
         self.options = options
 
     def hilite(self, shebang=True):
         """
-        Pass code to the [Pygments](https://pygments.org/) highliter with
-        optional line numbers. The output should then be styled with css to
+        Pass code to the [Pygments](https://pygments.org/) highlighter with
+        optional line numbers. The output should then be styled with CSS to
         your liking. No styles are applied by default - only styling hooks
-        (i.e.: <span class="k">).
+        (i.e.: `<span class="k">`).
 
         returns : A string of html.
 
         """
 
         self.src = self.src.strip('\n')
 
@@ -156,15 +156,15 @@
                     formatter = get_formatter_by_name(self.pygments_formatter, **self.options)
                 except ClassNotFound:
                     formatter = get_formatter_by_name('html', **self.options)
             else:
                 formatter = self.pygments_formatter(lang_str=lang_str, **self.options)
             return highlight(self.src, lexer, formatter)
         else:
-            # just escape and build markup usable by JS highlighting libs
+            # just escape and build markup usable by JavaScript highlighting libraries
             txt = self.src.replace('&', '&amp;')
             txt = txt.replace('<', '&lt;')
             txt = txt.replace('>', '&gt;')
             txt = txt.replace('"', '&quot;')
             classes = []
             if self.lang:
                 classes.append('{}{}'.format(self.lang_prefix, self.lang))
@@ -181,19 +181,19 @@
 
     def _parseHeader(self):
         """
         Determines language of a code block from shebang line and whether the
         said line should be removed or left in place. If the shebang line
         contains a path (even a single /) then it is assumed to be a real
         shebang line and left alone. However, if no path is given
-        (e.i.: #!python or :::python) then it is assumed to be a mock shebang
+        (e.i.: `#!python` or `:::python`) then it is assumed to be a mock shebang
         for language identification of a code fragment and removed from the
         code block prior to processing for code highlighting. When a mock
-        shebang (e.i: #!python) is found, line numbering is turned on. When
-        colons are found in place of a shebang (e.i.: :::python), line
+        shebang (e.i: `#!python`) is found, line numbering is turned on. When
+        colons are found in place of a shebang (e.i.: `:::python`), line
         numbering is left in the current state - off by default.
 
         Also parses optional list of highlight lines, like:
 
             :::python hl_lines="1 3"
         """
 
@@ -247,36 +247,36 @@
         text = text.replace("&gt;", ">")
         # Escaped '&' should be replaced at the end to avoid
         # conflicting with < and >.
         text = text.replace("&amp;", "&")
         return text
 
     def run(self, root):
-        """ Find code blocks and store in htmlStash. """
+        """ Find code blocks and store in `htmlStash`. """
         blocks = root.iter('pre')
         for block in blocks:
             if len(block) == 1 and block[0].tag == 'code':
                 local_config = self.config.copy()
                 code = CodeHilite(
                     self.code_unescape(block[0].text),
                     tab_length=self.md.tab_length,
                     style=local_config.pop('pygments_style', 'default'),
                     **local_config
                 )
                 placeholder = self.md.htmlStash.store(code.hilite())
-                # Clear codeblock in etree instance
+                # Clear code block in `etree` instance
                 block.clear()
-                # Change to p element which will later
+                # Change to `p` element which will later
                 # be removed when inserting raw html
                 block.tag = 'p'
                 block.text = placeholder
 
 
 class CodeHiliteExtension(Extension):
-    """ Add source code highlighting to markdown codeblocks. """
+    """ Add source code highlighting to markdown code blocks. """
 
     def __init__(self, **kwargs):
         # define default configs
         self.config = {
             'linenums': [None,
                          "Use lines numbers. True|table|inline=yes, False=no, None=auto"],
             'guess_lang': [True,
@@ -307,22 +307,22 @@
         for key, value in kwargs.items():
             if key in self.config:
                 self.setConfig(key, value)
             else:
                 # manually set unknown keywords.
                 if isinstance(value, str):
                     try:
-                        # Attempt to parse str as a bool value
+                        # Attempt to parse `str` as a boolean value
                         value = parseBoolValue(value, preserve_none=True)
                     except ValueError:
-                        pass  # Assume it's not a bool value. Use as-is.
+                        pass  # Assume it's not a boolean value. Use as-is.
                 self.config[key] = [value, '']
 
     def extendMarkdown(self, md):
-        """ Add HilitePostprocessor to Markdown instance. """
+        """ Add `HilitePostprocessor` to Markdown instance. """
         hiliter = HiliteTreeprocessor(md)
         hiliter.config = self.getConfigs()
         md.treeprocessors.register(hiliter, 'hilite', 30)
 
         md.registerExtension(self)
```

### Comparing `Markdown-3.4.3/markdown/extensions/def_list.py` & `Markdown-3.4.4/markdown/extensions/def_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,24 +88,24 @@
     """ Process indented children of definition list items. """
 
     # Definition lists need to be aware of all list types
     ITEM_TYPES = ['dd', 'li']
     LIST_TYPES = ['dl', 'ol', 'ul']
 
     def create_item(self, parent, block):
-        """ Create a new dd or li (depending on parent) and parse the block with it as the parent. """
+        """ Create a new `dd` or `li` (depending on parent) and parse the block with it as the parent. """
 
         dd = etree.SubElement(parent, 'dd')
         self.parser.parseBlocks(dd, [block])
 
 
 class DefListExtension(Extension):
     """ Add definition lists to Markdown. """
 
     def extendMarkdown(self, md):
-        """ Add an instance of DefListProcessor to BlockParser. """
+        """ Add an instance of `DefListProcessor` to `BlockParser`. """
         md.parser.blockprocessors.register(DefListIndentProcessor(md.parser), 'defindent', 85)
         md.parser.blockprocessors.register(DefListProcessor(md.parser), 'deflist', 25)
 
 
 def makeExtension(**kwargs):  # pragma: no cover
     return DefListExtension(**kwargs)
```

### Comparing `Markdown-3.4.3/markdown/extensions/extra.py` & `Markdown-3.4.4/markdown/extensions/extra.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 ]
 
 
 class ExtraExtension(Extension):
     """ Add various extensions to Markdown class."""
 
     def __init__(self, **kwargs):
-        """ config is a dumb holder which gets passed to actual ext later. """
+        """ `config` is a dumb holder which gets passed to the actual extension later. """
         self.config = kwargs
 
     def extendMarkdown(self, md):
         """ Register extension instances. """
         md.registerExtensions(extensions, self.config)
```

### Comparing `Markdown-3.4.3/markdown/extensions/fenced_code.py` & `Markdown-3.4.4/markdown/extensions/fenced_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     def __init__(self, **kwargs):
         self.config = {
             'lang_prefix': ['language-', 'Prefix prepended to the language. Default: "language-"']
         }
         super().__init__(**kwargs)
 
     def extendMarkdown(self, md):
-        """ Add FencedBlockPreprocessor to the Markdown instance. """
+        """ Add `FencedBlockPreprocessor` to the Markdown instance. """
         md.registerExtension(self)
 
         md.preprocessors.register(FencedBlockPreprocessor(md, self.getConfigs()), 'fenced_code_block', 25)
 
 
 class FencedBlockPreprocessor(Preprocessor):
     FENCED_BLOCK_RE = re.compile(
@@ -56,24 +56,24 @@
 
     def __init__(self, md, config):
         super().__init__(md)
         self.config = config
         self.checked_for_deps = False
         self.codehilite_conf = {}
         self.use_attr_list = False
-        # List of options to convert to bool values
+        # List of options to convert to boolean values
         self.bool_options = [
             'linenums',
             'guess_lang',
             'noclasses',
             'use_pygments'
         ]
 
     def run(self, lines):
-        """ Match and store Fenced Code Blocks in the HtmlStash. """
+        """ Match and store Fenced Code Blocks in the `HtmlStash`. """
 
         # Check for dependent extensions
         if not self.checked_for_deps:
             for ext in self.md.registeredExtensions:
                 if isinstance(ext, CodeHiliteExtension):
                     self.codehilite_conf = ext.getConfigs()
                 if isinstance(ext, AttrListExtension):
@@ -90,24 +90,24 @@
                     id, classes, config = self.handle_attrs(get_attrs(m.group('attrs')))
                     if len(classes):
                         lang = classes.pop(0)
                 else:
                     if m.group('lang'):
                         lang = m.group('lang')
                     if m.group('hl_lines'):
-                        # Support hl_lines outside of attrs for backward-compatibility
+                        # Support `hl_lines` outside of `attrs` for backward-compatibility
                         config['hl_lines'] = parse_hl_lines(m.group('hl_lines'))
 
-                # If config is not empty, then the codehighlite extension
+                # If `config` is not empty, then the `codehighlite` extension
                 # is enabled, so we call it to highlight the code
                 if self.codehilite_conf and self.codehilite_conf['use_pygments'] and config.get('use_pygments', True):
                     local_config = self.codehilite_conf.copy()
                     local_config.update(config)
-                    # Combine classes with cssclass. Ensure cssclass is at end
-                    # as pygments appends a suffix under certain circumstances.
+                    # Combine classes with `cssclass`. Ensure `cssclass` is at end
+                    # as Pygments appends a suffix under certain circumstances.
                     # Ignore ID as Pygments does not offer an option to set it.
                     if classes:
                         local_config['css_class'] = '{} {}'.format(
                             ' '.join(classes),
                             local_config['css_class']
                         )
                     highliter = CodeHilite(
@@ -124,17 +124,17 @@
                         prefix = self.config.get('lang_prefix', 'language-')
                         lang_attr = f' class="{prefix}{_escape_attrib_html(lang)}"'
                     if classes:
                         class_attr = f' class="{_escape_attrib_html(" ".join(classes))}"'
                     if id:
                         id_attr = f' id="{_escape_attrib_html(id)}"'
                     if self.use_attr_list and config and not config.get('use_pygments', False):
-                        # Only assign key/value pairs to code element if attr_list ext is enabled, key/value pairs
-                        # were defined on the code block, and the `use_pygments` key was not set to True. The
-                        # `use_pygments` key could be either set to False or not defined. It is omitted from output.
+                        # Only assign key/value pairs to code element if `attr_list` extension is enabled, key/value
+                        # pairs were defined on the code block, and the `use_pygments` key was not set to `True`. The
+                        # `use_pygments` key could be either set to `False` or not defined. It is omitted from output.
                         kv_pairs = ''.join(
                             f' {k}="{_escape_attrib_html(v)}"' for k, v in config.items() if k != 'use_pygments'
                         )
                     code = self._escape(m.group('code'))
                     code = f'<pre{id_attr}{class_attr}><code{lang_attr}{kv_pairs}>{code}</code></pre>'
 
                 placeholder = self.md.htmlStash.store(code)
```

### Comparing `Markdown-3.4.3/markdown/extensions/footnotes.py` & `Markdown-3.4.4/markdown/extensions/footnotes.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,28 +70,28 @@
         self.reset()
 
     def extendMarkdown(self, md):
         """ Add pieces to Markdown. """
         md.registerExtension(self)
         self.parser = md.parser
         self.md = md
-        # Insert a blockprocessor before ReferencePreprocessor
+        # Insert a `blockprocessor` before `ReferencePreprocessor`
         md.parser.blockprocessors.register(FootnoteBlockProcessor(self), 'footnote', 17)
 
-        # Insert an inline pattern before ImageReferencePattern
+        # Insert an inline pattern before `ImageReferencePattern`
         FOOTNOTE_RE = r'\[\^([^\]]*)\]'  # blah blah [^1] blah
         md.inlinePatterns.register(FootnoteInlineProcessor(FOOTNOTE_RE, self), 'footnote', 175)
         # Insert a tree-processor that would actually add the footnote div
-        # This must be before all other treeprocessors (i.e., inline and
-        # codehilite) so they can run on the the contents of the div.
+        # This must be before all other tree-processors (i.e., `inline` and
+        # `codehilite`) so they can run on the the contents of the div.
         md.treeprocessors.register(FootnoteTreeprocessor(self), 'footnote', 50)
 
         # Insert a tree-processor that will run after inline is done.
         # In this tree-processor we want to check our duplicate footnote tracker
-        # And add additional backrefs to the footnote pointing back to the
+        # And add additional `backrefs` to the footnote pointing back to the
         # duplicated references.
         md.treeprocessors.register(FootnotePostTreeprocessor(self), 'footnote-duplicate', 15)
 
         # Insert a postprocessor after amp_substitute processor
         md.postprocessors.register(FootnotePostprocessor(self), 'footnote', 25)
 
     def reset(self):
@@ -159,15 +159,15 @@
         """ Return footnote back-link id. """
         if self.getConfig("UNIQUE_IDS"):
             return self.unique_ref('fnref%s%d-%s' % (self.get_separator(), self.unique_prefix, id), found)
         else:
             return self.unique_ref('fnref{}{}'.format(self.get_separator(), id), found)
 
     def makeFootnotesDiv(self, root):
-        """ Return div of footnotes as et Element. """
+        """ Return `div` of footnotes as `etree` Element. """
 
         if not list(self.footnotes.keys()):
             return None
 
         div = etree.Element("div")
         div.set('class', 'footnote')
         etree.SubElement(div, "hr")
@@ -176,17 +176,17 @@
 
         # Backward compatibility with old '%d' placeholder
         backlink_title = self.getConfig("BACKLINK_TITLE").replace("%d", "{}")
 
         for index, id in enumerate(self.footnotes.keys(), start=1):
             li = etree.SubElement(ol, "li")
             li.set("id", self.makeFootnoteId(id))
-            # Parse footnote with surrogate parent as li cannot be used.
-            # List block handlers have special logic to deal with li.
-            # When we are done parsing, we will copy everything over to li.
+            # Parse footnote with surrogate parent as `li` cannot be used.
+            # List block handlers have special logic to deal with `li`.
+            # When we are done parsing, we will copy everything over to `li`.
             self.parser.parseChunk(surrogate_parent, self.footnotes[id])
             for el in list(surrogate_parent):
                 li.append(el)
                 surrogate_parent.remove(el)
             backlink = etree.Element("a")
             backlink.set("href", "#" + self.makeFootnoteRefId(id))
             backlink.set("class", "footnote-backref")
@@ -292,15 +292,15 @@
         for i, line in enumerate(lines):
             if line.startswith(' '*4):
                 lines[i] = line[4:]
         return '\n'.join(lines)
 
 
 class FootnoteInlineProcessor(InlineProcessor):
-    """ InlinePattern for footnote markers in a document's body text. """
+    """ `InlinePattern` for footnote markers in a document's body text. """
 
     def __init__(self, pattern, footnotes):
         super().__init__(pattern)
         self.footnotes = footnotes
 
     def handleMatch(self, m, data):
         id = m.group(1)
@@ -321,15 +321,15 @@
 class FootnotePostTreeprocessor(Treeprocessor):
     """ Amend footnote div with duplicates. """
 
     def __init__(self, footnotes):
         self.footnotes = footnotes
 
     def add_duplicates(self, li, duplicates):
-        """ Adjust current li and add the duplicates: fnref2, fnref3, etc. """
+        """ Adjust current `li` and add the duplicates: `fnref2`, `fnref3`, etc. """
         for link in li.iter('a'):
             # Find the link that needs to be duplicated.
             if link.attrib.get('class', '') == 'footnote-backref':
                 ref, rest = link.attrib['href'].split(self.footnotes.get_separator(), 1)
                 # Duplicate link the number of times we need to
                 # and point the to the appropriate references.
                 links = []
@@ -403,9 +403,9 @@
         text = text.replace(
             FN_BACKLINK_TEXT, self.footnotes.getConfig("BACKLINK_TEXT")
         )
         return text.replace(NBSP_PLACEHOLDER, "&#160;")
 
 
 def makeExtension(**kwargs):  # pragma: no cover
-    """ Return an instance of the FootnoteExtension """
+    """ Return an instance of the `FootnoteExtension` """
     return FootnoteExtension(**kwargs)
```

### Comparing `Markdown-3.4.3/markdown/extensions/legacy_attrs.py` & `Markdown-3.4.4/markdown/extensions/legacy_attrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 ===========================
 
 An extension to Python Markdown which implements legacy attributes.
 
 Prior to Python-Markdown version 3.0, the Markdown class had an `enable_attributes`
 keyword which was on by default and provided for attributes to be defined for elements
 using the format `{@key=value}`. This extension is provided as a replacement for
-backward compatibility. New documents should be authored using attr_lists. However,
-numerious documents exist which have been using the old attribute format for many
+backward compatibility. New documents should be authored using `attr_lists`. However,
+numerous documents exist which have been using the old attribute format for many
 years. This extension can be used to continue to render those documents correctly.
 """
 
 import re
 from markdown.treeprocessors import Treeprocessor, isString
 from markdown.extensions import Extension
```

### Comparing `Markdown-3.4.3/markdown/extensions/legacy_em.py` & `Markdown-3.4.4/markdown/extensions/legacy_em.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,9 +41,9 @@
 
     def extendMarkdown(self, md):
         """ Modify inline patterns. """
         md.inlinePatterns.register(LegacyUnderscoreProcessor(r'_'), 'em_strong2', 50)
 
 
 def makeExtension(**kwargs):  # pragma: no cover
-    """ Return an instance of the LegacyEmExtension """
+    """ Return an instance of the `LegacyEmExtension` """
     return LegacyEmExtension(**kwargs)
```

### Comparing `Markdown-3.4.3/markdown/extensions/md_in_html.py` & `Markdown-3.4.4/markdown/extensions/md_in_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 from .. import util
 from ..htmlparser import HTMLExtractor, blank_line_re
 import xml.etree.ElementTree as etree
 
 
 class HTMLExtractorExtra(HTMLExtractor):
     """
-    Override HTMLExtractor and create etree Elements for any elements which should have content parsed as Markdown.
+    Override `HTMLExtractor` and create `etree` `Elements` for any elements which should have content parsed as
+    Markdown.
     """
 
     def __init__(self, md, *args, **kwargs):
         # All block-level tags.
         self.block_level_tags = set(md.block_level_elements.copy())
         # Block-level tags in which the content only gets span level parsing
         self.span_tags = set(
@@ -52,25 +53,25 @@
         super().reset()
 
     def close(self):
         """Handle any buffered data."""
         super().close()
         # Handle any unclosed tags.
         if self.mdstack:
-            # Close the outermost parent. handle_endtag will close all unclosed children.
+            # Close the outermost parent. `handle_endtag` will close all unclosed children.
             self.handle_endtag(self.mdstack[0])
 
     def get_element(self):
-        """ Return element from treebuilder and reset treebuilder for later use. """
+        """ Return element from `treebuilder` and reset `treebuilder` for later use. """
         element = self.treebuilder.close()
         self.treebuilder = etree.TreeBuilder()
         return element
 
     def get_state(self, tag, attrs):
-        """ Return state from tag and `markdown` attr. One of 'block', 'span', or 'off'. """
+        """ Return state from tag and `markdown` attribute. One of 'block', 'span', or 'off'. """
         md_attr = attrs.get('markdown', '0')
         if md_attr == 'markdown':
             # `<tag markdown>` is the same as `<tag markdown='1'>`.
             md_attr = '1'
         parent_state = self.mdstate[-1] if self.mdstate else None
         if parent_state == 'off' or (parent_state == 'span' and md_attr != '0'):
             # Only use the parent state if it is more restrictive than the markdown attribute.
@@ -96,15 +97,15 @@
                 data = etree.tostring(element, encoding='unicode', method='html')
             else:
                 data = self.get_starttag_text()
             self.handle_empty_tag(data, True)
             return
 
         if tag in self.block_level_tags and (self.at_line_start() or self.intail):
-            # Valueless attr (ex: `<tag checked>`) results in `[('checked', None)]`.
+            # Valueless attribute (ex: `<tag checked>`) results in `[('checked', None)]`.
             # Convert to `{'checked': 'checked'}`.
             attrs = {key: value if value is not None else key for key, value in attrs}
             state = self.get_state(tag, attrs)
             if self.inraw or (state in [None, 'off'] and not self.mdstack):
                 # fall back to default behavior
                 attrs.pop('markdown', None)
                 super().handle_starttag(tag, attrs)
@@ -153,15 +154,15 @@
                         self.cleandoc.append('\n')
                     self.cleandoc.append(self.md.htmlStash.store(element))
                     self.cleandoc.append('\n\n')
                     self.state = []
                     # Check if element has a tail
                     if not blank_line_re.match(
                             self.rawdata[self.line_offset + self.offset + len(self.get_endtag_text(tag)):]):
-                        # More content exists after endtag.
+                        # More content exists after `endtag`.
                         self.intail = True
             else:
                 # Treat orphan closing tag as a span level tag.
                 text = self.get_endtag_text(tag)
                 if self.mdstate and self.mdstate[-1] == "off":
                     self.handle_data(self.md.htmlStash.store(text))
                 else:
@@ -205,26 +206,26 @@
             if self.at_line_start() and is_block:
                 self.handle_data('\n' + self.md.htmlStash.store(data) + '\n\n')
             else:
                 self.handle_data(self.md.htmlStash.store(data))
 
     def parse_pi(self, i):
         if self.at_line_start() or self.intail or self.mdstack:
-            # The same override exists in HTMLExtractor without the check
-            # for mdstack. Therefore, use HTMLExtractor's parent instead.
+            # The same override exists in `HTMLExtractor` without the check
+            # for `mdstack`. Therefore, use parent of `HTMLExtractor` instead.
             return super(HTMLExtractor, self).parse_pi(i)
         # This is not the beginning of a raw block so treat as plain data
         # and avoid consuming any tags which may follow (see #1066).
         self.handle_data('<?')
         return i + 2
 
     def parse_html_declaration(self, i):
         if self.at_line_start() or self.intail or self.mdstack:
-            # The same override exists in HTMLExtractor without the check
-            # for mdstack. Therefore, use HTMLExtractor's parent instead.
+            # The same override exists in `HTMLExtractor` without the check
+            # for `mdstack`. Therefore, use parent of `HTMLExtractor` instead.
             return super(HTMLExtractor, self).parse_html_declaration(i)
         # This is not the beginning of a raw block so treat as plain data
         # and avoid consuming any tags which may follow (see #1066).
         self.handle_data('<!')
         return i + 2
 
 
@@ -236,27 +237,27 @@
         parser = HTMLExtractorExtra(self.md)
         parser.feed(source)
         parser.close()
         return ''.join(parser.cleandoc).split('\n')
 
 
 class MarkdownInHtmlProcessor(BlockProcessor):
-    """Process Markdown Inside HTML Blocks which have been stored in the HtmlStash."""
+    """Process Markdown Inside HTML Blocks which have been stored in the `HtmlStash`."""
 
     def test(self, parent, block):
-        # ALways return True. `run` will return `False` it not a valid match.
+        # Always return True. `run` will return `False` it not a valid match.
         return True
 
     def parse_element_content(self, element):
         """
-        Recursively parse the text content of an etree Element as Markdown.
+        Recursively parse the text content of an `etree` Element as Markdown.
 
         Any block level elements generated from the Markdown will be inserted as children of the element in place
         of the text content. All `markdown` attributes are removed. For any elements in which Markdown parsing has
-        been disabled, the text content of it and its chidlren are wrapped in an `AtomicString`.
+        been disabled, the text content of it and its children are wrapped in an `AtomicString`.
         """
 
         md_attr = element.attrib.pop('markdown', 'off')
 
         if md_attr == 'block':
             # Parse content as block level
             # The order in which the different parts are parsed (text, children, tails) is important here as the
@@ -297,15 +298,15 @@
                 self.parser.parseBlocks(dummy, block.split('\n\n'))
                 children = list(dummy)
                 children.reverse()
                 for child in children:
                     element.insert(0, child)
 
         elif md_attr == 'span':
-            # Span level parsing will be handled by inlineprocessors.
+            # Span level parsing will be handled by inline processors.
             # Walk children here to remove any `markdown` attributes.
             for child in list(element):
                 self.parse_element_content(child)
 
         else:
             # Disable inline parsing for everything else
             if element.text is None:
@@ -325,38 +326,38 @@
                 # We have a matched element. Process it.
                 blocks.pop(0)
                 self.parse_element_content(element)
                 parent.append(element)
                 # Cleanup stash. Replace element with empty string to avoid confusing postprocessor.
                 self.parser.md.htmlStash.rawHtmlBlocks.pop(index)
                 self.parser.md.htmlStash.rawHtmlBlocks.insert(index, '')
-                # Confirm the match to the blockparser.
+                # Confirm the match to the `blockparser`.
                 return True
         # No match found.
         return False
 
 
 class MarkdownInHTMLPostprocessor(RawHtmlPostprocessor):
     def stash_to_string(self, text):
-        """ Override default to handle any etree elements still in the stash. """
+        """ Override default to handle any `etree` elements still in the stash. """
         if isinstance(text, etree.Element):
             return self.md.serializer(text)
         else:
             return str(text)
 
 
 class MarkdownInHtmlExtension(Extension):
     """Add Markdown parsing in HTML to Markdown class."""
 
     def extendMarkdown(self, md):
         """ Register extension instances. """
 
         # Replace raw HTML preprocessor
         md.preprocessors.register(HtmlBlockPreprocessor(md), 'html_block', 20)
-        # Add blockprocessor which handles the placeholders for etree elements
+        # Add `blockprocessor` which handles the placeholders for `etree` elements
         md.parser.blockprocessors.register(
             MarkdownInHtmlProcessor(md.parser), 'markdown_block', 105
         )
         # Replace raw HTML postprocessor
         md.postprocessors.register(MarkdownInHTMLPostprocessor(md), 'raw_html', 30)
```

### Comparing `Markdown-3.4.3/markdown/extensions/meta.py` & `Markdown-3.4.4/markdown/extensions/meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 END_RE = re.compile(r'^(-{3}|\.{3})(\s.*)?')
 
 
 class MetaExtension (Extension):
     """ Meta-Data extension for Python-Markdown. """
 
     def extendMarkdown(self, md):
-        """ Add MetaPreprocessor to Markdown instance. """
+        """ Add `MetaPreprocessor` to Markdown instance. """
         md.registerExtension(self)
         self.md = md
         md.preprocessors.register(MetaPreprocessor(md), 'meta', 27)
 
     def reset(self):
         self.md.Meta = {}
```

### Comparing `Markdown-3.4.3/markdown/extensions/nl2br.py` & `Markdown-3.4.4/markdown/extensions/nl2br.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
-NL2BR Extension
+`NL2BR` Extension
 ===============
 
 A Python-Markdown extension to treat newlines as hard breaks; like
 GitHub-flavored Markdown does.
 
 See <https://Python-Markdown.github.io/extensions/nl2br>
 for documentation.
 
-Oringinal code Copyright 2011 [Brian Neal](https://deathofagremmie.com/)
+Original code Copyright 2011 [Brian Neal](https://deathofagremmie.com/)
 
 All changes Copyright 2011-2014 The Python Markdown Project
 
 License: [BSD](https://opensource.org/licenses/bsd-license.php)
 
 """
```

### Comparing `Markdown-3.4.3/markdown/extensions/sane_lists.py` & `Markdown-3.4.4/markdown/extensions/sane_lists.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/markdown/extensions/smarty.py` & `Markdown-3.4.4/markdown/extensions/smarty.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
    limited to, procurement of substitute goods or services; loss of use,
    data, or profits; or business interruption) however caused and on any
    theory of liability, whether in contract, strict liability, or tort
    (including negligence or otherwise) arising in any way out of the use
    of this software, even if advised of the possibility of such damage.
 
 
-smartypants.py license:
+`smartypants.py` license:
 
-   smartypants.py is a derivative work of SmartyPants.
+   `smartypants.py` is a derivative work of SmartyPants.
    Copyright (c) 2004, 2007 Chad Miller <http://web.chad.org/>
 
    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions are
    met:
 
    *  Redistributions of source code must retain the above copyright
@@ -91,15 +91,15 @@
 endOfWordClass = r"[\s.,;:!?)]"
 closeClass = r"[^\ \t\r\n\[\{\(\-\u0002\u0003]"
 
 openingQuotesBase = (
     r'(\s'               # a  whitespace char
     r'|&nbsp;'           # or a non-breaking space entity
     r'|--'               # or dashes
-    r'|–|—'              # or unicode
+    r'|–|—'              # or Unicode
     r'|&[mn]dash;'       # or named dash entities
     r'|&#8211;|&#8212;'  # or decimal entities
     r')'
 )
 
 substitutions = {
     'mdash': '&mdash;',
@@ -135,15 +135,15 @@
 closingDoubleQuotesRegex2 = '(?<=%s)"' % closeClass
 
 # Get most opening single quotes:
 openingSingleQuotesRegex = r"%s'(?=\w)" % openingQuotesBase
 
 # Single closing quotes:
 closingSingleQuotesRegex = r"(?<=%s)'(?!\s|s\b|\d)" % closeClass
-closingSingleQuotesRegex2 = r"(?<=%s)'(\s|s\b)" % closeClass
+closingSingleQuotesRegex2 = r"'(\s|s\b)"
 
 # All remaining quotes should be opening ones
 remainingSingleQuotesRegex = r"'"
 remainingDoubleQuotesRegex = r'"'
 
 HTML_STRICT_RE = HTML_RE + r'(?!\>)'
 
@@ -238,15 +238,15 @@
         self.inlinePatterns = Registry()
         if configs['smart_ellipses']:
             self.educateEllipses(md)
         if configs['smart_quotes']:
             self.educateQuotes(md)
         if configs['smart_angled_quotes']:
             self.educateAngledQuotes(md)
-            # Override HTML_RE from inlinepatterns.py so that it does not
+            # Override `HTML_RE` from `inlinepatterns.py` so that it does not
             # process tags with duplicate closing quotes.
             md.inlinePatterns.register(HtmlInlineProcessor(HTML_STRICT_RE, md), 'html', 90)
         if configs['smart_dashes']:
             self.educateDashes(md)
         inlineProcessor = InlineProcessor(md)
         inlineProcessor.inlinePatterns = self.inlinePatterns
         md.treeprocessors.register(inlineProcessor, 'smarty', 2)
```

### Comparing `Markdown-3.4.3/markdown/extensions/tables.py` & `Markdown-3.4.4/markdown/extensions/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         self.config = {
             'use_align_attribute': [False, 'True to use align attribute instead of style.'],
         }
 
         super().__init__(**kwargs)
 
     def extendMarkdown(self, md):
-        """ Add an instance of TableProcessor to BlockParser. """
+        """ Add an instance of `TableProcessor` to `BlockParser`. """
         if '|' not in md.ESCAPED_CHARS:
             md.ESCAPED_CHARS.append('|')
         processor = TableProcessor(md.parser, self.getConfigs())
         md.parser.blockprocessors.register(processor, 'table', 75)
 
 
 def makeExtension(**kwargs):  # pragma: no cover
```

### Comparing `Markdown-3.4.3/markdown/extensions/toc.py` & `Markdown-3.4.4/markdown/extensions/toc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 Table of Contents Extension for Python-Markdown
 ===============================================
 
 See <https://Python-Markdown.github.io/extensions/toc>
 for documentation.
 
-Oringinal code Copyright 2008 [Jack Miller](https://codezen.org/)
+Original code Copyright 2008 [Jack Miller](https://codezen.org/)
 
 All changes Copyright 2008-2014 The Python Markdown Project
 
 License: [BSD](https://opensource.org/licenses/bsd-license.php)
 
 """
 
@@ -22,15 +22,15 @@
 import unicodedata
 import xml.etree.ElementTree as etree
 
 
 def slugify(value, separator, unicode=False):
     """ Slugify a string, to make it URL friendly. """
     if not unicode:
-        # Replace Extended Latin characters with ASCII, i.e. žlutý → zluty
+        # Replace Extended Latin characters with ASCII, i.e. `žlutý` => `zluty`
         value = unicodedata.normalize('NFKD', value)
         value = value.encode('ascii', 'ignore').decode('ascii')
     value = re.sub(r'[^\w\s-]', '', value).strip().lower()
     return re.sub(r'[{}\s]+'.format(separator), separator, value)
 
 
 def slugify_unicode(value, separator):
@@ -175,50 +175,50 @@
             self.toc_top = 1
             self.toc_bottom = int(config["toc_depth"])
 
     def iterparent(self, node):
         ''' Iterator wrapper to get allowed parent and child all at once. '''
 
         # We do not allow the marker inside a header as that
-        # would causes an enless loop of placing a new TOC
+        # would causes an endless loop of placing a new TOC
         # inside previously generated TOC.
         for child in node:
             if not self.header_rgx.match(child.tag) and child.tag not in ['pre', 'code']:
                 yield node, child
                 yield from self.iterparent(child)
 
     def replace_marker(self, root, elem):
         ''' Replace marker with elem. '''
         for (p, c) in self.iterparent(root):
             text = ''.join(c.itertext()).strip()
             if not text:
                 continue
 
             # To keep the output from screwing up the
-            # validation by putting a <div> inside of a <p>
-            # we actually replace the <p> in its entirety.
+            # validation by putting a `<div>` inside of a `<p>`
+            # we actually replace the `<p>` in its entirety.
 
-            # The <p> element may contain more than a single text content
-            # (nl2br can introduce a <br>). In this situation, c.text returns
+            # The `<p>` element may contain more than a single text content
+            # (`nl2br` can introduce a `<br>`). In this situation, `c.text` returns
             # the very first content, ignore children contents or tail content.
-            # len(c) == 0 is here to ensure there is only text in the <p>.
+            # `len(c) == 0` is here to ensure there is only text in the `<p>`.
             if c.text and c.text.strip() == self.marker and len(c) == 0:
                 for i in range(len(p)):
                     if p[i] == c:
                         p[i] = elem
                         break
 
     def set_level(self, elem):
         ''' Adjust header level according to base level. '''
         level = int(elem.tag[-1]) + self.base_level
         if level > 6:
             level = 6
         elem.tag = 'h%d' % level
 
-    def add_anchor(self, c, elem_id):  # @ReservedAssignment
+    def add_anchor(self, c, elem_id):
         anchor = etree.Element("a")
         anchor.text = c.text
         anchor.attrib["href"] = "#" + elem_id
         anchor.attrib["class"] = self.anchorlink_class
         c.text = ""
         for elem in c:
             anchor.append(elem)
@@ -285,18 +285,18 @@
                     innertext = unescape(stashedHTML2text(text, self.md))
                     el.attrib["id"] = unique(self.slugify(innertext, self.sep), used_ids)
 
                 if int(el.tag[-1]) >= self.toc_top and int(el.tag[-1]) <= self.toc_bottom:
                     toc_tokens.append({
                         'level': int(el.tag[-1]),
                         'id': el.attrib["id"],
-                        'name': stashedHTML2text(
+                        'name': unescape(stashedHTML2text(
                             code_escape(el.attrib.get('data-toc-label', text)),
                             self.md, strip_entities=False
-                        )
+                        ))
                     })
 
                 # Remove the data-toc-label attribute as it is no longer needed
                 if 'data-toc-label' in el.attrib:
                     del el.attrib['data-toc-label']
 
                 if self.use_anchors:
@@ -364,19 +364,14 @@
         super().__init__(**kwargs)
 
     def extendMarkdown(self, md):
         md.registerExtension(self)
         self.md = md
         self.reset()
         tocext = self.TreeProcessorClass(md, self.getConfigs())
-        # Headerid ext is set to '>prettify'. With this set to '_end',
-        # it should always come after headerid ext (and honor ids assigned
-        # by the header id extension) if both are used. Same goes for
-        # attr_list extension. This must come last because we don't want
-        # to redefine ids after toc is created. But we do want toc prettified.
         md.treeprocessors.register(tocext, 'toc', 5)
 
     def reset(self):
         self.md.toc = ''
         self.md.toc_tokens = []
```

### Comparing `Markdown-3.4.3/markdown/extensions/wikilinks.py` & `Markdown-3.4.4/markdown/extensions/wikilinks.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from . import Extension
 from ..inlinepatterns import InlineProcessor
 import xml.etree.ElementTree as etree
 import re
 
 
 def build_url(label, base, end):
-    """ Build a url from the label, a base, and an end. """
+    """ Build a URL from the label, a base, and an end. """
     clean_label = re.sub(r'([ ]+_)|(_[ ]+)|([ ]+)', '_', label)
     return '{}{}{}'.format(base, clean_label, end)
 
 
 class WikiLinkExtension(Extension):
 
     def __init__(self, **kwargs):
@@ -65,15 +65,15 @@
             if html_class:
                 a.set('class', html_class)
         else:
             a = ''
         return a, m.start(0), m.end(0)
 
     def _getMeta(self):
-        """ Return meta data or config data. """
+        """ Return meta data or `config` data. """
         base_url = self.config['base_url']
         end_url = self.config['end_url']
         html_class = self.config['html_class']
         if hasattr(self.md, 'Meta'):
             if 'wiki_base_url' in self.md.Meta:
                 base_url = self.md.Meta['wiki_base_url'][0]
             if 'wiki_end_url' in self.md.Meta:
```

### Comparing `Markdown-3.4.3/markdown/htmlparser.py` & `Markdown-3.4.4/markdown/htmlparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 # Import a copy of the html.parser lib as `htmlparser` so we can monkeypatch it.
 # Users can still do `from html import parser` and get the default behavior.
 spec = importlib.util.find_spec('html.parser')
 htmlparser = importlib.util.module_from_spec(spec)
 spec.loader.exec_module(htmlparser)
 sys.modules['htmlparser'] = htmlparser
 
-# Monkeypatch HTMLParser to only accept `?>` to close Processing Instructions.
+# Monkeypatch `HTMLParser` to only accept `?>` to close Processing Instructions.
 htmlparser.piclose = re.compile(r'\?>')
-# Monkeypatch HTMLParser to only recognize entity references with a closing semicolon.
+# Monkeypatch `HTMLParser` to only recognize entity references with a closing semicolon.
 htmlparser.entityref = re.compile(r'&([a-zA-Z][-.a-zA-Z0-9]*);')
-# Monkeypatch HTMLParser to no longer support partial entities. We are always feeding a complete block,
-# so the 'incomplete' functionality is unnecessary. As the entityref regex is run right before incomplete,
+# Monkeypatch `HTMLParser` to no longer support partial entities. We are always feeding a complete block,
+# so the 'incomplete' functionality is unnecessary. As the `entityref` regex is run right before incomplete,
 # and the two regex are the same, then incomplete will simply never match and we avoid the logic within.
 htmlparser.incomplete = htmlparser.entityref
-# Monkeypatch HTMLParser to not accept a backtick in a tag name, attribute name, or bare value.
+# Monkeypatch `HTMLParser` to not accept a backtick in a tag name, attribute name, or bare value.
 htmlparser.locatestarttagend_tolerant = re.compile(r"""
   <[a-zA-Z][^`\t\n\r\f />\x00]*       # tag name <= added backtick here
   (?:[\s/]*                           # optional whitespace before attribute name
     (?:(?<=['"\s/])[^`\s/>][^\s/=>]*  # attribute name <= added backtick here
       (?:\s*=+\s*                     # value indicator
         (?:'[^']*'                    # LITA-enclosed value
           |"[^"]*"                    # LIT-enclosed value
@@ -80,15 +80,15 @@
         super().__init__(*args, **kwargs)
         self.md = md
 
     def reset(self):
         """Reset this instance.  Loses all unprocessed data."""
         self.inraw = False
         self.intail = False
-        self.stack = []  # When inraw==True, stack contains a list of tags
+        self.stack = []  # When `inraw==True`, stack contains a list of tags
         self._cache = []
         self.cleandoc = []
         super().reset()
 
     def close(self):
         """Handle any buffered data."""
         super().close()
@@ -102,21 +102,21 @@
         # Handle any unclosed tags.
         if len(self._cache):
             self.cleandoc.append(self.md.htmlStash.store(''.join(self._cache)))
             self._cache = []
 
     @property
     def line_offset(self):
-        """Returns char index in self.rawdata for the start of the current line. """
+        """Returns char index in `self.rawdata` for the start of the current line. """
         if self.lineno > 1 and '\n' in self.rawdata:
             m = re.match(r'([^\n]*\n){{{}}}'.format(self.lineno-1), self.rawdata)
             if m:
                 return m.end()
             else:  # pragma: no cover
-                # Value of self.lineno must exceed total number of lines.
+                # Value of `self.lineno` must exceed total number of lines.
                 # Find index of beginning of last line.
                 return self.rawdata.rfind('\n')
         return 0
 
     def at_line_start(self):
         """
         Returns True if current position is at start of line.
@@ -178,15 +178,15 @@
                         break
             if len(self.stack) == 0:
                 # End of raw block.
                 if blank_line_re.match(self.rawdata[self.line_offset + self.offset + len(text):]):
                     # Preserve blank line and end of raw block.
                     self._cache.append('\n')
                 else:
-                    # More content exists after endtag.
+                    # More content exists after `endtag`.
                     self.intail = True
                 # Reset stack.
                 self.inraw = False
                 self.cleandoc.append(self.md.htmlStash.store(''.join(self._cache)))
                 # Insert blank line between this and next line.
                 self.cleandoc.append('\n\n')
                 self._cache = []
@@ -259,32 +259,32 @@
             return super().parse_html_declaration(i)
         # This is not the beginning of a raw block so treat as plain data
         # and avoid consuming any tags which may follow (see #1066).
         self.handle_data('<!')
         return i + 2
 
     # The rest has been copied from base class in standard lib to address #1036.
-    # As __startag_text is private, all references to it must be in this subclass.
-    # The last few lines of parse_starttag are reversed so that handle_starttag
-    # can override cdata_mode in certain situations (in a code span).
+    # As `__startag_text` is private, all references to it must be in this subclass.
+    # The last few lines of `parse_starttag` are reversed so that `handle_starttag`
+    # can override `cdata_mode` in certain situations (in a code span).
     __starttag_text = None
 
     def get_starttag_text(self):
-        """Return full source of start tag: '<...>'."""
+        """Return full source of start tag: `<...>`."""
         return self.__starttag_text
 
     def parse_starttag(self, i):  # pragma: no cover
         self.__starttag_text = None
         endpos = self.check_for_whole_start_tag(i)
         if endpos < 0:
             return endpos
         rawdata = self.rawdata
         self.__starttag_text = rawdata[i:endpos]
 
-        # Now parse the data between i+1 and j into a tag and attrs
+        # Now parse the data between `i+1` and `j` into a tag and `attrs`
         attrs = []
         match = htmlparser.tagfind_tolerant.match(rawdata, i+1)
         assert match, 'unexpected call to parse_starttag()'
         k = match.end()
         self.lasttag = tag = match.group(1).lower()
         while k < endpos:
             m = htmlparser.attrfind_tolerant.match(rawdata, k)
@@ -309,15 +309,15 @@
                 offset = len(self.__starttag_text) \
                          - self.__starttag_text.rfind("\n")  # noqa: E127
             else:
                 offset = offset + len(self.__starttag_text)
             self.handle_data(rawdata[i:endpos])
             return endpos
         if end.endswith('/>'):
-            # XHTML-style empty tag: <span attr="value" />
+            # XHTML-style empty tag: `<span attr="value" />`
             self.handle_startendtag(tag, attrs)
         else:
-            # *** set cdata_mode first so we can override it in handle_starttag (see #1036) ***
+            # *** set `cdata_mode` first so we can override it in `handle_starttag` (see #1036) ***
             if tag in self.CDATA_CONTENT_ELEMENTS:
                 self.set_cdata_mode(tag)
             self.handle_starttag(tag, attrs)
         return endpos
```

### Comparing `Markdown-3.4.3/markdown/inlinepatterns.py` & `Markdown-3.4.4/markdown/inlinepatterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,19 +32,19 @@
                            # an ElementTree element or just plain text
 
 All of python markdown's built-in patterns subclass from Pattern,
 but you can add additional patterns that don't.
 
 Also note that all the regular expressions used by inline must
 capture the whole block.  For this reason, they all start with
-'^(.*)' and end with '(.*)!'.  In case with built-in expression
-Pattern takes care of adding the "^(.*)" and "(.*)!".
+`^(.*)` and end with `(.*)!`.  In case with built-in expression
+Pattern takes care of adding the `^(.*)` and `(.*)!`.
 
 Finally, the order in which regular expressions are applied is very
-important - e.g. if we first replace http://.../ links with <a> tags
+important - e.g. if we first replace `http://.../` links with `<a>` tags
 and _then_ try to replace inline html, we would end up with a mess.
 So, we apply the expressions in the following order:
 
 * escape and backticks have to go before everything else, so
   that we can preempt any markdown patterns by escaping them.
 
 * then we handle auto-links (must be done before inline html)
@@ -104,72 +104,72 @@
 """
 
 NOIMG = r'(?<!\!)'
 
 # `e=f()` or ``e=f("`")``
 BACKTICK_RE = r'(?:(?<!\\)((?:\\{2})+)(?=`+)|(?<!\\)(`+)(.+?)(?<!`)\2(?!`))'
 
-# \<
+# `\<`
 ESCAPE_RE = r'\\(.)'
 
-# *emphasis*
+# `*emphasis*`
 EMPHASIS_RE = r'(\*)([^\*]+)\1'
 
-# **strong**
+# `**strong**`
 STRONG_RE = r'(\*{2})(.+?)\1'
 
-# __smart__strong__
+# `__smart__strong__`
 SMART_STRONG_RE = r'(?<!\w)(_{2})(?!_)(.+?)(?<!_)\1(?!\w)'
 
-# _smart_emphasis_
+# `_smart_emphasis_`
 SMART_EMPHASIS_RE = r'(?<!\w)(_)(?!_)(.+?)(?<!_)\1(?!\w)'
 
-# __strong _em__
+# `__strong _em__`
 SMART_STRONG_EM_RE = r'(?<!\w)(\_)\1(?!\1)(.+?)(?<!\w)\1(?!\1)(.+?)\1{3}(?!\w)'
 
-# ***strongem*** or ***em*strong**
+# `***strongem***` or `***em*strong**`
 EM_STRONG_RE = r'(\*)\1{2}(.+?)\1(.*?)\1{2}'
 
-# ___strongem___ or ___em_strong__
+# `___strongem___` or `___em_strong__`
 EM_STRONG2_RE = r'(_)\1{2}(.+?)\1(.*?)\1{2}'
 
-# ***strong**em*
+# `***strong**em*`
 STRONG_EM_RE = r'(\*)\1{2}(.+?)\1{2}(.*?)\1'
 
-# ___strong__em_
+# `___strong__em_`
 STRONG_EM2_RE = r'(_)\1{2}(.+?)\1{2}(.*?)\1'
 
-# **strong*em***
+# `**strong*em***`
 STRONG_EM3_RE = r'(\*)\1(?!\1)([^*]+?)\1(?!\1)(.+?)\1{3}'
 
-# [text](url) or [text](<url>) or [text](url "title")
+# `[text](url)` or `[text](<url>)` or `[text](url "title")`
 LINK_RE = NOIMG + r'\['
 
-# ![alttxt](http://x.com/) or ![alttxt](<http://x.com/>)
+# `![alttxt](http://x.com/)` or `![alttxt](<http://x.com/>)`
 IMAGE_LINK_RE = r'\!\['
 
-# [Google][3]
+# `[Google][3]`
 REFERENCE_RE = LINK_RE
 
-# ![alt text][2]
+# `![alt text][2]`
 IMAGE_REFERENCE_RE = IMAGE_LINK_RE
 
-# stand-alone * or _
+# stand-alone `*` or `_`
 NOT_STRONG_RE = r'((^|(?<=\s))(\*{1,3}|_{1,3})(?=\s|$))'
 
-# <http://www.123.com>
+# `<http://www.123.com>`
 AUTOLINK_RE = r'<((?:[Ff]|[Hh][Tt])[Tt][Pp][Ss]?://[^<>]*)>'
 
-# <me@example.com>
+# `<me@example.com>`
 AUTOMAIL_RE = r'<([^<> !]+@[^@<> ]+)>'
 
-# <...>
+# `<...>`
 HTML_RE = r'(<(\/?[a-zA-Z][^<>@ ]*( [^<>]*)?|!--(?:(?!<!--|-->).)*--)>)'
 
-# "&#38;" (decimal) or "&#x26;" (hex) or "&amp;" (named)
+# `&#38;` (decimal) or `&#x26;` (hex) or `&amp;` (named)
 ENTITY_RE = r'(&(?:\#[0-9]+|\#x[0-9a-fA-F]+|[a-zA-Z0-9]+);)'
 
 # two spaces at end of line
 LINE_BREAK_RE = r'  \n'
 
 
 def dequote(string):
@@ -241,15 +241,15 @@
         def get_stash(m):
             id = m.group(1)
             if id in stash:
                 value = stash.get(id)
                 if isinstance(value, str):
                     return value
                 else:
-                    # An etree Element - return text content only
+                    # An `etree` Element - return text content only
                     return ''.join(value.itertext())
         return util.INLINE_PLACEHOLDER_RE.sub(get_stash, text)
 
 
 class InlineProcessor(Pattern):
     """
     Base class that inline patterns subclass.
@@ -266,15 +266,15 @@
 
         * pattern: A regular expression that matches a pattern
 
         """
         self.pattern = pattern
         self.compiled_re = re.compile(pattern, re.DOTALL | re.UNICODE)
 
-        # Api for Markdown to pass safe_mode into instance
+        # API for Markdown to pass `safe_mode` into instance
         self.safe_mode = False
         self.md = md
 
     def handleMatch(self, m, data):
         """Return a ElementTree element from the given match and the
         start and end index of the matched text.
 
@@ -412,15 +412,15 @@
             el2.tail = m.group(3)
         return el1, m.start(0), m.end(0)
 
 
 class HtmlInlineProcessor(InlineProcessor):
     """ Store raw inline html and return a placeholder. """
     def handleMatch(self, m, data):
-        rawhtml = self.unescape(m.group(1))
+        rawhtml = self.backslash_unescape(self.unescape(m.group(1)))
         place_holder = self.md.htmlStash.store(rawhtml)
         return place_holder, m.start(0), m.end(0)
 
     def unescape(self, text):
         """ Return unescaped text given text with an inline placeholder. """
         try:
             stash = self.md.treeprocessors['inline'].stashed_nodes
@@ -434,14 +434,26 @@
                 try:
                     return self.md.serializer(value)
                 except Exception:
                     return r'\%s' % value
 
         return util.INLINE_PLACEHOLDER_RE.sub(get_stash, text)
 
+    def backslash_unescape(self, text):
+        """ Return text with backslash escapes undone (backslashes are restored). """
+        try:
+            RE = self.md.treeprocessors['unescape'].RE
+        except KeyError:  # pragma: no cover
+            return text
+
+        def _unescape(m):
+            return chr(int(m.group(1)))
+
+        return RE.sub(_unescape, text)
+
 
 class AsteriskProcessor(InlineProcessor):
     """Emphasis processor for handling strong and em matches inside asterisks."""
 
     PATTERNS = [
         EmStrongItem(re.compile(EM_STRONG_RE, re.DOTALL | re.UNICODE), 'double', 'strong,em'),
         EmStrongItem(re.compile(STRONG_EM_RE, re.DOTALL | re.UNICODE), 'double', 'em,strong'),
@@ -706,15 +718,15 @@
                     else:
                         href = data[start_index:index - 1]
                     break
 
                 if c != ' ':
                     last = c
 
-            # We have a scenario: [test](link"notitle)
+            # We have a scenario: `[test](link"notitle)`
             # When we enter a string, we stop tracking bracket resolution in the main counter,
             # but we do keep a backup counter up until we discover where we might resolve all brackets
             # if the title string fails to resolve.
             if bracket_count != 0 and backtrack_count == 0:
                 href = data[start_index:last_bracket - 1]
                 index = last_bracket
                 bracket_count = 0
@@ -745,15 +757,15 @@
             if bracket_count == 0:
                 break
             text.append(c)
         return ''.join(text), index, bracket_count == 0
 
 
 class ImageInlineProcessor(LinkInlineProcessor):
-    """ Return a img element from the given match. """
+    """ Return a `img` element from the given match. """
 
     def handleMatch(self, m, data):
         text, index, handled = self.getText(data, m.end(0))
         if not handled:
             return None, None, None
 
         src, title, index, handled = self.getLink(data, index)
@@ -782,15 +794,15 @@
         if not handled:
             return None, None, None
 
         id, end, handled = self.evalId(data, index, text)
         if not handled:
             return None, None, None
 
-        # Clean up linebreaks in id
+        # Clean up line breaks in id
         id = self.NEWLINE_CLEANUP_RE.sub(' ', id)
         if id not in self.md.references:  # ignore undefined refs
             return None, m.start(0), end
 
         href, title = self.md.references[id]
 
         return self.makeTag(href, title, text), m.start(0), end
@@ -827,44 +839,44 @@
     def evalId(self, data, index, text):
         """Evaluate the id from of [ref]  """
 
         return text.lower(), index, True
 
 
 class ImageReferenceInlineProcessor(ReferenceInlineProcessor):
-    """ Match to a stored reference and return img element. """
+    """ Match to a stored reference and return `img` element. """
     def makeTag(self, href, title, text):
         el = etree.Element("img")
         el.set("src", href)
         if title:
             el.set("title", title)
         el.set("alt", self.unescape(text))
         return el
 
 
 class ShortImageReferenceInlineProcessor(ImageReferenceInlineProcessor):
-    """ Short form of inage reference: ![ref]. """
+    """ Short form of image reference: `![ref]`. """
     def evalId(self, data, index, text):
         """Evaluate the id from of [ref]  """
 
         return text.lower(), index, True
 
 
 class AutolinkInlineProcessor(InlineProcessor):
-    """ Return a link Element given an autolink (`<http://example/com>`). """
+    """ Return a link Element given an auto-link (`<http://example/com>`). """
     def handleMatch(self, m, data):
         el = etree.Element("a")
         el.set('href', self.unescape(m.group(1)))
         el.text = util.AtomicString(m.group(1))
         return el, m.start(0), m.end(0)
 
 
 class AutomailInlineProcessor(InlineProcessor):
     """
-    Return a mailto link Element given an automail link (`<foo@example.com>`).
+    Return a `mailto` link Element given an auto-mail link (`<foo@example.com>`).
     """
     def handleMatch(self, m, data):
         el = etree.Element('a')
         email = self.unescape(m.group(1))
         if email.startswith("mailto:"):
             email = email[len("mailto:"):]
```

### Comparing `Markdown-3.4.3/markdown/postprocessors.py` & `Markdown-3.4.4/markdown/postprocessors.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
         else:
             return self.run(processed_text)
 
     def isblocklevel(self, html):
         m = self.BLOCK_LEVEL_REGEX.match(html)
         if m:
             if m.group(1)[0] in ('!', '?', '@', '%'):
-                # Comment, php etc...
+                # Comment, PHP etc...
                 return True
             return self.md.is_block_level(m.group(1))
         return False
 
     def stash_to_string(self, text):
         """ Convert a stashed object to a string. """
         return str(text)
```

### Comparing `Markdown-3.4.3/markdown/preprocessors.py` & `Markdown-3.4.4/markdown/preprocessors.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/markdown/serializers.py` & `Markdown-3.4.4/markdown/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# markdown/searializers.py
-#
-# Add x/html serialization to Elementree
+# Add x/html serialization to `Elementree`
 # Taken from ElementTree 1.3 preview with slight modifications
 #
 # Copyright (c) 1999-2007 by Fredrik Lundh.  All rights reserved.
 #
 # fredrik@pythonware.com
 # https://www.pythonware.com/
 #
@@ -124,29 +122,29 @@
         if text:
             write(_escape_cdata(text))
         for e in elem:
             _serialize_html(write, e, format)
     else:
         namespace_uri = None
         if isinstance(tag, QName):
-            # QNAME objects store their data as a string: `{uri}tag`
+            # `QNAME` objects store their data as a string: `{uri}tag`
             if tag.text[:1] == "{":
                 namespace_uri, tag = tag.text[1:].split("}", 1)
             else:
                 raise ValueError('QName objects must define a tag.')
         write("<" + tag)
         items = elem.items()
         if items:
             items = sorted(items)  # lexical order
             for k, v in items:
                 if isinstance(k, QName):
-                    # Assume a text only QName
+                    # Assume a text only `QName`
                     k = k.text
                 if isinstance(v, QName):
-                    # Assume a text only QName
+                    # Assume a text only `QName`
                     v = v.text
                 else:
                     v = _escape_attrib_html(v)
                 if k == v and format == 'html':
                     # handle boolean attributes
                     write(" %s" % v)
                 else:
```

### Comparing `Markdown-3.4.3/markdown/test_tools.py` & `Markdown-3.4.4/markdown/test_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,29 +31,29 @@
     tidylib = None
 
 __all__ = ['TestCase', 'LegacyTestCase', 'Kwargs']
 
 
 class TestCase(unittest.TestCase):
     """
-    A unittest.TestCase subclass with helpers for testing Markdown output.
+    A `unittest.TestCase` subclass with helpers for testing Markdown output.
 
     Define `default_kwargs` as a dict of keywords to pass to Markdown for each
     test. The defaults can be overridden on individual tests.
 
     The `assertMarkdownRenders` method accepts the source text, the expected
     output, and any keywords to pass to Markdown. The `default_kwargs` are used
     except where overridden by `kwargs`. The output and expected output are passed
-    to `TestCase.assertMultiLineEqual`. An AssertionError is raised with a diff
+    to `TestCase.assertMultiLineEqual`. An `AssertionError` is raised with a diff
     if the actual output does not equal the expected output.
 
     The `dedent` method is available to dedent triple-quoted strings if
     necessary.
 
-    In all other respects, behaves as unittest.TestCase.
+    In all other respects, behaves as `unittest.TestCase`.
     """
 
     default_kwargs = {}
 
     def assertMarkdownRenders(self, source, expected, expected_attrs=None, **kwargs):
         """
         Test that source Markdown text renders to expected output with given keywords.
@@ -76,15 +76,15 @@
 
     def dedent(self, text):
         """
         Dedent text.
         """
 
         # TODO: If/when actual output ends with a newline, then use:
-        # return textwrap.dedent(text.strip('/n'))
+        #     return textwrap.dedent(text.strip('/n'))
         return textwrap.dedent(text).strip()
 
 
 class recursionlimit:
     """
     A context manager which temporarily modifies the Python recursion limit.
 
@@ -117,15 +117,15 @@
 
 class Kwargs(dict):
     """ A dict like class for holding keyword arguments. """
     pass
 
 
 def _normalize_whitespace(text):
-    """ Normalize whitespace for a string of html using tidylib. """
+    """ Normalize whitespace for a string of html using `tidylib`. """
     output, errors = tidylib.tidy_fragment(text, options={
         'drop_empty_paras': 0,
         'fix_backslash': 0,
         'fix_bad_comments': 0,
         'fix_uri': 0,
         'join_styles': 0,
         'lower_literals': 0,
@@ -191,30 +191,30 @@
     """
     A `unittest.TestCase` subclass for running Markdown's legacy file-based tests.
 
     A subclass should define various properties which point to a directory of
     text-based test files and define various behaviors/defaults for those tests.
     The following properties are supported:
 
-    location: A path to the directory of test files. An absolute path is preferred.
-    exclude: A list of tests to exclude. Each test name should comprise the filename
+    `location`: A path to the directory of test files. An absolute path is preferred.
+    `exclude`: A list of tests to exclude. Each test name should comprise the filename
              without an extension.
-    normalize: A boolean value indicating if the HTML should be normalized.
+    `normalize`: A boolean value indicating if the HTML should be normalized.
                Default: `False`.
-    input_ext: A string containing the file extension of input files. Default: `.txt`.
-    ouput_ext: A string containing the file extension of expected output files.
+    `input_ext`: A string containing the file extension of input files. Default: `.txt`.
+    `output_ext`: A string containing the file extension of expected output files.
                Default: `html`.
-    default_kwargs: A `Kwargs` instance which stores the default set of keyword
+    `default_kwargs`: A `Kwargs` instance which stores the default set of keyword
                     arguments for all test files in the directory.
 
     In addition, properties can be defined for each individual set of test files within
     the directory. The property should be given the name of the file without the file
     extension. Any spaces and dashes in the filename should be replaced with
     underscores. The value of the property should be a `Kwargs` instance which
     contains the keyword arguments that should be passed to `Markdown` for that
     test file. The keyword arguments will "update" the `default_kwargs`.
 
     When the class instance is created, it will walk the given directory and create
-    a separate unitttest for each set of test files using the naming scheme:
-    `test_filename`. One unittest will be run for each set of input and output files.
+    a separate `Unitttest` for each set of test files using the naming scheme:
+    `test_filename`. One `Unittest` will be run for each set of input and output files.
     """
     pass
```

### Comparing `Markdown-3.4.3/markdown/treeprocessors.py` & `Markdown-3.4.4/markdown/treeprocessors.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import re
 import xml.etree.ElementTree as etree
 from . import util
 from . import inlinepatterns
 
 
 def build_treeprocessors(md, **kwargs):
-    """ Build the default treeprocessors for Markdown. """
+    """ Build the default  `treeprocessors` for Markdown. """
     treeprocessors = util.Registry()
     treeprocessors.register(InlineProcessor(md), 'inline', 20)
     treeprocessors.register(PrettifyTreeprocessor(md), 'prettify', 10)
     treeprocessors.register(UnescapeTreeprocessor(md), 'unescape', 0)
     return treeprocessors
 
 
@@ -39,36 +39,36 @@
     if not isinstance(s, util.AtomicString):
         return isinstance(s, str)
     return False
 
 
 class Treeprocessor(util.Processor):
     """
-    Treeprocessors are run on the ElementTree object before serialization.
+    `Treeprocessor`s are run on the `ElementTree` object before serialization.
 
-    Each Treeprocessor implements a "run" method that takes a pointer to an
-    ElementTree, modifies it as necessary and returns an ElementTree
+    Each `Treeprocessor` implements a `run` method that takes a pointer to an
+    `ElementTree`, modifies it as necessary and returns an `ElementTree`
     object.
 
-    Treeprocessors must extend markdown.Treeprocessor.
+    `Treeprocessors` must extend `markdown.Treeprocessor`.
 
     """
     def run(self, root):
         """
-        Subclasses of Treeprocessor should implement a `run` method, which
-        takes a root ElementTree. This method can return another ElementTree
-        object, and the existing root ElementTree will be replaced, or it can
-        modify the current tree and return None.
+        Subclasses of `Treeprocessor` should implement a `run` method, which
+        takes a root `ElementTree`. This method can return another `ElementTree`
+        object, and the existing root `ElementTree `will be replaced, or it can
+        modify the current tree and return `None`.
         """
         pass  # pragma: no cover
 
 
 class InlineProcessor(Treeprocessor):
     """
-    A Treeprocessor that traverses a tree, applying inline patterns.
+    A `Treeprocessor` that traverses a tree, applying inline patterns.
     """
 
     def __init__(self, md):
         self.__placeholder_prefix = util.INLINE_PLACEHOLDER_PREFIX
         self.__placeholder_suffix = util.ETX
         self.__placeholder_length = 4 + len(self.__placeholder_prefix) \
                                       + len(self.__placeholder_suffix)
@@ -85,16 +85,16 @@
 
     def __findPlaceholder(self, data, index):
         """
         Extract id from data string, start from index
 
         Keyword arguments:
 
-        * data: string
-        * index: index, from which we start search
+        * `data`: string
+        * `index`: index, from which we start search
 
         Returns: placeholder id and string index, after the found placeholder.
 
         """
         m = self.__placeholder_re.search(data, index)
         if m:
             return m.group(1), m.end()
@@ -110,16 +110,16 @@
     def __handleInline(self, data, patternIndex=0):
         """
         Process string with inline patterns and replace it
         with placeholders
 
         Keyword arguments:
 
-        * data: A line of Markdown text
-        * patternIndex: The index of the inlinePattern to start with
+        * `data`: A line of Markdown text
+        * `patternIndex`: The index of the `inlinePattern` to start with
 
         Returns: String with placeholders.
 
         """
         if not isinstance(data, util.AtomicString):
             startIndex = 0
             count = len(self.inlinePatterns)
@@ -129,22 +129,22 @@
                 )
                 if not matched:
                     patternIndex += 1
         return data
 
     def __processElementText(self, node, subnode, isText=True):
         """
-        Process placeholders in Element.text or Element.tail
-        of Elements popped from self.stashed_nodes.
+        Process placeholders in `Element.text` or `Element.tail`
+        of Elements popped from `self.stashed_nodes`.
 
         Keywords arguments:
 
-        * node: parent node
-        * subnode: processing node
-        * isText: bool variable, True - it's text, False - it's tail
+        * `node`: parent node
+        * `subnode`: processing node
+        * `isText`: boolean variable, True - it's text, False - it's a tail
 
         Returns: None
 
         """
         if isText:
             text = subnode.text
             subnode.text = None
@@ -161,22 +161,22 @@
 
         childResult.reverse()
         for newChild in childResult:
             node.insert(pos, newChild[0])
 
     def __processPlaceholders(self, data, parent, isText=True):
         """
-        Process string with placeholders and generate ElementTree tree.
+        Process string with placeholders and generate `ElementTree` tree.
 
         Keyword arguments:
 
-        * data: string with placeholders instead of ElementTree elements.
-        * parent: Element, which contains processing inline data
+        * `data`: string with placeholders instead of `ElementTree` elements.
+        * `parent`: Element, which contains processing inline data
 
-        Returns: list with ElementTree elements with applied inline patterns.
+        Returns: list with `ElementTree` elements with applied inline patterns.
 
         """
         def linkText(text):
             if text:
                 if result:
                     if result[-1][0].tail:
                         result[-1][0].tail += text
@@ -227,45 +227,45 @@
                 else:  # wrong placeholder
                     end = index + len(self.__placeholder_prefix)
                     linkText(data[strartIndex:end])
                     strartIndex = end
             else:
                 text = data[strartIndex:]
                 if isinstance(data, util.AtomicString):
-                    # We don't want to loose the AtomicString
+                    # We don't want to loose the `AtomicString`
                     text = util.AtomicString(text)
                 linkText(text)
                 data = ""
 
         return result
 
     def __applyPattern(self, pattern, data, patternIndex, startIndex=0):
         """
         Check if the line fits the pattern, create the necessary
-        elements, add it to stashed_nodes.
+        elements, add it to `stashed_nodes`.
 
         Keyword arguments:
 
-        * data: the text to be processed
-        * pattern: the pattern to be checked
-        * patternIndex: index of current pattern
-        * startIndex: string index, from which we start searching
+        * `data`: the text to be processed
+        * `pattern`: the pattern to be checked
+        * `patternIndex`: index of current pattern
+        * `startIndex`: string index, from which we start searching
 
-        Returns: String with placeholders instead of ElementTree elements.
+        Returns: String with placeholders instead of `ElementTree` elements.
 
         """
         new_style = isinstance(pattern, inlinepatterns.InlineProcessor)
 
         for exclude in pattern.ANCESTOR_EXCLUDES:
             if exclude.lower() in self.ancestors:
                 return data, False, 0
 
         if new_style:
             match = None
-            # Since handleMatch may reject our first match,
+            # Since `handleMatch` may reject our first match,
             # we iterate over the buffer looking for matches
             # until we can't find any more.
             for match in pattern.getCompiledRegExp().finditer(data, startIndex):
                 node, start, end = pattern.handleMatch(match, data)
                 if start is None or end is None:
                     startIndex += match.end(0)
                     match = None
@@ -321,27 +321,27 @@
             parent = self.parent_map.get(parent)
         ancestors.reverse()
         parents.extend(ancestors)
 
     def run(self, tree, ancestors=None):
         """Apply inline patterns to a parsed Markdown tree.
 
-        Iterate over ElementTree, find elements with inline tag, apply inline
+        Iterate over `ElementTree`, find elements with inline tag, apply inline
         patterns and append newly created Elements to tree.  If you don't
         want to process your data with inline patterns, instead of normal
-        string, use subclass AtomicString:
+        string, use subclass `AtomicString`:
 
             node.text = markdown.AtomicString("This will not be processed.")
 
         Arguments:
 
-        * tree: ElementTree object, representing Markdown tree.
-        * ancestors: List of parent tag names that precede the tree node (if needed).
+        * `tree`: `ElementTree` object, representing Markdown tree.
+        * `ancestors`: List of parent tag names that precede the tree node (if needed).
 
-        Returns: ElementTree object with applied inline patterns.
+        Returns: `ElementTree` object with applied inline patterns.
 
         """
         self.stashed_nodes = {}
 
         # Ensure a valid parent list, but copy passed in lists
         # to ensure we don't have the user accidentally change it on us.
         tree_parents = [] if ancestors is None else ancestors[:]
@@ -391,36 +391,36 @@
                 for i, obj in enumerate(lst):
                     newChild = obj[0]
                     element.insert(i, newChild)
         return tree
 
 
 class PrettifyTreeprocessor(Treeprocessor):
-    """ Add linebreaks to the html document. """
+    """ Add line breaks to the html document. """
 
     def _prettifyETree(self, elem):
-        """ Recursively add linebreaks to ElementTree children. """
+        """ Recursively add line breaks to `ElementTree` children. """
 
         i = "\n"
         if self.md.is_block_level(elem.tag) and elem.tag not in ['code', 'pre']:
             if (not elem.text or not elem.text.strip()) \
                     and len(elem) and self.md.is_block_level(elem[0].tag):
                 elem.text = i
             for e in elem:
                 if self.md.is_block_level(e.tag):
                     self._prettifyETree(e)
         if not elem.tail or not elem.tail.strip():
             elem.tail = i
 
     def run(self, root):
-        """ Add linebreaks to ElementTree root object. """
+        """ Add line breaks to `ElementTree` root object. """
 
         self._prettifyETree(root)
-        # Do <br />'s separately as they are often in the middle of
-        # inline content and missed by _prettifyETree.
+        # Do `<br />`'s separately as they are often in the middle of
+        # inline content and missed by `_prettifyETree`.
         brs = root.iter('br')
         for br in brs:
             if not br.tail or not br.tail.strip():
                 br.tail = '\n'
             else:
                 br.tail = '\n%s' % br.tail
         # Clean up extra empty lines at end of code blocks.
```

### Comparing `Markdown-3.4.3/markdown/util.py` & `Markdown-3.4.4/markdown/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     # Other elements which Markdown should not be mucking up the contents of.
     'canvas', 'colgroup', 'dd', 'body', 'dt', 'group', 'html', 'iframe', 'li', 'legend',
     'math', 'map', 'noscript', 'output', 'object', 'option', 'progress', 'script',
     'style', 'summary', 'tbody', 'td', 'textarea', 'tfoot', 'th', 'thead', 'tr', 'video'
 ]
 
 # Placeholders
-STX = '\u0002'  # Use STX ("Start of text") for start-of-placeholder
-ETX = '\u0003'  # Use ETX ("End of text") for end-of-placeholder
+STX = '\u0002'  # Use `STX` ("Start of text") for start-of-placeholder
+ETX = '\u0003'  # Use `ETX` ("End of text") for end-of-placeholder
 INLINE_PLACEHOLDER_PREFIX = STX+"klzzwxh:"
 INLINE_PLACEHOLDER = INLINE_PLACEHOLDER_PREFIX + "%s" + ETX
 INLINE_PLACEHOLDER_RE = re.compile(INLINE_PLACEHOLDER % r'([0-9]+)')
 AMP_SUBSTITUTE = STX+"amp"+ETX
 HTML_PLACEHOLDER = STX + "wzxhzdk:%s" + ETX
 HTML_PLACEHOLDER_RE = re.compile(HTML_PLACEHOLDER % r'([0-9]+)')
 TAG_PLACEHOLDER = STX + "hzzhzkh:%s" + ETX
@@ -78,23 +78,23 @@
 """
 
 
 @lru_cache(maxsize=None)
 def get_installed_extensions():
     if sys.version_info >= (3, 10):
         from importlib import metadata
-    else:  # <PY310 use backport
+    else:  # `<PY310` use backport
         import importlib_metadata as metadata
     # Only load extension entry_points once.
     return metadata.entry_points(group='markdown.extensions')
 
 
 def deprecated(message, stacklevel=2):
     """
-    Raise a DeprecationWarning when wrapped function/method is called.
+    Raise a `DeprecationWarning` when wrapped function/method is called.
 
     Usage:
         @deprecated("This method will be removed in version X; use Y instead.")
         def some_method()"
             pass
     """
     def wrapper(func):
@@ -107,18 +107,18 @@
             )
             return func(*args, **kwargs)
         return deprecated_func
     return wrapper
 
 
 def parseBoolValue(value, fail_on_errors=True, preserve_none=False):
-    """Parses a string representing bool value. If parsing was successful,
-       returns True or False. If preserve_none=True, returns True, False,
-       or None. If parsing was not successful, raises  ValueError, or, if
-       fail_on_errors=False, returns None."""
+    """Parses a string representing boolean value. If parsing was successful,
+       returns True or False. If `preserve_none=True`, returns `True`, `False`,
+       or `None`. If parsing was not successful, raises `ValueError`, or, if
+       `fail_on_errors=False`, returns `None`."""
     if not isinstance(value, str):
         if preserve_none and value is None:
             return value
         return bool(value)
     elif preserve_none and value.lower() == 'none':
         return None
     elif value.lower() in ('true', 'yes', 'y', 'on', '1'):
@@ -175,29 +175,29 @@
 class HtmlStash:
     """
     This class is used for stashing HTML objects that we extract
     in the beginning and replace with place-holders.
     """
 
     def __init__(self):
-        """ Create a HtmlStash. """
+        """ Create an `HtmlStash`. """
         self.html_counter = 0  # for counting inline html segments
         self.rawHtmlBlocks = []
         self.tag_counter = 0
         self.tag_data = []  # list of dictionaries in the order tags appear
 
     def store(self, html):
         """
         Saves an HTML segment for later reinsertion.  Returns a
         placeholder string that needs to be inserted into the
         document.
 
         Keyword arguments:
 
-        * html: an html segment
+        * `html`: an html segment
 
         Returns : a placeholder string
 
         """
         self.rawHtmlBlocks.append(html)
         placeholder = self.get_placeholder(self.html_counter)
         self.html_counter += 1
@@ -212,15 +212,15 @@
 
     def store_tag(self, tag, attrs, left_index, right_index):
         """Store tag data and return a placeholder."""
         self.tag_data.append({'tag': tag, 'attrs': attrs,
                               'left_index': left_index,
                               'right_index': right_index})
         placeholder = TAG_PLACEHOLDER % str(self.tag_counter)
-        self.tag_counter += 1  # equal to the tag's index in self.tag_data
+        self.tag_counter += 1  # equal to the tag's index in `self.tag_data`
         return placeholder
 
 
 # Used internally by `Registry` for each item in its sorted list.
 # Provides an easier to read API when editing the code later.
 # For example, `item.name` is more clear than `item[0]`.
 _PriorityItem = namedtuple('PriorityItem', ['name', 'priority'])
```

### Comparing `Markdown-3.4.3/mkdocs.yml` & `Markdown-3.4.4/mkdocs.yml`

 * *Files 6% similar despite different names*

```diff
@@ -58,7 +58,10 @@
 markdown_extensions:
   - extra
   - admonition
   - smarty
   - codehilite
   - toc:
       permalink: true
+  - mdx_gh_links:
+      user: Python-Markdown
+      repo: markdown
```

### Comparing `Markdown-3.4.3/pyproject.toml` & `Markdown-3.4.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 ]
 
 [project.optional-dependencies]
 testing = [
     'coverage',
     'pyyaml',
 ]
+docs = [
+    'mkdocs>=1.0',
+    'mkdocs-nature>=0.4',
+    'mdx_gh_links>=0.2'
+]
 
 [project.urls]
 'Homepage' = 'https://Python-Markdown.github.io/'
 'Documentation' = 'https://Python-Markdown.github.io/'
 'Repository' = 'https://github.com/Python-Markdown/markdown'
 'Issue Tracker' = 'https://github.com/Python-Markdown/markdown/issues'
 'Changelog' = 'https://github.com/Python-Markdown/markdown/blob/master/docs/change_log/index.md'
```

### Comparing `Markdown-3.4.3/tests/__init__.py` & `Markdown-3.4.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/auto-links.html` & `Markdown-3.4.4/tests/basic/auto-links.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/backlash-escapes.html` & `Markdown-3.4.4/tests/basic/backlash-escapes.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/backlash-escapes.txt` & `Markdown-3.4.4/tests/basic/backlash-escapes.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/links-reference.html` & `Markdown-3.4.4/tests/basic/links-reference.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/links-reference.txt` & `Markdown-3.4.4/tests/basic/links-reference.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/markdown-documentation-basics.html` & `Markdown-3.4.4/tests/basic/markdown-documentation-basics.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/markdown-documentation-basics.txt` & `Markdown-3.4.4/tests/basic/markdown-documentation-basics.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/markdown-syntax.html` & `Markdown-3.4.4/tests/basic/markdown-syntax.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/markdown-syntax.txt` & `Markdown-3.4.4/tests/basic/markdown-syntax.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/ordered-and-unordered-list.html` & `Markdown-3.4.4/tests/basic/ordered-and-unordered-list.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/basic/ordered-and-unordered-list.txt` & `Markdown-3.4.4/tests/basic/ordered-and-unordered-list.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/admonition.html` & `Markdown-3.4.4/tests/extensions/admonition.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/admonition.txt` & `Markdown-3.4.4/tests/extensions/admonition.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/attr_list.html` & `Markdown-3.4.4/tests/extensions/attr_list.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/attr_list.txt` & `Markdown-3.4.4/tests/extensions/attr_list.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/codehilite.html` & `Markdown-3.4.4/tests/extensions/codehilite.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/extra/footnote.html` & `Markdown-3.4.4/tests/extensions/extra/footnote.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/extra/footnote.txt` & `Markdown-3.4.4/tests/extensions/extra/footnote.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/extra/footnote_many_footnotes.html` & `Markdown-3.4.4/tests/extensions/extra/footnote_many_footnotes.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/extra/footnote_many_footnotes.txt` & `Markdown-3.4.4/tests/extensions/extra/footnote_many_footnotes.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/extra/markdown-syntax.html` & `Markdown-3.4.4/tests/extensions/extra/markdown-syntax.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/extra/markdown-syntax.txt` & `Markdown-3.4.4/tests/extensions/extra/markdown-syntax.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/extra/named_markers.html` & `Markdown-3.4.4/tests/extensions/extra/named_markers.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/extra/raw-html.html` & `Markdown-3.4.4/tests/extensions/extra/raw-html.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/extra/raw-html.txt` & `Markdown-3.4.4/tests/extensions/extra/raw-html.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/extra/simple_def-lists.html` & `Markdown-3.4.4/tests/extensions/extra/simple_def-lists.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/github_flavored.html` & `Markdown-3.4.4/tests/extensions/github_flavored.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/github_flavored.txt` & `Markdown-3.4.4/tests/extensions/github_flavored.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/toc.html` & `Markdown-3.4.4/tests/extensions/toc.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/toc.txt` & `Markdown-3.4.4/tests/extensions/toc.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/toc_nested.html` & `Markdown-3.4.4/tests/extensions/toc_nested.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/toc_nested2.html` & `Markdown-3.4.4/tests/extensions/toc_nested2.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/toc_nested_list.html` & `Markdown-3.4.4/tests/extensions/toc_nested_list.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/extensions/wikilinks.html` & `Markdown-3.4.4/tests/extensions/wikilinks.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/arabic.html` & `Markdown-3.4.4/tests/misc/arabic.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/arabic.txt` & `Markdown-3.4.4/tests/misc/arabic.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/bidi.html` & `Markdown-3.4.4/tests/misc/bidi.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/bidi.txt` & `Markdown-3.4.4/tests/misc/bidi.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/blank_lines_in_codeblocks.txt` & `Markdown-3.4.4/tests/misc/blank_lines_in_codeblocks.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/blockquote.html` & `Markdown-3.4.4/tests/misc/blockquote.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/br.html` & `Markdown-3.4.4/tests/misc/br.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/brackets-in-img-title.html` & `Markdown-3.4.4/tests/misc/brackets-in-img-title.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/em-around-links.html` & `Markdown-3.4.4/tests/misc/em-around-links.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/em-around-links.txt` & `Markdown-3.4.4/tests/misc/em-around-links.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/em_strong_complex.html` & `Markdown-3.4.4/tests/misc/em_strong_complex.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/email.html` & `Markdown-3.4.4/tests/misc/email.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/japanese.html` & `Markdown-3.4.4/tests/misc/japanese.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/japanese.txt` & `Markdown-3.4.4/tests/misc/japanese.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/lists7.html` & `Markdown-3.4.4/tests/misc/lists7.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/lists7.txt` & `Markdown-3.4.4/tests/misc/lists7.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/lists8.html` & `Markdown-3.4.4/tests/misc/lists8.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/multi-test.html` & `Markdown-3.4.4/tests/misc/multi-test.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/nested-lists.html` & `Markdown-3.4.4/tests/misc/nested-lists.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/nested-patterns.html` & `Markdown-3.4.4/tests/misc/nested-patterns.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/russian.html` & `Markdown-3.4.4/tests/misc/russian.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/russian.txt` & `Markdown-3.4.4/tests/misc/russian.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/some-test.html` & `Markdown-3.4.4/tests/misc/some-test.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/misc/some-test.txt` & `Markdown-3.4.4/tests/misc/some-test.txt`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2004/Auto links.html` & `Markdown-3.4.4/tests/pl/Tests_2004/Auto links.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2004/Backslash escapes.html` & `Markdown-3.4.4/tests/pl/Tests_2004/Backslash escapes.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2004/Inline HTML (Simple).html` & `Markdown-3.4.4/tests/pl/Tests_2004/Inline HTML (Simple).html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2004/Markdown Documentation - Basics.html` & `Markdown-3.4.4/tests/pl/Tests_2004/Markdown Documentation - Basics.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2004/Markdown Documentation - Syntax.html` & `Markdown-3.4.4/tests/pl/Tests_2004/Markdown Documentation - Syntax.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2004/Ordered and unordered lists.html` & `Markdown-3.4.4/tests/pl/Tests_2004/Ordered and unordered lists.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2004/Yuri-Attributes.html` & `Markdown-3.4.4/tests/pl/Tests_2004/Yuri-Attributes.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2004/Yuri-Email.html` & `Markdown-3.4.4/tests/pl/Tests_2004/Yuri-Email.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2004/Yuri-Footnotes.html` & `Markdown-3.4.4/tests/pl/Tests_2004/Yuri-Footnotes.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2007/Auto links.html` & `Markdown-3.4.4/tests/pl/Tests_2007/Auto links.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2007/Backslash escapes.html` & `Markdown-3.4.4/tests/pl/Tests_2007/Backslash escapes.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2007/Images.html` & `Markdown-3.4.4/tests/pl/Tests_2007/Images.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2007/Inline HTML (Simple).html` & `Markdown-3.4.4/tests/pl/Tests_2007/Inline HTML (Simple).html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2007/Links, inline style.html` & `Markdown-3.4.4/tests/pl/Tests_2007/Links, inline style.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2007/Links, reference style.html` & `Markdown-3.4.4/tests/pl/Tests_2007/Links, reference style.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2007/Markdown Documentation - Basics.html` & `Markdown-3.4.4/tests/pl/Tests_2007/Markdown Documentation - Basics.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2007/Markdown Documentation - Syntax.html` & `Markdown-3.4.4/tests/pl/Tests_2007/Markdown Documentation - Syntax.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/pl/Tests_2007/Ordered and unordered lists.html` & `Markdown-3.4.4/tests/pl/Tests_2007/Ordered and unordered lists.html`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_apis.py` & `Markdown-3.4.4/tests/test_apis.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Copyright 2004 Manfred Stienstra (the original version)
 
 License: BSD (see LICENSE.md for details).
 
 Python-Markdown Regression Tests
 ================================
 
-Tests of the various APIs with the python markdown lib.
+Tests of the various APIs with the Python Markdown library.
 """
 
 import unittest
 import sys
 import os
 import markdown
 import warnings
@@ -118,37 +118,37 @@
     """ Tests of the BlockParser class. """
 
     def setUp(self):
         """ Create instance of BlockParser. """
         self.parser = markdown.Markdown().parser
 
     def testParseChunk(self):
-        """ Test BlockParser.parseChunk. """
+        """ Test `BlockParser.parseChunk`. """
         root = etree.Element("div")
         text = 'foo'
         self.parser.parseChunk(root, text)
         self.assertEqual(
             markdown.serializers.to_xhtml_string(root),
             "<div><p>foo</p></div>"
         )
 
     def testParseDocument(self):
-        """ Test BlockParser.parseDocument. """
+        """ Test `BlockParser.parseDocument`. """
         lines = ['#foo', '', 'bar', '', '    baz']
         tree = self.parser.parseDocument(lines)
         self.assertIsInstance(tree, etree.ElementTree)
         self.assertIs(etree.iselement(tree.getroot()), True)
         self.assertEqual(
             markdown.serializers.to_xhtml_string(tree.getroot()),
             "<div><h1>foo</h1><p>bar</p><pre><code>baz\n</code></pre></div>"
         )
 
 
 class TestBlockParserState(unittest.TestCase):
-    """ Tests of the State class for BlockParser. """
+    """ Tests of the State class for `BlockParser`. """
 
     def setUp(self):
         self.state = markdown.blockparser.State()
 
     def testBlankState(self):
         """ Test State when empty. """
         self.assertEqual(self.state, [])
@@ -157,66 +157,66 @@
         """ Test State.set(). """
         self.state.set('a_state')
         self.assertEqual(self.state, ['a_state'])
         self.state.set('state2')
         self.assertEqual(self.state, ['a_state', 'state2'])
 
     def testIsSate(self):
-        """ Test State.isstate(). """
+        """ Test `State.isstate()`. """
         self.assertEqual(self.state.isstate('anything'), False)
         self.state.set('a_state')
         self.assertEqual(self.state.isstate('a_state'), True)
         self.state.set('state2')
         self.assertEqual(self.state.isstate('state2'), True)
         self.assertEqual(self.state.isstate('a_state'), False)
         self.assertEqual(self.state.isstate('missing'), False)
 
     def testReset(self):
-        """ Test State.reset(). """
+        """ Test `State.reset()`. """
         self.state.set('a_state')
         self.state.reset()
         self.assertEqual(self.state, [])
         self.state.set('state1')
         self.state.set('state2')
         self.state.reset()
         self.assertEqual(self.state, ['state1'])
 
 
 class TestHtmlStash(unittest.TestCase):
-    """ Test Markdown's HtmlStash. """
+    """ Test Markdown's `HtmlStash`. """
 
     def setUp(self):
         self.stash = markdown.util.HtmlStash()
         self.placeholder = self.stash.store('foo')
 
     def testSimpleStore(self):
-        """ Test HtmlStash.store. """
+        """ Test `HtmlStash.store`. """
         self.assertEqual(self.placeholder, self.stash.get_placeholder(0))
         self.assertEqual(self.stash.html_counter, 1)
         self.assertEqual(self.stash.rawHtmlBlocks, ['foo'])
 
     def testStoreMore(self):
-        """ Test HtmlStash.store with additional blocks. """
+        """ Test `HtmlStash.store` with additional blocks. """
         placeholder = self.stash.store('bar')
         self.assertEqual(placeholder, self.stash.get_placeholder(1))
         self.assertEqual(self.stash.html_counter, 2)
         self.assertEqual(
             self.stash.rawHtmlBlocks,
             ['foo', 'bar']
         )
 
     def testReset(self):
-        """ Test HtmlStash.reset. """
+        """ Test `HtmlStash.reset`. """
         self.stash.reset()
         self.assertEqual(self.stash.html_counter, 0)
         self.assertEqual(self.stash.rawHtmlBlocks, [])
 
 
 class Item:
-    """ A dummy Registry item object for testing. """
+    """ A dummy `Registry` item object for testing. """
     def __init__(self, data):
         self.data = data
 
     def __repr__(self):
         return repr(self.data)
 
     def __eq__(self, other):
@@ -268,19 +268,19 @@
         r.register(Item('b'), 'b', 30)
         r.register(Item('c'), 'c', 40)
         self.assertEqual(len(r), 3)
         r.deregister('b')
         self.assertEqual(len(r), 2)
         r.deregister('c', strict=False)
         self.assertEqual(len(r), 1)
-        # deregister non-existent item with strict=False
+        # deregister non-existent item with `strict=False`
         r.deregister('d', strict=False)
         self.assertEqual(len(r), 1)
         with self.assertRaises(ValueError):
-            # deregister non-existent item with strict=True
+            # deregister non-existent item with `strict=True`
             r.deregister('e')
         self.assertEqual(list(r), ['a'])
 
     def testRegistryContains(self):
         r = markdown.util.Registry()
         item = Item('a')
         r.register(item, 'a', 20)
@@ -392,78 +392,78 @@
         self.assertRaises(
             AttributeError,
             markdown.Markdown,
             extensions=['markdown.extensions.footnotes:MissingExtension']
         )
 
     def testBaseExtention(self):
-        """ Test that the base Extension class will raise NotImplemented. """
+        """ Test that the base Extension class will raise `NotImplemented`. """
         self.assertRaises(
             NotImplementedError,
             markdown.Markdown, extensions=[markdown.extensions.Extension()]
         )
 
 
 class testETreeComments(unittest.TestCase):
     """
-    Test that ElementTree Comments work.
+    Test that `ElementTree` Comments work.
 
-    These tests should only be a concern when using cElementTree with third
+    These tests should only be a concern when using `cElementTree` with third
     party serializers (including markdown's (x)html serializer). While markdown
-    doesn't use ElementTree.Comment itself, we should certainly support any
+    doesn't use `ElementTree.Comment` itself, we should certainly support any
     third party extensions which may. Therefore, these tests are included to
     ensure such support is maintained.
     """
 
     def setUp(self):
         # Create comment node
         self.comment = etree.Comment('foo')
 
     def testCommentIsComment(self):
-        """ Test that an ElementTree Comment passes the `is Comment` test. """
+        """ Test that an `ElementTree` `Comment` passes the `is Comment` test. """
         self.assertIs(self.comment.tag, etree.Comment)
 
     def testCommentIsBlockLevel(self):
-        """ Test that an ElementTree Comment is recognized as BlockLevel. """
+        """ Test that an `ElementTree` `Comment` is recognized as `BlockLevel`. """
         md = markdown.Markdown()
         self.assertIs(md.is_block_level(self.comment.tag), False)
 
     def testCommentSerialization(self):
-        """ Test that an ElementTree Comment serializes properly. """
+        """ Test that an `ElementTree` `Comment` serializes properly. """
         self.assertEqual(
             markdown.serializers.to_html_string(self.comment),
             '<!--foo-->'
         )
 
     def testCommentPrettify(self):
-        """ Test that an ElementTree Comment is prettified properly. """
+        """ Test that an `ElementTree` `Comment` is prettified properly. """
         pretty = markdown.treeprocessors.PrettifyTreeprocessor(markdown.Markdown())
         pretty.run(self.comment)
         self.assertEqual(
             markdown.serializers.to_html_string(self.comment),
             '<!--foo-->\n'
         )
 
 
 class testElementTailTests(unittest.TestCase):
     """ Element Tail Tests """
     def setUp(self):
         self.pretty = markdown.treeprocessors.PrettifyTreeprocessor(markdown.Markdown())
 
     def testBrTailNoNewline(self):
-        """ Test that last <br> in tree has a new line tail """
+        """ Test that last `<br>` in tree has a new line tail """
         root = etree.Element('root')
         br = etree.SubElement(root, 'br')
         self.assertEqual(br.tail, None)
         self.pretty.run(root)
         self.assertEqual(br.tail, "\n")
 
 
 class testElementPreCodeTests(unittest.TestCase):
-    """ Element PreCode Tests """
+    """ Element `PreCode` Tests """
     def setUp(self):
         md = markdown.Markdown()
         self.pretty = markdown.treeprocessors.PrettifyTreeprocessor(md)
 
     def prettify(self, xml):
         root = etree.fromstring(xml)
         self.pretty.run(root)
@@ -553,24 +553,24 @@
         etree.SubElement(el, 'HR')
         self.assertEqual(
             markdown.serializers.to_xhtml_string(el),
             '<MixedCase>not valid <EMPHASIS>html</EMPHASIS><HR /></MixedCase>'
         )
 
     def testProsessingInstruction(self):
-        """ Test serialization of ProcessignInstruction. """
+        """ Test serialization of `ProcessignInstruction`. """
         pi = ProcessingInstruction('foo', text='<&"test\nescaping">')
         self.assertIs(pi.tag, ProcessingInstruction)
         self.assertEqual(
             markdown.serializers.to_xhtml_string(pi),
             '<?foo &lt;&amp;"test\nescaping"&gt;?>'
         )
 
     def testQNameTag(self):
-        """ Test serialization of QName tag. """
+        """ Test serialization of `QName` tag. """
         div = etree.Element('div')
         qname = etree.QName('http://www.w3.org/1998/Math/MathML', 'math')
         math = etree.SubElement(div, qname)
         math.set('display', 'block')
         sem = etree.SubElement(math, 'semantics')
         msup = etree.SubElement(sem, 'msup')
         mi = etree.SubElement(msup, 'mi')
@@ -591,50 +591,50 @@
             '<annotations>x^2</annotations>'
             '</semantics>'
             '</math>'
             '</div>'
         )
 
     def testQNameAttribute(self):
-        """ Test serialization of QName attribute. """
+        """ Test serialization of `QName` attribute. """
         div = etree.Element('div')
         div.set(etree.QName('foo'), etree.QName('bar'))
         self.assertEqual(
             markdown.serializers.to_xhtml_string(div),
             '<div foo="bar"></div>'
         )
 
     def testBadQNameTag(self):
-        """ Test serialization of QName with no tag. """
+        """ Test serialization of `QName` with no tag. """
         qname = etree.QName('http://www.w3.org/1998/Math/MathML')
         el = etree.Element(qname)
         self.assertRaises(ValueError, markdown.serializers.to_xhtml_string, el)
 
     def testQNameEscaping(self):
-        """ Test QName escaping. """
+        """ Test `QName` escaping. """
         qname = etree.QName('<&"test\nescaping">', 'div')
         el = etree.Element(qname)
         self.assertEqual(
             markdown.serializers.to_xhtml_string(el),
             '<div xmlns="&lt;&amp;&quot;test&#10;escaping&quot;&gt;"></div>'
         )
 
     def testQNamePreEscaping(self):
-        """ Test QName that is already partially escaped. """
+        """ Test `QName` that is already partially escaped. """
         qname = etree.QName('&lt;&amp;"test&#10;escaping"&gt;', 'div')
         el = etree.Element(qname)
         self.assertEqual(
             markdown.serializers.to_xhtml_string(el),
             '<div xmlns="&lt;&amp;&quot;test&#10;escaping&quot;&gt;"></div>'
         )
 
     def buildExtension(self):
-        """ Build an extension which registers fakeSerializer. """
+        """ Build an extension which registers `fakeSerializer`. """
         def fakeSerializer(elem):
-            # Ignore input and return hardcoded output
+            # Ignore input and return hard-coded output
             return '<div><p>foo</p></div>'
 
         class registerFakeSerializer(markdown.extensions.Extension):
             def extendMarkdown(self, md):
                 md.output_formats['fake'] = fakeSerializer
 
         return registerFakeSerializer()
@@ -657,15 +657,15 @@
         self.assertEqual(
             markdown.markdown('foo  \nbar', output_format='html'),
             '<p>foo<br>\nbar</p>'
         )
 
 
 class testAtomicString(unittest.TestCase):
-    """ Test that AtomicStrings are honored (not parsed). """
+    """ Test that `AtomicStrings` are honored (not parsed). """
 
     def setUp(self):
         md = markdown.Markdown()
         self.inlineprocessor = md.treeprocessors['inline']
 
     def testString(self):
         """ Test that a regular string is parsed. """
@@ -675,26 +675,26 @@
         new = self.inlineprocessor.run(tree)
         self.assertEqual(
             markdown.serializers.to_html_string(new),
             '<div><p>some <em>text</em></p></div>'
         )
 
     def testSimpleAtomicString(self):
-        """ Test that a simple AtomicString is not parsed. """
+        """ Test that a simple `AtomicString` is not parsed. """
         tree = etree.Element('div')
         p = etree.SubElement(tree, 'p')
         p.text = markdown.util.AtomicString('some *text*')
         new = self.inlineprocessor.run(tree)
         self.assertEqual(
             markdown.serializers.to_html_string(new),
             '<div><p>some *text*</p></div>'
         )
 
     def testNestedAtomicString(self):
-        """ Test that a nested AtomicString is not parsed. """
+        """ Test that a nested `AtomicString` is not parsed. """
         tree = etree.Element('div')
         p = etree.SubElement(tree, 'p')
         p.text = markdown.util.AtomicString('*some* ')
         span1 = etree.SubElement(p, 'span')
         span1.text = markdown.util.AtomicString('*more* ')
         span2 = etree.SubElement(span1, 'span')
         span2.text = markdown.util.AtomicString('*text* ')
@@ -811,15 +811,15 @@
         self.default_options['extensions'] = [
             'markdown.extensions.footnotes',
             'markdown.extensions.smarty'
         ]
         self.assertEqual(options, self.default_options)
 
     def create_config_file(self, config):
-        """ Helper to create temp config files. """
+        """ Helper to create temporary configuration files. """
         if not isinstance(config, str):
             # convert to string
             config = yaml.dump(config)
         fd, self.tempfile = tempfile.mkstemp('.yml')
         with os.fdopen(fd, 'w') as fp:
             fp.write(config)
 
@@ -890,15 +890,15 @@
         md.ESCAPED_CHARS.append('|')
         self.assertEqual('|' in md.ESCAPED_CHARS, True)
         md2 = markdown.Markdown()
         self.assertEqual('|' not in md2.ESCAPED_CHARS, True)
 
 
 class TestBlockAppend(unittest.TestCase):
-    """ Tests block kHTML append. """
+    """ Tests block `kHTML` append. """
 
     def testBlockAppend(self):
         """ Test that appended escapes are only in the current instance. """
         md = markdown.Markdown()
         md.block_level_elements.append('test')
         self.assertEqual('test' in md.block_level_elements, True)
         md2 = markdown.Markdown()
```

### Comparing `Markdown-3.4.3/tests/test_extensions.py` & `Markdown-3.4.4/tests/test_extensions.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 License: BSD (see LICENSE.md for details).
 
 Python-Markdown Extension Regression Tests
 ==========================================
 
 A collection of regression tests to confirm that the included extensions
-continue to work as advertised. This used to be accomplished by doctests.
+continue to work as advertised. This used to be accomplished by `doctests`.
 """
 
 import unittest
 import markdown
 
 
 class TestCaseWithAssertStartsWith(unittest.TestCase):
@@ -73,15 +73,15 @@
         )
 
     def testSetConfig(self):
         self.ext.setConfig('foo', 'baz')
         self.assertEqual(self.ext.getConfigs(), {'foo': 'baz', 'bar': 'baz'})
 
     def testSetConfigWithBadKey(self):
-        # self.ext.setConfig('bad', 'baz) ==> KeyError
+        # `self.ext.setConfig('bad', 'baz)` => `KeyError`
         self.assertRaises(KeyError, self.ext.setConfig, 'bad', 'baz')
 
     def testConfigAsKwargsOnInit(self):
         ext = self.ExtKlass(foo='baz', bar='blah')
         self.assertEqual(ext.getConfigs(), {'foo': 'baz', 'bar': 'blah'})
 
 
@@ -111,15 +111,15 @@
             self.md.convert(text),
             '<p><a href="/foo"><abbr title="Abbreviation">ABBR</abbr></a> '
             'and <em><abbr title="Abbreviation">ABBR</abbr></em></p>'
         )
 
 
 class TestMetaData(unittest.TestCase):
-    """ Test MetaData extension. """
+    """ Test `MetaData` extension. """
 
     def setUp(self):
         self.md = markdown.Markdown(extensions=['meta'])
 
     def testBasicMetaData(self):
         """ Test basic metadata. """
 
@@ -192,31 +192,31 @@
         self.md.convert(text)
 
         self.md.reset()
         self.assertEqual(self.md.Meta, {})
 
 
 class TestWikiLinks(unittest.TestCase):
-    """ Test Wikilinks Extension. """
+    """ Test `Wikilinks` Extension. """
 
     def setUp(self):
         self.md = markdown.Markdown(extensions=['wikilinks'])
         self.text = "Some text with a [[WikiLink]]."
 
     def testBasicWikilinks(self):
-        """ Test [[wikilinks]]. """
+        """ Test `[[wikilinks]]`. """
 
         self.assertEqual(
             self.md.convert(self.text),
             '<p>Some text with a '
             '<a class="wikilink" href="/WikiLink/">WikiLink</a>.</p>'
         )
 
     def testWikilinkWhitespace(self):
-        """ Test whitespace in wikilinks. """
+        """ Test whitespace in `wikilinks`. """
         self.assertEqual(
             self.md.convert('[[ foo bar_baz ]]'),
             '<p><a class="wikilink" href="/foo_bar_baz/">foo bar_baz</a></p>'
         )
         self.assertEqual(
             self.md.convert('foo [[ ]] bar'),
             '<p>foo  bar</p>'
@@ -253,29 +253,29 @@
         self.assertEqual(
             md.convert(self.text),
             '<p>Some text with a '
             '<a href="http://example.com/WikiLink.html">WikiLink</a>.</p>'
         )
 
     def testWikilinksMetaData(self):
-        """ test MetaData with Wikilinks Extension. """
+        """ test `MetaData` with `Wikilinks` Extension. """
 
         text = """wiki_base_url: http://example.com/
 wiki_end_url:   .html
 wiki_html_class:
 
 Some text with a [[WikiLink]]."""
         md = markdown.Markdown(extensions=['meta', 'wikilinks'])
         self.assertEqual(
             md.convert(text),
             '<p>Some text with a '
             '<a href="http://example.com/WikiLink.html">WikiLink</a>.</p>'
         )
 
-        # MetaData should not carry over to next document:
+        # `MetaData` should not carry over to next document:
         self.assertEqual(
             md.convert("No [[MetaData]] here."),
             '<p>No <a class="wikilink" href="/MetaData/">MetaData</a> '
             'here.</p>'
         )
 
     def testURLCallback(self):
@@ -544,15 +544,15 @@
         md.convert('# Header 1\n\n## Header 2')
         self.assertStartsWith(
             '<div class="toc"><span class="toctitle">Table of Contents</span><ul>',
             md.toc
         )
 
     def testWithAttrList(self):
-        """ Test TOC with attr_list Extension. """
+        """ Test TOC with `attr_list` Extension. """
         md = markdown.Markdown(extensions=['toc', 'attr_list'])
         text = ('# Header 1\n\n'
                 '## Header 2 { #foo }\n\n'
                 '## Header 3 { data-toc-label="Foo Bar" }\n\n'
                 '# Header 4 { data-toc-label="Foo > Baz" }\n\n'
                 '# Header 5 { data-toc-label="Foo <b>Quux</b>" }')
 
@@ -625,41 +625,7 @@
             '<div class="toc">\n'                       # noqa
               '<ul>\n'                                  # noqa
                 '<li><a href="#toc">[TOC]</a></li>\n'   # noqa
               '</ul>\n'                                 # noqa
             '</div>\n'                                  # noqa
             '<h1 id="toc"><em>[TOC]</em></h1>'          # noqa
         )
-
-
-class TestSmarty(unittest.TestCase):
-    def setUp(self):
-        config = {
-            'smarty': [
-                ('smart_angled_quotes', True),
-                ('substitutions', {
-                    'ndash': '\u2013',
-                    'mdash': '\u2014',
-                    'ellipsis': '\u2026',
-                    'left-single-quote': '&sbquo;',  # sb is not a typo!
-                    'right-single-quote': '&lsquo;',
-                    'left-double-quote': '&bdquo;',
-                    'right-double-quote': '&ldquo;',
-                    'left-angle-quote': '[',
-                    'right-angle-quote': ']',
-                }),
-            ]
-        }
-        self.md = markdown.Markdown(
-            extensions=['smarty'],
-            extension_configs=config
-        )
-
-    def testCustomSubstitutions(self):
-        text = """<< The "Unicode char of the year 2014"
-is the 'mdash': ---
-Must not be confused with 'ndash'  (--) ... >>
-"""
-        correct = """<p>[ The &bdquo;Unicode char of the year 2014&ldquo;
-is the &sbquo;mdash&lsquo;: \u2014
-Must not be confused with &sbquo;ndash&lsquo;  (\u2013) \u2026 ]</p>"""
-        self.assertEqual(self.md.convert(text), correct)
```

### Comparing `Markdown-3.4.3/tests/test_legacy.py` & `Markdown-3.4.4/tests/test_legacy.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,32 +42,32 @@
 
 class TestPhp(LegacyTestCase):
     """
     Notes on "excluded" tests:
 
     Quotes in attributes: attributes get output in different order
 
-    Inline HTML (Span): Backtick in raw HTML attribute TODO: fixme
+    Inline HTML (Span): Backtick in raw HTML attribute TODO: fix me
 
     Backslash escapes: Weird whitespace issue in output
 
-    Ins & del: Our behavior follows markdown.pl I think PHP is wrong here
+    `Ins` & `del`: Our behavior follows `markdown.pl`. I think PHP is wrong here
 
-    Auto Links: TODO: fix raw HTML so is doesn't match <hr@example.com> as a <hr>.
+    Auto Links: TODO: fix raw HTML so is doesn't match <hr@example.com> as a `<hr>`.
 
-    Empty List Item: We match markdown.pl here. Maybe someday we'll support this
+    Empty List Item: We match `markdown.pl` here. Maybe someday we'll support this
 
     Headers: TODO: fix headers to not require blank line before
 
-    Mixed OLs and ULs: We match markdown.pl here. I think PHP is wrong here
+    Mixed `OL`s and `UL`s: We match `markdown.pl` here. I think PHP is wrong here
 
     Emphasis: We have various minor differences in combined & incorrect em markup.
     Maybe fix a few of them - but most aren't too important
 
-    Code block in a list item: We match markdown.pl - not sure how php gets that output??
+    Code block in a list item: We match `markdown.pl` - not sure how PHP gets that output??
 
     PHP-Specific Bugs: Not sure what to make of the escaping stuff here.
     Why is PHP not removing a backslash?
     """
     location = os.path.join(parent_test_dir, 'php')
     normalize = True
     input_ext = '.text'
@@ -83,22 +83,14 @@
         'Mixed_OLs_and_ULs',
         'Emphasis',
         'Code_block_in_a_list_item',
         'PHP_Specific_Bugs'
     ]
 
 
-# class TestPhpExtra(LegacyTestCase):
-#     location = os.path.join(parent_test_dir, 'php/extra')
-#     normalize = True
-#     input_ext = '.text'
-#     output_ext = '.xhtml'
-#     default_kwargs = Kwargs(extensions=['extra'])
-
-
 class TestPl2004(LegacyTestCase):
     location = os.path.join(parent_test_dir, 'pl/Tests_2004')
     normalize = True
     input_ext = '.text'
     exclude = ['Yuri_Footnotes', 'Yuri_Attributes']
 
 
@@ -106,19 +98,19 @@
     """
     Notes on "excluded" tests:
 
     Images: the attributes don't get ordered the same so we skip this
 
     Code Blocks: some weird whitespace issue
 
-    Links, reference style: weird issue with nested brackets TODO: fixme
+    Links, reference style: weird issue with nested brackets TODO: fix me
 
-    Backslash escapes: backticks in raw html attributes TODO: fixme
+    Backslash escapes: backticks in raw html attributes TODO: fix me
 
-    Code Spans: more backticks in raw html attributes TODO: fixme
+    Code Spans: more backticks in raw html attributes TODO: fix me
     """
     location = os.path.join(parent_test_dir, 'pl/Tests_2007')
     normalize = True
     input_ext = '.text'
     exclude = [
         'Images',
         'Code_Blocks',
@@ -160,19 +152,14 @@
 
     sane_lists = Kwargs(extensions=['sane_lists'])
 
     nl2br_w_attr_list = Kwargs(extensions=['nl2br', 'attr_list'])
 
     admonition = Kwargs(extensions=['admonition'])
 
-    smarty = Kwargs(
-        extensions=['smarty'],
-        extension_configs={'smarty': {'smart_angled_quotes': True}}
-    )
-
 
 class TestExtensionsExtra(LegacyTestCase):
     location = os.path.join(parent_test_dir, 'extensions/extra')
     default_kwargs = Kwargs(extensions=['extra'])
 
     loose_def_list = Kwargs(extensions=['def_list'])
```

### Comparing `Markdown-3.4.3/tests/test_meta.py` & `Markdown-3.4.4/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/__init__.py` & `Markdown-3.4.4/tests/test_syntax/__init__.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/blocks/__init__.py` & `Markdown-3.4.4/tests/test_syntax/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/blocks/test_blockquotes.py` & `Markdown-3.4.4/tests/test_syntax/blocks/test_blockquotes.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/blocks/test_code_blocks.py` & `Markdown-3.4.4/tests/test_syntax/blocks/test_code_blocks.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/blocks/test_headers.py` & `Markdown-3.4.4/tests/test_syntax/blocks/test_headers.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/blocks/test_hr.py` & `Markdown-3.4.4/tests/test_syntax/blocks/test_hr.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/blocks/test_html_blocks.py` & `Markdown-3.4.4/tests/test_syntax/blocks/test_html_blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1607,13 +1607,13 @@
                 """
             )
         )
 
     def test_placeholder_in_source(self):
         # This should never occur, but third party extensions could create weird edge cases.
         md = markdown.Markdown()
-        # Ensure there is an htmlstash so relevant code (nested in `if replacements`) is run.
+        # Ensure there is an `htmlstash` so relevant code (nested in `if replacements`) is run.
         md.htmlStash.store('foo')
         # Run with a placeholder which is not in the stash
         placeholder = md.htmlStash.get_placeholder(md.htmlStash.html_counter + 1)
         result = md.postprocessors['raw_html'].run(placeholder)
         self.assertEqual(placeholder, result)
```

### Comparing `Markdown-3.4.3/tests/test_syntax/blocks/test_paragraphs.py` & `Markdown-3.4.4/tests/test_syntax/blocks/test_paragraphs.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/__init__.py` & `Markdown-3.4.4/tests/test_syntax/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_abbr.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_abbr.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_admonition.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_admonition.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_attr_list.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_attr_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from markdown.test_tools import TestCase
 
 
 class TestAttrList(TestCase):
 
     maxDiff = None
 
-    # TODO: Move the rest of the attr_list tests here.
+    # TODO: Move the rest of the `attr_list` tests here.
 
     def test_empty_list(self):
         self.assertMarkdownRenders(
             '*foo*{ }',
             '<p><em>foo</em>{ }</p>',
             extensions=['attr_list']
         )
```

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_code_hilite.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_code_hilite.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 try:
     import pygments  # noqa
     has_pygments = True
 except ImportError:
     has_pygments = False
 
-# The version required by the tests is the version specified and installed in the 'pygments' tox env.
-# In any environment where the PYGMENTS_VERSION environment variable is either not defined or doesn't
-# match the version of Pygments installed, all tests which rely in pygments will be skipped.
+# The version required by the tests is the version specified and installed in the `pygments` tox environment.
+# In any environment where the `PYGMENTS_VERSION` environment variable is either not defined or doesn't
+# match the version of Pygments installed, all tests which rely in Pygments will be skipped.
 required_pygments_version = os.environ.get('PYGMENTS_VERSION', '')
 
 
 class TestCodeHiliteClass(TestCase):
     """ Test the markdown.extensions.codehilite.CodeHilite class. """
 
     def setUp(self):
@@ -50,15 +50,15 @@
         """
 
         output = CodeHilite(source, **options).hilite()
         self.assertMultiLineEqual(output.strip(), expected)
 
     def test_codehilite_defaults(self):
         if has_pygments:
-            # Odd result as no lang given and a single comment is not enough for guessing.
+            # Odd result as no `lang` given and a single comment is not enough for guessing.
             expected = (
                 '<div class="codehilite"><pre><span></span><code><span class="err"># A Code Comment</span>\n'
                 '</code></pre></div>'
             )
         else:
             expected = (
                 '<pre class="codehilite"><code># A Code Comment\n'
@@ -94,15 +94,15 @@
                 '</code></pre>'
             )
         # This will be difficult to guess.
         self.assertOutputEquals('plain text', expected, guess_lang=True)
 
     def test_codehilite_set_lang(self):
         if has_pygments:
-            # Note an extra `<span class="x">` is added to end of code block when lang explicitly set.
+            # Note an extra `<span class="x">` is added to end of code block when `lang` explicitly set.
             # Compare with expected output for `test_guess_lang`. Not sure why this happens.
             expected = (
                 '<div class="codehilite"><pre><span></span><code><span class="cp">&lt;?php</span> '
                 '<span class="k">print</span><span class="p">(</span><span class="s2">&quot;Hello World&quot;</span>'
                 '<span class="p">);</span> <span class="cp">?&gt;</span><span class="x"></span>\n'
                 '</code></pre></div>'
             )
@@ -118,15 +118,15 @@
             expected = (
                 '<div class="codehilite"><pre><span></span><code><span class="cp">&lt;?php</span> '
                 '<span class="k">print</span><span class="p">(</span><span class="s2">'
                 '&quot;Hello World&quot;</span><span class="p">);</span> <span class="cp">?&gt;</span>\n'
                 '</code></pre></div>'
             )
         else:
-            # Note that without pygments there is no way to check that the language name is bad.
+            # Note that without Pygments there is no way to check that the language name is bad.
             expected = (
                 '<pre class="codehilite"><code class="language-unkown">'
                 '&lt;?php print(&quot;Hello World&quot;); ?&gt;\n'
                 '</code></pre>'
             )
         # The starting `<?php` tag ensures an accurate guess.
         self.assertOutputEquals('<?php print("Hello World"); ?>', expected, lang='unkown')
@@ -269,15 +269,15 @@
     def test_codehilite_linenostart(self):
         if has_pygments:
             expected = (
                 '<div class="codehilite"><pre><span></span><code><span class="linenos">42</span>plain text\n'
                 '</code></pre></div>'
             )
         else:
-            # TODO: Implement linenostart for no-pygments. Will need to check what JS libs look for.
+            # TODO: Implement `linenostart` for no-Pygments. Will need to check what JavaScript libraries look for.
             expected = (
                 '<pre class="codehilite"><code class="language-text linenums">plain text\n'
                 '</code></pre>'
             )
         self.assertOutputEquals('plain text', expected, lang='text', linenos='inline', linenostart=42)
 
     def test_codehilite_linenos_hl_lines(self):
@@ -370,15 +370,15 @@
 
         self.custom_pygments_formatter = CustomAddLangHtmlFormatter
 
     maxDiff = None
 
     def testBasicCodeHilite(self):
         if has_pygments:
-            # Odd result as no lang given and a single comment is not enough for guessing.
+            # Odd result as no `lang` given and a single comment is not enough for guessing.
             expected = (
                 '<div class="codehilite"><pre><span></span><code><span class="err"># A Code Comment</span>\n'
                 '</code></pre></div>'
             )
         else:
             expected = (
                 '<pre class="codehilite"><code># A Code Comment\n'
@@ -641,15 +641,15 @@
             ),
             expected,
             extensions=['codehilite']
         )
 
     def testUnknownOption(self):
         if has_pygments:
-            # Odd result as no lang given and a single comment is not enough for guessing.
+            # Odd result as no `lang` given and a single comment is not enough for guessing.
             expected = (
                 '<div class="codehilite"><pre><span></span><code><span class="err"># A Code Comment</span>\n'
                 '</code></pre></div>'
             )
         else:
             expected = (
                 '<pre class="codehilite"><code># A Code Comment\n'
```

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_def_list.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_def_list.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_fenced_code.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_fenced_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,17 +27,17 @@
 try:
     import pygments  # noqa
     import pygments.formatters  # noqa
     has_pygments = True
 except ImportError:
     has_pygments = False
 
-# The version required by the tests is the version specified and installed in the 'pygments' tox env.
-# In any environment where the PYGMENTS_VERSION environment variable is either not defined or doesn't
-# match the version of Pygments installed, all tests which rely in pygments will be skipped.
+# The version required by the tests is the version specified and installed in the `pygments` tox environment.
+# In any environment where the `PYGMENTS_VERSION` environment variable is either not defined or doesn't
+# match the version of Pygments installed, all tests which rely in Pygments will be skipped.
 required_pygments_version = os.environ.get('PYGMENTS_VERSION', '')
 
 
 class TestFencedCode(TestCase):
 
     def testBasicFence(self):
         self.assertMarkdownRenders(
```

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_footnotes.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_footnotes.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
             ' title="Jump back to footnote 2 in the text">&#8617;</a></p>\n'
             '</li>\n'
             '</ol>\n'
             '</div>'
         )
 
     def test_backlink_text(self):
-        """Test backlink configuration."""
+        """Test back-link configuration."""
 
         self.assertMarkdownRenders(
             'paragraph[^1]\n\n[^1]: A Footnote',
             '<p>paragraph<sup id="fnref:1"><a class="footnote-ref" href="#fn:1">1</a></sup></p>\n'
             '<div class="footnote">\n'
             '<hr />\n'
             '<ol>\n'
@@ -298,15 +298,15 @@
             '</li>\n'
             '</ol>\n'
             '</div>',
             extension_configs={'footnotes': {'SEPARATOR': '-'}}
         )
 
     def test_backlink_title(self):
-        """Test backlink title configuration without placeholder."""
+        """Test back-link title configuration without placeholder."""
 
         self.assertMarkdownRenders(
             'paragraph[^1]\n\n[^1]: A Footnote',
             '<p>paragraph<sup id="fnref:1"><a class="footnote-ref" href="#fn:1">1</a></sup></p>\n'
             '<div class="footnote">\n'
             '<hr />\n'
             '<ol>\n'
```

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_legacy_attrs.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_legacy_attrs.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_legacy_em.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_legacy_em.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_md_in_html.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_md_in_html.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 
 class TestMarkdownInHTMLPostProcessor(TestCase):
     """ Ensure any remaining elements in HTML stash are properly serialized. """
 
     def test_stash_to_string(self):
         # There should be no known cases where this actually happens so we need to
-        # forcefully pass an etree Element to the method to ensure proper behavior.
+        # forcefully pass an `etree` `Element` to the method to ensure proper behavior.
         element = Element('div')
         element.text = 'Foo bar.'
         md = Markdown(extensions=['md_in_html'])
         result = md.postprocessors['raw_html'].stash_to_string(element)
         self.assertEqual(result, '<div>Foo bar.</div>')
 
 
@@ -1204,13 +1204,13 @@
             '</ol>\n'
             '</div>',
             extensions=['md_in_html', 'footnotes']
         )
 
 
 def load_tests(loader, tests, pattern):
-    ''' Ensure TestHTMLBlocks doesn't get run twice by excluding it here. '''
+    ''' Ensure `TestHTMLBlocks` doesn't get run twice by excluding it here. '''
     suite = TestSuite()
     for test_class in [TestDefaultwMdInHTML, TestMdInHTML, TestMarkdownInHTMLPostProcessor]:
         tests = loader.loadTestsFromTestCase(test_class)
         suite.addTests(tests)
     return suite
```

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_smarty.py` & `Markdown-3.4.4/tests/test_syntax/inline/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,20 @@
-# -*- coding: utf-8 -*-
 """
 Python Markdown
 
 A Python implementation of John Gruber's Markdown.
 
 Documentation: https://python-markdown.github.io/
 GitHub: https://github.com/Python-Markdown/markdown/
 PyPI: https://pypi.org/project/Markdown/
 
 Started by Manfred Stienstra (http://www.dwerg.net/).
 Maintained for a few years by Yuri Takhteyev (http://www.freewisdom.org).
 Currently maintained by Waylan Limberg (https://github.com/waylan),
 Dmitry Shachnev (https://github.com/mitya57) and Isaac Muse (https://github.com/facelessuser).
 
-Copyright 2007-2022 The Python Markdown Project (v. 1.7 and later)
+Copyright 2007-2018 The Python Markdown Project (v. 1.7 and later)
 Copyright 2004, 2005, 2006 Yuri Takhteyev (v. 0.2-1.6b)
 Copyright 2004 Manfred Stienstra (the original version)
 
 License: BSD (see LICENSE.md for details).
 """
-
-from markdown.test_tools import TestCase
-
-
-class TestSmarty(TestCase):
-
-    default_kwargs = {'extensions': ['smarty']}
-
-    def test_escaped_attr(self):
-        self.assertMarkdownRenders(
-            '![x\"x](x)',
-            '<p><img alt="x&quot;x" src="x" /></p>'
-        )
-
-    # TODO: Move rest of smarty tests here.
```

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_tables.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from markdown.test_tools import TestCase
 from markdown.extensions.tables import TableExtension
 
 
 class TestTableBlocks(TestCase):
 
     def test_empty_cells(self):
-        """Empty cells (nbsp)."""
+        """Empty cells (`nbsp`)."""
 
         text = """
    | Second Header
 ------------- | -------------
    | Content Cell
 Content Cell  |  
 """
```

### Comparing `Markdown-3.4.3/tests/test_syntax/extensions/test_toc.py` & `Markdown-3.4.4/tests/test_syntax/extensions/test_toc.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,14 +438,31 @@
             extensions=['toc']
         )
 
     def test_escaped_char_in_id(self):
         self.assertMarkdownRenders(
             r'# escaped\_character',
             '<h1 id="escaped_character">escaped_character</h1>',
+            expected_attrs={
+                'toc': (
+                    '<div class="toc">\n'
+                      '<ul>\n'                                                           # noqa
+                        '<li><a href="#escaped_character">escaped_character</a></li>\n'  # noqa
+                      '</ul>\n'                                                          # noqa
+                    '</div>\n'                                                           # noqa
+                ),
+                'toc_tokens': [
+                    {
+                        'level': 1,
+                        'id': 'escaped_character',
+                        'name': 'escaped_character',
+                        'children': []
+                    }
+                ]
+            },
             extensions=['toc']
         )
 
     def testAnchorLinkWithCustomClass(self):
         self.assertMarkdownRenders(
             self.dedent(
                 '''
```

### Comparing `Markdown-3.4.3/tests/test_syntax/inline/test_autolinks.py` & `Markdown-3.4.4/tests/test_syntax/inline/test_autolinks.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/inline/test_emphasis.py` & `Markdown-3.4.4/tests/test_syntax/inline/test_emphasis.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/inline/test_entities.py` & `Markdown-3.4.4/tests/test_syntax/inline/test_entities.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/inline/test_images.py` & `Markdown-3.4.4/tests/test_syntax/inline/test_images.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/inline/test_links.py` & `Markdown-3.4.4/tests/test_syntax/inline/test_links.py`

 * *Files identical despite different names*

### Comparing `Markdown-3.4.3/tests/test_syntax/inline/test_raw_html.py` & `Markdown-3.4.4/tests/test_syntax/inline/test_raw_html.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,7 +24,10 @@
 
 class TestRawHtml(TestCase):
     def test_inline_html_angle_brackets(self):
         self.assertMarkdownRenders("<span>e<c</span>", "<p><span>e&lt;c</span></p>")
         self.assertMarkdownRenders("<span>e>c</span>", "<p><span>e&gt;c</span></p>")
         self.assertMarkdownRenders("<span>e < c</span>", "<p><span>e &lt; c</span></p>")
         self.assertMarkdownRenders("<span>e > c</span>", "<p><span>e &gt; c</span></p>")
+
+    def test_inline_html_backslashes(self):
+        self.assertMarkdownRenders('<img src="..\\..\\foo.png">', '<p><img src="..\\..\\foo.png"></p>')
```

