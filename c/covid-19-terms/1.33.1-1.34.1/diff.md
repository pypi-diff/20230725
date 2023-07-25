# Comparing `tmp/covid_19_terms-1.33.1.tar.gz` & `tmp/covid_19_terms-1.34.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covid_19_terms-1.33.1.tar", last modified: Mon Feb  6 12:52:21 2023, max compression
+gzip compressed data, was "covid_19_terms-1.34.1.tar", last modified: Tue Jul 25 09:38:02 2023, max compression
```

## Comparing `covid_19_terms-1.33.1.tar` & `covid_19_terms-1.34.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 12:52:21.355029 covid_19_terms-1.33.1/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-06 12:52:21.355029 covid_19_terms-1.33.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-02-06 12:51:56.000000 covid_19_terms-1.33.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 12:52:21.351029 covid_19_terms-1.33.1/covid_19_terms/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-02-06 12:52:19.000000 covid_19_terms-1.33.1/covid_19_terms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   130323 2023-02-06 12:52:19.000000 covid_19_terms-1.33.1/covid_19_terms/terms.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-06 12:52:21.355029 covid_19_terms-1.33.1/covid_19_terms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-06 12:52:21.000000 covid_19_terms-1.33.1/covid_19_terms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-06 12:52:21.000000 covid_19_terms-1.33.1/covid_19_terms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-06 12:52:21.000000 covid_19_terms-1.33.1/covid_19_terms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-06 12:52:21.000000 covid_19_terms-1.33.1/covid_19_terms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-06 12:52:21.355029 covid_19_terms-1.33.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-02-06 12:51:56.000000 covid_19_terms-1.33.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:38:02.760844 covid_19_terms-1.34.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-25 09:38:02.760844 covid_19_terms-1.34.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-25 09:37:35.000000 covid_19_terms-1.34.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:38:02.760844 covid_19_terms-1.34.1/covid_19_terms/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-25 09:37:59.000000 covid_19_terms-1.34.1/covid_19_terms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   138679 2023-07-25 09:37:59.000000 covid_19_terms-1.34.1/covid_19_terms/terms.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:38:02.760844 covid_19_terms-1.34.1/covid_19_terms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-25 09:38:02.000000 covid_19_terms-1.34.1/covid_19_terms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-25 09:38:02.000000 covid_19_terms-1.34.1/covid_19_terms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:38:02.000000 covid_19_terms-1.34.1/covid_19_terms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 09:38:02.000000 covid_19_terms-1.34.1/covid_19_terms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-25 09:38:02.760844 covid_19_terms-1.34.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-25 09:37:35.000000 covid_19_terms-1.34.1/setup.py
```

### Comparing `covid_19_terms-1.33.1/covid_19_terms/terms.json` & `covid_19_terms-1.34.1/covid_19_terms/terms.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9935483870967742%*

 * *Differences: {"'products'": "{'42029111000001101': OrderedDict([('name', OrderedDict([('display', 'Spikevax'), "*

 * *               "('eu', OrderedDict([('display', 'Spikevax'), ('code', 'EU/1/20/1507')]))])), "*

 * *               "('term', 'Generic Spikevax XBB.1.5 COVID-19 mRNA Vaccine 0.1mg/1ml dispersion for "*

 * *               "injection multidose vials'), ('type', 'VMP'), ('manufacturer', "*

 * *               "OrderedDict([('display', 'Moderna, Inc'), ('eu', OrderedDict([('code', "*

 * *               "'ORG-100031184'), ('display', ' […]*

```diff
@@ -4702,14 +4702,342 @@
                 {
                     "code": "41343811000001106",
                     "type": "APM"
                 }
             ],
             "term": "Generic COVID-19 Vaccine Spikevax Original/Omicron BA.4/BA.5 dispersion for injection 0.1mg/ml multidose vials",
             "type": "VMP"
+        },
+        "42020611000001103": {
+            "manufacturer": {
+                "display": "Pfizer Ltd",
+                "eu": {
+                    "code": "ORG-100030215",
+                    "display": "Biontech Manafacturing GmbH"
+                }
+            },
+            "name": {
+                "display": "Comirnaty",
+                "eu": {
+                    "code": "EU/1/20/1528",
+                    "display": "Comirnaty"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42020711000001107",
+                    "type": "APM"
+                },
+                {
+                    "code": "42029211000001107",
+                    "type": "VMP"
+                }
+            ],
+            "term": "Generic Comirnaty Omicron XBB.1.5 COVID-19 mRNA Vaccine 30micrograms/0.3ml dose dispersion for injection multidose vials 6 dose",
+            "type": "VMPP"
+        },
+        "42020711000001107": {
+            "manufacturer": {
+                "display": "Pfizer Ltd",
+                "eu": {
+                    "code": "ORG-100030215",
+                    "display": "Biontech Manafacturing GmbH"
+                }
+            },
+            "name": {
+                "display": "Comirnaty",
+                "eu": {
+                    "code": "EU/1/20/1528",
+                    "display": "Comirnaty"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42020711000001107",
+                    "type": "APM"
+                },
+                {
+                    "code": "42029211000001107",
+                    "type": "VMP"
+                }
+            ],
+            "term": "Comirnaty Omicron XBB.1.5 COVID-19 mRNA Vaccine 30micrograms/0.3ml dose dispersion for injection multidose vials (Pfizer Ltd)",
+            "type": "AMP"
+        },
+        "42020811000001104": {
+            "manufacturer": {
+                "display": "Pfizer Ltd",
+                "eu": {
+                    "code": "ORG-100030215",
+                    "display": "Biontech Manafacturing GmbH"
+                }
+            },
+            "name": {
+                "display": "Comirnaty",
+                "eu": {
+                    "code": "EU/1/20/1528",
+                    "display": "Comirnaty"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42020711000001107",
+                    "type": "APM"
+                },
+                {
+                    "code": "42029211000001107",
+                    "type": "VMP"
+                }
+            ],
+            "term": "Comirnaty Omicron XBB.1.5 COVID-19 mRNA Vaccine 30micrograms/0.3ml dose dispersion for injection multidose vials (Pfizer Ltd) 6 dose",
+            "type": "AMPP"
+        },
+        "42022811000001103": {
+            "manufacturer": {
+                "display": "Pfizer Ltd",
+                "eu": {
+                    "code": "ORG-100030215",
+                    "display": "Biontech Manafacturing GmbH"
+                }
+            },
+            "name": {
+                "display": "Comirnaty",
+                "eu": {
+                    "code": "EU/1/20/1528",
+                    "display": "Comirnaty"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42020711000001107",
+                    "type": "APM"
+                },
+                {
+                    "code": "42029211000001107",
+                    "type": "VMP"
+                }
+            ],
+            "term": "Generic Comirnaty Omicron XBB.1.5 COVID-19 mRNA Vaccine 30micrograms/0.3ml dose dispersion for injection multidose vials 60 dose",
+            "type": "VMPP"
+        },
+        "42022911000001108": {
+            "manufacturer": {
+                "display": "Pfizer Ltd",
+                "eu": {
+                    "code": "ORG-100030215",
+                    "display": "Biontech Manafacturing GmbH"
+                }
+            },
+            "name": {
+                "display": "Comirnaty",
+                "eu": {
+                    "code": "EU/1/20/1528",
+                    "display": "Comirnaty"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42020711000001107",
+                    "type": "APM"
+                },
+                {
+                    "code": "42029211000001107",
+                    "type": "VMP"
+                }
+            ],
+            "term": "Comirnaty Omicron XBB.1.5 COVID-19 mRNA Vaccine 30micrograms/0.3ml dose dispersion for injection multidose vials (Pfizer Ltd) 60 dose 10 x 6 doses",
+            "type": "AMPP"
+        },
+        "42023111000001104": {
+            "manufacturer": {
+                "display": "Moderna, Inc",
+                "eu": {
+                    "code": "ORG-100031184",
+                    "display": "Moderna Biotech Spain S.L"
+                }
+            },
+            "name": {
+                "display": "Spikevax",
+                "eu": {
+                    "code": "EU/1/20/1507",
+                    "display": "Spikevax"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42023311000001102",
+                    "type": "APM"
+                },
+                {
+                    "code": "42029111000001101",
+                    "type": "VMP"
+                }
+            ],
+            "term": "Generic Spikevax XBB.1.5 COVID-19 mRNA Vaccine 0.1mg/1ml dispersion for injection multidose vials 25 ml",
+            "type": "VMPP"
+        },
+        "42023211000001105": {
+            "manufacturer": {
+                "display": "Moderna, Inc",
+                "eu": {
+                    "code": "ORG-100031184",
+                    "display": "Moderna Biotech Spain S.L"
+                }
+            },
+            "name": {
+                "display": "Spikevax",
+                "eu": {
+                    "code": "EU/1/20/1507",
+                    "display": "Spikevax"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42023311000001102",
+                    "type": "APM"
+                },
+                {
+                    "code": "42029111000001101",
+                    "type": "VMP"
+                }
+            ],
+            "term": "Generic Spikevax XBB.1.5 COVID-19 mRNA Vaccine 0.1mg/1ml dispersion for injection multidose vials 2.5 ml",
+            "type": "VMPP"
+        },
+        "42023311000001102": {
+            "manufacturer": {
+                "display": "Moderna, Inc",
+                "eu": {
+                    "code": "ORG-100031184",
+                    "display": "Moderna Biotech Spain S.L"
+                }
+            },
+            "name": {
+                "display": "Spikevax",
+                "eu": {
+                    "code": "EU/1/20/1507",
+                    "display": "Spikevax"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42023311000001102",
+                    "type": "APM"
+                },
+                {
+                    "code": "42029111000001101",
+                    "type": "VMP"
+                }
+            ],
+            "term": "Spikevax XBB.1.5 COVID-19 mRNA Vaccine 0.1mg/1ml dispersion for injection multidose vials (Moderna, Inc)",
+            "type": "AMP"
+        },
+        "42023411000001109": {
+            "manufacturer": {
+                "display": "Moderna, Inc",
+                "eu": {
+                    "code": "ORG-100031184",
+                    "display": "Moderna Biotech Spain S.L"
+                }
+            },
+            "name": {
+                "display": "Spikevax",
+                "eu": {
+                    "code": "EU/1/20/1507",
+                    "display": "Spikevax"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42023311000001102",
+                    "type": "APM"
+                },
+                {
+                    "code": "42029111000001101",
+                    "type": "VMP"
+                }
+            ],
+            "term": "Spikevax XBB.1.5 COVID-19 mRNA Vaccine 0.1mg/1ml dispersion for injection multidose vials (Moderna, Inc) 2.5 ml",
+            "type": "AMPP"
+        },
+        "42023511000001108": {
+            "manufacturer": {
+                "display": "Moderna, Inc",
+                "eu": {
+                    "code": "ORG-100031184",
+                    "display": "Moderna Biotech Spain S.L"
+                }
+            },
+            "name": {
+                "display": "Spikevax",
+                "eu": {
+                    "code": "EU/1/20/1507",
+                    "display": "Spikevax"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42023311000001102",
+                    "type": "APM"
+                },
+                {
+                    "code": "42029111000001101",
+                    "type": "VMP"
+                }
+            ],
+            "term": "Spikevax XBB.1.5 COVID-19 mRNA Vaccine 0.1mg/1ml dispersion for injection multidose vials (Moderna, Inc) 25 ml 10 x 2.5ml vials",
+            "type": "AMPP"
+        },
+        "42029111000001101": {
+            "manufacturer": {
+                "display": "Moderna, Inc",
+                "eu": {
+                    "code": "ORG-100031184",
+                    "display": "Moderna Biotech Spain S.L"
+                }
+            },
+            "name": {
+                "display": "Spikevax",
+                "eu": {
+                    "code": "EU/1/20/1507",
+                    "display": "Spikevax"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42023311000001102",
+                    "type": "APM"
+                }
+            ],
+            "term": "Generic Spikevax XBB.1.5 COVID-19 mRNA Vaccine 0.1mg/1ml dispersion for injection multidose vials",
+            "type": "VMP"
+        },
+        "42029211000001107": {
+            "manufacturer": {
+                "display": "Pfizer Ltd",
+                "eu": {
+                    "code": "ORG-100030215",
+                    "display": "Biontech Manafacturing GmbH"
+                }
+            },
+            "name": {
+                "display": "Comirnaty",
+                "eu": {
+                    "code": "EU/1/20/1528",
+                    "display": "Comirnaty"
+                }
+            },
+            "rels": [
+                {
+                    "code": "42020711000001107",
+                    "type": "APM"
+                }
+            ],
+            "term": "Generic Comirnaty Omicron XBB.1.5 COVID-19 mRNA Vaccine 30micrograms/0.3ml dose dispersion for injection multidose vials",
+            "type": "VMP"
         }
     },
     "situations": {
         "1324721000000108": "SARS-CoV-2 (severe acute respiratory syndrome coronavirus 2) vaccination dose declined",
         "1324731000000105": "SARS-CoV-2 (severe acute respiratory syndrome coronavirus 2) immunisation course not indicated",
         "1324741000000101": "SARS-CoV-2 (severe acute respiratory syndrome coronavirus 2) vaccination first dose declined",
         "1324751000000103": "SARS-CoV-2 (severe acute respiratory syndrome coronavirus 2) vaccination second dose declined",
```

### Comparing `covid_19_terms-1.33.1/setup.py` & `covid_19_terms-1.34.1/setup.py`

 * *Files identical despite different names*

