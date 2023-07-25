# Comparing `tmp/mknodes-0.3.2.tar.gz` & `tmp/mknodes-0.4.0.tar.gz`

## Comparing `mknodes-0.3.2.tar` & `mknodes-0.4.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.3.2/.editorconfig
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.3.2/Makefile
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 mknodes-0.3.2/mkdocs.yml
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.3.2/.github/workflows/build.yml
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.3.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 mknodes-0.3.2/docs/gen_pages.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mknodes-0.3.2/docs/gen_qt.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/__init__.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkadmonition.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkbinaryimage.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkblock.py
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkcode.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkcontainer.py
--rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkcritic.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkdiagram.py
--rw-r--r--   0        0        0    10465 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkdoc.py
--rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkdocstrings.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkimage.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mklink.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mklist.py
--rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mknav.py
--rw-r--r--   0        0        0     4797 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mknode.py
--rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkpage.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkpageinclude.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mkshields.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mksnippet.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mksourceandresult.py
--rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mktabcontainer.py
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mktable.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mktabs.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/mktext.py
--rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/node.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/__linkreplacer/__init__.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/__linkreplacer/linkreplacer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/classnodes/__init__.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/classnodes/mkbaseclasstable.py
--rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/classnodes/mkclassdiagram.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/classnodes/mkclasspage.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/classnodes/mkclasstable.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/manual/__init__.py
--rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/manual/page_1.py
--rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/manual/page_2.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/manual/page_3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/modulenodes/__init__.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/modulenodes/mkmodulepage.py
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/modulenodes/mkmoduletable.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/__init__.py
--rw-r--r--   0        0        0     5869 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/classhelpers.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/connectionbuilder.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/helpers.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/inventorymanager.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/mermaid.py
--rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.3.2/mknodes/utils/noderesolver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_admonition.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_block.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_classdiagram.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_docstrings.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_image.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_list.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_manual.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_markdownnode.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_modulepage.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_nav.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_page.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_tabblock.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_tabcontainer.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/test_text.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/SUMMARY.md
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_file.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_folder/sub_1.md
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_folder/sub_2.md
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_subnav/SUMMARY.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_subnav/subnav_page_1.md
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.3.2/tests/data/nav_tree/test_subnav/subnav_page_2.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.3.2/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.3.2/LICENSE
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.3.2/README.md
--rw-r--r--   0        0        0     6269 2020-02-02 00:00:00.000000 mknodes-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 mknodes-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 mknodes-0.4.0/.editorconfig
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 mknodes-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 mknodes-0.4.0/Makefile
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 mknodes-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 mknodes-0.4.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 mknodes-0.4.0/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 mknodes-0.4.0/docs/gen_pages.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mknodes-0.4.0/docs/gen_qt.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/__init__.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkadmonition.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkbinaryimage.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkblock.py
+-rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkcode.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkcontainer.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkcritic.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkdiagram.py
+-rw-r--r--   0        0        0    10727 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkdoc.py
+-rw-r--r--   0        0        0     9048 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkdocstrings.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkimage.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mklink.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mklist.py
+-rw-r--r--   0        0        0     8484 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mknav.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mknode.py
+-rw-r--r--   0        0        0    12118 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkpage.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkpageinclude.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mkshields.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mksnippet.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mksourceandresult.py
+-rw-r--r--   0        0        0     3932 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mktabcontainer.py
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mktable.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mktabs.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/mktext.py
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/node.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/__linkreplacer/__init__.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/__linkreplacer/linkreplacer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/classnodes/__init__.py
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/classnodes/mkbaseclasstable.py
+-rw-r--r--   0        0        0     3423 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/classnodes/mkclassdiagram.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/classnodes/mkclasspage.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/classnodes/mkclasstable.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/manual/__init__.py
+-rw-r--r--   0        0        0     2738 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/manual/page_1.py
+-rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/manual/page_2.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/manual/page_3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/modulenodes/__init__.py
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/modulenodes/mkmodulepage.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/modulenodes/mkmoduletable.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/__init__.py
+-rw-r--r--   0        0        0     5874 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/classhelpers.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/connectionbuilder.py
+-rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/helpers.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/inventorymanager.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/mermaid.py
+-rw-r--r--   0        0        0    10753 2020-02-02 00:00:00.000000 mknodes-0.4.0/mknodes/utils/noderesolver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/conftest.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_admonition.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_block.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_classdiagram.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_docstrings.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_image.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_list.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_manual.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_markdownnode.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_modulepage.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_nav.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_page.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_tabblock.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_tabcontainer.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/test_text.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/SUMMARY.md
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_file.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_folder/sub_1.md
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_folder/sub_2.md
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_subnav/SUMMARY.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_subnav/subnav_page_1.md
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mknodes-0.4.0/tests/data/nav_tree/test_subnav/subnav_page_2.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mknodes-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mknodes-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 mknodes-0.4.0/README.md
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 mknodes-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 mknodes-0.4.0/PKG-INFO
```

### Comparing `mknodes-0.3.2/.pre-commit-config.yaml` & `mknodes-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/Makefile` & `mknodes-0.4.0/Makefile`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mkdocs.yml` & `mknodes-0.4.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/.github/workflows/build.yml` & `mknodes-0.4.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/.github/workflows/documentation.yml` & `mknodes-0.4.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/docs/gen_pages.py` & `mknodes-0.4.0/docs/gen_pages.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 HEADER = "Don't write docs. Code them."
 WARNING = "This is all very alpha and subject to change."
 FOOTER = """Thats it. We created a website without touching any .md file
 and without having to care about file paths at at all.
 Now check out what we have created!
 """
 
-# this Nav object is basically the root of everything. It corresponds tou your root
+# this Nav object is basically the root of everything. It corresponds to your root
 # SUMMARY.md.
 
 root_nav = mknodes.MkNav()
 
 # Let's begin with the start page. This is your index.md file.
 page = root_nav.add_index_page(hide_toc=True, hide_nav=True)
```

