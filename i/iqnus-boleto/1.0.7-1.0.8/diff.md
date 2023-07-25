# Comparing `tmp/iqnus-boleto-1.0.7.tar.gz` & `tmp/iqnus-boleto-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iqnus-boleto-1.0.7.tar", last modified: Tue Jul 25 16:47:38 2023, max compression
+gzip compressed data, was "iqnus-boleto-1.0.8.tar", last modified: Tue Jul 25 16:54:14 2023, max compression
```

## Comparing `iqnus-boleto-1.0.7.tar` & `iqnus-boleto-1.0.8.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:47:38.939938 iqnus-boleto-1.0.7/
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1537 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/LICENSE
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)      206 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/MANIFEST.in
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6194 2023-07-25 16:47:38.939938 iqnus-boleto-1.0.7/PKG-INFO
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4145 2023-07-25 16:47:07.000000 iqnus-boleto-1.0.7/README.rst
-drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:47:38.911937 iqnus-boleto-1.0.7/bin/
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     8716 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/bin/html_pyboleto_sample.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     9038 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/bin/pdf_pyboleto_sample.py
-drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:47:38.919937 iqnus-boleto-1.0.7/iqnus_boleto.egg-info/
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6194 2023-07-25 16:47:38.000000 iqnus-boleto-1.0.7/iqnus_boleto.egg-info/PKG-INFO
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2674 2023-07-25 16:47:38.000000 iqnus-boleto-1.0.7/iqnus_boleto.egg-info/SOURCES.txt
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)        1 2023-07-25 16:47:38.000000 iqnus-boleto-1.0.7/iqnus_boleto.egg-info/dependency_links.txt
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)        1 2023-07-25 16:32:32.000000 iqnus-boleto-1.0.7/iqnus_boleto.egg-info/not-zip-safe
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)       10 2023-07-25 16:47:38.000000 iqnus-boleto-1.0.7/iqnus_boleto.egg-info/requires.txt
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)       15 2023-07-25 16:47:38.000000 iqnus-boleto-1.0.7/iqnus_boleto.egg-info/top_level.txt
-drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:47:38.923938 iqnus-boleto-1.0.7/pyboleto/
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)       22 2023-07-25 16:31:34.000000 iqnus-boleto-1.0.7/pyboleto/__init__.py
-drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:47:38.923938 iqnus-boleto-1.0.7/pyboleto/bank/
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1004 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/__init__.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4986 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/bancodobrasil.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1111 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/banrisul.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1685 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/bradesco.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1922 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/caixa.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1250 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/caixa_sigcb.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1604 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/cecred.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2427 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/hsbc.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2273 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/itau.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1889 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/santander.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2323 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/sicoob.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2136 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/bank/sicredi.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    18235 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/data.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    10233 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/html.py
-drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:47:38.927938 iqnus-boleto-1.0.7/pyboleto/media/
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4007 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_bancobradesco.jpg
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     3350 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_bancocaixa.jpg
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     3414 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_bancohsbc.jpg
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    13780 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_bancoreal.jpg
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4457 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_banrisul.jpg
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2877 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_bb.jpg
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4161 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_cecred.jpg
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     5467 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_itau.jpg
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1683 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_santander.png
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4189 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_sicoob.jpg
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    11268 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/media/logo_sicredi.png
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    31341 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/pdf.py
-drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:47:38.927938 iqnus-boleto-1.0.7/pyboleto/templates/
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2873 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/templates/head.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     3742 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/templates/recibo_caixa.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1859 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/pyboleto/templates/recibo_sacado.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)      158 2023-07-25 16:47:38.939938 iqnus-boleto-1.0.7/setup.cfg
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2341 2023-07-25 16:47:28.000000 iqnus-boleto-1.0.7/setup.py
-drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:47:38.931938 iqnus-boleto-1.0.7/tests/
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/__init__.py
-drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:47:38.931938 iqnus-boleto-1.0.7/tests/html/
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    21448 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/html/BoletoBB-expected.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    25590 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/html/BoletoBanrisul-expected.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    24437 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/html/BoletoBradesco-expected.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    22682 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/html/BoletoCaixa-expected.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    22837 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/html/BoletoHsbc-expected.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    22823 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/html/BoletoHsbcComRegistro-expected.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    28331 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/html/BoletoItau-expected.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    18201 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/html/BoletoSantander-expected.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    24926 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/html/BoletoSicoob-expected.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    22793 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/html/BoletoSicredi-expected.html
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1457 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/test_banco_banrisul.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1415 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/test_banco_bradesco.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1357 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/test_banco_caixa.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1228 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/test_banco_do_brasil.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1513 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/test_banco_hsbc.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1509 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/test_banco_hsbc_com_registro.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1626 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/test_banco_itau.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1498 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/test_banco_santander.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1383 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/test_banco_sicoob.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1581 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/test_banco_sicredi.py
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6988 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/testutils.py
-drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:47:38.939938 iqnus-boleto-1.0.7/tests/xml/
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6190 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/BoletoBB-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6037 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/BoletoBanrisul-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6155 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/BoletoBradesco-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6153 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/BoletoCaixa-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6141 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/BoletoHsbc-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6196 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/BoletoHsbcComRegistro-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6232 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/BoletoItau-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6121 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/BoletoSantander-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6221 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/BoletoSicoob-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6197 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/BoletoSicredi-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17978 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoBB-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17519 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoBanrisul-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17873 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoBradesco-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17867 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoCaixa-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17831 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoHsbc-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17996 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoHsbcComRegistro-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    18104 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoItau-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17771 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoSantander-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6221 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoSicoob-expected.xml
--rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17999 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoSicredi-expected.xml
+drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:54:14.790809 iqnus-boleto-1.0.8/
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1537 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/LICENSE
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)      206 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/MANIFEST.in
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6207 2023-07-25 16:54:14.794809 iqnus-boleto-1.0.8/PKG-INFO
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4144 2023-07-25 16:49:52.000000 iqnus-boleto-1.0.8/README.rst
+drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:54:14.774808 iqnus-boleto-1.0.8/bin/
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     8716 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/bin/html_pyboleto_sample.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     9038 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/bin/pdf_pyboleto_sample.py
+drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:54:14.778808 iqnus-boleto-1.0.8/iqnus_boleto.egg-info/
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6207 2023-07-25 16:54:14.000000 iqnus-boleto-1.0.8/iqnus_boleto.egg-info/PKG-INFO
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2674 2023-07-25 16:54:14.000000 iqnus-boleto-1.0.8/iqnus_boleto.egg-info/SOURCES.txt
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)        1 2023-07-25 16:54:14.000000 iqnus-boleto-1.0.8/iqnus_boleto.egg-info/dependency_links.txt
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)        1 2023-07-25 16:32:32.000000 iqnus-boleto-1.0.8/iqnus_boleto.egg-info/not-zip-safe
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)       10 2023-07-25 16:54:14.000000 iqnus-boleto-1.0.8/iqnus_boleto.egg-info/requires.txt
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)       15 2023-07-25 16:54:14.000000 iqnus-boleto-1.0.8/iqnus_boleto.egg-info/top_level.txt
+drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:54:14.778808 iqnus-boleto-1.0.8/pyboleto/
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)       22 2023-07-25 16:54:03.000000 iqnus-boleto-1.0.8/pyboleto/__init__.py
+drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:54:14.778808 iqnus-boleto-1.0.8/pyboleto/bank/
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1004 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/__init__.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4986 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/bancodobrasil.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1111 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/banrisul.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1685 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/bradesco.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1922 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/caixa.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1250 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/caixa_sigcb.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1604 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/cecred.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2427 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/hsbc.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2273 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/itau.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1889 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/santander.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2373 2023-07-25 16:53:53.000000 iqnus-boleto-1.0.8/pyboleto/bank/sicoob.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2136 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/bank/sicredi.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    18235 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/data.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    10233 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/html.py
+drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:54:14.782808 iqnus-boleto-1.0.8/pyboleto/media/
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4007 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_bancobradesco.jpg
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     3350 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_bancocaixa.jpg
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     3414 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_bancohsbc.jpg
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    13780 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_bancoreal.jpg
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4457 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_banrisul.jpg
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2877 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_bb.jpg
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4161 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_cecred.jpg
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     5467 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_itau.jpg
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1683 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_santander.png
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     4189 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_sicoob.jpg
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    11268 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/media/logo_sicredi.png
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    31341 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/pdf.py
+drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:54:14.782808 iqnus-boleto-1.0.8/pyboleto/templates/
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2873 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/templates/head.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     3742 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/templates/recibo_caixa.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1859 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/pyboleto/templates/recibo_sacado.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)      158 2023-07-25 16:54:14.794809 iqnus-boleto-1.0.8/setup.cfg
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     2357 2023-07-25 16:50:18.000000 iqnus-boleto-1.0.8/setup.py
+drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:54:14.786808 iqnus-boleto-1.0.8/tests/
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/__init__.py
+drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:54:14.786808 iqnus-boleto-1.0.8/tests/html/
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    21448 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/html/BoletoBB-expected.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    25590 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/html/BoletoBanrisul-expected.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    24437 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/html/BoletoBradesco-expected.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    22682 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/html/BoletoCaixa-expected.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    22837 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/html/BoletoHsbc-expected.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    22823 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/html/BoletoHsbcComRegistro-expected.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    28331 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/html/BoletoItau-expected.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    18201 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/html/BoletoSantander-expected.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    24926 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/html/BoletoSicoob-expected.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    22793 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/html/BoletoSicredi-expected.html
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1457 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/test_banco_banrisul.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1415 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/test_banco_bradesco.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1357 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/test_banco_caixa.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1228 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/test_banco_do_brasil.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1513 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/test_banco_hsbc.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1509 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/test_banco_hsbc_com_registro.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1626 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/test_banco_itau.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1498 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/test_banco_santander.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1383 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/test_banco_sicoob.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     1581 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/test_banco_sicredi.py
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6988 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/testutils.py
+drwxrwxr-x   0 iqnus     (1000) iqnus     (1000)        0 2023-07-25 16:54:14.790809 iqnus-boleto-1.0.8/tests/xml/
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6190 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/BoletoBB-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6037 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/BoletoBanrisul-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6155 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/BoletoBradesco-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6153 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/BoletoCaixa-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6141 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/BoletoHsbc-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6196 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/BoletoHsbcComRegistro-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6232 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/BoletoItau-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6121 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/BoletoSantander-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6221 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/BoletoSicoob-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6197 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/BoletoSicredi-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17978 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoBB-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17519 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoBanrisul-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17873 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoBradesco-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17867 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoCaixa-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17831 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoHsbc-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17996 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoHsbcComRegistro-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    18104 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoItau-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17771 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoSantander-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)     6221 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoSicoob-expected.xml
+-rw-rw-r--   0 iqnus     (1000) iqnus     (1000)    17999 2023-07-25 16:24:39.000000 iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoSicredi-expected.xml
```

### Comparing `iqnus-boleto-1.0.7/LICENSE` & `iqnus-boleto-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/PKG-INFO` & `iqnus-boleto-1.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: iqnus-boleto
-Version: 1.0.7
-Summary: Python Library to create "boletos de cobrança bancária" for several Brazilian banks
+Version: 1.0.8
+Summary: Python Library to create "boletos de cobrança bancária" for     several Brazilian banks
 Home-page: https://github.com/Trust-Code/python-boleto
 Author: Trust-Code
 Author-email: suporte@trustcode.com.br
 License: BSD
