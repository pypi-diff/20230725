# Comparing `tmp/inewave-0.0.96.tar.gz` & `tmp/inewave-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inewave-0.0.96.tar", last modified: Tue Jun 13 20:15:29 2023, max compression
+gzip compressed data, was "inewave-0.0.97.tar", last modified: Tue Jul 25 00:12:29 2023, max compression
```

## Comparing `inewave-0.0.96.tar` & `inewave-0.0.97.tar`

### file list

```diff
@@ -1,659 +1,695 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:29.026776 inewave-0.0.96/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 20:08:26.000000 inewave-0.0.96/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-13 20:15:29.026776 inewave-0.0.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-13 20:08:26.000000 inewave-0.0.96/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.702771 inewave-0.0.96/inewave/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.702771 inewave-0.0.96/inewave/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/_utils/leituracsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.722771 inewave-0.0.96/inewave/newave/
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/abertura.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/bid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    75043 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/elnino.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)    42179 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/forwarh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/gee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/manutt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.790772 inewave-0.0.96/inewave/newave/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/abertura.py
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/agrint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/arquivos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.790772 inewave-0.0.96/inewave/newave/modelos/arquivoscsv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/arquivoscsv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/arquivoscsv/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/bid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.790772 inewave-0.0.96/inewave/newave/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/clasgas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    30466 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)   135879 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/elnino.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/ensoaux.py
--rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/expt.py
--rw-r--r--   0 runner    (1001) docker     (123)    87572 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/forwarh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/gee.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/ghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/gtminpat.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/itaipu.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/manutt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16085 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/perda.py
--rw-r--r--   0 runner    (1001) docker     (123)    24454 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/tecno.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modelos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15833 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/perda.py
--rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/sar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/shist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/tecno.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/newave/vazpast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.790772 inewave-0.0.96/inewave/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/estados.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.790772 inewave-0.0.96/inewave/nwlistcf/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/modelos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/modelos/estados.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/modelos/nwlistcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistcf/nwlistcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.830773 inewave-0.0.96/inewave/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/merclsin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.854773 inewave-0.0.96/inewave/nwlistop/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.858773 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoree.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivousina.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.858773 inewave-0.0.96/inewave/nwlistop/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/parsubmercados.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/submercado.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/usina.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/valoresserie.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/def.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dflppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dflpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/modelos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/nwlistop/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/inewave/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.702771 inewave-0.0.96/inewave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-13 20:15:28.000000 inewave-0.0.96/inewave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20208 2023-06-13 20:15:28.000000 inewave-0.0.96/inewave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:15:28.000000 inewave-0.0.96/inewave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 20:15:28.000000 inewave-0.0.96/inewave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 20:15:28.000000 inewave-0.0.96/inewave.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:15:29.026776 inewave-0.0.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-13 20:08:26.000000 inewave-0.0.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.858773 inewave-0.0.96/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.858773 inewave-0.0.96/tests/_arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/_arquivos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.858773 inewave-0.0.96/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:28.982775 inewave-0.0.96/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)    46951 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    30063 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/clast.py
--rw-r--r--   0 runner    (1001) docker     (123)   847210 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)   295249 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/conft.py
--rw-r--r--   0 runner    (1001) docker     (123)   295245 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/coper.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105146 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)   295190 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)   295196 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   847164 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dger.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)   120243 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)   267099 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267152 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)   267153 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267144 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)   291239 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)   291240 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicaconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/estados.py
--rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/evert.py
--rw-r--r--   0 runner    (1001) docker     (123)   267138 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104654 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/exces.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/exph.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104650 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105178 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/geol.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105179 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105181 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   847144 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105136 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105139 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105141 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105140 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105189 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105190 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)    49768 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105188 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105191 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1087195 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/invade.py
--rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)    56692 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/modif.py
--rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)    76518 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/nwlistcf.py
--rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)   378349 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/parp.py
--rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)   267136 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   380918 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/term.py
--rw-r--r--   0 runner    (1001) docker     (123)   271157 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)   283139 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   283209 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vazpast.py
--rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vento.py
--rw-r--r--   0 runner    (1001) docker     (123)   847200 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267158 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)   267117 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105173 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105174 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)  1105176 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)   847195 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)   847135 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/arquivos/vturuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/mocks/mock_open.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:29.002776 inewave-0.0.96/tests/newave/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_adterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_arquivos.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_avl_cortesfpha_nwv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_avl_desvfpha_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_avl_desvfpha_v_q.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_cadic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_caso.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_clast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_confhd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_conft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_cortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_cortesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_curva.py
--rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_cvar.py
--rw-r--r--   0 runner    (1001) docker     (123)    49743 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_dger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_dsvagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eafpast.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_enavazb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_enavazf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_energiab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_energiaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_energias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_engnat.py
--rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicacadastro.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicaconfiguracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicafte.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicageracao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicahistorico.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicaposto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_eolicasubmercado.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_exph.py
--rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_forwarh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6257 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_modif.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_newavetim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_nwv_avl_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_nwv_cortes_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_nwv_eco_evap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_parp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_parpeol.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_parpvaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_patamar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_penalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_pmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_ree.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_restricaoeletrica.py
--rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_restricaoenergia.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_restricaovazao.py
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_sistema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_term.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_vazaob.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_vazaof.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_vazaos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_vazoes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/newave/test_vazpast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:29.006775 inewave-0.0.96/tests/nwlistcf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistcf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistcf/test_estados.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistcf/test_nwlistcf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:15:29.026776 inewave-0.0.96/tests/nwlistop/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_cdef.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_cdefsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_cmarg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_cmargmed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_coper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_corteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_cterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ctermsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_deficit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_defsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_depminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dfphauh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlppdfmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlppdfmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlppdfmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlpptbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlpptbmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dlpptbmaxs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dtbmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dtbmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_dvazmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_eaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_eafb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_eafbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_eafbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_eafm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmfp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmfpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmfpsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_earmfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_evert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_evertm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_evertsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_exces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_excessin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_fteolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_fteolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_geol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_geolm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_geolsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghiduh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmaxm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmaxmr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmaxr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmaxrsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghmaxsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghtot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghtotm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_ghtotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_gttot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_gttotsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_intercambio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_invade.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_invadem.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_mediasmerc.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_mediassin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_mercl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_merclsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_perdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_perdfm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_perdfsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_qafluh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_qincruh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_rhslppdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_rhslpptb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vagua.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_varmpuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_varmuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vento.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vertuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_verturb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_verturbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_verturbsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vevmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vevminm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vevminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vghmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vghminm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vghminsin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vghminuh.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-13 20:08:26.000000 inewave-0.0.96/tests/nwlistop/test_vturuh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:29.032600 inewave-0.0.97/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 00:08:24.000000 inewave-0.0.97/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-25 00:12:29.032600 inewave-0.0.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-07-25 00:08:24.000000 inewave-0.0.97/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.860597 inewave-0.0.97/inewave/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.860597 inewave-0.0.97/inewave/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/_utils/leituracsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.868597 inewave-0.0.97/inewave/newave/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16603 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/bid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13918 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75043 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6701 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42179 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10812 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/gee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/manutt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.880597 inewave-0.0.97/inewave/newave/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/abertura.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/arquivos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.880597 inewave-0.0.97/inewave/newave/modelos/arquivoscsv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/arquivoscsv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/arquivoscsv/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/bid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.880597 inewave-0.0.97/inewave/newave/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/blocos/versaomodelo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/clasgas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30466 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13124 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135879 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2836 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/elnino.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/ensoaux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10108 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87572 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/gee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/gtminpat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/itaipu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30568 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17460 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/perda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24454 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6198 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20506 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modelos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15914 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19155 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15903 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/perda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7300 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/sar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6668 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/tecno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/newave/vazpast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.880597 inewave-0.0.97/inewave/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8174 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/estados.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.880597 inewave-0.0.97/inewave/nwlistcf/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/modelos/nwlistcfrel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistcf/nwlistcfrel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.892598 inewave-0.0.97/inewave/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/merclsin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.904598 inewave-0.0.97/inewave/nwlistop/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.904598 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivousina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.904598 inewave-0.0.97/inewave/nwlistop/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/parsubmercados.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/submercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/usina.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresserie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/def.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dflppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dflpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/modelos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/nwlistop/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/inewave/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.860597 inewave-0.0.97/inewave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-25 00:12:28.000000 inewave-0.0.97/inewave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21445 2023-07-25 00:12:28.000000 inewave-0.0.97/inewave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 00:12:28.000000 inewave-0.0.97/inewave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-25 00:12:28.000000 inewave-0.0.97/inewave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 00:12:28.000000 inewave-0.0.97/inewave.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 00:12:29.032600 inewave-0.0.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-25 00:08:24.000000 inewave-0.0.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.908598 inewave-0.0.97/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.908598 inewave-0.0.97/tests/_arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/_arquivos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.908598 inewave-0.0.97/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:28.996600 inewave-0.0.97/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/arquivos_nwlistcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46951 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/caso_nwlistcf_nwlistop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30063 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847210 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295249 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295245 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105146 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295190 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   295196 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847164 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105161 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105169 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105154 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120243 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267099 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267152 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267153 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267144 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291239 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   291240 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14002 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicaconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56476 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267138 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104654 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120990 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104650 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1104652 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105178 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105179 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105181 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847144 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105136 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105139 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105138 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105141 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105140 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105189 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105190 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49768 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16887 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105188 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105191 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1087195 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49720 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57012 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45543 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76521 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwlistcfrel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9502 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12629 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10775 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)   378349 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50087 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38585 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52098 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267136 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267137 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267139 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   380918 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283145 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105160 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)   271157 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283139 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   283209 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32259 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vazpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267101 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847200 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267155 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267156 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267158 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267122 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267130 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)   267117 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105173 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105174 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1105176 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847195 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)   847135 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/arquivos/vturuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:29.012600 inewave-0.0.97/tests/newave/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_adterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_agrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_avl_cortesfpha_nwv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_avl_desvfpha_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_avl_desvfpha_v_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_cadic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_clast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_confhd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_conft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_cortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_cortesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_curva.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3215 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_cvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49743 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_dger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_dsvagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eafpast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_enavazb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_enavazf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_energiab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_energiaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_energias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_engnat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7992 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicacadastro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicaconfiguracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicafte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicageracao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicahistorico.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicaposto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_eolicasubmercado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_exph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_expt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36320 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_forwarh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_ghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_manutt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_modif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_newavetim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_nwv_avl_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_nwv_cortes_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_nwv_eco_evap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7495 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_parp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_parpeol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_parpvaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_patamar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_penalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_pmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_ree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_restricaoeletrica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_restricaoenergia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_restricaovazao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_selcor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_shist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_sistema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_vazaob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_vazaof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_vazaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_vazoes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/newave/test_vazpast.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:29.012600 inewave-0.0.97/tests/nwlistcf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/test_arquivos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/test_caso.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/test_estados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/test_nwlistcfdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistcf/test_nwlistcfrel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 00:12:29.032600 inewave-0.0.97/tests/nwlistop/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_cdef.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_cdefsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_cmarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_cmargmed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_coper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_corteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_cterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ctermsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_deficit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_defsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_depminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dfphauh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlppdfmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlppdfmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlppdfmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlpptbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlpptbmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dlpptbmaxs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dtbmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dtbmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_dvazmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_eaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_eafb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_eafbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_eafbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_eafm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmfp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmfpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmfpsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_earmfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_evert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_evertm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_evertsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_exces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_excessin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_fteolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_fteolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_geol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_geolm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_geolsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghiduh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmaxm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmaxmr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmaxr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmaxrsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghmaxsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghtot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghtotm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_ghtotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_gtert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_gttot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_gttotsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_intercambio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_invade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_invadem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_mediasmerc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_mediassin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_mercl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_merclsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_nwlistopdat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_perdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_perdfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_perdfsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_qafluh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_qincruh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_rhslppdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_rhslpptb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vagua.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_varmpuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_varmuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vento.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vertuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_verturb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_verturbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_verturbsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vevmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vevminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vevminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vghmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vghminm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vghminsin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vghminuh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-25 00:08:24.000000 inewave-0.0.97/tests/nwlistop/test_vturuh.py
```

### Comparing `inewave-0.0.96/LICENSE.md` & `inewave-0.0.97/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/PKG-INFO` & `inewave-0.0.97/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 0.0.96
+Version: 0.0.97
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-0.0.96/README.md` & `inewave-0.0.97/README.md`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/_utils/leituracsv.py` & `inewave-0.0.97/inewave/_utils/leituracsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/config.py` & `inewave-0.0.97/inewave/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 MAX_SERIES_SINTETICAS = 2000
 MAX_PATAMARES = 5
 NUM_CENARIOS = 2000
+MAX_AGRUPAMENTOS_INTERCAMBIOS = 20
 MAX_ANOS_ESTUDO = 30
 MAX_ANOS_HISTORICO = 100
 MAX_CONFIGURACOES = 360
 MAX_SUBMERCADOS = 15
 MAX_ITERS = 100
 MAX_FORWARDS = 300
 MAX_CORTES = MAX_ITERS * MAX_FORWARDS
```

### Comparing `inewave-0.0.96/inewave/newave/__init__.py` & `inewave-0.0.97/inewave/newave/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Inclui os membros
 
 from .abertura import Abertura  # noqa
 from .adterm import AdTerm  # noqa
-from .agrint import AgrInt  # noqa
+from .agrint import Agrint  # noqa
 from .arquivos import Arquivos  # noqa
 from .bid import BID  # noqa
 from .cadic import CAdic  # noqa
 from .caso import Caso  # noqa
 from .clasgas import ClasGas  # noqa
 from .clast import ClasT  # noqa
 from .confhd import Confhd  # noqa
@@ -17,32 +17,33 @@
 from .dsvagua import DSVAgua  # noqa
 from .eafpast import EafPast  # noqa
 from .elnino import ElNino  # noqa
 from .ensoaux import ENSOAux  # noqa
 from .exph import Exph  # noqa
 from .expt import Expt  # noqa
 from .gee import GEE  # noqa
-from .ghmin import GHMin  # noqa
+from .ghmin import Ghmin  # noqa
 from .gtminpat import GTMinPat  # noqa
 from .hidr import Hidr  # noqa
 from .itaipu import Itaipu  # noqa
-from .manutt import ManutT  # noqa
+from .manutt import Manutt  # noqa
 from .modif import Modif  # noqa
 from .newavetim import NewaveTim  # noqa
 from .parp import PARp  # noqa
 from .parpvaz import PARpvaz  # noqa
 from .parpeol import PARpeol  # noqa
 from .patamar import Patamar  # noqa
 from .penalid import Penalid  # noqa
 from .perda import Perda  # noqa
 from .pmo import PMO  # noqa
 from .re import RE  # noqa
 from .ree import REE  # noqa
 from .sar import SAR  # noqa
 from .shist import Shist  # noqa
+from .selcor import Selcor  # noqa
 from .sistema import Sistema  # noqa
 from .tecno import Tecno  # noqa
 from .term import Term  # noqa
 from .vazoes import Vazoes  # noqa
 from .vazpast import VazPast  # noqa
 from .eolicacadastro import EolicaCadastro  # noqa
 from .eolicaconfiguracao import EolicaConfiguracao  # noqa