### Comparing `mknodes-0.3.2/docs/gen_qt.py` & `mknodes-0.4.0/docs/gen_qt.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,24 +9,20 @@
 
 QT_MODULE_ATTR = "QT_MODULE"
 
 root_nav = mknodes.MkNav()
 page = root_nav.add_index_page(hide_toc=True, hide_nav=True)
 page.add_header("Not in the mood to write documentation? Let´s code it then!", level=3)
 
-qt_docs = root_nav.add_doc(prettyqt, section_name="Qt modules")
-extra_docs = root_nav.add_doc(prettyqt, section_name="Additional modules")
+qt_docs = root_nav.add_doc(prettyqt, section_name="qt_modules")
+extra_docs = root_nav.add_doc(prettyqt, section_name="additional_modules")
 
 for submod in qt_docs.iter_modules(predicate=lambda x: hasattr(x, QT_MODULE_ATTR)):
-    subdoc = qt_docs.add_doc(submod)
-    subdoc.add_module_overview()
-    for klass in subdoc.iter_classes():
-        subdoc.add_class_page(klass=klass, flatten=True)
+    subdoc = qt_docs.add_doc(submod, flatten_nav=True)
+    subdoc.collect_classes()
 for submod in extra_docs.iter_modules(predicate=lambda x: not hasattr(x, QT_MODULE_ATTR)):
-    subdoc = extra_docs.add_doc(submod)
-    subdoc.add_module_overview()
-    for klass in subdoc.iter_classes():
-        subdoc.add_class_page(klass=klass, flatten=True)
+    subdoc = extra_docs.add_doc(submod, flatten_nav=True)
+    subdoc.collect_classes()
 
 
 # root_nav.pretty_print()
 root_nav.write()  # Finally, we write the whole tree.
```

### Comparing `mknodes-0.3.2/mknodes/__init__.py` & `mknodes-0.4.0/mknodes/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,8 +61,8 @@
     "MkSourceAndResult",
     "MkSnippet",
     "MkShields",
     "MkPageInclude",
     "MkCritic",
 ]
 