-Download-URL: http://pypi.python.org/pypi/pyboleto
+Download-URL: https://github.com/luanpontes100/python-boleto
 Description: ================================================
         iqnus-boleto mantido por Iqnus Tecnologia
         ================================================
         
         .. _pyboleto-synopsis:
         
-        python-boleto é um projeto python para gerar boletos de cobrança.
+        iqnus-boleto é um projeto python para gerar boletos de cobrança.
         
         O projeto original pode ser encontrado aqui:
         https://github.com/eduardocereto/pyboleto
         
         
         .. contents::
             :local:
```

### Comparing `iqnus-boleto-1.0.7/README.rst` & `iqnus-boleto-1.0.8/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ================================================
 iqnus-boleto mantido por Iqnus Tecnologia
 ================================================
 
 .. _pyboleto-synopsis:
 
-python-boleto é um projeto python para gerar boletos de cobrança.
+iqnus-boleto é um projeto python para gerar boletos de cobrança.
 
 O projeto original pode ser encontrado aqui:
 https://github.com/eduardocereto/pyboleto
 
 
 .. contents::
     :local:
```

### Comparing `iqnus-boleto-1.0.7/bin/html_pyboleto_sample.py` & `iqnus-boleto-1.0.8/bin/html_pyboleto_sample.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/bin/pdf_pyboleto_sample.py` & `iqnus-boleto-1.0.8/bin/pdf_pyboleto_sample.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/iqnus_boleto.egg-info/PKG-INFO` & `iqnus-boleto-1.0.8/iqnus_boleto.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: iqnus-boleto
-Version: 1.0.7
-Summary: Python Library to create "boletos de cobrança bancária" for several Brazilian banks
+Version: 1.0.8
+Summary: Python Library to create "boletos de cobrança bancária" for     several Brazilian banks
 Home-page: https://github.com/Trust-Code/python-boleto
 Author: Trust-Code
 Author-email: suporte@trustcode.com.br
 License: BSD
