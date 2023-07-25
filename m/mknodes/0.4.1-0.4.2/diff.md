# Comparing `tmp/mknodes-0.4.1.tar.gz` & `tmp/mknodes-0.4.2.tar.gz`

## Comparing `mknodes-0.4.1.tar` & `mknodes-0.4.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.4.1/.editorconfig
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.4.1/Makefile
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mknodes-0.4.1/mkdocs.yml
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.4.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.4.1/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mknodes-0.4.1/docs/gen_pages.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mknodes-0.4.1/docs/gen_qt.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkadmonition.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkbinaryimage.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkblock.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkcode.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkcontainer.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkcritic.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkdiagram.py
--rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkdoc.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkdocstrings.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkimage.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkinstallguide.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mklink.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mklist.py
--rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mknav.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mknode.py
--rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkpage.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkpageinclude.py
--rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkshields.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mksnippet.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mksourceandresult.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mktabcontainer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mktable.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mktabs.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mktext.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/node.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/__linkreplacer/__init__.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/__linkreplacer/linkreplacer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/classnodes/__init__.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/classnodes/mkclassdiagram.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/classnodes/mkclasspage.py
--rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/classnodes/mkclasstable.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/manual/__init__.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/manual/page_1.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/manual/page_2.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/manual/page_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/modulenodes/__init__.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/modulenodes/mkmodulepage.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/modulenodes/mkmoduletable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/__init__.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/classhelpers.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/connectionbuilder.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/helpers.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/inventorymanager.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/linkprovider.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/mermaid.py
--rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/noderesolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_admonition.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_block.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_classdiagram.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_docstrings.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_image.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_list.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_manual.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_markdownnode.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_modulepage.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_nav.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_page.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_tabblock.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_tabcontainer.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_text.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/SUMMARY.md
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_file.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_folder/sub_1.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_folder/sub_2.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_subnav/SUMMARY.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_subnav/subnav_page_1.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_subnav/subnav_page_2.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.4.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.4.1/LICENSE
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.4.1/README.md
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 mknodes-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 mknodes-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.4.2/.editorconfig
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.4.2/Makefile
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mknodes-0.4.2/mkdocs.yml
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.4.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.4.2/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mknodes-0.4.2/docs/gen_pages.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mknodes-0.4.2/docs/gen_qt.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkadmonition.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkbinaryimage.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkblock.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkcode.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkcontainer.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkcritic.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkdiagram.py
+-rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkdoc.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkdocstrings.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkimage.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkinstallguide.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mklink.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mklist.py
+-rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mknav.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mknode.py
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkpage.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkpageinclude.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mkshields.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mksnippet.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mksourceandresult.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mktabcontainer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mktable.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mktabs.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/mktext.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/node.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/__linkreplacer/__init__.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/__linkreplacer/linkreplacer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/classnodes/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/classnodes/mkclassdiagram.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/classnodes/mkclasspage.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/classnodes/mkclasstable.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/manual/__init__.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/manual/page_1.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/manual/page_2.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/manual/page_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/modulenodes/__init__.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/modulenodes/mkmodulepage.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/modulenodes/mkmoduletable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/__init__.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/classhelpers.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/connectionbuilder.py
+-rw-r--r--   0        0        0     6573 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/helpers.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/inventorymanager.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/linkprovider.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/mermaid.py
+-rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.4.2/mknodes/utils/noderesolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/conftest.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_admonition.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_block.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_classdiagram.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_docstrings.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_image.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_list.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_manual.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_markdownnode.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_modulepage.py
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_nav.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_page.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_tabblock.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_tabcontainer.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/test_text.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/SUMMARY.md
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_file.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_folder/sub_1.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_folder/sub_2.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_subnav/SUMMARY.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_subnav/subnav_page_1.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.2/tests/data/nav_tree/test_subnav/subnav_page_2.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.4.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.4.2/README.md
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 mknodes-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 mknodes-0.4.2/PKG-INFO
```

### Comparing `mknodes-0.4.1/.pre-commit-config.yaml` & `mknodes-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/Makefile` & `mknodes-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mkdocs.yml` & `mknodes-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/.github/workflows/build.yml` & `mknodes-0.4.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/.github/workflows/documentation.yml` & `mknodes-0.4.2/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/docs/gen_pages.py` & `mknodes-0.4.2/docs/gen_pages.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/docs/gen_qt.py` & `mknodes-0.4.2/docs/gen_qt.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/__init__.py` & `mknodes-0.4.2/mknodes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,8 +61,8 @@
     "MkSnippet",
     "MkShields",
     "MkPageInclude",
     "MkCritic",
     "MkInstallGuide",
 ]
 
