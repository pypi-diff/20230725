# Comparing `tmp/mknodes-0.4.0.tar.gz` & `tmp/mknodes-0.4.1.tar.gz`

## Comparing `mknodes-0.4.0.tar` & `mknodes-0.4.1.tar`

### file list

```diff
@@ -1,82 +1,83 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.4.0/.editorconfig
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.4.0/Makefile
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 mknodes-0.4.0/mkdocs.yml
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.4.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.4.0/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mknodes-0.4.0/docs/gen_pages.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mknodes-0.4.0/docs/gen_qt.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkadmonition.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkbinaryimage.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkblock.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkcode.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkcontainer.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkcritic.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkdiagram.py
--rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkdoc.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkdocstrings.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkimage.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mklink.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mklist.py
--rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mknav.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mknode.py
--rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkpage.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkpageinclude.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkshields.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mksnippet.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mksourceandresult.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mktabcontainer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mktable.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mktabs.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mktext.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/node.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/__linkreplacer/__init__.py
--rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/__linkreplacer/linkreplacer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/classnodes/__init__.py
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/classnodes/mkbaseclasstable.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/classnodes/mkclassdiagram.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/classnodes/mkclasspage.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/classnodes/mkclasstable.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/manual/__init__.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/manual/page_1.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/manual/page_2.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/manual/page_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/modulenodes/__init__.py
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/modulenodes/mkmodulepage.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/modulenodes/mkmoduletable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/__init__.py
--rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/classhelpers.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/connectionbuilder.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/helpers.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/inventorymanager.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/mermaid.py
--rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/noderesolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_admonition.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_block.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_classdiagram.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_docstrings.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_image.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_list.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_manual.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_markdownnode.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_modulepage.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_nav.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_page.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_tabblock.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_tabcontainer.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_text.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/SUMMARY.md
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_file.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_folder/sub_1.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_folder/sub_2.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_subnav/SUMMARY.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_subnav/subnav_page_1.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_subnav/subnav_page_2.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.4.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.4.0/LICENSE
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.4.0/README.md
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 mknodes-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 mknodes-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.4.1/.editorconfig
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.4.1/Makefile
+-rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 mknodes-0.4.1/mkdocs.yml
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.4.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.4.1/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mknodes-0.4.1/docs/gen_pages.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mknodes-0.4.1/docs/gen_qt.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkadmonition.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkbinaryimage.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkblock.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkcode.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkcontainer.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkcritic.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkdiagram.py
+-rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkdoc.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkdocstrings.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkimage.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkinstallguide.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mklink.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mklist.py
+-rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mknav.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mknode.py
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkpage.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkpageinclude.py
+-rw-r--r--   0        0        0     3509 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mkshields.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mksnippet.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mksourceandresult.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mktabcontainer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mktable.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mktabs.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/mktext.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/node.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/__linkreplacer/__init__.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/__linkreplacer/linkreplacer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/classnodes/__init__.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/classnodes/mkclassdiagram.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/classnodes/mkclasspage.py
+-rw-r--r--   0        0        0     3108 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/classnodes/mkclasstable.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/manual/__init__.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/manual/page_1.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/manual/page_2.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/manual/page_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/modulenodes/__init__.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/modulenodes/mkmodulepage.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/modulenodes/mkmoduletable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/__init__.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/classhelpers.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/connectionbuilder.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/helpers.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/inventorymanager.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/linkprovider.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/mermaid.py
+-rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.4.1/mknodes/utils/noderesolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_admonition.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_block.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_classdiagram.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_docstrings.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_image.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_list.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_manual.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_markdownnode.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_modulepage.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_nav.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_page.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_tabblock.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_tabcontainer.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/test_text.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/SUMMARY.md
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_file.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_folder/sub_1.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_folder/sub_2.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_subnav/SUMMARY.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_subnav/subnav_page_1.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.1/tests/data/nav_tree/test_subnav/subnav_page_2.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.4.1/README.md
+-rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 mknodes-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 mknodes-0.4.1/PKG-INFO
```

### Comparing `mknodes-0.4.0/.pre-commit-config.yaml` & `mknodes-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/Makefile` & `mknodes-0.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mkdocs.yml` & `mknodes-0.4.1/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -42,24 +42,25 @@
   # - navigation.sections # top-level sections are rendered as groups
 plugins:
 - search
 # - social  # this one has dependency which is not on pypi for windows. (cairocffi)
 - tags
 - section-index  # clickable sections leading to index page (https://github.com/oprypin/mkdocs-section-index)
 - glightbox  # better image support