-Download-URL: http://pypi.python.org/pypi/pyboleto
+Download-URL: https://github.com/luanpontes100/python-boleto
 Description: ================================================
         iqnus-boleto mantido por Iqnus Tecnologia
         ================================================
         
         .. _pyboleto-synopsis:
         
-        python-boleto é um projeto python para gerar boletos de cobrança.
+        iqnus-boleto é um projeto python para gerar boletos de cobrança.
         
         O projeto original pode ser encontrado aqui:
         https://github.com/eduardocereto/pyboleto
         
         
         .. contents::
             :local:
```

### Comparing `iqnus-boleto-1.0.7/iqnus_boleto.egg-info/SOURCES.txt` & `iqnus-boleto-1.0.8/iqnus_boleto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/__init__.py` & `iqnus-boleto-1.0.8/pyboleto/bank/__init__.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/bancodobrasil.py` & `iqnus-boleto-1.0.8/pyboleto/bank/bancodobrasil.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/banrisul.py` & `iqnus-boleto-1.0.8/pyboleto/bank/banrisul.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/bradesco.py` & `iqnus-boleto-1.0.8/pyboleto/bank/bradesco.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/caixa.py` & `iqnus-boleto-1.0.8/pyboleto/bank/caixa.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/caixa_sigcb.py` & `iqnus-boleto-1.0.8/pyboleto/bank/caixa_sigcb.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/cecred.py` & `iqnus-boleto-1.0.8/pyboleto/bank/cecred.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/hsbc.py` & `iqnus-boleto-1.0.8/pyboleto/bank/hsbc.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/itau.py` & `iqnus-boleto-1.0.8/pyboleto/bank/itau.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/santander.py` & `iqnus-boleto-1.0.8/pyboleto/bank/santander.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/sicoob.py` & `iqnus-boleto-1.0.8/pyboleto/bank/sicoob.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
     agencia_cedente = CustomProperty('agencia_cedente', 4)
     conta_cedente = CustomProperty('conta_cedente', 6)
     codigo_beneficiario = CustomProperty('codigo_beneficiario', 7)
     nosso_numero = CustomProperty('nosso_numero', 7)
 
     carteira = CustomProperty('carteira', 1)