```

### Comparing `inewave-0.0.96/inewave/newave/abertura.py` & `inewave-0.0.97/inewave/newave/abertura.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/adterm.py` & `inewave-0.0.97/inewave/newave/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/agrint.py` & `inewave-0.0.97/inewave/newave/itaipu.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from typing import TypeVar, List, Type
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class AgrInt(SectionFile):
+class Itaipu(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes aos agrupamentos
-    livres de intercâmbio.
+    Armazena os dados de entrada do NEWAVE referentes às restrições
+    de Itaipu.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="agrint.dat") -> "AgrInt":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="itaipu.dat") -> "Itaipu":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="agrint.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="itaipu.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/newave/arquivos.py` & `inewave-0.0.97/inewave/newave/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/avl_cortesfpha_nwv.py` & `inewave-0.0.97/inewave/newave/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/avl_desvfpha_s.py` & `inewave-0.0.97/inewave/newave/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/avl_desvfpha_v_q.py` & `inewave-0.0.97/inewave/newave/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/bid.py` & `inewave-0.0.97/inewave/newave/bid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/cadic.py` & `inewave-0.0.97/inewave/newave/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/caso.py` & `inewave-0.0.97/inewave/newave/caso.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,19 +6,18 @@
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
 class Caso(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às
-    configurações das usinas hidrelétricas.
+    Armazena os dados de entrada do NEWAVE referentes ao caso de estudo.
 
     Esta classe lida com informações de entrada fornecidas ao NEWAVE e
-    que podem ser modificadas através do arquivo `modif.dat`.
+    que podem ser modificadas através do arquivo `caso.dat`.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS = [NomeCaso, CaminhoGerenciadorProcessos]
```

### Comparing `inewave-0.0.96/inewave/newave/clasgas.py` & `inewave-0.0.97/inewave/newave/clasgas.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/clast.py` & `inewave-0.0.97/inewave/newave/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/confhd.py` & `inewave-0.0.97/inewave/newave/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/conft.py` & `inewave-0.0.97/inewave/newave/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/cortes.py` & `inewave-0.0.97/inewave/newave/cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/cortesh.py` & `inewave-0.0.97/inewave/newave/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/curva.py` & `inewave-0.0.97/inewave/newave/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/cvar.py` & `inewave-0.0.97/inewave/newave/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/dger.py` & `inewave-0.0.97/inewave/newave/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/dsvagua.py` & `inewave-0.0.97/inewave/newave/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/eafpast.py` & `inewave-0.0.97/inewave/newave/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/elnino.py` & `inewave-0.0.97/inewave/newave/elnino.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/enavazb.py` & `inewave-0.0.97/inewave/newave/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/enavazf.py` & `inewave-0.0.97/inewave/newave/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/energiab.py` & `inewave-0.0.97/inewave/newave/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/energiaf.py` & `inewave-0.0.97/inewave/newave/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/energias.py` & `inewave-0.0.97/inewave/newave/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/engnat.py` & `inewave-0.0.97/inewave/newave/engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/ensoaux.py` & `inewave-0.0.97/inewave/newave/ensoaux.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/eolicacadastro.py` & `inewave-0.0.97/inewave/newave/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/eolicaconfiguracao.py` & `inewave-0.0.97/inewave/newave/eolicaconfiguracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/eolicafte.py` & `inewave-0.0.97/inewave/newave/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/eolicageracao.py` & `inewave-0.0.97/inewave/newave/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/eolicahistorico.py` & `inewave-0.0.97/inewave/newave/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/eolicaposto.py` & `inewave-0.0.97/inewave/newave/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/eolicasubmercado.py` & `inewave-0.0.97/inewave/newave/eolicasubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/exph.py` & `inewave-0.0.97/inewave/newave/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/expt.py` & `inewave-0.0.97/inewave/newave/tecno.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from typing import TypeVar, List, Type
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Expt(SectionFile):
+class Tecno(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes à expansão
-    térmica do sistema.
+    Armazena os dados de entrada do NEWAVE referentes às tecnologias
+    disponíveis para geração de energia.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="expt.dat") -> "Expt":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="tecno.dat") -> "Tecno":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="expt.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="tecno.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/newave/forward.py` & `inewave-0.0.97/inewave/newave/forward.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/forwarh.py` & `inewave-0.0.97/inewave/newave/forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/gee.py` & `inewave-0.0.97/inewave/newave/gee.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/ghmin.py` & `inewave-0.0.97/inewave/newave/gtminpat.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,38 +3,40 @@
 from typing import TypeVar, List, Type
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class GHMin(SectionFile):
+class GTMinPat(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes à geração hidráulica
-    mínima por usina.
+    Armazena os dados de entrada do NEWAVE referentes à geração térmica
+    mínima por patamar.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="ghmin.dat") -> "GHMin":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="gtminpat.dat"
+    ) -> "GTMinPat":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="ghmin.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="gtminpat.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/newave/gtminpat.py` & `inewave-0.0.97/inewave/newave/perda.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,40 +3,38 @@
 from typing import TypeVar, List, Type
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class GTMinPat(SectionFile):
+class Perda(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes à geração térmica
-    mínima por patamar.
+    Armazena os dados de entrada do NEWAVE referentes aos fatores de perda
+    das usinas e das interligações.
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="gtminpat.dat"
-    ) -> "GTMinPat":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="perda.dat") -> "Perda":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="gtminpat.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="perda.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/newave/hidr.py` & `inewave-0.0.97/inewave/newave/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/itaipu.py` & `inewave-0.0.97/inewave/newave/sar.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 from typing import TypeVar, List, Type
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Itaipu(SectionFile):
+class SAR(SectionFile):
     """
-    Armazena os dados de entrada do NEWAVE referentes às restrições
-    de Itaipu.
+    Armazena os dados de entrada do NEWAVE referentes à superfície de
+    aversão à risco (SAR).
 
     """
 
     T = TypeVar("T")
 
     SECTIONS: List[Type[Section]] = []
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="itaipu.dat") -> "Itaipu":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="sar.dat") -> "SAR":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
 
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="itaipu.dat"):
+    def escreve_arquivo(self, diretorio: str, nome_arquivo="sar.dat"):
         msg = (
             "O método escreve_arquivo(diretorio, nome_arquivo) será"
             + " descontinuado na versão 1.0.0 -"
             + " use o método write(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/newave/manutt.py` & `inewave-0.0.97/inewave/nwlistop/cdefsin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,34 @@
-from cfinterface.files.sectionfile import SectionFile
-from cfinterface.components.section import Section
-from typing import TypeVar, List, Type
+from inewave.nwlistop.modelos.cdefsin import CdefAnos
+
+from inewave.nwlistop.modelos.arquivos.arquivosin import (
+    ArquivoSIN,
+)
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class ManutT(SectionFile):
+class CdefSIN(ArquivoSIN):
     """
-    Armazena os dados de entrada do NEWAVE referentes à programação
-    da manutenção das usinas térmicas.
+    Armazena os dados das saídas referentes ao custo de déficit
+    de cada estágio em cada série.
 
+    Esta classe lida com as informações de saída fornecidas pelo
+    NWLISTOP e reproduzidas nos `cdefsin.out`.
     """
 
-    T = TypeVar("T")
-
-    SECTIONS: List[Type[Section]] = []
-
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
+    BLOCKS = [
+        CdefAnos,
+    ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="manutt.dat") -> "ManutT":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="cdefsin.out"
+    ) -> "CdefSIN":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="manutt.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/newave/modelos/adterm.py` & `inewave-0.0.97/inewave/newave/modelos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/arquivos.py` & `inewave-0.0.97/inewave/newave/modelos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/arquivoscsv/arquivocsv.py` & `inewave-0.0.97/inewave/newave/modelos/arquivoscsv/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/avl_cortesfpha_nwv.py` & `inewave-0.0.97/inewave/newave/modelos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/avl_desvfpha_s.py` & `inewave-0.0.97/inewave/newave/modelos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/avl_desvfpha_v_q.py` & `inewave-0.0.97/inewave/newave/modelos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/blocos/tabelacsv.py` & `inewave-0.0.97/inewave/newave/modelos/blocos/tabelacsv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/blocos/versaomodelo.py` & `inewave-0.0.97/inewave/newave/modelos/blocos/versaomodelo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/cadic.py` & `inewave-0.0.97/inewave/newave/modelos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/caso.py` & `inewave-0.0.97/inewave/newave/modelos/caso.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/clast.py` & `inewave-0.0.97/inewave/newave/modelos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/confhd.py` & `inewave-0.0.97/inewave/newave/modelos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/conft.py` & `inewave-0.0.97/inewave/newave/modelos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/cortes.py` & `inewave-0.0.97/inewave/newave/modelos/cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/cortesh.py` & `inewave-0.0.97/inewave/newave/modelos/cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/curva.py` & `inewave-0.0.97/inewave/newave/modelos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/cvar.py` & `inewave-0.0.97/inewave/newave/modelos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/dger.py` & `inewave-0.0.97/inewave/newave/modelos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/dsvagua.py` & `inewave-0.0.97/inewave/newave/modelos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/eafpast.py` & `inewave-0.0.97/inewave/newave/modelos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/enavazb.py` & `inewave-0.0.97/inewave/newave/modelos/enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/enavazf.py` & `inewave-0.0.97/inewave/newave/modelos/enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/energiab.py` & `inewave-0.0.97/inewave/newave/modelos/energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/energiaf.py` & `inewave-0.0.97/inewave/newave/modelos/energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/energias.py` & `inewave-0.0.97/inewave/newave/modelos/energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/engnat.py` & `inewave-0.0.97/inewave/newave/modelos/engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/eolicacadastro.py` & `inewave-0.0.97/inewave/newave/modelos/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/eolicaconfiguracao.py` & `inewave-0.0.97/inewave/newave/modelos/eolicaconfiguracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/eolicafte.py` & `inewave-0.0.97/inewave/newave/modelos/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/eolicageracao.py` & `inewave-0.0.97/inewave/newave/modelos/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/eolicahistorico.py` & `inewave-0.0.97/inewave/newave/modelos/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/eolicaposto.py` & `inewave-0.0.97/inewave/newave/modelos/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/eolicasubmercado.py` & `inewave-0.0.97/inewave/newave/modelos/eolicasubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/exph.py` & `inewave-0.0.97/inewave/newave/modelos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/forward.py` & `inewave-0.0.97/inewave/newave/modelos/forward.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/forwarh.py` & `inewave-0.0.97/inewave/newave/modelos/forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/hidr.py` & `inewave-0.0.97/inewave/newave/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/modif.py` & `inewave-0.0.97/inewave/newave/modelos/modif.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,84 +49,82 @@
     """
     Registro que contém uma modificação de volume mínimo
     operativo para uma usina.
     """
 
     IDENTIFIER = " VOLMIN"
     IDENTIFIER_DIGITS = 8
-    LINE = Line([LiteralField(30, 10)])
-    # LINE = Line([FloatField(15, 10, 2), LiteralField(3, 26)])
+    LINE = Line([FloatField(8, 10, 2), LiteralField(3, 19)])
 
-    # @property
-    # def volume(self) -> Optional[float]:
-    #     """
-    #     O novo valor de volume
-
-    #     :return: O novo valor de volume
-    #     :rtype: Optional[float]
-    #     """
-    #     return self.data[0]
-
-    # @volume.setter
-    # def volume(self, t: float):
-    #     self.data[0] = t
-
-    # @property
-    # def unidade(self) -> Optional[str]:
-    #     """
-    #     A unidade do volume informado
-
-    #     :return: A unidade do volume
-    #     :rtype: Optional[str]
-    #     """
-    #     return self.data[1]
-
-    # @unidade.setter
-    # def unidade(self, t: str):
-    #     self.data[1] = t
+    @property
+    def volume(self) -> Optional[float]:
+        """
+        O novo valor de volume
+
+        :return: O novo valor de volume
+        :rtype: Optional[float]
+        """
+        return self.data[0]
+
+    @volume.setter
+    def volume(self, t: float):
+        self.data[0] = t
+
+    @property
+    def unidade(self) -> Optional[str]:
+        """
+        A unidade do volume informado
+
+        :return: A unidade do volume
+        :rtype: Optional[str]
+        """
+        return self.data[1]
+
+    @unidade.setter
+    def unidade(self, t: str):
+        self.data[1] = t
 
 
 class VOLMAX(Register):
     """
     Registro que contém uma modificação de volume máximo
     operativo para uma usina.
     """
 
     IDENTIFIER = " VOLMAX"
     IDENTIFIER_DIGITS = 8
-    LINE = Line([LiteralField(30, 10)])
-    # LINE = Line([FloatField(15, 10, 2), LiteralField(3, 26)])
+    LINE = Line([FloatField(6, 10, 3), LiteralField(3, 17)])
+
+    @property
+    def volume(self) -> Optional[float]:
+        """
+        O novo valor de volume
+
+        :return: O novo valor de volume
+        :rtype: Optional[float]
+        """
+        return self.data[0]
+
+    @volume.setter
+    def volume(self, t: float):
+        self.data[0] = t
+
+    @property
+    def unidade(self) -> Optional[str]:
+        """
+        A unidade do volume informado
+
+        :return: A unidade do volume
+        :rtype: Optional[str]
+        """
+        return self.data[1]
 
-    # @property
-    # def volume(self) -> Optional[float]:
-    #     """
-    #     O novo valor de volume
-
-    #     :return: O novo valor de volume
-    #     :rtype: Optional[float]
-    #     """
-    #     return self.data[0]
-
-    # @volume.setter
-    # def volume(self, t: float):
-    #     self.data[0] = t
-
-    # @property
-    # def unidade(self) -> Optional[str]:
-    #     """
-    #     A unidade do volume informado
-
-    #     :return: A unidade do volume
-    #     :rtype: Optional[str]
-    #     """
-    #     return self.data[1]
-
-    # @unidade.setter
-    # def unidade(self, t: str):
-    #     self.data[1] = t
+    @unidade.setter
+    def unidade(self, t: str):
+        self.data[1] = t
 
 
 class NUMCNJ(Register):
     """
     Registro que contém uma modificação de número de conjunto
     de máquinas.
     """
@@ -664,15 +662,15 @@
 class TURBMAXT(Register):
     """
     Registro que contém uma modificação da turbinamento máximo
     com data.
     """
 
     IDENTIFIER = " TURBMAXT"
-    IDENTIFIER_DIGITS = 8
+    IDENTIFIER_DIGITS = 9
     LINE = Line(
         [
             IntegerField(2, 10),
             IntegerField(4, 13),
             FloatField(7, 18, 2),
         ]
     )
@@ -723,15 +721,15 @@
 class TURBMINT(Register):
     """
     Registro que contém uma modificação da turbinamento mínimo
     com data.
     """
 
     IDENTIFIER = " TURBMINT"
-    IDENTIFIER_DIGITS = 8
+    IDENTIFIER_DIGITS = 9
     LINE = Line(
         [
             IntegerField(2, 10),
             IntegerField(4, 13),
             FloatField(7, 18, 2),
         ]
     )
```

### Comparing `inewave-0.0.96/inewave/newave/modelos/newavetim.py` & `inewave-0.0.97/inewave/newave/modelos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/nwv_avl_evap.py` & `inewave-0.0.97/inewave/newave/modelos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/nwv_cortes_evap.py` & `inewave-0.0.97/inewave/newave/modelos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/nwv_eco_evap.py` & `inewave-0.0.97/inewave/newave/modelos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/parp.py` & `inewave-0.0.97/inewave/newave/modelos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/parpeol.py` & `inewave-0.0.97/inewave/newave/modelos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/parpvaz.py` & `inewave-0.0.97/inewave/newave/modelos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/patamar.py` & `inewave-0.0.97/inewave/newave/modelos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/penalid.py` & `inewave-0.0.97/inewave/newave/modelos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/pmo.py` & `inewave-0.0.97/inewave/newave/modelos/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/re.py` & `inewave-0.0.97/inewave/newave/modelos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/ree.py` & `inewave-0.0.97/inewave/newave/modelos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/restricaoeletrica.py` & `inewave-0.0.97/inewave/newave/modelos/restricaoeletrica.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/restricaoenergia.py` & `inewave-0.0.97/inewave/newave/modelos/restricaoenergia.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/restricaovazao.py` & `inewave-0.0.97/inewave/newave/modelos/restricaovazao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/sistema.py` & `inewave-0.0.97/inewave/newave/modelos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/term.py` & `inewave-0.0.97/inewave/newave/modelos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/vazaob.py` & `inewave-0.0.97/inewave/newave/modelos/vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/vazaof.py` & `inewave-0.0.97/inewave/newave/modelos/vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/vazaos.py` & `inewave-0.0.97/inewave/newave/modelos/vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/vazoes.py` & `inewave-0.0.97/inewave/newave/modelos/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modelos/vazpast.py` & `inewave-0.0.97/inewave/newave/modelos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/modif.py` & `inewave-0.0.97/inewave/newave/modif.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from cfinterface.components.register import Register
 from cfinterface.files.registerfile import RegisterFile
 from inewave.newave.modelos.modif import (
-    TURBMAXT,
-    TURBMINT,
     USINA,
-    VAZMAXT,
     VOLMIN,
     VOLMAX,
     NUMCNJ,
     NUMMAQ,
     VAZMIN,
     CFUGA,
     CMONT,
     VMAXT,
     VMINT,
     VMINP,
     VAZMINT,
+    VAZMAXT,
+    TURBMAXT,
+    TURBMINT,
 )
 
 
 from typing import Type, TypeVar, List, Optional, Union
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
@@ -43,14 +43,17 @@
         VAZMIN,
         CFUGA,
         CMONT,
         VMAXT,
         VMINT,
         VMINP,
         VAZMINT,