-- macros
-- include-markdown  # include content of other markdown files
+# - macros
+# - include-markdown  # include content of other markdown files
 - literate-nav:  # move nav out of mkdocs.yml
     nav_file: SUMMARY.md
     # implicit_index: true
 # - autorefs  # allows linking to any header
 - linkreplacer  # allows linking to any markdown page
 - gen-files: # https://github.com/oprypin/mkdocs-gen-files
     scripts:
       - docs/gen_pages.py  # or any other name or path
+- coverage
 - mkdocstrings:
     default_handler: python
     handlers:
       python:
         import:
         - url: https://docs.python.org/3/objects.inv
           domains: [std, py]
```

### Comparing `mknodes-0.4.0/.github/workflows/build.yml` & `mknodes-0.4.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/.github/workflows/documentation.yml` & `mknodes-0.4.1/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/docs/gen_pages.py` & `mknodes-0.4.1/docs/gen_pages.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/docs/gen_qt.py` & `mknodes-0.4.1/docs/gen_qt.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/__init__.py` & `mknodes-0.4.1/mknodes/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from .mktabcontainer import MkTabBlock, MkTabbed
 from .mksnippet import MkSnippet
 from .mkcritic import MkCritic
 from .mksourceandresult import MkSourceAndResult
 from .mkshields import MkShields
 from .mkpage import MkPage
 from .mkpageinclude import MkPageInclude
+from .mkinstallguide import MkInstallGuide
 
 from .classnodes.mkclassdiagram import MkClassDiagram
-from .classnodes.mkbaseclasstable import MkBaseClassTable
 from .classnodes.mkclasstable import MkClassTable
 from .classnodes.mkclasspage import MkClassPage
 
 from .modulenodes.mkmoduletable import MkModuleTable
 from .modulenodes.mkmodulepage import MkModulePage
 
 
@@ -45,24 +45,24 @@
     "MkBinaryImage",
     "MkPage",
     "MkAdmonition",
     "MkDiagram",
     "MkClassDiagram",
     "ConnectionBuilder",
     "MkTable",
-    "MkBaseClassTable",
     "MkClassTable",
     "MkList",
     "MkClassPage",
     "MkModulePage",
     "MkModuleTable",
     "MkDoc",
     "MkTabBlock",
     "MkTabbed",
     "MkSourceAndResult",
     "MkSnippet",
     "MkShields",
     "MkPageInclude",
     "MkCritic",
+    "MkInstallGuide",
 ]
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `mknodes-0.4.0/mknodes/mkadmonition.py` & `mknodes-0.4.1/mknodes/mkadmonition.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkbinaryimage.py` & `mknodes-0.4.1/mknodes/mkbinaryimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkblock.py` & `mknodes-0.4.1/mknodes/mkblock.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkcode.py` & `mknodes-0.4.1/mknodes/mkcode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkcontainer.py` & `mknodes-0.4.1/mknodes/mkcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkcritic.py` & `mknodes-0.4.1/mknodes/mkcritic.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkdiagram.py` & `mknodes-0.4.1/mknodes/mkdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkdoc.py` & `mknodes-0.4.1/mknodes/mkdoc.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkdocstrings.py` & `mknodes-0.4.1/mknodes/mkdocstrings.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 import importlib
 import logging
 import os
 import types
 
 from typing import Any, Literal
 
-from mknodes import mktext
+from mknodes import mknode
 from mknodes.utils import classhelpers, helpers
 
 
 logger = logging.getLogger(__name__)
 
 
-class MkDocStrings(mktext.MkText):
+class MkDocStrings(mknode.MkNode):
     """Docstring section (powered by mkdocstrings)."""
 
     REQUIRED_PLUGINS = "mkdocstrings"
     OPTIONS_DEFAULT: dict[str, Any] = {}
 
     def __init__(
         self,
```

### Comparing `mknodes-0.4.0/mknodes/mkimage.py` & `mknodes-0.4.1/mknodes/mkimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mklink.py` & `mknodes-0.4.1/mknodes/mklink.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mklist.py` & `mknodes-0.4.1/mknodes/mklist.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mknav.py` & `mknodes-0.4.1/mknodes/mknav.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mknode.py` & `mknodes-0.4.1/mknodes/mknode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkpage.py` & `mknodes-0.4.1/mknodes/mkpage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkpageinclude.py` & `mknodes-0.4.1/mknodes/mkpageinclude.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mkshields.py` & `mknodes-0.4.1/mknodes/mkshields.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,13 +134,13 @@
             shields=["version", "status", "codecov"],
             user="phil65",
             project="mknodes",
         )
 
 
 if __name__ == "__main__":