-__version__ = "0.3.2"
+__version__ = "0.4.0"
```

### Comparing `mknodes-0.3.2/mknodes/mkadmonition.py` & `mknodes-0.4.0/mknodes/mkadmonition.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mkbinaryimage.py` & `mknodes-0.4.0/mknodes/mkbinaryimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mkblock.py` & `mknodes-0.4.0/mknodes/mkblock.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mkcode.py` & `mknodes-0.4.0/mknodes/mkcode.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mkcontainer.py` & `mknodes-0.4.0/mknodes/mkcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mkcritic.py` & `mknodes-0.4.0/mknodes/mkcritic.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mkdiagram.py` & `mknodes-0.4.0/mknodes/mkdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mkdoc.py` & `mknodes-0.4.0/mknodes/mkdoc.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     """Nav for showing a module documenation.
 
     Arguments:
         module: Module to document
         filter_by___all__: Whether to filter stuff according to "__all__"
         exclude_modules: List of modules to exclude
         section_name: Optional section name override
+        class_page: Override for the default ClassPage
+                    (default: [MkClassPage](MkClassPage.md))
+        flatten_nav: Whether classes should be put into top-level of the nav
     """
 
     def __init__(
         self,
         module: types.ModuleType | Sequence[str] | str,
         *,
         filter_by___all__: bool = False,
@@ -61,14 +64,15 @@
             self,
             module=self.module_name,
             section=self.section or "<root>",
             filename=self.filename,
         )
 
     def to_markdown(self) -> str:
+        self.add_module_overview()
         for klass in self.klasses:
             self.add_class_page(klass=klass, flatten=self.flatten_nav)
         for submod in self.submodules:
             self.add_doc(submod, class_page=self.ClassPage, flatten_nav=self.flatten_nav)
         return super().to_markdown()
 
     def collect_classes(
@@ -230,14 +234,15 @@
         """
         # TODO: slugify?
         path = pathlib.Path("index.md" if title is None else f"{title}.md")
         # parts = path.parts[:-1]
         page = mkmodulepage.MkModulePage(
             hide_toc=True,
             module=self.module,
+            klasses=self.klasses,
             path=path,
             parent=self,
             **kwargs,
         )
         self.nav[title or self.module_name] = page
         return page
```

### Comparing `mknodes-0.3.2/mknodes/mkdocstrings.py` & `mknodes-0.4.0/mknodes/mkdocstrings.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mkimage.py` & `mknodes-0.4.0/mknodes/mkimage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mklink.py` & `mknodes-0.4.0/mknodes/mklink.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mklist.py` & `mknodes-0.4.0/mknodes/mklist.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mknav.py` & `mknodes-0.4.0/mknodes/mknav.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mknode.py` & `mknodes-0.4.0/mknodes/mknode.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,14 +82,15 @@
 
         This can be overridden by nodes if they want files to be included in the build.
         """
         return {}
 
     @property
     def resolved_virtual_files(self) -> dict[str, str | bytes]:
+        """Return a dict containing all virtual files with resolved file paths."""
         from mknodes import mknav
 
         sections = [i.section for i in self.ancestors if isinstance(i, mknav.MkNav)]
         section = "/".join(i for i in reversed(sections) if i is not None)
         if section:
             section += "/"
         return {f"{section}{k}": v for k, v in self.virtual_files().items()}
@@ -105,14 +106,19 @@
         for des in self.descendants:
             all_files |= des.resolved_virtual_files
         if not only_children:
             all_files |= self.resolved_virtual_files
         return all_files
 
     def write(self, only_children: bool = False):
+        """Write files to virtual folder.
+
+        Arguments:
+            only_children: Whether to exclude self for data.
+        """
         # path = pathlib.Path(self.path)
         # path.parent.mkdir(parents=True, exist_ok=True)
         for k, v in self.all_virtual_files(only_children=only_children).items():
             logger.info("Written file to %s", k)
             mode = "w" if isinstance(v, str) else "wb"
             with mkdocs_gen_files.open(k, mode) as file:
                 file.write(v)
```

### Comparing `mknodes-0.3.2/mknodes/mkpage.py` & `mknodes-0.4.0/mknodes/mkpage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mkpageinclude.py` & `mknodes-0.4.0/mknodes/mkpageinclude.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mkshields.py` & `mknodes-0.4.0/mknodes/mkshields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import dataclasses
 import logging
 
 from typing import Literal
 
-from mknodes import mktext
+from mknodes import mknode
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class Shield:
@@ -99,15 +99,15 @@
     "black",
     "pyup",
     "code_triage",
     "license",
 ]
 
 