+        VAZMAXT,
+        TURBMAXT,
+        TURBMINT,
     ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(cls, diretorio: str, nome_arquivo="modif.dat") -> "Modif":
@@ -416,16 +419,16 @@
         """
         Obtém um registro que define o turbinamento máximo por período.
 
         :param mes: mês de validade do turbinamento
         :type mes: int | None
         :param ano: ano de validade do turbinamento
         :type ano: int | None
-        :param vazao: o turbinamento máximo
-        :type vazao: float | None
+        :param turbinamento: o turbinamento máximo
+        :type turbinamento: float | None
         :return: Um ou mais registros, se existirem.
         :rtype: :class:`TURBMAXT` | list[:class:`TURBMAXT`] | None
         """
         return self.__obtem_registros_com_filtros(
             TURBMAXT, mes=mes, ano=ano, turbinamento=turbinamento
         )
 
@@ -437,16 +440,16 @@
     ) -> Optional[Union[TURBMINT, List[TURBMINT]]]:
         """
         Obtém um registro que define o turbinamento mínimo por período.
         :param mes: mês de validade do turbinamento
         :type mes: int | None
         :param ano: ano de validade do turbinamento
         :type ano: int | None
-        :param vazao: o turbinamento mínimo
-        :type vazao: float | None
+        :param turbinamento: o turbinamento mínimo
+        :type turbinamento: float | None
         :return: Um ou mais registros, se existirem.
         :rtype: :class:`TURBMINT` | list[:class:`TURBMINT`] | None
         """
         return self.__obtem_registros_com_filtros(
             TURBMINT, mes=mes, ano=ano, turbinamento=turbinamento
         )
```

### Comparing `inewave-0.0.96/inewave/newave/newavetim.py` & `inewave-0.0.97/inewave/newave/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/nwv_avl_evap.py` & `inewave-0.0.97/inewave/newave/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/nwv_cortes_evap.py` & `inewave-0.0.97/inewave/newave/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/nwv_eco_evap.py` & `inewave-0.0.97/inewave/newave/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/parp.py` & `inewave-0.0.97/inewave/newave/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/parpeol.py` & `inewave-0.0.97/inewave/newave/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/parpvaz.py` & `inewave-0.0.97/inewave/newave/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/patamar.py` & `inewave-0.0.97/inewave/newave/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/penalid.py` & `inewave-0.0.97/inewave/newave/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/perda.py` & `inewave-0.0.97/inewave/nwlistop/ghmaxrsin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,33 @@
-from cfinterface.files.sectionfile import SectionFile
-from cfinterface.components.section import Section
-from typing import TypeVar, List, Type
+from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
+    ArquivoSINPatamar,
+)
+from inewave.nwlistop.modelos.ghmaxrsin import GHAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Perda(SectionFile):
+class GhmaxrSIN(ArquivoSINPatamar):
     """
-    Armazena os dados de entrada do NEWAVE referentes aos fatores de perda
-    das usinas e das interligações.
+    Armazena os dados das saídas referentes à geração hidraulica máxima
+    considerando restrições elétricas por patamar para o SIN.
 
+    Esta classe lida com as informações de saída fornecidas pelo
+    NWLISTOP e reproduzidas nos `ghmaxsin.out`.
     """
 
-    T = TypeVar("T")
-
-    SECTIONS: List[Type[Section]] = []
-
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
+    BLOCKS = [
+        GHAnos,
+    ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="perda.dat") -> "Perda":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="ghmaxrsin.out"
+    ) -> "GhmaxrSIN":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="perda.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/newave/pmo.py` & `inewave-0.0.97/inewave/newave/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/re.py` & `inewave-0.0.97/inewave/newave/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/ree.py` & `inewave-0.0.97/inewave/newave/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/restricaoeletrica.py` & `inewave-0.0.97/inewave/newave/restricaoeletrica.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/restricaoenergia.py` & `inewave-0.0.97/inewave/newave/restricaoenergia.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/restricaovazao.py` & `inewave-0.0.97/inewave/newave/restricaovazao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/sar.py` & `inewave-0.0.97/inewave/nwlistop/merclsin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,34 @@
-from cfinterface.files.sectionfile import SectionFile
-from cfinterface.components.section import Section
-from typing import TypeVar, List, Type
+from inewave.nwlistop.modelos.merclsin import MerclAnos
+
+from inewave.nwlistop.modelos.arquivos.arquivosin import (
+    ArquivoSIN,
+)
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class SAR(SectionFile):
+class MerclSIN(ArquivoSIN):
     """
-    Armazena os dados de entrada do NEWAVE referentes à superfície de
-    aversão à risco (SAR).
+    Armazena os dados das saídas referentes ao mercado líquido
+    de cada estágio em cada série.
 
+    Esta classe lida com as informações de saída fornecidas pelo
+    NWLISTOP e reproduzidas nos `merclsin.out`.
     """
 
-    T = TypeVar("T")
-
-    SECTIONS: List[Type[Section]] = []
-
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
+    BLOCKS = [
+        MerclAnos,
+    ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="sar.dat") -> "SAR":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="merclsin.out"
+    ) -> "MerclSIN":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="sar.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/newave/shist.py` & `inewave-0.0.97/inewave/nwlistop/earmfsin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,34 @@
-from cfinterface.files.sectionfile import SectionFile
-from cfinterface.components.section import Section
-from typing import TypeVar, List, Type
+from inewave.nwlistop.modelos.earmfsin import EarmAnos
+
+from inewave.nwlistop.modelos.arquivos.arquivosin import (
+    ArquivoSIN,
+)
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Shist(SectionFile):
+class EarmfSIN(ArquivoSIN):
     """
-    Armazena os dados de entrada do NEWAVE referentes à varredura
-    das séries históricas para simulação.
+    Armazena os dados das saídas referentes à energia armazenada
+    final em MWmes para o SIN.
 
+    Esta classe lida com as informações de saída fornecidas pelo
+    NWLISTOP e reproduzidas nos `eafmfsin.out`.
     """
 
-    T = TypeVar("T")
-
-    SECTIONS: List[Type[Section]] = []
-
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
+    BLOCKS = [
+        EarmAnos,
+    ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="shist.dat") -> "Shist":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="earmfsin.out"
+    ) -> "EarmfSIN":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="shist.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/newave/sistema.py` & `inewave-0.0.97/inewave/newave/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/tecno.py` & `inewave-0.0.97/inewave/nwlistop/cdef.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,31 @@
-from cfinterface.files.sectionfile import SectionFile
-from cfinterface.components.section import Section
-from typing import TypeVar, List, Type
+from inewave.nwlistop.modelos.cdef import CdefAnos
+
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
+    Submercado,
+)
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Tecno(SectionFile):
+class Cdef(ArquivoSubmercado):
     """
-    Armazena os dados de entrada do NEWAVE referentes às tecnologias
-    disponíveis para geração de energia.
+    Armazena os dados das saídas referentes ao custo de déficit
+    de cada estágio em cada série.
 
+    Esta classe lida com as informações de saída fornecidas pelo
+    NWLISTOP e reproduzidas nos `cdef00x.out`.
     """
 