-    mkcritic = MkShields(
+    shields = MkShields(
         shields=["version", "status", "codecov"],
         user="phil65",
         project="prettyqt",
     )
-    print(mkcritic)
+    print(shields)
```

### Comparing `mknodes-0.4.0/mknodes/mksnippet.py` & `mknodes-0.4.1/mknodes/mksnippet.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mksourceandresult.py` & `mknodes-0.4.1/mknodes/mksourceandresult.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mktabcontainer.py` & `mknodes-0.4.1/mknodes/mktabcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mktable.py` & `mknodes-0.4.1/mknodes/mktable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mktabs.py` & `mknodes-0.4.1/mknodes/mktabs.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/mktext.py` & `mknodes-0.4.1/mknodes/mktext.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/node.py` & `mknodes-0.4.1/mknodes/node.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/__linkreplacer/linkreplacer.py` & `mknodes-0.4.1/mknodes/__linkreplacer/linkreplacer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/classnodes/mkbaseclasstable.py` & `mknodes-0.4.1/mknodes/classnodes/mkclasstable.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from mknodes import mktable
 from mknodes.utils import helpers
 
 
 logger = logging.getLogger(__name__)
 
 
-class MkBaseClassTable(mktable.MkTable):
+class MkClassTable(mktable.MkTable):
     """Table showing info for a list of classes."""
 
     def __init__(
         self,
         klasses: list[type] | set[type],
         *,
         layout: Literal["compact", "extended"] = "extended",
@@ -47,17 +47,17 @@
     def __repr__(self):
         return helpers.get_repr(self, klasses=self.klasses)
 
     @staticmethod
     def examples():
         from mknodes import mknav
 
-        yield dict(klasses=[mktable.MkTable, MkBaseClassTable, mknav.MkNav])
+        yield dict(klasses=[mktable.MkTable, MkClassTable, mknav.MkNav])
         yield dict(
-            klasses=[mktable.MkTable, MkBaseClassTable, mknav.MkNav],
+            klasses=[mktable.MkTable, MkClassTable, mknav.MkNav],
             layout="extended",
         )
 
     def default_row_for_klass(self, kls: type) -> dict[str, str]:
         return dict(
             Class=helpers.link_for_class(kls),
             Module=kls.__module__,
@@ -91,9 +91,9 @@
             Children=subclass_str,
             Inherits=parent_str,
             # Description=desc,
         )
 
 
 if __name__ == "__main__":
-    table = MkBaseClassTable(klasses=[mktable.MkTable], layout="extended")
+    table = MkClassTable(klasses=[mktable.MkTable], layout="extended")
     print(table)
```

### Comparing `mknodes-0.4.0/mknodes/classnodes/mkclassdiagram.py` & `mknodes-0.4.1/mknodes/classnodes/mkclassdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/classnodes/mkclasspage.py` & `mknodes-0.4.1/mknodes/classnodes/mkclasspage.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         return diagram
 
     def _build(self):
         module_path = ".".join(self.parts).rstrip(".")
         path = f"{module_path}.{self.klass.__name__}"
         item = mkdocstrings.MkDocStrings(path, header="DocStrings")
         self.append(item)
-        if tbl := mkclasstable.MkClassTable(self.klass):
+        if tbl := mkclasstable.MkClassTable(list(self.klass.__bases__)):
             self.append(tbl)
         item = mkclassdiagram.MkClassDiagram(self.klass, header="Inheritance diagram")
         self.append(item)
 
 
 if __name__ == "__main__":
     doc = MkClassPage(MkClassPage)
```

### Comparing `mknodes-0.4.0/mknodes/manual/page_1.py` & `mknodes-0.4.1/mknodes/manual/page_1.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/manual/page_2.py` & `mknodes-0.4.1/mknodes/manual/page_2.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/manual/page_3.py` & `mknodes-0.4.1/mknodes/manual/page_3.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/modulenodes/mkmodulepage.py` & `mknodes-0.4.1/mknodes/modulenodes/mkmodulepage.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import os
 import pathlib
 import types
 
 from mknodes import mkdocstrings, mkpage
-from mknodes.classnodes import mkbaseclasstable
+from mknodes.classnodes import mkclasstable
 from mknodes.utils import classhelpers, helpers
 
 
 logger = logging.getLogger(__name__)
 
 
 class MkModulePage(mkpage.MkPage):
@@ -23,15 +23,15 @@
         show_class_table: ModuleType or path to model to show info for.
     """
 
     def __init__(
         self,
         module: tuple[str, ...] | str | types.ModuleType,
         *,
-        klasses: list[type] | set[type] = None,
+        klasses: list[type] | set[type] | None = None,
         path: str | os.PathLike = "index.md",
         docstrings: bool = False,
         show_class_table: bool = True,
         **kwargs,
     ):
         path = pathlib.Path(path)
         super().__init__(path=path, **kwargs)
@@ -56,15 +56,15 @@
     def _build(self):
         if doc := self.module.__doc__:
             self.append(doc)
         if self.docstrings:
             item = mkdocstrings.MkDocStrings(f'{".".join(self.parts)}')
             self.append(item)
         if self.show_class_table:
-            table = mkbaseclasstable.MkBaseClassTable(self.klasses)
+            table = mkclasstable.MkClassTable(self.klasses)
             self.append(table)
 
 
 if __name__ == "__main__":
     doc = MkModulePage(mkpage)
     doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
     print(doc)
```

### Comparing `mknodes-0.4.0/mknodes/modulenodes/mkmoduletable.py` & `mknodes-0.4.1/mknodes/modulenodes/mkmoduletable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/utils/classhelpers.py` & `mknodes-0.4.1/mknodes/utils/classhelpers.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/utils/connectionbuilder.py` & `mknodes-0.4.1/mknodes/utils/connectionbuilder.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/utils/helpers.py` & `mknodes-0.4.1/mknodes/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/utils/inventorymanager.py` & `mknodes-0.4.1/mknodes/utils/inventorymanager.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 
 logger = logging.getLogger(__name__)
 
 
 class InventoryManager:
     def __init__(self):
-        self.inv_files: set[inventory.Inventory] = set()
+        self.inv_files: list[inventory.Inventory] = list()
 
     def add_inv_file(self, path: str | os.PathLike):
         with pathlib.Path(path).open("rb") as file:
             inv = inventory.Inventory.parse_sphinx(file)
-        self.inv_files.add(inv)
+        self.inv_files.append(inv)
 
     def __getitem__(self, name: str | type | types.FunctionType | types.MethodType):
         match name:
             case type():
                 path = f"{name.__module__}.{name.__qualname__}"
             case str():
                 path = name
@@ -32,7 +32,10 @@
             if path in inv_file:
                 return inv_file[path]
         return None
 
 
 if __name__ == "__main__":
     inv_manager = InventoryManager()
+    inv_manager.add_inv_file("mknodes/utils/objects.inv")
+    file = inv_manager.inv_files[0]
+    print(file.keys())
```

### Comparing `mknodes-0.4.0/mknodes/utils/mermaid.py` & `mknodes-0.4.1/mknodes/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/mknodes/utils/noderesolver.py` & `mknodes-0.4.1/mknodes/utils/noderesolver.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/tests/test_nav.py` & `mknodes-0.4.1/tests/test_nav.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/tests/data/nav_tree/test_file.md` & `mknodes-0.4.1/tests/data/nav_tree/test_file.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/.gitignore` & `mknodes-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/LICENSE` & `mknodes-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/README.md` & `mknodes-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.4.0/pyproject.toml` & `mknodes-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,20 +17,22 @@
     "pytest",
     "pytest-cov",
     "mkdocs",
     "mkdocs-material",
     "mkdocstrings[python]",
     "pymdown-extensions",
     "mkdocs-literate-nav",
-    "mkdocs-include-markdown-plugin",
+    # "mkdocs-include-markdown-plugin",
     # "mkdocs-autorefs",
     "mkdocs-glightbox",
     "mkdocs-section-index",
     "mkdocs-gen-files",
-    "mkdocs-macros-plugin",
+    # "mkdocs-macros-plugin",
+    "markdown-exec[ansi]",
+    "mkdocs-coverage",
     "pygments",
     "typing_extensions",
 ]
 
 [tool.hatch.envs.default.scripts]
 test = "pytest"
 test-cov-xml = "pytest --cov-report=xml"
```

### Comparing `mknodes-0.4.0/PKG-INFO` & `mknodes-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mknodes
-Version: 0.4.0
+Version: 0.4.1
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
-Metadata-Version: 2.1 Name: mknodes Version: 0.4.0 Summary: Generate docs with
+Metadata-Version: 2.1 Name: mknodes Version: 0.4.1 Summary: Generate docs with
 ease. Project-URL: Documentation, https://phil65.github.io/mknodes/ Project-
 URL: Source, https://github.com/phil65/mknodes Author-email: mknodes
 gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
 docs,docstrings,documentation,framework,internet,markdown Classifier:
 Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