-class MkShields(mktext.MkText):
+class MkShields(mknode.MkNode):
     """MkCritic block."""
 
     def __init__(
         self,
         shields: list[ShieldTypeStr],
         user: str,
         project: str,
```

### Comparing `mknodes-0.3.2/mknodes/mksnippet.py` & `mknodes-0.4.0/mknodes/mksnippet.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mksourceandresult.py` & `mknodes-0.4.0/mknodes/mksourceandresult.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mktabcontainer.py` & `mknodes-0.4.0/mknodes/mktabcontainer.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mktable.py` & `mknodes-0.4.0/mknodes/mktable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mktabs.py` & `mknodes-0.4.0/mknodes/mktabs.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/mktext.py` & `mknodes-0.4.0/mknodes/mktext.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/node.py` & `mknodes-0.4.0/mknodes/node.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/__linkreplacer/linkreplacer.py` & `mknodes-0.4.0/mknodes/__linkreplacer/linkreplacer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from __future__ import annotations
 
 import collections
 import logging
 import os
 import pathlib
 import re
+
+from typing import TYPE_CHECKING
 import urllib.parse
 
 from mkdocs.plugins import BasePlugin
 import mkdocs.utils
 
 
+if TYPE_CHECKING:
+    from mkdocs.config.defaults import MkDocsConfig
+    from mkdocs.structure.files import Files
+    from mkdocs.structure.pages import Page
+
 logger = logging.getLogger(f"mkdocs.plugins.{__name__}")
 logger.addFilter(mkdocs.utils.warning_filter)
 
 # For Regex, match groups are:
 #       0: Whole markdown link e.g. [Alt-text](url)
 #       1: Alt text
 #       2: Full URL e.g. url + hash anchor
@@ -60,16 +67,25 @@
             match.group(3),
             rel_link_url,
         )
         return new_text
 
 
 class LinkReplacerPlugin(BasePlugin):
-    def on_page_markdown(self, markdown, page, config, files, **kwargs):
+    def on_page_markdown(
+        self,
+        markdown: str,
+        *,
+        page: Page,
+        config: MkDocsConfig,
+        files: Files,
+    ) -> str | None:
         base_docs_url = config["docs_dir"]
         page_url = page.file.src_path
         mapping = collections.defaultdict(list)
         for file_ in files:
             filename = os.path.basename(file_.abs_src_path)  # noqa: PTH119
             mapping[filename].append(file_.url)
+        #     print(file_.url, file_.dest_uri)
+        # raise ValueError
         plugin = AutoLinkReplacerPlugin(base_docs_url, page_url, mapping)
         return re.sub(AUTOLINK_RE, plugin, markdown)
```

### Comparing `mknodes-0.3.2/mknodes/classnodes/mkbaseclasstable.py` & `mknodes-0.4.0/mknodes/classnodes/mkbaseclasstable.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class MkBaseClassTable(mktable.MkTable):
     """Table showing info for a list of classes."""
 
     def __init__(
         self,
-        klasses: list[type],
+        klasses: list[type] | set[type],
         *,
         layout: Literal["compact", "extended"] = "extended",
         filter_fn: Callable | None = None,
         **kwargs,
     ):
         self.klasses = klasses
         if filter_fn is None:
```

### Comparing `mknodes-0.3.2/mknodes/classnodes/mkclassdiagram.py` & `mknodes-0.4.0/mknodes/classnodes/mkclassdiagram.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/classnodes/mkclasspage.py` & `mknodes-0.4.0/mknodes/classnodes/mkclasspage.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/classnodes/mkclasstable.py` & `mknodes-0.4.0/mknodes/classnodes/mkclasstable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/manual/page_1.py` & `mknodes-0.4.0/mknodes/manual/page_1.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/manual/page_2.py` & `mknodes-0.4.0/mknodes/manual/page_2.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,17 +19,14 @@
     # we are here right now.
     overview.add_code(inspect.getsource(create_page_2))
 
     # lets create the complete documentation for our module.
     # Each Documentation section can have global filters for what it should include.
     # In this case, we only want to document stuff which is listed in "__all__".
     mknodes_docs = doc_section.add_doc(module=mknodes, filter_by___all__=True)
-    # we start by adding a nice overview page. This might gain some kwargs for different
-    # styles in the future.
-    mknodes_docs.add_module_overview()
 
     # the Documentation Nav hast some helper methods to iterate through the submodules
     # / classes of a module. We can also pass a predicate to filter specific subclasses,
     # or do other fancy stuff to generate a customized, automated documentation.
     # now we add some pre-defined pages ("MkClassPages") to our docs.
     # they contain MkDocStrings, a table for eventual subclasses and an
     # inheritance graph. It`s also possible to build custom pages of course.