-__version__ = "0.4.1"
+__version__ = "0.4.2"
```

### Comparing `mknodes-0.4.1/mknodes/mkadmonition.py` & `mknodes-0.4.2/mknodes/mkadmonition.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkbinaryimage.py` & `mknodes-0.4.2/mknodes/mkbinaryimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkblock.py` & `mknodes-0.4.2/mknodes/mkblock.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkcode.py` & `mknodes-0.4.2/mknodes/mkcode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkcontainer.py` & `mknodes-0.4.2/mknodes/mkcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkcritic.py` & `mknodes-0.4.2/mknodes/mkcritic.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkdiagram.py` & `mknodes-0.4.2/mknodes/mkdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkdoc.py` & `mknodes-0.4.2/mknodes/mkdoc.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkdocstrings.py` & `mknodes-0.4.2/mknodes/mkdocstrings.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkimage.py` & `mknodes-0.4.2/mknodes/mkimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkinstallguide.py` & `mknodes-0.4.2/mknodes/mkinstallguide.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mklink.py` & `mknodes-0.4.2/mknodes/mklink.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mklist.py` & `mknodes-0.4.2/mknodes/mklist.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mknav.py` & `mknodes-0.4.2/mknodes/mknav.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,16 +190,18 @@
             case MkNav():
                 self.nav[(node.section,)] = node
             case mkpage.MkPage():
                 self.nav[node.path.removesuffix(".md")] = node
 
     @classmethod
     def from_file(cls, path: str | os.PathLike, section: str | None):
-        content = pathlib.Path(path).read_text()
-        return cls.from_text(content, section)
+        path = pathlib.Path(path)
+        content = path.read_text()
+        with helpers.new_cd(path.parent):
+            return cls.from_text(content, section)
         # max_indent = max(len(line) - len(line.lstrip()) for line in content.split("\n"))
         # content = [line.lstrip() for line in content.split("\n")]
 
     @classmethod
     def from_text(cls, text: str, section: str | None):
         nav = cls(section)
         lines = text.split("\n")
@@ -207,15 +209,15 @@
             if match := re.match(r"\* \[(.*)\]\((.*\.md)\)", line):
                 title = match[1]
                 file_path = pathlib.Path(match[2])
                 text = file_path.read_text()
                 node = mktext.MkText(text)
                 nav[title] = mkpage.MkPage(items=[node], path=file_path.name)
             elif match := re.match(r"\* \[(.*)\]\((.*)\/\)", line):
-                subnav = MkNav(match[1])
+                subnav = MkNav.from_file(f"{match[2]}/SUMMARY.md", section=match[1])
                 title = match[1]
                 nav[title] = subnav
             elif match := re.match(r"\* (.*)", line):
                 subnav_lines = []
                 for subline in lines[i + 1 :]:
                     if subline.startswith("    "):
                         subnav_lines.append(subline[4:])
@@ -225,30 +227,38 @@
                 title = match[1]
                 nav[title] = subnav
         return nav
 
     @classmethod
     def from_folder(cls, folder: str | os.PathLike, parent=None) -> Self:
         folder = pathlib.Path(folder)
-        nav = cls(folder.name, parent=parent)
+        nav = cls(folder.name if parent else None, parent=parent)
         for path in folder.iterdir():
             if path.is_dir():
                 subnav = cls.from_folder(folder / path.parts[-1], parent=nav)
                 nav._register(subnav)