+    parcela = CustomProperty('parcela', 3)
 
     def __init__(self):
         super(BoletoSicoob, self).__init__()
 
         self.codigo_banco = "756"
         self.logo_image = "logo_sicoob.jpg"
         self.especie_documento = 'DM'
@@ -57,9 +58,9 @@
     def campo_livre(self):
         content = "%1s%4s%2s%7s%7s%1s%3s" % (self.carteira,
                                              self.agencia_cedente.strip(),
                                              self.modalidade,
                                              self.codigo_beneficiario,
                                              self.nosso_numero[:7],
                                              self.dv_nosso_numero,
-                                             '001')
+                                             self.parcela)
         return content
```

### Comparing `iqnus-boleto-1.0.7/pyboleto/bank/sicredi.py` & `iqnus-boleto-1.0.8/pyboleto/bank/sicredi.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/data.py` & `iqnus-boleto-1.0.8/pyboleto/data.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/html.py` & `iqnus-boleto-1.0.8/pyboleto/html.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_bancobradesco.jpg` & `iqnus-boleto-1.0.8/pyboleto/media/logo_bancobradesco.jpg`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_bancocaixa.jpg` & `iqnus-boleto-1.0.8/pyboleto/media/logo_bancocaixa.jpg`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_bancohsbc.jpg` & `iqnus-boleto-1.0.8/pyboleto/media/logo_bancohsbc.jpg`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_bancoreal.jpg` & `iqnus-boleto-1.0.8/pyboleto/media/logo_bancoreal.jpg`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_banrisul.jpg` & `iqnus-boleto-1.0.8/pyboleto/media/logo_banrisul.jpg`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_bb.jpg` & `iqnus-boleto-1.0.8/pyboleto/media/logo_bb.jpg`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_cecred.jpg` & `iqnus-boleto-1.0.8/pyboleto/media/logo_cecred.jpg`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_itau.jpg` & `iqnus-boleto-1.0.8/pyboleto/media/logo_itau.jpg`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_santander.png` & `iqnus-boleto-1.0.8/pyboleto/media/logo_santander.png`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_sicoob.jpg` & `iqnus-boleto-1.0.8/pyboleto/media/logo_sicoob.jpg`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/media/logo_sicredi.png` & `iqnus-boleto-1.0.8/pyboleto/media/logo_sicredi.png`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/pdf.py` & `iqnus-boleto-1.0.8/pyboleto/pdf.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/templates/head.html` & `iqnus-boleto-1.0.8/pyboleto/templates/head.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/templates/recibo_caixa.html` & `iqnus-boleto-1.0.8/pyboleto/templates/recibo_caixa.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/pyboleto/templates/recibo_sacado.html` & `iqnus-boleto-1.0.8/pyboleto/templates/recibo_sacado.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/setup.py` & `iqnus-boleto-1.0.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,18 +33,19 @@
         'tests': ['xml/*.xml']
     },
     zip_safe=False,
     provides=[
         'pyboleto'
     ],
     license='BSD',
-    description='Python Library to create "boletos de cobrança bancária" for several Brazilian banks',
+    description='Python Library to create "boletos de cobrança bancária" for \
+    several Brazilian banks',
     long_description=read('README.rst'),
     long_description_content_type='text/x-rst',
-    download_url='http://pypi.python.org/pypi/pyboleto',
+    download_url='https://github.com/luanpontes100/python-boleto',
     scripts=[
         'bin/html_pyboleto_sample.py',
         'bin/pdf_pyboleto_sample.py'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Operating System :: OS Independent',
```