@@ -37,15 +34,14 @@
 
     # Not enough documentation for your taste? Let`s document random stuff.
     # What about the std library?
     std_lib_nav = doc_section.add_nav("std_library")
     for stdlib_mod in ["pathlib", "inspect", "logging"]:
         docs = std_lib_nav.add_doc(module=stdlib_mod)
         docs.collect_classes(recursive=True)
-        docs.add_module_overview()
 
     overview.add_admonition(text="That was easy, right?")
 
 
 if __name__ == "__main__":
     nav = mknodes.MkNav()
     create_page_2(nav)
```

### Comparing `mknodes-0.3.2/mknodes/manual/page_3.py` & `mknodes-0.4.0/mknodes/manual/page_3.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/modulenodes/mkmodulepage.py` & `mknodes-0.4.0/mknodes/modulenodes/mkmodulepage.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,24 +23,28 @@
         show_class_table: ModuleType or path to model to show info for.
     """
 
     def __init__(
         self,
         module: tuple[str, ...] | str | types.ModuleType,
         *,
+        klasses: list[type] | set[type] = None,
         path: str | os.PathLike = "index.md",
         docstrings: bool = False,
         show_class_table: bool = True,
         **kwargs,
     ):
         path = pathlib.Path(path)
         super().__init__(path=path, **kwargs)
         self.parts = classhelpers.to_module_parts(module)
         self.module = classhelpers.to_module(module)
         self.docstrings = docstrings
+        self.klasses = klasses or list(
+            classhelpers.iter_classes(module=self.parts, module_filter=self.parts[0]),
+        )
         self.show_class_table = show_class_table
         self._build()
 
     def __repr__(self):
         return helpers.get_repr(self, module=self.module, path=str(self.path))
 
     @staticmethod
@@ -52,18 +56,15 @@
     def _build(self):
         if doc := self.module.__doc__:
             self.append(doc)
         if self.docstrings:
             item = mkdocstrings.MkDocStrings(f'{".".join(self.parts)}')
             self.append(item)
         if self.show_class_table:
-            klasses = list(
-                classhelpers.iter_classes(module=self.parts, module_filter=self.parts[0]),
-            )
-            table = mkbaseclasstable.MkBaseClassTable(klasses)
+            table = mkbaseclasstable.MkBaseClassTable(self.klasses)
             self.append(table)
 
 
 if __name__ == "__main__":
     doc = MkModulePage(mkpage)
     doc.add_admonition("Warning. This is still beta", typ="danger", title="Warning")
     print(doc)
```

### Comparing `mknodes-0.3.2/mknodes/modulenodes/mkmoduletable.py` & `mknodes-0.4.0/mknodes/modulenodes/mkmoduletable.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/utils/classhelpers.py` & `mknodes-0.4.0/mknodes/utils/classhelpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         case pathlib.Path() if not module.is_absolute():
             return module.parts
         case _:
             raise TypeError(module)
 
 
 def iter_classes(
-    module: types.ModuleType | str | tuple[str],
+    module: types.ModuleType | str | tuple[str, ...],
     *,
     type_filter: type | None | types.UnionType = None,
     module_filter: str | None = None,
     filter_by___all__: bool = False,
     recursive: bool = False,
 ) -> Iterator[type]:
     """Yield classes from given module.