-            elif path.suffix == ".md":
-                page = mkpage.MkPage(path)
+            elif path.suffix == ".md" and path.name != "SUMMARY.md":
+                page = mkpage.MkPage(path.relative_to(folder))
+                text = path.read_text()
+                page += text
                 nav._register(page)
         return nav
 
 
 if __name__ == "__main__":
     docs = MkNav()
-    nav_file = pathlib.Path(__file__).parent / "SUMMARY.md"
+    nav_tree_path = pathlib.Path(__file__).parent.parent / "tests/data/nav_tree/"
+    nav_file = nav_tree_path / "SUMMARY.md"
     # print(pathlib.Path(nav_file).read_text())
-    nav = MkNav.from_file(pathlib.Path(__file__).parent / "SUMMARY.md", None)
+    nav = MkNav.from_folder(nav_tree_path, None)
+    lines = [f"{level * '    '} {node!r}" for level, node in nav.iter_nodes()]
+    print("\n".join(lines))
+
+    # print(nav.all_virtual_files())
+    nav = MkNav.from_file(nav_file, None)
     lines = [f"{level * '    '} {node!r}" for level, node in nav.iter_nodes()]
     print("\n".join(lines))
     # print(nav_file.read_text())
     # subnav = docs.add_nav("subnav")
     # page = subnav.add_page("My first page!")
     # page.add_admonition("Warning This is still beta", typ="danger", title="Warning!")
     # page2 = subnav.add_page("And a second one")
```

### Comparing `mknodes-0.4.1/mknodes/mknode.py` & `mknodes-0.4.2/mknodes/mknode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkpage.py` & `mknodes-0.4.2/mknodes/mkpage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkpageinclude.py` & `mknodes-0.4.2/mknodes/mkpageinclude.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mkshields.py` & `mknodes-0.4.2/mknodes/mkshields.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mksnippet.py` & `mknodes-0.4.2/mknodes/mksnippet.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mksourceandresult.py` & `mknodes-0.4.2/mknodes/mksourceandresult.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mktabcontainer.py` & `mknodes-0.4.2/mknodes/mktabcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mktable.py` & `mknodes-0.4.2/mknodes/mktable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mktabs.py` & `mknodes-0.4.2/mknodes/mktabs.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/mktext.py` & `mknodes-0.4.2/mknodes/mktext.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/node.py` & `mknodes-0.4.2/mknodes/node.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/__linkreplacer/linkreplacer.py` & `mknodes-0.4.2/mknodes/__linkreplacer/linkreplacer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/classnodes/mkclassdiagram.py` & `mknodes-0.4.2/mknodes/classnodes/mkclassdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/classnodes/mkclasspage.py` & `mknodes-0.4.2/mknodes/classnodes/mkclasspage.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,19 +65,19 @@
         diagram = mkclassdiagram.MkClassDiagram(self.klass, mode=mode)
         self.append(diagram)
         return diagram
 
     def _build(self):
         module_path = ".".join(self.parts).rstrip(".")
         path = f"{module_path}.{self.klass.__name__}"
-        item = mkdocstrings.MkDocStrings(path, header="DocStrings")
+        item = mkdocstrings.MkDocStrings(path, header="⁇ DocStrings")
         self.append(item)
         if tbl := mkclasstable.MkClassTable(list(self.klass.__bases__)):
             self.append(tbl)