-    T = TypeVar("T")
-
-    SECTIONS: List[Type[Section]] = []
-
-    def __init__(self, data=...) -> None:
-        super().__init__(data)
+    BLOCKS = [CdefAnos, Submercado]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="tecno.dat") -> "Tecno":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="cdef001.out") -> "Cdef":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
-
-    def escreve_arquivo(self, diretorio: str, nome_arquivo="tecno.dat"):
-        msg = (
-            "O método escreve_arquivo(diretorio, nome_arquivo) será"
-            + " descontinuado na versão 1.0.0 -"
-            + " use o método write(caminho_arquivo)"
-        )
-        warnings.warn(msg, category=FutureWarning)
-        self.write(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/newave/term.py` & `inewave-0.0.97/inewave/newave/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/vazaob.py` & `inewave-0.0.97/inewave/newave/vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/vazaof.py` & `inewave-0.0.97/inewave/newave/vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/vazaos.py` & `inewave-0.0.97/inewave/newave/vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/vazoes.py` & `inewave-0.0.97/inewave/newave/vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/newave/vazpast.py` & `inewave-0.0.97/inewave/newave/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistcf/estados.py` & `inewave-0.0.97/inewave/nwlistcf/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistcf/modelos/estados.py` & `inewave-0.0.97/inewave/nwlistcf/modelos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistcf/modelos/nwlistcf.py` & `inewave-0.0.97/inewave/nwlistcf/modelos/nwlistcfrel.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistcf/nwlistcf.py` & `inewave-0.0.97/inewave/nwlistcf/nwlistcfrel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from inewave.nwlistcf.modelos.nwlistcf import CortesPeriodoNwlistcf
+from inewave.nwlistcf.modelos.nwlistcfrel import CortesPeriodoNwlistcf
 
 from cfinterface.files.blockfile import BlockFile
 from typing import TypeVar, Optional
 import pandas as pd  # type: ignore
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Nwlistcf(BlockFile):
+class Nwlistcfrel(BlockFile):
     """
     Armazena os dados dos cortes construídos pelo NEWAVE existentes
     no arquivo `nwlistcf.rel` do NWLISTCF.
 
     Esta classe armazena os cortes da FCF de cada uma das variáveis,
     para cada registro e REE dentro do registro.
 
@@ -26,15 +26,15 @@
     def __init__(self, data=...) -> None:
         super().__init__(data)
         self.__cortes_periodos = None
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="nwlistcf.rel"
-    ) -> "Nwlistcf":
+    ) -> "Nwlistcfrel":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/__init__.py` & `inewave-0.0.97/inewave/nwlistop/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Inclui os membros
 
+from .nwlistopdat import Nwlistopdat  # noqa
 from .cmarg import Cmarg  # noqa
 from .cmargmed import CmargMed  # noqa
 from .coper import Coper  # noqa
 from .cterm import Cterm  # noqa
 from .ctermsin import CtermSIN  # noqa
 from .dlppdfmax import DLPPdfmax  # noqa
 from .dlppdfmaxs import DLPPdfmaxs  # noqa
@@ -35,14 +36,16 @@
 from .gttot import Gttot  # noqa
 from .gttotsin import GttotSIN  # noqa
 from .intercambio import Intercambio  # noqa
 from .invade import Invade  # noqa
 from .invadem import Invadem  # noqa
 from .mediasmerc import MediasMerc  # noqa
 from .mediassin import MediasSIN  # noqa
+from .mercl import Mercl  # noqa
+from .merclsin import MerclSIN  # noqa
 from .qafluh import QaflUH  # noqa
 from .qincruh import QincrUH  # noqa
 from .rhslppdf import RHSLPPdf  # noqa
 from .rhslpptb import RHSLPPtb  # noqa
 from .varmuh import VarmUH  # noqa
 from .varmpuh import VarmpUH  # noqa
 from .vento import Vento  # noqa
```

### Comparing `inewave-0.0.96/inewave/nwlistop/cdef.py` & `inewave-0.0.97/inewave/nwlistop/gttot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,37 @@
-from inewave.nwlistop.modelos.cdef import CdefAnos
-
-from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
-    ArquivoSubmercado,
-    Submercado,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
+    ArquivoSubmercadoPatamar,
 )
+from inewave.nwlistop.modelos.gttot import GTAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Cdef(ArquivoSubmercado):
+class Gttot(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes ao custo de déficit
-    de cada estágio em cada série.
+    Armazena os dados das saídas referentes à geração térmica total
+    por patamar, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `cdef00x.out`.
+    NWLISTOP e reproduzidas nos `gttot00x.out`, onde x varia conforme o
+    Submercado em questão.
+
     """
 
-    BLOCKS = [CdefAnos, Submercado]
+    BLOCKS = [
+        Submercado,
+        GTAnos,
+    ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="cdef001.out") -> "Cdef":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="gttot001.out"
+    ) -> "Gttot":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/cdefsin.py` & `inewave-0.0.97/inewave/nwlistop/coper.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,32 @@
-from inewave.nwlistop.modelos.cdefsin import CdefAnos
+from inewave.nwlistop.modelos.coper import CoperAnos
 
 from inewave.nwlistop.modelos.arquivos.arquivosin import (
     ArquivoSIN,
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class CdefSIN(ArquivoSIN):
+class Coper(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes ao custo de déficit
+    Armazena os dados das saídas referentes ao custo total de operação
     de cada estágio em cada série.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `cdefsin.out`.
+    NWLISTOP e reproduzidas nos `coper.out`.
     """
 
     BLOCKS = [
-        CdefAnos,
+        CoperAnos,
     ]
 
     @classmethod
-    def le_arquivo(
-        cls, diretorio: str, nome_arquivo="cdefsin.out"
-    ) -> "CdefSIN":
+    def le_arquivo(cls, diretorio: str, nome_arquivo="coper.out") -> "Coper":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/cmarg.py` & `inewave-0.0.97/inewave/nwlistop/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/cmargmed.py` & `inewave-0.0.97/inewave/nwlistop/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/coper.py` & `inewave-0.0.97/inewave/nwlistop/rhslpptb.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-from inewave.nwlistop.modelos.coper import CoperAnos
-
-from inewave.nwlistop.modelos.arquivos.arquivosin import (
-    ArquivoSIN,
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
+    ArquivoREEPatamar,
 )
+from inewave.nwlistop.modelos.rhslpptb import RHSLPPtbAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Coper(ArquivoSIN):
+class RHSLPPtb(ArquivoREEPatamar):
     """
-    Armazena os dados das saídas referentes ao custo total de operação
-    de cada estágio em cada série.
+    Armazena os dados das saídas referentes ao RHS das restrições LPP
+    de turbinamento máximo por patamar, por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `coper.out`.
+    NWLISTOP e reproduzidas nos `rhslpptb00x.out`, onde x varia conforme o
+    REE em questão.
+
     """
 
     BLOCKS = [
-        CoperAnos,
+        REE,
+        RHSLPPtbAnos,
     ]
 
     @classmethod
-    def le_arquivo(cls, diretorio: str, nome_arquivo="coper.out") -> "Coper":
+    def le_arquivo(
+        cls, diretorio: str, nome_arquivo="rhslpptb001.out"
+    ) -> "RHSLPPtb":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/corteolm.py` & `inewave-0.0.97/inewave/nwlistop/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/cterm.py` & `inewave-0.0.97/inewave/nwlistop/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/ctermsin.py` & `inewave-0.0.97/inewave/nwlistop/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/deficit.py` & `inewave-0.0.97/inewave/nwlistop/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/defsin.py` & `inewave-0.0.97/inewave/nwlistop/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/depminuh.py` & `inewave-0.0.97/inewave/nwlistop/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/dfphauh.py` & `inewave-0.0.97/inewave/nwlistop/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/dlppdfmax.py` & `inewave-0.0.97/inewave/nwlistop/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/dlppdfmaxm.py` & `inewave-0.0.97/inewave/nwlistop/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/dlppdfmaxs.py` & `inewave-0.0.97/inewave/nwlistop/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/dlpptbmax.py` & `inewave-0.0.97/inewave/nwlistop/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/dlpptbmaxm.py` & `inewave-0.0.97/inewave/nwlistop/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/dlpptbmaxs.py` & `inewave-0.0.97/inewave/nwlistop/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/dtbmax.py` & `inewave-0.0.97/inewave/nwlistop/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/dtbmin.py` & `inewave-0.0.97/inewave/nwlistop/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/dvazmax.py` & `inewave-0.0.97/inewave/nwlistop/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/eaf.py` & `inewave-0.0.97/inewave/nwlistop/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/eafb.py` & `inewave-0.0.97/inewave/nwlistop/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/eafbm.py` & `inewave-0.0.97/inewave/nwlistop/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/eafbsin.py` & `inewave-0.0.97/inewave/nwlistop/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/eafm.py` & `inewave-0.0.97/inewave/nwlistop/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/earmf.py` & `inewave-0.0.97/inewave/nwlistop/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/earmfm.py` & `inewave-0.0.97/inewave/nwlistop/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/earmfp.py` & `inewave-0.0.97/inewave/nwlistop/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/earmfpm.py` & `inewave-0.0.97/inewave/nwlistop/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/earmfpsin.py` & `inewave-0.0.97/inewave/nwlistop/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/earmfsin.py` & `inewave-0.0.97/inewave/nwlistop/perdfsin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from inewave.nwlistop.modelos.earmfsin import EarmAnos
-
 from inewave.nwlistop.modelos.arquivos.arquivosin import (
     ArquivoSIN,
 )
+from inewave.nwlistop.modelos.perdfsin import PerdfAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class EarmfSIN(ArquivoSIN):
+class PerdfSIN(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes à energia armazenada
-    final em MWmes para o SIN.
+    Armazena os dados das saídas referentes ao vertimento fio d'água
+    , para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `eafmfsin.out`.
+    NWLISTOP e reproduzidas no `perdfsin.out`.
+
     """
 
     BLOCKS = [
-        EarmAnos,
+        PerdfAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="earmfsin.out"
-    ) -> "EarmfSIN":
+        cls, diretorio: str, nome_arquivo="perdfsin.out"
+    ) -> "PerdfSIN":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/evert.py` & `inewave-0.0.97/inewave/nwlistop/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/evertm.py` & `inewave-0.0.97/inewave/nwlistop/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/evertsin.py` & `inewave-0.0.97/inewave/nwlistop/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/exces.py` & `inewave-0.0.97/inewave/nwlistop/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/excessin.py` & `inewave-0.0.97/inewave/nwlistop/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/fteolm.py` & `inewave-0.0.97/inewave/nwlistop/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/fteolsin.py` & `inewave-0.0.97/inewave/nwlistop/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/geol.py` & `inewave-0.0.97/inewave/nwlistop/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/geolm.py` & `inewave-0.0.97/inewave/nwlistop/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/geolsin.py` & `inewave-0.0.97/inewave/nwlistop/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/ghiduh.py` & `inewave-0.0.97/inewave/nwlistop/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/ghmax.py` & `inewave-0.0.97/inewave/nwlistop/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/ghmaxm.py` & `inewave-0.0.97/inewave/nwlistop/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/ghmaxmr.py` & `inewave-0.0.97/inewave/nwlistop/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/ghmaxr.py` & `inewave-0.0.97/inewave/nwlistop/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/ghmaxrsin.py` & `inewave-0.0.97/inewave/nwlistop/vghminuh.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
-    ArquivoSINPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.ghmaxrsin import GHAnos
+from inewave.nwlistop.modelos.vghminuh import VGhminuhAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class GhmaxrSIN(ArquivoSINPatamar):
+class VghminUH(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à geração hidraulica máxima
-    considerando restrições elétricas por patamar para o SIN.
+    Armazena os dados das saídas referentes à violação da meta de
+    geração hidráulica mínima por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `ghmaxsin.out`.
+    NWLISTOP e reproduzidas nos `vghminuh00x.out`, onde x varia conforme a
+    usina em questão.
+
     """
 
     BLOCKS = [
-        GHAnos,
+        Usina,
+        VGhminuhAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="ghmaxrsin.out"
-    ) -> "GhmaxrSIN":
+        cls, diretorio: str, nome_arquivo="vghminuh001.out"
+    ) -> "VghminUH":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/ghmaxsin.py` & `inewave-0.0.97/inewave/nwlistop/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/ghtot.py` & `inewave-0.0.97/inewave/nwlistop/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/ghtotm.py` & `inewave-0.0.97/inewave/nwlistop/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/ghtotsin.py` & `inewave-0.0.97/inewave/nwlistop/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/gttot.py` & `inewave-0.0.97/inewave/nwlistop/verturbm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
-    ArquivoSubmercadoPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
+    ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.gttot import GTAnos
+from inewave.nwlistop.modelos.verturbm import VertAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Gttot(ArquivoSubmercadoPatamar):
+class Verturbm(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes à geração térmica total
-    por patamar, por REE.
+    Armazena os dados das saídas referentes às energias
+    vertidas, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `gttot00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `vertub00x.out`, onde x varia conforme o
     REE em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        GTAnos,
+        VertAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="gttot001.out"
-    ) -> "Gttot":
+        cls, diretorio: str, nome_arquivo="verturbm001.out"
+    ) -> "Verturbm":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/gttotsin.py` & `inewave-0.0.97/inewave/nwlistop/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/intercambio.py` & `inewave-0.0.97/inewave/nwlistop/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/invade.py` & `inewave-0.0.97/inewave/nwlistop/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/invadem.py` & `inewave-0.0.97/inewave/nwlistop/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/mediasmerc.py` & `inewave-0.0.97/inewave/nwlistop/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/mediassin.py` & `inewave-0.0.97/inewave/nwlistop/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/mercl.py` & `inewave-0.0.97/inewave/nwlistop/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/merclsin.py` & `inewave-0.0.97/inewave/nwlistop/verturbsin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from inewave.nwlistop.modelos.merclsin import MerclAnos
-
+from inewave.nwlistop.modelos.verturbsin import VertAnos
 from inewave.nwlistop.modelos.arquivos.arquivosin import (
     ArquivoSIN,
 )
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class MerclSIN(ArquivoSIN):
+class VerturbSIN(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes ao mercado líquido
-    de cada estágio em cada série.
+    Armazena os dados das saídas referentes às energias
+    vertidas para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `merclsin.out`.
+    NWLISTOP e reproduzidas nos `verturbsin.out`.
+
     """
 
     BLOCKS = [
-        MerclAnos,
+        VertAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="merclsin.out"
-    ) -> "MerclSIN":
+        cls, diretorio: str, nome_arquivo="verturbsin.out"
+    ) -> "VerturbSIN":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py` & `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoree.py` & `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py` & `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py` & `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py` & `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosubmercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py` & `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivousina.py` & `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivousina.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py` & `inewave-0.0.97/inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/blocos/parsubmercados.py` & `inewave-0.0.97/inewave/nwlistop/modelos/blocos/parsubmercados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/blocos/ree.py` & `inewave-0.0.97/inewave/nwlistop/modelos/blocos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/blocos/submercado.py` & `inewave-0.0.97/inewave/nwlistop/modelos/blocos/submercado.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/blocos/usina.py` & `inewave-0.0.97/inewave/nwlistop/modelos/blocos/usina.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/blocos/valoresserie.py` & `inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresserie.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py` & `inewave-0.0.97/inewave/nwlistop/modelos/blocos/valoresseriepatamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/cdef.py` & `inewave-0.0.97/inewave/nwlistop/modelos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/cdefsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/cmarg.py` & `inewave-0.0.97/inewave/nwlistop/modelos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/cmargmed.py` & `inewave-0.0.97/inewave/nwlistop/modelos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/coper.py` & `inewave-0.0.97/inewave/nwlistop/modelos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/corteolm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/cterm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ctermsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/def.py` & `inewave-0.0.97/inewave/nwlistop/modelos/def.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/defsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/depminuh.py` & `inewave-0.0.97/inewave/nwlistop/modelos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/dflppdfmaxm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/dflppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/dflpptbmaxm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/dflpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/dfphauh.py` & `inewave-0.0.97/inewave/nwlistop/modelos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/dlppdfmax.py` & `inewave-0.0.97/inewave/nwlistop/modelos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/dlppdfmaxs.py` & `inewave-0.0.97/inewave/nwlistop/modelos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/dlpptbmax.py` & `inewave-0.0.97/inewave/nwlistop/modelos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/dlpptbmaxs.py` & `inewave-0.0.97/inewave/nwlistop/modelos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/dtbmax.py` & `inewave-0.0.97/inewave/nwlistop/modelos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/dtbmin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/dvazmax.py` & `inewave-0.0.97/inewave/nwlistop/modelos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/eaf.py` & `inewave-0.0.97/inewave/nwlistop/modelos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/eafb.py` & `inewave-0.0.97/inewave/nwlistop/modelos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/eafbm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/eafbsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/eafm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/earmf.py` & `inewave-0.0.97/inewave/nwlistop/modelos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/earmfm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/earmfp.py` & `inewave-0.0.97/inewave/nwlistop/modelos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/earmfpm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/earmfpsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/earmfsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/evert.py` & `inewave-0.0.97/inewave/nwlistop/modelos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/evertm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/evertsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/exces.py` & `inewave-0.0.97/inewave/nwlistop/modelos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/excessin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/fteolm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/fteolsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/geol.py` & `inewave-0.0.97/inewave/nwlistop/modelos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/geolm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/geolsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ghiduh.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ghmax.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ghmaxm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ghmaxmr.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ghmaxr.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ghmaxrsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ghmaxsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ghtot.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ghtotm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/ghtotsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/gttot.py` & `inewave-0.0.97/inewave/nwlistop/modelos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/gttotsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/intercambio.py` & `inewave-0.0.97/inewave/nwlistop/modelos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/invade.py` & `inewave-0.0.97/inewave/nwlistop/modelos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/invadem.py` & `inewave-0.0.97/inewave/nwlistop/modelos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/mediasmerc.py` & `inewave-0.0.97/inewave/nwlistop/modelos/mediasmerc.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/mediassin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/mediassin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/mercl.py` & `inewave-0.0.97/inewave/nwlistop/modelos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/merclsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/perdf.py` & `inewave-0.0.97/inewave/nwlistop/modelos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/perdfm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/perdfsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/qafluh.py` & `inewave-0.0.97/inewave/nwlistop/modelos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/qincruh.py` & `inewave-0.0.97/inewave/nwlistop/modelos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/rhslppdf.py` & `inewave-0.0.97/inewave/nwlistop/modelos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/rhslpptb.py` & `inewave-0.0.97/inewave/nwlistop/modelos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vagua.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/varmpuh.py` & `inewave-0.0.97/inewave/nwlistop/modelos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/varmuh.py` & `inewave-0.0.97/inewave/nwlistop/modelos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vento.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vertuh.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/verturb.py` & `inewave-0.0.97/inewave/nwlistop/modelos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/verturbm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/verturbsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vevmin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vevminm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vevminsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vghmin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vghminm.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vghminsin.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vghminuh.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/modelos/vturuh.py` & `inewave-0.0.97/inewave/nwlistop/modelos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/perdf.py` & `inewave-0.0.97/inewave/nwlistop/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/perdfm.py` & `inewave-0.0.97/inewave/nwlistop/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/perdfsin.py` & `inewave-0.0.97/inewave/nwlistop/vagua.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from inewave.nwlistop.modelos.arquivos.arquivosin import (
-    ArquivoSIN,
-)
-from inewave.nwlistop.modelos.perdfsin import PerdfAnos
+from inewave.nwlistop.modelos.blocos.ree import REE
+from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
+
+from inewave.nwlistop.modelos.vagua import VAAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class PerdfSIN(ArquivoSIN):
+class Vagua(ArquivoREE):
     """
-    Armazena os dados das saídas referentes ao vertimento fio d'água
-    , para o SIN.
+    Armazena os dados das saídas referentes aos valores da água
+    por REE.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas no `perdfsin.out`.
+    NWLISTOP e reproduzidas nos `vagua00x.out`, onde x varia conforme o
+    REE em questão.
 
     """
 
     BLOCKS = [
-        PerdfAnos,
+        REE,
+        VAAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="perdfsin.out"
-    ) -> "PerdfSIN":
+        cls, diretorio: str, nome_arquivo="vagua001.out"
+    ) -> "Vagua":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/qafluh.py` & `inewave-0.0.97/inewave/nwlistop/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/qincruh.py` & `inewave-0.0.97/inewave/nwlistop/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/rhslppdf.py` & `inewave-0.0.97/inewave/nwlistop/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/rhslpptb.py` & `inewave-0.0.97/inewave/nwlistop/vevminsin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoreepatamar import (
-    ArquivoREEPatamar,
+from inewave.nwlistop.modelos.arquivos.arquivosin import (
+    ArquivoSIN,
 )
-from inewave.nwlistop.modelos.rhslpptb import RHSLPPtbAnos
+from inewave.nwlistop.modelos.vevminsin import VevminAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class RHSLPPtb(ArquivoREEPatamar):
+class VevminSIN(ArquivoSIN):
     """
-    Armazena os dados das saídas referentes ao RHS das restrições LPP
-    de turbinamento máximo por patamar, por REE.
+    Armazena os dados das saídas referentes às violações da meta
+    de energia da vazão mínima para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `rhslpptb00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `vevminsin.out`
 
     """
 
     BLOCKS = [
-        REE,
-        RHSLPPtbAnos,
+        VevminAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="rhslpptb001.out"
-    ) -> "RHSLPPtb":
+        cls, diretorio: str, nome_arquivo="vevminsin.out"
+    ) -> "VevminSIN":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/vagua.py` & `inewave-0.0.97/inewave/nwlistop/vento.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from inewave.nwlistop.modelos.blocos.ree import REE
-from inewave.nwlistop.modelos.arquivos.arquivoree import ArquivoREE
-
-from inewave.nwlistop.modelos.vagua import VAAnos
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousina import (
+    ArquivoUsina,
+)
+from inewave.nwlistop.modelos.vento import VentoAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Vagua(ArquivoREE):
+class Vento(ArquivoUsina):
     """
-    Armazena os dados das saídas referentes aos valores da água
-    por REE.
+    Armazena os dados das saídas referentes às velocidades do
+    vento por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vagua00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `vento00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
-        REE,
-        VAAnos,
+        Usina,
+        VentoAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vagua001.out"
-    ) -> "Vagua":
+        cls, diretorio: str, nome_arquivo="vento001.out"
+    ) -> "Vento":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/varmpuh.py` & `inewave-0.0.97/inewave/nwlistop/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/varmuh.py` & `inewave-0.0.97/inewave/nwlistop/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/vento.py` & `inewave-0.0.97/inewave/nwlistop/vghminsin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-from inewave.nwlistop.modelos.blocos.usina import Usina
-from inewave.nwlistop.modelos.arquivos.arquivousina import (
-    ArquivoUsina,
+from inewave.nwlistop.modelos.arquivos.arquivosinpatamar import (
+    ArquivoSINPatamar,
 )
-from inewave.nwlistop.modelos.vento import VentoAnos
+from inewave.nwlistop.modelos.vghmin import VghminAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Vento(ArquivoUsina):
+class VghminSIN(ArquivoSINPatamar):
     """