```

### Comparing `mknodes-0.3.2/mknodes/utils/connectionbuilder.py` & `mknodes-0.4.0/mknodes/utils/connectionbuilder.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/utils/helpers.py` & `mknodes-0.4.0/mknodes/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/utils/inventorymanager.py` & `mknodes-0.4.0/mknodes/utils/inventorymanager.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/utils/mermaid.py` & `mknodes-0.4.0/mknodes/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/mknodes/utils/noderesolver.py` & `mknodes-0.4.0/mknodes/utils/noderesolver.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/tests/test_nav.py` & `mknodes-0.4.0/tests/test_nav.py`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/tests/data/nav_tree/test_file.md` & `mknodes-0.4.0/tests/data/nav_tree/test_file.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/.gitignore` & `mknodes-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/LICENSE` & `mknodes-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/README.md` & `mknodes-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mknodes-0.3.2/pyproject.toml` & `mknodes-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 allow-direct-references = true
 
 [tool.hatch.version]
 source = "regex_commit"
 commit_extra_args = ["-e"]
 path = "mknodes/__init__.py"
 
-[project.entry-points."mkdocs.plugins"]
-linkreplacer = "mknodes.__linkreplacer:LinkReplacerPlugin"
-
 [tool.hatch.envs.default]
 python = "3.10"
 dependencies = [
     "black",
     "mypy",
     "ruff",
     "pytest",
@@ -59,22 +56,46 @@
 authors = [
   { name = "mknodes", email = "philipptemminghoff@gmail.com" }
 ]
 description = "Generate docs with ease."
 readme = "README.md"
 dynamic = ["version"]
 classifiers = [
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Documentation",
+    "Topic :: Internet",
+    "Topic :: Text Processing :: Markup :: Markdown",
+]
+keywords = [
+    "framework",
+    "docs",
+    "docstrings",
+    "documentation",
+    "internet",
+    "markdown",
 ]
+
 requires-python = ">=3.10"
 dependencies = [
     "typing_extensions",
     "mkdocs-gen-files",
     "mkdocs",
 ]
+license = "MIT"
+
+
+[project.entry-points."mkdocs.plugins"]
+linkreplacer = "mknodes.__linkreplacer:LinkReplacerPlugin"
 
 [project.urls]
 Documentation = "https://phil65.github.io/mknodes/"
 Source = "https://github.com/phil65/mknodes"
 
 
 [tool.pytest.ini_options]
```

### Comparing `mknodes-0.3.2/PKG-INFO` & `mknodes-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 Metadata-Version: 2.1
 Name: mknodes
-Version: 0.3.2
+Version: 0.4.0
 Summary: Generate docs with ease.
 Project-URL: Documentation, https://phil65.github.io/mknodes/
 Project-URL: Source, https://github.com/phil65/mknodes
 Author-email: mknodes <philipptemminghoff@gmail.com>
+License-Expression: MIT
 License-File: LICENSE
+Keywords: docs,docstrings,documentation,framework,internet,markdown
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation
+Classifier: Topic :: Internet
+Classifier: Topic :: Text Processing :: Markup :: Markdown
 Requires-Python: >=3.10
 Requires-Dist: mkdocs
 Requires-Dist: mkdocs-gen-files
 Requires-Dist: typing-extensions
 Description-Content-Type: text/markdown
 
 # MkNodes
```

#### html2text {}

```diff
@@ -1,14 +1,21 @@
-Metadata-Version: 2.1 Name: mknodes Version: 0.3.2 Summary: Generate docs with
+Metadata-Version: 2.1 Name: mknodes Version: 0.4.0 Summary: Generate docs with
 ease. Project-URL: Documentation, https://phil65.github.io/mknodes/ Project-
 URL: Source, https://github.com/phil65/mknodes Author-email: mknodes
-gmail.com> License-File: LICENSE Classifier: Programming Language :: Python ::
-3 :: Only Requires-Python: >=3.10 Requires-Dist: mkdocs Requires-Dist: mkdocs-
-gen-files Requires-Dist: typing-extensions Description-Content-Type: text/
-markdown # MkNodes
+gmail.com> License-Expression: MIT License-File: LICENSE Keywords:
+docs,docstrings,documentation,framework,internet,markdown Classifier:
+Development Status :: 4 - Beta Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Documentation Classifier: Topic :: Internet Classifier: Topic :: Text
+Processing :: Markup :: Markdown Requires-Python: >=3.10 Requires-Dist: mkdocs
+Requires-Dist: mkdocs-gen-files Requires-Dist: typing-extensions Description-
+Content-Type: text/markdown # MkNodes
                            Generate docs with ease.
 [![build](https://github.com/phil65/mknodes/workflows/Build/badge.svg)](https:/
 /github.com/phil65/mknodes/actions) [![codecov](https://codecov.io/gh/phil65/
 mknodes/branch/master/graph/badge.svg)](https://codecov.io/gh/phil65/mknodes)
 [![PyPI version](https://badge.fury.io/py/mknodes.svg)](https://badge.fury.io/
 py/mknodes) --- **Documentation**: https://phil65.github.io/mknodes/ **Source
 Code**: https://github.com/phil65/mknodes --- ## Development ### Setup
```