### Comparing `iqnus-boleto-1.0.7/tests/html/BoletoBB-expected.html` & `iqnus-boleto-1.0.8/tests/html/BoletoBB-expected.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/html/BoletoBanrisul-expected.html` & `iqnus-boleto-1.0.8/tests/html/BoletoBanrisul-expected.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/html/BoletoBradesco-expected.html` & `iqnus-boleto-1.0.8/tests/html/BoletoBradesco-expected.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/html/BoletoCaixa-expected.html` & `iqnus-boleto-1.0.8/tests/html/BoletoCaixa-expected.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/html/BoletoHsbc-expected.html` & `iqnus-boleto-1.0.8/tests/html/BoletoHsbc-expected.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/html/BoletoHsbcComRegistro-expected.html` & `iqnus-boleto-1.0.8/tests/html/BoletoHsbcComRegistro-expected.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/html/BoletoItau-expected.html` & `iqnus-boleto-1.0.8/tests/html/BoletoItau-expected.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/html/BoletoSantander-expected.html` & `iqnus-boleto-1.0.8/tests/html/BoletoSantander-expected.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/html/BoletoSicoob-expected.html` & `iqnus-boleto-1.0.8/tests/html/BoletoSicoob-expected.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/html/BoletoSicredi-expected.html` & `iqnus-boleto-1.0.8/tests/html/BoletoSicredi-expected.html`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/test_banco_banrisul.py` & `iqnus-boleto-1.0.8/tests/test_banco_banrisul.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/test_banco_bradesco.py` & `iqnus-boleto-1.0.8/tests/test_banco_bradesco.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/test_banco_caixa.py` & `iqnus-boleto-1.0.8/tests/test_banco_caixa.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/test_banco_do_brasil.py` & `iqnus-boleto-1.0.8/tests/test_banco_do_brasil.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/test_banco_hsbc.py` & `iqnus-boleto-1.0.8/tests/test_banco_hsbc.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/test_banco_hsbc_com_registro.py` & `iqnus-boleto-1.0.8/tests/test_banco_hsbc_com_registro.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/test_banco_itau.py` & `iqnus-boleto-1.0.8/tests/test_banco_itau.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/test_banco_santander.py` & `iqnus-boleto-1.0.8/tests/test_banco_santander.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/test_banco_sicoob.py` & `iqnus-boleto-1.0.8/tests/test_banco_sicoob.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/test_banco_sicredi.py` & `iqnus-boleto-1.0.8/tests/test_banco_sicredi.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/testutils.py` & `iqnus-boleto-1.0.8/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/BoletoBB-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/BoletoBB-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/BoletoBanrisul-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/BoletoBanrisul-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/BoletoBradesco-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/BoletoBradesco-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/BoletoCaixa-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/BoletoCaixa-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/BoletoHsbc-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/BoletoHsbc-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/BoletoHsbcComRegistro-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/BoletoHsbcComRegistro-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/BoletoItau-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/BoletoItau-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/BoletoSantander-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/BoletoSantander-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/BoletoSicoob-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/BoletoSicoob-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/BoletoSicredi-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/BoletoSicredi-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoBB-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoBB-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoBanrisul-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoBanrisul-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoBradesco-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoBradesco-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoCaixa-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoCaixa-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoHsbc-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoHsbc-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoHsbcComRegistro-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoHsbcComRegistro-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoItau-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoItau-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoSantander-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoSantander-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoSicoob-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoSicoob-expected.xml`

 * *Files identical despite different names*

### Comparing `iqnus-boleto-1.0.7/tests/xml/Triplo-BoletoSicredi-expected.xml` & `iqnus-boleto-1.0.8/tests/xml/Triplo-BoletoSicredi-expected.xml`

 * *Files identical despite different names*