-    Armazena os dados das saídas referentes às velocidades do
-    vento por usina.
+    Armazena os dados das saídas referentes à violação da meta de geração
+    hidraulica mínima por patamar, para o SIN.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vento00x.out`, onde x varia conforme a
-    usina em questão.
+    NWLISTOP e reproduzidas no `vghminsin.out`.
 
     """
 
     BLOCKS = [
-        Usina,
-        VentoAnos,
+        VghminAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vento001.out"
-    ) -> "Vento":
+        cls, diretorio: str, nome_arquivo="vghminsin.out"
+    ) -> "VghminSIN":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/vertuh.py` & `inewave-0.0.97/inewave/nwlistop/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/verturb.py` & `inewave-0.0.97/inewave/nwlistop/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/verturbm.py` & `inewave-0.0.97/inewave/nwlistop/vevminm.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
 from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
     ArquivoSubmercado,
 )
-from inewave.nwlistop.modelos.verturbm import VertAnos
+from inewave.nwlistop.modelos.vevminm import VevminAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Verturbm(ArquivoSubmercado):
+class Vevminm(ArquivoSubmercado):
     """
-    Armazena os dados das saídas referentes às energias
-    vertidas, por submercado.
+    Armazena os dados das saídas referentes às violações da meta
+    de energia da vazão mínima, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vertub00x.out`, onde x varia conforme o
-    REE em questão.
+    NWLISTOP e reproduzidas nos `vevminm00x.out`, onde x varia conforme o
+    Submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        VertAnos,
+        VevminAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="verturbm001.out"
-    ) -> "Verturbm":
+        cls, diretorio: str, nome_arquivo="vevminm001.out"
+    ) -> "Vevminm":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/verturbsin.py` & `inewave-0.0.97/inewave/nwlistop/vghminm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-from inewave.nwlistop.modelos.verturbsin import VertAnos
-from inewave.nwlistop.modelos.arquivos.arquivosin import (
-    ArquivoSIN,
+from inewave.nwlistop.modelos.blocos.submercado import Submercado
+from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
+    ArquivoSubmercadoPatamar,
 )
