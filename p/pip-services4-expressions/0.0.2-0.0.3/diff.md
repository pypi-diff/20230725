# Comparing `tmp/pip_services4_expressions-0.0.2.tar.gz` & `tmp/pip_services4_expressions-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_services4_expressions-0.0.2.tar", last modified: Tue Jul 25 19:32:45 2023, max compression
+gzip compressed data, was "pip_services4_expressions-0.0.3.tar", last modified: Tue Jul 25 19:40:32 2023, max compression
```

## Comparing `pip_services4_expressions-0.0.2.tar` & `pip_services4_expressions-0.0.3.tar`

### file list

```diff
@@ -1,171 +1,171 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.208124 pip_services4_expressions-0.0.2/
--rw-rw-rw-   0        0        0      318 2023-07-25 19:32:26.000000 pip_services4_expressions-0.0.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1077 2021-01-07 09:04:44.000000 pip_services4_expressions-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       54 2020-12-23 20:20:18.000000 pip_services4_expressions-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3805 2023-07-25 19:32:45.209126 pip_services4_expressions-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2808 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:44.977149 pip_services4_expressions-0.0.2/pip_services4_expressions/
--rw-rw-rw-   0        0        0       24 2021-01-07 09:04:44.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.008885 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/
--rw-rw-rw-   0        0        0      794 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/CalculationStack.py
--rw-rw-rw-   0        0        0    13749 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/ExpressionCalculator.py
--rw-rw-rw-   0        0        0      586 2023-07-24 08:32:16.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/ExpressionException.py
--rw-rw-rw-   0        0        0      644 2021-07-21 18:30:08.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/SyntaxErrorCode.py
--rw-rw-rw-   0        0        0      574 2023-07-24 08:32:19.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/SyntaxException.py
--rw-rw-rw-   0        0        0      378 2021-10-05 00:40:00.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.029890 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/
--rw-rw-rw-   0        0        0    18721 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/DefaultFunctionCollection.py
--rw-rw-rw-   0        0        0     1773 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/DelegatedFunction.py
--rw-rw-rw-   0        0        0     2799 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/FunctionCollection.py
--rw-rw-rw-   0        0        0      686 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/IFunction.py
--rw-rw-rw-   0        0        0     1620 2021-07-21 18:01:04.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/IFunctionCollection.py
--rw-rw-rw-   0        0        0      407 2021-10-05 00:41:20.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.038887 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/parsers/
--rw-rw-rw-   0        0        0    20874 2023-07-24 08:29:22.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/parsers/ExpressionParser.py
--rw-rw-rw-   0        0        0     1342 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/parsers/ExpressionToken.py
--rw-rw-rw-   0        0        0      892 2021-03-15 23:41:16.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/parsers/ExpressionTokenType.py
--rw-rw-rw-   0        0        0      250 2021-10-05 00:40:30.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.053753 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/
--rw-rw-rw-   0        0        0     2455 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/ExpressionNumberState.py
--rw-rw-rw-   0        0        0     2953 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/ExpressionQuoteState.py
--rw-rw-rw-   0        0        0      602 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/ExpressionSymbolState.py
--rw-rw-rw-   0        0        0     2275 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/ExpressionTokenizer.py
--rw-rw-rw-   0        0        0     1897 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/ExpressionWordState.py
--rw-rw-rw-   0        0        0      441 2021-10-05 00:40:00.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.063751 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/variables/
--rw-rw-rw-   0        0        0      665 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/variables/IVariable.py
--rw-rw-rw-   0        0        0     2276 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/variables/IVariableCollection.py
--rw-rw-rw-   0        0        0     1056 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/variables/Variable.py
--rw-rw-rw-   0        0        0     3649 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/variables/VariableCollection.py
--rw-rw-rw-   0        0        0      284 2021-10-05 00:40:00.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/variables/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.072753 pip_services4_expressions-0.0.2/pip_services4_expressions/csv/
--rw-rw-rw-   0        0        0      109 2021-07-21 18:30:22.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/csv/CsvConstant.py
--rw-rw-rw-   0        0        0     2799 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/csv/CsvQuoteState.py
--rw-rw-rw-   0        0        0     1267 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/csv/CsvSymbolState.py
--rw-rw-rw-   0        0        0     4129 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/csv/CsvTokenizer.py
--rw-rw-rw-   0        0        0     1112 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/csv/CsvWordState.py
--rw-rw-rw-   0        0        0      329 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/csv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.075751 pip_services4_expressions-0.0.2/pip_services4_expressions/io/
--rw-rw-rw-   0        0        0     1728 2021-07-21 18:34:06.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/io/IScanner.py
--rw-rw-rw-   0        0        0     6152 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/io/StringScanner.py
--rw-rw-rw-   0        0        0      144 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/io/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.080761 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/
--rw-rw-rw-   0        0        0      594 2023-07-24 08:32:24.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/MustacheException.py
--rw-rw-rw-   0        0        0     7021 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/MustacheTemplate.py
--rw-rw-rw-   0        0        0      188 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.088757 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/parsers/
--rw-rw-rw-   0        0        0      815 2021-07-21 18:36:08.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/parsers/MustacheErrorCode.py
--rw-rw-rw-   0        0        0      292 2021-03-15 15:30:28.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/parsers/MustacheLexicalState.py
--rw-rw-rw-   0        0        0    13981 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/parsers/MustacheParser.py
--rw-rw-rw-   0        0        0     1502 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/parsers/MustacheToken.py
--rw-rw-rw-   0        0        0      359 2021-03-15 15:30:20.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/parsers/MustacheTokenType.py
--rw-rw-rw-   0        0        0      376 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/parsers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.091758 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/tokenizers/
--rw-rw-rw-   0        0        0     1549 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/tokenizers/MustacheSpecialState.py
--rw-rw-rw-   0        0        0     3499 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/tokenizers/MustacheTokenizer.py
--rw-rw-rw-   0        0        0      200 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/tokenizers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.108769 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/
--rw-rw-rw-   0        0        0     6322 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/AbstractTokenizer.py
--rw-rw-rw-   0        0        0      258 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/ICommentState.py
--rw-rw-rw-   0        0        0      245 2021-10-05 00:57:42.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/INumberState.py
--rw-rw-rw-   0        0        0      770 2021-07-23 15:47:40.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/IQuoteState.py
--rw-rw-rw-   0        0        0      479 2021-07-23 15:48:00.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/ISymbolState.py
--rw-rw-rw-   0        0        0     4968 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/ITokenizer.py
--rw-rw-rw-   0        0        0     1285 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/ITokenizerState.py
--rw-rw-rw-   0        0        0      759 2021-07-23 15:50:06.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/IWhitespaceState.py
--rw-rw-rw-   0        0        0      899 2021-07-23 15:50:24.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/IWordState.py
--rw-rw-rw-   0        0        0     1660 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/Token.py
--rw-rw-rw-   0        0        0      445 2021-01-07 09:04:44.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/TokenType.py
--rw-rw-rw-   0        0        0      654 2021-10-05 01:06:26.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.125075 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/
--rw-rw-rw-   0        0        0     1713 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/CCommentState.py
--rw-rw-rw-   0        0        0     3106 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/CppCommentState.py
--rw-rw-rw-   0        0        0     1659 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericCommentState.py
--rw-rw-rw-   0        0        0     2920 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericNumberState.py
--rw-rw-rw-   0        0        0     2845 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericQuoteState.py
--rw-rw-rw-   0        0        0     2259 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericSymbolState.py
--rw-rw-rw-   0        0        0     2284 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericTokenizer.py
--rw-rw-rw-   0        0        0     2326 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericWhitespaceState.py
--rw-rw-rw-   0        0        0     3639 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericWordState.py
--rw-rw-rw-   0        0        0     5543 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/SymbolNode.py
--rw-rw-rw-   0        0        0     1807 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/SymbolRootNode.py
--rw-rw-rw-   0        0        0      794 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.130077 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/utilities/
--rw-rw-rw-   0        0        0      771 2021-07-23 15:43:42.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/utilities/CharReferenceInterval.py
--rw-rw-rw-   0        0        0     1474 2021-07-23 15:44:32.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/utilities/CharReferenceMap.py
--rw-rw-rw-   0        0        0      449 2021-07-23 15:45:16.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/utilities/CharValidator.py
--rw-rw-rw-   0        0        0      250 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.139077 pip_services4_expressions-0.0.2/pip_services4_expressions/variants/
--rw-rw-rw-   0        0        0    30097 2021-07-26 23:09:32.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/variants/AbstractVariantOperations.py
--rw-rw-rw-   0        0        0     6843 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/variants/IVariantOperations.py
--rw-rw-rw-   0        0        0     2932 2021-07-23 15:55:38.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/variants/TypeSafeVariantOperations.py
--rw-rw-rw-   0        0        0    10867 2023-07-24 08:29:22.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/variants/TypeUnsafeVariantOperations.py
--rw-rw-rw-   0        0        0    12273 2023-07-24 08:29:22.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/variants/Variant.py
--rw-rw-rw-   0        0        0      359 2021-01-07 09:04:44.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/variants/VariantType.py
--rw-rw-rw-   0        0        0      532 2021-10-05 00:50:48.000000 pip_services4_expressions-0.0.2/pip_services4_expressions/variants/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.000663 pip_services4_expressions-0.0.2/pip_services4_expressions.egg-info/
--rw-rw-rw-   0        0        0     3805 2023-07-25 19:32:44.000000 pip_services4_expressions-0.0.2/pip_services4_expressions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7047 2023-07-25 19:32:44.000000 pip_services4_expressions-0.0.2/pip_services4_expressions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 19:32:44.000000 pip_services4_expressions-0.0.2/pip_services4_expressions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-07-25 19:32:44.000000 pip_services4_expressions-0.0.2/pip_services4_expressions.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-07-25 19:32:44.000000 pip_services4_expressions-0.0.2/pip_services4_expressions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 08:34:43.000000 pip_services4_expressions-0.0.2/pip_services4_expressions.egg-info/zip-safe
--rw-rw-rw-   0        0        0      181 2023-07-25 19:32:45.211125 pip_services4_expressions-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1723 2023-07-25 19:32:26.000000 pip_services4_expressions-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:44.963136 pip_services4_expressions-0.0.2/test/
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.142079 pip_services4_expressions-0.0.2/test/calculator/
--rw-rw-rw-   0        0        0       24 2021-03-18 22:19:58.000000 pip_services4_expressions-0.0.2/test/calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.146075 pip_services4_expressions-0.0.2/test/calculator/functions/
--rw-rw-rw-   0        0        0       24 2021-03-18 22:19:58.000000 pip_services4_expressions-0.0.2/test/calculator/functions/__init__.py
--rw-rw-rw-   0        0        0     1890 2023-07-24 08:29:22.000000 pip_services4_expressions-0.0.2/test/calculator/functions/test_DefaultFunctionCollection.py
--rw-rw-rw-   0        0        0     1044 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/test/calculator/functions/test_FunctionCollection.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.149076 pip_services4_expressions-0.0.2/test/calculator/parsers/
--rw-rw-rw-   0        0        0       24 2021-03-18 22:19:58.000000 pip_services4_expressions-0.0.2/test/calculator/parsers/__init__.py
--rw-rw-rw-   0        0        0     1732 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/calculator/parsers/test_ExpressionParser.py
--rw-rw-rw-   0        0        0     2680 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/calculator/test_ExpressionCalculator.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.151136 pip_services4_expressions-0.0.2/test/calculator/tokenizers/
--rw-rw-rw-   0        0        0       24 2021-03-18 22:19:58.000000 pip_services4_expressions-0.0.2/test/calculator/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     3339 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/calculator/tokenizers/test_ExpressionTokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.154141 pip_services4_expressions-0.0.2/test/calculator/variables/
--rw-rw-rw-   0        0        0       24 2021-03-18 22:19:58.000000 pip_services4_expressions-0.0.2/test/calculator/variables/__init__.py
--rw-rw-rw-   0        0        0      886 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/calculator/variables/test_VariableCollection.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.156143 pip_services4_expressions-0.0.2/test/csv/
--rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.2/test/csv/__init__.py
--rw-rw-rw-   0        0        0     4974 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/csv/test_CsvTokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.159142 pip_services4_expressions-0.0.2/test/io/
--rw-rw-rw-   0        0        0     1937 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.2/test/io/ScannerFixture.py
--rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.2/test/io/__init__.py
--rw-rw-rw-   0        0        0      959 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/io/test_StringScanner.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.163142 pip_services4_expressions-0.0.2/test/mustache/
--rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.2/test/mustache/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.167143 pip_services4_expressions-0.0.2/test/mustache/parsers/
--rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.2/test/mustache/parsers/__init__.py
--rw-rw-rw-   0        0        0     2476 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/test/mustache/parsers/test_MustacheParser.py
--rw-rw-rw-   0        0        0      701 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/mustache/test_MustacheTemplate.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.170143 pip_services4_expressions-0.0.2/test/mustache/tokenizers/
--rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.2/test/mustache/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     2694 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/test/mustache/tokenizers/test_MustacheTokenizer.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.174606 pip_services4_expressions-0.0.2/test/tokenizers/
--rw-rw-rw-   0        0        0      651 2021-03-18 22:20:48.000000 pip_services4_expressions-0.0.2/test/tokenizers/TokenizerFixture.py
--rw-rw-rw-   0        0        0       24 2021-03-18 22:20:48.000000 pip_services4_expressions-0.0.2/test/tokenizers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.190611 pip_services4_expressions-0.0.2/test/tokenizers/generic/
--rw-rw-rw-   0        0        0       24 2021-03-18 22:20:48.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/__init__.py
--rw-rw-rw-   0        0        0      782 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/test_CCommentState.py
--rw-rw-rw-   0        0        0      772 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/test_CppCommentState.py
--rw-rw-rw-   0        0        0      757 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericCommentState.py
--rw-rw-rw-   0        0        0     1442 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericNumberState.py
--rw-rw-rw-   0        0        0     1068 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericQuoteState.py
--rw-rw-rw-   0        0        0     1045 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericSymbolState.py
--rw-rw-rw-   0        0        0     3591 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericTokenizer.py
--rw-rw-rw-   0        0        0      560 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericWhitespaceState.py
--rw-rw-rw-   0        0        0      524 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericWordState.py
--rw-rw-rw-   0        0        0     1040 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/generic/test_SymbolRootNode.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.200125 pip_services4_expressions-0.0.2/test/tokenizers/utilities/
--rw-rw-rw-   0        0        0       24 2021-03-18 22:20:48.000000 pip_services4_expressions-0.0.2/test/tokenizers/utilities/__init__.py
--rw-rw-rw-   0        0        0     1230 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/utilities/test_CharReferenceMap.py
--rw-rw-rw-   0        0        0      708 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/tokenizers/utilities/test_CharValidator.py
-drwxrwxrwx   0        0        0        0 2023-07-25 19:32:45.207127 pip_services4_expressions-0.0.2/test/variants/
--rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.2/test/variants/__init__.py
--rw-rw-rw-   0        0        0     1020 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/variants/test_TypeSafeVariantOperations.py
--rw-rw-rw-   0        0        0      720 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/variants/test_TypeUnsafeVariantOperations.py
--rw-rw-rw-   0        0        0      494 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.2/test/variants/test_Variant.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.504590 pip_services4_expressions-0.0.3/
+-rw-rw-rw-   0        0        0      318 2023-07-25 19:32:26.000000 pip_services4_expressions-0.0.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1077 2021-01-07 09:04:44.000000 pip_services4_expressions-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       54 2020-12-23 20:20:18.000000 pip_services4_expressions-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3805 2023-07-25 19:40:32.505590 pip_services4_expressions-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2808 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.330054 pip_services4_expressions-0.0.3/pip_services4_expressions/
+-rw-rw-rw-   0        0        0       24 2021-01-07 09:04:44.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.346562 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/
+-rw-rw-rw-   0        0        0      794 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/CalculationStack.py
+-rw-rw-rw-   0        0        0    13749 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/ExpressionCalculator.py
+-rw-rw-rw-   0        0        0      586 2023-07-24 08:32:16.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/ExpressionException.py
+-rw-rw-rw-   0        0        0      644 2021-07-21 18:30:08.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/SyntaxErrorCode.py
+-rw-rw-rw-   0        0        0      574 2023-07-24 08:32:19.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/SyntaxException.py
+-rw-rw-rw-   0        0        0      378 2021-10-05 00:40:00.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.353560 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/
+-rw-rw-rw-   0        0        0    18721 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/DefaultFunctionCollection.py
+-rw-rw-rw-   0        0        0     1773 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/DelegatedFunction.py
+-rw-rw-rw-   0        0        0     2799 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/FunctionCollection.py
+-rw-rw-rw-   0        0        0      686 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/IFunction.py
+-rw-rw-rw-   0        0        0     1620 2021-07-21 18:01:04.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/IFunctionCollection.py
+-rw-rw-rw-   0        0        0      407 2021-10-05 00:41:20.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.358564 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/parsers/
+-rw-rw-rw-   0        0        0    20874 2023-07-24 08:29:22.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/parsers/ExpressionParser.py
+-rw-rw-rw-   0        0        0     1342 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/parsers/ExpressionToken.py
+-rw-rw-rw-   0        0        0      892 2021-03-15 23:41:16.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/parsers/ExpressionTokenType.py
+-rw-rw-rw-   0        0        0      250 2021-10-05 00:40:30.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.366560 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/
+-rw-rw-rw-   0        0        0     2455 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/ExpressionNumberState.py
+-rw-rw-rw-   0        0        0     2953 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/ExpressionQuoteState.py
+-rw-rw-rw-   0        0        0      602 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/ExpressionSymbolState.py
+-rw-rw-rw-   0        0        0     2275 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/ExpressionTokenizer.py
+-rw-rw-rw-   0        0        0     1897 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/ExpressionWordState.py
+-rw-rw-rw-   0        0        0      441 2021-10-05 00:40:00.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.374562 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/variables/
+-rw-rw-rw-   0        0        0      665 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/variables/IVariable.py
+-rw-rw-rw-   0        0        0     2276 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/variables/IVariableCollection.py
+-rw-rw-rw-   0        0        0     1056 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/variables/Variable.py
+-rw-rw-rw-   0        0        0     3649 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/variables/VariableCollection.py
+-rw-rw-rw-   0        0        0      284 2021-10-05 00:40:00.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/variables/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.385016 pip_services4_expressions-0.0.3/pip_services4_expressions/csv/
+-rw-rw-rw-   0        0        0      109 2021-07-21 18:30:22.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/csv/CsvConstant.py
+-rw-rw-rw-   0        0        0     2799 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/csv/CsvQuoteState.py
+-rw-rw-rw-   0        0        0     1267 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/csv/CsvSymbolState.py
+-rw-rw-rw-   0        0        0     4129 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/csv/CsvTokenizer.py
+-rw-rw-rw-   0        0        0     1112 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/csv/CsvWordState.py
+-rw-rw-rw-   0        0        0      329 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/csv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.389078 pip_services4_expressions-0.0.3/pip_services4_expressions/io/
+-rw-rw-rw-   0        0        0     1728 2021-07-21 18:34:06.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/io/IScanner.py
+-rw-rw-rw-   0        0        0     6152 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/io/StringScanner.py
+-rw-rw-rw-   0        0        0      144 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/io/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.394074 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/
+-rw-rw-rw-   0        0        0      594 2023-07-24 08:32:24.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/MustacheException.py
+-rw-rw-rw-   0        0        0     7021 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/MustacheTemplate.py
+-rw-rw-rw-   0        0        0      188 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.402074 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/parsers/
+-rw-rw-rw-   0        0        0      815 2021-07-21 18:36:08.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/parsers/MustacheErrorCode.py
+-rw-rw-rw-   0        0        0      292 2021-03-15 15:30:28.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/parsers/MustacheLexicalState.py
+-rw-rw-rw-   0        0        0    13981 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/parsers/MustacheParser.py
+-rw-rw-rw-   0        0        0     1502 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/parsers/MustacheToken.py
+-rw-rw-rw-   0        0        0      359 2021-03-15 15:30:20.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/parsers/MustacheTokenType.py
+-rw-rw-rw-   0        0        0      376 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/parsers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.406074 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/tokenizers/
+-rw-rw-rw-   0        0        0     1549 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/tokenizers/MustacheSpecialState.py
+-rw-rw-rw-   0        0        0     3499 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/tokenizers/MustacheTokenizer.py
+-rw-rw-rw-   0        0        0      200 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/tokenizers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.422076 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/
+-rw-rw-rw-   0        0        0     6322 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/AbstractTokenizer.py
+-rw-rw-rw-   0        0        0      258 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/ICommentState.py
+-rw-rw-rw-   0        0        0      245 2021-10-05 00:57:42.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/INumberState.py
+-rw-rw-rw-   0        0        0      770 2021-07-23 15:47:40.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/IQuoteState.py
+-rw-rw-rw-   0        0        0      479 2021-07-23 15:48:00.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/ISymbolState.py
+-rw-rw-rw-   0        0        0     4968 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/ITokenizer.py
+-rw-rw-rw-   0        0        0     1285 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/ITokenizerState.py
+-rw-rw-rw-   0        0        0      759 2021-07-23 15:50:06.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/IWhitespaceState.py
+-rw-rw-rw-   0        0        0      899 2021-07-23 15:50:24.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/IWordState.py
+-rw-rw-rw-   0        0        0     1660 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/Token.py
+-rw-rw-rw-   0        0        0      445 2021-01-07 09:04:44.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/TokenType.py
+-rw-rw-rw-   0        0        0      654 2021-10-05 01:06:26.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.437081 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/
+-rw-rw-rw-   0        0        0     1713 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/CCommentState.py
+-rw-rw-rw-   0        0        0     3106 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/CppCommentState.py
+-rw-rw-rw-   0        0        0     1659 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericCommentState.py
+-rw-rw-rw-   0        0        0     2920 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericNumberState.py
+-rw-rw-rw-   0        0        0     2845 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericQuoteState.py
+-rw-rw-rw-   0        0        0     2259 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericSymbolState.py
+-rw-rw-rw-   0        0        0     2284 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericTokenizer.py
+-rw-rw-rw-   0        0        0     2326 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericWhitespaceState.py
+-rw-rw-rw-   0        0        0     3639 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericWordState.py
+-rw-rw-rw-   0        0        0     5543 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/SymbolNode.py
+-rw-rw-rw-   0        0        0     1807 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/SymbolRootNode.py
+-rw-rw-rw-   0        0        0      794 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.442591 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/utilities/
+-rw-rw-rw-   0        0        0      771 2021-07-23 15:43:42.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/utilities/CharReferenceInterval.py
+-rw-rw-rw-   0        0        0     1474 2021-07-23 15:44:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/utilities/CharReferenceMap.py
+-rw-rw-rw-   0        0        0      449 2021-07-23 15:45:16.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/utilities/CharValidator.py
+-rw-rw-rw-   0        0        0      250 2021-10-05 00:50:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.450592 pip_services4_expressions-0.0.3/pip_services4_expressions/variants/
+-rw-rw-rw-   0        0        0    30097 2021-07-26 23:09:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/variants/AbstractVariantOperations.py
+-rw-rw-rw-   0        0        0     6843 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/variants/IVariantOperations.py
+-rw-rw-rw-   0        0        0     2932 2021-07-23 15:55:38.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/variants/TypeSafeVariantOperations.py
+-rw-rw-rw-   0        0        0    10867 2023-07-24 08:29:22.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/variants/TypeUnsafeVariantOperations.py
+-rw-rw-rw-   0        0        0    12273 2023-07-24 08:29:22.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/variants/Variant.py
+-rw-rw-rw-   0        0        0      359 2021-01-07 09:04:44.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/variants/VariantType.py
+-rw-rw-rw-   0        0        0      532 2021-10-05 00:50:48.000000 pip_services4_expressions-0.0.3/pip_services4_expressions/variants/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.339052 pip_services4_expressions-0.0.3/pip_services4_expressions.egg-info/
+-rw-rw-rw-   0        0        0     3805 2023-07-25 19:40:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7047 2023-07-25 19:40:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 19:40:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-07-25 19:40:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-07-25 19:40:32.000000 pip_services4_expressions-0.0.3/pip_services4_expressions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 08:34:43.000000 pip_services4_expressions-0.0.3/pip_services4_expressions.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      181 2023-07-25 19:40:32.506591 pip_services4_expressions-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1723 2023-07-25 19:40:17.000000 pip_services4_expressions-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.321048 pip_services4_expressions-0.0.3/test/
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.452592 pip_services4_expressions-0.0.3/test/calculator/
+-rw-rw-rw-   0        0        0       24 2021-03-18 22:19:58.000000 pip_services4_expressions-0.0.3/test/calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.456592 pip_services4_expressions-0.0.3/test/calculator/functions/
+-rw-rw-rw-   0        0        0       24 2021-03-18 22:19:58.000000 pip_services4_expressions-0.0.3/test/calculator/functions/__init__.py
+-rw-rw-rw-   0        0        0     1890 2023-07-24 08:29:22.000000 pip_services4_expressions-0.0.3/test/calculator/functions/test_DefaultFunctionCollection.py
+-rw-rw-rw-   0        0        0     1044 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/test/calculator/functions/test_FunctionCollection.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.458591 pip_services4_expressions-0.0.3/test/calculator/parsers/
+-rw-rw-rw-   0        0        0       24 2021-03-18 22:19:58.000000 pip_services4_expressions-0.0.3/test/calculator/parsers/__init__.py
+-rw-rw-rw-   0        0        0     1732 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/calculator/parsers/test_ExpressionParser.py
+-rw-rw-rw-   0        0        0     2680 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/calculator/test_ExpressionCalculator.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.460590 pip_services4_expressions-0.0.3/test/calculator/tokenizers/
+-rw-rw-rw-   0        0        0       24 2021-03-18 22:19:58.000000 pip_services4_expressions-0.0.3/test/calculator/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     3339 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/calculator/tokenizers/test_ExpressionTokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.463591 pip_services4_expressions-0.0.3/test/calculator/variables/
+-rw-rw-rw-   0        0        0       24 2021-03-18 22:19:58.000000 pip_services4_expressions-0.0.3/test/calculator/variables/__init__.py
+-rw-rw-rw-   0        0        0      886 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/calculator/variables/test_VariableCollection.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.465591 pip_services4_expressions-0.0.3/test/csv/
+-rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.3/test/csv/__init__.py
+-rw-rw-rw-   0        0        0     4974 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/csv/test_CsvTokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.469594 pip_services4_expressions-0.0.3/test/io/
+-rw-rw-rw-   0        0        0     1937 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.3/test/io/ScannerFixture.py
+-rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.3/test/io/__init__.py
+-rw-rw-rw-   0        0        0      959 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/io/test_StringScanner.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.471590 pip_services4_expressions-0.0.3/test/mustache/
+-rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.3/test/mustache/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.474592 pip_services4_expressions-0.0.3/test/mustache/parsers/
+-rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.3/test/mustache/parsers/__init__.py
+-rw-rw-rw-   0        0        0     2476 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/test/mustache/parsers/test_MustacheParser.py
+-rw-rw-rw-   0        0        0      701 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/mustache/test_MustacheTemplate.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.476592 pip_services4_expressions-0.0.3/test/mustache/tokenizers/
+-rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.3/test/mustache/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     2694 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/test/mustache/tokenizers/test_MustacheTokenizer.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.478590 pip_services4_expressions-0.0.3/test/tokenizers/
+-rw-rw-rw-   0        0        0      651 2021-03-18 22:20:48.000000 pip_services4_expressions-0.0.3/test/tokenizers/TokenizerFixture.py
+-rw-rw-rw-   0        0        0       24 2021-03-18 22:20:48.000000 pip_services4_expressions-0.0.3/test/tokenizers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.491592 pip_services4_expressions-0.0.3/test/tokenizers/generic/
+-rw-rw-rw-   0        0        0       24 2021-03-18 22:20:48.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/__init__.py
+-rw-rw-rw-   0        0        0      782 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/test_CCommentState.py
+-rw-rw-rw-   0        0        0      772 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/test_CppCommentState.py
+-rw-rw-rw-   0        0        0      757 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericCommentState.py
+-rw-rw-rw-   0        0        0     1442 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericNumberState.py
+-rw-rw-rw-   0        0        0     1068 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericQuoteState.py
+-rw-rw-rw-   0        0        0     1045 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericSymbolState.py
+-rw-rw-rw-   0        0        0     3591 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericTokenizer.py
+-rw-rw-rw-   0        0        0      560 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericWhitespaceState.py
+-rw-rw-rw-   0        0        0      524 2023-07-24 08:27:46.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericWordState.py
+-rw-rw-rw-   0        0        0     1040 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/generic/test_SymbolRootNode.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.497590 pip_services4_expressions-0.0.3/test/tokenizers/utilities/
+-rw-rw-rw-   0        0        0       24 2021-03-18 22:20:48.000000 pip_services4_expressions-0.0.3/test/tokenizers/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1230 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/utilities/test_CharReferenceMap.py
+-rw-rw-rw-   0        0        0      708 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/tokenizers/utilities/test_CharValidator.py
+drwxrwxrwx   0        0        0        0 2023-07-25 19:40:32.504590 pip_services4_expressions-0.0.3/test/variants/
+-rw-rw-rw-   0        0        0       24 2021-03-18 23:19:16.000000 pip_services4_expressions-0.0.3/test/variants/__init__.py
+-rw-rw-rw-   0        0        0     1020 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/variants/test_TypeSafeVariantOperations.py
+-rw-rw-rw-   0        0        0      720 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/variants/test_TypeUnsafeVariantOperations.py
+-rw-rw-rw-   0        0        0      494 2023-07-24 08:27:47.000000 pip_services4_expressions-0.0.3/test/variants/test_Variant.py
```

### Comparing `pip_services4_expressions-0.0.2/LICENSE` & `pip_services4_expressions-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/PKG-INFO` & `pip_services4_expressions-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip_services4_expressions
-Version: 0.0.2
+Version: 0.0.3
 Summary: Basic portable abstractions for Pip.Services in Python
 Home-page: http://github.com/pip-services3-python/pip-services3-expressions-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_expressions-0.0.2/README.md` & `pip_services4_expressions-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/CalculationStack.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/CalculationStack.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/ExpressionCalculator.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/ExpressionCalculator.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/ExpressionException.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/ExpressionException.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/SyntaxErrorCode.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/SyntaxErrorCode.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/SyntaxException.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/SyntaxException.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/DefaultFunctionCollection.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/DefaultFunctionCollection.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/DelegatedFunction.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/DelegatedFunction.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/FunctionCollection.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/FunctionCollection.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/IFunction.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/IFunction.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/functions/IFunctionCollection.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/functions/IFunctionCollection.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/parsers/ExpressionParser.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/parsers/ExpressionParser.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/parsers/ExpressionToken.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/parsers/ExpressionToken.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/parsers/ExpressionTokenType.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/parsers/ExpressionTokenType.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/ExpressionNumberState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/ExpressionNumberState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/ExpressionQuoteState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/ExpressionQuoteState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/ExpressionSymbolState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/ExpressionSymbolState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/ExpressionTokenizer.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/ExpressionTokenizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/tokenizers/ExpressionWordState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/tokenizers/ExpressionWordState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/variables/IVariable.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/variables/IVariable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/variables/IVariableCollection.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/variables/IVariableCollection.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/variables/Variable.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/variables/Variable.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/calculator/variables/VariableCollection.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/calculator/variables/VariableCollection.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/csv/CsvQuoteState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/csv/CsvQuoteState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/csv/CsvSymbolState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/csv/CsvSymbolState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/csv/CsvTokenizer.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/csv/CsvTokenizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/csv/CsvWordState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/csv/CsvWordState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/io/IScanner.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/io/IScanner.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/io/StringScanner.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/io/StringScanner.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/MustacheException.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/MustacheException.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/MustacheTemplate.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/MustacheTemplate.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/parsers/MustacheErrorCode.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/parsers/MustacheErrorCode.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/parsers/MustacheParser.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/parsers/MustacheParser.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/parsers/MustacheToken.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/parsers/MustacheToken.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/tokenizers/MustacheSpecialState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/tokenizers/MustacheSpecialState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/mustache/tokenizers/MustacheTokenizer.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/mustache/tokenizers/MustacheTokenizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/AbstractTokenizer.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/AbstractTokenizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/IQuoteState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/IQuoteState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/ITokenizer.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/ITokenizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/ITokenizerState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/ITokenizerState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/IWhitespaceState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/IWhitespaceState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/IWordState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/IWordState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/Token.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/Token.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/__init__.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/CCommentState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/CCommentState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/CppCommentState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/CppCommentState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericCommentState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericCommentState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericNumberState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericNumberState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericQuoteState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericQuoteState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericSymbolState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericSymbolState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericTokenizer.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericTokenizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericWhitespaceState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericWhitespaceState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/GenericWordState.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/GenericWordState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/SymbolNode.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/SymbolNode.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/SymbolRootNode.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/SymbolRootNode.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/generic/__init__.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/utilities/CharReferenceInterval.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/utilities/CharReferenceInterval.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/tokenizers/utilities/CharReferenceMap.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/tokenizers/utilities/CharReferenceMap.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/variants/AbstractVariantOperations.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/variants/AbstractVariantOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/variants/IVariantOperations.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/variants/IVariantOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/variants/TypeSafeVariantOperations.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/variants/TypeSafeVariantOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/variants/TypeUnsafeVariantOperations.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/variants/TypeUnsafeVariantOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/variants/Variant.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/variants/Variant.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions/variants/__init__.py` & `pip_services4_expressions-0.0.3/pip_services4_expressions/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions.egg-info/PKG-INFO` & `pip_services4_expressions-0.0.3/pip_services4_expressions.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-services4-expressions