-        item = mkclassdiagram.MkClassDiagram(self.klass, header="Inheritance diagram")
+        item = mkclassdiagram.MkClassDiagram(self.klass, header="⋔ Inheritance diagram")
         self.append(item)
 
 
 if __name__ == "__main__":
     doc = MkClassPage(MkClassPage)
     doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
     print(doc)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mknodes-0.4.1/mknodes/classnodes/mkclasstable.py` & `mknodes-0.4.2/mknodes/classnodes/mkclasstable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/manual/page_1.py` & `mknodes-0.4.2/mknodes/manual/page_1.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/manual/page_2.py` & `mknodes-0.4.2/mknodes/manual/page_2.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/manual/page_3.py` & `mknodes-0.4.2/mknodes/manual/page_3.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/modulenodes/mkmodulepage.py` & `mknodes-0.4.2/mknodes/modulenodes/mkmodulepage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/modulenodes/mkmoduletable.py` & `mknodes-0.4.2/mknodes/modulenodes/mkmoduletable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/utils/classhelpers.py` & `mknodes-0.4.2/mknodes/utils/classhelpers.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/utils/connectionbuilder.py` & `mknodes-0.4.2/mknodes/utils/connectionbuilder.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/utils/helpers.py` & `mknodes-0.4.2/mknodes/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from __future__ import annotations
 
 from collections.abc import Callable
+import contextlib
+
 from importlib import metadata
 import inspect
 import itertools
 import logging
+import os
 import re
 import reprlib
 import sys
 import types
-
 from typing import Any
 
 
 logger = logging.getLogger(__name__)
 
 BASE_URL = "https://doc.qt.io/qtforpython-6/PySide6/"
 BUILTIN_URL = "https://docs.python.org/3/library/{mod}.html#{name}"
@@ -24,14 +26,22 @@
 
 
 limit_repr = LengthLimitRepr()
 limit_repr.maxlist = 10
 limit_repr.maxstring = 80
 
 
+@contextlib.contextmanager
+def new_cd(x):
+    d = os.getcwd()  # noqa: PTH109
+    os.chdir(x)
+    yield
+    os.chdir(d)
+
+
 def get_repr(_obj: Any, *args: Any, _shorten: bool = True, **kwargs: Any) -> str:
     """Get a suitable __repr__ string for an object.
 
     Args:
         _obj: The object to get a repr for.
         _shorten: Whether to shorten the repr.
         *args: Arguments for the repr
```

### Comparing `mknodes-0.4.1/mknodes/utils/inventorymanager.py` & `mknodes-0.4.2/mknodes/utils/inventorymanager.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 class InventoryManager:
     def __init__(self):
-        self.inv_files: list[inventory.Inventory] = list()
+        self.inv_files: list[inventory.Inventory] = []
 
     def add_inv_file(self, path: str | os.PathLike):
         with pathlib.Path(path).open("rb") as file:
             inv = inventory.Inventory.parse_sphinx(file)
         self.inv_files.append(inv)
 
     def __getitem__(self, name: str | type | types.FunctionType | types.MethodType):
```

### Comparing `mknodes-0.4.1/mknodes/utils/linkprovider.py` & `mknodes-0.4.2/mknodes/utils/linkprovider.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/utils/mermaid.py` & `mknodes-0.4.2/mknodes/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/mknodes/utils/noderesolver.py` & `mknodes-0.4.2/mknodes/utils/noderesolver.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/tests/data/nav_tree/test_file.md` & `mknodes-0.4.2/tests/data/nav_tree/test_file.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/.gitignore` & `mknodes-0.4.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/LICENSE` & `mknodes-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/README.md` & `mknodes-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/pyproject.toml` & `mknodes-0.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.1/PKG-INFO` & `mknodes-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknodes
-Version: 0.4.1
+Version: 0.4.2
 Summary: Generate docs with ease.
 Project-URL: Documentation, https://phil65.github.io/mknodes/
 Project-URL: Source, https://github.com/phil65/mknodes
 Author-email: mknodes <philipptemminghoff@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: docs,docstrings,documentation,framework,internet,markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mknodes Version: 0.4.1 Summary: Generate docs with
+Metadata-Version: 2.1 Name: mknodes Version: 0.4.2 Summary: Generate docs with
 ease. Project-URL: Documentation, https://phil65.github.io/mknodes/ Project-
 URL: Source, https://github.com/phil65/mknodes Author-email: mknodes
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 docs,docstrings,documentation,framework,internet,markdown Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