+from inewave.nwlistop.modelos.vghminm import VghminAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class VerturbSIN(ArquivoSIN):
+class Vghminm(ArquivoSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes às energias
-    vertidas para o SIN.
+    Armazena os dados das saídas referentes à violação da meta de geração
+    hidráulica mínima por patamar, por Submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `verturbsin.out`.
+    NWLISTOP e reproduzidas nos `vghmin00x.out`, onde x varia conforme o
+    Submercado em questão.
 
     """
 
     BLOCKS = [
-        VertAnos,
+        Submercado,
+        VghminAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="verturbsin.out"
-    ) -> "VerturbSIN":
+        cls, diretorio: str, nome_arquivo="vghminm001.out"
+    ) -> "Vghminm":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/vevmin.py` & `inewave-0.0.97/inewave/nwlistop/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/vevminm.py` & `inewave-0.0.97/inewave/nwlistop/gtert.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercado import (
-    ArquivoSubmercado,
+from inewave.nwlistop.modelos.arquivos.arquivoclassetermicasubmercadopatamar import (
+    ArquivoClasseTermicaSubmercadoPatamar,
 )
-from inewave.nwlistop.modelos.vevminm import VevminAnos
+from inewave.nwlistop.modelos.gtert import GTAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Vevminm(ArquivoSubmercado):
+class Gtert(ArquivoClasseTermicaSubmercadoPatamar):
     """
-    Armazena os dados das saídas referentes às violações da meta
-    de energia da vazão mínima, por Submercado.
+    Armazena os dados das saídas referentes à geração térmica por classe
+    térmica, por patamar, por submercado.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vevminm00x.out`, onde x varia conforme o
+    NWLISTOP e reproduzidas nos `gtert00x.out`, onde x varia conforme o
     Submercado em questão.
 
     """
 
     BLOCKS = [
         Submercado,
-        VevminAnos,
+        GTAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vevminm001.out"
-    ) -> "Vevminm":
+        cls, diretorio: str, nome_arquivo="gtert001.out"
+    ) -> "Gtert":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave/nwlistop/vghmin.py` & `inewave-0.0.97/inewave/nwlistop/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/inewave/nwlistop/vghminm.py` & `inewave-0.0.97/inewave/nwlistop/vturuh.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-from inewave.nwlistop.modelos.blocos.submercado import Submercado
-from inewave.nwlistop.modelos.arquivos.arquivosubmercadopatamar import (
-    ArquivoSubmercadoPatamar,
+from inewave.nwlistop.modelos.blocos.usina import Usina
+from inewave.nwlistop.modelos.arquivos.arquivousinapatamar import (
+    ArquivoUsinaPatamar,
 )
-from inewave.nwlistop.modelos.vghminm import VghminAnos
+from inewave.nwlistop.modelos.vturuh import VturAnos
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
-class Vghminm(ArquivoSubmercadoPatamar):
+class VturUH(ArquivoUsinaPatamar):
     """
-    Armazena os dados das saídas referentes à violação da meta de geração
-    hidráulica mínima por patamar, por Submercado.
+    Armazena os dados das saídas referentes às vazões turbinadas por usina.
 
     Esta classe lida com as informações de saída fornecidas pelo
-    NWLISTOP e reproduzidas nos `vghmin00x.out`, onde x varia conforme o
-    Submercado em questão.
+    NWLISTOP e reproduzidas nos `vturuh00x.out`, onde x varia conforme a
+    usina em questão.
 
     """
 
     BLOCKS = [
-        Submercado,
-        VghminAnos,
+        Usina,
+        VturAnos,
     ]
 
     @classmethod
     def le_arquivo(
-        cls, diretorio: str, nome_arquivo="vghminm001.out"
-    ) -> "Vghminm":
+        cls, diretorio: str, nome_arquivo="vturuh001.out"
+    ) -> "VturUH":
         msg = (
             "O método le_arquivo(diretorio, nome_arquivo) será descontinuado"
             + " na versão 1.0.0 - use o método read(caminho_arquivo)"
         )
         warnings.warn(msg, category=FutureWarning)
         return cls.read(join(diretorio, nome_arquivo))
```

### Comparing `inewave-0.0.96/inewave.egg-info/PKG-INFO` & `inewave-0.0.97/inewave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inewave
-Version: 0.0.96
+Version: 0.0.97
 Summary: Interface para arquivos do NEWAVE
 Home-page: https://github.com/rjmalves/inewave
 Author: Rogerio Alves
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `inewave-0.0.96/inewave.egg-info/SOURCES.txt` & `inewave-0.0.97/inewave.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 inewave/newave/pmo.py
 inewave/newave/re.py
 inewave/newave/ree.py
 inewave/newave/restricaoeletrica.py
 inewave/newave/restricaoenergia.py
 inewave/newave/restricaovazao.py
 inewave/newave/sar.py
+inewave/newave/selcor.py
 inewave/newave/shist.py
 inewave/newave/sistema.py
 inewave/newave/tecno.py
 inewave/newave/term.py
 inewave/newave/vazaob.py
 inewave/newave/vazaof.py
 inewave/newave/vazaos.py
@@ -146,14 +147,15 @@
 inewave/newave/modelos/pmo.py
 inewave/newave/modelos/re.py
 inewave/newave/modelos/ree.py
 inewave/newave/modelos/restricaoeletrica.py
 inewave/newave/modelos/restricaoenergia.py
 inewave/newave/modelos/restricaovazao.py
 inewave/newave/modelos/sar.py
+inewave/newave/modelos/selcor.py
 inewave/newave/modelos/shist.py
 inewave/newave/modelos/sistema.py
 inewave/newave/modelos/tecno.py
 inewave/newave/modelos/term.py
 inewave/newave/modelos/vazaob.py
 inewave/newave/modelos/vazaof.py
 inewave/newave/modelos/vazaos.py
@@ -161,19 +163,25 @@
 inewave/newave/modelos/vazpast.py
 inewave/newave/modelos/arquivoscsv/__init__.py
 inewave/newave/modelos/arquivoscsv/arquivocsv.py
 inewave/newave/modelos/blocos/__init__.py
 inewave/newave/modelos/blocos/tabelacsv.py
 inewave/newave/modelos/blocos/versaomodelo.py
 inewave/nwlistcf/__init__.py
+inewave/nwlistcf/arquivos.py
+inewave/nwlistcf/caso.py
 inewave/nwlistcf/estados.py
-inewave/nwlistcf/nwlistcf.py
+inewave/nwlistcf/nwlistcfdat.py
+inewave/nwlistcf/nwlistcfrel.py
 inewave/nwlistcf/modelos/__init__.py
+inewave/nwlistcf/modelos/arquivos.py
+inewave/nwlistcf/modelos/caso.py
 inewave/nwlistcf/modelos/estados.py
-inewave/nwlistcf/modelos/nwlistcf.py
+inewave/nwlistcf/modelos/nwlistcfdat.py
+inewave/nwlistcf/modelos/nwlistcfrel.py
 inewave/nwlistop/__init__.py
 inewave/nwlistop/cdef.py
 inewave/nwlistop/cdefsin.py
 inewave/nwlistop/cmarg.py
 inewave/nwlistop/cmargmed.py
 inewave/nwlistop/coper.py
 inewave/nwlistop/corteolm.py
@@ -219,23 +227,25 @@
 inewave/nwlistop/ghmaxmr.py
 inewave/nwlistop/ghmaxr.py
 inewave/nwlistop/ghmaxrsin.py
 inewave/nwlistop/ghmaxsin.py
 inewave/nwlistop/ghtot.py
 inewave/nwlistop/ghtotm.py
 inewave/nwlistop/ghtotsin.py
+inewave/nwlistop/gtert.py
 inewave/nwlistop/gttot.py
 inewave/nwlistop/gttotsin.py
 inewave/nwlistop/intercambio.py
 inewave/nwlistop/invade.py
 inewave/nwlistop/invadem.py
 inewave/nwlistop/mediasmerc.py
 inewave/nwlistop/mediassin.py
 inewave/nwlistop/mercl.py
 inewave/nwlistop/merclsin.py
+inewave/nwlistop/nwlistopdat.py
 inewave/nwlistop/perdf.py
 inewave/nwlistop/perdfm.py
 inewave/nwlistop/perdfsin.py
 inewave/nwlistop/qafluh.py
 inewave/nwlistop/qincruh.py
 inewave/nwlistop/rhslppdf.py
 inewave/nwlistop/rhslpptb.py
@@ -304,23 +314,25 @@
 inewave/nwlistop/modelos/ghmaxmr.py
 inewave/nwlistop/modelos/ghmaxr.py
 inewave/nwlistop/modelos/ghmaxrsin.py
 inewave/nwlistop/modelos/ghmaxsin.py
 inewave/nwlistop/modelos/ghtot.py
 inewave/nwlistop/modelos/ghtotm.py
 inewave/nwlistop/modelos/ghtotsin.py
+inewave/nwlistop/modelos/gtert.py
 inewave/nwlistop/modelos/gttot.py
 inewave/nwlistop/modelos/gttotsin.py
 inewave/nwlistop/modelos/intercambio.py
 inewave/nwlistop/modelos/invade.py
 inewave/nwlistop/modelos/invadem.py
 inewave/nwlistop/modelos/mediasmerc.py
 inewave/nwlistop/modelos/mediassin.py
 inewave/nwlistop/modelos/mercl.py
 inewave/nwlistop/modelos/merclsin.py
+inewave/nwlistop/modelos/nwlistopdat.py
 inewave/nwlistop/modelos/perdf.py
 inewave/nwlistop/modelos/perdfm.py
 inewave/nwlistop/modelos/perdfsin.py
 inewave/nwlistop/modelos/qafluh.py
 inewave/nwlistop/modelos/qincruh.py
 inewave/nwlistop/modelos/rhslppdf.py
 inewave/nwlistop/modelos/rhslpptb.py
@@ -337,42 +349,47 @@
 inewave/nwlistop/modelos/vevminsin.py
 inewave/nwlistop/modelos/vghmin.py
 inewave/nwlistop/modelos/vghminm.py
 inewave/nwlistop/modelos/vghminsin.py
 inewave/nwlistop/modelos/vghminuh.py
 inewave/nwlistop/modelos/vturuh.py
 inewave/nwlistop/modelos/arquivos/__init__.py
+inewave/nwlistop/modelos/arquivos/arquivoclassetermicasubmercadopatamar.py
 inewave/nwlistop/modelos/arquivos/arquivoparsubmercadopatamar.py
 inewave/nwlistop/modelos/arquivos/arquivoree.py
 inewave/nwlistop/modelos/arquivos/arquivoreepatamar.py
 inewave/nwlistop/modelos/arquivos/arquivosin.py
 inewave/nwlistop/modelos/arquivos/arquivosinpatamar.py
 inewave/nwlistop/modelos/arquivos/arquivosubmercado.py
 inewave/nwlistop/modelos/arquivos/arquivosubmercadopatamar.py
 inewave/nwlistop/modelos/arquivos/arquivousina.py
 inewave/nwlistop/modelos/arquivos/arquivousinapatamar.py
 inewave/nwlistop/modelos/blocos/__init__.py
 inewave/nwlistop/modelos/blocos/parsubmercados.py
 inewave/nwlistop/modelos/blocos/ree.py
 inewave/nwlistop/modelos/blocos/submercado.py
 inewave/nwlistop/modelos/blocos/usina.py
+inewave/nwlistop/modelos/blocos/valoresclassetermicaseriepatamar.py
 inewave/nwlistop/modelos/blocos/valoresserie.py
 inewave/nwlistop/modelos/blocos/valoresseriepatamar.py
 tests/__init__.py
 tests/_arquivos/__init__.py
 tests/mocks/__init__.py
 tests/mocks/mock_open.py
 tests/mocks/arquivos/__init__.py
 tests/mocks/arquivos/adterm.py
+tests/mocks/arquivos/agrint.py
 tests/mocks/arquivos/arquivos.py
+tests/mocks/arquivos/arquivos_nwlistcf.py
 tests/mocks/arquivos/avl_cortesfpha_nwv.py
 tests/mocks/arquivos/avl_desvfpha_s.py
 tests/mocks/arquivos/avl_desvfpha_v_q.py
 tests/mocks/arquivos/cadic.py
 tests/mocks/arquivos/caso.py
+tests/mocks/arquivos/caso_nwlistcf_nwlistop.py
 tests/mocks/arquivos/cdef.py
 tests/mocks/arquivos/cdefsin.py
 tests/mocks/arquivos/clast.py
 tests/mocks/arquivos/cmarg.py
 tests/mocks/arquivos/cmargmed.py
 tests/mocks/arquivos/confhd.py
 tests/mocks/arquivos/conft.py
@@ -419,39 +436,45 @@
 tests/mocks/arquivos/estados.py
 tests/mocks/arquivos/evert.py
 tests/mocks/arquivos/evertm.py
 tests/mocks/arquivos/evertsin.py
 tests/mocks/arquivos/exces.py
 tests/mocks/arquivos/excessin.py
 tests/mocks/arquivos/exph.py
+tests/mocks/arquivos/expt.py
 tests/mocks/arquivos/fteolm.py
 tests/mocks/arquivos/fteolsin.py
 tests/mocks/arquivos/geol.py
 tests/mocks/arquivos/geolm.py
 tests/mocks/arquivos/geolsin.py
 tests/mocks/arquivos/ghiduh.py
 tests/mocks/arquivos/ghmax.py
 tests/mocks/arquivos/ghmaxm.py
 tests/mocks/arquivos/ghmaxmr.py
 tests/mocks/arquivos/ghmaxr.py
 tests/mocks/arquivos/ghmaxrsin.py
 tests/mocks/arquivos/ghmaxsin.py
+tests/mocks/arquivos/ghmin.py
 tests/mocks/arquivos/ghtot.py
 tests/mocks/arquivos/ghtotm.py
 tests/mocks/arquivos/ghtotsin.py
+tests/mocks/arquivos/gtert.py
 tests/mocks/arquivos/gttot.py
 tests/mocks/arquivos/gttotsin.py
 tests/mocks/arquivos/intercambio.py
 tests/mocks/arquivos/invade.py
 tests/mocks/arquivos/invadem.py
+tests/mocks/arquivos/manutt.py
 tests/mocks/arquivos/mercl.py
 tests/mocks/arquivos/merclsin.py
 tests/mocks/arquivos/modif.py
 tests/mocks/arquivos/newavetim.py
-tests/mocks/arquivos/nwlistcf.py
+tests/mocks/arquivos/nwlistcfdat.py
+tests/mocks/arquivos/nwlistcfrel.py
+tests/mocks/arquivos/nwlistopdat.py
 tests/mocks/arquivos/nwv_avl_evap.py
 tests/mocks/arquivos/nwv_cortes_evap.py
 tests/mocks/arquivos/nwv_eco_evap.py
 tests/mocks/arquivos/parp.py
 tests/mocks/arquivos/parpeol.py
 tests/mocks/arquivos/parpvaz.py
 tests/mocks/arquivos/patamar.py
@@ -465,14 +488,16 @@
 tests/mocks/arquivos/re.py
 tests/mocks/arquivos/ree.py
 tests/mocks/arquivos/restricaoeletrica.py
 tests/mocks/arquivos/restricaoenergia.py
 tests/mocks/arquivos/restricaovazao.py
 tests/mocks/arquivos/rhslppdf.py
 tests/mocks/arquivos/rhslpptb.py
+tests/mocks/arquivos/selcor.py
+tests/mocks/arquivos/shist.py
 tests/mocks/arquivos/sistema.py
 tests/mocks/arquivos/term.py
 tests/mocks/arquivos/vagua.py
 tests/mocks/arquivos/varmpuh.py
 tests/mocks/arquivos/varmuh.py
 tests/mocks/arquivos/vazpast.py
 tests/mocks/arquivos/vento.py
@@ -486,14 +511,15 @@
 tests/mocks/arquivos/vghmin.py
 tests/mocks/arquivos/vghminm.py
 tests/mocks/arquivos/vghminsin.py
 tests/mocks/arquivos/vghminuh.py
 tests/mocks/arquivos/vturuh.py
 tests/newave/__init__.py
 tests/newave/test_adterm.py
+tests/newave/test_agrint.py
 tests/newave/test_arquivos.py
 tests/newave/test_avl_cortesfpha_nwv.py
 tests/newave/test_avl_desvfpha_s.py
 tests/newave/test_avl_desvfpha_v_q.py
 tests/newave/test_cadic.py
 tests/newave/test_caso.py
 tests/newave/test_clast.py
@@ -516,17 +542,20 @@
 tests/newave/test_eolicaconfiguracao.py
 tests/newave/test_eolicafte.py
 tests/newave/test_eolicageracao.py
 tests/newave/test_eolicahistorico.py
 tests/newave/test_eolicaposto.py
 tests/newave/test_eolicasubmercado.py
 tests/newave/test_exph.py
+tests/newave/test_expt.py
 tests/newave/test_forward.py
 tests/newave/test_forwarh.py
+tests/newave/test_ghmin.py
 tests/newave/test_hidr.py
+tests/newave/test_manutt.py
 tests/newave/test_modif.py
 tests/newave/test_newavetim.py
 tests/newave/test_nwv_avl_evap.py
 tests/newave/test_nwv_cortes_evap.py
 tests/newave/test_nwv_eco_evap.py
 tests/newave/test_parp.py
 tests/newave/test_parpeol.py
@@ -535,24 +564,29 @@
 tests/newave/test_penalid.py
 tests/newave/test_pmo.py
 tests/newave/test_re.py
 tests/newave/test_ree.py
 tests/newave/test_restricaoeletrica.py
 tests/newave/test_restricaoenergia.py
 tests/newave/test_restricaovazao.py
+tests/newave/test_selcor.py
+tests/newave/test_shist.py
 tests/newave/test_sistema.py
 tests/newave/test_term.py
 tests/newave/test_vazaob.py
 tests/newave/test_vazaof.py
 tests/newave/test_vazaos.py
 tests/newave/test_vazoes.py
 tests/newave/test_vazpast.py
 tests/nwlistcf/__init__.py
+tests/nwlistcf/test_arquivos.py
+tests/nwlistcf/test_caso.py
 tests/nwlistcf/test_estados.py
-tests/nwlistcf/test_nwlistcf.py
+tests/nwlistcf/test_nwlistcfdat.py
+tests/nwlistcf/test_nwlistcfrel.py
 tests/nwlistop/__init__.py
 tests/nwlistop/test_cdef.py
 tests/nwlistop/test_cdefsin.py
 tests/nwlistop/test_cmarg.py
 tests/nwlistop/test_cmargmed.py
 tests/nwlistop/test_coper.py
 tests/nwlistop/test_corteolm.py
@@ -598,23 +632,25 @@
 tests/nwlistop/test_ghmaxmr.py
 tests/nwlistop/test_ghmaxr.py
 tests/nwlistop/test_ghmaxrsin.py
 tests/nwlistop/test_ghmaxsin.py
 tests/nwlistop/test_ghtot.py
 tests/nwlistop/test_ghtotm.py
 tests/nwlistop/test_ghtotsin.py
+tests/nwlistop/test_gtert.py
 tests/nwlistop/test_gttot.py
 tests/nwlistop/test_gttotsin.py
 tests/nwlistop/test_intercambio.py
 tests/nwlistop/test_invade.py
 tests/nwlistop/test_invadem.py
 tests/nwlistop/test_mediasmerc.py
 tests/nwlistop/test_mediassin.py
 tests/nwlistop/test_mercl.py
 tests/nwlistop/test_merclsin.py
+tests/nwlistop/test_nwlistopdat.py
 tests/nwlistop/test_perdf.py
 tests/nwlistop/test_perdfm.py
 tests/nwlistop/test_perdfsin.py
 tests/nwlistop/test_qafluh.py
 tests/nwlistop/test_qincruh.py
 tests/nwlistop/test_rhslppdf.py
 tests/nwlistop/test_rhslpptb.py
```

### Comparing `inewave-0.0.96/setup.py` & `inewave-0.0.97/setup.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/adterm.py` & `inewave-0.0.97/tests/mocks/arquivos/adterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/arquivos.py` & `inewave-0.0.97/tests/mocks/arquivos/arquivos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/avl_cortesfpha_nwv.py` & `inewave-0.0.97/tests/mocks/arquivos/avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/avl_desvfpha_s.py` & `inewave-0.0.97/tests/mocks/arquivos/avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/avl_desvfpha_v_q.py` & `inewave-0.0.97/tests/mocks/arquivos/avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/cadic.py` & `inewave-0.0.97/tests/mocks/arquivos/cadic.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/cdef.py` & `inewave-0.0.97/tests/mocks/arquivos/cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/cdefsin.py` & `inewave-0.0.97/tests/mocks/arquivos/cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/clast.py` & `inewave-0.0.97/tests/mocks/arquivos/clast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/cmarg.py` & `inewave-0.0.97/tests/mocks/arquivos/cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/cmargmed.py` & `inewave-0.0.97/tests/mocks/arquivos/cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/confhd.py` & `inewave-0.0.97/tests/mocks/arquivos/confhd.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/conft.py` & `inewave-0.0.97/tests/mocks/arquivos/conft.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/coper.py` & `inewave-0.0.97/tests/mocks/arquivos/coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/corteolm.py` & `inewave-0.0.97/tests/mocks/arquivos/corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/cterm.py` & `inewave-0.0.97/tests/mocks/arquivos/cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ctermsin.py` & `inewave-0.0.97/tests/mocks/arquivos/ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/curva.py` & `inewave-0.0.97/tests/mocks/arquivos/curva.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/cvar.py` & `inewave-0.0.97/tests/mocks/arquivos/cvar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/deficit.py` & `inewave-0.0.97/tests/mocks/arquivos/deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/defsin.py` & `inewave-0.0.97/tests/mocks/arquivos/defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/depminuh.py` & `inewave-0.0.97/tests/mocks/arquivos/depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dfphauh.py` & `inewave-0.0.97/tests/mocks/arquivos/dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dger.py` & `inewave-0.0.97/tests/mocks/arquivos/dger.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dlppdfmax.py` & `inewave-0.0.97/tests/mocks/arquivos/dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dlppdfmaxm.py` & `inewave-0.0.97/tests/mocks/arquivos/dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dlppdfmaxs.py` & `inewave-0.0.97/tests/mocks/arquivos/dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dlpptbmax.py` & `inewave-0.0.97/tests/mocks/arquivos/dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dlpptbmaxm.py` & `inewave-0.0.97/tests/mocks/arquivos/dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dlpptbmaxs.py` & `inewave-0.0.97/tests/mocks/arquivos/dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dsvagua.py` & `inewave-0.0.97/tests/mocks/arquivos/dsvagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dtbmax.py` & `inewave-0.0.97/tests/mocks/arquivos/dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dtbmin.py` & `inewave-0.0.97/tests/mocks/arquivos/dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/dvazmax.py` & `inewave-0.0.97/tests/mocks/arquivos/dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eaf.py` & `inewave-0.0.97/tests/mocks/arquivos/eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eafb.py` & `inewave-0.0.97/tests/mocks/arquivos/eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eafbm.py` & `inewave-0.0.97/tests/mocks/arquivos/eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eafbsin.py` & `inewave-0.0.97/tests/mocks/arquivos/eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eafm.py` & `inewave-0.0.97/tests/mocks/arquivos/eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eafpast.py` & `inewave-0.0.97/tests/mocks/arquivos/eafpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/earmf.py` & `inewave-0.0.97/tests/mocks/arquivos/earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/earmfm.py` & `inewave-0.0.97/tests/mocks/arquivos/earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/earmfp.py` & `inewave-0.0.97/tests/mocks/arquivos/earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/earmfpm.py` & `inewave-0.0.97/tests/mocks/arquivos/earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/earmfpsin.py` & `inewave-0.0.97/tests/mocks/arquivos/earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/earmfsin.py` & `inewave-0.0.97/tests/mocks/arquivos/earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eolicacadastro.py` & `inewave-0.0.97/tests/mocks/arquivos/eolicacadastro.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eolicaconfig.py` & `inewave-0.0.97/tests/mocks/arquivos/eolicaconfig.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eolicafte.py` & `inewave-0.0.97/tests/mocks/arquivos/eolicafte.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eolicageracao.py` & `inewave-0.0.97/tests/mocks/arquivos/eolicageracao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eolicahistorico.py` & `inewave-0.0.97/tests/mocks/arquivos/eolicahistorico.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/eolicaposto.py` & `inewave-0.0.97/tests/mocks/arquivos/eolicaposto.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/estados.py` & `inewave-0.0.97/tests/mocks/arquivos/estados.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/evert.py` & `inewave-0.0.97/tests/mocks/arquivos/evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/evertm.py` & `inewave-0.0.97/tests/mocks/arquivos/evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/evertsin.py` & `inewave-0.0.97/tests/mocks/arquivos/evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/exces.py` & `inewave-0.0.97/tests/mocks/arquivos/exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/excessin.py` & `inewave-0.0.97/tests/mocks/arquivos/excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/exph.py` & `inewave-0.0.97/tests/mocks/arquivos/exph.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/fteolm.py` & `inewave-0.0.97/tests/mocks/arquivos/fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/fteolsin.py` & `inewave-0.0.97/tests/mocks/arquivos/fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/geol.py` & `inewave-0.0.97/tests/mocks/arquivos/geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/geolm.py` & `inewave-0.0.97/tests/mocks/arquivos/geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/geolsin.py` & `inewave-0.0.97/tests/mocks/arquivos/geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ghiduh.py` & `inewave-0.0.97/tests/mocks/arquivos/ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ghmax.py` & `inewave-0.0.97/tests/mocks/arquivos/ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ghmaxm.py` & `inewave-0.0.97/tests/mocks/arquivos/ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ghmaxmr.py` & `inewave-0.0.97/tests/mocks/arquivos/ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ghmaxr.py` & `inewave-0.0.97/tests/mocks/arquivos/ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ghmaxrsin.py` & `inewave-0.0.97/tests/mocks/arquivos/ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ghmaxsin.py` & `inewave-0.0.97/tests/mocks/arquivos/ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ghtot.py` & `inewave-0.0.97/tests/mocks/arquivos/ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ghtotm.py` & `inewave-0.0.97/tests/mocks/arquivos/ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ghtotsin.py` & `inewave-0.0.97/tests/mocks/arquivos/ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/gttot.py` & `inewave-0.0.97/tests/mocks/arquivos/gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/gttotsin.py` & `inewave-0.0.97/tests/mocks/arquivos/gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/intercambio.py` & `inewave-0.0.97/tests/mocks/arquivos/intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/invade.py` & `inewave-0.0.97/tests/mocks/arquivos/invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/invadem.py` & `inewave-0.0.97/tests/mocks/arquivos/invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/mercl.py` & `inewave-0.0.97/tests/mocks/arquivos/mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/merclsin.py` & `inewave-0.0.97/tests/mocks/arquivos/merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/modif.py` & `inewave-0.0.97/tests/mocks/arquivos/modif.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,35 +4,47 @@
 
 MockVAZMIN = " VAZMIN       34\n"
 
 MockVMAXT = " VMAXT    12 2021  61.310 '%'\n"
 
 MockVAZMINT = " VAZMINT  10 2021   10.00 \n"
 
-MockVOLMIN = " VOLMIN          15563.63 'h'\n"
+MockVOLMIN = " VOLMIN   15563.63 'h' \n"
 
-MockVOLMAX = " VOLMAX          15563.63 'h'\n"
+MockVOLMAX = " VOLMAX   55.000 '%'\n"
 
 MockNUMCNJ = " NUMCNJ     2\n"
 
 MockNUMMAQ = " NUMMAQ     2  5\n"
 
 MockVMINT = " VMINT    10 2021  20.000 '%'\n"
 
 MockVMINP = " VMINP    10 2021  20.000 '%'\n"
 
 MockCFUGA = " CFUGA    10 2021    5.60\n"
 
 MockCMONT = " CMONT    10 2021   71.30\n"
 
+MockVAZMAXT = " VAZMAXT   1 2020    0.00"
+
+MockTURBMAXT = " TURBMAXT  1 2020    0.00"
+
+MockTURBMINT = " TURBMINT  1 2020    0.00"
+
 MockModif = [
     " P.CHAVE  MODIFICACOES E INDICES\n",
     " XXXXXXXX XXXXXXXXXXXXXXXXXXXXX\n",
     " USINA    1                                 CAMARGOS            \n",
     " VAZMIN       34\n",
+    " VAZMAXT   1 2020    0.00\n",
+    " VAZMAXT   2 2020    0.00\n",
+    " TURBMAXT  1 2020    0.00\n",
+    " TURBMAXT  2 2020    0.00\n",
+    " TURBMINT  1 2020    0.00\n",
+    " TURBMINT  2 2020    0.00\n",
     " NUMCNJ     2\n",
     " NUMMAQ     2  5\n",
     " VMAXT    11 2021  92.560 '%'\n",
     " VMAXT    12 2021  61.310 '%'\n",
     " VMAXT     1 2022  70.240 '%'\n",
     " VMAXT     2 2022  85.120 '%'\n",
     " VMAXT     3 2022 100.000 '%'\n",
@@ -607,15 +619,15 @@
     " VAZMINT   1 2022   95.00 \n",
     " USINA    4                                 FUNIL-GRANDE        \n",
     " VAZMIN       70\n",
     " USINA    28                                CAPIM BRANC2        \n",
     " VAZMIN       72\n",
     " USINA    34                                I. SOLTEIRA        \n",
     " VAZMIN      1450 \n",
-    " VOLMIN          15563.63 'h'\n",
+    " VOLMIN   15563.63 'h' \n",
     " VMINT    12 2021  45.890 '%'\n",
     " VMAXT    11 2021  48.770 '%'\n",
     " VMAXT    12 2021  45.990 '%'\n",
     " VMAXT     1 2022  49.620 '%'\n",
     " VMAXT     2 2022  63.730 '%'\n",
     " VMAXT     3 2022  82.380 '%'\n",
     " VMAXT     4 2022 100.000 '%'\n",
```

### Comparing `inewave-0.0.96/tests/mocks/arquivos/newavetim.py` & `inewave-0.0.97/tests/mocks/arquivos/newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/nwlistcf.py` & `inewave-0.0.97/tests/mocks/arquivos/nwlistcfrel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-MockNwlistcf = [
+MockNwlistcfrel = [
     "\n",
     "=>  CORTES A SEREM IMPRESSOS NESTE RELATORIO:  SOMENTE CORTES VALIDOS ATE A ULTIMA ITERACAO\n",
     "\n",
     "  PERIODO:            5\n",
     " X--------X---X---------------X-----------------X-----------------X-----------------X-----------------X-----------------X-----------------X-----------------X-----------------X-----------------X-----------------X-----------------X-----------------X-----------------X-----------------X-----------------X\n",
     "   IREG    REE     RHS             PIV               PIH( 1)           PIH( 2)           PIH( 3)           PIH( 4)           PIH( 5)           PIH( 6)        PIGTAD(P1L1)      PIGTAD(P1L2)      PIGTAD(P2L1)      PIGTAD(P2L2)      PIGTAD(P3L1)      PIGTAD(P3L2)        PIMX_SAR            PIMX_VMN       \n",
     "   1043800   1   77807116.0178     -12.093730000     -63.667410000      -4.036300000       0.000000000       0.000000000       0.000000000       0.000000000      -8.699350000      -9.887430000      -8.699350000      -9.887430000      -8.699350000      -9.886130000       0.000000000       0.000000000\n",
```

### Comparing `inewave-0.0.96/tests/mocks/arquivos/nwv_avl_evap.py` & `inewave-0.0.97/tests/mocks/arquivos/nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/nwv_cortes_evap.py` & `inewave-0.0.97/tests/mocks/arquivos/nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/nwv_eco_evap.py` & `inewave-0.0.97/tests/mocks/arquivos/nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/parp.py` & `inewave-0.0.97/tests/mocks/arquivos/parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/parpeol.py` & `inewave-0.0.97/tests/mocks/arquivos/parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/parpvaz.py` & `inewave-0.0.97/tests/mocks/arquivos/parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/patamar.py` & `inewave-0.0.97/tests/mocks/arquivos/patamar.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/penalid.py` & `inewave-0.0.97/tests/mocks/arquivos/penalid.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/perdf.py` & `inewave-0.0.97/tests/mocks/arquivos/perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/perdfm.py` & `inewave-0.0.97/tests/mocks/arquivos/perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/perdfsin.py` & `inewave-0.0.97/tests/mocks/arquivos/perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/pmo.py` & `inewave-0.0.97/tests/mocks/arquivos/pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/qafluh.py` & `inewave-0.0.97/tests/mocks/arquivos/qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/qincruh.py` & `inewave-0.0.97/tests/mocks/arquivos/qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/re.py` & `inewave-0.0.97/tests/mocks/arquivos/re.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/ree.py` & `inewave-0.0.97/tests/mocks/arquivos/ree.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/restricaoeletrica.py` & `inewave-0.0.97/tests/mocks/arquivos/restricaoeletrica.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/restricaoenergia.py` & `inewave-0.0.97/tests/mocks/arquivos/restricaoenergia.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/restricaovazao.py` & `inewave-0.0.97/tests/mocks/arquivos/restricaovazao.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/rhslppdf.py` & `inewave-0.0.97/tests/mocks/arquivos/rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/rhslpptb.py` & `inewave-0.0.97/tests/mocks/arquivos/rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/sistema.py` & `inewave-0.0.97/tests/mocks/arquivos/sistema.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/term.py` & `inewave-0.0.97/tests/mocks/arquivos/term.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vagua.py` & `inewave-0.0.97/tests/mocks/arquivos/vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/varmpuh.py` & `inewave-0.0.97/tests/mocks/arquivos/varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/varmuh.py` & `inewave-0.0.97/tests/mocks/arquivos/varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vazpast.py` & `inewave-0.0.97/tests/mocks/arquivos/vazpast.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vento.py` & `inewave-0.0.97/tests/mocks/arquivos/vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vertuh.py` & `inewave-0.0.97/tests/mocks/arquivos/vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/verturb.py` & `inewave-0.0.97/tests/mocks/arquivos/verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/verturbm.py` & `inewave-0.0.97/tests/mocks/arquivos/verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/verturbsin.py` & `inewave-0.0.97/tests/mocks/arquivos/verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vevmin.py` & `inewave-0.0.97/tests/mocks/arquivos/vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vevminm.py` & `inewave-0.0.97/tests/mocks/arquivos/vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vevminsin.py` & `inewave-0.0.97/tests/mocks/arquivos/vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vghmin.py` & `inewave-0.0.97/tests/mocks/arquivos/vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vghminm.py` & `inewave-0.0.97/tests/mocks/arquivos/vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vghminsin.py` & `inewave-0.0.97/tests/mocks/arquivos/vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vghminuh.py` & `inewave-0.0.97/tests/mocks/arquivos/vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/arquivos/vturuh.py` & `inewave-0.0.97/tests/mocks/arquivos/vturuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/mocks/mock_open.py` & `inewave-0.0.97/tests/mocks/mock_open.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_adterm.py` & `inewave-0.0.97/tests/newave/test_adterm.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,13 +60,13 @@
         ad1 = AdTerm.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         ad2 = AdTerm.read(ARQ_TESTE)
         assert ad1 == ad2
```

### Comparing `inewave-0.0.96/tests/newave/test_arquivos.py` & `inewave-0.0.97/tests/newave/test_arquivos.py`

 * *Files 0% similar despite different names*

```diff
@@ -145,13 +145,13 @@
         ad1 = Arquivos.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         ad2 = Arquivos.read(ARQ_TESTE)
         assert ad1 == ad2
```

### Comparing `inewave-0.0.96/tests/newave/test_avl_cortesfpha_nwv.py` & `inewave-0.0.97/tests/newave/test_avl_cortesfpha_nwv.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_avl_desvfpha_s.py` & `inewave-0.0.97/tests/newave/test_avl_desvfpha_s.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_avl_desvfpha_v_q.py` & `inewave-0.0.97/tests/newave/test_avl_desvfpha_v_q.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_cadic.py` & `inewave-0.0.97/tests/newave/test_cadic.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,13 +63,13 @@
         ad1 = CAdic.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         ad2 = CAdic.read(ARQ_TESTE)
         assert ad1 == ad2
```

### Comparing `inewave-0.0.96/tests/newave/test_caso.py` & `inewave-0.0.97/tests/newave/test_caso.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,13 +72,13 @@
         ad1 = Caso.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         ad2 = Caso.read(ARQ_TESTE)
         assert ad1 == ad2
```

### Comparing `inewave-0.0.96/tests/newave/test_clast.py` & `inewave-0.0.97/tests/newave/test_clast.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,13 +88,13 @@
         ct1 = ClasT.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         ct1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         ct2 = ClasT.read(ARQ_TESTE)
         assert ct1 == ct2
```

### Comparing `inewave-0.0.96/tests/newave/test_confhd.py` & `inewave-0.0.97/tests/newave/test_confhd.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,13 +61,13 @@
         cf1 = Confhd.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = Confhd.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_conft.py` & `inewave-0.0.97/tests/newave/test_conft.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,13 +61,13 @@
         cf1 = ConfT.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = ConfT.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_cortes.py` & `inewave-0.0.97/tests/newave/test_cortes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_cortesh.py` & `inewave-0.0.97/tests/newave/test_cortesh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_curva.py` & `inewave-0.0.97/tests/newave/test_curva.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,13 +158,13 @@
         cf1 = Curva.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = Curva.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_cvar.py` & `inewave-0.0.97/tests/newave/test_cvar.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,13 +96,13 @@
         cf1 = CVAR.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = CVAR.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_dger.py` & `inewave-0.0.97/tests/newave/test_dger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1364,13 +1364,13 @@
         d1 = DGer.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         d1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         d2 = DGer.read(ARQ_TESTE)
         assert d1 == d2
```

### Comparing `inewave-0.0.96/tests/newave/test_dsvagua.py` & `inewave-0.0.97/tests/newave/test_dsvagua.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,13 +61,13 @@
         cf1 = DSVAgua.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = DSVAgua.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_eafpast.py` & `inewave-0.0.97/tests/newave/test_eafpast.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,13 +62,13 @@
         cf1 = EafPast.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = EafPast.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_enavazb.py` & `inewave-0.0.97/tests/newave/test_enavazb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_enavazf.py` & `inewave-0.0.97/tests/newave/test_enavazf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_energiab.py` & `inewave-0.0.97/tests/newave/test_energiab.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_energiaf.py` & `inewave-0.0.97/tests/newave/test_energiaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_energias.py` & `inewave-0.0.97/tests/newave/test_energias.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_engnat.py` & `inewave-0.0.97/tests/newave/test_engnat.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_eolicacadastro.py` & `inewave-0.0.97/tests/newave/test_eolicacadastro.py`

 * *Files 0% similar despite different names*

```diff
@@ -229,13 +229,13 @@
         cf1 = EolicaCadastro.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = EolicaCadastro.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_eolicaconfiguracao.py` & `inewave-0.0.97/tests/newave/test_eolicaconfiguracao.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,13 +99,13 @@
         cf1 = EolicaConfiguracao.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = EolicaConfiguracao.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_eolicafte.py` & `inewave-0.0.97/tests/newave/test_eolicafte.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,13 +98,13 @@
         cf1 = EolicaFTE.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = EolicaFTE.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_eolicageracao.py` & `inewave-0.0.97/tests/newave/test_eolicageracao.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,13 +93,13 @@
         cf1 = EolicaGeracao.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = EolicaGeracao.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_eolicahistorico.py` & `inewave-0.0.97/tests/newave/test_eolicahistorico.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,13 +125,13 @@
         cf1 = EolicaHistorico.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = EolicaHistorico.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_eolicaposto.py` & `inewave-0.0.97/tests/newave/test_eolicaposto.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,13 +78,13 @@
         cf1 = EolicaPosto.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = EolicaPosto.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_eolicasubmercado.py` & `inewave-0.0.97/tests/newave/test_eolicasubmercado.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,13 +76,13 @@
         cf1 = EolicaSubmercado.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = EolicaSubmercado.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_exph.py` & `inewave-0.0.97/tests/newave/test_exph.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,13 +68,13 @@
         ad1 = Exph.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         ad1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         ad2 = Exph.read(ARQ_TESTE)
         assert ad1 == ad2
```

### Comparing `inewave-0.0.96/tests/newave/test_forward.py` & `inewave-0.0.97/tests/newave/test_forward.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_forwarh.py` & `inewave-0.0.97/tests/newave/test_forwarh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_hidr.py` & `inewave-0.0.97/tests/newave/test_hidr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_modif.py` & `inewave-0.0.97/tests/newave/test_modif.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,17 @@
     VAZMIN,
     CFUGA,
     CMONT,
     VMAXT,
     VMINT,
     VMINP,
     VAZMINT,
+    VAZMAXT,
+    TURBMAXT,
+    TURBMINT,
 )
 
 from inewave.newave import Modif
 
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
@@ -30,14 +33,17 @@
     MockVAZMIN,
     MockCFUGA,
     MockCMONT,
     MockVMAXT,
     MockVMINT,
     MockVMINP,
     MockVAZMINT,
+    MockVAZMAXT,
+    MockTURBMAXT,
+    MockTURBMINT,
 )
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_registro_usina_modif():
     m: MagicMock = mock_open(read_data="".join(MockUSINA))
@@ -85,37 +91,35 @@
 
     assert r.data == [10, 2021, 10.00]
     assert r.mes == 10
     assert r.ano == 2021
     assert r.vazao == 10.00
 
 
-# def test_registro_volmin_modif():
-
-#     m: MagicMock = mock_open(read_data="".join(MockVOLMIN))
-#     r = VOLMIN()
-#     with patch("builtins.open", m):
-#         with open("", "") as fp:
-#             r.read(fp)
-
-#     assert r.data == [15563.63, "'h'"]
-#     assert r.volume == 15563.63
+def test_registro_volmin_modif():
+    m: MagicMock = mock_open(read_data="".join(MockVOLMIN))
+    r = VOLMIN()
+    with patch("builtins.open", m):
+        with open("", "") as fp:
+            r.read(fp)
 
+    assert r.data == [15563.63, "'h'"]
+    assert r.volume == 15563.63
 
-# def test_registro_volmax_modif():
 
-#     m: MagicMock = mock_open(read_data="".join(MockVOLMAX))
-#     r = VOLMAX()
-#     with patch("builtins.open", m):
-#         with open("", "") as fp:
-#             r.read(fp)
+def test_registro_volmax_modif():
+    m: MagicMock = mock_open(read_data="".join(MockVOLMAX))
+    r = VOLMAX()
+    with patch("builtins.open", m):
+        with open("", "") as fp:
+            r.read(fp)
 
-#     assert r.data == [15563.63, "'h'"]
-#     assert r.volume == 15563.63
-#     assert r.unidade == "'h'"
+    assert r.data == [55.0, "'%'"]
+    assert r.volume == 55.0
+    assert r.unidade == "'%'"
 
 
 def test_registro_numcnj_modif():
     m: MagicMock = mock_open(read_data="".join(MockNUMCNJ))
     r = NUMCNJ()
     with patch("builtins.open", m):
         with open("", "") as fp:
@@ -187,14 +191,53 @@
 
     assert r.data == [10, 2021, 71.30]
     assert r.mes == 10
     assert r.ano == 2021
     assert r.nivel == 71.30
 
 
+def test_registro_vazmaxt_modif():
+    m: MagicMock = mock_open(read_data="".join(MockVAZMAXT))
+    r = VAZMAXT()
+    with patch("builtins.open", m):
+        with open("", "") as fp:
+            r.read(fp)
+
+    assert r.data == [1, 2020, 0.00]
+    assert r.mes == 1
+    assert r.ano == 2020
+    assert r.vazao == 0.0
+
+
+def test_registro_turbmaxt_modif():
+    m: MagicMock = mock_open(read_data="".join(MockTURBMAXT))
+    r = TURBMAXT()
+    with patch("builtins.open", m):
+        with open("", "") as fp:
+            r.read(fp)
+
+    assert r.data == [1, 2020, 0.00]
+    assert r.mes == 1
+    assert r.ano == 2020
+    assert r.turbinamento == 0.0
+
+
+def test_registro_turbmint_modif():
+    m: MagicMock = mock_open(read_data="".join(MockTURBMINT))
+    r = TURBMINT()
+    with patch("builtins.open", m):
+        with open("", "") as fp:
+            r.read(fp)
+
+    assert r.data == [1, 2020, 0.00]
+    assert r.mes == 1
+    assert r.ano == 2020
+    assert r.turbinamento == 0.0
+
+
 def test_atributos_encontrados_modif():
     m: MagicMock = mock_open(read_data="".join(MockModif))
     with patch("builtins.open", m):
         ad = Modif.read(ARQ_TESTE)
         assert len(ad.usina()) > 0
         assert len(ad.vazmin()) > 0
         assert len(ad.vmaxt()) > 0
@@ -203,42 +246,28 @@
         assert isinstance(ad.volmax(), VOLMAX)
         assert len(ad.numcnj()) > 0
         assert len(ad.nummaq()) > 0
         assert len(ad.vmint()) > 0
         assert len(ad.vminp()) > 0
         assert len(ad.cfuga()) > 0
         assert len(ad.cmont()) > 0
-
-
-# def test_eq_patamar():
-#     m: MagicMock = mock_open(read_data="".join(MockPatamar))
-#     with patch("builtins.open", m):
-#         cf1 = Patamar.read(ARQ_TESTE)
-#         cf2 = Patamar.read(ARQ_TESTE)
-#         assert cf1 == cf2
-
-
-# def test_neq_patamar():
-#     m: MagicMock = mock_open(read_data="".join(MockPatamar))
-#     with patch("builtins.open", m):
-#         cf1 = Patamar.read(ARQ_TESTE)
-#         cf2 = Patamar.read(ARQ_TESTE)
-#         cf2.numero_patamares = 0
-#         assert cf1 != cf2
-
-
-# def test_leitura_escrita_patamar():
-#     m_leitura: MagicMock = mock_open(read_data="".join(MockPatamar))
-#     with patch("builtins.open", m_leitura):
-#         cf1 = Patamar.read(ARQ_TESTE)
-#     m_escrita: MagicMock = mock_open(read_data="")
-#     with patch("builtins.open", m_escrita):
-#         cf1.write(ARQ_TESTE)
-#         # Recupera o que foi escrito
-#         chamadas = m_escrita.mock_calls
-#         linhas_escritas = [
-#             chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
-#         ]
-#     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
-#     with patch("builtins.open", m_releitura):
-#         cf2 = Patamar.read(ARQ_TESTE)
-#         assert cf1 == cf2
+        assert len(ad.vazmaxt()) > 0
+        assert len(ad.turbmaxt()) > 0
+        assert len(ad.turbmint()) > 0
+
+
+def test_leitura_escrita_modif():
+    m_leitura: MagicMock = mock_open(read_data="".join(MockModif))
+    with patch("builtins.open", m_leitura):
+        cf1 = Modif.read(ARQ_TESTE)
+    m_escrita: MagicMock = mock_open(read_data="")
+    with patch("builtins.open", m_escrita):
+        cf1.write(ARQ_TESTE)
+        # Recupera o que foi escrito
+        chamadas = m_escrita.mock_calls
+        linhas_escritas = [
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
+        ]
+    m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
+    with patch("builtins.open", m_releitura):
+        cf2 = Modif.read(ARQ_TESTE)
+        assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_newavetim.py` & `inewave-0.0.97/tests/newave/test_newavetim.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_nwv_avl_evap.py` & `inewave-0.0.97/tests/newave/test_nwv_avl_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_nwv_cortes_evap.py` & `inewave-0.0.97/tests/newave/test_nwv_cortes_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_nwv_eco_evap.py` & `inewave-0.0.97/tests/newave/test_nwv_eco_evap.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_parp.py` & `inewave-0.0.97/tests/newave/test_parp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_parpeol.py` & `inewave-0.0.97/tests/newave/test_parpeol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_parpvaz.py` & `inewave-0.0.97/tests/newave/test_parpvaz.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_patamar.py` & `inewave-0.0.97/tests/newave/test_patamar.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,13 +182,13 @@
         cf1 = Patamar.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = Patamar.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_penalid.py` & `inewave-0.0.97/tests/newave/test_penalid.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,13 +50,13 @@
         cf1 = Penalid.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = Penalid.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_pmo.py` & `inewave-0.0.97/tests/newave/test_pmo.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_re.py` & `inewave-0.0.97/tests/newave/test_re.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,13 +82,13 @@
         cf1 = RE.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = RE.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_ree.py` & `inewave-0.0.97/tests/newave/test_ree.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,13 +51,13 @@
         cf1 = REE.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = REE.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_restricaoeletrica.py` & `inewave-0.0.97/tests/newave/test_restricaoeletrica.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,13 +110,13 @@
         cf1 = RestricaoEletrica.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = RestricaoEletrica.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_restricaoenergia.py` & `inewave-0.0.97/tests/newave/test_restricaoenergia.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,13 +101,13 @@
         cf1 = RestricaoEnergia.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = RestricaoEnergia.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_restricaovazao.py` & `inewave-0.0.97/tests/newave/test_restricaovazao.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,13 +101,13 @@
         cf1 = RestricaoVazao.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = RestricaoVazao.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_sistema.py` & `inewave-0.0.97/tests/newave/test_sistema.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,13 +129,13 @@
         cf1 = Sistema.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = Sistema.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_term.py` & `inewave-0.0.97/tests/newave/test_term.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,13 +61,13 @@
         cf1 = Term.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = Term.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/newave/test_vazaob.py` & `inewave-0.0.97/tests/newave/test_vazaob.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_vazaof.py` & `inewave-0.0.97/tests/newave/test_vazaof.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_vazaos.py` & `inewave-0.0.97/tests/newave/test_vazaos.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_vazoes.py` & `inewave-0.0.97/tests/newave/test_vazoes.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/newave/test_vazpast.py` & `inewave-0.0.97/tests/newave/test_vazpast.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,13 +63,13 @@
         cf1 = VazPast.read(ARQ_TESTE)
     m_escrita: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m_escrita):
         cf1.write(ARQ_TESTE)
         # Recupera o que foi escrito
         chamadas = m_escrita.mock_calls
         linhas_escritas = [
-            chamadas[i].args[0] for i in range(2, len(chamadas) - 1)
+            chamadas[i].args[0] for i in range(1, len(chamadas) - 1)
         ]
     m_releitura: MagicMock = mock_open(read_data="".join(linhas_escritas))
     with patch("builtins.open", m_releitura):
         cf2 = VazPast.read(ARQ_TESTE)
         assert cf1 == cf2
```

### Comparing `inewave-0.0.96/tests/nwlistcf/test_estados.py` & `inewave-0.0.97/tests/nwlistcf/test_estados.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
 def test_atributos_encontrados_estados():
     m: MagicMock = mock_open(read_data="".join(MockEstados))
     with patch("builtins.open", m):
         n = Estados.read(ARQ_TESTE)
-        print(n.estados)
         assert n.estados is not None
 
 
 def test_atributos_nao_encontrados_estados():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
         n = Estados.read(ARQ_TESTE)
```

### Comparing `inewave-0.0.96/tests/nwlistcf/test_nwlistcf.py` & `inewave-0.0.97/tests/nwlistcf/test_nwlistcfrel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from inewave.nwlistcf import Nwlistcf
+from inewave.nwlistcf import Nwlistcfrel
 
 from tests.mocks.mock_open import mock_open
 from unittest.mock import MagicMock, patch
 
-from tests.mocks.arquivos.nwlistcf import MockNwlistcf
+from tests.mocks.arquivos.nwlistcfrel import MockNwlistcfrel
 
 ARQ_TESTE = "./tests/mocks/arquivos/__init__.py"
 
 
-def test_atributos_encontrados_nwlistcf():
-    m: MagicMock = mock_open(read_data="".join(MockNwlistcf))
+def test_atributos_encontrados_nwlistcfrel():
+    m: MagicMock = mock_open(read_data="".join(MockNwlistcfrel))
     with patch("builtins.open", m):
-        n = Nwlistcf.read(ARQ_TESTE)
+        n = Nwlistcfrel.read(ARQ_TESTE)
         assert n.cortes is not None
 
 
-def test_atributos_nao_encontrados_nwlistcf():
+def test_atributos_nao_encontrados_nwlistcfrel():
     m: MagicMock = mock_open(read_data="")
     with patch("builtins.open", m):
-        n = Nwlistcf.read(ARQ_TESTE)
+        n = Nwlistcfrel.read(ARQ_TESTE)
         assert n.cortes is None
 
 
-def test_eq_nwlistcf():
-    m: MagicMock = mock_open(read_data="".join(MockNwlistcf))
+def test_eq_nwlistcfrel():
+    m: MagicMock = mock_open(read_data="".join(MockNwlistcfrel))
     with patch("builtins.open", m):
-        n1 = Nwlistcf.read(ARQ_TESTE)
-        n2 = Nwlistcf.read(ARQ_TESTE)
+        n1 = Nwlistcfrel.read(ARQ_TESTE)
+        n2 = Nwlistcfrel.read(ARQ_TESTE)
         assert n1 == n2
 
 
 # Não deve ter teste de diferença, visto que o atributo é
 # implementado como Lazy Property.
```

### Comparing `inewave-0.0.96/tests/nwlistop/test_cdef.py` & `inewave-0.0.97/tests/nwlistop/test_cdef.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_cdefsin.py` & `inewave-0.0.97/tests/nwlistop/test_cdefsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_cmarg.py` & `inewave-0.0.97/tests/nwlistop/test_cmarg.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_cmargmed.py` & `inewave-0.0.97/tests/nwlistop/test_cmargmed.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_coper.py` & `inewave-0.0.97/tests/nwlistop/test_coper.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_corteolm.py` & `inewave-0.0.97/tests/nwlistop/test_corteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_cterm.py` & `inewave-0.0.97/tests/nwlistop/test_cterm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ctermsin.py` & `inewave-0.0.97/tests/nwlistop/test_ctermsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_deficit.py` & `inewave-0.0.97/tests/nwlistop/test_deficit.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_defsin.py` & `inewave-0.0.97/tests/nwlistop/test_defsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_depminuh.py` & `inewave-0.0.97/tests/nwlistop/test_depminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_dfphauh.py` & `inewave-0.0.97/tests/nwlistop/test_dfphauh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_dlppdfmax.py` & `inewave-0.0.97/tests/nwlistop/test_dlppdfmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_dlppdfmaxm.py` & `inewave-0.0.97/tests/nwlistop/test_dlppdfmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_dlppdfmaxs.py` & `inewave-0.0.97/tests/nwlistop/test_dlppdfmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_dlpptbmax.py` & `inewave-0.0.97/tests/nwlistop/test_dlpptbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_dlpptbmaxm.py` & `inewave-0.0.97/tests/nwlistop/test_dlpptbmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_dlpptbmaxs.py` & `inewave-0.0.97/tests/nwlistop/test_dlpptbmaxs.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_dtbmax.py` & `inewave-0.0.97/tests/nwlistop/test_dtbmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_dtbmin.py` & `inewave-0.0.97/tests/nwlistop/test_dtbmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_dvazmax.py` & `inewave-0.0.97/tests/nwlistop/test_dvazmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_eaf.py` & `inewave-0.0.97/tests/nwlistop/test_eaf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_eafb.py` & `inewave-0.0.97/tests/nwlistop/test_eafb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_eafbm.py` & `inewave-0.0.97/tests/nwlistop/test_eafbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_eafbsin.py` & `inewave-0.0.97/tests/nwlistop/test_eafbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_eafm.py` & `inewave-0.0.97/tests/nwlistop/test_eafm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_earmf.py` & `inewave-0.0.97/tests/nwlistop/test_earmf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_earmfm.py` & `inewave-0.0.97/tests/nwlistop/test_earmfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_earmfp.py` & `inewave-0.0.97/tests/nwlistop/test_earmfp.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_earmfpm.py` & `inewave-0.0.97/tests/nwlistop/test_earmfpm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_earmfpsin.py` & `inewave-0.0.97/tests/nwlistop/test_earmfpsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_earmfsin.py` & `inewave-0.0.97/tests/nwlistop/test_earmfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_evert.py` & `inewave-0.0.97/tests/nwlistop/test_evert.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_evertm.py` & `inewave-0.0.97/tests/nwlistop/test_evertm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_evertsin.py` & `inewave-0.0.97/tests/nwlistop/test_evertsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_exces.py` & `inewave-0.0.97/tests/nwlistop/test_exces.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_excessin.py` & `inewave-0.0.97/tests/nwlistop/test_excessin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_fteolm.py` & `inewave-0.0.97/tests/nwlistop/test_fteolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_fteolsin.py` & `inewave-0.0.97/tests/nwlistop/test_fteolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_geol.py` & `inewave-0.0.97/tests/nwlistop/test_geol.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_geolm.py` & `inewave-0.0.97/tests/nwlistop/test_geolm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_geolsin.py` & `inewave-0.0.97/tests/nwlistop/test_geolsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ghiduh.py` & `inewave-0.0.97/tests/nwlistop/test_ghiduh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ghmax.py` & `inewave-0.0.97/tests/nwlistop/test_ghmax.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ghmaxm.py` & `inewave-0.0.97/tests/nwlistop/test_ghmaxm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ghmaxmr.py` & `inewave-0.0.97/tests/nwlistop/test_ghmaxmr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ghmaxr.py` & `inewave-0.0.97/tests/nwlistop/test_ghmaxr.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ghmaxrsin.py` & `inewave-0.0.97/tests/nwlistop/test_ghmaxrsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ghmaxsin.py` & `inewave-0.0.97/tests/nwlistop/test_ghmaxsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ghtot.py` & `inewave-0.0.97/tests/nwlistop/test_ghtot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ghtotm.py` & `inewave-0.0.97/tests/nwlistop/test_ghtotm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_ghtotsin.py` & `inewave-0.0.97/tests/nwlistop/test_ghtotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_gttot.py` & `inewave-0.0.97/tests/nwlistop/test_gttot.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_gttotsin.py` & `inewave-0.0.97/tests/nwlistop/test_gttotsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_intercambio.py` & `inewave-0.0.97/tests/nwlistop/test_intercambio.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_invade.py` & `inewave-0.0.97/tests/nwlistop/test_invade.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_invadem.py` & `inewave-0.0.97/tests/nwlistop/test_invadem.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_mercl.py` & `inewave-0.0.97/tests/nwlistop/test_mercl.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_merclsin.py` & `inewave-0.0.97/tests/nwlistop/test_merclsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_perdf.py` & `inewave-0.0.97/tests/nwlistop/test_perdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_perdfm.py` & `inewave-0.0.97/tests/nwlistop/test_perdfm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_perdfsin.py` & `inewave-0.0.97/tests/nwlistop/test_perdfsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_qafluh.py` & `inewave-0.0.97/tests/nwlistop/test_qafluh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_qincruh.py` & `inewave-0.0.97/tests/nwlistop/test_qincruh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_rhslppdf.py` & `inewave-0.0.97/tests/nwlistop/test_rhslppdf.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_rhslpptb.py` & `inewave-0.0.97/tests/nwlistop/test_rhslpptb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vagua.py` & `inewave-0.0.97/tests/nwlistop/test_vagua.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_varmpuh.py` & `inewave-0.0.97/tests/nwlistop/test_varmpuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_varmuh.py` & `inewave-0.0.97/tests/nwlistop/test_varmuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vento.py` & `inewave-0.0.97/tests/nwlistop/test_vento.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vertuh.py` & `inewave-0.0.97/tests/nwlistop/test_vertuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_verturb.py` & `inewave-0.0.97/tests/nwlistop/test_verturb.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_verturbm.py` & `inewave-0.0.97/tests/nwlistop/test_verturbm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_verturbsin.py` & `inewave-0.0.97/tests/nwlistop/test_verturbsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vevmin.py` & `inewave-0.0.97/tests/nwlistop/test_vevmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vevminm.py` & `inewave-0.0.97/tests/nwlistop/test_vevminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vevminsin.py` & `inewave-0.0.97/tests/nwlistop/test_vevminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vghmin.py` & `inewave-0.0.97/tests/nwlistop/test_vghmin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vghminm.py` & `inewave-0.0.97/tests/nwlistop/test_vghminm.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vghminsin.py` & `inewave-0.0.97/tests/nwlistop/test_vghminsin.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vghminuh.py` & `inewave-0.0.97/tests/nwlistop/test_vghminuh.py`

 * *Files identical despite different names*

### Comparing `inewave-0.0.96/tests/nwlistop/test_vturuh.py` & `inewave-0.0.97/tests/nwlistop/test_vturuh.py`

 * *Files identical despite different names*