-Version: 0.0.2
+Version: 0.0.3
 Summary: Basic portable abstractions for Pip.Services in Python
 Home-page: http://github.com/pip-services3-python/pip-services3-expressions-python
 Author: Conceptual Vision Consulting LLC
 Author-email: seroukhov@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pip_services4_expressions-0.0.2/pip_services4_expressions.egg-info/SOURCES.txt` & `pip_services4_expressions-0.0.3/pip_services4_expressions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/setup.py` & `pip_services4_expressions-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,29 +19,29 @@
 try:
     readme = open('readme.md').read()
 except:
     readme = __doc__
 
 setup(
     name='pip_services4_expressions',
-    version='0.0.2',
+    version='0.0.3',
     url='http://github.com/pip-services3-python/pip-services3-expressions-python',
     license='MIT',
     description='Basic portable abstractions for Pip.Services in Python',
     author='Conceptual Vision Consulting LLC',
     author_email='seroukhov@gmail.com',
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=['config', 'data', 'test']),
     include_package_data=True,
     zip_safe=True,
     platforms='any',
     install_requires=[
         'pytest',
-        'pip_services4_commons >= 0.0.2, < 1.0'
+        'pip_services4_commons >= 0.0.1, < 1.0'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
```

### Comparing `pip_services4_expressions-0.0.2/test/calculator/functions/test_DefaultFunctionCollection.py` & `pip_services4_expressions-0.0.3/test/calculator/functions/test_DefaultFunctionCollection.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/calculator/functions/test_FunctionCollection.py` & `pip_services4_expressions-0.0.3/test/calculator/functions/test_FunctionCollection.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/calculator/parsers/test_ExpressionParser.py` & `pip_services4_expressions-0.0.3/test/calculator/parsers/test_ExpressionParser.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/calculator/test_ExpressionCalculator.py` & `pip_services4_expressions-0.0.3/test/calculator/test_ExpressionCalculator.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/calculator/tokenizers/test_ExpressionTokenizer.py` & `pip_services4_expressions-0.0.3/test/calculator/tokenizers/test_ExpressionTokenizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/calculator/variables/test_VariableCollection.py` & `pip_services4_expressions-0.0.3/test/calculator/variables/test_VariableCollection.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/csv/test_CsvTokenizer.py` & `pip_services4_expressions-0.0.3/test/csv/test_CsvTokenizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/io/ScannerFixture.py` & `pip_services4_expressions-0.0.3/test/io/ScannerFixture.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/io/test_StringScanner.py` & `pip_services4_expressions-0.0.3/test/io/test_StringScanner.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/mustache/parsers/test_MustacheParser.py` & `pip_services4_expressions-0.0.3/test/mustache/parsers/test_MustacheParser.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/mustache/test_MustacheTemplate.py` & `pip_services4_expressions-0.0.3/test/mustache/test_MustacheTemplate.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/mustache/tokenizers/test_MustacheTokenizer.py` & `pip_services4_expressions-0.0.3/test/mustache/tokenizers/test_MustacheTokenizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/TokenizerFixture.py` & `pip_services4_expressions-0.0.3/test/tokenizers/TokenizerFixture.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/generic/test_CCommentState.py` & `pip_services4_expressions-0.0.3/test/tokenizers/generic/test_CCommentState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/generic/test_CppCommentState.py` & `pip_services4_expressions-0.0.3/test/tokenizers/generic/test_CppCommentState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericCommentState.py` & `pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericCommentState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericNumberState.py` & `pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericNumberState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericQuoteState.py` & `pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericQuoteState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericSymbolState.py` & `pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericSymbolState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericTokenizer.py` & `pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericTokenizer.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericWhitespaceState.py` & `pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericWhitespaceState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/generic/test_GenericWordState.py` & `pip_services4_expressions-0.0.3/test/tokenizers/generic/test_GenericWordState.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/generic/test_SymbolRootNode.py` & `pip_services4_expressions-0.0.3/test/tokenizers/generic/test_SymbolRootNode.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/utilities/test_CharReferenceMap.py` & `pip_services4_expressions-0.0.3/test/tokenizers/utilities/test_CharReferenceMap.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/tokenizers/utilities/test_CharValidator.py` & `pip_services4_expressions-0.0.3/test/tokenizers/utilities/test_CharValidator.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/variants/test_TypeSafeVariantOperations.py` & `pip_services4_expressions-0.0.3/test/variants/test_TypeSafeVariantOperations.py`

 * *Files identical despite different names*

### Comparing `pip_services4_expressions-0.0.2/test/variants/test_TypeUnsafeVariantOperations.py` & `pip_services4_expressions-0.0.3/test/variants/test_TypeUnsafeVariantOperations.py`

 * *Files identical despite different names*

